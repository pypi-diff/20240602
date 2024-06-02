# Comparing `tmp/aligo-6.2.3.tar.gz` & `tmp/aligo-6.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aligo-6.2.3.tar", last modified: Wed May 29 07:58:47 2024, max compression
+gzip compressed data, was "aligo-6.2.4.tar", last modified: Sun Jun  2 06:38:02 2024, max compression
```

## Comparing `aligo-6.2.3.tar` & `aligo-6.2.4.tar`

### file list

```diff
@@ -1,219 +1,219 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:58:47.400884 aligo-6.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-29 07:58:42.000000 aligo-6.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7573 2024-05-29 07:58:47.400884 aligo-6.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-05-29 07:58:42.000000 aligo-6.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-29 07:58:42.000000 aligo-6.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-29 07:58:42.000000 aligo-6.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 07:58:47.400884 aligo-6.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:58:47.360883 aligo-6.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:58:47.364883 aligo-6.2.3/src/aligo/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-29 07:58:46.000000 aligo-6.2.3/src/aligo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:58:47.368883 aligo-6.2.3/src/aligo/apis/
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Album.py
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Aligo.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Compress.py
--rw-r--r--   0 runner    (1001) docker     (127)     4495 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/CustomShare.py
--rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Download.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Drive.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Duplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/File.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Move.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Other.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Recyclebin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Search.py
--rw-r--r--   0 runner    (1001) docker     (127)    23848 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Share.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Star.py
--rw-r--r--   0 runner    (1001) docker     (127)    17900 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/SyncFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Video.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:58:47.372883 aligo-6.2.3/src/aligo/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Album.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Audio.py
--rw-r--r--   0 runner    (1001) docker     (127)    20148 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/BaseAligo.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Compress.py
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Copy.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Core.py
--rw-r--r--   0 runner    (1001) docker     (127)    12871 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Create.py
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Download.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Drive.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Duplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/EMail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/File.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/LoginServer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Move.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Other.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Recyclebin.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/SBox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Search.py
--rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Share.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Star.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Template.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/User.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Video.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:58:47.372883 aligo-6.2.3/src/aligo/error/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/error/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:58:47.384883 aligo-6.2.3/src/aligo/request/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/AimSearchRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/AlbumListFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/AlbumListRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/ArchiveStatusRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/ArchiveUncompressRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/BatchCancelShareRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/BatchCopyFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/BatchDownloadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/BatchGetFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/BatchMoveFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/BatchMoveToTrashRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/BatchRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/BatchRestoreRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/BatchShareFileSaveToDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/BatchStarFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/BatchSubRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/CancelShareLinkRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/CompleteFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/CopyFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/CreateFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/CreateFolderRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/CreateShareLinkRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetAudioPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetDefaultDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetDownloadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetFileListRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetFilePathRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetRecycleBinListRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetShareFileListRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetShareFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetShareInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetShareLinkDownloadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetShareLinkListRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetShareLinkVideoPreviewPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetShareTokenRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetStarredListRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetUploadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetVideoPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetVideoPreviewPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/ListToCleanRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/MoveFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/MoveFileToTrashRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/PrivateShareRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/RenameFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/RestoreFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/SearchFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/SearchShareFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/ShareFileSaveToDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/StarredFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/TemplateRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/UpdateFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/UpdateShareLinkRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:58:47.392884 aligo-6.2.3/src/aligo/response/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/AimSearchResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/AlbumInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/AlbumListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/ArchiveStatusResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/ArchiveUncompressResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/BatchDownloadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/BatchShareFileSaveToDriveResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/BatchSubResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/CancelShareLinkResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/CopyFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/CreateFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/CreateShareLinkResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/DuplicateListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetAudioPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetDownloadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetFileListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetFilePathResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetOfficePreviewUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetPersonalInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetRecycleBinListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetShareFileListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetShareInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetShareLinkDownloadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetShareLinkListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetShareLinkVideoPreviewPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetShareTokenResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetStarredListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetUploadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetVideoPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetVideoPreviewPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/ListMyDrivesResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/ListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/ListToCleanResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/MoveFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/MoveFileToTrashResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/PrivateShareResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/RestoreFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/RewardSpaceResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/SearchFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/SearchShareFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/ShareFileSaveToDriveResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/ShareItemInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/ShareLinkExtractCodeResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/TemplateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/UpdateShareLinkResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/UsersVipInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:58:47.396884 aligo-6.2.3/src/aligo/types/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/AudioMeta.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/AudioMusicMeta.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/AudioTranscodeTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/BaseAlbum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/BaseDrive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/BaseFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/BaseShareFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/BaseUser.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/CroppingBoundary.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/CroppingSuggestionItem.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/DriveCapacityDetail.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/DriveFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/EMailConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/Enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/FaceThumbnail.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/FieldsInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/FolderSizeInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/ImageMedia.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/ImageQuality.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/ImageTag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/ListAlbumItem.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/LoginDevice.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/MediaTransCodeTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/Null.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/PersonalRightsInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/PersonalSpaceInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/Privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/RateLimit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/ShareLinkBaseFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/ShareLinkSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/SystemTag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/Type.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/UploadPartInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/UserConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/VideoMedia.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/VideoMediaAudioStream.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/VideoMediaVideoStream.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/VideoPreview.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/VideoPreviewPlayInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/VideoPreviewSprite.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/VideoTranscodeTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:58:47.396884 aligo-6.2.3/src/aligo/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/utils/LoginTimout.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:58:47.396884 aligo-6.2.3/src/aligo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7573 2024-05-29 07:58:47.000000 aligo-6.2.3/src/aligo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-05-29 07:58:47.000000 aligo-6.2.3/src/aligo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 07:58:47.000000 aligo-6.2.3/src/aligo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-29 07:58:47.000000 aligo-6.2.3/src/aligo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 07:58:47.000000 aligo-6.2.3/src/aligo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:38:02.071010 aligo-6.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-02 06:37:52.000000 aligo-6.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7573 2024-06-02 06:38:02.071010 aligo-6.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-06-02 06:37:52.000000 aligo-6.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-06-02 06:37:52.000000 aligo-6.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-06-02 06:37:52.000000 aligo-6.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-02 06:38:02.071010 aligo-6.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:38:02.035010 aligo-6.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:38:02.039010 aligo-6.2.4/src/aligo/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-06-02 06:38:00.000000 aligo-6.2.4/src/aligo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:38:02.043010 aligo-6.2.4/src/aligo/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/apis/Album.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4704 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/apis/Aligo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/apis/Audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/apis/Compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4495 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/apis/Copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/apis/Create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/apis/CustomShare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/apis/Download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/apis/Drive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/apis/Duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/apis/File.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/apis/Move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/apis/Other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/apis/Recyclebin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/apis/Search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23848 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/apis/Share.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/apis/Star.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17900 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/apis/SyncFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/apis/Update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/apis/Video.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:38:02.047010 aligo-6.2.4/src/aligo/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/Album.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/Audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20541 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/Auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10818 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/BaseAligo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/Compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/Config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/Copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/Core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12871 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/Create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/Download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/Drive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/Duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/EMail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/File.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/LoginServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/Move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/Other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/Recyclebin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/SBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/Search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/Share.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/Star.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/Template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/Update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/User.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/Video.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:38:02.047010 aligo-6.2.4/src/aligo/error/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/error/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:38:02.055010 aligo-6.2.4/src/aligo/request/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/AimSearchRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/AlbumListFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/AlbumListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/ArchiveStatusRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/ArchiveUncompressRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/BatchCancelShareRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/BatchCopyFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/BatchDownloadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/BatchGetFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/BatchMoveFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/BatchMoveToTrashRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/BatchRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/BatchRestoreRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/BatchShareFileSaveToDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/BatchStarFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/BatchSubRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/CancelShareLinkRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/CompleteFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/CopyFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/CreateFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/CreateFolderRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/CreateShareLinkRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/GetAudioPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/GetDefaultDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/GetDownloadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/GetDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/GetFileListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/GetFilePathRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/GetFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/GetRecycleBinListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/GetShareFileListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/GetShareFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/GetShareInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/GetShareLinkDownloadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/GetShareLinkListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/GetShareLinkVideoPreviewPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/GetShareTokenRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/GetStarredListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/GetUploadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/GetVideoPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/GetVideoPreviewPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/ListToCleanRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/MoveFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/MoveFileToTrashRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/PrivateShareRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/RenameFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/RestoreFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/SearchFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/SearchShareFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/ShareFileSaveToDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/StarredFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/TemplateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/UpdateFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/UpdateShareLinkRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/request/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:38:02.063010 aligo-6.2.4/src/aligo/response/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/AimSearchResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/AlbumInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/AlbumListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/ArchiveStatusResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/ArchiveUncompressResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/BatchDownloadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/BatchShareFileSaveToDriveResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/BatchSubResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/CancelShareLinkResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/CopyFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/CreateFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/CreateShareLinkResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/DuplicateListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/GetAudioPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/GetDownloadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/GetFileListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/GetFilePathResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/GetOfficePreviewUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/GetPersonalInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/GetRecycleBinListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/GetShareFileListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/GetShareInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/GetShareLinkDownloadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/GetShareLinkListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/GetShareLinkVideoPreviewPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/GetShareTokenResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/GetStarredListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/GetUploadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/GetVideoPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/GetVideoPreviewPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/ListMyDrivesResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/ListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/ListToCleanResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/MoveFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/MoveFileToTrashResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/PrivateShareResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/RestoreFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/RewardSpaceResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/SearchFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/SearchShareFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/ShareFileSaveToDriveResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/ShareItemInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/ShareLinkExtractCodeResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/TemplateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/UpdateShareLinkResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/UsersVipInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/response/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:38:02.071010 aligo-6.2.4/src/aligo/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/AudioMeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/AudioMusicMeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/AudioTranscodeTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/BaseAlbum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/BaseDrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/BaseFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/BaseShareFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/BaseUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/CroppingBoundary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/CroppingSuggestionItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/DriveCapacityDetail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/DriveFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/EMailConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/Enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/FaceThumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/FieldsInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/FolderSizeInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/ImageMedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/ImageQuality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/ImageTag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/ListAlbumItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/LoginDevice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/MediaTransCodeTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/Null.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/PersonalRightsInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/PersonalSpaceInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/Privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/RateLimit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/ShareLinkBaseFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/ShareLinkSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/SystemTag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/Type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/UploadPartInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/UserConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/VideoMedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/VideoMediaAudioStream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/VideoMediaVideoStream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/VideoPreview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/VideoPreviewPlayInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/VideoPreviewSprite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/VideoTranscodeTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:38:02.071010 aligo-6.2.4/src/aligo/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/utils/LoginTimout.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-02 06:37:52.000000 aligo-6.2.4/src/aligo/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-02 06:38:02.071010 aligo-6.2.4/src/aligo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7573 2024-06-02 06:38:02.000000 aligo-6.2.4/src/aligo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-06-02 06:38:02.000000 aligo-6.2.4/src/aligo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-02 06:38:02.000000 aligo-6.2.4/src/aligo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-06-02 06:38:02.000000 aligo-6.2.4/src/aligo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-02 06:38:02.000000 aligo-6.2.4/src/aligo.egg-info/top_level.txt
```

### Comparing `aligo-6.2.3/LICENSE` & `aligo-6.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/PKG-INFO` & `aligo-6.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aligo
-Version: 6.2.3
+Version: 6.2.4
 Summary: aliyun drive sdk
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/aligo
 Project-URL: Homepage, https://github.com/foyoux/aligo
 Project-URL: Bug Tracker, https://github.com/foyoux/aligo/issues
 Keywords: aligo
 Classifier: Programming Language :: Python
```

### Comparing `aligo-6.2.3/README.md` & `aligo-6.2.4/README.md`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/pyproject.toml` & `aligo-6.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/apis/Album.py` & `aligo-6.2.4/src/aligo/apis/Album.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/apis/Aligo.py` & `aligo-6.2.4/src/aligo/apis/Aligo.py`

 * *Files 9% similar despite different names*

```diff
@@ -58,15 +58,16 @@
             use_aria2: bool = False,
             proxies: Dict = None,
             port: int = None,
             email: EMailConfig = None,
             request_failed_delay: float = 3,
             requests_timeout: float = None,
             login_timeout: float = None,
-            re_login: bool = True
+            re_login: bool = True,
+            request_interval: int = 0,
     ):
         """
         Aligo
         :param name: (可选, 默认: aligo) 配置文件名称, 便于使用不同配置文件进行身份验证
         :param refresh_token:
         :param show: (可选) 显示二维码的函数
         :param level: (可选) 控制控制台输出
@@ -74,14 +75,15 @@
         :param proxies: (可选) 自定义代理 [proxies={"https":"localhost:10809"}],支持 http 和 socks5（具体参考requests库的用法）
         :param port: (可选) 开启 http server 端口，用于网页端扫码登录. 提供此值时，将不再弹出或打印二维码
         :param email: (可选) 邮箱配置，参考 EMailConfig
         :param request_failed_delay: (可选) 由于网络异常导致的 request 异常，等待多少秒后重试
         :param requests_timeout: (可选) 应网友提议，添加 requests timeout 参数
         :param login_timeout: (可选) 登录超时时间，单位：秒。
         :param re_login: refresh_token 失效后是否继续登录（弹出二维码或邮件，需等待） fix #73
+        :param request_interval: 每次请求等待的时间，避免请求频繁触发风控
 
         level, use_aria2, proxies, port, email 可以通过 配置文件 配置默认值，在 <用户家目录>/.aligo/config.json5 中
         ```json5
         {
           "level": 10,
           "use_aria2": false,
           "proxies": {
@@ -93,39 +95,42 @@
         }
         ```
         """
         config = aligo_config_folder / 'config.json5'
         if config.exists():
             config = json.loads(config.read_text(encoding='utf8'))
             if level == logging.DEBUG and 'level' in config:
-                level = config.get('level')
+                level = config.get('level', level)
             if not use_aria2:
-                use_aria2 = config.get('use_aria2')
+                use_aria2 = config.get('use_aria2', use_aria2)
             if proxies is None:
-                proxies = config.get('proxies')
+                proxies = config.get('proxies', proxies)
             if port is None:
-                port = config.get('port')
+                port = config.get('port', port)
             if email is None:
-                email = config.get('email')
+                email = config.get('email', email)
             if request_failed_delay == 3:
                 requests_timeout = config.get('request_failed_delay', 3)
             if requests_timeout is None:
-                requests_timeout = config.get('requests_timeout')
-            if requests_timeout is None:
-                login_timeout = config.get('login_timeout')
+                requests_timeout = config.get('requests_timeout', requests_timeout)
+            if login_timeout is None:
+                login_timeout = config.get('login_timeout', login_timeout)
             if re_login is True:
-                re_login = config.get('re_login')
+                re_login = config.get('re_login', re_login)
+            if request_interval is True:
+                request_interval = config.get('request_interval', request_interval)
 
         super().__init__(
             name,
             refresh_token,
             show,
             level,
             use_aria2,
             proxies,
             port,
             email,
             request_failed_delay,
             requests_timeout,
             login_timeout,
             re_login,
+            request_interval,
         )
```

### Comparing `aligo-6.2.3/src/aligo/apis/Audio.py` & `aligo-6.2.4/src/aligo/apis/Audio.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/apis/Compress.py` & `aligo-6.2.4/src/aligo/apis/Compress.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/apis/Copy.py` & `aligo-6.2.4/src/aligo/apis/Copy.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/apis/Create.py` & `aligo-6.2.4/src/aligo/apis/Create.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/apis/CustomShare.py` & `aligo-6.2.4/src/aligo/apis/CustomShare.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/apis/Download.py` & `aligo-6.2.4/src/aligo/apis/Download.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/apis/Drive.py` & `aligo-6.2.4/src/aligo/apis/Drive.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/apis/Duplicate.py` & `aligo-6.2.4/src/aligo/apis/Duplicate.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/apis/File.py` & `aligo-6.2.4/src/aligo/apis/File.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/apis/Move.py` & `aligo-6.2.4/src/aligo/apis/Move.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/apis/Other.py` & `aligo-6.2.4/src/aligo/apis/Other.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/apis/Recyclebin.py` & `aligo-6.2.4/src/aligo/apis/Recyclebin.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/apis/Search.py` & `aligo-6.2.4/src/aligo/apis/Search.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/apis/Share.py` & `aligo-6.2.4/src/aligo/apis/Share.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/apis/Star.py` & `aligo-6.2.4/src/aligo/apis/Star.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/apis/SyncFolder.py` & `aligo-6.2.4/src/aligo/apis/SyncFolder.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/apis/Update.py` & `aligo-6.2.4/src/aligo/apis/Update.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/apis/Video.py` & `aligo-6.2.4/src/aligo/apis/Video.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/core/Album.py` & `aligo-6.2.4/src/aligo/core/Album.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/core/Audio.py` & `aligo-6.2.4/src/aligo/core/Audio.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/core/Auth.py` & `aligo-6.2.4/src/aligo/core/Auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,28 +84,30 @@
             show: Callable[[str], None] = None,
             level=logging.DEBUG,
             proxies: Dict = None,
             port: int = None,
             email: EMailConfig = None,
             request_failed_delay: float = 3,
             requests_timeout: float = None,
+            request_interval: int = 0,
     ):
         """扫描二维码登录"""
 
     @overload
     def __init__(
             self,
             name: str = 'aligo',
             refresh_token: str = None,
             level=logging.DEBUG,
             proxies: Dict = None,
             port: int = None,
             email: EMailConfig = None,
             request_failed_delay: float = 3,
             requests_timeout: float = None,
+            request_interval: int = 0,
     ):
         """refresh_token 登录"""
 
     @overload
     def __init__(
             self, name: str = 'aligo',
             refresh_token: str = None,
@@ -114,14 +116,15 @@
             proxies: Dict = None,
             port: int = None,
             email: EMailConfig = None,
             request_failed_delay: float = 3,
             requests_timeout: float = None,
             login_timeout: float = None,
             re_login: bool = True,
+            request_interval: int = 0,
     ):
         """..."""
 
     # noinspection PyPep8Naming,SpellCheckingInspection
     def __init__(
             self, name: str = 'aligo',
             refresh_token: str = None,
@@ -130,39 +133,42 @@
             proxies: Dict = None,
             port: int = None,
             email: EMailConfig = None,
             request_failed_delay: float = 3,
             requests_timeout: float = None,
             login_timeout: float = None,
             re_login: bool = True,
+            request_interval: int = 0,
     ):
         """登录验证
 
         :param name: (可选, 默认: aligo) 配置文件名称, 便于使用不同配置文件进行身份验证
         :param refresh_token:
         :param show: (可选) 显示二维码的函数
         :param level: (可选) 控制控制台输出
         :param proxies: (可选) 自定义代理 [proxies={"https":"localhost:10809"}],支持 http 和 socks5（具体参考requests库的用法）
         :param port: (可选) 开启 http server 端口，用于网页端扫码登录. 提供此值时，将不再弹出或打印二维码
         :param email: (可选) 邮箱配置，参考 EMailConfig
         :param request_failed_delay: 请求失败后，延迟时间，单位：秒
         :param requests_timeout: same as requests timeout
         :param login_timeout: 登录超时时间，单位：秒
         :param re_login: refresh_token 失效后是否继续登录（弹出二维码或邮件，需等待） fix #73
+        :param request_interval: 每次请求等待的时间，避免请求频繁触发风控
         """
         self._name_name = name
         self._name = aligo_config_folder.joinpath(f'{name}.json')
         self._port = port
         self._webServer: HTTPServer = None  # type: ignore
         self._email = email
         self.log = logging.getLogger(name)
         self._request_failed_delay = request_failed_delay
         self._requests_timeout = requests_timeout
         self._login_timeout = LoginTimeout(login_timeout)
         self._re_login = re_login
+        self._request_interval = request_interval
 
         fmt = f'%(asctime)s.%(msecs)03d {name}.%(levelname)s %(message)s'
 
         coloredlogs.install(
             level=level,
             logger=self.log,
             milliseconds=True,
@@ -370,14 +376,18 @@
                     self._login()
                 else:
                     raise AligoRefreshFailed('使用 refresh_token 刷新 token 失败，re_login=False，不继续登录')
 
     def request(self, method: str, url: str, params: Dict = None,
                 headers: Dict = None, data=None, body: Dict = None) -> requests.Response:
         """统一请求方法"""
+        #
+        if self._request_interval:
+            time.sleep(self._request_interval)
+
         # 删除值为None的键
         if body is not None:
             body = {k: v for k, v in body.items() if v is not None}
 
         if data is not None and isinstance(data, dict):
             data = {k: v for k, v in data.items() if v is not None}
```

### Comparing `aligo-6.2.3/src/aligo/core/BaseAligo.py` & `aligo-6.2.4/src/aligo/core/BaseAligo.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,16 @@
             use_aria2: bool = False,
             proxies: Dict = None,
             port: int = None,
             email: EMailConfig = None,
             request_failed_delay: float = 3,
             requests_timeout: float = None,
             login_timeout: float = None,
-            re_login: bool = True
+            re_login: bool = True,
+            request_interval: int = 0,
     ):
         """
         BaseAligo
         :param name: (可选, 默认: aligo) 配置文件名称, 便于使用不同配置文件进行身份验证
         :param refresh_token:
         :param show: (可选) 显示二维码的函数
         :param level: (可选) 控制控制台输出
@@ -44,27 +45,29 @@
         :param proxies: (可选) 自定义代理 [proxies={"https":"localhost:10809"}],支持 http 和 socks5（具体参考requests库的用法）
         :param port: (可选) 开启 http server 端口，用于网页端扫码登录. 提供此值时，将不再弹出或打印二维码
         :param email: (可选) 邮箱配置，参考 EMailConfig
         :param request_failed_delay: 请求失败后，延迟时间，单位：秒
         :param requests_timeout: same as requests timeout
         :param login_timeout: 登录超时时间，单位：秒
         :param re_login: refresh_token 失效后是否继续登录（弹出二维码或邮件，需等待） fix #73
+        :param request_interval: 每次请求等待的时间，避免请求频繁触发风控
         """
         self._auth = Auth(
             name=name,
             refresh_token=refresh_token,
             show=show,
             level=level,
             proxies=proxies,
             port=port,
             email=email,
             request_failed_delay=request_failed_delay,
             requests_timeout=requests_timeout,
             login_timeout=login_timeout,
             re_login=re_login,
+            request_interval=request_interval,
         )
         # 因为 self._auth.session 没有被重新赋值, 所以可以这么用
         self._session: requests.Session = self._auth.session
         # 在刷新 token 时, self._auth.token 被重新赋值, 而 self._token 却不会被更新
         # self._token: Token = self._auth.token
         self._user: Optional[BaseUser] = None
         self._personal_info: Optional[GetPersonalInfoResponse] = None
```

### Comparing `aligo-6.2.3/src/aligo/core/Compress.py` & `aligo-6.2.4/src/aligo/core/Compress.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/core/Config.py` & `aligo-6.2.4/src/aligo/core/Config.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/core/Copy.py` & `aligo-6.2.4/src/aligo/core/Copy.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/core/Core.py` & `aligo-6.2.4/src/aligo/core/Core.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/core/Create.py` & `aligo-6.2.4/src/aligo/core/Create.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/core/Download.py` & `aligo-6.2.4/src/aligo/core/Download.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/core/Drive.py` & `aligo-6.2.4/src/aligo/core/Drive.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/core/Duplicate.py` & `aligo-6.2.4/src/aligo/core/Duplicate.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/core/EMail.py` & `aligo-6.2.4/src/aligo/core/EMail.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/core/File.py` & `aligo-6.2.4/src/aligo/core/File.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/core/LoginServer.py` & `aligo-6.2.4/src/aligo/core/LoginServer.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/core/Move.py` & `aligo-6.2.4/src/aligo/core/Move.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/core/Other.py` & `aligo-6.2.4/src/aligo/core/Other.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/core/Recyclebin.py` & `aligo-6.2.4/src/aligo/core/Recyclebin.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/core/SBox.py` & `aligo-6.2.4/src/aligo/core/SBox.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/core/Search.py` & `aligo-6.2.4/src/aligo/core/Search.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/core/Share.py` & `aligo-6.2.4/src/aligo/core/Share.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/core/Star.py` & `aligo-6.2.4/src/aligo/core/Star.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/core/Update.py` & `aligo-6.2.4/src/aligo/core/Update.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/core/User.py` & `aligo-6.2.4/src/aligo/core/User.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/core/Video.py` & `aligo-6.2.4/src/aligo/core/Video.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/request/AlbumListFilesRequest.py` & `aligo-6.2.4/src/aligo/request/AlbumListFilesRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/request/CreateFileRequest.py` & `aligo-6.2.4/src/aligo/request/CreateFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/request/CreateShareLinkRequest.py` & `aligo-6.2.4/src/aligo/request/CreateShareLinkRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/request/GetFileListRequest.py` & `aligo-6.2.4/src/aligo/request/GetFileListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/request/GetFileRequest.py` & `aligo-6.2.4/src/aligo/request/GetFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/request/GetRecycleBinListRequest.py` & `aligo-6.2.4/src/aligo/request/GetRecycleBinListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/request/GetShareFileListRequest.py` & `aligo-6.2.4/src/aligo/request/GetShareFileListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/request/GetShareLinkDownloadUrlRequest.py` & `aligo-6.2.4/src/aligo/request/GetShareLinkDownloadUrlRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/request/GetShareLinkListRequest.py` & `aligo-6.2.4/src/aligo/request/GetShareLinkListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/request/GetStarredListRequest.py` & `aligo-6.2.4/src/aligo/request/GetStarredListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/request/SearchFileRequest.py` & `aligo-6.2.4/src/aligo/request/SearchFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/request/UpdateFileRequest.py` & `aligo-6.2.4/src/aligo/request/UpdateFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/request/UpdateShareLinkRequest.py` & `aligo-6.2.4/src/aligo/request/UpdateShareLinkRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/request/__init__.py` & `aligo-6.2.4/src/aligo/request/__init__.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/response/CreateFileResponse.py` & `aligo-6.2.4/src/aligo/response/CreateFileResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/response/CreateShareLinkResponse.py` & `aligo-6.2.4/src/aligo/response/CreateShareLinkResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/response/DuplicateListResponse.py` & `aligo-6.2.4/src/aligo/response/DuplicateListResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/response/GetDownloadUrlResponse.py` & `aligo-6.2.4/src/aligo/response/GetDownloadUrlResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/response/GetShareInfoResponse.py` & `aligo-6.2.4/src/aligo/response/GetShareInfoResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/response/GetShareLinkVideoPreviewPlayInfoResponse.py` & `aligo-6.2.4/src/aligo/response/GetShareLinkVideoPreviewPlayInfoResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/response/GetShareTokenResponse.py` & `aligo-6.2.4/src/aligo/response/GetShareTokenResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/response/UpdateShareLinkResponse.py` & `aligo-6.2.4/src/aligo/response/UpdateShareLinkResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/response/__init__.py` & `aligo-6.2.4/src/aligo/response/__init__.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/types/BaseAlbum.py` & `aligo-6.2.4/src/aligo/types/BaseAlbum.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/types/BaseDrive.py` & `aligo-6.2.4/src/aligo/types/BaseDrive.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/types/BaseFile.py` & `aligo-6.2.4/src/aligo/types/BaseFile.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/types/BaseShareFile.py` & `aligo-6.2.4/src/aligo/types/BaseShareFile.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/types/BaseUser.py` & `aligo-6.2.4/src/aligo/types/BaseUser.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/types/Enum.py` & `aligo-6.2.4/src/aligo/types/Enum.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/types/ImageMedia.py` & `aligo-6.2.4/src/aligo/types/ImageMedia.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/types/ListAlbumItem.py` & `aligo-6.2.4/src/aligo/types/ListAlbumItem.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/types/Null.py` & `aligo-6.2.4/src/aligo/types/Null.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/types/ShareLinkBaseFile.py` & `aligo-6.2.4/src/aligo/types/ShareLinkBaseFile.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/types/ShareLinkSchema.py` & `aligo-6.2.4/src/aligo/types/ShareLinkSchema.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/types/Token.py` & `aligo-6.2.4/src/aligo/types/Token.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/types/UserConfig.py` & `aligo-6.2.4/src/aligo/types/UserConfig.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/types/VideoMedia.py` & `aligo-6.2.4/src/aligo/types/VideoMedia.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/types/VideoPreview.py` & `aligo-6.2.4/src/aligo/types/VideoPreview.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/types/VideoPreviewPlayInfo.py` & `aligo-6.2.4/src/aligo/types/VideoPreviewPlayInfo.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo/types/__init__.py` & `aligo-6.2.4/src/aligo/types/__init__.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.3/src/aligo.egg-info/PKG-INFO` & `aligo-6.2.4/src/aligo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aligo
-Version: 6.2.3
+Version: 6.2.4
 Summary: aliyun drive sdk
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/aligo
 Project-URL: Homepage, https://github.com/foyoux/aligo
 Project-URL: Bug Tracker, https://github.com/foyoux/aligo/issues
 Keywords: aligo
 Classifier: Programming Language :: Python
```

### Comparing `aligo-6.2.3/src/aligo.egg-info/SOURCES.txt` & `aligo-6.2.4/src/aligo.egg-info/SOURCES.txt`

 * *Files identical despite different names*


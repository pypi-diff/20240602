# Comparing `tmp/outline_python_api-0.0.1a0.tar.gz` & `tmp/outline_python_api-0.1.0a0.tar.gz`

## Comparing `outline_python_api-0.0.1a0.tar` & `outline_python_api-0.1.0a0.tar`

### file list

```diff
@@ -1,146 +1,146 @@
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/__init__.py
--rw-r--r--   0        0        0    64424 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/_base_client.py
--rw-r--r--   0        0        0    19287 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/_constants.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/_files.py
--rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/_qs.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/_resource.py
--rw-r--r--   0        0        0    28381 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/_response.py
--rw-r--r--   0        0        0    10104 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/_streaming.py
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/_types.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/_utils/__init__.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/lib/.keep
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/resources/__init__.py
--rw-r--r--   0        0        0    13094 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/resources/attachments.py
--rw-r--r--   0        0        0     5898 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/resources/auth.py
--rw-r--r--   0        0        0    16258 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/resources/comments.py
--rw-r--r--   0        0        0    72703 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/resources/documents.py
--rw-r--r--   0        0        0     7696 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/resources/events.py
--rw-r--r--   0        0        0    16595 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/resources/file_operations.py
--rw-r--r--   0        0        0    17935 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/resources/groups.py
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/resources/collections/__init__.py
--rw-r--r--   0        0        0    48231 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/resources/collections/collections.py
--rw-r--r--   0        0        0     6714 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/resources/collections/group_memberships.py
--rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/resources/collections/memberships.py
--rw-r--r--   0        0        0     8352 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/__init__.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/attachment_create_params.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/attachment_create_response.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/attachment_delete_params.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/attachment_delete_response.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/attachment_redirect_params.py
--rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/auth.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/auth_config_response.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/auth_info_response.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collection.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collection_add_group_params.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collection_add_group_response.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collection_add_user_params.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collection_add_user_response.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collection_create_params.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collection_create_response.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collection_delete_params.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collection_delete_response.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collection_documents_params.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collection_documents_response.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collection_export_all_params.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collection_export_all_response.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collection_export_params.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collection_export_response.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collection_list_params.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collection_list_response.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collection_remove_group_params.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collection_remove_group_response.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collection_remove_user_params.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collection_remove_user_response.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collection_retrieve_params.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collection_retrieve_response.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collection_update_params.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collection_update_response.py
--rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/comment.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/comment_create_params.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/comment_create_response.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/comment_delete_params.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/comment_delete_response.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/comment_list_params.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/comment_list_response.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/comment_update_params.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/comment_update_response.py
--rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_archive_params.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_archive_response.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_create_params.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_create_response.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_delete_params.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_delete_response.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_drafts_params.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_drafts_response.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_export_params.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_export_response.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_import_params.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_import_response.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_info_params.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_info_response.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_list_params.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_list_response.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_move_params.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_move_response.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_restore_params.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_restore_response.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_search_params.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_search_response.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_star_params.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_star_response.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_templatize_params.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_templatize_response.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_unpublish_params.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_unpublish_response.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_unstar_params.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_unstar_response.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_update_params.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_update_response.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_viewed_params.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/document_viewed_response.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/event_create_params.py
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/event_create_response.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/file_operation.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/file_operation_delete_params.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/file_operation_delete_response.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/file_operation_info_params.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/file_operation_info_response.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/file_operation_list_params.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/file_operation_list_response.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/file_operation_redirect_params.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/group.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/group_create_params.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/group_create_response.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/group_delete_params.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/group_delete_response.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/group_info_params.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/group_info_response.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/group_list_params.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/group_list_response.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/group_update_params.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/group_update_response.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collections/__init__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collections/group_membership_list_params.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collections/group_membership_list_response.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collections/membership_list_params.py
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/collections/membership_list_response.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/shared/__init__.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/src/outline/types/shared/pagination.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/.gitignore
--rw-r--r--   0        0        0    11337 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/LICENSE
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/pyproject.toml
--rw-r--r--   0        0        0    11884 2020-02-02 00:00:00.000000 outline_python_api-0.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/__init__.py
+-rw-r--r--   0        0        0    64424 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/_base_client.py
+-rw-r--r--   0        0        0    19287 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/_constants.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/_qs.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/_resource.py
+-rw-r--r--   0        0        0    28381 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/_response.py
+-rw-r--r--   0        0        0    10104 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/_streaming.py
+-rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/_types.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/_utils/__init__.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/_utils/_typing.py
+-rw-r--r--   0        0        0    11447 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/lib/.keep
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/resources/__init__.py
+-rw-r--r--   0        0        0    13094 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/resources/attachments.py
+-rw-r--r--   0        0        0     5898 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/resources/auth.py
+-rw-r--r--   0        0        0    16258 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/resources/comments.py
+-rw-r--r--   0        0        0    72703 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/resources/documents.py
+-rw-r--r--   0        0        0     7696 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/resources/events.py
+-rw-r--r--   0        0        0    16595 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/resources/file_operations.py
+-rw-r--r--   0        0        0    17935 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/resources/groups.py
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/resources/collections/__init__.py
+-rw-r--r--   0        0        0    48231 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/resources/collections/collections.py
+-rw-r--r--   0        0        0     6714 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/resources/collections/group_memberships.py
+-rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/resources/collections/memberships.py
+-rw-r--r--   0        0        0     8352 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/__init__.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/attachment_create_params.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/attachment_create_response.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/attachment_delete_params.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/attachment_delete_response.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/attachment_redirect_params.py
+-rw-r--r--   0        0        0     4232 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/auth.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/auth_config_response.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/auth_info_response.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collection.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collection_add_group_params.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collection_add_group_response.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collection_add_user_params.py
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collection_add_user_response.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collection_create_params.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collection_create_response.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collection_delete_params.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collection_delete_response.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collection_documents_params.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collection_documents_response.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collection_export_all_params.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collection_export_all_response.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collection_export_params.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collection_export_response.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collection_list_params.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collection_list_response.py
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collection_remove_group_params.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collection_remove_group_response.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collection_remove_user_params.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collection_remove_user_response.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collection_retrieve_params.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collection_retrieve_response.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collection_update_params.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collection_update_response.py
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/comment.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/comment_create_params.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/comment_create_response.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/comment_delete_params.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/comment_delete_response.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/comment_list_params.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/comment_list_response.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/comment_update_params.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/comment_update_response.py
+-rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_archive_params.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_archive_response.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_create_params.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_create_response.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_delete_params.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_delete_response.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_drafts_params.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_drafts_response.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_export_params.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_export_response.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_import_params.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_import_response.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_info_params.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_info_response.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_list_params.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_list_response.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_move_params.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_move_response.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_restore_params.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_restore_response.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_search_params.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_search_response.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_star_params.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_star_response.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_templatize_params.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_templatize_response.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_unpublish_params.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_unpublish_response.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_unstar_params.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_unstar_response.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_update_params.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_update_response.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_viewed_params.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/document_viewed_response.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/event_create_params.py
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/event_create_response.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/file_operation.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/file_operation_delete_params.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/file_operation_delete_response.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/file_operation_info_params.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/file_operation_info_response.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/file_operation_list_params.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/file_operation_list_response.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/file_operation_redirect_params.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/group.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/group_create_params.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/group_create_response.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/group_delete_params.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/group_delete_response.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/group_info_params.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/group_info_response.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/group_list_params.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/group_list_response.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/group_update_params.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/group_update_response.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collections/__init__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collections/group_membership_list_params.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collections/group_membership_list_response.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collections/membership_list_params.py
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/collections/membership_list_response.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/shared/__init__.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/src/outline/types/shared/pagination.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/.gitignore
+-rw-r--r--   0        0        0    11337 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/LICENSE
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/pyproject.toml
+-rw-r--r--   0        0        0    11884 2020-02-02 00:00:00.000000 outline_python_api-0.1.0a0/PKG-INFO
```

### Comparing `outline_python_api-0.0.1a0/src/outline/__init__.py` & `outline_python_api-0.1.0a0/src/outline/__init__.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/_base_client.py` & `outline_python_api-0.1.0a0/src/outline/_base_client.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/_client.py` & `outline_python_api-0.1.0a0/src/outline/_client.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/_compat.py` & `outline_python_api-0.1.0a0/src/outline/_compat.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/_exceptions.py` & `outline_python_api-0.1.0a0/src/outline/_exceptions.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/_files.py` & `outline_python_api-0.1.0a0/src/outline/_files.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/_models.py` & `outline_python_api-0.1.0a0/src/outline/_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     get_model_config,
     get_model_fields,
     field_get_default,
 )
 from ._constants import RAW_RESPONSE_HEADER
 
 if TYPE_CHECKING:
-    from pydantic_core.core_schema import ModelField, ModelFieldsSchema
+    from pydantic_core.core_schema import ModelField, LiteralSchema, ModelFieldsSchema
 
 __all__ = ["BaseModel", "GenericModel"]
 
 _T = TypeVar("_T")
 
 
 @runtime_checkable
@@ -247,15 +247,17 @@
             include: IncEx = None,
             exclude: IncEx = None,
             by_alias: bool = False,
             exclude_unset: bool = False,
             exclude_defaults: bool = False,
             exclude_none: bool = False,
             round_trip: bool = False,
-            warnings: bool = True,
+            warnings: bool | Literal["none", "warn", "error"] = True,
+            context: dict[str, Any] | None = None,
+            serialize_as_any: bool = False,
         ) -> dict[str, Any]:
             """Usage docs: https://docs.pydantic.dev/2.4/concepts/serialization/#modelmodel_dump
 
             Generate a dictionary representation of the model, optionally specifying which fields to include or exclude.
 
             Args:
                 mode: The mode in which `to_python` should run.
@@ -275,14 +277,18 @@
             """
             if mode != "python":
                 raise ValueError("mode is only supported in Pydantic v2")
             if round_trip != False:
                 raise ValueError("round_trip is only supported in Pydantic v2")
             if warnings != True:
                 raise ValueError("warnings is only supported in Pydantic v2")
+            if context is not None:
+                raise ValueError("context is only supported in Pydantic v2")
+            if serialize_as_any != False:
+                raise ValueError("serialize_as_any is only supported in Pydantic v2")
             return super().dict(  # pyright: ignore[reportDeprecated]
                 include=include,
                 exclude=exclude,
                 by_alias=by_alias,
                 exclude_unset=exclude_unset,
                 exclude_defaults=exclude_defaults,
                 exclude_none=exclude_none,
@@ -296,15 +302,17 @@
             include: IncEx = None,
             exclude: IncEx = None,
             by_alias: bool = False,
             exclude_unset: bool = False,
             exclude_defaults: bool = False,
             exclude_none: bool = False,
             round_trip: bool = False,
-            warnings: bool = True,
+            warnings: bool | Literal["none", "warn", "error"] = True,
+            context: dict[str, Any] | None = None,
+            serialize_as_any: bool = False,
         ) -> str:
             """Usage docs: https://docs.pydantic.dev/2.4/concepts/serialization/#modelmodel_dump_json
 
             Generates a JSON representation of the model using Pydantic's `to_json` method.
 
             Args:
                 indent: Indentation to use in the JSON output. If None is passed, the output will be compact.
@@ -320,14 +328,18 @@
             Returns:
                 A JSON string representation of the model.
             """
             if round_trip != False:
                 raise ValueError("round_trip is only supported in Pydantic v2")
             if warnings != True:
                 raise ValueError("warnings is only supported in Pydantic v2")
+            if context is not None:
+                raise ValueError("context is only supported in Pydantic v2")
+            if serialize_as_any != False:
+                raise ValueError("serialize_as_any is only supported in Pydantic v2")
             return super().json(  # type: ignore[reportDeprecated]
                 indent=indent,
                 include=include,
                 exclude=exclude,
                 by_alias=by_alias,
                 exclude_unset=exclude_unset,
                 exclude_defaults=exclude_defaults,
@@ -546,15 +558,15 @@
 
                 # Note: if one variant defines an alias then they all should
                 discriminator_alias = field.get("serialization_alias")
 
                 field_schema = field["schema"]
 
                 if field_schema["type"] == "literal":
-                    for entry in field_schema["expected"]:
+                    for entry in cast("LiteralSchema", field_schema)["expected"]:
                         if isinstance(entry, str):
                             mapping[entry] = variant
             else:
                 field_info = cast("dict[str, FieldInfo]", variant.__fields__).get(discriminator_field_name)  # pyright: ignore[reportDeprecated, reportUnnecessaryCast]
                 if not field_info:
                     continue
```

### Comparing `outline_python_api-0.0.1a0/src/outline/_qs.py` & `outline_python_api-0.1.0a0/src/outline/_qs.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/_resource.py` & `outline_python_api-0.1.0a0/src/outline/_resource.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/_response.py` & `outline_python_api-0.1.0a0/src/outline/_response.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/_streaming.py` & `outline_python_api-0.1.0a0/src/outline/_streaming.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/_types.py` & `outline_python_api-0.1.0a0/src/outline/_types.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/_utils/__init__.py` & `outline_python_api-0.1.0a0/src/outline/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/_utils/_logs.py` & `outline_python_api-0.1.0a0/src/outline/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/_utils/_proxy.py` & `outline_python_api-0.1.0a0/src/outline/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/_utils/_sync.py` & `outline_python_api-0.1.0a0/src/outline/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/_utils/_transform.py` & `outline_python_api-0.1.0a0/src/outline/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/_utils/_typing.py` & `outline_python_api-0.1.0a0/src/outline/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/_utils/_utils.py` & `outline_python_api-0.1.0a0/src/outline/_utils/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     overload,
 )
 from pathlib import Path
 from typing_extensions import TypeGuard
 
 import sniffio
 
-from .._types import Headers, NotGiven, FileTypes, NotGivenOr, HeadersLike
+from .._types import NotGiven, FileTypes, NotGivenOr, HeadersLike
 from .._compat import parse_date as parse_date, parse_datetime as parse_datetime
 
 _T = TypeVar("_T")
 _TupleT = TypeVar("_TupleT", bound=Tuple[object, ...])
 _MappingT = TypeVar("_MappingT", bound=Mapping[str, object])
 _SequenceT = TypeVar("_SequenceT", bound=Sequence[object])
 CallableT = TypeVar("CallableT", bound=Callable[..., Any])
@@ -366,15 +366,14 @@
     file_name = os.path.basename(path)
     return (file_name, contents)
 
 
 def get_required_header(headers: HeadersLike, header: str) -> str:
     lower_header = header.lower()
     if isinstance(headers, Mapping):
-        headers = cast(Headers, headers)
         for k, v in headers.items():
             if k.lower() == lower_header and isinstance(v, str):
                 return v
 
     """ to deal with the case where the header looks like Stainless-Event-Id """
     intercaps_header = re.sub(r"([^\w])(\w)", lambda pat: pat.group(1) + pat.group(2).upper(), header.capitalize())
```

### Comparing `outline_python_api-0.0.1a0/src/outline/resources/__init__.py` & `outline_python_api-0.1.0a0/src/outline/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/resources/attachments.py` & `outline_python_api-0.1.0a0/src/outline/resources/attachments.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/resources/auth.py` & `outline_python_api-0.1.0a0/src/outline/resources/auth.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/resources/comments.py` & `outline_python_api-0.1.0a0/src/outline/resources/comments.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/resources/documents.py` & `outline_python_api-0.1.0a0/src/outline/resources/documents.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/resources/events.py` & `outline_python_api-0.1.0a0/src/outline/resources/events.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/resources/file_operations.py` & `outline_python_api-0.1.0a0/src/outline/resources/file_operations.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/resources/groups.py` & `outline_python_api-0.1.0a0/src/outline/resources/groups.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/resources/collections/__init__.py` & `outline_python_api-0.1.0a0/src/outline/resources/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/resources/collections/collections.py` & `outline_python_api-0.1.0a0/src/outline/resources/collections/collections.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/resources/collections/group_memberships.py` & `outline_python_api-0.1.0a0/src/outline/resources/collections/group_memberships.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/resources/collections/memberships.py` & `outline_python_api-0.1.0a0/src/outline/resources/collections/memberships.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/__init__.py` & `outline_python_api-0.1.0a0/src/outline/types/__init__.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/attachment_create_params.py` & `outline_python_api-0.1.0a0/src/outline/types/attachment_create_params.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/attachment_create_response.py` & `outline_python_api-0.1.0a0/src/outline/types/attachment_create_response.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/auth.py` & `outline_python_api-0.1.0a0/src/outline/types/auth.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/auth_config_response.py` & `outline_python_api-0.1.0a0/src/outline/types/auth_config_response.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/collection.py` & `outline_python_api-0.1.0a0/src/outline/types/collection.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/collection_add_group_response.py` & `outline_python_api-0.1.0a0/src/outline/types/collection_add_group_response.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/collection_add_user_response.py` & `outline_python_api-0.1.0a0/src/outline/types/collection_add_user_response.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/collection_create_response.py` & `outline_python_api-0.1.0a0/src/outline/types/collection_create_response.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/collection_documents_response.py` & `outline_python_api-0.1.0a0/src/outline/types/collection_documents_response.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/collection_update_response.py` & `outline_python_api-0.1.0a0/src/outline/types/collection_update_response.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/comment.py` & `outline_python_api-0.1.0a0/src/outline/types/comment.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/comment_list_params.py` & `outline_python_api-0.1.0a0/src/outline/types/comment_list_params.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/comment_list_response.py` & `outline_python_api-0.1.0a0/src/outline/types/comment_list_response.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/document.py` & `outline_python_api-0.1.0a0/src/outline/types/document.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/document_archive_response.py` & `outline_python_api-0.1.0a0/src/outline/types/document_archive_response.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/document_create_params.py` & `outline_python_api-0.1.0a0/src/outline/types/document_create_params.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/document_create_response.py` & `outline_python_api-0.1.0a0/src/outline/types/document_create_response.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/document_delete_params.py` & `outline_python_api-0.1.0a0/src/outline/types/document_delete_params.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/document_drafts_params.py` & `outline_python_api-0.1.0a0/src/outline/types/document_drafts_params.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/document_drafts_response.py` & `outline_python_api-0.1.0a0/src/outline/types/document_drafts_response.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/document_import_params.py` & `outline_python_api-0.1.0a0/src/outline/types/document_import_params.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/document_info_params.py` & `outline_python_api-0.1.0a0/src/outline/types/document_info_params.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/document_list_params.py` & `outline_python_api-0.1.0a0/src/outline/types/document_list_params.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/document_list_response.py` & `outline_python_api-0.1.0a0/src/outline/types/document_list_response.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/document_move_params.py` & `outline_python_api-0.1.0a0/src/outline/types/document_move_params.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/document_move_response.py` & `outline_python_api-0.1.0a0/src/outline/types/document_move_response.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/document_restore_params.py` & `outline_python_api-0.1.0a0/src/outline/types/document_restore_params.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/document_restore_response.py` & `outline_python_api-0.1.0a0/src/outline/types/document_restore_response.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/document_search_params.py` & `outline_python_api-0.1.0a0/src/outline/types/document_search_params.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/document_search_response.py` & `outline_python_api-0.1.0a0/src/outline/types/document_search_response.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/document_templatize_response.py` & `outline_python_api-0.1.0a0/src/outline/types/document_templatize_response.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/document_unpublish_response.py` & `outline_python_api-0.1.0a0/src/outline/types/document_unpublish_response.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/document_update_params.py` & `outline_python_api-0.1.0a0/src/outline/types/document_update_params.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/document_update_response.py` & `outline_python_api-0.1.0a0/src/outline/types/document_update_response.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/document_viewed_response.py` & `outline_python_api-0.1.0a0/src/outline/types/document_viewed_response.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/event_create_params.py` & `outline_python_api-0.1.0a0/src/outline/types/event_create_params.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/event_create_response.py` & `outline_python_api-0.1.0a0/src/outline/types/event_create_response.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/file_operation.py` & `outline_python_api-0.1.0a0/src/outline/types/file_operation.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/group.py` & `outline_python_api-0.1.0a0/src/outline/types/group.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/group_create_response.py` & `outline_python_api-0.1.0a0/src/outline/types/group_create_response.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/group_update_response.py` & `outline_python_api-0.1.0a0/src/outline/types/group_update_response.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/collections/group_membership_list_response.py` & `outline_python_api-0.1.0a0/src/outline/types/collections/group_membership_list_response.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/src/outline/types/collections/membership_list_response.py` & `outline_python_api-0.1.0a0/src/outline/types/collections/membership_list_response.py`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/LICENSE` & `outline_python_api-0.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `outline_python_api-0.0.1a0/pyproject.toml` & `outline_python_api-0.1.0a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "outline-python-api"
-version = "0.0.1-alpha"
+version = "0.1.0-alpha"
 description = "The official Python library for the outline API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Outline", email = "hello@getoutline.com" },
 ]
 dependencies = [
```

### Comparing `outline_python_api-0.0.1a0/PKG-INFO` & `outline_python_api-0.1.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: outline-python-api
-Version: 0.0.1a0
+Version: 0.1.0a0
 Summary: The official Python library for the outline API
 Project-URL: Homepage, https://github.com/Yoshino-s/outline-python-api
 Project-URL: Repository, https://github.com/Yoshino-s/outline-python-api
 Author-email: Outline <hello@getoutline.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
```


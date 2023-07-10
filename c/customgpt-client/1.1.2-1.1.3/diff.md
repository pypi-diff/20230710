# Comparing `tmp/customgpt_client-1.1.2-py3-none-any.whl.zip` & `tmp/customgpt_client-1.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,378 +1,507 @@
-Zip file size: 304733 bytes, number of entries: 376
+Zip file size: 404484 bytes, number of entries: 505
 -rw-r--r--  2.0 unx      105 b- defN 80-Jan-01 00:00 customgpt_client/__init__.py
 -rw-r--r--  2.0 unx       47 b- defN 80-Jan-01 00:00 customgpt_client/api/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 customgpt_client/api/citations/__init__.py
--rw-r--r--  2.0 unx     6513 b- defN 80-Jan-01 00:00 customgpt_client/api/citations/get_open_graph_data_for_citation.py
+-rw-r--r--  2.0 unx     5868 b- defN 80-Jan-01 00:00 customgpt_client/api/citations/get_open_graph_data_for_citation.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 customgpt_client/api/conversations/__init__.py
--rw-r--r--  2.0 unx     7370 b- defN 80-Jan-01 00:00 customgpt_client/api/conversations/create_project_conversation.py
--rw-r--r--  2.0 unx     6970 b- defN 80-Jan-01 00:00 customgpt_client/api/conversations/delete_project_conversation.py
--rw-r--r--  2.0 unx     8648 b- defN 80-Jan-01 00:00 customgpt_client/api/conversations/get_project_conversations.py
--rw-r--r--  2.0 unx     8015 b- defN 80-Jan-01 00:00 customgpt_client/api/conversations/messages.py
--rw-r--r--  2.0 unx    12846 b- defN 80-Jan-01 00:00 customgpt_client/api/conversations/send_message_to_conversation.py
--rw-r--r--  2.0 unx     7725 b- defN 80-Jan-01 00:00 customgpt_client/api/conversations/update_project_conversation.py
+-rw-r--r--  2.0 unx     6697 b- defN 80-Jan-01 00:00 customgpt_client/api/conversations/create_project_conversation.py
+-rw-r--r--  2.0 unx     6332 b- defN 80-Jan-01 00:00 customgpt_client/api/conversations/delete_project_conversation.py
+-rw-r--r--  2.0 unx     7825 b- defN 80-Jan-01 00:00 customgpt_client/api/conversations/get_project_conversations.py
+-rw-r--r--  2.0 unx     7199 b- defN 80-Jan-01 00:00 customgpt_client/api/conversations/messages.py
+-rw-r--r--  2.0 unx     8580 b- defN 80-Jan-01 00:00 customgpt_client/api/conversations/send_message_to_conversation.py
+-rw-r--r--  2.0 unx     7032 b- defN 80-Jan-01 00:00 customgpt_client/api/conversations/update_project_conversation.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 customgpt_client/api/pages/__init__.py
--rw-r--r--  2.0 unx     6716 b- defN 80-Jan-01 00:00 customgpt_client/api/pages/delete_project_page.py
--rw-r--r--  2.0 unx     8458 b- defN 80-Jan-01 00:00 customgpt_client/api/pages/get_project_pages.py
--rw-r--r--  2.0 unx     4706 b- defN 80-Jan-01 00:00 customgpt_client/api/pages/preview.py
+-rw-r--r--  2.0 unx     6060 b- defN 80-Jan-01 00:00 customgpt_client/api/pages/delete_project_page.py
+-rw-r--r--  2.0 unx     7653 b- defN 80-Jan-01 00:00 customgpt_client/api/pages/get_project_pages.py
+-rw-r--r--  2.0 unx     4239 b- defN 80-Jan-01 00:00 customgpt_client/api/pages/preview.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 customgpt_client/api/project_plugins/__init__.py
+-rw-r--r--  2.0 unx     6346 b- defN 80-Jan-01 00:00 customgpt_client/api/project_plugins/create_project_plugin.py
+-rw-r--r--  2.0 unx     5618 b- defN 80-Jan-01 00:00 customgpt_client/api/project_plugins/get_project_plugins.py
+-rw-r--r--  2.0 unx     6319 b- defN 80-Jan-01 00:00 customgpt_client/api/project_plugins/update_project_plugin.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 customgpt_client/api/project_settings/__init__.py
--rw-r--r--  2.0 unx     6233 b- defN 80-Jan-01 00:00 customgpt_client/api/project_settings/get_project_settings.py
--rw-r--r--  2.0 unx     7313 b- defN 80-Jan-01 00:00 customgpt_client/api/project_settings/update_project_settings.py
+-rw-r--r--  2.0 unx     5651 b- defN 80-Jan-01 00:00 customgpt_client/api/project_settings/get_project_settings.py
+-rw-r--r--  2.0 unx     6646 b- defN 80-Jan-01 00:00 customgpt_client/api/project_settings/update_project_settings.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 customgpt_client/api/projects/__init__.py
--rw-r--r--  2.0 unx     6242 b- defN 80-Jan-01 00:00 customgpt_client/api/projects/create_project.py
--rw-r--r--  2.0 unx     5760 b- defN 80-Jan-01 00:00 customgpt_client/api/projects/delete_project.py
--rw-r--r--  2.0 unx     7074 b- defN 80-Jan-01 00:00 customgpt_client/api/projects/get_project.py
--rw-r--r--  2.0 unx     8489 b- defN 80-Jan-01 00:00 customgpt_client/api/projects/list_projects.py
--rw-r--r--  2.0 unx     5767 b- defN 80-Jan-01 00:00 customgpt_client/api/projects/stats_project.py
--rw-r--r--  2.0 unx     6358 b- defN 80-Jan-01 00:00 customgpt_client/api/projects/update_project.py
+-rw-r--r--  2.0 unx     5647 b- defN 80-Jan-01 00:00 customgpt_client/api/projects/create_project.py
+-rw-r--r--  2.0 unx     5205 b- defN 80-Jan-01 00:00 customgpt_client/api/projects/delete_project.py
+-rw-r--r--  2.0 unx     6372 b- defN 80-Jan-01 00:00 customgpt_client/api/projects/get_project.py
+-rw-r--r--  2.0 unx     7625 b- defN 80-Jan-01 00:00 customgpt_client/api/projects/list_projects.py
+-rw-r--r--  2.0 unx     5203 b- defN 80-Jan-01 00:00 customgpt_client/api/projects/stats_project.py
+-rw-r--r--  2.0 unx     5799 b- defN 80-Jan-01 00:00 customgpt_client/api/projects/update_project.py
+-rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 customgpt_client/api/sources/__init__.py
+-rw-r--r--  2.0 unx     7048 b- defN 80-Jan-01 00:00 customgpt_client/api/sources/create_project_source.py
+-rw-r--r--  2.0 unx     5998 b- defN 80-Jan-01 00:00 customgpt_client/api/sources/delete_project_source.py
+-rw-r--r--  2.0 unx     5641 b- defN 80-Jan-01 00:00 customgpt_client/api/sources/list_project_sources.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 customgpt_client/api/users/__init__.py
--rw-r--r--  2.0 unx     4857 b- defN 80-Jan-01 00:00 customgpt_client/api/users/get_user_profile.py
--rw-r--r--  2.0 unx     5851 b- defN 80-Jan-01 00:00 customgpt_client/api/users/update_user_profile.py
--rw-r--r--  2.0 unx    28543 b- defN 80-Jan-01 00:00 customgpt_client/client.py
+-rw-r--r--  2.0 unx     4358 b- defN 80-Jan-01 00:00 customgpt_client/api/users/get_user_profile.py
+-rw-r--r--  2.0 unx     5275 b- defN 80-Jan-01 00:00 customgpt_client/api/users/update_user_profile.py
+-rw-r--r--  2.0 unx    17457 b- defN 80-Jan-01 00:00 customgpt_client/client.py
 -rw-r--r--  2.0 unx      470 b- defN 80-Jan-01 00:00 customgpt_client/errors.py
--rw-r--r--  2.0 unx    42317 b- defN 80-Jan-01 00:00 customgpt_client/models/__init__.py
--rw-r--r--  2.0 unx     4878 b- defN 80-Jan-01 00:00 customgpt_client/models/conversation.py
--rw-r--r--  2.0 unx     1604 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_conversation_json_body.py
--rw-r--r--  2.0 unx     3055 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_conversation_response_201.py
--rw-r--r--  2.0 unx     5033 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_conversation_response_201_data.py
+-rw-r--r--  2.0 unx    58865 b- defN 80-Jan-01 00:00 customgpt_client/models/__init__.py
+-rw-r--r--  2.0 unx     4857 b- defN 80-Jan-01 00:00 customgpt_client/models/conversation.py
+-rw-r--r--  2.0 unx     1583 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_conversation_json_body.py
+-rw-r--r--  2.0 unx     3034 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_conversation_response_201.py
+-rw-r--r--  2.0 unx     5141 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_conversation_response_201_data.py
 -rw-r--r--  2.0 unx      191 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_conversation_response_201_status.py
--rw-r--r--  2.0 unx     3341 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_conversation_response_401.py
--rw-r--r--  2.0 unx     2456 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_conversation_response_401_data.py
+-rw-r--r--  2.0 unx     3320 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_conversation_response_401.py
+-rw-r--r--  2.0 unx     2435 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_conversation_response_401_data.py
 -rw-r--r--  2.0 unx      270 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_conversation_response_401_data_code.py
 -rw-r--r--  2.0 unx      191 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_conversation_response_401_status.py
--rw-r--r--  2.0 unx     3341 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_conversation_response_404.py
--rw-r--r--  2.0 unx     3034 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_conversation_response_404_data.py
+-rw-r--r--  2.0 unx     3320 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_conversation_response_404.py
+-rw-r--r--  2.0 unx     3013 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_conversation_response_404_data.py
 -rw-r--r--  2.0 unx      270 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_conversation_response_404_data_code.py
 -rw-r--r--  2.0 unx      270 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_conversation_response_404_data_message.py
 -rw-r--r--  2.0 unx      191 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_conversation_response_404_status.py
--rw-r--r--  2.0 unx     3341 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_conversation_response_500.py
--rw-r--r--  2.0 unx     2439 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_conversation_response_500_data.py
+-rw-r--r--  2.0 unx     3320 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_conversation_response_500.py
+-rw-r--r--  2.0 unx     2418 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_conversation_response_500_data.py
 -rw-r--r--  2.0 unx      270 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_conversation_response_500_data_code.py
 -rw-r--r--  2.0 unx      191 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_conversation_response_500_status.py
--rw-r--r--  2.0 unx     4400 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_multipart_data.py
--rw-r--r--  2.0 unx     2821 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_response_201.py
--rw-r--r--  2.0 unx     8090 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_response_201_data.py
+-rw-r--r--  2.0 unx     4379 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_multipart_data.py
+-rw-r--r--  2.0 unx     3030 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_plugin_json_body.py
+-rw-r--r--  2.0 unx     2920 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_plugin_response_201.py
+-rw-r--r--  2.0 unx     3355 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_plugin_response_201_data.py
+-rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_plugin_response_201_status.py
+-rw-r--r--  2.0 unx     3206 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_plugin_response_401.py
+-rw-r--r--  2.0 unx     2369 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_plugin_response_401_data.py
+-rw-r--r--  2.0 unx      264 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_plugin_response_401_data_code.py
+-rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_plugin_response_401_status.py
+-rw-r--r--  2.0 unx     3206 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_plugin_response_404.py
+-rw-r--r--  2.0 unx     2902 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_plugin_response_404_data.py
+-rw-r--r--  2.0 unx      264 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_plugin_response_404_data_code.py
+-rw-r--r--  2.0 unx      264 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_plugin_response_404_data_message.py
+-rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_plugin_response_404_status.py
+-rw-r--r--  2.0 unx     3206 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_plugin_response_500.py
+-rw-r--r--  2.0 unx     2352 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_plugin_response_500_data.py
+-rw-r--r--  2.0 unx      264 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_plugin_response_500_data_code.py
+-rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_plugin_response_500_status.py
+-rw-r--r--  2.0 unx     2800 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_response_201.py
+-rw-r--r--  2.0 unx     8069 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_response_201_data.py
 -rw-r--r--  2.0 unx      177 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_response_201_data_type.py
 -rw-r--r--  2.0 unx      179 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_response_201_status.py
--rw-r--r--  2.0 unx     3107 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_response_400.py
--rw-r--r--  2.0 unx     2819 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_response_400_data.py
+-rw-r--r--  2.0 unx     3086 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_response_400.py
+-rw-r--r--  2.0 unx     2798 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_response_400_data.py
 -rw-r--r--  2.0 unx      258 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_response_400_data_code.py
 -rw-r--r--  2.0 unx      362 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_response_400_data_message.py
 -rw-r--r--  2.0 unx      179 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_response_400_status.py
--rw-r--r--  2.0 unx     3107 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_response_401.py
--rw-r--r--  2.0 unx     2320 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_response_401_data.py
+-rw-r--r--  2.0 unx     3086 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_response_401.py
+-rw-r--r--  2.0 unx     2299 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_response_401_data.py
 -rw-r--r--  2.0 unx      258 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_response_401_data_code.py
 -rw-r--r--  2.0 unx      179 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_response_401_status.py
--rw-r--r--  2.0 unx     3107 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_response_500.py
--rw-r--r--  2.0 unx     2303 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_response_500_data.py
+-rw-r--r--  2.0 unx     3086 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_response_500.py
+-rw-r--r--  2.0 unx     2282 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_response_500_data.py
 -rw-r--r--  2.0 unx      258 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_response_500_data_code.py
 -rw-r--r--  2.0 unx      179 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_response_500_status.py
--rw-r--r--  2.0 unx     3055 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_conversation_response_200.py
--rw-r--r--  2.0 unx     1700 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_conversation_response_200_data.py
+-rw-r--r--  2.0 unx     3787 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_multipart_data.py
+-rw-r--r--  2.0 unx     2920 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_response_201.py
+-rw-r--r--  2.0 unx     5993 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_response_201_data.py
+-rw-r--r--  2.0 unx     9212 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_response_201_data_pages_item.py
+-rw-r--r--  2.0 unx      256 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_response_201_data_pages_item_crawl_status.py
+-rw-r--r--  2.0 unx      256 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_response_201_data_pages_item_index_status.py
+-rw-r--r--  2.0 unx     3078 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_response_201_data_settings.py
+-rw-r--r--  2.0 unx      249 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_response_201_data_type.py
+-rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_response_201_status.py
+-rw-r--r--  2.0 unx     3206 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_response_400.py
+-rw-r--r--  2.0 unx     2898 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_response_400_data.py
+-rw-r--r--  2.0 unx      264 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_response_400_data_code.py
+-rw-r--r--  2.0 unx      406 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_response_400_data_message.py
+-rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_response_400_status.py
+-rw-r--r--  2.0 unx     3206 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_response_401.py
+-rw-r--r--  2.0 unx     2369 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_response_401_data.py
+-rw-r--r--  2.0 unx      264 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_response_401_data_code.py
+-rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_response_401_status.py
+-rw-r--r--  2.0 unx     3206 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_response_404.py
+-rw-r--r--  2.0 unx     2902 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_response_404_data.py
+-rw-r--r--  2.0 unx      264 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_response_404_data_code.py
+-rw-r--r--  2.0 unx      264 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_response_404_data_message.py
+-rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_response_404_status.py
+-rw-r--r--  2.0 unx     3206 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_response_500.py
+-rw-r--r--  2.0 unx     2352 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_response_500_data.py
+-rw-r--r--  2.0 unx      264 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_response_500_data_code.py
+-rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 customgpt_client/models/create_project_source_response_500_status.py
+-rw-r--r--  2.0 unx     3034 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_conversation_response_200.py
+-rw-r--r--  2.0 unx     1679 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_conversation_response_200_data.py
 -rw-r--r--  2.0 unx      191 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_conversation_response_200_status.py
--rw-r--r--  2.0 unx     3341 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_conversation_response_401.py
--rw-r--r--  2.0 unx     2456 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_conversation_response_401_data.py
+-rw-r--r--  2.0 unx     3320 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_conversation_response_401.py
+-rw-r--r--  2.0 unx     2435 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_conversation_response_401_data.py
 -rw-r--r--  2.0 unx      270 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_conversation_response_401_data_code.py
 -rw-r--r--  2.0 unx      191 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_conversation_response_401_status.py
--rw-r--r--  2.0 unx     3341 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_conversation_response_404.py
--rw-r--r--  2.0 unx     3034 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_conversation_response_404_data.py
+-rw-r--r--  2.0 unx     3320 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_conversation_response_404.py
+-rw-r--r--  2.0 unx     3013 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_conversation_response_404_data.py
 -rw-r--r--  2.0 unx      270 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_conversation_response_404_data_code.py
 -rw-r--r--  2.0 unx      270 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_conversation_response_404_data_message.py
 -rw-r--r--  2.0 unx      191 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_conversation_response_404_status.py
--rw-r--r--  2.0 unx     3341 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_conversation_response_500.py
--rw-r--r--  2.0 unx     2439 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_conversation_response_500_data.py
+-rw-r--r--  2.0 unx     3320 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_conversation_response_500.py
+-rw-r--r--  2.0 unx     2418 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_conversation_response_500_data.py
 -rw-r--r--  2.0 unx      270 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_conversation_response_500_data_code.py
 -rw-r--r--  2.0 unx      191 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_conversation_response_500_status.py
--rw-r--r--  2.0 unx     2903 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_page_response_200.py
--rw-r--r--  2.0 unx     1660 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_page_response_200_data.py
+-rw-r--r--  2.0 unx     2882 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_page_response_200.py
+-rw-r--r--  2.0 unx     1639 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_page_response_200_data.py
 -rw-r--r--  2.0 unx      183 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_page_response_200_status.py
--rw-r--r--  2.0 unx     3189 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_page_response_401.py
--rw-r--r--  2.0 unx     2368 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_page_response_401_data.py
+-rw-r--r--  2.0 unx     3168 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_page_response_401.py
+-rw-r--r--  2.0 unx     2347 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_page_response_401_data.py
 -rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_page_response_401_data_code.py
 -rw-r--r--  2.0 unx      183 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_page_response_401_status.py
--rw-r--r--  2.0 unx     3189 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_page_response_404.py
--rw-r--r--  2.0 unx     2889 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_page_response_404_data.py
+-rw-r--r--  2.0 unx     3168 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_page_response_404.py
+-rw-r--r--  2.0 unx     2868 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_page_response_404_data.py
 -rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_page_response_404_data_code.py
 -rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_page_response_404_data_message.py
 -rw-r--r--  2.0 unx      183 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_page_response_404_status.py
--rw-r--r--  2.0 unx     3189 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_page_response_500.py
--rw-r--r--  2.0 unx     2351 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_page_response_500_data.py
+-rw-r--r--  2.0 unx     3168 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_page_response_500.py
+-rw-r--r--  2.0 unx     2330 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_page_response_500_data.py
 -rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_page_response_500_data_code.py
 -rw-r--r--  2.0 unx      183 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_page_response_500_status.py
--rw-r--r--  2.0 unx     2821 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_response_200.py
--rw-r--r--  2.0 unx     1637 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_response_200_data.py
+-rw-r--r--  2.0 unx     2800 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_response_200.py
+-rw-r--r--  2.0 unx     1616 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_response_200_data.py
 -rw-r--r--  2.0 unx      179 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_response_200_status.py
--rw-r--r--  2.0 unx     3107 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_response_401.py
--rw-r--r--  2.0 unx     2320 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_response_401_data.py
+-rw-r--r--  2.0 unx     3086 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_response_401.py
+-rw-r--r--  2.0 unx     2299 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_response_401_data.py
 -rw-r--r--  2.0 unx      258 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_response_401_data_code.py
 -rw-r--r--  2.0 unx      179 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_response_401_status.py
--rw-r--r--  2.0 unx     3107 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_response_404.py
--rw-r--r--  2.0 unx     2816 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_response_404_data.py
+-rw-r--r--  2.0 unx     3086 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_response_404.py
+-rw-r--r--  2.0 unx     2795 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_response_404_data.py
 -rw-r--r--  2.0 unx      258 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_response_404_data_code.py
 -rw-r--r--  2.0 unx      258 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_response_404_data_message.py
 -rw-r--r--  2.0 unx      179 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_response_404_status.py
--rw-r--r--  2.0 unx     3107 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_response_500.py
--rw-r--r--  2.0 unx     2303 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_response_500_data.py
+-rw-r--r--  2.0 unx     3086 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_response_500.py
+-rw-r--r--  2.0 unx     2282 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_response_500_data.py
 -rw-r--r--  2.0 unx      258 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_response_500_data_code.py
 -rw-r--r--  2.0 unx      179 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_response_500_status.py
--rw-r--r--  2.0 unx     3148 b- defN 80-Jan-01 00:00 customgpt_client/models/get_open_graph_data_for_citation_response_200.py
--rw-r--r--  2.0 unx     4443 b- defN 80-Jan-01 00:00 customgpt_client/models/get_open_graph_data_for_citation_response_200_data.py
+-rw-r--r--  2.0 unx     2920 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_source_response_200.py
+-rw-r--r--  2.0 unx     1656 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_source_response_200_data.py
+-rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_source_response_200_status.py
+-rw-r--r--  2.0 unx     3206 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_source_response_401.py
+-rw-r--r--  2.0 unx     2369 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_source_response_401_data.py
+-rw-r--r--  2.0 unx      264 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_source_response_401_data_code.py
+-rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_source_response_401_status.py
+-rw-r--r--  2.0 unx     3206 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_source_response_404.py
+-rw-r--r--  2.0 unx     2902 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_source_response_404_data.py
+-rw-r--r--  2.0 unx      264 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_source_response_404_data_code.py
+-rw-r--r--  2.0 unx      264 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_source_response_404_data_message.py
+-rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_source_response_404_status.py
+-rw-r--r--  2.0 unx     3206 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_source_response_500.py
+-rw-r--r--  2.0 unx     2352 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_source_response_500_data.py
+-rw-r--r--  2.0 unx      264 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_source_response_500_data_code.py
+-rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 customgpt_client/models/delete_project_source_response_500_status.py
+-rw-r--r--  2.0 unx     3127 b- defN 80-Jan-01 00:00 customgpt_client/models/get_open_graph_data_for_citation_response_200.py
+-rw-r--r--  2.0 unx     4422 b- defN 80-Jan-01 00:00 customgpt_client/models/get_open_graph_data_for_citation_response_200_data.py
 -rw-r--r--  2.0 unx      193 b- defN 80-Jan-01 00:00 customgpt_client/models/get_open_graph_data_for_citation_response_200_status.py
--rw-r--r--  2.0 unx     3422 b- defN 80-Jan-01 00:00 customgpt_client/models/get_open_graph_data_for_citation_response_401.py
--rw-r--r--  2.0 unx     2499 b- defN 80-Jan-01 00:00 customgpt_client/models/get_open_graph_data_for_citation_response_401_data.py
+-rw-r--r--  2.0 unx     3401 b- defN 80-Jan-01 00:00 customgpt_client/models/get_open_graph_data_for_citation_response_401.py
+-rw-r--r--  2.0 unx     2478 b- defN 80-Jan-01 00:00 customgpt_client/models/get_open_graph_data_for_citation_response_401_data.py
 -rw-r--r--  2.0 unx      272 b- defN 80-Jan-01 00:00 customgpt_client/models/get_open_graph_data_for_citation_response_401_data_code.py
 -rw-r--r--  2.0 unx      193 b- defN 80-Jan-01 00:00 customgpt_client/models/get_open_graph_data_for_citation_response_401_status.py
--rw-r--r--  2.0 unx     3422 b- defN 80-Jan-01 00:00 customgpt_client/models/get_open_graph_data_for_citation_response_404.py
--rw-r--r--  2.0 unx     3092 b- defN 80-Jan-01 00:00 customgpt_client/models/get_open_graph_data_for_citation_response_404_data.py
+-rw-r--r--  2.0 unx     3401 b- defN 80-Jan-01 00:00 customgpt_client/models/get_open_graph_data_for_citation_response_404.py
+-rw-r--r--  2.0 unx     3071 b- defN 80-Jan-01 00:00 customgpt_client/models/get_open_graph_data_for_citation_response_404_data.py
 -rw-r--r--  2.0 unx      272 b- defN 80-Jan-01 00:00 customgpt_client/models/get_open_graph_data_for_citation_response_404_data_code.py
 -rw-r--r--  2.0 unx      272 b- defN 80-Jan-01 00:00 customgpt_client/models/get_open_graph_data_for_citation_response_404_data_message.py
 -rw-r--r--  2.0 unx      193 b- defN 80-Jan-01 00:00 customgpt_client/models/get_open_graph_data_for_citation_response_404_status.py
 -rw-r--r--  2.0 unx      167 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_order.py
--rw-r--r--  2.0 unx     3017 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_200.py
--rw-r--r--  2.0 unx     7137 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_200_data.py
--rw-r--r--  2.0 unx     5069 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_200_data_data_item.py
--rw-r--r--  2.0 unx     2602 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_200_data_links.py
+-rw-r--r--  2.0 unx     2996 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_200.py
+-rw-r--r--  2.0 unx     6186 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_200_data.py
+-rw-r--r--  2.0 unx     5177 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_200_data_data_item.py
 -rw-r--r--  2.0 unx      189 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_200_status.py
--rw-r--r--  2.0 unx     3303 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_401.py
--rw-r--r--  2.0 unx     2434 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_401_data.py
+-rw-r--r--  2.0 unx     3282 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_401.py
+-rw-r--r--  2.0 unx     2413 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_401_data.py
 -rw-r--r--  2.0 unx      268 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_401_data_code.py
 -rw-r--r--  2.0 unx      189 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_401_status.py
--rw-r--r--  2.0 unx     3303 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_404.py
--rw-r--r--  2.0 unx     2991 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_404_data.py
+-rw-r--r--  2.0 unx     3282 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_404.py
+-rw-r--r--  2.0 unx     2970 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_404_data.py
 -rw-r--r--  2.0 unx      268 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_404_data_code.py
 -rw-r--r--  2.0 unx      268 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_404_data_message.py
 -rw-r--r--  2.0 unx      189 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_404_status.py
--rw-r--r--  2.0 unx     3303 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_500.py
--rw-r--r--  2.0 unx     2417 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_500_data.py
+-rw-r--r--  2.0 unx     3282 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_500.py
+-rw-r--r--  2.0 unx     2396 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_500_data.py
 -rw-r--r--  2.0 unx      268 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_500_data_code.py
 -rw-r--r--  2.0 unx      189 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_conversations_response_500_status.py
 -rw-r--r--  2.0 unx      159 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_order.py
--rw-r--r--  2.0 unx     2865 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_200.py
--rw-r--r--  2.0 unx     3094 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_200_data.py
--rw-r--r--  2.0 unx     7042 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_200_data_pages.py
--rw-r--r--  2.0 unx     9561 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_200_data_pages_data_item.py
+-rw-r--r--  2.0 unx     2844 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_200.py
+-rw-r--r--  2.0 unx     3073 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_200_data.py
+-rw-r--r--  2.0 unx     6138 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_200_data_pages.py
+-rw-r--r--  2.0 unx     9217 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_200_data_pages_data_item.py
 -rw-r--r--  2.0 unx      256 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_200_data_pages_data_item_crawl_status.py
 -rw-r--r--  2.0 unx      256 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_200_data_pages_data_item_index_status.py
--rw-r--r--  2.0 unx     2590 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_200_data_pages_links.py
--rw-r--r--  2.0 unx     8215 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_200_data_project.py
+-rw-r--r--  2.0 unx     8194 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_200_data_project.py
 -rw-r--r--  2.0 unx      186 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_200_data_project_type.py
 -rw-r--r--  2.0 unx      181 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_200_status.py
--rw-r--r--  2.0 unx     3151 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_401.py
--rw-r--r--  2.0 unx     2346 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_401_data.py
+-rw-r--r--  2.0 unx     3130 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_401.py
+-rw-r--r--  2.0 unx     2325 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_401_data.py
 -rw-r--r--  2.0 unx      260 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_401_data_code.py
 -rw-r--r--  2.0 unx      181 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_401_status.py
--rw-r--r--  2.0 unx     3151 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_404.py
--rw-r--r--  2.0 unx     2855 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_404_data.py
+-rw-r--r--  2.0 unx     3130 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_404.py
+-rw-r--r--  2.0 unx     2834 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_404_data.py
 -rw-r--r--  2.0 unx      260 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_404_data_code.py
 -rw-r--r--  2.0 unx      260 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_404_data_message.py
 -rw-r--r--  2.0 unx      181 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_404_status.py
--rw-r--r--  2.0 unx     3151 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_500.py
--rw-r--r--  2.0 unx     2329 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_500_data.py
+-rw-r--r--  2.0 unx     3130 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_500.py
+-rw-r--r--  2.0 unx     2308 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_500_data.py
 -rw-r--r--  2.0 unx      260 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_500_data_code.py
 -rw-r--r--  2.0 unx      181 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_pages_response_500_status.py
--rw-r--r--  2.0 unx     2764 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_response_200.py
--rw-r--r--  2.0 unx     8051 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_response_200_data.py
+-rw-r--r--  2.0 unx     2882 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_plugins_response_200.py
+-rw-r--r--  2.0 unx     3568 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_plugins_response_200_data.py
+-rw-r--r--  2.0 unx      183 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_plugins_response_200_status.py
+-rw-r--r--  2.0 unx     3168 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_plugins_response_401.py
+-rw-r--r--  2.0 unx     2347 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_plugins_response_401_data.py
+-rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_plugins_response_401_data_code.py
+-rw-r--r--  2.0 unx      183 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_plugins_response_401_status.py
+-rw-r--r--  2.0 unx     3168 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_plugins_response_404.py
+-rw-r--r--  2.0 unx     2868 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_plugins_response_404_data.py
+-rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_plugins_response_404_data_code.py
+-rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_plugins_response_404_data_message.py
+-rw-r--r--  2.0 unx      183 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_plugins_response_404_status.py
+-rw-r--r--  2.0 unx     3168 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_plugins_response_500.py
+-rw-r--r--  2.0 unx     2330 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_plugins_response_500_data.py
+-rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_plugins_response_500_data_code.py
+-rw-r--r--  2.0 unx      183 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_plugins_response_500_status.py
+-rw-r--r--  2.0 unx     2743 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_response_200.py
+-rw-r--r--  2.0 unx     8030 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_response_200_data.py
 -rw-r--r--  2.0 unx      174 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_response_200_data_type.py
 -rw-r--r--  2.0 unx      176 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_response_200_status.py
--rw-r--r--  2.0 unx     3050 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_response_401.py
--rw-r--r--  2.0 unx     2287 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_response_401_data.py
+-rw-r--r--  2.0 unx     3029 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_response_401.py
+-rw-r--r--  2.0 unx     2266 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_response_401_data.py
 -rw-r--r--  2.0 unx      255 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_response_401_data_code.py
 -rw-r--r--  2.0 unx      176 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_response_401_status.py
--rw-r--r--  2.0 unx     3050 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_response_404.py
--rw-r--r--  2.0 unx     2753 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_response_404_data.py
+-rw-r--r--  2.0 unx     3029 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_response_404.py
+-rw-r--r--  2.0 unx     2732 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_response_404_data.py
 -rw-r--r--  2.0 unx      255 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_response_404_data_code.py
 -rw-r--r--  2.0 unx      255 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_response_404_data_message.py
 -rw-r--r--  2.0 unx      176 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_response_404_status.py
--rw-r--r--  2.0 unx     3050 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_response_500.py
--rw-r--r--  2.0 unx     2270 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_response_500_data.py
+-rw-r--r--  2.0 unx     3029 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_response_500.py
+-rw-r--r--  2.0 unx     2249 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_response_500_data.py
 -rw-r--r--  2.0 unx      255 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_response_500_data_code.py
 -rw-r--r--  2.0 unx      176 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_response_500_status.py
--rw-r--r--  2.0 unx     2922 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_settings_response_200.py
--rw-r--r--  2.0 unx     4690 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_settings_response_200_data.py
+-rw-r--r--  2.0 unx     2901 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_settings_response_200.py
+-rw-r--r--  2.0 unx     4669 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_settings_response_200_data.py
 -rw-r--r--  2.0 unx      254 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_settings_response_200_data_response_source.py
 -rw-r--r--  2.0 unx      184 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_settings_response_200_status.py
--rw-r--r--  2.0 unx     3208 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_settings_response_401.py
--rw-r--r--  2.0 unx     2379 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_settings_response_401_data.py
+-rw-r--r--  2.0 unx     3187 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_settings_response_401.py
+-rw-r--r--  2.0 unx     2358 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_settings_response_401_data.py
 -rw-r--r--  2.0 unx      263 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_settings_response_401_data_code.py
 -rw-r--r--  2.0 unx      184 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_settings_response_401_status.py
--rw-r--r--  2.0 unx     3208 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_settings_response_404.py
--rw-r--r--  2.0 unx     2906 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_settings_response_404_data.py
+-rw-r--r--  2.0 unx     3187 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_settings_response_404.py
+-rw-r--r--  2.0 unx     2885 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_settings_response_404_data.py
 -rw-r--r--  2.0 unx      263 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_settings_response_404_data_code.py
 -rw-r--r--  2.0 unx      263 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_settings_response_404_data_message.py
 -rw-r--r--  2.0 unx      184 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_settings_response_404_status.py
--rw-r--r--  2.0 unx     3208 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_settings_response_500.py
--rw-r--r--  2.0 unx     2362 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_settings_response_500_data.py
+-rw-r--r--  2.0 unx     3187 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_settings_response_500.py
+-rw-r--r--  2.0 unx     2341 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_settings_response_500_data.py
 -rw-r--r--  2.0 unx      263 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_settings_response_500_data_code.py
 -rw-r--r--  2.0 unx      184 b- defN 80-Jan-01 00:00 customgpt_client/models/get_project_settings_response_500_status.py
--rw-r--r--  2.0 unx     2846 b- defN 80-Jan-01 00:00 customgpt_client/models/get_user_profile_response_200.py
--rw-r--r--  2.0 unx     3931 b- defN 80-Jan-01 00:00 customgpt_client/models/get_user_profile_response_200_data.py
+-rw-r--r--  2.0 unx     2825 b- defN 80-Jan-01 00:00 customgpt_client/models/get_user_profile_response_200.py
+-rw-r--r--  2.0 unx     3910 b- defN 80-Jan-01 00:00 customgpt_client/models/get_user_profile_response_200_data.py
 -rw-r--r--  2.0 unx      180 b- defN 80-Jan-01 00:00 customgpt_client/models/get_user_profile_response_200_status.py
--rw-r--r--  2.0 unx     3132 b- defN 80-Jan-01 00:00 customgpt_client/models/get_user_profile_response_401.py
--rw-r--r--  2.0 unx     2335 b- defN 80-Jan-01 00:00 customgpt_client/models/get_user_profile_response_401_data.py
+-rw-r--r--  2.0 unx     3111 b- defN 80-Jan-01 00:00 customgpt_client/models/get_user_profile_response_401.py
+-rw-r--r--  2.0 unx     2314 b- defN 80-Jan-01 00:00 customgpt_client/models/get_user_profile_response_401_data.py
 -rw-r--r--  2.0 unx      259 b- defN 80-Jan-01 00:00 customgpt_client/models/get_user_profile_response_401_data_code.py
 -rw-r--r--  2.0 unx      180 b- defN 80-Jan-01 00:00 customgpt_client/models/get_user_profile_response_401_status.py
--rw-r--r--  2.0 unx     3132 b- defN 80-Jan-01 00:00 customgpt_client/models/get_user_profile_response_500.py
--rw-r--r--  2.0 unx     2318 b- defN 80-Jan-01 00:00 customgpt_client/models/get_user_profile_response_500_data.py
+-rw-r--r--  2.0 unx     3111 b- defN 80-Jan-01 00:00 customgpt_client/models/get_user_profile_response_500.py
+-rw-r--r--  2.0 unx     2297 b- defN 80-Jan-01 00:00 customgpt_client/models/get_user_profile_response_500_data.py
 -rw-r--r--  2.0 unx      259 b- defN 80-Jan-01 00:00 customgpt_client/models/get_user_profile_response_500_data_code.py
 -rw-r--r--  2.0 unx      180 b- defN 80-Jan-01 00:00 customgpt_client/models/get_user_profile_response_500_status.py
+-rw-r--r--  2.0 unx     2901 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_200.py
+-rw-r--r--  2.0 unx     2835 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_200_data.py
+-rw-r--r--  2.0 unx     6387 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_200_data_sitemaps_item.py
+-rw-r--r--  2.0 unx     9893 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_200_data_sitemaps_item_pages_item.py
+-rw-r--r--  2.0 unx      267 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_200_data_sitemaps_item_pages_item_crawl_status.py
+-rw-r--r--  2.0 unx      267 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_200_data_sitemaps_item_pages_item_index_status.py
+-rw-r--r--  2.0 unx     3139 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_200_data_sitemaps_item_settings.py
+-rw-r--r--  2.0 unx      260 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_200_data_sitemaps_item_type.py
+-rw-r--r--  2.0 unx     6216 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_200_data_uploads.py
+-rw-r--r--  2.0 unx     9343 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_200_data_uploads_pages_item.py
+-rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_200_data_uploads_pages_item_crawl_status.py
+-rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_200_data_uploads_pages_item_index_status.py
+-rw-r--r--  2.0 unx     3111 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_200_data_uploads_settings.py
+-rw-r--r--  2.0 unx      255 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_200_data_uploads_type.py
+-rw-r--r--  2.0 unx      184 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_200_status.py
+-rw-r--r--  2.0 unx     3187 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_401.py
+-rw-r--r--  2.0 unx     2358 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_401_data.py
+-rw-r--r--  2.0 unx      263 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_401_data_code.py
+-rw-r--r--  2.0 unx      184 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_401_status.py
+-rw-r--r--  2.0 unx     3187 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_404.py
+-rw-r--r--  2.0 unx     2885 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_404_data.py
+-rw-r--r--  2.0 unx      263 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_404_data_code.py
+-rw-r--r--  2.0 unx      263 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_404_data_message.py
+-rw-r--r--  2.0 unx      184 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_404_status.py
+-rw-r--r--  2.0 unx     3187 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_500.py
+-rw-r--r--  2.0 unx     2341 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_500_data.py
+-rw-r--r--  2.0 unx      263 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_500_data_code.py
+-rw-r--r--  2.0 unx      184 b- defN 80-Jan-01 00:00 customgpt_client/models/list_project_sources_response_500_status.py
 -rw-r--r--  2.0 unx      156 b- defN 80-Jan-01 00:00 customgpt_client/models/list_projects_order.py
--rw-r--r--  2.0 unx     2802 b- defN 80-Jan-01 00:00 customgpt_client/models/list_projects_response_200.py
--rw-r--r--  2.0 unx     6843 b- defN 80-Jan-01 00:00 customgpt_client/models/list_projects_response_200_data.py
--rw-r--r--  2.0 unx     8189 b- defN 80-Jan-01 00:00 customgpt_client/models/list_projects_response_200_data_data_item.py
+-rw-r--r--  2.0 unx     2781 b- defN 80-Jan-01 00:00 customgpt_client/models/list_projects_response_200.py
+-rw-r--r--  2.0 unx     6007 b- defN 80-Jan-01 00:00 customgpt_client/models/list_projects_response_200_data.py
+-rw-r--r--  2.0 unx     8168 b- defN 80-Jan-01 00:00 customgpt_client/models/list_projects_response_200_data_data_item.py
 -rw-r--r--  2.0 unx      184 b- defN 80-Jan-01 00:00 customgpt_client/models/list_projects_response_200_data_data_item_type.py
--rw-r--r--  2.0 unx     2544 b- defN 80-Jan-01 00:00 customgpt_client/models/list_projects_response_200_data_links.py
 -rw-r--r--  2.0 unx      178 b- defN 80-Jan-01 00:00 customgpt_client/models/list_projects_response_200_status.py
--rw-r--r--  2.0 unx     3088 b- defN 80-Jan-01 00:00 customgpt_client/models/list_projects_response_401.py
--rw-r--r--  2.0 unx     2309 b- defN 80-Jan-01 00:00 customgpt_client/models/list_projects_response_401_data.py
+-rw-r--r--  2.0 unx     3067 b- defN 80-Jan-01 00:00 customgpt_client/models/list_projects_response_401.py
+-rw-r--r--  2.0 unx     2288 b- defN 80-Jan-01 00:00 customgpt_client/models/list_projects_response_401_data.py
 -rw-r--r--  2.0 unx      257 b- defN 80-Jan-01 00:00 customgpt_client/models/list_projects_response_401_data_code.py
 -rw-r--r--  2.0 unx      178 b- defN 80-Jan-01 00:00 customgpt_client/models/list_projects_response_401_status.py
--rw-r--r--  2.0 unx     3088 b- defN 80-Jan-01 00:00 customgpt_client/models/list_projects_response_500.py
--rw-r--r--  2.0 unx     2292 b- defN 80-Jan-01 00:00 customgpt_client/models/list_projects_response_500_data.py
+-rw-r--r--  2.0 unx     3067 b- defN 80-Jan-01 00:00 customgpt_client/models/list_projects_response_500.py
+-rw-r--r--  2.0 unx     2271 b- defN 80-Jan-01 00:00 customgpt_client/models/list_projects_response_500_data.py
 -rw-r--r--  2.0 unx      257 b- defN 80-Jan-01 00:00 customgpt_client/models/list_projects_response_500_data_code.py
 -rw-r--r--  2.0 unx      178 b- defN 80-Jan-01 00:00 customgpt_client/models/list_projects_response_500_status.py
 -rw-r--r--  2.0 unx      152 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_order.py
--rw-r--r--  2.0 unx     3753 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_200.py
--rw-r--r--  2.0 unx     4982 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_200_conversation.py
--rw-r--r--  2.0 unx     6836 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_200_messages.py
--rw-r--r--  2.0 unx     5141 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_200_messages_data_item.py
--rw-r--r--  2.0 unx     2541 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_200_messages_links.py
+-rw-r--r--  2.0 unx     2699 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_200.py
+-rw-r--r--  2.0 unx     3120 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_200_data.py
+-rw-r--r--  2.0 unx     5113 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_200_data_conversation.py
+-rw-r--r--  2.0 unx     6055 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_200_data_messages.py
+-rw-r--r--  2.0 unx     5143 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_200_data_messages_data_item.py
 -rw-r--r--  2.0 unx      174 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_200_status.py
--rw-r--r--  2.0 unx     3006 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_401.py
--rw-r--r--  2.0 unx     2261 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_401_data.py
+-rw-r--r--  2.0 unx     2985 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_401.py
+-rw-r--r--  2.0 unx     2240 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_401_data.py
 -rw-r--r--  2.0 unx      253 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_401_data_code.py
 -rw-r--r--  2.0 unx      174 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_401_status.py
--rw-r--r--  2.0 unx     3006 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_404.py
--rw-r--r--  2.0 unx     2714 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_404_data.py
+-rw-r--r--  2.0 unx     2985 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_404.py
+-rw-r--r--  2.0 unx     2693 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_404_data.py
 -rw-r--r--  2.0 unx      253 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_404_data_code.py
 -rw-r--r--  2.0 unx      253 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_404_data_message.py
 -rw-r--r--  2.0 unx      174 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_404_status.py
--rw-r--r--  2.0 unx     3006 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_500.py
--rw-r--r--  2.0 unx     2244 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_500_data.py
+-rw-r--r--  2.0 unx     2985 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_500.py
+-rw-r--r--  2.0 unx     2223 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_500_data.py
 -rw-r--r--  2.0 unx      253 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_500_data_code.py
 -rw-r--r--  2.0 unx      174 b- defN 80-Jan-01 00:00 customgpt_client/models/messages_response_500_status.py
--rw-r--r--  2.0 unx     4285 b- defN 80-Jan-01 00:00 customgpt_client/models/open_graph_cache.py
--rw-r--r--  2.0 unx     8656 b- defN 80-Jan-01 00:00 customgpt_client/models/page.py
+-rw-r--r--  2.0 unx     4264 b- defN 80-Jan-01 00:00 customgpt_client/models/open_graph_cache.py
+-rw-r--r--  2.0 unx     8312 b- defN 80-Jan-01 00:00 customgpt_client/models/page.py
 -rw-r--r--  2.0 unx      217 b- defN 80-Jan-01 00:00 customgpt_client/models/page_crawl_status.py
 -rw-r--r--  2.0 unx      217 b- defN 80-Jan-01 00:00 customgpt_client/models/page_index_status.py
--rw-r--r--  2.0 unx     2987 b- defN 80-Jan-01 00:00 customgpt_client/models/preview_response_401.py
--rw-r--r--  2.0 unx     2250 b- defN 80-Jan-01 00:00 customgpt_client/models/preview_response_401_data.py
+-rw-r--r--  2.0 unx     2966 b- defN 80-Jan-01 00:00 customgpt_client/models/preview_response_401.py
+-rw-r--r--  2.0 unx     2229 b- defN 80-Jan-01 00:00 customgpt_client/models/preview_response_401_data.py
 -rw-r--r--  2.0 unx      252 b- defN 80-Jan-01 00:00 customgpt_client/models/preview_response_401_data_code.py
 -rw-r--r--  2.0 unx      173 b- defN 80-Jan-01 00:00 customgpt_client/models/preview_response_401_status.py
--rw-r--r--  2.0 unx     2987 b- defN 80-Jan-01 00:00 customgpt_client/models/preview_response_404.py
--rw-r--r--  2.0 unx     2697 b- defN 80-Jan-01 00:00 customgpt_client/models/preview_response_404_data.py
+-rw-r--r--  2.0 unx     2966 b- defN 80-Jan-01 00:00 customgpt_client/models/preview_response_404.py
+-rw-r--r--  2.0 unx     2676 b- defN 80-Jan-01 00:00 customgpt_client/models/preview_response_404_data.py
 -rw-r--r--  2.0 unx      252 b- defN 80-Jan-01 00:00 customgpt_client/models/preview_response_404_data_code.py
 -rw-r--r--  2.0 unx      252 b- defN 80-Jan-01 00:00 customgpt_client/models/preview_response_404_data_message.py
 -rw-r--r--  2.0 unx      173 b- defN 80-Jan-01 00:00 customgpt_client/models/preview_response_404_status.py
--rw-r--r--  2.0 unx     2987 b- defN 80-Jan-01 00:00 customgpt_client/models/preview_response_500.py
--rw-r--r--  2.0 unx     2233 b- defN 80-Jan-01 00:00 customgpt_client/models/preview_response_500_data.py
+-rw-r--r--  2.0 unx     2966 b- defN 80-Jan-01 00:00 customgpt_client/models/preview_response_500.py
+-rw-r--r--  2.0 unx     2212 b- defN 80-Jan-01 00:00 customgpt_client/models/preview_response_500_data.py
 -rw-r--r--  2.0 unx      252 b- defN 80-Jan-01 00:00 customgpt_client/models/preview_response_500_data_code.py
 -rw-r--r--  2.0 unx      173 b- defN 80-Jan-01 00:00 customgpt_client/models/preview_response_500_status.py
--rw-r--r--  2.0 unx     7789 b- defN 80-Jan-01 00:00 customgpt_client/models/project.py
--rw-r--r--  2.0 unx     3482 b- defN 80-Jan-01 00:00 customgpt_client/models/project_plugin.py
--rw-r--r--  2.0 unx     4467 b- defN 80-Jan-01 00:00 customgpt_client/models/project_settings.py
+-rw-r--r--  2.0 unx     7768 b- defN 80-Jan-01 00:00 customgpt_client/models/project.py
+-rw-r--r--  2.0 unx     3238 b- defN 80-Jan-01 00:00 customgpt_client/models/project_plugin.py
+-rw-r--r--  2.0 unx     4818 b- defN 80-Jan-01 00:00 customgpt_client/models/project_settings.py
 -rw-r--r--  2.0 unx      236 b- defN 80-Jan-01 00:00 customgpt_client/models/project_settings_response_source.py
+-rw-r--r--  2.0 unx     5258 b- defN 80-Jan-01 00:00 customgpt_client/models/project_source.py
+-rw-r--r--  2.0 unx     2961 b- defN 80-Jan-01 00:00 customgpt_client/models/project_source_settings.py
+-rw-r--r--  2.0 unx      228 b- defN 80-Jan-01 00:00 customgpt_client/models/project_source_type.py
 -rw-r--r--  2.0 unx      156 b- defN 80-Jan-01 00:00 customgpt_client/models/project_type.py
--rw-r--r--  2.0 unx     5019 b- defN 80-Jan-01 00:00 customgpt_client/models/prompt_history.py
--rw-r--r--  2.0 unx     1654 b- defN 80-Jan-01 00:00 customgpt_client/models/send_message_to_conversation_json_body.py
--rw-r--r--  2.0 unx     3061 b- defN 80-Jan-01 00:00 customgpt_client/models/send_message_to_conversation_response_200.py
--rw-r--r--  2.0 unx     5169 b- defN 80-Jan-01 00:00 customgpt_client/models/send_message_to_conversation_response_200_data.py
+-rw-r--r--  2.0 unx     4998 b- defN 80-Jan-01 00:00 customgpt_client/models/prompt_history.py
+-rw-r--r--  2.0 unx     1633 b- defN 80-Jan-01 00:00 customgpt_client/models/send_message_to_conversation_json_body.py
+-rw-r--r--  2.0 unx     3040 b- defN 80-Jan-01 00:00 customgpt_client/models/send_message_to_conversation_response_200.py
+-rw-r--r--  2.0 unx     5148 b- defN 80-Jan-01 00:00 customgpt_client/models/send_message_to_conversation_response_200_data.py
 -rw-r--r--  2.0 unx      191 b- defN 80-Jan-01 00:00 customgpt_client/models/send_message_to_conversation_response_200_status.py
--rw-r--r--  2.0 unx     3347 b- defN 80-Jan-01 00:00 customgpt_client/models/send_message_to_conversation_response_401.py
--rw-r--r--  2.0 unx     2460 b- defN 80-Jan-01 00:00 customgpt_client/models/send_message_to_conversation_response_401_data.py
+-rw-r--r--  2.0 unx     3326 b- defN 80-Jan-01 00:00 customgpt_client/models/send_message_to_conversation_response_401.py
+-rw-r--r--  2.0 unx     2439 b- defN 80-Jan-01 00:00 customgpt_client/models/send_message_to_conversation_response_401_data.py
 -rw-r--r--  2.0 unx      270 b- defN 80-Jan-01 00:00 customgpt_client/models/send_message_to_conversation_response_401_data_code.py
 -rw-r--r--  2.0 unx      191 b- defN 80-Jan-01 00:00 customgpt_client/models/send_message_to_conversation_response_401_status.py
--rw-r--r--  2.0 unx     3347 b- defN 80-Jan-01 00:00 customgpt_client/models/send_message_to_conversation_response_404.py
--rw-r--r--  2.0 unx     3039 b- defN 80-Jan-01 00:00 customgpt_client/models/send_message_to_conversation_response_404_data.py
+-rw-r--r--  2.0 unx     3326 b- defN 80-Jan-01 00:00 customgpt_client/models/send_message_to_conversation_response_404.py
+-rw-r--r--  2.0 unx     3018 b- defN 80-Jan-01 00:00 customgpt_client/models/send_message_to_conversation_response_404_data.py
 -rw-r--r--  2.0 unx      270 b- defN 80-Jan-01 00:00 customgpt_client/models/send_message_to_conversation_response_404_data_code.py
 -rw-r--r--  2.0 unx      270 b- defN 80-Jan-01 00:00 customgpt_client/models/send_message_to_conversation_response_404_data_message.py
 -rw-r--r--  2.0 unx      191 b- defN 80-Jan-01 00:00 customgpt_client/models/send_message_to_conversation_response_404_status.py
--rw-r--r--  2.0 unx     3347 b- defN 80-Jan-01 00:00 customgpt_client/models/send_message_to_conversation_response_500.py
--rw-r--r--  2.0 unx     2443 b- defN 80-Jan-01 00:00 customgpt_client/models/send_message_to_conversation_response_500_data.py
+-rw-r--r--  2.0 unx     3326 b- defN 80-Jan-01 00:00 customgpt_client/models/send_message_to_conversation_response_500.py
+-rw-r--r--  2.0 unx     2422 b- defN 80-Jan-01 00:00 customgpt_client/models/send_message_to_conversation_response_500_data.py
 -rw-r--r--  2.0 unx      270 b- defN 80-Jan-01 00:00 customgpt_client/models/send_message_to_conversation_response_500_data_code.py
 -rw-r--r--  2.0 unx      191 b- defN 80-Jan-01 00:00 customgpt_client/models/send_message_to_conversation_response_500_status.py
--rw-r--r--  2.0 unx     2802 b- defN 80-Jan-01 00:00 customgpt_client/models/stats_project_response_200.py
--rw-r--r--  2.0 unx     3719 b- defN 80-Jan-01 00:00 customgpt_client/models/stats_project_response_200_data.py
+-rw-r--r--  2.0 unx     2781 b- defN 80-Jan-01 00:00 customgpt_client/models/stats_project_response_200.py
+-rw-r--r--  2.0 unx     3698 b- defN 80-Jan-01 00:00 customgpt_client/models/stats_project_response_200_data.py
 -rw-r--r--  2.0 unx      178 b- defN 80-Jan-01 00:00 customgpt_client/models/stats_project_response_200_status.py
--rw-r--r--  2.0 unx     3088 b- defN 80-Jan-01 00:00 customgpt_client/models/stats_project_response_401.py
--rw-r--r--  2.0 unx     2309 b- defN 80-Jan-01 00:00 customgpt_client/models/stats_project_response_401_data.py
+-rw-r--r--  2.0 unx     3067 b- defN 80-Jan-01 00:00 customgpt_client/models/stats_project_response_401.py
+-rw-r--r--  2.0 unx     2288 b- defN 80-Jan-01 00:00 customgpt_client/models/stats_project_response_401_data.py
 -rw-r--r--  2.0 unx      257 b- defN 80-Jan-01 00:00 customgpt_client/models/stats_project_response_401_data_code.py
 -rw-r--r--  2.0 unx      178 b- defN 80-Jan-01 00:00 customgpt_client/models/stats_project_response_401_status.py
--rw-r--r--  2.0 unx     3088 b- defN 80-Jan-01 00:00 customgpt_client/models/stats_project_response_404.py
--rw-r--r--  2.0 unx     2787 b- defN 80-Jan-01 00:00 customgpt_client/models/stats_project_response_404_data.py
+-rw-r--r--  2.0 unx     3067 b- defN 80-Jan-01 00:00 customgpt_client/models/stats_project_response_404.py
+-rw-r--r--  2.0 unx     2766 b- defN 80-Jan-01 00:00 customgpt_client/models/stats_project_response_404_data.py
 -rw-r--r--  2.0 unx      257 b- defN 80-Jan-01 00:00 customgpt_client/models/stats_project_response_404_data_code.py
 -rw-r--r--  2.0 unx      257 b- defN 80-Jan-01 00:00 customgpt_client/models/stats_project_response_404_data_message.py
 -rw-r--r--  2.0 unx      178 b- defN 80-Jan-01 00:00 customgpt_client/models/stats_project_response_404_status.py
--rw-r--r--  2.0 unx     3088 b- defN 80-Jan-01 00:00 customgpt_client/models/stats_project_response_500.py
--rw-r--r--  2.0 unx     2292 b- defN 80-Jan-01 00:00 customgpt_client/models/stats_project_response_500_data.py
+-rw-r--r--  2.0 unx     3067 b- defN 80-Jan-01 00:00 customgpt_client/models/stats_project_response_500.py
+-rw-r--r--  2.0 unx     2271 b- defN 80-Jan-01 00:00 customgpt_client/models/stats_project_response_500_data.py
 -rw-r--r--  2.0 unx      257 b- defN 80-Jan-01 00:00 customgpt_client/models/stats_project_response_500_data_code.py
 -rw-r--r--  2.0 unx      178 b- defN 80-Jan-01 00:00 customgpt_client/models/stats_project_response_500_status.py
--rw-r--r--  2.0 unx     1628 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_conversation_json_body.py
--rw-r--r--  2.0 unx     3055 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_conversation_response_200.py
--rw-r--r--  2.0 unx     5033 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_conversation_response_200_data.py
+-rw-r--r--  2.0 unx     1607 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_conversation_json_body.py
+-rw-r--r--  2.0 unx     3034 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_conversation_response_200.py
+-rw-r--r--  2.0 unx     5141 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_conversation_response_200_data.py
 -rw-r--r--  2.0 unx      191 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_conversation_response_200_status.py
--rw-r--r--  2.0 unx     3341 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_conversation_response_401.py
--rw-r--r--  2.0 unx     2456 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_conversation_response_401_data.py
+-rw-r--r--  2.0 unx     3320 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_conversation_response_401.py
+-rw-r--r--  2.0 unx     2435 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_conversation_response_401_data.py
 -rw-r--r--  2.0 unx      270 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_conversation_response_401_data_code.py
 -rw-r--r--  2.0 unx      191 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_conversation_response_401_status.py
--rw-r--r--  2.0 unx     3341 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_conversation_response_404.py
--rw-r--r--  2.0 unx     3034 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_conversation_response_404_data.py
+-rw-r--r--  2.0 unx     3320 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_conversation_response_404.py
+-rw-r--r--  2.0 unx     3013 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_conversation_response_404_data.py
 -rw-r--r--  2.0 unx      270 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_conversation_response_404_data_code.py
 -rw-r--r--  2.0 unx      270 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_conversation_response_404_data_message.py
 -rw-r--r--  2.0 unx      191 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_conversation_response_404_status.py
--rw-r--r--  2.0 unx     3341 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_conversation_response_500.py
--rw-r--r--  2.0 unx     2439 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_conversation_response_500_data.py
+-rw-r--r--  2.0 unx     3320 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_conversation_response_500.py
+-rw-r--r--  2.0 unx     2418 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_conversation_response_500_data.py
 -rw-r--r--  2.0 unx      270 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_conversation_response_500_data_code.py
 -rw-r--r--  2.0 unx      191 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_conversation_response_500_status.py
--rw-r--r--  2.0 unx     4948 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_multipart_data.py
--rw-r--r--  2.0 unx     2821 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_response_200.py
--rw-r--r--  2.0 unx     8090 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_response_200_data.py
+-rw-r--r--  2.0 unx     4927 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_multipart_data.py
+-rw-r--r--  2.0 unx     3030 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_plugin_json_body.py
+-rw-r--r--  2.0 unx     2920 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_plugin_response_200.py
+-rw-r--r--  2.0 unx     3355 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_plugin_response_200_data.py
+-rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_plugin_response_200_status.py
+-rw-r--r--  2.0 unx     3206 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_plugin_response_401.py
+-rw-r--r--  2.0 unx     2369 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_plugin_response_401_data.py
+-rw-r--r--  2.0 unx      264 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_plugin_response_401_data_code.py
+-rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_plugin_response_401_status.py
+-rw-r--r--  2.0 unx     3206 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_plugin_response_404.py
+-rw-r--r--  2.0 unx     2902 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_plugin_response_404_data.py
+-rw-r--r--  2.0 unx      264 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_plugin_response_404_data_code.py
+-rw-r--r--  2.0 unx      264 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_plugin_response_404_data_message.py
+-rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_plugin_response_404_status.py
+-rw-r--r--  2.0 unx     3206 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_plugin_response_500.py
+-rw-r--r--  2.0 unx     2352 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_plugin_response_500_data.py
+-rw-r--r--  2.0 unx      264 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_plugin_response_500_data_code.py
+-rw-r--r--  2.0 unx      185 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_plugin_response_500_status.py
+-rw-r--r--  2.0 unx     2800 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_response_200.py
+-rw-r--r--  2.0 unx     8069 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_response_200_data.py
 -rw-r--r--  2.0 unx      177 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_response_200_data_type.py
 -rw-r--r--  2.0 unx      179 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_response_200_status.py
--rw-r--r--  2.0 unx     3107 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_response_401.py
--rw-r--r--  2.0 unx     2320 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_response_401_data.py
+-rw-r--r--  2.0 unx     3086 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_response_401.py
+-rw-r--r--  2.0 unx     2299 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_response_401_data.py
 -rw-r--r--  2.0 unx      258 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_response_401_data_code.py
 -rw-r--r--  2.0 unx      179 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_response_401_status.py
--rw-r--r--  2.0 unx     3107 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_response_404.py
--rw-r--r--  2.0 unx     2816 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_response_404_data.py
+-rw-r--r--  2.0 unx     3086 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_response_404.py
+-rw-r--r--  2.0 unx     2795 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_response_404_data.py
 -rw-r--r--  2.0 unx      258 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_response_404_data_code.py
 -rw-r--r--  2.0 unx      258 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_response_404_data_message.py
 -rw-r--r--  2.0 unx      179 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_response_404_status.py
--rw-r--r--  2.0 unx     3107 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_response_500.py
--rw-r--r--  2.0 unx     2303 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_response_500_data.py
+-rw-r--r--  2.0 unx     3086 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_response_500.py
+-rw-r--r--  2.0 unx     2282 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_response_500_data.py
 -rw-r--r--  2.0 unx      258 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_response_500_data_code.py
 -rw-r--r--  2.0 unx      179 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_response_500_status.py
--rw-r--r--  2.0 unx     6861 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_settings_multipart_data.py
--rw-r--r--  2.0 unx     2979 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_settings_response_200.py
--rw-r--r--  2.0 unx     1680 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_settings_response_200_data.py
+-rw-r--r--  2.0 unx     6840 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_settings_multipart_data.py
+-rw-r--r--  2.0 unx     2958 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_settings_response_200.py
+-rw-r--r--  2.0 unx     1659 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_settings_response_200_data.py
 -rw-r--r--  2.0 unx      187 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_settings_response_200_status.py
--rw-r--r--  2.0 unx     3265 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_settings_response_400.py
--rw-r--r--  2.0 unx     2976 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_settings_response_400_data.py
+-rw-r--r--  2.0 unx     3244 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_settings_response_400.py
+-rw-r--r--  2.0 unx     2955 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_settings_response_400_data.py
 -rw-r--r--  2.0 unx      266 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_settings_response_400_data_code.py
 -rw-r--r--  2.0 unx      423 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_settings_response_400_data_message.py
 -rw-r--r--  2.0 unx      187 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_settings_response_400_status.py
--rw-r--r--  2.0 unx     3265 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_settings_response_401.py
--rw-r--r--  2.0 unx     2412 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_settings_response_401_data.py
+-rw-r--r--  2.0 unx     3244 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_settings_response_401.py
+-rw-r--r--  2.0 unx     2391 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_settings_response_401_data.py
 -rw-r--r--  2.0 unx      266 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_settings_response_401_data_code.py
 -rw-r--r--  2.0 unx      187 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_settings_response_401_status.py
--rw-r--r--  2.0 unx     3265 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_settings_response_500.py
--rw-r--r--  2.0 unx     2395 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_settings_response_500_data.py
+-rw-r--r--  2.0 unx     3244 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_settings_response_500.py
+-rw-r--r--  2.0 unx     2374 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_settings_response_500_data.py
 -rw-r--r--  2.0 unx      266 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_settings_response_500_data_code.py
 -rw-r--r--  2.0 unx      187 b- defN 80-Jan-01 00:00 customgpt_client/models/update_project_settings_response_500_status.py
--rw-r--r--  2.0 unx     3050 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_multipart_data.py
--rw-r--r--  2.0 unx     2903 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_response_200.py
--rw-r--r--  2.0 unx     3946 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_response_200_data.py
+-rw-r--r--  2.0 unx     3029 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_multipart_data.py
+-rw-r--r--  2.0 unx     2882 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_response_200.py
+-rw-r--r--  2.0 unx     3925 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_response_200_data.py
 -rw-r--r--  2.0 unx      183 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_response_200_status.py
--rw-r--r--  2.0 unx     3189 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_response_401.py
--rw-r--r--  2.0 unx     2368 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_response_401_data.py
+-rw-r--r--  2.0 unx     3168 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_response_401.py
+-rw-r--r--  2.0 unx     2347 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_response_401_data.py
 -rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_response_401_data_code.py
 -rw-r--r--  2.0 unx      183 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_response_401_status.py
--rw-r--r--  2.0 unx     3189 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_response_500.py
--rw-r--r--  2.0 unx     2351 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_response_500_data.py
+-rw-r--r--  2.0 unx     3168 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_response_500.py
+-rw-r--r--  2.0 unx     2330 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_response_500_data.py
 -rw-r--r--  2.0 unx      262 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_response_500_data_code.py
 -rw-r--r--  2.0 unx      183 b- defN 80-Jan-01 00:00 customgpt_client/models/update_user_profile_response_500_status.py
--rw-r--r--  2.0 unx     3791 b- defN 80-Jan-01 00:00 customgpt_client/models/user.py
+-rw-r--r--  2.0 unx     3770 b- defN 80-Jan-01 00:00 customgpt_client/models/user.py
 -rw-r--r--  2.0 unx       25 b- defN 80-Jan-01 00:00 customgpt_client/py.typed
 -rw-r--r--  2.0 unx      993 b- defN 80-Jan-01 00:00 customgpt_client/types.py
--rw-r--r--  2.0 unx     1226 b- defN 80-Jan-01 00:00 customgpt_client-1.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 customgpt_client-1.1.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx    44509 b- defN 16-Jan-01 00:00 customgpt_client-1.1.2.dist-info/RECORD
-376 files, 888243 bytes uncompressed, 229497 bytes compressed:  74.2%
+-rw-r--r--  2.0 unx     1224 b- defN 80-Jan-01 00:00 customgpt_client-1.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 customgpt_client-1.1.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx    60483 b- defN 16-Jan-01 00:00 customgpt_client-1.1.3.dist-info/RECORD
+505 files, 1144978 bytes uncompressed, 302066 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -39,14 +39,26 @@
 
 Filename: customgpt_client/api/pages/get_project_pages.py
 Comment: 
 
 Filename: customgpt_client/api/pages/preview.py
 Comment: 
 
+Filename: customgpt_client/api/project_plugins/__init__.py
+Comment: 
+
+Filename: customgpt_client/api/project_plugins/create_project_plugin.py
+Comment: 
+
+Filename: customgpt_client/api/project_plugins/get_project_plugins.py
+Comment: 
+
+Filename: customgpt_client/api/project_plugins/update_project_plugin.py
+Comment: 
+
 Filename: customgpt_client/api/project_settings/__init__.py
 Comment: 
 
 Filename: customgpt_client/api/project_settings/get_project_settings.py
 Comment: 
 
 Filename: customgpt_client/api/project_settings/update_project_settings.py
@@ -69,14 +81,26 @@
 
 Filename: customgpt_client/api/projects/stats_project.py
 Comment: 
 
 Filename: customgpt_client/api/projects/update_project.py
 Comment: 
 
+Filename: customgpt_client/api/sources/__init__.py
+Comment: 
+
+Filename: customgpt_client/api/sources/create_project_source.py
+Comment: 
+
+Filename: customgpt_client/api/sources/delete_project_source.py
+Comment: 
+
+Filename: customgpt_client/api/sources/list_project_sources.py
+Comment: 
+
 Filename: customgpt_client/api/users/__init__.py
 Comment: 
 
 Filename: customgpt_client/api/users/get_user_profile.py
 Comment: 
 
 Filename: customgpt_client/api/users/update_user_profile.py
@@ -144,14 +168,65 @@
 
 Filename: customgpt_client/models/create_project_conversation_response_500_status.py
 Comment: 
 
 Filename: customgpt_client/models/create_project_multipart_data.py
 Comment: 
 
+Filename: customgpt_client/models/create_project_plugin_json_body.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_plugin_response_201.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_plugin_response_201_data.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_plugin_response_201_status.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_plugin_response_401.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_plugin_response_401_data.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_plugin_response_401_data_code.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_plugin_response_401_status.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_plugin_response_404.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_plugin_response_404_data.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_plugin_response_404_data_code.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_plugin_response_404_data_message.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_plugin_response_404_status.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_plugin_response_500.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_plugin_response_500_data.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_plugin_response_500_data_code.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_plugin_response_500_status.py
+Comment: 
+
 Filename: customgpt_client/models/create_project_response_201.py
 Comment: 
 
 Filename: customgpt_client/models/create_project_response_201_data.py
 Comment: 
 
 Filename: customgpt_client/models/create_project_response_201_data_type.py
@@ -195,14 +270,95 @@
 
 Filename: customgpt_client/models/create_project_response_500_data_code.py
 Comment: 
 
 Filename: customgpt_client/models/create_project_response_500_status.py
 Comment: 
 
+Filename: customgpt_client/models/create_project_source_multipart_data.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_source_response_201.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_source_response_201_data.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_source_response_201_data_pages_item.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_source_response_201_data_pages_item_crawl_status.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_source_response_201_data_pages_item_index_status.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_source_response_201_data_settings.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_source_response_201_data_type.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_source_response_201_status.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_source_response_400.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_source_response_400_data.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_source_response_400_data_code.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_source_response_400_data_message.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_source_response_400_status.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_source_response_401.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_source_response_401_data.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_source_response_401_data_code.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_source_response_401_status.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_source_response_404.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_source_response_404_data.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_source_response_404_data_code.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_source_response_404_data_message.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_source_response_404_status.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_source_response_500.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_source_response_500_data.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_source_response_500_data_code.py
+Comment: 
+
+Filename: customgpt_client/models/create_project_source_response_500_status.py
+Comment: 
+
 Filename: customgpt_client/models/delete_project_conversation_response_200.py
 Comment: 
 
 Filename: customgpt_client/models/delete_project_conversation_response_200_data.py
 Comment: 
 
 Filename: customgpt_client/models/delete_project_conversation_response_200_status.py
@@ -339,14 +495,62 @@
 
 Filename: customgpt_client/models/delete_project_response_500_data_code.py
 Comment: 
 
 Filename: customgpt_client/models/delete_project_response_500_status.py
 Comment: 
 
+Filename: customgpt_client/models/delete_project_source_response_200.py
+Comment: 
+
+Filename: customgpt_client/models/delete_project_source_response_200_data.py
+Comment: 
+
+Filename: customgpt_client/models/delete_project_source_response_200_status.py
+Comment: 
+
+Filename: customgpt_client/models/delete_project_source_response_401.py
+Comment: 
+
+Filename: customgpt_client/models/delete_project_source_response_401_data.py
+Comment: 
+
+Filename: customgpt_client/models/delete_project_source_response_401_data_code.py
+Comment: 
+
+Filename: customgpt_client/models/delete_project_source_response_401_status.py
+Comment: 
+
+Filename: customgpt_client/models/delete_project_source_response_404.py
+Comment: 
+
+Filename: customgpt_client/models/delete_project_source_response_404_data.py
+Comment: 
+
+Filename: customgpt_client/models/delete_project_source_response_404_data_code.py
+Comment: 
+
+Filename: customgpt_client/models/delete_project_source_response_404_data_message.py
+Comment: 
+
+Filename: customgpt_client/models/delete_project_source_response_404_status.py
+Comment: 
+
+Filename: customgpt_client/models/delete_project_source_response_500.py
+Comment: 
+
+Filename: customgpt_client/models/delete_project_source_response_500_data.py
+Comment: 
+
+Filename: customgpt_client/models/delete_project_source_response_500_data_code.py
+Comment: 
+
+Filename: customgpt_client/models/delete_project_source_response_500_status.py
+Comment: 
+
 Filename: customgpt_client/models/get_open_graph_data_for_citation_response_200.py
 Comment: 
 
 Filename: customgpt_client/models/get_open_graph_data_for_citation_response_200_data.py
 Comment: 
 
 Filename: customgpt_client/models/get_open_graph_data_for_citation_response_200_status.py
@@ -387,17 +591,14 @@
 
 Filename: customgpt_client/models/get_project_conversations_response_200_data.py
 Comment: 
 
 Filename: customgpt_client/models/get_project_conversations_response_200_data_data_item.py
 Comment: 
 
-Filename: customgpt_client/models/get_project_conversations_response_200_data_links.py
-Comment: 
-
 Filename: customgpt_client/models/get_project_conversations_response_200_status.py
 Comment: 
 
 Filename: customgpt_client/models/get_project_conversations_response_401.py
 Comment: 
 
 Filename: customgpt_client/models/get_project_conversations_response_401_data.py
@@ -453,17 +654,14 @@
 
 Filename: customgpt_client/models/get_project_pages_response_200_data_pages_data_item_crawl_status.py
 Comment: 
 
 Filename: customgpt_client/models/get_project_pages_response_200_data_pages_data_item_index_status.py
 Comment: 
 
-Filename: customgpt_client/models/get_project_pages_response_200_data_pages_links.py
-Comment: 
-
 Filename: customgpt_client/models/get_project_pages_response_200_data_project.py
 Comment: 
 
 Filename: customgpt_client/models/get_project_pages_response_200_data_project_type.py
 Comment: 
 
 Filename: customgpt_client/models/get_project_pages_response_200_status.py
@@ -504,14 +702,62 @@
 
 Filename: customgpt_client/models/get_project_pages_response_500_data_code.py
 Comment: 
 
 Filename: customgpt_client/models/get_project_pages_response_500_status.py
 Comment: 
 
+Filename: customgpt_client/models/get_project_plugins_response_200.py
+Comment: 
+
+Filename: customgpt_client/models/get_project_plugins_response_200_data.py
+Comment: 
+
+Filename: customgpt_client/models/get_project_plugins_response_200_status.py
+Comment: 
+
+Filename: customgpt_client/models/get_project_plugins_response_401.py
+Comment: 
+
+Filename: customgpt_client/models/get_project_plugins_response_401_data.py
+Comment: 
+
+Filename: customgpt_client/models/get_project_plugins_response_401_data_code.py
+Comment: 
+
+Filename: customgpt_client/models/get_project_plugins_response_401_status.py
+Comment: 
+
+Filename: customgpt_client/models/get_project_plugins_response_404.py
+Comment: 
+
+Filename: customgpt_client/models/get_project_plugins_response_404_data.py
+Comment: 
+
+Filename: customgpt_client/models/get_project_plugins_response_404_data_code.py
+Comment: 
+
+Filename: customgpt_client/models/get_project_plugins_response_404_data_message.py
+Comment: 
+
+Filename: customgpt_client/models/get_project_plugins_response_404_status.py
+Comment: 
+
+Filename: customgpt_client/models/get_project_plugins_response_500.py
+Comment: 
+
+Filename: customgpt_client/models/get_project_plugins_response_500_data.py
+Comment: 
+
+Filename: customgpt_client/models/get_project_plugins_response_500_data_code.py
+Comment: 
+
+Filename: customgpt_client/models/get_project_plugins_response_500_status.py
+Comment: 
+
 Filename: customgpt_client/models/get_project_response_200.py
 Comment: 
 
 Filename: customgpt_client/models/get_project_response_200_data.py
 Comment: 
 
 Filename: customgpt_client/models/get_project_response_200_data_type.py
@@ -639,14 +885,98 @@
 
 Filename: customgpt_client/models/get_user_profile_response_500_data_code.py
 Comment: 
 
 Filename: customgpt_client/models/get_user_profile_response_500_status.py
 Comment: 
 
+Filename: customgpt_client/models/list_project_sources_response_200.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_200_data.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_200_data_sitemaps_item.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_200_data_sitemaps_item_pages_item.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_200_data_sitemaps_item_pages_item_crawl_status.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_200_data_sitemaps_item_pages_item_index_status.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_200_data_sitemaps_item_settings.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_200_data_sitemaps_item_type.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_200_data_uploads.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_200_data_uploads_pages_item.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_200_data_uploads_pages_item_crawl_status.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_200_data_uploads_pages_item_index_status.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_200_data_uploads_settings.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_200_data_uploads_type.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_200_status.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_401.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_401_data.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_401_data_code.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_401_status.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_404.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_404_data.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_404_data_code.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_404_data_message.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_404_status.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_500.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_500_data.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_500_data_code.py
+Comment: 
+
+Filename: customgpt_client/models/list_project_sources_response_500_status.py
+Comment: 
+
 Filename: customgpt_client/models/list_projects_order.py
 Comment: 
 
 Filename: customgpt_client/models/list_projects_response_200.py
 Comment: 
 
 Filename: customgpt_client/models/list_projects_response_200_data.py
@@ -654,17 +984,14 @@
 
 Filename: customgpt_client/models/list_projects_response_200_data_data_item.py
 Comment: 
 
 Filename: customgpt_client/models/list_projects_response_200_data_data_item_type.py
 Comment: 
 
-Filename: customgpt_client/models/list_projects_response_200_data_links.py
-Comment: 
-
 Filename: customgpt_client/models/list_projects_response_200_status.py
 Comment: 
 
 Filename: customgpt_client/models/list_projects_response_401.py
 Comment: 
 
 Filename: customgpt_client/models/list_projects_response_401_data.py
@@ -690,24 +1017,24 @@
 
 Filename: customgpt_client/models/messages_order.py
 Comment: 
 
 Filename: customgpt_client/models/messages_response_200.py
 Comment: 
 
-Filename: customgpt_client/models/messages_response_200_conversation.py
+Filename: customgpt_client/models/messages_response_200_data.py
 Comment: 
 
-Filename: customgpt_client/models/messages_response_200_messages.py
+Filename: customgpt_client/models/messages_response_200_data_conversation.py
 Comment: 
 
-Filename: customgpt_client/models/messages_response_200_messages_data_item.py
+Filename: customgpt_client/models/messages_response_200_data_messages.py
 Comment: 
 
-Filename: customgpt_client/models/messages_response_200_messages_links.py
+Filename: customgpt_client/models/messages_response_200_data_messages_data_item.py
 Comment: 
 
 Filename: customgpt_client/models/messages_response_200_status.py
 Comment: 
 
 Filename: customgpt_client/models/messages_response_401.py
 Comment: 
@@ -807,14 +1134,23 @@
 
 Filename: customgpt_client/models/project_settings.py
 Comment: 
 
 Filename: customgpt_client/models/project_settings_response_source.py
 Comment: 
 
+Filename: customgpt_client/models/project_source.py
+Comment: 
+
+Filename: customgpt_client/models/project_source_settings.py
+Comment: 
+
+Filename: customgpt_client/models/project_source_type.py
+Comment: 
+
 Filename: customgpt_client/models/project_type.py
 Comment: 
 
 Filename: customgpt_client/models/prompt_history.py
 Comment: 
 
 Filename: customgpt_client/models/send_message_to_conversation_json_body.py
@@ -966,14 +1302,65 @@
 
 Filename: customgpt_client/models/update_project_conversation_response_500_status.py
 Comment: 
 
 Filename: customgpt_client/models/update_project_multipart_data.py
 Comment: 
 
+Filename: customgpt_client/models/update_project_plugin_json_body.py
+Comment: 
+
+Filename: customgpt_client/models/update_project_plugin_response_200.py
+Comment: 
+
+Filename: customgpt_client/models/update_project_plugin_response_200_data.py
+Comment: 
+
+Filename: customgpt_client/models/update_project_plugin_response_200_status.py
+Comment: 
+
+Filename: customgpt_client/models/update_project_plugin_response_401.py
+Comment: 
+
+Filename: customgpt_client/models/update_project_plugin_response_401_data.py
+Comment: 
+
+Filename: customgpt_client/models/update_project_plugin_response_401_data_code.py
+Comment: 
+
+Filename: customgpt_client/models/update_project_plugin_response_401_status.py
+Comment: 
+
+Filename: customgpt_client/models/update_project_plugin_response_404.py
+Comment: 
+
+Filename: customgpt_client/models/update_project_plugin_response_404_data.py
+Comment: 
+
+Filename: customgpt_client/models/update_project_plugin_response_404_data_code.py
+Comment: 
+
+Filename: customgpt_client/models/update_project_plugin_response_404_data_message.py
+Comment: 
+
+Filename: customgpt_client/models/update_project_plugin_response_404_status.py
+Comment: 
+
+Filename: customgpt_client/models/update_project_plugin_response_500.py
+Comment: 
+
+Filename: customgpt_client/models/update_project_plugin_response_500_data.py
+Comment: 
+
+Filename: customgpt_client/models/update_project_plugin_response_500_data_code.py
+Comment: 
+
+Filename: customgpt_client/models/update_project_plugin_response_500_status.py
+Comment: 
+
 Filename: customgpt_client/models/update_project_response_200.py
 Comment: 
 
 Filename: customgpt_client/models/update_project_response_200_data.py
 Comment: 
 
 Filename: customgpt_client/models/update_project_response_200_data_type.py
@@ -1113,17 +1500,17 @@
 
 Filename: customgpt_client/py.typed
 Comment: 
 
 Filename: customgpt_client/types.py
 Comment: 
 
-Filename: customgpt_client-1.1.2.dist-info/METADATA
+Filename: customgpt_client-1.1.3.dist-info/METADATA
 Comment: 
 
-Filename: customgpt_client-1.1.2.dist-info/WHEEL
+Filename: customgpt_client-1.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: customgpt_client-1.1.2.dist-info/RECORD
+Filename: customgpt_client-1.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## customgpt_client/api/citations/get_open_graph_data_for_citation.py

```diff
@@ -1,11 +1,12 @@
+import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
-import httpx
+import requests
 
 from ... import errors
 from ...models.get_open_graph_data_for_citation_response_200 import GetOpenGraphDataForCitationResponse200
 from ...models.get_open_graph_data_for_citation_response_401 import GetOpenGraphDataForCitationResponse401
 from ...models.get_open_graph_data_for_citation_response_404 import GetOpenGraphDataForCitationResponse404
 from ...types import Response
 
@@ -25,47 +26,47 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "allow_redirects": client.follow_redirects,
     }
 
 
 def _parse_response(
-    *, client: {}, response: httpx.Response
+    *, client: {}, response: None
 ) -> Optional[
     Union[
         GetOpenGraphDataForCitationResponse200,
         GetOpenGraphDataForCitationResponse401,
         GetOpenGraphDataForCitationResponse404,
     ]
 ]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetOpenGraphDataForCitationResponse200.from_dict(response.json())
+        response_200 = GetOpenGraphDataForCitationResponse200.from_dict(json.loads(response.text))
 
         return response_200
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = GetOpenGraphDataForCitationResponse401.from_dict(response.json())
+        response_401 = GetOpenGraphDataForCitationResponse401.from_dict(json.loads(response.text))
 
         return response_401
     if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = GetOpenGraphDataForCitationResponse404.from_dict(response.json())
+        response_404 = GetOpenGraphDataForCitationResponse404.from_dict(json.loads(response.text))
 
         return response_404
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: {}, response: httpx.Response, content: Optional[bytes] = None
+    *, client: {}, response: None, content: Optional[bytes] = None
 ) -> Response[
     Union[
         GetOpenGraphDataForCitationResponse200,
         GetOpenGraphDataForCitationResponse401,
         GetOpenGraphDataForCitationResponse404,
     ]
 ]:
@@ -102,16 +103,15 @@
 
     kwargs = _get_kwargs(
         project_id=project_id,
         citation_id=citation_id,
         client=client,
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = requests.request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
@@ -157,38 +157,23 @@
 ) -> Response[
     Union[
         GetOpenGraphDataForCitationResponse200,
         GetOpenGraphDataForCitationResponse401,
         GetOpenGraphDataForCitationResponse404,
     ]
 ]:
-    """Get the Open Graph data for a citation.
-
-     Get the Open Graph data for a citation by its unique identifier.
-
-    Args:
-        project_id (int):
-        citation_id (int):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[GetOpenGraphDataForCitationResponse200, GetOpenGraphDataForCitationResponse401, GetOpenGraphDataForCitationResponse404]]
-    """
-
     kwargs = _get_kwargs(
         project_id=project_id,
         citation_id=citation_id,
         client=client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    response = requests.request(
+        **kwargs,
+    )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_id: int,
     citation_id: int,
```

## customgpt_client/api/conversations/create_project_conversation.py

```diff
@@ -1,11 +1,12 @@
+import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
-import httpx
+import requests
 
 from ... import errors
 from ...models.create_project_conversation_json_body import CreateProjectConversationJsonBody
 from ...models.create_project_conversation_response_201 import CreateProjectConversationResponse201
 from ...models.create_project_conversation_response_401 import CreateProjectConversationResponse401
 from ...models.create_project_conversation_response_404 import CreateProjectConversationResponse404
 from ...models.create_project_conversation_response_500 import CreateProjectConversationResponse500
@@ -27,53 +28,53 @@
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "allow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
 def _parse_response(
-    *, client: {}, response: httpx.Response
+    *, client: {}, response: None
 ) -> Optional[
     Union[
         CreateProjectConversationResponse201,
         CreateProjectConversationResponse401,
         CreateProjectConversationResponse404,
         CreateProjectConversationResponse500,
     ]
 ]:
     if response.status_code == HTTPStatus.CREATED:
-        response_201 = CreateProjectConversationResponse201.from_dict(response.json())
+        response_201 = CreateProjectConversationResponse201.from_dict(json.loads(response.text))
 
         return response_201
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = CreateProjectConversationResponse401.from_dict(response.json())
+        response_401 = CreateProjectConversationResponse401.from_dict(json.loads(response.text))
 
         return response_401
     if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = CreateProjectConversationResponse404.from_dict(response.json())
+        response_404 = CreateProjectConversationResponse404.from_dict(json.loads(response.text))
 
         return response_404
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        response_500 = CreateProjectConversationResponse500.from_dict(response.json())
+        response_500 = CreateProjectConversationResponse500.from_dict(json.loads(response.text))
 
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: {}, response: httpx.Response, content: Optional[bytes] = None
+    *, client: {}, response: None, content: Optional[bytes] = None
 ) -> Response[
     Union[
         CreateProjectConversationResponse201,
         CreateProjectConversationResponse401,
         CreateProjectConversationResponse404,
         CreateProjectConversationResponse500,
     ]
@@ -111,16 +112,15 @@
 
     kwargs = _get_kwargs(
         project_id=project_id,
         client=client,
         json_body=json_body,
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = requests.request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
@@ -168,38 +168,23 @@
     Union[
         CreateProjectConversationResponse201,
         CreateProjectConversationResponse401,
         CreateProjectConversationResponse404,
         CreateProjectConversationResponse500,
     ]
 ]:
-    """Create a new conversation.
-
-     Create a new conversation for a project by `projectId`.
-
-    Args:
-        project_id (int):
-        json_body (CreateProjectConversationJsonBody):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[CreateProjectConversationResponse201, CreateProjectConversationResponse401, CreateProjectConversationResponse404, CreateProjectConversationResponse500]]
-    """
-
     kwargs = _get_kwargs(
         project_id=project_id,
         client=client,
         json_body=json_body,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    response = requests.request(
+        **kwargs,
+    )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_id: int,
     *,
```

## customgpt_client/api/conversations/delete_project_conversation.py

```diff
@@ -1,11 +1,12 @@
+import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
-import httpx
+import requests
 
 from ... import errors
 from ...models.delete_project_conversation_response_200 import DeleteProjectConversationResponse200
 from ...models.delete_project_conversation_response_401 import DeleteProjectConversationResponse401
 from ...models.delete_project_conversation_response_404 import DeleteProjectConversationResponse404
 from ...models.delete_project_conversation_response_500 import DeleteProjectConversationResponse500
 from ...types import Response
@@ -26,52 +27,52 @@
 
     return {
         "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "allow_redirects": client.follow_redirects,
     }
 
 
 def _parse_response(
-    *, client: {}, response: httpx.Response
+    *, client: {}, response: None
 ) -> Optional[
     Union[
         DeleteProjectConversationResponse200,
         DeleteProjectConversationResponse401,
         DeleteProjectConversationResponse404,
         DeleteProjectConversationResponse500,
     ]
 ]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = DeleteProjectConversationResponse200.from_dict(response.json())
+        response_200 = DeleteProjectConversationResponse200.from_dict(json.loads(response.text))
 
         return response_200
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = DeleteProjectConversationResponse401.from_dict(response.json())
+        response_401 = DeleteProjectConversationResponse401.from_dict(json.loads(response.text))
 
         return response_401
     if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = DeleteProjectConversationResponse404.from_dict(response.json())
+        response_404 = DeleteProjectConversationResponse404.from_dict(json.loads(response.text))
 
         return response_404
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        response_500 = DeleteProjectConversationResponse500.from_dict(response.json())
+        response_500 = DeleteProjectConversationResponse500.from_dict(json.loads(response.text))
 
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: {}, response: httpx.Response, content: Optional[bytes] = None
+    *, client: {}, response: None, content: Optional[bytes] = None
 ) -> Response[
     Union[
         DeleteProjectConversationResponse200,
         DeleteProjectConversationResponse401,
         DeleteProjectConversationResponse404,
         DeleteProjectConversationResponse500,
     ]
@@ -109,16 +110,15 @@
 
     kwargs = _get_kwargs(
         project_id=project_id,
         session_id=session_id,
         client=client,
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = requests.request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
@@ -166,38 +166,23 @@
     Union[
         DeleteProjectConversationResponse200,
         DeleteProjectConversationResponse401,
         DeleteProjectConversationResponse404,
         DeleteProjectConversationResponse500,
     ]
 ]:
-    """Delete a conversation.
-
-     Delete a conversation by `projectId` and `sessionId`.
-
-    Args:
-        project_id (int):
-        session_id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[DeleteProjectConversationResponse200, DeleteProjectConversationResponse401, DeleteProjectConversationResponse404, DeleteProjectConversationResponse500]]
-    """
-
     kwargs = _get_kwargs(
         project_id=project_id,
         session_id=session_id,
         client=client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    response = requests.request(
+        **kwargs,
+    )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_id: int,
     session_id: str,
```

## customgpt_client/api/conversations/get_project_conversations.py

```diff
@@ -1,11 +1,12 @@
+import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
-import httpx
+import requests
 
 from ... import errors
 from ...models.get_project_conversations_order import GetProjectConversationsOrder
 from ...models.get_project_conversations_response_200 import GetProjectConversationsResponse200
 from ...models.get_project_conversations_response_401 import GetProjectConversationsResponse401
 from ...models.get_project_conversations_response_404 import GetProjectConversationsResponse404
 from ...models.get_project_conversations_response_500 import GetProjectConversationsResponse500
@@ -37,53 +38,53 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "allow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
-    *, client: {}, response: httpx.Response
+    *, client: {}, response: None
 ) -> Optional[
     Union[
         GetProjectConversationsResponse200,
         GetProjectConversationsResponse401,
         GetProjectConversationsResponse404,
         GetProjectConversationsResponse500,
     ]
 ]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetProjectConversationsResponse200.from_dict(response.json())
+        response_200 = GetProjectConversationsResponse200.from_dict(json.loads(response.text))
 
         return response_200
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = GetProjectConversationsResponse401.from_dict(response.json())
+        response_401 = GetProjectConversationsResponse401.from_dict(json.loads(response.text))
 
         return response_401
     if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = GetProjectConversationsResponse404.from_dict(response.json())
+        response_404 = GetProjectConversationsResponse404.from_dict(json.loads(response.text))
 
         return response_404
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        response_500 = GetProjectConversationsResponse500.from_dict(response.json())
+        response_500 = GetProjectConversationsResponse500.from_dict(json.loads(response.text))
 
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: {}, response: httpx.Response, content: Optional[bytes] = None
+    *, client: {}, response: None, content: Optional[bytes] = None
 ) -> Response[
     Union[
         GetProjectConversationsResponse200,
         GetProjectConversationsResponse401,
         GetProjectConversationsResponse404,
         GetProjectConversationsResponse500,
     ]
@@ -124,16 +125,15 @@
     kwargs = _get_kwargs(
         project_id=project_id,
         client=client,
         page=page,
         order=order,
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = requests.request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
@@ -185,40 +185,24 @@
     Union[
         GetProjectConversationsResponse200,
         GetProjectConversationsResponse401,
         GetProjectConversationsResponse404,
         GetProjectConversationsResponse500,
     ]
 ]:
-    """List all conversations for a project
-    Retrieve all conversations for a project by `projectId`.
-
-    Args:
-        project_id (int):  Example: 1.
-        page (Union[Unset, None, int]):  Default: 1.
-        order (Union[Unset, None, GetProjectConversationsOrder]):  Default:
-            GetProjectConversationsOrder.DESC. Example: desc.
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[GetProjectConversationsResponse200, GetProjectConversationsResponse401, GetProjectConversationsResponse404, GetProjectConversationsResponse500]]
-    """
-
     kwargs = _get_kwargs(
         project_id=project_id,
         client=client,
         page=page,
         order=order,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    response = requests.request(
+        **kwargs,
+    )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_id: int,
     *,
```

## customgpt_client/api/conversations/messages.py

```diff
@@ -1,11 +1,12 @@
+import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
-import httpx
+import requests
 
 from ... import errors
 from ...models.messages_order import MessagesOrder
 from ...models.messages_response_200 import MessagesResponse200
 from ...models.messages_response_401 import MessagesResponse401
 from ...models.messages_response_404 import MessagesResponse404
 from ...models.messages_response_500 import MessagesResponse500
@@ -40,46 +41,46 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "allow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
-    *, client: {}, response: httpx.Response
+    *, client: {}, response: None
 ) -> Optional[Union[MessagesResponse200, MessagesResponse401, MessagesResponse404, MessagesResponse500]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = MessagesResponse200.from_dict(response.json())
+        response_200 = MessagesResponse200.from_dict(json.loads(response.text))
 
         return response_200
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = MessagesResponse401.from_dict(response.json())
+        response_401 = MessagesResponse401.from_dict(json.loads(response.text))
 
         return response_401
     if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = MessagesResponse404.from_dict(response.json())
+        response_404 = MessagesResponse404.from_dict(json.loads(response.text))
 
         return response_404
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        response_500 = MessagesResponse500.from_dict(response.json())
+        response_500 = MessagesResponse500.from_dict(json.loads(response.text))
 
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: {}, response: httpx.Response, content: Optional[bytes] = None
+    *, client: {}, response: None, content: Optional[bytes] = None
 ) -> Response[Union[MessagesResponse200, MessagesResponse401, MessagesResponse404, MessagesResponse500]]:
     parse = _parse_response(client=client, response=response)
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content if content is None else content,
         headers=response.headers,
         parsed=parse,
@@ -116,16 +117,15 @@
         project_id=project_id,
         session_id=session_id,
         client=client,
         page=page,
         order=order,
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = requests.request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
@@ -167,42 +167,25 @@
     project_id: int,
     session_id: str,
     *,
     client: {},
     page: Union[Unset, None, int] = 1,
     order: Union[Unset, None, MessagesOrder] = MessagesOrder.DESC,
 ) -> Response[Union[MessagesResponse200, MessagesResponse401, MessagesResponse404, MessagesResponse500]]:
-    """Retrieve messages that have been sent in a conversation.
-
-     Get all the messages that have been sent in a conversation by `projectId` and `sessionId`.
-
-    Args:
-        project_id (int):  Example: 1.
-        session_id (str):  Example: 1.
-        page (Union[Unset, None, int]):  Default: 1.
-        order (Union[Unset, None, MessagesOrder]):  Default: MessagesOrder.DESC. Example: desc.
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[MessagesResponse200, MessagesResponse401, MessagesResponse404, MessagesResponse500]]
-    """
-
     kwargs = _get_kwargs(
         project_id=project_id,
         session_id=session_id,
         client=client,
         page=page,
         order=order,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    response = requests.request(
+        **kwargs,
+    )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_id: int,
     session_id: str,
```

## customgpt_client/api/conversations/send_message_to_conversation.py

```diff
@@ -1,14 +1,13 @@
-import inspect
 import json
-import re
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
-import httpx
+import requests
+from sseclient import SSEClient
 
 from ... import errors
 from ...models.send_message_to_conversation_json_body import SendMessageToConversationJsonBody
 from ...models.send_message_to_conversation_response_200 import SendMessageToConversationResponse200
 from ...models.send_message_to_conversation_response_401 import SendMessageToConversationResponse401
 from ...models.send_message_to_conversation_response_404 import SendMessageToConversationResponse404
 from ...models.send_message_to_conversation_response_500 import SendMessageToConversationResponse500
@@ -28,107 +27,98 @@
         client.base_url, projectId=project_id, sessionId=session_id
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
-    params["stream"] = stream
+    params["stream"] = 1 if stream else 0
 
     params["lang"] = lang
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     json_json_body = json_body.to_dict()
 
+    if stream:
+        headers["Accept"] = "text/event-stream"
+
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "allow_redirects": client.follow_redirects,
         "json": json_json_body,
         "params": params,
+        "stream": stream,
     }
 
 
 def _parse_response(
-    *, client: {}, response: httpx.Response
+    *, client: {}, response: None
 ) -> Optional[
     Union[
         SendMessageToConversationResponse200,
         SendMessageToConversationResponse401,
         SendMessageToConversationResponse404,
         SendMessageToConversationResponse500,
     ]
 ]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = SendMessageToConversationResponse200.from_dict(response.json())
+        response_200 = SendMessageToConversationResponse200.from_dict(json.loads(response.text))
 
         return response_200
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = SendMessageToConversationResponse401.from_dict(response.json())
+        response_401 = SendMessageToConversationResponse401.from_dict(json.loads(response.text))
 
         return response_401
     if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = SendMessageToConversationResponse404.from_dict(response.json())
+        response_404 = SendMessageToConversationResponse404.from_dict(json.loads(response.text))
 
         return response_404
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        response_500 = SendMessageToConversationResponse500.from_dict(response.json())
+        response_500 = SendMessageToConversationResponse500.from_dict(json.loads(response.text))
 
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: {}, response: httpx.Response, content: Optional[bytes] = None
+    *, client: {}, response: None, content: Optional[bytes] = None
 ) -> Response[
     Union[
         SendMessageToConversationResponse200,
         SendMessageToConversationResponse401,
         SendMessageToConversationResponse404,
         SendMessageToConversationResponse500,
     ]
 ]:
-    caller_frame = inspect.currentframe().f_back
-    caller_method_name = caller_frame.f_code.co_name
-    parse = (
-        _parse_response(client=client, response=response)
-        if not caller_method_name in ["stream_detailed", "astream_detailed"]
-        else None
-    )
+    parse = _parse_response(client=client, response=response)
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content if content is None else content,
         headers=response.headers,
         parsed=parse,
     )
 
 
-def stream_detailed(
+def sync_detailed(
     project_id: int,
     session_id: str,
     *,
     client: {},
     json_body: SendMessageToConversationJsonBody,
     stream: Union[Unset, None, bool] = False,
     lang: Union[Unset, None, str] = "en",
-) -> Response[
-    Union[
-        SendMessageToConversationResponse200,
-        SendMessageToConversationResponse401,
-        SendMessageToConversationResponse404,
-        SendMessageToConversationResponse500,
-    ]
-]:
+):
     """Send a message to a conversation.
 
      Send a message to a conversation by `projectId` and `sessionId`.
 
     Args:
         project_id (int):  Example: 1.
         session_id (str):  Example: 1.
@@ -149,107 +139,21 @@
         session_id=session_id,
         client=client,
         json_body=json_body,
         stream=stream,
         lang=lang,
     )
 
-    response = httpx.request(**kwargs)
-    with httpx.stream(**kwargs) as response:
-        response_text = ""
-        for chunk in response.iter_text():
-            response_text += chunk
-
-        json_objects = re.findall(r"\{.*?\}", response_text)
-        for json_str in json_objects:
-            json_data = json.loads(json_str)
-            yield _build_response(client=client, response=response, content=json_data)
-
-
-async def astream_detailed(
-    project_id: int,
-    session_id: str,
-    *,
-    client: {},
-    json_body: SendMessageToConversationJsonBody,
-    stream: Union[Unset, None, bool] = False,
-    lang: Union[Unset, None, str] = "en",
-):
-    kwargs = _get_kwargs(
-        project_id=project_id,
-        session_id=session_id,
-        client=client,
-        json_body=json_body,
-        stream=stream,
-        lang=lang,
+    response = requests.request(
+        **kwargs,
     )
-    async with httpx.AsyncClient() as client:
-        async with client.stream(**kwargs) as response:
-            response_text = ""
-            async for chunk in response.aiter_text():
-                response_text += chunk
-
-            json_objects = re.findall(r"\{.*?\}", response_text)
-            for json_str in json_objects:
-                json_data = json.loads(json_str)
-                yield _build_response(client=client, response=response, content=json_data)
-
 
-def sync_detailed(
-    project_id: int,
-    session_id: str,
-    *,
-    client: {},
-    json_body: SendMessageToConversationJsonBody,
-    stream: Union[Unset, None, bool] = False,
-    lang: Union[Unset, None, str] = "en",
-):
     if stream:
-        yield from stream_detailed(
-            project_id=project_id,
-            session_id=session_id,
-            client=client,
-            json_body=json_body,
-            stream=stream,
-            lang=lang,
-        )
+        return SSEClient(response)
     else:
-        """Send a message to a conversation.
-
-         Send a message to a conversation by `projectId` and `sessionId`.
-
-        Args:
-            project_id (int):  Example: 1.
-            session_id (str):  Example: 1.
-            stream (Union[Unset, None, bool]):
-            lang (Union[Unset, None, str]):  Default: 'en'.
-            json_body (SendMessageToConversationJsonBody):
-
-        Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-            httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-        Returns:
-            Response[Union[SendMessageToConversationResponse200, SendMessageToConversationResponse401, SendMessageToConversationResponse404, SendMessageToConversationResponse500]]
-        """
-
-        kwargs = _get_kwargs(
-            project_id=project_id,
-            session_id=session_id,
-            client=client,
-            json_body=json_body,
-            stream=stream,
-            lang=lang,
-        )
-
-        response = httpx.request(
-            verify=client.verify_ssl,
-            **kwargs,
-        )
-
         return _build_response(client=client, response=response)
 
 
 def sync(
     project_id: int,
     session_id: str,
     *,
@@ -306,55 +210,30 @@
     Union[
         SendMessageToConversationResponse200,
         SendMessageToConversationResponse401,
         SendMessageToConversationResponse404,
         SendMessageToConversationResponse500,
     ]
 ]:
-    if stream:
-        return astream_detailed(
-            project_id=project_id,
-            session_id=session_id,
-            client=client,
-            json_body=json_body,
-            stream=stream,
-            lang=lang,
-        )
-    else:
-        """Send a message to a conversation.
-
-         Send a message to a conversation by `projectId` and `sessionId`.
-
-        Args:
-            project_id (int):  Example: 1.
-            session_id (str):  Example: 1.
-            stream (Union[Unset, None, bool]):
-            lang (Union[Unset, None, str]):  Default: 'en'.
-            json_body (SendMessageToConversationJsonBody):
-
-        Raises:
-            errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-            httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-        Returns:
-            Response[Union[SendMessageToConversationResponse200, SendMessageToConversationResponse401, SendMessageToConversationResponse404, SendMessageToConversationResponse500]]
-        """
-
-        kwargs = _get_kwargs(
-            project_id=project_id,
-            session_id=session_id,
-            client=client,
-            json_body=json_body,
-            stream=stream,
-            lang=lang,
-        )
+    kwargs = _get_kwargs(
+        project_id=project_id,
+        session_id=session_id,
+        client=client,
+        json_body=json_body,
+        stream=stream,
+        lang=lang,
+    )
 
-        async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-            response = await _client.request(**kwargs)
+    response = requests.request(
+        **kwargs,
+    )
 
+    if stream:
+        return SSEClient(response)
+    else:
         return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_id: int,
     session_id: str,
     *,
```

## customgpt_client/api/conversations/update_project_conversation.py

```diff
@@ -1,11 +1,12 @@
+import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
-import httpx
+import requests
 
 from ... import errors
 from ...models.update_project_conversation_json_body import UpdateProjectConversationJsonBody
 from ...models.update_project_conversation_response_200 import UpdateProjectConversationResponse200
 from ...models.update_project_conversation_response_401 import UpdateProjectConversationResponse401
 from ...models.update_project_conversation_response_404 import UpdateProjectConversationResponse404
 from ...models.update_project_conversation_response_500 import UpdateProjectConversationResponse500
@@ -30,53 +31,53 @@
 
     return {
         "method": "put",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "allow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
 def _parse_response(
-    *, client: {}, response: httpx.Response
+    *, client: {}, response: None
 ) -> Optional[
     Union[
         UpdateProjectConversationResponse200,
         UpdateProjectConversationResponse401,
         UpdateProjectConversationResponse404,
         UpdateProjectConversationResponse500,
     ]
 ]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = UpdateProjectConversationResponse200.from_dict(response.json())
+        response_200 = UpdateProjectConversationResponse200.from_dict(json.loads(response.text))
 
         return response_200
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = UpdateProjectConversationResponse401.from_dict(response.json())
+        response_401 = UpdateProjectConversationResponse401.from_dict(json.loads(response.text))
 
         return response_401
     if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = UpdateProjectConversationResponse404.from_dict(response.json())
+        response_404 = UpdateProjectConversationResponse404.from_dict(json.loads(response.text))
 
         return response_404
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        response_500 = UpdateProjectConversationResponse500.from_dict(response.json())
+        response_500 = UpdateProjectConversationResponse500.from_dict(json.loads(response.text))
 
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: {}, response: httpx.Response, content: Optional[bytes] = None
+    *, client: {}, response: None, content: Optional[bytes] = None
 ) -> Response[
     Union[
         UpdateProjectConversationResponse200,
         UpdateProjectConversationResponse401,
         UpdateProjectConversationResponse404,
         UpdateProjectConversationResponse500,
     ]
@@ -117,16 +118,15 @@
     kwargs = _get_kwargs(
         project_id=project_id,
         session_id=session_id,
         client=client,
         json_body=json_body,
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = requests.request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
@@ -178,40 +178,24 @@
     Union[
         UpdateProjectConversationResponse200,
         UpdateProjectConversationResponse401,
         UpdateProjectConversationResponse404,
         UpdateProjectConversationResponse500,
     ]
 ]:
-    """Update a conversation.
-
-     Update a conversation by `projectId` and `sessionId`.
-
-    Args:
-        project_id (int):
-        session_id (str):
-        json_body (UpdateProjectConversationJsonBody):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[UpdateProjectConversationResponse200, UpdateProjectConversationResponse401, UpdateProjectConversationResponse404, UpdateProjectConversationResponse500]]
-    """
-
     kwargs = _get_kwargs(
         project_id=project_id,
         session_id=session_id,
         client=client,
         json_body=json_body,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    response = requests.request(
+        **kwargs,
+    )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_id: int,
     session_id: str,
```

## customgpt_client/api/pages/delete_project_page.py

```diff
@@ -1,11 +1,12 @@
+import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
-import httpx
+import requests
 
 from ... import errors
 from ...models.delete_project_page_response_200 import DeleteProjectPageResponse200
 from ...models.delete_project_page_response_401 import DeleteProjectPageResponse401
 from ...models.delete_project_page_response_404 import DeleteProjectPageResponse404
 from ...models.delete_project_page_response_500 import DeleteProjectPageResponse500
 from ...types import Response
@@ -24,52 +25,52 @@
 
     return {
         "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "allow_redirects": client.follow_redirects,
     }
 
 
 def _parse_response(
-    *, client: {}, response: httpx.Response
+    *, client: {}, response: None
 ) -> Optional[
     Union[
         DeleteProjectPageResponse200,
         DeleteProjectPageResponse401,
         DeleteProjectPageResponse404,
         DeleteProjectPageResponse500,
     ]
 ]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = DeleteProjectPageResponse200.from_dict(response.json())
+        response_200 = DeleteProjectPageResponse200.from_dict(json.loads(response.text))
 
         return response_200
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = DeleteProjectPageResponse401.from_dict(response.json())
+        response_401 = DeleteProjectPageResponse401.from_dict(json.loads(response.text))
 
         return response_401
     if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = DeleteProjectPageResponse404.from_dict(response.json())
+        response_404 = DeleteProjectPageResponse404.from_dict(json.loads(response.text))
 
         return response_404
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        response_500 = DeleteProjectPageResponse500.from_dict(response.json())
+        response_500 = DeleteProjectPageResponse500.from_dict(json.loads(response.text))
 
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: {}, response: httpx.Response, content: Optional[bytes] = None
+    *, client: {}, response: None, content: Optional[bytes] = None
 ) -> Response[
     Union[
         DeleteProjectPageResponse200,
         DeleteProjectPageResponse401,
         DeleteProjectPageResponse404,
         DeleteProjectPageResponse500,
     ]
@@ -107,16 +108,15 @@
 
     kwargs = _get_kwargs(
         project_id=project_id,
         page_id=page_id,
         client=client,
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = requests.request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
@@ -164,38 +164,23 @@
     Union[
         DeleteProjectPageResponse200,
         DeleteProjectPageResponse401,
         DeleteProjectPageResponse404,
         DeleteProjectPageResponse500,
     ]
 ]:
-    """Delete a certain page that belongs to a certain project.
-
-     Delete a certain page of a specific project by `projectId` and `pageId`.
-
-    Args:
-        project_id (int):
-        page_id (int):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[DeleteProjectPageResponse200, DeleteProjectPageResponse401, DeleteProjectPageResponse404, DeleteProjectPageResponse500]]
-    """
-
     kwargs = _get_kwargs(
         project_id=project_id,
         page_id=page_id,
         client=client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    response = requests.request(
+        **kwargs,
+    )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_id: int,
     page_id: int,
```

## customgpt_client/api/pages/get_project_pages.py

```diff
@@ -1,11 +1,12 @@
+import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
-import httpx
+import requests
 
 from ... import errors
 from ...models.get_project_pages_order import GetProjectPagesOrder
 from ...models.get_project_pages_response_200 import GetProjectPagesResponse200
 from ...models.get_project_pages_response_401 import GetProjectPagesResponse401
 from ...models.get_project_pages_response_404 import GetProjectPagesResponse404
 from ...models.get_project_pages_response_500 import GetProjectPagesResponse500
@@ -40,50 +41,50 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "allow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
-    *, client: {}, response: httpx.Response
+    *, client: {}, response: None
 ) -> Optional[
     Union[
         GetProjectPagesResponse200, GetProjectPagesResponse401, GetProjectPagesResponse404, GetProjectPagesResponse500
     ]
 ]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetProjectPagesResponse200.from_dict(response.json())
+        response_200 = GetProjectPagesResponse200.from_dict(json.loads(response.text))
 
         return response_200
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = GetProjectPagesResponse401.from_dict(response.json())
+        response_401 = GetProjectPagesResponse401.from_dict(json.loads(response.text))
 
         return response_401
     if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = GetProjectPagesResponse404.from_dict(response.json())
+        response_404 = GetProjectPagesResponse404.from_dict(json.loads(response.text))
 
         return response_404
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        response_500 = GetProjectPagesResponse500.from_dict(response.json())
+        response_500 = GetProjectPagesResponse500.from_dict(json.loads(response.text))
 
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: {}, response: httpx.Response, content: Optional[bytes] = None
+    *, client: {}, response: None, content: Optional[bytes] = None
 ) -> Response[
     Union[
         GetProjectPagesResponse200, GetProjectPagesResponse401, GetProjectPagesResponse404, GetProjectPagesResponse500
     ]
 ]:
     parse = _parse_response(client=client, response=response)
     return Response(
@@ -124,16 +125,15 @@
         project_id=project_id,
         client=client,
         page=page,
         duration=duration,
         order=order,
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = requests.request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
@@ -183,42 +183,25 @@
     duration: Union[Unset, None, int] = 90,
     order: Union[Unset, None, GetProjectPagesOrder] = GetProjectPagesOrder.DESC,
 ) -> Response[
     Union[
         GetProjectPagesResponse200, GetProjectPagesResponse401, GetProjectPagesResponse404, GetProjectPagesResponse500
     ]
 ]:
-    """List all pages that belong to a project.
-
-     Get a list of all pages that belong to a project.
-
-    Args:
-        project_id (int):  Example: 1.
-        page (Union[Unset, None, int]):  Default: 1.
-        duration (Union[Unset, None, int]):  Default: 90.
-        order (Union[Unset, None, GetProjectPagesOrder]):  Default: GetProjectPagesOrder.DESC.
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[GetProjectPagesResponse200, GetProjectPagesResponse401, GetProjectPagesResponse404, GetProjectPagesResponse500]]
-    """
-
     kwargs = _get_kwargs(
         project_id=project_id,
         client=client,
         page=page,
         duration=duration,
         order=order,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    response = requests.request(
+        **kwargs,
+    )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_id: int,
     *,
```

## customgpt_client/api/pages/preview.py

```diff
@@ -1,11 +1,12 @@
+import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
-import httpx
+import requests
 
 from ... import errors
 from ...models.preview_response_401 import PreviewResponse401
 from ...models.preview_response_404 import PreviewResponse404
 from ...models.preview_response_500 import PreviewResponse500
 from ...types import Response
 
@@ -22,41 +23,41 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "allow_redirects": client.follow_redirects,
     }
 
 
 def _parse_response(
-    *, client: {}, response: httpx.Response
+    *, client: {}, response: None
 ) -> Optional[Union[PreviewResponse401, PreviewResponse404, PreviewResponse500]]:
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = PreviewResponse401.from_dict(response.json())
+        response_401 = PreviewResponse401.from_dict(json.loads(response.text))
 
         return response_401
     if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = PreviewResponse404.from_dict(response.json())
+        response_404 = PreviewResponse404.from_dict(json.loads(response.text))
 
         return response_404
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        response_500 = PreviewResponse500.from_dict(response.json())
+        response_500 = PreviewResponse500.from_dict(json.loads(response.text))
 
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: {}, response: httpx.Response, content: Optional[bytes] = None
+    *, client: {}, response: None, content: Optional[bytes] = None
 ) -> Response[Union[PreviewResponse401, PreviewResponse404, PreviewResponse500]]:
     parse = _parse_response(client=client, response=response)
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content if content is None else content,
         headers=response.headers,
         parsed=parse,
@@ -82,16 +83,15 @@
     """
 
     kwargs = _get_kwargs(
         id=id,
         client=client,
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = requests.request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
@@ -119,34 +119,22 @@
 
 
 async def asyncio_detailed(
     id: str,
     *,
     client: {},
 ) -> Response[Union[PreviewResponse401, PreviewResponse404, PreviewResponse500]]:
-    """Preview file from citation.
-
-    Args:
-        id (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[PreviewResponse401, PreviewResponse404, PreviewResponse500]]
-    """
-
     kwargs = _get_kwargs(
         id=id,
         client=client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    response = requests.request(
+        **kwargs,
+    )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     id: str,
     *,
```

## customgpt_client/api/project_settings/get_project_settings.py

```diff
@@ -1,11 +1,12 @@
+import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
-import httpx
+import requests
 
 from ... import errors
 from ...models.get_project_settings_response_200 import GetProjectSettingsResponse200
 from ...models.get_project_settings_response_401 import GetProjectSettingsResponse401
 from ...models.get_project_settings_response_404 import GetProjectSettingsResponse404
 from ...models.get_project_settings_response_500 import GetProjectSettingsResponse500
 from ...types import Response
@@ -23,52 +24,52 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "allow_redirects": client.follow_redirects,
     }
 
 
 def _parse_response(
-    *, client: {}, response: httpx.Response
+    *, client: {}, response: None
 ) -> Optional[
     Union[
         GetProjectSettingsResponse200,
         GetProjectSettingsResponse401,
         GetProjectSettingsResponse404,
         GetProjectSettingsResponse500,
     ]
 ]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetProjectSettingsResponse200.from_dict(response.json())
+        response_200 = GetProjectSettingsResponse200.from_dict(json.loads(response.text))
 
         return response_200
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = GetProjectSettingsResponse401.from_dict(response.json())
+        response_401 = GetProjectSettingsResponse401.from_dict(json.loads(response.text))
 
         return response_401
     if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = GetProjectSettingsResponse404.from_dict(response.json())
+        response_404 = GetProjectSettingsResponse404.from_dict(json.loads(response.text))
 
         return response_404
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        response_500 = GetProjectSettingsResponse500.from_dict(response.json())
+        response_500 = GetProjectSettingsResponse500.from_dict(json.loads(response.text))
 
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: {}, response: httpx.Response, content: Optional[bytes] = None
+    *, client: {}, response: None, content: Optional[bytes] = None
 ) -> Response[
     Union[
         GetProjectSettingsResponse200,
         GetProjectSettingsResponse401,
         GetProjectSettingsResponse404,
         GetProjectSettingsResponse500,
     ]
@@ -103,16 +104,15 @@
     """
 
     kwargs = _get_kwargs(
         project_id=project_id,
         client=client,
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = requests.request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
@@ -156,36 +156,22 @@
     Union[
         GetProjectSettingsResponse200,
         GetProjectSettingsResponse401,
         GetProjectSettingsResponse404,
         GetProjectSettingsResponse500,
     ]
 ]:
-    """Get project settings.
-
-     Retrieve the current project settings for a project.
-
-    Args:
-        project_id (int):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[GetProjectSettingsResponse200, GetProjectSettingsResponse401, GetProjectSettingsResponse404, GetProjectSettingsResponse500]]
-    """
-
     kwargs = _get_kwargs(
         project_id=project_id,
         client=client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    response = requests.request(
+        **kwargs,
+    )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_id: int,
     *,
```

## customgpt_client/api/project_settings/update_project_settings.py

```diff
@@ -1,11 +1,12 @@
+import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
-import httpx
+import requests
 
 from ... import errors
 from ...models.update_project_settings_multipart_data import UpdateProjectSettingsMultipartData
 from ...models.update_project_settings_response_200 import UpdateProjectSettingsResponse200
 from ...models.update_project_settings_response_400 import UpdateProjectSettingsResponse400
 from ...models.update_project_settings_response_401 import UpdateProjectSettingsResponse401
 from ...models.update_project_settings_response_500 import UpdateProjectSettingsResponse500
@@ -27,53 +28,53 @@
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "allow_redirects": client.follow_redirects,
         "files": multipart_multipart_data,
     }
 
 
 def _parse_response(
-    *, client: {}, response: httpx.Response
+    *, client: {}, response: None
 ) -> Optional[
     Union[
         UpdateProjectSettingsResponse200,
         UpdateProjectSettingsResponse400,
         UpdateProjectSettingsResponse401,
         UpdateProjectSettingsResponse500,
     ]
 ]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = UpdateProjectSettingsResponse200.from_dict(response.json())
+        response_200 = UpdateProjectSettingsResponse200.from_dict(json.loads(response.text))
 
         return response_200
     if response.status_code == HTTPStatus.BAD_REQUEST:
-        response_400 = UpdateProjectSettingsResponse400.from_dict(response.json())
+        response_400 = UpdateProjectSettingsResponse400.from_dict(json.loads(response.text))
 
         return response_400
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = UpdateProjectSettingsResponse401.from_dict(response.json())
+        response_401 = UpdateProjectSettingsResponse401.from_dict(json.loads(response.text))
 
         return response_401
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        response_500 = UpdateProjectSettingsResponse500.from_dict(response.json())
+        response_500 = UpdateProjectSettingsResponse500.from_dict(json.loads(response.text))
 
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: {}, response: httpx.Response, content: Optional[bytes] = None
+    *, client: {}, response: None, content: Optional[bytes] = None
 ) -> Response[
     Union[
         UpdateProjectSettingsResponse200,
         UpdateProjectSettingsResponse400,
         UpdateProjectSettingsResponse401,
         UpdateProjectSettingsResponse500,
     ]
@@ -111,16 +112,15 @@
 
     kwargs = _get_kwargs(
         project_id=project_id,
         client=client,
         multipart_data=multipart_data,
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = requests.request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
@@ -168,38 +168,23 @@
     Union[
         UpdateProjectSettingsResponse200,
         UpdateProjectSettingsResponse400,
         UpdateProjectSettingsResponse401,
         UpdateProjectSettingsResponse500,
     ]
 ]:
-    """Update project settings.
-
-     Update project settings of a specific project by `projectId`.
-
-    Args:
-        project_id (int):
-        multipart_data (UpdateProjectSettingsMultipartData):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[UpdateProjectSettingsResponse200, UpdateProjectSettingsResponse400, UpdateProjectSettingsResponse401, UpdateProjectSettingsResponse500]]
-    """
-
     kwargs = _get_kwargs(
         project_id=project_id,
         client=client,
         multipart_data=multipart_data,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    response = requests.request(
+        **kwargs,
+    )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_id: int,
     *,
```

## customgpt_client/api/projects/create_project.py

```diff
@@ -1,11 +1,12 @@
+import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
-import httpx
+import requests
 
 from ... import errors
 from ...models.create_project_multipart_data import CreateProjectMultipartData
 from ...models.create_project_response_201 import CreateProjectResponse201
 from ...models.create_project_response_400 import CreateProjectResponse400
 from ...models.create_project_response_401 import CreateProjectResponse401
 from ...models.create_project_response_500 import CreateProjectResponse500
@@ -26,48 +27,48 @@
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "allow_redirects": client.follow_redirects,
         "files": multipart_multipart_data,
     }
 
 
 def _parse_response(
-    *, client: {}, response: httpx.Response
+    *, client: {}, response: None
 ) -> Optional[
     Union[CreateProjectResponse201, CreateProjectResponse400, CreateProjectResponse401, CreateProjectResponse500]
 ]:
     if response.status_code == HTTPStatus.CREATED:
-        response_201 = CreateProjectResponse201.from_dict(response.json())
+        response_201 = CreateProjectResponse201.from_dict(json.loads(response.text))
 
         return response_201
     if response.status_code == HTTPStatus.BAD_REQUEST:
-        response_400 = CreateProjectResponse400.from_dict(response.json())
+        response_400 = CreateProjectResponse400.from_dict(json.loads(response.text))
 
         return response_400
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = CreateProjectResponse401.from_dict(response.json())
+        response_401 = CreateProjectResponse401.from_dict(json.loads(response.text))
 
         return response_401
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        response_500 = CreateProjectResponse500.from_dict(response.json())
+        response_500 = CreateProjectResponse500.from_dict(json.loads(response.text))
 
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: {}, response: httpx.Response, content: Optional[bytes] = None
+    *, client: {}, response: None, content: Optional[bytes] = None
 ) -> Response[
     Union[CreateProjectResponse201, CreateProjectResponse400, CreateProjectResponse401, CreateProjectResponse500]
 ]:
     parse = _parse_response(client=client, response=response)
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content if content is None else content,
@@ -97,16 +98,15 @@
     """
 
     kwargs = _get_kwargs(
         client=client,
         multipart_data=multipart_data,
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = requests.request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
@@ -140,36 +140,22 @@
 async def asyncio_detailed(
     *,
     client: {},
     multipart_data: CreateProjectMultipartData,
 ) -> Response[
     Union[CreateProjectResponse201, CreateProjectResponse400, CreateProjectResponse401, CreateProjectResponse500]
 ]:
-    """Create a new project.
-
-     Create a new project from either sitemap or uploaded file.
-
-    Args:
-        multipart_data (CreateProjectMultipartData):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[CreateProjectResponse201, CreateProjectResponse400, CreateProjectResponse401, CreateProjectResponse500]]
-    """
-
     kwargs = _get_kwargs(
         client=client,
         multipart_data=multipart_data,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    response = requests.request(
+        **kwargs,
+    )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: {},
```

## customgpt_client/api/projects/delete_project.py

```diff
@@ -1,11 +1,12 @@
+import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
-import httpx
+import requests
 
 from ... import errors
 from ...models.delete_project_response_200 import DeleteProjectResponse200
 from ...models.delete_project_response_401 import DeleteProjectResponse401
 from ...models.delete_project_response_404 import DeleteProjectResponse404
 from ...models.delete_project_response_500 import DeleteProjectResponse500
 from ...types import Response
@@ -23,47 +24,47 @@
 
     return {
         "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "allow_redirects": client.follow_redirects,
     }
 
 
 def _parse_response(
-    *, client: {}, response: httpx.Response
+    *, client: {}, response: None
 ) -> Optional[
     Union[DeleteProjectResponse200, DeleteProjectResponse401, DeleteProjectResponse404, DeleteProjectResponse500]
 ]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = DeleteProjectResponse200.from_dict(response.json())
+        response_200 = DeleteProjectResponse200.from_dict(json.loads(response.text))
 
         return response_200
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = DeleteProjectResponse401.from_dict(response.json())
+        response_401 = DeleteProjectResponse401.from_dict(json.loads(response.text))
 
         return response_401
     if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = DeleteProjectResponse404.from_dict(response.json())
+        response_404 = DeleteProjectResponse404.from_dict(json.loads(response.text))
 
         return response_404
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        response_500 = DeleteProjectResponse500.from_dict(response.json())
+        response_500 = DeleteProjectResponse500.from_dict(json.loads(response.text))
 
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: {}, response: httpx.Response, content: Optional[bytes] = None
+    *, client: {}, response: None, content: Optional[bytes] = None
 ) -> Response[
     Union[DeleteProjectResponse200, DeleteProjectResponse401, DeleteProjectResponse404, DeleteProjectResponse500]
 ]:
     parse = _parse_response(client=client, response=response)
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content if content is None else content,
@@ -93,16 +94,15 @@
     """
 
     kwargs = _get_kwargs(
         project_id=project_id,
         client=client,
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = requests.request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
@@ -136,36 +136,22 @@
 async def asyncio_detailed(
     project_id: int,
     *,
     client: {},
 ) -> Response[
     Union[DeleteProjectResponse200, DeleteProjectResponse401, DeleteProjectResponse404, DeleteProjectResponse500]
 ]:
-    """Delete a certain project.
-
-     Delete an existing project by project ID.
-
-    Args:
-        project_id (int):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[DeleteProjectResponse200, DeleteProjectResponse401, DeleteProjectResponse404, DeleteProjectResponse500]]
-    """
-
     kwargs = _get_kwargs(
         project_id=project_id,
         client=client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    response = requests.request(
+        **kwargs,
+    )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_id: int,
     *,
```

## customgpt_client/api/projects/get_project.py

```diff
@@ -1,11 +1,12 @@
+import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
-import httpx
+import requests
 
 from ... import errors
 from ...models.get_project_response_200 import GetProjectResponse200
 from ...models.get_project_response_401 import GetProjectResponse401
 from ...models.get_project_response_404 import GetProjectResponse404
 from ...models.get_project_response_500 import GetProjectResponse500
 from ...types import UNSET, Response, Unset
@@ -32,46 +33,46 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "allow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
-    *, client: {}, response: httpx.Response
+    *, client: {}, response: None
 ) -> Optional[Union[GetProjectResponse200, GetProjectResponse401, GetProjectResponse404, GetProjectResponse500]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetProjectResponse200.from_dict(response.json())
+        response_200 = GetProjectResponse200.from_dict(json.loads(response.text))
 
         return response_200
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = GetProjectResponse401.from_dict(response.json())
+        response_401 = GetProjectResponse401.from_dict(json.loads(response.text))
 
         return response_401
     if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = GetProjectResponse404.from_dict(response.json())
+        response_404 = GetProjectResponse404.from_dict(json.loads(response.text))
 
         return response_404
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        response_500 = GetProjectResponse500.from_dict(response.json())
+        response_500 = GetProjectResponse500.from_dict(json.loads(response.text))
 
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: {}, response: httpx.Response, content: Optional[bytes] = None
+    *, client: {}, response: None, content: Optional[bytes] = None
 ) -> Response[Union[GetProjectResponse200, GetProjectResponse401, GetProjectResponse404, GetProjectResponse500]]:
     parse = _parse_response(client=client, response=response)
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content if content is None else content,
         headers=response.headers,
         parsed=parse,
@@ -105,16 +106,15 @@
     kwargs = _get_kwargs(
         project_id=project_id,
         client=client,
         width=width,
         height=height,
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = requests.request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
@@ -152,40 +152,24 @@
 async def asyncio_detailed(
     project_id: int,
     *,
     client: {},
     width: Union[Unset, None, str] = "100%",
     height: Union[Unset, None, str] = "auto",
 ) -> Response[Union[GetProjectResponse200, GetProjectResponse401, GetProjectResponse404, GetProjectResponse500]]:
-    """Show a certain project.
-
-     View a specific project by project ID.
-
-    Args:
-        project_id (int):  Example: 1.
-        width (Union[Unset, None, str]):  Default: '100%'. Example: 50rem.
-        height (Union[Unset, None, str]):  Default: 'auto'. Example: 50rem.
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[GetProjectResponse200, GetProjectResponse401, GetProjectResponse404, GetProjectResponse500]]
-    """
-
     kwargs = _get_kwargs(
         project_id=project_id,
         client=client,
         width=width,
         height=height,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    response = requests.request(
+        **kwargs,
+    )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_id: int,
     *,
```

## customgpt_client/api/projects/list_projects.py

```diff
@@ -1,11 +1,12 @@
+import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
-import httpx
+import requests
 
 from ... import errors
 from ...models.list_projects_order import ListProjectsOrder
 from ...models.list_projects_response_200 import ListProjectsResponse200
 from ...models.list_projects_response_401 import ListProjectsResponse401
 from ...models.list_projects_response_500 import ListProjectsResponse500
 from ...types import UNSET, Response, Unset
@@ -44,42 +45,42 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "allow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
-    *, client: {}, response: httpx.Response
+    *, client: {}, response: None
 ) -> Optional[Union[ListProjectsResponse200, ListProjectsResponse401, ListProjectsResponse500]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ListProjectsResponse200.from_dict(response.json())
+        response_200 = ListProjectsResponse200.from_dict(json.loads(response.text))
 
         return response_200
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = ListProjectsResponse401.from_dict(response.json())
+        response_401 = ListProjectsResponse401.from_dict(json.loads(response.text))
 
         return response_401
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        response_500 = ListProjectsResponse500.from_dict(response.json())
+        response_500 = ListProjectsResponse500.from_dict(json.loads(response.text))
 
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: {}, response: httpx.Response, content: Optional[bytes] = None
+    *, client: {}, response: None, content: Optional[bytes] = None
 ) -> Response[Union[ListProjectsResponse200, ListProjectsResponse401, ListProjectsResponse500]]:
     parse = _parse_response(client=client, response=response)
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content if content is None else content,
         headers=response.headers,
         parsed=parse,
@@ -119,16 +120,15 @@
         page=page,
         duration=duration,
         order=order,
         width=width,
         height=height,
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = requests.request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
@@ -174,44 +174,26 @@
     client: {},
     page: Union[Unset, None, int] = 1,
     duration: Union[Unset, None, int] = 90,
     order: Union[Unset, None, ListProjectsOrder] = ListProjectsOrder.DESC,
     width: Union[Unset, None, str] = "100%",
     height: Union[Unset, None, str] = "auto",
 ) -> Response[Union[ListProjectsResponse200, ListProjectsResponse401, ListProjectsResponse500]]:
-    """List all projects.
-
-     Get a list of all projects that belong to the user.
-
-    Args:
-        page (Union[Unset, None, int]):  Default: 1.
-        duration (Union[Unset, None, int]):  Default: 90.
-        order (Union[Unset, None, ListProjectsOrder]):  Default: ListProjectsOrder.DESC.
-        width (Union[Unset, None, str]):  Default: '100%'. Example: 50rem.
-        height (Union[Unset, None, str]):  Default: 'auto'. Example: 50rem.
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[ListProjectsResponse200, ListProjectsResponse401, ListProjectsResponse500]]
-    """
-
     kwargs = _get_kwargs(
         client=client,
         page=page,
         duration=duration,
         order=order,
         width=width,
         height=height,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    response = requests.request(
+        **kwargs,
+    )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: {},
```

## customgpt_client/api/projects/stats_project.py

```diff
@@ -1,11 +1,12 @@
+import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
-import httpx
+import requests
 
 from ... import errors
 from ...models.stats_project_response_200 import StatsProjectResponse200
 from ...models.stats_project_response_401 import StatsProjectResponse401
 from ...models.stats_project_response_404 import StatsProjectResponse404
 from ...models.stats_project_response_500 import StatsProjectResponse500
 from ...types import Response
@@ -23,47 +24,47 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "allow_redirects": client.follow_redirects,
     }
 
 
 def _parse_response(
-    *, client: {}, response: httpx.Response
+    *, client: {}, response: None
 ) -> Optional[
     Union[StatsProjectResponse200, StatsProjectResponse401, StatsProjectResponse404, StatsProjectResponse500]
 ]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = StatsProjectResponse200.from_dict(response.json())
+        response_200 = StatsProjectResponse200.from_dict(json.loads(response.text))
 
         return response_200
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = StatsProjectResponse401.from_dict(response.json())
+        response_401 = StatsProjectResponse401.from_dict(json.loads(response.text))
 
         return response_401
     if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = StatsProjectResponse404.from_dict(response.json())
+        response_404 = StatsProjectResponse404.from_dict(json.loads(response.text))
 
         return response_404
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        response_500 = StatsProjectResponse500.from_dict(response.json())
+        response_500 = StatsProjectResponse500.from_dict(json.loads(response.text))
 
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: {}, response: httpx.Response, content: Optional[bytes] = None
+    *, client: {}, response: None, content: Optional[bytes] = None
 ) -> Response[
     Union[StatsProjectResponse200, StatsProjectResponse401, StatsProjectResponse404, StatsProjectResponse500]
 ]:
     parse = _parse_response(client=client, response=response)
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content if content is None else content,
@@ -93,16 +94,15 @@
     """
 
     kwargs = _get_kwargs(
         project_id=project_id,
         client=client,
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = requests.request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
@@ -136,36 +136,22 @@
 async def asyncio_detailed(
     project_id: int,
     *,
     client: {},
 ) -> Response[
     Union[StatsProjectResponse200, StatsProjectResponse401, StatsProjectResponse404, StatsProjectResponse500]
 ]:
-    """Get the stats for a certain project.
-
-     Get the stats for a project by `projectId`.
-
-    Args:
-        project_id (int):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[StatsProjectResponse200, StatsProjectResponse401, StatsProjectResponse404, StatsProjectResponse500]]
-    """
-
     kwargs = _get_kwargs(
         project_id=project_id,
         client=client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    response = requests.request(
+        **kwargs,
+    )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_id: int,
     *,
```

## customgpt_client/api/projects/update_project.py

```diff
@@ -1,11 +1,12 @@
+import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
-import httpx
+import requests
 
 from ... import errors
 from ...models.update_project_multipart_data import UpdateProjectMultipartData
 from ...models.update_project_response_200 import UpdateProjectResponse200
 from ...models.update_project_response_401 import UpdateProjectResponse401
 from ...models.update_project_response_404 import UpdateProjectResponse404
 from ...models.update_project_response_500 import UpdateProjectResponse500
@@ -27,48 +28,48 @@
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "allow_redirects": client.follow_redirects,
         "files": multipart_multipart_data,
     }
 
 
 def _parse_response(
-    *, client: {}, response: httpx.Response
+    *, client: {}, response: None
 ) -> Optional[
     Union[UpdateProjectResponse200, UpdateProjectResponse401, UpdateProjectResponse404, UpdateProjectResponse500]
 ]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = UpdateProjectResponse200.from_dict(response.json())
+        response_200 = UpdateProjectResponse200.from_dict(json.loads(response.text))
 
         return response_200
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = UpdateProjectResponse401.from_dict(response.json())
+        response_401 = UpdateProjectResponse401.from_dict(json.loads(response.text))
 
         return response_401
     if response.status_code == HTTPStatus.NOT_FOUND:
-        response_404 = UpdateProjectResponse404.from_dict(response.json())
+        response_404 = UpdateProjectResponse404.from_dict(json.loads(response.text))
 
         return response_404
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        response_500 = UpdateProjectResponse500.from_dict(response.json())
+        response_500 = UpdateProjectResponse500.from_dict(json.loads(response.text))
 
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: {}, response: httpx.Response, content: Optional[bytes] = None
+    *, client: {}, response: None, content: Optional[bytes] = None
 ) -> Response[
     Union[UpdateProjectResponse200, UpdateProjectResponse401, UpdateProjectResponse404, UpdateProjectResponse500]
 ]:
     parse = _parse_response(client=client, response=response)
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content if content is None else content,
@@ -99,16 +100,15 @@
 
     kwargs = _get_kwargs(
         project_id=project_id,
         client=client,
         multipart_data=multipart_data,
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = requests.request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
@@ -144,36 +144,23 @@
     project_id: int,
     *,
     client: {},
     multipart_data: UpdateProjectMultipartData,
 ) -> Response[
     Union[UpdateProjectResponse200, UpdateProjectResponse401, UpdateProjectResponse404, UpdateProjectResponse500]
 ]:
-    """Update a certain project
-
-    Args:
-        project_id (int):
-        multipart_data (UpdateProjectMultipartData):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[UpdateProjectResponse200, UpdateProjectResponse401, UpdateProjectResponse404, UpdateProjectResponse500]]
-    """
-
     kwargs = _get_kwargs(
         project_id=project_id,
         client=client,
         multipart_data=multipart_data,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    response = requests.request(
+        **kwargs,
+    )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_id: int,
     *,
```

## customgpt_client/api/users/get_user_profile.py

```diff
@@ -1,11 +1,12 @@
+import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
-import httpx
+import requests
 
 from ... import errors
 from ...models.get_user_profile_response_200 import GetUserProfileResponse200
 from ...models.get_user_profile_response_401 import GetUserProfileResponse401
 from ...models.get_user_profile_response_500 import GetUserProfileResponse500
 from ...types import Response
 
@@ -21,41 +22,41 @@
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "allow_redirects": client.follow_redirects,
     }
 
 
 def _parse_response(
-    *, client: {}, response: httpx.Response
+    *, client: {}, response: None
 ) -> Optional[Union[GetUserProfileResponse200, GetUserProfileResponse401, GetUserProfileResponse500]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetUserProfileResponse200.from_dict(response.json())
+        response_200 = GetUserProfileResponse200.from_dict(json.loads(response.text))
 
         return response_200
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = GetUserProfileResponse401.from_dict(response.json())
+        response_401 = GetUserProfileResponse401.from_dict(json.loads(response.text))
 
         return response_401
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        response_500 = GetUserProfileResponse500.from_dict(response.json())
+        response_500 = GetUserProfileResponse500.from_dict(json.loads(response.text))
 
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: {}, response: httpx.Response, content: Optional[bytes] = None
+    *, client: {}, response: None, content: Optional[bytes] = None
 ) -> Response[Union[GetUserProfileResponse200, GetUserProfileResponse401, GetUserProfileResponse500]]:
     parse = _parse_response(client=client, response=response)
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content if content is None else content,
         headers=response.headers,
         parsed=parse,
@@ -78,16 +79,15 @@
         Response[Union[GetUserProfileResponse200, GetUserProfileResponse401, GetUserProfileResponse500]]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = requests.request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
@@ -111,32 +111,21 @@
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: {},
 ) -> Response[Union[GetUserProfileResponse200, GetUserProfileResponse401, GetUserProfileResponse500]]:
-    """Show the user's profile.
-
-     Retrieve the current user's profile.
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[GetUserProfileResponse200, GetUserProfileResponse401, GetUserProfileResponse500]]
-    """
-
     kwargs = _get_kwargs(
         client=client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    response = requests.request(
+        **kwargs,
+    )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: {},
```

## customgpt_client/api/users/update_user_profile.py

```diff
@@ -1,11 +1,12 @@
+import json
 from http import HTTPStatus
 from typing import Any, Dict, Optional, Union
 
-import httpx
+import requests
 
 from ... import errors
 from ...models.update_user_profile_multipart_data import UpdateUserProfileMultipartData
 from ...models.update_user_profile_response_200 import UpdateUserProfileResponse200
 from ...models.update_user_profile_response_401 import UpdateUserProfileResponse401
 from ...models.update_user_profile_response_500 import UpdateUserProfileResponse500
 from ...types import Response
@@ -25,42 +26,42 @@
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "allow_redirects": client.follow_redirects,
         "files": multipart_multipart_data,
     }
 
 
 def _parse_response(
-    *, client: {}, response: httpx.Response
+    *, client: {}, response: None
 ) -> Optional[Union[UpdateUserProfileResponse200, UpdateUserProfileResponse401, UpdateUserProfileResponse500]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = UpdateUserProfileResponse200.from_dict(response.json())
+        response_200 = UpdateUserProfileResponse200.from_dict(json.loads(response.text))
 
         return response_200
     if response.status_code == HTTPStatus.UNAUTHORIZED:
-        response_401 = UpdateUserProfileResponse401.from_dict(response.json())
+        response_401 = UpdateUserProfileResponse401.from_dict(json.loads(response.text))
 
         return response_401
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
-        response_500 = UpdateUserProfileResponse500.from_dict(response.json())
+        response_500 = UpdateUserProfileResponse500.from_dict(json.loads(response.text))
 
         return response_500
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
-    *, client: {}, response: httpx.Response, content: Optional[bytes] = None
+    *, client: {}, response: None, content: Optional[bytes] = None
 ) -> Response[Union[UpdateUserProfileResponse200, UpdateUserProfileResponse401, UpdateUserProfileResponse500]]:
     parse = _parse_response(client=client, response=response)
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content if content is None else content,
         headers=response.headers,
         parsed=parse,
@@ -88,16 +89,15 @@
     """
 
     kwargs = _get_kwargs(
         client=client,
         multipart_data=multipart_data,
     )
 
-    response = httpx.request(
-        verify=client.verify_ssl,
+    response = requests.request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
@@ -127,36 +127,22 @@
 
 
 async def asyncio_detailed(
     *,
     client: {},
     multipart_data: UpdateUserProfileMultipartData,
 ) -> Response[Union[UpdateUserProfileResponse200, UpdateUserProfileResponse401, UpdateUserProfileResponse500]]:
-    """Update the user's profile.
-
-     Update the current user's profile.
-
-    Args:
-        multipart_data (UpdateUserProfileMultipartData):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Union[UpdateUserProfileResponse200, UpdateUserProfileResponse401, UpdateUserProfileResponse500]]
-    """
-
     kwargs = _get_kwargs(
         client=client,
         multipart_data=multipart_data,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    response = requests.request(
+        **kwargs,
+    )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: {},
```

## customgpt_client/client.py

```diff
@@ -9,35 +9,55 @@
     delete_project_conversation,
     get_project_conversations,
     messages,
     send_message_to_conversation,
     update_project_conversation,
 )
 from customgpt_client.api.pages import delete_project_page, get_project_pages, preview
+from customgpt_client.api.project_plugins import create_project_plugin, get_project_plugins, update_project_plugin
 from customgpt_client.api.project_settings import get_project_settings, update_project_settings
 from customgpt_client.api.projects import (
     create_project,
     delete_project,
     get_project,
     list_projects,
     stats_project,
     update_project,
 )
+from customgpt_client.api.sources import create_project_source, delete_project_source, list_project_sources
 from customgpt_client.api.users import get_user_profile, update_user_profile
 from customgpt_client.models import (
     CreateProjectConversationJsonBody,
     CreateProjectMultipartData,
+    CreateProjectPluginJsonBody,
+    CreateProjectSourceMultipartData,
     SendMessageToConversationJsonBody,
     UpdateProjectConversationJsonBody,
     UpdateProjectMultipartData,
+    UpdateProjectPluginJsonBody,
     UpdateProjectSettingsMultipartData,
     UpdateUserProfileMultipartData,
 )
 
 
+def set_client():
+    api_key = CustomGPT.api_key
+    base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
+    timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
+    return CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+
+
+def pluck_data(fields, kwargs):
+    json = {}
+    for field in fields:
+        if field in kwargs:
+            json[field] = kwargs.pop(field)
+    return json
+
+
 @attr.s(auto_attribs=True)
 class CustomGPT:
     """A Client which has been authenticated for use on secured endpoints
     Attributes:
         base_url: The base URL for the API, all requests are made to a relative path to this URL
         cookies: A dictionary of cookies to be sent with every request
         headers: A dictionary of headers to be sent with every request
@@ -82,478 +102,346 @@
     def get_headers(self) -> Dict[str, str]:
         """Get headers to be used in authenticated endpoints"""
         auth_header_value = f"{self.prefix} {self.api_key}" if self.prefix else self.api_key
         return {self.auth_header_name: auth_header_value, **self.headers}
 
     class Project:
         def list(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+            client = set_client()
 
             return list_projects.sync_detailed(client=client, *args, **kwargs)
 
         def alist(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+            client = set_client()
 
             return list_projects.asyncio_detailed(client=client, *args, **kwargs)
 
         def create(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
-            json = {}
-            if "project_name" in kwargs:
-                field = kwargs.pop("project_name")
-                json["project_name"] = field
-            if "sitemap_path" in kwargs:
-                field = kwargs.pop("sitemap_path")
-                json["sitemap_path"] = field
-            if "file_data_retension" in kwargs:
-                field = kwargs.pop("file_data_retension")
-                json["file_data_retension"] = field
-            if "file" in kwargs:
-                field = kwargs.pop("file")
-                json["file"] = field
+            client = set_client()
+            fields = ["project_name", "sitemap_path", "file_data_retension", "file"]
+            json = pluck_data(fields, kwargs)
             kwargs["multipart_data"] = CreateProjectMultipartData(**json)
 
             return create_project.sync_detailed(client=client, *args, **kwargs)
 
         def acreate(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
-            json = {}
-            if "project_name" in kwargs:
-                field = kwargs.pop("project_name")
-                json["project_name"] = field
-            if "sitemap_path" in kwargs:
-                field = kwargs.pop("sitemap_path")
-                json["sitemap_path"] = field
-            if "file_data_retension" in kwargs:
-                field = kwargs.pop("file_data_retension")
-                json["file_data_retension"] = field
-            if "file" in kwargs:
-                field = kwargs.pop("file")
-                json["file"] = field
+            client = set_client()
+            fields = ["project_name", "sitemap_path", "file_data_retension", "file"]
+            json = pluck_data(fields, kwargs)
             kwargs["multipart_data"] = CreateProjectMultipartData(**json)
 
             return create_project.asyncio_detailed(client=client, *args, **kwargs)
 
         def get(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+            client = set_client()
 
             return get_project.sync_detailed(client=client, *args, **kwargs)
 
         def aget(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+            client = set_client()
 
             return get_project.asyncio_detailed(client=client, *args, **kwargs)
 
         def update(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
-            json = {}
-            if "project_name" in kwargs:
-                field = kwargs.pop("project_name")
-                json["project_name"] = field
-            if "is_shared" in kwargs:
-                field = kwargs.pop("is_shared")
-                json["is_shared"] = field
-            if "sitemap_path" in kwargs:
-                field = kwargs.pop("sitemap_path")
-                json["sitemap_path"] = field
-            if "file_data_retension" in kwargs:
-                field = kwargs.pop("file_data_retension")
-                json["file_data_retension"] = field
-            if "file" in kwargs:
-                field = kwargs.pop("file")
-                json["file"] = field
+            client = set_client()
+            fields = ["project_name", "is_shared", "sitemap_path", "file_data_retension", "file"]
+            json = pluck_data(fields, kwargs)
             kwargs["multipart_data"] = UpdateProjectMultipartData(**json)
 
             return update_project.sync_detailed(client=client, *args, **kwargs)
 
         def aupdate(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
-            json = {}
-            if "project_name" in kwargs:
-                field = kwargs.pop("project_name")
-                json["project_name"] = field
-            if "is_shared" in kwargs:
-                field = kwargs.pop("is_shared")
-                json["is_shared"] = field
-            if "sitemap_path" in kwargs:
-                field = kwargs.pop("sitemap_path")
-                json["sitemap_path"] = field
-            if "file_data_retension" in kwargs:
-                field = kwargs.pop("file_data_retension")
-                json["file_data_retension"] = field
-            if "file" in kwargs:
-                field = kwargs.pop("file")
-                json["file"] = field
+            client = set_client()
+            fields = ["project_name", "is_shared", "sitemap_path", "file_data_retension", "file"]
+            json = pluck_data(fields, kwargs)
             kwargs["multipart_data"] = UpdateProjectMultipartData(**json)
 
             return update_project.asyncio_detailed(client=client, *args, **kwargs)
 
         def delete(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+            client = set_client()
 
             return delete_project.sync_detailed(client=client, *args, **kwargs)
 
         def adelete(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+            client = set_client()
 
             return delete_project.asyncio_detailed(client=client, *args, **kwargs)
 
         def stats(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+            client = set_client()
 
             return stats_project.sync_detailed(client=client, *args, **kwargs)
 
         def astats(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+            client = set_client()
 
             return stats_project.asyncio_detailed(client=client, *args, **kwargs)
 
     class Page:
         def get(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+            client = set_client()
 
             return get_project_pages.sync_detailed(client=client, *args, **kwargs)
 
         def aget(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+            client = set_client()
 
             return get_project_pages.asyncio_detailed(client=client, *args, **kwargs)
 
         def delete(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+            client = set_client()
 
             return delete_project_page.sync_detailed(client=client, *args, **kwargs)
 
         def adelete(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+            client = set_client()
 
             return delete_project_page.asyncio_detailed(client=client, *args, **kwargs)
 
         def preview(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+            client = set_client()
 
             return preview.sync_detailed(client=client, *args, **kwargs)
 
         def apreview(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+            client = set_client()
 
             return preview.asyncio_detailed(client=client, *args, **kwargs)
 
     class ProjectSettings:
         def get(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+            client = set_client()
 
             return get_project_settings.sync_detailed(client=client, *args, **kwargs)
 
         def aget(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+            client = set_client()
 
             return get_project_settings.asyncio_detailed(client=client, *args, **kwargs)
 
         def update(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
-            json = {}
-            if "chat_bot_avatar" in kwargs:
-                field = kwargs.pop("chat_bot_avatar")
-                json["chat_bot_avatar"] = field
-            if "chat_bot_bg" in kwargs:
-                field = kwargs.pop("chat_bot_bg")
-                json["chat_bot_bg"] = field
-            if "default_prompt" in kwargs:
-                field = kwargs.pop("default_prompt")
-                json["default_prompt"] = field
-            if "example_questions" in kwargs:
-                field = kwargs.pop("example_questions")
-                json["example_questions"] = field
-            if "response_source" in kwargs:
-                field = kwargs.pop("response_source")
-                json["response_source"] = field
-            if "chatbot_msg_lang" in kwargs:
-                field = kwargs.pop("chatbot_msg_lang")
-                json["chatbot_msg_lang"] = field
+            client = set_client()
+            fields = [
+                "chat_bot_avatar",
+                "chat_bot_bg",
+                "default_prompt",
+                "example_questions",
+                "response_source",
+                "chatbot_msg_lang",
+            ]
+            json = pluck_data(fields, kwargs)
             kwargs["multipart_data"] = UpdateProjectSettingsMultipartData(**json)
 
             return update_project_settings.sync_detailed(client=client, *args, **kwargs)
 
         def aupdate(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
-            json = {}
-            if "chat_bot_avatar" in kwargs:
-                field = kwargs.pop("chat_bot_avatar")
-                json["chat_bot_avatar"] = field
-            if "chat_bot_bg" in kwargs:
-                field = kwargs.pop("chat_bot_bg")
-                json["chat_bot_bg"] = field
-            if "default_prompt" in kwargs:
-                field = kwargs.pop("default_prompt")
-                json["default_prompt"] = field
-            if "example_questions" in kwargs:
-                field = kwargs.pop("example_questions")
-                json["example_questions"] = field
-            if "response_source" in kwargs:
-                field = kwargs.pop("response_source")
-                json["response_source"] = field
-            if "chatbot_msg_lang" in kwargs:
-                field = kwargs.pop("chatbot_msg_lang")
-                json["chatbot_msg_lang"] = field
+            client = set_client()
+            fields = [
+                "chat_bot_avatar",
+                "chat_bot_bg",
+                "default_prompt",
+                "example_questions",
+                "response_source",
+                "chatbot_msg_lang",
+            ]
+            json = pluck_data(fields, kwargs)
             kwargs["multipart_data"] = UpdateProjectSettingsMultipartData(**json)
 
             return update_project_settings.asyncio_detailed(client=client, *args, **kwargs)
 
+    class ProjectPlugins:
+        def get(*args: Any, **kwargs: Any):
+            client = set_client()
+
+            return get_project_plugins.sync_detailed(client=client, *args, **kwargs)
+
+        def aget(*args: Any, **kwargs: Any):
+            client = set_client()
+
+            return get_project_plugins.asyncio_detailed(client=client, *args, **kwargs)
+
+        def update(*args: Any, **kwargs: Any):
+            client = set_client()
+            fields = ["model_name", "human_name", "keywords", "description", "is_active"]
+            json = pluck_data(fields, kwargs)
+            kwargs["json_body"] = UpdateProjectPluginJsonBody(**json)
+
+            return update_project_plugin.sync_detailed(client=client, *args, **kwargs)
+
+        def aupdate(*args: Any, **kwargs: Any):
+            client = set_client()
+            fields = ["model_name", "human_name", "keywords", "description", "is_active"]
+            json = pluck_data(fields, kwargs)
+            kwargs["json_body"] = UpdateProjectPluginJsonBody(**json)
+
+            return update_project_plugin.asyncio_detailed(client=client, *args, **kwargs)
+
+        def create(*args: Any, **kwargs: Any):
+            client = set_client()
+            fields = ["model_name", "human_name", "keywords", "description", "is_active"]
+            json = pluck_data(fields, kwargs)
+            kwargs["json_body"] = CreateProjectPluginJsonBody(**json)
+
+            return create_project_plugin.sync_detailed(client=client, *args, **kwargs)
+
+        def acreate(*args: Any, **kwargs: Any):
+            client = set_client()
+            fields = ["model_name", "human_name", "keywords", "description", "is_active"]
+            json = pluck_data(fields, kwargs)
+            kwargs["json_body"] = CreateProjectPluginJsonBody(**json)
+
+            return create_project_plugin.asyncio_detailed(client=client, *args, **kwargs)
+
     class Conversation:
         def get(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+            client = set_client()
 
             return get_project_conversations.sync_detailed(client=client, *args, **kwargs)
 
         def aget(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+            client = set_client()
 
             return get_project_conversations.asyncio_detailed(client=client, *args, **kwargs)
 
         def create(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
-            json = {}
-            if "name" in kwargs:
-                field = kwargs.pop("name")
-                json["name"] = field
+            client = set_client()
+            fields = ["name"]
+            json = pluck_data(fields, kwargs)
             kwargs["json_body"] = CreateProjectConversationJsonBody(**json)
 
             return create_project_conversation.sync_detailed(client=client, *args, **kwargs)
 
         def acreate(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
-            json = {}
-            if "name" in kwargs:
-                field = kwargs.pop("name")
-                json["name"] = field
+            client = set_client()
+            fields = ["name"]
+            json = pluck_data(fields, kwargs)
             kwargs["json_body"] = CreateProjectConversationJsonBody(**json)
 
             return create_project_conversation.asyncio_detailed(client=client, *args, **kwargs)
 
         def update(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
-            json = {}
-            if "name" in kwargs:
-                field = kwargs.pop("name")
-                json["name"] = field
+            client = set_client()
+            fields = ["name"]
+            json = pluck_data(fields, kwargs)
             kwargs["json_body"] = UpdateProjectConversationJsonBody(**json)
 
             return update_project_conversation.sync_detailed(client=client, *args, **kwargs)
 
         def aupdate(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
-            json = {}
-            if "name" in kwargs:
-                field = kwargs.pop("name")
-                json["name"] = field
+            client = set_client()
+            fields = ["name"]
+            json = pluck_data(fields, kwargs)
             kwargs["json_body"] = UpdateProjectConversationJsonBody(**json)
 
             return update_project_conversation.asyncio_detailed(client=client, *args, **kwargs)
 
         def delete(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+            client = set_client()
 
             return delete_project_conversation.sync_detailed(client=client, *args, **kwargs)
 
         def adelete(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+            client = set_client()
 
             return delete_project_conversation.asyncio_detailed(client=client, *args, **kwargs)
 
         def messages(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+            client = set_client()
 
             return messages.sync_detailed(client=client, *args, **kwargs)
 
         def amessages(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+            client = set_client()
 
             return messages.asyncio_detailed(client=client, *args, **kwargs)
 
         def send(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
-            json = {}
-            if "prompt" in kwargs:
-                field = kwargs.pop("prompt")
-                json["prompt"] = field
+            client = set_client()
+            fields = ["prompt"]
+            json = pluck_data(fields, kwargs)
             kwargs["json_body"] = SendMessageToConversationJsonBody(**json)
 
             return send_message_to_conversation.sync_detailed(client=client, *args, **kwargs)
 
         def asend(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
-            json = {}
-            if "prompt" in kwargs:
-                field = kwargs.pop("prompt")
-                json["prompt"] = field
+            client = set_client()
+            fields = ["prompt"]
+            json = pluck_data(fields, kwargs)
             kwargs["json_body"] = SendMessageToConversationJsonBody(**json)
 
             return send_message_to_conversation.asyncio_detailed(client=client, *args, **kwargs)
 
     class Citation:
         def get(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+            client = set_client()
 
             return get_open_graph_data_for_citation.sync_detailed(client=client, *args, **kwargs)
 
         def aget(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+            client = set_client()
 
             return get_open_graph_data_for_citation.asyncio_detailed(client=client, *args, **kwargs)
 
+    class Source:
+        def list(*args: Any, **kwargs: Any):
+            client = set_client()
+
+            return list_project_sources.sync_detailed(client=client, *args, **kwargs)
+
+        def alist(*args: Any, **kwargs: Any):
+            client = set_client()
+
+            return list_project_sources.asyncio_detailed(client=client, *args, **kwargs)
+
+        def create(*args: Any, **kwargs: Any):
+            client = set_client()
+            fields = ["sitemap_path", "file_data_retension", "file"]
+            json = pluck_data(fields, kwargs)
+            kwargs["multipart_data"] = CreateProjectSourceMultipartData(**json)
+
+            return create_project_source.sync_detailed(client=client, *args, **kwargs)
+
+        def acreate(*args: Any, **kwargs: Any):
+            client = set_client()
+            fields = ["sitemap_path", "file_data_retension", "file"]
+            json = pluck_data(fields, kwargs)
+            kwargs["multipart_data"] = CreateProjectSourceMultipartData(**json)
+
+            return create_project_source.asyncio_detailed(client=client, *args, **kwargs)
+
+        def delete(*args: Any, **kwargs: Any):
+            client = set_client()
+
+            return delete_project_source.sync_detailed(client=client, *args, **kwargs)
+
+        def adelete(*args: Any, **kwargs: Any):
+            client = set_client()
+
+            return delete_project_source.asyncio_detailed(client=client, *args, **kwargs)
+
     class User:
         def get(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+            client = set_client()
 
             return get_user_profile.sync_detailed(client=client, *args, **kwargs)
 
         def aget(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
+            client = set_client()
 
             return get_user_profile.asyncio_detailed(client=client, *args, **kwargs)
 
         def update(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
-            json = {}
-            if "profile_photo" in kwargs:
-                field = kwargs.pop("profile_photo")
-                json["profile_photo"] = field
-            if "name" in kwargs:
-                field = kwargs.pop("name")
-                json["name"] = field
+            client = set_client()
+            fields = ["profile_photo", "name"]
+            json = pluck_data(fields, kwargs)
             kwargs["multipart_data"] = UpdateUserProfileMultipartData(**json)
 
             return update_user_profile.sync_detailed(client=client, *args, **kwargs)
 
         def aupdate(*args: Any, **kwargs: Any):
-            api_key = CustomGPT.api_key
-            base_url = CustomGPT.base_url if hasattr(CustomGPT, "base_url") else "https://app.customgpt.ai"
-            timeout = CustomGPT.timeout if hasattr(CustomGPT, "timeout") else 100.0
-            client = CustomGPT(api_key=api_key, base_url=base_url, timeout=timeout)
-            json = {}
-            if "profile_photo" in kwargs:
-                field = kwargs.pop("profile_photo")
-                json["profile_photo"] = field
-            if "name" in kwargs:
-                field = kwargs.pop("name")
-                json["name"] = field
+            client = set_client()
+            fields = ["profile_photo", "name"]
+            json = pluck_data(fields, kwargs)
             kwargs["multipart_data"] = UpdateUserProfileMultipartData(**json)
 
             return update_user_profile.asyncio_detailed(client=client, *args, **kwargs)
```

## customgpt_client/models/__init__.py

```diff
@@ -15,14 +15,31 @@
 from .create_project_conversation_response_404_data_message import CreateProjectConversationResponse404DataMessage
 from .create_project_conversation_response_404_status import CreateProjectConversationResponse404Status
 from .create_project_conversation_response_500 import CreateProjectConversationResponse500
 from .create_project_conversation_response_500_data import CreateProjectConversationResponse500Data
 from .create_project_conversation_response_500_data_code import CreateProjectConversationResponse500DataCode
 from .create_project_conversation_response_500_status import CreateProjectConversationResponse500Status
 from .create_project_multipart_data import CreateProjectMultipartData
+from .create_project_plugin_json_body import CreateProjectPluginJsonBody
+from .create_project_plugin_response_201 import CreateProjectPluginResponse201
+from .create_project_plugin_response_201_data import CreateProjectPluginResponse201Data
+from .create_project_plugin_response_201_status import CreateProjectPluginResponse201Status
+from .create_project_plugin_response_401 import CreateProjectPluginResponse401
+from .create_project_plugin_response_401_data import CreateProjectPluginResponse401Data
+from .create_project_plugin_response_401_data_code import CreateProjectPluginResponse401DataCode
+from .create_project_plugin_response_401_status import CreateProjectPluginResponse401Status
+from .create_project_plugin_response_404 import CreateProjectPluginResponse404
+from .create_project_plugin_response_404_data import CreateProjectPluginResponse404Data
+from .create_project_plugin_response_404_data_code import CreateProjectPluginResponse404DataCode
+from .create_project_plugin_response_404_data_message import CreateProjectPluginResponse404DataMessage
+from .create_project_plugin_response_404_status import CreateProjectPluginResponse404Status
+from .create_project_plugin_response_500 import CreateProjectPluginResponse500
+from .create_project_plugin_response_500_data import CreateProjectPluginResponse500Data
+from .create_project_plugin_response_500_data_code import CreateProjectPluginResponse500DataCode
+from .create_project_plugin_response_500_status import CreateProjectPluginResponse500Status
 from .create_project_response_201 import CreateProjectResponse201
 from .create_project_response_201_data import CreateProjectResponse201Data
 from .create_project_response_201_data_type import CreateProjectResponse201DataType
 from .create_project_response_201_status import CreateProjectResponse201Status
 from .create_project_response_400 import CreateProjectResponse400
 from .create_project_response_400_data import CreateProjectResponse400Data
 from .create_project_response_400_data_code import CreateProjectResponse400DataCode
@@ -32,14 +49,45 @@
 from .create_project_response_401_data import CreateProjectResponse401Data
 from .create_project_response_401_data_code import CreateProjectResponse401DataCode
 from .create_project_response_401_status import CreateProjectResponse401Status
 from .create_project_response_500 import CreateProjectResponse500
 from .create_project_response_500_data import CreateProjectResponse500Data
 from .create_project_response_500_data_code import CreateProjectResponse500DataCode
 from .create_project_response_500_status import CreateProjectResponse500Status
+from .create_project_source_multipart_data import CreateProjectSourceMultipartData
+from .create_project_source_response_201 import CreateProjectSourceResponse201
+from .create_project_source_response_201_data import CreateProjectSourceResponse201Data
+from .create_project_source_response_201_data_pages_item import CreateProjectSourceResponse201DataPagesItem
+from .create_project_source_response_201_data_pages_item_crawl_status import (
+    CreateProjectSourceResponse201DataPagesItemCrawlStatus,
+)
+from .create_project_source_response_201_data_pages_item_index_status import (
+    CreateProjectSourceResponse201DataPagesItemIndexStatus,
+)
+from .create_project_source_response_201_data_settings import CreateProjectSourceResponse201DataSettings
+from .create_project_source_response_201_data_type import CreateProjectSourceResponse201DataType
+from .create_project_source_response_201_status import CreateProjectSourceResponse201Status
+from .create_project_source_response_400 import CreateProjectSourceResponse400
+from .create_project_source_response_400_data import CreateProjectSourceResponse400Data
+from .create_project_source_response_400_data_code import CreateProjectSourceResponse400DataCode
+from .create_project_source_response_400_data_message import CreateProjectSourceResponse400DataMessage
+from .create_project_source_response_400_status import CreateProjectSourceResponse400Status
+from .create_project_source_response_401 import CreateProjectSourceResponse401
+from .create_project_source_response_401_data import CreateProjectSourceResponse401Data
+from .create_project_source_response_401_data_code import CreateProjectSourceResponse401DataCode
+from .create_project_source_response_401_status import CreateProjectSourceResponse401Status
+from .create_project_source_response_404 import CreateProjectSourceResponse404
+from .create_project_source_response_404_data import CreateProjectSourceResponse404Data
+from .create_project_source_response_404_data_code import CreateProjectSourceResponse404DataCode
+from .create_project_source_response_404_data_message import CreateProjectSourceResponse404DataMessage
+from .create_project_source_response_404_status import CreateProjectSourceResponse404Status
+from .create_project_source_response_500 import CreateProjectSourceResponse500
+from .create_project_source_response_500_data import CreateProjectSourceResponse500Data
+from .create_project_source_response_500_data_code import CreateProjectSourceResponse500DataCode
+from .create_project_source_response_500_status import CreateProjectSourceResponse500Status
 from .delete_project_conversation_response_200 import DeleteProjectConversationResponse200
 from .delete_project_conversation_response_200_data import DeleteProjectConversationResponse200Data
 from .delete_project_conversation_response_200_status import DeleteProjectConversationResponse200Status
 from .delete_project_conversation_response_401 import DeleteProjectConversationResponse401
 from .delete_project_conversation_response_401_data import DeleteProjectConversationResponse401Data
 from .delete_project_conversation_response_401_data_code import DeleteProjectConversationResponse401DataCode
 from .delete_project_conversation_response_401_status import DeleteProjectConversationResponse401Status
@@ -80,14 +128,30 @@
 from .delete_project_response_404_data_code import DeleteProjectResponse404DataCode
 from .delete_project_response_404_data_message import DeleteProjectResponse404DataMessage
 from .delete_project_response_404_status import DeleteProjectResponse404Status
 from .delete_project_response_500 import DeleteProjectResponse500
 from .delete_project_response_500_data import DeleteProjectResponse500Data
 from .delete_project_response_500_data_code import DeleteProjectResponse500DataCode
 from .delete_project_response_500_status import DeleteProjectResponse500Status
+from .delete_project_source_response_200 import DeleteProjectSourceResponse200
+from .delete_project_source_response_200_data import DeleteProjectSourceResponse200Data
+from .delete_project_source_response_200_status import DeleteProjectSourceResponse200Status
+from .delete_project_source_response_401 import DeleteProjectSourceResponse401
+from .delete_project_source_response_401_data import DeleteProjectSourceResponse401Data
+from .delete_project_source_response_401_data_code import DeleteProjectSourceResponse401DataCode
+from .delete_project_source_response_401_status import DeleteProjectSourceResponse401Status
+from .delete_project_source_response_404 import DeleteProjectSourceResponse404
+from .delete_project_source_response_404_data import DeleteProjectSourceResponse404Data
+from .delete_project_source_response_404_data_code import DeleteProjectSourceResponse404DataCode
+from .delete_project_source_response_404_data_message import DeleteProjectSourceResponse404DataMessage
+from .delete_project_source_response_404_status import DeleteProjectSourceResponse404Status
+from .delete_project_source_response_500 import DeleteProjectSourceResponse500
+from .delete_project_source_response_500_data import DeleteProjectSourceResponse500Data
+from .delete_project_source_response_500_data_code import DeleteProjectSourceResponse500DataCode
+from .delete_project_source_response_500_status import DeleteProjectSourceResponse500Status
 from .get_open_graph_data_for_citation_response_200 import GetOpenGraphDataForCitationResponse200
 from .get_open_graph_data_for_citation_response_200_data import GetOpenGraphDataForCitationResponse200Data
 from .get_open_graph_data_for_citation_response_200_status import GetOpenGraphDataForCitationResponse200Status
 from .get_open_graph_data_for_citation_response_401 import GetOpenGraphDataForCitationResponse401
 from .get_open_graph_data_for_citation_response_401_data import GetOpenGraphDataForCitationResponse401Data
 from .get_open_graph_data_for_citation_response_401_data_code import GetOpenGraphDataForCitationResponse401DataCode
 from .get_open_graph_data_for_citation_response_401_status import GetOpenGraphDataForCitationResponse401Status
@@ -98,15 +162,14 @@
     GetOpenGraphDataForCitationResponse404DataMessage,
 )
 from .get_open_graph_data_for_citation_response_404_status import GetOpenGraphDataForCitationResponse404Status
 from .get_project_conversations_order import GetProjectConversationsOrder
 from .get_project_conversations_response_200 import GetProjectConversationsResponse200
 from .get_project_conversations_response_200_data import GetProjectConversationsResponse200Data
 from .get_project_conversations_response_200_data_data_item import GetProjectConversationsResponse200DataDataItem
-from .get_project_conversations_response_200_data_links import GetProjectConversationsResponse200DataLinks
 from .get_project_conversations_response_200_status import GetProjectConversationsResponse200Status
 from .get_project_conversations_response_401 import GetProjectConversationsResponse401
 from .get_project_conversations_response_401_data import GetProjectConversationsResponse401Data
 from .get_project_conversations_response_401_data_code import GetProjectConversationsResponse401DataCode
 from .get_project_conversations_response_401_status import GetProjectConversationsResponse401Status
 from .get_project_conversations_response_404 import GetProjectConversationsResponse404
 from .get_project_conversations_response_404_data import GetProjectConversationsResponse404Data
@@ -124,15 +187,14 @@
 from .get_project_pages_response_200_data_pages_data_item import GetProjectPagesResponse200DataPagesDataItem
 from .get_project_pages_response_200_data_pages_data_item_crawl_status import (
     GetProjectPagesResponse200DataPagesDataItemCrawlStatus,
 )
 from .get_project_pages_response_200_data_pages_data_item_index_status import (
     GetProjectPagesResponse200DataPagesDataItemIndexStatus,
 )
-from .get_project_pages_response_200_data_pages_links import GetProjectPagesResponse200DataPagesLinks
 from .get_project_pages_response_200_data_project import GetProjectPagesResponse200DataProject
 from .get_project_pages_response_200_data_project_type import GetProjectPagesResponse200DataProjectType
 from .get_project_pages_response_200_status import GetProjectPagesResponse200Status
 from .get_project_pages_response_401 import GetProjectPagesResponse401
 from .get_project_pages_response_401_data import GetProjectPagesResponse401Data
 from .get_project_pages_response_401_data_code import GetProjectPagesResponse401DataCode
 from .get_project_pages_response_401_status import GetProjectPagesResponse401Status
@@ -141,14 +203,30 @@
 from .get_project_pages_response_404_data_code import GetProjectPagesResponse404DataCode
 from .get_project_pages_response_404_data_message import GetProjectPagesResponse404DataMessage
 from .get_project_pages_response_404_status import GetProjectPagesResponse404Status
 from .get_project_pages_response_500 import GetProjectPagesResponse500
 from .get_project_pages_response_500_data import GetProjectPagesResponse500Data
 from .get_project_pages_response_500_data_code import GetProjectPagesResponse500DataCode
 from .get_project_pages_response_500_status import GetProjectPagesResponse500Status
+from .get_project_plugins_response_200 import GetProjectPluginsResponse200
+from .get_project_plugins_response_200_data import GetProjectPluginsResponse200Data
+from .get_project_plugins_response_200_status import GetProjectPluginsResponse200Status
+from .get_project_plugins_response_401 import GetProjectPluginsResponse401
+from .get_project_plugins_response_401_data import GetProjectPluginsResponse401Data
+from .get_project_plugins_response_401_data_code import GetProjectPluginsResponse401DataCode
+from .get_project_plugins_response_401_status import GetProjectPluginsResponse401Status
+from .get_project_plugins_response_404 import GetProjectPluginsResponse404
+from .get_project_plugins_response_404_data import GetProjectPluginsResponse404Data
+from .get_project_plugins_response_404_data_code import GetProjectPluginsResponse404DataCode
+from .get_project_plugins_response_404_data_message import GetProjectPluginsResponse404DataMessage
+from .get_project_plugins_response_404_status import GetProjectPluginsResponse404Status
+from .get_project_plugins_response_500 import GetProjectPluginsResponse500
+from .get_project_plugins_response_500_data import GetProjectPluginsResponse500Data
+from .get_project_plugins_response_500_data_code import GetProjectPluginsResponse500DataCode
+from .get_project_plugins_response_500_status import GetProjectPluginsResponse500Status
 from .get_project_response_200 import GetProjectResponse200
 from .get_project_response_200_data import GetProjectResponse200Data
 from .get_project_response_200_data_type import GetProjectResponse200DataType
 from .get_project_response_200_status import GetProjectResponse200Status
 from .get_project_response_401 import GetProjectResponse401
 from .get_project_response_401_data import GetProjectResponse401Data
 from .get_project_response_401_data_code import GetProjectResponse401DataCode
@@ -186,35 +264,74 @@
 from .get_user_profile_response_401_data import GetUserProfileResponse401Data
 from .get_user_profile_response_401_data_code import GetUserProfileResponse401DataCode
 from .get_user_profile_response_401_status import GetUserProfileResponse401Status
 from .get_user_profile_response_500 import GetUserProfileResponse500
 from .get_user_profile_response_500_data import GetUserProfileResponse500Data
 from .get_user_profile_response_500_data_code import GetUserProfileResponse500DataCode
 from .get_user_profile_response_500_status import GetUserProfileResponse500Status
+from .list_project_sources_response_200 import ListProjectSourcesResponse200
+from .list_project_sources_response_200_data import ListProjectSourcesResponse200Data
+from .list_project_sources_response_200_data_sitemaps_item import ListProjectSourcesResponse200DataSitemapsItem
+from .list_project_sources_response_200_data_sitemaps_item_pages_item import (
+    ListProjectSourcesResponse200DataSitemapsItemPagesItem,
+)
+from .list_project_sources_response_200_data_sitemaps_item_pages_item_crawl_status import (
+    ListProjectSourcesResponse200DataSitemapsItemPagesItemCrawlStatus,
+)
+from .list_project_sources_response_200_data_sitemaps_item_pages_item_index_status import (
+    ListProjectSourcesResponse200DataSitemapsItemPagesItemIndexStatus,
+)
+from .list_project_sources_response_200_data_sitemaps_item_settings import (
+    ListProjectSourcesResponse200DataSitemapsItemSettings,
+)
+from .list_project_sources_response_200_data_sitemaps_item_type import ListProjectSourcesResponse200DataSitemapsItemType
+from .list_project_sources_response_200_data_uploads import ListProjectSourcesResponse200DataUploads
+from .list_project_sources_response_200_data_uploads_pages_item import ListProjectSourcesResponse200DataUploadsPagesItem
+from .list_project_sources_response_200_data_uploads_pages_item_crawl_status import (
+    ListProjectSourcesResponse200DataUploadsPagesItemCrawlStatus,
+)
+from .list_project_sources_response_200_data_uploads_pages_item_index_status import (
+    ListProjectSourcesResponse200DataUploadsPagesItemIndexStatus,
+)
+from .list_project_sources_response_200_data_uploads_settings import ListProjectSourcesResponse200DataUploadsSettings
+from .list_project_sources_response_200_data_uploads_type import ListProjectSourcesResponse200DataUploadsType
+from .list_project_sources_response_200_status import ListProjectSourcesResponse200Status
+from .list_project_sources_response_401 import ListProjectSourcesResponse401
+from .list_project_sources_response_401_data import ListProjectSourcesResponse401Data
+from .list_project_sources_response_401_data_code import ListProjectSourcesResponse401DataCode
+from .list_project_sources_response_401_status import ListProjectSourcesResponse401Status
+from .list_project_sources_response_404 import ListProjectSourcesResponse404
+from .list_project_sources_response_404_data import ListProjectSourcesResponse404Data
+from .list_project_sources_response_404_data_code import ListProjectSourcesResponse404DataCode
+from .list_project_sources_response_404_data_message import ListProjectSourcesResponse404DataMessage
+from .list_project_sources_response_404_status import ListProjectSourcesResponse404Status
+from .list_project_sources_response_500 import ListProjectSourcesResponse500
+from .list_project_sources_response_500_data import ListProjectSourcesResponse500Data
+from .list_project_sources_response_500_data_code import ListProjectSourcesResponse500DataCode
+from .list_project_sources_response_500_status import ListProjectSourcesResponse500Status
 from .list_projects_order import ListProjectsOrder
 from .list_projects_response_200 import ListProjectsResponse200
 from .list_projects_response_200_data import ListProjectsResponse200Data
 from .list_projects_response_200_data_data_item import ListProjectsResponse200DataDataItem
 from .list_projects_response_200_data_data_item_type import ListProjectsResponse200DataDataItemType
-from .list_projects_response_200_data_links import ListProjectsResponse200DataLinks
 from .list_projects_response_200_status import ListProjectsResponse200Status
 from .list_projects_response_401 import ListProjectsResponse401
 from .list_projects_response_401_data import ListProjectsResponse401Data
 from .list_projects_response_401_data_code import ListProjectsResponse401DataCode
 from .list_projects_response_401_status import ListProjectsResponse401Status
 from .list_projects_response_500 import ListProjectsResponse500
 from .list_projects_response_500_data import ListProjectsResponse500Data
 from .list_projects_response_500_data_code import ListProjectsResponse500DataCode
 from .list_projects_response_500_status import ListProjectsResponse500Status
 from .messages_order import MessagesOrder
 from .messages_response_200 import MessagesResponse200
-from .messages_response_200_conversation import MessagesResponse200Conversation
-from .messages_response_200_messages import MessagesResponse200Messages
-from .messages_response_200_messages_data_item import MessagesResponse200MessagesDataItem
-from .messages_response_200_messages_links import MessagesResponse200MessagesLinks
+from .messages_response_200_data import MessagesResponse200Data
+from .messages_response_200_data_conversation import MessagesResponse200DataConversation
+from .messages_response_200_data_messages import MessagesResponse200DataMessages
+from .messages_response_200_data_messages_data_item import MessagesResponse200DataMessagesDataItem
 from .messages_response_200_status import MessagesResponse200Status
 from .messages_response_401 import MessagesResponse401
 from .messages_response_401_data import MessagesResponse401Data
 from .messages_response_401_data_code import MessagesResponse401DataCode
 from .messages_response_401_status import MessagesResponse401Status
 from .messages_response_404 import MessagesResponse404
 from .messages_response_404_data import MessagesResponse404Data
@@ -242,14 +359,17 @@
 from .preview_response_500_data import PreviewResponse500Data
 from .preview_response_500_data_code import PreviewResponse500DataCode
 from .preview_response_500_status import PreviewResponse500Status
 from .project import Project
 from .project_plugin import ProjectPlugin
 from .project_settings import ProjectSettings
 from .project_settings_response_source import ProjectSettingsResponseSource
+from .project_source import ProjectSource
+from .project_source_settings import ProjectSourceSettings
+from .project_source_type import ProjectSourceType
 from .project_type import ProjectType
 from .prompt_history import PromptHistory
 from .send_message_to_conversation_json_body import SendMessageToConversationJsonBody
 from .send_message_to_conversation_response_200 import SendMessageToConversationResponse200
 from .send_message_to_conversation_response_200_data import SendMessageToConversationResponse200Data
 from .send_message_to_conversation_response_200_status import SendMessageToConversationResponse200Status
 from .send_message_to_conversation_response_401 import SendMessageToConversationResponse401
@@ -295,14 +415,31 @@
 from .update_project_conversation_response_404_data_message import UpdateProjectConversationResponse404DataMessage
 from .update_project_conversation_response_404_status import UpdateProjectConversationResponse404Status
 from .update_project_conversation_response_500 import UpdateProjectConversationResponse500
 from .update_project_conversation_response_500_data import UpdateProjectConversationResponse500Data
 from .update_project_conversation_response_500_data_code import UpdateProjectConversationResponse500DataCode
 from .update_project_conversation_response_500_status import UpdateProjectConversationResponse500Status
 from .update_project_multipart_data import UpdateProjectMultipartData
+from .update_project_plugin_json_body import UpdateProjectPluginJsonBody
+from .update_project_plugin_response_200 import UpdateProjectPluginResponse200
+from .update_project_plugin_response_200_data import UpdateProjectPluginResponse200Data
+from .update_project_plugin_response_200_status import UpdateProjectPluginResponse200Status
+from .update_project_plugin_response_401 import UpdateProjectPluginResponse401
+from .update_project_plugin_response_401_data import UpdateProjectPluginResponse401Data
+from .update_project_plugin_response_401_data_code import UpdateProjectPluginResponse401DataCode
+from .update_project_plugin_response_401_status import UpdateProjectPluginResponse401Status
+from .update_project_plugin_response_404 import UpdateProjectPluginResponse404
+from .update_project_plugin_response_404_data import UpdateProjectPluginResponse404Data
+from .update_project_plugin_response_404_data_code import UpdateProjectPluginResponse404DataCode
+from .update_project_plugin_response_404_data_message import UpdateProjectPluginResponse404DataMessage
+from .update_project_plugin_response_404_status import UpdateProjectPluginResponse404Status
+from .update_project_plugin_response_500 import UpdateProjectPluginResponse500
+from .update_project_plugin_response_500_data import UpdateProjectPluginResponse500Data
+from .update_project_plugin_response_500_data_code import UpdateProjectPluginResponse500DataCode
+from .update_project_plugin_response_500_status import UpdateProjectPluginResponse500Status
 from .update_project_response_200 import UpdateProjectResponse200
 from .update_project_response_200_data import UpdateProjectResponse200Data
 from .update_project_response_200_data_type import UpdateProjectResponse200DataType
 from .update_project_response_200_status import UpdateProjectResponse200Status
 from .update_project_response_401 import UpdateProjectResponse401
 from .update_project_response_401_data import UpdateProjectResponse401Data
 from .update_project_response_401_data_code import UpdateProjectResponse401DataCode
@@ -363,14 +500,31 @@
     "CreateProjectConversationResponse404DataMessage",
     "CreateProjectConversationResponse404Status",
     "CreateProjectConversationResponse500",
     "CreateProjectConversationResponse500Data",
     "CreateProjectConversationResponse500DataCode",
     "CreateProjectConversationResponse500Status",
     "CreateProjectMultipartData",
+    "CreateProjectPluginJsonBody",
+    "CreateProjectPluginResponse201",
+    "CreateProjectPluginResponse201Data",
+    "CreateProjectPluginResponse201Status",
+    "CreateProjectPluginResponse401",
+    "CreateProjectPluginResponse401Data",
+    "CreateProjectPluginResponse401DataCode",
+    "CreateProjectPluginResponse401Status",
+    "CreateProjectPluginResponse404",
+    "CreateProjectPluginResponse404Data",
+    "CreateProjectPluginResponse404DataCode",
+    "CreateProjectPluginResponse404DataMessage",
+    "CreateProjectPluginResponse404Status",
+    "CreateProjectPluginResponse500",
+    "CreateProjectPluginResponse500Data",
+    "CreateProjectPluginResponse500DataCode",
+    "CreateProjectPluginResponse500Status",
     "CreateProjectResponse201",
     "CreateProjectResponse201Data",
     "CreateProjectResponse201DataType",
     "CreateProjectResponse201Status",
     "CreateProjectResponse400",
     "CreateProjectResponse400Data",
     "CreateProjectResponse400DataCode",
@@ -380,14 +534,41 @@
     "CreateProjectResponse401Data",
     "CreateProjectResponse401DataCode",
     "CreateProjectResponse401Status",
     "CreateProjectResponse500",
     "CreateProjectResponse500Data",
     "CreateProjectResponse500DataCode",
     "CreateProjectResponse500Status",
+    "CreateProjectSourceMultipartData",
+    "CreateProjectSourceResponse201",
+    "CreateProjectSourceResponse201Data",
+    "CreateProjectSourceResponse201DataPagesItem",
+    "CreateProjectSourceResponse201DataPagesItemCrawlStatus",
+    "CreateProjectSourceResponse201DataPagesItemIndexStatus",
+    "CreateProjectSourceResponse201DataSettings",
+    "CreateProjectSourceResponse201DataType",
+    "CreateProjectSourceResponse201Status",
+    "CreateProjectSourceResponse400",
+    "CreateProjectSourceResponse400Data",
+    "CreateProjectSourceResponse400DataCode",
+    "CreateProjectSourceResponse400DataMessage",
+    "CreateProjectSourceResponse400Status",
+    "CreateProjectSourceResponse401",
+    "CreateProjectSourceResponse401Data",
+    "CreateProjectSourceResponse401DataCode",
+    "CreateProjectSourceResponse401Status",
+    "CreateProjectSourceResponse404",
+    "CreateProjectSourceResponse404Data",
+    "CreateProjectSourceResponse404DataCode",
+    "CreateProjectSourceResponse404DataMessage",
+    "CreateProjectSourceResponse404Status",
+    "CreateProjectSourceResponse500",
+    "CreateProjectSourceResponse500Data",
+    "CreateProjectSourceResponse500DataCode",
+    "CreateProjectSourceResponse500Status",
     "DeleteProjectConversationResponse200",
     "DeleteProjectConversationResponse200Data",
     "DeleteProjectConversationResponse200Status",
     "DeleteProjectConversationResponse401",
     "DeleteProjectConversationResponse401Data",
     "DeleteProjectConversationResponse401DataCode",
     "DeleteProjectConversationResponse401Status",
@@ -428,14 +609,30 @@
     "DeleteProjectResponse404DataCode",
     "DeleteProjectResponse404DataMessage",
     "DeleteProjectResponse404Status",
     "DeleteProjectResponse500",
     "DeleteProjectResponse500Data",
     "DeleteProjectResponse500DataCode",
     "DeleteProjectResponse500Status",
+    "DeleteProjectSourceResponse200",
+    "DeleteProjectSourceResponse200Data",
+    "DeleteProjectSourceResponse200Status",
+    "DeleteProjectSourceResponse401",
+    "DeleteProjectSourceResponse401Data",
+    "DeleteProjectSourceResponse401DataCode",
+    "DeleteProjectSourceResponse401Status",
+    "DeleteProjectSourceResponse404",
+    "DeleteProjectSourceResponse404Data",
+    "DeleteProjectSourceResponse404DataCode",
+    "DeleteProjectSourceResponse404DataMessage",
+    "DeleteProjectSourceResponse404Status",
+    "DeleteProjectSourceResponse500",
+    "DeleteProjectSourceResponse500Data",
+    "DeleteProjectSourceResponse500DataCode",
+    "DeleteProjectSourceResponse500Status",
     "GetOpenGraphDataForCitationResponse200",
     "GetOpenGraphDataForCitationResponse200Data",
     "GetOpenGraphDataForCitationResponse200Status",
     "GetOpenGraphDataForCitationResponse401",
     "GetOpenGraphDataForCitationResponse401Data",
     "GetOpenGraphDataForCitationResponse401DataCode",
     "GetOpenGraphDataForCitationResponse401Status",
@@ -444,15 +641,14 @@
     "GetOpenGraphDataForCitationResponse404DataCode",
     "GetOpenGraphDataForCitationResponse404DataMessage",
     "GetOpenGraphDataForCitationResponse404Status",
     "GetProjectConversationsOrder",
     "GetProjectConversationsResponse200",
     "GetProjectConversationsResponse200Data",
     "GetProjectConversationsResponse200DataDataItem",
-    "GetProjectConversationsResponse200DataLinks",
     "GetProjectConversationsResponse200Status",
     "GetProjectConversationsResponse401",
     "GetProjectConversationsResponse401Data",
     "GetProjectConversationsResponse401DataCode",
     "GetProjectConversationsResponse401Status",
     "GetProjectConversationsResponse404",
     "GetProjectConversationsResponse404Data",
@@ -466,15 +662,14 @@
     "GetProjectPagesOrder",
     "GetProjectPagesResponse200",
     "GetProjectPagesResponse200Data",
     "GetProjectPagesResponse200DataPages",
     "GetProjectPagesResponse200DataPagesDataItem",
     "GetProjectPagesResponse200DataPagesDataItemCrawlStatus",
     "GetProjectPagesResponse200DataPagesDataItemIndexStatus",
-    "GetProjectPagesResponse200DataPagesLinks",
     "GetProjectPagesResponse200DataProject",
     "GetProjectPagesResponse200DataProjectType",
     "GetProjectPagesResponse200Status",
     "GetProjectPagesResponse401",
     "GetProjectPagesResponse401Data",
     "GetProjectPagesResponse401DataCode",
     "GetProjectPagesResponse401Status",
@@ -483,14 +678,30 @@
     "GetProjectPagesResponse404DataCode",
     "GetProjectPagesResponse404DataMessage",
     "GetProjectPagesResponse404Status",
     "GetProjectPagesResponse500",
     "GetProjectPagesResponse500Data",
     "GetProjectPagesResponse500DataCode",
     "GetProjectPagesResponse500Status",
+    "GetProjectPluginsResponse200",
+    "GetProjectPluginsResponse200Data",
+    "GetProjectPluginsResponse200Status",
+    "GetProjectPluginsResponse401",
+    "GetProjectPluginsResponse401Data",
+    "GetProjectPluginsResponse401DataCode",
+    "GetProjectPluginsResponse401Status",
+    "GetProjectPluginsResponse404",
+    "GetProjectPluginsResponse404Data",
+    "GetProjectPluginsResponse404DataCode",
+    "GetProjectPluginsResponse404DataMessage",
+    "GetProjectPluginsResponse404Status",
+    "GetProjectPluginsResponse500",
+    "GetProjectPluginsResponse500Data",
+    "GetProjectPluginsResponse500DataCode",
+    "GetProjectPluginsResponse500Status",
     "GetProjectResponse200",
     "GetProjectResponse200Data",
     "GetProjectResponse200DataType",
     "GetProjectResponse200Status",
     "GetProjectResponse401",
     "GetProjectResponse401Data",
     "GetProjectResponse401DataCode",
@@ -529,34 +740,61 @@
     "GetUserProfileResponse401DataCode",
     "GetUserProfileResponse401Status",
     "GetUserProfileResponse500",
     "GetUserProfileResponse500Data",
     "GetUserProfileResponse500DataCode",
     "GetUserProfileResponse500Status",
     "ListProjectsOrder",
+    "ListProjectSourcesResponse200",
+    "ListProjectSourcesResponse200Data",
+    "ListProjectSourcesResponse200DataSitemapsItem",
+    "ListProjectSourcesResponse200DataSitemapsItemPagesItem",
+    "ListProjectSourcesResponse200DataSitemapsItemPagesItemCrawlStatus",
+    "ListProjectSourcesResponse200DataSitemapsItemPagesItemIndexStatus",
+    "ListProjectSourcesResponse200DataSitemapsItemSettings",
+    "ListProjectSourcesResponse200DataSitemapsItemType",
+    "ListProjectSourcesResponse200DataUploads",
+    "ListProjectSourcesResponse200DataUploadsPagesItem",
+    "ListProjectSourcesResponse200DataUploadsPagesItemCrawlStatus",
+    "ListProjectSourcesResponse200DataUploadsPagesItemIndexStatus",
+    "ListProjectSourcesResponse200DataUploadsSettings",
+    "ListProjectSourcesResponse200DataUploadsType",
+    "ListProjectSourcesResponse200Status",
+    "ListProjectSourcesResponse401",
+    "ListProjectSourcesResponse401Data",
+    "ListProjectSourcesResponse401DataCode",
+    "ListProjectSourcesResponse401Status",
+    "ListProjectSourcesResponse404",
+    "ListProjectSourcesResponse404Data",
+    "ListProjectSourcesResponse404DataCode",
+    "ListProjectSourcesResponse404DataMessage",
+    "ListProjectSourcesResponse404Status",
+    "ListProjectSourcesResponse500",
+    "ListProjectSourcesResponse500Data",
+    "ListProjectSourcesResponse500DataCode",
+    "ListProjectSourcesResponse500Status",
     "ListProjectsResponse200",
     "ListProjectsResponse200Data",
     "ListProjectsResponse200DataDataItem",
     "ListProjectsResponse200DataDataItemType",
-    "ListProjectsResponse200DataLinks",
     "ListProjectsResponse200Status",
     "ListProjectsResponse401",
     "ListProjectsResponse401Data",
     "ListProjectsResponse401DataCode",
     "ListProjectsResponse401Status",
     "ListProjectsResponse500",
     "ListProjectsResponse500Data",
     "ListProjectsResponse500DataCode",
     "ListProjectsResponse500Status",
     "MessagesOrder",
     "MessagesResponse200",
-    "MessagesResponse200Conversation",
-    "MessagesResponse200Messages",
-    "MessagesResponse200MessagesDataItem",
-    "MessagesResponse200MessagesLinks",
+    "MessagesResponse200Data",
+    "MessagesResponse200DataConversation",
+    "MessagesResponse200DataMessages",
+    "MessagesResponse200DataMessagesDataItem",
     "MessagesResponse200Status",
     "MessagesResponse401",
     "MessagesResponse401Data",
     "MessagesResponse401DataCode",
     "MessagesResponse401Status",
     "MessagesResponse404",
     "MessagesResponse404Data",
@@ -584,14 +822,17 @@
     "PreviewResponse500Data",
     "PreviewResponse500DataCode",
     "PreviewResponse500Status",
     "Project",
     "ProjectPlugin",
     "ProjectSettings",
     "ProjectSettingsResponseSource",
+    "ProjectSource",
+    "ProjectSourceSettings",
+    "ProjectSourceType",
     "ProjectType",
     "PromptHistory",
     "SendMessageToConversationJsonBody",
     "SendMessageToConversationResponse200",
     "SendMessageToConversationResponse200Data",
     "SendMessageToConversationResponse200Status",
     "SendMessageToConversationResponse401",
@@ -637,14 +878,31 @@
     "UpdateProjectConversationResponse404DataMessage",
     "UpdateProjectConversationResponse404Status",
     "UpdateProjectConversationResponse500",
     "UpdateProjectConversationResponse500Data",
     "UpdateProjectConversationResponse500DataCode",
     "UpdateProjectConversationResponse500Status",
     "UpdateProjectMultipartData",
+    "UpdateProjectPluginJsonBody",
+    "UpdateProjectPluginResponse200",
+    "UpdateProjectPluginResponse200Data",
+    "UpdateProjectPluginResponse200Status",
+    "UpdateProjectPluginResponse401",
+    "UpdateProjectPluginResponse401Data",
+    "UpdateProjectPluginResponse401DataCode",
+    "UpdateProjectPluginResponse401Status",
+    "UpdateProjectPluginResponse404",
+    "UpdateProjectPluginResponse404Data",
+    "UpdateProjectPluginResponse404DataCode",
+    "UpdateProjectPluginResponse404DataMessage",
+    "UpdateProjectPluginResponse404Status",
+    "UpdateProjectPluginResponse500",
+    "UpdateProjectPluginResponse500Data",
+    "UpdateProjectPluginResponse500DataCode",
+    "UpdateProjectPluginResponse500Status",
     "UpdateProjectResponse200",
     "UpdateProjectResponse200Data",
     "UpdateProjectResponse200DataType",
     "UpdateProjectResponse200Status",
     "UpdateProjectResponse401",
     "UpdateProjectResponse401Data",
     "UpdateProjectResponse401DataCode",
```

## customgpt_client/models/conversation.py

```diff
@@ -72,58 +72,57 @@
         if session_id is not UNSET:
             field_dict["session_id"] = session_id
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _created_at = d.pop("created_at", UNSET)
+        _created_at = src_dict.get("created_at")
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
-        _updated_at = d.pop("updated_at", UNSET)
+        _updated_at = src_dict.get("updated_at")
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
-        _deleted_at = d.pop("deleted_at", UNSET)
+        _deleted_at = src_dict.get("deleted_at")
         deleted_at: Union[Unset, datetime.datetime]
         if isinstance(_deleted_at, Unset):
             deleted_at = UNSET
         else:
             deleted_at = isoparse(_deleted_at)
 
-        id = d.pop("id", UNSET)
+        id = src_dict.get("id")
 
-        name = d.pop("name", UNSET)
+        name = src_dict.get("name")
 
-        project_id = d.pop("project_id", UNSET)
+        project_id = src_dict.get("project_id")
 
-        created_by = d.pop("created_by", UNSET)
+        created_by = src_dict.get("created_by")
 
-        session_id = d.pop("session_id", UNSET)
+        session_id = src_dict.get("session_id")
 
         conversation = cls(
             created_at=created_at,
             updated_at=updated_at,
             deleted_at=deleted_at,
             id=id,
             name=name,
             project_id=project_id,
             created_by=created_by,
             session_id=session_id,
         )
 
-        conversation.additional_properties = d
+        conversation.additional_properties = src_dict
         return conversation
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/create_project_conversation_json_body.py

```diff
@@ -26,22 +26,21 @@
         if name is not UNSET:
             field_dict["name"] = name
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        name = d.pop("name", UNSET)
+        name = src_dict.get("name")
 
         create_project_conversation_json_body = cls(
             name=name,
         )
 
-        create_project_conversation_json_body.additional_properties = d
+        create_project_conversation_json_body.additional_properties = src_dict
         return create_project_conversation_json_body
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/create_project_conversation_response_201.py

```diff
@@ -43,35 +43,34 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.create_project_conversation_response_201_data import CreateProjectConversationResponse201Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, CreateProjectConversationResponse201Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = CreateProjectConversationResponse201Status(_status)
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, CreateProjectConversationResponse201Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = CreateProjectConversationResponse201Data.from_dict(_data)
 
         create_project_conversation_response_201 = cls(
             status=status,
             data=data,
         )
 
-        create_project_conversation_response_201.additional_properties = d
+        create_project_conversation_response_201.additional_properties = src_dict
         return create_project_conversation_response_201
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/create_project_conversation_response_201_data.py

```diff
@@ -11,25 +11,26 @@
 
 @attr.s(auto_attribs=True)
 class CreateProjectConversationResponse201Data:
     """
     Attributes:
         created_at (Union[Unset, datetime.datetime]): When was this conversation created? Example: 2023-04-30 16:43:53.
         updated_at (Union[Unset, datetime.datetime]): When was this conversation updated? Example: 2023-04-30 16:43:53.
-        deleted_at (Union[Unset, datetime.datetime]): When was this conversation deleted? Example: 2023-04-30 16:43:53.
+        deleted_at (Union[Unset, None, datetime.datetime]): When was this conversation deleted? Example: 2023-04-30
+            16:43:53.
         id (Union[Unset, int]): Conversation ID Example: 1.
         name (Union[Unset, str]): Conversation name Example: Conversation 1.
         project_id (Union[Unset, str]): Project ID for this conversation Example: 1.
         created_by (Union[Unset, str]): User ID for the user who created this conversation Example: 1.
         session_id (Union[Unset, str]): Session ID for this conversation Example: f1b9aaf0-5e4e-11eb-ae93-0242ac130002.
     """
 
     created_at: Union[Unset, datetime.datetime] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
-    deleted_at: Union[Unset, datetime.datetime] = UNSET
+    deleted_at: Union[Unset, None, datetime.datetime] = UNSET
     id: Union[Unset, int] = UNSET
     name: Union[Unset, str] = UNSET
     project_id: Union[Unset, str] = UNSET
     created_by: Union[Unset, str] = UNSET
     session_id: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -38,17 +39,17 @@
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
 
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
 
-        deleted_at: Union[Unset, str] = UNSET
+        deleted_at: Union[Unset, None, str] = UNSET
         if not isinstance(self.deleted_at, Unset):
-            deleted_at = self.deleted_at.isoformat()
+            deleted_at = self.deleted_at.isoformat() if self.deleted_at else None
 
         id = self.id
         name = self.name
         project_id = self.project_id
         created_by = self.created_by
         session_id = self.session_id
 
@@ -72,58 +73,59 @@
         if session_id is not UNSET:
             field_dict["session_id"] = session_id
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _created_at = d.pop("created_at", UNSET)
+        _created_at = src_dict.get("created_at")
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
-        _updated_at = d.pop("updated_at", UNSET)
+        _updated_at = src_dict.get("updated_at")
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
-        _deleted_at = d.pop("deleted_at", UNSET)
-        deleted_at: Union[Unset, datetime.datetime]
-        if isinstance(_deleted_at, Unset):
+        _deleted_at = src_dict.get("deleted_at")
+        deleted_at: Union[Unset, None, datetime.datetime]
+        if _deleted_at is None:
+            deleted_at = None
+        elif isinstance(_deleted_at, Unset):
             deleted_at = UNSET
         else:
             deleted_at = isoparse(_deleted_at)
 
-        id = d.pop("id", UNSET)
+        id = src_dict.get("id")
 
-        name = d.pop("name", UNSET)
+        name = src_dict.get("name")
 
-        project_id = d.pop("project_id", UNSET)
+        project_id = src_dict.get("project_id")
 
-        created_by = d.pop("created_by", UNSET)
+        created_by = src_dict.get("created_by")
 
-        session_id = d.pop("session_id", UNSET)
+        session_id = src_dict.get("session_id")
 
         create_project_conversation_response_201_data = cls(
             created_at=created_at,
             updated_at=updated_at,
             deleted_at=deleted_at,
             id=id,
             name=name,
             project_id=project_id,
             created_by=created_by,
             session_id=session_id,
         )
 
-        create_project_conversation_response_201_data.additional_properties = d
+        create_project_conversation_response_201_data.additional_properties = src_dict
         return create_project_conversation_response_201_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/create_project_conversation_response_401.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.create_project_conversation_response_401_data import CreateProjectConversationResponse401Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, CreateProjectConversationResponse401Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = CreateProjectConversationResponse401Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, CreateProjectConversationResponse401Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = CreateProjectConversationResponse401Data.from_dict(_data)
 
         create_project_conversation_response_401 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        create_project_conversation_response_401.additional_properties = d
+        create_project_conversation_response_401.additional_properties = src_dict
         return create_project_conversation_response_401
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/create_project_conversation_response_401_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, CreateProjectConversationResponse401DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = CreateProjectConversationResponse401DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         create_project_conversation_response_401_data = cls(
             code=code,
             message=message,
         )
 
-        create_project_conversation_response_401_data.additional_properties = d
+        create_project_conversation_response_401_data.additional_properties = src_dict
         return create_project_conversation_response_401_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/create_project_conversation_response_404.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.create_project_conversation_response_404_data import CreateProjectConversationResponse404Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, CreateProjectConversationResponse404Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = CreateProjectConversationResponse404Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, CreateProjectConversationResponse404Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = CreateProjectConversationResponse404Data.from_dict(_data)
 
         create_project_conversation_response_404 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        create_project_conversation_response_404.additional_properties = d
+        create_project_conversation_response_404.additional_properties = src_dict
         return create_project_conversation_response_404
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/create_project_conversation_response_404_data.py

```diff
@@ -41,35 +41,34 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, CreateProjectConversationResponse404DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = CreateProjectConversationResponse404DataCode(_code)
 
-        _message = d.pop("message", UNSET)
+        _message = src_dict.get("message")
         message: Union[Unset, CreateProjectConversationResponse404DataMessage]
         if isinstance(_message, Unset):
             message = UNSET
         else:
             message = CreateProjectConversationResponse404DataMessage(_message)
 
         create_project_conversation_response_404_data = cls(
             code=code,
             message=message,
         )
 
-        create_project_conversation_response_404_data.additional_properties = d
+        create_project_conversation_response_404_data.additional_properties = src_dict
         return create_project_conversation_response_404_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/create_project_conversation_response_500.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.create_project_conversation_response_500_data import CreateProjectConversationResponse500Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, CreateProjectConversationResponse500Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = CreateProjectConversationResponse500Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, CreateProjectConversationResponse500Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = CreateProjectConversationResponse500Data.from_dict(_data)
 
         create_project_conversation_response_500 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        create_project_conversation_response_500.additional_properties = d
+        create_project_conversation_response_500.additional_properties = src_dict
         return create_project_conversation_response_500
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/create_project_conversation_response_500_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, CreateProjectConversationResponse500DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = CreateProjectConversationResponse500DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         create_project_conversation_response_500_data = cls(
             code=code,
             message=message,
         )
 
-        create_project_conversation_response_500_data.additional_properties = d
+        create_project_conversation_response_500_data.additional_properties = src_dict
         return create_project_conversation_response_500_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/create_project_multipart_data.py

```diff
@@ -80,36 +80,35 @@
         if file is not UNSET:
             field_dict["file"] = file
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        project_name = d.pop("project_name", UNSET)
+        project_name = src_dict.get("project_name")
 
-        sitemap_path = d.pop("sitemap_path", UNSET)
+        sitemap_path = src_dict.get("sitemap_path")
 
-        file_data_retension = d.pop("file_data_retension", UNSET)
+        file_data_retension = src_dict.get("file_data_retension")
 
-        _file = d.pop("file", UNSET)
+        _file = src_dict.get("file")
         file: Union[Unset, File]
         if isinstance(_file, Unset):
             file = UNSET
         else:
             file = File(payload=BytesIO(_file))
 
         create_project_multipart_data = cls(
             project_name=project_name,
             sitemap_path=sitemap_path,
             file_data_retension=file_data_retension,
             file=file,
         )
 
-        create_project_multipart_data.additional_properties = d
+        create_project_multipart_data.additional_properties = src_dict
         return create_project_multipart_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/create_project_response_201.py

```diff
@@ -43,35 +43,34 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.create_project_response_201_data import CreateProjectResponse201Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, CreateProjectResponse201Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = CreateProjectResponse201Status(_status)
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, CreateProjectResponse201Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = CreateProjectResponse201Data.from_dict(_data)
 
         create_project_response_201 = cls(
             status=status,
             data=data,
         )
 
-        create_project_response_201.additional_properties = d
+        create_project_response_201.additional_properties = src_dict
         return create_project_response_201
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/create_project_response_201_data.py

```diff
@@ -111,64 +111,63 @@
         if live_chat_code is not UNSET:
             field_dict["live_chat_code"] = live_chat_code
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        id = d.pop("id", UNSET)
+        id = src_dict.get("id")
 
-        project_name = d.pop("project_name", UNSET)
+        project_name = src_dict.get("project_name")
 
-        sitemap_path = d.pop("sitemap_path", UNSET)
+        sitemap_path = src_dict.get("sitemap_path")
 
-        is_chat_active = d.pop("is_chat_active", UNSET)
+        is_chat_active = src_dict.get("is_chat_active")
 
-        user_id = d.pop("user_id", UNSET)
+        user_id = src_dict.get("user_id")
 
-        _created_at = d.pop("created_at", UNSET)
+        _created_at = src_dict.get("created_at")
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
-        _updated_at = d.pop("updated_at", UNSET)
+        _updated_at = src_dict.get("updated_at")
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
-        _deleted_at = d.pop("deleted_at", UNSET)
+        _deleted_at = src_dict.get("deleted_at")
         deleted_at: Union[Unset, None, datetime.datetime]
         if _deleted_at is None:
             deleted_at = None
         elif isinstance(_deleted_at, Unset):
             deleted_at = UNSET
         else:
             deleted_at = isoparse(_deleted_at)
 
-        _type = d.pop("type", UNSET)
+        _type = src_dict.get("type")
         type: Union[Unset, CreateProjectResponse201DataType]
         if isinstance(_type, Unset):
             type = UNSET
         else:
             type = CreateProjectResponse201DataType(_type)
 
-        is_shared = d.pop("is_shared", UNSET)
+        is_shared = src_dict.get("is_shared")
 
-        shareable_slug = d.pop("shareable_slug", UNSET)
+        shareable_slug = src_dict.get("shareable_slug")
 
-        shareable_link = d.pop("shareable_link", UNSET)
+        shareable_link = src_dict.get("shareable_link")
 
-        embed_code = d.pop("embed_code", UNSET)
+        embed_code = src_dict.get("embed_code")
 
-        live_chat_code = d.pop("live_chat_code", UNSET)
+        live_chat_code = src_dict.get("live_chat_code")
 
         create_project_response_201_data = cls(
             id=id,
             project_name=project_name,
             sitemap_path=sitemap_path,
             is_chat_active=is_chat_active,
             user_id=user_id,
@@ -179,15 +178,15 @@
             is_shared=is_shared,
             shareable_slug=shareable_slug,
             shareable_link=shareable_link,
             embed_code=embed_code,
             live_chat_code=live_chat_code,
         )
 
-        create_project_response_201_data.additional_properties = d
+        create_project_response_201_data.additional_properties = src_dict
         return create_project_response_201_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/create_project_response_400.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.create_project_response_400_data import CreateProjectResponse400Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, CreateProjectResponse400Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = CreateProjectResponse400Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, CreateProjectResponse400Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = CreateProjectResponse400Data.from_dict(_data)
 
         create_project_response_400 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        create_project_response_400.additional_properties = d
+        create_project_response_400.additional_properties = src_dict
         return create_project_response_400
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/create_project_response_400_data.py

```diff
@@ -39,35 +39,34 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, CreateProjectResponse400DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = CreateProjectResponse400DataCode(_code)
 
-        _message = d.pop("message", UNSET)
+        _message = src_dict.get("message")
         message: Union[Unset, CreateProjectResponse400DataMessage]
         if isinstance(_message, Unset):
             message = UNSET
         else:
             message = CreateProjectResponse400DataMessage(_message)
 
         create_project_response_400_data = cls(
             code=code,
             message=message,
         )
 
-        create_project_response_400_data.additional_properties = d
+        create_project_response_400_data.additional_properties = src_dict
         return create_project_response_400_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/create_project_response_401.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.create_project_response_401_data import CreateProjectResponse401Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, CreateProjectResponse401Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = CreateProjectResponse401Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, CreateProjectResponse401Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = CreateProjectResponse401Data.from_dict(_data)
 
         create_project_response_401 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        create_project_response_401.additional_properties = d
+        create_project_response_401.additional_properties = src_dict
         return create_project_response_401
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/create_project_response_401_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, CreateProjectResponse401DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = CreateProjectResponse401DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         create_project_response_401_data = cls(
             code=code,
             message=message,
         )
 
-        create_project_response_401_data.additional_properties = d
+        create_project_response_401_data.additional_properties = src_dict
         return create_project_response_401_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/create_project_response_500.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.create_project_response_500_data import CreateProjectResponse500Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, CreateProjectResponse500Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = CreateProjectResponse500Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, CreateProjectResponse500Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = CreateProjectResponse500Data.from_dict(_data)
 
         create_project_response_500 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        create_project_response_500.additional_properties = d
+        create_project_response_500.additional_properties = src_dict
         return create_project_response_500
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/create_project_response_500_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, CreateProjectResponse500DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = CreateProjectResponse500DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         create_project_response_500_data = cls(
             code=code,
             message=message,
         )
 
-        create_project_response_500_data.additional_properties = d
+        create_project_response_500_data.additional_properties = src_dict
         return create_project_response_500_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/delete_project_conversation_response_200.py

```diff
@@ -43,35 +43,34 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.delete_project_conversation_response_200_data import DeleteProjectConversationResponse200Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, DeleteProjectConversationResponse200Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = DeleteProjectConversationResponse200Status(_status)
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, DeleteProjectConversationResponse200Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = DeleteProjectConversationResponse200Data.from_dict(_data)
 
         delete_project_conversation_response_200 = cls(
             status=status,
             data=data,
         )
 
-        delete_project_conversation_response_200.additional_properties = d
+        delete_project_conversation_response_200.additional_properties = src_dict
         return delete_project_conversation_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/delete_project_conversation_response_200_data.py

```diff
@@ -26,22 +26,21 @@
         if deleted is not UNSET:
             field_dict["deleted"] = deleted
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        deleted = d.pop("deleted", UNSET)
+        deleted = src_dict.get("deleted")
 
         delete_project_conversation_response_200_data = cls(
             deleted=deleted,
         )
 
-        delete_project_conversation_response_200_data.additional_properties = d
+        delete_project_conversation_response_200_data.additional_properties = src_dict
         return delete_project_conversation_response_200_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/delete_project_conversation_response_401.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.delete_project_conversation_response_401_data import DeleteProjectConversationResponse401Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, DeleteProjectConversationResponse401Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = DeleteProjectConversationResponse401Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, DeleteProjectConversationResponse401Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = DeleteProjectConversationResponse401Data.from_dict(_data)
 
         delete_project_conversation_response_401 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        delete_project_conversation_response_401.additional_properties = d
+        delete_project_conversation_response_401.additional_properties = src_dict
         return delete_project_conversation_response_401
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/delete_project_conversation_response_401_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, DeleteProjectConversationResponse401DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = DeleteProjectConversationResponse401DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         delete_project_conversation_response_401_data = cls(
             code=code,
             message=message,
         )
 
-        delete_project_conversation_response_401_data.additional_properties = d
+        delete_project_conversation_response_401_data.additional_properties = src_dict
         return delete_project_conversation_response_401_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/delete_project_conversation_response_404.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.delete_project_conversation_response_404_data import DeleteProjectConversationResponse404Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, DeleteProjectConversationResponse404Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = DeleteProjectConversationResponse404Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, DeleteProjectConversationResponse404Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = DeleteProjectConversationResponse404Data.from_dict(_data)
 
         delete_project_conversation_response_404 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        delete_project_conversation_response_404.additional_properties = d
+        delete_project_conversation_response_404.additional_properties = src_dict
         return delete_project_conversation_response_404
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/delete_project_conversation_response_404_data.py

```diff
@@ -41,35 +41,34 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, DeleteProjectConversationResponse404DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = DeleteProjectConversationResponse404DataCode(_code)
 
-        _message = d.pop("message", UNSET)
+        _message = src_dict.get("message")
         message: Union[Unset, DeleteProjectConversationResponse404DataMessage]
         if isinstance(_message, Unset):
             message = UNSET
         else:
             message = DeleteProjectConversationResponse404DataMessage(_message)
 
         delete_project_conversation_response_404_data = cls(
             code=code,
             message=message,
         )
 
-        delete_project_conversation_response_404_data.additional_properties = d
+        delete_project_conversation_response_404_data.additional_properties = src_dict
         return delete_project_conversation_response_404_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/delete_project_conversation_response_500.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.delete_project_conversation_response_500_data import DeleteProjectConversationResponse500Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, DeleteProjectConversationResponse500Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = DeleteProjectConversationResponse500Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, DeleteProjectConversationResponse500Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = DeleteProjectConversationResponse500Data.from_dict(_data)
 
         delete_project_conversation_response_500 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        delete_project_conversation_response_500.additional_properties = d
+        delete_project_conversation_response_500.additional_properties = src_dict
         return delete_project_conversation_response_500
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/delete_project_conversation_response_500_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, DeleteProjectConversationResponse500DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = DeleteProjectConversationResponse500DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         delete_project_conversation_response_500_data = cls(
             code=code,
             message=message,
         )
 
-        delete_project_conversation_response_500_data.additional_properties = d
+        delete_project_conversation_response_500_data.additional_properties = src_dict
         return delete_project_conversation_response_500_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/delete_project_page_response_200.py

```diff
@@ -43,35 +43,34 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.delete_project_page_response_200_data import DeleteProjectPageResponse200Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, DeleteProjectPageResponse200Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = DeleteProjectPageResponse200Status(_status)
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, DeleteProjectPageResponse200Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = DeleteProjectPageResponse200Data.from_dict(_data)
 
         delete_project_page_response_200 = cls(
             status=status,
             data=data,
         )
 
-        delete_project_page_response_200.additional_properties = d
+        delete_project_page_response_200.additional_properties = src_dict
         return delete_project_page_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/delete_project_page_response_200_data.py

```diff
@@ -26,22 +26,21 @@
         if deleted is not UNSET:
             field_dict["deleted"] = deleted
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        deleted = d.pop("deleted", UNSET)
+        deleted = src_dict.get("deleted")
 
         delete_project_page_response_200_data = cls(
             deleted=deleted,
         )
 
-        delete_project_page_response_200_data.additional_properties = d
+        delete_project_page_response_200_data.additional_properties = src_dict
         return delete_project_page_response_200_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/delete_project_page_response_401.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.delete_project_page_response_401_data import DeleteProjectPageResponse401Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, DeleteProjectPageResponse401Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = DeleteProjectPageResponse401Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, DeleteProjectPageResponse401Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = DeleteProjectPageResponse401Data.from_dict(_data)
 
         delete_project_page_response_401 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        delete_project_page_response_401.additional_properties = d
+        delete_project_page_response_401.additional_properties = src_dict
         return delete_project_page_response_401
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/delete_project_page_response_401_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, DeleteProjectPageResponse401DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = DeleteProjectPageResponse401DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         delete_project_page_response_401_data = cls(
             code=code,
             message=message,
         )
 
-        delete_project_page_response_401_data.additional_properties = d
+        delete_project_page_response_401_data.additional_properties = src_dict
         return delete_project_page_response_401_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/delete_project_page_response_404.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.delete_project_page_response_404_data import DeleteProjectPageResponse404Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, DeleteProjectPageResponse404Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = DeleteProjectPageResponse404Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, DeleteProjectPageResponse404Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = DeleteProjectPageResponse404Data.from_dict(_data)
 
         delete_project_page_response_404 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        delete_project_page_response_404.additional_properties = d
+        delete_project_page_response_404.additional_properties = src_dict
         return delete_project_page_response_404
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/delete_project_page_response_404_data.py

```diff
@@ -39,35 +39,34 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, DeleteProjectPageResponse404DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = DeleteProjectPageResponse404DataCode(_code)
 
-        _message = d.pop("message", UNSET)
+        _message = src_dict.get("message")
         message: Union[Unset, DeleteProjectPageResponse404DataMessage]
         if isinstance(_message, Unset):
             message = UNSET
         else:
             message = DeleteProjectPageResponse404DataMessage(_message)
 
         delete_project_page_response_404_data = cls(
             code=code,
             message=message,
         )
 
-        delete_project_page_response_404_data.additional_properties = d
+        delete_project_page_response_404_data.additional_properties = src_dict
         return delete_project_page_response_404_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/delete_project_page_response_500.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.delete_project_page_response_500_data import DeleteProjectPageResponse500Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, DeleteProjectPageResponse500Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = DeleteProjectPageResponse500Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, DeleteProjectPageResponse500Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = DeleteProjectPageResponse500Data.from_dict(_data)
 
         delete_project_page_response_500 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        delete_project_page_response_500.additional_properties = d
+        delete_project_page_response_500.additional_properties = src_dict
         return delete_project_page_response_500
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/delete_project_page_response_500_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, DeleteProjectPageResponse500DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = DeleteProjectPageResponse500DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         delete_project_page_response_500_data = cls(
             code=code,
             message=message,
         )
 
-        delete_project_page_response_500_data.additional_properties = d
+        delete_project_page_response_500_data.additional_properties = src_dict
         return delete_project_page_response_500_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/delete_project_response_200.py

```diff
@@ -43,35 +43,34 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.delete_project_response_200_data import DeleteProjectResponse200Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, DeleteProjectResponse200Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = DeleteProjectResponse200Status(_status)
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, DeleteProjectResponse200Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = DeleteProjectResponse200Data.from_dict(_data)
 
         delete_project_response_200 = cls(
             status=status,
             data=data,
         )
 
-        delete_project_response_200.additional_properties = d
+        delete_project_response_200.additional_properties = src_dict
         return delete_project_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/delete_project_response_200_data.py

```diff
@@ -26,22 +26,21 @@
         if deleted is not UNSET:
             field_dict["deleted"] = deleted
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        deleted = d.pop("deleted", UNSET)
+        deleted = src_dict.get("deleted")
 
         delete_project_response_200_data = cls(
             deleted=deleted,
         )
 
-        delete_project_response_200_data.additional_properties = d
+        delete_project_response_200_data.additional_properties = src_dict
         return delete_project_response_200_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/delete_project_response_401.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.delete_project_response_401_data import DeleteProjectResponse401Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, DeleteProjectResponse401Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = DeleteProjectResponse401Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, DeleteProjectResponse401Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = DeleteProjectResponse401Data.from_dict(_data)
 
         delete_project_response_401 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        delete_project_response_401.additional_properties = d
+        delete_project_response_401.additional_properties = src_dict
         return delete_project_response_401
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/delete_project_response_401_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, DeleteProjectResponse401DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = DeleteProjectResponse401DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         delete_project_response_401_data = cls(
             code=code,
             message=message,
         )
 
-        delete_project_response_401_data.additional_properties = d
+        delete_project_response_401_data.additional_properties = src_dict
         return delete_project_response_401_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/delete_project_response_404.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.delete_project_response_404_data import DeleteProjectResponse404Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, DeleteProjectResponse404Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = DeleteProjectResponse404Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, DeleteProjectResponse404Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = DeleteProjectResponse404Data.from_dict(_data)
 
         delete_project_response_404 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        delete_project_response_404.additional_properties = d
+        delete_project_response_404.additional_properties = src_dict
         return delete_project_response_404
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/delete_project_response_404_data.py

```diff
@@ -39,35 +39,34 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, DeleteProjectResponse404DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = DeleteProjectResponse404DataCode(_code)
 
-        _message = d.pop("message", UNSET)
+        _message = src_dict.get("message")
         message: Union[Unset, DeleteProjectResponse404DataMessage]
         if isinstance(_message, Unset):
             message = UNSET
         else:
             message = DeleteProjectResponse404DataMessage(_message)
 
         delete_project_response_404_data = cls(
             code=code,
             message=message,
         )
 
-        delete_project_response_404_data.additional_properties = d
+        delete_project_response_404_data.additional_properties = src_dict
         return delete_project_response_404_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/delete_project_response_500.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.delete_project_response_500_data import DeleteProjectResponse500Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, DeleteProjectResponse500Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = DeleteProjectResponse500Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, DeleteProjectResponse500Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = DeleteProjectResponse500Data.from_dict(_data)
 
         delete_project_response_500 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        delete_project_response_500.additional_properties = d
+        delete_project_response_500.additional_properties = src_dict
         return delete_project_response_500
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/delete_project_response_500_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, DeleteProjectResponse500DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = DeleteProjectResponse500DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         delete_project_response_500_data = cls(
             code=code,
             message=message,
         )
 
-        delete_project_response_500_data.additional_properties = d
+        delete_project_response_500_data.additional_properties = src_dict
         return delete_project_response_500_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_open_graph_data_for_citation_response_200.py

```diff
@@ -46,35 +46,34 @@
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.get_open_graph_data_for_citation_response_200_data import (
             GetOpenGraphDataForCitationResponse200Data,
         )
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, GetOpenGraphDataForCitationResponse200Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = GetOpenGraphDataForCitationResponse200Status(_status)
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, GetOpenGraphDataForCitationResponse200Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = GetOpenGraphDataForCitationResponse200Data.from_dict(_data)
 
         get_open_graph_data_for_citation_response_200 = cls(
             status=status,
             data=data,
         )
 
-        get_open_graph_data_for_citation_response_200.additional_properties = d
+        get_open_graph_data_for_citation_response_200.additional_properties = src_dict
         return get_open_graph_data_for_citation_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_open_graph_data_for_citation_response_200_data.py

```diff
@@ -68,46 +68,45 @@
         if site_name is not UNSET:
             field_dict["site_name"] = site_name
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        page_url = d.pop("page_url", UNSET)
+        page_url = src_dict.get("page_url")
 
-        title = d.pop("title", UNSET)
+        title = src_dict.get("title")
 
-        description = d.pop("description", UNSET)
+        description = src_dict.get("description")
 
-        image = d.pop("image", UNSET)
+        image = src_dict.get("image")
 
-        image_width = d.pop("image_width", UNSET)
+        image_width = src_dict.get("image_width")
 
-        image_height = d.pop("image_height", UNSET)
+        image_height = src_dict.get("image_height")
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        favicon = d.pop("favicon", UNSET)
+        favicon = src_dict.get("favicon")
 
-        site_name = d.pop("site_name", UNSET)
+        site_name = src_dict.get("site_name")
 
         get_open_graph_data_for_citation_response_200_data = cls(
             page_url=page_url,
             title=title,
             description=description,
             image=image,
             image_width=image_width,
             image_height=image_height,
             url=url,
             favicon=favicon,
             site_name=site_name,
         )
 
-        get_open_graph_data_for_citation_response_200_data.additional_properties = d
+        get_open_graph_data_for_citation_response_200_data.additional_properties = src_dict
         return get_open_graph_data_for_citation_response_200_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_open_graph_data_for_citation_response_401.py

```diff
@@ -50,38 +50,37 @@
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.get_open_graph_data_for_citation_response_401_data import (
             GetOpenGraphDataForCitationResponse401Data,
         )
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, GetOpenGraphDataForCitationResponse401Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = GetOpenGraphDataForCitationResponse401Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, GetOpenGraphDataForCitationResponse401Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = GetOpenGraphDataForCitationResponse401Data.from_dict(_data)
 
         get_open_graph_data_for_citation_response_401 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        get_open_graph_data_for_citation_response_401.additional_properties = d
+        get_open_graph_data_for_citation_response_401.additional_properties = src_dict
         return get_open_graph_data_for_citation_response_401
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_open_graph_data_for_citation_response_401_data.py

```diff
@@ -37,30 +37,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, GetOpenGraphDataForCitationResponse401DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = GetOpenGraphDataForCitationResponse401DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         get_open_graph_data_for_citation_response_401_data = cls(
             code=code,
             message=message,
         )
 
-        get_open_graph_data_for_citation_response_401_data.additional_properties = d
+        get_open_graph_data_for_citation_response_401_data.additional_properties = src_dict
         return get_open_graph_data_for_citation_response_401_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_open_graph_data_for_citation_response_404.py

```diff
@@ -50,38 +50,37 @@
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.get_open_graph_data_for_citation_response_404_data import (
             GetOpenGraphDataForCitationResponse404Data,
         )
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, GetOpenGraphDataForCitationResponse404Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = GetOpenGraphDataForCitationResponse404Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, GetOpenGraphDataForCitationResponse404Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = GetOpenGraphDataForCitationResponse404Data.from_dict(_data)
 
         get_open_graph_data_for_citation_response_404 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        get_open_graph_data_for_citation_response_404.additional_properties = d
+        get_open_graph_data_for_citation_response_404.additional_properties = src_dict
         return get_open_graph_data_for_citation_response_404
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_open_graph_data_for_citation_response_404_data.py

```diff
@@ -43,35 +43,34 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, GetOpenGraphDataForCitationResponse404DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = GetOpenGraphDataForCitationResponse404DataCode(_code)
 
-        _message = d.pop("message", UNSET)
+        _message = src_dict.get("message")
         message: Union[Unset, GetOpenGraphDataForCitationResponse404DataMessage]
         if isinstance(_message, Unset):
             message = UNSET
         else:
             message = GetOpenGraphDataForCitationResponse404DataMessage(_message)
 
         get_open_graph_data_for_citation_response_404_data = cls(
             code=code,
             message=message,
         )
 
-        get_open_graph_data_for_citation_response_404_data.additional_properties = d
+        get_open_graph_data_for_citation_response_404_data.additional_properties = src_dict
         return get_open_graph_data_for_citation_response_404_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_conversations_response_200.py

```diff
@@ -43,35 +43,34 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.get_project_conversations_response_200_data import GetProjectConversationsResponse200Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, GetProjectConversationsResponse200Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = GetProjectConversationsResponse200Status(_status)
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, GetProjectConversationsResponse200Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = GetProjectConversationsResponse200Data.from_dict(_data)
 
         get_project_conversations_response_200 = cls(
             status=status,
             data=data,
         )
 
-        get_project_conversations_response_200.additional_properties = d
+        get_project_conversations_response_200.additional_properties = src_dict
         return get_project_conversations_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_conversations_response_200_data.py

```diff
@@ -4,15 +4,14 @@
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.get_project_conversations_response_200_data_data_item import (
         GetProjectConversationsResponse200DataDataItem,
     )
-    from ..models.get_project_conversations_response_200_data_links import GetProjectConversationsResponse200DataLinks
 
 
 T = TypeVar("T", bound="GetProjectConversationsResponse200Data")
 
 
 @attr.s(auto_attribs=True)
 class GetProjectConversationsResponse200Data:
@@ -20,30 +19,28 @@
     Attributes:
         current_page (Union[Unset, int]): The current page number Example: 1.
         data (Union[Unset, List['GetProjectConversationsResponse200DataDataItem']]):
         first_page_url (Union[Unset, str]): The first page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         from_ (Union[Unset, int]): The first item number of the current page Example: 1.
         last_page (Union[Unset, int]): The last page number Example: 1.
         last_page_url (Union[Unset, str]): The last page url Example: https://app.customgpt.ai/api/v1/users?page=1.
-        links (Union[Unset, GetProjectConversationsResponse200DataLinks]):
         next_page_url (Union[Unset, str]): The next page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         path (Union[Unset, str]): The current page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         per_page (Union[Unset, int]): The number of items per page Example: 10.
         prev_page_url (Union[Unset, str]): The previous page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         to (Union[Unset, int]): The last item number of the current page Example: 1.
         total (Union[Unset, int]): The total number of items Example: 1.
     """
 
     current_page: Union[Unset, int] = UNSET
     data: Union[Unset, List["GetProjectConversationsResponse200DataDataItem"]] = UNSET
     first_page_url: Union[Unset, str] = UNSET
     from_: Union[Unset, int] = UNSET
     last_page: Union[Unset, int] = UNSET
     last_page_url: Union[Unset, str] = UNSET
-    links: Union[Unset, "GetProjectConversationsResponse200DataLinks"] = UNSET
     next_page_url: Union[Unset, str] = UNSET
     path: Union[Unset, str] = UNSET
     per_page: Union[Unset, int] = UNSET
     prev_page_url: Union[Unset, str] = UNSET
     to: Union[Unset, int] = UNSET
     total: Union[Unset, int] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
@@ -58,18 +55,14 @@
 
                 data.append(data_item)
 
         first_page_url = self.first_page_url
         from_ = self.from_
         last_page = self.last_page
         last_page_url = self.last_page_url
-        links: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.links, Unset):
-            links = self.links.to_dict()
-
         next_page_url = self.next_page_url
         path = self.path
         per_page = self.per_page
         prev_page_url = self.prev_page_url
         to = self.to
         total = self.total
 
@@ -85,16 +78,14 @@
             field_dict["first_page_url"] = first_page_url
         if from_ is not UNSET:
             field_dict["from"] = from_
         if last_page is not UNSET:
             field_dict["last_page"] = last_page
         if last_page_url is not UNSET:
             field_dict["last_page_url"] = last_page_url
-        if links is not UNSET:
-            field_dict["links"] = links
         if next_page_url is not UNSET:
             field_dict["next_page_url"] = next_page_url
         if path is not UNSET:
             field_dict["path"] = path
         if per_page is not UNSET:
             field_dict["per_page"] = per_page
         if prev_page_url is not UNSET:
@@ -107,72 +98,60 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.get_project_conversations_response_200_data_data_item import (
             GetProjectConversationsResponse200DataDataItem,
         )
-        from ..models.get_project_conversations_response_200_data_links import (
-            GetProjectConversationsResponse200DataLinks,
-        )
 
-        d = src_dict.copy()
-        current_page = d.pop("current_page", UNSET)
+        current_page = src_dict.get("current_page")
 
         data = []
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         for data_item_data in _data or []:
             data_item = GetProjectConversationsResponse200DataDataItem.from_dict(data_item_data)
 
             data.append(data_item)
 
-        first_page_url = d.pop("first_page_url", UNSET)
-
-        from_ = d.pop("from", UNSET)
+        first_page_url = src_dict.get("first_page_url")
 
-        last_page = d.pop("last_page", UNSET)
+        from_ = src_dict.get("from")
 
-        last_page_url = d.pop("last_page_url", UNSET)
+        last_page = src_dict.get("last_page")
 
-        _links = d.pop("links", UNSET)
-        links: Union[Unset, GetProjectConversationsResponse200DataLinks]
-        if isinstance(_links, Unset):
-            links = UNSET
-        else:
-            links = GetProjectConversationsResponse200DataLinks.from_dict(_links)
+        last_page_url = src_dict.get("last_page_url")
 
-        next_page_url = d.pop("next_page_url", UNSET)
+        next_page_url = src_dict.get("next_page_url")
 
-        path = d.pop("path", UNSET)
+        path = src_dict.get("path")
 
-        per_page = d.pop("per_page", UNSET)
+        per_page = src_dict.get("per_page")
 
-        prev_page_url = d.pop("prev_page_url", UNSET)
+        prev_page_url = src_dict.get("prev_page_url")
 
-        to = d.pop("to", UNSET)
+        to = src_dict.get("to")
 
-        total = d.pop("total", UNSET)
+        total = src_dict.get("total")
 
         get_project_conversations_response_200_data = cls(
             current_page=current_page,
             data=data,
             first_page_url=first_page_url,
             from_=from_,
             last_page=last_page,
             last_page_url=last_page_url,
-            links=links,
             next_page_url=next_page_url,
             path=path,
             per_page=per_page,
             prev_page_url=prev_page_url,
             to=to,
             total=total,
         )
 
-        get_project_conversations_response_200_data.additional_properties = d
+        get_project_conversations_response_200_data.additional_properties = src_dict
         return get_project_conversations_response_200_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_conversations_response_200_data_data_item.py

```diff
@@ -11,25 +11,26 @@
 
 @attr.s(auto_attribs=True)
 class GetProjectConversationsResponse200DataDataItem:
     """
     Attributes:
         created_at (Union[Unset, datetime.datetime]): When was this conversation created? Example: 2023-04-30 16:43:53.
         updated_at (Union[Unset, datetime.datetime]): When was this conversation updated? Example: 2023-04-30 16:43:53.
-        deleted_at (Union[Unset, datetime.datetime]): When was this conversation deleted? Example: 2023-04-30 16:43:53.
+        deleted_at (Union[Unset, None, datetime.datetime]): When was this conversation deleted? Example: 2023-04-30
+            16:43:53.
         id (Union[Unset, int]): Conversation ID Example: 1.
         name (Union[Unset, str]): Conversation name Example: Conversation 1.
         project_id (Union[Unset, str]): Project ID for this conversation Example: 1.
         created_by (Union[Unset, str]): User ID for the user who created this conversation Example: 1.
         session_id (Union[Unset, str]): Session ID for this conversation Example: f1b9aaf0-5e4e-11eb-ae93-0242ac130002.
     """
 
     created_at: Union[Unset, datetime.datetime] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
-    deleted_at: Union[Unset, datetime.datetime] = UNSET
+    deleted_at: Union[Unset, None, datetime.datetime] = UNSET
     id: Union[Unset, int] = UNSET
     name: Union[Unset, str] = UNSET
     project_id: Union[Unset, str] = UNSET
     created_by: Union[Unset, str] = UNSET
     session_id: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -38,17 +39,17 @@
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
 
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
 
-        deleted_at: Union[Unset, str] = UNSET
+        deleted_at: Union[Unset, None, str] = UNSET
         if not isinstance(self.deleted_at, Unset):
-            deleted_at = self.deleted_at.isoformat()
+            deleted_at = self.deleted_at.isoformat() if self.deleted_at else None
 
         id = self.id
         name = self.name
         project_id = self.project_id
         created_by = self.created_by
         session_id = self.session_id
 
@@ -72,58 +73,59 @@
         if session_id is not UNSET:
             field_dict["session_id"] = session_id
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _created_at = d.pop("created_at", UNSET)
+        _created_at = src_dict.get("created_at")
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
-        _updated_at = d.pop("updated_at", UNSET)
+        _updated_at = src_dict.get("updated_at")
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
-        _deleted_at = d.pop("deleted_at", UNSET)
-        deleted_at: Union[Unset, datetime.datetime]
-        if isinstance(_deleted_at, Unset):
+        _deleted_at = src_dict.get("deleted_at")
+        deleted_at: Union[Unset, None, datetime.datetime]
+        if _deleted_at is None:
+            deleted_at = None
+        elif isinstance(_deleted_at, Unset):
             deleted_at = UNSET
         else:
             deleted_at = isoparse(_deleted_at)
 
-        id = d.pop("id", UNSET)
+        id = src_dict.get("id")
 
-        name = d.pop("name", UNSET)
+        name = src_dict.get("name")
 
-        project_id = d.pop("project_id", UNSET)
+        project_id = src_dict.get("project_id")
 
-        created_by = d.pop("created_by", UNSET)
+        created_by = src_dict.get("created_by")
 
-        session_id = d.pop("session_id", UNSET)
+        session_id = src_dict.get("session_id")
 
         get_project_conversations_response_200_data_data_item = cls(
             created_at=created_at,
             updated_at=updated_at,
             deleted_at=deleted_at,
             id=id,
             name=name,
             project_id=project_id,
             created_by=created_by,
             session_id=session_id,
         )
 
-        get_project_conversations_response_200_data_data_item.additional_properties = d
+        get_project_conversations_response_200_data_data_item.additional_properties = src_dict
         return get_project_conversations_response_200_data_data_item
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_conversations_response_401.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.get_project_conversations_response_401_data import GetProjectConversationsResponse401Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, GetProjectConversationsResponse401Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = GetProjectConversationsResponse401Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, GetProjectConversationsResponse401Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = GetProjectConversationsResponse401Data.from_dict(_data)
 
         get_project_conversations_response_401 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        get_project_conversations_response_401.additional_properties = d
+        get_project_conversations_response_401.additional_properties = src_dict
         return get_project_conversations_response_401
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_conversations_response_401_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, GetProjectConversationsResponse401DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = GetProjectConversationsResponse401DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         get_project_conversations_response_401_data = cls(
             code=code,
             message=message,
         )
 
-        get_project_conversations_response_401_data.additional_properties = d
+        get_project_conversations_response_401_data.additional_properties = src_dict
         return get_project_conversations_response_401_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_conversations_response_404.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.get_project_conversations_response_404_data import GetProjectConversationsResponse404Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, GetProjectConversationsResponse404Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = GetProjectConversationsResponse404Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, GetProjectConversationsResponse404Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = GetProjectConversationsResponse404Data.from_dict(_data)
 
         get_project_conversations_response_404 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        get_project_conversations_response_404.additional_properties = d
+        get_project_conversations_response_404.additional_properties = src_dict
         return get_project_conversations_response_404
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_conversations_response_404_data.py

```diff
@@ -39,35 +39,34 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, GetProjectConversationsResponse404DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = GetProjectConversationsResponse404DataCode(_code)
 
-        _message = d.pop("message", UNSET)
+        _message = src_dict.get("message")
         message: Union[Unset, GetProjectConversationsResponse404DataMessage]
         if isinstance(_message, Unset):
             message = UNSET
         else:
             message = GetProjectConversationsResponse404DataMessage(_message)
 
         get_project_conversations_response_404_data = cls(
             code=code,
             message=message,
         )
 
-        get_project_conversations_response_404_data.additional_properties = d
+        get_project_conversations_response_404_data.additional_properties = src_dict
         return get_project_conversations_response_404_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_conversations_response_500.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.get_project_conversations_response_500_data import GetProjectConversationsResponse500Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, GetProjectConversationsResponse500Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = GetProjectConversationsResponse500Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, GetProjectConversationsResponse500Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = GetProjectConversationsResponse500Data.from_dict(_data)
 
         get_project_conversations_response_500 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        get_project_conversations_response_500.additional_properties = d
+        get_project_conversations_response_500.additional_properties = src_dict
         return get_project_conversations_response_500
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_conversations_response_500_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, GetProjectConversationsResponse500DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = GetProjectConversationsResponse500DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         get_project_conversations_response_500_data = cls(
             code=code,
             message=message,
         )
 
-        get_project_conversations_response_500_data.additional_properties = d
+        get_project_conversations_response_500_data.additional_properties = src_dict
         return get_project_conversations_response_500_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_pages_response_200.py

```diff
@@ -43,35 +43,34 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.get_project_pages_response_200_data import GetProjectPagesResponse200Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, GetProjectPagesResponse200Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = GetProjectPagesResponse200Status(_status)
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, GetProjectPagesResponse200Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = GetProjectPagesResponse200Data.from_dict(_data)
 
         get_project_pages_response_200 = cls(
             status=status,
             data=data,
         )
 
-        get_project_pages_response_200.additional_properties = d
+        get_project_pages_response_200.additional_properties = src_dict
         return get_project_pages_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_pages_response_200_data.py

```diff
@@ -44,35 +44,34 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.get_project_pages_response_200_data_pages import GetProjectPagesResponse200DataPages
         from ..models.get_project_pages_response_200_data_project import GetProjectPagesResponse200DataProject
 
-        d = src_dict.copy()
-        _project = d.pop("project", UNSET)
+        _project = src_dict.get("project")
         project: Union[Unset, GetProjectPagesResponse200DataProject]
         if isinstance(_project, Unset):
             project = UNSET
         else:
             project = GetProjectPagesResponse200DataProject.from_dict(_project)
 
-        _pages = d.pop("pages", UNSET)
+        _pages = src_dict.get("pages")
         pages: Union[Unset, GetProjectPagesResponse200DataPages]
         if isinstance(_pages, Unset):
             pages = UNSET
         else:
             pages = GetProjectPagesResponse200DataPages.from_dict(_pages)
 
         get_project_pages_response_200_data = cls(
             project=project,
             pages=pages,
         )
 
-        get_project_pages_response_200_data.additional_properties = d
+        get_project_pages_response_200_data.additional_properties = src_dict
         return get_project_pages_response_200_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_pages_response_200_data_pages.py

```diff
@@ -2,15 +2,14 @@
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.get_project_pages_response_200_data_pages_data_item import GetProjectPagesResponse200DataPagesDataItem
-    from ..models.get_project_pages_response_200_data_pages_links import GetProjectPagesResponse200DataPagesLinks
 
 
 T = TypeVar("T", bound="GetProjectPagesResponse200DataPages")
 
 
 @attr.s(auto_attribs=True)
 class GetProjectPagesResponse200DataPages:
@@ -18,30 +17,28 @@
     Attributes:
         current_page (Union[Unset, int]): The current page number Example: 1.
         data (Union[Unset, List['GetProjectPagesResponse200DataPagesDataItem']]):
         first_page_url (Union[Unset, str]): The first page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         from_ (Union[Unset, int]): The first item number of the current page Example: 1.
         last_page (Union[Unset, int]): The last page number Example: 1.
         last_page_url (Union[Unset, str]): The last page url Example: https://app.customgpt.ai/api/v1/users?page=1.
-        links (Union[Unset, GetProjectPagesResponse200DataPagesLinks]):
         next_page_url (Union[Unset, str]): The next page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         path (Union[Unset, str]): The current page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         per_page (Union[Unset, int]): The number of items per page Example: 10.
         prev_page_url (Union[Unset, str]): The previous page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         to (Union[Unset, int]): The last item number of the current page Example: 1.
         total (Union[Unset, int]): The total number of items Example: 1.
     """
 
     current_page: Union[Unset, int] = UNSET
     data: Union[Unset, List["GetProjectPagesResponse200DataPagesDataItem"]] = UNSET
     first_page_url: Union[Unset, str] = UNSET
     from_: Union[Unset, int] = UNSET
     last_page: Union[Unset, int] = UNSET
     last_page_url: Union[Unset, str] = UNSET
-    links: Union[Unset, "GetProjectPagesResponse200DataPagesLinks"] = UNSET
     next_page_url: Union[Unset, str] = UNSET
     path: Union[Unset, str] = UNSET
     per_page: Union[Unset, int] = UNSET
     prev_page_url: Union[Unset, str] = UNSET
     to: Union[Unset, int] = UNSET
     total: Union[Unset, int] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
@@ -56,18 +53,14 @@
 
                 data.append(data_item)
 
         first_page_url = self.first_page_url
         from_ = self.from_
         last_page = self.last_page
         last_page_url = self.last_page_url
-        links: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.links, Unset):
-            links = self.links.to_dict()
-
         next_page_url = self.next_page_url
         path = self.path
         per_page = self.per_page
         prev_page_url = self.prev_page_url
         to = self.to
         total = self.total
 
@@ -83,16 +76,14 @@
             field_dict["first_page_url"] = first_page_url
         if from_ is not UNSET:
             field_dict["from"] = from_
         if last_page is not UNSET:
             field_dict["last_page"] = last_page
         if last_page_url is not UNSET:
             field_dict["last_page_url"] = last_page_url
-        if links is not UNSET:
-            field_dict["links"] = links
         if next_page_url is not UNSET:
             field_dict["next_page_url"] = next_page_url
         if path is not UNSET:
             field_dict["path"] = path
         if per_page is not UNSET:
             field_dict["per_page"] = per_page
         if prev_page_url is not UNSET:
@@ -105,70 +96,60 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.get_project_pages_response_200_data_pages_data_item import (
             GetProjectPagesResponse200DataPagesDataItem,
         )
-        from ..models.get_project_pages_response_200_data_pages_links import GetProjectPagesResponse200DataPagesLinks
 
-        d = src_dict.copy()
-        current_page = d.pop("current_page", UNSET)
+        current_page = src_dict.get("current_page")
 
         data = []
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         for data_item_data in _data or []:
             data_item = GetProjectPagesResponse200DataPagesDataItem.from_dict(data_item_data)
 
             data.append(data_item)
 
-        first_page_url = d.pop("first_page_url", UNSET)
-
-        from_ = d.pop("from", UNSET)
+        first_page_url = src_dict.get("first_page_url")
 
-        last_page = d.pop("last_page", UNSET)
+        from_ = src_dict.get("from")
 
-        last_page_url = d.pop("last_page_url", UNSET)
+        last_page = src_dict.get("last_page")
 
-        _links = d.pop("links", UNSET)
-        links: Union[Unset, GetProjectPagesResponse200DataPagesLinks]
-        if isinstance(_links, Unset):
-            links = UNSET
-        else:
-            links = GetProjectPagesResponse200DataPagesLinks.from_dict(_links)
+        last_page_url = src_dict.get("last_page_url")
 
-        next_page_url = d.pop("next_page_url", UNSET)
+        next_page_url = src_dict.get("next_page_url")
 
-        path = d.pop("path", UNSET)
+        path = src_dict.get("path")
 
-        per_page = d.pop("per_page", UNSET)
+        per_page = src_dict.get("per_page")
 
-        prev_page_url = d.pop("prev_page_url", UNSET)
+        prev_page_url = src_dict.get("prev_page_url")
 
-        to = d.pop("to", UNSET)
+        to = src_dict.get("to")
 
-        total = d.pop("total", UNSET)
+        total = src_dict.get("total")
 
         get_project_pages_response_200_data_pages = cls(
             current_page=current_page,
             data=data,
             first_page_url=first_page_url,
             from_=from_,
             last_page=last_page,
             last_page_url=last_page_url,
-            links=links,
             next_page_url=next_page_url,
             path=path,
             per_page=per_page,
             prev_page_url=prev_page_url,
             to=to,
             total=total,
         )
 
-        get_project_pages_response_200_data_pages.additional_properties = d
+        get_project_pages_response_200_data_pages.additional_properties = src_dict
         return get_project_pages_response_200_data_pages
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_pages_response_200_data_pages_data_item.py

```diff
@@ -1,21 +1,20 @@
 import datetime
-from io import BytesIO
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.get_project_pages_response_200_data_pages_data_item_crawl_status import (
     GetProjectPagesResponse200DataPagesDataItemCrawlStatus,
 )
 from ..models.get_project_pages_response_200_data_pages_data_item_index_status import (
     GetProjectPagesResponse200DataPagesDataItemIndexStatus,
 )
-from ..types import UNSET, File, FileJsonType, Unset
+from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="GetProjectPagesResponse200DataPagesDataItem")
 
 
 @attr.s(auto_attribs=True)
 class GetProjectPagesResponse200DataPagesDataItem:
     r"""
@@ -30,23 +29,23 @@
         crawl_status (Union[Unset, GetProjectPagesResponse200DataPagesDataItemCrawlStatus]): Crawl status of the page
             Default: GetProjectPagesResponse200DataPagesDataItemCrawlStatus.QUEUED. Example: queued.
         index_status (Union[Unset, GetProjectPagesResponse200DataPagesDataItemIndexStatus]): Index status of the page
             Default: GetProjectPagesResponse200DataPagesDataItemIndexStatus.QUEUED. Example: queued.
         is_file (Union[Unset, bool]): Whether the page is a file or not Example: True.
         is_file_kept (Union[Unset, bool]): Whether the file is kept after processing or not.\nNote: This is omitted in
             the response if the page is not a file Default: True. Example: True.
-        filename (Union[Unset, None, File]): Filename of the page.\nNote: This is omitted in the response if the page is
+        filename (Union[Unset, None, str]): Filename of the page.\nNote: This is omitted in the response if the page is
             not a file Example: file.pdf.
         filesize (Union[Unset, None, int]): Filesize of the page.\nNote: This is omitted in the response if the page is
             not a file Example: 100.
         created_at (Union[Unset, datetime.datetime]): Date and time when the page was created Example: 2021-01-01
             00:00:00.
         updated_at (Union[Unset, datetime.datetime]): Date and time when the page was updated Example: 2021-01-01
             00:00:00.
-        deleted_at (Union[Unset, datetime.datetime]): Date and time when the page was deleted Example: 2021-01-01
+        deleted_at (Union[Unset, None, datetime.datetime]): Date and time when the page was deleted Example: 2021-01-01
             00:00:00.
     """
 
     id: Union[Unset, int] = UNSET
     page_url: Union[Unset, str] = UNSET
     page_url_hash: Union[Unset, str] = UNSET
     project_id: Union[Unset, int] = UNSET
@@ -55,19 +54,19 @@
         Unset, GetProjectPagesResponse200DataPagesDataItemCrawlStatus
     ] = GetProjectPagesResponse200DataPagesDataItemCrawlStatus.QUEUED
     index_status: Union[
         Unset, GetProjectPagesResponse200DataPagesDataItemIndexStatus
     ] = GetProjectPagesResponse200DataPagesDataItemIndexStatus.QUEUED
     is_file: Union[Unset, bool] = False
     is_file_kept: Union[Unset, bool] = True
-    filename: Union[Unset, None, File] = UNSET
+    filename: Union[Unset, None, str] = UNSET
     filesize: Union[Unset, None, int] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
-    deleted_at: Union[Unset, datetime.datetime] = UNSET
+    deleted_at: Union[Unset, None, datetime.datetime] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
         page_url = self.page_url
         page_url_hash = self.page_url_hash
         project_id = self.project_id
@@ -78,30 +77,27 @@
 
         index_status: Union[Unset, str] = UNSET
         if not isinstance(self.index_status, Unset):
             index_status = self.index_status.value
 
         is_file = self.is_file
         is_file_kept = self.is_file_kept
-        filename: Union[Unset, None, FileJsonType] = UNSET
-        if not isinstance(self.filename, Unset):
-            filename = self.filename.to_tuple() if self.filename else None
-
+        filename = self.filename
         filesize = self.filesize
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
 
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
 
-        deleted_at: Union[Unset, str] = UNSET
+        deleted_at: Union[Unset, None, str] = UNSET
         if not isinstance(self.deleted_at, Unset):
-            deleted_at = self.deleted_at.isoformat()
+            deleted_at = self.deleted_at.isoformat() if self.deleted_at else None
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if id is not UNSET:
             field_dict["id"] = id
         if page_url is not UNSET:
@@ -131,71 +127,65 @@
         if deleted_at is not UNSET:
             field_dict["deleted_at"] = deleted_at
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        id = d.pop("id", UNSET)
+        id = src_dict.get("id")
 
-        page_url = d.pop("page_url", UNSET)
+        page_url = src_dict.get("page_url")
 
-        page_url_hash = d.pop("page_url_hash", UNSET)
+        page_url_hash = src_dict.get("page_url_hash")
 
-        project_id = d.pop("project_id", UNSET)
+        project_id = src_dict.get("project_id")
 
-        s3_path = d.pop("s3_path", UNSET)
+        s3_path = src_dict.get("s3_path")
 
-        _crawl_status = d.pop("crawl_status", UNSET)
+        _crawl_status = src_dict.get("crawl_status")
         crawl_status: Union[Unset, GetProjectPagesResponse200DataPagesDataItemCrawlStatus]
         if isinstance(_crawl_status, Unset):
             crawl_status = UNSET
         else:
             crawl_status = GetProjectPagesResponse200DataPagesDataItemCrawlStatus(_crawl_status)
 
-        _index_status = d.pop("index_status", UNSET)
+        _index_status = src_dict.get("index_status")
         index_status: Union[Unset, GetProjectPagesResponse200DataPagesDataItemIndexStatus]
         if isinstance(_index_status, Unset):
             index_status = UNSET
         else:
             index_status = GetProjectPagesResponse200DataPagesDataItemIndexStatus(_index_status)
 
-        is_file = d.pop("is_file", UNSET)
+        is_file = src_dict.get("is_file")
 
-        is_file_kept = d.pop("is_file_kept", UNSET)
+        is_file_kept = src_dict.get("is_file_kept")
 
-        _filename = d.pop("filename", UNSET)
-        filename: Union[Unset, None, File]
-        if _filename is None:
-            filename = None
-        elif isinstance(_filename, Unset):
-            filename = UNSET
-        else:
-            filename = File(payload=BytesIO(_filename))
+        filename = src_dict.get("filename")
 
-        filesize = d.pop("filesize", UNSET)
+        filesize = src_dict.get("filesize")
 
-        _created_at = d.pop("created_at", UNSET)
+        _created_at = src_dict.get("created_at")
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
-        _updated_at = d.pop("updated_at", UNSET)
+        _updated_at = src_dict.get("updated_at")
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
-        _deleted_at = d.pop("deleted_at", UNSET)
-        deleted_at: Union[Unset, datetime.datetime]
-        if isinstance(_deleted_at, Unset):
+        _deleted_at = src_dict.get("deleted_at")
+        deleted_at: Union[Unset, None, datetime.datetime]
+        if _deleted_at is None:
+            deleted_at = None
+        elif isinstance(_deleted_at, Unset):
             deleted_at = UNSET
         else:
             deleted_at = isoparse(_deleted_at)
 
         get_project_pages_response_200_data_pages_data_item = cls(
             id=id,
             page_url=page_url,
@@ -209,15 +199,15 @@
             filename=filename,
             filesize=filesize,
             created_at=created_at,
             updated_at=updated_at,
             deleted_at=deleted_at,
         )
 
-        get_project_pages_response_200_data_pages_data_item.additional_properties = d
+        get_project_pages_response_200_data_pages_data_item.additional_properties = src_dict
         return get_project_pages_response_200_data_pages_data_item
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_pages_response_200_data_project.py

```diff
@@ -111,64 +111,63 @@
         if live_chat_code is not UNSET:
             field_dict["live_chat_code"] = live_chat_code
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        id = d.pop("id", UNSET)
+        id = src_dict.get("id")
 
-        project_name = d.pop("project_name", UNSET)
+        project_name = src_dict.get("project_name")
 
-        sitemap_path = d.pop("sitemap_path", UNSET)
+        sitemap_path = src_dict.get("sitemap_path")
 
-        is_chat_active = d.pop("is_chat_active", UNSET)
+        is_chat_active = src_dict.get("is_chat_active")
 
-        user_id = d.pop("user_id", UNSET)
+        user_id = src_dict.get("user_id")
 
-        _created_at = d.pop("created_at", UNSET)
+        _created_at = src_dict.get("created_at")
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
-        _updated_at = d.pop("updated_at", UNSET)
+        _updated_at = src_dict.get("updated_at")
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
-        _deleted_at = d.pop("deleted_at", UNSET)
+        _deleted_at = src_dict.get("deleted_at")
         deleted_at: Union[Unset, None, datetime.datetime]
         if _deleted_at is None:
             deleted_at = None
         elif isinstance(_deleted_at, Unset):
             deleted_at = UNSET
         else:
             deleted_at = isoparse(_deleted_at)
 
-        _type = d.pop("type", UNSET)
+        _type = src_dict.get("type")
         type: Union[Unset, GetProjectPagesResponse200DataProjectType]
         if isinstance(_type, Unset):
             type = UNSET
         else:
             type = GetProjectPagesResponse200DataProjectType(_type)
 
-        is_shared = d.pop("is_shared", UNSET)
+        is_shared = src_dict.get("is_shared")
 
-        shareable_slug = d.pop("shareable_slug", UNSET)
+        shareable_slug = src_dict.get("shareable_slug")
 
-        shareable_link = d.pop("shareable_link", UNSET)
+        shareable_link = src_dict.get("shareable_link")
 
-        embed_code = d.pop("embed_code", UNSET)
+        embed_code = src_dict.get("embed_code")
 
-        live_chat_code = d.pop("live_chat_code", UNSET)
+        live_chat_code = src_dict.get("live_chat_code")
 
         get_project_pages_response_200_data_project = cls(
             id=id,
             project_name=project_name,
             sitemap_path=sitemap_path,
             is_chat_active=is_chat_active,
             user_id=user_id,
@@ -179,15 +178,15 @@
             is_shared=is_shared,
             shareable_slug=shareable_slug,
             shareable_link=shareable_link,
             embed_code=embed_code,
             live_chat_code=live_chat_code,
         )
 
-        get_project_pages_response_200_data_project.additional_properties = d
+        get_project_pages_response_200_data_project.additional_properties = src_dict
         return get_project_pages_response_200_data_project
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_pages_response_401.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.get_project_pages_response_401_data import GetProjectPagesResponse401Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, GetProjectPagesResponse401Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = GetProjectPagesResponse401Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, GetProjectPagesResponse401Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = GetProjectPagesResponse401Data.from_dict(_data)
 
         get_project_pages_response_401 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        get_project_pages_response_401.additional_properties = d
+        get_project_pages_response_401.additional_properties = src_dict
         return get_project_pages_response_401
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_pages_response_401_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, GetProjectPagesResponse401DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = GetProjectPagesResponse401DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         get_project_pages_response_401_data = cls(
             code=code,
             message=message,
         )
 
-        get_project_pages_response_401_data.additional_properties = d
+        get_project_pages_response_401_data.additional_properties = src_dict
         return get_project_pages_response_401_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_pages_response_404.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.get_project_pages_response_404_data import GetProjectPagesResponse404Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, GetProjectPagesResponse404Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = GetProjectPagesResponse404Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, GetProjectPagesResponse404Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = GetProjectPagesResponse404Data.from_dict(_data)
 
         get_project_pages_response_404 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        get_project_pages_response_404.additional_properties = d
+        get_project_pages_response_404.additional_properties = src_dict
         return get_project_pages_response_404
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_pages_response_404_data.py

```diff
@@ -39,35 +39,34 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, GetProjectPagesResponse404DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = GetProjectPagesResponse404DataCode(_code)
 
-        _message = d.pop("message", UNSET)
+        _message = src_dict.get("message")
         message: Union[Unset, GetProjectPagesResponse404DataMessage]
         if isinstance(_message, Unset):
             message = UNSET
         else:
             message = GetProjectPagesResponse404DataMessage(_message)
 
         get_project_pages_response_404_data = cls(
             code=code,
             message=message,
         )
 
-        get_project_pages_response_404_data.additional_properties = d
+        get_project_pages_response_404_data.additional_properties = src_dict
         return get_project_pages_response_404_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_pages_response_500.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.get_project_pages_response_500_data import GetProjectPagesResponse500Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, GetProjectPagesResponse500Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = GetProjectPagesResponse500Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, GetProjectPagesResponse500Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = GetProjectPagesResponse500Data.from_dict(_data)
 
         get_project_pages_response_500 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        get_project_pages_response_500.additional_properties = d
+        get_project_pages_response_500.additional_properties = src_dict
         return get_project_pages_response_500
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_pages_response_500_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, GetProjectPagesResponse500DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = GetProjectPagesResponse500DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         get_project_pages_response_500_data = cls(
             code=code,
             message=message,
         )
 
-        get_project_pages_response_500_data.additional_properties = d
+        get_project_pages_response_500_data.additional_properties = src_dict
         return get_project_pages_response_500_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_response_200.py

```diff
@@ -43,35 +43,34 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.get_project_response_200_data import GetProjectResponse200Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, GetProjectResponse200Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = GetProjectResponse200Status(_status)
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, GetProjectResponse200Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = GetProjectResponse200Data.from_dict(_data)
 
         get_project_response_200 = cls(
             status=status,
             data=data,
         )
 
-        get_project_response_200.additional_properties = d
+        get_project_response_200.additional_properties = src_dict
         return get_project_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_response_200_data.py

```diff
@@ -111,64 +111,63 @@
         if live_chat_code is not UNSET:
             field_dict["live_chat_code"] = live_chat_code
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        id = d.pop("id", UNSET)
+        id = src_dict.get("id")
 
-        project_name = d.pop("project_name", UNSET)
+        project_name = src_dict.get("project_name")
 
-        sitemap_path = d.pop("sitemap_path", UNSET)
+        sitemap_path = src_dict.get("sitemap_path")
 
-        is_chat_active = d.pop("is_chat_active", UNSET)
+        is_chat_active = src_dict.get("is_chat_active")
 
-        user_id = d.pop("user_id", UNSET)
+        user_id = src_dict.get("user_id")
 
-        _created_at = d.pop("created_at", UNSET)
+        _created_at = src_dict.get("created_at")
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
-        _updated_at = d.pop("updated_at", UNSET)
+        _updated_at = src_dict.get("updated_at")
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
-        _deleted_at = d.pop("deleted_at", UNSET)
+        _deleted_at = src_dict.get("deleted_at")
         deleted_at: Union[Unset, None, datetime.datetime]
         if _deleted_at is None:
             deleted_at = None
         elif isinstance(_deleted_at, Unset):
             deleted_at = UNSET
         else:
             deleted_at = isoparse(_deleted_at)
 
-        _type = d.pop("type", UNSET)
+        _type = src_dict.get("type")
         type: Union[Unset, GetProjectResponse200DataType]
         if isinstance(_type, Unset):
             type = UNSET
         else:
             type = GetProjectResponse200DataType(_type)
 
-        is_shared = d.pop("is_shared", UNSET)
+        is_shared = src_dict.get("is_shared")
 
-        shareable_slug = d.pop("shareable_slug", UNSET)
+        shareable_slug = src_dict.get("shareable_slug")
 
-        shareable_link = d.pop("shareable_link", UNSET)
+        shareable_link = src_dict.get("shareable_link")
 
-        embed_code = d.pop("embed_code", UNSET)
+        embed_code = src_dict.get("embed_code")
 
-        live_chat_code = d.pop("live_chat_code", UNSET)
+        live_chat_code = src_dict.get("live_chat_code")
 
         get_project_response_200_data = cls(
             id=id,
             project_name=project_name,
             sitemap_path=sitemap_path,
             is_chat_active=is_chat_active,
             user_id=user_id,
@@ -179,15 +178,15 @@
             is_shared=is_shared,
             shareable_slug=shareable_slug,
             shareable_link=shareable_link,
             embed_code=embed_code,
             live_chat_code=live_chat_code,
         )
 
-        get_project_response_200_data.additional_properties = d
+        get_project_response_200_data.additional_properties = src_dict
         return get_project_response_200_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_response_401.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.get_project_response_401_data import GetProjectResponse401Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, GetProjectResponse401Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = GetProjectResponse401Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, GetProjectResponse401Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = GetProjectResponse401Data.from_dict(_data)
 
         get_project_response_401 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        get_project_response_401.additional_properties = d
+        get_project_response_401.additional_properties = src_dict
         return get_project_response_401
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_response_401_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, GetProjectResponse401DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = GetProjectResponse401DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         get_project_response_401_data = cls(
             code=code,
             message=message,
         )
 
-        get_project_response_401_data.additional_properties = d
+        get_project_response_401_data.additional_properties = src_dict
         return get_project_response_401_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_response_404.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.get_project_response_404_data import GetProjectResponse404Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, GetProjectResponse404Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = GetProjectResponse404Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, GetProjectResponse404Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = GetProjectResponse404Data.from_dict(_data)
 
         get_project_response_404 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        get_project_response_404.additional_properties = d
+        get_project_response_404.additional_properties = src_dict
         return get_project_response_404
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_response_404_data.py

```diff
@@ -38,35 +38,34 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, GetProjectResponse404DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = GetProjectResponse404DataCode(_code)
 
-        _message = d.pop("message", UNSET)
+        _message = src_dict.get("message")
         message: Union[Unset, GetProjectResponse404DataMessage]
         if isinstance(_message, Unset):
             message = UNSET
         else:
             message = GetProjectResponse404DataMessage(_message)
 
         get_project_response_404_data = cls(
             code=code,
             message=message,
         )
 
-        get_project_response_404_data.additional_properties = d
+        get_project_response_404_data.additional_properties = src_dict
         return get_project_response_404_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_response_500.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.get_project_response_500_data import GetProjectResponse500Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, GetProjectResponse500Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = GetProjectResponse500Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, GetProjectResponse500Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = GetProjectResponse500Data.from_dict(_data)
 
         get_project_response_500 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        get_project_response_500.additional_properties = d
+        get_project_response_500.additional_properties = src_dict
         return get_project_response_500
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_response_500_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, GetProjectResponse500DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = GetProjectResponse500DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         get_project_response_500_data = cls(
             code=code,
             message=message,
         )
 
-        get_project_response_500_data.additional_properties = d
+        get_project_response_500_data.additional_properties = src_dict
         return get_project_response_500_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_settings_response_200.py

```diff
@@ -43,35 +43,34 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.get_project_settings_response_200_data import GetProjectSettingsResponse200Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, GetProjectSettingsResponse200Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = GetProjectSettingsResponse200Status(_status)
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, GetProjectSettingsResponse200Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = GetProjectSettingsResponse200Data.from_dict(_data)
 
         get_project_settings_response_200 = cls(
             status=status,
             data=data,
         )
 
-        get_project_settings_response_200.additional_properties = d
+        get_project_settings_response_200.additional_properties = src_dict
         return get_project_settings_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_settings_response_200_data.py

```diff
@@ -63,42 +63,41 @@
         if chatbot_msg_lang is not UNSET:
             field_dict["chatbot_msg_lang"] = chatbot_msg_lang
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        chatbot_avatar = d.pop("chatbot_avatar", UNSET)
+        chatbot_avatar = src_dict.get("chatbot_avatar")
 
-        chatbot_background = d.pop("chatbot_background", UNSET)
+        chatbot_background = src_dict.get("chatbot_background")
 
-        default_prompt = d.pop("default_prompt", UNSET)
+        default_prompt = src_dict.get("default_prompt")
 
-        example_questions = cast(List[str], d.pop("example_questions", UNSET))
+        example_questions = cast(List[str], src_dict.get("example_questions"))
 
-        _response_source = d.pop("response_source", UNSET)
+        _response_source = src_dict.get("response_source")
         response_source: Union[Unset, GetProjectSettingsResponse200DataResponseSource]
         if isinstance(_response_source, Unset):
             response_source = UNSET
         else:
             response_source = GetProjectSettingsResponse200DataResponseSource(_response_source)
 
-        chatbot_msg_lang = d.pop("chatbot_msg_lang", UNSET)
+        chatbot_msg_lang = src_dict.get("chatbot_msg_lang")
 
         get_project_settings_response_200_data = cls(
             chatbot_avatar=chatbot_avatar,
             chatbot_background=chatbot_background,
             default_prompt=default_prompt,
             example_questions=example_questions,
             response_source=response_source,
             chatbot_msg_lang=chatbot_msg_lang,
         )
 
-        get_project_settings_response_200_data.additional_properties = d
+        get_project_settings_response_200_data.additional_properties = src_dict
         return get_project_settings_response_200_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_settings_response_401.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.get_project_settings_response_401_data import GetProjectSettingsResponse401Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, GetProjectSettingsResponse401Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = GetProjectSettingsResponse401Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, GetProjectSettingsResponse401Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = GetProjectSettingsResponse401Data.from_dict(_data)
 
         get_project_settings_response_401 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        get_project_settings_response_401.additional_properties = d
+        get_project_settings_response_401.additional_properties = src_dict
         return get_project_settings_response_401
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_settings_response_401_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, GetProjectSettingsResponse401DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = GetProjectSettingsResponse401DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         get_project_settings_response_401_data = cls(
             code=code,
             message=message,
         )
 
-        get_project_settings_response_401_data.additional_properties = d
+        get_project_settings_response_401_data.additional_properties = src_dict
         return get_project_settings_response_401_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_settings_response_404.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.get_project_settings_response_404_data import GetProjectSettingsResponse404Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, GetProjectSettingsResponse404Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = GetProjectSettingsResponse404Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, GetProjectSettingsResponse404Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = GetProjectSettingsResponse404Data.from_dict(_data)
 
         get_project_settings_response_404 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        get_project_settings_response_404.additional_properties = d
+        get_project_settings_response_404.additional_properties = src_dict
         return get_project_settings_response_404
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_settings_response_404_data.py

```diff
@@ -39,35 +39,34 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, GetProjectSettingsResponse404DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = GetProjectSettingsResponse404DataCode(_code)
 
-        _message = d.pop("message", UNSET)
+        _message = src_dict.get("message")
         message: Union[Unset, GetProjectSettingsResponse404DataMessage]
         if isinstance(_message, Unset):
             message = UNSET
         else:
             message = GetProjectSettingsResponse404DataMessage(_message)
 
         get_project_settings_response_404_data = cls(
             code=code,
             message=message,
         )
 
-        get_project_settings_response_404_data.additional_properties = d
+        get_project_settings_response_404_data.additional_properties = src_dict
         return get_project_settings_response_404_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_settings_response_500.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.get_project_settings_response_500_data import GetProjectSettingsResponse500Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, GetProjectSettingsResponse500Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = GetProjectSettingsResponse500Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, GetProjectSettingsResponse500Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = GetProjectSettingsResponse500Data.from_dict(_data)
 
         get_project_settings_response_500 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        get_project_settings_response_500.additional_properties = d
+        get_project_settings_response_500.additional_properties = src_dict
         return get_project_settings_response_500
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_project_settings_response_500_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, GetProjectSettingsResponse500DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = GetProjectSettingsResponse500DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         get_project_settings_response_500_data = cls(
             code=code,
             message=message,
         )
 
-        get_project_settings_response_500_data.additional_properties = d
+        get_project_settings_response_500_data.additional_properties = src_dict
         return get_project_settings_response_500_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_user_profile_response_200.py

```diff
@@ -43,35 +43,34 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.get_user_profile_response_200_data import GetUserProfileResponse200Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, GetUserProfileResponse200Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = GetUserProfileResponse200Status(_status)
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, GetUserProfileResponse200Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = GetUserProfileResponse200Data.from_dict(_data)
 
         get_user_profile_response_200 = cls(
             status=status,
             data=data,
         )
 
-        get_user_profile_response_200.additional_properties = d
+        get_user_profile_response_200.additional_properties = src_dict
         return get_user_profile_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_user_profile_response_200_data.py

```diff
@@ -59,31 +59,30 @@
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _created_at = d.pop("created_at", UNSET)
+        _created_at = src_dict.get("created_at")
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
-        email = d.pop("email", UNSET)
+        email = src_dict.get("email")
 
-        id = d.pop("id", UNSET)
+        id = src_dict.get("id")
 
-        name = d.pop("name", UNSET)
+        name = src_dict.get("name")
 
-        profile_photo_url = d.pop("profile_photo_url", UNSET)
+        profile_photo_url = src_dict.get("profile_photo_url")
 
-        _updated_at = d.pop("updated_at", UNSET)
+        _updated_at = src_dict.get("updated_at")
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         get_user_profile_response_200_data = cls(
@@ -91,15 +90,15 @@
             email=email,
             id=id,
             name=name,
             profile_photo_url=profile_photo_url,
             updated_at=updated_at,
         )
 
-        get_user_profile_response_200_data.additional_properties = d
+        get_user_profile_response_200_data.additional_properties = src_dict
         return get_user_profile_response_200_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_user_profile_response_401.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.get_user_profile_response_401_data import GetUserProfileResponse401Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, GetUserProfileResponse401Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = GetUserProfileResponse401Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, GetUserProfileResponse401Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = GetUserProfileResponse401Data.from_dict(_data)
 
         get_user_profile_response_401 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        get_user_profile_response_401.additional_properties = d
+        get_user_profile_response_401.additional_properties = src_dict
         return get_user_profile_response_401
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_user_profile_response_401_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, GetUserProfileResponse401DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = GetUserProfileResponse401DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         get_user_profile_response_401_data = cls(
             code=code,
             message=message,
         )
 
-        get_user_profile_response_401_data.additional_properties = d
+        get_user_profile_response_401_data.additional_properties = src_dict
         return get_user_profile_response_401_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_user_profile_response_500.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.get_user_profile_response_500_data import GetUserProfileResponse500Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, GetUserProfileResponse500Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = GetUserProfileResponse500Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, GetUserProfileResponse500Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = GetUserProfileResponse500Data.from_dict(_data)
 
         get_user_profile_response_500 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        get_user_profile_response_500.additional_properties = d
+        get_user_profile_response_500.additional_properties = src_dict
         return get_user_profile_response_500
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/get_user_profile_response_500_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, GetUserProfileResponse500DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = GetUserProfileResponse500DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         get_user_profile_response_500_data = cls(
             code=code,
             message=message,
         )
 
-        get_user_profile_response_500_data.additional_properties = d
+        get_user_profile_response_500_data.additional_properties = src_dict
         return get_user_profile_response_500_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/list_projects_response_200.py

```diff
@@ -43,35 +43,34 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.list_projects_response_200_data import ListProjectsResponse200Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, ListProjectsResponse200Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = ListProjectsResponse200Status(_status)
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, ListProjectsResponse200Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = ListProjectsResponse200Data.from_dict(_data)
 
         list_projects_response_200 = cls(
             status=status,
             data=data,
         )
 
-        list_projects_response_200.additional_properties = d
+        list_projects_response_200.additional_properties = src_dict
         return list_projects_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/list_projects_response_200_data.py

```diff
@@ -2,15 +2,14 @@
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
     from ..models.list_projects_response_200_data_data_item import ListProjectsResponse200DataDataItem
-    from ..models.list_projects_response_200_data_links import ListProjectsResponse200DataLinks
 
 
 T = TypeVar("T", bound="ListProjectsResponse200Data")
 
 
 @attr.s(auto_attribs=True)
 class ListProjectsResponse200Data:
@@ -18,30 +17,28 @@
     Attributes:
         current_page (Union[Unset, int]): The current page number Example: 1.
         data (Union[Unset, List['ListProjectsResponse200DataDataItem']]):
         first_page_url (Union[Unset, str]): The first page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         from_ (Union[Unset, int]): The first item number of the current page Example: 1.
         last_page (Union[Unset, int]): The last page number Example: 1.
         last_page_url (Union[Unset, str]): The last page url Example: https://app.customgpt.ai/api/v1/users?page=1.
-        links (Union[Unset, ListProjectsResponse200DataLinks]):
         next_page_url (Union[Unset, str]): The next page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         path (Union[Unset, str]): The current page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         per_page (Union[Unset, int]): The number of items per page Example: 10.
         prev_page_url (Union[Unset, str]): The previous page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         to (Union[Unset, int]): The last item number of the current page Example: 1.
         total (Union[Unset, int]): The total number of items Example: 1.
     """
 
     current_page: Union[Unset, int] = UNSET
     data: Union[Unset, List["ListProjectsResponse200DataDataItem"]] = UNSET
     first_page_url: Union[Unset, str] = UNSET
     from_: Union[Unset, int] = UNSET
     last_page: Union[Unset, int] = UNSET
     last_page_url: Union[Unset, str] = UNSET
-    links: Union[Unset, "ListProjectsResponse200DataLinks"] = UNSET
     next_page_url: Union[Unset, str] = UNSET
     path: Union[Unset, str] = UNSET
     per_page: Union[Unset, int] = UNSET
     prev_page_url: Union[Unset, str] = UNSET
     to: Union[Unset, int] = UNSET
     total: Union[Unset, int] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
@@ -56,18 +53,14 @@
 
                 data.append(data_item)
 
         first_page_url = self.first_page_url
         from_ = self.from_
         last_page = self.last_page
         last_page_url = self.last_page_url
-        links: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.links, Unset):
-            links = self.links.to_dict()
-
         next_page_url = self.next_page_url
         path = self.path
         per_page = self.per_page
         prev_page_url = self.prev_page_url
         to = self.to
         total = self.total
 
@@ -83,16 +76,14 @@
             field_dict["first_page_url"] = first_page_url
         if from_ is not UNSET:
             field_dict["from"] = from_
         if last_page is not UNSET:
             field_dict["last_page"] = last_page
         if last_page_url is not UNSET:
             field_dict["last_page_url"] = last_page_url
-        if links is not UNSET:
-            field_dict["links"] = links
         if next_page_url is not UNSET:
             field_dict["next_page_url"] = next_page_url
         if path is not UNSET:
             field_dict["path"] = path
         if per_page is not UNSET:
             field_dict["per_page"] = per_page
         if prev_page_url is not UNSET:
@@ -103,70 +94,60 @@
             field_dict["total"] = total
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.list_projects_response_200_data_data_item import ListProjectsResponse200DataDataItem
-        from ..models.list_projects_response_200_data_links import ListProjectsResponse200DataLinks
 
-        d = src_dict.copy()
-        current_page = d.pop("current_page", UNSET)
+        current_page = src_dict.get("current_page")
 
         data = []
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         for data_item_data in _data or []:
             data_item = ListProjectsResponse200DataDataItem.from_dict(data_item_data)
 
             data.append(data_item)
 
-        first_page_url = d.pop("first_page_url", UNSET)
-
-        from_ = d.pop("from", UNSET)
+        first_page_url = src_dict.get("first_page_url")
 
-        last_page = d.pop("last_page", UNSET)
+        from_ = src_dict.get("from")
 
-        last_page_url = d.pop("last_page_url", UNSET)
+        last_page = src_dict.get("last_page")
 
-        _links = d.pop("links", UNSET)
-        links: Union[Unset, ListProjectsResponse200DataLinks]
-        if isinstance(_links, Unset):
-            links = UNSET
-        else:
-            links = ListProjectsResponse200DataLinks.from_dict(_links)
+        last_page_url = src_dict.get("last_page_url")
 
-        next_page_url = d.pop("next_page_url", UNSET)
+        next_page_url = src_dict.get("next_page_url")
 
-        path = d.pop("path", UNSET)
+        path = src_dict.get("path")
 
-        per_page = d.pop("per_page", UNSET)
+        per_page = src_dict.get("per_page")
 
-        prev_page_url = d.pop("prev_page_url", UNSET)
+        prev_page_url = src_dict.get("prev_page_url")
 
-        to = d.pop("to", UNSET)
+        to = src_dict.get("to")
 
-        total = d.pop("total", UNSET)
+        total = src_dict.get("total")
 
         list_projects_response_200_data = cls(
             current_page=current_page,
             data=data,
             first_page_url=first_page_url,
             from_=from_,
             last_page=last_page,
             last_page_url=last_page_url,
-            links=links,
             next_page_url=next_page_url,
             path=path,
             per_page=per_page,
             prev_page_url=prev_page_url,
             to=to,
             total=total,
         )
 
-        list_projects_response_200_data.additional_properties = d
+        list_projects_response_200_data.additional_properties = src_dict
         return list_projects_response_200_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/list_projects_response_200_data_data_item.py

```diff
@@ -111,64 +111,63 @@
         if live_chat_code is not UNSET:
             field_dict["live_chat_code"] = live_chat_code
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        id = d.pop("id", UNSET)
+        id = src_dict.get("id")
 
-        project_name = d.pop("project_name", UNSET)
+        project_name = src_dict.get("project_name")
 
-        sitemap_path = d.pop("sitemap_path", UNSET)
+        sitemap_path = src_dict.get("sitemap_path")
 
-        is_chat_active = d.pop("is_chat_active", UNSET)
+        is_chat_active = src_dict.get("is_chat_active")
 
-        user_id = d.pop("user_id", UNSET)
+        user_id = src_dict.get("user_id")
 
-        _created_at = d.pop("created_at", UNSET)
+        _created_at = src_dict.get("created_at")
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
-        _updated_at = d.pop("updated_at", UNSET)
+        _updated_at = src_dict.get("updated_at")
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
-        _deleted_at = d.pop("deleted_at", UNSET)
+        _deleted_at = src_dict.get("deleted_at")
         deleted_at: Union[Unset, None, datetime.datetime]
         if _deleted_at is None:
             deleted_at = None
         elif isinstance(_deleted_at, Unset):
             deleted_at = UNSET
         else:
             deleted_at = isoparse(_deleted_at)
 
-        _type = d.pop("type", UNSET)
+        _type = src_dict.get("type")
         type: Union[Unset, ListProjectsResponse200DataDataItemType]
         if isinstance(_type, Unset):
             type = UNSET
         else:
             type = ListProjectsResponse200DataDataItemType(_type)
 
-        is_shared = d.pop("is_shared", UNSET)
+        is_shared = src_dict.get("is_shared")
 
-        shareable_slug = d.pop("shareable_slug", UNSET)
+        shareable_slug = src_dict.get("shareable_slug")
 
-        shareable_link = d.pop("shareable_link", UNSET)
+        shareable_link = src_dict.get("shareable_link")
 
-        embed_code = d.pop("embed_code", UNSET)
+        embed_code = src_dict.get("embed_code")
 
-        live_chat_code = d.pop("live_chat_code", UNSET)
+        live_chat_code = src_dict.get("live_chat_code")
 
         list_projects_response_200_data_data_item = cls(
             id=id,
             project_name=project_name,
             sitemap_path=sitemap_path,
             is_chat_active=is_chat_active,
             user_id=user_id,
@@ -179,15 +178,15 @@
             is_shared=is_shared,
             shareable_slug=shareable_slug,
             shareable_link=shareable_link,
             embed_code=embed_code,
             live_chat_code=live_chat_code,
         )
 
-        list_projects_response_200_data_data_item.additional_properties = d
+        list_projects_response_200_data_data_item.additional_properties = src_dict
         return list_projects_response_200_data_data_item
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/list_projects_response_401.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.list_projects_response_401_data import ListProjectsResponse401Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, ListProjectsResponse401Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = ListProjectsResponse401Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, ListProjectsResponse401Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = ListProjectsResponse401Data.from_dict(_data)
 
         list_projects_response_401 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        list_projects_response_401.additional_properties = d
+        list_projects_response_401.additional_properties = src_dict
         return list_projects_response_401
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/list_projects_response_401_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, ListProjectsResponse401DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = ListProjectsResponse401DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         list_projects_response_401_data = cls(
             code=code,
             message=message,
         )
 
-        list_projects_response_401_data.additional_properties = d
+        list_projects_response_401_data.additional_properties = src_dict
         return list_projects_response_401_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/list_projects_response_500.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.list_projects_response_500_data import ListProjectsResponse500Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, ListProjectsResponse500Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = ListProjectsResponse500Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, ListProjectsResponse500Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = ListProjectsResponse500Data.from_dict(_data)
 
         list_projects_response_500 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        list_projects_response_500.additional_properties = d
+        list_projects_response_500.additional_properties = src_dict
         return list_projects_response_500
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/list_projects_response_500_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, ListProjectsResponse500DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = ListProjectsResponse500DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         list_projects_response_500_data = cls(
             code=code,
             message=message,
         )
 
-        list_projects_response_500_data.additional_properties = d
+        list_projects_response_500_data.additional_properties = src_dict
         return list_projects_response_500_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/messages_response_200.py

```diff
@@ -2,94 +2,75 @@
 
 import attr
 
 from ..models.messages_response_200_status import MessagesResponse200Status
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.messages_response_200_conversation import MessagesResponse200Conversation
-    from ..models.messages_response_200_messages import MessagesResponse200Messages
+    from ..models.messages_response_200_data import MessagesResponse200Data
 
 
 T = TypeVar("T", bound="MessagesResponse200")
 
 
 @attr.s(auto_attribs=True)
 class MessagesResponse200:
     """
     Attributes:
         status (Union[Unset, MessagesResponse200Status]): The status of the response Example: success.
-        conversation (Union[Unset, MessagesResponse200Conversation]):
-        messages (Union[Unset, MessagesResponse200Messages]):
+        data (Union[Unset, MessagesResponse200Data]):
     """
 
     status: Union[Unset, MessagesResponse200Status] = UNSET
-    conversation: Union[Unset, "MessagesResponse200Conversation"] = UNSET
-    messages: Union[Unset, "MessagesResponse200Messages"] = UNSET
+    data: Union[Unset, "MessagesResponse200Data"] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         status: Union[Unset, str] = UNSET
         if not isinstance(self.status, Unset):
             status = self.status.value
 
-        conversation: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.conversation, Unset):
-            conversation = self.conversation.to_dict()
-
-        messages: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.messages, Unset):
-            messages = self.messages.to_dict()
+        data: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.data, Unset):
+            data = self.data.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if status is not UNSET:
             field_dict["status"] = status
-        if conversation is not UNSET:
-            field_dict["conversation"] = conversation
-        if messages is not UNSET:
-            field_dict["messages"] = messages
+        if data is not UNSET:
+            field_dict["data"] = data
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.messages_response_200_conversation import MessagesResponse200Conversation
-        from ..models.messages_response_200_messages import MessagesResponse200Messages
+        from ..models.messages_response_200_data import MessagesResponse200Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, MessagesResponse200Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = MessagesResponse200Status(_status)
 
-        _conversation = d.pop("conversation", UNSET)
-        conversation: Union[Unset, MessagesResponse200Conversation]
-        if isinstance(_conversation, Unset):
-            conversation = UNSET
+        _data = src_dict.get("data")
+        data: Union[Unset, MessagesResponse200Data]
+        if isinstance(_data, Unset):
+            data = UNSET
         else:
-            conversation = MessagesResponse200Conversation.from_dict(_conversation)
-
-        _messages = d.pop("messages", UNSET)
-        messages: Union[Unset, MessagesResponse200Messages]
-        if isinstance(_messages, Unset):
-            messages = UNSET
-        else:
-            messages = MessagesResponse200Messages.from_dict(_messages)
+            data = MessagesResponse200Data.from_dict(_data)
 
         messages_response_200 = cls(
             status=status,
-            conversation=conversation,
-            messages=messages,
+            data=data,
         )
 
-        messages_response_200.additional_properties = d
+        messages_response_200.additional_properties = src_dict
         return messages_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/messages_response_401.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.messages_response_401_data import MessagesResponse401Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, MessagesResponse401Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = MessagesResponse401Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, MessagesResponse401Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = MessagesResponse401Data.from_dict(_data)
 
         messages_response_401 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        messages_response_401.additional_properties = d
+        messages_response_401.additional_properties = src_dict
         return messages_response_401
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/messages_response_401_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, MessagesResponse401DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = MessagesResponse401DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         messages_response_401_data = cls(
             code=code,
             message=message,
         )
 
-        messages_response_401_data.additional_properties = d
+        messages_response_401_data.additional_properties = src_dict
         return messages_response_401_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/messages_response_404.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.messages_response_404_data import MessagesResponse404Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, MessagesResponse404Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = MessagesResponse404Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, MessagesResponse404Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = MessagesResponse404Data.from_dict(_data)
 
         messages_response_404 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        messages_response_404.additional_properties = d
+        messages_response_404.additional_properties = src_dict
         return messages_response_404
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/messages_response_404_data.py

```diff
@@ -38,35 +38,34 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, MessagesResponse404DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = MessagesResponse404DataCode(_code)
 
-        _message = d.pop("message", UNSET)
+        _message = src_dict.get("message")
         message: Union[Unset, MessagesResponse404DataMessage]
         if isinstance(_message, Unset):
             message = UNSET
         else:
             message = MessagesResponse404DataMessage(_message)
 
         messages_response_404_data = cls(
             code=code,
             message=message,
         )
 
-        messages_response_404_data.additional_properties = d
+        messages_response_404_data.additional_properties = src_dict
         return messages_response_404_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/messages_response_500.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.messages_response_500_data import MessagesResponse500Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, MessagesResponse500Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = MessagesResponse500Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, MessagesResponse500Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = MessagesResponse500Data.from_dict(_data)
 
         messages_response_500 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        messages_response_500.additional_properties = d
+        messages_response_500.additional_properties = src_dict
         return messages_response_500
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/messages_response_500_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, MessagesResponse500DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = MessagesResponse500DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         messages_response_500_data = cls(
             code=code,
             message=message,
         )
 
-        messages_response_500_data.additional_properties = d
+        messages_response_500_data.additional_properties = src_dict
         return messages_response_500_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/open_graph_cache.py

```diff
@@ -68,46 +68,45 @@
         if site_name is not UNSET:
             field_dict["site_name"] = site_name
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        page_url = d.pop("page_url", UNSET)
+        page_url = src_dict.get("page_url")
 
-        title = d.pop("title", UNSET)
+        title = src_dict.get("title")
 
-        description = d.pop("description", UNSET)
+        description = src_dict.get("description")
 
-        image = d.pop("image", UNSET)
+        image = src_dict.get("image")
 
-        image_width = d.pop("image_width", UNSET)
+        image_width = src_dict.get("image_width")
 
-        image_height = d.pop("image_height", UNSET)
+        image_height = src_dict.get("image_height")
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        favicon = d.pop("favicon", UNSET)
+        favicon = src_dict.get("favicon")
 
-        site_name = d.pop("site_name", UNSET)
+        site_name = src_dict.get("site_name")
 
         open_graph_cache = cls(
             page_url=page_url,
             title=title,
             description=description,
             image=image,
             image_width=image_width,
             image_height=image_height,
             url=url,
             favicon=favicon,
             site_name=site_name,
         )
 
-        open_graph_cache.additional_properties = d
+        open_graph_cache.additional_properties = src_dict
         return open_graph_cache
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/page.py

```diff
@@ -1,17 +1,16 @@
 import datetime
-from io import BytesIO
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..models.page_crawl_status import PageCrawlStatus
 from ..models.page_index_status import PageIndexStatus
-from ..types import UNSET, File, FileJsonType, Unset
+from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="Page")
 
 
 @attr.s(auto_attribs=True)
 class Page:
     r"""
@@ -26,40 +25,40 @@
         crawl_status (Union[Unset, PageCrawlStatus]): Crawl status of the page Default: PageCrawlStatus.QUEUED. Example:
             queued.
         index_status (Union[Unset, PageIndexStatus]): Index status of the page Default: PageIndexStatus.QUEUED. Example:
             queued.
         is_file (Union[Unset, bool]): Whether the page is a file or not Example: True.
         is_file_kept (Union[Unset, bool]): Whether the file is kept after processing or not.\nNote: This is omitted in
             the response if the page is not a file Default: True. Example: True.
-        filename (Union[Unset, None, File]): Filename of the page.\nNote: This is omitted in the response if the page is
+        filename (Union[Unset, None, str]): Filename of the page.\nNote: This is omitted in the response if the page is
             not a file Example: file.pdf.
         filesize (Union[Unset, None, int]): Filesize of the page.\nNote: This is omitted in the response if the page is
             not a file Example: 100.
         created_at (Union[Unset, datetime.datetime]): Date and time when the page was created Example: 2021-01-01
             00:00:00.
         updated_at (Union[Unset, datetime.datetime]): Date and time when the page was updated Example: 2021-01-01
             00:00:00.
-        deleted_at (Union[Unset, datetime.datetime]): Date and time when the page was deleted Example: 2021-01-01
+        deleted_at (Union[Unset, None, datetime.datetime]): Date and time when the page was deleted Example: 2021-01-01
             00:00:00.
     """
 
     id: Union[Unset, int] = UNSET
     page_url: Union[Unset, str] = UNSET
     page_url_hash: Union[Unset, str] = UNSET
     project_id: Union[Unset, int] = UNSET
     s3_path: Union[Unset, None, str] = UNSET
     crawl_status: Union[Unset, PageCrawlStatus] = PageCrawlStatus.QUEUED
     index_status: Union[Unset, PageIndexStatus] = PageIndexStatus.QUEUED
     is_file: Union[Unset, bool] = False
     is_file_kept: Union[Unset, bool] = True
-    filename: Union[Unset, None, File] = UNSET
+    filename: Union[Unset, None, str] = UNSET
     filesize: Union[Unset, None, int] = UNSET
     created_at: Union[Unset, datetime.datetime] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
-    deleted_at: Union[Unset, datetime.datetime] = UNSET
+    deleted_at: Union[Unset, None, datetime.datetime] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
         page_url = self.page_url
         page_url_hash = self.page_url_hash
         project_id = self.project_id
@@ -70,30 +69,27 @@
 
         index_status: Union[Unset, str] = UNSET
         if not isinstance(self.index_status, Unset):
             index_status = self.index_status.value
 
         is_file = self.is_file
         is_file_kept = self.is_file_kept
-        filename: Union[Unset, None, FileJsonType] = UNSET
-        if not isinstance(self.filename, Unset):
-            filename = self.filename.to_tuple() if self.filename else None
-
+        filename = self.filename
         filesize = self.filesize
         created_at: Union[Unset, str] = UNSET
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
 
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
 
-        deleted_at: Union[Unset, str] = UNSET
+        deleted_at: Union[Unset, None, str] = UNSET
         if not isinstance(self.deleted_at, Unset):
-            deleted_at = self.deleted_at.isoformat()
+            deleted_at = self.deleted_at.isoformat() if self.deleted_at else None
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if id is not UNSET:
             field_dict["id"] = id
         if page_url is not UNSET:
@@ -123,71 +119,65 @@
         if deleted_at is not UNSET:
             field_dict["deleted_at"] = deleted_at
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        id = d.pop("id", UNSET)
+        id = src_dict.get("id")
 
-        page_url = d.pop("page_url", UNSET)
+        page_url = src_dict.get("page_url")
 
-        page_url_hash = d.pop("page_url_hash", UNSET)
+        page_url_hash = src_dict.get("page_url_hash")
 
-        project_id = d.pop("project_id", UNSET)
+        project_id = src_dict.get("project_id")
 
-        s3_path = d.pop("s3_path", UNSET)
+        s3_path = src_dict.get("s3_path")
 
-        _crawl_status = d.pop("crawl_status", UNSET)
+        _crawl_status = src_dict.get("crawl_status")
         crawl_status: Union[Unset, PageCrawlStatus]
         if isinstance(_crawl_status, Unset):
             crawl_status = UNSET
         else:
             crawl_status = PageCrawlStatus(_crawl_status)
 
-        _index_status = d.pop("index_status", UNSET)
+        _index_status = src_dict.get("index_status")
         index_status: Union[Unset, PageIndexStatus]
         if isinstance(_index_status, Unset):
             index_status = UNSET
         else:
             index_status = PageIndexStatus(_index_status)
 
-        is_file = d.pop("is_file", UNSET)
+        is_file = src_dict.get("is_file")
 
-        is_file_kept = d.pop("is_file_kept", UNSET)
+        is_file_kept = src_dict.get("is_file_kept")
 
-        _filename = d.pop("filename", UNSET)
-        filename: Union[Unset, None, File]
-        if _filename is None:
-            filename = None
-        elif isinstance(_filename, Unset):
-            filename = UNSET
-        else:
-            filename = File(payload=BytesIO(_filename))
+        filename = src_dict.get("filename")
 
-        filesize = d.pop("filesize", UNSET)
+        filesize = src_dict.get("filesize")
 
-        _created_at = d.pop("created_at", UNSET)
+        _created_at = src_dict.get("created_at")
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
-        _updated_at = d.pop("updated_at", UNSET)
+        _updated_at = src_dict.get("updated_at")
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
-        _deleted_at = d.pop("deleted_at", UNSET)
-        deleted_at: Union[Unset, datetime.datetime]
-        if isinstance(_deleted_at, Unset):
+        _deleted_at = src_dict.get("deleted_at")
+        deleted_at: Union[Unset, None, datetime.datetime]
+        if _deleted_at is None:
+            deleted_at = None
+        elif isinstance(_deleted_at, Unset):
             deleted_at = UNSET
         else:
             deleted_at = isoparse(_deleted_at)
 
         page = cls(
             id=id,
             page_url=page_url,
@@ -201,15 +191,15 @@
             filename=filename,
             filesize=filesize,
             created_at=created_at,
             updated_at=updated_at,
             deleted_at=deleted_at,
         )
 
-        page.additional_properties = d
+        page.additional_properties = src_dict
         return page
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/preview_response_401.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.preview_response_401_data import PreviewResponse401Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, PreviewResponse401Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = PreviewResponse401Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, PreviewResponse401Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = PreviewResponse401Data.from_dict(_data)
 
         preview_response_401 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        preview_response_401.additional_properties = d
+        preview_response_401.additional_properties = src_dict
         return preview_response_401
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/preview_response_401_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, PreviewResponse401DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = PreviewResponse401DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         preview_response_401_data = cls(
             code=code,
             message=message,
         )
 
-        preview_response_401_data.additional_properties = d
+        preview_response_401_data.additional_properties = src_dict
         return preview_response_401_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/preview_response_404.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.preview_response_404_data import PreviewResponse404Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, PreviewResponse404Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = PreviewResponse404Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, PreviewResponse404Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = PreviewResponse404Data.from_dict(_data)
 
         preview_response_404 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        preview_response_404.additional_properties = d
+        preview_response_404.additional_properties = src_dict
         return preview_response_404
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/preview_response_404_data.py

```diff
@@ -38,35 +38,34 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, PreviewResponse404DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = PreviewResponse404DataCode(_code)
 
-        _message = d.pop("message", UNSET)
+        _message = src_dict.get("message")
         message: Union[Unset, PreviewResponse404DataMessage]
         if isinstance(_message, Unset):
             message = UNSET
         else:
             message = PreviewResponse404DataMessage(_message)
 
         preview_response_404_data = cls(
             code=code,
             message=message,
         )
 
-        preview_response_404_data.additional_properties = d
+        preview_response_404_data.additional_properties = src_dict
         return preview_response_404_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/preview_response_500.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.preview_response_500_data import PreviewResponse500Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, PreviewResponse500Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = PreviewResponse500Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, PreviewResponse500Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = PreviewResponse500Data.from_dict(_data)
 
         preview_response_500 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        preview_response_500.additional_properties = d
+        preview_response_500.additional_properties = src_dict
         return preview_response_500
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/preview_response_500_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, PreviewResponse500DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = PreviewResponse500DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         preview_response_500_data = cls(
             code=code,
             message=message,
         )
 
-        preview_response_500_data.additional_properties = d
+        preview_response_500_data.additional_properties = src_dict
         return preview_response_500_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/project.py

```diff
@@ -110,64 +110,63 @@
         if live_chat_code is not UNSET:
             field_dict["live_chat_code"] = live_chat_code
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        id = d.pop("id", UNSET)
+        id = src_dict.get("id")
 
-        project_name = d.pop("project_name", UNSET)
+        project_name = src_dict.get("project_name")
 
-        sitemap_path = d.pop("sitemap_path", UNSET)
+        sitemap_path = src_dict.get("sitemap_path")
 
-        is_chat_active = d.pop("is_chat_active", UNSET)
+        is_chat_active = src_dict.get("is_chat_active")
 
-        user_id = d.pop("user_id", UNSET)
+        user_id = src_dict.get("user_id")
 
-        _created_at = d.pop("created_at", UNSET)
+        _created_at = src_dict.get("created_at")
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
-        _updated_at = d.pop("updated_at", UNSET)
+        _updated_at = src_dict.get("updated_at")
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
-        _deleted_at = d.pop("deleted_at", UNSET)
+        _deleted_at = src_dict.get("deleted_at")
         deleted_at: Union[Unset, None, datetime.datetime]
         if _deleted_at is None:
             deleted_at = None
         elif isinstance(_deleted_at, Unset):
             deleted_at = UNSET
         else:
             deleted_at = isoparse(_deleted_at)
 
-        _type = d.pop("type", UNSET)
+        _type = src_dict.get("type")
         type: Union[Unset, ProjectType]
         if isinstance(_type, Unset):
             type = UNSET
         else:
             type = ProjectType(_type)
 
-        is_shared = d.pop("is_shared", UNSET)
+        is_shared = src_dict.get("is_shared")
 
-        shareable_slug = d.pop("shareable_slug", UNSET)
+        shareable_slug = src_dict.get("shareable_slug")
 
-        shareable_link = d.pop("shareable_link", UNSET)
+        shareable_link = src_dict.get("shareable_link")
 
-        embed_code = d.pop("embed_code", UNSET)
+        embed_code = src_dict.get("embed_code")
 
-        live_chat_code = d.pop("live_chat_code", UNSET)
+        live_chat_code = src_dict.get("live_chat_code")
 
         project = cls(
             id=id,
             project_name=project_name,
             sitemap_path=sitemap_path,
             is_chat_active=is_chat_active,
             user_id=user_id,
@@ -178,15 +177,15 @@
             is_shared=is_shared,
             shareable_slug=shareable_slug,
             shareable_link=shareable_link,
             embed_code=embed_code,
             live_chat_code=live_chat_code,
         )
 
-        project.additional_properties = d
+        project.additional_properties = src_dict
         return project
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/project_plugin.py

```diff
@@ -7,47 +7,42 @@
 T = TypeVar("T", bound="ProjectPlugin")
 
 
 @attr.s(auto_attribs=True)
 class ProjectPlugin:
     """
     Attributes:
-        id (Union[Unset, int]): Plugin ID Example: 1.
         model_name (Union[Unset, str]): Model Name Example: IndoorPlants.
         human_name (Union[Unset, str]): Name For Human Example: The Indoor Plants Channel.
         keywords (Union[Unset, str]): Keywords For Model Example: Indoor plants, Gardening, Trusted information..
         description (Union[Unset, str]): Description For Human Example: Trusted information about indoor plants and
             gardening..
         logo (Union[Unset, str]): Project plugin logo Example: https://app.customgpt.ai/logo.svg.
         is_active (Union[Unset, bool]): Whether the project plugin is active or not Example: True.
     """
 
-    id: Union[Unset, int] = UNSET
     model_name: Union[Unset, str] = UNSET
     human_name: Union[Unset, str] = UNSET
     keywords: Union[Unset, str] = UNSET
     description: Union[Unset, str] = UNSET
     logo: Union[Unset, str] = UNSET
     is_active: Union[Unset, bool] = False
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        id = self.id
         model_name = self.model_name
         human_name = self.human_name
         keywords = self.keywords
         description = self.description
         logo = self.logo
         is_active = self.is_active
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if id is not UNSET:
-            field_dict["id"] = id
         if model_name is not UNSET:
             field_dict["model_name"] = model_name
         if human_name is not UNSET:
             field_dict["human_name"] = human_name
         if keywords is not UNSET:
             field_dict["keywords"] = keywords
         if description is not UNSET:
@@ -57,40 +52,36 @@
         if is_active is not UNSET:
             field_dict["is_active"] = is_active
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        id = d.pop("id", UNSET)
+        model_name = src_dict.get("model_name")
 
-        model_name = d.pop("model_name", UNSET)
+        human_name = src_dict.get("human_name")
 
-        human_name = d.pop("human_name", UNSET)
+        keywords = src_dict.get("keywords")
 
-        keywords = d.pop("keywords", UNSET)
+        description = src_dict.get("description")
 
-        description = d.pop("description", UNSET)
+        logo = src_dict.get("logo")
 
-        logo = d.pop("logo", UNSET)
-
-        is_active = d.pop("is_active", UNSET)
+        is_active = src_dict.get("is_active")
 
         project_plugin = cls(
-            id=id,
             model_name=model_name,
             human_name=human_name,
             keywords=keywords,
             description=description,
             logo=logo,
             is_active=is_active,
         )
 
-        project_plugin.additional_properties = d
+        project_plugin.additional_properties = src_dict
         return project_plugin
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/project_settings.py

```diff
@@ -16,22 +16,24 @@
         chatbot_background (Union[Unset, str]): The chatbot background Example:
             https://example.com/chatbot_background.png.
         default_prompt (Union[Unset, str]): The default prompt Example: How can I help you?.
         example_questions (Union[Unset, List[str]]): The example questions Example: ['How do I get started?'].
         response_source (Union[Unset, ProjectSettingsResponseSource]): The response source Example:
             https://example.com/response_source.json.
         chatbot_msg_lang (Union[Unset, str]): The chatbot message language Example: en.
+        chatbot_color (Union[Unset, str]): The chatbot color in hex format Example: #000000.
     """
 
     chatbot_avatar: Union[Unset, str] = UNSET
     chatbot_background: Union[Unset, str] = UNSET
     default_prompt: Union[Unset, str] = UNSET
     example_questions: Union[Unset, List[str]] = UNSET
     response_source: Union[Unset, ProjectSettingsResponseSource] = UNSET
     chatbot_msg_lang: Union[Unset, str] = UNSET
+    chatbot_color: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         chatbot_avatar = self.chatbot_avatar
         chatbot_background = self.chatbot_background
         default_prompt = self.default_prompt
         example_questions: Union[Unset, List[str]] = UNSET
@@ -39,14 +41,15 @@
             example_questions = self.example_questions
 
         response_source: Union[Unset, str] = UNSET
         if not isinstance(self.response_source, Unset):
             response_source = self.response_source.value
 
         chatbot_msg_lang = self.chatbot_msg_lang
+        chatbot_color = self.chatbot_color
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
         if chatbot_avatar is not UNSET:
             field_dict["chatbot_avatar"] = chatbot_avatar
         if chatbot_background is not UNSET:
@@ -56,47 +59,51 @@
         if example_questions is not UNSET:
             for index, field_value in enumerate(example_questions):
                 field_dict[f"example_questions[]{index}"] = field_value
         if response_source is not UNSET:
             field_dict["response_source"] = response_source
         if chatbot_msg_lang is not UNSET:
             field_dict["chatbot_msg_lang"] = chatbot_msg_lang
+        if chatbot_color is not UNSET:
+            field_dict["chatbot_color"] = chatbot_color
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        chatbot_avatar = d.pop("chatbot_avatar", UNSET)
+        chatbot_avatar = src_dict.get("chatbot_avatar")
 
-        chatbot_background = d.pop("chatbot_background", UNSET)
+        chatbot_background = src_dict.get("chatbot_background")
 
-        default_prompt = d.pop("default_prompt", UNSET)
+        default_prompt = src_dict.get("default_prompt")
 
-        example_questions = cast(List[str], d.pop("example_questions", UNSET))
+        example_questions = cast(List[str], src_dict.get("example_questions"))
 
-        _response_source = d.pop("response_source", UNSET)
+        _response_source = src_dict.get("response_source")
         response_source: Union[Unset, ProjectSettingsResponseSource]
         if isinstance(_response_source, Unset):
             response_source = UNSET
         else:
             response_source = ProjectSettingsResponseSource(_response_source)
 
-        chatbot_msg_lang = d.pop("chatbot_msg_lang", UNSET)
+        chatbot_msg_lang = src_dict.get("chatbot_msg_lang")
+
+        chatbot_color = src_dict.get("chatbot_color")
 
         project_settings = cls(
             chatbot_avatar=chatbot_avatar,
             chatbot_background=chatbot_background,
             default_prompt=default_prompt,
             example_questions=example_questions,
             response_source=response_source,
             chatbot_msg_lang=chatbot_msg_lang,
+            chatbot_color=chatbot_color,
         )
 
-        project_settings.additional_properties = d
+        project_settings.additional_properties = src_dict
         return project_settings
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/prompt_history.py

```diff
@@ -75,53 +75,52 @@
             for index, field_value in enumerate(citations):
                 field_dict[f"citations[]{index}"] = field_value
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        id = d.pop("id", UNSET)
+        id = src_dict.get("id")
 
-        user_id = d.pop("user_id", UNSET)
+        user_id = src_dict.get("user_id")
 
-        user_query = d.pop("user_query", UNSET)
+        user_query = src_dict.get("user_query")
 
-        openai_response = d.pop("openai_response", UNSET)
+        openai_response = src_dict.get("openai_response")
 
-        _created_at = d.pop("created_at", UNSET)
+        _created_at = src_dict.get("created_at")
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
-        _updated_at = d.pop("updated_at", UNSET)
+        _updated_at = src_dict.get("updated_at")
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
-        conversation_id = d.pop("conversation_id", UNSET)
+        conversation_id = src_dict.get("conversation_id")
 
-        citations = cast(List[int], d.pop("citations", UNSET))
+        citations = cast(List[int], src_dict.get("citations"))
 
         prompt_history = cls(
             id=id,
             user_id=user_id,
             user_query=user_query,
             openai_response=openai_response,
             created_at=created_at,
             updated_at=updated_at,
             conversation_id=conversation_id,
             citations=citations,
         )
 
-        prompt_history.additional_properties = d
+        prompt_history.additional_properties = src_dict
         return prompt_history
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/send_message_to_conversation_json_body.py

```diff
@@ -26,22 +26,21 @@
         if prompt is not UNSET:
             field_dict["prompt"] = prompt
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        prompt = d.pop("prompt", UNSET)
+        prompt = src_dict.get("prompt")
 
         send_message_to_conversation_json_body = cls(
             prompt=prompt,
         )
 
-        send_message_to_conversation_json_body.additional_properties = d
+        send_message_to_conversation_json_body.additional_properties = src_dict
         return send_message_to_conversation_json_body
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/send_message_to_conversation_response_200.py

```diff
@@ -43,35 +43,34 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.send_message_to_conversation_response_200_data import SendMessageToConversationResponse200Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, SendMessageToConversationResponse200Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = SendMessageToConversationResponse200Status(_status)
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, SendMessageToConversationResponse200Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = SendMessageToConversationResponse200Data.from_dict(_data)
 
         send_message_to_conversation_response_200 = cls(
             status=status,
             data=data,
         )
 
-        send_message_to_conversation_response_200.additional_properties = d
+        send_message_to_conversation_response_200.additional_properties = src_dict
         return send_message_to_conversation_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/send_message_to_conversation_response_200_data.py

```diff
@@ -75,53 +75,52 @@
             for index, field_value in enumerate(citations):
                 field_dict[f"citations[]{index}"] = field_value
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        id = d.pop("id", UNSET)
+        id = src_dict.get("id")
 
-        user_id = d.pop("user_id", UNSET)
+        user_id = src_dict.get("user_id")
 
-        user_query = d.pop("user_query", UNSET)
+        user_query = src_dict.get("user_query")
 
-        openai_response = d.pop("openai_response", UNSET)
+        openai_response = src_dict.get("openai_response")
 
-        _created_at = d.pop("created_at", UNSET)
+        _created_at = src_dict.get("created_at")
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
-        _updated_at = d.pop("updated_at", UNSET)
+        _updated_at = src_dict.get("updated_at")
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
-        conversation_id = d.pop("conversation_id", UNSET)
+        conversation_id = src_dict.get("conversation_id")
 
-        citations = cast(List[int], d.pop("citations", UNSET))
+        citations = cast(List[int], src_dict.get("citations"))
 
         send_message_to_conversation_response_200_data = cls(
             id=id,
             user_id=user_id,
             user_query=user_query,
             openai_response=openai_response,
             created_at=created_at,
             updated_at=updated_at,
             conversation_id=conversation_id,
             citations=citations,
         )
 
-        send_message_to_conversation_response_200_data.additional_properties = d
+        send_message_to_conversation_response_200_data.additional_properties = src_dict
         return send_message_to_conversation_response_200_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/send_message_to_conversation_response_401.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.send_message_to_conversation_response_401_data import SendMessageToConversationResponse401Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, SendMessageToConversationResponse401Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = SendMessageToConversationResponse401Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, SendMessageToConversationResponse401Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = SendMessageToConversationResponse401Data.from_dict(_data)
 
         send_message_to_conversation_response_401 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        send_message_to_conversation_response_401.additional_properties = d
+        send_message_to_conversation_response_401.additional_properties = src_dict
         return send_message_to_conversation_response_401
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/send_message_to_conversation_response_401_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, SendMessageToConversationResponse401DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = SendMessageToConversationResponse401DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         send_message_to_conversation_response_401_data = cls(
             code=code,
             message=message,
         )
 
-        send_message_to_conversation_response_401_data.additional_properties = d
+        send_message_to_conversation_response_401_data.additional_properties = src_dict
         return send_message_to_conversation_response_401_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/send_message_to_conversation_response_404.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.send_message_to_conversation_response_404_data import SendMessageToConversationResponse404Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, SendMessageToConversationResponse404Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = SendMessageToConversationResponse404Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, SendMessageToConversationResponse404Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = SendMessageToConversationResponse404Data.from_dict(_data)
 
         send_message_to_conversation_response_404 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        send_message_to_conversation_response_404.additional_properties = d
+        send_message_to_conversation_response_404.additional_properties = src_dict
         return send_message_to_conversation_response_404
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/send_message_to_conversation_response_404_data.py

```diff
@@ -41,35 +41,34 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, SendMessageToConversationResponse404DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = SendMessageToConversationResponse404DataCode(_code)
 
-        _message = d.pop("message", UNSET)
+        _message = src_dict.get("message")
         message: Union[Unset, SendMessageToConversationResponse404DataMessage]
         if isinstance(_message, Unset):
             message = UNSET
         else:
             message = SendMessageToConversationResponse404DataMessage(_message)
 
         send_message_to_conversation_response_404_data = cls(
             code=code,
             message=message,
         )
 
-        send_message_to_conversation_response_404_data.additional_properties = d
+        send_message_to_conversation_response_404_data.additional_properties = src_dict
         return send_message_to_conversation_response_404_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/send_message_to_conversation_response_500.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.send_message_to_conversation_response_500_data import SendMessageToConversationResponse500Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, SendMessageToConversationResponse500Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = SendMessageToConversationResponse500Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, SendMessageToConversationResponse500Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = SendMessageToConversationResponse500Data.from_dict(_data)
 
         send_message_to_conversation_response_500 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        send_message_to_conversation_response_500.additional_properties = d
+        send_message_to_conversation_response_500.additional_properties = src_dict
         return send_message_to_conversation_response_500
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/send_message_to_conversation_response_500_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, SendMessageToConversationResponse500DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = SendMessageToConversationResponse500DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         send_message_to_conversation_response_500_data = cls(
             code=code,
             message=message,
         )
 
-        send_message_to_conversation_response_500_data.additional_properties = d
+        send_message_to_conversation_response_500_data.additional_properties = src_dict
         return send_message_to_conversation_response_500_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/stats_project_response_200.py

```diff
@@ -43,35 +43,34 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.stats_project_response_200_data import StatsProjectResponse200Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, StatsProjectResponse200Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = StatsProjectResponse200Status(_status)
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, StatsProjectResponse200Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = StatsProjectResponse200Data.from_dict(_data)
 
         stats_project_response_200 = cls(
             status=status,
             data=data,
         )
 
-        stats_project_response_200.additional_properties = d
+        stats_project_response_200.additional_properties = src_dict
         return stats_project_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/stats_project_response_200_data.py

```diff
@@ -51,37 +51,36 @@
         if index_credits_used is not UNSET:
             field_dict["index_credits_used"] = index_credits_used
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        pages_found = d.pop("pages_found", UNSET)
+        pages_found = src_dict.get("pages_found")
 
-        pages_crawled = d.pop("pages_crawled", UNSET)
+        pages_crawled = src_dict.get("pages_crawled")
 
-        pages_indexed = d.pop("pages_indexed", UNSET)
+        pages_indexed = src_dict.get("pages_indexed")
 
-        crawl_credits_used = d.pop("crawl_credits_used", UNSET)
+        crawl_credits_used = src_dict.get("crawl_credits_used")
 
-        query_credits_used = d.pop("query_credits_used", UNSET)
+        query_credits_used = src_dict.get("query_credits_used")
 
-        index_credits_used = d.pop("index_credits_used", UNSET)
+        index_credits_used = src_dict.get("index_credits_used")
 
         stats_project_response_200_data = cls(
             pages_found=pages_found,
             pages_crawled=pages_crawled,
             pages_indexed=pages_indexed,
             crawl_credits_used=crawl_credits_used,
             query_credits_used=query_credits_used,
             index_credits_used=index_credits_used,
         )
 
-        stats_project_response_200_data.additional_properties = d
+        stats_project_response_200_data.additional_properties = src_dict
         return stats_project_response_200_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/stats_project_response_401.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.stats_project_response_401_data import StatsProjectResponse401Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, StatsProjectResponse401Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = StatsProjectResponse401Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, StatsProjectResponse401Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = StatsProjectResponse401Data.from_dict(_data)
 
         stats_project_response_401 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        stats_project_response_401.additional_properties = d
+        stats_project_response_401.additional_properties = src_dict
         return stats_project_response_401
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/stats_project_response_401_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, StatsProjectResponse401DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = StatsProjectResponse401DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         stats_project_response_401_data = cls(
             code=code,
             message=message,
         )
 
-        stats_project_response_401_data.additional_properties = d
+        stats_project_response_401_data.additional_properties = src_dict
         return stats_project_response_401_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/stats_project_response_404.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.stats_project_response_404_data import StatsProjectResponse404Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, StatsProjectResponse404Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = StatsProjectResponse404Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, StatsProjectResponse404Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = StatsProjectResponse404Data.from_dict(_data)
 
         stats_project_response_404 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        stats_project_response_404.additional_properties = d
+        stats_project_response_404.additional_properties = src_dict
         return stats_project_response_404
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/stats_project_response_404_data.py

```diff
@@ -38,35 +38,34 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, StatsProjectResponse404DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = StatsProjectResponse404DataCode(_code)
 
-        _message = d.pop("message", UNSET)
+        _message = src_dict.get("message")
         message: Union[Unset, StatsProjectResponse404DataMessage]
         if isinstance(_message, Unset):
             message = UNSET
         else:
             message = StatsProjectResponse404DataMessage(_message)
 
         stats_project_response_404_data = cls(
             code=code,
             message=message,
         )
 
-        stats_project_response_404_data.additional_properties = d
+        stats_project_response_404_data.additional_properties = src_dict
         return stats_project_response_404_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/stats_project_response_500.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.stats_project_response_500_data import StatsProjectResponse500Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, StatsProjectResponse500Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = StatsProjectResponse500Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, StatsProjectResponse500Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = StatsProjectResponse500Data.from_dict(_data)
 
         stats_project_response_500 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        stats_project_response_500.additional_properties = d
+        stats_project_response_500.additional_properties = src_dict
         return stats_project_response_500
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/stats_project_response_500_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, StatsProjectResponse500DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = StatsProjectResponse500DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         stats_project_response_500_data = cls(
             code=code,
             message=message,
         )
 
-        stats_project_response_500_data.additional_properties = d
+        stats_project_response_500_data.additional_properties = src_dict
         return stats_project_response_500_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_conversation_json_body.py

```diff
@@ -26,22 +26,21 @@
         if name is not UNSET:
             field_dict["name"] = name
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        name = d.pop("name", UNSET)
+        name = src_dict.get("name")
 
         update_project_conversation_json_body = cls(
             name=name,
         )
 
-        update_project_conversation_json_body.additional_properties = d
+        update_project_conversation_json_body.additional_properties = src_dict
         return update_project_conversation_json_body
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_conversation_response_200.py

```diff
@@ -43,35 +43,34 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.update_project_conversation_response_200_data import UpdateProjectConversationResponse200Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, UpdateProjectConversationResponse200Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = UpdateProjectConversationResponse200Status(_status)
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, UpdateProjectConversationResponse200Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = UpdateProjectConversationResponse200Data.from_dict(_data)
 
         update_project_conversation_response_200 = cls(
             status=status,
             data=data,
         )
 
-        update_project_conversation_response_200.additional_properties = d
+        update_project_conversation_response_200.additional_properties = src_dict
         return update_project_conversation_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_conversation_response_200_data.py

```diff
@@ -11,25 +11,26 @@
 
 @attr.s(auto_attribs=True)
 class UpdateProjectConversationResponse200Data:
     """
     Attributes:
         created_at (Union[Unset, datetime.datetime]): When was this conversation created? Example: 2023-04-30 16:43:53.
         updated_at (Union[Unset, datetime.datetime]): When was this conversation updated? Example: 2023-04-30 16:43:53.
-        deleted_at (Union[Unset, datetime.datetime]): When was this conversation deleted? Example: 2023-04-30 16:43:53.
+        deleted_at (Union[Unset, None, datetime.datetime]): When was this conversation deleted? Example: 2023-04-30
+            16:43:53.
         id (Union[Unset, int]): Conversation ID Example: 1.
         name (Union[Unset, str]): Conversation name Example: Conversation 1.
         project_id (Union[Unset, str]): Project ID for this conversation Example: 1.
         created_by (Union[Unset, str]): User ID for the user who created this conversation Example: 1.
         session_id (Union[Unset, str]): Session ID for this conversation Example: f1b9aaf0-5e4e-11eb-ae93-0242ac130002.
     """
 
     created_at: Union[Unset, datetime.datetime] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
-    deleted_at: Union[Unset, datetime.datetime] = UNSET
+    deleted_at: Union[Unset, None, datetime.datetime] = UNSET
     id: Union[Unset, int] = UNSET
     name: Union[Unset, str] = UNSET
     project_id: Union[Unset, str] = UNSET
     created_by: Union[Unset, str] = UNSET
     session_id: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -38,17 +39,17 @@
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
 
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
 
-        deleted_at: Union[Unset, str] = UNSET
+        deleted_at: Union[Unset, None, str] = UNSET
         if not isinstance(self.deleted_at, Unset):
-            deleted_at = self.deleted_at.isoformat()
+            deleted_at = self.deleted_at.isoformat() if self.deleted_at else None
 
         id = self.id
         name = self.name
         project_id = self.project_id
         created_by = self.created_by
         session_id = self.session_id
 
@@ -72,58 +73,59 @@
         if session_id is not UNSET:
             field_dict["session_id"] = session_id
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _created_at = d.pop("created_at", UNSET)
+        _created_at = src_dict.get("created_at")
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
-        _updated_at = d.pop("updated_at", UNSET)
+        _updated_at = src_dict.get("updated_at")
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
-        _deleted_at = d.pop("deleted_at", UNSET)
-        deleted_at: Union[Unset, datetime.datetime]
-        if isinstance(_deleted_at, Unset):
+        _deleted_at = src_dict.get("deleted_at")
+        deleted_at: Union[Unset, None, datetime.datetime]
+        if _deleted_at is None:
+            deleted_at = None
+        elif isinstance(_deleted_at, Unset):
             deleted_at = UNSET
         else:
             deleted_at = isoparse(_deleted_at)
 
-        id = d.pop("id", UNSET)
+        id = src_dict.get("id")
 
-        name = d.pop("name", UNSET)
+        name = src_dict.get("name")
 
-        project_id = d.pop("project_id", UNSET)
+        project_id = src_dict.get("project_id")
 
-        created_by = d.pop("created_by", UNSET)
+        created_by = src_dict.get("created_by")
 
-        session_id = d.pop("session_id", UNSET)
+        session_id = src_dict.get("session_id")
 
         update_project_conversation_response_200_data = cls(
             created_at=created_at,
             updated_at=updated_at,
             deleted_at=deleted_at,
             id=id,
             name=name,
             project_id=project_id,
             created_by=created_by,
             session_id=session_id,
         )
 
-        update_project_conversation_response_200_data.additional_properties = d
+        update_project_conversation_response_200_data.additional_properties = src_dict
         return update_project_conversation_response_200_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_conversation_response_401.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.update_project_conversation_response_401_data import UpdateProjectConversationResponse401Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, UpdateProjectConversationResponse401Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = UpdateProjectConversationResponse401Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, UpdateProjectConversationResponse401Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = UpdateProjectConversationResponse401Data.from_dict(_data)
 
         update_project_conversation_response_401 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        update_project_conversation_response_401.additional_properties = d
+        update_project_conversation_response_401.additional_properties = src_dict
         return update_project_conversation_response_401
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_conversation_response_401_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, UpdateProjectConversationResponse401DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = UpdateProjectConversationResponse401DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         update_project_conversation_response_401_data = cls(
             code=code,
             message=message,
         )
 
-        update_project_conversation_response_401_data.additional_properties = d
+        update_project_conversation_response_401_data.additional_properties = src_dict
         return update_project_conversation_response_401_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_conversation_response_404.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.update_project_conversation_response_404_data import UpdateProjectConversationResponse404Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, UpdateProjectConversationResponse404Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = UpdateProjectConversationResponse404Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, UpdateProjectConversationResponse404Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = UpdateProjectConversationResponse404Data.from_dict(_data)
 
         update_project_conversation_response_404 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        update_project_conversation_response_404.additional_properties = d
+        update_project_conversation_response_404.additional_properties = src_dict
         return update_project_conversation_response_404
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_conversation_response_404_data.py

```diff
@@ -41,35 +41,34 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, UpdateProjectConversationResponse404DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = UpdateProjectConversationResponse404DataCode(_code)
 
-        _message = d.pop("message", UNSET)
+        _message = src_dict.get("message")
         message: Union[Unset, UpdateProjectConversationResponse404DataMessage]
         if isinstance(_message, Unset):
             message = UNSET
         else:
             message = UpdateProjectConversationResponse404DataMessage(_message)
 
         update_project_conversation_response_404_data = cls(
             code=code,
             message=message,
         )
 
-        update_project_conversation_response_404_data.additional_properties = d
+        update_project_conversation_response_404_data.additional_properties = src_dict
         return update_project_conversation_response_404_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_conversation_response_500.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.update_project_conversation_response_500_data import UpdateProjectConversationResponse500Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, UpdateProjectConversationResponse500Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = UpdateProjectConversationResponse500Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, UpdateProjectConversationResponse500Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = UpdateProjectConversationResponse500Data.from_dict(_data)
 
         update_project_conversation_response_500 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        update_project_conversation_response_500.additional_properties = d
+        update_project_conversation_response_500.additional_properties = src_dict
         return update_project_conversation_response_500
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_conversation_response_500_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, UpdateProjectConversationResponse500DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = UpdateProjectConversationResponse500DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         update_project_conversation_response_500_data = cls(
             code=code,
             message=message,
         )
 
-        update_project_conversation_response_500_data.additional_properties = d
+        update_project_conversation_response_500_data.additional_properties = src_dict
         return update_project_conversation_response_500_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_multipart_data.py

```diff
@@ -90,39 +90,38 @@
         if file is not UNSET:
             field_dict["file"] = file
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        project_name = d.pop("project_name", UNSET)
+        project_name = src_dict.get("project_name")
 
-        is_shared = d.pop("is_shared", UNSET)
+        is_shared = src_dict.get("is_shared")
 
-        sitemap_path = d.pop("sitemap_path", UNSET)
+        sitemap_path = src_dict.get("sitemap_path")
 
-        file_data_retension = d.pop("file_data_retension", UNSET)
+        file_data_retension = src_dict.get("file_data_retension")
 
-        _file = d.pop("file", UNSET)
+        _file = src_dict.get("file")
         file: Union[Unset, File]
         if isinstance(_file, Unset):
             file = UNSET
         else:
             file = File(payload=BytesIO(_file))
 
         update_project_multipart_data = cls(
             project_name=project_name,
             is_shared=is_shared,
             sitemap_path=sitemap_path,
             file_data_retension=file_data_retension,
             file=file,
         )
 
-        update_project_multipart_data.additional_properties = d
+        update_project_multipart_data.additional_properties = src_dict
         return update_project_multipart_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_response_200.py

```diff
@@ -43,35 +43,34 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.update_project_response_200_data import UpdateProjectResponse200Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, UpdateProjectResponse200Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = UpdateProjectResponse200Status(_status)
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, UpdateProjectResponse200Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = UpdateProjectResponse200Data.from_dict(_data)
 
         update_project_response_200 = cls(
             status=status,
             data=data,
         )
 
-        update_project_response_200.additional_properties = d
+        update_project_response_200.additional_properties = src_dict
         return update_project_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_response_200_data.py

```diff
@@ -111,64 +111,63 @@
         if live_chat_code is not UNSET:
             field_dict["live_chat_code"] = live_chat_code
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        id = d.pop("id", UNSET)
+        id = src_dict.get("id")
 
-        project_name = d.pop("project_name", UNSET)
+        project_name = src_dict.get("project_name")
 
-        sitemap_path = d.pop("sitemap_path", UNSET)
+        sitemap_path = src_dict.get("sitemap_path")
 
-        is_chat_active = d.pop("is_chat_active", UNSET)
+        is_chat_active = src_dict.get("is_chat_active")
 
-        user_id = d.pop("user_id", UNSET)
+        user_id = src_dict.get("user_id")
 
-        _created_at = d.pop("created_at", UNSET)
+        _created_at = src_dict.get("created_at")
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
-        _updated_at = d.pop("updated_at", UNSET)
+        _updated_at = src_dict.get("updated_at")
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
-        _deleted_at = d.pop("deleted_at", UNSET)
+        _deleted_at = src_dict.get("deleted_at")
         deleted_at: Union[Unset, None, datetime.datetime]
         if _deleted_at is None:
             deleted_at = None
         elif isinstance(_deleted_at, Unset):
             deleted_at = UNSET
         else:
             deleted_at = isoparse(_deleted_at)
 
-        _type = d.pop("type", UNSET)
+        _type = src_dict.get("type")
         type: Union[Unset, UpdateProjectResponse200DataType]
         if isinstance(_type, Unset):
             type = UNSET
         else:
             type = UpdateProjectResponse200DataType(_type)
 
-        is_shared = d.pop("is_shared", UNSET)
+        is_shared = src_dict.get("is_shared")
 
-        shareable_slug = d.pop("shareable_slug", UNSET)
+        shareable_slug = src_dict.get("shareable_slug")
 
-        shareable_link = d.pop("shareable_link", UNSET)
+        shareable_link = src_dict.get("shareable_link")
 
-        embed_code = d.pop("embed_code", UNSET)
+        embed_code = src_dict.get("embed_code")
 
-        live_chat_code = d.pop("live_chat_code", UNSET)
+        live_chat_code = src_dict.get("live_chat_code")
 
         update_project_response_200_data = cls(
             id=id,
             project_name=project_name,
             sitemap_path=sitemap_path,
             is_chat_active=is_chat_active,
             user_id=user_id,
@@ -179,15 +178,15 @@
             is_shared=is_shared,
             shareable_slug=shareable_slug,
             shareable_link=shareable_link,
             embed_code=embed_code,
             live_chat_code=live_chat_code,
         )
 
-        update_project_response_200_data.additional_properties = d
+        update_project_response_200_data.additional_properties = src_dict
         return update_project_response_200_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_response_401.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.update_project_response_401_data import UpdateProjectResponse401Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, UpdateProjectResponse401Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = UpdateProjectResponse401Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, UpdateProjectResponse401Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = UpdateProjectResponse401Data.from_dict(_data)
 
         update_project_response_401 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        update_project_response_401.additional_properties = d
+        update_project_response_401.additional_properties = src_dict
         return update_project_response_401
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_response_401_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, UpdateProjectResponse401DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = UpdateProjectResponse401DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         update_project_response_401_data = cls(
             code=code,
             message=message,
         )
 
-        update_project_response_401_data.additional_properties = d
+        update_project_response_401_data.additional_properties = src_dict
         return update_project_response_401_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_response_404.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.update_project_response_404_data import UpdateProjectResponse404Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, UpdateProjectResponse404Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = UpdateProjectResponse404Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, UpdateProjectResponse404Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = UpdateProjectResponse404Data.from_dict(_data)
 
         update_project_response_404 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        update_project_response_404.additional_properties = d
+        update_project_response_404.additional_properties = src_dict
         return update_project_response_404
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_response_404_data.py

```diff
@@ -39,35 +39,34 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, UpdateProjectResponse404DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = UpdateProjectResponse404DataCode(_code)
 
-        _message = d.pop("message", UNSET)
+        _message = src_dict.get("message")
         message: Union[Unset, UpdateProjectResponse404DataMessage]
         if isinstance(_message, Unset):
             message = UNSET
         else:
             message = UpdateProjectResponse404DataMessage(_message)
 
         update_project_response_404_data = cls(
             code=code,
             message=message,
         )
 
-        update_project_response_404_data.additional_properties = d
+        update_project_response_404_data.additional_properties = src_dict
         return update_project_response_404_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_response_500.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.update_project_response_500_data import UpdateProjectResponse500Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, UpdateProjectResponse500Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = UpdateProjectResponse500Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, UpdateProjectResponse500Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = UpdateProjectResponse500Data.from_dict(_data)
 
         update_project_response_500 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        update_project_response_500.additional_properties = d
+        update_project_response_500.additional_properties = src_dict
         return update_project_response_500
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_response_500_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, UpdateProjectResponse500DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = UpdateProjectResponse500DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         update_project_response_500_data = cls(
             code=code,
             message=message,
         )
 
-        update_project_response_500_data.additional_properties = d
+        update_project_response_500_data.additional_properties = src_dict
         return update_project_response_500_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_settings_multipart_data.py

```diff
@@ -116,47 +116,46 @@
         if chatbot_msg_lang is not UNSET:
             field_dict["chatbot_msg_lang"] = chatbot_msg_lang
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _chat_bot_avatar = d.pop("chat_bot_avatar", UNSET)
+        _chat_bot_avatar = src_dict.get("chat_bot_avatar")
         chat_bot_avatar: Union[Unset, File]
         if isinstance(_chat_bot_avatar, Unset):
             chat_bot_avatar = UNSET
         else:
             chat_bot_avatar = File(payload=BytesIO(_chat_bot_avatar))
 
-        _chat_bot_bg = d.pop("chat_bot_bg", UNSET)
+        _chat_bot_bg = src_dict.get("chat_bot_bg")
         chat_bot_bg: Union[Unset, File]
         if isinstance(_chat_bot_bg, Unset):
             chat_bot_bg = UNSET
         else:
             chat_bot_bg = File(payload=BytesIO(_chat_bot_bg))
 
-        default_prompt = d.pop("default_prompt", UNSET)
+        default_prompt = src_dict.get("default_prompt")
 
-        example_questions = cast(List[str], d.pop("example_questions", UNSET))
+        example_questions = cast(List[str], src_dict.get("example_questions"))
 
-        response_source = d.pop("response_source", UNSET)
+        response_source = src_dict.get("response_source")
 
-        chatbot_msg_lang = d.pop("chatbot_msg_lang", UNSET)
+        chatbot_msg_lang = src_dict.get("chatbot_msg_lang")
 
         update_project_settings_multipart_data = cls(
             chat_bot_avatar=chat_bot_avatar,
             chat_bot_bg=chat_bot_bg,
             default_prompt=default_prompt,
             example_questions=example_questions,
             response_source=response_source,
             chatbot_msg_lang=chatbot_msg_lang,
         )
 
-        update_project_settings_multipart_data.additional_properties = d
+        update_project_settings_multipart_data.additional_properties = src_dict
         return update_project_settings_multipart_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_settings_response_200.py

```diff
@@ -43,35 +43,34 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.update_project_settings_response_200_data import UpdateProjectSettingsResponse200Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, UpdateProjectSettingsResponse200Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = UpdateProjectSettingsResponse200Status(_status)
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, UpdateProjectSettingsResponse200Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = UpdateProjectSettingsResponse200Data.from_dict(_data)
 
         update_project_settings_response_200 = cls(
             status=status,
             data=data,
         )
 
-        update_project_settings_response_200.additional_properties = d
+        update_project_settings_response_200.additional_properties = src_dict
         return update_project_settings_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_settings_response_200_data.py

```diff
@@ -26,22 +26,21 @@
         if updated is not UNSET:
             field_dict["updated"] = updated
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        updated = d.pop("updated", UNSET)
+        updated = src_dict.get("updated")
 
         update_project_settings_response_200_data = cls(
             updated=updated,
         )
 
-        update_project_settings_response_200_data.additional_properties = d
+        update_project_settings_response_200_data.additional_properties = src_dict
         return update_project_settings_response_200_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_settings_response_400.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.update_project_settings_response_400_data import UpdateProjectSettingsResponse400Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, UpdateProjectSettingsResponse400Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = UpdateProjectSettingsResponse400Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, UpdateProjectSettingsResponse400Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = UpdateProjectSettingsResponse400Data.from_dict(_data)
 
         update_project_settings_response_400 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        update_project_settings_response_400.additional_properties = d
+        update_project_settings_response_400.additional_properties = src_dict
         return update_project_settings_response_400
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_settings_response_400_data.py

```diff
@@ -39,35 +39,34 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, UpdateProjectSettingsResponse400DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = UpdateProjectSettingsResponse400DataCode(_code)
 
-        _message = d.pop("message", UNSET)
+        _message = src_dict.get("message")
         message: Union[Unset, UpdateProjectSettingsResponse400DataMessage]
         if isinstance(_message, Unset):
             message = UNSET
         else:
             message = UpdateProjectSettingsResponse400DataMessage(_message)
 
         update_project_settings_response_400_data = cls(
             code=code,
             message=message,
         )
 
-        update_project_settings_response_400_data.additional_properties = d
+        update_project_settings_response_400_data.additional_properties = src_dict
         return update_project_settings_response_400_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_settings_response_401.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.update_project_settings_response_401_data import UpdateProjectSettingsResponse401Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, UpdateProjectSettingsResponse401Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = UpdateProjectSettingsResponse401Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, UpdateProjectSettingsResponse401Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = UpdateProjectSettingsResponse401Data.from_dict(_data)
 
         update_project_settings_response_401 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        update_project_settings_response_401.additional_properties = d
+        update_project_settings_response_401.additional_properties = src_dict
         return update_project_settings_response_401
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_settings_response_401_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, UpdateProjectSettingsResponse401DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = UpdateProjectSettingsResponse401DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         update_project_settings_response_401_data = cls(
             code=code,
             message=message,
         )
 
-        update_project_settings_response_401_data.additional_properties = d
+        update_project_settings_response_401_data.additional_properties = src_dict
         return update_project_settings_response_401_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_settings_response_500.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.update_project_settings_response_500_data import UpdateProjectSettingsResponse500Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, UpdateProjectSettingsResponse500Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = UpdateProjectSettingsResponse500Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, UpdateProjectSettingsResponse500Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = UpdateProjectSettingsResponse500Data.from_dict(_data)
 
         update_project_settings_response_500 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        update_project_settings_response_500.additional_properties = d
+        update_project_settings_response_500.additional_properties = src_dict
         return update_project_settings_response_500
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_project_settings_response_500_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, UpdateProjectSettingsResponse500DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = UpdateProjectSettingsResponse500DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         update_project_settings_response_500_data = cls(
             code=code,
             message=message,
         )
 
-        update_project_settings_response_500_data.additional_properties = d
+        update_project_settings_response_500_data.additional_properties = src_dict
         return update_project_settings_response_500_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_user_profile_multipart_data.py

```diff
@@ -54,30 +54,29 @@
         if name is not UNSET:
             field_dict["name"] = name
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _profile_photo = d.pop("profile_photo", UNSET)
+        _profile_photo = src_dict.get("profile_photo")
         profile_photo: Union[Unset, File]
         if isinstance(_profile_photo, Unset):
             profile_photo = UNSET
         else:
             profile_photo = File(payload=BytesIO(_profile_photo))
 
-        name = d.pop("name", UNSET)
+        name = src_dict.get("name")
 
         update_user_profile_multipart_data = cls(
             profile_photo=profile_photo,
             name=name,
         )
 
-        update_user_profile_multipart_data.additional_properties = d
+        update_user_profile_multipart_data.additional_properties = src_dict
         return update_user_profile_multipart_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_user_profile_response_200.py

```diff
@@ -43,35 +43,34 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.update_user_profile_response_200_data import UpdateUserProfileResponse200Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, UpdateUserProfileResponse200Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = UpdateUserProfileResponse200Status(_status)
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, UpdateUserProfileResponse200Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = UpdateUserProfileResponse200Data.from_dict(_data)
 
         update_user_profile_response_200 = cls(
             status=status,
             data=data,
         )
 
-        update_user_profile_response_200.additional_properties = d
+        update_user_profile_response_200.additional_properties = src_dict
         return update_user_profile_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_user_profile_response_200_data.py

```diff
@@ -59,31 +59,30 @@
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _created_at = d.pop("created_at", UNSET)
+        _created_at = src_dict.get("created_at")
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
-        email = d.pop("email", UNSET)
+        email = src_dict.get("email")
 
-        id = d.pop("id", UNSET)
+        id = src_dict.get("id")
 
-        name = d.pop("name", UNSET)
+        name = src_dict.get("name")
 
-        profile_photo_url = d.pop("profile_photo_url", UNSET)
+        profile_photo_url = src_dict.get("profile_photo_url")
 
-        _updated_at = d.pop("updated_at", UNSET)
+        _updated_at = src_dict.get("updated_at")
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         update_user_profile_response_200_data = cls(
@@ -91,15 +90,15 @@
             email=email,
             id=id,
             name=name,
             profile_photo_url=profile_photo_url,
             updated_at=updated_at,
         )
 
-        update_user_profile_response_200_data.additional_properties = d
+        update_user_profile_response_200_data.additional_properties = src_dict
         return update_user_profile_response_200_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_user_profile_response_401.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.update_user_profile_response_401_data import UpdateUserProfileResponse401Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, UpdateUserProfileResponse401Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = UpdateUserProfileResponse401Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, UpdateUserProfileResponse401Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = UpdateUserProfileResponse401Data.from_dict(_data)
 
         update_user_profile_response_401 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        update_user_profile_response_401.additional_properties = d
+        update_user_profile_response_401.additional_properties = src_dict
         return update_user_profile_response_401
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_user_profile_response_401_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, UpdateUserProfileResponse401DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = UpdateUserProfileResponse401DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         update_user_profile_response_401_data = cls(
             code=code,
             message=message,
         )
 
-        update_user_profile_response_401_data.additional_properties = d
+        update_user_profile_response_401_data.additional_properties = src_dict
         return update_user_profile_response_401_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_user_profile_response_500.py

```diff
@@ -48,38 +48,37 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.update_user_profile_response_500_data import UpdateUserProfileResponse500Data
 
-        d = src_dict.copy()
-        _status = d.pop("status", UNSET)
+        _status = src_dict.get("status")
         status: Union[Unset, UpdateUserProfileResponse500Status]
         if isinstance(_status, Unset):
             status = UNSET
         else:
             status = UpdateUserProfileResponse500Status(_status)
 
-        url = d.pop("url", UNSET)
+        url = src_dict.get("url")
 
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         data: Union[Unset, UpdateUserProfileResponse500Data]
         if isinstance(_data, Unset):
             data = UNSET
         else:
             data = UpdateUserProfileResponse500Data.from_dict(_data)
 
         update_user_profile_response_500 = cls(
             status=status,
             url=url,
             data=data,
         )
 
-        update_user_profile_response_500.additional_properties = d
+        update_user_profile_response_500.additional_properties = src_dict
         return update_user_profile_response_500
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/update_user_profile_response_500_data.py

```diff
@@ -35,30 +35,29 @@
         if message is not UNSET:
             field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _code = d.pop("code", UNSET)
+        _code = src_dict.get("code")
         code: Union[Unset, UpdateUserProfileResponse500DataCode]
         if isinstance(_code, Unset):
             code = UNSET
         else:
             code = UpdateUserProfileResponse500DataCode(_code)
 
-        message = d.pop("message", UNSET)
+        message = src_dict.get("message")
 
         update_user_profile_response_500_data = cls(
             code=code,
             message=message,
         )
 
-        update_user_profile_response_500_data.additional_properties = d
+        update_user_profile_response_500_data.additional_properties = src_dict
         return update_user_profile_response_500_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## customgpt_client/models/user.py

```diff
@@ -59,31 +59,30 @@
         if updated_at is not UNSET:
             field_dict["updated_at"] = updated_at
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _created_at = d.pop("created_at", UNSET)
+        _created_at = src_dict.get("created_at")
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
-        email = d.pop("email", UNSET)
+        email = src_dict.get("email")
 
-        id = d.pop("id", UNSET)
+        id = src_dict.get("id")
 
-        name = d.pop("name", UNSET)
+        name = src_dict.get("name")
 
-        profile_photo_url = d.pop("profile_photo_url", UNSET)
+        profile_photo_url = src_dict.get("profile_photo_url")
 
-        _updated_at = d.pop("updated_at", UNSET)
+        _updated_at = src_dict.get("updated_at")
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
         user = cls(
@@ -91,15 +90,15 @@
             email=email,
             id=id,
             name=name,
             profile_photo_url=profile_photo_url,
             updated_at=updated_at,
         )
 
-        user.additional_properties = d
+        user.additional_properties = src_dict
         return user
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
```

## Comparing `customgpt_client/models/get_project_conversations_response_200_data_links.py` & `customgpt_client/models/delete_project_source_response_500.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,85 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
+from ..models.delete_project_source_response_500_status import DeleteProjectSourceResponse500Status
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="GetProjectConversationsResponse200DataLinks")
+if TYPE_CHECKING:
+    from ..models.delete_project_source_response_500_data import DeleteProjectSourceResponse500Data
+
+
+T = TypeVar("T", bound="DeleteProjectSourceResponse500")
 
 
 @attr.s(auto_attribs=True)
-class GetProjectConversationsResponse200DataLinks:
+class DeleteProjectSourceResponse500:
     """
     Attributes:
-        first (Union[Unset, str]): The first page url Example: https://app.customgpt.ai/api/v1/users?page=1.
-        last (Union[Unset, str]): The last page url Example: https://app.customgpt.ai/api/v1/users?page=1.
-        prev (Union[Unset, str]): The previous page url Example: https://app.customgpt.ai/api/v1/users?page=1.
-        next_ (Union[Unset, str]): The next page url Example: https://app.customgpt.ai/api/v1/users?page=1.
+        status (Union[Unset, DeleteProjectSourceResponse500Status]): The status of the response Example: error.
+        url (Union[Unset, str]): The URL of the request Example: https://app.customgpt.ai/api/v1/projects/1.
+        data (Union[Unset, DeleteProjectSourceResponse500Data]):
     """
 
-    first: Union[Unset, str] = UNSET
-    last: Union[Unset, str] = UNSET
-    prev: Union[Unset, str] = UNSET
-    next_: Union[Unset, str] = UNSET
+    status: Union[Unset, DeleteProjectSourceResponse500Status] = UNSET
+    url: Union[Unset, str] = UNSET
+    data: Union[Unset, "DeleteProjectSourceResponse500Data"] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        first = self.first
-        last = self.last
-        prev = self.prev
-        next_ = self.next_
+        status: Union[Unset, str] = UNSET
+        if not isinstance(self.status, Unset):
+            status = self.status.value
+
+        url = self.url
+        data: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.data, Unset):
+            data = self.data.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if first is not UNSET:
-            field_dict["first"] = first
-        if last is not UNSET:
-            field_dict["last"] = last
-        if prev is not UNSET:
-            field_dict["prev"] = prev
-        if next_ is not UNSET:
-            field_dict["next"] = next_
+        if status is not UNSET:
+            field_dict["status"] = status
+        if url is not UNSET:
+            field_dict["url"] = url
+        if data is not UNSET:
+            field_dict["data"] = data
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        first = d.pop("first", UNSET)
-
-        last = d.pop("last", UNSET)
-
-        prev = d.pop("prev", UNSET)
-
-        next_ = d.pop("next", UNSET)
+        from ..models.delete_project_source_response_500_data import DeleteProjectSourceResponse500Data
 
-        get_project_conversations_response_200_data_links = cls(
-            first=first,
-            last=last,
-            prev=prev,
-            next_=next_,
+        _status = src_dict.get("status")
+        status: Union[Unset, DeleteProjectSourceResponse500Status]
+        if isinstance(_status, Unset):
+            status = UNSET
+        else:
+            status = DeleteProjectSourceResponse500Status(_status)
+
+        url = src_dict.get("url")
+
+        _data = src_dict.get("data")
+        data: Union[Unset, DeleteProjectSourceResponse500Data]
+        if isinstance(_data, Unset):
+            data = UNSET
+        else:
+            data = DeleteProjectSourceResponse500Data.from_dict(_data)
+
+        delete_project_source_response_500 = cls(
+            status=status,
+            url=url,
+            data=data,
         )
 
-        get_project_conversations_response_200_data_links.additional_properties = d
-        return get_project_conversations_response_200_data_links
+        delete_project_source_response_500.additional_properties = src_dict
+        return delete_project_source_response_500
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

## Comparing `customgpt_client/models/get_project_pages_response_200_data_pages_links.py` & `customgpt_client/models/list_project_sources_response_500_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,64 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
+from ..models.list_project_sources_response_500_data_code import ListProjectSourcesResponse500DataCode
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="GetProjectPagesResponse200DataPagesLinks")
+T = TypeVar("T", bound="ListProjectSourcesResponse500Data")
 
 
 @attr.s(auto_attribs=True)
-class GetProjectPagesResponse200DataPagesLinks:
+class ListProjectSourcesResponse500Data:
     """
     Attributes:
-        first (Union[Unset, str]): The first page url Example: https://app.customgpt.ai/api/v1/users?page=1.
-        last (Union[Unset, str]): The last page url Example: https://app.customgpt.ai/api/v1/users?page=1.
-        prev (Union[Unset, str]): The previous page url Example: https://app.customgpt.ai/api/v1/users?page=1.
-        next_ (Union[Unset, str]): The next page url Example: https://app.customgpt.ai/api/v1/users?page=1.
+        code (Union[Unset, ListProjectSourcesResponse500DataCode]): The error status code Example: 500.
+        message (Union[Unset, str]):  Example: Internal Server Error.
     """
 
-    first: Union[Unset, str] = UNSET
-    last: Union[Unset, str] = UNSET
-    prev: Union[Unset, str] = UNSET
-    next_: Union[Unset, str] = UNSET
+    code: Union[Unset, ListProjectSourcesResponse500DataCode] = UNSET
+    message: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        first = self.first
-        last = self.last
-        prev = self.prev
-        next_ = self.next_
+        code: Union[Unset, int] = UNSET
+        if not isinstance(self.code, Unset):
+            code = self.code.value
+
+        message = self.message
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if first is not UNSET:
-            field_dict["first"] = first
-        if last is not UNSET:
-            field_dict["last"] = last
-        if prev is not UNSET:
-            field_dict["prev"] = prev
-        if next_ is not UNSET:
-            field_dict["next"] = next_
+        if code is not UNSET:
+            field_dict["code"] = code
+        if message is not UNSET:
+            field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        first = d.pop("first", UNSET)
-
-        last = d.pop("last", UNSET)
-
-        prev = d.pop("prev", UNSET)
-
-        next_ = d.pop("next", UNSET)
-
-        get_project_pages_response_200_data_pages_links = cls(
-            first=first,
-            last=last,
-            prev=prev,
-            next_=next_,
+        _code = src_dict.get("code")
+        code: Union[Unset, ListProjectSourcesResponse500DataCode]
+        if isinstance(_code, Unset):
+            code = UNSET
+        else:
+            code = ListProjectSourcesResponse500DataCode(_code)
+
+        message = src_dict.get("message")
+
+        list_project_sources_response_500_data = cls(
+            code=code,
+            message=message,
         )
 
-        get_project_pages_response_200_data_pages_links.additional_properties = d
-        return get_project_pages_response_200_data_pages_links
+        list_project_sources_response_500_data.additional_properties = src_dict
+        return list_project_sources_response_500_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

## Comparing `customgpt_client/models/list_projects_response_200_data_links.py` & `customgpt_client/models/create_project_source_response_500.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,85 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
+from ..models.create_project_source_response_500_status import CreateProjectSourceResponse500Status
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ListProjectsResponse200DataLinks")
+if TYPE_CHECKING:
+    from ..models.create_project_source_response_500_data import CreateProjectSourceResponse500Data
+
+
+T = TypeVar("T", bound="CreateProjectSourceResponse500")
 
 
 @attr.s(auto_attribs=True)
-class ListProjectsResponse200DataLinks:
+class CreateProjectSourceResponse500:
     """
     Attributes:
-        first (Union[Unset, str]): The first page url Example: https://app.customgpt.ai/api/v1/users?page=1.
-        last (Union[Unset, str]): The last page url Example: https://app.customgpt.ai/api/v1/users?page=1.
-        prev (Union[Unset, str]): The previous page url Example: https://app.customgpt.ai/api/v1/users?page=1.
-        next_ (Union[Unset, str]): The next page url Example: https://app.customgpt.ai/api/v1/users?page=1.
+        status (Union[Unset, CreateProjectSourceResponse500Status]): The status of the response Example: error.
+        url (Union[Unset, str]): The URL of the request Example: https://app.customgpt.ai/api/v1/projects/1.
+        data (Union[Unset, CreateProjectSourceResponse500Data]):
     """
 
-    first: Union[Unset, str] = UNSET
-    last: Union[Unset, str] = UNSET
-    prev: Union[Unset, str] = UNSET
-    next_: Union[Unset, str] = UNSET
+    status: Union[Unset, CreateProjectSourceResponse500Status] = UNSET
+    url: Union[Unset, str] = UNSET
+    data: Union[Unset, "CreateProjectSourceResponse500Data"] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        first = self.first
-        last = self.last
-        prev = self.prev
-        next_ = self.next_
+        status: Union[Unset, str] = UNSET
+        if not isinstance(self.status, Unset):
+            status = self.status.value
+
+        url = self.url
+        data: Union[Unset, Dict[str, Any]] = UNSET
+        if not isinstance(self.data, Unset):
+            data = self.data.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if first is not UNSET:
-            field_dict["first"] = first
-        if last is not UNSET:
-            field_dict["last"] = last
-        if prev is not UNSET:
-            field_dict["prev"] = prev
-        if next_ is not UNSET:
-            field_dict["next"] = next_
+        if status is not UNSET:
+            field_dict["status"] = status
+        if url is not UNSET:
+            field_dict["url"] = url
+        if data is not UNSET:
+            field_dict["data"] = data
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        first = d.pop("first", UNSET)
-
-        last = d.pop("last", UNSET)
-
-        prev = d.pop("prev", UNSET)
-
-        next_ = d.pop("next", UNSET)
+        from ..models.create_project_source_response_500_data import CreateProjectSourceResponse500Data
 
-        list_projects_response_200_data_links = cls(
-            first=first,
-            last=last,
-            prev=prev,
-            next_=next_,
+        _status = src_dict.get("status")
+        status: Union[Unset, CreateProjectSourceResponse500Status]
+        if isinstance(_status, Unset):
+            status = UNSET
+        else:
+            status = CreateProjectSourceResponse500Status(_status)
+
+        url = src_dict.get("url")
+
+        _data = src_dict.get("data")
+        data: Union[Unset, CreateProjectSourceResponse500Data]
+        if isinstance(_data, Unset):
+            data = UNSET
+        else:
+            data = CreateProjectSourceResponse500Data.from_dict(_data)
+
+        create_project_source_response_500 = cls(
+            status=status,
+            url=url,
+            data=data,
         )
 
-        list_projects_response_200_data_links.additional_properties = d
-        return list_projects_response_200_data_links
+        create_project_source_response_500.additional_properties = src_dict
+        return create_project_source_response_500
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

## Comparing `customgpt_client/models/messages_response_200_conversation.py` & `customgpt_client/models/messages_response_200_data_conversation.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,34 +2,35 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="MessagesResponse200Conversation")
+T = TypeVar("T", bound="MessagesResponse200DataConversation")
 
 
 @attr.s(auto_attribs=True)
-class MessagesResponse200Conversation:
+class MessagesResponse200DataConversation:
     """
     Attributes:
         created_at (Union[Unset, datetime.datetime]): When was this conversation created? Example: 2023-04-30 16:43:53.
         updated_at (Union[Unset, datetime.datetime]): When was this conversation updated? Example: 2023-04-30 16:43:53.
-        deleted_at (Union[Unset, datetime.datetime]): When was this conversation deleted? Example: 2023-04-30 16:43:53.
+        deleted_at (Union[Unset, None, datetime.datetime]): When was this conversation deleted? Example: 2023-04-30
+            16:43:53.
         id (Union[Unset, int]): Conversation ID Example: 1.
         name (Union[Unset, str]): Conversation name Example: Conversation 1.
         project_id (Union[Unset, str]): Project ID for this conversation Example: 1.
         created_by (Union[Unset, str]): User ID for the user who created this conversation Example: 1.
         session_id (Union[Unset, str]): Session ID for this conversation Example: f1b9aaf0-5e4e-11eb-ae93-0242ac130002.
     """
 
     created_at: Union[Unset, datetime.datetime] = UNSET
     updated_at: Union[Unset, datetime.datetime] = UNSET
-    deleted_at: Union[Unset, datetime.datetime] = UNSET
+    deleted_at: Union[Unset, None, datetime.datetime] = UNSET
     id: Union[Unset, int] = UNSET
     name: Union[Unset, str] = UNSET
     project_id: Union[Unset, str] = UNSET
     created_by: Union[Unset, str] = UNSET
     session_id: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
@@ -38,17 +39,17 @@
         if not isinstance(self.created_at, Unset):
             created_at = self.created_at.isoformat()
 
         updated_at: Union[Unset, str] = UNSET
         if not isinstance(self.updated_at, Unset):
             updated_at = self.updated_at.isoformat()
 
-        deleted_at: Union[Unset, str] = UNSET
+        deleted_at: Union[Unset, None, str] = UNSET
         if not isinstance(self.deleted_at, Unset):
-            deleted_at = self.deleted_at.isoformat()
+            deleted_at = self.deleted_at.isoformat() if self.deleted_at else None
 
         id = self.id
         name = self.name
         project_id = self.project_id
         created_by = self.created_by
         session_id = self.session_id
 
@@ -72,59 +73,60 @@
         if session_id is not UNSET:
             field_dict["session_id"] = session_id
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _created_at = d.pop("created_at", UNSET)
+        _created_at = src_dict.get("created_at")
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
-        _updated_at = d.pop("updated_at", UNSET)
+        _updated_at = src_dict.get("updated_at")
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
-        _deleted_at = d.pop("deleted_at", UNSET)
-        deleted_at: Union[Unset, datetime.datetime]
-        if isinstance(_deleted_at, Unset):
+        _deleted_at = src_dict.get("deleted_at")
+        deleted_at: Union[Unset, None, datetime.datetime]
+        if _deleted_at is None:
+            deleted_at = None
+        elif isinstance(_deleted_at, Unset):
             deleted_at = UNSET
         else:
             deleted_at = isoparse(_deleted_at)
 
-        id = d.pop("id", UNSET)
+        id = src_dict.get("id")
 
-        name = d.pop("name", UNSET)
+        name = src_dict.get("name")
 
-        project_id = d.pop("project_id", UNSET)
+        project_id = src_dict.get("project_id")
 
-        created_by = d.pop("created_by", UNSET)
+        created_by = src_dict.get("created_by")
 
-        session_id = d.pop("session_id", UNSET)
+        session_id = src_dict.get("session_id")
 
-        messages_response_200_conversation = cls(
+        messages_response_200_data_conversation = cls(
             created_at=created_at,
             updated_at=updated_at,
             deleted_at=deleted_at,
             id=id,
             name=name,
             project_id=project_id,
             created_by=created_by,
             session_id=session_id,
         )
 
-        messages_response_200_conversation.additional_properties = d
-        return messages_response_200_conversation
+        messages_response_200_data_conversation.additional_properties = src_dict
+        return messages_response_200_data_conversation
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

## Comparing `customgpt_client/models/messages_response_200_messages.py` & `customgpt_client/models/messages_response_200_data_messages.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,44 @@
 from typing import TYPE_CHECKING, Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
 if TYPE_CHECKING:
-    from ..models.messages_response_200_messages_data_item import MessagesResponse200MessagesDataItem
-    from ..models.messages_response_200_messages_links import MessagesResponse200MessagesLinks
+    from ..models.messages_response_200_data_messages_data_item import MessagesResponse200DataMessagesDataItem
 
 
-T = TypeVar("T", bound="MessagesResponse200Messages")
+T = TypeVar("T", bound="MessagesResponse200DataMessages")
 
 
 @attr.s(auto_attribs=True)
-class MessagesResponse200Messages:
+class MessagesResponse200DataMessages:
     """
     Attributes:
         current_page (Union[Unset, int]): The current page number Example: 1.
-        data (Union[Unset, List['MessagesResponse200MessagesDataItem']]):
+        data (Union[Unset, List['MessagesResponse200DataMessagesDataItem']]):
         first_page_url (Union[Unset, str]): The first page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         from_ (Union[Unset, int]): The first item number of the current page Example: 1.
         last_page (Union[Unset, int]): The last page number Example: 1.
         last_page_url (Union[Unset, str]): The last page url Example: https://app.customgpt.ai/api/v1/users?page=1.
-        links (Union[Unset, MessagesResponse200MessagesLinks]):
         next_page_url (Union[Unset, str]): The next page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         path (Union[Unset, str]): The current page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         per_page (Union[Unset, int]): The number of items per page Example: 10.
         prev_page_url (Union[Unset, str]): The previous page url Example: https://app.customgpt.ai/api/v1/users?page=1.
         to (Union[Unset, int]): The last item number of the current page Example: 1.
         total (Union[Unset, int]): The total number of items Example: 1.
     """
 
     current_page: Union[Unset, int] = UNSET
-    data: Union[Unset, List["MessagesResponse200MessagesDataItem"]] = UNSET
+    data: Union[Unset, List["MessagesResponse200DataMessagesDataItem"]] = UNSET
     first_page_url: Union[Unset, str] = UNSET
     from_: Union[Unset, int] = UNSET
     last_page: Union[Unset, int] = UNSET
     last_page_url: Union[Unset, str] = UNSET
-    links: Union[Unset, "MessagesResponse200MessagesLinks"] = UNSET
     next_page_url: Union[Unset, str] = UNSET
     path: Union[Unset, str] = UNSET
     per_page: Union[Unset, int] = UNSET
     prev_page_url: Union[Unset, str] = UNSET
     to: Union[Unset, int] = UNSET
     total: Union[Unset, int] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
@@ -56,18 +53,14 @@
 
                 data.append(data_item)
 
         first_page_url = self.first_page_url
         from_ = self.from_
         last_page = self.last_page
         last_page_url = self.last_page_url
-        links: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.links, Unset):
-            links = self.links.to_dict()
-
         next_page_url = self.next_page_url
         path = self.path
         per_page = self.per_page
         prev_page_url = self.prev_page_url
         to = self.to
         total = self.total
 
@@ -83,16 +76,14 @@
             field_dict["first_page_url"] = first_page_url
         if from_ is not UNSET:
             field_dict["from"] = from_
         if last_page is not UNSET:
             field_dict["last_page"] = last_page
         if last_page_url is not UNSET:
             field_dict["last_page_url"] = last_page_url
-        if links is not UNSET:
-            field_dict["links"] = links
         if next_page_url is not UNSET:
             field_dict["next_page_url"] = next_page_url
         if path is not UNSET:
             field_dict["path"] = path
         if per_page is not UNSET:
             field_dict["per_page"] = per_page
         if prev_page_url is not UNSET:
@@ -102,72 +93,62 @@
         if total is not UNSET:
             field_dict["total"] = total
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.messages_response_200_messages_data_item import MessagesResponse200MessagesDataItem
-        from ..models.messages_response_200_messages_links import MessagesResponse200MessagesLinks
+        from ..models.messages_response_200_data_messages_data_item import MessagesResponse200DataMessagesDataItem
 
-        d = src_dict.copy()
-        current_page = d.pop("current_page", UNSET)
+        current_page = src_dict.get("current_page")
 
         data = []
-        _data = d.pop("data", UNSET)
+        _data = src_dict.get("data")
         for data_item_data in _data or []:
-            data_item = MessagesResponse200MessagesDataItem.from_dict(data_item_data)
+            data_item = MessagesResponse200DataMessagesDataItem.from_dict(data_item_data)
 
             data.append(data_item)
 
-        first_page_url = d.pop("first_page_url", UNSET)
-
-        from_ = d.pop("from", UNSET)
+        first_page_url = src_dict.get("first_page_url")
 
-        last_page = d.pop("last_page", UNSET)
+        from_ = src_dict.get("from")
 
-        last_page_url = d.pop("last_page_url", UNSET)
+        last_page = src_dict.get("last_page")
 
-        _links = d.pop("links", UNSET)
-        links: Union[Unset, MessagesResponse200MessagesLinks]
-        if isinstance(_links, Unset):
-            links = UNSET
-        else:
-            links = MessagesResponse200MessagesLinks.from_dict(_links)
+        last_page_url = src_dict.get("last_page_url")
 
-        next_page_url = d.pop("next_page_url", UNSET)
+        next_page_url = src_dict.get("next_page_url")
 
-        path = d.pop("path", UNSET)
+        path = src_dict.get("path")
 
-        per_page = d.pop("per_page", UNSET)
+        per_page = src_dict.get("per_page")
 
-        prev_page_url = d.pop("prev_page_url", UNSET)
+        prev_page_url = src_dict.get("prev_page_url")
 
-        to = d.pop("to", UNSET)
+        to = src_dict.get("to")
 
-        total = d.pop("total", UNSET)
+        total = src_dict.get("total")
 
-        messages_response_200_messages = cls(
+        messages_response_200_data_messages = cls(
             current_page=current_page,
             data=data,
             first_page_url=first_page_url,
             from_=from_,
             last_page=last_page,
             last_page_url=last_page_url,
-            links=links,
             next_page_url=next_page_url,
             path=path,
             per_page=per_page,
             prev_page_url=prev_page_url,
             to=to,
             total=total,
         )
 
-        messages_response_200_messages.additional_properties = d
-        return messages_response_200_messages
+        messages_response_200_data_messages.additional_properties = src_dict
+        return messages_response_200_data_messages
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

## Comparing `customgpt_client/models/messages_response_200_messages_data_item.py` & `customgpt_client/models/messages_response_200_data_messages_data_item.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from typing import Any, Dict, List, Type, TypeVar, Union, cast
 
 import attr
 from dateutil.parser import isoparse
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="MessagesResponse200MessagesDataItem")
+T = TypeVar("T", bound="MessagesResponse200DataMessagesDataItem")
 
 
 @attr.s(auto_attribs=True)
-class MessagesResponse200MessagesDataItem:
+class MessagesResponse200DataMessagesDataItem:
     """
     Attributes:
         id (Union[Unset, int]): The unique identifier of the prompt history. Example: 1.
         user_id (Union[Unset, int]): The unique identifier of the user. Example: 1.
         user_query (Union[Unset, str]): The user prompt query. Example: What is the meaning of life?.
         openai_response (Union[Unset, str]): The OpenAI response to the user prompt query. Example: The meaning of life
             is to be happy..
@@ -75,54 +75,53 @@
             for index, field_value in enumerate(citations):
                 field_dict[f"citations[]{index}"] = field_value
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        id = d.pop("id", UNSET)
+        id = src_dict.get("id")
 
-        user_id = d.pop("user_id", UNSET)
+        user_id = src_dict.get("user_id")
 
-        user_query = d.pop("user_query", UNSET)
+        user_query = src_dict.get("user_query")
 
-        openai_response = d.pop("openai_response", UNSET)
+        openai_response = src_dict.get("openai_response")
 
-        _created_at = d.pop("created_at", UNSET)
+        _created_at = src_dict.get("created_at")
         created_at: Union[Unset, datetime.datetime]
         if isinstance(_created_at, Unset):
             created_at = UNSET
         else:
             created_at = isoparse(_created_at)
 
-        _updated_at = d.pop("updated_at", UNSET)
+        _updated_at = src_dict.get("updated_at")
         updated_at: Union[Unset, datetime.datetime]
         if isinstance(_updated_at, Unset):
             updated_at = UNSET
         else:
             updated_at = isoparse(_updated_at)
 
-        conversation_id = d.pop("conversation_id", UNSET)
+        conversation_id = src_dict.get("conversation_id")
 
-        citations = cast(List[int], d.pop("citations", UNSET))
+        citations = cast(List[int], src_dict.get("citations"))
 
-        messages_response_200_messages_data_item = cls(
+        messages_response_200_data_messages_data_item = cls(
             id=id,
             user_id=user_id,
             user_query=user_query,
             openai_response=openai_response,
             created_at=created_at,
             updated_at=updated_at,
             conversation_id=conversation_id,
             citations=citations,
         )
 
-        messages_response_200_messages_data_item.additional_properties = d
-        return messages_response_200_messages_data_item
+        messages_response_200_data_messages_data_item.additional_properties = src_dict
+        return messages_response_200_data_messages_data_item
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

## Comparing `customgpt_client/models/messages_response_200_messages_links.py` & `customgpt_client/models/create_project_source_response_401_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,64 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
+from ..models.create_project_source_response_401_data_code import CreateProjectSourceResponse401DataCode
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="MessagesResponse200MessagesLinks")
+T = TypeVar("T", bound="CreateProjectSourceResponse401Data")
 
 
 @attr.s(auto_attribs=True)
-class MessagesResponse200MessagesLinks:
+class CreateProjectSourceResponse401Data:
     """
     Attributes:
-        first (Union[Unset, str]): The first page url Example: https://app.customgpt.ai/api/v1/users?page=1.
-        last (Union[Unset, str]): The last page url Example: https://app.customgpt.ai/api/v1/users?page=1.
-        prev (Union[Unset, str]): The previous page url Example: https://app.customgpt.ai/api/v1/users?page=1.
-        next_ (Union[Unset, str]): The next page url Example: https://app.customgpt.ai/api/v1/users?page=1.
+        code (Union[Unset, CreateProjectSourceResponse401DataCode]): The error status code Example: 401.
+        message (Union[Unset, str]):  Example: API Token is either missing or invalid.
     """
 
-    first: Union[Unset, str] = UNSET
-    last: Union[Unset, str] = UNSET
-    prev: Union[Unset, str] = UNSET
-    next_: Union[Unset, str] = UNSET
+    code: Union[Unset, CreateProjectSourceResponse401DataCode] = UNSET
+    message: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        first = self.first
-        last = self.last
-        prev = self.prev
-        next_ = self.next_
+        code: Union[Unset, int] = UNSET
+        if not isinstance(self.code, Unset):
+            code = self.code.value
+
+        message = self.message
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        if first is not UNSET:
-            field_dict["first"] = first
-        if last is not UNSET:
-            field_dict["last"] = last
-        if prev is not UNSET:
-            field_dict["prev"] = prev
-        if next_ is not UNSET:
-            field_dict["next"] = next_
+        if code is not UNSET:
+            field_dict["code"] = code
+        if message is not UNSET:
+            field_dict["message"] = message
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        first = d.pop("first", UNSET)
-
-        last = d.pop("last", UNSET)
-
-        prev = d.pop("prev", UNSET)
-
-        next_ = d.pop("next", UNSET)
-
-        messages_response_200_messages_links = cls(
-            first=first,
-            last=last,
-            prev=prev,
-            next_=next_,
+        _code = src_dict.get("code")
+        code: Union[Unset, CreateProjectSourceResponse401DataCode]
+        if isinstance(_code, Unset):
+            code = UNSET
+        else:
+            code = CreateProjectSourceResponse401DataCode(_code)
+
+        message = src_dict.get("message")
+
+        create_project_source_response_401_data = cls(
+            code=code,
+            message=message,
         )
 
-        messages_response_200_messages_links.additional_properties = d
-        return messages_response_200_messages_links
+        create_project_source_response_401_data.additional_properties = src_dict
+        return create_project_source_response_401_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

## Comparing `customgpt_client-1.1.2.dist-info/METADATA` & `customgpt_client-1.1.3.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: customgpt-client
-Version: 1.1.2
+Version: 1.1.3
 Summary: A client library for accessing customgpt
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=21.3.0)
-Requires-Dist: httpx (>=0.15.4,<0.25.0)
 Requires-Dist: python-dateutil (>=2.8.0,<3.0.0)
+Requires-Dist: sseclient-py (==1.7.2)
 Description-Content-Type: text/markdown
 
 # CustomGPT SDK
 
 ## Usage
 First, create a client:
```

## Comparing `customgpt_client-1.1.2.dist-info/RECORD` & `customgpt_client-1.1.3.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,376 +1,505 @@
 customgpt_client/__init__.py,sha256=hA1KHzu3u-PQ5zh9yOG0np6ZsEYjw9bs_aeGCsfZZbc,105
 customgpt_client/api/__init__.py,sha256=87ApBzKyGb5zsgTMOkQXDqsLZCmaSFoJMwbGzCDQZMw,47
 customgpt_client/api/citations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-customgpt_client/api/citations/get_open_graph_data_for_citation.py,sha256=LEqhCbvID3yLZcATz958exB2l_GCbHlqMOGuD7HNTp8,6513
+customgpt_client/api/citations/get_open_graph_data_for_citation.py,sha256=r1B_QHRhMwCByl8BMS7uUt6thCYilFQHC6BlWFa-1p0,5868
 customgpt_client/api/conversations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-customgpt_client/api/conversations/create_project_conversation.py,sha256=JLvtGNfBxHGwLiphetuBbQMzDCwM6r_7OzGu3y525tQ,7370
-customgpt_client/api/conversations/delete_project_conversation.py,sha256=jCoilmEkPFBKCf3aUAFw08oMGHwHjmVAzPIQqYLVqbU,6970
-customgpt_client/api/conversations/get_project_conversations.py,sha256=o4fXGDnZhbHxUK5zXCPNYetYUH1t8RuSf4IoU87k5OE,8648
-customgpt_client/api/conversations/messages.py,sha256=moepVvCLdm87tQgoRq6snDI--FN115qiRrAwcxuQhY0,8015
-customgpt_client/api/conversations/send_message_to_conversation.py,sha256=_WQO4SKSMc5RdZ0eFQlJKBPYPQZX5sBDRGrG4NLRaMQ,12846
-customgpt_client/api/conversations/update_project_conversation.py,sha256=vEueOTUh86Mz2DfPrAmBC1UBI-9ho7OYTJrYxWZeEoE,7725
+customgpt_client/api/conversations/create_project_conversation.py,sha256=4e9aEdSF4MuzDeGLLMW_Q27ThY_zDlPIvG_b1VbqCY8,6697
+customgpt_client/api/conversations/delete_project_conversation.py,sha256=hMZmyaMAx6XT3UF0EhTKq51rXpU8eXwRiyen5pop57w,6332
+customgpt_client/api/conversations/get_project_conversations.py,sha256=RyafymnxTb69aNFT1ltxfbTjIbC41g2EzBELrIksiMo,7825
+customgpt_client/api/conversations/messages.py,sha256=BAUxmlsPFTgUNrcae-TeuSpvoP9Cm57zWoruSkdU99Q,7199
+customgpt_client/api/conversations/send_message_to_conversation.py,sha256=X0bWDu2Cz-mN9G1o32Z7b5432yLH-F1_gH4E-efuQsY,8580
+customgpt_client/api/conversations/update_project_conversation.py,sha256=wyXGBrSG9pv4o7e4EH0v_ejkr3vs1JSfVTLVOUn7C2Y,7032
 customgpt_client/api/pages/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-customgpt_client/api/pages/delete_project_page.py,sha256=p0_lLDjGvn8P3Y4vbWSamMYxl7ySxM_HX4-IYnVsK1w,6716
-customgpt_client/api/pages/get_project_pages.py,sha256=FQNZVyRLYe7WGOYeN-MAxxjpld1uuApj-jxrMNne9_g,8458
-customgpt_client/api/pages/preview.py,sha256=f5hCz1niwbG9ysYXfbTW49iiJOVPUmLaduX8pdjzevU,4706
+customgpt_client/api/pages/delete_project_page.py,sha256=rRkrUYa-LLOgY0kWL1qW01MYC-E_zJiqoMvyMhhBVAU,6060
+customgpt_client/api/pages/get_project_pages.py,sha256=2bDww3UDOkZwIZKiPyztAPfIsk7eXUMI8o-ydGuTUpU,7653
+customgpt_client/api/pages/preview.py,sha256=3Gn23FA0_7DRATY4AAw3c5YouQLXHZAePg-rSLy5NBE,4239
+customgpt_client/api/project_plugins/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+customgpt_client/api/project_plugins/create_project_plugin.py,sha256=X7VbcMCZ9z6HwGs6ZwMyJjgaiO1Won5-L-VMcfMsIqQ,6346
+customgpt_client/api/project_plugins/get_project_plugins.py,sha256=Heiz6fKEKFNAkXTgMoOlUJoZa94Y9I_9T36yFgbhIE4,5618
+customgpt_client/api/project_plugins/update_project_plugin.py,sha256=L98HcfMlUwl-C2kbR6N8FeTfwCh3XExFvJED1Uazx30,6319
 customgpt_client/api/project_settings/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-customgpt_client/api/project_settings/get_project_settings.py,sha256=ufuGyw4PWvE1mAYxgZl2022hswaSq62oman6k_RhQzc,6233
-customgpt_client/api/project_settings/update_project_settings.py,sha256=58WxRwZH5TXSC7_gjNTMVlOZ9ewGyeKtA6QFq-utbW0,7313
+customgpt_client/api/project_settings/get_project_settings.py,sha256=NIMZG9xF_Nmeew6XdgbWzXezDi2KdoAJah_tL_ONb1w,5651
+customgpt_client/api/project_settings/update_project_settings.py,sha256=VIpIHClrAVUsaOKyOSuUVrC_1HdCzpv8SGwyPgsU6TQ,6646
 customgpt_client/api/projects/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-customgpt_client/api/projects/create_project.py,sha256=j2m5dxnuOpk60Bw8lCue57yi_dTz9mG0WGoVanvf1Cg,6242
-customgpt_client/api/projects/delete_project.py,sha256=j2zMM8N3PqbUMgy9bxw6encTr4sgwScfV6Rm8BlBPwc,5760
-customgpt_client/api/projects/get_project.py,sha256=gbiUsQ83uFXTmdH8kOdyPsMlOh4bHGGMYncDYwHTT3Q,7074
-customgpt_client/api/projects/list_projects.py,sha256=Skxr8WOhwX3W5wN1OVFMNF_L1jA3FbAtKL2XG7sLbEA,8489
-customgpt_client/api/projects/stats_project.py,sha256=Qp0w1Gvilp53nZS7En9A5EkKOez4I66xQG-Y3apTD6U,5767
-customgpt_client/api/projects/update_project.py,sha256=Wh5cCgqwRQqTZUAmVb-wuKOuK-QY2qLkCa6sZKoAdfw,6358
+customgpt_client/api/projects/create_project.py,sha256=zs41vZoQOTf8RYAWfzlcfF5DrgGBeJCWYrWGCgI5eFc,5647
+customgpt_client/api/projects/delete_project.py,sha256=UL6L60mT816vBpQIqJT4_smxzXT6e9jMmWT_OjHE1g0,5205
+customgpt_client/api/projects/get_project.py,sha256=nipNlJNM5YksuSFmXdvH31MVWUaDEpjTUcE_5ImpwNA,6372
+customgpt_client/api/projects/list_projects.py,sha256=PPLtnIdXEkRR8jWOg-AGuUnURrOazbWz6QkeOu4Z6Oc,7625
+customgpt_client/api/projects/stats_project.py,sha256=MDfRBkBj8fSpV3-dtSFrbSDzifb7l0gQkOHJpxM9pt4,5203
+customgpt_client/api/projects/update_project.py,sha256=0q8rCji1EFTa6S3BUn45uusZlY8avnercs908e83wzA,5799
+customgpt_client/api/sources/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+customgpt_client/api/sources/create_project_source.py,sha256=LjJ2dXQuuDn0JSATMzX4kGZtA7T9D9mNQCkatkxvugM,7048
+customgpt_client/api/sources/delete_project_source.py,sha256=ZNlEwPpVFezmACiljSE6J1xmevgv2-OUyFkGFsC1ots,5998
+customgpt_client/api/sources/list_project_sources.py,sha256=r8GEUln3i4jhyZHS1lk_ukJiGOzD1YMdl8xPyi41-4E,5641
 customgpt_client/api/users/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-customgpt_client/api/users/get_user_profile.py,sha256=S8NFQIbyHuH_kYJ7_Gw9lCpAVZ55DRBAweNhtOaEUUk,4857
-customgpt_client/api/users/update_user_profile.py,sha256=tdUDOMPdOUZbFTPK8bikbRXNQ9lJTFJMqKSPfEgZJeE,5851
-customgpt_client/client.py,sha256=yZpzWt3cLt0BgfuvwzQsRioRr9pW7-g1wxhKDJ3GxCw,28543
+customgpt_client/api/users/get_user_profile.py,sha256=3GLm6aF4Ayt7iuCdhfMqcL-lm087iusAdMy8k5sHhiw,4358
+customgpt_client/api/users/update_user_profile.py,sha256=qprd9dcxoaBBS2eyqzIxuynjMN7syZOMg9ms3Aumo8U,5275
+customgpt_client/client.py,sha256=6u-vFjvyBkP6j2gOF39TL-ZLjXlasyFFXHKfZEAJJDo,17457
 customgpt_client/errors.py,sha256=8mXSxdfSGzxT82srdhYbR0fHfgenxJXaUtMkaGgb6iU,470
-customgpt_client/models/__init__.py,sha256=Q72_LR32FOZXyOjyHj8fZHuLVsevukgAqKAUmmzTElU,42317
-customgpt_client/models/conversation.py,sha256=sz1WLQepF_GYstr3pnQ932kJnm-6Yja9_iw6xmQOC2M,4878
-customgpt_client/models/create_project_conversation_json_body.py,sha256=2wm1-QMTq4K0DJj9wciyjGRrdrobqAx1uacc6XJ1Awo,1604
-customgpt_client/models/create_project_conversation_response_201.py,sha256=o8AC0Ji9tQSHBcXO37WNgkczFYkyYyeoAdWCM5StRdU,3055
-customgpt_client/models/create_project_conversation_response_201_data.py,sha256=ZqRphILiMIG-t6Wn06L87bT3FXuYJS-iGB9cQ0c_HK8,5033
+customgpt_client/models/__init__.py,sha256=hT26lWc9CTMywbBKXeQfQEdItCcPS4yv0w6CmdZtQyc,58865
+customgpt_client/models/conversation.py,sha256=2Eir_2i70aYie6G6TYOrGqp1Y55XA2HDsetznj5SEFQ,4857
+customgpt_client/models/create_project_conversation_json_body.py,sha256=nt9D7xSqH67s8KT1225PCTSuAzy0YNbowIRZFDFp1IQ,1583
+customgpt_client/models/create_project_conversation_response_201.py,sha256=Nhso-yBcBePcNgNB9i1v_rUUvclVXqyxev6Up5y-b6k,3034
+customgpt_client/models/create_project_conversation_response_201_data.py,sha256=QcD-M8j2-es5YY6_QQnxhBWWOLxcZ3c5-X4GcD9qGbo,5141
 customgpt_client/models/create_project_conversation_response_201_status.py,sha256=3hUZM4eDdpawPLFD1rYTxCtA9oSX03Ia8pzDKtwX9Po,191
-customgpt_client/models/create_project_conversation_response_401.py,sha256=TfHnjkxl7uHTpl7Gy_7cpAE66ipIZsozV5H-eO5H_tw,3341
-customgpt_client/models/create_project_conversation_response_401_data.py,sha256=0BFo7a5d4-mH4scKVc2F02u8VkAnz1S5oPs9JumQH10,2456
+customgpt_client/models/create_project_conversation_response_401.py,sha256=adp1PJVqOMMiBN_lfw-SFxDqePt33-5v76zNp-DOHM8,3320
+customgpt_client/models/create_project_conversation_response_401_data.py,sha256=tawpW0mCdAYaAoMYOkRNawuwztxNxId_37cJsrR2RLk,2435
 customgpt_client/models/create_project_conversation_response_401_data_code.py,sha256=FcT0bcjBLqW9DLm1eZz-C_I92SyILE-0hAliOmMl0Qc,270
 customgpt_client/models/create_project_conversation_response_401_status.py,sha256=-zl7ZRNvTmwXm71PGkFeq8hn3fyLrLty6pQ7LPG5D08,191
-customgpt_client/models/create_project_conversation_response_404.py,sha256=bVwB5bwLGeeEweFMiedImwZfVNeZOVf4LDamkl1L5oE,3341
-customgpt_client/models/create_project_conversation_response_404_data.py,sha256=QUEnKXsyg_6bS_JsUJmEdjTiPL-ELmOCAXdrb3zv-6w,3034
+customgpt_client/models/create_project_conversation_response_404.py,sha256=HsTzM6b7jGH1TY3QBwhXat4etR3xT2iLvHg6ayszvB0,3320
+customgpt_client/models/create_project_conversation_response_404_data.py,sha256=9iOLuRci7cCcvtbwkXBx5hyknJTOqAUPQOcd_Jhu9UI,3013
 customgpt_client/models/create_project_conversation_response_404_data_code.py,sha256=vQw3dQ947dzRg6PCKD1iXipaoSOaltPuf4sdb3kNyO4,270
 customgpt_client/models/create_project_conversation_response_404_data_message.py,sha256=DNvOhmVQVv_mZle_4Ef5cHD_z2rGLFFAkbo95IAGsFg,270
 customgpt_client/models/create_project_conversation_response_404_status.py,sha256=6MmKdGtUOkvf-ORDTZyvYjR0O79MwfUD9XlEyR1V0jI,191
-customgpt_client/models/create_project_conversation_response_500.py,sha256=hzp7KSx77kHACr4d8MYp-hXXXv35VZSU458H_Arf9c4,3341
-customgpt_client/models/create_project_conversation_response_500_data.py,sha256=56MlDop7TJysI3Q-r7TGF-S9n66RaTuxIodRblbJnGY,2439
+customgpt_client/models/create_project_conversation_response_500.py,sha256=yHa-0_8LfC8wl6vmQ5ZmuWv8sxzgxcVq3MsOyWXMFUo,3320
+customgpt_client/models/create_project_conversation_response_500_data.py,sha256=_EUi_Q2sDfyKXSI1Xt0Jz2PwJ15MOowUcJnigcRY83s,2418
 customgpt_client/models/create_project_conversation_response_500_data_code.py,sha256=zWJpAieSHqQjY4iNlCdD1l_Af0AohP6ktIZIwVP8Q6k,270
 customgpt_client/models/create_project_conversation_response_500_status.py,sha256=JcnZ6zLJcK9dypddxzwjM5A-3B32iJzRTS_jQ6f8nNg,191
-customgpt_client/models/create_project_multipart_data.py,sha256=4xSJTo0FCTHg4cDH28M2fgFeUnoNue8k9Ic4bZkflq8,4400
-customgpt_client/models/create_project_response_201.py,sha256=ztSZLXLbYalHbUsEELURt9tOkqnDHVWSq6NEeunxQAc,2821
-customgpt_client/models/create_project_response_201_data.py,sha256=lqBaAebzACWwTDJBarDKX52jPEEjpD-oJ_B99jCnc4U,8090
+customgpt_client/models/create_project_multipart_data.py,sha256=GkVljifa4dyBCg4tQCkgySkUgTyUKijgazQBXoUiuSU,4379
+customgpt_client/models/create_project_plugin_json_body.py,sha256=Fo8XZNHGteZ-P6Npw34_m7RZVGqKUYD7ya5bhtMf1Ys,3030
+customgpt_client/models/create_project_plugin_response_201.py,sha256=Z6Y8CPLPHWiN26gRZkZtaQ6Lo78Ot_aATmSbp0zmyV4,2920
+customgpt_client/models/create_project_plugin_response_201_data.py,sha256=gCV0nxqSzJnSCgVrixViaimt7lCcX8ELETp9LVDf9zI,3355
+customgpt_client/models/create_project_plugin_response_201_status.py,sha256=5TSgrHcSXAdygB0_ikE0ZNQPvjOo2yi8r1SSonPwU7o,185
+customgpt_client/models/create_project_plugin_response_401.py,sha256=O7Q3Rss_Un4qda9RGgBdLYVA6h2-oXKUIcTdY7SLR_c,3206
+customgpt_client/models/create_project_plugin_response_401_data.py,sha256=kW1EfzETwzbv36os_vYYrbI4lP-5PVMsctT93-gl6kA,2369
+customgpt_client/models/create_project_plugin_response_401_data_code.py,sha256=WrIFkaFY9pOefn8rv5Wc_Q_FOne85YKTdbWhVThMzC8,264
+customgpt_client/models/create_project_plugin_response_401_status.py,sha256=GZ0PhLHKdzsfgD4mMrvduRWNgjwCXx3rFAGdOIpm9C0,185
+customgpt_client/models/create_project_plugin_response_404.py,sha256=QTJFJn8CnyJRfrPvRMOLI43SpazLafnLUoPxdHpVxFU,3206
+customgpt_client/models/create_project_plugin_response_404_data.py,sha256=IcA3lDunN9ugqOxtS0HGCPKVLEL0sa5Ldmph6ePAmTc,2902
+customgpt_client/models/create_project_plugin_response_404_data_code.py,sha256=jG58PvoCi03t4DhX2YxLo59tfAn94dv1AApPgXYqp6E,264
+customgpt_client/models/create_project_plugin_response_404_data_message.py,sha256=pRrwriI6lABp-0PXSzXVFRMiSTJ18cG0Rxi5ZLUGxsA,264
+customgpt_client/models/create_project_plugin_response_404_status.py,sha256=icBnfPZUXBYzDbnZ7o-MAVgvbRlw0uHaSwzSApaaY7s,185
+customgpt_client/models/create_project_plugin_response_500.py,sha256=nyNS7cvoXkUpe3DhVkWtf1orOzXRQr824g6M4ZdIPVA,3206
+customgpt_client/models/create_project_plugin_response_500_data.py,sha256=MZbfGvhMENss41gcmFwWkGi6XUEWTCClHM5xaWsT0ss,2352
+customgpt_client/models/create_project_plugin_response_500_data_code.py,sha256=LfnSqD5NqSyGoG2PuGjGueccG2Bk0JvTqKt1dX38l_o,264
+customgpt_client/models/create_project_plugin_response_500_status.py,sha256=0vVi-ljeXwKme8O43onMeuSwduX0UAMyLNe99lVCaDw,185
+customgpt_client/models/create_project_response_201.py,sha256=zAWkG2jjPcMBxNM4z4CdP38dLk4xE7nFiZFFaPe_dgQ,2800
+customgpt_client/models/create_project_response_201_data.py,sha256=RVL2hz70abFd6t1HNoQC8S75kNKq2LBHTeDff19AOi4,8069
 customgpt_client/models/create_project_response_201_data_type.py,sha256=TAFCcj2gcEKxqQXRmfGnH3KV4GfHyyZygM3qVwI9mW8,177
 customgpt_client/models/create_project_response_201_status.py,sha256=B6Wyd7_kvxhRZjblTUmS5GnAmYjxAwV73tDBIo9ONtI,179
-customgpt_client/models/create_project_response_400.py,sha256=UdwAqRAGJdjmCz3AhSAaXx61Vviij3IKEMaacaaqQ3U,3107
-customgpt_client/models/create_project_response_400_data.py,sha256=LjKil8v7QO3I2i9rUPF2jC0_BodzDx7yB2hHJnTl4No,2819
+customgpt_client/models/create_project_response_400.py,sha256=Ya4vq0lh88MrtA02CK90j6ENR2Uohpj3lCwD1visQ1Q,3086
+customgpt_client/models/create_project_response_400_data.py,sha256=bARyRJYWDj2ravsQa1x_JNideVeDiPCZ-2VBAE1KFlk,2798
 customgpt_client/models/create_project_response_400_data_code.py,sha256=57e23WK3yCBW0NEHhoYyvKUU_-RsZlvY5uigyMUzo-4,258
 customgpt_client/models/create_project_response_400_data_message.py,sha256=9WeG5zlNTRKvkG0H4QuNXr2CX4vJMkMmX3Rr7sQ6K1o,362
 customgpt_client/models/create_project_response_400_status.py,sha256=bkf4DDKRow381oGs4tZxw9sdR_81TSbyfzjhbgf22sk,179
-customgpt_client/models/create_project_response_401.py,sha256=VYPnQs9-OEeP4CVtq8zQFzE-ZmmOE8IcNSCBcHGFxUc,3107
-customgpt_client/models/create_project_response_401_data.py,sha256=lrJl9HFCH7CQwZ8NUFC_z60GsPjB1epmlKoB5ia75uY,2320
+customgpt_client/models/create_project_response_401.py,sha256=Rh1bgVfH8GDeEl3hbwBroexh0D79Jc2awz9s1GA3fOM,3086
+customgpt_client/models/create_project_response_401_data.py,sha256=-p9WVRocVmvTU4l8MWCKQy-2Glv3e_IISMn-QH1xspg,2299
 customgpt_client/models/create_project_response_401_data_code.py,sha256=AU5gFgzs4rgTMAfNOesLf30VkBlSEBbojx0g81buwfc,258
 customgpt_client/models/create_project_response_401_status.py,sha256=IpceX7yCd6LPZg1z-AlTX_Ny8BdM_XVHSxGJp43fde8,179
-customgpt_client/models/create_project_response_500.py,sha256=2K-aS9jRfBp7VALJaVS6YQETE2NdxKzZoYlAtX4zOzw,3107
-customgpt_client/models/create_project_response_500_data.py,sha256=7VxOeifIyJhQl-vCs_UlzMpJ52rGWQO6X9XVaeABVZc,2303
+customgpt_client/models/create_project_response_500.py,sha256=nCqL1bgBFQiBPKxPrd6u6WV98YcBYDCksFgPi67pVrE,3086
+customgpt_client/models/create_project_response_500_data.py,sha256=84_CirSQNDQtHkNeXx-topxs58v4VJLr5tNpxZU-Lxk,2282
 customgpt_client/models/create_project_response_500_data_code.py,sha256=DlH6CgVsJj-OSowFd-mbrgFw8fOouCRO5etqqELjTIw,258
 customgpt_client/models/create_project_response_500_status.py,sha256=3xryTEQHvvU6LCE9ii5aHy2A5xsATpDRHq6WmdzMKl4,179
-customgpt_client/models/delete_project_conversation_response_200.py,sha256=GhxxDs9M0vp55HsumYYCDFw9R2Igfq7YSewSicqXwaM,3055
-customgpt_client/models/delete_project_conversation_response_200_data.py,sha256=_k2AwBkxPzCf6ePs7YNC1ymYeaUuBGOeMqxdiccynJQ,1700
+customgpt_client/models/create_project_source_multipart_data.py,sha256=WyQvhjy55WuppmEh2l1GJjeYG1snWaD_saMxJpr9DU0,3787
+customgpt_client/models/create_project_source_response_201.py,sha256=rhVNPPKXO_oh1wm9ELE3h80CCCS4CZhBHZ9kXbIt92E,2920
+customgpt_client/models/create_project_source_response_201_data.py,sha256=e8uHlyT_HpxgiygzpOHpq7gg3yGu9JAwKVOeO0yiRU4,5993
+customgpt_client/models/create_project_source_response_201_data_pages_item.py,sha256=5WQUXMOdIgliPqF-7GyDLE6LxKj8XU8zOpfOWzXjg3c,9212
+customgpt_client/models/create_project_source_response_201_data_pages_item_crawl_status.py,sha256=iTbLaNiksHt1cJzV3FOk9uru4zfKX_f2hcmcCBNGXFc,256
+customgpt_client/models/create_project_source_response_201_data_pages_item_index_status.py,sha256=pyj4zkzkjd320H2h9t-0gzknH8l2MY9LIkkQOmuN7Nc,256
+customgpt_client/models/create_project_source_response_201_data_settings.py,sha256=dOuUHe7HmTXZq61UAI8KlGUdTXCITvXf50l_KHBdoIg,3078
+customgpt_client/models/create_project_source_response_201_data_type.py,sha256=eBs6Je19B21_q1lbOy7D6aM6G9vWWhH3uxL_JnXxa_E,249
+customgpt_client/models/create_project_source_response_201_status.py,sha256=97BBm8J7cuUSMzp25do13pqrrzCZHuNbSqYJ5wJFkOs,185
+customgpt_client/models/create_project_source_response_400.py,sha256=DAtOHDBM52qSt9HwEt_qLPnRcl4Zb_RFdviO-tEDrX0,3206
+customgpt_client/models/create_project_source_response_400_data.py,sha256=alI-YTG-ZKBRPkt5bvJ359ndXIHwHtj40pRwAW5WPdk,2898
+customgpt_client/models/create_project_source_response_400_data_code.py,sha256=VPZk7QWna_4DTkINge2vVVbnF99RYJS3pb5ZywwoieY,264
+customgpt_client/models/create_project_source_response_400_data_message.py,sha256=TMZOHp87LqQzEd3GpfYQ22wkJlhSkG4UEdWmzF5ZTRw,406
+customgpt_client/models/create_project_source_response_400_status.py,sha256=sY7jsdho29rZhoOEn_4wLuHvdnIRwS85xN-kgP2RA5E,185
+customgpt_client/models/create_project_source_response_401.py,sha256=g9hjg0Q64oq8fSSaglHPbv67JGQ6a7tIA5_H-e7OzvU,3206
+customgpt_client/models/create_project_source_response_401_data.py,sha256=dudPBWmBAX6Qo7yOhAft_aWFzOpCOL1toKyRu2yUKts,2369
+customgpt_client/models/create_project_source_response_401_data_code.py,sha256=I_PZKu8Q-4BjfnZpEkS_8BDav22M3GmPEFqATpyPIf4,264
+customgpt_client/models/create_project_source_response_401_status.py,sha256=zTkI9lunWJLZ4kOFNnR2T4BvyMJzusmq9G2hbcarnx0,185
+customgpt_client/models/create_project_source_response_404.py,sha256=EU5WWRPBXVF30UyllGwfpqY2rNqFWOUWf8pLGSduWe8,3206
+customgpt_client/models/create_project_source_response_404_data.py,sha256=9_YbYqeW4WKWLlXXnU1J-kn2KUaLZoz5f2BOwl2ayz8,2902
+customgpt_client/models/create_project_source_response_404_data_code.py,sha256=Lxn5XD6mKanaafd_2AAuZ9J9S8erQBvOpwPbkbNQerw,264
+customgpt_client/models/create_project_source_response_404_data_message.py,sha256=xUANsu1sx7LSrPCxSwXeQgzVTBGkyFQgkF8iuad3mjY,264
+customgpt_client/models/create_project_source_response_404_status.py,sha256=W05WQl7EYGjXitzRoq7ZW0uFJmVQHZfZXkub_YTYiVQ,185
+customgpt_client/models/create_project_source_response_500.py,sha256=dKk8SFy6QCM9_73xgHMc9MbTwk5FBqeikttXfLTFBxg,3206
+customgpt_client/models/create_project_source_response_500_data.py,sha256=pJq0FA4DGckDqJEP5a_1AtOmzim2ZN8ACqGqmSK8yAs,2352
+customgpt_client/models/create_project_source_response_500_data_code.py,sha256=9dGcHQySAUpqpkiyy5ePsFQP_xZ7ZlVQEbvkDSaY_jg,264
+customgpt_client/models/create_project_source_response_500_status.py,sha256=shZFepWeawnfRH9dIt3e-08DU_3uMPKqnDEikt_jRnk,185
+customgpt_client/models/delete_project_conversation_response_200.py,sha256=lnAQPg21sUszayUqcfPsebAR_m-ttMSzS5-lngJTAgM,3034
+customgpt_client/models/delete_project_conversation_response_200_data.py,sha256=FRbqLbDm3Yg_qEUyLbojl6K3Lr-y1xBCFn4nli9fzeE,1679
 customgpt_client/models/delete_project_conversation_response_200_status.py,sha256=8olXZZ7w7GPN6yxPsU9NFo7XBeWmJzZ8BZrto27s5cc,191
-customgpt_client/models/delete_project_conversation_response_401.py,sha256=aeLpF8OEtnSPwXFvzCGKtovwNAWRC1zwR3A7i7Jka7M,3341
-customgpt_client/models/delete_project_conversation_response_401_data.py,sha256=Ujfg7v4B1BfDhG9V9aTrsY1zh-CbP-3SmAjZrXXyWsA,2456
+customgpt_client/models/delete_project_conversation_response_401.py,sha256=lGu_F_bRCFje_GMZZQTmp00tGatgRXKxf1NIJy3RIsg,3320
+customgpt_client/models/delete_project_conversation_response_401_data.py,sha256=smjFpoMl9NMU7_dU4S4QxAQZVqLtL7PkXBW3uOLOyag,2435
 customgpt_client/models/delete_project_conversation_response_401_data_code.py,sha256=FwK3-_uGOOi1wTBtfUrnRegdhhT2Lc5UwKSajMRnH-g,270
 customgpt_client/models/delete_project_conversation_response_401_status.py,sha256=YnKEZZxPyAYS9MK4xOoAhGLdMM2QNZ0Ha851-2WCT9c,191
-customgpt_client/models/delete_project_conversation_response_404.py,sha256=-joSN-u6xnpEMYUyTJdx1w44RbCCcTehG3yrPb-63aI,3341
-customgpt_client/models/delete_project_conversation_response_404_data.py,sha256=tiii1ybTQIQaGGBhtavYJiCrOrIbOyYIniRXW9cens0,3034
+customgpt_client/models/delete_project_conversation_response_404.py,sha256=UsRP3fUQc923RD52vI1oGE6Pm6QZy_ebl-wXFeQz9Fs,3320
+customgpt_client/models/delete_project_conversation_response_404_data.py,sha256=GvxWqrUTkFzeYAowYzikVRCxf5dNeMImzOE2EU4lm8g,3013
 customgpt_client/models/delete_project_conversation_response_404_data_code.py,sha256=RtvG_bLNpnjhiX7jljUikKdPbFa5Uv6OwMed1CX6T7g,270
 customgpt_client/models/delete_project_conversation_response_404_data_message.py,sha256=2OQ6YjkLLo59sWcb8GJAlHAX14TRzOIDHbHLlRyuYFU,270
 customgpt_client/models/delete_project_conversation_response_404_status.py,sha256=gsIkjkNz054RB-9yv-gb3YufNnA0l51w4C2-BGigrRo,191
-customgpt_client/models/delete_project_conversation_response_500.py,sha256=QY5XNCy-thHUEfpDQ5lKZ0viY0JIAnw8wN979aeOHlc,3341
-customgpt_client/models/delete_project_conversation_response_500_data.py,sha256=wkntKqjE7ThHzA1vvLoTWHb-AodCQAZqlysdKz1y9cs,2439
+customgpt_client/models/delete_project_conversation_response_500.py,sha256=Ah6WkN1AEKz3X8iiXSsZTcc46OO7s711DhLXucFTX34,3320
+customgpt_client/models/delete_project_conversation_response_500_data.py,sha256=ZZuiD84FENOCi2u6Jl0CGYpVI30siWVJg4cURwVvTgU,2418
 customgpt_client/models/delete_project_conversation_response_500_data_code.py,sha256=6CswZhX3DCXldhfg5OU5KOEC6JJ1ILlpn7zPj1fAbOk,270
 customgpt_client/models/delete_project_conversation_response_500_status.py,sha256=AQh5TBRPAgmia8k21BhiMc7_X8sLiEkcVi86ECLH-D8,191
-customgpt_client/models/delete_project_page_response_200.py,sha256=nrzhN3nCqzyfoLNPr7Ba4h51oqhdzf22uuyHzSxFTa8,2903
-customgpt_client/models/delete_project_page_response_200_data.py,sha256=r_DqGjh_Vp_OL_v7Gikggg_7IzmsGyIhHHvFtSWUMco,1660
+customgpt_client/models/delete_project_page_response_200.py,sha256=xEfVra-QA_RYcF5RgC9LgWkO8duvRDzc_Lyoln-bMtw,2882
+customgpt_client/models/delete_project_page_response_200_data.py,sha256=jQI0-NKaOHLJk2PHWZ7fqcY_i-3grPr3fZkEi3650fM,1639
 customgpt_client/models/delete_project_page_response_200_status.py,sha256=xbyoqRNFyVECdJ1bOUuMvqFNtEapyGKKo8yHssyNvqc,183
-customgpt_client/models/delete_project_page_response_401.py,sha256=V2dAdPgHNJvPT0EjmtpBNO3hhxMz3d48tX9wSFkpSEc,3189
-customgpt_client/models/delete_project_page_response_401_data.py,sha256=tUDzkk3OyvqQV_zCDaqZvQqojy0iWBeXU5yh1yUjZrs,2368
+customgpt_client/models/delete_project_page_response_401.py,sha256=EQin2QIVI0zj014cDWzsyZBX9Bl0JDHjlscu-fKIBq0,3168
+customgpt_client/models/delete_project_page_response_401_data.py,sha256=VYg0rETYvhp5ptjMp9PXcDXU4i9aMAJZWemJ4z_4xlc,2347
 customgpt_client/models/delete_project_page_response_401_data_code.py,sha256=gKAllkOb2E7r7XQGSo4JyLG9efv6PXW8HYm_jIObeIY,262
 customgpt_client/models/delete_project_page_response_401_status.py,sha256=jc8ntLI6_OUsbvPIRpdG2vpXC7NTHz1iyZh06ZpnfMU,183
-customgpt_client/models/delete_project_page_response_404.py,sha256=6uNdupnLD2eSUDMbknUjfcHXR2KgwZiUsMpUxE41YSw,3189
-customgpt_client/models/delete_project_page_response_404_data.py,sha256=RjutNTdkdy_kAaWVlUBrNd9tXt56siR8pNnga10nSv0,2889
+customgpt_client/models/delete_project_page_response_404.py,sha256=ieRp6nfuZ6xXNHoab2Ao6gcOQw-yE4yLQjhO-vRVEzY,3168
+customgpt_client/models/delete_project_page_response_404_data.py,sha256=b3ocbAlmJT94tMgT_NxEDobxo-o1v7zCjbAg4XfLN1c,2868
 customgpt_client/models/delete_project_page_response_404_data_code.py,sha256=8klGMqaSzCKaL3yT7Ecq1PmCTccetnx2IsiiiEpCFho,262
 customgpt_client/models/delete_project_page_response_404_data_message.py,sha256=buBaac-elrBoM_958d6TafNygiHsp0oxOGtSCyCvZ6M,262
 customgpt_client/models/delete_project_page_response_404_status.py,sha256=y5p8Aox003PqXeUk22m5LF9vFlGo_AozXQ7l4l-jpeE,183
-customgpt_client/models/delete_project_page_response_500.py,sha256=t2XeKxgFjNHg1XGSgV-4Bsz-x2fxie74fE9y26_j16E,3189
-customgpt_client/models/delete_project_page_response_500_data.py,sha256=3d53gb6i5EHPmGgtv2yl4eioeK_XOoRAhOY6PqBfxZw,2351
+customgpt_client/models/delete_project_page_response_500.py,sha256=IYScj0DZMEC3h9HBdy1U_eB49HSiB8p7OCoYPieY1fY,3168
+customgpt_client/models/delete_project_page_response_500_data.py,sha256=uKKB-zgDpMIZxelNLOPEX6asvggte8YEDtQO21vL9PI,2330
 customgpt_client/models/delete_project_page_response_500_data_code.py,sha256=r4xUBA5JHAGGauqluT2Mb2c-nX2w3WK4FHjjD9Hzuec,262
 customgpt_client/models/delete_project_page_response_500_status.py,sha256=SrI7OUmkuT4OWLUV0H7mYyR3gVb4ZN6M-M6uVcrGBGw,183
-customgpt_client/models/delete_project_response_200.py,sha256=ypoqcsFNwzR9ZCM5uQ6FS4pyqPqbYyHeacFNErJuBL8,2821
-customgpt_client/models/delete_project_response_200_data.py,sha256=Kj8fqXE43XxM1Q7TgTymLthUWcD4M1k8_qSGTJxhJvA,1637
+customgpt_client/models/delete_project_response_200.py,sha256=cRzP53n54HrTBDAS-em8hihoCdtDTq1zQQVzLwhmXig,2800
+customgpt_client/models/delete_project_response_200_data.py,sha256=HUjQ4vUxTmcGT9Ax4eFJP0nuLNfPA2LuZSIWCtTMs3Q,1616
 customgpt_client/models/delete_project_response_200_status.py,sha256=dqWc6Uo2JxUJTumwf7XTJ9DyToCVhowtdIOOZzbZNOI,179
-customgpt_client/models/delete_project_response_401.py,sha256=x51vNt8Xkyl6a4aRUEmOWVNyrZo2-XmT2puJJgKGrUU,3107
-customgpt_client/models/delete_project_response_401_data.py,sha256=9EVvRcTh2sZV0Vg7tYHVfllW1yBr8XMWyaDcmmSDjbI,2320
+customgpt_client/models/delete_project_response_401.py,sha256=98DrcAaL8bKQLhGL5psFO6G99UytcCU5skaaRAtjr-8,3086
+customgpt_client/models/delete_project_response_401_data.py,sha256=tBrfhAAy-7ZbPO152A01wEjnxQ3AvWh93KMI_FkF9Bs,2299
 customgpt_client/models/delete_project_response_401_data_code.py,sha256=xOE4r96E513BnIJrnayJxGFx6cdtHKu0DYuePvTzAgM,258
 customgpt_client/models/delete_project_response_401_status.py,sha256=VLyZwY4h19YcIvHJypt7P5oyEj6LMZMVuB1oBYsRIto,179
-customgpt_client/models/delete_project_response_404.py,sha256=zcO-zIcSLlaf2PJ5BonJK48Yr5TQO1VF-9QkyujIw00,3107
-customgpt_client/models/delete_project_response_404_data.py,sha256=_mDj8lAhTkTwYLfQ9vidl95rXLqXMC9DT1jo6NvHa2k,2816
+customgpt_client/models/delete_project_response_404.py,sha256=3p2J5JER45M4_-6p1tVNqQd3SqBdcMFwVmI9R1DDovY,3086
+customgpt_client/models/delete_project_response_404_data.py,sha256=sZXLInovwsltsy4q2MPl5xVJF8_a5_zfRByU8Uu_ixY,2795
 customgpt_client/models/delete_project_response_404_data_code.py,sha256=a7MMf9NTOWc-iFmbzan7b6e9v9PeXiedafYuwgq8omY,258
 customgpt_client/models/delete_project_response_404_data_message.py,sha256=Wcxia5OmDQaca9MAqQlhFuM1nYLkMqJxoqcRI2lIpHk,258
 customgpt_client/models/delete_project_response_404_status.py,sha256=AEFeRreVy_Ac_BW5OwKjgerJmzkQwhUG5PHa0iqPC24,179
-customgpt_client/models/delete_project_response_500.py,sha256=7gO_ld7_vmRmNuqHHCEIZ3nqGRgD5xLK4WgmUWxS6Uw,3107
-customgpt_client/models/delete_project_response_500_data.py,sha256=gFFmLn5G2SL2ApgBXuwvxpwrgYcdURHHjl1qJ0svTOo,2303
+customgpt_client/models/delete_project_response_500.py,sha256=HzJ_2qObwrUap22Qw9COrVv6qNo-Bmz7nlp4bE8ZFlI,3086
+customgpt_client/models/delete_project_response_500_data.py,sha256=3tXpgU0wZ1ncKoXWmDmewKEjRSJ8fvx-CkLaGuD9vYY,2282
 customgpt_client/models/delete_project_response_500_data_code.py,sha256=9W_vx0bu51d-y2xQmMPnadJF5TRiPSc5wohn2ZmjQdg,258
 customgpt_client/models/delete_project_response_500_status.py,sha256=9o6P_sFhc77oIC8t6DyIal2pJiYslIdSy02fq-0lM-o,179
-customgpt_client/models/get_open_graph_data_for_citation_response_200.py,sha256=1jrk4ygzeuvZFh_NJH78mlit4EoHNDz1LyK0R14G5g8,3148
-customgpt_client/models/get_open_graph_data_for_citation_response_200_data.py,sha256=CStKL9_jqf1Rd9fIGeJxgMYcz7TjvcIuzvit-zQO9jg,4443
+customgpt_client/models/delete_project_source_response_200.py,sha256=fHmE2L2J3ITs32r-bUYgEEX9aMPbPA1Sr51dnIpO8BY,2920
+customgpt_client/models/delete_project_source_response_200_data.py,sha256=ViHEKJWnSYqjZ4IGo36sdfMxsI5mZkEcKm3t_oBWZ_Q,1656
+customgpt_client/models/delete_project_source_response_200_status.py,sha256=54hNIaHhc87gniCDJvd5Qn6rvZRFICCt0HjNRawkMwE,185
+customgpt_client/models/delete_project_source_response_401.py,sha256=1NaOLcibzk3N9xlzU--jMdery2yd5EhQyJWin_gNdBA,3206
+customgpt_client/models/delete_project_source_response_401_data.py,sha256=_ix-qaomxosqETZhWrbEi8t64eAmgSo3kwqVEkaXyRA,2369
+customgpt_client/models/delete_project_source_response_401_data_code.py,sha256=IksBMTDDAOePCdlHhth69t6yAV8VjNy7uewO5o0l6Aw,264
+customgpt_client/models/delete_project_source_response_401_status.py,sha256=Hz31LHuiKlNNRQIjSrAhOvLY1p0-kTlbmc3-jwT7Vbk,185
+customgpt_client/models/delete_project_source_response_404.py,sha256=mv73hJ9XmWgkO8po4VX1v7tWphuV8svNC3g89D8OSiQ,3206
+customgpt_client/models/delete_project_source_response_404_data.py,sha256=GnJEOy8t7zLKAEJMyPeI3ejLwdvUICDKsDXXrKpyGqA,2902
+customgpt_client/models/delete_project_source_response_404_data_code.py,sha256=eLBPitPUcb2PZwH8bO6x9CSdPpZQE2TVyZzPqlOgJhs,264
+customgpt_client/models/delete_project_source_response_404_data_message.py,sha256=gz796VNFjnLq0-R1wtWiGY19HLU4OAn-fsthdFsCY8k,264
+customgpt_client/models/delete_project_source_response_404_status.py,sha256=-MthPZuB6NqV9q7vltVSW4HoEMJwyAlMNRodn9JLz7M,185
+customgpt_client/models/delete_project_source_response_500.py,sha256=GIJ1MUUB_rCkHWvy6Zm8a-EtCrQKIMn_YCInqfwQ2xM,3206
+customgpt_client/models/delete_project_source_response_500_data.py,sha256=9ITvf5m9V4PrhvZ-waoAyH1RecjXpa9ZF1rPqK76rso,2352
+customgpt_client/models/delete_project_source_response_500_data_code.py,sha256=-r2oaFjsiWAmi0P36rEWoPWOTJN637tu_klZ_qk7OuY,264
+customgpt_client/models/delete_project_source_response_500_status.py,sha256=4W8GOd2JxL5Hc3DQz2DvqLZQBpOYJhBj57SueeRZZMg,185
+customgpt_client/models/get_open_graph_data_for_citation_response_200.py,sha256=RP6EBw3Q-l64QjoG_FzkgSEHgX0ZTrJ8QnBXFmFOECA,3127
+customgpt_client/models/get_open_graph_data_for_citation_response_200_data.py,sha256=4r_w20qxD8bBHYTQeFXbtZUSvDm-DMDrzR1nX5tAQ1o,4422
 customgpt_client/models/get_open_graph_data_for_citation_response_200_status.py,sha256=1hYcWLusvS55udpyy5wAZo1LHa5sS2bW1bqNaWbsaK8,193
-customgpt_client/models/get_open_graph_data_for_citation_response_401.py,sha256=GM8HWMYkuibRc-bCejvofDSAg45Ak-vKlnjU_K2BBBo,3422
-customgpt_client/models/get_open_graph_data_for_citation_response_401_data.py,sha256=zuy0nqjiIwK7P4wcIfLOFzLSn4Bzh8lGvX_ViEAp0Oo,2499
+customgpt_client/models/get_open_graph_data_for_citation_response_401.py,sha256=rSKM06kAlwnUhLUMnbcyw6lzY8w9YvHewrE-7bMB1EU,3401
+customgpt_client/models/get_open_graph_data_for_citation_response_401_data.py,sha256=ZCKuqIX28NzwaLvLc604rQIJMP9X7jeY5oPzq78-mHE,2478
 customgpt_client/models/get_open_graph_data_for_citation_response_401_data_code.py,sha256=RXqjDv2a13msP3NlFSTnigTg754toJaukh8j9fr_Dhs,272
 customgpt_client/models/get_open_graph_data_for_citation_response_401_status.py,sha256=NuMKsKo1jdYyNuM7EBvH1_zbgH94ZW5nYkbfLVB1QZE,193
-customgpt_client/models/get_open_graph_data_for_citation_response_404.py,sha256=oKHhruUi2duCgp0MoomW4chZXa9N051wY634BCZj5wU,3422
-customgpt_client/models/get_open_graph_data_for_citation_response_404_data.py,sha256=d4xLpaaay-raamjPoi_WRnYvej_Fr9sxsYPneqohkps,3092
+customgpt_client/models/get_open_graph_data_for_citation_response_404.py,sha256=PRKxzOSZsFR0jUthywNCijYGZq46JMzJt2MZIXJ4Pho,3401
+customgpt_client/models/get_open_graph_data_for_citation_response_404_data.py,sha256=_7y0zhMhzydD0g5ljqIdo8u297Hh0Gh0yrF0l-ei1iU,3071
 customgpt_client/models/get_open_graph_data_for_citation_response_404_data_code.py,sha256=HpI1n9CRAFY-mXS1yQWXJoBoTVL76cKnBDab7SdiWnI,272
 customgpt_client/models/get_open_graph_data_for_citation_response_404_data_message.py,sha256=8_MvUu-uUOqHi8O-S-POcaMFwsYmJ-UYQCBbobfhX2M,272
 customgpt_client/models/get_open_graph_data_for_citation_response_404_status.py,sha256=91MuKYVjMyHs2tUbPko_9-zAIYX5GCUvoQGq8cxuKyg,193
 customgpt_client/models/get_project_conversations_order.py,sha256=zCYvVb85cUEBpfM0QNZopcPRbt6f_d3sVN1NTiYwyVw,167
-customgpt_client/models/get_project_conversations_response_200.py,sha256=ed_9JMdTPauKMr5bxN37-poEsXflnBD7FB0Wyw_wnuU,3017
-customgpt_client/models/get_project_conversations_response_200_data.py,sha256=DNvdzxFNP490vrswdkG2WpYNqcd4BI6WLDZCwa-D_Gw,7137
-customgpt_client/models/get_project_conversations_response_200_data_data_item.py,sha256=AoIu8pJTa3kKCCtlGK9AsAjF4QLLOvnWiZBzDQG_ZmQ,5069
-customgpt_client/models/get_project_conversations_response_200_data_links.py,sha256=NnbwadhdBxZ7D2LFx29u7bsAcw61xEieTKgua1g072I,2602
+customgpt_client/models/get_project_conversations_response_200.py,sha256=wfStLZ1b-pujAPdmlQanDJ12v_Q5KveA5SdF9wtDZOA,2996
+customgpt_client/models/get_project_conversations_response_200_data.py,sha256=WwyS3WKIj3hLmlb8U922zqlWfiDjf3kJw6THzrKsZ6A,6186
+customgpt_client/models/get_project_conversations_response_200_data_data_item.py,sha256=GOPnGI7d5N_OlcvSmL1IrWIUiQMN_-Qv6vF-6vSUORE,5177
 customgpt_client/models/get_project_conversations_response_200_status.py,sha256=3yTJSCsopWHmBO6L5qo15nIPdU_D_PJqs5GL5UTcxms,189
-customgpt_client/models/get_project_conversations_response_401.py,sha256=xTsgzbmXC6P-He0EuLx2b5IWeyJqyWS2HmzmhnsS2Ro,3303
-customgpt_client/models/get_project_conversations_response_401_data.py,sha256=1eYZudD3hMGd3TTrR-XVRgNpHTZl6KZRIt36kTR5MNE,2434
+customgpt_client/models/get_project_conversations_response_401.py,sha256=V4QkG2yFNzEQ_riqiO1nh2Bco2X3e6B2a38vEo1cMv4,3282
+customgpt_client/models/get_project_conversations_response_401_data.py,sha256=w8IUcIcGP-LUGCIGKnV4oazb6u4QjSs03RFfY08DikI,2413
 customgpt_client/models/get_project_conversations_response_401_data_code.py,sha256=rvcTMn9frWk-bgSmYEri2o9wy6cnxnWg5W7QG2jX3JY,268
 customgpt_client/models/get_project_conversations_response_401_status.py,sha256=UddjP_DE8by8yP0R6Wg3Plr0LygKqCH95JgyREG-e4U,189
-customgpt_client/models/get_project_conversations_response_404.py,sha256=x8DgzvYrxLrqMK-FbuW2HgUtqhs4UO1pdoxqpzA9jrw,3303
-customgpt_client/models/get_project_conversations_response_404_data.py,sha256=2q9JqfvOjSpPoe3eXDqDQQhb8wVaEesoxOlkDWZqxQo,2991
+customgpt_client/models/get_project_conversations_response_404.py,sha256=wczqT6nHL149nNw8sBQIkIODeBiXQXi1oIUPt578FaA,3282
+customgpt_client/models/get_project_conversations_response_404_data.py,sha256=ZqYM94rFzKQIXbQuvuv_rPfIfXBhz8lX56rVHp25SBQ,2970
 customgpt_client/models/get_project_conversations_response_404_data_code.py,sha256=z6lZqGPCo_wjAj41-mPAoySuR2bYuFcXxpN-jC_J8z4,268
 customgpt_client/models/get_project_conversations_response_404_data_message.py,sha256=23mE7e3CsGTTotZ8e2DA22Kneo-8JqJrQ7mZCs3VwA8,268
 customgpt_client/models/get_project_conversations_response_404_status.py,sha256=qpaWKUO62D-OSSxlzOqtXCkJomTzJmZ7fbBFvDFn5Pg,189
-customgpt_client/models/get_project_conversations_response_500.py,sha256=OI_3E1k9yyNv3qrCMS7q2Kd-s1hecF7Ahwj1Vw5t5v0,3303
-customgpt_client/models/get_project_conversations_response_500_data.py,sha256=5y8gi6DUVeS7_njs1cmj017MpKibduhQdm0c2HmlL7A,2417
+customgpt_client/models/get_project_conversations_response_500.py,sha256=lRdIG6BpysNas36cm1hpgkZ62DDbEVSng7qlu2Dal58,3282
+customgpt_client/models/get_project_conversations_response_500_data.py,sha256=qX2acEFJgTwX8Quorp_2kg2OOvpfZ5iDerZ0b3v2nT0,2396
 customgpt_client/models/get_project_conversations_response_500_data_code.py,sha256=HNHKms7yWsXGt2n5a4yyetyjWIP1m0dmf4emEff3p8Y,268
 customgpt_client/models/get_project_conversations_response_500_status.py,sha256=eJj4q3dAkLN2JCcUYhZ4gsErFPfY3GDQHPuF-zMXjtU,189
 customgpt_client/models/get_project_pages_order.py,sha256=xo5fevqZ9EzsS_MYCsvLnYWccsceTgKyfmWeZC0rVu8,159
-customgpt_client/models/get_project_pages_response_200.py,sha256=HHxIKuGttas21Fx8RJu4UEaiUwTYtQF2MvwkYKw5oEI,2865
-customgpt_client/models/get_project_pages_response_200_data.py,sha256=HUTdyi3_pQlobBCbrSUaMgmu0RFJG6XTRnHhpeV_R9s,3094
-customgpt_client/models/get_project_pages_response_200_data_pages.py,sha256=VvYvE1AviDDpen5IIAZ3MsPep-qMmBKkyMq0lCw-QIo,7042
-customgpt_client/models/get_project_pages_response_200_data_pages_data_item.py,sha256=zcSpeRALY_oVhrn5dbB8HRUoILKcI4szosbIlnS_HUE,9561
+customgpt_client/models/get_project_pages_response_200.py,sha256=bw8kgMvNj_YIPnJq_6Tgx-ppUe1sqiYHZnSt10Rh7kM,2844
+customgpt_client/models/get_project_pages_response_200_data.py,sha256=v0kLeqbNAOrGnGzASdjlo7w-l8Rj4rBqkzi5w3m_IOE,3073
+customgpt_client/models/get_project_pages_response_200_data_pages.py,sha256=WZ1ylKfEmnooqh4sGXHwVFCd3iK3WtK0B0Yla3ImipQ,6138
+customgpt_client/models/get_project_pages_response_200_data_pages_data_item.py,sha256=eKCBeEypgLzHSjO5RthVZguRav2hIA7KsuXbqRDGdAA,9217
 customgpt_client/models/get_project_pages_response_200_data_pages_data_item_crawl_status.py,sha256=G1H-A6HJKf6K4boOGDJPVWiFHTplHasKqfquuXHk3Hg,256
 customgpt_client/models/get_project_pages_response_200_data_pages_data_item_index_status.py,sha256=U_1FcuYmRQA5V2r8YQIEItUzQNIJWd7aTiaIK48xOH0,256
-customgpt_client/models/get_project_pages_response_200_data_pages_links.py,sha256=_9JvP81041S_szgz0nQRfQ7D4XLnabvM-nrV-a2wfS4,2590
-customgpt_client/models/get_project_pages_response_200_data_project.py,sha256=PQlBZK4jRzhURg5GyOEsi0KfdBrqpAhRroeJmybQfZQ,8215
+customgpt_client/models/get_project_pages_response_200_data_project.py,sha256=70xMiltXOXXM7y1t5qvevcTDVElO3HrfGBj41P9mudo,8194
 customgpt_client/models/get_project_pages_response_200_data_project_type.py,sha256=gHCNa8WdvI1DNlCTEu6KmoKrFx_ruL7CzguLr--Y2eo,186
 customgpt_client/models/get_project_pages_response_200_status.py,sha256=r-s-HDUz6xu-HFyZSIH33ZhsXE5D9wzjl_s7qUh3VZ8,181
-customgpt_client/models/get_project_pages_response_401.py,sha256=rsmsXKY8QOgMp0ZN0nCvC4puN7-1LI5uMCbUcl9n2EY,3151
-customgpt_client/models/get_project_pages_response_401_data.py,sha256=xbPyV7ytVHQcC1-42kNL1RtTofo2QyN_yI5jefdQz7M,2346
+customgpt_client/models/get_project_pages_response_401.py,sha256=QAOwUDF-zkb3NXptvKUymFRz73rN2y5vLSKQ5zPVJsQ,3130
+customgpt_client/models/get_project_pages_response_401_data.py,sha256=gUWTHRmhOmLG6KzsisUrn1XosMnDp4j-eBwVq1fJFtY,2325
 customgpt_client/models/get_project_pages_response_401_data_code.py,sha256=wQDdbzVR8BCuJkbcWVnnetgucAWK_Z3rLWtLJx9h2bs,260
 customgpt_client/models/get_project_pages_response_401_status.py,sha256=DgbRssSo-TH3J990dSafvTMihB7XyZF2tItFaBXYy0Q,181
-customgpt_client/models/get_project_pages_response_404.py,sha256=LVzssmRi9t2sN-dMdfnflw0Vwx4Qdj9FQnvdChirMnA,3151
-customgpt_client/models/get_project_pages_response_404_data.py,sha256=1w2-tkrf9c2b-GpKn6HOYqbON5NoVgFfDoEk3Shq13A,2855
+customgpt_client/models/get_project_pages_response_404.py,sha256=i2Go4wLsJ5tY4YjNRc5acD_GIfupt4DzkHLsN68WHjk,3130
+customgpt_client/models/get_project_pages_response_404_data.py,sha256=BZkfZMbXLGaPwL-98z4qw--W1n4-ssQid5jiYrRyu3s,2834
 customgpt_client/models/get_project_pages_response_404_data_code.py,sha256=unjT_ddtLPvKm38JBV3dZQ14ijtY9IXqP6-q4eURI68,260
 customgpt_client/models/get_project_pages_response_404_data_message.py,sha256=MpRnAzQu1m2Co6oo7H-9dWactSjbnSL1yIHZB5tbqjQ,260
 customgpt_client/models/get_project_pages_response_404_status.py,sha256=RKl6hcXQxtFO9u4I_G_PdfQIxIXHZ1HGERTFfXufpy4,181
-customgpt_client/models/get_project_pages_response_500.py,sha256=sErp4S-ybDJZ0VD3RZV9ui9cWsD7lA3FbRBRbq3Qr7k,3151
-customgpt_client/models/get_project_pages_response_500_data.py,sha256=UvHB0_bzVwl8WDZf_iJJ1irzA-vSbd5E-teDRpT77dY,2329
+customgpt_client/models/get_project_pages_response_500.py,sha256=2doMRn9wibYPvuxnWJSkjfrrqzRPL1DWBF32z-FCpAg,3130
+customgpt_client/models/get_project_pages_response_500_data.py,sha256=2NhLp4SEYKfDn1zFawfJDaRBl1FJe8mu9TfRNx-mTso,2308
 customgpt_client/models/get_project_pages_response_500_data_code.py,sha256=9nYPd7rVuQKXr4LjeLzG70A0HiYCU0GTvU1BwJPlkns,260
 customgpt_client/models/get_project_pages_response_500_status.py,sha256=CvjsBwEzNhkYKrMT38lH5CXS-UTnRPavrFDyVJpIom8,181
-customgpt_client/models/get_project_response_200.py,sha256=qOtZlGHyicxA8xMfhZBpBLIodJhYIBbxeJcZlKb9occ,2764
-customgpt_client/models/get_project_response_200_data.py,sha256=gEPd3CcsniA6N3FhrdKoUQNm5hEas_z0BxjlXENcC40,8051
+customgpt_client/models/get_project_plugins_response_200.py,sha256=qhsaJ6G6cgtGfDbX5a1ihF9pLxYMzS9tPlrxjzweG00,2882
+customgpt_client/models/get_project_plugins_response_200_data.py,sha256=CT5qU0eIrxukibxT-ZXk52gOTvS3PxpsDlvRZBi80Uc,3568
+customgpt_client/models/get_project_plugins_response_200_status.py,sha256=CHtp33akfk-RPc4vuGODX6W8HbHA0H4pcB1waYw-Vg4,183
+customgpt_client/models/get_project_plugins_response_401.py,sha256=H-Y60sEW41O5ahIntIfmN0GIDzQ3-ETqr6JQLxIILnk,3168
+customgpt_client/models/get_project_plugins_response_401_data.py,sha256=la52g33jWcx23XygVgNlZtl9TKZM4CTWEkGZKmuiezE,2347
+customgpt_client/models/get_project_plugins_response_401_data_code.py,sha256=hT2kP7D9gEiTuYVSHnLtmLxLbvkrho--CS52sfG4tI4,262
+customgpt_client/models/get_project_plugins_response_401_status.py,sha256=d_-eLFW5h6wI-ta8Q2hwkdeyPr98az1jk1SKcfWpi5A,183
+customgpt_client/models/get_project_plugins_response_404.py,sha256=-WBG2ybBptO8jZCPo3Zr_Nz94reCIGuxDQy1CJV0Dkk,3168
+customgpt_client/models/get_project_plugins_response_404_data.py,sha256=pJtDJit_HOBkj5qj1ji3wRSDFpWywPJypBNTgIaxgrM,2868
+customgpt_client/models/get_project_plugins_response_404_data_code.py,sha256=Z9K6KXaGc45lO-KbvfE8lKPN4bowacU9mwHZKch1i4o,262
+customgpt_client/models/get_project_plugins_response_404_data_message.py,sha256=JR4iNA7NK-jRQ_x4uI1fD_voyABTZKxfgGx46e3q01o,262
+customgpt_client/models/get_project_plugins_response_404_status.py,sha256=p8x9nBevyllJkuHtoPDnSmtGWEyVm341zrQXLAsjpas,183
+customgpt_client/models/get_project_plugins_response_500.py,sha256=mq1H7xrqaIi8YdTctcWeltePvrKVv3w1YPg3ycaqcqI,3168
+customgpt_client/models/get_project_plugins_response_500_data.py,sha256=G2FXBLlgBGwMV5N_bIrD5hLxq30djUtxuZdDqL1rD-A,2330
+customgpt_client/models/get_project_plugins_response_500_data_code.py,sha256=ueB6iUvmMpda3pDrPv0N_HpBOWKHIJTRpsVGDHQ-GQ0,262
+customgpt_client/models/get_project_plugins_response_500_status.py,sha256=ltNB_K3xGrd6LaiA-x0rf50oY6EaFZltq4ivmkCpuZE,183
+customgpt_client/models/get_project_response_200.py,sha256=XojyZfC6RhApHSSHrRk758oVkLHNUBxtWMi6mXBL8jo,2743
+customgpt_client/models/get_project_response_200_data.py,sha256=k19ReVgvzf5I9e1Vc-BbUCFPwo-0WPJ4W8nCzsjpCTE,8030
 customgpt_client/models/get_project_response_200_data_type.py,sha256=cK1YiH6TGvFSU0pZkitCF_IIH3riFIrV8LFKfG8Vxis,174
 customgpt_client/models/get_project_response_200_status.py,sha256=vf93iMdE9uHxVG_proHosOjYgPGGDIOTyWet3cxQVpA,176
-customgpt_client/models/get_project_response_401.py,sha256=by9Fum6ae8tCFbAl8GLbryyqPtl5k1e-ZWrucuxOEIc,3050
-customgpt_client/models/get_project_response_401_data.py,sha256=S0ZmwZfb6Zix1Vm8DgvGLkUw822dU4liSroDlRs0rXA,2287
+customgpt_client/models/get_project_response_401.py,sha256=5LIiFtpZ2s5hHOUW_OdqNPsDvpITQHGKuEbiKRkKFUU,3029
+customgpt_client/models/get_project_response_401_data.py,sha256=3GoiWA876g5CpJGuNoaV6vBzRexpPESQpBBEttdMfJ8,2266
 customgpt_client/models/get_project_response_401_data_code.py,sha256=ZxtOEvqnE21zNx8lpjKzZfcH9we47xgIDJnx6wCnsy4,255
 customgpt_client/models/get_project_response_401_status.py,sha256=CEaFiYpjPB2AhNHxHgiXl8hlz5D4PiZUXBIvRUhbGLA,176
-customgpt_client/models/get_project_response_404.py,sha256=ZDhZRDG2tTXttxjawhlICWXM7BhjKHReDUxfJPsJ03E,3050
-customgpt_client/models/get_project_response_404_data.py,sha256=jq3lTd-a9b6KIHfVnNiGbZ3So6rGD6FCSVmQXvWhZG4,2753
+customgpt_client/models/get_project_response_404.py,sha256=LwD6JoEjxdRdV1ss8oaGVGY_2gYyPjs-VTDPzOiG9E8,3029
+customgpt_client/models/get_project_response_404_data.py,sha256=K9SVXk-0Hwig2RWW6Lr5khu84_NeOHbCY9_H30DaJFA,2732
 customgpt_client/models/get_project_response_404_data_code.py,sha256=8JMLo9lTo63m0U934ooyNnEGh6CYYz8e2XVCwqc9_bU,255
 customgpt_client/models/get_project_response_404_data_message.py,sha256=ZigDM26-QDpoGrO7yzzRWz7j3N_TWj4NqA5u-uE9KIY,255
 customgpt_client/models/get_project_response_404_status.py,sha256=UAZ0xr62mBkCrfMejzcbMOmb8L9AUNLqt9BtwqPoF4k,176
-customgpt_client/models/get_project_response_500.py,sha256=oMQCfyK_K9jWQlhcQBzzNK_vDLyYQ1INeXIPzyBnL3g,3050
-customgpt_client/models/get_project_response_500_data.py,sha256=YJnotgZK74-_FWUEYBGuasVGaI0Vrv75z-CmNR2cPEE,2270
+customgpt_client/models/get_project_response_500.py,sha256=9WXU1ywaGv9z8aoFmL9b4HvyetrcxSbIlt5ydjnrerg,3029
+customgpt_client/models/get_project_response_500_data.py,sha256=iDu8mB5yLUE-ymhin8XaUal4rUreIf7qavvoAgcAuKU,2249
 customgpt_client/models/get_project_response_500_data_code.py,sha256=3S83BU1Vqp60Yeb_A3V53_xxOj2Nt9FXID94DWsaybs,255
 customgpt_client/models/get_project_response_500_status.py,sha256=fQZ72Abgw22TZpInxFWXgeO2B-grOgjFPcW-vW9OXCo,176
-customgpt_client/models/get_project_settings_response_200.py,sha256=N8gqn5PS0jXCpCyq5cfGWfmz05kxPs1p45xCh1Bwzf4,2922
-customgpt_client/models/get_project_settings_response_200_data.py,sha256=ZE4px4Nnh5-dUoRtWo3sSqULT1pIhkn4mD6D1mUJQpw,4690
+customgpt_client/models/get_project_settings_response_200.py,sha256=okgyc0_B-wQLM_UP-fj01UFCVEnKQG2Al1LQVraLHVw,2901
+customgpt_client/models/get_project_settings_response_200_data.py,sha256=Ar-wiPE8_Dg-P0CXS5pz6xmgstc4Pr7kTq7aAmQERiM,4669
 customgpt_client/models/get_project_settings_response_200_data_response_source.py,sha256=uiIghmwFgquzQXs-GqdYeRW6Ths2XdSNw6DxvLKdRAI,254
 customgpt_client/models/get_project_settings_response_200_status.py,sha256=y6VeGaeJVtiv8oCNtLA8h1SdUWyX7aJN2SmwMgCsZ0M,184
-customgpt_client/models/get_project_settings_response_401.py,sha256=cr5TrjN8JwVV3gpvDTnLagwqnsgkbsSvlPMOmI5PFj8,3208
-customgpt_client/models/get_project_settings_response_401_data.py,sha256=Wj8IcCU1c9Ud7RqvyWZnof-myyX_F1XC3lIYfMsKppM,2379
+customgpt_client/models/get_project_settings_response_401.py,sha256=4FjD6Q8YgH4sUP_3UCyqB8IZ-PY4mL6RO5e3mGG5sq8,3187
+customgpt_client/models/get_project_settings_response_401_data.py,sha256=tjOX-wR5U7fhOpjlqBQxnDx2_8uebqZP2Gjb9k-8Y0A,2358
 customgpt_client/models/get_project_settings_response_401_data_code.py,sha256=B1PUKnx_PHey6yj3V05Itfo6j-3w8awfpJepSZ-D_70,263
 customgpt_client/models/get_project_settings_response_401_status.py,sha256=F7q6oEkhkPkLo8Z-k3p6IMGlzXYDd_MhymyGnYcTzf4,184
-customgpt_client/models/get_project_settings_response_404.py,sha256=HYHLdRSjbRpuvZr2A800LODVGmWgE4BpAF87Xs5Dq2A,3208
-customgpt_client/models/get_project_settings_response_404_data.py,sha256=bd7uNPtjI9hTrKQje7S6cjfgwSi3nFJyge5B9xXDvMQ,2906
+customgpt_client/models/get_project_settings_response_404.py,sha256=cDtXC5Uh2plrH7hK7-50l8ztGh-CTg3t_nGh9llUdiE,3187
+customgpt_client/models/get_project_settings_response_404_data.py,sha256=s2H0DobbBGZcbyDR7byoIUlObbEEFJrxhoHXYYMXNpc,2885
 customgpt_client/models/get_project_settings_response_404_data_code.py,sha256=l-2HMJWRzkmA7VO2WjJIWH_JKcn1TzthpHe8MpQv7wY,263
 customgpt_client/models/get_project_settings_response_404_data_message.py,sha256=o8fmCCmEvRLvHi-BEARmbQDLHnmziSb_RdfhmFqqwDo,263
 customgpt_client/models/get_project_settings_response_404_status.py,sha256=pCwbQddpPmMXSesDdt-9xPX3g-9Z3A_BJoEDCwofGrc,184
-customgpt_client/models/get_project_settings_response_500.py,sha256=p-1oRXSLRiYr-moFgP5vamICIPC91-wzT4FAEINwlT8,3208
-customgpt_client/models/get_project_settings_response_500_data.py,sha256=EeHmSXGh_DM7h6QD4xH8PZFqSc1296oN22iqGuFWNtc,2362
+customgpt_client/models/get_project_settings_response_500.py,sha256=RmkqwyqkGKVZwXfgtUOelObx850Y4VS7vc7aMklwBYo,3187
+customgpt_client/models/get_project_settings_response_500_data.py,sha256=OvPd2U01WhF8M4LUbBBjTNl5Agc6N5zzQl79_A2uGp0,2341
 customgpt_client/models/get_project_settings_response_500_data_code.py,sha256=m4UdLxG-CQhmiR6-7h4DBszDBY34kbU1i6c6re04fvM,263
 customgpt_client/models/get_project_settings_response_500_status.py,sha256=CETUrdSyInFUHweS1Hms0c0SR5OJXhxmDA96VlaAYLc,184
-customgpt_client/models/get_user_profile_response_200.py,sha256=l9_m_0hC1_vuxugR7lr_wOtvytalV3GGcVLPHNBicGw,2846
-customgpt_client/models/get_user_profile_response_200_data.py,sha256=wE-s2cO4j6WyUlPCgpG1F2btj74DHCGtnxS4yacvXqc,3931
+customgpt_client/models/get_user_profile_response_200.py,sha256=KsbydL_XiWJ46F4TdxRsI2tyGF7eXCvioPAxgyfjmBU,2825
+customgpt_client/models/get_user_profile_response_200_data.py,sha256=UAunKdA_yNe7Og9Amw4b2YNG0r8TIVpBXsWJxrqopzo,3910
 customgpt_client/models/get_user_profile_response_200_status.py,sha256=HK4YhUSuhP7SwIM4ZbnlTdF5rALWGtxC6eT6ED1lrD8,180
-customgpt_client/models/get_user_profile_response_401.py,sha256=RT-qkl_d5dFLAxUGXu7XU-gUg4A3dxPGhvLmRxyw37I,3132
-customgpt_client/models/get_user_profile_response_401_data.py,sha256=_ogpPZeoRhwP1h9VjFQFFekmIhhZuB9i7l-02twqwDM,2335
+customgpt_client/models/get_user_profile_response_401.py,sha256=b9-OLRGLrv0UMyTkMt2LU_gpHY3l8uT599rPeCv0dTs,3111
+customgpt_client/models/get_user_profile_response_401_data.py,sha256=KK4irN-7hriycA0VaZ-5aEH5J7TdnOXB7BMlcmHEigc,2314
 customgpt_client/models/get_user_profile_response_401_data_code.py,sha256=LylNg7vuX9ollKH1hvQ4On6_fL78wPD3noK66jALBz8,259
 customgpt_client/models/get_user_profile_response_401_status.py,sha256=p2cv3zoMF7-y2a1CO7hMbDeWq-JcwCKsiWDMAXC4mOs,180
-customgpt_client/models/get_user_profile_response_500.py,sha256=p7A6eQh4UUAkLlLo-mJiSXg3n8s9wJcHXCFDp_2ph-0,3132
-customgpt_client/models/get_user_profile_response_500_data.py,sha256=520AIGquC3pPqzYNnXCB5d1YVeBzO7ezQZOGuXLeg0A,2318
+customgpt_client/models/get_user_profile_response_500.py,sha256=h4yEw6nPyCwbSIX4sz66CZenEzvYrDnm_jKD7IP0vxE,3111
+customgpt_client/models/get_user_profile_response_500_data.py,sha256=n989Q5e4h0IH2pygneM-dW-NIvdIGmgrDOyD5oNkPFU,2297
 customgpt_client/models/get_user_profile_response_500_data_code.py,sha256=sTmrsBbo2d4098ZBOb2xGqJJdfuxC5G099fmV2wdYGQ,259
 customgpt_client/models/get_user_profile_response_500_status.py,sha256=7JwBeQJ2ZAx_0FnR4xsvUBK0oFhyRRhV86m1KJDgndU,180
+customgpt_client/models/list_project_sources_response_200.py,sha256=eqnjRbjS2RYYB5Ustv7dNZRJhsdbRnVjKLA8lDl_M5Y,2901
+customgpt_client/models/list_project_sources_response_200_data.py,sha256=8SlSUjHWLfCCEkJvWdF_ZQZ8Fx2sAgq9NC1VBDvE484,2835
+customgpt_client/models/list_project_sources_response_200_data_sitemaps_item.py,sha256=SF4smzg-jqPFpWKDh-PSurfG7X9kmU7iD4Oimz4wvWw,6387
+customgpt_client/models/list_project_sources_response_200_data_sitemaps_item_pages_item.py,sha256=kWebn3r7ayNbWqqfIOJnPN_EZ4TleXyToECUk_uJqdU,9893
+customgpt_client/models/list_project_sources_response_200_data_sitemaps_item_pages_item_crawl_status.py,sha256=tXbn7OxIh3je3J-bq1gyOxrSu-gfj04rEKZsrZp6LFU,267
+customgpt_client/models/list_project_sources_response_200_data_sitemaps_item_pages_item_index_status.py,sha256=p8IVdwydyej40qmjegTRgWdzg9ejSR4_NyMCj8TWYGo,267
+customgpt_client/models/list_project_sources_response_200_data_sitemaps_item_settings.py,sha256=GAE2mC3YZ8ZboPjs3eMeSNYHTvugxxaJN6JmjXXdirA,3139
+customgpt_client/models/list_project_sources_response_200_data_sitemaps_item_type.py,sha256=Vf7Nx-9OfErf9GP1GwboWmwK1B_L_Q-T_XGBXObQ4SA,260
+customgpt_client/models/list_project_sources_response_200_data_uploads.py,sha256=48lqLaOx79Mr2-LtN08IdnYG7P1ZL9hi9EUlC0XmamI,6216
+customgpt_client/models/list_project_sources_response_200_data_uploads_pages_item.py,sha256=l85W6L2d8wsZHvRVfQepBx1k1QhtbWaT-4Gc9HBjymw,9343
+customgpt_client/models/list_project_sources_response_200_data_uploads_pages_item_crawl_status.py,sha256=StkKuIV1V_xMKjBDxBlQy8cYQgwjaBBmQhXeeJmQ4PQ,262
+customgpt_client/models/list_project_sources_response_200_data_uploads_pages_item_index_status.py,sha256=Pgx81JacKlK4tkrt3CK6RivYToAVcAVIc3RUciZPnlk,262
+customgpt_client/models/list_project_sources_response_200_data_uploads_settings.py,sha256=d014G0ckRytETVX-Gb5RrXLuuUI_xVnQSTBLEEN8lEU,3111
+customgpt_client/models/list_project_sources_response_200_data_uploads_type.py,sha256=MCk1ZEjtHKtjEoebzbN4c_OJtOHYD62I6O14Rs1E3YU,255
+customgpt_client/models/list_project_sources_response_200_status.py,sha256=UDksUiUSvydQDdgD7IRhIBDbBxCd_dKWfIFfWd3J0hc,184
+customgpt_client/models/list_project_sources_response_401.py,sha256=h-oBUB98EUSiBwnqzT2BV08Giz-QK7neHX6kaiVxOS0,3187
+customgpt_client/models/list_project_sources_response_401_data.py,sha256=3wHznJVJRRlUhyKxv1AD5F9bgoTYVoWTQ5SPJe5CsQY,2358
+customgpt_client/models/list_project_sources_response_401_data_code.py,sha256=lO2L2WlGO01rUpZGvVc2lofmpSEyswKGXjWED5lJHnw,263
+customgpt_client/models/list_project_sources_response_401_status.py,sha256=qkdkgZCZShW_Hzz5c_GfJtxp-apr7f9Gh_tSCUK3Ds4,184
+customgpt_client/models/list_project_sources_response_404.py,sha256=Eif3J5ZgtJ-L4RytN3dvPY7HZJDRsMhAqXd4mimb9Uw,3187
+customgpt_client/models/list_project_sources_response_404_data.py,sha256=PtxOmKZRiIgHqrIrqrpARBIvDZBCDxG2Zv78YF5AsWY,2885
+customgpt_client/models/list_project_sources_response_404_data_code.py,sha256=LJbFXW6nNe0kjZuw4T3bMqLORkjUH3TVAWEIsVVAkxo,263
+customgpt_client/models/list_project_sources_response_404_data_message.py,sha256=WieoNsnZV-yoSdBDwzZH6OsBVWR-kNdSAp20q-VgKXI,263
+customgpt_client/models/list_project_sources_response_404_status.py,sha256=aBdOZYOBAxtngC8iyJkYU1xYFV2lhD8nALemA080KIw,184
+customgpt_client/models/list_project_sources_response_500.py,sha256=Lr1xcw1yA-1TT-5BPs8subkwqvqNxUOkWLH_4AMgvlY,3187
+customgpt_client/models/list_project_sources_response_500_data.py,sha256=vr5Snwz7zeeWjXDXn2PZYW1qGokBeyHQ_jUCSwGJF4s,2341
+customgpt_client/models/list_project_sources_response_500_data_code.py,sha256=dFEh2fYXX9bIUez7TOItgCkEQs-atM33w-Qut4mYb9o,263
+customgpt_client/models/list_project_sources_response_500_status.py,sha256=u1SbcdWooaqGuKmLiyETvVydbNJrDTl2CcsGXY-qeJc,184
 customgpt_client/models/list_projects_order.py,sha256=vxNX-HKOdzGSDpWR7NW-gSgW4dWo84uwj7niUdSfJ2I,156
-customgpt_client/models/list_projects_response_200.py,sha256=pT5kj9MCUWzaJw97g6JHukxM1UsGStO3NolJZ0iF-BA,2802
-customgpt_client/models/list_projects_response_200_data.py,sha256=WAqAk4DzEfE2NVzA5lWxJ5_D1QsD57YR94OW-6MHlso,6843
-customgpt_client/models/list_projects_response_200_data_data_item.py,sha256=maGUAYOFJx8K71BAJpiqizNzX7YM6LyX0xRJXqqSQrE,8189
+customgpt_client/models/list_projects_response_200.py,sha256=OE5PGr3l-VA8-epJJyNaGB3ZdCRezkJjEw3PD2pfLL8,2781
+customgpt_client/models/list_projects_response_200_data.py,sha256=J7x6kYFxfit8YX5VTYE6tFQ9joroPlXlfo2uBYAyZc8,6007
+customgpt_client/models/list_projects_response_200_data_data_item.py,sha256=Oq63XG73sN_qJRctlH7yWD4MWfiSPI0lW3jXvvPNhb4,8168
 customgpt_client/models/list_projects_response_200_data_data_item_type.py,sha256=_9N-XBSV0IPvL90LQnJM8UpVynwYyGF2eswKIUtAhhQ,184
-customgpt_client/models/list_projects_response_200_data_links.py,sha256=kVFZBPvW625V3UX81IL2BWV1BSQZx2WMxreeZ4bfvRo,2544
 customgpt_client/models/list_projects_response_200_status.py,sha256=eu0StnuHGTXjk8yJs6i0t1KykudRR5M5IF-14EINNyo,178
-customgpt_client/models/list_projects_response_401.py,sha256=GgKm64F0R_tT5w9-2Jdt1xTaChZxMgSy8dJofuRyYkU,3088
-customgpt_client/models/list_projects_response_401_data.py,sha256=61qKjmKHzlsmahoiIlQOSaJgbK7x3OxBbTI1dL1IGSk,2309
+customgpt_client/models/list_projects_response_401.py,sha256=Be_yaf-Mh8zGEc3ZLdMdljPUq6CokdtbIpDKcOWt2HM,3067
+customgpt_client/models/list_projects_response_401_data.py,sha256=_WOPW-3y_vVAGg5gKq0RjxoTjKYYg0f3Vve_Am9V1QI,2288
 customgpt_client/models/list_projects_response_401_data_code.py,sha256=rQZbrPZU_YB3RKc0jHVRdxnXyKIBWDr6KNt0q1WG0hw,257
 customgpt_client/models/list_projects_response_401_status.py,sha256=cQVEBwlGWTiEVKj11C1Z8qidllqV2gZni3hlttU1NoM,178
-customgpt_client/models/list_projects_response_500.py,sha256=2-lApCeldrA5NVJRSqZh0M1wq8TgMdozDVs02GXYDz8,3088
-customgpt_client/models/list_projects_response_500_data.py,sha256=fC8rYBracC5EUzexPNA5ijeqHWcNg6gmw5ijw1MI7Ac,2292
+customgpt_client/models/list_projects_response_500.py,sha256=ubeoGZEGx7c338xj9PDsu_6K9eZf9AliTJx3JbKURx4,3067
+customgpt_client/models/list_projects_response_500_data.py,sha256=zaNedBJt6UYgmcZwRYwSCxYNavFMgwb6m0lBLDHMDRs,2271
 customgpt_client/models/list_projects_response_500_data_code.py,sha256=fQDRnc6np9qE28Fg4woVSkR-zobwrebiBXPidoACHH0,257
 customgpt_client/models/list_projects_response_500_status.py,sha256=_nYnvX_gJbZ19Ek04wLt-CYLnlMcu0H6dvxO1oTlhhA,178
 customgpt_client/models/messages_order.py,sha256=Az5l-9LSjyNm9Hi7mwoTeyeKL6tm2G0czGrWsFUdr7U,152
-customgpt_client/models/messages_response_200.py,sha256=Sqli0gjgZs7xJUgNZf9nIrearFy8yEU6jx0E99pa6Yw,3753
-customgpt_client/models/messages_response_200_conversation.py,sha256=_lmT9KKjJGSVsFAQK50HPI_WCjvEMDDPZHMxz1vv7RI,4982
-customgpt_client/models/messages_response_200_messages.py,sha256=5ZQn9ZkRRoH0j8Fs2hop4BcxsPhzOY8nsApQnlB4DX4,6836
-customgpt_client/models/messages_response_200_messages_data_item.py,sha256=UGAX0QKujN_bc7-YsloahOK6iGoWwwxeDNeVCQ8jong,5141
-customgpt_client/models/messages_response_200_messages_links.py,sha256=p66Cpudl0tlSjIX9yEFkv2tTFvs-KCrawEy-c_P9nnQ,2541
+customgpt_client/models/messages_response_200.py,sha256=yKJbYQvl32qm-A-nHQ3Ui9K8BRk1O_cjPM_Ob1gqzgs,2699
+customgpt_client/models/messages_response_200_data.py,sha256=VZpLJoPwadyiebhwD04EbwjAYH_SAJV_basykQI-2Yg,3120
+customgpt_client/models/messages_response_200_data_conversation.py,sha256=F8TCQ2oos1hT817dNBHhZ5XZD6knzjb3kiWs-v2-my8,5113
+customgpt_client/models/messages_response_200_data_messages.py,sha256=kZus8of5TglOUkqfpEUxuiUIL8DQULu_9qbDNRKsyEM,6055
+customgpt_client/models/messages_response_200_data_messages_data_item.py,sha256=LdeBqb7YXnNXWREemiNcL4uhsh0Gc8k_9kP2Jef4Sx4,5143
 customgpt_client/models/messages_response_200_status.py,sha256=hYKqXZ8xnXNnTWP0gQTrkfTAkX_6Omlyy3aOwSBvnhw,174
-customgpt_client/models/messages_response_401.py,sha256=-ksAlXVf8X9a4udJPzn-ndHSG1l4p94i55tR05SFixM,3006
-customgpt_client/models/messages_response_401_data.py,sha256=yY-wN8Wxuwonm3c24QRDej2QpW1RBXlZhuv0jfVWj-I,2261
+customgpt_client/models/messages_response_401.py,sha256=b2NEnUTq0lb2ixODGpCcIebbWFDkO24Jpm1ly0IM2BY,2985
+customgpt_client/models/messages_response_401_data.py,sha256=PiN6c-zIPjNihgDkFWn8UWghoOnS3RTjw8SYjE__bQI,2240
 customgpt_client/models/messages_response_401_data_code.py,sha256=G_zjJ--Ilf1uUrpjBZjj07lOyN2hML4Xxi_HFeqcvR0,253
 customgpt_client/models/messages_response_401_status.py,sha256=gZe6xyeG2Lqhu3EHX9pzggZ1eSBOw_FNr6JN1zQHGVw,174
-customgpt_client/models/messages_response_404.py,sha256=w94YBJe5WQkT9Wx4AOhYnOF-5V2QxUVMX3jtUQ1ZHr4,3006
-customgpt_client/models/messages_response_404_data.py,sha256=UoQJYjeuCLcEe5oVkBKwI3fMkYyq646_2xcUA5FGcZE,2714
+customgpt_client/models/messages_response_404.py,sha256=AUbQYHrfQnCoiPUqXiCsX6M_3mKse4i8s3apAerdpOk,2985
+customgpt_client/models/messages_response_404_data.py,sha256=VLNsEhuWsah21ylcjRMDyv7Vo1gtLNpOjqn5u38hM2I,2693
 customgpt_client/models/messages_response_404_data_code.py,sha256=bqw4D2WSdElKe_e-DoseDpzTJ7g5KRImhfdNRQO2tS8,253
 customgpt_client/models/messages_response_404_data_message.py,sha256=JzG8PsVq8vdlXcfE2_mQ7oHw6arOtolpZl5env9J5nE,253
 customgpt_client/models/messages_response_404_status.py,sha256=kM9b0Ckq-j8ifAwrUK-PACuMzEUVSNics-BfRy-qKiA,174
-customgpt_client/models/messages_response_500.py,sha256=L7dYbT5cI3UQoJkfk3FMBeHti2AEph6xaHwIlgdRWW0,3006
-customgpt_client/models/messages_response_500_data.py,sha256=AdfXRjQ9PmNzT2fzfVRMszooby9NyTGOMfmPQk3Ac40,2244
+customgpt_client/models/messages_response_500.py,sha256=DVwObGC4pEpyVq4sL153NBWpeq6DYTAn1BtyUCva_Ls,2985
+customgpt_client/models/messages_response_500_data.py,sha256=F6S5LFeaB3a10UY9XAf6LVbmrZSuPoqR_-sVQQm5hVA,2223
 customgpt_client/models/messages_response_500_data_code.py,sha256=oFAKl0tyxZ9diBfLFcK8gP7FqtUnPMG051cpq_7RLpc,253
 customgpt_client/models/messages_response_500_status.py,sha256=tyHoJ-hX7LzWOSDQ4JlloRDsLHVv4ltsa3rwgvd6mm0,174
-customgpt_client/models/open_graph_cache.py,sha256=xmniR8ViTRAjjOpe2FN6tZ9B-PUZpQzoO7pXjdIe494,4285
-customgpt_client/models/page.py,sha256=IE3k2xTcmR1Nr8BjKsucEqcIIs69chuigPWGw25Px2A,8656
+customgpt_client/models/open_graph_cache.py,sha256=URmiYZjD9y0iTdU-HIX0JYi4vLFSoGZ7X3rnlc1-mpo,4264
+customgpt_client/models/page.py,sha256=nyaJ0f8SMcI3BlicxmWBv5hEMBsVKzNOjp2pVXRCt7I,8312
 customgpt_client/models/page_crawl_status.py,sha256=d4OfTmehu_jOYYJm8Ork3c1olNEyPbOoOHwsKrNJkVQ,217
 customgpt_client/models/page_index_status.py,sha256=M3D13YILuZ1-g9D91Xs0aVpDsFdn9-9NA_-22lQ25HM,217
-customgpt_client/models/preview_response_401.py,sha256=ruMTvJ-UyIxaOa7hSaT8xo7kylm4UBD9ZmMGoUHuRzU,2987
-customgpt_client/models/preview_response_401_data.py,sha256=wMEv9PcdaOMbcPj2vXWM67c1te_4mrmSuxyKqn2iMvw,2250
+customgpt_client/models/preview_response_401.py,sha256=YpDxGufq6X2W77vHeSGlw5jFT4TKrOMzZ9Ygk_IY2y4,2966
+customgpt_client/models/preview_response_401_data.py,sha256=nGJhwftdI4cmAcuDDqfpcTzaT1sx8su2hbu3diUzHto,2229
 customgpt_client/models/preview_response_401_data_code.py,sha256=dNb2hCq42Cy8QjoURredM8NXe2x0HStP5JszR0hATt8,252
 customgpt_client/models/preview_response_401_status.py,sha256=g2iR8n7zarVfQgOzgsbX4NjVJ_sRU2Z04TgDj8ydeMk,173
-customgpt_client/models/preview_response_404.py,sha256=UUxjjcZYjsRroJFQ1iAKXLQGuVQVGaqgjoueoN3icRM,2987
-customgpt_client/models/preview_response_404_data.py,sha256=XCFzZpnLxpinkPFKHdexalhkg_NrLeytGsiHJFKjHGg,2697
+customgpt_client/models/preview_response_404.py,sha256=bvdkjDkHk5OpqxPFqzDe8DpJQRQPcoRtM1Xjfb61Sr8,2966
+customgpt_client/models/preview_response_404_data.py,sha256=jpHKyN6tfpyJcaisv_3TcBDfmV2_pgmi2Be6vW4i7t0,2676
 customgpt_client/models/preview_response_404_data_code.py,sha256=rDksF27k-S3-a16RcoNKrBZmMHs_xmkT1xKMkb0eSao,252
 customgpt_client/models/preview_response_404_data_message.py,sha256=gm9CCH2iMCcNxPZsfA1KJW02HK1uduqtFTLAhzCilhU,252
 customgpt_client/models/preview_response_404_status.py,sha256=_2w4p2l_KEymuZr7_q8HuykjZ5xKVQf5MS8PLiHff8E,173
-customgpt_client/models/preview_response_500.py,sha256=p6rU6YB7XRk1ZfdvmbNlzQ1yVgVh1a7L87lcs35Uw6M,2987
-customgpt_client/models/preview_response_500_data.py,sha256=aRpyFvNKDHjV1CRWvST4SeWPL-8jqB9YQI4dnBBGHbM,2233
+customgpt_client/models/preview_response_500.py,sha256=I--Hoyk8oggM2dHrSrKoEALmA4xaal9IbjeOFxoAxts,2966
+customgpt_client/models/preview_response_500_data.py,sha256=47zgL3F0LGHYObDf2dK-aHFt5eZo04DeR30a3NZnGq0,2212
 customgpt_client/models/preview_response_500_data_code.py,sha256=cpMdeDwz3NiXPAfSvRe330jgIGzpBGWYhMtsPgrGHco,252
 customgpt_client/models/preview_response_500_status.py,sha256=iTrvMHEVkQucovjl8ASVcQSSEkiEHZyRoVfym-ANH-Q,173
-customgpt_client/models/project.py,sha256=U8FcUJ7bYxhONJ-mhyjleM3bpVQoCR03Y-ClhP7LMhY,7789
-customgpt_client/models/project_plugin.py,sha256=5p1uMdqHaxt1jfhg1U1cy2xvoDM5LHXJmRBou3XqG38,3482
-customgpt_client/models/project_settings.py,sha256=fhf8aFhmOZUVKb-bb1ScYc_JtnIr4tzedC6bpVmkCkA,4467
+customgpt_client/models/project.py,sha256=yKEgt5IgeC-ovcgkK71Pe0BHqSVSnzKPQ4VXuhaxYBQ,7768
+customgpt_client/models/project_plugin.py,sha256=Q9q_w8SAXlsr4O7P3Fd9oPYe0RhGcojSGXgNnXfqWGg,3238
+customgpt_client/models/project_settings.py,sha256=hf126OsZen-zU0-Rq6zjnpws0iajmNw3QAXZddP63BI,4818
 customgpt_client/models/project_settings_response_source.py,sha256=U2TvEDkHrI_2_J6BulyWlInTt4jkkLyxZ9KkbEqCGVg,236
+customgpt_client/models/project_source.py,sha256=pfBa9j4YBUK1_rSW3XDScPzUeiMRjgW-j-Ckysf07lY,5258
+customgpt_client/models/project_source_settings.py,sha256=wB2oDFZ_ElvOxTlc0hHds3xrIGSQacjplw3BVUyFKD8,2961
+customgpt_client/models/project_source_type.py,sha256=-XS9qgRE24tfr5CJ_PaqI072cpfopinMU1EkoqWKK2w,228
 customgpt_client/models/project_type.py,sha256=NRVy0mhDyH1efUNYMFE5Cv-N0fRezFiWO5U9Vb9oxDY,156
-customgpt_client/models/prompt_history.py,sha256=qrlqMuEPe6L_VdQ8Ue4RoSNE89X0CiRjx3KayC5DsyI,5019
-customgpt_client/models/send_message_to_conversation_json_body.py,sha256=kpjdL32cWxGpyB55gPGWNBhRWqQuvw9vOHxXkJHwif0,1654
-customgpt_client/models/send_message_to_conversation_response_200.py,sha256=0h09HD4qXZU0whgxFbLD5mh59WpMN8aQNGGAbAQTYaU,3061
-customgpt_client/models/send_message_to_conversation_response_200_data.py,sha256=-i47XcGSAYvK-fTmSrnCtiB7O_aig3pHLE0ey_u84vA,5169
+customgpt_client/models/prompt_history.py,sha256=TK0dOYO7XtkuySZqsXXDsTO8YRPIF2YjwI-Og9Mfv5s,4998
+customgpt_client/models/send_message_to_conversation_json_body.py,sha256=VWCpQaGeFUPkjcd6qVSZw7t4CaFvDELLmEJcRUUSePI,1633
+customgpt_client/models/send_message_to_conversation_response_200.py,sha256=tQAC3V7a6gas4BF5O8qTWiAT5fMlArO34mDb-50Ma-k,3040
+customgpt_client/models/send_message_to_conversation_response_200_data.py,sha256=5wFr-C08ehw0C5AUzrAnlsN28BidTeDCbXD_W3wddhQ,5148
 customgpt_client/models/send_message_to_conversation_response_200_status.py,sha256=gCa2JhJFIEYjz2aSykQOcCAQ1qMsZVMd0PrzHLISBpw,191
-customgpt_client/models/send_message_to_conversation_response_401.py,sha256=aGEXOrSQUZBAcw56XCaZyu44HFqvCb3hUOUXLMCKKco,3347
-customgpt_client/models/send_message_to_conversation_response_401_data.py,sha256=4PjSKXd4FE4YtpBoyJduEFnrg6Dp2V2S6eA2UjBxxl4,2460
+customgpt_client/models/send_message_to_conversation_response_401.py,sha256=9VpeWiqlBp88XQplVp-6bY1vy4FdxZePTQ1QbnHeppU,3326
+customgpt_client/models/send_message_to_conversation_response_401_data.py,sha256=pZbOTyNb8UQF-JOdoFYkiRxgXNmWQeptXf-evfxdAsc,2439
 customgpt_client/models/send_message_to_conversation_response_401_data_code.py,sha256=Tnj5RDE0CpKbjdVei6M8aqSupLHU4SWiMzmsDP4qwR8,270
 customgpt_client/models/send_message_to_conversation_response_401_status.py,sha256=x4FCHr4sFcpZH-GvrC-39vH9pFJ5Kfwsrvans_ba-6c,191
-customgpt_client/models/send_message_to_conversation_response_404.py,sha256=ViEtVn6mwvLzH6Xwe7wv8qOfKLZA7AFAQ5QNrkU48Zk,3347
-customgpt_client/models/send_message_to_conversation_response_404_data.py,sha256=VOLU1iJrvJU3pJMctKat0GErjNGU1i3Ef1XFVbcWvYI,3039
+customgpt_client/models/send_message_to_conversation_response_404.py,sha256=smZZXT1C2wowJxk_52Iqv6YU6vQai69sut8pvd52PWo,3326
+customgpt_client/models/send_message_to_conversation_response_404_data.py,sha256=FlTnStfTPUYzwSwr-EnxBSFD6oXDmAty5cMKDlCtgnQ,3018
 customgpt_client/models/send_message_to_conversation_response_404_data_code.py,sha256=uEDNMhiAP5w2MGeTCiPqw4jlj2j80jnWA6ql3aTapFk,270
 customgpt_client/models/send_message_to_conversation_response_404_data_message.py,sha256=nj-cXtX67Djaf-oPt47lb_DOfBSRXdufmuc-RQolCDE,270
 customgpt_client/models/send_message_to_conversation_response_404_status.py,sha256=fBdWowpqAa52MEEmTa2fbX92Nc7BqdN-AOfAiDht0vQ,191
-customgpt_client/models/send_message_to_conversation_response_500.py,sha256=JhPJAp8Eu8-532N2F6qJJRMghv6AjCjlEYFkQJCtuWQ,3347
-customgpt_client/models/send_message_to_conversation_response_500_data.py,sha256=4seHSrl-H5W3ujnj3pGDbAZCPMX7iCJmDfXBFdtwb_c,2443
+customgpt_client/models/send_message_to_conversation_response_500.py,sha256=psxwCeZJdtIrgiGEjrHu0qJLo1PweWV_G8aWdbi-FEc,3326
+customgpt_client/models/send_message_to_conversation_response_500_data.py,sha256=q-foC9JzjJhNjX3BD2Tae14aWx-Us-zWMIgoCwHoeos,2422
 customgpt_client/models/send_message_to_conversation_response_500_data_code.py,sha256=KuvtySWITsLYnr1LVneej3LSoFiXn1VEOWFhUv3bRVs,270
 customgpt_client/models/send_message_to_conversation_response_500_status.py,sha256=L9LtSG0q_6aRKCU5u5wLwQnU2XhxuLWsiuUgWRG3z50,191
-customgpt_client/models/stats_project_response_200.py,sha256=smFcWLlLgzBiOO04Zg8faQdzfe2oC8xfwYe4g9RhdMY,2802
-customgpt_client/models/stats_project_response_200_data.py,sha256=Q0-AcbH-PELAhsLAjCihkUGUlZaQepjktRX7JOpky2g,3719
+customgpt_client/models/stats_project_response_200.py,sha256=zkiVhGm-bnQ5Kn2HQ7YbiaNrPkfkaax5LVQ0YmE_QMQ,2781
+customgpt_client/models/stats_project_response_200_data.py,sha256=PEiukDtRXurGrWWSDdeZnOX6I0XD3mGBgOkVDyytmAA,3698
 customgpt_client/models/stats_project_response_200_status.py,sha256=HHWClJhffILrpqwAjMfdinSClwHS-RRbrj4NLGmxFrY,178
-customgpt_client/models/stats_project_response_401.py,sha256=yyA5qj2L2N0Xt9kntZMIXycqoo8DyxZIqsz2wq0iIgs,3088
-customgpt_client/models/stats_project_response_401_data.py,sha256=ufxg3jMHrkUz4YZJfQmg6aJ3YcaLffh9G_U4LRGMEmM,2309
+customgpt_client/models/stats_project_response_401.py,sha256=yUvQ7Y-UxQumf0tGLb3rAQ0_-0CPI96VPcmmG-SV8KQ,3067
+customgpt_client/models/stats_project_response_401_data.py,sha256=0s35JJpxjTs4e3if5o88tdPfmcor7sVwwINwjiqS-BA,2288
 customgpt_client/models/stats_project_response_401_data_code.py,sha256=V6Xhp10VoiKXIUeZQi03ZuQJ_7KIoqx2-IxZ_oQvIaE,257
 customgpt_client/models/stats_project_response_401_status.py,sha256=9RfavKKcslXQ32TLf_qyD2OgyttG2K39eZfswVbQdy4,178
-customgpt_client/models/stats_project_response_404.py,sha256=BZaSr2dfOuzE6EYzwETvsA0ztxP6qJmgSWEATdI5L4A,3088
-customgpt_client/models/stats_project_response_404_data.py,sha256=7mfFWURtcbI7LulWAH3wmtiW8zQrmtPV1_btK-FKTow,2787
+customgpt_client/models/stats_project_response_404.py,sha256=P1ub5F8RJMW9damRLIPtgtp7L1B8QwpwHYKCs2f-jNs,3067
+customgpt_client/models/stats_project_response_404_data.py,sha256=3xZ0ysc1umI0PQSmBYgjeEuB3CCEjXsNvpm0y2Qw_wg,2766
 customgpt_client/models/stats_project_response_404_data_code.py,sha256=QEFHOb4HE6vJ4VIijCB5GosoxpL8td2ZJTHi9wwtJFQ,257
 customgpt_client/models/stats_project_response_404_data_message.py,sha256=m7HX6EfLgixckHecr35W1mfjvBg_72V81-NUPWQHf9k,257
 customgpt_client/models/stats_project_response_404_status.py,sha256=tL0A4Oy6C9EVaKN1QO45lKQZFZb_PK6N1mWmGdg5VSk,178
-customgpt_client/models/stats_project_response_500.py,sha256=jRSkWCLXtL33VkCiqzsx0xDD4Mx3Vqzqk_dZ5Nt9hgo,3088
-customgpt_client/models/stats_project_response_500_data.py,sha256=Y4BtoEBdkxRG11ClAZTC365uOZ-QwbQ1jrwxUPqetKk,2292
+customgpt_client/models/stats_project_response_500.py,sha256=ZxemTMvmYmwuoWqZVFjC1Thx2iQPIgZ4YgxpIbFzGpc,3067
+customgpt_client/models/stats_project_response_500_data.py,sha256=Z89h5lOUdaUXuMqJLOmE40esBCmCwVmFIKqJU_gIvvc,2271
 customgpt_client/models/stats_project_response_500_data_code.py,sha256=ddWW4LXKmwChLpPg1A7bQpusvh28wu5p4I2qTBZ5QHE,257
 customgpt_client/models/stats_project_response_500_status.py,sha256=dE_h4LEScDtM4a6a2H9CrXnbpbMblA1Rj85n-EfD5-w,178
-customgpt_client/models/update_project_conversation_json_body.py,sha256=OOO33yt-sSfbRI7Xd4m4MYZUW-DaTGI-H8rqRLfJ4xE,1628
-customgpt_client/models/update_project_conversation_response_200.py,sha256=EBxNL_DVi5k5WPtWdXgMz82WTXWVqEi-jgSBmcO3-sE,3055
-customgpt_client/models/update_project_conversation_response_200_data.py,sha256=iZqtJeskgrCb_zByPyGf5kfasYNdvSUd-_RU2udKD3w,5033
+customgpt_client/models/update_project_conversation_json_body.py,sha256=_dYEhWzb2e53SgEjbsd8FzWIHyS0pK8cniCcN8x5upg,1607
+customgpt_client/models/update_project_conversation_response_200.py,sha256=Pe8c4kZxD4QDNnpZyL5-drqgc_lfKOoINE4i_Vmr35A,3034
+customgpt_client/models/update_project_conversation_response_200_data.py,sha256=azy4vvOxHYmP279Y-RIKwJA6ltBqDRuwgkUDarWa3i4,5141
 customgpt_client/models/update_project_conversation_response_200_status.py,sha256=YgdzPzVFW9vlMYzSOkw_-1SVv5Ty4-Q-aS_wwHqrm0E,191
-customgpt_client/models/update_project_conversation_response_401.py,sha256=upNfsd7-RuKuksvWnBhVJ9PqjfR6pte3WQO9kwYt8EE,3341
-customgpt_client/models/update_project_conversation_response_401_data.py,sha256=jzHpmTIhg_qiVFOafwpLGA4bZXSzzCIwmuCW-RJ3yFE,2456
+customgpt_client/models/update_project_conversation_response_401.py,sha256=QNy4zXiwZI43Cjrf4kQL0X9iUol7Q50HjVcZoIqUT3s,3320
+customgpt_client/models/update_project_conversation_response_401_data.py,sha256=oVDI0xqXS4cDVSuw6XgCadywVGSxXSjgZmtv5UWVa2c,2435
 customgpt_client/models/update_project_conversation_response_401_data_code.py,sha256=u1Qgz9Gcgt_7uoupuizCy0as6fGG3qC1twFTJ3Se34Q,270
 customgpt_client/models/update_project_conversation_response_401_status.py,sha256=Sn_JUgLIsZ2wYp5r5i5mRRII8dJwuhkVyzUOOPx5rJ0,191
-customgpt_client/models/update_project_conversation_response_404.py,sha256=DguBAuO-CGm6yRvutM2WzzsjounSkQmyaHN36DWpWgs,3341
-customgpt_client/models/update_project_conversation_response_404_data.py,sha256=L32Gmvbn80oahrkMcahXLYdHKN7f1_Z9erNBKAfG7-4,3034
+customgpt_client/models/update_project_conversation_response_404.py,sha256=4gBccVcdv3tV6am7DEyRDLYoZ66opq3BNPTJSkJG5B0,3320
+customgpt_client/models/update_project_conversation_response_404_data.py,sha256=zpnvzPIk2tvQRmYvTKKTlZX0xJD-F7cFbDJAX5yRVbA,3013
 customgpt_client/models/update_project_conversation_response_404_data_code.py,sha256=y_uYfOxnqF26A_yS6WkNyeaqGdRvTiGslXO5E3dCEdI,270
 customgpt_client/models/update_project_conversation_response_404_data_message.py,sha256=UHeTgBMjIiEqkaQnUXaL5EJt3ZI8g6mAhzUmNA58pME,270
 customgpt_client/models/update_project_conversation_response_404_status.py,sha256=Xl_tJQxJQwh7k-hwLiqSajzArlGWyu1U2p85-RLprdc,191
-customgpt_client/models/update_project_conversation_response_500.py,sha256=kICFC77h9PCjqq9BOLwzZo0j3VIiJn0DFg1BxsiVeko,3341
-customgpt_client/models/update_project_conversation_response_500_data.py,sha256=--nN1gn5I8mAtqOrzvdEd01kO6IyXs7s0OSHUOyZabc,2439
+customgpt_client/models/update_project_conversation_response_500.py,sha256=NFy35E8Fk86vEIIkeKGLnmQGgky_BvfAFPpup965KLY,3320
+customgpt_client/models/update_project_conversation_response_500_data.py,sha256=vQ6n1tcnkH0Cj4-3dZAMWGujUKWMXGBmnXXxHifyvwU,2418
 customgpt_client/models/update_project_conversation_response_500_data_code.py,sha256=h1EvHQ87gohQsG_DxB6RYdBymTrB_r6ovXOpMVJHRTQ,270
 customgpt_client/models/update_project_conversation_response_500_status.py,sha256=rQC_PJ16A2xQaEgLrRWMy70rH2ufPoBFOGPjyPH3QqY,191
-customgpt_client/models/update_project_multipart_data.py,sha256=qKBb8AK3BQ8wXunFC9k9_WZXArwTJ4xhsp-nuL-3wXQ,4948
-customgpt_client/models/update_project_response_200.py,sha256=-9at7VCpq2sHrDbGcAYIJEO6wPhBQHhiVON7qwsGPFk,2821
-customgpt_client/models/update_project_response_200_data.py,sha256=qy47ev7n7104ox6H_5uPkrCFjhQFAxRx0pZuf3kzYWw,8090
+customgpt_client/models/update_project_multipart_data.py,sha256=2REVDqmcvWG9jq2xweJWVpGYakebVZqPPiKGksdi1Xg,4927
+customgpt_client/models/update_project_plugin_json_body.py,sha256=VODYvdsKoCLhthFVmIzqM9WlXfh9W5bL_BC9TXgf17c,3030
+customgpt_client/models/update_project_plugin_response_200.py,sha256=yAJSd0--JCtKH6T6SacP9sXoHxGhXDNT0ZkK5GVFvaU,2920
+customgpt_client/models/update_project_plugin_response_200_data.py,sha256=wCxK9atLUQ_OUOE5hNWnj7CiS7tgc3-66c4XsgIJSCw,3355
+customgpt_client/models/update_project_plugin_response_200_status.py,sha256=ArT0-lCpdM9rkTlFSm3d2TJEX6Os5vaU3B0pRf_lmz0,185
+customgpt_client/models/update_project_plugin_response_401.py,sha256=arK0n5eKRul-6tWc9Wcb-sRQUAaKq4bXID2LAf8r-aA,3206
+customgpt_client/models/update_project_plugin_response_401_data.py,sha256=yRJ1p2Agia5JWNWsciFb4vPFmO109iqYfD-1GWCqWdU,2369
+customgpt_client/models/update_project_plugin_response_401_data_code.py,sha256=bssPrpnA1Lmdv_dghQ823C7TOn8f4dPyjbfsqioGvB0,264
+customgpt_client/models/update_project_plugin_response_401_status.py,sha256=5m-CcxpFHsbSJbyfwJL4lQ2gWLOrrylWX0ls_jcrxyg,185
+customgpt_client/models/update_project_plugin_response_404.py,sha256=R4y8CkYI7LwuQ8AmSCsDY4Z0eFR-iJx37_1kdJAmBR8,3206
+customgpt_client/models/update_project_plugin_response_404_data.py,sha256=ceVF49_8R9gv0tSQGiI4nv4-oqT9-8G2xqsgZjh2B-E,2902
+customgpt_client/models/update_project_plugin_response_404_data_code.py,sha256=I5tQl0sG2A3TNoa3CXdhdz7XKiwkATK3pxf-DOkKHWc,264
+customgpt_client/models/update_project_plugin_response_404_data_message.py,sha256=BK2grwo7LVlODNuMr2LvzEBK6Mq3WlwKm6oAoPy5kl0,264
+customgpt_client/models/update_project_plugin_response_404_status.py,sha256=gWA-vXclE0XUyjvmdHSMRXyM5pk6J9iCdhW3iZY3NjU,185
+customgpt_client/models/update_project_plugin_response_500.py,sha256=af9HIrmxL8uz3AJhby-h36_zZcMI6bPeB0hpyfZhTYQ,3206
+customgpt_client/models/update_project_plugin_response_500_data.py,sha256=5qc5IV-H0lnMQFxvD6Iy4M-R8k1agUYNq_Ka1ZWCGO4,2352
+customgpt_client/models/update_project_plugin_response_500_data_code.py,sha256=OomxH13Eu4M3_wqFpxi2jWI8ZemAtAsd_qfaYiUSG0I,264
+customgpt_client/models/update_project_plugin_response_500_status.py,sha256=-0LlXqE-9utlqb9EnMP5SS0DR4oqWfqltqW9XdSE8WU,185
+customgpt_client/models/update_project_response_200.py,sha256=yO19eiLZK09fvVFx8t6hKAmOg_LCeMRXdScl85uSecw,2800
+customgpt_client/models/update_project_response_200_data.py,sha256=eR43QVe2vCpSd6dE5BK_ZMD2G6FpgJWchCnZ3Qrj1R0,8069
 customgpt_client/models/update_project_response_200_data_type.py,sha256=2b4mB17d9w2xrX4S7h272RPC0ZyMp28-U5-i8RZJXFo,177
 customgpt_client/models/update_project_response_200_status.py,sha256=etfN5tEytq8t2Z-xCQ1IY9U49SQUUFNR_VUnXewfROo,179
-customgpt_client/models/update_project_response_401.py,sha256=itU9cpOR50sh3jyIB29pPTfhWxQhJhrAAWt7CzM8cms,3107
-customgpt_client/models/update_project_response_401_data.py,sha256=fuBgdeH6k6IN-qfSxAZU4gJr-xJRqEYafQ74Q2sF0UY,2320
+customgpt_client/models/update_project_response_401.py,sha256=720Dj9M2XuvubOWy17FpNwgGVcTKCIxi4d8O6oR_hYE,3086
+customgpt_client/models/update_project_response_401_data.py,sha256=nKzAZnOZtW9JEu0HSLy5zDsxPWmhkGlfrL4rGxJJi2w,2299
 customgpt_client/models/update_project_response_401_data_code.py,sha256=hN4MCHqUuSwi8YghVOXmIyabPxfEV-OGY34f5Y4KSRo,258
 customgpt_client/models/update_project_response_401_status.py,sha256=GF5-pJ3UVLXSqC1L9nE0u7JAzc5MTeGJJh2yVcpCA6E,179
-customgpt_client/models/update_project_response_404.py,sha256=lLuR_OK88Bxp6lafbA2-an_nnNAg6mt9UBj7SxPJ1yI,3107
-customgpt_client/models/update_project_response_404_data.py,sha256=hPv9GGdOLXNJuk18ZQ5OaxAdm0noNaW2_ArLgyjfivk,2816
+customgpt_client/models/update_project_response_404.py,sha256=XbOj8U8bZh-J_NZwhHg1V8TAqYUGrX3_NBQrfIme8s4,3086
+customgpt_client/models/update_project_response_404_data.py,sha256=AxGtB34DPLmjSeG72yvcf3yktkjFkB67mJsyM84ZX_U,2795
 customgpt_client/models/update_project_response_404_data_code.py,sha256=NEqGDqMpYKsheIbD_Ch0sYJh0n8n_nABojCFqTNkDvo,258
 customgpt_client/models/update_project_response_404_data_message.py,sha256=RZ9legbDFQfMmRaQ4WzvhdO0sMCAJYnQOUJOeH00_yY,258
 customgpt_client/models/update_project_response_404_status.py,sha256=KqxNROhDqDg4z58A0bnA23yv5ApJTlVsYwXCC-VmJsU,179
-customgpt_client/models/update_project_response_500.py,sha256=62RT6BuiS6fxFyfLrviNA-17Z9Hx3F5sfPsBLU55emM,3107
-customgpt_client/models/update_project_response_500_data.py,sha256=J5lWHDyDu02ZMxQutLDZwY6_KkYNY80K4yhBl4sPEu0,2303
+customgpt_client/models/update_project_response_500.py,sha256=fHFuM2EB8VrqL3qqm7QchPfwC7sDZvD628aR2QuKeyc,3086
+customgpt_client/models/update_project_response_500_data.py,sha256=ZHnD_J0L4gM5DOfNo-11fE2xCr41K04cvvW2w5ENEbA,2282
 customgpt_client/models/update_project_response_500_data_code.py,sha256=vLZLuouRww6ubtWR6li2GE-SE9gcQWTz1ysDrAH5nMU,258
 customgpt_client/models/update_project_response_500_status.py,sha256=XJKH8ignznkHWwefHwsTLqJIDm1peNQ4K3Yc9Ej_PV8,179
-customgpt_client/models/update_project_settings_multipart_data.py,sha256=vOUmY6P4VuSBaIejVEIZGlFGksliR3xAdvv5M6o9tt0,6861
-customgpt_client/models/update_project_settings_response_200.py,sha256=7_Ys-8u1uNkdqPgSoT7RDWKAX6fvKYvzKP_zzc4VHo0,2979
-customgpt_client/models/update_project_settings_response_200_data.py,sha256=jRllCdEacFNp_0lLywsa60epo4xc9w8puyHO61f6MOQ,1680
+customgpt_client/models/update_project_settings_multipart_data.py,sha256=rTAi07oY0AWb3_ooz3XEWamrAQwqUuHR-g6oS7-l0mw,6840
+customgpt_client/models/update_project_settings_response_200.py,sha256=bNWTu5NSW9OAJHoIVhVX445JpXN0SJqgGo4YH2knOqk,2958
+customgpt_client/models/update_project_settings_response_200_data.py,sha256=7yzW3skvCBngEFhO6EEZDeMI9h5JzybCtvgl88vhYeI,1659
 customgpt_client/models/update_project_settings_response_200_status.py,sha256=HaWQtEvCP07uuF4gLt952G72ubV9fugiZxO-0Fyd3Sc,187
-customgpt_client/models/update_project_settings_response_400.py,sha256=oT5xTd5uBstcUDSWp_4AAgHF0O9rLLoIKPaexy860Uc,3265
-customgpt_client/models/update_project_settings_response_400_data.py,sha256=vgzayeIihcc_R3p4TkYhBLQqGcT3x8F3-L08exzhqJs,2976
+customgpt_client/models/update_project_settings_response_400.py,sha256=HCW3m1m-ZaOB6u4YkQA6mX-uScOS39-idozIGkqqw2U,3244
+customgpt_client/models/update_project_settings_response_400_data.py,sha256=MGBkz8BQd_TGfAVVUc7QlwdKpJBeyCRudXrJf2hdZJc,2955
 customgpt_client/models/update_project_settings_response_400_data_code.py,sha256=e-dI7AzfXu7KIaYM3BEHiKLZ-qAD1I1WJLhUtYmhzng,266
 customgpt_client/models/update_project_settings_response_400_data_message.py,sha256=5f4BoPT-SVZfhgX5gBgcejNtVMVMqcxXjS80lJRxP-4,423
 customgpt_client/models/update_project_settings_response_400_status.py,sha256=hm8obbKl-7eu90vz-zi7rA-vbL6kV1J6jG9PT5-QIeM,187
-customgpt_client/models/update_project_settings_response_401.py,sha256=eucSWiEVKAQXwCQgsF5s62MdoiYQ1iFGv3gzQoXl3tM,3265
-customgpt_client/models/update_project_settings_response_401_data.py,sha256=jnX7HvvmDN9q5q_PkZyrrHnvnpPLO6v7Ik4fSVHknV8,2412
+customgpt_client/models/update_project_settings_response_401.py,sha256=be2Xs0nWDffN2qKguXBksZv5oSsbiVaLDjy9BDND_rk,3244
+customgpt_client/models/update_project_settings_response_401_data.py,sha256=cCY9e09-TGIJi3LJyf4TAu67DY9oP3byvGnvFr7hzT4,2391
 customgpt_client/models/update_project_settings_response_401_data_code.py,sha256=jSlmiVTnDlDW8fjH3D7KmCsxB_wSMJAemT-yWzmqA5k,266
 customgpt_client/models/update_project_settings_response_401_status.py,sha256=Dqmecy3vrIaGhpwuIbbF30LqneYr92rhTsgT7AeknmI,187
-customgpt_client/models/update_project_settings_response_500.py,sha256=I79bkPKXbTNipvaVoVCMDNiY_qSDc2AanA4E3qie27w,3265
-customgpt_client/models/update_project_settings_response_500_data.py,sha256=jSJcQF0M4XWXlngOvLMUWyt8eaL_fgc6kU4tg8gbTcI,2395
+customgpt_client/models/update_project_settings_response_500.py,sha256=5ae1vb9lnwxrIfJOrtYTJKQ7-V2RBWY7LN6c4efM-sY,3244
+customgpt_client/models/update_project_settings_response_500_data.py,sha256=r5OVve37H3FH6g5C-sqCfMYAfyEWjV1l71poiHq9dzI,2374
 customgpt_client/models/update_project_settings_response_500_data_code.py,sha256=0D-PySFPGVwp17AFyFY87HPtV6jyIBFqjScCPmP5F3o,266
 customgpt_client/models/update_project_settings_response_500_status.py,sha256=BokPDahgmeV9HLSqVY-0UlgS-dL21SLSGFSeBIXezSc,187
-customgpt_client/models/update_user_profile_multipart_data.py,sha256=s0BsrSKtOz17CRLaAk8KzlqrnOrClfcaqZhRYvbXI_c,3050
-customgpt_client/models/update_user_profile_response_200.py,sha256=v0Z1MdCux8Kxd_JyBQNxdplfmbq62fE79UFWlosuZyA,2903
-customgpt_client/models/update_user_profile_response_200_data.py,sha256=obXQkhh4FodT0-L90rYVQenJ_isEiST24ipFTIJowLU,3946
+customgpt_client/models/update_user_profile_multipart_data.py,sha256=2JZ6qegjvCG3Sh9JoyT7exe5B6sE38xalADlmQbn-6I,3029
+customgpt_client/models/update_user_profile_response_200.py,sha256=7fCYKSBBe5QNNA0dbQmqRSb626x6VrwyWW7AXyJZg6w,2882
+customgpt_client/models/update_user_profile_response_200_data.py,sha256=hT7G-g25MVQZag_czUgyf81TOZukVHgqo0zdXbKUnps,3925
 customgpt_client/models/update_user_profile_response_200_status.py,sha256=8IDbnl27kUcm9u6AJHmmx8Avc_lrkhVEM2enEJjotlo,183
-customgpt_client/models/update_user_profile_response_401.py,sha256=c0-3HXnx-XEhEmWV-mL65ntx8cuvkE9XZKKwUTHfCvo,3189
-customgpt_client/models/update_user_profile_response_401_data.py,sha256=ajLvAboATyV8CruKHQ73JdkxmIvC4mY5AnEz3j7i8sQ,2368
+customgpt_client/models/update_user_profile_response_401.py,sha256=aJIaloknPPYAGJvRF_GSDIAE_Bw2m5_gp5a90qIJt98,3168
+customgpt_client/models/update_user_profile_response_401_data.py,sha256=-On9SgTy7z6jbD_QlfWCg87Cumgp9Ua0Vk3PR9Z8IHA,2347
 customgpt_client/models/update_user_profile_response_401_data_code.py,sha256=3fLyCMozcJk0c3m2lgIFP_s6-gC0P8RZOLgyweXVR6I,262
 customgpt_client/models/update_user_profile_response_401_status.py,sha256=003UX_nIk2hHJLvCAcY8EpRFxRyGlZsEi5hiPuwaDB4,183
-customgpt_client/models/update_user_profile_response_500.py,sha256=vE_fP4yX8UVMMbO-96_tctsZ8YsdS1D2AF7q5mFsRNk,3189
-customgpt_client/models/update_user_profile_response_500_data.py,sha256=MAg1i8t243owgdIi0NdEPNLAPxypRLrVIiWb_iuSpBc,2351
+customgpt_client/models/update_user_profile_response_500.py,sha256=DFB1mxDP5sTW90072fG8quTkEIv2VwreJEvDMqwZSJI,3168
+customgpt_client/models/update_user_profile_response_500_data.py,sha256=qQ42Uw6yxVZu6a5X7AdlL2nIH-yIMbIZfFo7FPNmFQ0,2330
 customgpt_client/models/update_user_profile_response_500_data_code.py,sha256=o-GDpigGzvI3qFGG1HstdR5Lx5p508fuGNvkauwP9s8,262
 customgpt_client/models/update_user_profile_response_500_status.py,sha256=sX5mpQWL7wNrEpdCiSpvQgsm1f6kaNvLlPmfSkzW-I8,183
-customgpt_client/models/user.py,sha256=Wlz5CcnbrVuJswNviFnkEthU9gCAV8GvPfnEE5DTKhI,3791
+customgpt_client/models/user.py,sha256=mgFRGG_RaO2qScwDVy9Lw-LzKPtkvfyIbrumqE42T74,3770
 customgpt_client/py.typed,sha256=8ZJUsxZiuOy1oJeVhsTWQhTG_6pTVHVXk5hJL79ebTk,25
 customgpt_client/types.py,sha256=4xaUIOliefW-5jz_p-JT2LO7-V0wKWaniHGtjPBQfvQ,993
-customgpt_client-1.1.2.dist-info/METADATA,sha256=iyRSM5Ut5mGOJnOvj86mkvWYK4QqdRpO30WTnjdYIzU,1226
-customgpt_client-1.1.2.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-customgpt_client-1.1.2.dist-info/RECORD,,
+customgpt_client-1.1.3.dist-info/METADATA,sha256=-CrUglvh4ybAvOMveIiwHvYHZbOW418ZmfTA4LDyAmk,1224
+customgpt_client-1.1.3.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+customgpt_client-1.1.3.dist-info/RECORD,,
```


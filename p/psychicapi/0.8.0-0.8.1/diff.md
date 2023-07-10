# Comparing `tmp/psychicapi-0.8.0.tar.gz` & `tmp/psychicapi-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/psychicapi-0.8.0.tar", last modified: Thu Jun 22 21:23:36 2023, max compression
+gzip compressed data, was "psychicapi-0.8.1.tar", last modified: Mon Jul 10 00:23:53 2023, max compression
```

## Comparing `psychicapi-0.8.0.tar` & `psychicapi-0.8.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-22 21:23:36.000000 psychicapi-0.8.0/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4819 2023-06-22 21:23:36.000000 psychicapi-0.8.0/PKG-INFO
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-22 21:23:36.000000 psychicapi-0.8.0/psychicapi/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       65 2023-06-12 16:34:35.000000 psychicapi-0.8.0/psychicapi/__init__.py
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     7858 2023-06-22 21:16:22.000000 psychicapi-0.8.0/psychicapi/psychic.py
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     3726 2023-06-17 23:03:51.000000 psychicapi-0.8.0/README.md
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      648 2023-06-22 21:22:03.000000 psychicapi-0.8.0/setup.py
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-22 21:23:36.000000 psychicapi-0.8.0/psychicapi.egg-info/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4819 2023-06-22 21:23:36.000000 psychicapi-0.8.0/psychicapi.egg-info/PKG-INFO
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      232 2023-06-22 21:23:36.000000 psychicapi-0.8.0/psychicapi.egg-info/SOURCES.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        9 2023-06-22 21:23:36.000000 psychicapi-0.8.0/psychicapi.egg-info/requires.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       11 2023-06-22 21:23:36.000000 psychicapi-0.8.0/psychicapi.egg-info/top_level.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        1 2023-06-22 21:23:36.000000 psychicapi-0.8.0/psychicapi.egg-info/dependency_links.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       38 2023-06-22 21:23:36.000000 psychicapi-0.8.0/setup.cfg
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-07-10 00:23:53.478316 psychicapi-0.8.1/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4537 2023-07-10 00:23:53.478184 psychicapi-0.8.1/PKG-INFO
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4271 2023-07-10 00:22:36.000000 psychicapi-0.8.1/README.md
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-07-10 00:23:53.477341 psychicapi-0.8.1/psychicapi/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       65 2023-07-07 03:04:36.000000 psychicapi-0.8.1/psychicapi/__init__.py
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     8870 2023-07-10 00:21:30.000000 psychicapi-0.8.1/psychicapi/psychic.py
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-07-10 00:23:53.478028 psychicapi-0.8.1/psychicapi.egg-info/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4537 2023-07-10 00:23:53.000000 psychicapi-0.8.1/psychicapi.egg-info/PKG-INFO
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      232 2023-07-10 00:23:53.000000 psychicapi-0.8.1/psychicapi.egg-info/SOURCES.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        1 2023-07-10 00:23:53.000000 psychicapi-0.8.1/psychicapi.egg-info/dependency_links.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        9 2023-07-10 00:23:53.000000 psychicapi-0.8.1/psychicapi.egg-info/requires.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       11 2023-07-10 00:23:53.000000 psychicapi-0.8.1/psychicapi.egg-info/top_level.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       38 2023-07-10 00:23:53.478355 psychicapi-0.8.1/setup.cfg
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      648 2023-07-10 00:23:00.000000 psychicapi-0.8.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `psychicapi-0.8.0/PKG-INFO` & `psychicapi-0.8.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,106 +1,113 @@
-Metadata-Version: 2.1
-Name: psychicapi
-Version: 0.8.0
-Summary: Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic
-Home-page: UNKNOWN
-Author: Ayan Bandyopadhyay
-Author-email: ayan@psychic.dev
-License: UNKNOWN
-Description: # Psychic
-        
-        `psychicapi` is the python client library for [Psychic](https://www.psychic.dev/).
-        
-        ## What is Psychic?
-        
-        Psychic is a platform for integrating with your customer’s SaaS tools like Notion, Zendesk, Confluence, and Google Drive via OAuth and syncing documents from these applications to your SQL or vector database. You can think of it like Plaid for unstructured data. Psychic is easy to set up - you use it by importing the react library and configuring it with your Psychic API key, which you can get from the [Psychic dashboard](https://dashboard.psychic.dev/). When your users connect their applications, you can view these connections from the dashboard and retrieve data using the server-side libraries. 
-        
-        ## Quick start
-        
-        1. Create an account in the [dashboard](https://dashboard.psychic.dev/).
-        2. Use the [react library](https://docs.psychic.dev/psychic-link) to add the Psychic link modal to your frontend react app. Users will use this to connect their SaaS apps. Or, use the [playground](https://dashboard.psychic.dev/playground) to connect your own data sources.
-        3. Use `psychicapi` to retrieve documents from your active connections.
-        
-        ## Usage 
-        
-        ### Initialization
-        
-        ```
-        from psychicapi import ConnectorId, Psychic 
-        psychic = Psychic(secret_key="secret-key")
-        ```
-        
-        ### Get active connections
-        
-        ```
-        # Get all active connections and optionally filter by connector id and/or account id
-        connections = psychic.get_connections(account_id="account_id")
-        ```
-        
-        ### Retrieve documents from a connection
-        
-        ```
-        page_cursor = None
-        all_docs = []
-        while True:
-            docs_response = psychic.get_documents(account_id="account_id", connector_id=ConnectorId.notion, page_cursor=page_cursor, page_size=100)
-            if docs_response is None:
-                break
-            all_docs.extend(docs_response.documents)
-            page_cursor = docs_response.next_page_cursor
-            if page_cursor is None:
-                break
-        print(all_docs)
-        ```
-        
-        ## Advanced Filtering
-        
-        ### Filtering by section(s)
-        
-        Most file storage, CRM and helpdesk apps have documents organized in sections. Confluence calls them spaces, Zendesk calls them  sections, Google Drive calls them folders. Psychic allows you to define filters based on these sections using the `SectionFilter` class. You can define and query sections as follows:
-        
-        ```
-        from psychicapi import Psychic, ConnectorId, Section, SectionFilter
-        
-        client = Psychic("YOUR-SECRET-KEY")
-        connections = client.get_connections(connector_id=ConnectorId.notion, account_id="test")
-        connection = connections[0]
-        
-        # get existing section filters
-        existing_filters = connection.section_filters
-        
-        # get all available sections from the connection. these will be folders, sections, spaces, etc. depending on the connector
-        sections = connection.sections
-        
-        # have the user pick one or more sections
-        i = 0
-        filter = SectionFilter(id='index1', sections=[sections[i]])
-        
-        # add the section filter to the connection
-        client.add_section_filter(connector_id=ConnectorId.notion, account_id="test", section_filter=filter)
-        
-        # get documents from the sections in the filter
-        client.get_documents(account_id="test", connector_id=ConnectorId.notion, section_filter_id="index1")
-        ```
-        
-        ### Filtering by uri
-        
-        Every document returned by Psychic has a uri. If you want to query a document by uri instead of retrieving all documents in a connection, you can use the optional `uris` parameter in `get_documents`
-        
-        
-        ```
-        client.get_documents(
-            account_id="test", 
-            connector_id=ConnectorId.notion, 
-            uris=["https://docs.google.com/document/d/document-id-1/edit?usp=drivesdk", "https://drive.google.com/file/d/document-id-2/view?usp=drivesdk"]
-        )
-        ```
-        ## Local development
-        
-        To run the python package locally, use the following command:
-        
-        ```
-        pip install -e /path/to/package
-        ```
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+# Psychic
+
+`psychicapi` is the python client library for [Psychic](https://www.psychic.dev/).
+
+## What is Psychic?
+
+Psychic is a platform for integrating with your customer’s SaaS tools like Notion, Zendesk, Confluence, and Google Drive via OAuth and syncing documents from these applications to your SQL or vector database. You can think of it like Plaid for unstructured data. Psychic is easy to set up - you use it by importing the react library and configuring it with your Psychic API key, which you can get from the [Psychic dashboard](https://dashboard.psychic.dev/). When your users connect their applications, you can view these connections from the dashboard and retrieve data using the server-side libraries. 
+
+## Quick start
+
+1. Create an account in the [dashboard](https://dashboard.psychic.dev/).
+2. Use the [react library](https://docs.psychic.dev/psychic-link) to add the Psychic link modal to your frontend react app. Users will use this to connect their SaaS apps. Or, use the [playground](https://dashboard.psychic.dev/playground) to connect your own data sources.
+3. Use `psychicapi` to retrieve documents from your active connections.
+
+## Usage 
+
+### Initialization
+
+```
+from psychicapi import ConnectorId, Psychic 
+psychic = Psychic(secret_key="secret-key")
+```
+
+### Get active connections
+
+```
+# Get all active connections and optionally filter by connector id and/or account id
+connections = psychic.get_connections(account_id="account_id")
+```
+
+### Retrieve documents from a connection
+
+```
+page_cursor = None
+all_docs = []
+while True:
+    docs_response = psychic.get_documents(account_id="account_id", connector_id=ConnectorId.notion, page_cursor=page_cursor, page_size=100)
+    if docs_response is None:
+        break
+    all_docs.extend(docs_response.documents)
+    page_cursor = docs_response.next_page_cursor
+    if page_cursor is None:
+        break
+print(all_docs)
+```
+
+### Retrieve messages from a connection
+
+To retrieve messages from connectors like `slack` and `gmail`, use the `get_conversations` function.
+
+```
+page_cursor = None
+all_messages = []
+while True:
+    messages_response = psychic.get_documents(account_id="account_id", connector_id=ConnectorId.notion, page_cursor=page_cursor)
+    if messages_response is None:
+        break
+    all_messages.extend(messages_response.messages)
+    page_cursor = messages_response.next_page_cursor
+    if page_cursor is None:
+        break
+print(all_messages)
+```
+
+## Advanced Filtering
+
+### Filtering by section(s)
+
+Most file storage, CRM and helpdesk apps have documents organized in sections. Confluence calls them spaces, Zendesk calls them  sections, Google Drive calls them folders. Psychic allows you to define filters based on these sections using the `SectionFilter` class. You can define and query sections as follows:
+
+```
+from psychicapi import Psychic, ConnectorId, Section, SectionFilter
+
+client = Psychic("YOUR-SECRET-KEY")
+connections = client.get_connections(connector_id=ConnectorId.notion, account_id="test")
+connection = connections[0]
+
+# get existing section filters
+existing_filters = connection.section_filters
+
+# get all available sections from the connection. these will be folders, sections, spaces, etc. depending on the connector
+sections = connection.sections
+
+# have the user pick one or more sections
+i = 0
+filter = SectionFilter(id='index1', sections=[sections[i]])
+
+# add the section filter to the connection
+client.add_section_filter(connector_id=ConnectorId.notion, account_id="test", section_filter=filter)
+
+# get documents from the sections in the filter
+client.get_documents(account_id="test", connector_id=ConnectorId.notion, section_filter_id="index1")
+```
+
+### Filtering by uri
+
+Every document returned by Psychic has a uri. If you want to query a document by uri instead of retrieving all documents in a connection, you can use the optional `uris` parameter in `get_documents`
+
+
+```
+client.get_documents(
+    account_id="test", 
+    connector_id=ConnectorId.notion, 
+    uris=["https://docs.google.com/document/d/document-id-1/edit?usp=drivesdk", "https://drive.google.com/file/d/document-id-2/view?usp=drivesdk"]
+)
+```
+## Local development
+
+To run the python package locally, use the following command:
+
+```
+pip install -e /path/to/package
+```
```

### Comparing `psychicapi-0.8.0/psychicapi/psychic.py` & `psychicapi-0.8.1/psychicapi/psychic.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,211 +1,287 @@
 import requests
 from enum import Enum
 from typing import List, Optional, Dict, Any
 
+
 class ConnectorId(Enum):
-    notion = "notion"
     confluence = "confluence"
-    zendesk = "zendesk"
+    dropbox = "dropbox"
     gdrive = "gdrive"
+    github = "github"
+    gmail = "gmail"
+    hubspot = "hubspot"
+    intercom = "intercom"
+    notion = "notion"
+    readme = "readme"
+    salesforce = "salesforce"
+    sharepoint = "sharepoint"
     slack = "slack"
+    web = "web"
+    zendesk = "zendesk"
+
 
 class SectionType(str, Enum):
     folder = "folder"
     document = "document"
 
+
 class Section:
     id: str
     name: str
     type: SectionType
     children: Optional[List["Section"]] = None
 
-    def __init__(self, id: str, name: str, type: SectionType, children: Optional[List["Section"]] = None) -> None:
+    def __init__(
+        self,
+        id: str,
+        name: str,
+        type: SectionType,
+        children: Optional[List["Section"]] = None,
+    ) -> None:
         self.id = id
         self.name = name
         self.type = type
         self.children = children
 
+
 class SectionFilter:
     id: str
     sections: List[Section]
 
     def __init__(self, id: str, sections: List[Section]) -> None:
         self.id = id
         self.sections = sections
 
+
 class ConnectionFilter:
     account_id: str
     connector_id: Optional[ConnectorId] = None
     uris: Optional[List[str]] = None
     section_filter_id: Optional[str] = None
 
+
 class Connection:
     account_id: str
     connector_id: ConnectorId
     metadata: Dict
     section_filters: List[SectionFilter] = []
     sections: Optional[List[Section]] = None
     credential: Optional[str]
     config: Optional[Any]
 
-    def __init__(self, account_id: str, connector_id: ConnectorId, metadata: Dict, section_filters: List[SectionFilter] = [], sections: Optional[List[Section]] = None, credential: Optional[str] = None, config: Optional[Any] = None) -> None:
+    def __init__(
+        self,
+        account_id: str,
+        connector_id: ConnectorId,
+        metadata: Dict,
+        section_filters: List[SectionFilter] = [],
+        sections: Optional[List[Section]] = None,
+        credential: Optional[str] = None,
+        config: Optional[Any] = None,
+    ) -> None:
         self.account_id = account_id
         self.connector_id = connector_id
         self.metadata = metadata
         self.section_filters = section_filters
         self.sections = sections
         self.credential = credential
         self.config = config
 
+
+class GetConversationsResponse:
+    messages: List[Dict]
+    next_page_cursor: Optional[str] = None
+
+    def __init__(self, messages: List[Dict], next_page_cursor: Optional[str]) -> None:
+        self.messages = messages
+        self.next_page_cursor = next_page_cursor
+
+
 class GetDocumentsResponse:
     documents: List[Dict]
     next_page_cursor: Optional[str] = None
 
-    def __init__(self, documents: List[Dict], next_page_cursor: Optional[str] = None) -> None:
+    def __init__(
+        self, documents: List[Dict], next_page_cursor: Optional[str] = None
+    ) -> None:
         self.documents = documents
         self.next_page_cursor = next_page_cursor
 
+
 class ChunkingOptions:
     min_chunk_size: Optional[int] = None
     max_chunk_size: Optional[int] = None
 
+
 class Psychic:
     def __init__(self, secret_key: str):
         self.api_url = "https://api.psychic.dev/"
         self.secret_key = secret_key
 
     def handle_http_error(self, response: requests.Response):
         if response.status_code == 401 or response.status_code == 403:
             raise Exception("Unauthorized: Invalid or missing secret key")
         try:
             data = response.json()
-            message = data.get('detail', 'No additional information')
+            message = data.get("detail", "No additional information")
         except requests.exceptions.JSONDecodeError:
-            message = 'No additional information'
+            message = "No additional information"
         raise Exception(f"HTTP error {response.status_code}: {message}")
 
-    def get_documents(self, 
-                      *, 
-                      account_id: str, 
-                      connector_id: Optional[ConnectorId] = None, 
-                      section_filter_id: Optional[str] = None, 
-                      uris: Optional[List[str]] = None, 
-                      chunked: Optional[bool] = False, 
-                      min_chunk_size: Optional[int] = None, 
-                      max_chunk_size: Optional[int] = None,
-                      page_cursor: Optional[str] = None,
-                      page_size: Optional[int] = 100):
+    def get_documents(
+        self,
+        *,
+        account_id: str,
+        connector_id: Optional[ConnectorId] = None,
+        section_filter_id: Optional[str] = None,
+        uris: Optional[List[str]] = None,
+        chunked: Optional[bool] = False,
+        min_chunk_size: Optional[int] = None,
+        max_chunk_size: Optional[int] = None,
+        page_cursor: Optional[str] = None,
+        page_size: Optional[int] = 100,
+    ):
         body = {
             "account_id": account_id,
             "connector_id": connector_id.value if connector_id is not None else None,
             "section_filter_id": section_filter_id,
             "uris": uris,
             "chunked": chunked,
             "min_chunk_size": min_chunk_size,
             "max_chunk_size": max_chunk_size,
             "page_cursor": page_cursor,
-            "page_size": page_size
+            "page_size": page_size,
         }
         response = requests.post(
             self.api_url + "get-documents",
             json=body,
             headers={
-                'Authorization': 'Bearer ' + self.secret_key,
-                'Accept': 'application/json'
-            }
+                "Authorization": "Bearer " + self.secret_key,
+                "Accept": "application/json",
+            },
         )
         if response.status_code == 200:
             data = response.json()
             documents = data["documents"]
             next_page_cursor = data["next_page_cursor"]
-            return GetDocumentsResponse(documents=documents, next_page_cursor=next_page_cursor)
+            return GetDocumentsResponse(
+                documents=documents, next_page_cursor=next_page_cursor
+            )
         else:
             self.handle_http_error(response)
-        
-    def get_connections(self, *, connector_id: Optional[ConnectorId] = None, account_id: Optional[str] = None):
+
+    def get_connections(
+        self,
+        *,
+        connector_id: Optional[ConnectorId] = None,
+        account_id: Optional[str] = None,
+    ):
         filter = {
             "connector_id": connector_id.value if connector_id is not None else None,
-            "account_id": account_id
+            "account_id": account_id,
         }
 
         response = requests.post(
             self.api_url + "get-connections",
             json={
                 "filter": filter,
             },
             headers={
-                'Authorization': 'Bearer ' + self.secret_key,
-                'Accept': 'application/json'
-            }
+                "Authorization": "Bearer " + self.secret_key,
+                "Accept": "application/json",
+            },
         )
         if response.status_code == 200:
             connections = response.json()["connections"]
             for connection in connections:
                 connection["connector_id"] = ConnectorId(connection["connector_id"])
                 if connection.get("sections"):
-                    connection["sections"] = [Section(**section) for section in connection["sections"]]
+                    connection["sections"] = [
+                        Section(**section) for section in connection["sections"]
+                    ]
                 if connection.get("section_filters"):
                     typed_section_filters = []
                     for section_filter in connection["section_filters"]:
-                        sections = [Section(**section) for section in section_filter["sections"]]
+                        sections = [
+                            Section(**section) for section in section_filter["sections"]
+                        ]
                         id = section_filter["id"]
-                        typed_section_filters.append(SectionFilter(id=id, sections=sections))
+                        typed_section_filters.append(
+                            SectionFilter(id=id, sections=sections)
+                        )
                     connection["section_filters"] = typed_section_filters
 
             return [Connection(**connection) for connection in connections]
         else:
             self.handle_http_error(response)
-        
-    def add_section_filter(self, *, connector_id: ConnectorId, account_id: str, section_filter: SectionFilter):
+
+    def add_section_filter(
+        self,
+        *,
+        connector_id: ConnectorId,
+        account_id: str,
+        section_filter: SectionFilter,
+    ):
         body = {
             "connector_id": connector_id.value,
             "account_id": account_id,
             "section_filter": {
                 "id": section_filter.id,
                 "sections": [
-                    {
-                        "id": section.id,
-                        "name": section.name,
-                        "type": section.type
-                    }
+                    {"id": section.id, "name": section.name, "type": section.type}
                     for section in section_filter.sections
-                ]
-            }    
+                ],
+            },
         }
         response = requests.post(
             self.api_url + "add-section-filter",
             json=body,
             headers={
-                'Authorization': 'Bearer ' + self.secret_key,
-                'Accept': 'application/json'
-            }
+                "Authorization": "Bearer " + self.secret_key,
+                "Accept": "application/json",
+            },
         )
         if response.status_code == 200:
             filter = response.json()["section_filter"]
-            filter = SectionFilter(id=filter["id"], sections=[Section(**section) for section in filter["sections"]])
+            filter = SectionFilter(
+                id=filter["id"],
+                sections=[Section(**section) for section in filter["sections"]],
+            )
             return filter
         else:
             self.handle_http_error(response)
 
-        
-    def get_conversations(self, *, account_id: str, connector_id: ConnectorId, oldest_timestamp: Optional[int] = None):
+    def get_conversations(
+        self,
+        *,
+        account_id: str,
+        connector_id: ConnectorId,
+        page_cursor: Optional[str] = None,
+        oldest_timestamp: Optional[int] = None,
+    ):
         body = {
             "connector_id": connector_id.value,
             "account_id": account_id,
+            "page_cursor": page_cursor,
         }
         if oldest_timestamp is not None:
             body["oldest_timestamp"] = oldest_timestamp
 
         response = requests.post(
             self.api_url + "get-conversations",
             json=body,
             headers={
-                'Authorization': 'Bearer ' + self.secret_key,
-                'Accept': 'application/json'
-            }
+                "Authorization": "Bearer " + self.secret_key,
+                "Accept": "application/json",
+            },
         )
         if response.status_code == 200:
-            messages = response.json()["messages"]
-            return messages
+            data = response.json()
+            messages = data["messages"]
+            next_page_cursor = data["next_page_cursor"]
+            return GetConversationsResponse(
+                messages=messages, next_page_cursor=next_page_cursor
+            )
+
         else:
-            self.handle_http_error(response)
+            self.handle_http_error(response)
```

### Comparing `psychicapi-0.8.0/README.md` & `psychicapi-0.8.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: psychicapi
+Version: 0.8.1
+Summary: Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic
+Author: Ayan Bandyopadhyay
+Author-email: ayan@psychic.dev
+Description-Content-Type: text/markdown
+
 # Psychic
 
 `psychicapi` is the python client library for [Psychic](https://www.psychic.dev/).
 
 ## What is Psychic?
 
 Psychic is a platform for integrating with your customer’s SaaS tools like Notion, Zendesk, Confluence, and Google Drive via OAuth and syncing documents from these applications to your SQL or vector database. You can think of it like Plaid for unstructured data. Psychic is easy to set up - you use it by importing the react library and configuring it with your Psychic API key, which you can get from the [Psychic dashboard](https://dashboard.psychic.dev/). When your users connect their applications, you can view these connections from the dashboard and retrieve data using the server-side libraries. 
@@ -40,14 +48,32 @@
     all_docs.extend(docs_response.documents)
     page_cursor = docs_response.next_page_cursor
     if page_cursor is None:
         break
 print(all_docs)
 ```
 
+### Retrieve messages from a connection
+
+To retrieve messages from connectors like `slack` and `gmail`, use the `get_conversations` function.
+
+```
+page_cursor = None
+all_messages = []
+while True:
+    messages_response = psychic.get_documents(account_id="account_id", connector_id=ConnectorId.notion, page_cursor=page_cursor)
+    if messages_response is None:
+        break
+    all_messages.extend(messages_response.messages)
+    page_cursor = messages_response.next_page_cursor
+    if page_cursor is None:
+        break
+print(all_messages)
+```
+
 ## Advanced Filtering
 
 ### Filtering by section(s)
 
 Most file storage, CRM and helpdesk apps have documents organized in sections. Confluence calls them spaces, Zendesk calls them  sections, Google Drive calls them folders. Psychic allows you to define filters based on these sections using the `SectionFilter` class. You can define and query sections as follows:
 
 ```
```

### Comparing `psychicapi-0.8.0/setup.py` & `psychicapi-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md')) as f:
     long_description = f.read()
 
 setup(
     name='psychicapi',
-    version='0.8.0',
+    version='0.8.1',
     description='Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayan Bandyopadhyay',
     author_email='ayan@psychic.dev',
     packages=['psychicapi'],
     install_requires=[
```

### Comparing `psychicapi-0.8.0/psychicapi.egg-info/PKG-INFO` & `psychicapi-0.8.1/psychicapi.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,106 +1,121 @@
 Metadata-Version: 2.1
 Name: psychicapi
-Version: 0.8.0
+Version: 0.8.1
 Summary: Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic
-Home-page: UNKNOWN
 Author: Ayan Bandyopadhyay
 Author-email: ayan@psychic.dev
-License: UNKNOWN
-Description: # Psychic
-        
-        `psychicapi` is the python client library for [Psychic](https://www.psychic.dev/).
-        
-        ## What is Psychic?
-        
-        Psychic is a platform for integrating with your customer’s SaaS tools like Notion, Zendesk, Confluence, and Google Drive via OAuth and syncing documents from these applications to your SQL or vector database. You can think of it like Plaid for unstructured data. Psychic is easy to set up - you use it by importing the react library and configuring it with your Psychic API key, which you can get from the [Psychic dashboard](https://dashboard.psychic.dev/). When your users connect their applications, you can view these connections from the dashboard and retrieve data using the server-side libraries. 
-        
-        ## Quick start
-        
-        1. Create an account in the [dashboard](https://dashboard.psychic.dev/).
-        2. Use the [react library](https://docs.psychic.dev/psychic-link) to add the Psychic link modal to your frontend react app. Users will use this to connect their SaaS apps. Or, use the [playground](https://dashboard.psychic.dev/playground) to connect your own data sources.
-        3. Use `psychicapi` to retrieve documents from your active connections.
-        
-        ## Usage 
-        
-        ### Initialization
-        
-        ```
-        from psychicapi import ConnectorId, Psychic 
-        psychic = Psychic(secret_key="secret-key")
-        ```
-        
-        ### Get active connections
-        
-        ```
-        # Get all active connections and optionally filter by connector id and/or account id
-        connections = psychic.get_connections(account_id="account_id")
-        ```
-        
-        ### Retrieve documents from a connection
-        
-        ```
-        page_cursor = None
-        all_docs = []
-        while True:
-            docs_response = psychic.get_documents(account_id="account_id", connector_id=ConnectorId.notion, page_cursor=page_cursor, page_size=100)
-            if docs_response is None:
-                break
-            all_docs.extend(docs_response.documents)
-            page_cursor = docs_response.next_page_cursor
-            if page_cursor is None:
-                break
-        print(all_docs)
-        ```
-        
-        ## Advanced Filtering
-        
-        ### Filtering by section(s)
-        
-        Most file storage, CRM and helpdesk apps have documents organized in sections. Confluence calls them spaces, Zendesk calls them  sections, Google Drive calls them folders. Psychic allows you to define filters based on these sections using the `SectionFilter` class. You can define and query sections as follows:
-        
-        ```
-        from psychicapi import Psychic, ConnectorId, Section, SectionFilter
-        
-        client = Psychic("YOUR-SECRET-KEY")
-        connections = client.get_connections(connector_id=ConnectorId.notion, account_id="test")
-        connection = connections[0]
-        
-        # get existing section filters
-        existing_filters = connection.section_filters
-        
-        # get all available sections from the connection. these will be folders, sections, spaces, etc. depending on the connector
-        sections = connection.sections
-        
-        # have the user pick one or more sections
-        i = 0
-        filter = SectionFilter(id='index1', sections=[sections[i]])
-        
-        # add the section filter to the connection
-        client.add_section_filter(connector_id=ConnectorId.notion, account_id="test", section_filter=filter)
-        
-        # get documents from the sections in the filter
-        client.get_documents(account_id="test", connector_id=ConnectorId.notion, section_filter_id="index1")
-        ```
-        
-        ### Filtering by uri
-        
-        Every document returned by Psychic has a uri. If you want to query a document by uri instead of retrieving all documents in a connection, you can use the optional `uris` parameter in `get_documents`
-        
-        
-        ```
-        client.get_documents(
-            account_id="test", 
-            connector_id=ConnectorId.notion, 
-            uris=["https://docs.google.com/document/d/document-id-1/edit?usp=drivesdk", "https://drive.google.com/file/d/document-id-2/view?usp=drivesdk"]
-        )
-        ```
-        ## Local development
-        
-        To run the python package locally, use the following command:
-        
-        ```
-        pip install -e /path/to/package
-        ```
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+
+# Psychic
+
+`psychicapi` is the python client library for [Psychic](https://www.psychic.dev/).
+
+## What is Psychic?
+
+Psychic is a platform for integrating with your customer’s SaaS tools like Notion, Zendesk, Confluence, and Google Drive via OAuth and syncing documents from these applications to your SQL or vector database. You can think of it like Plaid for unstructured data. Psychic is easy to set up - you use it by importing the react library and configuring it with your Psychic API key, which you can get from the [Psychic dashboard](https://dashboard.psychic.dev/). When your users connect their applications, you can view these connections from the dashboard and retrieve data using the server-side libraries. 
+
+## Quick start
+
+1. Create an account in the [dashboard](https://dashboard.psychic.dev/).
+2. Use the [react library](https://docs.psychic.dev/psychic-link) to add the Psychic link modal to your frontend react app. Users will use this to connect their SaaS apps. Or, use the [playground](https://dashboard.psychic.dev/playground) to connect your own data sources.
+3. Use `psychicapi` to retrieve documents from your active connections.
+
+## Usage 
+
+### Initialization
+
+```
+from psychicapi import ConnectorId, Psychic 
+psychic = Psychic(secret_key="secret-key")
+```
+
+### Get active connections
+
+```
+# Get all active connections and optionally filter by connector id and/or account id
+connections = psychic.get_connections(account_id="account_id")
+```
+
+### Retrieve documents from a connection
+
+```
+page_cursor = None
+all_docs = []
+while True:
+    docs_response = psychic.get_documents(account_id="account_id", connector_id=ConnectorId.notion, page_cursor=page_cursor, page_size=100)
+    if docs_response is None:
+        break
+    all_docs.extend(docs_response.documents)
+    page_cursor = docs_response.next_page_cursor
+    if page_cursor is None:
+        break
+print(all_docs)
+```
+
+### Retrieve messages from a connection
+
+To retrieve messages from connectors like `slack` and `gmail`, use the `get_conversations` function.
+
+```
+page_cursor = None
+all_messages = []
+while True:
+    messages_response = psychic.get_documents(account_id="account_id", connector_id=ConnectorId.notion, page_cursor=page_cursor)
+    if messages_response is None:
+        break
+    all_messages.extend(messages_response.messages)
+    page_cursor = messages_response.next_page_cursor
+    if page_cursor is None:
+        break
+print(all_messages)
+```
+
+## Advanced Filtering
+
+### Filtering by section(s)
+
+Most file storage, CRM and helpdesk apps have documents organized in sections. Confluence calls them spaces, Zendesk calls them  sections, Google Drive calls them folders. Psychic allows you to define filters based on these sections using the `SectionFilter` class. You can define and query sections as follows:
+
+```
+from psychicapi import Psychic, ConnectorId, Section, SectionFilter
+
+client = Psychic("YOUR-SECRET-KEY")
+connections = client.get_connections(connector_id=ConnectorId.notion, account_id="test")
+connection = connections[0]
+
+# get existing section filters
+existing_filters = connection.section_filters
+
+# get all available sections from the connection. these will be folders, sections, spaces, etc. depending on the connector
+sections = connection.sections
+
+# have the user pick one or more sections
+i = 0
+filter = SectionFilter(id='index1', sections=[sections[i]])
+
+# add the section filter to the connection
+client.add_section_filter(connector_id=ConnectorId.notion, account_id="test", section_filter=filter)
+
+# get documents from the sections in the filter
+client.get_documents(account_id="test", connector_id=ConnectorId.notion, section_filter_id="index1")
+```
+
+### Filtering by uri
+
+Every document returned by Psychic has a uri. If you want to query a document by uri instead of retrieving all documents in a connection, you can use the optional `uris` parameter in `get_documents`
+
+
+```
+client.get_documents(
+    account_id="test", 
+    connector_id=ConnectorId.notion, 
+    uris=["https://docs.google.com/document/d/document-id-1/edit?usp=drivesdk", "https://drive.google.com/file/d/document-id-2/view?usp=drivesdk"]
+)
+```
+## Local development
+
+To run the python package locally, use the following command:
+
+```
+pip install -e /path/to/package
+```
```


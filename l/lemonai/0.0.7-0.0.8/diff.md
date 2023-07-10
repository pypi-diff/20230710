# Comparing `tmp/lemonai-0.0.7.tar.gz` & `tmp/lemonai-0.0.8.tar.gz`

## Comparing `lemonai-0.0.7.tar` & `lemonai-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,19 @@
--rw-r--r--   0        0        0  5358251 2020-02-02 00:00:00.000000 lemonai-0.0.7/heatmap-example.gif
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 lemonai-0.0.7/src/lemonai/__init__.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 lemonai-0.0.7/src/lemonai/api_wrapper.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 lemonai-0.0.7/src/lemonai/execute_workflow.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 lemonai-0.0.7/src/lemonai/filter_tools.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 lemonai-0.0.7/src/lemonai/get_integrations.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 lemonai-0.0.7/src/lemonai/tool.py
--rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 lemonai-0.0.7/src/lemonai/toolkit.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 lemonai-0.0.7/src/lemonai/workflow.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lemonai-0.0.7/tests/.gitkeep
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 lemonai-0.0.7/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 lemonai-0.0.7/LICENSE
--rw-r--r--   0        0        0    11953 2020-02-02 00:00:00.000000 lemonai-0.0.7/README.md
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 lemonai-0.0.7/pyproject.toml
--rw-r--r--   0        0        0    12698 2020-02-02 00:00:00.000000 lemonai-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0  5358251 2020-02-02 00:00:00.000000 lemonai-0.0.8/heatmap-example.gif
+-rw-r--r--   0        0        0   459819 2020-02-02 00:00:00.000000 lemonai-0.0.8/heatmap-example.png
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 lemonai-0.0.8/test.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 lemonai-0.0.8/.vscode/launch.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 lemonai-0.0.8/.vscode/settings.json
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 lemonai-0.0.8/src/lemonai/__init__.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 lemonai-0.0.8/src/lemonai/api_wrapper.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 lemonai-0.0.8/src/lemonai/execute_workflow.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 lemonai-0.0.8/src/lemonai/filter_tools.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 lemonai-0.0.8/src/lemonai/get_integrations.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 lemonai-0.0.8/src/lemonai/tool.py
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 lemonai-0.0.8/src/lemonai/toolkit.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 lemonai-0.0.8/src/lemonai/workflow.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lemonai-0.0.8/tests/.gitkeep
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 lemonai-0.0.8/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 lemonai-0.0.8/LICENSE
+-rw-r--r--   0        0        0    12607 2020-02-02 00:00:00.000000 lemonai-0.0.8/README.md
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 lemonai-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0    13352 2020-02-02 00:00:00.000000 lemonai-0.0.8/PKG-INFO
```

### Comparing `lemonai-0.0.7/heatmap-example.gif` & `lemonai-0.0.8/heatmap-example.gif`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.7/src/lemonai/api_wrapper.py` & `lemonai-0.0.8/src/lemonai/api_wrapper.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.7/src/lemonai/execute_workflow.py` & `lemonai-0.0.8/src/lemonai/execute_workflow.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,16 +16,15 @@
     api_keys_dict, access_tokens_dict = get_apis_from_env()
     session_id = uuid.uuid4()
 
     _wrapper = APIWrapper()
     toolkit = Toolkit.from_api_wrapper(_wrapper, api_keys_dict, access_tokens_dict, logger, str(session_id))
     tools = toolkit.get_tools()
 
-    prompt = f"Your task is '{prompt_string}'. Focus on the ordering of the tasks given. Do not use a workflow unless it is mentioned. Give your action input as a valid JSON object where the keys are the params and the values are the value for each input parameter. If a param is optional and you have not been given a value, do not include that field in the input. Your final answer should give a brief conversational overview of what you did."
-    
+    prompt = f"Your task is '{prompt_string}'. Focus on the ordering of the tasks given. Do not use a workflow unless it is mentioned. Give your action input as a valid JSON object where the keys are the params and the values are the value for each input parameter. The description of the tool may provide the JSON structure of the action input using round brackets () instead of curly brackets. Follow this structure for your action input. Your final answer should give a brief conversational overview of what you did."    
     filtered_tools = filter_tools(llm=llm, task=prompt_string, tools=tools)
     
     agent = initialize_agent(
         tools=filtered_tools,
         llm=llm,
         agent=AgentType.ZERO_SHOT_REACT_DESCRIPTION,
         verbose=True
```

### Comparing `lemonai-0.0.7/src/lemonai/filter_tools.py` & `lemonai-0.0.8/src/lemonai/filter_tools.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.7/src/lemonai/get_integrations.py` & `lemonai-0.0.8/src/lemonai/get_integrations.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.7/src/lemonai/tool.py` & `lemonai-0.0.8/src/lemonai/tool.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.7/src/lemonai/toolkit.py` & `lemonai-0.0.8/src/lemonai/toolkit.py`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.7/.gitignore` & `lemonai-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.7/LICENSE` & `lemonai-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lemonai-0.0.7/README.md` & `lemonai-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # 🍋 Lemon AI
 
+![Heatmap Example](heatmap-example.gif)
+
 ## About
 
-**Build powerful AI assistants in minutes and execute highly efficient workflow automations by accessing tools like Airtable, Hubspot, Slack and Github.**
+**Build powerful AI assistants in minutes and execute highly efficient workflow automations by accessing tools like Airtable, Hubspot, Notion, Slack and Github.**
 
 Most connectors available today are focused on read-only operations, limiting the potential of LLMs. Agents, on the other hand, have a tendency to hallucinate from time to time due to missing context or instructions.
 
 With Lemon AI, it is possible to give your agents access to well-defined APIs for more reliable read and write operations. In addition, Lemon AI functions allow you to reduce the risk of hallucinations even more by providing a way to statically define workflows that the model can rely on in case of insecurity.
 
 ## 🖲️ Getting Started
 
@@ -115,17 +117,17 @@
 ```log
 2023-06-26T11:50:27.708785+0100 - b5f91c59-8487-45c2-800a-156eac0c7dae - HackerNews: Get User
 2023-06-26T11:50:39.624035+0100 - b5f91c59-8487-45c2-800a-156eac0c7dae - Airtable: Append the data to a table
 2023-06-26T11:58:32.925228+0100 - 5efe603c-9898-4143-b99a-55b50007ed9d - HackerNews: Get User
 2023-06-26T11:58:43.988788+0100 - 5efe603c-9898-4143-b99a-55b50007ed9d - Airtable: Append the data to a table
 ```
 
-By using the [Lemon AI Analytics Notebook](https://github.com/felixbrock/lemonai-analytics) you can easily gain a better understanding of how frequently and in which workflow combination tools are used. As a result you can identify weak spots in your agent’s decision making capabilities and move to a more deterministic behaviour by defining [Lemon AI functions](#lemon-ai-functions---solve-tasks-based-on-predefined-workflows):
+By using the [Lemon AI Analytics Tool](https://github.com/felixbrock/lemonai-analytics) you can easily gain a better understanding of how frequently and in which workflow combination tools are used. As a result you can identify weak spots in your agent’s decision making capabilities and move to a more deterministic behaviour by defining [Lemon AI functions](#lemon-ai-functions---solve-tasks-based-on-predefined-workflows):
 
-![Heatmap Example](heatmap-example.gif)
+![Heatmap Example](heatmap-example.png)
 
 ## Supported Tools
 
 Below is a list of all tools supported by Lemon AI and their ids (for use in the lemonai.json workflow file):
 
 ### HackerNews
 
@@ -242,25 +244,44 @@
 - Get a review for a pull request: github-review-get
 - Get all reviews for a pull request: github-review-get-all
 - Update a review: github-review-update
 - Return the repositories of a user: github-user-repos
 - Invite a user to an organisation: github-user-org-invite
 - Return the repositories of an organisation: github-org-repos-get
 
+### Notion
+
+- Append block child: notion-append-after-block
+- Get block children: notion-get-child-blocks
+- Get database: notion-get-database
+- Get all databases: notion-get-many-database
+- Search database: notion-search-database
+- Create database page: notion-create-database-page
+- Get database page: notion-get-database-page
+- Get all database pages: notion-get-many-database-page
+- Update database page: notion-update-database-page
+- Archive page: notion-archive-page
+- Create page: notion-create-page
+- Search page: notion-search-page
+- Get user: notion-get-user
+- Get all users: notion-get-many-user
+
+
 ## ❤️‍🔥 Next Up
 
 - [x] Github
+- [x] Notion
+- [ ] Gmail
+- [ ] Google Calendar
 - [ ] Kafka
 - [ ] Pipedrive
 - [ ] Monday.com
 - [ ] Stripe
 - [ ] Medium
 - [ ] Discord
-- [ ] Gmail
-- [ ] Google Calendar
 - [ ] Google Cloud Realtime Database
 - [ ] Salesforce
-- [ ] Notion
+
 
 ## Contributing
 
 Do you have a connector you want to see included in Lemon AI or do you want to contribute in any other way? That's amazing 🥳 Just reach out, we are extremely open to contributions!
```

### Comparing `lemonai-0.0.7/pyproject.toml` & `lemonai-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lemonai"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Felix Brockmeier", email="fe.brockmeier@gmail.com" },
 ]
 description = "Lemon AI's A Python client. Grant your LLM agents access to a wide range of APIs for read and write operations, creating copilots in minutes and unlocking the true potential of LLMs."
 readme = "README.md"
 requires-python = ">=3.8.1"
 classifiers = [
```

### Comparing `lemonai-0.0.7/PKG-INFO` & `lemonai-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lemonai
-Version: 0.0.7
+Version: 0.0.8
 Summary: Lemon AI's A Python client. Grant your LLM agents access to a wide range of APIs for read and write operations, creating copilots in minutes and unlocking the true potential of LLMs.
 Project-URL: Homepage, https://github.com/felixbrock/lemonai-py-client
 Project-URL: Bug Tracker, https://github.com/felixbrock/lemonai-py-client/issues
 Author-email: Felix Brockmeier <fe.brockmeier@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -12,17 +12,19 @@
 Requires-Python: >=3.8.1
 Requires-Dist: langchain
 Requires-Dist: loguru
 Description-Content-Type: text/markdown
 
 # 🍋 Lemon AI
 
+![Heatmap Example](heatmap-example.gif)
+
 ## About
 
-**Build powerful AI assistants in minutes and execute highly efficient workflow automations by accessing tools like Airtable, Hubspot, Slack and Github.**
+**Build powerful AI assistants in minutes and execute highly efficient workflow automations by accessing tools like Airtable, Hubspot, Notion, Slack and Github.**
 
 Most connectors available today are focused on read-only operations, limiting the potential of LLMs. Agents, on the other hand, have a tendency to hallucinate from time to time due to missing context or instructions.
 
 With Lemon AI, it is possible to give your agents access to well-defined APIs for more reliable read and write operations. In addition, Lemon AI functions allow you to reduce the risk of hallucinations even more by providing a way to statically define workflows that the model can rely on in case of insecurity.
 
 ## 🖲️ Getting Started
 
@@ -131,17 +133,17 @@
 ```log
 2023-06-26T11:50:27.708785+0100 - b5f91c59-8487-45c2-800a-156eac0c7dae - HackerNews: Get User
 2023-06-26T11:50:39.624035+0100 - b5f91c59-8487-45c2-800a-156eac0c7dae - Airtable: Append the data to a table
 2023-06-26T11:58:32.925228+0100 - 5efe603c-9898-4143-b99a-55b50007ed9d - HackerNews: Get User
 2023-06-26T11:58:43.988788+0100 - 5efe603c-9898-4143-b99a-55b50007ed9d - Airtable: Append the data to a table
 ```
 
-By using the [Lemon AI Analytics Notebook](https://github.com/felixbrock/lemonai-analytics) you can easily gain a better understanding of how frequently and in which workflow combination tools are used. As a result you can identify weak spots in your agent’s decision making capabilities and move to a more deterministic behaviour by defining [Lemon AI functions](#lemon-ai-functions---solve-tasks-based-on-predefined-workflows):
+By using the [Lemon AI Analytics Tool](https://github.com/felixbrock/lemonai-analytics) you can easily gain a better understanding of how frequently and in which workflow combination tools are used. As a result you can identify weak spots in your agent’s decision making capabilities and move to a more deterministic behaviour by defining [Lemon AI functions](#lemon-ai-functions---solve-tasks-based-on-predefined-workflows):
 
-![Heatmap Example](heatmap-example.gif)
+![Heatmap Example](heatmap-example.png)
 
 ## Supported Tools
 
 Below is a list of all tools supported by Lemon AI and their ids (for use in the lemonai.json workflow file):
 
 ### HackerNews
 
@@ -258,25 +260,44 @@
 - Get a review for a pull request: github-review-get
 - Get all reviews for a pull request: github-review-get-all
 - Update a review: github-review-update
 - Return the repositories of a user: github-user-repos
 - Invite a user to an organisation: github-user-org-invite
 - Return the repositories of an organisation: github-org-repos-get
 
+### Notion
+
+- Append block child: notion-append-after-block
+- Get block children: notion-get-child-blocks
+- Get database: notion-get-database
+- Get all databases: notion-get-many-database
+- Search database: notion-search-database
+- Create database page: notion-create-database-page
+- Get database page: notion-get-database-page
+- Get all database pages: notion-get-many-database-page
+- Update database page: notion-update-database-page
+- Archive page: notion-archive-page
+- Create page: notion-create-page
+- Search page: notion-search-page
+- Get user: notion-get-user
+- Get all users: notion-get-many-user
+
+
 ## ❤️‍🔥 Next Up
 
 - [x] Github
+- [x] Notion
+- [ ] Gmail
+- [ ] Google Calendar
 - [ ] Kafka
 - [ ] Pipedrive
 - [ ] Monday.com
 - [ ] Stripe
 - [ ] Medium
 - [ ] Discord
-- [ ] Gmail
-- [ ] Google Calendar
 - [ ] Google Cloud Realtime Database
 - [ ] Salesforce
-- [ ] Notion
+
 
 ## Contributing
 
 Do you have a connector you want to see included in Lemon AI or do you want to contribute in any other way? That's amazing 🥳 Just reach out, we are extremely open to contributions!
```


# Comparing `tmp/remindmail-2023.6.8.1.tar.gz` & `tmp/remindmail-2023.7.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remindmail-2023.6.8.1.tar", last modified: Thu Jun  8 06:31:47 2023, max compression
+gzip compressed data, was "remindmail-2023.7.9.1.tar", last modified: Mon Jul 10 04:17:43 2023, max compression
```

## Comparing `remindmail-2023.6.8.1.tar` & `remindmail-2023.7.9.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-08 06:31:47.037063 remindmail-2023.6.8.1/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1070 2022-10-19 22:48:49.000000 remindmail-2023.6.8.1/LICENSE.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    13861 2023-06-08 06:31:47.037063 remindmail-2023.6.8.1/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    13512 2023-06-08 06:27:14.000000 remindmail-2023.6.8.1/README.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2022-10-19 22:48:49.000000 remindmail-2023.6.8.1/pyproject.toml
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      751 2023-06-08 06:31:47.037063 remindmail-2023.6.8.1/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-08 06:31:47.033063 remindmail-2023.6.8.1/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-08 06:31:47.037063 remindmail-2023.6.8.1/src/remind/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        0 2023-04-30 04:24:17.000000 remindmail-2023.6.8.1/src/remind/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     4611 2023-06-08 06:31:13.000000 remindmail-2023.6.8.1/src/remind/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2405 2023-04-30 04:24:17.000000 remindmail-2023.6.8.1/src/remind/reminder.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    25417 2023-06-05 04:59:42.000000 remindmail-2023.6.8.1/src/remind/remindmail.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    12809 2023-06-08 06:30:34.000000 remindmail-2023.6.8.1/src/remind/remindmail_utils.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-06-08 06:31:47.037063 remindmail-2023.6.8.1/src/remindmail.egg-info/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    13861 2023-06-08 06:31:47.000000 remindmail-2023.6.8.1/src/remindmail.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      363 2023-06-08 06:31:47.000000 remindmail-2023.6.8.1/src/remindmail.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-06-08 06:31:47.000000 remindmail-2023.6.8.1/src/remindmail.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2023-06-08 06:31:47.000000 remindmail-2023.6.8.1/src/remindmail.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2023-06-08 06:31:47.000000 remindmail-2023.6.8.1/src/remindmail.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-10 04:17:43.412616 remindmail-2023.7.9.1/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1070 2022-10-19 22:48:49.000000 remindmail-2023.7.9.1/LICENSE.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    15502 2023-07-10 04:17:43.412616 remindmail-2023.7.9.1/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    15153 2023-06-22 04:24:04.000000 remindmail-2023.7.9.1/README.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2022-10-19 22:48:49.000000 remindmail-2023.7.9.1/pyproject.toml
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      751 2023-07-10 04:17:43.412616 remindmail-2023.7.9.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-10 04:17:43.412616 remindmail-2023.7.9.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-10 04:17:43.412616 remindmail-2023.7.9.1/src/remind/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        0 2023-04-30 04:24:17.000000 remindmail-2023.7.9.1/src/remind/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     7621 2023-06-28 22:32:45.000000 remindmail-2023.7.9.1/src/remind/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2405 2023-04-30 04:24:17.000000 remindmail-2023.7.9.1/src/remind/reminder.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    26549 2023-07-10 04:16:58.000000 remindmail-2023.7.9.1/src/remind/remindmail.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    12881 2023-06-28 22:32:45.000000 remindmail-2023.7.9.1/src/remind/remindmail_utils.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     6501 2023-06-22 04:24:04.000000 remindmail-2023.7.9.1/src/remind/trello_manager.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-07-10 04:17:43.412616 remindmail-2023.7.9.1/src/remindmail.egg-info/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    15502 2023-07-10 04:17:43.000000 remindmail-2023.7.9.1/src/remindmail.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      392 2023-07-10 04:17:43.000000 remindmail-2023.7.9.1/src/remindmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-07-10 04:17:43.000000 remindmail-2023.7.9.1/src/remindmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2023-07-10 04:17:43.000000 remindmail-2023.7.9.1/src/remindmail.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2023-07-10 04:17:43.000000 remindmail-2023.7.9.1/src/remindmail.egg-info/top_level.txt
```

### Comparing `remindmail-2023.6.8.1/LICENSE.md` & `remindmail-2023.7.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `remindmail-2023.6.8.1/PKG-INFO` & `remindmail-2023.7.9.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: remindmail
-Version: 2023.6.8.1
-Summary: Easily schedule reminders to be emailed
-Home-page: https://github.com/tylerjwoodfin/remindmail
-Author: Tyler Woodfin
-Author-email: feedback@tyler.cloud
-License: : OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # remindmail
 
 - turns reminders written in terminal into emails; supports scheduled reminders
 
 ## features
 
 - easily manage your To Do list from anywhere in the terminal
@@ -89,14 +77,27 @@
 - `--show-tomorrow`: Lists reminders in remind.md that are marked with tomorrow's date in YYYY-MM-DD
 - `--sent-today`: Prints the number of reminders sent today (or yesterday, if before 4AM)
 - `--stats`: Prints usage statistics about RemindMail
 - `-o` (or `--offset`): Calculates the offset of a date (see [offset](##offset))
 - `-e` (or `--edit`): Opens `remind.md` in vim
 - `-j` (or `--jira`): Sends your reminder to a new Jira task for your desired board (see [Jira](#jira))
 
+## Trello
+- `-b` (or `--board`): An argument; the name of the Trello board to use
+- `--list-name`: An argument; the name of the Trello list to use
+- `-ti` (or `--trello-items`): Prints items within a Trello list (accepts `-b` or `--board`, `--list-name`)
+  - If a board is not specified, the user is prompted to choose one
+  - If a list is not specified, the user is prompted to choose one
+- `-tl` (or `--trello-list`): Prints the lists within a Trello board (accepts `-b` or `--board`, `--list-name`)
+  - If a board is not specified, the user is prompted to choose one
+- `-ta` (or `--trello-add`): Adds an item to a Trello list (accepts `-b` or `--board`, `--list-name`, `--item-name`)
+  - If a board is not specified, the user is prompted to choose one
+  - If a list is not specified, the user is prompted to choose one
+  - If an item is not specified, the user is prompted to enter one
+
 ## list (-l, -ls, or --list)
 - lists all current reminders in `remind.md`
 
 ## generate (-g or --generate)
 - generates reminders from `remind.md` that match the condition in brackets, 
 such as `[wed]` matching if today is Wednesday
 
@@ -332,7 +333,37 @@
 remind --jira "this is a story 4" -t task --desc "Testing description" --label "testing"
 
 # select '(j)' in confirmation menu
 remind -m this is a new jira ticket
 ```
 
 After the issue has been created, a success message and link to the new issue will appear.
+
+## Trello Integration
+
+## configuration
+
+Before using the Trello integration, [obtain a Trello API Key](https://developer.atlassian.com/cloud/trello/guides/rest-api/authorization/).
+
+Using [Cabinet](https://pypi.org/project/cabinet/), set the API key by running:
+
+```
+cabinet --put keys trello <api key here>
+```
+
+Upon first running a Trello-related command, you will be prompted to authorize your application in the browser.
+
+## usage
+
+```
+# prints all lists in the `Shopping` board
+remind -tl Shopping
+
+# prints all items from a list (interactive)
+remind -ti
+
+# prints all items from the `Tyler` list in the `Shopping` board
+remind -ti --board Shopping --list-name Tyler
+
+# select '(j)' in confirmation menu
+remind -m this is a new jira ticket
+```
```

### Comparing `remindmail-2023.6.8.1/README.md` & `remindmail-2023.7.9.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: remindmail
+Version: 2023.7.9.1
+Summary: Easily schedule reminders to be emailed
+Home-page: https://github.com/tylerjwoodfin/remindmail
+Author: Tyler Woodfin
+Author-email: feedback@tyler.cloud
+License: : OSI Approved :: MIT License
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # remindmail
 
 - turns reminders written in terminal into emails; supports scheduled reminders
 
 ## features
 
 - easily manage your To Do list from anywhere in the terminal
@@ -77,14 +89,27 @@
 - `--show-tomorrow`: Lists reminders in remind.md that are marked with tomorrow's date in YYYY-MM-DD
 - `--sent-today`: Prints the number of reminders sent today (or yesterday, if before 4AM)
 - `--stats`: Prints usage statistics about RemindMail
 - `-o` (or `--offset`): Calculates the offset of a date (see [offset](##offset))
 - `-e` (or `--edit`): Opens `remind.md` in vim
 - `-j` (or `--jira`): Sends your reminder to a new Jira task for your desired board (see [Jira](#jira))
 
+## Trello
+- `-b` (or `--board`): An argument; the name of the Trello board to use
+- `--list-name`: An argument; the name of the Trello list to use
+- `-ti` (or `--trello-items`): Prints items within a Trello list (accepts `-b` or `--board`, `--list-name`)
+  - If a board is not specified, the user is prompted to choose one
+  - If a list is not specified, the user is prompted to choose one
+- `-tl` (or `--trello-list`): Prints the lists within a Trello board (accepts `-b` or `--board`, `--list-name`)
+  - If a board is not specified, the user is prompted to choose one
+- `-ta` (or `--trello-add`): Adds an item to a Trello list (accepts `-b` or `--board`, `--list-name`, `--item-name`)
+  - If a board is not specified, the user is prompted to choose one
+  - If a list is not specified, the user is prompted to choose one
+  - If an item is not specified, the user is prompted to enter one
+
 ## list (-l, -ls, or --list)
 - lists all current reminders in `remind.md`
 
 ## generate (-g or --generate)
 - generates reminders from `remind.md` that match the condition in brackets, 
 such as `[wed]` matching if today is Wednesday
 
@@ -319,8 +344,38 @@
 # creates a ticket without prompts
 remind --jira "this is a story 4" -t task --desc "Testing description" --label "testing"
 
 # select '(j)' in confirmation menu
 remind -m this is a new jira ticket
 ```
 
-After the issue has been created, a success message and link to the new issue will appear.
+After the issue has been created, a success message and link to the new issue will appear.
+
+## Trello Integration
+
+## configuration
+
+Before using the Trello integration, [obtain a Trello API Key](https://developer.atlassian.com/cloud/trello/guides/rest-api/authorization/).
+
+Using [Cabinet](https://pypi.org/project/cabinet/), set the API key by running:
+
+```
+cabinet --put keys trello <api key here>
+```
+
+Upon first running a Trello-related command, you will be prompted to authorize your application in the browser.
+
+## usage
+
+```
+# prints all lists in the `Shopping` board
+remind -tl Shopping
+
+# prints all items from a list (interactive)
+remind -ti
+
+# prints all items from the `Tyler` list in the `Shopping` board
+remind -ti --board Shopping --list-name Tyler
+
+# select '(j)' in confirmation menu
+remind -m this is a new jira ticket
+```
```

### Comparing `remindmail-2023.6.8.1/setup.cfg` & `remindmail-2023.7.9.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [metadata]
 name = remindmail
-version = 2023.06.08.1
+version = 2023.07.09.1
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily schedule reminders to be emailed
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/remindmail
 project_urls = 
-Bug Tracker = https://github.com/tylerjwoodfin/remindmail/issues
+bug tracker = https://github.com/tylerjwoodfin/remindmail/issues
 py_modules = ["remind"]
 classifiers = 
-Programming Language = : Python :: 3
-License = : OSI Approved :: MIT License
-Operating System = : OS Independent
+programming language = : Python :: 3
+license = : OSI Approved :: MIT License
+operating system = : OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
```

### Comparing `remindmail-2023.6.8.1/src/remind/reminder.py` & `remindmail-2023.7.9.1/src/remind/reminder.py`

 * *Files identical despite different names*

### Comparing `remindmail-2023.6.8.1/src/remind/remindmail.py` & `remindmail-2023.7.9.1/src/remind/remindmail.py`

 * *Files 5% similar despite different names*

```diff
@@ -270,14 +270,22 @@
             noconfirm (bool, optional): If True, bypass the confirmation screen.
         """
 
         today = str(datetime.today().strftime('%Y-%m-%d'))
         weekdays = ['sunday', 'monday', 'tuesday',
                     'wednesday', 'thursday', 'friday', 'saturday']
 
+        def extract_url(string):
+            """
+            Returns any URLs from a string
+            """
+            pattern = r'(https?://\S+)'
+            urls = re.findall(pattern, string)
+            return urls
+
         # helper functions
         def get_larger(string_a: str, string_b: str):
             """A helper function to return the larger string between string_a and string_b"""
 
             return string_a if len(string_a) > len(string_b) else string_b
 
         def strip_to(query):
@@ -302,18 +310,30 @@
 
             Notes:
                 - The function supports parsing various date formats.
                 - If the query contains the word 'tomorrow', it returns the date for the next day.
                 - If a date is parsed into before 90 days ago, it is returns a date for next year.
             """
 
+            # if before 4AM, a request for a reminder 'tomorrow' will
+            # appear as a request for today
+            is_after_4am = datetime.now().hour > 4
+
             # handle 'tomorrow'
             if 'tomorrow' in query:
-                _days = 0 if datetime.now().hour < 3 else 1
-                query = (datetime.now() + timedelta(days=_days)).strftime('%F')
+                query = (datetime.now() +
+                         timedelta(days=int(is_after_4am))).strftime('%F')
+
+            # handle current day
+            current_day = datetime.now().strftime('%A')
+            if is_after_4am and current_day.lower() in query.lower():
+                query_date = (datetime.now() +
+                              timedelta(days=7)).strftime('%F')
+                query = re.sub(r'\b' + re.escape(current_day) + r'\b',
+                               query_date, query, flags=re.IGNORECASE)
 
             try:
                 parsed_date = parse(query, fuzzy_with_tokens=True)
 
                 # handle dates in the past
                 days_from_now = (parsed_date[0] - datetime.today()).days
                 if days_from_now < -90:
@@ -342,17 +362,24 @@
             RemindMailUtils().send_email(f"Bad Query: {today}", '<br>'.join(
                 RemindMailUtils.query_trace).replace("\n", "<br>"), False, is_quiet=False)
 
         if manual_date == 'now':
             manual_date = today
 
         # parse for notes
-        if ':' in query:
-            query_notes = ''.join(query.split(":")[1:])
-            query = query.split(":")[0]
+        query_remove_urls = query.replace("http://", "").replace("https://", "")
+        if ':' in query_remove_urls:
+            query_notes = ''.join(query_remove_urls.split(":")[1:])
+            query = query_remove_urls.split(":")[0]
+
+        # parse for URLs
+        urls = extract_url(query)
+        if len(urls) > 0:
+            link_tags = ' '.join([f'<a href="{url}">{url}</a>' for url in urls])
+            query_notes += f"<br>Your link: {link_tags}"
 
         # remove filler text
         for item in ['me to ', 'to ', 'me ']:
             if item in query.lower() and len(query.split(item)[0]) < 3:
                 query = re.sub(item, '', query, flags=re.IGNORECASE, count=1)
 
         # handle recurring reminders
@@ -443,15 +470,15 @@
             for day in day_prefixes:
                 if re.search(day, query, flags=re.IGNORECASE):
 
                     _query_match = re.split(day, query, flags=re.IGNORECASE)
                     query = get_larger(_query_match[0], _query_match[1])
 
                     query_time_token = re.sub(
-                        'on|next|day', '', day, flags=re.IGNORECASE).strip()
+                        'on|next|day', '', day, flags=re.IGNORECASE, count=1).strip()
 
                     query_time_formatted = {
                         'sun': 'Sunday',
                         'mon': 'Monday',
                         'tues': 'Tuesday',
                         'wednes': 'Wednesday',
                         'thurs': 'Thursday',
@@ -567,15 +594,15 @@
             elif response == 'j':
                 print("Creating Jira issue...")
                 RemindMailUtils().create_jira_issue(summary=query, description=query_notes or '')
                 return
 
         # send immediate reminders
         if query_time_formatted == 'right now' and response == 'y':
-            RemindMailUtils().send_email(query.strip(), query_notes, False, is_quiet=True)
+            RemindMailUtils().send_email(query.strip(), query_notes, 'RemindMail', is_quiet=True)
             return
 
         # scheduled reminders
         if query_time_token:
             if len(response) > 0 and not response.startswith('n'):
                 if response == 'r':
                     report_query()
@@ -603,15 +630,15 @@
                 # send 'right now' reminder
                 RemindMailUtils().send_email(query.strip(), query_notes, is_quiet=True)
 
     def manual_reminder(self, manual_message='', manual_date='', noconfirm=False):
         """
         Creates a reminder with a message and a date.
         If manual_message and/or manual_date are not provided,
-            prompts the user to input them. 
+            prompts the user to input them.
 
         Args:
             manual_message (str): Optional. The reminder message.
             manual_date (str): Optional. The reminder date in a string format.
 
         Returns:
             None
```

### Comparing `remindmail-2023.6.8.1/src/remind/remindmail_utils.py` & `remindmail-2023.7.9.1/src/remind/remindmail_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,15 +244,15 @@
 
         body += f"<br><br>Sent via {method}"
 
         RemindMailUtils.mail.send(
             f"Reminder - {subject}", body or "", is_quiet=is_quiet)
         print("\nSent! Check your inbox.")
 
-    def create_jira_issue(self, summary, description, issue_type: str = None, label=None):
+    def create_jira_issue(self, summary, description, issue_type: str = None, label: str = None):
         """
         A barebones integration with Jira.
 
         Requires Cabinet to be configured as described in README.
 
         Parameters:
             summary(str): issue title
@@ -277,19 +277,14 @@
 
         if not jira_api_token or not jira_email:
             self.cab.log("RemindMail - cannot create Jira issue; cabinet is missing "
                          "`keys -> jira` or `jira -> email` (see README)",
                          level="warn")
             return
 
-        if not summary:
-            self.cab.log("RemindMail - cannot create Jira issue; summary cannot be blank",
-                         level="warn")
-            return
-
         # Create the authentication header
         credentials = f'{jira_email}:{jira_api_token}'
         encoded_credentials = base64.b64encode(
             credentials.encode('utf-8')).decode('utf-8')
         headers = {
             'Content-Type': 'application/json',
             'Authorization': f'Basic {encoded_credentials}'
@@ -302,18 +297,23 @@
                 'summary': f"RMMJ: {summary}",
                 'issuetype': {'name': issue_type.capitalize() if issue_type else ''},
                 'labels': [label] if label else None,
             }
         }
 
         # Prompt for missing fields
-        if not issue_type:
-            issue_type_input = input('Please enter an issue type:\n'
-                                     'story\nbug\ntask\nspike\nepic\n\n').capitalize()
-            payload['fields']['issuetype']['name'] = issue_type_input
+        if not summary:
+            summary = input("Enter the summary for your Jira ticket:\n")
+
+        valid_issue_types = ['Story', 'Bug', 'Task', 'Spike', 'Epic']
+        valid_issue_types_str = '\n'.join(valid_issue_types)
+        while issue_type not in valid_issue_types:
+            issue_type = input(f'\nPlease enter an issue type:\n'
+                                     f'{valid_issue_types_str}\n\n').capitalize()
+            payload['fields']['issuetype']['name'] = issue_type
 
         if description is None:
             description_input = input(
                 '\nPlease enter a description (or Enter for none)\n')
             payload['fields']['description'] = description_input
         else:
             payload['fields']['description'] = description
```

### Comparing `remindmail-2023.6.8.1/src/remindmail.egg-info/PKG-INFO` & `remindmail-2023.7.9.1/src/remindmail.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remindmail
-Version: 2023.6.8.1
+Version: 2023.7.9.1
 Summary: Easily schedule reminders to be emailed
 Home-page: https://github.com/tylerjwoodfin/remindmail
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -89,14 +89,27 @@
 - `--show-tomorrow`: Lists reminders in remind.md that are marked with tomorrow's date in YYYY-MM-DD
 - `--sent-today`: Prints the number of reminders sent today (or yesterday, if before 4AM)
 - `--stats`: Prints usage statistics about RemindMail
 - `-o` (or `--offset`): Calculates the offset of a date (see [offset](##offset))
 - `-e` (or `--edit`): Opens `remind.md` in vim
 - `-j` (or `--jira`): Sends your reminder to a new Jira task for your desired board (see [Jira](#jira))
 
+## Trello
+- `-b` (or `--board`): An argument; the name of the Trello board to use
+- `--list-name`: An argument; the name of the Trello list to use
+- `-ti` (or `--trello-items`): Prints items within a Trello list (accepts `-b` or `--board`, `--list-name`)
+  - If a board is not specified, the user is prompted to choose one
+  - If a list is not specified, the user is prompted to choose one
+- `-tl` (or `--trello-list`): Prints the lists within a Trello board (accepts `-b` or `--board`, `--list-name`)
+  - If a board is not specified, the user is prompted to choose one
+- `-ta` (or `--trello-add`): Adds an item to a Trello list (accepts `-b` or `--board`, `--list-name`, `--item-name`)
+  - If a board is not specified, the user is prompted to choose one
+  - If a list is not specified, the user is prompted to choose one
+  - If an item is not specified, the user is prompted to enter one
+
 ## list (-l, -ls, or --list)
 - lists all current reminders in `remind.md`
 
 ## generate (-g or --generate)
 - generates reminders from `remind.md` that match the condition in brackets, 
 such as `[wed]` matching if today is Wednesday
 
@@ -332,7 +345,37 @@
 remind --jira "this is a story 4" -t task --desc "Testing description" --label "testing"
 
 # select '(j)' in confirmation menu
 remind -m this is a new jira ticket
 ```
 
 After the issue has been created, a success message and link to the new issue will appear.
+
+## Trello Integration
+
+## configuration
+
+Before using the Trello integration, [obtain a Trello API Key](https://developer.atlassian.com/cloud/trello/guides/rest-api/authorization/).
+
+Using [Cabinet](https://pypi.org/project/cabinet/), set the API key by running:
+
+```
+cabinet --put keys trello <api key here>
+```
+
+Upon first running a Trello-related command, you will be prompted to authorize your application in the browser.
+
+## usage
+
+```
+# prints all lists in the `Shopping` board
+remind -tl Shopping
+
+# prints all items from a list (interactive)
+remind -ti
+
+# prints all items from the `Tyler` list in the `Shopping` board
+remind -ti --board Shopping --list-name Tyler
+
+# select '(j)' in confirmation menu
+remind -m this is a new jira ticket
+```
```


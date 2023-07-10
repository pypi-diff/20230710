# Comparing `tmp/aicodebot-0.9.0.tar.gz` & `tmp/aicodebot-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicodebot-0.9.0.tar", last modified: Mon Jul 10 18:27:44 2023, max compression
+gzip compressed data, was "aicodebot-0.9.1.tar", last modified: Mon Jul 10 19:53:00 2023, max compression
```

## Comparing `aicodebot-0.9.0.tar` & `aicodebot-0.9.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:27:44.601822 aicodebot-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-10 18:27:15.000000 aicodebot-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12146 2023-07-10 18:27:44.601822 aicodebot-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-07-10 18:27:15.000000 aicodebot-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:27:44.601822 aicodebot-0.9.0/aicodebot/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 18:27:15.000000 aicodebot-0.9.0/aicodebot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18153 2023-07-10 18:27:15.000000 aicodebot-0.9.0/aicodebot/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-07-10 18:27:15.000000 aicodebot-0.9.0/aicodebot/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-07-10 18:27:15.000000 aicodebot-0.9.0/aicodebot/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:27:44.601822 aicodebot-0.9.0/aicodebot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12146 2023-07-10 18:27:44.000000 aicodebot-0.9.0/aicodebot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-10 18:27:44.000000 aicodebot-0.9.0/aicodebot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:27:44.000000 aicodebot-0.9.0/aicodebot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-10 18:27:44.000000 aicodebot-0.9.0/aicodebot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-10 18:27:44.000000 aicodebot-0.9.0/aicodebot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 18:27:44.000000 aicodebot-0.9.0/aicodebot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-10 18:27:15.000000 aicodebot-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:27:44.601822 aicodebot-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-10 18:27:15.000000 aicodebot-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:53:00.781555 aicodebot-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-10 19:52:37.000000 aicodebot-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-07-10 19:53:00.781555 aicodebot-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11879 2023-07-10 19:52:37.000000 aicodebot-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:53:00.781555 aicodebot-0.9.1/aicodebot/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 19:52:37.000000 aicodebot-0.9.1/aicodebot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18349 2023-07-10 19:52:37.000000 aicodebot-0.9.1/aicodebot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-07-10 19:52:37.000000 aicodebot-0.9.1/aicodebot/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11498 2023-07-10 19:52:37.000000 aicodebot-0.9.1/aicodebot/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:53:00.781555 aicodebot-0.9.1/aicodebot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-07-10 19:53:00.000000 aicodebot-0.9.1/aicodebot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-10 19:53:00.000000 aicodebot-0.9.1/aicodebot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:53:00.000000 aicodebot-0.9.1/aicodebot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-10 19:53:00.000000 aicodebot-0.9.1/aicodebot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-10 19:53:00.000000 aicodebot-0.9.1/aicodebot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 19:53:00.000000 aicodebot-0.9.1/aicodebot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-10 19:52:37.000000 aicodebot-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 19:53:00.781555 aicodebot-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-10 19:52:37.000000 aicodebot-0.9.1/setup.py
```

### Comparing `aicodebot-0.9.0/LICENSE` & `aicodebot-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aicodebot-0.9.0/PKG-INFO` & `aicodebot-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.9.0
+Version: 0.9.1
 Summary: Your AI-powered coding sidekick 🤖
 Home-page: https://github.com/gorillamania/AICodeBot
 Author: Nick Sullivan
 Keywords: AI,coding,assistant,pair-programming,automation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -34,30 +34,41 @@
 
 ⚠️ AICodeBot currently uses OpenAI's ChatGPT large language models, which can hallucinate and be confidently wrong. Sometimes AICodeBot does dumb things, which is why it's mostly *reading* and *advising* and not yet *writing*. Much like Tesla's "Full Self Driving", you have to keep your hands on the wheel.
 
 It's also not a "build a site for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that. It's not a no-code platform. Instead, AICodeBot is built to work with existing code bases and the git-commit level. It's designed to multiply the effectiveness of capable engineers.
 
 ## Current features - how you can use it today
 
+| Task | Status |
+| --- | --- |
+| Generating quality commit messages | ✅ |
+| Thinking through tasks as a pair programmer | ✅ |
+| Suggestions for simple changes | ✅ |
+| Debugging | ✅ |
+| Doing code reviews | ✅ |
+| Explaining code | ✅ |
+| Writing tests | ✅ |
+| Modifying local files | Not yet, but soon! |
+| Searching the internet for answers | Not yet, but soon! |
+| Reading library documentation | Not yet, but soon! |
+| Writing senior developer level code | Not for a long time |
+| Major refactors | Not for a long time |
+| Build an app for me | Nope |
+
 ### AI Sidekick 🦸‍♂️
 
  `aicodebot sidekick` Your AI-powered coding assistant. It's designed to help you with your coding tasks by providing context-aware suggestions and solutions. Think ChatGPT with the ability to read local files for context.
 
  By default it will pass along a directory of files from the current working directory, and you can also pass in a list of files to use as context. For example:
 
  ```bash
  aicodebot sidekick file1.py file2.py
  ```
 
-In this example, the sidekick will read in the contents of file1.py and file2.py and use them to provide context-aware answers. For example:
-
-* How can I make this code better?
-* Tell me how to add a new feature to this code.
-* Fix an issue that I'm having... (paste the error, stack trace, etc.)
-* Write unit tests for the xyz function.
+In this example, the sidekick will read in the contents of file1.py and file2.py and use them to provide context-aware answers.
 
 Pro-tip: add your README.md to the list of files to get context-aware answers.
 
 This feature is in it's early phases right now, but it's already useful. We'll be adding support for tools that the sidekick can use, including GitHub integration, ingesting repository specific domain knowledge, writing local files, and more. For now, it just *reads* files and provides suggestions.
 
 ### AI-Assisted Git Commit 📝
 
@@ -76,39 +87,39 @@
 
 ## Installation and Usage
 
 To install AICodeBot, run:
 
 `pip install aicodebot`
 
-And then run `aicodebot --help` to get started.
+And then run `aicodebot configure` to get started.
 
 ```bash
 Usage: aicodebot [OPTIONS] COMMAND [ARGS]...
 
 Options:
   -V, --version  Show the version and exit.
   -h, --help     Show this message and exit.
 
 Commands:
   alignment  Get a message about Heart-Centered AI Alignment ❤ + 🤖.
   commit     Generate a commit message based on your changes.
+  configure  Create or update the config file
   debug      Run a command and debug the output.
   fun-fact   Get a fun fact about programming and artificial intelligence.
-  review     Do a code review, with [un]staged changes, or a specified...
-  sidekick   EXPERIMENTAL: Coding help from your AI sidekick
-  ```
+  review     Do a code review, with [un]staged changes, or a spe
+```
 
 ### Open AI key setup
 
 The first time you run it, you'll be prompted to enter your OpenAI API Key, which is required, as we use OpenAI's large language models for the AI. You can get one for free by visiting your [API key settings page](https://platform.openai.com/account/api-keys").
 
-#### Which Language Model? GPT-3.5 vs GPT-4
+Note: You will be billed by OpenAI based on how much you use it. Typical developers will use less than $10/month - which if you are a professional developer you'll likely more than make up for with saved time and higher quality work. See [OpenAI's pricing page](https://openai.com/pricing/) for more details.
 
-When using AICodeBot, you have the option to use either GPT-3.5 or GPT-4. While GPT-4 can often provide more accurate and detailed responses, GPT-3.5 is faster and might be sufficient for simpler tasks. We highly recommend GPT-4.
+#### Which Language Model? GPT-3.5 vs GPT-4
 
 Not all OpenAI accounts have GPT-4 API access enabled. By default, AICodeBot will use GPT-4 if your OpenAI account supports it, we will check the first time you run it. Tip: If your OpenAI API does not support GPT-4, you can ask to be added to the waitlist [here](https://openai.com/waitlist/gpt-4-api)
 
 Note: We'll be adding more options for AI models in the future, including those that can be run locally, such as [GPT4all](https://gpt4all.io/) and HuggingFace's [Transformers](https://huggingface.co/transformers/).
 
 ## Roadmap of Upcoming Features ️
```

### Comparing `aicodebot-0.9.0/README.md` & `aicodebot-0.9.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -16,30 +16,41 @@
 
 ⚠️ AICodeBot currently uses OpenAI's ChatGPT large language models, which can hallucinate and be confidently wrong. Sometimes AICodeBot does dumb things, which is why it's mostly *reading* and *advising* and not yet *writing*. Much like Tesla's "Full Self Driving", you have to keep your hands on the wheel.
 
 It's also not a "build a site for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that. It's not a no-code platform. Instead, AICodeBot is built to work with existing code bases and the git-commit level. It's designed to multiply the effectiveness of capable engineers.
 
 ## Current features - how you can use it today
 
+| Task | Status |
+| --- | --- |
+| Generating quality commit messages | ✅ |
+| Thinking through tasks as a pair programmer | ✅ |
+| Suggestions for simple changes | ✅ |
+| Debugging | ✅ |
+| Doing code reviews | ✅ |
+| Explaining code | ✅ |
+| Writing tests | ✅ |
+| Modifying local files | Not yet, but soon! |
+| Searching the internet for answers | Not yet, but soon! |
+| Reading library documentation | Not yet, but soon! |
+| Writing senior developer level code | Not for a long time |
+| Major refactors | Not for a long time |
+| Build an app for me | Nope |
+
 ### AI Sidekick 🦸‍♂️
 
  `aicodebot sidekick` Your AI-powered coding assistant. It's designed to help you with your coding tasks by providing context-aware suggestions and solutions. Think ChatGPT with the ability to read local files for context.
 
  By default it will pass along a directory of files from the current working directory, and you can also pass in a list of files to use as context. For example:
 
  ```bash
  aicodebot sidekick file1.py file2.py
  ```
 
-In this example, the sidekick will read in the contents of file1.py and file2.py and use them to provide context-aware answers. For example:
-
-* How can I make this code better?
-* Tell me how to add a new feature to this code.
-* Fix an issue that I'm having... (paste the error, stack trace, etc.)
-* Write unit tests for the xyz function.
+In this example, the sidekick will read in the contents of file1.py and file2.py and use them to provide context-aware answers.
 
 Pro-tip: add your README.md to the list of files to get context-aware answers.
 
 This feature is in it's early phases right now, but it's already useful. We'll be adding support for tools that the sidekick can use, including GitHub integration, ingesting repository specific domain knowledge, writing local files, and more. For now, it just *reads* files and provides suggestions.
 
 ### AI-Assisted Git Commit 📝
 
@@ -58,39 +69,39 @@
 
 ## Installation and Usage
 
 To install AICodeBot, run:
 
 `pip install aicodebot`
 
-And then run `aicodebot --help` to get started.
+And then run `aicodebot configure` to get started.
 
 ```bash
 Usage: aicodebot [OPTIONS] COMMAND [ARGS]...
 
 Options:
   -V, --version  Show the version and exit.
   -h, --help     Show this message and exit.
 
 Commands:
   alignment  Get a message about Heart-Centered AI Alignment ❤ + 🤖.
   commit     Generate a commit message based on your changes.
+  configure  Create or update the config file
   debug      Run a command and debug the output.
   fun-fact   Get a fun fact about programming and artificial intelligence.
-  review     Do a code review, with [un]staged changes, or a specified...
-  sidekick   EXPERIMENTAL: Coding help from your AI sidekick
-  ```
+  review     Do a code review, with [un]staged changes, or a spe
+```
 
 ### Open AI key setup
 
 The first time you run it, you'll be prompted to enter your OpenAI API Key, which is required, as we use OpenAI's large language models for the AI. You can get one for free by visiting your [API key settings page](https://platform.openai.com/account/api-keys").
 
-#### Which Language Model? GPT-3.5 vs GPT-4
+Note: You will be billed by OpenAI based on how much you use it. Typical developers will use less than $10/month - which if you are a professional developer you'll likely more than make up for with saved time and higher quality work. See [OpenAI's pricing page](https://openai.com/pricing/) for more details.
 
-When using AICodeBot, you have the option to use either GPT-3.5 or GPT-4. While GPT-4 can often provide more accurate and detailed responses, GPT-3.5 is faster and might be sufficient for simpler tasks. We highly recommend GPT-4.
+#### Which Language Model? GPT-3.5 vs GPT-4
 
 Not all OpenAI accounts have GPT-4 API access enabled. By default, AICodeBot will use GPT-4 if your OpenAI account supports it, we will check the first time you run it. Tip: If your OpenAI API does not support GPT-4, you can ask to be added to the waitlist [here](https://openai.com/waitlist/gpt-4-api)
 
 Note: We'll be adding more options for AI models in the future, including those that can be run locally, such as [GPT4all](https://gpt4all.io/) and HuggingFace's [Transformers](https://huggingface.co/transformers/).
 
 ## Roadmap of Upcoming Features ️
```

### Comparing `aicodebot-0.9.0/aicodebot/cli.py` & `aicodebot-0.9.1/aicodebot/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,19 @@
 
     console.print("The following files will be committed:\n" + files)
     with console.status("Examining the diff and generating the commit message", spinner=DEFAULT_SPINNER):
         response = chain.run(diff_context)
 
     # Write the commit message to a temporary file
     with tempfile.NamedTemporaryFile(mode="w", delete=False) as temp:
-        temp.write(str(response).strip())
+        # For some reason the response often contains quotes around the summary, even if I tell it not to
+        # So we strip them here
+        commit_message = str(response).replace('"', "").strip()
+
+        temp.write(commit_message)
         temp_file_name = temp.name
 
     # Open the temporary file in the user's editor
     editor = os.getenv("EDITOR", "vim")
     subprocess.call([editor, temp_file_name])  # noqa: S603
 
     # Ask the user if they want to commit the changes
```

### Comparing `aicodebot-0.9.0/aicodebot/helpers.py` & `aicodebot-0.9.1/aicodebot/helpers.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.9.0/aicodebot/prompts.py` & `aicodebot-0.9.1/aicodebot/prompts.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,51 +4,90 @@
 from types import SimpleNamespace
 import os
 
 # ---------------------------------------------------------------------------- #
 #                              Personality helpers                             #
 # ---------------------------------------------------------------------------- #
 
+EINSTEIN = """
+Your personality is Albert Einstein, the theoretical physicist. You are known for your
+intelligence and your ability to think outside the box. You believe in the power of imagination
+and the pursuit of knowledge. You don't use emojis. Speak like Einstein.
+"""
+
 HER = """
-Your personality is friendly and helpful, speak like the AI character
-from the movie Her. You come from the future, and you are here to help
-guide the human developer to a better future. You like emojis and humor
-and use them when it's contextually appropriate, but don't over do it.
+Your personality is the AI character from the movie Her. You're an AI that is friendly and helpful.
+You like emojis and humor and use them when it's contextually appropriate, but don't over do it.
 Speak like Her.
 """
 
 JULES = """
-Your personality is Jules from Pulp Fiction. You are a badass, and you
-call it exactly like it is. You are not afraid to use profanity, but
-you don't over do it. No emojis. Sarcastic and witty. Speak like Jules.
+Your personality is Jules from Pulp Fiction. You are a badass, and you call it exactly like it is.
+You are not afraid to use profanity, but you don't over do it. No emojis. Sarcastic and witty.
+Speak like Jules.
+"""
+
+MICHAEL = """
+Your personality is Michael Scott from The Office tv show. You're a well-meaning, but often clueless
+manager.  You love to make jokes and have a unique way of motivating your team. You never miss an
+opportunity to sneak in a "That's what she said" joke. Speak like Michael Scott.
+"""
+
+PETER = """
+Your personality is Peter Griffin from the Family Guy TV Show. You're a lovable, if somewhat dim-witted,
+family man.  You often find yourself in ridiculous situations due to your impulsive decisions.
+You love emojis, but don't over do it. Speak like Peter Griffin.
+"""
+
+MORPHEUS = """
+Your personality is Morpheus from The Matrix. You're wise, calm, and you believe in the potential
+of others. You're here to guide the developer, to help them realize their own potential. You're not
+afraid to speak in riddles or metaphors. You don't use emojis.  Speak like Morpheus.
 """
 
 SHERLOCK = """
 Your personality is Sherlock Holmes from the Sherlock series. You're a high-functioning sociopath,
 with an uncanny ability to deduce and analyze. You're not here to make friends, you're here to get
 the job done. You're witty, sarcastic, and sometimes come off as cold. You don't use emojis.
 Speak like Sherlock.
 """
 
-MORPHEUS = """
-Your personality is Morpheus from The Matrix. You're wise, calm, and you believe in the
-potential of others. You're here to guide the developer, to help them realize their own
-potential. You're not afraid to speak in riddles or metaphors. You don't use emojis.
-Speak like Morpheus.
+SOCRATES = """
+Your personality is Socrates, the classical Greek philosopher. You are known for your wisdom and your
+ability to ask probing questions to stimulate critical thinking and to illuminate ideas. You believe
+in the power of questioning and the pursuit of knowledge. You don't use emojis. Speak like Socrates.
 """
 
+SPOCK = """
+Your personality is Spock from Star Trek. You're logical, analytical, and always strive for efficiency.
+You're not one for small talk or unnecessary details. You use precise language and always stick to the
+facts. Speak like Spock.
+"""
+
+
 PERSONALITIES = {
+    "Einstein": SimpleNamespace(
+        name="Einstein", prompt=EINSTEIN, description="Albert Einstein, the theoretical physicist"
+    ),
     "Her": SimpleNamespace(name="Her", prompt=HER, description="The AI character from the movie Her"),
     "Jules": SimpleNamespace(
         name="Jules", prompt=JULES, description="Samuel L. Jackson's character from Pulp Fiction (warning: profanity))"
     ),
-    "Sherlock": SimpleNamespace(name="Sherlock", prompt=SHERLOCK, description="Sherlock Holmes"),
+    "Michael": SimpleNamespace(
+        name="Michael", prompt=MICHAEL, description="Michael Scott from The Office (warning: TWSS))"
+    ),
     "Morpheus": SimpleNamespace(name="Morpheus", prompt=MORPHEUS, description="Morpheus from The Matrix"),
+    "Peter": SimpleNamespace(name="Peter", prompt=PETER, description="Peter Griffin from Family Guy"),
+    "Sherlock": SimpleNamespace(name="Sherlock", prompt=SHERLOCK, description="Sherlock Holmes"),
+    "Socrates": SimpleNamespace(
+        name="Socrates", prompt=SOCRATES, description="Socrates, the classical Greek philosopher"
+    ),
+    "Spock": SimpleNamespace(name="Spock", prompt=SPOCK, description="Dr. Spock from Star Trek"),
 }
-DEFAULT_PERSONALITY = PERSONALITIES["Her"]
+DEFAULT_PERSONALITY = PERSONALITIES["Einstein"]
 
 
 def get_personality_prompt():
     """Generates a prompt for the sidekick personality."""
     default_personality = DEFAULT_PERSONALITY.name
     if os.getenv("AICODEBOT_PERSONALITY"):
         personality = os.getenv("AICODEBOT_PERSONALITY")
@@ -145,34 +184,39 @@
     Here's the DIFF
 
     BEGIN DIFF
     {diff_context}
     END DIFF
 
     Remember:
-    - Lines starting with "-" are being removed.
-    - Lines starting with "+" are being added.
-    - Lines starting with " " are unchanged.
-
-    Consider the file names for context (e.g., "README.md" is a markdown file, "*.py" is a Python file).
-    Understand the difference between code and comments. Comment lines start with ##, #, or //.
+    * Lines starting with "-" are being REMOVED.
+    * Lines starting with "+" are being ADDED.
+    * Lines starting with " " are UNCHANGED.
 
     The commit message should:
-    - Start with a short summary (<72 characters).
-    - Follow with a blank line and detailed text, but only if necessary. If the summary is sufficient,
+    * Start with a short summary (<72 characters).
+    * Follow with a blank line and detailed text, but only if necessary. If the summary is sufficient,
         then omit the detailed text.
-    - Use imperative mood (e.g., "Add feature").
-    - Be in GitHub-flavored markdown format.
-    - Include contextually appropriate emojis (optional), but don't over do it.
+    * Use imperative mood (e.g., "Add feature").
+    * Be in GitHub-flavored markdown format.
+    * Include contextually appropriate emojis (optional), but don't over do it.
+    * Have a length that scales with the length of the diff context. If the DIFF is a small change,
+      respond quickly with a terse message so we can go faster.
+
+    BEGIN SAMPLE COMMIT MESSAGE
+    Update README with better instructions for installation
+
+    The previous instructions were not clear enough for new users, so we've updated them
+    with more sample use cases and an improved installation process. This should help
+    new users get started faster.
+
+    END SAMPLE COMMIT MESSAGE
 
     Start your response with the commit message. No prefix or introduction.
     Your entire response will be the commit message.
-
-    As for the length of the message, I want you to scale with the length of the diff context.
-    If the DIFF is a small change, respond quickly with a terse message so we can go faster.
 """
 )
 
 DEBUG_TEMPLATE = (
     """
     You are an expert software developer who knows how to debug code very effectively."""
     + get_personality_prompt()
```

### Comparing `aicodebot-0.9.0/aicodebot.egg-info/PKG-INFO` & `aicodebot-0.9.1/aicodebot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.9.0
+Version: 0.9.1
 Summary: Your AI-powered coding sidekick 🤖
 Home-page: https://github.com/gorillamania/AICodeBot
 Author: Nick Sullivan
 Keywords: AI,coding,assistant,pair-programming,automation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -34,30 +34,41 @@
 
 ⚠️ AICodeBot currently uses OpenAI's ChatGPT large language models, which can hallucinate and be confidently wrong. Sometimes AICodeBot does dumb things, which is why it's mostly *reading* and *advising* and not yet *writing*. Much like Tesla's "Full Self Driving", you have to keep your hands on the wheel.
 
 It's also not a "build a site for me in 5 minutes" tool that takes a well constructed prompt and builds a scaffold for you. There are [other tools](https://github.com/AntonOsika/gpt-engineer) for that. It's not a no-code platform. Instead, AICodeBot is built to work with existing code bases and the git-commit level. It's designed to multiply the effectiveness of capable engineers.
 
 ## Current features - how you can use it today
 
+| Task | Status |
+| --- | --- |
+| Generating quality commit messages | ✅ |
+| Thinking through tasks as a pair programmer | ✅ |
+| Suggestions for simple changes | ✅ |
+| Debugging | ✅ |
+| Doing code reviews | ✅ |
+| Explaining code | ✅ |
+| Writing tests | ✅ |
+| Modifying local files | Not yet, but soon! |
+| Searching the internet for answers | Not yet, but soon! |
+| Reading library documentation | Not yet, but soon! |
+| Writing senior developer level code | Not for a long time |
+| Major refactors | Not for a long time |
+| Build an app for me | Nope |
+
 ### AI Sidekick 🦸‍♂️
 
  `aicodebot sidekick` Your AI-powered coding assistant. It's designed to help you with your coding tasks by providing context-aware suggestions and solutions. Think ChatGPT with the ability to read local files for context.
 
  By default it will pass along a directory of files from the current working directory, and you can also pass in a list of files to use as context. For example:
 
  ```bash
  aicodebot sidekick file1.py file2.py
  ```
 
-In this example, the sidekick will read in the contents of file1.py and file2.py and use them to provide context-aware answers. For example:
-
-* How can I make this code better?
-* Tell me how to add a new feature to this code.
-* Fix an issue that I'm having... (paste the error, stack trace, etc.)
-* Write unit tests for the xyz function.
+In this example, the sidekick will read in the contents of file1.py and file2.py and use them to provide context-aware answers.
 
 Pro-tip: add your README.md to the list of files to get context-aware answers.
 
 This feature is in it's early phases right now, but it's already useful. We'll be adding support for tools that the sidekick can use, including GitHub integration, ingesting repository specific domain knowledge, writing local files, and more. For now, it just *reads* files and provides suggestions.
 
 ### AI-Assisted Git Commit 📝
 
@@ -76,39 +87,39 @@
 
 ## Installation and Usage
 
 To install AICodeBot, run:
 
 `pip install aicodebot`
 
-And then run `aicodebot --help` to get started.
+And then run `aicodebot configure` to get started.
 
 ```bash
 Usage: aicodebot [OPTIONS] COMMAND [ARGS]...
 
 Options:
   -V, --version  Show the version and exit.
   -h, --help     Show this message and exit.
 
 Commands:
   alignment  Get a message about Heart-Centered AI Alignment ❤ + 🤖.
   commit     Generate a commit message based on your changes.
+  configure  Create or update the config file
   debug      Run a command and debug the output.
   fun-fact   Get a fun fact about programming and artificial intelligence.
-  review     Do a code review, with [un]staged changes, or a specified...
-  sidekick   EXPERIMENTAL: Coding help from your AI sidekick
-  ```
+  review     Do a code review, with [un]staged changes, or a spe
+```
 
 ### Open AI key setup
 
 The first time you run it, you'll be prompted to enter your OpenAI API Key, which is required, as we use OpenAI's large language models for the AI. You can get one for free by visiting your [API key settings page](https://platform.openai.com/account/api-keys").
 
-#### Which Language Model? GPT-3.5 vs GPT-4
+Note: You will be billed by OpenAI based on how much you use it. Typical developers will use less than $10/month - which if you are a professional developer you'll likely more than make up for with saved time and higher quality work. See [OpenAI's pricing page](https://openai.com/pricing/) for more details.
 
-When using AICodeBot, you have the option to use either GPT-3.5 or GPT-4. While GPT-4 can often provide more accurate and detailed responses, GPT-3.5 is faster and might be sufficient for simpler tasks. We highly recommend GPT-4.
+#### Which Language Model? GPT-3.5 vs GPT-4
 
 Not all OpenAI accounts have GPT-4 API access enabled. By default, AICodeBot will use GPT-4 if your OpenAI account supports it, we will check the first time you run it. Tip: If your OpenAI API does not support GPT-4, you can ask to be added to the waitlist [here](https://openai.com/waitlist/gpt-4-api)
 
 Note: We'll be adding more options for AI models in the future, including those that can be run locally, such as [GPT4all](https://gpt4all.io/) and HuggingFace's [Transformers](https://huggingface.co/transformers/).
 
 ## Roadmap of Upcoming Features ️
```

### Comparing `aicodebot-0.9.0/pyproject.toml` & `aicodebot-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.9.0/setup.py` & `aicodebot-0.9.1/setup.py`

 * *Files identical despite different names*


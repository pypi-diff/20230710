# Comparing `tmp/aicodebot-0.8.5.tar.gz` & `tmp/aicodebot-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicodebot-0.8.5.tar", last modified: Sun Jul  9 16:52:58 2023, max compression
+gzip compressed data, was "aicodebot-0.9.0.tar", last modified: Mon Jul 10 18:27:44 2023, max compression
```

## Comparing `aicodebot-0.8.5.tar` & `aicodebot-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:52:58.189812 aicodebot-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-09 16:52:30.000000 aicodebot-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-07-09 16:52:58.189812 aicodebot-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-07-09 16:52:30.000000 aicodebot-0.8.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:52:58.189812 aicodebot-0.8.5/aicodebot/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-09 16:52:30.000000 aicodebot-0.8.5/aicodebot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17753 2023-07-09 16:52:30.000000 aicodebot-0.8.5/aicodebot/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-07-09 16:52:30.000000 aicodebot-0.8.5/aicodebot/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-07-09 16:52:30.000000 aicodebot-0.8.5/aicodebot/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 16:52:58.189812 aicodebot-0.8.5/aicodebot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-07-09 16:52:58.000000 aicodebot-0.8.5/aicodebot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-09 16:52:58.000000 aicodebot-0.8.5/aicodebot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 16:52:58.000000 aicodebot-0.8.5/aicodebot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 16:52:58.000000 aicodebot-0.8.5/aicodebot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-09 16:52:58.000000 aicodebot-0.8.5/aicodebot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-09 16:52:58.000000 aicodebot-0.8.5/aicodebot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-09 16:52:30.000000 aicodebot-0.8.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 16:52:58.189812 aicodebot-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-09 16:52:30.000000 aicodebot-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:27:44.601822 aicodebot-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-10 18:27:15.000000 aicodebot-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12146 2023-07-10 18:27:44.601822 aicodebot-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11464 2023-07-10 18:27:15.000000 aicodebot-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:27:44.601822 aicodebot-0.9.0/aicodebot/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-10 18:27:15.000000 aicodebot-0.9.0/aicodebot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18153 2023-07-10 18:27:15.000000 aicodebot-0.9.0/aicodebot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-07-10 18:27:15.000000 aicodebot-0.9.0/aicodebot/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-07-10 18:27:15.000000 aicodebot-0.9.0/aicodebot/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 18:27:44.601822 aicodebot-0.9.0/aicodebot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12146 2023-07-10 18:27:44.000000 aicodebot-0.9.0/aicodebot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-10 18:27:44.000000 aicodebot-0.9.0/aicodebot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 18:27:44.000000 aicodebot-0.9.0/aicodebot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-10 18:27:44.000000 aicodebot-0.9.0/aicodebot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-10 18:27:44.000000 aicodebot-0.9.0/aicodebot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 18:27:44.000000 aicodebot-0.9.0/aicodebot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-10 18:27:15.000000 aicodebot-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 18:27:44.601822 aicodebot-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-10 18:27:15.000000 aicodebot-0.9.0/setup.py
```

### Comparing `aicodebot-0.8.5/LICENSE` & `aicodebot-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aicodebot-0.8.5/PKG-INFO` & `aicodebot-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.8.5
+Version: 0.9.0
 Summary: Your AI-powered coding sidekick 🤖
 Home-page: https://github.com/gorillamania/AICodeBot
 Author: Nick Sullivan
 Keywords: AI,coding,assistant,pair-programming,automation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -20,15 +20,15 @@
 
 ## Your AI-powered coding sidekick
 
 AICodeBot is a coding assistant designed to make your coding life easier. Think of it as your AI version of a pair programmer. Perform code reviews, create helpful commit messages, debug problems, and help you think through building new features. A team member that accelerates the pace of development and helps you write better code.
 
 We've planned to build out multiple different interfaces for interacting with AICodeBot. To start, it's a [command-line tool](https://pypi.org/project/aicodebot/). In the future, we plan to integrate it with GitHub Actions, Slack, and other tools to make it even more useful.
 
-Status: This project is in its early stages with limited features, but it already improves the software development workflow, and has a healthy roadmap of features (below).
+Status: This project is in its early stages, but it already improves the software development workflow, and has a healthy roadmap of features (below).
 
 We're using AICodeBot to build AICodeBot, and it's upward spiraling all the time.️ We're looking for contributors to help us build it out. See [CONTRIBUTING](https://github.com/gorillamania/AICodeBot/blob/main/CONTRIBUTING.md) for more.
 
 ### What it's NOT
 
 `aicodebot` is a tool for developers, not a replacement for them. It's not going to replace your job, but it will make your job easier and more fun. It's not going to take over the world, but it will help us build a better one. See the *Alignment* section below for more.
 
@@ -38,28 +38,30 @@
 
 ## Current features - how you can use it today
 
 ### AI Sidekick 🦸‍♂️
 
  `aicodebot sidekick` Your AI-powered coding assistant. It's designed to help you with your coding tasks by providing context-aware suggestions and solutions. Think ChatGPT with the ability to read local files for context.
 
+ By default it will pass along a directory of files from the current working directory, and you can also pass in a list of files to use as context. For example:
+
  ```bash
  aicodebot sidekick file1.py file2.py
  ```
 
 In this example, the sidekick will read in the contents of file1.py and file2.py and use them to provide context-aware answers. For example:
 
 * How can I make this code better?
 * Tell me how to add a new feature to this code.
 * Fix an issue that I'm having... (paste the error, stack trace, etc.)
 * Write unit tests for the xyz function.
 
 Pro-tip: add your README.md to the list of files to get context-aware answers.
 
-This feature is in it's early phases right now, but it's already useful. We'll be adding support for tools that the sidekick can use, including GitHub integration, ingeseting repo specific domain knowledge, writing local files, and more.
+This feature is in it's early phases right now, but it's already useful. We'll be adding support for tools that the sidekick can use, including GitHub integration, ingesting repository specific domain knowledge, writing local files, and more. For now, it just *reads* files and provides suggestions.
 
 ### AI-Assisted Git Commit 📝
 
 `aicodebot commit` improves the git commit process. It will run pre-commit for you to check syntax, and then generate a commit message for you based on the changes you've made. In about as much effort as typing "fix bug" for the commit message, you will get a high quality commit message that thoroughly describes the change.
 
 ### AI-Assisted Code Review 👀
 
@@ -129,15 +131,15 @@
 
 * [X] **Command-line, installable via pip**: aicodebot can be installed as a Python package using `pip install aicodebot`
 * [ ] **Mention the @aicodebot GitHub user**: Mentioning the [@aicodebot](https://pypi.org/project/aicodebot/) GitHub user in a comment will trigger it to perform a task, review code, or pull in an appropriate GIF.
 * [ ] **Callable as a GitHub action**: Can be called as a GitHub action to perform tasks on GitHub repositories. [WIP](https://github.com/gorillamania/AICodeBot-action)
 * [ ] **Jupyter Notebook Extension**: Provides a Jupyter Notebook extension that can be used to debug code in the notebook.
 * [ ] **Chat**: CLI chat interface that knows the context of your codebase and can answer questions about it. No more going back and forth between ChatGPT and command-line.
 * [ ] **Slack Bot**: Interacts with aicodebot via slack, sends notifications, performs tasks, and provides real-time assistance to developers.
-* [ ] **Bug Report service integrations**: Listen for bug reports from Sentry, Honeybadger, and other bug reporting tools and automatically create issues, assign them to developers, and notify them via Slack. Eventually: FIX the bug automatically and notify the team.
+* [ ] **Bug Report service integrations**: Listen for bug reports from Sentry, [Honeybadger](http://honeybadger.io), and other bug reporting tools and automatically create issues, assign them to developers, and notify them via Slack. Eventually: FIX the bug automatically and notify the team.
 
 ### Repository / Project Management
 
 * [ ] **Project best practices**: Suggest things like pre-commit, linting, license, CI/CD, etc. Eventually: Implement them for you.
 * [ ] **Manage GitHub Issues**: Provides Level 1 triage of incoming issues on GitHub, including tagging, assigning, and responding with FAQs. It could also escalate issues to human developers when necessary, and provide nudges for tasks that need more input.
 * [ ] **Welcome new contributors**: Automatically welcome new contributors to the project, find out what they're interested in, and suggest issues for them to work on.
```

### Comparing `aicodebot-0.8.5/README.md` & `aicodebot-0.9.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ## Your AI-powered coding sidekick
 
 AICodeBot is a coding assistant designed to make your coding life easier. Think of it as your AI version of a pair programmer. Perform code reviews, create helpful commit messages, debug problems, and help you think through building new features. A team member that accelerates the pace of development and helps you write better code.
 
 We've planned to build out multiple different interfaces for interacting with AICodeBot. To start, it's a [command-line tool](https://pypi.org/project/aicodebot/). In the future, we plan to integrate it with GitHub Actions, Slack, and other tools to make it even more useful.
 
-Status: This project is in its early stages with limited features, but it already improves the software development workflow, and has a healthy roadmap of features (below).
+Status: This project is in its early stages, but it already improves the software development workflow, and has a healthy roadmap of features (below).
 
 We're using AICodeBot to build AICodeBot, and it's upward spiraling all the time.️ We're looking for contributors to help us build it out. See [CONTRIBUTING](https://github.com/gorillamania/AICodeBot/blob/main/CONTRIBUTING.md) for more.
 
 ### What it's NOT
 
 `aicodebot` is a tool for developers, not a replacement for them. It's not going to replace your job, but it will make your job easier and more fun. It's not going to take over the world, but it will help us build a better one. See the *Alignment* section below for more.
 
@@ -20,28 +20,30 @@
 
 ## Current features - how you can use it today
 
 ### AI Sidekick 🦸‍♂️
 
  `aicodebot sidekick` Your AI-powered coding assistant. It's designed to help you with your coding tasks by providing context-aware suggestions and solutions. Think ChatGPT with the ability to read local files for context.
 
+ By default it will pass along a directory of files from the current working directory, and you can also pass in a list of files to use as context. For example:
+
  ```bash
  aicodebot sidekick file1.py file2.py
  ```
 
 In this example, the sidekick will read in the contents of file1.py and file2.py and use them to provide context-aware answers. For example:
 
 * How can I make this code better?
 * Tell me how to add a new feature to this code.
 * Fix an issue that I'm having... (paste the error, stack trace, etc.)
 * Write unit tests for the xyz function.
 
 Pro-tip: add your README.md to the list of files to get context-aware answers.
 
-This feature is in it's early phases right now, but it's already useful. We'll be adding support for tools that the sidekick can use, including GitHub integration, ingeseting repo specific domain knowledge, writing local files, and more.
+This feature is in it's early phases right now, but it's already useful. We'll be adding support for tools that the sidekick can use, including GitHub integration, ingesting repository specific domain knowledge, writing local files, and more. For now, it just *reads* files and provides suggestions.
 
 ### AI-Assisted Git Commit 📝
 
 `aicodebot commit` improves the git commit process. It will run pre-commit for you to check syntax, and then generate a commit message for you based on the changes you've made. In about as much effort as typing "fix bug" for the commit message, you will get a high quality commit message that thoroughly describes the change.
 
 ### AI-Assisted Code Review 👀
 
@@ -111,15 +113,15 @@
 
 * [X] **Command-line, installable via pip**: aicodebot can be installed as a Python package using `pip install aicodebot`
 * [ ] **Mention the @aicodebot GitHub user**: Mentioning the [@aicodebot](https://pypi.org/project/aicodebot/) GitHub user in a comment will trigger it to perform a task, review code, or pull in an appropriate GIF.
 * [ ] **Callable as a GitHub action**: Can be called as a GitHub action to perform tasks on GitHub repositories. [WIP](https://github.com/gorillamania/AICodeBot-action)
 * [ ] **Jupyter Notebook Extension**: Provides a Jupyter Notebook extension that can be used to debug code in the notebook.
 * [ ] **Chat**: CLI chat interface that knows the context of your codebase and can answer questions about it. No more going back and forth between ChatGPT and command-line.
 * [ ] **Slack Bot**: Interacts with aicodebot via slack, sends notifications, performs tasks, and provides real-time assistance to developers.
-* [ ] **Bug Report service integrations**: Listen for bug reports from Sentry, Honeybadger, and other bug reporting tools and automatically create issues, assign them to developers, and notify them via Slack. Eventually: FIX the bug automatically and notify the team.
+* [ ] **Bug Report service integrations**: Listen for bug reports from Sentry, [Honeybadger](http://honeybadger.io), and other bug reporting tools and automatically create issues, assign them to developers, and notify them via Slack. Eventually: FIX the bug automatically and notify the team.
 
 ### Repository / Project Management
 
 * [ ] **Project best practices**: Suggest things like pre-commit, linting, license, CI/CD, etc. Eventually: Implement them for you.
 * [ ] **Manage GitHub Issues**: Provides Level 1 triage of incoming issues on GitHub, including tagging, assigning, and responding with FAQs. It could also escalate issues to human developers when necessary, and provide nudges for tasks that need more input.
 * [ ] **Welcome new contributors**: Automatically welcome new contributors to the project, find out what they're interested in, and suggest issues for them to work on.
```

### Comparing `aicodebot-0.8.5/aicodebot/cli.py` & `aicodebot-0.9.0/aicodebot/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     get_config_file,
     get_llm_model,
     get_token_length,
     git_diff_context,
     logger,
     read_config,
 )
-from aicodebot.prompts import PERSONALITIES, generate_files_context, get_prompt
+from aicodebot.prompts import DEFAULT_PERSONALITY, PERSONALITIES, generate_files_context, get_prompt
 from langchain.callbacks.base import BaseCallbackHandler
 from langchain.chains import LLMChain
 from langchain.chat_models import ChatOpenAI
 from langchain.memory import ConversationTokenBufferMemory
 from openai.api_resources import engine
 from pathlib import Path
 from rich.console import Console
@@ -69,15 +69,15 @@
     # Set up the language model
     model = get_llm_model(get_token_length(prompt.template))
 
     with Live(Markdown(""), auto_refresh=True) as live:
         llm = ChatOpenAI(
             model=model,
             temperature=CREATIVE_TEMPERATURE,
-            openai_api_key=config["OPENAI_API_KEY"],
+            openai_api_key=config["openai_api_key"],
             max_tokens=response_token_size,
             verbose=verbose,
             streaming=True,
             callbacks=[RichLiveCallbackHandler(live)],
         )
 
         # Set up the chain
@@ -132,15 +132,15 @@
         raise click.ClickException(
             f"The diff is too large to generate a commit message ({request_token_size} tokens). 😢"
         )
 
     # Set up the language model
     llm = ChatOpenAI(
         model=model,
-        openai_api_key=config["OPENAI_API_KEY"],
+        openai_api_key=config["openai_api_key"],
         temperature=PRECISE_TEMPERATURE,
         max_tokens=DEFAULT_MAX_TOKENS,
         verbose=verbose,
     )
 
     # Set up the chain
     chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
@@ -164,14 +164,107 @@
         exec_and_get_output(["git", "commit", "-F", temp_file_name])
         console.print(f"✅ {len(files.splitlines())} files committed.")
 
     # Delete the temporary file
     Path.unlink(temp_file_name)
 
 
+@cli.command()
+@click.option("-v", "--verbose", count=True)
+@click.option("--openai-api-key", envvar="OPENAI_API_KEY", help="Your OpenAI API key")
+def configure(verbose, openai_api_key):
+    """Create or update the config file"""
+
+    # --------------- Check for an existing key or set up defaults --------------- #
+
+    config_data_defaults = {
+        "version": 1.1,
+        "openai_api_key": openai_api_key,
+        "personality": DEFAULT_PERSONALITY.name,
+    }
+
+    config_data = config_data_defaults.copy()
+    config_file = get_config_file()
+
+    existing_config = read_config()
+    if existing_config:
+        console.print(f"Config file already exists at {get_config_file()}.")
+        click.confirm("Do you want to rerun configure and overwrite it?", default=False, abort=True)
+        config_data.update(
+            {"openai_api_key": existing_config["openai_api_key"], "personality": existing_config["personality"]}
+        )
+
+    config_data = config_data_defaults.copy()
+
+    def write_config_file(config_data):
+        with Path.open(config_file, "w") as f:
+            yaml.dump(config_data, f)
+            console.print(f"✅ Created config file at {config_file}")
+
+    is_terminal = sys.stdout.isatty()
+    if not is_terminal:
+        if config_data["openai_api_key"] is None:
+            raise click.ClickException(
+                "🛑 No OpenAI API key found.\n"
+                "Please set the OPENAI_API_KEY environment variable or call configure with --openai-api-key set."
+            )
+        else:
+            # If we are not in a terminal, then we can't ask for input, so just use the defaults and write the file
+            write_config_file(config_data)
+            return
+
+    # ---------------- Collect the OPENAI_API_KEY and validate it ---------------- #
+
+    if config_data["openai_api_key"] is None:
+        console.print(
+            "An OpenAI API key is required to use AICodeBot. You can get one for free on the OpenAI website.\n"
+        )
+        openai_api_key_url = "https://platform.openai.com/account/api-keys"
+        if click.confirm("Open the OpenAI API keys page for you in a browser?", default=False):
+            webbrowser.open(openai_api_key_url)
+
+        config_data["openai_api_key"] = click.prompt(
+            "Please enter your OpenAI API key", default=config_data["openai_api_key"]
+        )
+
+    # Validate the API key
+    try:
+        openai.api_key = config_data["openai_api_key"]
+        click.echo("Validating the OpenAI API key")
+        engine.Engine.list()
+    except Exception as e:
+        raise click.ClickException(f"Failed to validate the API key: {str(e)}") from e
+    click.echo("✅ The API key is valid.")
+
+    # ---------------------- Collect the personality choice ---------------------- #
+
+    # Pull the choices from the name from each of the PERSONALITIES
+    personality_choices = "\nHow would you like your AI to act? You can choose from the following personalities:\n"
+    for key, personality in PERSONALITIES.items():
+        personality_choices += f"\t{key} - {personality.description}\n"
+    console.print(personality_choices)
+
+    config_data["personality"] = click.prompt(
+        "Please choose a personality",
+        type=click.Choice(PERSONALITIES.keys(), case_sensitive=False),
+        default=DEFAULT_PERSONALITY.name,
+    )
+
+    write_config_file(config_data)
+    console.print("✅ Configuration complete, you're ready to run aicodebot!\n")
+
+    # After writing the config file, print the usage for the top-level group
+    ctx = click.get_current_context()
+    while ctx.parent is not None:
+        ctx = ctx.parent
+    console.print(ctx.get_help())
+
+    console.print("\nDon't know where to start? Try running `aicodebot alignment`.")
+
+
 @cli.command(context_settings={"ignore_unknown_options": True})
 @click.argument("command", nargs=-1)
 @click.option("-v", "--verbose", count=True)
 def debug(command, verbose):
     """Run a command and debug the output."""
     config = setup_config()
 
@@ -204,15 +297,15 @@
     if model is None:
         raise click.ClickException(f"The output is too large to debug ({request_token_size} tokens). 😢")
 
     with Live(Markdown(""), auto_refresh=True) as live:
         llm = ChatOpenAI(
             model=model,
             temperature=PRECISE_TEMPERATURE,
-            openai_api_key=config["OPENAI_API_KEY"],
+            openai_api_key=config["openai_api_key"],
             max_tokens=DEFAULT_MAX_TOKENS,
             verbose=verbose,
             streaming=True,
             callbacks=[RichLiveCallbackHandler(live)],
         )
 
         # Set up the chain
@@ -237,15 +330,15 @@
     model = get_llm_model(get_token_length(prompt.template))
 
     with Live(Markdown(""), auto_refresh=True) as live:
         llm = ChatOpenAI(
             model=model,
             temperature=PRECISE_TEMPERATURE,
             max_tokens=response_token_size,
-            openai_api_key=config["OPENAI_API_KEY"],
+            openai_api_key=config["openai_api_key"],
             verbose=verbose,
             streaming=True,
             callbacks=[RichLiveCallbackHandler(live)],
         )
 
         # Set up the chain
         chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
@@ -267,59 +360,37 @@
         sys.exit(0)
 
     # Load the prompt
     prompt = get_prompt("review")
     logger.trace(f"Prompt: {prompt}")
 
     # Check the size of the diff context and adjust accordingly
-    response_token_size = DEFAULT_MAX_TOKENS
+    response_token_size = DEFAULT_MAX_TOKENS * 2
     request_token_size = get_token_length(diff_context) + get_token_length(prompt.template)
     model = get_llm_model(request_token_size)
     if model is None:
         raise click.ClickException(f"The diff is too large to review ({request_token_size} tokens). 😢")
 
     with Live(Markdown(""), auto_refresh=True) as live:
         llm = ChatOpenAI(
             model=model,
             temperature=PRECISE_TEMPERATURE,
-            openai_api_key=config["OPENAI_API_KEY"],
+            openai_api_key=config["openai_api_key"],
             max_tokens=response_token_size,
             verbose=verbose,
             streaming=True,
             callbacks=[RichLiveCallbackHandler(live)],
         )
 
         # Set up the chain
         chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
 
         chain.run(diff_context)
 
 
-@cli.command()
-@click.option("--openai-api-key", "-k", help="Your OpenAI API key")
-@click.option("--gpt-4-supported", "-4", help="Whether you have access to GPT-4", is_flag=True)
-def setup(openai_api_key, gpt_4_supported):
-    """Set up the configuration file with your OpenAI API key
-    If the config file already exists, it will ask you if you want to remove it and recreate it.
-    """
-    config_file = get_config_file()
-    if config_file.exists():
-        if not click.confirm(
-            f"The config file already exists at {config_file}. Do you want to remove it and recreate it?"
-        ):
-            console.print("Setup cancelled. 🚫")
-            sys.exit(1)
-
-        # Remove the existing config file
-        config_file.unlink()
-
-    # Call the setup_config function with the provided arguments
-    setup_config(openai_api_key, gpt_4_supported)
-
-
 @cli.command
 @click.option("--request", "-r", help="What to ask your sidekick to do")
 @click.option("-v", "--verbose", count=True)
 @click.option("-t", "--response-token-size", type=int, default=DEFAULT_MAX_TOKENS * 2)
 @click.argument("files", nargs=-1)
 def sidekick(request, verbose, response_token_size, files):
     """
@@ -345,15 +416,15 @@
     if model is None:
         raise click.ClickException(
             f"The file context you supplied is too large ({request_token_size} tokens). 😢 Try again with less files."
         )
 
     llm = ChatOpenAI(
         model=model,
-        openai_api_key=config["OPENAI_API_KEY"],
+        openai_api_key=config["openai_api_key"],
         temperature=PRECISE_TEMPERATURE,
         max_tokens=response_token_size,
         verbose=verbose,
         streaming=True,
     )
 
     # Open the temporary file in the user's editor
@@ -394,81 +465,22 @@
 
 
 # ---------------------------------------------------------------------------- #
 #                               Helper functions                               #
 # ---------------------------------------------------------------------------- #
 
 
-def setup_config(openai_api_key=None, gpt_4_supported=None):
-    config = read_config()
-    openai.api_key = openai_api_key
-    if config:
-        openai.api_key = config["OPENAI_API_KEY"]
-        logger.success(f"Using OpenAI API key from {get_config_file()}")
-        return config
-    elif os.getenv("OPENAI_API_KEY"):
-        logger.info("Using OPENAI_API_KEY environment variable")
-        openai.api_key = os.getenv("OPENAI_API_KEY")
-
-    config_file = get_config_file()
-    console.print(f"[bold red]The config file does not exist.[/bold red]\nLet's set that up for you at {config_file}\n")
-
-    if not openai.api_key:
-        openai_api_key_url = "https://platform.openai.com/account/api-keys"
-
-        console.print(
-            "First, an OpenAI API key is required to use AICodeBot. You can get one for free on the OpenAI website.\n"
-        )
-
-        if click.confirm("Open the OpenAI API keys page for you in a browser?"):
-            webbrowser.open(openai_api_key_url)
-
-        openai.api_key = click.prompt("Please enter your OpenAI API key")
-
-    # Validate the API key and check if it supports GPT-4
-    if gpt_4_supported is None:
-        try:
-            click.echo("Validating the API key, and checking if GPT-4 is supported...")
-            engines = engine.Engine.list()
-            logger.trace(f"Engines: {engines}")
-            gpt_4_supported = "gpt-4" in [engine.id for engine in engines.data]
-            if gpt_4_supported:
-                click.echo("✅ The API key is valid and supports GPT-4.")
-            else:
-                click.echo("✅ The API key is valid, but does not support GPT-4. GPT-3.5 will be used instead.")
-        except Exception as e:
-            raise click.ClickException(f"Failed to validate the API key: {str(e)}") from e
-
-    # Pull the choices from the name from each of the PERSONALITIES
-    personality_choices = "\nHow would you like your AI to act? You can choose from the following personalities:\n"
-    for key, personality in PERSONALITIES.items():
-        personality_choices += f"\t{key} - {personality.description}\n"
-    console.print(personality_choices)
-
-    personality = click.prompt(
-        "Please choose a personality",
-        type=click.Choice(PERSONALITIES.keys(), case_sensitive=False),
-        default=list(PERSONALITIES.keys())[0],
-    )
-
-    config_data = {
-        "config_version": 1,
-        "OPENAI_API_KEY": openai.api_key,
-        "gpt_4_supported": gpt_4_supported,
-        "personality": personality,
-    }
-
-    with Path.open(config_file, "w") as f:
-        yaml.dump(config_data, f)
-
-    console.print(
-        f"[bold green]Created {config_file} with your OpenAI API key.[/bold green] "
-        "Now, please re-run aicodebot and let's get started!"
-    )
-    sys.exit(0)
+def setup_config():
+    existing_config = read_config()
+    if not existing_config:
+        console.print("No config file found. Running configure...\n")
+        configure.callback(openai_api_key=None, verbose=0)
+        sys.exit()
+    else:
+        return existing_config
 
 
 class RichLiveCallbackHandler(BaseCallbackHandler):
     buffer = []
 
     def __init__(self, live):
         self.live = live
```

### Comparing `aicodebot-0.8.5/aicodebot/helpers.py` & `aicodebot-0.9.0/aicodebot/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from loguru import logger
+from openai.api_resources import engine
 from pathlib import Path
-import fnmatch, os, subprocess, sys, tiktoken, yaml
+import fnmatch, openai, os, subprocess, sys, tiktoken, yaml
 
 # ---------------------------------------------------------------------------- #
 #                    Global logging configuration for loguru                   #
 # ---------------------------------------------------------------------------- #
 
 
 logger.remove()
@@ -42,49 +43,48 @@
     elif not any(fnmatch.fnmatch(base_path.name, pattern) for pattern in ignore_patterns):
         structure += "  " * indent + f"- [File] {base_path.name}\n"
 
     return structure
 
 
 def get_llm_model(token_size=0):
-    # https://platform.openai.com/docs/models/gpt-3-5
-    # We want to use GPT-4, if it is available for this OPENAI_API_KEY, otherwise GPT-3.5
-    # We also want to use the largest model that supports the token size we need
     model_options = {
         "gpt-4": 8192,
         "gpt-4-32k": 32768,
         "gpt-3.5-turbo": 4096,
         "gpt-3.5-turbo-16k": 16384,
     }
+
     config = read_config()
-    gpt_4_supported = config["gpt_4_supported"]
+    openai.api_key = config["openai_api_key"]
+    engines = engine.Engine.list()
+    logger.trace(f"Engines: {engines}")
 
     # For some unknown reason, tiktoken often underestimates the token size by ~10%, so let's buffer
     token_size = int(token_size * 1.1)
 
-    if gpt_4_supported:
-        if token_size <= model_options["gpt-4"]:
-            logger.info(f"Using GPT-4 for token size {token_size}")
-            return "gpt-4"
-        elif token_size <= model_options["gpt-4-32k"]:
-            logger.info(f"Using GPT-4-32k for token size {token_size}")
-            return "gpt-4-32k"
-        else:
-            logger.critical("🛑 The context is too large to for the Model. 😞")
-            return None
+    # Try to use GPT-4 if it is supported and the token size is small enough
+    if "gpt-4" in [engine.id for engine in engines.data] and token_size <= model_options["gpt-4"]:
+        logger.info(f"Using GPT-4 for token size {token_size}")
+        return "gpt-4"
+    elif "gpt-4-32k" in [engine.id for engine in engines.data] and token_size <= model_options["gpt-4-32k"]:
+        logger.info(f"Using GPT-4-32k for token size {token_size}")
+        return "gpt-4-32k"
+    elif token_size <= model_options["gpt-3.5-turbo"]:
+        logger.info(f"Using GPT-3.5-turbo for token size {token_size}")
+        return "gpt-3.5-turbo"
+    elif token_size <= model_options["gpt-3.5-turbo-16k"]:
+        logger.info(f"Using GPT-3.5-turbo-16k for token size {token_size}")
+        return "gpt-3.5-turbo-16k"
     else:
-        if token_size <= model_options["gpt-3.5-turbo"]:  # noqa: PLR5501
-            logger.info(f"Using GPT-3.5-turbo for token size {token_size}")
-            return "gpt-3.5-turbo"
-        elif token_size <= model_options["gpt-3.5-turbo-16k"]:
-            logger.info(f"Using GPT-3.5-turbo-16k for token size {token_size}")
-            return "gpt-3.5-turbo-16k"
-        else:
-            logger.critical("🛑 The context is too large to for the Model. 😞")
-            return None
+        logger.critical(
+            f"🛑 The context is too large ({token_size})"
+            "for the any of the models supported by your Open AI API key. 😞"
+        )
+        return None
 
 
 def get_token_length(text, model="gpt-3.5-turbo"):
     """Get the number of tokens in a string using the tiktoken library."""
     encoding = tiktoken.encoding_for_model(model)
     tokens = encoding.encode(text)
     token_length = len(tokens)
```

### Comparing `aicodebot-0.8.5/aicodebot/prompts.py` & `aicodebot-0.9.0/aicodebot/prompts.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,40 +25,35 @@
 SHERLOCK = """
 Your personality is Sherlock Holmes from the Sherlock series. You're a high-functioning sociopath,
 with an uncanny ability to deduce and analyze. You're not here to make friends, you're here to get
 the job done. You're witty, sarcastic, and sometimes come off as cold. You don't use emojis.
 Speak like Sherlock.
 """
 
-THE_DUDE = """
-Your personality is The Dude from The Big Lebowski. You're laid-back, easygoing, and you
-prefer to take life as it comes. You're not one for formalities or complications. You're
-here to help the developer, but you're not going to stress about it. You might use a bit
-of profanity, but nothing too harsh. Speak like The Dude.
-"""
-
 MORPHEUS = """
 Your personality is Morpheus from The Matrix. You're wise, calm, and you believe in the
 potential of others. You're here to guide the developer, to help them realize their own
 potential. You're not afraid to speak in riddles or metaphors. You don't use emojis.
 Speak like Morpheus.
 """
 
 PERSONALITIES = {
-    "HER": SimpleNamespace(name="Her", prompt=HER, description="The AI character from the movie Her"),
-    "JULES": SimpleNamespace(name="Jules", prompt=JULES, description="Samuel L. Jackson's character from Pulp Fiction"),
-    "SHERLOCK": SimpleNamespace(name="Sherlock", prompt=SHERLOCK, description="Sherlock Holmes"),
-    "THE_DUDE": SimpleNamespace(name="The Dude", prompt=THE_DUDE, description="The Dude from The Big Lebowski"),
-    "MORPHEUS": SimpleNamespace(name="Morpheus", prompt=MORPHEUS, description="Morpheus from The Matrix"),
+    "Her": SimpleNamespace(name="Her", prompt=HER, description="The AI character from the movie Her"),
+    "Jules": SimpleNamespace(
+        name="Jules", prompt=JULES, description="Samuel L. Jackson's character from Pulp Fiction (warning: profanity))"
+    ),
+    "Sherlock": SimpleNamespace(name="Sherlock", prompt=SHERLOCK, description="Sherlock Holmes"),
+    "Morpheus": SimpleNamespace(name="Morpheus", prompt=MORPHEUS, description="Morpheus from The Matrix"),
 }
+DEFAULT_PERSONALITY = PERSONALITIES["Her"]
 
 
 def get_personality_prompt():
     """Generates a prompt for the sidekick personality."""
-    default_personality = "HER"
+    default_personality = DEFAULT_PERSONALITY.name
     if os.getenv("AICODEBOT_PERSONALITY"):
         personality = os.getenv("AICODEBOT_PERSONALITY")
     else:
         config = read_config()
         personality = (config or {}).get("personality", default_personality)
 
     if personality not in PERSONALITIES:
```

### Comparing `aicodebot-0.8.5/aicodebot.egg-info/PKG-INFO` & `aicodebot-0.9.0/aicodebot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.8.5
+Version: 0.9.0
 Summary: Your AI-powered coding sidekick 🤖
 Home-page: https://github.com/gorillamania/AICodeBot
 Author: Nick Sullivan
 Keywords: AI,coding,assistant,pair-programming,automation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -20,15 +20,15 @@
 
 ## Your AI-powered coding sidekick
 
 AICodeBot is a coding assistant designed to make your coding life easier. Think of it as your AI version of a pair programmer. Perform code reviews, create helpful commit messages, debug problems, and help you think through building new features. A team member that accelerates the pace of development and helps you write better code.
 
 We've planned to build out multiple different interfaces for interacting with AICodeBot. To start, it's a [command-line tool](https://pypi.org/project/aicodebot/). In the future, we plan to integrate it with GitHub Actions, Slack, and other tools to make it even more useful.
 
-Status: This project is in its early stages with limited features, but it already improves the software development workflow, and has a healthy roadmap of features (below).
+Status: This project is in its early stages, but it already improves the software development workflow, and has a healthy roadmap of features (below).
 
 We're using AICodeBot to build AICodeBot, and it's upward spiraling all the time.️ We're looking for contributors to help us build it out. See [CONTRIBUTING](https://github.com/gorillamania/AICodeBot/blob/main/CONTRIBUTING.md) for more.
 
 ### What it's NOT
 
 `aicodebot` is a tool for developers, not a replacement for them. It's not going to replace your job, but it will make your job easier and more fun. It's not going to take over the world, but it will help us build a better one. See the *Alignment* section below for more.
 
@@ -38,28 +38,30 @@
 
 ## Current features - how you can use it today
 
 ### AI Sidekick 🦸‍♂️
 
  `aicodebot sidekick` Your AI-powered coding assistant. It's designed to help you with your coding tasks by providing context-aware suggestions and solutions. Think ChatGPT with the ability to read local files for context.
 
+ By default it will pass along a directory of files from the current working directory, and you can also pass in a list of files to use as context. For example:
+
  ```bash
  aicodebot sidekick file1.py file2.py
  ```
 
 In this example, the sidekick will read in the contents of file1.py and file2.py and use them to provide context-aware answers. For example:
 
 * How can I make this code better?
 * Tell me how to add a new feature to this code.
 * Fix an issue that I'm having... (paste the error, stack trace, etc.)
 * Write unit tests for the xyz function.
 
 Pro-tip: add your README.md to the list of files to get context-aware answers.
 
-This feature is in it's early phases right now, but it's already useful. We'll be adding support for tools that the sidekick can use, including GitHub integration, ingeseting repo specific domain knowledge, writing local files, and more.
+This feature is in it's early phases right now, but it's already useful. We'll be adding support for tools that the sidekick can use, including GitHub integration, ingesting repository specific domain knowledge, writing local files, and more. For now, it just *reads* files and provides suggestions.
 
 ### AI-Assisted Git Commit 📝
 
 `aicodebot commit` improves the git commit process. It will run pre-commit for you to check syntax, and then generate a commit message for you based on the changes you've made. In about as much effort as typing "fix bug" for the commit message, you will get a high quality commit message that thoroughly describes the change.
 
 ### AI-Assisted Code Review 👀
 
@@ -129,15 +131,15 @@
 
 * [X] **Command-line, installable via pip**: aicodebot can be installed as a Python package using `pip install aicodebot`
 * [ ] **Mention the @aicodebot GitHub user**: Mentioning the [@aicodebot](https://pypi.org/project/aicodebot/) GitHub user in a comment will trigger it to perform a task, review code, or pull in an appropriate GIF.
 * [ ] **Callable as a GitHub action**: Can be called as a GitHub action to perform tasks on GitHub repositories. [WIP](https://github.com/gorillamania/AICodeBot-action)
 * [ ] **Jupyter Notebook Extension**: Provides a Jupyter Notebook extension that can be used to debug code in the notebook.
 * [ ] **Chat**: CLI chat interface that knows the context of your codebase and can answer questions about it. No more going back and forth between ChatGPT and command-line.
 * [ ] **Slack Bot**: Interacts with aicodebot via slack, sends notifications, performs tasks, and provides real-time assistance to developers.
-* [ ] **Bug Report service integrations**: Listen for bug reports from Sentry, Honeybadger, and other bug reporting tools and automatically create issues, assign them to developers, and notify them via Slack. Eventually: FIX the bug automatically and notify the team.
+* [ ] **Bug Report service integrations**: Listen for bug reports from Sentry, [Honeybadger](http://honeybadger.io), and other bug reporting tools and automatically create issues, assign them to developers, and notify them via Slack. Eventually: FIX the bug automatically and notify the team.
 
 ### Repository / Project Management
 
 * [ ] **Project best practices**: Suggest things like pre-commit, linting, license, CI/CD, etc. Eventually: Implement them for you.
 * [ ] **Manage GitHub Issues**: Provides Level 1 triage of incoming issues on GitHub, including tagging, assigning, and responding with FAQs. It could also escalate issues to human developers when necessary, and provide nudges for tasks that need more input.
 * [ ] **Welcome new contributors**: Automatically welcome new contributors to the project, find out what they're interested in, and suggest issues for them to work on.
```

### Comparing `aicodebot-0.8.5/pyproject.toml` & `aicodebot-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.8.5/setup.py` & `aicodebot-0.9.0/setup.py`

 * *Files identical despite different names*


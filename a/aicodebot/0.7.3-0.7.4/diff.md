# Comparing `tmp/aicodebot-0.7.3.tar.gz` & `tmp/aicodebot-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicodebot-0.7.3.tar", last modified: Mon Jul  3 01:35:21 2023, max compression
+gzip compressed data, was "aicodebot-0.7.4.tar", last modified: Mon Jul  3 21:31:53 2023, max compression
```

## Comparing `aicodebot-0.7.3.tar` & `aicodebot-0.7.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:35:21.198485 aicodebot-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-03 01:34:50.000000 aicodebot-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-07-03 01:35:21.198485 aicodebot-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-07-03 01:34:50.000000 aicodebot-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:35:21.194485 aicodebot-0.7.3/aicodebot/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-03 01:34:50.000000 aicodebot-0.7.3/aicodebot/.aicodebot.template
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 01:34:50.000000 aicodebot-0.7.3/aicodebot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-03 01:34:50.000000 aicodebot-0.7.3/aicodebot/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)    14629 2023-07-03 01:34:50.000000 aicodebot-0.7.3/aicodebot/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-03 01:34:50.000000 aicodebot-0.7.3/aicodebot/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:35:21.198485 aicodebot-0.7.3/aicodebot/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 01:34:50.000000 aicodebot-0.7.3/aicodebot/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-03 01:34:50.000000 aicodebot-0.7.3/aicodebot/prompts/alignment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-03 01:34:50.000000 aicodebot-0.7.3/aicodebot/prompts/commit_message.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-03 01:34:50.000000 aicodebot-0.7.3/aicodebot/prompts/debug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-03 01:34:50.000000 aicodebot-0.7.3/aicodebot/prompts/fun_fact.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-03 01:34:50.000000 aicodebot-0.7.3/aicodebot/prompts/review.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 01:35:21.198485 aicodebot-0.7.3/aicodebot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-07-03 01:35:21.000000 aicodebot-0.7.3/aicodebot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-03 01:35:21.000000 aicodebot-0.7.3/aicodebot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 01:35:21.000000 aicodebot-0.7.3/aicodebot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-03 01:35:21.000000 aicodebot-0.7.3/aicodebot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-03 01:35:21.000000 aicodebot-0.7.3/aicodebot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 01:35:21.000000 aicodebot-0.7.3/aicodebot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-03 01:34:50.000000 aicodebot-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 01:35:21.198485 aicodebot-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-03 01:34:50.000000 aicodebot-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:31:53.405542 aicodebot-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-03 21:31:19.000000 aicodebot-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-07-03 21:31:53.401543 aicodebot-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-07-03 21:31:19.000000 aicodebot-0.7.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:31:53.401543 aicodebot-0.7.4/aicodebot/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-03 21:31:19.000000 aicodebot-0.7.4/aicodebot/.aicodebot.template
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-03 21:31:19.000000 aicodebot-0.7.4/aicodebot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-03 21:31:19.000000 aicodebot-0.7.4/aicodebot/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15281 2023-07-03 21:31:19.000000 aicodebot-0.7.4/aicodebot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-03 21:31:19.000000 aicodebot-0.7.4/aicodebot/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:31:53.401543 aicodebot-0.7.4/aicodebot/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 21:31:19.000000 aicodebot-0.7.4/aicodebot/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-03 21:31:19.000000 aicodebot-0.7.4/aicodebot/prompts/alignment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-03 21:31:19.000000 aicodebot-0.7.4/aicodebot/prompts/commit_message.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-03 21:31:19.000000 aicodebot-0.7.4/aicodebot/prompts/debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-03 21:31:19.000000 aicodebot-0.7.4/aicodebot/prompts/fun_fact.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-03 21:31:19.000000 aicodebot-0.7.4/aicodebot/prompts/review.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:31:53.401543 aicodebot-0.7.4/aicodebot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-07-03 21:31:53.000000 aicodebot-0.7.4/aicodebot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-03 21:31:53.000000 aicodebot-0.7.4/aicodebot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 21:31:53.000000 aicodebot-0.7.4/aicodebot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-03 21:31:53.000000 aicodebot-0.7.4/aicodebot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-03 21:31:53.000000 aicodebot-0.7.4/aicodebot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 21:31:53.000000 aicodebot-0.7.4/aicodebot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-03 21:31:19.000000 aicodebot-0.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 21:31:53.405542 aicodebot-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-03 21:31:19.000000 aicodebot-0.7.4/setup.py
```

### Comparing `aicodebot-0.7.3/LICENSE` & `aicodebot-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aicodebot-0.7.3/PKG-INFO` & `aicodebot-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.7.3
+Version: 0.7.4
 Summary: Your AI-powered coding sidekick 🤖
 Home-page: https://github.com/gorillamania/AICodeBot
 Author: Nick Sullivan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aicodebot-0.7.3/README.md` & `aicodebot-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `aicodebot-0.7.3/aicodebot/agents.py` & `aicodebot-0.7.4/aicodebot/agents.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.7.3/aicodebot/cli.py` & `aicodebot-0.7.4/aicodebot/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 from aicodebot import version as aicodebot_version
 from aicodebot.agents import get_agent
 from aicodebot.helpers import exec_and_get_output, get_token_length, git_diff_context
 from dotenv import load_dotenv
+from langchain.callbacks.base import BaseCallbackHandler
 from langchain.chains import LLMChain
 from langchain.chat_models import ChatOpenAI
 from langchain.prompts import load_prompt
 from openai.api_resources import engine
 from pathlib import Path
 from rich.console import Console
+from rich.live import Live
+from rich.markdown import Markdown
 from rich.style import Style
 import click, datetime, openai, os, random, subprocess, sys, tempfile, webbrowser
 
 # ----------------------------- Default settings ----------------------------- #
 
 DEFAULT_MAX_TOKENS = 512
-DEFAULT_TEMPERATURE = 0.1
+PRECISE_TEMPERATURE = 0
+CREATIVE_TEMPERATURE = 0.7
 DEFAULT_SPINNER = "point"
 
 # ----------------------- Setup for rich console output ---------------------- #
+
 console = Console()
 bot_style = Style(color="#30D5C8")
 error_style = Style(color="#FF0000")
 warning_style = Style(color="#FFA500")
 
-
 # -------------------------- Top level command group ------------------------- #
 
 
 @click.group()
 @click.version_option(aicodebot_version, "--version", "-V")
 @click.help_option("--help", "-h")
 def cli():
@@ -50,22 +54,29 @@
     setup_environment()
 
     # Load the prompt
     prompt = load_prompt(Path(__file__).parent / "prompts" / "alignment.yaml")
 
     # Set up the language model
     model = get_llm_model(get_token_length(prompt.template))
-    llm = ChatOpenAI(model=model, temperature=DEFAULT_TEMPERATURE, max_tokens=DEFAULT_MAX_TOKENS, verbose=verbose)
 
-    # Set up the chain
-    chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
+    with Live(Markdown(""), auto_refresh=True) as live:
+        llm = ChatOpenAI(
+            model=model,
+            temperature=CREATIVE_TEMPERATURE,
+            max_tokens=DEFAULT_MAX_TOKENS,
+            verbose=verbose,
+            streaming=True,
+            callbacks=[RichLiveCallbackHandler(live)],
+        )
 
-    with console.status("Generating an inspirational message", spinner=DEFAULT_SPINNER):
-        response = chain.run({})
-        console.print(response, style=bot_style)
+        # Set up the chain
+        chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
+
+        chain.run({})
 
 
 @cli.command()
 @click.option("-v", "--verbose", count=True)
 @click.option("-t", "--response-token-size", type=int, default=250)
 @click.option("-y", "--yes", is_flag=True, default=False, help="Don't ask for confirmation before committing.")
 @click.option("--skip-pre-commit", is_flag=True, help="Skip running pre-commit (otherwise run it if it is found).")
@@ -104,21 +115,21 @@
     # Check the size of the diff context and adjust accordingly
     request_token_size = get_token_length(diff_context) + get_token_length(prompt.template)
     model = get_llm_model(request_token_size)
     if verbose:
         console.print(f"Diff context token size: {request_token_size}, using model: {model}")
 
     # Set up the language model
-    llm = ChatOpenAI(model=model, temperature=DEFAULT_TEMPERATURE, max_tokens=DEFAULT_MAX_TOKENS, verbose=verbose)
+    llm = ChatOpenAI(model=model, temperature=PRECISE_TEMPERATURE, max_tokens=DEFAULT_MAX_TOKENS, verbose=verbose)
 
     # Set up the chain
     chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
 
     console.print("The following files will be committed:\n" + files)
-    with console.status("Generating the commit message", spinner=DEFAULT_SPINNER):
+    with console.status("Examining the diff and generating the commit message", spinner=DEFAULT_SPINNER):
         response = chain.run(diff_context)
 
     # Write the commit message to a temporary file
     with tempfile.NamedTemporaryFile(mode="w", delete=False) as temp:
         temp.write(str(response).strip())
         temp_file_name = temp.name
 
@@ -163,22 +174,28 @@
     console.print(f"The command exited with status {process.returncode}.")
 
     # Load the prompt
     prompt = load_prompt(Path(__file__).parent / "prompts" / "debug.yaml")
 
     # Set up the language model
     model = get_llm_model(get_token_length(error_output) + get_token_length(prompt.template))
-    llm = ChatOpenAI(model=model, temperature=DEFAULT_TEMPERATURE, max_tokens=DEFAULT_MAX_TOKENS, verbose=verbose)
 
-    # Set up the chain
-    chat_chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
+    with Live(Markdown(""), auto_refresh=True) as live:
+        llm = ChatOpenAI(
+            model=model,
+            temperature=PRECISE_TEMPERATURE,
+            max_tokens=DEFAULT_MAX_TOKENS,
+            verbose=verbose,
+            streaming=True,
+            callbacks=[RichLiveCallbackHandler(live)],
+        )
 
-    with console.status("Debugging", spinner=DEFAULT_SPINNER):
-        response = chat_chain.run(error_output)
-        console.print(response, style=bot_style)
+        # Set up the chain
+        chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
+        chain.run(error_output)
 
     sys.exit(process.returncode)
 
 
 @cli.command()
 @click.option("-v", "--verbose", count=True)
 def fun_fact(verbose):
@@ -186,24 +203,30 @@
     setup_environment()
 
     # Load the prompt
     prompt = load_prompt(Path(__file__).parent / "prompts" / "fun_fact.yaml")
 
     # Set up the language model
     model = get_llm_model(get_token_length(prompt.template))
-    llm = ChatOpenAI(model=model, temperature=0.9, max_tokens=250, verbose=verbose)
 
-    # Set up the chain
-    chat_chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
+    with Live(Markdown(""), auto_refresh=True) as live:
+        llm = ChatOpenAI(
+            model=model,
+            temperature=PRECISE_TEMPERATURE,
+            max_tokens=DEFAULT_MAX_TOKENS / 2,
+            verbose=verbose,
+            streaming=True,
+            callbacks=[RichLiveCallbackHandler(live)],
+        )
+
+        # Set up the chain
+        chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
 
-    with console.status("Fetching a fun fact", spinner=DEFAULT_SPINNER):
-        # Select a random year so that we get a different answer each time
         year = random.randint(1942, datetime.datetime.utcnow().year)
-        response = chat_chain.run(f"programming and artificial intelligence in the year {year}")
-        console.print(response, style=bot_style)
+        chain.run(f"programming and artificial intelligence in the year {year}")
 
 
 @cli.command
 @click.option("-c", "--commit", help="The commit hash to review (otherwise look at [un]staged changes).")
 @click.option("-v", "--verbose", count=True)
 def review(commit, verbose):
     """Do a code review, with [un]staged changes, or a specified commit."""
@@ -220,23 +243,28 @@
     # Check the size of the diff context and adjust accordingly
     response_token_size = DEFAULT_MAX_TOKENS / 2
     request_token_size = get_token_length(diff_context) + get_token_length(prompt.template)
     model = get_llm_model(request_token_size)
     if verbose:
         console.print(f"Diff context token size: {request_token_size}, using model: {model}")
 
-    # Set up the language model
-    llm = ChatOpenAI(model=model, temperature=DEFAULT_TEMPERATURE, max_tokens=response_token_size, verbose=verbose)
+    with Live(Markdown(""), auto_refresh=True) as live:
+        llm = ChatOpenAI(
+            model=model,
+            temperature=PRECISE_TEMPERATURE,
+            max_tokens=response_token_size,
+            verbose=verbose,
+            streaming=True,
+            callbacks=[RichLiveCallbackHandler(live)],
+        )
 
-    # Set up the chain
-    chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
+        # Set up the chain
+        chain = LLMChain(llm=llm, prompt=prompt, verbose=verbose)
 
-    with console.status("Reviewing code", spinner=DEFAULT_SPINNER):
-        response = chain.run(diff_context)
-        console.print(response, style=bot_style)
+        chain.run(diff_context)
 
 
 @cli.command
 @click.option("--task", "-t", help="The task you want to perform - a description of what you want to do.")
 @click.option("-v", "--verbose", count=True)
 def sidekick(task, verbose):
     """ALPHA/EXPERIMENTAL: Get coding help from your AI sidekick."""
@@ -249,15 +277,15 @@
         "See docs/sidekick.md for more information.",
         style=warning_style,
     )
 
     setup_environment()
 
     model = get_llm_model()
-    llm = ChatOpenAI(model=model, temperature=DEFAULT_TEMPERATURE, max_tokens=3500, verbose=verbose)
+    llm = ChatOpenAI(model=model, temperature=PRECISE_TEMPERATURE, max_tokens=2000, verbose=verbose)
 
     agent = get_agent("sidekick", llm, verbose)
 
     with console.status("Thinking", spinner=DEFAULT_SPINNER):
         response = agent({"input": task})
         console.print("")
         console.print(response["output"], style=bot_style)
@@ -353,9 +381,20 @@
             return "gpt-3.5-turbo"
         elif token_size <= model_options["gpt-3.5-turbo-16k"]:
             return "gpt-3.5-turbo-16k"
         else:
             raise click.ClickException("🛑 The context is too large to for the Model. 😞")
 
 
+class RichLiveCallbackHandler(BaseCallbackHandler):
+    buffer = []
+
+    def __init__(self, live):
+        self.live = live
+
+    def on_llm_new_token(self, token, **kwargs):
+        self.buffer.append(token)
+        self.live.update(Markdown("".join(self.buffer)))
+
+
 if __name__ == "__main__":
     cli()
```

### Comparing `aicodebot-0.7.3/aicodebot/helpers.py` & `aicodebot-0.7.4/aicodebot/helpers.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.7.3/aicodebot/prompts/commit_message.yaml` & `aicodebot-0.7.4/aicodebot/prompts/commit_message.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.7.3/aicodebot/prompts/review.yaml` & `aicodebot-0.7.4/aicodebot/prompts/review.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -25,7 +25,9 @@
 
     Consider the file names for context (e.g., "README.md" is a markdown file, "*.py" is a Python file).
     Understand the difference between code and comments. Comment lines start with ##, #, or //.
 
     The main focus is to tell me how I could make the code better.
 
     If the changes look good overall and don't require any feedback, then just respond with "LGTM" (looks good to me).
+
+    Respond in markdown format.
```

### Comparing `aicodebot-0.7.3/aicodebot.egg-info/PKG-INFO` & `aicodebot-0.7.4/aicodebot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.7.3
+Version: 0.7.4
 Summary: Your AI-powered coding sidekick 🤖
 Home-page: https://github.com/gorillamania/AICodeBot
 Author: Nick Sullivan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aicodebot-0.7.3/aicodebot.egg-info/SOURCES.txt` & `aicodebot-0.7.4/aicodebot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aicodebot-0.7.3/pyproject.toml` & `aicodebot-0.7.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.7.3/setup.py` & `aicodebot-0.7.4/setup.py`

 * *Files identical despite different names*


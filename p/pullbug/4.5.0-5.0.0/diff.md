# Comparing `tmp/pullbug-4.5.0.tar.gz` & `tmp/pullbug-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pullbug-4.5.0.tar", last modified: Tue Oct 25 20:03:20 2022, max compression
+gzip compressed data, was "pullbug-5.0.0.tar", last modified: Mon Jun 26 17:46:02 2023, max compression
```

## Comparing `pullbug-4.5.0.tar` & `pullbug-5.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 20:03:20.363772 pullbug-4.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-10-25 20:02:06.000000 pullbug-4.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4426 2022-10-25 20:03:20.363772 pullbug-4.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3937 2022-10-25 20:02:06.000000 pullbug-4.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 20:03:20.363772 pullbug-4.5.0/pullbug/
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-10-25 20:02:06.000000 pullbug-4.5.0/pullbug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13007 2022-10-25 20:02:06.000000 pullbug-4.5.0/pullbug/bug.py
--rw-r--r--   0 runner    (1001) docker     (121)     5183 2022-10-25 20:02:06.000000 pullbug-4.5.0/pullbug/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    10661 2022-10-25 20:02:06.000000 pullbug-4.5.0/pullbug/messages.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-25 20:02:06.000000 pullbug-4.5.0/pullbug/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 20:03:20.363772 pullbug-4.5.0/pullbug.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4426 2022-10-25 20:03:20.000000 pullbug-4.5.0/pullbug.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-10-25 20:03:20.000000 pullbug-4.5.0/pullbug.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 20:03:20.000000 pullbug-4.5.0/pullbug.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-10-25 20:03:20.000000 pullbug-4.5.0/pullbug.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-10-25 20:03:20.000000 pullbug-4.5.0/pullbug.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-25 20:03:20.000000 pullbug-4.5.0/pullbug.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-10-25 20:02:06.000000 pullbug-4.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-25 20:03:20.363772 pullbug-4.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-10-25 20:02:06.000000 pullbug-4.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 20:03:20.359772 pullbug-4.5.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 20:03:20.363772 pullbug-4.5.0/test/unit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-25 20:02:06.000000 pullbug-4.5.0/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6864 2022-10-25 20:02:06.000000 pullbug-4.5.0/test/unit/test_bug.py
--rw-r--r--   0 runner    (1001) docker     (121)    11135 2022-10-25 20:02:06.000000 pullbug-4.5.0/test/unit/test_messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:46:02.432378 pullbug-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-26 17:45:34.000000 pullbug-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-06-26 17:46:02.432378 pullbug-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-26 17:45:34.000000 pullbug-5.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:46:02.432378 pullbug-5.0.0/pullbug/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-26 17:45:34.000000 pullbug-5.0.0/pullbug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13702 2023-06-26 17:45:34.000000 pullbug-5.0.0/pullbug/bug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-06-26 17:45:34.000000 pullbug-5.0.0/pullbug/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10880 2023-06-26 17:45:34.000000 pullbug-5.0.0/pullbug/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:45:34.000000 pullbug-5.0.0/pullbug/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:46:02.432378 pullbug-5.0.0/pullbug.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-06-26 17:46:02.000000 pullbug-5.0.0/pullbug.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-26 17:46:02.000000 pullbug-5.0.0/pullbug.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:46:02.000000 pullbug-5.0.0/pullbug.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-26 17:46:02.000000 pullbug-5.0.0/pullbug.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-26 17:46:02.000000 pullbug-5.0.0/pullbug.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 17:46:02.000000 pullbug-5.0.0/pullbug.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-26 17:45:34.000000 pullbug-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 17:46:02.432378 pullbug-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-26 17:45:34.000000 pullbug-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:46:02.432378 pullbug-5.0.0/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:46:02.432378 pullbug-5.0.0/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:45:34.000000 pullbug-5.0.0/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-06-26 17:45:34.000000 pullbug-5.0.0/test/unit/test_bug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11147 2023-06-26 17:45:34.000000 pullbug-5.0.0/test/unit/test_messages.py
```

### Comparing `pullbug-4.5.0/LICENSE` & `pullbug-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pullbug-4.5.0/PKG-INFO` & `pullbug-5.0.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: pullbug
-Version: 4.5.0
-Summary: Get bugged via Discord or Slack to merge your GitHub pull requests or close open issues.
-Home-page: http://github.com/justintime50/pullbug
-Author: Justintime50
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7, <4
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 <div align="center">
 
 # Pullbug 🐛
 
 Get bugged via Discord or Slack to merge your GitHub pull requests or close open issues.
 
 [![Build Status](https://github.com/Justintime50/pullbug/workflows/build/badge.svg)](https://github.com/Justintime50/pullbug/actions)
@@ -42,48 +27,51 @@
 make install
 ```
 
 ## Usage
 
 Pullbug works best when run on a schedule. Run one-off reports or setup Pullbug to notify you at whatever interval you'd like to be bugged via Discord or Slack about pull requests.
 
-Pullbug is highly customizable allowing you to mix and match version control software along with messaging platforms to get the right fit. Additionally choose which kinds of pull requests to retrieve.
+Pullbug is highly customizable allowing you to choose which messaging service and what kinds of pull requests or issues you'd like.
 
-```
+```text
 Usage:
-    pullbug --github_token 123... --github_owner justintime50 --github_context users
+  pullbug --github_token 123... --github_owner justintime50 --github_context users
 
 Options:
-    -h, --help            show this help message and exit
-    -p, --pulls           Bug GitHub for Pull Requests.
-    -i, --issues          Bug GitHub for Issues.
-    -gt GITHUB_TOKEN, --github_token GITHUB_TOKEN
-                            The token to authenticate with GitHub.
-    -go GITHUB_OWNER, --github_owner GITHUB_OWNER
-                            The GitHub owner to retrieve pull requests or issues for (can be a user or organization).
-    -gs {closed,all,open}, --github_state {closed,all,open}
-                            The GitHub state to retrieve pull requests or issues for.
-    -gc {orgs,users}, --github_context {orgs,users}
-                            The GitHub context to retrieve pull requests or issues for.
-    -d, --discord         Send Pullbug messages to Discord.
-    -du DISCORD_URL, --discord_url DISCORD_URL
-                            The Discord webhook URL to send messages to.
-    -s, --slack           Send Pullbug messages to Slack.
-    -st SLACK_TOKEN, --slack_token SLACK_TOKEN
-                            The Slackbot token to authenticate with Slack.
-    -sc SLACK_CHANNEL, --slack_channel SLACK_CHANNEL
-                            The Slack channel to send messages to.
-    -r REPOS, --repos REPOS
-                            A comma-separated list of repos to run Pullbug against.
-    -dr, --drafts         Include draft pull requests.
-    -l LOCATION, --location LOCATION
-                            The location of the Pullbug logs and files.
-    --base_url BASE_URL   The base URL of your GitHub instance (useful for enterprise users with custom hostnames).
-    --log_level {error,debug,warning,info,critical}
-                            The log level used for the tool.
+  -h, --help            show this help message and exit
+  -p, --pulls           Bug GitHub for Pull Requests.
+  -i, --issues          Bug GitHub for Issues.
+  -gt GITHUB_TOKEN, --github_token GITHUB_TOKEN
+                        The token to authenticate with GitHub.
+  -go GITHUB_OWNER, --github_owner GITHUB_OWNER
+                        The GitHub owner to retrieve pull requests or issues for (can be a user or organization).
+  -gs {all,open,closed}, --github_state {all,open,closed}
+                        The GitHub state to retrieve pull requests or issues for.
+  -gc {orgs,users}, --github_context {orgs,users}
+                        The GitHub context to retrieve pull requests or issues for.
+  -d, --discord         Send Pullbug messages to Discord.
+  -du DISCORD_URL, --discord_url DISCORD_URL
+                        The Discord webhook URL to send messages to.
+  -s, --slack           Send Pullbug messages to Slack.
+  -st SLACK_TOKEN, --slack_token SLACK_TOKEN
+                        The Slackbot token to authenticate with Slack.
+  -sc SLACK_CHANNEL, --slack_channel SLACK_CHANNEL
+                        The Slack channel to send messages to.
+  -r REPOS, --repos REPOS
+                        A comma-separated list of repos to run Pullbug against.
+  -dr, --drafts         Include draft pull requests.
+  -l LOCATION, --location LOCATION
+                        The location of the Pullbug logs and files.
+  --base_url BASE_URL   The base URL of your GitHub instance (useful for enterprise users with custom hostnames).
+  --log_level {warning,debug,info,notset,error,critical}
+                        The log level used for the tool.
+  --disable_descriptions
+                        Disables descriptions in messages.
+  --quiet               Does not output when there is nothing to bug about.
 ```
 
 ## Development
 
 ```bash
 # Get a comprehensive list of development tools
 make help
```

### Comparing `pullbug-4.5.0/README.md` & `pullbug-5.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: pullbug
+Version: 5.0.0
+Summary: Get bugged via Discord or Slack to merge your GitHub pull requests or close open issues.
+Home-page: http://github.com/justintime50/pullbug
+Author: Justintime50
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8, <4
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 <div align="center">
 
 # Pullbug 🐛
 
 Get bugged via Discord or Slack to merge your GitHub pull requests or close open issues.
 
 [![Build Status](https://github.com/Justintime50/pullbug/workflows/build/badge.svg)](https://github.com/Justintime50/pullbug/actions)
@@ -27,48 +42,51 @@
 make install
 ```
 
 ## Usage
 
 Pullbug works best when run on a schedule. Run one-off reports or setup Pullbug to notify you at whatever interval you'd like to be bugged via Discord or Slack about pull requests.
 
-Pullbug is highly customizable allowing you to mix and match version control software along with messaging platforms to get the right fit. Additionally choose which kinds of pull requests to retrieve.
+Pullbug is highly customizable allowing you to choose which messaging service and what kinds of pull requests or issues you'd like.
 
-```
+```text
 Usage:
-    pullbug --github_token 123... --github_owner justintime50 --github_context users
+  pullbug --github_token 123... --github_owner justintime50 --github_context users
 
 Options:
-    -h, --help            show this help message and exit
-    -p, --pulls           Bug GitHub for Pull Requests.
-    -i, --issues          Bug GitHub for Issues.
-    -gt GITHUB_TOKEN, --github_token GITHUB_TOKEN
-                            The token to authenticate with GitHub.
-    -go GITHUB_OWNER, --github_owner GITHUB_OWNER
-                            The GitHub owner to retrieve pull requests or issues for (can be a user or organization).
-    -gs {closed,all,open}, --github_state {closed,all,open}
-                            The GitHub state to retrieve pull requests or issues for.
-    -gc {orgs,users}, --github_context {orgs,users}
-                            The GitHub context to retrieve pull requests or issues for.
-    -d, --discord         Send Pullbug messages to Discord.
-    -du DISCORD_URL, --discord_url DISCORD_URL
-                            The Discord webhook URL to send messages to.
-    -s, --slack           Send Pullbug messages to Slack.
-    -st SLACK_TOKEN, --slack_token SLACK_TOKEN
-                            The Slackbot token to authenticate with Slack.
-    -sc SLACK_CHANNEL, --slack_channel SLACK_CHANNEL
-                            The Slack channel to send messages to.
-    -r REPOS, --repos REPOS
-                            A comma-separated list of repos to run Pullbug against.
-    -dr, --drafts         Include draft pull requests.
-    -l LOCATION, --location LOCATION
-                            The location of the Pullbug logs and files.
-    --base_url BASE_URL   The base URL of your GitHub instance (useful for enterprise users with custom hostnames).
-    --log_level {error,debug,warning,info,critical}
-                            The log level used for the tool.
+  -h, --help            show this help message and exit
+  -p, --pulls           Bug GitHub for Pull Requests.
+  -i, --issues          Bug GitHub for Issues.
+  -gt GITHUB_TOKEN, --github_token GITHUB_TOKEN
+                        The token to authenticate with GitHub.
+  -go GITHUB_OWNER, --github_owner GITHUB_OWNER
+                        The GitHub owner to retrieve pull requests or issues for (can be a user or organization).
+  -gs {all,open,closed}, --github_state {all,open,closed}
+                        The GitHub state to retrieve pull requests or issues for.
+  -gc {orgs,users}, --github_context {orgs,users}
+                        The GitHub context to retrieve pull requests or issues for.
+  -d, --discord         Send Pullbug messages to Discord.
+  -du DISCORD_URL, --discord_url DISCORD_URL
+                        The Discord webhook URL to send messages to.
+  -s, --slack           Send Pullbug messages to Slack.
+  -st SLACK_TOKEN, --slack_token SLACK_TOKEN
+                        The Slackbot token to authenticate with Slack.
+  -sc SLACK_CHANNEL, --slack_channel SLACK_CHANNEL
+                        The Slack channel to send messages to.
+  -r REPOS, --repos REPOS
+                        A comma-separated list of repos to run Pullbug against.
+  -dr, --drafts         Include draft pull requests.
+  -l LOCATION, --location LOCATION
+                        The location of the Pullbug logs and files.
+  --base_url BASE_URL   The base URL of your GitHub instance (useful for enterprise users with custom hostnames).
+  --log_level {warning,debug,info,notset,error,critical}
+                        The log level used for the tool.
+  --disable_descriptions
+                        Disables descriptions in messages.
+  --quiet               Does not output when there is nothing to bug about.
 ```
 
 ## Development
 
 ```bash
 # Get a comprehensive list of development tools
 make help
```

### Comparing `pullbug-4.5.0/pullbug/bug.py` & `pullbug-5.0.0/pullbug/bug.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import os
 from typing import (
     Any,
     Dict,
     List,
+    Literal,
+    Optional,
     Tuple,
 )
 
 import woodchips
 from github import (
+    Auth,
     Github,
     Issue,
     NamedUser,
     PaginatedList,
     PullRequest,
 )
-from typing_extensions import Literal
 
 from pullbug.messages import Message
 
 
 GITHUB_STATE_CHOICES = Literal[
     'all',
     'closed',
@@ -44,15 +46,15 @@
 LOGGER_NAME = 'pullbug'
 
 
 class Pullbug:
     def __init__(  # nosec - no hardcoded token here, ignore
         self,
         github_owner: str,
-        github_token: str = None,
+        github_token: Optional[str] = None,
         github_state: GITHUB_STATE_CHOICES = 'open',
         github_context: GITHUB_CONTEXT_CHOICES = 'users',
         pulls: bool = False,
         issues: bool = False,
         discord: bool = False,
         discord_url: str = '',
         slack: bool = False,
@@ -60,14 +62,15 @@
         slack_channel: str = '',
         repos: str = '',
         drafts: bool = False,
         location: str = os.path.expanduser('~/pullbug'),
         base_url: str = DEFAULT_BASE_URL,
         log_level: str = DEFAULT_LOG_LEVEL,
         disable_descriptions: bool = False,
+        quiet: bool = False,
     ):
         # Parameter variables
         self.github_owner = github_owner
         self.github_token = github_token
         self.github_state = github_state
         self.github_context = github_context
         self.pulls = pulls
@@ -79,17 +82,21 @@
         self.slack_channel = slack_channel
         self.repos = [repo.strip() for repo in repos.lower().split(',')] if repos else ''
         self.drafts = drafts
         self.location = location
         self.base_url = base_url
         self.log_level = log_level
         self.disable_descriptions = disable_descriptions
+        self.quiet = quiet
 
         # Internal variables
-        self.github_instance = Github(login_or_token=self.github_token, base_url=self.base_url)
+        if github_token:
+            self.github_instance = Github(auth=Auth.Token(github_token), base_url=self.base_url)
+        else:
+            self.github_instance = Github(base_url=self.base_url)
 
     def run(self):
         """Run the logic to get PR's from GitHub and send that data via message."""
         self.setup_logger()
         logger = woodchips.get(LOGGER_NAME)
         logger.info('Running Pullbug...')
         self._run_missing_checks()
@@ -98,37 +105,49 @@
 
         if self.pulls:
             pull_requests = self.get_pull_requests(repos)
             slack_pull_messages, discord_pull_messages = self.iterate_pull_requests(pull_requests)
 
             # Check if there are pull requests and available messages to send (eg: filtering for drafts)
             if pull_requests != [] and slack_pull_messages:
+                found_pull_requests = True
                 pull_message_preamble = '\n:bug: *The following GitHub pull requests still need your help!*\n'
                 slack_pull_messages.insert(0, pull_message_preamble)
                 discord_pull_messages.insert(0, pull_message_preamble)
             else:
+                found_pull_requests = False
                 slack_pull_messages = discord_pull_messages = ['\n:bug: *Pullbug found no ready pull requests!*\n']
                 logger.info(slack_pull_messages[0])
 
-            self.send_messages(slack_pull_messages, discord_pull_messages)
+            if found_pull_requests is False and self.quiet:
+                # The user doesn't want messages sent when there are no pull requests
+                pass
+            else:
+                self.send_messages(slack_pull_messages, discord_pull_messages)
 
         if self.issues:
             issues = self.get_issues(repos)
             slack_issue_messages, discord_issue_messages = self.iterate_issues(issues)
 
             # Check if there are issues and available messages to send
             if issues != [] and slack_issue_messages:
+                found_issues = True
                 issue_message_preamble = '\n:bug: *The following GitHub issues still need your help!*\n'
                 slack_issue_messages.insert(0, issue_message_preamble)
                 discord_issue_messages.insert(0, issue_message_preamble)
             else:
+                found_issues = False
                 slack_issue_messages = discord_issue_messages = ['\n:bug: *Pullbug found no open issues!*\n']
                 logger.info(slack_issue_messages[0])
 
-            self.send_messages(slack_issue_messages, discord_issue_messages)
+            if found_issues is False and self.quiet:
+                # The user doesn't want messages sent when there are no issues
+                pass
+            else:
+                self.send_messages(slack_issue_messages, discord_issue_messages)
 
         logger.info('Pullbug finished bugging!')
 
     def setup_logger(self):
         """Setup a `woodchips` logger for the project."""
         logger = woodchips.Logger(
             name=LOGGER_NAME,
```

### Comparing `pullbug-4.5.0/pullbug/cli.py` & `pullbug-5.0.0/pullbug/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,14 +149,21 @@
         parser.add_argument(
             '--disable_descriptions',
             required=False,
             action='store_true',
             default=False,
             help='Disables descriptions in messages.',
         )
+        parser.add_argument(
+            '--quiet',
+            required=False,
+            action='store_true',
+            default=False,
+            help='Does not output when there is nothing to bug about.',
+        )
         parser.parse_args(namespace=self)
 
     def run(self):
         bug = Pullbug(
             self.github_owner,
             self.github_token,
             self.github_state,
@@ -170,14 +177,15 @@
             self.slack_channel,
             self.repos,
             self.drafts,
             self.location,
             self.base_url,
             self.log_level,
             self.disable_descriptions,
+            self.quiet,
         )
         bug.run()
 
 
 def main():
     PullBugCli().run()
```

### Comparing `pullbug-4.5.0/pullbug/messages.py` & `pullbug-5.0.0/pullbug/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,39 +17,46 @@
 
 
 LOGGER_NAME = 'pullbug'
 
 DESCRIPTION_CONTINUATION = '...'
 DESCRIPTION_MAX_LENGTH = 120
 
+TIMEOUT = 30
+
 
 class Message:
     @staticmethod
     def send_discord_message(messages: List[str], discord_url: str):
         """Send a Discord message.
 
         Discord has a hard limit of 2000 characters per message.
         As such, we break up the messages into batches, allow for
         breathing room, and send each batch of messages separately.
         """
         logger = woodchips.get(LOGGER_NAME)
 
         num_of_messages = len(messages)
+        # The message size of ~300 characters means we can send 6 messages per request plus some buffer room
         max_messages_per_batch = 6
         i = 1
         new_cutoff = max_messages_per_batch
         old_cutoff = 0
 
         while i <= math.ceil(num_of_messages / max_messages_per_batch):
             i += 1
             batch_message = ''.join(messages[old_cutoff:new_cutoff])
             new_cutoff += max_messages_per_batch
             old_cutoff += max_messages_per_batch
             try:
-                requests.post(discord_url, json={'content': batch_message})
+                requests.post(
+                    discord_url,
+                    json={'content': batch_message},
+                    timeout=TIMEOUT,
+                )
                 logger.info('Discord message sent!')
             except requests.exceptions.RequestException as discord_error:
                 logger.error(f'Could not send Discord message: {discord_error}')
                 raise requests.exceptions.RequestException(discord_error)
 
     @staticmethod
     def send_slack_message(messages: List[str], slack_token: str, slack_channel: str):
```

### Comparing `pullbug-4.5.0/pullbug.egg-info/PKG-INFO` & `pullbug-5.0.0/pullbug.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pullbug
-Version: 4.5.0
+Version: 5.0.0
 Summary: Get bugged via Discord or Slack to merge your GitHub pull requests or close open issues.
 Home-page: http://github.com/justintime50/pullbug
 Author: Justintime50
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7, <4
+Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
 
 # Pullbug 🐛
@@ -42,48 +42,51 @@
 make install
 ```
 
 ## Usage
 
 Pullbug works best when run on a schedule. Run one-off reports or setup Pullbug to notify you at whatever interval you'd like to be bugged via Discord or Slack about pull requests.
 
-Pullbug is highly customizable allowing you to mix and match version control software along with messaging platforms to get the right fit. Additionally choose which kinds of pull requests to retrieve.
+Pullbug is highly customizable allowing you to choose which messaging service and what kinds of pull requests or issues you'd like.
 
-```
+```text
 Usage:
-    pullbug --github_token 123... --github_owner justintime50 --github_context users
+  pullbug --github_token 123... --github_owner justintime50 --github_context users
 
 Options:
-    -h, --help            show this help message and exit
-    -p, --pulls           Bug GitHub for Pull Requests.
-    -i, --issues          Bug GitHub for Issues.
-    -gt GITHUB_TOKEN, --github_token GITHUB_TOKEN
-                            The token to authenticate with GitHub.
-    -go GITHUB_OWNER, --github_owner GITHUB_OWNER
-                            The GitHub owner to retrieve pull requests or issues for (can be a user or organization).
-    -gs {closed,all,open}, --github_state {closed,all,open}
-                            The GitHub state to retrieve pull requests or issues for.
-    -gc {orgs,users}, --github_context {orgs,users}
-                            The GitHub context to retrieve pull requests or issues for.
-    -d, --discord         Send Pullbug messages to Discord.
-    -du DISCORD_URL, --discord_url DISCORD_URL
-                            The Discord webhook URL to send messages to.
-    -s, --slack           Send Pullbug messages to Slack.
-    -st SLACK_TOKEN, --slack_token SLACK_TOKEN
-                            The Slackbot token to authenticate with Slack.
-    -sc SLACK_CHANNEL, --slack_channel SLACK_CHANNEL
-                            The Slack channel to send messages to.
-    -r REPOS, --repos REPOS
-                            A comma-separated list of repos to run Pullbug against.
-    -dr, --drafts         Include draft pull requests.
-    -l LOCATION, --location LOCATION
-                            The location of the Pullbug logs and files.
-    --base_url BASE_URL   The base URL of your GitHub instance (useful for enterprise users with custom hostnames).
-    --log_level {error,debug,warning,info,critical}
-                            The log level used for the tool.
+  -h, --help            show this help message and exit
+  -p, --pulls           Bug GitHub for Pull Requests.
+  -i, --issues          Bug GitHub for Issues.
+  -gt GITHUB_TOKEN, --github_token GITHUB_TOKEN
+                        The token to authenticate with GitHub.
+  -go GITHUB_OWNER, --github_owner GITHUB_OWNER
+                        The GitHub owner to retrieve pull requests or issues for (can be a user or organization).
+  -gs {all,open,closed}, --github_state {all,open,closed}
+                        The GitHub state to retrieve pull requests or issues for.
+  -gc {orgs,users}, --github_context {orgs,users}
+                        The GitHub context to retrieve pull requests or issues for.
+  -d, --discord         Send Pullbug messages to Discord.
+  -du DISCORD_URL, --discord_url DISCORD_URL
+                        The Discord webhook URL to send messages to.
+  -s, --slack           Send Pullbug messages to Slack.
+  -st SLACK_TOKEN, --slack_token SLACK_TOKEN
+                        The Slackbot token to authenticate with Slack.
+  -sc SLACK_CHANNEL, --slack_channel SLACK_CHANNEL
+                        The Slack channel to send messages to.
+  -r REPOS, --repos REPOS
+                        A comma-separated list of repos to run Pullbug against.
+  -dr, --drafts         Include draft pull requests.
+  -l LOCATION, --location LOCATION
+                        The location of the Pullbug logs and files.
+  --base_url BASE_URL   The base URL of your GitHub instance (useful for enterprise users with custom hostnames).
+  --log_level {warning,debug,info,notset,error,critical}
+                        The log level used for the tool.
+  --disable_descriptions
+                        Disables descriptions in messages.
+  --quiet               Does not output when there is nothing to bug about.
 ```
 
 ## Development
 
 ```bash
 # Get a comprehensive list of development tools
 make help
```

### Comparing `pullbug-4.5.0/setup.py` & `pullbug-5.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,35 +4,33 @@
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 REQUIREMENTS = [
     'PyGithub == 1.*',
     'requests == 2.*',
     'slackclient == 2.*',
-    'typing_extensions',  # TODO: Remove once we drop support for Python 3.7
     'woodchips == 0.2.*',
 ]
 
 DEV_REQUIREMENTS = [
     'bandit == 1.7.*',
-    'black == 22.*',
-    'build == 0.7.*',
-    'coveralls == 3.*',
-    'flake8 == 4.*',
+    'black == 23.*',
+    'build == 0.10.*',
+    'flake8 == 6.*',
     'isort == 5.*',
-    'mypy == 0.942',
+    'mypy == 1.3.*',
     'pytest == 7.*',
-    'pytest-cov == 3.*',
+    'pytest-cov == 4.*',
     'twine == 4.*',
     'types-requests',
 ]
 
 setuptools.setup(
     name='pullbug',
-    version='4.5.0',
+    version='5.0.0',
     description='Get bugged via Discord or Slack to merge your GitHub pull requests or close open issues.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://github.com/justintime50/pullbug',
     author='Justintime50',
     license='MIT',
     packages=setuptools.find_packages(
@@ -56,9 +54,9 @@
         'dev': DEV_REQUIREMENTS,
     },
     entry_points={
         'console_scripts': [
             'pullbug=pullbug.cli:main',
         ],
     },
-    python_requires='>=3.7, <4',
+    python_requires='>=3.8, <4',
 )
```

### Comparing `pullbug-4.5.0/test/unit/test_bug.py` & `pullbug-5.0.0/test/unit/test_bug.py`

 * *Files 7% similar despite different names*

```diff
@@ -227,7 +227,28 @@
         github_owner='justintime50',
         slack=True,
         slack_token=mock_token,
         slack_channel=mock_channel,
     ).send_messages(slack_messages, discord_messages)
 
     mock_send_slack_message.assert_called_once_with(slack_messages, mock_token, mock_channel)
+
+
+@patch('pullbug.bug.Pullbug.send_messages')
+@patch('pullbug.bug.Pullbug.get_pull_requests')
+@patch('pullbug.bug.Pullbug.get_repos')
+@patch('logging.Logger.info')
+def test_no_messages_when_quiet(mock_logger, mock_get_repos, mock_pull_request, mock_send_messages):
+    """Tests that we do not send messages when the user passes the `quiet` flag."""
+    Pullbug(
+        github_owner='justintime50',
+        github_token='123',
+        github_context='users',
+        pulls=True,
+        issues=True,
+        quiet=True,
+    ).run()
+
+    mock_get_repos.assert_called_once()
+    mock_pull_request.assert_called_once()
+    mock_logger.assert_called()
+    mock_send_messages.assert_not_called()
```

### Comparing `pullbug-4.5.0/test/unit/test_messages.py` & `pullbug-5.0.0/test/unit/test_messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 @patch('logging.Logger.info')
 @patch('requests.post')
 def test_discord_success(mock_request, mock_logger, mock_url, mock_messages):
     """Tests that we can send a Discord message."""
     Message.send_discord_message(mock_messages, mock_url)
 
-    mock_request.assert_called_once_with(mock_url, json={'content': mock_messages[0]})
+    mock_request.assert_called_once_with(mock_url, json={'content': mock_messages[0]}, timeout=30)
     mock_logger.assert_called_once_with('Discord message sent!')
 
 
 @patch('logging.Logger.error')
 @patch('requests.post', side_effect=requests.exceptions.RequestException('mock-error'))
 def test_discord_exception(mock_request, mock_logger, mock_url, mock_messages):
     """Tests that we log errors when sending Discord messages."""
```


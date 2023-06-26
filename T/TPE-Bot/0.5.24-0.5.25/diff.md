# Comparing `tmp/TPE_Bot-0.5.24.tar.gz` & `tmp/TPE_Bot-0.5.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TPE_Bot-0.5.24.tar", last modified: Mon Jun 26 06:32:02 2023, max compression
+gzip compressed data, was "TPE_Bot-0.5.25.tar", last modified: Mon Jun 26 06:35:50 2023, max compression
```

## Comparing `TPE_Bot-0.5.24.tar` & `TPE_Bot-0.5.25.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.874245 TPE_Bot-0.5.24/
--rw-rw-rw-   0        0        0      242 2023-06-26 06:32:02.873247 TPE_Bot-0.5.24/PKG-INFO
--rw-rw-rw-   0        0        0      720 2023-05-23 10:33:05.000000 TPE_Bot-0.5.24/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.290712 TPE_Bot-0.5.24/TPE_Bot.egg-info/
--rw-rw-rw-   0        0        0      242 2023-06-26 06:32:02.000000 TPE_Bot-0.5.24/TPE_Bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6530 2023-06-26 06:32:02.000000 TPE_Bot-0.5.24/TPE_Bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 06:32:02.000000 TPE_Bot-0.5.24/TPE_Bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-06-26 06:32:02.000000 TPE_Bot-0.5.24/TPE_Bot.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.450800 TPE_Bot-0.5.24/buildABot/
--rw-rw-rw-   0        0        0    40255 2023-05-17 19:55:47.000000 TPE_Bot-0.5.24/buildABot/Analytics.py
-drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.452793 TPE_Bot-0.5.24/buildABot/Data/
-drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.544065 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/
--rw-rw-rw-   0        0        0     1062 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Default Fallback Intent.json
--rw-rw-rw-   0        0        0     1096 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Default Welcome Intent - fallback.json
--rw-rw-rw-   0        0        0     3158 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Default Welcome Intent.json
--rw-rw-rw-   0        0        0      244 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Default Welcome Intent_usersays_en.json
--rw-rw-rw-   0        0        0     1131 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Downvote.json
--rw-rw-rw-   0        0        0      982 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Downvote_usersays_en.json
--rw-rw-rw-   0        0        0     3785 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Email Enquiry.json
--rw-rw-rw-   0        0        0     2453 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Email Enquiry_usersays_en.json
--rw-rw-rw-   0        0        0     1518 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Exit Conversation.json
--rw-rw-rw-   0        0        0     2173 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Exit Conversation_usersays_en.json
--rw-rw-rw-   0        0        0      682 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Fallback - Logged In - fallback.json
--rw-rw-rw-   0        0        0     1525 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Fallback - Logged In - no.json
--rw-rw-rw-   0        0        0    10929 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Fallback - Logged In - no_usersays_en.json
--rw-rw-rw-   0        0        0     1074 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Fallback - Logged In - yes.json
--rw-rw-rw-   0        0        0    10255 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Fallback - Logged In - yes_usersays_en.json
--rw-rw-rw-   0        0        0     1164 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Remember Name.json
--rw-rw-rw-   0        0        0      239 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Remember Name_usersays_en.json
--rw-rw-rw-   0        0        0     2186 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password - Correct.json
--rw-rw-rw-   0        0        0      613 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password - Correct_usersays_en.json
--rw-rw-rw-   0        0        0     1177 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback - fallback.json
--rw-rw-rw-   0        0        0     1238 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback.json
--rw-rw-rw-   0        0        0     1197 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password - fallback.json
--rw-rw-rw-   0        0        0     2257 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password.json
--rw-rw-rw-   0        0        0      752 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password_usersays_en.json
--rw-rw-rw-   0        0        0      249 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Sentiment (Awesome)_usersays_en.json
--rw-rw-rw-   0        0        0      252 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Sentiment (Doing Fine)_usersays_en.json
--rw-rw-rw-   0        0        0      264 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Sentiment (It's been a rough week)_usersays_en.json
--rw-rw-rw-   0        0        0      261 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Sentiment (Still Hanging There)_usersays_en.json
--rw-rw-rw-   0        0        0     1665 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In.json
--rw-rw-rw-   0        0        0      597 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In_usersays_en.json
--rw-rw-rw-   0        0        0     1741 2023-05-17 19:35:50.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Menu - Main.json
--rw-rw-rw-   0        0        0     2454 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Menu - Main_usersays_en.json
--rw-rw-rw-   0        0        0     1079 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Thankyou.json
--rw-rw-rw-   0        0        0     1496 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Thankyou_usersays_en.json
--rw-rw-rw-   0        0        0      891 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Upvote.json
--rw-rw-rw-   0        0        0      241 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Upvote_usersays_en.json
-drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.638333 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/
--rw-rw-rw-   0        0        0     1062 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Default Fallback Intent.json
--rw-rw-rw-   0        0        0     1096 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Default Welcome Intent - fallback.json
--rw-rw-rw-   0        0        0     3158 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Default Welcome Intent.json
--rw-rw-rw-   0        0        0      244 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Default Welcome Intent_usersays_en.json
--rw-rw-rw-   0        0        0     1131 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Downvote.json
--rw-rw-rw-   0        0        0      982 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Downvote_usersays_en.json
--rw-rw-rw-   0        0        0     3785 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Email Enquiry.json
--rw-rw-rw-   0        0        0     2453 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Email Enquiry_usersays_en.json
--rw-rw-rw-   0        0        0     1518 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Exit Conversation.json
--rw-rw-rw-   0        0        0     2173 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Exit Conversation_usersays_en.json
--rw-rw-rw-   0        0        0      682 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Fallback - Logged In - fallback.json
--rw-rw-rw-   0        0        0     1525 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Fallback - Logged In - no.json
--rw-rw-rw-   0        0        0    10929 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Fallback - Logged In - no_usersays_en.json
--rw-rw-rw-   0        0        0     1074 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Fallback - Logged In - yes.json
--rw-rw-rw-   0        0        0    10255 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Fallback - Logged In - yes_usersays_en.json
--rw-rw-rw-   0        0        0     1164 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Remember Name.json
--rw-rw-rw-   0        0        0      239 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Remember Name_usersays_en.json
--rw-rw-rw-   0        0        0     2186 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct.json
--rw-rw-rw-   0        0        0      613 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct_usersays_en.json
--rw-rw-rw-   0        0        0     2219 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password - Template.json
--rw-rw-rw-   0        0        0     1177 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback - fallback.json
--rw-rw-rw-   0        0        0     1238 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback.json
--rw-rw-rw-   0        0        0     1197 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback.json
--rw-rw-rw-   0        0        0      752 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password_usersays_en.json
--rw-rw-rw-   0        0        0      249 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Sentiment (Awesome)_usersays_en.json
--rw-rw-rw-   0        0        0      252 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Sentiment (Doing Fine)_usersays_en.json
--rw-rw-rw-   0        0        0      264 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Sentiment (It's been a rough week)_usersays_en.json
--rw-rw-rw-   0        0        0      261 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Sentiment (Still Hanging There)_usersays_en.json
--rw-rw-rw-   0        0        0     1665 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In.json
--rw-rw-rw-   0        0        0      597 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In_usersays_en.json
--rw-rw-rw-   0        0        0     2076 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Menu - Main.json
--rw-rw-rw-   0        0        0     2454 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Menu - Main_usersays_en.json
--rw-rw-rw-   0        0        0     1079 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Thankyou.json
--rw-rw-rw-   0        0        0     1496 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Thankyou_usersays_en.json
--rw-rw-rw-   0        0        0      891 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Upvote.json
--rw-rw-rw-   0        0        0      241 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Upvote_usersays_en.json
-drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.645310 TPE_Bot-0.5.24/buildABot/Data/Default - Worksheets/
--rw-rw-rw-   0        0        0      249 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Worksheets/Log In - Sentiment (Awesome)_usersays_en.json
--rw-rw-rw-   0        0        0      252 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Worksheets/Log In - Sentiment (Doing Fine)_usersays_en.json
--rw-rw-rw-   0        0        0      264 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Worksheets/Log In - Sentiment (It's been a rough week)_usersays_en.json
--rw-rw-rw-   0        0        0      261 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Worksheets/Log In - Sentiment (Still Hanging There)_usersays_en.json
-drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.650296 TPE_Bot-0.5.24/buildABot/Data/Entities/
--rw-rw-rw-   0        0        0      208 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Entities/LoginID.json
-drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.798931 TPE_Bot-0.5.24/buildABot/Data/WebApp/
--rw-rw-rw-   0        0        0    26827 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/WebApp/index_template_LEARN.html
--rw-rw-rw-   0        0        0    21879 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/WebApp/index_template_RECO.html
--rw-rw-rw-   0        0        0   817197 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/WebApp/reset_template_RECO.js
-drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.826856 TPE_Bot-0.5.24/buildABot/Data/Webhook/
--rw-rw-rw-   0        0        0     2162 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Webhook/CheckPwd_Template_RECO.js
--rw-rw-rw-   0        0        0     4597 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Webhook/RecommendedMenu_Template_RECO.js
--rw-rw-rw-   0        0        0     7331 2023-05-17 19:11:48.000000 TPE_Bot-0.5.24/buildABot/Data/Webhook/index_template_LEARN.js
--rw-rw-rw-   0        0        0    10693 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Webhook/index_template_RECO.js
--rw-rw-rw-   0        0        0       89 2023-05-15 04:03:04.000000 TPE_Bot-0.5.24/buildABot/Data/__init__.py
--rw-rw-rw-   0        0        0    15847 2023-05-17 19:55:48.000000 TPE_Bot-0.5.24/buildABot/Entities.py
--rw-rw-rw-   0        0        0    12267 2023-05-17 19:55:48.000000 TPE_Bot-0.5.24/buildABot/FallbackSocialTag.py
--rw-rw-rw-   0        0        0    12103 2023-05-17 19:55:48.000000 TPE_Bot-0.5.24/buildABot/Firebase_Learn.py
--rw-rw-rw-   0        0        0    14567 2023-06-26 06:30:22.000000 TPE_Bot-0.5.24/buildABot/Firebase_Reco.py
--rw-rw-rw-   0        0        0    36243 2023-05-17 19:55:48.000000 TPE_Bot-0.5.24/buildABot/Intents.py
--rw-rw-rw-   0        0        0    42387 2023-05-18 07:15:14.000000 TPE_Bot-0.5.24/buildABot/LearnMenu.py
--rw-rw-rw-   0        0        0    79895 2023-05-18 10:21:25.000000 TPE_Bot-0.5.24/buildABot/Manager.py
--rw-rw-rw-   0        0        0    15947 2023-05-17 19:55:48.000000 TPE_Bot-0.5.24/buildABot/Paraphraser.py
--rw-rw-rw-   0        0        0     6151 2023-05-17 19:55:48.000000 TPE_Bot-0.5.24/buildABot/Password.py
--rw-rw-rw-   0        0        0    44723 2023-05-17 19:55:48.000000 TPE_Bot-0.5.24/buildABot/RecommendedMenu.py
--rw-rw-rw-   0        0        0     8791 2023-05-17 19:55:48.000000 TPE_Bot-0.5.24/buildABot/TelegramLogs.py
--rw-rw-rw-   0        0        0     7539 2023-05-17 19:55:48.000000 TPE_Bot-0.5.24/buildABot/WebApp_Learn.py
--rw-rw-rw-   0        0        0    11283 2023-05-17 19:55:48.000000 TPE_Bot-0.5.24/buildABot/WebApp_Reco.py
--rw-rw-rw-   0        0        0     9259 2023-05-17 19:55:48.000000 TPE_Bot-0.5.24/buildABot/Webhook_Learn.py
--rw-rw-rw-   0        0        0    33791 2023-05-18 09:37:37.000000 TPE_Bot-0.5.24/buildABot/Webhook_Reco.py
--rw-rw-rw-   0        0        0    23915 2023-05-16 14:52:33.000000 TPE_Bot-0.5.24/buildABot/Worksheets.py
--rw-rw-rw-   0        0        0    23811 2023-05-18 10:10:18.000000 TPE_Bot-0.5.24/buildABot/Worksheets_Learn.py
--rw-rw-rw-   0        0        0    23923 2023-05-18 10:10:18.000000 TPE_Bot-0.5.24/buildABot/Worksheets_Reco.py
--rw-rw-rw-   0        0        0     5075 2023-05-17 19:55:48.000000 TPE_Bot-0.5.24/buildABot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.833837 TPE_Bot-0.5.24/buildABot/pytransform/
--rw-rw-rw-   0        0        0    13587 2023-03-23 18:24:51.000000 TPE_Bot-0.5.24/buildABot/pytransform/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.855778 TPE_Bot-0.5.24/parrot/
--rw-rw-rw-   0        0        0     1219 2023-05-16 14:54:08.000000 TPE_Bot-0.5.24/parrot/__init__.py
--rw-rw-rw-   0        0        0     3643 2023-05-16 14:54:08.000000 TPE_Bot-0.5.24/parrot/demo.py
--rw-rw-rw-   0        0        0    25523 2023-05-16 14:54:08.000000 TPE_Bot-0.5.24/parrot/filters.py
--rw-rw-rw-   0        0        0    16591 2023-05-16 14:54:08.000000 TPE_Bot-0.5.24/parrot/parrot.py
-drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.864757 TPE_Bot-0.5.24/parrot/pytransform/
--rw-rw-rw-   0        0        0    13587 2023-03-23 18:24:51.000000 TPE_Bot-0.5.24/parrot/pytransform/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.872247 TPE_Bot-0.5.24/pytransform/
--rw-rw-rw-   0        0        0    13587 2023-03-23 18:24:51.000000 TPE_Bot-0.5.24/pytransform/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-26 06:32:02.874245 TPE_Bot-0.5.24/setup.cfg
--rw-rw-rw-   0        0        0      575 2023-06-26 06:31:53.000000 TPE_Bot-0.5.24/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 06:35:50.589748 TPE_Bot-0.5.25/
+-rw-rw-rw-   0        0        0      242 2023-06-26 06:35:50.589748 TPE_Bot-0.5.25/PKG-INFO
+-rw-rw-rw-   0        0        0      720 2023-05-23 10:33:05.000000 TPE_Bot-0.5.25/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 06:35:50.470550 TPE_Bot-0.5.25/TPE_Bot.egg-info/
+-rw-rw-rw-   0        0        0      242 2023-06-26 06:35:50.000000 TPE_Bot-0.5.25/TPE_Bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6530 2023-06-26 06:35:50.000000 TPE_Bot-0.5.25/TPE_Bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 06:35:50.000000 TPE_Bot-0.5.25/TPE_Bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-06-26 06:35:50.000000 TPE_Bot-0.5.25/TPE_Bot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 06:35:50.500474 TPE_Bot-0.5.25/buildABot/
+-rw-rw-rw-   0        0        0    40255 2023-05-17 19:55:47.000000 TPE_Bot-0.5.25/buildABot/Analytics.py
+drwxrwxrwx   0        0        0        0 2023-06-26 06:35:50.501471 TPE_Bot-0.5.25/buildABot/Data/
+drwxrwxrwx   0        0        0        0 2023-06-26 06:35:50.535915 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/
+-rw-rw-rw-   0        0        0     1062 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Default Fallback Intent.json
+-rw-rw-rw-   0        0        0     1096 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Default Welcome Intent - fallback.json
+-rw-rw-rw-   0        0        0     3158 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Default Welcome Intent.json
+-rw-rw-rw-   0        0        0      244 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Default Welcome Intent_usersays_en.json
+-rw-rw-rw-   0        0        0     1131 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Downvote.json
+-rw-rw-rw-   0        0        0      982 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Downvote_usersays_en.json
+-rw-rw-rw-   0        0        0     3785 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Email Enquiry.json
+-rw-rw-rw-   0        0        0     2453 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Email Enquiry_usersays_en.json
+-rw-rw-rw-   0        0        0     1518 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Exit Conversation.json
+-rw-rw-rw-   0        0        0     2173 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Exit Conversation_usersays_en.json
+-rw-rw-rw-   0        0        0      682 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Fallback - Logged In - fallback.json
+-rw-rw-rw-   0        0        0     1525 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Fallback - Logged In - no.json
+-rw-rw-rw-   0        0        0    10929 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Fallback - Logged In - no_usersays_en.json
+-rw-rw-rw-   0        0        0     1074 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Fallback - Logged In - yes.json
+-rw-rw-rw-   0        0        0    10255 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Fallback - Logged In - yes_usersays_en.json
+-rw-rw-rw-   0        0        0     1164 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Log In - Remember Name.json
+-rw-rw-rw-   0        0        0      239 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Log In - Remember Name_usersays_en.json
+-rw-rw-rw-   0        0        0     2186 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Log In - Results - Password - Correct.json
+-rw-rw-rw-   0        0        0      613 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Log In - Results - Password - Correct_usersays_en.json
+-rw-rw-rw-   0        0        0     1177 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback - fallback.json
+-rw-rw-rw-   0        0        0     1238 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback.json
+-rw-rw-rw-   0        0        0     1197 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Log In - Results - Password - fallback.json
+-rw-rw-rw-   0        0        0     2257 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Log In - Results - Password.json
+-rw-rw-rw-   0        0        0      752 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Log In - Results - Password_usersays_en.json
+-rw-rw-rw-   0        0        0      249 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Log In - Sentiment (Awesome)_usersays_en.json
+-rw-rw-rw-   0        0        0      252 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Log In - Sentiment (Doing Fine)_usersays_en.json
+-rw-rw-rw-   0        0        0      264 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Log In - Sentiment (It's been a rough week)_usersays_en.json
+-rw-rw-rw-   0        0        0      261 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Log In - Sentiment (Still Hanging There)_usersays_en.json
+-rw-rw-rw-   0        0        0     1665 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Log In.json
+-rw-rw-rw-   0        0        0      597 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Log In_usersays_en.json
+-rw-rw-rw-   0        0        0     1741 2023-05-17 19:35:50.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Menu - Main.json
+-rw-rw-rw-   0        0        0     2454 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Menu - Main_usersays_en.json
+-rw-rw-rw-   0        0        0     1079 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Thankyou.json
+-rw-rw-rw-   0        0        0     1496 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Thankyou_usersays_en.json
+-rw-rw-rw-   0        0        0      891 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Upvote.json
+-rw-rw-rw-   0        0        0      241 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Upvote_usersays_en.json
+drwxrwxrwx   0        0        0        0 2023-06-26 06:35:50.569800 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/
+-rw-rw-rw-   0        0        0     1062 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Default Fallback Intent.json
+-rw-rw-rw-   0        0        0     1096 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Default Welcome Intent - fallback.json
+-rw-rw-rw-   0        0        0     3158 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Default Welcome Intent.json
+-rw-rw-rw-   0        0        0      244 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Default Welcome Intent_usersays_en.json
+-rw-rw-rw-   0        0        0     1131 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Downvote.json
+-rw-rw-rw-   0        0        0      982 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Downvote_usersays_en.json
+-rw-rw-rw-   0        0        0     3785 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Email Enquiry.json
+-rw-rw-rw-   0        0        0     2453 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Email Enquiry_usersays_en.json
+-rw-rw-rw-   0        0        0     1518 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Exit Conversation.json
+-rw-rw-rw-   0        0        0     2173 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Exit Conversation_usersays_en.json
+-rw-rw-rw-   0        0        0      682 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Fallback - Logged In - fallback.json
+-rw-rw-rw-   0        0        0     1525 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Fallback - Logged In - no.json
+-rw-rw-rw-   0        0        0    10929 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Fallback - Logged In - no_usersays_en.json
+-rw-rw-rw-   0        0        0     1074 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Fallback - Logged In - yes.json
+-rw-rw-rw-   0        0        0    10255 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Fallback - Logged In - yes_usersays_en.json
+-rw-rw-rw-   0        0        0     1164 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Log In - Remember Name.json
+-rw-rw-rw-   0        0        0      239 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Log In - Remember Name_usersays_en.json
+-rw-rw-rw-   0        0        0     2186 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct.json
+-rw-rw-rw-   0        0        0      613 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct_usersays_en.json
+-rw-rw-rw-   0        0        0     2219 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Log In - Results - Password - Template.json
+-rw-rw-rw-   0        0        0     1177 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback - fallback.json
+-rw-rw-rw-   0        0        0     1238 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback.json
+-rw-rw-rw-   0        0        0     1197 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback.json
+-rw-rw-rw-   0        0        0      752 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Log In - Results - Password_usersays_en.json
+-rw-rw-rw-   0        0        0      249 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Log In - Sentiment (Awesome)_usersays_en.json
+-rw-rw-rw-   0        0        0      252 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Log In - Sentiment (Doing Fine)_usersays_en.json
+-rw-rw-rw-   0        0        0      264 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Log In - Sentiment (It's been a rough week)_usersays_en.json
+-rw-rw-rw-   0        0        0      261 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Log In - Sentiment (Still Hanging There)_usersays_en.json
+-rw-rw-rw-   0        0        0     1665 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Log In.json
+-rw-rw-rw-   0        0        0      597 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Log In_usersays_en.json
+-rw-rw-rw-   0        0        0     2076 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Menu - Main.json
+-rw-rw-rw-   0        0        0     2454 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Menu - Main_usersays_en.json
+-rw-rw-rw-   0        0        0     1079 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Thankyou.json
+-rw-rw-rw-   0        0        0     1496 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Thankyou_usersays_en.json
+-rw-rw-rw-   0        0        0      891 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Upvote.json
+-rw-rw-rw-   0        0        0      241 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Upvote_usersays_en.json
+drwxrwxrwx   0        0        0        0 2023-06-26 06:35:50.573791 TPE_Bot-0.5.25/buildABot/Data/Default - Worksheets/
+-rw-rw-rw-   0        0        0      249 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Worksheets/Log In - Sentiment (Awesome)_usersays_en.json
+-rw-rw-rw-   0        0        0      252 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Worksheets/Log In - Sentiment (Doing Fine)_usersays_en.json
+-rw-rw-rw-   0        0        0      264 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Worksheets/Log In - Sentiment (It's been a rough week)_usersays_en.json
+-rw-rw-rw-   0        0        0      261 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Default - Worksheets/Log In - Sentiment (Still Hanging There)_usersays_en.json
+drwxrwxrwx   0        0        0        0 2023-06-26 06:35:50.574789 TPE_Bot-0.5.25/buildABot/Data/Entities/
+-rw-rw-rw-   0        0        0      208 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Entities/LoginID.json
+drwxrwxrwx   0        0        0        0 2023-06-26 06:35:50.577780 TPE_Bot-0.5.25/buildABot/Data/WebApp/
+-rw-rw-rw-   0        0        0    26827 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/WebApp/index_template_LEARN.html
+-rw-rw-rw-   0        0        0    21879 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/WebApp/index_template_RECO.html
+-rw-rw-rw-   0        0        0   817197 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/WebApp/reset_template_RECO.js
+drwxrwxrwx   0        0        0        0 2023-06-26 06:35:50.581769 TPE_Bot-0.5.25/buildABot/Data/Webhook/
+-rw-rw-rw-   0        0        0     2162 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Webhook/CheckPwd_Template_RECO.js
+-rw-rw-rw-   0        0        0     4597 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Webhook/RecommendedMenu_Template_RECO.js
+-rw-rw-rw-   0        0        0     7331 2023-05-17 19:11:48.000000 TPE_Bot-0.5.25/buildABot/Data/Webhook/index_template_LEARN.js
+-rw-rw-rw-   0        0        0    10693 2023-05-12 06:25:07.000000 TPE_Bot-0.5.25/buildABot/Data/Webhook/index_template_RECO.js
+-rw-rw-rw-   0        0        0       89 2023-05-15 04:03:04.000000 TPE_Bot-0.5.25/buildABot/Data/__init__.py
+-rw-rw-rw-   0        0        0    15847 2023-05-17 19:55:48.000000 TPE_Bot-0.5.25/buildABot/Entities.py
+-rw-rw-rw-   0        0        0    12267 2023-05-17 19:55:48.000000 TPE_Bot-0.5.25/buildABot/FallbackSocialTag.py
+-rw-rw-rw-   0        0        0    12103 2023-05-17 19:55:48.000000 TPE_Bot-0.5.25/buildABot/Firebase_Learn.py
+-rw-rw-rw-   0        0        0    14611 2023-06-26 06:35:04.000000 TPE_Bot-0.5.25/buildABot/Firebase_Reco.py
+-rw-rw-rw-   0        0        0    36243 2023-05-17 19:55:48.000000 TPE_Bot-0.5.25/buildABot/Intents.py
+-rw-rw-rw-   0        0        0    42387 2023-05-18 07:15:14.000000 TPE_Bot-0.5.25/buildABot/LearnMenu.py
+-rw-rw-rw-   0        0        0    79895 2023-05-18 10:21:25.000000 TPE_Bot-0.5.25/buildABot/Manager.py
+-rw-rw-rw-   0        0        0    15947 2023-05-17 19:55:48.000000 TPE_Bot-0.5.25/buildABot/Paraphraser.py
+-rw-rw-rw-   0        0        0     6151 2023-05-17 19:55:48.000000 TPE_Bot-0.5.25/buildABot/Password.py
+-rw-rw-rw-   0        0        0    44723 2023-05-17 19:55:48.000000 TPE_Bot-0.5.25/buildABot/RecommendedMenu.py
+-rw-rw-rw-   0        0        0     8791 2023-05-17 19:55:48.000000 TPE_Bot-0.5.25/buildABot/TelegramLogs.py
+-rw-rw-rw-   0        0        0     7539 2023-05-17 19:55:48.000000 TPE_Bot-0.5.25/buildABot/WebApp_Learn.py
+-rw-rw-rw-   0        0        0    11283 2023-05-17 19:55:48.000000 TPE_Bot-0.5.25/buildABot/WebApp_Reco.py
+-rw-rw-rw-   0        0        0     9259 2023-05-17 19:55:48.000000 TPE_Bot-0.5.25/buildABot/Webhook_Learn.py
+-rw-rw-rw-   0        0        0    33791 2023-05-18 09:37:37.000000 TPE_Bot-0.5.25/buildABot/Webhook_Reco.py
+-rw-rw-rw-   0        0        0    23915 2023-05-16 14:52:33.000000 TPE_Bot-0.5.25/buildABot/Worksheets.py
+-rw-rw-rw-   0        0        0    23811 2023-05-18 10:10:18.000000 TPE_Bot-0.5.25/buildABot/Worksheets_Learn.py
+-rw-rw-rw-   0        0        0    23923 2023-05-18 10:10:18.000000 TPE_Bot-0.5.25/buildABot/Worksheets_Reco.py
+-rw-rw-rw-   0        0        0     5075 2023-05-17 19:55:48.000000 TPE_Bot-0.5.25/buildABot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 06:35:50.582767 TPE_Bot-0.5.25/buildABot/pytransform/
+-rw-rw-rw-   0        0        0    13587 2023-03-23 18:24:51.000000 TPE_Bot-0.5.25/buildABot/pytransform/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 06:35:50.586787 TPE_Bot-0.5.25/parrot/
+-rw-rw-rw-   0        0        0     1219 2023-05-16 14:54:08.000000 TPE_Bot-0.5.25/parrot/__init__.py
+-rw-rw-rw-   0        0        0     3643 2023-05-16 14:54:08.000000 TPE_Bot-0.5.25/parrot/demo.py
+-rw-rw-rw-   0        0        0    25523 2023-05-16 14:54:08.000000 TPE_Bot-0.5.25/parrot/filters.py
+-rw-rw-rw-   0        0        0    16591 2023-05-16 14:54:08.000000 TPE_Bot-0.5.25/parrot/parrot.py
+drwxrwxrwx   0        0        0        0 2023-06-26 06:35:50.587783 TPE_Bot-0.5.25/parrot/pytransform/
+-rw-rw-rw-   0        0        0    13587 2023-03-23 18:24:51.000000 TPE_Bot-0.5.25/parrot/pytransform/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 06:35:50.588781 TPE_Bot-0.5.25/pytransform/
+-rw-rw-rw-   0        0        0    13587 2023-03-23 18:24:51.000000 TPE_Bot-0.5.25/pytransform/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-26 06:35:50.589748 TPE_Bot-0.5.25/setup.cfg
+-rw-rw-rw-   0        0        0      575 2023-06-26 06:35:34.000000 TPE_Bot-0.5.25/setup.py
```

### Comparing `TPE_Bot-0.5.24/README.md` & `TPE_Bot-0.5.25/README.md`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/TPE_Bot.egg-info/SOURCES.txt` & `TPE_Bot-0.5.25/TPE_Bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Analytics.py` & `TPE_Bot-0.5.25/buildABot/Analytics.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Default Fallback Intent.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Default Fallback Intent.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Default Welcome Intent - fallback.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Default Welcome Intent - fallback.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Default Welcome Intent.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Default Welcome Intent.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Downvote.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Downvote.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Downvote_usersays_en.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Downvote_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Email Enquiry.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Email Enquiry.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Email Enquiry_usersays_en.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Email Enquiry_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Exit Conversation.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Exit Conversation.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Exit Conversation_usersays_en.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Exit Conversation_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Fallback - Logged In - fallback.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Fallback - Logged In - fallback.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Fallback - Logged In - no.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Fallback - Logged In - no.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Fallback - Logged In - no_usersays_en.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Fallback - Logged In - no_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Fallback - Logged In - yes.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Fallback - Logged In - yes.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Fallback - Logged In - yes_usersays_en.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Fallback - Logged In - yes_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Remember Name.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Log In - Remember Name.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password - Correct.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Log In - Results - Password - Correct.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password - Correct_usersays_en.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Log In - Results - Password - Correct_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback - fallback.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback - fallback.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password - fallback.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Log In - Results - Password - fallback.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Log In - Results - Password.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password_usersays_en.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Log In - Results - Password_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Log In.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In_usersays_en.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Log In_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Menu - Main.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Menu - Main.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Menu - Main_usersays_en.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Menu - Main_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Thankyou.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Thankyou.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Thankyou_usersays_en.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Thankyou_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Upvote.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Learn/Upvote.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Default Fallback Intent.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Default Fallback Intent.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Default Welcome Intent - fallback.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Default Welcome Intent - fallback.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Default Welcome Intent.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Default Welcome Intent.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Downvote.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Downvote.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Downvote_usersays_en.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Downvote_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Email Enquiry.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Email Enquiry.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Email Enquiry_usersays_en.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Email Enquiry_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Exit Conversation.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Exit Conversation.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Exit Conversation_usersays_en.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Exit Conversation_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Fallback - Logged In - fallback.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Fallback - Logged In - fallback.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Fallback - Logged In - no.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Fallback - Logged In - no.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Fallback - Logged In - no_usersays_en.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Fallback - Logged In - no_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Fallback - Logged In - yes.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Fallback - Logged In - yes.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Fallback - Logged In - yes_usersays_en.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Fallback - Logged In - yes_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Remember Name.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Log In - Remember Name.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct_usersays_en.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password - Template.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Log In - Results - Password - Template.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback - fallback.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback - fallback.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password_usersays_en.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Log In - Results - Password_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Log In.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In_usersays_en.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Log In_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Menu - Main.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Menu - Main.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Menu - Main_usersays_en.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Menu - Main_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Thankyou.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Thankyou.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Thankyou_usersays_en.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Thankyou_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Upvote.json` & `TPE_Bot-0.5.25/buildABot/Data/Default - Recommended/Upvote.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/WebApp/index_template_LEARN.html` & `TPE_Bot-0.5.25/buildABot/Data/WebApp/index_template_LEARN.html`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/WebApp/index_template_RECO.html` & `TPE_Bot-0.5.25/buildABot/Data/WebApp/index_template_RECO.html`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/WebApp/reset_template_RECO.js` & `TPE_Bot-0.5.25/buildABot/Data/WebApp/reset_template_RECO.js`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Webhook/CheckPwd_Template_RECO.js` & `TPE_Bot-0.5.25/buildABot/Data/Webhook/CheckPwd_Template_RECO.js`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Webhook/RecommendedMenu_Template_RECO.js` & `TPE_Bot-0.5.25/buildABot/Data/Webhook/RecommendedMenu_Template_RECO.js`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Webhook/index_template_LEARN.js` & `TPE_Bot-0.5.25/buildABot/Data/Webhook/index_template_LEARN.js`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Data/Webhook/index_template_RECO.js` & `TPE_Bot-0.5.25/buildABot/Data/Webhook/index_template_RECO.js`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Entities.py` & `TPE_Bot-0.5.25/buildABot/Entities.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/FallbackSocialTag.py` & `TPE_Bot-0.5.25/buildABot/FallbackSocialTag.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Firebase_Learn.py` & `TPE_Bot-0.5.25/buildABot/Firebase_Learn.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Firebase_Reco.py` & `TPE_Bot-0.5.25/buildABot/Firebase_Reco.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,3 +1,3 @@
 from pytransform import pyarmor_runtime
 pyarmor_runtime()
-__pyarmor__(__name__, __file__, b'\x50\x59\x41\x52\x4d\x4f\x52\x00\x00\x03\x09\x00\x61\x0d\x0d\x0a\x09\x34\xe0\x02\x00\x00\x00\x00\x01\x00\x00\x00\x40\x00\x00\x00\xe1\x0d\x00\x00\x00\x00\x00\x18\xd2\xa3\x73\x27\x0c\x75\x7b\x8f\xf3\x6a\x28\x46\x00\x19\x39\x8d\x00\x00\x00\x00\x00\x00\x00\x00\xb1\xda\x15\x0a\x62\x2b\xa0\x0a\xb9\x8e\xd0\x87\x09\x28\x25\x55\x7d\xdf\x7f\xd3\xb3\x0a\x3d\xa1\x33\x58\xcc\x8a\xf2\xd1\xe8\x60\x99\x0d\xd4\x7d\x25\x2f\x1c\xc5\xef\xd1\x3c\xac\x43\x4b\x90\x02\x9c\x1c\x31\x18\x09\x09\x5e\x09\x43\x9e\xfc\xc3\xd6\xc1\x4a\x5a\x50\xb8\xae\xc9\xca\xca\xb5\xb8\x5f\x47\x92\x1a\xdc\xe6\x81\xd6\x57\x3d\xb3\x7e\x07\x47\xfa\x5c\x9d\x5a\x78\xdc\xc6\xc8\xb4\xbe\xd3\xe8\x66\xd1\xeb\xe4\xd9\x46\x4c\xe0\x11\xc1\x84\xfb\x1f\xad\x23\x62\x4e\xc9\x42\xab\x4a\x28\x73\x6b\xee\x91\xc0\xb1\xea\xf3\x2d\xe0\x16\xad\x21\x73\x3b\xff\x2f\x1f\x79\x85\xac\x31\xa2\xe1\x3b\xf6\xca\xca\x4d\x16\xe6\xf4\x2d\xcf\x1b\xe0\x62\xc0\x4e\x9f\x2a\x95\x56\x22\x51\x72\xd0\x13\xb7\xf2\xa4\xab\x12\x89\x05\x3c\xdf\xb3\x5c\x1a\x2e\x47\x48\xeb\x0c\x4c\x68\xc0\xd1\x60\x51\x7a\xf0\xbd\x6a\x06\xd7\xff\xc9\xf2\xe6\xca\x9c\xb7\x42\xc8\x76\xb8\xf2\xd0\x84\x3a\xd1\x76\xf5\xf0\x72\xf9\xe0\x56\x24\xf8\x68\x44\x28\xba\x82\x34\x72\x49\xea\x51\x5e\x3d\x9b\x94\xe3\xea\x7a\x85\x8a\x47\x95\x36\x96\xa5\xe3\xbc\x9a\xdd\x84\x21\x11\x03\x06\x53\xc7\x43\x7a\x15\xa7\xc4\x9d\x1b\x84\x61\x14\xf1\xc2\xfc\x4b\x59\x71\xcf\xa6\x66\xbc\x3c\x51\x4c\xb2\xad\x22\xd4\xc4\xe8\x4e\x19\xca\x28\x8c\xdd\x67\xf1\x8b\xe6\x8b\xc7\xf6\x5b\x6b\x65\x11\x1d\xb6\x44\x50\x90\xfd\x6e\x6d\x95\xd6\xfd\xbf\x34\xcb\x39\xf6\xd5\x1f\x3f\xbc\xc7\x99\x93\xa1\xf4\x84\x3a\x74\xf4\x71\xf2\x77\x6c\x62\xd6\x04\xb6\x19\xab\xd4\x0e\x4b\xb1\x9f\x77\x55\x10\x36\x16\xee\x02\xc1\x95\x05\xea\xcb\xdc\xe3\x0a\xc1\x61\x3e\x97\x66\x82\x79\x1a\x3a\x95\x4b\x08\x71\x64\xd8\x7b\xbf\x3d\x31\xf8\xce\xa3\x3e\x34\x3c\x4b\xd8\x3b\x18\x00\x22\x1b\xba\x7e\x11\x04\x47\xf3\xb0\xb7\xfe\xef\xc1\x4c\x8d\x65\x09\x59\xbc\xe1\x63\xbd\xe0\x14\x13\xa3\x8e\x92\x42\xf9\xf7\x55\xa3\xad\x94\xd8\xbd\x1a\x98\xbd\xf9\xe1\xa6\xc7\x01\x71\x92\x0f\xfd\xcb\x25\x6e\xec\x7d\x87\xa8\x1c\x86\xae\x1b\x42\xe6\xc4\x02\x66\xa8\x17\x9f\x88\x07\x11\x8a\x11\xad\x98\x12\x0b\x7d\xde\x2c\x1b\x2d\x33\x93\x73\xe8\x4f\xcd\xbe\xb0\x54\x6e\x87\x55\x03\x04\x79\xd9\x04\x74\xbb\x85\x6f\xdb\x23\x58\x33\xf0\xe2\x64\x11\x1d\x3a\x11\x67\xe1\xdb\xe6\x03\x5d\xc2\xae\xa1\xb2\x02\x6f\xd0\xe1\xd4\x4b\x63\xbc\x42\xa9\x81\xb6\x77\x05\xce\xa5\x3b\x54\xf0\x77\x1d\xd5\x0c\x41\x79\xc0\xe9\xd5\xe7\x3d\xbe\xda\xd7\x04\x75\x98\x7c\x42\x39\x09\x1f\x8b\x7a\x23\xae\xc1\x1e\x0c\xe2\xc6\xcd\xd4\x9f\xf4\xe5\xac\xcf\x77\xd2\xce\xb0\x51\x8d\x06\x9c\x42\xa2\x79\xe6\xd9\x75\xb9\x88\x4c\xe0\xec\x07\xc6\x94\xb3\x18\xf9\x15\x91\x6f\x2d\x53\xbd\x99\x5c\x1d\xfd\x7a\x89\xbf\xb6\x82\x43\x42\x0c\x3a\xd8\x8b\x43\x96\x72\xf2\xab\xed\x67\x79\x9b\x5c\x2b\x81\x82\x8d\xad\xf0\xea\x17\x34\x70\x16\xc8\xe4\x3f\xe6\x66\xc7\x11\x99\x4b\x53\xa2\x01\x04\xbd\x4e\x36\x97\x22\x7d\x6e\xfb\xd3\x28\xeb\x4e\xd6\x57\x21\x26\x77\x7c\x10\x97\x83\x1a\x75\x21\x04\xb1\x63\xfc\xd1\x51\x12\xf3\x3d\xbf\xf2\x8d\x02\x78\xef\xad\x31\x1d\x9f\x3b\x52\x23\xaa\x65\x9e\x43\xf3\x42\xe4\x43\x27\xf2\x82\x84\xd4\x68\xbe\x91\x42\x6d\xc4\x3d\x49\xf9\xfc\xed\xd6\x23\x1e\xe8\x8f\x42\xd9\x75\x57\xa5\x15\x0a\x63\x4e\x87\xd6\xb0\x75\x8d\xf3\xc3\xe9\x22\xfc\x63\x8b\xb9\xcd\xbe\x79\x47\xd3\x76\x62\xa1\xbf\x7e\x64\x49\xaf\x67\x18\x67\xc1\xbe\xb8\x6b\x61\xb6\x20\x5c\x1c\x2e\x3b\xb5\x38\x0f\x51\x12\x1a\x4b\x01\xa8\x54\x32\x83\xfb\x70\x30\xa7\x07\xe5\x94\x89\x79\x56\x08\xf8\x04\xfa\xe5\xa5\x7e\x3e\xc5\xe4\x27\xe2\xc9\x26\x7f\x20\xfe\x82\x52\x84\x17\xd5\x81\x0d\xf4\x66\x22\x3f\x50\xde\xde\xfd\x96\x0c\xd3\x18\x3f\x6d\x73\x1f\xbc\x80\x0f\x2e\x98\x03\x62\x1a\xc7\xdd\x5a\x09\xd9\x5e\x9b\xcb\xda\xc4\x6e\x0d\x6c\x13\x16\x22\xac\x91\xd9\xe1\x84\xcf\xef\x26\x1a\x63\x68\xa4\xa1\x2a\xb0\xcd\x5b\x4c\xbd\x57\xca\xe0\x3a\x7e\xdf\x21\xe4\x10\xdf\x12\x38\x44\x11\xf0\x20\xff\x16\x40\xcc\xc8\x46\x50\xe5\x5e\x3b\x4f\x40\x83\x36\x68\xe5\x08\x95\x52\xa1\x0e\x87\x8c\x89\x7e\x3d\xb4\xe9\x21\x9d\x58\xd0\xf8\xab\xfa\x47\x63\xa3\x80\x91\x38\xa9\x4e\xe1\x88\xfa\x6f\xe1\x7d\xd7\xf1\xbd\xc7\x85\x5a\x89\xc9\xe2\x09\x69\x05\xb5\x99\xc1\xa9\x58\xf0\x27\x8c\x30\x42\x6f\x86\x6a\x9f\x34\x9f\xe3\xd3\x2c\x13\xe6\x88\x36\xac\x70\x88\x9a\x45\xc4\xaa\x61\xa7\xf3\x06\xef\xb2\x8d\x34\x30\x3c\xd4\xbc\xc4\x77\xa6\x2e\xdf\x30\x86\x40\x41\x4f\x76\x32\xe6\x0f\xd8\xfa\x4b\x3e\x4e\x3c\x59\x5b\x4f\x82\xce\x70\xe5\xf3\x9c\x58\xc5\x51\x5b\x5b\xd7\x57\x46\x53\xae\xd5\xcc\x09\xd4\x16\x78\x66\xc8\xb1\xf0\x61\x08\x00\xe0\xd3\xfd\xa7\xac\x3c\xd6\x14\x2f\xcc\x74\x29\xf7\xbd\x19\x7e\x78\x14\xf3\x8d\xd5\xdb\x39\x0d\xfa\x4b\x4d\x68\x46\xcd\x87\xe8\xe3\xed\x3a\x50\x58\x18\x21\x97\x2b\xc3\x8a\x14\xc7\xae\x12\x27\x87\xd4\x2c\xb2\x99\xb1\xf8\xe8\x50\x3f\xc5\x84\x75\x6c\x4a\x30\x8a\x78\x49\x66\x41\x28\x7a\x5d\xc7\x0a\x98\xc8\x7d\x65\x22\xac\xe0\x2d\x1b\xed\x43\x77\xe7\x2a\x03\x53\x0a\x49\x2a\xe2\x17\x60\xdd\xcf\x87\xee\x96\x87\x04\x67\x2c\xf4\x8a\x72\x7d\xac\x0e\x0f\x66\xf2\x32\x61\xf4\x36\xd1\xb5\xb2\xf5\x8c\x1f\x53\x20\xca\x89\x9f\xbf\xdf\x62\x99\xa9\xee\x17\x58\xe6\xe9\xed\x54\x53\x66\xef\xdf\x2d\x53\x9a\xc8\x51\x6e\x69\x70\xd7\x06\xe6\x7a\xfa\xf2\x44\xc5\xb6\x5d\x63\xef\x0a\x67\xef\x24\x06\x17\x97\xff\x07\x8e\xfb\x8d\xef\xde\xfb\xe9\x10\x5a\x42\x4e\x7a\xf4\x67\xc7\xaf\x6c\x6a\xd8\xc6\x17\x44\x59\xac\x3c\xcc\x86\x72\x63\xa5\xf3\x3d\x0d\x11\x06\x0d\x77\x66\x0a\x9d\x02\x7d\x4c\xf1\x0a\x74\xc8\x2d\x39\x0d\x42\x63\x64\x8b\x30\x9e\x4a\xab\xa1\x79\x56\x77\x1b\x7b\x28\x48\xfc\xe4\xae\x54\x3a\x94\x5f\x4e\xb3\x54\x7a\x32\x3d\xb1\x0b\x83\x8a\x03\xa5\x4a\x41\xc0\xd0\x25\xec\x0e\xb4\x02\x7f\x93\xf2\xf1\xf9\x02\xee\x2b\x3b\x0c\x3f\x24\xad\x18\xf4\x5c\x2f\xee\x7a\x70\x53\x3a\x90\xfd\x59\x0c\xc2\x5e\x4c\xc3\xac\xbf\xc5\x14\xa1\x7b\xc9\x79\xd0\xd6\x0d\x44\xeb\x63\xa4\x42\x3d\x4f\x06\x72\x85\x7c\x02\xa3\x2d\x71\x61\x8b\xd7\xca\x21\x8f\x66\x57\x39\xdc\xf4\xe6\x52\xe9\xa3\xac\x9b\x1a\xa5\x45\xd7\x45\xd3\x69\x37\x32\x05\x21\x63\x60\x71\x64\x54\xe3\x93\xb3\x0d\x03\xd6\xa6\xd1\xf0\x09\x36\x0b\x40\x1c\x36\x67\x52\x93\x37\x37\xe8\xf1\x86\xec\x72\x8e\xdc\x23\x93\xc1\x01\x11\x75\x24\x37\xe7\xe3\x16\x2e\x84\xf5\x6a\x54\xf8\xae\x32\xdf\x3b\x9e\xae\xa7\x0e\x73\x54\xe1\xa9\x13\x69\xc0\x03\x43\xd1\xb7\x9a\x27\x93\x34\x82\xbc\x74\x40\xe1\x92\xaf\x40\xcf\xc3\xfe\x22\xba\x30\x4b\x25\xee\x88\xef\xdd\x8b\x3f\x59\x3e\x0a\xaa\xab\xe3\x65\x27\xd9\x22\xae\x43\xb1\x91\x37\xea\x25\x84\x82\x3c\x06\x1f\x82\xd3\xb5\xee\xe6\xc9\x40\xd0\xa0\xde\x4d\xc4\xa1\x65\x83\x13\xc2\x9e\xeb\x4f\xb2\x93\xff\x87\x15\x81\x15\x5b\x2a\x02\xd5\x59\x50\xfd\x83\xc5\x13\x90\x7a\xfa\xc4\x92\x5f\xc5\x52\x07\x98\x17\x22\x2f\xfc\x4a\x33\x40\x21\x95\x5d\x63\x86\xc3\x9f\x86\xd8\x98\xd1\xb8\xd6\x1e\x00\xed\xe0\x46\xbc\xb6\xf8\x2f\xca\xcb\xa3\x2d\xf1\xc0\x2e\x5e\x5c\x0d\x0c\xa7\xab\x42\x34\x55\x39\xa2\xd2\x7b\x6a\x82\x3a\x98\x19\x61\x7b\x68\xa7\xbf\x97\x6d\x13\x6e\x8f\x7f\xd0\x5c\x28\x40\xd0\x90\x97\x4b\xfd\xeb\xe1\x5f\x47\x86\xae\xb7\x5b\xb4\x66\x9a\x1d\x4e\x3a\x53\xc1\x66\x17\xdf\x67\xd4\xa1\x53\x0c\xc5\xa5\x42\x23\x4c\xfd\x05\x5b\x61\xab\x4f\x8b\x8d\x01\x73\x77\x4e\x9f\x21\x5d\xc2\xbf\x2f\x51\xbe\xcf\xd5\xce\x2f\xab\x2b\xa4\x2f\x1a\xc2\x10\x03\x49\x23\xc4\x1e\x8e\x34\x83\xe6\x05\x1c\xc9\xf7\x5f\x5f\xbd\x33\x3e\x92\x13\xf3\x8c\x4c\x57\x36\xd7\x6b\x47\x16\x63\x95\xcb\x93\x64\x55\x1f\x08\x4a\x36\x0a\x4b\xcb\xd3\x11\x2f\x32\x6a\xab\x60\x80\xd9\x01\x19\xd2\x95\xb3\x32\x88\x44\x3e\x16\xe0\xd3\x3b\xb6\x5b\xc5\x27\xe8\x78\x5c\xf3\x0e\x30\x25\x2e\xf1\x10\x6e\xf7\x17\x0f\x0a\x17\x96\xc0\xc5\xb3\x5c\x94\x2e\xf3\xea\xd0\x28\x72\xf0\x9b\xae\x84\xd3\x92\xb6\x0c\xce\x42\x28\x52\x13\xb2\x1c\xb0\xfd\xb4\xed\x5b\xc9\x30\x58\xce\xe0\xee\xb8\x13\x10\x06\x0c\x06\x48\x98\x6b\xa9\x4f\x55\x76\x2b\x12\xe3\x00\x42\x88\x77\xd1\x5a\xe9\x84\x76\xce\x47\x94\x8b\x4d\x33\x83\x80\x33\xd8\x48\x31\x2e\xae\xd6\x08\x00\x44\xed\x25\xa4\xff\xea\x2d\xd9\x90\x56\x77\x76\xb7\x3c\x6e\x2b\x75\xe3\xdf\x96\xd9\x38\xc1\xab\x47\x78\x23\x73\xb2\x15\x31\xa9\xa4\x39\x3e\x9e\x8a\x7c\x81\x4e\x46\x83\x6b\x3b\xbb\x27\x7c\x3b\x22\xb8\x4c\xf8\x2c\x1f\xbc\xec\x1c\x57\x26\xaf\xca\xcd\xe5\x95\x40\xa9\xe9\xe3\xf4\xe3\xdd\xe0\x9e\x52\x22\xb7\xa0\xcf\x52\x78\x7f\x3f\x90\x35\xa3\x3a\x6f\x5b\x41\x20\x61\x3d\x0d\x13\x9b\xa2\x0a\xb3\xb9\xfc\x2b\xbe\xdc\xae\x2c\xc5\x44\x25\x0f\x13\xb0\x71\xd1\x61\xaa\x00\xed\xbe\xf0\x36\xa2\x14\x44\xb6\x8e\xf7\x3f\xfa\x26\x1a\xe0\x0b\x44\xbf\x97\x8c\x85\x8d\x9a\x73\x1a\x0b\xcc\x77\x60\x79\x41\x8c\x95\xc5\x39\x77\x60\x64\x62\xe7\x02\x57\x3f\x24\x32\x0c\x3f\xe4\xb7\x7c\xc7\x5e\x03\xfd\x89\x70\xb3\xe5\x3e\xf8\x97\x23\x80\x6f\x5a\x1b\x5c\x1d\xcb\x31\x2a\x6d\x4a\x11\x31\x7d\x6c\xe2\x97\xbf\x42\x22\xd6\x6f\x35\x09\x43\x5f\xd3\x6c\x01\x1c\x75\xd9\xc3\xfb\x1c\xa7\xfb\x92\x9a\xef\xf6\x51\x9e\x1d\x82\x6e\x49\xda\xf1\x8d\x66\x33\x18\x99\x22\xc6\x77\xfd\x71\x31\x83\x5e\xa7\x1e\x74\x88\xdf\x8a\x6b\xe3\xa3\xa6\xda\x2f\x53\xce\x75\xa9\x05\x53\xa3\x86\x66\xdb\x11\x65\xec\xe2\x47\x07\xe7\x31\x93\x60\xca\xe4\x99\xb4\x81\xad\xc3\x65\x54\xec\xc0\xe2\xfa\xf4\xc6\xce\xe1\xd9\x6c\xba\x66\x9f\xa5\x13\x2d\x1e\x57\x85\x3a\xb9\x82\x28\x92\xe2\x3d\xc4\x2c\xb1\x4a\x52\x53\x2c\x0e\xe2\xdd\x8b\x5e\xec\x68\x8b\x48\xea\xb5\xe3\x09\xbb\x23\x9d\x63\xc6\xe8\x2e\xa9\xd0\xd2\xc8\x9a\xd1\x42\x8b\xd9\x50\x05\x8b\x35\x57\x39\x0d\xa3\x92\x67\x97\x46\x55\x88\x81\x9c\x5a\x5c\x0c\xc6\xa6\xce\x78\x3a\x72\xec\x6a\x07\x90\xe8\x96\x0f\x79\xa2\x5c\x24\xc4\xc6\x5d\xab\x85\x40\x08\xad\xe8\x1b\x16\xa1\xd7\x87\xb0\x58\xf4\x01\x8f\x06\x20\x16\xda\xfb\x67\x21\xd0\x65\x3c\x05\x88\x4a\x1f\x46\xb2\x78\x59\x8b\x80\x0f\x4d\x46\xbd\x08\xb8\x1e\x4a\x35\x8b\x04\x3d\x43\x6b\x60\xc5\x32\x26\xcf\x2b\xb3\xcc\xb1\xa6\x47\xa3\x5d\xdc\x55\x97\x00\xe2\x25\x98\x33\xfe\x7c\x6e\x9e\xbb\xb2\x49\x1d\xfc\x0c\x2a\x87\x17\xa3\x57\x1a\x04\x38\x31\x89\x28\x70\x00\xb4\xca\x9d\x99\xda\x89\x15\x93\xcd\xa1\xd2\xfd\x5b\xac\x92\x7e\xd6\xfc\xb0\x78\x36\x82\x08\x0f\x93\x41\x74\x9f\x32\x14\x4a\xc8\xf0\xca\x80\xd2\x57\x7f\x39\x91\x33\x59\xfa\x95\xb8\x5d\xf6\xdd\x07\x29\xd9\x52\x40\x41\xfd\x47\x78\xc5\x64\x2d\x5d\x6e\xe6\x75\x34\xe9\xca\x38\x4f\xba\xea\x1d\x1c\xb7\x2e\x21\x04\x23\x0f\x8e\xfa\x9b\x71\xef\x0f\xe8\xc9\x5c\x46\xbb\x71\xab\xbd\x99\xc7\x05\xcb\xe9\xf9\x66\x5f\x12\xe0\xc3\x87\x5b\x13\x02\x3b\x3a\x83\x99\xac\x85\x90\x94\x1f\xb1\xca\xb0\x05\x6e\xc0\xac\x71\x3d\xf7\x9a\x65\xf0\xee\xef\xed\xc0\x57\xc6\xbd\x94\x0d\xf1\x1c\xf2\x1f\x76\x37\x33\xb5\xf1\xec\xf8\x88\x88\x2a\x11\x7f\x91\x63\xb7\x22\xd4\x8a\xb8\xc7\x6c\xf0\x92\x08\xfc\x66\x5a\x93\x07\x31\x21\xc5\x85\x07\xff\xb8\x98\xb1\x34\x31\x13\x34\x50\x55\x1e\xe3\x6b\xb6\xd6\x3b\x84\xdb\xce\x50\x28\xfb\xd3\xd1\x74\x1b\x98\x52\x73\x0d\xc1\x07\x07\x51\x67\x0d\xbf\x6f\xed\xb8\x01\x8b\x78\x8c\x53\x84\x73\x5a\xa1\xec\x45\xf3\x79\xc2\x1d\x94\x16\x7c\xe0\xd6\x0a\xbd\x53\x44\xdf\x1b\xdf\x5f\x0e\xbf\x59\xae\xf5\x1d\x85\x08\x23\xc7\x30\x10\x82\x3d\x91\xe5\x02\xb8\x95\x2b\xbb\xb3\xde\x30\x9e\x61\x77\x44\xcb\x30\x92\x51\x0c\x94\x70\x71\x0f\x19\xac\x70\xc7\x05\xf7\x0f\x55\x4d\x9b\xc4\xa5\x54\x45\x5f\x81\xe7\xe5\xd0\x21\x40\xc8\x50\x78\xc9\x28\x8d\x2d\x52\x21\x1c\x12\x97\x9c\x71\x15\x83\x8c\xe7\x73\x8d\xe6\xdf\x24\x3e\xdc\x40\x49\xaf\xfa\xb2\x58\x7d\xf9\x81\x76\x21\xaa\xa5\xb3\x5c\x1d\x17\x49\x11\xb5\x9b\xba\xe3\x21\x2b\x91\x7d\x46\xa8\x59\xcb\xe2\xdf\x84\xfe\x76\x91\x1e\x1f\xba\x3b\x37\x51\x08\x67\xa0\x2b\xe2\xfa\x9e\xe7\x6b\x9a\x10\x68\x30\xe5\x04\x66\x41\x9e\x42\x07\x7c\xda\xb3\x97\x3e\xdd\xe1\xe5\xcf\x4a\x30\x7b\x4d\xa0\x7b\x92\xb1\xaa\x7a\x38\x8e\x1a\x00\x78\xb3\x74\xe1\x82\x25\xc2\xf4\xa3\x13\xb7\xa3\xab\xe7\xc9\x66\xce\x16\xc0\x71\x14\x56\x60\x11\xaf\xbd\xbc\xa9\xe5\xbf\x35\x31\xa7\x44\x49\x22\x29\xf2\xdf\xa6\x8c\x70\x36\x89\x2c\x72\xac\xee\xaa\xfd\x8c\xf0\xa4\x6c\xf6\x16\xe8\xa9\xf7\x04\xa9\x05\x21\xa9\xb7\x0c\xb7\xaa\x01\x00\x33\x1e\x37\x0c\xa1\x9a\x79\x3f\x82\x7d\x89\x01\x1e\x47\x46\x9a\xca\xed\x5b\x09\x5d\x57\x22\x8a\x15\x3d\xb9\x17\x39\xfc\x59\x1c\xda\x33\xc4\xab\xe7\x7c\x23\xef\xae\x49\xc6\xd2\x47\xb2\xd2\xa6\x91\x48\x8e\x1a\x47\x27\x77\x7c\x8c\x37\xb8\x0c\x07\x2f\xee\x2e\xaf\x5f\xaf\xac\xaf\xe4\x54\x07\xd8\xd8\x35\x54\x64\xf3\x82\x84\x3f\x00\xe1\x0b\x6e\x3a\x2c\x5f\x96\xc4\x06\x82\x04\x55\x65\x2c\x39\x60\xcf\x97\x19\x7d\x3f\x42\xd4\x34\x8d\x89\x1b\x54\x06\x4c\x1a\x73\x3a\xfc\x57\xe5\xa7\xaa\xd9\x4d\xb2\x9a\xfd\xf4\x8d\x38\xa9\x24\xdb\xcc\x12\xb4\xf3\x1e\xe9\xd8\xc9\xd0\xdb\x9a\xf8\xae\x55\x04\x74\xc2\xdb\x88\xdb\x21\xe0\x76\xa9\x7e\x2d\x55\xae\xc9\xdb\xc7\xf7\x2f\x45\x5c\x55\x3e\x43\xff\x7b\x10\x5d\x93\x41\x31\xa5\x7e\xbf\x59\xa8\xe8\xa8\x4e\x01\x50\x0b\x42\x5a\xaf\x6c\xb8\xfa\x4a\xf0\xee\x17\xff\x93\x98\x13\x6b\x34\x62\x17\x5b\x7f\x39\xc5\x41\xd1\x53\x69\x8c\xe0\x2b\xbd\xd7\xf7\x5d\x7c\xe8\xca\x1b\x38\x93\x56\x0a\x92\x91\x4a\x2b\x80\xfb\x6a\x85\xf5\x5b\x74\x3d\x88\x09\xd1\xb0\xbf\xb7\xf3\x3e\xa8\x97\x1a\x4f\x1d\x73\x64\x99\xea\x6e\x83\xb4\xe1\xe7\x3e\xcb\x77\x56\xd3\x42\x15\xc0\xa5\x9f\xf3\xd9\xb5\xdb\x24\x29\x77\xba\x41\xc1\xdb\x04\x3c\x83\x3e\x8d\x4e\x6d\x88\x03\xf9\x71\x6b\xb3\xab\x26\x82\xb5\xa7\x32\xb5\x59\x12\x69\xca\xc8\x1d\x7b\xb2\x7d\x42\xee\x84\xd1\x28\x7a\x22\xd0\x04\x31\x9c\x27\x9d\x46\x10\x82\x29\xde\xbe\xe4\xda\x23\x36\x62\x6a\x09\x16\x44\x6c\x0d\x2a\xff\x99\xb3\xc1\x84\x81\x00\xba\x88\x05\x26\x58\xb1\x45\x61\x30\xf6\x43\xd2\xb6\x67\x4b\x87\x64\x5b\xac\xc1\xc2\x01\xec\xaa\x0d\xf4\x0f\xfe\xe1\x76\x8d\x33\xa5\x73\x73\xe0\xb3\x1f\x53\x02\xd4\x96\xd3\x33\xca\x99\x2a\x4a\x44\xe0\xca\x6b\x0d\xfa\xf7\x52\x10\x16\x8e\x5b\x98\x0e\x25\x61\x5f\x5a\x4d\x3e\x14\x6d\xed\xa1\x65\x6f\x9e\x41\xd6\x73\x21\xb7\xa9\xf0\xaf\x69\x81\x8a\x91\x85\xb4\xc4\xdd\x61\x90\x76\xc4\x26\x69\x90\xb4\xf2\x29\x09\xd7\x01\x64\xe5\x1f\x34\xd6\xe0\xc9\x32\x8a\x67\x9e\xa8\xa3\x46\x3e\x25\xbc\x75\xee\x07\x18\x5b\x34\x7d\x56\x3c\x25\x34\x5f\x0d\x26\xfe\x2f\x28\x6b\x2a\x9b\x93\x8f\x19\xe2\x18\xbd\xd1\xd6\xaf\x77\xa9\x15\xcf\x7d\x3f\x63\xee\xdd\x01\x5c\x15\xc5\x2d\xc7\x74\x35\x7a\x1e\xe8\x78\xb1\x44\x4e\x05\xb2\x13\xb0\x59\x10\xb3\x84\x71\xd9\x6e\xf3\x92\x6e\x18\x54\x5b\x60\x74\xa7\xab\x6e\x44\x72\xcf\xfe\x7e\x78\x8a\xbd\x64\x20\x59\xc3\x12\xee\x28\x7b\xf4\xa2\x3a\x9e\xe4\xef\x52\x15\x0b\x79\xec\x99\x7b\x14\x76\xb9\x61\xeb\x88\xfe\x4c\xa5\xc5\xff\x95\x06\xb8\x86\x4e\x14\x97\x5b\xdf\xb8\xe8\xfe\x5e\x56\x9e\x79\x15\x8e\x0e\xc0\x40\xf9\x05\xf6\x06\x0b\x09\x94\xf0\xc6\xaf\xf4\x5a\xde\xf5\x6e\x6f\x4b\x31\x4d\x6a\x58\xef\x25\x6e\x18\x16\x8a\x8f\xc3\x75\x9e\x6e\x00\x37\x44\x9f\xb7\xfa\xe6\x93\x72\x6b\xa4\x06\x47\x2c\xb1\xb8\xc3\x9d\x93\x33\x95\xa5\x41\x24\x37\x70\x07\x8d\xb1\xfa\xaf\x12\xa6\x1a\x4c\xca\xdb\xfc\x9d\x88\x78\xf1\x3e\x51\x45\x80\x41\xb4\xfc\x14\x8f\xb4\xbc\xd6\x91\xc0\x24\x43\x6b\x92\xaa\xf7\xbb\xc2\x9c\x06\x95\x21\x2d\x93\xb2\xee\x00\x35\x6a\x68\x89\xab\x3c\x47\x2d\x90\xb6\xcd\x22\xfd\x71\x22', 2)
+__pyarmor__(__name__, __file__, b'\x50\x59\x41\x52\x4d\x4f\x52\x00\x00\x03\x09\x00\x61\x0d\x0d\x0a\x09\x34\xe0\x02\x00\x00\x00\x00\x01\x00\x00\x00\x40\x00\x00\x00\xec\x0d\x00\x00\x00\x00\x00\x18\xac\xf5\x87\xe3\x42\xa9\xd3\x8f\xb5\xb7\x19\x15\xef\x83\xfc\xc5\x00\x00\x00\x00\x00\x00\x00\x00\x33\x7e\xb9\xd4\xdd\x77\x92\x2c\x32\xf3\x75\x40\x56\xcf\x08\xc7\xc0\xba\xf7\x9e\x08\xf6\x28\xb5\x2d\x80\x15\x0f\x69\x27\x83\x78\x29\x43\x63\xfe\xc6\xff\xa6\xb1\x11\x17\x62\x64\xef\x3c\x00\xef\xee\xb9\xf5\x05\xad\x11\x8e\xf3\x47\xe4\xde\x59\xc0\xaa\xfd\x13\x8a\x7e\x8f\xc4\x6b\xe1\x83\xc4\x96\x0d\x95\x98\x8a\xbf\xf8\xff\x42\x3a\xf9\x9e\xe9\x43\x68\x7c\x64\xac\xaf\xf8\x75\x8a\xe2\x38\x55\x46\x9e\xdf\x54\x63\xab\x2b\x1f\x58\x83\xf3\x5d\x96\xd9\x0b\x82\x2c\x7d\x78\x31\x66\xd8\x3a\x22\xf2\x18\x1d\x6e\x20\x01\xd6\x88\xb8\x62\x1c\x02\xfc\x87\x38\xa2\xe4\xd4\x4e\x85\x05\x09\x00\x11\x0c\xfa\xab\x79\x1d\x20\x26\x85\x98\x24\xcc\x37\xaf\x6d\xfb\xbc\x0b\x7c\xf0\x4c\x7b\x95\xed\xc9\x18\xdb\xd3\xee\x5b\x81\x85\xf8\x5d\xaf\xe8\xe8\x09\x91\xa8\x59\xe1\x97\xbb\x28\x53\x99\x01\x77\xff\x54\xb6\xfc\x65\x6c\x8d\x89\xb5\x3d\x23\xeb\x2c\xae\x58\x3d\x0b\x68\x2c\x12\xf3\xd3\x29\x4e\xf7\xdb\xfb\x55\xbd\xc8\x3b\x41\xa1\x45\xac\x5c\x41\xfb\x7d\x89\xc2\xe5\xf2\x43\xd0\xb9\x38\x31\x86\x27\x60\x6b\xc9\x1d\xd8\xd4\x4c\x9a\x30\x9f\x7a\x88\x6f\x23\x6e\x7e\x9f\xfd\xbe\x16\x24\x13\x2a\x02\xbd\xef\xc9\x41\xa3\x7f\xf0\x46\x04\x5c\x95\xa4\x87\x01\x9e\xe7\x73\x3f\xd4\xf0\x9e\xc1\x64\x9b\xd1\xa7\xf0\x4b\x05\xce\x5b\x51\xb3\x0b\x27\x13\x48\x05\x0c\x75\xd0\x9d\x82\x26\x12\xc7\x52\x4a\x0b\x9c\x77\xbb\xfd\x90\xac\x67\xdb\x5d\x01\x22\x5d\x7c\x1c\x6c\x26\x39\xd4\x40\x3a\x39\xbd\xe2\x21\x5a\x00\x1a\x16\xf7\x24\x70\x3e\x29\x16\xcc\xdf\xa9\xdf\x6e\xfe\x74\xcc\xdf\xee\xf3\x87\xae\xcc\x29\xc5\x7c\x2e\x3a\x09\x3c\xa4\xac\x5b\xf4\x78\x2f\x7c\x91\x22\x9e\x7e\xd4\x19\xf4\x44\x35\xe0\xfd\xeb\x6c\xec\x11\x3a\x4d\x3d\x38\xd2\xdf\xc5\x36\x6f\x40\xe2\xd6\xb9\x55\xb1\xea\x7d\x99\x7f\xd8\x2e\xf3\xdf\xfd\x8a\xf9\x86\xb1\x50\xc8\x49\x98\xc2\x4e\x40\xe3\x2d\x45\xa7\x8a\x9d\xcf\xb7\x1d\xc5\x37\x02\xe5\x93\x83\xcd\x38\xdb\x78\x8a\xd1\xff\x2b\xcf\xdd\x0c\xb9\xbb\xd9\xfa\x9a\x23\x17\xdf\xd4\x8e\x04\x03\x0a\xdc\xd9\x93\xd0\x40\xf9\xd5\xf2\xdf\xba\x33\xd9\x3b\x84\xe1\x67\xd7\xae\xff\x49\x0a\xd0\x3f\x9d\x04\x46\x5a\x77\x73\x37\xb2\x83\xef\xc8\xe8\xd4\xff\xca\xfc\x43\xcc\xe1\x0d\x6d\x1e\x68\x8d\x89\x50\x25\xde\x58\x49\x13\xcb\x2f\x22\xac\x28\x4b\x9a\xa1\xe0\x5a\x43\x78\xe7\x11\xa4\xf9\x9d\x70\x40\x64\x72\xee\x70\x14\xb9\x73\x62\x83\xcc\x51\x82\xa2\x2e\xb5\xd9\x76\xf9\xd6\x02\x8b\x91\x28\x4a\x23\x1f\x32\x0c\xbb\xd6\xe1\x6d\xe7\x26\x5c\x2a\x09\x58\xae\x4b\x7a\x48\xc2\xd4\x75\x66\xf5\xe6\x7b\x67\x53\x71\x4a\x43\x4c\x73\xef\xea\x46\xac\xc4\xe3\x80\xea\x59\xd6\x55\xb2\xf6\x03\xfc\x4c\xed\x99\x56\x3b\x89\xed\x54\x12\x35\x08\x2b\x37\x6d\x31\x0f\xbe\x51\xf8\x4b\xa1\x38\x38\x40\x47\x08\x4d\xa7\xd3\x48\x9d\x09\x0b\xa7\xbc\xd7\x38\x00\xa1\x54\xbb\x1e\x49\x84\x25\xae\x05\xcd\xba\x22\x02\x6b\xe9\xe7\xc8\xa1\x0b\x84\x39\x28\x62\xf0\x43\x80\xd0\x24\x7a\x26\x78\x1a\x98\x35\xd8\x37\x0a\x99\xd5\x84\x96\x84\xe4\x5d\x31\xc3\xd8\xb2\xaa\x7b\xe4\x9b\x65\x37\xa8\xf0\x80\x5e\x15\x7c\xce\xe0\xae\xc7\x07\x03\xf0\xf4\x04\xf9\x2c\x0d\x2e\xdf\x1c\x02\xe5\x98\x22\x6c\x5c\xdb\xd5\x25\x27\x29\xa9\x4f\x9b\x74\x07\x64\x0a\x44\xc2\x19\x48\x98\x46\x75\x48\x26\xbc\x81\x8e\x9d\x23\x05\x94\x70\x12\xb5\x42\x9f\xaf\x59\x16\xc9\xb5\x09\x9a\x37\x0a\x90\x48\xf2\xfe\xc0\x71\xbf\xfd\x10\xa3\x2f\xb2\xfc\x6a\x16\x0b\xfa\xe1\xfa\xdc\x57\x0d\x49\x0d\x93\xac\xb2\xd0\x08\x60\xa5\x67\x5c\x4c\x3e\xa7\x80\x95\x5a\x66\xf9\x68\x64\x6c\x91\x40\xff\xff\x28\xab\xd2\xcf\xcb\xc6\x13\x36\x31\xd8\x37\xa5\xf8\x90\x65\xfc\xac\x55\xd4\xae\x09\x1e\x77\xdf\x1d\xad\xe5\x69\x0c\x06\xda\xb3\x25\x0e\x7f\xd6\x83\x58\x5e\x2c\x75\xdc\xf1\xb4\x89\xa3\xac\x4c\xf4\xf7\xd5\x9d\xcd\xb5\xe8\x0e\xa1\x7b\xe2\x56\x4f\x27\xe2\xa0\xe6\xcd\x48\x83\xf1\x75\x72\x9a\x54\x27\x33\x35\xf1\x19\x08\x97\x82\x7b\x87\xd4\xab\x86\xaa\x7c\x91\xbd\x7a\xb5\x49\xb5\x4d\x1b\xe2\xc2\x46\x09\x8b\x84\x7c\x69\x5a\xbf\xf8\x95\x2d\xd3\xd7\xf2\x53\x35\x33\x13\x40\x1e\x1e\x60\xa1\x3b\x80\x45\xc9\xda\xb8\x3b\xce\xd5\x8e\xbe\x39\xb9\x24\x41\x6f\x98\x5b\xf8\x4d\x3a\x6e\x55\xd6\xf2\x88\xf9\x3a\xe5\x58\x7b\x9b\x83\x78\xd5\xe5\xef\x13\x83\x6b\x2d\xbc\x7e\xd5\x00\x04\xf0\xb9\x96\x15\x85\xdc\x11\xae\x7e\xff\xae\x02\x94\x9c\x9e\x0e\x9b\xf7\x20\x83\x17\x17\x79\x11\x58\xea\xf7\x11\x6f\x62\x70\x0e\x66\x20\xe1\xe5\x7e\xe7\x1e\xf3\xfb\x30\x95\xc6\x95\x3b\x50\x7d\x3d\x12\xd9\x1e\x3a\x5b\xba\x35\x0e\x29\xad\x03\xc1\x53\xa1\xfb\xd9\x8a\xe9\x69\x30\xd0\x79\x8d\xd4\x89\x00\xc3\x6b\x00\x1c\x48\xed\x3f\xe7\x0e\xcb\x02\x53\x43\x0e\xf1\x52\xc2\x1c\x94\x9d\x08\xbd\xdb\x13\xf7\x1d\x07\x8e\x99\x02\x63\x83\x70\xfe\x93\xc6\xb3\x02\xc0\xa4\xd7\x49\xd4\x8f\xe5\x48\xb9\xa5\x76\xb8\xa3\xa1\x5e\xde\xa5\xaf\x86\xd4\xb4\x1b\x59\xbf\x58\xc3\xd6\xb3\xe4\xf5\xcf\xc8\xb6\x29\x3c\xbc\xd8\x73\x4b\x2f\x6c\xbf\x78\x8e\xa9\xdd\xb0\x31\x8b\x55\xbf\xee\xa6\xa4\xbd\xa5\x6f\x0a\x1f\x81\xc1\xeb\x65\x41\xf2\x0c\x9a\xfb\xe4\x50\x17\x13\xf8\xf5\xdd\xfd\x1a\x31\x7e\xb4\x19\x05\xca\x33\x0b\x16\x5d\x49\xab\x61\x46\x4a\x0a\xb0\x9c\x40\x45\x28\xda\x76\x88\x82\xda\x3d\x3e\x93\x5e\x54\x54\x68\xf2\xcc\xa8\xa8\x2a\x28\xf6\xb3\x20\x67\xca\x4d\xe2\xf7\xa6\x0a\xc6\x82\x85\xc2\x69\xdc\xd5\x29\x8c\x17\x0b\x29\xf3\x36\xd8\x33\x45\xe3\x85\x73\x9e\x20\x12\x2f\xa3\x8d\x75\x92\xb8\xd2\xda\x8a\x48\xa6\x26\x1f\xef\x93\x2c\xfe\x3f\x17\x86\xeb\xb4\xe1\xe1\x34\x45\xa0\x49\xa8\xd3\x80\x68\xe9\x41\x0c\x4e\x0d\x72\x8a\xe4\xf5\xbc\x9a\xf7\x11\xb0\x2a\xa9\x0d\x38\x59\xae\x8a\x15\x0a\x14\x62\xd2\x26\x11\xe1\x3a\x87\x97\xe9\x75\xfc\x72\x96\xf0\x7b\xe2\xd7\x8f\x0a\x0d\x8d\xa3\x9c\x7a\x99\x72\x17\xe1\x8e\x15\x1e\xf5\x55\xea\x25\x6f\x15\x48\x2e\xe2\x95\x44\xee\x83\x4e\x45\x7f\x27\x74\xea\x69\x95\x2a\xf9\x4b\x28\xb3\x4a\x06\x9a\x3a\xde\x37\x27\x65\xed\x24\x68\x7f\x5f\x54\xf8\x69\xd3\x4b\x6f\x28\x51\x85\x81\xdf\x03\xc5\x36\xb4\xb0\x5e\x42\xba\xc3\xcb\x22\x62\x12\x59\xa3\x69\x16\xcb\x28\x42\x77\x20\x8c\x3b\x02\x04\x14\xec\xdc\x13\xed\x1b\xd9\x0d\xc6\x77\xa7\x9b\xd0\x48\x81\xdb\xf0\x34\x11\x70\x9e\x9c\xdf\xb0\xf2\xc2\x6a\xf1\x40\x2f\x50\xcc\x68\x44\xde\x84\x54\x52\x4b\x55\x7e\x90\x9b\xcd\x56\xf3\x68\x7b\x94\x8a\x87\xd6\x70\x31\x3b\x3c\xb4\x46\x4d\x27\x3b\xc7\x24\xbf\x84\xa4\x9b\xf9\x07\x1f\x59\xc8\x5d\x9f\xc9\x40\xc8\x77\x38\x85\x1d\x72\xbf\xcc\x5a\x82\xde\x06\x16\x9f\x9e\xee\x24\xf4\x19\xce\x9f\x24\x01\xe4\xb1\xfa\x4b\xaa\xad\xee\x27\xf0\x5c\xca\x09\x4b\xbb\x8f\xf6\xc2\x79\x83\xd6\x68\xc7\xf5\x8f\x01\x42\x37\x35\xd6\x8b\xde\x36\x32\xb0\x48\xc1\x8f\x93\x4f\xe6\xd3\xbb\x7e\x48\xf1\xfe\x20\x78\xd5\x26\xd4\x93\x18\x1e\x48\x00\x15\xde\x73\x5c\x47\x43\x85\xa9\xbf\x28\xf6\xb6\x80\x0b\xa8\x9e\xc0\x91\xf6\x89\x79\x18\x6a\xf8\x56\xd6\x7c\x96\x6a\x23\x3e\x8e\x24\x76\x6c\x0a\x14\xa4\xac\xf5\xe9\x5f\x1c\xf6\x4f\xf8\x07\xc3\xf0\xf5\x15\x68\x73\x98\xff\x94\xd9\xc7\x14\x26\x01\x1b\xa9\x63\x30\x6a\x1b\x0f\x7a\x94\x12\xca\xf1\x63\x71\x7f\xe7\x95\xc1\xb3\x83\xf3\x4d\x96\xf1\x7f\xbc\x7f\x92\x39\x21\x57\xd4\x84\x31\x68\xff\x68\xa8\x7d\x07\x05\x14\xe6\xc7\x0e\xa2\x27\x00\x80\x71\x4e\x68\x85\x93\x5d\x2a\xf4\x23\x8b\xcf\x04\x64\x2c\x82\xb9\x32\xe7\x52\x43\xda\xe5\x02\xc8\x99\xf2\x7a\xef\x0b\x29\xb4\xf4\x6a\xb5\xdf\x43\x2a\xee\xd2\x90\xa3\xd7\x21\xdd\xc2\x22\xde\xdc\xfa\x30\xb8\xc2\xf0\x84\x2e\x3f\xff\xea\x32\x66\x3d\x52\x24\x15\x1e\xbd\x81\x46\x4c\x7d\xa9\xe8\x99\xdb\x1b\x3d\x74\x15\x75\xb8\xcb\xe9\xf0\x75\xe1\x85\x0d\xd3\xe6\x1d\xda\x21\x3b\xcd\x50\x9f\x2d\xba\xd9\xb0\x7b\xa4\xec\xf4\x44\x3b\xfc\x5b\x8d\x5a\x4e\xf0\xdb\x40\xd8\xcc\x91\x64\x74\x76\xf2\x59\xd8\x44\xff\xa1\xe5\xd9\xdd\x87\x55\x53\xf1\x7f\x94\xb9\xfa\x7f\x4a\x4e\xd3\x84\x73\xaf\x37\x10\x64\xf8\x77\xe1\x6d\x7b\x86\x2c\xb1\x73\x86\xb1\x8e\x00\xed\xa9\xea\x58\x10\xa6\x6a\x91\xd1\x61\xcf\x17\x53\x70\xa0\x25\xbe\x24\x8c\xf0\x9d\x0b\x5d\x25\xba\x40\x31\xfe\x93\x5a\x79\x97\xd3\x1a\xb7\x8c\x5e\x43\x06\x15\x1b\x4e\xa3\x63\xd1\x23\x58\x8e\x73\x23\xe1\x7c\x0e\xfe\x8e\xa7\xcb\x47\x85\x5d\x78\xe3\xb6\xe9\xcc\xd9\x22\x4a\x01\x10\x26\x5d\x6c\x3a\xa9\xcc\xd3\xb3\x1e\x6b\x36\xd9\xd2\xee\x8f\x2e\x25\x14\x8e\x69\x75\xd3\xdd\x0d\xa1\x61\x8b\xb9\xb8\x8b\x04\x4f\x5d\x25\x93\x5a\xd1\xd0\x25\x12\xb0\x2f\x77\x21\xb1\x70\x7f\x68\xd4\x18\x15\xd7\xda\xcc\x28\x87\xe7\x02\xdd\x0d\xbc\x14\xa8\x88\x2e\xfa\x04\xa3\x6b\x37\x18\x91\x1c\xf8\xe6\x0e\x8e\x87\x43\xb4\x88\xd1\x72\x14\x48\x31\x6a\xb3\xcf\x9c\x5f\x49\x65\xf3\xe6\x6c\x81\x32\xd4\x83\xaf\x4f\xe1\x74\xe8\x17\x53\x89\xaa\x81\x8a\xb9\x0f\x28\x8a\xd2\x86\xa6\x4b\x96\xcb\xe6\x6f\x11\x87\x69\xf1\xf7\x98\x34\x3e\x06\x7b\x6f\x25\x2b\x8d\xb9\xe2\x37\x50\x92\x30\x30\xfd\x64\xcc\xf2\xd8\xab\x2f\x2a\x6c\x49\x5d\xc9\xff\xdc\xfc\x3e\x14\x30\x56\x0c\x3a\x72\xcf\xe9\x65\xd0\x1c\xbb\x6e\x5c\xee\x65\xdb\xdf\x07\x11\xf4\xa1\x96\x02\x59\x70\xac\x0b\x55\x74\x71\xff\xe8\xfc\x7d\xab\xf1\x79\x72\x7b\x02\x08\x33\xa1\x86\xb3\xad\x9d\xf5\xbe\x79\xf5\xa1\x86\xa9\xc1\xe2\x58\x27\x76\x04\xc9\x08\x96\x3d\x39\xd8\x2c\xf9\x4e\x30\xf4\x7e\x13\x7d\x41\xd9\x8e\x8d\xca\xf5\x37\xad\x62\xec\x89\xb2\xd1\x39\x34\x49\xde\xdc\xe7\xc1\x0d\x67\x0c\x7f\x6c\xc2\x72\x23\x8f\x26\xfd\xb6\x52\x3c\xa1\x1f\xe4\x0e\x73\x94\xef\x99\x2f\xb0\x8c\xa2\x95\xf1\xc0\xbe\xcc\x46\xe2\x92\xde\xa0\x7c\x17\xdc\x37\x6a\x1e\xb1\x5e\xc5\x03\xbf\x70\x61\x24\x03\x11\xe5\xf5\x50\x0e\xd3\xa4\x7c\x51\x15\x4e\xb0\xff\xb5\x9f\x51\x37\x34\xea\x39\x5a\xc7\x7c\xbd\x4a\x07\x92\xdb\x4d\x84\x80\x71\x4d\xa3\xa2\xd0\x82\x27\x30\x20\xe8\x8a\x67\xfc\x5e\x64\x34\xde\x2d\x60\xda\x42\xea\x6d\xa5\x7d\xed\xda\x5d\x4b\xbb\x53\x10\x63\x5b\xe3\x76\xa3\xac\x5c\xfa\x04\x02\x3d\x1e\x6b\x44\x6b\x6a\xf6\xdf\x6f\x1b\x36\x1d\xd2\xb8\x9d\x62\xf3\xec\x84\x95\xfd\xb1\x2b\x3d\xbf\x55\x6f\xc1\xc7\x39\xec\xaf\xd6\x4b\x00\x99\x8f\xa3\x55\xf0\xfa\x33\x01\xf5\xd9\x1d\x5f\x7e\xce\x20\xaa\xa1\x9c\xe3\x30\x78\xe2\xa3\x31\x70\x06\x3c\x1d\xc4\x0b\xa2\x4e\x99\x78\x4b\x8b\xe1\x1f\xd0\x20\x47\x46\x99\x3f\xed\xdc\xe8\x4c\x58\x4b\xee\x25\x86\x11\xab\xcd\x61\x60\xba\xb6\x89\xf6\x59\x89\x79\xde\xf0\x73\xe7\xd7\x09\x43\x99\x2f\x03\x95\xa2\xda\xc6\x5f\xe6\x01\xa1\xf2\x31\x6a\xc0\x25\x8f\x59\x07\xe0\x85\x36\x1c\xad\x8a\xcc\x08\xf5\xdf\x90\xda\xa8\x77\x09\x99\xd0\xad\x7a\x8c\xdb\xc4\x4c\x1b\x83\x1a\xd4\xcf\x46\x62\xc6\x72\xed\x1f\xb8\x06\x35\x9d\x1a\x7e\x2a\x07\x09\xa6\x8a\xfa\x5c\x50\xe0\xc4\x30\x31\x46\x9f\x91\x78\x20\xa8\x4b\xab\x35\xb6\xa0\xa4\xdd\x2a\x9a\x0e\x94\x48\x9e\x4e\xfa\xd8\x07\x52\x89\xaa\x5f\x2e\x73\x7e\xb8\x12\xcb\xfe\xd9\x64\x3d\x6b\x7a\xd5\x8e\x6a\x45\xd8\x72\xf1\xc5\xca\x79\x13\x76\x92\x1c\x74\xda\xc5\xa2\xed\xb6\x90\x6d\xb5\xce\xa5\xe0\xe3\xb6\x74\xd3\x39\x14\x9a\xce\xa5\x0f\xc9\x22\x33\x1f\x16\x14\x48\x61\xa1\xec\xaa\x3a\xba\xb4\xf5\xf8\x58\x2f\x9c\xf8\x35\x9b\xdc\x2c\xbb\x89\x9b\xf2\x4d\x7b\x7f\x4d\x10\x15\x23\x27\x61\x3b\x06\x97\xb3\x05\xe8\x0f\x0d\xe2\x38\xf9\x9d\x46\x10\x15\x07\x4a\x36\xfa\xe3\xd9\xd7\x2c\xc5\xe1\xc2\x9d\xcd\xb3\x33\xa6\x42\x1b\x22\x8b\xfb\xe7\xa7\x1b\x77\xb0\xd6\x4b\xcf\xbb\xb7\x2b\x23\x10\x3b\xfd\xe3\xa7\xbb\x33\xe6\x9a\xf5\x33\xc7\x2b\xfb\x3b\x1e\xff\xf4\xe0\x31\x53\xf3\x07\x79\xc9\x5d\x9c\x04\x3d\x53\xa2\x9e\xf8\x5b\xb9\x89\x03\x92\xe6\x19\xd5\x4e\xf0\x33\x31\x99\x5b\x40\x67\x2a\x6d\xc0\xad\xb8\xcb\x62\x56\xa8\xcd\x26\x46\xa3\xd4\xec\x0d\xdd\x45\x57\x33\x7a\x52\xc0\x6d\x97\x9b\x9b\xec\xc6\x28\xfe\x00\x7b\x5a\x40\x60\x31\x45\x68\xdf\xe4\x9e\x19\xeb\xa7\x85\x2e\x74\x17\x49\x81\x57\x34\x68\x16\xda\xd9\x9a\x45\x83\x21\x3a\xdd\x64\xa1\x67\xe3\x2c\x4f\x26\x9f\x49\x76\x18\xe3\x06\x5b\xd4\xe2\xd1\xdc\x66\x1d\x59\x23\xc1\xb3\xd7\x1e\x40\x23\x35\xf8\xff\x49\xdf\xef\x77\xfa\xee\xc7\xcc\xa8\x61\x6d\xe1\x75\x6a\xb3\x8f\x33\x45\x5b\x4e\xe6\x83\x73\x81\x22\x3c\x59\x7f\xdd\x8f\xc4\x90\x69\xeb\x89\x6d\x6b\xd8\xfb\xaf\xf9\x20\x4f\x5e\xf7\x04\x11\xb1\x7b\x92\xba\x18\x62\x66\xeb\xeb\x4b\x77\x9f\x8d\x87\xef\xc9\x26\xd3\x1f\xac\x77\x04\xf7\x41\x21\x2a\x25\xa9\x54\x04\x15\xe2\x8e\xa1\xaf\x8a\x5c\x62\xdc\xa1\x00\x22\x43\x37\x69\x6f\xcd\x7d\xf8\x6f\x59\x1f\x65\x46\x2c\x96\x99\x1a\x18\x9c\xe0\xdb\x06\x6f\x87\xfe\xc5\x04\x9e\xb0\xf8\x8e\x64\xc7\x03\x6c\x5d\x27\xa3\x81\x40\x13\xca\xbc\x22\x51\x08\x5f\x9c\x10\xf7\x75\x2a\x6b\x7a\x77\xa9\x05\x4d\xdf\xdd\x86\x45\xca\xd9\x84\x28\xdb\x3e\x9f\x42\x95\x4d\xce\x6e\xe3\x96\xd9\x39\xc0\x29\x79\x08\xdb\x5c\x35\x13\x9c\x09\x7f\xf0\xfe\x5c\x1f\x83\x1a\x0b\x77\x71\x20\xa5\x0a\x86\xb2\xb8\xb5\x62\x54\x04\x54\x1a\x5f\x05\xc9\x36\xca\x71\x24\x3a\xe0\x18\xb0\x52\x40\x1c\x97\xf4\xf1\xfe\xa1\x5a\x93\x65\x67\xcf\x61\x78\x30\xb8\x76\xe2\xce\x8d\x27\x17\x7b\xa5\x9e\x95\x13\xae\x28\x4f\x50\xd4\x0e\xc8\x79\x61\x17\x79\xb5\xda\xbf\x54\x3e\x07\xd6\x4e\xa7\x9a\x87\x29\x35\x76\x1e\x28\xa1\x72\x9e\xbc\xb4\x83\xe7\x4c\xba\x27\x92\x65\x5c\x47\x59\x3c\x37\x43\x3d\xae\x97\x39\xa9\xaf\x18\x8b\x01\xcf\x49\x85\x43\x9e\x9e\x5d\xdc\xd9\x16\xad\x0d\x88\xc6\x10\x83\x08\x20\xc8\x00\x6c\xac\x8b\x33\x4c\x4d\x22\x8e\x79\x8f\x59\x6d\x23\xcc\xb2\xc5\x79\x37\xc0\x7d\x74\x75\x84\x61\x82\xde\x07\x1f\xf3\x7e\x62\xd9\x80\xce\xe5\x46\xee\xf3\x9f\x96\x44\x17\xb9\xfd\x28\xd1\x0f\xd1\x38\x3c\x59\x37\x6e\xcd\x99\xee\x32\x5e\xed\xae\x0c\xc6\x58\x9c\x21\xe8\x51\x76\x49\x7d\xa8\x5b\x21\x38\xb9\xad\xef\xe1\x5b\x97\x5b\xf8\x84\x00\x1a\x46\x61\xaa\xe3\x9c\xd2\x52\x31\x9e\xfa\xaf\xb9\x6e\xb0\x62\xd2\x0c\x5e\x8b\x23\x18\x98\xc2\x67\x9e\xb0\x55\xe7\x71\x8a\x58\xcd\x9a\x4f\xe8\xa2\x9b\xff\x18\x9e\xc5\xfd\xbc\xe0\xae\xf7\xcc\xe4\x9a\xb0\xae\x4d\x9e\x70\xbd\xff\x66\x72\x29\x61\xdc\xd9\xc0\x79\x57\x37\x9b\xa0\xf1\x05\x32\xe1\x13\x5a\x41\x76\x72\x4c\xee\x10\x11\x91\x16\x6f\x54\x5d\x02\x76\xb4\xc9\xa5\xe4\x59\x4f\xbb\x6a\x29\x94\x9a\x3c\x55\x34\xd7\xb9\xa0\x0d\xee\x8e\x82\x4a\xb4\xe9\x6f\x12\x0b\x14\x7e\x61\xa8\x9c\x6d\x75\x5e\x06\xc1\xed\x02\x8b\xf7\xf2\x43\xf6\xe1\xf2\x1b\xa9\x94\xcd\x3d\x1a\x69\xff\x13\xa7\xf5\x5f\xe8\xad\x92\xf5\x42\xd1\xae\xa2\x9d\xa2\x29\xd1\x51\x61\xec\x58\x1e\x13\x5b\xba\x94\xfd\x9c\x14\xa6\x3c\xd9\x1a\x43\x25\x8d\x29\x99\xb7\xd3\x51\x10\x67\xb7\x0a\x36\x55\x1f\xce\x2d\x11\x32\x5f\x19\x56\x86\x85\xf8\x6e\x2f\x5f\x84\xb1\x46\xb1\xb8\x6c\x30\xc3\x78\xb6\x2e\x9f\x60\x63\x38\x04\x31\xbb\x90\x36\x50\x95\xa0\x5e\xf6\xb3\x7c\x50\x0e\x4c\xb9\x7b\xf1\x36\xd6\x8a\x90\xf1\xc2\x14\xb2\xde\x66\x12\x0f\x98\xe1\x61\x4b\x70\xee\x69\xe5\x79\xc8\x4f\x57\x72\x3f\x04\xdd\xdc\xd2\x22\x2a\x80\xe6\x0e\x42\xb8\x3f\x95\xe0\xe1\x7b\xf8\xef\x06\xe2\x99\x75\xbe\x83\x04\x30\x62\x71\x61\x7c\x5f\x29\xfc\xb6\x4c\x62\xe8\xc1\xc5\xa3\xa0\xbf\x21\xa7\x72\x64\x7d\xbe\x5d\x3d\x8b\x4c\xb6\x6f\xe8\x08\x15\xae\xb8\x54\xbe\xb6\x06\x02\xf1\xfd\xa3\x5a\xeb\xcb\x3e\xcf\x2e\x61\xb5\x48\x4b\x5f\xac\x4a\x01\x1a\xe0\x72\x42\x68\x74\xd2\x47\x1a\xfc\x14\xee\xb6\x74\x24\x6e\x65\x3f\xc4\x2f\x5b\x3f\xd6\xe7\x3f\xf2\xbe\xde\xbd\x29\x54\x4e\x14\x14\x4f\x70\x1b\xbf\x45\x5b\x98\x65\xa3\x4c\xda\xde\x16\x7f\xa5\xb8\x07\xeb\xb8\xea\xff\x01\x8b\xd9\x3a', 2)
```

### Comparing `TPE_Bot-0.5.24/buildABot/Intents.py` & `TPE_Bot-0.5.25/buildABot/Intents.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/LearnMenu.py` & `TPE_Bot-0.5.25/buildABot/LearnMenu.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Manager.py` & `TPE_Bot-0.5.25/buildABot/Manager.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Paraphraser.py` & `TPE_Bot-0.5.25/buildABot/Paraphraser.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Password.py` & `TPE_Bot-0.5.25/buildABot/Password.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/RecommendedMenu.py` & `TPE_Bot-0.5.25/buildABot/RecommendedMenu.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/TelegramLogs.py` & `TPE_Bot-0.5.25/buildABot/TelegramLogs.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/WebApp_Learn.py` & `TPE_Bot-0.5.25/buildABot/WebApp_Learn.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/WebApp_Reco.py` & `TPE_Bot-0.5.25/buildABot/WebApp_Reco.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Webhook_Learn.py` & `TPE_Bot-0.5.25/buildABot/Webhook_Learn.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Webhook_Reco.py` & `TPE_Bot-0.5.25/buildABot/Webhook_Reco.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Worksheets.py` & `TPE_Bot-0.5.25/buildABot/Worksheets.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Worksheets_Learn.py` & `TPE_Bot-0.5.25/buildABot/Worksheets_Learn.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/Worksheets_Reco.py` & `TPE_Bot-0.5.25/buildABot/Worksheets_Reco.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/__init__.py` & `TPE_Bot-0.5.25/buildABot/__init__.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/buildABot/pytransform/__init__.py` & `TPE_Bot-0.5.25/buildABot/pytransform/__init__.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/parrot/__init__.py` & `TPE_Bot-0.5.25/parrot/__init__.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/parrot/demo.py` & `TPE_Bot-0.5.25/parrot/demo.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/parrot/filters.py` & `TPE_Bot-0.5.25/parrot/filters.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/parrot/parrot.py` & `TPE_Bot-0.5.25/parrot/parrot.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/parrot/pytransform/__init__.py` & `TPE_Bot-0.5.25/parrot/pytransform/__init__.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/pytransform/__init__.py` & `TPE_Bot-0.5.25/pytransform/__init__.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.24/setup.py` & `TPE_Bot-0.5.25/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="TPE_Bot", # Replace with your own username
-    version="0.5.24",
+    version="0.5.25",
     author="Ester Goh",
     description="A TPEdu personalised chatbot package",
     packages=setuptools.find_packages(),
     package_data={'': ['Data/*/*.js', 'Data/*/*.html', 'Data/*/*.json']},
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
```


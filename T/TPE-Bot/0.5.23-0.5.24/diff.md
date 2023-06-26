# Comparing `tmp/TPE_Bot-0.5.23.tar.gz` & `tmp/TPE_Bot-0.5.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TPE_Bot-0.5.23.tar", last modified: Wed Jun  7 08:00:19 2023, max compression
+gzip compressed data, was "TPE_Bot-0.5.24.tar", last modified: Mon Jun 26 06:32:02 2023, max compression
```

## Comparing `TPE_Bot-0.5.23.tar` & `TPE_Bot-0.5.24.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 08:00:19.337359 TPE_Bot-0.5.23/
--rw-rw-rw-   0        0        0      242 2023-06-07 08:00:19.337359 TPE_Bot-0.5.23/PKG-INFO
--rw-rw-rw-   0        0        0      720 2023-05-23 10:33:05.000000 TPE_Bot-0.5.23/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 08:00:19.217679 TPE_Bot-0.5.23/TPE_Bot.egg-info/
--rw-rw-rw-   0        0        0      242 2023-06-07 08:00:19.000000 TPE_Bot-0.5.23/TPE_Bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6530 2023-06-07 08:00:19.000000 TPE_Bot-0.5.23/TPE_Bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 08:00:19.000000 TPE_Bot-0.5.23/TPE_Bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-06-07 08:00:19.000000 TPE_Bot-0.5.23/TPE_Bot.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-07 08:00:19.240619 TPE_Bot-0.5.23/buildABot/
--rw-rw-rw-   0        0        0    40255 2023-05-17 19:55:47.000000 TPE_Bot-0.5.23/buildABot/Analytics.py
-drwxrwxrwx   0        0        0        0 2023-06-07 08:00:19.241618 TPE_Bot-0.5.23/buildABot/Data/
-drwxrwxrwx   0        0        0        0 2023-06-07 08:00:19.278516 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/
--rw-rw-rw-   0        0        0     1062 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Default Fallback Intent.json
--rw-rw-rw-   0        0        0     1096 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Default Welcome Intent - fallback.json
--rw-rw-rw-   0        0        0     3158 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Default Welcome Intent.json
--rw-rw-rw-   0        0        0      244 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Default Welcome Intent_usersays_en.json
--rw-rw-rw-   0        0        0     1131 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Downvote.json
--rw-rw-rw-   0        0        0      982 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Downvote_usersays_en.json
--rw-rw-rw-   0        0        0     3785 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Email Enquiry.json
--rw-rw-rw-   0        0        0     2453 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Email Enquiry_usersays_en.json
--rw-rw-rw-   0        0        0     1518 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Exit Conversation.json
--rw-rw-rw-   0        0        0     2173 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Exit Conversation_usersays_en.json
--rw-rw-rw-   0        0        0      682 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Fallback - Logged In - fallback.json
--rw-rw-rw-   0        0        0     1525 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Fallback - Logged In - no.json
--rw-rw-rw-   0        0        0    10929 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Fallback - Logged In - no_usersays_en.json
--rw-rw-rw-   0        0        0     1074 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Fallback - Logged In - yes.json
--rw-rw-rw-   0        0        0    10255 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Fallback - Logged In - yes_usersays_en.json
--rw-rw-rw-   0        0        0     1164 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Log In - Remember Name.json
--rw-rw-rw-   0        0        0      239 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Log In - Remember Name_usersays_en.json
--rw-rw-rw-   0        0        0     2186 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Log In - Results - Password - Correct.json
--rw-rw-rw-   0        0        0      613 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Log In - Results - Password - Correct_usersays_en.json
--rw-rw-rw-   0        0        0     1177 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback - fallback.json
--rw-rw-rw-   0        0        0     1238 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback.json
--rw-rw-rw-   0        0        0     1197 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Log In - Results - Password - fallback.json
--rw-rw-rw-   0        0        0     2257 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Log In - Results - Password.json
--rw-rw-rw-   0        0        0      752 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Log In - Results - Password_usersays_en.json
--rw-rw-rw-   0        0        0      249 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Log In - Sentiment (Awesome)_usersays_en.json
--rw-rw-rw-   0        0        0      252 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Log In - Sentiment (Doing Fine)_usersays_en.json
--rw-rw-rw-   0        0        0      264 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Log In - Sentiment (It's been a rough week)_usersays_en.json
--rw-rw-rw-   0        0        0      261 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Log In - Sentiment (Still Hanging There)_usersays_en.json
--rw-rw-rw-   0        0        0     1665 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Log In.json
--rw-rw-rw-   0        0        0      597 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Log In_usersays_en.json
--rw-rw-rw-   0        0        0     1741 2023-05-17 19:35:50.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Menu - Main.json
--rw-rw-rw-   0        0        0     2454 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Menu - Main_usersays_en.json
--rw-rw-rw-   0        0        0     1079 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Thankyou.json
--rw-rw-rw-   0        0        0     1496 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Thankyou_usersays_en.json
--rw-rw-rw-   0        0        0      891 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Upvote.json
--rw-rw-rw-   0        0        0      241 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Upvote_usersays_en.json
-drwxrwxrwx   0        0        0        0 2023-06-07 08:00:19.314420 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/
--rw-rw-rw-   0        0        0     1062 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Default Fallback Intent.json
--rw-rw-rw-   0        0        0     1096 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Default Welcome Intent - fallback.json
--rw-rw-rw-   0        0        0     3158 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Default Welcome Intent.json
--rw-rw-rw-   0        0        0      244 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Default Welcome Intent_usersays_en.json
--rw-rw-rw-   0        0        0     1131 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Downvote.json
--rw-rw-rw-   0        0        0      982 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Downvote_usersays_en.json
--rw-rw-rw-   0        0        0     3785 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Email Enquiry.json
--rw-rw-rw-   0        0        0     2453 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Email Enquiry_usersays_en.json
--rw-rw-rw-   0        0        0     1518 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Exit Conversation.json
--rw-rw-rw-   0        0        0     2173 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Exit Conversation_usersays_en.json
--rw-rw-rw-   0        0        0      682 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Fallback - Logged In - fallback.json
--rw-rw-rw-   0        0        0     1525 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Fallback - Logged In - no.json
--rw-rw-rw-   0        0        0    10929 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Fallback - Logged In - no_usersays_en.json
--rw-rw-rw-   0        0        0     1074 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Fallback - Logged In - yes.json
--rw-rw-rw-   0        0        0    10255 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Fallback - Logged In - yes_usersays_en.json
--rw-rw-rw-   0        0        0     1164 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Log In - Remember Name.json
--rw-rw-rw-   0        0        0      239 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Log In - Remember Name_usersays_en.json
--rw-rw-rw-   0        0        0     2186 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct.json
--rw-rw-rw-   0        0        0      613 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct_usersays_en.json
--rw-rw-rw-   0        0        0     2219 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Log In - Results - Password - Template.json
--rw-rw-rw-   0        0        0     1177 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback - fallback.json
--rw-rw-rw-   0        0        0     1238 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback.json
--rw-rw-rw-   0        0        0     1197 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback.json
--rw-rw-rw-   0        0        0      752 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Log In - Results - Password_usersays_en.json
--rw-rw-rw-   0        0        0      249 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Log In - Sentiment (Awesome)_usersays_en.json
--rw-rw-rw-   0        0        0      252 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Log In - Sentiment (Doing Fine)_usersays_en.json
--rw-rw-rw-   0        0        0      264 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Log In - Sentiment (It's been a rough week)_usersays_en.json
--rw-rw-rw-   0        0        0      261 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Log In - Sentiment (Still Hanging There)_usersays_en.json
--rw-rw-rw-   0        0        0     1665 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Log In.json
--rw-rw-rw-   0        0        0      597 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Log In_usersays_en.json
--rw-rw-rw-   0        0        0     2076 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Menu - Main.json
--rw-rw-rw-   0        0        0     2454 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Menu - Main_usersays_en.json
--rw-rw-rw-   0        0        0     1079 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Thankyou.json
--rw-rw-rw-   0        0        0     1496 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Thankyou_usersays_en.json
--rw-rw-rw-   0        0        0      891 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Upvote.json
--rw-rw-rw-   0        0        0      241 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Upvote_usersays_en.json
-drwxrwxrwx   0        0        0        0 2023-06-07 08:00:19.319407 TPE_Bot-0.5.23/buildABot/Data/Default - Worksheets/
--rw-rw-rw-   0        0        0      249 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Worksheets/Log In - Sentiment (Awesome)_usersays_en.json
--rw-rw-rw-   0        0        0      252 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Worksheets/Log In - Sentiment (Doing Fine)_usersays_en.json
--rw-rw-rw-   0        0        0      264 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Worksheets/Log In - Sentiment (It's been a rough week)_usersays_en.json
--rw-rw-rw-   0        0        0      261 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Default - Worksheets/Log In - Sentiment (Still Hanging There)_usersays_en.json
-drwxrwxrwx   0        0        0        0 2023-06-07 08:00:19.320405 TPE_Bot-0.5.23/buildABot/Data/Entities/
--rw-rw-rw-   0        0        0      208 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Entities/LoginID.json
-drwxrwxrwx   0        0        0        0 2023-06-07 08:00:19.323396 TPE_Bot-0.5.23/buildABot/Data/WebApp/
--rw-rw-rw-   0        0        0    26827 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/WebApp/index_template_LEARN.html
--rw-rw-rw-   0        0        0    21879 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/WebApp/index_template_RECO.html
--rw-rw-rw-   0        0        0   817197 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/WebApp/reset_template_RECO.js
-drwxrwxrwx   0        0        0        0 2023-06-07 08:00:19.328393 TPE_Bot-0.5.23/buildABot/Data/Webhook/
--rw-rw-rw-   0        0        0     2162 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Webhook/CheckPwd_Template_RECO.js
--rw-rw-rw-   0        0        0     4597 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Webhook/RecommendedMenu_Template_RECO.js
--rw-rw-rw-   0        0        0     7331 2023-05-17 19:11:48.000000 TPE_Bot-0.5.23/buildABot/Data/Webhook/index_template_LEARN.js
--rw-rw-rw-   0        0        0    10693 2023-05-12 06:25:07.000000 TPE_Bot-0.5.23/buildABot/Data/Webhook/index_template_RECO.js
--rw-rw-rw-   0        0        0       89 2023-05-15 04:03:04.000000 TPE_Bot-0.5.23/buildABot/Data/__init__.py
--rw-rw-rw-   0        0        0    15847 2023-05-17 19:55:48.000000 TPE_Bot-0.5.23/buildABot/Entities.py
--rw-rw-rw-   0        0        0    12267 2023-05-17 19:55:48.000000 TPE_Bot-0.5.23/buildABot/FallbackSocialTag.py
--rw-rw-rw-   0        0        0    12103 2023-05-17 19:55:48.000000 TPE_Bot-0.5.23/buildABot/Firebase_Learn.py
--rw-rw-rw-   0        0        0    14523 2023-05-18 10:01:27.000000 TPE_Bot-0.5.23/buildABot/Firebase_Reco.py
--rw-rw-rw-   0        0        0    36243 2023-05-17 19:55:48.000000 TPE_Bot-0.5.23/buildABot/Intents.py
--rw-rw-rw-   0        0        0    42387 2023-05-18 07:15:14.000000 TPE_Bot-0.5.23/buildABot/LearnMenu.py
--rw-rw-rw-   0        0        0    79895 2023-05-18 10:21:25.000000 TPE_Bot-0.5.23/buildABot/Manager.py
--rw-rw-rw-   0        0        0    15947 2023-05-17 19:55:48.000000 TPE_Bot-0.5.23/buildABot/Paraphraser.py
--rw-rw-rw-   0        0        0     6151 2023-05-17 19:55:48.000000 TPE_Bot-0.5.23/buildABot/Password.py
--rw-rw-rw-   0        0        0    44723 2023-05-17 19:55:48.000000 TPE_Bot-0.5.23/buildABot/RecommendedMenu.py
--rw-rw-rw-   0        0        0     8791 2023-05-17 19:55:48.000000 TPE_Bot-0.5.23/buildABot/TelegramLogs.py
--rw-rw-rw-   0        0        0     7539 2023-05-17 19:55:48.000000 TPE_Bot-0.5.23/buildABot/WebApp_Learn.py
--rw-rw-rw-   0        0        0    11283 2023-05-17 19:55:48.000000 TPE_Bot-0.5.23/buildABot/WebApp_Reco.py
--rw-rw-rw-   0        0        0     9259 2023-05-17 19:55:48.000000 TPE_Bot-0.5.23/buildABot/Webhook_Learn.py
--rw-rw-rw-   0        0        0    33791 2023-05-18 09:37:37.000000 TPE_Bot-0.5.23/buildABot/Webhook_Reco.py
--rw-rw-rw-   0        0        0    23915 2023-05-16 14:52:33.000000 TPE_Bot-0.5.23/buildABot/Worksheets.py
--rw-rw-rw-   0        0        0    23811 2023-05-18 10:10:18.000000 TPE_Bot-0.5.23/buildABot/Worksheets_Learn.py
--rw-rw-rw-   0        0        0    23923 2023-05-18 10:10:18.000000 TPE_Bot-0.5.23/buildABot/Worksheets_Reco.py
--rw-rw-rw-   0        0        0     5075 2023-05-17 19:55:48.000000 TPE_Bot-0.5.23/buildABot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 08:00:19.330379 TPE_Bot-0.5.23/buildABot/pytransform/
--rw-rw-rw-   0        0        0    13587 2023-03-23 18:24:51.000000 TPE_Bot-0.5.23/buildABot/pytransform/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 08:00:19.334369 TPE_Bot-0.5.23/parrot/
--rw-rw-rw-   0        0        0     1219 2023-05-16 14:54:08.000000 TPE_Bot-0.5.23/parrot/__init__.py
--rw-rw-rw-   0        0        0     3643 2023-05-16 14:54:08.000000 TPE_Bot-0.5.23/parrot/demo.py
--rw-rw-rw-   0        0        0    25523 2023-05-16 14:54:08.000000 TPE_Bot-0.5.23/parrot/filters.py
--rw-rw-rw-   0        0        0    16591 2023-05-16 14:54:08.000000 TPE_Bot-0.5.23/parrot/parrot.py
-drwxrwxrwx   0        0        0        0 2023-06-07 08:00:19.335364 TPE_Bot-0.5.23/parrot/pytransform/
--rw-rw-rw-   0        0        0    13587 2023-03-23 18:24:51.000000 TPE_Bot-0.5.23/parrot/pytransform/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 08:00:19.336361 TPE_Bot-0.5.23/pytransform/
--rw-rw-rw-   0        0        0    13587 2023-03-23 18:24:51.000000 TPE_Bot-0.5.23/pytransform/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-07 08:00:19.338356 TPE_Bot-0.5.23/setup.cfg
--rw-rw-rw-   0        0        0      575 2023-06-07 08:00:06.000000 TPE_Bot-0.5.23/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.874245 TPE_Bot-0.5.24/
+-rw-rw-rw-   0        0        0      242 2023-06-26 06:32:02.873247 TPE_Bot-0.5.24/PKG-INFO
+-rw-rw-rw-   0        0        0      720 2023-05-23 10:33:05.000000 TPE_Bot-0.5.24/README.md
+drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.290712 TPE_Bot-0.5.24/TPE_Bot.egg-info/
+-rw-rw-rw-   0        0        0      242 2023-06-26 06:32:02.000000 TPE_Bot-0.5.24/TPE_Bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6530 2023-06-26 06:32:02.000000 TPE_Bot-0.5.24/TPE_Bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-26 06:32:02.000000 TPE_Bot-0.5.24/TPE_Bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-06-26 06:32:02.000000 TPE_Bot-0.5.24/TPE_Bot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.450800 TPE_Bot-0.5.24/buildABot/
+-rw-rw-rw-   0        0        0    40255 2023-05-17 19:55:47.000000 TPE_Bot-0.5.24/buildABot/Analytics.py
+drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.452793 TPE_Bot-0.5.24/buildABot/Data/
+drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.544065 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/
+-rw-rw-rw-   0        0        0     1062 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Default Fallback Intent.json
+-rw-rw-rw-   0        0        0     1096 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Default Welcome Intent - fallback.json
+-rw-rw-rw-   0        0        0     3158 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Default Welcome Intent.json
+-rw-rw-rw-   0        0        0      244 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Default Welcome Intent_usersays_en.json
+-rw-rw-rw-   0        0        0     1131 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Downvote.json
+-rw-rw-rw-   0        0        0      982 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Downvote_usersays_en.json
+-rw-rw-rw-   0        0        0     3785 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Email Enquiry.json
+-rw-rw-rw-   0        0        0     2453 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Email Enquiry_usersays_en.json
+-rw-rw-rw-   0        0        0     1518 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Exit Conversation.json
+-rw-rw-rw-   0        0        0     2173 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Exit Conversation_usersays_en.json
+-rw-rw-rw-   0        0        0      682 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Fallback - Logged In - fallback.json
+-rw-rw-rw-   0        0        0     1525 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Fallback - Logged In - no.json
+-rw-rw-rw-   0        0        0    10929 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Fallback - Logged In - no_usersays_en.json
+-rw-rw-rw-   0        0        0     1074 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Fallback - Logged In - yes.json
+-rw-rw-rw-   0        0        0    10255 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Fallback - Logged In - yes_usersays_en.json
+-rw-rw-rw-   0        0        0     1164 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Remember Name.json
+-rw-rw-rw-   0        0        0      239 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Remember Name_usersays_en.json
+-rw-rw-rw-   0        0        0     2186 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password - Correct.json
+-rw-rw-rw-   0        0        0      613 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password - Correct_usersays_en.json
+-rw-rw-rw-   0        0        0     1177 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback - fallback.json
+-rw-rw-rw-   0        0        0     1238 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback.json
+-rw-rw-rw-   0        0        0     1197 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password - fallback.json
+-rw-rw-rw-   0        0        0     2257 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password.json
+-rw-rw-rw-   0        0        0      752 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password_usersays_en.json
+-rw-rw-rw-   0        0        0      249 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Sentiment (Awesome)_usersays_en.json
+-rw-rw-rw-   0        0        0      252 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Sentiment (Doing Fine)_usersays_en.json
+-rw-rw-rw-   0        0        0      264 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Sentiment (It's been a rough week)_usersays_en.json
+-rw-rw-rw-   0        0        0      261 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Sentiment (Still Hanging There)_usersays_en.json
+-rw-rw-rw-   0        0        0     1665 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In.json
+-rw-rw-rw-   0        0        0      597 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In_usersays_en.json
+-rw-rw-rw-   0        0        0     1741 2023-05-17 19:35:50.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Menu - Main.json
+-rw-rw-rw-   0        0        0     2454 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Menu - Main_usersays_en.json
+-rw-rw-rw-   0        0        0     1079 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Thankyou.json
+-rw-rw-rw-   0        0        0     1496 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Thankyou_usersays_en.json
+-rw-rw-rw-   0        0        0      891 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Upvote.json
+-rw-rw-rw-   0        0        0      241 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Upvote_usersays_en.json
+drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.638333 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/
+-rw-rw-rw-   0        0        0     1062 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Default Fallback Intent.json
+-rw-rw-rw-   0        0        0     1096 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Default Welcome Intent - fallback.json
+-rw-rw-rw-   0        0        0     3158 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Default Welcome Intent.json
+-rw-rw-rw-   0        0        0      244 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Default Welcome Intent_usersays_en.json
+-rw-rw-rw-   0        0        0     1131 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Downvote.json
+-rw-rw-rw-   0        0        0      982 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Downvote_usersays_en.json
+-rw-rw-rw-   0        0        0     3785 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Email Enquiry.json
+-rw-rw-rw-   0        0        0     2453 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Email Enquiry_usersays_en.json
+-rw-rw-rw-   0        0        0     1518 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Exit Conversation.json
+-rw-rw-rw-   0        0        0     2173 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Exit Conversation_usersays_en.json
+-rw-rw-rw-   0        0        0      682 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Fallback - Logged In - fallback.json
+-rw-rw-rw-   0        0        0     1525 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Fallback - Logged In - no.json
+-rw-rw-rw-   0        0        0    10929 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Fallback - Logged In - no_usersays_en.json
+-rw-rw-rw-   0        0        0     1074 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Fallback - Logged In - yes.json
+-rw-rw-rw-   0        0        0    10255 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Fallback - Logged In - yes_usersays_en.json
+-rw-rw-rw-   0        0        0     1164 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Remember Name.json
+-rw-rw-rw-   0        0        0      239 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Remember Name_usersays_en.json
+-rw-rw-rw-   0        0        0     2186 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct.json
+-rw-rw-rw-   0        0        0      613 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct_usersays_en.json
+-rw-rw-rw-   0        0        0     2219 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password - Template.json
+-rw-rw-rw-   0        0        0     1177 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback - fallback.json
+-rw-rw-rw-   0        0        0     1238 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback.json
+-rw-rw-rw-   0        0        0     1197 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback.json
+-rw-rw-rw-   0        0        0      752 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password_usersays_en.json
+-rw-rw-rw-   0        0        0      249 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Sentiment (Awesome)_usersays_en.json
+-rw-rw-rw-   0        0        0      252 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Sentiment (Doing Fine)_usersays_en.json
+-rw-rw-rw-   0        0        0      264 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Sentiment (It's been a rough week)_usersays_en.json
+-rw-rw-rw-   0        0        0      261 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Sentiment (Still Hanging There)_usersays_en.json
+-rw-rw-rw-   0        0        0     1665 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In.json
+-rw-rw-rw-   0        0        0      597 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In_usersays_en.json
+-rw-rw-rw-   0        0        0     2076 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Menu - Main.json
+-rw-rw-rw-   0        0        0     2454 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Menu - Main_usersays_en.json
+-rw-rw-rw-   0        0        0     1079 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Thankyou.json
+-rw-rw-rw-   0        0        0     1496 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Thankyou_usersays_en.json
+-rw-rw-rw-   0        0        0      891 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Upvote.json
+-rw-rw-rw-   0        0        0      241 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Upvote_usersays_en.json
+drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.645310 TPE_Bot-0.5.24/buildABot/Data/Default - Worksheets/
+-rw-rw-rw-   0        0        0      249 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Worksheets/Log In - Sentiment (Awesome)_usersays_en.json
+-rw-rw-rw-   0        0        0      252 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Worksheets/Log In - Sentiment (Doing Fine)_usersays_en.json
+-rw-rw-rw-   0        0        0      264 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Worksheets/Log In - Sentiment (It's been a rough week)_usersays_en.json
+-rw-rw-rw-   0        0        0      261 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Default - Worksheets/Log In - Sentiment (Still Hanging There)_usersays_en.json
+drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.650296 TPE_Bot-0.5.24/buildABot/Data/Entities/
+-rw-rw-rw-   0        0        0      208 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Entities/LoginID.json
+drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.798931 TPE_Bot-0.5.24/buildABot/Data/WebApp/
+-rw-rw-rw-   0        0        0    26827 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/WebApp/index_template_LEARN.html
+-rw-rw-rw-   0        0        0    21879 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/WebApp/index_template_RECO.html
+-rw-rw-rw-   0        0        0   817197 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/WebApp/reset_template_RECO.js
+drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.826856 TPE_Bot-0.5.24/buildABot/Data/Webhook/
+-rw-rw-rw-   0        0        0     2162 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Webhook/CheckPwd_Template_RECO.js
+-rw-rw-rw-   0        0        0     4597 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Webhook/RecommendedMenu_Template_RECO.js
+-rw-rw-rw-   0        0        0     7331 2023-05-17 19:11:48.000000 TPE_Bot-0.5.24/buildABot/Data/Webhook/index_template_LEARN.js
+-rw-rw-rw-   0        0        0    10693 2023-05-12 06:25:07.000000 TPE_Bot-0.5.24/buildABot/Data/Webhook/index_template_RECO.js
+-rw-rw-rw-   0        0        0       89 2023-05-15 04:03:04.000000 TPE_Bot-0.5.24/buildABot/Data/__init__.py
+-rw-rw-rw-   0        0        0    15847 2023-05-17 19:55:48.000000 TPE_Bot-0.5.24/buildABot/Entities.py
+-rw-rw-rw-   0        0        0    12267 2023-05-17 19:55:48.000000 TPE_Bot-0.5.24/buildABot/FallbackSocialTag.py
+-rw-rw-rw-   0        0        0    12103 2023-05-17 19:55:48.000000 TPE_Bot-0.5.24/buildABot/Firebase_Learn.py
+-rw-rw-rw-   0        0        0    14567 2023-06-26 06:30:22.000000 TPE_Bot-0.5.24/buildABot/Firebase_Reco.py
+-rw-rw-rw-   0        0        0    36243 2023-05-17 19:55:48.000000 TPE_Bot-0.5.24/buildABot/Intents.py
+-rw-rw-rw-   0        0        0    42387 2023-05-18 07:15:14.000000 TPE_Bot-0.5.24/buildABot/LearnMenu.py
+-rw-rw-rw-   0        0        0    79895 2023-05-18 10:21:25.000000 TPE_Bot-0.5.24/buildABot/Manager.py
+-rw-rw-rw-   0        0        0    15947 2023-05-17 19:55:48.000000 TPE_Bot-0.5.24/buildABot/Paraphraser.py
+-rw-rw-rw-   0        0        0     6151 2023-05-17 19:55:48.000000 TPE_Bot-0.5.24/buildABot/Password.py
+-rw-rw-rw-   0        0        0    44723 2023-05-17 19:55:48.000000 TPE_Bot-0.5.24/buildABot/RecommendedMenu.py
+-rw-rw-rw-   0        0        0     8791 2023-05-17 19:55:48.000000 TPE_Bot-0.5.24/buildABot/TelegramLogs.py
+-rw-rw-rw-   0        0        0     7539 2023-05-17 19:55:48.000000 TPE_Bot-0.5.24/buildABot/WebApp_Learn.py
+-rw-rw-rw-   0        0        0    11283 2023-05-17 19:55:48.000000 TPE_Bot-0.5.24/buildABot/WebApp_Reco.py
+-rw-rw-rw-   0        0        0     9259 2023-05-17 19:55:48.000000 TPE_Bot-0.5.24/buildABot/Webhook_Learn.py
+-rw-rw-rw-   0        0        0    33791 2023-05-18 09:37:37.000000 TPE_Bot-0.5.24/buildABot/Webhook_Reco.py
+-rw-rw-rw-   0        0        0    23915 2023-05-16 14:52:33.000000 TPE_Bot-0.5.24/buildABot/Worksheets.py
+-rw-rw-rw-   0        0        0    23811 2023-05-18 10:10:18.000000 TPE_Bot-0.5.24/buildABot/Worksheets_Learn.py
+-rw-rw-rw-   0        0        0    23923 2023-05-18 10:10:18.000000 TPE_Bot-0.5.24/buildABot/Worksheets_Reco.py
+-rw-rw-rw-   0        0        0     5075 2023-05-17 19:55:48.000000 TPE_Bot-0.5.24/buildABot/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.833837 TPE_Bot-0.5.24/buildABot/pytransform/
+-rw-rw-rw-   0        0        0    13587 2023-03-23 18:24:51.000000 TPE_Bot-0.5.24/buildABot/pytransform/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.855778 TPE_Bot-0.5.24/parrot/
+-rw-rw-rw-   0        0        0     1219 2023-05-16 14:54:08.000000 TPE_Bot-0.5.24/parrot/__init__.py
+-rw-rw-rw-   0        0        0     3643 2023-05-16 14:54:08.000000 TPE_Bot-0.5.24/parrot/demo.py
+-rw-rw-rw-   0        0        0    25523 2023-05-16 14:54:08.000000 TPE_Bot-0.5.24/parrot/filters.py
+-rw-rw-rw-   0        0        0    16591 2023-05-16 14:54:08.000000 TPE_Bot-0.5.24/parrot/parrot.py
+drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.864757 TPE_Bot-0.5.24/parrot/pytransform/
+-rw-rw-rw-   0        0        0    13587 2023-03-23 18:24:51.000000 TPE_Bot-0.5.24/parrot/pytransform/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-26 06:32:02.872247 TPE_Bot-0.5.24/pytransform/
+-rw-rw-rw-   0        0        0    13587 2023-03-23 18:24:51.000000 TPE_Bot-0.5.24/pytransform/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-26 06:32:02.874245 TPE_Bot-0.5.24/setup.cfg
+-rw-rw-rw-   0        0        0      575 2023-06-26 06:31:53.000000 TPE_Bot-0.5.24/setup.py
```

### Comparing `TPE_Bot-0.5.23/README.md` & `TPE_Bot-0.5.24/README.md`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/TPE_Bot.egg-info/SOURCES.txt` & `TPE_Bot-0.5.24/TPE_Bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Analytics.py` & `TPE_Bot-0.5.24/buildABot/Analytics.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Default Fallback Intent.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Default Fallback Intent.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Default Welcome Intent - fallback.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Default Welcome Intent - fallback.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Default Welcome Intent.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Default Welcome Intent.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Downvote.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Downvote.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Downvote_usersays_en.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Downvote_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Email Enquiry.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Email Enquiry.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Email Enquiry_usersays_en.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Email Enquiry_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Exit Conversation.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Exit Conversation.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Exit Conversation_usersays_en.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Exit Conversation_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Fallback - Logged In - fallback.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Fallback - Logged In - fallback.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Fallback - Logged In - no.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Fallback - Logged In - no.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Fallback - Logged In - no_usersays_en.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Fallback - Logged In - no_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Fallback - Logged In - yes.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Fallback - Logged In - yes.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Fallback - Logged In - yes_usersays_en.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Fallback - Logged In - yes_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Log In - Remember Name.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Remember Name.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Log In - Results - Password - Correct.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password - Correct.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Log In - Results - Password - Correct_usersays_en.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password - Correct_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback - fallback.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback - fallback.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password - fallback - fallback.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Log In - Results - Password - fallback.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password - fallback.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Log In - Results - Password.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Log In - Results - Password_usersays_en.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In - Results - Password_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Log In.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Log In_usersays_en.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Log In_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Menu - Main.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Menu - Main.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Menu - Main_usersays_en.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Menu - Main_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Thankyou.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Thankyou.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Thankyou_usersays_en.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Thankyou_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Learn/Upvote.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Learn/Upvote.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Default Fallback Intent.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Default Fallback Intent.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Default Welcome Intent - fallback.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Default Welcome Intent - fallback.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Default Welcome Intent.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Default Welcome Intent.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Downvote.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Downvote.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Downvote_usersays_en.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Downvote_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Email Enquiry.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Email Enquiry.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Email Enquiry_usersays_en.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Email Enquiry_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Exit Conversation.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Exit Conversation.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Exit Conversation_usersays_en.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Exit Conversation_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Fallback - Logged In - fallback.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Fallback - Logged In - fallback.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Fallback - Logged In - no.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Fallback - Logged In - no.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Fallback - Logged In - no_usersays_en.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Fallback - Logged In - no_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Fallback - Logged In - yes.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Fallback - Logged In - yes.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Fallback - Logged In - yes_usersays_en.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Fallback - Logged In - yes_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Log In - Remember Name.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Remember Name.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct_usersays_en.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password - Correct_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Log In - Results - Password - Template.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password - Template.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback - fallback.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback - fallback.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback - fallback.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password - fallback.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Log In - Results - Password_usersays_en.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In - Results - Password_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Log In.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Log In_usersays_en.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Log In_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Menu - Main.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Menu - Main.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Menu - Main_usersays_en.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Menu - Main_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Thankyou.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Thankyou.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Thankyou_usersays_en.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Thankyou_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Default - Recommended/Upvote.json` & `TPE_Bot-0.5.24/buildABot/Data/Default - Recommended/Upvote.json`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/WebApp/index_template_LEARN.html` & `TPE_Bot-0.5.24/buildABot/Data/WebApp/index_template_LEARN.html`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/WebApp/index_template_RECO.html` & `TPE_Bot-0.5.24/buildABot/Data/WebApp/index_template_RECO.html`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/WebApp/reset_template_RECO.js` & `TPE_Bot-0.5.24/buildABot/Data/WebApp/reset_template_RECO.js`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Webhook/CheckPwd_Template_RECO.js` & `TPE_Bot-0.5.24/buildABot/Data/Webhook/CheckPwd_Template_RECO.js`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Webhook/RecommendedMenu_Template_RECO.js` & `TPE_Bot-0.5.24/buildABot/Data/Webhook/RecommendedMenu_Template_RECO.js`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Webhook/index_template_LEARN.js` & `TPE_Bot-0.5.24/buildABot/Data/Webhook/index_template_LEARN.js`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Data/Webhook/index_template_RECO.js` & `TPE_Bot-0.5.24/buildABot/Data/Webhook/index_template_RECO.js`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Entities.py` & `TPE_Bot-0.5.24/buildABot/Entities.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/FallbackSocialTag.py` & `TPE_Bot-0.5.24/buildABot/FallbackSocialTag.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Firebase_Learn.py` & `TPE_Bot-0.5.24/buildABot/Firebase_Learn.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Firebase_Reco.py` & `TPE_Bot-0.5.24/buildABot/Firebase_Reco.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,3 +1,3 @@
 from pytransform import pyarmor_runtime
 pyarmor_runtime()
-__pyarmor__(__name__, __file__, b'\x50\x59\x41\x52\x4d\x4f\x52\x00\x00\x03\x09\x00\x61\x0d\x0d\x0a\x09\x34\xe0\x02\x00\x00\x00\x00\x01\x00\x00\x00\x40\x00\x00\x00\xd6\x0d\x00\x00\x00\x00\x00\x18\x5d\x5b\xd2\xf0\x21\x7d\x24\xd7\x99\xef\x12\xc8\xd9\x1f\x6e\x2e\x00\x00\x00\x00\x00\x00\x00\x00\x85\x22\x64\x92\x1d\x70\xd3\x7e\xd9\xe4\x61\x81\xf1\x6b\xbf\xf7\x4d\x32\xe2\x5a\x8f\xf8\xd7\x50\x15\x68\x22\xaa\x75\x84\xda\x55\x0c\xc7\x19\x07\x48\x25\x55\x0c\x97\xe5\x29\xbc\xb3\x50\x60\xf0\xa3\xc8\xe9\x54\xae\xec\x8c\x73\x2b\x8a\x36\x28\xa4\xb2\x54\x88\x5c\x2f\x37\x7e\x2e\xf1\x6a\x9b\x3a\xc3\x10\x69\x0a\xdd\x2f\xbe\x16\xde\x27\x16\x38\x76\xfe\x1e\xca\xec\xa0\xd2\x86\xd8\x9f\xc7\x66\x1c\x0f\xed\x8a\x6d\xf9\x8c\x3d\xf3\x36\xb9\xc6\x48\x33\x26\x45\x05\xfe\x9b\xfc\x86\xb5\x42\xe8\x2b\x12\xd8\xc6\x82\x86\x82\xf9\xe2\x01\x63\xca\x9a\xa5\xcf\x7f\x7f\xba\xf5\xac\x84\xe2\x6e\x7a\x9e\x5e\x6f\x14\xa9\x06\x98\xfa\x26\xf3\x94\x4d\xb6\x48\xba\x20\x0d\x4d\x3e\x65\xcc\xcf\x5c\xe4\xae\x2d\x76\xac\xc6\xa0\x3e\xa9\x9a\x63\x2a\xb6\xaa\x3e\x7b\x83\xc8\x72\xd4\xcf\x9a\xd2\x29\xee\xcb\xb6\xe2\xbc\xfa\xf9\xca\x29\xe7\xa7\x29\x94\xc1\x15\x49\xee\x11\xdc\xd1\x29\x8c\x8c\xd7\x18\x56\x5f\x72\xa1\x5f\xd6\x5d\xce\x69\xc8\x3a\xb7\x31\x04\x3c\xeb\x08\x30\xcb\x3b\x54\x46\x3a\x68\x07\x7c\xb3\xd7\x9a\x11\x30\x45\xf3\x6a\xc1\x01\xdc\x1c\x19\xf7\x0a\x85\x3b\x6e\x1b\xdd\x25\x3a\xb2\xdf\x67\xc1\x28\x27\x1e\x35\xc6\xb6\xa1\x1b\xce\xd4\xb4\xf8\x63\x3c\x6d\xcc\x3c\x72\xf7\x26\x5d\x4d\xce\x74\xf9\x81\xad\x9b\x5f\xa6\xec\x33\x35\xc7\x0d\xe9\xef\x17\xf3\x93\x1a\xa7\x62\xb2\x43\x3f\x29\x4a\x56\xbb\xd4\x9b\xf9\x8e\x06\x38\x10\xb8\xb9\xd4\xcc\x2a\xf3\xd8\xea\xc7\x35\x29\xa6\x80\x75\x3f\xc5\x64\xcb\x04\x43\xeb\x34\x09\x29\x3b\xa1\xc9\x9f\xa4\x67\x7b\x7e\x5a\xe9\xac\xa1\x8e\x3e\xa0\x80\xcc\x21\x36\x96\x99\xdc\x75\x3f\xb0\xd2\xa5\x97\x5c\x7a\x3c\xe0\x29\x4a\x40\xd0\xef\x16\x76\x46\x5c\x1b\x2b\x6d\x03\x77\x31\x38\xb1\xa5\xb5\x33\xf7\x31\x70\x47\xc4\x1c\x0a\x02\xab\xd0\x3b\x3d\x06\x47\xc0\x21\xe7\xdd\xd5\xd2\xd3\x2f\x77\xf1\x96\xc6\x68\x8a\x2d\x14\xca\x86\xdd\xcb\x08\xbf\xa5\x21\xca\xc9\x22\xc9\x0f\xf1\xc0\x21\x78\xfd\x64\x46\x96\x87\x1f\x67\x37\xa5\x2c\x62\x64\xbd\x49\xc0\x85\xce\x98\xe0\xd4\x27\xd2\x17\xf8\x4c\x78\xfb\x99\xcb\x0f\x45\x52\x5d\x78\x31\xbb\x64\x50\xc4\xa4\x02\x8c\x90\xf4\xa7\x79\x30\xad\xbf\x3c\xea\xd4\x2d\xdc\x0a\x55\x51\x3e\x50\x08\x94\x30\x18\xb9\x11\xc8\x24\x5b\xea\x9f\xfd\x14\xdf\x8e\x9b\x68\xa5\x4e\x4e\x74\xea\x1a\x1c\x9d\x99\x0c\x0b\x17\x5f\x42\x10\x94\x97\xdb\x9e\x51\x7c\x15\xc3\x35\x29\xde\x06\x42\x2e\x47\x70\x10\xd0\xdc\xe0\x27\x8e\x62\xef\x9e\xd4\x37\x8f\x6c\x54\xce\x47\xb0\x69\x3f\xc0\x80\x08\xd7\x3c\x85\x24\x58\xbc\xc8\x60\xeb\xff\xc0\xe0\x88\x32\x39\x36\x42\xe2\x76\x3d\x8c\x82\x88\xe5\xee\x6f\xef\x71\xf8\xaa\x06\x2d\x69\xb3\x16\x1f\x61\xdd\x93\xca\x60\xd8\x8e\x25\xf6\xfb\x47\x52\x07\x2c\xda\xdf\xf0\xb3\xa1\x85\xde\x96\xb6\xdf\x1e\xf5\x72\x7d\x95\x0e\x13\x89\xdc\xa8\x54\x34\x13\xbe\xef\xaf\x34\x5f\x46\x0c\x01\xcc\x8d\xff\x8e\x59\x12\x26\xeb\x6e\x6d\x49\x62\x51\x0b\x43\x34\xf7\xd5\x2f\x02\x7d\x0b\x97\x2c\x9b\x56\x7f\xcb\x65\xb0\x44\xdf\x07\x04\x85\x77\xd0\x89\x2b\x71\xa0\x27\xfb\x12\xcc\xf1\x76\xa0\x96\x6a\x80\xf7\x84\x60\x0d\x08\xfa\x2a\x2a\xa0\x1c\x18\xc4\xdc\xe8\x64\x8b\x05\xed\x0a\xd1\x09\x5f\x45\x25\xef\x2b\x2b\xfd\xf2\xf1\x9c\x0e\x52\x23\x81\xb6\x3a\xfe\xfd\x6b\x2d\x8d\xe3\x63\x18\x48\xe5\x13\x84\x63\xd6\xa4\xe1\xdf\xbd\x46\xb8\x57\x4b\x6f\x6f\xc7\x31\x4a\x45\x87\xb2\x8b\x39\x35\xd3\x40\xe6\xf1\xc1\xf1\xfa\x19\x02\x0f\x43\x5a\xa8\x68\xab\xd4\xe4\x29\x4c\x89\x83\xc9\x4f\x41\x8e\x06\xa7\x3a\x29\x2e\x1a\x34\x9c\x35\x7f\x4a\x85\x40\xbf\x7b\xd0\x3b\x89\xfa\x45\x6a\xd7\x9c\x57\x9a\x35\xa2\x60\x32\x29\x9a\x81\x34\xb5\x26\x0b\x45\x2b\xf4\x60\x52\xf5\xd9\x67\xab\x20\x82\x1f\x74\x28\xd1\x40\xb7\x95\x9b\xfc\x0d\x33\x38\xa6\x8a\xb3\xae\x3d\x4c\x80\x94\x69\x7f\xcc\xe0\x6e\xb8\x8a\x63\x2a\xc2\xae\x9f\x94\xf4\x7b\x4a\xa6\x06\x4a\x8e\x46\xa6\x93\xe9\x02\x64\x83\x96\x06\xf3\x3b\x0f\x02\xb6\x95\x79\x52\x60\xba\x16\x34\xac\xfa\x12\x34\xa2\x50\x11\xec\xeb\x36\x56\x57\x71\xf8\xf7\x3d\xcb\x57\x30\xaa\xe2\x11\x6e\x1a\x97\x48\x5f\x14\xcb\x93\x2e\xda\x62\x41\x9d\x3b\x45\x57\x17\xed\x75\x08\x27\xa2\xab\x81\x1c\x52\x07\x93\x3b\xbc\x1d\x23\xb3\xb4\xec\xee\x60\xd5\xb4\xb0\x05\x1d\x89\xb3\x07\x27\x31\x5a\x4d\xea\x84\x21\x0e\xfe\xbd\x56\x17\xf4\x66\xdd\x85\x1f\xb5\x5f\xbe\x66\x2a\x6e\xb6\xdf\x97\x54\x58\x54\x13\xc3\x2d\x3c\x82\x95\x36\x49\xd9\x03\x22\xdc\x15\x14\x67\x94\x7e\x48\x3f\x66\x96\x53\x02\x34\xc9\xc3\xdd\x50\x9c\xb2\xd3\x78\x16\xbc\x03\xe2\xff\xa8\xb5\xcc\x12\x1c\xdf\xff\xab\x49\xb2\x2b\x46\xae\xe1\x9c\xe5\x20\x41\x37\x2a\x17\x5d\x96\xea\x46\xe3\x8f\xc6\x34\x94\x65\xf4\x92\xa6\x85\x43\x0d\x50\xc9\xcd\x4d\xc2\x5a\xb1\x3a\x4c\xd9\x12\x25\x24\x16\xfd\xe9\x33\x60\x72\x9b\x97\x51\x12\x63\x0e\x28\x0c\xd3\x18\xd2\xc6\x0e\x2f\x79\x84\xd7\xf3\x06\x89\x54\x0f\xf3\x5d\xeb\x33\xe7\x1f\x86\x6f\xca\x13\xf2\xcf\xf9\xb7\x9c\x61\x0b\x0c\x50\x28\xc6\xfb\x90\x8d\xac\x8f\x2b\x5b\xfe\x46\xd3\x82\xb6\x51\x30\xc3\x2b\xaf\x28\xbf\x22\xd3\x7d\x01\x1c\x6c\x21\x60\x1b\x17\x38\x91\x5a\x0e\xd9\x2a\x8d\x0c\xdd\xaf\x8d\x86\x1f\xbd\x8b\x1e\xa5\xdf\xd2\xbc\x55\x9b\xd4\x79\xcb\x28\xce\x52\x29\xa9\xe0\x90\x95\xc8\xe7\xf8\x57\x2c\x42\xd9\x4b\xb3\x0c\xde\x08\x3c\x6e\x15\x63\x00\x09\xcc\xd2\x04\xa7\x58\xb5\x07\x01\xc8\xb0\x3b\x14\xe4\x59\x5e\x07\x7a\x63\x79\x38\x27\x93\x36\x2c\xd8\xe4\xec\x1c\x3a\x05\x58\x28\x11\x3e\xce\x22\xa3\x6c\x80\x94\x2f\xce\x12\x39\x6a\x73\x61\x1c\x4d\x24\x55\x52\xff\x87\x7a\xae\xe8\x99\xd7\xf1\x16\xb8\x10\xea\x65\x38\x5c\x47\xbd\x38\xc2\x3b\xdb\x97\x14\x86\xf2\xbf\x75\x7d\x8c\x1d\x23\xb1\x02\x68\x84\xef\xa5\x5b\x67\x36\x0c\x08\x76\xd7\x69\xb5\x9e\x4f\x23\x43\x36\x7d\x6d\x1b\x97\x9c\x7f\x35\xa8\x54\xb1\xa4\x7b\xe7\xc2\x87\x00\x42\xf1\x48\xa5\xf8\xa1\xda\xf5\x0f\xf7\x74\x99\x1d\xc0\x22\x7a\xff\xcd\x48\x7a\xaa\xd8\x8e\x65\x14\xe3\x06\x56\xa1\x1e\x9f\xc5\xfd\xe9\x5a\x75\xd3\x35\x4a\x32\x1c\x47\xec\xa4\x47\xe6\xbf\xa9\xb0\xc6\xe6\x28\x56\x0a\xba\x47\x25\x85\xf8\xb5\xcb\x48\x01\xd4\xf3\x23\x3f\xe2\x59\xe1\x7b\x07\xb6\x4f\x2b\xaa\xc6\xea\x91\xca\x11\xdf\x79\xba\x71\x09\x53\x84\x2c\x50\xee\x9b\xdc\xc3\xf5\x53\x98\xc2\x44\xdf\xdf\x14\xfa\xfb\x25\x8a\x11\x44\xbc\x74\xf6\xb4\x6f\x50\xa3\x77\x31\xae\xf4\x4d\x02\xcd\x1a\x44\x9c\xd6\xdb\x0d\xdf\x4b\x84\x7b\xb7\x63\x8b\x74\xe0\xd9\xd4\x51\x3c\xfb\xbf\x8c\xde\x5d\xe3\x43\x8f\xac\xdb\xaa\x1a\xbb\x48\x0a\x61\xaf\xbe\x90\x4f\x32\xa3\x47\xab\xdc\x97\x36\x02\xe5\xe2\x40\x9c\xa3\x6e\x81\x0a\x75\xc1\x65\x84\xfb\x56\xb0\x42\x7a\xa6\xbc\x1f\x02\x7c\x35\xf0\xe0\xf8\x34\xd6\x9f\x74\xe8\x5f\x6e\x38\x4d\x2f\x4d\x55\x0e\xca\x2b\x0d\xca\x82\x8f\x88\xb0\x73\x0e\x4e\x35\xc1\x76\x21\x0f\x8a\xe5\x2c\x02\x97\x12\x2b\xd0\x2f\x27\x0e\xd7\x86\x4e\x9e\x19\x61\x5e\xa5\xb3\x54\x36\xa3\xf0\xc2\xdd\xe6\xf5\xb6\x57\xfe\x08\x10\x83\xb7\xbe\x29\xac\xfb\x83\x0a\x1e\x18\x3c\xb5\x96\xbe\x57\x7d\x06\x1c\xde\x42\xfa\x1a\x0a\x2b\x6b\x3a\x96\xab\x0d\x25\xf2\x62\x9d\xfc\xfb\x93\x92\x0f\x1a\xca\x24\x99\x85\xa9\x13\x9d\xc1\xd7\xb2\xdd\xfb\x7e\xe3\xbd\x95\xc0\x03\xaa\xa4\xcd\x12\xb7\x90\x47\x02\xce\x32\x67\xdd\x18\x7b\x2f\x61\x98\x9a\x25\xbf\xb4\xc5\x62\x83\xa6\x16\x5f\xf3\xf1\x3a\x84\x0b\x9e\x6e\x88\x50\x45\x8c\x61\x4f\x8f\x39\xad\x35\xfc\x18\xcf\x87\x6b\x01\x88\xff\x8e\xaa\x8b\x96\x60\xe5\x9e\x82\x77\x91\xd3\xdb\x2e\x91\xc8\xc0\x16\x62\x14\x15\xd2\x9e\x00\x9c\x16\x37\x80\x17\x1a\xf5\x62\x32\xa6\x39\x42\x9b\xa3\x6c\x1e\x1d\x3a\x06\xf6\x58\x66\xb2\xfe\x8f\x7c\xe8\x3a\x27\x75\xfb\xdf\x4a\xa2\x05\x6d\x41\x83\x01\x52\x4d\x15\xcd\x8a\xe3\x02\x58\x45\x92\x10\xbc\x27\xf8\x56\x91\x0d\x6b\xfa\x9e\x89\x5b\xe6\xea\xdf\x19\x39\x5a\x03\x4a\x8b\x53\x07\xee\xec\x95\x02\x15\x8c\xf0\x9d\x37\x42\xe6\x93\xce\xa7\x21\xb7\x04\xe3\xdb\x66\x9b\xd2\x05\x05\x96\xb0\xad\xc7\x78\x54\x5f\xda\x71\x58\x26\x22\xcf\x67\x7d\x21\x6f\x57\x8e\x8f\x3d\x3c\xa8\x2c\x56\xf3\xe2\x66\x58\x62\xb3\x20\xbf\x4f\xc1\x37\x42\xd3\xf2\x1f\xaa\x3b\xdc\xc3\x52\x91\x1c\xd0\x06\x91\x0b\x04\xa4\x05\x90\x0b\xa8\x8d\x96\x12\xa2\x92\x31\x9a\xb4\xb7\xe0\x9a\xd3\x98\x97\x6b\x15\xa0\xc4\x98\x59\xb0\x10\x35\xbf\x06\xdf\x92\x26\x5c\x80\x71\xf8\x0d\xf8\x5e\x0f\x01\xe4\xcb\xff\x6a\x7d\xd3\xba\x15\xe1\x7a\xab\x64\x5e\x54\xf5\x0d\x0e\x10\xb5\x88\xf9\x72\xd3\x80\x54\xe6\xe8\xd4\x41\x33\x64\x95\x8e\xf3\x50\xf1\x18\x30\x6d\xec\x66\xa8\x10\x3a\x11\x14\xe9\x69\xef\xcd\x29\xf0\x4f\xdd\x6c\xca\xac\x65\xe4\xa1\x51\xee\xa4\xdc\xaf\x4a\xd0\xf4\x17\xd4\x8c\xb4\x14\x18\xea\x1d\x18\x71\x97\x12\xea\xa6\xf2\xb8\xea\x15\x49\x8c\x6c\x26\x40\x23\x52\x6a\xe4\xae\xa7\xcd\x1b\x4d\x38\x03\xf5\x5f\x0e\xcf\x01\x70\x64\xfe\xda\xc3\xe7\xdf\xe5\x67\x0d\x96\x14\xf9\xbe\x11\x4d\x4f\x0d\x05\xd6\xd0\x8d\x3b\xa4\x27\xce\x4b\x28\xe4\x3b\x06\x11\xf7\xe2\x0f\x67\xce\x0c\x19\x24\xc2\x7e\xa7\xe7\x55\x0a\xb2\xa1\x42\x0b\x81\x36\x73\xf4\xb2\x34\x6b\x63\x8b\x13\xa2\x97\xaa\xa6\x62\xa9\x69\xe8\x22\x4d\xdc\x79\x6c\xa9\x06\x39\x22\x80\xa2\xc8\x10\xff\xac\x54\xe8\xf2\x75\x15\xea\xc9\xa8\x81\xe1\x4d\xd0\x7d\x13\xca\xcc\x5b\x46\x5f\xba\xd3\xc4\xa6\xa9\x00\xe4\xe0\xee\x56\x9c\x7b\x8b\x41\xa5\xec\xc1\xe9\x34\x9f\xdd\xf5\xbc\x79\x05\x9d\x19\x18\xa8\x48\x42\x0b\x8c\x1a\xd2\xa2\x81\xfd\xf5\x54\x70\x57\xfd\x08\xb1\xd0\x5a\xab\x5b\x8d\x5e\x9c\x8b\x82\xaf\x47\x0e\x4c\xb5\x4b\xc7\x5d\x45\x4e\x07\x09\x13\x4c\xf3\x57\x2a\xf8\x17\x57\x79\xb3\x9b\xfc\x3f\xa4\xa8\x81\x22\x88\xe9\x06\x93\x9c\x13\x2d\x1b\x9e\xc9\xc3\xbe\xaf\xa4\x87\xc2\xfe\xae\x1a\xf3\xc0\xf3\xa0\x68\x14\x87\x20\x96\xd9\xf5\x3c\x9e\x1c\x15\xf7\xc6\x2a\x66\x2d\x5f\x45\xbc\x2b\xb6\x6a\x04\x3d\x73\x59\xed\x19\x39\xb4\x9e\xaa\x0f\xb6\x1a\x8a\x78\x1b\xc7\x45\x8b\xd1\xf3\x06\xea\xfc\xb6\xba\x67\xea\x8a\x7d\x69\x43\xa7\x87\xab\xc4\xc1\x4e\x82\xb7\x7e\x9c\x2e\x03\xe7\xed\x59\x20\x87\x98\xc2\xb8\xe1\x7c\x06\x03\x16\xac\x95\xee\x01\xc0\xc3\x65\x42\x28\x45\xc4\xbe\xc9\xb1\x50\xe5\x08\x5a\x0a\x4a\x60\x08\xb0\xf2\x58\x42\x11\x91\x59\x4d\x68\x6b\x64\x22\xbc\x07\x78\x1c\xf6\x15\x53\xf8\x1e\xcf\xc2\x94\xde\xff\x51\x83\xce\x5e\xb5\x85\x4f\x07\xdb\x96\xb0\xbc\x3a\x8d\xb0\x11\xe3\xb7\xd5\x97\x7c\xf7\x31\x53\xce\xb2\x49\x70\x2a\x02\x1c\xef\x4a\x7d\xd0\x8a\xae\x18\xef\x03\xe0\x24\x3c\x42\x9e\x5d\x61\x6a\xab\x65\x6c\xea\x1d\x88\x35\x44\x8d\x78\xa4\xbb\x29\xcb\xa1\x09\x7c\xb4\xd7\x66\xaa\xe1\xbb\x9c\xbc\xe2\xe4\xf4\x5e\x6a\x97\x08\x51\xb4\x77\x00\x42\x7c\x2b\x54\xf7\x65\x90\x31\x94\x66\x4a\x05\x6a\xa7\x61\x4e\x15\xbd\xbf\x75\x98\x09\x1d\xd4\x33\xc5\x32\x3d\xc4\x45\x8a\xea\xa5\x93\xd7\xd1\xef\x00\x7a\x5f\x2e\x0d\xb6\xff\xf5\x47\xed\x3f\x01\x5e\x90\x87\x80\xe8\xe2\x5b\x3e\x1b\x18\x82\x2c\xcd\xc0\x0e\x6a\xea\xe9\x53\xcd\x3d\xd0\x70\xd0\xbe\x99\x75\x1a\xaa\x73\xcb\xb4\xe0\x17\xc1\xa7\xc8\x74\xc4\xe1\xb6\x95\xa0\x91\x41\x3f\xf3\x17\x85\xd6\x67\xe8\x15\x57\x6f\x5c\x95\xfd\xee\xa9\x7a\x25\x82\xd1\xf8\x9a\xab\xe8\xe5\xf3\xc6\x24\x6b\xab\xdc\xcd\x07\x79\x37\x39\x48\x65\x8a\x77\x91\xe6\x24\x22\x6c\xd7\x22\x53\x2b\x05\xa9\xc5\x41\x8c\xe9\xce\x0e\x68\xbd\x07\x6f\x52\x1f\x0e\x30\xe0\x69\xac\x7e\x1a\xb5\x7b\x86\x3b\xd2\x93\x8d\xd0\x3d\xcd\x4f\xb6\x26\xc1\x28\x65\x76\x39\xe3\x1b\xcb\x16\xc8\xdf\x89\xdf\x3c\x0c\x0b\x42\x84\x64\xdf\x2f\x77\x2c\xa2\xd1\xd8\x3c\xd9\xf0\x99\x49\x95\x7d\x68\x5f\xd5\x22\xa7\xed\x0f\x22\x7d\x93\x9d\x15\x95\xb4\xdc\xa8\xd4\x06\xce\x1a\x73\x06\xb8\x8e\x29\x50\x4d\xce\x14\xfa\x16\x50\x22\xe4\xf9\xa6\x94\xc0\x52\x48\x68\x5c\x44\xad\x1f\x67\x0e\xc4\x43\xe8\xea\xf2\xb1\x28\x88\x27\x95\xc8\xa5\xf8\xb9\xf8\x24\x1d\x74\xf1\x4d\x5b\x59\x35\xd4\xc0\x25\xac\x79\x02\x00\xe6\x74\xe4\x68\x6f\x3d\x38\xe7\xc8\x16\x91\xe5\x02\x73\xc2\xfa\x23\x3b\xc7\xe6\xab\x69\x44\x67\xb7\x71\x8f\x13\x80\xa9\xe3\x9f\xfa\x3f\x7b\xf6\xb6\xa3\xad\x04\xc2\x6e\xeb\xcc\xbf\xae\x6a\xec\xe9\x74\x95\xee\x51\x45\x75\x4e\xd3\x66\xec\x94\xbe\xd8\x41\x8b\x5b\xf6\x6a\xad\x97\x30\xb9\xf7\xb5\x04\x1e\xb3\xe0\x10\xda\x64\x28\x50\xe8\x86\x01\xc9\xad\xb4\x68\xb4\x99\x82\x96\x79\x05\x0a\x72\x49\xc8\x54\xe0\xbb\x71\xfb\xd6\x4f\x88\x7d\xc7\xed\xaa\xd3\x74\xb3\xc1\x5b\x7a\xf8\x70\x44\x5b\x65\x55\x97\x36\x7a\x20\x0b\x7e\x8c\x28\x70\x38\xef\xde\xf4\x03\x43\xab\x35\x09\x09\xbc\xfd\xba\x01\xdb\x6f\x75\xf6\x88\x73\xf1\x75\xa2\xdd\x82\x91\xcf\x43\x79\xc4\x19\xc7\xe9\xe7\x28\x15\xd8\x27\x18\x3e\x15\xa0\x99\x21\x71\x0d\x0b\xa1\x84\x88\x84\xe8\xf9\xaf\x6b\x38\x0f\xd2\xd0\xe6\xda\x03\xe2\x02\x58\x9a\x2e\xc2\x87\x70\x62\x09\x8b\xf8\x4d\xfb\xc9\x09\x6b\x2d\x78\x1d\x07\x3f\x9c\x91\xa4\x4e\x17\x28\x20\x78\x65\xe5\x75\xe3\x97\x3b\x8d\xd8\x1f\xa1\x75\xc5\x23\xf2\xf7\x4c\x82\x42\x27\x02\xee\xd6\x87\xa4\xc3\x0e\x54\x29\x83\x4b\x67\x73\xc1\x52\x3b\xd4\xd5\x71\x9e\x25\x5c\xe3\xba\xab\x13\x5d\x05\xc1\xb8\x7f\x02\xd0\xa9\xe8\xb2\xcb\x62\xf4\xb2\x22\x85\x1f\x4c\x6a\xc6\x21\x0e\x9a\x9e\x5f\xc1\x7b\xb4\x04\x17\x93\x6e\x33\x9c\xf2\x90\x5f\x11\x0a\xf4\x20\xa5\x7b\x46\x3e\xd6\x18\x71\x8b\xe2\x68\x7e\x75\x6b\xb0\x1d\x93\xb5\xb1\x84\x5a\xa7\xd2\xc5\xec\x8c\xde\x4d\x7f\xe1\x44\xeb\x8d\xdb\x09\x3a\x95\x70\x2a\x95\xe5\x68\x0b\x5a\x56\x2e\x0a\x88\x3f\xf5\x06\xa3\x24\x2b\xf9\x40\x34\xb7\x81\x13\xea\x72\x97\x4f\xbd\x4d\xc5\x1c\xb4\xda\xcc\x9d\x0c\x5d\x78\x25\x94\x5a\x7d\x0d\x28\x5c\x3c\xdc\x9f\xc9\x4d\x4c\x5b\x0d\xe3\x42\x37\xc4\xc6\x70\x23\xa4\xdc\x3c\x97\xf9\x79\x79\x34\x0c\x63\x59\xd2\x81\xa7\xbc\xfb\x52\x7b\xd6\x30\x13\x3c\x20\x57\x32\xa5\x12\x1a\xb9\x58\x4f\x3f\x3b\x9c\xca\xd1\xb6\x0b\x53\x62\x6c\xe0\x58\x2e\x5a\x2e\x24\xe5\x57\x9a\xcb\x6d\xa7\xe6\xc7\x56\x70\x74\xcd\x4d\x5e\xc0\xd5\xa7\x31\x98\x0a\x1b\x47\xb7\x54\x4a\x73\x7a\xea\x0c\xae\x3a\xcc\xe1\xc7\xd8\xdb\x13\xd6\x59\xf4\x44\x01\x3d\xc6\xe9\x60\x9a\x09\x62\x43\x3a\xd2\xb9\x1a\x80\x46\x1e\xc7\x0a\x45\xf4\x47\x71\x12\x24\x8d\x4d\x37\xc5\xaf\x3f\x5d\x01\x25\x53\x77\x7b\xd3\xf8\xb9\x8c\x18\xab\xe1\x32\xc6\xe9\xab\x37\x63\x32\x6d\xf8\x36\xb5\x17\x82\x39\xb5\x42\xe1\x8a\xcf\xff\x06\x15\x02\xe2\x5b\x22\xf2\xff\x70\xef\x9d\xe4\x23\xa2\x46\x6d\xa6\x03\x0d\x7a\x9c\x79\x8f\x6c\x9f\xb9\xb9\x3c\x73\xec\x8b\xb7\xf9\x1f\xf3\xb8\xee\x47\x63\xe1\x92\x76\x00\x91\x8e\x10\x08\x12\xde\x2b\xe4\xee\xbc\x6c\xf1\x93\xf8\x30\xb8\xd2\x35\xab\xc8\x14\xfd\xfd\xe3\x27\xf9\x9a\xca\xc8\x3a\x56\x13\x14\x76\x0f\xf8\x7a\x18\xe4\x5f\x71\xe8\x23\x45\x64\x05\x16\x94\x95\x33\xb1\x84\x33\xb5\x10\x06\x83\x8a\xda\xe0\xa8\xb1\x15\x5a\x1e\xd7\x02\x57\x2c\x37\x2a\x9b\xdf\x78\x58\x30\x08\xc3\xc9\xdf\x19\x6c\x67\xfc\x58\x4b\xbc\xd2\x19\xfa\x7b\xc2\xcc\x9b\xb6\x9d\xe9\x60\x5c\x30\x65\x38\x89\x3d\x9d\x9a\x82\x02\xa8\xfe\x28\xfa\x37\x03\x6b\xc6\x30\x8b\x95\xc8\x69\xfb\x42\x37\x3f\x74\x77\x11\xa9\x2e\x37\x02\x05\xa1\x22\x07\xf9\x23\xe9\x28\x6c\x9e\x03\xcb\x17\xf8\xf1\x46\x07\x7d\xf1\xc3\x06\x5f\x92\xaa\x19\xd3\x64\x9b\xf0\x6f\x4e\x7e\x10\xbb\x4b\xa5\x95\x4f\x60\xf6\x14\x1a\x90\xfd\x1a\x80\x68\xd7\x58\x1a\xc8\xd4\x95\xc5\x4e\x13\xb1\x0d\x2a\xfa\xd3\x2c\xfc\xb1\xac\xc2\x8c\x5e\xae\x88\xbe\x49\x5b\x7e\xa7', 2)
+__pyarmor__(__name__, __file__, b'\x50\x59\x41\x52\x4d\x4f\x52\x00\x00\x03\x09\x00\x61\x0d\x0d\x0a\x09\x34\xe0\x02\x00\x00\x00\x00\x01\x00\x00\x00\x40\x00\x00\x00\xe1\x0d\x00\x00\x00\x00\x00\x18\xd2\xa3\x73\x27\x0c\x75\x7b\x8f\xf3\x6a\x28\x46\x00\x19\x39\x8d\x00\x00\x00\x00\x00\x00\x00\x00\xb1\xda\x15\x0a\x62\x2b\xa0\x0a\xb9\x8e\xd0\x87\x09\x28\x25\x55\x7d\xdf\x7f\xd3\xb3\x0a\x3d\xa1\x33\x58\xcc\x8a\xf2\xd1\xe8\x60\x99\x0d\xd4\x7d\x25\x2f\x1c\xc5\xef\xd1\x3c\xac\x43\x4b\x90\x02\x9c\x1c\x31\x18\x09\x09\x5e\x09\x43\x9e\xfc\xc3\xd6\xc1\x4a\x5a\x50\xb8\xae\xc9\xca\xca\xb5\xb8\x5f\x47\x92\x1a\xdc\xe6\x81\xd6\x57\x3d\xb3\x7e\x07\x47\xfa\x5c\x9d\x5a\x78\xdc\xc6\xc8\xb4\xbe\xd3\xe8\x66\xd1\xeb\xe4\xd9\x46\x4c\xe0\x11\xc1\x84\xfb\x1f\xad\x23\x62\x4e\xc9\x42\xab\x4a\x28\x73\x6b\xee\x91\xc0\xb1\xea\xf3\x2d\xe0\x16\xad\x21\x73\x3b\xff\x2f\x1f\x79\x85\xac\x31\xa2\xe1\x3b\xf6\xca\xca\x4d\x16\xe6\xf4\x2d\xcf\x1b\xe0\x62\xc0\x4e\x9f\x2a\x95\x56\x22\x51\x72\xd0\x13\xb7\xf2\xa4\xab\x12\x89\x05\x3c\xdf\xb3\x5c\x1a\x2e\x47\x48\xeb\x0c\x4c\x68\xc0\xd1\x60\x51\x7a\xf0\xbd\x6a\x06\xd7\xff\xc9\xf2\xe6\xca\x9c\xb7\x42\xc8\x76\xb8\xf2\xd0\x84\x3a\xd1\x76\xf5\xf0\x72\xf9\xe0\x56\x24\xf8\x68\x44\x28\xba\x82\x34\x72\x49\xea\x51\x5e\x3d\x9b\x94\xe3\xea\x7a\x85\x8a\x47\x95\x36\x96\xa5\xe3\xbc\x9a\xdd\x84\x21\x11\x03\x06\x53\xc7\x43\x7a\x15\xa7\xc4\x9d\x1b\x84\x61\x14\xf1\xc2\xfc\x4b\x59\x71\xcf\xa6\x66\xbc\x3c\x51\x4c\xb2\xad\x22\xd4\xc4\xe8\x4e\x19\xca\x28\x8c\xdd\x67\xf1\x8b\xe6\x8b\xc7\xf6\x5b\x6b\x65\x11\x1d\xb6\x44\x50\x90\xfd\x6e\x6d\x95\xd6\xfd\xbf\x34\xcb\x39\xf6\xd5\x1f\x3f\xbc\xc7\x99\x93\xa1\xf4\x84\x3a\x74\xf4\x71\xf2\x77\x6c\x62\xd6\x04\xb6\x19\xab\xd4\x0e\x4b\xb1\x9f\x77\x55\x10\x36\x16\xee\x02\xc1\x95\x05\xea\xcb\xdc\xe3\x0a\xc1\x61\x3e\x97\x66\x82\x79\x1a\x3a\x95\x4b\x08\x71\x64\xd8\x7b\xbf\x3d\x31\xf8\xce\xa3\x3e\x34\x3c\x4b\xd8\x3b\x18\x00\x22\x1b\xba\x7e\x11\x04\x47\xf3\xb0\xb7\xfe\xef\xc1\x4c\x8d\x65\x09\x59\xbc\xe1\x63\xbd\xe0\x14\x13\xa3\x8e\x92\x42\xf9\xf7\x55\xa3\xad\x94\xd8\xbd\x1a\x98\xbd\xf9\xe1\xa6\xc7\x01\x71\x92\x0f\xfd\xcb\x25\x6e\xec\x7d\x87\xa8\x1c\x86\xae\x1b\x42\xe6\xc4\x02\x66\xa8\x17\x9f\x88\x07\x11\x8a\x11\xad\x98\x12\x0b\x7d\xde\x2c\x1b\x2d\x33\x93\x73\xe8\x4f\xcd\xbe\xb0\x54\x6e\x87\x55\x03\x04\x79\xd9\x04\x74\xbb\x85\x6f\xdb\x23\x58\x33\xf0\xe2\x64\x11\x1d\x3a\x11\x67\xe1\xdb\xe6\x03\x5d\xc2\xae\xa1\xb2\x02\x6f\xd0\xe1\xd4\x4b\x63\xbc\x42\xa9\x81\xb6\x77\x05\xce\xa5\x3b\x54\xf0\x77\x1d\xd5\x0c\x41\x79\xc0\xe9\xd5\xe7\x3d\xbe\xda\xd7\x04\x75\x98\x7c\x42\x39\x09\x1f\x8b\x7a\x23\xae\xc1\x1e\x0c\xe2\xc6\xcd\xd4\x9f\xf4\xe5\xac\xcf\x77\xd2\xce\xb0\x51\x8d\x06\x9c\x42\xa2\x79\xe6\xd9\x75\xb9\x88\x4c\xe0\xec\x07\xc6\x94\xb3\x18\xf9\x15\x91\x6f\x2d\x53\xbd\x99\x5c\x1d\xfd\x7a\x89\xbf\xb6\x82\x43\x42\x0c\x3a\xd8\x8b\x43\x96\x72\xf2\xab\xed\x67\x79\x9b\x5c\x2b\x81\x82\x8d\xad\xf0\xea\x17\x34\x70\x16\xc8\xe4\x3f\xe6\x66\xc7\x11\x99\x4b\x53\xa2\x01\x04\xbd\x4e\x36\x97\x22\x7d\x6e\xfb\xd3\x28\xeb\x4e\xd6\x57\x21\x26\x77\x7c\x10\x97\x83\x1a\x75\x21\x04\xb1\x63\xfc\xd1\x51\x12\xf3\x3d\xbf\xf2\x8d\x02\x78\xef\xad\x31\x1d\x9f\x3b\x52\x23\xaa\x65\x9e\x43\xf3\x42\xe4\x43\x27\xf2\x82\x84\xd4\x68\xbe\x91\x42\x6d\xc4\x3d\x49\xf9\xfc\xed\xd6\x23\x1e\xe8\x8f\x42\xd9\x75\x57\xa5\x15\x0a\x63\x4e\x87\xd6\xb0\x75\x8d\xf3\xc3\xe9\x22\xfc\x63\x8b\xb9\xcd\xbe\x79\x47\xd3\x76\x62\xa1\xbf\x7e\x64\x49\xaf\x67\x18\x67\xc1\xbe\xb8\x6b\x61\xb6\x20\x5c\x1c\x2e\x3b\xb5\x38\x0f\x51\x12\x1a\x4b\x01\xa8\x54\x32\x83\xfb\x70\x30\xa7\x07\xe5\x94\x89\x79\x56\x08\xf8\x04\xfa\xe5\xa5\x7e\x3e\xc5\xe4\x27\xe2\xc9\x26\x7f\x20\xfe\x82\x52\x84\x17\xd5\x81\x0d\xf4\x66\x22\x3f\x50\xde\xde\xfd\x96\x0c\xd3\x18\x3f\x6d\x73\x1f\xbc\x80\x0f\x2e\x98\x03\x62\x1a\xc7\xdd\x5a\x09\xd9\x5e\x9b\xcb\xda\xc4\x6e\x0d\x6c\x13\x16\x22\xac\x91\xd9\xe1\x84\xcf\xef\x26\x1a\x63\x68\xa4\xa1\x2a\xb0\xcd\x5b\x4c\xbd\x57\xca\xe0\x3a\x7e\xdf\x21\xe4\x10\xdf\x12\x38\x44\x11\xf0\x20\xff\x16\x40\xcc\xc8\x46\x50\xe5\x5e\x3b\x4f\x40\x83\x36\x68\xe5\x08\x95\x52\xa1\x0e\x87\x8c\x89\x7e\x3d\xb4\xe9\x21\x9d\x58\xd0\xf8\xab\xfa\x47\x63\xa3\x80\x91\x38\xa9\x4e\xe1\x88\xfa\x6f\xe1\x7d\xd7\xf1\xbd\xc7\x85\x5a\x89\xc9\xe2\x09\x69\x05\xb5\x99\xc1\xa9\x58\xf0\x27\x8c\x30\x42\x6f\x86\x6a\x9f\x34\x9f\xe3\xd3\x2c\x13\xe6\x88\x36\xac\x70\x88\x9a\x45\xc4\xaa\x61\xa7\xf3\x06\xef\xb2\x8d\x34\x30\x3c\xd4\xbc\xc4\x77\xa6\x2e\xdf\x30\x86\x40\x41\x4f\x76\x32\xe6\x0f\xd8\xfa\x4b\x3e\x4e\x3c\x59\x5b\x4f\x82\xce\x70\xe5\xf3\x9c\x58\xc5\x51\x5b\x5b\xd7\x57\x46\x53\xae\xd5\xcc\x09\xd4\x16\x78\x66\xc8\xb1\xf0\x61\x08\x00\xe0\xd3\xfd\xa7\xac\x3c\xd6\x14\x2f\xcc\x74\x29\xf7\xbd\x19\x7e\x78\x14\xf3\x8d\xd5\xdb\x39\x0d\xfa\x4b\x4d\x68\x46\xcd\x87\xe8\xe3\xed\x3a\x50\x58\x18\x21\x97\x2b\xc3\x8a\x14\xc7\xae\x12\x27\x87\xd4\x2c\xb2\x99\xb1\xf8\xe8\x50\x3f\xc5\x84\x75\x6c\x4a\x30\x8a\x78\x49\x66\x41\x28\x7a\x5d\xc7\x0a\x98\xc8\x7d\x65\x22\xac\xe0\x2d\x1b\xed\x43\x77\xe7\x2a\x03\x53\x0a\x49\x2a\xe2\x17\x60\xdd\xcf\x87\xee\x96\x87\x04\x67\x2c\xf4\x8a\x72\x7d\xac\x0e\x0f\x66\xf2\x32\x61\xf4\x36\xd1\xb5\xb2\xf5\x8c\x1f\x53\x20\xca\x89\x9f\xbf\xdf\x62\x99\xa9\xee\x17\x58\xe6\xe9\xed\x54\x53\x66\xef\xdf\x2d\x53\x9a\xc8\x51\x6e\x69\x70\xd7\x06\xe6\x7a\xfa\xf2\x44\xc5\xb6\x5d\x63\xef\x0a\x67\xef\x24\x06\x17\x97\xff\x07\x8e\xfb\x8d\xef\xde\xfb\xe9\x10\x5a\x42\x4e\x7a\xf4\x67\xc7\xaf\x6c\x6a\xd8\xc6\x17\x44\x59\xac\x3c\xcc\x86\x72\x63\xa5\xf3\x3d\x0d\x11\x06\x0d\x77\x66\x0a\x9d\x02\x7d\x4c\xf1\x0a\x74\xc8\x2d\x39\x0d\x42\x63\x64\x8b\x30\x9e\x4a\xab\xa1\x79\x56\x77\x1b\x7b\x28\x48\xfc\xe4\xae\x54\x3a\x94\x5f\x4e\xb3\x54\x7a\x32\x3d\xb1\x0b\x83\x8a\x03\xa5\x4a\x41\xc0\xd0\x25\xec\x0e\xb4\x02\x7f\x93\xf2\xf1\xf9\x02\xee\x2b\x3b\x0c\x3f\x24\xad\x18\xf4\x5c\x2f\xee\x7a\x70\x53\x3a\x90\xfd\x59\x0c\xc2\x5e\x4c\xc3\xac\xbf\xc5\x14\xa1\x7b\xc9\x79\xd0\xd6\x0d\x44\xeb\x63\xa4\x42\x3d\x4f\x06\x72\x85\x7c\x02\xa3\x2d\x71\x61\x8b\xd7\xca\x21\x8f\x66\x57\x39\xdc\xf4\xe6\x52\xe9\xa3\xac\x9b\x1a\xa5\x45\xd7\x45\xd3\x69\x37\x32\x05\x21\x63\x60\x71\x64\x54\xe3\x93\xb3\x0d\x03\xd6\xa6\xd1\xf0\x09\x36\x0b\x40\x1c\x36\x67\x52\x93\x37\x37\xe8\xf1\x86\xec\x72\x8e\xdc\x23\x93\xc1\x01\x11\x75\x24\x37\xe7\xe3\x16\x2e\x84\xf5\x6a\x54\xf8\xae\x32\xdf\x3b\x9e\xae\xa7\x0e\x73\x54\xe1\xa9\x13\x69\xc0\x03\x43\xd1\xb7\x9a\x27\x93\x34\x82\xbc\x74\x40\xe1\x92\xaf\x40\xcf\xc3\xfe\x22\xba\x30\x4b\x25\xee\x88\xef\xdd\x8b\x3f\x59\x3e\x0a\xaa\xab\xe3\x65\x27\xd9\x22\xae\x43\xb1\x91\x37\xea\x25\x84\x82\x3c\x06\x1f\x82\xd3\xb5\xee\xe6\xc9\x40\xd0\xa0\xde\x4d\xc4\xa1\x65\x83\x13\xc2\x9e\xeb\x4f\xb2\x93\xff\x87\x15\x81\x15\x5b\x2a\x02\xd5\x59\x50\xfd\x83\xc5\x13\x90\x7a\xfa\xc4\x92\x5f\xc5\x52\x07\x98\x17\x22\x2f\xfc\x4a\x33\x40\x21\x95\x5d\x63\x86\xc3\x9f\x86\xd8\x98\xd1\xb8\xd6\x1e\x00\xed\xe0\x46\xbc\xb6\xf8\x2f\xca\xcb\xa3\x2d\xf1\xc0\x2e\x5e\x5c\x0d\x0c\xa7\xab\x42\x34\x55\x39\xa2\xd2\x7b\x6a\x82\x3a\x98\x19\x61\x7b\x68\xa7\xbf\x97\x6d\x13\x6e\x8f\x7f\xd0\x5c\x28\x40\xd0\x90\x97\x4b\xfd\xeb\xe1\x5f\x47\x86\xae\xb7\x5b\xb4\x66\x9a\x1d\x4e\x3a\x53\xc1\x66\x17\xdf\x67\xd4\xa1\x53\x0c\xc5\xa5\x42\x23\x4c\xfd\x05\x5b\x61\xab\x4f\x8b\x8d\x01\x73\x77\x4e\x9f\x21\x5d\xc2\xbf\x2f\x51\xbe\xcf\xd5\xce\x2f\xab\x2b\xa4\x2f\x1a\xc2\x10\x03\x49\x23\xc4\x1e\x8e\x34\x83\xe6\x05\x1c\xc9\xf7\x5f\x5f\xbd\x33\x3e\x92\x13\xf3\x8c\x4c\x57\x36\xd7\x6b\x47\x16\x63\x95\xcb\x93\x64\x55\x1f\x08\x4a\x36\x0a\x4b\xcb\xd3\x11\x2f\x32\x6a\xab\x60\x80\xd9\x01\x19\xd2\x95\xb3\x32\x88\x44\x3e\x16\xe0\xd3\x3b\xb6\x5b\xc5\x27\xe8\x78\x5c\xf3\x0e\x30\x25\x2e\xf1\x10\x6e\xf7\x17\x0f\x0a\x17\x96\xc0\xc5\xb3\x5c\x94\x2e\xf3\xea\xd0\x28\x72\xf0\x9b\xae\x84\xd3\x92\xb6\x0c\xce\x42\x28\x52\x13\xb2\x1c\xb0\xfd\xb4\xed\x5b\xc9\x30\x58\xce\xe0\xee\xb8\x13\x10\x06\x0c\x06\x48\x98\x6b\xa9\x4f\x55\x76\x2b\x12\xe3\x00\x42\x88\x77\xd1\x5a\xe9\x84\x76\xce\x47\x94\x8b\x4d\x33\x83\x80\x33\xd8\x48\x31\x2e\xae\xd6\x08\x00\x44\xed\x25\xa4\xff\xea\x2d\xd9\x90\x56\x77\x76\xb7\x3c\x6e\x2b\x75\xe3\xdf\x96\xd9\x38\xc1\xab\x47\x78\x23\x73\xb2\x15\x31\xa9\xa4\x39\x3e\x9e\x8a\x7c\x81\x4e\x46\x83\x6b\x3b\xbb\x27\x7c\x3b\x22\xb8\x4c\xf8\x2c\x1f\xbc\xec\x1c\x57\x26\xaf\xca\xcd\xe5\x95\x40\xa9\xe9\xe3\xf4\xe3\xdd\xe0\x9e\x52\x22\xb7\xa0\xcf\x52\x78\x7f\x3f\x90\x35\xa3\x3a\x6f\x5b\x41\x20\x61\x3d\x0d\x13\x9b\xa2\x0a\xb3\xb9\xfc\x2b\xbe\xdc\xae\x2c\xc5\x44\x25\x0f\x13\xb0\x71\xd1\x61\xaa\x00\xed\xbe\xf0\x36\xa2\x14\x44\xb6\x8e\xf7\x3f\xfa\x26\x1a\xe0\x0b\x44\xbf\x97\x8c\x85\x8d\x9a\x73\x1a\x0b\xcc\x77\x60\x79\x41\x8c\x95\xc5\x39\x77\x60\x64\x62\xe7\x02\x57\x3f\x24\x32\x0c\x3f\xe4\xb7\x7c\xc7\x5e\x03\xfd\x89\x70\xb3\xe5\x3e\xf8\x97\x23\x80\x6f\x5a\x1b\x5c\x1d\xcb\x31\x2a\x6d\x4a\x11\x31\x7d\x6c\xe2\x97\xbf\x42\x22\xd6\x6f\x35\x09\x43\x5f\xd3\x6c\x01\x1c\x75\xd9\xc3\xfb\x1c\xa7\xfb\x92\x9a\xef\xf6\x51\x9e\x1d\x82\x6e\x49\xda\xf1\x8d\x66\x33\x18\x99\x22\xc6\x77\xfd\x71\x31\x83\x5e\xa7\x1e\x74\x88\xdf\x8a\x6b\xe3\xa3\xa6\xda\x2f\x53\xce\x75\xa9\x05\x53\xa3\x86\x66\xdb\x11\x65\xec\xe2\x47\x07\xe7\x31\x93\x60\xca\xe4\x99\xb4\x81\xad\xc3\x65\x54\xec\xc0\xe2\xfa\xf4\xc6\xce\xe1\xd9\x6c\xba\x66\x9f\xa5\x13\x2d\x1e\x57\x85\x3a\xb9\x82\x28\x92\xe2\x3d\xc4\x2c\xb1\x4a\x52\x53\x2c\x0e\xe2\xdd\x8b\x5e\xec\x68\x8b\x48\xea\xb5\xe3\x09\xbb\x23\x9d\x63\xc6\xe8\x2e\xa9\xd0\xd2\xc8\x9a\xd1\x42\x8b\xd9\x50\x05\x8b\x35\x57\x39\x0d\xa3\x92\x67\x97\x46\x55\x88\x81\x9c\x5a\x5c\x0c\xc6\xa6\xce\x78\x3a\x72\xec\x6a\x07\x90\xe8\x96\x0f\x79\xa2\x5c\x24\xc4\xc6\x5d\xab\x85\x40\x08\xad\xe8\x1b\x16\xa1\xd7\x87\xb0\x58\xf4\x01\x8f\x06\x20\x16\xda\xfb\x67\x21\xd0\x65\x3c\x05\x88\x4a\x1f\x46\xb2\x78\x59\x8b\x80\x0f\x4d\x46\xbd\x08\xb8\x1e\x4a\x35\x8b\x04\x3d\x43\x6b\x60\xc5\x32\x26\xcf\x2b\xb3\xcc\xb1\xa6\x47\xa3\x5d\xdc\x55\x97\x00\xe2\x25\x98\x33\xfe\x7c\x6e\x9e\xbb\xb2\x49\x1d\xfc\x0c\x2a\x87\x17\xa3\x57\x1a\x04\x38\x31\x89\x28\x70\x00\xb4\xca\x9d\x99\xda\x89\x15\x93\xcd\xa1\xd2\xfd\x5b\xac\x92\x7e\xd6\xfc\xb0\x78\x36\x82\x08\x0f\x93\x41\x74\x9f\x32\x14\x4a\xc8\xf0\xca\x80\xd2\x57\x7f\x39\x91\x33\x59\xfa\x95\xb8\x5d\xf6\xdd\x07\x29\xd9\x52\x40\x41\xfd\x47\x78\xc5\x64\x2d\x5d\x6e\xe6\x75\x34\xe9\xca\x38\x4f\xba\xea\x1d\x1c\xb7\x2e\x21\x04\x23\x0f\x8e\xfa\x9b\x71\xef\x0f\xe8\xc9\x5c\x46\xbb\x71\xab\xbd\x99\xc7\x05\xcb\xe9\xf9\x66\x5f\x12\xe0\xc3\x87\x5b\x13\x02\x3b\x3a\x83\x99\xac\x85\x90\x94\x1f\xb1\xca\xb0\x05\x6e\xc0\xac\x71\x3d\xf7\x9a\x65\xf0\xee\xef\xed\xc0\x57\xc6\xbd\x94\x0d\xf1\x1c\xf2\x1f\x76\x37\x33\xb5\xf1\xec\xf8\x88\x88\x2a\x11\x7f\x91\x63\xb7\x22\xd4\x8a\xb8\xc7\x6c\xf0\x92\x08\xfc\x66\x5a\x93\x07\x31\x21\xc5\x85\x07\xff\xb8\x98\xb1\x34\x31\x13\x34\x50\x55\x1e\xe3\x6b\xb6\xd6\x3b\x84\xdb\xce\x50\x28\xfb\xd3\xd1\x74\x1b\x98\x52\x73\x0d\xc1\x07\x07\x51\x67\x0d\xbf\x6f\xed\xb8\x01\x8b\x78\x8c\x53\x84\x73\x5a\xa1\xec\x45\xf3\x79\xc2\x1d\x94\x16\x7c\xe0\xd6\x0a\xbd\x53\x44\xdf\x1b\xdf\x5f\x0e\xbf\x59\xae\xf5\x1d\x85\x08\x23\xc7\x30\x10\x82\x3d\x91\xe5\x02\xb8\x95\x2b\xbb\xb3\xde\x30\x9e\x61\x77\x44\xcb\x30\x92\x51\x0c\x94\x70\x71\x0f\x19\xac\x70\xc7\x05\xf7\x0f\x55\x4d\x9b\xc4\xa5\x54\x45\x5f\x81\xe7\xe5\xd0\x21\x40\xc8\x50\x78\xc9\x28\x8d\x2d\x52\x21\x1c\x12\x97\x9c\x71\x15\x83\x8c\xe7\x73\x8d\xe6\xdf\x24\x3e\xdc\x40\x49\xaf\xfa\xb2\x58\x7d\xf9\x81\x76\x21\xaa\xa5\xb3\x5c\x1d\x17\x49\x11\xb5\x9b\xba\xe3\x21\x2b\x91\x7d\x46\xa8\x59\xcb\xe2\xdf\x84\xfe\x76\x91\x1e\x1f\xba\x3b\x37\x51\x08\x67\xa0\x2b\xe2\xfa\x9e\xe7\x6b\x9a\x10\x68\x30\xe5\x04\x66\x41\x9e\x42\x07\x7c\xda\xb3\x97\x3e\xdd\xe1\xe5\xcf\x4a\x30\x7b\x4d\xa0\x7b\x92\xb1\xaa\x7a\x38\x8e\x1a\x00\x78\xb3\x74\xe1\x82\x25\xc2\xf4\xa3\x13\xb7\xa3\xab\xe7\xc9\x66\xce\x16\xc0\x71\x14\x56\x60\x11\xaf\xbd\xbc\xa9\xe5\xbf\x35\x31\xa7\x44\x49\x22\x29\xf2\xdf\xa6\x8c\x70\x36\x89\x2c\x72\xac\xee\xaa\xfd\x8c\xf0\xa4\x6c\xf6\x16\xe8\xa9\xf7\x04\xa9\x05\x21\xa9\xb7\x0c\xb7\xaa\x01\x00\x33\x1e\x37\x0c\xa1\x9a\x79\x3f\x82\x7d\x89\x01\x1e\x47\x46\x9a\xca\xed\x5b\x09\x5d\x57\x22\x8a\x15\x3d\xb9\x17\x39\xfc\x59\x1c\xda\x33\xc4\xab\xe7\x7c\x23\xef\xae\x49\xc6\xd2\x47\xb2\xd2\xa6\x91\x48\x8e\x1a\x47\x27\x77\x7c\x8c\x37\xb8\x0c\x07\x2f\xee\x2e\xaf\x5f\xaf\xac\xaf\xe4\x54\x07\xd8\xd8\x35\x54\x64\xf3\x82\x84\x3f\x00\xe1\x0b\x6e\x3a\x2c\x5f\x96\xc4\x06\x82\x04\x55\x65\x2c\x39\x60\xcf\x97\x19\x7d\x3f\x42\xd4\x34\x8d\x89\x1b\x54\x06\x4c\x1a\x73\x3a\xfc\x57\xe5\xa7\xaa\xd9\x4d\xb2\x9a\xfd\xf4\x8d\x38\xa9\x24\xdb\xcc\x12\xb4\xf3\x1e\xe9\xd8\xc9\xd0\xdb\x9a\xf8\xae\x55\x04\x74\xc2\xdb\x88\xdb\x21\xe0\x76\xa9\x7e\x2d\x55\xae\xc9\xdb\xc7\xf7\x2f\x45\x5c\x55\x3e\x43\xff\x7b\x10\x5d\x93\x41\x31\xa5\x7e\xbf\x59\xa8\xe8\xa8\x4e\x01\x50\x0b\x42\x5a\xaf\x6c\xb8\xfa\x4a\xf0\xee\x17\xff\x93\x98\x13\x6b\x34\x62\x17\x5b\x7f\x39\xc5\x41\xd1\x53\x69\x8c\xe0\x2b\xbd\xd7\xf7\x5d\x7c\xe8\xca\x1b\x38\x93\x56\x0a\x92\x91\x4a\x2b\x80\xfb\x6a\x85\xf5\x5b\x74\x3d\x88\x09\xd1\xb0\xbf\xb7\xf3\x3e\xa8\x97\x1a\x4f\x1d\x73\x64\x99\xea\x6e\x83\xb4\xe1\xe7\x3e\xcb\x77\x56\xd3\x42\x15\xc0\xa5\x9f\xf3\xd9\xb5\xdb\x24\x29\x77\xba\x41\xc1\xdb\x04\x3c\x83\x3e\x8d\x4e\x6d\x88\x03\xf9\x71\x6b\xb3\xab\x26\x82\xb5\xa7\x32\xb5\x59\x12\x69\xca\xc8\x1d\x7b\xb2\x7d\x42\xee\x84\xd1\x28\x7a\x22\xd0\x04\x31\x9c\x27\x9d\x46\x10\x82\x29\xde\xbe\xe4\xda\x23\x36\x62\x6a\x09\x16\x44\x6c\x0d\x2a\xff\x99\xb3\xc1\x84\x81\x00\xba\x88\x05\x26\x58\xb1\x45\x61\x30\xf6\x43\xd2\xb6\x67\x4b\x87\x64\x5b\xac\xc1\xc2\x01\xec\xaa\x0d\xf4\x0f\xfe\xe1\x76\x8d\x33\xa5\x73\x73\xe0\xb3\x1f\x53\x02\xd4\x96\xd3\x33\xca\x99\x2a\x4a\x44\xe0\xca\x6b\x0d\xfa\xf7\x52\x10\x16\x8e\x5b\x98\x0e\x25\x61\x5f\x5a\x4d\x3e\x14\x6d\xed\xa1\x65\x6f\x9e\x41\xd6\x73\x21\xb7\xa9\xf0\xaf\x69\x81\x8a\x91\x85\xb4\xc4\xdd\x61\x90\x76\xc4\x26\x69\x90\xb4\xf2\x29\x09\xd7\x01\x64\xe5\x1f\x34\xd6\xe0\xc9\x32\x8a\x67\x9e\xa8\xa3\x46\x3e\x25\xbc\x75\xee\x07\x18\x5b\x34\x7d\x56\x3c\x25\x34\x5f\x0d\x26\xfe\x2f\x28\x6b\x2a\x9b\x93\x8f\x19\xe2\x18\xbd\xd1\xd6\xaf\x77\xa9\x15\xcf\x7d\x3f\x63\xee\xdd\x01\x5c\x15\xc5\x2d\xc7\x74\x35\x7a\x1e\xe8\x78\xb1\x44\x4e\x05\xb2\x13\xb0\x59\x10\xb3\x84\x71\xd9\x6e\xf3\x92\x6e\x18\x54\x5b\x60\x74\xa7\xab\x6e\x44\x72\xcf\xfe\x7e\x78\x8a\xbd\x64\x20\x59\xc3\x12\xee\x28\x7b\xf4\xa2\x3a\x9e\xe4\xef\x52\x15\x0b\x79\xec\x99\x7b\x14\x76\xb9\x61\xeb\x88\xfe\x4c\xa5\xc5\xff\x95\x06\xb8\x86\x4e\x14\x97\x5b\xdf\xb8\xe8\xfe\x5e\x56\x9e\x79\x15\x8e\x0e\xc0\x40\xf9\x05\xf6\x06\x0b\x09\x94\xf0\xc6\xaf\xf4\x5a\xde\xf5\x6e\x6f\x4b\x31\x4d\x6a\x58\xef\x25\x6e\x18\x16\x8a\x8f\xc3\x75\x9e\x6e\x00\x37\x44\x9f\xb7\xfa\xe6\x93\x72\x6b\xa4\x06\x47\x2c\xb1\xb8\xc3\x9d\x93\x33\x95\xa5\x41\x24\x37\x70\x07\x8d\xb1\xfa\xaf\x12\xa6\x1a\x4c\xca\xdb\xfc\x9d\x88\x78\xf1\x3e\x51\x45\x80\x41\xb4\xfc\x14\x8f\xb4\xbc\xd6\x91\xc0\x24\x43\x6b\x92\xaa\xf7\xbb\xc2\x9c\x06\x95\x21\x2d\x93\xb2\xee\x00\x35\x6a\x68\x89\xab\x3c\x47\x2d\x90\xb6\xcd\x22\xfd\x71\x22', 2)
```

### Comparing `TPE_Bot-0.5.23/buildABot/Intents.py` & `TPE_Bot-0.5.24/buildABot/Intents.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/LearnMenu.py` & `TPE_Bot-0.5.24/buildABot/LearnMenu.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Manager.py` & `TPE_Bot-0.5.24/buildABot/Manager.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Paraphraser.py` & `TPE_Bot-0.5.24/buildABot/Paraphraser.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Password.py` & `TPE_Bot-0.5.24/buildABot/Password.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/RecommendedMenu.py` & `TPE_Bot-0.5.24/buildABot/RecommendedMenu.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/TelegramLogs.py` & `TPE_Bot-0.5.24/buildABot/TelegramLogs.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/WebApp_Learn.py` & `TPE_Bot-0.5.24/buildABot/WebApp_Learn.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/WebApp_Reco.py` & `TPE_Bot-0.5.24/buildABot/WebApp_Reco.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Webhook_Learn.py` & `TPE_Bot-0.5.24/buildABot/Webhook_Learn.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Webhook_Reco.py` & `TPE_Bot-0.5.24/buildABot/Webhook_Reco.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Worksheets.py` & `TPE_Bot-0.5.24/buildABot/Worksheets.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Worksheets_Learn.py` & `TPE_Bot-0.5.24/buildABot/Worksheets_Learn.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/Worksheets_Reco.py` & `TPE_Bot-0.5.24/buildABot/Worksheets_Reco.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/__init__.py` & `TPE_Bot-0.5.24/buildABot/__init__.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/buildABot/pytransform/__init__.py` & `TPE_Bot-0.5.24/buildABot/pytransform/__init__.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/parrot/__init__.py` & `TPE_Bot-0.5.24/parrot/__init__.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/parrot/demo.py` & `TPE_Bot-0.5.24/parrot/demo.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/parrot/filters.py` & `TPE_Bot-0.5.24/parrot/filters.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/parrot/parrot.py` & `TPE_Bot-0.5.24/parrot/parrot.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/parrot/pytransform/__init__.py` & `TPE_Bot-0.5.24/parrot/pytransform/__init__.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/pytransform/__init__.py` & `TPE_Bot-0.5.24/pytransform/__init__.py`

 * *Files identical despite different names*

### Comparing `TPE_Bot-0.5.23/setup.py` & `TPE_Bot-0.5.24/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="TPE_Bot", # Replace with your own username
-    version="0.5.23",
+    version="0.5.24",
     author="Ester Goh",
     description="A TPEdu personalised chatbot package",
     packages=setuptools.find_packages(),
     package_data={'': ['Data/*/*.js', 'Data/*/*.html', 'Data/*/*.json']},
     include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
```


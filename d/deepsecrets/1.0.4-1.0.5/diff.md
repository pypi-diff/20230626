# Comparing `tmp/deepsecrets-1.0.4.tar.gz` & `tmp/deepsecrets-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepsecrets-1.0.4.tar", max compression
+gzip compressed data, was "deepsecrets-1.0.5.tar", max compression
```

## Comparing `deepsecrets-1.0.4.tar` & `deepsecrets-1.0.5.tar`

### file list

```diff
@@ -1,144 +1,146 @@
--rw-r--r--   0        0        0     1061 2023-03-27 10:35:08.129343 deepsecrets-1.0.4/LICENSE
--rw-r--r--   0        0        0     5013 2023-04-28 10:40:14.241731 deepsecrets-1.0.4/README.md
--rw-r--r--   0        0        0     8196 2023-03-28 08:59:04.340095 deepsecrets-1.0.4/deepsecrets/.DS_Store
--rw-r--r--   0        0        0      674 2023-04-27 13:31:17.046975 deepsecrets-1.0.4/deepsecrets/__init__.py
--rw-r--r--   0        0        0      107 2023-04-27 13:10:21.769450 deepsecrets-1.0.4/deepsecrets/__main__.py
--rw-r--r--   0        0        0     6429 2023-04-28 06:49:11.562918 deepsecrets-1.0.4/deepsecrets/cli.py
--rw-r--r--   0        0        0     1675 2023-04-17 13:19:49.920625 deepsecrets-1.0.4/deepsecrets/config.py
--rw-r--r--   0        0        0     8196 2023-02-26 15:19:47.000000 deepsecrets-1.0.4/deepsecrets/core/.DS_Store
--rw-r--r--   0        0        0        0 2022-05-17 09:51:36.000000 deepsecrets-1.0.4/deepsecrets/core/engines/__init__.py
--rw-r--r--   0        0        0      150 2023-01-28 13:47:04.000000 deepsecrets-1.0.4/deepsecrets/core/engines/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2696 2023-04-17 12:40:25.353990 deepsecrets-1.0.4/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc
--rw-r--r--   0        0        0     2660 2023-04-17 13:34:38.819504 deepsecrets-1.0.4/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc
--rw-r--r--   0        0        0     1992 2023-04-17 13:35:10.334351 deepsecrets-1.0.4/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc
--rw-r--r--   0        0        0     6184 2023-04-14 12:59:29.927306 deepsecrets-1.0.4/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc
--rw-r--r--   0        0        0     1611 2023-04-17 12:40:24.547637 deepsecrets-1.0.4/deepsecrets/core/engines/hashed_secret.py
--rw-r--r--   0        0        0     1200 2023-04-17 13:34:38.199667 deepsecrets-1.0.4/deepsecrets/core/engines/iengine.py
--rw-r--r--   0        0        0     1196 2023-04-17 13:35:09.681785 deepsecrets-1.0.4/deepsecrets/core/engines/regex.py
--rw-r--r--   0        0        0     4333 2023-04-14 12:59:29.251562 deepsecrets-1.0.4/deepsecrets/core/engines/semantic.py
--rw-r--r--   0        0        0     2561 2023-02-28 16:49:26.000000 deepsecrets-1.0.4/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc
--rw-r--r--   0        0        0     1495 2022-09-15 09:37:41.000000 deepsecrets-1.0.4/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc
--rw-r--r--   0        0        0     2971 2023-04-14 12:50:22.603515 deepsecrets-1.0.4/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc
--rw-r--r--   0        0        0     1686 2022-09-15 09:36:08.000000 deepsecrets-1.0.4/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc
--rw-r--r--   0        0        0     1145 2023-02-28 16:18:28.000000 deepsecrets-1.0.4/deepsecrets/core/helpers/content_analyzer.py
--rw-r--r--   0        0        0     1831 2023-04-14 12:50:21.979920 deepsecrets-1.0.4/deepsecrets/core/helpers/entropy.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.4/deepsecrets/core/model/.DS_Store
--rw-r--r--   0        0        0       82 2023-02-23 12:04:19.000000 deepsecrets-1.0.4/deepsecrets/core/model/__init__.py
--rw-r--r--   0        0        0      292 2023-02-23 12:04:20.000000 deepsecrets-1.0.4/deepsecrets/core/model/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6910 2023-04-14 13:22:42.127475 deepsecrets-1.0.4/deepsecrets/core/model/__pycache__/file.cpython-311.pyc
--rw-r--r--   0        0        0     8418 2023-03-27 20:52:52.004543 deepsecrets-1.0.4/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc
--rw-r--r--   0        0        0      695 2023-02-28 15:59:52.000000 deepsecrets-1.0.4/deepsecrets/core/model/__pycache__/semantic.cpython-311.pyc
--rw-r--r--   0        0        0     3926 2023-04-17 12:50:07.084349 deepsecrets-1.0.4/deepsecrets/core/model/__pycache__/token.cpython-311.pyc
--rw-r--r--   0        0        0     3719 2023-04-14 13:22:41.393440 deepsecrets-1.0.4/deepsecrets/core/model/file.py
--rw-r--r--   0        0        0     4374 2023-03-27 20:52:51.349485 deepsecrets-1.0.4/deepsecrets/core/model/finding.py
--rw-r--r--   0        0        0        0 2023-01-27 16:18:29.000000 deepsecrets-1.0.4/deepsecrets/core/model/rules/__init__.py
--rw-r--r--   0        0        0      154 2023-01-28 13:47:51.000000 deepsecrets-1.0.4/deepsecrets/core/model/rules/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      954 2023-02-23 12:04:24.000000 deepsecrets-1.0.4/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc
--rw-r--r--   0        0        0      488 2023-04-17 13:45:18.933981 deepsecrets-1.0.4/deepsecrets/core/model/rules/__pycache__/false_finding.cpython-311.pyc
--rw-r--r--   0        0        0     2589 2023-04-17 13:06:29.025295 deepsecrets-1.0.4/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc
--rw-r--r--   0        0        0      510 2023-04-17 12:50:07.086386 deepsecrets-1.0.4/deepsecrets/core/model/rules/__pycache__/hashing.cpython-311.pyc
--rw-r--r--   0        0        0     5588 2023-04-14 12:57:25.499628 deepsecrets-1.0.4/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc
--rw-r--r--   0        0        0     2295 2023-04-14 12:57:56.098733 deepsecrets-1.0.4/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc
--rw-r--r--   0        0        0      269 2023-02-23 11:55:43.000000 deepsecrets-1.0.4/deepsecrets/core/model/rules/exlcuded_path.py
--rw-r--r--   0        0        0      121 2023-04-17 13:44:30.761705 deepsecrets-1.0.4/deepsecrets/core/model/rules/false_finding.py
--rw-r--r--   0        0        0     1438 2023-04-17 13:06:28.309253 deepsecrets-1.0.4/deepsecrets/core/model/rules/hashed_secret.py
--rw-r--r--   0        0        0      119 2023-04-17 12:41:47.443006 deepsecrets-1.0.4/deepsecrets/core/model/rules/hashing.py
--rw-r--r--   0        0        0     2971 2023-04-14 12:57:24.773737 deepsecrets-1.0.4/deepsecrets/core/model/rules/regex.py
--rw-r--r--   0        0        0      871 2023-04-14 12:57:55.404355 deepsecrets-1.0.4/deepsecrets/core/model/rules/rule.py
--rw-r--r--   0        0        0       88 2023-02-23 11:55:43.000000 deepsecrets-1.0.4/deepsecrets/core/model/rules/semantic.py
--rw-r--r--   0        0        0      237 2023-02-28 15:59:50.000000 deepsecrets-1.0.4/deepsecrets/core/model/semantic.py
--rw-r--r--   0        0        0     2007 2023-04-17 12:50:06.475278 deepsecrets-1.0.4/deepsecrets/core/model/token.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.4/deepsecrets/core/modes/.DS_Store
--rw-r--r--   0        0        0     8425 2023-06-13 10:12:51.339833 deepsecrets-1.0.4/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc
--rw-r--r--   0        0        0     5157 2023-06-13 10:12:50.784613 deepsecrets-1.0.4/deepsecrets/core/modes/iscan_mode.py
--rw-r--r--   0        0        0      214 2023-01-25 14:00:27.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/confidence.cpython-311.pyc
--rw-r--r--   0        0        0      184 2022-09-13 14:18:23.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/confidence.cpython-39.pyc
--rw-r--r--   0        0        0      648 2023-02-28 15:59:52.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc
--rw-r--r--   0        0        0      649 2023-04-17 13:45:18.931553 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc
--rw-r--r--   0        0        0     1424 2022-11-24 10:59:56.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc
--rw-r--r--   0        0        0     1796 2022-01-29 06:07:43.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc
--rw-r--r--   0        0        0     1059 2022-05-17 09:51:38.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc
--rw-r--r--   0        0        0     2551 2023-04-17 13:11:28.556085 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc
--rw-r--r--   0        0        0     1515 2022-10-14 09:00:28.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc
--rw-r--r--   0        0        0     2281 2023-02-28 16:49:26.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc
--rw-r--r--   0        0        0     4653 2022-11-24 10:59:56.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc
--rw-r--r--   0        0        0     2752 2022-05-17 09:51:38.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc
--rw-r--r--   0        0        0      682 2023-01-28 14:26:39.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc
--rw-r--r--   0        0        0      821 2022-01-29 06:16:36.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc
--rw-r--r--   0        0        0      855 2022-10-13 11:40:21.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc
--rw-r--r--   0        0        0      783 2022-01-28 15:38:18.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc
--rw-r--r--   0        0        0     1661 2022-02-02 13:16:29.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc
--rw-r--r--   0        0        0      615 2023-02-28 15:59:52.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc
--rw-r--r--   0        0        0     2903 2022-10-13 11:43:01.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc
--rw-r--r--   0        0        0      250 2023-02-28 15:59:51.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/excluded_paths.py
--rw-r--r--   0        0        0      252 2023-04-17 13:45:18.253008 deepsecrets-1.0.4/deepsecrets/core/rulesets/false_findings.py
--rw-r--r--   0        0        0     1434 2023-04-17 13:11:27.888766 deepsecrets-1.0.4/deepsecrets/core/rulesets/hashed_secrets.py
--rw-r--r--   0        0        0      627 2023-02-28 16:35:44.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/ibuilder.py
--rw-r--r--   0        0        0      220 2023-02-28 15:59:51.000000 deepsecrets-1.0.4/deepsecrets/core/rulesets/regex.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/.DS_Store
--rw-r--r--   0        0        0      181 2023-02-23 11:55:44.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__init__.py
--rw-r--r--   0        0        0      366 2023-02-23 11:55:45.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      129 2022-09-12 09:34:48.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1059 2023-02-15 14:21:01.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc
--rw-r--r--   0        0        0      649 2022-01-28 16:00:02.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc
--rw-r--r--   0        0        0      732 2022-10-13 14:47:47.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc
--rw-r--r--   0        0        0     1948 2023-02-28 15:59:52.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc
--rw-r--r--   0        0        0      520 2022-01-28 13:54:30.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc
--rw-r--r--   0        0        0     1549 2022-10-13 14:13:37.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc
--rw-r--r--   0        0        0     2569 2022-04-25 16:49:33.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc
--rw-r--r--   0        0        0     9685 2023-03-27 20:23:09.189108 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc
--rw-r--r--   0        0        0     4195 2022-05-27 10:40:16.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc
--rw-r--r--   0        0        0     1482 2023-04-14 12:50:35.476023 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc
--rw-r--r--   0        0        0      852 2022-01-28 17:43:01.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc
--rw-r--r--   0        0        0      899 2022-09-12 09:34:48.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc
--rw-r--r--   0        0        0     1723 2023-01-25 14:00:28.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc
--rw-r--r--   0        0        0      977 2022-01-28 18:09:20.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc
--rw-r--r--   0        0        0     1010 2022-09-12 09:34:48.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc
--rw-r--r--   0        0        0      349 2023-02-15 13:58:04.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/full_content.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/.DS_Store
--rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/__init__.py
--rw-r--r--   0        0        0      153 2023-01-25 14:00:28.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      135 2022-09-12 09:34:48.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     9952 2023-02-10 11:22:52.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc
--rw-r--r--   0        0        0     6003 2022-10-13 14:25:20.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc
--rw-r--r--   0        0        0     3570 2023-04-14 12:50:43.000351 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc
--rw-r--r--   0        0        0     2799 2023-04-21 14:40:38.036123 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store
--rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/__init__.py
--rw-r--r--   0        0        0      162 2023-01-25 14:00:28.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      144 2022-09-12 10:58:48.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1353 2023-04-13 12:42:45.606082 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc
--rw-r--r--   0        0        0     2684 2022-06-08 15:19:48.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc
--rw-r--r--   0        0        0    10645 2023-02-10 11:00:04.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc
--rw-r--r--   0        0        0     4836 2022-10-13 14:38:14.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc
--rw-r--r--   0        0        0      529 2023-04-13 12:42:44.862774 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/language.py
--rw-r--r--   0        0        0        0 2023-02-10 15:56:26.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__init__.py
--rw-r--r--   0        0        0      184 2023-02-10 15:56:27.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5347 2023-04-14 13:00:04.497720 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc
--rw-r--r--   0        0        0     6476 2023-04-14 13:10:20.748746 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc
--rw-r--r--   0        0        0     2711 2023-04-14 13:00:03.807886 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py
--rw-r--r--   0        0        0     5781 2023-04-14 13:10:20.026707 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py
--rw-r--r--   0        0        0     2027 2023-04-14 12:50:42.345036 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/spot_improvements.py
--rw-r--r--   0        0        0     1801 2023-04-21 14:40:37.153608 deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/type_stream.py
--rw-r--r--   0        0        0      735 2023-02-28 15:59:51.000000 deepsecrets-1.0.4/deepsecrets/core/tokenizers/itokenizer.py
--rw-r--r--   0        0        0     6015 2023-03-27 20:23:08.303488 deepsecrets-1.0.4/deepsecrets/core/tokenizers/lexer.py
--rw-r--r--   0        0        0      600 2023-04-14 12:50:34.810801 deepsecrets-1.0.4/deepsecrets/core/tokenizers/per_line.py
--rw-r--r--   0        0        0     1022 2023-04-14 12:50:38.878506 deepsecrets-1.0.4/deepsecrets/core/tokenizers/per_word.py
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.4/deepsecrets/core/utils/.DS_Store
--rw-r--r--   0        0        0        0 2019-08-30 09:25:52.000000 deepsecrets-1.0.4/deepsecrets/core/utils/__init__.py
--rw-r--r--   0        0        0      148 2023-02-10 10:44:34.000000 deepsecrets-1.0.4/deepsecrets/core/utils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      586 2023-02-28 15:32:35.000000 deepsecrets-1.0.4/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc
--rw-r--r--   0        0        0     5469 2023-03-27 20:23:09.183623 deepsecrets-1.0.4/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc
--rw-r--r--   0        0        0     1415 2023-02-28 16:49:26.000000 deepsecrets-1.0.4/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc
--rw-r--r--   0        0        0     1774 2023-04-17 12:50:07.088140 deepsecrets-1.0.4/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc
--rw-r--r--   0        0        0      100 2023-02-28 15:32:34.000000 deepsecrets-1.0.4/deepsecrets/core/utils/exceptions.py
--rw-r--r--   0        0        0     3018 2023-03-27 20:23:08.288214 deepsecrets-1.0.4/deepsecrets/core/utils/file_analyzer.py
--rw-r--r--   0        0        0      517 2023-02-28 16:47:36.000000 deepsecrets-1.0.4/deepsecrets/core/utils/fs.py
--rw-r--r--   0        0        0      771 2023-04-17 12:49:00.602766 deepsecrets-1.0.4/deepsecrets/core/utils/hashing.py
--rw-r--r--   0        0        0     2562 2023-01-29 12:25:02.000000 deepsecrets-1.0.4/deepsecrets/rules/excluded_paths.json
--rw-r--r--   0        0        0     3990 2023-03-27 20:07:41.216976 deepsecrets-1.0.4/deepsecrets/rules/regexes.json
--rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.4/deepsecrets/scan_modes/.DS_Store
--rw-r--r--   0        0        0     5698 2023-04-17 13:42:10.557066 deepsecrets-1.0.4/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc
--rw-r--r--   0        0        0     3268 2023-04-17 13:42:09.893195 deepsecrets-1.0.4/deepsecrets/scan_modes/cli.py
--rw-r--r--   0        0        0     1666 2023-06-13 10:15:09.562204 deepsecrets-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     6189 1970-01-01 00:00:00.000000 deepsecrets-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-03-27 10:35:08.129343 deepsecrets-1.0.5/LICENSE
+-rw-r--r--   0        0        0     5013 2023-04-28 10:40:14.241731 deepsecrets-1.0.5/README.md
+-rw-r--r--   0        0        0     8196 2023-03-28 08:59:04.340095 deepsecrets-1.0.5/deepsecrets/.DS_Store
+-rw-r--r--   0        0        0      674 2023-04-27 13:31:17.046975 deepsecrets-1.0.5/deepsecrets/__init__.py
+-rw-r--r--   0        0        0      107 2023-04-27 13:10:21.769450 deepsecrets-1.0.5/deepsecrets/__main__.py
+-rw-r--r--   0        0        0     6429 2023-04-28 06:49:11.562918 deepsecrets-1.0.5/deepsecrets/cli.py
+-rw-r--r--   0        0        0     1675 2023-04-17 13:19:49.920625 deepsecrets-1.0.5/deepsecrets/config.py
+-rw-r--r--   0        0        0     8196 2023-02-26 15:19:47.000000 deepsecrets-1.0.5/deepsecrets/core/.DS_Store
+-rw-r--r--   0        0        0        0 2022-05-17 09:51:36.000000 deepsecrets-1.0.5/deepsecrets/core/engines/__init__.py
+-rw-r--r--   0        0        0      150 2023-01-28 13:47:04.000000 deepsecrets-1.0.5/deepsecrets/core/engines/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2696 2023-04-17 12:40:25.353990 deepsecrets-1.0.5/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc
+-rw-r--r--   0        0        0     2660 2023-04-17 13:34:38.819504 deepsecrets-1.0.5/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc
+-rw-r--r--   0        0        0     1992 2023-06-26 12:35:59.459732 deepsecrets-1.0.5/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc
+-rw-r--r--   0        0        0     6192 2023-06-21 09:26:58.841320 deepsecrets-1.0.5/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc
+-rw-r--r--   0        0        0     1611 2023-04-17 12:40:24.547637 deepsecrets-1.0.5/deepsecrets/core/engines/hashed_secret.py
+-rw-r--r--   0        0        0     1200 2023-04-17 13:34:38.199667 deepsecrets-1.0.5/deepsecrets/core/engines/iengine.py
+-rw-r--r--   0        0        0     1196 2023-06-26 12:35:58.745163 deepsecrets-1.0.5/deepsecrets/core/engines/regex.py
+-rw-r--r--   0        0        0     4341 2023-06-21 09:26:58.182165 deepsecrets-1.0.5/deepsecrets/core/engines/semantic.py
+-rw-r--r--   0        0        0     2561 2023-02-28 16:49:26.000000 deepsecrets-1.0.5/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc
+-rw-r--r--   0        0        0     1495 2022-09-15 09:37:41.000000 deepsecrets-1.0.5/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc
+-rw-r--r--   0        0        0     2971 2023-04-14 12:50:22.603515 deepsecrets-1.0.5/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc
+-rw-r--r--   0        0        0     1686 2022-09-15 09:36:08.000000 deepsecrets-1.0.5/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc
+-rw-r--r--   0        0        0     1145 2023-02-28 16:18:28.000000 deepsecrets-1.0.5/deepsecrets/core/helpers/content_analyzer.py
+-rw-r--r--   0        0        0     1831 2023-04-14 12:50:21.979920 deepsecrets-1.0.5/deepsecrets/core/helpers/entropy.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.5/deepsecrets/core/model/.DS_Store
+-rw-r--r--   0        0        0       82 2023-02-23 12:04:19.000000 deepsecrets-1.0.5/deepsecrets/core/model/__init__.py
+-rw-r--r--   0        0        0      292 2023-02-23 12:04:20.000000 deepsecrets-1.0.5/deepsecrets/core/model/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7459 2023-06-26 13:33:19.902788 deepsecrets-1.0.5/deepsecrets/core/model/__pycache__/file.cpython-311.pyc
+-rw-r--r--   0        0        0     8418 2023-03-27 20:52:52.004543 deepsecrets-1.0.5/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc
+-rw-r--r--   0        0        0      695 2023-02-28 15:59:52.000000 deepsecrets-1.0.5/deepsecrets/core/model/__pycache__/semantic.cpython-311.pyc
+-rw-r--r--   0        0        0     3926 2023-04-17 12:50:07.084349 deepsecrets-1.0.5/deepsecrets/core/model/__pycache__/token.cpython-311.pyc
+-rw-r--r--   0        0        0     4034 2023-06-26 13:33:19.226359 deepsecrets-1.0.5/deepsecrets/core/model/file.py
+-rw-r--r--   0        0        0     4374 2023-03-27 20:52:51.349485 deepsecrets-1.0.5/deepsecrets/core/model/finding.py
+-rw-r--r--   0        0        0        0 2023-01-27 16:18:29.000000 deepsecrets-1.0.5/deepsecrets/core/model/rules/__init__.py
+-rw-r--r--   0        0        0      154 2023-01-28 13:47:51.000000 deepsecrets-1.0.5/deepsecrets/core/model/rules/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      954 2023-02-23 12:04:24.000000 deepsecrets-1.0.5/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc
+-rw-r--r--   0        0        0      488 2023-04-17 13:45:18.933981 deepsecrets-1.0.5/deepsecrets/core/model/rules/__pycache__/false_finding.cpython-311.pyc
+-rw-r--r--   0        0        0     2589 2023-04-17 13:06:29.025295 deepsecrets-1.0.5/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc
+-rw-r--r--   0        0        0      510 2023-04-17 12:50:07.086386 deepsecrets-1.0.5/deepsecrets/core/model/rules/__pycache__/hashing.cpython-311.pyc
+-rw-r--r--   0        0        0     5588 2023-04-14 12:57:25.499628 deepsecrets-1.0.5/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc
+-rw-r--r--   0        0        0     2295 2023-04-14 12:57:56.098733 deepsecrets-1.0.5/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc
+-rw-r--r--   0        0        0      269 2023-02-23 11:55:43.000000 deepsecrets-1.0.5/deepsecrets/core/model/rules/exlcuded_path.py
+-rw-r--r--   0        0        0      121 2023-04-17 13:44:30.761705 deepsecrets-1.0.5/deepsecrets/core/model/rules/false_finding.py
+-rw-r--r--   0        0        0     1438 2023-04-17 13:06:28.309253 deepsecrets-1.0.5/deepsecrets/core/model/rules/hashed_secret.py
+-rw-r--r--   0        0        0      119 2023-04-17 12:41:47.443006 deepsecrets-1.0.5/deepsecrets/core/model/rules/hashing.py
+-rw-r--r--   0        0        0     2971 2023-04-14 12:57:24.773737 deepsecrets-1.0.5/deepsecrets/core/model/rules/regex.py
+-rw-r--r--   0        0        0      871 2023-04-14 12:57:55.404355 deepsecrets-1.0.5/deepsecrets/core/model/rules/rule.py
+-rw-r--r--   0        0        0       88 2023-02-23 11:55:43.000000 deepsecrets-1.0.5/deepsecrets/core/model/rules/semantic.py
+-rw-r--r--   0        0        0      237 2023-02-28 15:59:50.000000 deepsecrets-1.0.5/deepsecrets/core/model/semantic.py
+-rw-r--r--   0        0        0     2007 2023-04-17 12:50:06.475278 deepsecrets-1.0.5/deepsecrets/core/model/token.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.5/deepsecrets/core/modes/.DS_Store
+-rw-r--r--   0        0        0     8425 2023-06-13 10:12:51.339833 deepsecrets-1.0.5/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc
+-rw-r--r--   0        0        0     5157 2023-06-13 10:12:50.784613 deepsecrets-1.0.5/deepsecrets/core/modes/iscan_mode.py
+-rw-r--r--   0        0        0      214 2023-01-25 14:00:27.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/confidence.cpython-311.pyc
+-rw-r--r--   0        0        0      184 2022-09-13 14:18:23.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/confidence.cpython-39.pyc
+-rw-r--r--   0        0        0      648 2023-02-28 15:59:52.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc
+-rw-r--r--   0        0        0      649 2023-04-17 13:45:18.931553 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc
+-rw-r--r--   0        0        0     1424 2022-11-24 10:59:56.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc
+-rw-r--r--   0        0        0     1796 2022-01-29 06:07:43.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc
+-rw-r--r--   0        0        0     1059 2022-05-17 09:51:38.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc
+-rw-r--r--   0        0        0     2551 2023-04-17 13:11:28.556085 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc
+-rw-r--r--   0        0        0     1515 2022-10-14 09:00:28.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc
+-rw-r--r--   0        0        0     2281 2023-02-28 16:49:26.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc
+-rw-r--r--   0        0        0     4653 2022-11-24 10:59:56.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc
+-rw-r--r--   0        0        0     2752 2022-05-17 09:51:38.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc
+-rw-r--r--   0        0        0      682 2023-01-28 14:26:39.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc
+-rw-r--r--   0        0        0      821 2022-01-29 06:16:36.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc
+-rw-r--r--   0        0        0      855 2022-10-13 11:40:21.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc
+-rw-r--r--   0        0        0      783 2022-01-28 15:38:18.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc
+-rw-r--r--   0        0        0     1661 2022-02-02 13:16:29.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc
+-rw-r--r--   0        0        0      615 2023-02-28 15:59:52.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc
+-rw-r--r--   0        0        0     2903 2022-10-13 11:43:01.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc
+-rw-r--r--   0        0        0      250 2023-02-28 15:59:51.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/excluded_paths.py
+-rw-r--r--   0        0        0      252 2023-04-17 13:45:18.253008 deepsecrets-1.0.5/deepsecrets/core/rulesets/false_findings.py
+-rw-r--r--   0        0        0     1434 2023-04-17 13:11:27.888766 deepsecrets-1.0.5/deepsecrets/core/rulesets/hashed_secrets.py
+-rw-r--r--   0        0        0      627 2023-02-28 16:35:44.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/ibuilder.py
+-rw-r--r--   0        0        0      220 2023-02-28 15:59:51.000000 deepsecrets-1.0.5/deepsecrets/core/rulesets/regex.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/.DS_Store
+-rw-r--r--   0        0        0      181 2023-02-23 11:55:44.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__init__.py
+-rw-r--r--   0        0        0      366 2023-02-23 11:55:45.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      129 2022-09-12 09:34:48.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1059 2023-02-15 14:21:01.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc
+-rw-r--r--   0        0        0      649 2022-01-28 16:00:02.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc
+-rw-r--r--   0        0        0      732 2022-10-13 14:47:47.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc
+-rw-r--r--   0        0        0     1948 2023-02-28 15:59:52.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc
+-rw-r--r--   0        0        0      520 2022-01-28 13:54:30.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc
+-rw-r--r--   0        0        0     1549 2022-10-13 14:13:37.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc
+-rw-r--r--   0        0        0     2569 2022-04-25 16:49:33.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc
+-rw-r--r--   0        0        0    10200 2023-06-26 13:42:04.228723 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc
+-rw-r--r--   0        0        0     4195 2022-05-27 10:40:16.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc
+-rw-r--r--   0        0        0     1482 2023-04-14 12:50:35.476023 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc
+-rw-r--r--   0        0        0      852 2022-01-28 17:43:01.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc
+-rw-r--r--   0        0        0      899 2022-09-12 09:34:48.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc
+-rw-r--r--   0        0        0     1723 2023-01-25 14:00:28.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc
+-rw-r--r--   0        0        0      977 2022-01-28 18:09:20.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc
+-rw-r--r--   0        0        0     1010 2022-09-12 09:34:48.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc
+-rw-r--r--   0        0        0      349 2023-02-15 13:58:04.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/full_content.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/.DS_Store
+-rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/__init__.py
+-rw-r--r--   0        0        0      153 2023-01-25 14:00:28.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      135 2022-09-12 09:34:48.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     9952 2023-02-10 11:22:52.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc
+-rw-r--r--   0        0        0     6003 2022-10-13 14:25:20.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc
+-rw-r--r--   0        0        0     3663 2023-06-26 16:51:54.572701 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc
+-rw-r--r--   0        0        0     2799 2023-04-21 14:40:38.036123 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store
+-rw-r--r--   0        0        0        0 2023-01-25 14:00:23.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/__init__.py
+-rw-r--r--   0        0        0      162 2023-01-25 14:00:28.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      144 2022-09-12 10:58:48.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1353 2023-04-13 12:42:45.606082 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc
+-rw-r--r--   0        0        0     2684 2022-06-08 15:19:48.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc
+-rw-r--r--   0        0        0    10645 2023-02-10 11:00:04.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc
+-rw-r--r--   0        0        0     4836 2022-10-13 14:38:14.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc
+-rw-r--r--   0        0        0      529 2023-04-13 12:42:44.862774 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/language.py
+-rw-r--r--   0        0        0        0 2023-02-10 15:56:26.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__init__.py
+-rw-r--r--   0        0        0      184 2023-02-10 15:56:27.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5347 2023-04-14 13:00:04.497720 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc
+-rw-r--r--   0        0        0     6476 2023-04-14 13:10:20.748746 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc
+-rw-r--r--   0        0        0     2711 2023-04-14 13:00:03.807886 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py
+-rw-r--r--   0        0        0     5781 2023-04-14 13:10:20.026707 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py
+-rw-r--r--   0        0        0     2115 2023-06-26 16:51:53.987615 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/spot_improvements.py
+-rw-r--r--   0        0        0     1801 2023-04-21 14:40:37.153608 deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/type_stream.py
+-rw-r--r--   0        0        0      735 2023-02-28 15:59:51.000000 deepsecrets-1.0.5/deepsecrets/core/tokenizers/itokenizer.py
+-rw-r--r--   0        0        0     6481 2023-06-26 13:42:02.632935 deepsecrets-1.0.5/deepsecrets/core/tokenizers/lexer.py
+-rw-r--r--   0        0        0      600 2023-04-14 12:50:34.810801 deepsecrets-1.0.5/deepsecrets/core/tokenizers/per_line.py
+-rw-r--r--   0        0        0     1022 2023-04-14 12:50:38.878506 deepsecrets-1.0.5/deepsecrets/core/tokenizers/per_word.py
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.5/deepsecrets/core/utils/.DS_Store
+-rw-r--r--   0        0        0        0 2019-08-30 09:25:52.000000 deepsecrets-1.0.5/deepsecrets/core/utils/__init__.py
+-rw-r--r--   0        0        0      148 2023-02-10 10:44:34.000000 deepsecrets-1.0.5/deepsecrets/core/utils/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      586 2023-02-28 15:32:35.000000 deepsecrets-1.0.5/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc
+-rw-r--r--   0        0        0     5469 2023-03-27 20:23:09.183623 deepsecrets-1.0.5/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc
+-rw-r--r--   0        0        0     1415 2023-02-28 16:49:26.000000 deepsecrets-1.0.5/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc
+-rw-r--r--   0        0        0     1841 2023-06-26 16:37:09.047505 deepsecrets-1.0.5/deepsecrets/core/utils/__pycache__/guess_filetype.cpython-311.pyc
+-rw-r--r--   0        0        0     1774 2023-04-17 12:50:07.088140 deepsecrets-1.0.5/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc
+-rw-r--r--   0        0        0      100 2023-02-28 15:32:34.000000 deepsecrets-1.0.5/deepsecrets/core/utils/exceptions.py
+-rw-r--r--   0        0        0     3018 2023-03-27 20:23:08.288214 deepsecrets-1.0.5/deepsecrets/core/utils/file_analyzer.py
+-rw-r--r--   0        0        0      517 2023-02-28 16:47:36.000000 deepsecrets-1.0.5/deepsecrets/core/utils/fs.py
+-rw-r--r--   0        0        0     1060 2023-06-26 16:37:08.518447 deepsecrets-1.0.5/deepsecrets/core/utils/guess_filetype.py
+-rw-r--r--   0        0        0      771 2023-04-17 12:49:00.602766 deepsecrets-1.0.5/deepsecrets/core/utils/hashing.py
+-rw-r--r--   0        0        0     2562 2023-01-29 12:25:02.000000 deepsecrets-1.0.5/deepsecrets/rules/excluded_paths.json
+-rw-r--r--   0        0        0     3993 2023-06-26 12:38:43.101327 deepsecrets-1.0.5/deepsecrets/rules/regexes.json
+-rw-r--r--   0        0        0     6148 2023-02-26 15:19:47.000000 deepsecrets-1.0.5/deepsecrets/scan_modes/.DS_Store
+-rw-r--r--   0        0        0     5698 2023-04-17 13:42:10.557066 deepsecrets-1.0.5/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc
+-rw-r--r--   0        0        0     3268 2023-04-17 13:42:09.893195 deepsecrets-1.0.5/deepsecrets/scan_modes/cli.py
+-rw-r--r--   0        0        0     1646 2023-06-26 16:56:53.909334 deepsecrets-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6148 1970-01-01 00:00:00.000000 deepsecrets-1.0.5/PKG-INFO
```

### Comparing `deepsecrets-1.0.4/LICENSE` & `deepsecrets-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/README.md` & `deepsecrets-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/.DS_Store` & `deepsecrets-1.0.5/deepsecrets/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/__init__.py` & `deepsecrets-1.0.5/deepsecrets/__init__.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/cli.py` & `deepsecrets-1.0.5/deepsecrets/cli.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/config.py` & `deepsecrets-1.0.5/deepsecrets/config.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/.DS_Store` & `deepsecrets-1.0.5/deepsecrets/core/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/engines/__pycache__/hashed_secret.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/engines/__pycache__/iengine.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/engines/__pycache__/regex.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x0d4b3d64 (Mon Apr 17 13:35:09 2023 UTC)
+moddate:  0x2e869964 (Mon Jun 26 12:35:58 2023 UTC)
 files sz: 1196
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `deepsecrets-1.0.4/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/engines/__pycache__/semantic.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x314e3964 (Fri Apr 14 12:59:29 2023 UTC)
-files sz: 4333
+moddate:  0x62c29264 (Wed Jun 21 09:26:58 2023 UTC)
+files sz: 4341
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a01640064026c026d035a030100640064036c046d
@@ -148,15 +148,15 @@
           32          18 LOAD_CONST               2 (4.15)
                       20 STORE_NAME               4 (entropy_threshold)
          
           33          22 PUSH_NULL
                       24 LOAD_NAME                5 (re)
                       26 LOAD_ATTR                6 (compile)
          
-          34          36 LOAD_CONST               3 ('(secret|passw|\\bpass\\b|\\btoken\\b|\\baccess\\b|\\bpwd\\b|rivateke|cesstoke|authkey|\\bsecret\\b).{0,15}')
+          34          36 LOAD_CONST               3 ('(secret|passw|\\bpass\\b|\\btoken\\b|\\baccess\\b|\\bpwd\\b|rivateke|cesstoke|authkey|\\bsecret\\b|\\bkey\\b).{0,15}')
          
           35          38 LOAD_NAME                5 (re)
                       40 LOAD_ATTR                7 (IGNORECASE)
          
           33          50 PRECALL                  2
                       54 CALL                     2
                       64 STORE_NAME               8 (dangerous_variable_regex)
@@ -226,15 +226,15 @@
                      214 COPY                     1
                      216 STORE_NAME              23 (__classcell__)
                      218 RETURN_VALUE
          consts
             'SemanticEngine'
             'semantic'
             4.15
-            '(secret|passw|\\bpass\\b|\\btoken\\b|\\baccess\\b|\\bpwd\\b|rivateke|cesstoke|authkey|\\bsecret\\b).{0,15}'
+            '(secret|passw|\\bpass\\b|\\btoken\\b|\\baccess\\b|\\bpwd\\b|rivateke|cesstoke|authkey|\\bsecret\\b|\\bkey\\b).{0,15}'
             '^[^A-Za-z0-9]*$|^%.*%$|^\\[.*\\]$|^{.*}$'
             'subengine'
             'return'
             None
             code
                argcount  : 2
                nlocals   : 3
```

### Comparing `deepsecrets-1.0.4/deepsecrets/core/engines/hashed_secret.py` & `deepsecrets-1.0.5/deepsecrets/core/engines/hashed_secret.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/engines/iengine.py` & `deepsecrets-1.0.5/deepsecrets/core/engines/iengine.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/engines/regex.py` & `deepsecrets-1.0.5/deepsecrets/core/engines/regex.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/engines/semantic.py` & `deepsecrets-1.0.5/deepsecrets/core/engines/semantic.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 ]
 
 
 class SemanticEngine(IEngine):
     name = 'semantic'
     entropy_threshold = 4.15
     dangerous_variable_regex = re.compile(
-        r'(secret|passw|\bpass\b|\btoken\b|\baccess\b|\bpwd\b|rivateke|cesstoke|authkey|\bsecret\b).{0,15}',
+        r'(secret|passw|\bpass\b|\btoken\b|\baccess\b|\bpwd\b|rivateke|cesstoke|authkey|\bsecret\b|\bkey\b).{0,15}',
         re.IGNORECASE,
     )
     useless_value_regex = re.compile(r'^[^A-Za-z0-9]*$|^%.*%$|^\[.*\]$|^{.*}$', re.IGNORECASE)
     subengine: IEngine
 
     def __init__(self, subengine: IEngine, **kwargs) -> None:
         super().__init__(**kwargs)
```

### Comparing `deepsecrets-1.0.4/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc` & `deepsecrets-1.0.5/deepsecrets/core/helpers/__pycache__/content_analyzer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/helpers/__pycache__/entropy.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc` & `deepsecrets-1.0.5/deepsecrets/core/helpers/__pycache__/entropy.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/helpers/content_analyzer.py` & `deepsecrets-1.0.5/deepsecrets/core/helpers/content_analyzer.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/helpers/entropy.py` & `deepsecrets-1.0.5/deepsecrets/core/helpers/entropy.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/model/.DS_Store` & `deepsecrets-1.0.5/deepsecrets/core/model/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/model/__pycache__/file.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/model/__pycache__/file.cpython-311.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -1,19 +1,20 @@
 magic:    0xa70d0d0a
-moddate:  0xa1533964 (Fri Apr 14 13:22:41 2023 UTC)
-files sz: 3719
+moddate:  0x9f939964 (Mon Jun 26 13:33:19 2023 UTC)
+files sz: 4034
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a01640064026c026d035a036d045a046d055a0501
-      00640064036c066d075a070100640064046c086d095a0901000200470064
-      0584006406a6020000ab0200000000000000005a0a64015300
+      00640064036c066d075a070100640064046c086d095a090100640064056c
+      0a6d0b5a0b010002004700640684006407a6020000ab0200000000000000
+      005a0c64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (regex)
                  8 STORE_NAME               1 (re)
    
@@ -38,266 +39,292 @@
      5          42 LOAD_CONST               0 (0)
                 44 LOAD_CONST               4 (('get_abspath',))
                 46 IMPORT_NAME              8 (deepsecrets.core.utils.fs)
                 48 IMPORT_FROM              9 (get_abspath)
                 50 STORE_NAME               9 (get_abspath)
                 52 POP_TOP
    
-     8          54 PUSH_NULL
-                56 LOAD_BUILD_CLASS
-                58 LOAD_CONST               5 (<code object File, file "/app/deepsecrets/core/model/file.py", line 8>)
-                60 MAKE_FUNCTION            0
-                62 LOAD_CONST               6 ('File')
-                64 PRECALL                  2
-                68 CALL                     2
-                78 STORE_NAME              10 (File)
-                80 LOAD_CONST               1 (None)
-                82 RETURN_VALUE
+     6          54 LOAD_CONST               0 (0)
+                56 LOAD_CONST               5 (('FileTypeGuesser',))
+                58 IMPORT_NAME             10 (deepsecrets.core.utils.guess_filetype)
+                60 IMPORT_FROM             11 (FileTypeGuesser)
+                62 STORE_NAME              11 (FileTypeGuesser)
+                64 POP_TOP
+   
+     9          66 PUSH_NULL
+                68 LOAD_BUILD_CLASS
+                70 LOAD_CONST               6 (<code object File, file "/app/deepsecrets/core/model/file.py", line 9>)
+                72 MAKE_FUNCTION            0
+                74 LOAD_CONST               7 ('File')
+                76 PRECALL                  2
+                80 CALL                     2
+                90 STORE_NAME              12 (File)
+                92 LOAD_CONST               1 (None)
+                94 RETURN_VALUE
    consts
       0
       None
       ('Dict', 'Optional', 'Tuple')
       ('logger',)
       ('get_abspath',)
+      ('FileTypeGuesser',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 11
          flags     : 0
          code
             0x970065005a0164005a0255006503650464013c0000006503650464023c
             00000064035a056503650464043c0000006506650464053c00000069005a
             076508650665096506650666021900000000000000000066021900000000
             0000000000650464063c00000069005a0a65086506650366021900000000
             0000000000650464073c000000650b650464083c000000650c6503190000
-            00000000000000650464093c000000090009000900641c64026503640165
-            0c6503190000000000000000006404650c65031900000000000000000064
-            0b650c650819000000000000000000640c640a660a640d84055a0d640c65
-            0c6503190000000000000000006602640e84045a0e641d640f84045a0f64
-            0c65036602641084045a1064116506640c650c6506190000000000000000
-            006604641284045a1164116506640c650c65061900000000000000000066
-            04641384045a1264146506640c650c650319000000000000000000660464
-            1584045a1364166506640c650c6503190000000000000000006604641784
-            045a14641e641865036419650c6509650665066602190000000000000000
-            0019000000000000000000640c650c650965066506660219000000000000
-            000000190000000000000000006606641a84055a15640c65036602641b84
-            045a16640a5300
-           8           0 RESUME                   0
+            00000000000000650464093c000000650c65031900000000000000000065
+            04640a3c000000090009000900641e640265036401650c65031900000000
+            00000000006404650c650319000000000000000000640c650c6508190000
+            00000000000000640d640b660a640e84055a0d640d650c65031900000000
+            00000000006602640f84045a0e640d650c65031900000000000000000066
+            02641084045a0f641f641184045a10640d65036602641284045a11641365
+            06640d650c6506190000000000000000006604641484045a126413650664
+            0d650c6506190000000000000000006604641584045a1364166506640d65
+            0c6503190000000000000000006604641784045a1464186506640d650c65
+            03190000000000000000006604641984045a156420641a6503641b650c65
+            096506650666021900000000000000000019000000000000000000640d65
+            0c6509650665066602190000000000000000001900000000000000000066
+            06641c84055a16640d65036602641d84045a17640b5300
+           9           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('File')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-           9          12 LOAD_NAME                3 (str)
+          10          12 LOAD_NAME                3 (str)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('relative_path')
                       18 STORE_SUBSCR
          
-          10          22 LOAD_NAME                3 (str)
+          11          22 LOAD_NAME                3 (str)
                       24 LOAD_NAME                4 (__annotations__)
                       26 LOAD_CONST               2 ('path')
                       28 STORE_SUBSCR
          
-          11          32 LOAD_CONST               3 ('')
+          12          32 LOAD_CONST               3 ('')
                       34 STORE_NAME               5 (content)
                       36 LOAD_NAME                3 (str)
                       38 LOAD_NAME                4 (__annotations__)
                       40 LOAD_CONST               4 ('content')
                       42 STORE_SUBSCR
          
-          12          46 LOAD_NAME                6 (int)
+          13          46 LOAD_NAME                6 (int)
                       48 LOAD_NAME                4 (__annotations__)
                       50 LOAD_CONST               5 ('length')
                       52 STORE_SUBSCR
          
-          13          56 BUILD_MAP                0
+          14          56 BUILD_MAP                0
                       58 STORE_NAME               7 (line_offsets)
                       60 LOAD_NAME                8 (Dict)
                       62 LOAD_NAME                6 (int)
                       64 LOAD_NAME                9 (Tuple)
                       66 LOAD_NAME                6 (int)
                       68 LOAD_NAME                6 (int)
                       70 BUILD_TUPLE              2
                       72 BINARY_SUBSCR
                       82 BUILD_TUPLE              2
                       84 BINARY_SUBSCR
                       94 LOAD_NAME                4 (__annotations__)
                       96 LOAD_CONST               6 ('line_offsets')
                       98 STORE_SUBSCR
          
-          14         102 BUILD_MAP                0
+          15         102 BUILD_MAP                0
                      104 STORE_NAME              10 (line_contents_cache)
                      106 LOAD_NAME                8 (Dict)
                      108 LOAD_NAME                6 (int)
                      110 LOAD_NAME                3 (str)
                      112 BUILD_TUPLE              2
                      114 BINARY_SUBSCR
                      124 LOAD_NAME                4 (__annotations__)
                      126 LOAD_CONST               7 ('line_contents_cache')
                      128 STORE_SUBSCR
          
-          15         132 LOAD_NAME               11 (bool)
+          16         132 LOAD_NAME               11 (bool)
                      134 LOAD_NAME                4 (__annotations__)
                      136 LOAD_CONST               8 ('empty')
                      138 STORE_SUBSCR
          
-          16         142 LOAD_NAME               12 (Optional)
+          17         142 LOAD_NAME               12 (Optional)
                      144 LOAD_NAME                3 (str)
                      146 BINARY_SUBSCR
                      156 LOAD_NAME                4 (__annotations__)
                      158 LOAD_CONST               9 ('extension')
                      160 STORE_SUBSCR
          
-          21         164 NOP
-         
-          22         166 NOP
-         
-          23         168 NOP
-         
-          18         170 LOAD_CONST              28 ((None, None, None))
-                     172 LOAD_CONST               2 ('path')
-         
-          20         174 LOAD_NAME                3 (str)
-         
-          18         176 LOAD_CONST               1 ('relative_path')
-         
-          21         178 LOAD_NAME               12 (Optional)
-                     180 LOAD_NAME                3 (str)
-                     182 BINARY_SUBSCR
-         
-          18         192 LOAD_CONST               4 ('content')
-         
-          22         194 LOAD_NAME               12 (Optional)
-                     196 LOAD_NAME                3 (str)
-                     198 BINARY_SUBSCR
-         
-          18         208 LOAD_CONST              11 ('offsets')
-         
-          23         210 LOAD_NAME               12 (Optional)
-                     212 LOAD_NAME                8 (Dict)
-                     214 BINARY_SUBSCR
-         
-          18         224 LOAD_CONST              12 ('return')
-         
-          24         226 LOAD_CONST              10 (None)
-         
-          18         228 BUILD_TUPLE             10
-                     230 LOAD_CONST              13 (<code object __init__, file "/app/deepsecrets/core/model/file.py", line 18>)
-                     232 MAKE_FUNCTION            5 (defaults, annotations)
-                     234 STORE_NAME              13 (__init__)
-         
-          52         236 LOAD_CONST              12 ('return')
-                     238 LOAD_NAME               12 (Optional)
-                     240 LOAD_NAME                3 (str)
-                     242 BINARY_SUBSCR
-                     252 BUILD_TUPLE              2
-                     254 LOAD_CONST              14 (<code object _get_extension, file "/app/deepsecrets/core/model/file.py", line 52>)
-                     256 MAKE_FUNCTION            4 (annotations)
-                     258 STORE_NAME              14 (_get_extension)
-         
-          59         260 LOAD_CONST              29 (('return', None))
-                     262 LOAD_CONST              15 (<code object _calc_offsets, file "/app/deepsecrets/core/model/file.py", line 59>)
-                     264 MAKE_FUNCTION            4 (annotations)
-                     266 STORE_NAME              15 (_calc_offsets)
-         
-          68         268 LOAD_CONST              12 ('return')
-                     270 LOAD_NAME                3 (str)
-                     272 BUILD_TUPLE              2
-                     274 LOAD_CONST              16 (<code object _get_contents, file "/app/deepsecrets/core/model/file.py", line 68>)
-                     276 MAKE_FUNCTION            4 (annotations)
-                     278 STORE_NAME              16 (_get_contents)
-         
-          75         280 LOAD_CONST              17 ('position')
-                     282 LOAD_NAME                6 (int)
-                     284 LOAD_CONST              12 ('return')
-                     286 LOAD_NAME               12 (Optional)
-                     288 LOAD_NAME                6 (int)
-                     290 BINARY_SUBSCR
-                     300 BUILD_TUPLE              4
-                     302 LOAD_CONST              18 (<code object get_line_number, file "/app/deepsecrets/core/model/file.py", line 75>)
-                     304 MAKE_FUNCTION            4 (annotations)
-                     306 STORE_NAME              17 (get_line_number)
-         
-          78         308 LOAD_CONST              17 ('position')
-                     310 LOAD_NAME                6 (int)
-                     312 LOAD_CONST              12 ('return')
-                     314 LOAD_NAME               12 (Optional)
-                     316 LOAD_NAME                6 (int)
-                     318 BINARY_SUBSCR
-                     328 BUILD_TUPLE              4
-                     330 LOAD_CONST              19 (<code object _get_line_number_for_position, file "/app/deepsecrets/core/model/file.py", line 78>)
-                     332 MAKE_FUNCTION            4 (annotations)
-                     334 STORE_NAME              18 (_get_line_number_for_position)
-         
-          85         336 LOAD_CONST              20 ('line_number')
-                     338 LOAD_NAME                6 (int)
-                     340 LOAD_CONST              12 ('return')
-                     342 LOAD_NAME               12 (Optional)
-                     344 LOAD_NAME                3 (str)
-                     346 BINARY_SUBSCR
-                     356 BUILD_TUPLE              4
-                     358 LOAD_CONST              21 (<code object get_line_contents, file "/app/deepsecrets/core/model/file.py", line 85>)
-                     360 MAKE_FUNCTION            4 (annotations)
-                     362 STORE_NAME              19 (get_line_contents)
-         
-          95         364 LOAD_CONST              22 ('span_end')
-                     366 LOAD_NAME                6 (int)
-                     368 LOAD_CONST              12 ('return')
-                     370 LOAD_NAME               12 (Optional)
-                     372 LOAD_NAME                3 (str)
-                     374 BINARY_SUBSCR
-                     384 BUILD_TUPLE              4
-                     386 LOAD_CONST              23 (<code object get_full_line_for_position, file "/app/deepsecrets/core/model/file.py", line 95>)
-                     388 MAKE_FUNCTION            4 (annotations)
-                     390 STORE_NAME              20 (get_full_line_for_position)
-         
-         102         392 LOAD_CONST              30 ((None,))
-                     394 LOAD_CONST              24 ('str')
-                     396 LOAD_NAME                3 (str)
-                     398 LOAD_CONST              25 ('between')
-                     400 LOAD_NAME               12 (Optional)
-                     402 LOAD_NAME                9 (Tuple)
-                     404 LOAD_NAME                6 (int)
-                     406 LOAD_NAME                6 (int)
-                     408 BUILD_TUPLE              2
-                     410 BINARY_SUBSCR
+          18         164 LOAD_NAME               12 (Optional)
+                     166 LOAD_NAME                3 (str)
+                     168 BINARY_SUBSCR
+                     178 LOAD_NAME                4 (__annotations__)
+                     180 LOAD_CONST              10 ('guessed_extension')
+                     182 STORE_SUBSCR
+         
+          23         186 NOP
+         
+          24         188 NOP
+         
+          25         190 NOP
+         
+          20         192 LOAD_CONST              30 ((None, None, None))
+                     194 LOAD_CONST               2 ('path')
+         
+          22         196 LOAD_NAME                3 (str)
+         
+          20         198 LOAD_CONST               1 ('relative_path')
+         
+          23         200 LOAD_NAME               12 (Optional)
+                     202 LOAD_NAME                3 (str)
+                     204 BINARY_SUBSCR
+         
+          20         214 LOAD_CONST               4 ('content')
+         
+          24         216 LOAD_NAME               12 (Optional)
+                     218 LOAD_NAME                3 (str)
+                     220 BINARY_SUBSCR
+         
+          20         230 LOAD_CONST              12 ('offsets')
+         
+          25         232 LOAD_NAME               12 (Optional)
+                     234 LOAD_NAME                8 (Dict)
+                     236 BINARY_SUBSCR
+         
+          20         246 LOAD_CONST              13 ('return')
+         
+          26         248 LOAD_CONST              11 (None)
+         
+          20         250 BUILD_TUPLE             10
+                     252 LOAD_CONST              14 (<code object __init__, file "/app/deepsecrets/core/model/file.py", line 20>)
+                     254 MAKE_FUNCTION            5 (defaults, annotations)
+                     256 STORE_NAME              13 (__init__)
+         
+          57         258 LOAD_CONST              13 ('return')
+                     260 LOAD_NAME               12 (Optional)
+                     262 LOAD_NAME                3 (str)
+                     264 BINARY_SUBSCR
+                     274 BUILD_TUPLE              2
+                     276 LOAD_CONST              15 (<code object _get_extension, file "/app/deepsecrets/core/model/file.py", line 57>)
+                     278 MAKE_FUNCTION            4 (annotations)
+                     280 STORE_NAME              14 (_get_extension)
+         
+          64         282 LOAD_CONST              13 ('return')
+                     284 LOAD_NAME               12 (Optional)
+                     286 LOAD_NAME                3 (str)
+                     288 BINARY_SUBSCR
+                     298 BUILD_TUPLE              2
+                     300 LOAD_CONST              16 (<code object _try_guess_extension, file "/app/deepsecrets/core/model/file.py", line 64>)
+                     302 MAKE_FUNCTION            4 (annotations)
+                     304 STORE_NAME              15 (_try_guess_extension)
+         
+          67         306 LOAD_CONST              31 (('return', None))
+                     308 LOAD_CONST              17 (<code object _calc_offsets, file "/app/deepsecrets/core/model/file.py", line 67>)
+                     310 MAKE_FUNCTION            4 (annotations)
+                     312 STORE_NAME              16 (_calc_offsets)
+         
+          76         314 LOAD_CONST              13 ('return')
+                     316 LOAD_NAME                3 (str)
+                     318 BUILD_TUPLE              2
+                     320 LOAD_CONST              18 (<code object _get_contents, file "/app/deepsecrets/core/model/file.py", line 76>)
+                     322 MAKE_FUNCTION            4 (annotations)
+                     324 STORE_NAME              17 (_get_contents)
+         
+          83         326 LOAD_CONST              19 ('position')
+                     328 LOAD_NAME                6 (int)
+                     330 LOAD_CONST              13 ('return')
+                     332 LOAD_NAME               12 (Optional)
+                     334 LOAD_NAME                6 (int)
+                     336 BINARY_SUBSCR
+                     346 BUILD_TUPLE              4
+                     348 LOAD_CONST              20 (<code object get_line_number, file "/app/deepsecrets/core/model/file.py", line 83>)
+                     350 MAKE_FUNCTION            4 (annotations)
+                     352 STORE_NAME              18 (get_line_number)
+         
+          86         354 LOAD_CONST              19 ('position')
+                     356 LOAD_NAME                6 (int)
+                     358 LOAD_CONST              13 ('return')
+                     360 LOAD_NAME               12 (Optional)
+                     362 LOAD_NAME                6 (int)
+                     364 BINARY_SUBSCR
+                     374 BUILD_TUPLE              4
+                     376 LOAD_CONST              21 (<code object _get_line_number_for_position, file "/app/deepsecrets/core/model/file.py", line 86>)
+                     378 MAKE_FUNCTION            4 (annotations)
+                     380 STORE_NAME              19 (_get_line_number_for_position)
+         
+          93         382 LOAD_CONST              22 ('line_number')
+                     384 LOAD_NAME                6 (int)
+                     386 LOAD_CONST              13 ('return')
+                     388 LOAD_NAME               12 (Optional)
+                     390 LOAD_NAME                3 (str)
+                     392 BINARY_SUBSCR
+                     402 BUILD_TUPLE              4
+                     404 LOAD_CONST              23 (<code object get_line_contents, file "/app/deepsecrets/core/model/file.py", line 93>)
+                     406 MAKE_FUNCTION            4 (annotations)
+                     408 STORE_NAME              20 (get_line_contents)
+         
+         103         410 LOAD_CONST              24 ('span_end')
+                     412 LOAD_NAME                6 (int)
+                     414 LOAD_CONST              13 ('return')
+                     416 LOAD_NAME               12 (Optional)
+                     418 LOAD_NAME                3 (str)
                      420 BINARY_SUBSCR
-                     430 LOAD_CONST              12 ('return')
-                     432 LOAD_NAME               12 (Optional)
-                     434 LOAD_NAME                9 (Tuple)
-                     436 LOAD_NAME                6 (int)
-                     438 LOAD_NAME                6 (int)
-                     440 BUILD_TUPLE              2
-                     442 BINARY_SUBSCR
-                     452 BINARY_SUBSCR
-                     462 BUILD_TUPLE              6
-                     464 LOAD_CONST              26 (<code object get_span_for_string, file "/app/deepsecrets/core/model/file.py", line 102>)
-                     466 MAKE_FUNCTION            5 (defaults, annotations)
-                     468 STORE_NAME              21 (get_span_for_string)
-         
-         116         470 LOAD_CONST              12 ('return')
-                     472 LOAD_NAME                3 (str)
-                     474 BUILD_TUPLE              2
-                     476 LOAD_CONST              27 (<code object __repr__, file "/app/deepsecrets/core/model/file.py", line 116>)
-                     478 MAKE_FUNCTION            4 (annotations)
-                     480 STORE_NAME              22 (__repr__)
-                     482 LOAD_CONST              10 (None)
-                     484 RETURN_VALUE
+                     430 BUILD_TUPLE              4
+                     432 LOAD_CONST              25 (<code object get_full_line_for_position, file "/app/deepsecrets/core/model/file.py", line 103>)
+                     434 MAKE_FUNCTION            4 (annotations)
+                     436 STORE_NAME              21 (get_full_line_for_position)
+         
+         110         438 LOAD_CONST              32 ((None,))
+                     440 LOAD_CONST              26 ('str')
+                     442 LOAD_NAME                3 (str)
+                     444 LOAD_CONST              27 ('between')
+                     446 LOAD_NAME               12 (Optional)
+                     448 LOAD_NAME                9 (Tuple)
+                     450 LOAD_NAME                6 (int)
+                     452 LOAD_NAME                6 (int)
+                     454 BUILD_TUPLE              2
+                     456 BINARY_SUBSCR
+                     466 BINARY_SUBSCR
+                     476 LOAD_CONST              13 ('return')
+                     478 LOAD_NAME               12 (Optional)
+                     480 LOAD_NAME                9 (Tuple)
+                     482 LOAD_NAME                6 (int)
+                     484 LOAD_NAME                6 (int)
+                     486 BUILD_TUPLE              2
+                     488 BINARY_SUBSCR
+                     498 BINARY_SUBSCR
+                     508 BUILD_TUPLE              6
+                     510 LOAD_CONST              28 (<code object get_span_for_string, file "/app/deepsecrets/core/model/file.py", line 110>)
+                     512 MAKE_FUNCTION            5 (defaults, annotations)
+                     514 STORE_NAME              22 (get_span_for_string)
+         
+         124         516 LOAD_CONST              13 ('return')
+                     518 LOAD_NAME                3 (str)
+                     520 BUILD_TUPLE              2
+                     522 LOAD_CONST              29 (<code object __repr__, file "/app/deepsecrets/core/model/file.py", line 124>)
+                     524 MAKE_FUNCTION            4 (annotations)
+                     526 STORE_NAME              23 (__repr__)
+                     528 LOAD_CONST              11 (None)
+                     530 RETURN_VALUE
          consts
             'File'
             'relative_path'
             'path'
             ''
             'content'
             'length'
             'line_offsets'
             'line_contents_cache'
             'empty'
             'extension'
+            'guessed_extension'
             None
             'offsets'
             'return'
             code
                argcount  : 5
                nlocals   : 6
                stacksize : 4
@@ -311,74 +338,77 @@
                   000000a6000000ab0000000000000000007c005f0500000000000000006e
                   2b2300740e000000000000000000002400721e7d05741100000000000000
                   0000006a0900000000000000006401a6010000ab01000000000000000001
                   00590064007d057e056e0864007d057e0577017700780359007701741500
                   0000000000000000007c006a050000000000000000a6010000ab01000000
                   00000000007c005f0b00000000000000007c00a00c000000000000000000
                   0000000000000000000000a6000000ab0000000000000000007c005f0d00
-                  000000000000007c006a0b000000000000000064026b0200000000720264
-                  036e0164047c005f0e00000000000000007c0481077c047c005f00000000
-                  00000000007c006a0e0000000000000000732e7415000000000000000000
-                  007c006a000000000000000000a6010000ab01000000000000000064026b
-                  020000000072187c00a00f00000000000000000000000000000000000000
-                  00a6000000ab0000000000000000000100640053006400530064005300
-                18           0 RESUME                   0
+                  000000000000007c006a0d000000000000000080197c00a00e0000000000
+                  000000000000000000000000000000a6000000ab0000000000000000007c
+                  005f0f00000000000000007c006a0b000000000000000064026b02000000
+                  00720264036e0164047c005f1000000000000000007c0481077c047c005f
+                  0000000000000000007c006a100000000000000000732e74150000000000
+                  00000000007c006a000000000000000000a6010000ab0100000000000000
+                  0064026b020000000072187c00a011000000000000000000000000000000
+                  0000000000a6000000ab0000000000000000000100640053006400530064
+                  005300
+                20           0 RESUME                   0
                
-                25           2 BUILD_MAP                0
+                27           2 BUILD_MAP                0
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (line_offsets)
                
-                26          16 BUILD_MAP                0
+                28          16 BUILD_MAP                0
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               1 (line_contents_cache)
                
-                28          30 LOAD_FAST                1 (path)
+                30          30 LOAD_FAST                1 (path)
                             32 POP_JUMP_FORWARD_IF_NONE    20 (to 74)
                
-                29          34 LOAD_GLOBAL              5 (NULL + get_abspath)
+                31          34 LOAD_GLOBAL              5 (NULL + get_abspath)
                             46 LOAD_FAST                1 (path)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               3 (path)
                
-                31     >>   74 LOAD_FAST                2 (relative_path)
+                33     >>   74 LOAD_FAST                2 (relative_path)
                             76 POP_JUMP_FORWARD_IF_NONE     2 (to 82)
                             78 LOAD_FAST                2 (relative_path)
                             80 JUMP_FORWARD             6 (to 94)
                        >>   82 LOAD_FAST                0 (self)
                             84 LOAD_ATTR                3 (path)
                        >>   94 LOAD_FAST                0 (self)
                             96 STORE_ATTR               4 (relative_path)
                
-                33         106 LOAD_FAST                3 (content)
+                35         106 LOAD_FAST                3 (content)
                            108 POP_JUMP_FORWARD_IF_NONE     8 (to 126)
                
-                34         110 LOAD_FAST                3 (content)
+                36         110 LOAD_FAST                3 (content)
                            112 LOAD_FAST                0 (self)
                            114 STORE_ATTR               5 (content)
                            124 JUMP_FORWARD            70 (to 266)
                
-                36     >>  126 NOP
+                38     >>  126 NOP
                
-                37         128 LOAD_FAST                0 (self)
+                39         128 LOAD_FAST                0 (self)
                            130 LOAD_METHOD              6 (_get_contents)
                            152 PRECALL                  0
                            156 CALL                     0
                            166 LOAD_FAST                0 (self)
                            168 STORE_ATTR               5 (content)
                            178 JUMP_FORWARD            43 (to 266)
                        >>  180 PUSH_EXC_INFO
                
-                38         182 LOAD_GLOBAL             14 (Exception)
+                40         182 LOAD_GLOBAL             14 (Exception)
                            194 CHECK_EXC_MATCH
                            196 POP_JUMP_FORWARD_IF_FALSE    30 (to 258)
                            198 STORE_FAST               5 (e)
                
-                39         200 LOAD_GLOBAL             17 (NULL + logger)
+                41         200 LOAD_GLOBAL             17 (NULL + logger)
                            212 LOAD_ATTR                9 (error)
                            222 LOAD_CONST               1 ('Error during fetching file contents')
                            224 PRECALL                  1
                            228 CALL                     1
                            238 POP_TOP
                            240 POP_EXCEPT
                            242 LOAD_CONST               0 (None)
@@ -386,147 +416,188 @@
                            246 DELETE_FAST              5 (e)
                            248 JUMP_FORWARD             8 (to 266)
                        >>  250 LOAD_CONST               0 (None)
                            252 STORE_FAST               5 (e)
                            254 DELETE_FAST              5 (e)
                            256 RERAISE                  1
                
-                38     >>  258 RERAISE                  0
+                40     >>  258 RERAISE                  0
                        >>  260 COPY                     3
                            262 POP_EXCEPT
                            264 RERAISE                  1
                
-                41     >>  266 LOAD_GLOBAL             21 (NULL + len)
+                43     >>  266 LOAD_GLOBAL             21 (NULL + len)
                            278 LOAD_FAST                0 (self)
                            280 LOAD_ATTR                5 (content)
                            290 PRECALL                  1
                            294 CALL                     1
                            304 LOAD_FAST                0 (self)
                            306 STORE_ATTR              11 (length)
                
-                43         316 LOAD_FAST                0 (self)
+                45         316 LOAD_FAST                0 (self)
                            318 LOAD_METHOD             12 (_get_extension)
                            340 PRECALL                  0
                            344 CALL                     0
                            354 LOAD_FAST                0 (self)
                            356 STORE_ATTR              13 (extension)
                
-                44         366 LOAD_FAST                0 (self)
-                           368 LOAD_ATTR               11 (length)
-                           378 LOAD_CONST               2 (0)
-                           380 COMPARE_OP               2 (==)
-                           386 POP_JUMP_FORWARD_IF_FALSE     2 (to 392)
-                           388 LOAD_CONST               3 (True)
-                           390 JUMP_FORWARD             1 (to 394)
-                       >>  392 LOAD_CONST               4 (False)
-                       >>  394 LOAD_FAST                0 (self)
-                           396 STORE_ATTR              14 (empty)
-               
-                46         406 LOAD_FAST                4 (offsets)
-                           408 POP_JUMP_FORWARD_IF_NONE     7 (to 424)
-               
-                47         410 LOAD_FAST                4 (offsets)
-                           412 LOAD_FAST                0 (self)
-                           414 STORE_ATTR               0 (line_offsets)
-               
-                49     >>  424 LOAD_FAST                0 (self)
-                           426 LOAD_ATTR               14 (empty)
-                           436 POP_JUMP_FORWARD_IF_TRUE    46 (to 530)
-                           438 LOAD_GLOBAL             21 (NULL + len)
-                           450 LOAD_FAST                0 (self)
-                           452 LOAD_ATTR                0 (line_offsets)
-                           462 PRECALL                  1
-                           466 CALL                     1
-                           476 LOAD_CONST               2 (0)
-                           478 COMPARE_OP               2 (==)
-                           484 POP_JUMP_FORWARD_IF_FALSE    24 (to 534)
-               
-                50         486 LOAD_FAST                0 (self)
-                           488 LOAD_METHOD             15 (_calc_offsets)
-                           510 PRECALL                  0
-                           514 CALL                     0
-                           524 POP_TOP
-                           526 LOAD_CONST               0 (None)
-                           528 RETURN_VALUE
-               
-                49     >>  530 LOAD_CONST               0 (None)
-                           532 RETURN_VALUE
-                       >>  534 LOAD_CONST               0 (None)
-                           536 RETURN_VALUE
+                46         366 LOAD_FAST                0 (self)
+                           368 LOAD_ATTR               13 (extension)
+                           378 POP_JUMP_FORWARD_IF_NOT_NONE    25 (to 430)
+               
+                47         380 LOAD_FAST                0 (self)
+                           382 LOAD_METHOD             14 (_try_guess_extension)
+                           404 PRECALL                  0
+                           408 CALL                     0
+                           418 LOAD_FAST                0 (self)
+                           420 STORE_ATTR              15 (guessed_extension)
+               
+                49     >>  430 LOAD_FAST                0 (self)
+                           432 LOAD_ATTR               11 (length)
+                           442 LOAD_CONST               2 (0)
+                           444 COMPARE_OP               2 (==)
+                           450 POP_JUMP_FORWARD_IF_FALSE     2 (to 456)
+                           452 LOAD_CONST               3 (True)
+                           454 JUMP_FORWARD             1 (to 458)
+                       >>  456 LOAD_CONST               4 (False)
+                       >>  458 LOAD_FAST                0 (self)
+                           460 STORE_ATTR              16 (empty)
+               
+                51         470 LOAD_FAST                4 (offsets)
+                           472 POP_JUMP_FORWARD_IF_NONE     7 (to 488)
+               
+                52         474 LOAD_FAST                4 (offsets)
+                           476 LOAD_FAST                0 (self)
+                           478 STORE_ATTR               0 (line_offsets)
+               
+                54     >>  488 LOAD_FAST                0 (self)
+                           490 LOAD_ATTR               16 (empty)
+                           500 POP_JUMP_FORWARD_IF_TRUE    46 (to 594)
+                           502 LOAD_GLOBAL             21 (NULL + len)
+                           514 LOAD_FAST                0 (self)
+                           516 LOAD_ATTR                0 (line_offsets)
+                           526 PRECALL                  1
+                           530 CALL                     1
+                           540 LOAD_CONST               2 (0)
+                           542 COMPARE_OP               2 (==)
+                           548 POP_JUMP_FORWARD_IF_FALSE    24 (to 598)
+               
+                55         550 LOAD_FAST                0 (self)
+                           552 LOAD_METHOD             17 (_calc_offsets)
+                           574 PRECALL                  0
+                           578 CALL                     0
+                           588 POP_TOP
+                           590 LOAD_CONST               0 (None)
+                           592 RETURN_VALUE
+               
+                54     >>  594 LOAD_CONST               0 (None)
+                           596 RETURN_VALUE
+                       >>  598 LOAD_CONST               0 (None)
+                           600 RETURN_VALUE
                ExceptionTable:
                  128 to 176 -> 180 [0]
                  180 to 198 -> 260 [1] lasti
                  200 to 238 -> 250 [1] lasti
                  250 to 258 -> 260 [1] lasti
                consts
                   None
                   'Error during fetching file contents'
                   0
                   True
                   False
-               names      ('line_offsets', 'line_contents_cache', 'get_abspath', 'path', 'relative_path', 'content', '_get_contents', 'Exception', 'logger', 'error', 'len', 'length', '_get_extension', 'extension', 'empty', '_calc_offsets')
+               names      ('line_offsets', 'line_contents_cache', 'get_abspath', 'path', 'relative_path', 'content', '_get_contents', 'Exception', 'logger', 'error', 'len', 'length', '_get_extension', 'extension', '_try_guess_extension', 'guessed_extension', 'empty', '_calc_offsets')
                varnames   ('self', 'path', 'relative_path', 'content', 'offsets', 'e')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/model/file.py'
                name       '__init__'
-               firstlineno 18
+               firstlineno 20
                lnotab
                   0x02070e010e02040128022002040110020201360112013aff0803320232
-                  01280204010e023e012cff
+                  010e013202280204010e023e012cff
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab0100000000000000007d017405000000
                   000000000000007c01a6010000ab01000000000000000064026b02000000
                   007202640053007c016403190000000000000000005300
-                52           0 RESUME                   0
+                57           0 RESUME                   0
                
-                53           2 LOAD_FAST                0 (self)
+                58           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (path)
                             14 LOAD_METHOD              1 (split)
                             36 LOAD_CONST               1 ('.')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               1 (by_dot)
                
-                54          54 LOAD_GLOBAL              5 (NULL + len)
+                59          54 LOAD_GLOBAL              5 (NULL + len)
                             66 LOAD_FAST                1 (by_dot)
                             68 PRECALL                  1
                             72 CALL                     1
                             82 LOAD_CONST               2 (1)
                             84 COMPARE_OP               2 (==)
                             90 POP_JUMP_FORWARD_IF_FALSE     2 (to 96)
                
-                55          92 LOAD_CONST               0 (None)
+                60          92 LOAD_CONST               0 (None)
                             94 RETURN_VALUE
                
-                57     >>   96 LOAD_FAST                1 (by_dot)
+                62     >>   96 LOAD_FAST                1 (by_dot)
                             98 LOAD_CONST               3 (-1)
                            100 BINARY_SUBSCR
                            110 RETURN_VALUE
                consts
                   None
                   '.'
                   1
                   -1
                names      ('path', 'split', 'len')
                varnames   ('self', 'by_dot')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/model/file.py'
                name       '_get_extension'
-               firstlineno 52
+               firstlineno 57
                lnotab 0x0201340126010402
             code
                argcount  : 1
+               nlocals   : 1
+               stacksize : 3
+               flags     : 3
+               code
+                  0x9700740100000000000000000000a6000000ab000000000000000000a0
+                  0100000000000000000000000000000000000000007c006a020000000000
+                  000000a6010000ab0100000000000000005300
+                64           0 RESUME                   0
+               
+                65           2 LOAD_GLOBAL              1 (NULL + FileTypeGuesser)
+                            14 PRECALL                  0
+                            18 CALL                     0
+                            28 LOAD_METHOD              1 (guess)
+                            50 LOAD_FAST                0 (self)
+                            52 LOAD_ATTR                2 (content)
+                            62 PRECALL                  1
+                            66 CALL                     1
+                            76 RETURN_VALUE
+               consts
+                  None
+               names      ('FileTypeGuesser', 'guess', 'content')
+               varnames   ('self',)
+               freevars   ()
+               cellvars   ()
+               filename   '/app/deepsecrets/core/model/file.py'
+               name       '_try_guess_extension'
+               firstlineno 64
+               lnotab 0x0201
+            code
+               argcount  : 1
                nlocals   : 5
                stacksize : 5
                flags     : 3
                code
                   0x9700640184007401000000000000000000006a01000000000000000064
                   027c006a020000000000000000a6020000ab0200000000000000004400a6
                   000000ab0000000000000000007d017407000000000000000000007c01a6
@@ -534,106 +605,106 @@
                   0400000000720e7c017c0264047a0a00001900000000000000000064047a
                   0000006e0164037d047c047c0366027c006a0400000000000000007c0264
                   047a0000003c0000008c2b740b000000000000000000007c006a04000000
                   0000000000a6010000ab01000000000000000064036b0200000000721e7c
                   006a06000000000000000064036b0400000000721564037c006a06000000
                   000000000066027c006a04000000000000000064043c0000006400530064
                   00530064005300
-                59           0 RESUME                   0
+                67           0 RESUME                   0
                
-                60           2 LOAD_CONST               1 (<code object <listcomp>, file "/app/deepsecrets/core/model/file.py", line 60>)
+                68           2 LOAD_CONST               1 (<code object <listcomp>, file "/app/deepsecrets/core/model/file.py", line 68>)
                              4 MAKE_FUNCTION            0
                              6 LOAD_GLOBAL              1 (NULL + re)
                             18 LOAD_ATTR                1 (finditer)
                             28 LOAD_CONST               2 ('\n')
                             30 LOAD_FAST                0 (self)
                             32 LOAD_ATTR                2 (content)
                             42 PRECALL                  2
                             46 CALL                     2
                             56 GET_ITER
                             58 PRECALL                  0
                             62 CALL                     0
                             72 STORE_FAST               1 (line_breaks)
                
-                61          74 LOAD_GLOBAL              7 (NULL + enumerate)
+                69          74 LOAD_GLOBAL              7 (NULL + enumerate)
                             86 LOAD_FAST                1 (line_breaks)
                             88 PRECALL                  1
                             92 CALL                     1
                            102 GET_ITER
                        >>  104 FOR_ITER                42 (to 190)
                            106 UNPACK_SEQUENCE          2
                            110 STORE_FAST               2 (i)
                            112 STORE_FAST               3 (lb)
                
-                62         114 LOAD_FAST                2 (i)
+                70         114 LOAD_FAST                2 (i)
                            116 LOAD_CONST               3 (0)
                            118 COMPARE_OP               4 (>)
                            124 POP_JUMP_FORWARD_IF_FALSE    14 (to 154)
                            126 LOAD_FAST                1 (line_breaks)
                            128 LOAD_FAST                2 (i)
                            130 LOAD_CONST               4 (1)
                            132 BINARY_OP               10 (-)
                            136 BINARY_SUBSCR
                            146 LOAD_CONST               4 (1)
                            148 BINARY_OP                0 (+)
                            152 JUMP_FORWARD             1 (to 156)
                        >>  154 LOAD_CONST               3 (0)
                        >>  156 STORE_FAST               4 (start)
                
-                63         158 LOAD_FAST                4 (start)
+                71         158 LOAD_FAST                4 (start)
                            160 LOAD_FAST                3 (lb)
                            162 BUILD_TUPLE              2
                            164 LOAD_FAST                0 (self)
                            166 LOAD_ATTR                4 (line_offsets)
                            176 LOAD_FAST                2 (i)
                            178 LOAD_CONST               4 (1)
                            180 BINARY_OP                0 (+)
                            184 STORE_SUBSCR
                            188 JUMP_BACKWARD           43 (to 104)
                
-                65     >>  190 LOAD_GLOBAL             11 (NULL + len)
+                73     >>  190 LOAD_GLOBAL             11 (NULL + len)
                            202 LOAD_FAST                0 (self)
                            204 LOAD_ATTR                4 (line_offsets)
                            214 PRECALL                  1
                            218 CALL                     1
                            228 LOAD_CONST               3 (0)
                            230 COMPARE_OP               2 (==)
                            236 POP_JUMP_FORWARD_IF_FALSE    30 (to 298)
                            238 LOAD_FAST                0 (self)
                            240 LOAD_ATTR                6 (length)
                            250 LOAD_CONST               3 (0)
                            252 COMPARE_OP               4 (>)
                            258 POP_JUMP_FORWARD_IF_FALSE    21 (to 302)
                
-                66         260 LOAD_CONST               3 (0)
+                74         260 LOAD_CONST               3 (0)
                            262 LOAD_FAST                0 (self)
                            264 LOAD_ATTR                6 (length)
                            274 BUILD_TUPLE              2
                            276 LOAD_FAST                0 (self)
                            278 LOAD_ATTR                4 (line_offsets)
                            288 LOAD_CONST               4 (1)
                            290 STORE_SUBSCR
                            294 LOAD_CONST               0 (None)
                            296 RETURN_VALUE
                
-                65     >>  298 LOAD_CONST               0 (None)
+                73     >>  298 LOAD_CONST               0 (None)
                            300 RETURN_VALUE
                        >>  302 LOAD_CONST               0 (None)
                            304 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 4
                      flags     : 19
                      code
                         0x970067007c005d167d017c01a000000000000000000000000000000000
                         0000000000a6000000ab00000000000000000091028c175300
-                      60           0 RESUME                   0
+                      68           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                22 (to 52)
                                    8 STORE_FAST               1 (i)
                                   10 LOAD_FAST                1 (i)
                                   12 LOAD_METHOD              0 (start)
                                   34 PRECALL                  0
@@ -644,70 +715,70 @@
                      consts
                      names      ('start',)
                      varnames   ('.0', 'i')
                      freevars   ()
                      cellvars   ()
                      filename   '/app/deepsecrets/core/model/file.py'
                      name       '<listcomp>'
-                     firstlineno 60
+                     firstlineno 68
                      lnotab 0x
                   '\n'
                   0
                   1
                names      ('re', 'finditer', 'content', 'enumerate', 'line_offsets', 'len', 'length')
                varnames   ('self', 'line_breaks', 'i', 'lb', 'start')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/model/file.py'
                name       '_calc_offsets'
-               firstlineno 59
+               firstlineno 67
                lnotab 0x0201480128012c012002460126ff
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 6
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab01000000000000000035007d017c01a0020000000000000000000000
                   000000000000000000a6000000ab0000000000000000007d027c02640119
                   00000000000000000064026b030000000072057c0264027a0d00007d027c
                   026302640064006400a6020000ab02000000000000000001005300230031
                   0073047702780359007701010059000100010064005300
-                68           0 RESUME                   0
+                76           0 RESUME                   0
                
-                69           2 LOAD_GLOBAL              1 (NULL + open)
+                77           2 LOAD_GLOBAL              1 (NULL + open)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (path)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 BEFORE_WITH
                             42 STORE_FAST               1 (f)
                
-                70          44 LOAD_FAST                1 (f)
+                78          44 LOAD_FAST                1 (f)
                             46 LOAD_METHOD              2 (read)
                             68 PRECALL                  0
                             72 CALL                     0
                             82 STORE_FAST               2 (raw)
                
-                71          84 LOAD_FAST                2 (raw)
+                79          84 LOAD_FAST                2 (raw)
                             86 LOAD_CONST               1 (-1)
                             88 BINARY_SUBSCR
                             98 LOAD_CONST               2 ('\n')
                            100 COMPARE_OP               3 (!=)
                            106 POP_JUMP_FORWARD_IF_FALSE     5 (to 118)
                
-                72         108 LOAD_FAST                2 (raw)
+                80         108 LOAD_FAST                2 (raw)
                            110 LOAD_CONST               2 ('\n')
                            112 BINARY_OP               13 (+=)
                            116 STORE_FAST               2 (raw)
                
-                73     >>  118 LOAD_FAST                2 (raw)
+                81     >>  118 LOAD_FAST                2 (raw)
                
-                69         120 SWAP                     2
+                77         120 SWAP                     2
                            122 LOAD_CONST               0 (None)
                            124 LOAD_CONST               0 (None)
                            126 LOAD_CONST               0 (None)
                            128 PRECALL                  2
                            132 CALL                     2
                            142 POP_TOP
                            144 RETURN_VALUE
@@ -734,28 +805,28 @@
                   '\n'
                names      ('open', 'path', 'read')
                varnames   ('self', 'f', 'raw')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/model/file.py'
                name       '_get_contents'
-               firstlineno 68
+               firstlineno 76
                lnotab 0x02012a01280118010a0102fc
             'position'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c01ac
                   01a6010000ab0100000000000000005300
-                75           0 RESUME                   0
+                83           0 RESUME                   0
                
-                76           2 LOAD_FAST                0 (self)
+                84           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (_get_line_number_for_position)
                             26 LOAD_FAST                1 (position)
                             28 KW_NAMES                 1
                             30 PRECALL                  1
                             34 CALL                     1
                             44 RETURN_VALUE
                consts
@@ -763,174 +834,174 @@
                   ('position',)
                names      ('_get_line_number_for_position',)
                varnames   ('self', 'position')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/model/file.py'
                name       'get_line_number'
-               firstlineno 75
+               firstlineno 83
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000a6000000ab00000000000000000044005d155c0200007d
                   027d037c036401190000000000000000007c016b000000000072018c127c
                   0263020100530064005300
-                78           0 RESUME                   0
+                86           0 RESUME                   0
                
-                79           2 LOAD_FAST                0 (self)
+                87           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (line_offsets)
                             14 LOAD_METHOD              1 (items)
                             36 PRECALL                  0
                             40 CALL                     0
                             50 GET_ITER
                        >>   52 FOR_ITER                21 (to 96)
                             54 UNPACK_SEQUENCE          2
                             58 STORE_FAST               2 (linum)
                             60 STORE_FAST               3 (offsets)
                
-                80          62 LOAD_FAST                3 (offsets)
+                88          62 LOAD_FAST                3 (offsets)
                             64 LOAD_CONST               1 (1)
                             66 BINARY_SUBSCR
                             76 LOAD_FAST                1 (position)
                             78 COMPARE_OP               0 (<)
                             84 POP_JUMP_FORWARD_IF_FALSE     1 (to 88)
                
-                81          86 JUMP_BACKWARD           18 (to 52)
+                89          86 JUMP_BACKWARD           18 (to 52)
                
-                82     >>   88 LOAD_FAST                2 (linum)
+                90     >>   88 LOAD_FAST                2 (linum)
                             90 SWAP                     2
                             92 POP_TOP
                             94 RETURN_VALUE
                
-                83     >>   96 LOAD_CONST               0 (None)
+                91     >>   96 LOAD_CONST               0 (None)
                             98 RETURN_VALUE
                consts
                   None
                   1
                names      ('line_offsets', 'items')
                varnames   ('self', 'position', 'linum', 'offsets')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/model/file.py'
                name       '_get_line_number_for_position'
-               firstlineno 78
+               firstlineno 86
                lnotab 0x02013c01180102010801
             'line_number'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
                flags     : 3
                code
                   0x97007c018002640053007c017c006a000000000000000000760172397c
                   006a0100000000000000007c006a0200000000000000007c011900000000
                   00000000006401190000000000000000007c006a0200000000000000007c
                   011900000000000000000064021900000000000000000085021900000000
                   00000000007c006a0000000000000000007c013c0000007c006a00000000
                   00000000007c01190000000000000000005300
-                85           0 RESUME                   0
+                93           0 RESUME                   0
                
-                86           2 LOAD_FAST                1 (line_number)
+                94           2 LOAD_FAST                1 (line_number)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 10)
                
-                87           6 LOAD_CONST               0 (None)
+                95           6 LOAD_CONST               0 (None)
                              8 RETURN_VALUE
                
-                89     >>   10 LOAD_FAST                1 (line_number)
+                97     >>   10 LOAD_FAST                1 (line_number)
                             12 LOAD_FAST                0 (self)
                             14 LOAD_ATTR                0 (line_contents_cache)
                             24 CONTAINS_OP              1
                             26 POP_JUMP_FORWARD_IF_FALSE    57 (to 142)
                
-                90          28 LOAD_FAST                0 (self)
+                98          28 LOAD_FAST                0 (self)
                             30 LOAD_ATTR                1 (content)
                
-                91          40 LOAD_FAST                0 (self)
+                99          40 LOAD_FAST                0 (self)
                             42 LOAD_ATTR                2 (line_offsets)
                             52 LOAD_FAST                1 (line_number)
                             54 BINARY_SUBSCR
                             64 LOAD_CONST               1 (0)
                             66 BINARY_SUBSCR
                             76 LOAD_FAST                0 (self)
                             78 LOAD_ATTR                2 (line_offsets)
                             88 LOAD_FAST                1 (line_number)
                             90 BINARY_SUBSCR
                            100 LOAD_CONST               2 (1)
                            102 BINARY_SUBSCR
                            112 BUILD_SLICE              2
                
-                90         114 BINARY_SUBSCR
+                98         114 BINARY_SUBSCR
                            124 LOAD_FAST                0 (self)
                            126 LOAD_ATTR                0 (line_contents_cache)
                            136 LOAD_FAST                1 (line_number)
                            138 STORE_SUBSCR
                
-                93     >>  142 LOAD_FAST                0 (self)
+               101     >>  142 LOAD_FAST                0 (self)
                            144 LOAD_ATTR                0 (line_contents_cache)
                            154 LOAD_FAST                1 (line_number)
                            156 BINARY_SUBSCR
                            166 RETURN_VALUE
                consts
                   None
                   0
                   1
                names      ('line_contents_cache', 'content', 'line_offsets')
                varnames   ('self', 'line_number')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/model/file.py'
                name       'get_line_contents'
-               firstlineno 85
+               firstlineno 93
                lnotab 0x02010401040212010c014aff1c03
             'span_end'
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c01a6
                   010000ab0100000000000000007d027c028002640053007c00a001000000
                   00000000000000000000000000000000007c02a6010000ab010000000000
                   0000005300
-                95           0 RESUME                   0
+               103           0 RESUME                   0
                
-                96           2 LOAD_FAST                0 (self)
+               104           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (_get_line_number_for_position)
                             26 LOAD_FAST                1 (span_end)
                             28 PRECALL                  1
                             32 CALL                     1
                             42 STORE_FAST               2 (linum)
                
-                97          44 LOAD_FAST                2 (linum)
+               105          44 LOAD_FAST                2 (linum)
                             46 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 52)
                
-                98          48 LOAD_CONST               0 (None)
+               106          48 LOAD_CONST               0 (None)
                             50 RETURN_VALUE
                
-               100     >>   52 LOAD_FAST                0 (self)
+               108     >>   52 LOAD_FAST                0 (self)
                             54 LOAD_METHOD              1 (get_line_contents)
                             76 LOAD_FAST                2 (linum)
                             78 PRECALL                  1
                             82 CALL                     1
                             92 RETURN_VALUE
                consts
                   None
                names      ('_get_line_number_for_position', 'get_line_contents')
                varnames   ('self', 'span_end', 'linum')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/model/file.py'
                name       'get_full_line_for_position'
-               firstlineno 95
+               firstlineno 103
                lnotab 0x02012a0104010402
             'str'
             'between'
             code
                argcount  : 3
                nlocals   : 8
                stacksize : 5
@@ -945,77 +1016,77 @@
                   00000064056406a6020000ab0200000000000000007d0474050000000000
                   00000000006a0500000000000000007c047c03a6020000ab020000000000
                   0000007d057c0544005d397d067c06a00600000000000000000000000000
                   00000000000000a6000000ab0000000000000000007d077c026401190000
                   000000000000007c076401190000000000000000007a0000007c02640119
                   0000000000000000007c076402190000000000000000007a000000660263
                   020100530064005300
-               102           0 RESUME                   0
+               110           0 RESUME                   0
                
-               103           2 LOAD_FAST                2 (between)
+               111           2 LOAD_FAST                2 (between)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     9 (to 24)
                
-               104           6 LOAD_CONST               1 (0)
+               112           6 LOAD_CONST               1 (0)
                              8 LOAD_FAST                0 (self)
                             10 LOAD_ATTR                0 (length)
                             20 BUILD_TUPLE              2
                             22 STORE_FAST               2 (between)
                
-               106     >>   24 LOAD_FAST                0 (self)
+               114     >>   24 LOAD_FAST                0 (self)
                             26 LOAD_ATTR                1 (content)
                             36 LOAD_FAST                2 (between)
                             38 LOAD_CONST               1 (0)
                             40 BINARY_SUBSCR
                             50 LOAD_FAST                2 (between)
                             52 LOAD_CONST               2 (1)
                             54 BINARY_SUBSCR
                             64 BUILD_SLICE              2
                             66 BINARY_SUBSCR
                             76 STORE_FAST               3 (search_window)
                
-               108          78 LOAD_GLOBAL              5 (NULL + re)
+               116          78 LOAD_GLOBAL              5 (NULL + re)
                             90 LOAD_ATTR                3 (escape)
                            100 LOAD_FAST                1 (str)
                            102 PRECALL                  1
                            106 CALL                     1
                            116 STORE_FAST               4 (pattern)
                
-               109         118 LOAD_FAST                4 (pattern)
+               117         118 LOAD_FAST                4 (pattern)
                            120 LOAD_METHOD              4 (replace)
                            142 LOAD_CONST               3 ('\\\n')
                            144 LOAD_CONST               4 ('\n')
                            146 PRECALL                  2
                            150 CALL                     2
                            160 LOAD_METHOD              4 (replace)
                            182 LOAD_CONST               5 ('\\\t')
                            184 LOAD_CONST               6 ('\t')
                            186 PRECALL                  2
                            190 CALL                     2
                            200 STORE_FAST               4 (pattern)
                
-               110         202 LOAD_GLOBAL              5 (NULL + re)
+               118         202 LOAD_GLOBAL              5 (NULL + re)
                            214 LOAD_ATTR                5 (finditer)
                            224 LOAD_FAST                4 (pattern)
                            226 LOAD_FAST                3 (search_window)
                            228 PRECALL                  2
                            232 CALL                     2
                            242 STORE_FAST               5 (detects)
                
-               111         244 LOAD_FAST                5 (detects)
+               119         244 LOAD_FAST                5 (detects)
                            246 GET_ITER
                            248 FOR_ITER                57 (to 364)
                            250 STORE_FAST               6 (detect)
                
-               112         252 LOAD_FAST                6 (detect)
+               120         252 LOAD_FAST                6 (detect)
                            254 LOAD_METHOD              6 (span)
                            276 PRECALL                  0
                            280 CALL                     0
                            290 STORE_FAST               7 (span)
                
-               113         292 LOAD_FAST                2 (between)
+               121         292 LOAD_FAST                2 (between)
                            294 LOAD_CONST               1 (0)
                            296 BINARY_SUBSCR
                            306 LOAD_FAST                7 (span)
                            308 LOAD_CONST               1 (0)
                            310 BINARY_SUBSCR
                            320 BINARY_OP                0 (+)
                            324 LOAD_FAST                2 (between)
@@ -1026,15 +1097,15 @@
                            342 BINARY_SUBSCR
                            352 BINARY_OP                0 (+)
                            356 BUILD_TUPLE              2
                            358 SWAP                     2
                            360 POP_TOP
                            362 RETURN_VALUE
                
-               114     >>  364 LOAD_CONST               0 (None)
+               122     >>  364 LOAD_CONST               0 (None)
                            366 RETURN_VALUE
                consts
                   None
                   0
                   1
                   '\\\n'
                   '\n'
@@ -1042,53 +1113,53 @@
                   '\t'
                names      ('length', 'content', 're', 'escape', 'replace', 'finditer', 'span')
                varnames   ('self', 'str', 'between', 'search_window', 'pattern', 'detects', 'detect', 'span')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/model/file.py'
                name       'get_span_for_string'
-               firstlineno 102
+               firstlineno 110
                lnotab 0x0201040112023602280154012a01080128014801
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000005300
-               116           0 RESUME                   0
+               124           0 RESUME                   0
                
-               117           2 LOAD_FAST                0 (self)
+               125           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (path)
                             14 RETURN_VALUE
                consts
                   None
                names      ('path',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/model/file.py'
                name       '__repr__'
-               firstlineno 116
+               firstlineno 124
                lnotab 0x0201
             (None, None, None)
             ('return', None)
             (None,)
-         names      ('__name__', '__module__', '__qualname__', 'str', '__annotations__', 'content', 'int', 'line_offsets', 'Dict', 'Tuple', 'line_contents_cache', 'bool', 'Optional', '__init__', '_get_extension', '_calc_offsets', '_get_contents', 'get_line_number', '_get_line_number_for_position', 'get_line_contents', 'get_full_line_for_position', 'get_span_for_string', '__repr__')
+         names      ('__name__', '__module__', '__qualname__', 'str', '__annotations__', 'content', 'int', 'line_offsets', 'Dict', 'Tuple', 'line_contents_cache', 'bool', 'Optional', '__init__', '_get_extension', '_try_guess_extension', '_calc_offsets', '_get_contents', 'get_line_number', '_get_line_number_for_position', 'get_line_contents', 'get_full_line_for_position', 'get_span_for_string', '__repr__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/app/deepsecrets/core/model/file.py'
          name       'File'
-         firstlineno 8
+         firstlineno 9
          lnotab
-            0x0c010a010a010e010a012e011e010a0116050201020102fb040202fe02
-            030efd02040efc02050efb020602fa0822180708090c071c031c071c0a1c
-            074e0e
+            0x0c010a010a010e010a012e011e010a01160116050201020102fb040202
+            fe02030efd02040efc02050efb020602fa08251807180308090c071c031c
+            071c0a1c074e0e
       'File'
-   names      ('regex', 're', 'typing', 'Dict', 'Optional', 'Tuple', 'deepsecrets', 'logger', 'deepsecrets.core.utils.fs', 'get_abspath', 'File')
+   names      ('regex', 're', 'typing', 'Dict', 'Optional', 'Tuple', 'deepsecrets', 'logger', 'deepsecrets.core.utils.fs', 'get_abspath', 'deepsecrets.core.utils.guess_filetype', 'FileTypeGuesser', 'File')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/app/deepsecrets/core/model/file.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff0201080114020c010c03
+   lnotab 0x00ff0201080114020c010c010c03
```

### Comparing `deepsecrets-1.0.4/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/model/__pycache__/finding.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/model/__pycache__/semantic.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/model/__pycache__/semantic.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/model/__pycache__/token.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/model/__pycache__/token.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/model/file.py` & `deepsecrets-1.0.5/deepsecrets/core/model/file.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import regex as re
 from typing import Dict, Optional, Tuple
 
 from deepsecrets import logger
 from deepsecrets.core.utils.fs import get_abspath
+from deepsecrets.core.utils.guess_filetype import FileTypeGuesser
 
 
 class File:
     relative_path: str
     path: str
     content: str = ''
     length: int
     line_offsets: Dict[int, Tuple[int, int]] = {}
     line_contents_cache: Dict[int, str] = {}
     empty: bool
     extension: Optional[str]
+    guessed_extension: Optional[str]
 
     def __init__(
         self,
         path: str,
         relative_path: Optional[str] = None,
         content: Optional[str] = None,
         offsets: Optional[Dict] = None,
@@ -37,28 +39,34 @@
                 self.content = self._get_contents()
             except Exception as e:
                 logger.error('Error during fetching file contents')
 
         self.length = len(self.content)
 
         self.extension = self._get_extension()
+        if self.extension is None:
+            self.guessed_extension = self._try_guess_extension()
+
         self.empty = True if self.length == 0 else False
 
         if offsets is not None:
             self.line_offsets = offsets
 
         if not self.empty and len(self.line_offsets) == 0:
             self._calc_offsets()
 
     def _get_extension(self) -> Optional[str]:
         by_dot = self.path.split('.')
         if len(by_dot) == 1:
             return None
 
         return by_dot[-1]
+    
+    def _try_guess_extension(self) -> Optional[str]:
+        return FileTypeGuesser().guess(self.content)
 
     def _calc_offsets(self) -> None:
         line_breaks = [i.start() for i in re.finditer('\n', self.content)]
         for i, lb in enumerate(line_breaks):
             start = line_breaks[i - 1] + 1 if i > 0 else 0
             self.line_offsets[i + 1] = (start, lb)
```

### Comparing `deepsecrets-1.0.4/deepsecrets/core/model/finding.py` & `deepsecrets-1.0.5/deepsecrets/core/model/finding.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/model/rules/__pycache__/exlcuded_path.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/model/rules/__pycache__/hashed_secret.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/model/rules/__pycache__/regex.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/model/rules/__pycache__/rule.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/model/rules/hashed_secret.py` & `deepsecrets-1.0.5/deepsecrets/core/model/rules/hashed_secret.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/model/rules/regex.py` & `deepsecrets-1.0.5/deepsecrets/core/model/rules/regex.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/model/rules/rule.py` & `deepsecrets-1.0.5/deepsecrets/core/model/rules/rule.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/model/token.py` & `deepsecrets-1.0.5/deepsecrets/core/model/token.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/modes/.DS_Store` & `deepsecrets-1.0.5/deepsecrets/core/modes/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/modes/__pycache__/iscan_mode.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/modes/iscan_mode.py` & `deepsecrets-1.0.5/deepsecrets/core/modes/iscan_mode.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/excluded_paths.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/false_findings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc` & `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc` & `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/false_tokens.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc` & `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/hashed_secrets.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/ibuilder.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc` & `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/ldap_detector.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc` & `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc` & `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/path_exclusions.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc` & `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc` & `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/plaintext.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/regex.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc` & `deepsecrets-1.0.5/deepsecrets/core/rulesets/__pycache__/regex.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/rulesets/hashed_secrets.py` & `deepsecrets-1.0.5/deepsecrets/core/rulesets/hashed_secrets.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/rulesets/ibuilder.py` & `deepsecrets-1.0.5/deepsecrets/core/rulesets/ibuilder.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/.DS_Store` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/full_content.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/itokenizer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/lex_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,319 +1,300 @@
 magic:    0xa70d0d0a
-moddate:  0x2cfb2164 (Mon Mar 27 20:23:08 2023 UTC)
-files sz: 6015
+moddate:  0x0829e663 (Fri Feb 10 11:22:48 2023 UTC)
+files sz: 6353
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x9700640064016c006d015a016d025a026d035a036d045a046d055a0501
-      00640064026c066d075a070100640064036c086d095a090100640064046c
-      0a6d0b5a0b0100640064056c0c6d0d5a0d0100640064066c0e6d0f5a0f6d
-      105a100100640064076c116d125a130100640064086c146d155a15010064
-      0064096c166d175a1701006400640a6c186d195a1901006400640b6c1a6d
-      1b5a1b6d1c5a1c6d125a1201006400640c6c1d6d1e5a1e01006400640d6c
-      1f6d205a2001006400640e6c216d225a2201006400640f6c236d245a246d
-      255a256d265a260100640064106c276d285a28010067006411a2015a2902
-      0047006412840064136528a6030000ab0300000000000000005a2a641453
-      00
+      0x9700640064016c006d015a016d025a026d035a030100640064026c046d
+      055a050100640064036c066d075a070100640064046c086d095a09010064
+      0064056c0a6d0b5a0b0100640064066c0c6d0d5a0d6d0e5a0e0100640064
+      076c0f6d105a110100640064086c126d135a130100640064096c146d155a
+      1501006400640a6c166d175a1701006400640b6c186d195a190100640064
+      0c6c1a6d1b5a1b01006400640d6c1c6d1d5a1d01006400640e6c1e6d1f5a
+      1f6d205a206d105a1001006400640f6c216d225a220100640064106c236d
+      245a246d255a256d265a260100640064116c276d285a28010067006412a2
+      015a29020047006413840064146517a6030000ab0300000000000000005a
+      2a64155300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('List', 'Sequence', 'Set', 'Type', 'Union'))
+                 4 LOAD_CONST               1 (('List', 'Sequence', 'Type'))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (List)
                 10 STORE_NAME               1 (List)
                 12 IMPORT_FROM              2 (Sequence)
                 14 STORE_NAME               2 (Sequence)
-                16 IMPORT_FROM              3 (Set)
-                18 STORE_NAME               3 (Set)
-                20 IMPORT_FROM              4 (Type)
-                22 STORE_NAME               4 (Type)
-                24 IMPORT_FROM              5 (Union)
-                26 STORE_NAME               5 (Union)
-                28 POP_TOP
+                16 IMPORT_FROM              3 (Type)
+                18 STORE_NAME               3 (Type)
+                20 POP_TOP
    
-     3          30 LOAD_CONST               0 (0)
-                32 LOAD_CONST               2 (('OrderedSet',))
-                34 IMPORT_NAME              6 (ordered_set)
-                36 IMPORT_FROM              7 (OrderedSet)
-                38 STORE_NAME               7 (OrderedSet)
-                40 POP_TOP
+     7          22 LOAD_CONST               0 (0)
+                24 LOAD_CONST               2 (('OrderedSet',))
+                26 IMPORT_NAME              4 (ordered_set)
+                28 IMPORT_FROM              5 (OrderedSet)
+                30 STORE_NAME               5 (OrderedSet)
+                32 POP_TOP
    
-     4          42 LOAD_CONST               0 (0)
-                44 LOAD_CONST               3 (('highlight',))
-                46 IMPORT_NAME              8 (pygments)
-                48 IMPORT_FROM              9 (highlight)
-                50 STORE_NAME               9 (highlight)
-                52 POP_TOP
+     8          34 LOAD_CONST               0 (0)
+                36 LOAD_CONST               3 (('highlight',))
+                38 IMPORT_NAME              6 (pygments)
+                40 IMPORT_FROM              7 (highlight)
+                42 STORE_NAME               7 (highlight)
+                44 POP_TOP
    
-     5          54 LOAD_CONST               0 (0)
-                56 LOAD_CONST               4 (('RawTokenFormatter',))
-                58 IMPORT_NAME             10 (pygments.formatters)
-                60 IMPORT_FROM             11 (RawTokenFormatter)
-                62 STORE_NAME              11 (RawTokenFormatter)
-                64 POP_TOP
+     9          46 LOAD_CONST               0 (0)
+                48 LOAD_CONST               4 (('RawTokenFormatter',))
+                50 IMPORT_NAME              8 (pygments.formatters)
+                52 IMPORT_FROM              9 (RawTokenFormatter)
+                54 STORE_NAME               9 (RawTokenFormatter)
+                56 POP_TOP
    
-     6          66 LOAD_CONST               0 (0)
-                68 LOAD_CONST               5 (('get_lexer_for_filename',))
-                70 IMPORT_NAME             12 (pygments.lexers)
-                72 IMPORT_FROM             13 (get_lexer_for_filename)
-                74 STORE_NAME              13 (get_lexer_for_filename)
-                76 POP_TOP
+    10          58 LOAD_CONST               0 (0)
+                60 LOAD_CONST               5 (('get_lexer_for_filename',))
+                62 IMPORT_NAME             10 (pygments.lexers)
+                64 IMPORT_FROM             11 (get_lexer_for_filename)
+                66 STORE_NAME              11 (get_lexer_for_filename)
+                68 POP_TOP
    
-     7          78 LOAD_CONST               0 (0)
-                80 LOAD_CONST               6 (('Lexer', 'RawTokenLexer'))
-                82 IMPORT_NAME             14 (pygments.lexers.special)
-                84 IMPORT_FROM             15 (Lexer)
-                86 STORE_NAME              15 (Lexer)
-                88 IMPORT_FROM             16 (RawTokenLexer)
-                90 STORE_NAME              16 (RawTokenLexer)
-                92 POP_TOP
+    11          70 LOAD_CONST               0 (0)
+                72 LOAD_CONST               6 (('Lexer', 'RawTokenLexer'))
+                74 IMPORT_NAME             12 (pygments.lexers.special)
+                76 IMPORT_FROM             13 (Lexer)
+                78 STORE_NAME              13 (Lexer)
+                80 IMPORT_FROM             14 (RawTokenLexer)
+                82 STORE_NAME              14 (RawTokenLexer)
+                84 POP_TOP
    
-     8          94 LOAD_CONST               0 (0)
-                96 LOAD_CONST               7 (('Token',))
-                98 IMPORT_NAME             17 (pygments.token)
-               100 IMPORT_FROM             18 (Token)
-               102 STORE_NAME              19 (PygmentsToken)
-               104 POP_TOP
+    12          86 LOAD_CONST               0 (0)
+                88 LOAD_CONST               7 (('Token',))
+                90 IMPORT_NAME             15 (pygments.token)
+                92 IMPORT_FROM             16 (Token)
+                94 STORE_NAME              17 (PygmentsToken)
+                96 POP_TOP
    
-     9         106 LOAD_CONST               0 (0)
-               108 LOAD_CONST               8 (('ClassNotFound',))
-               110 IMPORT_NAME             20 (pygments.util)
-               112 IMPORT_FROM             21 (ClassNotFound)
-               114 STORE_NAME              21 (ClassNotFound)
-               116 POP_TOP
+    13          98 LOAD_CONST               0 (0)
+               100 LOAD_CONST               8 (('ClassNotFound',))
+               102 IMPORT_NAME             18 (pygments.util)
+               104 IMPORT_FROM             19 (ClassNotFound)
+               106 STORE_NAME              19 (ClassNotFound)
+               108 POP_TOP
    
-    11         118 LOAD_CONST               0 (0)
-               120 LOAD_CONST               9 (('File',))
-               122 IMPORT_NAME             22 (deepsecrets.core.model.file)
-               124 IMPORT_FROM             23 (File)
-               126 STORE_NAME              23 (File)
-               128 POP_TOP
+    14         110 LOAD_CONST               0 (0)
+               112 LOAD_CONST               9 (('Variable',))
+               114 IMPORT_NAME             20 (deepsecrets.core.model.semantic)
+               116 IMPORT_FROM             21 (Variable)
+               118 STORE_NAME              21 (Variable)
+               120 POP_TOP
    
-    12         130 LOAD_CONST               0 (0)
-               132 LOAD_CONST              10 (('Variable',))
-               134 IMPORT_NAME             24 (deepsecrets.core.model.semantic)
-               136 IMPORT_FROM             25 (Variable)
-               138 STORE_NAME              25 (Variable)
-               140 POP_TOP
+    16         122 LOAD_CONST               0 (0)
+               124 LOAD_CONST              10 (('Tokenizer',))
+               126 IMPORT_NAME             22 (deepsecrets.core.tokenizers.itokenizer)
+               128 IMPORT_FROM             23 (Tokenizer)
+               130 STORE_NAME              23 (Tokenizer)
+               132 POP_TOP
    
-    13         142 LOAD_CONST               0 (0)
-               144 LOAD_CONST              11 (('Semantic', 'SemanticType', 'Token'))
-               146 IMPORT_NAME             26 (deepsecrets.core.model.token)
-               148 IMPORT_FROM             27 (Semantic)
-               150 STORE_NAME              27 (Semantic)
-               152 IMPORT_FROM             28 (SemanticType)
-               154 STORE_NAME              28 (SemanticType)
-               156 IMPORT_FROM             18 (Token)
-               158 STORE_NAME              18 (Token)
-               160 POP_TOP
+    17         134 LOAD_CONST               0 (0)
+               136 LOAD_CONST              11 (('Language',))
+               138 IMPORT_NAME             24 (deepsecrets.core.tokenizers.lexer.semantic.language)
+               140 IMPORT_FROM             25 (Language)
+               142 STORE_NAME              25 (Language)
+               144 POP_TOP
    
-    14         162 LOAD_CONST               0 (0)
-               164 LOAD_CONST              12 (('Language',))
-               166 IMPORT_NAME             29 (deepsecrets.core.tokenizers.helpers.semantic.language)
-               168 IMPORT_FROM             30 (Language)
-               170 STORE_NAME              30 (Language)
-               172 POP_TOP
+    18         146 LOAD_CONST               0 (0)
+               148 LOAD_CONST              12 (('VariableDetectionRules',))
+               150 IMPORT_NAME             26 (deepsecrets.core.tokenizers.lexer.semantic.var_detection.rules)
+               152 IMPORT_FROM             27 (VariableDetectionRules)
+               154 STORE_NAME              27 (VariableDetectionRules)
+               156 POP_TOP
    
-    15         174 LOAD_CONST               0 (0)
-               176 LOAD_CONST              13 (('VariableDetectionRules',))
-               178 IMPORT_NAME             31 (deepsecrets.core.tokenizers.helpers.semantic.var_detection.rules)
-               180 IMPORT_FROM             32 (VariableDetectionRules)
-               182 STORE_NAME              32 (VariableDetectionRules)
-               184 POP_TOP
+    19         158 LOAD_CONST               0 (0)
+               160 LOAD_CONST              13 (('File',))
+               162 IMPORT_NAME             28 (deepsecrets.core.model.file)
+               164 IMPORT_FROM             29 (File)
+               166 STORE_NAME              29 (File)
+               168 POP_TOP
    
-    16         186 LOAD_CONST               0 (0)
-               188 LOAD_CONST              14 (('SpotImprovements',))
-               190 IMPORT_NAME             33 (deepsecrets.core.tokenizers.helpers.spot_improvements)
-               192 IMPORT_FROM             34 (SpotImprovements)
-               194 STORE_NAME              34 (SpotImprovements)
-               196 POP_TOP
+    20         170 LOAD_CONST               0 (0)
+               172 LOAD_CONST              14 (('Semantic', 'SemanticType', 'Token'))
+               174 IMPORT_NAME             30 (deepsecrets.core.model.token)
+               176 IMPORT_FROM             31 (Semantic)
+               178 STORE_NAME              31 (Semantic)
+               180 IMPORT_FROM             32 (SemanticType)
+               182 STORE_NAME              32 (SemanticType)
+               184 IMPORT_FROM             16 (Token)
+               186 STORE_NAME              16 (Token)
+               188 POP_TOP
    
-    17         198 LOAD_CONST               0 (0)
-               200 LOAD_CONST              15 (('token_to_typestream_item', 'types_to_filter_after', 'types_to_filter_before'))
-               202 IMPORT_NAME             35 (deepsecrets.core.tokenizers.helpers.type_stream)
-               204 IMPORT_FROM             36 (token_to_typestream_item)
-               206 STORE_NAME              36 (token_to_typestream_item)
-               208 IMPORT_FROM             37 (types_to_filter_after)
-               210 STORE_NAME              37 (types_to_filter_after)
-               212 IMPORT_FROM             38 (types_to_filter_before)
-               214 STORE_NAME              38 (types_to_filter_before)
-               216 POP_TOP
+    25         190 LOAD_CONST               0 (0)
+               192 LOAD_CONST              15 (('SpotImprovements',))
+               194 IMPORT_NAME             33 (deepsecrets.core.tokenizers.lexer.spot_improvements)
+               196 IMPORT_FROM             34 (SpotImprovements)
+               198 STORE_NAME              34 (SpotImprovements)
+               200 POP_TOP
    
-    22         218 LOAD_CONST               0 (0)
-               220 LOAD_CONST              16 (('Tokenizer',))
-               222 IMPORT_NAME             39 (deepsecrets.core.tokenizers.itokenizer)
-               224 IMPORT_FROM             40 (Tokenizer)
-               226 STORE_NAME              40 (Tokenizer)
-               228 POP_TOP
+    26         202 LOAD_CONST               0 (0)
+               204 LOAD_CONST              16 (('token_to_typestream_item', 'types_to_filter_before', 'types_to_filter_after'))
+               206 IMPORT_NAME             35 (deepsecrets.core.tokenizers.lexer.type_stream)
+               208 IMPORT_FROM             36 (token_to_typestream_item)
+               210 STORE_NAME              36 (token_to_typestream_item)
+               212 IMPORT_FROM             37 (types_to_filter_before)
+               214 STORE_NAME              37 (types_to_filter_before)
+               216 IMPORT_FROM             38 (types_to_filter_after)
+               218 STORE_NAME              38 (types_to_filter_after)
+               220 POP_TOP
    
-    24         230 BUILD_LIST               0
-               232 LOAD_CONST              17 (('\n', '\t', "'", "''", '"', '""'))
-               234 LIST_EXTEND              1
-               236 STORE_NAME              41 (empty_tokens)
+    29         222 LOAD_CONST               0 (0)
+               224 LOAD_CONST              17 (('TokenizationException',))
+               226 IMPORT_NAME             39 (deepsecrets.core.utils.exceptions)
+               228 IMPORT_FROM             40 (TokenizationException)
+               230 STORE_NAME              40 (TokenizationException)
+               232 POP_TOP
    
-    27         238 PUSH_NULL
-               240 LOAD_BUILD_CLASS
-               242 LOAD_CONST              18 (<code object LexerTokenizer, file "/app/deepsecrets/core/tokenizers/lexer.py", line 27>)
-               244 MAKE_FUNCTION            0
-               246 LOAD_CONST              19 ('LexerTokenizer')
-               248 LOAD_NAME               40 (Tokenizer)
-               250 PRECALL                  3
-               254 CALL                     3
-               264 STORE_NAME              42 (LexerTokenizer)
-               266 LOAD_CONST              20 (None)
-               268 RETURN_VALUE
+    33         234 BUILD_LIST               0
+               236 LOAD_CONST              18 (('\n', '\t', "'", "''", '"', '""'))
+               238 LIST_EXTEND              1
+               240 STORE_NAME              41 (empty_tokens)
+   
+    35         242 PUSH_NULL
+               244 LOAD_BUILD_CLASS
+               246 LOAD_CONST              19 (<code object LexerTokenizer, file "/app/deepsecrets/core/tokenizers/lexer/lexer.py", line 35>)
+               248 MAKE_FUNCTION            0
+               250 LOAD_CONST              20 ('LexerTokenizer')
+               252 LOAD_NAME               23 (Tokenizer)
+               254 PRECALL                  3
+               258 CALL                     3
+               268 STORE_NAME              42 (LexerTokenizer)
+               270 LOAD_CONST              21 (None)
+               272 RETURN_VALUE
    consts
       0
-      ('List', 'Sequence', 'Set', 'Type', 'Union')
+      ('List', 'Sequence', 'Type')
       ('OrderedSet',)
       ('highlight',)
       ('RawTokenFormatter',)
       ('get_lexer_for_filename',)
       ('Lexer', 'RawTokenLexer')
       ('Token',)
       ('ClassNotFound',)
-      ('File',)
       ('Variable',)
-      ('Semantic', 'SemanticType', 'Token')
+      ('Tokenizer',)
       ('Language',)
       ('VariableDetectionRules',)
+      ('File',)
+      ('Semantic', 'SemanticType', 'Token')
       ('SpotImprovements',)
-      ('token_to_typestream_item', 'types_to_filter_after', 'types_to_filter_before')
-      ('Tokenizer',)
+      ('token_to_typestream_item', 'types_to_filter_before', 'types_to_filter_after')
+      ('TokenizationException',)
       ('\n', '\t', "'", "''", '"', '""')
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 7
+         stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a0255006503650464013c0000006505650464023c
             0000006506650464033c0000006404650764056508650919000000000000
-            0000006604640684045a0a640765036405650b6503650c66021900000000
-            00000000006604640884045a0d6415640a650e64056508650f1900000000
-            00000000006604640b84055a10640c6508650f1900000000000000000064
-            05640d6604640e84045a11640f6512650f19000000000000000000641065
-            12650f1900000000000000000064056508650f1900000000000000000066
-            06641184045a1364056514650f190000000000000000006602641284045a
-            1564056508650f190000000000000000006602641384045a166416641484
-            045a17640d5300
-          27           0 RESUME                   0
+            0000006604640684045a0a640765036602640884045a0b64096503660264
+            0a84045a0c6417640c650d6602640d84055a0e640e6508650f1900000000
+            00000000006602640f84045a1064106511650f1900000000000000000064
+            116511650f190000000000000000006604641284045a12641384005a1364
+            1484005a14641584005a1564165300
+          35           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('LexerTokenizer')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          28          12 LOAD_NAME                3 (str)
+          37          12 LOAD_NAME                3 (str)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('token_stream')
                       18 STORE_SUBSCR
          
-          29          22 LOAD_NAME                5 (Lexer)
+          38          22 LOAD_NAME                5 (Lexer)
                       24 LOAD_NAME                4 (__annotations__)
                       26 LOAD_CONST               2 ('lexer')
                       28 STORE_SUBSCR
          
-          30          32 LOAD_NAME                6 (Language)
+          39          32 LOAD_NAME                6 (Language)
                       34 LOAD_NAME                4 (__annotations__)
                       36 LOAD_CONST               3 ('language')
                       38 STORE_SUBSCR
          
-          32          42 LOAD_CONST               4 ('token')
+          41          42 LOAD_CONST               4 ('token')
                       44 LOAD_NAME                7 (PygmentsToken)
                       46 LOAD_CONST               5 ('return')
                       48 LOAD_NAME                8 (List)
                       50 LOAD_NAME                9 (Type)
                       52 BINARY_SUBSCR
                       62 BUILD_TUPLE              4
-                      64 LOAD_CONST               6 (<code object _get_types_for_token, file "/app/deepsecrets/core/tokenizers/lexer.py", line 32>)
+                      64 LOAD_CONST               6 (<code object _get_types_for_token, file "/app/deepsecrets/core/tokenizers/lexer/lexer.py", line 41>)
                       66 MAKE_FUNCTION            4 (annotations)
                       68 STORE_NAME              10 (_get_types_for_token)
          
-          42          70 LOAD_CONST               7 ('content')
+          51          70 LOAD_CONST               7 ('content')
                       72 LOAD_NAME                3 (str)
-                      74 LOAD_CONST               5 ('return')
-                      76 LOAD_NAME               11 (Union)
-                      78 LOAD_NAME                3 (str)
-                      80 LOAD_NAME               12 (bool)
-                      82 BUILD_TUPLE              2
-                      84 BINARY_SUBSCR
-                      94 BUILD_TUPLE              4
-                      96 LOAD_CONST               8 (<code object sanitize, file "/app/deepsecrets/core/tokenizers/lexer.py", line 42>)
-                      98 MAKE_FUNCTION            4 (annotations)
-                     100 STORE_NAME              13 (sanitize)
+                      74 BUILD_TUPLE              2
+                      76 LOAD_CONST               8 (<code object sanitize, file "/app/deepsecrets/core/tokenizers/lexer/lexer.py", line 51>)
+                      78 MAKE_FUNCTION            4 (annotations)
+                      80 STORE_NAME              11 (sanitize)
+         
+          73          82 LOAD_CONST               9 ('string')
+                      84 LOAD_NAME                3 (str)
+                      86 BUILD_TUPLE              2
+                      88 LOAD_CONST              10 (<code object get_token_for_string, file "/app/deepsecrets/core/tokenizers/lexer/lexer.py", line 73>)
+                      90 MAKE_FUNCTION            4 (annotations)
+                      92 STORE_NAME              12 (get_token_for_string)
          
-          63         102 LOAD_CONST              21 ((True,))
-                     104 LOAD_CONST              10 ('file')
-                     106 LOAD_NAME               14 (File)
-                     108 LOAD_CONST               5 ('return')
+          79          94 LOAD_CONST              23 ((True,))
+                      96 LOAD_CONST              12 ('file')
+                      98 LOAD_NAME               13 (File)
+                     100 BUILD_TUPLE              2
+                     102 LOAD_CONST              13 (<code object tokenize, file "/app/deepsecrets/core/tokenizers/lexer/lexer.py", line 79>)
+                     104 MAKE_FUNCTION            5 (defaults, annotations)
+                     106 STORE_NAME              14 (tokenize)
+         
+         140         108 LOAD_CONST              14 ('tokens')
                      110 LOAD_NAME                8 (List)
                      112 LOAD_NAME               15 (Token)
                      114 BINARY_SUBSCR
-                     124 BUILD_TUPLE              4
-                     126 LOAD_CONST              11 (<code object tokenize, file "/app/deepsecrets/core/tokenizers/lexer.py", line 63>)
-                     128 MAKE_FUNCTION            5 (defaults, annotations)
-                     130 STORE_NAME              16 (tokenize)
+                     124 BUILD_TUPLE              2
+                     126 LOAD_CONST              15 (<code object add_to_token_stream, file "/app/deepsecrets/core/tokenizers/lexer/lexer.py", line 140>)
+                     128 MAKE_FUNCTION            4 (annotations)
+                     130 STORE_NAME              16 (add_to_token_stream)
          
-         114         132 LOAD_CONST              12 ('tokens')
-                     134 LOAD_NAME                8 (List)
+         145         132 LOAD_CONST              16 ('tokens_all')
+                     134 LOAD_NAME               17 (Sequence)
                      136 LOAD_NAME               15 (Token)
                      138 BINARY_SUBSCR
-                     148 LOAD_CONST               5 ('return')
-                     150 LOAD_CONST              13 (None)
-                     152 BUILD_TUPLE              4
-                     154 LOAD_CONST              14 (<code object add_to_token_stream, file "/app/deepsecrets/core/tokenizers/lexer.py", line 114>)
-                     156 MAKE_FUNCTION            4 (annotations)
-                     158 STORE_NAME              17 (add_to_token_stream)
-         
-         118         160 LOAD_CONST              15 ('tokens_all')
-                     162 LOAD_NAME               18 (Sequence)
-                     164 LOAD_NAME               15 (Token)
-                     166 BINARY_SUBSCR
-                     176 LOAD_CONST              16 ('tokens_to_be_excluded')
-                     178 LOAD_NAME               18 (Sequence)
-                     180 LOAD_NAME               15 (Token)
-                     182 BINARY_SUBSCR
-                     192 LOAD_CONST               5 ('return')
-                     194 LOAD_NAME                8 (List)
-                     196 LOAD_NAME               15 (Token)
-                     198 BINARY_SUBSCR
-                     208 BUILD_TUPLE              6
-                     210 LOAD_CONST              17 (<code object final_cleanup, file "/app/deepsecrets/core/tokenizers/lexer.py", line 118>)
-                     212 MAKE_FUNCTION            4 (annotations)
-                     214 STORE_NAME              19 (final_cleanup)
+                     148 LOAD_CONST              17 ('tokens_to_be_excluded')
+                     150 LOAD_NAME               17 (Sequence)
+                     152 LOAD_NAME               15 (Token)
+                     154 BINARY_SUBSCR
+                     164 BUILD_TUPLE              4
+                     166 LOAD_CONST              18 (<code object final_cleanup, file "/app/deepsecrets/core/tokenizers/lexer/lexer.py", line 145>)
+                     168 MAKE_FUNCTION            4 (annotations)
+                     170 STORE_NAME              18 (final_cleanup)
          
-         138         216 LOAD_CONST               5 ('return')
-                     218 LOAD_NAME               20 (Set)
-                     220 LOAD_NAME               15 (Token)
-                     222 BINARY_SUBSCR
-                     232 BUILD_TUPLE              2
-                     234 LOAD_CONST              18 (<code object deep_analyze, file "/app/deepsecrets/core/tokenizers/lexer.py", line 138>)
-                     236 MAKE_FUNCTION            4 (annotations)
-                     238 STORE_NAME              21 (deep_analyze)
+         165         172 LOAD_CONST              19 (<code object deep_analyze, file "/app/deepsecrets/core/tokenizers/lexer/lexer.py", line 165>)
+                     174 MAKE_FUNCTION            0
+                     176 STORE_NAME              19 (deep_analyze)
          
-         160         240 LOAD_CONST               5 ('return')
-                     242 LOAD_NAME                8 (List)
-                     244 LOAD_NAME               15 (Token)
-                     246 BINARY_SUBSCR
-                     256 BUILD_TUPLE              2
-                     258 LOAD_CONST              19 (<code object get_variables, file "/app/deepsecrets/core/tokenizers/lexer.py", line 160>)
-                     260 MAKE_FUNCTION            4 (annotations)
-                     262 STORE_NAME              22 (get_variables)
+         187         178 LOAD_CONST              20 (<code object get_variables, file "/app/deepsecrets/core/tokenizers/lexer/lexer.py", line 187>)
+                     180 MAKE_FUNCTION            0
+                     182 STORE_NAME              20 (get_variables)
          
-         176         264 LOAD_CONST              22 (('return', None))
-                     266 LOAD_CONST              20 (<code object print_token_type_stream, file "/app/deepsecrets/core/tokenizers/lexer.py", line 176>)
-                     268 MAKE_FUNCTION            4 (annotations)
-                     270 STORE_NAME              23 (print_token_type_stream)
-                     272 LOAD_CONST              13 (None)
-                     274 RETURN_VALUE
+         203         184 LOAD_CONST              21 (<code object print_token_type_stream, file "/app/deepsecrets/core/tokenizers/lexer/lexer.py", line 203>)
+                     186 MAKE_FUNCTION            0
+                     188 STORE_NAME              21 (print_token_type_stream)
+                     190 LOAD_CONST              22 (None)
+                     192 RETURN_VALUE
          consts
             'LexerTokenizer'
             'token_stream'
             'lexer'
             'language'
             'token'
             'return'
@@ -326,65 +307,65 @@
                   0x970067007d027c02a00000000000000000000000000000000000000000
                   007c01a6010000ab01000000000000000001007c016a0100000000000000
                   0081417c016a0100000000000000007404000000000000000000006b0200
                   00000072027c0253007c00a0030000000000000000000000000000000000
                   0000007c016a010000000000000000a6010000ab0100000000000000007d
                   037c02a00400000000000000000000000000000000000000007c03a60100
                   00ab01000000000000000001007c025300
-                32           0 RESUME                   0
+                41           0 RESUME                   0
                
-                33           2 BUILD_LIST               0
+                42           2 BUILD_LIST               0
                              4 STORE_FAST               2 (types)
                
-                34           6 LOAD_FAST                2 (types)
+                43           6 LOAD_FAST                2 (types)
                              8 LOAD_METHOD              0 (append)
                             30 LOAD_FAST                1 (token)
                             32 PRECALL                  1
                             36 CALL                     1
                             46 POP_TOP
                
-                35          48 LOAD_FAST                1 (token)
+                44          48 LOAD_FAST                1 (token)
                             50 LOAD_ATTR                1 (parent)
                             60 POP_JUMP_FORWARD_IF_NONE    65 (to 192)
                
-                36          62 LOAD_FAST                1 (token)
+                45          62 LOAD_FAST                1 (token)
                             64 LOAD_ATTR                1 (parent)
                             74 LOAD_GLOBAL              4 (PygmentsToken)
                             86 COMPARE_OP               2 (==)
                             92 POP_JUMP_FORWARD_IF_FALSE     2 (to 98)
                
-                37          94 LOAD_FAST                2 (types)
+                46          94 LOAD_FAST                2 (types)
                             96 RETURN_VALUE
                
-                38     >>   98 LOAD_FAST                0 (self)
+                47     >>   98 LOAD_FAST                0 (self)
                            100 LOAD_METHOD              3 (_get_types_for_token)
                            122 LOAD_FAST                1 (token)
                            124 LOAD_ATTR                1 (parent)
                            134 PRECALL                  1
                            138 CALL                     1
                            148 STORE_FAST               3 (deep)
                
-                39         150 LOAD_FAST                2 (types)
+                48         150 LOAD_FAST                2 (types)
                            152 LOAD_METHOD              4 (extend)
                            174 LOAD_FAST                3 (deep)
                            176 PRECALL                  1
                            180 CALL                     1
                            190 POP_TOP
                
-                40     >>  192 LOAD_FAST                2 (types)
+                49     >>  192 LOAD_FAST                2 (types)
                            194 RETURN_VALUE
                consts
                   None
                names      ('append', 'parent', 'PygmentsToken', '_get_types_for_token', 'extend')
                varnames   ('self', 'token', 'types', 'deep')
                freevars   ()
                cellvars   ()
-               filename   '/app/deepsecrets/core/tokenizers/lexer.py'
+               filename   '/app/deepsecrets/core/tokenizers/lexer/lexer.py'
                name       '_get_types_for_token'
-               firstlineno 32
+               firstlineno 41
                lnotab 0x020104012a010e012001040134012a01
             'content'
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 4
                flags     : 3
@@ -395,30 +376,30 @@
                   0100000000720664046b020000000072056e0201006e0264055300740300
                   0000000000000000007c01a6010000ab01000000000000000064066b0400
                   00000072167c0164071900000000000000000064086b0200000000720a7c
                   01640064078502190000000000000000007d017c01640419000000000000
                   0000007c016407190000000000000000006b020000000072147c01640419
                   0000000000000000007c027600720a7c0164066407850219000000000000
                   0000007d017c017c0276007202640553007c015300
-                42           0 RESUME                   0
+                51           0 RESUME                   0
                
-                43           2 BUILD_LIST               0
+                53           2 BUILD_LIST               0
                              4 LOAD_CONST               1 (("'", "''", '"', '""'))
                              6 LIST_EXTEND              1
                              8 STORE_FAST               2 (quotes)
                
-                45          10 LOAD_FAST                1 (content)
+                55          10 LOAD_FAST                1 (content)
                             12 LOAD_METHOD              0 (replace)
                             34 LOAD_CONST               2 (' ')
                             36 LOAD_CONST               3 ('')
                             38 PRECALL                  2
                             42 CALL                     2
                             52 STORE_FAST               3 (whitespace_cleaned)
                
-                46          54 LOAD_CONST               4 (0)
+                56          54 LOAD_CONST               4 (0)
                             56 LOAD_GLOBAL              3 (NULL + len)
                             68 LOAD_FAST                3 (whitespace_cleaned)
                             70 PRECALL                  1
                             74 CALL                     1
                             84 SWAP                     2
                             86 COPY                     2
                             88 COMPARE_OP               1 (<=)
@@ -426,70 +407,70 @@
                             96 LOAD_CONST               4 (0)
                             98 COMPARE_OP               2 (==)
                            104 POP_JUMP_FORWARD_IF_FALSE     5 (to 116)
                            106 JUMP_FORWARD             2 (to 112)
                        >>  108 POP_TOP
                            110 JUMP_FORWARD             2 (to 116)
                
-                47     >>  112 LOAD_CONST               5 (False)
+                57     >>  112 LOAD_CONST               5 (False)
                            114 RETURN_VALUE
                
-                51     >>  116 LOAD_GLOBAL              3 (NULL + len)
+                61     >>  116 LOAD_GLOBAL              3 (NULL + len)
                            128 LOAD_FAST                1 (content)
                            130 PRECALL                  1
                            134 CALL                     1
                            144 LOAD_CONST               6 (1)
                            146 COMPARE_OP               4 (>)
                            152 POP_JUMP_FORWARD_IF_FALSE    22 (to 198)
                            154 LOAD_FAST                1 (content)
                            156 LOAD_CONST               7 (-1)
                            158 BINARY_SUBSCR
                            168 LOAD_CONST               8 ('\n')
                            170 COMPARE_OP               2 (==)
                            176 POP_JUMP_FORWARD_IF_FALSE    10 (to 198)
                
-                52         178 LOAD_FAST                1 (content)
+                62         178 LOAD_FAST                1 (content)
                            180 LOAD_CONST               0 (None)
                            182 LOAD_CONST               7 (-1)
                            184 BUILD_SLICE              2
                            186 BINARY_SUBSCR
                            196 STORE_FAST               1 (content)
                
-                54     >>  198 LOAD_FAST                1 (content)
+                64     >>  198 LOAD_FAST                1 (content)
                            200 LOAD_CONST               4 (0)
                            202 BINARY_SUBSCR
                            212 LOAD_FAST                1 (content)
                            214 LOAD_CONST               7 (-1)
                            216 BINARY_SUBSCR
                            226 COMPARE_OP               2 (==)
                            232 POP_JUMP_FORWARD_IF_FALSE    20 (to 274)
                
-                55         234 LOAD_FAST                1 (content)
+                65         234 LOAD_FAST                1 (content)
                            236 LOAD_CONST               4 (0)
                            238 BINARY_SUBSCR
                            248 LOAD_FAST                2 (quotes)
                            250 CONTAINS_OP              0
                            252 POP_JUMP_FORWARD_IF_FALSE    10 (to 274)
                
-                56         254 LOAD_FAST                1 (content)
+                66         254 LOAD_FAST                1 (content)
                            256 LOAD_CONST               6 (1)
                            258 LOAD_CONST               7 (-1)
                            260 BUILD_SLICE              2
                            262 BINARY_SUBSCR
                            272 STORE_FAST               1 (content)
                
-                58     >>  274 LOAD_FAST                1 (content)
+                68     >>  274 LOAD_FAST                1 (content)
                            276 LOAD_FAST                2 (quotes)
                            278 CONTAINS_OP              0
                            280 POP_JUMP_FORWARD_IF_FALSE     2 (to 286)
                
-                59         282 LOAD_CONST               5 (False)
+                69         282 LOAD_CONST               5 (False)
                            284 RETURN_VALUE
                
-                61     >>  286 LOAD_FAST                1 (content)
+                71     >>  286 LOAD_FAST                1 (content)
                            288 RETURN_VALUE
                consts
                   None
                   ("'", "''", '"', '""')
                   ' '
                   ''
                   0
@@ -497,18 +478,69 @@
                   1
                   -1
                   '\n'
                names      ('replace', 'len')
                varnames   ('self', 'content', 'quotes', 'whitespace_cleaned')
                freevars   ()
                cellvars   ()
-               filename   '/app/deepsecrets/core/tokenizers/lexer.py'
+               filename   '/app/deepsecrets/core/tokenizers/lexer/lexer.py'
                name       'sanitize'
-               firstlineno 42
-               lnotab 0x020108022c013a0104043e01140224011401140208010402
+               firstlineno 51
+               lnotab 0x020208022c013a0104043e01140224011401140208010402
+            'string'
+            code
+               argcount  : 2
+               nlocals   : 4
+               stacksize : 3
+               flags     : 3
+               code
+                  0x97007401000000000000000000007c006a010000000000000000a60100
+                  00ab01000000000000000044005d145c0200007d027d037c017c036a0200
+                  00000000000000760072067c027c0366026302010053008c1564015300
+                73           0 RESUME                   0
+               
+                74           2 LOAD_GLOBAL              1 (NULL + enumerate)
+                            14 LOAD_FAST                0 (self)
+                            16 LOAD_ATTR                1 (tokens)
+                            26 PRECALL                  1
+                            30 CALL                     1
+                            40 GET_ITER
+                       >>   42 FOR_ITER                20 (to 84)
+                            44 UNPACK_SEQUENCE          2
+                            48 STORE_FAST               2 (i)
+                            50 STORE_FAST               3 (token)
+               
+                75          52 LOAD_FAST                1 (string)
+                            54 LOAD_FAST                3 (token)
+                            56 LOAD_ATTR                2 (content)
+                            66 CONTAINS_OP              0
+                            68 POP_JUMP_FORWARD_IF_FALSE     6 (to 82)
+               
+                76          70 LOAD_FAST                2 (i)
+                            72 LOAD_FAST                3 (token)
+                            74 BUILD_TUPLE              2
+                            76 SWAP                     2
+                            78 POP_TOP
+                            80 RETURN_VALUE
+               
+                75     >>   82 JUMP_BACKWARD           21 (to 42)
+               
+                77     >>   84 LOAD_CONST               1 ((None, None))
+                            86 RETURN_VALUE
+               consts
+                  None
+                  (None, None)
+               names      ('enumerate', 'tokens', 'content')
+               varnames   ('self', 'string', 'i', 'token')
+               freevars   ()
+               cellvars   ()
+               filename   '/app/deepsecrets/core/tokenizers/lexer/lexer.py'
+               name       'get_token_for_string'
+               firstlineno 73
+               lnotab 0x0201320112010cff0202
             True
             'file'
             code
                argcount  : 3
                nlocals   : 18
                stacksize : 7
                flags     : 3
@@ -553,246 +585,250 @@
                   007d107e107701770078035900770167007d117c006a1f00000000000000
                   006a2000000000000000006407750072147c00a021000000000000000000
                   0000000000000000000000a6000000ab0000000000000000007d117c0272
                   1b7c00a02200000000000000000000000000000000000000007c006a0500
                   000000000000007c11a6020000ab0200000000000000006e13741f000000
                   000000000000007c006a050000000000000000a6010000ab010000000000
                   0000005300
-                63           0 RESUME                   0
+                79           0 RESUME                   0
                
-                64           2 LOAD_CONST               1 ('')
+                80           2 LOAD_CONST               1 ('')
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (token_stream)
                
-                66          16 NOP
+                82          16 NOP
                
-                67          18 LOAD_GLOBAL              3 (NULL + get_lexer_for_filename)
+                83          18 LOAD_GLOBAL              3 (NULL + get_lexer_for_filename)
                             30 LOAD_FAST                1 (file)
                             32 LOAD_ATTR                2 (path)
                             42 PRECALL                  1
                             46 CALL                     1
                             56 LOAD_FAST                0 (self)
                             58 STORE_ATTR               3 (lexer)
                             68 JUMP_FORWARD            23 (to 116)
                        >>   70 PUSH_EXC_INFO
                
-                68          72 LOAD_GLOBAL              8 (ClassNotFound)
+                84          72 LOAD_GLOBAL              8 (ClassNotFound)
                             84 CHECK_EXC_MATCH
                             86 POP_JUMP_FORWARD_IF_FALSE    10 (to 108)
                             88 POP_TOP
                
-                69          90 LOAD_CONST               0 (None)
+                85          90 LOAD_CONST               0 (None)
                             92 LOAD_FAST                0 (self)
                             94 STORE_ATTR               3 (lexer)
                            104 POP_EXCEPT
                            106 JUMP_FORWARD             4 (to 116)
                
-                68     >>  108 RERAISE                  0
+                84     >>  108 RERAISE                  0
                        >>  110 COPY                     3
                            112 POP_EXCEPT
                            114 RERAISE                  1
                
-                71     >>  116 LOAD_FAST                0 (self)
+                87     >>  116 LOAD_FAST                0 (self)
                            118 LOAD_ATTR                3 (lexer)
                            128 POP_JUMP_FORWARD_IF_TRUE     7 (to 144)
                
-                72         130 LOAD_FAST                0 (self)
+                88         130 LOAD_FAST                0 (self)
                            132 LOAD_ATTR                5 (tokens)
                            142 RETURN_VALUE
                
-                74     >>  144 NOP
+                90     >>  144 NOP
                
-                75         146 LOAD_GLOBAL             13 (NULL + Language)
+                91         146 LOAD_GLOBAL             13 (NULL + Language)
                            158 LOAD_ATTR                7 (from_text)
                            168 LOAD_FAST                0 (self)
                            170 LOAD_ATTR                3 (lexer)
                            180 LOAD_ATTR                8 (filenames)
                            190 LOAD_CONST               2 (0)
                            192 BINARY_SUBSCR
                            202 PRECALL                  1
                            206 CALL                     1
                            216 LOAD_FAST                0 (self)
                            218 STORE_ATTR               9 (language)
                            228 JUMP_FORWARD            46 (to 322)
                        >>  230 PUSH_EXC_INFO
                
-                76         232 LOAD_GLOBAL             20 (ValueError)
+                92         232 LOAD_GLOBAL             20 (ValueError)
                            244 CHECK_EXC_MATCH
                            246 POP_JUMP_FORWARD_IF_FALSE    33 (to 314)
                            248 POP_TOP
                
-                77         250 LOAD_GLOBAL             13 (NULL + Language)
+                93         250 LOAD_GLOBAL             13 (NULL + Language)
                            262 LOAD_ATTR                7 (from_text)
                            272 LOAD_FAST                1 (file)
                            274 LOAD_ATTR               11 (extension)
                            284 PRECALL                  1
                            288 CALL                     1
                            298 LOAD_FAST                0 (self)
                            300 STORE_ATTR               9 (language)
                            310 POP_EXCEPT
                            312 JUMP_FORWARD             4 (to 322)
                
-                76     >>  314 RERAISE                  0
+                92     >>  314 RERAISE                  0
                        >>  316 COPY                     3
                            318 POP_EXCEPT
                            320 RERAISE                  1
                
-                79     >>  322 LOAD_GLOBAL             25 (NULL + highlight)
+                95     >>  322 LOAD_GLOBAL             25 (NULL + highlight)
                            334 LOAD_FAST                1 (file)
                            336 LOAD_ATTR               13 (content)
                            346 LOAD_FAST                0 (self)
                            348 LOAD_ATTR                3 (lexer)
                            358 LOAD_GLOBAL             29 (NULL + RawTokenFormatter)
                            370 PRECALL                  0
                            374 CALL                     0
                            384 PRECALL                  3
                            388 CALL                     3
                            398 STORE_FAST               3 (result)
                
-                80         400 LOAD_GLOBAL             31 (NULL + list)
+                96         400 LOAD_GLOBAL             31 (NULL + list)
                            412 LOAD_GLOBAL             33 (NULL + RawTokenLexer)
                            424 PRECALL                  0
                            428 CALL                     0
                            438 LOAD_METHOD             17 (get_tokens)
                            460 LOAD_FAST                3 (result)
                            462 PRECALL                  1
                            466 CALL                     1
                            476 PRECALL                  1
                            480 CALL                     1
                            490 STORE_FAST               4 (raw_tokens)
                
-                81         492 LOAD_GLOBAL             37 (NULL + SpotImprovements)
+                97         492 LOAD_GLOBAL             37 (NULL + SpotImprovements)
                            504 LOAD_FAST                0 (self)
                            506 LOAD_ATTR                9 (language)
                            516 KW_NAMES                 3
                            518 PRECALL                  1
                            522 CALL                     1
                            532 STORE_FAST               5 (token_improver)
                
-                83         534 LOAD_CONST               2 (0)
+                99         534 LOAD_CONST               2 (0)
                            536 STORE_FAST               6 (current_position)
                
-                85         538 LOAD_GLOBAL             39 (NULL + enumerate)
+               101         538 LOAD_GLOBAL             39 (NULL + enumerate)
                            550 LOAD_FAST                4 (raw_tokens)
                            552 PRECALL                  1
                            556 CALL                     1
                            566 GET_ITER
                        >>  568 EXTENDED_ARG             1
                            570 FOR_ITER               276 (to 1124)
                            572 UNPACK_SEQUENCE          2
                            576 STORE_FAST               7 (i)
                            578 STORE_FAST               8 (raw_token)
                
-                86         580 LOAD_FAST                8 (raw_token)
+               102         580 LOAD_FAST                8 (raw_token)
                            582 LOAD_CONST               4 (1)
                            584 BINARY_SUBSCR
                            594 STORE_FAST               9 (content)
                
-                87         596 LOAD_FAST                0 (self)
+               103         596 LOAD_FAST                0 (self)
                            598 LOAD_METHOD             20 (_get_types_for_token)
                            620 LOAD_FAST                8 (raw_token)
                            622 LOAD_CONST               2 (0)
                            624 BINARY_SUBSCR
                            634 PRECALL                  1
                            638 CALL                     1
                            648 STORE_FAST              10 (types)
                
-                88         650 LOAD_FAST                6 (current_position)
+               104         650 LOAD_FAST                6 (current_position)
                            652 STORE_FAST              11 (start)
                
-                89         654 LOAD_FAST               11 (start)
+               105         654 LOAD_FAST               11 (start)
                            656 LOAD_GLOBAL             43 (NULL + len)
                            668 LOAD_FAST                9 (content)
                            670 PRECALL                  1
                            674 CALL                     1
                            684 BINARY_OP                0 (+)
                            688 STORE_FAST              12 (end)
                
-                90         690 LOAD_FAST               12 (end)
+               106         690 LOAD_FAST               12 (end)
                            692 STORE_FAST               6 (current_position)
                
-                92         694 NOP
+               108         694 NOP
                
-                93         696 LOAD_FAST                0 (self)
+               109         696 LOAD_FAST                0 (self)
                            698 LOAD_METHOD             22 (sanitize)
                            720 LOAD_FAST                9 (content)
                            722 PRECALL                  1
                            726 CALL                     1
                            736 STORE_FAST               9 (content)
                
-                94         738 LOAD_FAST                9 (content)
+               110         738 LOAD_FAST                9 (content)
                            740 POP_JUMP_FORWARD_IF_TRUE     1 (to 744)
                
-                95         742 JUMP_BACKWARD           88 (to 568)
+               111         742 JUMP_BACKWARD           88 (to 568)
                
-                97     >>  744 LOAD_FAST                1 (file)
+               114     >>  744 LOAD_FAST                1 (file)
                            746 LOAD_METHOD             23 (get_span_for_string)
                            768 LOAD_FAST                9 (content)
                            770 LOAD_FAST               11 (start)
                            772 LOAD_CONST               4 (1)
                            774 BINARY_OP               10 (-)
                            778 LOAD_FAST               12 (end)
                            780 LOAD_CONST               4 (1)
                            782 BINARY_OP                0 (+)
                            786 BUILD_LIST               2
                            788 KW_NAMES                 5
                            790 PRECALL                  2
                            794 CALL                     2
                            804 STORE_FAST              13 (span)
                
-                98         806 LOAD_GLOBAL             49 (NULL + Token)
-                           818 LOAD_FAST                1 (file)
-                           820 LOAD_FAST                9 (content)
-                           822 LOAD_FAST               13 (span)
-                           824 KW_NAMES                 6
+               115         806 LOAD_GLOBAL             49 (NULL + Token)
+               
+               116         818 LOAD_FAST                1 (file)
+               
+               117         820 LOAD_FAST                9 (content)
+               
+               118         822 LOAD_FAST               13 (span)
+               
+               115         824 KW_NAMES                 6
                            826 PRECALL                  3
                            830 CALL                     3
                            840 STORE_FAST              14 (token)
                
-                99         842 LOAD_FAST               14 (token)
+               120         842 LOAD_FAST               14 (token)
                            844 LOAD_METHOD             25 (set_type)
                            866 LOAD_FAST               10 (types)
                            868 PRECALL                  1
                            872 CALL                     1
                            882 POP_TOP
                
-               101         884 LOAD_FAST                5 (token_improver)
+               122         884 LOAD_FAST                5 (token_improver)
                            886 LOAD_METHOD             26 (improve_token)
                            908 LOAD_FAST                0 (self)
                            910 LOAD_ATTR                5 (tokens)
                            920 LOAD_FAST                0 (self)
                            922 LOAD_ATTR                0 (token_stream)
                            932 LOAD_FAST               14 (token)
                            934 PRECALL                  3
                            938 CALL                     3
                            948 STORE_FAST              15 (improved_tokens)
                
-               103         950 LOAD_FAST                0 (self)
+               124         950 LOAD_FAST                0 (self)
                            952 LOAD_ATTR                5 (tokens)
                            962 LOAD_METHOD             27 (extend)
                            984 LOAD_FAST               15 (improved_tokens)
                            986 PRECALL                  1
                            990 CALL                     1
                           1000 POP_TOP
                
-               104        1002 LOAD_FAST                0 (self)
+               125        1002 LOAD_FAST                0 (self)
                           1004 LOAD_METHOD             28 (add_to_token_stream)
                           1026 LOAD_FAST               15 (improved_tokens)
                           1028 PRECALL                  1
                           1032 CALL                     1
                           1042 POP_TOP
                           1044 JUMP_BACKWARD          239 (to 568)
                        >> 1046 PUSH_EXC_INFO
                
-               105        1048 LOAD_GLOBAL             58 (Exception)
+               126        1048 LOAD_GLOBAL             58 (Exception)
                           1060 CHECK_EXC_MATCH
                           1062 POP_JUMP_FORWARD_IF_FALSE    26 (to 1116)
                           1064 STORE_FAST              16 (e)
                
-               106        1066 LOAD_GLOBAL             61 (NULL + str)
+               127        1066 LOAD_GLOBAL             61 (NULL + str)
                           1078 LOAD_FAST               16 (e)
                           1080 PRECALL                  1
                           1084 CALL                     1
                           1094 POP_TOP
                           1096 POP_EXCEPT
                           1098 LOAD_CONST               0 (None)
                           1100 STORE_FAST              16 (e)
@@ -800,51 +836,54 @@
                           1104 EXTENDED_ARG             1
                           1106 JUMP_BACKWARD          270 (to 568)
                        >> 1108 LOAD_CONST               0 (None)
                           1110 STORE_FAST              16 (e)
                           1112 DELETE_FAST             16 (e)
                           1114 RERAISE                  1
                
-               105     >> 1116 RERAISE                  0
+               126     >> 1116 RERAISE                  0
                        >> 1118 COPY                     3
                           1120 POP_EXCEPT
                           1122 RERAISE                  1
                
-               108     >> 1124 BUILD_LIST               0
+               129     >> 1124 BUILD_LIST               0
                           1126 STORE_FAST              17 (tokens_to_be_excluded)
                
-               109        1128 LOAD_FAST                0 (self)
+               130        1128 LOAD_FAST                0 (self)
                           1130 LOAD_ATTR               31 (settings)
                           1140 LOAD_ATTR               32 (deep_token_inspection)
                           1150 LOAD_CONST               7 (True)
                           1152 IS_OP                    0
                           1154 POP_JUMP_FORWARD_IF_FALSE    20 (to 1196)
                
-               110        1156 LOAD_FAST                0 (self)
+               131        1156 LOAD_FAST                0 (self)
                           1158 LOAD_METHOD             33 (deep_analyze)
                           1180 PRECALL                  0
                           1184 CALL                     0
                           1194 STORE_FAST              17 (tokens_to_be_excluded)
                
-               112     >> 1196 LOAD_FAST                2 (post_filter)
-                          1198 POP_JUMP_FORWARD_IF_FALSE    27 (to 1254)
+               135     >> 1196 LOAD_FAST                2 (post_filter)
+               
+               134        1198 POP_JUMP_FORWARD_IF_FALSE    27 (to 1254)
                           1200 LOAD_FAST                0 (self)
                           1202 LOAD_METHOD             34 (final_cleanup)
                           1224 LOAD_FAST                0 (self)
                           1226 LOAD_ATTR                5 (tokens)
                           1236 LOAD_FAST               17 (tokens_to_be_excluded)
                           1238 PRECALL                  2
                           1242 CALL                     2
                           1252 JUMP_FORWARD            19 (to 1292)
-                       >> 1254 LOAD_GLOBAL             31 (NULL + list)
+               
+               136     >> 1254 LOAD_GLOBAL             31 (NULL + list)
                           1266 LOAD_FAST                0 (self)
                           1268 LOAD_ATTR                5 (tokens)
                           1278 PRECALL                  1
                           1282 CALL                     1
-                       >> 1292 RETURN_VALUE
+               
+               133     >> 1292 RETURN_VALUE
                ExceptionTable:
                  18 to 66 -> 70 [0]
                  70 to 102 -> 110 [1] lasti
                  108 to 108 -> 110 [1] lasti
                  146 to 226 -> 230 [0]
                  230 to 308 -> 316 [1] lasti
                  314 to 314 -> 316 [1] lasti
@@ -856,70 +895,70 @@
                consts
                   None
                   ''
                   0
                   ('lang',)
                   1
                   ('between',)
-                  ('file', 'content', 'span')
+                  ('file', 'cont', 'span')
                   True
                names      ('token_stream', 'get_lexer_for_filename', 'path', 'lexer', 'ClassNotFound', 'tokens', 'Language', 'from_text', 'filenames', 'language', 'ValueError', 'extension', 'highlight', 'content', 'RawTokenFormatter', 'list', 'RawTokenLexer', 'get_tokens', 'SpotImprovements', 'enumerate', '_get_types_for_token', 'len', 'sanitize', 'get_span_for_string', 'Token', 'set_type', 'improve_token', 'extend', 'add_to_token_stream', 'Exception', 'str', 'settings', 'deep_token_inspection', 'deep_analyze', 'final_cleanup')
                varnames   ('self', 'file', 'post_filter', 'result', 'raw_tokens', 'token_improver', 'current_position', 'i', 'raw_token', 'content', 'types', 'start', 'end', 'span', 'token', 'improved_tokens', 'e', 'tokens_to_be_excluded')
                freevars   ()
                cellvars   ()
-               filename   '/app/deepsecrets/core/tokenizers/lexer.py'
+               filename   '/app/deepsecrets/core/tokenizers/lexer/lexer.py'
                name       'tokenize'
-               firstlineno 63
+               firstlineno 79
                lnotab
                   0x02010e0202013601120112ff08030e010e0202015601120140ff08034e
-                  015c012a0204022a011001360104012401040202012a01040102023e0124
-                  012a02420234012e01120132ff080304011c012802
+                  015c012a0204022a011001360104012401040202012a01040102033e010c
+                  010201020102fd12052a02420234012e01120132ff080304011c01280402
+                  ff380226fd
             'tokens'
-            None
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 6
                flags     : 3
                code
                   0x97007c0144005d207d027c0078016a0000000000000000007403000000
                   000000000000007c02ac01a6010000ab0100000000000000007a0d000063
                   025f0000000000000000008c2164005300
-               114           0 RESUME                   0
+               140           0 RESUME                   0
                
-               115           2 LOAD_FAST                1 (tokens)
+               141           2 LOAD_FAST                1 (tokens)
                              4 GET_ITER
                        >>    6 FOR_ITER                32 (to 72)
                              8 STORE_FAST               2 (token)
                
-               116          10 LOAD_FAST                0 (self)
+               142          10 LOAD_FAST                0 (self)
                             12 COPY                     1
                             14 LOAD_ATTR                0 (token_stream)
                             24 LOAD_GLOBAL              3 (NULL + token_to_typestream_item)
                             36 LOAD_FAST                2 (token)
                             38 KW_NAMES                 1
                             40 PRECALL                  1
                             44 CALL                     1
                             54 BINARY_OP               13 (+=)
                             58 SWAP                     2
                             60 STORE_ATTR               0 (token_stream)
                             70 JUMP_BACKWARD           33 (to 6)
                
-               115     >>   72 LOAD_CONST               0 (None)
+               141     >>   72 LOAD_CONST               0 (None)
                             74 RETURN_VALUE
                consts
                   None
                   ('token',)
                names      ('token_stream', 'token_to_typestream_item')
                varnames   ('self', 'tokens', 'token')
                freevars   ()
                cellvars   ()
-               filename   '/app/deepsecrets/core/tokenizers/lexer.py'
+               filename   '/app/deepsecrets/core/tokenizers/lexer/lexer.py'
                name       'add_to_token_stream'
-               firstlineno 114
+               firstlineno 140
                lnotab 0x020108013eff
             'tokens_all'
             'tokens_to_be_excluded'
             code
                argcount  : 3
                nlocals   : 4
                stacksize : 5
@@ -934,103 +973,103 @@
                   01640284087408000000000000000000004400a6000000ab000000000000
                   000000a6010000ab01000000000000000072018c4489046a050000000000
                   000000740c00000000000000000000760072018c537c03a0070000000000
                   0000000000000000000000000000008904a6010000ab0100000000000000
                   0001008c697c035300
                              0 MAKE_CELL                4 (token)
                
-               118           2 RESUME                   0
+               145           2 RESUME                   0
                
-               119           4 LOAD_GLOBAL              1 (NULL + isinstance)
+               146           4 LOAD_GLOBAL              1 (NULL + isinstance)
                             16 LOAD_FAST                1 (tokens_all)
                             18 LOAD_GLOBAL              2 (OrderedSet)
                             30 PRECALL                  2
                             34 CALL                     2
                             44 POP_JUMP_FORWARD_IF_TRUE    15 (to 76)
                
-               120          46 LOAD_GLOBAL              3 (NULL + OrderedSet)
+               147          46 LOAD_GLOBAL              3 (NULL + OrderedSet)
                             58 LOAD_FAST                1 (tokens_all)
                             60 PRECALL                  1
                             64 CALL                     1
                             74 STORE_FAST               1 (tokens_all)
                
-               122     >>   76 LOAD_FAST                1 (tokens_all)
+               149     >>   76 LOAD_FAST                1 (tokens_all)
                             78 LOAD_FAST                2 (tokens_to_be_excluded)
                             80 BINARY_OP               10 (-)
                             84 STORE_FAST               1 (tokens_all)
                
-               123          86 BUILD_LIST               0
+               150          86 BUILD_LIST               0
                             88 STORE_FAST               3 (final)
                
-               124          90 LOAD_FAST                1 (tokens_all)
+               151          90 LOAD_FAST                1 (tokens_all)
                             92 GET_ITER
                        >>   94 FOR_ITER               104 (to 304)
                             96 STORE_DEREF              4 (token)
                
-               125          98 LOAD_GLOBAL              5 (NULL + any)
+               152          98 LOAD_GLOBAL              5 (NULL + any)
                            110 LOAD_CLOSURE             4 (token)
                            112 BUILD_TUPLE              1
-                           114 LOAD_CONST               1 (<code object <genexpr>, file "/app/deepsecrets/core/tokenizers/lexer.py", line 125>)
+                           114 LOAD_CONST               1 (<code object <genexpr>, file "/app/deepsecrets/core/tokenizers/lexer/lexer.py", line 152>)
                            116 MAKE_FUNCTION            8 (closure)
                            118 LOAD_GLOBAL              6 (types_to_filter_before)
                            130 GET_ITER
                            132 PRECALL                  0
                            136 CALL                     0
                            146 PRECALL                  1
                            150 CALL                     1
                            160 POP_JUMP_FORWARD_IF_FALSE     1 (to 164)
                
-               126         162 JUMP_BACKWARD           35 (to 94)
+               153         162 JUMP_BACKWARD           35 (to 94)
                
-               128     >>  164 LOAD_GLOBAL              5 (NULL + any)
+               155     >>  164 LOAD_GLOBAL              5 (NULL + any)
                            176 LOAD_CLOSURE             4 (token)
                            178 BUILD_TUPLE              1
-                           180 LOAD_CONST               2 (<code object <genexpr>, file "/app/deepsecrets/core/tokenizers/lexer.py", line 128>)
+                           180 LOAD_CONST               2 (<code object <genexpr>, file "/app/deepsecrets/core/tokenizers/lexer/lexer.py", line 155>)
                            182 MAKE_FUNCTION            8 (closure)
                            184 LOAD_GLOBAL              8 (types_to_filter_after)
                            196 GET_ITER
                            198 PRECALL                  0
                            202 CALL                     0
                            212 PRECALL                  1
                            216 CALL                     1
                            226 POP_JUMP_FORWARD_IF_FALSE     1 (to 230)
                
-               129         228 JUMP_BACKWARD           68 (to 94)
+               156         228 JUMP_BACKWARD           68 (to 94)
                
-               131     >>  230 LOAD_DEREF               4 (token)
+               158     >>  230 LOAD_DEREF               4 (token)
                            232 LOAD_ATTR                5 (content)
                            242 LOAD_GLOBAL             12 (empty_tokens)
                            254 CONTAINS_OP              0
                            256 POP_JUMP_FORWARD_IF_FALSE     1 (to 260)
                
-               132         258 JUMP_BACKWARD           83 (to 94)
+               159         258 JUMP_BACKWARD           83 (to 94)
                
-               134     >>  260 LOAD_FAST                3 (final)
+               161     >>  260 LOAD_FAST                3 (final)
                            262 LOAD_METHOD              7 (append)
                            284 LOAD_DEREF               4 (token)
                            286 PRECALL                  1
                            290 CALL                     1
                            300 POP_TOP
                            302 JUMP_BACKWARD          105 (to 94)
                
-               136     >>  304 LOAD_FAST                3 (final)
+               163     >>  304 LOAD_FAST                3 (final)
                            306 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 51
                      code
                         0x95014b00010097007c005d0d7d017c0189026a00000000000000000076
                         005600970101008c0e64005300
                                    0 COPY_FREE_VARS           1
                      
-                     125           2 RETURN_GENERATOR
+                     152           2 RETURN_GENERATOR
                                    4 POP_TOP
                                    6 RESUME                   0
                                    8 LOAD_FAST                0 (.0)
                              >>   10 FOR_ITER                13 (to 38)
                                   12 STORE_FAST               1 (type)
                                   14 LOAD_FAST                1 (type)
                                   16 LOAD_DEREF               2 (token)
@@ -1044,29 +1083,29 @@
                                   40 RETURN_VALUE
                      consts
                         None
                      names      ('type',)
                      varnames   ('.0', 'type')
                      freevars   ('token',)
                      cellvars   ()
-                     filename   '/app/deepsecrets/core/tokenizers/lexer.py'
+                     filename   '/app/deepsecrets/core/tokenizers/lexer/lexer.py'
                      name       '<genexpr>'
-                     firstlineno 125
+                     firstlineno 152
                      lnotab 0x
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 51
                      code
                         0x95014b00010097007c005d0d7d017c0189026a00000000000000000076
                         005600970101008c0e64005300
                                    0 COPY_FREE_VARS           1
                      
-                     128           2 RETURN_GENERATOR
+                     155           2 RETURN_GENERATOR
                                    4 POP_TOP
                                    6 RESUME                   0
                                    8 LOAD_FAST                0 (.0)
                              >>   10 FOR_ITER                13 (to 38)
                                   12 STORE_FAST               1 (type)
                                   14 LOAD_FAST                1 (type)
                                   16 LOAD_DEREF               2 (token)
@@ -1080,25 +1119,25 @@
                                   40 RETURN_VALUE
                      consts
                         None
                      names      ('type',)
                      varnames   ('.0', 'type')
                      freevars   ('token',)
                      cellvars   ()
-                     filename   '/app/deepsecrets/core/tokenizers/lexer.py'
+                     filename   '/app/deepsecrets/core/tokenizers/lexer/lexer.py'
                      name       '<genexpr>'
-                     firstlineno 128
+                     firstlineno 155
                      lnotab 0x
                names      ('isinstance', 'OrderedSet', 'any', 'types_to_filter_before', 'types_to_filter_after', 'content', 'empty_tokens', 'append')
                varnames   ('self', 'tokens_all', 'tokens_to_be_excluded', 'final')
                freevars   ()
                cellvars   ('token',)
-               filename   '/app/deepsecrets/core/tokenizers/lexer.py'
+               filename   '/app/deepsecrets/core/tokenizers/lexer/lexer.py'
                name       'final_cleanup'
-               firstlineno 118
+               firstlineno 145
                lnotab 0x04012a011e020a010401080140010202400102021c0102022c02
             code
                argcount  : 1
                nlocals   : 7
                stacksize : 7
                flags     : 3
                code
@@ -1113,112 +1152,112 @@
                   00ab01000000000000000001008c367c0344005d567d0674130000000000
                   00000000007414000000000000000000006a0b00000000000000007c066a
                   0c00000000000000006a0d00000000000000007c066a0e00000000000000
                   006a0f0000000000000000ac01a6030000ab0300000000000000007c066a
                   1000000000000000005f1100000000000000007c02a01200000000000000
                   000000000000000000000000007c066a0c0000000000000000a6010000ab
                   01000000000000000001008c577c025300
-               138           0 RESUME                   0
+               165           0 RESUME                   0
                
-               139           2 LOAD_GLOBAL              1 (NULL + OrderedSet)
+               166           2 LOAD_GLOBAL              1 (NULL + OrderedSet)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (tokens)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 STORE_FAST               1 (tokens_all)
                
-               140          42 LOAD_FAST                0 (self)
+               167          42 LOAD_FAST                0 (self)
                             44 LOAD_ATTR                2 (language)
                             54 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 60)
                
-               141          56 LOAD_FAST                1 (tokens_all)
+               168          56 LOAD_FAST                1 (tokens_all)
                             58 RETURN_VALUE
                
-               143     >>   60 LOAD_GLOBAL              7 (NULL + set)
+               170     >>   60 LOAD_GLOBAL              7 (NULL + set)
                             72 PRECALL                  0
                             76 CALL                     0
                             86 STORE_FAST               2 (exclude_after)
                
-               145          88 BUILD_LIST               0
+               172          88 BUILD_LIST               0
                             90 STORE_FAST               3 (true_detections)
                
-               146          92 LOAD_GLOBAL              9 (NULL + VariableDetectionRules)
+               173          92 LOAD_GLOBAL              9 (NULL + VariableDetectionRules)
                            104 LOAD_ATTR                5 (for_language)
                            114 LOAD_FAST                0 (self)
                            116 LOAD_ATTR                2 (language)
                            126 PRECALL                  1
                            130 CALL                     1
                            140 STORE_FAST               4 (rules)
                
-               147         142 LOAD_FAST                4 (rules)
+               174         142 LOAD_FAST                4 (rules)
                            144 GET_ITER
                        >>  146 FOR_ITER                53 (to 254)
                            148 STORE_FAST               5 (rule)
                
-               148         150 LOAD_FAST                3 (true_detections)
+               175         150 LOAD_FAST                3 (true_detections)
                            152 LOAD_METHOD              6 (extend)
                            174 LOAD_FAST                5 (rule)
                            176 LOAD_METHOD              7 (match)
                            198 LOAD_FAST                0 (self)
                            200 LOAD_ATTR                1 (tokens)
                            210 LOAD_FAST                0 (self)
                            212 LOAD_ATTR                8 (token_stream)
                            222 PRECALL                  2
                            226 CALL                     2
                            236 PRECALL                  1
                            240 CALL                     1
                            250 POP_TOP
                            252 JUMP_BACKWARD           54 (to 146)
                
-               150     >>  254 LOAD_FAST                3 (true_detections)
+               177     >>  254 LOAD_FAST                3 (true_detections)
                            256 GET_ITER
                        >>  258 FOR_ITER                86 (to 432)
                            260 STORE_FAST               6 (var)
                
-               151         262 LOAD_GLOBAL             19 (NULL + Semantic)
+               178         262 LOAD_GLOBAL             19 (NULL + Semantic)
                
-               152         274 LOAD_GLOBAL             20 (SemanticType)
+               179         274 LOAD_GLOBAL             20 (SemanticType)
                            286 LOAD_ATTR               11 (VAR)
                
-               153         296 LOAD_FAST                6 (var)
+               180         296 LOAD_FAST                6 (var)
                            298 LOAD_ATTR               12 (name)
                            308 LOAD_ATTR               13 (content)
                
-               154         318 LOAD_FAST                6 (var)
+               181         318 LOAD_FAST                6 (var)
                            320 LOAD_ATTR               14 (found_by)
                            330 LOAD_ATTR               15 (creds_probability)
                
-               151         340 KW_NAMES                 1
+               178         340 KW_NAMES                 1
                            342 PRECALL                  3
                            346 CALL                     3
                            356 LOAD_FAST                6 (var)
                            358 LOAD_ATTR               16 (value)
                            368 STORE_ATTR              17 (semantic)
                
-               156         378 LOAD_FAST                2 (exclude_after)
+               183         378 LOAD_FAST                2 (exclude_after)
                            380 LOAD_METHOD             18 (add)
                            402 LOAD_FAST                6 (var)
                            404 LOAD_ATTR               12 (name)
                            414 PRECALL                  1
                            418 CALL                     1
                            428 POP_TOP
                            430 JUMP_BACKWARD           87 (to 258)
                
-               158     >>  432 LOAD_FAST                2 (exclude_after)
+               185     >>  432 LOAD_FAST                2 (exclude_after)
                            434 RETURN_VALUE
                consts
                   None
                   ('type', 'name', 'creds_probability')
                names      ('OrderedSet', 'tokens', 'language', 'set', 'VariableDetectionRules', 'for_language', 'extend', 'match', 'token_stream', 'Semantic', 'SemanticType', 'VAR', 'name', 'content', 'found_by', 'creds_probability', 'value', 'semantic', 'add')
                varnames   ('self', 'tokens_all', 'exclude_after', 'true_detections', 'rules', 'rule', 'var')
                freevars   ()
                cellvars   ()
-               filename   '/app/deepsecrets/core/tokenizers/lexer.py'
+               filename   '/app/deepsecrets/core/tokenizers/lexer/lexer.py'
                name       'deep_analyze'
-               firstlineno 138
+               firstlineno 165
                lnotab
                   0x020128010e0104021c02040132010801680208010c011601160116fd26
                   053602
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
@@ -1227,117 +1266,117 @@
                   0x970067007d017401000000000000000000007c006a0100000000000000
                   00a6010000ab01000000000000000064016b02000000007202670053007c
                   006a01000000000000000044005d3a7d027c026a02000000000000000080
                   018c0a7c026a0200000000000000006a0300000000000000007408000000
                   000000000000006a0500000000000000006b030000000072018c257c01a0
                   0600000000000000000000000000000000000000007c02a6010000ab0100
                   0000000000000001008c3b7c015300
-               160           0 RESUME                   0
+               187           0 RESUME                   0
                
-               161           2 BUILD_LIST               0
+               188           2 BUILD_LIST               0
                              4 STORE_FAST               1 (vars)
                
-               162           6 LOAD_GLOBAL              1 (NULL + len)
+               189           6 LOAD_GLOBAL              1 (NULL + len)
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (tokens)
                             30 PRECALL                  1
                             34 CALL                     1
                             44 LOAD_CONST               1 (0)
                             46 COMPARE_OP               2 (==)
                             52 POP_JUMP_FORWARD_IF_FALSE     2 (to 58)
                
-               163          54 BUILD_LIST               0
+               190          54 BUILD_LIST               0
                             56 RETURN_VALUE
                
-               165     >>   58 LOAD_FAST                0 (self)
+               192     >>   58 LOAD_FAST                0 (self)
                             60 LOAD_ATTR                1 (tokens)
                             70 GET_ITER
                        >>   72 FOR_ITER                58 (to 190)
                             74 STORE_FAST               2 (token)
                
-               166          76 LOAD_FAST                2 (token)
+               193          76 LOAD_FAST                2 (token)
                             78 LOAD_ATTR                2 (semantic)
                             88 POP_JUMP_FORWARD_IF_NOT_NONE     1 (to 92)
                
-               167          90 JUMP_BACKWARD           10 (to 72)
+               194          90 JUMP_BACKWARD           10 (to 72)
                
-               169     >>   92 LOAD_FAST                2 (token)
+               196     >>   92 LOAD_FAST                2 (token)
                             94 LOAD_ATTR                2 (semantic)
                            104 LOAD_ATTR                3 (type)
                            114 LOAD_GLOBAL              8 (SemanticType)
                            126 LOAD_ATTR                5 (VAR)
                            136 COMPARE_OP               3 (!=)
                            142 POP_JUMP_FORWARD_IF_FALSE     1 (to 146)
                
-               170         144 JUMP_BACKWARD           37 (to 72)
+               197         144 JUMP_BACKWARD           37 (to 72)
                
-               172     >>  146 LOAD_FAST                1 (vars)
+               199     >>  146 LOAD_FAST                1 (vars)
                            148 LOAD_METHOD              6 (append)
                            170 LOAD_FAST                2 (token)
                            172 PRECALL                  1
                            176 CALL                     1
                            186 POP_TOP
                            188 JUMP_BACKWARD           59 (to 72)
                
-               174     >>  190 LOAD_FAST                1 (vars)
+               201     >>  190 LOAD_FAST                1 (vars)
                            192 RETURN_VALUE
                consts
                   None
                   0
                names      ('len', 'tokens', 'semantic', 'type', 'SemanticType', 'VAR', 'append')
                varnames   ('self', 'vars', 'token')
                freevars   ()
                cellvars   ()
-               filename   '/app/deepsecrets/core/tokenizers/lexer.py'
+               filename   '/app/deepsecrets/core/tokenizers/lexer/lexer.py'
                name       'get_variables'
-               firstlineno 160
+               firstlineno 187
                lnotab 0x020104013001040212010e010202340102022c02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab010000000000000000010064005300
-               176           0 RESUME                   0
+               203           0 RESUME                   0
                
-               177           2 LOAD_GLOBAL              1 (NULL + print)
+               204           2 LOAD_GLOBAL              1 (NULL + print)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (token_stream)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('print', 'token_stream')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/app/deepsecrets/core/tokenizers/lexer.py'
+               filename   '/app/deepsecrets/core/tokenizers/lexer/lexer.py'
                name       'print_token_type_stream'
-               firstlineno 176
+               firstlineno 203
                lnotab 0x0201
+            None
             (True,)
-            ('return', None)
-         names      ('__name__', '__module__', '__qualname__', 'str', '__annotations__', 'Lexer', 'Language', 'PygmentsToken', 'List', 'Type', '_get_types_for_token', 'Union', 'bool', 'sanitize', 'File', 'Token', 'tokenize', 'add_to_token_stream', 'Sequence', 'final_cleanup', 'Set', 'deep_analyze', 'get_variables', 'print_token_type_stream')
+         names      ('__name__', '__module__', '__qualname__', 'str', '__annotations__', 'Lexer', 'Language', 'PygmentsToken', 'List', 'Type', '_get_types_for_token', 'sanitize', 'get_token_for_string', 'File', 'tokenize', 'Token', 'add_to_token_stream', 'Sequence', 'final_cleanup', 'deep_analyze', 'get_variables', 'print_token_type_stream')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/app/deepsecrets/core/tokenizers/lexer.py'
+         filename   '/app/deepsecrets/core/tokenizers/lexer/lexer.py'
          name       'LexerTokenizer'
-         firstlineno 27
-         lnotab 0x0c010a010a010a021c0a20151e331c04381418161810
+         firstlineno 35
+         lnotab 0x0c020a010a010a021c0a0c160c060e3d1805281406160610
       'LexerTokenizer'
       None
-   names      ('typing', 'List', 'Sequence', 'Set', 'Type', 'Union', 'ordered_set', 'OrderedSet', 'pygments', 'highlight', 'pygments.formatters', 'RawTokenFormatter', 'pygments.lexers', 'get_lexer_for_filename', 'pygments.lexers.special', 'Lexer', 'RawTokenLexer', 'pygments.token', 'Token', 'PygmentsToken', 'pygments.util', 'ClassNotFound', 'deepsecrets.core.model.file', 'File', 'deepsecrets.core.model.semantic', 'Variable', 'deepsecrets.core.model.token', 'Semantic', 'SemanticType', 'deepsecrets.core.tokenizers.helpers.semantic.language', 'Language', 'deepsecrets.core.tokenizers.helpers.semantic.var_detection.rules', 'VariableDetectionRules', 'deepsecrets.core.tokenizers.helpers.spot_improvements', 'SpotImprovements', 'deepsecrets.core.tokenizers.helpers.type_stream', 'token_to_typestream_item', 'types_to_filter_after', 'types_to_filter_before', 'deepsecrets.core.tokenizers.itokenizer', 'Tokenizer', 'empty_tokens', 'LexerTokenizer')
+   names      ('typing', 'List', 'Sequence', 'Type', 'ordered_set', 'OrderedSet', 'pygments', 'highlight', 'pygments.formatters', 'RawTokenFormatter', 'pygments.lexers', 'get_lexer_for_filename', 'pygments.lexers.special', 'Lexer', 'RawTokenLexer', 'pygments.token', 'Token', 'PygmentsToken', 'pygments.util', 'ClassNotFound', 'deepsecrets.core.model.semantic', 'Variable', 'deepsecrets.core.tokenizers.itokenizer', 'Tokenizer', 'deepsecrets.core.tokenizers.lexer.semantic.language', 'Language', 'deepsecrets.core.tokenizers.lexer.semantic.var_detection.rules', 'VariableDetectionRules', 'deepsecrets.core.model.file', 'File', 'deepsecrets.core.model.token', 'Semantic', 'SemanticType', 'deepsecrets.core.tokenizers.lexer.spot_improvements', 'SpotImprovements', 'deepsecrets.core.tokenizers.lexer.type_stream', 'token_to_typestream_item', 'types_to_filter_before', 'types_to_filter_after', 'deepsecrets.core.utils.exceptions', 'TokenizationException', 'empty_tokens', 'LexerTokenizer')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/app/deepsecrets/core/tokenizers/lexer.py'
+   filename   '/app/deepsecrets/core/tokenizers/lexer/lexer.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02011c020c010c010c010c0110010c010c020c010c0114010c010c
-      010c0114050c020803
+      0x00ff020114060c010c010c010c0110010c010c010c020c010c010c010c
+      0114050c0114030c040802
```

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/per_line.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/per_word.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/.DS_Store` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/__pycache__/lexer.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,300 +1,326 @@
 magic:    0xa70d0d0a
-moddate:  0x0829e663 (Fri Feb 10 11:22:48 2023 UTC)
-files sz: 6353
+moddate:  0xaa959964 (Mon Jun 26 13:42:02 2023 UTC)
+files sz: 6481
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x9700640064016c006d015a016d025a026d035a030100640064026c046d
-      055a050100640064036c066d075a070100640064046c086d095a09010064
-      0064056c0a6d0b5a0b0100640064066c0c6d0d5a0d6d0e5a0e0100640064
-      076c0f6d105a110100640064086c126d135a130100640064096c146d155a
-      1501006400640a6c166d175a1701006400640b6c186d195a190100640064
-      0c6c1a6d1b5a1b01006400640d6c1c6d1d5a1d01006400640e6c1e6d1f5a
-      1f6d205a206d105a1001006400640f6c216d225a220100640064106c236d
-      245a246d255a256d265a260100640064116c276d285a28010067006412a2
-      015a29020047006413840064146517a6030000ab0300000000000000005a
-      2a64155300
+      0x9700640064016c006d015a016d025a026d035a036d045a046d055a0501
+      00640064026c066d075a070100640064036c086d095a090100640064046c
+      0a6d0b5a0b0100640064056c0c6d0d5a0d0100640064066c0e6d0f5a0f6d
+      105a100100640064076c116d125a130100640064086c146d155a15010064
+      0064096c166d175a1701006400640a6c186d195a1901006400640b6c1a6d
+      1b5a1b6d1c5a1c6d125a1201006400640c6c1d6d1e5a1e01006400640d6c
+      1f6d205a2001006400640e6c216d225a2201006400640f6c236d245a246d
+      255a256d265a260100640064106c276d285a28010067006411a2015a2902
+      0047006412840064136528a6030000ab0300000000000000005a2a641453
+      00
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('List', 'Sequence', 'Type'))
+                 4 LOAD_CONST               1 (('List', 'Sequence', 'Set', 'Type', 'Union'))
                  6 IMPORT_NAME              0 (typing)
                  8 IMPORT_FROM              1 (List)
                 10 STORE_NAME               1 (List)
                 12 IMPORT_FROM              2 (Sequence)
                 14 STORE_NAME               2 (Sequence)
-                16 IMPORT_FROM              3 (Type)
-                18 STORE_NAME               3 (Type)
-                20 POP_TOP
+                16 IMPORT_FROM              3 (Set)
+                18 STORE_NAME               3 (Set)
+                20 IMPORT_FROM              4 (Type)
+                22 STORE_NAME               4 (Type)
+                24 IMPORT_FROM              5 (Union)
+                26 STORE_NAME               5 (Union)
+                28 POP_TOP
    
-     7          22 LOAD_CONST               0 (0)
-                24 LOAD_CONST               2 (('OrderedSet',))
-                26 IMPORT_NAME              4 (ordered_set)
-                28 IMPORT_FROM              5 (OrderedSet)
-                30 STORE_NAME               5 (OrderedSet)
-                32 POP_TOP
+     3          30 LOAD_CONST               0 (0)
+                32 LOAD_CONST               2 (('OrderedSet',))
+                34 IMPORT_NAME              6 (ordered_set)
+                36 IMPORT_FROM              7 (OrderedSet)
+                38 STORE_NAME               7 (OrderedSet)
+                40 POP_TOP
    
-     8          34 LOAD_CONST               0 (0)
-                36 LOAD_CONST               3 (('highlight',))
-                38 IMPORT_NAME              6 (pygments)
-                40 IMPORT_FROM              7 (highlight)
-                42 STORE_NAME               7 (highlight)
-                44 POP_TOP
+     4          42 LOAD_CONST               0 (0)
+                44 LOAD_CONST               3 (('highlight',))
+                46 IMPORT_NAME              8 (pygments)
+                48 IMPORT_FROM              9 (highlight)
+                50 STORE_NAME               9 (highlight)
+                52 POP_TOP
    
-     9          46 LOAD_CONST               0 (0)
-                48 LOAD_CONST               4 (('RawTokenFormatter',))
-                50 IMPORT_NAME              8 (pygments.formatters)
-                52 IMPORT_FROM              9 (RawTokenFormatter)
-                54 STORE_NAME               9 (RawTokenFormatter)
-                56 POP_TOP
+     5          54 LOAD_CONST               0 (0)
+                56 LOAD_CONST               4 (('RawTokenFormatter',))
+                58 IMPORT_NAME             10 (pygments.formatters)
+                60 IMPORT_FROM             11 (RawTokenFormatter)
+                62 STORE_NAME              11 (RawTokenFormatter)
+                64 POP_TOP
    
-    10          58 LOAD_CONST               0 (0)
-                60 LOAD_CONST               5 (('get_lexer_for_filename',))
-                62 IMPORT_NAME             10 (pygments.lexers)
-                64 IMPORT_FROM             11 (get_lexer_for_filename)
-                66 STORE_NAME              11 (get_lexer_for_filename)
-                68 POP_TOP
+     6          66 LOAD_CONST               0 (0)
+                68 LOAD_CONST               5 (('get_lexer_for_filename',))
+                70 IMPORT_NAME             12 (pygments.lexers)
+                72 IMPORT_FROM             13 (get_lexer_for_filename)
+                74 STORE_NAME              13 (get_lexer_for_filename)
+                76 POP_TOP
    
-    11          70 LOAD_CONST               0 (0)
-                72 LOAD_CONST               6 (('Lexer', 'RawTokenLexer'))
-                74 IMPORT_NAME             12 (pygments.lexers.special)
-                76 IMPORT_FROM             13 (Lexer)
-                78 STORE_NAME              13 (Lexer)
-                80 IMPORT_FROM             14 (RawTokenLexer)
-                82 STORE_NAME              14 (RawTokenLexer)
-                84 POP_TOP
+     7          78 LOAD_CONST               0 (0)
+                80 LOAD_CONST               6 (('Lexer', 'RawTokenLexer'))
+                82 IMPORT_NAME             14 (pygments.lexers.special)
+                84 IMPORT_FROM             15 (Lexer)
+                86 STORE_NAME              15 (Lexer)
+                88 IMPORT_FROM             16 (RawTokenLexer)
+                90 STORE_NAME              16 (RawTokenLexer)
+                92 POP_TOP
    
-    12          86 LOAD_CONST               0 (0)
-                88 LOAD_CONST               7 (('Token',))
-                90 IMPORT_NAME             15 (pygments.token)
-                92 IMPORT_FROM             16 (Token)
-                94 STORE_NAME              17 (PygmentsToken)
-                96 POP_TOP
+     8          94 LOAD_CONST               0 (0)
+                96 LOAD_CONST               7 (('Token',))
+                98 IMPORT_NAME             17 (pygments.token)
+               100 IMPORT_FROM             18 (Token)
+               102 STORE_NAME              19 (PygmentsToken)
+               104 POP_TOP
    
-    13          98 LOAD_CONST               0 (0)
-               100 LOAD_CONST               8 (('ClassNotFound',))
-               102 IMPORT_NAME             18 (pygments.util)
-               104 IMPORT_FROM             19 (ClassNotFound)
-               106 STORE_NAME              19 (ClassNotFound)
-               108 POP_TOP
+     9         106 LOAD_CONST               0 (0)
+               108 LOAD_CONST               8 (('ClassNotFound',))
+               110 IMPORT_NAME             20 (pygments.util)
+               112 IMPORT_FROM             21 (ClassNotFound)
+               114 STORE_NAME              21 (ClassNotFound)
+               116 POP_TOP
    
-    14         110 LOAD_CONST               0 (0)
-               112 LOAD_CONST               9 (('Variable',))
-               114 IMPORT_NAME             20 (deepsecrets.core.model.semantic)
-               116 IMPORT_FROM             21 (Variable)
-               118 STORE_NAME              21 (Variable)
-               120 POP_TOP
+    11         118 LOAD_CONST               0 (0)
+               120 LOAD_CONST               9 (('File',))
+               122 IMPORT_NAME             22 (deepsecrets.core.model.file)
+               124 IMPORT_FROM             23 (File)
+               126 STORE_NAME              23 (File)
+               128 POP_TOP
    
-    16         122 LOAD_CONST               0 (0)
-               124 LOAD_CONST              10 (('Tokenizer',))
-               126 IMPORT_NAME             22 (deepsecrets.core.tokenizers.itokenizer)
-               128 IMPORT_FROM             23 (Tokenizer)
-               130 STORE_NAME              23 (Tokenizer)
-               132 POP_TOP
+    12         130 LOAD_CONST               0 (0)
+               132 LOAD_CONST              10 (('Variable',))
+               134 IMPORT_NAME             24 (deepsecrets.core.model.semantic)
+               136 IMPORT_FROM             25 (Variable)
+               138 STORE_NAME              25 (Variable)
+               140 POP_TOP
    
-    17         134 LOAD_CONST               0 (0)
-               136 LOAD_CONST              11 (('Language',))
-               138 IMPORT_NAME             24 (deepsecrets.core.tokenizers.lexer.semantic.language)
-               140 IMPORT_FROM             25 (Language)
-               142 STORE_NAME              25 (Language)
-               144 POP_TOP
+    13         142 LOAD_CONST               0 (0)
+               144 LOAD_CONST              11 (('Semantic', 'SemanticType', 'Token'))
+               146 IMPORT_NAME             26 (deepsecrets.core.model.token)
+               148 IMPORT_FROM             27 (Semantic)
+               150 STORE_NAME              27 (Semantic)
+               152 IMPORT_FROM             28 (SemanticType)
+               154 STORE_NAME              28 (SemanticType)
+               156 IMPORT_FROM             18 (Token)
+               158 STORE_NAME              18 (Token)
+               160 POP_TOP
    
-    18         146 LOAD_CONST               0 (0)
-               148 LOAD_CONST              12 (('VariableDetectionRules',))
-               150 IMPORT_NAME             26 (deepsecrets.core.tokenizers.lexer.semantic.var_detection.rules)
-               152 IMPORT_FROM             27 (VariableDetectionRules)
-               154 STORE_NAME              27 (VariableDetectionRules)
-               156 POP_TOP
+    14         162 LOAD_CONST               0 (0)
+               164 LOAD_CONST              12 (('Language',))
+               166 IMPORT_NAME             29 (deepsecrets.core.tokenizers.helpers.semantic.language)
+               168 IMPORT_FROM             30 (Language)
+               170 STORE_NAME              30 (Language)
+               172 POP_TOP
    
-    19         158 LOAD_CONST               0 (0)
-               160 LOAD_CONST              13 (('File',))
-               162 IMPORT_NAME             28 (deepsecrets.core.model.file)
-               164 IMPORT_FROM             29 (File)
-               166 STORE_NAME              29 (File)
-               168 POP_TOP
+    15         174 LOAD_CONST               0 (0)
+               176 LOAD_CONST              13 (('VariableDetectionRules',))
+               178 IMPORT_NAME             31 (deepsecrets.core.tokenizers.helpers.semantic.var_detection.rules)
+               180 IMPORT_FROM             32 (VariableDetectionRules)
+               182 STORE_NAME              32 (VariableDetectionRules)
+               184 POP_TOP
    
-    20         170 LOAD_CONST               0 (0)
-               172 LOAD_CONST              14 (('Semantic', 'SemanticType', 'Token'))
-               174 IMPORT_NAME             30 (deepsecrets.core.model.token)
-               176 IMPORT_FROM             31 (Semantic)
-               178 STORE_NAME              31 (Semantic)
-               180 IMPORT_FROM             32 (SemanticType)
-               182 STORE_NAME              32 (SemanticType)
-               184 IMPORT_FROM             16 (Token)
-               186 STORE_NAME              16 (Token)
-               188 POP_TOP
+    16         186 LOAD_CONST               0 (0)
+               188 LOAD_CONST              14 (('SpotImprovements',))
+               190 IMPORT_NAME             33 (deepsecrets.core.tokenizers.helpers.spot_improvements)
+               192 IMPORT_FROM             34 (SpotImprovements)
+               194 STORE_NAME              34 (SpotImprovements)
+               196 POP_TOP
    
-    25         190 LOAD_CONST               0 (0)
-               192 LOAD_CONST              15 (('SpotImprovements',))
-               194 IMPORT_NAME             33 (deepsecrets.core.tokenizers.lexer.spot_improvements)
-               196 IMPORT_FROM             34 (SpotImprovements)
-               198 STORE_NAME              34 (SpotImprovements)
-               200 POP_TOP
+    17         198 LOAD_CONST               0 (0)
+               200 LOAD_CONST              15 (('token_to_typestream_item', 'types_to_filter_after', 'types_to_filter_before'))
+               202 IMPORT_NAME             35 (deepsecrets.core.tokenizers.helpers.type_stream)
+               204 IMPORT_FROM             36 (token_to_typestream_item)
+               206 STORE_NAME              36 (token_to_typestream_item)
+               208 IMPORT_FROM             37 (types_to_filter_after)
+               210 STORE_NAME              37 (types_to_filter_after)
+               212 IMPORT_FROM             38 (types_to_filter_before)
+               214 STORE_NAME              38 (types_to_filter_before)
+               216 POP_TOP
    
-    26         202 LOAD_CONST               0 (0)
-               204 LOAD_CONST              16 (('token_to_typestream_item', 'types_to_filter_before', 'types_to_filter_after'))
-               206 IMPORT_NAME             35 (deepsecrets.core.tokenizers.lexer.type_stream)
-               208 IMPORT_FROM             36 (token_to_typestream_item)
-               210 STORE_NAME              36 (token_to_typestream_item)
-               212 IMPORT_FROM             37 (types_to_filter_before)
-               214 STORE_NAME              37 (types_to_filter_before)
-               216 IMPORT_FROM             38 (types_to_filter_after)
-               218 STORE_NAME              38 (types_to_filter_after)
-               220 POP_TOP
+    22         218 LOAD_CONST               0 (0)
+               220 LOAD_CONST              16 (('Tokenizer',))
+               222 IMPORT_NAME             39 (deepsecrets.core.tokenizers.itokenizer)
+               224 IMPORT_FROM             40 (Tokenizer)
+               226 STORE_NAME              40 (Tokenizer)
+               228 POP_TOP
    
-    29         222 LOAD_CONST               0 (0)
-               224 LOAD_CONST              17 (('TokenizationException',))
-               226 IMPORT_NAME             39 (deepsecrets.core.utils.exceptions)
-               228 IMPORT_FROM             40 (TokenizationException)
-               230 STORE_NAME              40 (TokenizationException)
-               232 POP_TOP
+    24         230 BUILD_LIST               0
+               232 LOAD_CONST              17 (('\n', '\t', "'", "''", '"', '""'))
+               234 LIST_EXTEND              1
+               236 STORE_NAME              41 (empty_tokens)
    
-    33         234 BUILD_LIST               0
-               236 LOAD_CONST              18 (('\n', '\t', "'", "''", '"', '""'))
-               238 LIST_EXTEND              1
-               240 STORE_NAME              41 (empty_tokens)
-   
-    35         242 PUSH_NULL
-               244 LOAD_BUILD_CLASS
-               246 LOAD_CONST              19 (<code object LexerTokenizer, file "/app/deepsecrets/core/tokenizers/lexer/lexer.py", line 35>)
-               248 MAKE_FUNCTION            0
-               250 LOAD_CONST              20 ('LexerTokenizer')
-               252 LOAD_NAME               23 (Tokenizer)
-               254 PRECALL                  3
-               258 CALL                     3
-               268 STORE_NAME              42 (LexerTokenizer)
-               270 LOAD_CONST              21 (None)
-               272 RETURN_VALUE
+    27         238 PUSH_NULL
+               240 LOAD_BUILD_CLASS
+               242 LOAD_CONST              18 (<code object LexerTokenizer, file "/app/deepsecrets/core/tokenizers/lexer.py", line 27>)
+               244 MAKE_FUNCTION            0
+               246 LOAD_CONST              19 ('LexerTokenizer')
+               248 LOAD_NAME               40 (Tokenizer)
+               250 PRECALL                  3
+               254 CALL                     3
+               264 STORE_NAME              42 (LexerTokenizer)
+               266 LOAD_CONST              20 (None)
+               268 RETURN_VALUE
    consts
       0
-      ('List', 'Sequence', 'Type')
+      ('List', 'Sequence', 'Set', 'Type', 'Union')
       ('OrderedSet',)
       ('highlight',)
       ('RawTokenFormatter',)
       ('get_lexer_for_filename',)
       ('Lexer', 'RawTokenLexer')
       ('Token',)
       ('ClassNotFound',)
+      ('File',)
       ('Variable',)
-      ('Tokenizer',)
+      ('Semantic', 'SemanticType', 'Token')
       ('Language',)
       ('VariableDetectionRules',)
-      ('File',)
-      ('Semantic', 'SemanticType', 'Token')
       ('SpotImprovements',)
-      ('token_to_typestream_item', 'types_to_filter_before', 'types_to_filter_after')
-      ('TokenizationException',)
+      ('token_to_typestream_item', 'types_to_filter_after', 'types_to_filter_before')
+      ('Tokenizer',)
       ('\n', '\t', "'", "''", '"', '""')
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 5
+         stacksize : 7
          flags     : 0
          code
             0x970065005a0164005a0255006503650464013c0000006505650464023c
             0000006506650464033c0000006404650764056508650919000000000000
-            0000006604640684045a0a640765036602640884045a0b64096503660264
-            0a84045a0c6417640c650d6602640d84055a0e640e6508650f1900000000
-            00000000006602640f84045a1064106511650f1900000000000000000064
-            116511650f190000000000000000006604641284045a12641384005a1364
-            1484005a14641584005a1564165300
-          35           0 RESUME                   0
+            0000006604640684045a0a640765036405650b6503650c66021900000000
+            00000000006604640884045a0d6409650e6602640a84045a0f6416640965
+            0e640565086510190000000000000000006604640c84055a11640d650865
+            10190000000000000000006405640e6604640f84045a1264106513651019
+            000000000000000000641165136510190000000000000000006405650865
+            10190000000000000000006606641284045a146405651565101900000000
+            00000000006602641384045a166405650865101900000000000000000066
+            02641484045a176417641584045a18640e5300
+          27           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('LexerTokenizer')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          37          12 LOAD_NAME                3 (str)
+          28          12 LOAD_NAME                3 (str)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('token_stream')
                       18 STORE_SUBSCR
          
-          38          22 LOAD_NAME                5 (Lexer)
+          29          22 LOAD_NAME                5 (Lexer)
                       24 LOAD_NAME                4 (__annotations__)
                       26 LOAD_CONST               2 ('lexer')
                       28 STORE_SUBSCR
          
-          39          32 LOAD_NAME                6 (Language)
+          30          32 LOAD_NAME                6 (Language)
                       34 LOAD_NAME                4 (__annotations__)
                       36 LOAD_CONST               3 ('language')
                       38 STORE_SUBSCR
          
-          41          42 LOAD_CONST               4 ('token')
+          32          42 LOAD_CONST               4 ('token')
                       44 LOAD_NAME                7 (PygmentsToken)
                       46 LOAD_CONST               5 ('return')
                       48 LOAD_NAME                8 (List)
                       50 LOAD_NAME                9 (Type)
                       52 BINARY_SUBSCR
                       62 BUILD_TUPLE              4
-                      64 LOAD_CONST               6 (<code object _get_types_for_token, file "/app/deepsecrets/core/tokenizers/lexer/lexer.py", line 41>)
+                      64 LOAD_CONST               6 (<code object _get_types_for_token, file "/app/deepsecrets/core/tokenizers/lexer.py", line 32>)
                       66 MAKE_FUNCTION            4 (annotations)
                       68 STORE_NAME              10 (_get_types_for_token)
          
-          51          70 LOAD_CONST               7 ('content')
+          42          70 LOAD_CONST               7 ('content')
                       72 LOAD_NAME                3 (str)
-                      74 BUILD_TUPLE              2
-                      76 LOAD_CONST               8 (<code object sanitize, file "/app/deepsecrets/core/tokenizers/lexer/lexer.py", line 51>)
-                      78 MAKE_FUNCTION            4 (annotations)
-                      80 STORE_NAME              11 (sanitize)
+                      74 LOAD_CONST               5 ('return')
+                      76 LOAD_NAME               11 (Union)
+                      78 LOAD_NAME                3 (str)
+                      80 LOAD_NAME               12 (bool)
+                      82 BUILD_TUPLE              2
+                      84 BINARY_SUBSCR
+                      94 BUILD_TUPLE              4
+                      96 LOAD_CONST               8 (<code object sanitize, file "/app/deepsecrets/core/tokenizers/lexer.py", line 42>)
+                      98 MAKE_FUNCTION            4 (annotations)
+                     100 STORE_NAME              13 (sanitize)
          
-          73          82 LOAD_CONST               9 ('string')
-                      84 LOAD_NAME                3 (str)
-                      86 BUILD_TUPLE              2
-                      88 LOAD_CONST              10 (<code object get_token_for_string, file "/app/deepsecrets/core/tokenizers/lexer/lexer.py", line 73>)
-                      90 MAKE_FUNCTION            4 (annotations)
-                      92 STORE_NAME              12 (get_token_for_string)
+          63         102 LOAD_CONST               9 ('file')
+                     104 LOAD_NAME               14 (File)
+                     106 BUILD_TUPLE              2
+                     108 LOAD_CONST              10 (<code object _find_lexer_for_file, file "/app/deepsecrets/core/tokenizers/lexer.py", line 63>)
+                     110 MAKE_FUNCTION            4 (annotations)
+                     112 STORE_NAME              15 (_find_lexer_for_file)
          
-          79          94 LOAD_CONST              23 ((True,))
-                      96 LOAD_CONST              12 ('file')
-                      98 LOAD_NAME               13 (File)
-                     100 BUILD_TUPLE              2
-                     102 LOAD_CONST              13 (<code object tokenize, file "/app/deepsecrets/core/tokenizers/lexer/lexer.py", line 79>)
-                     104 MAKE_FUNCTION            5 (defaults, annotations)
-                     106 STORE_NAME              14 (tokenize)
+          83         114 LOAD_CONST              22 ((True,))
+                     116 LOAD_CONST               9 ('file')
+                     118 LOAD_NAME               14 (File)
+                     120 LOAD_CONST               5 ('return')
+                     122 LOAD_NAME                8 (List)
+                     124 LOAD_NAME               16 (Token)
+                     126 BINARY_SUBSCR
+                     136 BUILD_TUPLE              4
+                     138 LOAD_CONST              12 (<code object tokenize, file "/app/deepsecrets/core/tokenizers/lexer.py", line 83>)
+                     140 MAKE_FUNCTION            5 (defaults, annotations)
+                     142 STORE_NAME              17 (tokenize)
          
-         140         108 LOAD_CONST              14 ('tokens')
-                     110 LOAD_NAME                8 (List)
-                     112 LOAD_NAME               15 (Token)
-                     114 BINARY_SUBSCR
-                     124 BUILD_TUPLE              2
-                     126 LOAD_CONST              15 (<code object add_to_token_stream, file "/app/deepsecrets/core/tokenizers/lexer/lexer.py", line 140>)
-                     128 MAKE_FUNCTION            4 (annotations)
-                     130 STORE_NAME              16 (add_to_token_stream)
-         
-         145         132 LOAD_CONST              16 ('tokens_all')
-                     134 LOAD_NAME               17 (Sequence)
-                     136 LOAD_NAME               15 (Token)
-                     138 BINARY_SUBSCR
-                     148 LOAD_CONST              17 ('tokens_to_be_excluded')
-                     150 LOAD_NAME               17 (Sequence)
-                     152 LOAD_NAME               15 (Token)
-                     154 BINARY_SUBSCR
+         131         144 LOAD_CONST              13 ('tokens')
+                     146 LOAD_NAME                8 (List)
+                     148 LOAD_NAME               16 (Token)
+                     150 BINARY_SUBSCR
+                     160 LOAD_CONST               5 ('return')
+                     162 LOAD_CONST              14 (None)
                      164 BUILD_TUPLE              4
-                     166 LOAD_CONST              18 (<code object final_cleanup, file "/app/deepsecrets/core/tokenizers/lexer/lexer.py", line 145>)
+                     166 LOAD_CONST              15 (<code object add_to_token_stream, file "/app/deepsecrets/core/tokenizers/lexer.py", line 131>)
                      168 MAKE_FUNCTION            4 (annotations)
-                     170 STORE_NAME              18 (final_cleanup)
+                     170 STORE_NAME              18 (add_to_token_stream)
+         
+         135         172 LOAD_CONST              16 ('tokens_all')
+                     174 LOAD_NAME               19 (Sequence)
+                     176 LOAD_NAME               16 (Token)
+                     178 BINARY_SUBSCR
+                     188 LOAD_CONST              17 ('tokens_to_be_excluded')
+                     190 LOAD_NAME               19 (Sequence)
+                     192 LOAD_NAME               16 (Token)
+                     194 BINARY_SUBSCR
+                     204 LOAD_CONST               5 ('return')
+                     206 LOAD_NAME                8 (List)
+                     208 LOAD_NAME               16 (Token)
+                     210 BINARY_SUBSCR
+                     220 BUILD_TUPLE              6
+                     222 LOAD_CONST              18 (<code object final_cleanup, file "/app/deepsecrets/core/tokenizers/lexer.py", line 135>)
+                     224 MAKE_FUNCTION            4 (annotations)
+                     226 STORE_NAME              20 (final_cleanup)
          
-         165         172 LOAD_CONST              19 (<code object deep_analyze, file "/app/deepsecrets/core/tokenizers/lexer/lexer.py", line 165>)
-                     174 MAKE_FUNCTION            0
-                     176 STORE_NAME              19 (deep_analyze)
+         155         228 LOAD_CONST               5 ('return')
+                     230 LOAD_NAME               21 (Set)
+                     232 LOAD_NAME               16 (Token)
+                     234 BINARY_SUBSCR
+                     244 BUILD_TUPLE              2
+                     246 LOAD_CONST              19 (<code object deep_analyze, file "/app/deepsecrets/core/tokenizers/lexer.py", line 155>)
+                     248 MAKE_FUNCTION            4 (annotations)
+                     250 STORE_NAME              22 (deep_analyze)
          
-         187         178 LOAD_CONST              20 (<code object get_variables, file "/app/deepsecrets/core/tokenizers/lexer/lexer.py", line 187>)
-                     180 MAKE_FUNCTION            0
-                     182 STORE_NAME              20 (get_variables)
+         177         252 LOAD_CONST               5 ('return')
+                     254 LOAD_NAME                8 (List)
+                     256 LOAD_NAME               16 (Token)
+                     258 BINARY_SUBSCR
+                     268 BUILD_TUPLE              2
+                     270 LOAD_CONST              20 (<code object get_variables, file "/app/deepsecrets/core/tokenizers/lexer.py", line 177>)
+                     272 MAKE_FUNCTION            4 (annotations)
+                     274 STORE_NAME              23 (get_variables)
          
-         203         184 LOAD_CONST              21 (<code object print_token_type_stream, file "/app/deepsecrets/core/tokenizers/lexer/lexer.py", line 203>)
-                     186 MAKE_FUNCTION            0
-                     188 STORE_NAME              21 (print_token_type_stream)
-                     190 LOAD_CONST              22 (None)
-                     192 RETURN_VALUE
+         193         276 LOAD_CONST              23 (('return', None))
+                     278 LOAD_CONST              21 (<code object print_token_type_stream, file "/app/deepsecrets/core/tokenizers/lexer.py", line 193>)
+                     280 MAKE_FUNCTION            4 (annotations)
+                     282 STORE_NAME              24 (print_token_type_stream)
+                     284 LOAD_CONST              14 (None)
+                     286 RETURN_VALUE
          consts
             'LexerTokenizer'
             'token_stream'
             'lexer'
             'language'
             'token'
             'return'
@@ -307,65 +333,65 @@
                   0x970067007d027c02a00000000000000000000000000000000000000000
                   007c01a6010000ab01000000000000000001007c016a0100000000000000
                   0081417c016a0100000000000000007404000000000000000000006b0200
                   00000072027c0253007c00a0030000000000000000000000000000000000
                   0000007c016a010000000000000000a6010000ab0100000000000000007d
                   037c02a00400000000000000000000000000000000000000007c03a60100
                   00ab01000000000000000001007c025300
-                41           0 RESUME                   0
+                32           0 RESUME                   0
                
-                42           2 BUILD_LIST               0
+                33           2 BUILD_LIST               0
                              4 STORE_FAST               2 (types)
                
-                43           6 LOAD_FAST                2 (types)
+                34           6 LOAD_FAST                2 (types)
                              8 LOAD_METHOD              0 (append)
                             30 LOAD_FAST                1 (token)
                             32 PRECALL                  1
                             36 CALL                     1
                             46 POP_TOP
                
-                44          48 LOAD_FAST                1 (token)
+                35          48 LOAD_FAST                1 (token)
                             50 LOAD_ATTR                1 (parent)
                             60 POP_JUMP_FORWARD_IF_NONE    65 (to 192)
                
-                45          62 LOAD_FAST                1 (token)
+                36          62 LOAD_FAST                1 (token)
                             64 LOAD_ATTR                1 (parent)
                             74 LOAD_GLOBAL              4 (PygmentsToken)
                             86 COMPARE_OP               2 (==)
                             92 POP_JUMP_FORWARD_IF_FALSE     2 (to 98)
                
-                46          94 LOAD_FAST                2 (types)
+                37          94 LOAD_FAST                2 (types)
                             96 RETURN_VALUE
                
-                47     >>   98 LOAD_FAST                0 (self)
+                38     >>   98 LOAD_FAST                0 (self)
                            100 LOAD_METHOD              3 (_get_types_for_token)
                            122 LOAD_FAST                1 (token)
                            124 LOAD_ATTR                1 (parent)
                            134 PRECALL                  1
                            138 CALL                     1
                            148 STORE_FAST               3 (deep)
                
-                48         150 LOAD_FAST                2 (types)
+                39         150 LOAD_FAST                2 (types)
                            152 LOAD_METHOD              4 (extend)
                            174 LOAD_FAST                3 (deep)
                            176 PRECALL                  1
                            180 CALL                     1
                            190 POP_TOP
                
-                49     >>  192 LOAD_FAST                2 (types)
+                40     >>  192 LOAD_FAST                2 (types)
                            194 RETURN_VALUE
                consts
                   None
                names      ('append', 'parent', 'PygmentsToken', '_get_types_for_token', 'extend')
                varnames   ('self', 'token', 'types', 'deep')
                freevars   ()
                cellvars   ()
-               filename   '/app/deepsecrets/core/tokenizers/lexer/lexer.py'
+               filename   '/app/deepsecrets/core/tokenizers/lexer.py'
                name       '_get_types_for_token'
-               firstlineno 41
+               firstlineno 32
                lnotab 0x020104012a010e012001040134012a01
             'content'
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 4
                flags     : 3
@@ -376,30 +402,30 @@
                   0100000000720664046b020000000072056e0201006e0264055300740300
                   0000000000000000007c01a6010000ab01000000000000000064066b0400
                   00000072167c0164071900000000000000000064086b0200000000720a7c
                   01640064078502190000000000000000007d017c01640419000000000000
                   0000007c016407190000000000000000006b020000000072147c01640419
                   0000000000000000007c027600720a7c0164066407850219000000000000
                   0000007d017c017c0276007202640553007c015300
-                51           0 RESUME                   0
+                42           0 RESUME                   0
                
-                53           2 BUILD_LIST               0
+                43           2 BUILD_LIST               0
                              4 LOAD_CONST               1 (("'", "''", '"', '""'))
                              6 LIST_EXTEND              1
                              8 STORE_FAST               2 (quotes)
                
-                55          10 LOAD_FAST                1 (content)
+                45          10 LOAD_FAST                1 (content)
                             12 LOAD_METHOD              0 (replace)
                             34 LOAD_CONST               2 (' ')
                             36 LOAD_CONST               3 ('')
                             38 PRECALL                  2
                             42 CALL                     2
                             52 STORE_FAST               3 (whitespace_cleaned)
                
-                56          54 LOAD_CONST               4 (0)
+                46          54 LOAD_CONST               4 (0)
                             56 LOAD_GLOBAL              3 (NULL + len)
                             68 LOAD_FAST                3 (whitespace_cleaned)
                             70 PRECALL                  1
                             74 CALL                     1
                             84 SWAP                     2
                             86 COPY                     2
                             88 COMPARE_OP               1 (<=)
@@ -407,70 +433,70 @@
                             96 LOAD_CONST               4 (0)
                             98 COMPARE_OP               2 (==)
                            104 POP_JUMP_FORWARD_IF_FALSE     5 (to 116)
                            106 JUMP_FORWARD             2 (to 112)
                        >>  108 POP_TOP
                            110 JUMP_FORWARD             2 (to 116)
                
-                57     >>  112 LOAD_CONST               5 (False)
+                47     >>  112 LOAD_CONST               5 (False)
                            114 RETURN_VALUE
                
-                61     >>  116 LOAD_GLOBAL              3 (NULL + len)
+                51     >>  116 LOAD_GLOBAL              3 (NULL + len)
                            128 LOAD_FAST                1 (content)
                            130 PRECALL                  1
                            134 CALL                     1
                            144 LOAD_CONST               6 (1)
                            146 COMPARE_OP               4 (>)
                            152 POP_JUMP_FORWARD_IF_FALSE    22 (to 198)
                            154 LOAD_FAST                1 (content)
                            156 LOAD_CONST               7 (-1)
                            158 BINARY_SUBSCR
                            168 LOAD_CONST               8 ('\n')
                            170 COMPARE_OP               2 (==)
                            176 POP_JUMP_FORWARD_IF_FALSE    10 (to 198)
                
-                62         178 LOAD_FAST                1 (content)
+                52         178 LOAD_FAST                1 (content)
                            180 LOAD_CONST               0 (None)
                            182 LOAD_CONST               7 (-1)
                            184 BUILD_SLICE              2
                            186 BINARY_SUBSCR
                            196 STORE_FAST               1 (content)
                
-                64     >>  198 LOAD_FAST                1 (content)
+                54     >>  198 LOAD_FAST                1 (content)
                            200 LOAD_CONST               4 (0)
                            202 BINARY_SUBSCR
                            212 LOAD_FAST                1 (content)
                            214 LOAD_CONST               7 (-1)
                            216 BINARY_SUBSCR
                            226 COMPARE_OP               2 (==)
                            232 POP_JUMP_FORWARD_IF_FALSE    20 (to 274)
                
-                65         234 LOAD_FAST                1 (content)
+                55         234 LOAD_FAST                1 (content)
                            236 LOAD_CONST               4 (0)
                            238 BINARY_SUBSCR
                            248 LOAD_FAST                2 (quotes)
                            250 CONTAINS_OP              0
                            252 POP_JUMP_FORWARD_IF_FALSE    10 (to 274)
                
-                66         254 LOAD_FAST                1 (content)
+                56         254 LOAD_FAST                1 (content)
                            256 LOAD_CONST               6 (1)
                            258 LOAD_CONST               7 (-1)
                            260 BUILD_SLICE              2
                            262 BINARY_SUBSCR
                            272 STORE_FAST               1 (content)
                
-                68     >>  274 LOAD_FAST                1 (content)
+                58     >>  274 LOAD_FAST                1 (content)
                            276 LOAD_FAST                2 (quotes)
                            278 CONTAINS_OP              0
                            280 POP_JUMP_FORWARD_IF_FALSE     2 (to 286)
                
-                69         282 LOAD_CONST               5 (False)
+                59         282 LOAD_CONST               5 (False)
                            284 RETURN_VALUE
                
-                71     >>  286 LOAD_FAST                1 (content)
+                61     >>  286 LOAD_FAST                1 (content)
                            288 RETURN_VALUE
                consts
                   None
                   ("'", "''", '"', '""')
                   ' '
                   ''
                   0
@@ -478,487 +504,511 @@
                   1
                   -1
                   '\n'
                names      ('replace', 'len')
                varnames   ('self', 'content', 'quotes', 'whitespace_cleaned')
                freevars   ()
                cellvars   ()
-               filename   '/app/deepsecrets/core/tokenizers/lexer/lexer.py'
+               filename   '/app/deepsecrets/core/tokenizers/lexer.py'
                name       'sanitize'
-               firstlineno 51
-               lnotab 0x020208022c013a0104043e01140224011401140208010402
-            'string'
+               firstlineno 42
+               lnotab 0x020108022c013a0104043e01140224011401140208010402
+            'file'
             code
                argcount  : 2
-               nlocals   : 4
-               stacksize : 3
+               nlocals   : 3
+               stacksize : 5
                flags     : 3
                code
-                  0x97007401000000000000000000007c006a010000000000000000a60100
-                  00ab01000000000000000044005d145c0200007d027d037c017c036a0200
-                  00000000000000760072067c027c0366026302010053008c1564015300
-                73           0 RESUME                   0
+                  0x970064007d027c016a0000000000000000008127090074030000000000
+                  00000000007c016a020000000000000000a6010000ab0100000000000000
+                  007d027c025300230074060000000000000000000024007203010059006e
+                  0477007803590077017c016a040000000000000000813109007403000000
+                  000000000000007c016a0200000000000000009b0064017c016a04000000
+                  00000000009b009d03a6010000ab0100000000000000007d027c02530023
+                  0074060000000000000000000024007203010059006e0477007803590077
+                  017c025300
+                63           0 RESUME                   0
+               
+                64           2 LOAD_CONST               0 (None)
+                             4 STORE_FAST               2 (lexer)
+               
+                65           6 LOAD_FAST                1 (file)
+                             8 LOAD_ATTR                0 (extension)
+                            18 POP_JUMP_FORWARD_IF_NONE    39 (to 98)
+               
+                66          20 NOP
+               
+                67          22 LOAD_GLOBAL              3 (NULL + get_lexer_for_filename)
+                            34 LOAD_FAST                1 (file)
+                            36 LOAD_ATTR                2 (path)
+                            46 PRECALL                  1
+                            50 CALL                     1
+                            60 STORE_FAST               2 (lexer)
+               
+                68          62 LOAD_FAST                2 (lexer)
+                            64 RETURN_VALUE
+                       >>   66 PUSH_EXC_INFO
+               
+                69          68 LOAD_GLOBAL              6 (ClassNotFound)
+                            80 CHECK_EXC_MATCH
+                            82 POP_JUMP_FORWARD_IF_FALSE     3 (to 90)
+                            84 POP_TOP
+               
+                70          86 POP_EXCEPT
+                            88 JUMP_FORWARD             4 (to 98)
+               
+                69     >>   90 RERAISE                  0
+                       >>   92 COPY                     3
+                            94 POP_EXCEPT
+                            96 RERAISE                  1
+               
+                72     >>   98 LOAD_FAST                1 (file)
+                           100 LOAD_ATTR                4 (guessed_extension)
+                           110 POP_JUMP_FORWARD_IF_NONE    49 (to 210)
+               
+                73         112 NOP
+               
+                74         114 LOAD_GLOBAL              3 (NULL + get_lexer_for_filename)
+                           126 LOAD_FAST                1 (file)
+                           128 LOAD_ATTR                2 (path)
+                           138 FORMAT_VALUE             0
+                           140 LOAD_CONST               1 ('.')
+                           142 LOAD_FAST                1 (file)
+                           144 LOAD_ATTR                4 (guessed_extension)
+                           154 FORMAT_VALUE             0
+                           156 BUILD_STRING             3
+                           158 PRECALL                  1
+                           162 CALL                     1
+                           172 STORE_FAST               2 (lexer)
+               
+                75         174 LOAD_FAST                2 (lexer)
+                           176 RETURN_VALUE
+                       >>  178 PUSH_EXC_INFO
+               
+                76         180 LOAD_GLOBAL              6 (ClassNotFound)
+                           192 CHECK_EXC_MATCH
+                           194 POP_JUMP_FORWARD_IF_FALSE     3 (to 202)
+                           196 POP_TOP
+               
+                77         198 POP_EXCEPT
+                           200 JUMP_FORWARD             4 (to 210)
+               
+                76     >>  202 RERAISE                  0
+                       >>  204 COPY                     3
+                           206 POP_EXCEPT
+                           208 RERAISE                  1
                
-                74           2 LOAD_GLOBAL              1 (NULL + enumerate)
-                            14 LOAD_FAST                0 (self)
-                            16 LOAD_ATTR                1 (tokens)
-                            26 PRECALL                  1
-                            30 CALL                     1
-                            40 GET_ITER
-                       >>   42 FOR_ITER                20 (to 84)
-                            44 UNPACK_SEQUENCE          2
-                            48 STORE_FAST               2 (i)
-                            50 STORE_FAST               3 (token)
-               
-                75          52 LOAD_FAST                1 (string)
-                            54 LOAD_FAST                3 (token)
-                            56 LOAD_ATTR                2 (content)
-                            66 CONTAINS_OP              0
-                            68 POP_JUMP_FORWARD_IF_FALSE     6 (to 82)
-               
-                76          70 LOAD_FAST                2 (i)
-                            72 LOAD_FAST                3 (token)
-                            74 BUILD_TUPLE              2
-                            76 SWAP                     2
-                            78 POP_TOP
-                            80 RETURN_VALUE
-               
-                75     >>   82 JUMP_BACKWARD           21 (to 42)
-               
-                77     >>   84 LOAD_CONST               1 ((None, None))
-                            86 RETURN_VALUE
+                79     >>  210 LOAD_FAST                2 (lexer)
+                           212 RETURN_VALUE
+               ExceptionTable:
+                 22 to 62 -> 66 [0]
+                 66 to 84 -> 92 [1] lasti
+                 90 to 90 -> 92 [1] lasti
+                 114 to 174 -> 178 [0]
+                 178 to 196 -> 204 [1] lasti
+                 202 to 202 -> 204 [1] lasti
                consts
                   None
-                  (None, None)
-               names      ('enumerate', 'tokens', 'content')
-               varnames   ('self', 'string', 'i', 'token')
+                  '.'
+               names      ('extension', 'get_lexer_for_filename', 'path', 'ClassNotFound', 'guessed_extension')
+               varnames   ('self', 'file', 'lexer')
                freevars   ()
                cellvars   ()
-               filename   '/app/deepsecrets/core/tokenizers/lexer/lexer.py'
-               name       'get_token_for_string'
-               firstlineno 73
-               lnotab 0x0201320112010cff0202
+               filename   '/app/deepsecrets/core/tokenizers/lexer.py'
+               name       '_find_lexer_for_file'
+               firstlineno 63
+               lnotab
+                  0x020104010e01020128010601120104ff08030e0102013c010601120104
+                  ff0803
             True
-            'file'
             code
                argcount  : 3
                nlocals   : 18
                stacksize : 7
                flags     : 3
                code
-                  0x970064017c005f00000000000000000009007403000000000000000000
-                  007c016a020000000000000000a6010000ab0100000000000000007c005f
-                  0300000000000000006e1723007408000000000000000000002400720a01
-                  0064007c005f03000000000000000059006e0477007803590077017c006a
-                  03000000000000000073077c006a05000000000000000053000900740d00
-                  0000000000000000006a0700000000000000007c006a0300000000000000
-                  006a080000000000000000640219000000000000000000a6010000ab0100
-                  000000000000007c005f0900000000000000006e2e230074140000000000
-                  0000000000240072210100740d000000000000000000006a070000000000
-                  0000007c016a0b0000000000000000a6010000ab0100000000000000007c
-                  005f09000000000000000059006e04770078035900770174190000000000
-                  00000000007c016a0d00000000000000007c006a03000000000000000074
-                  1d00000000000000000000a6000000ab000000000000000000a6030000ab
-                  0300000000000000007d03741f0000000000000000000074210000000000
-                  0000000000a6000000ab000000000000000000a011000000000000000000
-                  00000000000000000000007c03a6010000ab010000000000000000a60100
-                  00ab0100000000000000007d047425000000000000000000007c006a0900
-                  00000000000000ac03a6010000ab0100000000000000007d0564027d0674
-                  27000000000000000000007c04a6010000ab010000000000000000440090
-                  015d145c0200007d077d087c086404190000000000000000007d097c00a0
-                  1400000000000000000000000000000000000000007c0864021900000000
-                  0000000000a6010000ab0100000000000000007d0a7c067d0b7c0b742b00
-                  0000000000000000007c09a6010000ab0100000000000000007a0000007d
-                  0c7c0c7d0609007c00a01600000000000000000000000000000000000000
-                  007c09a6010000ab0100000000000000007d097c0973018c587c01a01700
-                  000000000000000000000000000000000000007c097c0b64047a0a00007c
-                  0c64047a0000006702ac05a6020000ab0200000000000000007d0d743100
-                  0000000000000000007c017c097c0dac06a6030000ab0300000000000000
-                  007d0e7c0ea01900000000000000000000000000000000000000007c0aa6
-                  010000ab01000000000000000001007c05a01a0000000000000000000000
-                  0000000000000000007c006a0500000000000000007c006a000000000000
-                  0000007c0ea6030000ab0300000000000000007d0f7c006a050000000000
-                  000000a01b00000000000000000000000000000000000000007c0fa60100
-                  00ab01000000000000000001007c00a01c00000000000000000000000000
-                  000000000000007c0fa6010000ab01000000000000000001008cef230074
-                  3a000000000000000000002400721a7d10743d000000000000000000007c
-                  10a6010000ab0100000000000000000100590064007d107e1090018c0e64
-                  007d107e107701770078035900770167007d117c006a1f00000000000000
-                  006a2000000000000000006407750072147c00a021000000000000000000
-                  0000000000000000000000a6000000ab0000000000000000007d117c0272
-                  1b7c00a02200000000000000000000000000000000000000007c006a0500
-                  000000000000007c11a6020000ab0200000000000000006e13741f000000
-                  000000000000007c006a050000000000000000a6010000ab010000000000
-                  0000005300
-                79           0 RESUME                   0
+                  0x970064017c005f0000000000000000007c00a001000000000000000000
+                  00000000000000000000007c01a6010000ab0100000000000000007c005f
+                  0200000000000000007c006a02000000000000000073077c006a03000000
+                  0000000000530009007409000000000000000000006a0500000000000000
+                  007c006a0200000000000000006a06000000000000000064021900000000
+                  0000000000a6010000ab0100000000000000007c005f0700000000000000
+                  006e2e230074100000000000000000000024007221010074090000000000
+                  00000000006a0500000000000000007c016a090000000000000000a60100
+                  00ab0100000000000000007c005f07000000000000000059006e04770078
+                  03590077017415000000000000000000007c016a0b00000000000000007c
+                  006a020000000000000000741900000000000000000000a6000000ab0000
+                  00000000000000a6030000ab0300000000000000007d03741b0000000000
+                  0000000000741d00000000000000000000a6000000ab0000000000000000
+                  00a00f00000000000000000000000000000000000000007c03a6010000ab
+                  010000000000000000a6010000ab0100000000000000007d047421000000
+                  000000000000007c006a070000000000000000ac03a6010000ab01000000
+                  00000000007d0564027d067423000000000000000000007c04a6010000ab
+                  010000000000000000440090015d145c0200007d077d087c086404190000
+                  000000000000007d097c00a0120000000000000000000000000000000000
+                  0000007c08640219000000000000000000a6010000ab0100000000000000
+                  007d0a7c067d0b7c0b7427000000000000000000007c09a6010000ab0100
+                  000000000000007a0000007d0c7c0c7d0609007c00a01400000000000000
+                  000000000000000000000000007c09a6010000ab0100000000000000007d
+                  097c0973018c587c01a01500000000000000000000000000000000000000
+                  007c097c0b64047a0a00007c0c64047a0000006702ac05a6020000ab0200
+                  000000000000007d0d742d000000000000000000007c017c097c0dac06a6
+                  030000ab0300000000000000007d0e7c0ea0170000000000000000000000
+                  0000000000000000007c0aa6010000ab01000000000000000001007c05a0
+                  1800000000000000000000000000000000000000007c006a030000000000
+                  0000007c006a0000000000000000007c0ea6030000ab0300000000000000
+                  007d0f7c006a030000000000000000a01900000000000000000000000000
+                  000000000000007c0fa6010000ab01000000000000000001007c00a01a00
+                  000000000000000000000000000000000000007c0fa6010000ab01000000
+                  000000000001008cef23007436000000000000000000002400721a7d1074
+                  39000000000000000000007c10a6010000ab010000000000000000010059
+                  0064007d107e1090018c0e64007d107e107701770078035900770167007d
+                  117c006a1d00000000000000006a1e00000000000000006407750072147c
+                  00a01f0000000000000000000000000000000000000000a6000000ab0000
+                  000000000000007d117c02721b7c00a02000000000000000000000000000
+                  000000000000007c006a0300000000000000007c11a6020000ab02000000
+                  00000000006e13741b000000000000000000007c006a0300000000000000
+                  00a6010000ab0100000000000000005300
+                83           0 RESUME                   0
                
-                80           2 LOAD_CONST               1 ('')
+                84           2 LOAD_CONST               1 ('')
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (token_stream)
                
-                82          16 NOP
-               
-                83          18 LOAD_GLOBAL              3 (NULL + get_lexer_for_filename)
-                            30 LOAD_FAST                1 (file)
-                            32 LOAD_ATTR                2 (path)
+                87          16 LOAD_FAST                0 (self)
+                            18 LOAD_METHOD              1 (_find_lexer_for_file)
+                            40 LOAD_FAST                1 (file)
                             42 PRECALL                  1
                             46 CALL                     1
                             56 LOAD_FAST                0 (self)
-                            58 STORE_ATTR               3 (lexer)
-                            68 JUMP_FORWARD            23 (to 116)
-                       >>   70 PUSH_EXC_INFO
-               
-                84          72 LOAD_GLOBAL              8 (ClassNotFound)
-                            84 CHECK_EXC_MATCH
-                            86 POP_JUMP_FORWARD_IF_FALSE    10 (to 108)
-                            88 POP_TOP
-               
-                85          90 LOAD_CONST               0 (None)
-                            92 LOAD_FAST                0 (self)
-                            94 STORE_ATTR               3 (lexer)
-                           104 POP_EXCEPT
-                           106 JUMP_FORWARD             4 (to 116)
-               
-                84     >>  108 RERAISE                  0
-                       >>  110 COPY                     3
-                           112 POP_EXCEPT
-                           114 RERAISE                  1
-               
-                87     >>  116 LOAD_FAST                0 (self)
-                           118 LOAD_ATTR                3 (lexer)
-                           128 POP_JUMP_FORWARD_IF_TRUE     7 (to 144)
-               
-                88         130 LOAD_FAST                0 (self)
-                           132 LOAD_ATTR                5 (tokens)
-                           142 RETURN_VALUE
+                            58 STORE_ATTR               2 (lexer)
                
-                90     >>  144 NOP
-               
-                91         146 LOAD_GLOBAL             13 (NULL + Language)
-                           158 LOAD_ATTR                7 (from_text)
+                88          68 LOAD_FAST                0 (self)
+                            70 LOAD_ATTR                2 (lexer)
+                            80 POP_JUMP_FORWARD_IF_TRUE     7 (to 96)
+               
+                89          82 LOAD_FAST                0 (self)
+                            84 LOAD_ATTR                3 (tokens)
+                            94 RETURN_VALUE
+               
+                91     >>   96 NOP
+               
+                92          98 LOAD_GLOBAL              9 (NULL + Language)
+                           110 LOAD_ATTR                5 (from_text)
+                           120 LOAD_FAST                0 (self)
+                           122 LOAD_ATTR                2 (lexer)
+                           132 LOAD_ATTR                6 (filenames)
+                           142 LOAD_CONST               2 (0)
+                           144 BINARY_SUBSCR
+                           154 PRECALL                  1
+                           158 CALL                     1
                            168 LOAD_FAST                0 (self)
-                           170 LOAD_ATTR                3 (lexer)
-                           180 LOAD_ATTR                8 (filenames)
-                           190 LOAD_CONST               2 (0)
-                           192 BINARY_SUBSCR
-                           202 PRECALL                  1
-                           206 CALL                     1
-                           216 LOAD_FAST                0 (self)
-                           218 STORE_ATTR               9 (language)
-                           228 JUMP_FORWARD            46 (to 322)
-                       >>  230 PUSH_EXC_INFO
-               
-                92         232 LOAD_GLOBAL             20 (ValueError)
-                           244 CHECK_EXC_MATCH
-                           246 POP_JUMP_FORWARD_IF_FALSE    33 (to 314)
-                           248 POP_TOP
-               
-                93         250 LOAD_GLOBAL             13 (NULL + Language)
-                           262 LOAD_ATTR                7 (from_text)
-                           272 LOAD_FAST                1 (file)
-                           274 LOAD_ATTR               11 (extension)
-                           284 PRECALL                  1
-                           288 CALL                     1
+                           170 STORE_ATTR               7 (language)
+                           180 JUMP_FORWARD            46 (to 274)
+                       >>  182 PUSH_EXC_INFO
+               
+                93         184 LOAD_GLOBAL             16 (ValueError)
+                           196 CHECK_EXC_MATCH
+                           198 POP_JUMP_FORWARD_IF_FALSE    33 (to 266)
+                           200 POP_TOP
+               
+                94         202 LOAD_GLOBAL              9 (NULL + Language)
+                           214 LOAD_ATTR                5 (from_text)
+                           224 LOAD_FAST                1 (file)
+                           226 LOAD_ATTR                9 (extension)
+                           236 PRECALL                  1
+                           240 CALL                     1
+                           250 LOAD_FAST                0 (self)
+                           252 STORE_ATTR               7 (language)
+                           262 POP_EXCEPT
+                           264 JUMP_FORWARD             4 (to 274)
+               
+                93     >>  266 RERAISE                  0
+                       >>  268 COPY                     3
+                           270 POP_EXCEPT
+                           272 RERAISE                  1
+               
+                96     >>  274 LOAD_GLOBAL             21 (NULL + highlight)
+                           286 LOAD_FAST                1 (file)
+                           288 LOAD_ATTR               11 (content)
                            298 LOAD_FAST                0 (self)
-                           300 STORE_ATTR               9 (language)
-                           310 POP_EXCEPT
-                           312 JUMP_FORWARD             4 (to 322)
-               
-                92     >>  314 RERAISE                  0
-                       >>  316 COPY                     3
-                           318 POP_EXCEPT
-                           320 RERAISE                  1
-               
-                95     >>  322 LOAD_GLOBAL             25 (NULL + highlight)
-                           334 LOAD_FAST                1 (file)
-                           336 LOAD_ATTR               13 (content)
-                           346 LOAD_FAST                0 (self)
-                           348 LOAD_ATTR                3 (lexer)
-                           358 LOAD_GLOBAL             29 (NULL + RawTokenFormatter)
-                           370 PRECALL                  0
-                           374 CALL                     0
-                           384 PRECALL                  3
-                           388 CALL                     3
-                           398 STORE_FAST               3 (result)
-               
-                96         400 LOAD_GLOBAL             31 (NULL + list)
-                           412 LOAD_GLOBAL             33 (NULL + RawTokenLexer)
-                           424 PRECALL                  0
-                           428 CALL                     0
-                           438 LOAD_METHOD             17 (get_tokens)
-                           460 LOAD_FAST                3 (result)
-                           462 PRECALL                  1
-                           466 CALL                     1
-                           476 PRECALL                  1
-                           480 CALL                     1
-                           490 STORE_FAST               4 (raw_tokens)
-               
-                97         492 LOAD_GLOBAL             37 (NULL + SpotImprovements)
-                           504 LOAD_FAST                0 (self)
-                           506 LOAD_ATTR                9 (language)
-                           516 KW_NAMES                 3
-                           518 PRECALL                  1
-                           522 CALL                     1
-                           532 STORE_FAST               5 (token_improver)
-               
-                99         534 LOAD_CONST               2 (0)
-                           536 STORE_FAST               6 (current_position)
-               
-               101         538 LOAD_GLOBAL             39 (NULL + enumerate)
-                           550 LOAD_FAST                4 (raw_tokens)
-                           552 PRECALL                  1
-                           556 CALL                     1
-                           566 GET_ITER
-                       >>  568 EXTENDED_ARG             1
-                           570 FOR_ITER               276 (to 1124)
-                           572 UNPACK_SEQUENCE          2
-                           576 STORE_FAST               7 (i)
-                           578 STORE_FAST               8 (raw_token)
-               
-               102         580 LOAD_FAST                8 (raw_token)
-                           582 LOAD_CONST               4 (1)
-                           584 BINARY_SUBSCR
-                           594 STORE_FAST               9 (content)
-               
-               103         596 LOAD_FAST                0 (self)
-                           598 LOAD_METHOD             20 (_get_types_for_token)
-                           620 LOAD_FAST                8 (raw_token)
-                           622 LOAD_CONST               2 (0)
-                           624 BINARY_SUBSCR
-                           634 PRECALL                  1
-                           638 CALL                     1
-                           648 STORE_FAST              10 (types)
-               
-               104         650 LOAD_FAST                6 (current_position)
-                           652 STORE_FAST              11 (start)
-               
-               105         654 LOAD_FAST               11 (start)
-                           656 LOAD_GLOBAL             43 (NULL + len)
-                           668 LOAD_FAST                9 (content)
-                           670 PRECALL                  1
-                           674 CALL                     1
-                           684 BINARY_OP                0 (+)
-                           688 STORE_FAST              12 (end)
+                           300 LOAD_ATTR                2 (lexer)
+                           310 LOAD_GLOBAL             25 (NULL + RawTokenFormatter)
+                           322 PRECALL                  0
+                           326 CALL                     0
+                           336 PRECALL                  3
+                           340 CALL                     3
+                           350 STORE_FAST               3 (result)
+               
+                97         352 LOAD_GLOBAL             27 (NULL + list)
+                           364 LOAD_GLOBAL             29 (NULL + RawTokenLexer)
+                           376 PRECALL                  0
+                           380 CALL                     0
+                           390 LOAD_METHOD             15 (get_tokens)
+                           412 LOAD_FAST                3 (result)
+                           414 PRECALL                  1
+                           418 CALL                     1
+                           428 PRECALL                  1
+                           432 CALL                     1
+                           442 STORE_FAST               4 (raw_tokens)
+               
+                98         444 LOAD_GLOBAL             33 (NULL + SpotImprovements)
+                           456 LOAD_FAST                0 (self)
+                           458 LOAD_ATTR                7 (language)
+                           468 KW_NAMES                 3
+                           470 PRECALL                  1
+                           474 CALL                     1
+                           484 STORE_FAST               5 (token_improver)
+               
+               100         486 LOAD_CONST               2 (0)
+                           488 STORE_FAST               6 (current_position)
+               
+               102         490 LOAD_GLOBAL             35 (NULL + enumerate)
+                           502 LOAD_FAST                4 (raw_tokens)
+                           504 PRECALL                  1
+                           508 CALL                     1
+                           518 GET_ITER
+                       >>  520 EXTENDED_ARG             1
+                           522 FOR_ITER               276 (to 1076)
+                           524 UNPACK_SEQUENCE          2
+                           528 STORE_FAST               7 (i)
+                           530 STORE_FAST               8 (raw_token)
+               
+               103         532 LOAD_FAST                8 (raw_token)
+                           534 LOAD_CONST               4 (1)
+                           536 BINARY_SUBSCR
+                           546 STORE_FAST               9 (content)
+               
+               104         548 LOAD_FAST                0 (self)
+                           550 LOAD_METHOD             18 (_get_types_for_token)
+                           572 LOAD_FAST                8 (raw_token)
+                           574 LOAD_CONST               2 (0)
+                           576 BINARY_SUBSCR
+                           586 PRECALL                  1
+                           590 CALL                     1
+                           600 STORE_FAST              10 (types)
+               
+               105         602 LOAD_FAST                6 (current_position)
+                           604 STORE_FAST              11 (start)
+               
+               106         606 LOAD_FAST               11 (start)
+                           608 LOAD_GLOBAL             39 (NULL + len)
+                           620 LOAD_FAST                9 (content)
+                           622 PRECALL                  1
+                           626 CALL                     1
+                           636 BINARY_OP                0 (+)
+                           640 STORE_FAST              12 (end)
+               
+               107         642 LOAD_FAST               12 (end)
+                           644 STORE_FAST               6 (current_position)
+               
+               109         646 NOP
+               
+               110         648 LOAD_FAST                0 (self)
+                           650 LOAD_METHOD             20 (sanitize)
+                           672 LOAD_FAST                9 (content)
+                           674 PRECALL                  1
+                           678 CALL                     1
+                           688 STORE_FAST               9 (content)
                
-               106         690 LOAD_FAST               12 (end)
-                           692 STORE_FAST               6 (current_position)
+               111         690 LOAD_FAST                9 (content)
+                           692 POP_JUMP_FORWARD_IF_TRUE     1 (to 696)
                
-               108         694 NOP
+               112         694 JUMP_BACKWARD           88 (to 520)
                
-               109         696 LOAD_FAST                0 (self)
-                           698 LOAD_METHOD             22 (sanitize)
+               114     >>  696 LOAD_FAST                1 (file)
+                           698 LOAD_METHOD             21 (get_span_for_string)
                            720 LOAD_FAST                9 (content)
-                           722 PRECALL                  1
-                           726 CALL                     1
-                           736 STORE_FAST               9 (content)
-               
-               110         738 LOAD_FAST                9 (content)
-                           740 POP_JUMP_FORWARD_IF_TRUE     1 (to 744)
-               
-               111         742 JUMP_BACKWARD           88 (to 568)
-               
-               114     >>  744 LOAD_FAST                1 (file)
-                           746 LOAD_METHOD             23 (get_span_for_string)
-                           768 LOAD_FAST                9 (content)
-                           770 LOAD_FAST               11 (start)
-                           772 LOAD_CONST               4 (1)
-                           774 BINARY_OP               10 (-)
-                           778 LOAD_FAST               12 (end)
-                           780 LOAD_CONST               4 (1)
-                           782 BINARY_OP                0 (+)
-                           786 BUILD_LIST               2
-                           788 KW_NAMES                 5
-                           790 PRECALL                  2
-                           794 CALL                     2
-                           804 STORE_FAST              13 (span)
-               
-               115         806 LOAD_GLOBAL             49 (NULL + Token)
-               
-               116         818 LOAD_FAST                1 (file)
-               
-               117         820 LOAD_FAST                9 (content)
-               
-               118         822 LOAD_FAST               13 (span)
-               
-               115         824 KW_NAMES                 6
-                           826 PRECALL                  3
-                           830 CALL                     3
-                           840 STORE_FAST              14 (token)
-               
-               120         842 LOAD_FAST               14 (token)
-                           844 LOAD_METHOD             25 (set_type)
-                           866 LOAD_FAST               10 (types)
-                           868 PRECALL                  1
-                           872 CALL                     1
-                           882 POP_TOP
-               
-               122         884 LOAD_FAST                5 (token_improver)
-                           886 LOAD_METHOD             26 (improve_token)
-                           908 LOAD_FAST                0 (self)
-                           910 LOAD_ATTR                5 (tokens)
-                           920 LOAD_FAST                0 (self)
-                           922 LOAD_ATTR                0 (token_stream)
-                           932 LOAD_FAST               14 (token)
-                           934 PRECALL                  3
-                           938 CALL                     3
-                           948 STORE_FAST              15 (improved_tokens)
-               
-               124         950 LOAD_FAST                0 (self)
-                           952 LOAD_ATTR                5 (tokens)
-                           962 LOAD_METHOD             27 (extend)
-                           984 LOAD_FAST               15 (improved_tokens)
-                           986 PRECALL                  1
-                           990 CALL                     1
-                          1000 POP_TOP
-               
-               125        1002 LOAD_FAST                0 (self)
-                          1004 LOAD_METHOD             28 (add_to_token_stream)
-                          1026 LOAD_FAST               15 (improved_tokens)
-                          1028 PRECALL                  1
-                          1032 CALL                     1
-                          1042 POP_TOP
-                          1044 JUMP_BACKWARD          239 (to 568)
-                       >> 1046 PUSH_EXC_INFO
-               
-               126        1048 LOAD_GLOBAL             58 (Exception)
-                          1060 CHECK_EXC_MATCH
-                          1062 POP_JUMP_FORWARD_IF_FALSE    26 (to 1116)
-                          1064 STORE_FAST              16 (e)
-               
-               127        1066 LOAD_GLOBAL             61 (NULL + str)
-                          1078 LOAD_FAST               16 (e)
-                          1080 PRECALL                  1
-                          1084 CALL                     1
-                          1094 POP_TOP
-                          1096 POP_EXCEPT
-                          1098 LOAD_CONST               0 (None)
-                          1100 STORE_FAST              16 (e)
-                          1102 DELETE_FAST             16 (e)
-                          1104 EXTENDED_ARG             1
-                          1106 JUMP_BACKWARD          270 (to 568)
-                       >> 1108 LOAD_CONST               0 (None)
-                          1110 STORE_FAST              16 (e)
-                          1112 DELETE_FAST             16 (e)
-                          1114 RERAISE                  1
-               
-               126     >> 1116 RERAISE                  0
-                       >> 1118 COPY                     3
-                          1120 POP_EXCEPT
-                          1122 RERAISE                  1
-               
-               129     >> 1124 BUILD_LIST               0
-                          1126 STORE_FAST              17 (tokens_to_be_excluded)
-               
-               130        1128 LOAD_FAST                0 (self)
-                          1130 LOAD_ATTR               31 (settings)
-                          1140 LOAD_ATTR               32 (deep_token_inspection)
-                          1150 LOAD_CONST               7 (True)
-                          1152 IS_OP                    0
-                          1154 POP_JUMP_FORWARD_IF_FALSE    20 (to 1196)
-               
-               131        1156 LOAD_FAST                0 (self)
-                          1158 LOAD_METHOD             33 (deep_analyze)
-                          1180 PRECALL                  0
-                          1184 CALL                     0
-                          1194 STORE_FAST              17 (tokens_to_be_excluded)
-               
-               135     >> 1196 LOAD_FAST                2 (post_filter)
-               
-               134        1198 POP_JUMP_FORWARD_IF_FALSE    27 (to 1254)
-                          1200 LOAD_FAST                0 (self)
-                          1202 LOAD_METHOD             34 (final_cleanup)
-                          1224 LOAD_FAST                0 (self)
-                          1226 LOAD_ATTR                5 (tokens)
-                          1236 LOAD_FAST               17 (tokens_to_be_excluded)
-                          1238 PRECALL                  2
-                          1242 CALL                     2
-                          1252 JUMP_FORWARD            19 (to 1292)
-               
-               136     >> 1254 LOAD_GLOBAL             31 (NULL + list)
-                          1266 LOAD_FAST                0 (self)
-                          1268 LOAD_ATTR                5 (tokens)
-                          1278 PRECALL                  1
-                          1282 CALL                     1
-               
-               133     >> 1292 RETURN_VALUE
+                           722 LOAD_FAST               11 (start)
+                           724 LOAD_CONST               4 (1)
+                           726 BINARY_OP               10 (-)
+                           730 LOAD_FAST               12 (end)
+                           732 LOAD_CONST               4 (1)
+                           734 BINARY_OP                0 (+)
+                           738 BUILD_LIST               2
+                           740 KW_NAMES                 5
+                           742 PRECALL                  2
+                           746 CALL                     2
+                           756 STORE_FAST              13 (span)
+               
+               115         758 LOAD_GLOBAL             45 (NULL + Token)
+                           770 LOAD_FAST                1 (file)
+                           772 LOAD_FAST                9 (content)
+                           774 LOAD_FAST               13 (span)
+                           776 KW_NAMES                 6
+                           778 PRECALL                  3
+                           782 CALL                     3
+                           792 STORE_FAST              14 (token)
+               
+               116         794 LOAD_FAST               14 (token)
+                           796 LOAD_METHOD             23 (set_type)
+                           818 LOAD_FAST               10 (types)
+                           820 PRECALL                  1
+                           824 CALL                     1
+                           834 POP_TOP
+               
+               118         836 LOAD_FAST                5 (token_improver)
+                           838 LOAD_METHOD             24 (improve_token)
+                           860 LOAD_FAST                0 (self)
+                           862 LOAD_ATTR                3 (tokens)
+                           872 LOAD_FAST                0 (self)
+                           874 LOAD_ATTR                0 (token_stream)
+                           884 LOAD_FAST               14 (token)
+                           886 PRECALL                  3
+                           890 CALL                     3
+                           900 STORE_FAST              15 (improved_tokens)
+               
+               120         902 LOAD_FAST                0 (self)
+                           904 LOAD_ATTR                3 (tokens)
+                           914 LOAD_METHOD             25 (extend)
+                           936 LOAD_FAST               15 (improved_tokens)
+                           938 PRECALL                  1
+                           942 CALL                     1
+                           952 POP_TOP
+               
+               121         954 LOAD_FAST                0 (self)
+                           956 LOAD_METHOD             26 (add_to_token_stream)
+                           978 LOAD_FAST               15 (improved_tokens)
+                           980 PRECALL                  1
+                           984 CALL                     1
+                           994 POP_TOP
+                           996 JUMP_BACKWARD          239 (to 520)
+                       >>  998 PUSH_EXC_INFO
+               
+               122        1000 LOAD_GLOBAL             54 (Exception)
+                          1012 CHECK_EXC_MATCH
+                          1014 POP_JUMP_FORWARD_IF_FALSE    26 (to 1068)
+                          1016 STORE_FAST              16 (e)
+               
+               123        1018 LOAD_GLOBAL             57 (NULL + str)
+                          1030 LOAD_FAST               16 (e)
+                          1032 PRECALL                  1
+                          1036 CALL                     1
+                          1046 POP_TOP
+                          1048 POP_EXCEPT
+                          1050 LOAD_CONST               0 (None)
+                          1052 STORE_FAST              16 (e)
+                          1054 DELETE_FAST             16 (e)
+                          1056 EXTENDED_ARG             1
+                          1058 JUMP_BACKWARD          270 (to 520)
+                       >> 1060 LOAD_CONST               0 (None)
+                          1062 STORE_FAST              16 (e)
+                          1064 DELETE_FAST             16 (e)
+                          1066 RERAISE                  1
+               
+               122     >> 1068 RERAISE                  0
+                       >> 1070 COPY                     3
+                          1072 POP_EXCEPT
+                          1074 RERAISE                  1
+               
+               125     >> 1076 BUILD_LIST               0
+                          1078 STORE_FAST              17 (tokens_to_be_excluded)
+               
+               126        1080 LOAD_FAST                0 (self)
+                          1082 LOAD_ATTR               29 (settings)
+                          1092 LOAD_ATTR               30 (deep_token_inspection)
+                          1102 LOAD_CONST               7 (True)
+                          1104 IS_OP                    0
+                          1106 POP_JUMP_FORWARD_IF_FALSE    20 (to 1148)
+               
+               127        1108 LOAD_FAST                0 (self)
+                          1110 LOAD_METHOD             31 (deep_analyze)
+                          1132 PRECALL                  0
+                          1136 CALL                     0
+                          1146 STORE_FAST              17 (tokens_to_be_excluded)
+               
+               129     >> 1148 LOAD_FAST                2 (post_filter)
+                          1150 POP_JUMP_FORWARD_IF_FALSE    27 (to 1206)
+                          1152 LOAD_FAST                0 (self)
+                          1154 LOAD_METHOD             32 (final_cleanup)
+                          1176 LOAD_FAST                0 (self)
+                          1178 LOAD_ATTR                3 (tokens)
+                          1188 LOAD_FAST               17 (tokens_to_be_excluded)
+                          1190 PRECALL                  2
+                          1194 CALL                     2
+                          1204 JUMP_FORWARD            19 (to 1244)
+                       >> 1206 LOAD_GLOBAL             27 (NULL + list)
+                          1218 LOAD_FAST                0 (self)
+                          1220 LOAD_ATTR                3 (tokens)
+                          1230 PRECALL                  1
+                          1234 CALL                     1
+                       >> 1244 RETURN_VALUE
                ExceptionTable:
-                 18 to 66 -> 70 [0]
-                 70 to 102 -> 110 [1] lasti
-                 108 to 108 -> 110 [1] lasti
-                 146 to 226 -> 230 [0]
-                 230 to 308 -> 316 [1] lasti
-                 314 to 314 -> 316 [1] lasti
-                 696 to 740 -> 1046 [1]
-                 744 to 1042 -> 1046 [1]
-                 1046 to 1064 -> 1118 [2] lasti
-                 1066 to 1094 -> 1108 [2] lasti
-                 1108 to 1116 -> 1118 [2] lasti
+                 98 to 178 -> 182 [0]
+                 182 to 260 -> 268 [1] lasti
+                 266 to 266 -> 268 [1] lasti
+                 648 to 692 -> 998 [1]
+                 696 to 994 -> 998 [1]
+                 998 to 1016 -> 1070 [2] lasti
+                 1018 to 1046 -> 1060 [2] lasti
+                 1060 to 1068 -> 1070 [2] lasti
                consts
                   None
                   ''
                   0
                   ('lang',)
                   1
                   ('between',)
-                  ('file', 'cont', 'span')
+                  ('file', 'content', 'span')
                   True
-               names      ('token_stream', 'get_lexer_for_filename', 'path', 'lexer', 'ClassNotFound', 'tokens', 'Language', 'from_text', 'filenames', 'language', 'ValueError', 'extension', 'highlight', 'content', 'RawTokenFormatter', 'list', 'RawTokenLexer', 'get_tokens', 'SpotImprovements', 'enumerate', '_get_types_for_token', 'len', 'sanitize', 'get_span_for_string', 'Token', 'set_type', 'improve_token', 'extend', 'add_to_token_stream', 'Exception', 'str', 'settings', 'deep_token_inspection', 'deep_analyze', 'final_cleanup')
+               names      ('token_stream', '_find_lexer_for_file', 'lexer', 'tokens', 'Language', 'from_text', 'filenames', 'language', 'ValueError', 'extension', 'highlight', 'content', 'RawTokenFormatter', 'list', 'RawTokenLexer', 'get_tokens', 'SpotImprovements', 'enumerate', '_get_types_for_token', 'len', 'sanitize', 'get_span_for_string', 'Token', 'set_type', 'improve_token', 'extend', 'add_to_token_stream', 'Exception', 'str', 'settings', 'deep_token_inspection', 'deep_analyze', 'final_cleanup')
                varnames   ('self', 'file', 'post_filter', 'result', 'raw_tokens', 'token_improver', 'current_position', 'i', 'raw_token', 'content', 'types', 'start', 'end', 'span', 'token', 'improved_tokens', 'e', 'tokens_to_be_excluded')
                freevars   ()
                cellvars   ()
-               filename   '/app/deepsecrets/core/tokenizers/lexer/lexer.py'
+               filename   '/app/deepsecrets/core/tokenizers/lexer.py'
                name       'tokenize'
-               firstlineno 79
+               firstlineno 83
                lnotab
-                  0x02010e0202013601120112ff08030e010e0202015601120140ff08034e
-                  015c012a0204022a011001360104012401040202012a01040102033e010c
-                  010201020102fd12052a02420234012e01120132ff080304011c01280402
-                  ff380226fd
+                  0x02010e0334010e010e0202015601120140ff08034e015c012a0204022a
+                  011001360104012401040202012a01040102023e0124012a02420234012e
+                  01120132ff080304011c012802
             'tokens'
+            None
             code
                argcount  : 2
                nlocals   : 3
                stacksize : 6
                flags     : 3
                code
                   0x97007c0144005d207d027c0078016a0000000000000000007403000000
                   000000000000007c02ac01a6010000ab0100000000000000007a0d000063
                   025f0000000000000000008c2164005300
-               140           0 RESUME                   0
+               131           0 RESUME                   0
                
-               141           2 LOAD_FAST                1 (tokens)
+               132           2 LOAD_FAST                1 (tokens)
                              4 GET_ITER
                        >>    6 FOR_ITER                32 (to 72)
                              8 STORE_FAST               2 (token)
                
-               142          10 LOAD_FAST                0 (self)
+               133          10 LOAD_FAST                0 (self)
                             12 COPY                     1
                             14 LOAD_ATTR                0 (token_stream)
                             24 LOAD_GLOBAL              3 (NULL + token_to_typestream_item)
                             36 LOAD_FAST                2 (token)
                             38 KW_NAMES                 1
                             40 PRECALL                  1
                             44 CALL                     1
                             54 BINARY_OP               13 (+=)
                             58 SWAP                     2
                             60 STORE_ATTR               0 (token_stream)
                             70 JUMP_BACKWARD           33 (to 6)
                
-               141     >>   72 LOAD_CONST               0 (None)
+               132     >>   72 LOAD_CONST               0 (None)
                             74 RETURN_VALUE
                consts
                   None
                   ('token',)
                names      ('token_stream', 'token_to_typestream_item')
                varnames   ('self', 'tokens', 'token')
                freevars   ()
                cellvars   ()
-               filename   '/app/deepsecrets/core/tokenizers/lexer/lexer.py'
+               filename   '/app/deepsecrets/core/tokenizers/lexer.py'
                name       'add_to_token_stream'
-               firstlineno 140
+               firstlineno 131
                lnotab 0x020108013eff
             'tokens_all'
             'tokens_to_be_excluded'
             code
                argcount  : 3
                nlocals   : 4
                stacksize : 5
@@ -973,103 +1023,103 @@
                   01640284087408000000000000000000004400a6000000ab000000000000
                   000000a6010000ab01000000000000000072018c4489046a050000000000
                   000000740c00000000000000000000760072018c537c03a0070000000000
                   0000000000000000000000000000008904a6010000ab0100000000000000
                   0001008c697c035300
                              0 MAKE_CELL                4 (token)
                
-               145           2 RESUME                   0
+               135           2 RESUME                   0
                
-               146           4 LOAD_GLOBAL              1 (NULL + isinstance)
+               136           4 LOAD_GLOBAL              1 (NULL + isinstance)
                             16 LOAD_FAST                1 (tokens_all)
                             18 LOAD_GLOBAL              2 (OrderedSet)
                             30 PRECALL                  2
                             34 CALL                     2
                             44 POP_JUMP_FORWARD_IF_TRUE    15 (to 76)
                
-               147          46 LOAD_GLOBAL              3 (NULL + OrderedSet)
+               137          46 LOAD_GLOBAL              3 (NULL + OrderedSet)
                             58 LOAD_FAST                1 (tokens_all)
                             60 PRECALL                  1
                             64 CALL                     1
                             74 STORE_FAST               1 (tokens_all)
                
-               149     >>   76 LOAD_FAST                1 (tokens_all)
+               139     >>   76 LOAD_FAST                1 (tokens_all)
                             78 LOAD_FAST                2 (tokens_to_be_excluded)
                             80 BINARY_OP               10 (-)
                             84 STORE_FAST               1 (tokens_all)
                
-               150          86 BUILD_LIST               0
+               140          86 BUILD_LIST               0
                             88 STORE_FAST               3 (final)
                
-               151          90 LOAD_FAST                1 (tokens_all)
+               141          90 LOAD_FAST                1 (tokens_all)
                             92 GET_ITER
                        >>   94 FOR_ITER               104 (to 304)
                             96 STORE_DEREF              4 (token)
                
-               152          98 LOAD_GLOBAL              5 (NULL + any)
+               142          98 LOAD_GLOBAL              5 (NULL + any)
                            110 LOAD_CLOSURE             4 (token)
                            112 BUILD_TUPLE              1
-                           114 LOAD_CONST               1 (<code object <genexpr>, file "/app/deepsecrets/core/tokenizers/lexer/lexer.py", line 152>)
+                           114 LOAD_CONST               1 (<code object <genexpr>, file "/app/deepsecrets/core/tokenizers/lexer.py", line 142>)
                            116 MAKE_FUNCTION            8 (closure)
                            118 LOAD_GLOBAL              6 (types_to_filter_before)
                            130 GET_ITER
                            132 PRECALL                  0
                            136 CALL                     0
                            146 PRECALL                  1
                            150 CALL                     1
                            160 POP_JUMP_FORWARD_IF_FALSE     1 (to 164)
                
-               153         162 JUMP_BACKWARD           35 (to 94)
+               143         162 JUMP_BACKWARD           35 (to 94)
                
-               155     >>  164 LOAD_GLOBAL              5 (NULL + any)
+               145     >>  164 LOAD_GLOBAL              5 (NULL + any)
                            176 LOAD_CLOSURE             4 (token)
                            178 BUILD_TUPLE              1
-                           180 LOAD_CONST               2 (<code object <genexpr>, file "/app/deepsecrets/core/tokenizers/lexer/lexer.py", line 155>)
+                           180 LOAD_CONST               2 (<code object <genexpr>, file "/app/deepsecrets/core/tokenizers/lexer.py", line 145>)
                            182 MAKE_FUNCTION            8 (closure)
                            184 LOAD_GLOBAL              8 (types_to_filter_after)
                            196 GET_ITER
                            198 PRECALL                  0
                            202 CALL                     0
                            212 PRECALL                  1
                            216 CALL                     1
                            226 POP_JUMP_FORWARD_IF_FALSE     1 (to 230)
                
-               156         228 JUMP_BACKWARD           68 (to 94)
+               146         228 JUMP_BACKWARD           68 (to 94)
                
-               158     >>  230 LOAD_DEREF               4 (token)
+               148     >>  230 LOAD_DEREF               4 (token)
                            232 LOAD_ATTR                5 (content)
                            242 LOAD_GLOBAL             12 (empty_tokens)
                            254 CONTAINS_OP              0
                            256 POP_JUMP_FORWARD_IF_FALSE     1 (to 260)
                
-               159         258 JUMP_BACKWARD           83 (to 94)
+               149         258 JUMP_BACKWARD           83 (to 94)
                
-               161     >>  260 LOAD_FAST                3 (final)
+               151     >>  260 LOAD_FAST                3 (final)
                            262 LOAD_METHOD              7 (append)
                            284 LOAD_DEREF               4 (token)
                            286 PRECALL                  1
                            290 CALL                     1
                            300 POP_TOP
                            302 JUMP_BACKWARD          105 (to 94)
                
-               163     >>  304 LOAD_FAST                3 (final)
+               153     >>  304 LOAD_FAST                3 (final)
                            306 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 51
                      code
                         0x95014b00010097007c005d0d7d017c0189026a00000000000000000076
                         005600970101008c0e64005300
                                    0 COPY_FREE_VARS           1
                      
-                     152           2 RETURN_GENERATOR
+                     142           2 RETURN_GENERATOR
                                    4 POP_TOP
                                    6 RESUME                   0
                                    8 LOAD_FAST                0 (.0)
                              >>   10 FOR_ITER                13 (to 38)
                                   12 STORE_FAST               1 (type)
                                   14 LOAD_FAST                1 (type)
                                   16 LOAD_DEREF               2 (token)
@@ -1083,29 +1133,29 @@
                                   40 RETURN_VALUE
                      consts
                         None
                      names      ('type',)
                      varnames   ('.0', 'type')
                      freevars   ('token',)
                      cellvars   ()
-                     filename   '/app/deepsecrets/core/tokenizers/lexer/lexer.py'
+                     filename   '/app/deepsecrets/core/tokenizers/lexer.py'
                      name       '<genexpr>'
-                     firstlineno 152
+                     firstlineno 142
                      lnotab 0x
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 51
                      code
                         0x95014b00010097007c005d0d7d017c0189026a00000000000000000076
                         005600970101008c0e64005300
                                    0 COPY_FREE_VARS           1
                      
-                     155           2 RETURN_GENERATOR
+                     145           2 RETURN_GENERATOR
                                    4 POP_TOP
                                    6 RESUME                   0
                                    8 LOAD_FAST                0 (.0)
                              >>   10 FOR_ITER                13 (to 38)
                                   12 STORE_FAST               1 (type)
                                   14 LOAD_FAST                1 (type)
                                   16 LOAD_DEREF               2 (token)
@@ -1119,25 +1169,25 @@
                                   40 RETURN_VALUE
                      consts
                         None
                      names      ('type',)
                      varnames   ('.0', 'type')
                      freevars   ('token',)
                      cellvars   ()
-                     filename   '/app/deepsecrets/core/tokenizers/lexer/lexer.py'
+                     filename   '/app/deepsecrets/core/tokenizers/lexer.py'
                      name       '<genexpr>'
-                     firstlineno 155
+                     firstlineno 145
                      lnotab 0x
                names      ('isinstance', 'OrderedSet', 'any', 'types_to_filter_before', 'types_to_filter_after', 'content', 'empty_tokens', 'append')
                varnames   ('self', 'tokens_all', 'tokens_to_be_excluded', 'final')
                freevars   ()
                cellvars   ('token',)
-               filename   '/app/deepsecrets/core/tokenizers/lexer/lexer.py'
+               filename   '/app/deepsecrets/core/tokenizers/lexer.py'
                name       'final_cleanup'
-               firstlineno 145
+               firstlineno 135
                lnotab 0x04012a011e020a010401080140010202400102021c0102022c02
             code
                argcount  : 1
                nlocals   : 7
                stacksize : 7
                flags     : 3
                code
@@ -1152,112 +1202,112 @@
                   00ab01000000000000000001008c367c0344005d567d0674130000000000
                   00000000007414000000000000000000006a0b00000000000000007c066a
                   0c00000000000000006a0d00000000000000007c066a0e00000000000000
                   006a0f0000000000000000ac01a6030000ab0300000000000000007c066a
                   1000000000000000005f1100000000000000007c02a01200000000000000
                   000000000000000000000000007c066a0c0000000000000000a6010000ab
                   01000000000000000001008c577c025300
-               165           0 RESUME                   0
+               155           0 RESUME                   0
                
-               166           2 LOAD_GLOBAL              1 (NULL + OrderedSet)
+               156           2 LOAD_GLOBAL              1 (NULL + OrderedSet)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (tokens)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 STORE_FAST               1 (tokens_all)
                
-               167          42 LOAD_FAST                0 (self)
+               157          42 LOAD_FAST                0 (self)
                             44 LOAD_ATTR                2 (language)
                             54 POP_JUMP_FORWARD_IF_NOT_NONE     2 (to 60)
                
-               168          56 LOAD_FAST                1 (tokens_all)
+               158          56 LOAD_FAST                1 (tokens_all)
                             58 RETURN_VALUE
                
-               170     >>   60 LOAD_GLOBAL              7 (NULL + set)
+               160     >>   60 LOAD_GLOBAL              7 (NULL + set)
                             72 PRECALL                  0
                             76 CALL                     0
                             86 STORE_FAST               2 (exclude_after)
                
-               172          88 BUILD_LIST               0
+               162          88 BUILD_LIST               0
                             90 STORE_FAST               3 (true_detections)
                
-               173          92 LOAD_GLOBAL              9 (NULL + VariableDetectionRules)
+               163          92 LOAD_GLOBAL              9 (NULL + VariableDetectionRules)
                            104 LOAD_ATTR                5 (for_language)
                            114 LOAD_FAST                0 (self)
                            116 LOAD_ATTR                2 (language)
                            126 PRECALL                  1
                            130 CALL                     1
                            140 STORE_FAST               4 (rules)
                
-               174         142 LOAD_FAST                4 (rules)
+               164         142 LOAD_FAST                4 (rules)
                            144 GET_ITER
                        >>  146 FOR_ITER                53 (to 254)
                            148 STORE_FAST               5 (rule)
                
-               175         150 LOAD_FAST                3 (true_detections)
+               165         150 LOAD_FAST                3 (true_detections)
                            152 LOAD_METHOD              6 (extend)
                            174 LOAD_FAST                5 (rule)
                            176 LOAD_METHOD              7 (match)
                            198 LOAD_FAST                0 (self)
                            200 LOAD_ATTR                1 (tokens)
                            210 LOAD_FAST                0 (self)
                            212 LOAD_ATTR                8 (token_stream)
                            222 PRECALL                  2
                            226 CALL                     2
                            236 PRECALL                  1
                            240 CALL                     1
                            250 POP_TOP
                            252 JUMP_BACKWARD           54 (to 146)
                
-               177     >>  254 LOAD_FAST                3 (true_detections)
+               167     >>  254 LOAD_FAST                3 (true_detections)
                            256 GET_ITER
                        >>  258 FOR_ITER                86 (to 432)
                            260 STORE_FAST               6 (var)
                
-               178         262 LOAD_GLOBAL             19 (NULL + Semantic)
+               168         262 LOAD_GLOBAL             19 (NULL + Semantic)
                
-               179         274 LOAD_GLOBAL             20 (SemanticType)
+               169         274 LOAD_GLOBAL             20 (SemanticType)
                            286 LOAD_ATTR               11 (VAR)
                
-               180         296 LOAD_FAST                6 (var)
+               170         296 LOAD_FAST                6 (var)
                            298 LOAD_ATTR               12 (name)
                            308 LOAD_ATTR               13 (content)
                
-               181         318 LOAD_FAST                6 (var)
+               171         318 LOAD_FAST                6 (var)
                            320 LOAD_ATTR               14 (found_by)
                            330 LOAD_ATTR               15 (creds_probability)
                
-               178         340 KW_NAMES                 1
+               168         340 KW_NAMES                 1
                            342 PRECALL                  3
                            346 CALL                     3
                            356 LOAD_FAST                6 (var)
                            358 LOAD_ATTR               16 (value)
                            368 STORE_ATTR              17 (semantic)
                
-               183         378 LOAD_FAST                2 (exclude_after)
+               173         378 LOAD_FAST                2 (exclude_after)
                            380 LOAD_METHOD             18 (add)
                            402 LOAD_FAST                6 (var)
                            404 LOAD_ATTR               12 (name)
                            414 PRECALL                  1
                            418 CALL                     1
                            428 POP_TOP
                            430 JUMP_BACKWARD           87 (to 258)
                
-               185     >>  432 LOAD_FAST                2 (exclude_after)
+               175     >>  432 LOAD_FAST                2 (exclude_after)
                            434 RETURN_VALUE
                consts
                   None
                   ('type', 'name', 'creds_probability')
                names      ('OrderedSet', 'tokens', 'language', 'set', 'VariableDetectionRules', 'for_language', 'extend', 'match', 'token_stream', 'Semantic', 'SemanticType', 'VAR', 'name', 'content', 'found_by', 'creds_probability', 'value', 'semantic', 'add')
                varnames   ('self', 'tokens_all', 'exclude_after', 'true_detections', 'rules', 'rule', 'var')
                freevars   ()
                cellvars   ()
-               filename   '/app/deepsecrets/core/tokenizers/lexer/lexer.py'
+               filename   '/app/deepsecrets/core/tokenizers/lexer.py'
                name       'deep_analyze'
-               firstlineno 165
+               firstlineno 155
                lnotab
                   0x020128010e0104021c02040132010801680208010c011601160116fd26
                   053602
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
@@ -1266,117 +1316,117 @@
                   0x970067007d017401000000000000000000007c006a0100000000000000
                   00a6010000ab01000000000000000064016b02000000007202670053007c
                   006a01000000000000000044005d3a7d027c026a02000000000000000080
                   018c0a7c026a0200000000000000006a0300000000000000007408000000
                   000000000000006a0500000000000000006b030000000072018c257c01a0
                   0600000000000000000000000000000000000000007c02a6010000ab0100
                   0000000000000001008c3b7c015300
-               187           0 RESUME                   0
+               177           0 RESUME                   0
                
-               188           2 BUILD_LIST               0
+               178           2 BUILD_LIST               0
                              4 STORE_FAST               1 (vars)
                
-               189           6 LOAD_GLOBAL              1 (NULL + len)
+               179           6 LOAD_GLOBAL              1 (NULL + len)
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (tokens)
                             30 PRECALL                  1
                             34 CALL                     1
                             44 LOAD_CONST               1 (0)
                             46 COMPARE_OP               2 (==)
                             52 POP_JUMP_FORWARD_IF_FALSE     2 (to 58)
                
-               190          54 BUILD_LIST               0
+               180          54 BUILD_LIST               0
                             56 RETURN_VALUE
                
-               192     >>   58 LOAD_FAST                0 (self)
+               182     >>   58 LOAD_FAST                0 (self)
                             60 LOAD_ATTR                1 (tokens)
                             70 GET_ITER
                        >>   72 FOR_ITER                58 (to 190)
                             74 STORE_FAST               2 (token)
                
-               193          76 LOAD_FAST                2 (token)
+               183          76 LOAD_FAST                2 (token)
                             78 LOAD_ATTR                2 (semantic)
                             88 POP_JUMP_FORWARD_IF_NOT_NONE     1 (to 92)
                
-               194          90 JUMP_BACKWARD           10 (to 72)
+               184          90 JUMP_BACKWARD           10 (to 72)
                
-               196     >>   92 LOAD_FAST                2 (token)
+               186     >>   92 LOAD_FAST                2 (token)
                             94 LOAD_ATTR                2 (semantic)
                            104 LOAD_ATTR                3 (type)
                            114 LOAD_GLOBAL              8 (SemanticType)
                            126 LOAD_ATTR                5 (VAR)
                            136 COMPARE_OP               3 (!=)
                            142 POP_JUMP_FORWARD_IF_FALSE     1 (to 146)
                
-               197         144 JUMP_BACKWARD           37 (to 72)
+               187         144 JUMP_BACKWARD           37 (to 72)
                
-               199     >>  146 LOAD_FAST                1 (vars)
+               189     >>  146 LOAD_FAST                1 (vars)
                            148 LOAD_METHOD              6 (append)
                            170 LOAD_FAST                2 (token)
                            172 PRECALL                  1
                            176 CALL                     1
                            186 POP_TOP
                            188 JUMP_BACKWARD           59 (to 72)
                
-               201     >>  190 LOAD_FAST                1 (vars)
+               191     >>  190 LOAD_FAST                1 (vars)
                            192 RETURN_VALUE
                consts
                   None
                   0
                names      ('len', 'tokens', 'semantic', 'type', 'SemanticType', 'VAR', 'append')
                varnames   ('self', 'vars', 'token')
                freevars   ()
                cellvars   ()
-               filename   '/app/deepsecrets/core/tokenizers/lexer/lexer.py'
+               filename   '/app/deepsecrets/core/tokenizers/lexer.py'
                name       'get_variables'
-               firstlineno 187
+               firstlineno 177
                lnotab 0x020104013001040212010e010202340102022c02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab010000000000000000010064005300
-               203           0 RESUME                   0
+               193           0 RESUME                   0
                
-               204           2 LOAD_GLOBAL              1 (NULL + print)
+               194           2 LOAD_GLOBAL              1 (NULL + print)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (token_stream)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('print', 'token_stream')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/app/deepsecrets/core/tokenizers/lexer/lexer.py'
+               filename   '/app/deepsecrets/core/tokenizers/lexer.py'
                name       'print_token_type_stream'
-               firstlineno 203
+               firstlineno 193
                lnotab 0x0201
-            None
             (True,)
-         names      ('__name__', '__module__', '__qualname__', 'str', '__annotations__', 'Lexer', 'Language', 'PygmentsToken', 'List', 'Type', '_get_types_for_token', 'sanitize', 'get_token_for_string', 'File', 'tokenize', 'Token', 'add_to_token_stream', 'Sequence', 'final_cleanup', 'deep_analyze', 'get_variables', 'print_token_type_stream')
+            ('return', None)
+         names      ('__name__', '__module__', '__qualname__', 'str', '__annotations__', 'Lexer', 'Language', 'PygmentsToken', 'List', 'Type', '_get_types_for_token', 'Union', 'bool', 'sanitize', 'File', '_find_lexer_for_file', 'Token', 'tokenize', 'add_to_token_stream', 'Sequence', 'final_cleanup', 'Set', 'deep_analyze', 'get_variables', 'print_token_type_stream')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/app/deepsecrets/core/tokenizers/lexer/lexer.py'
+         filename   '/app/deepsecrets/core/tokenizers/lexer.py'
          name       'LexerTokenizer'
-         firstlineno 35
-         lnotab 0x0c020a010a010a021c0a0c160c060e3d1805281406160610
+         firstlineno 27
+         lnotab 0x0c010a010a010a021c0a20150c141e301c04381418161810
       'LexerTokenizer'
       None
-   names      ('typing', 'List', 'Sequence', 'Type', 'ordered_set', 'OrderedSet', 'pygments', 'highlight', 'pygments.formatters', 'RawTokenFormatter', 'pygments.lexers', 'get_lexer_for_filename', 'pygments.lexers.special', 'Lexer', 'RawTokenLexer', 'pygments.token', 'Token', 'PygmentsToken', 'pygments.util', 'ClassNotFound', 'deepsecrets.core.model.semantic', 'Variable', 'deepsecrets.core.tokenizers.itokenizer', 'Tokenizer', 'deepsecrets.core.tokenizers.lexer.semantic.language', 'Language', 'deepsecrets.core.tokenizers.lexer.semantic.var_detection.rules', 'VariableDetectionRules', 'deepsecrets.core.model.file', 'File', 'deepsecrets.core.model.token', 'Semantic', 'SemanticType', 'deepsecrets.core.tokenizers.lexer.spot_improvements', 'SpotImprovements', 'deepsecrets.core.tokenizers.lexer.type_stream', 'token_to_typestream_item', 'types_to_filter_before', 'types_to_filter_after', 'deepsecrets.core.utils.exceptions', 'TokenizationException', 'empty_tokens', 'LexerTokenizer')
+   names      ('typing', 'List', 'Sequence', 'Set', 'Type', 'Union', 'ordered_set', 'OrderedSet', 'pygments', 'highlight', 'pygments.formatters', 'RawTokenFormatter', 'pygments.lexers', 'get_lexer_for_filename', 'pygments.lexers.special', 'Lexer', 'RawTokenLexer', 'pygments.token', 'Token', 'PygmentsToken', 'pygments.util', 'ClassNotFound', 'deepsecrets.core.model.file', 'File', 'deepsecrets.core.model.semantic', 'Variable', 'deepsecrets.core.model.token', 'Semantic', 'SemanticType', 'deepsecrets.core.tokenizers.helpers.semantic.language', 'Language', 'deepsecrets.core.tokenizers.helpers.semantic.var_detection.rules', 'VariableDetectionRules', 'deepsecrets.core.tokenizers.helpers.spot_improvements', 'SpotImprovements', 'deepsecrets.core.tokenizers.helpers.type_stream', 'token_to_typestream_item', 'types_to_filter_after', 'types_to_filter_before', 'deepsecrets.core.tokenizers.itokenizer', 'Tokenizer', 'empty_tokens', 'LexerTokenizer')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/app/deepsecrets/core/tokenizers/lexer/lexer.py'
+   filename   '/app/deepsecrets/core/tokenizers/lexer.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020114060c010c010c010c0110010c010c010c020c010c010c010c
-      0114050c0114030c040802
+      0x00ff02011c020c010c010c010c0110010c010c020c010c0114010c010c
+      010c0114050c020803
```

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/__pycache__/lexer.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/__pycache__/spot_improvements.cpython-311.pyc`

 * *Files 9% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x224c3964 (Fri Apr 14 12:50:42 2023 UTC)
-files sz: 2027
+moddate:  0x29c29964 (Mon Jun 26 16:51:53 2023 UTC)
+files sz: 2115
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x9700640064016c005a01640064026c026d035a036d045a040100640064
@@ -289,23 +289,25 @@
                   000000000000000000000000000000a6000000ab00000000000000000044
                   005d475c0200007d077d087c06a005000000000000000000000000000000
                   00000000007c07a6010000ab0100000000000000007d097c017c09640719
                   000000000000000000190000000000000000007d0a7c08a0030000000000
                   0000000000000000000000000000007c0a6a060000000000000000a60100
                   00ab01000000000000000073057c0367016302010053008c487c036a0600
                   00000000000000a007000000000000000000000000000000000000000064
-                  08a6010000ab0100000000000000007d0b67007d0c7c0b44005d6d7d0d74
-                  11000000000000000000007c036a0900000000000000007c0d7c036a0900
-                  00000000000000a00a00000000000000000000000000000000000000007c
-                  0d7c036a050000000000000000ac09a6020000ab020000000000000000ac
-                  0aa6030000ab0300000000000000007d0e7c0ea00b000000000000000000
-                  00000000000000000000007418000000000000000000006a0d0000000000
-                  0000006701a6010000ab01000000000000000001007c0ca00e0000000000
-                  0000000000000000000000000000007c0ea6010000ab0100000000000000
-                  0001008c6e7c0c5300
+                  08a6010000ab0100000000000000007d0b7c0b6407190000000000000000
+                  0064096b0200000000730c7c0b64021900000000000000000064096b0200
+                  00000072037c036701530067007d0c7c0b44005d6d7d0d74110000000000
+                  00000000007c036a0900000000000000007c0d7c036a0900000000000000
+                  00a00a00000000000000000000000000000000000000007c0d7c036a0500
+                  00000000000000ac0aa6020000ab020000000000000000ac0ba6030000ab
+                  0300000000000000007d0e7c0ea00b000000000000000000000000000000
+                  00000000007418000000000000000000006a0d00000000000000006701a6
+                  010000ab01000000000000000001007c0ca00e0000000000000000000000
+                  0000000000000000007c0ea6010000ab01000000000000000001008c6e7c
+                  0c5300
                 29           0 RESUME                   0
                
                 32           2 LOAD_FAST                2 (so_far_type_stream)
                              4 LOAD_GLOBAL              1 (NULL + token_to_typestream_item)
                             16 LOAD_FAST                3 (current_token)
                             18 PRECALL                  1
                             22 CALL                     1
@@ -390,85 +392,103 @@
                            386 LOAD_ATTR                6 (content)
                            396 LOAD_METHOD              7 (split)
                            418 LOAD_CONST               8 (':')
                            420 PRECALL                  1
                            424 CALL                     1
                            434 STORE_FAST              11 (new_parts)
                
-                46         436 BUILD_LIST               0
-                           438 STORE_FAST              12 (final)
+                45         436 LOAD_FAST               11 (new_parts)
+                           438 LOAD_CONST               7 (0)
+                           440 BINARY_SUBSCR
+                           450 LOAD_CONST               9 ('')
+                           452 COMPARE_OP               2 (==)
+                           458 POP_JUMP_FORWARD_IF_TRUE    12 (to 484)
+                           460 LOAD_FAST               11 (new_parts)
+                           462 LOAD_CONST               2 (1)
+                           464 BINARY_SUBSCR
+                           474 LOAD_CONST               9 ('')
+                           476 COMPARE_OP               2 (==)
+                           482 POP_JUMP_FORWARD_IF_FALSE     3 (to 490)
+               
+                46     >>  484 LOAD_FAST                3 (current_token)
+                           486 BUILD_LIST               1
+                           488 RETURN_VALUE
+               
+                48     >>  490 BUILD_LIST               0
+                           492 STORE_FAST              12 (final)
+               
+                49         494 LOAD_FAST               11 (new_parts)
+                           496 GET_ITER
+                       >>  498 FOR_ITER               109 (to 718)
+                           500 STORE_FAST              13 (part)
+               
+                50         502 LOAD_GLOBAL             17 (NULL + Token)
+               
+                51         514 LOAD_FAST                3 (current_token)
+                           516 LOAD_ATTR                9 (file)
+               
+                52         526 LOAD_FAST               13 (part)
+               
+                53         528 LOAD_FAST                3 (current_token)
+                           530 LOAD_ATTR                9 (file)
+                           540 LOAD_METHOD             10 (get_span_for_string)
+                           562 LOAD_FAST               13 (part)
+                           564 LOAD_FAST                3 (current_token)
+                           566 LOAD_ATTR                5 (span)
+                           576 KW_NAMES                10
+                           578 PRECALL                  2
+                           582 CALL                     2
+               
+                50         592 KW_NAMES                11
+                           594 PRECALL                  3
+                           598 CALL                     3
+                           608 STORE_FAST              14 (t)
+               
+                55         610 LOAD_FAST               14 (t)
+                           612 LOAD_METHOD             11 (set_type)
+                           634 LOAD_GLOBAL             24 (PygmentsToken)
+                           646 LOAD_ATTR               13 (Text)
+                           656 BUILD_LIST               1
+                           658 PRECALL                  1
+                           662 CALL                     1
+                           672 POP_TOP
+               
+                56         674 LOAD_FAST               12 (final)
+                           676 LOAD_METHOD             14 (append)
+                           698 LOAD_FAST               14 (t)
+                           700 PRECALL                  1
+                           704 CALL                     1
+                           714 POP_TOP
+                           716 JUMP_BACKWARD          110 (to 498)
                
-                47         440 LOAD_FAST               11 (new_parts)
-                           442 GET_ITER
-                       >>  444 FOR_ITER               109 (to 664)
-                           446 STORE_FAST              13 (part)
-               
-                48         448 LOAD_GLOBAL             17 (NULL + Token)
-               
-                49         460 LOAD_FAST                3 (current_token)
-                           462 LOAD_ATTR                9 (file)
-               
-                50         472 LOAD_FAST               13 (part)
-               
-                51         474 LOAD_FAST                3 (current_token)
-                           476 LOAD_ATTR                9 (file)
-                           486 LOAD_METHOD             10 (get_span_for_string)
-                           508 LOAD_FAST               13 (part)
-                           510 LOAD_FAST                3 (current_token)
-                           512 LOAD_ATTR                5 (span)
-                           522 KW_NAMES                 9
-                           524 PRECALL                  2
-                           528 CALL                     2
-               
-                48         538 KW_NAMES                10
-                           540 PRECALL                  3
-                           544 CALL                     3
-                           554 STORE_FAST              14 (t)
-               
-                53         556 LOAD_FAST               14 (t)
-                           558 LOAD_METHOD             11 (set_type)
-                           580 LOAD_GLOBAL             24 (PygmentsToken)
-                           592 LOAD_ATTR               13 (Text)
-                           602 BUILD_LIST               1
-                           604 PRECALL                  1
-                           608 CALL                     1
-                           618 POP_TOP
-               
-                54         620 LOAD_FAST               12 (final)
-                           622 LOAD_METHOD             14 (append)
-                           644 LOAD_FAST               14 (t)
-                           646 PRECALL                  1
-                           650 CALL                     1
-                           660 POP_TOP
-                           662 JUMP_BACKWARD          110 (to 444)
-               
-                56     >>  664 LOAD_FAST               12 (final)
-                           666 RETURN_VALUE
+                58     >>  718 LOAD_FAST               12 (final)
+                           720 RETURN_VALUE
                consts
                   None
                   '(L)(L)$'
                   1
                   '^-u$'
                   ('pattern', 'checks')
                   'pattern'
                   'checks'
                   0
                   ':'
+                  ''
                   ('between',)
                   ('file', 'content', 'span')
                names      ('token_to_typestream_item', 're', 'compile', 'search', 'items', 'span', 'content', 'split', 'Token', 'file', 'get_span_for_string', 'set_type', 'PygmentsToken', 'Text', 'append')
                varnames   ('self', 'so_far_tokens', 'so_far_type_stream', 'current_token', 'projected_typestream', 'rule', 'match', 'group_i', 'pattern', 'span', 'group_token', 'new_parts', 'final', 'part', 't')
                freevars   ()
                cellvars   ()
                filename   '/app/deepsecrets/core/tokenizers/helpers/spot_improvements.py'
                name       '_curl_argstring_breakdown'
                firstlineno 29
                lnotab
-                  0x0203240156013601040106023e012a011c0134010aff02033402040108
-                  010c010c01020140fd120540012c02
+                  0x0203240156013601040106023e012a011c0134010aff02033401300106
+                  02040108010c010c01020140fd120540012c02
          names      ('__name__', '__module__', '__qualname__', 'Language', '__annotations__', 'dict', 'List', 'Callable', '__init__', 'Token', 'str', 'improve_token', '_curl_argstring_breakdown')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/app/deepsecrets/core/tokenizers/helpers/spot_improvements.py'
          name       'SpotImprovements'
          firstlineno 11
```

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/__pycache__/type_stream.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/language.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/python.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/__pycache__/variable_detection.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/language.py` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/language.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/detector.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/var_detection/__pycache__/rules.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/var_detection/detector.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/semantic/var_detection/rules.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/spot_improvements.py` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/spot_improvements.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,14 +38,16 @@
         for group_i, pattern in rule['checks'].items():
             span = match.span(group_i)
             group_token: Token = so_far_tokens[span[0]]
             if not pattern.search(group_token.content):
                 return [current_token]
 
         new_parts = current_token.content.split(':')
+        if new_parts[0] == '' or new_parts[1] == '':
+            return [current_token]
 
         final = []
         for part in new_parts:
             t = Token(
                 file=current_token.file,
                 content=part,
                 span=current_token.file.get_span_for_string(part, between=current_token.span),
```

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/helpers/type_stream.py` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/helpers/type_stream.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/itokenizer.py` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/itokenizer.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/lexer.py` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/lexer.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,22 +56,39 @@
                 content = content[1:-1]
 
         if content in quotes:
             return False
 
         return content
 
+    def _find_lexer_for_file(self, file: File):
+        lexer = None
+        if file.extension is not None:
+            try:
+                lexer = get_lexer_for_filename(file.path)
+                return lexer
+            except ClassNotFound:
+                pass
+        
+        if file.guessed_extension is not None:
+            try:
+                lexer = get_lexer_for_filename(f'{file.path}.{file.guessed_extension}')
+                return lexer
+            except ClassNotFound:
+                pass
+        
+        return lexer
+
+
+
     def tokenize(self, file: File, post_filter=True) -> List[Token]:
         self.token_stream = ''
         # TODO: don't trust the extension, use 'file' utility ?
-        try:
-            self.lexer = get_lexer_for_filename(file.path)
-        except ClassNotFound:
-            self.lexer = None
 
+        self.lexer = self._find_lexer_for_file(file)
         if not self.lexer:
             return self.tokens
 
         try:
             self.language: Language = Language.from_text(self.lexer.filenames[0])
         except ValueError:
             self.language: Language = Language.from_text(file.extension)
```

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/per_line.py` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/per_line.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/tokenizers/per_word.py` & `deepsecrets-1.0.5/deepsecrets/core/tokenizers/per_word.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/utils/.DS_Store` & `deepsecrets-1.0.5/deepsecrets/core/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/utils/__pycache__/exceptions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/utils/__pycache__/file_analyzer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/utils/__pycache__/fs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/core/utils/__pycache__/hashing.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/utils/file_analyzer.py` & `deepsecrets-1.0.5/deepsecrets/core/utils/file_analyzer.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/utils/fs.py` & `deepsecrets-1.0.5/deepsecrets/core/utils/fs.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/core/utils/hashing.py` & `deepsecrets-1.0.5/deepsecrets/core/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/rules/excluded_paths.json` & `deepsecrets-1.0.5/deepsecrets/rules/excluded_paths.json`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/rules/regexes.json` & `deepsecrets-1.0.5/deepsecrets/rules/regexes.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965986394557822%*

 * *Differences: {'18': "{'pattern': '\\\\b(pass|password|pwd|passwd)\\\\b(\\\\W+)([A-Za-z0-9()$]*)\\\\b'}"}*

```diff
@@ -122,15 +122,15 @@
         "id": "S28",
         "match_rules": {
             "2": {
                 "pattern": "^\\s*(?:'|:|=)*\\s*$"
             }
         },
         "name": "Suspicious password declaration",
-        "pattern": "\\b(pass|password|pwd|passwd)\\b(\\W+)([A-Za-z0-9]*)\\b",
+        "pattern": "\\b(pass|password|pwd|passwd)\\b(\\W+)([A-Za-z0-9()$]*)\\b",
         "target_group": 3
     },
     {
         "confidence": 9,
         "id": "S29",
         "name": "Ansible vault",
         "pattern": "\\$ANSIBLE_VAULT;[0-9]\\.[0-9];AES256"
```

### Comparing `deepsecrets-1.0.4/deepsecrets/scan_modes/.DS_Store` & `deepsecrets-1.0.5/deepsecrets/scan_modes/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc` & `deepsecrets-1.0.5/deepsecrets/scan_modes/__pycache__/cli.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/deepsecrets/scan_modes/cli.py` & `deepsecrets-1.0.5/deepsecrets/scan_modes/cli.py`

 * *Files identical despite different names*

### Comparing `deepsecrets-1.0.4/pyproject.toml` & `deepsecrets-1.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deepsecrets"
-version = "1.0.4"
+version = "1.0.5"
 description = "A better tool for secrets search"
 license = "MIT"
 authors = [
   "Nikolai Khechumov <khechumov@gmail.com>",
 ]
 keywords = ["security", "secrets", "credentials", "scanning", "appsec"]
 packages = [{include = "deepsecrets"}]
@@ -32,15 +32,14 @@
 python = ">=3.9,<3.12"
 pydantic = "^1.10.4"
 pyyaml = "^5.4.1"
 pygments = "^2.14.0"
 ordered-set = "^4.1.0"
 dotwiz = "^0.4.0"
 mmh3 = "^3.0.0"
-argparse = "^1.4.0"
 regex = "^2023.3.23"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.1"
 coverage = "^7.2.0"
 pytest-cov = "^4.0.0"
```

### Comparing `deepsecrets-1.0.4/PKG-INFO` & `deepsecrets-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepsecrets
-Version: 1.0.4
+Version: 1.0.5
 Summary: A better tool for secrets search
 License: MIT
 Keywords: security,secrets,credentials,scanning,appsec
 Author: Nikolai Khechumov
 Author-email: khechumov@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Environment :: Console
@@ -12,15 +12,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
-Requires-Dist: argparse (>=1.4.0,<2.0.0)
 Requires-Dist: dotwiz (>=0.4.0,<0.5.0)
 Requires-Dist: mmh3 (>=3.0.0,<4.0.0)
 Requires-Dist: ordered-set (>=4.1.0,<5.0.0)
 Requires-Dist: pydantic (>=1.10.4,<2.0.0)
 Requires-Dist: pygments (>=2.14.0,<3.0.0)
 Requires-Dist: pyyaml (>=5.4.1,<6.0.0)
 Requires-Dist: regex (>=2023.3.23,<2024.0.0)
```


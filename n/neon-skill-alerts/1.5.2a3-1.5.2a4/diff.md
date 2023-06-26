# Comparing `tmp/neon-skill-alerts-1.5.2a3.tar.gz` & `tmp/neon-skill-alerts-1.5.2a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-alerts-1.5.2a3.tar", last modified: Tue Jun 20 23:07:59 2023, max compression
+gzip compressed data, was "neon-skill-alerts-1.5.2a4.tar", last modified: Mon Jun 26 17:10:04 2023, max compression
```

## Comparing `neon-skill-alerts-1.5.2a3.tar` & `neon-skill-alerts-1.5.2a4.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:07:59.863636 neon-skill-alerts-1.5.2a3/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-20 23:07:59.863636 neon-skill-alerts-1.5.2a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    62744 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:07:59.827636 neon-skill-alerts-1.5.2a3/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:07:59.827636 neon-skill-alerts-1.5.2a3/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:07:59.847636 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/confirm_alert_playback.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/confirm_alert_recurring.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/confirm_alert_recurring_playback.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/confirm_alert_recurring_script.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/confirm_alert_script.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/confirm_alert_set.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/confirm_cancel_alert.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/confirm_cancel_all.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/confirm_dismiss_alert.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/confirm_snooze_alert.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/confirm_timer_started.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/error_audio_reminder_too_far.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/error_no_duration.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/error_no_scheduled_kind_to_cancel.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/error_no_time.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/error_nothing_to_cancel.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/expired_alert.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/expired_audio_alert_intro.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/expired_reminder.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/list_alert.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/list_alert_intro.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/list_alert_missed_intro.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/list_alert_none_missed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/list_alert_none_upcoming.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/list_alert_repeating.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/next_alert_named.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/next_alert_unnamed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/quiet_hours_end.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/quiet_hours_start.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/timer_status.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/timer_status_none_active.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/word_alarm.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/word_alert.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/word_day.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/word_reminder.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/word_timer.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/word_weekday.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/word_weekday_friday.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/word_weekday_monday.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/word_weekday_saturday.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/word_weekday_sunday.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/word_weekday_thursday.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/word_weekday_tuesday.dialog
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/word_weekday_wednesday.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/dialog/word_weekend.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:07:59.847636 neon-skill-alerts-1.5.2a3/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/intent/list_alerts.intent
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/intent/quiet_hours_end.intent
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/intent/quiet_hours_start.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:07:59.851636 neon-skill-alerts-1.5.2a3/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/vocab/alarm.voc
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/vocab/alert.voc
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/vocab/all.voc
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/vocab/articles.voc
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/vocab/cancel.voc
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/vocab/dismiss.voc
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/vocab/event.voc
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/vocab/everyday.voc
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/vocab/next.voc
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/vocab/playable.voc
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/vocab/priority.voc
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/vocab/query.voc
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/vocab/remind_me.voc
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/vocab/reminder.voc
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/vocab/repeat.voc
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/vocab/script.voc
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/vocab/set.voc
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/vocab/snooze.voc
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/vocab/timer.voc
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/vocab/timer_time_remaining.voc
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/vocab/until.voc
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/vocab/weekdays.voc
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/locale/en-us/vocab/weekends.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:07:59.855636 neon-skill-alerts-1.5.2a3/neon_skill_alerts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-20 23:07:59.000000 neon-skill-alerts-1.5.2a3/neon_skill_alerts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-06-20 23:07:59.000000 neon-skill-alerts-1.5.2a3/neon_skill_alerts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 23:07:59.000000 neon-skill-alerts-1.5.2a3/neon_skill_alerts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-20 23:07:59.000000 neon-skill-alerts-1.5.2a3/neon_skill_alerts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-20 23:07:59.000000 neon-skill-alerts-1.5.2a3/neon_skill_alerts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 23:07:59.000000 neon-skill-alerts-1.5.2a3/neon_skill_alerts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 23:07:59.863636 neon-skill-alerts-1.5.2a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:07:59.855636 neon-skill-alerts-1.5.2a3/test/
--rw-r--r--   0 runner    (1001) docker     (123)   114134 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/test/test_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:07:59.855636 neon-skill-alerts-1.5.2a3/ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:07:59.859636 neon-skill-alerts-1.5.2a3/ui/+mediacenter/
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/+mediacenter/RoundProgress.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/+mediacenter/Timer.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/+mediacenter/TimerCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/AlarmBoxControl.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/AlarmBoxView.qml
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/AlarmButtonView.qml
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/AlarmCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/AlarmsOverviewCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/AlarmsOverviewDelegate.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/RoundProgress.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/Timer.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/TimerCard.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:07:59.859636 neon-skill-alerts-1.5.2a3/ui/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/icons/close.svg
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/icons/continue.svg
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/icons/pause.svg
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/qmldir
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:07:59.859636 neon-skill-alerts-1.5.2a3/ui/sounds/
--rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/sounds/clicked.wav
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:07:59.859636 neon-skill-alerts-1.5.2a3/ui/translations/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/translations/TimerCard_de.ts
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/translations/TimerCard_es.ts
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/translations/TimerCard_fr.ts
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/translations/TimerCard_it.ts
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/translations/TimerCard_nl.ts
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/translations/TimerCard_pt.ts
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/translations/skill-ovos-timer.openvoiceos_de.qm
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/translations/skill-ovos-timer.openvoiceos_es.qm
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/translations/skill-ovos-timer.openvoiceos_fr.qm
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/translations/skill-ovos-timer.openvoiceos_it.qm
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/translations/skill-ovos-timer.openvoiceos_nl.qm
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/ui/translations/skill-ovos-timer.openvoiceos_pt.qm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:07:59.863636 neon-skill-alerts-1.5.2a3/util/
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/util/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)    16625 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/util/alert_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    22330 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/util/parse_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/util/ui_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-20 23:07:54.000000 neon-skill-alerts-1.5.2a3/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:10:04.149191 neon-skill-alerts-1.5.2a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-26 17:10:04.149191 neon-skill-alerts-1.5.2a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    62733 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:10:04.133191 neon-skill-alerts-1.5.2a4/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:10:04.137191 neon-skill-alerts-1.5.2a4/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:10:04.141191 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/confirm_alert_playback.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/confirm_alert_recurring.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/confirm_alert_recurring_playback.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/confirm_alert_recurring_script.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/confirm_alert_script.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/confirm_alert_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/confirm_cancel_alert.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/confirm_cancel_all.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/confirm_dismiss_alert.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/confirm_snooze_alert.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/confirm_timer_started.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/error_audio_reminder_too_far.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/error_no_duration.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/error_no_scheduled_kind_to_cancel.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/error_no_time.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/error_nothing_to_cancel.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/expired_alert.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/expired_audio_alert_intro.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/expired_reminder.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/list_alert.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/list_alert_intro.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/list_alert_missed_intro.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/list_alert_none_missed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/list_alert_none_upcoming.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/list_alert_repeating.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/next_alert_named.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/next_alert_unnamed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/quiet_hours_end.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/quiet_hours_start.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/timer_status.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/timer_status_none_active.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/word_alarm.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/word_alert.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/word_day.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/word_reminder.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/word_timer.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/word_weekday.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/word_weekday_friday.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/word_weekday_monday.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/word_weekday_saturday.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/word_weekday_sunday.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/word_weekday_thursday.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/word_weekday_tuesday.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/word_weekday_wednesday.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/dialog/word_weekend.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:10:04.141191 neon-skill-alerts-1.5.2a4/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/intent/list_alerts.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/intent/quiet_hours_end.intent
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/intent/quiet_hours_start.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:10:04.145191 neon-skill-alerts-1.5.2a4/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/vocab/alarm.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/vocab/alert.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/vocab/all.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/vocab/articles.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/vocab/cancel.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/vocab/dismiss.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/vocab/event.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/vocab/everyday.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/vocab/next.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/vocab/playable.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/vocab/priority.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/vocab/query.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/vocab/remind_me.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/vocab/reminder.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/vocab/repeat.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/vocab/script.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/vocab/set.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/vocab/snooze.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/vocab/timer.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/vocab/timer_time_remaining.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/vocab/until.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/vocab/weekdays.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/locale/en-us/vocab/weekends.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:10:04.145191 neon-skill-alerts-1.5.2a4/neon_skill_alerts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-26 17:10:04.000000 neon-skill-alerts-1.5.2a4/neon_skill_alerts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-06-26 17:10:04.000000 neon-skill-alerts-1.5.2a4/neon_skill_alerts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:10:04.000000 neon-skill-alerts-1.5.2a4/neon_skill_alerts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-26 17:10:04.000000 neon-skill-alerts-1.5.2a4/neon_skill_alerts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-26 17:10:04.000000 neon-skill-alerts-1.5.2a4/neon_skill_alerts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-26 17:10:04.000000 neon-skill-alerts-1.5.2a4/neon_skill_alerts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 17:10:04.149191 neon-skill-alerts-1.5.2a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:10:04.145191 neon-skill-alerts-1.5.2a4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)   114134 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/test/test_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:10:04.145191 neon-skill-alerts-1.5.2a4/ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:10:04.145191 neon-skill-alerts-1.5.2a4/ui/+mediacenter/
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/+mediacenter/RoundProgress.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/+mediacenter/Timer.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/+mediacenter/TimerCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/AlarmBoxControl.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/AlarmBoxView.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/AlarmButtonView.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/AlarmCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/AlarmsOverviewCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/AlarmsOverviewDelegate.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/RoundProgress.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/Timer.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/TimerCard.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:10:04.145191 neon-skill-alerts-1.5.2a4/ui/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/icons/close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/icons/continue.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/icons/pause.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/qmldir
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:10:04.145191 neon-skill-alerts-1.5.2a4/ui/sounds/
+-rw-r--r--   0 runner    (1001) docker     (123)    15240 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/sounds/clicked.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:10:04.149191 neon-skill-alerts-1.5.2a4/ui/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/translations/TimerCard_de.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/translations/TimerCard_es.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/translations/TimerCard_fr.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/translations/TimerCard_it.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/translations/TimerCard_nl.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/translations/TimerCard_pt.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/translations/skill-ovos-timer.openvoiceos_de.qm
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/translations/skill-ovos-timer.openvoiceos_es.qm
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/translations/skill-ovos-timer.openvoiceos_fr.qm
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/translations/skill-ovos-timer.openvoiceos_it.qm
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/translations/skill-ovos-timer.openvoiceos_nl.qm
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/ui/translations/skill-ovos-timer.openvoiceos_pt.qm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:10:04.149191 neon-skill-alerts-1.5.2a4/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10166 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/util/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16625 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/util/alert_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22330 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/util/parse_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/util/ui_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-26 17:09:59.000000 neon-skill-alerts-1.5.2a4/version.py
```

### Comparing `neon-skill-alerts-1.5.2a3/LICENSE.md` & `neon-skill-alerts-1.5.2a4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-1.5.2a3/PKG-INFO` & `neon-skill-alerts-1.5.2a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-alerts
-Version: 1.5.2a3
+Version: 1.5.2a4
 Home-page: https://github.com/NeonGeckoCom/skill-alerts
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-alerts-1.5.2a3/README.md` & `neon-skill-alerts-1.5.2a4/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-1.5.2a3/__init__.py` & `neon-skill-alerts-1.5.2a4/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         # Initialize manager with any cached alerts
         self._alert_manager = AlertManager(os.path.join(self.file_system.path,
                                                         "alerts.json"),
                                            self.event_scheduler,
                                            self._alert_expired)
 
         # Update Homescreen UI models
-        self.add_event("mycroft.ready", self.on_ready, once=True)
+        self.add_event("mycroft.ready", self.on_ready)
 
         self.add_event("neon.get_events", self._get_events)
         self.add_event("alerts.gui.dismiss_notification",
                        self._gui_dismiss_notification)
         self.add_event("ovos.gui.show.active.timers", self._on_display_gui)
         self.add_event("ovos.gui.show.active.alarms", self._on_display_gui)
```

### Comparing `neon-skill-alerts-1.5.2a3/neon_skill_alerts.egg-info/PKG-INFO` & `neon-skill-alerts-1.5.2a4/neon_skill_alerts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-alerts
-Version: 1.5.2a3
+Version: 1.5.2a4
 Home-page: https://github.com/NeonGeckoCom/skill-alerts
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-alerts-1.5.2a3/neon_skill_alerts.egg-info/SOURCES.txt` & `neon-skill-alerts-1.5.2a4/neon_skill_alerts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-1.5.2a3/setup.py` & `neon-skill-alerts-1.5.2a4/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-1.5.2a3/skill.json` & `neon-skill-alerts-1.5.2a4/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-1.5.2a3/test/test_skill.py` & `neon-skill-alerts-1.5.2a4/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-1.5.2a3/ui/+mediacenter/RoundProgress.qml` & `neon-skill-alerts-1.5.2a4/ui/+mediacenter/RoundProgress.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-1.5.2a3/ui/+mediacenter/Timer.qml` & `neon-skill-alerts-1.5.2a4/ui/+mediacenter/Timer.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-1.5.2a3/ui/+mediacenter/TimerCard.qml` & `neon-skill-alerts-1.5.2a4/ui/+mediacenter/TimerCard.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-1.5.2a3/ui/AlarmBoxControl.qml` & `neon-skill-alerts-1.5.2a4/ui/AlarmBoxControl.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-1.5.2a3/ui/AlarmBoxView.qml` & `neon-skill-alerts-1.5.2a4/ui/AlarmBoxView.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-1.5.2a3/ui/AlarmButtonView.qml` & `neon-skill-alerts-1.5.2a4/ui/AlarmButtonView.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-1.5.2a3/ui/AlarmCard.qml` & `neon-skill-alerts-1.5.2a4/ui/AlarmCard.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-1.5.2a3/ui/AlarmsOverviewCard.qml` & `neon-skill-alerts-1.5.2a4/ui/AlarmsOverviewCard.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-1.5.2a3/ui/AlarmsOverviewDelegate.qml` & `neon-skill-alerts-1.5.2a4/ui/AlarmsOverviewDelegate.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-1.5.2a3/ui/RoundProgress.qml` & `neon-skill-alerts-1.5.2a4/ui/RoundProgress.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-1.5.2a3/ui/Timer.qml` & `neon-skill-alerts-1.5.2a4/ui/Timer.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-1.5.2a3/ui/TimerCard.qml` & `neon-skill-alerts-1.5.2a4/ui/TimerCard.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-1.5.2a3/ui/icons/close.svg` & `neon-skill-alerts-1.5.2a4/ui/icons/close.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-1.5.2a3/ui/sounds/clicked.wav` & `neon-skill-alerts-1.5.2a4/ui/sounds/clicked.wav`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-1.5.2a3/util/__init__.py` & `neon-skill-alerts-1.5.2a4/util/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-1.5.2a3/util/alert.py` & `neon-skill-alerts-1.5.2a4/util/alert.py`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-1.5.2a3/util/alert_manager.py` & `neon-skill-alerts-1.5.2a4/util/alert_manager.py`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-1.5.2a3/util/parse_utils.py` & `neon-skill-alerts-1.5.2a4/util/parse_utils.py`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-1.5.2a3/util/ui_models.py` & `neon-skill-alerts-1.5.2a4/util/ui_models.py`

 * *Files identical despite different names*

### Comparing `neon-skill-alerts-1.5.2a3/version.py` & `neon-skill-alerts-1.5.2a4/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.5.2a3"
+__version__ = "1.5.2a4"
```


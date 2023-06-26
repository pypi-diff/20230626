# Comparing `tmp/xirvik-tools-0.3.1.tar.gz` & `tmp/xirvik_tools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xirvik-tools-0.3.1.tar", last modified: Sun Mar  8 10:08:49 2020, max compression
+gzip compressed data, was "xirvik_tools-0.4.0.tar", max compression
```

## Comparing `xirvik-tools-0.3.1.tar` & `xirvik_tools-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,20 @@
-drwxr-x---   0 tatsh     (1000) tatsh     (1000)        0 2020-03-08 10:08:49.282678 xirvik-tools-0.3.1/
--rw-r-----   0 tatsh     (1000) tatsh     (1000)      586 2020-03-08 10:08:49.281679 xirvik-tools-0.3.1/PKG-INFO
--rw-r-----   0 tatsh     (1000) tatsh     (1000)      300 2020-02-20 00:53:15.000000 xirvik-tools-0.3.1/README.md
--rw-r-----   0 tatsh     (1000) tatsh     (1000)       38 2020-03-08 10:08:49.282678 xirvik-tools-0.3.1/setup.cfg
--rw-r-----   0 tatsh     (1000) tatsh     (1000)     1600 2020-03-08 10:08:25.000000 xirvik-tools-0.3.1/setup.py
-drwxr-x---   0 tatsh     (1000) tatsh     (1000)        0 2020-03-08 10:08:49.280679 xirvik-tools-0.3.1/xirvik/
--rw-r-----   0 tatsh     (1000) tatsh     (1000)       27 2018-07-18 04:54:42.000000 xirvik-tools-0.3.1/xirvik/__init__.py
--rw-r-----   0 tatsh     (1000) tatsh     (1000)    18647 2020-02-20 00:53:15.000000 xirvik-tools-0.3.1/xirvik/client.py
-drwxr-x---   0 tatsh     (1000) tatsh     (1000)        0 2020-03-08 10:08:49.280679 xirvik-tools-0.3.1/xirvik/commands/
--rw-r-----   0 tatsh     (1000) tatsh     (1000)      252 2019-12-05 00:32:29.000000 xirvik-tools-0.3.1/xirvik/commands/__init__.py
--rwxr-x---   0 tatsh     (1000) tatsh     (1000)     4024 2020-02-26 00:39:18.000000 xirvik-tools-0.3.1/xirvik/commands/delete_old.py
--rwxr-x---   0 tatsh     (1000) tatsh     (1000)     3031 2020-02-25 08:13:29.000000 xirvik-tools-0.3.1/xirvik/commands/move_by_label.py
--rwxr-x---   0 tatsh     (1000) tatsh     (1000)     2848 2020-03-08 10:06:46.000000 xirvik-tools-0.3.1/xirvik/commands/move_erroneous.py
--rw-r-----   0 tatsh     (1000) tatsh     (1000)    21626 2020-02-26 00:38:40.000000 xirvik-tools-0.3.1/xirvik/commands/simple.py
--rw-r-----   0 tatsh     (1000) tatsh     (1000)     1922 2020-03-08 09:44:03.000000 xirvik-tools-0.3.1/xirvik/commands/util.py
--rw-r-----   0 tatsh     (1000) tatsh     (1000)     1383 2020-03-08 09:08:45.000000 xirvik-tools-0.3.1/xirvik/log.py
--rw-r-----   0 tatsh     (1000) tatsh     (1000)    10669 2020-03-08 09:26:25.000000 xirvik-tools-0.3.1/xirvik/sftp.py
-drwxr-x---   0 tatsh     (1000) tatsh     (1000)        0 2020-03-08 10:08:49.281679 xirvik-tools-0.3.1/xirvik/test/
--rw-r-----   0 tatsh     (1000) tatsh     (1000)       94 2018-10-20 17:31:00.000000 xirvik-tools-0.3.1/xirvik/test/__init__.py
--rw-r-----   0 tatsh     (1000) tatsh     (1000)     6899 2020-01-23 04:25:17.000000 xirvik-tools-0.3.1/xirvik/test/test_client.py
--rw-r-----   0 tatsh     (1000) tatsh     (1000)     6859 2020-02-20 00:53:15.000000 xirvik-tools-0.3.1/xirvik/test/test_util.py
--rw-r-----   0 tatsh     (1000) tatsh     (1000)     1064 2020-03-08 09:53:51.000000 xirvik-tools-0.3.1/xirvik/typing.py
--rw-r-----   0 tatsh     (1000) tatsh     (1000)     6845 2020-03-08 09:46:09.000000 xirvik-tools-0.3.1/xirvik/util.py
-drwxr-x---   0 tatsh     (1000) tatsh     (1000)        0 2020-03-08 10:08:49.281679 xirvik-tools-0.3.1/xirvik_tools.egg-info/
--rw-r-----   0 tatsh     (1000) tatsh     (1000)      586 2020-03-08 10:08:49.000000 xirvik-tools-0.3.1/xirvik_tools.egg-info/PKG-INFO
--rw-r-----   0 tatsh     (1000) tatsh     (1000)      584 2020-03-08 10:08:49.000000 xirvik-tools-0.3.1/xirvik_tools.egg-info/SOURCES.txt
--rw-r-----   0 tatsh     (1000) tatsh     (1000)        1 2020-03-08 10:08:49.000000 xirvik-tools-0.3.1/xirvik_tools.egg-info/dependency_links.txt
--rw-r-----   0 tatsh     (1000) tatsh     (1000)      493 2020-03-08 10:08:49.000000 xirvik-tools-0.3.1/xirvik_tools.egg-info/entry_points.txt
--rw-r-----   0 tatsh     (1000) tatsh     (1000)      205 2020-03-08 10:08:49.000000 xirvik-tools-0.3.1/xirvik_tools.egg-info/requires.txt
--rw-r-----   0 tatsh     (1000) tatsh     (1000)        7 2020-03-08 10:08:49.000000 xirvik-tools-0.3.1/xirvik_tools.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1072 2015-04-05 10:25:34.116301 xirvik_tools-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0      628 2023-04-11 15:59:06.810994 xirvik_tools-0.4.0/LaunchAgents/README.md
+-rw-r--r--   0        0        0      733 2023-04-14 20:37:57.649077 xirvik_tools-0.4.0/LaunchAgents/sh.tat.XirvikStartTorrents.plist
+-rw-r--r--   0        0        0      297 2021-09-30 10:40:35.069636 xirvik_tools-0.4.0/README.md
+-rw-r--r--   0        0        0     1509 2023-06-26 20:04:24.702376 xirvik_tools-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      815 2020-02-20 00:53:15.113538 xirvik_tools-0.4.0/systemd/README.md
+-rw-r--r--   0        0        0      140 2021-09-12 02:01:33.922925 xirvik_tools-0.4.0/systemd/xirvik-start-torrents.service
+-rw-r--r--   0        0        0      128 2020-02-20 00:53:15.113538 xirvik_tools-0.4.0/systemd/xirvik-start-torrents.timer
+-rw-r--r--   0        0        0       95 2020-10-29 09:51:37.765849 xirvik_tools-0.4.0/xirvik/__init__.py
+-rw-r--r--   0        0        0    15074 2023-06-26 20:04:24.702376 xirvik_tools-0.4.0/xirvik/client.py
+-rw-r--r--   0        0        0       71 2021-09-14 05:10:34.682258 xirvik_tools-0.4.0/xirvik/commands/__init__.py
+-rw-r--r--   0        0        0     4104 2023-04-14 20:32:03.847391 xirvik_tools-0.4.0/xirvik/commands/delete_old.py
+-rw-r--r--   0        0        0     3841 2023-05-25 22:51:02.179751 xirvik_tools-0.4.0/xirvik/commands/move_by_label.py
+-rw-r--r--   0        0        0     2936 2023-04-14 20:32:03.841391 xirvik_tools-0.4.0/xirvik/commands/move_erroneous.py
+-rw-r--r--   0        0        0     1710 2023-04-14 20:32:03.847391 xirvik_tools-0.4.0/xirvik/commands/root.py
+-rw-r--r--   0        0        0    18568 2023-04-14 20:37:57.649077 xirvik_tools-0.4.0/xirvik/commands/simple.py
+-rw-r--r--   0        0        0     7017 2023-04-16 21:50:00.051679 xirvik_tools-0.4.0/xirvik/commands/util.py
+-rw-r--r--   0        0        0     2412 2023-04-14 20:37:57.649077 xirvik_tools-0.4.0/xirvik/typing.py
+-rw-r--r--   0        0        0     1065 2023-06-26 20:04:24.702376 xirvik_tools-0.4.0/xirvik/utils.py
+-rw-r--r--   0        0        0     1419 1970-01-01 00:00:00.000000 xirvik_tools-0.4.0/PKG-INFO
```

### Comparing `xirvik-tools-0.3.1/xirvik/commands/delete_old.py` & `xirvik_tools-0.4.0/xirvik/commands/delete_old.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,117 +1,117 @@
 #!/usr/bin/env python
-# PYTHON_ARGCOMPLETE_OK
 """
 Deletes old torrents based on specified criteria.
 """
 from datetime import datetime, timedelta
+from os.path import expanduser
 from time import sleep
-from typing import Any, Callable, Dict, Optional, Tuple, Union
-import logging
-import sys
+from typing import Callable
 import xmlrpc.client as xmlrpc
 
+from loguru import logger
 from requests.exceptions import HTTPError
-import argcomplete
+import click
+
+from xirvik.typing import TorrentInfo
 
 from ..client import ruTorrentClient
-from .util import common_parser, setup_logging_stdout
+from .util import command_with_config_file, common_options_and_arguments, setup_logging
 
-TestCallable = Callable[[Dict[str, Any], logging.Logger], Tuple[str, bool]]
-TestsDict = Dict[str, Tuple[bool, TestCallable]]
+TestCallable = Callable[[TorrentInfo], tuple[str, bool]]
+TestsDict = dict[str, tuple[bool, TestCallable]]
 
 
 def _test_date_cb(days: int = 14) -> TestCallable:
-    def test_date(info: Dict[str, datetime],
-                  log: logging.Logger) -> Tuple[str, bool]:
-        cond1 = info.get('creation_date')
-        cond2 = info.get('state_changed')
+    def test_date(info: TorrentInfo) -> tuple[str, bool]:
+        condition1 = info.creation_date
+        condition2 = info.state_changed
         expect = datetime.now() - timedelta(days=days)
-        log = setup_logging_stdout()
-        log.debug('creation date: %s', cond1)
-        log.debug('state changed: %s', cond2)
-        log.debug('%s <= %s or', cond1, expect)
-        log.debug('    %s <= %s', cond2, expect)
+        logger.debug(f'creation date: {condition1}')
+        logger.debug(f'state changed: {condition2}')
+        logger.debug(f'{condition1} <= {expect} or')
+        logger.debug(f'    {condition2} <= {expect}')
         return (
-            'over 14 days seeded',
-            bool((cond1 and cond1 <= expect) or (cond2 and cond2 <= expect)),
+            f'over {days} days seeded',
+            bool((condition1 and condition1 <= expect) or (condition2 and condition2 <= expect)),
         )
 
     return test_date
 
 
-def _test_ratio(info: Dict[str, float],
-                log: logging.Logger) -> Tuple[str, bool]:
-    log.debug('ratio: %.2f', info.get('ratio', 0.0))
-    return 'ratio >= 1', info.get('ratio', 0.0) >= 1
-
-
-def _test_ignore(_info: Any) -> Tuple[str, bool]:
-    return 'ignoring criteria', True
-
-
-def main() -> int:
-    """Entry point."""
-    parser = common_parser()
-    parser.add_argument('-a', '--ignore-ratio', action='store_true')
-    parser.add_argument('-D', '--ignore-date', action='store_true')
-    parser.add_argument('-y', '--dry-run', action='store_true')
-    parser.add_argument('--max-attempts', type=int, default=3)
-    parser.add_argument('--label')
-    parser.add_argument('--sleep-time', type=int, default=10)
-    parser.add_argument('--days', type=int, default=14)
-    argcomplete.autocomplete(parser)
-    args = parser.parse_args()
-    log = setup_logging_stdout(verbose=args.verbose)
-    client = ruTorrentClient(args.host[0],
-                             name=args.username,
-                             password=args.password,
-                             max_retries=args.max_retries,
-                             netrc_path=args.netrc)
+def _test_ratio(info: TorrentInfo) -> tuple[str, bool]:
+    logger.debug(f'ratio: {info.ratio:.2f}')
+    return 'ratio >= 1', info.ratio >= 1
+
+
+@click.command(cls=command_with_config_file('config', 'delete-old'))
+@common_options_and_arguments
+@click.option('-D', '--ignore-date', is_flag=True)
+@click.option('-a', '--ignore-ratio', is_flag=True)
+@click.option('-y', '--dry-run', is_flag=True)
+@click.option('--days', type=int, default=14)
+@click.option('--label', default=None)
+@click.option('--max-attempts', type=int, default=3)
+@click.option('--sleep-time', type=int, default=10)
+def main(  # pylint: disable=too-many-arguments,unused-argument,unused-variable
+        host: str,
+        debug: bool = False,
+        netrc: str | None = None,
+        username: str | None = None,
+        password: str | None = None,
+        ignore_ratio: bool = False,
+        ignore_date: bool = False,
+        label: str | None = None,
+        max_attempts: int = 3,
+        dry_run: bool = False,
+        max_retries: int = 10,
+        days: int = 14,
+        backoff_factor: int = 1,
+        sleep_time: int = 10,
+        config: str | None = None) -> None:
+    """Delete torrents based on certain criteria."""
+    setup_logging(debug)
+    client = ruTorrentClient(host,
+                             name=username,
+                             password=password,
+                             max_retries=max_retries,
+                             netrc_path=netrc or expanduser('~/.netrc'))
     try:
-        torrents = client.list_torrents_dict().items()
-    except HTTPError:
-        log.error('Connection failed on list_torrents() call', file=sys.stderr)
-        return 1
-    tests: TestsDict = dict(
-        ratio=(args.ignore_ratio, _test_ratio),
-        date=(args.ignore_date, _test_date_cb(args.days)),
+        torrents = client.list_torrents()
+    except HTTPError as e:
+        logger.error('Connection failed on list_torrents() call')
+        raise click.Abort() from e
+    tests = dict(
+        ratio=(ignore_ratio, _test_ratio),
+        date=(ignore_date, _test_date_cb(days)),
     )
-    info: Dict[str, Union[int, str, bool]]
-    for hash_, info in torrents:
-        if info['left_bytes'] != 0 or info['custom1'] != args.label:
+    for info in torrents:
+        if info.left_bytes != 0 or info.custom1 != label:
             continue
-        reason: Optional[str] = None
-        can_delete: bool = False
+        reason: str | None = None
+        can_delete = False
         for key, (can_ignore, test) in tests.items():
             if can_ignore:
                 can_delete = True
                 reason = f'ignoring {key}'
                 break
-            reason, can_delete = test(info, log)
+            reason, can_delete = test(info)
             if can_delete:
                 break
         if not can_delete:
-            log.info('Cannot delete %s', info['name'])
+            logger.info(f'Cannot delete {info.name}')
             continue
-        if args.dry_run:
-            log.info('Would delete %s, reason: %s', info['name'], reason)
+        if dry_run:
+            logger.info(f'Would delete {info.name}, reason: {reason}')
             continue
-        else:
-            log.info('Deleting %s, reason: %s', info['name'], reason)
+        logger.info(f'Deleting {info.name}, reason: {reason}')
         attempts = 0
-        while attempts < args.max_attempts:
+        while attempts < max_attempts:
             attempts += 1
             try:
-                client.delete(hash_)
-            except xmlrpc.Fault as e:
-                log.exception(e)
-                sleep_time = args.backoff_factor * (2**(attempts - 1))
+                client.delete(info.hash)
+            except (xmlrpc.Fault, xmlrpc.ProtocolError):
+                sleep_time = backoff_factor * (2 ** (attempts - 1))
                 sleep(sleep_time)
             else:
-                sleep(args.sleep_time)
+                sleep(sleep_time)
                 break
-    return 0
-
-
-if __name__ == '__main__':
-    sys.exit(main())
```

### Comparing `xirvik-tools-0.3.1/xirvik/commands/move_erroneous.py` & `xirvik_tools-0.4.0/xirvik/commands/move_erroneous.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,86 +1,89 @@
 """Move torrents in error state to another location."""
 from time import sleep
-from typing import Iterable, List, Tuple, TypeVar, cast
-import sys
+from typing import Any, Final, Iterable, TypeVar
 
-from typing_extensions import Final
-import argcomplete
+from loguru import logger
+import click
 
 from ..client import ruTorrentClient
-from ..typing import TorrentDict
-from .util import common_parser, setup_logging_stdout
+from ..typing import TorrentInfo
+from .util import command_with_config_file, common_options_and_arguments, setup_logging
 
-__all__ = ("main", )
+__all__ = ('main',)
 
-PREFIX: Final = '/torrents/{}/_completed-not-active'
-BAD_MESSAGES: Final = (
+PREFIX: Final[str] = '/torrents/{}/_completed-not-active'
+BAD_MESSAGES: Final[tuple[str, ...]] = (
     'unregistered torrent',
-    "couldn't connect to server",
+    "couldn't connect to server",  # pylint: disable=invalid-string-quote
     'server returned nothing',
 )
 T = TypeVar('T')
 
 
 def _has_one(look_for_list: Iterable[T], val: Iterable[T]) -> bool:
     for candidate in look_for_list:
         if candidate in val:
             return True
     return False
 
 
-def _should_process(x: TorrentDict) -> bool:
-    return (_has_one(BAD_MESSAGES, x['message']) and not x['is_hash_checking']
-            and x['left_bytes'] == 0)
+def _should_process(x: TorrentInfo) -> bool:
+    logger.debug(f'Name: "{x.name}", message: "{x.message}", '
+                 f'is_hash_checking: {x.is_hash_checking}, '
+                 f'left_bytes: {x.left_bytes}')
+    return (_has_one(BAD_MESSAGES, x.message.lower()) and not x.is_hash_checking
+            and x.left_bytes == 0 and bool(x.custom1))
 
 
 def _make_move_to(prefix: str, label: str) -> str:
-    return '{}/{}'.format(prefix, label)
+    return f'{prefix}/{label}'
 
 
-def main() -> int:
+# pylint: disable=unused-argument
+@click.command(cls=command_with_config_file('config', 'move-erroneous'))
+@common_options_and_arguments
+@click.option('--sleep-time', type=int, default=10)
+def main(
+    host: str,
+    netrc: str | None = None,
+    username: str | None = None,
+    password: str | None = None,
+    sleep_time: int = 10,
+    debug: bool = False,
+    max_retries: int = 10,
+    **kwargs: Any,
+) -> None:
     """Move torrents in error state to another location."""
-    parser: Final = common_parser()
-    parser.add_argument('-a', '--ignore-ratio', action='store_true')
-    parser.add_argument('-t', '--sleep-time', default=10, type=int)
-    argcomplete.autocomplete(parser)
-    args: Final = parser.parse_args()
-    log: Final = setup_logging_stdout(verbose=args.verbose)
-    client: Final = ruTorrentClient(args.host[0],
-                                    name=args.username,
-                                    password=args.password,
-                                    max_retries=args.max_retries,
-                                    netrc_path=args.netrc)
-    prefix: Final = PREFIX.format(args.username)
-    to_delete: List[Tuple[str, str]] = []
-    items: Final = [(hash_, cast(TorrentDict, info))
-                    for hash_, info in client.list_torrents_dict().items()
-                    if _should_process(cast(TorrentDict, info))]
+    setup_logging(debug)
+    client = ruTorrentClient(host,
+                             name=username,
+                             password=password,
+                             max_retries=max_retries,
+                             netrc_path=netrc)
+    prefix = PREFIX.format(client.name)
+    to_delete: list[tuple[str, str]] = []
+    items = [info for info in client.list_torrents() if _should_process(info)]
     count = 0
-    for hash_, info in items:
-        log.info('Stopping %s', info['name'])
-        client.stop(hash_)
+    for info in items:
+        logger.info(f'Stopping {info.name}')
+        client.stop(info.hash)
         count += 1
         if count > 0 and (count % 10) == 0:
-            sleep(args.sleep_time)
+            sleep(sleep_time)
     count = 0
-    for hash_, info in items:
-        move_to = _make_move_to(prefix, info['custom1'].lower())
-        to_delete.append((hash_, info['name']))
-        log.info('Moving %s to %s/', info['name'], move_to)
-        client.move_torrent(hash_, move_to)
-        client.stop(hash_)
+    for info in items:
+        move_to = _make_move_to(prefix, info.custom1.lower())
+        to_delete.append((info.hash, info.name))
+        logger.info(f'Moving {info.name} to {move_to}/')
+        client.move_torrent(info.hash, move_to)
+        client.stop(info.hash)
         count += 1
         if count > 0 and (count % 10) == 0:
-            sleep(args.sleep_time)
+            sleep(sleep_time)
     count = 0
     for hash_, name in to_delete:
-        log.info('Removing torrent "%s" (without deleting data)', name)
+        logger.info(f'Removing torrent "{name}" (without deleting data)')
         client.remove(hash_)
         count += 1
         if count > 0 and (count % 10) == 0:
-            sleep(args.sleep_time)
-    return 0
-
-
-if __name__ == '__main__':
-    sys.exit(main())
+            sleep(sleep_time)
```


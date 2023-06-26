# Comparing `tmp/libretrofuzz-3.3.3.tar.gz` & `tmp/libretrofuzz-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretrofuzz-3.3.3.tar", max compression
+gzip compressed data, was "libretrofuzz-3.3.4.tar", max compression
```

## Comparing `libretrofuzz-3.3.3.tar` & `libretrofuzz-3.3.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-22 04:05:13.362689 libretrofuzz-3.3.3/LICENSE
--rw-r--r--   0        0        0     7554 2023-06-22 04:05:13.362689 libretrofuzz-3.3.3/README.rst
--rw-r--r--   0        0        0       22 2023-06-22 04:05:13.362689 libretrofuzz-3.3.3/libretrofuzz/__init__.py
--rw-r--r--   0        0        0    56511 2023-06-22 04:05:13.366689 libretrofuzz-3.3.3/libretrofuzz/__main__.py
--rw-r--r--   0        0        0     1275 2023-06-22 04:05:13.366689 libretrofuzz-3.3.3/pyproject.toml
--rw-r--r--   0        0        0     8735 2023-06-22 04:05:23.446710 libretrofuzz-3.3.3/setup.py
--rw-r--r--   0        0        0     8743 2023-06-22 04:05:23.447914 libretrofuzz-3.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-26 18:00:49.676042 libretrofuzz-3.3.4/LICENSE
+-rw-r--r--   0        0        0     8035 2023-06-26 18:00:49.676042 libretrofuzz-3.3.4/README.rst
+-rw-r--r--   0        0        0       22 2023-06-26 18:00:49.676042 libretrofuzz-3.3.4/libretrofuzz/__init__.py
+-rw-r--r--   0        0        0    56851 2023-06-26 18:00:49.676042 libretrofuzz-3.3.4/libretrofuzz/__main__.py
+-rw-r--r--   0        0        0     1275 2023-06-26 18:00:49.676042 libretrofuzz-3.3.4/pyproject.toml
+-rw-r--r--   0        0        0     9233 2023-06-26 18:01:01.822805 libretrofuzz-3.3.4/setup.py
+-rw-r--r--   0        0        0     9224 2023-06-26 18:01:01.823924 libretrofuzz-3.3.4/PKG-INFO
```

### Comparing `libretrofuzz-3.3.3/LICENSE` & `libretrofuzz-3.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `libretrofuzz-3.3.3/README.rst` & `libretrofuzz-3.3.4/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -48,35 +48,52 @@
                         Linux default:   ``~/.config/retroarch/retroarch.cfg``
 
                         Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``
 
                         MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``
 
   --playlist <NAME libretro-fuzz only>
-                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.
+                        | Playlist name with labels used for thumbnail fuzzy matching.
+                        | If not provided, asked from the user.
   --system <NAME libretro-fuzz only>
-                        Directory name in the server to download thumbnails. If not provided, asked from the user.
-  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.
+                        | Directory name in the server to download thumbnails.
+                        | If not provided, asked from the user.
+  --delay-after SECS    | Seconds after download to skip replacing thumbnails, enter continues.
+                        | No-op with ``--no-image``.
                         | [1<=x<=60]
-  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.
+  --delay SECS          | Seconds to skip thumbnails download, enter continues.
                         | [1<=x<=60]
-  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.
+  --filter GLOB         | Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times.
+                        | Resets thumbnails, ``--filter '*'`` redownloads all.
   --min SCORE           | 0=any, 100≃equal, 90=default. No-op with ``--no-fail``.
                         | [default: 90; 0<=x<=100]
   --no-fail             Download any score. Equivalent to ``--min 0``.
   --no-image            Don't show images even with chafa installed.
-  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.
-  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.
-  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.
-  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.
-  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.
+  --no-merge            | Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls.
+                        | No-op with ``--filter``.
+  --no-meta             | Ignores () delimited metadata.
+                        | May cause false positives.
+                        | Forced with ``--before``.
+  --hack                | Matches [] delimited metadata, best used if the hack has thumbnails.
+                        | May cause false positives.
+                        | Ignored with ``--before``.
+  --before TEXT         | Use only the part of the label before TEXT to match.
+                        | TEXT may not be inside of brackets of any kind.
+                        | May cause false positives.
+                        | Forces ignoring metadata.
+  --address URL         | URL with libretro-thumbnails server, for local files:
+                        | Go to RA thumbnail dir/git clone/unzip packs;
+                        | Run ``'python3 -m http.server'`` in parent dir;
+                        | Then use ``--address 'http://localhost:8000'``.
                         | [default: https://thumbnails.libretro.com]
   --dry-run             Print results only, no delay or image download.
-  --verbose N           | Show length N list: score, name, emoji hyperlinks.
-                        | [x>=1]
+  --limit GAMES         | Show a number of winners or losers.
+                        | Any equal score winners can download images.
+                        | [default: 1; x>=1]
+  --verbose             Show failed matches.
   --install-completion  Install completion for the current shell.
   --show-completion     Show completion for the current shell, to copy it or customize the installation.
   --help                Show this message and exit.
 
 
 
 To install the program, type on the cmd line
```

### Comparing `libretrofuzz-3.3.3/libretrofuzz/__main__.py` & `libretrofuzz-3.3.4/libretrofuzz/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,25 +55,30 @@
 ###########################################
 
 ADDRESS = "https://thumbnails.libretro.com"
 DEF_SCORE = 90
 MAX_SCORE = 100
 MAX_RETRIES = 3
 MAX_WAIT_SECS = 60
+# Local libretro thumbnail directories
+THUMB_LDIRS = ["Named_Boxarts", "Named_Titles", "Named_Snaps"]
+# Server thumbnail directories, change if the server
+# is organized the same way but with different names
+THUMB_SDIRS = ["Named_Boxarts", "Named_Titles", "Named_Snaps"]
 # 00-1f are ascii control codes, rest are illegal windows filename chars according to powershell + &
 forbidden = regex.compile(
     r"[\u0022\u003c\u003e\u007c\u0000\u0001\u0002\u0003\u0004\u0005\u0006\u0007\u0008"
     + r"\u0009\u000a\u000b\u000c\u000d\u000e\u000f\u0010\u0011\u0012\u0013\u0014\u0015"
     + r"\u0016\u0017\u0018\u0019\u001a\u001b\u001c\u001d\u001e\u001f\u003a\u002a\u003f\u005c\u002f\u0026]"
 )
 # external terminal image viewer application
 viewer = None
 
 # makes a class with these fields, the subdir names on the server system dir of the types of thumbnails
-Thumbs = collections.namedtuple("Thumbs", ["Named_Boxarts", "Named_Titles", "Named_Snaps"])
+Thumbs = collections.namedtuple("Thumbs", THUMB_LDIRS)
 # this is for 64 bits too
 if sys.platform == "win32":
     # this order is to make 'portable' installs have priority in windows
     # a concept that doesn't exist in linux or macosx
     # these are the default 32 and 64 bits installer paths, since there
     # is no way to know what the user choses, check the defaults only.
     CONFIG = Path(r"C:/RetroArch-Win64/retroarch.cfg")
@@ -534,15 +539,15 @@
     # create the directories we will 'maybe' need. This is not so problematic
     # as it seems since likely len(dbs) == 1, so 6 directories per playlist
     # versus having os.makedirs called hundred of times for larger playlists
     # this is vulnerable to ToCToU deletion but everything is with directories
     dbs_set = set(dbs)
     for parent in [temp_dir, thumbnails_dir]:
         for db in dbs_set:
-            for dirname in Thumbs._fields:
+            for dirname in THUMB_LDIRS:
                 os.makedirs(Path(parent, db, dirname), exist_ok=True)
     return names, dbs
 
 
 def getPath(cfg: Path, setting: str, default_value: str):
     """returns paths inside of a cfg file setting"""
     try:
@@ -687,31 +692,31 @@
     ),
     wait_after: Optional[float] = Option(
         None,
         "--delay-after",
         min=1,
         max=MAX_WAIT_SECS,
         clamp=True,
-        metavar="FLOAT",
+        metavar="SECS",
         help="Seconds after download to skip replacing thumbnails, enter continues. No-op with --no-image.",
     ),
     wait_before: Optional[float] = Option(
         None,
         "--delay",
         min=1,
         max=MAX_WAIT_SECS,
         clamp=True,
-        metavar="FLOAT",
+        metavar="SECS",
         help="Seconds to skip thumbnails download, enter continues.",
     ),
     filters: Optional[List[str]] = Option(
         None,
         "--filter",
         metavar="GLOB",
-        help="Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, --filter '*' redownloads all.",
+        help="Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times. Resets thumbnails, --filter '*' redownloads all.",
     ),
     score: int = Option(
         DEF_SCORE,
         "--min",
         min=0,
         max=MAX_SCORE,
         metavar="SCORE",
@@ -723,34 +728,39 @@
         False,
         "--no-merge",
         help="Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with --filter.",
     ),
     nometa: bool = Option(
         False,
         "--no-meta",
-        help="Ignores () delimited metadata and may cause false positives. Forced with --before.",
+        help="Ignores () delimited metadata. May cause false positives. Forced with --before.",
     ),
     hack: bool = Option(
         False,
         "--hack",
-        help="Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with --before.",
+        help="Matches [] delimited metadata, best used if the hack has thumbnails. May cause false positives. Ignored with --before.",
     ),
     before: Optional[str] = Option(
         None,
-        help="Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.",
+        help="Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind. May cause false positives. Forces ignoring metadata.",
     ),
     address: Optional[str] = Option(
         ADDRESS,
         metavar="URL",
-        help="URL with libretro-thumbnails server. For local files, git clone/unzip packs, run 'python3 -m http.server' in parent dir, and use --address 'http://localhost:8000'.",
+        help="URL with libretro-thumbnails server, for local files: go to RA thumbnail dir/git clone/unzip packs; run 'python3 -m http.server' in parent dir; then use --address 'http://localhost:8000'.",
     ),
     dryrun: bool = Option(False, "--dry-run", help="Print results only, no delay or image download."),
-    verbose: Optional[int] = Option(
-        None, "--verbose", min=1, metavar="N", help="Show length N list: score, name, emoji hyperlinks."
+    limit: Optional[int] = Option(
+        1,
+        "--limit",
+        min=1,
+        metavar="GAMES",
+        help="Show a number of winners or losers. Any equal score winners can download images.",
     ),
+    verbose: bool = Option(False, "--verbose", min=1, help="Show failed matches."),
 ):
     if playlist and not playlist.lower().endswith(".lpl"):
         playlist = playlist + ".lpl"
 
     (nub_verbose, playlist_dir, thumbnails_dir, playlists, systems) = common_errors(
         cfg, playlist, system, address
     )
@@ -804,14 +814,15 @@
                         dryrun,
                         score,
                         noimage,
                         nomerge,
                         nofail,
                         nometa,
                         hack,
+                        limit,
                         verbose,
                         nub_verbose,
                         before,
                         tmpdir,
                         thumbnails_dir,
                         client,
                     )
@@ -838,31 +849,31 @@
     ),
     wait_after: Optional[float] = Option(
         None,
         "--delay-after",
         min=1,
         max=MAX_WAIT_SECS,
         clamp=True,
-        metavar="FLOAT",
+        metavar="SECS",
         help="Seconds after download to skip replacing thumbnails, enter continues. No-op with --no-image.",
     ),
     wait_before: Optional[float] = Option(
         None,
         "--delay",
         min=1,
         max=MAX_WAIT_SECS,
         clamp=True,
-        metavar="FLOAT",
+        metavar="SECS",
         help="Seconds to skip thumbnails download, enter continues.",
     ),
     filters: Optional[List[str]] = Option(
         None,
         "--filter",
         metavar="GLOB",
-        help="Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, --filter '*' redownloads all.",
+        help="Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times. Resets thumbnails, --filter '*' redownloads all.",
     ),
     score: int = Option(
         DEF_SCORE,
         "--min",
         min=0,
         max=MAX_SCORE,
         metavar="SCORE",
@@ -874,34 +885,39 @@
         False,
         "--no-merge",
         help="Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with --filter.",
     ),
     nometa: bool = Option(
         False,
         "--no-meta",
-        help="Ignores () delimited metadata and may cause false positives. Forced with --before.",
+        help="Ignores () delimited metadata. May cause false positives. Forced with --before.",
     ),
     hack: bool = Option(
         False,
         "--hack",
-        help="Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with --before.",
+        help="Matches [] delimited metadata, best used if the hack has thumbnails. May cause false positives. Ignored with --before.",
     ),
     before: Optional[str] = Option(
         None,
-        help="Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.",
+        help="Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind. May cause false positives. Forces ignoring metadata.",
     ),
     address: Optional[str] = Option(
         ADDRESS,
         metavar="URL",
-        help="URL with libretro-thumbnails server. For local files, git clone/unzip packs, run 'python3 -m http.server' in parent dir, and use --address 'http://localhost:8000'.",
+        help="URL with libretro-thumbnails server, for local files: go to RA thumbnail dir/git clone/unzip packs; run 'python3 -m http.server' in parent dir; then use --address 'http://localhost:8000'.",
     ),
     dryrun: bool = Option(False, "--dry-run", help="Print results only, no delay or image download."),
-    verbose: Optional[int] = Option(
-        None, "--verbose", min=1, metavar="N", help="Show length N list: score, name, emoji hyperlinks."
+    limit: Optional[int] = Option(
+        1,
+        "--limit",
+        min=1,
+        metavar="GAMES",
+        help="Show a number of winners or losers. Any equal score winners can download images.",
     ),
+    verbose: bool = Option(False, "--verbose", min=1, help="Show failed matches."),
 ):
     (nub_verbose, _, thumbnails_dir, playlists, systems) = common_errors(cfg, None, None, address)
 
     notInSystems = [
         (playlist, os.path.basename(playlist)[:-4])
         for playlist in playlists
         if os.path.basename(playlist)[:-4] not in systems
@@ -933,14 +949,15 @@
                                 dryrun,
                                 score,
                                 noimage,
                                 nomerge,
                                 nofail,
                                 nometa,
                                 hack,
+                                limit,
                                 verbose,
                                 nub_verbose,
                                 before,
                                 tmpdir,
                                 thumbnails_dir,
                                 client,
                             )
@@ -950,23 +967,22 @@
             error("Cancelled by user, exiting")
             raise Exit()
 
     asyncio.run(runit(), debug=False)
 
 
 async def downloadgamenames(client, system, nub_verbose):
-    """returns [ dict(Game_Name, Game_Url), dict(Game_Name, Game_Url), dict(Game_Name, Game_Url) ]
-    for each of the server directories '/Named_Boxarts/', '/Named_Titles/', '/Named_Snaps/'
-    (potentially some of these dicts may be empty if the server doesn't have the directory)
+    """returns [ dict(Game_Name, Game_Url),..., dict(Game_Name, Game_Url) ] for each
+    of the server download directories (dicts may be empty if the server dir is empty)
     """
     lr_thumbs = ADDRESS + "/" + quote(system)  # then get the thumbnails from the system name
     args = []
     try:
-        for tdir, emoji in [("/Named_Boxarts/", "🎴"), ("/Named_Titles/", "🎬"), ("/Named_Snaps/", "📸")]:
-            lr_thumb = lr_thumbs + tdir
+        for tdir, emoji in zip(THUMB_SDIRS, ["🎴", "🎬", "📸"]):
+            lr_thumb = f"{lr_thumbs}/{tdir}/"
             response = ""
             async with client.stream("GET", lr_thumb, timeout=15) as r:
                 async for chunk in r.aiter_text(4096):
                     checkEscape()
                     response += chunk
             # not found is ok, some system directories don't have all the subdirectories
             if r.status_code == 404:
@@ -1005,15 +1021,16 @@
     dryrun: bool,
     score: int,
     noimage: bool,
     nomerge: bool,
     nofail: bool,
     nometa: bool,
     hack: bool,
-    verbose: Optional[int],
+    limit: Optional[int],
+    verbose: bool,
     nub_verbose: bool,
     before: Optional[str],
     tmpdir: Path,
     thumbnails_dir: Path,
     client: AsyncClient,
 ):
     # number of success and failures to print at the end
@@ -1041,15 +1058,15 @@
 
     thumbs = Thumbs._make(await downloadgamenames(client, system, nub_verbose))
     # we choose the highest similarity of all 3 directories,
     # since no mixed matches are allowed
     # (until you call again without --no-merge anyway
     # or if they have the same score)
     remote_names = set()
-    remote_names.update(thumbs.Named_Boxarts.keys(), thumbs.Named_Titles.keys(), thumbs.Named_Snaps.keys())
+    remote_names.update(thumbs[0].keys(), thumbs[1].keys(), thumbs[2].keys())
     if not remote_names:
         raise StopPlaylist()
 
     # preprocess data to build a heuristic later. Do not move
     # into the later loop because thats when the heuristic is used
     def norm(n):
         return normalizer(nometa, hack, n)
@@ -1074,42 +1091,42 @@
     for name, destination in zip(names, dbs):
         await asyncio.sleep(0)  # update key status
         checkEscape()  # check key status
         # if the user used filters, filter everything that doesn't match any of the globs
         if filters and not any(map(lambda x: fnmatch.fnmatch(name, x), filters)):
             continue
         # normalization can make it so that the winner has the same score as the runner up(s)
-        # so enabling 'verbose 2+' can improve results if the server is badly organized
+        # so enabling 'limit 2+' can improve results if the server is badly organized
         # however, do not do it by default, since it's a bit confusing.
-        result = process.extract(name, remote_names, scorer=scorer, limit=verbose or 1)
+        result = process.extract(name, remote_names, scorer=scorer, limit=limit or 1)
         assert result
         _, best_score, _ = result[0]
         winners = [x for x in result if x[1] == best_score and x[1] >= score]
         show = result if verbose else winners
         name_format = style((normcache[name][0] if short_names else name) + ": ", bold=True)
         # still remove the forbidden characters
         # the name will be used in the filename
         name = regex.sub(forbidden, "_", name)
         # Delete old images in the case of --filter.
         # this always happens, for consistency
         if filters and not dryrun:
-            for dirname in Thumbs._fields:
+            for dirname in THUMB_LDIRS:
                 Path(thumbnails_dir, destination, dirname, name + ".png").unlink(missing_ok=True)
         if winners:
             allow = True
             # these parent directories were created when reading the playlist
             # more efficient than doing it a playlist game loop
             real_thumb_dir = Path(thumbnails_dir, destination)
             down_thumb_dir = Path(tmpdir, destination)
             if nomerge:
                 # to implement no-merge you have to disable downloads on
                 # 'at least one' thumbnail (including user added ones)
                 missing_thumbs = 0
                 served__thumbs = False
-                for dirname in Thumbs._fields:
+                for dirname in THUMB_LDIRS:
                     real = Path(real_thumb_dir, dirname, name + ".png")
                     if not real.exists():
                         missing_thumbs += 1
                         if not served__thumbs:
 
                             def checkremote(winner):
                                 return winner[0] in getattr(thumbs, dirname)
@@ -1135,15 +1152,15 @@
                 getting_format = f'{style("Getting",    fg=BLUE, bold=True)}: {dull_format}' + style(
                     " {percentage:3.0f}%", fg=BLUE, bold=True
                 )
                 waiting_format = f'{style("Waiting",  fg=YELLOW, bold=True)}: {dull_format}' + style(
                     " {remaining_s:2.1f}s", fg=RED, bold=True
                 )
                 try:
-                    for dirname in Thumbs._fields:
+                    for dirname in THUMB_LDIRS:
                         real = Path(real_thumb_dir, dirname, name + ".png")
                         temp = Path(down_thumb_dir, dirname, name + ".png")
                         downloaded_dict[dirname] = (real, temp)
                         for winner in winners:
                             t_name, t_score, _ = winner
                             # something to download
                             url = getattr(thumbs, dirname).get(t_name, None)
@@ -1211,17 +1228,17 @@
     thumb_norm = norm_cache[thumb_name][0]
     score_color = RED if thumb_score < required_score else GREEN
     thumb_magnt = f"{thumb_score:.4f}" if short_names else f"{thumb_score:.1f}"
     score_text = style(thumb_magnt, fg=score_color, bold=True)
     if nub_verbose:
         return f"{score_text} {thumb_norm}"
     elif urlsdict:
-        url1 = urlsdict.get(("Named_Boxarts", r), None)
-        url2 = urlsdict.get(("Named_Titles", r), None)
-        url3 = urlsdict.get(("Named_Snaps", r), None)
+        url1 = urlsdict.get((THUMB_LDIRS[0], r), None)
+        url2 = urlsdict.get((THUMB_LDIRS[1], r), None)
+        url3 = urlsdict.get((THUMB_LDIRS[2], r), None)
     else:
         url1 = None
         url2 = None
         url3 = None
     thumb_text = thumb_norm if short_names else thumb_name
     linked1 = link(url1, "🎴") if url1 else ""
     linked2 = link(url2, "🎬") if url2 else ""
@@ -1297,17 +1314,17 @@
             colors[k] = (128, 128, 128)
         else:
             # default transparent images, small enough to give primacy
             # to the others while still showing 'something missing'
             # size taken from the SNES snapshot default resolution
             imgs[k] = Image.new("RGBA", (256, 224), (255, 0, 0, 0))
             colors[k] = (0, 0, 0, 0)  # transparent 'border'
-    box = imgs.get("Named_Boxarts", None)
-    title = imgs.get("Named_Titles", None)
-    snap = imgs.get("Named_Snaps", None)
+    box = imgs.get(THUMB_LDIRS[0], None)
+    title = imgs.get(THUMB_LDIRS[1], None)
+    snap = imgs.get(THUMB_LDIRS[2], None)
     # we are trying to make a rectangle, where the left side has the boxart,
     # and the right side has the snap and title, stacked vertically.
     # the height of left and right will be the largest height on the
     # available thumbnails, except for the borders
     # (added after the resizes, so they look the same)
     wanted_box_y = max([i.size[1] for i in imgs.values()])
     x, y = box.size
@@ -1331,17 +1348,17 @@
     samex = wanted_y / (y1 / x1 + y2 / x2)
     new_y1 = max(1, round(y1 * samex / x1))
     new_y2 = max(1, round(y2 * samex / x2))
     samex = max(1, round(samex))
     title = title.resize((samex, new_y1))
     snap = snap.resize((samex, new_y2))
     # add borders
-    box = ImageOps.expand(box, border=(BORDER_SIZE,) * 4, fill=colors["Named_Boxarts"])
-    title = ImageOps.expand(title, border=(BORDER_SIZE,) * 4, fill=colors["Named_Titles"])
-    snap = ImageOps.expand(snap, border=(BORDER_SIZE,) * 4, fill=colors["Named_Snaps"])
+    box = ImageOps.expand(box, border=(BORDER_SIZE,) * 4, fill=colors[THUMB_LDIRS[0]])
+    title = ImageOps.expand(title, border=(BORDER_SIZE,) * 4, fill=colors[THUMB_LDIRS[1]])
+    snap = ImageOps.expand(snap, border=(BORDER_SIZE,) * 4, fill=colors[THUMB_LDIRS[2]])
     # create a 'paste' image
     combined = Image.new("RGBA", (box.size[0] + title.size[0], box.size[1]))
     combined.paste(box, box=(0, 0))
     combined.paste(title, box=(box.size[0], 0))
     combined.paste(snap, box=(box.size[0], title.size[1]))
     # save it, print TODO if a _good_ python sixtel library happens, replace this
     with io.BytesIO() as f:
```

### Comparing `libretrofuzz-3.3.3/pyproject.toml` & `libretrofuzz-3.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libretrofuzz"
-version = "3.3.3"
+version = "3.3.4"
 description = "Fuzzy Retroarch thumbnail downloader"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/i30817/libretrofuzz"
 
 [tool.poetry.dependencies]
```

### Comparing `libretrofuzz-3.3.3/setup.py` & `libretrofuzz-3.3.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 entry_points = \
 {'console_scripts': ['libretro-fuzz = libretrofuzz.__main__:fuzzsingle',
                      'libretro-fuzzall = libretrofuzz.__main__:fuzzall']}
 
 setup_kwargs = {
     'name': 'libretrofuzz',
-    'version': '3.3.3',
+    'version': '3.3.4',
     'description': 'Fuzzy Retroarch thumbnail downloader',
-    'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get a adequate default that is neither too strict or lax.\n\nIf you still want more thumbnails, using ``libretro-fuzz --min 80 --delay 15 --delay-after 15`` works (smaller ``--min`` increases fuzz), with some delays introduced to check if you want to keep the game selected for the thumbnails. If you prefer only exact matches, use ``--min 100``.\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --before '_'``\n\n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n\n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nA common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 90 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --before '_' --filter '[Ii]shar*'``\n\n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload because the glob used matches all names that start with 'Ishar' or 'ishar'.\n\nTo debug why a game is not being matched, SHORT=1 before the command will display the simplified names checked for similarity.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n\n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n\n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n\n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n\n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=60]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=60]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --min SCORE           | 0=any, 100≃equal, 90=default. No-op with ``--no-fail``.\n                        | [default: 90; 0<=x<=100]\n  --no-fail             Download any score. Equivalent to ``--min 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --dry-run             Print results only, no delay or image download.\n  --verbose N           | Show length N list: score, name, emoji hyperlinks.\n                        | [x>=1]\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
+    'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get a adequate default that is neither too strict or lax.\n\nIf you still want more thumbnails, using ``libretro-fuzz --min 80 --delay 15 --delay-after 15`` works (smaller ``--min`` increases fuzz), with some delays introduced to check if you want to keep the game selected for the thumbnails. If you prefer only exact matches, use ``--min 100``.\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --before '_'``\n\n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n\n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nA common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 90 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --before '_' --filter '[Ii]shar*'``\n\n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload because the glob used matches all names that start with 'Ishar' or 'ishar'.\n\nTo debug why a game is not being matched, SHORT=1 before the command will display the simplified names checked for similarity.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n\n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n\n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n\n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n\n  --playlist <NAME libretro-fuzz only>\n                        | Playlist name with labels used for thumbnail fuzzy matching.\n                        | If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        | Directory name in the server to download thumbnails.\n                        | If not provided, asked from the user.\n  --delay-after SECS    | Seconds after download to skip replacing thumbnails, enter continues.\n                        | No-op with ``--no-image``.\n                        | [1<=x<=60]\n  --delay SECS          | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=60]\n  --filter GLOB         | Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times.\n                        | Resets thumbnails, ``--filter '*'`` redownloads all.\n  --min SCORE           | 0=any, 100≃equal, 90=default. No-op with ``--no-fail``.\n                        | [default: 90; 0<=x<=100]\n  --no-fail             Download any score. Equivalent to ``--min 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            | Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls.\n                        | No-op with ``--filter``.\n  --no-meta             | Ignores () delimited metadata.\n                        | May cause false positives.\n                        | Forced with ``--before``.\n  --hack                | Matches [] delimited metadata, best used if the hack has thumbnails.\n                        | May cause false positives.\n                        | Ignored with ``--before``.\n  --before TEXT         | Use only the part of the label before TEXT to match.\n                        | TEXT may not be inside of brackets of any kind.\n                        | May cause false positives.\n                        | Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server, for local files:\n                        | Go to RA thumbnail dir/git clone/unzip packs;\n                        | Run ``'python3 -m http.server'`` in parent dir;\n                        | Then use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --dry-run             Print results only, no delay or image download.\n  --limit GAMES         | Show a number of winners or losers.\n                        | Any equal score winners can download images.\n                        | [default: 1; x>=1]\n  --verbose             Show failed matches.\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/libretrofuzz',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `libretrofuzz-3.3.3/PKG-INFO` & `libretrofuzz-3.3.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretrofuzz
-Version: 3.3.3
+Version: 3.3.4
 Summary: Fuzzy Retroarch thumbnail downloader
 Home-page: https://github.com/i30817/libretrofuzz
 License: MIT
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -77,35 +77,52 @@
                         Linux default:   ``~/.config/retroarch/retroarch.cfg``
 
                         Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``
 
                         MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``
 
   --playlist <NAME libretro-fuzz only>
-                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.
+                        | Playlist name with labels used for thumbnail fuzzy matching.
+                        | If not provided, asked from the user.
   --system <NAME libretro-fuzz only>
-                        Directory name in the server to download thumbnails. If not provided, asked from the user.
-  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.
+                        | Directory name in the server to download thumbnails.
+                        | If not provided, asked from the user.
+  --delay-after SECS    | Seconds after download to skip replacing thumbnails, enter continues.
+                        | No-op with ``--no-image``.
                         | [1<=x<=60]
-  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.
+  --delay SECS          | Seconds to skip thumbnails download, enter continues.
                         | [1<=x<=60]
-  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.
+  --filter GLOB         | Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times.
+                        | Resets thumbnails, ``--filter '*'`` redownloads all.
   --min SCORE           | 0=any, 100≃equal, 90=default. No-op with ``--no-fail``.
                         | [default: 90; 0<=x<=100]
   --no-fail             Download any score. Equivalent to ``--min 0``.
   --no-image            Don't show images even with chafa installed.
-  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.
-  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.
-  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.
-  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.
-  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.
+  --no-merge            | Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls.
+                        | No-op with ``--filter``.
+  --no-meta             | Ignores () delimited metadata.
+                        | May cause false positives.
+                        | Forced with ``--before``.
+  --hack                | Matches [] delimited metadata, best used if the hack has thumbnails.
+                        | May cause false positives.
+                        | Ignored with ``--before``.
+  --before TEXT         | Use only the part of the label before TEXT to match.
+                        | TEXT may not be inside of brackets of any kind.
+                        | May cause false positives.
+                        | Forces ignoring metadata.
+  --address URL         | URL with libretro-thumbnails server, for local files:
+                        | Go to RA thumbnail dir/git clone/unzip packs;
+                        | Run ``'python3 -m http.server'`` in parent dir;
+                        | Then use ``--address 'http://localhost:8000'``.
                         | [default: https://thumbnails.libretro.com]
   --dry-run             Print results only, no delay or image download.
-  --verbose N           | Show length N list: score, name, emoji hyperlinks.
-                        | [x>=1]
+  --limit GAMES         | Show a number of winners or losers.
+                        | Any equal score winners can download images.
+                        | [default: 1; x>=1]
+  --verbose             Show failed matches.
   --install-completion  Install completion for the current shell.
   --show-completion     Show completion for the current shell, to copy it or customize the installation.
   --help                Show this message and exit.
 
 
 
 To install the program, type on the cmd line
```


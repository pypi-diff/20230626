# Comparing `tmp/iciba-0.1.1.tar.gz` & `tmp/iciba-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iciba-0.1.1.tar", max compression
+gzip compressed data, was "iciba-0.1.2.tar", max compression
```

## Comparing `iciba-0.1.1.tar` & `iciba-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      516 2023-06-04 03:19:54.330629 iciba-0.1.1/README.md
--rw-r--r--   0        0        0        1 2023-06-04 03:00:04.274371 iciba-0.1.1/iciba/__init__.py
--rwxr-xr-x   0        0        0     3026 2023-06-04 03:11:38.414092 iciba-0.1.1/iciba/__main__.py
--rw-r--r--   0        0        0      531 2023-06-04 03:22:56.966479 iciba-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1358 1970-01-01 00:00:00.000000 iciba-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      516 2023-06-26 11:24:18.190549 iciba-0.1.2/README.md
+-rw-r--r--   0        0        0        1 2023-06-26 11:24:18.190549 iciba-0.1.2/iciba/__init__.py
+-rwxr-xr-x   0        0        0     3232 2023-06-26 11:31:31.492533 iciba-0.1.2/iciba/__main__.py
+-rw-r--r--   0        0        0      531 2023-06-26 11:31:59.262586 iciba-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1358 1970-01-01 00:00:00.000000 iciba-0.1.2/PKG-INFO
```

### Comparing `iciba-0.1.1/README.md` & `iciba-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `iciba-0.1.1/iciba/__main__.py` & `iciba-0.1.2/iciba/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,56 +6,70 @@
 from prompt_toolkit.document import Document
 from rich.console import Console
 from prompt_toolkit import prompt
 import json
 
 c = Console()
 
+
 class WordCompleter(Completer):
-    def get_completions(self, document: Document, complete_event: CompleteEvent) -> Iterable[Completion]:
+    def get_completions(
+        self, document: Document, complete_event: CompleteEvent
+    ) -> Iterable[Completion]:
         if len(document.text) <= 1:
             return []
-        url = "http://dict.iciba.com/dictionary/word/suggestion?word=%s&nums=5" % document.text
+        url = (
+            "http://dict.iciba.com/dictionary/word/suggestion?word=%s&nums=5"
+            % document.text
+        )
         try:
-            for w in httpx.get(url).json()['message']:
+            for w in httpx.get(url).json()["message"]:
                 yield Completion(w["key"], start_position=-len(document.text))
         except:
             return []
-    
+
 
 def main():
     if len(sys.argv) < 2:
-        word = prompt("Word: ", completer=WordCompleter(), complete_in_thread=True, complete_while_typing=True)
+        word = prompt(
+            "Word: ",
+            completer=WordCompleter(),
+            complete_in_thread=True,
+            complete_while_typing=True,
+        )
     elif len(sys.argv) > 2:
-        c.print("[cyan]Usage: [/cyan] main.py <word>") 
+        c.print("[cyan]Usage: [/cyan] main.py <word>")
         return
     else:
         word = sys.argv[1]
 
-    
-
-    url = "http://www.iciba.com/word?w=" + word
+    url = "https://www.iciba.com/word?w=" + word
 
     with c.status("Querying for '%s'..." % word):
-        resp = httpx.get(url, headers={
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/113.0"
-        })
+        resp = httpx.get(
+            url,
+            headers={
+                "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/113.0"
+            },
+        )
         data = resp.text.split("</script></body></html>")[0]
         data = data.split('<script id="__NEXT_DATA__" type="application/json">')[1]
-        data = json.loads(data)["props"]["pageProps"]["initialReduxState"]["word"]["wordInfo"]
+        data = json.loads(data)["props"]["pageProps"]["initialReduxState"]["word"][
+            "wordInfo"
+        ]
         # c.print(data)
 
     try:
         s = data["baesInfo"]["symbols"][0]
     except KeyError:
         c.print("[red]Word not found[/red]")
         exit(1)
 
     ph = s["ph_en"]
-    if len(s["ph_am"]) > 0: 
+    if len(s["ph_am"]) > 0:
         ph = s["ph_am"]
     if len(s["ph_other"]) > 0:
         ph = s["ph_other"]
     c.print(data["baesInfo"]["word_name"], "[i]" + ph + "[/i]")
 
     meanings = "\n[bold]= Meanings: [/bold] \n"
 
@@ -68,28 +82,32 @@
 
     synonyms = "[bold]= Synonyms: [/bold] \n"
 
     if "synonym" in data:
         for synonym in data["synonym"]:
             for m in synonym["means"]:
                 if len(synonym["part_name"]) > 0:
-                    synonyms += "[cyan][bold]" + synonym["part_name"] + "[/cyan][/bold] "
+                    synonyms += (
+                        "[cyan][bold]" + synonym["part_name"] + "[/cyan][/bold] "
+                    )
                 synonyms += m["word_mean"] + "\n"
                 synonyms += ", ".join(m["cis"])
                 synonyms += "\n"
-        
+
         c.print(synonyms)
 
     c.print("[bold]= Other forms: [/bold][i]" + ", ".join(data["exchanges"]) + "[/i]")
 
+
 def start():
     try:
         main()
     except KeyboardInterrupt:
         c.print("[yellow]User Interrupt[/yellow]")
     except EOFError:
         pass
     except Exception:
         c.print_exception()
 
+
 if __name__ == "__main__":
     start()
```

### Comparing `iciba-0.1.1/pyproject.toml` & `iciba-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "iciba"
-version = "0.1.1"
+version = "0.1.2"
 description = "A cli query tool for iciba.com (金山词霸)"
 authors = ["He <li@imlihe.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/lihe07/iciba"
 keywords = ["cli", "dictionary", "iciba", "translate"]
```

### Comparing `iciba-0.1.1/PKG-INFO` & `iciba-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iciba
-Version: 0.1.1
+Version: 0.1.2
 Summary: A cli query tool for iciba.com (金山词霸)
 Home-page: https://github.com/lihe07/iciba
 License: MIT
 Keywords: cli,dictionary,iciba,translate
 Author: He
 Author-email: li@imlihe.com
 Requires-Python: >=3.7.0
```


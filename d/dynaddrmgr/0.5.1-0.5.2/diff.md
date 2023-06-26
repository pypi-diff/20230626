# Comparing `tmp/dynaddrmgr-0.5.1.tar.gz` & `tmp/dynaddrmgr-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynaddrmgr-0.5.1.tar", max compression
+gzip compressed data, was "dynaddrmgr-0.5.2.tar", max compression
```

## Comparing `dynaddrmgr-0.5.1.tar` & `dynaddrmgr-0.5.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1097 2023-01-15 15:37:55.155474 dynaddrmgr-0.5.1/LICENSE
--rw-r--r--   0        0        0     1606 2023-02-09 13:27:57.592714 dynaddrmgr-0.5.1/README.md
--rw-r--r--   0        0        0       59 2023-06-23 19:50:27.588565 dynaddrmgr-0.5.1/dynaddrmgr/__init__.py
--rw-r--r--   0        0        0     5156 2023-06-23 19:50:27.588565 dynaddrmgr-0.5.1/dynaddrmgr/app.py
--rw-r--r--   0        0        0     3885 2023-01-23 13:03:17.636247 dynaddrmgr-0.5.1/dynaddrmgr/dynhost.py
--rw-r--r--   0        0        0     2401 2023-06-19 17:51:53.034497 dynaddrmgr-0.5.1/dynaddrmgr/dynrules.py
--rw-r--r--   0        0        0     2189 2023-06-19 17:51:53.034497 dynaddrmgr-0.5.1/dynaddrmgr/dyntmpls.py
--rw-r--r--   0        0        0      655 2023-06-19 17:51:53.034497 dynaddrmgr-0.5.1/dynaddrmgr/foos.py
--rw-r--r--   0        0        0     5070 2023-01-23 13:03:17.636247 dynaddrmgr-0.5.1/dynaddrmgr/fwhdlr.py
--rw-r--r--   0        0        0      294 2023-01-23 13:03:17.636247 dynaddrmgr-0.5.1/dynaddrmgr/kinds.py
--rw-r--r--   0        0        0        0 2023-01-23 13:03:17.636247 dynaddrmgr-0.5.1/dynaddrmgr/py.typed
--rw-r--r--   0        0        0     3850 2023-01-23 13:03:17.636247 dynaddrmgr-0.5.1/dynaddrmgr/rule.py
--rw-r--r--   0        0        0     4256 2023-06-19 17:51:53.038497 dynaddrmgr-0.5.1/dynaddrmgr/tmplmgr.py
--rw-r--r--   0        0        0     8661 2023-01-23 13:03:17.636247 dynaddrmgr-0.5.1/dynaddrmgr/ufw.py
--rw-r--r--   0        0        0     1480 2023-06-23 19:50:27.588565 dynaddrmgr-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2594 1970-01-01 00:00:00.000000 dynaddrmgr-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-01-15 15:37:55.155474 dynaddrmgr-0.5.2/LICENSE
+-rw-r--r--   0        0        0     1606 2023-02-09 13:27:57.592714 dynaddrmgr-0.5.2/README.md
+-rw-r--r--   0        0        0       59 2023-06-26 17:42:33.028641 dynaddrmgr-0.5.2/dynaddrmgr/__init__.py
+-rw-r--r--   0        0        0     6210 2023-06-26 17:42:33.028641 dynaddrmgr-0.5.2/dynaddrmgr/app.py
+-rw-r--r--   0        0        0     3885 2023-01-23 13:03:17.636247 dynaddrmgr-0.5.2/dynaddrmgr/dynhost.py
+-rw-r--r--   0        0        0     2401 2023-06-19 17:51:53.034497 dynaddrmgr-0.5.2/dynaddrmgr/dynrules.py
+-rw-r--r--   0        0        0     2189 2023-06-19 17:51:53.034497 dynaddrmgr-0.5.2/dynaddrmgr/dyntmpls.py
+-rw-r--r--   0        0        0      655 2023-06-19 17:51:53.034497 dynaddrmgr-0.5.2/dynaddrmgr/foos.py
+-rw-r--r--   0        0        0     5070 2023-01-23 13:03:17.636247 dynaddrmgr-0.5.2/dynaddrmgr/fwhdlr.py
+-rw-r--r--   0        0        0      294 2023-01-23 13:03:17.636247 dynaddrmgr-0.5.2/dynaddrmgr/kinds.py
+-rw-r--r--   0        0        0        0 2023-01-23 13:03:17.636247 dynaddrmgr-0.5.2/dynaddrmgr/py.typed
+-rw-r--r--   0        0        0     3850 2023-01-23 13:03:17.636247 dynaddrmgr-0.5.2/dynaddrmgr/rule.py
+-rw-r--r--   0        0        0     4256 2023-06-19 17:51:53.038497 dynaddrmgr-0.5.2/dynaddrmgr/tmplmgr.py
+-rw-r--r--   0        0        0     8661 2023-01-23 13:03:17.636247 dynaddrmgr-0.5.2/dynaddrmgr/ufw.py
+-rw-r--r--   0        0        0     1654 2023-06-26 17:42:33.032641 dynaddrmgr-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2644 1970-01-01 00:00:00.000000 dynaddrmgr-0.5.2/PKG-INFO
```

### Comparing `dynaddrmgr-0.5.1/LICENSE` & `dynaddrmgr-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dynaddrmgr-0.5.1/README.md` & `dynaddrmgr-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `dynaddrmgr-0.5.1/dynaddrmgr/app.py` & `dynaddrmgr-0.5.2/dynaddrmgr/app.py`

 * *Files 25% similar despite different names*

```diff
@@ -118,59 +118,95 @@
         for ip in ips:
             if is_ipv6_address(ip):
                 converted.append(ipv6_to_netprefix(ip, prefix_len))
             else:
                 converted.append(ip)
         return tuple(converted)
 
-    def _lookup_host(  # noqa: WPS231
+    def _verify_lookup_answer(  # noqa: WPS211
         self,
         name: str,
-        ipv4: bool,
+        answer: List[str],
         ipv6: bool,
         ipv6net: int = 0,
+        minlen: int = 1,
     ) -> Tuple[str, ...]:
         """Retrun a unique list of IP source strings.
 
         Parameters
         ----------
         name : str
-            Host name
-        ipv4 : bool
-            Lookup ipv4 flag
+            Name of host looked up
+        answer : List[str}
+            List of ip address strings
         ipv6 : bool
             Lookup ipv6 flag
         ipv6net : int
             Prefix length if ipv6 addreses represent networks
+        minlen : int
+            Minimum number of addresses to accept
 
         Returns
         -------
         Tuple[str, ...]
             Unique list of IP source strings
 
         Raises
         ------
         DNSException
             If lookup failed
         """
+        if answer:
+            if len(answer) >= minlen:
+                first_set = set(answer)
+                if ipv6 and ipv6net:
+                    return self._six_to_net(ipv6net, list(first_set))
+                return tuple(first_set)
+            raise DNSException(  # type: ignore [no-untyped-call]
+                "'{0}' name expected {1} addresses.!!!".format(name, minlen),
+            )
+        raise DNSException(  # type: ignore [no-untyped-call]
+            "'{0}' name not found.!!!".format(name),
+        )
+
+    def _lookup_host(
+        self,
+        name: str,
+        ipv4: bool,
+        ipv6: bool,
+        ipv6net: int = 0,
+    ) -> Tuple[str, ...]:
+        """Retrun a unique list of IP source strings.
+
+        Parameters
+        ----------
+        name : str
+            Host name
+        ipv4 : bool
+            Lookup ipv4 flag
+        ipv6 : bool
+            Lookup ipv6 flag
+        ipv6net : int
+            Prefix length if ipv6 addreses represent networks
+
+        Returns
+        -------
+        Tuple[str, ...]
+            Unique list of IP source strings
+        """
         ips: DNSresponse
+        minlen: int = 1
         if ipv4 and ipv6:
             ips = self.dns.dns_lookup_all(name)
+            minlen = 2
         elif ipv4:
             ips = self.dns.dns_lookup(name)
         elif ipv6:
             ips = self.dns.dns_lookup6(name)
-        if ips.answer:
-            first_set = set(ips.answer)
-            if ipv6net and ipv6:
-                return self._six_to_net(ipv6net, list(first_set))
-            return tuple(first_set)
-        raise DNSException(  # type: ignore [no-untyped-call]
-            "'{0}' name not found.!!!".format(name),
-        )
+        return self._verify_lookup_answer(name, ips.answer, ipv6, ipv6net, minlen)
 
     def _run_command(
         self,
         args: Tuple[str, ...],
         **kwargs,
     ) -> WtfProcessResult:
         """Runs commands specified by args."""
```

### Comparing `dynaddrmgr-0.5.1/dynaddrmgr/dynhost.py` & `dynaddrmgr-0.5.2/dynaddrmgr/dynhost.py`

 * *Files identical despite different names*

### Comparing `dynaddrmgr-0.5.1/dynaddrmgr/dynrules.py` & `dynaddrmgr-0.5.2/dynaddrmgr/dynrules.py`

 * *Files identical despite different names*

### Comparing `dynaddrmgr-0.5.1/dynaddrmgr/dyntmpls.py` & `dynaddrmgr-0.5.2/dynaddrmgr/dyntmpls.py`

 * *Files identical despite different names*

### Comparing `dynaddrmgr-0.5.1/dynaddrmgr/foos.py` & `dynaddrmgr-0.5.2/dynaddrmgr/foos.py`

 * *Files identical despite different names*

### Comparing `dynaddrmgr-0.5.1/dynaddrmgr/fwhdlr.py` & `dynaddrmgr-0.5.2/dynaddrmgr/fwhdlr.py`

 * *Files identical despite different names*

### Comparing `dynaddrmgr-0.5.1/dynaddrmgr/rule.py` & `dynaddrmgr-0.5.2/dynaddrmgr/rule.py`

 * *Files identical despite different names*

### Comparing `dynaddrmgr-0.5.1/dynaddrmgr/tmplmgr.py` & `dynaddrmgr-0.5.2/dynaddrmgr/tmplmgr.py`

 * *Files identical despite different names*

### Comparing `dynaddrmgr-0.5.1/dynaddrmgr/ufw.py` & `dynaddrmgr-0.5.2/dynaddrmgr/ufw.py`

 * *Files identical despite different names*

### Comparing `dynaddrmgr-0.5.1/pyproject.toml` & `dynaddrmgr-0.5.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "dynaddrmgr"
 description = "Tools to manage actions based on dynamic host address changes."
-version = "0.5.1"
+version = "0.5.2"
 license = "MIT"
 
 authors = [
   "Quien Sabe <qs5779@mail.com>",
 ]
 
 readme = "README.md"
@@ -15,14 +15,18 @@
 keywords = []
 
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Libraries :: Python Modules",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.scripts]
 dyntmplmgr = "dynaddrmgr.dyntmpls:main"
 dynfwrules = "dynaddrmgr.dynrules:main"
 
 [tool.poetry.dependencies]
```

### Comparing `dynaddrmgr-0.5.1/PKG-INFO` & `dynaddrmgr-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: dynaddrmgr
-Version: 0.5.1
+Version: 0.5.2
 Summary: Tools to manage actions based on dynamic host address changes.
 Home-page: https://github.com/wtfo-guru/dynaddrmgr
 License: MIT
 Author: Quien Sabe
 Author-email: qs5779@mail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: click (>=8.1.0,<9.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: nslookup (>=1.7.0,<2.0.0)
 Requires-Dist: wtforglib (>=0.8.2)
 Project-URL: Repository, https://github.com/wtfo-guru/dynaddrmgr
 Description-Content-Type: text/markdown
```


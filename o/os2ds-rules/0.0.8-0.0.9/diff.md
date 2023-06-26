# Comparing `tmp/os2ds-rules-0.0.8.tar.gz` & `tmp/os2ds-rules-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os2ds-rules-0.0.8.tar", last modified: Wed May 24 11:10:23 2023, max compression
+gzip compressed data, was "os2ds-rules-0.0.9.tar", last modified: Mon Jun 26 08:02:13 2023, max compression
```

## Comparing `os2ds-rules-0.0.8.tar` & `os2ds-rules-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:10:23.614684 os2ds-rules-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    25239 2023-05-24 11:10:23.614684 os2ds-rules-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:10:23.610684 os2ds-rules-0.0.8/include/
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/include/cpr-detector.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:10:23.610684 os2ds-rules-0.0.8/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/lib/address_rule.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     8816 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/lib/cpr-detector.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/lib/name_rule.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/lib/wordlist_rule.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 11:10:23.614684 os2ds-rules-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:10:23.610684 os2ds-rules-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:10:23.610684 os2ds-rules-0.0.8/src/os2ds_rules/
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/src/os2ds_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/src/os2ds_rules/address_rule.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/src/os2ds_rules/cpr.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/src/os2ds_rules/name_rule.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-05-24 11:10:13.000000 os2ds-rules-0.0.8/src/os2ds_rules/wordlist_rule.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 11:10:23.614684 os2ds-rules-0.0.8/src/os2ds_rules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25239 2023-05-24 11:10:23.000000 os2ds-rules-0.0.8/src/os2ds_rules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-24 11:10:23.000000 os2ds-rules-0.0.8/src/os2ds_rules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 11:10:23.000000 os2ds-rules-0.0.8/src/os2ds_rules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 11:10:23.000000 os2ds-rules-0.0.8/src/os2ds_rules.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:02:13.278809 os2ds-rules-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-26 08:02:05.000000 os2ds-rules-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-26 08:02:05.000000 os2ds-rules-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    25239 2023-06-26 08:02:13.278809 os2ds-rules-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5056 2023-06-26 08:02:05.000000 os2ds-rules-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:02:13.274809 os2ds-rules-0.0.9/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-06-26 08:02:05.000000 os2ds-rules-0.0.9/include/cpr-detector.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:02:13.274809 os2ds-rules-0.0.9/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-26 08:02:05.000000 os2ds-rules-0.0.9/lib/address_rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-06-26 08:02:05.000000 os2ds-rules-0.0.9/lib/cpr-detector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-06-26 08:02:05.000000 os2ds-rules-0.0.9/lib/name_rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-26 08:02:05.000000 os2ds-rules-0.0.9/lib/wordlist_rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-26 08:02:05.000000 os2ds-rules-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 08:02:13.278809 os2ds-rules-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-26 08:02:05.000000 os2ds-rules-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:02:13.274809 os2ds-rules-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:02:13.274809 os2ds-rules-0.0.9/src/os2ds_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-26 08:02:05.000000 os2ds-rules-0.0.9/src/os2ds_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-26 08:02:05.000000 os2ds-rules-0.0.9/src/os2ds_rules/address_rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-26 08:02:05.000000 os2ds-rules-0.0.9/src/os2ds_rules/cpr.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-26 08:02:05.000000 os2ds-rules-0.0.9/src/os2ds_rules/name_rule.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-06-26 08:02:05.000000 os2ds-rules-0.0.9/src/os2ds_rules/wordlist_rule.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 08:02:13.278809 os2ds-rules-0.0.9/src/os2ds_rules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25239 2023-06-26 08:02:13.000000 os2ds-rules-0.0.9/src/os2ds_rules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-26 08:02:13.000000 os2ds-rules-0.0.9/src/os2ds_rules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 08:02:13.000000 os2ds-rules-0.0.9/src/os2ds_rules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 08:02:13.000000 os2ds-rules-0.0.9/src/os2ds_rules.egg-info/top_level.txt
```

### Comparing `os2ds-rules-0.0.8/LICENSE` & `os2ds-rules-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.8/PKG-INFO` & `os2ds-rules-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os2ds-rules
-Version: 0.0.8
+Version: 0.0.9
 Summary: Text processing tool for detecting Danish CPR-numbers.
 Author-email: HackTheOxidation <tomas.hagenau@protonmail.ch>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

### Comparing `os2ds-rules-0.0.8/README.md` & `os2ds-rules-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.8/include/cpr-detector.hpp` & `os2ds-rules-0.0.9/include/cpr-detector.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 
 constexpr bool is_nonzero_digit(char c) noexcept { return '0' < c && c <= '9'; }
 
 constexpr bool is_digit(char c) noexcept { return '0' <= c && c <= '9'; }
 
 const auto is_separator = make_predicate(' ', '-', '/', '\t');
 
-const auto is_previous_ok = make_predicate(char(0), ' ', '.', ',', '\n', '\t', '\0');
+const auto is_previous_ok =
+    make_predicate(char(0), ' ', '.', ',', '\n', '\t', '\0');
 
 constexpr bool is_space(const char c) noexcept { return c == ' '; }
 
 static constexpr std::array<int, 10> modulus11_factors = {4, 3, 2, 7, 6,
                                                           5, 4, 3, 2, 1};
 
 class CPRDetector {
@@ -45,18 +46,19 @@
 
   bool check_mod11_;
   bool examine_context_;
   void reset(CPRDetectorState &state) noexcept;
   char update(char, CPRDetectorState, CPRDetectorState &, Predicate) noexcept;
   bool check_day_month(const std::string &, CPRDetectorState &) noexcept;
   void check_leap_year(const std::string &, CPRDetectorState &) noexcept;
-  void check_and_append_cpr(std::string &, MatchResults &, size_t,
-                            size_t) noexcept;
+  void check_and_append_cpr(std::string &, MatchResults &, size_t, size_t,
+                            char) noexcept;
   bool check_mod11(const MatchResult &) noexcept;
   bool examine_context(const std::string &) noexcept;
+  [[nodiscard]] std::string format_cpr(std::string &, char) const noexcept;
 
 public:
   constexpr CPRDetector(bool check_mod11 = false,
                         bool examine_context = false) noexcept
       : check_mod11_(check_mod11), examine_context_(examine_context) {}
 
   constexpr CPRDetector(const CPRDetector &) noexcept = default;
```

### Comparing `os2ds-rules-0.0.8/lib/address_rule.cpp` & `os2ds-rules-0.0.9/lib/address_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.8/lib/cpr-detector.cpp` & `os2ds-rules-0.0.9/lib/cpr-detector.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #include <algorithm>
 #include <array>
-#include <cstddef>
 #include <cctype>
+#include <cstddef>
 #include <iterator>
 #include <numeric>
 #include <string_view>
 
 #include <cpr-detector.hpp>
 #include <data_structures.hpp>
 
@@ -21,30 +21,32 @@
      "bilagsnummer", "order number", "ordrenummer", "fakturanummer", "faknr",
      "fak-nr", "tullstatistisk", "tullstatistik", "test report no",
      "protocol no.", "dhk:tx"});
 
 static const auto blacklist_words_set = FrozenHashSet(blacklist_words);
 }; // namespace
 
-static bool find_blacklisted_words(const std::string &content, const std::array<std::size_t, 4> indices) noexcept {
+static bool
+find_blacklisted_words(const std::string &content,
+                       const std::array<std::size_t, 4> indices) noexcept {
 
   for (std::size_t i = 1; i < 4; ++i) {
     for (std::size_t j = 0; j < i; ++j) {
       auto begin = indices[j];
       auto end = indices[i] - begin;
 
       if (end > content.size())
-	end = content.size() - begin - 1;
+        end = content.size() - begin - 1;
 
       std::string target = content.substr(begin, end);
       std::transform(target.begin(), target.end(), target.begin(),
                      [](unsigned char c) { return std::tolower(c); });
 
       if (blacklist_words_set.contains(target))
-	return true;
+        return true;
     }
   }
 
   return false;
 }
 
 void CPRDetector::reset(CPRDetectorState &state) noexcept {
@@ -100,22 +102,33 @@
   if (control < 4 && year == 0)
     reset(state);
 
   if (year % 4 != 0)
     reset(state);
 }
 
+std::string CPRDetector::format_cpr(std::string &cpr,
+                                    char separator = 0) const noexcept {
+  if (separator == 0) {
+    return cpr;
+  } else {
+    return std::string(cpr, 0, 6) + separator + std::string(cpr, 6, 4);
+  }
+}
+
 void CPRDetector::check_and_append_cpr(std::string &cpr, MatchResults &results,
-                                       size_t begin, size_t end) noexcept {
+                                       size_t begin, size_t end,
+                                       char separator = 0) noexcept {
   // Convert the 4 control digits to an int.
   int control = std::stoi(std::string(cpr, 6, 4));
 
   // We reject the control sequence '0000'.
   if (control > 0) {
-    MatchResult result(cpr, begin, end, CPRDetector::sensitivity);
+    MatchResult result(format_cpr(cpr, separator), begin, end,
+                       CPRDetector::sensitivity);
 
     if (check_mod11_ && !check_mod11(result))
       return;
 
     results.push_back(result);
   }
 }
@@ -142,19 +155,19 @@
   std::array<std::size_t, 4> indices = {0, 0, 0, 0};
 
   for (std::size_t i = 0; i < content.size(); ++i) {
     if (content[i] == ' ') {
       indices[4 - spaces] = i;
       --spaces;
       if (spaces == 0) {
-	if (find_blacklisted_words(content, indices))
-	  return true;
-	
-	spaces = 3;
-	indices[0] = indices[3] + 1;
+        if (find_blacklisted_words(content, indices))
+          return true;
+
+        spaces = 3;
+        indices[0] = indices[3] + 1;
       }
     }
   }
 
   if (find_blacklisted_words(content, indices))
     return true;
 
@@ -172,16 +185,17 @@
     return results;
   }
 
   // Initialize.
   CPRDetectorState state = CPRDetectorState::Empty;
   std::string cpr(10, 0);
   char previous = 0;
-  std::size_t count = 0;
+  char separator = 0;
   std::size_t begin = 0;
+  std::size_t end = 0;
   bool allow_separator, leap_year = false;
   Predicate is_acceptable = [](char) { return false; };
 
   for (auto it = std::begin(content); it != std::end(content); ++it) {
     switch (state) {
     case CPRDetectorState::Empty:
       if (!is_previous_ok(previous)) {
@@ -191,35 +205,34 @@
 
       is_acceptable = make_predicate('0', '1', '2', '3');
       update(*it, CPRDetectorState::First, state, is_acceptable);
       previous = *it;
 
       if (state == CPRDetectorState::First) {
         cpr[0] = *it;
-        begin = count;
+        begin =
+            static_cast<std::size_t>(std::distance(std::begin(content), it));
       }
 
       break;
     case CPRDetectorState::First:
       if (previous == '0') {
         is_acceptable = is_nonzero_digit;
       } else if (previous == '1' || previous == '2') {
         is_acceptable = is_digit;
       } else if (previous == '3') {
         is_acceptable = make_predicate('0', '1');
       } else {
         reset(state);
         previous = *it;
-        ++count;
         continue;
       }
 
       previous = cpr[1] =
           update(*it, CPRDetectorState::Second, state, is_acceptable);
-
       if (previous != 0)
         // Next time, we allow a space.
         allow_separator = true;
 
       break;
     case CPRDetectorState::Second:
       is_acceptable = make_predicate('0', '1');
@@ -231,15 +244,14 @@
       if (previous == '0') {
         is_acceptable = is_nonzero_digit;
       } else if (previous == '1') {
         is_acceptable = make_predicate('0', '1', '2');
       } else {
         reset(state);
         previous = 0;
-        ++count;
         continue;
       }
 
       previous = cpr[3] =
           update(*it, CPRDetectorState::Fourth, state, is_acceptable);
 
       leap_year = check_day_month(cpr, state);
@@ -270,16 +282,16 @@
         // Next time we allow one of the valid separators.
         allow_separator = true;
 
       break;
     case CPRDetectorState::Sixth:
       if (allow_separator && is_separator(*it)) {
         // Skip one of the valid separator characters.
+        separator = *it;
         allow_separator = false;
-	++count;
         continue;
       }
 
       is_acceptable = is_digit;
       previous = cpr[6] =
           update(*it, CPRDetectorState::Seventh, state, is_acceptable);
 
@@ -300,25 +312,24 @@
 
       break;
     case CPRDetectorState::Match:
       is_acceptable = is_digit;
       cpr[9] = update(*it, CPRDetectorState::Match, state, is_acceptable);
 
       auto ahead = it;
-      if (is_previous_ok(*(++ahead)))
-        check_and_append_cpr(cpr, results, begin, count);
-
+      if (is_previous_ok(*(++ahead))) {
+        end = static_cast<std::size_t>(std::distance(std::begin(content), it));
+        check_and_append_cpr(cpr, results, begin, end, separator);
+      }
       previous = *it;
       allow_separator = false;
       reset(state);
 
       break;
     }
-
-    ++count;
   }
 
   return results;
 }
 
 }; // namespace CPRDetector
 }; // namespace OS2DSRules
```

### Comparing `os2ds-rules-0.0.8/lib/name_rule.cpp` & `os2ds-rules-0.0.9/lib/name_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.8/lib/wordlist_rule.cpp` & `os2ds-rules-0.0.9/lib/wordlist_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.8/pyproject.toml` & `os2ds-rules-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "os2ds-rules"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="HackTheOxidation", email="tomas.hagenau@protonmail.ch" },
 ]
 description = "Text processing tool for detecting Danish CPR-numbers."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `os2ds-rules-0.0.8/setup.py` & `os2ds-rules-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.8/src/os2ds_rules/__init__.py` & `os2ds-rules-0.0.9/src/os2ds_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.8/src/os2ds_rules/address_rule.cpp` & `os2ds-rules-0.0.9/src/os2ds_rules/address_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.8/src/os2ds_rules/cpr.cpp` & `os2ds-rules-0.0.9/src/os2ds_rules/cpr.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.8/src/os2ds_rules/name_rule.cpp` & `os2ds-rules-0.0.9/src/os2ds_rules/name_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.8/src/os2ds_rules/wordlist_rule.cpp` & `os2ds-rules-0.0.9/src/os2ds_rules/wordlist_rule.cpp`

 * *Files identical despite different names*

### Comparing `os2ds-rules-0.0.8/src/os2ds_rules.egg-info/PKG-INFO` & `os2ds-rules-0.0.9/src/os2ds_rules.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os2ds-rules
-Version: 0.0.8
+Version: 0.0.9
 Summary: Text processing tool for detecting Danish CPR-numbers.
 Author-email: HackTheOxidation <tomas.hagenau@protonmail.ch>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```


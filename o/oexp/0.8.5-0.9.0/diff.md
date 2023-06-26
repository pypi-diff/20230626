# Comparing `tmp/oexp-0.8.5.tar.gz` & `tmp/oexp-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oexp-0.8.5.tar", last modified: Tue Jun 20 17:30:22 2023, max compression
+gzip compressed data, was "oexp-0.9.0.tar", last modified: Tue Jun 20 23:15:05 2023, max compression
```

## Comparing `oexp-0.8.5.tar` & `oexp-0.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 17:30:22.254590 oexp-0.8.5/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-20 17:30:22.254425 oexp-0.8.5/PKG-INFO
--r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.8.5/README.rst
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 17:30:22.253157 oexp-0.8.5/oexp/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      189 2023-06-20 15:09:33.000000 oexp-0.8.5/oexp/__init__.py
--r--r--r--   0 matthewgroth   (501) staff       (20)    81355 2023-06-20 17:25:07.000000 oexp-0.8.5/oexp/access.py
--r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-06-20 17:25:02.000000 oexp-0.8.5/oexp/gen.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     2042 2023-06-20 17:29:19.000000 oexp-0.8.5/oexp/jbridge.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 17:30:22.254230 oexp-0.8.5/oexp/util/
--rw-r--r--   0 matthewgroth   (501) staff       (20)        0 2023-06-10 17:43:13.000000 oexp-0.8.5/oexp/util/__init__.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     2650 2023-06-12 14:09:05.000000 oexp-0.8.5/oexp/util/ops.py
--rw-r--r--   0 matthewgroth   (501) staff       (20)     1612 2023-06-10 17:47:40.000000 oexp-0.8.5/oexp/util/vals.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 17:30:22.253838 oexp-0.8.5/oexp.egg-info/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-20 17:30:22.000000 oexp-0.8.5/oexp.egg-info/PKG-INFO
--rw-r--r--   0 matthewgroth   (501) staff       (20)      281 2023-06-20 17:30:22.000000 oexp-0.8.5/oexp.egg-info/SOURCES.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-06-20 17:30:22.000000 oexp-0.8.5/oexp.egg-info/dependency_links.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-06-20 17:30:22.000000 oexp-0.8.5/oexp.egg-info/requires.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-06-20 17:30:22.000000 oexp-0.8.5/oexp.egg-info/top_level.txt
--r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-06-20 17:30:17.000000 oexp-0.8.5/pyproject.toml
--rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-06-20 17:30:22.254674 oexp-0.8.5/setup.cfg
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 23:15:05.538425 oexp-0.9.0/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-20 23:15:05.538276 oexp-0.9.0/PKG-INFO
+-r--r--r--   0 matthewgroth   (501) staff       (20)       23 2023-04-04 21:36:40.000000 oexp-0.9.0/README.rst
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 23:15:05.537088 oexp-0.9.0/oexp/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      229 2023-06-20 23:12:58.000000 oexp-0.9.0/oexp/__init__.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)    87600 2023-06-20 23:01:14.000000 oexp-0.9.0/oexp/access.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)       44 2023-06-20 23:01:10.000000 oexp-0.9.0/oexp/gen.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     2010 2023-06-20 17:34:24.000000 oexp-0.9.0/oexp/jbridge.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 23:15:05.538125 oexp-0.9.0/oexp/util/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        0 2023-06-10 17:43:13.000000 oexp-0.9.0/oexp/util/__init__.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     2650 2023-06-12 14:09:05.000000 oexp-0.9.0/oexp/util/ops.py
+-rw-r--r--   0 matthewgroth   (501) staff       (20)     1612 2023-06-10 17:47:40.000000 oexp-0.9.0/oexp/util/vals.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-06-20 23:15:05.537760 oexp-0.9.0/oexp.egg-info/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      119 2023-06-20 23:15:05.000000 oexp-0.9.0/oexp.egg-info/PKG-INFO
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      281 2023-06-20 23:15:05.000000 oexp-0.9.0/oexp.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-06-20 23:15:05.000000 oexp-0.9.0/oexp.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       36 2023-06-20 23:15:05.000000 oexp-0.9.0/oexp.egg-info/requires.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        5 2023-06-20 23:15:05.000000 oexp-0.9.0/oexp.egg-info/top_level.txt
+-r--r--r--   0 matthewgroth   (501) staff       (20)      212 2023-06-20 23:15:00.000000 oexp-0.9.0/pyproject.toml
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-06-20 23:15:05.538468 oexp-0.9.0/setup.cfg
```

### Comparing `oexp-0.8.5/oexp/access.py` & `oexp-0.9.0/oexp/access.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     global _SAFE_PROCESS, _SAFE_THREAD
     if current_process().pid != _SAFE_PROCESS or current_thread().ident != _SAFE_THREAD:
         raise Exception(
             f"Python-Kotlin communication is currently not safe to use across multiple threads or processes. If you need this feature, please let me know."
         )
 
 
-JAR_URL = f"https://matt-central.s3.us-east-2.amazonaws.com//0/versioned/front/559/oexp-front-0-all.jar"
+JAR_URL = f"https://matt-central.s3.us-east-2.amazonaws.com//0/versioned/front/565/oexp-front-0-all.jar"
 
 
 class OexpExitSocketHeaders(Enum):
     EXIT = b"\x00"
 
 
 EXIT = b"\x00"
@@ -1307,59 +1307,14 @@
         return _recv_string(nullable=False)
 
     # [[matt.oexp.olang.lab.model.trial.Trial]]
     def to_dict(self):
         return json.loads(self.to_json())
 
 
-def encrypted_stimulus_path(cipher_path=NO_DEFAULT):
-    _check_required_parameters(**dict(cipher_path=cipher_path))
-    return EncryptedStimulusPath(cipher_path)
-
-
-# [[matt.oexp.olang.model.EncryptedStimulusPath]]
-class EncryptedStimulusPath(KBVClass):
-    def __init__(self, *args, _id=None):
-        _ensure_synchronized()
-        if _id is None:
-            jbridge._init_java()
-            _sendall(CREATE_OBJECT)
-            _send_string("matt.oexp.olang.model.EncryptedStimulusPath")
-            _send_string(args[0])
-            self._id = _object_id(_recv_long())
-        else:
-            self._id = _object_id(_id)
-
-    # [[matt.oexp.olang.model.EncryptedStimulusPath#cipherPath]]
-    @property
-    def cipher_path(self) -> str:
-        _ensure_synchronized()
-        _sendall(GET_VAL)
-        _send_long(self._id._id)
-        _send_int(0)
-        temp = _recv_string(nullable=False)
-        return temp
-
-    # [[matt.oexp.olang.model.EncryptedStimulusPath]]
-    def to_json(self):
-        _ensure_synchronized()
-        _sendall(GET_JSON)
-        _send_long(self._id._id)
-        return _recv_string(nullable=False)
-
-    # [[matt.oexp.olang.model.EncryptedStimulusPath]]
-    def to_dict(self):
-        return json.loads(self.to_json())
-
-    # [[matt.oexp.olang.model.EncryptedStimulusPath]]
-    def __eq__(self, other):
-        _ensure_synchronized()
-        return type(other) == type(self) and other.cipher_path == self.cipher_path
-
-
 # [[matt.oexp.olang.model.ExperimentEvent]]
 class ExperimentEvent(KBClass, abc.ABC):
     # [[matt.oexp.olang.model.ExperimentEvent#expUID]]
     @property
     @abc.abstractmethod
     def exp_uid(self) -> ExperimentUid:
         pass
@@ -1529,790 +1484,856 @@
             _send_long(self._id._id)
             _send_long(other._id._id)
             return _recv_bool()
         else:
             return False
 
 
-def experiment_uid(uid=NO_DEFAULT):
-    _check_required_parameters(**dict(uid=uid))
-    return ExperimentUid(uid)
+# [[matt.oexp.olang.model.TrialData]]
+class TrialData(ExperimentEvent, KBClass, abc.ABC):
+    # [[matt.oexp.olang.model.TrialData#log]]
+    @property
+    @abc.abstractmethod
+    def log(self) -> List[SubjectTrialEvent]:
+        pass
 
+    # [[matt.oexp.olang.model.TrialData#pid]]
+    @property
+    @abc.abstractmethod
+    def pid(self) -> ProlificParticipantUid:
+        pass
 
-# [[matt.oexp.olang.model.ExperimentUID]]
-class ExperimentUid(KBVClass):
+    # [[matt.oexp.olang.model.TrialData#response]]
+    @property
+    @abc.abstractmethod
+    def response(self) -> TrialResponse:
+        pass
+
+    # [[matt.oexp.olang.model.TrialData#sessionID]]
+    @property
+    @abc.abstractmethod
+    def session_id(self) -> ProlificSessionId:
+        pass
+
+    # [[matt.oexp.olang.model.TrialData#sessionNumber]]
+    @property
+    @abc.abstractmethod
+    def session_number(self) -> SessionNumber:
+        pass
+
+    # [[matt.oexp.olang.model.TrialData#startTimeUnixMillis]]
+    @property
+    @abc.abstractmethod
+    def start_time_unix_millis(self) -> int:
+        pass
+
+    # [[matt.oexp.olang.model.TrialData#stimuli]]
+    @property
+    @abc.abstractmethod
+    def stimuli(self) -> S:
+        pass
+
+    # [[matt.oexp.olang.model.TrialData#trialIndex]]
+    @property
+    @abc.abstractmethod
+    def trial_index(self) -> int:
+        pass
+
+    # [[matt.oexp.olang.model.TrialData#expUID]]
+    @property
+    @abc.abstractmethod
+    def exp_uid(self) -> ExperimentUid:
+        pass
+
+
+def completion_code(code=NO_DEFAULT, code_type=NO_DEFAULT, actions=NO_DEFAULT):
+    _check_required_parameters(**dict(code=code, code_type=code_type, actions=actions))
+    return CompletionCode(code, code_type, actions)
+
+
+# [[matt.oexp.olang.model.prolific.CompletionCode]]
+class CompletionCode(KBDClass):
     def __init__(self, *args, _id=None):
         _ensure_synchronized()
         if _id is None:
             jbridge._init_java()
             _sendall(CREATE_OBJECT)
-            _send_string("matt.oexp.olang.model.ExperimentUID")
-            _send_long(args[0])
+            _send_string("matt.oexp.olang.model.prolific.CompletionCode")
+            _send_string(args[0])
+            _send_string(args[1])
+            _send_int(len(args[2]))
+            for e in args[2]:
+                _send_int(len(e))
+                for k, v in e.items():
+                    _send_string(k)
+                    _send_string(v)
             self._id = _object_id(_recv_long())
         else:
             self._id = _object_id(_id)
 
-    # [[matt.oexp.olang.model.ExperimentUID#uid]]
+    # [[matt.oexp.olang.model.prolific.CompletionCode#actions]]
     @property
-    def uid(self) -> int:
+    def actions(self) -> List[Dict[str, str]]:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(0)
-        temp = _recv_long(nullable=False)
+        temp = _recv_list(
+            elementReceiveFun=lambda: _recv_map(
+                keyReceiveFun=lambda: _recv_string(nullable=False),
+                valueReceiveFun=lambda: _recv_string(nullable=False),
+                nullable=False,
+            ),
+            nullable=False,
+        )
+        return temp
+
+    # [[matt.oexp.olang.model.prolific.CompletionCode#code]]
+    @property
+    def code(self) -> str:
+        _ensure_synchronized()
+        _sendall(GET_VAL)
+        _send_long(self._id._id)
+        _send_int(1)
+        temp = _recv_string(nullable=False)
+        return temp
+
+    # [[matt.oexp.olang.model.prolific.CompletionCode#code_type]]
+    @property
+    def code_type(self) -> str:
+        _ensure_synchronized()
+        _sendall(GET_VAL)
+        _send_long(self._id._id)
+        _send_int(2)
+        temp = _recv_string(nullable=False)
         return temp
 
-    # [[matt.oexp.olang.model.ExperimentUID]]
+    # [[matt.oexp.olang.model.prolific.CompletionCode]]
     def to_json(self):
         _ensure_synchronized()
         _sendall(GET_JSON)
         _send_long(self._id._id)
         return _recv_string(nullable=False)
 
-    # [[matt.oexp.olang.model.ExperimentUID]]
+    # [[matt.oexp.olang.model.prolific.CompletionCode]]
     def to_dict(self):
         return json.loads(self.to_json())
 
-    # [[matt.oexp.olang.model.ExperimentUID]]
+    # [[matt.oexp.olang.model.prolific.CompletionCode]]
     def __eq__(self, other):
         _ensure_synchronized()
-        return type(other) == type(self) and other.uid == self.uid
+        if isinstance(other, KBClass):
+            _sendall(CHECK_EQUALITY)
+            _send_long(self._id._id)
+            _send_long(other._id._id)
+            return _recv_bool()
+        else:
+            return False
 
 
-def manifest_number(num=NO_DEFAULT):
-    _check_required_parameters(**dict(num=num))
-    return ManifestNumber(num)
+# [[matt.oexp.olang.model.prolific.CompletionOption]]
+class CompletionOption(Enum):
+    url = 0
+    code = 1
+    # [[matt.oexp.olang.model.prolific.CompletionOption]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
 
+    # [[matt.oexp.olang.model.prolific.CompletionOption]]
+    def to_dict(self):
+        return json.loads(self.to_json())
 
-# [[matt.oexp.olang.model.ManifestNumber]]
-class ManifestNumber(KBVClass):
+
+def prolific_study_data(
+    external_study_url=NO_DEFAULT,
+    completion_option=NO_DEFAULT,
+    completion_codes=NO_DEFAULT,
+):
+    _check_required_parameters(
+        **dict(
+            external_study_url=external_study_url,
+            completion_option=completion_option,
+            completion_codes=completion_codes,
+        )
+    )
+    return ProlificStudyData(external_study_url, completion_option, completion_codes)
+
+
+# [[matt.oexp.olang.model.prolific.ProlificStudyData]]
+class ProlificStudyData(KBDClass):
     def __init__(self, *args, _id=None):
         _ensure_synchronized()
         if _id is None:
             jbridge._init_java()
             _sendall(CREATE_OBJECT)
-            _send_string("matt.oexp.olang.model.ManifestNumber")
-            _send_int(args[0])
+            _send_string("matt.oexp.olang.model.prolific.ProlificStudyData")
+            _send_string(args[0])
+            _send_short(args[1].value)
+            _send_int(len(args[2]))
+            for e in args[2]:
+                _send_long(e._id._id)
             self._id = _object_id(_recv_long())
         else:
             self._id = _object_id(_id)
 
-    # [[matt.oexp.olang.model.ManifestNumber#num]]
+    # [[matt.oexp.olang.model.prolific.ProlificStudyData#completion_codes]]
     @property
-    def num(self) -> int:
+    def completion_codes(self) -> List[CompletionCode]:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(0)
-        temp = _recv_int(nullable=False)
+        temp = _recv_list(
+            elementReceiveFun=lambda: _recv_object(CompletionCode, nullable=False),
+            nullable=False,
+        )
+        return temp
+
+    # [[matt.oexp.olang.model.prolific.ProlificStudyData#completion_option]]
+    @property
+    def completion_option(self) -> CompletionOption:
+        _ensure_synchronized()
+        _sendall(GET_VAL)
+        _send_long(self._id._id)
+        _send_int(1)
+        temp = _recv_enum(CompletionOption, nullable=False)
+        return temp
+
+    # [[matt.oexp.olang.model.prolific.ProlificStudyData#external_study_url]]
+    @property
+    def external_study_url(self) -> str:
+        _ensure_synchronized()
+        _sendall(GET_VAL)
+        _send_long(self._id._id)
+        _send_int(2)
+        temp = _recv_string(nullable=False)
         return temp
 
-    # [[matt.oexp.olang.model.ManifestNumber]]
+    # [[matt.oexp.olang.model.prolific.ProlificStudyData]]
     def to_json(self):
         _ensure_synchronized()
         _sendall(GET_JSON)
         _send_long(self._id._id)
         return _recv_string(nullable=False)
 
-    # [[matt.oexp.olang.model.ManifestNumber]]
+    # [[matt.oexp.olang.model.prolific.ProlificStudyData]]
     def to_dict(self):
         return json.loads(self.to_json())
 
-    # [[matt.oexp.olang.model.ManifestNumber]]
+    # [[matt.oexp.olang.model.prolific.ProlificStudyData]]
     def __eq__(self, other):
         _ensure_synchronized()
-        return type(other) == type(self) and other.num == self.num
+        if isinstance(other, KBClass):
+            _sendall(CHECK_EQUALITY)
+            _send_long(self._id._id)
+            _send_long(other._id._id)
+            return _recv_bool()
+        else:
+            return False
 
 
-def prolific_participant_uid(pid=NO_DEFAULT):
-    _check_required_parameters(**dict(pid=pid))
-    return ProlificParticipantUid(pid)
+# [[matt.oexp.olang.model.response.TrialResponse]]
+class TrialResponse(KBClass, abc.ABC):
+    # [[matt.oexp.olang.model.response.TrialResponse]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
 
+    # [[matt.oexp.olang.model.response.TrialResponse]]
+    def to_dict(self):
+        return json.loads(self.to_json())
 
-# [[matt.oexp.olang.model.ProlificParticipantUid]]
-class ProlificParticipantUid(KBVClass):
+
+def encrypted_stimulus_path(cipher_path=NO_DEFAULT):
+    _check_required_parameters(**dict(cipher_path=cipher_path))
+    return EncryptedStimulusPath(cipher_path)
+
+
+# [[matt.oexp.olang.model.stim.EncryptedStimulusPath]]
+class EncryptedStimulusPath(KBVClass):
     def __init__(self, *args, _id=None):
         _ensure_synchronized()
         if _id is None:
             jbridge._init_java()
             _sendall(CREATE_OBJECT)
-            _send_string("matt.oexp.olang.model.ProlificParticipantUid")
+            _send_string("matt.oexp.olang.model.stim.EncryptedStimulusPath")
             _send_string(args[0])
             self._id = _object_id(_recv_long())
         else:
             self._id = _object_id(_id)
 
-    # [[matt.oexp.olang.model.ProlificParticipantUid#pid]]
+    # [[matt.oexp.olang.model.stim.EncryptedStimulusPath#cipherPath]]
     @property
-    def pid(self) -> str:
+    def cipher_path(self) -> str:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(0)
         temp = _recv_string(nullable=False)
         return temp
 
-    # [[matt.oexp.olang.model.ProlificParticipantUid#isPilot]]
-    def is_pilot(self) -> bool:
-        _ensure_synchronized()
-        _check_required_parameters(**dict())
-        _sendall(CALL_FUN)
-        _send_long(self._id._id)
-        _send_int(0)
-        _recv_exception_check()
-        return _recv_bool(nullable=False)
-
-    # [[matt.oexp.olang.model.ProlificParticipantUid#isTest]]
-    def is_test(self) -> bool:
-        _ensure_synchronized()
-        _check_required_parameters(**dict())
-        _sendall(CALL_FUN)
-        _send_long(self._id._id)
-        _send_int(1)
-        _recv_exception_check()
-        return _recv_bool(nullable=False)
-
-    # [[matt.oexp.olang.model.ProlificParticipantUid]]
+    # [[matt.oexp.olang.model.stim.EncryptedStimulusPath]]
     def to_json(self):
         _ensure_synchronized()
         _sendall(GET_JSON)
         _send_long(self._id._id)
         return _recv_string(nullable=False)
 
-    # [[matt.oexp.olang.model.ProlificParticipantUid]]
+    # [[matt.oexp.olang.model.stim.EncryptedStimulusPath]]
     def to_dict(self):
         return json.loads(self.to_json())
 
-    # [[matt.oexp.olang.model.ProlificParticipantUid]]
+    # [[matt.oexp.olang.model.stim.EncryptedStimulusPath]]
     def __eq__(self, other):
         _ensure_synchronized()
-        return type(other) == type(self) and other.pid == self.pid
+        return type(other) == type(self) and other.cipher_path == self.cipher_path
 
 
-def prolific_session_id(id=NO_DEFAULT):
-    _check_required_parameters(**dict(id=id))
-    return ProlificSessionId(id)
+def temporary_encrypted_stimulus(path=NO_DEFAULT, temp_url=NO_DEFAULT):
+    _check_required_parameters(**dict(path=path, temp_url=temp_url))
+    return TemporaryEncryptedStimulus(path, temp_url)
 
 
-# [[matt.oexp.olang.model.ProlificSessionId]]
-class ProlificSessionId(KBVClass):
+# [[matt.oexp.olang.model.stim.TemporaryEncryptedStimulus]]
+class TemporaryEncryptedStimulus(KBClass):
     def __init__(self, *args, _id=None):
         _ensure_synchronized()
         if _id is None:
             jbridge._init_java()
             _sendall(CREATE_OBJECT)
-            _send_string("matt.oexp.olang.model.ProlificSessionId")
-            _send_string(args[0])
+            _send_string("matt.oexp.olang.model.stim.TemporaryEncryptedStimulus")
+            _send_long(args[0]._id._id)
+            _send_string(args[1])
             self._id = _object_id(_recv_long())
         else:
             self._id = _object_id(_id)
 
-    # [[matt.oexp.olang.model.ProlificSessionId#id]]
+    # [[matt.oexp.olang.model.stim.TemporaryEncryptedStimulus#path]]
     @property
-    def id(self) -> str:
+    def path(self) -> EncryptedStimulusPath:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(0)
-        temp = _recv_string(nullable=False)
+        temp = _recv_object(EncryptedStimulusPath, nullable=False)
         return temp
 
-    # [[matt.oexp.olang.model.ProlificSessionId#isPilot]]
-    def is_pilot(self) -> bool:
+    # [[matt.oexp.olang.model.stim.TemporaryEncryptedStimulus#tempURL]]
+    @property
+    def temp_url(self) -> str:
         _ensure_synchronized()
-        _check_required_parameters(**dict())
-        _sendall(CALL_FUN)
+        _sendall(GET_VAL)
         _send_long(self._id._id)
-        _send_int(0)
-        _recv_exception_check()
-        return _recv_bool(nullable=False)
+        _send_int(1)
+        temp = _recv_string(nullable=False)
+        return temp
 
-    # [[matt.oexp.olang.model.ProlificSessionId#isTest]]
-    def is_test(self) -> bool:
+    # [[matt.oexp.olang.model.stim.TemporaryEncryptedStimulus#url]]
+    @property
+    def url(self) -> str:
         _ensure_synchronized()
-        _check_required_parameters(**dict())
-        _sendall(CALL_FUN)
+        _sendall(GET_VAL)
         _send_long(self._id._id)
-        _send_int(1)
-        _recv_exception_check()
-        return _recv_bool(nullable=False)
+        _send_int(2)
+        temp = _recv_string(nullable=False)
+        return temp
 
-    # [[matt.oexp.olang.model.ProlificSessionId]]
+    # [[matt.oexp.olang.model.stim.TemporaryEncryptedStimulus]]
     def to_json(self):
         _ensure_synchronized()
         _sendall(GET_JSON)
         _send_long(self._id._id)
         return _recv_string(nullable=False)
 
-    # [[matt.oexp.olang.model.ProlificSessionId]]
+    # [[matt.oexp.olang.model.stim.TemporaryEncryptedStimulus]]
     def to_dict(self):
         return json.loads(self.to_json())
 
-    # [[matt.oexp.olang.model.ProlificSessionId]]
+    # [[matt.oexp.olang.model.stim.TemporaryEncryptedStimulus]]
     def __eq__(self, other):
         _ensure_synchronized()
-        return type(other) == type(self) and other.id == self.id
+        if isinstance(other, KBClass):
+            _sendall(CHECK_EQUALITY)
+            _send_long(self._id._id)
+            _send_long(other._id._id)
+            return _recv_bool()
+        else:
+            return False
 
 
-def prolific_study_id(id=NO_DEFAULT):
-    _check_required_parameters(**dict(id=id))
-    return ProlificStudyId(id)
+# [[matt.oexp.olang.model.stim.TrialStimuli]]
+class TrialStimuli(KBClass, abc.ABC):
+    # [[matt.oexp.olang.model.stim.TrialStimuli]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
 
+    # [[matt.oexp.olang.model.stim.TrialStimuli]]
+    def to_dict(self):
+        return json.loads(self.to_json())
 
-# [[matt.oexp.olang.model.ProlificStudyID]]
-class ProlificStudyId(KBVClass):
+
+# [[matt.oexp.olang.model.trialevent.SubjectTrialEvent]]
+class SubjectTrialEvent(KBClass, abc.ABC):
+    # [[matt.oexp.olang.model.trialevent.SubjectTrialEvent#timeMillis]]
+    @property
+    @abc.abstractmethod
+    def time_millis(self) -> int:
+        pass
+
+    # [[matt.oexp.olang.model.trialevent.SubjectTrialEvent]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.model.trialevent.SubjectTrialEvent]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+
+def experiment_uid(uid=NO_DEFAULT):
+    _check_required_parameters(**dict(uid=uid))
+    return ExperimentUid(uid)
+
+
+# [[matt.oexp.olang.model.uid.ExperimentUID]]
+class ExperimentUid(KBVClass):
     def __init__(self, *args, _id=None):
         _ensure_synchronized()
         if _id is None:
             jbridge._init_java()
             _sendall(CREATE_OBJECT)
-            _send_string("matt.oexp.olang.model.ProlificStudyID")
-            _send_string(args[0])
+            _send_string("matt.oexp.olang.model.uid.ExperimentUID")
+            _send_long(args[0])
             self._id = _object_id(_recv_long())
         else:
             self._id = _object_id(_id)
 
-    # [[matt.oexp.olang.model.ProlificStudyID#id]]
+    # [[matt.oexp.olang.model.uid.ExperimentUID#uid]]
     @property
-    def id(self) -> str:
+    def uid(self) -> int:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(0)
-        temp = _recv_string(nullable=False)
+        temp = _recv_long(nullable=False)
         return temp
 
-    # [[matt.oexp.olang.model.ProlificStudyID]]
+    # [[matt.oexp.olang.model.uid.ExperimentUID]]
     def to_json(self):
         _ensure_synchronized()
         _sendall(GET_JSON)
         _send_long(self._id._id)
         return _recv_string(nullable=False)
 
-    # [[matt.oexp.olang.model.ProlificStudyID]]
+    # [[matt.oexp.olang.model.uid.ExperimentUID]]
     def to_dict(self):
         return json.loads(self.to_json())
 
-    # [[matt.oexp.olang.model.ProlificStudyID]]
+    # [[matt.oexp.olang.model.uid.ExperimentUID]]
     def __eq__(self, other):
         _ensure_synchronized()
-        return type(other) == type(self) and other.id == self.id
+        return type(other) == type(self) and other.uid == self.uid
 
 
-def session_number(num=NO_DEFAULT):
+def manifest_number(num=NO_DEFAULT):
     _check_required_parameters(**dict(num=num))
-    return SessionNumber(num)
+    return ManifestNumber(num)
 
 
-# [[matt.oexp.olang.model.SessionNumber]]
-class SessionNumber(KBVClass):
+# [[matt.oexp.olang.model.uid.ManifestNumber]]
+class ManifestNumber(KBVClass):
     def __init__(self, *args, _id=None):
         _ensure_synchronized()
         if _id is None:
             jbridge._init_java()
             _sendall(CREATE_OBJECT)
-            _send_string("matt.oexp.olang.model.SessionNumber")
-            _send_long(args[0])
+            _send_string("matt.oexp.olang.model.uid.ManifestNumber")
+            _send_int(args[0])
             self._id = _object_id(_recv_long())
         else:
             self._id = _object_id(_id)
 
-    # [[matt.oexp.olang.model.SessionNumber#num]]
+    # [[matt.oexp.olang.model.uid.ManifestNumber#num]]
     @property
     def num(self) -> int:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(0)
-        temp = _recv_long(nullable=False)
+        temp = _recv_int(nullable=False)
         return temp
 
-    # [[matt.oexp.olang.model.SessionNumber]]
+    # [[matt.oexp.olang.model.uid.ManifestNumber]]
     def to_json(self):
         _ensure_synchronized()
         _sendall(GET_JSON)
         _send_long(self._id._id)
         return _recv_string(nullable=False)
 
-    # [[matt.oexp.olang.model.SessionNumber]]
+    # [[matt.oexp.olang.model.uid.ManifestNumber]]
     def to_dict(self):
         return json.loads(self.to_json())
 
-    # [[matt.oexp.olang.model.SessionNumber]]
+    # [[matt.oexp.olang.model.uid.ManifestNumber]]
     def __eq__(self, other):
         _ensure_synchronized()
         return type(other) == type(self) and other.num == self.num
 
 
-# [[matt.oexp.olang.model.SubjectTrialEvent]]
-class SubjectTrialEvent(KBClass, abc.ABC):
-    # [[matt.oexp.olang.model.SubjectTrialEvent#timeMillis]]
-    @property
-    @abc.abstractmethod
-    def time_millis(self) -> int:
-        pass
-
-    # [[matt.oexp.olang.model.SubjectTrialEvent]]
-    def to_json(self):
-        _ensure_synchronized()
-        _sendall(GET_JSON)
-        _send_long(self._id._id)
-        return _recv_string(nullable=False)
-
-    # [[matt.oexp.olang.model.SubjectTrialEvent]]
-    def to_dict(self):
-        return json.loads(self.to_json())
-
-
-def temporary_encrypted_stimulus(path=NO_DEFAULT, temp_url=NO_DEFAULT):
-    _check_required_parameters(**dict(path=path, temp_url=temp_url))
-    return TemporaryEncryptedStimulus(path, temp_url)
+def prolific_participant_uid(pid=NO_DEFAULT):
+    _check_required_parameters(**dict(pid=pid))
+    return ProlificParticipantUid(pid)
 
 
-# [[matt.oexp.olang.model.TemporaryEncryptedStimulus]]
-class TemporaryEncryptedStimulus(KBClass):
+# [[matt.oexp.olang.model.uid.ProlificParticipantUid]]
+class ProlificParticipantUid(KBVClass):
     def __init__(self, *args, _id=None):
         _ensure_synchronized()
         if _id is None:
             jbridge._init_java()
             _sendall(CREATE_OBJECT)
-            _send_string("matt.oexp.olang.model.TemporaryEncryptedStimulus")
-            _send_long(args[0]._id._id)
-            _send_string(args[1])
+            _send_string("matt.oexp.olang.model.uid.ProlificParticipantUid")
+            _send_string(args[0])
             self._id = _object_id(_recv_long())
         else:
             self._id = _object_id(_id)
 
-    # [[matt.oexp.olang.model.TemporaryEncryptedStimulus#path]]
+    # [[matt.oexp.olang.model.uid.ProlificParticipantUid#pid]]
     @property
-    def path(self) -> EncryptedStimulusPath:
+    def pid(self) -> str:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(0)
-        temp = _recv_object(EncryptedStimulusPath, nullable=False)
+        temp = _recv_string(nullable=False)
         return temp
 
-    # [[matt.oexp.olang.model.TemporaryEncryptedStimulus#tempURL]]
-    @property
-    def temp_url(self) -> str:
+    # [[matt.oexp.olang.model.uid.ProlificParticipantUid#isPilot]]
+    def is_pilot(self) -> bool:
         _ensure_synchronized()
-        _sendall(GET_VAL)
+        _check_required_parameters(**dict())
+        _sendall(CALL_FUN)
         _send_long(self._id._id)
-        _send_int(1)
-        temp = _recv_string(nullable=False)
-        return temp
+        _send_int(0)
+        _recv_exception_check()
+        return _recv_bool(nullable=False)
 
-    # [[matt.oexp.olang.model.TemporaryEncryptedStimulus#url]]
-    @property
-    def url(self) -> str:
+    # [[matt.oexp.olang.model.uid.ProlificParticipantUid#isTest]]
+    def is_test(self) -> bool:
         _ensure_synchronized()
-        _sendall(GET_VAL)
+        _check_required_parameters(**dict())
+        _sendall(CALL_FUN)
         _send_long(self._id._id)
-        _send_int(2)
-        temp = _recv_string(nullable=False)
-        return temp
+        _send_int(1)
+        _recv_exception_check()
+        return _recv_bool(nullable=False)
 
-    # [[matt.oexp.olang.model.TemporaryEncryptedStimulus]]
+    # [[matt.oexp.olang.model.uid.ProlificParticipantUid]]
     def to_json(self):
         _ensure_synchronized()
         _sendall(GET_JSON)
         _send_long(self._id._id)
         return _recv_string(nullable=False)
 
-    # [[matt.oexp.olang.model.TemporaryEncryptedStimulus]]
+    # [[matt.oexp.olang.model.uid.ProlificParticipantUid]]
     def to_dict(self):
         return json.loads(self.to_json())
 
-    # [[matt.oexp.olang.model.TemporaryEncryptedStimulus]]
+    # [[matt.oexp.olang.model.uid.ProlificParticipantUid]]
     def __eq__(self, other):
         _ensure_synchronized()
-        if isinstance(other, KBClass):
-            _sendall(CHECK_EQUALITY)
-            _send_long(self._id._id)
-            _send_long(other._id._id)
-            return _recv_bool()
-        else:
-            return False
-
-
-# [[matt.oexp.olang.model.TrialData]]
-class TrialData(ExperimentEvent, KBClass, abc.ABC):
-    # [[matt.oexp.olang.model.TrialData#distractors]]
-    @property
-    @abc.abstractmethod
-    def distractors(self) -> List[S]:
-        pass
-
-    # [[matt.oexp.olang.model.TrialData#log]]
-    @property
-    @abc.abstractmethod
-    def log(self) -> List[SubjectTrialEvent]:
-        pass
-
-    # [[matt.oexp.olang.model.TrialData#pid]]
-    @property
-    @abc.abstractmethod
-    def pid(self) -> ProlificParticipantUid:
-        pass
-
-    # [[matt.oexp.olang.model.TrialData#selectionIndices]]
-    @property
-    @abc.abstractmethod
-    def selection_indices(self) -> List[int]:
-        pass
-
-    # [[matt.oexp.olang.model.TrialData#sessionID]]
-    @property
-    @abc.abstractmethod
-    def session_id(self) -> ProlificSessionId:
-        pass
-
-    # [[matt.oexp.olang.model.TrialData#sessionNumber]]
-    @property
-    @abc.abstractmethod
-    def session_number(self) -> SessionNumber:
-        pass
-
-    # [[matt.oexp.olang.model.TrialData#startTimeUnixMillis]]
-    @property
-    @abc.abstractmethod
-    def start_time_unix_millis(self) -> int:
-        pass
-
-    # [[matt.oexp.olang.model.TrialData#target]]
-    @property
-    @abc.abstractmethod
-    def target(self) -> S:
-        pass
-
-    @target.setter
-    @abc.abstractmethod
-    def target(self, value) -> S:
-        pass
-
-    # [[matt.oexp.olang.model.TrialData#trialIndex]]
-    @property
-    @abc.abstractmethod
-    def trial_index(self) -> int:
-        pass
-
-    # [[matt.oexp.olang.model.TrialData#expUID]]
-    @property
-    @abc.abstractmethod
-    def exp_uid(self) -> ExperimentUid:
-        pass
+        return type(other) == type(self) and other.pid == self.pid
 
 
-def completion_code(code=NO_DEFAULT, code_type=NO_DEFAULT, actions=NO_DEFAULT):
-    _check_required_parameters(**dict(code=code, code_type=code_type, actions=actions))
-    return CompletionCode(code, code_type, actions)
+def prolific_session_id(id=NO_DEFAULT):
+    _check_required_parameters(**dict(id=id))
+    return ProlificSessionId(id)
 
 
-# [[matt.oexp.olang.model.prolific.CompletionCode]]
-class CompletionCode(KBDClass):
+# [[matt.oexp.olang.model.uid.ProlificSessionId]]
+class ProlificSessionId(KBVClass):
     def __init__(self, *args, _id=None):
         _ensure_synchronized()
         if _id is None:
             jbridge._init_java()
             _sendall(CREATE_OBJECT)
-            _send_string("matt.oexp.olang.model.prolific.CompletionCode")
+            _send_string("matt.oexp.olang.model.uid.ProlificSessionId")
             _send_string(args[0])
-            _send_string(args[1])
-            _send_int(len(args[2]))
-            for e in args[2]:
-                _send_int(len(e))
-                for k, v in e.items():
-                    _send_string(k)
-                    _send_string(v)
             self._id = _object_id(_recv_long())
         else:
             self._id = _object_id(_id)
 
-    # [[matt.oexp.olang.model.prolific.CompletionCode#actions]]
+    # [[matt.oexp.olang.model.uid.ProlificSessionId#id]]
     @property
-    def actions(self) -> List[Dict[str, str]]:
+    def id(self) -> str:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(0)
-        temp = _recv_list(
-            elementReceiveFun=lambda: _recv_map(
-                keyReceiveFun=lambda: _recv_string(nullable=False),
-                valueReceiveFun=lambda: _recv_string(nullable=False),
-                nullable=False,
-            ),
-            nullable=False,
-        )
+        temp = _recv_string(nullable=False)
         return temp
 
-    # [[matt.oexp.olang.model.prolific.CompletionCode#code]]
-    @property
-    def code(self) -> str:
+    # [[matt.oexp.olang.model.uid.ProlificSessionId#isPilot]]
+    def is_pilot(self) -> bool:
         _ensure_synchronized()
-        _sendall(GET_VAL)
+        _check_required_parameters(**dict())
+        _sendall(CALL_FUN)
         _send_long(self._id._id)
-        _send_int(1)
-        temp = _recv_string(nullable=False)
-        return temp
+        _send_int(0)
+        _recv_exception_check()
+        return _recv_bool(nullable=False)
 
-    # [[matt.oexp.olang.model.prolific.CompletionCode#code_type]]
-    @property
-    def code_type(self) -> str:
+    # [[matt.oexp.olang.model.uid.ProlificSessionId#isTest]]
+    def is_test(self) -> bool:
         _ensure_synchronized()
-        _sendall(GET_VAL)
+        _check_required_parameters(**dict())
+        _sendall(CALL_FUN)
         _send_long(self._id._id)
-        _send_int(2)
-        temp = _recv_string(nullable=False)
-        return temp
+        _send_int(1)
+        _recv_exception_check()
+        return _recv_bool(nullable=False)
 
-    # [[matt.oexp.olang.model.prolific.CompletionCode]]
+    # [[matt.oexp.olang.model.uid.ProlificSessionId]]
     def to_json(self):
         _ensure_synchronized()
         _sendall(GET_JSON)
         _send_long(self._id._id)
         return _recv_string(nullable=False)
 
-    # [[matt.oexp.olang.model.prolific.CompletionCode]]
+    # [[matt.oexp.olang.model.uid.ProlificSessionId]]
     def to_dict(self):
         return json.loads(self.to_json())
 
-    # [[matt.oexp.olang.model.prolific.CompletionCode]]
+    # [[matt.oexp.olang.model.uid.ProlificSessionId]]
     def __eq__(self, other):
         _ensure_synchronized()
-        if isinstance(other, KBClass):
-            _sendall(CHECK_EQUALITY)
-            _send_long(self._id._id)
-            _send_long(other._id._id)
-            return _recv_bool()
+        return type(other) == type(self) and other.id == self.id
+
+
+def prolific_study_id(id=NO_DEFAULT):
+    _check_required_parameters(**dict(id=id))
+    return ProlificStudyId(id)
+
+
+# [[matt.oexp.olang.model.uid.ProlificStudyID]]
+class ProlificStudyId(KBVClass):
+    def __init__(self, *args, _id=None):
+        _ensure_synchronized()
+        if _id is None:
+            jbridge._init_java()
+            _sendall(CREATE_OBJECT)
+            _send_string("matt.oexp.olang.model.uid.ProlificStudyID")
+            _send_string(args[0])
+            self._id = _object_id(_recv_long())
         else:
-            return False
+            self._id = _object_id(_id)
 
+    # [[matt.oexp.olang.model.uid.ProlificStudyID#id]]
+    @property
+    def id(self) -> str:
+        _ensure_synchronized()
+        _sendall(GET_VAL)
+        _send_long(self._id._id)
+        _send_int(0)
+        temp = _recv_string(nullable=False)
+        return temp
 
-# [[matt.oexp.olang.model.prolific.CompletionOption]]
-class CompletionOption(Enum):
-    url = 0
-    code = 1
-    # [[matt.oexp.olang.model.prolific.CompletionOption]]
+    # [[matt.oexp.olang.model.uid.ProlificStudyID]]
     def to_json(self):
         _ensure_synchronized()
         _sendall(GET_JSON)
         _send_long(self._id._id)
         return _recv_string(nullable=False)
 
-    # [[matt.oexp.olang.model.prolific.CompletionOption]]
+    # [[matt.oexp.olang.model.uid.ProlificStudyID]]
     def to_dict(self):
         return json.loads(self.to_json())
 
+    # [[matt.oexp.olang.model.uid.ProlificStudyID]]
+    def __eq__(self, other):
+        _ensure_synchronized()
+        return type(other) == type(self) and other.id == self.id
 
-def prolific_study_data(
-    external_study_url=NO_DEFAULT,
-    completion_option=NO_DEFAULT,
-    completion_codes=NO_DEFAULT,
-):
-    _check_required_parameters(
-        **dict(
-            external_study_url=external_study_url,
-            completion_option=completion_option,
-            completion_codes=completion_codes,
-        )
-    )
-    return ProlificStudyData(external_study_url, completion_option, completion_codes)
+
+def session_number(num=NO_DEFAULT):
+    _check_required_parameters(**dict(num=num))
+    return SessionNumber(num)
 
 
-# [[matt.oexp.olang.model.prolific.ProlificStudyData]]
-class ProlificStudyData(KBDClass):
+# [[matt.oexp.olang.model.uid.SessionNumber]]
+class SessionNumber(KBVClass):
     def __init__(self, *args, _id=None):
         _ensure_synchronized()
         if _id is None:
             jbridge._init_java()
             _sendall(CREATE_OBJECT)
-            _send_string("matt.oexp.olang.model.prolific.ProlificStudyData")
-            _send_string(args[0])
-            _send_short(args[1].value)
-            _send_int(len(args[2]))
-            for e in args[2]:
-                _send_long(e._id._id)
+            _send_string("matt.oexp.olang.model.uid.SessionNumber")
+            _send_long(args[0])
             self._id = _object_id(_recv_long())
         else:
             self._id = _object_id(_id)
 
-    # [[matt.oexp.olang.model.prolific.ProlificStudyData#completion_codes]]
+    # [[matt.oexp.olang.model.uid.SessionNumber#num]]
     @property
-    def completion_codes(self) -> List[CompletionCode]:
+    def num(self) -> int:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(0)
-        temp = _recv_list(
-            elementReceiveFun=lambda: _recv_object(CompletionCode, nullable=False),
-            nullable=False,
-        )
-        return temp
-
-    # [[matt.oexp.olang.model.prolific.ProlificStudyData#completion_option]]
-    @property
-    def completion_option(self) -> CompletionOption:
-        _ensure_synchronized()
-        _sendall(GET_VAL)
-        _send_long(self._id._id)
-        _send_int(1)
-        temp = _recv_enum(CompletionOption, nullable=False)
-        return temp
-
-    # [[matt.oexp.olang.model.prolific.ProlificStudyData#external_study_url]]
-    @property
-    def external_study_url(self) -> str:
-        _ensure_synchronized()
-        _sendall(GET_VAL)
-        _send_long(self._id._id)
-        _send_int(2)
-        temp = _recv_string(nullable=False)
+        temp = _recv_long(nullable=False)
         return temp
 
-    # [[matt.oexp.olang.model.prolific.ProlificStudyData]]
+    # [[matt.oexp.olang.model.uid.SessionNumber]]
     def to_json(self):
         _ensure_synchronized()
         _sendall(GET_JSON)
         _send_long(self._id._id)
         return _recv_string(nullable=False)
 
-    # [[matt.oexp.olang.model.prolific.ProlificStudyData]]
+    # [[matt.oexp.olang.model.uid.SessionNumber]]
     def to_dict(self):
         return json.loads(self.to_json())
 
-    # [[matt.oexp.olang.model.prolific.ProlificStudyData]]
+    # [[matt.oexp.olang.model.uid.SessionNumber]]
     def __eq__(self, other):
         _ensure_synchronized()
-        if isinstance(other, KBClass):
-            _sendall(CHECK_EQUALITY)
-            _send_long(self._id._id)
-            _send_long(other._id._id)
-            return _recv_bool()
-        else:
-            return False
+        return type(other) == type(self) and other.num == self.num
 
 
-def gallery_trial(query=NO_DEFAULT, distractors=NO_DEFAULT):
-    _check_required_parameters(**dict(query=query, distractors=distractors))
-    return GalleryTrial(query, distractors)
+def choice_trial(image=NO_DEFAULT, choices=NO_DEFAULT):
+    _check_required_parameters(**dict(image=image, choices=choices))
+    return ChoiceTrial(image, choices)
 
 
-# [[matt.oexp.olang.lab.model.trial.GalleryTrial]]
-class GalleryTrial(Trial, KBDClass):
+# [[matt.oexp.olang.lab.model.trial.ChoiceTrial]]
+class ChoiceTrial(Trial, KBDClass):
     def __init__(self, *args, _id=None):
         _ensure_synchronized()
         if _id is None:
             jbridge._init_java()
             _sendall(CREATE_OBJECT)
-            _send_string("matt.oexp.olang.lab.model.trial.GalleryTrial")
+            _send_string("matt.oexp.olang.lab.model.trial.ChoiceTrial")
             _send_string(args[0])
             _send_int(len(args[1]))
             for e in args[1]:
                 _send_string(e)
             self._id = _object_id(_recv_long())
         else:
             self._id = _object_id(_id)
 
-    # [[matt.oexp.olang.lab.model.trial.GalleryTrial#distractors]]
+    # [[matt.oexp.olang.lab.model.trial.ChoiceTrial#choices]]
     @property
-    def distractors(self) -> List[str]:
+    def choices(self) -> List[str]:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(0)
         temp = _recv_list(
             elementReceiveFun=lambda: _recv_string(nullable=False), nullable=False
         )
         return temp
 
-    # [[matt.oexp.olang.lab.model.trial.GalleryTrial#query]]
+    # [[matt.oexp.olang.lab.model.trial.ChoiceTrial#image]]
     @property
-    def query(self) -> str:
+    def image(self) -> str:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(1)
         temp = _recv_string(nullable=False)
         return temp
 
-    # [[matt.oexp.olang.lab.model.trial.GalleryTrial]]
+    # [[matt.oexp.olang.lab.model.trial.ChoiceTrial]]
     def to_json(self):
         _ensure_synchronized()
         _sendall(GET_JSON)
         _send_long(self._id._id)
         return _recv_string(nullable=False)
 
-    # [[matt.oexp.olang.lab.model.trial.GalleryTrial]]
+    # [[matt.oexp.olang.lab.model.trial.ChoiceTrial]]
     def to_dict(self):
         return json.loads(self.to_json())
 
-    # [[matt.oexp.olang.lab.model.trial.GalleryTrial]]
+    # [[matt.oexp.olang.lab.model.trial.ChoiceTrial]]
     def __eq__(self, other):
         _ensure_synchronized()
         if isinstance(other, KBClass):
             _sendall(CHECK_EQUALITY)
             _send_long(self._id._id)
             _send_long(other._id._id)
             return _recv_bool()
         else:
             return False
 
 
-def button_event(time_millis=NO_DEFAULT, button=NO_DEFAULT):
-    _check_required_parameters(**dict(time_millis=time_millis, button=button))
-    return ButtonEvent(time_millis, button)
+def gallery_trial(query=NO_DEFAULT, distractors=NO_DEFAULT):
+    _check_required_parameters(**dict(query=query, distractors=distractors))
+    return GalleryTrial(query, distractors)
 
 
-# [[matt.oexp.olang.model.ButtonEvent]]
-class ButtonEvent(SubjectTrialEvent, KBClass):
+# [[matt.oexp.olang.lab.model.trial.GalleryTrial]]
+class GalleryTrial(Trial, KBDClass):
     def __init__(self, *args, _id=None):
         _ensure_synchronized()
         if _id is None:
             jbridge._init_java()
             _sendall(CREATE_OBJECT)
-            _send_string("matt.oexp.olang.model.ButtonEvent")
-            _send_int(args[0])
-            _send_string(args[1])
+            _send_string("matt.oexp.olang.lab.model.trial.GalleryTrial")
+            _send_string(args[0])
+            _send_int(len(args[1]))
+            for e in args[1]:
+                _send_string(e)
             self._id = _object_id(_recv_long())
         else:
             self._id = _object_id(_id)
 
-    # [[matt.oexp.olang.model.ButtonEvent#button]]
+    # [[matt.oexp.olang.lab.model.trial.GalleryTrial#distractors]]
     @property
-    def button(self) -> str:
+    def distractors(self) -> List[str]:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(0)
-        temp = _recv_string(nullable=False)
+        temp = _recv_list(
+            elementReceiveFun=lambda: _recv_string(nullable=False), nullable=False
+        )
         return temp
 
-    # [[matt.oexp.olang.model.ButtonEvent#timeMillis]]
+    # [[matt.oexp.olang.lab.model.trial.GalleryTrial#query]]
     @property
-    def time_millis(self) -> int:
+    def query(self) -> str:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(1)
-        temp = _recv_int(nullable=False)
+        temp = _recv_string(nullable=False)
         return temp
 
-    # [[matt.oexp.olang.model.ButtonEvent]]
+    # [[matt.oexp.olang.lab.model.trial.GalleryTrial]]
     def to_json(self):
         _ensure_synchronized()
         _sendall(GET_JSON)
         _send_long(self._id._id)
         return _recv_string(nullable=False)
 
-    # [[matt.oexp.olang.model.ButtonEvent]]
+    # [[matt.oexp.olang.lab.model.trial.GalleryTrial]]
     def to_dict(self):
         return json.loads(self.to_json())
 
-    # [[matt.oexp.olang.model.ButtonEvent]]
+    # [[matt.oexp.olang.lab.model.trial.GalleryTrial]]
     def __eq__(self, other):
         _ensure_synchronized()
         if isinstance(other, KBClass):
             _sendall(CHECK_EQUALITY)
             _send_long(self._id._id)
             _send_long(other._id._id)
             return _recv_bool()
@@ -2321,41 +2342,39 @@
 
 
 def encrypted_subject_trial_data(
     pid=NO_DEFAULT,
     session_number=NO_DEFAULT,
     session_id=NO_DEFAULT,
     trial_index=NO_DEFAULT,
-    target=NO_DEFAULT,
-    distractors=NO_DEFAULT,
-    selection_indices=DEFAULT_VALUE,
+    stimuli=NO_DEFAULT,
+    response=NO_DEFAULT,
     start_time_unix_millis=NO_DEFAULT,
     log=DEFAULT_VALUE,
     exp_uid=NO_DEFAULT,
 ):
     _check_required_parameters(
         **dict(
             pid=pid,
             session_number=session_number,
             session_id=session_id,
             trial_index=trial_index,
-            target=target,
-            distractors=distractors,
+            stimuli=stimuli,
+            response=response,
             start_time_unix_millis=start_time_unix_millis,
             exp_uid=exp_uid,
         )
     )
     return EncryptedSubjectTrialData(
         pid,
         session_number,
         session_id,
         trial_index,
-        target,
-        distractors,
-        selection_indices,
+        stimuli,
+        response,
         start_time_unix_millis,
         log,
         exp_uid,
     )
 
 
 # [[matt.oexp.olang.model.EncryptedSubjectTrialData]]
@@ -2367,153 +2386,127 @@
             _sendall(CREATE_OBJECT)
             _send_string("matt.oexp.olang.model.EncryptedSubjectTrialData")
             _send_long(args[0]._id._id)
             _send_long(args[1]._id._id)
             _send_long(args[2]._id._id)
             _send_int(args[3])
             _send_long(args[4]._id._id)
-            _send_int(len(args[5]))
-            for e in args[5]:
-                _send_long(e._id._id)
-            if args[6] == DEFAULT_VALUE:
+            _send_long(args[5]._id._id)
+            _send_long(args[6])
+            if args[7] == DEFAULT_VALUE:
                 _sendall(b"\x00")
             else:
                 _sendall(b"\x01")
-                _send_int(len(args[6]))
-                for e in args[6]:
-                    _send_int(e)
-            _send_long(args[7])
-            if args[8] == DEFAULT_VALUE:
-                _sendall(b"\x00")
-            else:
-                _sendall(b"\x01")
-                _send_int(len(args[8]))
-                for e in args[8]:
+                _send_int(len(args[7]))
+                for e in args[7]:
                     _send_long(e._id._id)
-            _send_long(args[9]._id._id)
+            _send_long(args[8]._id._id)
             self._id = _object_id(_recv_long())
         else:
             self._id = _object_id(_id)
 
-    # [[matt.oexp.olang.model.EncryptedSubjectTrialData#distractors]]
-    @property
-    def distractors(self) -> List[TemporaryEncryptedStimulus]:
-        _ensure_synchronized()
-        _sendall(GET_VAL)
-        _send_long(self._id._id)
-        _send_int(0)
-        temp = _recv_list(
-            elementReceiveFun=lambda: _recv_object(
-                TemporaryEncryptedStimulus, nullable=False
-            ),
-            nullable=False,
-        )
-        return temp
-
     # [[matt.oexp.olang.model.EncryptedSubjectTrialData#expUID]]
     @property
     def exp_uid(self) -> ExperimentUid:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
-        _send_int(1)
+        _send_int(0)
         temp = _recv_object(ExperimentUid, nullable=False)
         return temp
 
     # [[matt.oexp.olang.model.EncryptedSubjectTrialData#log]]
     @property
     def log(self) -> List[SubjectTrialEvent]:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
-        _send_int(2)
+        _send_int(1)
         temp = _recv_list(
             elementReceiveFun=lambda: _recv_object(SubjectTrialEvent, nullable=False),
             nullable=False,
         )
         return temp
 
     # [[matt.oexp.olang.model.EncryptedSubjectTrialData#pid]]
     @property
     def pid(self) -> ProlificParticipantUid:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
-        _send_int(3)
+        _send_int(2)
         temp = _recv_object(ProlificParticipantUid, nullable=False)
         return temp
 
-    # [[matt.oexp.olang.model.EncryptedSubjectTrialData#selectionIndices]]
+    # [[matt.oexp.olang.model.EncryptedSubjectTrialData#response]]
     @property
-    def selection_indices(self) -> List[int]:
+    def response(self) -> TrialResponse:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
-        _send_int(4)
-        temp = _recv_list(
-            elementReceiveFun=lambda: _recv_int(nullable=False), nullable=False
-        )
+        _send_int(3)
+        temp = _recv_object(TrialResponse, nullable=False)
         return temp
 
     # [[matt.oexp.olang.model.EncryptedSubjectTrialData#sessionID]]
     @property
     def session_id(self) -> ProlificSessionId:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
-        _send_int(5)
+        _send_int(4)
         temp = _recv_object(ProlificSessionId, nullable=False)
         return temp
 
     # [[matt.oexp.olang.model.EncryptedSubjectTrialData#sessionNumber]]
     @property
     def session_number(self) -> SessionNumber:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
-        _send_int(6)
+        _send_int(5)
         temp = _recv_object(SessionNumber, nullable=False)
         return temp
 
     # [[matt.oexp.olang.model.EncryptedSubjectTrialData#startTimeUnixMillis]]
     @property
     def start_time_unix_millis(self) -> int:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
-        _send_int(7)
+        _send_int(6)
         temp = _recv_long(nullable=False)
         return temp
 
-    # [[matt.oexp.olang.model.EncryptedSubjectTrialData#target]]
+    # [[matt.oexp.olang.model.EncryptedSubjectTrialData#stimuli]]
     @property
-    def target(self) -> TemporaryEncryptedStimulus:
+    def stimuli(self) -> EncryptedTrial:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
-        _send_int(8)
-        temp = _recv_object(TemporaryEncryptedStimulus, nullable=False)
+        _send_int(7)
+        temp = _recv_object(EncryptedTrial, nullable=False)
         return temp
 
-    @target.setter
-    def target(self, value) -> TemporaryEncryptedStimulus:
+    @stimuli.setter
+    def stimuli(self, value) -> EncryptedTrial:
         _ensure_synchronized()
         _sendall(SET_VAR)
         _send_long(self._id._id)
-        _send_int(8)
+        _send_int(7)
         _send_long(value._id._id)
         _recv_confirmation()
 
     # [[matt.oexp.olang.model.EncryptedSubjectTrialData#trialIndex]]
     @property
     def trial_index(self) -> int:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
-        _send_int(9)
+        _send_int(8)
         temp = _recv_int(nullable=False)
         return temp
 
     # [[matt.oexp.olang.model.EncryptedSubjectTrialData]]
     def to_json(self):
         _ensure_synchronized()
         _sendall(GET_JSON)
@@ -2643,84 +2636,280 @@
             _send_long(self._id._id)
             _send_long(other._id._id)
             return _recv_bool()
         else:
             return False
 
 
+def choice(choice=NO_DEFAULT):
+    _check_required_parameters(**dict(choice=choice))
+    return Choice(choice)
+
+
+# [[matt.oexp.olang.model.response.Choice]]
+class Choice(TrialResponse, KBClass):
+    def __init__(self, *args, _id=None):
+        _ensure_synchronized()
+        if _id is None:
+            jbridge._init_java()
+            _sendall(CREATE_OBJECT)
+            _send_string("matt.oexp.olang.model.response.Choice")
+            _send_string(args[0])
+            self._id = _object_id(_recv_long())
+        else:
+            self._id = _object_id(_id)
+
+    # [[matt.oexp.olang.model.response.Choice#choice]]
+    @property
+    def choice(self) -> str:
+        _ensure_synchronized()
+        _sendall(GET_VAL)
+        _send_long(self._id._id)
+        _send_int(0)
+        temp = _recv_string(nullable=False)
+        return temp
+
+    # [[matt.oexp.olang.model.response.Choice]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.model.response.Choice]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+    # [[matt.oexp.olang.model.response.Choice]]
+    def __eq__(self, other):
+        _ensure_synchronized()
+        if isinstance(other, KBClass):
+            _sendall(CHECK_EQUALITY)
+            _send_long(self._id._id)
+            _send_long(other._id._id)
+            return _recv_bool()
+        else:
+            return False
+
+
+def gallery_selections(selection_indices=NO_DEFAULT):
+    _check_required_parameters(**dict(selection_indices=selection_indices))
+    return GallerySelections(selection_indices)
+
+
+# [[matt.oexp.olang.model.response.GallerySelections]]
+class GallerySelections(TrialResponse, KBClass):
+    def __init__(self, *args, _id=None):
+        _ensure_synchronized()
+        if _id is None:
+            jbridge._init_java()
+            _sendall(CREATE_OBJECT)
+            _send_string("matt.oexp.olang.model.response.GallerySelections")
+            _send_int(len(args[0]))
+            for e in args[0]:
+                _send_int(e)
+            self._id = _object_id(_recv_long())
+        else:
+            self._id = _object_id(_id)
+
+    # [[matt.oexp.olang.model.response.GallerySelections#selectionIndices]]
+    @property
+    def selection_indices(self) -> List[int]:
+        _ensure_synchronized()
+        _sendall(GET_VAL)
+        _send_long(self._id._id)
+        _send_int(0)
+        temp = _recv_list(
+            elementReceiveFun=lambda: _recv_int(nullable=False), nullable=False
+        )
+        return temp
+
+    # [[matt.oexp.olang.model.response.GallerySelections]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.model.response.GallerySelections]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+    # [[matt.oexp.olang.model.response.GallerySelections]]
+    def __eq__(self, other):
+        _ensure_synchronized()
+        if isinstance(other, KBClass):
+            _sendall(CHECK_EQUALITY)
+            _send_long(self._id._id)
+            _send_long(other._id._id)
+            return _recv_bool()
+        else:
+            return False
+
+
+# [[matt.oexp.olang.model.stim.EncryptedTrial]]
+class EncryptedTrial(TrialStimuli, KBClass, abc.ABC):
+    # [[matt.oexp.olang.model.stim.EncryptedTrial]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.model.stim.EncryptedTrial]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+
+# [[matt.oexp.olang.model.stim.RawTrial]]
+class RawTrial(TrialStimuli, KBClass, abc.ABC):
+    # [[matt.oexp.olang.model.stim.RawTrial]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.model.stim.RawTrial]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+
+def button_event(time_millis=NO_DEFAULT, button=NO_DEFAULT):
+    _check_required_parameters(**dict(time_millis=time_millis, button=button))
+    return ButtonEvent(time_millis, button)
+
+
+# [[matt.oexp.olang.model.trialevent.ButtonEvent]]
+class ButtonEvent(SubjectTrialEvent, KBClass):
+    def __init__(self, *args, _id=None):
+        _ensure_synchronized()
+        if _id is None:
+            jbridge._init_java()
+            _sendall(CREATE_OBJECT)
+            _send_string("matt.oexp.olang.model.trialevent.ButtonEvent")
+            _send_int(args[0])
+            _send_string(args[1])
+            self._id = _object_id(_recv_long())
+        else:
+            self._id = _object_id(_id)
+
+    # [[matt.oexp.olang.model.trialevent.ButtonEvent#button]]
+    @property
+    def button(self) -> str:
+        _ensure_synchronized()
+        _sendall(GET_VAL)
+        _send_long(self._id._id)
+        _send_int(0)
+        temp = _recv_string(nullable=False)
+        return temp
+
+    # [[matt.oexp.olang.model.trialevent.ButtonEvent#timeMillis]]
+    @property
+    def time_millis(self) -> int:
+        _ensure_synchronized()
+        _sendall(GET_VAL)
+        _send_long(self._id._id)
+        _send_int(1)
+        temp = _recv_int(nullable=False)
+        return temp
+
+    # [[matt.oexp.olang.model.trialevent.ButtonEvent]]
+    def to_json(self):
+        _ensure_synchronized()
+        _sendall(GET_JSON)
+        _send_long(self._id._id)
+        return _recv_string(nullable=False)
+
+    # [[matt.oexp.olang.model.trialevent.ButtonEvent]]
+    def to_dict(self):
+        return json.loads(self.to_json())
+
+    # [[matt.oexp.olang.model.trialevent.ButtonEvent]]
+    def __eq__(self, other):
+        _ensure_synchronized()
+        if isinstance(other, KBClass):
+            _sendall(CHECK_EQUALITY)
+            _send_long(self._id._id)
+            _send_long(other._id._id)
+            return _recv_bool()
+        else:
+            return False
+
+
 def selection_event(
     time_millis=NO_DEFAULT, selection_index=NO_DEFAULT, distractor_index=NO_DEFAULT
 ):
     _check_required_parameters(
         **dict(
             time_millis=time_millis,
             selection_index=selection_index,
             distractor_index=distractor_index,
         )
     )
     return SelectionEvent(time_millis, selection_index, distractor_index)
 
 
-# [[matt.oexp.olang.model.SelectionEvent]]
+# [[matt.oexp.olang.model.trialevent.SelectionEvent]]
 class SelectionEvent(SubjectTrialEvent, KBClass):
     def __init__(self, *args, _id=None):
         _ensure_synchronized()
         if _id is None:
             jbridge._init_java()
             _sendall(CREATE_OBJECT)
-            _send_string("matt.oexp.olang.model.SelectionEvent")
+            _send_string("matt.oexp.olang.model.trialevent.SelectionEvent")
             _send_int(args[0])
             _send_int(args[1])
             _send_int(args[2])
             self._id = _object_id(_recv_long())
         else:
             self._id = _object_id(_id)
 
-    # [[matt.oexp.olang.model.SelectionEvent#distractorIndex]]
+    # [[matt.oexp.olang.model.trialevent.SelectionEvent#distractorIndex]]
     @property
     def distractor_index(self) -> int:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(0)
         temp = _recv_int(nullable=False)
         return temp
 
-    # [[matt.oexp.olang.model.SelectionEvent#selectionIndex]]
+    # [[matt.oexp.olang.model.trialevent.SelectionEvent#selectionIndex]]
     @property
     def selection_index(self) -> int:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(1)
         temp = _recv_int(nullable=False)
         return temp
 
-    # [[matt.oexp.olang.model.SelectionEvent#timeMillis]]
+    # [[matt.oexp.olang.model.trialevent.SelectionEvent#timeMillis]]
     @property
     def time_millis(self) -> int:
         _ensure_synchronized()
         _sendall(GET_VAL)
         _send_long(self._id._id)
         _send_int(2)
         temp = _recv_int(nullable=False)
         return temp
 
-    # [[matt.oexp.olang.model.SelectionEvent]]
+    # [[matt.oexp.olang.model.trialevent.SelectionEvent]]
     def to_json(self):
         _ensure_synchronized()
         _sendall(GET_JSON)
         _send_long(self._id._id)
         return _recv_string(nullable=False)
 
-    # [[matt.oexp.olang.model.SelectionEvent]]
+    # [[matt.oexp.olang.model.trialevent.SelectionEvent]]
     def to_dict(self):
         return json.loads(self.to_json())
 
-    # [[matt.oexp.olang.model.SelectionEvent]]
+    # [[matt.oexp.olang.model.trialevent.SelectionEvent]]
     def __eq__(self, other):
         _ensure_synchronized()
         if isinstance(other, KBClass):
             _sendall(CHECK_EQUALITY)
             _send_long(self._id._id)
             _send_long(other._id._id)
             return _recv_bool()
```

### Comparing `oexp-0.8.5/oexp/jbridge.py` & `oexp-0.9.0/oexp/jbridge.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,20 @@
 
 import oexp.access as access
 from oexp.util import ops
 from oexp.util import vals
 
 import os
 
-print("invalidate version 3")
-
 _jar_process: Optional[subprocess.Popen] = None
 _java_sock: Optional[socket.socket] = None
 _java_exit_sock: Optional[socket.socket] = None
 _java_conn: Optional[socket.socket] = None
 _java_exit_conn: Optional[socket.socket] = None
 
-
 LOCAL_JAR = os.getenv("LOCAL_JAR")
 
 
 # https://stackoverflow.com/questions/1395593/managing-resources-in-a-python-project
 # https://docs.python.org/3/library/subprocess.html
 # https://docs.python.org/3/library/importlib.resources.html#module-importlib.resources
 def _init_java():
```

### Comparing `oexp-0.8.5/oexp/util/ops.py` & `oexp-0.9.0/oexp/util/ops.py`

 * *Files identical despite different names*

### Comparing `oexp-0.8.5/oexp/util/vals.py` & `oexp-0.9.0/oexp/util/vals.py`

 * *Files identical despite different names*


# Comparing `tmp/ifd_python-10.1.8.tar.gz` & `tmp/ifd_python-10.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifd_python-10.1.8.tar", max compression
+gzip compressed data, was "ifd_python-10.1.9.tar", max compression
```

## Comparing `ifd_python-10.1.8.tar` & `ifd_python-10.1.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1093 2023-05-16 13:28:13.433655 ifd_python-10.1.8/LICENSE
--rw-r--r--   0        0        0      551 2023-05-16 13:28:13.433655 ifd_python-10.1.8/README.md
--rw-r--r--   0        0        0      283 2023-05-16 13:28:13.433655 ifd_python-10.1.8/ifd/__init__.py
--rw-r--r--   0        0        0      971 2023-05-16 13:28:13.433655 ifd_python-10.1.8/ifd/entities/Abstract/ADetection.py
--rw-r--r--   0        0        0       34 2023-05-16 13:28:13.433655 ifd_python-10.1.8/ifd/entities/Abstract/__init__.py
--rw-r--r--   0        0        0      630 2023-05-16 13:28:13.433655 ifd_python-10.1.8/ifd/entities/BodyTicket.py
--rw-r--r--   0        0        0      734 2023-05-16 13:28:13.433655 ifd_python-10.1.8/ifd/entities/Classification.py
--rw-r--r--   0        0        0      228 2023-05-16 13:28:13.433655 ifd_python-10.1.8/ifd/entities/Couleur.py
--rw-r--r--   0        0        0      707 2023-05-16 13:28:13.433655 ifd_python-10.1.8/ifd/entities/Detection.py
--rw-r--r--   0        0        0     2303 2023-05-16 13:28:13.433655 ifd_python-10.1.8/ifd/entities/Image.py
--rw-r--r--   0        0        0      730 2023-05-16 13:28:13.433655 ifd_python-10.1.8/ifd/entities/Intervention.py
--rw-r--r--   0        0        0     1428 2023-05-16 13:28:13.433655 ifd_python-10.1.8/ifd/entities/LogResult.py
--rw-r--r--   0        0        0      741 2023-05-16 13:28:13.433655 ifd_python-10.1.8/ifd/entities/Malfacon.py
--rw-r--r--   0        0        0      477 2023-05-16 13:28:13.433655 ifd_python-10.1.8/ifd/entities/Modele.py
--rw-r--r--   0        0        0      794 2023-05-16 13:28:13.433655 ifd_python-10.1.8/ifd/entities/OCR.py
--rw-r--r--   0        0        0      529 2023-05-16 13:28:13.433655 ifd_python-10.1.8/ifd/entities/RabbitMqMessage.py
--rw-r--r--   0        0        0     1033 2023-05-17 09:32:12.521357 ifd_python-10.1.8/ifd/entities/Tag.py
--rw-r--r--   0        0        0      449 2023-05-25 07:06:16.414795 ifd_python-10.1.8/ifd/entities/Ticket.py
--rw-r--r--   0        0        0      400 2023-05-16 13:28:13.433655 ifd_python-10.1.8/ifd/entities/__init__.py
--rw-r--r--   0        0        0      717 2023-05-16 13:28:13.433655 ifd_python-10.1.8/ifd/entities/bbox.py
--rw-r--r--   0        0        0     2161 2023-05-16 13:28:13.433655 ifd_python-10.1.8/ifd/repository/AmqpImageRepository.py
--rw-r--r--   0        0        0     2215 2023-05-16 13:28:13.433655 ifd_python-10.1.8/ifd/repository/RestTicketRepository.py
--rw-r--r--   0        0        0     1039 2023-05-17 15:23:08.904378 ifd_python-10.1.8/ifd/repository/SqlLogRepository.py
--rw-r--r--   0        0        0     1900 2023-06-06 07:46:40.923654 ifd_python-10.1.8/ifd/repository/SqlTicketRepository.py
--rw-r--r--   0        0        0      210 2023-05-16 13:28:13.433655 ifd_python-10.1.8/ifd/repository/__init__.py
--rw-r--r--   0        0        0      940 2023-05-16 13:28:13.433655 ifd_python-10.1.8/ifd/repository/abstract/AbsSqlRepository.py
--rw-r--r--   0        0        0       46 2023-05-16 13:28:13.433655 ifd_python-10.1.8/ifd/repository/abstract/__init__.py
--rw-r--r--   0        0        0     1082 2023-05-16 13:28:13.433655 ifd_python-10.1.8/ifd/spec.py
--rw-r--r--   0        0        0      831 2023-05-25 07:06:16.414795 ifd_python-10.1.8/ifd/tools.py
--rw-r--r--   0        0        0      131 2023-05-16 13:28:13.433655 ifd_python-10.1.8/ifd/usecase/Interfaces/IFonction.py
--rw-r--r--   0        0        0       32 2023-05-16 13:28:13.433655 ifd_python-10.1.8/ifd/usecase/Interfaces/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 07:46:40.955654 ifd_python-10.1.8/ifd/usecase/__init__.py
--rw-r--r--   0        0        0      407 2023-06-06 07:46:50.191567 ifd_python-10.1.8/pyproject.toml
--rw-r--r--   0        0        0     1244 1970-01-01 00:00:00.000000 ifd_python-10.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-05-16 13:28:13.433655 ifd_python-10.1.9/LICENSE
+-rw-r--r--   0        0        0      551 2023-05-16 13:28:13.433655 ifd_python-10.1.9/README.md
+-rw-r--r--   0        0        0      283 2023-05-16 13:28:13.433655 ifd_python-10.1.9/ifd/__init__.py
+-rw-r--r--   0        0        0      971 2023-05-16 13:28:13.433655 ifd_python-10.1.9/ifd/entities/Abstract/ADetection.py
+-rw-r--r--   0        0        0       34 2023-05-16 13:28:13.433655 ifd_python-10.1.9/ifd/entities/Abstract/__init__.py
+-rw-r--r--   0        0        0      630 2023-05-16 13:28:13.433655 ifd_python-10.1.9/ifd/entities/BodyTicket.py
+-rw-r--r--   0        0        0      734 2023-05-16 13:28:13.433655 ifd_python-10.1.9/ifd/entities/Classification.py
+-rw-r--r--   0        0        0      228 2023-05-16 13:28:13.433655 ifd_python-10.1.9/ifd/entities/Couleur.py
+-rw-r--r--   0        0        0      707 2023-05-16 13:28:13.433655 ifd_python-10.1.9/ifd/entities/Detection.py
+-rw-r--r--   0        0        0     2303 2023-05-16 13:28:13.433655 ifd_python-10.1.9/ifd/entities/Image.py
+-rw-r--r--   0        0        0      730 2023-05-16 13:28:13.433655 ifd_python-10.1.9/ifd/entities/Intervention.py
+-rw-r--r--   0        0        0     1428 2023-05-16 13:28:13.433655 ifd_python-10.1.9/ifd/entities/LogResult.py
+-rw-r--r--   0        0        0      741 2023-05-16 13:28:13.433655 ifd_python-10.1.9/ifd/entities/Malfacon.py
+-rw-r--r--   0        0        0      477 2023-05-16 13:28:13.433655 ifd_python-10.1.9/ifd/entities/Modele.py
+-rw-r--r--   0        0        0      794 2023-05-16 13:28:13.433655 ifd_python-10.1.9/ifd/entities/OCR.py
+-rw-r--r--   0        0        0      529 2023-05-16 13:28:13.433655 ifd_python-10.1.9/ifd/entities/RabbitMqMessage.py
+-rw-r--r--   0        0        0     1033 2023-05-17 09:32:12.521357 ifd_python-10.1.9/ifd/entities/Tag.py
+-rw-r--r--   0        0        0      449 2023-05-25 07:06:16.414795 ifd_python-10.1.9/ifd/entities/Ticket.py
+-rw-r--r--   0        0        0      400 2023-05-16 13:28:13.433655 ifd_python-10.1.9/ifd/entities/__init__.py
+-rw-r--r--   0        0        0      717 2023-05-16 13:28:13.433655 ifd_python-10.1.9/ifd/entities/bbox.py
+-rw-r--r--   0        0        0     2161 2023-05-16 13:28:13.433655 ifd_python-10.1.9/ifd/repository/AmqpImageRepository.py
+-rw-r--r--   0        0        0     2215 2023-05-16 13:28:13.433655 ifd_python-10.1.9/ifd/repository/RestTicketRepository.py
+-rw-r--r--   0        0        0     1039 2023-05-17 15:23:08.904378 ifd_python-10.1.9/ifd/repository/SqlLogRepository.py
+-rw-r--r--   0        0        0     1891 2023-06-06 08:19:56.169556 ifd_python-10.1.9/ifd/repository/SqlTicketRepository.py
+-rw-r--r--   0        0        0      210 2023-05-16 13:28:13.433655 ifd_python-10.1.9/ifd/repository/__init__.py
+-rw-r--r--   0        0        0      940 2023-05-16 13:28:13.433655 ifd_python-10.1.9/ifd/repository/abstract/AbsSqlRepository.py
+-rw-r--r--   0        0        0       46 2023-05-16 13:28:13.433655 ifd_python-10.1.9/ifd/repository/abstract/__init__.py
+-rw-r--r--   0        0        0     1082 2023-05-16 13:28:13.433655 ifd_python-10.1.9/ifd/spec.py
+-rw-r--r--   0        0        0      831 2023-05-25 07:06:16.414795 ifd_python-10.1.9/ifd/tools.py
+-rw-r--r--   0        0        0      131 2023-05-16 13:28:13.433655 ifd_python-10.1.9/ifd/usecase/Interfaces/IFonction.py
+-rw-r--r--   0        0        0       32 2023-05-16 13:28:13.433655 ifd_python-10.1.9/ifd/usecase/Interfaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 08:19:56.181556 ifd_python-10.1.9/ifd/usecase/__init__.py
+-rw-r--r--   0        0        0      407 2023-06-06 08:20:05.749470 ifd_python-10.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1244 1970-01-01 00:00:00.000000 ifd_python-10.1.9/PKG-INFO
```

### Comparing `ifd_python-10.1.8/LICENSE` & `ifd_python-10.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.8/README.md` & `ifd_python-10.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.8/ifd/entities/Abstract/ADetection.py` & `ifd_python-10.1.9/ifd/entities/Abstract/ADetection.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.8/ifd/entities/BodyTicket.py` & `ifd_python-10.1.9/ifd/entities/BodyTicket.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.8/ifd/entities/Classification.py` & `ifd_python-10.1.9/ifd/entities/Classification.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.8/ifd/entities/Detection.py` & `ifd_python-10.1.9/ifd/entities/Detection.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.8/ifd/entities/Image.py` & `ifd_python-10.1.9/ifd/entities/Image.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.8/ifd/entities/Intervention.py` & `ifd_python-10.1.9/ifd/entities/Intervention.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.8/ifd/entities/LogResult.py` & `ifd_python-10.1.9/ifd/entities/LogResult.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.8/ifd/entities/Malfacon.py` & `ifd_python-10.1.9/ifd/entities/Malfacon.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.8/ifd/entities/OCR.py` & `ifd_python-10.1.9/ifd/entities/OCR.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.8/ifd/entities/RabbitMqMessage.py` & `ifd_python-10.1.9/ifd/entities/RabbitMqMessage.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.8/ifd/entities/Tag.py` & `ifd_python-10.1.9/ifd/entities/Tag.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.8/ifd/entities/bbox.py` & `ifd_python-10.1.9/ifd/entities/bbox.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.8/ifd/repository/AmqpImageRepository.py` & `ifd_python-10.1.9/ifd/repository/AmqpImageRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.8/ifd/repository/RestTicketRepository.py` & `ifd_python-10.1.9/ifd/repository/RestTicketRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.8/ifd/repository/SqlLogRepository.py` & `ifd_python-10.1.9/ifd/repository/SqlLogRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.8/ifd/repository/SqlTicketRepository.py` & `ifd_python-10.1.9/ifd/repository/SqlTicketRepository.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,24 +13,24 @@
             EXEC PROC_SELECT_IRRIS_TICKET_AUTOMATIC_ITA
             """, 
             self.connection
         )
         
         return self._dataframe_to_list_of_ticket(df)
     
-    def updateStatut(self, ticket, statut):
+    def updateStatut(self, ticket, statut, message):
         if not self.is_open:
             self._connectToDatabase()
         
         ticket.ita_ticket_request = ticket.ita_ticket_request.replace("'", "''")
         
         cur = self.connection.cursor()
         req = f"""
             UPDATE [Infradeep].[dbo].[T_D_IRRIS_TICKET_AUTOMATIC_ITA]
-            SET ITA_VALIDATION_STATUT = '{statut}', ITA_TICKET_RESPONSE = '{ticket.ita_ticket_request}', ITA_DATE_ACTION_TICKET = GETDATE()
+            SET ITA_VALIDATION_STATUT = '{statut}', ITA_TICKET_RESPONSE = '{message}', ITA_DATE_ACTION_TICKET = GETDATE()
             WHERE ITA_ID = {ticket.ita_id}
             """
         cur.execute(req)
         cur.close()
         
     def insertLog(self, ticket, sendRoute, response, expediteur):
         if not self.is_open:
```

### Comparing `ifd_python-10.1.8/ifd/repository/abstract/AbsSqlRepository.py` & `ifd_python-10.1.9/ifd/repository/abstract/AbsSqlRepository.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.8/ifd/spec.py` & `ifd_python-10.1.9/ifd/spec.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.8/ifd/tools.py` & `ifd_python-10.1.9/ifd/tools.py`

 * *Files identical despite different names*

### Comparing `ifd_python-10.1.8/PKG-INFO` & `ifd_python-10.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifd-python
-Version: 10.1.8
+Version: 10.1.9
 Summary: 
 Author: Antonin Lemoine
 Author-email: antonin.lemoine@altitudeinfra.fr
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```


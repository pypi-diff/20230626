# Comparing `tmp/pywa-0.0.1rc7-py3-none-any.whl.zip` & `tmp/pywa-0.0.1rc8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 21025 bytes, number of entries: 14
--rw-rw-r--  2.0 unx      143 b- defN 23-Jun-22 18:25 pywa/__init__.py
--rw-rw-r--  2.0 unx     7965 b- defN 23-Jun-22 15:59 pywa/api.py
--rw-rw-r--  2.0 unx    23158 b- defN 23-Jun-22 18:15 pywa/client.py
+Zip file size: 22785 bytes, number of entries: 14
+-rw-rw-r--  2.0 unx      143 b- defN 23-Jun-26 09:18 pywa/__init__.py
+-rw-rw-r--  2.0 unx    14911 b- defN 23-Jun-26 08:51 pywa/api.py
+-rw-rw-r--  2.0 unx    26284 b- defN 23-Jun-26 09:16 pywa/client.py
 -rw-rw-r--  2.0 unx      989 b- defN 23-Jun-19 21:14 pywa/errors.py
 -rw-rw-r--  2.0 unx    11021 b- defN 23-Jun-22 17:14 pywa/filters.py
 -rw-rw-r--  2.0 unx     1464 b- defN 23-Jun-22 18:21 pywa/handlers.py
--rw-rw-r--  2.0 unx    25776 b- defN 23-Jun-22 15:59 pywa/types.py
+-rw-rw-r--  2.0 unx    32258 b- defN 23-Jun-26 09:16 pywa/types.py
 -rw-rw-r--  2.0 unx      991 b- defN 23-Jun-20 16:58 pywa/utils.py
--rw-rw-r--  2.0 unx     4141 b- defN 23-Jun-22 18:21 pywa/webhook.py
--rw-rw-r--  2.0 unx     1066 b- defN 23-Jun-22 18:25 pywa-0.0.1rc7.dist-info/LICENSE
--rw-rw-r--  2.0 unx    10203 b- defN 23-Jun-22 18:25 pywa-0.0.1rc7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-22 18:25 pywa-0.0.1rc7.dist-info/WHEEL
--rw-rw-r--  2.0 unx        5 b- defN 23-Jun-22 18:25 pywa-0.0.1rc7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1026 b- defN 23-Jun-22 18:25 pywa-0.0.1rc7.dist-info/RECORD
-14 files, 88040 bytes uncompressed, 19367 bytes compressed:  78.0%
+-rw-rw-r--  2.0 unx     4161 b- defN 23-Jun-26 07:53 pywa/webhook.py
+-rw-rw-r--  2.0 unx     1066 b- defN 23-Jun-26 09:19 pywa-0.0.1rc8.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     4489 b- defN 23-Jun-26 09:19 pywa-0.0.1rc8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-26 09:19 pywa-0.0.1rc8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jun-26 09:19 pywa-0.0.1rc8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1026 b- defN 23-Jun-26 09:19 pywa-0.0.1rc8.dist-info/RECORD
+14 files, 98900 bytes uncompressed, 21127 bytes compressed:  78.6%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: pywa/utils.py
 Comment: 
 
 Filename: pywa/webhook.py
 Comment: 
 
-Filename: pywa-0.0.1rc7.dist-info/LICENSE
+Filename: pywa-0.0.1rc8.dist-info/LICENSE
 Comment: 
 
-Filename: pywa-0.0.1rc7.dist-info/METADATA
+Filename: pywa-0.0.1rc8.dist-info/METADATA
 Comment: 
 
-Filename: pywa-0.0.1rc7.dist-info/WHEEL
+Filename: pywa-0.0.1rc8.dist-info/WHEEL
 Comment: 
 
-Filename: pywa-0.0.1rc7.dist-info/top_level.txt
+Filename: pywa-0.0.1rc8.dist-info/top_level.txt
 Comment: 
 
-Filename: pywa-0.0.1rc7.dist-info/RECORD
+Filename: pywa-0.0.1rc8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pywa/__init__.py

```diff
@@ -1,5 +1,5 @@
 """Python wrapper for the WhatsApp Cloud API. https://github.com/david-lev/pywa"""
 
-__version__ = "0.0.1rc7"
+__version__ = "0.0.1rc8"
 
 from pywa.client import WhatsApp
```

## pywa/api.py

```diff
@@ -1,10 +1,10 @@
 import mimetypes
-from typing import Iterable
 import requests
+from typing import Iterable
 from pywa.errors import WhatsAppApiError
 from pywa.types import InlineButton, SectionList, Contact
 
 
 class WhatsAppCloudApi:
     """Internal methods for the WhatsApp client."""
 
@@ -30,61 +30,102 @@
 
     def _make_request(
             self,
             method: str,
             endpoint: str,
             **kwargs
     ) -> dict | list:
-        res = self._session.request(method=method, url=f"{self._base_url}/{self.phone_id}{endpoint}", **kwargs)
+        """
+        Internal method to make a request to the WhatsApp API.
+
+        Args:
+            method: The HTTP method to use.
+            endpoint: The endpoint to request.
+            **kwargs: Additional arguments to pass to the request.
+
+        Returns:
+            The response JSON.
+
+        Raises:
+            WhatsAppApiError: If the request failed.
+        """
+        res = self._session.request(method=method, url=f"{self._base_url}{endpoint}", **kwargs)
         if res.status_code != 200:
             raise WhatsAppApiError(status_code=res.status_code, error=res.json()["error"])
         return res.json()
 
     def send_text_message(
             self,
             to: str | int,
             text: str,
             preview_url: bool = False,
             reply_to_message_id: str | None = None,
-    ) -> str:
+    ) -> dict[str, dict | list]:
+        """
+        Send a text message to a WhatsApp user.
+
+        Return example::
+
+            {
+                'messaging_product': 'whatsapp',
+                'contacts': [{'input': '1234567890', 'wa_id': '1234567890'}],
+                'messages': [{'id': 'wamid.XXXXXXXXXXXXXXXX=='}]
+            }
+
+        Args:
+            to: The WhatsApp ID of the recipient.
+            text: The text to send.
+            preview_url: Whether to show a preview of the URL in the message.
+            reply_to_message_id: The ID of the message to reply to.
+
+        Returns:
+            The sent message.
+        """
         data = {
             **self._common_keys,
             "to": str(to),
             "type": "text",
             "text": {
                 "body": text,
                 "preview_url": preview_url
             },
         }
         if reply_to_message_id:
             data["context"] = {"message_id": reply_to_message_id}
 
         return self._make_request(
             method="POST",
-            endpoint=f"/messages",
+            endpoint=f"/{self.phone_id}/messages",
             json=data
-        )['messages'][0]['id']
+        )
 
     def upload_media(
             self,
             media: str | bytes,
             mime_type: str | None
-    ) -> str:
+    ) -> dict[str, str]:
         """
         Upload a media file to WhatsApp.
 
+        Return example::
+
+            {
+              'id':'<MEDIA_ID>'
+            }
+
         Args:
             media: media bytes / path / URL to upload.
             mime_type: The type of the media file (if not provided, it will be guessed with the `mimetypes` library).
 
         Returns:
-            The ID of the uploaded media file.
+            A dict with the ID of the uploaded media file.
 
         Raises:
-            ValueError: If ``mime_type`` is not provided and cannot be guessed (e.g. for bytes or URLs without ``Content-Type`` header).
+            ValueError: If ``mime_type`` is not provided and cannot be guessed (e.g. for bytes or URLs without
+             ``Content-Type`` header).
         """
         if isinstance(media, str):
             if media.startswith(("https://", "http://")):
                 res = requests.get(media)
                 res.raise_for_status()
                 file = res.content
                 mime_type = mime_type or res.headers.get('Content-Type', default=res.headers.get('content-type'))
@@ -101,109 +142,268 @@
         files = {
             'file': (None, file),
             'type': (None, mime_type),
             'messaging_product': (None, '"whatsapp"'),
         }
         return self._make_request(
             method="POST",
-            endpoint=f"/media",
+            endpoint=f"/{self.phone_id}/media",
             headers=headers,
             files=files
-        )["id"]
+        )
+
+    def get_media_url(self, media_id: str) -> dict:
+        """
+        Get the URL of a media file.
+            - The url is valid for 5 minutes and can be downloaded only with access token.
+            - For more info: https://developers.facebook.com/docs/whatsapp/cloud-api/reference/media#retrieve-media-url
+
+        Return example::
+
+            {
+                'url': 'https://lookaside.fbsbx.com/whatsapp_business/attachments/?mid=645645&ext=54353&hash=xxx-xx',
+                'mime_type': 'image/jpeg',
+                'sha256': '73298ec14751fhfonf4wfxxxf52f4fb031db3892ff5',
+                'file_size': 61901,
+                'id': '137524587935346',
+                'messaging_product': 'whatsapp'
+            }
+
+        Args:
+            media_id: The ID of the media file.
+
+        Returns:
+            A dict with the URL and other info about the media file.
+        """
+        return self._make_request(
+            method="GET",
+            endpoint=f"/{media_id}"
+        )
+
+    def download_media(
+            self,
+            media_url: str,
+    ) -> tuple[bytes, str]:
+        """
+        Download a media file from WhatsApp servers.
+
+        Args:
+            media_url: The URL of the media file (from ``get_media_url``).
+
+        Returns:
+            The media file bytes and the MIME type.
+        """
+        headers = self._session.headers.copy()
+        del headers["Content-Type"]
+        res = self._session.get(media_url, headers=headers)
+        res.raise_for_status()
+        return res.content, res.headers.get("Content-Type", default=res.headers.get("content-type")) \
+                            or 'application/octet-stream'
+
+    def delete_media(self, media_id: str) -> dict[str, bool]:
+        """
+        Delete a media file from WhatsApp servers.
+
+        Return example::
+
+            {'success': True}
+
+        Args:
+            media_id: The ID of the media file.
+
+        Returns:
+            True if the media file was deleted successfully, False otherwise.
+        """
+        return self._make_request(
+            method="DELETE",
+            endpoint=f"/{media_id}"
+        )
 
     def send_media(
             self,
             to: str | int,
             media_id_or_url: str,
             media_type: str,
             reply_to_message_id: str | None = None,
             **kwargs
-    ):
+    ) -> dict[str, dict | list]:
+        """
+        Send a media file to a WhatsApp user.
+
+        Return example::
+
+            {
+                'messaging_product': 'whatsapp',
+                'contacts': [{'input': '1234567890', 'wa_id': '1234567890'}],
+                'messages': [{'id': 'wamid.XXXXXXXXXXXXXXXX=='}]
+            }
+
+        Args:
+            to: The WhatsApp ID of the recipient.
+            media_id_or_url: The ID or URL of the media file to send.
+            media_type: The type of the media file.
+            reply_to_message_id: The ID of the message to reply to.
+            **kwargs: Additional arguments to send with the message.
+
+        Returns:
+            The sent message.
+        """
         if reply_to_message_id:
             kwargs["context"] = {"message_id": reply_to_message_id}
         data = {
             **self._common_keys,
             "to": str(to),
             "type": media_type,
             media_type: {
                 "link" if media_id_or_url.startswith(('https:', 'http:')) else "id": media_id_or_url,
                 **{k: v for k, v in kwargs.items() if v is not None}
             }
         }
         return self._make_request(
             method="POST",
-            endpoint=f"/messages",
+            endpoint=f"/{self.phone_id}/messages",
             json=data
-        )['messages'][0]['id']
+        )
 
     def send_reaction(
             self,
             to: str | int,
             emoji: str,
             message_id: str,
-    ):
+    ) -> dict[str, dict | list]:
+        """
+        Send a reaction to a message.
+
+        Return example::
+
+            {
+                'messaging_product': 'whatsapp',
+                'contacts': [{'input': '1234567890', 'wa_id': '1234567890'}],
+                'messages': [{'id': 'wamid.XXXXXXXXXXXXXXXX=='}]
+            }
+
+        Args:
+            to: The WhatsApp ID of the recipient.
+            emoji: The emoji to react with (empty to remove reaction).
+            message_id: The ID of the message to react to.
+
+        Returns:
+            The sent message.
+        """
         return self._make_request(
             method="POST",
-            endpoint="/messages/",
+            endpoint=f"/{self.phone_id}/messages/",
             json={
                 **self._common_keys,
                 "to": str(to),
                 "type": "reaction",
                 "reaction": {
                     "emoji": emoji,
                     "message_id": message_id
                 }
             }
-        )['messages'][0]['id']
+        )
 
     def send_location(
             self,
             to: str | int,
             latitude: float,
             longitude: float,
             name: str | None = None,
             address: str | None = None,
-    ):
+    ) -> dict[str, dict | list]:
+        """
+        Send a location to a WhatsApp user.
+
+        Return example::
+
+            {
+                'messaging_product': 'whatsapp',
+                'contacts': [{'input': '1234567890', 'wa_id': '1234567890'}],
+                'messages': [{'id': 'wamid.XXXXXXXXXXXXXXXX=='}]
+            }
+
+        Args:
+            to: The WhatsApp ID of the recipient.
+            latitude: The latitude of the location.
+            longitude: The longitude of the location.
+            name: The name of the location.
+            address: The address of the location.
+
+        Returns:
+            The sent message.
+        """
         data = {
             **self._common_keys,
             "to": str(to),
             "type": "location",
             "location": {
                 "latitude": latitude,
                 "longitude": longitude,
                 "name": name,
                 "address": address
             }
         }
 
         return self._make_request(
             method="POST",
-            endpoint=f"/messages",
+            endpoint=f"/{self.phone_id}/messages",
             json=data
         )['messages'][0]['id']
 
     def send_raw_json(
             self,
             data: dict
     ) -> dict:
+        """
+        Send a raw JSON message to a WhatsApp Cloud API.
+
+        Args:
+            data: The raw JSON data to send.
+
+        Returns:
+            The sent message.
+        """
         return self._make_request(
             method="POST",
-            endpoint=f"/messages",
+            endpoint=f"/{self.phone_id}/messages",
             json=data
         )
 
     def send_interactive_message(
             self,
             to: str | int,
             keyboard: list[InlineButton] | SectionList,
             body: str,
             header: dict | None = None,
             footer: str | None = None,
             reply_to_message_id: str | None = None,
-    ) -> str:
+    ) -> dict[str, dict | list]:
+        """
+        Send an interactive message to a WhatsApp user.
+
+        Return example::
+
+            {
+                'messaging_product': 'whatsapp',
+                'contacts': [{'input': '1234567890', 'wa_id': '1234567890'}],
+                'messages': [{'id': 'wamid.XXXXXXXXXXXXXXXX=='}]
+            }
+
+        Args:
+            to: The WhatsApp ID of the recipient.
+            keyboard: The keyboard to send.
+            body: The body of the message.
+            header: The header of the message.
+            footer: The footer of the message.
+            reply_to_message_id: The ID of the message to reply to.
+
+        Returns:
+            The sent message.
+        """
         data = {
             **self._common_keys,
             "to": str(to),
             "type": "interactive",
             "interactive": {
                 "type": "",
                 "action": {},
@@ -221,44 +421,76 @@
         if header:
             data["interactive"]["header"] = header
         if footer:
             data["interactive"]["footer"] = {"text": footer}
 
         return self._make_request(
             method="POST",
-            endpoint=f"/messages",
+            endpoint=f"/{self.phone_id}/messages",
             json=data
-        )['messages'][0]['id']
+        )
 
     def send_contacts(
             self,
             to: str | int,
             contacts: Iterable[Contact],
             reply_to_message_id: str | None = None,
-    ) -> str:
+    ) -> dict[str, dict | list]:
+        """
+        Send a list of contacts to a WhatsApp user.
+
+        Return example::
+
+            {
+                'messaging_product': 'whatsapp',
+                'contacts': [{'input': '1234567890', 'wa_id': '1234567890'}],
+                'messages': [{'id': 'wamid.XXXXXXXXXXXXXXXX=='}]
+            }
+
+        Args:
+            to: The WhatsApp ID of the recipient.
+            contacts: The contacts to send.
+            reply_to_message_id: The ID of the message to reply to.
+
+        Returns:
+            The sent message.
+        """
         data = {
             **self._common_keys,
             "to": str(to),
             "type": "contacts",
             "contacts": [contact.to_dict() for contact in contacts]
         }
         if reply_to_message_id:
             data["context"] = {"message_id": reply_to_message_id}
         return self._make_request(
             method="POST",
-            endpoint=f"/messages",
+            endpoint=f"/{self.phone_id}/messages",
             json=data
-        )['messages'][0]['id']
+        )
 
     def mark_message_as_read(
             self,
             message_id: str
-    ) -> bool:
+    ) -> dict[str, bool]:
+        """
+        Mark a message as read.
+
+        Return example::
+
+            {'success': True}
+
+        Args:
+            message_id: The ID of the message to mark as read.
+
+        Returns:
+            The success of the operation.
+        """
         return self._make_request(
             method="POST",
-            endpoint=f"/messages",
+            endpoint=f"/{self.phone_id}/messages",
             json={
                 "messaging_product": "whatsapp",
                 "status": "read",
                 "message_id": message_id
             }
-        )["success"]
+        )
```

## pywa/client.py

```diff
@@ -1,14 +1,18 @@
 import collections
+import hashlib
+import mimetypes
+import os
 import requests
 from typing import Callable, Any, Iterable
 from pywa.api import WhatsAppCloudApi
 from pywa.handlers import Handler, MessageHandler, ButtonCallbackHandler, SelectionCallbackHandler, RawUpdateHandler, \
     MessageStatusHandler
-from pywa.types import InlineButton, SectionList, Message, CallbackButton, CallbackSelection, MessageStatus, Contact
+from pywa.types import InlineButton, SectionList, Message, CallbackButton, CallbackSelection, MessageStatus, Contact, \
+    MediaUrlResponse
 from pywa import webhook
 
 
 class WhatsApp:
     def __init__(
             self,
             phone_id: str | int,
@@ -245,25 +249,25 @@
         """
         if not keyboard:
             return self.api.send_text_message(
                 to=to,
                 text=text,
                 preview_url=preview_url,
                 reply_to_message_id=reply_to_message_id,
-            )
+            )['messages'][0]['id']
         return self.api.send_interactive_message(
             to=to,
             keyboard=keyboard,
             header={
                 "type": "text",
                 "text": header,
             } if header else None,
             body=text,
             footer=footer,
-        )
+        )['messages'][0]['id']
 
     def send_image(
             self,
             to: str,
             image: str | bytes,
             caption: str | None = None,
             reply_to_message_id: str | None = None,
@@ -297,30 +301,30 @@
         if not buttons:
             return self.api.send_media(
                 to=to,
                 media_id_or_url=image,
                 media_type="image",
                 reply_to_message_id=reply_to_message_id,
                 caption=caption,
-            )
+            )['messages'][0]['id']
         if not body and not caption:
             raise ValueError("Either body or caption must be provided when sending an image with buttons.")
         return self.api.send_interactive_message(
             to=to,
             keyboard=buttons,
             header={
                 "type": "image",
                 "image": {
                     "link" if image.startswith(("https://", "http://")) else "id": image,
                 }
             },
             body=body or caption,
             footer=footer,
             reply_to_message_id=reply_to_message_id,
-        )
+        )['messages'][0]['id']
 
     def send_video(
             self,
             to: str,
             video: str | bytes,
             caption: str | None = None,
             reply_to_message_id: str | None = None,
@@ -354,42 +358,42 @@
         if not buttons:
             return self.api.send_media(
                 to=to,
                 media_id_or_url=video,
                 media_type="video",
                 reply_to_message_id=reply_to_message_id,
                 caption=caption,
-            )
+            )['messages'][0]['id']
         if not body and not caption:
             raise ValueError("Either body or caption must be provided when sending a video with buttons.")
         return self.api.send_interactive_message(
             to=to,
             keyboard=buttons,
             header={
                 "type": "video",
                 "video": {
                     "link" if video.startswith(("https://", "http://")) else "id": video,
                 }
             },
             body=body or caption,
             footer=footer,
             reply_to_message_id=reply_to_message_id,
-        )
+        )['messages'][0]['id']
 
     def send_document(
             self,
             to: str,
             document: str | bytes,
             filename: str | None = None,
             caption: str | None = None,
             reply_to_message_id: str | None = None,
             buttons: list[InlineButton] | None = None,
             body: str | None = None,
             footer: str | None = None,
-    ):
+    ) -> str:
         """
         Send a document to a WhatsApp user.
 
         Example:
 
             >>> wa.send_document(
             ...     to="1234567890",
@@ -416,15 +420,15 @@
             return self.api.send_media(
                 to=to,
                 media_id_or_url=document,
                 media_type="document",
                 reply_to_message_id=reply_to_message_id,
                 filename=filename,
                 caption=caption,
-            )
+            )['messages'][0]['id']
         if not body and not caption:
             raise ValueError("Either body or caption must be provided when sending a document with buttons.")
         return self.api.send_interactive_message(
             to=to,
             keyboard=buttons,
             header={
                 "type": "document",
@@ -432,15 +436,15 @@
                     "link" if document.startswith(("https://", "http://")) else "id": document,
                     "filename": filename,
                 }
             },
             body=body or caption,
             footer=footer,
             reply_to_message_id=reply_to_message_id,
-        )
+        )['messages'][0]['id']
 
     def send_audio(
             self,
             to: str,
             audio: str | bytes,
             reply_to_message_id: str | None = None,
     ) -> str:
@@ -463,15 +467,15 @@
             The message ID of the sent message.
         """
         return self.api.send_media(
             to=to,
             media_id_or_url=audio,
             media_type="audio",
             reply_to_message_id=reply_to_message_id,
-        )
+        )['messages'][0]['id']
 
     def send_sticker(
             self,
             to: str,
             sticker: str | bytes,
             animated: bool = False,
             reply_to_message_id: str | None = None,
@@ -499,15 +503,15 @@
         """
         return self.api.send_media(
             to=to,
             media_id_or_url=sticker,
             media_type="sticker",
             reply_to_message_id=reply_to_message_id,
             animated=animated,
-        )
+        )['messages'][0]['id']
 
     def send_reaction(
             self,
             to: str,
             emoji: str,
             message_id: str,
     ) -> str:
@@ -530,15 +534,15 @@
         Returns:
             The message ID of the reaction.
         """
         return self.api.send_reaction(
             to=to,
             emoji=emoji,
             message_id=message_id,
-        )
+        )['messages'][0]['id']
 
     def remove_reaction(
             self,
             to: str,
             message_id: str,
     ) -> str:
         """
@@ -551,15 +555,15 @@
             ...     message_id='wamid.XXX='
             ... )
         """
         return self.api.send_reaction(
             to=to,
             message_id=message_id,
             emoji=""
-        )
+        )['messages'][0]['id']
 
     def send_location(
             self,
             to: str,
             latitude: float,
             longitude: float,
             name: str | None = None,
@@ -587,15 +591,15 @@
         """
         return self.api.send_location(
             to=to,
             latitude=latitude,
             longitude=longitude,
             name=name,
             address=address,
-        )
+        )['messages'][0]['id']
 
     def send_contact(
             self,
             to: str,
             contact: Contact | Iterable[Contact],
             reply_to_message_id: str | None = None,
     ) -> str:
@@ -623,23 +627,109 @@
         Returns:
             The message ID of the sent message.
         """
         return self.api.send_contacts(
             to=to,
             contacts=contact if isinstance(contact, Iterable) else [contact],
             reply_to_message_id=reply_to_message_id,
-        )
+        )['messages'][0]['id']
 
     def mark_message_as_read(
             self,
             message_id: str,
     ) -> bool:
         """
         Mark a message as read.
 
         Args:
             message_id: The message ID to mark as read.
 
         Returns:
             Whether the message was marked as read.
         """
-        return self.api.mark_message_as_read(message_id=message_id)
+        return self.api.mark_message_as_read(message_id=message_id)['success']
+
+    def upload_media(
+            self,
+            media: str | bytes,
+            mime_type: str | None = None,
+    ) -> str:
+        """
+        Upload media to WhatsApp servers.
+
+        Example:
+            >>> wa.upload_media(
+            ...     media='https://example.com/image.jpg',
+            ...     mime_type='image/jpeg',
+            ... )
+
+        Args:
+            media: The media to upload (either a URL or a file Path or bytes).
+            mime_type: The MIME type of the media (optional).
+
+        Returns:
+            The media ID.
+
+        Raises:
+            ValueError: If mime_type is not provided and cannot be guessed (e.g. for bytes or URLs without
+                Content-Type header).
+        """
+        return self.api.upload_media(
+            media=media,
+            mime_type=mime_type,
+        )['id']
+
+    def get_media_url(
+            self,
+            media_id: str
+    ) -> MediaUrlResponse:
+        """
+        Get the URL of a media.
+            - The URL is valid for 5 minutes.
+            - You can download with ``wa.download_media``.
+
+        Args:
+            media_id: The media ID.
+
+        Returns:
+            A MediaResponse object with the media URL.
+        """
+        res = self.api.get_media_url(media_id=media_id)
+        return MediaUrlResponse(
+            _client=self,
+            id=res['id'],
+            url=res['url'],
+            mime_type=res['mime_type'],
+            sha256=res['sha256'],
+            file_size=res['file_size'],
+        )
+
+    def download_media(
+            self,
+            url: str,
+            path: str | None = None,
+            filename: str | None = None,
+            in_memory: bool = False,
+    ) -> str | bytes:
+        """
+        Download a media file from WhatsApp servers.
+
+        Args:
+            url: The URL of the media file (from ``get_media_url``).
+            path: The path where to save the file (if not provided, the current working directory will be used).
+            filename: The name of the file (if not provided, it will be guessed from the URL + extension).
+            in_memory: Whether to return the file as bytes instead of saving it to disk (default: False).
+
+        Returns:
+            The path of the saved file if ``in_memory`` is False, the file as bytes otherwise.
+        """
+        content, mimetype = self.api.download_media(media_url=url)
+        if in_memory:
+            return content
+        if path is None:
+            path = os.getcwd()
+        if filename is None:
+            filename = hashlib.sha256(url.encode()).hexdigest() + mimetypes.guess_extension(mimetype)
+        path = os.path.join(path, filename)
+        with open(path, "wb") as f:
+            f.write(content)
+        return path
```

## pywa/types.py

```diff
@@ -8,14 +8,15 @@
     "MessageStatusType",
     "CallbackButton",
     "CallbackSelection",
     "InlineButton",
     "SectionRow",
     "Section",
     "SectionList",
+    "MediaUrlResponse"
 )
 
 from datetime import datetime
 from dataclasses import dataclass, field, asdict
 from enum import Enum
 from typing import TYPE_CHECKING, Iterable
 
@@ -143,21 +144,53 @@
 
     def __str__(self):
         return self.value
 
 
 @dataclass(frozen=True, slots=True)
 class MediaBase:
+    _client: WhatsApp = field(repr=False, hash=False, compare=False)
     id: str
     sha256: str
     mime_type: str
 
     @classmethod
-    def from_dict(cls, data: dict | None):
-        return cls(**data) if data else None
+    def from_dict(cls, client: WhatsApp, data: dict | None):
+        return cls(_client=client, **data) if data else None
+
+    def get_media_url(self) -> str:
+        """Gets the URL of the media. (expires after 5 minutes)"""
+        return self._client.get_media_url(media_id=self.id).url
+
+    def download(
+            self,
+            path: str | None = None,
+            filename: str | None = None,
+            in_memory: bool = False,
+    ) -> bytes | str:
+        """
+        Download a media file from WhatsApp servers.
+            - Same as ``WhatsApp.download_media(media_url=WhatsApp.get_media_url(media_id))``
+
+        >>> message.image.download()
+
+        Args:
+            path: The path where to save the file (if not provided, the current working directory will be used).
+            filename: The name of the file (if not provided, it will be guessed from the URL + extension).
+            in_memory: Whether to return the file as bytes instead of saving it to disk (default: False).
+
+        Returns:
+            The path of the saved file if ``in_memory`` is False, the file as bytes otherwise.
+        """
+        return self._client.download_media(
+            url=self.get_media_url(),
+            path=path,
+            filename=filename,
+            in_memory=in_memory
+        )
 
 
 @dataclass(frozen=True, slots=True)
 class Image(MediaBase):
     """
     Represents an image.
 
@@ -274,15 +307,66 @@
         """
         return utils.get_distance(
             lat1=self.latitude, lon1=self.longitude, lat2=other.latitude, lon2=other.longitude
         ) <= radius
 
 
 @dataclass(frozen=True, slots=True)
+class MediaUrlResponse:
+    """
+    Represents a media response.
+
+    Attributes:
+        id: The ID of the media.
+        url: The URL of the media (valid for 5 minutes).
+        mime_type: The MIME type of the media.
+        sha256: The SHA256 hash of the media.
+        file_size: The size of the media in bytes.
+    """
+    _client: WhatsApp = field(repr=False, hash=False, compare=False)
+    id: str
+    url: str
+    mime_type: str
+    sha256: str
+    file_size: int
+
+    def download(
+            self,
+            filepath: str | None = None,
+            filename: str | None = None,
+            in_memory: bool = False,
+    ) -> bytes | str:
+        """
+        Download a media file from WhatsApp servers.
+
+        Args:
+            filepath: The path where to save the file (if not provided, the current working directory will be used).
+            filename: The name of the file (if not provided, it will be guessed from the URL + extension).
+            in_memory: Whether to return the file as bytes instead of saving it to disk (default: False).
+
+        Returns:
+            The path of the saved file if ``in_memory`` is False, the file as bytes otherwise.
+        """
+        return self._client.download_media(url=self.url, path=filepath, filename=filename, in_memory=in_memory)
+
+
+@dataclass(frozen=True, slots=True)
 class Contact:
+    """
+    Represents a contact.
+
+    Attributes:
+        name: The name of the contact.
+        birthday: The birthday of the contact (in ``YYYY-MM-DD`` format, optional).
+        phones: The phone numbers of the contact.
+        emails: The email addresses of the contact.
+        urls: The URLs of the contact.
+        addresses: The addresses of the contact.
+        org: The organization of the contact (optional).
+    """
     name: Name
     birthday: str | None = None
     phones: list[Phone] = field(default_factory=list)
     emails: list[Email] = field(default_factory=list)
     urls: list[Url] = field(default_factory=list)
     addresses: list[Address] = field(default_factory=list)
     org: Org | None = None
@@ -308,61 +392,116 @@
             "urls": [asdict(url) for url in self.urls],
             "addresses": [asdict(address) for address in self.addresses],
             "org": asdict(self.org) if self.org else None,
         }
 
     @dataclass(frozen=True, slots=True)
     class Name:
+        """
+        Represents a contact's name.
+
+        - At least one of the optional parameters needs to be included along with the formatted_name parameter.
+
+        Attributes:
+            formatted_name: The formatted name of the contact.
+            first_name: The first name of the contact (optional).
+            last_name: The last name of the contact (optional).
+            middle_name: The middle name of the contact (optional).
+            suffix: The suffix of the contact (optional).
+            prefix: The prefix of the contact (optional).
+        """
         formatted_name: str
         first_name: str | None = None
         last_name: str | None = None
         middle_name: str | None = None
         suffix: str | None = None
         prefix: str | None = None
 
     @dataclass(frozen=True, slots=True)
     class Phone:
+        """
+        Represents a contact's phone number.
+
+        Attributes:
+            phone: The phone number (If ``wa_id`` is provided, No need for the ``phone``).
+            type: The type of the phone number (Standard Values are CELL, MAIN, IPHONE, HOME, and WORK. optional).
+            wa_id: The WhatsApp ID of the contact (optional).
+        """
         phone: str | None = None
         type: str | None = None
         wa_id: str | None = None
 
         @classmethod
         def from_dict(cls, data: dict | None):
             return cls(**data) if data else None
 
     @dataclass(frozen=True, slots=True)
     class Email:
+        """
+        Represents a contact's email address.
+
+        Attributes:
+            email: The email address.
+            type: The type of the email address (Standard Values are WORK and HOME. optional).
+        """
         email: str | None = None
         type: str | None = None
 
         @classmethod
         def from_dict(cls, data: dict | None):
             return cls(**data) if data else None
 
     @dataclass(frozen=True, slots=True)
     class Url:
+        """
+        Represents a contact's URL.
+
+        Attributes:
+            url: The URL.
+            type: The type of the URL (Standard Values are WORK and HOME. optional).
+        """
         url: str | None = None
         type: str | None = None
 
         @classmethod
         def from_dict(cls, data: dict | None):
             return cls(**data) if data else None
 
     @dataclass(frozen=True, slots=True)
     class Org:
+        """
+        Represents a contact's organization.
+
+        Attributes:
+            company: The company of the contact (optional).
+            department: The department of the contact (optional).
+            title: The title of the business contact (optional).
+        """
         company: str | None = None
         department: str | None = None
         title: str | None = None
 
         @classmethod
         def from_dict(cls, data: dict | None):
             return cls(**data) if data else None
 
     @dataclass(frozen=True, slots=True)
     class Address:
+        """
+        Represents a contact's address.
+
+        Attributes:
+            street: The street number and name of the address (optional).
+            city: The city name of the address (optional).
+            state: State abbreviation.
+            zip: Zip code of the address (optional).
+            country: Full country name.
+            country_code: Two-letter country abbreviation (e.g. US, GB, IN. optional).
+            type: The type of the address (Standard Values are WORK and HOME. optional).
+        """
         street: str | None = None
         city: str | None = None
         state: str | None = None
         zip: str | None = None
         country: str | None = None
         country_code: str | None = None
         type: str | None = None
@@ -403,14 +542,15 @@
     """
     display_phone_number: str
     phone_number_id: str
 
 
 @dataclass(frozen=True, slots=True)
 class BaseUpdate:
+    """Base class for all update types."""
     _client: WhatsApp = field(repr=False, hash=False, compare=False)
     id: str
     metadata: Metadata
     from_user: User
     timestamp: datetime
 
     @property
@@ -737,24 +877,49 @@
             id=message['id'],
             type=msg_type,
             from_user=User.from_dict(value['contacts'][0]),
             timestamp=datetime.fromtimestamp(int(message['timestamp'])),
             metadata=Metadata(**value['metadata']),
             reply_to_message=ReplyToMessage.from_dict(message.get('context')),
             text=message['text']['body'] if 'text' in message else None,
-            image=Image.from_dict(message.get('image')),
-            video=Video.from_dict(message.get('video')),
-            sticker=Sticker.from_dict(message.get('sticker')),
-            document=Document.from_dict(message.get('document')),
-            audio=Audio.from_dict(message.get('audio')),
+            image=Image.from_dict(client=client, data=message.get('image')),
+            video=Video.from_dict(client=client, data=message.get('video')),
+            sticker=Sticker.from_dict(client=client, data=message.get('sticker')),
+            document=Document.from_dict(client=client, data=message.get('document')),
+            audio=Audio.from_dict(client=client, data=message.get('audio')),
             reaction=Reaction.from_dict(message.get('reaction')),
             location=Location.from_dict(message.get('location')),
             contacts=[Contact.from_dict(contact) for contact in message.get('contacts', [])] or None
         )
 
+    def download_media(
+            self,
+            filepath: str | None = None,
+            filename: str | None = None,
+            in_memory: bool = False,
+    ) -> str | bytes:
+        """
+        Download a media file from WhatsApp servers (image, video, sticker, document or audio).
+
+        Args:
+            filepath: The path where to save the file (if not provided, the current working directory will be used).
+            filename: The name of the file (if not provided, it will be guessed from the URL + extension).
+            in_memory: Whether to return the file as bytes instead of saving it to disk (default: False).
+
+        Returns:
+            The path of the saved file if ``in_memory`` is False, the file as bytes otherwise.
+
+        Raises:
+            ValueError: If the message does not contain any media.
+        """
+        media = self.image or self.video or self.sticker or self.document or self.audio
+        if not media:
+            raise ValueError('The message does not contain any media.')
+        return media.download(path=filepath, filename=filename, in_memory=in_memory)
+
 
 @dataclass(frozen=True, slots=True)
 class CallbackButton(BaseUpdate):
     """
     Represents a callback button.
 
     Attributes:
```

## pywa/webhook.py

```diff
@@ -31,18 +31,18 @@
                         return flask.request.args.get("hub.challenge"), 200
                     else:
                         return "Error, invalid verification token", 403
                 elif flask.request.method == "POST":
                     if flask.request.json["entry"][0]["changes"][0]["value"]["metadata"]["phone_number_id"] \
                             == wa_client.phone_id:
                         for raw_update_handler in wa_client._handlers["raw_update"]:
-                            raw_update_handler(self, flask.request.json)
+                            raw_update_handler(wa_client, flask.request.json)
                         update, key = convert_dict_to_update(client=wa_client, d=flask.request.json)
                         for handler in wa_client._handlers[key]:  # TODO execute in parallel
-                            handler(self, update)
+                            handler(wa_client, update)
                     return "ok", 200
 
         elif utils.is_fastapi_app(app):
             import fastapi
 
             @app.middleware("http")
             async def before_request(request: fastapi.Request, call_next: Callable):
@@ -54,18 +54,18 @@
                     else:
                         return fastapi.Response(content="Error, invalid verification token", status_code=403)
                 elif request.method == "POST":
                     request_body = await request.json()
                     if request_body["entry"][0]["changes"][0]["value"]["metadata"]["phone_number_id"] \
                             == wa_client.phone_id:
                         for raw_update_handler in wa_client._handlers["raw_update"]:
-                            raw_update_handler(self, request_body)
+                            raw_update_handler(wa_client, request_body)
                         update, key = convert_dict_to_update(client=wa_client, d=request_body)
                         for handler in wa_client._handlers[key]:  # TODO execute in parallel
-                            handler(self, update)
+                            handler(wa_client, update)
                     return fastapi.Response(content="ok", status_code=200)
                 return await call_next(request)
 
         else:
             raise ValueError("The app must be a Flask or FastAPI app.")
```

## Comparing `pywa-0.0.1rc7.dist-info/LICENSE` & `pywa-0.0.1rc8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pywa-0.0.1rc7.dist-info/RECORD` & `pywa-0.0.1rc8.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-pywa/__init__.py,sha256=17F_xdmkNPv_gvpm8tTxkf6YQb__7Di_HokVTzCR3uU,143
-pywa/api.py,sha256=smTijxsjGP_6rMOey4Wq6KVfaFz4LVmmxI_B9C2Af2g,7965
-pywa/client.py,sha256=KspV7b-2PbtE_wl3MpVEit3ABn1R8Om1q4c-aJ_atn0,23158
+pywa/__init__.py,sha256=Fr6IdoF7QKBhoumRqAUgkI-5iHb5-dIWbjJSBWOm2-w,143
+pywa/api.py,sha256=jnP9iAxnW86f1VTndPsvR8aaFglswnrRhXCFbLOvhxg,14911
+pywa/client.py,sha256=YcqpjdvynYlBQDbFbXcbwStk3NXagemyZjy4U-3HA5k,26284
 pywa/errors.py,sha256=Vs5SJehEt5PhUrJBbia710gpusoxmTPQmlgDBBnYpWM,989
 pywa/filters.py,sha256=uDkVr9cyJRmEMF9GSoKhUdQZm4I4h3-Q2r4kdJ0dJyU,11021
 pywa/handlers.py,sha256=Z4j2jiEwQ0_mzlcybHFDmRg7OR8agakXXkzU85eQyGk,1464
-pywa/types.py,sha256=eBBbdMCCT4kcTjVFkFWLeoUAJSTpxapvdqn1Qm80MeI,25776
+pywa/types.py,sha256=rz7rPpk31e0zKAGy_qj8Sp04JAvWyWJNcqhjSH3dj4w,32258
 pywa/utils.py,sha256=GRTfSvmsuOBd1_Yw2c90XoALqVPuy6HzyvJuqg3xjtI,991
-pywa/webhook.py,sha256=mOE-EZ89bxHht-AyzUYO0ANjKW5MGSl3bxLdNrQt188,4141
-pywa-0.0.1rc7.dist-info/LICENSE,sha256=RwljuP8WgWttLkSivccHoHEFSDhOY8aLM_vg6Ix48yQ,1066
-pywa-0.0.1rc7.dist-info/METADATA,sha256=RRa75AFf6_GnJRH50nbRlnTJlg7wznXI-sl-2QZfIgQ,10203
-pywa-0.0.1rc7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pywa-0.0.1rc7.dist-info/top_level.txt,sha256=Cl24ggXVvxvOUnQfKRASer1LzHxpYCPZd5ZcVyS98Oo,5
-pywa-0.0.1rc7.dist-info/RECORD,,
+pywa/webhook.py,sha256=NCJpIrUssm5XXKeRpgupG2GSx38NoTzObKojN-3yMvQ,4161
+pywa-0.0.1rc8.dist-info/LICENSE,sha256=RwljuP8WgWttLkSivccHoHEFSDhOY8aLM_vg6Ix48yQ,1066
+pywa-0.0.1rc8.dist-info/METADATA,sha256=eu_RgdgeWpfODIZwGj8kJU2lYRywjta-yT_iK90TXoI,4489
+pywa-0.0.1rc8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pywa-0.0.1rc8.dist-info/top_level.txt,sha256=Cl24ggXVvxvOUnQfKRASer1LzHxpYCPZd5ZcVyS98Oo,5
+pywa-0.0.1rc8.dist-info/RECORD,,
```


# Comparing `tmp/pywa-0.0.1rc15-py3-none-any.whl.zip` & `tmp/pywa-0.0.1rc16-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 27715 bytes, number of entries: 15
+Zip file size: 28295 bytes, number of entries: 15
 -rw-rw-r--  2.0 unx      117 b- defN 23-Jun-27 07:52 pywa/__init__.py
--rw-rw-r--  2.0 unx       26 b- defN 23-Jul-04 09:54 pywa/__version__.py
+-rw-rw-r--  2.0 unx       26 b- defN 23-Jul-07 08:22 pywa/__version__.py
 -rw-rw-r--  2.0 unx    14991 b- defN 23-Jul-03 08:35 pywa/api.py
 -rw-rw-r--  2.0 unx    26847 b- defN 23-Jul-03 08:42 pywa/client.py
 -rw-rw-r--  2.0 unx     7191 b- defN 23-Jul-03 08:28 pywa/errors.py
--rw-rw-r--  2.0 unx    20873 b- defN 23-Jul-04 09:51 pywa/filters.py
+-rw-rw-r--  2.0 unx    20703 b- defN 23-Jul-04 19:49 pywa/filters.py
 -rw-rw-r--  2.0 unx     1794 b- defN 23-Jul-02 08:19 pywa/handlers.py
--rw-rw-r--  2.0 unx    34447 b- defN 23-Jul-02 08:21 pywa/types.py
+-rw-rw-r--  2.0 unx    39628 b- defN 23-Jul-07 08:18 pywa/types.py
 -rw-rw-r--  2.0 unx      991 b- defN 23-Jun-20 16:58 pywa/utils.py
 -rw-rw-r--  2.0 unx     4613 b- defN 23-Jul-03 08:35 pywa/webhook.py
--rw-rw-r--  2.0 unx     1066 b- defN 23-Jul-04 09:54 pywa-0.0.1rc15.dist-info/LICENSE
--rw-rw-r--  2.0 unx     4387 b- defN 23-Jul-04 09:54 pywa-0.0.1rc15.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-04 09:54 pywa-0.0.1rc15.dist-info/WHEEL
--rw-rw-r--  2.0 unx        5 b- defN 23-Jul-04 09:54 pywa-0.0.1rc15.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1106 b- defN 23-Jul-04 09:54 pywa-0.0.1rc15.dist-info/RECORD
-15 files, 118546 bytes uncompressed, 25933 bytes compressed:  78.1%
+-rw-rw-r--  2.0 unx     1066 b- defN 23-Jul-07 08:22 pywa-0.0.1rc16.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     4387 b- defN 23-Jul-07 08:22 pywa-0.0.1rc16.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-07 08:22 pywa-0.0.1rc16.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jul-07 08:22 pywa-0.0.1rc16.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1106 b- defN 23-Jul-07 08:22 pywa-0.0.1rc16.dist-info/RECORD
+15 files, 123557 bytes uncompressed, 26513 bytes compressed:  78.5%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: pywa/utils.py
 Comment: 
 
 Filename: pywa/webhook.py
 Comment: 
 
-Filename: pywa-0.0.1rc15.dist-info/LICENSE
+Filename: pywa-0.0.1rc16.dist-info/LICENSE
 Comment: 
 
-Filename: pywa-0.0.1rc15.dist-info/METADATA
+Filename: pywa-0.0.1rc16.dist-info/METADATA
 Comment: 
 
-Filename: pywa-0.0.1rc15.dist-info/WHEEL
+Filename: pywa-0.0.1rc16.dist-info/WHEEL
 Comment: 
 
-Filename: pywa-0.0.1rc15.dist-info/top_level.txt
+Filename: pywa-0.0.1rc16.dist-info/top_level.txt
 Comment: 
 
-Filename: pywa-0.0.1rc15.dist-info/RECORD
+Filename: pywa-0.0.1rc16.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pywa/__version__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.1rc15"
+__version__ = "0.0.1rc16"
```

## pywa/filters.py

```diff
@@ -1,12 +1,16 @@
 """Usefully filters to use in your handlers."""
 from __future__ import annotations
 
 __all__ = (
-    "FilterCombine",
+    "all_",
+    "any_",
+    "not_",
+    "FORWARDED",
+    "from_user",
     "TextFilter",
     "ImageFilter",
     "VideoFilter",
     "AudioFilter",
     "DocumentFilter",
     "StickerFilter",
     "ReactionFilter",
@@ -30,126 +34,119 @@
     MessageT: TypeAlias = Callable[[Wa, Msg], bool]
     CallbackT: TypeAlias = Callable[[Wa, CallbackButton | CallbackSelection], bool]
     MessageStatusT: TypeAlias = Callable[[Wa, Ms], bool]
 
 T = TypeVar("T")
 
 
-class FilterCombine:
-    """
-    Combine filters with ``and`` & ``or`` like operators.
+FORWARDED: MessageT = lambda wa, m: m.forwarded
+"""
+Filter for forwarded messages.
+
+>>> filters.FORWARDED
+"""
 
-    If you need to combine filters with ``and`` or ``or``, use ``FilterCombine.all`` or ``FilterCombine.any``.
 
-    Here are some examples:
+def all_(*filters: Callable[[Wa, T], bool]) -> Callable[[Wa, T], bool]:
+    """
+    Filter for messages that pass all the given filters.
 
-    >>> from pywa.filters import FilterCombine as FC  # short name for convenience
+    >>> all_(TextFilter.startswith("World"), TextFilter.contains("Word"))
+    """
+    return lambda wa, m: all(f(wa, m) for f in filters)
 
-    Matches messages that start with "Hello" and end with "World" or have a length between 1 and 10:
 
-    >>> FC.all(TextFilter.startswith("Hello"), FC.any(TextFilter.endswith("World"), TextFilter.length((1, 10))))
+def any_(*filters: Callable[[Wa, T], bool]) -> Callable[[Wa, T], bool]:
+    """
+    Filter for messages that pass any of the given filters.
 
-    Matches messages that are either images or videos with a caption:
+    >>> any_(TextFilter.contains("Hello"), TextFilter.contains("World"))
+    """
+    return lambda wa, m: any(f(wa, m) for f in filters)
 
-    >>> FC.any(ImageFilter.ANY, FC.all(VideoFilter.mimetype("video/mp4"), VideoFilter.HAS_CAPTION))
 
-    Keep in mind that all macth-filters (``match``, ``startswith``, ``endswith``, ``contains`` etc.) returns True if
-    any of the given matches are found. so there is no need to use ``FC.any`` with them.
+def not_(fil: Callable[[Wa, T], bool]) -> Callable[[Wa, T], bool]:
     """
+    Filter for messages that don't pass the given filter.
 
-    @staticmethod
-    def all(*filters: Callable[[Wa, T], bool]) -> Callable[[Wa, T], bool]:
-        """
-        Filter for messages that pass all the given filters.
+    >>> not_(TextFilter.contains("Hello"))
+    """
+    return lambda wa, m: not fil(wa, m)
 
-        >>> FilterCombine.all(TextFilter.startswith("World"), TextFilter.contains("Word"))
-        """
-        return lambda wa, m: all(f(wa, m) for f in filters)
 
-    @staticmethod
-    def any(*filters: Callable[[Wa, T], bool]) -> Callable[[Wa, T], bool]:
-        """
-        Filter for messages that pass any of the given filters.
+def from_user(*numbers: str) -> MessageT:
+    """
+    Filter for messages that are sent from the given numbers.
+        - Aliases: ``from_users``, ``from_numbers``, ``from_number``
 
-        >>> FilterCombine.any(TextFilter.contains("Hello"), TextFilter.contains("World"))
-        """
-        return lambda wa, m: any(f(wa, m) for f in filters)
+    >>> filters.from_user("1234567890", "0987654321")
+    """
+    only_nums_pattern = re.compile(r"\D")
+    numbers = tuple(re.sub(only_nums_pattern, "", n) for n in numbers)
+    return lambda wa, m: m.from_user.wa_id in numbers
+
+
+from_users = from_user  # alias
+from_number = from_user  # alias
+from_numbers = from_user  # alias
 
 
 class _BaseUpdateFilter:
 
     __message_types__: tuple[Mt, ...] = ()
     
     @classmethod
     def _match_type(cls, m: Msg) -> bool:
         return m.type in cls.__message_types__
 
-    @classmethod
-    def from_user(cls, *numbers: str) -> MessageT:
-        """
-        Filter for messages that are sent from the given numbers.
-            - Aliases: ``from_numbers``, ``from_number``
-
-        >>> TextFilter.from_user("1234567890", "0987654321")
-        """
-        only_nums_pattern = re.compile(r"\D")
-        numbers = tuple(re.sub(only_nums_pattern, "", n) for n in numbers)
-        return lambda wa, m: cls._match_type(m) and any(n == m.from_user.wa_id for n in numbers)
-
-    from_users = from_user  # alias
-    from_number = from_user  # alias
-    from_numbers = from_user  # alias
-
 
-class _UpdateWithForwardedFilter(_BaseUpdateFilter):
-    FORWARDED: MessageT = lambda wa, m: m.forwarded
-    """Filter for forwarded messages."""
-
-
-class _MediaFilter(_UpdateWithForwardedFilter):
+class _MediaFilter(_BaseUpdateFilter):
 
     @classmethod
-    def mimetype(cls, *mime_types: str) -> MessageT:
+    def mimetype(cls, *mimetypes: str) -> MessageT:
         """
         Filter for media messages that match any of the given mime types.
-        See https://developers.facebook.com/docs/whatsapp/cloud-api/reference/media#supported-media-types
-
             - Aliases: ``mimetypes``, ``mime_type``, ``mime_types``
+            - See https://developers.facebook.com/docs/whatsapp/cloud-api/reference/media#supported-media-types
 
-        >>> ImageFilter.mimetype("image/png")
-        >>> VideoFilter.mimetypes("video/mp4", "video/3gpp")
-        >>> AudioFilter.mimetypes("audio/mpeg", "audio/ogg")
-        >>> DocumentFilter.mimetypes("application/pdf", "application/msword")
-        >>> StickerFilter.mime_type("image/webp")
+        >>> ImageFilter.mimetype("image/png", "image/jpeg")
         """
         return lambda wa, m: cls._match_type(m) and any(
-            t == getattr(m, cls.__message_types__[0].value).mime_type for t in mime_types
+            t == getattr(m, cls.__message_types__[0].value).mime_type for t in mimetypes
         )
 
     mimetypes = mimetype  # alias
     mime_type = mimetype  # alias
     mime_types = mimetype  # alias
 
 
 class _MediaWithCaptionFilter(_MediaFilter):
     @classmethod
     def _has_caption(cls, wa: Wa, m: Msg) -> bool:
-        return m.type == cls.__message_types__[0] and m.caption is not None
+        return cls._match_type(m) and m.caption is not None
 
     HAS_CAPTION: MessageT = _has_caption
-    """Filter for media messages that have a caption."""
+    """
+    Filter for media messages that have a caption.
+    
+    >>> ImageFilter.HAS_CAPTION
+    """
 
 
-class TextFilter(_UpdateWithForwardedFilter):
+class TextFilter(_BaseUpdateFilter):
     """Useful filters for text messages."""
     
     __message_types__ = (Mt.TEXT,)
 
     ANY: MessageT = lambda wa, m: m.type == Mt.TEXT
-    """Filter for all text messages."""
+    """
+    Filter for all text messages.
+    
+    >>> TextFilter.ANY
+    """
 
     @staticmethod
     def match(*matches: str, ignore_case: bool = False) -> MessageT:
         """
         Filter for text messages that match exactly the given text/s.
             - Aliases: ``same_as``, ``matches``, ``equals``
 
@@ -279,72 +276,112 @@
 
 class ImageFilter(_MediaWithCaptionFilter):
     """Useful filters for image messages."""
 
     __message_types__ = (Mt.IMAGE,)
 
     ANY: MessageT = lambda wa, m: ImageFilter._match_type(m)
-    """Filter for all image messages."""
+    """
+    Filter for all image messages.
+    
+    >>> ImageFilter.ANY
+    """
 
 
 class VideoFilter(_MediaWithCaptionFilter):
     """Useful filters for video messages."""
 
     __message_types__ = (Mt.VIDEO,)
 
     ANY: MessageT = lambda wa, m: VideoFilter._match_type(m)
-    """Filter for all video messages."""
+    """
+    Filter for all video messages.
+    
+    >>> VideoFilter.ANY
+    """
 
 
 class DocumentFilter(_MediaWithCaptionFilter):
     """Useful filters for document messages."""
 
     __message_types__ = (Mt.DOCUMENT,)
 
     ANY: MessageT = lambda wa, m: DocumentFilter._match_type(m)
-    """Filter for all document messages."""
+    """
+    Filter for all document messages.
+    
+    >>> DocumentFilter.ANY
+    """
 
 
 class AudioFilter(_MediaFilter):
     """Useful filters for audio messages."""
 
     __message_types__ = (Mt.AUDIO,)
 
     ANY: MessageT = lambda wa, m: AudioFilter._match_type(m)
-    """Filter for all audio messages."""
+    """
+    Filter for all audio messages (voice notes and audio files).
+    
+    >>> AudioFilter.ANY
+    """
 
     VOICE: MessageT = lambda wa, m: AudioFilter._match_type(m) and m.audio.voice
-    """Filter for audio messages that are voice notes."""
+    """
+    Filter for audio messages that are voice notes.
+    
+    >>> AudioFilter.VOICE
+    """
 
     AUDIO: MessageT = lambda wa, m: AudioFilter._match_type(m) and not m.audio.voice
-    """Filter for audio messages that are audio files."""
+    """
+    Filter for audio messages that are audio files.
+    
+    >>> AudioFilter.AUDIO
+    """
 
 
 class StickerFilter(_MediaFilter):
     """Useful filters for sticker messages."""
 
     __message_types__ = (Mt.STICKER,)
 
     ANY: MessageT = lambda wa, m: StickerFilter._match_type(m)
-    """Filter for all sticker messages."""
+    """
+    Filter for all sticker messages.
+    
+    >>> StickerFilter.ANY
+    """
 
     ANIMATED: MessageT = lambda wa, m: StickerFilter._match_type(m) and m.sticker.animated
-    """Filter for animated sticker messages."""
+    """
+    Filter for animated sticker messages.
+    
+    >>> StickerFilter.ANIMATED
+    """
 
     STATIC: MessageT = lambda wa, m: StickerFilter._match_type(m) and not m.sticker.animated
-    """Filter for static sticker messages."""
+    """
+    Filter for static sticker messages.
+    
+    >>> StickerFilter.STATIC
+    """
 
 
-class LocationFilter(_UpdateWithForwardedFilter):
+class LocationFilter(_BaseUpdateFilter):
     """Useful filters for location messages."""
 
     __message_types__ = (Mt.LOCATION,)
 
     ANY: MessageT = lambda wa, m: LocationFilter._match_type(m)
-    """Filter for all location messages."""
+    """
+    Filter for all location messages.
+    
+    >>> LocationFilter.ANY
+    """
 
     @staticmethod
     def in_radius(lat: float, lon: float, radius: float | int) -> MessageT:
         """
         Filter for location messages that are in a given radius.
 
         >>> LocationFilter.in_radius(lat=37.48508108998884, lon=-122.14744733542707, radius=1)
@@ -366,21 +403,33 @@
 
 class ReactionFilter(_BaseUpdateFilter):
     """Useful filters for reaction messages."""
 
     __message_types__ = (Mt.REACTION,)
 
     ANY: MessageT = lambda wa, m: ReactionFilter._match_type(m)
-    """Filter for all reaction updates (added or removed)."""
+    """
+    Filter for all reaction updates (added or removed).
+    
+    >>> ReactionFilter.ANY
+    """
 
     ADDED: MessageT = lambda wa, m: ReactionFilter._match_type(m) and m.reaction.emoji is not None
-    """Filter for reaction messages that were added."""
+    """
+    Filter for reaction messages that were added.
+    
+    >>> ReactionFilter.ADDED
+    """
 
     REMOVED: MessageT = lambda wa, m: ReactionFilter._match_type(m) and m.reaction.emoji is None
-    """Filter for reaction messages that were removed."""
+    """
+    Filter for reaction messages that were removed.
+    
+    >>> ReactionFilter.REMOVED
+    """
 
     @staticmethod
     def emoji(*emojis: str) -> MessageT:
         """
         Filter for custom reaction messages. pass emojis as strings.
             - Aliases: ``emojis``, ``reaction``, ``reactions``
 
@@ -389,21 +438,25 @@
         return lambda wa, m: ReactionFilter._match_type(m) and m.reaction.emoji in emojis
 
     emojis = emoji  # alias
     reaction = emoji  # alias
     reactions = emoji  # alias
 
 
-class ContactsFilter(_UpdateWithForwardedFilter):
+class ContactsFilter(_BaseUpdateFilter):
     """Useful filters for contact messages."""
 
     __message_types__ = (Mt.CONTACTS,)
 
     ANY: MessageT = lambda wa, m: ContactsFilter._match_type(m)
-    """Filter for all contacts messages."""
+    """
+    Filter for all contacts messages.
+    
+    >>> ContactsFilter.ANY
+    """
 
     HAS_WA: MessageT = lambda wa, m: ContactsFilter._match_type(m) and (
         any((p.wa_id for p in (phone for contact in m.contacts for phone in contact.phones)))
     )
     """Filter for contacts messages that have a WhatsApp account."""
 
     @staticmethod
@@ -441,24 +494,32 @@
 
 class UnsupportedMsgFilter(_BaseUpdateFilter):
     """Useful filters for unsupported messages."""
 
     __message_types__ = (Mt.UNSUPPORTED,)
 
     ANY: MessageT = lambda wa, m: m.type == Mt.UNSUPPORTED
-    """Filter for all unsupported messages."""
+    """
+    Filter for all unsupported messages.
+    
+    >>> UnsupportedMsgFilter.ANY
+    """
 
 
 class CallbackFilter(_BaseUpdateFilter):
     """Useful filters for callback queries."""
 
     __message_types__ = (Mt.INTERACTIVE,)
 
     ANY: CallbackT = lambda wa, c: True
-    """Filter for all callback queries (the default)."""
+    """
+    Filter for all callback queries (the default).
+    
+    >>> CallbackFilter.ANY
+    """
 
     @staticmethod
     def data_match(*matches: str, ignore_case: bool = False) -> CallbackT:
         """
         Filter for callbacks their data match exactly the given string/s.
             - Aliases: ``data_equals``, ``data_matches``, ``data_same_as``
 
@@ -540,24 +601,40 @@
 
 class MessageStatusFilter(_BaseUpdateFilter):
     """Useful filters for message status updates."""
 
     __message_types__ = (Mt.MESSAGE_STATUS,)
 
     SENT: MessageStatusT = lambda wa, data: data.status == Mst.SENT
-    """Filter for messages that have been sent."""
+    """
+    Filter for messages that have been sent.
+    
+    >>> MessageStatusFilter.SENT
+    """
 
     DELIVERED: MessageStatusT = lambda wa, data: data.status == Mst.DELIVERED
-    """Filter for messages that have been delivered."""
+    """
+    Filter for messages that have been delivered.
+    
+    >>> MessageStatusFilter.DELIVERED
+    """
 
     READ: MessageStatusT = lambda wa, data: data.status == Mst.READ
-    """Filter for messages that have been read."""
+    """
+    Filter for messages that have been read.
+    
+    >>> MessageStatusFilter.READ
+    """
 
     FAILED: MessageStatusT = lambda wa, data: data.status == Mst.FAILED
-    """Filter for messages that have failed to send (than you can access to the ``error`` attribute)."""
+    """
+    Filter for messages that have failed to send (than you can access to the ``error`` attribute).
+    
+    >>> MessageStatusFilter.FAILED
+    """
 
     @staticmethod
     def failed_with_error_code(*codes: int) -> MessageStatusT:
         """
         Filter for messages that have failed to send with the given error code/s.
             - Aliases: ``failed_with_error_codes``
```

## pywa/types.py

```diff
@@ -147,18 +147,18 @@
     def __str__(self):
         return self.value
 
 
 @dataclass(frozen=True, slots=True, kw_only=True)
 class _FromDict:
     """Base class for dataclasses that can be created from dict unpacking."""
+
     # noinspection PyArgumentList
     @classmethod
     def from_dict(cls, **kwargs):
-
         return cls(**{
             k: v for k, v in kwargs.items()
             if k in (f.name for f in fields(cls))
         })
 
 
 @dataclass(frozen=True, slots=True)
@@ -825,28 +825,30 @@
         id: The message ID.
         metadata: The metadata of the message (to which phone number it was sent).
         type: The message type (text, image, video, etc).
         from_user: The user who sent the message.
         timestamp: The timestamp when the message was sent.
         reply_to_message: The message to which this message is a reply to. (optional)
         forwarded: Whether the message was forwarded.
+        forwarded_many_times: Whether the message was forwarded many times. (when True, ``forwarded`` will be True as well)
         text: The text of the message (if the message type is text). (optional)
         image: The image of the message (if the message type is image). (optional)
         video: The video of the message (if the message type is video). (optional)
         sticker: The sticker of the message (if the message type is sticker). (optional)
         document: The document of the message (if the message type is document). (optional)
         audio: The audio of the message (if the message type is audio). (optional)
         caption: The caption of the message (if the message type is image, video, or document). (optional)
         reaction: The reaction of the message (if the message type is reaction). (optional)
         location: The location of the message (if the message type is location). (optional)
         contacts: The contacts of the message (if the message type is contacts). (optional)
         error: The error of the message (if the message type is `unsupported`). (optional)
     """
     reply_to_message: ReplyToMessage | None
     forwarded: bool
+    forwarded_many_times: bool
     text: str | None
     image: Image | None
     video: Video | None
     sticker: Sticker | None
     document: Document | None
     audio: Audio | None
     caption: str | None
@@ -859,22 +861,24 @@
     def message_id_to_reply(self) -> str:
         """The ID of the message to reply to."""
         return self.id if self.type != MessageType.REACTION else self.reaction.message_id
 
     @classmethod
     def from_dict(cls, client: WhatsApp, value: dict) -> Message:
         message = value['messages'][0]
+        context = message.get('context')
         return cls(
             _client=client,
             id=message['id'],
             type=MessageType(message['type']),
             from_user=User.from_dict(value['contacts'][0]),
             timestamp=datetime.fromtimestamp(int(message['timestamp'])),
             metadata=Metadata.from_dict(**value['metadata']),
-            forwarded=message.get('context', {}).get('forwarded', False),
+            forwarded=any(context.get(key) for key in ('forwarded', 'frequently_forwarded')) if context else False,
+            forwarded_many_times=context.get('frequently_forwarded', False) if context else False,
             reply_to_message=ReplyToMessage.from_dict(message.get('context')),
             text=message['text']['body'] if 'text' in message else None,
             image=Image.from_dict(_client=client, **message.get('image')) if 'image' in message else None,
             video=Video.from_dict(_client=client, **message.get('video')) if 'video' in message else None,
             sticker=Sticker.from_dict(_client=client, **message.get('sticker')) if 'sticker' in message else None,
             document=Document.from_dict(_client=client, **message.get('document')) if 'document' in message else None,
             audio=Audio.from_dict(_client=client, **message.get('audio')) if 'audio' in message else None,
@@ -907,14 +911,126 @@
             ValueError: If the message does not contain any media.
         """
         media = self.image or self.video or self.sticker or self.document or self.audio
         if not media:
             raise ValueError('The message does not contain any media.')
         return media.download(path=filepath, filename=filename, in_memory=in_memory)
 
+    def copy(
+            self,
+            to: str,
+            reply_to_message_id: str = None,
+            preview_url: bool = False,
+            keyboard: list[InlineButton] | SectionList | None = None,
+            header: str | None = None,
+            body: str | None = None,
+            footer: str | None = None,
+    ) -> str:
+        """
+        Copy incoming message to another chat
+            - The WhatsApp Cloud API does not offer a `real` forward option so this is just copy the message content.
+
+        Args:
+            to: The phone ID of the WhatsApp user to copy the message to.
+            reply_to_message_id:  The message ID to reply to (optional).
+            preview_url: Whether to show a preview of the URL in the message (if any).
+            keyboard: The buttons to send with the message (only in case of message from type ``text``, ``document``,
+             ``video`` and ``image``. also, the ``SectionList`` is only available to ``text`` type)
+            header: The header of the message (if keyboard is provided, optional, up to 60 characters, no markdown allowed).
+            body: The body of the message (if keyboard are provided, optional, up to 1024 characters, markdown allowed).
+            footer: The footer of the message (if keyboard is provided, optional, markdown has no effect).
+
+        Returns:
+            The ID of the sent message.
+
+        Raises:
+            ValueError: If the message type is ``reaction`` and no ``reply_to_message_id`` is provided, or if the message
+             type is ``unsupported``.
+        """
+        match self.type:
+            case MessageType.TEXT:
+                return self._client.send_message(
+                    to=to,
+                    reply_to_message_id=reply_to_message_id,
+                    text=self.text,
+                    preview_url=preview_url,
+                    keyboard=keyboard,
+                    header=header,
+                    footer=footer,
+                )
+            case MessageType.DOCUMENT:
+                return self._client.send_document(
+                    to=to,
+                    reply_to_message_id=reply_to_message_id,
+                    document=self.document.id,
+                    filename=self.document.filename,
+                    caption=self.caption,
+                    buttons=keyboard,
+                    body=body,
+                    footer=footer,
+                )
+            case MessageType.IMAGE:
+                return self._client.send_image(
+                    to=to,
+                    reply_to_message_id=reply_to_message_id,
+                    image=self.image.id,
+                    caption=self.caption,
+                    buttons=keyboard,
+                    body=body,
+                    footer=footer,
+                )
+            case MessageType.VIDEO:
+                return self._client.send_video(
+                    to=to,
+                    reply_to_message_id=reply_to_message_id,
+                    video=self.video.id,
+                    caption=self.caption,
+                    buttons=keyboard,
+                    body=body,
+                    footer=footer,
+                )
+            case MessageType.STICKER:
+                return self._client.send_sticker(
+                    to=to,
+                    reply_to_message_id=reply_to_message_id,
+                    sticker=self.sticker.id
+                )
+            case MessageType.LOCATION:
+                return self._client.send_location(
+                    to=to,
+                    latitude=self.location.latitude,
+                    longitude=self.location.longitude,
+                    name=self.location.name,
+                    address=self.location.address
+                )
+            case MessageType.AUDIO:
+                return self._client.send_audio(
+                    to=to,
+                    reply_to_message_id=reply_to_message_id,
+                    audio=self.audio.id
+                )
+            case MessageType.CONTACTS:
+                return self._client.send_contact(
+                    to=to,
+                    reply_to_message_id=reply_to_message_id,
+                    contact=self.contacts
+                )
+            case MessageType.REACTION:
+                if reply_to_message_id is None:
+                    raise ValueError("You need to provide `reply_to_message_id` in order to `copy` a reaction")
+                return self._client.send_reaction(
+                    to=to,
+                    message_id=reply_to_message_id,
+                    emoji=self.reaction.emoji or ""
+                )
+            case MessageType.UNSUPPORTED:
+                raise ValueError("MessageType.UNSUPPORTED cannot be copied!")
+            case _:
+                raise ValueError("Message with unknown type cannot be copied!")
+
 
 @dataclass(frozen=True, slots=True)
 class CallbackButton(BaseUpdate):
     """
     Represents a callback button.
 
     Attributes:
```

## Comparing `pywa-0.0.1rc15.dist-info/LICENSE` & `pywa-0.0.1rc16.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pywa-0.0.1rc15.dist-info/METADATA` & `pywa-0.0.1rc16.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywa
-Version: 0.0.1rc15
+Version: 0.0.1rc16
 Summary: Python wrapper for the WhatsApp Cloud API
 Download-URL: https://pypi.org/project/pywa/
 Author: David Lev
 Author-email: davidlev@telegmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/david-lev/pywa#readme
 Project-URL: Issue Tracker, https://github.com/david-lev/pywa/issues
```

## Comparing `pywa-0.0.1rc15.dist-info/RECORD` & `pywa-0.0.1rc16.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 pywa/__init__.py,sha256=u98CpT0wYk8-XDPUGB_hW-a_23agBkzTSzfwmoqnsE0,117
-pywa/__version__.py,sha256=Mm3FjBiBHyngSJq_VQ1PUFke9K5Xdawv6X07m1SjF3Y,26
+pywa/__version__.py,sha256=M93UajZ2PPnX4gqdGnY2tyhRbdEJ1BncArFGCRSHvkM,26
 pywa/api.py,sha256=G3NL2PKhGO7YhrVeEz2bfJhGNfD7j1lGwgKnhsZpAuU,14991
 pywa/client.py,sha256=ita4mY7UfM8xwjvEV_a60-3W4frC3uAJP-xumP5oYdM,26847
 pywa/errors.py,sha256=ErB0UGIpIOF5vZXK39WmiSrB_PSYvTJL8PLIp90vTjU,7191
-pywa/filters.py,sha256=zl4pDSnn_iA8jBujcY9LJfeAm9DEzTH0IRk0ROLEPzk,20873
+pywa/filters.py,sha256=2-hPWfevDpLsnJIvdsXdkRvazJyKGNsxHIAalJ6i48w,20703
 pywa/handlers.py,sha256=DTlKr-yvVKpTgh3F0Gsq78gT5XhBIo_VVnYHz3lu25w,1794
-pywa/types.py,sha256=1eSkFpuq-nntPe3-jjrbjIVfkkBWuRTrGQcyxQ39rv8,34447
+pywa/types.py,sha256=PKCefN4pMLNn9Dx_fbBXEUohGFEhMeGLTZfW-F4gYBU,39628
 pywa/utils.py,sha256=GRTfSvmsuOBd1_Yw2c90XoALqVPuy6HzyvJuqg3xjtI,991
 pywa/webhook.py,sha256=UFsV3UyltYLj3MYjURG6YImjU4hYVHkDffweyEe1Jdc,4613
-pywa-0.0.1rc15.dist-info/LICENSE,sha256=RwljuP8WgWttLkSivccHoHEFSDhOY8aLM_vg6Ix48yQ,1066
-pywa-0.0.1rc15.dist-info/METADATA,sha256=FIU008rTLL6qcQTre_JnD8tT1Uio_NFBImncVDGJJX4,4387
-pywa-0.0.1rc15.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-pywa-0.0.1rc15.dist-info/top_level.txt,sha256=Cl24ggXVvxvOUnQfKRASer1LzHxpYCPZd5ZcVyS98Oo,5
-pywa-0.0.1rc15.dist-info/RECORD,,
+pywa-0.0.1rc16.dist-info/LICENSE,sha256=RwljuP8WgWttLkSivccHoHEFSDhOY8aLM_vg6Ix48yQ,1066
+pywa-0.0.1rc16.dist-info/METADATA,sha256=eOdVyuz_KnoR9ZRFIyCobhAERtFK4x87soHl_5YYWoA,4387
+pywa-0.0.1rc16.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pywa-0.0.1rc16.dist-info/top_level.txt,sha256=Cl24ggXVvxvOUnQfKRASer1LzHxpYCPZd5ZcVyS98Oo,5
+pywa-0.0.1rc16.dist-info/RECORD,,
```


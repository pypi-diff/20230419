# Comparing `tmp/mafic-2.0.1.tar.gz` & `tmp/mafic-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mafic-2.0.1.tar", max compression
+gzip compressed data, was "mafic-2.1.0.tar", max compression
```

## Comparing `mafic-2.0.1.tar` & `mafic-2.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1070 2023-02-17 20:39:42.921247 mafic-2.0.1/LICENSE
--rw-r--r--   0        0        0     3315 2023-02-17 20:39:42.921247 mafic-2.0.1/README.md
--rw-r--r--   0        0        0      899 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/__init__.py
--rw-r--r--   0        0        0     3496 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/__libraries.py
--rw-r--r--   0        0        0     1348 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/__main__.py
--rw-r--r--   0        0        0     4323 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/errors.py
--rw-r--r--   0        0        0     5225 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/events.py
--rw-r--r--   0        0        0    22283 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/filter.py
--rw-r--r--   0        0        0     7310 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/ip.py
--rw-r--r--   0        0        0    34909 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/node.py
--rw-r--r--   0        0        0    22598 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/player.py
--rw-r--r--   0        0        0      874 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/playlist.py
--rw-r--r--   0        0        0      640 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/plugin.py
--rw-r--r--   0        0        0     8087 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/pool.py
--rw-r--r--   0        0        0        0 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/py.typed
--rw-r--r--   0        0        0     3417 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/region.py
--rw-r--r--   0        0        0      986 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/search_type.py
--rw-r--r--   0        0        0     3314 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/stats.py
--rw-r--r--   0        0        0     5119 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/strategy.py
--rw-r--r--   0        0        0     4045 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/track.py
--rw-r--r--   0        0        0      712 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/type_variables.py
--rw-r--r--   0        0        0      229 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/typings/__init__.py
--rw-r--r--   0        0        0     2817 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/typings/common.py
--rw-r--r--   0        0        0     3926 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/typings/http.py
--rw-r--r--   0        0        0     1968 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/typings/incoming.py
--rw-r--r--   0        0        0      497 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/typings/misc.py
--rw-r--r--   0        0        0     1115 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/typings/outgoing.py
--rw-r--r--   0        0        0       83 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/utils/__init__.py
--rw-r--r--   0        0        0     1005 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/utils/classproperty.py
--rw-r--r--   0        0        0     4888 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/utils/decode.py
--rw-r--r--   0        0        0      664 2023-02-17 20:39:42.921247 mafic-2.0.1/mafic/warnings.py
--rw-r--r--   0        0        0     2651 2023-02-17 20:39:42.921247 mafic-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 mafic-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-19 19:42:12.955674 mafic-2.1.0/LICENSE
+-rw-r--r--   0        0        0     3315 2023-04-19 19:42:12.955674 mafic-2.1.0/README.md
+-rw-r--r--   0        0        0      886 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/__init__.py
+-rw-r--r--   0        0        0     3554 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/__libraries.py
+-rw-r--r--   0        0        0     1559 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/__main__.py
+-rw-r--r--   0        0        0     4447 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/errors.py
+-rw-r--r--   0        0        0     5609 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/events.py
+-rw-r--r--   0        0        0    27782 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/filter.py
+-rw-r--r--   0        0        0     7397 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/ip.py
+-rw-r--r--   0        0        0    35580 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/node.py
+-rw-r--r--   0        0        0    23615 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/player.py
+-rw-r--r--   0        0        0      929 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/playlist.py
+-rw-r--r--   0        0        0      674 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/plugin.py
+-rw-r--r--   0        0        0     8150 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/pool.py
+-rw-r--r--   0        0        0        0 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/py.typed
+-rw-r--r--   0        0        0     3648 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/region.py
+-rw-r--r--   0        0        0     1031 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/search_type.py
+-rw-r--r--   0        0        0     3378 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/stats.py
+-rw-r--r--   0        0        0     5254 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/strategy.py
+-rw-r--r--   0        0        0     4149 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/track.py
+-rw-r--r--   0        0        0      747 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/type_variables.py
+-rw-r--r--   0        0        0      199 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/typings/__init__.py
+-rw-r--r--   0        0        0     2817 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/typings/common.py
+-rw-r--r--   0        0        0     4018 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/typings/http.py
+-rw-r--r--   0        0        0     1968 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/typings/incoming.py
+-rw-r--r--   0        0        0      524 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/typings/misc.py
+-rw-r--r--   0        0        0     1152 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/typings/outgoing.py
+-rw-r--r--   0        0        0      139 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/utils/__init__.py
+-rw-r--r--   0        0        0     1129 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/utils/classproperty.py
+-rw-r--r--   0        0        0     4987 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/utils/decode.py
+-rw-r--r--   0        0        0      710 2023-04-19 19:42:12.959674 mafic-2.1.0/mafic/warnings.py
+-rw-r--r--   0        0        0     3766 2023-04-19 19:42:12.959674 mafic-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4619 1970-01-01 00:00:00.000000 mafic-2.1.0/PKG-INFO
```

### Comparing `mafic-2.0.1/LICENSE` & `mafic-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mafic-2.0.1/README.md` & `mafic-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mafic-2.0.1/mafic/__init__.py` & `mafic-2.1.0/mafic/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 # SPDX-License-Identifier: MIT
-"""
-Mafic
-=====
-A properly typehinted lavalink client for discord.py, nextcord, disnake and py-cord.
+"""A properly typehinted lavalink client for discord.py, nextcord, disnake and py-cord.
 
 :copyright: (c) 2022-present ooliver1
 :license: MIT, see LICENSE for more details.
 """
 
 import logging
 
@@ -26,15 +23,15 @@
 from .track import *
 from .warnings import *
 
 __title__ = "mafic"
 __author__ = "ooliver1"
 __license__ = "MIT"
 __copyright__ = "Copyright 2022-present ooliver1"
-__version__ = "2.0.1"
+__version__ = "2.1.0"
 """The current version of mafic, using `PEP 440`_ format.
 
 .. _PEP 440: https://peps.python.org/pep-0440/
 """
 
 del __libraries
```

### Comparing `mafic-2.0.1/mafic/__libraries.py` & `mafic-2.1.0/mafic/__libraries.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 from os import getenv
 from typing import TYPE_CHECKING, Any
 
-from pkg_resources import get_distribution  # pyright: ignore[reportUnknownVariableType]
-from pkg_resources import DistributionNotFound
+from pkg_resources import (
+    DistributionNotFound,
+    get_distribution,  # pyright: ignore[reportUnknownVariableType]
+)
 
 from .errors import MultipleCompatibleLibraries, NoCompatibleLibraries
 
 __all__ = (
     "Client",
     "Connectable",
     "ExponentialBackoff",
@@ -36,15 +38,15 @@
         get_distribution(library)
     except DistributionNotFound:
         pass
     else:
         found.append(library)
 
 
-if not getenv("MAFIC_IGNORE_LIBRARY_CHECK", False):
+if not getenv("MAFIC_IGNORE_LIBRARY_CHECK", default=False):
     if len(found) == 0:
         raise NoCompatibleLibraries
     elif len(found) > 1:
         raise MultipleCompatibleLibraries(found)
 else:
     if found[0] == "nextcord":
         from warnings import simplefilter
@@ -113,24 +115,25 @@
     )
     from discord.abc import Connectable, GuildChannel
     from discord.backoff import ExponentialBackoff
     from discord.utils import MISSING
 
     if TYPE_CHECKING:
         from discord.types.voice import (
-            GuildVoiceState as GuildVoiceStatePayload,
-            VoiceServerUpdate as VoiceServerUpdatePayload,
+            GuildVoiceState as GuildVoiceStatePayload,  # noqa: TCH004
+            VoiceServerUpdate as VoiceServerUpdatePayload,  # noqa: TCH004
         )
 
 
 try:
     from orjson import dumps as _dumps, loads
 
-    def dumps(obj: Any) -> str:
+    def dumps(obj: Any) -> str:  # noqa: ANN401
         return _dumps(obj).decode()
 
 except ImportError:
     from json import dumps, loads
 
 
 if version_info.major != 2:
-    raise RuntimeError(f"Mafic requires version 2 of {library}.")
+    msg = f"Mafic requires version 2 of {library}."
+    raise RuntimeError(msg)
```

### Comparing `mafic-2.0.1/mafic/__main__.py` & `mafic-2.1.0/mafic/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Mafic CLI tools."""
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import platform
 import sys
 from argparse import ArgumentParser, Namespace
@@ -18,44 +19,48 @@
 - aiohttp v{aiohttp}
 - {lib} v{pkg.major}.{pkg.minor}.{pkg.micro}-{pkg.releaselevel}
 - system info: {uname.system} {uname.release} {uname.version}
 """.strip()
 
 
 def show_version() -> None:
+    """Show version information."""
     version = mafic.__version__
     uname = platform.uname()
-    print(
+    print(  # noqa: T201
         VERSION_OUTPUT.format(
             py=sys.version_info,
             mafic=version,
             aiohttp=aiohttp.__version__,
             uname=uname,
             lib=library,
             pkg=version_info,
         )
     )
 
 
 def core(_: ArgumentParser, args: Namespace) -> None:
+    """Core function for mafic CLI tools."""
     if args.version:
         show_version()
 
 
 def parse_args() -> tuple[ArgumentParser, Namespace]:
+    """Parse arguments from the CLI."""
     parser = ArgumentParser(prog="mafic", description="CLI tools for mafic")
     parser.add_argument(
         "-v",
         "--version",
         action="store_true",
         help="shows mafic and other related versions",
     )
     return parser, parser.parse_args()
 
 
 def main() -> None:
+    """Run the parser for arguments then execute."""
     parser, args = parse_args()
     core(parser, args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `mafic-2.0.1/mafic/errors.py` & `mafic-2.1.0/mafic/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Errors raised by Mafic."""
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
@@ -58,31 +59,34 @@
 
 
 class PlayerException(MaficException):
     """An issue occured when trying to play a track."""
 
 
 class TrackLoadException(PlayerException):
-    """This is raised when a track could not be loaded.
+    r"""An error raised when a track could not be loaded.
 
     Attributes
     ----------
     message: :class:`str`
         The message returned by the node.
-    severity: :data:`~typing.Literal`\\[``"COMMON"``, ``"SUSPICIOUS"``, ``"FATAL"``]
+    severity: :data:`~typing.Literal`\[``"COMMON"``, ``"SUSPICIOUS"``, ``"FATAL"``]
         The severity of the error.
+    cause: :class:`str`
+        The cause of the error.
     """
 
     def __init__(
         self, *, message: str, severity: ExceptionSeverity, cause: str
     ) -> None:
         super().__init__(f"The track could not be loaded: {message} ({severity} error)")
 
         self.message: str = message
         self.severity: ExceptionSeverity = severity
+        self.cause: str = cause
 
     @classmethod
     def from_data(cls, data: LavalinkException) -> Self:
         """Construct a new TrackLoadException from raw Lavalink data.
 
         Parameters
         ----------
@@ -90,36 +94,35 @@
             The raw data from Lavalink.
 
         Returns
         -------
         TrackLoadException
             The constructed exception.
         """
-
         return cls(
             message=data["message"], severity=data["severity"], cause=data["cause"]
         )
 
 
 class PlayerNotConnected(PlayerException):
-    """This is raised when a player is not connected to a voice channel."""
+    """An error raised when a player is not connected to a voice channel."""
 
     def __init__(self) -> None:
         super().__init__("The player is not connected to a voice channel.")
 
 
 class NodeAlreadyConnected(MaficException):
-    """This is raised when a node is already connected to Mafic."""
+    """An error raised when a node is already connected to Mafic."""
 
     def __init__(self) -> None:
         super().__init__("The node is already connected to Mafic.")
 
 
 class NoNodesAvailable(MaficException):
-    """This is raised when no nodes are available to handle a player."""
+    """An error raised when no nodes are available to handle a player."""
 
     def __init__(self) -> None:
         super().__init__("No nodes are available to handle this player.")
 
 
 class HTTPException(MaficException):
     """An issue occured when trying to make a request to the Lavalink REST API."""
@@ -128,25 +131,25 @@
         super().__init__(f"An HTTP error occured: {message} ({status})")
 
         self.status: int = status
         self.message: str = message
 
 
 class HTTPBadRequest(HTTPException):
-    """This is raised when a bad request is made to the Lavalink REST API."""
+    """An error raised when a bad request is made to the Lavalink REST API."""
 
     def __init__(self, message: str) -> None:
         super().__init__(400, message)
 
 
 class HTTPUnauthorized(HTTPException):
-    """This is raised when an unauthorized request is made to the Lavalink REST API."""
+    """An error raised when an unauthorized request is made to the Lavalink REST API."""
 
     def __init__(self, message: str) -> None:
         super().__init__(401, message)
 
 
 class HTTPNotFound(HTTPException):
-    """This is raised when a request is made to a non-existent endpoint."""
+    """An error raised when a request is made to a non-existent endpoint."""
 
     def __init__(self, message: str) -> None:
         super().__init__(404, message)
```

### Comparing `mafic-2.0.1/mafic/events.py` & `mafic-2.1.0/mafic/events.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Objects for dispatched events via the client."""
 # SPDX-License-Identifier: MIT
 # pyright: reportImportCycles=false
 # Player import.
 
 from __future__ import annotations
 
 from enum import Enum
@@ -57,32 +58,35 @@
 
     Attributes
     ----------
     code: :class:`int`
         The close code.
         Find what this can be in the Discord `docs`_.
 
-        .. _docs: https://discord.com/developers/docs/topics/opcodes-and-status-codes#close-event-codes.
+        .. _docs: https://discord.dev/topics/opcodes-and-status-codes#close-event-codes.
     reason: :class:`str`
         The close reason.
     by_discord: :class:`bool`
         Whether the close was initiated by Discord.
     player: :class:`Player`
         The player that the event was dispatched from.
     """
 
     __slots__ = ("code", "reason", "by_discord", "player")
 
-    def __init__(self, *, payload: WebSocketClosedEventPayload, player: PlayerT):
+    def __init__(
+        self, *, payload: WebSocketClosedEventPayload, player: PlayerT
+    ) -> None:
         self.code: int = payload["code"]
         self.reason: str = payload["reason"]
         self.by_discord: bool = payload["byRemote"]
         self.player: PlayerT = player
 
     def __repr__(self) -> str:
+        """Get a string representation of the event."""
         return (
             f"<WebSocketClosedEvent code={self.code} reason={self.reason!r} "
             f"by_discord={self.by_discord}>"
         )
 
 
 class TrackStartEvent(Generic[PlayerT]):
@@ -94,19 +98,20 @@
         The track that started playing.
     player: :class:`Player`
         The player that the event was dispatched from.
     """
 
     __slots__ = ("track", "player")
 
-    def __init__(self, *, track: Track, player: PlayerT):
+    def __init__(self, *, track: Track, player: PlayerT) -> None:
         self.track: Track = track
         self.player: PlayerT = player
 
     def __repr__(self) -> str:
+        """Get a string representation of the event."""
         return f"<TrackStartEvent track={self.track!r}>"
 
 
 class TrackEndEvent(Generic[PlayerT]):
     """Represents an event when a track ends.
 
     Attributes
@@ -117,20 +122,23 @@
         The reason why the track ended.
     player: :class:`Player`
         The player that the event was dispatched from.
     """
 
     __slots__ = ("track", "reason", "player")
 
-    def __init__(self, *, track: Track, payload: TrackEndEventPayload, player: PlayerT):
+    def __init__(
+        self, *, track: Track, payload: TrackEndEventPayload, player: PlayerT
+    ) -> None:
         self.track: Track = track
         self.reason: EndReason = EndReason(payload["reason"])
         self.player: PlayerT = player
 
     def __repr__(self) -> str:
+        """Get a string representation of the event."""
         return f"<TrackEndEvent track={self.track!r} reason={self.reason!r}>"
 
 
 class TrackExceptionEvent(Generic[PlayerT]):
     """Represents an event when an exception occurs while playing a track.
 
     Attributes
@@ -147,20 +155,21 @@
 
     def __init__(
         self,
         *,
         track: Track,
         payload: TrackExceptionEventPayload,
         player: PlayerT,
-    ):
+    ) -> None:
         self.track: Track = track
         self.exception: LavalinkException = payload["exception"]
         self.player: PlayerT = player
 
     def __repr__(self) -> str:
+        """Get a string representation of the event."""
         return (
             f"<TrackExceptionEvent track={self.track!r} exception={self.exception!r}>"
         )
 
 
 class TrackStuckEvent(Generic[PlayerT]):
     """Represents an event when a track gets stuck.
@@ -175,16 +184,17 @@
         The player that the event was dispatched from.
     """
 
     __slots__ = ("track", "threshold_ms", "player")
 
     def __init__(
         self, *, track: Track, payload: TrackStuckEventPayload, player: PlayerT
-    ):
+    ) -> None:
         self.track: Track = track
         self.threshold_ms: int = payload["thresholdMs"]
         self.player: PlayerT = player
 
     def __repr__(self) -> str:
+        """Get a string representation of the event."""
         return (
             f"<TrackStuckEvent track={self.track!r} threshold_ms={self.threshold_ms}>"
         )
```

### Comparing `mafic-2.0.1/mafic/filter.py` & `mafic-2.1.0/mafic/filter.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,18 @@
+"""Filters that can be applied to a Player."""
 # SPDX-License-Identifier: MIT
 # Reference to filter meanings can be found in:
 # https://github.com/natanbc/lavadsp
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from typing import Any
-
     from typing_extensions import Self
 
     from .typings import (
         ChannelMix as ChannelMixPayload,
         Distortion as DistortionPayload,
         EQBand as EQBandPayload,
         Filters,
@@ -57,76 +56,115 @@
 
     band: int
     gain: float
 
     @property
     def payload(self) -> EQBandPayload:
         """Generate the raw Lavalink payload for this band."""
-
         return {"band": self.band, "gain": self.gain}
 
 
-@dataclass(unsafe_hash=True)
 class Equalizer:
-    """Represents an `equaliser`_.
+    r"""Represents an `equaliser`_.
 
     .. _equaliser: https://en.wikipedia.org/wiki/Equalization_(audio)
 
+    .. versionchanged:: 2.1
+
+        Added support for :class:`list`\s of
+        :class:`tuple`\[:class:`int`, :class:`float`] and :class:`float` to the
+        constructor.
+
     Attributes
     ----------
-    bands: :class:`list`\\[:class:`EQBand`]
+    bands: :class:`list`\[:class:`EQBand`]
         The bands to set the gains of.
     """
 
-    bands: list[EQBand]
+    __slots__ = ("bands",)
+
+    def __init__(
+        self, bands: list[EQBand] | list[tuple[int, float]] | list[float]
+    ) -> None:
+        self.bands = [self._convert_band(band, i) for i, band in enumerate(bands)]
+
+    @staticmethod
+    def _convert_band(band: EQBand | tuple[int, float] | float, i: int) -> EQBand:
+        if isinstance(band, EQBand):
+            return band
+        elif isinstance(band, tuple):
+            return EQBand(band=band[0], gain=band[1])
+        elif isinstance(
+            band, (float, int)
+        ):  # pyright: ignore[reportUnnecessaryIsInstance]
+            return EQBand(band=i, gain=band)
+        else:
+            msg = f"Expected EQBand, tuple[int, float] or float, got {band!r}"
+            raise TypeError(msg)
+
+    def __eq__(self, other: object) -> bool:
+        """Check if this equaliser is equal to another."""
+        if not isinstance(other, Equalizer):
+            return NotImplemented
+
+        return self.bands == other.bands
+
+    def __repr__(self) -> str:
+        """Generate a representation of this equaliser."""
+        return f"<Equalizer bands={self.bands!r}>"
+
+    def __hash__(self) -> int:
+        """Get the hash of this equaliser."""
+        return hash(tuple(self.bands))
 
     @property
     def payload(self) -> list[EQBandPayload]:
+        """Generate the raw Lavalink payload for this equaliser."""
         return [band.payload for band in self.bands]
 
     @classmethod
     def from_payload(cls, payload: list[EQBandPayload]) -> Self:
+        """Generate an :class:`Equalizer` from a Lavalink payload."""
         return cls(
             bands=[EQBand(band=band["band"], gain=band["gain"]) for band in payload]
         )
 
 
 @dataclass(unsafe_hash=True)
 class Karaoke:
-    """Represents a filter which can be used to eliminate part of a band.
+    r"""Represents a filter which can be used to eliminate part of a band.
 
     This usually targets vocals, to sound like karaoke music.
 
     Attributes
     ----------
-    level: :data:`~typing.Optional`\\[:class:`float`]
+    level: :data:`~typing.Optional`\[:class:`float`]
         The level of the karaoke effect. Must be between ``0.0`` and ``1.0``.
         Where ``0.0`` is no effect and ``1.0`` is full effect.
         This defaults to ``1.0``.
-    mono_level: :data:`~typing.Optional`\\[:class:`float`]
+    mono_level: :data:`~typing.Optional`\[:class:`float`]
         The level of the mono effect. Must be between ``0.0`` and ``1.0``.
         Where ``0.0`` is no effect and ``1.0`` is full effect.
         This defaults to ``1.0``.
-    filter_band: :data:`~typing.Optional`\\[:class:`float`]
+    filter_band: :data:`~typing.Optional`\[:class:`float`]
         The frequency of the filter band in Hz.
         This defaults to ``220.0``.
-    filter_width: :data:`~typing.Optional`\\[:class:`float`]
+    filter_width: :data:`~typing.Optional`\[:class:`float`]
         The width of the filter band.
         This defaults to ``100.0``.
     """
 
     level: float | None = None
     mono_level: float | None = None
     filter_band: float | None = None
     filter_width: float | None = None
 
     @property
     def payload(self) -> KaraokePayload:
         """Generate the raw Lavalink payload for this filter."""
-
         data: KaraokePayload = {}
 
         if self.level is not None:
             data["level"] = self.level
 
         if self.mono_level is not None:
             data["monoLevel"] = self.mono_level
@@ -137,45 +175,44 @@
         if self.filter_width is not None:
             data["filterWidth"] = self.filter_width
 
         return data
 
     @classmethod
     def from_payload(cls, payload: KaraokePayload) -> Self:
+        """Generate a :class:`Karaoke` from a Lavalink payload."""
         return cls(
             level=payload.get("level"),
             mono_level=payload.get("monoLevel"),
             filter_band=payload.get("filterBand"),
             filter_width=payload.get("filterWidth"),
         )
 
 
 @dataclass(unsafe_hash=True)
 class Timescale:
-    """Represents a filter which can be used to change the speed,
-    pitch and rate of audio.
+    r"""Represents a filter which is used to change the speed, pitch and rate of audio.
 
     Attributes
     ----------
-    speed: :data:`~typing.Optional`\\[:class:`float`]
+    speed: :data:`~typing.Optional`\[:class:`float`]
         The speed of the audio. Must be at least ``0.0``. ``1.0`` is normal speed.
-    pitch: :data:`~typing.Optional`\\[:class:`float`]
+    pitch: :data:`~typing.Optional`\[:class:`float`]
         The pitch of the audio. Must be at least ``0.0``. ``1.0`` is normal pitch.
-    rate: :data:`~typing.Optional`\\[:class:`float`]
+    rate: :data:`~typing.Optional`\[:class:`float`]
         The rate of the audio. Must be at least ``0.0``. ``1.0`` is normal rate.
     """
 
     speed: float | None = None
     pitch: float | None = None
     rate: float | None = None
 
     @property
     def payload(self) -> TimescalePayload:
         """Generate the raw Lavalink payload for this filter."""
-
         data: TimescalePayload = {}
 
         if self.speed is not None:
             data["speed"] = self.speed
 
         if self.pitch is not None:
             data["pitch"] = self.pitch
@@ -183,147 +220,148 @@
         if self.rate is not None:
             data["rate"] = self.rate
 
         return data
 
     @classmethod
     def from_payload(cls, payload: TimescalePayload) -> Self:
+        """Generate a :class:`Timescale` from a Lavalink payload."""
         return cls(
             speed=payload.get("speed"),
             pitch=payload.get("pitch"),
             rate=payload.get("rate"),
         )
 
 
 @dataclass(unsafe_hash=True)
 class Tremolo:
-    """Represents a filter which can be used to add a `tremolo`_ effect to audio.
+    r"""Represents a filter which can be used to add a `tremolo`_ effect to audio.
 
     Tremolo oscillates the volume of the audio.
 
     .. _tremolo: https://en.wikipedia.org/wiki/Tremolo
 
     Attributes
     ----------
-    frequency: :data:`~typing.Optional`\\[:class:`float`]
+    frequency: :data:`~typing.Optional`\[:class:`float`]
         The frequency of the tremolo effect. Must be at least ``0.0``.
         This defaults to ``2.0``.
-    depth: :data:`~typing.Optional`\\[:class:`float`]
+    depth: :data:`~typing.Optional`\[:class:`float`]
         The depth of the tremolo effect. Must be between ``0.0`` and ``1.0``.
         Where ``0.0`` is no effect and ``1.0`` is full effect.
         This defaults to ``0.5``.
     """
 
     frequency: float | None = None
     depth: float | None = None
 
     @property
     def payload(self) -> TremoloPayload:
         """Generate the raw Lavalink payload for this filter."""
-
         data: TremoloPayload = {}
 
         if self.frequency is not None:
             data["frequency"] = self.frequency
 
         if self.depth is not None:
             data["depth"] = self.depth
 
         return data
 
     @classmethod
     def from_payload(cls, payload: TremoloPayload) -> Self:
+        """Generate a :class:`Tremolo` from a Lavalink payload."""
         return cls(
             frequency=payload.get("frequency"),
             depth=payload.get("depth"),
         )
 
 
 @dataclass(repr=True)
 class Vibrato:
-    """Represents a filter which can be used to add a `vibrato`_ effect to audio.
+    r"""Represents a filter which can be used to add a `vibrato`_ effect to audio.
 
     Vibrato oscillates the pitch of the audio.
 
     .. _vibrato: https://en.wikipedia.org/wiki/Vibrato
 
     Attributes
     ----------
-    frequency: :data:`~typing.Optional`\\[:class:`float`]
+    frequency: :data:`~typing.Optional`\[:class:`float`]
         The frequency of the vibrato effect. Must be at least ``0.0``.
         This defaults to ``2.0``.
-    depth: :data:`~typing.Optional`\\[:class:`float`]
+    depth: :data:`~typing.Optional`\[:class:`float`]
         The depth of the vibrato effect. Must be between ``0.0`` and ``1.0``.
         Where ``0.0`` is no effect and ``1.0`` is full effect.
         This defaults to ``0.5``.
     """
 
     frequency: float | None = None
     depth: float | None = None
 
     @property
     def payload(self) -> VibratoPayload:
         """Generate the raw Lavalink payload for this filter."""
-
         data: VibratoPayload = {}
 
         if self.frequency is not None:
             data["frequency"] = self.frequency
 
         if self.depth is not None:
             data["depth"] = self.depth
 
         return data
 
     @classmethod
     def from_payload(cls, payload: VibratoPayload) -> Self:
+        """Generate a :class:`Vibrato` from a Lavalink payload."""
         return cls(
             frequency=payload.get("frequency"),
             depth=payload.get("depth"),
         )
 
 
 @dataclass(unsafe_hash=True)
 class Rotation:
-    """Represents a filter which can be used to add a rotating effect to audio.
+    r"""Represents a filter which can be used to add a rotating effect to audio.
 
     An example can be with `"8D audio" (without the reverb)`_.
 
     .. _"8D audio" (without the reverb): https://youtu.be/QB9EB8mTKcc>
 
     Attributes
     ----------
-    rotation_hz: :data:`~typing.Optional`\\[:class:`float`]
+    rotation_hz: :data:`~typing.Optional`\[:class:`float`]
         The rotation speed in Hz. Must be at least ``0.0``.
         ``0.2`` is similar to the example above.
     """
 
     rotation_hz: float | None = None
 
     @property
     def payload(self) -> RotationPayload:
         """Generate the raw Lavalink payload for this filter."""
-
         data: RotationPayload = {}
 
         if self.rotation_hz is not None:
             data["rotationHz"] = self.rotation_hz
 
         return data
 
     @classmethod
     def from_payload(cls, payload: RotationPayload) -> Self:
+        """Generate a :class:`Rotation` from a Lavalink payload."""
         return cls(
             rotation_hz=payload.get("rotationHz"),
         )
 
 
 @dataclass(unsafe_hash=True)
 class Distortion:
-    """Represents a filter which can be used to add a distortion effect to audio.
+    r"""Represents a filter which can be used to add a distortion effect to audio.
 
     This applies sine, cosine and tangent distortion to the audio.
     The formula that is used::
 
         sample_sin = sin_offset + math.sin(sample * sin_scale);
         sample_cos = cos_offset + math.cos(sample * cos_scale);
         sample_tan = tan_offset + math.tan(sample * tan_scale);
@@ -334,36 +372,36 @@
                 offset +
                 scale * sample_sin * sample_cos * sample_tan
             )
         )
 
     Attributes
     ----------
-    sin_offset: :data:`~typing.Optional`\\[:class:`float`]
+    sin_offset: :data:`~typing.Optional`\[:class:`float`]
         The offset of the sine distortion.
         This defaults to ``0.0``.
-    sin_scale: :data:`~typing.Optional`\\[:class:`float`]
+    sin_scale: :data:`~typing.Optional`\[:class:`float`]
         The scale of the sine distortion.
         This defaults to ``1.0``.
-    cos_offset: :data:`~typing.Optional`\\[:class:`float`]
+    cos_offset: :data:`~typing.Optional`\[:class:`float`]
         The offset of the cosine distortion.
         This defaults to ``0.0``.
-    cos_scale: :data:`~typing.Optional`\\[:class:`float`]
+    cos_scale: :data:`~typing.Optional`\[:class:`float`]
         The scale of the cosine distortion.
         This defaults to ``1.0``.
-    tan_offset: :data:`~typing.Optional`\\[:class:`float`]
+    tan_offset: :data:`~typing.Optional`\[:class:`float`]
         The offset of the tangent distortion.
         This defaults to ``0.0``.
-    tan_scale: :data:`~typing.Optional`\\[:class:`float`]
+    tan_scale: :data:`~typing.Optional`\[:class:`float`]
         The scale of the tangent distortion.
         This defaults to ``1.0``.
-    offset: :data:`~typing.Optional`\\[:class:`float`]
+    offset: :data:`~typing.Optional`\[:class:`float`]
         The offset of the distortion.
         This defaults to ``0.0``.
-    scale: :data:`~typing.Optional`\\[:class:`float`]
+    scale: :data:`~typing.Optional`\[:class:`float`]
         The scale of the distortion.
         This defaults to ``1.0``.
     """
 
     sin_offset: float | None = None
     sin_scale: float | None = None
     cos_offset: float | None = None
@@ -372,15 +410,14 @@
     tan_scale: float | None = None
     offset: float | None = None
     scale: float | None = None
 
     @property
     def payload(self) -> DistortionPayload:
         """Generate the raw Lavalink payload for this filter."""
-
         data: DistortionPayload = {}
 
         if self.sin_offset is not None:
             data["sinOffset"] = self.sin_offset
 
         if self.sin_scale is not None:
             data["sinScale"] = self.sin_scale
@@ -403,57 +440,57 @@
         if self.scale is not None:
             data["scale"] = self.scale
 
         return data
 
     @classmethod
     def from_payload(cls, payload: DistortionPayload) -> Self:
+        """Generate a :class:`Distortion` from a Lavalink payload."""
         return cls(
             sin_offset=payload.get("sinOffset"),
             sin_scale=payload.get("sinScale"),
             cos_offset=payload.get("cosOffset"),
             cos_scale=payload.get("cosScale"),
             tan_offset=payload.get("tanOffset"),
             tan_scale=payload.get("tanScale"),
             offset=payload.get("offset"),
             scale=payload.get("scale"),
         )
 
 
 @dataclass(unsafe_hash=True)
 class ChannelMix:
-    """Represents a filter which can be used to mix the audio channels.
+    r"""Represents a filter which can be used to mix the audio channels.
 
     Setting all of these to ``0.5`` will make the audio mono.
 
     Attributes
     ----------
-    left_to_left: :data:`~typing.Optional`\\[:class:`float`]
+    left_to_left: :data:`~typing.Optional`\[:class:`float`]
         The amount of the left channel to mix into the left channel.
         This defaults to ``1.0``.
-    left_to_right: :data:`~typing.Optional`\\[:class:`float`]
+    left_to_right: :data:`~typing.Optional`\[:class:`float`]
         The amount of the left channel to mix into the right channel.
         This defaults to ``0.0``.
-    right_to_left: :data:`~typing.Optional`\\[:class:`float`]
+    right_to_left: :data:`~typing.Optional`\[:class:`float`]
         The amount of the right channel to mix into the left channel.
         This defaults to ``0.0``.
-    right_to_right: :data:`~typing.Optional`\\[:class:`float`]
+    right_to_right: :data:`~typing.Optional`\[:class:`float`]
         The amount of the right channel to mix into the right channel.
         This defaults to ``1.0``.
     """
 
     left_to_left: float | None = None
     left_to_right: float | None = None
     right_to_left: float | None = None
     right_to_right: float | None = None
 
     @property
     def payload(self) -> ChannelMixPayload:
         """Generate the raw Lavalink payload for this filter."""
-
         data: ChannelMixPayload = {}
 
         if self.left_to_left is not None:
             data["leftToLeft"] = self.left_to_left
 
         if self.left_to_right is not None:
             data["leftToRight"] = self.left_to_right
@@ -464,58 +501,58 @@
         if self.right_to_right is not None:
             data["rightToRight"] = self.right_to_right
 
         return data
 
     @classmethod
     def from_payload(cls, payload: ChannelMixPayload) -> Self:
+        """Generate a :class:`ChannelMix` from a Lavalink payload."""
         return cls(
             left_to_left=payload.get("leftToLeft"),
             left_to_right=payload.get("leftToRight"),
             right_to_left=payload.get("rightToLeft"),
             right_to_right=payload.get("rightToRight"),
         )
 
 
 @dataclass(unsafe_hash=True)
 class LowPass:
-    """Represents a filter which can be used to apply a `low pass filter` to audio.
+    r"""Represents a filter which can be used to apply a `low pass filter` to audio.
 
     High frequencies are suppressed, while low frequencies are passed through.
 
     .. _low pass filter: http://phrogz.net/js/framerate-independent-low-pass-filter.html
 
     Attributes
     ----------
-    smoothing: :data:`~typing.Optional`\\[:class:`float`]
+    smoothing: :data:`~typing.Optional`\[:class:`float`]
         The smoothing of the low pass filter.
         This defaults to ``0.0``.
     """
 
     smoothing: float | None = None
 
     @property
     def payload(self) -> LowPassPayload:
         """Generate the raw Lavalink payload for this filter."""
-
         data: LowPassPayload = {}
 
         if self.smoothing is not None:
             data["smoothing"] = self.smoothing
 
         return data
 
     @classmethod
     def from_payload(cls, payload: LowPassPayload) -> Self:
+        """Generate a :class:`LowPass` from a Lavalink payload."""
         return cls(smoothing=payload.get("smoothing"))
 
 
-@dataclass(unsafe_hash=True)
 class Filter:
-    """Represents a filter which can be applied to audio.
+    r"""Represents a filter which can be applied to audio.
 
     .. container:: operations
 
         .. describe:: x | y
 
             Merges two filters together, favouring attributes from y.
 
@@ -527,53 +564,154 @@
 
             Merges two filters together, favouring attributes from x.
 
         .. describe:: x &= y
 
             Merges two filters together, favouring attributes from y, assigning to x.
 
+    .. versionchanged:: 2.1
+
+        ``equalizer`` now accepts a :class:`list` of any of the following:
+
+        - :class:`tuple`\[:class:`int`, :class:`float`\]
+        - :class:`float`
+        - :class:`EQBand`
+
     Attributes
     ----------
-    equalizer: :data:`~typing.Optional`\\[:class:`Equalizer`]
+    equalizer: :data:`~typing.Optional`\[:class:`Equalizer`]
         The equalizer to use.
-    karaoke: :data:`~typing.Optional`\\[:class:`Karaoke`]
+    karaoke: :data:`~typing.Optional`\[:class:`Karaoke`]
         The karaoke filter to use.
-    timescale: :data:`~typing.Optional`\\[:class:`Timescale`]
+    timescale: :data:`~typing.Optional`\[:class:`Timescale`]
         The timescale filter to use.
-    tremolo: :data:`~typing.Optional`\\[:class:`Tremolo`]
+    tremolo: :data:`~typing.Optional`\[:class:`Tremolo`]
         The tremolo filter to use.
-    vibrato: :data:`~typing.Optional`\\[:class:`Vibrato`]
+    vibrato: :data:`~typing.Optional`\[:class:`Vibrato`]
         The vibrato filter to use.
-    rotation: :data:`~typing.Optional`\\[:class:`Rotation`]
+    rotation: :data:`~typing.Optional`\[:class:`Rotation`]
         The rotation filter to use.
-    distortion: :data:`~typing.Optional`\\[:class:`Distortion`]
+    distortion: :data:`~typing.Optional`\[:class:`Distortion`]
         The distortion filter to use.
-    channel_mix: :data:`~typing.Optional`\\[:class:`ChannelMix`]
+    channel_mix: :data:`~typing.Optional`\[:class:`ChannelMix`]
         The channel mix filter to use.
-    low_pass: :data:`~typing.Optional`\\[:class:`LowPass`]
+    low_pass: :data:`~typing.Optional`\[:class:`LowPass`]
         The low pass filter to use.
-    volume: :data:`~typing.Optional`\\[:class:`float`]
+    volume: :data:`~typing.Optional`\[:class:`float`]
         The volume to use.
     """
 
-    equalizer: Equalizer | None = None
-    karaoke: Karaoke | None = None
-    timescale: Timescale | None = None
-    tremolo: Tremolo | None = None
-    vibrato: Vibrato | None = None
-    rotation: Rotation | None = None
-    distortion: Distortion | None = None
-    channel_mix: ChannelMix | None = None
-    low_pass: LowPass | None = None
-    volume: float | None = None
+    __slots__ = (
+        "equalizer",
+        "karaoke",
+        "timescale",
+        "tremolo",
+        "vibrato",
+        "rotation",
+        "distortion",
+        "channel_mix",
+        "low_pass",
+        "volume",
+    )
+
+    def __init__(
+        self,
+        *,
+        equalizer: Equalizer
+        | list[tuple[int, float]]
+        | list[float]
+        | list[EQBand]
+        | None = None,
+        karaoke: Karaoke | None = None,
+        timescale: Timescale | None = None,
+        tremolo: Tremolo | None = None,
+        vibrato: Vibrato | None = None,
+        rotation: Rotation | None = None,
+        distortion: Distortion | None = None,
+        channel_mix: ChannelMix | None = None,
+        low_pass: LowPass | None = None,
+        volume: float | None = None,
+    ) -> None:
+        self.equalizer: Equalizer | None = self._convert_equalizer(equalizer)
+        self.karaoke: Karaoke | None = karaoke
+        self.timescale: Timescale | None = timescale
+        self.tremolo: Tremolo | None = tremolo
+        self.vibrato: Vibrato | None = vibrato
+        self.rotation: Rotation | None = rotation
+        self.distortion: Distortion | None = distortion
+        self.channel_mix: ChannelMix | None = channel_mix
+        self.low_pass: LowPass | None = low_pass
+        self.volume: float | None = volume
+
+    def _convert_equalizer(
+        self,
+        equalizer: Equalizer
+        | list[tuple[int, float]]
+        | list[float]
+        | list[EQBand]
+        | None,
+    ) -> Equalizer | None:
+        if equalizer is None:
+            return None
+
+        if isinstance(equalizer, list):
+            return Equalizer(equalizer)
+
+        return equalizer
+
+    def __hash__(self) -> int:
+        """Get the hash of this filter."""
+        return hash(
+            (
+                self.equalizer,
+                self.karaoke,
+                self.timescale,
+                self.tremolo,
+                self.vibrato,
+                self.rotation,
+                self.distortion,
+                self.channel_mix,
+                self.low_pass,
+                self.volume,
+            )
+        )
+
+    def __eq__(self, other: object) -> bool:
+        """Check if two filters are equal."""
+        if not isinstance(other, Filter):
+            return NotImplemented
+
+        return (
+            self.equalizer == other.equalizer
+            and self.karaoke == other.karaoke
+            and self.timescale == other.timescale
+            and self.tremolo == other.tremolo
+            and self.vibrato == other.vibrato
+            and self.rotation == other.rotation
+            and self.distortion == other.distortion
+            and self.channel_mix == other.channel_mix
+            and self.low_pass == other.low_pass
+            and self.volume == other.volume
+        )
+
+    def __repr__(self) -> str:
+        """Gemerate the string representation of this filter."""
+        slots = self.__slots__
+
+        attrs = [
+            f"{attr}={getattr(self, attr)!r}"
+            for attr in slots
+            if getattr(self, attr) is not None
+        ]
+
+        return f"<Filter {' '.join(attrs)}>" if attrs else "<Filter>"
 
     @property
     def payload(self) -> Filters:
         """Generate the raw Lavalink payload for this filter."""
-
         payload: Filters = {}
 
         if self.equalizer:
             payload["equalizer"] = self.equalizer.payload
 
         if self.karaoke:
             payload["karaoke"] = self.karaoke.payload
@@ -603,15 +741,14 @@
             payload["volume"] = self.volume
 
         return payload
 
     @classmethod
     def from_payload(cls, data: Filters) -> Self:
         """Generate a filter from a raw Lavalink payload."""
-
         self = cls()
 
         if "equalizer" in data:
             self.equalizer = Equalizer.from_payload(data["equalizer"])
 
         if "karaoke" in data:
             self.karaoke = Karaoke.from_payload(data["karaoke"])
@@ -638,74 +775,82 @@
             self.low_pass = LowPass.from_payload(data["lowPass"])
 
         if "volume" in data:
             self.volume = data["volume"]
 
         return self
 
-    def __or__(self, other: Any) -> Filter:
-        # A | B uses A and replaces B, like dictionaries.
-
-        if not isinstance(other, Filter):
-            raise TypeError(f"Expected Filter instance, not {type(other)!r}")
+    def __or__(self, other: Filter) -> Filter:
+        """Merge two filters together, favouring attributes from other."""
+        if not isinstance(
+            other, Filter
+        ):  # pyright: ignore[reportUnnecessaryIsInstance]
+            msg = f"Expected Filter instance, not {type(other)!r}"
+            raise TypeError(msg)
 
         return Filter(
             equalizer=other.equalizer or self.equalizer,
             karaoke=other.karaoke or self.karaoke,
             timescale=other.timescale or self.timescale,
             tremolo=other.tremolo or self.tremolo,
             vibrato=other.vibrato or self.vibrato,
             rotation=other.rotation or self.rotation,
             distortion=other.distortion or self.distortion,
             channel_mix=other.channel_mix or self.channel_mix,
             low_pass=other.low_pass or self.low_pass,
             volume=other.volume or self.volume,
         )
 
-    def __ior__(self, other: Any) -> None:
-        # Like __or__ but |=
-
-        if not isinstance(other, Filter):
-            raise TypeError(f"Expected Filter instance, not {type(other)!r}")
+    def __ior__(self, other: Filter) -> None:
+        """Merge two filters together, favouring attributes from other, in place."""
+        if not isinstance(
+            other, Filter
+        ):  # pyright: ignore[reportUnnecessaryIsInstance]
+            msg = f"Expected Filter instance, not {type(other)!r}"
+            raise TypeError(msg)
 
         self.equalizer = other.equalizer or self.equalizer
         self.karaoke = other.karaoke or self.karaoke
         self.timescale = other.timescale or self.timescale
         self.tremolo = other.tremolo or self.tremolo
         self.vibrato = other.vibrato or self.vibrato
         self.rotation = other.rotation or self.rotation
         self.distortion = other.distortion or self.distortion
         self.channel_mix = other.channel_mix or self.channel_mix
         self.low_pass = other.low_pass or self.low_pass
         self.volume = other.volume or self.volume
 
-    def __and__(self, other: Any) -> Filter:
-        # A & B uses A and only B if A does not have that field.
-
-        if not isinstance(other, Filter):
-            raise TypeError(f"Expected Filter instance, not {type(other)!r}")
+    def __and__(self, other: Filter) -> Filter:
+        """Merge two filters together, favouring attributes from self."""
+        if not isinstance(
+            other, Filter
+        ):  # pyright: ignore[reportUnnecessaryIsInstance]
+            msg = f"Expected Filter instance, not {type(other)!r}"
+            raise TypeError(msg)
 
         return Filter(
             equalizer=self.equalizer or other.equalizer,
             karaoke=self.karaoke or other.karaoke,
             timescale=self.timescale or other.timescale,
             tremolo=self.tremolo or other.tremolo,
             vibrato=self.vibrato or other.vibrato,
             rotation=self.rotation or other.rotation,
             distortion=self.distortion or other.distortion,
             channel_mix=self.channel_mix or other.channel_mix,
             low_pass=self.low_pass or other.low_pass,
             volume=self.volume or other.volume,
         )
 
-    def __iand__(self, other: Any) -> None:
-        # Like __and__ but &=
-
-        if not isinstance(other, Filter):
-            raise TypeError(f"Expected Filter instance, not {type(other)!r}")
+    def __iand__(self, other: Filter) -> None:
+        """Merge two filters together, favouring attributes from self, in place."""
+        if not isinstance(
+            other, Filter
+        ):  # pyright: ignore[reportUnnecessaryIsInstance]
+            msg = f"Expected Filter instance, not {type(other)!r}"
+            raise TypeError(msg)
 
         self.equalizer = self.equalizer or other.equalizer
         self.karaoke = self.karaoke or other.karaoke
         self.timescale = self.timescale or other.timescale
         self.tremolo = self.tremolo or other.tremolo
         self.vibrato = self.vibrato or other.vibrato
         self.rotation = self.rotation or other.rotation
```

### Comparing `mafic-2.0.1/mafic/ip.py` & `mafic-2.1.0/mafic/ip.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+"""The Lavalink route planner API."""
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 from abc import ABC
-from datetime import datetime
+from datetime import datetime, timezone
 from enum import Enum
 from typing import TYPE_CHECKING, Union
 
 if TYPE_CHECKING:
     from .typings import (
         BalancingIPRouteDetails,
         BaseDetails,
@@ -109,23 +110,25 @@
         The time the address was added to the list of failing addresses.
     """
 
     __slots__ = ("address", "time")
 
     def __init__(self, data: FailingIPAddress) -> None:
         self.address: str = data["address"]
-        self.time: datetime = datetime.fromtimestamp(data["failingTimestamp"])
+        self.time: datetime = datetime.fromtimestamp(
+            data["failingTimestamp"], tz=timezone.utc
+        )
 
 
 class BaseIPRoutePlannerStatus(ABC):
-    """An :term:`abstract base class` representing the status of an IP route planner.
+    r"""An :term:`abstract base class` representing the status of an IP route planner.
 
     Attributes
     ----------
-    failing_addresses: :class:`list`\\[:class:`FailingAddress`]
+    failing_addresses: :class:`list`\[:class:`FailingAddress`]
         The list of failing addresses.
     ip_block: :class:`IPBlock`
         The IP block.
     type: :class:`IPRoutePlannerType`
         The type of route planner.
     """
 
@@ -137,19 +140,19 @@
         self.ip_block: IPBlock = IPBlock(data["ipBlock"])
         self.failing_addresses: list[FailingAddress] = [
             FailingAddress(addr) for addr in data["failingAddresses"]
         ]
 
 
 class RotatingIPRoutePlannerStatus(BaseIPRoutePlannerStatus):
-    """Represents the status of a rotating IP route planner.
+    r"""Represents the status of a rotating IP route planner.
 
     Attributes
     ----------
-    type: :data:`~typing.Literal`\\[:attr:`IPRoutePlannerType.ROTATING_IP`]
+    type: :data:`~typing.Literal`\[:attr:`IPRoutePlannerType.ROTATING_IP`]
         The type of route planner. This will always be
         :attr:`IPRoutePlannerType.ROTATING_IP`.
     current_address: :class:`str`
         The current IP address.
     ip_index: :class:`int`
         The offset of the current IP address.
     rotate_index: :class:`int`
@@ -164,19 +167,19 @@
         super().__init__(data)
         self.rotate_index: int = int(data["rotateIndex"])
         self.ip_index: int = int(data["ipIndex"])
         self.current_address: str = data["currentAddress"]
 
 
 class NanoIPRoutePlannerStatus(BaseIPRoutePlannerStatus):
-    """Represents the status of a nano IP route planner.
+    r"""Represents the status of a nano IP route planner.
 
     Attributes
     ----------
-    type: :data:`~typing.Literal`\\[:attr:`IPRoutePlannerType.NANO_IP`]
+    type: :data:`~typing.Literal`\[:attr:`IPRoutePlannerType.NANO_IP`]
         The type of route planner. This will always be
         :attr:`IPRoutePlannerType.NANO_IP`.
     current_address_index: :class:`int`
         The index of the current address.
     """
 
     __slots__ = ("current_address_index",)
@@ -185,19 +188,19 @@
 
     def __init__(self, data: NanoIPRouteDetails) -> None:
         super().__init__(data)
         self.current_address_index: int = int(data["currentAddressIndex"])
 
 
 class RotatingNanoIPRoutePlannerStatus(BaseIPRoutePlannerStatus):
-    """Represents the status of a rotating nano IP route planner.
+    r"""Represents the status of a rotating nano IP route planner.
 
     Attributes
     ----------
-    type: :data:`~typing.Literal`\\[:attr:`IPRoutePlannerType.ROTATING_NANO_IP`]
+    type: :data:`~typing.Literal`\[:attr:`IPRoutePlannerType.ROTATING_NANO_IP`]
         The type of route planner. This will always be
         :attr:`IPRoutePlannerType.ROTATING_NANO_IP`.
     block_index: :class:`int`
         The index of the current block.
     current_address_index: :class:`int`
         The index of the current address.
     """
@@ -209,19 +212,19 @@
     def __init__(self, data: RotatingNanoIPRouteDetails) -> None:
         super().__init__(data)
         self.block_index: int = int(data["blockIndex"])
         self.current_address_index: int = int(data["currentAddressIndex"])
 
 
 class BalancingIPRoutePlannerStatus(BaseIPRoutePlannerStatus):
-    """Represents the status of a balancing IP route planner.
+    r"""Represents the status of a balancing IP route planner.
 
     Attributes
     ----------
-    type: :data:`~typing.Literal`\\[:attr:`IPRoutePlannerType.BALANCING_IP`]
+    type: :data:`~typing.Literal`\[:attr:`IPRoutePlannerType.BALANCING_IP`]
         The type of route planner. This will always be
         :attr:`IPRoutePlannerType.BALANCING_IP`.
     current_address_index: :class:`int`
         The index of the current address.
     ip_index: :class:`int`
         The offset of the current IP block in the IP block list.
     rotate_index: :class:`int`
```

### Comparing `mafic-2.0.1/mafic/node.py` & `mafic-2.1.0/mafic/node.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Node class to represent one Lavalink instance."""
 # SPDX-License-Identifier: MIT
 # pyright: reportImportCycles=false
 # Player import.
 
 from __future__ import annotations
 
 import re
@@ -10,54 +11,56 @@
 from logging import getLogger
 from traceback import print_exc
 from typing import TYPE_CHECKING, Generic, cast
 
 import aiohttp
 import yarl
 
-from mafic.typings.http import TrackWithInfo
-
 from .__libraries import MISSING, ExponentialBackoff, dumps, loads
 from .errors import *
 from .ip import (
     BalancingIPRoutePlannerStatus,
     NanoIPRoutePlannerStatus,
     RotatingIPRoutePlannerStatus,
     RotatingNanoIPRoutePlannerStatus,
 )
 from .playlist import Playlist
 from .plugin import Plugin
 from .region import Group, Region, VoiceRegion
 from .stats import NodeStats
 from .track import Track
 from .type_variables import ClientT
+from .typings import (
+    BalancingIPRouteDetails,
+    NanoIPRouteDetails,
+    RotatingIPRouteDetails,
+    RotatingNanoIPRouteDetails,
+    TrackWithInfo,
+)
 from .warnings import *
 
 if TYPE_CHECKING:
     from asyncio import Task
-    from typing import Any, Literal, Sequence
+    from collections.abc import Sequence
+    from typing import Any, Literal
 
     from aiohttp import ClientWebSocketResponse
 
     from .__libraries import VoiceServerUpdatePayload
     from .filter import Filter
     from .ip import RoutePlannerStatus
     from .player import Player
     from .typings import (
-        BalancingIPRouteDetails,
         Coro,
         EventPayload,
         IncomingMessage,
-        NanoIPRouteDetails,
         OutgoingMessage,
         OutgoingParams,
         Player as PlayerPayload,
         PluginData,
-        RotatingIPRouteDetails,
-        RotatingNanoIPRouteDetails,
         RoutePlannerStatus as RoutePlannerStatusPayload,
         TrackInfo,
         TrackLoadingResult,
         UpdatePlayerParams,
         UpdatePlayerPayload,
     )
 
@@ -66,27 +69,26 @@
 
 __all__ = ("Node",)
 
 
 def _wrap_regions(
     regions: Sequence[Group | Region | VoiceRegion] | None,
 ) -> list[VoiceRegion] | None:
-    """Converts a list of voice regions, regions and groups into a list of regions.
+    r"""Convert a list of voice regions, regions and groups into a list of regions.
 
     Parameters
     ----------
     regions:
         The list of regions to convert.
 
     Returns
     -------
-    :class:`list`\\[:class:`Region`] | None
+    :class:`list`\[:class:`Region`] | None
         The converted list of regions.
     """
-
     if not regions:
         return None
 
     actual_regions: list[VoiceRegion] = []
 
     for item in regions:
         if isinstance(item, Group):
@@ -95,23 +97,22 @@
         elif isinstance(item, Region):
             actual_regions.append(item.value)
         elif isinstance(
             item, VoiceRegion
         ):  # pyright: ignore[reportUnnecessaryIsInstance]
             actual_regions.append(item)
         else:
-            raise TypeError(
-                f"Expected Group, Region, or VoiceRegion, got {type(item)!r}."
-            )
+            msg = f"Expected Group, Region, or VoiceRegion, got {type(item)!r}."
+            raise TypeError(msg)
 
     return actual_regions
 
 
 class Node(Generic[ClientT]):
-    """Represents a Lavalink node.
+    r"""Represents a Lavalink node.
 
     .. warning::
 
         This class should not be instantiated manually.
         Instead, use :meth:`NodePool.create_node`.
 
     Parameters
@@ -130,45 +131,47 @@
         Whether the node is using a secure connection.
         This determines whether the node uses HTTP or HTTPS, WS or WSS.
     heartbeat:
         The interval at which the node will send a heartbeat to the client.
     timeout:
         The amount of time the node will wait for a response before raising a timeout
         error.
-    session: :data:`~typing.Optional`\\[:class:`aiohttp.ClientSession`]
+    session: :data:`~typing.Optional`\[:class:`aiohttp.ClientSession`]
         The session to use for the node.
         If not provided, a new session will be created.
     resume_key:
         The key to use when resuming the node.
         If not provided, the key will be generated from the host, port and label.
     regions:
         The voice regions that the node can be used in.
         This is used to determine when to use this node.
     shard_ids:
         The shard IDs that the node can be used in.
         This is used to determine when to use this node.
 
     Attributes
     ----------
-    regions: :data:`~typing.Optional`\\[:class:`list`\\[:class:`~mafic.region.VoiceRegion`]]
+    regions: :data:`~typing.Optional`\[:class:`list`\[:class:`~.VoiceRegion`]]
         The regions that the node can be used in.
         This is used to determine when to use this node.
-    shard_ids: :data:`~typing.Optional`\\[:class:`list`\\[:class:`int`]]
+    shard_ids: :data:`~typing.Optional`\[:class:`list`\[:class:`int`]]
         The shard IDs that the node can be used in.
         This is used to determine when to use this node.
     """
 
     __slots__ = (
         "__password",
         "__session",
         "_available",
         "_client",
+        "_connect_task",
         "_heartbeat",
         "_host",
         "_label",
+        "_msg_tasks",
         "_players",
         "_port",
         "_resume_key",
         "_secure",
         "_timeout",
         "_ready",
         "_rest_uri",
@@ -222,42 +225,40 @@
         self._ready = Event()
 
         self._players: dict[int, Player[ClientT]] = {}
 
         self._stats: NodeStats | None = None
         self._session_id: str | None = None
 
+        self._msg_tasks: set[Task[None]] = set()
+        self._connect_task: Task[None] | None = None
+
     @property
     def host(self) -> str:
         """The host of the node."""
-
         return self._host
 
     @property
     def port(self) -> int:
         """The port of the node."""
-
         return self._port
 
     @property
     def label(self) -> str:
         """The label of the node."""
-
         return self._label
 
     @property
     def client(self) -> ClientT:
         """The client that the node is attached to."""
-
         return self._client
 
     @property
     def secure(self) -> bool:
         """Whether the node is using a secure connection."""
-
         return self._secure
 
     @property
     def stats(self) -> NodeStats | None:
         """The stats of the node.
 
         This will be ``None`` if the node has not sent stats yet.
@@ -268,15 +269,14 @@
 
     @property
     def available(self) -> bool:
         """Whether the node is available.
 
         This is ``False`` if the node is not connected, or if it is not ready.
         """
-
         return self._available
 
     @property
     def weight(self) -> float:
         """The weight of the node.
 
         This is used to determine which node to use when multiple nodes are available.
@@ -291,15 +291,14 @@
         - The number of UDP frames that are lost.
         - If the node memory is very close to full.
 
         If the node has not sent stats yet, then a high value will be returned.
         This is so that the node will be used if it is the only one available,
         or if stats sending is disabled on the node.
         """
-
         if self._stats is None:
             # Stats haven't been set yet, so we'll just return a high value.
             # This is so we can properly balance known nodes.
             # If stats sending is turned off
             # - that's on the user
             # - they likely have done it on all if they have multiple, so it is equal
             return 6.63e34
@@ -360,44 +359,41 @@
     def players(self) -> list[Player[ClientT]]:
         """The players connected to the node.
 
         .. versionchanged:: 2.0
 
             This is now a list.
         """
-
         return [*self._players.values()]
 
     def get_player(self, guild_id: int) -> Player[ClientT] | None:
-        """Get a player from the node.
+        r"""Get a player from the node.
 
         Parameters
         ----------
         guild_id:
             The guild ID to get the player for.
 
         Returns
         -------
-        :data:`~typing.Optional`\\[:class:`Player`]
+        :data:`~typing.Optional`\[:class:`Player`]
             The player for the guild, if found.
         """
-
         return self._players.get(guild_id)
 
     def add_player(self, guild_id: int, player: Player[ClientT]) -> None:
         """Add a player to the node.
 
         Parameters
         ----------
         guild_id:
             The guild ID to add the player for.
         player:
             The player to add.
         """
-
         self._players[guild_id] = player
 
     def remove_player(self, guild_id: int) -> None:
         """Remove a player from the node.
 
         .. note::
 
@@ -405,15 +401,14 @@
             This simply exists to remove the player from the node cache.
 
         Parameters
         ----------
         guild_id:
             The guild ID to remove the player for.
         """
-
         self._players.pop(guild_id, None)
 
     async def _check_version(self) -> None:
         """Check the version of the node.
 
         Raises
         ------
@@ -426,15 +421,14 @@
 
         Warns
         -----
         :class:`UnsupportedVersionWarning`
             If the minor version is greater than 7.
             Some features may not work.
         """
-
         if self._rest_uri.path.endswith("/v3") or self._ws_uri.path.endswith(
             "/websocket"
         ):
             # This process was already ran likely.
             return
 
         if self.__session is None:
@@ -452,22 +446,17 @@
             except ValueError:
                 message = UnknownVersionWarning.message
                 warnings.warn(message, UnknownVersionWarning)
             else:
                 major = int(major)
                 minor = int(minor)
 
-                if major != 3:
-                    raise RuntimeError(
-                        f"Unsupported lavalink version {version} (expected 3.7.x)"
-                    )
-                elif minor < 7:
-                    raise RuntimeError(
-                        f"Unsupported lavalink version {version} (expected 3.7.x)"
-                    )
+                if major != 3 or minor < 7:
+                    msg = f"Unsupported lavalink version {version} (expected 3.7.x)"
+                    raise RuntimeError(msg)
                 elif minor > 7:
                     message = UnsupportedVersionWarning.message
                     warnings.warn(message, UnsupportedVersionWarning)
 
             self._rest_uri /= "v3"
             self._ws_uri /= "v3/websocket"
 
@@ -479,15 +468,14 @@
         Parameters
         ----------
         headers:
             The headers to use for the websocket connection.
         session:
             The session to use for the websocket connection.
         """
-
         try:
             self._ws = (
                 await session.ws_connect(  # pyright: ignore[reportUnknownMemberType]
                     self._ws_uri,
                     timeout=self._timeout,
                     heartbeat=self._heartbeat,
                     headers=headers,
@@ -516,21 +504,22 @@
         ------
         NodeAlreadyConnected
             If the node is already connected.
         asyncio.TimeoutError
             If the connection times out.
             You can change the timeout with the `timeout` parameter.
         """
-
         if self._ws is not None:
-            raise NodeAlreadyConnected()
+            raise NodeAlreadyConnected
 
         _log.info("Waiting for client to be ready...", extra={"label": self._label})
         await self._client.wait_until_ready()
-        assert self._client.user is not None
+        if self._client.user is None:
+            msg = "Client.user is None"
+            raise RuntimeError(msg)
 
         if self.__session is None:
             self.__session = await self._create_session()
 
         session = self.__session
 
         headers: dict[str, str] = {
@@ -546,33 +535,40 @@
         _log.info(
             "Connecting to lavalink at %s...",
             self._rest_uri,
             extra={"label": self._label},
         )
         try:
             await self._connect_to_websocket(headers=headers, session=session)
-        except Exception:
+        except Exception as e:  # noqa: BLE001
             _log.error(
-                "Failed to connect to lavalink at %s",
+                "Failed to connect to lavalink at %s: %s",
                 self._rest_uri,
+                e,
                 extra={"label": self._label},
             )
             print_exc()
 
             backoff = backoff or ExponentialBackoff()
             delay = backoff.delay()
             _log.info(
                 "Retrying connection to lavalink at %s in %s seconds...",
                 self._rest_uri,
                 delay,
                 extra={"label": self._label},
             )
             await sleep(delay)
 
-            create_task(self.connect(backoff=backoff))
+            task = create_task(self.connect(backoff=backoff))
+            self._connect_task = task
+
+            def remove_task(_: Task[None]) -> None:
+                self._connect_task = None
+
+            task.add_done_callback(remove_task)
 
         _log.info("Connected to lavalink.", extra={"label": self._label})
 
         _log.debug(
             "Creating task for websocket listener...", extra={"label": self._label}
         )
         self._ws_task = create_task(
@@ -593,25 +589,23 @@
                 "Node %s is now available.", self._label, extra={"label": self._label}
             )
             await self.sync_players()
             self._available = True
 
     async def _ws_listener(self) -> None:
         """Listen for messages from the websocket."""
-
         backoff = ExponentialBackoff()
 
         if self._ws is None:
             _log.error(
                 "No websocket was found, aborting listener.",
                 extra={"label": self._label},
             )
-            raise RuntimeError(
-                "Websocket is not connected but attempted to listen, report this."
-            )
+            msg = "Websocket is not connected but attempted to listen, report this."
+            raise RuntimeError(msg)
 
         # To catch closing messages, we cannot use async for.
         while True:
             msg = await self._ws.receive()
 
             _log.debug("Received message from websocket.", extra={"label": self._label})
 
@@ -633,32 +627,39 @@
                     self._port,
                     close_code,
                     wait_time,
                     extra={"label": self._label},
                 )
 
                 await sleep(wait_time)
-                create_task(self.connect(backoff=backoff))
+                task = create_task(self.connect(backoff=backoff))
+                self._connect_task = task
+
+                def remove_task(_: Task[None]) -> None:
+                    self._connect_task = None
+
+                task.add_done_callback(remove_task)
                 return
             else:
                 _log.debug(
                     "Creating task to handle websocket message.",
                     extra={"label": self._label},
                 )
-                create_task(self._handle_msg(msg.json(loads=loads)))
+                task = create_task(self._handle_msg(msg.json(loads=loads)))
+                self._msg_tasks.add(task)
+                task.add_done_callback(self._msg_tasks.discard)
 
     async def _handle_msg(self, data: IncomingMessage) -> None:
         """Handle a message from the websocket.
 
         Parameters
         ----------
         data:
             The data to handle.
         """
-
         _log.debug("Received event with op %s", data["op"])
         _log.debug("Event data: %s", data)
 
         if data["op"] == "playerUpdate":
             guild_id = int(data["guildId"])
             player = self.get_player(guild_id)
 
@@ -708,15 +709,14 @@
         """Handle an event from the websocket.
 
         Parameters
         ----------
         data:
             The data to handle.
         """
-
         if not (player := self.get_player(int(data["guildId"]))):
             _log.error(
                 "Could not find player for guild %s, discarding event.", data["guildId"]
             )
             return
 
         player.dispatch_event(data)
@@ -739,21 +739,21 @@
             The voice server update payload to send.
 
         Raises
         ------
         :exc:`ValueError`
             If the endpoint in the payload is ``None``.
         """
-
         _log.debug(
             "Sending player update to lavalink.",
             extra={"label": self._label, "guild": guild_id},
         )
         if data["endpoint"] is None:
-            raise ValueError("Discord did not provide an endpoint.")
+            msg = "Discord did not provide an endpoint."
+            raise ValueError(msg)
 
         return self.__request(
             "PATCH",
             f"sessions/{self._session_id}/players/{guild_id}",
             {
                 "voice": {
                     "sessionId": session_id,
@@ -761,15 +761,14 @@
                     "token": data["token"],
                 },
             },
         )
 
     def configure_resuming(self) -> Coro[None]:
         """Configure the node to resume."""
-
         _log.info(
             "Sending resume configuration to lavalink with resume key %s.",
             self._resume_key,
             extra={"label": self._label},
         )
 
         return self.__request(
@@ -785,15 +784,14 @@
         """Destroy a player.
 
         Parameters
         ----------
         guild_id:
             The guild ID to destroy the player for.
         """
-
         _log.debug("Sending request to destroy player", extra={"label": self._label})
 
         return self.__request(
             "DELETE", f"sessions/{self._session_id}/players/{guild_id}"
         )
 
     def update(
@@ -826,15 +824,14 @@
         no_replace:
             Whether to replace the current track or leave it playing.
         pause:
             Whether to pause the player.
         filter:
             The filter to apply to the player.
         """
-
         data: UpdatePlayerPayload = {}
 
         if track is not MISSING:
             data["encodedTrack"] = track.id if track is not None else None
 
         if position is not None:
             data["position"] = position
@@ -867,24 +864,23 @@
             f"sessions/{self._session_id}/players/{guild_id}",
             data,
             query,
         )
 
     async def _create_session(self) -> aiohttp.ClientSession:
         """Create a new session for the node."""
-
         return aiohttp.ClientSession(json_serialize=dumps)
 
     async def __request(
         self,
         method: str,
         path: str,
         json: OutgoingMessage | None = None,
         params: OutgoingParams | None = None,
-    ) -> Any:
+    ) -> Any:  # noqa: ANN401
         """Send a request to the node.
 
         Parameters
         ----------
         method:
             The HTTP method to use.
         path:
@@ -895,15 +891,14 @@
             The query parameters to send.
 
         Returns
         -------
         :data:`~typing.Any`
             The JSON response from the node.
         """
-
         if self.__session is None:
             self.__session = await self._create_session()
 
         session = self.__session
         uri = self._rest_uri / path
 
         _log.debug(
@@ -943,33 +938,32 @@
             json = await resp.json(loads=loads)
             _log.debug("Received raw data %s from %s", json, path)
             return json
 
     async def fetch_tracks(
         self, query: str, *, search_type: str
     ) -> list[Track] | Playlist | None:
-        """Fetch tracks from the node.
+        r"""Fetch tracks from the node.
 
         Parameters
         ----------
         query:
             The query to search for.
         search_type:
             The search type to use.
 
         Returns
         -------
-        :class:`list`\\[:class:`Track`]
+        :class:`list`\[:class:`Track`]
             A list of tracks if the load type is ``TRACK_LOADED`` or ``SEARCH_RESULT``.
         :class:`Playlist`
             A playlist if the load type is ``PLAYLIST_LOADED``.
         None
             If the load type is ``NO_MATCHES``.
         """
-
         if not URL_REGEX.match(query):
             query = f"{search_type}:{query}"
 
         data: TrackLoadingResult = await self.__request(
             "GET", "loadtracks", params={"identifier": query}
         )
 
@@ -981,14 +975,15 @@
             return Playlist(info=data["playlistInfo"], tracks=data["tracks"])
         elif data["loadType"] == "SEARCH_RESULT":
             return [Track.from_data_with_info(track) for track in data["tracks"]]
         elif data["loadType"] == "LOAD_FAILED":
             raise TrackLoadException.from_data(data["exception"])
         else:
             _log.warning("Unknown load type recieved: %s", data["loadType"])
+            return None
 
     async def decode_track(self, track: str) -> Track:
         """Decode a track from the encoded base64 data.
 
         Parameters
         ----------
         track:
@@ -999,67 +994,63 @@
         :class:`Track`
             The decoded track.
 
         See Also
         --------
         :meth:`decode_tracks`
         """
-
         info: TrackInfo = await self.__request(
             "GET", "decodetrack", params={"encodedTrack": track}
         )
 
         return Track.from_data(track=track, info=info)
 
     async def decode_tracks(self, tracks: list[str]) -> list[Track]:
-        """Decode a list of tracks from the encoded base64 data.
+        r"""Decode a list of tracks from the encoded base64 data.
 
         Parameters
         ----------
         tracks:
             The encoded track data.
 
         Returns
         -------
-        :class:`list`\\[:class:`Track`]
+        :class:`list`\[:class:`Track`]
             The decoded tracks.
 
         See Also
         --------
         :meth:`decode_track`
         """
-
         track_data: list[TrackWithInfo] = await self.__request(
             "POST", "decodetracks", json=tracks
         )
 
         return [Track.from_data_with_info(track) for track in track_data]
 
     async def fetch_plugins(self) -> list[Plugin]:
-        """Fetch the plugins from the node.
+        r"""Fetch the plugins from the node.
 
         Returns
         -------
-        :class:`list`\\[:class:`Plugin`]
+        :class:`list`\[:class:`Plugin`]
             The plugins from the node.
         """
-
         plugins: list[PluginData] = await self.__request("GET", "plugins")
 
         return [Plugin(plugin) for plugin in plugins]
 
     async def fetch_route_planner_status(self) -> RoutePlannerStatus | None:
         """Fetch the route planner status from the node.
 
         Returns
         -------
         :data:`.RoutePlannerStatus`
             The route planner status from the node.
         """
-
         data: RoutePlannerStatusPayload = await self.__request(
             "GET", "routeplanner/status"
         )
 
         if data["class"] == "RotatingIpRoutePlanner":
             return RotatingIPRoutePlannerStatus(
                 cast(RotatingIPRouteDetails, data["details"])
@@ -1073,45 +1064,43 @@
         elif data["class"] == "BalancingIpRoutePlanner":
             return BalancingIPRoutePlannerStatus(
                 cast(BalancingIPRouteDetails, data["details"])
             )
         elif data["class"] is None:
             return None
         else:
-            raise RuntimeError(f"Unknown route planner class {data['class']}.")
+            msg = f"Unknown route planner class {data['class']}."
+            raise RuntimeError(msg)
 
     async def unmark_failed_address(self, address: str) -> None:
         """Unmark a failed address so it can be used again.
 
         Parameters
         ----------
         address:
             The address to unmark.
         """
-
         await self.__request(
             "POST", "routeplanner/free/address", json={"address": address}
         )
 
     async def unmark_all_addresses(self) -> None:
         """Unmark all failed addresses so they can be used again."""
-
         await self.__request("POST", "routeplanner/free/all")
 
     async def _add_unknown_player(self, player_id: int, state: PlayerPayload) -> None:
         """Add an unknown player to the node.
 
         Parameters
         ----------
         player_id:
             The guild ID of the player.
         state:
             The state of the player.
         """
-
         guild = self.client.get_guild(player_id)
         if guild is None:
             guild = await self.client.fetch_guild(player_id)
 
         voice_state = guild.me.voice
 
         if voice_state is None:
@@ -1135,27 +1124,25 @@
         """Remove an unknown player from the node.
 
         Parameters
         ----------
         player_id:
             The guild ID of the player.
         """
-
         await self._players[player_id].disconnect(force=True)
         self.remove_player(player_id)
 
     async def sync_players(self) -> None:
         """Sync the players with the node.
 
         .. note::
 
             This method is called automatically when the client is ready.
             You should not need to call this method yourself.
         """
-
         players: list[PlayerPayload] = await self.__request(
             "GET", f"sessions/{self._session_id}/players"
         )
         actual_players = {int(player["guildId"]): player for player in players}
         actual_player_ids = set(actual_players.keys())
         expected_player_ids = set(self._players.keys())
```

### Comparing `mafic-2.0.1/mafic/player.py` & `mafic-2.1.0/mafic/player.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""A Player is used to connect to a channel."""
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 from collections import OrderedDict
 from functools import reduce
 from logging import getLogger
@@ -15,28 +16,28 @@
     StageChannel,
     VoiceChannel,
     VoiceProtocol,
 )
 from .errors import NoNodesAvailable, PlayerNotConnected
 from .events import *
 from .filter import Filter
-from .playlist import Playlist
 from .pool import NodePool
 from .search_type import SearchType
 from .track import Track
 from .type_variables import ClientT
 
 if TYPE_CHECKING:
     from .__libraries import (
         Connectable,
         Guild,
         GuildVoiceStatePayload,
         VoiceServerUpdatePayload,
     )
     from .node import Node
+    from .playlist import Playlist
     from .typings import EventPayload, Player as PlayerPayload, PlayerUpdateState
 
 
 _log = getLogger(__name__)
 __all__ = ("Player",)
 
 
@@ -76,15 +77,16 @@
         *,
         node: Node[ClientT] | None = None,
     ) -> None:
         self.client: ClientT = client
         self.channel: Connectable = channel
 
         if not isinstance(self.channel, GuildChannel):
-            raise TypeError("Voice channel must be a GuildChannel.")
+            msg = "Voice channel must be a GuildChannel."
+            raise TypeError(msg)
 
         self.guild: Guild = self.channel.guild
 
         self._node = node
 
         self._guild_id: int = self.guild.id
         self._session_id: str | None = None
@@ -103,15 +105,14 @@
         """Set the state of the player.
 
         .. note::
 
             This is used internally to set the state of the player.
             You should not need to use this.
         """
-
         self._session_id = state["voice"]["sessionId"]
         self._ping = state["voice"]["ping"]
         self._current = (
             Track.from_data_with_info(state["track"]) if state["track"] else None
         )
         self._filters = OrderedDict({"RESUME": Filter.from_payload(state["filters"])})
         self._paused = state["paused"]
@@ -120,104 +121,96 @@
             "endpoint": state["voice"]["endpoint"],
             "guild_id": self._guild_id,
         }
         if state["track"]:
             self._position = state["track"]["info"]["position"]
 
     def __repr__(self) -> str:
+        """Return a string representation of the player."""
         attrs = (
             ("guild_id", self._guild_id),
             ("session_id", self._session_id),
             ("connected", self._connected),
             ("position", self._position),
             ("current", self._current),
         )
         resolved = " ".join(f"{attr}={value!r}" for attr, value in attrs)
         return f"<{type(self).__name__} {resolved}>"
 
     @property
     def connected(self) -> bool:
         """Whether the player is connected to a voice channel."""
-
         return self._connected
 
     @property
     def position(self) -> int:
         """The current position of the player in milliseconds."""
-
         pos = self._position
 
         if self._connected and self._current is not None:
             # Add the time since the last update to the position.
             # If the track total time is less than that, use that.
             pos = min(
-                self._current.length, pos + int(((time() * 1000) - self._last_update))
+                self._current.length, pos + int((time() * 1000) - self._last_update)
             )
 
         return pos
 
     @property
     def ping(self) -> int:
         """The current ping of the player in milliseconds."""
-
         return self._ping
 
     @property
     def node(self) -> Node[ClientT]:
         """The node that the player is connected to."""
-
         if self._node is None:
             _log.warning(
                 "Unable to use best node, player not connected, finding random node.",
                 extra={"guild": self._guild_id},
             )
             return NodePool[ClientT].get_random_node()
 
         return self._node
 
     @property
     def current(self) -> Track | None:
         """The current track that is playing."""
-
         return self._current
 
     @property
     def paused(self) -> bool:
         """Whether the player is paused."""
-
         return self._paused
 
     def update_state(self, state: PlayerUpdateState) -> None:
         """Update the player state.
 
         This is called by the library and usually should not be called by the user.
 
         Parameters
         ----------
         state:
             The state to update the player with.
         """
-
         self._last_update = state["time"]
         self._position = state.get("position", 0)
         self._connected = state["connected"]
         self._ping = state.get("ping", -1)
 
     # If people are so in love with the VoiceClient interface
     def is_connected(self) -> bool:
         """Whether the player is connected to a voice channel.
 
         This is an alias for :attr:`connected`.
         """
-
         return self._connected
 
     async def _dispatch_player_update(self) -> None:
         """Dispatch a player update to the node."""
-
         if self._node is None:
             _log.debug("Recieved voice update before node was found.")
             return
 
         if self._session_id is None:
             _log.debug("Receieved player update before session ID was set.")
             return
@@ -229,14 +222,23 @@
         await self._node.voice_update(
             guild_id=self._guild_id,
             session_id=self._session_id,
             data=self._server_state,
         )
 
     def dispatch_event(self, data: EventPayload) -> None:
+        """Dispatch an event to the player.
+
+        This is called by the library and usually should not be called by the user.
+
+        Parameters
+        ----------
+        data:
+            The event payload to dispatch.
+        """
         if data["type"] == "WebSocketClosedEvent":
             event = WebSocketClosedEvent(payload=data, player=self)
             _log.debug("Received websocket closed event: %s", event)
             self.client.dispatch("websocket_closed", event)
         elif data["type"] == "TrackStartEvent":
             track = self._current
 
@@ -266,15 +268,16 @@
             if data["reason"] != "REPLACED":
                 self._current = None
         elif data["type"] == "TrackExceptionEvent":
             track = self._current
 
             if track is None:
                 _log.error(
-                    "Received track exception event but no track was playing, discarding."
+                    "Received track exception event but no track was playing, "
+                    "discarding."
                 )
                 return
 
             event = TrackExceptionEvent(player=self, track=track, payload=data)
             self.client.dispatch("track_exception", event)
             _log.debug("Received track exception event: %s", event)
         elif data["type"] == "TrackStuckEvent":
@@ -302,43 +305,44 @@
         This is called by the library and usually should not be called by the user.
 
         Parameters
         ----------
         data:
             The voice state update payload.
         """
-
         before_session_id = self._session_id
         self._session_id = data["session_id"]
 
         channel_id = data["channel_id"]
 
         if channel_id is None:  # pyright: ignore[reportUnnecessaryComparison]
-            # This can happen and is on disconnect, not sure why this is typed as always Snowflake.
+            # This can happen and is on disconnect.
+            # Not sure why this is typed as always Snowflake.
             return self.cleanup()
 
         channel = self.guild.get_channel(int(channel_id))
-        assert isinstance(channel, (StageChannel, VoiceChannel))
+        if not isinstance(channel, (VoiceChannel, StageChannel)):
+            msg = "Channel was not a connectable channel that was recognised."
+            raise TypeError(msg)
 
         self.channel = channel
 
-        if self._session_id != before_session_id:
-            await self._dispatch_player_update()
+        if self._session_id != before_session_id:  # noqa: RET503
+            await self._dispatch_player_update()  # noqa: RET503
 
     async def on_voice_server_update(self, data: VoiceServerUpdatePayload) -> None:
         """Handle a voice server update.
 
         This is called by the library and usually should not be called by the user.
 
         Parameters
         ----------
         data:
             The voice server update payload.
         """
-
         # Fetch the best node as we either don't know the best one yet.
         # Or the node we were using was not the best one (endpoint optimisation).
         if (
             self._node is None
             or self._server_state is None
             or self._server_state["endpoint"] != data["endpoint"]
         ):
@@ -358,16 +362,16 @@
         self._server_state = data
 
         await self._dispatch_player_update()
 
     async def connect(
         self,
         *,
-        timeout: float,
-        reconnect: bool,
+        timeout: float,  # noqa: ARG002
+        reconnect: bool,  # noqa: ARG002
         self_mute: bool = False,
         self_deaf: bool = False,
     ) -> None:
         """Connect to a voice channel.
 
         This is called by your Discord library when using ``Connectable.connect``.
 
@@ -378,17 +382,17 @@
         reconnect:
             Whether to reconnect to the voice channel if the connection is lost.
         self_mute:
             Whether to mute the bot on connect.
         self_deaf:
             Whether to deafen the bot on connect.
         """
-
         if not isinstance(self.channel, (VoiceChannel, StageChannel)):
-            raise TypeError("Voice channel must be a VoiceChannel or StageChannel.")
+            msg = "Voice channel must be a VoiceChannel or StageChannel."
+            raise TypeError(msg)
 
         if not NodePool.nodes:
             raise NoNodesAvailable
 
         _log.debug("Connecting to voice channel %s", self.channel.id)
 
         await self.channel.guild.change_voice_state(
@@ -400,15 +404,14 @@
         """Disconnect from the voice channel.
 
         Parameters
         ----------
         force:
             Whether to force the disconnect even if not connected.
         """
-
         if not self._connected and not force:
             return
 
         # Handled by Discord
         if self.client.is_closed():
             return
 
@@ -423,67 +426,64 @@
             self._connected = False
 
     def cleanup(self) -> None:
         """Clean up the player.
 
         This shouldn't be called directly. Instead, use :meth:`disconnect`.
         """
-
         self._current = None
         self._position = 0
         self._paused = False
         self._ping = 0
         self._channel = None
         self._connected = False
 
         return super().cleanup()
 
     async def destroy(self) -> None:
         """Destroy the player.
 
         This will disconnect the player and remove it from the node.
         """
-
         _log.debug(
             "Disconnecting player and destroying client.",
             extra={"guild": self._guild_id},
         )
         await self.disconnect()
 
         if self._node is not None:
             self._node.remove_player(self.guild.id)
             await self._node.destroy(guild_id=self.guild.id)
 
     async def fetch_tracks(
         self, query: str, search_type: SearchType | str = SearchType.YOUTUBE
     ) -> list[Track] | Playlist | None:
-        """Fetch tracks from the node.
+        r"""Fetch tracks from the node.
 
         Parameters
         ----------
         query:
             The query to search for.
         search_type:
             The search type to use.
 
         Returns
         -------
-        :class:`list`\\[:class:`Track`]
+        :class:`list`\[:class:`Track`]
             A list of tracks if the load type is ``TRACK_LOADED`` or ``SEARCH_RESULT``.
         :class:`Playlist`
             A playlist if the load type is ``PLAYLIST_LOADED``.
         None
             If the load type is ``NO_MATCHES``.
 
         Notes
         -----
         If a node was not selected due to not being connected, this will use a
         random node.
         """
-
         node = self.node
 
         raw_type: str
         if isinstance(search_type, SearchType):
             raw_type = search_type.value
         else:
             raw_type = search_type
@@ -521,15 +521,14 @@
             Whether to replace the current track if one is playing.
 
         Raises
         ------
         PlayerNotConnected
             If the player is not connected to a voice channel.
         """
-
         if self._node is None or not self._connected:
             raise PlayerNotConnected
 
         if track is not MISSING:
             self._current = track
 
         if position is not None:
@@ -582,25 +581,24 @@
         PlayerNotConnected
             If the player is not connected to a voice channel.
 
         Notes
         -----
         This is a convenience method for :meth:`update`.
         """
-
         return await self.update(
             track=track,
             position=start_time,
             end_time=end_time,
             volume=volume,
             replace=replace,
             pause=pause,
         )
 
-    async def pause(self, pause: bool = True) -> None:
+    async def pause(self, pause: bool = True) -> None:  # noqa: FBT
         """Pause the current track.
 
         Parameters
         ----------
         pause:
             Whether to pause the track.
 
@@ -609,15 +607,14 @@
         PlayerNotConnected
             If the player is not connected to a voice channel.
 
         Notes
         -----
         This is a convenience method for :meth:`update`.
         """
-
         return await self.update(pause=pause)
 
     async def resume(self) -> None:
         """Resume the current track.
 
         Raises
         ------
@@ -625,41 +622,38 @@
             If the player is not connected to a voice channel.
 
         Notes
         -----
         This is a convenience method for :meth:`pause`, with ``pause`` set to
         ``False``.
         """
-
-        return await self.pause(False)
+        return await self.pause(False)  # noqa: FBT003
 
     async def stop(self) -> None:
         """Stop the current track.
 
         Raises
         ------
         PlayerNotConnected
             If the player is not connected to a voice channel.
 
         Notes
         -----
         This is a convenience method for :meth:`update`.
         """
-
         await self.update(track=None, replace=True)
 
     async def _update_filters(self, *, fast_apply: bool) -> None:
         """Update the filters on the player.
 
         Parameters
         ----------
         fast_apply:
             Whether to seek to the current position after updating the filters.
         """
-
         await self.update(
             filter=reduce(or_, self._filters.values()) if self._filters else Filter()
         )
 
         if fast_apply:
             await self.seek(self.position)
 
@@ -681,19 +675,35 @@
             delay in the audio.
 
         Raises
         ------
         PlayerNotConnected
             If the player is not connected to a voice channel.
         """
-
         self._filters[label] = filter
 
         await self._update_filters(fast_apply=fast_apply)
 
+    async def has_filter(self, label: str) -> bool:
+        """Check if the player has a filter with the given label.
+
+        .. versionadded:: 2.1
+
+        Parameters
+        ----------
+        label:
+            The label to check for.
+
+        Returns
+        -------
+        :class:`bool`
+            Whether the player has a filter with the given label.
+        """
+        return label in self._filters
+
     async def remove_filter(self, label: str, *, fast_apply: bool = False) -> None:
         """Remove a filter from the player.
 
         Parameters
         ----------
         label:
             The label of the filter to remove.
@@ -705,15 +715,14 @@
         Raises
         ------
         PlayerNotConnected
             If the player is not connected to a voice channel.
         ValueError
             If the filter does not exist.
         """
-
         self._filters.pop(label)
 
         await self._update_filters(fast_apply=fast_apply)
 
     async def clear_filters(self, *, fast_apply: bool = False) -> None:
         """Remove all filters from the player.
 
@@ -725,15 +734,14 @@
             delay in the audio.
 
         Raises
         ------
         PlayerNotConnected
             If the player is not connected to a voice channel.
         """
-
         self._filters.clear()
 
         await self._update_filters(fast_apply=fast_apply)
 
     async def set_volume(self, volume: int, /) -> None:
         """Set the volume of the player.
 
@@ -747,15 +755,14 @@
         PlayerNotConnected
             If the player is not connected to a voice channel.
 
         Notes
         -----
         This is a convenience method for :meth:`update`.
         """
-
         await self.update(volume=volume)
 
     async def seek(self, position: int, /) -> None:
         """Seek to a position in the current track.
 
         Parameters
         ----------
@@ -767,9 +774,8 @@
         PlayerNotConnected
             If the player is not connected to a voice channel.
 
         Notes
         -----
         This is a convenience method for :meth:`update`.
         """
-
         return await self.update(position=position)
```

### Comparing `mafic-2.0.1/mafic/playlist.py` & `mafic-2.1.0/mafic/playlist.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""The module containing :class:`Playlist`."""
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from .track import Track
@@ -9,27 +10,27 @@
 if TYPE_CHECKING:
     from .typings import PlaylistInfo, TrackWithInfo
 
 __all__ = ("Playlist",)
 
 
 class Playlist:
-    """Represents a playlist.
+    r"""Represents a playlist.
 
     Attributes
     ----------
     name: :class:`str`
         The name of the playlist.
     selected_track: :class:`int`
         The index of the selected track, if any.
-    tracks: :class:`list`\\[:class:`Track`]
+    tracks: :class:`list`\[:class:`Track`]
         A list of tracks in the playlist.
     """
 
     __slots__ = ("name", "selected_track", "tracks")
 
-    def __init__(self, *, info: PlaylistInfo, tracks: list[TrackWithInfo]):
+    def __init__(self, *, info: PlaylistInfo, tracks: list[TrackWithInfo]) -> None:
         self.name: str = info["name"]
         self.selected_track: int = info["selectedTrack"]
         self.tracks: list[Track] = [
             Track.from_data_with_info(track) for track in tracks
         ]
```

### Comparing `mafic-2.0.1/mafic/plugin.py` & `mafic-2.1.0/mafic/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""The Lavalink plugin system."""
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
```

### Comparing `mafic-2.0.1/mafic/pool.py` & `mafic-2.1.0/mafic/pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+r"""A module containing a :class:`NodePool`, used to manage :class:`Node`\s."""
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 from collections.abc import Sequence
 from functools import partial
 from logging import getLogger
@@ -81,22 +82,20 @@
             ]
             if default_strategies is None
             else default_strategies
         )
 
     @classproperty
     def label_to_node(cls) -> dict[str, Node[ClientT]]:
-        """A dictionary mapping node labels to nodes."""
-
+        """Get a mapping node labels to nodes."""
         return cls._nodes
 
     @classproperty
     def nodes(cls) -> list[Node[ClientT]]:
-        """A list of all nodes."""
-
+        """Get the list of all nodes."""
         return list(cls._nodes.values())
 
     async def create_node(
         self,
         *,
         host: str,
         port: int,
@@ -106,15 +105,15 @@
         heartbeat: int = 30,
         timeout: float = 10,
         session: aiohttp.ClientSession | None = None,
         resume_key: str | None = None,
         regions: Sequence[Group | Region | VoiceRegion] | None = None,
         shard_ids: Sequence[int] | None = None,
     ) -> Node[ClientT]:
-        """Create a node and connect it.
+        r"""Create a node and connect it.
 
         The parameters here relate to :class:`Node`.
 
         Parameters
         ----------
         host:
             The host of the node to connect to.
@@ -126,15 +125,15 @@
             The password of the node to authenticate.
         secure:
             Whether to use SSL (TLS) or not.
         heartbeat:
             The interval to send heartbeats to the node websocket connection.
         timeout:
             The timeout to use for the node websocket connection.
-        session: :data:`~typing.Optional`\\ [:class:`aiohttp.ClientSession`]
+        session: :data:`~typing.Optional`\[:class:`aiohttp.ClientSession`]
             The session to use for the node websocket connection.
         resume_key:
             The key to use to resume the node websocket connection.
             This is used to resume a connection if the connection is lost.
             Defaults to using the `host`, `port` and `label`.
         regions:
             The regions this node is best to connect to.
@@ -151,17 +150,17 @@
             The created node.
 
         Raises
         ------
         RuntimeError
             If the node pool has not been initialized.
         """
-
         if self._client is None:
-            raise RuntimeError("NodePool has not been initialized.")
+            msg = "NodePool has not been initialized."
+            raise RuntimeError(msg)
 
         node = Node(
             host=host,
             port=port,
             label=label,
             password=password,
             client=self._client,
@@ -221,26 +220,23 @@
             The node to use.
 
         Raises
         ------
         RuntimeError
             If the node pool has not been initialized.
         """
-
         if cls._client is None:
-            raise RuntimeError("NodePool has not been initialized.")
+            msg = "NodePool has not been initialized."
+            raise RuntimeError(msg)
 
         actual_strategies: Sequence[StrategyCallable[ClientT] | Strategy]
 
         strategies = strategies or cls._default_strategies
 
-        if callable(strategies):
-            actual_strategies = [strategies]
-        else:
-            actual_strategies = strategies
+        actual_strategies = [strategies] if callable(strategies) else strategies
 
         nodes = cls.nodes
 
         for strategy in actual_strategies:
             if isinstance(strategy, Strategy):
                 strategy_callable = partial(call_strategy, strategy)
             else:
@@ -273,12 +269,11 @@
             The random node.
 
         Raises
         ------
         ValueError
             If there are no nodes.
         """
-
         if node := choice(list(cls._nodes.values())):
             return node
 
         raise NoNodesAvailable
```

### Comparing `mafic-2.0.1/mafic/region.py` & `mafic-2.1.0/mafic/region.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""A module contains region enums for voice regions and groups."""
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 from enum import Enum
 
 __all__ = ("Group", "Region", "VoiceRegion")
@@ -47,14 +48,15 @@
     FRANKFURT = "frankfurt"
     LONDON = "london"
     SOUTH_KOREA = "south-korea"
     EUROPE = "europe"
     AMSTERDAM = "amsterdam"
 
     def __repr__(self) -> str:
+        """Get the representation of this voice region."""
         return f"VoiceRegion.{self.name}"
 
 
 class Region(Enum):
     """Represents a region of voice regions.
 
     This groups voice regions by geographical location.
@@ -85,14 +87,15 @@
         VoiceRegion.ROTTERDAM,
         VoiceRegion.LONDON,
         VoiceRegion.AMSTERDAM,
     )
     OCEANIA = (VoiceRegion.SYDNEY,)
 
     def __repr__(self) -> str:
+        """Get the representation of this region."""
         return f"<Region.{self.name}>"
 
 
 class Group(Enum):
     """Represents a group of regions.
 
     This groups regions by geographical location. These are very generic and should
@@ -118,8 +121,9 @@
         Region.EAST_ASIA,
         Region.SOUTH_ASIA,
         Region.WEST_ASIA,
         Region.OCEANIA,
     )
 
     def __repr__(self) -> str:
+        """Get the representation of this group."""
         return f"<Group.{self.name}>"
```

### Comparing `mafic-2.0.1/mafic/search_type.py` & `mafic-2.1.0/mafic/search_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Represents a search type for Lavalink."""
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 from enum import Enum
 
 __all__ = ("SearchType",)
```

### Comparing `mafic-2.0.1/mafic/stats.py` & `mafic-2.1.0/mafic/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""A module containing classes to represent node statistics."""
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 from datetime import timedelta
 from typing import TYPE_CHECKING
 
@@ -80,29 +81,29 @@
     def __init__(self, payload: FrameStatsPayload) -> None:
         self.sent: int = payload["sent"]
         self.nulled: int = payload["nulled"]
         self.deficit: int = payload["deficit"]
 
 
 class NodeStats:
-    """Represents stats for a node.
+    r"""Represents stats for a node.
 
     Attributes
     ----------
     player_count: :class:`int`
         The amount of players connected to the node.
     playing_player_count: :class:`int`
         The amount of players playing on the node.
     uptime: :class:`datetime.timedelta`
         The uptime of the node.
     memory: :class:`MemoryStats`
         The memory stats of the node.
     cpu: :class:`CPUStats`
         The CPU stats of the node.
-    frame_stats: :data:`~typing.Optional`\\[:class:`FrameStats`]
+    frame_stats: :data:`~typing.Optional`\[:class:`FrameStats`]
         The frame stats of the node.
     """
 
     __slots__ = (
         "cpu",
         "frame_stats",
         "memory",
```

### Comparing `mafic-2.0.1/mafic/strategy.py` & `mafic-2.1.0/mafic/strategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+"""The strategy system for selecting a :class:`Node` from a :class:`NodePool`."""
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import re
+from collections.abc import Callable
 from enum import Enum, auto
 from logging import getLogger
 from random import choice
-from typing import Callable, List, Optional
+from typing import List, Optional
 
 from .node import Node
 from .type_variables import ClientT
 
 StrategyCallable = Callable[
     [List[Node[ClientT]], int, Optional[int], Optional[str]], List[Node[ClientT]]
 ]
@@ -39,28 +41,27 @@
     USAGE = auto()
     """Selects a node based on the least used node."""
 
 
 def shard_strategy(
     nodes: list[Node[ClientT]], guild_id: int, shard_count: int | None, _: str | None
 ) -> list[Node[ClientT]]:
-    """Selects a node based on the shard ID of the guild.
+    """Get a node based on the shard ID of the guild.
 
     Parameters
     ----------
     nodes:
         The nodes to select from.
     guild_id:
         The ID of the guild to select a node for.
     shard_count:
         The number of shards the bot is using.
     _:
         Unused parameter.
     """
-
     if shard_count is None:
         shard_count = 1
 
     shard_id = (guild_id >> 22) % shard_count
 
     return list(
         filter(lambda node: node.shard_ids is None or shard_id in node.shard_ids, nodes)
@@ -69,28 +70,27 @@
 
 _REGION_REGEX = re.compile(r"(?:vip-)?(?P<region>[a-z-]{1,15})\d{1,5}\.discord\.media")
 
 
 def location_strategy(
     nodes: list[Node[ClientT]], _: int, __: int | None, endpoint: str | None
 ) -> list[Node[ClientT]]:
-    """Selects a node based on the region the guild is in.
+    """Get a node based on the region the guild is in.
 
     Parameters
     ----------
     nodes:
         The nodes to select from.
     _:
         Unused parameter.
     __:
         Unused parameter.
     endpoint:
         The endpoint of the guild to select a node for.
     """
-
     if endpoint is None:
         return nodes
 
     match = _REGION_REGEX.match(endpoint)
 
     if not match:
         _log.error("Failed to find the region in an endpoint, defaulting to all nodes.")
@@ -120,30 +120,29 @@
 
     return regional_nodes
 
 
 def usage_strategy(
     nodes: list[Node[ClientT]], _: int, __: int | None, ___: str | None
 ) -> list[Node[ClientT]]:
-    """Selects a node based on the least used node.
+    """Get a node based on the least used node.
 
     This is calculated using :attr:`Node.weight`.
 
     Parameters
     ----------
     nodes:
         The nodes to select from.
     _:
         Unused parameter.
     __:
         Unused parameter.
     ___:
         Unused parameter.
     """
-
     # max() would be nice, however if all nodes have no stats, it returns the first.
 
     lowest = None
 
     for node in nodes:
         weight = node.weight
 
@@ -155,58 +154,57 @@
 
     return list(filter(lambda node: node.weight == lowest, nodes))
 
 
 def random_strategy(
     nodes: list[Node[ClientT]], _: int, __: int | None, ___: str | None
 ) -> list[Node[ClientT]]:
-    """Selects a random node.
+    """Get a random node.
 
     Parameters
     ----------
     nodes:
         The nodes to select from.
     _:
         Unused parameter.
     __:
         Unused parameter.
     ___:
         Unused parameter.
     """
-
     return [choice(nodes)]
 
 
 # Used for ClientT preservation.
 def call_strategy(
     strategy: Strategy,
     nodes: list[Node[ClientT]],
     guild_id: int,
     shard_count: int | None,
     endpoint: str | None,
 ) -> list[Node[ClientT]]:
-    """Calls a strategy.
+    """Call a strategy's callback and get the result.
 
     Parameters
     ----------
     strategy:
         The strategy to call.
     nodes:
         The nodes to select from.
     guild_id:
         The ID of the guild to select a node for.
     shard_count:
         The number of shards the bot is using.
     endpoint:
         The endpoint of the voice client to select a node for.
     """
-
     if strategy is Strategy.LOCATION:
         return location_strategy(nodes, guild_id, shard_count, endpoint)
     elif strategy is Strategy.RANDOM:
         return random_strategy(nodes, guild_id, shard_count, endpoint)
     elif strategy is Strategy.SHARD:
         return shard_strategy(nodes, guild_id, shard_count, endpoint)
     elif strategy is Strategy.USAGE:
         return usage_strategy(nodes, guild_id, shard_count, endpoint)
     else:
-        raise ValueError(f"Unknown strategy {strategy}")
+        msg = f"Unknown strategy {strategy}"
+        raise ValueError(msg)
```

### Comparing `mafic-2.0.1/mafic/track.py` & `mafic-2.1.0/mafic/track.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""The module containing :class:`Track`."""
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
@@ -9,15 +10,15 @@
 
     from .typings import TrackInfo, TrackWithInfo
 
 __all__ = ("Track",)
 
 
 class Track:
-    """Represents a track.
+    r"""Represents a track.
 
     Parameters
     ----------
     track_id:
         The ID of the track.
     title:
         The title of the track.
@@ -42,15 +43,15 @@
         The ID of the track. This is base64 encoded data used by Lavalink.
     title: :class:`str`
         The title of the track.
     author: :class:`str`
         The author of the track.
     identifier: :class:`str`
         The identifier of the track. This is the ID of the track on the source.
-    uri: :data:`~typing.Optional`\\[:class:`str`]
+    uri: :data:`~typing.Optional`\[:class:`str`]
         The URI of the track.
     source: :class:`str`
         The source of the track.
     stream: :class:`bool`
         Whether the track is a stream.
     seekable: :class:`bool`
         Whether the track is seekable.
@@ -115,15 +116,14 @@
             The track info.
 
         Returns
         -------
         :class:`Track`
             The track.
         """
-
         return cls(
             track_id=track,
             title=info["title"],
             author=info["author"],
             identifier=info["identifier"],
             uri=info["uri"],
             source=info["sourceName"],
@@ -143,18 +143,18 @@
             The track and info.
 
         Returns
         -------
         :class:`Track`
             The track.
         """
-
         return cls.from_data(track=data["encoded"], info=data["info"])
 
     def __repr__(self) -> str:
+        """Return the string representation of this track."""
         attrs = (
             ("id", self.id),
             ("title", self.title),
             ("author", self.author),
             ("identifier", self.identifier),
             ("uri", self.uri),
             ("source", self.source),
```

### Comparing `mafic-2.0.1/mafic/typings/common.py` & `mafic-2.1.0/mafic/typings/common.py`

 * *Files identical despite different names*

### Comparing `mafic-2.0.1/mafic/typings/http.py` & `mafic-2.1.0/mafic/typings/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # SPDX-License-Identifier: MIT
+# ruff: noqa: UP013
+# `class` in `TypedDict` does not work as that is a reserved keyword
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Literal, Optional, TypedDict, Union
 
-from .common import PlaylistInfo, TrackWithInfo
-
 if TYPE_CHECKING:
     from typing_extensions import NotRequired
 
+    from .common import PlaylistInfo, TrackWithInfo
     from .misc import LavalinkException
 
 
 __all__ = (
     "BalancingIPRouteDetails",
     "BalancingIPRoutePlanner",
     "BaseDetails",
```

### Comparing `mafic-2.0.1/mafic/typings/incoming.py` & `mafic-2.1.0/mafic/typings/incoming.py`

 * *Files identical despite different names*

### Comparing `mafic-2.0.1/mafic/typings/outgoing.py` & `mafic-2.1.0/mafic/typings/outgoing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
-from typing import List, TypedDict, Union
+from typing import TYPE_CHECKING, List, TypedDict, Union
 
-from .common import Filters, VoiceStateRequest
+if TYPE_CHECKING:
+    from .common import Filters, VoiceStateRequest
 
 __all__ = (
     "DecodeTrackParams",
     "OutgoingMessage",
     "OutgoingParams",
     "TrackLoadParams",
     "UnmarkAddressPayload",
```

### Comparing `mafic-2.0.1/mafic/utils/classproperty.py` & `mafic-2.1.0/mafic/utils/classproperty.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,41 @@
+"""Contains a decorator to merge properties and classmethods."""
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
-from typing import Callable, Generic, TypeVar
+from typing import TYPE_CHECKING, Generic, TypeVar
+
+if TYPE_CHECKING:
+    from collections.abc import Callable
 
 T = TypeVar("T")
 
 __all__ = ("classproperty",)
 
 
 class _ClassPropertyDescriptor(Generic[T]):
     """A descriptor that mimics the behavior of a property, but for classmethods."""
 
-    def __init__(self, fget: classmethod[T] | staticmethod[T], fset: None = None):
+    def __init__(self, fget: classmethod[T] | staticmethod[T]) -> None:
         self.fget = fget
 
     def __get__(self, instance: object, owner: type | None = None) -> T:
         if owner is None:
             owner = type(instance)
         return self.fget.__get__(instance, owner)()
 
 
 def classproperty(
     func: Callable[..., T] | classmethod[T] | staticmethod[T]
 ) -> _ClassPropertyDescriptor[T]:
-    """A decorator that mimics the behavior of a property, but for classmethods.
+    """Contains a decorator to mimic the behavior of a property, but for classmethods.
 
     Parameters
     ----------
     func:
         The function to decorate.
     """
-
     if not isinstance(func, (classmethod, staticmethod)):
         func = classmethod(func)
 
     return _ClassPropertyDescriptor(func)
```

### Comparing `mafic-2.0.1/mafic/utils/decode.py` & `mafic-2.1.0/mafic/utils/decode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+"""A module to decode a track id into a Track object."""
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 from base64 import b64decode
-from typing import Iterator
+from collections.abc import Iterator
 
 from ..track import Track
 
 __all__ = ("decode_track",)
 
 
 def _bytes_to_int(bytes: list[int]) -> int:
@@ -20,15 +21,15 @@
 
 class _TrackDataIterator(Iterator[int]):
     __slots__ = ("__previous_null", "flags", "__iterable", "size", "version")
 
     _TRACK_INFO_VERSIONED = 1
     _FLAG_MASK = 0xC0000000
 
-    def __init__(self, data: bytes):
+    def __init__(self, data: bytes) -> None:
         self.__iterable = iter(data)
 
         # https://github.com/sedmelluq/lavaplayer/blob/97a8efecfe3cb79da4d7d0422de0179e18c30947/main/src/main/java/com/sedmelluq/discord/lavaplayer/tools/io/MessageInput.java#L37
         value = self.read_int(bit_length=4)
         self.flags = (value & self._FLAG_MASK) >> 30
         self.size = value & 0x3FFFFFFF
         self.version = (
@@ -84,18 +85,19 @@
         # URLs seem to be prefixed with `+`
         exists = self.read_bool()
 
         if not exists:
             return None
 
         if (byte := next(self)) != 0:
-            raise ValueError(
+            msg = (
                 "Attempted to traverse a track id "
                 f"and came across an unexpected character: {byte}."
             )
+            raise ValueError(msg)
 
         return self.read_str()
 
 
 def decode_track(track_id: str) -> Track:
     """Decode a track id into a Track object.
 
@@ -111,17 +113,16 @@
         The track id to decode.
 
     Returns
     -------
     Track:
         The decoded track.
     """
-
     raw = b64decode(track_id)
-    print(raw)
+    # print(raw)
     iterator = _TrackDataIterator(raw)
 
     # https://github.com/sedmelluq/lavaplayer/blob/97a8efecfe3cb79da4d7d0422de0179e18c30947/main/src/main/java/com/sedmelluq/discord/lavaplayer/player/DefaultAudioPlayerManager.java#L268
     title = iterator.read_str()
     author = iterator.read_str()
     length = iterator.read_int()
     identifier = iterator.read_str()
```

### Comparing `mafic-2.0.1/mafic/warnings.py` & `mafic-2.1.0/mafic/warnings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Contains the warnings shown from Mafic."""
 # SPDX-License-Identifier: MIT
 
 
 __all__ = ("UnsupportedVersionWarning", "UnknownVersionWarning")
 
 
 class UnsupportedVersionWarning(UserWarning):
```

### Comparing `mafic-2.0.1/PKG-INFO` & `mafic-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mafic
-Version: 2.0.1
+Version: 2.1.0
 Summary: A properly typehinted lavalink client for discord.py, nextcord, disnake and py-cord.
 Home-page: https://github.com/ooliver1/mafic
 License: MIT
 Keywords: nextcord,disnake,discord,disnake.py,lavalink,lavalink.py,pycord,py-cord
 Author: ooliver1
 Author-email: oliverwilkes2006@icloud.com
 Requires-Python: >=3.8,<4.0
```


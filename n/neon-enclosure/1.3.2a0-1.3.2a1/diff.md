# Comparing `tmp/neon_enclosure-1.3.2a0-py3-none-any.whl.zip` & `tmp/neon_enclosure-1.3.2a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 11930 bytes, number of entries: 12
--rw-r--r--  2.0 unx     1831 b- defN 23-Apr-12 02:36 neon_enclosure/__init__.py
--rw-r--r--  2.0 unx     2586 b- defN 23-Apr-12 02:36 neon_enclosure/__main__.py
--rw-r--r--  2.0 unx     3580 b- defN 23-Apr-12 02:36 neon_enclosure/service.py
--rw-r--r--  2.0 unx     1832 b- defN 23-Apr-12 02:36 neon_enclosure/admin/__init__.py
--rw-r--r--  2.0 unx     2535 b- defN 23-Apr-12 02:36 neon_enclosure/admin/__main__.py
--rw-r--r--  2.0 unx     2326 b- defN 23-Apr-12 02:36 neon_enclosure/admin/service.py
--rw-r--r--  2.0 unx     1634 b- defN 23-Apr-12 02:36 neon_enclosure-1.3.2a0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2681 b- defN 23-Apr-12 02:36 neon_enclosure-1.3.2a0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 02:36 neon_enclosure-1.3.2a0.dist-info/WHEEL
--rw-r--r--  2.0 unx       71 b- defN 23-Apr-12 02:36 neon_enclosure-1.3.2a0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       15 b- defN 23-Apr-12 02:36 neon_enclosure-1.3.2a0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1052 b- defN 23-Apr-12 02:36 neon_enclosure-1.3.2a0.dist-info/RECORD
-12 files, 20235 bytes uncompressed, 10140 bytes compressed:  49.9%
+Zip file size: 12016 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     1831 b- defN 23-Apr-19 20:39 neon_enclosure/__init__.py
+-rw-r--r--  2.0 unx     2616 b- defN 23-Apr-19 20:39 neon_enclosure/__main__.py
+-rw-r--r--  2.0 unx     3660 b- defN 23-Apr-19 20:39 neon_enclosure/service.py
+-rw-r--r--  2.0 unx     1832 b- defN 23-Apr-19 20:39 neon_enclosure/admin/__init__.py
+-rw-r--r--  2.0 unx     2564 b- defN 23-Apr-19 20:39 neon_enclosure/admin/__main__.py
+-rw-r--r--  2.0 unx     2406 b- defN 23-Apr-19 20:39 neon_enclosure/admin/service.py
+-rw-r--r--  2.0 unx     1634 b- defN 23-Apr-19 20:39 neon_enclosure-1.3.2a1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2713 b- defN 23-Apr-19 20:39 neon_enclosure-1.3.2a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 20:39 neon_enclosure-1.3.2a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       71 b- defN 23-Apr-19 20:39 neon_enclosure-1.3.2a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       15 b- defN 23-Apr-19 20:39 neon_enclosure-1.3.2a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1052 b- defN 23-Apr-19 20:39 neon_enclosure-1.3.2a1.dist-info/RECORD
+12 files, 20486 bytes uncompressed, 10226 bytes compressed:  50.1%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: neon_enclosure/admin/__main__.py
 Comment: 
 
 Filename: neon_enclosure/admin/service.py
 Comment: 
 
-Filename: neon_enclosure-1.3.2a0.dist-info/LICENSE.md
+Filename: neon_enclosure-1.3.2a1.dist-info/LICENSE.md
 Comment: 
 
-Filename: neon_enclosure-1.3.2a0.dist-info/METADATA
+Filename: neon_enclosure-1.3.2a1.dist-info/METADATA
 Comment: 
 
-Filename: neon_enclosure-1.3.2a0.dist-info/WHEEL
+Filename: neon_enclosure-1.3.2a1.dist-info/WHEEL
 Comment: 
 
-Filename: neon_enclosure-1.3.2a0.dist-info/entry_points.txt
+Filename: neon_enclosure-1.3.2a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: neon_enclosure-1.3.2a0.dist-info/top_level.txt
+Filename: neon_enclosure-1.3.2a1.dist-info/top_level.txt
 Comment: 
 
-Filename: neon_enclosure-1.3.2a0.dist-info/RECORD
+Filename: neon_enclosure-1.3.2a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## neon_enclosure/__main__.py

```diff
@@ -25,28 +25,29 @@
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from neon_utils.configuration_utils import init_config_dir
 from neon_utils.log_utils import init_log
 from ovos_utils.messagebus import get_mycroft_bus
+from ovos_utils.process_utils import reset_sigint_handler
+from ovos_utils import wait_for_exit_signal
 
 
 def main(*args, **kwargs):
     init_config_dir()
     init_log(log_name="enclosure")
     bus = get_mycroft_bus()
     kwargs["bus"] = bus
     from neon_utils.signal_utils import init_signal_bus, \
         init_signal_handlers
     init_signal_bus(bus)
     init_signal_handlers()
 
     from .service import NeonHardwareAbstractionLayer
-    from mycroft.util import reset_sigint_handler, wait_for_exit_signal
 
     reset_sigint_handler()
     service = NeonHardwareAbstractionLayer(*args, **kwargs)
     service.start()
     wait_for_exit_signal()
     service.shutdown()
```

## neon_enclosure/service.py

```diff
@@ -36,14 +36,15 @@
 
 class NeonHardwareAbstractionLayer(PHAL):
     def __init__(self, *args, **kwargs):
         LOG.info(f"Initializing PHAL")
         super().__init__(*args, **kwargs)
         self.status.set_alive()
         self.started = Event()
+        self.config = self.config or dict()  # TODO: Fixed in ovos_PHAL 0.0.5a1
 
     def start(self):
         LOG.info("Starting PHAL")
         if self.config.get('wait_for_gui'):
             LOG.info("Waiting for GUI Service to start")
             timeout = time() + 30
             while time() < timeout:
```

## neon_enclosure/admin/__main__.py

```diff
@@ -24,28 +24,28 @@
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from neon_utils.log_utils import init_log
 from ovos_utils.messagebus import get_mycroft_bus
-
+from ovos_utils.process_utils import reset_sigint_handler
+from ovos_utils import wait_for_exit_signal
 
 def main(*args, **kwargs):
     # init_config_dir()
     init_log(log_name="admin")
     bus = get_mycroft_bus()
     kwargs["bus"] = bus
     from neon_utils.signal_utils import init_signal_bus, \
         init_signal_handlers
     init_signal_bus(bus)
     init_signal_handlers()
 
     from .service import NeonAdminHardwareAbstractionLayer
-    from mycroft.util import reset_sigint_handler, wait_for_exit_signal
 
     reset_sigint_handler()
     service = NeonAdminHardwareAbstractionLayer(*args, **kwargs)
     service.start()
     wait_for_exit_signal()
     service.shutdown()
```

## neon_enclosure/admin/service.py

```diff
@@ -33,13 +33,14 @@
 
 class NeonAdminHardwareAbstractionLayer(AdminPHAL):
     def __init__(self, *args, **kwargs):
         LOG.info(f"Initializing Admin PHAL")
         super().__init__(*args, **kwargs)
         self.status.set_alive()
         self.started = Event()
+        self.config = self.config or dict()  # TODO: Fixed in ovos_PHAL 0.0.5a1
 
     def start(self):
         LOG.info("Starting Admin PHAL")
         AdminPHAL.start(self)
         LOG.info("Started Admin PHAL")
         self.started.set()
```

## Comparing `neon_enclosure-1.3.2a0.dist-info/LICENSE.md` & `neon_enclosure-1.3.2a1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `neon_enclosure-1.3.2a0.dist-info/METADATA` & `neon_enclosure-1.3.2a1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: neon-enclosure
-Version: 1.3.2a0
+Version: 1.3.2a1
 Summary: Neon Enclosure Module
 Home-page: https://github.com/NeonGeckoCom/neon-enclosure
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: ovos-PHAL (>=0.0.5a4,~=0.0.4)
-Requires-Dist: neon-utils[network] (>=1.2.4,~=1.2)
-Requires-Dist: ovos-utils[extras] (>=0.0.31a11,~=0.0.30)
-Requires-Dist: ovos-core (~=0.0.5)
+Requires-Dist: ovos-PHAL (~=0.0.4)
+Requires-Dist: neon-utils[network] (~=1.3)
+Requires-Dist: ovos-utils[extras] (~=0.0.32)
+Requires-Dist: ovos-bus-client (>=0.0.3a22,~=0.0.2)
+Requires-Dist: ovos-backend-client (~=0.0.6)
 Provides-Extra: docker
 Requires-Dist: ovos-phal-plugin-homeassistant (~=0.0.1) ; extra == 'docker'
 Requires-Dist: ovos-phal-plugin-notification-widgets (~=1.0.0) ; extra == 'docker'
 Requires-Dist: ovos-phal-plugin-color-scheme-manager (~=1.0.0) ; extra == 'docker'
 Requires-Dist: ovos-phal-plugin-configuration-provider (~=1.0.0) ; extra == 'docker'
 Requires-Dist: ovos-phal-plugin-dashboard (~=0.0.1) ; extra == 'docker'
 Requires-Dist: ovos-phal-plugin-connectivity-events (~=0.0.2) ; extra == 'docker'
```

## Comparing `neon_enclosure-1.3.2a0.dist-info/RECORD` & `neon_enclosure-1.3.2a1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 neon_enclosure/__init__.py,sha256=UDwbScPcnqA05m_zQmXnY6YeoL5j6NS_TaLj0mQdU_8,1831
-neon_enclosure/__main__.py,sha256=utweyoTXU5MUVrdQHnVUWLU1kEobUp_lug8uqoRjnh0,2586
-neon_enclosure/service.py,sha256=vhCkiAEfodte8ks1Jn-Otik-jLzLOD2ko-FioBy6FiE,3580
+neon_enclosure/__main__.py,sha256=pX8kUAiDtx8qCdNKSKT1LkA61R8qiu_nNC3_Qf1WWOI,2616
+neon_enclosure/service.py,sha256=ntd4ky4nfdtDEkWEKn8wRJkrqQFX1_N9l0HDXQwDcfI,3660
 neon_enclosure/admin/__init__.py,sha256=FCW9FTGwZxZm9BbxptD2ri02MXw5mq0YtuIfJ0Rm0SA,1832
-neon_enclosure/admin/__main__.py,sha256=23trrM05ZNp0RaWPP55SoHX9zLAbT-xaZgsj9aMj1m0,2535
-neon_enclosure/admin/service.py,sha256=p2y_n5TYBJwYpsiavH476yZB2kDksKHFH2_CO2FlBtQ,2326
-neon_enclosure-1.3.2a0.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
-neon_enclosure-1.3.2a0.dist-info/METADATA,sha256=qhqwK2SoSj4BN3steyvAYLI0t-foMAQzGks49KMZQGs,2681
-neon_enclosure-1.3.2a0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-neon_enclosure-1.3.2a0.dist-info/entry_points.txt,sha256=B38ve9l9IDVVfjPQFWLh0CYSoOJ454sgGWq3dfu6EPU,71
-neon_enclosure-1.3.2a0.dist-info/top_level.txt,sha256=JyzbDWcL_LA7RBt9baW_93Ep9FDpe-ukXCsowuQm2Ug,15
-neon_enclosure-1.3.2a0.dist-info/RECORD,,
+neon_enclosure/admin/__main__.py,sha256=iBkWDpV1GCLCclglNExFJguzd_Qz_C-mWLnEp1nMePE,2564
+neon_enclosure/admin/service.py,sha256=UrD0RLVFi-27A0wnFFfQjVlmo-GHWxEyma1Q0W8TLqE,2406
+neon_enclosure-1.3.2a1.dist-info/LICENSE.md,sha256=gxKa3HnxC7fSIlGFpLAiSAhQS22pIyVEyXmPQR2KlXM,1634
+neon_enclosure-1.3.2a1.dist-info/METADATA,sha256=YucwlXTOWygWd-rx2Wtemwo0ihkz2hKr3fTQyMUa9T0,2713
+neon_enclosure-1.3.2a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+neon_enclosure-1.3.2a1.dist-info/entry_points.txt,sha256=B38ve9l9IDVVfjPQFWLh0CYSoOJ454sgGWq3dfu6EPU,71
+neon_enclosure-1.3.2a1.dist-info/top_level.txt,sha256=JyzbDWcL_LA7RBt9baW_93Ep9FDpe-ukXCsowuQm2Ug,15
+neon_enclosure-1.3.2a1.dist-info/RECORD,,
```


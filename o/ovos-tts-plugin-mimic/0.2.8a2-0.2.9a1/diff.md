# Comparing `tmp/ovos_tts_plugin_mimic-0.2.8a2-py3-none-any.whl.zip` & `tmp/ovos_tts_plugin_mimic-0.2.9a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8783 bytes, number of entries: 9
--rw-r--r--  2.0 unx     6408 b- defN 23-Apr-24 08:28 ovos_tts_plugin_mimic/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-Apr-24 08:28 ovos_tts_plugin_mimic/version.py
--rw-r--r--  2.0 unx    11349 b- defN 23-Apr-24 08:29 ovos_tts_plugin_mimic-0.2.8a2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1065 b- defN 23-Apr-24 08:29 ovos_tts_plugin_mimic-0.2.8a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-24 08:29 ovos_tts_plugin_mimic-0.2.8a2.dist-info/WHEEL
--rw-r--r--  2.0 unx      186 b- defN 23-Apr-24 08:29 ovos_tts_plugin_mimic-0.2.8a2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       22 b- defN 23-Apr-24 08:29 ovos_tts_plugin_mimic-0.2.8a2.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-24 08:29 ovos_tts_plugin_mimic-0.2.8a2.dist-info/zip-safe
--rw-rw-r--  2.0 unx      859 b- defN 23-Apr-24 08:29 ovos_tts_plugin_mimic-0.2.8a2.dist-info/RECORD
-9 files, 20159 bytes uncompressed, 7261 bytes compressed:  64.0%
+Zip file size: 9263 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     8724 b- defN 23-Jul-04 11:12 ovos_tts_plugin_mimic/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Jul-04 11:12 ovos_tts_plugin_mimic/version.py
+-rw-r--r--  2.0 unx    11349 b- defN 23-Jul-04 11:12 ovos_tts_plugin_mimic-0.2.9a1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1065 b- defN 23-Jul-04 11:12 ovos_tts_plugin_mimic-0.2.9a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-04 11:12 ovos_tts_plugin_mimic-0.2.9a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      271 b- defN 23-Jul-04 11:12 ovos_tts_plugin_mimic-0.2.9a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       22 b- defN 23-Jul-04 11:12 ovos_tts_plugin_mimic-0.2.9a1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-04 11:12 ovos_tts_plugin_mimic-0.2.9a1.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      859 b- defN 23-Jul-04 11:12 ovos_tts_plugin_mimic-0.2.9a1.dist-info/RECORD
+9 files, 22560 bytes uncompressed, 7741 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: ovos_tts_plugin_mimic/__init__.py
 Comment: 
 
 Filename: ovos_tts_plugin_mimic/version.py
 Comment: 
 
-Filename: ovos_tts_plugin_mimic-0.2.8a2.dist-info/LICENSE
+Filename: ovos_tts_plugin_mimic-0.2.9a1.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_tts_plugin_mimic-0.2.8a2.dist-info/METADATA
+Filename: ovos_tts_plugin_mimic-0.2.9a1.dist-info/METADATA
 Comment: 
 
-Filename: ovos_tts_plugin_mimic-0.2.8a2.dist-info/WHEEL
+Filename: ovos_tts_plugin_mimic-0.2.9a1.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_tts_plugin_mimic-0.2.8a2.dist-info/entry_points.txt
+Filename: ovos_tts_plugin_mimic-0.2.9a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_tts_plugin_mimic-0.2.8a2.dist-info/top_level.txt
+Filename: ovos_tts_plugin_mimic-0.2.9a1.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_tts_plugin_mimic-0.2.8a2.dist-info/zip-safe
+Filename: ovos_tts_plugin_mimic-0.2.9a1.dist-info/zip-safe
 Comment: 
 
-Filename: ovos_tts_plugin_mimic-0.2.8a2.dist-info/RECORD
+Filename: ovos_tts_plugin_mimic-0.2.9a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_tts_plugin_mimic/__init__.py

```diff
@@ -9,22 +9,77 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import subprocess
 from distutils.spawn import find_executable
 from os.path import join, isfile, expanduser
-
+from ovos_plugin_manager.templates.g2p import Grapheme2PhonemePlugin, OutOfVocabulary
 from ovos_plugin_manager.templates.tts import TTS, TTSValidator
 from ovos_utils.configuration import get_xdg_base
 from ovos_utils.configuration import read_mycroft_config
 from ovos_utils.lang.visimes import VISIMES
 from ovos_utils.xdg_utils import xdg_config_home
 
 
+class MimicPhonemesPlugin(Grapheme2PhonemePlugin):
+
+    def __init__(self, config=None):
+        super().__init__(config)
+        self.mimic_bin = expanduser(self.config.get("binary") or
+                                    find_executable("mimic") or
+                                    "mimic")
+
+    @staticmethod
+    def parse_phonemes(phonemes, normalize=False):
+        """Parse mimic phoneme string into a list of phone, duration pairs.
+        Arguments
+            phonemes (bytes): phoneme output from mimic
+        Returns:
+            (list) list of phoneme duration pairs
+        """
+        phon_str = phonemes.decode()
+        pairs = phon_str.replace("pau", ".").split(' ')
+        phones = [pair.split(':') for pair in pairs if ':' in pair]
+        # remove silence at start/end/repeated
+        if normalize:
+            for idx, (pho, dur) in enumerate(phones):
+                next_pho = phones[idx + 1][0] if idx + 1 < len(phones) else None
+                if pho == ".":
+                    if idx == 0 or idx == len(phones) - 1 or next_pho == ".":
+                        phones[idx] = None
+        return [p for p in phones if p is not None]
+
+    def get_mimic_phonemes(self, sentence, normalize=True):
+        args = [self.mimic_bin, '-psdur', '-ssml', '-t', sentence, '-o', '/tmp/mimic.pho']
+        phonemes = subprocess.check_output(args)
+        return self.parse_phonemes(phonemes, normalize)
+
+    def get_arpa(self, word, lang, ignore_oov=True):
+        if lang.lower().startswith("en"):
+            return [p[0].upper() for p in self.get_mimic_phonemes(word)]
+        if ignore_oov:
+            return None
+        raise OutOfVocabulary
+
+    def utterance2visemes(self, utterance, lang="en", default_dur=0.4):
+        phonemes = self.get_mimic_phonemes(utterance, normalize=False)
+        return [(VISIMES.get(pho[0], '4'), float(pho[1])) for pho in phonemes]
+
+    @property
+    def available_languages(self):
+        """Return languages supported by this G2P implementation in this state
+        This property should be overridden by the derived class to advertise
+        what languages that engine supports.
+        Returns:
+            set: supported languages
+        """
+        return {"en"}
+
+
 class MimicTTSPlugin(TTS):
     """Interface to Mimic TTS."""
 
     def __init__(self, lang="en-us", config=None):
         super(MimicTTSPlugin, self).__init__(lang, config,
                                              MimicTTSValidator(self), 'wav')
         self.mimic_bin = self.config.get("binary") or \
```

## ovos_tts_plugin_mimic/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 2
-VERSION_BUILD = 8
-VERSION_ALPHA = 2
+VERSION_BUILD = 9
+VERSION_ALPHA = 1
 # END_VERSION_BLOCK
```

## Comparing `ovos_tts_plugin_mimic-0.2.8a2.dist-info/LICENSE` & `ovos_tts_plugin_mimic-0.2.9a1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_tts_plugin_mimic-0.2.8a2.dist-info/METADATA` & `ovos_tts_plugin_mimic-0.2.9a1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-tts-plugin-mimic
-Version: 0.2.8a2
+Version: 0.2.9a1
 Summary: mimic tts plugin for OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/ovos-tts-plugin-mimic
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: mycroft plugin tts OVOS OpenVoiceOS
 Platform: UNKNOWN
```

## Comparing `ovos_tts_plugin_mimic-0.2.8a2.dist-info/RECORD` & `ovos_tts_plugin_mimic-0.2.9a1.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-ovos_tts_plugin_mimic/__init__.py,sha256=oIott377j6-Ys3IKZLQs2Z0TxqBNQ-yr_AhLRG2FasM,6408
-ovos_tts_plugin_mimic/version.py,sha256=NN7KkFKdBuVhWyCXuDk9kKMoX5nHT9llvz6PzpcScac,177
-ovos_tts_plugin_mimic-0.2.8a2.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
-ovos_tts_plugin_mimic-0.2.8a2.dist-info/METADATA,sha256=8Dk84w2m1MKIlIQHV1zMlzi0QEeprKvFGMQZW0P-7Hc,1065
-ovos_tts_plugin_mimic-0.2.8a2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ovos_tts_plugin_mimic-0.2.8a2.dist-info/entry_points.txt,sha256=cpMDp3sVYWI7-Zrn2LaccI0BClDVNaxg_DqLzJ9herw,186
-ovos_tts_plugin_mimic-0.2.8a2.dist-info/top_level.txt,sha256=wHdv3nP76RPxU4Mrw1HE2P3kTZOz6X4iJ_AQB4_fGtc,22
-ovos_tts_plugin_mimic-0.2.8a2.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-ovos_tts_plugin_mimic-0.2.8a2.dist-info/RECORD,,
+ovos_tts_plugin_mimic/__init__.py,sha256=e4-8EqlCugz5L7IvfEWrUgSzaUv7QW0wEiPS-f53FPI,8724
+ovos_tts_plugin_mimic/version.py,sha256=b9HKmjXKSGfqohMCSS7K82Hm30gpNO5sJd5xhsWKZBI,177
+ovos_tts_plugin_mimic-0.2.9a1.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
+ovos_tts_plugin_mimic-0.2.9a1.dist-info/METADATA,sha256=itdEHzb73Q4F61eNX7T8Xozc8V2Fy1ZUP3UhaiMAT0w,1065
+ovos_tts_plugin_mimic-0.2.9a1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ovos_tts_plugin_mimic-0.2.9a1.dist-info/entry_points.txt,sha256=XWMQOHim03OJkxfyQNnpN01CC6WGPRHQSh-rqAWryZM,271
+ovos_tts_plugin_mimic-0.2.9a1.dist-info/top_level.txt,sha256=wHdv3nP76RPxU4Mrw1HE2P3kTZOz6X4iJ_AQB4_fGtc,22
+ovos_tts_plugin_mimic-0.2.9a1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+ovos_tts_plugin_mimic-0.2.9a1.dist-info/RECORD,,
```


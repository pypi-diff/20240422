# Comparing `tmp/ovos_ww_plugin_openwakeword-0.4.0-py3-none-any.whl.zip` & `tmp/ovos_ww_plugin_openwakeword-0.4.1a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7888 bytes, number of entries: 8
--rw-r--r--  2.0 unx     3782 b- defN 23-Dec-23 15:23 ovos_ww_plugin_openwakeword/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-Dec-23 15:23 ovos_ww_plugin_openwakeword/version.py
--rw-r--r--  2.0 unx    11349 b- defN 23-Dec-23 15:23 ovos_ww_plugin_openwakeword-0.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      386 b- defN 23-Dec-23 15:23 ovos_ww_plugin_openwakeword-0.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Dec-23 15:23 ovos_ww_plugin_openwakeword-0.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      101 b- defN 23-Dec-23 15:23 ovos_ww_plugin_openwakeword-0.4.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       28 b- defN 23-Dec-23 15:23 ovos_ww_plugin_openwakeword-0.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      792 b- defN 23-Dec-23 15:23 ovos_ww_plugin_openwakeword-0.4.0.dist-info/RECORD
-8 files, 16707 bytes uncompressed, 6466 bytes compressed:  61.3%
+Zip file size: 7973 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     3880 b- defN 24-Apr-22 00:57 ovos_ww_plugin_openwakeword/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 24-Apr-22 00:57 ovos_ww_plugin_openwakeword/version.py
+-rw-r--r--  2.0 unx    11349 b- defN 24-Apr-22 00:57 ovos_ww_plugin_openwakeword-0.4.1a1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      388 b- defN 24-Apr-22 00:57 ovos_ww_plugin_openwakeword-0.4.1a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 00:57 ovos_ww_plugin_openwakeword-0.4.1a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      101 b- defN 24-Apr-22 00:57 ovos_ww_plugin_openwakeword-0.4.1a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-22 00:57 ovos_ww_plugin_openwakeword-0.4.1a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      804 b- defN 24-Apr-22 00:57 ovos_ww_plugin_openwakeword-0.4.1a1.dist-info/RECORD
+8 files, 16819 bytes uncompressed, 6527 bytes compressed:  61.2%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: ovos_ww_plugin_openwakeword/__init__.py
 Comment: 
 
 Filename: ovos_ww_plugin_openwakeword/version.py
 Comment: 
 
-Filename: ovos_ww_plugin_openwakeword-0.4.0.dist-info/LICENSE
+Filename: ovos_ww_plugin_openwakeword-0.4.1a1.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_ww_plugin_openwakeword-0.4.0.dist-info/METADATA
+Filename: ovos_ww_plugin_openwakeword-0.4.1a1.dist-info/METADATA
 Comment: 
 
-Filename: ovos_ww_plugin_openwakeword-0.4.0.dist-info/WHEEL
+Filename: ovos_ww_plugin_openwakeword-0.4.1a1.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_ww_plugin_openwakeword-0.4.0.dist-info/entry_points.txt
+Filename: ovos_ww_plugin_openwakeword-0.4.1a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_ww_plugin_openwakeword-0.4.0.dist-info/top_level.txt
+Filename: ovos_ww_plugin_openwakeword-0.4.1a1.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_ww_plugin_openwakeword-0.4.0.dist-info/RECORD
+Filename: ovos_ww_plugin_openwakeword-0.4.1a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_ww_plugin_openwakeword/__init__.py

```diff
@@ -12,28 +12,31 @@
 #
 
 # Imports
 from ovos_plugin_manager.templates.hotwords import HotWordEngine
 from ovos_utils.log import LOG
 import openwakeword
 import numpy as np
+from openwakeword.utils import download_models
 
 class OwwHotwordPlugin(HotWordEngine):
     """OpenWakeWord is an open-source wakeword or phrase engine that can be trained on 100% synthetic data.
     It can produce high-quality models for arbitrary words and phrases that perform well across
     a wide range of voices and acoustic environments.
     """
 
     def __init__(self, key_phrase="hey jarvis", config=None, lang="en-us"):
         super().__init__(key_phrase, config, lang)
+        # Support for 0.6.0, which removes packaged defaults
+        download_models()
 
         # Load openWakeWord model
-        pretrained_models = openwakeword.get_pretrained_model_paths()
+        pretrained_models = openwakeword.get_pretrained_model_paths() or []
         self.model = openwakeword.Model(
-            wakeword_model_paths=self.config.get('models', [i for i in pretrained_models if key_phrase in i]),
+            wakeword_models=self.config.get('models', [i for i in pretrained_models if key_phrase in i]),
             custom_verifier_models=self.config.get('custom_verifier_models', {}),
             custom_verifier_threshold=self.config.get('custom_verifier_threshold', 0.1),
             inference_framework=self.config.get('inference_framework', 'tflite')
         )
         self.model_names = list(self.model.models.keys())
 
         # Define short buffer for audio to ensure correct chunk sizes
@@ -66,16 +69,16 @@
                     self.has_found = True
 
                     # Flush recent history of openWakeWord internal audio buffer to avoid re-activations
                     n_frames = self.model.model_inputs[mdl_name]
                     self.model.preprocessor.raw_data_buffer.extend([0.0]*n_frames*1280)
                     self.model.preprocessor.feature_buffer[-n_frames:, :] = np.zeros((n_frames, 96)).astype(np.float32)
                     self.model.preprocessor.melspectrogram_buffer[-250:, :] = np.zeros((250, 32)).astype(np.float32)
-                    
+
                     break
-                    
+
 
     def found_wake_word(self, frame_data):
         if self.has_found:
             self.has_found = False
             return True
         return False
```

## ovos_ww_plugin_openwakeword/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 4
-VERSION_BUILD = 0
-VERSION_ALPHA = 0
+VERSION_BUILD = 1
+VERSION_ALPHA = 1
 # END_VERSION_BLOCK
```

## Comparing `ovos_ww_plugin_openwakeword-0.4.0.dist-info/LICENSE` & `ovos_ww_plugin_openwakeword-0.4.1a1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ovos_ww_plugin_openwakeword-0.4.0.dist-info/RECORD` & `ovos_ww_plugin_openwakeword-0.4.1a1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-ovos_ww_plugin_openwakeword/__init__.py,sha256=wjelYqn1CZ2-VTmeSuQju2ctuQUbFZgpZIQDkaleQLs,3782
-ovos_ww_plugin_openwakeword/version.py,sha256=aH7_xL5ISG_aX2ms5n3HeNDhQaAiYpSf0HCWl026D7k,177
-ovos_ww_plugin_openwakeword-0.4.0.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
-ovos_ww_plugin_openwakeword-0.4.0.dist-info/METADATA,sha256=yUwxKHPXjlrOCiHemiJerI4uSyFXHFRBOoA3suqjSAc,386
-ovos_ww_plugin_openwakeword-0.4.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-ovos_ww_plugin_openwakeword-0.4.0.dist-info/entry_points.txt,sha256=SYCbpP3QESdyhmtKvgf-HwLH47vh0SMxoZa9zgAy9Do,101
-ovos_ww_plugin_openwakeword-0.4.0.dist-info/top_level.txt,sha256=lK7TUGVCPjHNf7cenysfPz0SV6ykkL_fQW4syOCYWsM,28
-ovos_ww_plugin_openwakeword-0.4.0.dist-info/RECORD,,
+ovos_ww_plugin_openwakeword/__init__.py,sha256=sdoEjDgOKwidma8hPQ270_zSIONYXvM0QJzeF1tYxqI,3880
+ovos_ww_plugin_openwakeword/version.py,sha256=YHzOY5iulVS6nY6xXP4nTzvQihrTw-15vpa-jmGTTBc,177
+ovos_ww_plugin_openwakeword-0.4.1a1.dist-info/LICENSE,sha256=fYHkowW9JcaEcqCPTXYBayNJ9J1lGdYVb7Mf9oy6oEY,11349
+ovos_ww_plugin_openwakeword-0.4.1a1.dist-info/METADATA,sha256=PYYuKhd3vhhB0RLcxSnQDQCpcUwvhma3zn1AkEXbZQM,388
+ovos_ww_plugin_openwakeword-0.4.1a1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ovos_ww_plugin_openwakeword-0.4.1a1.dist-info/entry_points.txt,sha256=SYCbpP3QESdyhmtKvgf-HwLH47vh0SMxoZa9zgAy9Do,101
+ovos_ww_plugin_openwakeword-0.4.1a1.dist-info/top_level.txt,sha256=lK7TUGVCPjHNf7cenysfPz0SV6ykkL_fQW4syOCYWsM,28
+ovos_ww_plugin_openwakeword-0.4.1a1.dist-info/RECORD,,
```


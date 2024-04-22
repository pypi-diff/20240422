# Comparing `tmp/strauss-0.1.1.tar.gz` & `tmp/strauss-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strauss-0.1.1.tar", last modified: Tue Apr 16 10:18:48 2024, max compression
+gzip compressed data, was "strauss-0.1.2.tar", last modified: Mon Apr 22 08:48:06 2024, max compression
```

## Comparing `strauss-0.1.1.tar` & `strauss-0.1.2.tar`

### file list

```diff
@@ -1,41 +1,46 @@
-drwxrwxr-x   0 youless   (1002) youless   (1002)        0 2024-04-16 10:18:48.345445 strauss-0.1.1/
--rw-rw-r--   0 youless   (1002) youless   (1002)    11358 2023-08-30 13:06:36.000000 strauss-0.1.1/LICENSE
--rw-rw-r--   0 youless   (1002) youless   (1002)       73 2023-08-30 13:06:36.000000 strauss-0.1.1/MANIFEST.in
--rw-r--r--   0 youless   (1002) youless   (1002)     2998 2024-04-16 10:18:48.345445 strauss-0.1.1/PKG-INFO
--rw-rw-r--   0 youless   (1002) youless   (1002)     2190 2024-04-16 10:15:35.000000 strauss-0.1.1/README.md
--rw-rw-r--   0 youless   (1002) youless   (1002)      223 2023-08-30 13:06:36.000000 strauss-0.1.1/pyproject.toml
--rw-rw-r--   0 youless   (1002) youless   (1002)      782 2024-04-16 10:18:48.345445 strauss-0.1.1/setup.cfg
--rw-rw-r--   0 youless   (1002) youless   (1002)       37 2023-08-30 13:06:36.000000 strauss-0.1.1/setup.py
-drwxrwxr-x   0 youless   (1002) youless   (1002)        0 2024-04-16 10:18:48.333445 strauss-0.1.1/src/
-drwxrwxr-x   0 youless   (1002) youless   (1002)        0 2024-04-16 10:18:48.341445 strauss-0.1.1/src/strauss/
--rw-rw-r--   0 youless   (1002) youless   (1002)      441 2023-08-30 13:06:36.000000 strauss-0.1.1/src/strauss/__init__.py
--rw-rw-r--   0 youless   (1002) youless   (1002)     9831 2024-03-19 11:04:43.000000 strauss-0.1.1/src/strauss/channels.py
--rw-rw-r--   0 youless   (1002) youless   (1002)      340 2023-08-30 13:06:36.000000 strauss-0.1.1/src/strauss/filters.py
--rw-rw-r--   0 youless   (1002) youless   (1002)    31437 2024-03-19 11:04:43.000000 strauss-0.1.1/src/strauss/generator.py
--rw-rw-r--   0 youless   (1002) youless   (1002)     1068 2023-08-30 13:06:36.000000 strauss-0.1.1/src/strauss/notes.py
-drwxrwxr-x   0 youless   (1002) youless   (1002)        0 2024-04-16 10:18:48.341445 strauss-0.1.1/src/strauss/presets/
--rw-rw-r--   0 youless   (1002) youless   (1002)       42 2023-08-30 13:06:36.000000 strauss-0.1.1/src/strauss/presets/__init__.py
-drwxrwxr-x   0 youless   (1002) youless   (1002)        0 2024-04-16 10:18:48.341445 strauss-0.1.1/src/strauss/presets/sampler/
--rw-rw-r--   0 youless   (1002) youless   (1002)      946 2023-08-30 13:06:36.000000 strauss-0.1.1/src/strauss/presets/sampler/__init__.py
--rw-rw-r--   0 youless   (1002) youless   (1002)     1430 2023-08-30 13:06:36.000000 strauss-0.1.1/src/strauss/presets/sampler/default.yml
-drwxrwxr-x   0 youless   (1002) youless   (1002)        0 2024-04-16 10:18:48.341445 strauss-0.1.1/src/strauss/presets/sampler/ranges/
--rw-rw-r--   0 youless   (1002) youless   (1002)      971 2024-03-19 11:04:43.000000 strauss-0.1.1/src/strauss/presets/sampler/ranges/default.yml
-drwxrwxr-x   0 youless   (1002) youless   (1002)        0 2024-04-16 10:18:48.345445 strauss-0.1.1/src/strauss/presets/synth/
--rw-rw-r--   0 youless   (1002) youless   (1002)      946 2023-08-30 13:06:36.000000 strauss-0.1.1/src/strauss/presets/synth/__init__.py
--rw-rw-r--   0 youless   (1002) youless   (1002)     1884 2024-03-19 11:04:43.000000 strauss-0.1.1/src/strauss/presets/synth/default.yml
--rw-rw-r--   0 youless   (1002) youless   (1002)      487 2023-08-30 13:06:36.000000 strauss-0.1.1/src/strauss/presets/synth/pitch_mapper.yml
-drwxrwxr-x   0 youless   (1002) youless   (1002)        0 2024-04-16 10:18:48.345445 strauss-0.1.1/src/strauss/presets/synth/ranges/
--rw-rw-r--   0 youless   (1002) youless   (1002)      971 2024-03-19 11:04:43.000000 strauss-0.1.1/src/strauss/presets/synth/ranges/default.yml
--rw-rw-r--   0 youless   (1002) youless   (1002)      356 2023-08-30 13:06:36.000000 strauss-0.1.1/src/strauss/presets/synth/spectraliser.yml
--rw-rw-r--   0 youless   (1002) youless   (1002)      320 2023-08-30 13:06:36.000000 strauss-0.1.1/src/strauss/presets/synth/windy.yml
--rw-rw-r--   0 youless   (1002) youless   (1002)     4233 2023-08-30 13:06:36.000000 strauss-0.1.1/src/strauss/score.py
--rw-rw-r--   0 youless   (1002) youless   (1002)    15294 2024-04-16 09:06:44.000000 strauss-0.1.1/src/strauss/sonification.py
--rw-rw-r--   0 youless   (1002) youless   (1002)    12205 2024-03-19 11:04:43.000000 strauss-0.1.1/src/strauss/sources.py
--rw-rw-r--   0 youless   (1002) youless   (1002)     5669 2023-08-30 13:06:36.000000 strauss-0.1.1/src/strauss/stream.py
--rw-rw-r--   0 youless   (1002) youless   (1002)     3024 2023-11-28 11:37:47.000000 strauss-0.1.1/src/strauss/utilities.py
-drwxrwxr-x   0 youless   (1002) youless   (1002)        0 2024-04-16 10:18:48.345445 strauss-0.1.1/src/strauss.egg-info/
--rw-r--r--   0 youless   (1002) youless   (1002)     2998 2024-04-16 10:18:48.000000 strauss-0.1.1/src/strauss.egg-info/PKG-INFO
--rw-rw-r--   0 youless   (1002) youless   (1002)      875 2024-04-16 10:18:48.000000 strauss-0.1.1/src/strauss.egg-info/SOURCES.txt
--rw-rw-r--   0 youless   (1002) youless   (1002)        1 2024-04-16 10:18:48.000000 strauss-0.1.1/src/strauss.egg-info/dependency_links.txt
--rw-rw-r--   0 youless   (1002) youless   (1002)      119 2024-04-16 10:18:48.000000 strauss-0.1.1/src/strauss.egg-info/requires.txt
--rw-rw-r--   0 youless   (1002) youless   (1002)        8 2024-04-16 10:18:48.000000 strauss-0.1.1/src/strauss.egg-info/top_level.txt
+drwxrwxr-x   0 youless   (1002) youless   (1002)        0 2024-04-22 08:48:06.193615 strauss-0.1.2/
+-rw-rw-r--   0 youless   (1002) youless   (1002)    11358 2023-08-30 13:06:36.000000 strauss-0.1.2/LICENSE
+-rw-rw-r--   0 youless   (1002) youless   (1002)       73 2023-08-30 13:06:36.000000 strauss-0.1.2/MANIFEST.in
+-rw-r--r--   0 youless   (1002) youless   (1002)     3026 2024-04-22 08:48:06.193615 strauss-0.1.2/PKG-INFO
+-rw-rw-r--   0 youless   (1002) youless   (1002)     2218 2024-04-22 08:19:55.000000 strauss-0.1.2/README.md
+-rw-rw-r--   0 youless   (1002) youless   (1002)      223 2023-08-30 13:06:36.000000 strauss-0.1.2/pyproject.toml
+-rw-rw-r--   0 youless   (1002) youless   (1002)      782 2024-04-22 08:48:06.193615 strauss-0.1.2/setup.cfg
+-rw-rw-r--   0 youless   (1002) youless   (1002)       37 2023-08-30 13:06:36.000000 strauss-0.1.2/setup.py
+drwxrwxr-x   0 youless   (1002) youless   (1002)        0 2024-04-22 08:48:06.181614 strauss-0.1.2/src/
+drwxrwxr-x   0 youless   (1002) youless   (1002)        0 2024-04-22 08:48:06.189615 strauss-0.1.2/src/strauss/
+-rw-rw-r--   0 youless   (1002) youless   (1002)      441 2023-08-30 13:06:36.000000 strauss-0.1.2/src/strauss/__init__.py
+-rw-rw-r--   0 youless   (1002) youless   (1002)     9831 2024-03-19 11:04:43.000000 strauss-0.1.2/src/strauss/channels.py
+-rw-rw-r--   0 youless   (1002) youless   (1002)      340 2023-08-30 13:06:36.000000 strauss-0.1.2/src/strauss/filters.py
+-rw-rw-r--   0 youless   (1002) youless   (1002)    41413 2024-04-22 08:17:39.000000 strauss-0.1.2/src/strauss/generator.py
+-rw-rw-r--   0 youless   (1002) youless   (1002)     1068 2023-08-30 13:06:36.000000 strauss-0.1.2/src/strauss/notes.py
+drwxrwxr-x   0 youless   (1002) youless   (1002)        0 2024-04-22 08:48:06.189615 strauss-0.1.2/src/strauss/presets/
+-rw-rw-r--   0 youless   (1002) youless   (1002)       61 2024-04-22 08:17:39.000000 strauss-0.1.2/src/strauss/presets/__init__.py
+drwxrwxr-x   0 youless   (1002) youless   (1002)        0 2024-04-22 08:48:06.189615 strauss-0.1.2/src/strauss/presets/sampler/
+-rw-rw-r--   0 youless   (1002) youless   (1002)      946 2023-08-30 13:06:36.000000 strauss-0.1.2/src/strauss/presets/sampler/__init__.py
+-rw-rw-r--   0 youless   (1002) youless   (1002)     1471 2024-04-22 08:17:39.000000 strauss-0.1.2/src/strauss/presets/sampler/default.yml
+drwxrwxr-x   0 youless   (1002) youless   (1002)        0 2024-04-22 08:48:06.189615 strauss-0.1.2/src/strauss/presets/sampler/ranges/
+-rw-rw-r--   0 youless   (1002) youless   (1002)      971 2024-03-19 11:04:43.000000 strauss-0.1.2/src/strauss/presets/sampler/ranges/default.yml
+drwxrwxr-x   0 youless   (1002) youless   (1002)        0 2024-04-22 08:48:06.189615 strauss-0.1.2/src/strauss/presets/spec/
+-rw-rw-r--   0 youless   (1002) youless   (1002)      946 2024-04-22 08:17:39.000000 strauss-0.1.2/src/strauss/presets/spec/__init__.py
+-rw-rw-r--   0 youless   (1002) youless   (1002)     1799 2024-04-22 08:17:39.000000 strauss-0.1.2/src/strauss/presets/spec/default.yml
+drwxrwxr-x   0 youless   (1002) youless   (1002)        0 2024-04-22 08:48:06.189615 strauss-0.1.2/src/strauss/presets/spec/ranges/
+-rw-rw-r--   0 youless   (1002) youless   (1002)     1071 2024-04-22 08:17:39.000000 strauss-0.1.2/src/strauss/presets/spec/ranges/default.yml
+drwxrwxr-x   0 youless   (1002) youless   (1002)        0 2024-04-22 08:48:06.189615 strauss-0.1.2/src/strauss/presets/synth/
+-rw-rw-r--   0 youless   (1002) youless   (1002)      946 2023-08-30 13:06:36.000000 strauss-0.1.2/src/strauss/presets/synth/__init__.py
+-rw-rw-r--   0 youless   (1002) youless   (1002)     1884 2024-03-19 11:04:43.000000 strauss-0.1.2/src/strauss/presets/synth/default.yml
+-rw-rw-r--   0 youless   (1002) youless   (1002)      487 2023-08-30 13:06:36.000000 strauss-0.1.2/src/strauss/presets/synth/pitch_mapper.yml
+drwxrwxr-x   0 youless   (1002) youless   (1002)        0 2024-04-22 08:48:06.189615 strauss-0.1.2/src/strauss/presets/synth/ranges/
+-rw-rw-r--   0 youless   (1002) youless   (1002)      971 2024-03-19 11:04:43.000000 strauss-0.1.2/src/strauss/presets/synth/ranges/default.yml
+-rw-rw-r--   0 youless   (1002) youless   (1002)      356 2023-08-30 13:06:36.000000 strauss-0.1.2/src/strauss/presets/synth/spectraliser.yml
+-rw-rw-r--   0 youless   (1002) youless   (1002)      320 2023-08-30 13:06:36.000000 strauss-0.1.2/src/strauss/presets/synth/windy.yml
+-rw-rw-r--   0 youless   (1002) youless   (1002)     4821 2024-04-22 08:17:39.000000 strauss-0.1.2/src/strauss/score.py
+-rw-rw-r--   0 youless   (1002) youless   (1002)    15680 2024-04-22 08:17:39.000000 strauss-0.1.2/src/strauss/sonification.py
+-rw-rw-r--   0 youless   (1002) youless   (1002)    12462 2024-04-22 08:17:39.000000 strauss-0.1.2/src/strauss/sources.py
+-rw-rw-r--   0 youless   (1002) youless   (1002)     5752 2024-04-22 08:17:39.000000 strauss-0.1.2/src/strauss/stream.py
+-rw-rw-r--   0 youless   (1002) youless   (1002)     3296 2024-04-22 08:17:39.000000 strauss-0.1.2/src/strauss/utilities.py
+drwxrwxr-x   0 youless   (1002) youless   (1002)        0 2024-04-22 08:48:06.189615 strauss-0.1.2/src/strauss.egg-info/
+-rw-r--r--   0 youless   (1002) youless   (1002)     3026 2024-04-22 08:48:06.000000 strauss-0.1.2/src/strauss.egg-info/PKG-INFO
+-rw-rw-r--   0 youless   (1002) youless   (1002)      993 2024-04-22 08:48:06.000000 strauss-0.1.2/src/strauss.egg-info/SOURCES.txt
+-rw-rw-r--   0 youless   (1002) youless   (1002)        1 2024-04-22 08:48:06.000000 strauss-0.1.2/src/strauss.egg-info/dependency_links.txt
+-rw-rw-r--   0 youless   (1002) youless   (1002)      119 2024-04-22 08:48:06.000000 strauss-0.1.2/src/strauss.egg-info/requires.txt
+-rw-rw-r--   0 youless   (1002) youless   (1002)        8 2024-04-22 08:48:06.000000 strauss-0.1.2/src/strauss.egg-info/top_level.txt
```

### Comparing `strauss-0.1.1/LICENSE` & `strauss-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `strauss-0.1.1/PKG-INFO` & `strauss-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strauss
-Version: 0.1.1
+Version: 0.1.2
 Summary: Sonification Tools and Resources for Astronomers Using Sound Synthesis
 Home-page: https://github.com/james-trayford/strauss
 Author: James Trayford
 Author-email: james.trayford@port.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,27 +25,27 @@
 Requires-Dist: wavio
 Requires-Dist: wheel
 Requires-Dist: sounddevice
 
 # STRAUSS
 ***S**onification **T**ools and **R**esources for **A**stronomers **U**sing **S**ound **S**ynthesis*
 
-![Sonification Tools & Resources for Astronomers Using Sound Synthesis](/misc/strauss_logo.png "STRAUSS logo")
+![Sonification Tools & Resources for Astronomers Using Sound Synthesis](https://github.com/james-trayford/strauss/tree/main/misc/strauss_logo.png)
 
 ## Sonification and STRAUSS
 
 *"Sonification"* is the process of conveying data via the medium of sound. Sonification can be used to make scientific data more accessible to those with visual impairments, enhance visualisations and movies, and even convey information more efficiently than by visual means. The *STRAUSS* python package is intended to make sonification simple for both scientific and outreach applications.
 
 ## Getting Started
 
 Access the [full documentation here](https://strauss.readthedocs.io/) *(under construction!)* and read more about the associated [Audio Universe project here](https://www.audiouniverse.org/).
 
 Releases are registered on [PyPI](https://pypi.org/project/strauss). *STRAUSS* may be installed using pip.
 
-Development is occurring at the [*STRAUSS* GitHub page](https://github.com/james-trayford/strauss.git strauss).
+Development is occurring at the [*STRAUSS* GitHub page](https://github.com/james-trayford/strauss.git).
 
 Make a copy of the *STRAUSS* repository via SSH,
 
 `git clone git@github.com:james-trayford/strauss.git strauss`
 
 or HTTPS if you don't have [SSH keys set up](https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh),
 
@@ -70,9 +70,9 @@
 before `pip install -e .`
 
 and activate the environment with
 
 `conda activate strauss`
 
 ## Acknowledgments
-The *STRAUSS* code has benefited from funding via an [Royal Astronomical Society Eduaction & Outreach grant award](https://ras.ac.uk/awards-and-grants/outreach/education-outreach-small-grants-scheme), providing hardware and software for sound development and spatialisation testing.
+The *STRAUSS* code has benefited from funding via an [Royal Astronomical Society Education & Outreach grant award](https://ras.ac.uk/awards-and-grants/outreach/education-outreach-small-grants-scheme), providing hardware and software for sound development and spatialisation testing.
```

### Comparing `strauss-0.1.1/README.md` & `strauss-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # STRAUSS
 ***S**onification **T**ools and **R**esources for **A**stronomers **U**sing **S**ound **S**ynthesis*
 
-![Sonification Tools & Resources for Astronomers Using Sound Synthesis](/misc/strauss_logo.png "STRAUSS logo")
+![Sonification Tools & Resources for Astronomers Using Sound Synthesis](https://github.com/james-trayford/strauss/tree/main/misc/strauss_logo.png)
 
 ## Sonification and STRAUSS
 
 *"Sonification"* is the process of conveying data via the medium of sound. Sonification can be used to make scientific data more accessible to those with visual impairments, enhance visualisations and movies, and even convey information more efficiently than by visual means. The *STRAUSS* python package is intended to make sonification simple for both scientific and outreach applications.
 
 ## Getting Started
 
 Access the [full documentation here](https://strauss.readthedocs.io/) *(under construction!)* and read more about the associated [Audio Universe project here](https://www.audiouniverse.org/).
 
 Releases are registered on [PyPI](https://pypi.org/project/strauss). *STRAUSS* may be installed using pip.
 
-Development is occurring at the [*STRAUSS* GitHub page](https://github.com/james-trayford/strauss.git strauss).
+Development is occurring at the [*STRAUSS* GitHub page](https://github.com/james-trayford/strauss.git).
 
 Make a copy of the *STRAUSS* repository via SSH,
 
 `git clone git@github.com:james-trayford/strauss.git strauss`
 
 or HTTPS if you don't have [SSH keys set up](https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh),
 
@@ -42,9 +42,9 @@
 before `pip install -e .`
 
 and activate the environment with
 
 `conda activate strauss`
 
 ## Acknowledgments
-The *STRAUSS* code has benefited from funding via an [Royal Astronomical Society Eduaction & Outreach grant award](https://ras.ac.uk/awards-and-grants/outreach/education-outreach-small-grants-scheme), providing hardware and software for sound development and spatialisation testing.
+The *STRAUSS* code has benefited from funding via an [Royal Astronomical Society Education & Outreach grant award](https://ras.ac.uk/awards-and-grants/outreach/education-outreach-small-grants-scheme), providing hardware and software for sound development and spatialisation testing.
```

### Comparing `strauss-0.1.1/setup.cfg` & `strauss-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = strauss
-version = 0.1.1
+version = 0.1.2
 author = James Trayford
 author_email = james.trayford@port.ac.uk
 description = Sonification Tools and Resources for Astronomers Using Sound Synthesis
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/james-trayford/strauss
 classifiers =
```

### Comparing `strauss-0.1.1/src/strauss/channels.py` & `strauss-0.1.2/src/strauss/channels.py`

 * *Files identical despite different names*

### Comparing `strauss-0.1.1/src/strauss/generator.py` & `strauss-0.1.2/src/strauss/generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,22 +5,30 @@
 choices dictated by the :obj:`Score`.
 
 Todo:
     * Consolidate more common code into the :obj:`Generator` parent
       class.
     * Support more Envelope and LFO types in the :obj:`play` methods
       (want pitch, volume and filter options for each)
+    * Check buffer length consistency for spectralizer - do we hit
+      grid points?
+    * Throw appropriate errors when rendering with unreasonable length
+      and freq combinations
 """
 
 from . import stream
 from . import notes
 from . import presets
 from . import utilities as utils
 from . import filters
 import numpy as np
+import scipy
+# use FFTW backend in scipy
+#scipy.fft.set_backend(pyfftw.interfaces.scipy_fft)
+from scipy.fft import fft, ifft, fftfreq
 import glob
 import copy
 import scipy
 from scipy.io import wavfile
 from scipy.interpolate import interp1d
 import matplotlib.pyplot as plt
 import warnings
@@ -90,15 +98,15 @@
         """
         if not hasattr(self, preset):
             self.preset = getattr(presets, self.gtype).load_preset('default')
             self.preset['ranges'] = getattr(presets, self.gtype).load_ranges() 
         if preset != 'default':
             preset = getattr(presets, self.gtype).load_preset(preset)
             self.modify_preset(preset)
-        
+
     def modify_preset(self, parameters, cleargroup=[]):
         """modify parameters within current preset
 
         method allows user to tweak generator parameters directly,
         using a dictionary of parameters and their values. subgroups
         within the preset are represented as nested dictionaries. 
 
@@ -113,15 +121,15 @@
         """
         utils.nested_dict_reassign(parameters, self.preset)
         for grp in cleargroup:
             if grp in parameters:
                 for k in list(self.preset[grp].keys()):
                     if k not in parameters[grp]:
                         del self.preset[grp][k]
-
+            
     def preset_details(self, term="*"):
         """ Print the names and descriptions of presets
 
         Wrapper for preset_details function. lists the name and description
         of built-in presets with names matching the search term.
 
         Args:
@@ -470,15 +478,15 @@
         samprate = self.samprate
         audbuff = self.audbuff
 
         params = copy.deepcopy(self.preset)
         utils.linear_to_nested_dict_reassign(mapping, params)
 
         nlength = (params['note_length']+params['volume_envelope']['R'])*samprate
-
+        
         # generator stream (attribute of stream?)
         sstream = stream.Stream(nlength/samprate, samprate)
         samples = sstream.samples
         sstream.get_sampfracs()
 
         pindex  = np.zeros(samples.size)
         if callable(params['pitch_shift']):
@@ -741,14 +749,221 @@
                 sstream.bufferize(sstream.length/4)
             else:
                 # 30 ms buffer (hardcoded for now)
                 sstream.bufferize(0.03)
             sstream.filt_sweep(getattr(filters, params['filter_type']),
                                utils.const_or_evo_func(params['cutoff']))
         return sstream    
+
+class Spectralizer(Generator):
+    """Spectralizer generator class
+    """
+    def __init__(self, params=None, samprate=48000):
+
+        # default synth preset
+        self.gtype = 'spec'
+        self.preset = getattr(presets, self.gtype).load_preset()
+        self.preset['ranges'] = getattr(presets, self.gtype).load_ranges() 
+
+        self.freqwarn = True
+        
+        # universal initialisation for generator objects:
+        super().__init__(params, samprate)
+
+    def spectrum_to_signal(self, spectrum, phases, new_nlen, mindx, maxdx, interp_type):
+        """ Convert the input spectrum into sound signal
+        """        
+
+        # NOTE: interpolation around a delta function can lead to splitting power between adjacent
+        # frequencies and result in an artificial beating. This can be avoided by choosing values
+        # a length that places the spectrum on the grid exactly
+        
+        if interp_type == "sample":
+            ps = np.interp(np.linspace(0,1,maxdx-mindx), np.linspace(0, 1, spectrum.size), spectrum)
+        elif interp_type == "preserve_power":
+            # we don't renormalise by len(ps) / spectrum.size,
+            # as renormalising to peak later anyway.
+            ps = np.diff(np.interp(np.linspace(0, 1, maxdx-mindx+1),
+                                   np.linspace(0, 1, spectrum.size),
+                                   np.cumsum(spectrum)))
+           
+        empt = np.zeros(new_nlen)
+        empt[mindx:maxdx] = ps
+        ps = empt
+        PS = ps*np.cos(phases) + 1j*ps*np.sin(phases)
+        return np.real(ifft(PS))[:new_nlen]
+        
+    def play(self, mapping):
+        """ Play the sound for a given source.
+
+        Play a given source and return the sample values for
+        combination into the overall sonification.
+
+        Note:
+          :obj:`mapping` is a linear dictionary (not nested, as for 
+          :meth:`strauss.generator.modify_preset`) where group members
+          are indicated using :obj:`'/'` notation
+          (e.g. :obj:`{'volume_envelope/A': 0.5, ...`).
+
+        Args:
+          mapping (:obj:`dict`): keys and items are generator
+            parameter names and their values. This combines all the
+            preset mapped parameters, overwritten by any
+            :obj:`Source`-mapped parameters (represented as values or
+            interpolation functions for static and evolving
+            parameters, respectively). This is a linear dictionary
+            (not nested, see :meth:`strauss.generator.modify_preset`)
+            where group members are indicated using :obj:`'/'`
+            notation (e.g. :obj:`{'volume_envelope/A': 0.5, ...`).
+
+        """
+        samprate = self.samprate
+        audbuff = self.audbuff
+
+        params = copy.deepcopy(self.preset)
+        utils.linear_to_nested_dict_reassign(mapping, params)
+
+        duration = (params['note_length']+params['volume_envelope']['R'])
+        nlength = int(duration*samprate)
+        # generator stream (attribute of stream?)
+        sstream = stream.Stream(nlength/samprate, samprate)
+        samples = sstream.samples
+        sstream.get_sampfracs()
+
+        spectrum = params['spectrum']
+        interp_type = params['interpolation_type']
+        
+        if np.array(spectrum).ndim == 1:
+            # number of discrete frequencies available in ifft between freq. limits 
+            discrete_freqs = duration*(params['max_freq']-params['min_freq'])
+            
+            # how many spectra points fit into the available intermediate frequencies
+            spectra_multiples = (discrete_freqs - 1)/(spectrum.size - 1)
+            
+            # the minimum factor by which to increase the stream length to accomodate spectra in whole number multiples
+            buffer_factor = np.ceil(spectra_multiples)/spectra_multiples
+
+            # number of samples to generate including buffer
+            new_nlen = int(buffer_factor * nlength)
+        
+            # the frequency bound indices which the spectrum will be mapped into
+            mindx = int(params['min_freq'] * duration * buffer_factor)
+            maxdx = int(params['max_freq'] * duration * buffer_factor)
+            
+            # hardcode phase randomisation for now
+            phases = 2*np.pi*np.random.random(new_nlen)
+            
+            # generate stream values
+            sstream.values = self.spectrum_to_signal(spectrum, phases, new_nlen, mindx, maxdx, interp_type)[:nlength]
+        else:
+
+            if 'time_evo' in params:
+                np.diff(params['time_evo'])
+
+            nspec, nwlen  = np.array(spectrum).shape
+                
+            # buffer for each spectrum
+            buffdur = duration / (nspec-1)
+            sstream.bufferize(buffdur)
+
+            # indices of IFFT input spectrum corresponding to the nearest desired frequencies
+            # NOTE: we don't force the spectrum to reproduce desired frequencies to the accuracy of
+            # a few samples in the evolving spectrum case.
+            mindx = np.round(params['min_freq'] * buffdur).astype(int)
+            maxdx = np.round(params['max_freq'] * buffdur).astype(int)
+
+            if ((maxdx - mindx)*10 < nwlen) and self.freqwarn and params['interpolation_type'] == 'sample':
+
+                basewarn = ("\n\n Spectrum strongly undersampled (by more than a factor 10) while using 'sample' \n"
+                            "interpolation type. This could miss spectral features. You could consider: \n"
+                            "\t - Changing interpolation type to 'preserve power' (i.e. generator.modify_preset({'interpolation_type':'preserve_power'})) \n")
+
+                fdiff = params['max_freq']- params['min_freq']
+                newdur = (nwlen/fdiff) *(nspec-1)
+                if newdur < 300: # i.e. 5 minutes
+                    # suggest increasing duration if reasonable 
+                    basewarn += f"\t - Increase the duration of the sonification (e.g. to > {newdur:.0f}) \n"
+                if ((2e4 - 30) * buffdur > nwlen):
+                    newdiff = np.log10(nwlen / buffdur)
+                    flo = pow(10,0.5*(np.log10(30) + np.log10(2e4)) - 0.5*newdiff)
+                    fhi = pow(10,0.5*(np.log10(30) + np.log10(2e4)) + 0.5*newdiff)
+                    basewarn += f"\t - Increase the sound frequency range eg ({np.floor(flo):.0f} to {np.ceil(fhi):.0f} Hz)\n"
+
+                warnings.warn(basewarn
+                    + f"\t - Rebin spectra more coarsely \n")
+                    
+                # only warn once per instance
+                self.freqwarn = False
+            
+            # length of buffer and therefore IFFT in this case
+            new_nlen = sstream.buffers._nsamp_buff
+            
+            # hardcode phase randomisation for now
+            phases = 2*np.pi*np.random.random(new_nlen)
+            
+            # iterate through buffers and spectra
+            nolap = nspec-1
+            buffsize = sstream.buffers._nsamp_buff
+
+            for i in range(nspec):
+                # print(buffsize)
+                buffs = self.spectrum_to_signal(spectrum[i], phases, new_nlen,
+                                                mindx, maxdx, interp_type)
+                # print(sstream.buffers._nsamp_buff, buffs.size)
+                sstream.buffers.buffs_tile[i] = buffs[:sstream.buffers._nsamp_buff]
+                if i == nolap:
+                    continue
+                # print(sstream.buffers.buffs_tile[i][0], sstream.buffers.buffs_tile[i][-1])
+                sstream.buffers.buffs_olap[i][buffsize//2:] = sstream.buffers.buffs_tile[i][:buffsize//2]
+                sstream.buffers.buffs_olap[i][:buffsize//2] = sstream.buffers.buffs_tile[i][buffsize//2:]
+
+                if params['regen_phases']:
+                    # regenerate randomised phases if doing so
+                    phases = 2*np.pi*np.random.random(new_nlen)
+                  
+            sstream.consolidate_buffers()
+            
+
+        sstream.values /= abs(sstream.values).max()
+        
+        # get volume envelope
+        env = self.envelope(sstream.samples, params)
+        if params['volume_lfo']['use']:
+            env *= np.clip(1.-self.lfo(sstream.samples, sstream.sampfracs,
+                                       params, 'volume')*0.5, 0, 1)
+
+        pindex  = np.zeros(samples.size)
+        if callable(params['pitch_shift']):
+            pindex += params['pitch_shift'](sstream.sampfracs)/12.
+        elif params['pitch_shift'] != 0:
+            pindex += params['pitch_shift']/12.
+        if params['pitch_lfo']['use']:
+            pindex += self.lfo(samples, sstream.sampfracs, params, 'pitch')/12.
+        if np.any(pindex):
+            sampfunc = interp1d(samples, sstream.values,
+                                bounds_error=False,
+                                fill_value = (0.,0.),
+                                assume_sorted=True)
+            newsamp = np.cumsum(pow(2., pindex))
+            sstream.values = sampfunc(newsamp)
+
+        # apply volume normalisation or modulation (TO DO: envelope, pre or post filter?)
+        sstream.values *= utils.const_or_evo(params['volume'], sstream.sampfracs) * env
+
+        # filter stream
+        if params['filter'] == "on":
+            if hasattr(params['cutoff'], "__iter__"):
+                # if static cutoff, use minimum buffer count
+                sstream.bufferize(sstream.length/4)
+        else:
+            # 30 ms buffer (hardcoded for now)
+            sstream.bufferize(0.03)
+            sstream.filt_sweep(getattr(filters, params['filter_type']),
+                               utils.const_or_evo_func(params['cutoff']))
+        return sstream    
     
 def gen_chord(stream, chordname, rootoctv=3):
     """DEPRECATED CODE:
     generate chord over entire stream given chord name and optional
     octave of root note
     """
     frqs = notes.parse_chord(chordname, rootoctv)
```

### Comparing `strauss-0.1.1/src/strauss/notes.py` & `strauss-0.1.2/src/strauss/notes.py`

 * *Files identical despite different names*

### Comparing `strauss-0.1.1/src/strauss/presets/sampler/__init__.py` & `strauss-0.1.2/src/strauss/presets/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `strauss-0.1.1/src/strauss/presets/sampler/default.yml` & `strauss-0.1.2/src/strauss/presets/sampler/default.yml`

 * *Files 22% similar despite different names*

```diff
@@ -72,11 +72,16 @@
 
 # Master Volume
 volume: 1.
 
 # Default pitch selection
 pitch: 1.
 
+# center panning:
+azimuth: 0.
+polar: 0
+
 # pitch range and default shift in semitones
 pitch_hi: 36
 pitch_lo: 0
 pitch_shift: 0.
+
```

### Comparing `strauss-0.1.1/src/strauss/presets/sampler/ranges/default.yml` & `strauss-0.1.2/src/strauss/presets/sampler/ranges/default.yml`

 * *Files identical despite different names*

### Comparing `strauss-0.1.1/src/strauss/presets/synth/__init__.py` & `strauss-0.1.2/src/strauss/presets/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `strauss-0.1.1/src/strauss/presets/synth/default.yml` & `strauss-0.1.2/src/strauss/presets/synth/default.yml`

 * *Files identical despite different names*

### Comparing `strauss-0.1.1/src/strauss/presets/synth/ranges/default.yml` & `strauss-0.1.2/src/strauss/presets/synth/ranges/default.yml`

 * *Files identical despite different names*

### Comparing `strauss-0.1.1/src/strauss/score.py` & `strauss-0.1.2/src/strauss/score.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,30 +48,41 @@
     	notation, e.g. :obj:`[['C3','E3', 'G3'], ['C3', 'F3', 'A4']]`. If
     	floats, take values as note frequency in Hz. NOTE: currently
     	only supported in compination with the :obj:`Synthesiser`
     	generator class.
       length: (:obj:`str` or :obj:`float`): the length of the
     	sonification. If a string, parse minutes and seconds from
     	format 'Xm Y.Zs'. If a float read as seconds.
+      pitch_binning (optional, :obj:`str`): pitch binning mode - choose
+        from 'adaptive', where sources are binned by the pitch mapping
+        such that each interval is represented the same fraction of the
+        time, and 'uniform' where the pitch binning is based on uniform
+        size bins in the mapped pitch parameter. 
     """
-    def __init__(self, chord_sequence, length):
+    def __init__(self, chord_sequence, length, pitch_binning='adaptive'):
         # check types to handle score length correctly
         if isinstance(length, str):
             regex = "([0-9]*)m\s*([0-9]*.[0-9]*)s"
             reobj = re.match(regex, length, re.M | re.I)
             self.length = float(reobj.group(1))*60. + float(reobj.group(2))            
         else:
             self.length = length        
         
         # check types to handle different chord formats correctly
         if isinstance(chord_sequence, list):
             self.note_sequence = chord_sequence
         if isinstance(chord_sequence, str):
             self.note_sequence = parse_chord_sequence(chord_sequence)
 
+        if pitch_binning in ['adaptive','uniform']:
+            self.pitch_binning = pitch_binning
+        else:
+            raise Exception(
+                f"\"{pitch_binning}\" is not a valid pitch_binning mode")        
+
         # number of chords in the sequence 
         self.nchords = len(self.note_sequence)
         self.nintervals = [len(c) for c in self.note_sequence]
         
         # For now, chords changes are just equally spaced in the timeline
         self.fracbins = np.linspace(0,1, self.nchords+1) 
         self.timebins = self.length * self.fracbins
```

### Comparing `strauss-0.1.1/src/strauss/sonification.py` & `strauss-0.1.2/src/strauss/sonification.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,27 +11,30 @@
 
 Todo:
   * Delegate more musical process to the :obj:`score` module
 """
 
 from .stream import Stream
 from .channels import audio_channels
-from .utilities import const_or_evo, nested_dict_idx_reassign
+from .utilities import const_or_evo, nested_dict_idx_reassign, NoSoundDevice
 import numpy as np
 import matplotlib.pyplot as plt
 from tqdm import tqdm
 import sys
 import os
 import ffmpeg as ff
 import wavio as wav
 import IPython.display as ipd
 from IPython.core.display import display
 from scipy.io import wavfile
 import warnings
-import sounddevice as sd
+try:
+    import sounddevice as sd
+except OSError as sderr:
+    sd = NoSoundDevice(sderr)
 
 class Sonification:
     """Representing the overall sonification
 
     This class combines the data sources, musical score constraints
     and generator together to generate and render the ultimate
     sonification for saving or playing in the :obj:`jupyter-notebook`
@@ -110,16 +113,19 @@
             
         # index each chord
         cbin = np.digitize(self.sources.mapping['time'], self.score.fracbins, 0)
         cbin = np.clip(cbin-1, 0, self.score.nchords-1)
 
         # pitch rank of each source divided by the number of sources
         pitchfrac = np.empty_like(self.sources.mapping['pitch'])
-        pitchfrac[np.argsort(self.sources.mapping['pitch'])] = np.arange(self.sources.n_sources)/self.sources.n_sources
-
+        if self.score.pitch_binning == 'adaptive':
+            pitchfrac[np.argsort(self.sources.mapping['pitch'])] = np.arange(self.sources.n_sources)/self.sources.n_sources
+        elif self.score.pitch_binning == 'uniform':
+            pitchfrac = np.clip(self.sources.mapping['pitch'], 0, 9.999999e-1)
+            
         # get some relevant numbers before iterating through sources
         Nsamp = self.out_channels['0'].values.size
         lastsamp = Nsamp - 1
         Nchan = len(self.out_channels.keys())
         indices = range(0,self.sources.n_sources, downsamp)
 
         for source in tqdm(indices):
@@ -127,14 +133,15 @@
             # index note properties
             t = self.sources.mapping['time'][source]
             tsamp = int(Nsamp * t)
             chord = self.score.note_sequence[cbin[source]]
             nints = self.score.nintervals[cbin[source]]
             pitch = pitchfrac[source]
             note = chord[int(pitch * nints)]
+
             # make dictionary for feeding to play function with each notes properties
             sourcemap = {}
             # for k in self.sources.mapping.keys():
             #     sourcemap[k] = self.soures.mapping[k][source]
             nested_dict_idx_reassign(self.sources.mapping, sourcemap, source)
             sourcemap['note'] = note
 
@@ -294,15 +301,15 @@
             chans[:,c] = (vals*norm).astype("int32")
             
         # finally combine and write out wav file
         wavfile.write(fname, self.samprate, chans)
         print(f"Saved {fname}")
 
         
-    def notebook_display(self):
+    def notebook_display(self, show_waveform=True):
         """ plot the waveforms and embed player in the notebook
 
         Show waveforms and embed an audio player in the python
         notebook for direct playback. the notebook player only
         supports up to stereo, so if more than two channels, only the
         first two are used as left and right.
         """
@@ -312,34 +319,35 @@
         for c in range(len(self.out_channels)):
             vmax = max(
                 abs(self.out_channels[str(c)].values.max()),
                 abs(self.out_channels[str(c)].values.min()),
                 vmax
             ) * 1.05
         
-        for i in range(len(self.out_channels)):
-            plt.plot(time[::20], self.out_channels[str(i)].values[::20]+2*i*vmax, label=self.channels.labels[i])
-
-        plt.xlabel('Time (s)')
-        plt.ylabel('Relative Amplitude')
-        plt.legend(frameon=False, loc=5)
-        plt.xlim(-time[-1]*0.05,time[-1]*1.2)
-        for s in plt.gca().spines.values():
-            s.set_visible(False)
-        plt.gca().get_yaxis().set_visible(False)
+        if show_waveform:
+            for i in range(len(self.out_channels)):
+                plt.plot(time[::20], self.out_channels[str(i)].values[::20]+2*i*vmax, label=self.channels.labels[i])
+            plt.xlabel('Time (s)')
+            plt.ylabel('Relative Amplitude')
+            plt.legend(frameon=False, loc=5)
+            plt.xlim(-time[-1]*0.05,time[-1]*1.2)
+            for s in plt.gca().spines.values():
+                s.set_visible(False)
+                plt.gca().get_yaxis().set_visible(False)
+            plt.show()
+        
 
         if len(self.channels.labels) == 1:
             # we have used 48000 Hz everywhere above as standard, but to quickly hear the sonification sped up / slowed down,
             # you can modify the 'rate' argument below (e.g. multiply by 0.5 for half speed, by 2 for double speed, etc)
             outfmt = np.column_stack([self.out_channels['0'].values, self.out_channels['0'].values]).T
         else:
             outfmt = np.column_stack([self.out_channels['0'].values, self.out_channels['1'].values]).T
-        plt.show()
         display(ipd.Audio(outfmt,rate=self.out_channels['0'].samprate, autoplay=False))
-
+        
     def hear(self):
         """ Play audio directly to the sound device, for command-line
             playback.
         """
 
         vmax = 0.
         for c in range(len(self.out_channels)):
@@ -358,13 +366,11 @@
         dur = int(np.round(outfmt.shape[0]/self.out_channels['0'].samprate))
         playback_msg = f"Playing Sonification ({dur} s): "
         print(playback_msg)
         try:
             sd.play(outfmt,self.out_channels['0'].samprate,blocking=1)
         except OSError as error: 
             print(error) 
-            print("The Sonification.hear() function requires the PortAudio C-library. This may be missing from your system or "
-                  "unsupported in this context. This should be installed by pip on Windows and OSx automatically with the "
+            print("The Sonification.hear() function requires the PortAudio C-library. This may be missing from your system or \n"
+                  "unsupported in this context. This should be installed by pip on Windows and OSx automatically with the \n "
                   "sounddevice library, but on Linux you may need to install manually using e.g.:\n"
-                  "\t 'sudo apt-get install libportaudio2.'\n") 
-
-
+                  "\t 'sudo apt-get install libportaudio2.'\n")
```

### Comparing `strauss-0.1.1/src/strauss/sources.py` & `strauss-0.1.2/src/strauss/sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
             'theta',
             'phi',
             'volume',
             'pitch',
             'time',
             'cutoff',
             'time_evo',
+            'spectrum',
             'pitch_shift',
             'volume_envelope/A',
             'volume_envelope/D',
             'volume_envelope/S',
             'volume_envelope/R',
             'volume_lfo/freq',
             'volume_lfo/freq_shift',
@@ -66,14 +67,15 @@
                 (0,1),#np.pi),
                 (0,1),#2*np.pi),
                 (0,1),
                 (0,1),
                 (0,1),
                 (0,1),
                 (0,1),
+                (0,1),
                 (0,24),
                 (1e-2, 10),
                 (1e-2, 10),
                 (0,1),
                 (1e-2, 10),
                 (1,12),
                 (0,3),
@@ -217,14 +219,18 @@
                 scaledvals = rescale_values(np.array(mapvals), lims, plims)
                 self.mapping[key] =  list(scaledvals)
             
         # finally, iterate through sources and interpolate evo functions 
         for key in self.mapping:
             if key == "time_evo":
                 continue
+            if key == "spectrum":
+                # if hasattr(self.mapping[key][0][0], "__iter__"):
+                # ^ in case we want to catch and pre process multi-spectra
+                continue
             elif hasattr(self.mapping[key][0], "__iter__"):
                 # print(key, self.mapping[key][0])
                 for i in range(self.n_sources):
                     if key not in evolvable:
                         raise Exception(f"Mapping error: Parameter \"{key}\" cannot be evolved.")
                     x = self.mapping["time_evo"][i]
                     y = self.mapping[key][i]
@@ -271,15 +277,15 @@
         	sources can be represented as single values.
         """
         for key in self.mapped_quantities:
             if key in datadict:
                 self.raw_mapping[key] = datadict[key]
             else:
                 Exception(f"Mapped property {key} not in datadict.")
-        self.n_sources = datadict[key].shape[0]
+        self.n_sources = np.array(datadict[key]).shape[0]
  
 class Objects(Source):
     """ Represent data as time-continuous objects.
     
     Child class of `Source`. In addition to supporting single values
     for each parameter (see `Events` class), objects also support
     time evolution for `evolvable` parameters, given a `time-evo`
@@ -310,8 +316,7 @@
             else:
                 Exception(f"Mapped property {key} not in datadict.")
         self.n_sources = np.array(self.raw_mapping[key]).shape[0]
 
 class UnrecognisedProperty(Exception):
     "Error raised when trying to map unrecognised parameters"
     pass
-
```

### Comparing `strauss-0.1.1/src/strauss/stream.py` & `strauss-0.1.2/src/strauss/stream.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import wavio
 import matplotlib.pyplot as plt
+from scipy.signal.windows import hann
 # To Do
 # - implement filter Q-parameter mapping
 
 class Stream:
     """ Stream object representing audio samples"""
     def __init__(self, length, samprate=44100):
         # variables we want to keep constant
@@ -97,15 +98,16 @@
         # minimum number of tiled buffers to completely enclose stream 
         self._nbuffs = 1+(stream._nsamp_stream//self._nsamp_buff)
 
         # total number buffers including overlaps
         self._nbuffs_tot = 2*self._nbuffs-1
 
         # tent function for linearly x-fading buffers on recombination
-        self.fade = 1.-abs(np.linspace(1,-1, self._nsamp_buff))
+        # self.fade = 1.-abs(np.linspace(1,-1, self._nsamp_buff))
+        self.fade = hann(self._nsamp_buff)
 
         # pad the stream up to an exact multiple of buffer sample length
         self.nsamp_padstream = self._nbuffs * self._nsamp_buff
         self.nsamp_pad = self.nsamp_padstream-stream._nsamp_stream
         self.olap_pad = self.nsamp_pad-self._nsamp_halfbuff
         self.olap_lim = min(stream._nsamp_stream, stream._nsamp_stream+self.olap_pad)
```

### Comparing `strauss-0.1.1/src/strauss/utilities.py` & `strauss-0.1.2/src/strauss/utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 from functools import reduce
 import operator
 import numpy as np
 from scipy.interpolate import interp1d
 
+
+class NoSoundDevice:
+    """
+    drop-in replacement for sounddevice module if not working,
+    so can still use other functionality.
+    """
+    def __init__(self, err):
+        self.err = err
+    def play(self, audio, rate, blocking=1):
+        raise self.err
+        
 # a load of utility functions used by STRAUSS
 
 def nested_dict_reassign(fromdict, todict):
     """recurse through dictionaries and sub-dictionaries"""
     for k, v in fromdict.items():
         if isinstance(v, dict):
             # recurse through nested dictionaries
```

### Comparing `strauss-0.1.1/src/strauss.egg-info/PKG-INFO` & `strauss-0.1.2/src/strauss.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strauss
-Version: 0.1.1
+Version: 0.1.2
 Summary: Sonification Tools and Resources for Astronomers Using Sound Synthesis
 Home-page: https://github.com/james-trayford/strauss
 Author: James Trayford
 Author-email: james.trayford@port.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,27 +25,27 @@
 Requires-Dist: wavio
 Requires-Dist: wheel
 Requires-Dist: sounddevice
 
 # STRAUSS
 ***S**onification **T**ools and **R**esources for **A**stronomers **U**sing **S**ound **S**ynthesis*
 
-![Sonification Tools & Resources for Astronomers Using Sound Synthesis](/misc/strauss_logo.png "STRAUSS logo")
+![Sonification Tools & Resources for Astronomers Using Sound Synthesis](https://github.com/james-trayford/strauss/tree/main/misc/strauss_logo.png)
 
 ## Sonification and STRAUSS
 
 *"Sonification"* is the process of conveying data via the medium of sound. Sonification can be used to make scientific data more accessible to those with visual impairments, enhance visualisations and movies, and even convey information more efficiently than by visual means. The *STRAUSS* python package is intended to make sonification simple for both scientific and outreach applications.
 
 ## Getting Started
 
 Access the [full documentation here](https://strauss.readthedocs.io/) *(under construction!)* and read more about the associated [Audio Universe project here](https://www.audiouniverse.org/).
 
 Releases are registered on [PyPI](https://pypi.org/project/strauss). *STRAUSS* may be installed using pip.
 
-Development is occurring at the [*STRAUSS* GitHub page](https://github.com/james-trayford/strauss.git strauss).
+Development is occurring at the [*STRAUSS* GitHub page](https://github.com/james-trayford/strauss.git).
 
 Make a copy of the *STRAUSS* repository via SSH,
 
 `git clone git@github.com:james-trayford/strauss.git strauss`
 
 or HTTPS if you don't have [SSH keys set up](https://docs.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh),
 
@@ -70,9 +70,9 @@
 before `pip install -e .`
 
 and activate the environment with
 
 `conda activate strauss`
 
 ## Acknowledgments
-The *STRAUSS* code has benefited from funding via an [Royal Astronomical Society Eduaction & Outreach grant award](https://ras.ac.uk/awards-and-grants/outreach/education-outreach-small-grants-scheme), providing hardware and software for sound development and spatialisation testing.
+The *STRAUSS* code has benefited from funding via an [Royal Astronomical Society Education & Outreach grant award](https://ras.ac.uk/awards-and-grants/outreach/education-outreach-small-grants-scheme), providing hardware and software for sound development and spatialisation testing.
```

### Comparing `strauss-0.1.1/src/strauss.egg-info/SOURCES.txt` & `strauss-0.1.2/src/strauss.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -19,13 +19,16 @@
 src/strauss.egg-info/dependency_links.txt
 src/strauss.egg-info/requires.txt
 src/strauss.egg-info/top_level.txt
 src/strauss/presets/__init__.py
 src/strauss/presets/sampler/__init__.py
 src/strauss/presets/sampler/default.yml
 src/strauss/presets/sampler/ranges/default.yml
+src/strauss/presets/spec/__init__.py
+src/strauss/presets/spec/default.yml
+src/strauss/presets/spec/ranges/default.yml
 src/strauss/presets/synth/__init__.py
 src/strauss/presets/synth/default.yml
 src/strauss/presets/synth/pitch_mapper.yml
 src/strauss/presets/synth/spectraliser.yml
 src/strauss/presets/synth/windy.yml
 src/strauss/presets/synth/ranges/default.yml
```


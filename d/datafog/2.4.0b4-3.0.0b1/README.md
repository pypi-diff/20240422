# Comparing `tmp/datafog-2.4.0b4.tar.gz` & `tmp/datafog-3.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-2.4.0b4.tar", last modified: Tue Apr  2 02:16:36 2024, max compression
+gzip compressed data, was "datafog-3.0.0b1.tar", last modified: Sun Apr 21 23:51:34 2024, max compression
```

## Comparing `datafog-2.4.0b4.tar` & `datafog-3.0.0b1.tar`

### file list

```diff
@@ -1,23 +1,20 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-02 02:16:36.643102 datafog-2.4.0b4/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-03-28 17:43:37.000000 datafog-2.4.0b4/LICENSE
--rw-r--r--   0 sidmohan   (501) staff       (20)     7749 2024-04-02 02:16:36.642817 datafog-2.4.0b4/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)     6355 2024-03-28 17:43:37.000000 datafog-2.4.0b4/README.md
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-04-02 02:16:36.643178 datafog-2.4.0b4/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)     1712 2024-04-02 02:00:59.000000 datafog-2.4.0b4/setup.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-02 02:16:36.629112 datafog-2.4.0b4/src/
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-02 02:16:36.633524 datafog-2.4.0b4/src/datafog/
--rw-r--r--   0 sidmohan   (501) staff       (20)       53 2024-03-28 17:43:37.000000 datafog-2.4.0b4/src/datafog/__about__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     4866 2024-04-02 02:15:41.000000 datafog-2.4.0b4/src/datafog/__init__.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-02 02:16:36.629381 datafog-2.4.0b4/src/datafog/pii_tools/
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-02 02:16:36.640915 datafog-2.4.0b4/src/datafog/pii_tools/PresidioEngine/
--rw-r--r--   0 sidmohan   (501) staff       (20)     6651 2024-04-02 02:15:41.000000 datafog-2.4.0b4/src/datafog/pii_tools/PresidioEngine/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     6226 2024-04-02 02:15:41.000000 datafog-2.4.0b4/src/datafog/pii_tools/PresidioEngine/analyzer.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-02 02:16:36.642355 datafog-2.4.0b4/src/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)     7749 2024-04-02 02:16:36.000000 datafog-2.4.0b4/src/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      392 2024-04-02 02:16:36.000000 datafog-2.4.0b4/src/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-04-02 02:16:36.000000 datafog-2.4.0b4/src/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)      103 2024-04-02 02:16:36.000000 datafog-2.4.0b4/src/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        8 2024-04-02 02:16:36.000000 datafog-2.4.0b4/src/datafog.egg-info/top_level.txt
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-02 02:16:36.641743 datafog-2.4.0b4/tests/
--rw-r--r--   0 sidmohan   (501) staff       (20)     3505 2024-04-02 02:15:41.000000 datafog-2.4.0b4/tests/test_datafog.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2711 2024-04-01 15:24:39.000000 datafog-2.4.0b4/tests/test_presidio.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-21 23:51:34.663197 datafog-3.0.0b1/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-04-21 22:55:54.000000 datafog-3.0.0b1/LICENSE
+-rw-r--r--   0 sidmohan   (501) staff       (20)     7747 2024-04-21 23:51:34.662961 datafog-3.0.0b1/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6353 2024-04-21 22:55:54.000000 datafog-3.0.0b1/README.md
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-04-21 23:51:34.663246 datafog-3.0.0b1/setup.cfg
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1717 2024-04-21 23:48:45.000000 datafog-3.0.0b1/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-21 23:51:34.659613 datafog-3.0.0b1/src/
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-21 23:51:34.660735 datafog-3.0.0b1/src/datafog/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      931 2024-04-21 23:45:38.000000 datafog-3.0.0b1/src/datafog/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2106 2024-04-21 23:36:47.000000 datafog-3.0.0b1/src/datafog/models.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      402 2024-04-21 19:35:47.000000 datafog-3.0.0b1/src/datafog/utils.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-21 23:51:34.662607 datafog-3.0.0b1/src/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     7747 2024-04-21 23:51:34.000000 datafog-3.0.0b1/src/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      301 2024-04-21 23:51:34.000000 datafog-3.0.0b1/src/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-04-21 23:51:34.000000 datafog-3.0.0b1/src/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)      103 2024-04-21 23:51:34.000000 datafog-3.0.0b1/src/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       13 2024-04-21 23:51:34.000000 datafog-3.0.0b1/src/datafog.egg-info/top_level.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)      972 2024-04-21 23:34:10.000000 datafog-3.0.0b1/src/test.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-04-21 23:51:34.662304 datafog-3.0.0b1/tests/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      928 2024-04-21 23:36:39.000000 datafog-3.0.0b1/tests/test_datafog.py
```

### Comparing `datafog-2.4.0b4/LICENSE` & `datafog-3.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `datafog-2.4.0b4/PKG-INFO` & `datafog-3.0.0b1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 2.4.0b4
+Version: 3.0.0b1
 Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
 Home-page: https://datafog.ai
 Author: DataFog
 Author-email: hi@datafog.ai
 Maintainer: DataFog
 Maintainer-email: hi@datafog.ai
 License: MIT
@@ -55,84 +55,102 @@
 
 ## Overview
 
 ### What is DataFog?
 
 DataFog is an open-source DevSecOps platform that lets you scan and redact Personally Identifiable Information (PII) out of your Generative AI applications.
 
-### What problem are we solving?
+### Core Problem
 
-**Context**
+![image](https://github.com/DataFog/datafog-python/assets/61345237/57fba4e5-21cc-458f-ac6a-6fbbb70a8de1)
 
-The primary use case today is Retrieval Augmented Generation (RAG) systems. As a refresher, RAG systems operate by retrieving information from a custom knowledge base—constructed by you or your team—and leverage this information, either by directly citing the files in a response or inferred through the model's responses. This knowledge base is assembled through a deliberate process, which involves uploading files into a workflow. These files are then segmented into logical information blocks and tagged according to their contextual significance. There are a thousand ways to add nuance to this characterization, but this suffices for the vast majority of cases!
-
-**Problem**
 
 How do you keep:
 
 - Customer PII
 - Employee PII
 - Sensitive company information pertaining to org changes or restructurings
 - Pending M&A activity
 - Conversations with external counsel on material corporate matters (i.e. product recall, etc)
 - and more
 
 from entering a Generative AI environment in the first place? What you need is a tool to scan and redact your RAG-bound documents based on your organization or team needs.
 
-That's where DataFog comes in. Our solution to this problem is through two major approaches:
-
-**PII Observability** Take in your batch/streaming data and return a scan indicating character-level detection of entities
-**Privacy Filter** DataFog can slot in as a pre-processor that redacts PII from your files before they get uploaded to a RAG database
-
-With this SDK, you can import it into a Python environment (like a Google Colab notebook, check out our [Getting Started](examples/getting-started.ipynb)) and within a few lines of code you're up and running.
+**That's where DataFog comes in.**
 
 ### How it works
 
-<img src="https://www.datafog.ai/hero.png" alt="DataFog Overview" style="width:50%;">
+![image](https://github.com/DataFog/datafog-python/assets/61345237/91f4634a-8a9f-4621-81bc-09930feda78a)
+
 
 ### There's lots of PII tools out there; why DataFog?
 
 If you look at the landscape of PII detection tools, their very existence was in many cases driven by regulatory requirements (i.e. 'comply with CCPA/GDPR/HIPAA').
 In this scenario, there's a very defined problem, a specific set of immutable entities to look for, and a relatively static universe of document schema to work with. What that means as an end-result is that the products
 are purpose-built for the problem that they are solving.
 
 However, Generative AI changes how we think about privacy. There's now a changing set of privacy requirements (new M&A deals, internal discussions means new terms to scan/redact) as well as different and varying document sources to contend with. PII detection is no longer just about compliance, it's an active - and for some, new - internal security threat for CISOs and Eng Leaders to contend with. We want DataFog to be built and driven to meet the needs of the open-source community as they tackle this challenge.
 
+### Roadmap
+DataFog is an active project with regular weekly releases to production (typically on/around Monday evenings US PT).  Here's a snapshot of our coming roadmap; if you have questions or would like to weigh in, join our discord and let us know what we can do to make the product better!
+
+![image](https://github.com/DataFog/datafog-python/assets/61345237/62964d22-a221-4f1d-a0e6-0cc99de2ba92)
+
+
+
 ## Installation
 
 DataFog can be installed via pip:
 
 ```bash
 pip install datafog
 ```
 
 and in your python environment:
 
 ```
 from datafog import PresidioEngine as presidio
+datafog = datafog.DataFog()
+
 ```
 
 ## Examples
 
 Here are some examples of datafog being used to redact information in business contexts. Please see '/examples' for our [Getting Started](examples/getting-started.ipynb) notebook. We'll be regularly updating content and providing comprehensive guides to using DataFog in production contexts. If you have any ideas for a tutorial or guide that you would like to see, please let us know!
 
+### Scanning a single string
+
 ```
   ceo_email_chunk = "I'm announcing on Friday that Jeff is going to be CTO."
 
   scan_results1 = presidio.scan(ceo_email_chunk)
   print("PII Detected - base case:", scan_results1)
   # PII Detected - base case: [type: PERSON, start: 30, end: 34, score: 0.85]
 
 
   scan_results2 = presidio.scan(ceo_email_chunk, deny_list=['CTO'])
   print("PII Detected with deny list:", scan_results2)
   # PII Detected with deny list: [type: CUSTOM_PII, start: 50, end: 53, score: 1.0, type: PERSON, start: 30, end: 34, score: 0.85]
 
 ```
 
+### Scanning a list of PDFs
+
+```
+file_dir = ["/Users/sidmohan/Desktop/datafog-v2.4.0/datafog-python/tests/files/input_files/agi-builder-meetup.pdf",
+           "/Users/sidmohan/Desktop/datafog-v2.4.0/datafog-python/tests/files/input_files/pypdf-readthedocs-io-en-stable.pdf"]
+datafog = datafog.DataFog()
+result = datafog.upload_files(uploaded_files=file_dir)
+print(result)
+```
+
+The output here will be a dictionary where the keys are the file names and the values are the scan results for that file.
+for ex:
+`{'agi-builder-meetup.pdf': "2/26/24, 2:16 PM\nAGI Builders Meetup SF · Luma\nContact the HostReport Event29\nEvent FullIf youʼd like"}`
+
 ## Contributing
 
 DataFog is a community-driven **open-source** platform and we've been fortunate to have a small and growing contributor base. We'd love to hear ideas, feedback, suggestions for improvement - anything on your mind about what you think can be done to make DataFog better! Join our [Discord](https://discord.gg/bzDth394R4) and join our growing community.
 
 ### Dev Notes
 
 - Justfile commands:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datafog Version: 2.4.0b4 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.0.0b1 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: DataFog Author-
 email: hi@datafog.ai Maintainer: DataFog Maintainer-email: hi@datafog.ai
 License: MIT Project-URL: Homepage, https://datafog.ai Project-URL:
 Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
@@ -19,67 +19,68 @@
 Requires-Dist: en_spacy_pii_fast
                                 _[_D_a_t_a_F_o_g_ _l_o_g_o_]
                OOppeenn--ssoouurrccee DDeevvSSeeccOOppss ffoorr GGeenneerraattiivvee AAII SSyysstteemmss.
   _[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _p_y_v_e_r_s_i_o_n_s_]_[_G_i_t_H_u_b_ _s_t_a_r_s_]_[_P_y_P_i_ _d_o_w_n_l_o_a_d_s_]_[_D_i_s_c_o_r_d_]_[_C_o_d_e
                      _s_t_y_l_e_:_ _b_l_a_c_k_]_[_c_o_d_e_c_o_v_]_[_G_i_t_H_u_b_ _I_s_s_u_e_s_]
 ## Overview ### What is DataFog? DataFog is an open-source DevSecOps platform
 that lets you scan and redact Personally Identifiable Information (PII) out of
-your Generative AI applications. ### What problem are we solving? **Context**
-The primary use case today is Retrieval Augmented Generation (RAG) systems. As
-a refresher, RAG systems operate by retrieving information from a custom
-knowledge baseâconstructed by you or your teamâand leverage this
-information, either by directly citing the files in a response or inferred
-through the model's responses. This knowledge base is assembled through a
-deliberate process, which involves uploading files into a workflow. These files
-are then segmented into logical information blocks and tagged according to
-their contextual significance. There are a thousand ways to add nuance to this
-characterization, but this suffices for the vast majority of cases! **Problem**
+your Generative AI applications. ### Core Problem ![image](https://github.com/
+DataFog/datafog-python/assets/61345237/57fba4e5-21cc-458f-ac6a-6fbbb70a8de1)
 How do you keep: - Customer PII - Employee PII - Sensitive company information
 pertaining to org changes or restructurings - Pending M&A activity -
 Conversations with external counsel on material corporate matters (i.e. product
 recall, etc) - and more from entering a Generative AI environment in the first
 place? What you need is a tool to scan and redact your RAG-bound documents
-based on your organization or team needs. That's where DataFog comes in. Our
-solution to this problem is through two major approaches: **PII Observability**
-Take in your batch/streaming data and return a scan indicating character-level
-detection of entities **Privacy Filter** DataFog can slot in as a pre-processor
-that redacts PII from your files before they get uploaded to a RAG database
-With this SDK, you can import it into a Python environment (like a Google Colab
-notebook, check out our [Getting Started](examples/getting-started.ipynb)) and
-within a few lines of code you're up and running. ### How it works [DataFog
-Overview]### There's lots of PII tools out there; why DataFog? If you look at
-the landscape of PII detection tools, their very existence was in many cases
-driven by regulatory requirements (i.e. 'comply with CCPA/GDPR/HIPAA'). In this
-scenario, there's a very defined problem, a specific set of immutable entities
-to look for, and a relatively static universe of document schema to work with.
-What that means as an end-result is that the products are purpose-built for the
-problem that they are solving. However, Generative AI changes how we think
-about privacy. There's now a changing set of privacy requirements (new M&A
-deals, internal discussions means new terms to scan/redact) as well as
-different and varying document sources to contend with. PII detection is no
-longer just about compliance, it's an active - and for some, new - internal
-security threat for CISOs and Eng Leaders to contend with. We want DataFog to
-be built and driven to meet the needs of the open-source community as they
-tackle this challenge. ## Installation DataFog can be installed via pip:
-```bash pip install datafog ``` and in your python environment: ``` from
-datafog import PresidioEngine as presidio ``` ## Examples Here are some
-examples of datafog being used to redact information in business contexts.
+based on your organization or team needs. **That's where DataFog comes in.**
+### How it works ![image](https://github.com/DataFog/datafog-python/assets/
+61345237/91f4634a-8a9f-4621-81bc-09930feda78a) ### There's lots of PII tools
+out there; why DataFog? If you look at the landscape of PII detection tools,
+their very existence was in many cases driven by regulatory requirements (i.e.
+'comply with CCPA/GDPR/HIPAA'). In this scenario, there's a very defined
+problem, a specific set of immutable entities to look for, and a relatively
+static universe of document schema to work with. What that means as an end-
+result is that the products are purpose-built for the problem that they are
+solving. However, Generative AI changes how we think about privacy. There's now
+a changing set of privacy requirements (new M&A deals, internal discussions
+means new terms to scan/redact) as well as different and varying document
+sources to contend with. PII detection is no longer just about compliance, it's
+an active - and for some, new - internal security threat for CISOs and Eng
+Leaders to contend with. We want DataFog to be built and driven to meet the
+needs of the open-source community as they tackle this challenge. ### Roadmap
+DataFog is an active project with regular weekly releases to production
+(typically on/around Monday evenings US PT). Here's a snapshot of our coming
+roadmap; if you have questions or would like to weigh in, join our discord and
+let us know what we can do to make the product better! ![image](https://
+github.com/DataFog/datafog-python/assets/61345237/62964d22-a221-4f1d-a0e6-
+0cc99de2ba92) ## Installation DataFog can be installed via pip: ```bash pip
+install datafog ``` and in your python environment: ``` from datafog import
+PresidioEngine as presidio datafog = datafog.DataFog() ``` ## Examples Here are
+some examples of datafog being used to redact information in business contexts.
 Please see '/examples' for our [Getting Started](examples/getting-
 started.ipynb) notebook. We'll be regularly updating content and providing
 comprehensive guides to using DataFog in production contexts. If you have any
 ideas for a tutorial or guide that you would like to see, please let us know!
-``` ceo_email_chunk = "I'm announcing on Friday that Jeff is going to be CTO."
-scan_results1 = presidio.scan(ceo_email_chunk) print("PII Detected - base case:
-", scan_results1) # PII Detected - base case: [type: PERSON, start: 30, end:
-34, score: 0.85] scan_results2 = presidio.scan(ceo_email_chunk, deny_list=
-['CTO']) print("PII Detected with deny list:", scan_results2) # PII Detected
-with deny list: [type: CUSTOM_PII, start: 50, end: 53, score: 1.0, type:
-PERSON, start: 30, end: 34, score: 0.85] ``` ## Contributing DataFog is a
-community-driven **open-source** platform and we've been fortunate to have a
-small and growing contributor base. We'd love to hear ideas, feedback,
-suggestions for improvement - anything on your mind about what you think can be
-done to make DataFog better! Join our [Discord](https://discord.gg/bzDth394R4)
-and join our growing community. ### Dev Notes - Justfile commands: - `just
-format` to apply formatting. - `just lint` to check formatting and style. ###
-Testing To run the datafog unit tests, check out this repository and do ``` tox
-``` ## License This software is published under the [MIT license](https://
-en.wikipedia.org/wiki/MIT_License).
+### Scanning a single string ``` ceo_email_chunk = "I'm announcing on Friday
+that Jeff is going to be CTO." scan_results1 = presidio.scan(ceo_email_chunk)
+print("PII Detected - base case:", scan_results1) # PII Detected - base case:
+[type: PERSON, start: 30, end: 34, score: 0.85] scan_results2 = presidio.scan
+(ceo_email_chunk, deny_list=['CTO']) print("PII Detected with deny list:",
+scan_results2) # PII Detected with deny list: [type: CUSTOM_PII, start: 50,
+end: 53, score: 1.0, type: PERSON, start: 30, end: 34, score: 0.85] ``` ###
+Scanning a list of PDFs ``` file_dir = ["/Users/sidmohan/Desktop/datafog-
+v2.4.0/datafog-python/tests/files/input_files/agi-builder-meetup.pdf", "/Users/
+sidmohan/Desktop/datafog-v2.4.0/datafog-python/tests/files/input_files/pypdf-
+readthedocs-io-en-stable.pdf"] datafog = datafog.DataFog() result =
+datafog.upload_files(uploaded_files=file_dir) print(result) ``` The output here
+will be a dictionary where the keys are the file names and the values are the
+scan results for that file. for ex: `{'agi-builder-meetup.pdf': "2/26/24, 2:16
+PM\nAGI Builders Meetup SF Â· Luma\nContact the HostReport Event29\nEvent
+FullIf youÊ¼d like"}` ## Contributing DataFog is a community-driven **open-
+source** platform and we've been fortunate to have a small and growing
+contributor base. We'd love to hear ideas, feedback, suggestions for
+improvement - anything on your mind about what you think can be done to make
+DataFog better! Join our [Discord](https://discord.gg/bzDth394R4) and join our
+growing community. ### Dev Notes - Justfile commands: - `just format` to apply
+formatting. - `just lint` to check formatting and style. ### Testing To run the
+datafog unit tests, check out this repository and do ``` tox ``` ## License
+This software is published under the [MIT license](https://en.wikipedia.org/
+wiki/MIT_License).
```

### Comparing `datafog-2.4.0b4/README.md` & `datafog-3.0.0b1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -19,84 +19,102 @@
 
 ## Overview
 
 ### What is DataFog?
 
 DataFog is an open-source DevSecOps platform that lets you scan and redact Personally Identifiable Information (PII) out of your Generative AI applications.
 
-### What problem are we solving?
+### Core Problem
 
-**Context**
+![image](https://github.com/DataFog/datafog-python/assets/61345237/57fba4e5-21cc-458f-ac6a-6fbbb70a8de1)
 
-The primary use case today is Retrieval Augmented Generation (RAG) systems. As a refresher, RAG systems operate by retrieving information from a custom knowledge base—constructed by you or your team—and leverage this information, either by directly citing the files in a response or inferred through the model's responses. This knowledge base is assembled through a deliberate process, which involves uploading files into a workflow. These files are then segmented into logical information blocks and tagged according to their contextual significance. There are a thousand ways to add nuance to this characterization, but this suffices for the vast majority of cases!
-
-**Problem**
 
 How do you keep:
 
 - Customer PII
 - Employee PII
 - Sensitive company information pertaining to org changes or restructurings
 - Pending M&A activity
 - Conversations with external counsel on material corporate matters (i.e. product recall, etc)
 - and more
 
 from entering a Generative AI environment in the first place? What you need is a tool to scan and redact your RAG-bound documents based on your organization or team needs.
 
-That's where DataFog comes in. Our solution to this problem is through two major approaches:
-
-**PII Observability** Take in your batch/streaming data and return a scan indicating character-level detection of entities
-**Privacy Filter** DataFog can slot in as a pre-processor that redacts PII from your files before they get uploaded to a RAG database
-
-With this SDK, you can import it into a Python environment (like a Google Colab notebook, check out our [Getting Started](examples/getting-started.ipynb)) and within a few lines of code you're up and running.
+**That's where DataFog comes in.**
 
 ### How it works
 
-<img src="https://www.datafog.ai/hero.png" alt="DataFog Overview" style="width:50%;">
+![image](https://github.com/DataFog/datafog-python/assets/61345237/91f4634a-8a9f-4621-81bc-09930feda78a)
+
 
 ### There's lots of PII tools out there; why DataFog?
 
 If you look at the landscape of PII detection tools, their very existence was in many cases driven by regulatory requirements (i.e. 'comply with CCPA/GDPR/HIPAA').
 In this scenario, there's a very defined problem, a specific set of immutable entities to look for, and a relatively static universe of document schema to work with. What that means as an end-result is that the products
 are purpose-built for the problem that they are solving.
 
 However, Generative AI changes how we think about privacy. There's now a changing set of privacy requirements (new M&A deals, internal discussions means new terms to scan/redact) as well as different and varying document sources to contend with. PII detection is no longer just about compliance, it's an active - and for some, new - internal security threat for CISOs and Eng Leaders to contend with. We want DataFog to be built and driven to meet the needs of the open-source community as they tackle this challenge.
 
+### Roadmap
+DataFog is an active project with regular weekly releases to production (typically on/around Monday evenings US PT).  Here's a snapshot of our coming roadmap; if you have questions or would like to weigh in, join our discord and let us know what we can do to make the product better!
+
+![image](https://github.com/DataFog/datafog-python/assets/61345237/62964d22-a221-4f1d-a0e6-0cc99de2ba92)
+
+
+
 ## Installation
 
 DataFog can be installed via pip:
 
 ```bash
 pip install datafog
 ```
 
 and in your python environment:
 
 ```
 from datafog import PresidioEngine as presidio
+datafog = datafog.DataFog()
+
 ```
 
 ## Examples
 
 Here are some examples of datafog being used to redact information in business contexts. Please see '/examples' for our [Getting Started](examples/getting-started.ipynb) notebook. We'll be regularly updating content and providing comprehensive guides to using DataFog in production contexts. If you have any ideas for a tutorial or guide that you would like to see, please let us know!
 
+### Scanning a single string
+
 ```
   ceo_email_chunk = "I'm announcing on Friday that Jeff is going to be CTO."
 
   scan_results1 = presidio.scan(ceo_email_chunk)
   print("PII Detected - base case:", scan_results1)
   # PII Detected - base case: [type: PERSON, start: 30, end: 34, score: 0.85]
 
 
   scan_results2 = presidio.scan(ceo_email_chunk, deny_list=['CTO'])
   print("PII Detected with deny list:", scan_results2)
   # PII Detected with deny list: [type: CUSTOM_PII, start: 50, end: 53, score: 1.0, type: PERSON, start: 30, end: 34, score: 0.85]
 
 ```
 
+### Scanning a list of PDFs
+
+```
+file_dir = ["/Users/sidmohan/Desktop/datafog-v2.4.0/datafog-python/tests/files/input_files/agi-builder-meetup.pdf",
+           "/Users/sidmohan/Desktop/datafog-v2.4.0/datafog-python/tests/files/input_files/pypdf-readthedocs-io-en-stable.pdf"]
+datafog = datafog.DataFog()
+result = datafog.upload_files(uploaded_files=file_dir)
+print(result)
+```
+
+The output here will be a dictionary where the keys are the file names and the values are the scan results for that file.
+for ex:
+`{'agi-builder-meetup.pdf': "2/26/24, 2:16 PM\nAGI Builders Meetup SF · Luma\nContact the HostReport Event29\nEvent FullIf youʼd like"}`
+
 ## Contributing
 
 DataFog is a community-driven **open-source** platform and we've been fortunate to have a small and growing contributor base. We'd love to hear ideas, feedback, suggestions for improvement - anything on your mind about what you think can be done to make DataFog better! Join our [Discord](https://discord.gg/bzDth394R4) and join our growing community.
 
 ### Dev Notes
 
 - Justfile commands:
```

#### html2text {}

```diff
@@ -1,66 +1,67 @@
                                 _[_D_a_t_a_F_o_g_ _l_o_g_o_]
                OOppeenn--ssoouurrccee DDeevvSSeeccOOppss ffoorr GGeenneerraattiivvee AAII SSyysstteemmss.
   _[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _p_y_v_e_r_s_i_o_n_s_]_[_G_i_t_H_u_b_ _s_t_a_r_s_]_[_P_y_P_i_ _d_o_w_n_l_o_a_d_s_]_[_D_i_s_c_o_r_d_]_[_C_o_d_e
                      _s_t_y_l_e_:_ _b_l_a_c_k_]_[_c_o_d_e_c_o_v_]_[_G_i_t_H_u_b_ _I_s_s_u_e_s_]
 ## Overview ### What is DataFog? DataFog is an open-source DevSecOps platform
 that lets you scan and redact Personally Identifiable Information (PII) out of
-your Generative AI applications. ### What problem are we solving? **Context**
-The primary use case today is Retrieval Augmented Generation (RAG) systems. As
-a refresher, RAG systems operate by retrieving information from a custom
-knowledge baseâconstructed by you or your teamâand leverage this
-information, either by directly citing the files in a response or inferred
-through the model's responses. This knowledge base is assembled through a
-deliberate process, which involves uploading files into a workflow. These files
-are then segmented into logical information blocks and tagged according to
-their contextual significance. There are a thousand ways to add nuance to this
-characterization, but this suffices for the vast majority of cases! **Problem**
+your Generative AI applications. ### Core Problem ![image](https://github.com/
+DataFog/datafog-python/assets/61345237/57fba4e5-21cc-458f-ac6a-6fbbb70a8de1)
 How do you keep: - Customer PII - Employee PII - Sensitive company information
 pertaining to org changes or restructurings - Pending M&A activity -
 Conversations with external counsel on material corporate matters (i.e. product
 recall, etc) - and more from entering a Generative AI environment in the first
 place? What you need is a tool to scan and redact your RAG-bound documents
-based on your organization or team needs. That's where DataFog comes in. Our
-solution to this problem is through two major approaches: **PII Observability**
-Take in your batch/streaming data and return a scan indicating character-level
-detection of entities **Privacy Filter** DataFog can slot in as a pre-processor
-that redacts PII from your files before they get uploaded to a RAG database
-With this SDK, you can import it into a Python environment (like a Google Colab
-notebook, check out our [Getting Started](examples/getting-started.ipynb)) and
-within a few lines of code you're up and running. ### How it works [DataFog
-Overview]### There's lots of PII tools out there; why DataFog? If you look at
-the landscape of PII detection tools, their very existence was in many cases
-driven by regulatory requirements (i.e. 'comply with CCPA/GDPR/HIPAA'). In this
-scenario, there's a very defined problem, a specific set of immutable entities
-to look for, and a relatively static universe of document schema to work with.
-What that means as an end-result is that the products are purpose-built for the
-problem that they are solving. However, Generative AI changes how we think
-about privacy. There's now a changing set of privacy requirements (new M&A
-deals, internal discussions means new terms to scan/redact) as well as
-different and varying document sources to contend with. PII detection is no
-longer just about compliance, it's an active - and for some, new - internal
-security threat for CISOs and Eng Leaders to contend with. We want DataFog to
-be built and driven to meet the needs of the open-source community as they
-tackle this challenge. ## Installation DataFog can be installed via pip:
-```bash pip install datafog ``` and in your python environment: ``` from
-datafog import PresidioEngine as presidio ``` ## Examples Here are some
-examples of datafog being used to redact information in business contexts.
+based on your organization or team needs. **That's where DataFog comes in.**
+### How it works ![image](https://github.com/DataFog/datafog-python/assets/
+61345237/91f4634a-8a9f-4621-81bc-09930feda78a) ### There's lots of PII tools
+out there; why DataFog? If you look at the landscape of PII detection tools,
+their very existence was in many cases driven by regulatory requirements (i.e.
+'comply with CCPA/GDPR/HIPAA'). In this scenario, there's a very defined
+problem, a specific set of immutable entities to look for, and a relatively
+static universe of document schema to work with. What that means as an end-
+result is that the products are purpose-built for the problem that they are
+solving. However, Generative AI changes how we think about privacy. There's now
+a changing set of privacy requirements (new M&A deals, internal discussions
+means new terms to scan/redact) as well as different and varying document
+sources to contend with. PII detection is no longer just about compliance, it's
+an active - and for some, new - internal security threat for CISOs and Eng
+Leaders to contend with. We want DataFog to be built and driven to meet the
+needs of the open-source community as they tackle this challenge. ### Roadmap
+DataFog is an active project with regular weekly releases to production
+(typically on/around Monday evenings US PT). Here's a snapshot of our coming
+roadmap; if you have questions or would like to weigh in, join our discord and
+let us know what we can do to make the product better! ![image](https://
+github.com/DataFog/datafog-python/assets/61345237/62964d22-a221-4f1d-a0e6-
+0cc99de2ba92) ## Installation DataFog can be installed via pip: ```bash pip
+install datafog ``` and in your python environment: ``` from datafog import
+PresidioEngine as presidio datafog = datafog.DataFog() ``` ## Examples Here are
+some examples of datafog being used to redact information in business contexts.
 Please see '/examples' for our [Getting Started](examples/getting-
 started.ipynb) notebook. We'll be regularly updating content and providing
 comprehensive guides to using DataFog in production contexts. If you have any
 ideas for a tutorial or guide that you would like to see, please let us know!
-``` ceo_email_chunk = "I'm announcing on Friday that Jeff is going to be CTO."
-scan_results1 = presidio.scan(ceo_email_chunk) print("PII Detected - base case:
-", scan_results1) # PII Detected - base case: [type: PERSON, start: 30, end:
-34, score: 0.85] scan_results2 = presidio.scan(ceo_email_chunk, deny_list=
-['CTO']) print("PII Detected with deny list:", scan_results2) # PII Detected
-with deny list: [type: CUSTOM_PII, start: 50, end: 53, score: 1.0, type:
-PERSON, start: 30, end: 34, score: 0.85] ``` ## Contributing DataFog is a
-community-driven **open-source** platform and we've been fortunate to have a
-small and growing contributor base. We'd love to hear ideas, feedback,
-suggestions for improvement - anything on your mind about what you think can be
-done to make DataFog better! Join our [Discord](https://discord.gg/bzDth394R4)
-and join our growing community. ### Dev Notes - Justfile commands: - `just
-format` to apply formatting. - `just lint` to check formatting and style. ###
-Testing To run the datafog unit tests, check out this repository and do ``` tox
-``` ## License This software is published under the [MIT license](https://
-en.wikipedia.org/wiki/MIT_License).
+### Scanning a single string ``` ceo_email_chunk = "I'm announcing on Friday
+that Jeff is going to be CTO." scan_results1 = presidio.scan(ceo_email_chunk)
+print("PII Detected - base case:", scan_results1) # PII Detected - base case:
+[type: PERSON, start: 30, end: 34, score: 0.85] scan_results2 = presidio.scan
+(ceo_email_chunk, deny_list=['CTO']) print("PII Detected with deny list:",
+scan_results2) # PII Detected with deny list: [type: CUSTOM_PII, start: 50,
+end: 53, score: 1.0, type: PERSON, start: 30, end: 34, score: 0.85] ``` ###
+Scanning a list of PDFs ``` file_dir = ["/Users/sidmohan/Desktop/datafog-
+v2.4.0/datafog-python/tests/files/input_files/agi-builder-meetup.pdf", "/Users/
+sidmohan/Desktop/datafog-v2.4.0/datafog-python/tests/files/input_files/pypdf-
+readthedocs-io-en-stable.pdf"] datafog = datafog.DataFog() result =
+datafog.upload_files(uploaded_files=file_dir) print(result) ``` The output here
+will be a dictionary where the keys are the file names and the values are the
+scan results for that file. for ex: `{'agi-builder-meetup.pdf': "2/26/24, 2:16
+PM\nAGI Builders Meetup SF Â· Luma\nContact the HostReport Event29\nEvent
+FullIf youÊ¼d like"}` ## Contributing DataFog is a community-driven **open-
+source** platform and we've been fortunate to have a small and growing
+contributor base. We'd love to hear ideas, feedback, suggestions for
+improvement - anything on your mind about what you think can be done to make
+DataFog better! Join our [Discord](https://discord.gg/bzDth394R4) and join our
+growing community. ### Dev Notes - Justfile commands: - `just format` to apply
+formatting. - `just lint` to check formatting and style. ### Testing To run the
+datafog unit tests, check out this repository and do ``` tox ``` ## License
+This software is published under the [MIT license](https://en.wikipedia.org/
+wiki/MIT_License).
```

### Comparing `datafog-2.4.0b4/setup.py` & `datafog-3.0.0b1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read README for the long description
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 def __version__():
-    return "2.4.0b4"
+    return "3.0.0-beta.1"
 
 
 project_urls = {
     "Homepage": "https://datafog.ai",
     "Documentation": "https://docs.datafog.ai",
     "Discord": "https://discord.gg/bzDth394R4",
     "Twitter": "https://twitter.com/datafoginc",
```

### Comparing `datafog-2.4.0b4/src/datafog.egg-info/PKG-INFO` & `datafog-3.0.0b1/src/datafog.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 2.4.0b4
+Version: 3.0.0b1
 Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
 Home-page: https://datafog.ai
 Author: DataFog
 Author-email: hi@datafog.ai
 Maintainer: DataFog
 Maintainer-email: hi@datafog.ai
 License: MIT
@@ -55,84 +55,102 @@
 
 ## Overview
 
 ### What is DataFog?
 
 DataFog is an open-source DevSecOps platform that lets you scan and redact Personally Identifiable Information (PII) out of your Generative AI applications.
 
-### What problem are we solving?
+### Core Problem
 
-**Context**
+![image](https://github.com/DataFog/datafog-python/assets/61345237/57fba4e5-21cc-458f-ac6a-6fbbb70a8de1)
 
-The primary use case today is Retrieval Augmented Generation (RAG) systems. As a refresher, RAG systems operate by retrieving information from a custom knowledge base—constructed by you or your team—and leverage this information, either by directly citing the files in a response or inferred through the model's responses. This knowledge base is assembled through a deliberate process, which involves uploading files into a workflow. These files are then segmented into logical information blocks and tagged according to their contextual significance. There are a thousand ways to add nuance to this characterization, but this suffices for the vast majority of cases!
-
-**Problem**
 
 How do you keep:
 
 - Customer PII
 - Employee PII
 - Sensitive company information pertaining to org changes or restructurings
 - Pending M&A activity
 - Conversations with external counsel on material corporate matters (i.e. product recall, etc)
 - and more
 
 from entering a Generative AI environment in the first place? What you need is a tool to scan and redact your RAG-bound documents based on your organization or team needs.
 
-That's where DataFog comes in. Our solution to this problem is through two major approaches:
-
-**PII Observability** Take in your batch/streaming data and return a scan indicating character-level detection of entities
-**Privacy Filter** DataFog can slot in as a pre-processor that redacts PII from your files before they get uploaded to a RAG database
-
-With this SDK, you can import it into a Python environment (like a Google Colab notebook, check out our [Getting Started](examples/getting-started.ipynb)) and within a few lines of code you're up and running.
+**That's where DataFog comes in.**
 
 ### How it works
 
-<img src="https://www.datafog.ai/hero.png" alt="DataFog Overview" style="width:50%;">
+![image](https://github.com/DataFog/datafog-python/assets/61345237/91f4634a-8a9f-4621-81bc-09930feda78a)
+
 
 ### There's lots of PII tools out there; why DataFog?
 
 If you look at the landscape of PII detection tools, their very existence was in many cases driven by regulatory requirements (i.e. 'comply with CCPA/GDPR/HIPAA').
 In this scenario, there's a very defined problem, a specific set of immutable entities to look for, and a relatively static universe of document schema to work with. What that means as an end-result is that the products
 are purpose-built for the problem that they are solving.
 
 However, Generative AI changes how we think about privacy. There's now a changing set of privacy requirements (new M&A deals, internal discussions means new terms to scan/redact) as well as different and varying document sources to contend with. PII detection is no longer just about compliance, it's an active - and for some, new - internal security threat for CISOs and Eng Leaders to contend with. We want DataFog to be built and driven to meet the needs of the open-source community as they tackle this challenge.
 
+### Roadmap
+DataFog is an active project with regular weekly releases to production (typically on/around Monday evenings US PT).  Here's a snapshot of our coming roadmap; if you have questions or would like to weigh in, join our discord and let us know what we can do to make the product better!
+
+![image](https://github.com/DataFog/datafog-python/assets/61345237/62964d22-a221-4f1d-a0e6-0cc99de2ba92)
+
+
+
 ## Installation
 
 DataFog can be installed via pip:
 
 ```bash
 pip install datafog
 ```
 
 and in your python environment:
 
 ```
 from datafog import PresidioEngine as presidio
+datafog = datafog.DataFog()
+
 ```
 
 ## Examples
 
 Here are some examples of datafog being used to redact information in business contexts. Please see '/examples' for our [Getting Started](examples/getting-started.ipynb) notebook. We'll be regularly updating content and providing comprehensive guides to using DataFog in production contexts. If you have any ideas for a tutorial or guide that you would like to see, please let us know!
 
+### Scanning a single string
+
 ```
   ceo_email_chunk = "I'm announcing on Friday that Jeff is going to be CTO."
 
   scan_results1 = presidio.scan(ceo_email_chunk)
   print("PII Detected - base case:", scan_results1)
   # PII Detected - base case: [type: PERSON, start: 30, end: 34, score: 0.85]
 
 
   scan_results2 = presidio.scan(ceo_email_chunk, deny_list=['CTO'])
   print("PII Detected with deny list:", scan_results2)
   # PII Detected with deny list: [type: CUSTOM_PII, start: 50, end: 53, score: 1.0, type: PERSON, start: 30, end: 34, score: 0.85]
 
 ```
 
+### Scanning a list of PDFs
+
+```
+file_dir = ["/Users/sidmohan/Desktop/datafog-v2.4.0/datafog-python/tests/files/input_files/agi-builder-meetup.pdf",
+           "/Users/sidmohan/Desktop/datafog-v2.4.0/datafog-python/tests/files/input_files/pypdf-readthedocs-io-en-stable.pdf"]
+datafog = datafog.DataFog()
+result = datafog.upload_files(uploaded_files=file_dir)
+print(result)
+```
+
+The output here will be a dictionary where the keys are the file names and the values are the scan results for that file.
+for ex:
+`{'agi-builder-meetup.pdf': "2/26/24, 2:16 PM\nAGI Builders Meetup SF · Luma\nContact the HostReport Event29\nEvent FullIf youʼd like"}`
+
 ## Contributing
 
 DataFog is a community-driven **open-source** platform and we've been fortunate to have a small and growing contributor base. We'd love to hear ideas, feedback, suggestions for improvement - anything on your mind about what you think can be done to make DataFog better! Join our [Discord](https://discord.gg/bzDth394R4) and join our growing community.
 
 ### Dev Notes
 
 - Justfile commands:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datafog Version: 2.4.0b4 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.0.0b1 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: DataFog Author-
 email: hi@datafog.ai Maintainer: DataFog Maintainer-email: hi@datafog.ai
 License: MIT Project-URL: Homepage, https://datafog.ai Project-URL:
 Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
@@ -19,67 +19,68 @@
 Requires-Dist: en_spacy_pii_fast
                                 _[_D_a_t_a_F_o_g_ _l_o_g_o_]
                OOppeenn--ssoouurrccee DDeevvSSeeccOOppss ffoorr GGeenneerraattiivvee AAII SSyysstteemmss.
   _[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _p_y_v_e_r_s_i_o_n_s_]_[_G_i_t_H_u_b_ _s_t_a_r_s_]_[_P_y_P_i_ _d_o_w_n_l_o_a_d_s_]_[_D_i_s_c_o_r_d_]_[_C_o_d_e
                      _s_t_y_l_e_:_ _b_l_a_c_k_]_[_c_o_d_e_c_o_v_]_[_G_i_t_H_u_b_ _I_s_s_u_e_s_]
 ## Overview ### What is DataFog? DataFog is an open-source DevSecOps platform
 that lets you scan and redact Personally Identifiable Information (PII) out of
-your Generative AI applications. ### What problem are we solving? **Context**
-The primary use case today is Retrieval Augmented Generation (RAG) systems. As
-a refresher, RAG systems operate by retrieving information from a custom
-knowledge baseâconstructed by you or your teamâand leverage this
-information, either by directly citing the files in a response or inferred
-through the model's responses. This knowledge base is assembled through a
-deliberate process, which involves uploading files into a workflow. These files
-are then segmented into logical information blocks and tagged according to
-their contextual significance. There are a thousand ways to add nuance to this
-characterization, but this suffices for the vast majority of cases! **Problem**
+your Generative AI applications. ### Core Problem ![image](https://github.com/
+DataFog/datafog-python/assets/61345237/57fba4e5-21cc-458f-ac6a-6fbbb70a8de1)
 How do you keep: - Customer PII - Employee PII - Sensitive company information
 pertaining to org changes or restructurings - Pending M&A activity -
 Conversations with external counsel on material corporate matters (i.e. product
 recall, etc) - and more from entering a Generative AI environment in the first
 place? What you need is a tool to scan and redact your RAG-bound documents
-based on your organization or team needs. That's where DataFog comes in. Our
-solution to this problem is through two major approaches: **PII Observability**
-Take in your batch/streaming data and return a scan indicating character-level
-detection of entities **Privacy Filter** DataFog can slot in as a pre-processor
-that redacts PII from your files before they get uploaded to a RAG database
-With this SDK, you can import it into a Python environment (like a Google Colab
-notebook, check out our [Getting Started](examples/getting-started.ipynb)) and
-within a few lines of code you're up and running. ### How it works [DataFog
-Overview]### There's lots of PII tools out there; why DataFog? If you look at
-the landscape of PII detection tools, their very existence was in many cases
-driven by regulatory requirements (i.e. 'comply with CCPA/GDPR/HIPAA'). In this
-scenario, there's a very defined problem, a specific set of immutable entities
-to look for, and a relatively static universe of document schema to work with.
-What that means as an end-result is that the products are purpose-built for the
-problem that they are solving. However, Generative AI changes how we think
-about privacy. There's now a changing set of privacy requirements (new M&A
-deals, internal discussions means new terms to scan/redact) as well as
-different and varying document sources to contend with. PII detection is no
-longer just about compliance, it's an active - and for some, new - internal
-security threat for CISOs and Eng Leaders to contend with. We want DataFog to
-be built and driven to meet the needs of the open-source community as they
-tackle this challenge. ## Installation DataFog can be installed via pip:
-```bash pip install datafog ``` and in your python environment: ``` from
-datafog import PresidioEngine as presidio ``` ## Examples Here are some
-examples of datafog being used to redact information in business contexts.
+based on your organization or team needs. **That's where DataFog comes in.**
+### How it works ![image](https://github.com/DataFog/datafog-python/assets/
+61345237/91f4634a-8a9f-4621-81bc-09930feda78a) ### There's lots of PII tools
+out there; why DataFog? If you look at the landscape of PII detection tools,
+their very existence was in many cases driven by regulatory requirements (i.e.
+'comply with CCPA/GDPR/HIPAA'). In this scenario, there's a very defined
+problem, a specific set of immutable entities to look for, and a relatively
+static universe of document schema to work with. What that means as an end-
+result is that the products are purpose-built for the problem that they are
+solving. However, Generative AI changes how we think about privacy. There's now
+a changing set of privacy requirements (new M&A deals, internal discussions
+means new terms to scan/redact) as well as different and varying document
+sources to contend with. PII detection is no longer just about compliance, it's
+an active - and for some, new - internal security threat for CISOs and Eng
+Leaders to contend with. We want DataFog to be built and driven to meet the
+needs of the open-source community as they tackle this challenge. ### Roadmap
+DataFog is an active project with regular weekly releases to production
+(typically on/around Monday evenings US PT). Here's a snapshot of our coming
+roadmap; if you have questions or would like to weigh in, join our discord and
+let us know what we can do to make the product better! ![image](https://
+github.com/DataFog/datafog-python/assets/61345237/62964d22-a221-4f1d-a0e6-
+0cc99de2ba92) ## Installation DataFog can be installed via pip: ```bash pip
+install datafog ``` and in your python environment: ``` from datafog import
+PresidioEngine as presidio datafog = datafog.DataFog() ``` ## Examples Here are
+some examples of datafog being used to redact information in business contexts.
 Please see '/examples' for our [Getting Started](examples/getting-
 started.ipynb) notebook. We'll be regularly updating content and providing
 comprehensive guides to using DataFog in production contexts. If you have any
 ideas for a tutorial or guide that you would like to see, please let us know!
-``` ceo_email_chunk = "I'm announcing on Friday that Jeff is going to be CTO."
-scan_results1 = presidio.scan(ceo_email_chunk) print("PII Detected - base case:
-", scan_results1) # PII Detected - base case: [type: PERSON, start: 30, end:
-34, score: 0.85] scan_results2 = presidio.scan(ceo_email_chunk, deny_list=
-['CTO']) print("PII Detected with deny list:", scan_results2) # PII Detected
-with deny list: [type: CUSTOM_PII, start: 50, end: 53, score: 1.0, type:
-PERSON, start: 30, end: 34, score: 0.85] ``` ## Contributing DataFog is a
-community-driven **open-source** platform and we've been fortunate to have a
-small and growing contributor base. We'd love to hear ideas, feedback,
-suggestions for improvement - anything on your mind about what you think can be
-done to make DataFog better! Join our [Discord](https://discord.gg/bzDth394R4)
-and join our growing community. ### Dev Notes - Justfile commands: - `just
-format` to apply formatting. - `just lint` to check formatting and style. ###
-Testing To run the datafog unit tests, check out this repository and do ``` tox
-``` ## License This software is published under the [MIT license](https://
-en.wikipedia.org/wiki/MIT_License).
+### Scanning a single string ``` ceo_email_chunk = "I'm announcing on Friday
+that Jeff is going to be CTO." scan_results1 = presidio.scan(ceo_email_chunk)
+print("PII Detected - base case:", scan_results1) # PII Detected - base case:
+[type: PERSON, start: 30, end: 34, score: 0.85] scan_results2 = presidio.scan
+(ceo_email_chunk, deny_list=['CTO']) print("PII Detected with deny list:",
+scan_results2) # PII Detected with deny list: [type: CUSTOM_PII, start: 50,
+end: 53, score: 1.0, type: PERSON, start: 30, end: 34, score: 0.85] ``` ###
+Scanning a list of PDFs ``` file_dir = ["/Users/sidmohan/Desktop/datafog-
+v2.4.0/datafog-python/tests/files/input_files/agi-builder-meetup.pdf", "/Users/
+sidmohan/Desktop/datafog-v2.4.0/datafog-python/tests/files/input_files/pypdf-
+readthedocs-io-en-stable.pdf"] datafog = datafog.DataFog() result =
+datafog.upload_files(uploaded_files=file_dir) print(result) ``` The output here
+will be a dictionary where the keys are the file names and the values are the
+scan results for that file. for ex: `{'agi-builder-meetup.pdf': "2/26/24, 2:16
+PM\nAGI Builders Meetup SF Â· Luma\nContact the HostReport Event29\nEvent
+FullIf youÊ¼d like"}` ## Contributing DataFog is a community-driven **open-
+source** platform and we've been fortunate to have a small and growing
+contributor base. We'd love to hear ideas, feedback, suggestions for
+improvement - anything on your mind about what you think can be done to make
+DataFog better! Join our [Discord](https://discord.gg/bzDth394R4) and join our
+growing community. ### Dev Notes - Justfile commands: - `just format` to apply
+formatting. - `just lint` to check formatting and style. ### Testing To run the
+datafog unit tests, check out this repository and do ``` tox ``` ## License
+This software is published under the [MIT license](https://en.wikipedia.org/
+wiki/MIT_License).
```


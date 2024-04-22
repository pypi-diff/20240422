# Comparing `tmp/msg2po-1.1.9.tar.gz` & `tmp/msg2po-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msg2po-1.1.9.tar", max compression
+gzip compressed data, was "msg2po-1.2.0.tar", max compression
```

## Comparing `msg2po-1.1.9.tar` & `msg2po-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     1428 2023-02-23 18:25:08.757121 msg2po-1.1.9/README.md
--rw-r--r--   0        0        0        0 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/__init__.py
--rwxr-xr-x   0        0        0     1617 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/bgforge_config.py
--rw-r--r--   0        0        0      511 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/common.py
--rw-r--r--   0        0        0     2033 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/config.py
--rw-r--r--   0        0        0    31400 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/core.py
--rwxr-xr-x   0        0        0      731 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/diff_male_female_po_to_csv.py
--rwxr-xr-x   0        0        0     4016 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/dir2msgstr.py
--rwxr-xr-x   0        0        0     1144 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/female_csv2po.py
--rwxr-xr-x   0        0        0     1374 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/file2msgstr.py
--rwxr-xr-x   0        0        0      731 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/file2po.py
--rwxr-xr-x   0        0        0     1756 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/lowercase.py
--rwxr-xr-x   0        0        0     2447 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/msgmerge.py
--rwxr-xr-x   0        0        0      892 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/po2file.py
--rwxr-xr-x   0        0        0     4477 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/poify.py
--rwxr-xr-x   0        0        0      662 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/resave_po.py
--rwxr-xr-x   0        0        0     2199 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/unfuzzy.py
--rw-r--r--   0        0        0     1336 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/unfuzzy.yml
--rwxr-xr-x   0        0        0     1122 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/unfuzzy_cassidy.py
--rwxr-xr-x   0        0        0     2272 2023-02-23 18:25:08.757121 msg2po-1.1.9/msg2po/unpoify.py
--rw-r--r--   0        0        0     1155 2023-02-23 18:25:08.757121 msg2po-1.1.9/pyproject.toml
--rw-r--r--   0        0        0     2834 1970-01-01 00:00:00.000000 msg2po-1.1.9/setup.py
--rw-r--r--   0        0        0     2351 1970-01-01 00:00:00.000000 msg2po-1.1.9/PKG-INFO
+-rw-r--r--   0        0        0     2038 2024-04-22 04:13:33.754976 msg2po-1.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/__init__.py
+-rwxr-xr-x   0        0        0     1623 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/bgforge_config.py
+-rw-r--r--   0        0        0      511 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/common.py
+-rw-r--r--   0        0        0     2364 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/config.py
+-rw-r--r--   0        0        0    32070 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/core.py
+-rwxr-xr-x   0        0        0      746 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/diff_male_female_po_to_csv.py
+-rwxr-xr-x   0        0        0     4017 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/dir2msgstr.py
+-rwxr-xr-x   0        0        0     1162 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/female_csv2po.py
+-rwxr-xr-x   0        0        0     1334 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/file2msgstr.py
+-rwxr-xr-x   0        0        0      731 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/file2po.py
+-rwxr-xr-x   0        0        0     1756 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/lowercase.py
+-rwxr-xr-x   0        0        0     2447 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/msgmerge.py
+-rwxr-xr-x   0        0        0      892 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/po2file.py
+-rwxr-xr-x   0        0        0     4659 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/poify.py
+-rwxr-xr-x   0        0        0      702 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/resave_po.py
+-rwxr-xr-x   0        0        0     2193 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/unfuzzy.py
+-rw-r--r--   0        0        0     1336 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/unfuzzy.yml
+-rwxr-xr-x   0        0        0     1122 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/unfuzzy_cassidy.py
+-rwxr-xr-x   0        0        0     2272 2024-04-22 04:13:33.754976 msg2po-1.2.0/msg2po/unpoify.py
+-rw-r--r--   0        0        0     1218 2024-04-22 04:13:33.754976 msg2po-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2961 1970-01-01 00:00:00.000000 msg2po-1.2.0/PKG-INFO
```

### Comparing `msg2po-1.1.9/msg2po/config.py` & `msg2po-1.2.0/msg2po/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import ruamel.yaml
 import sys
 import os
 
-VERSION = "1.1.9"
+VERSION = "1.2.0"
 
 
 class Config:
     def __init__(self):
         yml = ".bgforge.yml"
         translation_defaults = {
             "encoding": "cp1252",
@@ -14,19 +14,23 @@
             "src_lang": "english",
             "simple_languages": True,  # extract into language name, not language code. pt_BR.po -> portuguese/1.msg
             "skip_files": [],
             "extract_format": "",  # could be 'sfall'
             "no_female": False,  # explicitly disable female extraction (TODO: reason unclear)
             "extract_fuzzy": False,
             "lowercase": True,
+            # work with all files in utf-8
+            "all_utf8": False,
+            # and even console files (DOS_FILENAMES)
+            "all_utf8_yes_really_all": False,
         }
 
         config = translation_defaults
         try:
-            with open(yml) as yf:
+            with open(yml, encoding="utf-8") as yf:
                 yaml = ruamel.yaml.YAML()
                 config = yaml.load(yf)
             translation_config = {**translation_defaults, **config["translation"]}
         except:
             print(yml + " not found, assuming defaults", file=sys.stderr)
             translation_config = translation_defaults
         config["translation"] = translation_config
@@ -37,14 +41,16 @@
         self.src_lang = translation_config["src_lang"]
         self.simple_languages = translation_config["simple_languages"]
         self.skip_files = translation_config["skip_files"]
         self.extract_format = translation_config["extract_format"]
         self.no_female = translation_config["no_female"]
         self.extract_fuzzy = translation_config["extract_fuzzy"]
         self.lowercase = translation_config["lowercase"]
+        self.all_utf8 = translation_config["all_utf8"]
+        self.all_utf8_yes_really_all = translation_config["all_utf8_yes_really_all"]
 
         self.po_dirname = "po"
         self.female_dir_suffix = "_female"
         self.po_dir = os.path.join(self.tra_dir, self.po_dirname)
         self.poify_dir = os.path.join(self.tra_dir, self.src_lang)
         self.version = VERSION
         self.newline_tra = "\r\n"
```

### Comparing `msg2po-1.1.9/msg2po/core.py` & `msg2po-1.2.0/msg2po/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,27 +162,34 @@
         "install.tra",
     ]
 
     UTF_FILENAMES = [
         "ee.tra",
     ]
 
+    if CONFIG.all_utf8_yes_really_all is True:
+        return "utf-8"
+
     encoding = CONFIG.encoding
     lang = language_slug(lang_path)
     filename = basename(file_path)
 
     if lang in ENCODINGS:
         encoding = ENCODINGS[lang]
 
     if filename in DOS_FILENAMES:
         try:
             encoding = DOS_ENCODINGS[lang]
+            return encoding
         except:
             pass
 
+    if CONFIG.all_utf8 is True:
+        return "utf-8"
+
     if filename in UTF_FILENAMES:
         encoding = "utf-8"
 
     utf_name = re.compile(".*_ee.tra$")
     if utf_name.match(filename):
         encoding = "utf-8"
 
@@ -491,25 +498,27 @@
     entries_dict = OrderedDict()
     for e in po:
         for eo in e.occurrences:
             entries_dict[(eo[0], eo[1])] = e
     if female_map is None:
         female_map = female_entries(po)
 
+    # newly added female entries, without PO counterpart
+    new_female_enties = []
+
     for t in trans.entries:
         index = t.index
         value = t.value
         context = t.context
         female_value = t.female
 
         if (value is None) or (value == ""):
             print("WARN: no msgid found for {}:{}, skipping string\n      {}".format(occurence_path, index, value))
             continue
 
-        new_female_enties = []
         if (occurence_path, index) in entries_dict:
             # map entries to occurrences for faster access, part 2
             e: polib.POEntry = entries_dict[(occurence_path, index)]
 
             if female_value:
                 # female entries have no occurences, checking if female translation already present
                 if e.msgid in female_map:
@@ -549,18 +558,26 @@
                     print("  MALE:   {}".format(e.msgstr))
                     print("  FEMALE: {}".format(female_value))
                     fe = polib.POEntry(msgid=e.msgid, msgstr=female_value, msgctxt=CONTEXT_FEMALE)
                     new_female_enties.append(fe)
 
             # translation is the same
             if e.msgstr == value and e.msgctxt == context:
-                print("  translation is the same for {}".format(e.msgid))
+                print("  translation is the same for {}".format(e.occurrences))
                 if "fuzzy" in e.flags:
-                    print("  {}  is fuzzy. Keeping fuzzy flag.".format(e.msgid))
-                continue
+                    if CONFIG.extract_fuzzy:
+                        print("  {}  is fuzzy. Keeping fuzzy flag.".format(e.occurrences))
+                        continue
+                    else:
+                        print(
+                            f"  {e.occurrences} is fuzzy, but extract_fuzzy is not set. "
+                            "Assuming manual translation change to the same value, clearing fuzzy flag."
+                        )
+                else:
+                    continue
 
             # translation is the same as source
             if e.msgid == value and not same:
                 print("INFO: string and new translation are the same for {}. Skipping:".format(e.occurrences))
                 print("   {}".format(e.msgid))
                 continue
 
@@ -577,18 +594,19 @@
             print("INFO: translation update found for {}.".format(e.occurrences))
             print("  Replacing old string with new:")
             print("    ORIG: {}".format(e.msgid))
             print("    OLD:  {}".format(e.msgstr))
             print("    NEW:  {}".format(value))
             e.msgstr = value
             e.msgctxt = context
-            if "fuzzy" in e.flags:
+            if "fuzzy" in e.flags or e.previous_msgid:
                 print("    Unfuzzied entry")
-                e.flags.remove("fuzzy")
                 e.previous_msgid = None
+                if "fuzzy" in e.flags:
+                    e.flags.remove("fuzzy")
 
     # add newly found female entries
     for nfe in new_female_enties:
         po.append(nfe)
 
     return po
```

### Comparing `msg2po-1.1.9/msg2po/diff_male_female_po_to_csv.py` & `msg2po-1.2.0/msg2po/diff_male_female_po_to_csv.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# diffs male vs female PO and saves the result into CSV suitable for BGforge Weblate
+# diffs male vs female PO and saves the result into CSV suitable for BGforge Hive
 # PO files MUST be identical - except for msgstr's (translations)
 
 import polib
 import csv
 import sys
 
 
@@ -17,14 +17,14 @@
 
     for i in range(0, len(male_po) - 1):
         if male_po[i].msgstr != female_po[i].msgstr:
             rows.append([male_po[i].msgid, female_po[i].msgstr])
 
     rows = sorted(rows, key=lambda k: k[0])
 
-    with open(female_csv, "w") as csvfile:
+    with open(female_csv, "w", encoding="utf-8") as csvfile:
         writer = csv.writer(csvfile, quoting=csv.QUOTE_ALL)
         writer.writerows(rows)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `msg2po-1.1.9/msg2po/dir2msgstr.py` & `msg2po-1.2.0/msg2po/dir2msgstr.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                 po = file2msgstr(
                     input_file=full_name,
                     po=po,
                     occurence_path=full_name,
                     encoding=enc,
                     overwrite=overwrite,
                     same=args.same,
-                    female_map=female_map
+                    female_map=female_map,
                 )
     po = po_make_unique(po)
     return po
 
 
 def main():
     if not args.auto and ((args.output_file is None) or (args.file_ext is None)):
```

### Comparing `msg2po-1.1.9/msg2po/female_csv2po.py` & `msg2po-1.2.0/msg2po/female_csv2po.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 parser.add_argument("INPUT_CSV", help="input CSV file")
 parser.add_argument("OUTPUT_PO", help="output PO file")
 args = parser.parse_args()
 
 
 def load_csv(path):
     female_strings = OrderedDict()
-    with open(path, "r") as csvfile:
+    with open(path, "r", encoding="utf-8") as csvfile:
         reader = csv.reader(csvfile)
         for row in reader:
             female_strings[row[0]] = row[1]
     sorted_strings = OrderedDict(sorted(female_strings.items()))
     return sorted_strings
```

### Comparing `msg2po-1.1.9/msg2po/file2msgstr.py` & `msg2po-1.2.0/msg2po/file2msgstr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python3
-# coding: utf-8
 
 import argparse
 from msg2po.core import file2msgstr, CONFIG, VALID_EXTENSIONS
 from polib import pofile
 
 formats = "/".join(VALID_EXTENSIONS)
 parser = argparse.ArgumentParser(
@@ -11,17 +10,15 @@
 )
 parser.add_argument("INPUT_FILE", help="input file")
 parser.add_argument("OUTPUT_FILE", help="output PO file")
 parser.add_argument(
     "--path", dest="path", help="load as filename (PO occurrence). If not specified, defaults to input filename"
 )
 parser.add_argument("-e", dest="encoding", default="cp1252", help="source encoding")
-parser.add_argument(
-    "overwrite", dest="overwrite", default=False, action="store_true", help="overwrite existing msgstr's"
-)
+parser.add_argument("overwrite", default=False, action="store_true", help="overwrite existing msgstr's")
 parser.add_argument(
     "--same",
     dest="same",
     default=False,
     action="store_true",
     help="load translations that are identical to original strings",
 )
```

### Comparing `msg2po-1.1.9/msg2po/file2po.py` & `msg2po-1.2.0/msg2po/file2po.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.1.9/msg2po/lowercase.py` & `msg2po-1.2.0/msg2po/lowercase.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.1.9/msg2po/msgmerge.py` & `msg2po-1.2.0/msg2po/msgmerge.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.1.9/msg2po/po2file.py` & `msg2po-1.2.0/msg2po/po2file.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.1.9/msg2po/poify.py` & `msg2po-1.2.0/msg2po/poify.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,14 +64,19 @@
         for dir_name, subdir_list, file_list in natsort.natsorted(
             os.walk(".", topdown=False, followlinks=True), alg=natsort.PATH
         ):
             subdir_list = natsort.natsorted(subdir_list, alg=natsort.PATH)
             file_list = natsort.natsorted(file_list, alg=natsort.PATH)
             for file_name in file_list:
                 full_name = os.path.join(dir_name, file_name)
+
+                # convert windows paths to linux style, for consistency in POs
+                if os.path.sep == "\\":
+                    full_name = full_name.replace("\\", "/")
+
                 full_name = re.sub("^\./", "", full_name)  # remove trailing './'
 
                 # skip female cuts
                 pretty_dir_name = re.sub("^\./", "", dir_name)
                 if extract_format == "sfall" and pretty_dir_name == "cuts_female":
                     print("{} is in cuts_female. Skipping!".format(full_name))
                     continue
```

### Comparing `msg2po-1.1.9/msg2po/resave_po.py` & `msg2po-1.2.0/msg2po/resave_po.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 import argparse
 from polib import pofile
-from msg2po.core import sort_po, update_female_entries, CONFIG, unfuzzy_exact_matches
+from msg2po.core import sort_po, update_female_entries, CONFIG, unfuzzy_exact_matches, po_make_unique
 
 parser = argparse.ArgumentParser(
     description="Resave PO file using polib API, to correct formatting",
     formatter_class=argparse.ArgumentDefaultsHelpFormatter,
 )
 parser.add_argument("INPUT_FILE", help="PO file to resave")
 args = parser.parse_args()
 
 
 def main():
     po = pofile(args.INPUT_FILE)
     po = update_female_entries(po)
-    po2 = sort_po(po)
-    po2 = unfuzzy_exact_matches(po2)
-    po2.save(args.INPUT_FILE, newline=CONFIG.newline_po)
+    po = po_make_unique(po)
+    po = unfuzzy_exact_matches(po)
+    po = sort_po(po)
+    po.save(args.INPUT_FILE, newline=CONFIG.newline_po)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `msg2po-1.1.9/msg2po/unfuzzy.py` & `msg2po-1.2.0/msg2po/unfuzzy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
 
 import argparse
 from polib import pofile
 import ruamel.yaml
 import os
 from msg2po.core import CONFIG
 
 parser = argparse.ArgumentParser(
-    description="Unmark PO entries as fuzzy,"
-    "if replacing string 1 with string2 in previous msgid results in current msgid",
+    description="Unmark PO entries as fuzzy, "
+    "if replacing string1 with string2 in previous msgid results in current msgid",
     formatter_class=argparse.ArgumentDefaultsHelpFormatter,
 )
 parser.add_argument("INPUT_FILE", help="input PO file")
 parser.add_argument("-w", default=False, dest="WRITE", action="store_true", help="save PO file?")
 args = parser.parse_args()
 
 input_file = args.INPUT_FILE
@@ -22,15 +21,15 @@
 
 
 def load_replacements():
     if os.path.isfile("unfuzzy.yml"):
         yml = "unfuzzy.yml"
     else:
         yml = os.path.join(os.path.dirname(os.path.realpath(__file__)), "unfuzzy.yml")
-    with open(yml) as yf:
+    with open(yml, encoding="utf-8") as yf:
         yaml = ruamel.yaml.YAML()
         replace_list = yaml.load(yf)
     return replace_list
 
 
 def make_replaces(line, replace_list):
     for r in replace_list:
```

### Comparing `msg2po-1.1.9/msg2po/unfuzzy.yml` & `msg2po-1.2.0/msg2po/unfuzzy.yml`

 * *Files identical despite different names*

### Comparing `msg2po-1.1.9/msg2po/unfuzzy_cassidy.py` & `msg2po-1.2.0/msg2po/unfuzzy_cassidy.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.1.9/msg2po/unpoify.py` & `msg2po-1.2.0/msg2po/unpoify.py`

 * *Files identical despite different names*

### Comparing `msg2po-1.1.9/pyproject.toml` & `msg2po-1.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "msg2po"
-version = "1.1.9"
-description = "A set of helper tools to convert Fallout 1/2 MSG and WeiDU TRA into GNU gettext PO and back"
+version = "1.2.0"
+description = "A set of helper tools to convert Fallout 1/2 MSG and WeiDU TRA into GNU gettext PO and back."
 authors = ["BGforge <dev@bgforge.net>"]
 keywords = ["Fallout", "Fallout 2", "Baldur's Gate", "Infinity Engine", "WeiDU"]
 readme = "README.md"
 homepage = "https://github.com/BGforgeNet/msg2po"
 repository = "https://github.com/BGforgeNet/msg2po"
 
 [tool.poetry.dependencies]
 configparser = ">=5.2.0"
 natsort = ">=6.2.1,<7"
 polib = ">=1.1.1"
 python-dateutil = ">=2.8.2"
 "ruamel.yaml" = ">=0.17.21"
-python = ">=3.6.2"
+python = ">=3.8"
 
 [tool.poetry.dev-dependencies]
-black = ">=22.3.0"
-flake8 = ">=4.0.1"
+black = ">=24.4.0"
+flake8 = ">=5.0.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
@@ -31,9 +31,11 @@
 "bgforge-config" = "msg2po.bgforge_config:main"
 "dir2msgstr" = "msg2po.dir2msgstr:main"
 "file2msgstr" = "msg2po.file2msgstr:main"
 "file2po" = "msg2po.file2po:main"
 "lowercase" = "msg2po.lowercase:main"
 "msgmerge-female" = "msg2po.msgmerge:main"
 "po2file" = "msg2po.po2file:main"
+"poify" = "msg2po.poify:main"
 "resave-po" = "msg2po.resave_po:main"
 "unpoify" = "msg2po.unpoify:main"
+"unfuzzy" = "msg2po.unfuzzy:main"
```

### Comparing `msg2po-1.1.9/PKG-INFO` & `msg2po-1.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: msg2po
-Version: 1.1.9
-Summary: A set of helper tools to convert Fallout 1/2 MSG and WeiDU TRA into GNU gettext PO and back
+Version: 1.2.0
+Summary: A set of helper tools to convert Fallout 1/2 MSG and WeiDU TRA into GNU gettext PO and back.
 Home-page: https://github.com/BGforgeNet/msg2po
 Keywords: Fallout,Fallout 2,Baldur's Gate,Infinity Engine,WeiDU
 Author: BGforge
 Author-email: dev@bgforge.net
-Requires-Python: >=3.6.2
+Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: configparser (>=5.2.0)
 Requires-Dist: natsort (>=6.2.1,<7)
 Requires-Dist: polib (>=1.1.1)
 Requires-Dist: python-dateutil (>=2.8.2)
 Requires-Dist: ruamel.yaml (>=0.17.21)
 Project-URL: Repository, https://github.com/BGforgeNet/msg2po
 Description-Content-Type: text/markdown
@@ -27,20 +27,24 @@
 [![Patreon](https://img.shields.io/badge/Patreon-donate-FF424D?logo=Patreon&labelColor=141518)](https://www.patreon.com/BGforge)
 [![Telegram](https://img.shields.io/badge/telegram-join%20%20%20%20%E2%9D%B1%E2%9D%B1%E2%9D%B1-darkorange?logo=telegram)](https://t.me/bgforge)
 [![Discord](https://img.shields.io/discord/420268540700917760?logo=discord&label=discord&color=blue&logoColor=FEE75C)](https://discord.gg/4Yqfggm)
 [![IRC](https://img.shields.io/badge/%23IRC-join%20%20%20%20%E2%9D%B1%E2%9D%B1%E2%9D%B1-darkorange)](https://bgforge.net/irc)
 
 This is a set of tools to convert Fallout 1/2 MSG and WeiDU TRA into GNU gettext PO and back, used in [BGforge Hive](https://hive.bgforge.net/). Ask questions [here](https://forums.bgforge.net/viewforum.php?f=9).
 
-## Installation
+### Installation
+
 ```bash
 pip install msg2po
 ```
 
-## Usage
+Also install [Gettext tools](https://www.gnu.org/software/gettext/), and make sure they are in PATH.
+
+### Poify
+
 ```bash
 $ poify.py -h
 .bgforge.yml not found, assuming defaults
 usage: poify.py [-h] [-e ENC] [DIR]
 
 Poify files in selected directory
 
@@ -48,13 +52,32 @@
   DIR         source language directory (default: ./english)
 
 options:
   -h, --help  show this help message and exit
   -e ENC      source encoding (default: cp1252)
 ```
 
-## Action
+### Action
+
 Github [action](docs/action.md) is available for automatic processing.
 
 ---
+
 [Changelog](docs/changelog.md)
 
+### Unfuzzy
+
+Unfuzzy removes fuzzy flag and previous msgid from PO entries, if after all replacements current msgid and previous msgid match exactly. Usually it is run after spelling changes in source language, to reduce diff noise and avoid extra review burden.
+
+The comparison is case sensitive. The replacements are read from `unfuzzy.yml` in current directory, example:
+
+```yaml
+- ["Nuka Cola", "Nuka-Cola"]
+- ["nuka cola", "Nuka-Cola"]
+```
+
+Run
+
+```bash
+unfuzzy.py -w data/text/po/french.po
+```
+
```


# Comparing `tmp/cs.fstags-20240412.tar.gz` & `tmp/cs.fstags-20240422.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.fstags-20240412.tar", last modified: Fri Apr 12 05:44:48 2024, max compression
+gzip compressed data, was "cs.fstags-20240422.tar", last modified: Mon Apr 22 03:03:32 2024, max compression
```

## Comparing `cs.fstags-20240412.tar` & `cs.fstags-20240422.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:44:48.348170 cs.fstags-20240412/
--rw-rw-r--   0 cameron    (501) cameron    (502)      148 2024-04-12 05:44:16.000000 cs.fstags-20240412/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    37873 2024-04-12 05:44:48.347893 cs.fstags-20240412/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    37084 2024-04-12 05:44:26.000000 cs.fstags-20240412/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:44:48.341050 cs.fstags-20240412/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:44:48.341279 cs.fstags-20240412/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:44:48.345249 cs.fstags-20240412/lib/python/cs/
--rw-rw-r--   0 cameron    (501) cameron    (502)        4 2024-04-12 05:44:16.000000 cs.fstags-20240412/lib/python/cs/fstags.1
--rw-r--r--   0 cameron    (501) cameron    (502)     7052 2024-04-12 05:44:01.000000 cs.fstags-20240412/lib/python/cs/fstags.1.md
--rw-rw-r--   0 cameron    (501) cameron    (502)        4 2024-04-12 05:44:16.000000 cs.fstags-20240412/lib/python/cs/fstags.5
--rw-r--r--   0 cameron    (501) cameron    (502)    17938 2024-04-12 05:44:01.000000 cs.fstags-20240412/lib/python/cs/fstags.5.md
--rw-r--r--   0 cameron    (501) cameron    (502)    72286 2024-04-12 05:44:01.000000 cs.fstags-20240412/lib/python/cs/fstags.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:44:48.347503 cs.fstags-20240412/lib/python/cs.fstags.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    37873 2024-04-12 05:44:47.000000 cs.fstags-20240412/lib/python/cs.fstags.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      424 2024-04-12 05:44:48.000000 cs.fstags-20240412/lib/python/cs.fstags.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 05:44:47.000000 cs.fstags-20240412/lib/python/cs.fstags.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)       42 2024-04-12 05:44:47.000000 cs.fstags-20240412/lib/python/cs.fstags.egg-info/entry_points.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      247 2024-04-12 05:44:48.000000 cs.fstags-20240412/lib/python/cs.fstags.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 05:44:48.000000 cs.fstags-20240412/lib/python/cs.fstags.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    38674 2024-04-12 05:44:46.000000 cs.fstags-20240412/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 05:44:48.348254 cs.fstags-20240412/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 03:03:32.660908 cs.fstags-20240422/
+-rw-rw-r--   0 cameron    (501) cameron    (502)      148 2024-04-22 03:02:53.000000 cs.fstags-20240422/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    37946 2024-04-22 03:03:32.660512 cs.fstags-20240422/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    37157 2024-04-22 03:03:05.000000 cs.fstags-20240422/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 03:03:32.648381 cs.fstags-20240422/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 03:03:32.648738 cs.fstags-20240422/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 03:03:32.656431 cs.fstags-20240422/lib/python/cs/
+-rw-rw-r--   0 cameron    (501) cameron    (502)        4 2024-04-22 03:02:53.000000 cs.fstags-20240422/lib/python/cs/fstags.1
+-rw-r--r--   0 cameron    (501) cameron    (502)     7052 2024-04-22 03:02:37.000000 cs.fstags-20240422/lib/python/cs/fstags.1.md
+-rw-rw-r--   0 cameron    (501) cameron    (502)        4 2024-04-22 03:02:53.000000 cs.fstags-20240422/lib/python/cs/fstags.5
+-rw-r--r--   0 cameron    (501) cameron    (502)    17938 2024-04-22 03:02:37.000000 cs.fstags-20240422/lib/python/cs/fstags.5.md
+-rw-r--r--   0 cameron    (501) cameron    (502)    71175 2024-04-22 03:02:37.000000 cs.fstags-20240422/lib/python/cs/fstags.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 03:03:32.659951 cs.fstags-20240422/lib/python/cs.fstags.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    37946 2024-04-22 03:03:31.000000 cs.fstags-20240422/lib/python/cs.fstags.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      424 2024-04-22 03:03:32.000000 cs.fstags-20240422/lib/python/cs.fstags.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-22 03:03:31.000000 cs.fstags-20240422/lib/python/cs.fstags.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       42 2024-04-22 03:03:32.000000 cs.fstags-20240422/lib/python/cs.fstags.egg-info/entry_points.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      247 2024-04-22 03:03:32.000000 cs.fstags-20240422/lib/python/cs.fstags.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-22 03:03:32.000000 cs.fstags-20240422/lib/python/cs.fstags.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    38747 2024-04-22 03:03:30.000000 cs.fstags-20240422/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-22 03:03:32.661033 cs.fstags-20240422/setup.cfg
```

### Comparing `cs.fstags-20240412/PKG-INFO` & `cs.fstags-20240422/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.fstags
-Version: 20240412
+Version: 20240422
 Summary: Simple filesystem based file tagging and the associated `fstags` command line script.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -15,16 +15,17 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Simple filesystem based file tagging
 and the associated `fstags` command line script.
 
-*Latest release 20240412*:
-Changes to accomodate dropping BaseCommandOptions.runstate.
+*Latest release 20240422*:
+* Bugfix: .fstags files should no longer get Python repr() output for weirdly typed tag values.
+* Some other minor internal updates.
 
 Many basic tasks can be performed with the `fstags` command line utility,
 documented under the `FSTagsCommand` class below.
 
 Why `fstags`?
 By storing the tags in a separate file we:
 * can store tags without modifying a file
@@ -182,16 +183,16 @@
 Walk the file tree from `path`
 searching for files matching the supplied `tag_tests`.
 Yield the matching file paths.
 
 Parameters:
 * `path`: the top of the file tree to walk
 * `tag_tests`: a sequence of `TagBasedTest`s
-* `use_direct_tags`: test the direct_tags if true,
-  otherwise the all_tags.
+* `use_direct_tags`: test the `direct_tags` if true,
+  otherwise the `all_tags`.
   Default: `False`
 
 *Method `FSTags.find_ontology(self, dirpath, ontbase=None)`*:
 Locate an ontology for the directory `dirpath`.
 The optional `ontbase` may override the relative path to the file,
 default is `self.ontology_filepath`.
 Return a `TagOntology` or `None` if not found.
@@ -277,15 +278,17 @@
   otherwise the `all_tags`.
   Default: `False`
 
 ## Class `FSTagsCommand(cs.cmdutils.BaseCommand, cs.tagset.TagsCommandMixin)`
 
 `fstags` main command line utility.
 
-Command line usage:
+Command line implementation.
+
+Usage summary:
 
     Usage: fstags [-o ontology] [-P] subcommand [...]
       -o ontology   Specify the path to an ontology file.
       -P            Physical. Resolve pathnames through symlinks.
                     Default ~/.fstagsrc[general]physical or False.
       Subcommands:
         autotag paths...
@@ -347,23 +350,24 @@
         ln [-finv] srcpath dstpath, ln [-finv] srcpaths... dstdirpath
           POSIX ln(1) equivalent, but also copying the tags:
           link files and their tags into targetdir.
           -f  Force: remove destination if it exists.
           -i  Interactive: fail if the destination exists.
           -n  No remove: fail if the destination exists.
           -v  Verbose: show linked files.
-        ls [-d] [--direct] [-o output_format] [paths...]
+        ls [-dlr] [--direct] [-o output_format] [paths...]
           List files from paths and their tags.
           -d          Treat directories like files, do not recurse.
           --direct    List direct tags instead of all tags.
           -l          Long format.
           -o output_format
                       Use output_format as a Python format string to lay out
                       the listing.
                       Default: {fspath:json} {tags}
+          -r          Recurse into subdirectories.
         mv [-finv] srcpath dstpath, mv [-finv] srcpaths... dstdirpath
           POSIX mv(1) equivalent, but also copying the tags:
           move files and their tags into targetdir.
           -f  Force: remove destination if it exists.
           -i  Interactive: fail if the destination exists.
           -n  No remove: fail if the destination exists.
           -v  Verbose: show moved files.
@@ -409,15 +413,15 @@
           Update extended attributes from tags.
 
 *`FSTagsCommand.Options`*
 
 *Method `FSTagsCommand.apply_opt(self, opt, val)`*:
 Apply command line option.
 
-*Method `FSTagsCommand.cmd_autotag(self, argv, *, upd: cs.upd.Upd, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x1111add80>)`*:
+*Method `FSTagsCommand.cmd_autotag(self, argv, *, upd: cs.upd.Upd, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x10b33df30>)`*:
 Usage: {cmd} paths...
 Tag paths based on rules from the rc file.
 
 *Method `FSTagsCommand.cmd_cp(self, argv)`*:
 Usage: {cmd} [-finv] srcpath dstpath, {cmd} [-finv] srcpaths... dstdirpath
 POSIX cp(1) equivalent, but also copying tags:
 copy files and their tags into targetdir.
@@ -435,27 +439,27 @@
 Edit the direct tagsets of path, default: '.'
 If path is a directory, provide the tags of its entries.
 Otherwise edit just the tags for path.
 -a    List all names in directory edit mode; normally
       names commencing with a dot are omitted.
 -d    Treat directories like files: edit just its tags.
 
-*Method `FSTagsCommand.cmd_export(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x1111add80>)`*:
+*Method `FSTagsCommand.cmd_export(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x10b33df30>)`*:
 Usage: {cmd} [-a] [--direct] path {{tag[=value]|-tag}}...
 Export tags for files from paths matching all the constraints.
 -a        Export all paths, not just those with tags.
 --direct  Export the direct tags instead of the computed tags.
 The output is in the same CSV format as that from "sqltags export",
 with the following columns:
 * unixtime: the file's st_mtime from os.stat.
 * id: empty
 * name: the file path
 * tags: the file's direct or indirect tags
 
-*Method `FSTagsCommand.cmd_find(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x1111add80>)`*:
+*Method `FSTagsCommand.cmd_find(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x10b33df30>)`*:
 Usage: {cmd} [--direct] [--for-rsync] [-o output_format] path {{tag[=value]|-tag}}...
 List files from path matching all the constraints.
 --direct    Use direct tags instead of all tags.
 --for-rsync Instead of listing matching paths, emit a
             sequence of rsync(1) patterns suitable for use with
             --include-from in order to do a selective rsync of the
             matched paths.
@@ -487,24 +491,25 @@
 POSIX ln(1) equivalent, but also copying the tags:
 link files and their tags into targetdir.
 -f  Force: remove destination if it exists.
 -i  Interactive: fail if the destination exists.
 -n  No remove: fail if the destination exists.
 -v  Verbose: show linked files.
 
-*Method `FSTagsCommand.cmd_ls(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x1111add80>)`*:
-Usage: {cmd} [-d] [--direct] [-o output_format] [paths...]
+*Method `FSTagsCommand.cmd_ls(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x10b33df30>)`*:
+Usage: {cmd} [-dlr] [--direct] [-o output_format] [paths...]
 List files from paths and their tags.
 -d          Treat directories like files, do not recurse.
 --direct    List direct tags instead of all tags.
 -l          Long format.
 -o output_format
             Use output_format as a Python format string to lay out
             the listing.
             Default: {LS_OUTPUT_FORMAT_DEFAULT}
+-r          Recurse into subdirectories.
 
 *Method `FSTagsCommand.cmd_mv(self, argv)`*:
 Usage: {cmd} [-finv] srcpath dstpath, {cmd} [-finv] srcpaths... dstdirpath
 POSIX mv(1) equivalent, but also copying the tags:
 move files and their tags into targetdir.
 -f  Force: remove destination if it exists.
 -i  Interactive: fail if the destination exists.
@@ -639,23 +644,14 @@
 
 Test whether `name` is a valid basefile for something in a directory.
 
 ## Function `main(argv=None)`
 
 Command line mode.
 
-## Function `rfilepaths(path, name_selector=None)`
-
-Generator yielding relative pathnames of files found under `path`.
-
-## Function `rpaths(path, *, yield_dirs=False, name_selector=None)`
-
-Generator to recurse over `path`, yielding `(is_dir,subpath)`
-for all selected subpaths.
-
 ## Function `rsync_patterns(paths, top_path)`
 
 Return a list of rsync include lines
 suitable for use with the `--include-from` option.
 
 ## Class `TaggedPath(cs.tagset.TagSet, HasFSTagsMixin, cs.fs.HasFSPath, cs.deco.Promotable)`
 
@@ -718,15 +714,15 @@
 the following additional names are available:
 * `fspath.basename`: basename of the `TaggedPath.fspath`
 * `fspath.ext`: the file extension of the basename
   of the `TaggedPath.fspath`
 * `fspath.pathname`: the `TaggedPath.fspath`
 * `fspath.encoded`: the JSON encoded fspath
 
-*Method `TaggedPath.from_str(fspath, *, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x1112f9510>)`*:
+*Method `TaggedPath.from_str(fspath, *, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x10b571090>)`*:
 Supports the `@promote` decorator.
 
 *Method `TaggedPath.get_xattr_tagset(self, xattr_name=None)`*:
 Return a new `TagSet`
 from the extended attribute `xattr_name` of `self.fspath`.
 The default `xattr_name` is `XATTR_B` (`None`).
 
@@ -799,14 +795,18 @@
 
 Emit message if in verbose mode.
 
 # Release Log
 
 
 
+*Release 20240422*:
+* Bugfix: .fstags files should no longer get Python repr() output for weirdly typed tag values.
+* Some other minor internal updates.
+
 *Release 20240412*:
 Changes to accomodate dropping BaseCommandOptions.runstate.
 
 *Release 20240316*:
 * TaggedPath.infer_tags: add _dt, _date, _f conversions, skip conversions which raise TypeError or ValueError.
 * rpaths: fix to yield relative paths.
```

### Comparing `cs.fstags-20240412/README.md` & `cs.fstags-20240422/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Simple filesystem based file tagging
 and the associated `fstags` command line script.
 
-*Latest release 20240412*:
-Changes to accomodate dropping BaseCommandOptions.runstate.
+*Latest release 20240422*:
+* Bugfix: .fstags files should no longer get Python repr() output for weirdly typed tag values.
+* Some other minor internal updates.
 
 Many basic tasks can be performed with the `fstags` command line utility,
 documented under the `FSTagsCommand` class below.
 
 Why `fstags`?
 By storing the tags in a separate file we:
 * can store tags without modifying a file
@@ -164,16 +165,16 @@
 Walk the file tree from `path`
 searching for files matching the supplied `tag_tests`.
 Yield the matching file paths.
 
 Parameters:
 * `path`: the top of the file tree to walk
 * `tag_tests`: a sequence of `TagBasedTest`s
-* `use_direct_tags`: test the direct_tags if true,
-  otherwise the all_tags.
+* `use_direct_tags`: test the `direct_tags` if true,
+  otherwise the `all_tags`.
   Default: `False`
 
 *Method `FSTags.find_ontology(self, dirpath, ontbase=None)`*:
 Locate an ontology for the directory `dirpath`.
 The optional `ontbase` may override the relative path to the file,
 default is `self.ontology_filepath`.
 Return a `TagOntology` or `None` if not found.
@@ -259,15 +260,17 @@
   otherwise the `all_tags`.
   Default: `False`
 
 ## Class `FSTagsCommand(cs.cmdutils.BaseCommand, cs.tagset.TagsCommandMixin)`
 
 `fstags` main command line utility.
 
-Command line usage:
+Command line implementation.
+
+Usage summary:
 
     Usage: fstags [-o ontology] [-P] subcommand [...]
       -o ontology   Specify the path to an ontology file.
       -P            Physical. Resolve pathnames through symlinks.
                     Default ~/.fstagsrc[general]physical or False.
       Subcommands:
         autotag paths...
@@ -329,23 +332,24 @@
         ln [-finv] srcpath dstpath, ln [-finv] srcpaths... dstdirpath
           POSIX ln(1) equivalent, but also copying the tags:
           link files and their tags into targetdir.
           -f  Force: remove destination if it exists.
           -i  Interactive: fail if the destination exists.
           -n  No remove: fail if the destination exists.
           -v  Verbose: show linked files.
-        ls [-d] [--direct] [-o output_format] [paths...]
+        ls [-dlr] [--direct] [-o output_format] [paths...]
           List files from paths and their tags.
           -d          Treat directories like files, do not recurse.
           --direct    List direct tags instead of all tags.
           -l          Long format.
           -o output_format
                       Use output_format as a Python format string to lay out
                       the listing.
                       Default: {fspath:json} {tags}
+          -r          Recurse into subdirectories.
         mv [-finv] srcpath dstpath, mv [-finv] srcpaths... dstdirpath
           POSIX mv(1) equivalent, but also copying the tags:
           move files and their tags into targetdir.
           -f  Force: remove destination if it exists.
           -i  Interactive: fail if the destination exists.
           -n  No remove: fail if the destination exists.
           -v  Verbose: show moved files.
@@ -391,15 +395,15 @@
           Update extended attributes from tags.
 
 *`FSTagsCommand.Options`*
 
 *Method `FSTagsCommand.apply_opt(self, opt, val)`*:
 Apply command line option.
 
-*Method `FSTagsCommand.cmd_autotag(self, argv, *, upd: cs.upd.Upd, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x1111add80>)`*:
+*Method `FSTagsCommand.cmd_autotag(self, argv, *, upd: cs.upd.Upd, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x10b33df30>)`*:
 Usage: {cmd} paths...
 Tag paths based on rules from the rc file.
 
 *Method `FSTagsCommand.cmd_cp(self, argv)`*:
 Usage: {cmd} [-finv] srcpath dstpath, {cmd} [-finv] srcpaths... dstdirpath
 POSIX cp(1) equivalent, but also copying tags:
 copy files and their tags into targetdir.
@@ -417,27 +421,27 @@
 Edit the direct tagsets of path, default: '.'
 If path is a directory, provide the tags of its entries.
 Otherwise edit just the tags for path.
 -a    List all names in directory edit mode; normally
       names commencing with a dot are omitted.
 -d    Treat directories like files: edit just its tags.
 
-*Method `FSTagsCommand.cmd_export(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x1111add80>)`*:
+*Method `FSTagsCommand.cmd_export(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x10b33df30>)`*:
 Usage: {cmd} [-a] [--direct] path {{tag[=value]|-tag}}...
 Export tags for files from paths matching all the constraints.
 -a        Export all paths, not just those with tags.
 --direct  Export the direct tags instead of the computed tags.
 The output is in the same CSV format as that from "sqltags export",
 with the following columns:
 * unixtime: the file's st_mtime from os.stat.
 * id: empty
 * name: the file path
 * tags: the file's direct or indirect tags
 
-*Method `FSTagsCommand.cmd_find(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x1111add80>)`*:
+*Method `FSTagsCommand.cmd_find(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x10b33df30>)`*:
 Usage: {cmd} [--direct] [--for-rsync] [-o output_format] path {{tag[=value]|-tag}}...
 List files from path matching all the constraints.
 --direct    Use direct tags instead of all tags.
 --for-rsync Instead of listing matching paths, emit a
             sequence of rsync(1) patterns suitable for use with
             --include-from in order to do a selective rsync of the
             matched paths.
@@ -469,24 +473,25 @@
 POSIX ln(1) equivalent, but also copying the tags:
 link files and their tags into targetdir.
 -f  Force: remove destination if it exists.
 -i  Interactive: fail if the destination exists.
 -n  No remove: fail if the destination exists.
 -v  Verbose: show linked files.
 
-*Method `FSTagsCommand.cmd_ls(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x1111add80>)`*:
-Usage: {cmd} [-d] [--direct] [-o output_format] [paths...]
+*Method `FSTagsCommand.cmd_ls(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x10b33df30>)`*:
+Usage: {cmd} [-dlr] [--direct] [-o output_format] [paths...]
 List files from paths and their tags.
 -d          Treat directories like files, do not recurse.
 --direct    List direct tags instead of all tags.
 -l          Long format.
 -o output_format
             Use output_format as a Python format string to lay out
             the listing.
             Default: {LS_OUTPUT_FORMAT_DEFAULT}
+-r          Recurse into subdirectories.
 
 *Method `FSTagsCommand.cmd_mv(self, argv)`*:
 Usage: {cmd} [-finv] srcpath dstpath, {cmd} [-finv] srcpaths... dstdirpath
 POSIX mv(1) equivalent, but also copying the tags:
 move files and their tags into targetdir.
 -f  Force: remove destination if it exists.
 -i  Interactive: fail if the destination exists.
@@ -621,23 +626,14 @@
 
 Test whether `name` is a valid basefile for something in a directory.
 
 ## Function `main(argv=None)`
 
 Command line mode.
 
-## Function `rfilepaths(path, name_selector=None)`
-
-Generator yielding relative pathnames of files found under `path`.
-
-## Function `rpaths(path, *, yield_dirs=False, name_selector=None)`
-
-Generator to recurse over `path`, yielding `(is_dir,subpath)`
-for all selected subpaths.
-
 ## Function `rsync_patterns(paths, top_path)`
 
 Return a list of rsync include lines
 suitable for use with the `--include-from` option.
 
 ## Class `TaggedPath(cs.tagset.TagSet, HasFSTagsMixin, cs.fs.HasFSPath, cs.deco.Promotable)`
 
@@ -700,15 +696,15 @@
 the following additional names are available:
 * `fspath.basename`: basename of the `TaggedPath.fspath`
 * `fspath.ext`: the file extension of the basename
   of the `TaggedPath.fspath`
 * `fspath.pathname`: the `TaggedPath.fspath`
 * `fspath.encoded`: the JSON encoded fspath
 
-*Method `TaggedPath.from_str(fspath, *, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x1112f9510>)`*:
+*Method `TaggedPath.from_str(fspath, *, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x10b571090>)`*:
 Supports the `@promote` decorator.
 
 *Method `TaggedPath.get_xattr_tagset(self, xattr_name=None)`*:
 Return a new `TagSet`
 from the extended attribute `xattr_name` of `self.fspath`.
 The default `xattr_name` is `XATTR_B` (`None`).
 
@@ -781,14 +777,18 @@
 
 Emit message if in verbose mode.
 
 # Release Log
 
 
 
+*Release 20240422*:
+* Bugfix: .fstags files should no longer get Python repr() output for weirdly typed tag values.
+* Some other minor internal updates.
+
 *Release 20240412*:
 Changes to accomodate dropping BaseCommandOptions.runstate.
 
 *Release 20240316*:
 * TaggedPath.infer_tags: add _dt, _date, _f conversions, skip conversions which raise TypeError or ValueError.
 * rpaths: fix to yield relative paths.
```

### Comparing `cs.fstags-20240412/lib/python/cs/fstags.1.md` & `cs.fstags-20240422/lib/python/cs/fstags.1.md`

 * *Files identical despite different names*

### Comparing `cs.fstags-20240412/lib/python/cs/fstags.5.md` & `cs.fstags-20240422/lib/python/cs/fstags.5.md`

 * *Files identical despite different names*

### Comparing `cs.fstags-20240412/lib/python/cs/fstags.py` & `cs.fstags-20240422/lib/python/cs/fstags.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,23 +102,23 @@
 
 from icontract import ensure, require
 
 from cs.cmdutils import BaseCommand
 from cs.context import stackattrs
 from cs.deco import default_params, fmtdoc, Promotable
 from cs.fileutils import crop_name, findup, shortpath
-from cs.fs import HasFSPath, FSPathBasedSingleton
+from cs.fs import HasFSPath, FSPathBasedSingleton, scandirpaths, scandirtree
 from cs.lex import (
     cutsuffix,
     get_ini_clause_entryname,
     FormatAsError,
     titleify_lc,
 )
 from cs.logutils import error, warning, ifverbose
-from cs.pfx import Pfx, pfx, pfx_method, pfx_call
+from cs.pfx import Pfx, pfx_method, pfx_call
 from cs.resources import MultiOpenMixin, RunState, uses_runstate
 from cs.tagset import (
     Tag,
     TagSet,
     TagBasedTest,
     TagsOntology,
     TagFile,
@@ -126,15 +126,15 @@
     TagsCommandMixin,
     RegexpTagRule,
     tag_or_tag_value,
 )
 from cs.threads import locked, locked_property, State
 from cs.upd import Upd, UpdProxy, uses_upd, print  # pylint: disable=redefined-builtin
 
-__version__ = '20240412'
+__version__ = '20240422'
 
 DISTINFO = {
     'keywords': ["python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
@@ -248,29 +248,29 @@
     fstags = options.fstags
     if not argv:
       argv = ['.']
     filename_rules = fstags.config.filename_rules
     with state(verbose=True):
       with UpdProxy() as proxy:
         for top_path in argv:
-          for isdir, path in rpaths(top_path, yield_dirs=True):
+          for is_dir, path in scandirtree(top_path, sort_names=True):
             runstate.raiseif()
             spath = shortpath(path)
             proxy.text = spath
             with Pfx(spath):
               ont = fstags.ontology_for(path)
               tagged_path = fstags[path]
               all_tags = tagged_path.merged_tags()
               for autotag in tagged_path.infer_from_basename(filename_rules):
                 proxy.text = spath + ' ' + str(autotag)
                 if ont:
                   autotag = ont.convert_tag(autotag)
                 if autotag not in all_tags:
                   tagged_path.add(autotag, verbose=state.verbose)
-              if not isdir:
+              if not is_dir:
                 try:
                   S = os.stat(path)
                 except OSError:
                   pass
                 else:
                   tagged_path.add('filesize', S.st_size)
               # update the merged tags
@@ -581,60 +581,65 @@
             tagged_path.add(
                 Tag(tag_name, value, ontology=ont), verbose=verbose
             )
     return 0
 
   @uses_runstate
   def cmd_ls(self, argv, *, runstate: RunState):
-    ''' Usage: {cmd} [-d] [--direct] [-o output_format] [paths...]
+    ''' Usage: {cmd} [-dlr] [--direct] [-o output_format] [paths...]
           List files from paths and their tags.
           -d          Treat directories like files, do not recurse.
           --direct    List direct tags instead of all tags.
           -l          Long format.
           -o output_format
                       Use output_format as a Python format string to lay out
                       the listing.
                       Default: {LS_OUTPUT_FORMAT_DEFAULT}
+          -r          Recurse into subdirectories.
     '''
     options = self.options
     fstags = options.fstags
-    directories_like_files = False
-    use_direct_tags = False
-    long_format = False
-    output_format = LS_OUTPUT_FORMAT_DEFAULT
-    opts, argv = getopt(argv, 'dlo:', longopts=['direct'])
-    for opt, value in opts:
-      with Pfx(opt):
-        if opt == '-d':
-          directories_like_files = True
-        elif opt == '--direct':
-          use_direct_tags = True
-        elif opt == '-l':
-          long_format = True
-        elif opt == '-o':
-          output_format = fstags.resolve_format_string(value)
-        else:
-          raise RuntimeError("unsupported option")
+    options.update(
+        directories_like_files=False,
+        use_direct_tags=False,
+        long_format=False,
+        output_format=LS_OUTPUT_FORMAT_DEFAULT,
+        recurse=False,
+    )
+    options.popopts(
+        argv,
+        d='directories_like_files',
+        direct='use_direct_tags',
+        l='long_format',
+        o_=('output_format', fstags.resolve_format_string),
+        r='recurse',
+    )
     xit = 0
     paths = argv or ['.']
     for path in paths:
       fullpath = realpath(path)
       for fspath in ((fullpath,)
-                     if directories_like_files else rfilepaths(fullpath)):
+                     if options.directories_like_files else scandirpaths(
+                         fullpath,
+                         sort_names=True,
+                         recurse=options.recurse,
+                     )):
         runstate.raiseif()
         with Pfx(fspath):
           tags = fstags[fspath]
-          if long_format:
+          if options.long_format:
             print(fspath)
-            for tag in tags.as_tags(all_tags=not use_direct_tags):
+            for tag in tags.as_tags(all_tags=not options.use_direct_tags):
               print(" ", tag)
           else:
             try:
               listing = tags.format_as(
-                  output_format, error_sep='\n  ', direct=use_direct_tags
+                  options.output_format,
+                  error_sep='\n  ',
+                  direct=options.use_direct_tags,
               )
             except FormatAsError as e:
               error(str(e))
               xit = 1
               continue
             print(listing)
     return xit
@@ -748,16 +753,16 @@
           use_direct_tags = True
         else:
           raise RuntimeError("unsupported option")
     xit = 0
     paths = argv or ['.']
     for path in paths:
       fullpath = realpath(path)
-      for fspath in ((fullpath,)
-                     if directories_like_files else rfilepaths(fullpath)):
+      for fspath in ((fullpath,) if directories_like_files else scandirpaths(
+          fullpath, sort_names=True)):
         with Pfx(fspath):
           tags = fstags[fspath].format_tagset(direct=use_direct_tags)
           print(fspath)
           for tag in sorted(tags.as_tags()):
             print(" ", tag)
     return xit
 
@@ -948,15 +953,15 @@
     '''
     badopts = False
     if not argv:
       warning("missing tag choice")
       badopts = True
     else:
       tag_choice_s = argv.pop(0)
-      with Pfx(repr(tag_choice_s)):
+      with Pfx("%r", tag_choice_s):
         try:
           remove, tag = self.parse_tag_addremove(tag_choice_s)
         except ValueError as e:
           warning(e)
           badopts = True
     if not argv:
       warning("missing paths")
@@ -1370,20 +1375,20 @@
     ''' Walk the file tree from `path`
         searching for files matching the supplied `tag_tests`.
         Yield the matching file paths.
 
         Parameters:
         * `path`: the top of the file tree to walk
         * `tag_tests`: a sequence of `TagBasedTest`s
-        * `use_direct_tags`: test the direct_tags if true,
-          otherwise the all_tags.
+        * `use_direct_tags`: test the `direct_tags` if true,
+          otherwise the `all_tags`.
           Default: `False`
     '''
     assert isinstance(tag_tests, (tuple, list))
-    for _, fspath in rpaths(path, yield_dirs=use_direct_tags):
+    for _, fspath in scandirtree(path, include_dirs=use_direct_tags):
       if self.test(fspath, tag_tests, use_direct_tags=use_direct_tags):
         yield fspath
 
   def test(self, path, tag_tests, use_direct_tags=False):
     ''' Test a path against `tag_tests`.
 
         Parameters:
@@ -1997,55 +2002,14 @@
         or `None` if there is no match.
     '''
     for tag_name in self.cascade:
       if tag_name in tagset:
         return Tag(self.target, tagset[tag_name])
     return None
 
-@pfx
-def rpaths(path, *, yield_dirs=False, name_selector=None):
-  ''' Generator to recurse over `path`, yielding `(is_dir,subpath)`
-      for all selected subpaths.
-  '''
-  if name_selector is None:
-    name_selector = lambda name: name and not name.startswith('.')
-  pending = [path]
-  while pending:
-    dirpath = pending.pop(0)
-    rdirpath = relpath(dirpath, path)
-    try:
-      with Pfx("scandir(%r)", dirpath):
-        dirents = sorted(os.scandir(dirpath), key=lambda entry: entry.name)
-    except NotADirectoryError:
-      yield False, rdirpath
-      continue
-    except (FileNotFoundError, PermissionError) as e:
-      warning("%s", e)
-      continue
-    for entry in dirents:
-      name = entry.name
-      if not name_selector(name):
-        continue
-      entrypath = entry.path
-      subpath = joinpath(rdirpath, entry.name)
-      if entry.is_dir(follow_symlinks=False):
-        if yield_dirs:
-          yield True, subpath
-        pending.append(entrypath)
-      else:
-        yield False, subpath
-
-def rfilepaths(path, name_selector=None):
-  ''' Generator yielding relative pathnames of files found under `path`.
-  '''
-  return (
-      subpath for is_dir, subpath in
-      rpaths(path, yield_dirs=False, name_selector=name_selector) if not is_dir
-  )
-
 def rsync_patterns(paths, top_path):
   ''' Return a list of rsync include lines
       suitable for use with the `--include-from` option.
   '''
   patterns = []
   include_dirs = set()
   for path in paths:
```

### Comparing `cs.fstags-20240412/lib/python/cs.fstags.egg-info/PKG-INFO` & `cs.fstags-20240422/lib/python/cs.fstags.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.fstags
-Version: 20240412
+Version: 20240422
 Summary: Simple filesystem based file tagging and the associated `fstags` command line script.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -15,16 +15,17 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Simple filesystem based file tagging
 and the associated `fstags` command line script.
 
-*Latest release 20240412*:
-Changes to accomodate dropping BaseCommandOptions.runstate.
+*Latest release 20240422*:
+* Bugfix: .fstags files should no longer get Python repr() output for weirdly typed tag values.
+* Some other minor internal updates.
 
 Many basic tasks can be performed with the `fstags` command line utility,
 documented under the `FSTagsCommand` class below.
 
 Why `fstags`?
 By storing the tags in a separate file we:
 * can store tags without modifying a file
@@ -182,16 +183,16 @@
 Walk the file tree from `path`
 searching for files matching the supplied `tag_tests`.
 Yield the matching file paths.
 
 Parameters:
 * `path`: the top of the file tree to walk
 * `tag_tests`: a sequence of `TagBasedTest`s
-* `use_direct_tags`: test the direct_tags if true,
-  otherwise the all_tags.
+* `use_direct_tags`: test the `direct_tags` if true,
+  otherwise the `all_tags`.
   Default: `False`
 
 *Method `FSTags.find_ontology(self, dirpath, ontbase=None)`*:
 Locate an ontology for the directory `dirpath`.
 The optional `ontbase` may override the relative path to the file,
 default is `self.ontology_filepath`.
 Return a `TagOntology` or `None` if not found.
@@ -277,15 +278,17 @@
   otherwise the `all_tags`.
   Default: `False`
 
 ## Class `FSTagsCommand(cs.cmdutils.BaseCommand, cs.tagset.TagsCommandMixin)`
 
 `fstags` main command line utility.
 
-Command line usage:
+Command line implementation.
+
+Usage summary:
 
     Usage: fstags [-o ontology] [-P] subcommand [...]
       -o ontology   Specify the path to an ontology file.
       -P            Physical. Resolve pathnames through symlinks.
                     Default ~/.fstagsrc[general]physical or False.
       Subcommands:
         autotag paths...
@@ -347,23 +350,24 @@
         ln [-finv] srcpath dstpath, ln [-finv] srcpaths... dstdirpath
           POSIX ln(1) equivalent, but also copying the tags:
           link files and their tags into targetdir.
           -f  Force: remove destination if it exists.
           -i  Interactive: fail if the destination exists.
           -n  No remove: fail if the destination exists.
           -v  Verbose: show linked files.
-        ls [-d] [--direct] [-o output_format] [paths...]
+        ls [-dlr] [--direct] [-o output_format] [paths...]
           List files from paths and their tags.
           -d          Treat directories like files, do not recurse.
           --direct    List direct tags instead of all tags.
           -l          Long format.
           -o output_format
                       Use output_format as a Python format string to lay out
                       the listing.
                       Default: {fspath:json} {tags}
+          -r          Recurse into subdirectories.
         mv [-finv] srcpath dstpath, mv [-finv] srcpaths... dstdirpath
           POSIX mv(1) equivalent, but also copying the tags:
           move files and their tags into targetdir.
           -f  Force: remove destination if it exists.
           -i  Interactive: fail if the destination exists.
           -n  No remove: fail if the destination exists.
           -v  Verbose: show moved files.
@@ -409,15 +413,15 @@
           Update extended attributes from tags.
 
 *`FSTagsCommand.Options`*
 
 *Method `FSTagsCommand.apply_opt(self, opt, val)`*:
 Apply command line option.
 
-*Method `FSTagsCommand.cmd_autotag(self, argv, *, upd: cs.upd.Upd, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x1111add80>)`*:
+*Method `FSTagsCommand.cmd_autotag(self, argv, *, upd: cs.upd.Upd, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x10b33df30>)`*:
 Usage: {cmd} paths...
 Tag paths based on rules from the rc file.
 
 *Method `FSTagsCommand.cmd_cp(self, argv)`*:
 Usage: {cmd} [-finv] srcpath dstpath, {cmd} [-finv] srcpaths... dstdirpath
 POSIX cp(1) equivalent, but also copying tags:
 copy files and their tags into targetdir.
@@ -435,27 +439,27 @@
 Edit the direct tagsets of path, default: '.'
 If path is a directory, provide the tags of its entries.
 Otherwise edit just the tags for path.
 -a    List all names in directory edit mode; normally
       names commencing with a dot are omitted.
 -d    Treat directories like files: edit just its tags.
 
-*Method `FSTagsCommand.cmd_export(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x1111add80>)`*:
+*Method `FSTagsCommand.cmd_export(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x10b33df30>)`*:
 Usage: {cmd} [-a] [--direct] path {{tag[=value]|-tag}}...
 Export tags for files from paths matching all the constraints.
 -a        Export all paths, not just those with tags.
 --direct  Export the direct tags instead of the computed tags.
 The output is in the same CSV format as that from "sqltags export",
 with the following columns:
 * unixtime: the file's st_mtime from os.stat.
 * id: empty
 * name: the file path
 * tags: the file's direct or indirect tags
 
-*Method `FSTagsCommand.cmd_find(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x1111add80>)`*:
+*Method `FSTagsCommand.cmd_find(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x10b33df30>)`*:
 Usage: {cmd} [--direct] [--for-rsync] [-o output_format] path {{tag[=value]|-tag}}...
 List files from path matching all the constraints.
 --direct    Use direct tags instead of all tags.
 --for-rsync Instead of listing matching paths, emit a
             sequence of rsync(1) patterns suitable for use with
             --include-from in order to do a selective rsync of the
             matched paths.
@@ -487,24 +491,25 @@
 POSIX ln(1) equivalent, but also copying the tags:
 link files and their tags into targetdir.
 -f  Force: remove destination if it exists.
 -i  Interactive: fail if the destination exists.
 -n  No remove: fail if the destination exists.
 -v  Verbose: show linked files.
 
-*Method `FSTagsCommand.cmd_ls(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x1111add80>)`*:
-Usage: {cmd} [-d] [--direct] [-o output_format] [paths...]
+*Method `FSTagsCommand.cmd_ls(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x10b33df30>)`*:
+Usage: {cmd} [-dlr] [--direct] [-o output_format] [paths...]
 List files from paths and their tags.
 -d          Treat directories like files, do not recurse.
 --direct    List direct tags instead of all tags.
 -l          Long format.
 -o output_format
             Use output_format as a Python format string to lay out
             the listing.
             Default: {LS_OUTPUT_FORMAT_DEFAULT}
+-r          Recurse into subdirectories.
 
 *Method `FSTagsCommand.cmd_mv(self, argv)`*:
 Usage: {cmd} [-finv] srcpath dstpath, {cmd} [-finv] srcpaths... dstdirpath
 POSIX mv(1) equivalent, but also copying the tags:
 move files and their tags into targetdir.
 -f  Force: remove destination if it exists.
 -i  Interactive: fail if the destination exists.
@@ -639,23 +644,14 @@
 
 Test whether `name` is a valid basefile for something in a directory.
 
 ## Function `main(argv=None)`
 
 Command line mode.
 
-## Function `rfilepaths(path, name_selector=None)`
-
-Generator yielding relative pathnames of files found under `path`.
-
-## Function `rpaths(path, *, yield_dirs=False, name_selector=None)`
-
-Generator to recurse over `path`, yielding `(is_dir,subpath)`
-for all selected subpaths.
-
 ## Function `rsync_patterns(paths, top_path)`
 
 Return a list of rsync include lines
 suitable for use with the `--include-from` option.
 
 ## Class `TaggedPath(cs.tagset.TagSet, HasFSTagsMixin, cs.fs.HasFSPath, cs.deco.Promotable)`
 
@@ -718,15 +714,15 @@
 the following additional names are available:
 * `fspath.basename`: basename of the `TaggedPath.fspath`
 * `fspath.ext`: the file extension of the basename
   of the `TaggedPath.fspath`
 * `fspath.pathname`: the `TaggedPath.fspath`
 * `fspath.encoded`: the JSON encoded fspath
 
-*Method `TaggedPath.from_str(fspath, *, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x1112f9510>)`*:
+*Method `TaggedPath.from_str(fspath, *, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x10b571090>)`*:
 Supports the `@promote` decorator.
 
 *Method `TaggedPath.get_xattr_tagset(self, xattr_name=None)`*:
 Return a new `TagSet`
 from the extended attribute `xattr_name` of `self.fspath`.
 The default `xattr_name` is `XATTR_B` (`None`).
 
@@ -799,14 +795,18 @@
 
 Emit message if in verbose mode.
 
 # Release Log
 
 
 
+*Release 20240422*:
+* Bugfix: .fstags files should no longer get Python repr() output for weirdly typed tag values.
+* Some other minor internal updates.
+
 *Release 20240412*:
 Changes to accomodate dropping BaseCommandOptions.runstate.
 
 *Release 20240316*:
 * TaggedPath.infer_tags: add _dt, _date, _f conversions, skip conversions which raise TypeError or ValueError.
 * rpaths: fix to yield relative paths.
```

### Comparing `cs.fstags-20240412/pyproject.toml` & `cs.fstags-20240422/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,30 +12,30 @@
     "cs.context>=20240412",
     "cs.deco>=20240412",
     "cs.fileutils>=20240316",
     "cs.fs>=20220429",
     "cs.lex>=20240316",
     "cs.logutils>=20230212",
     "cs.pfx>=20240412",
-    "cs.resources>=20240412",
+    "cs.resources>=20240422",
     "cs.tagset>=20211212",
-    "cs.threads>=20240412",
+    "cs.threads>=20240422",
     "cs.upd>=20240412",
     "icontract",
 ]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20240412"
+version = "20240422"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
@@ -43,16 +43,17 @@
 fstags = "cs.fstags:main"
 
 [project.readme]
 text = """
 Simple filesystem based file tagging
 and the associated `fstags` command line script.
 
-*Latest release 20240412*:
-Changes to accomodate dropping BaseCommandOptions.runstate.
+*Latest release 20240422*:
+* Bugfix: .fstags files should no longer get Python repr() output for weirdly typed tag values.
+* Some other minor internal updates.
 
 Many basic tasks can be performed with the `fstags` command line utility,
 documented under the `FSTagsCommand` class below.
 
 Why `fstags`?
 By storing the tags in a separate file we:
 * can store tags without modifying a file
@@ -210,16 +211,16 @@
 Walk the file tree from `path`
 searching for files matching the supplied `tag_tests`.
 Yield the matching file paths.
 
 Parameters:
 * `path`: the top of the file tree to walk
 * `tag_tests`: a sequence of `TagBasedTest`s
-* `use_direct_tags`: test the direct_tags if true,
-  otherwise the all_tags.
+* `use_direct_tags`: test the `direct_tags` if true,
+  otherwise the `all_tags`.
   Default: `False`
 
 *Method `FSTags.find_ontology(self, dirpath, ontbase=None)`*:
 Locate an ontology for the directory `dirpath`.
 The optional `ontbase` may override the relative path to the file,
 default is `self.ontology_filepath`.
 Return a `TagOntology` or `None` if not found.
@@ -305,15 +306,17 @@
   otherwise the `all_tags`.
   Default: `False`
 
 ## Class `FSTagsCommand(cs.cmdutils.BaseCommand, cs.tagset.TagsCommandMixin)`
 
 `fstags` main command line utility.
 
-Command line usage:
+Command line implementation.
+
+Usage summary:
 
     Usage: fstags [-o ontology] [-P] subcommand [...]
       -o ontology   Specify the path to an ontology file.
       -P            Physical. Resolve pathnames through symlinks.
                     Default ~/.fstagsrc[general]physical or False.
       Subcommands:
         autotag paths...
@@ -375,23 +378,24 @@
         ln [-finv] srcpath dstpath, ln [-finv] srcpaths... dstdirpath
           POSIX ln(1) equivalent, but also copying the tags:
           link files and their tags into targetdir.
           -f  Force: remove destination if it exists.
           -i  Interactive: fail if the destination exists.
           -n  No remove: fail if the destination exists.
           -v  Verbose: show linked files.
-        ls [-d] [--direct] [-o output_format] [paths...]
+        ls [-dlr] [--direct] [-o output_format] [paths...]
           List files from paths and their tags.
           -d          Treat directories like files, do not recurse.
           --direct    List direct tags instead of all tags.
           -l          Long format.
           -o output_format
                       Use output_format as a Python format string to lay out
                       the listing.
                       Default: {fspath:json} {tags}
+          -r          Recurse into subdirectories.
         mv [-finv] srcpath dstpath, mv [-finv] srcpaths... dstdirpath
           POSIX mv(1) equivalent, but also copying the tags:
           move files and their tags into targetdir.
           -f  Force: remove destination if it exists.
           -i  Interactive: fail if the destination exists.
           -n  No remove: fail if the destination exists.
           -v  Verbose: show moved files.
@@ -437,15 +441,15 @@
           Update extended attributes from tags.
 
 *`FSTagsCommand.Options`*
 
 *Method `FSTagsCommand.apply_opt(self, opt, val)`*:
 Apply command line option.
 
-*Method `FSTagsCommand.cmd_autotag(self, argv, *, upd: cs.upd.Upd, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x1111add80>)`*:
+*Method `FSTagsCommand.cmd_autotag(self, argv, *, upd: cs.upd.Upd, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x10b33df30>)`*:
 Usage: {cmd} paths...
 Tag paths based on rules from the rc file.
 
 *Method `FSTagsCommand.cmd_cp(self, argv)`*:
 Usage: {cmd} [-finv] srcpath dstpath, {cmd} [-finv] srcpaths... dstdirpath
 POSIX cp(1) equivalent, but also copying tags:
 copy files and their tags into targetdir.
@@ -463,27 +467,27 @@
 Edit the direct tagsets of path, default: '.'
 If path is a directory, provide the tags of its entries.
 Otherwise edit just the tags for path.
 -a    List all names in directory edit mode; normally
       names commencing with a dot are omitted.
 -d    Treat directories like files: edit just its tags.
 
-*Method `FSTagsCommand.cmd_export(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x1111add80>)`*:
+*Method `FSTagsCommand.cmd_export(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x10b33df30>)`*:
 Usage: {cmd} [-a] [--direct] path {{tag[=value]|-tag}}...
 Export tags for files from paths matching all the constraints.
 -a        Export all paths, not just those with tags.
 --direct  Export the direct tags instead of the computed tags.
 The output is in the same CSV format as that from \"sqltags export\",
 with the following columns:
 * unixtime: the file's st_mtime from os.stat.
 * id: empty
 * name: the file path
 * tags: the file's direct or indirect tags
 
-*Method `FSTagsCommand.cmd_find(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x1111add80>)`*:
+*Method `FSTagsCommand.cmd_find(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x10b33df30>)`*:
 Usage: {cmd} [--direct] [--for-rsync] [-o output_format] path {{tag[=value]|-tag}}...
 List files from path matching all the constraints.
 --direct    Use direct tags instead of all tags.
 --for-rsync Instead of listing matching paths, emit a
             sequence of rsync(1) patterns suitable for use with
             --include-from in order to do a selective rsync of the
             matched paths.
@@ -515,24 +519,25 @@
 POSIX ln(1) equivalent, but also copying the tags:
 link files and their tags into targetdir.
 -f  Force: remove destination if it exists.
 -i  Interactive: fail if the destination exists.
 -n  No remove: fail if the destination exists.
 -v  Verbose: show linked files.
 
-*Method `FSTagsCommand.cmd_ls(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x1111add80>)`*:
-Usage: {cmd} [-d] [--direct] [-o output_format] [paths...]
+*Method `FSTagsCommand.cmd_ls(self, argv, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x10b33df30>)`*:
+Usage: {cmd} [-dlr] [--direct] [-o output_format] [paths...]
 List files from paths and their tags.
 -d          Treat directories like files, do not recurse.
 --direct    List direct tags instead of all tags.
 -l          Long format.
 -o output_format
             Use output_format as a Python format string to lay out
             the listing.
             Default: {LS_OUTPUT_FORMAT_DEFAULT}
+-r          Recurse into subdirectories.
 
 *Method `FSTagsCommand.cmd_mv(self, argv)`*:
 Usage: {cmd} [-finv] srcpath dstpath, {cmd} [-finv] srcpaths... dstdirpath
 POSIX mv(1) equivalent, but also copying the tags:
 move files and their tags into targetdir.
 -f  Force: remove destination if it exists.
 -i  Interactive: fail if the destination exists.
@@ -667,23 +672,14 @@
 
 Test whether `name` is a valid basefile for something in a directory.
 
 ## Function `main(argv=None)`
 
 Command line mode.
 
-## Function `rfilepaths(path, name_selector=None)`
-
-Generator yielding relative pathnames of files found under `path`.
-
-## Function `rpaths(path, *, yield_dirs=False, name_selector=None)`
-
-Generator to recurse over `path`, yielding `(is_dir,subpath)`
-for all selected subpaths.
-
 ## Function `rsync_patterns(paths, top_path)`
 
 Return a list of rsync include lines
 suitable for use with the `--include-from` option.
 
 ## Class `TaggedPath(cs.tagset.TagSet, HasFSTagsMixin, cs.fs.HasFSPath, cs.deco.Promotable)`
 
@@ -746,15 +742,15 @@
 the following additional names are available:
 * `fspath.basename`: basename of the `TaggedPath.fspath`
 * `fspath.ext`: the file extension of the basename
   of the `TaggedPath.fspath`
 * `fspath.pathname`: the `TaggedPath.fspath`
 * `fspath.encoded`: the JSON encoded fspath
 
-*Method `TaggedPath.from_str(fspath, *, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x1112f9510>)`*:
+*Method `TaggedPath.from_str(fspath, *, fstags: Optional[cs.fstags.FSTags] = <function <lambda> at 0x10b571090>)`*:
 Supports the `@promote` decorator.
 
 *Method `TaggedPath.get_xattr_tagset(self, xattr_name=None)`*:
 Return a new `TagSet`
 from the extended attribute `xattr_name` of `self.fspath`.
 The default `xattr_name` is `XATTR_B` (`None`).
 
@@ -827,14 +823,18 @@
 
 Emit message if in verbose mode.
 
 # Release Log
 
 
 
+*Release 20240422*:
+* Bugfix: .fstags files should no longer get Python repr() output for weirdly typed tag values.
+* Some other minor internal updates.
+
 *Release 20240412*:
 Changes to accomodate dropping BaseCommandOptions.runstate.
 
 *Release 20240316*:
 * TaggedPath.infer_tags: add _dt, _date, _f conversions, skip conversions which raise TypeError or ValueError.
 * rpaths: fix to yield relative paths.
```


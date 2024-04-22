# Comparing `tmp/cs.cmdutils-20240412.tar.gz` & `tmp/cs.cmdutils-20240422.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.cmdutils-20240412.tar", last modified: Fri Apr 12 05:25:38 2024, max compression
+gzip compressed data, was "cs.cmdutils-20240422.tar", last modified: Mon Apr 22 02:56:31 2024, max compression
```

## Comparing `cs.cmdutils-20240412.tar` & `cs.cmdutils-20240422.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:25:38.222527 cs.cmdutils-20240412/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-12 05:24:59.000000 cs.cmdutils-20240412/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    30680 2024-04-12 05:25:38.222192 cs.cmdutils-20240412/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    29810 2024-04-12 05:25:12.000000 cs.cmdutils-20240412/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:25:38.217738 cs.cmdutils-20240412/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:25:38.217991 cs.cmdutils-20240412/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:25:38.219329 cs.cmdutils-20240412/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    50878 2024-04-12 05:24:48.000000 cs.cmdutils-20240412/lib/python/cs/cmdutils.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-12 05:25:38.221723 cs.cmdutils-20240412/lib/python/cs.cmdutils.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    30680 2024-04-12 05:25:37.000000 cs.cmdutils-20240412/lib/python/cs.cmdutils.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      291 2024-04-12 05:25:38.000000 cs.cmdutils-20240412/lib/python/cs.cmdutils.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-12 05:25:37.000000 cs.cmdutils-20240412/lib/python/cs.cmdutils.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      231 2024-04-12 05:25:38.000000 cs.cmdutils-20240412/lib/python/cs.cmdutils.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-12 05:25:38.000000 cs.cmdutils-20240412/lib/python/cs.cmdutils.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    31399 2024-04-12 05:25:36.000000 cs.cmdutils-20240412/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-12 05:25:38.222625 cs.cmdutils-20240412/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:56:31.562566 cs.cmdutils-20240422/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-22 02:55:45.000000 cs.cmdutils-20240422/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    31799 2024-04-22 02:56:31.561543 cs.cmdutils-20240422/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    30929 2024-04-22 02:56:00.000000 cs.cmdutils-20240422/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:56:31.557411 cs.cmdutils-20240422/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:56:31.557725 cs.cmdutils-20240422/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:56:31.559253 cs.cmdutils-20240422/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    52525 2024-04-22 02:55:32.000000 cs.cmdutils-20240422/lib/python/cs/cmdutils.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:56:31.561063 cs.cmdutils-20240422/lib/python/cs.cmdutils.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    31799 2024-04-22 02:56:31.000000 cs.cmdutils-20240422/lib/python/cs.cmdutils.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      291 2024-04-22 02:56:31.000000 cs.cmdutils-20240422/lib/python/cs.cmdutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-22 02:56:31.000000 cs.cmdutils-20240422/lib/python/cs.cmdutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      231 2024-04-22 02:56:31.000000 cs.cmdutils-20240422/lib/python/cs.cmdutils.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-22 02:56:31.000000 cs.cmdutils-20240422/lib/python/cs.cmdutils.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    32520 2024-04-22 02:56:30.000000 cs.cmdutils-20240422/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-22 02:56:31.562677 cs.cmdutils-20240422/setup.cfg
```

### Comparing `cs.cmdutils-20240412/PKG-INFO` & `cs.cmdutils-20240422/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.cmdutils
-Version: 20240412
+Version: 20240422
 Summary: Convenience functions for working with the Cmd module, the BaseCommand class for constructing command line programmes, and other command line related stuff.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -16,17 +16,18 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Convenience functions for working with the Cmd module,
 the BaseCommand class for constructing command line programmes,
 and other command line related stuff.
 
-*Latest release 20240412*:
-* BaseCommand.run_context: do not store .upd and .runstate on the options (it confuses options in subcommands and we have @uses_runstate and @uses_upd forthis anyway these days).
-* BaseCommand.run_context: catch SIGQUIT, present the default handler as BaseCommand.handle_signal.
+*Latest release 20240422*:
+* BaseCommandOptions.popopts: return the dict from BaseCommand.popopts().
+* BaseCommand.apply_preargv: apply the default options supported by self.options.
+* BaseCommandOptions.update(mapping) method, useful for dropping subcommand-specific defaults onto the options ahead of the local popopts() call.
 
 ## Class `BaseCommand`
 
 A base class for handling nestable command lines.
 
 This class provides the basic parse and dispatch mechanisms
 for command lines.
@@ -201,15 +202,17 @@
 Subclasses can override this
 but it is usually easier to override `apply_opt(opt,val)`.
 
 *Method `BaseCommand.apply_preargv(self, argv)`*:
 Do any preparsing of `argv` before the subcommand/main-args.
 Return the remaining arguments.
 
-This default implementation returns `argv` unchanged.
+This default implementation applies the default options
+supported by `self.options` (an instance of `self.Options`
+class).
 
 *Method `BaseCommand.cmd_help(argv)`*:
 Usage: {cmd} [-l] [subcommand-names...]
 Print help for subcommands.
 This outputs the full help for the named subcommands,
 or the short help for all subcommands if no names are specified.
 -l  Long help even if no subcommand-names provided.
@@ -248,15 +251,15 @@
 this can be overridden with a method which just returns `False`.
 
 Otherwise,
 the handler may perform any suitable action
 and return `True` to contain the exception
 or `False` to cause the exception to be reraised.
 
-*Method `BaseCommand.handle_signal(self, sig, frame, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x10d5b1d80>)`*:
+*Method `BaseCommand.handle_signal(self, sig, frame, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x104df9f30>)`*:
 The default signal handler, which cancels the default `RunState`.
 
 *Method `BaseCommand.poparg(argv: List[str], *a, unpop_on_error=False)`*:
 Pop the leading argument off `argv` and parse it.
 Return the parsed argument.
 Raises `getopt.GetoptError` on a missing or invalid argument.
 
@@ -347,57 +350,63 @@
 * a single letter name specifies a short option
   and a multiletter name specifies a long option
 * options requiring an argument have a trailing underscore
 * options not requiring an argument normally imply a value
   of `True`; if their synonym commences with a dash they will
   imply a value of `False`, for example `n='dry_run',y='-dry_run'`
 
-As it happens, the `BaseCommandOptions` class provided a `popopts` method
-which is a shim for this method with `attrfor=self` i.e. the options object.
-So common use in a command method might look like this:
+The `BaseCommandOptions` class provides a `popopts` method
+which is a shim for this method with `attrfor=self` i.e.
+the options object.
+So common use in a command method usually looks like this:
 
     class SomeCommand(BaseCommand):
 
         def cmd_foo(self, argv):
             options = self.options
             # accept a -j or --jobs options
-            options.poopts(argv, jobs=1, j='jobs')
+            options.popopts(argv, jobs=1, j='jobs')
             print("jobs =", options.jobs)
 
+The `self.options` object is preprovided as an instance of
+the `self.Options` class, which is `BaseCommandOptions` by
+default. This presupplies support for some basic options
+like `-v` for "verbose" and so forth, and a subcommand
+need not describe these in a call to `self.options.popopts()`.
+
 Example:
 
     >>> import os.path
-    >>> options = SimpleNamespace(
-    ...   all=False,
-    ...   jobs=1,
-    ...   number=0,
-    ...   once=False,
-    ...   path=None,
-    ...   trace_exec=True,
-    ...   verbose=False,
-    ...   dry_run=False)
+    >>> from typing import Optional
+    >>> @dataclass
+    ... class DemoOptions(BaseCommandOptions):
+    ...   all: bool = False
+    ...   jobs: int = 1
+    ...   number: int = 0
+    ...   once: bool = False
+    ...   path: Optional[str] = None
+    ...   trace_exec: bool = False
+    ...
+    >>> options = DemoOptions()
     >>> argv = ['-1', '-v', '-y', '-j4', '--path=/foo', 'bah', '-x']
-    >>> opt_dict = BaseCommand.popopts(
+    >>> opt_dict = options.popopts(
     ...   argv,
-    ...   options,
     ...   _1='once',
     ...   a='all',
     ...   j_=('jobs',int),
-    ...   n='dry_run',
-    ...   v='verbose',
     ...   x='-trace_exec',
     ...   y='-dry_run',
     ...   dry_run=None,
     ...   path_=(str, os.path.isabs, 'not an absolute path'),
     ...   verbose=None,
     ... )
     >>> opt_dict
     {'once': True, 'verbose': True, 'dry_run': False, 'jobs': 4, 'path': '/foo'}
-    >>> options
-    namespace(all=False, jobs=4, number=0, once=True, path='/foo', trace_exec=True, verbose=True, dry_run=False)
+    >>> options # doctest: +ELLIPSIS
+    DemoOptions(cmd=None, dry_run=False, force=False, quiet=False, runstate_signals=(...), verbose=True, all=False, jobs=4, number=0, once=True, path='/foo', trace_exec=False)
 
 *Method `BaseCommand.repl(self, *argv, banner=None, local=None)`*:
 Run an interactive Python prompt with some predefined local names.
 Aka REPL (Read Evaluate Print Loop).
 
 Parameters:
 * `argv`: any notional command line arguments
@@ -438,15 +447,15 @@
 Otherwise `self.main(argv)` is called
 and its value returned.
 
 If the command implementation requires some setup or teardown
 then this may be provided by the `run_context()`
 context manager method.
 
-*Method `BaseCommand.run_context(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x10d48e290>, **kw)`*:
+*Method `BaseCommand.run_context(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x104cea3b0>, **kw)`*:
 The context manager which surrounds `main` or `cmd_`*subcmd*.
 
 This default does several things, and subclasses should
 override it like this:
 
     @contextmanager
     def run_context(self):
@@ -515,20 +524,24 @@
 
     @dataclass
     class Options(BaseCommand.Options):
         ... optional extra fields etc ...
 
 *Method `BaseCommandOptions.__call__(self, **updates)`*:
 Calling the options object returns a context manager whose
-value is a copy of the options with any `suboptions` applied.
+value is a shallow copy of the options with any `suboptions` applied.
 
 Example showing the semantics:
 
     >>> from cs.cmdutils import BaseCommandOptions
-    >>> options = BaseCommandOptions(x=1)
+    >>> @dataclass
+    ... class DemoOptions(BaseCommandOptions):
+    ...   x: int = 0
+    ...
+    >>> options = DemoOptions(x=1)
     >>> assert options.x == 1
     >>> assert not options.verbose
     >>> with options(verbose=True) as subopts:
     ...     assert options is not subopts
     ...     assert options.x == 1
     ...     assert not options.verbose
     ...     assert subopts.x == 1
@@ -573,14 +586,19 @@
     COMMON_OPT_SPECS = dict(
         e='ssh_exe',
         h_='hashname',
         H_='hashindex_exe',
         **BaseCommand.Options.COMMON_OPT_SPECS,
     )
 
+*Method `BaseCommandOptions.update(self, **updates)`*:
+Modify the options in place with the mapping `updates`.
+It would be more normal to call the options in a `with` statement
+as shown for `__call__`.
+
 ## Function `docmd(dofunc)`
 
 Decorator for `cmd.Cmd` subclass methods
 to supply some basic quality of service.
 
 This decorator:
 - wraps the function call in a `cs.pfx.Pfx` for context
@@ -635,14 +653,19 @@
             print("doing f with x =", x)
         ....
 
 # Release Log
 
 
 
+*Release 20240422*:
+* BaseCommandOptions.popopts: return the dict from BaseCommand.popopts().
+* BaseCommand.apply_preargv: apply the default options supported by self.options.
+* BaseCommandOptions.update(mapping) method, useful for dropping subcommand-specific defaults onto the options ahead of the local popopts() call.
+
 *Release 20240412*:
 * BaseCommand.run_context: do not store .upd and .runstate on the options (it confuses options in subcommands and we have @uses_runstate and @uses_upd forthis anyway these days).
 * BaseCommand.run_context: catch SIGQUIT, present the default handler as BaseCommand.handle_signal.
 
 *Release 20240316*:
 * New @uses_cmd_options decorator to provide an "options" parameter being the prevailing BaseCommandOptions instance.
 * BaseCommandOptions.popopts: get common options from BaseCommandOptions.COMMON_OPT_SPECS.
```

### Comparing `cs.cmdutils-20240412/README.md` & `cs.cmdutils-20240422/lib/python/cs.cmdutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,33 @@
+Metadata-Version: 2.1
+Name: cs.cmdutils
+Version: 20240422
+Summary: Convenience functions for working with the Cmd module, the BaseCommand class for constructing command line programmes, and other command line related stuff.
+Author-email: Cameron Simpson <cs@cskk.id.au>
+License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
+Keywords: python2,python3
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Description-Content-Type: text/markdown
+
 Convenience functions for working with the Cmd module,
 the BaseCommand class for constructing command line programmes,
 and other command line related stuff.
 
-*Latest release 20240412*:
-* BaseCommand.run_context: do not store .upd and .runstate on the options (it confuses options in subcommands and we have @uses_runstate and @uses_upd forthis anyway these days).
-* BaseCommand.run_context: catch SIGQUIT, present the default handler as BaseCommand.handle_signal.
+*Latest release 20240422*:
+* BaseCommandOptions.popopts: return the dict from BaseCommand.popopts().
+* BaseCommand.apply_preargv: apply the default options supported by self.options.
+* BaseCommandOptions.update(mapping) method, useful for dropping subcommand-specific defaults onto the options ahead of the local popopts() call.
 
 ## Class `BaseCommand`
 
 A base class for handling nestable command lines.
 
 This class provides the basic parse and dispatch mechanisms
 for command lines.
@@ -183,15 +202,17 @@
 Subclasses can override this
 but it is usually easier to override `apply_opt(opt,val)`.
 
 *Method `BaseCommand.apply_preargv(self, argv)`*:
 Do any preparsing of `argv` before the subcommand/main-args.
 Return the remaining arguments.
 
-This default implementation returns `argv` unchanged.
+This default implementation applies the default options
+supported by `self.options` (an instance of `self.Options`
+class).
 
 *Method `BaseCommand.cmd_help(argv)`*:
 Usage: {cmd} [-l] [subcommand-names...]
 Print help for subcommands.
 This outputs the full help for the named subcommands,
 or the short help for all subcommands if no names are specified.
 -l  Long help even if no subcommand-names provided.
@@ -230,15 +251,15 @@
 this can be overridden with a method which just returns `False`.
 
 Otherwise,
 the handler may perform any suitable action
 and return `True` to contain the exception
 or `False` to cause the exception to be reraised.
 
-*Method `BaseCommand.handle_signal(self, sig, frame, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x10d5b1d80>)`*:
+*Method `BaseCommand.handle_signal(self, sig, frame, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x104df9f30>)`*:
 The default signal handler, which cancels the default `RunState`.
 
 *Method `BaseCommand.poparg(argv: List[str], *a, unpop_on_error=False)`*:
 Pop the leading argument off `argv` and parse it.
 Return the parsed argument.
 Raises `getopt.GetoptError` on a missing or invalid argument.
 
@@ -329,57 +350,63 @@
 * a single letter name specifies a short option
   and a multiletter name specifies a long option
 * options requiring an argument have a trailing underscore
 * options not requiring an argument normally imply a value
   of `True`; if their synonym commences with a dash they will
   imply a value of `False`, for example `n='dry_run',y='-dry_run'`
 
-As it happens, the `BaseCommandOptions` class provided a `popopts` method
-which is a shim for this method with `attrfor=self` i.e. the options object.
-So common use in a command method might look like this:
+The `BaseCommandOptions` class provides a `popopts` method
+which is a shim for this method with `attrfor=self` i.e.
+the options object.
+So common use in a command method usually looks like this:
 
     class SomeCommand(BaseCommand):
 
         def cmd_foo(self, argv):
             options = self.options
             # accept a -j or --jobs options
-            options.poopts(argv, jobs=1, j='jobs')
+            options.popopts(argv, jobs=1, j='jobs')
             print("jobs =", options.jobs)
 
+The `self.options` object is preprovided as an instance of
+the `self.Options` class, which is `BaseCommandOptions` by
+default. This presupplies support for some basic options
+like `-v` for "verbose" and so forth, and a subcommand
+need not describe these in a call to `self.options.popopts()`.
+
 Example:
 
     >>> import os.path
-    >>> options = SimpleNamespace(
-    ...   all=False,
-    ...   jobs=1,
-    ...   number=0,
-    ...   once=False,
-    ...   path=None,
-    ...   trace_exec=True,
-    ...   verbose=False,
-    ...   dry_run=False)
+    >>> from typing import Optional
+    >>> @dataclass
+    ... class DemoOptions(BaseCommandOptions):
+    ...   all: bool = False
+    ...   jobs: int = 1
+    ...   number: int = 0
+    ...   once: bool = False
+    ...   path: Optional[str] = None
+    ...   trace_exec: bool = False
+    ...
+    >>> options = DemoOptions()
     >>> argv = ['-1', '-v', '-y', '-j4', '--path=/foo', 'bah', '-x']
-    >>> opt_dict = BaseCommand.popopts(
+    >>> opt_dict = options.popopts(
     ...   argv,
-    ...   options,
     ...   _1='once',
     ...   a='all',
     ...   j_=('jobs',int),
-    ...   n='dry_run',
-    ...   v='verbose',
     ...   x='-trace_exec',
     ...   y='-dry_run',
     ...   dry_run=None,
     ...   path_=(str, os.path.isabs, 'not an absolute path'),
     ...   verbose=None,
     ... )
     >>> opt_dict
     {'once': True, 'verbose': True, 'dry_run': False, 'jobs': 4, 'path': '/foo'}
-    >>> options
-    namespace(all=False, jobs=4, number=0, once=True, path='/foo', trace_exec=True, verbose=True, dry_run=False)
+    >>> options # doctest: +ELLIPSIS
+    DemoOptions(cmd=None, dry_run=False, force=False, quiet=False, runstate_signals=(...), verbose=True, all=False, jobs=4, number=0, once=True, path='/foo', trace_exec=False)
 
 *Method `BaseCommand.repl(self, *argv, banner=None, local=None)`*:
 Run an interactive Python prompt with some predefined local names.
 Aka REPL (Read Evaluate Print Loop).
 
 Parameters:
 * `argv`: any notional command line arguments
@@ -420,15 +447,15 @@
 Otherwise `self.main(argv)` is called
 and its value returned.
 
 If the command implementation requires some setup or teardown
 then this may be provided by the `run_context()`
 context manager method.
 
-*Method `BaseCommand.run_context(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x10d48e290>, **kw)`*:
+*Method `BaseCommand.run_context(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x104cea3b0>, **kw)`*:
 The context manager which surrounds `main` or `cmd_`*subcmd*.
 
 This default does several things, and subclasses should
 override it like this:
 
     @contextmanager
     def run_context(self):
@@ -497,20 +524,24 @@
 
     @dataclass
     class Options(BaseCommand.Options):
         ... optional extra fields etc ...
 
 *Method `BaseCommandOptions.__call__(self, **updates)`*:
 Calling the options object returns a context manager whose
-value is a copy of the options with any `suboptions` applied.
+value is a shallow copy of the options with any `suboptions` applied.
 
 Example showing the semantics:
 
     >>> from cs.cmdutils import BaseCommandOptions
-    >>> options = BaseCommandOptions(x=1)
+    >>> @dataclass
+    ... class DemoOptions(BaseCommandOptions):
+    ...   x: int = 0
+    ...
+    >>> options = DemoOptions(x=1)
     >>> assert options.x == 1
     >>> assert not options.verbose
     >>> with options(verbose=True) as subopts:
     ...     assert options is not subopts
     ...     assert options.x == 1
     ...     assert not options.verbose
     ...     assert subopts.x == 1
@@ -555,14 +586,19 @@
     COMMON_OPT_SPECS = dict(
         e='ssh_exe',
         h_='hashname',
         H_='hashindex_exe',
         **BaseCommand.Options.COMMON_OPT_SPECS,
     )
 
+*Method `BaseCommandOptions.update(self, **updates)`*:
+Modify the options in place with the mapping `updates`.
+It would be more normal to call the options in a `with` statement
+as shown for `__call__`.
+
 ## Function `docmd(dofunc)`
 
 Decorator for `cmd.Cmd` subclass methods
 to supply some basic quality of service.
 
 This decorator:
 - wraps the function call in a `cs.pfx.Pfx` for context
@@ -617,14 +653,19 @@
             print("doing f with x =", x)
         ....
 
 # Release Log
 
 
 
+*Release 20240422*:
+* BaseCommandOptions.popopts: return the dict from BaseCommand.popopts().
+* BaseCommand.apply_preargv: apply the default options supported by self.options.
+* BaseCommandOptions.update(mapping) method, useful for dropping subcommand-specific defaults onto the options ahead of the local popopts() call.
+
 *Release 20240412*:
 * BaseCommand.run_context: do not store .upd and .runstate on the options (it confuses options in subcommands and we have @uses_runstate and @uses_upd forthis anyway these days).
 * BaseCommand.run_context: catch SIGQUIT, present the default handler as BaseCommand.handle_signal.
 
 *Release 20240316*:
 * New @uses_cmd_options decorator to provide an "options" parameter being the prevailing BaseCommandOptions instance.
 * BaseCommandOptions.popopts: get common options from BaseCommandOptions.COMMON_OPT_SPECS.
@@ -793,7 +834,8 @@
 Minor documentation updates.
 
 *Release 20190617.2*:
 Lint.
 
 *Release 20190617.1*:
 Initial release with @docmd decorator and alpha quality BaseCommand command line assistance class.
+
```

### Comparing `cs.cmdutils-20240412/lib/python/cs/cmdutils.py` & `cs.cmdutils-20240422/lib/python/cs/cmdutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from cs.py.doc import obj_docstring
 from cs.resources import RunState, uses_runstate
 from cs.result import CancellationError
 from cs.threads import HasThreadState, ThreadState
 from cs.typingutils import subtype
 from cs.upd import Upd, uses_upd
 
-__version__ = '20240412'
+__version__ = '20240422'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
@@ -323,24 +323,36 @@
             if not k.startswith('_')
         },
     )
     for k, v in updates.items():
       setattr(copied, k, v)
     return copied
 
+  def update(self, **updates):
+    ''' Modify the options in place with the mapping `updates`.
+        It would be more normal to call the options in a `with` statement
+        as shown for `__call__`.
+    '''
+    for k, v in updates.items():
+      setattr(self, k, v)
+
   # TODO: remove this - the overt make-a-copy-and-with-the-copy is clearer
   @contextmanager
   def __call__(self, **updates):
     ''' Calling the options object returns a context manager whose
-        value is a copy of the options with any `suboptions` applied.
+        value is a shallow copy of the options with any `suboptions` applied.
 
         Example showing the semantics:
 
             >>> from cs.cmdutils import BaseCommandOptions
-            >>> options = BaseCommandOptions(x=1)
+            >>> @dataclass
+            ... class DemoOptions(BaseCommandOptions):
+            ...   x: int = 0
+            ...
+            >>> options = DemoOptions(x=1)
             >>> assert options.x == 1
             >>> assert not options.verbose
             >>> with options(verbose=True) as subopts:
             ...     assert options is not subopts
             ...     assert options.x == 1
             ...     assert not options.verbose
             ...     assert subopts.x == 1
@@ -394,15 +406,15 @@
                 H_='hashindex_exe',
                 **BaseCommand.Options.COMMON_OPT_SPECS,
             )
 
     '''
     for k, v in self.COMMON_OPT_SPECS.items():
       opt_specs.setdefault(k, v)
-    BaseCommand.popopts(argv, self, **opt_specs)
+    return BaseCommand.popopts(argv, self, **opt_specs)
 
 def uses_cmd_options(
     func, cls=BaseCommandOptions, options_param_name='options'
 ):
   ''' A decorator to provide a default parameter containing the
       prevailing `BaseCommandOptions` instance as the `options` keyword
       argument, using the `cs.deco.default_params` decorator factory.
@@ -547,16 +559,18 @@
 
   def __init_subclass__(cls):
     ''' Update subclasses of `BaseCommand`.
 
         Appends the usage message to the class docstring.
     '''
     usage_message = cls.usage_text()
+    # NB: 2 leading lines so that the dedenting preserves the indents for MarkDown.
     usage_doc = (
-        'Command line usage:\n\n    ' + usage_message.replace('\n', '\n    ')
+        'Command line implementation.\n\nUsage summary:\n\n    ' +
+        usage_message.replace('\n', '\n    ')
     )
     cls_doc = obj_docstring(cls)
     cls_doc = cls_doc + '\n\n' + usage_doc if cls_doc else usage_doc
     cls.__doc__ = cls_doc
 
   # pylint: disable=too-many-branches,too-many-statements,too-many-locals
   def __init__(self, argv=None, *, cmd=None, options=None, **kw_options):
@@ -885,16 +899,19 @@
       raise GetoptError("bad options")
 
   # pylint: disable=no-self-use
   def apply_preargv(self, argv):
     ''' Do any preparsing of `argv` before the subcommand/main-args.
         Return the remaining arguments.
 
-        This default implementation returns `argv` unchanged.
+        This default implementation applies the default options
+        supported by `self.options` (an instance of `self.Options`
+        class).
     '''
+    self.options.popopts(argv)
     return argv
 
   class _OptSpec(
       namedtuple('_OptSpec',
                  'help_text, parse, validate, unvalidated_message'),
       Promotable,
   ):
@@ -953,22 +970,22 @@
           unvalidated_message=unvalidated_message,
       )
 
     def parse_value(self, value):
       ''' Parse `value` according to the spec.
           Raises a `GetoptError` for invalid values.
       '''
-      with Pfx("%s %r", self.help_text, value):
-        try:
+      try:
+        with Pfx("%s %r", self.help_text, value):
           value = pfx_call(self.parse, value)
           if self.validate is not None:
             if not pfx_call(self.validate, value):
               raise ValueError(self.unvalidated_message)
-        except ValueError as e:
-          raise GetoptError(str(e))  # pylint: disable=raise-missing-from
+      except ValueError as e:
+        raise GetoptError(str(e)) from e  # pylint: disable=raise-missing-from
       return value
 
   @classmethod
   def poparg(cls, argv: List[str], *a, unpop_on_error=False):
     ''' Pop the leading argument off `argv` and parse it.
         Return the parsed argument.
         Raises `getopt.GetoptError` on a missing or invalid argument.
@@ -1078,94 +1095,110 @@
         * a single letter name specifies a short option
           and a multiletter name specifies a long option
         * options requiring an argument have a trailing underscore
         * options not requiring an argument normally imply a value
           of `True`; if their synonym commences with a dash they will
           imply a value of `False`, for example `n='dry_run',y='-dry_run'`
 
-        As it happens, the `BaseCommandOptions` class provided a `popopts` method
-        which is a shim for this method with `attrfor=self` i.e. the options object.
-        So common use in a command method might look like this:
+        The `BaseCommandOptions` class provides a `popopts` method
+        which is a shim for this method with `attrfor=self` i.e.
+        the options object.
+        So common use in a command method usually looks like this:
 
             class SomeCommand(BaseCommand):
 
                 def cmd_foo(self, argv):
                     options = self.options
                     # accept a -j or --jobs options
-                    options.poopts(argv, jobs=1, j='jobs')
+                    options.popopts(argv, jobs=1, j='jobs')
                     print("jobs =", options.jobs)
 
+        The `self.options` object is preprovided as an instance of
+        the `self.Options` class, which is `BaseCommandOptions` by
+        default. This presupplies support for some basic options
+        like `-v` for "verbose" and so forth, and a subcommand
+        need not describe these in a call to `self.options.popopts()`.
+
         Example:
 
             >>> import os.path
-            >>> options = SimpleNamespace(
-            ...   all=False,
-            ...   jobs=1,
-            ...   number=0,
-            ...   once=False,
-            ...   path=None,
-            ...   trace_exec=True,
-            ...   verbose=False,
-            ...   dry_run=False)
+            >>> from typing import Optional
+            >>> @dataclass
+            ... class DemoOptions(BaseCommandOptions):
+            ...   all: bool = False
+            ...   jobs: int = 1
+            ...   number: int = 0
+            ...   once: bool = False
+            ...   path: Optional[str] = None
+            ...   trace_exec: bool = False
+            ...
+            >>> options = DemoOptions()
             >>> argv = ['-1', '-v', '-y', '-j4', '--path=/foo', 'bah', '-x']
-            >>> opt_dict = BaseCommand.popopts(
+            >>> opt_dict = options.popopts(
             ...   argv,
-            ...   options,
             ...   _1='once',
             ...   a='all',
             ...   j_=('jobs',int),
-            ...   n='dry_run',
-            ...   v='verbose',
             ...   x='-trace_exec',
             ...   y='-dry_run',
             ...   dry_run=None,
             ...   path_=(str, os.path.isabs, 'not an absolute path'),
             ...   verbose=None,
             ... )
             >>> opt_dict
             {'once': True, 'verbose': True, 'dry_run': False, 'jobs': 4, 'path': '/foo'}
-            >>> options
-            namespace(all=False, jobs=4, number=0, once=True, path='/foo', trace_exec=True, verbose=True, dry_run=False)
+            >>> options # doctest: +ELLIPSIS
+            DemoOptions(cmd=None, dry_run=False, force=False, quiet=False, runstate_signals=(...), verbose=True, all=False, jobs=4, number=0, once=True, path='/foo', trace_exec=False)
     '''
     keyfor = {}
     shortopts = ''
     longopts = []
     opt_spec_map = {}
     opt_name_map = {}
     for opt_name, opt_spec in opt_specs.items():
       with Pfx("opt_spec[%r]=%r", opt_name, opt_spec):
         needs_arg = False
+        # leading underscore for numeric options like -1
         if opt_name.startswith('_'):
           opt_name = opt_name[1:]
           if is_identifier(opt_name):
             warning(
                 "unnecessary leading underscore on valid identifier option"
             )
+        # trailing underscore indicates that the option expected an argument
         if opt_name.endswith('_'):
           needs_arg = True
           opt_name = opt_name[:-1]
+        # single character option -x
         if len(opt_name) == 1:
           opt = '-' + opt_name
           shortopts += opt_name
           if needs_arg:
             shortopts += ':'
+        # long option
         elif len(opt_name) > 1:
           opt_dashed = opt_name.replace('_', '-')
           opt = '--' + opt_dashed
           longopts.append(opt_dashed + '=' if needs_arg else opt_dashed)
           default_help_text = opt
         else:
           raise ValueError("unexpected opt_name %s" % (r(opt_name),))
+        # construct an option specification list containing:
+        #   [opt_name:str] [help_text:str] [parse:Callable [validate:Callable [invalid_msg:str]]]
         if opt_spec is None:
+          # default opt_spec: opt citation and type str
           specs = [opt_name, str]
         elif isinstance(opt_spec, (list, tuple)):
+          # list or tuple: copyt to a list
           specs = list(opt_spec)
         else:
+          # promote scaler to single element list
           specs = [opt_spec]
         if specs:
+          # see if the leading spec is an option citation
           spec0 = specs[0]
           if isinstance(spec0, str) and (is_identifier(spec0) or
                                          (spec0.startswith('-')
                                           and is_identifier(spec0[1:]))):
             opt_name = specs[0]
             if len(specs) > 1 and isinstance(specs[1], str):
               specs.pop(0)
```

### Comparing `cs.cmdutils-20240412/lib/python/cs.cmdutils.egg-info/PKG-INFO` & `cs.cmdutils-20240422/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,90 @@
-Metadata-Version: 2.1
-Name: cs.cmdutils
-Version: 20240412
-Summary: Convenience functions for working with the Cmd module, the BaseCommand class for constructing command line programmes, and other command line related stuff.
-Author-email: Cameron Simpson <cs@cskk.id.au>
-License: GNU General Public License v3 or later (GPLv3+)
-Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
-Keywords: python2,python3
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Description-Content-Type: text/markdown
+[project]
+name = "cs.cmdutils"
+description = "Convenience functions for working with the Cmd module, the BaseCommand class for constructing command line programmes, and other command line related stuff."
+authors = [
+    { name = "Cameron Simpson", email = "cs@cskk.id.au" },
+]
+keywords = [
+    "python2",
+    "python3",
+]
+dependencies = [
+    "cs.context>=20240412",
+    "cs.deco>=20240412",
+    "cs.lex>=20240316",
+    "cs.logutils>=20230212",
+    "cs.pfx>=20240412",
+    "cs.py.doc>=20240422",
+    "cs.resources>=20240422",
+    "cs.result>=20240412",
+    "cs.threads>=20240422",
+    "cs.typingutils>=20230331",
+    "cs.upd>=20240412",
+    "typeguard",
+]
+classifiers = [
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Developers",
+    "Operating System :: OS Independent",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+]
+version = "20240422"
 
+[project.license]
+text = "GNU General Public License v3 or later (GPLv3+)"
+
+[project.urls]
+URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
+
+[project.readme]
+text = """
 Convenience functions for working with the Cmd module,
 the BaseCommand class for constructing command line programmes,
 and other command line related stuff.
 
-*Latest release 20240412*:
-* BaseCommand.run_context: do not store .upd and .runstate on the options (it confuses options in subcommands and we have @uses_runstate and @uses_upd forthis anyway these days).
-* BaseCommand.run_context: catch SIGQUIT, present the default handler as BaseCommand.handle_signal.
+*Latest release 20240422*:
+* BaseCommandOptions.popopts: return the dict from BaseCommand.popopts().
+* BaseCommand.apply_preargv: apply the default options supported by self.options.
+* BaseCommandOptions.update(mapping) method, useful for dropping subcommand-specific defaults onto the options ahead of the local popopts() call.
 
 ## Class `BaseCommand`
 
 A base class for handling nestable command lines.
 
 This class provides the basic parse and dispatch mechanisms
 for command lines.
 To implement a command line
 one instantiates a subclass of `BaseCommand`:
 
     class MyCommand(BaseCommand):
         GETOPT_SPEC = 'ab:c'
-        USAGE_FORMAT = r"""Usage: {cmd} [-a] [-b bvalue] [-c] [--] arguments...
+        USAGE_FORMAT = r\"\"\"Usage: {cmd} [-a] [-b bvalue] [-c] [--] arguments...
           -a    Do it all.
           -b    But using bvalue.
           -c    The 'c' option!
-        """
+        \"\"\"
         ...
 
 and provides either a `main` method if the command has no subcommands
 or a suite of `cmd_`*subcommand* methods, one per subcommand.
 
 Running a command is done by:
 
     MyCommand(argv).run()
 
 Modules which implement a command line mode generally look like this:
 
     ... imports etc ...
     def main(argv=None, **run_kw):
-        """ The command line mode.
-        """
+        \"\"\" The command line mode.
+        \"\"\"
         return MyCommand(argv).run(**run_kw)
     ... other code ...
     class MyCommand(BaseCommand):
     ... other code ...
     if __name__ == '__main__':
         sys.exit(main(sys.argv))
 
@@ -80,20 +106,20 @@
 Returning to methods, if there is a paragraph in the method docstring
 commencing with `Usage:`
 then that paragraph is incorporated automatically
 into the main usage message.
 Example:
 
     def cmd_ls(self, argv):
-        """ Usage: {cmd} [paths...]
+        \"\"\" Usage: {cmd} [paths...]
               Emit a listing for the named paths.
 
             Further docstring non-usage information here.
-        """
-        ... do the "ls" subcommand ...
+        \"\"\"
+        ... do the \"ls\" subcommand ...
 
 The subclass is customised by overriding the following methods:
 * `apply_opt(opt,val)`:
   apply an individual getopt global command line option
   to `self.options`.
 * `apply_opts(opts)`:
   apply the `opts` to `self.options`.
@@ -201,15 +227,17 @@
 Subclasses can override this
 but it is usually easier to override `apply_opt(opt,val)`.
 
 *Method `BaseCommand.apply_preargv(self, argv)`*:
 Do any preparsing of `argv` before the subcommand/main-args.
 Return the remaining arguments.
 
-This default implementation returns `argv` unchanged.
+This default implementation applies the default options
+supported by `self.options` (an instance of `self.Options`
+class).
 
 *Method `BaseCommand.cmd_help(argv)`*:
 Usage: {cmd} [-l] [subcommand-names...]
 Print help for subcommands.
 This outputs the full help for the named subcommands,
 or the short help for all subcommands if no names are specified.
 -l  Long help even if no subcommand-names provided.
@@ -248,15 +276,15 @@
 this can be overridden with a method which just returns `False`.
 
 Otherwise,
 the handler may perform any suitable action
 and return `True` to contain the exception
 or `False` to cause the exception to be reraised.
 
-*Method `BaseCommand.handle_signal(self, sig, frame, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x10d5b1d80>)`*:
+*Method `BaseCommand.handle_signal(self, sig, frame, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x104df9f30>)`*:
 The default signal handler, which cancels the default `RunState`.
 
 *Method `BaseCommand.poparg(argv: List[str], *a, unpop_on_error=False)`*:
 Pop the leading argument off `argv` and parse it.
 Return the parsed argument.
 Raises `getopt.GetoptError` on a missing or invalid argument.
 
@@ -281,49 +309,49 @@
   for values failing the validation
 * `unpop_on_error`: optional keyword parameter, default `False`;
   if true then push the argument back onto the front of `argv`
   if it fails to parse; `GetoptError` is still raised
 
 Typical use inside a `main` or `cmd_*` method might look like:
 
-    self.options.word = self.poparg(argv, int, "a count value")
+    self.options.word = self.poparg(argv, int, \"a count value\")
     self.options.word = self.poparg(
-        argv, int, "a count value",
-       lambda count: count > 0, "count should be positive")
+        argv, int, \"a count value\",
+       lambda count: count > 0, \"count should be positive\")
 
 Because it raises `GetoptError` on a bad argument
 the normal usage message failure mode follows automatically.
 
 Demonstration:
 
     >>> argv = ['word', '3', 'nine', '4']
-    >>> BaseCommand.poparg(argv, "word to process")
+    >>> BaseCommand.poparg(argv, \"word to process\")
     'word'
-    >>> BaseCommand.poparg(argv, int, "count value")
+    >>> BaseCommand.poparg(argv, int, \"count value\")
     3
-    >>> BaseCommand.poparg(argv, float, "length")
+    >>> BaseCommand.poparg(argv, float, \"length\")
     Traceback (most recent call last):
       ...
     getopt.GetoptError: length 'nine': float('nine'): could not convert string to float: 'nine'
-    >>> BaseCommand.poparg(argv, float, "width", lambda width: width > 5)
+    >>> BaseCommand.poparg(argv, float, \"width\", lambda width: width > 5)
     Traceback (most recent call last):
       ...
     getopt.GetoptError: width '4': invalid value
-    >>> BaseCommand.poparg(argv, float, "length")
+    >>> BaseCommand.poparg(argv, float, \"length\")
     Traceback (most recent call last):
       ...
     getopt.GetoptError: length: missing argument
     >>> argv = ['-5', 'zz']
-    >>> BaseCommand.poparg(argv, float, "size", lambda f: f>0, "size should be >0")
+    >>> BaseCommand.poparg(argv, float, \"size\", lambda f: f>0, \"size should be >0\")
     Traceback (most recent call last):
       ...
     getopt.GetoptError: size '-5': size should be >0
     >>> argv  # -5 was still consumed
     ['zz']
-    >>> BaseCommand.poparg(argv, float, "size2", unpop_on_error=True)
+    >>> BaseCommand.poparg(argv, float, \"size2\", unpop_on_error=True)
     Traceback (most recent call last):
       ...
     getopt.GetoptError: size2 'zz': float('zz'): could not convert string to float: 'zz'
     >>> argv  # zz was pushed back
     ['zz']
 
 *Method `BaseCommand.popopts(argv, attrfor=None, **opt_specs)`*:
@@ -347,57 +375,63 @@
 * a single letter name specifies a short option
   and a multiletter name specifies a long option
 * options requiring an argument have a trailing underscore
 * options not requiring an argument normally imply a value
   of `True`; if their synonym commences with a dash they will
   imply a value of `False`, for example `n='dry_run',y='-dry_run'`
 
-As it happens, the `BaseCommandOptions` class provided a `popopts` method
-which is a shim for this method with `attrfor=self` i.e. the options object.
-So common use in a command method might look like this:
+The `BaseCommandOptions` class provides a `popopts` method
+which is a shim for this method with `attrfor=self` i.e.
+the options object.
+So common use in a command method usually looks like this:
 
     class SomeCommand(BaseCommand):
 
         def cmd_foo(self, argv):
             options = self.options
             # accept a -j or --jobs options
-            options.poopts(argv, jobs=1, j='jobs')
-            print("jobs =", options.jobs)
+            options.popopts(argv, jobs=1, j='jobs')
+            print(\"jobs =\", options.jobs)
+
+The `self.options` object is preprovided as an instance of
+the `self.Options` class, which is `BaseCommandOptions` by
+default. This presupplies support for some basic options
+like `-v` for \"verbose\" and so forth, and a subcommand
+need not describe these in a call to `self.options.popopts()`.
 
 Example:
 
     >>> import os.path
-    >>> options = SimpleNamespace(
-    ...   all=False,
-    ...   jobs=1,
-    ...   number=0,
-    ...   once=False,
-    ...   path=None,
-    ...   trace_exec=True,
-    ...   verbose=False,
-    ...   dry_run=False)
+    >>> from typing import Optional
+    >>> @dataclass
+    ... class DemoOptions(BaseCommandOptions):
+    ...   all: bool = False
+    ...   jobs: int = 1
+    ...   number: int = 0
+    ...   once: bool = False
+    ...   path: Optional[str] = None
+    ...   trace_exec: bool = False
+    ...
+    >>> options = DemoOptions()
     >>> argv = ['-1', '-v', '-y', '-j4', '--path=/foo', 'bah', '-x']
-    >>> opt_dict = BaseCommand.popopts(
+    >>> opt_dict = options.popopts(
     ...   argv,
-    ...   options,
     ...   _1='once',
     ...   a='all',
     ...   j_=('jobs',int),
-    ...   n='dry_run',
-    ...   v='verbose',
     ...   x='-trace_exec',
     ...   y='-dry_run',
     ...   dry_run=None,
     ...   path_=(str, os.path.isabs, 'not an absolute path'),
     ...   verbose=None,
     ... )
     >>> opt_dict
     {'once': True, 'verbose': True, 'dry_run': False, 'jobs': 4, 'path': '/foo'}
-    >>> options
-    namespace(all=False, jobs=4, number=0, once=True, path='/foo', trace_exec=True, verbose=True, dry_run=False)
+    >>> options # doctest: +ELLIPSIS
+    DemoOptions(cmd=None, dry_run=False, force=False, quiet=False, runstate_signals=(...), verbose=True, all=False, jobs=4, number=0, once=True, path='/foo', trace_exec=False)
 
 *Method `BaseCommand.repl(self, *argv, banner=None, local=None)`*:
 Run an interactive Python prompt with some predefined local names.
 Aka REPL (Read Evaluate Print Loop).
 
 Parameters:
 * `argv`: any notional command line arguments
@@ -412,17 +446,17 @@
 * the attributes of `self`
 
 This is not presented automatically as a subcommand, but
 commands wishing such a command should provide something
 like this:
 
     def cmd_repl(self, argv):
-        """ Usage: {cmd}
+        \"\"\" Usage: {cmd}
               Run an interactive Python prompt with some predefined local names.
-        """
+        \"\"\"
         return self.repl(*argv)
 
 *Method `BaseCommand.run(self, **kw_options)`*:
 Run a command.
 Returns the exit status of the command.
 May raise `GetoptError` from subcommands.
 
@@ -438,15 +472,15 @@
 Otherwise `self.main(argv)` is called
 and its value returned.
 
 If the command implementation requires some setup or teardown
 then this may be provided by the `run_context()`
 context manager method.
 
-*Method `BaseCommand.run_context(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x10d48e290>, **kw)`*:
+*Method `BaseCommand.run_context(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x104cea3b0>, **kw)`*:
 The context manager which surrounds `main` or `cmd_`*subcmd*.
 
 This default does several things, and subclasses should
 override it like this:
 
     @contextmanager
     def run_context(self):
@@ -467,15 +501,15 @@
 
 *Method `BaseCommand.subcommands()`*:
 Return a mapping of subcommand names to subcommand specifications
 for class attributes which commence with `cls.SUBCOMMAND_METHOD_PREFIX`
 by default `'cmd_'`.
 
 *Method `BaseCommand.usage_text(*, cmd=None, format_mapping=None, subcmd=None, short=False)`*:
-Compute the "Usage:" message for this class
+Compute the \"Usage:\" message for this class
 from the top level `USAGE_FORMAT`
 and the `'Usage:'`-containing docstrings of its `cmd_*` methods.
 
 Parameters:
 * `cmd`: optional command name, default derived from the class name
 * `format_mapping`: an optional format mapping for filling
   in format strings in the usage text
@@ -515,20 +549,24 @@
 
     @dataclass
     class Options(BaseCommand.Options):
         ... optional extra fields etc ...
 
 *Method `BaseCommandOptions.__call__(self, **updates)`*:
 Calling the options object returns a context manager whose
-value is a copy of the options with any `suboptions` applied.
+value is a shallow copy of the options with any `suboptions` applied.
 
 Example showing the semantics:
 
     >>> from cs.cmdutils import BaseCommandOptions
-    >>> options = BaseCommandOptions(x=1)
+    >>> @dataclass
+    ... class DemoOptions(BaseCommandOptions):
+    ...   x: int = 0
+    ...
+    >>> options = DemoOptions(x=1)
     >>> assert options.x == 1
     >>> assert not options.verbose
     >>> with options(verbose=True) as subopts:
     ...     assert options is not subopts
     ...     assert options.x == 1
     ...     assert not options.verbose
     ...     assert subopts.x == 1
@@ -557,15 +595,15 @@
     def cmd_foo(self, argv):
         self.options.popopts(
             c_='config',
             l='long',
             x='trace',
         )
         if self.options.dry_run:
-            print("dry run!")
+            print(\"dry run!\")
 
 The class attribute `COMMON_OPT_SPECS` is a mapping of
 options which are always supported. `BaseCommandOptions`
 has: `COMMON_OPT_SPECS={'n': 'dry_run', 'q': 'quiet', 'v': 'verbose'}`.
 
 A subclass with more common options might extend this like so,
 from `cs.hashindex`:
@@ -573,14 +611,19 @@
     COMMON_OPT_SPECS = dict(
         e='ssh_exe',
         h_='hashname',
         H_='hashindex_exe',
         **BaseCommand.Options.COMMON_OPT_SPECS,
     )
 
+*Method `BaseCommandOptions.update(self, **updates)`*:
+Modify the options in place with the mapping `updates`.
+It would be more normal to call the options in a `with` statement
+as shown for `__call__`.
+
 ## Function `docmd(dofunc)`
 
 Decorator for `cmd.Cmd` subclass methods
 to supply some basic quality of service.
 
 This decorator:
 - wraps the function call in a `cs.pfx.Pfx` for context
@@ -617,38 +660,43 @@
   provided its `cls.Options` class is used.
 * `options_param_name`: the parameter name to provide, default `options`
 
 Examples:
 
     @uses_cmd_options
     def f(x,*,options):
-        """ Run directly from the prevailing options. """
+        \"\"\" Run directly from the prevailing options. \"\"\"
         if options.verbose:
-            print("doing f with x =", x)
+            print(\"doing f with x =\", x)
         ....
 
     @uses_cmd_options
     def f(x,*,verbose=None,options):
-        """ Get defaults from the prevailing options. """
+        \"\"\" Get defaults from the prevailing options. \"\"\"
         if verbose is None:
             verbose = options.verbose
         if verbose:
-            print("doing f with x =", x)
+            print(\"doing f with x =\", x)
         ....
 
 # Release Log
 
 
 
+*Release 20240422*:
+* BaseCommandOptions.popopts: return the dict from BaseCommand.popopts().
+* BaseCommand.apply_preargv: apply the default options supported by self.options.
+* BaseCommandOptions.update(mapping) method, useful for dropping subcommand-specific defaults onto the options ahead of the local popopts() call.
+
 *Release 20240412*:
 * BaseCommand.run_context: do not store .upd and .runstate on the options (it confuses options in subcommands and we have @uses_runstate and @uses_upd forthis anyway these days).
 * BaseCommand.run_context: catch SIGQUIT, present the default handler as BaseCommand.handle_signal.
 
 *Release 20240316*:
-* New @uses_cmd_options decorator to provide an "options" parameter being the prevailing BaseCommandOptions instance.
+* New @uses_cmd_options decorator to provide an \"options\" parameter being the prevailing BaseCommandOptions instance.
 * BaseCommandOptions.popopts: get common options from BaseCommandOptions.COMMON_OPT_SPECS.
 
 *Release 20240211*:
 * Include the first sentence of the subcommand description in the short help.
 * BaseCommandOptions: move the runstate_signals into this directly.
 * BaseCommand: move the run() options stuff into run_context() and have it work on a copy of the original options.
 * BaseCommandCmd: implement get_names(), provide docstrings for the do_* attributes, thus help.
@@ -703,27 +751,27 @@
 * BaseCommand: new poparg(argv,...) compact validating argument consumer.
 * BaseCommand: drop run_argv, provided no utility.
 * BaseCommand.run: get the RunState signal list from self.options.runstate_signals.
 * BaseCommand.apply_opts: support multiple individual options raising GetoptError, as I hate commands which abort at the first bad option.
 * Assorted other small things.
 
 *Release 20220429*:
-* BaseCommand: fold dots in argv[0] into underscores, supports subcommands like "setup.py".
+* BaseCommand: fold dots in argv[0] into underscores, supports subcommands like \"setup.py\".
 * BaseCommand: new popargv(argv[,help_text[,parse[,validate[,unvalidated_message]]]]) helper class method.
 * BaseCommand: accept dashed-form of the underscored_form subcommand name.
 * BaseCommand: new self.options.runstate_signals=SIGINT,SIGTERM specifying singals to catch-and-cancel, shuffle run() context managers.
 
 *Release 20220318*:
 BaseCommand.__init__: handle main() method in the New Scheme.
 
 *Release 20220315*:
 _BaseSubCommand.__init__: hook in the class USAGE_KEYWORDS for methods.
 
 *Release 20220311*:
-BaseCommand: big refactor of subcommand internals and make the "cmd_foo=FooCommand" implementation work properly.
+BaseCommand: big refactor of subcommand internals and make the \"cmd_foo=FooCommand\" implementation work properly.
 
 *Release 20211208*:
 BaseCommand: better handle an unknown subcommand.
 
 *Release 20210927*:
 * Usage: show only the per subcommand usage for in-subcommand GetoptError.
 * Usage: show terse usage when the subcommand cannot be recognised.
@@ -738,57 +786,57 @@
 
 *Release 20210809*:
 Bugfix BaseCommand.cmd_help for modern API.
 
 *Release 20210731*:
 * BaseCommand.run: apply optional keyword arguments to self.options during the run.
 * Look for self.SUBCOMMAND_ARGV_DEFAULT if no subcommand is supplied.
-* Bugfix case for "main" method and no "cmd_*" methods.
+* Bugfix case for \"main\" method and no \"cmd_*\" methods.
 * Bugfix BaseCommand.cmd_help.
 
 *Release 20210420*:
 * BaseCommand.getopt_error_handler: replace error print() with warning().
 * Docstring improvements.
 
 *Release 20210407.1*:
 BaseCommand: bugfix for __init_subclass__ docstring update.
 
 *Release 20210407*:
 * BaseCommand.__init_subclass__: behave sanely if the subclass has no initial __doc__.
-* BaseCommand: new .run_argv convenience method, obviates the "def main" boilerplate.
+* BaseCommand: new .run_argv convenience method, obviates the \"def main\" boilerplate.
 
 *Release 20210404*:
 BaseCommand subclasses: automatically add the main usage message to the subclass docstring.
 
 *Release 20210306*:
 * BREAKING CHANGE: rework BaseCommand as a more normal class instantiated with argv and with most methods being instance methods, getting the former `options` parameter from self.options.
 * BaseCommand: provide default `apply_opt` and `apply_opts` methods; subclasses will generally just override the former.
 
 *Release 20210123*:
 BaseCommand: propagate the format mapping (cmd, USAGE_KEYWORDS) to the subusage generation.
 
 *Release 20201102*:
-* BaseCommand.cmd_help: supply usage only for "all commands", full docstring for specified commands.
+* BaseCommand.cmd_help: supply usage only for \"all commands\", full docstring for specified commands.
 * BaseCommand: honour presupplied options.log_level.
 * BaseCommand.usage_text: handle missing USAGE_FORMAT better.
 * BaseCommand.run: provide options.upd.
 * BaseCommand subclasses may now override BaseCommand.OPTIONS_CLASS (default SimpleNamespace) in order to provide convenience methods on the options.
 * BaseCommand.run: separate variable for subcmd with dash translated to underscore to match method names.
 * Minor fixes.
 
 *Release 20200615*:
-BaseCommand.usage_text: do not mention the "help" command if it is the only subcommand (it won't be available if there are no other subcommands).
+BaseCommand.usage_text: do not mention the \"help\" command if it is the only subcommand (it won't be available if there are no other subcommands).
 
 *Release 20200521.1*:
 Fix DISTINFO.install_requires.
 
 *Release 20200521*:
 * BaseCommand.run: support using BaseCommand subclasses as cmd_* names to make it easy to nest BaseCommands.
 * BaseCommand: new hack_postopts_argv method called after parsing the main command line options, for inferring subcommands or the like.
-* BaseCommand: extract "Usage:" paragraphs from subcommand method docstrings to build the main usage message.
+* BaseCommand: extract \"Usage:\" paragraphs from subcommand method docstrings to build the main usage message.
 * BaseCommand: new cmd_help default command.
 * Assorted bugfixes and small improvements.
 
 *Release 20200318*:
 * BaseCommand.run: make argv optional, get additional usage keywords from self.USAGE_KEYWORDS.
 * @BaseCommand.add_usage_to_docstring: honour cls.USAGE_KEYWORDS.
 * BaseCommand: do not require GETOPT_SPEC for commands with no defined options.
@@ -810,9 +858,25 @@
 *Release 20190619*:
 Minor documentation updates.
 
 *Release 20190617.2*:
 Lint.
 
 *Release 20190617.1*:
-Initial release with @docmd decorator and alpha quality BaseCommand command line assistance class.
+Initial release with @docmd decorator and alpha quality BaseCommand command line assistance class."""
+content-type = "text/markdown"
+
+[build-system]
+build-backend = "setuptools.build_meta"
+requires = [
+    "setuptools >= 61.2",
+    "trove-classifiers",
+    "wheel",
+]
+
+[tool.setuptools]
+py-modules = [
+    "cs.cmdutils",
+]
 
+[tool.setuptools.package-dir]
+"" = "lib/python"
```

### Comparing `cs.cmdutils-20240412/pyproject.toml` & `cs.cmdutils-20240422/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,89 +1,47 @@
-[project]
-name = "cs.cmdutils"
-description = "Convenience functions for working with the Cmd module, the BaseCommand class for constructing command line programmes, and other command line related stuff."
-authors = [
-    { name = "Cameron Simpson", email = "cs@cskk.id.au" },
-]
-keywords = [
-    "python2",
-    "python3",
-]
-dependencies = [
-    "cs.context>=20240412",
-    "cs.deco>=20240412",
-    "cs.lex>=20240316",
-    "cs.logutils>=20230212",
-    "cs.pfx>=20240412",
-    "cs.py.doc>=20240412",
-    "cs.resources>=20240412",
-    "cs.result>=20240412",
-    "cs.threads>=20240412",
-    "cs.typingutils>=20230331",
-    "cs.upd>=20240412",
-    "typeguard",
-]
-classifiers = [
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Development Status :: 4 - Beta",
-    "Intended Audience :: Developers",
-    "Operating System :: OS Independent",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-]
-version = "20240412"
-
-[project.license]
-text = "GNU General Public License v3 or later (GPLv3+)"
-
-[project.urls]
-URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
-
-[project.readme]
-text = """
 Convenience functions for working with the Cmd module,
 the BaseCommand class for constructing command line programmes,
 and other command line related stuff.
 
-*Latest release 20240412*:
-* BaseCommand.run_context: do not store .upd and .runstate on the options (it confuses options in subcommands and we have @uses_runstate and @uses_upd forthis anyway these days).
-* BaseCommand.run_context: catch SIGQUIT, present the default handler as BaseCommand.handle_signal.
+*Latest release 20240422*:
+* BaseCommandOptions.popopts: return the dict from BaseCommand.popopts().
+* BaseCommand.apply_preargv: apply the default options supported by self.options.
+* BaseCommandOptions.update(mapping) method, useful for dropping subcommand-specific defaults onto the options ahead of the local popopts() call.
 
 ## Class `BaseCommand`
 
 A base class for handling nestable command lines.
 
 This class provides the basic parse and dispatch mechanisms
 for command lines.
 To implement a command line
 one instantiates a subclass of `BaseCommand`:
 
     class MyCommand(BaseCommand):
         GETOPT_SPEC = 'ab:c'
-        USAGE_FORMAT = r\"\"\"Usage: {cmd} [-a] [-b bvalue] [-c] [--] arguments...
+        USAGE_FORMAT = r"""Usage: {cmd} [-a] [-b bvalue] [-c] [--] arguments...
           -a    Do it all.
           -b    But using bvalue.
           -c    The 'c' option!
-        \"\"\"
+        """
         ...
 
 and provides either a `main` method if the command has no subcommands
 or a suite of `cmd_`*subcommand* methods, one per subcommand.
 
 Running a command is done by:
 
     MyCommand(argv).run()
 
 Modules which implement a command line mode generally look like this:
 
     ... imports etc ...
     def main(argv=None, **run_kw):
-        \"\"\" The command line mode.
-        \"\"\"
+        """ The command line mode.
+        """
         return MyCommand(argv).run(**run_kw)
     ... other code ...
     class MyCommand(BaseCommand):
     ... other code ...
     if __name__ == '__main__':
         sys.exit(main(sys.argv))
 
@@ -105,20 +63,20 @@
 Returning to methods, if there is a paragraph in the method docstring
 commencing with `Usage:`
 then that paragraph is incorporated automatically
 into the main usage message.
 Example:
 
     def cmd_ls(self, argv):
-        \"\"\" Usage: {cmd} [paths...]
+        """ Usage: {cmd} [paths...]
               Emit a listing for the named paths.
 
             Further docstring non-usage information here.
-        \"\"\"
-        ... do the \"ls\" subcommand ...
+        """
+        ... do the "ls" subcommand ...
 
 The subclass is customised by overriding the following methods:
 * `apply_opt(opt,val)`:
   apply an individual getopt global command line option
   to `self.options`.
 * `apply_opts(opts)`:
   apply the `opts` to `self.options`.
@@ -226,15 +184,17 @@
 Subclasses can override this
 but it is usually easier to override `apply_opt(opt,val)`.
 
 *Method `BaseCommand.apply_preargv(self, argv)`*:
 Do any preparsing of `argv` before the subcommand/main-args.
 Return the remaining arguments.
 
-This default implementation returns `argv` unchanged.
+This default implementation applies the default options
+supported by `self.options` (an instance of `self.Options`
+class).
 
 *Method `BaseCommand.cmd_help(argv)`*:
 Usage: {cmd} [-l] [subcommand-names...]
 Print help for subcommands.
 This outputs the full help for the named subcommands,
 or the short help for all subcommands if no names are specified.
 -l  Long help even if no subcommand-names provided.
@@ -273,15 +233,15 @@
 this can be overridden with a method which just returns `False`.
 
 Otherwise,
 the handler may perform any suitable action
 and return `True` to contain the exception
 or `False` to cause the exception to be reraised.
 
-*Method `BaseCommand.handle_signal(self, sig, frame, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x10d5b1d80>)`*:
+*Method `BaseCommand.handle_signal(self, sig, frame, *, runstate: Optional[cs.resources.RunState] = <function <lambda> at 0x104df9f30>)`*:
 The default signal handler, which cancels the default `RunState`.
 
 *Method `BaseCommand.poparg(argv: List[str], *a, unpop_on_error=False)`*:
 Pop the leading argument off `argv` and parse it.
 Return the parsed argument.
 Raises `getopt.GetoptError` on a missing or invalid argument.
 
@@ -306,49 +266,49 @@
   for values failing the validation
 * `unpop_on_error`: optional keyword parameter, default `False`;
   if true then push the argument back onto the front of `argv`
   if it fails to parse; `GetoptError` is still raised
 
 Typical use inside a `main` or `cmd_*` method might look like:
 
-    self.options.word = self.poparg(argv, int, \"a count value\")
+    self.options.word = self.poparg(argv, int, "a count value")
     self.options.word = self.poparg(
-        argv, int, \"a count value\",
-       lambda count: count > 0, \"count should be positive\")
+        argv, int, "a count value",
+       lambda count: count > 0, "count should be positive")
 
 Because it raises `GetoptError` on a bad argument
 the normal usage message failure mode follows automatically.
 
 Demonstration:
 
     >>> argv = ['word', '3', 'nine', '4']
-    >>> BaseCommand.poparg(argv, \"word to process\")
+    >>> BaseCommand.poparg(argv, "word to process")
     'word'
-    >>> BaseCommand.poparg(argv, int, \"count value\")
+    >>> BaseCommand.poparg(argv, int, "count value")
     3
-    >>> BaseCommand.poparg(argv, float, \"length\")
+    >>> BaseCommand.poparg(argv, float, "length")
     Traceback (most recent call last):
       ...
     getopt.GetoptError: length 'nine': float('nine'): could not convert string to float: 'nine'
-    >>> BaseCommand.poparg(argv, float, \"width\", lambda width: width > 5)
+    >>> BaseCommand.poparg(argv, float, "width", lambda width: width > 5)
     Traceback (most recent call last):
       ...
     getopt.GetoptError: width '4': invalid value
-    >>> BaseCommand.poparg(argv, float, \"length\")
+    >>> BaseCommand.poparg(argv, float, "length")
     Traceback (most recent call last):
       ...
     getopt.GetoptError: length: missing argument
     >>> argv = ['-5', 'zz']
-    >>> BaseCommand.poparg(argv, float, \"size\", lambda f: f>0, \"size should be >0\")
+    >>> BaseCommand.poparg(argv, float, "size", lambda f: f>0, "size should be >0")
     Traceback (most recent call last):
       ...
     getopt.GetoptError: size '-5': size should be >0
     >>> argv  # -5 was still consumed
     ['zz']
-    >>> BaseCommand.poparg(argv, float, \"size2\", unpop_on_error=True)
+    >>> BaseCommand.poparg(argv, float, "size2", unpop_on_error=True)
     Traceback (most recent call last):
       ...
     getopt.GetoptError: size2 'zz': float('zz'): could not convert string to float: 'zz'
     >>> argv  # zz was pushed back
     ['zz']
 
 *Method `BaseCommand.popopts(argv, attrfor=None, **opt_specs)`*:
@@ -372,57 +332,63 @@
 * a single letter name specifies a short option
   and a multiletter name specifies a long option
 * options requiring an argument have a trailing underscore
 * options not requiring an argument normally imply a value
   of `True`; if their synonym commences with a dash they will
   imply a value of `False`, for example `n='dry_run',y='-dry_run'`
 
-As it happens, the `BaseCommandOptions` class provided a `popopts` method
-which is a shim for this method with `attrfor=self` i.e. the options object.
-So common use in a command method might look like this:
+The `BaseCommandOptions` class provides a `popopts` method
+which is a shim for this method with `attrfor=self` i.e.
+the options object.
+So common use in a command method usually looks like this:
 
     class SomeCommand(BaseCommand):
 
         def cmd_foo(self, argv):
             options = self.options
             # accept a -j or --jobs options
-            options.poopts(argv, jobs=1, j='jobs')
-            print(\"jobs =\", options.jobs)
+            options.popopts(argv, jobs=1, j='jobs')
+            print("jobs =", options.jobs)
+
+The `self.options` object is preprovided as an instance of
+the `self.Options` class, which is `BaseCommandOptions` by
+default. This presupplies support for some basic options
+like `-v` for "verbose" and so forth, and a subcommand
+need not describe these in a call to `self.options.popopts()`.
 
 Example:
 
     >>> import os.path
-    >>> options = SimpleNamespace(
-    ...   all=False,
-    ...   jobs=1,
-    ...   number=0,
-    ...   once=False,
-    ...   path=None,
-    ...   trace_exec=True,
-    ...   verbose=False,
-    ...   dry_run=False)
+    >>> from typing import Optional
+    >>> @dataclass
+    ... class DemoOptions(BaseCommandOptions):
+    ...   all: bool = False
+    ...   jobs: int = 1
+    ...   number: int = 0
+    ...   once: bool = False
+    ...   path: Optional[str] = None
+    ...   trace_exec: bool = False
+    ...
+    >>> options = DemoOptions()
     >>> argv = ['-1', '-v', '-y', '-j4', '--path=/foo', 'bah', '-x']
-    >>> opt_dict = BaseCommand.popopts(
+    >>> opt_dict = options.popopts(
     ...   argv,
-    ...   options,
     ...   _1='once',
     ...   a='all',
     ...   j_=('jobs',int),
-    ...   n='dry_run',
-    ...   v='verbose',
     ...   x='-trace_exec',
     ...   y='-dry_run',
     ...   dry_run=None,
     ...   path_=(str, os.path.isabs, 'not an absolute path'),
     ...   verbose=None,
     ... )
     >>> opt_dict
     {'once': True, 'verbose': True, 'dry_run': False, 'jobs': 4, 'path': '/foo'}
-    >>> options
-    namespace(all=False, jobs=4, number=0, once=True, path='/foo', trace_exec=True, verbose=True, dry_run=False)
+    >>> options # doctest: +ELLIPSIS
+    DemoOptions(cmd=None, dry_run=False, force=False, quiet=False, runstate_signals=(...), verbose=True, all=False, jobs=4, number=0, once=True, path='/foo', trace_exec=False)
 
 *Method `BaseCommand.repl(self, *argv, banner=None, local=None)`*:
 Run an interactive Python prompt with some predefined local names.
 Aka REPL (Read Evaluate Print Loop).
 
 Parameters:
 * `argv`: any notional command line arguments
@@ -437,17 +403,17 @@
 * the attributes of `self`
 
 This is not presented automatically as a subcommand, but
 commands wishing such a command should provide something
 like this:
 
     def cmd_repl(self, argv):
-        \"\"\" Usage: {cmd}
+        """ Usage: {cmd}
               Run an interactive Python prompt with some predefined local names.
-        \"\"\"
+        """
         return self.repl(*argv)
 
 *Method `BaseCommand.run(self, **kw_options)`*:
 Run a command.
 Returns the exit status of the command.
 May raise `GetoptError` from subcommands.
 
@@ -463,15 +429,15 @@
 Otherwise `self.main(argv)` is called
 and its value returned.
 
 If the command implementation requires some setup or teardown
 then this may be provided by the `run_context()`
 context manager method.
 
-*Method `BaseCommand.run_context(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x10d48e290>, **kw)`*:
+*Method `BaseCommand.run_context(*a, upd: Optional[cs.upd.Upd] = <function uses_upd.<locals>.<lambda> at 0x104cea3b0>, **kw)`*:
 The context manager which surrounds `main` or `cmd_`*subcmd*.
 
 This default does several things, and subclasses should
 override it like this:
 
     @contextmanager
     def run_context(self):
@@ -492,15 +458,15 @@
 
 *Method `BaseCommand.subcommands()`*:
 Return a mapping of subcommand names to subcommand specifications
 for class attributes which commence with `cls.SUBCOMMAND_METHOD_PREFIX`
 by default `'cmd_'`.
 
 *Method `BaseCommand.usage_text(*, cmd=None, format_mapping=None, subcmd=None, short=False)`*:
-Compute the \"Usage:\" message for this class
+Compute the "Usage:" message for this class
 from the top level `USAGE_FORMAT`
 and the `'Usage:'`-containing docstrings of its `cmd_*` methods.
 
 Parameters:
 * `cmd`: optional command name, default derived from the class name
 * `format_mapping`: an optional format mapping for filling
   in format strings in the usage text
@@ -540,20 +506,24 @@
 
     @dataclass
     class Options(BaseCommand.Options):
         ... optional extra fields etc ...
 
 *Method `BaseCommandOptions.__call__(self, **updates)`*:
 Calling the options object returns a context manager whose
-value is a copy of the options with any `suboptions` applied.
+value is a shallow copy of the options with any `suboptions` applied.
 
 Example showing the semantics:
 
     >>> from cs.cmdutils import BaseCommandOptions
-    >>> options = BaseCommandOptions(x=1)
+    >>> @dataclass
+    ... class DemoOptions(BaseCommandOptions):
+    ...   x: int = 0
+    ...
+    >>> options = DemoOptions(x=1)
     >>> assert options.x == 1
     >>> assert not options.verbose
     >>> with options(verbose=True) as subopts:
     ...     assert options is not subopts
     ...     assert options.x == 1
     ...     assert not options.verbose
     ...     assert subopts.x == 1
@@ -582,15 +552,15 @@
     def cmd_foo(self, argv):
         self.options.popopts(
             c_='config',
             l='long',
             x='trace',
         )
         if self.options.dry_run:
-            print(\"dry run!\")
+            print("dry run!")
 
 The class attribute `COMMON_OPT_SPECS` is a mapping of
 options which are always supported. `BaseCommandOptions`
 has: `COMMON_OPT_SPECS={'n': 'dry_run', 'q': 'quiet', 'v': 'verbose'}`.
 
 A subclass with more common options might extend this like so,
 from `cs.hashindex`:
@@ -598,14 +568,19 @@
     COMMON_OPT_SPECS = dict(
         e='ssh_exe',
         h_='hashname',
         H_='hashindex_exe',
         **BaseCommand.Options.COMMON_OPT_SPECS,
     )
 
+*Method `BaseCommandOptions.update(self, **updates)`*:
+Modify the options in place with the mapping `updates`.
+It would be more normal to call the options in a `with` statement
+as shown for `__call__`.
+
 ## Function `docmd(dofunc)`
 
 Decorator for `cmd.Cmd` subclass methods
 to supply some basic quality of service.
 
 This decorator:
 - wraps the function call in a `cs.pfx.Pfx` for context
@@ -642,38 +617,43 @@
   provided its `cls.Options` class is used.
 * `options_param_name`: the parameter name to provide, default `options`
 
 Examples:
 
     @uses_cmd_options
     def f(x,*,options):
-        \"\"\" Run directly from the prevailing options. \"\"\"
+        """ Run directly from the prevailing options. """
         if options.verbose:
-            print(\"doing f with x =\", x)
+            print("doing f with x =", x)
         ....
 
     @uses_cmd_options
     def f(x,*,verbose=None,options):
-        \"\"\" Get defaults from the prevailing options. \"\"\"
+        """ Get defaults from the prevailing options. """
         if verbose is None:
             verbose = options.verbose
         if verbose:
-            print(\"doing f with x =\", x)
+            print("doing f with x =", x)
         ....
 
 # Release Log
 
 
 
+*Release 20240422*:
+* BaseCommandOptions.popopts: return the dict from BaseCommand.popopts().
+* BaseCommand.apply_preargv: apply the default options supported by self.options.
+* BaseCommandOptions.update(mapping) method, useful for dropping subcommand-specific defaults onto the options ahead of the local popopts() call.
+
 *Release 20240412*:
 * BaseCommand.run_context: do not store .upd and .runstate on the options (it confuses options in subcommands and we have @uses_runstate and @uses_upd forthis anyway these days).
 * BaseCommand.run_context: catch SIGQUIT, present the default handler as BaseCommand.handle_signal.
 
 *Release 20240316*:
-* New @uses_cmd_options decorator to provide an \"options\" parameter being the prevailing BaseCommandOptions instance.
+* New @uses_cmd_options decorator to provide an "options" parameter being the prevailing BaseCommandOptions instance.
 * BaseCommandOptions.popopts: get common options from BaseCommandOptions.COMMON_OPT_SPECS.
 
 *Release 20240211*:
 * Include the first sentence of the subcommand description in the short help.
 * BaseCommandOptions: move the runstate_signals into this directly.
 * BaseCommand: move the run() options stuff into run_context() and have it work on a copy of the original options.
 * BaseCommandCmd: implement get_names(), provide docstrings for the do_* attributes, thus help.
@@ -728,27 +708,27 @@
 * BaseCommand: new poparg(argv,...) compact validating argument consumer.
 * BaseCommand: drop run_argv, provided no utility.
 * BaseCommand.run: get the RunState signal list from self.options.runstate_signals.
 * BaseCommand.apply_opts: support multiple individual options raising GetoptError, as I hate commands which abort at the first bad option.
 * Assorted other small things.
 
 *Release 20220429*:
-* BaseCommand: fold dots in argv[0] into underscores, supports subcommands like \"setup.py\".
+* BaseCommand: fold dots in argv[0] into underscores, supports subcommands like "setup.py".
 * BaseCommand: new popargv(argv[,help_text[,parse[,validate[,unvalidated_message]]]]) helper class method.
 * BaseCommand: accept dashed-form of the underscored_form subcommand name.
 * BaseCommand: new self.options.runstate_signals=SIGINT,SIGTERM specifying singals to catch-and-cancel, shuffle run() context managers.
 
 *Release 20220318*:
 BaseCommand.__init__: handle main() method in the New Scheme.
 
 *Release 20220315*:
 _BaseSubCommand.__init__: hook in the class USAGE_KEYWORDS for methods.
 
 *Release 20220311*:
-BaseCommand: big refactor of subcommand internals and make the \"cmd_foo=FooCommand\" implementation work properly.
+BaseCommand: big refactor of subcommand internals and make the "cmd_foo=FooCommand" implementation work properly.
 
 *Release 20211208*:
 BaseCommand: better handle an unknown subcommand.
 
 *Release 20210927*:
 * Usage: show only the per subcommand usage for in-subcommand GetoptError.
 * Usage: show terse usage when the subcommand cannot be recognised.
@@ -763,57 +743,57 @@
 
 *Release 20210809*:
 Bugfix BaseCommand.cmd_help for modern API.
 
 *Release 20210731*:
 * BaseCommand.run: apply optional keyword arguments to self.options during the run.
 * Look for self.SUBCOMMAND_ARGV_DEFAULT if no subcommand is supplied.
-* Bugfix case for \"main\" method and no \"cmd_*\" methods.
+* Bugfix case for "main" method and no "cmd_*" methods.
 * Bugfix BaseCommand.cmd_help.
 
 *Release 20210420*:
 * BaseCommand.getopt_error_handler: replace error print() with warning().
 * Docstring improvements.
 
 *Release 20210407.1*:
 BaseCommand: bugfix for __init_subclass__ docstring update.
 
 *Release 20210407*:
 * BaseCommand.__init_subclass__: behave sanely if the subclass has no initial __doc__.
-* BaseCommand: new .run_argv convenience method, obviates the \"def main\" boilerplate.
+* BaseCommand: new .run_argv convenience method, obviates the "def main" boilerplate.
 
 *Release 20210404*:
 BaseCommand subclasses: automatically add the main usage message to the subclass docstring.
 
 *Release 20210306*:
 * BREAKING CHANGE: rework BaseCommand as a more normal class instantiated with argv and with most methods being instance methods, getting the former `options` parameter from self.options.
 * BaseCommand: provide default `apply_opt` and `apply_opts` methods; subclasses will generally just override the former.
 
 *Release 20210123*:
 BaseCommand: propagate the format mapping (cmd, USAGE_KEYWORDS) to the subusage generation.
 
 *Release 20201102*:
-* BaseCommand.cmd_help: supply usage only for \"all commands\", full docstring for specified commands.
+* BaseCommand.cmd_help: supply usage only for "all commands", full docstring for specified commands.
 * BaseCommand: honour presupplied options.log_level.
 * BaseCommand.usage_text: handle missing USAGE_FORMAT better.
 * BaseCommand.run: provide options.upd.
 * BaseCommand subclasses may now override BaseCommand.OPTIONS_CLASS (default SimpleNamespace) in order to provide convenience methods on the options.
 * BaseCommand.run: separate variable for subcmd with dash translated to underscore to match method names.
 * Minor fixes.
 
 *Release 20200615*:
-BaseCommand.usage_text: do not mention the \"help\" command if it is the only subcommand (it won't be available if there are no other subcommands).
+BaseCommand.usage_text: do not mention the "help" command if it is the only subcommand (it won't be available if there are no other subcommands).
 
 *Release 20200521.1*:
 Fix DISTINFO.install_requires.
 
 *Release 20200521*:
 * BaseCommand.run: support using BaseCommand subclasses as cmd_* names to make it easy to nest BaseCommands.
 * BaseCommand: new hack_postopts_argv method called after parsing the main command line options, for inferring subcommands or the like.
-* BaseCommand: extract \"Usage:\" paragraphs from subcommand method docstrings to build the main usage message.
+* BaseCommand: extract "Usage:" paragraphs from subcommand method docstrings to build the main usage message.
 * BaseCommand: new cmd_help default command.
 * Assorted bugfixes and small improvements.
 
 *Release 20200318*:
 * BaseCommand.run: make argv optional, get additional usage keywords from self.USAGE_KEYWORDS.
 * @BaseCommand.add_usage_to_docstring: honour cls.USAGE_KEYWORDS.
 * BaseCommand: do not require GETOPT_SPEC for commands with no defined options.
@@ -835,25 +815,8 @@
 *Release 20190619*:
 Minor documentation updates.
 
 *Release 20190617.2*:
 Lint.
 
 *Release 20190617.1*:
-Initial release with @docmd decorator and alpha quality BaseCommand command line assistance class."""
-content-type = "text/markdown"
-
-[build-system]
-build-backend = "setuptools.build_meta"
-requires = [
-    "setuptools >= 61.2",
-    "trove-classifiers",
-    "wheel",
-]
-
-[tool.setuptools]
-py-modules = [
-    "cs.cmdutils",
-]
-
-[tool.setuptools.package-dir]
-"" = "lib/python"
+Initial release with @docmd decorator and alpha quality BaseCommand command line assistance class.
```


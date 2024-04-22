# Comparing `tmp/cs.tagset-20240316.tar.gz` & `tmp/cs.tagset-20240422.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.tagset-20240316.tar", last modified: Sat Mar 16 06:05:55 2024, max compression
+gzip compressed data, was "cs.tagset-20240422.tar", last modified: Mon Apr 22 03:00:29 2024, max compression
```

## Comparing `cs.tagset-20240316.tar` & `cs.tagset-20240422.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:05:55.017844 cs.tagset-20240316/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-03-16 06:05:27.000000 cs.tagset-20240316/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    32240 2024-03-16 06:05:55.017471 cs.tagset-20240316/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    66005 2024-03-16 06:05:35.000000 cs.tagset-20240316/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:05:55.012443 cs.tagset-20240316/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:05:55.012750 cs.tagset-20240316/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:05:55.014395 cs.tagset-20240316/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)   132927 2024-03-16 06:05:16.000000 cs.tagset-20240316/lib/python/cs/tagset.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-03-16 06:05:55.016873 cs.tagset-20240316/lib/python/cs.tagset.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    32240 2024-03-16 06:05:54.000000 cs.tagset-20240316/lib/python/cs.tagset.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      279 2024-03-16 06:05:54.000000 cs.tagset-20240316/lib/python/cs.tagset.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-03-16 06:05:54.000000 cs.tagset-20240316/lib/python/cs.tagset.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      296 2024-03-16 06:05:54.000000 cs.tagset-20240316/lib/python/cs.tagset.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-03-16 06:05:54.000000 cs.tagset-20240316/lib/python/cs.tagset.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    33057 2024-03-16 06:05:53.000000 cs.tagset-20240316/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-03-16 06:05:55.017959 cs.tagset-20240316/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 03:00:29.538258 cs.tagset-20240422/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-22 02:59:59.000000 cs.tagset-20240422/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    66713 2024-04-22 03:00:29.537890 cs.tagset-20240422/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    65929 2024-04-22 03:00:09.000000 cs.tagset-20240422/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 03:00:29.533013 cs.tagset-20240422/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 03:00:29.533338 cs.tagset-20240422/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 03:00:29.534994 cs.tagset-20240422/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)   134320 2024-04-22 02:59:42.000000 cs.tagset-20240422/lib/python/cs/tagset.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 03:00:29.537196 cs.tagset-20240422/lib/python/cs.tagset.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    66713 2024-04-22 03:00:28.000000 cs.tagset-20240422/lib/python/cs.tagset.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      279 2024-04-22 03:00:29.000000 cs.tagset-20240422/lib/python/cs.tagset.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-22 03:00:28.000000 cs.tagset-20240422/lib/python/cs.tagset.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      296 2024-04-22 03:00:29.000000 cs.tagset-20240422/lib/python/cs.tagset.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-22 03:00:29.000000 cs.tagset-20240422/lib/python/cs.tagset.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    67585 2024-04-22 03:00:27.000000 cs.tagset-20240422/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-22 03:00:29.538361 cs.tagset-20240422/setup.cfg
```

### Comparing `cs.tagset-20240316/README.md` & `cs.tagset-20240422/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Tags and sets of tags
 with __format__ support and optional ontology information.
 
-*Latest release 20240316*:
-Fixed release upload artifacts.
+*Latest release 20240422*:
+* New jsonable(obj) function to return a deep copy of `obj` which can be transcribed as JSON.
+* Tag.transcribe_value: pass jsonable(value) to the JSON encoder, drop special checks now done by jsonable().
+* Tag.__str__: do not catch TypeError any more, was embedding Python repr()s in .fstags files - now Tag.transcribe_value() does the correct thing where that is possible.
 
 See `cs.fstags` for support for applying these to filesystem objects
 such as directories and files.
 
 See `cs.sqltags` for support for databases of entities with tags,
 not directly associated with filesystem objects.
 This is suited to both log entries (entities with no "name")
@@ -190,15 +192,15 @@
 
 This accepts `int`, `float` (already a timestamp)
 and `date` or `datetime`
 (use `datetime.timestamp() for a nonnaive `datetime`,
 otherwise `time.mktime(tag_value.time_tuple())`,
 which assumes the local time zone).
 
-## Class `BaseTagSets(cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin, collections.abc.MutableMapping, collections.abc.Mapping, collections.abc.Collection, collections.abc.Sized, collections.abc.Iterable, collections.abc.Container)`
+## Class `BaseTagSets(cs.resources.MultiOpenMixin, collections.abc.MutableMapping)`
 
 Base class for collections of `TagSet` instances
 such as `cs.fstags.FSTags` and `cs.sqltags.SQLTags`.
 
 Examples of this include:
 * `cs.cdrip.MBSQLTags`: a mapping of MusicbrainsNG entities to their associated `TagSet`
 * `cs.fstags.FSTags`: a mapping of filesystem paths to their associated `TagSet`
@@ -305,15 +307,24 @@
 Return a proxy for this `BaseTagSets` for the `name`s
 starting with `subname+'.'`.
 
 *Method `BaseTagSets.values(self, *, prefix=None)`*:
 Generator yielding the mapping values (`TagSet`s),
 optionally constrained to keys starting with `prefix+'.'`.
 
-## Class `MappingTagSets(BaseTagSets, cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin, collections.abc.MutableMapping, collections.abc.Mapping, collections.abc.Collection, collections.abc.Sized, collections.abc.Iterable, collections.abc.Container)`
+## Function `jsonable(obj, converted: dict)`
+
+Convert `obj` to a JSON encodable form.
+This returns `obj` for purely JSONable objects and a JSONable
+deep copy of `obj` if it or some subcomponent required
+conversion.
+`converted` is a dict mapping object ids to their converted forms
+to prevent loops.
+
+## Class `MappingTagSets(BaseTagSets)`
 
 A `BaseTagSets` subclass using an arbitrary mapping.
 
 If no mapping is supplied, a `dict` is created for the purpose.
 
 Example:
 
@@ -351,15 +362,15 @@
 *Method `RegexpTagRule.infer_tags(self, s)`*:
 Apply the rule to the string `s`, return a list of `Tag`s.
 
 ## Function `selftest(argv)`
 
 Run some ad hoc self tests.
 
-## Class `Tag(Tag, builtins.tuple, cs.lex.FormatableMixin, cs.lex.FormatableFormatter, string.Formatter)`
+## Class `Tag(Tag, cs.lex.FormatableMixin)`
 
 A `Tag` has a `.name` (`str`) and a `.value`
 and an optional `.ontology`.
 
 The `name` must be a dotted identifier.
 
 Terminology:
@@ -624,15 +635,15 @@
     tags = TagSet()
     ....
     tags.add('colour', 'blue')
     ....
     tag = Tag('size', 9)
     tags.add(tag)
 
-## Class `TagBasedTest(TagBasedTest, builtins.tuple, TagSetCriterion, cs.deco.Promotable)`
+## Class `TagBasedTest(TagBasedTest, TagSetCriterion)`
 
 A test based on a `Tag`.
 
 Attributes:
 * `spec`: the source text from which this choice was parsed,
   possibly `None`
 * `choice`: the apply/reject flag
@@ -661,15 +672,15 @@
 *Method `TagBasedTest.parse(s, offset=0, delim=None)`*:
 Parse *tag_name*[{`<`|`<=`|'='|'>='|`>`|'~'}*value*]
 and return `(dict,offset)`
 where the `dict` contains the following keys and values:
 * `tag`: a `Tag` embodying the tag name and value
 * `comparison`: an indication of the test comparison
 
-## Class `TagFile(cs.fs.FSPathBasedSingleton, cs.obj.SingletonMixin, cs.fs.HasFSPath, BaseTagSets, cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin, collections.abc.MutableMapping, collections.abc.Mapping, collections.abc.Collection, collections.abc.Sized, collections.abc.Iterable, collections.abc.Container)`
+## Class `TagFile(cs.fs.FSPathBasedSingleton, BaseTagSets)`
 
 A reference to a specific file containing tags.
 
 This manages a mapping of `name` => `TagSet`,
 itself a mapping of tag name => tag value.
 
 *Method `TagFile.__setitem__(self, name, te)`*:
@@ -709,20 +720,17 @@
 
 This method will create the required intermediate directories
 if missing.
 
 This method *does not* clear the `.modified` attribute of the `TagSet`s
 because it does not know it is saving to the `Tagset`'s primary location.
 
-*Method `TagFile.shutdown(self)`*:
+*Method `TagFile.startup_shutdown(self)`*:
 Save the tagsets if modified.
 
-*Method `TagFile.startup(self)`*:
-No special startup.
-
 *Method `TagFile.tags_line(name, tags, extra_types=None, prune=False)`*:
 Transcribe a `name` and its `tags` for use as a `.fstags` file line.
 
 *Property `TagFile.tagsets`*:
 The tag map from the tag file,
 a mapping of name=>`TagSet`.
 
@@ -788,15 +796,15 @@
 which itself defaults to class `TagSetCriterion`.
 
 The default `TagSetCriterion.from_str` recognises:
 * `-`*tag_name*: a negative requirement for *tag_name*
 * *tag_name*[`=`*value*]: a positive requirement for a *tag_name*
   with optional *value*.
 
-## Class `TagSet(builtins.dict, cs.dateutils.UNIXTimeMixin, cs.lex.FormatableMixin, cs.lex.FormatableFormatter, string.Formatter, cs.mappings.AttrableMappingMixin)`
+## Class `TagSet(builtins.dict, cs.dateutils.UNIXTimeMixin, cs.lex.FormatableMixin, cs.mappings.AttrableMappingMixin)`
 
 A setlike class associating a set of tag names with values.
 
 This actually subclasses `dict`, so a `TagSet` is a direct
 mapping of tag names to values.
 It accepts attribute access to simple tag values when they
 do not conflict with the class methods;
@@ -1153,15 +1161,15 @@
 indicating negation of the test,
 followed by a criterion recognised by the `.parse` method
 of one of the classes in `cls.CRITERION_PARSE_CLASSES`.
 
 *Method `TagSetCriterion.match_tagged_entity(self, te: 'TagSet') -> bool`*:
 Apply this `TagSetCriterion` to a `TagSet`.
 
-## Class `TagSetPrefixView(cs.lex.FormatableMixin, cs.lex.FormatableFormatter, string.Formatter)`
+## Class `TagSetPrefixView(cs.lex.FormatableMixin)`
 
 A view of a `TagSet` via a `prefix`.
 
 Access to a key `k` accesses the `TagSet`
 with the key `prefix+'.'+k`.
 
 This is a kind of funny hybrid of a `Tag` and a `TagSet`
@@ -1236,23 +1244,23 @@
 
 *Property `TagSetPrefixView.value`*:
 Return the `Tag` value for the prefix, or `None` if there is no such `Tag`.
 
 *Method `TagSetPrefixView.values(self)`*:
 Return an iterable of the values (`Tag`s).
 
-## Class `TagSetsSubdomain(cs.obj.SingletonMixin, cs.mappings.PrefixedMappingProxy, cs.mappings.RemappedMappingProxy)`
+## Class `TagSetsSubdomain(cs.obj.SingletonMixin, cs.mappings.PrefixedMappingProxy)`
 
 A view into a `BaseTagSets` for keys commencing with a prefix
 being the subdomain plus a dot (`'.'`).
 
 *Property `TagSetsSubdomain.TAGGED_ENTITY_FACTORY`*:
 The entity factory comes from the parent collection.
 
-## Class `TagsOntology(cs.obj.SingletonMixin, BaseTagSets, cs.resources.MultiOpenMixin, cs.context.ContextManagerMixin, collections.abc.MutableMapping, collections.abc.Mapping, collections.abc.Collection, collections.abc.Sized, collections.abc.Iterable, collections.abc.Container)`
+## Class `TagsOntology(cs.obj.SingletonMixin, BaseTagSets)`
 
 An ontology for tag names.
 This is based around a mapping of names
 to ontological information expressed as a `TagSet`.
 
 Normally an object's tags are not a self contained repository of all the information;
 instead a tag just names some information.
@@ -1519,15 +1527,17 @@
   for example `"Marvel.Captain America"`
   becomes `"marvel.captain_america"`.
 
 ## Class `TagsOntologyCommand(cs.cmdutils.BaseCommand)`
 
 A command line for working with ontology types.
 
-Command line usage:
+Command line implementation.
+
+Usage summary:
 
     Usage: tagsontology subcommand [...]
       Subcommands:
         edit [{/name-regexp | entity-name}]
           Edit entities.
           With no arguments, edit all the entities.
           With an argument starting with a slash, edit the entities
@@ -1586,14 +1596,19 @@
 {cmd} type_name + entity_name [tags...]
   Create type_name.entity_name and apply the tags.
 
 # Release Log
 
 
 
+*Release 20240422*:
+* New jsonable(obj) function to return a deep copy of `obj` which can be transcribed as JSON.
+* Tag.transcribe_value: pass jsonable(value) to the JSON encoder, drop special checks now done by jsonable().
+* Tag.__str__: do not catch TypeError any more, was embedding Python repr()s in .fstags files - now Tag.transcribe_value() does the correct thing where that is possible.
+
 *Release 20240316*:
 Fixed release upload artifacts.
 
 *Release 20240305*:
 * Tag.from_str2: make the ontology optional.
 * TagSetPrefixView: provide __len__() and update().
```

### Comparing `cs.tagset-20240316/lib/python/cs/tagset.py` & `cs.tagset-20240422/lib/python/cs/tagset.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,15 @@
 )
 from cs.obj import SingletonMixin
 from cs.pfx import Pfx, pfx, pfx_call, pfx_method
 from cs.py3 import date_fromisoformat, datetime_fromisoformat
 from cs.resources import MultiOpenMixin
 from cs.threads import locked_property
 
-__version__ = '20240316'
+__version__ = '20240422'
 
 DISTINFO = {
     'keywords': ["python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
@@ -358,14 +358,63 @@
   if isinstance(tag_value, (int, float)):
     return float(tag_value)
   raise ValueError(
       "requires an int, float, date or datetime, got %s:%r" %
       (type(tag_value), tag_value)
   )
 
+def jsonable(obj, converted: dict):
+  ''' Convert `obj` to a JSON encodable form.
+      This returns `obj` for purely JSONable objects and a JSONable
+      deep copy of `obj` if it or some subcomponent required
+      conversion.
+      `converted` is a dict mapping object ids to their converted forms
+      to prevent loops.
+  '''
+  if obj is None:
+    return obj
+  try:
+    # known object - return conversion from the cache
+    return converted[id(obj)]
+  except KeyError:
+    pass
+  t = type(obj)
+  if t in (int, float, str, bool):
+    # return unchanged - no need to record the convobj
+    return obj
+  if isinstance(t, (set, tuple, list)):
+    # convert to list
+    converted[id(obj)] = convobj = []
+    convobj.extend(jsonable(item, converted) for item in obj)
+    return convobj
+  # a mapping?
+  try:
+    keys = obj.keys
+  except AttributeError:
+    # an iterable?
+    try:
+      it = iter(obj)
+    except TypeError:
+      raise TypeError(f'jsoanble({t.__name__}): cannot convert for JSON')
+    else:
+      if it is obj:
+        raise TypeError(
+            f'jsoanble(t.__name__): refusing to convert an iterator for JSON because it would consume it'
+        )
+      # convert to list
+      converted[id(obj)] = convobj = []
+      convobj.extend(jsonable(item, converted) for item in it)
+      return convobj
+  else:
+    # a mapping
+    converted[id(obj)] = convobj = {}
+    for k in keys():
+      convobj[k] = jsonable(obj[k], converted)
+    return convobj
+
 class _FormatStringTagProxy:
   ''' A proxy for a `Tag` where `__str__` returns `str(self.value)`.
 
       This is for use during `TagSet` string formatting
       because the "no format spec" falls through to `__str__`.
   '''
 
@@ -1302,21 +1351,21 @@
     except AttributeError:
       raise ValueError("tag has no .name attribute")  # pylint: disable=raise-missing-from
     else:
       name0 = name  # keep the preprefix name
       if prefix:
         name = prefix + '.' + name
     if value is not None:
-      raise ValueError(
-          "name(%s) is not a str, value must be None" % (r(name),)
-      )
+      raise ValueError(f'name({r(name)}) is not a str, value must be None')
     try:
       value = tag.value
     except AttributeError:
-      raise ValueError("tag has no .value attribute")  # pylint: disable=raise-missing-from
+      # pylint: disable=raise-missing-from
+      # noqa: B904
+      raise ValueError("tag has no .value attribute")
     if isinstance(tag, Tag):
       # already a Tag subtype, see if the ontology needs updating or the name was changed
       if name != name0 or (ontology is not None
                            and tag.ontology is not ontology):
         # new Tag with supplied ontology
         tag = super().__new__(cls, name, value, ontology)
     else:
@@ -1361,18 +1410,15 @@
   def __str__(self):
     ''' Encode `name` and `value`.
     '''
     name = self.name
     value = self.value
     if value is None:
       return name
-    try:
-      value_s = self.transcribe_value(value)
-    except TypeError:
-      value_s = str(value)
+    value_s = self.transcribe_value(value)
     return name + '=' + value_s
 
   @classmethod
   def transcribe_value(cls, value, extra_types=None, json_options=None):
     ''' Transcribe `value` for use in `Tag` transcription.
 
         The optional `extra_types` parameter may be an iterable of
@@ -1400,27 +1446,24 @@
           raise ValueError(
               "to_str(%r) => %r: contains whitespace" % (value, value_s)
           )
         return value_s
     # "bare" dotted identifiers
     if isinstance(value, str) and is_dotted_identifier(value):
       return value
-    # convert some values to a suitable type
-    if isinstance(value, (tuple, set)):
-      value = list(value)
     # fall back to JSON encoded form of value
     if json_options:
       # custom encoder
       json_options = dict(json_options)
       for k, v in cls.JSON_ENCODER_DEFAULTS.items():
         json_options.setdefault(k, v)
       encoder = JSONEncoder(**json_options)
     else:
       encoder = cls.JSON_ENCODER
-    return encoder.encode(value)
+    return encoder.encode(jsonable(value, {}))
 
   @classmethod
   def from_str(cls, s, offset=0, ontology=None, fallback_parse=None):
     ''' Parse a `Tag` definition from `s` at `offset` (default `0`).
     '''
     with Pfx("%s.from_str(%r[%d:],...)", cls.__name__, s, offset):
       tag, post_offset = cls.from_str2(
@@ -1557,15 +1600,16 @@
     if s[offset] in '"[{':
       # must be a JSON value - collect it
       value_part = s[offset:]
       try:
         value, suboffset = cls.JSON_DECODER.raw_decode(value_part)
       except JSONDecodeError as e:
         raise ValueError(
-            "offset %d: raw_decode(%r): %s" % (offset, value_part, e)
+            "offset %d: raw_decode(%s): %s" %
+            (offset, cropped_repr(value_part), e)
         ) from e
       offset += suboffset
       return value, offset
     # collect nonwhitespace (or whatever fallback_parse gathers),
     nonwhite, offset = fallback_parse(s, offset)
     # check for the basic types - these are never overridden
     # check for round trip int or float
@@ -1761,27 +1805,30 @@
     ''' The type name for members of this tag.
 
         This is required if `.value` is a mapping.
     '''
     try:
       return self.typedata['key_type']
     except KeyError:
-      raise AttributeError('key_type')  # pylint: disable=raise-missing-from
+      # pylint: disable=raise-missing-from
+      # noqa: B904
+      raise AttributeError('key_type')
 
   @property
-  @pfx_method
   def member_type(self):
     ''' The type name for members of this tag.
 
         This is required if `.value` is a sequence or mapping.
     '''
     try:
       return self.typedata['member_type']
     except KeyError:
-      raise AttributeError('member_type')  # pylint: disable=raise-missing-from
+      # pylint: disable=raise-missing-from
+      # noqa: B904
+      raise AttributeError('member_type')
 
 class TagSetCriterion(Promotable):
   ''' A testable criterion for a `TagSet`.
   '''
 
   # list of TagSetCriterion classes
   # whose .parse methods are used by .parse
@@ -2159,16 +2206,16 @@
     return {k: self._tags[self._prefix_ + k] for k in self.keys()}
 
   def __getattr__(self, attr):
     ''' Proxy other attributes through to the `TagSet`.
     '''
     try:
       return self[attr]
-    except (KeyError, TypeError):
-      raise AttributeError("%s.%s" % (self.__class__.__name__, attr))
+    except (KeyError, TypeError) as e:
+      raise AttributeError(f'{self.__class__.__name__}.{attr}') from e
 
   def __setattr__(self, attr, value):
     ''' Attribute based `Tag` access.
 
         If `attr` is in `self.__dict__` then that is updated,
         supporting "normal" attributes set on the instance.
         Otherwise the `Tag` named `attr` is set to `value`.
@@ -3295,22 +3342,23 @@
 
   def __str__(self):
     return "%s(%r)" % (type(self).__name__, shortpath(self.fspath))
 
   def __repr__(self):
     return "%s(%r)" % (type(self).__name__, self.fspath)
 
-  def startup(self):
-    ''' No special startup.
-    '''
-
-  def shutdown(self):
+  @contextmanager
+  def startup_shutdown(self):
     ''' Save the tagsets if modified.
     '''
-    self.save()
+    try:
+      with super().startup_shutdown():
+        yield
+    finally:
+      self.save()
 
   def get(self, name, default=None):
     ''' Get from the tagsets.
     '''
     return self.tagsets.get(name, default)
 
   def __setitem__(self, name, te):
@@ -3347,15 +3395,14 @@
       return False
     sig = self._loadsave_signature()
     if self._loaded_signature != sig:
       return True
     return any(map(lambda tagset: tagset.modified, tagsets.values()))
 
   @locked_property
-  @pfx_method
   def tagsets(self):
     ''' The tag map from the tag file,
         a mapping of name=>`TagSet`.
 
         This is loaded on demand.
     '''
     ts = {}
@@ -3374,15 +3421,14 @@
   @property
   def names(self):
     ''' The names from this `FSTagsTagFile` as a list.
     '''
     return list(self.tagsets.keys())
 
   @classmethod
-  @pfx_method
   def parse_tags_line(
       cls,
       line,
       ontology=None,
       verbose=None,
       extra_types=None,
   ) -> Tuple[str, TagSet]:
```


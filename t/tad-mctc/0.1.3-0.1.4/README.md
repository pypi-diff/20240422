# Comparing `tmp/tad_mctc-0.1.3.tar.gz` & `tmp/tad_mctc-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tad_mctc-0.1.3.tar", last modified: Mon Apr 15 10:38:59 2024, max compression
+gzip compressed data, was "tad_mctc-0.1.4.tar", last modified: Mon Apr 22 07:21:00 2024, max compression
```

## Comparing `tad_mctc-0.1.3.tar` & `tad_mctc-0.1.4.tar`

### file list

```diff
@@ -1,113 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.473671 tad_mctc-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10602 2024-04-15 10:38:59.473671 tad_mctc-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8658 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-15 10:38:59.477671 tad_mctc-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.457671 tad_mctc-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.461671 tad_mctc-0.1.3/src/tad_mctc/
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.461671 tad_mctc-0.1.3/src/tad_mctc/autograd/
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/autograd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/autograd/batched.py
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/autograd/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/autograd/gradcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/autograd/hessian.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/autograd/internals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/autograd/nonfunctorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.461671 tad_mctc-0.1.3/src/tad_mctc/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/batch/agnostic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.461671 tad_mctc-0.1.3/src/tad_mctc/batch/mask/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/batch/mask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/batch/mask/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/batch/mask/jit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/batch/mask/pairs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/batch/mask/triples.py
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/batch/pack.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/batch/unpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.465671 tad_mctc-0.1.3/src/tad_mctc/convert/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/convert/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/convert/pse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/convert/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/convert/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.465671 tad_mctc-0.1.3/src/tad_mctc/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/data/en.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/data/getters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/data/mass.py
--rw-r--r--   0 runner    (1001) docker     (127)    69463 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/data/molecules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/data/pse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/data/radii.py
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/data/zeff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.465671 tad_mctc-0.1.3/src/tad_mctc/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/exceptions/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/exceptions/molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/exceptions/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.465671 tad_mctc-0.1.3/src/tad_mctc/io/
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.465671 tad_mctc-0.1.3/src/tad_mctc/io/checks/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/checks/molecule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/checks/shape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.469671 tad_mctc-0.1.3/src/tad_mctc/io/read/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/read/dotfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/read/frompath.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/read/orca.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/read/qcschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/read/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/read/tblite.py
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/read/turbomole.py
--rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/read/xyz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.469671 tad_mctc-0.1.3/src/tad_mctc/io/write/
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/write/turbomole.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/write/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/io/write/xyz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.469671 tad_mctc-0.1.3/src/tad_mctc/math/
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/math/einsum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.469671 tad_mctc-0.1.3/src/tad_mctc/molecule/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/molecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13209 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/molecule/bond.py
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/molecule/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/molecule/property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.469671 tad_mctc-0.1.3/src/tad_mctc/ncoord/
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/ncoord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/ncoord/count.py
--rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/ncoord/d3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/ncoord/d4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/ncoord/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/ncoord/eeq.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.473671 tad_mctc-0.1.3/src/tad_mctc/storch/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/storch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/storch/distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/storch/elemental.py
--rw-r--r--   0 runner    (1001) docker     (127)    30570 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/storch/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/storch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.473671 tad_mctc-0.1.3/src/tad_mctc/typing/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/typing/builtin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/typing/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8427 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/typing/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.473671 tad_mctc-0.1.3/src/tad_mctc/units/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/units/codata.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/units/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/units/length.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/units/mass.py
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/units/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/units/spectroscopy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-15 10:38:56.000000 tad_mctc-0.1.3/src/tad_mctc/units/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:38:59.473671 tad_mctc-0.1.3/src/tad_mctc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10602 2024-04-15 10:38:59.000000 tad_mctc-0.1.3/src/tad_mctc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-15 10:38:59.000000 tad_mctc-0.1.3/src/tad_mctc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 10:38:59.000000 tad_mctc-0.1.3/src/tad_mctc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-15 10:38:59.000000 tad_mctc-0.1.3/src/tad_mctc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 10:38:59.000000 tad_mctc-0.1.3/src/tad_mctc.egg-info/top_level.txt
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.026948 tad_mctc-0.1.4/
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)    11358 2024-03-29 08:44:28.000000 tad_mctc-0.1.4/LICENSE
+-rw-r--r--   0 marvin    (1000) marvin    (1000)    10999 2024-04-22 07:21:00.026948 tad_mctc-0.1.4/PKG-INFO
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     8946 2024-04-20 21:35:38.000000 tad_mctc-0.1.4/README.md
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     1648 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/pyproject.toml
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     1597 2024-04-22 07:21:00.026948 tad_mctc-0.1.4/setup.cfg
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      714 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/setup.py
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:20:59.994948 tad_mctc-0.1.4/src/
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:20:59.998948 tad_mctc-0.1.4/src/tad_mctc/
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     4375 2024-04-20 20:54:14.000000 tad_mctc-0.1.4/src/tad_mctc/__init__.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     1590 2024-04-20 21:35:38.000000 tad_mctc-0.1.4/src/tad_mctc/_version.py
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.002948 tad_mctc-0.1.4/src/tad_mctc/autograd/
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      921 2024-04-07 07:40:43.000000 tad_mctc-0.1.4/src/tad_mctc/autograd/__init__.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     1455 2024-04-14 12:23:40.000000 tad_mctc-0.1.4/src/tad_mctc/autograd/batched.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     4489 2024-04-07 07:40:43.000000 tad_mctc-0.1.4/src/tad_mctc/autograd/compat.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     4188 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/autograd/gradcheck.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     2691 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/autograd/hessian.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     2087 2024-04-22 07:10:01.000000 tad_mctc-0.1.4/src/tad_mctc/autograd/internals.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     2578 2024-04-07 07:40:43.000000 tad_mctc-0.1.4/src/tad_mctc/autograd/nonfunctorch.py
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.002948 tad_mctc-0.1.4/src/tad_mctc/batch/
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      817 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/batch/__init__.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     1911 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/batch/agnostic.py
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.002948 tad_mctc-0.1.4/src/tad_mctc/batch/mask/
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      923 2024-04-20 10:53:40.000000 tad_mctc-0.1.4/src/tad_mctc/batch/mask/__init__.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     1291 2024-04-20 10:53:40.000000 tad_mctc-0.1.4/src/tad_mctc/batch/mask/atoms.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     2861 2024-04-20 10:53:40.000000 tad_mctc-0.1.4/src/tad_mctc/batch/mask/jit.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     2667 2024-04-20 10:53:40.000000 tad_mctc-0.1.4/src/tad_mctc/batch/mask/pairs.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     2103 2024-04-20 10:53:40.000000 tad_mctc-0.1.4/src/tad_mctc/batch/mask/triples.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     5722 2024-04-14 12:23:40.000000 tad_mctc-0.1.4/src/tad_mctc/batch/pack.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     5898 2024-04-14 12:23:40.000000 tad_mctc-0.1.4/src/tad_mctc/batch/unpack.py
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.006948 tad_mctc-0.1.4/src/tad_mctc/convert/
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      903 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/convert/__init__.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     3963 2024-04-07 07:40:43.000000 tad_mctc-0.1.4/src/tad_mctc/convert/numpy.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     1692 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/convert/pse.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     3952 2024-04-20 20:54:14.000000 tad_mctc-0.1.4/src/tad_mctc/convert/pytorch.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     2733 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/convert/tensor.py
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.006948 tad_mctc-0.1.4/src/tad_mctc/data/
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     1041 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/data/__init__.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     1890 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/data/en.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     3320 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/data/getters.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     2421 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/data/mass.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)    69463 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/data/molecules.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     4440 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/data/pse.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     4312 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/data/radii.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     3607 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/data/zeff.py
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.010948 tad_mctc-0.1.4/src/tad_mctc/exceptions/
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      803 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/exceptions/__init__.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     1143 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/exceptions/io.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      994 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/exceptions/molecule.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      944 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/exceptions/pytorch.py
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.010948 tad_mctc-0.1.4/src/tad_mctc/io/
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      750 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/io/__init__.py
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.010948 tad_mctc-0.1.4/src/tad_mctc/io/checks/
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      782 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/io/checks/__init__.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     7839 2024-04-22 07:10:01.000000 tad_mctc-0.1.4/src/tad_mctc/io/checks/molecule.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     2281 2024-04-22 07:10:01.000000 tad_mctc-0.1.4/src/tad_mctc/io/checks/shape.py
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.014948 tad_mctc-0.1.4/src/tad_mctc/io/read/
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     1144 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/io/read/__init__.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     2463 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/io/read/dotfiles.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     6759 2024-04-22 07:10:01.000000 tad_mctc-0.1.4/src/tad_mctc/io/read/frompath.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     2834 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/io/read/orca.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     3169 2024-04-22 07:10:01.000000 tad_mctc-0.1.4/src/tad_mctc/io/read/qcschema.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     5446 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/io/read/reader.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     2416 2024-04-22 07:10:01.000000 tad_mctc-0.1.4/src/tad_mctc/io/read/tblite.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     5433 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/io/read/turbomole.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     5472 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/io/read/xyz.py
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.014948 tad_mctc-0.1.4/src/tad_mctc/io/write/
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      770 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/io/write/__init__.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     2240 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/io/write/turbomole.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     2817 2024-04-22 07:10:01.000000 tad_mctc-0.1.4/src/tad_mctc/io/write/writer.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     2446 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/io/write/xyz.py
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.014948 tad_mctc-0.1.4/src/tad_mctc/math/
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      746 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/math/__init__.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     2305 2024-04-20 10:53:40.000000 tad_mctc-0.1.4/src/tad_mctc/math/einsum.py
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.014948 tad_mctc-0.1.4/src/tad_mctc/molecule/
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      838 2024-04-20 20:54:14.000000 tad_mctc-0.1.4/src/tad_mctc/molecule/__init__.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)    13256 2024-04-20 20:54:14.000000 tad_mctc-0.1.4/src/tad_mctc/molecule/bond.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     5706 2024-04-22 07:10:01.000000 tad_mctc-0.1.4/src/tad_mctc/molecule/container.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     4014 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/molecule/geometry.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     4546 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/molecule/property.py
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.018948 tad_mctc-0.1.4/src/tad_mctc/ncoord/
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     2871 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/ncoord/__init__.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     5967 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/ncoord/count.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     5623 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/ncoord/d3.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     3731 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/ncoord/d4.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     1593 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/ncoord/defaults.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     4385 2024-04-22 07:10:01.000000 tad_mctc-0.1.4/src/tad_mctc/ncoord/eeq.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)        0 2024-01-10 18:46:05.000000 tad_mctc-0.1.4/src/tad_mctc/py.typed
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.018948 tad_mctc-0.1.4/src/tad_mctc/storch/
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     1113 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/storch/__init__.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     4532 2024-04-20 10:53:40.000000 tad_mctc-0.1.4/src/tad_mctc/storch/distance.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     4289 2024-04-14 16:23:38.000000 tad_mctc-0.1.4/src/tad_mctc/storch/elemental.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)    30570 2024-04-17 05:57:02.000000 tad_mctc-0.1.4/src/tad_mctc/storch/linalg.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     1343 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/storch/utils.py
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.018948 tad_mctc-0.1.4/src/tad_mctc/tools/
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      755 2024-04-20 20:54:14.000000 tad_mctc-0.1.4/src/tad_mctc/tools/__init__.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     6412 2024-04-20 20:54:14.000000 tad_mctc-0.1.4/src/tad_mctc/tools/caching.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     3188 2024-04-22 07:10:01.000000 tad_mctc-0.1.4/src/tad_mctc/tools/memory.py
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.022948 tad_mctc-0.1.4/src/tad_mctc/typing/
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      920 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/typing/__init__.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     1107 2024-04-20 10:53:40.000000 tad_mctc-0.1.4/src/tad_mctc/typing/builtin.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     4777 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/typing/compat.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     8809 2024-04-20 20:54:14.000000 tad_mctc-0.1.4/src/tad_mctc/typing/pytorch.py
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.022948 tad_mctc-0.1.4/src/tad_mctc/units/
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      841 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/units/__init__.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     2025 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/units/codata.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     3517 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/units/energy.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     1463 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/units/length.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     1682 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/units/mass.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      873 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/units/math.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     2490 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/units/spectroscopy.py
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     1047 2024-03-29 21:07:36.000000 tad_mctc-0.1.4/src/tad_mctc/units/time.py
+drwxrwxr-x   0 marvin    (1000) marvin    (1000)        0 2024-04-22 07:21:00.022948 tad_mctc-0.1.4/src/tad_mctc.egg-info/
+-rw-r--r--   0 marvin    (1000) marvin    (1000)    10999 2024-04-22 07:20:59.000000 tad_mctc-0.1.4/src/tad_mctc.egg-info/PKG-INFO
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)     2883 2024-04-22 07:20:59.000000 tad_mctc-0.1.4/src/tad_mctc.egg-info/SOURCES.txt
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)        1 2024-04-22 07:20:59.000000 tad_mctc-0.1.4/src/tad_mctc.egg-info/dependency_links.txt
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)      245 2024-04-22 07:20:59.000000 tad_mctc-0.1.4/src/tad_mctc.egg-info/requires.txt
+-rw-rw-r--   0 marvin    (1000) marvin    (1000)        9 2024-04-22 07:20:59.000000 tad_mctc-0.1.4/src/tad_mctc.egg-info/top_level.txt
```

### Comparing `tad_mctc-0.1.3/LICENSE` & `tad_mctc-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/PKG-INFO` & `tad_mctc-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: tad_mctc
-Version: 0.1.3
+Version: 0.1.4
 Summary: Torch Autodiff Utility
 Home-page: https://github.com/tad-mctc/tad-mctc
 Author: "Marvin Friede"
 License: Apache-2.0
 Project-URL: Documentation, https://tad-mctc.readthedocs.io
 Project-URL: Source, https://github.com/tad-mctc/tad-mctc
 Project-URL: Tracker, https://github.com/tad-mctc/tad-mctc/issues
-Classifier: Framework :: Pytest
+Keywords: pytorch,autograd,computational chemistry,quantum chemistry
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -22,14 +23,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: opt-einsum
+Requires-Dist: psutil
 Requires-Dist: scipy
 Requires-Dist: torch>=1.11
 Requires-Dist: typing-extensions
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: covdefaults; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
@@ -99,21 +101,25 @@
 
 
 This library is a collection of utility functions that are used in PyTorch (re-)implementations of projects from the [Grimme group](https://github.com/grimme-lab).
 In particular, the *tad-mctc* library provides:
 
 - autograd functions (Jacobian, Hessian)
 
+- atomic data (radii, EN, example molecules, ...)
+
 - batch utility (packing, masks, ...)
 
-- atomic data (radii, EN, example molecules, ...)
+- conversion functions (numpy, atmoic symbols/numbers, ...)
 
-- io (reading coordinate files)
+- coordination numbers (DFT-D3, DFT-D4, EEQ)
 
-- coordination numbers
+- io (reading/writing coordinate files)
+
+- molecular properties (bond lengths/orders/angles, moment of inertia, ...)
 
 - safeops (autograd-safe implementations of common functions)
 
 - typing (base class for tensor-like behavior of arbitrary classes)
 
 - units
 
@@ -155,16 +161,18 @@
 ```sh
 pip install .
 ```
 
 The following dependencies are required
 
 - [numpy](https://numpy.org/)
-- [torch](https://pytorch.org/)
+- [opt_einsum](https://optimized-einsum.readthedocs.io/en/stable/)
+- [psutil](https://psutil.readthedocs.io/en/latest/)
 - [pytest](https://docs.pytest.org/) (tests only)
+- [torch](https://pytorch.org/)
 
 ## Development
 
 For development, additionally install the following tools in your environment.
 
 ```sh
 mamba install black covdefaults mypy pre-commit pylint pytest pytest-cov pytest-xdist tox
```

#### html2text {}

```diff
@@ -1,59 +1,65 @@
-Metadata-Version: 2.1 Name: tad_mctc Version: 0.1.3 Summary: Torch Autodiff
+Metadata-Version: 2.1 Name: tad_mctc Version: 0.1.4 Summary: Torch Autodiff
 Utility Home-page: https://github.com/tad-mctc/tad-mctc Author: "Marvin Friede"
 License: Apache-2.0 Project-URL: Documentation, https://tad-mctc.readthedocs.io
 Project-URL: Source, https://github.com/tad-mctc/tad-mctc Project-URL: Tracker,
-https://github.com/tad-mctc/tad-mctc/issues Classifier: Framework :: Pytest
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Natural Language :: English Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
-3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Scientific/Engineering Classifier: Typing :: Typed
-Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: numpy Requires-Dist: opt-einsum Requires-Dist: scipy
-Requires-Dist: torch>=1.11 Requires-Dist: typing-extensions Provides-Extra: dev
-Requires-Dist: black; extra == "dev" Requires-Dist: covdefaults; extra == "dev"
-Requires-Dist: mypy; extra == "dev" Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pylint; extra == "dev" Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev" Requires-Dist: pytest-random-order;
-extra == "dev" Requires-Dist: pytest-xdist; extra == "dev" Requires-Dist:
-scipy; extra == "dev" Requires-Dist: tox; extra == "dev" Provides-Extra: tox
-Requires-Dist: covdefaults; extra == "tox" Requires-Dist: pytest; extra ==
-"tox" Requires-Dist: pytest-cov; extra == "tox" Requires-Dist: pytest-random-
-order; extra == "tox" Requires-Dist: pytest-xdist; extra == "tox" Requires-
-Dist: scipy; extra == "tox" # Torch Autodiff Utility
+https://github.com/tad-mctc/tad-mctc/issues Keywords:
+pytorch,autograd,computational chemistry,quantum chemistry Classifier: Intended
+Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
+Software License Classifier: Natural Language :: English Classifier: Operating
+System :: OS Independent Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python ::
+Implementation :: CPython Classifier: Topic :: Scientific/Engineering
+Classifier: Typing :: Typed Requires-Python: >=3.8 Description-Content-Type:
+text/markdown License-File: LICENSE Requires-Dist: numpy Requires-Dist: opt-
+einsum Requires-Dist: psutil Requires-Dist: scipy Requires-Dist: torch>=1.11
+Requires-Dist: typing-extensions Provides-Extra: dev Requires-Dist: black;
+extra == "dev" Requires-Dist: covdefaults; extra == "dev" Requires-Dist: mypy;
+extra == "dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist: pylint;
+extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-cov;
+extra == "dev" Requires-Dist: pytest-random-order; extra == "dev" Requires-
+Dist: pytest-xdist; extra == "dev" Requires-Dist: scipy; extra == "dev"
+Requires-Dist: tox; extra == "dev" Provides-Extra: tox Requires-Dist:
+covdefaults; extra == "tox" Requires-Dist: pytest; extra == "tox" Requires-
+Dist: pytest-cov; extra == "tox" Requires-Dist: pytest-random-order; extra ==
+"tox" Requires-Dist: pytest-xdist; extra == "tox" Requires-Dist: scipy; extra
+== "tox" # Torch Autodiff Utility
 Compatibility: [Python Versions][PyTorch Versions]
 Availability:  _[_R_e_l_e_a_s_e_]_[_P_y_P_I_]_[_A_p_a_c_h_e_-_2_._0_]
 Status:        _[_T_e_s_t_ _S_t_a_t_u_s_]_[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_p_r_e_-_c_o_m_m_i_t_._c_i
                _S_t_a_t_u_s_]_[_C_o_v_e_r_a_g_e_]
 
 This library is a collection of utility functions that are used in PyTorch (re-
 )implementations of projects from the [Grimme group](https://github.com/grimme-
 lab). In particular, the *tad-mctc* library provides: - autograd functions
-(Jacobian, Hessian) - batch utility (packing, masks, ...) - atomic data (radii,
-EN, example molecules, ...) - io (reading coordinate files) - coordination
-numbers - safeops (autograd-safe implementations of common functions) - typing
-(base class for tensor-like behavior of arbitrary classes) - units The name is
-inspired by the Fortran pendant "modular computation tool chain library" (
-[mctc-lib](https://github.com/grimme-lab/mctc-lib/)). ## Installation ### pip
-*tad-mctc* can easily be installed with ``pip``. ```sh pip install tad-mctc ```
-### From source This project is hosted on GitHub at [tad-mctc/tad-mctc](https:/
-/github.com/tad-mctc/tad-mctc/). Obtain the source by cloning the repository
-with ```sh git clone https://github.com/tad-mctc/tad-mctc cd tad-mctc ``` We
-recommend using a [conda](https://conda.io/) environment to install the
-package. You can setup the environment manager using a [mambaforge](https://
-github.com/conda-forge/miniforge) installer. Install the required dependencies
-from the conda-forge channel. ```sh mamba env create -n torch -
-f environment.yaml mamba activate torch ``` Install this project with ``pip``
-in the environment ```sh pip install . ``` The following dependencies are
-required - [numpy](https://numpy.org/) - [torch](https://pytorch.org/) -
-[pytest](https://docs.pytest.org/) (tests only) ## Development For development,
+(Jacobian, Hessian) - atomic data (radii, EN, example molecules, ...) - batch
+utility (packing, masks, ...) - conversion functions (numpy, atmoic symbols/
+numbers, ...) - coordination numbers (DFT-D3, DFT-D4, EEQ) - io (reading/
+writing coordinate files) - molecular properties (bond lengths/orders/angles,
+moment of inertia, ...) - safeops (autograd-safe implementations of common
+functions) - typing (base class for tensor-like behavior of arbitrary classes)
+- units The name is inspired by the Fortran pendant "modular computation tool
+chain library" ([mctc-lib](https://github.com/grimme-lab/mctc-lib/)). ##
+Installation ### pip *tad-mctc* can easily be installed with ``pip``. ```sh pip
+install tad-mctc ``` ### From source This project is hosted on GitHub at [tad-
+mctc/tad-mctc](https://github.com/tad-mctc/tad-mctc/). Obtain the source by
+cloning the repository with ```sh git clone https://github.com/tad-mctc/tad-
+mctc cd tad-mctc ``` We recommend using a [conda](https://conda.io/
+) environment to install the package. You can setup the environment manager
+using a [mambaforge](https://github.com/conda-forge/miniforge) installer.
+Install the required dependencies from the conda-forge channel. ```sh mamba env
+create -n torch -f environment.yaml mamba activate torch ``` Install this
+project with ``pip`` in the environment ```sh pip install . ``` The following
+dependencies are required - [numpy](https://numpy.org/) - [opt_einsum](https://
+optimized-einsum.readthedocs.io/en/stable/) - [psutil](https://
+psutil.readthedocs.io/en/latest/) - [pytest](https://docs.pytest.org/) (tests
+only) - [torch](https://pytorch.org/) ## Development For development,
 additionally install the following tools in your environment. ```sh mamba
 install black covdefaults mypy pre-commit pylint pytest pytest-cov pytest-xdist
 tox pip install pytest-random-order ``` With pip, add the option ``-e`` for
 installing in development mode, and add ``[dev]`` for the development
 dependencies ```sh pip install -e .[dev] ``` The pre-commit hooks are
 initialized by running the following command in the root of the repository.
 ```sh pre-commit install ``` For testing all Python environments, simply run
```

### Comparing `tad_mctc-0.1.3/README.md` & `tad_mctc-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -48,21 +48,25 @@
 
 
 This library is a collection of utility functions that are used in PyTorch (re-)implementations of projects from the [Grimme group](https://github.com/grimme-lab).
 In particular, the *tad-mctc* library provides:
 
 - autograd functions (Jacobian, Hessian)
 
+- atomic data (radii, EN, example molecules, ...)
+
 - batch utility (packing, masks, ...)
 
-- atomic data (radii, EN, example molecules, ...)
+- conversion functions (numpy, atmoic symbols/numbers, ...)
 
-- io (reading coordinate files)
+- coordination numbers (DFT-D3, DFT-D4, EEQ)
 
-- coordination numbers
+- io (reading/writing coordinate files)
+
+- molecular properties (bond lengths/orders/angles, moment of inertia, ...)
 
 - safeops (autograd-safe implementations of common functions)
 
 - typing (base class for tensor-like behavior of arbitrary classes)
 
 - units
 
@@ -104,16 +108,18 @@
 ```sh
 pip install .
 ```
 
 The following dependencies are required
 
 - [numpy](https://numpy.org/)
-- [torch](https://pytorch.org/)
+- [opt_einsum](https://optimized-einsum.readthedocs.io/en/stable/)
+- [psutil](https://psutil.readthedocs.io/en/latest/)
 - [pytest](https://docs.pytest.org/) (tests only)
+- [torch](https://pytorch.org/)
 
 ## Development
 
 For development, additionally install the following tools in your environment.
 
 ```sh
 mamba install black covdefaults mypy pre-commit pylint pytest pytest-cov pytest-xdist tox
```

#### html2text {}

```diff
@@ -3,32 +3,36 @@
 Availability:  _[_R_e_l_e_a_s_e_]_[_P_y_P_I_]_[_A_p_a_c_h_e_-_2_._0_]
 Status:        _[_T_e_s_t_ _S_t_a_t_u_s_]_[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_p_r_e_-_c_o_m_m_i_t_._c_i
                _S_t_a_t_u_s_]_[_C_o_v_e_r_a_g_e_]
 
 This library is a collection of utility functions that are used in PyTorch (re-
 )implementations of projects from the [Grimme group](https://github.com/grimme-
 lab). In particular, the *tad-mctc* library provides: - autograd functions
-(Jacobian, Hessian) - batch utility (packing, masks, ...) - atomic data (radii,
-EN, example molecules, ...) - io (reading coordinate files) - coordination
-numbers - safeops (autograd-safe implementations of common functions) - typing
-(base class for tensor-like behavior of arbitrary classes) - units The name is
-inspired by the Fortran pendant "modular computation tool chain library" (
-[mctc-lib](https://github.com/grimme-lab/mctc-lib/)). ## Installation ### pip
-*tad-mctc* can easily be installed with ``pip``. ```sh pip install tad-mctc ```
-### From source This project is hosted on GitHub at [tad-mctc/tad-mctc](https:/
-/github.com/tad-mctc/tad-mctc/). Obtain the source by cloning the repository
-with ```sh git clone https://github.com/tad-mctc/tad-mctc cd tad-mctc ``` We
-recommend using a [conda](https://conda.io/) environment to install the
-package. You can setup the environment manager using a [mambaforge](https://
-github.com/conda-forge/miniforge) installer. Install the required dependencies
-from the conda-forge channel. ```sh mamba env create -n torch -
-f environment.yaml mamba activate torch ``` Install this project with ``pip``
-in the environment ```sh pip install . ``` The following dependencies are
-required - [numpy](https://numpy.org/) - [torch](https://pytorch.org/) -
-[pytest](https://docs.pytest.org/) (tests only) ## Development For development,
+(Jacobian, Hessian) - atomic data (radii, EN, example molecules, ...) - batch
+utility (packing, masks, ...) - conversion functions (numpy, atmoic symbols/
+numbers, ...) - coordination numbers (DFT-D3, DFT-D4, EEQ) - io (reading/
+writing coordinate files) - molecular properties (bond lengths/orders/angles,
+moment of inertia, ...) - safeops (autograd-safe implementations of common
+functions) - typing (base class for tensor-like behavior of arbitrary classes)
+- units The name is inspired by the Fortran pendant "modular computation tool
+chain library" ([mctc-lib](https://github.com/grimme-lab/mctc-lib/)). ##
+Installation ### pip *tad-mctc* can easily be installed with ``pip``. ```sh pip
+install tad-mctc ``` ### From source This project is hosted on GitHub at [tad-
+mctc/tad-mctc](https://github.com/tad-mctc/tad-mctc/). Obtain the source by
+cloning the repository with ```sh git clone https://github.com/tad-mctc/tad-
+mctc cd tad-mctc ``` We recommend using a [conda](https://conda.io/
+) environment to install the package. You can setup the environment manager
+using a [mambaforge](https://github.com/conda-forge/miniforge) installer.
+Install the required dependencies from the conda-forge channel. ```sh mamba env
+create -n torch -f environment.yaml mamba activate torch ``` Install this
+project with ``pip`` in the environment ```sh pip install . ``` The following
+dependencies are required - [numpy](https://numpy.org/) - [opt_einsum](https://
+optimized-einsum.readthedocs.io/en/stable/) - [psutil](https://
+psutil.readthedocs.io/en/latest/) - [pytest](https://docs.pytest.org/) (tests
+only) - [torch](https://pytorch.org/) ## Development For development,
 additionally install the following tools in your environment. ```sh mamba
 install black covdefaults mypy pre-commit pylint pytest pytest-cov pytest-xdist
 tox pip install pytest-random-order ``` With pip, add the option ``-e`` for
 installing in development mode, and add ``[dev]`` for the development
 dependencies ```sh pip install -e .[dev] ``` The pre-commit hooks are
 initialized by running the following command in the root of the repository.
 ```sh pre-commit install ``` For testing all Python environments, simply run
```

### Comparing `tad_mctc-0.1.3/pyproject.toml` & `tad_mctc-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/setup.cfg` & `tad_mctc-0.1.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -5,37 +5,43 @@
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tad-mctc/tad-mctc
 author = "Marvin Friede"
 license = Apache-2.0
 license_files = LICENSE
 classifiers = 
-	Framework :: Pytest
+	Intended Audience :: Science/Research
 	License :: OSI Approved :: Apache Software License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Scientific/Engineering
 	Typing :: Typed
+keywords = 
+	pytorch
+	autograd
+	computational chemistry
+	quantum chemistry
 project_urls = 
 	Documentation = https://tad-mctc.readthedocs.io
 	Source = https://github.com/tad-mctc/tad-mctc
 	Tracker = https://github.com/tad-mctc/tad-mctc/issues
 
 [options]
 packages = find:
 install_requires = 
 	numpy
 	opt-einsum
+	psutil
 	scipy
 	torch>=1.11
 	typing-extensions
 python_requires = >=3.8
 package_dir = 
 	=src
```

### Comparing `tad_mctc-0.1.3/setup.py` & `tad_mctc-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/__init__.py` & `tad_mctc-0.1.4/src/tad_mctc/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,42 +14,47 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """
 Torch Autodiff Utilities
 ========================
 
-This library is a collection of utility functions that are used in PyTorch (re-)implementations of projects from the `Grimme group <https://github.com/grimme-lab>`__.
+This library is a collection of utility functions that are used in PyTorch (re-)
+implementations of projects from the
+`Grimme group <https://github.com/grimme-lab>`__.
 In particular, the *tad-mctc* library provides:
 
 - autograd functions (Jacobian, Hessian)
 
 - atomic data (radii, EN, example molecules, ...)
 
 - batch utility (packing, masks, ...)
 
+- conversion functions (numpy, atmoic symbols/numbers, ...)
+
 - coordination numbers (DFT-D3, DFT-D4, EEQ)
 
-- io (reading coordinate files)
+- io (reading/writing coordinate files)
 
 - molecular properties (bond lengths/orders/angles, moment of inertia, ...)
 
 - safeops (autograd-safe implementations of common functions)
 
 - typing (base class for tensor-like behavior of arbitrary classes)
 
 - units
 
-The name is inspired by the Fortran pendant "modular computation tool chain library" (`mctc-lib <https://github.com/grimme-lab/mctc-lib/>`__).
+The name is inspired by the Fortran pendant "modular computation tool chain
+library" (`mctc-lib <https://github.com/grimme-lab/mctc-lib/>`__).
 
 .. note::
 
    This project is still in early development and the API is subject to change.
    Contributions are welcome, please checkout our
-   `contributing guidelines <https://github.com/dftd4/tad_mctc/blob/main/CONTRIBUTING.md>`_.
+   `contributing guidelines <https://github.com/tad-mctc/tad-mctc/blob/main/CONTRIBUTING.md>`_.
 
 Example
 -------
 >>> import torch
 >>> import tad_mctc as mctc
 >>>
 >>> # S22 system 4: formamide dimer
```

### Comparing `tad_mctc-0.1.3/src/tad_mctc/_version.py` & `tad_mctc-0.1.4/src/tad_mctc/_version.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,9 +46,9 @@
             f"versioning scheme of MAJOR.MINOR.PATCH ({s})."
         )
 
     version_numbers = [int(part) for part in s[:3]]
     return tuple(version_numbers)
 
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __tversion__ = version_tuple(torch.__version__)
```

### Comparing `tad_mctc-0.1.3/src/tad_mctc/autograd/__init__.py` & `tad_mctc-0.1.4/src/tad_mctc/autograd/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/autograd/batched.py` & `tad_mctc-0.1.4/src/tad_mctc/autograd/batched.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/autograd/compat.py` & `tad_mctc-0.1.4/src/tad_mctc/autograd/compat.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/autograd/gradcheck.py` & `tad_mctc-0.1.4/src/tad_mctc/autograd/gradcheck.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/autograd/hessian.py` & `tad_mctc-0.1.4/src/tad_mctc/autograd/hessian.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/autograd/internals.py` & `tad_mctc-0.1.4/src/tad_mctc/autograd/internals.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,16 @@
     from .compat import jacrev_compat as jacrev
     from .compat import vmap_compat as vmap
 
     try:
         from functorch import jacrev as fjacrev  # type: ignore[import-error]
         from functorch import vmap as fvmap  # type: ignore[import-error]
     except ModuleNotFoundError:
+        # pylint: disable=invalid-name
         fjacrev = None
         fvmap = None
 else:
-    from torch.func import jacrev as jacrev  # type: ignore[import-error]
+    from torch.func import jacrev  # type: ignore[import-error]
     from torch.func import vmap  # type: ignore[import-error]
 
     fjacrev = jacrev
     fvmap = vmap
```

### Comparing `tad_mctc-0.1.3/src/tad_mctc/autograd/nonfunctorch.py` & `tad_mctc-0.1.4/src/tad_mctc/autograd/nonfunctorch.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/batch/__init__.py` & `tad_mctc-0.1.4/src/tad_mctc/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/batch/agnostic.py` & `tad_mctc-0.1.4/src/tad_mctc/batch/agnostic.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/batch/mask/__init__.py` & `tad_mctc-0.1.4/src/tad_mctc/batch/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/batch/mask/atoms.py` & `tad_mctc-0.1.4/src/tad_mctc/batch/mask/atoms.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/batch/mask/jit.py` & `tad_mctc-0.1.4/src/tad_mctc/batch/mask/jit.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/batch/mask/pairs.py` & `tad_mctc-0.1.4/src/tad_mctc/batch/mask/pairs.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/batch/mask/triples.py` & `tad_mctc-0.1.4/src/tad_mctc/batch/mask/triples.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/batch/pack.py` & `tad_mctc-0.1.4/src/tad_mctc/batch/pack.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/batch/unpack.py` & `tad_mctc-0.1.4/src/tad_mctc/batch/unpack.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/convert/__init__.py` & `tad_mctc-0.1.4/src/tad_mctc/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/convert/numpy.py` & `tad_mctc-0.1.4/src/tad_mctc/convert/numpy.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/convert/pse.py` & `tad_mctc-0.1.4/src/tad_mctc/convert/pse.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/convert/pytorch.py` & `tad_mctc-0.1.4/src/tad_mctc/convert/pytorch.py`

 * *Files 14% similar despite different names*

```diff
@@ -94,30 +94,30 @@
         If `x` is a string that cannot be converted to a float or if the list
         contains elements other than float, int, or bool.
     TypeError
         If `x` is of a type that cannot be converted to a tensor.
 
     Examples
     --------
-    >>> totensor(3.14)
+    >>> any_to_tensor(3.14)
     tensor(3.1400)
 
-    >>> totensor(42, dtype=torch.float32)
+    >>> any_to_tensor(42, dtype=torch.float32)
     tensor(42.)
 
-    >>> totensor(True)
+    >>> any_to_tensor(True)
     tensor(True)
 
-    >>> totensor('2.718')
+    >>> any_to_tensor('2.718')
     tensor(2.7180)
 
-    >>> totensor('not_a_number')
+    >>> any_to_tensor('not_a_number')
     ValueError: Cannot convert string 'not_a_number' to float
 
-    >>> totensor(["1", "2"])
+    >>> any_to_tensor(["1", "2"])
     TypeError: Tensor-incompatible type '<class 'list'>' of variable ["1", "2"].
     """
     if isinstance(x, Tensor):
         return x.to(device=device, dtype=dtype)
 
     if isinstance(x, list):
         if all(isinstance(item, (float, int, bool)) for item in x):
```

### Comparing `tad_mctc-0.1.3/src/tad_mctc/convert/tensor.py` & `tad_mctc-0.1.4/src/tad_mctc/convert/tensor.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/data/__init__.py` & `tad_mctc-0.1.4/src/tad_mctc/data/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/data/en.py` & `tad_mctc-0.1.4/src/tad_mctc/data/en.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/data/getters.py` & `tad_mctc-0.1.4/src/tad_mctc/data/getters.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/data/mass.py` & `tad_mctc-0.1.4/src/tad_mctc/data/mass.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/data/molecules.py` & `tad_mctc-0.1.4/src/tad_mctc/data/molecules.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/data/pse.py` & `tad_mctc-0.1.4/src/tad_mctc/data/pse.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/data/radii.py` & `tad_mctc-0.1.4/src/tad_mctc/data/radii.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/data/zeff.py` & `tad_mctc-0.1.4/src/tad_mctc/data/zeff.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/exceptions/__init__.py` & `tad_mctc-0.1.4/src/tad_mctc/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/exceptions/io.py` & `tad_mctc-0.1.4/src/tad_mctc/exceptions/io.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/exceptions/molecule.py` & `tad_mctc-0.1.4/src/tad_mctc/exceptions/molecule.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/exceptions/pytorch.py` & `tad_mctc-0.1.4/src/tad_mctc/exceptions/pytorch.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/io/__init__.py` & `tad_mctc-0.1.4/src/tad_mctc/io/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/io/checks/__init__.py` & `tad_mctc-0.1.4/src/tad_mctc/io/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/io/checks/molecule.py` & `tad_mctc-0.1.4/src/tad_mctc/io/checks/molecule.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,48 +31,56 @@
 value (default: 0) is the same as a triple of atomic positions, which would
 obscure the distinction between padding and actual atomic positions in batched
 calculations. This primarily occurs for single atoms, which are usually placed
 at the origin.
 The behavior of this check is best controlled through keyword arguments of the
 respective readers. The available keyword arguments are:
 - padding_value (`float | int`, default: 0): Value for padding used in check
-- raise_padding_exception (`bool`, default: False): Raise an exception (or just a warning)
+- raise_padding_exception (`bool`, default: False): Raise an exception (or just
+a warning)
 - raise_padding_warning (`bool`, default: True): Raise a warning
-- shift_for_last (`bool`, default: False): Automatically shift all positions by a constant if a clash is detected
+- shift_for_last (`bool`, default: False): Automatically shift all positions by
+a constant if a clash is detected
 - shift_value (`float | int`, default: 1.0): Constant for shift.
 
 For more details and examples, check `test/test_io/test_deflatable.py`.
 """
 from __future__ import annotations
 
 import torch
 
 from ... import storch
 from ...batch import deflate, real_pairs
 from ...data import pse
 from ...exceptions import MoleculeError, MoleculeWarning
-from ...typing import DD, IO, Any, Tensor
+from ...typing import DD, IO, Any, NoReturn, Tensor
 
-__all__ = ["coldfusion_check", "content_checks", "deflatable_check"]
+__all__ = [
+    "coldfusion_check",
+    "content_checks",
+    "deflatable_check",
+    "dimension_check",
+]
 
 
 def coldfusion_check(
     numbers: Tensor, positions: Tensor, threshold: Tensor | float | int | None = None
-) -> bool:
+) -> bool | NoReturn:
     """
     Check if interatomic distances are large enough (no fusion of atoms).
 
     Parameters
     ----------
     numbers : Tensor
         A 1D tensor containing atomic numbers or symbols.
     positions : Tensor
         A 2D tensor of shape (n_atoms, 3) containing atomic positions.
     threshold : Tensor | float | int | None, optional
-        Threshold for acceptable interatomic distances. Defaults to `None`, which resolves to `torch.tensor(torch.finfo(dtype).eps ** 0.75, **dd)`.
+        Threshold for acceptable interatomic distances. Defaults to `None`,
+        which resolves to `torch.tensor(torch.finfo(dtype).eps ** 0.75, **dd)`.
 
     Returns
     -------
     bool
         True of atoms are not too close.
 
     Raises
@@ -95,15 +103,15 @@
     # Check if any distance below the threshold is found
     if torch.any((distances < threshold) & mask):
         raise MoleculeError("Too close interatomic distances found")
 
     return True
 
 
-def content_checks(numbers: Tensor, positions: Tensor) -> bool:
+def content_checks(numbers: Tensor, positions: Tensor) -> bool | NoReturn:
     """
     Check the content of the numbers and positions tensors.
 
     This function should be asserted as it returns `True` on success and raises
     an error on failure.
 
     Parameters
@@ -134,15 +142,15 @@
     assert coldfusion_check(numbers, positions)
 
     return True
 
 
 def deflatable_check(
     positions: Tensor, fileobj: IO[Any] | None = None, **kwargs: Any
-) -> bool:
+) -> bool | NoReturn:
     """
     Check for the last coordinate being at the origin as this might clash with
     padding.
 
     This function should be asserted as it returns `True` on success and raises
     an error on failure.
 
@@ -183,12 +191,65 @@
         # shift all atoms
         if kwargs.pop("shift_for_last", False):
             positions += kwargs.pop("shift_value", 1.0)
             return True
 
         # issue warning
         if kwargs.pop("raise_padding_warning", True):
+            # pylint: disable=import-outside-toplevel
             from warnings import warn
 
             warn(msg, MoleculeWarning)
 
     return True
+
+
+def dimension_check(
+    x: Any,
+    min_ndim: int = -1,
+    max_ndim: int = 9999,
+) -> bool | NoReturn:
+    """
+    Check if the number of dimensions of a tensor is within a certain range.
+
+    Parameters
+    ----------
+    x : Any
+        The tensor to check.
+    min_ndim : int, optional
+        Minimum number of dimensions for the tensor. Defaults to `-1`.
+    max_ndim : int, optional
+        Maximum number of dimensions for the tensor. Defaults to `9999`.
+
+    Returns
+    -------
+    None | NoReturn
+        Returns `None` if the tensor has the correct number of dimensions.
+
+    Raises
+    ------
+    TypeError
+        If the input is not a tensor.
+    RuntimeError
+        If the number of dimensions is not within the specified range.
+
+    Examples
+    --------
+    >>> import torch
+    >>> from tad_mctc.io.checks.molecule import dimension_check
+    >>> x = torch.tensor([1, 2, 3])
+    >>> dimension_check(x, min_ndim=1, max_ndim=1)
+    True
+    >>> dimension_check(x, min_ndim=2, max_ndim=2)
+    Traceback (most recent call last):
+    ...
+    RuntimeError: The tensor should not fall below '2' dimensions.
+    """
+    if not isinstance(x, Tensor):
+        raise TypeError(f"Variable is not a tensor but '{type(x)}'.")
+
+    if x.ndim < min_ndim:
+        raise RuntimeError(f"The tensor should not fall below {min_ndim} dimensions.")
+    if x.ndim > max_ndim:
+        raise RuntimeError(f"The tensor should not exceed '{max_ndim}' dimensions.")
+
+    return True
```

### Comparing `tad_mctc-0.1.3/src/tad_mctc/io/checks/shape.py` & `tad_mctc-0.1.4/src/tad_mctc/io/checks/shape.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,16 @@
         raise ValueError(
             f"Shape of positions ({positions.shape[:-1]}) is not consistent "
             f"with atomic numbers ({numbers.shape})."
         )
 
     if positions.shape[-1] != 3:
         raise ValueError(
-            f"The last dimension of the position tensor must present the cartesian directions, i.e., it must be size 3 (but is {positions.shape[-1]}"
+            "The last dimension of the position tensor must present the "
+            "cartesian directions, i.e., it must be size 3 (but is "
+            f"{positions.shape[-1]}"
         )
 
     if len(numbers.shape) != 1 or len(positions.shape) != 2:
         raise ValueError("Invalid shape for tensors (batched tensors not allowed).")
 
     return True
```

### Comparing `tad_mctc-0.1.3/src/tad_mctc/io/read/__init__.py` & `tad_mctc-0.1.4/src/tad_mctc/io/read/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/io/read/dotfiles.py` & `tad_mctc-0.1.4/src/tad_mctc/io/read/dotfiles.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/io/read/frompath.py` & `tad_mctc-0.1.4/src/tad_mctc/io/read/frompath.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,24 +37,28 @@
 from ...typing import IO, Any, Literal, PathLike, Protocol, Tensor
 
 __all__ = ["create_path_reader", "create_path_reader_dotfiles"]
 
 
 @runtime_checkable
 class ReaderFunction(Protocol):
+    """Type annotation for a reader function."""
+
     def __call__(
         self,
         fileobj: IO[Any],
         device: torch.device | None = None,
         dtype: torch.dtype | None = None,
     ) -> Tensor | tuple[Tensor, Tensor]: ...
 
 
 @runtime_checkable
 class FileReaderFunction(Protocol):
+    """Type annotation for a file reader function."""
+
     def __call__(
         self,
         filepath: PathLike,
         mode: str = "r",
         encoding: str = "utf-8",
         device: torch.device | None = None,
         dtype: torch.dtype | None = None,
@@ -124,24 +128,28 @@
 
 
 ################################################################################
 
 
 @runtime_checkable
 class ReaderFunctionTensor(Protocol):
+    """Type annotation for a reader function that returns a tensor."""
+
     def __call__(
         self,
         fileobj: IO[Any],
         device: torch.device | None = None,
         dtype: torch.dtype | None = None,
     ) -> Tensor: ...
 
 
 @runtime_checkable
 class FileReaderFunctionTensor(Protocol):
+    """Type annotation for a file reader function that returns a tensor."""
+
     def __call__(
         self,
         filepath: PathLike,
         mode: str = "r",
         encoding: str = "utf-8",
         device: torch.device | None = None,
         dtype: torch.dtype | None = None,
@@ -165,15 +173,15 @@
     -------
     FileReaderFunction
         A function that takes a file path, mode, device, and dtype, and returns
         the processed data.
     """
     # return default if file is not found (must be integer to allow integer
     # dtypes from PyTorch, e.g., 0.0 fails with torch.long)
-    DEFAULT_VALUE = 0
+    default_value = 0
 
     def read_from_path(
         filepath: PathLike,
         mode: str = "r",
         encoding: str = "utf-8",
         device: torch.device | None = None,
         dtype: torch.dtype | None = None,
@@ -207,13 +215,13 @@
                 path = path.parent / name
 
         if path.is_dir():
             path = path / name
 
         # Check if the file now exists
         if not path.exists():
-            return torch.tensor(DEFAULT_VALUE, device=device, dtype=dtype)
+            return torch.tensor(default_value, device=device, dtype=dtype)
 
         with open(path, mode=mode, encoding=encoding) as fileobj:
             return reader_function(fileobj, device, dtype)
 
     return read_from_path
```

### Comparing `tad_mctc-0.1.3/src/tad_mctc/io/read/orca.py` & `tad_mctc-0.1.4/src/tad_mctc/io/read/orca.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/io/read/qcschema.py` & `tad_mctc-0.1.4/src/tad_mctc/io/read/qcschema.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     """
     dd: DD = {
         "device": device,
         "dtype": dtype if dtype is not None else get_default_dtype(),
     }
     ddi: DD = {"device": device, "dtype": dtype_int}
 
-    # pylint: disable=import-beyond-top-level
+    # pylint: disable=import-outside-toplevel
     from json import loads as json_load
 
     data = json_load(fileobj.read())
 
     if "molecule" not in data:
         raise KeyError(f"Invalid schema: Key 'molecule' not found in '{fileobj}'.")
```

### Comparing `tad_mctc-0.1.3/src/tad_mctc/io/read/reader.py` & `tad_mctc-0.1.4/src/tad_mctc/io/read/reader.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/io/read/tblite.py` & `tad_mctc-0.1.4/src/tad_mctc/io/read/tblite.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         The file-like object to read from.
 
     Returns
     -------
     dict[str, str | float]
         Full tblite JSON output.
     """
+    # pylint: disable=import-outside-toplevel
     from json import loads as json_load
 
     return json_load(fileobj.read())
 
 
 def read_tblite_engrad(
     fileobj: IO[Any],
```

### Comparing `tad_mctc-0.1.3/src/tad_mctc/io/read/turbomole.py` & `tad_mctc-0.1.4/src/tad_mctc/io/read/turbomole.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/io/read/xyz.py` & `tad_mctc-0.1.4/src/tad_mctc/io/read/xyz.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/io/write/__init__.py` & `tad_mctc-0.1.4/src/tad_mctc/io/write/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/io/write/turbomole.py` & `tad_mctc-0.1.4/src/tad_mctc/io/write/turbomole.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/io/write/writer.py` & `tad_mctc-0.1.4/src/tad_mctc/io/write/writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,25 +28,29 @@
 from ...typing import IO, Any, PathLike, Protocol, Tensor, runtime_checkable
 
 __all__ = ["create_path_writer"]
 
 
 @runtime_checkable
 class WriterFunction(Protocol):
+    """Type annotation for a writer function."""
+
     def __call__(
         self,
         fileobj: IO[Any],
         numbers: Tensor,
         positions: Tensor,
         **kwargs: Any,
     ) -> None: ...
 
 
 @runtime_checkable
 class FileWriterFunction(Protocol):
+    """Type annotation for a file writer function."""
+
     def __call__(
         self,
         filepath: PathLike,
         numbers: Tensor,
         positions: Tensor,
         mode: str = "w",
         fmt: str = "%22.15f",
@@ -63,15 +67,16 @@
     ----------
     writer_function : WriterFunction
         The function used to write the file contents.
 
     Returns
     -------
     FileWriterFunction
-        A function that takes a file path, numbers, positions, mode, comment, and format string, and writes the data to the file.
+        A function that takes a file path, numbers, positions, mode, comment,
+        and format string, and writes the data to the file.
     """
 
     @wraps(writer_function)
     def write_to_path(
         filepath: PathLike,
         numbers: Tensor,
         positions: Tensor,
```

### Comparing `tad_mctc-0.1.3/src/tad_mctc/io/write/xyz.py` & `tad_mctc-0.1.4/src/tad_mctc/io/write/xyz.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/math/__init__.py` & `tad_mctc-0.1.4/src/tad_mctc/math/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/math/einsum.py` & `tad_mctc-0.1.4/src/tad_mctc/math/einsum.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/molecule/__init__.py` & `tad_mctc-0.1.4/src/tad_mctc/molecule/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,9 +17,11 @@
 """
 Molecule
 ========
 
 Collection of utility functions for calculations related to a molecule.
 """
 
+from .bond import *
+from .container import *
 from .geometry import *
 from .property import *
```

### Comparing `tad_mctc-0.1.3/src/tad_mctc/molecule/bond.py` & `tad_mctc-0.1.4/src/tad_mctc/molecule/bond.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,20 +63,22 @@
         [False,  True, False, False, False, False, False, False]])
 """
 
 from __future__ import annotations
 
 import torch
 
-from tad_mctc import storch
-
+from .. import storch
 from ..batch import real_pairs
 from ..ncoord import defaults, erf_count
 from ..typing import DD, Any, CountingFunction, Tensor
 
+__all__ = ["guess_bond_length", "guess_bond_order"]
+
+
 _en = torch.tensor(
     [
         *[+0.00000000],
         *[+2.30085633, +2.78445145, +1.52956084, +1.51714704, +2.20568300],
         *[+2.49640820, +2.81007174, +4.51078438, +4.67476223, +3.29383610],
         *[+2.84505365, +2.20047950, +2.31739628, +2.03636974, +1.97558064],
         *[+2.13446570, +2.91638164, +1.54098156, +2.91656301, +2.26312147],
```

### Comparing `tad_mctc-0.1.3/src/tad_mctc/molecule/geometry.py` & `tad_mctc-0.1.4/src/tad_mctc/molecule/geometry.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/molecule/property.py` & `tad_mctc-0.1.4/src/tad_mctc/molecule/property.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/ncoord/__init__.py` & `tad_mctc-0.1.4/src/tad_mctc/ncoord/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/ncoord/count.py` & `tad_mctc-0.1.4/src/tad_mctc/ncoord/count.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/ncoord/d3.py` & `tad_mctc-0.1.4/src/tad_mctc/ncoord/d3.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/ncoord/d4.py` & `tad_mctc-0.1.4/src/tad_mctc/ncoord/d4.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/ncoord/defaults.py` & `tad_mctc-0.1.4/src/tad_mctc/ncoord/defaults.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/ncoord/eeq.py` & `tad_mctc-0.1.4/src/tad_mctc/ncoord/eeq.py`

 * *Files 9% similar despite different names*

```diff
@@ -117,14 +117,30 @@
 
     return cut_coordination_number(cn, cn_max)
 
 
 def cut_coordination_number(
     cn: Tensor, cn_max: Tensor | float | int = defaults.CUTOFF_EEQ_MAX
 ) -> Tensor:
+    """
+    Cut the coordination number at a maximum value.
+
+    Parameters
+    ----------
+    cn : Tensor
+        Coordination numbers.
+    cn_max : Tensor | float | int, optional
+        Maximum coordination number.
+        Defaults to :const:`tad_mctc.ncoord.defaults.CUTOFF_EEQ_MAX`.
+
+    Returns
+    -------
+    Tensor
+        Cut coordination numbers.
+    """
     if isinstance(cn_max, (float, int)):
         cn_max = torch.tensor(cn_max, device=cn.device, dtype=cn.dtype)
 
     if cn_max > 50:
         return cn
 
     return torch.log(1.0 + torch.exp(cn_max)) - torch.log(1.0 + torch.exp(cn_max - cn))
```

### Comparing `tad_mctc-0.1.3/src/tad_mctc/storch/__init__.py` & `tad_mctc-0.1.4/src/tad_mctc/storch/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/storch/distance.py` & `tad_mctc-0.1.4/src/tad_mctc/storch/distance.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/storch/elemental.py` & `tad_mctc-0.1.4/src/tad_mctc/storch/elemental.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/storch/linalg.py` & `tad_mctc-0.1.4/src/tad_mctc/storch/linalg.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/storch/utils.py` & `tad_mctc-0.1.4/src/tad_mctc/storch/utils.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/typing/__init__.py` & `tad_mctc-0.1.4/src/tad_mctc/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/typing/builtin.py` & `tad_mctc-0.1.4/src/tad_mctc/typing/builtin.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/typing/compat.py` & `tad_mctc-0.1.4/src/tad_mctc/typing/compat.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/typing/pytorch.py` & `tad_mctc-0.1.4/src/tad_mctc/typing/pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,20 +235,22 @@
         if dtype not in self.allowed_dtypes:
             raise DtypeError(
                 f"Only '{self.allowed_dtypes}' allowed (received '{dtype}')."
             )
 
         args = {}
         for s in self.__slots__:
-            if not s.startswith("__"):
-                attr = getattr(self, s)
-                if isinstance(attr, Tensor) or issubclass(type(attr), TensorLike):
-                    if attr.dtype in self.allowed_dtypes:
-                        attr = attr.type(dtype)
-                args[s] = attr
+            if s.startswith("__"):
+                continue
+
+            attr = getattr(self, s)
+            if isinstance(attr, Tensor) or issubclass(type(attr), TensorLike):
+                if attr.dtype in self.allowed_dtypes:
+                    attr = attr.type(dtype)
+            args[s] = attr
 
         return self.__class__(**args, dtype=dtype)
 
     def to(self, device: torch.device) -> Self:
         """
         Returns a copy of the `TensorLike` instance on the specified device.
 
@@ -285,14 +287,28 @@
                 attr = getattr(self, s)
                 if isinstance(attr, Tensor) or issubclass(type(attr), TensorLike):
                     attr = attr.to(device=device)
                 args[s] = attr
 
         return self.__class__(**args, device=device)
 
+    def cpu(self) -> Self:
+        """
+        Returns a copy of the `TensorLike` instance on the CPU.
+
+        This method creates and returns a new copy of the `TensorLike` instance
+        on the CPU.
+
+        Returns
+        -------
+        TensorLike
+            A copy of the `TensorLike` instance placed on the CPU.
+        """
+        return self.to(torch.device("cpu"))
+
     @property
     def allowed_dtypes(self) -> tuple[torch.dtype, ...]:
         """
         Specification of dtypes that the TensorLike object can take. Defaults
         to float types and must be overridden by subclass if float are not
         allowed. The IndexHelper is an example that should only allow integers.
```

### Comparing `tad_mctc-0.1.3/src/tad_mctc/units/__init__.py` & `tad_mctc-0.1.4/src/tad_mctc/units/__init__.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/units/codata.py` & `tad_mctc-0.1.4/src/tad_mctc/units/codata.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/units/energy.py` & `tad_mctc-0.1.4/src/tad_mctc/units/energy.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/units/length.py` & `tad_mctc-0.1.4/src/tad_mctc/units/length.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/units/mass.py` & `tad_mctc-0.1.4/src/tad_mctc/units/mass.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/units/math.py` & `tad_mctc-0.1.4/src/tad_mctc/units/math.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/units/spectroscopy.py` & `tad_mctc-0.1.4/src/tad_mctc/units/spectroscopy.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc/units/time.py` & `tad_mctc-0.1.4/src/tad_mctc/units/time.py`

 * *Files identical despite different names*

### Comparing `tad_mctc-0.1.3/src/tad_mctc.egg-info/PKG-INFO` & `tad_mctc-0.1.4/src/tad_mctc.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: tad_mctc
-Version: 0.1.3
+Version: 0.1.4
 Summary: Torch Autodiff Utility
 Home-page: https://github.com/tad-mctc/tad-mctc
 Author: "Marvin Friede"
 License: Apache-2.0
 Project-URL: Documentation, https://tad-mctc.readthedocs.io
 Project-URL: Source, https://github.com/tad-mctc/tad-mctc
 Project-URL: Tracker, https://github.com/tad-mctc/tad-mctc/issues
-Classifier: Framework :: Pytest
+Keywords: pytorch,autograd,computational chemistry,quantum chemistry
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -22,14 +23,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: opt-einsum
+Requires-Dist: psutil
 Requires-Dist: scipy
 Requires-Dist: torch>=1.11
 Requires-Dist: typing-extensions
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: covdefaults; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
@@ -99,21 +101,25 @@
 
 
 This library is a collection of utility functions that are used in PyTorch (re-)implementations of projects from the [Grimme group](https://github.com/grimme-lab).
 In particular, the *tad-mctc* library provides:
 
 - autograd functions (Jacobian, Hessian)
 
+- atomic data (radii, EN, example molecules, ...)
+
 - batch utility (packing, masks, ...)
 
-- atomic data (radii, EN, example molecules, ...)
+- conversion functions (numpy, atmoic symbols/numbers, ...)
 
-- io (reading coordinate files)
+- coordination numbers (DFT-D3, DFT-D4, EEQ)
 
-- coordination numbers
+- io (reading/writing coordinate files)
+
+- molecular properties (bond lengths/orders/angles, moment of inertia, ...)
 
 - safeops (autograd-safe implementations of common functions)
 
 - typing (base class for tensor-like behavior of arbitrary classes)
 
 - units
 
@@ -155,16 +161,18 @@
 ```sh
 pip install .
 ```
 
 The following dependencies are required
 
 - [numpy](https://numpy.org/)
-- [torch](https://pytorch.org/)
+- [opt_einsum](https://optimized-einsum.readthedocs.io/en/stable/)
+- [psutil](https://psutil.readthedocs.io/en/latest/)
 - [pytest](https://docs.pytest.org/) (tests only)
+- [torch](https://pytorch.org/)
 
 ## Development
 
 For development, additionally install the following tools in your environment.
 
 ```sh
 mamba install black covdefaults mypy pre-commit pylint pytest pytest-cov pytest-xdist tox
```

#### html2text {}

```diff
@@ -1,59 +1,65 @@
-Metadata-Version: 2.1 Name: tad_mctc Version: 0.1.3 Summary: Torch Autodiff
+Metadata-Version: 2.1 Name: tad_mctc Version: 0.1.4 Summary: Torch Autodiff
 Utility Home-page: https://github.com/tad-mctc/tad-mctc Author: "Marvin Friede"
 License: Apache-2.0 Project-URL: Documentation, https://tad-mctc.readthedocs.io
 Project-URL: Source, https://github.com/tad-mctc/tad-mctc Project-URL: Tracker,
-https://github.com/tad-mctc/tad-mctc/issues Classifier: Framework :: Pytest
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Natural Language :: English Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
-3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Scientific/Engineering Classifier: Typing :: Typed
-Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: numpy Requires-Dist: opt-einsum Requires-Dist: scipy
-Requires-Dist: torch>=1.11 Requires-Dist: typing-extensions Provides-Extra: dev
-Requires-Dist: black; extra == "dev" Requires-Dist: covdefaults; extra == "dev"
-Requires-Dist: mypy; extra == "dev" Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pylint; extra == "dev" Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev" Requires-Dist: pytest-random-order;
-extra == "dev" Requires-Dist: pytest-xdist; extra == "dev" Requires-Dist:
-scipy; extra == "dev" Requires-Dist: tox; extra == "dev" Provides-Extra: tox
-Requires-Dist: covdefaults; extra == "tox" Requires-Dist: pytest; extra ==
-"tox" Requires-Dist: pytest-cov; extra == "tox" Requires-Dist: pytest-random-
-order; extra == "tox" Requires-Dist: pytest-xdist; extra == "tox" Requires-
-Dist: scipy; extra == "tox" # Torch Autodiff Utility
+https://github.com/tad-mctc/tad-mctc/issues Keywords:
+pytorch,autograd,computational chemistry,quantum chemistry Classifier: Intended
+Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
+Software License Classifier: Natural Language :: English Classifier: Operating
+System :: OS Independent Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python ::
+Implementation :: CPython Classifier: Topic :: Scientific/Engineering
+Classifier: Typing :: Typed Requires-Python: >=3.8 Description-Content-Type:
+text/markdown License-File: LICENSE Requires-Dist: numpy Requires-Dist: opt-
+einsum Requires-Dist: psutil Requires-Dist: scipy Requires-Dist: torch>=1.11
+Requires-Dist: typing-extensions Provides-Extra: dev Requires-Dist: black;
+extra == "dev" Requires-Dist: covdefaults; extra == "dev" Requires-Dist: mypy;
+extra == "dev" Requires-Dist: pre-commit; extra == "dev" Requires-Dist: pylint;
+extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-cov;
+extra == "dev" Requires-Dist: pytest-random-order; extra == "dev" Requires-
+Dist: pytest-xdist; extra == "dev" Requires-Dist: scipy; extra == "dev"
+Requires-Dist: tox; extra == "dev" Provides-Extra: tox Requires-Dist:
+covdefaults; extra == "tox" Requires-Dist: pytest; extra == "tox" Requires-
+Dist: pytest-cov; extra == "tox" Requires-Dist: pytest-random-order; extra ==
+"tox" Requires-Dist: pytest-xdist; extra == "tox" Requires-Dist: scipy; extra
+== "tox" # Torch Autodiff Utility
 Compatibility: [Python Versions][PyTorch Versions]
 Availability:  _[_R_e_l_e_a_s_e_]_[_P_y_P_I_]_[_A_p_a_c_h_e_-_2_._0_]
 Status:        _[_T_e_s_t_ _S_t_a_t_u_s_]_[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_p_r_e_-_c_o_m_m_i_t_._c_i
                _S_t_a_t_u_s_]_[_C_o_v_e_r_a_g_e_]
 
 This library is a collection of utility functions that are used in PyTorch (re-
 )implementations of projects from the [Grimme group](https://github.com/grimme-
 lab). In particular, the *tad-mctc* library provides: - autograd functions
-(Jacobian, Hessian) - batch utility (packing, masks, ...) - atomic data (radii,
-EN, example molecules, ...) - io (reading coordinate files) - coordination
-numbers - safeops (autograd-safe implementations of common functions) - typing
-(base class for tensor-like behavior of arbitrary classes) - units The name is
-inspired by the Fortran pendant "modular computation tool chain library" (
-[mctc-lib](https://github.com/grimme-lab/mctc-lib/)). ## Installation ### pip
-*tad-mctc* can easily be installed with ``pip``. ```sh pip install tad-mctc ```
-### From source This project is hosted on GitHub at [tad-mctc/tad-mctc](https:/
-/github.com/tad-mctc/tad-mctc/). Obtain the source by cloning the repository
-with ```sh git clone https://github.com/tad-mctc/tad-mctc cd tad-mctc ``` We
-recommend using a [conda](https://conda.io/) environment to install the
-package. You can setup the environment manager using a [mambaforge](https://
-github.com/conda-forge/miniforge) installer. Install the required dependencies
-from the conda-forge channel. ```sh mamba env create -n torch -
-f environment.yaml mamba activate torch ``` Install this project with ``pip``
-in the environment ```sh pip install . ``` The following dependencies are
-required - [numpy](https://numpy.org/) - [torch](https://pytorch.org/) -
-[pytest](https://docs.pytest.org/) (tests only) ## Development For development,
+(Jacobian, Hessian) - atomic data (radii, EN, example molecules, ...) - batch
+utility (packing, masks, ...) - conversion functions (numpy, atmoic symbols/
+numbers, ...) - coordination numbers (DFT-D3, DFT-D4, EEQ) - io (reading/
+writing coordinate files) - molecular properties (bond lengths/orders/angles,
+moment of inertia, ...) - safeops (autograd-safe implementations of common
+functions) - typing (base class for tensor-like behavior of arbitrary classes)
+- units The name is inspired by the Fortran pendant "modular computation tool
+chain library" ([mctc-lib](https://github.com/grimme-lab/mctc-lib/)). ##
+Installation ### pip *tad-mctc* can easily be installed with ``pip``. ```sh pip
+install tad-mctc ``` ### From source This project is hosted on GitHub at [tad-
+mctc/tad-mctc](https://github.com/tad-mctc/tad-mctc/). Obtain the source by
+cloning the repository with ```sh git clone https://github.com/tad-mctc/tad-
+mctc cd tad-mctc ``` We recommend using a [conda](https://conda.io/
+) environment to install the package. You can setup the environment manager
+using a [mambaforge](https://github.com/conda-forge/miniforge) installer.
+Install the required dependencies from the conda-forge channel. ```sh mamba env
+create -n torch -f environment.yaml mamba activate torch ``` Install this
+project with ``pip`` in the environment ```sh pip install . ``` The following
+dependencies are required - [numpy](https://numpy.org/) - [opt_einsum](https://
+optimized-einsum.readthedocs.io/en/stable/) - [psutil](https://
+psutil.readthedocs.io/en/latest/) - [pytest](https://docs.pytest.org/) (tests
+only) - [torch](https://pytorch.org/) ## Development For development,
 additionally install the following tools in your environment. ```sh mamba
 install black covdefaults mypy pre-commit pylint pytest pytest-cov pytest-xdist
 tox pip install pytest-random-order ``` With pip, add the option ``-e`` for
 installing in development mode, and add ``[dev]`` for the development
 dependencies ```sh pip install -e .[dev] ``` The pre-commit hooks are
 initialized by running the following command in the root of the repository.
 ```sh pre-commit install ``` For testing all Python environments, simply run
```

### Comparing `tad_mctc-0.1.3/src/tad_mctc.egg-info/SOURCES.txt` & `tad_mctc-0.1.4/src/tad_mctc.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -61,27 +61,31 @@
 src/tad_mctc/io/write/turbomole.py
 src/tad_mctc/io/write/writer.py
 src/tad_mctc/io/write/xyz.py
 src/tad_mctc/math/__init__.py
 src/tad_mctc/math/einsum.py
 src/tad_mctc/molecule/__init__.py
 src/tad_mctc/molecule/bond.py
+src/tad_mctc/molecule/container.py
 src/tad_mctc/molecule/geometry.py
 src/tad_mctc/molecule/property.py
 src/tad_mctc/ncoord/__init__.py
 src/tad_mctc/ncoord/count.py
 src/tad_mctc/ncoord/d3.py
 src/tad_mctc/ncoord/d4.py
 src/tad_mctc/ncoord/defaults.py
 src/tad_mctc/ncoord/eeq.py
 src/tad_mctc/storch/__init__.py
 src/tad_mctc/storch/distance.py
 src/tad_mctc/storch/elemental.py
 src/tad_mctc/storch/linalg.py
 src/tad_mctc/storch/utils.py
+src/tad_mctc/tools/__init__.py
+src/tad_mctc/tools/caching.py
+src/tad_mctc/tools/memory.py
 src/tad_mctc/typing/__init__.py
 src/tad_mctc/typing/builtin.py
 src/tad_mctc/typing/compat.py
 src/tad_mctc/typing/pytorch.py
 src/tad_mctc/units/__init__.py
 src/tad_mctc/units/codata.py
 src/tad_mctc/units/energy.py
```


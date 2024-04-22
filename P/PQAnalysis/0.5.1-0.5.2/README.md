# Comparing `tmp/PQAnalysis-0.5.1.tar.gz` & `tmp/pqanalysis-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PQAnalysis-0.5.1.tar", last modified: Tue Nov 28 07:38:24 2023, max compression
+gzip compressed data, was "pqanalysis-0.5.2.tar", last modified: Mon Apr 22 06:38:42 2024, max compression
```

## Comparing `PQAnalysis-0.5.1.tar` & `pqanalysis-0.5.2.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.332002 PQAnalysis-0.5.1/
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.285212 PQAnalysis-0.5.1/.github/
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.288554 PQAnalysis-0.5.1/.github/workflows/
--rw-r--r--   0 jag       (1000) jag       (1000)      743 2023-10-31 11:11:49.000000 PQAnalysis-0.5.1/.github/workflows/ci.yml
--rw-r--r--   0 jag       (1000) jag       (1000)     1502 2023-10-31 11:11:49.000000 PQAnalysis-0.5.1/.github/workflows/docs.yml
--rw-r--r--   0 jag       (1000) jag       (1000)      116 2023-11-28 07:37:01.000000 PQAnalysis-0.5.1/.gitignore
--rw-r--r--   0 jag       (1000) jag       (1000)     1113 2023-11-09 23:22:54.000000 PQAnalysis-0.5.1/LICENSE
--rw-r--r--   0 jag       (1000) jag       (1000)     2290 2023-11-28 07:38:24.332002 PQAnalysis-0.5.1/PKG-INFO
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.288554 PQAnalysis-0.5.1/PQAnalysis/
--rw-r--r--   0 jag       (1000) jag       (1000)       73 2023-11-09 23:22:54.000000 PQAnalysis-0.5.1/PQAnalysis/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)      411 2023-11-28 07:38:24.000000 PQAnalysis-0.5.1/PQAnalysis/_version.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.291896 PQAnalysis-0.5.1/PQAnalysis/cli/
--rw-r--r--   0 jag       (1000) jag       (1000)       49 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/cli/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)     1590 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/cli/rst2xyz.py
--rw-r--r--   0 jag       (1000) jag       (1000)     2578 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/cli/traj2box.py
--rw-r--r--   0 jag       (1000) jag       (1000)     1692 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/cli/traj2qmcfc.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.291896 PQAnalysis-0.5.1/PQAnalysis/core/
--rw-r--r--   0 jag       (1000) jag       (1000)      333 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/core/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)    12233 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/core/atom.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.295239 PQAnalysis-0.5.1/PQAnalysis/core/atomicSystem/
--rw-r--r--   0 jag       (1000) jag       (1000)       39 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/core/atomicSystem/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)     1411 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/core/atomicSystem/_decorators.py
--rw-r--r--   0 jag       (1000) jag       (1000)     4022 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/core/atomicSystem/_indexing.py
--rw-r--r--   0 jag       (1000) jag       (1000)     4152 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/core/atomicSystem/_positions.py
--rw-r--r--   0 jag       (1000) jag       (1000)     2848 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/core/atomicSystem/_properties.py
--rw-r--r--   0 jag       (1000) jag       (1000)     2395 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/core/atomicSystem/_standardProperties.py
--rw-r--r--   0 jag       (1000) jag       (1000)     6197 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/core/atomicSystem/atomicSystem.py
--rw-r--r--   0 jag       (1000) jag       (1000)     6333 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/core/cell.py
--rw-r--r--   0 jag       (1000) jag       (1000)     1322 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/core/exceptions.py
--rw-r--r--   0 jag       (1000) jag       (1000)      364 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/exceptions.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.298581 PQAnalysis-0.5.1/PQAnalysis/io/
--rw-r--r--   0 jag       (1000) jag       (1000)      709 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/io/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)     3443 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/io/base.py
--rw-r--r--   0 jag       (1000) jag       (1000)     6671 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/io/boxWriter.py
--rw-r--r--   0 jag       (1000) jag       (1000)     4459 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/io/energyFileReader.py
--rw-r--r--   0 jag       (1000) jag       (1000)     2145 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/io/exceptions.py
--rw-r--r--   0 jag       (1000) jag       (1000)     8914 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/io/frameReader.py
--rw-r--r--   0 jag       (1000) jag       (1000)     4615 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/io/infoFileReader.py
--rw-r--r--   0 jag       (1000) jag       (1000)     3660 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/io/moldescriptorReader.py
--rw-r--r--   0 jag       (1000) jag       (1000)     6692 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/io/restartReader.py
--rw-r--r--   0 jag       (1000) jag       (1000)     3606 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/io/restartWriter.py
--rw-r--r--   0 jag       (1000) jag       (1000)     4985 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/io/trajectoryReader.py
--rw-r--r--   0 jag       (1000) jag       (1000)     9028 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/io/trajectoryWriter.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.298581 PQAnalysis-0.5.1/PQAnalysis/physicalData/
--rw-r--r--   0 jag       (1000) jag       (1000)       64 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/physicalData/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)     7918 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/physicalData/energy.py
--rw-r--r--   0 jag       (1000) jag       (1000)      435 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/physicalData/exceptions.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.298581 PQAnalysis-0.5.1/PQAnalysis/tools/
--rw-r--r--   0 jag       (1000) jag       (1000)       47 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/tools/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)     1360 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/tools/traj_to_com_traj.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.298581 PQAnalysis-0.5.1/PQAnalysis/topology/
--rw-r--r--   0 jag       (1000) jag       (1000)       98 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/topology/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)      435 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/topology/exceptions.py
--rw-r--r--   0 jag       (1000) jag       (1000)     6971 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/topology/molType.py
--rw-r--r--   0 jag       (1000) jag       (1000)     6251 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/topology/shakeTopology.py
--rw-r--r--   0 jag       (1000) jag       (1000)      285 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/topology/topology.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.301923 PQAnalysis-0.5.1/PQAnalysis/traj/
--rw-r--r--   0 jag       (1000) jag       (1000)      241 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/traj/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)     1919 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/traj/exceptions.py
--rw-r--r--   0 jag       (1000) jag       (1000)     3025 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/traj/formats.py
--rw-r--r--   0 jag       (1000) jag       (1000)     5860 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/traj/frame.py
--rw-r--r--   0 jag       (1000) jag       (1000)     4114 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/traj/trajectory.py
--rw-r--r--   0 jag       (1000) jag       (1000)     1324 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/types.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.301923 PQAnalysis-0.5.1/PQAnalysis/utils/
--rw-r--r--   0 jag       (1000) jag       (1000)      108 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/PQAnalysis/utils/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)     1313 2023-11-09 23:22:54.000000 PQAnalysis-0.5.1/PQAnalysis/utils/common.py
--rw-r--r--   0 jag       (1000) jag       (1000)     1358 2023-11-09 23:22:54.000000 PQAnalysis-0.5.1/PQAnalysis/utils/decorators.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.332002 PQAnalysis-0.5.1/PQAnalysis.egg-info/
--rw-r--r--   0 jag       (1000) jag       (1000)     2290 2023-11-28 07:38:24.000000 PQAnalysis-0.5.1/PQAnalysis.egg-info/PKG-INFO
--rw-r--r--   0 jag       (1000) jag       (1000)     4115 2023-11-28 07:38:24.000000 PQAnalysis-0.5.1/PQAnalysis.egg-info/SOURCES.txt
--rw-r--r--   0 jag       (1000) jag       (1000)        1 2023-11-28 07:38:24.000000 PQAnalysis-0.5.1/PQAnalysis.egg-info/dependency_links.txt
--rw-r--r--   0 jag       (1000) jag       (1000)      140 2023-11-28 07:38:24.000000 PQAnalysis-0.5.1/PQAnalysis.egg-info/entry_points.txt
--rw-r--r--   0 jag       (1000) jag       (1000)      121 2023-11-28 07:38:24.000000 PQAnalysis-0.5.1/PQAnalysis.egg-info/requires.txt
--rw-r--r--   0 jag       (1000) jag       (1000)       11 2023-11-28 07:38:24.000000 PQAnalysis-0.5.1/PQAnalysis.egg-info/top_level.txt
--rw-r--r--   0 jag       (1000) jag       (1000)     1223 2023-11-11 23:36:52.000000 PQAnalysis-0.5.1/README.md
--rw-r--r--   0 jag       (1000) jag       (1000)       50 2023-10-31 11:11:49.000000 PQAnalysis-0.5.1/codecov.yml
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.301923 PQAnalysis-0.5.1/docs/
--rw-r--r--   0 jag       (1000) jag       (1000)      638 2023-10-24 06:24:16.000000 PQAnalysis-0.5.1/docs/Makefile
--rw-r--r--   0 jag       (1000) jag       (1000)      804 2023-10-24 06:24:16.000000 PQAnalysis-0.5.1/docs/make.bat
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.301923 PQAnalysis-0.5.1/docs/source/
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.301923 PQAnalysis-0.5.1/docs/source/code/
--rw-r--r--   0 jag       (1000) jag       (1000)      510 2023-11-06 09:30:58.000000 PQAnalysis-0.5.1/docs/source/code/PQAnalysis.cli.rst
--rw-r--r--   0 jag       (1000) jag       (1000)      823 2023-11-09 23:22:54.000000 PQAnalysis-0.5.1/docs/source/code/PQAnalysis.core.rst
--rw-r--r--   0 jag       (1000) jag       (1000)     1196 2023-11-09 23:22:54.000000 PQAnalysis-0.5.1/docs/source/code/PQAnalysis.io.rst
--rw-r--r--   0 jag       (1000) jag       (1000)      394 2023-11-09 23:22:54.000000 PQAnalysis-0.5.1/docs/source/code/PQAnalysis.physicalData.rst
--rw-r--r--   0 jag       (1000) jag       (1000)      349 2023-11-09 23:22:54.000000 PQAnalysis-0.5.1/docs/source/code/PQAnalysis.rst
--rw-r--r--   0 jag       (1000) jag       (1000)      388 2023-11-06 09:30:58.000000 PQAnalysis-0.5.1/docs/source/code/PQAnalysis.tools.rst
--rw-r--r--   0 jag       (1000) jag       (1000)      510 2023-11-09 23:22:54.000000 PQAnalysis-0.5.1/docs/source/code/PQAnalysis.traj.rst
--rw-r--r--   0 jag       (1000) jag       (1000)      853 2023-11-09 23:22:54.000000 PQAnalysis-0.5.1/docs/source/code/PQAnalysis.utils.rst
--rw-r--r--   0 jag       (1000) jag       (1000)       67 2023-11-06 09:34:12.000000 PQAnalysis-0.5.1/docs/source/code/modules.rst
--rw-r--r--   0 jag       (1000) jag       (1000)     2418 2023-11-09 23:22:54.000000 PQAnalysis-0.5.1/docs/source/conf.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.301923 PQAnalysis-0.5.1/docs/source/developerGuide/
--rw-r--r--   0 jag       (1000) jag       (1000)     1721 2023-11-11 23:36:52.000000 PQAnalysis-0.5.1/docs/source/developerGuide/developerGuide.rst
--rw-r--r--   0 jag       (1000) jag       (1000)      377 2023-11-09 23:22:54.000000 PQAnalysis-0.5.1/docs/source/index.rst
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.301923 PQAnalysis-0.5.1/docs/source/logo/
--rw-r--r--   0 jag       (1000) jag       (1000)   204575 2023-11-09 23:22:54.000000 PQAnalysis-0.5.1/docs/source/logo/PQAnalysis.png
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.288554 PQAnalysis-0.5.1/examples/
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.305265 PQAnalysis-0.5.1/examples/traj2box/
--rw-r--r--   0 jag       (1000) jag       (1000)       17 2023-10-31 11:11:49.000000 PQAnalysis-0.5.1/examples/traj2box/.gitignore
--rw-r--r--   0 jag       (1000) jag       (1000)  1170470 2023-10-31 11:11:49.000000 PQAnalysis-0.5.1/examples/traj2box/acof_triclinic.xyz
--rw-r--r--   0 jag       (1000) jag       (1000)  1170470 2023-10-31 11:11:49.000000 PQAnalysis-0.5.1/examples/traj2box/acof_triclinic_2.xyz
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.308607 PQAnalysis-0.5.1/examples/traj2comtraj/
--rw-r--r--   0 jag       (1000) jag       (1000)  2600700 2023-10-31 11:11:49.000000 PQAnalysis-0.5.1/examples/traj2comtraj/umcm-9-md-01.xyz
--rw-r--r--   0 jag       (1000) jag       (1000)     1247 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/pyproject.toml
--rw-r--r--   0 jag       (1000) jag       (1000)      131 2023-11-28 07:38:24.332002 PQAnalysis-0.5.1/setup.cfg
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.311949 PQAnalysis-0.5.1/tests/
--rw-r--r--   0 jag       (1000) jag       (1000)        0 2023-11-03 20:48:26.000000 PQAnalysis-0.5.1/tests/__init__.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.311949 PQAnalysis-0.5.1/tests/cli/
--rw-r--r--   0 jag       (1000) jag       (1000)     1136 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/cli/test_rst2xyz.py
--rw-r--r--   0 jag       (1000) jag       (1000)     1458 2023-11-09 23:22:54.000000 PQAnalysis-0.5.1/tests/cli/test_traj2box.py
--rw-r--r--   0 jag       (1000) jag       (1000)      951 2023-11-09 23:22:54.000000 PQAnalysis-0.5.1/tests/cli/test_traj2qmcfc.py
--rw-r--r--   0 jag       (1000) jag       (1000)      646 2023-11-09 23:22:54.000000 PQAnalysis-0.5.1/tests/conftest.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.311949 PQAnalysis-0.5.1/tests/core/
--rw-r--r--   0 jag       (1000) jag       (1000)        0 2023-11-09 23:22:54.000000 PQAnalysis-0.5.1/tests/core/__init__.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.311949 PQAnalysis-0.5.1/tests/core/atomicSystem/
--rw-r--r--   0 jag       (1000) jag       (1000)     5895 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/core/atomicSystem/test_atomicSystem.py
--rw-r--r--   0 jag       (1000) jag       (1000)      687 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/core/atomicSystem/test_indexing.py
--rw-r--r--   0 jag       (1000) jag       (1000)     2486 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/core/atomicSystem/test_positions.py
--rw-r--r--   0 jag       (1000) jag       (1000)     2657 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/core/test_atom.py
--rw-r--r--   0 jag       (1000) jag       (1000)     2889 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/core/test_cell.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.288554 PQAnalysis-0.5.1/tests/data/
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.315291 PQAnalysis-0.5.1/tests/data/readEnergyFile/
--rw-r--r--   0 jag       (1000) jag       (1000)      481 2023-11-09 23:22:54.000000 PQAnalysis-0.5.1/tests/data/readEnergyFile/md-01.en
--rw-r--r--   0 jag       (1000) jag       (1000)      901 2023-11-09 23:22:54.000000 PQAnalysis-0.5.1/tests/data/readEnergyFile/md-01.info
--rw-r--r--   0 jag       (1000) jag       (1000)      468 2023-11-09 23:22:54.000000 PQAnalysis-0.5.1/tests/data/readEnergyFile/md-01_noinfo.en
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.315291 PQAnalysis-0.5.1/tests/data/readInfoFile/
--rw-r--r--   0 jag       (1000) jag       (1000)      901 2023-11-27 09:50:23.000000 PQAnalysis-0.5.1/tests/data/readInfoFile/md-01.info
--rw-r--r--   0 jag       (1000) jag       (1000)      982 2023-11-09 23:22:54.000000 PQAnalysis-0.5.1/tests/data/readInfoFile/md-01.qmcfc.info
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.315291 PQAnalysis-0.5.1/tests/data/readMoldescriptor/
--rw-r--r--   0 jag       (1000) jag       (1000)      424 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/data/readMoldescriptor/moldescriptor.dat
--rw-r--r--   0 jag       (1000) jag       (1000)      418 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/data/readMoldescriptor/moldescriptor_withError.dat
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.315291 PQAnalysis-0.5.1/tests/data/readRestartFile/
--rw-r--r--   0 jag       (1000) jag       (1000)      322 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/data/readRestartFile/md-01.rst
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.315291 PQAnalysis-0.5.1/tests/data/rst2xyz/
--rw-r--r--   0 jag       (1000) jag       (1000)      322 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/data/rst2xyz/md-01.rst
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.318633 PQAnalysis-0.5.1/tests/data/traj2box/
--rw-r--r--   0 jag       (1000) jag       (1000)  1170470 2023-10-31 11:11:49.000000 PQAnalysis-0.5.1/tests/data/traj2box/acof_triclinic.xyz
--rw-r--r--   0 jag       (1000) jag       (1000)  1170470 2023-10-31 11:11:49.000000 PQAnalysis-0.5.1/tests/data/traj2box/acof_triclinic_2.xyz
--rw-r--r--   0 jag       (1000) jag       (1000)     8632 2023-10-31 11:11:49.000000 PQAnalysis-0.5.1/tests/data/traj2box/box.dat
--rw-r--r--   0 jag       (1000) jag       (1000)    88940 2023-10-31 11:11:49.000000 PQAnalysis-0.5.1/tests/data/traj2box/box.vmd.xyz
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.325318 PQAnalysis-0.5.1/tests/data/traj2qmcfc/
--rw-r--r--   0 jag       (1000) jag       (1000)  1170470 2023-10-31 11:11:49.000000 PQAnalysis-0.5.1/tests/data/traj2qmcfc/acof_triclinic.xyz
--rw-r--r--   0 jag       (1000) jag       (1000)  1170470 2023-10-31 11:11:49.000000 PQAnalysis-0.5.1/tests/data/traj2qmcfc/acof_triclinic_2.xyz
--rw-r--r--   0 jag       (1000) jag       (1000)  1575832 2023-10-31 11:11:49.000000 PQAnalysis-0.5.1/tests/data/traj2qmcfc/traj.qmcfc.xyz
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.328660 PQAnalysis-0.5.1/tests/io/
--rw-r--r--   0 jag       (1000) jag       (1000)        0 2023-11-03 20:48:26.000000 PQAnalysis-0.5.1/tests/io/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)     2796 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/io/test_base.py
--rw-r--r--   0 jag       (1000) jag       (1000)     5394 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/io/test_boxWriter.py
--rw-r--r--   0 jag       (1000) jag       (1000)     4943 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/io/test_energyFileReader.py
--rw-r--r--   0 jag       (1000) jag       (1000)     4794 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/io/test_frameReader.py
--rw-r--r--   0 jag       (1000) jag       (1000)     3661 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/io/test_infoFileReader.py
--rw-r--r--   0 jag       (1000) jag       (1000)     3034 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/io/test_moldescriptorReader.py
--rw-r--r--   0 jag       (1000) jag       (1000)     4077 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/io/test_restartReader.py
--rw-r--r--   0 jag       (1000) jag       (1000)     3566 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/io/test_restartWriter.py
--rw-r--r--   0 jag       (1000) jag       (1000)     2869 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/io/test_trajectoryReader.py
--rw-r--r--   0 jag       (1000) jag       (1000)     5870 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/io/test_trajectoryWriter.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.328660 PQAnalysis-0.5.1/tests/physicalData/
--rw-r--r--   0 jag       (1000) jag       (1000)        0 2023-11-09 23:22:54.000000 PQAnalysis-0.5.1/tests/physicalData/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)     1995 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/physicalData/test_energy.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.328660 PQAnalysis-0.5.1/tests/tools/
--rw-r--r--   0 jag       (1000) jag       (1000)        0 2023-11-09 23:22:54.000000 PQAnalysis-0.5.1/tests/tools/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)     2335 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/tools/test_traj_to_com_traj.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.328660 PQAnalysis-0.5.1/tests/topology/
--rw-r--r--   0 jag       (1000) jag       (1000)     2822 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/topology/test_molType.py
--rw-r--r--   0 jag       (1000) jag       (1000)     3607 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/topology/test_shakeTopology.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.332002 PQAnalysis-0.5.1/tests/traj/
--rw-r--r--   0 jag       (1000) jag       (1000)        0 2023-11-03 20:48:26.000000 PQAnalysis-0.5.1/tests/traj/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)     3000 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/traj/test_frame.py
--rw-r--r--   0 jag       (1000) jag       (1000)     3510 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/traj/test_trajectory.py
-drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2023-11-28 07:38:24.332002 PQAnalysis-0.5.1/tests/utils/
--rw-r--r--   0 jag       (1000) jag       (1000)        0 2023-11-03 20:48:26.000000 PQAnalysis-0.5.1/tests/utils/__init__.py
--rw-r--r--   0 jag       (1000) jag       (1000)     1221 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/utils/test_common.py
--rw-r--r--   0 jag       (1000) jag       (1000)     1295 2023-11-28 07:31:36.000000 PQAnalysis-0.5.1/tests/utils/test_decorators.py
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.264764 pqanalysis-0.5.2/
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.231430 pqanalysis-0.5.2/.github/
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.238097 pqanalysis-0.5.2/.github/workflows/
+-rw-r--r--   0 jag       (1000) jag       (1000)      743 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/.github/workflows/ci.yml
+-rw-r--r--   0 jag       (1000) jag       (1000)     1502 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/.github/workflows/docs.yml
+-rw-r--r--   0 jag       (1000) jag       (1000)      116 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/.gitignore
+-rw-r--r--   0 jag       (1000) jag       (1000)     1113 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/LICENSE
+-rw-r--r--   0 jag       (1000) jag       (1000)     2290 2024-04-22 06:38:42.264764 pqanalysis-0.5.2/PKG-INFO
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.238097 pqanalysis-0.5.2/PQAnalysis/
+-rw-r--r--   0 jag       (1000) jag       (1000)       73 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/__init__.py
+-rw-r--r--   0 jag       (1000) jag       (1000)      411 2024-04-22 06:38:42.000000 pqanalysis-0.5.2/PQAnalysis/_version.py
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.238097 pqanalysis-0.5.2/PQAnalysis/cli/
+-rw-r--r--   0 jag       (1000) jag       (1000)       49 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/cli/__init__.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     1590 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/cli/rst2xyz.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     2578 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/cli/traj2box.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     1692 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/cli/traj2qmcfc.py
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.238097 pqanalysis-0.5.2/PQAnalysis/core/
+-rw-r--r--   0 jag       (1000) jag       (1000)      333 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/core/__init__.py
+-rw-r--r--   0 jag       (1000) jag       (1000)    12233 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/core/atom.py
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.238097 pqanalysis-0.5.2/PQAnalysis/core/atomicSystem/
+-rw-r--r--   0 jag       (1000) jag       (1000)       39 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/core/atomicSystem/__init__.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     1411 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/core/atomicSystem/_decorators.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     4022 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/core/atomicSystem/_indexing.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     4152 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/core/atomicSystem/_positions.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     2848 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/core/atomicSystem/_properties.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     2395 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/core/atomicSystem/_standardProperties.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     6197 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/core/atomicSystem/atomicSystem.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     6333 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/core/cell.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     1322 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/core/exceptions.py
+-rw-r--r--   0 jag       (1000) jag       (1000)      364 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/exceptions.py
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.241430 pqanalysis-0.5.2/PQAnalysis/io/
+-rw-r--r--   0 jag       (1000) jag       (1000)      709 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/io/__init__.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     3443 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/io/base.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     6671 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/io/boxWriter.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     4459 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/io/energyFileReader.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     2145 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/io/exceptions.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     8914 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/io/frameReader.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     4615 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/io/infoFileReader.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     3660 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/io/moldescriptorReader.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     6692 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/io/restartReader.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     3606 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/io/restartWriter.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     4985 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/io/trajectoryReader.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     9028 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/io/trajectoryWriter.py
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.241430 pqanalysis-0.5.2/PQAnalysis/physicalData/
+-rw-r--r--   0 jag       (1000) jag       (1000)       64 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/physicalData/__init__.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     7888 2024-04-22 06:35:44.000000 pqanalysis-0.5.2/PQAnalysis/physicalData/energy.py
+-rw-r--r--   0 jag       (1000) jag       (1000)      435 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/physicalData/exceptions.py
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.241430 pqanalysis-0.5.2/PQAnalysis/tools/
+-rw-r--r--   0 jag       (1000) jag       (1000)       47 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/tools/__init__.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     1360 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/tools/traj_to_com_traj.py
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.241430 pqanalysis-0.5.2/PQAnalysis/topology/
+-rw-r--r--   0 jag       (1000) jag       (1000)       98 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/topology/__init__.py
+-rw-r--r--   0 jag       (1000) jag       (1000)      435 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/topology/exceptions.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     6971 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/topology/molType.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     6251 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/topology/shakeTopology.py
+-rw-r--r--   0 jag       (1000) jag       (1000)      285 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/topology/topology.py
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.241430 pqanalysis-0.5.2/PQAnalysis/traj/
+-rw-r--r--   0 jag       (1000) jag       (1000)      241 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/traj/__init__.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     1919 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/traj/exceptions.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     3025 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/traj/formats.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     5860 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/traj/frame.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     4114 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/traj/trajectory.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     1324 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/types.py
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.241430 pqanalysis-0.5.2/PQAnalysis/utils/
+-rw-r--r--   0 jag       (1000) jag       (1000)      108 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/utils/__init__.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     1313 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/utils/common.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     1358 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/PQAnalysis/utils/decorators.py
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.261431 pqanalysis-0.5.2/PQAnalysis.egg-info/
+-rw-r--r--   0 jag       (1000) jag       (1000)     2290 2024-04-22 06:38:42.000000 pqanalysis-0.5.2/PQAnalysis.egg-info/PKG-INFO
+-rw-r--r--   0 jag       (1000) jag       (1000)     4115 2024-04-22 06:38:42.000000 pqanalysis-0.5.2/PQAnalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 jag       (1000) jag       (1000)        1 2024-04-22 06:38:42.000000 pqanalysis-0.5.2/PQAnalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 jag       (1000) jag       (1000)      140 2024-04-22 06:38:42.000000 pqanalysis-0.5.2/PQAnalysis.egg-info/entry_points.txt
+-rw-r--r--   0 jag       (1000) jag       (1000)      121 2024-04-22 06:38:42.000000 pqanalysis-0.5.2/PQAnalysis.egg-info/requires.txt
+-rw-r--r--   0 jag       (1000) jag       (1000)       11 2024-04-22 06:38:42.000000 pqanalysis-0.5.2/PQAnalysis.egg-info/top_level.txt
+-rw-r--r--   0 jag       (1000) jag       (1000)     1223 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/README.md
+-rw-r--r--   0 jag       (1000) jag       (1000)       50 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/codecov.yml
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.241430 pqanalysis-0.5.2/docs/
+-rw-r--r--   0 jag       (1000) jag       (1000)      638 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/docs/Makefile
+-rw-r--r--   0 jag       (1000) jag       (1000)      804 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/docs/make.bat
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.241430 pqanalysis-0.5.2/docs/source/
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.244764 pqanalysis-0.5.2/docs/source/code/
+-rw-r--r--   0 jag       (1000) jag       (1000)      510 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/docs/source/code/PQAnalysis.cli.rst
+-rw-r--r--   0 jag       (1000) jag       (1000)      823 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/docs/source/code/PQAnalysis.core.rst
+-rw-r--r--   0 jag       (1000) jag       (1000)     1196 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/docs/source/code/PQAnalysis.io.rst
+-rw-r--r--   0 jag       (1000) jag       (1000)      394 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/docs/source/code/PQAnalysis.physicalData.rst
+-rw-r--r--   0 jag       (1000) jag       (1000)      349 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/docs/source/code/PQAnalysis.rst
+-rw-r--r--   0 jag       (1000) jag       (1000)      388 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/docs/source/code/PQAnalysis.tools.rst
+-rw-r--r--   0 jag       (1000) jag       (1000)      510 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/docs/source/code/PQAnalysis.traj.rst
+-rw-r--r--   0 jag       (1000) jag       (1000)      853 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/docs/source/code/PQAnalysis.utils.rst
+-rw-r--r--   0 jag       (1000) jag       (1000)       67 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/docs/source/code/modules.rst
+-rw-r--r--   0 jag       (1000) jag       (1000)     2418 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/docs/source/conf.py
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.244764 pqanalysis-0.5.2/docs/source/developerGuide/
+-rw-r--r--   0 jag       (1000) jag       (1000)     1721 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/docs/source/developerGuide/developerGuide.rst
+-rw-r--r--   0 jag       (1000) jag       (1000)      377 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/docs/source/index.rst
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.244764 pqanalysis-0.5.2/docs/source/logo/
+-rw-r--r--   0 jag       (1000) jag       (1000)   204575 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/docs/source/logo/PQAnalysis.png
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.234764 pqanalysis-0.5.2/examples/
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.248097 pqanalysis-0.5.2/examples/traj2box/
+-rw-r--r--   0 jag       (1000) jag       (1000)       17 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/examples/traj2box/.gitignore
+-rw-r--r--   0 jag       (1000) jag       (1000)  1170470 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/examples/traj2box/acof_triclinic.xyz
+-rw-r--r--   0 jag       (1000) jag       (1000)  1170470 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/examples/traj2box/acof_triclinic_2.xyz
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.248097 pqanalysis-0.5.2/examples/traj2comtraj/
+-rw-r--r--   0 jag       (1000) jag       (1000)  2600700 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/examples/traj2comtraj/umcm-9-md-01.xyz
+-rw-r--r--   0 jag       (1000) jag       (1000)     1247 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/pyproject.toml
+-rw-r--r--   0 jag       (1000) jag       (1000)      131 2024-04-22 06:38:42.264764 pqanalysis-0.5.2/setup.cfg
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.251431 pqanalysis-0.5.2/tests/
+-rw-r--r--   0 jag       (1000) jag       (1000)        0 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/__init__.py
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.251431 pqanalysis-0.5.2/tests/cli/
+-rw-r--r--   0 jag       (1000) jag       (1000)     1136 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/cli/test_rst2xyz.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     1458 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/cli/test_traj2box.py
+-rw-r--r--   0 jag       (1000) jag       (1000)      951 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/cli/test_traj2qmcfc.py
+-rw-r--r--   0 jag       (1000) jag       (1000)      646 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/conftest.py
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.251431 pqanalysis-0.5.2/tests/core/
+-rw-r--r--   0 jag       (1000) jag       (1000)        0 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/core/__init__.py
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.254764 pqanalysis-0.5.2/tests/core/atomicSystem/
+-rw-r--r--   0 jag       (1000) jag       (1000)     5895 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/core/atomicSystem/test_atomicSystem.py
+-rw-r--r--   0 jag       (1000) jag       (1000)      687 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/core/atomicSystem/test_indexing.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     2486 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/core/atomicSystem/test_positions.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     2657 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/core/test_atom.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     2889 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/core/test_cell.py
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.234764 pqanalysis-0.5.2/tests/data/
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.254764 pqanalysis-0.5.2/tests/data/readEnergyFile/
+-rw-r--r--   0 jag       (1000) jag       (1000)      481 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/data/readEnergyFile/md-01.en
+-rw-r--r--   0 jag       (1000) jag       (1000)      901 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/data/readEnergyFile/md-01.info
+-rw-r--r--   0 jag       (1000) jag       (1000)      468 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/data/readEnergyFile/md-01_noinfo.en
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.254764 pqanalysis-0.5.2/tests/data/readInfoFile/
+-rw-r--r--   0 jag       (1000) jag       (1000)      901 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/data/readInfoFile/md-01.info
+-rw-r--r--   0 jag       (1000) jag       (1000)      982 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/data/readInfoFile/md-01.qmcfc.info
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.254764 pqanalysis-0.5.2/tests/data/readMoldescriptor/
+-rw-r--r--   0 jag       (1000) jag       (1000)      424 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/data/readMoldescriptor/moldescriptor.dat
+-rw-r--r--   0 jag       (1000) jag       (1000)      418 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/data/readMoldescriptor/moldescriptor_withError.dat
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.254764 pqanalysis-0.5.2/tests/data/readRestartFile/
+-rw-r--r--   0 jag       (1000) jag       (1000)      322 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/data/readRestartFile/md-01.rst
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.254764 pqanalysis-0.5.2/tests/data/rst2xyz/
+-rw-r--r--   0 jag       (1000) jag       (1000)      322 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/data/rst2xyz/md-01.rst
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.258098 pqanalysis-0.5.2/tests/data/traj2box/
+-rw-r--r--   0 jag       (1000) jag       (1000)  1170470 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/data/traj2box/acof_triclinic.xyz
+-rw-r--r--   0 jag       (1000) jag       (1000)  1170470 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/data/traj2box/acof_triclinic_2.xyz
+-rw-r--r--   0 jag       (1000) jag       (1000)     8632 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/data/traj2box/box.dat
+-rw-r--r--   0 jag       (1000) jag       (1000)    88940 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/data/traj2box/box.vmd.xyz
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.258098 pqanalysis-0.5.2/tests/data/traj2qmcfc/
+-rw-r--r--   0 jag       (1000) jag       (1000)  1170470 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/data/traj2qmcfc/acof_triclinic.xyz
+-rw-r--r--   0 jag       (1000) jag       (1000)  1170470 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/data/traj2qmcfc/acof_triclinic_2.xyz
+-rw-r--r--   0 jag       (1000) jag       (1000)  1575832 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/data/traj2qmcfc/traj.qmcfc.xyz
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.261431 pqanalysis-0.5.2/tests/io/
+-rw-r--r--   0 jag       (1000) jag       (1000)        0 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/io/__init__.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     2796 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/io/test_base.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     5394 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/io/test_boxWriter.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     4943 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/io/test_energyFileReader.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     4794 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/io/test_frameReader.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     3661 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/io/test_infoFileReader.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     3034 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/io/test_moldescriptorReader.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     4077 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/io/test_restartReader.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     3566 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/io/test_restartWriter.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     2869 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/io/test_trajectoryReader.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     5870 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/io/test_trajectoryWriter.py
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.261431 pqanalysis-0.5.2/tests/physicalData/
+-rw-r--r--   0 jag       (1000) jag       (1000)        0 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/physicalData/__init__.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     1995 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/physicalData/test_energy.py
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.261431 pqanalysis-0.5.2/tests/tools/
+-rw-r--r--   0 jag       (1000) jag       (1000)        0 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/tools/__init__.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     2335 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/tools/test_traj_to_com_traj.py
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.261431 pqanalysis-0.5.2/tests/topology/
+-rw-r--r--   0 jag       (1000) jag       (1000)     2822 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/topology/test_molType.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     3607 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/topology/test_shakeTopology.py
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.261431 pqanalysis-0.5.2/tests/traj/
+-rw-r--r--   0 jag       (1000) jag       (1000)        0 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/traj/__init__.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     3000 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/traj/test_frame.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     3510 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/traj/test_trajectory.py
+drwxr-xr-x   0 jag       (1000) jag       (1000)        0 2024-04-22 06:38:42.261431 pqanalysis-0.5.2/tests/utils/
+-rw-r--r--   0 jag       (1000) jag       (1000)        0 2024-03-11 07:57:56.000000 pqanalysis-0.5.2/tests/utils/__init__.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     1221 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/utils/test_common.py
+-rw-r--r--   0 jag       (1000) jag       (1000)     1295 2024-04-22 06:35:40.000000 pqanalysis-0.5.2/tests/utils/test_decorators.py
```

### Comparing `PQAnalysis-0.5.1/.github/workflows/ci.yml` & `pqanalysis-0.5.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/.github/workflows/docs.yml` & `pqanalysis-0.5.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/LICENSE` & `pqanalysis-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PKG-INFO` & `pqanalysis-0.5.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PQAnalysis
-Version: 0.5.1
+Version: 0.5.2
 Summary: PQAnalysis is a python package for the analysis of PIMD-QMCF simulations.
 Author-email: Jakob Gamper <97gamjak@gmail.com>, "Josef M. Gallmetzer" <gallmetzer.josef@gmail.com>, "Clarissa A. Seidler" <clarissa.seidler@gmail.com>
 Project-URL: Homepage, https://github.com/MolarVerse/PQAnalysis
 Project-URL: PIMD-QMCF, https://github.com/MolarVerse/pimd_qmcf
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PQAnalysis-0.5.1/PQAnalysis/cli/rst2xyz.py` & `pqanalysis-0.5.2/PQAnalysis/cli/rst2xyz.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/cli/traj2box.py` & `pqanalysis-0.5.2/PQAnalysis/cli/traj2box.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/cli/traj2qmcfc.py` & `pqanalysis-0.5.2/PQAnalysis/cli/traj2qmcfc.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/core/atom.py` & `pqanalysis-0.5.2/PQAnalysis/core/atom.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/core/atomicSystem/_decorators.py` & `pqanalysis-0.5.2/PQAnalysis/core/atomicSystem/_decorators.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/core/atomicSystem/_indexing.py` & `pqanalysis-0.5.2/PQAnalysis/core/atomicSystem/_indexing.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/core/atomicSystem/_positions.py` & `pqanalysis-0.5.2/PQAnalysis/core/atomicSystem/_positions.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/core/atomicSystem/_properties.py` & `pqanalysis-0.5.2/PQAnalysis/core/atomicSystem/_properties.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/core/atomicSystem/_standardProperties.py` & `pqanalysis-0.5.2/PQAnalysis/core/atomicSystem/_standardProperties.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/core/atomicSystem/atomicSystem.py` & `pqanalysis-0.5.2/PQAnalysis/core/atomicSystem/atomicSystem.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/core/cell.py` & `pqanalysis-0.5.2/PQAnalysis/core/cell.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/core/exceptions.py` & `pqanalysis-0.5.2/PQAnalysis/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/io/__init__.py` & `pqanalysis-0.5.2/PQAnalysis/io/__init__.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/io/base.py` & `pqanalysis-0.5.2/PQAnalysis/io/base.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/io/boxWriter.py` & `pqanalysis-0.5.2/PQAnalysis/io/boxWriter.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/io/energyFileReader.py` & `pqanalysis-0.5.2/PQAnalysis/io/energyFileReader.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/io/exceptions.py` & `pqanalysis-0.5.2/PQAnalysis/io/exceptions.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/io/frameReader.py` & `pqanalysis-0.5.2/PQAnalysis/io/frameReader.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/io/infoFileReader.py` & `pqanalysis-0.5.2/PQAnalysis/io/infoFileReader.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/io/moldescriptorReader.py` & `pqanalysis-0.5.2/PQAnalysis/io/moldescriptorReader.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/io/restartReader.py` & `pqanalysis-0.5.2/PQAnalysis/io/restartReader.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/io/restartWriter.py` & `pqanalysis-0.5.2/PQAnalysis/io/restartWriter.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/io/trajectoryReader.py` & `pqanalysis-0.5.2/PQAnalysis/io/trajectoryReader.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/io/trajectoryWriter.py` & `pqanalysis-0.5.2/PQAnalysis/io/trajectoryWriter.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/physicalData/energy.py` & `pqanalysis-0.5.2/PQAnalysis/physicalData/energy.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,19 +151,19 @@
         corresponding data entry (column in energy file). The attribute "simulation_time_unit"
         is the corresponding unit. The attribute "simulation_time_with_unit" is a tuple of
         the corresponding data entry and the corresponding unit.
         """
         for attribute in self.__data_attributes__:
             info_string = attribute
             if info_string in self.info or info_string in self.units:
-                setattr(self.__class__, self.__data_attributes__[attribute],
+                setattr(self, self.__data_attributes__[attribute],
                         self.data[self.info[attribute]])
-                setattr(self.__class__, self.__data_attributes__[attribute] + "_unit",
+                setattr(self, self.__data_attributes__[attribute] + "_unit",
                         self.units[attribute])
-                setattr(self.__class__, self.__data_attributes__[attribute] + "_with_unit", (self.data[self.info[
+                setattr(self, self.__data_attributes__[attribute] + "_with_unit", (self.data[self.info[
                         attribute]], self.units[attribute]))
 
     ################################################
     #                                              #
     # from here all attributes possible are listed #
     #                                              #
     ################################################
```

### Comparing `PQAnalysis-0.5.1/PQAnalysis/tools/traj_to_com_traj.py` & `pqanalysis-0.5.2/PQAnalysis/tools/traj_to_com_traj.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/topology/molType.py` & `pqanalysis-0.5.2/PQAnalysis/topology/molType.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/topology/shakeTopology.py` & `pqanalysis-0.5.2/PQAnalysis/topology/shakeTopology.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/traj/exceptions.py` & `pqanalysis-0.5.2/PQAnalysis/traj/exceptions.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/traj/formats.py` & `pqanalysis-0.5.2/PQAnalysis/traj/formats.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/traj/frame.py` & `pqanalysis-0.5.2/PQAnalysis/traj/frame.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/traj/trajectory.py` & `pqanalysis-0.5.2/PQAnalysis/traj/trajectory.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/types.py` & `pqanalysis-0.5.2/PQAnalysis/types.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/utils/common.py` & `pqanalysis-0.5.2/PQAnalysis/utils/common.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis/utils/decorators.py` & `pqanalysis-0.5.2/PQAnalysis/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/PQAnalysis.egg-info/PKG-INFO` & `pqanalysis-0.5.2/PQAnalysis.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PQAnalysis
-Version: 0.5.1
+Version: 0.5.2
 Summary: PQAnalysis is a python package for the analysis of PIMD-QMCF simulations.
 Author-email: Jakob Gamper <97gamjak@gmail.com>, "Josef M. Gallmetzer" <gallmetzer.josef@gmail.com>, "Clarissa A. Seidler" <clarissa.seidler@gmail.com>
 Project-URL: Homepage, https://github.com/MolarVerse/PQAnalysis
 Project-URL: PIMD-QMCF, https://github.com/MolarVerse/pimd_qmcf
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PQAnalysis-0.5.1/PQAnalysis.egg-info/SOURCES.txt` & `pqanalysis-0.5.2/PQAnalysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/README.md` & `pqanalysis-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/docs/Makefile` & `pqanalysis-0.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/docs/make.bat` & `pqanalysis-0.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/docs/source/code/PQAnalysis.core.rst` & `pqanalysis-0.5.2/docs/source/code/PQAnalysis.core.rst`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/docs/source/code/PQAnalysis.io.rst` & `pqanalysis-0.5.2/docs/source/code/PQAnalysis.io.rst`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/docs/source/code/PQAnalysis.utils.rst` & `pqanalysis-0.5.2/docs/source/code/PQAnalysis.utils.rst`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/docs/source/conf.py` & `pqanalysis-0.5.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/docs/source/developerGuide/developerGuide.rst` & `pqanalysis-0.5.2/docs/source/developerGuide/developerGuide.rst`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/docs/source/logo/PQAnalysis.png` & `pqanalysis-0.5.2/docs/source/logo/PQAnalysis.png`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/examples/traj2box/acof_triclinic.xyz` & `pqanalysis-0.5.2/examples/traj2box/acof_triclinic.xyz`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/examples/traj2box/acof_triclinic_2.xyz` & `pqanalysis-0.5.2/examples/traj2box/acof_triclinic_2.xyz`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/examples/traj2comtraj/umcm-9-md-01.xyz` & `pqanalysis-0.5.2/examples/traj2comtraj/umcm-9-md-01.xyz`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/pyproject.toml` & `pqanalysis-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/cli/test_rst2xyz.py` & `pqanalysis-0.5.2/tests/cli/test_rst2xyz.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/cli/test_traj2box.py` & `pqanalysis-0.5.2/tests/cli/test_traj2box.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/cli/test_traj2qmcfc.py` & `pqanalysis-0.5.2/tests/cli/test_traj2qmcfc.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/conftest.py` & `pqanalysis-0.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/core/atomicSystem/test_atomicSystem.py` & `pqanalysis-0.5.2/tests/core/atomicSystem/test_atomicSystem.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/core/atomicSystem/test_indexing.py` & `pqanalysis-0.5.2/tests/core/atomicSystem/test_indexing.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/core/atomicSystem/test_positions.py` & `pqanalysis-0.5.2/tests/core/atomicSystem/test_positions.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/core/test_atom.py` & `pqanalysis-0.5.2/tests/core/test_atom.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/core/test_cell.py` & `pqanalysis-0.5.2/tests/core/test_cell.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/data/readEnergyFile/md-01.info` & `pqanalysis-0.5.2/tests/data/readEnergyFile/md-01.info`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/data/readInfoFile/md-01.info` & `pqanalysis-0.5.2/tests/data/readInfoFile/md-01.info`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/data/readInfoFile/md-01.qmcfc.info` & `pqanalysis-0.5.2/tests/data/readInfoFile/md-01.qmcfc.info`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/data/traj2box/acof_triclinic.xyz` & `pqanalysis-0.5.2/tests/data/traj2box/acof_triclinic.xyz`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/data/traj2box/acof_triclinic_2.xyz` & `pqanalysis-0.5.2/tests/data/traj2box/acof_triclinic_2.xyz`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/data/traj2box/box.dat` & `pqanalysis-0.5.2/tests/data/traj2box/box.dat`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/data/traj2box/box.vmd.xyz` & `pqanalysis-0.5.2/tests/data/traj2box/box.vmd.xyz`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/data/traj2qmcfc/acof_triclinic.xyz` & `pqanalysis-0.5.2/tests/data/traj2qmcfc/acof_triclinic.xyz`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/data/traj2qmcfc/acof_triclinic_2.xyz` & `pqanalysis-0.5.2/tests/data/traj2qmcfc/acof_triclinic_2.xyz`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/data/traj2qmcfc/traj.qmcfc.xyz` & `pqanalysis-0.5.2/tests/data/traj2qmcfc/traj.qmcfc.xyz`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/io/test_base.py` & `pqanalysis-0.5.2/tests/io/test_base.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/io/test_boxWriter.py` & `pqanalysis-0.5.2/tests/io/test_boxWriter.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/io/test_energyFileReader.py` & `pqanalysis-0.5.2/tests/io/test_energyFileReader.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/io/test_frameReader.py` & `pqanalysis-0.5.2/tests/io/test_frameReader.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/io/test_infoFileReader.py` & `pqanalysis-0.5.2/tests/io/test_infoFileReader.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/io/test_moldescriptorReader.py` & `pqanalysis-0.5.2/tests/io/test_moldescriptorReader.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/io/test_restartReader.py` & `pqanalysis-0.5.2/tests/io/test_restartReader.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/io/test_restartWriter.py` & `pqanalysis-0.5.2/tests/io/test_restartWriter.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/io/test_trajectoryReader.py` & `pqanalysis-0.5.2/tests/io/test_trajectoryReader.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/io/test_trajectoryWriter.py` & `pqanalysis-0.5.2/tests/io/test_trajectoryWriter.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/physicalData/test_energy.py` & `pqanalysis-0.5.2/tests/physicalData/test_energy.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/tools/test_traj_to_com_traj.py` & `pqanalysis-0.5.2/tests/tools/test_traj_to_com_traj.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/topology/test_molType.py` & `pqanalysis-0.5.2/tests/topology/test_molType.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/topology/test_shakeTopology.py` & `pqanalysis-0.5.2/tests/topology/test_shakeTopology.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/traj/test_frame.py` & `pqanalysis-0.5.2/tests/traj/test_frame.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/traj/test_trajectory.py` & `pqanalysis-0.5.2/tests/traj/test_trajectory.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/utils/test_common.py` & `pqanalysis-0.5.2/tests/utils/test_common.py`

 * *Files identical despite different names*

### Comparing `PQAnalysis-0.5.1/tests/utils/test_decorators.py` & `pqanalysis-0.5.2/tests/utils/test_decorators.py`

 * *Files identical despite different names*


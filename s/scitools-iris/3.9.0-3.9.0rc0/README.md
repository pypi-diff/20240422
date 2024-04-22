# Comparing `tmp/scitools_iris-3.9.0.tar.gz` & `tmp/scitools-iris-3.9.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scitools_iris-3.9.0.tar", last modified: Mon Apr 22 09:26:07 2024, max compression
+gzip compressed data, was "scitools-iris-3.9.0rc0.tar", last modified: Wed Apr  3 11:05:16 2024, max compression
```

## Comparing `scitools_iris-3.9.0.tar` & `scitools-iris-3.9.0rc0.tar`

### file list

```diff
@@ -1,1814 +1,1814 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.637355 scitools_iris-3.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-04-22 09:26:07.637355 scitools_iris-3.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7430 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.389357 scitools_iris-3.9.0/etc/
--rw-r--r--   0 runner    (1001) docker     (127)  4218305 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/etc/cf-standard-name-table.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.389357 scitools_iris-3.9.0/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.401357 scitools_iris-3.9.0/lib/iris/
--rw-r--r--   0 runner    (1001) docker     (127)    16644 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51364 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/_concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)    24094 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)    17873 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/_lazy_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    63568 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/_merge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.401357 scitools_iris-3.9.0/lib/iris/_representation/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/_representation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12873 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/_representation/cube_printout.py
--rw-r--r--   0 runner    (1001) docker     (127)    15000 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/_representation/cube_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/_shapefiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-22 09:26:06.000000 scitools_iris-3.9.0/lib/iris/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.401357 scitools_iris-3.9.0/lib/iris/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)   113060 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23979 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/analysis/_area_weighted.py
--rw-r--r--   0 runner    (1001) docker     (127)    17857 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/analysis/_grid_angles.py
--rw-r--r--   0 runner    (1001) docker     (127)    25983 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/analysis/_interpolation.py
--rw-r--r--   0 runner    (1001) docker     (127)    41706 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/analysis/_regrid.py
--rw-r--r--   0 runner    (1001) docker     (127)    12533 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/analysis/_scipy_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (127)    28843 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/analysis/calculus.py
--rw-r--r--   0 runner    (1001) docker     (127)    46034 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/analysis/cartography.py
--rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/analysis/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)    37273 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/analysis/maths.py
--rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/analysis/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    36860 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/analysis/trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)    70141 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/aux_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.401357 scitools_iris-3.9.0/lib/iris/common/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/common/_split_attribute_dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)    21880 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/common/lenient.py
--rw-r--r--   0 runner    (1001) docker     (127)    55838 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/common/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/common/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)   108504 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/common/resolve.py
--rw-r--r--   0 runner    (1001) docker     (127)     9498 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14877 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/coord_categorisation.py
--rw-r--r--   0 runner    (1001) docker     (127)    58258 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/coord_systems.py
--rw-r--r--   0 runner    (1001) docker     (127)   113785 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/coords.py
--rw-r--r--   0 runner    (1001) docker     (127)   190896 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/cube.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.405357 scitools_iris-3.9.0/lib/iris/etc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.365357 scitools_iris-3.9.0/lib/iris/etc/palette/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.405357 scitools_iris-3.9.0/lib/iris/etc/palette/diverging/
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/diverging/BrBG_11.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/diverging/PRGn_11.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/diverging/PiYG_11.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/diverging/PuOr_11.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/diverging/RdBu_11.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/diverging/RdGy_11.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/diverging/RdYlBu_11.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/diverging/RdYlGn_11.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/diverging/Spectral_11.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.405357 scitools_iris-3.9.0/lib/iris/etc/palette/qualitative/
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/qualitative/Accent_08.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/qualitative/Dark2_08.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/qualitative/Paired_12.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/qualitative/Pastel1_09.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/qualitative/Pastel2_08.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/qualitative/Set1_09.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/qualitative/Set2_08.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/qualitative/Set3_12.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.409357 scitools_iris-3.9.0/lib/iris/etc/palette/sequential/
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/sequential/Blues_09.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/sequential/BuGn_09.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/sequential/BuPu_09.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/sequential/GnBu_09.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/sequential/Greens_09.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/sequential/Greys_09.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/sequential/OrRd_09.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/sequential/Oranges_09.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/sequential/PuBuGn_09.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/sequential/PuBu_09.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/sequential/PuRd_09.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/sequential/Purples_09.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/sequential/RdPu_09.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/sequential/Reds_09.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/sequential/YlGnBu_09.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/sequential/YlGn_09.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/sequential/YlOrBr_09.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/palette/sequential/YlOrRd_09.txt
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/etc/site.cfg.template
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.409357 scitools_iris-3.9.0/lib/iris/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/experimental/animate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11702 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/experimental/geovista.py
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/experimental/raster.py
--rw-r--r--   0 runner    (1001) docker     (127)    28058 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/experimental/regrid.py
--rw-r--r--   0 runner    (1001) docker     (127)    12735 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/experimental/regrid_conservative.py
--rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/experimental/representation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/experimental/stratify.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.409357 scitools_iris-3.9.0/lib/iris/experimental/ugrid/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/experimental/ugrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11957 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/experimental/ugrid/cf.py
--rw-r--r--   0 runner    (1001) docker     (127)    17472 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/experimental/ugrid/load.py
--rw-r--r--   0 runner    (1001) docker     (127)   113120 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/experimental/ugrid/mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/experimental/ugrid/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/experimental/ugrid/save.py
--rw-r--r--   0 runner    (1001) docker     (127)    13262 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/experimental/ugrid/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.413357 scitools_iris-3.9.0/lib/iris/fileformats/
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32983 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/_ff.py
--rw-r--r--   0 runner    (1001) docker     (127)   196071 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/_ff_cross_references.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.413357 scitools_iris-3.9.0/lib/iris/fileformats/_nc_load_rules/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/_nc_load_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22814 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/_nc_load_rules/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/_nc_load_rules/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    58767 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/_nc_load_rules/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/_pp_lbproc_pairs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19004 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/_structured_array_identification.py
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/abf.py
--rw-r--r--   0 runner    (1001) docker     (127)    49681 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/cf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/name.py
--rw-r--r--   0 runner    (1001) docker     (127)    44568 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/name_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.417357 scitools_iris-3.9.0/lib/iris/fileformats/netcdf/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/netcdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/netcdf/_dask_locks.py
--rw-r--r--   0 runner    (1001) docker     (127)    15709 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/netcdf/_thread_safe_nc.py
--rw-r--r--   0 runner    (1001) docker     (127)    32965 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/netcdf/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)   117932 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/netcdf/saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     9595 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/nimrod.py
--rw-r--r--   0 runner    (1001) docker     (127)    31785 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/nimrod_load_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    81696 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/pp.py
--rw-r--r--   0 runner    (1001) docker     (127)    46857 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/pp_load_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    31086 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/pp_save_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    15712 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.417357 scitools_iris-3.9.0/lib/iris/fileformats/um/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/um/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20658 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/um/_fast_load.py
--rw-r--r--   0 runner    (1001) docker     (127)    12017 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/um/_fast_load_structured_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/um/_ff_replacement.py
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/um/_optimal_array_structuring.py
--rw-r--r--   0 runner    (1001) docker     (127)   107311 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/fileformats/um_cf_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.417357 scitools_iris-3.9.0/lib/iris/io/
--rw-r--r--   0 runner    (1001) docker     (127)    17511 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/io/format_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)    12641 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/iterate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10862 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/palette.py
--rw-r--r--   0 runner    (1001) docker     (127)    35733 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)    71546 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.417357 scitools_iris-3.9.0/lib/iris/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/plugins/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    11201 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/quickplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/symbols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.425357 scitools_iris-3.9.0/lib/iris/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    39521 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.425357 scitools_iris-3.9.0/lib/iris/tests/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.425357 scitools_iris-3.9.0/lib/iris/tests/experimental/regrid/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/experimental/regrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25939 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/experimental/regrid/test_regrid_area_weighted_rectilinear_src_and_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    30060 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/experimental/regrid/test_regrid_conservative_via_esmpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/experimental/test_raster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.425357 scitools_iris-3.9.0/lib/iris/tests/graphics/
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/graphics/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/graphics/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6681 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/graphics/idiff.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2377 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/graphics/recreate_imagerepo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.429357 scitools_iris-3.9.0/lib/iris/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.429357 scitools_iris-3.9.0/lib/iris/tests/integration/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/analysis/test_area_weighted.py
--rw-r--r--   0 runner    (1001) docker     (127)    14908 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/attrs_matrix_results_load.json
--rw-r--r--   0 runner    (1001) docker     (127)    14164 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/attrs_matrix_results_roundtrip.json
--rw-r--r--   0 runner    (1001) docker     (127)    14164 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/attrs_matrix_results_save.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.429357 scitools_iris-3.9.0/lib/iris/tests/integration/aux_factory/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/aux_factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/aux_factory/test_OceanSigmaZFactory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.429357 scitools_iris-3.9.0/lib/iris/tests/integration/concatenate/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/concatenate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16978 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/concatenate/test_concatenate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.429357 scitools_iris-3.9.0/lib/iris/tests/integration/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.429357 scitools_iris-3.9.0/lib/iris/tests/integration/experimental/geovista/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/experimental/geovista/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/experimental/geovista/test_cube_to_poly.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/experimental/geovista/test_extract_unstructured_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/experimental/test_CubeRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/experimental/test_regrid_ProjectedUnstructured.py
--rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/experimental/test_ugrid_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/experimental/test_ugrid_save.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.433357 scitools_iris-3.9.0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex1_1d_mesh.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex2_2d_triangular.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex3_2d_flexible.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex4_3d_layered.cdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.433357 scitools_iris-3.9.0/lib/iris/tests/integration/fast_load/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/fast_load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27776 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/fast_load/test_fast_load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.433357 scitools_iris-3.9.0/lib/iris/tests/integration/merge/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/merge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/merge/test_merge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.433357 scitools_iris-3.9.0/lib/iris/tests/integration/netcdf/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/netcdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/netcdf/test__dask_locks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/netcdf/test_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/netcdf/test_aux_factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/netcdf/test_coord_systems.py
--rw-r--r--   0 runner    (1001) docker     (127)    10955 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/netcdf/test_delayed_save.py
--rw-r--r--   0 runner    (1001) docker     (127)    19738 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/netcdf/test_general.py
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/netcdf/test_self_referencing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/netcdf/test_thread_safety.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.433357 scitools_iris-3.9.0/lib/iris/tests/integration/plot/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/plot/test_animate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/plot/test_colorbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/plot/test_netcdftime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/plot/test_nzdateline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/plot/test_plot_2d_coords.py
--rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/plot/test_vector_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/test_Datums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/test_PartialDateTime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/test_climatology.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/test_cube.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/test_ff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/test_mask_cube_from_shapefile.py
--rw-r--r--   0 runner    (1001) docker     (127)    68487 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/test_netcdf__loadsaveattrs.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/test_new_axis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)    29154 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/test_pp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/test_pp_constrained_load_cubes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/test_regrid_equivalence.py
--rw-r--r--   0 runner    (1001) docker     (127)     9021 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/test_regridding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/test_subset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/test_trajectory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.433357 scitools_iris-3.9.0/lib/iris/tests/integration/um/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/um/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/integration/um/test_fieldsfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.437357 scitools_iris-3.9.0/lib/iris/tests/results/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.437357 scitools_iris-3.9.0/lib/iris/tests/results/COLPEX/
--rw-r--r--   0 runner    (1001) docker     (127)    37400 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/COLPEX/small_colpex_theta_p_alt.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.437357 scitools_iris-3.9.0/lib/iris/tests/results/FF/
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/FF/air_temperature_1.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/FF/air_temperature_2.cml
--rw-r--r--   0 runner    (1001) docker     (127)    11329 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/FF/ffheader.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/FF/soil_temperature_1.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/FF/surface_altitude_1.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.437357 scitools_iris-3.9.0/lib/iris/tests/results/PP/
--rw-r--r--   0 runner    (1001) docker     (127)    14102 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/PP/extra_char_data.pp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14102 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/PP/extra_char_data.w_data_loaded.pp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15286 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/PP/extra_data_time_series.pp.txt
--rw-r--r--   0 runner    (1001) docker     (127)   330620 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/PP/extra_x_data.pp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/PP/global_test.pp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/PP/nae_unpacked.pp.txt
--rw-r--r--   0 runner    (1001) docker     (127)    30791 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/PP/rle_unpacked.pp.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.437357 scitools_iris-3.9.0/lib/iris/tests/results/abf/
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/abf/load.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.461356 scitools_iris-3.9.0/lib/iris/tests/results/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/abs.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/addition.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/addition_coord_x.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/addition_coord_y.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/addition_different_std_name.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/addition_in_place.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/addition_in_place_coord.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/addition_scalar.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.461356 scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/easy.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/multi.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/multi_missing.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/multi_shared.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/single.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/single_missing.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/single_rms.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/single_shared.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/single_shared_circular.cml
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/weighted_easy.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/weighted_multi.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/weighted_multi_missing.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/weighted_multi_shared.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/weighted_single.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/weighted_single_missing.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/weighted_single_shared.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/weighted_single_shared_circular.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/apply_ifunc.cml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/apply_ifunc.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/apply_ifunc_frompyfunc.cml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/apply_ifunc_frompyfunc.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/apply_ifunc_original.cml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/apply_ifunc_original.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/apply_ufunc.cml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/apply_ufunc.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/apply_ufunc_frompyfunc.cml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/apply_ufunc_frompyfunc.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/apply_ufunc_original.cml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/apply_ufunc_original.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/areaweights_original.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.465356 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/cos_simple.xml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/cos_simple_radians.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/curl_contrived_cartesian2.cml
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/delta_handmade_simple_wrt_x.cml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/delta_handmade_simple_wrt_x.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_lat.cml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_lat.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_lon.cml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_lon.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_x.cml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_x.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_y.cml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_y.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/grad_contrived1.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/grad_contrived2.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/grad_contrived_non_spherical1.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/handmade2_wrt_lat.cml
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/handmade2_wrt_lat.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/handmade2_wrt_lon.cml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/handmade2_wrt_lon.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/handmade_simple_wrt_x.cml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/handmade_simple_wrt_x.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/handmade_wrt_lat.cml
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/handmade_wrt_lat.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/handmade_wrt_lon.cml
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/handmade_wrt_lon.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/handmade_wrt_x.cml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/handmade_wrt_x.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/handmade_wrt_y.cml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/handmade_wrt_y.data.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.469356 scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube1_cube1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube2_cube1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube3.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube4.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube5.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/cube2_cube3.txt
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/cube2_cube4.txt
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/cube2_cube5.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/cube3_cube4.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/cube3_cube5.txt
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/cube4_cube5.txt
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/count_bar_2d.cml
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/count_foo_1d.cml
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/count_foo_2d.cml
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/count_foo_bar_2d.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.473356 scitools_iris-3.9.0/lib/iris/tests/results/analysis/delta_and_midpoint/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/delta_and_midpoint/delta_one_element_explicit.xml
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/delta_and_midpoint/midpoint_one_element_explicit.xml
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/delta_and_midpoint/simple1.cml
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/delta_and_midpoint/simple1_delta.cml
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/delta_and_midpoint/simple1_midpoint.cml
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/delta_and_midpoint/simple2.cml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/delta_and_midpoint/simple2_delta.cml
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/delta_and_midpoint/simple2_midpoint.cml
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/delta_and_midpoint/simple3.cml
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/delta_and_midpoint/simple3_delta.cml
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/delta_and_midpoint/simple3_midpoint.cml
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/delta_and_midpoint/simple4.cml
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/delta_and_midpoint/simple4_delta.cml
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/delta_and_midpoint/simple4_midpoint.cml
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/delta_and_midpoint/simple5.cml
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/delta_and_midpoint/simple5_delta.cml
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/delta_and_midpoint/simple5_midpoint.cml
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/delta_and_midpoint/simple6.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/division.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/division_by_array.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/division_by_latitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/division_by_longitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/division_by_singular_coord.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/division_scalar.cml
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/exp.cml
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/exp.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/exponentiate.cml
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/exponentiate.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/first_quartile_foo_1d.cml
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/first_quartile_foo_1d_fast_percentile.cml
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/first_quartile_foo_2d.cml
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/first_quartile_foo_2d_fast_percentile.cml
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/first_quartile_foo_bar_2d.cml
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/first_quartile_foo_bar_2d_fast_percentile.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/gmean_latitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/gmean_latitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/gmean_latitude_longitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/gmean_latitude_longitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/gmean_latitude_longitude_1call.cml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/gmean_latitude_longitude_1call.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/hmean_latitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/hmean_latitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/hmean_latitude_longitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/hmean_latitude_longitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/hmean_latitude_longitude_1call.cml
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/hmean_latitude_longitude_1call.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/last_quartile_foo_3d_masked.cml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/last_quartile_foo_3d_notmasked.cml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/last_quartile_foo_3d_notmasked_fast_percentile.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/log.cml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/log.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/log10.cml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/log10.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/log2.cml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/log2.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/maths_original.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/max_latitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/max_latitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/max_latitude_longitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/max_latitude_longitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/max_latitude_longitude_1call.cml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/max_latitude_longitude_1call.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/max_run_bar_2d.cml
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/max_run_bar_2d_masked.cml
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/max_run_foo_1d.cml
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/max_run_foo_2d.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/mean_latitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/mean_latitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/mean_latitude_longitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/mean_latitude_longitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/mean_latitude_longitude_1call.cml
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/mean_latitude_longitude_1call.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/median_latitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/median_latitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/median_latitude_longitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/median_latitude_longitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/median_latitude_longitude_1call.cml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/median_latitude_longitude_1call.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/min_latitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/min_latitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/min_latitude_longitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/min_latitude_longitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/min_latitude_longitude_1call.cml
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/min_latitude_longitude_1call.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/multiply.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/multiply_different_std_name.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/original.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/original_common.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/original_hmean.cml
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/proportion_bar_2d.cml
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/proportion_foo_1d.cml
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/proportion_foo_2d.cml
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/proportion_foo_2d_masked.cml
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/proportion_foo_bar_2d.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.481356 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_both_circular.cml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_both_circular.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_circular_grid.cml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_circular_grid.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_circular_src.cml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_circular_src.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_circular_srcmissingmask.cml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_circular_srcmissingmask.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_masked_altitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_masked_altitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_non_circular.cml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_non_circular.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_partial_overlap.cml
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_partial_overlap.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_subset.cml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_subset.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_subset_anon.cml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_subset_anon.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_subset_masked_1.cml
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_subset_masked_1.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_subset_masked_2.cml
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_subset_masked_2.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_both_circular.cml
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_both_circular.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_circular_grid.cml
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_circular_grid.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_circular_src.cml
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_circular_src.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_circular_srcmissingmask.cml
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_circular_srcmissingmask.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_masked_altitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_masked_altitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_non_circular.cml
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_non_circular.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_partial_overlap.cml
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_partial_overlap.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_subset.cml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_subset.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_subset_anon.cml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_subset_anon.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_subset_masked_1.cml
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_subset_masked_1.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_subset_masked_2.cml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_subset_masked_2.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/no_overlap.cml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/no_overlap.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/rms_latitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/rms_latitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/rms_latitude_longitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/rms_latitude_longitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/rms_latitude_longitude_1call.cml
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/rms_latitude_longitude_1call.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/rms_weighted_2d.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.481356 scitools_iris-3.9.0/lib/iris/tests/results/analysis/rolling_window/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/rolling_window/simple_latitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/rolling_window/simple_longitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/rolling_window/size_4_longitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/rotated_pole.0.rlat.json
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/rotated_pole.0.rlon.json
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/rotated_pole.0.x.json
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/rotated_pole.0.y.json
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/rotated_pole.1.rlat.json
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/rotated_pole.1.rlon.json
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/rotated_pole.1.x.json
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/rotated_pole.1.y.json
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/sqrt.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/std_dev_latitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/std_dev_latitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/std_dev_latitude_longitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/std_dev_latitude_longitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/std_dev_latitude_longitude_1call.cml
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/std_dev_latitude_longitude_1call.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/subtract.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/subtract_array.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/subtract_coord_x.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/subtract_coord_y.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/subtract_scalar.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/sum_latitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/sum_latitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/sum_latitude_longitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/sum_latitude_longitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/sum_latitude_longitude_1call.cml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/sum_latitude_longitude_1call.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/sum_weighted_1d.cml
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/sum_weighted_2d.cml
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/third_quartile_foo_1d.cml
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/third_quartile_foo_1d_fast_percentile.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/variance_latitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/variance_latitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/variance_latitude_longitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/variance_latitude_longitude.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/variance_latitude_longitude_1call.cml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/variance_latitude_longitude_1call.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/weighted_mean_lat.cml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/weighted_mean_lat.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/weighted_mean_latlon.cml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/weighted_mean_latlon.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/weighted_mean_lon.cml
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/weighted_mean_lon.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/weighted_mean_original.cml
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/analysis/weighted_mean_source.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.369357 scitools_iris-3.9.0/lib/iris/tests/results/cartography/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.481356 scitools_iris-3.9.0/lib/iris/tests/results/cartography/get_xy_grids/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cartography/get_xy_grids/1d.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cartography/get_xy_grids/2d.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.481356 scitools_iris-3.9.0/lib/iris/tests/results/categorisation/
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/categorisation/customcheck.cml
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/categorisation/quickcheck.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.481356 scitools_iris-3.9.0/lib/iris/tests/results/cdm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.485356 scitools_iris-3.9.0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/0d_repr.txt
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/0d_str.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/1d_repr.txt
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/1d_str.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/2d_repr.txt
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/2d_str.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/3d_repr.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/3d_str.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/4d_repr.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/4d_str.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.485356 scitools_iris-3.9.0/lib/iris/tests/results/cdm/extract/
--rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/extract/lat_eq_10.cml
--rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/extract/lat_gt_10.cml
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/extract/lat_gt_10_and_lon_ge_10.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/masked_cube.cml
--rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/masked_save_pp.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.485356 scitools_iris-3.9.0/lib/iris/tests/results/cdm/str_repr/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/str_repr/0d_cube.__repr__.txt
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/str_repr/0d_cube.__str__.txt
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/str_repr/0d_cube.__unicode__.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/str_repr/cell_methods.__str__.txt
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/str_repr/cubelist.__repr__.txt
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/str_repr/cubelist.__str__.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/str_repr/missing_coords_cube.repr.txt
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/str_repr/missing_coords_cube.str.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/str_repr/multi_dim_coord.__repr__.txt
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/str_repr/multi_dim_coord.__str__.txt
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/str_repr/similar.__str__.txt
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/str_repr/simple.__str__.txt
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/str_repr/unicode_attribute.__unicode__.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cdm/test_simple_cube_intersection.cml
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/compatible_cubes.str.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.493356 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2x2d.cml
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x.cml
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_bounds.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_xy.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_y.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_y_xy.cml
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2x2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2x2d_aux_xy_bounds.cml
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2x2d_aux_y.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2x2d_aux_y_xy.cml
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2y2d.cml
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2y2d_aux_x.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2y2d_aux_x_xy.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2y2d_aux_x_y.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2y2d_aux_x_y_xy.cml
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2y2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2y2d_aux_y.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2y2d_aux_y_xy.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_3d_simple.cml
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_4mix2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_4x2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_4y2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_9mix2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_9x2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_9y2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_anonymous.cml
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_masked_2x2d.cml
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_masked_2y2d.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_merged_scalar_4mix2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_merged_scalar_4x2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_merged_scalar_4y2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_pre_merged_scalar_4mix2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_pre_merged_scalar_4x2_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_pre_merged_scalar_4y2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_scalar_4mix2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_scalar_4x2d_aux_xy.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_scalar_4y2d_aux_xy.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.497356 scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/
--rw-r--r--   0 runner    (1001) docker     (127)    10348 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/all_10_load_match.cml
--rw-r--r--   0 runner    (1001) docker     (127)    10878 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/all_ml_10_22_load_match.cml
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/attribute_constraint.cml
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/invalid_inequality_load_match.cml
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/pressure_950_load_match.cml
--rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_10_and_theta_level_gt_30_le_3_load_match.cml
--rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_10_and_theta_level_gt_30_le_3_load_strict.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_10_load_match.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_10_load_strict.cml
--rw-r--r--   0 runner    (1001) docker     (127)    16305 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_and_all_10_load_match.cml
--rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_and_theta_10_load_strict.cml
--rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_and_theta_load_match.cml
--rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_and_theta_load_strict.cml
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_gt_30_le_3_load_match.cml
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_gt_30_le_3_load_strict.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_lat_30_load_match.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_lat_30_load_strict.cml
--rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_lat_gt_30_load_match.cml
--rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_lat_gt_30_load_strict.cml
--rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_load_match.cml
--rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_load_strict.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.497356 scitools_iris-3.9.0/lib/iris/tests/results/coord_api/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_api/complex.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.497356 scitools_iris-3.9.0/lib/iris/tests/results/coord_api/coord_maths/
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_api/coord_maths/add_float_expl.xml
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_api/coord_maths/add_simple_expl.xml
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_api/coord_maths/divide_simple_expl.xml
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_api/coord_maths/mult_float_expl.xml
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_api/coord_maths/multiply_simple_expl.xml
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_api/coord_maths/negate_expl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_api/coord_maths/r_subtract_simple_exl.xml
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_api/coord_maths/right_divide_simple_expl.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_api/coord_maths/subtract_simple_expl.xml
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_api/intersection.xml
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_api/intersection_missing.xml
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_api/intersection_reversed.xml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_api/minimal.xml
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_api/nd_bounds.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.497356 scitools_iris-3.9.0/lib/iris/tests/results/coord_api/str_repr/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_api/str_repr/aux_nontime_repr.txt
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_api/str_repr/aux_nontime_str.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_api/str_repr/aux_time_repr.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_api/str_repr/aux_time_str.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_api/str_repr/dim_nontime_repr.txt
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_api/str_repr/dim_nontime_str.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_api/str_repr/dim_time_repr.txt
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_api/str_repr/dim_time_str.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.501356 scitools_iris-3.9.0/lib/iris/tests/results/coord_systems/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_systems/CoordSystem_xml_element.xml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_systems/GeogCS_init_no_invf.xml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_systems/GeogCS_init_no_major.xml
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_systems/GeogCS_init_no_minor.xml
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_systems/GeogCS_init_sphere.xml
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_systems/Mercator.xml
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_systems/PolarStereographic.xml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_systems/PolarStereographicScaleFactor.xml
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_systems/PolarStereographicStandardParallel.xml
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_systems/RotatedGeogCS_init.xml
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_systems/RotatedGeogCS_init_a.xml
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_systems/RotatedGeogCS_init_b.xml
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_systems/Stereographic.xml
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/coord_systems/TransverseMercator_osgb.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.509356 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/
--rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/latitude_longitude_dual_stage.cml
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/latitude_longitude_dual_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/latitude_longitude_single_stage.cml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/latitude_longitude_single_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/latitude_model_level_number_dual_stage.cml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/latitude_model_level_number_dual_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/latitude_model_level_number_single_stage.cml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/latitude_model_level_number_single_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/latitude_time_dual_stage.cml
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/latitude_time_dual_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/latitude_time_single_stage.cml
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/latitude_time_single_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/longitude_latitude_dual_stage.cml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/longitude_latitude_dual_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/longitude_latitude_single_stage.cml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/longitude_latitude_single_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/longitude_model_level_number_dual_stage.cml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/longitude_model_level_number_dual_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/longitude_model_level_number_single_stage.cml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/longitude_model_level_number_single_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/longitude_time_dual_stage.cml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/longitude_time_dual_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/longitude_time_single_stage.cml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/longitude_time_single_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/model_level_number_latitude_dual_stage.cml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/model_level_number_latitude_dual_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/model_level_number_latitude_single_stage.cml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/model_level_number_latitude_single_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/model_level_number_longitude_dual_stage.cml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/model_level_number_longitude_dual_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/model_level_number_longitude_single_stage.cml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/model_level_number_longitude_single_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/model_level_number_time_dual_stage.cml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/model_level_number_time_dual_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/model_level_number_time_single_stage.cml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/model_level_number_time_single_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/original.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/time_latitude_dual_stage.cml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/time_latitude_dual_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/time_latitude_single_stage.cml
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/time_latitude_single_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/time_longitude_dual_stage.cml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/time_longitude_dual_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/time_longitude_single_stage.cml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/time_longitude_single_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/time_model_level_number_dual_stage.cml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/time_model_level_number_dual_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/time_model_level_number_single_stage.cml
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/time_model_level_number_single_stage.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/triple_collapse_lat_ml_pt.cml
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/triple_collapse_lat_ml_pt.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/triple_collapse_ml_pt_lon.cml
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/triple_collapse_ml_pt_lon.data.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.373357 scitools_iris-3.9.0/lib/iris/tests/results/cube_io/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.509356 scitools_iris-3.9.0/lib/iris/tests/results/cube_io/pickling/
--rw-r--r--   0 runner    (1001) docker     (127)    19671 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_io/pickling/cubelist.cml
--rw-r--r--   0 runner    (1001) docker     (127)    17363 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_io/pickling/single_cube.cml
--rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_io/pickling/theta.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.373357 scitools_iris-3.9.0/lib/iris/tests/results/cube_io/pp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.509356 scitools_iris-3.9.0/lib/iris/tests/results/cube_io/pp/load/
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_io/pp/load/global.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.509356 scitools_iris-3.9.0/lib/iris/tests/results/cube_merge/
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_merge/multidim_coord_merge.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_merge/multidim_coord_merge_transpose.cml
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_merge/test_orig_point_cube.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_merge/test_simple_attributes1.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_merge/test_simple_attributes2.cml
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_merge/test_simple_attributes3.cml
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_merge/test_simple_bound_merge.cml
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_merge/test_simple_merge.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.513356 scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/2d_intersect_and_reverse.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/2d_orig.cml
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/2d_to_0d_cube_slice.cml
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/2d_to_1d_cube_multi_slice.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/2d_to_1d_cube_multi_slice2.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/2d_to_1d_cube_multi_slice3.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/2d_to_1d_cube_slice.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/2d_to_2d_revesed.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/2d_transposed.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/real_data_dual_tuple_indexing1.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/real_data_dual_tuple_indexing2.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/real_data_dual_tuple_indexing3.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/real_empty_data_indexing.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.513356 scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/
--rw-r--r--   0 runner    (1001) docker     (127)    17000 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/append_multi.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/append_single.txt
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/default_coord_system.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/depth.latitude.pp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/depth.time.pp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/eta.latitude.pp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/no_forecast_period.cml
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/no_forecast_period.txt
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/no_forecast_time.cml
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/no_forecast_time.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/pressure.latitude.pp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/pressure.time.pp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/replace_multi.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/replace_single.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/simple.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.517356 scitools_iris-3.9.0/lib/iris/tests/results/derived/
--rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/derived/column.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/derived/no_orog.__str__.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/derived/no_orog.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/derived/removed_derived_coord.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/derived/removed_orog.__str__.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/derived/removed_orog.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/derived/removed_sigma.__str__.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16859 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/derived/removed_sigma.cml
--rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/derived/transposed.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.373357 scitools_iris-3.9.0/lib/iris/tests/results/experimental/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.373357 scitools_iris-3.9.0/lib/iris/tests/results/experimental/analysis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.373357 scitools_iris-3.9.0/lib/iris/tests/results/experimental/analysis/interpolate/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.517356 scitools_iris-3.9.0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/basic_orthogonal_cube.cml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/basic_orthogonal_cube.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_1d_squashed.cml
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_1d_squashed.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_1d_squashed_2.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_with_factory.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.373357 scitools_iris-3.9.0/lib/iris/tests/results/experimental/regrid/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.517356 scitools_iris-3.9.0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/const_lat_cross_section.cml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/const_lat_cross_section.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/const_lon_cross_section.cml
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/const_lon_cross_section.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/higher.cml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/higher.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/hybridheight.cml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/hybridheight.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/latlonreduced.cml
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/latlonreduced.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/lonhalved.cml
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/lonhalved.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/lower.cml
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/lower.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/simple.cml
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/simple.data.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.521356 scitools_iris-3.9.0/lib/iris/tests/results/experimental/ugrid/
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/ugrid/2D_1t_face_half_levels.cml
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/ugrid/2D_72t_face_half_levels.cml
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/ugrid/3D_1t_face_full_levels.cml
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/ugrid/3D_1t_face_half_levels.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/ugrid/3D_snow_pseudo_levels.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/ugrid/3D_soil_pseudo_levels.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/ugrid/3D_tile_pseudo_levels.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/ugrid/3D_veg_pseudo_levels.cml
--rw-r--r--   0 runner    (1001) docker     (127)    50900 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/experimental/ugrid/surface_mean.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.521356 scitools_iris-3.9.0/lib/iris/tests/results/file_load/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/file_load/known_loaders.txt
--rw-r--r--   0 runner    (1001) docker     (127)    97746 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/file_load/theta_levels.cml
--rw-r--r--   0 runner    (1001) docker     (127)    97417 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/file_load/u_wind_levels.cml
--rw-r--r--   0 runner    (1001) docker     (127)    97417 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/file_load/v_wind_levels.cml
--rw-r--r--   0 runner    (1001) docker     (127)   194764 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/file_load/wind_levels.cml
--rw-r--r--   0 runner    (1001) docker     (127)    31710 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/imagerepo.json
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/incompatible_attr.str.txt
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/incompatible_cubes.str.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/incompatible_meth.str.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/incompatible_name.str.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/incompatible_unit.str.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.373357 scitools_iris-3.9.0/lib/iris/tests/results/integration/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.373357 scitools_iris-3.9.0/lib/iris/tests/results/integration/climatology/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.521356 scitools_iris-3.9.0/lib/iris/tests/results/integration/climatology/TestClimatology/
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/integration/climatology/TestClimatology/reference_simpledata.cdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.373357 scitools_iris-3.9.0/lib/iris/tests/results/integration/experimental/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.373357 scitools_iris-3.9.0/lib/iris/tests/results/integration/experimental/ugrid_save/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.521356 scitools_iris-3.9.0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex1_1d_mesh.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex2_2d_triangular.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex3_2d_flexible.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex4_3d_layered.cdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.373357 scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.373357 scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/attributes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.521356 scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/attributes/TestUmVersionAttribute/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/attributes/TestUmVersionAttribute/multiple_different_saves_on_variables.cdl
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/attributes/TestUmVersionAttribute/multiple_same_saves_as_global.cdl
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/attributes/TestUmVersionAttribute/single_saves_as_global.cdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.373357 scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/aux_factories/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.521356 scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/aux_factories/TestAtmosphereSigma/
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/aux_factories/TestAtmosphereSigma/save.cdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.521356 scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/aux_factories/TestHybridPressure/
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/aux_factories/TestHybridPressure/save.cdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.525356 scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/aux_factories/TestSaveMultipleAuxFactories/
--rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/aux_factories/TestSaveMultipleAuxFactories/hybrid_height_and_pressure.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/aux_factories/TestSaveMultipleAuxFactories/hybrid_height_cubes.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.373357 scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/general/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.525356 scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/general/TestDatasetAndPathSaves/
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/general/TestDatasetAndPathSaves/basic_save.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/general/TestDatasetAndPathSaves/path_string_save_same.cdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.525356 scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/multi_packed_multi_dtype.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/multi_packed_single_dtype.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/single_packed_manual.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/single_packed_signed.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/single_packed_unsigned.cdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.377357 scitools_iris-3.9.0/lib/iris/tests/results/integration/um/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.377357 scitools_iris-3.9.0/lib/iris/tests/results/integration/um/fieldsfile/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.525356 scitools_iris-3.9.0/lib/iris/tests/results/integration/um/fieldsfile/TestStructuredLoadFF/
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/integration/um/fieldsfile/TestStructuredLoadFF/simple.cml
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/integration/um/fieldsfile/TestStructuredLoadFF/simple_callback.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.525356 scitools_iris-3.9.0/lib/iris/tests/results/iterate/
--rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/iterate/izip_nd_ortho.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.529356 scitools_iris-3.9.0/lib/iris/tests/results/merge/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/a_aux_b_aux.cml
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/a_aux_b_dim.cml
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/a_dim_b_aux.cml
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/a_dim_b_dim.cml
--rw-r--r--   0 runner    (1001) docker     (127)    24030 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/dec.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/multi_split.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/separable_combination.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/single_split.cml
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/string_a_b.cml
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/string_a_with_aux.cml
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/string_a_with_dim.cml
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/string_b_with_aux.cml
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/string_b_with_dim.cml
--rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/theta.cml
--rw-r--r--   0 runner    (1001) docker     (127)    17223 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/theta_two_times.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_duplicate_data.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_independent.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_merging1.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_merging2.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_merging3.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_merging4.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_merging5.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_non_expanding.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_series.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_single_forecast.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_successive_forecasts.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_time_non_dim_coord.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_time_vs_forecast.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_time_vs_ref_time.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.533356 scitools_iris-3.9.0/lib/iris/tests/results/name/
--rw-r--r--   0 runner    (1001) docker     (127)    14642 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEIII_field.cml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEIII_field.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEIII_field.data.1.json
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEIII_field.data.2.json
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEIII_field.data.3.json
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEIII_field.data.4.json
--rw-r--r--   0 runner    (1001) docker     (127)    18200 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEIII_timeseries.cml
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEIII_timeseries.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEIII_timeseries.data.1.json
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEIII_timeseries.data.2.json
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEIII_timeseries.data.3.json
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEIII_timeseries.data.4.json
--rw-r--r--   0 runner    (1001) docker     (127)    49155 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEIII_trajectory.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEIII_trajectory0.cml
--rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEIII_version2.cml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEIII_version2.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEIII_version2.data.1.json
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEIII_version2.data.2.json
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEIII_version2.data.3.json
--rw-r--r--   0 runner    (1001) docker     (127)    14006 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEII_field.cml
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEII_field.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEII_field.data.1.json
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEII_field.data.2.json
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEII_field.data.3.json
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEII_field.data.4.json
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEII_field__no_time_averaging.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEII_field__no_time_averaging_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEII_timeseries.cml
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEII_timeseries.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEII_timeseries.data.1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.541356 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.541356 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/aliases.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/flag.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/fulldims.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/multiple.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/partialdims.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/shared.cdl
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/int64_auxiliary_coord_netcdf3.cml
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/int64_data_netcdf3.cml
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/int64_dimension_coord_netcdf3.cml
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/multi_dim_coord_slightly_different.cdl
--rw-r--r--   0 runner    (1001) docker     (127)    24811 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_cell_methods.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_deferred_index_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_deferred_index_1.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_deferred_index_2.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_deferred_mix_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_deferred_mix_1.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_deferred_slice_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_deferred_slice_1.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_deferred_slice_2.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_deferred_tuple_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_deferred_tuple_1.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_deferred_tuple_2.cml
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_global_xyt_hires.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_global_xyt_total.cml
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_global_xyzt_gems.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_global_xyzt_gems_iter_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_global_xyzt_gems_iter_1.cml
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_laea.cml
--rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_lcc.cml
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_merc.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_merc_false.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_merc_scale_factor.cml
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_monotonic.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_polar.cml
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_rotated_xy_land.cml
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_rotated_xyt_precipitation.cml
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_conf_aux.cdl
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_conf_name.cdl
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_confl_attr.cdl
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_confl_global_attr.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_gridmapmulti.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_hybrid_height.cdl
--rw-r--r--   0 runner    (1001) docker     (127)    17318 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_load_hybrid_height.cml
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_load_ndim_auxiliary.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_multi_0.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_multi_1.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_multi_2.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_multiple.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_ndim_auxiliary.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_no_global_attr.cdl
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_no_name.cdl
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_nocoord.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_realistic_0d.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_realistic_4d.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_realistic_4d_no_hybrid.cdl
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_samedimcoord.cdl
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_samevar.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_single.cdl
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_wcoord.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_stereo.cml
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_tmerc_and_climatology.cml
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_units_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_units_1.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/save_load_traj.cml
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/uint32_auxiliary_coord_netcdf3.cml
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/uint32_data_netcdf3.cml
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/netcdf/uint32_dimension_coord_netcdf3.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.549356 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/levels_below_ground.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/load_2flds.cml
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/mockography.cml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/period_of_interest.cml
--rw-r--r--   0 runner    (1001) docker     (127)   115358 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/probability_fields.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_bmr04_precip_2km.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_bsr05_precip_accum60_2km.cml
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_cloud3d0060_2km.cml
--rw-r--r--   0 runner    (1001) docker     (127)    18157 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_cloud_2km.cml
--rw-r--r--   0 runner    (1001) docker     (127)    23363 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_convection_2km.cml
--rw-r--r--   0 runner    (1001) docker     (127)    16563 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_convwind_2km.cml
--rw-r--r--   0 runner    (1001) docker     (127)    20032 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_frzlev_2km.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_height_2km.cml
--rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_precip_2km.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_precipaccum_2km.cml
--rw-r--r--   0 runner    (1001) docker     (127)    22519 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_preciptype_2km.cml
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_pressure_2km.cml
--rw-r--r--   0 runner    (1001) docker     (127)    17256 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_radiation_2km.cml
--rw-r--r--   0 runner    (1001) docker     (127)     7563 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_radiationuv_2km.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_refl_2km.cml
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_relhumidity3d0060_2km.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_relhumidity_2km.cml
--rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_snow_2km.cml
--rw-r--r--   0 runner    (1001) docker     (127)    11254 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_soil3d0060_2km.cml
--rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_soil_2km.cml
--rw-r--r--   0 runner    (1001) docker     (127)    11199 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_temperature_2km.cml
--rw-r--r--   0 runner    (1001) docker     (127)    13697 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_visibility_2km.cml
--rw-r--r--   0 runner    (1001) docker     (127)    16661 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_wind_2km.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_winduv3d0015_2km.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_winduv_2km.cml
--rw-r--r--   0 runner    (1001) docker     (127)    15065 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek01_cape_2km.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek07_precip0540_accum180_18km.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_umqv_fog_2km.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.377357 scitools_iris-3.9.0/lib/iris/tests/results/pandas/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.549356 scitools_iris-3.9.0/lib/iris/tests/results/pandas/as_cube/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/pandas/as_cube/data_frame_datetime_standard.cml
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/pandas/as_cube/data_frame_masked.cml
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/pandas/as_cube/data_frame_multidim.cml
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/pandas/as_cube/data_frame_netcdftime_360.cml
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/pandas/as_cube/data_frame_nonotonic.cml
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/pandas/as_cube/data_frame_simple.cml
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/pandas/as_cube/series_datetime_standard.cml
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/pandas/as_cube/series_masked.cml
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/pandas/as_cube/series_netcdfimte_360.cml
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/pandas/as_cube/series_object.cml
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/pandas/as_cube/series_simple.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.549356 scitools_iris-3.9.0/lib/iris/tests/results/pp_load_rules/
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/pp_load_rules/global.cml
--rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/pp_load_rules/lbproc_mean_max_min.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/pp_load_rules/lbtim_2.cml
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/pp_load_rules/ocean_depth.cml
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/pp_load_rules/ocean_depth_bounded.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/pp_load_rules/rotated_uk.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.549356 scitools_iris-3.9.0/lib/iris/tests/results/stock/
--rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/stock/realistic_4d.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.553356 scitools_iris-3.9.0/lib/iris/tests/results/system/
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/system/supported_filetype_.nc.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/system/supported_filetype_.pp.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.553356 scitools_iris-3.9.0/lib/iris/tests/results/trajectory/
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/trajectory/constant_latitude.cml
--rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/trajectory/hybrid_height.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/trajectory/single_point.cml
--rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/trajectory/tri_polar_latitude_slice.cml
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/trajectory/zigzag.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.381357 scitools_iris-3.9.0/lib/iris/tests/results/unit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.377357 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.377357 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/cartography/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.377357 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/cartography/project/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.553356 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/cartography/project/TestAll/
--rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/cartography/project/TestAll/cube.cml
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/cartography/project/TestAll/cube.data.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.377357 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.377357 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.553356 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/
--rw-r--r--   0 runner    (1001) docker     (127)    16599 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_all_dims.cml
--rw-r--r--   0 runner    (1001) docker     (127)    16599 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_last_dims.cml
--rw-r--r--   0 runner    (1001) docker     (127)    16599 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_middle_dim.cml
--rw-r--r--   0 runner    (1001) docker     (127)    16599 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_zeroth_dim.cml
--rw-r--r--   0 runner    (1001) docker     (127)    16599 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/slice.cml
--rw-r--r--   0 runner    (1001) docker     (127)    16599 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/transposed.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.377357 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.553356 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_all_dims.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_last_dims.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_middle_dim.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_zeroth_dim.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/slice.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/transposed.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.553356 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_all_dims.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_last_dims.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_middle_dim.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_zeroth_dim.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/slice.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/transposed.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.377357 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/add/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.557356 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_all_dims.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_last_dims.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_middle_dim.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_zeroth_dim.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/slice.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/transposed.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.377357 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/divide/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.557356 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_all_dims.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_last_dims.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_middle_dim.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_zeroth_dim.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/slice.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/transposed.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.377357 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/multiply/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.557356 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/
--rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_all_dims.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_last_dims.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_middle_dim.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_zeroth_dim.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/slice.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/transposed.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.377357 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/subtract/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.557356 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_all_dims.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_last_dims.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_middle_dim.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_zeroth_dim.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/slice.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/transposed.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.377357 scitools_iris-3.9.0/lib/iris/tests/results/unit/cube/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.377357 scitools_iris-3.9.0/lib/iris/tests/results/unit/cube/Cube/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.561356 scitools_iris-3.9.0/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/metadata.cml
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/metadata.data.0.json
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/metadata_wrapped.cml
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/metadata_wrapped.data.0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.561356 scitools_iris-3.9.0/lib/iris/tests/results/unit/cube/Cube/xml/
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/cube/Cube/xml/ancils.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/cube/Cube/xml/cell_measures.cml
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/cube/Cube/xml/checksum_ignores_masked_values.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.377357 scitools_iris-3.9.0/lib/iris/tests/results/unit/cube/CubeList/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.561356 scitools_iris-3.9.0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/combination_with_extra_realization.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/combination_with_extra_triple.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/combination_with_realization.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/orthogonal_with_realization.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.381357 scitools_iris-3.9.0/lib/iris/tests/results/unit/experimental/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.377357 scitools_iris-3.9.0/lib/iris/tests/results/unit/experimental/representation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.381357 scitools_iris-3.9.0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.561356 scitools_iris-3.9.0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content/mesh_result.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.561356 scitools_iris-3.9.0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content__string_attrs/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content__string_attrs/embedded_newlines_string_attribute.txt
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content__string_attrs/long_string_attribute.txt
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content__string_attrs/multi_string_attribute.txt
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content__string_attrs/simple_string_attribute.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.381357 scitools_iris-3.9.0/lib/iris/tests/results/unit/experimental/stratify/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.381357 scitools_iris-3.9.0/lib/iris/tests/results/unit/experimental/stratify/relevel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.561356 scitools_iris-3.9.0/lib/iris/tests/results/unit/experimental/stratify/relevel/Test/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/experimental/stratify/relevel/Test/multi_dim_target_levels.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.381357 scitools_iris-3.9.0/lib/iris/tests/results/unit/fileformats/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.381357 scitools_iris-3.9.0/lib/iris/tests/results/unit/fileformats/netcdf/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.381357 scitools_iris-3.9.0/lib/iris/tests/results/unit/fileformats/netcdf/saver/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.381357 scitools_iris-3.9.0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.561356 scitools_iris-3.9.0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/endian.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/mercator.cdl
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/mercator_no_ellipsoid.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/stereographic.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/stereographic_no_ellipsoid.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/stereographic_scale_factor.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/transverse_mercator.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/transverse_mercator_no_ellipsoid.cdl
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/with_climatology.cdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.381357 scitools_iris-3.9.0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver__ugrid/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.561356 scitools_iris-3.9.0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver__ugrid/TestSaveUgrid__cube/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver__ugrid/TestSaveUgrid__cube/basic_mesh.cdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.381357 scitools_iris-3.9.0/lib/iris/tests/results/unit/merge/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.381357 scitools_iris-3.9.0/lib/iris/tests/results/unit/merge/ProtoCube/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.561356 scitools_iris-3.9.0/lib/iris/tests/results/unit/merge/ProtoCube/register__CoordSig_general/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/merge/ProtoCube/register__CoordSig_general/noise.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.561356 scitools_iris-3.9.0/lib/iris/tests/results/unit/merge/ProtoCube/register__CubeSig/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/merge/ProtoCube/register__CubeSig/noise.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.381357 scitools_iris-3.9.0/lib/iris/tests/results/unit/util/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.561356 scitools_iris-3.9.0/lib/iris/tests/results/unit/util/describe_diff/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/util/describe_diff/incompatible_array_attrs.str.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.565356 scitools_iris-3.9.0/lib/iris/tests/results/unit/util/mask_cube/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.565356 scitools_iris-3.9.0/lib/iris/tests/results/unit/util/mask_cube/TestCubeMask/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/util/mask_cube/TestCubeMask/mask_cube_2d_create_new_dim.cml
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/util/mask_cube/original_cube_full2d_global.cml
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/util/mask_cube/original_cube_simple_1d.cml
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/unit/util/mask_cube/original_cube_simple_2d.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.565356 scitools_iris-3.9.0/lib/iris/tests/results/uri_callback/
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/uri_callback/pp_global.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.381357 scitools_iris-3.9.0/lib/iris/tests/results/usecases/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.381357 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.569356 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.03.236.000128.1990.12.01.00.00.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.03.236.004224.1990.12.01.00.00.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.03.236.008320.1990.12.01.00.00.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.16.202.000128.1860.09.01.00.00.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/001000000000.00.000.000000.1860.01.01.00.00.f.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/002000000000.44.101.131200.1920.09.01.00.00.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/008000000000.44.101.000128.1890.09.01.00.00.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/12187.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/HadCM2_ts_SAT_ann_18602100.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_level_lat_orig.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_lon_lat_press_orig.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_lon_lat_several.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_n10r13xy.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_time_press.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_tseries.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abcza_pa19591997_daily_29.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abcza_pa19591997_daily_29.b_1.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abcza_pa19591997_daily_29.b_2.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abxpa_press_lat.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/integer.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/model.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/ocean_xsect.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/st0fc699.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/st0fc942.b_0.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/st30211.b_0.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.569356 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.03.236.000128.1990.12.01.00.00.b.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.03.236.004224.1990.12.01.00.00.b.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.03.236.008320.1990.12.01.00.00.b.cml
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.16.202.000128.1860.09.01.00.00.b.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/001000000000.00.000.000000.1860.01.01.00.00.f.b.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/002000000000.44.101.131200.1920.09.01.00.00.b.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/008000000000.44.101.000128.1890.09.01.00.00.b.cml
--rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/12187.b.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/HadCM2_ts_SAT_ann_18602100.b.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_level_lat_orig.b.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_lon_lat_press_orig.b.cml
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_lon_lat_several.b.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_n10r13xy.b.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_time_press.b.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_tseries.b.cml
--rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/abcza_pa19591997_daily_29.b.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/abxpa_press_lat.b.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/integer.b.cml
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/model.b.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/ocean_xsect.b.cml
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/st0fc699.b.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/st0fc942.b.cml
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/st30211.b.cml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.573356 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.03.236.000128.1990.12.01.00.00.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.03.236.004224.1990.12.01.00.00.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.03.236.008320.1990.12.01.00.00.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.16.202.000128.1860.09.01.00.00.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/001000000000.00.000.000000.1860.01.01.00.00.f.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/002000000000.44.101.131200.1920.09.01.00.00.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/008000000000.44.101.000128.1890.09.01.00.00.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/12187.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/HadCM2_ts_SAT_ann_18602100.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_level_lat_orig.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_lon_lat_press_orig.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_lon_lat_several.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_n10r13xy.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_time_press.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_tseries.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abcza_pa19591997_daily_29.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abcza_pa19591997_daily_29.b_1.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abcza_pa19591997_daily_29.b_2.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abxpa_press_lat.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/integer.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/model.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/ocean_xsect.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/st0fc699.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/st0fc942.b_0.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/st30211.b_0.cdl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.573356 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.03.236.000128.1990.12.01.00.00.b.pp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.03.236.004224.1990.12.01.00.00.b.pp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.03.236.008320.1990.12.01.00.00.b.pp.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.16.202.000128.1860.09.01.00.00.b.pp.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.577355 scitools_iris-3.9.0/lib/iris/tests/stock/
--rw-r--r--   0 runner    (1001) docker     (127)    24891 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/stock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15181 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/stock/_stock_2d_latlons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.577355 scitools_iris-3.9.0/lib/iris/tests/stock/file_headers/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/stock/file_headers/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/stock/file_headers/minimal_bad_mesh_cf_role.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/stock/file_headers/minimal_bad_topology_dim.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/stock/file_headers/xios_2D_face_half_levels.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/stock/file_headers/xios_3D_face_full_levels.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/stock/file_headers/xios_3D_face_half_levels.cdl
--rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/stock/mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/stock/netcdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/system_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_abf.py
--rw-r--r--   0 runner    (1001) docker     (127)    49574 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_aggregate_by.py
--rw-r--r--   0 runner    (1001) docker     (127)    66121 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    29178 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_analysis_calculus.py
--rw-r--r--   0 runner    (1001) docker     (127)    32587 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_basic_maths.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_cartography.py
--rw-r--r--   0 runner    (1001) docker     (127)    50846 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_cdm.py
--rw-r--r--   0 runner    (1001) docker     (127)     9754 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)    15735 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_cf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10437 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_coding_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)    41997 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)    26671 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    34864 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_coord_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    18549 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_coordsystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_cube.py
--rw-r--r--   0 runner    (1001) docker     (127)    14064 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_cube_to_pp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_ff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_file_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_file_save.py
--rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_hybrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_image_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_intersect.py
--rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_io_init.py
--rw-r--r--   0 runner    (1001) docker     (127)    23755 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_iterate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_lazy_aggregate_by.py
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    41844 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_name.py
--rw-r--r--   0 runner    (1001) docker     (127)    53585 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_netcdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_nimrod.py
--rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_peak.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_pickling.py
--rw-r--r--   0 runner    (1001) docker     (127)    36173 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_pp_cf.py
--rw-r--r--   0 runner    (1001) docker     (127)    15490 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_pp_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_pp_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     8763 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_pp_to_cube.py
--rw-r--r--   0 runner    (1001) docker     (127)     9577 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_quickplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_std_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_uri_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.577355 scitools_iris-3.9.0/lib/iris/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.581355 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.581355 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/area_weighted/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/area_weighted/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/area_weighted/test_AreaWeightedRegridder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.581355 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/cartography/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/cartography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/cartography/test__get_lon_lat_coords.py
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/cartography/test__quadrant_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/cartography/test__xy_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/cartography/test_area_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)    12942 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/cartography/test_gridcell_angles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/cartography/test_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/cartography/test_rotate_grid_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    22434 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/cartography/test_rotate_winds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.581355 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/geometry/test__extract_relevant_cube_slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/geometry/test_geometry_area_weights.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.581355 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/interpolation/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/interpolation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22315 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/interpolation/test_RectilinearInterpolator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/interpolation/test_get_xy_dim_coords.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.585355 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/maths/
--rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/maths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/maths/test__arith__dask_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/maths/test__arith__derived_coords.py
--rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/maths/test__arith__meshcoords.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/maths/test__get_dtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/maths/test__inplace_common_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8037 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/maths/test__output_dtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/maths/test_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/maths/test_divide.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/maths/test_multiply.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/maths/test_subtract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.585355 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/regrid/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/regrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54848 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/regrid/test_RectilinearRegridder.py
--rw-r--r--   0 runner    (1001) docker     (127)    14597 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/regrid/test__CurvilinearRegridder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.585355 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/scipy_interpolate/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/scipy_interpolate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/scipy_interpolate/test__RegularGridInterpolator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.585355 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/stats/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8354 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/stats/test_pearsonr.py
--rw-r--r--   0 runner    (1001) docker     (127)    15006 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_Aggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_AreaWeighted.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_COUNT.py
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_Linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_MAX.py
--rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_MAX_RUN.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_MEAN.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_MIN.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_Nearest.py
--rw-r--r--   0 runner    (1001) docker     (127)    14272 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_PERCENTILE.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_PROPORTION.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_PercentileAggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_PointInCell.py
--rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_RMS.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_STD_DEV.py
--rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_SUM.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_VARIANCE.py
--rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_WPERCENTILE.py
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_WeightedPercentileAggregator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test__axis_to_single_trailing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.585355 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/trajectory/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/trajectory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/trajectory/test_Trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/trajectory/test_UnstructuredNearestNeighbourRegridder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/trajectory/test__nearest_neighbour_indices_ndcoords.py
--rw-r--r--   0 runner    (1001) docker     (127)    14365 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/analysis/trajectory/test_interpolate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.589355 scitools_iris-3.9.0/lib/iris/tests/unit/aux_factory/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/aux_factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10247 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/aux_factory/test_AtmosphereSigmaFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/aux_factory/test_AuxCoordFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/aux_factory/test_HybridPressureFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    10821 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/aux_factory/test_OceanSFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/aux_factory/test_OceanSg1Factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     9980 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/aux_factory/test_OceanSg2Factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/aux_factory/test_OceanSigmaFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    16785 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/aux_factory/test_OceanSigmaZFactory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.589355 scitools_iris-3.9.0/lib/iris/tests/unit/common/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.589355 scitools_iris-3.9.0/lib/iris/tests/unit/common/lenient/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/common/lenient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/common/lenient/test_Lenient.py
--rw-r--r--   0 runner    (1001) docker     (127)    27226 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/common/lenient/test__Lenient.py
--rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/common/lenient/test__lenient_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/common/lenient/test__lenient_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/common/lenient/test__qualname.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.589355 scitools_iris-3.9.0/lib/iris/tests/unit/common/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/common/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17596 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/common/metadata/test_AncillaryVariableMetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    57427 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/common/metadata/test_BaseMetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    24164 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/common/metadata/test_CellMeasureMetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    25452 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/common/metadata/test_CoordMetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    42695 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/common/metadata/test_CubeMetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/common/metadata/test__NamedTupleMeta.py
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/common/metadata/test_hexdigest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/common/metadata/test_metadata_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/common/metadata/test_metadata_manager_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.589355 scitools_iris-3.9.0/lib/iris/tests/unit/common/mixin/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/common/mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12829 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/common/mixin/test_CFVariableMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/common/mixin/test_LimitedAttributeDict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/common/mixin/test__get_valid_standard_name.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.593355 scitools_iris-3.9.0/lib/iris/tests/unit/common/resolve/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/common/resolve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   190389 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/common/resolve/test_Resolve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.593355 scitools_iris-3.9.0/lib/iris/tests/unit/concatenate/
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/concatenate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/concatenate/test__CoordMetaData.py
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/concatenate/test__CoordSignature.py
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/concatenate/test__CubeSignature.py
--rw-r--r--   0 runner    (1001) docker     (127)    16193 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/concatenate/test_concatenate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.593355 scitools_iris-3.9.0/lib/iris/tests/unit/config/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/config/test_NetCDF.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.593355 scitools_iris-3.9.0/lib/iris/tests/unit/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/constraints/test_Constraint_equality.py
--rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/constraints/test_NameConstraint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.593355 scitools_iris-3.9.0/lib/iris/tests/unit/coord_categorisation/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coord_categorisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coord_categorisation/test_add_categorised_coord.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coord_categorisation/test_add_hour.py
--rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coord_categorisation/test_coord_categorisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.597355 scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_AlbersEqualArea.py
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_GeogCS.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_Geostationary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_LambertAzimuthalEqualArea.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_LambertConformal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7540 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_Mercator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_ObliqueMercator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_Orthographic.py
--rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_PolarStereographic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_RotatedMercator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_RotatedPole.py
--rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_Stereographic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_TransverseMercator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_VerticalPerspective.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.597355 scitools_iris-3.9.0/lib/iris/tests/unit/coords/
--rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26049 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coords/test_AncillaryVariable.py
--rw-r--r--   0 runner    (1001) docker     (127)    29422 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coords/test_AuxCoord.py
--rw-r--r--   0 runner    (1001) docker     (127)     9244 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coords/test_Cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coords/test_CellMeasure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coords/test_CellMethod.py
--rw-r--r--   0 runner    (1001) docker     (127)    43553 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coords/test_Coord.py
--rw-r--r--   0 runner    (1001) docker     (127)    22247 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coords/test_DimCoord.py
--rw-r--r--   0 runner    (1001) docker     (127)    37979 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/coords/test__DimensionalMetadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.597355 scitools_iris-3.9.0/lib/iris/tests/unit/cube/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/cube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   133812 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/cube/test_Cube.py
--rw-r--r--   0 runner    (1001) docker     (127)    15580 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/cube/test_CubeAttrsDict.py
--rw-r--r--   0 runner    (1001) docker     (127)    26077 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/cube/test_CubeList.py
--rw-r--r--   0 runner    (1001) docker     (127)    31206 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/cube/test_Cube__aggregated_by.py
--rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/cube/test_Cube__operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.597355 scitools_iris-3.9.0/lib/iris/tests/unit/data_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/data_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21578 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/data_manager/test_DataManager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.597355 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.601355 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/geovista/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/geovista/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/geovista/test_cube_to_polydata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/geovista/test_extract_unstructured_region.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.601355 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/raster/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/raster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/raster/test_export_geotiff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.601355 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/regrid/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/regrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/regrid/test_regrid_area_weighted_rectilinear_src_and_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)    13938 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/regrid/test_regrid_weighted_curvilinear_to_rectilinear.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.601355 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/representation/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/representation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/representation/test_CubeListRepresentation.py
--rw-r--r--   0 runner    (1001) docker     (127)    17300 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/representation/test_CubeRepresentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.601355 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/stratify/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/stratify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/stratify/test_relevel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.601355 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.601355 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/cf/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/cf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridAuxiliaryCoordinateVariable.py
--rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridConnectivityVariable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)    10008 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridMeshVariable.py
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridReader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.601355 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/load/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/load/test_ParseUgridOnLoad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/load/test_load_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     7747 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/load/test_load_meshes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.605355 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12646 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/mesh/test_Connectivity.py
--rw-r--r--   0 runner    (1001) docker     (127)    48842 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/mesh/test_Mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    37097 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/mesh/test_MeshCoord.py
--rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/mesh/test_Mesh__from_coords.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.605355 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27719 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/metadata/test_ConnectivityMetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    25591 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/metadata/test_MeshCoordMetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    28317 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/metadata/test_MeshMetadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.605355 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18413 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/utils/test_recombine_submeshes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.605355 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.605355 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/abf/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/abf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/abf/test_ABFField.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.605355 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/cf/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/cf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/cf/test_CFGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)    14723 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/cf/test_CFReader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.605355 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/dot/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/dot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/dot/test__dot_path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.605355 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/ff/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/ff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/ff/test_ArakawaC.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/ff/test_ENDGame.py
--rw-r--r--   0 runner    (1001) docker     (127)    19381 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/ff/test_FF2PP.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/ff/test_FFHeader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/ff/test_Grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/ff/test_NewDynamics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.609355 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/name_loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/name_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/name_loaders/test__build_cell_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/name_loaders/test__build_lat_lon_for_NAME_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/name_loaders/test__calc_integration_period.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/name_loaders/test__cf_height_from_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/name_loaders/test__generate_cubes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.609355 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.609355 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/
--rw-r--r--   0 runner    (1001) docker     (127)     5996 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35919 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__grid_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)    11753 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__hybrid_formulae.py
--rw-r--r--   0 runner    (1001) docker     (127)    12070 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__latlon_dimcoords.py
--rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__miscellaneous.py
--rw-r--r--   0 runner    (1001) docker     (127)    17201 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__time_coords.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.609355 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/engine/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/engine/test_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.613355 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test__normalise_bounds_units.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_albers_equal_area_coordinate_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_ancil_var.py
--rw-r--r--   0 runner    (1001) docker     (127)    13185 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_auxiliary_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_cell_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_cube_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    20525 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_dimension_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_geostationary_coordinate_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_lambert_azimuthal_equal_area_coordinate_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_lambert_conformal_coordinate_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_mercator_coordinate_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_oblique_mercator_coordinate_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_polar_stereographic_coordinate_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_stereographic_coordinate_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_transverse_mercator_coordinate_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_verticalp_coordinate_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_get_attr_units.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_get_cf_bounds_var.py
--rw-r--r--   0 runner    (1001) docker     (127)    11376 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_get_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_has_supported_mercator_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_has_supported_polar_stereographic_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_parse_cell_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_reorder_bounds_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.613355 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.613355 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/loader/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/loader/test__chunk_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/loader/test__get_cf_var_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/loader/test__load_aux_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/loader/test__load_cube.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/loader/test__translate_constraints_to_var_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)    11463 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/loader/test_load_cubes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.613355 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/saver/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/saver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39213 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver__lazy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver__lazy_stream_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    48377 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver__ugrid.py
--rw-r--r--   0 runner    (1001) docker     (127)    18106 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/saver/test_save.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.617355 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nimrod_load_rules/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nimrod_load_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nimrod_load_rules/test_units.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nimrod_load_rules/test_vertical_coord.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.617355 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp/test_PPDataProxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    12723 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp/test_PPField.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp/test__convert_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp/test__create_field_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7117 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp/test__data_bytes_to_shaped_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp/test__field_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp/test__interpret_field.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp/test_as_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp/test_load.py
--rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp/test_save.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp/test_save_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp/test_save_pairs_from_cube.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.621355 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp_load_rules/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp_load_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp_load_rules/test__all_other_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp_load_rules/test__collapse_degenerate_points_and_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_scalar_pseudo_level_coords.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_scalar_realization_coords.py
--rw-r--r--   0 runner    (1001) docker     (127)    24943 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_time_coords.py
--rw-r--r--   0 runner    (1001) docker     (127)    23086 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_vertical_coords.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp_load_rules/test__dim_or_aux.py
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp_load_rules/test__epoch_date_hours.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp_load_rules/test__model_level_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp_load_rules/test__reduced_points_and_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp_load_rules/test__reshape_vector_args.py
--rw-r--r--   0 runner    (1001) docker     (127)    13641 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp_load_rules/test_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.621355 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/rules/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/rules/test_Loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/rules/test__make_cube.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.621355 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/structured_array_identification/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/structured_array_identification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/structured_array_identification/test_ArrayStructure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/structured_array_identification/test_GroupStructure.py
--rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/test_rules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.621355 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/um/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/um/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.621355 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/um/fast_load/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/um/fast_load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/um/fast_load/test_FieldCollation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/um/fast_load/test__convert_collation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.621355 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/um/fast_load_structured_fields/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/um/fast_load_structured_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/um/fast_load_structured_fields/test_BasicFieldCollation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/um/fast_load_structured_fields/test_group_structured_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.621355 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/um/optimal_array_structuring/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/um/optimal_array_structuring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9395 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/um/optimal_array_structuring/test_optimal_array_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/um/test_um_to_pp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.621355 scitools_iris-3.9.0/lib/iris/tests/unit/io/
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/io/test__generate_cubes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/io/test_expand_filespecs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/io/test_run_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/io/test_save.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.625355 scitools_iris-3.9.0/lib/iris/tests/unit/lazy_data/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/lazy_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/lazy_data/test_as_concrete_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7382 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/lazy_data/test_as_lazy_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/lazy_data/test_co_realise_cubes.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/lazy_data/test_is_lazy_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/lazy_data/test_is_lazy_masked_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/lazy_data/test_lazy_elementwise.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/lazy_data/test_map_complete_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/lazy_data/test_multidim_lazy_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/lazy_data/test_non_lazy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.625355 scitools_iris-3.9.0/lib/iris/tests/unit/merge/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/merge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16831 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/merge/test_ProtoCube.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.625355 scitools_iris-3.9.0/lib/iris/tests/unit/pandas/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47771 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/pandas/test_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.625355 scitools_iris-3.9.0/lib/iris/tests/unit/plot/
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/plot/_blockplot_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/plot/test__check_bounds_contiguity_and_mask.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/plot/test__check_geostationary_coords_and_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/plot/test__fixup_dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/plot/test__get_plot_defn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/plot/test__get_plot_defn_custom_coords_picked.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/plot/test__get_plot_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/plot/test__replace_axes_with_cartopy_axes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/plot/test_contour.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/plot/test_contourf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/plot/test_hist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/plot/test_outline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/plot/test_pcolor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/plot/test_pcolormesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/plot/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/plot/test_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/plot/test_scatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.629355 scitools_iris-3.9.0/lib/iris/tests/unit/quickplot/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/quickplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/quickplot/test_contour.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/quickplot/test_contourf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/quickplot/test_outline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/quickplot/test_pcolor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/quickplot/test_pcolormesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/quickplot/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/quickplot/test_points.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/quickplot/test_scatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.629355 scitools_iris-3.9.0/lib/iris/tests/unit/representation/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/representation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.629355 scitools_iris-3.9.0/lib/iris/tests/unit/representation/cube_printout/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/representation/cube_printout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22090 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/representation/cube_printout/test_CubePrintout.py
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/representation/cube_printout/test_Table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.629355 scitools_iris-3.9.0/lib/iris/tests/unit/representation/cube_summary/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/representation/cube_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/representation/cube_summary/test_CubeSummary.py
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/test_Future.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/test_sample_data_path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.629355 scitools_iris-3.9.0/lib/iris/tests/unit/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.629355 scitools_iris-3.9.0/lib/iris/tests/unit/tests/stock/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/tests/stock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/tests/stock/test_netcdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/tests/test_IrisTest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.629355 scitools_iris-3.9.0/lib/iris/tests/unit/time/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/time/test_PartialDateTime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.633355 scitools_iris-3.9.0/lib/iris/tests/unit/util/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/util/test__coord_regular.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/util/test__is_circular.py
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/util/test__mask_array.py
--rw-r--r--   0 runner    (1001) docker     (127)    15236 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/util/test__slice_data_with_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/util/test_array_equal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/util/test_broadcast_to_shape.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/util/test_column_slices_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/util/test_demote_dim_coord_to_aux_coord.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/util/test_describe_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     9500 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/util/test_equalise_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/util/test_file_is_newer_than.py
--rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/util/test_find_discontiguities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/util/test_guess_coord_axis.py
--rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/util/test_mask_cube.py
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/util/test_mask_cube_from_shapefile.py
--rw-r--r--   0 runner    (1001) docker     (127)    12248 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/util/test_new_axis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/util/test_promote_aux_coord_to_dim_coord.py
--rw-r--r--   0 runner    (1001) docker     (127)     7232 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/util/test_reverse.py
--rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/util/test_rolling_window.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/util/test_squeeze.py
--rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/tests/unit/util/test_unify_time_units.py
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/time.py
--rw-r--r--   0 runner    (1001) docker     (127)    74435 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/lib/iris/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.633355 scitools_iris-3.9.0/lib/scitools_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-04-22 09:26:06.000000 scitools_iris-3.9.0/lib/scitools_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    96854 2024-04-22 09:26:07.000000 scitools_iris-3.9.0/lib/scitools_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 09:26:06.000000 scitools_iris-3.9.0/lib/scitools_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 09:26:06.000000 scitools_iris-3.9.0/lib/scitools_iris.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-22 09:26:06.000000 scitools_iris-3.9.0/lib/scitools_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-22 09:26:06.000000 scitools_iris-3.9.0/lib/scitools_iris.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.633355 scitools_iris-3.9.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/requirements/pypi-core.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 09:26:07.637355 scitools_iris-3.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 09:26:07.633355 scitools_iris-3.9.0/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-22 09:25:59.000000 scitools_iris-3.9.0/tools/generate_std_names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:16.008775 scitools-iris-3.9.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9278 2024-04-03 11:05:16.008775 scitools-iris-3.9.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7430 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.744774 scitools-iris-3.9.0rc0/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)  4218305 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/etc/cf-standard-name-table.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.740774 scitools-iris-3.9.0rc0/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.756774 scitools-iris-3.9.0rc0/lib/iris/
+-rw-r--r--   0 runner    (1001) docker     (127)    16644 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51364 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/_concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24094 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17873 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/_lazy_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63568 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/_merge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.756774 scitools-iris-3.9.0rc0/lib/iris/_representation/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/_representation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12873 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/_representation/cube_printout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15000 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/_representation/cube_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/_shapefiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-03 11:05:15.000000 scitools-iris-3.9.0rc0/lib/iris/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.760774 scitools-iris-3.9.0rc0/lib/iris/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)   113060 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23979 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/analysis/_area_weighted.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17857 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/analysis/_grid_angles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25983 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/analysis/_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41706 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/analysis/_regrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12533 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/analysis/_scipy_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28843 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/analysis/calculus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46034 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/analysis/cartography.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/analysis/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37273 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/analysis/maths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/analysis/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36860 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/analysis/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70141 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/aux_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.760774 scitools-iris-3.9.0rc0/lib/iris/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/common/_split_attribute_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21880 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/common/lenient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55838 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/common/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/common/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)   108504 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/common/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9498 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14877 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/coord_categorisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58258 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/coord_systems.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113785 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)   190896 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/cube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.760774 scitools-iris-3.9.0rc0/lib/iris/etc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.716774 scitools-iris-3.9.0rc0/lib/iris/etc/palette/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.760774 scitools-iris-3.9.0rc0/lib/iris/etc/palette/diverging/
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/diverging/BrBG_11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/diverging/PRGn_11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/diverging/PiYG_11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/diverging/PuOr_11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/diverging/RdBu_11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/diverging/RdGy_11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/diverging/RdYlBu_11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/diverging/RdYlGn_11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/diverging/Spectral_11.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.764774 scitools-iris-3.9.0rc0/lib/iris/etc/palette/qualitative/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/qualitative/Accent_08.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/qualitative/Dark2_08.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/qualitative/Paired_12.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/qualitative/Pastel1_09.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/qualitative/Pastel2_08.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/qualitative/Set1_09.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/qualitative/Set2_08.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/qualitative/Set3_12.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.768774 scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/Blues_09.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/BuGn_09.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/BuPu_09.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/GnBu_09.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/Greens_09.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/Greys_09.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/OrRd_09.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/Oranges_09.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/PuBuGn_09.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/PuBu_09.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/PuRd_09.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/Purples_09.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/RdPu_09.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/Reds_09.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/YlGnBu_09.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/YlGn_09.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/YlOrBr_09.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/YlOrRd_09.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/etc/site.cfg.template
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.768774 scitools-iris-3.9.0rc0/lib/iris/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/experimental/animate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11702 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/experimental/geovista.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/experimental/raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28058 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/experimental/regrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12735 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/experimental/regrid_conservative.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13244 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/experimental/representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7269 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/experimental/stratify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.768774 scitools-iris-3.9.0rc0/lib/iris/experimental/ugrid/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/experimental/ugrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11957 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/experimental/ugrid/cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17472 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/experimental/ugrid/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113120 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/experimental/ugrid/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/experimental/ugrid/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/experimental/ugrid/save.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13262 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/experimental/ugrid/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.772774 scitools-iris-3.9.0rc0/lib/iris/fileformats/
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32983 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/_ff.py
+-rw-r--r--   0 runner    (1001) docker     (127)   196071 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/_ff_cross_references.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.772774 scitools-iris-3.9.0rc0/lib/iris/fileformats/_nc_load_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/_nc_load_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22814 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/_nc_load_rules/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/_nc_load_rules/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58767 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/_nc_load_rules/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/_pp_lbproc_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19004 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/_structured_array_identification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/abf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49681 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44568 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/name_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.776774 scitools-iris-3.9.0rc0/lib/iris/fileformats/netcdf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/netcdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/netcdf/_dask_locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15709 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/netcdf/_thread_safe_nc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32965 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/netcdf/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)   117932 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/netcdf/saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9595 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/nimrod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31785 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/nimrod_load_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81696 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/pp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46857 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/pp_load_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31086 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/pp_save_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15712 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.776774 scitools-iris-3.9.0rc0/lib/iris/fileformats/um/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/um/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20658 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/um/_fast_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12017 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/um/_fast_load_structured_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/um/_ff_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/um/_optimal_array_structuring.py
+-rw-r--r--   0 runner    (1001) docker     (127)   107311 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/fileformats/um_cf_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.776774 scitools-iris-3.9.0rc0/lib/iris/io/
+-rw-r--r--   0 runner    (1001) docker     (127)    17511 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/io/format_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12641 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/iterate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10862 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/palette.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35733 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71546 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.776774 scitools-iris-3.9.0rc0/lib/iris/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/plugins/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11201 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/quickplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.784774 scitools-iris-3.9.0rc0/lib/iris/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    39521 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.784774 scitools-iris-3.9.0rc0/lib/iris/tests/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.788774 scitools-iris-3.9.0rc0/lib/iris/tests/experimental/regrid/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/experimental/regrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25939 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/experimental/regrid/test_regrid_area_weighted_rectilinear_src_and_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30060 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/experimental/regrid/test_regrid_conservative_via_esmpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/experimental/test_raster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.788774 scitools-iris-3.9.0rc0/lib/iris/tests/graphics/
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/graphics/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/graphics/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6681 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/graphics/idiff.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2377 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/graphics/recreate_imagerepo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.792774 scitools-iris-3.9.0rc0/lib/iris/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.792774 scitools-iris-3.9.0rc0/lib/iris/tests/integration/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/analysis/test_area_weighted.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14908 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/attrs_matrix_results_load.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14164 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/attrs_matrix_results_roundtrip.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14164 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/attrs_matrix_results_save.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.792774 scitools-iris-3.9.0rc0/lib/iris/tests/integration/aux_factory/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/aux_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/aux_factory/test_OceanSigmaZFactory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.792774 scitools-iris-3.9.0rc0/lib/iris/tests/integration/concatenate/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/concatenate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16978 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/concatenate/test_concatenate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.792774 scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.792774 scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/geovista/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/geovista/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/geovista/test_cube_to_poly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/geovista/test_extract_unstructured_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/test_CubeRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/test_regrid_ProjectedUnstructured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8802 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/test_ugrid_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/test_ugrid_save.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.792774 scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex1_1d_mesh.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex2_2d_triangular.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex3_2d_flexible.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex4_3d_layered.cdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.792774 scitools-iris-3.9.0rc0/lib/iris/tests/integration/fast_load/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/fast_load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27776 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/fast_load/test_fast_load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.796774 scitools-iris-3.9.0rc0/lib/iris/tests/integration/merge/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/merge/test_merge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.796774 scitools-iris-3.9.0rc0/lib/iris/tests/integration/netcdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/netcdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/netcdf/test__dask_locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/netcdf/test_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/netcdf/test_aux_factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/netcdf/test_coord_systems.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10955 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/netcdf/test_delayed_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19738 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/netcdf/test_general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/netcdf/test_self_referencing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/netcdf/test_thread_safety.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.796774 scitools-iris-3.9.0rc0/lib/iris/tests/integration/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2462 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/plot/test_animate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/plot/test_colorbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/plot/test_netcdftime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/plot/test_nzdateline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/plot/test_plot_2d_coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/plot/test_vector_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_Datums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_PartialDateTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_climatology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_ff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4049 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_mask_cube_from_shapefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68487 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_netcdf__loadsaveattrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_new_axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29154 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_pp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_pp_constrained_load_cubes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8778 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_regrid_equivalence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9021 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_regridding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_trajectory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.796774 scitools-iris-3.9.0rc0/lib/iris/tests/integration/um/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/um/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/integration/um/test_fieldsfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.800774 scitools-iris-3.9.0rc0/lib/iris/tests/results/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.800774 scitools-iris-3.9.0rc0/lib/iris/tests/results/COLPEX/
+-rw-r--r--   0 runner    (1001) docker     (127)    37400 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/COLPEX/small_colpex_theta_p_alt.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.800774 scitools-iris-3.9.0rc0/lib/iris/tests/results/FF/
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/FF/air_temperature_1.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/FF/air_temperature_2.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    11329 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/FF/ffheader.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/FF/soil_temperature_1.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/FF/surface_altitude_1.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.800774 scitools-iris-3.9.0rc0/lib/iris/tests/results/PP/
+-rw-r--r--   0 runner    (1001) docker     (127)    14102 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/PP/extra_char_data.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14102 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/PP/extra_char_data.w_data_loaded.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15286 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/PP/extra_data_time_series.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   330620 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/PP/extra_x_data.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/PP/global_test.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/PP/nae_unpacked.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    30791 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/PP/rle_unpacked.pp.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.800774 scitools-iris-3.9.0rc0/lib/iris/tests/results/abf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/abf/load.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.824774 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/abs.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/addition.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/addition_coord_x.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/addition_coord_y.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/addition_different_std_name.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/addition_in_place.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/addition_in_place_coord.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/addition_scalar.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.828774 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/easy.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/multi.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/multi_missing.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/multi_shared.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/single.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/single_missing.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/single_rms.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/single_shared.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/single_shared_circular.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_easy.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_multi.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_multi_missing.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_multi_shared.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_single.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_single_missing.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_single_shared.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_single_shared_circular.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/apply_ifunc.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/apply_ifunc.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/apply_ifunc_frompyfunc.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/apply_ifunc_frompyfunc.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/apply_ifunc_original.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/apply_ifunc_original.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/apply_ufunc.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/apply_ufunc.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/apply_ufunc_frompyfunc.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/apply_ufunc_frompyfunc.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/apply_ufunc_original.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/apply_ufunc_original.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/areaweights_original.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.836774 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/cos_simple.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/cos_simple_radians.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/curl_contrived_cartesian2.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_simple_wrt_x.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_simple_wrt_x.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_lat.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_lat.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_lon.cml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_lon.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_x.cml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_x.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_y.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_y.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/grad_contrived1.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/grad_contrived2.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/grad_contrived_non_spherical1.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/handmade2_wrt_lat.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/handmade2_wrt_lat.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/handmade2_wrt_lon.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/handmade2_wrt_lon.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/handmade_simple_wrt_x.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/handmade_simple_wrt_x.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/handmade_wrt_lat.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/handmade_wrt_lat.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/handmade_wrt_lon.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/handmade_wrt_lon.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/handmade_wrt_x.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/handmade_wrt_x.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/handmade_wrt_y.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/handmade_wrt_y.data.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.836774 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube1_cube1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube2_cube1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube2_cube3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube2_cube4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube2_cube5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube3_cube4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube3_cube5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube4_cube5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/count_bar_2d.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/count_foo_1d.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/count_foo_2d.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/count_foo_bar_2d.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.840774 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/delta_one_element_explicit.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/midpoint_one_element_explicit.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple1.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple1_delta.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple1_midpoint.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple2.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple2_delta.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple2_midpoint.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple3.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple3_delta.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple3_midpoint.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple4.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple4_delta.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple4_midpoint.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple5.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple5_delta.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple5_midpoint.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/delta_and_midpoint/simple6.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/division.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/division_by_array.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/division_by_latitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/division_by_longitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/division_by_singular_coord.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/division_scalar.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/exp.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/exp.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/exponentiate.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/exponentiate.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/first_quartile_foo_1d.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/first_quartile_foo_1d_fast_percentile.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/first_quartile_foo_2d.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/first_quartile_foo_2d_fast_percentile.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/first_quartile_foo_bar_2d.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/first_quartile_foo_bar_2d_fast_percentile.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/gmean_latitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/gmean_latitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/gmean_latitude_longitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/gmean_latitude_longitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/gmean_latitude_longitude_1call.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/gmean_latitude_longitude_1call.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/hmean_latitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/hmean_latitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/hmean_latitude_longitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/hmean_latitude_longitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/hmean_latitude_longitude_1call.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/hmean_latitude_longitude_1call.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/last_quartile_foo_3d_masked.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/last_quartile_foo_3d_notmasked.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/last_quartile_foo_3d_notmasked_fast_percentile.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/log.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/log.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/log10.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/log10.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/log2.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/log2.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/maths_original.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/max_latitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/max_latitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/max_latitude_longitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/max_latitude_longitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/max_latitude_longitude_1call.cml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/max_latitude_longitude_1call.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/max_run_bar_2d.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/max_run_bar_2d_masked.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/max_run_foo_1d.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/max_run_foo_2d.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/mean_latitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/mean_latitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/mean_latitude_longitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/mean_latitude_longitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/mean_latitude_longitude_1call.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/mean_latitude_longitude_1call.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/median_latitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/median_latitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/median_latitude_longitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/median_latitude_longitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/median_latitude_longitude_1call.cml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/median_latitude_longitude_1call.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/min_latitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/min_latitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/min_latitude_longitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/min_latitude_longitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/min_latitude_longitude_1call.cml
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/min_latitude_longitude_1call.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/multiply.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/multiply_different_std_name.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/original.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/original_common.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/original_hmean.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/proportion_bar_2d.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/proportion_foo_1d.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/proportion_foo_2d.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/proportion_foo_2d_masked.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/proportion_foo_bar_2d.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.852774 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_both_circular.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_both_circular.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_circular_grid.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_circular_grid.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_circular_src.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_circular_src.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_circular_srcmissingmask.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_circular_srcmissingmask.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_masked_altitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_masked_altitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_non_circular.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_non_circular.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_partial_overlap.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_partial_overlap.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_subset.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_subset.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_subset_anon.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_subset_anon.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_subset_masked_1.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_subset_masked_1.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_subset_masked_2.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_subset_masked_2.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_both_circular.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_both_circular.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_circular_grid.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_circular_grid.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_circular_src.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_circular_src.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_circular_srcmissingmask.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_circular_srcmissingmask.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_masked_altitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_masked_altitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_non_circular.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_non_circular.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_partial_overlap.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_partial_overlap.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_subset.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_subset.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_subset_anon.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_subset_anon.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_subset_masked_1.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_subset_masked_1.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_subset_masked_2.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_subset_masked_2.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/no_overlap.cml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/no_overlap.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/rms_latitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/rms_latitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/rms_latitude_longitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/rms_latitude_longitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/rms_latitude_longitude_1call.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/rms_latitude_longitude_1call.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/rms_weighted_2d.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.852774 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/rolling_window/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/rolling_window/simple_latitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/rolling_window/simple_longitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/rolling_window/size_4_longitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/rotated_pole.0.rlat.json
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/rotated_pole.0.rlon.json
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/rotated_pole.0.x.json
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/rotated_pole.0.y.json
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/rotated_pole.1.rlat.json
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/rotated_pole.1.rlon.json
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/rotated_pole.1.x.json
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/rotated_pole.1.y.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/sqrt.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/std_dev_latitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/std_dev_latitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/std_dev_latitude_longitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/std_dev_latitude_longitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/std_dev_latitude_longitude_1call.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/std_dev_latitude_longitude_1call.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/subtract.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/subtract_array.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/subtract_coord_x.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/subtract_coord_y.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/subtract_scalar.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/sum_latitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/sum_latitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/sum_latitude_longitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/sum_latitude_longitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/sum_latitude_longitude_1call.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/sum_latitude_longitude_1call.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/sum_weighted_1d.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/sum_weighted_2d.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/third_quartile_foo_1d.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/third_quartile_foo_1d_fast_percentile.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/variance_latitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/variance_latitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/variance_latitude_longitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/variance_latitude_longitude.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/variance_latitude_longitude_1call.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/variance_latitude_longitude_1call.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/weighted_mean_lat.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/weighted_mean_lat.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/weighted_mean_latlon.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/weighted_mean_latlon.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/weighted_mean_lon.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/weighted_mean_lon.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/weighted_mean_original.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/weighted_mean_source.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.720774 scitools-iris-3.9.0rc0/lib/iris/tests/results/cartography/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.852774 scitools-iris-3.9.0rc0/lib/iris/tests/results/cartography/get_xy_grids/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cartography/get_xy_grids/1d.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cartography/get_xy_grids/2d.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.852774 scitools-iris-3.9.0rc0/lib/iris/tests/results/categorisation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/categorisation/customcheck.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/categorisation/quickcheck.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.852774 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.856774 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/0d_repr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/0d_str.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/1d_repr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/1d_str.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/2d_repr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/2d_str.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/3d_repr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/3d_str.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/4d_repr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/4d_str.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.856774 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/extract/
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/extract/lat_eq_10.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     6428 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/extract/lat_gt_10.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/extract/lat_gt_10_and_lon_ge_10.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/masked_cube.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/masked_save_pp.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.856774 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/str_repr/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/str_repr/0d_cube.__repr__.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/str_repr/0d_cube.__str__.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/str_repr/0d_cube.__unicode__.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/str_repr/cell_methods.__str__.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/str_repr/cubelist.__repr__.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/str_repr/cubelist.__str__.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/str_repr/missing_coords_cube.repr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/str_repr/missing_coords_cube.str.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/str_repr/multi_dim_coord.__repr__.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/str_repr/multi_dim_coord.__str__.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/str_repr/similar.__str__.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/str_repr/simple.__str__.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/str_repr/unicode_attribute.__unicode__.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/test_simple_cube_intersection.cml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/compatible_cubes.str.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.864774 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2x2d.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_bounds.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_y.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_y_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_xy_bounds.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_y.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_y_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2y2d.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_x.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_x_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_x_y.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_x_y_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_y.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_y_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_3d_simple.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_4mix2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_4x2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_4y2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_9mix2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_9x2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_9y2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_anonymous.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_masked_2x2d.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_masked_2y2d.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_merged_scalar_4mix2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_merged_scalar_4x2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_merged_scalar_4y2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_pre_merged_scalar_4mix2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_pre_merged_scalar_4x2_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_pre_merged_scalar_4y2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_scalar_4mix2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_scalar_4x2d_aux_xy.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_scalar_4y2d_aux_xy.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.864774 scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/
+-rw-r--r--   0 runner    (1001) docker     (127)    10348 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/all_10_load_match.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    10878 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/all_ml_10_22_load_match.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/attribute_constraint.cml
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/invalid_inequality_load_match.cml
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/pressure_950_load_match.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_10_and_theta_level_gt_30_le_3_load_match.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_10_and_theta_level_gt_30_le_3_load_strict.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_10_load_match.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_10_load_strict.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    16305 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_and_all_10_load_match.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_and_theta_10_load_strict.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_and_theta_load_match.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_and_theta_load_strict.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_gt_30_le_3_load_match.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_gt_30_le_3_load_strict.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_lat_30_load_match.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_lat_30_load_strict.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_lat_gt_30_load_match.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_lat_gt_30_load_strict.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_load_match.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_load_strict.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.868775 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/complex.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.868775 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/coord_maths/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/coord_maths/add_float_expl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/coord_maths/add_simple_expl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/coord_maths/divide_simple_expl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/coord_maths/mult_float_expl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/coord_maths/multiply_simple_expl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/coord_maths/negate_expl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/coord_maths/r_subtract_simple_exl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/coord_maths/right_divide_simple_expl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/coord_maths/subtract_simple_expl.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/intersection.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/intersection_missing.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/intersection_reversed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/minimal.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/nd_bounds.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.868775 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/str_repr/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/str_repr/aux_nontime_repr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/str_repr/aux_nontime_str.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/str_repr/aux_time_repr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/str_repr/aux_time_str.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/str_repr/dim_nontime_repr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/str_repr/dim_nontime_str.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/str_repr/dim_time_repr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/str_repr/dim_time_str.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.872774 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_systems/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_systems/CoordSystem_xml_element.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_systems/GeogCS_init_no_invf.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_systems/GeogCS_init_no_major.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_systems/GeogCS_init_no_minor.xml
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_systems/GeogCS_init_sphere.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_systems/Mercator.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_systems/PolarStereographic.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_systems/PolarStereographicScaleFactor.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_systems/PolarStereographicStandardParallel.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_systems/RotatedGeogCS_init.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_systems/RotatedGeogCS_init_a.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_systems/RotatedGeogCS_init_b.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_systems/Stereographic.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_systems/TransverseMercator_osgb.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.880774 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/
+-rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/latitude_longitude_dual_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/latitude_longitude_dual_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/latitude_longitude_single_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/latitude_longitude_single_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/latitude_model_level_number_dual_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/latitude_model_level_number_dual_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/latitude_model_level_number_single_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/latitude_model_level_number_single_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/latitude_time_dual_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/latitude_time_dual_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/latitude_time_single_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/latitude_time_single_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/longitude_latitude_dual_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/longitude_latitude_dual_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/longitude_latitude_single_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/longitude_latitude_single_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/longitude_model_level_number_dual_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/longitude_model_level_number_dual_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/longitude_model_level_number_single_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/longitude_model_level_number_single_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/longitude_time_dual_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/longitude_time_dual_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/longitude_time_single_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/longitude_time_single_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_latitude_dual_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_latitude_dual_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_latitude_single_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_latitude_single_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_longitude_dual_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_longitude_dual_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_longitude_single_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_longitude_single_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_time_dual_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_time_dual_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_time_single_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_time_single_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/original.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/time_latitude_dual_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/time_latitude_dual_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/time_latitude_single_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/time_latitude_single_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/time_longitude_dual_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/time_longitude_dual_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/time_longitude_single_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/time_longitude_single_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/time_model_level_number_dual_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/time_model_level_number_dual_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/time_model_level_number_single_stage.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/time_model_level_number_single_stage.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/triple_collapse_lat_ml_pt.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/triple_collapse_lat_ml_pt.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/triple_collapse_ml_pt_lon.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/triple_collapse_ml_pt_lon.data.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.724774 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_io/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.880774 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_io/pickling/
+-rw-r--r--   0 runner    (1001) docker     (127)    19671 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_io/pickling/cubelist.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    17363 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_io/pickling/single_cube.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_io/pickling/theta.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.724774 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_io/pp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.880774 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_io/pp/load/
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_io/pp/load/global.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.880774 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_merge/
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_merge/multidim_coord_merge.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_merge/multidim_coord_merge_transpose.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_merge/test_orig_point_cube.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_merge/test_simple_attributes1.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_merge/test_simple_attributes2.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_merge/test_simple_attributes3.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_merge/test_simple_bound_merge.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_merge/test_simple_merge.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.884775 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/2d_intersect_and_reverse.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/2d_orig.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/2d_to_0d_cube_slice.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/2d_to_1d_cube_multi_slice.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/2d_to_1d_cube_multi_slice2.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/2d_to_1d_cube_multi_slice3.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/2d_to_1d_cube_slice.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/2d_to_2d_revesed.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/2d_transposed.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/real_data_dual_tuple_indexing1.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/real_data_dual_tuple_indexing2.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/real_data_dual_tuple_indexing3.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/real_empty_data_indexing.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.884775 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/
+-rw-r--r--   0 runner    (1001) docker     (127)    17000 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/append_multi.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/append_single.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/default_coord_system.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/depth.latitude.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/depth.time.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/eta.latitude.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/no_forecast_period.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/no_forecast_period.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/no_forecast_time.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/no_forecast_time.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/pressure.latitude.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/pressure.time.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/replace_multi.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/replace_single.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/simple.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.884775 scitools-iris-3.9.0rc0/lib/iris/tests/results/derived/
+-rw-r--r--   0 runner    (1001) docker     (127)     6448 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/derived/column.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/derived/no_orog.__str__.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/derived/no_orog.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/derived/removed_derived_coord.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/derived/removed_orog.__str__.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/derived/removed_orog.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/derived/removed_sigma.__str__.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16859 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/derived/removed_sigma.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/derived/transposed.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.724774 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.724774 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/analysis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.724774 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/analysis/interpolate/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.888774 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/basic_orthogonal_cube.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/basic_orthogonal_cube.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_1d_squashed.cml
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_1d_squashed.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_1d_squashed_2.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_with_factory.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.724774 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/regrid/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.888774 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/const_lat_cross_section.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/const_lat_cross_section.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/const_lon_cross_section.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/const_lon_cross_section.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/higher.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/higher.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/hybridheight.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/hybridheight.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/latlonreduced.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/latlonreduced.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/lonhalved.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/lonhalved.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/lower.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/lower.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/simple.cml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/simple.data.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.892774 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/ugrid/
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/ugrid/2D_1t_face_half_levels.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/ugrid/2D_72t_face_half_levels.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/ugrid/3D_1t_face_full_levels.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/ugrid/3D_1t_face_half_levels.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/ugrid/3D_snow_pseudo_levels.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/ugrid/3D_soil_pseudo_levels.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/ugrid/3D_tile_pseudo_levels.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/ugrid/3D_veg_pseudo_levels.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    50900 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/ugrid/surface_mean.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.892774 scitools-iris-3.9.0rc0/lib/iris/tests/results/file_load/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/file_load/known_loaders.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    97746 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/file_load/theta_levels.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    97417 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/file_load/u_wind_levels.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    97417 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/file_load/v_wind_levels.cml
+-rw-r--r--   0 runner    (1001) docker     (127)   194764 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/file_load/wind_levels.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    31710 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/imagerepo.json
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/incompatible_attr.str.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/incompatible_cubes.str.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/incompatible_meth.str.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/incompatible_name.str.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/incompatible_unit.str.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.724774 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.724774 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/climatology/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.892774 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/climatology/TestClimatology/
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/climatology/TestClimatology/reference_simpledata.cdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.724774 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/experimental/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.724774 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/experimental/ugrid_save/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.892774 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex1_1d_mesh.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex2_2d_triangular.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex3_2d_flexible.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex4_3d_layered.cdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.724774 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.724774 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/attributes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.892774 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/attributes/TestUmVersionAttribute/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/attributes/TestUmVersionAttribute/multiple_different_saves_on_variables.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/attributes/TestUmVersionAttribute/multiple_same_saves_as_global.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/attributes/TestUmVersionAttribute/single_saves_as_global.cdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.724774 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/aux_factories/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.892774 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/aux_factories/TestAtmosphereSigma/
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/aux_factories/TestAtmosphereSigma/save.cdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.892774 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/aux_factories/TestHybridPressure/
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/aux_factories/TestHybridPressure/save.cdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.892774 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/aux_factories/TestSaveMultipleAuxFactories/
+-rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/aux_factories/TestSaveMultipleAuxFactories/hybrid_height_and_pressure.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/aux_factories/TestSaveMultipleAuxFactories/hybrid_height_cubes.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.724774 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/general/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.892774 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/general/TestDatasetAndPathSaves/
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/general/TestDatasetAndPathSaves/basic_save.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/general/TestDatasetAndPathSaves/path_string_save_same.cdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.896775 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/multi_packed_multi_dtype.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/multi_packed_single_dtype.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/single_packed_manual.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/single_packed_signed.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/single_packed_unsigned.cdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.724774 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/um/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.724774 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/um/fieldsfile/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.896775 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/um/fieldsfile/TestStructuredLoadFF/
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/um/fieldsfile/TestStructuredLoadFF/simple.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/um/fieldsfile/TestStructuredLoadFF/simple_callback.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.896775 scitools-iris-3.9.0rc0/lib/iris/tests/results/iterate/
+-rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/iterate/izip_nd_ortho.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.900775 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/a_aux_b_aux.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/a_aux_b_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/a_dim_b_aux.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/a_dim_b_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    24030 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/dec.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/multi_split.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/separable_combination.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/single_split.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/string_a_b.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/string_a_with_aux.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/string_a_with_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/string_b_with_aux.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/string_b_with_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/theta.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    17223 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/theta_two_times.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_duplicate_data.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_independent.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_merging1.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_merging2.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_merging3.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_merging4.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_merging5.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_non_expanding.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_series.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_single_forecast.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_successive_forecasts.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_time_non_dim_coord.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_time_vs_forecast.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_time_vs_ref_time.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.904775 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/
+-rw-r--r--   0 runner    (1001) docker     (127)    14642 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEIII_field.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEIII_field.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEIII_field.data.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEIII_field.data.2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEIII_field.data.3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEIII_field.data.4.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18200 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEIII_timeseries.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEIII_timeseries.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEIII_timeseries.data.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEIII_timeseries.data.2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEIII_timeseries.data.3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEIII_timeseries.data.4.json
+-rw-r--r--   0 runner    (1001) docker     (127)    49155 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEIII_trajectory.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEIII_trajectory0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    13751 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEIII_version2.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEIII_version2.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEIII_version2.data.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEIII_version2.data.2.json
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEIII_version2.data.3.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14006 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEII_field.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEII_field.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEII_field.data.1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEII_field.data.2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEII_field.data.3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEII_field.data.4.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEII_field__no_time_averaging.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEII_field__no_time_averaging_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEII_timeseries.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEII_timeseries.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEII_timeseries.data.1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.912775 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.912775 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/aliases.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/flag.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/fulldims.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/multiple.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/partialdims.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/shared.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/int64_auxiliary_coord_netcdf3.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/int64_data_netcdf3.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/int64_dimension_coord_netcdf3.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/multi_dim_coord_slightly_different.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)    24811 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_cell_methods.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_index_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_index_1.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_index_2.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_mix_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_mix_1.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_slice_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_slice_1.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_slice_2.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_tuple_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_tuple_1.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_tuple_2.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_global_xyt_hires.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_global_xyt_total.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_global_xyzt_gems.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_global_xyzt_gems_iter_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_global_xyzt_gems_iter_1.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_laea.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_lcc.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_merc.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_merc_false.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_merc_scale_factor.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_monotonic.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_polar.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_rotated_xy_land.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_rotated_xyt_precipitation.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_conf_aux.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_conf_name.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_confl_attr.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_confl_global_attr.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_gridmapmulti.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_hybrid_height.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)    17318 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_load_hybrid_height.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_load_ndim_auxiliary.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_multi_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_multi_1.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_multi_2.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_multiple.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_ndim_auxiliary.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_no_global_attr.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_no_name.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_nocoord.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_realistic_0d.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_realistic_4d.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_realistic_4d_no_hybrid.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_samedimcoord.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_samevar.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_single.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_wcoord.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_stereo.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_tmerc_and_climatology.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_units_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_units_1.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/save_load_traj.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/uint32_auxiliary_coord_netcdf3.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/uint32_data_netcdf3.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/uint32_dimension_coord_netcdf3.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.920775 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/levels_below_ground.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/load_2flds.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/mockography.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/period_of_interest.cml
+-rw-r--r--   0 runner    (1001) docker     (127)   115358 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/probability_fields.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_bmr04_precip_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_bsr05_precip_accum60_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_cloud3d0060_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    18157 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_cloud_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    23363 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_convection_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    16563 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_convwind_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    20032 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_frzlev_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_height_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_precip_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_precipaccum_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    22519 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_preciptype_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_pressure_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    17256 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_radiation_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     7563 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_radiationuv_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_refl_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_relhumidity3d0060_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_relhumidity_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_snow_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    11254 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_soil3d0060_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     8069 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_soil_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    11199 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_temperature_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    13697 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_visibility_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    16661 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_wind_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5492 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_winduv3d0015_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_winduv_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    15065 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek01_cape_2km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek07_precip0540_accum180_18km.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_umqv_fog_2km.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.728774 scitools-iris-3.9.0rc0/lib/iris/tests/results/pandas/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.920775 scitools-iris-3.9.0rc0/lib/iris/tests/results/pandas/as_cube/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/pandas/as_cube/data_frame_datetime_standard.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/pandas/as_cube/data_frame_masked.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/pandas/as_cube/data_frame_multidim.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/pandas/as_cube/data_frame_netcdftime_360.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/pandas/as_cube/data_frame_nonotonic.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/pandas/as_cube/data_frame_simple.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/pandas/as_cube/series_datetime_standard.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/pandas/as_cube/series_masked.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/pandas/as_cube/series_netcdfimte_360.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/pandas/as_cube/series_object.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/pandas/as_cube/series_simple.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.920775 scitools-iris-3.9.0rc0/lib/iris/tests/results/pp_load_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/pp_load_rules/global.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/pp_load_rules/lbproc_mean_max_min.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/pp_load_rules/lbtim_2.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/pp_load_rules/ocean_depth.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/pp_load_rules/ocean_depth_bounded.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/pp_load_rules/rotated_uk.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.920775 scitools-iris-3.9.0rc0/lib/iris/tests/results/stock/
+-rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/stock/realistic_4d.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.920775 scitools-iris-3.9.0rc0/lib/iris/tests/results/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/system/supported_filetype_.nc.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/system/supported_filetype_.pp.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.924775 scitools-iris-3.9.0rc0/lib/iris/tests/results/trajectory/
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/trajectory/constant_latitude.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     4753 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/trajectory/hybrid_height.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/trajectory/single_point.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/trajectory/tri_polar_latitude_slice.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/trajectory/zigzag.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.732774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.728774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.728774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/cartography/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.728774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/cartography/project/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.924775 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/cartography/project/TestAll/
+-rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/cartography/project/TestAll/cube.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/cartography/project/TestAll/cube.data.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.728774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.728774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.924775 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/
+-rw-r--r--   0 runner    (1001) docker     (127)    16599 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_all_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    16599 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_last_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    16599 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_middle_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    16599 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_zeroth_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    16599 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/slice.cml
+-rw-r--r--   0 runner    (1001) docker     (127)    16599 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/transposed.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.728774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.924775 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_all_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_last_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_middle_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_zeroth_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/slice.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/transposed.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.924775 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_all_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_last_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_middle_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_zeroth_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/slice.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/transposed.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.728774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/add/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.928775 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_all_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_last_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_middle_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_zeroth_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/slice.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/transposed.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.728774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.928775 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_all_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_last_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_middle_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_zeroth_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/slice.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/transposed.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.728774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.928775 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/
+-rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_all_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_last_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_middle_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_zeroth_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/slice.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/transposed.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.728774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.928775 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_all_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_last_dims.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_middle_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_zeroth_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/slice.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/transposed.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.728774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/cube/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.728774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/cube/Cube/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.932775 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/metadata.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/metadata.data.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/metadata_wrapped.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/metadata_wrapped.data.0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.932775 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/cube/Cube/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/cube/Cube/xml/ancils.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/cube/Cube/xml/cell_measures.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/cube/Cube/xml/checksum_ignores_masked_values.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.728774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/cube/CubeList/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.932775 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/combination_with_extra_realization.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/combination_with_extra_triple.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/combination_with_realization.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/orthogonal_with_realization.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.732774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/experimental/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.732774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/experimental/representation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.732774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.932775 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content/mesh_result.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.932775 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content__string_attrs/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content__string_attrs/embedded_newlines_string_attribute.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content__string_attrs/long_string_attribute.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content__string_attrs/multi_string_attribute.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content__string_attrs/simple_string_attribute.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.732774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/experimental/stratify/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.732774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/experimental/stratify/relevel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.932775 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/experimental/stratify/relevel/Test/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/experimental/stratify/relevel/Test/multi_dim_target_levels.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.732774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/fileformats/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.732774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.732774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.732774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.932775 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/endian.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/mercator.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/mercator_no_ellipsoid.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/stereographic.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/stereographic_no_ellipsoid.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/stereographic_scale_factor.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/transverse_mercator.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/transverse_mercator_no_ellipsoid.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/with_climatology.cdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.732774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver__ugrid/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.932775 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver__ugrid/TestSaveUgrid__cube/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver__ugrid/TestSaveUgrid__cube/basic_mesh.cdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.732774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/merge/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.732774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/merge/ProtoCube/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.932775 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/merge/ProtoCube/register__CoordSig_general/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/merge/ProtoCube/register__CoordSig_general/noise.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.936775 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/merge/ProtoCube/register__CubeSig/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/merge/ProtoCube/register__CubeSig/noise.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.732774 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/util/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.936775 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/util/describe_diff/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/util/describe_diff/incompatible_array_attrs.str.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.936775 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/util/mask_cube/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.936775 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/util/mask_cube/TestCubeMask/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/util/mask_cube/TestCubeMask/mask_cube_2d_create_new_dim.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/util/mask_cube/original_cube_full2d_global.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/util/mask_cube/original_cube_simple_1d.cml
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/util/mask_cube/original_cube_simple_2d.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.936775 scitools-iris-3.9.0rc0/lib/iris/tests/results/uri_callback/
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/uri_callback/pp_global.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.732774 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.732774 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.940775 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.03.236.000128.1990.12.01.00.00.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.03.236.004224.1990.12.01.00.00.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.03.236.008320.1990.12.01.00.00.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.16.202.000128.1860.09.01.00.00.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/001000000000.00.000.000000.1860.01.01.00.00.f.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/002000000000.44.101.131200.1920.09.01.00.00.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/008000000000.44.101.000128.1890.09.01.00.00.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/12187.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/HadCM2_ts_SAT_ann_18602100.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_level_lat_orig.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_lon_lat_press_orig.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_lon_lat_several.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_n10r13xy.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_time_press.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_tseries.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abcza_pa19591997_daily_29.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abcza_pa19591997_daily_29.b_1.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abcza_pa19591997_daily_29.b_2.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abxpa_press_lat.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/integer.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/model.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/ocean_xsect.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/st0fc699.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/st0fc942.b_0.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/st30211.b_0.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.944775 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.03.236.000128.1990.12.01.00.00.b.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.03.236.004224.1990.12.01.00.00.b.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.03.236.008320.1990.12.01.00.00.b.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.16.202.000128.1860.09.01.00.00.b.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/001000000000.00.000.000000.1860.01.01.00.00.f.b.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/002000000000.44.101.131200.1920.09.01.00.00.b.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/008000000000.44.101.000128.1890.09.01.00.00.b.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     6053 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/12187.b.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/HadCM2_ts_SAT_ann_18602100.b.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_level_lat_orig.b.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_lon_lat_press_orig.b.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_lon_lat_several.b.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_n10r13xy.b.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_time_press.b.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_tseries.b.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/abcza_pa19591997_daily_29.b.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/abxpa_press_lat.b.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/integer.b.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/model.b.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/ocean_xsect.b.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/st0fc699.b.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/st0fc942.b.cml
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/st30211.b.cml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.944775 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.03.236.000128.1990.12.01.00.00.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.03.236.004224.1990.12.01.00.00.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.03.236.008320.1990.12.01.00.00.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.16.202.000128.1860.09.01.00.00.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/001000000000.00.000.000000.1860.01.01.00.00.f.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/002000000000.44.101.131200.1920.09.01.00.00.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/008000000000.44.101.000128.1890.09.01.00.00.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/12187.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/HadCM2_ts_SAT_ann_18602100.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_level_lat_orig.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_lon_lat_press_orig.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_lon_lat_several.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_n10r13xy.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_time_press.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_tseries.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abcza_pa19591997_daily_29.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abcza_pa19591997_daily_29.b_1.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abcza_pa19591997_daily_29.b_2.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abxpa_press_lat.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/integer.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/model.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/ocean_xsect.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/st0fc699.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/st0fc942.b_0.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/st30211.b_0.cdl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.948775 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.03.236.000128.1990.12.01.00.00.b.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.03.236.004224.1990.12.01.00.00.b.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.03.236.008320.1990.12.01.00.00.b.pp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.16.202.000128.1860.09.01.00.00.b.pp.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.948775 scitools-iris-3.9.0rc0/lib/iris/tests/stock/
+-rw-r--r--   0 runner    (1001) docker     (127)    24891 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/stock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15181 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/stock/_stock_2d_latlons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.948775 scitools-iris-3.9.0rc0/lib/iris/tests/stock/file_headers/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/stock/file_headers/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/stock/file_headers/minimal_bad_mesh_cf_role.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/stock/file_headers/minimal_bad_topology_dim.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/stock/file_headers/xios_2D_face_half_levels.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/stock/file_headers/xios_3D_face_full_levels.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/stock/file_headers/xios_3D_face_half_levels.cdl
+-rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/stock/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/stock/netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/system_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_abf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49574 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_aggregate_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66121 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29178 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_analysis_calculus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32587 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_basic_maths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_cartography.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50846 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_cdm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9754 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15735 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10437 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_coding_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41997 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26671 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34864 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_coord_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18549 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_coordsystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14064 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_cube_to_pp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_ff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_file_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_file_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_image_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_intersect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5622 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_io_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23755 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_iterate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_lazy_aggregate_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41844 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53585 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_nimrod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9623 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_peak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_pickling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36173 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_pp_cf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15490 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_pp_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_pp_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8763 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_pp_to_cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9577 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_quickplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_std_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_uri_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.948775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.952775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.952775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/area_weighted/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/area_weighted/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/area_weighted/test_AreaWeightedRegridder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.952775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/cartography/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/cartography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/cartography/test__get_lon_lat_coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/cartography/test__quadrant_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/cartography/test__xy_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/cartography/test_area_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12942 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/cartography/test_gridcell_angles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/cartography/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/cartography/test_rotate_grid_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22434 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/cartography/test_rotate_winds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.952775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/geometry/test__extract_relevant_cube_slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/geometry/test_geometry_area_weights.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.956775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/interpolation/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/interpolation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22315 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/interpolation/test_RectilinearInterpolator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/interpolation/test_get_xy_dim_coords.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.956775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/maths/
+-rw-r--r--   0 runner    (1001) docker     (127)    12786 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/maths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/maths/test__arith__dask_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/maths/test__arith__derived_coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/maths/test__arith__meshcoords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/maths/test__get_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/maths/test__inplace_common_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8037 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/maths/test__output_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/maths/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/maths/test_divide.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/maths/test_multiply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/maths/test_subtract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.956775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/regrid/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/regrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54848 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/regrid/test_RectilinearRegridder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14597 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/regrid/test__CurvilinearRegridder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.956775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/scipy_interpolate/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/scipy_interpolate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/scipy_interpolate/test__RegularGridInterpolator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.956775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8354 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/stats/test_pearsonr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15006 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_Aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_AreaWeighted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_COUNT.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_Linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_MAX.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_MAX_RUN.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_MEAN.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_MIN.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_Nearest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14272 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_PERCENTILE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_PROPORTION.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_PercentileAggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_PointInCell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_RMS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_STD_DEV.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_SUM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_VARIANCE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_WPERCENTILE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_WeightedPercentileAggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test__axis_to_single_trailing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.956775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/trajectory/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/trajectory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/trajectory/test_Trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/trajectory/test_UnstructuredNearestNeighbourRegridder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/trajectory/test__nearest_neighbour_indices_ndcoords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14365 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/trajectory/test_interpolate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.960775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/aux_factory/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/aux_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10247 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/aux_factory/test_AtmosphereSigmaFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/aux_factory/test_AuxCoordFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11594 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/aux_factory/test_HybridPressureFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10821 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/aux_factory/test_OceanSFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/aux_factory/test_OceanSg1Factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9980 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/aux_factory/test_OceanSg2Factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/aux_factory/test_OceanSigmaFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16785 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/aux_factory/test_OceanSigmaZFactory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.960775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.960775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/lenient/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/lenient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/lenient/test_Lenient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27226 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/lenient/test__Lenient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/lenient/test__lenient_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/lenient/test__lenient_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/lenient/test__qualname.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.964775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17596 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/metadata/test_AncillaryVariableMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57427 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/metadata/test_BaseMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24164 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/metadata/test_CellMeasureMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25452 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/metadata/test_CoordMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42695 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/metadata/test_CubeMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/metadata/test__NamedTupleMeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/metadata/test_hexdigest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/metadata/test_metadata_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/metadata/test_metadata_manager_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.964775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/mixin/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12829 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/mixin/test_CFVariableMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/mixin/test_LimitedAttributeDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/mixin/test__get_valid_standard_name.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.964775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/resolve/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/resolve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   190389 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/resolve/test_Resolve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.964775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/concatenate/
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/concatenate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/concatenate/test__CoordMetaData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/concatenate/test__CoordSignature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/concatenate/test__CubeSignature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16193 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/concatenate/test_concatenate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.964775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/config/test_NetCDF.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.964775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8498 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/constraints/test_Constraint_equality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/constraints/test_NameConstraint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.964775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_categorisation/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_categorisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_categorisation/test_add_categorised_coord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_categorisation/test_add_hour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8114 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_categorisation/test_coord_categorisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.968775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_AlbersEqualArea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_GeogCS.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_Geostationary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_LambertAzimuthalEqualArea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_LambertConformal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7540 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_Mercator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_ObliqueMercator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_Orthographic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_PolarStereographic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_RotatedMercator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_RotatedPole.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_Stereographic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_TransverseMercator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_VerticalPerspective.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.968775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coords/
+-rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coords/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26049 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coords/test_AncillaryVariable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29422 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coords/test_AuxCoord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9244 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coords/test_Cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coords/test_CellMeasure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coords/test_CellMethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43553 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coords/test_Coord.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22247 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coords/test_DimCoord.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37979 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/coords/test__DimensionalMetadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.972775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/cube/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/cube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   133812 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/cube/test_Cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15580 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/cube/test_CubeAttrsDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26077 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/cube/test_CubeList.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31206 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/cube/test_Cube__aggregated_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/cube/test_Cube__operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.972775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/data_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/data_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21578 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/data_manager/test_DataManager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.972775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.972775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/geovista/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/geovista/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/geovista/test_cube_to_polydata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/geovista/test_extract_unstructured_region.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.972775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/raster/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/raster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/raster/test_export_geotiff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.972775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/regrid/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/regrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/regrid/test_regrid_area_weighted_rectilinear_src_and_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13938 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/regrid/test_regrid_weighted_curvilinear_to_rectilinear.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.972775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/representation/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/representation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/representation/test_CubeListRepresentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17300 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/representation/test_CubeRepresentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.972775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/stratify/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/stratify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/stratify/test_relevel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.972775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.972775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/cf/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/cf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridAuxiliaryCoordinateVariable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8254 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridConnectivityVariable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10008 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridMeshVariable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridReader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.976775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/load/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/load/test_ParseUgridOnLoad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/load/test_load_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7747 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/load/test_load_meshes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.976775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12646 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/mesh/test_Connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48842 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/mesh/test_Mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37097 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/mesh/test_MeshCoord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/mesh/test_Mesh__from_coords.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.976775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27719 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/metadata/test_ConnectivityMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25591 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/metadata/test_MeshCoordMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28317 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/metadata/test_MeshMetadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.976775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18413 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/utils/test_recombine_submeshes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.976775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.976775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/abf/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/abf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/abf/test_ABFField.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.976775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/cf/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/cf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/cf/test_CFGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14723 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/cf/test_CFReader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.976775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/dot/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/dot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/dot/test__dot_path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.980775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/ff/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/ff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/ff/test_ArakawaC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/ff/test_ENDGame.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19381 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/ff/test_FF2PP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/ff/test_FFHeader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/ff/test_Grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/ff/test_NewDynamics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.980775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/name_loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/name_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/name_loaders/test__build_cell_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/name_loaders/test__build_lat_lon_for_NAME_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/name_loaders/test__calc_integration_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/name_loaders/test__cf_height_from_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/name_loaders/test__generate_cubes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.980775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.980775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)     5996 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35919 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__grid_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11753 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__hybrid_formulae.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12070 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__latlon_dimcoords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__miscellaneous.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17201 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__time_coords.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.980775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/engine/test_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.984775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test__normalise_bounds_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_albers_equal_area_coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_ancil_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13185 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_auxiliary_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_cell_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4147 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_cube_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20525 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_dimension_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_geostationary_coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_lambert_azimuthal_equal_area_coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_lambert_conformal_coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_mercator_coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_oblique_mercator_coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_polar_stereographic_coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_stereographic_coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_transverse_mercator_coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_verticalp_coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_get_attr_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_get_cf_bounds_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11376 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_get_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_has_supported_mercator_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_has_supported_polar_stereographic_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_parse_cell_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_reorder_bounds_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.984775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.984775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/loader/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/loader/test__chunk_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/loader/test__get_cf_var_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/loader/test__load_aux_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/loader/test__load_cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/loader/test__translate_constraints_to_var_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11463 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/loader/test_load_cubes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.988775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39213 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver__lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver__lazy_stream_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48377 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver__ugrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18106 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/test_save.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.988775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nimrod_load_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nimrod_load_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nimrod_load_rules/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nimrod_load_rules/test_vertical_coord.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.988775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp/test_PPDataProxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12723 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp/test_PPField.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp/test__convert_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp/test__create_field_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7117 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp/test__data_bytes_to_shaped_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp/test__field_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp/test__interpret_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp/test_as_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp/test_save_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp/test_save_pairs_from_cube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.992775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__all_other_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__collapse_degenerate_points_and_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_scalar_pseudo_level_coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_scalar_realization_coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24943 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_time_coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23086 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_vertical_coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__dim_or_aux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__epoch_date_hours.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__model_level_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__reduced_points_and_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__reshape_vector_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13641 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.992775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/rules/test_Loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/rules/test__make_cube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.992775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/structured_array_identification/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/structured_array_identification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/structured_array_identification/test_ArrayStructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/structured_array_identification/test_GroupStructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/test_rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.992775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/um/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/um/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.992775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/um/fast_load/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/um/fast_load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/um/fast_load/test_FieldCollation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/um/fast_load/test__convert_collation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.992775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/um/fast_load_structured_fields/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/um/fast_load_structured_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/um/fast_load_structured_fields/test_BasicFieldCollation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/um/fast_load_structured_fields/test_group_structured_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.992775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/um/optimal_array_structuring/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/um/optimal_array_structuring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9395 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/um/optimal_array_structuring/test_optimal_array_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/um/test_um_to_pp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.996775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/io/test__generate_cubes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/io/test_expand_filespecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/io/test_run_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/io/test_save.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.996775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/lazy_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/lazy_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/lazy_data/test_as_concrete_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7382 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/lazy_data/test_as_lazy_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/lazy_data/test_co_realise_cubes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/lazy_data/test_is_lazy_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/lazy_data/test_is_lazy_masked_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/lazy_data/test_lazy_elementwise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/lazy_data/test_map_complete_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/lazy_data/test_multidim_lazy_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/lazy_data/test_non_lazy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.996775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/merge/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16831 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/merge/test_ProtoCube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:15.996775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47771 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/pandas/test_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:16.000775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/_blockplot_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test__check_bounds_contiguity_and_mask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test__check_geostationary_coords_and_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test__fixup_dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test__get_plot_defn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test__get_plot_defn_custom_coords_picked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test__get_plot_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test__replace_axes_with_cartopy_axes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test_contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test_contourf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test_hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test_outline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test_pcolor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test_pcolormesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test_scatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:16.000775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/quickplot/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/quickplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/quickplot/test_contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/quickplot/test_contourf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/quickplot/test_outline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/quickplot/test_pcolor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/quickplot/test_pcolormesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/quickplot/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/quickplot/test_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/quickplot/test_scatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:16.000775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/representation/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/representation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:16.000775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/representation/cube_printout/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/representation/cube_printout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22090 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/representation/cube_printout/test_CubePrintout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/representation/cube_printout/test_Table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:16.000775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/representation/cube_summary/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/representation/cube_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/representation/cube_summary/test_CubeSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/test_Future.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/test_sample_data_path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:16.000775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:16.000775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/tests/stock/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/tests/stock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/tests/stock/test_netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/tests/test_IrisTest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:16.000775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/time/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/time/test_PartialDateTime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:16.004775 scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test__coord_regular.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test__is_circular.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test__mask_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15236 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test__slice_data_with_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_array_equal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_broadcast_to_shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_column_slices_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_demote_dim_coord_to_aux_coord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_describe_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9500 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_equalise_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_file_is_newer_than.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_find_discontiguities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_guess_coord_axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_mask_cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_mask_cube_from_shapefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12248 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_new_axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_promote_aux_coord_to_dim_coord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7232 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4302 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_rolling_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_squeeze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_unify_time_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74435 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/lib/iris/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:16.008775 scitools-iris-3.9.0rc0/lib/scitools_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9278 2024-04-03 11:05:15.000000 scitools-iris-3.9.0rc0/lib/scitools_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    96854 2024-04-03 11:05:15.000000 scitools-iris-3.9.0rc0/lib/scitools_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 11:05:15.000000 scitools-iris-3.9.0rc0/lib/scitools_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 11:05:14.000000 scitools-iris-3.9.0rc0/lib/scitools_iris.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-03 11:05:15.000000 scitools-iris-3.9.0rc0/lib/scitools_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 11:05:15.000000 scitools-iris-3.9.0rc0/lib/scitools_iris.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:16.008775 scitools-iris-3.9.0rc0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/requirements/pypi-core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 11:05:16.008775 scitools-iris-3.9.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:16.008775 scitools-iris-3.9.0rc0/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-03 11:05:08.000000 scitools-iris-3.9.0rc0/tools/generate_std_names.py
```

### Comparing `scitools_iris-3.9.0/CITATION.cff` & `scitools-iris-3.9.0rc0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/LICENSE` & `scitools-iris-3.9.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/MANIFEST.in` & `scitools-iris-3.9.0rc0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/PKG-INFO` & `scitools-iris-3.9.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scitools-iris
-Version: 3.9.0
+Version: 3.9.0rc0
 Summary: A powerful, format-agnostic, community-driven Python package for analysing and visualising Earth science data
 Author-email: Iris Contributors <scitools.pub@gmail.com>
 License: BSD-3-Clause
 Project-URL: Code, https://github.com/SciTools/iris
 Project-URL: Discussions, https://github.com/SciTools/iris/discussions
 Project-URL: Documentation, https://scitools-iris.readthedocs.io/en/stable/
 Project-URL: Issues, https://github.com/SciTools/iris/issues
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: scitools-iris Version: 3.9.0 Summary: A powerful,
-format-agnostic, community-driven Python package for analysing and visualising
-Earth science data Author-email: Iris Contributors
+Metadata-Version: 2.1 Name: scitools-iris Version: 3.9.0rc0 Summary: A
+powerful, format-agnostic, community-driven Python package for analysing and
+visualising Earth science data Author-email: Iris Contributors
 gmail.com> License: BSD-3-Clause Project-URL: Code, https://github.com/
 SciTools/iris Project-URL: Discussions, https://github.com/SciTools/iris/
 discussions Project-URL: Documentation, https://scitools-iris.readthedocs.io/
 en/stable/ Project-URL: Issues, https://github.com/SciTools/iris/issues
 Keywords: cf-metadata,data-analysis,earth-
 science,grib,netcdf,meteorology,oceanography,space-weather,ugrid,visualisation
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
```

### Comparing `scitools_iris-3.9.0/README.md` & `scitools-iris-3.9.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/etc/cf-standard-name-table.xml` & `scitools-iris-3.9.0rc0/etc/cf-standard-name-table.xml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/__init__.py` & `scitools-iris-3.9.0rc0/lib/iris/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/_concatenate.py` & `scitools-iris-3.9.0rc0/lib/iris/_concatenate.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/_constraints.py` & `scitools-iris-3.9.0rc0/lib/iris/_constraints.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/_data_manager.py` & `scitools-iris-3.9.0rc0/lib/iris/_data_manager.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/_deprecation.py` & `scitools-iris-3.9.0rc0/lib/iris/_deprecation.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/_lazy_data.py` & `scitools-iris-3.9.0rc0/lib/iris/_lazy_data.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/_merge.py` & `scitools-iris-3.9.0rc0/lib/iris/_merge.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/_representation/cube_printout.py` & `scitools-iris-3.9.0rc0/lib/iris/_representation/cube_printout.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/_representation/cube_summary.py` & `scitools-iris-3.9.0rc0/lib/iris/_representation/cube_summary.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/_shapefiles.py` & `scitools-iris-3.9.0rc0/lib/iris/_shapefiles.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/analysis/__init__.py` & `scitools-iris-3.9.0rc0/lib/iris/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/analysis/_area_weighted.py` & `scitools-iris-3.9.0rc0/lib/iris/analysis/_area_weighted.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/analysis/_grid_angles.py` & `scitools-iris-3.9.0rc0/lib/iris/analysis/_grid_angles.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/analysis/_interpolation.py` & `scitools-iris-3.9.0rc0/lib/iris/analysis/_interpolation.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/analysis/_regrid.py` & `scitools-iris-3.9.0rc0/lib/iris/analysis/_regrid.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/analysis/_scipy_interpolate.py` & `scitools-iris-3.9.0rc0/lib/iris/analysis/_scipy_interpolate.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/analysis/calculus.py` & `scitools-iris-3.9.0rc0/lib/iris/analysis/calculus.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/analysis/cartography.py` & `scitools-iris-3.9.0rc0/lib/iris/analysis/cartography.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/analysis/geometry.py` & `scitools-iris-3.9.0rc0/lib/iris/analysis/geometry.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/analysis/maths.py` & `scitools-iris-3.9.0rc0/lib/iris/analysis/maths.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/analysis/stats.py` & `scitools-iris-3.9.0rc0/lib/iris/analysis/stats.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/analysis/trajectory.py` & `scitools-iris-3.9.0rc0/lib/iris/analysis/trajectory.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/aux_factory.py` & `scitools-iris-3.9.0rc0/lib/iris/aux_factory.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/common/_split_attribute_dicts.py` & `scitools-iris-3.9.0rc0/lib/iris/common/_split_attribute_dicts.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/common/lenient.py` & `scitools-iris-3.9.0rc0/lib/iris/common/lenient.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/common/metadata.py` & `scitools-iris-3.9.0rc0/lib/iris/common/metadata.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/common/mixin.py` & `scitools-iris-3.9.0rc0/lib/iris/common/mixin.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/common/resolve.py` & `scitools-iris-3.9.0rc0/lib/iris/common/resolve.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/config.py` & `scitools-iris-3.9.0rc0/lib/iris/config.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/coord_categorisation.py` & `scitools-iris-3.9.0rc0/lib/iris/coord_categorisation.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/coord_systems.py` & `scitools-iris-3.9.0rc0/lib/iris/coord_systems.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/coords.py` & `scitools-iris-3.9.0rc0/lib/iris/coords.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/cube.py` & `scitools-iris-3.9.0rc0/lib/iris/cube.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/diverging/BrBG_11.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/diverging/BrBG_11.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/diverging/PRGn_11.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/diverging/PRGn_11.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/diverging/PiYG_11.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/diverging/PiYG_11.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/diverging/PuOr_11.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/diverging/PuOr_11.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/diverging/RdBu_11.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/diverging/RdBu_11.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/diverging/RdGy_11.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/diverging/RdGy_11.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/diverging/RdYlBu_11.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/diverging/RdYlBu_11.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/diverging/RdYlGn_11.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/diverging/RdYlGn_11.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/diverging/Spectral_11.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/diverging/Spectral_11.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/qualitative/Accent_08.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/qualitative/Accent_08.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/qualitative/Dark2_08.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/qualitative/Dark2_08.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/qualitative/Paired_12.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/qualitative/Paired_12.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/qualitative/Pastel1_09.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/qualitative/Pastel1_09.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/qualitative/Pastel2_08.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/qualitative/Pastel2_08.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/qualitative/Set1_09.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/qualitative/Set1_09.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/qualitative/Set2_08.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/qualitative/Set2_08.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/qualitative/Set3_12.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/qualitative/Set3_12.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/sequential/Blues_09.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/Blues_09.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/sequential/BuGn_09.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/BuGn_09.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/sequential/BuPu_09.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/BuPu_09.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/sequential/GnBu_09.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/GnBu_09.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/sequential/Greens_09.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/Greens_09.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/sequential/Greys_09.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/Greys_09.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/sequential/OrRd_09.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/OrRd_09.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/sequential/Oranges_09.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/Oranges_09.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/sequential/PuBuGn_09.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/PuBuGn_09.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/sequential/PuBu_09.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/PuBu_09.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/sequential/PuRd_09.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/PuRd_09.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/sequential/Purples_09.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/Purples_09.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/sequential/RdPu_09.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/RdPu_09.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/sequential/Reds_09.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/Reds_09.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/sequential/YlGnBu_09.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/YlGnBu_09.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/sequential/YlGn_09.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/YlGn_09.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/sequential/YlOrBr_09.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/YlOrBr_09.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/etc/palette/sequential/YlOrRd_09.txt` & `scitools-iris-3.9.0rc0/lib/iris/etc/palette/sequential/YlOrRd_09.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/exceptions.py` & `scitools-iris-3.9.0rc0/lib/iris/exceptions.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/experimental/animate.py` & `scitools-iris-3.9.0rc0/lib/iris/experimental/animate.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/experimental/geovista.py` & `scitools-iris-3.9.0rc0/lib/iris/experimental/geovista.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/experimental/raster.py` & `scitools-iris-3.9.0rc0/lib/iris/experimental/raster.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/experimental/regrid.py` & `scitools-iris-3.9.0rc0/lib/iris/experimental/regrid.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/experimental/regrid_conservative.py` & `scitools-iris-3.9.0rc0/lib/iris/experimental/regrid_conservative.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/experimental/representation.py` & `scitools-iris-3.9.0rc0/lib/iris/experimental/representation.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/experimental/stratify.py` & `scitools-iris-3.9.0rc0/lib/iris/experimental/stratify.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/experimental/ugrid/__init__.py` & `scitools-iris-3.9.0rc0/lib/iris/experimental/ugrid/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/experimental/ugrid/cf.py` & `scitools-iris-3.9.0rc0/lib/iris/experimental/ugrid/cf.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/experimental/ugrid/load.py` & `scitools-iris-3.9.0rc0/lib/iris/experimental/ugrid/load.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/experimental/ugrid/mesh.py` & `scitools-iris-3.9.0rc0/lib/iris/experimental/ugrid/mesh.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/experimental/ugrid/metadata.py` & `scitools-iris-3.9.0rc0/lib/iris/experimental/ugrid/metadata.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/experimental/ugrid/save.py` & `scitools-iris-3.9.0rc0/lib/iris/experimental/ugrid/save.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/experimental/ugrid/utils.py` & `scitools-iris-3.9.0rc0/lib/iris/experimental/ugrid/utils.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/__init__.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/_ff.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/_ff.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/_ff_cross_references.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/_ff_cross_references.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/_nc_load_rules/actions.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/_nc_load_rules/actions.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/_nc_load_rules/engine.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/_nc_load_rules/engine.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/_nc_load_rules/helpers.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/_nc_load_rules/helpers.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/_pp_lbproc_pairs.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/_pp_lbproc_pairs.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/_structured_array_identification.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/_structured_array_identification.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/abf.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/abf.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/cf.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/cf.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/dot.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/dot.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/name.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/name.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/name_loaders.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/name_loaders.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/netcdf/__init__.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/netcdf/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/netcdf/_dask_locks.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/netcdf/_dask_locks.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/netcdf/_thread_safe_nc.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/netcdf/_thread_safe_nc.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/netcdf/loader.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/netcdf/loader.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/netcdf/saver.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/netcdf/saver.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/nimrod.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/nimrod.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/nimrod_load_rules.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/nimrod_load_rules.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/pp.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/pp.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/pp_load_rules.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/pp_load_rules.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/pp_save_rules.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/pp_save_rules.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/rules.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/rules.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/um/__init__.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/um/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/um/_fast_load.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/um/_fast_load.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/um/_fast_load_structured_fields.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/um/_fast_load_structured_fields.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/um/_ff_replacement.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/um/_ff_replacement.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/um/_optimal_array_structuring.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/um/_optimal_array_structuring.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/fileformats/um_cf_map.py` & `scitools-iris-3.9.0rc0/lib/iris/fileformats/um_cf_map.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/io/__init__.py` & `scitools-iris-3.9.0rc0/lib/iris/io/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/io/format_picker.py` & `scitools-iris-3.9.0rc0/lib/iris/io/format_picker.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/iterate.py` & `scitools-iris-3.9.0rc0/lib/iris/iterate.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/palette.py` & `scitools-iris-3.9.0rc0/lib/iris/palette.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/pandas.py` & `scitools-iris-3.9.0rc0/lib/iris/pandas.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/plot.py` & `scitools-iris-3.9.0rc0/lib/iris/plot.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/quickplot.py` & `scitools-iris-3.9.0rc0/lib/iris/quickplot.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/symbols.py` & `scitools-iris-3.9.0rc0/lib/iris/symbols.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/__init__.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/experimental/regrid/test_regrid_area_weighted_rectilinear_src_and_grid.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/experimental/regrid/test_regrid_area_weighted_rectilinear_src_and_grid.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/experimental/regrid/test_regrid_conservative_via_esmpy.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/experimental/regrid/test_regrid_conservative_via_esmpy.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/experimental/test_raster.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/experimental/test_raster.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/graphics/README.md` & `scitools-iris-3.9.0rc0/lib/iris/tests/graphics/README.md`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/graphics/__init__.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/graphics/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/graphics/idiff.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/graphics/idiff.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/graphics/recreate_imagerepo.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/graphics/recreate_imagerepo.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/analysis/test_area_weighted.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/analysis/test_area_weighted.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/attrs_matrix_results_load.json` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/attrs_matrix_results_load.json`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/attrs_matrix_results_roundtrip.json` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/attrs_matrix_results_roundtrip.json`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/attrs_matrix_results_save.json` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/attrs_matrix_results_save.json`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/aux_factory/test_OceanSigmaZFactory.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/aux_factory/test_OceanSigmaZFactory.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/concatenate/test_concatenate.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/concatenate/test_concatenate.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/experimental/geovista/test_cube_to_poly.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/geovista/test_cube_to_poly.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/experimental/geovista/test_extract_unstructured_region.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/geovista/test_extract_unstructured_region.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/experimental/test_CubeRepresentation.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/test_CubeRepresentation.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/experimental/test_regrid_ProjectedUnstructured.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/test_regrid_ProjectedUnstructured.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/experimental/test_ugrid_load.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/test_ugrid_load.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/experimental/test_ugrid_save.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/test_ugrid_save.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/README.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/README.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex1_1d_mesh.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex1_1d_mesh.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex2_2d_triangular.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex2_2d_triangular.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex3_2d_flexible.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex3_2d_flexible.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex4_3d_layered.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/experimental/ugrid_conventions_examples/ugrid_ex4_3d_layered.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/fast_load/test_fast_load.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/fast_load/test_fast_load.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/merge/test_merge.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/merge/test_merge.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/netcdf/test__dask_locks.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/netcdf/test__dask_locks.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/netcdf/test_attributes.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/netcdf/test_attributes.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/netcdf/test_aux_factories.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/netcdf/test_aux_factories.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/netcdf/test_coord_systems.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/netcdf/test_coord_systems.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/netcdf/test_delayed_save.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/netcdf/test_delayed_save.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/netcdf/test_general.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/netcdf/test_general.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/netcdf/test_self_referencing.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/netcdf/test_self_referencing.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/netcdf/test_thread_safety.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/netcdf/test_thread_safety.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/plot/test_animate.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/plot/test_animate.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/plot/test_colorbar.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/plot/test_colorbar.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/plot/test_netcdftime.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/plot/test_netcdftime.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/plot/test_nzdateline.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/plot/test_nzdateline.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/plot/test_plot_2d_coords.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/plot/test_plot_2d_coords.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/plot/test_vector_plots.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/plot/test_vector_plots.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/test_Datums.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_Datums.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/test_PartialDateTime.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_PartialDateTime.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/test_climatology.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_climatology.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/test_cube.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_cube.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/test_ff.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_ff.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/test_mask_cube_from_shapefile.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_mask_cube_from_shapefile.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/test_netcdf__loadsaveattrs.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_netcdf__loadsaveattrs.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/test_new_axis.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_new_axis.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/test_pickle.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_pickle.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/test_pp.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_pp.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/test_pp_constrained_load_cubes.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_pp_constrained_load_cubes.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/test_regrid_equivalence.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_regrid_equivalence.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/test_regridding.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_regridding.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/test_subset.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_subset.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/test_trajectory.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/test_trajectory.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/integration/um/test_fieldsfile.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/integration/um/test_fieldsfile.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/COLPEX/small_colpex_theta_p_alt.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/COLPEX/small_colpex_theta_p_alt.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/FF/air_temperature_1.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/FF/air_temperature_1.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/FF/air_temperature_2.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/FF/air_temperature_2.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/FF/ffheader.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/FF/ffheader.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/FF/soil_temperature_1.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/FF/soil_temperature_1.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/FF/surface_altitude_1.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/FF/surface_altitude_1.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/PP/extra_char_data.pp.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/PP/extra_char_data.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/PP/extra_char_data.w_data_loaded.pp.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/PP/extra_char_data.w_data_loaded.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/PP/extra_data_time_series.pp.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/PP/extra_data_time_series.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/PP/extra_x_data.pp.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/PP/extra_x_data.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/PP/global_test.pp.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/PP/global_test.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/PP/nae_unpacked.pp.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/PP/nae_unpacked.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/PP/rle_unpacked.pp.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/PP/rle_unpacked.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/abf/load.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/abf/load.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/abs.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/abs.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/addition.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/addition.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/addition_coord_x.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/addition_coord_x.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/addition_coord_y.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/addition_coord_y.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/addition_different_std_name.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/addition_different_std_name.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/addition_in_place.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/addition_in_place.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/addition_in_place_coord.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/addition_in_place_coord.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/addition_scalar.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/addition_scalar.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/easy.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/easy.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/multi.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/multi.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/multi_missing.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/multi_missing.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/multi_shared.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/multi_shared.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/single.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/single.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/single_missing.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/single_missing.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/single_rms.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/single_rms.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/single_shared.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/single_shared.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/single_shared_circular.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/single_shared_circular.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/weighted_easy.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_easy.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/weighted_multi.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_multi.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/weighted_multi_missing.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_multi_missing.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/weighted_multi_shared.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_multi_shared.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/weighted_single.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_single.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/weighted_single_missing.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_single_missing.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/weighted_single_shared.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_single_shared.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/aggregated_by/weighted_single_shared_circular.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/aggregated_by/weighted_single_shared_circular.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/apply_ifunc.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/apply_ifunc.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/apply_ifunc_frompyfunc.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/apply_ifunc_frompyfunc.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/apply_ifunc_original.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/apply_ifunc_original.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/apply_ufunc.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/apply_ufunc.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/apply_ufunc_frompyfunc.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/apply_ufunc_frompyfunc.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/apply_ufunc_original.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/apply_ufunc_original.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/areaweights_original.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/areaweights_original.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/curl_contrived_cartesian2.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/curl_contrived_cartesian2.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/delta_handmade_simple_wrt_x.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_simple_wrt_x.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_lat.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_lat.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_lon.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_lon.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_x.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_x.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_y.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/delta_handmade_wrt_y.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/grad_contrived1.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/grad_contrived1.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/grad_contrived2.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/grad_contrived2.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/grad_contrived_non_spherical1.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/grad_contrived_non_spherical1.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/handmade2_wrt_lat.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/handmade2_wrt_lat.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/handmade2_wrt_lon.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/handmade2_wrt_lon.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/handmade_simple_wrt_x.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/handmade_simple_wrt_x.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/handmade_wrt_lat.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/handmade_wrt_lat.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/handmade_wrt_lon.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/handmade_wrt_lon.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/handmade_wrt_x.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/handmade_wrt_x.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/calculus/handmade_wrt_y.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/calculus/handmade_wrt_y.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube1.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube1.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube1_cube1.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube1_cube1.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube2.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube2.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube2_cube1.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube2_cube1.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube3.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube3.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube4.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube4.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube5.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube1_cube5.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/cube2_cube3.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube2_cube3.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/cube2_cube4.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube2_cube4.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/cube2_cube5.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube2_cube5.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/cube3_cube4.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube3_cube4.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/cube3_cube5.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube3_cube5.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/coord_comparison/cube4_cube5.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/coord_comparison/cube4_cube5.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/count_bar_2d.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/count_bar_2d.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/count_foo_2d.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/count_foo_2d.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/count_foo_bar_2d.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/count_foo_bar_2d.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/division.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/division.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/division_by_array.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/division_by_array.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/division_by_latitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/division_by_latitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/division_by_longitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/division_by_longitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/division_by_singular_coord.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/division_by_singular_coord.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/division_scalar.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/division_scalar.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/exp.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/exp.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/exponentiate.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/exponentiate.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/first_quartile_foo_1d.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/first_quartile_foo_1d.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/first_quartile_foo_1d_fast_percentile.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/first_quartile_foo_1d_fast_percentile.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/first_quartile_foo_2d.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/first_quartile_foo_2d.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/first_quartile_foo_2d_fast_percentile.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/first_quartile_foo_2d_fast_percentile.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/first_quartile_foo_bar_2d.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/first_quartile_foo_bar_2d.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/first_quartile_foo_bar_2d_fast_percentile.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/first_quartile_foo_bar_2d_fast_percentile.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/gmean_latitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/gmean_latitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/gmean_latitude_longitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/gmean_latitude_longitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/gmean_latitude_longitude_1call.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/gmean_latitude_longitude_1call.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/hmean_latitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/hmean_latitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/hmean_latitude_longitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/hmean_latitude_longitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/hmean_latitude_longitude_1call.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/hmean_latitude_longitude_1call.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/last_quartile_foo_3d_masked.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/last_quartile_foo_3d_masked.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/last_quartile_foo_3d_notmasked.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/last_quartile_foo_3d_notmasked.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/last_quartile_foo_3d_notmasked_fast_percentile.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/last_quartile_foo_3d_notmasked_fast_percentile.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/log.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/log.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/log10.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/log10.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/log2.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/log2.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/maths_original.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/maths_original.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/max_latitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/max_latitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/max_latitude_longitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/max_latitude_longitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/max_latitude_longitude_1call.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/max_latitude_longitude_1call.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/max_run_bar_2d.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/max_run_bar_2d.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/max_run_bar_2d_masked.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/max_run_bar_2d_masked.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/max_run_foo_2d.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/max_run_foo_2d.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/mean_latitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/mean_latitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/mean_latitude_longitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/mean_latitude_longitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/mean_latitude_longitude_1call.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/mean_latitude_longitude_1call.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/median_latitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/median_latitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/median_latitude_longitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/median_latitude_longitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/median_latitude_longitude_1call.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/median_latitude_longitude_1call.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/min_latitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/min_latitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/min_latitude_longitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/min_latitude_longitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/min_latitude_longitude_1call.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/min_latitude_longitude_1call.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/multiply.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/multiply.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/multiply_different_std_name.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/multiply_different_std_name.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/original.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/original.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/original_common.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/original_common.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/original_hmean.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/original_hmean.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/proportion_bar_2d.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/proportion_bar_2d.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/proportion_foo_2d.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/proportion_foo_2d.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/proportion_foo_2d_masked.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/proportion_foo_2d_masked.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/proportion_foo_bar_2d.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/proportion_foo_bar_2d.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_both_circular.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_both_circular.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_circular_grid.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_circular_grid.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_circular_src.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_circular_src.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_circular_srcmissingmask.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_circular_srcmissingmask.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_masked_altitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_masked_altitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_non_circular.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_non_circular.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_partial_overlap.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_partial_overlap.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_subset.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_subset.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_subset_anon.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_subset_anon.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_subset_masked_1.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_subset_masked_1.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/linear_subset_masked_2.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/linear_subset_masked_2.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_both_circular.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_both_circular.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_circular_grid.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_circular_grid.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_circular_src.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_circular_src.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_circular_srcmissingmask.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_circular_srcmissingmask.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_masked_altitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_masked_altitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_non_circular.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_non_circular.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_partial_overlap.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_partial_overlap.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_subset.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_subset.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_subset_anon.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_subset_anon.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_subset_masked_1.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_subset_masked_1.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/nearest_subset_masked_2.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/nearest_subset_masked_2.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/regrid/no_overlap.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/regrid/no_overlap.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/rms_latitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/rms_latitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/rms_latitude_longitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/rms_latitude_longitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/rms_latitude_longitude_1call.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/rms_latitude_longitude_1call.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/rms_weighted_2d.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/rms_weighted_2d.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/rolling_window/simple_latitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/rolling_window/simple_latitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/rolling_window/simple_longitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/rolling_window/simple_longitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/rolling_window/size_4_longitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/rolling_window/size_4_longitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/sqrt.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/sqrt.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/std_dev_latitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/std_dev_latitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/std_dev_latitude_longitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/std_dev_latitude_longitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/std_dev_latitude_longitude_1call.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/std_dev_latitude_longitude_1call.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/subtract.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/subtract.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/subtract_array.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/subtract_array.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/subtract_coord_x.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/subtract_coord_x.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/subtract_coord_y.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/subtract_coord_y.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/subtract_scalar.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/subtract_scalar.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/sum_latitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/sum_latitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/sum_latitude_longitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/sum_latitude_longitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/sum_latitude_longitude_1call.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/sum_latitude_longitude_1call.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/sum_weighted_2d.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/sum_weighted_2d.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/third_quartile_foo_1d.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/third_quartile_foo_1d.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/third_quartile_foo_1d_fast_percentile.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/third_quartile_foo_1d_fast_percentile.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/variance_latitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/variance_latitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/variance_latitude_longitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/variance_latitude_longitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/variance_latitude_longitude_1call.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/variance_latitude_longitude_1call.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/weighted_mean_lat.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/weighted_mean_lat.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/weighted_mean_latlon.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/weighted_mean_latlon.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/weighted_mean_lon.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/weighted_mean_lon.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/weighted_mean_original.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/weighted_mean_original.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/analysis/weighted_mean_source.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/analysis/weighted_mean_source.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/categorisation/customcheck.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/categorisation/customcheck.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/categorisation/quickcheck.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/categorisation/quickcheck.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/0d_str.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/0d_str.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/1d_str.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/1d_str.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/2d_str.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/2d_str.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/3d_str.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/3d_str.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/4d_str.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/TestStockCubeStringRepresentations/4d_str.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cdm/extract/lat_eq_10.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/extract/lat_eq_10.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cdm/extract/lat_gt_10.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/extract/lat_gt_10.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cdm/extract/lat_gt_10_and_lon_ge_10.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/extract/lat_gt_10_and_lon_ge_10.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cdm/masked_cube.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/masked_cube.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cdm/masked_save_pp.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/masked_save_pp.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cdm/str_repr/0d_cube.__str__.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/str_repr/0d_cube.__str__.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cdm/str_repr/0d_cube.__unicode__.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/str_repr/0d_cube.__unicode__.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cdm/str_repr/cell_methods.__str__.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/str_repr/cell_methods.__str__.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cdm/str_repr/missing_coords_cube.str.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/str_repr/missing_coords_cube.str.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cdm/str_repr/similar.__str__.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/str_repr/similar.__str__.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cdm/test_simple_cube_intersection.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cdm/test_simple_cube_intersection.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2x2d.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2x2d.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_bounds.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_bounds.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_xy.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_y.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_y.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_y_xy.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_x_y_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2x2d_aux_xy.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2x2d_aux_xy_bounds.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_xy_bounds.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2x2d_aux_y.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_y.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2x2d_aux_y_xy.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2x2d_aux_y_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2y2d.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2y2d.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2y2d_aux_x.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_x.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2y2d_aux_x_xy.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_x_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2y2d_aux_x_y.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_x_y.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2y2d_aux_x_y_xy.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_x_y_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2y2d_aux_xy.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2y2d_aux_y.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_y.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_2y2d_aux_y_xy.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_2y2d_aux_y_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_3d_simple.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_3d_simple.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_4mix2d_aux_xy.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_4mix2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_4x2d_aux_xy.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_4x2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_4y2d_aux_xy.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_4y2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_9mix2d_aux_xy.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_9mix2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_9x2d_aux_xy.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_9x2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_9y2d_aux_xy.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_9y2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_anonymous.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_anonymous.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_masked_2x2d.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_masked_2x2d.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_masked_2y2d.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_masked_2y2d.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_merged_scalar_4mix2d_aux_xy.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_merged_scalar_4mix2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_merged_scalar_4x2d_aux_xy.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_merged_scalar_4x2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_merged_scalar_4y2d_aux_xy.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_merged_scalar_4y2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_pre_merged_scalar_4mix2d_aux_xy.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_pre_merged_scalar_4mix2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_pre_merged_scalar_4x2_aux_xy.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_pre_merged_scalar_4x2_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_pre_merged_scalar_4y2d_aux_xy.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_pre_merged_scalar_4y2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_scalar_4mix2d_aux_xy.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_scalar_4mix2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_scalar_4x2d_aux_xy.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_scalar_4x2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/concatenate/concat_scalar_4y2d_aux_xy.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/concatenate/concat_scalar_4y2d_aux_xy.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/all_10_load_match.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/all_10_load_match.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/all_ml_10_22_load_match.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/all_ml_10_22_load_match.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/attribute_constraint.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/attribute_constraint.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_10_and_theta_level_gt_30_le_3_load_match.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_10_and_theta_level_gt_30_le_3_load_match.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_10_and_theta_level_gt_30_le_3_load_strict.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_10_and_theta_level_gt_30_le_3_load_strict.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_10_load_match.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_10_load_match.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_10_load_strict.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_10_load_strict.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_and_all_10_load_match.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_and_all_10_load_match.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_and_theta_10_load_strict.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_and_theta_10_load_strict.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_and_theta_load_match.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_and_theta_load_match.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_and_theta_load_strict.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_and_theta_load_strict.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_gt_30_le_3_load_match.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_gt_30_le_3_load_match.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_gt_30_le_3_load_strict.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_gt_30_le_3_load_strict.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_lat_30_load_match.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_lat_30_load_match.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_lat_30_load_strict.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_lat_30_load_strict.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_lat_gt_30_load_match.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_lat_gt_30_load_match.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_lat_gt_30_load_strict.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_lat_gt_30_load_strict.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_load_match.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_load_match.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/constrained_load/theta_load_strict.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/constrained_load/theta_load_strict.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/coord_api/coord_maths/add_float_expl.xml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/coord_maths/add_float_expl.xml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/coord_api/coord_maths/add_simple_expl.xml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/coord_maths/add_simple_expl.xml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/coord_api/coord_maths/divide_simple_expl.xml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/coord_maths/divide_simple_expl.xml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/coord_api/coord_maths/mult_float_expl.xml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/coord_maths/mult_float_expl.xml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/coord_api/coord_maths/multiply_simple_expl.xml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/coord_maths/multiply_simple_expl.xml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/coord_api/coord_maths/negate_expl.xml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/coord_maths/negate_expl.xml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/coord_api/coord_maths/r_subtract_simple_exl.xml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/coord_maths/r_subtract_simple_exl.xml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/coord_api/coord_maths/right_divide_simple_expl.xml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/coord_maths/right_divide_simple_expl.xml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/coord_api/coord_maths/subtract_simple_expl.xml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/coord_maths/subtract_simple_expl.xml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/coord_api/nd_bounds.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/coord_api/nd_bounds.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/latitude_longitude_dual_stage.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/latitude_longitude_dual_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/latitude_longitude_single_stage.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/latitude_longitude_single_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/latitude_model_level_number_dual_stage.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/latitude_model_level_number_dual_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/latitude_model_level_number_single_stage.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/latitude_model_level_number_single_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/latitude_time_dual_stage.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/latitude_time_dual_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/latitude_time_single_stage.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/latitude_time_single_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/longitude_latitude_dual_stage.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/longitude_latitude_dual_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/longitude_latitude_single_stage.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/longitude_latitude_single_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/longitude_model_level_number_dual_stage.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/longitude_model_level_number_dual_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/longitude_model_level_number_single_stage.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/longitude_model_level_number_single_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/longitude_time_dual_stage.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/longitude_time_dual_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/longitude_time_single_stage.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/longitude_time_single_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/model_level_number_latitude_dual_stage.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_latitude_dual_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/model_level_number_latitude_single_stage.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_latitude_single_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/model_level_number_longitude_dual_stage.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_longitude_dual_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/model_level_number_longitude_single_stage.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_longitude_single_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/model_level_number_time_dual_stage.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_time_dual_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/model_level_number_time_single_stage.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/model_level_number_time_single_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/original.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/original.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/time_latitude_dual_stage.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/time_latitude_dual_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/time_latitude_single_stage.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/time_latitude_single_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/time_longitude_dual_stage.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/time_longitude_dual_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/time_longitude_single_stage.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/time_longitude_single_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/time_model_level_number_dual_stage.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/time_model_level_number_dual_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/time_model_level_number_single_stage.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/time_model_level_number_single_stage.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/triple_collapse_lat_ml_pt.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/triple_collapse_lat_ml_pt.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_collapsed/triple_collapse_ml_pt_lon.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_collapsed/triple_collapse_ml_pt_lon.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_io/pickling/cubelist.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_io/pickling/cubelist.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_io/pickling/single_cube.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_io/pickling/single_cube.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_io/pickling/theta.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_io/pickling/theta.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_io/pp/load/global.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_io/pp/load/global.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_merge/multidim_coord_merge.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_merge/multidim_coord_merge.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_merge/multidim_coord_merge_transpose.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_merge/multidim_coord_merge_transpose.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_merge/test_orig_point_cube.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_merge/test_orig_point_cube.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_merge/test_simple_attributes1.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_merge/test_simple_attributes1.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_merge/test_simple_attributes2.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_merge/test_simple_attributes2.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_merge/test_simple_attributes3.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_merge/test_simple_attributes3.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_merge/test_simple_bound_merge.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_merge/test_simple_bound_merge.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_merge/test_simple_merge.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_merge/test_simple_merge.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/2d_intersect_and_reverse.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/2d_intersect_and_reverse.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/2d_orig.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/2d_orig.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/2d_to_0d_cube_slice.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/2d_to_0d_cube_slice.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/2d_to_1d_cube_multi_slice.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/2d_to_1d_cube_multi_slice.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/2d_to_1d_cube_multi_slice2.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/2d_to_1d_cube_multi_slice2.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/2d_to_1d_cube_multi_slice3.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/2d_to_1d_cube_multi_slice3.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/2d_to_1d_cube_slice.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/2d_to_1d_cube_slice.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/2d_to_2d_revesed.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/2d_to_2d_revesed.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/2d_transposed.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/2d_transposed.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/real_data_dual_tuple_indexing1.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/real_data_dual_tuple_indexing1.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/real_data_dual_tuple_indexing2.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/real_data_dual_tuple_indexing2.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/real_data_dual_tuple_indexing3.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/real_data_dual_tuple_indexing3.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_slice/real_empty_data_indexing.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_slice/real_empty_data_indexing.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/append_multi.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/append_multi.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/append_single.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/append_single.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/default_coord_system.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/default_coord_system.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/depth.latitude.pp.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/depth.latitude.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/depth.time.pp.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/depth.time.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/eta.latitude.pp.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/eta.latitude.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/no_forecast_period.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/no_forecast_period.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/no_forecast_period.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/no_forecast_period.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/no_forecast_time.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/no_forecast_time.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/no_forecast_time.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/no_forecast_time.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/pressure.latitude.pp.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/pressure.latitude.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/pressure.time.pp.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/pressure.time.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/replace_multi.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/replace_multi.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/replace_single.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/replace_single.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/cube_to_pp/simple.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/cube_to_pp/simple.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/derived/column.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/derived/column.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/derived/no_orog.__str__.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/derived/no_orog.__str__.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/derived/no_orog.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/derived/no_orog.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/derived/removed_derived_coord.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/derived/removed_derived_coord.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/derived/removed_orog.__str__.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/derived/removed_orog.__str__.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/derived/removed_orog.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/derived/removed_orog.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/derived/removed_sigma.__str__.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/derived/removed_sigma.__str__.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/derived/removed_sigma.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/derived/removed_sigma.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/derived/transposed.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/derived/transposed.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/basic_orthogonal_cube.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/basic_orthogonal_cube.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_1d_squashed.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_1d_squashed.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_1d_squashed_2.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_1d_squashed_2.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_with_factory.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/analysis/interpolate/LinearInterpolator/orthogonal_cube_with_factory.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/const_lat_cross_section.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/const_lat_cross_section.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/const_lon_cross_section.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/const_lon_cross_section.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/higher.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/higher.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/hybridheight.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/hybridheight.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/latlonreduced.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/latlonreduced.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/lonhalved.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/lonhalved.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/lower.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/lower.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/simple.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/regrid/regrid_area_weighted_rectilinear_src_and_grid/simple.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/experimental/ugrid/2D_1t_face_half_levels.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/ugrid/2D_1t_face_half_levels.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/experimental/ugrid/2D_72t_face_half_levels.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/ugrid/2D_72t_face_half_levels.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/experimental/ugrid/3D_1t_face_full_levels.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/ugrid/3D_1t_face_full_levels.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/experimental/ugrid/3D_1t_face_half_levels.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/ugrid/3D_1t_face_half_levels.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/experimental/ugrid/3D_snow_pseudo_levels.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/ugrid/3D_snow_pseudo_levels.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/experimental/ugrid/3D_soil_pseudo_levels.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/ugrid/3D_soil_pseudo_levels.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/experimental/ugrid/3D_tile_pseudo_levels.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/ugrid/3D_tile_pseudo_levels.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/experimental/ugrid/3D_veg_pseudo_levels.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/ugrid/3D_veg_pseudo_levels.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/experimental/ugrid/surface_mean.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/experimental/ugrid/surface_mean.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/file_load/known_loaders.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/file_load/known_loaders.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/file_load/theta_levels.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/file_load/theta_levels.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/file_load/u_wind_levels.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/file_load/u_wind_levels.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/file_load/v_wind_levels.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/file_load/v_wind_levels.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/file_load/wind_levels.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/file_load/wind_levels.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/imagerepo.json` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/imagerepo.json`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/integration/climatology/TestClimatology/reference_simpledata.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/climatology/TestClimatology/reference_simpledata.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex1_1d_mesh.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex1_1d_mesh.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex2_2d_triangular.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex2_2d_triangular.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex3_2d_flexible.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex3_2d_flexible.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex4_3d_layered.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/experimental/ugrid_save/TestBasicSave/ugrid_ex4_3d_layered.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/aux_factories/TestAtmosphereSigma/save.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/aux_factories/TestAtmosphereSigma/save.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/aux_factories/TestHybridPressure/save.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/aux_factories/TestHybridPressure/save.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/aux_factories/TestSaveMultipleAuxFactories/hybrid_height_and_pressure.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/aux_factories/TestSaveMultipleAuxFactories/hybrid_height_and_pressure.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/aux_factories/TestSaveMultipleAuxFactories/hybrid_height_cubes.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/aux_factories/TestSaveMultipleAuxFactories/hybrid_height_cubes.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/general/TestDatasetAndPathSaves/basic_save.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/general/TestDatasetAndPathSaves/basic_save.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/general/TestDatasetAndPathSaves/path_string_save_same.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/general/TestDatasetAndPathSaves/path_string_save_same.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/multi_packed_multi_dtype.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/multi_packed_multi_dtype.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/multi_packed_single_dtype.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/multi_packed_single_dtype.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/single_packed_manual.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/single_packed_manual.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/single_packed_signed.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/single_packed_signed.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/single_packed_unsigned.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/netcdf/general/TestPackedData/single_packed_unsigned.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/integration/um/fieldsfile/TestStructuredLoadFF/simple.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/um/fieldsfile/TestStructuredLoadFF/simple.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/integration/um/fieldsfile/TestStructuredLoadFF/simple_callback.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/integration/um/fieldsfile/TestStructuredLoadFF/simple_callback.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/iterate/izip_nd_ortho.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/iterate/izip_nd_ortho.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/a_aux_b_aux.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/a_aux_b_aux.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/a_aux_b_dim.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/a_aux_b_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/a_dim_b_aux.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/a_dim_b_aux.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/a_dim_b_dim.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/a_dim_b_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/dec.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/dec.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/multi_split.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/multi_split.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/separable_combination.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/separable_combination.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/single_split.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/single_split.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/string_a_b.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/string_a_b.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/string_a_with_aux.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/string_a_with_aux.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/string_a_with_dim.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/string_a_with_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/string_b_with_aux.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/string_b_with_aux.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/string_b_with_dim.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/string_b_with_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/theta.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/theta.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/theta_two_times.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/theta_two_times.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_duplicate_data.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_duplicate_data.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_independent.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_independent.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_merging1.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_merging1.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_merging2.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_merging2.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_merging3.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_merging3.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_merging4.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_merging4.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_merging5.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_merging5.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_non_expanding.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_non_expanding.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_series.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_series.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_single_forecast.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_single_forecast.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_successive_forecasts.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_successive_forecasts.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_time_non_dim_coord.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_time_non_dim_coord.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_time_vs_forecast.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_time_vs_forecast.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/merge/time_triple_time_vs_ref_time.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/merge/time_triple_time_vs_ref_time.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEIII_field.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEIII_field.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEIII_timeseries.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEIII_timeseries.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEIII_trajectory.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEIII_trajectory.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEIII_trajectory0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEIII_trajectory0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEIII_version2.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEIII_version2.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEII_field.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEII_field.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEII_field__no_time_averaging.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEII_field__no_time_averaging.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEII_field__no_time_averaging_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEII_field__no_time_averaging_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/name/NAMEII_timeseries.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/name/NAMEII_timeseries.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/aliases.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/aliases.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/flag.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/flag.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/fulldims.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/fulldims.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/multiple.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/multiple.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/partialdims.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/partialdims.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/shared.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/TestNetCDFSave__ancillaries/shared.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/int64_auxiliary_coord_netcdf3.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/int64_auxiliary_coord_netcdf3.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/int64_dimension_coord_netcdf3.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/int64_dimension_coord_netcdf3.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/multi_dim_coord_slightly_different.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/multi_dim_coord_slightly_different.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_cell_methods.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_cell_methods.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_deferred_index_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_index_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_deferred_index_1.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_index_1.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_deferred_index_2.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_index_2.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_deferred_mix_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_mix_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_deferred_mix_1.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_mix_1.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_deferred_slice_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_slice_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_deferred_slice_1.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_slice_1.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_deferred_slice_2.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_slice_2.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_deferred_tuple_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_tuple_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_deferred_tuple_1.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_tuple_1.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_deferred_tuple_2.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_deferred_tuple_2.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_global_xyt_hires.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_global_xyt_hires.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_global_xyt_total.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_global_xyt_total.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_global_xyzt_gems.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_global_xyzt_gems.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_global_xyzt_gems_iter_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_global_xyzt_gems_iter_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_global_xyzt_gems_iter_1.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_global_xyzt_gems_iter_1.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_laea.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_laea.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_lcc.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_lcc.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_merc.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_merc.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_merc_false.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_merc_false.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_merc_scale_factor.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_merc_scale_factor.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_monotonic.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_monotonic.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_polar.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_polar.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_rotated_xy_land.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_rotated_xy_land.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_rotated_xyt_precipitation.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_rotated_xyt_precipitation.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_gridmapmulti.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_gridmapmulti.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_hybrid_height.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_hybrid_height.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_load_hybrid_height.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_load_hybrid_height.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_load_ndim_auxiliary.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_load_ndim_auxiliary.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_multi_0.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_multi_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_multi_1.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_multi_1.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_multi_2.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_multi_2.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_multiple.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_multiple.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_ndim_auxiliary.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_ndim_auxiliary.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_no_global_attr.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_no_global_attr.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_realistic_0d.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_realistic_0d.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_realistic_4d.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_realistic_4d.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_realistic_4d_no_hybrid.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_realistic_4d_no_hybrid.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_samedimcoord.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_samedimcoord.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_save_single.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_save_single.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_stereo.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_stereo.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_tmerc_and_climatology.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_tmerc_and_climatology.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_units_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_units_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/netcdf_units_1.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/netcdf_units_1.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/save_load_traj.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/save_load_traj.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/uint32_auxiliary_coord_netcdf3.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/uint32_auxiliary_coord_netcdf3.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/netcdf/uint32_dimension_coord_netcdf3.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/netcdf/uint32_dimension_coord_netcdf3.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/load_2flds.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/load_2flds.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/probability_fields.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/probability_fields.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_bmr04_precip_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_bmr04_precip_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_bsr05_precip_accum60_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_bsr05_precip_accum60_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_cloud3d0060_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_cloud3d0060_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_cloud_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_cloud_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_convection_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_convection_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_convwind_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_convwind_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_frzlev_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_frzlev_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_height_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_height_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_precip_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_precip_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_precipaccum_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_precipaccum_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_preciptype_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_preciptype_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_pressure_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_pressure_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_radiation_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_radiation_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_radiationuv_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_radiationuv_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_refl_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_refl_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_relhumidity3d0060_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_relhumidity3d0060_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_relhumidity_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_relhumidity_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_snow_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_snow_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_soil3d0060_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_soil3d0060_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_soil_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_soil_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_temperature_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_temperature_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_visibility_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_visibility_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_wind_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_wind_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_winduv3d0015_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_winduv3d0015_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek00_winduv_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek00_winduv_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek01_cape_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek01_cape_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_ek07_precip0540_accum180_18km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_ek07_precip0540_accum180_18km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/nimrod/u1096_ng_umqv_fog_2km.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/nimrod/u1096_ng_umqv_fog_2km.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/pandas/as_cube/data_frame_datetime_standard.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/pandas/as_cube/data_frame_datetime_standard.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/pandas/as_cube/data_frame_masked.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/pandas/as_cube/data_frame_masked.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/pandas/as_cube/data_frame_multidim.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/pandas/as_cube/data_frame_multidim.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/pandas/as_cube/data_frame_netcdftime_360.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/pandas/as_cube/data_frame_netcdftime_360.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/pandas/as_cube/data_frame_nonotonic.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/pandas/as_cube/data_frame_nonotonic.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/pandas/as_cube/data_frame_simple.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/pandas/as_cube/data_frame_simple.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/pandas/as_cube/series_datetime_standard.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/pandas/as_cube/series_datetime_standard.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/pandas/as_cube/series_netcdfimte_360.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/pandas/as_cube/series_netcdfimte_360.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/pp_load_rules/global.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/pp_load_rules/global.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/pp_load_rules/lbproc_mean_max_min.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/pp_load_rules/lbproc_mean_max_min.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/pp_load_rules/lbtim_2.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/pp_load_rules/lbtim_2.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/pp_load_rules/ocean_depth.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/pp_load_rules/ocean_depth.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/pp_load_rules/ocean_depth_bounded.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/pp_load_rules/ocean_depth_bounded.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/pp_load_rules/rotated_uk.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/pp_load_rules/rotated_uk.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/stock/realistic_4d.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/stock/realistic_4d.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/system/supported_filetype_.nc.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/system/supported_filetype_.nc.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/system/supported_filetype_.pp.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/system/supported_filetype_.pp.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/trajectory/constant_latitude.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/trajectory/constant_latitude.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/trajectory/hybrid_height.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/trajectory/hybrid_height.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/trajectory/single_point.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/trajectory/single_point.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/trajectory/tri_polar_latitude_slice.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/trajectory/tri_polar_latitude_slice.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/trajectory/zigzag.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/trajectory/zigzag.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/cartography/project/TestAll/cube.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/cartography/project/TestAll/cube.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_all_dims.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_all_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_last_dims.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_last_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_middle_dim.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_middle_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_zeroth_dim.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/collapse_zeroth_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/slice.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/slice.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/transposed.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__derived_coords/TestBroadcastingDerived/transposed.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_all_dims.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_all_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_last_dims.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_last_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_middle_dim.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_middle_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_zeroth_dim.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/collapse_zeroth_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/slice.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/slice.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/transposed.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMesh/transposed.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_all_dims.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_all_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_last_dims.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_last_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_middle_dim.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_middle_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_zeroth_dim.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/collapse_zeroth_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/slice.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/slice.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/transposed.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/_arith__meshcoords/TestBroadcastingWithMeshAndDerived/transposed.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_all_dims.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_all_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_last_dims.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_last_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_middle_dim.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_middle_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_zeroth_dim.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/collapse_zeroth_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/slice.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/slice.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/transposed.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/add/TestBroadcasting/transposed.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_all_dims.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_all_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_last_dims.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_last_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_middle_dim.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_middle_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_zeroth_dim.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/collapse_zeroth_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/slice.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/slice.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/transposed.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/divide/TestBroadcasting/transposed.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_all_dims.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_all_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_last_dims.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_last_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_middle_dim.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_middle_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_zeroth_dim.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/collapse_zeroth_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/slice.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/slice.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/transposed.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/multiply/TestBroadcasting/transposed.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_all_dims.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_all_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_last_dims.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_last_dims.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_middle_dim.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_middle_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_zeroth_dim.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/collapse_zeroth_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/slice.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/slice.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/transposed.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/analysis/maths/subtract/TestBroadcasting/transposed.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/metadata.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/metadata.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/metadata_wrapped.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/cube/Cube/intersection__Metadata/metadata_wrapped.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/cube/Cube/xml/ancils.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/cube/Cube/xml/ancils.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/cube/Cube/xml/cell_measures.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/cube/Cube/xml/cell_measures.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/combination_with_extra_realization.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/combination_with_extra_realization.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/combination_with_extra_triple.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/combination_with_extra_triple.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/combination_with_realization.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/combination_with_realization.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/orthogonal_with_realization.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/cube/CubeList/merge__time_triple/orthogonal_with_realization.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content/mesh_result.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/experimental/representation/CubeRepresentation/_make_content/mesh_result.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/experimental/stratify/relevel/Test/multi_dim_target_levels.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/experimental/stratify/relevel/Test/multi_dim_target_levels.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/mercator.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/mercator.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/mercator_no_ellipsoid.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/mercator_no_ellipsoid.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/stereographic.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/stereographic.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/stereographic_no_ellipsoid.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/stereographic_no_ellipsoid.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/stereographic_scale_factor.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/stereographic_scale_factor.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/transverse_mercator.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/transverse_mercator.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/transverse_mercator_no_ellipsoid.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/transverse_mercator_no_ellipsoid.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/with_climatology.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver/write/with_climatology.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver__ugrid/TestSaveUgrid__cube/basic_mesh.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/fileformats/netcdf/saver/Saver__ugrid/TestSaveUgrid__cube/basic_mesh.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/util/mask_cube/TestCubeMask/mask_cube_2d_create_new_dim.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/util/mask_cube/TestCubeMask/mask_cube_2d_create_new_dim.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/util/mask_cube/original_cube_full2d_global.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/util/mask_cube/original_cube_full2d_global.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/util/mask_cube/original_cube_simple_1d.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/util/mask_cube/original_cube_simple_1d.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/unit/util/mask_cube/original_cube_simple_2d.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/unit/util/mask_cube/original_cube_simple_2d.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/uri_callback/pp_global.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/uri_callback/pp_global.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.03.236.000128.1990.12.01.00.00.b_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.03.236.000128.1990.12.01.00.00.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.03.236.004224.1990.12.01.00.00.b_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.03.236.004224.1990.12.01.00.00.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.03.236.008320.1990.12.01.00.00.b_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.03.236.008320.1990.12.01.00.00.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.16.202.000128.1860.09.01.00.00.b_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/000003000000.16.202.000128.1860.09.01.00.00.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/001000000000.00.000.000000.1860.01.01.00.00.f.b_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/001000000000.00.000.000000.1860.01.01.00.00.f.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/002000000000.44.101.131200.1920.09.01.00.00.b_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/002000000000.44.101.131200.1920.09.01.00.00.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/008000000000.44.101.000128.1890.09.01.00.00.b_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/008000000000.44.101.000128.1890.09.01.00.00.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/12187.b_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/12187.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/HadCM2_ts_SAT_ann_18602100.b_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/HadCM2_ts_SAT_ann_18602100.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_level_lat_orig.b_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_level_lat_orig.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_lon_lat_press_orig.b_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_lon_lat_press_orig.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_lon_lat_several.b_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_lon_lat_several.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_n10r13xy.b_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_n10r13xy.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_time_press.b_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_time_press.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_tseries.b_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/aaxzc_tseries.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abcza_pa19591997_daily_29.b_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abcza_pa19591997_daily_29.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abcza_pa19591997_daily_29.b_1.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abcza_pa19591997_daily_29.b_1.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abcza_pa19591997_daily_29.b_2.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abcza_pa19591997_daily_29.b_2.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abxpa_press_lat.b_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/abxpa_press_lat.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/integer.b_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/integer.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/model.b_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/model.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/ocean_xsect.b_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/ocean_xsect.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/st0fc699.b_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/st0fc699.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/st0fc942.b_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/st0fc942.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/st30211.b_0.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_netcdf/st30211.b_0.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.03.236.000128.1990.12.01.00.00.b.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.03.236.000128.1990.12.01.00.00.b.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.03.236.004224.1990.12.01.00.00.b.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.03.236.004224.1990.12.01.00.00.b.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.03.236.008320.1990.12.01.00.00.b.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.03.236.008320.1990.12.01.00.00.b.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.16.202.000128.1860.09.01.00.00.b.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/000003000000.16.202.000128.1860.09.01.00.00.b.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/001000000000.00.000.000000.1860.01.01.00.00.f.b.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/001000000000.00.000.000000.1860.01.01.00.00.f.b.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/002000000000.44.101.131200.1920.09.01.00.00.b.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/002000000000.44.101.131200.1920.09.01.00.00.b.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/008000000000.44.101.000128.1890.09.01.00.00.b.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/008000000000.44.101.000128.1890.09.01.00.00.b.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/12187.b.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/12187.b.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/HadCM2_ts_SAT_ann_18602100.b.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/HadCM2_ts_SAT_ann_18602100.b.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_level_lat_orig.b.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_level_lat_orig.b.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_lon_lat_press_orig.b.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_lon_lat_press_orig.b.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_lon_lat_several.b.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_lon_lat_several.b.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_n10r13xy.b.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_n10r13xy.b.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_time_press.b.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_time_press.b.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_tseries.b.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/aaxzc_tseries.b.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/abcza_pa19591997_daily_29.b.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/abcza_pa19591997_daily_29.b.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/abxpa_press_lat.b.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/abxpa_press_lat.b.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/integer.b.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/integer.b.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/model.b.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/model.b.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/ocean_xsect.b.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/ocean_xsect.b.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/st0fc699.b.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/st0fc699.b.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/st0fc942.b.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/st0fc942.b.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/st30211.b.cml` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/from_pp/st30211.b.cml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.03.236.000128.1990.12.01.00.00.b_0.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.03.236.000128.1990.12.01.00.00.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.03.236.004224.1990.12.01.00.00.b_0.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.03.236.004224.1990.12.01.00.00.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.03.236.008320.1990.12.01.00.00.b_0.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.03.236.008320.1990.12.01.00.00.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.16.202.000128.1860.09.01.00.00.b_0.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/000003000000.16.202.000128.1860.09.01.00.00.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/001000000000.00.000.000000.1860.01.01.00.00.f.b_0.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/001000000000.00.000.000000.1860.01.01.00.00.f.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/002000000000.44.101.131200.1920.09.01.00.00.b_0.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/002000000000.44.101.131200.1920.09.01.00.00.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/008000000000.44.101.000128.1890.09.01.00.00.b_0.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/008000000000.44.101.000128.1890.09.01.00.00.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/12187.b_0.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/12187.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/HadCM2_ts_SAT_ann_18602100.b_0.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/HadCM2_ts_SAT_ann_18602100.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_level_lat_orig.b_0.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_level_lat_orig.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_lon_lat_press_orig.b_0.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_lon_lat_press_orig.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_lon_lat_several.b_0.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_lon_lat_several.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_n10r13xy.b_0.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_n10r13xy.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_time_press.b_0.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_time_press.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_tseries.b_0.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/aaxzc_tseries.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abcza_pa19591997_daily_29.b_0.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abcza_pa19591997_daily_29.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abcza_pa19591997_daily_29.b_1.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abcza_pa19591997_daily_29.b_1.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abcza_pa19591997_daily_29.b_2.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abcza_pa19591997_daily_29.b_2.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abxpa_press_lat.b_0.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/abxpa_press_lat.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/integer.b_0.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/integer.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/model.b_0.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/model.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/ocean_xsect.b_0.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/ocean_xsect.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/st0fc699.b_0.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/st0fc699.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/st0fc942.b_0.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/st0fc942.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/st30211.b_0.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_netcdf/st30211.b_0.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.03.236.000128.1990.12.01.00.00.b.pp.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.03.236.000128.1990.12.01.00.00.b.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.03.236.004224.1990.12.01.00.00.b.pp.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.03.236.004224.1990.12.01.00.00.b.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.03.236.008320.1990.12.01.00.00.b.pp.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.03.236.008320.1990.12.01.00.00.b.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.16.202.000128.1860.09.01.00.00.b.pp.txt` & `scitools-iris-3.9.0rc0/lib/iris/tests/results/usecases/pp_to_cf_conversion/to_pp/000003000000.16.202.000128.1860.09.01.00.00.b.pp.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/stock/__init__.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/stock/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/stock/_stock_2d_latlons.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/stock/_stock_2d_latlons.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/stock/file_headers/minimal_bad_mesh_cf_role.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/stock/file_headers/minimal_bad_mesh_cf_role.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/stock/file_headers/minimal_bad_topology_dim.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/stock/file_headers/minimal_bad_topology_dim.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/stock/file_headers/xios_2D_face_half_levels.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/stock/file_headers/xios_2D_face_half_levels.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/stock/file_headers/xios_3D_face_full_levels.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/stock/file_headers/xios_3D_face_full_levels.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/stock/file_headers/xios_3D_face_half_levels.cdl` & `scitools-iris-3.9.0rc0/lib/iris/tests/stock/file_headers/xios_3D_face_half_levels.cdl`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/stock/mesh.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/stock/mesh.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/stock/netcdf.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/stock/netcdf.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/system_test.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/system_test.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_abf.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_abf.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_aggregate_by.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_aggregate_by.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_analysis.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_analysis_calculus.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_analysis_calculus.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_basic_maths.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_basic_maths.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_cartography.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_cartography.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_cdm.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_cdm.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_cell.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_cell.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_cf.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_cf.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_coding_standards.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_coding_standards.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_concatenate.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_concatenate.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_constraints.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_coord_api.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_coord_api.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_coordsystem.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_coordsystem.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_cube.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_cube.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_cube_to_pp.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_cube_to_pp.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_ff.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_ff.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_file_load.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_file_load.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_file_save.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_file_save.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_hybrid.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_hybrid.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_image_json.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_image_json.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_imports.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_intersect.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_intersect.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_io_init.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_io_init.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_iterate.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_iterate.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_lazy_aggregate_by.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_lazy_aggregate_by.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_load.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_mapping.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_merge.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_name.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_name.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_netcdf.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_netcdf.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_nimrod.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_nimrod.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_peak.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_peak.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_pickling.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_plot.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_pp_cf.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_pp_cf.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_pp_module.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_pp_module.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_pp_stash.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_pp_stash.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_pp_to_cube.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_pp_to_cube.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_quickplot.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_quickplot.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_std_names.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_std_names.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_uri_callback.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_uri_callback.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/test_util.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/area_weighted/test_AreaWeightedRegridder.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/area_weighted/test_AreaWeightedRegridder.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/cartography/test__get_lon_lat_coords.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/cartography/test__get_lon_lat_coords.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/cartography/test__quadrant_area.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/cartography/test__quadrant_area.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/cartography/test__xy_range.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/cartography/test__xy_range.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/cartography/test_area_weights.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/cartography/test_area_weights.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/cartography/test_gridcell_angles.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/cartography/test_gridcell_angles.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/cartography/test_project.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/cartography/test_project.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/cartography/test_rotate_grid_vectors.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/cartography/test_rotate_grid_vectors.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/cartography/test_rotate_winds.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/cartography/test_rotate_winds.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/geometry/test__extract_relevant_cube_slice.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/geometry/test__extract_relevant_cube_slice.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/geometry/test_geometry_area_weights.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/geometry/test_geometry_area_weights.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/interpolation/test_RectilinearInterpolator.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/interpolation/test_RectilinearInterpolator.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/interpolation/test_get_xy_dim_coords.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/interpolation/test_get_xy_dim_coords.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/maths/__init__.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/maths/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/maths/test__arith__dask_array.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/maths/test__arith__dask_array.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/maths/test__arith__derived_coords.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/maths/test__arith__derived_coords.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/maths/test__arith__meshcoords.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/maths/test__arith__meshcoords.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/maths/test__get_dtype.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/maths/test__get_dtype.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/maths/test__inplace_common_checks.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/maths/test__inplace_common_checks.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/maths/test__output_dtype.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/maths/test__output_dtype.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/maths/test_add.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/maths/test_add.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/maths/test_divide.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/maths/test_divide.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/maths/test_multiply.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/maths/test_multiply.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/maths/test_subtract.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/maths/test_subtract.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/regrid/test_RectilinearRegridder.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/regrid/test_RectilinearRegridder.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/regrid/test__CurvilinearRegridder.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/regrid/test__CurvilinearRegridder.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/scipy_interpolate/test__RegularGridInterpolator.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/scipy_interpolate/test__RegularGridInterpolator.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/stats/test_pearsonr.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/stats/test_pearsonr.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_Aggregator.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_Aggregator.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_AreaWeighted.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_AreaWeighted.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_COUNT.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_COUNT.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_Linear.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_Linear.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_MAX.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_MAX.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_MAX_RUN.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_MAX_RUN.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_MEAN.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_MEAN.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_MIN.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_MIN.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_Nearest.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_Nearest.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_PERCENTILE.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_PERCENTILE.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_PROPORTION.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_PROPORTION.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_PercentileAggregator.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_PercentileAggregator.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_PointInCell.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_PointInCell.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_RMS.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_RMS.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_STD_DEV.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_STD_DEV.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_SUM.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_SUM.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_VARIANCE.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_VARIANCE.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_WPERCENTILE.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_WPERCENTILE.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test_WeightedPercentileAggregator.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test_WeightedPercentileAggregator.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/test__axis_to_single_trailing.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/test__axis_to_single_trailing.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/trajectory/test_Trajectory.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/trajectory/test_Trajectory.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/trajectory/test_UnstructuredNearestNeighbourRegridder.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/trajectory/test_UnstructuredNearestNeighbourRegridder.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/trajectory/test__nearest_neighbour_indices_ndcoords.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/trajectory/test__nearest_neighbour_indices_ndcoords.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/analysis/trajectory/test_interpolate.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/analysis/trajectory/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/aux_factory/test_AtmosphereSigmaFactory.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/aux_factory/test_AtmosphereSigmaFactory.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/aux_factory/test_AuxCoordFactory.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/aux_factory/test_AuxCoordFactory.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/aux_factory/test_HybridPressureFactory.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/aux_factory/test_HybridPressureFactory.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/aux_factory/test_OceanSFactory.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/aux_factory/test_OceanSFactory.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/aux_factory/test_OceanSg1Factory.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/aux_factory/test_OceanSg1Factory.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/aux_factory/test_OceanSg2Factory.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/aux_factory/test_OceanSg2Factory.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/aux_factory/test_OceanSigmaFactory.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/aux_factory/test_OceanSigmaFactory.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/aux_factory/test_OceanSigmaZFactory.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/aux_factory/test_OceanSigmaZFactory.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/common/lenient/test_Lenient.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/lenient/test_Lenient.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/common/lenient/test__Lenient.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/lenient/test__Lenient.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/common/lenient/test__lenient_client.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/lenient/test__lenient_client.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/common/lenient/test__lenient_service.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/lenient/test__lenient_service.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/common/lenient/test__qualname.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/lenient/test__qualname.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/common/metadata/test_AncillaryVariableMetadata.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/metadata/test_AncillaryVariableMetadata.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/common/metadata/test_BaseMetadata.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/metadata/test_BaseMetadata.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/common/metadata/test_CellMeasureMetadata.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/metadata/test_CellMeasureMetadata.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/common/metadata/test_CoordMetadata.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/metadata/test_CoordMetadata.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/common/metadata/test_CubeMetadata.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/metadata/test_CubeMetadata.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/common/metadata/test__NamedTupleMeta.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/metadata/test__NamedTupleMeta.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/common/metadata/test_hexdigest.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/metadata/test_hexdigest.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/common/metadata/test_metadata_filter.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/metadata/test_metadata_filter.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/common/metadata/test_metadata_manager_factory.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/metadata/test_metadata_manager_factory.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/common/mixin/test_CFVariableMixin.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/mixin/test_CFVariableMixin.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/common/mixin/test_LimitedAttributeDict.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/mixin/test_LimitedAttributeDict.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/common/mixin/test__get_valid_standard_name.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/mixin/test__get_valid_standard_name.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/common/resolve/test_Resolve.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/common/resolve/test_Resolve.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/concatenate/__init__.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/concatenate/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/concatenate/test__CoordMetaData.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/concatenate/test__CoordMetaData.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/concatenate/test__CoordSignature.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/concatenate/test__CoordSignature.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/concatenate/test__CubeSignature.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/concatenate/test__CubeSignature.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/concatenate/test_concatenate.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/concatenate/test_concatenate.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/config/test_NetCDF.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/config/test_NetCDF.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/constraints/test_Constraint_equality.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/constraints/test_Constraint_equality.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/constraints/test_NameConstraint.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/constraints/test_NameConstraint.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/coord_categorisation/test_add_categorised_coord.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_categorisation/test_add_categorised_coord.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/coord_categorisation/test_add_hour.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_categorisation/test_add_hour.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/coord_categorisation/test_coord_categorisation.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_categorisation/test_coord_categorisation.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_AlbersEqualArea.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_AlbersEqualArea.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_GeogCS.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_GeogCS.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_Geostationary.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_Geostationary.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_LambertAzimuthalEqualArea.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_LambertAzimuthalEqualArea.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_LambertConformal.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_LambertConformal.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_Mercator.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_Mercator.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_ObliqueMercator.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_ObliqueMercator.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_Orthographic.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_Orthographic.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_PolarStereographic.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_PolarStereographic.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_RotatedMercator.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_RotatedMercator.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_RotatedPole.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_RotatedPole.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_Stereographic.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_Stereographic.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_TransverseMercator.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_TransverseMercator.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/coord_systems/test_VerticalPerspective.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/coord_systems/test_VerticalPerspective.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/coords/__init__.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/coords/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/coords/test_AncillaryVariable.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/coords/test_AncillaryVariable.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/coords/test_AuxCoord.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/coords/test_AuxCoord.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/coords/test_Cell.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/coords/test_Cell.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/coords/test_CellMeasure.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/coords/test_CellMeasure.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/coords/test_CellMethod.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/coords/test_CellMethod.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/coords/test_Coord.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/coords/test_Coord.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/coords/test_DimCoord.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/coords/test_DimCoord.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/coords/test__DimensionalMetadata.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/coords/test__DimensionalMetadata.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/cube/test_Cube.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/cube/test_Cube.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/cube/test_CubeAttrsDict.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/cube/test_CubeAttrsDict.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/cube/test_CubeList.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/cube/test_CubeList.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/cube/test_Cube__aggregated_by.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/cube/test_Cube__aggregated_by.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/cube/test_Cube__operators.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/cube/test_Cube__operators.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/data_manager/test_DataManager.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/data_manager/test_DataManager.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/experimental/geovista/test_cube_to_polydata.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/geovista/test_cube_to_polydata.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/experimental/geovista/test_extract_unstructured_region.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/geovista/test_extract_unstructured_region.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/experimental/raster/test_export_geotiff.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/raster/test_export_geotiff.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/experimental/regrid/test_regrid_area_weighted_rectilinear_src_and_grid.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/regrid/test_regrid_area_weighted_rectilinear_src_and_grid.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/experimental/regrid/test_regrid_weighted_curvilinear_to_rectilinear.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/regrid/test_regrid_weighted_curvilinear_to_rectilinear.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/experimental/representation/test_CubeListRepresentation.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/representation/test_CubeListRepresentation.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/experimental/representation/test_CubeRepresentation.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/representation/test_CubeRepresentation.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/experimental/stratify/test_relevel.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/stratify/test_relevel.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridAuxiliaryCoordinateVariable.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridAuxiliaryCoordinateVariable.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridConnectivityVariable.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridConnectivityVariable.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridGroup.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridGroup.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridMeshVariable.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridMeshVariable.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridReader.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/cf/test_CFUGridReader.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/load/test_ParseUgridOnLoad.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/load/test_ParseUgridOnLoad.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/load/test_load_mesh.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/load/test_load_mesh.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/load/test_load_meshes.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/load/test_load_meshes.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/mesh/test_Connectivity.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/mesh/test_Connectivity.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/mesh/test_Mesh.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/mesh/test_Mesh.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/mesh/test_MeshCoord.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/mesh/test_MeshCoord.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/mesh/test_Mesh__from_coords.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/mesh/test_Mesh__from_coords.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/metadata/test_ConnectivityMetadata.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/metadata/test_ConnectivityMetadata.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/metadata/test_MeshCoordMetadata.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/metadata/test_MeshCoordMetadata.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/metadata/test_MeshMetadata.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/metadata/test_MeshMetadata.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/experimental/ugrid/utils/test_recombine_submeshes.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/experimental/ugrid/utils/test_recombine_submeshes.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/__init__.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/abf/test_ABFField.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/abf/test_ABFField.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/cf/test_CFGroup.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/cf/test_CFGroup.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/cf/test_CFReader.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/cf/test_CFReader.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/dot/test__dot_path.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/dot/test__dot_path.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/ff/test_ArakawaC.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/ff/test_ArakawaC.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/ff/test_ENDGame.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/ff/test_ENDGame.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/ff/test_FF2PP.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/ff/test_FF2PP.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/ff/test_FFHeader.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/ff/test_FFHeader.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/ff/test_Grid.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/ff/test_Grid.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/ff/test_NewDynamics.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/ff/test_NewDynamics.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/name_loaders/test__build_cell_methods.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/name_loaders/test__build_cell_methods.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/name_loaders/test__build_lat_lon_for_NAME_timeseries.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/name_loaders/test__build_lat_lon_for_NAME_timeseries.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/name_loaders/test__calc_integration_period.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/name_loaders/test__calc_integration_period.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/name_loaders/test__cf_height_from_name.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/name_loaders/test__cf_height_from_name.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/name_loaders/test__generate_cubes.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/name_loaders/test__generate_cubes.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/__init__.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__grid_mappings.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__grid_mappings.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__hybrid_formulae.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__hybrid_formulae.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__latlon_dimcoords.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__latlon_dimcoords.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__miscellaneous.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__miscellaneous.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__time_coords.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/actions/test__time_coords.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/engine/test_engine.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test__normalise_bounds_units.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test__normalise_bounds_units.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_albers_equal_area_coordinate_system.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_albers_equal_area_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_ancil_var.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_ancil_var.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_auxiliary_coordinate.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_auxiliary_coordinate.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_cell_measure.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_cell_measure.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_cube_metadata.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_cube_metadata.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_dimension_coordinate.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_dimension_coordinate.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_geostationary_coordinate_system.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_geostationary_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_lambert_azimuthal_equal_area_coordinate_system.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_lambert_azimuthal_equal_area_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_lambert_conformal_coordinate_system.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_lambert_conformal_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_mercator_coordinate_system.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_mercator_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_oblique_mercator_coordinate_system.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_oblique_mercator_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_polar_stereographic_coordinate_system.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_polar_stereographic_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_stereographic_coordinate_system.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_stereographic_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_transverse_mercator_coordinate_system.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_transverse_mercator_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_verticalp_coordinate_system.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_build_verticalp_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_get_attr_units.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_get_attr_units.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_get_cf_bounds_var.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_get_cf_bounds_var.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_get_names.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_get_names.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_has_supported_mercator_parameters.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_has_supported_mercator_parameters.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_has_supported_polar_stereographic_parameters.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_has_supported_polar_stereographic_parameters.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_parse_cell_methods.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_parse_cell_methods.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_reorder_bounds_data.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nc_load_rules/helpers/test_reorder_bounds_data.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/loader/test__chunk_control.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/loader/test__chunk_control.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/loader/test__get_cf_var_data.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/loader/test__get_cf_var_data.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/loader/test__load_aux_factory.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/loader/test__load_aux_factory.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/loader/test__load_cube.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/loader/test__load_cube.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/loader/test__translate_constraints_to_var_callback.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/loader/test__translate_constraints_to_var_callback.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/loader/test_load_cubes.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/loader/test_load_cubes.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver__lazy.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver__lazy.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver__lazy_stream_data.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver__lazy_stream_data.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver__ugrid.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/test_Saver__ugrid.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/netcdf/saver/test_save.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/netcdf/saver/test_save.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nimrod_load_rules/test_units.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nimrod_load_rules/test_units.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/nimrod_load_rules/test_vertical_coord.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/nimrod_load_rules/test_vertical_coord.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp/test_PPDataProxy.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp/test_PPDataProxy.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp/test_PPField.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp/test_PPField.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp/test__convert_constraints.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp/test__convert_constraints.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp/test__create_field_data.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp/test__create_field_data.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp/test__data_bytes_to_shaped_array.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp/test__data_bytes_to_shaped_array.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp/test__field_gen.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp/test__field_gen.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp/test__interpret_field.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp/test__interpret_field.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp/test_as_fields.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp/test_as_fields.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp/test_load.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp/test_load.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp/test_save.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp/test_save.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp/test_save_fields.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp/test_save_fields.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp/test_save_pairs_from_cube.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp/test_save_pairs_from_cube.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp_load_rules/test__all_other_rules.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__all_other_rules.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp_load_rules/test__collapse_degenerate_points_and_bounds.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__collapse_degenerate_points_and_bounds.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_scalar_pseudo_level_coords.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_scalar_pseudo_level_coords.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_scalar_realization_coords.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_scalar_realization_coords.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_time_coords.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_time_coords.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_vertical_coords.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__convert_vertical_coords.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp_load_rules/test__dim_or_aux.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__dim_or_aux.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp_load_rules/test__epoch_date_hours.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__epoch_date_hours.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp_load_rules/test__model_level_number.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__model_level_number.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp_load_rules/test__reduced_points_and_bounds.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__reduced_points_and_bounds.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp_load_rules/test__reshape_vector_args.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test__reshape_vector_args.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/pp_load_rules/test_convert.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/pp_load_rules/test_convert.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/rules/test_Loader.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/rules/test_Loader.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/rules/test__make_cube.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/rules/test__make_cube.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/structured_array_identification/test_ArrayStructure.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/structured_array_identification/test_ArrayStructure.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/structured_array_identification/test_GroupStructure.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/structured_array_identification/test_GroupStructure.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/test_rules.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/test_rules.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/um/fast_load/test_FieldCollation.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/um/fast_load/test_FieldCollation.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/um/fast_load/test__convert_collation.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/um/fast_load/test__convert_collation.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/um/fast_load_structured_fields/test_BasicFieldCollation.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/um/fast_load_structured_fields/test_BasicFieldCollation.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/um/fast_load_structured_fields/test_group_structured_fields.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/um/fast_load_structured_fields/test_group_structured_fields.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/um/optimal_array_structuring/test_optimal_array_structure.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/um/optimal_array_structuring/test_optimal_array_structure.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/fileformats/um/test_um_to_pp.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/fileformats/um/test_um_to_pp.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/io/test__generate_cubes.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/io/test__generate_cubes.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/io/test_expand_filespecs.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/io/test_expand_filespecs.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/io/test_run_callback.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/io/test_run_callback.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/io/test_save.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/io/test_save.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/lazy_data/test_as_concrete_data.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/lazy_data/test_as_concrete_data.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/lazy_data/test_as_lazy_data.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/lazy_data/test_as_lazy_data.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/lazy_data/test_co_realise_cubes.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/lazy_data/test_co_realise_cubes.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/lazy_data/test_is_lazy_data.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/lazy_data/test_is_lazy_data.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/lazy_data/test_is_lazy_masked_data.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/lazy_data/test_is_lazy_masked_data.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/lazy_data/test_lazy_elementwise.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/lazy_data/test_lazy_elementwise.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/lazy_data/test_map_complete_blocks.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/lazy_data/test_map_complete_blocks.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/lazy_data/test_multidim_lazy_stack.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/lazy_data/test_multidim_lazy_stack.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/lazy_data/test_non_lazy.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/lazy_data/test_non_lazy.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/merge/test_ProtoCube.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/merge/test_ProtoCube.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/pandas/test_pandas.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/pandas/test_pandas.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/plot/__init__.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/plot/_blockplot_common.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/_blockplot_common.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/plot/test__check_bounds_contiguity_and_mask.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test__check_bounds_contiguity_and_mask.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/plot/test__check_geostationary_coords_and_convert.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test__check_geostationary_coords_and_convert.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/plot/test__fixup_dates.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test__fixup_dates.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/plot/test__get_plot_defn.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test__get_plot_defn.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/plot/test__get_plot_defn_custom_coords_picked.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test__get_plot_defn_custom_coords_picked.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/plot/test__get_plot_objects.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test__get_plot_objects.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/plot/test__replace_axes_with_cartopy_axes.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test__replace_axes_with_cartopy_axes.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/plot/test_contour.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test_contour.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/plot/test_contourf.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test_contourf.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/plot/test_hist.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test_hist.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/plot/test_outline.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test_outline.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/plot/test_pcolor.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test_pcolor.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/plot/test_pcolormesh.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test_pcolormesh.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/plot/test_plot.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test_plot.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/plot/test_points.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test_points.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/plot/test_scatter.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/plot/test_scatter.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/quickplot/test_contour.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/quickplot/test_contour.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/quickplot/test_contourf.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/quickplot/test_contourf.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/quickplot/test_outline.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/quickplot/test_outline.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/quickplot/test_pcolor.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/quickplot/test_pcolor.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/quickplot/test_pcolormesh.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/quickplot/test_pcolormesh.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/quickplot/test_plot.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/quickplot/test_plot.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/quickplot/test_points.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/quickplot/test_points.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/quickplot/test_scatter.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/quickplot/test_scatter.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/representation/cube_printout/test_CubePrintout.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/representation/cube_printout/test_CubePrintout.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/representation/cube_printout/test_Table.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/representation/cube_printout/test_Table.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/representation/cube_summary/test_CubeSummary.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/representation/cube_summary/test_CubeSummary.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/test_Future.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/test_Future.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/test_sample_data_path.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/test_sample_data_path.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/tests/stock/test_netcdf.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/tests/stock/test_netcdf.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/tests/test_IrisTest.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/tests/test_IrisTest.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/time/test_PartialDateTime.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/time/test_PartialDateTime.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/util/test__coord_regular.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test__coord_regular.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/util/test__is_circular.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test__is_circular.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/util/test__mask_array.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test__mask_array.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/util/test__slice_data_with_keys.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test__slice_data_with_keys.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/util/test_array_equal.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_array_equal.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/util/test_broadcast_to_shape.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_broadcast_to_shape.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/util/test_column_slices_generator.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_column_slices_generator.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/util/test_demote_dim_coord_to_aux_coord.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_demote_dim_coord_to_aux_coord.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/util/test_describe_diff.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_describe_diff.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/util/test_equalise_attributes.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_equalise_attributes.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/util/test_file_is_newer_than.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_file_is_newer_than.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/util/test_find_discontiguities.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_find_discontiguities.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/util/test_guess_coord_axis.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_guess_coord_axis.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/util/test_mask_cube.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_mask_cube.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/util/test_mask_cube_from_shapefile.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_mask_cube_from_shapefile.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/util/test_new_axis.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_new_axis.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/util/test_promote_aux_coord_to_dim_coord.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_promote_aux_coord_to_dim_coord.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/util/test_reverse.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_reverse.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/util/test_rolling_window.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_rolling_window.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/util/test_squeeze.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_squeeze.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/tests/unit/util/test_unify_time_units.py` & `scitools-iris-3.9.0rc0/lib/iris/tests/unit/util/test_unify_time_units.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/time.py` & `scitools-iris-3.9.0rc0/lib/iris/time.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/util.py` & `scitools-iris-3.9.0rc0/lib/iris/util.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/iris/warnings.py` & `scitools-iris-3.9.0rc0/lib/iris/warnings.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/lib/scitools_iris.egg-info/PKG-INFO` & `scitools-iris-3.9.0rc0/lib/scitools_iris.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scitools-iris
-Version: 3.9.0
+Version: 3.9.0rc0
 Summary: A powerful, format-agnostic, community-driven Python package for analysing and visualising Earth science data
 Author-email: Iris Contributors <scitools.pub@gmail.com>
 License: BSD-3-Clause
 Project-URL: Code, https://github.com/SciTools/iris
 Project-URL: Discussions, https://github.com/SciTools/iris/discussions
 Project-URL: Documentation, https://scitools-iris.readthedocs.io/en/stable/
 Project-URL: Issues, https://github.com/SciTools/iris/issues
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: scitools-iris Version: 3.9.0 Summary: A powerful,
-format-agnostic, community-driven Python package for analysing and visualising
-Earth science data Author-email: Iris Contributors
+Metadata-Version: 2.1 Name: scitools-iris Version: 3.9.0rc0 Summary: A
+powerful, format-agnostic, community-driven Python package for analysing and
+visualising Earth science data Author-email: Iris Contributors
 gmail.com> License: BSD-3-Clause Project-URL: Code, https://github.com/
 SciTools/iris Project-URL: Discussions, https://github.com/SciTools/iris/
 discussions Project-URL: Documentation, https://scitools-iris.readthedocs.io/
 en/stable/ Project-URL: Issues, https://github.com/SciTools/iris/issues
 Keywords: cf-metadata,data-analysis,earth-
 science,grib,netcdf,meteorology,oceanography,space-weather,ugrid,visualisation
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
```

### Comparing `scitools_iris-3.9.0/lib/scitools_iris.egg-info/SOURCES.txt` & `scitools-iris-3.9.0rc0/lib/scitools_iris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/pyproject.toml` & `scitools-iris-3.9.0rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/setup.py` & `scitools-iris-3.9.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `scitools_iris-3.9.0/tools/generate_std_names.py` & `scitools-iris-3.9.0rc0/tools/generate_std_names.py`

 * *Files identical despite different names*


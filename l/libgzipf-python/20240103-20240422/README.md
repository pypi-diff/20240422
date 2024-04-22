# Comparing `tmp/libgzipf-python-20240103.tar.gz` & `tmp/libgzipf-python-20240422.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libgzipf-python-20240103.tar", last modified: Wed Jan  3 05:25:29 2024, max compression
+gzip compressed data, was "libgzipf-python-20240422.tar", last modified: Mon Apr 22 05:09:02 2024, max compression
```

## Comparing `libgzipf-python-20240103.tar` & `libgzipf-python-20240422.tar`

### file list

```diff
@@ -1,792 +1,792 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:28.000000 libgzipf-20240103/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_area.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_mapped_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3999 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1256 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_area.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_mapped_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_segments_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_segments_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32748 2024-01-03 05:12:40.000000 libgzipf-20240103/libfdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-01-03 05:12:26.000000 libgzipf-20240103/libfdata/libfdata_vector.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-01-03 04:40:29.000000 libgzipf-20240103/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-01-03 05:12:39.000000 libgzipf-20240103/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 04:40:29.000000 libgzipf-20240103/NEWS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-01-03 05:12:40.000000 libgzipf-20240103/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:28.000000 libgzipf-20240103/gzipftools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15357 2024-01-03 04:43:34.000000 libgzipf-20240103/gzipftools/gzipfmount.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1472 2024-01-03 04:40:30.000000 libgzipf-20240103/gzipftools/gzipftools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37205 2024-01-03 04:40:30.000000 libgzipf-20240103/gzipftools/mount_dokan.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2983 2024-01-03 04:43:34.000000 libgzipf-20240103/gzipftools/mount_file_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26459 2024-01-03 04:40:30.000000 libgzipf-20240103/gzipftools/mount_fuse.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2285 2024-01-03 04:43:34.000000 libgzipf-20240103/gzipftools/info_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5417 2024-01-03 04:40:30.000000 libgzipf-20240103/gzipftools/mount_dokan.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18940 2024-01-03 04:43:34.000000 libgzipf-20240103/gzipftools/mount_file_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-01-03 04:40:30.000000 libgzipf-20240103/gzipftools/gzipftools_libgzipf.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-01-03 04:40:30.000000 libgzipf-20240103/gzipftools/gzipftools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2192 2023-12-03 09:09:54.000000 libgzipf-20240103/gzipftools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-01-03 04:40:30.000000 libgzipf-20240103/gzipftools/gzipftools_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1771 2024-01-03 04:40:30.000000 libgzipf-20240103/gzipftools/gzipftools_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1213 2024-01-03 04:40:30.000000 libgzipf-20240103/gzipftools/gzipftools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1409 2024-01-03 04:40:30.000000 libgzipf-20240103/gzipftools/gzipftools_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20758 2024-01-03 04:43:34.000000 libgzipf-20240103/gzipftools/mount_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16724 2024-01-03 04:43:34.000000 libgzipf-20240103/gzipftools/info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5854 2024-01-03 04:43:34.000000 libgzipf-20240103/gzipftools/gzipfinfo.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3617 2024-01-03 04:43:34.000000 libgzipf-20240103/gzipftools/mount_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5751 2024-01-03 04:40:30.000000 libgzipf-20240103/gzipftools/gzipftools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2261 2024-01-03 04:40:30.000000 libgzipf-20240103/gzipftools/mount_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1761 2024-01-03 04:40:30.000000 libgzipf-20240103/gzipftools/gzipftools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-01-03 04:40:30.000000 libgzipf-20240103/gzipftools/gzipftools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-01-03 04:40:30.000000 libgzipf-20240103/gzipftools/gzipftools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11979 2024-01-03 04:43:34.000000 libgzipf-20240103/gzipftools/mount_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2024-01-03 04:40:30.000000 libgzipf-20240103/gzipftools/gzipftools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-01-03 04:40:30.000000 libgzipf-20240103/gzipftools/gzipftools_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-01-03 04:40:30.000000 libgzipf-20240103/gzipftools/gzipftools_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-01-03 04:40:30.000000 libgzipf-20240103/gzipftools/gzipftools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33604 2024-01-03 05:12:40.000000 libgzipf-20240103/gzipftools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3982 2024-01-03 04:40:30.000000 libgzipf-20240103/gzipftools/gzipftools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1483 2024-01-03 04:40:30.000000 libgzipf-20240103/gzipftools/gzipftools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2765 2024-01-03 04:40:30.000000 libgzipf-20240103/gzipftools/mount_fuse.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:27.000000 libgzipf-20240103/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18233 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/libfdatetime.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-01-03 05:12:35.000000 libgzipf-20240103/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-01-03 05:12:35.000000 libgzipf-20240103/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15545 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/libfdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5232 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/libfuse.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-01-03 05:12:35.000000 libgzipf-20240103/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/libbfio.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-01-03 05:12:35.000000 libgzipf-20240103/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-01-03 05:12:35.000000 libgzipf-20240103/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-18 04:33:12.000000 libgzipf-20240103/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7325 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/libfcache.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/pthread.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7383 2023-12-03 09:10:02.000000 libgzipf-20240103/m4/zlib.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:27.000000 libgzipf-20240103/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12865 2024-01-03 04:40:30.000000 libgzipf-20240103/include/libgzipf.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      474 2024-01-03 04:40:29.000000 libgzipf-20240103/include/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:27.000000 libgzipf-20240103/include/libgzipf/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1677 2024-01-03 04:40:30.000000 libgzipf-20240103/include/libgzipf/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1675 2024-01-03 05:12:48.000000 libgzipf-20240103/include/libgzipf/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4978 2024-01-03 04:40:30.000000 libgzipf-20240103/include/libgzipf/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4847 2024-01-03 05:12:48.000000 libgzipf-20240103/include/libgzipf/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-01-03 04:40:30.000000 libgzipf-20240103/include/libgzipf/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2024-01-03 04:40:30.000000 libgzipf-20240103/include/libgzipf/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-01-03 04:40:30.000000 libgzipf-20240103/include/libgzipf/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1487 2024-01-03 05:12:48.000000 libgzipf-20240103/include/libgzipf/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5306 2024-01-03 04:40:30.000000 libgzipf-20240103/include/libgzipf/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12865 2024-01-03 05:12:48.000000 libgzipf-20240103/include/libgzipf.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27556 2024-01-03 05:12:40.000000 libgzipf-20240103/include/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:27.000000 libgzipf-20240103/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-01-03 04:40:29.000000 libgzipf-20240103/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-01-03 04:40:29.000000 libgzipf-20240103/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-01-03 04:40:29.000000 libgzipf-20240103/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-01-03 04:40:29.000000 libgzipf-20240103/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-01-03 04:40:29.000000 libgzipf-20240103/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-01-03 04:40:29.000000 libgzipf-20240103/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-01-03 04:40:29.000000 libgzipf-20240103/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-01-03 04:40:29.000000 libgzipf-20240103/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-01-03 04:40:29.000000 libgzipf-20240103/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7374 2024-01-03 05:12:48.000000 libgzipf-20240103/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16627 2024-01-03 05:12:39.000000 libgzipf-20240103/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17609 2024-01-03 05:12:48.000000 libgzipf-20240103/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-01-03 04:40:29.000000 libgzipf-20240103/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-01-03 04:40:29.000000 libgzipf-20240103/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-01-03 04:40:29.000000 libgzipf-20240103/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24563 2024-01-03 05:12:39.000000 libgzipf-20240103/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:28.000000 libgzipf-20240103/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-01-03 05:12:19.000000 libgzipf-20240103/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-01-03 05:12:19.000000 libgzipf-20240103/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      744 2024-01-03 05:12:19.000000 libgzipf-20240103/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-01-03 05:12:19.000000 libgzipf-20240103/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-01-03 05:12:19.000000 libgzipf-20240103/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-01-03 05:12:19.000000 libgzipf-20240103/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-01-03 05:12:19.000000 libgzipf-20240103/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3094 2024-01-03 05:12:19.000000 libgzipf-20240103/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-01-03 05:12:19.000000 libgzipf-20240103/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-01-03 05:12:19.000000 libgzipf-20240103/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29519 2024-01-03 05:12:40.000000 libgzipf-20240103/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-01-03 05:12:19.000000 libgzipf-20240103/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-01-03 05:12:19.000000 libgzipf-20240103/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-01-03 05:12:19.000000 libgzipf-20240103/libclocale/libclocale_codepage.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:28.000000 libgzipf-20240103/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-01-03 05:12:25.000000 libgzipf-20240103/libfcache/libfcache_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-01-03 05:12:25.000000 libgzipf-20240103/libfcache/libfcache_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-01-03 05:12:25.000000 libgzipf-20240103/libfcache/libfcache_cache_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-01-03 05:12:25.000000 libgzipf-20240103/libfcache/libfcache_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      845 2024-01-03 05:12:25.000000 libgzipf-20240103/libfcache/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-01-03 05:12:25.000000 libgzipf-20240103/libfcache/libfcache_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-01-03 05:12:25.000000 libgzipf-20240103/libfcache/libfcache_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-01-03 05:12:25.000000 libgzipf-20240103/libfcache/libfcache_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-01-03 05:12:25.000000 libgzipf-20240103/libfcache/libfcache_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-01-03 05:12:25.000000 libgzipf-20240103/libfcache/libfcache_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-01-03 05:12:25.000000 libgzipf-20240103/libfcache/libfcache_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-01-03 05:12:25.000000 libgzipf-20240103/libfcache/libfcache_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-01-03 05:12:25.000000 libgzipf-20240103/libfcache/libfcache_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-01-03 05:12:25.000000 libgzipf-20240103/libfcache/libfcache_cache_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29992 2024-01-03 05:12:40.000000 libgzipf-20240103/libfcache/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-01-03 05:12:25.000000 libgzipf-20240103/libfcache/libfcache_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-01-03 05:12:25.000000 libgzipf-20240103/libfcache/libfcache_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-01-03 05:12:25.000000 libgzipf-20240103/libfcache/libfcache_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2228 2023-12-18 04:50:23.000000 libgzipf-20240103/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:28.000000 libgzipf-20240103/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33025 2024-01-03 05:12:40.000000 libgzipf-20240103/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-01-03 05:12:14.000000 libgzipf-20240103/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:09:53.000000 libgzipf-20240103/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-01-03 05:12:39.000000 libgzipf-20240103/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:27.000000 libgzipf-20240103/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1026 2024-01-03 04:40:30.000000 libgzipf-20240103/dpkg/copyright
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:27.000000 libgzipf-20240103/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-01-03 04:40:29.000000 libgzipf-20240103/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-01-03 04:40:29.000000 libgzipf-20240103/dpkg/libgzipf-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-01-03 04:40:29.000000 libgzipf-20240103/dpkg/libgzipf-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2063 2024-01-03 04:40:29.000000 libgzipf-20240103/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-01-03 04:40:29.000000 libgzipf-20240103/dpkg/libgzipf.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      769 2024-01-03 04:40:29.000000 libgzipf-20240103/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      121 2024-01-03 04:40:29.000000 libgzipf-20240103/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2024-01-03 05:12:48.000000 libgzipf-20240103/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-01-03 04:40:29.000000 libgzipf-20240103/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-01-03 04:40:29.000000 libgzipf-20240103/dpkg/libgzipf-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      486 2024-01-03 05:12:48.000000 libgzipf-20240103/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2340 2024-01-03 05:12:48.000000 libgzipf-20240103/libgzipf.spec
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-01-03 04:40:29.000000 libgzipf-20240103/COPYING.LESSER
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      690 2024-01-03 04:40:29.000000 libgzipf-20240103/libgzipf.pc.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1825437 2024-01-03 05:12:38.000000 libgzipf-20240103/configure
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:28.000000 libgzipf-20240103/libgzipf/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12520 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_huffman_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1071 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2280 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_bit_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8516 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2094 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_huffman_tree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14909 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_member_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2722 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2655 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3703 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1587 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3728 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_member.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1726 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2048 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_segment_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2453 2023-12-03 09:09:53.000000 libgzipf-20240103/libgzipf/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1069 2024-01-03 05:12:48.000000 libgzipf-20240103/libgzipf/libgzipf.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1316 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/gzipf_member_footer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    89920 2024-01-03 05:05:10.000000 libgzipf-20240103/libgzipf/libgzipf_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23484 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_member.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9597 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4109 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_member_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19792 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_compressed_segment.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_member_footer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1587 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1670 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_checksum.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2063 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2028 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7930 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_bit_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2863 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_compressed_segment.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19704 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_member_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1814 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9337 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7048 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_member_footer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48890 2024-01-03 04:43:34.000000 libgzipf-20240103/libgzipf/libgzipf_deflate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3488 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_deflate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35965 2024-01-03 05:12:40.000000 libgzipf-20240103/libgzipf/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2720 2024-01-03 05:12:48.000000 libgzipf-20240103/libgzipf/libgzipf_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/gzipf_member_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4882 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_checksum.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2484 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_member_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3570 2024-01-03 04:40:30.000000 libgzipf-20240103/libgzipf/libgzipf_segment_descriptor.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-01-03 05:12:39.000000 libgzipf-20240103/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-01-03 05:12:39.000000 libgzipf-20240103/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-01-03 04:40:48.000000 libgzipf-20240103/msvscpp/libfdata/libfdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/gzipf_test_tools_output/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5703 2024-01-03 04:43:04.000000 libgzipf-20240103/msvscpp/gzipf_test_tools_output/gzipf_test_tools_output.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/gzipf_test_checksum/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5683 2024-01-03 04:43:04.000000 libgzipf-20240103/msvscpp/gzipf_test_checksum/gzipf_test_checksum.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/gzipf_test_tools_signal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5703 2024-01-03 04:43:04.000000 libgzipf-20240103/msvscpp/gzipf_test_tools_signal/gzipf_test_tools_signal.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/gzipf_test_deflate/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5684 2024-01-03 04:43:04.000000 libgzipf-20240103/msvscpp/gzipf_test_deflate/gzipf_test_deflate.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/zlib/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6068 2024-01-03 04:40:49.000000 libgzipf-20240103/msvscpp/zlib/zlib.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/gzipf_test_tools_info_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5868 2024-01-03 04:43:04.000000 libgzipf-20240103/msvscpp/gzipf_test_tools_info_handle/gzipf_test_tools_info_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/gzipf_test_huffman_tree/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5776 2024-01-03 04:43:04.000000 libgzipf-20240103/msvscpp/gzipf_test_huffman_tree/gzipf_test_huffman_tree.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-01-03 04:40:49.000000 libgzipf-20240103/msvscpp/libclocale/libclocale.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-01-03 04:40:49.000000 libgzipf-20240103/msvscpp/libfcache/libfcache.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-01-03 04:43:04.000000 libgzipf-20240103/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/gzipf_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6424 2024-01-03 04:43:04.000000 libgzipf-20240103/msvscpp/gzipf_test_support/gzipf_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-01-03 04:40:49.000000 libgzipf-20240103/msvscpp/libbfio/libbfio.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/gzipf_test_compressed_segment/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5794 2024-01-03 04:43:04.000000 libgzipf-20240103/msvscpp/gzipf_test_compressed_segment/gzipf_test_compressed_segment.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/libgzipf/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9444 2024-01-03 04:40:49.000000 libgzipf-20240103/msvscpp/libgzipf/libgzipf.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/gzipf_test_bit_stream/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5770 2024-01-03 04:43:04.000000 libgzipf-20240103/msvscpp/gzipf_test_bit_stream/gzipf_test_bit_stream.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-01-03 04:40:49.000000 libgzipf-20240103/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/gzipf_test_member_footer/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6029 2024-01-03 04:43:04.000000 libgzipf-20240103/msvscpp/gzipf_test_member_footer/gzipf_test_member_footer.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/gzipf_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5767 2024-01-03 04:43:04.000000 libgzipf-20240103/msvscpp/gzipf_test_io_handle/gzipf_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-01-03 04:40:49.000000 libgzipf-20240103/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/gzipf_test_member/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5758 2024-01-03 04:43:04.000000 libgzipf-20240103/msvscpp/gzipf_test_member/gzipf_test_member.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-01-03 04:40:49.000000 libgzipf-20240103/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/gzipf_test_file/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6415 2024-01-03 04:43:04.000000 libgzipf-20240103/msvscpp/gzipf_test_file/gzipf_test_file.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/gzipf_test_member_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6029 2024-01-03 04:43:04.000000 libgzipf-20240103/msvscpp/gzipf_test_member_header/gzipf_test_member_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-01-03 04:40:49.000000 libgzipf-20240103/msvscpp/libcpath/libcpath.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/gzipfinfo/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6490 2024-01-03 04:40:48.000000 libgzipf-20240103/msvscpp/gzipfinfo/gzipfinfo.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/gzipf_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5596 2024-01-03 04:43:04.000000 libgzipf-20240103/msvscpp/gzipf_test_notify/gzipf_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-01-03 04:40:49.000000 libgzipf-20240103/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/pygzipf/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6695 2024-01-03 04:43:04.000000 libgzipf-20240103/msvscpp/pygzipf/pygzipf.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/gzipf_test_member_descriptor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5791 2024-01-03 04:43:04.000000 libgzipf-20240103/msvscpp/gzipf_test_member_descriptor/gzipf_test_member_descriptor.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-01-03 04:40:49.000000 libgzipf-20240103/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23124 2024-01-03 05:12:40.000000 libgzipf-20240103/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-01-03 04:40:49.000000 libgzipf-20240103/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-01-03 04:40:49.000000 libgzipf-20240103/msvscpp/libcerror/libcerror.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31425 2024-01-03 04:43:04.000000 libgzipf-20240103/msvscpp/libgzipf.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/gzipfmount/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7477 2024-01-03 04:40:49.000000 libgzipf-20240103/msvscpp/gzipfmount/gzipfmount.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-01-03 04:40:49.000000 libgzipf-20240103/msvscpp/libfdatetime/libfdatetime.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/msvscpp/gzipf_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5509 2024-01-03 04:43:04.000000 libgzipf-20240103/msvscpp/gzipf_test_error/gzipf_test_error.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       92 2024-01-03 04:40:29.000000 libgzipf-20240103/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:28.000000 libgzipf-20240103/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-01-03 05:12:18.000000 libgzipf-20240103/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-01-03 05:12:18.000000 libgzipf-20240103/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-01-03 05:12:18.000000 libgzipf-20240103/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-01-03 05:12:18.000000 libgzipf-20240103/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-01-03 05:12:18.000000 libgzipf-20240103/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-01-03 05:12:18.000000 libgzipf-20240103/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      907 2024-01-03 05:12:18.000000 libgzipf-20240103/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-01-03 05:12:18.000000 libgzipf-20240103/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-01-03 05:12:18.000000 libgzipf-20240103/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-01-03 05:12:18.000000 libgzipf-20240103/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-01-03 05:12:18.000000 libgzipf-20240103/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-01-03 05:12:18.000000 libgzipf-20240103/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-01-03 05:12:18.000000 libgzipf-20240103/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-01-03 05:12:18.000000 libgzipf-20240103/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-01-03 05:12:18.000000 libgzipf-20240103/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-01-03 05:12:18.000000 libgzipf-20240103/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-01-03 05:12:18.000000 libgzipf-20240103/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30283 2024-01-03 05:12:40.000000 libgzipf-20240103/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-01-03 05:12:18.000000 libgzipf-20240103/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-01-03 05:12:18.000000 libgzipf-20240103/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-01-03 05:12:18.000000 libgzipf-20240103/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-01-03 05:12:18.000000 libgzipf-20240103/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      295 2024-01-03 04:40:29.000000 libgzipf-20240103/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-01-03 05:12:39.000000 libgzipf-20240103/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:28.000000 libgzipf-20240103/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32014 2024-01-03 05:12:40.000000 libgzipf-20240103/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-01-03 05:12:15.000000 libgzipf-20240103/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-01-03 04:40:29.000000 libgzipf-20240103/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      487 2024-01-03 04:40:29.000000 libgzipf-20240103/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-01-03 05:12:39.000000 libgzipf-20240103/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-01-03 04:40:29.000000 libgzipf-20240103/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1508 2024-01-03 04:40:29.000000 libgzipf-20240103/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:09:53.000000 libgzipf-20240103/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:28.000000 libgzipf-20240103/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32420 2024-01-03 05:12:40.000000 libgzipf-20240103/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-01-03 05:12:24.000000 libgzipf-20240103/libcthreads/libcthreads_queue.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-01-03 05:12:40.000000 libgzipf-20240103/test-driver
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:28.000000 libgzipf-20240103/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-01-03 05:12:21.000000 libgzipf-20240103/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-01-03 05:12:21.000000 libgzipf-20240103/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-01-03 05:12:21.000000 libgzipf-20240103/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      807 2024-01-03 05:12:21.000000 libgzipf-20240103/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-01-03 05:12:21.000000 libgzipf-20240103/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-01-03 05:12:21.000000 libgzipf-20240103/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-01-03 05:12:21.000000 libgzipf-20240103/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-01-03 05:12:21.000000 libgzipf-20240103/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-01-03 05:12:21.000000 libgzipf-20240103/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-01-03 05:12:21.000000 libgzipf-20240103/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-01-03 05:12:21.000000 libgzipf-20240103/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-01-03 05:12:21.000000 libgzipf-20240103/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29561 2024-01-03 05:12:40.000000 libgzipf-20240103/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-01-03 05:12:21.000000 libgzipf-20240103/libcpath/libcpath_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-01-03 05:12:21.000000 libgzipf-20240103/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-01-03 05:12:21.000000 libgzipf-20240103/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-01-03 05:12:21.000000 libgzipf-20240103/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      206 2023-12-03 09:09:54.000000 libgzipf-20240103/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1255 2024-01-03 04:40:30.000000 libgzipf-20240103/manuals/gzipfinfo.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      158 2023-12-03 09:10:06.000000 libgzipf-20240103/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26533 2024-01-03 05:12:40.000000 libgzipf-20240103/manuals/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6086 2024-01-03 04:40:30.000000 libgzipf-20240103/manuals/libgzipf.3
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28883 2024-01-03 04:43:04.000000 libgzipf-20240103/tests/gzipf_test_member_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4146 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/gzipf_test_checksum.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57012 2024-01-03 04:43:04.000000 libgzipf-20240103/tests/gzipf_test_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/gzipf_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100638 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/gzipf_test_deflate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12829 2024-01-03 04:43:04.000000 libgzipf-20240103/tests/gzipf_test_member_footer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1812 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/gzipf_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8056 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/gzipf_test_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/gzipf_test_libgzipf.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4068 2024-01-03 04:43:34.000000 libgzipf-20240103/tests/test_tools.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3139 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/gzipf_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/gzipf_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13779 2024-01-03 04:43:04.000000 libgzipf-20240103/tests/gzipf_test_bit_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4169 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/gzipf_test_tools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15093 2024-01-03 04:43:04.000000 libgzipf-20240103/tests/gzipf_test_member_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/gzipf_test_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2447 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/gzipf_test_tools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/gzipf_test_memory.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3320 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/test_gzipfinfo.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7331 2024-01-03 04:43:04.000000 libgzipf-20240103/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4323 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/gzipf_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11372 2024-01-03 04:45:36.000000 libgzipf-20240103/tests/pygzipf_test_file.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2345 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/pygzipf_test_support.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/test_manpage.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3829 2024-01-03 04:49:57.000000 libgzipf-20240103/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8574 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/gzipf_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3124 2024-01-03 04:43:04.000000 libgzipf-20240103/tests/gzipf_test_member.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14367 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/gzipf_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/gzipf_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/gzipf_test_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/gzipf_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5634 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/gzipf_test_tools_info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1709 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/gzipf_test_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2866 2024-01-03 04:43:04.000000 libgzipf-20240103/tests/gzipf_test_compressed_segment.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64421 2024-01-03 05:12:40.000000 libgzipf-20240103/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/gzipf_test_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13259 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/gzipf_test_functions.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30822 2024-01-03 04:43:04.000000 libgzipf-20240103/tests/gzipf_test_huffman_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-01-03 04:40:30.000000 libgzipf-20240103/tests/gzipf_test_memory.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4188 2024-01-03 04:43:34.000000 libgzipf-20240103/tests/test_library.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      892 2023-12-03 09:09:55.000000 libgzipf-20240103/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      972 2024-01-03 04:40:30.000000 libgzipf-20240103/ossfuzz/ossfuzz_libgzipf.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-01-03 04:40:30.000000 libgzipf-20240103/ossfuzz/ossfuzz_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2214 2024-01-03 04:40:30.000000 libgzipf-20240103/ossfuzz/file_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31768 2024-01-03 05:12:40.000000 libgzipf-20240103/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3254 2024-01-03 04:40:29.000000 libgzipf-20240103/libgzipf.spec.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-01-03 05:12:35.000000 libgzipf-20240103/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:28.000000 libgzipf-20240103/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-01-03 05:12:22.000000 libgzipf-20240103/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-01-03 05:12:22.000000 libgzipf-20240103/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-01-03 05:12:22.000000 libgzipf-20240103/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-01-03 05:12:22.000000 libgzipf-20240103/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-01-03 05:12:22.000000 libgzipf-20240103/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      849 2024-01-03 05:12:22.000000 libgzipf-20240103/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-01-03 05:12:22.000000 libgzipf-20240103/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-01-03 05:12:22.000000 libgzipf-20240103/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-01-03 05:12:22.000000 libgzipf-20240103/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-01-03 05:12:22.000000 libgzipf-20240103/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-01-03 05:12:22.000000 libgzipf-20240103/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-01-03 05:12:22.000000 libgzipf-20240103/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-01-03 05:12:22.000000 libgzipf-20240103/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-01-03 05:12:22.000000 libgzipf-20240103/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-01-03 05:12:22.000000 libgzipf-20240103/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-01-03 05:12:22.000000 libgzipf-20240103/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30341 2024-01-03 05:12:40.000000 libgzipf-20240103/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-01-03 05:12:22.000000 libgzipf-20240103/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-01-03 05:12:22.000000 libgzipf-20240103/libcsplit/libcsplit_narrow_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:28.000000 libgzipf-20240103/pygzipf/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2335 2024-01-03 04:40:30.000000 libgzipf-20240103/pygzipf/pygzipf_member.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14794 2024-01-03 04:40:30.000000 libgzipf-20240103/pygzipf/pygzipf.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-01-03 04:40:30.000000 libgzipf-20240103/pygzipf/pygzipf_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2024-01-03 04:40:30.000000 libgzipf-20240103/pygzipf/pygzipf_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2033 2024-01-03 04:40:30.000000 libgzipf-20240103/pygzipf/pygzipf_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8876 2024-01-03 04:40:30.000000 libgzipf-20240103/pygzipf/pygzipf_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1860 2024-01-03 04:40:30.000000 libgzipf-20240103/pygzipf/pygzipf.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3278 2024-01-03 04:43:34.000000 libgzipf-20240103/pygzipf/pygzipf_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:10:01.000000 libgzipf-20240103/pygzipf/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-01-03 04:40:30.000000 libgzipf-20240103/pygzipf/pygzipf_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-01-03 04:40:30.000000 libgzipf-20240103/pygzipf/pygzipf_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15417 2024-01-03 04:43:34.000000 libgzipf-20240103/pygzipf/pygzipf_member.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33880 2024-01-03 04:40:30.000000 libgzipf-20240103/pygzipf/pygzipf_file_object_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-01-03 04:40:30.000000 libgzipf-20240103/pygzipf/pygzipf_libgzipf.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1826 2024-01-03 04:40:30.000000 libgzipf-20240103/pygzipf/pygzipf_datetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9143 2024-01-03 04:40:30.000000 libgzipf-20240103/pygzipf/pygzipf_members.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3290 2024-01-03 04:40:30.000000 libgzipf-20240103/pygzipf/pygzipf_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9546 2024-01-03 04:40:30.000000 libgzipf-20240103/pygzipf/pygzipf_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-01-03 04:40:30.000000 libgzipf-20240103/pygzipf/pygzipf_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4118 2024-01-03 04:40:30.000000 libgzipf-20240103/pygzipf/pygzipf_file_object_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2024-01-03 04:40:30.000000 libgzipf-20240103/pygzipf/pygzipf_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44863 2024-01-03 05:12:40.000000 libgzipf-20240103/pygzipf/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-01-03 04:40:30.000000 libgzipf-20240103/pygzipf/pygzipf_members.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34430 2024-01-03 04:43:34.000000 libgzipf-20240103/pygzipf/pygzipf_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16609 2024-01-03 04:40:30.000000 libgzipf-20240103/pygzipf/pygzipf_datetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1525 2024-01-03 04:40:30.000000 libgzipf-20240103/pygzipf/pygzipf_libbfio.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:29.000000 libgzipf-20240103/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:10:06.000000 libgzipf-20240103/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:10:06.000000 libgzipf-20240103/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:10:06.000000 libgzipf-20240103/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:10:06.000000 libgzipf-20240103/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:10:06.000000 libgzipf-20240103/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:10:06.000000 libgzipf-20240103/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:10:06.000000 libgzipf-20240103/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:10:06.000000 libgzipf-20240103/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:10:06.000000 libgzipf-20240103/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1854 2024-01-03 05:12:48.000000 libgzipf-20240103/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:10:06.000000 libgzipf-20240103/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:10:06.000000 libgzipf-20240103/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:28.000000 libgzipf-20240103/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4162 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-01-03 05:12:40.000000 libgzipf-20240103/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-01-03 05:12:31.000000 libgzipf-20240103/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40563 2024-01-03 05:12:39.000000 libgzipf-20240103/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:28.000000 libgzipf-20240103/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-01-03 05:12:20.000000 libgzipf-20240103/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-01-03 05:12:20.000000 libgzipf-20240103/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-01-03 05:12:20.000000 libgzipf-20240103/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-01-03 05:12:20.000000 libgzipf-20240103/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      693 2024-01-03 05:12:20.000000 libgzipf-20240103/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-01-03 05:12:20.000000 libgzipf-20240103/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-01-03 05:12:20.000000 libgzipf-20240103/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-01-03 05:12:20.000000 libgzipf-20240103/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-01-03 05:12:20.000000 libgzipf-20240103/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-01-03 05:12:20.000000 libgzipf-20240103/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-01-03 05:12:20.000000 libgzipf-20240103/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29395 2024-01-03 05:12:40.000000 libgzipf-20240103/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-01-03 05:12:20.000000 libgzipf-20240103/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-01-03 05:12:20.000000 libgzipf-20240103/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:28.000000 libgzipf-20240103/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-01-03 05:12:16.000000 libgzipf-20240103/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-01-03 05:12:16.000000 libgzipf-20240103/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-01-03 05:12:16.000000 libgzipf-20240103/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-01-03 05:12:16.000000 libgzipf-20240103/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-01-03 05:12:16.000000 libgzipf-20240103/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-01-03 05:12:16.000000 libgzipf-20240103/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-01-03 05:12:16.000000 libgzipf-20240103/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-01-03 05:12:16.000000 libgzipf-20240103/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-01-03 05:12:16.000000 libgzipf-20240103/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-01-03 05:12:16.000000 libgzipf-20240103/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-01-03 05:12:16.000000 libgzipf-20240103/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28955 2024-01-03 05:12:40.000000 libgzipf-20240103/libcerror/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-03 05:25:28.000000 libgzipf-20240103/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-01-03 05:12:27.000000 libgzipf-20240103/libfdatetime/libfdatetime_floatingtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-01-03 05:12:27.000000 libgzipf-20240103/libfdatetime/libfdatetime_nsf_timedate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-01-03 05:12:27.000000 libgzipf-20240103/libfdatetime/libfdatetime_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-01-03 05:12:27.000000 libgzipf-20240103/libfdatetime/libfdatetime_floatingtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-01-03 05:12:27.000000 libgzipf-20240103/libfdatetime/libfdatetime_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-01-03 05:12:27.000000 libgzipf-20240103/libfdatetime/libfdatetime_hfs_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-01-03 05:12:27.000000 libgzipf-20240103/libfdatetime/libfdatetime_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-01-03 05:12:27.000000 libgzipf-20240103/libfdatetime/libfdatetime_hfs_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1113 2024-01-03 05:12:27.000000 libgzipf-20240103/libfdatetime/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-01-03 05:12:27.000000 libgzipf-20240103/libfdatetime/libfdatetime_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-01-03 05:12:27.000000 libgzipf-20240103/libfdatetime/libfdatetime_systemtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-01-03 05:12:27.000000 libgzipf-20240103/libfdatetime/libfdatetime_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-01-03 05:12:27.000000 libgzipf-20240103/libfdatetime/libfdatetime_posix_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-01-03 05:12:27.000000 libgzipf-20240103/libfdatetime/libfdatetime_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-01-03 05:12:27.000000 libgzipf-20240103/libfdatetime/libfdatetime_fat_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-01-03 05:12:27.000000 libgzipf-20240103/libfdatetime/libfdatetime_systemtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-01-03 05:12:27.000000 libgzipf-20240103/libfdatetime/libfdatetime_nsf_timedate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-01-03 05:12:27.000000 libgzipf-20240103/libfdatetime/libfdatetime_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-01-03 05:12:27.000000 libgzipf-20240103/libfdatetime/libfdatetime_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-01-03 05:12:27.000000 libgzipf-20240103/libfdatetime/libfdatetime_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-01-03 05:12:27.000000 libgzipf-20240103/libfdatetime/libfdatetime_posix_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-01-03 05:12:27.000000 libgzipf-20240103/libfdatetime/libfdatetime_date_time_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-01-03 05:12:27.000000 libgzipf-20240103/libfdatetime/libfdatetime_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-01-03 05:12:27.000000 libgzipf-20240103/libfdatetime/libfdatetime_date_time_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-01-03 05:12:27.000000 libgzipf-20240103/libfdatetime/libfdatetime_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32134 2024-01-03 05:12:40.000000 libgzipf-20240103/libfdatetime/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-01-03 05:12:27.000000 libgzipf-20240103/libfdatetime/libfdatetime_fat_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56822 2024-01-03 05:12:37.000000 libgzipf-20240103/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7711 2024-01-03 04:40:29.000000 libgzipf-20240103/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      418 2024-01-03 05:25:29.937366 libgzipf-20240103/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:00.000000 libgzipf-20240422/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_area.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_mapped_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1287 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_area.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_mapped_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_segments_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_segments_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33415 2024-04-22 04:49:40.000000 libgzipf-20240422/libfdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-04-22 04:49:25.000000 libgzipf-20240422/libfdata/libfdata_vector.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-04-22 04:19:33.000000 libgzipf-20240422/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-04-22 04:49:39.000000 libgzipf-20240422/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 04:19:33.000000 libgzipf-20240422/NEWS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-04-22 04:49:40.000000 libgzipf-20240422/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:00.000000 libgzipf-20240422/gzipftools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15357 2024-04-22 04:21:03.000000 libgzipf-20240422/gzipftools/gzipfmount.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1472 2024-04-22 04:19:38.000000 libgzipf-20240422/gzipftools/gzipftools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37205 2024-04-22 04:19:38.000000 libgzipf-20240422/gzipftools/mount_dokan.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2983 2024-04-22 04:21:03.000000 libgzipf-20240422/gzipftools/mount_file_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26459 2024-04-22 04:21:03.000000 libgzipf-20240422/gzipftools/mount_fuse.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2285 2024-04-22 04:21:03.000000 libgzipf-20240422/gzipftools/info_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5417 2024-04-22 04:19:38.000000 libgzipf-20240422/gzipftools/mount_dokan.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18940 2024-04-22 04:21:03.000000 libgzipf-20240422/gzipftools/mount_file_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-04-22 04:19:38.000000 libgzipf-20240422/gzipftools/gzipftools_libgzipf.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-04-22 04:19:38.000000 libgzipf-20240422/gzipftools/gzipftools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2188 2024-04-22 04:26:08.000000 libgzipf-20240422/gzipftools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-04-22 04:19:38.000000 libgzipf-20240422/gzipftools/gzipftools_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1771 2024-04-22 04:19:38.000000 libgzipf-20240422/gzipftools/gzipftools_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1213 2024-04-22 04:19:38.000000 libgzipf-20240422/gzipftools/gzipftools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1409 2024-04-22 04:19:38.000000 libgzipf-20240422/gzipftools/gzipftools_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20758 2024-04-22 04:21:03.000000 libgzipf-20240422/gzipftools/mount_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16724 2024-04-22 04:21:03.000000 libgzipf-20240422/gzipftools/info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5854 2024-04-22 04:21:03.000000 libgzipf-20240422/gzipftools/gzipfinfo.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3617 2024-04-22 04:21:03.000000 libgzipf-20240422/gzipftools/mount_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5751 2024-04-22 04:19:38.000000 libgzipf-20240422/gzipftools/gzipftools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2261 2024-04-22 04:19:38.000000 libgzipf-20240422/gzipftools/mount_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1761 2024-04-22 04:19:38.000000 libgzipf-20240422/gzipftools/gzipftools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-22 04:19:38.000000 libgzipf-20240422/gzipftools/gzipftools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2024-04-22 04:19:38.000000 libgzipf-20240422/gzipftools/gzipftools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11979 2024-04-22 04:21:03.000000 libgzipf-20240422/gzipftools/mount_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2024-04-22 04:19:38.000000 libgzipf-20240422/gzipftools/gzipftools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1554 2024-04-22 04:19:38.000000 libgzipf-20240422/gzipftools/gzipftools_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-04-22 04:19:38.000000 libgzipf-20240422/gzipftools/gzipftools_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-04-22 04:19:38.000000 libgzipf-20240422/gzipftools/gzipftools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34097 2024-04-22 04:49:39.000000 libgzipf-20240422/gzipftools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3982 2024-04-22 04:19:38.000000 libgzipf-20240422/gzipftools/gzipftools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1483 2024-04-22 04:19:38.000000 libgzipf-20240422/gzipftools/gzipftools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2765 2024-04-22 04:21:03.000000 libgzipf-20240422/gzipftools/mount_fuse.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:08:57.000000 libgzipf-20240422/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11734 2024-04-22 04:19:39.000000 libgzipf-20240422/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18489 2024-04-22 04:19:39.000000 libgzipf-20240422/m4/libfdatetime.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:10:02.000000 libgzipf-20240422/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9615 2024-04-22 04:19:39.000000 libgzipf-20240422/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:10:02.000000 libgzipf-20240422/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:10:02.000000 libgzipf-20240422/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-04-22 04:19:39.000000 libgzipf-20240422/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:10:02.000000 libgzipf-20240422/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:10:02.000000 libgzipf-20240422/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-04-22 04:19:39.000000 libgzipf-20240422/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-04-22 04:19:39.000000 libgzipf-20240422/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7625 2024-04-22 04:19:39.000000 libgzipf-20240422/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-04-22 04:19:39.000000 libgzipf-20240422/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-04-22 04:19:39.000000 libgzipf-20240422/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-04-22 04:49:34.000000 libgzipf-20240422/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-04-22 04:49:34.000000 libgzipf-20240422/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15781 2024-04-22 04:19:39.000000 libgzipf-20240422/m4/libfdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:10:02.000000 libgzipf-20240422/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7058 2024-04-22 04:19:39.000000 libgzipf-20240422/m4/libfuse.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-04-22 04:49:34.000000 libgzipf-20240422/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:10:02.000000 libgzipf-20240422/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-04-22 04:19:39.000000 libgzipf-20240422/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-04-22 04:19:39.000000 libgzipf-20240422/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11923 2024-04-22 04:19:39.000000 libgzipf-20240422/m4/libbfio.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:10:02.000000 libgzipf-20240422/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-04-22 04:49:34.000000 libgzipf-20240422/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:10:02.000000 libgzipf-20240422/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:10:02.000000 libgzipf-20240422/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-04-22 04:49:34.000000 libgzipf-20240422/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:10:02.000000 libgzipf-20240422/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-04-22 04:19:39.000000 libgzipf-20240422/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:10:02.000000 libgzipf-20240422/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7566 2024-04-22 04:19:39.000000 libgzipf-20240422/m4/libfcache.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-04-22 04:19:39.000000 libgzipf-20240422/m4/pthread.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7819 2024-04-22 04:19:39.000000 libgzipf-20240422/m4/zlib.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:08:57.000000 libgzipf-20240422/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12865 2024-04-22 04:19:36.000000 libgzipf-20240422/include/libgzipf.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      425 2024-04-22 04:25:54.000000 libgzipf-20240422/include/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:08:57.000000 libgzipf-20240422/include/libgzipf/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1677 2024-04-22 04:19:36.000000 libgzipf-20240422/include/libgzipf/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1675 2024-04-22 04:49:58.000000 libgzipf-20240422/include/libgzipf/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4978 2024-04-22 04:19:36.000000 libgzipf-20240422/include/libgzipf/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4847 2024-04-22 04:49:58.000000 libgzipf-20240422/include/libgzipf/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-04-22 04:19:36.000000 libgzipf-20240422/include/libgzipf/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2024-04-22 04:19:36.000000 libgzipf-20240422/include/libgzipf/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-22 04:19:36.000000 libgzipf-20240422/include/libgzipf/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1487 2024-04-22 04:49:58.000000 libgzipf-20240422/include/libgzipf/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5306 2024-04-22 04:19:36.000000 libgzipf-20240422/include/libgzipf/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12865 2024-04-22 04:49:58.000000 libgzipf-20240422/include/libgzipf.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27592 2024-04-22 04:49:39.000000 libgzipf-20240422/include/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:08:57.000000 libgzipf-20240422/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-04-22 04:19:36.000000 libgzipf-20240422/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-04-22 04:19:36.000000 libgzipf-20240422/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-04-22 04:19:36.000000 libgzipf-20240422/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-04-22 04:19:36.000000 libgzipf-20240422/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-22 04:19:36.000000 libgzipf-20240422/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-04-22 04:19:36.000000 libgzipf-20240422/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-04-22 04:19:36.000000 libgzipf-20240422/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-04-22 04:25:54.000000 libgzipf-20240422/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-04-22 04:19:36.000000 libgzipf-20240422/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7374 2024-04-22 04:49:58.000000 libgzipf-20240422/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16710 2024-04-22 04:49:39.000000 libgzipf-20240422/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17698 2024-04-22 04:49:58.000000 libgzipf-20240422/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-04-22 04:19:36.000000 libgzipf-20240422/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-04-22 04:19:36.000000 libgzipf-20240422/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-04-22 04:19:36.000000 libgzipf-20240422/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24626 2024-04-22 04:49:39.000000 libgzipf-20240422/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:08:58.000000 libgzipf-20240422/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-04-22 04:49:17.000000 libgzipf-20240422/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-04-22 04:49:17.000000 libgzipf-20240422/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-04-22 04:49:17.000000 libgzipf-20240422/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-04-22 04:49:17.000000 libgzipf-20240422/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-22 04:49:17.000000 libgzipf-20240422/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-22 04:49:17.000000 libgzipf-20240422/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-04-22 04:49:17.000000 libgzipf-20240422/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-04-22 04:49:17.000000 libgzipf-20240422/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-04-22 04:49:17.000000 libgzipf-20240422/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-04-22 04:49:17.000000 libgzipf-20240422/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29824 2024-04-22 04:49:39.000000 libgzipf-20240422/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-22 04:49:17.000000 libgzipf-20240422/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-04-22 04:49:17.000000 libgzipf-20240422/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-04-22 04:49:17.000000 libgzipf-20240422/libclocale/libclocale_codepage.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:08:59.000000 libgzipf-20240422/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-04-22 04:49:24.000000 libgzipf-20240422/libfcache/libfcache_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-04-22 04:49:24.000000 libgzipf-20240422/libfcache/libfcache_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-04-22 04:49:24.000000 libgzipf-20240422/libfcache/libfcache_cache_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-22 04:49:24.000000 libgzipf-20240422/libfcache/libfcache_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      876 2024-04-22 04:49:24.000000 libgzipf-20240422/libfcache/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-22 04:49:24.000000 libgzipf-20240422/libfcache/libfcache_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-22 04:49:24.000000 libgzipf-20240422/libfcache/libfcache_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-04-22 04:49:24.000000 libgzipf-20240422/libfcache/libfcache_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-04-22 04:49:24.000000 libgzipf-20240422/libfcache/libfcache_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-22 04:49:24.000000 libgzipf-20240422/libfcache/libfcache_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-22 04:49:24.000000 libgzipf-20240422/libfcache/libfcache_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-04-22 04:49:24.000000 libgzipf-20240422/libfcache/libfcache_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-22 04:49:24.000000 libgzipf-20240422/libfcache/libfcache_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-04-22 04:49:24.000000 libgzipf-20240422/libfcache/libfcache_cache_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30333 2024-04-22 04:49:40.000000 libgzipf-20240422/libfcache/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-22 04:49:24.000000 libgzipf-20240422/libfcache/libfcache_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-04-22 04:49:24.000000 libgzipf-20240422/libfcache/libfcache_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-04-22 04:49:24.000000 libgzipf-20240422/libfcache/libfcache_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2036 2024-04-22 04:28:00.000000 libgzipf-20240422/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:08:59.000000 libgzipf-20240422/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33676 2024-04-22 04:49:39.000000 libgzipf-20240422/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-04-22 04:49:12.000000 libgzipf-20240422/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:09:53.000000 libgzipf-20240422/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-04-22 04:49:39.000000 libgzipf-20240422/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:08:57.000000 libgzipf-20240422/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1026 2024-04-22 04:19:39.000000 libgzipf-20240422/dpkg/copyright
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:08:57.000000 libgzipf-20240422/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-04-22 04:19:33.000000 libgzipf-20240422/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-04-22 04:19:33.000000 libgzipf-20240422/dpkg/libgzipf-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-04-22 04:19:33.000000 libgzipf-20240422/dpkg/libgzipf-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2063 2024-04-22 04:19:33.000000 libgzipf-20240422/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-04-22 04:19:33.000000 libgzipf-20240422/dpkg/libgzipf.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      769 2024-04-22 04:19:33.000000 libgzipf-20240422/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      121 2024-04-22 04:19:33.000000 libgzipf-20240422/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2024-04-22 04:49:58.000000 libgzipf-20240422/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-04-22 04:19:33.000000 libgzipf-20240422/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-04-22 04:19:33.000000 libgzipf-20240422/dpkg/libgzipf-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      486 2024-04-22 04:49:58.000000 libgzipf-20240422/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2342 2024-04-22 04:49:58.000000 libgzipf-20240422/libgzipf.spec
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-04-22 04:19:33.000000 libgzipf-20240422/COPYING.LESSER
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      690 2024-04-22 04:19:33.000000 libgzipf-20240422/libgzipf.pc.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1833084 2024-04-22 04:49:38.000000 libgzipf-20240422/configure
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:00.000000 libgzipf-20240422/libgzipf/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12520 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_huffman_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1071 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2280 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_bit_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8516 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2094 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_huffman_tree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14909 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_member_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2722 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2655 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3703 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1587 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3728 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_member.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1726 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2048 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_segment_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2439 2024-04-22 04:26:24.000000 libgzipf-20240422/libgzipf/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1069 2024-04-22 04:49:58.000000 libgzipf-20240422/libgzipf/libgzipf.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1316 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/gzipf_member_footer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    89920 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23484 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_member.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9597 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4109 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_member_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19792 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_compressed_segment.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_member_footer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1587 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1670 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_checksum.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2063 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2028 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7930 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_bit_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2863 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_compressed_segment.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19704 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_member_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1814 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9337 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7048 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_member_footer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48890 2024-04-22 04:21:15.000000 libgzipf-20240422/libgzipf/libgzipf_deflate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3488 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_deflate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36772 2024-04-22 04:49:40.000000 libgzipf-20240422/libgzipf/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2720 2024-04-22 04:49:58.000000 libgzipf-20240422/libgzipf/libgzipf_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/gzipf_member_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4882 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_checksum.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2484 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_member_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3570 2024-04-22 04:19:37.000000 libgzipf-20240422/libgzipf/libgzipf_segment_descriptor.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-04-22 04:49:39.000000 libgzipf-20240422/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-04-22 04:49:39.000000 libgzipf-20240422/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-04-22 04:19:59.000000 libgzipf-20240422/msvscpp/libfdata/libfdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/gzipf_test_tools_output/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5703 2024-04-22 04:20:28.000000 libgzipf-20240422/msvscpp/gzipf_test_tools_output/gzipf_test_tools_output.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/gzipf_test_checksum/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5683 2024-04-22 04:20:28.000000 libgzipf-20240422/msvscpp/gzipf_test_checksum/gzipf_test_checksum.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/gzipf_test_tools_signal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5703 2024-04-22 04:20:28.000000 libgzipf-20240422/msvscpp/gzipf_test_tools_signal/gzipf_test_tools_signal.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/gzipf_test_deflate/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5684 2024-04-22 04:20:28.000000 libgzipf-20240422/msvscpp/gzipf_test_deflate/gzipf_test_deflate.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/zlib/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6068 2024-04-22 04:19:59.000000 libgzipf-20240422/msvscpp/zlib/zlib.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/gzipf_test_tools_info_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5868 2024-04-22 04:20:28.000000 libgzipf-20240422/msvscpp/gzipf_test_tools_info_handle/gzipf_test_tools_info_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/gzipf_test_huffman_tree/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5776 2024-04-22 04:20:28.000000 libgzipf-20240422/msvscpp/gzipf_test_huffman_tree/gzipf_test_huffman_tree.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-04-22 04:19:59.000000 libgzipf-20240422/msvscpp/libclocale/libclocale.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-04-22 04:19:59.000000 libgzipf-20240422/msvscpp/libfcache/libfcache.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1564 2024-04-22 04:27:11.000000 libgzipf-20240422/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/gzipf_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6424 2024-04-22 04:20:28.000000 libgzipf-20240422/msvscpp/gzipf_test_support/gzipf_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-04-22 04:19:59.000000 libgzipf-20240422/msvscpp/libbfio/libbfio.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/gzipf_test_compressed_segment/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5794 2024-04-22 04:20:28.000000 libgzipf-20240422/msvscpp/gzipf_test_compressed_segment/gzipf_test_compressed_segment.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/libgzipf/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9444 2024-04-22 04:19:59.000000 libgzipf-20240422/msvscpp/libgzipf/libgzipf.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/gzipf_test_bit_stream/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5770 2024-04-22 04:20:28.000000 libgzipf-20240422/msvscpp/gzipf_test_bit_stream/gzipf_test_bit_stream.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-04-22 04:19:59.000000 libgzipf-20240422/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/gzipf_test_member_footer/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6029 2024-04-22 04:20:28.000000 libgzipf-20240422/msvscpp/gzipf_test_member_footer/gzipf_test_member_footer.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/gzipf_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5767 2024-04-22 04:20:28.000000 libgzipf-20240422/msvscpp/gzipf_test_io_handle/gzipf_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-04-22 04:19:59.000000 libgzipf-20240422/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/gzipf_test_member/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5758 2024-04-22 04:20:28.000000 libgzipf-20240422/msvscpp/gzipf_test_member/gzipf_test_member.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-04-22 04:19:59.000000 libgzipf-20240422/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/gzipf_test_file/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6415 2024-04-22 04:20:28.000000 libgzipf-20240422/msvscpp/gzipf_test_file/gzipf_test_file.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/gzipf_test_member_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6029 2024-04-22 04:20:28.000000 libgzipf-20240422/msvscpp/gzipf_test_member_header/gzipf_test_member_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-04-22 04:19:59.000000 libgzipf-20240422/msvscpp/libcpath/libcpath.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/gzipfinfo/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6490 2024-04-22 04:19:59.000000 libgzipf-20240422/msvscpp/gzipfinfo/gzipfinfo.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/gzipf_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5596 2024-04-22 04:20:28.000000 libgzipf-20240422/msvscpp/gzipf_test_notify/gzipf_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-04-22 04:19:59.000000 libgzipf-20240422/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/pygzipf/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6695 2024-04-22 04:20:28.000000 libgzipf-20240422/msvscpp/pygzipf/pygzipf.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/gzipf_test_member_descriptor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5791 2024-04-22 04:20:28.000000 libgzipf-20240422/msvscpp/gzipf_test_member_descriptor/gzipf_test_member_descriptor.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-04-22 04:19:59.000000 libgzipf-20240422/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23180 2024-04-22 04:49:40.000000 libgzipf-20240422/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-04-22 04:19:59.000000 libgzipf-20240422/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-04-22 04:19:59.000000 libgzipf-20240422/msvscpp/libcerror/libcerror.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31425 2024-04-22 04:20:28.000000 libgzipf-20240422/msvscpp/libgzipf.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/gzipfmount/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7477 2024-04-22 04:19:59.000000 libgzipf-20240422/msvscpp/gzipfmount/gzipfmount.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-04-22 04:19:59.000000 libgzipf-20240422/msvscpp/libfdatetime/libfdatetime.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/msvscpp/gzipf_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5509 2024-04-22 04:20:28.000000 libgzipf-20240422/msvscpp/gzipf_test_error/gzipf_test_error.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       92 2024-04-22 04:19:35.000000 libgzipf-20240422/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:08:59.000000 libgzipf-20240422/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-22 04:49:16.000000 libgzipf-20240422/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-04-22 04:49:16.000000 libgzipf-20240422/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-22 04:49:16.000000 libgzipf-20240422/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-04-22 04:49:16.000000 libgzipf-20240422/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-04-22 04:49:16.000000 libgzipf-20240422/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-04-22 04:49:16.000000 libgzipf-20240422/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      938 2024-04-22 04:49:16.000000 libgzipf-20240422/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-04-22 04:49:16.000000 libgzipf-20240422/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-04-22 04:49:16.000000 libgzipf-20240422/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-04-22 04:49:16.000000 libgzipf-20240422/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-22 04:49:16.000000 libgzipf-20240422/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-04-22 04:49:16.000000 libgzipf-20240422/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-22 04:49:16.000000 libgzipf-20240422/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-22 04:49:16.000000 libgzipf-20240422/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-04-22 04:49:16.000000 libgzipf-20240422/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-22 04:49:16.000000 libgzipf-20240422/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-04-22 04:49:16.000000 libgzipf-20240422/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30657 2024-04-22 04:49:39.000000 libgzipf-20240422/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-22 04:49:16.000000 libgzipf-20240422/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-22 04:49:16.000000 libgzipf-20240422/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-04-22 04:49:16.000000 libgzipf-20240422/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-04-22 04:49:16.000000 libgzipf-20240422/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      295 2024-04-22 04:19:33.000000 libgzipf-20240422/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-04-22 04:49:39.000000 libgzipf-20240422/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:08:58.000000 libgzipf-20240422/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32570 2024-04-22 04:49:39.000000 libgzipf-20240422/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-22 04:49:13.000000 libgzipf-20240422/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-22 04:19:33.000000 libgzipf-20240422/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      487 2024-04-22 04:19:33.000000 libgzipf-20240422/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-04-22 04:49:39.000000 libgzipf-20240422/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-04-22 04:19:33.000000 libgzipf-20240422/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1508 2024-04-22 04:19:33.000000 libgzipf-20240422/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:09:53.000000 libgzipf-20240422/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:08:58.000000 libgzipf-20240422/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33009 2024-04-22 04:49:40.000000 libgzipf-20240422/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-04-22 04:49:22.000000 libgzipf-20240422/libcthreads/libcthreads_queue.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-04-22 04:49:40.000000 libgzipf-20240422/test-driver
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:08:59.000000 libgzipf-20240422/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-04-22 04:49:20.000000 libgzipf-20240422/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-22 04:49:20.000000 libgzipf-20240422/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-04-22 04:49:20.000000 libgzipf-20240422/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2024-04-22 04:49:20.000000 libgzipf-20240422/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-22 04:49:20.000000 libgzipf-20240422/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-22 04:49:20.000000 libgzipf-20240422/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-04-22 04:49:20.000000 libgzipf-20240422/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-04-22 04:49:20.000000 libgzipf-20240422/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-04-22 04:49:20.000000 libgzipf-20240422/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-04-22 04:49:20.000000 libgzipf-20240422/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-04-22 04:49:20.000000 libgzipf-20240422/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-22 04:49:20.000000 libgzipf-20240422/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29855 2024-04-22 04:49:40.000000 libgzipf-20240422/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-04-22 04:49:20.000000 libgzipf-20240422/libcpath/libcpath_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-22 04:49:20.000000 libgzipf-20240422/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-04-22 04:49:20.000000 libgzipf-20240422/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-04-22 04:49:20.000000 libgzipf-20240422/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      206 2023-12-03 09:09:54.000000 libgzipf-20240422/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:01.000000 libgzipf-20240422/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1255 2024-04-22 04:19:39.000000 libgzipf-20240422/manuals/gzipfinfo.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      129 2024-04-22 04:27:01.000000 libgzipf-20240422/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26589 2024-04-22 04:49:40.000000 libgzipf-20240422/manuals/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6086 2024-04-22 04:19:39.000000 libgzipf-20240422/manuals/libgzipf.3
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:01.000000 libgzipf-20240422/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28883 2024-04-22 04:20:28.000000 libgzipf-20240422/tests/gzipf_test_member_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4146 2024-04-22 04:19:38.000000 libgzipf-20240422/tests/gzipf_test_checksum.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57012 2024-04-22 04:20:28.000000 libgzipf-20240422/tests/gzipf_test_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-04-22 04:19:39.000000 libgzipf-20240422/tests/gzipf_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100638 2024-04-22 04:19:38.000000 libgzipf-20240422/tests/gzipf_test_deflate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12829 2024-04-22 04:20:28.000000 libgzipf-20240422/tests/gzipf_test_member_footer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1812 2024-04-22 04:19:38.000000 libgzipf-20240422/tests/gzipf_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8056 2024-04-22 04:19:39.000000 libgzipf-20240422/tests/gzipf_test_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      981 2024-04-22 04:19:39.000000 libgzipf-20240422/tests/gzipf_test_libgzipf.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4037 2024-04-22 04:25:49.000000 libgzipf-20240422/tests/test_tools.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3139 2024-04-22 04:19:38.000000 libgzipf-20240422/tests/gzipf_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-22 04:19:39.000000 libgzipf-20240422/tests/gzipf_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13779 2024-04-22 04:20:28.000000 libgzipf-20240422/tests/gzipf_test_bit_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4169 2024-04-22 04:19:39.000000 libgzipf-20240422/tests/gzipf_test_tools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15093 2024-04-22 04:20:28.000000 libgzipf-20240422/tests/gzipf_test_member_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2024-04-22 04:19:39.000000 libgzipf-20240422/tests/gzipf_test_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2447 2024-04-22 04:19:39.000000 libgzipf-20240422/tests/gzipf_test_tools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2024-04-22 04:19:39.000000 libgzipf-20240422/tests/gzipf_test_memory.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3289 2024-04-22 04:19:38.000000 libgzipf-20240422/tests/test_gzipfinfo.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7348 2024-04-22 04:38:36.000000 libgzipf-20240422/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4323 2024-04-22 04:19:39.000000 libgzipf-20240422/tests/gzipf_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11372 2024-04-22 04:21:03.000000 libgzipf-20240422/tests/pygzipf_test_file.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2345 2024-04-22 04:19:38.000000 libgzipf-20240422/tests/pygzipf_test_support.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-22 04:19:38.000000 libgzipf-20240422/tests/test_manpage.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4412 2024-04-22 04:25:39.000000 libgzipf-20240422/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8574 2024-04-22 04:19:39.000000 libgzipf-20240422/tests/gzipf_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3124 2024-04-22 04:20:28.000000 libgzipf-20240422/tests/gzipf_test_member.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14367 2024-04-22 04:19:39.000000 libgzipf-20240422/tests/gzipf_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-04-22 04:19:39.000000 libgzipf-20240422/tests/gzipf_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-04-22 04:19:38.000000 libgzipf-20240422/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2024-04-22 04:19:39.000000 libgzipf-20240422/tests/gzipf_test_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2024-04-22 04:19:39.000000 libgzipf-20240422/tests/gzipf_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5634 2024-04-22 04:19:39.000000 libgzipf-20240422/tests/gzipf_test_tools_info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1709 2024-04-22 04:19:39.000000 libgzipf-20240422/tests/gzipf_test_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2866 2024-04-22 04:20:28.000000 libgzipf-20240422/tests/gzipf_test_compressed_segment.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    65574 2024-04-22 04:49:40.000000 libgzipf-20240422/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2024-04-22 04:19:39.000000 libgzipf-20240422/tests/gzipf_test_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13259 2024-04-22 04:19:38.000000 libgzipf-20240422/tests/gzipf_test_functions.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30822 2024-04-22 04:20:28.000000 libgzipf-20240422/tests/gzipf_test_huffman_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-04-22 04:19:39.000000 libgzipf-20240422/tests/gzipf_test_memory.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4157 2024-04-22 04:25:17.000000 libgzipf-20240422/tests/test_library.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:02.000000 libgzipf-20240422/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      888 2024-04-22 04:26:41.000000 libgzipf-20240422/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      972 2024-04-22 04:19:37.000000 libgzipf-20240422/ossfuzz/ossfuzz_libgzipf.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-04-22 04:19:37.000000 libgzipf-20240422/ossfuzz/ossfuzz_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2214 2024-04-22 04:19:37.000000 libgzipf-20240422/ossfuzz/file_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31885 2024-04-22 04:49:40.000000 libgzipf-20240422/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3254 2024-04-22 04:19:33.000000 libgzipf-20240422/libgzipf.spec.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-04-22 04:49:34.000000 libgzipf-20240422/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:08:58.000000 libgzipf-20240422/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-04-22 04:49:21.000000 libgzipf-20240422/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-04-22 04:49:21.000000 libgzipf-20240422/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-04-22 04:49:21.000000 libgzipf-20240422/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-04-22 04:49:21.000000 libgzipf-20240422/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-22 04:49:21.000000 libgzipf-20240422/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-04-22 04:49:21.000000 libgzipf-20240422/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-22 04:49:21.000000 libgzipf-20240422/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-04-22 04:49:21.000000 libgzipf-20240422/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-22 04:49:21.000000 libgzipf-20240422/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-04-22 04:49:21.000000 libgzipf-20240422/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-04-22 04:49:21.000000 libgzipf-20240422/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-04-22 04:49:21.000000 libgzipf-20240422/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-22 04:49:21.000000 libgzipf-20240422/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-22 04:49:21.000000 libgzipf-20240422/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-22 04:49:21.000000 libgzipf-20240422/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-04-22 04:49:21.000000 libgzipf-20240422/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30752 2024-04-22 04:49:40.000000 libgzipf-20240422/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-04-22 04:49:21.000000 libgzipf-20240422/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-04-22 04:49:21.000000 libgzipf-20240422/libcsplit/libcsplit_narrow_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:01.000000 libgzipf-20240422/pygzipf/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2335 2024-04-22 04:19:37.000000 libgzipf-20240422/pygzipf/pygzipf_member.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14794 2024-04-22 04:19:37.000000 libgzipf-20240422/pygzipf/pygzipf.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-04-22 04:19:37.000000 libgzipf-20240422/pygzipf/pygzipf_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2024-04-22 04:19:37.000000 libgzipf-20240422/pygzipf/pygzipf_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2033 2024-04-22 04:19:37.000000 libgzipf-20240422/pygzipf/pygzipf_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8876 2024-04-22 04:19:37.000000 libgzipf-20240422/pygzipf/pygzipf_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1860 2024-04-22 04:19:37.000000 libgzipf-20240422/pygzipf/pygzipf.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3278 2024-04-22 04:21:03.000000 libgzipf-20240422/pygzipf/pygzipf_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-22 04:26:33.000000 libgzipf-20240422/pygzipf/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-22 04:19:37.000000 libgzipf-20240422/pygzipf/pygzipf_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-22 04:19:37.000000 libgzipf-20240422/pygzipf/pygzipf_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15417 2024-04-22 04:21:03.000000 libgzipf-20240422/pygzipf/pygzipf_member.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33880 2024-04-22 04:19:37.000000 libgzipf-20240422/pygzipf/pygzipf_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-04-22 04:19:37.000000 libgzipf-20240422/pygzipf/pygzipf_libgzipf.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1826 2024-04-22 04:19:37.000000 libgzipf-20240422/pygzipf/pygzipf_datetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9143 2024-04-22 04:19:37.000000 libgzipf-20240422/pygzipf/pygzipf_members.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3290 2024-04-22 04:19:37.000000 libgzipf-20240422/pygzipf/pygzipf_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9546 2024-04-22 04:19:37.000000 libgzipf-20240422/pygzipf/pygzipf_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-22 04:19:37.000000 libgzipf-20240422/pygzipf/pygzipf_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4118 2024-04-22 04:19:37.000000 libgzipf-20240422/pygzipf/pygzipf_file_object_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2024-04-22 04:19:37.000000 libgzipf-20240422/pygzipf/pygzipf_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45406 2024-04-22 04:49:40.000000 libgzipf-20240422/pygzipf/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-04-22 04:19:37.000000 libgzipf-20240422/pygzipf/pygzipf_members.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34403 2024-04-22 04:21:03.000000 libgzipf-20240422/pygzipf/pygzipf_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16609 2024-04-22 04:19:37.000000 libgzipf-20240422/pygzipf/pygzipf_datetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1525 2024-04-22 04:19:37.000000 libgzipf-20240422/pygzipf/pygzipf_libbfio.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:01.000000 libgzipf-20240422/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:10:06.000000 libgzipf-20240422/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:10:06.000000 libgzipf-20240422/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:10:06.000000 libgzipf-20240422/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:10:06.000000 libgzipf-20240422/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:10:06.000000 libgzipf-20240422/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:10:06.000000 libgzipf-20240422/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:10:06.000000 libgzipf-20240422/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:10:06.000000 libgzipf-20240422/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:10:06.000000 libgzipf-20240422/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1854 2024-04-22 04:49:58.000000 libgzipf-20240422/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:10:06.000000 libgzipf-20240422/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:10:06.000000 libgzipf-20240422/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:08:59.000000 libgzipf-20240422/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56336 2024-04-22 04:49:40.000000 libgzipf-20240422/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-04-22 04:49:29.000000 libgzipf-20240422/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40501 2024-04-22 04:49:39.000000 libgzipf-20240422/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:08:58.000000 libgzipf-20240422/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-22 04:49:19.000000 libgzipf-20240422/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-22 04:49:18.000000 libgzipf-20240422/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-04-22 04:49:18.000000 libgzipf-20240422/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-04-22 04:49:18.000000 libgzipf-20240422/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-04-22 04:49:19.000000 libgzipf-20240422/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-22 04:49:18.000000 libgzipf-20240422/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-04-22 04:49:18.000000 libgzipf-20240422/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-04-22 04:49:18.000000 libgzipf-20240422/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-04-22 04:49:18.000000 libgzipf-20240422/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-04-22 04:49:18.000000 libgzipf-20240422/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-04-22 04:49:18.000000 libgzipf-20240422/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29693 2024-04-22 04:49:40.000000 libgzipf-20240422/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-22 04:49:18.000000 libgzipf-20240422/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-04-22 04:49:18.000000 libgzipf-20240422/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:08:57.000000 libgzipf-20240422/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-04-22 04:49:14.000000 libgzipf-20240422/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-04-22 04:49:14.000000 libgzipf-20240422/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-22 04:49:14.000000 libgzipf-20240422/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-04-22 04:49:14.000000 libgzipf-20240422/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-22 04:49:14.000000 libgzipf-20240422/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-22 04:49:14.000000 libgzipf-20240422/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-04-22 04:49:14.000000 libgzipf-20240422/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-04-22 04:49:14.000000 libgzipf-20240422/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-04-22 04:49:14.000000 libgzipf-20240422/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-22 04:49:14.000000 libgzipf-20240422/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-22 04:49:14.000000 libgzipf-20240422/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29160 2024-04-22 04:49:39.000000 libgzipf-20240422/libcerror/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-22 05:09:00.000000 libgzipf-20240422/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-22 04:49:26.000000 libgzipf-20240422/libfdatetime/libfdatetime_floatingtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-04-22 04:49:26.000000 libgzipf-20240422/libfdatetime/libfdatetime_nsf_timedate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-04-22 04:49:26.000000 libgzipf-20240422/libfdatetime/libfdatetime_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-04-22 04:49:26.000000 libgzipf-20240422/libfdatetime/libfdatetime_floatingtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-04-22 04:49:26.000000 libgzipf-20240422/libfdatetime/libfdatetime_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-04-22 04:49:26.000000 libgzipf-20240422/libfdatetime/libfdatetime_hfs_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-04-22 04:49:26.000000 libgzipf-20240422/libfdatetime/libfdatetime_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-04-22 04:49:26.000000 libgzipf-20240422/libfdatetime/libfdatetime_hfs_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-04-22 04:49:26.000000 libgzipf-20240422/libfdatetime/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-04-22 04:49:26.000000 libgzipf-20240422/libfdatetime/libfdatetime_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-04-22 04:49:26.000000 libgzipf-20240422/libfdatetime/libfdatetime_systemtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-22 04:49:26.000000 libgzipf-20240422/libfdatetime/libfdatetime_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-04-22 04:49:26.000000 libgzipf-20240422/libfdatetime/libfdatetime_posix_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-04-22 04:49:26.000000 libgzipf-20240422/libfdatetime/libfdatetime_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-04-22 04:49:26.000000 libgzipf-20240422/libfdatetime/libfdatetime_fat_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-04-22 04:49:26.000000 libgzipf-20240422/libfdatetime/libfdatetime_systemtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-04-22 04:49:26.000000 libgzipf-20240422/libfdatetime/libfdatetime_nsf_timedate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-22 04:49:26.000000 libgzipf-20240422/libfdatetime/libfdatetime_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-04-22 04:49:26.000000 libgzipf-20240422/libfdatetime/libfdatetime_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-04-22 04:49:26.000000 libgzipf-20240422/libfdatetime/libfdatetime_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-04-22 04:49:26.000000 libgzipf-20240422/libfdatetime/libfdatetime_posix_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-04-22 04:49:26.000000 libgzipf-20240422/libfdatetime/libfdatetime_date_time_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-04-22 04:49:26.000000 libgzipf-20240422/libfdatetime/libfdatetime_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-04-22 04:49:26.000000 libgzipf-20240422/libfdatetime/libfdatetime_date_time_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-04-22 04:49:26.000000 libgzipf-20240422/libfdatetime/libfdatetime_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32744 2024-04-22 04:49:40.000000 libgzipf-20240422/libfdatetime/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-04-22 04:49:26.000000 libgzipf-20240422/libfdatetime/libfdatetime_fat_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56822 2024-04-22 04:49:36.000000 libgzipf-20240422/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7711 2024-04-22 04:19:33.000000 libgzipf-20240422/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      418 2024-04-22 05:09:02.913293 libgzipf-20240422/PKG-INFO
```

### Comparing `libgzipf-20240103/libfdata/libfdata_error.h` & `libgzipf-20240422/libfdata/libfdata_error.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_area.c` & `libgzipf-20240422/libfdata/libfdata_area.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The area functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_stream.h` & `libgzipf-20240422/libfdata/libfdata_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The stream functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_cache.h` & `libgzipf-20240422/libfdata/libfdata_cache.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Cache functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_range_list.c` & `libgzipf-20240422/libfdata/libfdata_range_list.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The range list functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_mapped_range.c` & `libgzipf-20240422/libfdata/libfdata_mapped_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The (data) mapped range functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_libcerror.h` & `libgzipf-20240422/libfdata/libfdata_libcerror.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_definitions.h` & `libgzipf-20240422/libfdata/libfdata_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBFDATA )
 #include <libfdata/definitions.h>
 
 /* The definitions in <libfdata/definitions.h> are copied here
  * for local use of libfdata
  */
 #else
-#define LIBFDATA_VERSION						20230319
+#define LIBFDATA_VERSION						20240415
 
 /* The libfdata version string
  */
-#define LIBFDATA_VERSION_STRING						"20230319"
+#define LIBFDATA_VERSION_STRING						"20240415"
 
 /* The library flag definitions
  */
 enum LIBFDATA_FLAGS
 {
 	/* The data is not managed by the library
 	 */
```

### Comparing `libgzipf-20240103/libfdata/libfdata_list.c` & `libgzipf-20240422/libfdata/libfdata_list.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The list functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_libcdata.h` & `libgzipf-20240422/libfdata/libfdata_libcdata.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_list.h` & `libgzipf-20240422/libfdata/libfdata_list.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The list functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_list_element.h` & `libgzipf-20240422/libfdata/libfdata_list_element.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The list element functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -93,14 +93,15 @@
 int libfdata_list_element_get_timestamp(
      libfdata_list_element_t *element,
      int64_t *timestamp,
      libcerror_error_t **error );
 
 /* Data range functions
  */
+LIBFDATA_EXTERN \
 int libfdata_list_element_get_data_range(
      libfdata_list_element_t *element,
      int *file_index,
      off64_t *offset,
      size64_t *size,
      uint32_t *flags,
      libcerror_error_t **error );
```

### Comparing `libgzipf-20240103/libfdata/Makefile.am` & `libgzipf-20240422/libfdata/Makefile.am`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBFCACHE_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
@@ -31,17 +31,17 @@
 	libfdata_stream.c libfdata_stream.h \
 	libfdata_support.c libfdata_support.h \
 	libfdata_types.h \
 	libfdata_unused.h \
 	libfdata_vector.c libfdata_vector.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libfdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdata_la_SOURCES)
```

### Comparing `libgzipf-20240103/libfdata/libfdata_libcnotify.h` & `libgzipf-20240422/libfdata/libfdata_libcnotify.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcnotify header wrapper
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_extern.h` & `libgzipf-20240422/libfdata/libfdata_extern.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_notify.c` & `libgzipf-20240422/libfdata/libfdata_notify.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Notification functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_cache.c` & `libgzipf-20240422/libfdata/libfdata_cache.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Cache functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_stream.c` & `libgzipf-20240422/libfdata/libfdata_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The stream functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_unused.h` & `libgzipf-20240422/libfdata/libfdata_unused.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_range.h` & `libgzipf-20240422/libfdata/libfdata_range.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The range functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_area.h` & `libgzipf-20240422/libfdata/libfdata_area.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The area functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_error.c` & `libgzipf-20240422/libfdata/libfdata_error.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_support.h` & `libgzipf-20240422/libfdata/libfdata_support.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_range.c` & `libgzipf-20240422/libfdata/libfdata_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The range functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_mapped_range.h` & `libgzipf-20240422/libfdata/libfdata_mapped_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The (data) mapped range functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_support.c` & `libgzipf-20240422/libfcache/libfcache_support.c`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -20,22 +20,22 @@
  */
 
 #include <common.h>
 #include <types.h>
 
 #include <stdio.h>
 
-#include "libfdata_definitions.h"
-#include "libfdata_support.h"
+#include "libfcache_definitions.h"
+#include "libfcache_support.h"
 
-#if !defined( HAVE_LOCAL_LIBFDATA )
+#if !defined( HAVE_LOCAL_LIBFCACHE )
 
 /* Returns the library version as a string
  */
-const char *libfdata_get_version(
+const char *libfcache_get_version(
              void )
 {
-	return( (const char *) LIBFDATA_VERSION_STRING );
+	return( (const char *) LIBFCACHE_VERSION_STRING );
 }
 
-#endif /* !defined( HAVE_LOCAL_LIBFDATA ) */
+#endif /* !defined( HAVE_LOCAL_LIBFCACHE ) */
```

### Comparing `libgzipf-20240103/libfdata/libfdata_list_element.c` & `libgzipf-20240422/libfdata/libfdata_list_element.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The list element functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_segments_array.c` & `libgzipf-20240422/libfdata/libfdata_segments_array.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The segments array functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_types.h` & `libgzipf-20240422/libfdata/libfdata_types.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_notify.h` & `libgzipf-20240422/libfdata/libfdata_notify.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Notification functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_range_list.h` & `libgzipf-20240422/libfdata/libfdata_range_list.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The range list functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_segments_array.h` & `libgzipf-20240422/libfdata/libfdata_segments_array.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The segments array functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/Makefile.in` & `libgzipf-20240422/libfdata/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -471,14 +471,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -535,16 +537,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBFDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBFCACHE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
@@ -568,15 +570,16 @@
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_segments_array.c libfdata_segments_array.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_stream.c libfdata_stream.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_support.c libfdata_support.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_types.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_unused.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_vector.c libfdata_vector.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -788,24 +791,39 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfdata_area.Plo
+	-rm -f ./$(DEPDIR)/libfdata_cache.Plo
+	-rm -f ./$(DEPDIR)/libfdata_error.Plo
+	-rm -f ./$(DEPDIR)/libfdata_list.Plo
+	-rm -f ./$(DEPDIR)/libfdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libfdata_mapped_range.Plo
+	-rm -f ./$(DEPDIR)/libfdata_notify.Plo
+	-rm -f ./$(DEPDIR)/libfdata_range.Plo
+	-rm -f ./$(DEPDIR)/libfdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libfdata_segments_array.Plo
+	-rm -f ./$(DEPDIR)/libfdata_stream.Plo
+	-rm -f ./$(DEPDIR)/libfdata_support.Plo
+	-rm -f ./$(DEPDIR)/libfdata_vector.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -875,14 +893,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -893,23 +913,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libfdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libgzipf-20240103/libfdata/libfdata_vector.c` & `libgzipf-20240422/libfdata/libfdata_vector.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The vector functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_libfcache.h` & `libgzipf-20240422/libfdata/libfdata_libfcache.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libfcache header wrapper
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdata/libfdata_vector.h` & `libgzipf-20240422/libfdata/libfdata_vector.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The vector functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/COPYING` & `libgzipf-20240422/COPYING`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/install-sh` & `libgzipf-20240422/install-sh`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/depcomp` & `libgzipf-20240422/depcomp`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/gzipfmount.c` & `libgzipf-20240422/gzipftools/gzipfmount.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/gzipftools_output.h` & `libgzipf-20240422/gzipftools/gzipftools_output.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/mount_dokan.c` & `libgzipf-20240422/gzipftools/mount_dokan.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/mount_file_system.h` & `libgzipf-20240422/gzipftools/mount_file_system.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/mount_fuse.c` & `libgzipf-20240422/gzipftools/mount_fuse.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/info_handle.h` & `libgzipf-20240422/gzipftools/info_handle.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/mount_dokan.h` & `libgzipf-20240422/gzipftools/mount_dokan.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/mount_file_system.c` & `libgzipf-20240422/gzipftools/mount_file_system.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/gzipftools_libgzipf.h` & `libgzipf-20240422/gzipftools/gzipftools_libgzipf.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/gzipftools_getopt.h` & `libgzipf-20240422/gzipftools/gzipftools_getopt.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/Makefile.am` & `libgzipf-20240422/gzipftools/Makefile.am`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -73,19 +73,17 @@
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libgzipf/libgzipf.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on gzipfinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(gzipfinfo_SOURCES)
 	@echo "Running splint on gzipfmount ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(gzipfmount_SOURCES)
```

### Comparing `libgzipf-20240103/gzipftools/gzipftools_getopt.c` & `libgzipf-20240422/gzipftools/gzipftools_getopt.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/gzipftools_libfdatetime.h` & `libgzipf-20240422/gzipftools/gzipftools_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/gzipftools_i18n.h` & `libgzipf-20240422/gzipftools/gzipftools_i18n.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/gzipftools_libcpath.h` & `libgzipf-20240422/gzipftools/gzipftools_libcpath.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/mount_file_entry.c` & `libgzipf-20240422/gzipftools/mount_file_entry.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/info_handle.c` & `libgzipf-20240422/gzipftools/info_handle.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/gzipfinfo.c` & `libgzipf-20240422/gzipftools/gzipfinfo.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/mount_file_entry.h` & `libgzipf-20240422/gzipftools/mount_file_entry.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/gzipftools_signal.c` & `libgzipf-20240422/gzipftools/gzipftools_signal.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/mount_handle.h` & `libgzipf-20240422/gzipftools/mount_handle.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/gzipftools_signal.h` & `libgzipf-20240422/gzipftools/gzipftools_signal.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/gzipftools_unused.h` & `libgzipf-20240422/gzipftools/gzipftools_unused.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/gzipftools_libbfio.h` & `libgzipf-20240422/gzipftools/gzipftools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/mount_handle.c` & `libgzipf-20240422/gzipftools/mount_handle.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/gzipftools_libuna.h` & `libgzipf-20240422/gzipftools/gzipftools_libuna.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/gzipftools_libcdata.h` & `libgzipf-20240422/gzipftools/gzipftools_libcdata.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/gzipftools_libcnotify.h` & `libgzipf-20240422/gzipftools/gzipftools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/gzipftools_libclocale.h` & `libgzipf-20240422/gzipftools/gzipftools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/Makefile.in` & `libgzipf-20240422/gzipftools/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -454,14 +454,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -518,16 +520,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -591,15 +593,16 @@
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libgzipf/libgzipf.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -855,23 +858,36 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/gzipfinfo.Po
+	-rm -f ./$(DEPDIR)/gzipfmount.Po
+	-rm -f ./$(DEPDIR)/gzipftools_getopt.Po
+	-rm -f ./$(DEPDIR)/gzipftools_output.Po
+	-rm -f ./$(DEPDIR)/gzipftools_signal.Po
+	-rm -f ./$(DEPDIR)/info_handle.Po
+	-rm -f ./$(DEPDIR)/mount_dokan.Po
+	-rm -f ./$(DEPDIR)/mount_file_entry.Po
+	-rm -f ./$(DEPDIR)/mount_file_system.Po
+	-rm -f ./$(DEPDIR)/mount_fuse.Po
+	-rm -f ./$(DEPDIR)/mount_handle.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -965,17 +981,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on gzipfinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(gzipfinfo_SOURCES)
 	@echo "Running splint on gzipfmount ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(gzipfmount_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libgzipf-20240103/gzipftools/gzipftools_output.c` & `libgzipf-20240422/gzipftools/gzipftools_output.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/gzipftools_libcerror.h` & `libgzipf-20240422/gzipftools/gzipftools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/gzipftools/mount_fuse.h` & `libgzipf-20240422/gzipftools/mount_fuse.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/m4/libcfile.m4` & `libgzipf-20240422/m4/libcfile.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcfile required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcfile is available
 dnl ac_libcfile_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCFILE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno],
     [ac_cv_libcfile=no],
     [ac_cv_libcfile=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcfile which returns "yes" and --with-libcfile= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect],
+      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcfile"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcfile],
           [1])
@@ -199,16 +201,17 @@
             libcfile_file_remove_wide,
             [ac_cv_libcfile_dummy=yes],
             [ac_cv_libcfile=no])
           ])
 
         ac_cv_libcfile_LIBADD="-lcfile"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes],
+      [test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcfile in directory: $ac_cv_with_libcfile],
         [1])
       ])
     ])
 
   AS_IF(
@@ -354,15 +357,15 @@
   AS_IF(
     [test "x$ac_cv_func_unlink" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: unlink],
       [1])
     ])
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
   ])
 
 dnl Function to detect how to enable libcfile
 AC_DEFUN([AX_LIBCFILE_CHECK_ENABLE],
```

### Comparing `libgzipf-20240103/m4/libfdatetime.m4` & `libgzipf-20240422/m4/libfdatetime.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfdatetime required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfdatetime is available
 dnl ac_libfdatetime_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFDATETIME_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdatetime" = xno],
     [ac_cv_libfdatetime=no],
     [ac_cv_libfdatetime=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfdatetime which returns "yes" and --with-libfdatetime= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect],
+      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfdatetime"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfdatetime}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdatetime}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfdatetime],
           [1])
@@ -455,16 +457,17 @@
           fdatetime,
           libfdatetime_systemetime_copy_to_utf32_string_with_index,
           [ac_cv_libfdatetime_dummy=yes],
           [ac_cv_libfdatetime=no])
 
         ac_cv_libfdatetime_LIBADD="-lfdatetime"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_libfdatetime" != xyes],
+      [test "x$ac_cv_libfdatetime" != xyes && test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfdatetime in directory: $ac_cv_with_libfdatetime],
         [1])
       ])
     ])
 
   AS_IF(
@@ -486,15 +489,15 @@
     ])
   ])
 
 dnl Function to detect if libfdatetime dependencies are available
 AC_DEFUN([AX_LIBFDATETIME_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
   ])
 
 dnl Function to detect how to enable libfdatetime
 AC_DEFUN([AX_LIBFDATETIME_CHECK_ENABLE],
```

### Comparing `libgzipf-20240103/m4/tests.m4` & `libgzipf-20240422/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/m4/libcpath.m4` & `libgzipf-20240422/m4/libcpath.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcpath required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcpath is available
 dnl ac_libcpath_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCPATH_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno],
     [ac_cv_libcpath=no],
     [ac_cv_libcpath=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcpath which returns "yes" and --with-libcpath= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect],
+      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcpath"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcpath],
           [1])
@@ -148,16 +150,17 @@
             libcpath_path_make_directory_wide,
             [ac_cv_libcpath_dummy=yes],
             [ac_cv_libcpath=no])
           ])
 
         ac_cv_libcpath_LIBADD="-lcpath"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes],
+      [test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcpath in directory: $ac_cv_with_libcpath],
         [1])
       ])
     ])
 
   AS_IF(
@@ -269,15 +272,15 @@
     [AC_MSG_FAILURE(
       [Missing functions: getcwd],
       [1])
     ])
 
   AX_LIBCPATH_CHECK_FUNC_MKDIR
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
   ])
 
 dnl Function to detect how to enable libcpath
 AC_DEFUN([AX_LIBCPATH_CHECK_ENABLE],
```

### Comparing `libgzipf-20240103/m4/lib-prefix.m4` & `libgzipf-20240422/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/m4/progtest.m4` & `libgzipf-20240422/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/m4/libuna.m4` & `libgzipf-20240422/m4/libuna.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libuna or required headers and functions
 dnl
-dnl Version: 20230702
+dnl Version: 20240413
 
 dnl Function to detect if a specific libuna definition is available.
 AC_DEFUN([AX_LIBUNA_CHECK_DEFINITION],
   [AC_CACHE_CHECK(
     [if `$1' is defined],
     [$2],
     [AC_LANG_PUSH(C)
@@ -23,16 +23,18 @@
 dnl ac_libuna_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBUNA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno],
     [ac_cv_libuna=no],
     [ac_cv_libuna=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libuna which returns "yes" and --with-libuna= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect],
+      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libuna"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libuna],
           [1])
@@ -938,16 +940,17 @@
           [ac_cv_libuna_defines_compare_greater])
         AS_IF(
           [test "x$ac_cv_libuna_defines_utf16_stream_allow_unpaired_surrogate" != xyes],
           [ac_cv_libuna=no])
 
         ac_cv_libuna_LIBADD="-luna"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes],
+      [test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libuna in directory: $ac_cv_with_libuna],
         [1])
       ])
     ])
 
   AS_IF(
@@ -969,15 +972,15 @@
     ])
   ])
 
 dnl Function to detect if libuna dependencies are available
 AC_DEFUN([AX_LIBUNA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
   ])
 
 dnl Function to detect how to enable libuna
 AC_DEFUN([AX_LIBUNA_CHECK_ENABLE],
```

### Comparing `libgzipf-20240103/m4/gettext.m4` & `libgzipf-20240422/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/m4/lib-ld.m4` & `libgzipf-20240422/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/m4/libclocale.m4` & `libgzipf-20240422/m4/libclocale.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libclocale required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libclocale is available
 dnl ac_libclocale_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCLOCALE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno],
     [ac_cv_libclocale=no],
     [ac_cv_libclocale=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libclocale which returns "yes" and --with-libclocale= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect],
+      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libclocale"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libclocale],
           [1])
@@ -122,16 +124,17 @@
           clocale,
           libclocale_initialize,
           [ac_cv_libclocale_dummy=yes],
           [ac_cv_libclocale=no])
 
         ac_cv_libclocale_LIBADD="-lclocale"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes],
+      [test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libclocale in directory: $ac_cv_with_libclocale],
         [1])
       ])
     ])
 
   AS_IF(
@@ -216,15 +219,15 @@
     [AC_MSG_FAILURE(
       [Missing function: setlocale],
       [1])
     ])
 
   AX_LIBCLOCALE_CHECK_FUNC_LANGINFO_CODESET
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
   ])
 
 dnl Function to detect how to enable libclocale
 AC_DEFUN([AX_LIBCLOCALE_CHECK_ENABLE],
```

### Comparing `libgzipf-20240103/m4/libcdata.m4` & `libgzipf-20240422/m4/libcdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcdata required headers and functions
 dnl
-dnl Version: 20230108
+dnl Version: 20240413
 
 dnl Function to detect if libcdata is available
 dnl ac_libcdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno],
     [ac_cv_libcdata=no],
     [ac_cv_libcdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcdata which returns "yes" and --with-libcdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect],
+      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcdata],
           [1])
@@ -493,16 +495,17 @@
           cdata,
           libcdata_tree_node_get_leaf_node_list,
           [ac_cv_libcdata_dummy=yes],
           [ac_cv_libcdata=no])
 
         ac_cv_libcdata_LIBADD="-lcdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes],
+      [test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcdata in directory: $ac_cv_with_libcdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -524,15 +527,15 @@
     ])
   ])
 
 dnl Function to detect if libcdata dependencies are available
 AC_DEFUN([AX_LIBCDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
   ])
 
 dnl Function to detect how to enable libcdata
 AC_DEFUN([AX_LIBCDATA_CHECK_ENABLE],
```

### Comparing `libgzipf-20240103/m4/libcsplit.m4` & `libgzipf-20240422/m4/libcsplit.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcsplit required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcsplit is available
 dnl ac_libcsplit_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno],
     [ac_cv_libcsplit=no],
     [ac_cv_libcsplit=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcsplit which returns "yes" and --with-libcsplit= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect],
+      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcsplit"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcsplit],
           [1])
@@ -143,16 +145,17 @@
             libcsplit_wide_split_string_set_segment_by_index,
             [ac_cv_libcsplit_dummy=yes],
             [ac_cv_libcsplit=no])
           ])
 
         ac_cv_libcsplit_LIBADD="-lcsplit"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes],
+      [test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcsplit in directory: $ac_cv_with_libcsplit],
         [1])
       ])
     ])
 
   AS_IF(
@@ -174,15 +177,15 @@
     ])
   ])
 
 dnl Function to detect if libcsplit dependencies are available
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
   ])
 
 dnl Function to detect how to enable libcsplit
 AC_DEFUN([AX_LIBCSPLIT_CHECK_ENABLE],
```

### Comparing `libgzipf-20240103/m4/common.m4` & `libgzipf-20240422/m4/common.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for common headers and functions
 dnl
-dnl Version: 20181117
+dnl Version: 20240308
 
 dnl Function to test if a certain feature was disabled
 AC_DEFUN([AX_COMMON_ARG_DISABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
@@ -22,15 +22,15 @@
 dnl Function to test if a certain feature was enabled
 AC_DEFUN([AX_COMMON_ARG_ENABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
       [--enable-$1],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_enable_$2=$enableval],
     [ac_cv_enable_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to enable $3],
       [ac_cv_enable_$2],
       [ac_cv_enable_$2=$4])dnl
@@ -39,15 +39,15 @@
 dnl Function to test if the location of a certain feature was provided
 AC_DEFUN([AX_COMMON_ARG_WITH],
 [
   AC_ARG_WITH(
     [$1],
     [AS_HELP_STRING(
       [--with-$1[[=$5]]],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_with_$2=$withval],
     [ac_cv_with_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to use $3],
       [ac_cv_with_$2],
       [ac_cv_with_$2=$4])dnl
```

### Comparing `libgzipf-20240103/m4/libcthreads.m4` & `libgzipf-20240422/m4/libcthreads.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcthreads required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcthreads is available
 dnl ac_libcthreads_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCTHREADS_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno],
     [ac_cv_libcthreads=no],
     [ac_cv_libcthreads=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcthreads which returns "yes" and --with-libcthreads= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect],
+      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcthreads"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcthreads],
           [1])
@@ -244,15 +246,15 @@
           [ac_cv_libcthreads_dummy=yes],
           [ac_cv_libcthreads=no])
 
         ac_cv_libcthreads_LIBADD="-lcthreads"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes],
+      [test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcthreads in directory: $ac_cv_with_libcthreads],
         [1])
       ])
     ])
 
   AS_IF(
@@ -286,15 +288,15 @@
     [dnl Check for enabling pthread support
     AX_PTHREAD_CHECK_ENABLE
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread],
     [ac_cv_libcthreads_multi_threading="winapi"])
 
   AS_IF(
     [test "x$ac_cv_libcthreads_multi_threading" != xno],
-    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local],
     [ac_cv_libcthreads=no])
   ])
 
 dnl Function to detect how to enable libcthreads
```

### Comparing `libgzipf-20240103/m4/ltversion.m4` & `libgzipf-20240422/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/m4/ltsugar.m4` & `libgzipf-20240422/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/m4/libfdata.m4` & `libgzipf-20240422/m4/libfdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Functions for libfdata
 dnl
-dnl Version: 20230318
+dnl Version: 20240413
 
 dnl Function to detect if libfdata is available
 dnl ac_libfdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdata" = xno],
     [ac_cv_libfdata=no],
     [ac_cv_libfdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfdata which returns "yes" and --with-libfdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect],
+      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfdata],
           [1])
@@ -450,16 +452,17 @@
         dnl TODO: add functions
 
         dnl Vector list functions
         dnl TODO: add functions
 
         ac_cv_libfdata_LIBADD="-lfdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_libfdata" != xyes],
+      [test "x$ac_cv_libfdata" != xyes && test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfdata in directory: $ac_cv_with_libfdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -481,15 +484,15 @@
     ])
   ])
 
 dnl Function to detect if libfdata dependencies are available
 AC_DEFUN([AX_LIBFDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
   ])
 
 dnl Function to detect how to enable libfdata
 AC_DEFUN([AX_LIBFDATA_CHECK_ENABLE],
```

### Comparing `libgzipf-20240103/m4/host-cpu-c-abi.m4` & `libgzipf-20240422/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/m4/libfuse.m4` & `libgzipf-20240422/m4/libfuse.m4`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,90 @@
 dnl Checks for libfuse required headers and functions
 dnl
-dnl Version: 20220118
+dnl Version: 20240413
 
 dnl Function to detect if libfuse is available
 dnl ac_libfuse_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFUSE_CHECK_LIB],
-  [dnl Check if parameters were provided
-  AS_IF(
-    [test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_with_libfuse" != xauto-detect],
-    [AS_IF(
-      [test -d "$ac_cv_with_libfuse"],
-      [CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
-      LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"],
-      [AC_MSG_WARN([no such directory: $ac_cv_with_libfuse])
-      ])
-    ])
-
-  AS_IF(
-    [test "x$ac_cv_with_libfuse" = xno],
+  [AS_IF(
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfuse" = xno],
     [ac_cv_libfuse=no],
-    [dnl Check for a pkg-config file
+    [dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfuse which returns "yes" and --with-libfuse= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"],
-      [PKG_CHECK_MODULES(
-        [fuse],
-        [fuse >= 2.6],
-        [ac_cv_libfuse=libfuse],
-        [ac_cv_libfuse=no])
+      [test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_libfuse"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"],
+        [AC_MSG_FAILURE(
+          [no such directory: $ac_cv_with_libfuse],
+          [1])
+        ])],
+      [dnl Check for a pkg-config file
+      AS_IF(
+        [test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"],
+        [PKG_CHECK_MODULES(
+          [fuse3],
+          [fuse3 >= 3.0],
+          [ac_cv_libfuse=libfuse3],
+          [ac_cv_libfuse=no])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xno],
+          [PKG_CHECK_MODULES(
+            [fuse],
+            [fuse >= 2.6],
+            [ac_cv_libfuse=libfuse],
+            [ac_cv_libfuse=no])
+          ])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse3],
+          [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse3_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse3_LIBS"])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse],
+          [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"])
+        ])
       ])
 
+    backup_CPPFLAGS="$CPPFLAGS"
+
+    dnl Check for libfuse and libfuse3
     AS_IF(
-      [test "x$ac_cv_libfuse" = xlibfuse],
-      [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS"
-      ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"],
+      [test "x$ac_cv_libfuse" != xlibfuse && test "x$ac_cv_libfuse" != xlibfuse3],
       [dnl Check for headers
-      AC_CHECK_HEADERS(
-        [fuse.h],
-        [ac_cv_header_fuse_h=yes],
-        [ac_cv_header_fuse_h=no])
 
-      dnl libfuse sometimes requires -D_FILE_OFFSET_BITS=64 to be set
-      dnl macFuse requires -DFUSE_USE_VERSION=26 to be set
+      CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=30"
+      AC_CHECK_HEADERS([fuse.h])
+
       AS_IF(
-        [test "x$ac_cv_header_fuse_h" = xno],
-        [AS_UNSET([ac_cv_header_fuse_h])
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64 -DFUSE_USE_VERSION=26"
+        [test "x$ac_cv_header_fuse_h" = xyes],
+        [ac_cv_libfuse=libfuse3],
+        [CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
         AC_CHECK_HEADERS([fuse.h])
-      ])
+
+        AS_IF(
+          [test "x$ac_cv_header_fuse_h" = xyes],
+          [ac_cv_libfuse=libfuse])
+        ])
 
       AS_IF(
         [test "x$ac_cv_header_fuse_h" = xno],
         [ac_cv_libfuse=no],
         [dnl Check for the individual functions
-        ac_cv_libfuse=libfuse
+        AC_CHECK_LIB(
+          fuse,
+          fuse_invalidate,
+          [ac_cv_libfuse=libfuse],
+          [ac_cv_libfuse=libfuse3])
 
         AC_CHECK_LIB(
           fuse,
           fuse_daemonize,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
@@ -71,32 +99,30 @@
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
           fuse,
           fuse_new,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
 
-        ac_cv_libfuse_LIBADD="-lfuse";
+        dnl libfuse and libfuse3 require -D_FILE_OFFSET_BITS=64 to be set
+        ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse3],
+          [ac_cv_libfuse_LIBADD="-lfuse3"],
+          [ac_cv_libfuse_LIBADD="-lfuse"])
         ])
       ])
 
     dnl Check for libosxfuse
     AS_IF(
       [test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno],
-      [CPPFLAGS="$CPPFLAGS -DFUSE_USE_VERSION=26"
+      [CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
       AC_CHECK_HEADERS([osxfuse/fuse.h])
 
-      dnl libosxfuse sometimes requires -D_FILE_OFFSET_BITS=64 to be set
-      AS_IF(
-        [test "x$ac_cv_header_osxfuse_fuse_h" = xno],
-        [AS_UNSET([ac_cv_header_osxfuse_fuse_h])
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64"
-        AC_CHECK_HEADERS([osxfuse/fuse.h])
-      ])
-
       AS_IF(
         [test "x$ac_cv_header_osxfuse_fuse_h" = xno],
         [ac_cv_libfuse=no],
         [dnl Check for the individual functions
         ac_cv_libfuse=libosxfuse
 
         AC_CHECK_LIB(
@@ -116,27 +142,46 @@
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
           osxfuse,
           fuse_new,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
 
+        dnl libosxfuse requires -D_FILE_OFFSET_BITS=64 to be set
+        ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
         ac_cv_libfuse_LIBADD="-losxfuse";
         ])
       ])
+
+    AS_IF(
+      [test "x$ac_cv_libfuse" != xyes && test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported libfuse in directory: $ac_cv_with_libfuse],
+        [1])
+      ])
+
+    CPPFLAGS="$backup_CPPFLAGS"
     ])
 
   AS_IF(
     [test "x$ac_cv_libfuse" = xlibfuse],
     [AC_DEFINE(
       [HAVE_LIBFUSE],
       [1],
       [Define to 1 if you have the 'fuse' library (-lfuse).])
     ])
   AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_DEFINE(
+      [HAVE_LIBFUSE3],
+      [1],
+      [Define to 1 if you have the 'fuse3' library (-lfuse3).])
+    ])
+  AS_IF(
     [test "x$ac_cv_libfuse" = xlibosxfuse],
     [AC_DEFINE(
       [HAVE_LIBOSXFUSE],
       [1],
       [Define to 1 if you have the 'osxfuse' library (-losxfuse).])
     ])
 
@@ -179,14 +224,20 @@
   AS_IF(
     [test "x$ac_cv_libfuse" = xlibfuse],
     [AC_SUBST(
       [ax_libfuse_pc_libs_private],
       [-lfuse])
     ])
   AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_SUBST(
+      [ax_libfuse_pc_libs_private],
+      [-lfuse3])
+    ])
+  AS_IF(
     [test "x$ac_cv_libfuse" = xlibosxfuse],
     [AC_SUBST(
       [ax_libfuse_pc_libs_private],
       [-losxfuse])
     ])
 
   AS_IF(
@@ -194,9 +245,18 @@
     [AC_SUBST(
       [ax_libfuse_spec_requires],
       [fuse-libs])
     AC_SUBST(
       [ax_libfuse_spec_build_requires],
       [fuse-devel])
     ])
+  AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_SUBST(
+      [ax_libfuse_spec_requires],
+      [fuse3-libs])
+    AC_SUBST(
+      [ax_libfuse_spec_build_requires],
+      [fuse3-devel])
+    ])
   ])
```

### Comparing `libgzipf-20240103/m4/libtool.m4` & `libgzipf-20240422/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/m4/po.m4` & `libgzipf-20240422/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/m4/libcerror.m4` & `libgzipf-20240422/m4/libcerror.m4`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcerror required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcerror is available
 dnl ac_libcerror_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCERROR_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno],
     [ac_cv_libcerror=no],
     [ac_cv_libcerror=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcerror which returns "yes" and --with-libcerror= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect],
+      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcerror"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcerror],
           [1])
@@ -95,16 +97,17 @@
           cerror,
           libcerror_system_set_error,
           [ac_cv_libcerror_dummy=yes],
           [ac_cv_libcerror=no])
 
         ac_cv_libcerror_LIBADD="-lcerror"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes],
+      [test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcerror in directory: $ac_cv_with_libcerror],
         [1])
       ])
     ])
 
   AS_IF(
@@ -162,15 +165,15 @@
       [test "x$ac_cv_func_strerror" != xyes],
       [AC_MSG_FAILURE(
         [Missing functions: strerror_r and strerror],
         [1])
       ])
     ])
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
   ])
 
 dnl Function to detect how to enable libcerror
 AC_DEFUN([AX_LIBCERROR_CHECK_ENABLE],
```

### Comparing `libgzipf-20240103/m4/libcnotify.m4` & `libgzipf-20240422/m4/libcnotify.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcnotify required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcnotify is available
 dnl ac_libcnotify_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno],
     [ac_cv_libcnotify=no],
     [ac_cv_libcnotify=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcnotify which returns "yes" and --with-libcnotify= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect],
+      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcnotify"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcnotify],
           [1])
@@ -92,16 +94,17 @@
           cnotify,
           libcnotify_verbose_set,
           [ac_cv_libcnotify_dummy=yes],
           [ac_cv_libcnotify=no])
 
         ac_cv_libcnotify_LIBADD="-lcnotify"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes],
+      [test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcnotify in directory: $ac_cv_with_libcnotify],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
       [Missing headers: stdarg.h and varargs.h],
       [1])
     ])
 
   dnl Headers included in libcnotify/libcnotify_stream.c
   AC_CHECK_HEADERS([errno.h])
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
   ])
 
 dnl Function to detect how to enable libcnotify
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_ENABLE],
```

### Comparing `libgzipf-20240103/m4/libbfio.m4` & `libgzipf-20240422/m4/libbfio.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libbfio required headers and functions
 dnl
-dnl Version: 20201125
+dnl Version: 20240413
 
 dnl Function to detect if libbfio is available
 dnl ac_libbfio_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBBFIO_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno],
     [ac_cv_libbfio=no],
     [ac_cv_libbfio=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libbfio which returns "yes" and --with-libbfio= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect],
+      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libbfio"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libbfio],
           [1])
@@ -316,16 +318,17 @@
             libbfio_file_pool_open_wide,
             [ac_cv_libbfio_dummy=yes],
             [ac_cv_libbfio=no])
           ])
 
         ac_cv_libbfio_LIBADD="-lbfio"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes],
+      [test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libbfio in directory: $ac_cv_with_libbfio],
         [1])
       ])
     ])
 
   AS_IF(
@@ -347,15 +350,15 @@
     ])
   ])
 
 dnl Function to detect if libbfio dependencies are available
 AC_DEFUN([AX_LIBBFIO_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
   ])
 
 dnl Function to detect how to enable libbfio
 AC_DEFUN([AX_LIBBFIO_CHECK_ENABLE],
```

### Comparing `libgzipf-20240103/m4/intlmacosx.m4` & `libgzipf-20240422/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/m4/lt~obsolete.m4` & `libgzipf-20240422/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/m4/lib-link.m4` & `libgzipf-20240422/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/m4/iconv.m4` & `libgzipf-20240422/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/m4/ltoptions.m4` & `libgzipf-20240422/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/m4/nls.m4` & `libgzipf-20240422/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/m4/python.m4` & `libgzipf-20240422/m4/python.m4`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Functions for Python bindings
 dnl
-dnl Version: 20231119
+dnl Version: 20240418
 
 dnl Function to check if the python binary is available
 dnl "python${PYTHON_VERSION} python python# python#.#"
 AC_DEFUN([AX_PROG_PYTHON],
   [AS_IF(
     [test "x${PYTHON_VERSION}" != x],
     [ax_python_progs="python${PYTHON_VERSION}"],
@@ -72,18 +72,20 @@
     PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     AC_MSG_CHECKING(
       [for Python libraries])
     AC_MSG_RESULT(
       [$PYTHON_LDFLAGS])
 
-    dnl For CygWin add the -no-undefined linker flag
+    dnl For CygWin and MinGW add the -no-undefined linker flag
     AS_CASE(
-      [$host_os],
-      [cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [$build],
+      [*-*-cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-mingw*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-msys*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
       [*],[])
 
     dnl Check for the existence of Python.h
     BACKUP_CPPFLAGS="${CPPFLAGS}"
     CPPFLAGS="${CPPFLAGS} ${PYTHON_INCLUDES}"
 
     AC_CHECK_HEADERS(
```

### Comparing `libgzipf-20240103/m4/types.m4` & `libgzipf-20240422/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/m4/libfcache.m4` & `libgzipf-20240422/m4/libfcache.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfcache required headers and functions
 dnl
-dnl Version: 20230115
+dnl Version: 20240413
 
 dnl Function to detect if libfcache is available
 dnl ac_libfcache_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFCACHE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcache" = xno],
     [ac_cv_libfcache=no],
     [ac_cv_libfcache=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfcache which returns "yes" and --with-libfcache= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect],
+      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfcache"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfcache}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfcache}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfcache],
           [1])
@@ -147,16 +149,17 @@
           fcache,
           libfcache_date_time_get_timestamp,
           [ac_cv_libfcache_dummy=yes],
           [ac_cv_libfcache=no])
 
         ac_cv_libfcache_LIBADD="-lfcache"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_libfcache" != xyes],
+      [test "x$ac_cv_libfcache" != xyes && test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfcache in directory: $ac_cv_with_libfcache],
         [1])
       ])
     ])
 
   AS_IF(
@@ -192,15 +195,15 @@
   AS_IF(
     [test "x$ac_cv_func_time" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: time],
       [1])
     ])
 
-  ac_cv_libfcache_CPPFLAGS="-I../libfcache";
+  ac_cv_libfcache_CPPFLAGS="-I../libfcache -I\$(top_srcdir)/libfcache";
   ac_cv_libfcache_LIBADD="../libfcache/libfcache.la";
 
   ac_cv_libfcache=local
   ])
 
 dnl Function to detect how to enable libfcache
 AC_DEFUN([AX_LIBFCACHE_CHECK_ENABLE],
```

### Comparing `libgzipf-20240103/m4/pthread.m4` & `libgzipf-20240422/m4/pthread.m4`

 * *Files 18% similar despite different names*

```diff
@@ -1,183 +1,196 @@
 dnl Functions for pthread
 dnl
-dnl Version: 20130509
+dnl Version: 20240308
 
 dnl Function to detect if pthread is available
 AC_DEFUN([AX_PTHREAD_CHECK_LIB],
- [dnl Check if parameters were provided
- AS_IF(
-  [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect],
   [AS_IF(
-   [test -d "$ac_cv_with_pthread"],
-   [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
-   [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
-   ])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_with_pthread" = xno],
-  [ac_cv_pthread=no],
-  [dnl Check for headers
-  AC_CHECK_HEADERS([pthread.h])
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno],
+    [ac_cv_pthread=no],
+    [ac_cv_pthread=check
+    dnl Check if parameters were provided
+    dnl For both --with-pthread which returns "yes" and --with-pthread= which returns ""
+    dnl treat them as auto-detection.
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_pthread"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
+        [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
+        ])
+      ])
+    ])
+
+    AS_IF(
+      [test "x$ac_cv_pthread" = xcheck],
+      [dnl Check for headers
+      AC_CHECK_HEADERS([pthread.h])
+
+      AS_IF(
+        [test "x$ac_cv_header_pthread_h" = xno],
+        [ac_cv_pthread=no],
+        [dnl Check for the individual functions
+        ac_cv_pthread=pthread
+
+        dnl Thread functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_create,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_exit,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_join,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Condition functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_broadcast,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_signal,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_wait,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Mutex functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_lock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_trylock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Read/Write lock functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_rdlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_wrlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        ac_cv_pthread_LIBADD="-lpthread";
+      ])
+
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported pthread in directory: $ac_cv_with_pthread],
+        [1])
+      ])
+    ])
 
   AS_IF(
-   [test "x$ac_cv_header_pthread_h" = xno],
-   [ac_cv_pthread=no],
-   [dnl Check for the individual functions
-   ac_cv_pthread=pthread
-
-   dnl Thread functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_create,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_exit,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_join,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Condition functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_broadcast,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_signal,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_wait,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Mutex functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_lock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_trylock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Read/Write lock functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_rdlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_wrlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   ac_cv_pthread_LIBADD="-lpthread";
-   ])
-  ])
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_DEFINE(
+      [HAVE_PTHREAD],
+      [1],
+      [Define to 1 if you have the 'pthread' library (-lpthread).])
+    ])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_DEFINE(
-   [HAVE_PTHREAD],
-   [1],
-   [Define to 1 if you have the 'pthread' library (-lpthread).])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_pthread" != xno],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [1]) ],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [0])
+  AS_IF(
+    [test "x$ac_cv_pthread" != xno],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [1]) ],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [0])
+    ])
   ])
- ])
 
 dnl Function to detect how to enable pthread
 AC_DEFUN([AX_PTHREAD_CHECK_ENABLE],
- [AX_COMMON_ARG_WITH(
-  [pthread],
-  [pthread],
-  [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
-  [auto-detect],
-  [DIR])
-
- dnl Check for a shared library version
- AX_PTHREAD_CHECK_LIB
-
- AS_IF(
-  [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
-  [AC_SUBST(
-   [PTHREAD_CPPFLAGS],
-   [$ac_cv_pthread_CPPFLAGS])
-  ])
- AS_IF(
-  [test "x$ac_cv_pthread_LIBADD" != "x"],
-  [AC_SUBST(
-   [PTHREAD_LIBADD],
-   [$ac_cv_pthread_LIBADD])
-  ])
+  [AX_COMMON_ARG_WITH(
+    [pthread],
+    [pthread],
+    [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
+    [auto-detect],
+    [DIR])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_SUBST(
-   [ax_pthread_pc_libs_private],
-   [-lpthread])
+  dnl Check for a shared library version
+  AX_PTHREAD_CHECK_LIB
+
+  AS_IF(
+    [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
+    [AC_SUBST(
+      [PTHREAD_CPPFLAGS],
+      [$ac_cv_pthread_CPPFLAGS])
+    ])
+  AS_IF(
+    [test "x$ac_cv_pthread_LIBADD" != "x"],
+    [AC_SUBST(
+      [PTHREAD_LIBADD],
+      [$ac_cv_pthread_LIBADD])
+    ])
+
+  AS_IF(
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_SUBST(
+      [ax_pthread_pc_libs_private],
+      [-lpthread])
+    ])
   ])
- ])
```

### Comparing `libgzipf-20240103/m4/zlib.m4` & `libgzipf-20240422/m4/zlib.m4`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 dnl Checks for zlib required headers and functions
 dnl
-dnl Version: 20201230
+dnl Version: 20240314
 
 dnl Function to detect if zlib is available
 AC_DEFUN([AX_ZLIB_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_zlib" = xno],
     [ac_cv_zlib=no],
     [ac_cv_zlib=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-zlib which returns "yes" and --with-zlib= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect],
+      [test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect && test "x$ac_cv_with_zlib" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_zlib"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_zlib}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_zlib}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_zlib],
           [1])
@@ -58,14 +60,21 @@
             [Missing function: zlibVersion in library: zlib.],
             [1])
           ])
 
         ac_cv_zlib_LIBADD="-lz";
         ])
       ])
+
+    AS_IF(
+      [test "x$ac_cv_zlib" != xyes && test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect && test "x$ac_cv_with_zlib" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported zlib in directory: $ac_cv_with_zlib],
+        [1])
+      ])
     ])
 
   AS_IF(
     [test "x$ac_cv_zlib" = xzlib],
     [AC_DEFINE(
       [HAVE_ZLIB],
       [1],
```

### Comparing `libgzipf-20240103/include/libgzipf.h.in` & `libgzipf-20240422/include/libgzipf.h.in`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/include/libgzipf/definitions.h.in` & `libgzipf-20240422/include/libgzipf/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/include/libgzipf/definitions.h` & `libgzipf-20240422/include/libgzipf/definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBGZIPF_DEFINITIONS_H )
 #define _LIBGZIPF_DEFINITIONS_H
 
 #include <libgzipf/types.h>
 
-#define LIBGZIPF_VERSION		20240103
+#define LIBGZIPF_VERSION		20240422
 
 /* The libgzipf version string
  */
-#define LIBGZIPF_VERSION_STRING		"20240103"
+#define LIBGZIPF_VERSION_STRING		"20240422"
 
 /* The libgzipf file access
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBGZIPF_ACCESS_FLAGS
```

### Comparing `libgzipf-20240103/include/libgzipf/types.h.in` & `libgzipf-20240422/include/libgzipf/types.h.in`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/include/libgzipf/types.h` & `libgzipf-20240422/include/libgzipf/types.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/include/libgzipf/features.h.in` & `libgzipf-20240422/include/libgzipf/features.h.in`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/include/libgzipf/error.h` & `libgzipf-20240422/include/libgzipf/error.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/include/libgzipf/extern.h` & `libgzipf-20240422/include/libgzipf/extern.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/include/libgzipf/features.h` & `libgzipf-20240422/include/libgzipf/features.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/include/libgzipf/codepage.h` & `libgzipf-20240422/include/libgzipf/codepage.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/include/libgzipf.h` & `libgzipf-20240422/include/libgzipf.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/include/Makefile.in` & `libgzipf-20240422/include/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -437,14 +437,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -517,15 +519,20 @@
 
 EXTRA_DIST = \
 	libgzipf.h.in \
 	libgzipf/definitions.h.in \
 	libgzipf/features.h.in \
 	libgzipf/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libgzipf.h \
+	libgzipf/definitions.h \
+	libgzipf/features.h \
+	libgzipf/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -722,23 +729,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -820,17 +829,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libgzipf.h
-	-rm -f libgzipf/definitions.h
-	-rm -f libgzipf/features.h
-	-rm -f libgzipf/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libgzipf-20240103/common/config_borlandc.h` & `libgzipf-20240422/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/common/file_stream.h` & `libgzipf-20240422/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/common/memory.h` & `libgzipf-20240422/common/memory.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/common/byte_stream.h` & `libgzipf-20240422/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/common/common.h` & `libgzipf-20240422/common/common.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/common/config_winapi.h` & `libgzipf-20240422/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/common/system_string.h` & `libgzipf-20240422/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/common/types.h.in` & `libgzipf-20240422/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/common/types.h` & `libgzipf-20240422/common/types.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/common/config.h.in` & `libgzipf-20240422/common/config.h.in`

 * *Files 0% similar despite different names*

```diff
@@ -206,14 +206,17 @@
 
 /* Define to 1 if you have the <libfdatetime.h> header file. */
 #undef HAVE_LIBFDATETIME_H
 
 /* Define to 1 if you have the 'fuse' library (-lfuse). */
 #undef HAVE_LIBFUSE
 
+/* Define to 1 if you have the 'fuse3' library (-lfuse3). */
+#undef HAVE_LIBFUSE3
+
 /* Define to 1 if you have the <libintl.h> header file. */
 #undef HAVE_LIBINTL_H
 
 /* Define to 1 if you have the 'osxfuse' library (-losxfuse). */
 #undef HAVE_LIBOSXFUSE
 
 /* Define to 1 if you have the `una' library (-luna). */
```

### Comparing `libgzipf-20240103/common/config.h` & `libgzipf-20240422/common/config.h`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,18 @@
 /* Define to 1 if you have the `fdatetime' library (-lfdatetime). */
 /* #undef HAVE_LIBFDATETIME */
 
 /* Define to 1 if you have the <libfdatetime.h> header file. */
 /* #undef HAVE_LIBFDATETIME_H */
 
 /* Define to 1 if you have the 'fuse' library (-lfuse). */
-#define HAVE_LIBFUSE 1
+/* #undef HAVE_LIBFUSE */
+
+/* Define to 1 if you have the 'fuse3' library (-lfuse3). */
+#define HAVE_LIBFUSE3 1
 
 /* Define to 1 if you have the <libintl.h> header file. */
 #define HAVE_LIBINTL_H 1
 
 /* Define to 1 if you have the 'osxfuse' library (-losxfuse). */
 /* #undef HAVE_LIBOSXFUSE */
 
@@ -548,24 +551,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libgzipf"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libgzipf 20240103"
+#define PACKAGE_STRING "libgzipf 20240422"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libgzipf"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240103"
+#define PACKAGE_VERSION "20240422"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -586,15 +589,15 @@
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Define to 1 if your <sys/time.h> declares `struct tm'. */
 /* #undef TM_IN_SYS_TIME */
 
 /* Version number of package */
-#define VERSION "20240103"
+#define VERSION "20240422"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libgzipf-20240103/common/wide_string.h` & `libgzipf-20240422/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/common/narrow_string.h` & `libgzipf-20240422/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/common/config_msc.h` & `libgzipf-20240422/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/common/Makefile.in` & `libgzipf-20240422/common/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -407,14 +407,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -470,15 +472,17 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
-AM_CPPFLAGS = -I$(top_srcdir)/include
+AM_CPPFLAGS = \
+	-I../include -I$(top_srcdir)/include
+
 EXTRA_DIST = \
 	byte_stream.h \
 	common.h \
 	config.h \
 	config_borlandc.h \
 	config_msc.h \
 	config_winapi.h \
@@ -486,15 +490,18 @@
 	memory.h \
 	narrow_string.h \
 	system_string.h \
 	types.h \
 	types.h.in \
 	wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	config.h \
+	types.h \
+	Makefile \
 	Makefile.in
 
 all: config.h
 	$(MAKE) $(AM_MAKEFLAGS) all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -662,23 +669,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-hdr distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -758,15 +767,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f config.h
-	-rm -f types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libgzipf-20240103/libclocale/libclocale_wide_string.c` & `libgzipf-20240422/libclocale/libclocale_wide_string.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Wide character string functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libclocale/libclocale_support.h` & `libgzipf-20240422/libclocale/libclocale_support.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libclocale/Makefile.am` & `libgzipf-20240422/libclocale/Makefile.am`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 if HAVE_LOCAL_LIBCLOCALE
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libclocale.la
 
 libclocale_la_SOURCES = \
 	libclocale_codepage.c libclocale_codepage.h \
 	libclocale_definitions.h \
@@ -14,17 +14,17 @@
 	libclocale_libcerror.h \
 	libclocale_locale.c libclocale_locale.h \
 	libclocale_support.c libclocale_support.h \
 	libclocale_unused.h \
 	libclocale_wide_string.c libclocale_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
```

### Comparing `libgzipf-20240103/libclocale/libclocale_definitions.h` & `libgzipf-20240422/libclocale/libclocale_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -30,19 +30,19 @@
 #include <libclocale/definitions.h>
 
 /* The definitions in <libclocale/definitions.h> are copied here
  * for local use of libclocale
  */
 #else
 
-#define LIBCLOCALE_VERSION					20221218
+#define LIBCLOCALE_VERSION					20240414
 
 /* The libclocale version string
  */
-#define LIBCLOCALE_VERSION_STRING				"20221218"
+#define LIBCLOCALE_VERSION_STRING				"20240414"
 
 /* The codepage feature flag definitions
  */
 enum LIBCLOCALE_CODEPAGES_FEATURE_FLAGS
 {
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_ISO_8859		= 0x00000001UL,
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_KOI8		= 0x00000002UL,
```

### Comparing `libgzipf-20240103/libclocale/libclocale_unused.h` & `libgzipf-20240422/libclocale/libclocale_unused.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libclocale/libclocale_libcerror.h` & `libgzipf-20240422/libclocale/libclocale_libcerror.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcerror header
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libclocale/libclocale_locale.h` & `libgzipf-20240422/libclocale/libclocale_locale.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Locale functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libclocale/libclocale_support.c` & `libgzipf-20240422/libclocale/libclocale_support.c`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -64,15 +64,15 @@
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
 		 "%s: invalid domain name.",
 		 function );
 
 		return( -1 );
 	}
-#if defined( HAVE_BINDTEXTDOMAIN ) && defined( HAVE_TEXTDOMAIN )
+#if defined( HAVE_BINDTEXTDOMAIN ) && defined( HAVE_TEXTDOMAIN ) && defined( LOCALEDIR )
 	if( bindtextdomain(
 	     domain_name,
 	     LOCALEDIR ) == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
@@ -90,15 +90,15 @@
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
 		 "%s: unable to set text domain.",
 		 function );
 
 		return( -1 );
 	}
-#endif /* defined( HAVE_BINDTEXTDOMAIN ) && defined( HAVE_TEXTDOMAIN ) */
+#endif /* defined( HAVE_BINDTEXTDOMAIN ) && defined( HAVE_TEXTDOMAIN ) && defined( LOCALEDIR ) */
 
 #if !defined( HAVE_WIDE_SYSTEM_CHARACTER )
 	if( libclocale_locale_get_codepage(
 	     &codepage,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
```

### Comparing `libgzipf-20240103/libclocale/libclocale_codepage.c` & `libgzipf-20240422/libclocale/libclocale_codepage.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Codepage functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libclocale/libclocale_locale.c` & `libgzipf-20240422/libclocale/libclocale_locale.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Locale functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libclocale/Makefile.in` & `libgzipf-20240422/libclocale/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -451,14 +451,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -516,30 +518,31 @@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBCLOCALE_TRUE@AM_CPPFLAGS = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	-DLOCALEDIR=\"$(datadir)/locale\" \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCLOCALE_TRUE@noinst_LTLIBRARIES = libclocale.la
 @HAVE_LOCAL_LIBCLOCALE_TRUE@libclocale_la_SOURCES = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_codepage.c libclocale_codepage.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_definitions.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_extern.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_libcerror.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_locale.c libclocale_locale.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_support.c libclocale_support.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_unused.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_wide_string.c libclocale_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -742,24 +745,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libclocale_codepage.Plo
+	-rm -f ./$(DEPDIR)/libclocale_locale.Plo
+	-rm -f ./$(DEPDIR)/libclocale_support.Plo
+	-rm -f ./$(DEPDIR)/libclocale_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -820,14 +829,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -838,23 +849,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libgzipf-20240103/libclocale/libclocale_extern.h` & `libgzipf-20240422/libclocale/libclocale_extern.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libclocale/libclocale_wide_string.h` & `libgzipf-20240422/libclocale/libclocale_wide_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Wide character string functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libclocale/libclocale_codepage.h` & `libgzipf-20240422/libclocale/libclocale_codepage.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Codepage functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfcache/libfcache_libcdata.h` & `libgzipf-20240422/libfcache/libfcache_libcdata.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfcache/libfcache_types.h` & `libgzipf-20240422/libfcache/libfcache_types.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfcache/libfcache_cache_value.c` & `libgzipf-20240422/libfcache/libfcache_cache_value.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Cache value functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfcache/libfcache_unused.h` & `libgzipf-20240422/libfcache/libfcache_unused.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfcache/Makefile.am` & `libgzipf-20240422/libfcache/Makefile.am`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFCACHE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfcache.la
 
@@ -19,17 +19,17 @@
 	libfcache_libcdata.h \
 	libfcache_libcerror.h \
 	libfcache_support.c libfcache_support.h \
 	libfcache_types.h \
 	libfcache_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libfcache ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcache_la_SOURCES)
```

### Comparing `libgzipf-20240103/libfcache/libfcache_support.h` & `libgzipf-20240422/libfcache/libfcache_support.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfcache/libfcache_error.h` & `libgzipf-20240422/libfcache/libfcache_error.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfcache/libfcache_support.c` & `libgzipf-20240422/libcnotify/libcnotify_support.c`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -18,24 +18,22 @@
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
 #include <types.h>
 
-#include <stdio.h>
+#include "libcnotify_definitions.h"
+#include "libcnotify_support.h"
 
-#include "libfcache_definitions.h"
-#include "libfcache_support.h"
-
-#if !defined( HAVE_LOCAL_LIBFCACHE )
+#if !defined( HAVE_LOCAL_LIBCNOTIFY )
 
 /* Returns the library version as a string
  */
-const char *libfcache_get_version(
+const char *libcnotify_get_version(
              void )
 {
-	return( (const char *) LIBFCACHE_VERSION_STRING );
+	return( (const char *) LIBCNOTIFY_VERSION_STRING );
 }
 
-#endif /* !defined( HAVE_LOCAL_LIBFCACHE ) */
+#endif /* !defined( HAVE_LOCAL_LIBCNOTIFY ) */
```

### Comparing `libgzipf-20240103/libfcache/libfcache_cache.h` & `libgzipf-20240422/libfcache/libfcache_cache.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The cache functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfcache/libfcache_error.c` & `libgzipf-20240422/libfcache/libfcache_error.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfcache/libfcache_libcerror.h` & `libgzipf-20240422/libfcache/libfcache_libcerror.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfcache/libfcache_date_time.c` & `libgzipf-20240422/libfcache/libfcache_date_time.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Date and time functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfcache/libfcache_extern.h` & `libgzipf-20240422/libfcache/libfcache_extern.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfcache/libfcache_cache_value.h` & `libgzipf-20240422/libfcache/libfcache_cache_value.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Cache value functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfcache/Makefile.in` & `libgzipf-20240422/libfcache/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -454,14 +454,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -518,16 +520,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBFCACHE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFCACHE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFCACHE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFCACHE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFCACHE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFCACHE_TRUE@noinst_LTLIBRARIES = libfcache.la
 @HAVE_LOCAL_LIBFCACHE_TRUE@libfcache_la_SOURCES = \
@@ -539,15 +541,16 @@
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_extern.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_libcdata.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_libcerror.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_support.c libfcache_support.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_types.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -751,24 +754,31 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfcache_cache.Plo
+	-rm -f ./$(DEPDIR)/libfcache_cache_value.Plo
+	-rm -f ./$(DEPDIR)/libfcache_date_time.Plo
+	-rm -f ./$(DEPDIR)/libfcache_error.Plo
+	-rm -f ./$(DEPDIR)/libfcache_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -830,14 +840,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -848,23 +860,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libfcache ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcache_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libgzipf-20240103/libfcache/libfcache_date_time.h` & `libgzipf-20240422/libfcache/libfcache_date_time.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Date and time functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfcache/libfcache_definitions.h` & `libgzipf-20240422/libfcache/libfcache_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBFCACHE )
 #include <libfcache/definitions.h>
 
 /* The definitions in <libfcache/definitions.h> are copied here
  * for local use of libfcache
  */
 #else
-#define LIBFCACHE_VERSION					20230115
+#define LIBFCACHE_VERSION					20240414
 
 /* The libfcache version string
  */
-#define LIBFCACHE_VERSION_STRING				"20230115"
+#define LIBFCACHE_VERSION_STRING				"20240414"
 
 /* The cache value flags definitions
  */
 enum LIBFCACHE_CACHE_VALUE_FLAGS
 {
 	/* The cache value is not managed by the library
 	 */
```

### Comparing `libgzipf-20240103/libfcache/libfcache_cache.c` & `libgzipf-20240422/libfcache/libfcache_cache.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The cache functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/Makefile.am` & `libgzipf-20240422/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -58,16 +58,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libgzipf.pc \
+	libgzipf.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libgzipf.pc
 
 libtool: @LIBTOOL_DEPS@
@@ -89,19 +96,7 @@
 	(cd $(srcdir)/libbfio && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfcache && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdata && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libgzipf && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libgzipf.pc
-	-rm -f libgzipf.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libgzipf-20240103/libbfio/libbfio_file_range.h` & `libgzipf-20240422/libbfio/libbfio_file_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_file_range_io_handle.c` & `libgzipf-20240422/libbfio/libbfio_file_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_support.c` & `libgzipf-20240422/libbfio/libbfio_support.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_libcpath.h` & `libgzipf-20240422/libbfio/libbfio_libcpath.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcpath header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_error.h` & `libgzipf-20240422/libbfio/libbfio_error.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_libclocale.h` & `libgzipf-20240422/libbfio/libbfio_libclocale.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libclocale header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_error.c` & `libgzipf-20240422/libbfio/libbfio_error.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_libuna.h` & `libgzipf-20240422/libbfio/libbfio_libuna.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libuna header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_file_io_handle.h` & `libgzipf-20240422/libbfio/libbfio_file_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_file_pool.h` & `libgzipf-20240422/libbfio/libbfio_file_pool.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_file_range.c` & `libgzipf-20240422/libbfio/libbfio_file_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_types.h` & `libgzipf-20240422/libbfio/libbfio_types.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_unused.h` & `libgzipf-20240422/libbfio/libbfio_unused.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_libcdata.h` & `libgzipf-20240422/libbfio/libbfio_libcdata.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_file.h` & `libgzipf-20240422/libbfio/libbfio_file.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/Makefile.am` & `libgzipf-20240422/libbfio/Makefile.am`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBBFIO
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -38,17 +38,17 @@
 	libbfio_pool.c libbfio_pool.h \
 	libbfio_support.c libbfio_support.h \
 	libbfio_system_string.c libbfio_system_string.h \
 	libbfio_types.h \
 	libbfio_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
```

### Comparing `libgzipf-20240103/libbfio/libbfio_libcfile.h` & `libgzipf-20240422/libbfio/libbfio_libcfile.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcfile header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_definitions.h` & `libgzipf-20240422/libbfio/libbfio_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBBFIO )
 #include <libbfio/definitions.h>
 
 /* The definitions in <libbfio/definitions.h> are copied here
  * for local use of libbfio
  */
 #else
-#define LIBBFIO_VERSION					20221025
+#define LIBBFIO_VERSION					20240414
 
 /* The libbfio version string
  */
-#define LIBBFIO_VERSION_STRING				"20221025"
+#define LIBBFIO_VERSION_STRING				"20240414"
 
 /* The library flags definitions
  */
 enum LIBBFIO_FLAGS
 {
 	/* The IO handle is not managed by the library
 	 */
```

### Comparing `libgzipf-20240103/libbfio/libbfio_codepage.h` & `libgzipf-20240422/libbfio/libbfio_codepage.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Codepage functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_file_io_handle.c` & `libgzipf-20240422/libbfio/libbfio_file_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_support.h` & `libgzipf-20240422/libbfio/libbfio_support.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_memory_range.h` & `libgzipf-20240422/libbfio/libbfio_memory_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_file_pool.c` & `libgzipf-20240422/libbfio/libbfio_file_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_file_range_io_handle.h` & `libgzipf-20240422/libbfio/libbfio_file_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_libcthreads.h` & `libgzipf-20240422/libbfio/libbfio_libcthreads.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcthreads header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_system_string.h` & `libgzipf-20240422/libbfio/libbfio_system_string.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_memory_range_io_handle.c` & `libgzipf-20240422/libbfio/libbfio_memory_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_handle.c` & `libgzipf-20240422/libbfio/libbfio_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_file.c` & `libgzipf-20240422/libbfio/libbfio_file.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_handle.h` & `libgzipf-20240422/libbfio/libbfio_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_memory_range.c` & `libgzipf-20240422/libbfio/libbfio_memory_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_pool.c` & `libgzipf-20240422/libbfio/libbfio_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_libcerror.h` & `libgzipf-20240422/libbfio/libbfio_libcerror.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/Makefile.in` & `libgzipf-20240422/libbfio/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -472,14 +472,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -536,16 +538,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBBFIO_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCFILE_CPPFLAGS@ \
@@ -576,15 +578,16 @@
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_memory_range_io_handle.c libbfio_memory_range_io_handle.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_pool.c libbfio_pool.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_support.c libbfio_support.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_system_string.c libbfio_system_string.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_types.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -795,24 +798,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libbfio_error.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_support.Plo
+	-rm -f ./$(DEPDIR)/libbfio_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -881,14 +898,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -899,23 +918,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libgzipf-20240103/libbfio/libbfio_system_string.c` & `libgzipf-20240422/libbfio/libbfio_system_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_memory_range_io_handle.h` & `libgzipf-20240422/libbfio/libbfio_memory_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_extern.h` & `libgzipf-20240422/libbfio/libbfio_extern.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libbfio/libbfio_pool.h` & `libgzipf-20240422/libbfio/libbfio_pool.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/config.guess` & `libgzipf-20240422/config.guess`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/dpkg/copyright` & `libgzipf-20240422/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/dpkg/control` & `libgzipf-20240422/dpkg/control`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/dpkg/rules` & `libgzipf-20240422/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf.spec` & `libgzipf-20240422/libgzipf.spec`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libgzipf
-Version: 20240103
+Version: 20240422
 Release: 1
 Summary: Library to access the GZIP file format
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libgzipf
 Requires:              zlib
@@ -36,16 +36,16 @@
 
 %description -n libgzipf-python3
 Python 3 bindings for libgzipf
 
 %package -n libgzipf-tools
 Summary: Several tools for reading GZIP files
 Group: Applications/System
-Requires: libgzipf = %{version}-%{release} fuse-libs
-BuildRequires: fuse-devel
+Requires: libgzipf = %{version}-%{release} fuse3-libs
+BuildRequires: fuse3-devel
 
 %description -n libgzipf-tools
 Several tools for reading GZIP files
 
 %prep
 %setup -q
 
@@ -91,10 +91,10 @@
 %files -n libgzipf-tools
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Wed Jan  3 2024 Joachim Metz <joachim.metz@gmail.com> 20240103-1
+* Mon Apr 22 2024 Joachim Metz <joachim.metz@gmail.com> 20240422-1
 - Auto-generated
```

### Comparing `libgzipf-20240103/COPYING.LESSER` & `libgzipf-20240422/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf.pc.in` & `libgzipf-20240422/libgzipf.pc.in`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/configure` & `libgzipf-20240422/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libgzipf 20240103.
+# Generated by GNU Autoconf 2.71 for libgzipf 20240422.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='libgzipf'
 PACKAGE_TARNAME='libgzipf'
-PACKAGE_VERSION='20240103'
-PACKAGE_STRING='libgzipf 20240103'
+PACKAGE_VERSION='20240422'
+PACKAGE_STRING='libgzipf 20240422'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libgzipf.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -678,14 +678,16 @@
 ax_libfuse_spec_requires
 ax_libfuse_pc_libs_private
 LIBFUSE_LIBADD
 LIBFUSE_CPPFLAGS
 HAVE_LIBFUSE
 fuse_LIBS
 fuse_CFLAGS
+fuse3_LIBS
+fuse3_CFLAGS
 HAVE_PYTHON_TESTS_FALSE
 HAVE_PYTHON_TESTS_TRUE
 HAVE_PYTHON_FALSE
 HAVE_PYTHON_TRUE
 PYTHON_PACKAGE_DIR
 PYTHON_LIBRARY_DIR
 pyexecdir
@@ -1100,14 +1102,16 @@
 libfcache_LIBS
 libfdata_CFLAGS
 libfdata_LIBS
 libfdatetime_CFLAGS
 libfdatetime_LIBS
 zlib_CFLAGS
 zlib_LIBS
+fuse3_CFLAGS
+fuse3_LIBS
 fuse_CFLAGS
 fuse_LIBS'
 
 
 # Initialize some variables set by options.
 ac_init_help=
 ac_init_version=false
@@ -1650,15 +1654,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libgzipf 20240103 to adapt to many kinds of systems.
+\`configure' configures libgzipf 20240422 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1721,15 +1725,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libgzipf 20240103:";;
+     short | recursive ) echo "Configuration of libgzipf 20240422:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1899,14 +1903,17 @@
               linker flags for libfdata, overriding pkg-config
   libfdatetime_CFLAGS
               C compiler flags for libfdatetime, overriding pkg-config
   libfdatetime_LIBS
               linker flags for libfdatetime, overriding pkg-config
   zlib_CFLAGS C compiler flags for zlib, overriding pkg-config
   zlib_LIBS   linker flags for zlib, overriding pkg-config
+  fuse3_CFLAGS
+              C compiler flags for fuse3, overriding pkg-config
+  fuse3_LIBS  linker flags for fuse3, overriding pkg-config
   fuse_CFLAGS C compiler flags for fuse, overriding pkg-config
   fuse_LIBS   linker flags for fuse, overriding pkg-config
 
 Use these variables to override the choices made by `configure' or to help
 it to find libraries and programs with nonstandard names/locations.
 
 Report bugs to <joachim.metz@gmail.com>.
@@ -1969,15 +1976,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libgzipf configure 20240103
+libgzipf configure 20240422
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2690,15 +2697,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libgzipf $as_me 20240103, which was
+It was created by libgzipf $as_me 20240422, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4179,15 +4186,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libgzipf'
- VERSION='20240103'
+ VERSION='20240422'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23774,15 +23781,15 @@
 printf "%s\n" "$ac_cv_with_libcerror" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno
 then :
   ac_cv_libcerror=no
 else $as_nop
   ac_cv_libcerror=check
-        if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect
+                if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   if test -d "$ac_cv_with_libcerror"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -24273,15 +24280,16 @@
 fi
 
 
         ac_cv_libcerror_LIBADD="-lcerror"
 fi
 
 fi
-    if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes
+
+    if test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcerror in directory: $ac_cv_with_libcerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -24423,15 +24431,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24525,15 +24533,15 @@
     ac_cv_libcthreads_multi_threading="no"
 else $as_nop
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno
 then :
   ac_cv_libcthreads=no
 else $as_nop
   ac_cv_libcthreads=check
-        if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect
+                if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   if test -d "$ac_cv_with_libcthreads"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -26165,15 +26173,15 @@
 
 
         ac_cv_libcthreads_LIBADD="-lcthreads"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes
+    if test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcthreads in directory: $ac_cv_with_libcthreads
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -26227,47 +26235,52 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_pthread=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_pthread" >&5
 printf "%s\n" "$ac_cv_with_pthread" >&6; }
 
-   if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno
+then :
+  ac_cv_pthread=no
+else $as_nop
+  ac_cv_pthread=check
+                if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
 then :
   if test -d "$ac_cv_with_pthread"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
 else $as_nop
   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_pthread" >&5
 printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_pthread" >&2;}
 
 fi
 
 fi
 
- if test "x$ac_cv_with_pthread" = xno
+fi
+
+    if test "x$ac_cv_pthread" = xcheck
 then :
-  ac_cv_pthread=no
-else $as_nop
-    ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
+        ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
 if test "x$ac_cv_header_pthread_h" = xyes
 then :
   printf "%s\n" "#define HAVE_PTHREAD_H 1" >>confdefs.h
 
 fi
 
 
-  if test "x$ac_cv_header_pthread_h" = xno
+      if test "x$ac_cv_header_pthread_h" = xno
 then :
   ac_cv_pthread=no
 else $as_nop
-     ac_cv_pthread=pthread
+          ac_cv_pthread=pthread
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
 printf %s "checking for pthread_create in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_create+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26301,15 +26314,15 @@
 if test "x$ac_cv_lib_pthread_pthread_create" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
 printf %s "checking for pthread_exit in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_exit+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26343,15 +26356,15 @@
 if test "x$ac_cv_lib_pthread_pthread_exit" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
 printf %s "checking for pthread_join in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_join+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26386,15 +26399,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
 printf %s "checking for pthread_cond_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26428,15 +26441,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
 printf %s "checking for pthread_cond_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26470,15 +26483,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
 printf %s "checking for pthread_cond_broadcast in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_broadcast+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26512,15 +26525,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_broadcast" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
 printf %s "checking for pthread_cond_signal in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_signal+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26554,15 +26567,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_signal" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
 printf %s "checking for pthread_cond_wait in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_wait+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26597,15 +26610,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
 printf %s "checking for pthread_mutex_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26639,15 +26652,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
 printf %s "checking for pthread_mutex_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26681,15 +26694,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
 printf %s "checking for pthread_mutex_lock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_lock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26723,15 +26736,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_lock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
 printf %s "checking for pthread_mutex_trylock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_trylock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26765,15 +26778,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_trylock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
 printf %s "checking for pthread_mutex_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26808,15 +26821,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
 printf %s "checking for pthread_rwlock_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26850,15 +26863,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
 printf %s "checking for pthread_rwlock_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26892,15 +26905,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_rdlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_rdlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26934,15 +26947,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_rdlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_wrlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_wrlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26976,15 +26989,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_wrlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27019,67 +27032,76 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-   ac_cv_pthread_LIBADD="-lpthread";
+        ac_cv_pthread_LIBADD="-lpthread";
+
+fi
+
+    if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported pthread in directory: $ac_cv_with_pthread
+See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
 
 printf "%s\n" "#define HAVE_PTHREAD 1" >>confdefs.h
 
 
 fi
 
- if test "x$ac_cv_pthread" != xno
+  if test "x$ac_cv_pthread" != xno
 then :
   HAVE_PTHREAD=1
 
 else $as_nop
   HAVE_PTHREAD=0
 
 
 fi
 
 
- if test "x$ac_cv_pthread_CPPFLAGS" != "x"
+  if test "x$ac_cv_pthread_CPPFLAGS" != "x"
 then :
   PTHREAD_CPPFLAGS=$ac_cv_pthread_CPPFLAGS
 
 
 fi
- if test "x$ac_cv_pthread_LIBADD" != "x"
+  if test "x$ac_cv_pthread_LIBADD" != "x"
 then :
   PTHREAD_LIBADD=$ac_cv_pthread_LIBADD
 
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
   ax_pthread_pc_libs_private=-lpthread
 
 
 fi
 
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread
 else $as_nop
   ac_cv_libcthreads_multi_threading="winapi"
 fi
 
   if test "x$ac_cv_libcthreads_multi_threading" != xno
 then :
-  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local
 else $as_nop
   ac_cv_libcthreads=no
 fi
 
@@ -27167,15 +27189,15 @@
 printf "%s\n" "$ac_cv_with_libcdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno
 then :
   ac_cv_libcdata=no
 else $as_nop
   ac_cv_libcdata=check
-        if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect
+                if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   if test -d "$ac_cv_with_libcdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -30946,15 +30968,16 @@
 fi
 
 
         ac_cv_libcdata_LIBADD="-lcdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes
+
+    if test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcdata in directory: $ac_cv_with_libcdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -30979,15 +31002,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -31057,15 +31080,15 @@
 printf "%s\n" "$ac_cv_with_libclocale" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno
 then :
   ac_cv_libclocale=no
 else $as_nop
   ac_cv_libclocale=check
-        if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect
+                if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   if test -d "$ac_cv_with_libclocale"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -31612,15 +31635,16 @@
 fi
 
 
         ac_cv_libclocale_LIBADD="-lclocale"
 fi
 
 fi
-    if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes
+
+    if test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libclocale in directory: $ac_cv_with_libclocale
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31776,15 +31800,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -31854,15 +31878,15 @@
 printf "%s\n" "$ac_cv_with_libcnotify" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno
 then :
   ac_cv_libcnotify=no
 else $as_nop
   ac_cv_libcnotify=check
-        if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect
+                if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   if test -d "$ac_cv_with_libcnotify"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -32312,15 +32336,16 @@
 fi
 
 
         ac_cv_libcnotify_LIBADD="-lcnotify"
 fi
 
 fi
-    if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes
+
+    if test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcnotify in directory: $ac_cv_with_libcnotify
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -32375,15 +32400,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -32453,15 +32478,15 @@
 printf "%s\n" "$ac_cv_with_libcsplit" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno
 then :
   ac_cv_libcsplit=no
 else $as_nop
   ac_cv_libcsplit=check
-        if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect
+                if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   if test -d "$ac_cv_with_libcsplit"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -33176,15 +33201,16 @@
 
 fi
 
         ac_cv_libcsplit_LIBADD="-lcsplit"
 fi
 
 fi
-    if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes
+
+    if test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcsplit in directory: $ac_cv_with_libcsplit
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -33209,15 +33235,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcsplit" != xyes
 then :
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCSPLIT 1" >>confdefs.h
@@ -33287,15 +33313,15 @@
 printf "%s\n" "$ac_cv_with_libuna" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno
 then :
   ac_cv_libuna=no
 else $as_nop
   ac_cv_libuna=check
-        if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect
+                if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   if test -d "$ac_cv_with_libuna"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -40497,15 +40523,16 @@
   ac_cv_libuna=no
 fi
 
         ac_cv_libuna_LIBADD="-luna"
 fi
 
 fi
-    if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes
+
+    if test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libuna in directory: $ac_cv_with_libuna
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -40530,15 +40557,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -40608,15 +40635,15 @@
 printf "%s\n" "$ac_cv_with_libcfile" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno
 then :
   ac_cv_libcfile=no
 else $as_nop
   ac_cv_libcfile=check
-        if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect
+                if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   if test -d "$ac_cv_with_libcfile"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -41797,15 +41824,16 @@
 
 fi
 
         ac_cv_libcfile_LIBADD="-lcfile"
 fi
 
 fi
-    if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes
+
+    if test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcfile in directory: $ac_cv_with_libcfile
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -42119,15 +42147,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: unlink
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCFILE 1" >>confdefs.h
@@ -42197,15 +42225,15 @@
 printf "%s\n" "$ac_cv_with_libcpath" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno
 then :
   ac_cv_libcpath=no
 else $as_nop
   ac_cv_libcpath=check
-        if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect
+                if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   if test -d "$ac_cv_with_libcpath"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -43002,15 +43030,16 @@
 
 fi
 
         ac_cv_libcpath_LIBADD="-lcpath"
 fi
 
 fi
-    if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes
+
+    if test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcpath in directory: $ac_cv_with_libcpath
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -43200,15 +43229,15 @@
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: mkdir
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCPATH 1" >>confdefs.h
@@ -43278,15 +43307,15 @@
 printf "%s\n" "$ac_cv_with_libbfio" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno
 then :
   ac_cv_libbfio=no
 else $as_nop
   ac_cv_libbfio=check
-        if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect
+                if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   if test -d "$ac_cv_with_libbfio"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -45396,15 +45425,16 @@
 
 fi
 
         ac_cv_libbfio_LIBADD="-lbfio"
 fi
 
 fi
-    if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes
+
+    if test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libbfio in directory: $ac_cv_with_libbfio
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -45429,15 +45459,15 @@
 
 fi
 
 
     if test "x$ac_cv_libbfio" != xyes
 then :
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBBFIO 1" >>confdefs.h
@@ -45507,15 +45537,15 @@
 printf "%s\n" "$ac_cv_with_libfcache" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcache" = xno
 then :
   ac_cv_libfcache=no
 else $as_nop
   ac_cv_libfcache=check
-        if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect
+                if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes
 then :
   if test -d "$ac_cv_with_libfcache"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfcache}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfcache}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -46427,15 +46457,16 @@
 fi
 
 
         ac_cv_libfcache_LIBADD="-lfcache"
 fi
 
 fi
-    if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_libfcache" != xyes
+
+    if test "x$ac_cv_libfcache" != xyes && test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfcache in directory: $ac_cv_with_libfcache
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -46528,15 +46559,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: time
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libfcache_CPPFLAGS="-I../libfcache";
+  ac_cv_libfcache_CPPFLAGS="-I../libfcache -I\$(top_srcdir)/libfcache";
   ac_cv_libfcache_LIBADD="../libfcache/libfcache.la";
 
   ac_cv_libfcache=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFCACHE 1" >>confdefs.h
@@ -46606,15 +46637,15 @@
 printf "%s\n" "$ac_cv_with_libfdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdata" = xno
 then :
   ac_cv_libfdata=no
 else $as_nop
   ac_cv_libfdata=check
-        if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect
+                if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes
 then :
   if test -d "$ac_cv_with_libfdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -49894,15 +49925,16 @@
 
 
 
         ac_cv_libfdata_LIBADD="-lfdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_libfdata" != xyes
+
+    if test "x$ac_cv_libfdata" != xyes && test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfdata in directory: $ac_cv_with_libfdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -49927,15 +49959,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdata" != xyes
 then :
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATA 1" >>confdefs.h
@@ -50005,15 +50037,15 @@
 printf "%s\n" "$ac_cv_with_libfdatetime" >&6; }
 
   if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdatetime" = xno
 then :
   ac_cv_libfdatetime=no
 else $as_nop
   ac_cv_libfdatetime=check
-        if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect
+                if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes
 then :
   if test -d "$ac_cv_with_libfdatetime"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfdatetime}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdatetime}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -53449,15 +53481,16 @@
 fi
 
 
         ac_cv_libfdatetime_LIBADD="-lfdatetime"
 fi
 
 fi
-    if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_libfdatetime" != xyes
+
+    if test "x$ac_cv_libfdatetime" != xyes && test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfdatetime in directory: $ac_cv_with_libfdatetime
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -53482,15 +53515,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdatetime" != xyes
 then :
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATETIME 1" >>confdefs.h
@@ -53560,15 +53593,15 @@
 printf "%s\n" "$ac_cv_with_zlib" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_zlib" = xno
 then :
   ac_cv_zlib=no
 else $as_nop
   ac_cv_zlib=check
-        if test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect
+                if test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect && test "x$ac_cv_with_zlib" != xyes
 then :
   if test -d "$ac_cv_with_zlib"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_zlib}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_zlib}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -53735,14 +53768,23 @@
 
         ac_cv_zlib_LIBADD="-lz";
 
 fi
 
 fi
 
+    if test "x$ac_cv_zlib" != xyes && test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect && test "x$ac_cv_with_zlib" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported zlib in directory: $ac_cv_with_zlib
+See \`config.log' for more details" "$LINENO" 5; }
+
+fi
+
 fi
 
   if test "x$ac_cv_zlib" = xzlib
 then :
 
 printf "%s\n" "#define HAVE_ZLIB 1" >>confdefs.h
 
@@ -54379,16 +54421,20 @@
         PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for Python libraries" >&5
 printf %s "checking for Python libraries... " >&6; }
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $PYTHON_LDFLAGS" >&5
 printf "%s\n" "$PYTHON_LDFLAGS" >&6; }
 
-        case $host_os in #(
-  cygwin*) :
+        case $build in #(
+  *-*-cygwin*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-mingw*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-msys*) :
     PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
   *) :
      ;; #(
   *) :
      ;;
 esac
 
@@ -54546,33 +54592,107 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_libfuse=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_libfuse" >&5
 printf "%s\n" "$ac_cv_with_libfuse" >&6; }
 
-      if test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_with_libfuse" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfuse" = xno
+then :
+  ac_cv_libfuse=no
+else $as_nop
+              if test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes
 then :
   if test -d "$ac_cv_with_libfuse"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
-      LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"
 else $as_nop
-  { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_libfuse" >&5
-printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_libfuse" >&2;}
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "no such directory: $ac_cv_with_libfuse
+See \`config.log' for more details" "$LINENO" 5; }
 
 fi
+else $as_nop
+        if test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"
+then :
 
+pkg_failed=no
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse3 >= 3.0" >&5
+printf %s "checking for fuse3 >= 3.0... " >&6; }
+
+if test -n "$fuse3_CFLAGS"; then
+    pkg_cv_fuse3_CFLAGS="$fuse3_CFLAGS"
+ elif test -n "$PKG_CONFIG"; then
+    if test -n "$PKG_CONFIG" && \
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"fuse3 >= 3.0\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "fuse3 >= 3.0") 2>&5
+  ac_status=$?
+  printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
+  test $ac_status = 0; }; then
+  pkg_cv_fuse3_CFLAGS=`$PKG_CONFIG --cflags "fuse3 >= 3.0" 2>/dev/null`
+		      test "x$?" != "x0" && pkg_failed=yes
+else
+  pkg_failed=yes
+fi
+ else
+    pkg_failed=untried
+fi
+if test -n "$fuse3_LIBS"; then
+    pkg_cv_fuse3_LIBS="$fuse3_LIBS"
+ elif test -n "$PKG_CONFIG"; then
+    if test -n "$PKG_CONFIG" && \
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"fuse3 >= 3.0\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "fuse3 >= 3.0") 2>&5
+  ac_status=$?
+  printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
+  test $ac_status = 0; }; then
+  pkg_cv_fuse3_LIBS=`$PKG_CONFIG --libs "fuse3 >= 3.0" 2>/dev/null`
+		      test "x$?" != "x0" && pkg_failed=yes
+else
+  pkg_failed=yes
+fi
+ else
+    pkg_failed=untried
 fi
 
-  if test "x$ac_cv_with_libfuse" = xno
-then :
-  ac_cv_libfuse=no
-else $as_nop
-      if test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"
+
+
+if test $pkg_failed = yes; then
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
+printf "%s\n" "no" >&6; }
+
+if $PKG_CONFIG --atleast-pkgconfig-version 0.20; then
+        _pkg_short_errors_supported=yes
+else
+        _pkg_short_errors_supported=no
+fi
+        if test $_pkg_short_errors_supported = yes; then
+                fuse3_PKG_ERRORS=`$PKG_CONFIG --short-errors --print-errors --cflags --libs "fuse3 >= 3.0" 2>&1`
+        else
+                fuse3_PKG_ERRORS=`$PKG_CONFIG --print-errors --cflags --libs "fuse3 >= 3.0" 2>&1`
+        fi
+        # Put the nasty error message in config.log where it belongs
+        echo "$fuse3_PKG_ERRORS" >&5
+
+        ac_cv_libfuse=no
+elif test $pkg_failed = untried; then
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
+printf "%s\n" "no" >&6; }
+        ac_cv_libfuse=no
+else
+        fuse3_CFLAGS=$pkg_cv_fuse3_CFLAGS
+        fuse3_LIBS=$pkg_cv_fuse3_LIBS
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: yes" >&5
+printf "%s\n" "yes" >&6; }
+        ac_cv_libfuse=libfuse3
+fi
+
+        if test "x$ac_cv_libfuse" = xno
 then :
 
 pkg_failed=no
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse >= 2.6" >&5
 printf %s "checking for fuse >= 2.6... " >&6; }
 
 if test -n "$fuse_CFLAGS"; then
@@ -54640,51 +54760,110 @@
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: yes" >&5
 printf "%s\n" "yes" >&6; }
         ac_cv_libfuse=libfuse
 fi
 
 fi
 
-    if test "x$ac_cv_libfuse" = xlibfuse
+        if test "x$ac_cv_libfuse" = xlibfuse3
 then :
-  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS"
-      ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"
-else $as_nop
-               for ac_header in fuse.h
-do :
-  ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
+  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse3_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse3_LIBS"
+fi
+
+        if test "x$ac_cv_libfuse" = xlibfuse
+then :
+  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"
+fi
+
+fi
+
+fi
+
+    backup_CPPFLAGS="$CPPFLAGS"
+
+        if test "x$ac_cv_libfuse" != xlibfuse && test "x$ac_cv_libfuse" != xlibfuse3
+then :
+
+      CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=30"
+      ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_FUSE_H 1" >>confdefs.h
- ac_cv_header_fuse_h=yes
-else $as_nop
-  ac_cv_header_fuse_h=no
+
 fi
 
-done
 
-                  if test "x$ac_cv_header_fuse_h" = xno
+      if test "x$ac_cv_header_fuse_h" = xyes
 then :
-  { ac_cv_header_fuse_h=; unset ac_cv_header_fuse_h;}
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64 -DFUSE_USE_VERSION=26"
+  ac_cv_libfuse=libfuse3
+else $as_nop
+  CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
         ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_FUSE_H 1" >>confdefs.h
 
 fi
 
 
+        if test "x$ac_cv_header_fuse_h" = xyes
+then :
+  ac_cv_libfuse=libfuse
+fi
+
 fi
 
       if test "x$ac_cv_header_fuse_h" = xno
 then :
   ac_cv_libfuse=no
 else $as_nop
-          ac_cv_libfuse=libfuse
+          { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_invalidate in -lfuse" >&5
+printf %s "checking for fuse_invalidate in -lfuse... " >&6; }
+if test ${ac_cv_lib_fuse_fuse_invalidate+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-lfuse  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char fuse_invalidate ();
+int
+main (void)
+{
+return fuse_invalidate ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_fuse_fuse_invalidate=yes
+else $as_nop
+  ac_cv_lib_fuse_fuse_invalidate=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fuse_fuse_invalidate" >&5
+printf "%s\n" "$ac_cv_lib_fuse_fuse_invalidate" >&6; }
+if test "x$ac_cv_lib_fuse_fuse_invalidate" = xyes
+then :
+  ac_cv_libfuse=libfuse
+else $as_nop
+  ac_cv_libfuse=libfuse3
+fi
+
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_daemonize in -lfuse" >&5
 printf %s "checking for fuse_daemonize in -lfuse... " >&6; }
 if test ${ac_cv_lib_fuse_fuse_daemonize+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
@@ -54847,45 +55026,38 @@
 then :
   ac_cv_libfuse_dummy=yes
 else $as_nop
   ac_cv_libfuse=no
 fi
 
 
-        ac_cv_libfuse_LIBADD="-lfuse";
+                ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
 
+        if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ac_cv_libfuse_LIBADD="-lfuse3"
+else $as_nop
+  ac_cv_libfuse_LIBADD="-lfuse"
 fi
 
 fi
 
-        if test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno
-then :
-  CPPFLAGS="$CPPFLAGS -DFUSE_USE_VERSION=26"
-      ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
-if test "x$ac_cv_header_osxfuse_fuse_h" = xyes
-then :
-  printf "%s\n" "#define HAVE_OSXFUSE_FUSE_H 1" >>confdefs.h
-
 fi
 
-
-            if test "x$ac_cv_header_osxfuse_fuse_h" = xno
+        if test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno
 then :
-  { ac_cv_header_osxfuse_fuse_h=; unset ac_cv_header_osxfuse_fuse_h;}
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64"
-        ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
+  CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
+      ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_osxfuse_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_OSXFUSE_FUSE_H 1" >>confdefs.h
 
 fi
 
 
-fi
-
       if test "x$ac_cv_header_osxfuse_fuse_h" = xno
 then :
   ac_cv_libfuse=no
 else $as_nop
           ac_cv_libfuse=libosxfuse
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_daemonize in -losxfuse" >&5
@@ -55053,29 +55225,49 @@
 then :
   ac_cv_libfuse_dummy=yes
 else $as_nop
   ac_cv_libfuse=no
 fi
 
 
+                ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
         ac_cv_libfuse_LIBADD="-losxfuse";
 
 fi
 
 fi
 
+    if test "x$ac_cv_libfuse" != xyes && test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported libfuse in directory: $ac_cv_with_libfuse
+See \`config.log' for more details" "$LINENO" 5; }
+
+fi
+
+    CPPFLAGS="$backup_CPPFLAGS"
+
 fi
 
   if test "x$ac_cv_libfuse" = xlibfuse
 then :
 
 printf "%s\n" "#define HAVE_LIBFUSE 1" >>confdefs.h
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+
+printf "%s\n" "#define HAVE_LIBFUSE3 1" >>confdefs.h
+
+
+fi
   if test "x$ac_cv_libfuse" = xlibosxfuse
 then :
 
 printf "%s\n" "#define HAVE_LIBOSXFUSE 1" >>confdefs.h
 
 
 fi
@@ -55106,14 +55298,20 @@
 
   if test "x$ac_cv_libfuse" = xlibfuse
 then :
   ax_libfuse_pc_libs_private=-lfuse
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ax_libfuse_pc_libs_private=-lfuse3
+
+
+fi
   if test "x$ac_cv_libfuse" = xlibosxfuse
 then :
   ax_libfuse_pc_libs_private=-losxfuse
 
 
 fi
 
@@ -55121,14 +55319,22 @@
 then :
   ax_libfuse_spec_requires=fuse-libs
 
     ax_libfuse_spec_build_requires=fuse-devel
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ax_libfuse_spec_requires=fuse3-libs
+
+    ax_libfuse_spec_build_requires=fuse3-devel
+
+
+fi
 
 
 ac_fn_c_check_header_compile "$LINENO" "signal.h" "ac_cv_header_signal_h" "$ac_includes_default"
 if test "x$ac_cv_header_signal_h" = xyes
 then :
   printf "%s\n" "#define HAVE_SIGNAL_H 1" >>confdefs.h
 
@@ -56042,15 +56248,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libgzipf $as_me 20240103, which was
+This file was extended by libgzipf $as_me 20240422, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -56110,15 +56316,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libgzipf config.status 20240103
+libgzipf config.status 20240422
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libgzipf-20240103/libgzipf/libgzipf_huffman_tree.c` & `libgzipf-20240422/libgzipf/libgzipf_huffman_tree.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_notify.h` & `libgzipf-20240422/libgzipf/libgzipf_notify.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_libuna.h` & `libgzipf-20240422/libgzipf/libgzipf_libuna.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf.rc.in` & `libgzipf-20240422/libgzipf/libgzipf.rc.in`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_bit_stream.h` & `libgzipf-20240422/libgzipf/libgzipf_bit_stream.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_file.h` & `libgzipf-20240422/libgzipf/libgzipf_file.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_huffman_tree.h` & `libgzipf-20240422/libgzipf/libgzipf_huffman_tree.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_member_descriptor.c` & `libgzipf-20240422/libgzipf/libgzipf_member_descriptor.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_definitions.h.in` & `libgzipf-20240422/libgzipf/libgzipf_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_codepage.h` & `libgzipf-20240422/libgzipf/libgzipf_codepage.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_libcthreads.h` & `libgzipf-20240422/libgzipf/libgzipf_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_io_handle.c` & `libgzipf-20240422/libgzipf/libgzipf_io_handle.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_io_handle.h` & `libgzipf-20240422/libgzipf/libgzipf_io_handle.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_member.h` & `libgzipf-20240422/libgzipf/libgzipf_member.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_libfdata.h` & `libgzipf-20240422/libgzipf/libgzipf_libfdata.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_libfdatetime.h` & `libgzipf-20240422/libgzipf/libgzipf_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_segment_descriptor.h` & `libgzipf-20240422/libgzipf/libgzipf_segment_descriptor.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/Makefile.am` & `libgzipf-20240422/libgzipf/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -76,21 +76,19 @@
 libgzipf_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libgzipf_definitions.h.in \
 	libgzipf.rc \
 	libgzipf.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libgzipf_definitions.h \
+	libgzipf.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libgzipf_definitions.h
-	-rm -f libgzipf.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libgzipf ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libgzipf_la_SOURCES)
```

### Comparing `libgzipf-20240103/libgzipf/libgzipf.rc` & `libgzipf-20240422/libgzipf/libgzipf.rc`

 * *Files 16% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the GZIP file format\0"
-      VALUE "FileVersion",		"20240103" "\0"
+      VALUE "FileVersion",		"20240422" "\0"
       VALUE "InternalName",		"libgzipf.dll\0"
       VALUE "LegalCopyright",		"(C) 2019-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libgzipf.dll\0"
       VALUE "ProductName",		"libgzipf\0"
-      VALUE "ProductVersion",		"20240103" "\0"
+      VALUE "ProductVersion",		"20240422" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libgzipf/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libgzipf-20240103/libgzipf/libgzipf_error.c` & `libgzipf-20240422/libgzipf/libgzipf_error.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/gzipf_member_footer.h` & `libgzipf-20240422/libgzipf/gzipf_member_footer.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_file.c` & `libgzipf-20240422/libgzipf/libgzipf_file.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_member.c` & `libgzipf-20240422/libgzipf/libgzipf_member.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_unused.h` & `libgzipf-20240422/libgzipf/libgzipf_unused.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_debug.c` & `libgzipf-20240422/libgzipf/libgzipf_debug.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_member_descriptor.h` & `libgzipf-20240422/libgzipf/libgzipf_member_descriptor.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_extern.h` & `libgzipf-20240422/libgzipf/libgzipf_extern.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_compressed_segment.c` & `libgzipf-20240422/libgzipf/libgzipf_compressed_segment.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_libbfio.h` & `libgzipf-20240422/libgzipf/libgzipf_libbfio.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_member_footer.h` & `libgzipf-20240422/libgzipf/libgzipf_member_footer.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_types.h` & `libgzipf-20240422/libgzipf/libgzipf_types.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_checksum.h` & `libgzipf-20240422/libgzipf/libgzipf_checksum.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_debug.h` & `libgzipf-20240422/libgzipf/libgzipf_debug.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_support.h` & `libgzipf-20240422/libgzipf/libgzipf_support.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_error.h` & `libgzipf-20240422/libgzipf/libgzipf_error.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_libcnotify.h` & `libgzipf-20240422/libgzipf/libgzipf_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_libcdata.h` & `libgzipf-20240422/libgzipf/libgzipf_libcdata.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_bit_stream.c` & `libgzipf-20240422/libgzipf/libgzipf_bit_stream.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_compressed_segment.h` & `libgzipf-20240422/libgzipf/libgzipf_compressed_segment.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_member_header.c` & `libgzipf-20240422/libgzipf/libgzipf_member_header.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_libcerror.h` & `libgzipf-20240422/libgzipf/libgzipf_libcerror.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf.c` & `libgzipf-20240422/libgzipf/libgzipf.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_support.c` & `libgzipf-20240422/libgzipf/libgzipf_support.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_libclocale.h` & `libgzipf-20240422/libgzipf/libgzipf_libclocale.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_member_footer.c` & `libgzipf-20240422/libgzipf/libgzipf_member_footer.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_deflate.c` & `libgzipf-20240422/libgzipf/libgzipf_deflate.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_deflate.h` & `libgzipf-20240422/libgzipf/libgzipf_deflate.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/Makefile.in` & `libgzipf-20240422/libgzipf/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -491,14 +491,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -555,16 +557,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -634,15 +636,18 @@
 
 libgzipf_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libgzipf_definitions.h.in \
 	libgzipf.rc \
 	libgzipf.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libgzipf_definitions.h \
+	libgzipf.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -889,24 +894,43 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libLTLIBRARIES clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libgzipf.Plo
+	-rm -f ./$(DEPDIR)/libgzipf_bit_stream.Plo
+	-rm -f ./$(DEPDIR)/libgzipf_checksum.Plo
+	-rm -f ./$(DEPDIR)/libgzipf_compressed_segment.Plo
+	-rm -f ./$(DEPDIR)/libgzipf_debug.Plo
+	-rm -f ./$(DEPDIR)/libgzipf_deflate.Plo
+	-rm -f ./$(DEPDIR)/libgzipf_error.Plo
+	-rm -f ./$(DEPDIR)/libgzipf_file.Plo
+	-rm -f ./$(DEPDIR)/libgzipf_huffman_tree.Plo
+	-rm -f ./$(DEPDIR)/libgzipf_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libgzipf_member.Plo
+	-rm -f ./$(DEPDIR)/libgzipf_member_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libgzipf_member_footer.Plo
+	-rm -f ./$(DEPDIR)/libgzipf_member_header.Plo
+	-rm -f ./$(DEPDIR)/libgzipf_notify.Plo
+	-rm -f ./$(DEPDIR)/libgzipf_segment_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libgzipf_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1006,19 +1030,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libgzipf_definitions.h
-	-rm -f libgzipf.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libgzipf ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libgzipf_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libgzipf-20240103/libgzipf/libgzipf_definitions.h` & `libgzipf-20240422/libgzipf/libgzipf_definitions.h`

 * *Files 3% similar despite different names*

```diff
@@ -33,19 +33,19 @@
 #if !defined( HAVE_LOCAL_LIBGZIPF )
 #include <libgzipf/definitions.h>
 
 /* The definitions in <libgzipf/definitions.h> are copied here
  * for local use of libgzipf
  */
 #else
-#define LIBGZIPF_VERSION					20240103
+#define LIBGZIPF_VERSION					20240422
 
 /* The libgzipf version string
  */
-#define LIBGZIPF_VERSION_STRING					"20240103"
+#define LIBGZIPF_VERSION_STRING					"20240422"
 
 /* The libgzipf file access
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBGZIPF_ACCESS_FLAGS
```

### Comparing `libgzipf-20240103/libgzipf/gzipf_member_header.h` & `libgzipf-20240422/libgzipf/gzipf_member_header.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_checksum.c` & `libgzipf-20240422/libgzipf/libgzipf_checksum.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_member_header.h` & `libgzipf-20240422/libgzipf/libgzipf_member_header.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_notify.c` & `libgzipf-20240422/libgzipf/libgzipf_notify.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_libfcache.h` & `libgzipf-20240422/libgzipf/libgzipf_libfcache.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libgzipf/libgzipf_segment_descriptor.c` & `libgzipf-20240422/libgzipf/libgzipf_segment_descriptor.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/compile` & `libgzipf-20240422/compile`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/missing` & `libgzipf-20240422/missing`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/libfdata/libfdata.vcproj` & `libgzipf-20240422/msvscpp/libfdata/libfdata.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/gzipf_test_tools_output/gzipf_test_tools_output.vcproj` & `libgzipf-20240422/msvscpp/gzipf_test_tools_output/gzipf_test_tools_output.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/gzipf_test_checksum/gzipf_test_checksum.vcproj` & `libgzipf-20240422/msvscpp/gzipf_test_checksum/gzipf_test_checksum.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/gzipf_test_tools_signal/gzipf_test_tools_signal.vcproj` & `libgzipf-20240422/msvscpp/gzipf_test_tools_signal/gzipf_test_tools_signal.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/gzipf_test_deflate/gzipf_test_deflate.vcproj` & `libgzipf-20240422/msvscpp/gzipf_test_deflate/gzipf_test_deflate.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/zlib/zlib.vcproj` & `libgzipf-20240422/msvscpp/zlib/zlib.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/gzipf_test_tools_info_handle/gzipf_test_tools_info_handle.vcproj` & `libgzipf-20240422/msvscpp/gzipf_test_tools_info_handle/gzipf_test_tools_info_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/gzipf_test_huffman_tree/gzipf_test_huffman_tree.vcproj` & `libgzipf-20240422/msvscpp/gzipf_test_huffman_tree/gzipf_test_huffman_tree.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/libclocale/libclocale.vcproj` & `libgzipf-20240422/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/libfcache/libfcache.vcproj` & `libgzipf-20240422/msvscpp/libfcache/libfcache.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/Makefile.am` & `libgzipf-20240422/msvscpp/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -35,13 +35,11 @@
 	pygzipf/pygzipf.vcproj \
 	zlib/zlib.vcproj \
 	libgzipf.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libgzipf-20240103/msvscpp/gzipf_test_support/gzipf_test_support.vcproj` & `libgzipf-20240422/msvscpp/gzipf_test_support/gzipf_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/libbfio/libbfio.vcproj` & `libgzipf-20240422/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/gzipf_test_compressed_segment/gzipf_test_compressed_segment.vcproj` & `libgzipf-20240422/msvscpp/gzipf_test_compressed_segment/gzipf_test_compressed_segment.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/libgzipf/libgzipf.vcproj` & `libgzipf-20240422/msvscpp/libgzipf/libgzipf.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/gzipf_test_bit_stream/gzipf_test_bit_stream.vcproj` & `libgzipf-20240422/msvscpp/gzipf_test_bit_stream/gzipf_test_bit_stream.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/libcfile/libcfile.vcproj` & `libgzipf-20240422/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/gzipf_test_member_footer/gzipf_test_member_footer.vcproj` & `libgzipf-20240422/msvscpp/gzipf_test_member_footer/gzipf_test_member_footer.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/gzipf_test_io_handle/gzipf_test_io_handle.vcproj` & `libgzipf-20240422/msvscpp/gzipf_test_io_handle/gzipf_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/libcdata/libcdata.vcproj` & `libgzipf-20240422/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/gzipf_test_member/gzipf_test_member.vcproj` & `libgzipf-20240422/msvscpp/gzipf_test_member/gzipf_test_member.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/libcthreads/libcthreads.vcproj` & `libgzipf-20240422/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/gzipf_test_file/gzipf_test_file.vcproj` & `libgzipf-20240422/msvscpp/gzipf_test_file/gzipf_test_file.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/gzipf_test_member_header/gzipf_test_member_header.vcproj` & `libgzipf-20240422/msvscpp/gzipf_test_member_header/gzipf_test_member_header.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/libcpath/libcpath.vcproj` & `libgzipf-20240422/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/gzipfinfo/gzipfinfo.vcproj` & `libgzipf-20240422/msvscpp/gzipfinfo/gzipfinfo.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/gzipf_test_notify/gzipf_test_notify.vcproj` & `libgzipf-20240422/msvscpp/gzipf_test_notify/gzipf_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/libcsplit/libcsplit.vcproj` & `libgzipf-20240422/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/pygzipf/pygzipf.vcproj` & `libgzipf-20240422/msvscpp/pygzipf/pygzipf.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/gzipf_test_member_descriptor/gzipf_test_member_descriptor.vcproj` & `libgzipf-20240422/msvscpp/gzipf_test_member_descriptor/gzipf_test_member_descriptor.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/libuna/libuna.vcproj` & `libgzipf-20240422/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/Makefile.in` & `libgzipf-20240422/msvscpp/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -389,14 +389,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -493,15 +495,16 @@
 	pygzipf/pygzipf.vcproj \
 	zlib/zlib.vcproj \
 	libgzipf.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -605,23 +608,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -700,13 +705,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libgzipf-20240103/msvscpp/libcnotify/libcnotify.vcproj` & `libgzipf-20240422/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/libcerror/libcerror.vcproj` & `libgzipf-20240422/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/libgzipf.sln` & `libgzipf-20240422/msvscpp/libgzipf.sln`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/gzipfmount/gzipfmount.vcproj` & `libgzipf-20240422/msvscpp/gzipfmount/gzipfmount.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/libfdatetime/libfdatetime.vcproj` & `libgzipf-20240422/msvscpp/libfdatetime/libfdatetime.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/msvscpp/gzipf_test_error/gzipf_test_error.vcproj` & `libgzipf-20240422/msvscpp/gzipf_test_error/gzipf_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcfile/libcfile_extern.h` & `libgzipf-20240422/libcfile/libcfile_extern.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2008-2021, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcfile/libcfile_support.h` & `libgzipf-20240422/libcfile/libcfile_support.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2021, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcfile/libcfile_unused.h` & `libgzipf-20240422/libcfile/libcfile_unused.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2008-2021, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcfile/libcfile_notify.h` & `libgzipf-20240422/libcfile/libcfile_notify.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Notification functions
  *
- * Copyright (C) 2008-2021, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcfile/libcfile_support.c` & `libgzipf-20240422/libcfile/libcfile_support.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2021, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcfile/libcfile_types.h` & `libgzipf-20240422/libcfile/libcfile_types.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2008-2021, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcfile/Makefile.am` & `libgzipf-20240422/libcfile/Makefile.am`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCFILE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcfile.la
 
@@ -22,17 +22,17 @@
 	libcfile_support.c libcfile_support.h \
 	libcfile_system_string.c libcfile_system_string.h \
 	libcfile_types.h \
 	libcfile_unused.h \
 	libcfile_winapi.c libcfile_winapi.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
```

### Comparing `libgzipf-20240103/libcfile/libcfile_notify.c` & `libgzipf-20240422/libcfile/libcfile_notify.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Notification functions
  *
- * Copyright (C) 2008-2021, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcfile/libcfile_system_string.h` & `libgzipf-20240422/libcfile/libcfile_system_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2008-2021, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcfile/libcfile_file.h` & `libgzipf-20240422/libcfile/libcfile_file.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2008-2021, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcfile/libcfile_libcnotify.h` & `libgzipf-20240422/libcfile/libcfile_libcnotify.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcnotify header wrapper
  *
- * Copyright (C) 2008-2021, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcfile/libcfile_system_string.c` & `libgzipf-20240422/libcfile/libcfile_system_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2008-2021, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcfile/libcfile_error.h` & `libgzipf-20240422/libcfile/libcfile_error.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2008-2021, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcfile/libcfile_libcerror.h` & `libgzipf-20240422/libcfile/libcfile_libcerror.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2008-2021, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcfile/libcfile_file.c` & `libgzipf-20240422/libcfile/libcfile_file.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2008-2021, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcfile/libcfile_libclocale.h` & `libgzipf-20240422/libcfile/libcfile_libclocale.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libclocale header wrapper
  *
- * Copyright (C) 2008-2021, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcfile/libcfile_winapi.h` & `libgzipf-20240422/libcfile/libcfile_winapi.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * WINAPI fallback functions
  *
- * Copyright (C) 2008-2021, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcfile/Makefile.in` & `libgzipf-20240422/libcfile/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -454,14 +454,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -518,16 +520,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBCFILE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCFILE_TRUE@noinst_LTLIBRARIES = libcfile.la
 @HAVE_LOCAL_LIBCFILE_TRUE@libcfile_la_SOURCES = \
@@ -542,15 +544,16 @@
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_notify.c libcfile_notify.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_support.c libcfile_support.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_system_string.c libcfile_system_string.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_types.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_unused.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_winapi.c libcfile_winapi.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -755,24 +758,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcfile_error.Plo
+	-rm -f ./$(DEPDIR)/libcfile_file.Plo
+	-rm -f ./$(DEPDIR)/libcfile_notify.Plo
+	-rm -f ./$(DEPDIR)/libcfile_support.Plo
+	-rm -f ./$(DEPDIR)/libcfile_system_string.Plo
+	-rm -f ./$(DEPDIR)/libcfile_winapi.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -835,14 +846,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -853,23 +866,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libgzipf-20240103/libcfile/libcfile_error.c` & `libgzipf-20240422/libcfile/libcfile_error.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2008-2021, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcfile/libcfile_libuna.h` & `libgzipf-20240422/libcfile/libcfile_libuna.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libuna header wrapper
  *
- * Copyright (C) 2008-2021, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcfile/libcfile_winapi.c` & `libgzipf-20240422/libcfile/libcfile_winapi.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * WINAPI fallback functions
  *
- * Copyright (C) 2008-2021, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcfile/libcfile_definitions.h` & `libgzipf-20240422/libcfile/libcfile_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2008-2021, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -31,19 +31,19 @@
 #include <libcfile/definitions.h>
 
 /* The definitions in <libcfile/definitions.h> are copied here
  * for local use of libcfile
  */
 #else
 
-#define LIBCFILE_VERSION				20210616
+#define LIBCFILE_VERSION				20240414
 
 /* The libcfile version string
  */
-#define LIBCFILE_VERSION_STRING				"20210616"
+#define LIBCFILE_VERSION_STRING				"20240414"
 
 /* The file access flags
  * bit 1	set to 1 for read access
  * bit 2	set to 1 for write access
  * bit 3	set to 1 to truncate an existing file on write
  * bit 4-8	not used
  */
```

### Comparing `libgzipf-20240103/INSTALL` & `libgzipf-20240422/INSTALL`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/libcdata_list_element.h` & `libgzipf-20240422/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/libcdata_array.h` & `libgzipf-20240422/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/libcdata_definitions.h` & `libgzipf-20240422/libcdata/libcdata_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcdata/definitions.h>
 
 /* The definitions in <libcdata/definitions.h> are copied here
  * for local use of libcdata
  */
 #else
 
-#define LIBCDATA_VERSION				20240103
+#define LIBCDATA_VERSION				20240414
 
 /* The libcdata version string
  */
-#define LIBCDATA_VERSION_STRING				"20240103"
+#define LIBCDATA_VERSION_STRING				"20240414"
 
 /* The comparison function definitions
  */
 enum LIBCDATA_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libgzipf-20240103/libcdata/libcdata_libcerror.h` & `libgzipf-20240422/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/libcdata_unused.h` & `libgzipf-20240422/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/libcdata_btree.h` & `libgzipf-20240422/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/libcdata_btree.c` & `libgzipf-20240422/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/libcdata_support.c` & `libgzipf-20240422/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/libcdata_list.c` & `libgzipf-20240422/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/libcdata_extern.h` & `libgzipf-20240422/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/libcdata_list.h` & `libgzipf-20240422/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/libcdata_btree_values_list.h` & `libgzipf-20240422/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/Makefile.am` & `libgzipf-20240422/libcdata/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcdata.la
 
 libcdata_la_SOURCES = \
@@ -24,19 +24,17 @@
 	libcdata_range_list_value.c libcdata_range_list_value.h \
 	libcdata_support.c libcdata_support.h \
 	libcdata_tree_node.c libcdata_tree_node.h \
 	libcdata_types.h \
 	libcdata_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
```

### Comparing `libgzipf-20240103/libcdata/libcdata_btree_node.h` & `libgzipf-20240422/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/libcdata_range_list_value.h` & `libgzipf-20240422/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/libcdata_range_list.h` & `libgzipf-20240422/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/libcdata_range_list.c` & `libgzipf-20240422/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/libcdata_array.c` & `libgzipf-20240422/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/libcdata_list_element.c` & `libgzipf-20240422/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/libcdata_libcthreads.h` & `libgzipf-20240422/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/libcdata_tree_node.h` & `libgzipf-20240422/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/libcdata_error.h` & `libgzipf-20240422/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/libcdata_types.h` & `libgzipf-20240422/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/libcdata_btree_node.c` & `libgzipf-20240422/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/libcdata_tree_node.c` & `libgzipf-20240422/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/libcdata_support.h` & `libgzipf-20240422/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/Makefile.in` & `libgzipf-20240422/libcdata/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -468,14 +468,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -532,16 +534,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBCDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCDATA_TRUE@noinst_LTLIBRARIES = libcdata.la
 @HAVE_LOCAL_LIBCDATA_TRUE@libcdata_la_SOURCES = \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_array.c libcdata_array.h \
@@ -558,15 +560,16 @@
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list.c libcdata_range_list.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list_value.c libcdata_range_list_value.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_support.c libcdata_support.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_tree_node.c libcdata_tree_node.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_types.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -776,24 +779,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcdata_array.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_node.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_values_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_error.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list_value.Plo
+	-rm -f ./$(DEPDIR)/libcdata_support.Plo
+	-rm -f ./$(DEPDIR)/libcdata_tree_node.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -887,17 +903,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libgzipf-20240103/libcdata/libcdata_range_list_value.c` & `libgzipf-20240422/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/libcdata_btree_values_list.c` & `libgzipf-20240422/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcdata/libcdata_error.c` & `libgzipf-20240422/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/config.sub` & `libgzipf-20240422/config.sub`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/setup.py` & `libgzipf-20240422/setup.py`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/acinclude.m4` & `libgzipf-20240422/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/config.rpath` & `libgzipf-20240422/config.rpath`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcthreads/libcthreads_thread.h` & `libgzipf-20240422/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcthreads/libcthreads_read_write_lock.h` & `libgzipf-20240422/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcthreads/libcthreads_thread.c` & `libgzipf-20240422/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcthreads/libcthreads_thread_pool.h` & `libgzipf-20240422/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcthreads/libcthreads_support.h` & `libgzipf-20240422/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcthreads/libcthreads_lock.h` & `libgzipf-20240422/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcthreads/libcthreads_unused.h` & `libgzipf-20240422/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcthreads/libcthreads_lock.c` & `libgzipf-20240422/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcthreads/libcthreads_condition.h` & `libgzipf-20240422/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcthreads/libcthreads_repeating_thread.h` & `libgzipf-20240422/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcthreads/Makefile.am` & `libgzipf-20240422/libcthreads/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCTHREADS
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcthreads.la
 
 libcthreads_la_SOURCES = \
 	libcthreads_condition.c libcthreads_condition.h \
@@ -22,19 +22,17 @@
 	libcthreads_thread.c libcthreads_thread.h \
 	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 	libcthreads_types.h \
 	libcthreads_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
```

### Comparing `libgzipf-20240103/libcthreads/libcthreads_support.c` & `libgzipf-20240422/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcthreads/libcthreads_mutex.c` & `libgzipf-20240422/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcthreads/libcthreads_queue.c` & `libgzipf-20240422/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcthreads/libcthreads_mutex.h` & `libgzipf-20240422/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcthreads/libcthreads_types.h` & `libgzipf-20240422/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcthreads/libcthreads_thread_attributes.h` & `libgzipf-20240422/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcthreads/libcthreads_condition.c` & `libgzipf-20240422/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcthreads/libcthreads_error.c` & `libgzipf-20240422/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcthreads/libcthreads_read_write_lock.c` & `libgzipf-20240422/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcthreads/libcthreads_libcerror.h` & `libgzipf-20240422/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcthreads/libcthreads_definitions.h` & `libgzipf-20240422/libcthreads/libcthreads_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcthreads/definitions.h>
 
 /* The definitions in <libcthreads/definitions.h> are copied here
  * for local use of libcthreads
  */
 #else
 
-#define LIBCTHREADS_VERSION				20240102
+#define LIBCTHREADS_VERSION				20240413
 
 /* The libcthreads version string
  */
-#define LIBCTHREADS_VERSION_STRING			"20240102"
+#define LIBCTHREADS_VERSION_STRING			"20240413"
 
 /* The comparison function definitions
  */
 enum LIBCTHREADS_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libgzipf-20240103/libcthreads/libcthreads_thread_pool.c` & `libgzipf-20240422/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcthreads/libcthreads_error.h` & `libgzipf-20240422/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcthreads/libcthreads_thread_attributes.c` & `libgzipf-20240422/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcthreads/libcthreads_extern.h` & `libgzipf-20240422/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcthreads/libcthreads_repeating_thread.c` & `libgzipf-20240422/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcthreads/Makefile.in` & `libgzipf-20240422/libcthreads/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -472,14 +472,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -536,16 +538,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCTHREADS_TRUE@noinst_LTLIBRARIES = libcthreads.la
 @HAVE_LOCAL_LIBCTHREADS_TRUE@libcthreads_la_SOURCES = \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_condition.c libcthreads_condition.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_definitions.h \
@@ -560,15 +562,16 @@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_support.c libcthreads_support.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread.c libcthreads_thread.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_types.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -778,24 +781,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcthreads_condition.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_error.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_mutex.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_queue.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_read_write_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_repeating_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_support.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_attributes.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_pool.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -889,17 +905,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libgzipf-20240103/libcthreads/libcthreads_queue.h` & `libgzipf-20240422/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/test-driver` & `libgzipf-20240422/test-driver`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcpath/libcpath_support.c` & `libgzipf-20240422/libcpath/libcpath_support.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcpath/libcpath_libcerror.h` & `libgzipf-20240422/libcpath/libcpath_libcerror.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcpath/libcpath_definitions.h` & `libgzipf-20240422/libcpath/libcpath_definitions.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -31,19 +31,19 @@
 #include <libcpath/definitions.h>
 
 /* The definitions in <libcpath/definitions.h> are copied here
  * for local use of libcpath
  */
 #else
 
-#define LIBCPATH_VERSION			20220108
+#define LIBCPATH_VERSION			20240414
 
 /* The libcpath version string
  */
-#define LIBCPATH_VERSION_STRING			"20220108"
+#define LIBCPATH_VERSION_STRING			"20240414"
 
 #if defined( WINAPI )
 #define LIBCPATH_SEPARATOR			'\\'
 
 #else
 #define LIBCPATH_SEPARATOR			'/'
```

### Comparing `libgzipf-20240103/libcpath/Makefile.am` & `libgzipf-20240422/libcpath/Makefile.am`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCPATH
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcpath.la
 
@@ -19,17 +19,17 @@
 	libcpath_libcsplit.h \
 	libcpath_libuna.h \
 	libcpath_support.c libcpath_support.h \
 	libcpath_system_string.c libcpath_system_string.h \
 	libcpath_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
```

### Comparing `libgzipf-20240103/libcpath/libcpath_error.c` & `libgzipf-20240422/libcpath/libcpath_error.c`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcpath/libcpath_extern.h` & `libgzipf-20240422/libcpath/libcpath_extern.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcpath/libcpath_system_string.h` & `libgzipf-20240422/libcpath/libcpath_system_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcpath/libcpath_support.h` & `libgzipf-20240422/libcpath/libcpath_support.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcpath/libcpath_libcsplit.h` & `libgzipf-20240422/libcpath/libcpath_libcsplit.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcsplit header
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcpath/libcpath_system_string.c` & `libgzipf-20240422/libcpath/libcpath_system_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcpath/libcpath_libclocale.h` & `libgzipf-20240422/libcpath/libcpath_libclocale.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libclocale header wrapper
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcpath/libcpath_error.h` & `libgzipf-20240422/libcpath/libcpath_error.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcpath/Makefile.in` & `libgzipf-20240422/libcpath/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -448,14 +448,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -512,16 +514,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBCPATH_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCPATH_TRUE@noinst_LTLIBRARIES = libcpath.la
 @HAVE_LOCAL_LIBCPATH_TRUE@libcpath_la_SOURCES = \
@@ -533,15 +535,16 @@
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libclocale.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libcsplit.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libuna.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_support.c libcpath_support.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_system_string.c libcpath_system_string.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -744,24 +747,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcpath_error.Plo
+	-rm -f ./$(DEPDIR)/libcpath_path.Plo
+	-rm -f ./$(DEPDIR)/libcpath_support.Plo
+	-rm -f ./$(DEPDIR)/libcpath_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -822,14 +831,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -840,23 +851,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libgzipf-20240103/libcpath/libcpath_libuna.h` & `libgzipf-20240422/libcpath/libcpath_libuna.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libuna header wrapper
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcpath/libcpath_unused.h` & `libgzipf-20240422/libcpath/libcpath_unused.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcpath/libcpath_path.c` & `libgzipf-20240422/libcpath/libcpath_path.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Path functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcpath/libcpath_path.h` & `libgzipf-20240422/libcpath/libcpath_path.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Path functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/manuals/gzipfinfo.1` & `libgzipf-20240422/manuals/gzipfinfo.1`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/manuals/Makefile.in` & `libgzipf-20240422/manuals/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -421,14 +421,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -492,15 +494,16 @@
 	gzipfinfo.1 \
 	libgzipf.3
 
 EXTRA_DIST = \
 	gzipfinfo.1 \
 	libgzipf.3
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -693,23 +696,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -791,13 +796,10 @@
 	mostlyclean-libtool pdf pdf-am ps ps-am sources-am \
 	sources-local splint-am splint-local tags-am uninstall \
 	uninstall-am uninstall-man uninstall-man1 uninstall-man3
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libgzipf-20240103/manuals/libgzipf.3` & `libgzipf-20240422/manuals/libgzipf.3`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_member_descriptor.c` & `libgzipf-20240422/tests/gzipf_test_member_descriptor.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_checksum.c` & `libgzipf-20240422/tests/gzipf_test_checksum.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_file.c` & `libgzipf-20240422/tests/gzipf_test_file.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_libuna.h` & `libgzipf-20240422/tests/gzipf_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_deflate.c` & `libgzipf-20240422/tests/gzipf_test_deflate.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_member_footer.c` & `libgzipf-20240422/tests/gzipf_test_member_footer.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_functions.h` & `libgzipf-20240422/tests/gzipf_test_functions.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_io_handle.c` & `libgzipf-20240422/tests/gzipf_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_libgzipf.h` & `libgzipf-20240422/tests/gzipf_test_libgzipf.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/test_tools.sh` & `libgzipf-20240422/tests/test_library.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env bash
-# Tests tools functions and types.
+# Tests library functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
-TOOLS_TESTS="info_handle output signal";
-TOOLS_TESTS_WITH_INPUT="";
+LIBRARY_TESTS="bit_stream checksum compressed_segment deflate error huffman_tree io_handle member member_descriptor member_footer member_header notify";
+LIBRARY_TESTS_WITH_INPUT="file support";
 OPTION_SETS=();
 
 INPUT_GLOB="*";
 
 run_test()
 {
 	local TEST_NAME=$1;
 
 	local TEST_DESCRIPTION="Testing: ${TEST_NAME}";
-	local TEST_EXECUTABLE="./gzipf_test_tools_${TEST_NAME}";
+	local TEST_EXECUTABLE="./gzipf_test_${TEST_NAME}";
 
 	if ! test -x "${TEST_EXECUTABLE}";
 	then
 		TEST_EXECUTABLE="${TEST_EXECUTABLE}.exe";
 	fi
 
 	# TODO: add support for TEST_PROFILE and OPTION_SETS?
@@ -33,15 +33,15 @@
 }
 
 run_test_with_input()
 {
 	local TEST_NAME=$1;
 
 	local TEST_DESCRIPTION="Testing: ${TEST_NAME}";
-	local TEST_EXECUTABLE="./gzipf_test_tools_${TEST_NAME}";
+	local TEST_EXECUTABLE="./gzipf_test_${TEST_NAME}";
 
 	if ! test -x "${TEST_EXECUTABLE}";
 	then
 		TEST_EXECUTABLE="${TEST_EXECUTABLE}.exe";
 	fi
 
 	if ! test -d "input";
@@ -55,15 +55,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "gzipftools");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "libgzipf");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -132,38 +132,35 @@
 			break;
 		fi
 	done
 
 	return ${RESULT};
 }
 
-if test -n "${SKIP_TOOLS_TESTS}";
+if test -n "${SKIP_LIBRARY_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
 RESULT=${EXIT_IGNORE};
 
-for TEST_NAME in ${TOOLS_TESTS};
+for TEST_NAME in ${LIBRARY_TESTS};
 do
 	run_test "${TEST_NAME}";
 	RESULT=$?;
 
 	if test ${RESULT} -ne ${EXIT_SUCCESS};
 	then
 		break;
@@ -171,15 +168,15 @@
 done
 
 if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 then
 	exit ${RESULT};
 fi
 
-for TEST_NAME in ${TOOLS_TESTS_WITH_INPUT};
+for TEST_NAME in ${LIBRARY_TESTS_WITH_INPUT};
 do
 	if test -d "input";
 	then
 		run_test_with_input "${TEST_NAME}";
 		RESULT=$?;
 	else
 		run_test "${TEST_NAME}";
```

### Comparing `libgzipf-20240103/tests/gzipf_test_error.c` & `libgzipf-20240422/tests/gzipf_test_error.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_unused.h` & `libgzipf-20240422/tests/gzipf_test_unused.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_bit_stream.c` & `libgzipf-20240422/tests/gzipf_test_bit_stream.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_tools_signal.c` & `libgzipf-20240422/tests/gzipf_test_tools_signal.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_member_header.c` & `libgzipf-20240422/tests/gzipf_test_member_header.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_getopt.c` & `libgzipf-20240422/tests/gzipf_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_tools_output.c` & `libgzipf-20240422/tests/gzipf_test_tools_output.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_memory.c` & `libgzipf-20240422/tests/gzipf_test_memory.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/test_gzipfinfo.sh` & `libgzipf-20240422/tests/test_gzipfinfo.sh`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Info tool testing script
 #
-# Version: 20231005
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 PROFILES=("gzipfinfo");
 OPTIONS_PER_PROFILE=("");
@@ -28,20 +28,17 @@
 if ! test -x "${TEST_EXECUTABLE}";
 then
 	echo "Missing test executable: ${TEST_EXECUTABLE}";
 
 	exit ${EXIT_FAILURE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libgzipf-20240103/tests/Makefile.am` & `libgzipf-20240422/tests/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AUTOMAKE_OPTIONS = subdir-objects
 
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -308,13 +308,12 @@
 	gzipf_test_tools_signal.c \
 	gzipf_test_unused.h
 
 gzipf_test_tools_signal_LDADD = \
 	../libgzipf/libgzipf.la \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
-
-distclean: clean
-	-rm -f Makefile
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
```

### Comparing `libgzipf-20240103/tests/gzipf_test_notify.c` & `libgzipf-20240422/tests/gzipf_test_notify.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/pygzipf_test_file.py` & `libgzipf-20240422/tests/pygzipf_test_file.py`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/pygzipf_test_support.py` & `libgzipf-20240422/tests/pygzipf_test_support.py`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/test_python_module.sh` & `libgzipf-20240422/tests/test_python_module.sh`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 #!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20231005
+# Version: 20240417
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
+EXIT_NO_TESTS_RAN=5;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="support";
 TEST_FUNCTIONS_WITH_INPUT="file member";
 OPTION_SETS=();
 
 TEST_TOOL_DIRECTORY=".";
 INPUT_GLOB="*";
 
+LIBRARY_NAME="libgzipf";
+PYTHON_MODULE="pygzipf";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pygzipf_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pygzipf_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	if ! test -d "input";
 	then
 		echo "Test input directory not found.";
 
 		return ${EXIT_IGNORE};
 	fi
@@ -45,15 +49,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pygzipf");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "${PYTHON_MODULE}");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -120,38 +124,47 @@
 }
 
 if test -n "${SKIP_PYTHON_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
+PLATFORM=`uname -s | sed 's/-.*$//'`;
+
+if test "${PLATFORM}" = "MINGW64_NT" || test "${PLATFORM}" = "MSYS_NT";
+then
+	cp ../${LIBRARY_NAME}/.libs/*.dll ../${PYTHON_MODULE}/.libs/;
+	cp ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.dll ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.pyd;
+fi
+
 RESULT=${EXIT_IGNORE};
 
 for TEST_FUNCTION in ${TEST_FUNCTIONS};
 do
 	test_python_function "${TEST_FUNCTION}";
 	RESULT=$?;
 
-	if test ${RESULT} -ne ${EXIT_SUCCESS};
+	if test ${RESULT} -eq ${EXIT_NO_TESTS_RAN};
+	then
+		RESULT=${EXIT_IGNORE};
+	fi
+	if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 	then
 		break;
 	fi
 done
 
 if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 then
@@ -164,16 +177,19 @@
 	then
 		test_python_function_with_input "${TEST_FUNCTION}";
 		RESULT=$?;
 	else
 		test_python_function "${TEST_FUNCTION}";
 		RESULT=$?;
 	fi
-
-	if test ${RESULT} -ne ${EXIT_SUCCESS};
+	if test ${RESULT} -eq ${EXIT_NO_TESTS_RAN};
+	then
+		RESULT=${EXIT_IGNORE};
+	fi
+	if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 	then
 		break;
 	fi
 done
 
 exit ${RESULT};
```

### Comparing `libgzipf-20240103/tests/gzipf_test_macros.h` & `libgzipf-20240422/tests/gzipf_test_macros.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_member.c` & `libgzipf-20240422/tests/gzipf_test_member.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_support.c` & `libgzipf-20240422/tests/gzipf_test_support.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_libcnotify.h` & `libgzipf-20240422/tests/gzipf_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/test_runner.sh` & `libgzipf-20240422/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_libclocale.h` & `libgzipf-20240422/tests/gzipf_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_libcerror.h` & `libgzipf-20240422/tests/gzipf_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_tools_info_handle.c` & `libgzipf-20240422/tests/gzipf_test_tools_info_handle.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_libbfio.h` & `libgzipf-20240422/tests/gzipf_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_compressed_segment.c` & `libgzipf-20240422/tests/gzipf_test_compressed_segment.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/Makefile.in` & `libgzipf-20240422/tests/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -778,14 +778,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -843,16 +845,16 @@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 AUTOMAKE_OPTIONS = subdir-objects
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -1133,16 +1135,18 @@
 	gzipf_test_tools_signal.c \
 	gzipf_test_unused.h
 
 gzipf_test_tools_signal_LDADD = \
 	../libgzipf/libgzipf.la \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .log .o .obj .test .test$(EXEEXT) .trs
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -1635,24 +1639,49 @@
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
 	-rm -f ../gzipftools/$(DEPDIR)/$(am__dirstamp)
 	-rm -f ../gzipftools/$(am__dirstamp)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ../gzipftools/$(DEPDIR)/gzipftools_output.Po
+	-rm -f ../gzipftools/$(DEPDIR)/gzipftools_signal.Po
+	-rm -f ../gzipftools/$(DEPDIR)/info_handle.Po
+	-rm -f ./$(DEPDIR)/gzipf_test_bit_stream.Po
+	-rm -f ./$(DEPDIR)/gzipf_test_checksum.Po
+	-rm -f ./$(DEPDIR)/gzipf_test_compressed_segment.Po
+	-rm -f ./$(DEPDIR)/gzipf_test_deflate.Po
+	-rm -f ./$(DEPDIR)/gzipf_test_error.Po
+	-rm -f ./$(DEPDIR)/gzipf_test_file.Po
+	-rm -f ./$(DEPDIR)/gzipf_test_functions.Po
+	-rm -f ./$(DEPDIR)/gzipf_test_getopt.Po
+	-rm -f ./$(DEPDIR)/gzipf_test_huffman_tree.Po
+	-rm -f ./$(DEPDIR)/gzipf_test_io_handle.Po
+	-rm -f ./$(DEPDIR)/gzipf_test_member.Po
+	-rm -f ./$(DEPDIR)/gzipf_test_member_descriptor.Po
+	-rm -f ./$(DEPDIR)/gzipf_test_member_footer.Po
+	-rm -f ./$(DEPDIR)/gzipf_test_member_header.Po
+	-rm -f ./$(DEPDIR)/gzipf_test_memory.Po
+	-rm -f ./$(DEPDIR)/gzipf_test_notify.Po
+	-rm -f ./$(DEPDIR)/gzipf_test_support.Po
+	-rm -f ./$(DEPDIR)/gzipf_test_tools_info_handle.Po
+	-rm -f ./$(DEPDIR)/gzipf_test_tools_output.Po
+	-rm -f ./$(DEPDIR)/gzipf_test_tools_signal.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1758,13 +1787,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	recheck sources-am sources-local splint-am splint-local tags \
 	tags-am uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libgzipf-20240103/tests/gzipf_test_getopt.h` & `libgzipf-20240422/tests/gzipf_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_functions.c` & `libgzipf-20240422/tests/gzipf_test_functions.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_huffman_tree.c` & `libgzipf-20240422/tests/gzipf_test_huffman_tree.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/gzipf_test_memory.h` & `libgzipf-20240422/tests/gzipf_test_memory.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/tests/test_library.sh` & `libgzipf-20240422/tests/test_tools.sh`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env bash
-# Tests library functions and types.
+# Tests tools functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
-LIBRARY_TESTS="bit_stream checksum compressed_segment deflate error huffman_tree io_handle member member_descriptor member_footer member_header notify";
-LIBRARY_TESTS_WITH_INPUT="file support";
+TOOLS_TESTS="info_handle output signal";
+TOOLS_TESTS_WITH_INPUT="";
 OPTION_SETS=();
 
 INPUT_GLOB="*";
 
 run_test()
 {
 	local TEST_NAME=$1;
 
 	local TEST_DESCRIPTION="Testing: ${TEST_NAME}";
-	local TEST_EXECUTABLE="./gzipf_test_${TEST_NAME}";
+	local TEST_EXECUTABLE="./gzipf_test_tools_${TEST_NAME}";
 
 	if ! test -x "${TEST_EXECUTABLE}";
 	then
 		TEST_EXECUTABLE="${TEST_EXECUTABLE}.exe";
 	fi
 
 	# TODO: add support for TEST_PROFILE and OPTION_SETS?
@@ -33,15 +33,15 @@
 }
 
 run_test_with_input()
 {
 	local TEST_NAME=$1;
 
 	local TEST_DESCRIPTION="Testing: ${TEST_NAME}";
-	local TEST_EXECUTABLE="./gzipf_test_${TEST_NAME}";
+	local TEST_EXECUTABLE="./gzipf_test_tools_${TEST_NAME}";
 
 	if ! test -x "${TEST_EXECUTABLE}";
 	then
 		TEST_EXECUTABLE="${TEST_EXECUTABLE}.exe";
 	fi
 
 	if ! test -d "input";
@@ -55,15 +55,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "libgzipf");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "gzipftools");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -132,38 +132,35 @@
 			break;
 		fi
 	done
 
 	return ${RESULT};
 }
 
-if test -n "${SKIP_LIBRARY_TESTS}";
+if test -n "${SKIP_TOOLS_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
 RESULT=${EXIT_IGNORE};
 
-for TEST_NAME in ${LIBRARY_TESTS};
+for TEST_NAME in ${TOOLS_TESTS};
 do
 	run_test "${TEST_NAME}";
 	RESULT=$?;
 
 	if test ${RESULT} -ne ${EXIT_SUCCESS};
 	then
 		break;
@@ -171,15 +168,15 @@
 done
 
 if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 then
 	exit ${RESULT};
 fi
 
-for TEST_NAME in ${LIBRARY_TESTS_WITH_INPUT};
+for TEST_NAME in ${TOOLS_TESTS_WITH_INPUT};
 do
 	if test -d "input";
 	then
 		run_test_with_input "${TEST_NAME}";
 		RESULT=$?;
 	else
 		run_test "${TEST_NAME}";
```

### Comparing `libgzipf-20240103/ossfuzz/Makefile.am` & `libgzipf-20240422/ossfuzz/Makefile.am`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LIB_FUZZING_ENGINE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -29,17 +29,15 @@
 	../libgzipf/libgzipf.la \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on file_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(file_fuzzer_SOURCES)
```

### Comparing `libgzipf-20240103/ossfuzz/ossfuzz_libgzipf.h` & `libgzipf-20240422/ossfuzz/ossfuzz_libgzipf.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/ossfuzz/ossfuzz_libbfio.h` & `libgzipf-20240422/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/ossfuzz/file_fuzzer.cc` & `libgzipf-20240422/ossfuzz/file_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/ossfuzz/Makefile.in` & `libgzipf-20240422/ossfuzz/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -461,14 +461,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -525,16 +527,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@AM_CPPFLAGS = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -554,15 +556,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libgzipf/libgzipf.la \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .cc .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -804,23 +807,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/file_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -904,17 +910,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on file_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(file_fuzzer_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libgzipf-20240103/libgzipf.spec.in` & `libgzipf-20240422/libgzipf.spec.in`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/ltmain.sh` & `libgzipf-20240422/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcsplit/libcsplit_narrow_string.c` & `libgzipf-20240422/libcsplit/libcsplit_narrow_string.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Narrow character string functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcsplit/libcsplit_definitions.h` & `libgzipf-20240422/libcsplit/libcsplit_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -31,17 +31,17 @@
 #include <libcsplit/definitions.h>
 
 /* The definitions in <libcsplit/definitions.h> are copied here
  * for local use of libcsplit
  */
 #else
 
-#define LIBCSPLIT_VERSION			20220109
+#define LIBCSPLIT_VERSION			20240414
 
 /* The libcsplit version string
  */
-#define LIBCSPLIT_VERSION_STRING		"20220109"
+#define LIBCSPLIT_VERSION_STRING		"20240414"
 
 #endif /* !defined( HAVE_LOCAL_LIBCSPLIT ) */
 
 #endif
```

### Comparing `libgzipf-20240103/libcsplit/libcsplit_types.h` & `libgzipf-20240422/libcsplit/libcsplit_types.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcsplit/libcsplit_wide_split_string.c` & `libgzipf-20240422/libcsplit/libcsplit_wide_split_string.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Split wide string functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcsplit/libcsplit_support.h` & `libgzipf-20240422/libcsplit/libcsplit_support.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcsplit/Makefile.am` & `libgzipf-20240422/libcsplit/Makefile.am`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCSPLIT
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcsplit.la
 
 libcsplit_la_SOURCES = \
 	libcsplit_definitions.h \
 	libcsplit_error.c libcsplit_error.h \
@@ -16,17 +16,17 @@
 	libcsplit_support.c libcsplit_support.h \
 	libcsplit_types.h \
 	libcsplit_unused.h \
 	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 	libcsplit_wide_string.c libcsplit_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
```

### Comparing `libgzipf-20240103/libcsplit/libcsplit_libcerror.h` & `libgzipf-20240422/libcsplit/libcsplit_libcerror.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcsplit/libcsplit_wide_string.c` & `libgzipf-20240422/libcsplit/libcsplit_wide_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Wide character string functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcsplit/libcsplit_unused.h` & `libgzipf-20240422/libcsplit/libcsplit_unused.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcsplit/libcsplit_wide_split_string.h` & `libgzipf-20240422/libcsplit/libcsplit_wide_split_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Split wide string functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcsplit/libcsplit_error.c` & `libgzipf-20240422/libcsplit/libcsplit_error.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcsplit/libcsplit_narrow_split_string.c` & `libgzipf-20240422/libcsplit/libcsplit_narrow_split_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Split narrow string functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcsplit/libcsplit_extern.h` & `libgzipf-20240422/libcsplit/libcsplit_extern.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcsplit/libcsplit_error.h` & `libgzipf-20240422/libcsplit/libcsplit_error.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcsplit/libcsplit_support.c` & `libgzipf-20240422/libcsplit/libcsplit_support.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcsplit/libcsplit_wide_string.h` & `libgzipf-20240422/libcsplit/libcsplit_wide_string.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Wide character string functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcsplit/Makefile.in` & `libgzipf-20240422/libcsplit/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -458,14 +458,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -522,16 +524,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCSPLIT_TRUE@noinst_LTLIBRARIES = libcsplit.la
 @HAVE_LOCAL_LIBCSPLIT_TRUE@libcsplit_la_SOURCES = \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_definitions.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_error.c libcsplit_error.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_extern.h \
@@ -540,15 +542,16 @@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_libcerror.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_support.c libcsplit_support.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_types.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_unused.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_string.c libcsplit_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -753,24 +756,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcsplit_error.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_support.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -833,14 +844,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -851,23 +864,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libgzipf-20240103/libcsplit/libcsplit_narrow_split_string.h` & `libgzipf-20240422/libcsplit/libcsplit_narrow_split_string.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Split narrow string functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcsplit/libcsplit_narrow_string.h` & `libgzipf-20240422/libcsplit/libcsplit_narrow_string.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Narrow character string functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/pygzipf/pygzipf_member.h` & `libgzipf-20240422/pygzipf/pygzipf_member.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/pygzipf/pygzipf.c` & `libgzipf-20240422/pygzipf/pygzipf.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/pygzipf/pygzipf_codepage.h` & `libgzipf-20240422/pygzipf/pygzipf_codepage.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/pygzipf/pygzipf_error.h` & `libgzipf-20240422/pygzipf/pygzipf_error.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/pygzipf/pygzipf_python.h` & `libgzipf-20240422/pygzipf/pygzipf_python.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/pygzipf/pygzipf_integer.c` & `libgzipf-20240422/pygzipf/pygzipf_integer.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/pygzipf/pygzipf.h` & `libgzipf-20240422/pygzipf/pygzipf.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/pygzipf/pygzipf_file.h` & `libgzipf-20240422/pygzipf/pygzipf_file.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/pygzipf/Makefile.am` & `libgzipf-20240422/pygzipf/Makefile.am`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_PYTHON
 AM_CFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -43,13 +43,11 @@
 	@LIBBFIO_LIBADD@
 
 pygzipf_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pygzipf_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libgzipf-20240103/pygzipf/pygzipf_libcerror.h` & `libgzipf-20240422/pygzipf/pygzipf_libcerror.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/pygzipf/pygzipf_unused.h` & `libgzipf-20240422/pygzipf/pygzipf_unused.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/pygzipf/pygzipf_member.c` & `libgzipf-20240422/pygzipf/pygzipf_member.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/pygzipf/pygzipf_file_object_io_handle.c` & `libgzipf-20240422/pygzipf/pygzipf_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/pygzipf/pygzipf_libgzipf.h` & `libgzipf-20240422/pygzipf/pygzipf_libgzipf.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/pygzipf/pygzipf_datetime.h` & `libgzipf-20240422/pygzipf/pygzipf_datetime.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/pygzipf/pygzipf_members.c` & `libgzipf-20240422/pygzipf/pygzipf_members.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/pygzipf/pygzipf_codepage.c` & `libgzipf-20240422/pygzipf/pygzipf_codepage.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/pygzipf/pygzipf_error.c` & `libgzipf-20240422/pygzipf/pygzipf_error.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/pygzipf/pygzipf_libclocale.h` & `libgzipf-20240422/pygzipf/pygzipf_libclocale.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/pygzipf/pygzipf_file_object_io_handle.h` & `libgzipf-20240422/pygzipf/pygzipf_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/pygzipf/pygzipf_integer.h` & `libgzipf-20240422/pygzipf/pygzipf_integer.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/pygzipf/Makefile.in` & `libgzipf-20240422/pygzipf/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -494,14 +494,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -558,16 +560,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_PYTHON_TRUE@AM_CFLAGS = \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/include \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/common \
+@HAVE_PYTHON_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_PYTHON_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -601,15 +603,16 @@
 @HAVE_PYTHON_TRUE@	@LIBUNA_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBBFIO_LIBADD@
 
 @HAVE_PYTHON_TRUE@pygzipf_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pygzipf_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -907,24 +910,35 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-pyexecLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/pygzipf_la-pygzipf.Plo
+	-rm -f ./$(DEPDIR)/pygzipf_la-pygzipf_codepage.Plo
+	-rm -f ./$(DEPDIR)/pygzipf_la-pygzipf_datetime.Plo
+	-rm -f ./$(DEPDIR)/pygzipf_la-pygzipf_error.Plo
+	-rm -f ./$(DEPDIR)/pygzipf_la-pygzipf_file.Plo
+	-rm -f ./$(DEPDIR)/pygzipf_la-pygzipf_file_object_io_handle.Plo
+	-rm -f ./$(DEPDIR)/pygzipf_la-pygzipf_integer.Plo
+	-rm -f ./$(DEPDIR)/pygzipf_la-pygzipf_member.Plo
+	-rm -f ./$(DEPDIR)/pygzipf_la-pygzipf_members.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1017,13 +1031,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-pyexecLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libgzipf-20240103/pygzipf/pygzipf_members.h` & `libgzipf-20240422/pygzipf/pygzipf_members.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/pygzipf/pygzipf_file.c` & `libgzipf-20240422/pygzipf/pygzipf_file.c`

 * *Files 1% similar despite different names*

```diff
@@ -78,22 +78,22 @@
 	  "close() -> None\n"
 	  "\n"
 	  "Closes a file." },
 
 	{ "read_buffer",
 	  (PyCFunction) pygzipf_file_read_buffer,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read_buffer(size) -> Binary string\n"
+	  "read_buffer(size)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of uncompressed data from the current offset into a buffer." },
 
 	{ "read_buffer_at_offset",
 	  (PyCFunction) pygzipf_file_read_buffer_at_offset,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read_buffer_at_offset(size, offset) -> Binary string\n"
+	  "read_buffer_at_offset(size, offset)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of uncompressed data at a specific offset." },
 
 	{ "seek_offset",
 	  (PyCFunction) pygzipf_file_seek_offset,
 	  METH_VARARGS | METH_KEYWORDS,
 	  "seek_offset(offset, whence) -> None\n"
@@ -106,15 +106,15 @@
 	  "get_offset() -> Integer\n"
 	  "\n"
 	  "Retrieves the current offset of the uncompressed data." },
 
 	{ "read",
 	  (PyCFunction) pygzipf_file_read_buffer,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read(size) -> Binary string\n"
+	  "read(size)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of uncompressed data from the current offset into a buffer." },
 
 	{ "seek",
 	  (PyCFunction) pygzipf_file_seek_offset,
 	  METH_VARARGS | METH_KEYWORDS,
 	  "seek(offset, whence) -> None\n"
```

### Comparing `libgzipf-20240103/pygzipf/pygzipf_datetime.c` & `libgzipf-20240422/pygzipf/pygzipf_datetime.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/pygzipf/pygzipf_libbfio.h` & `libgzipf-20240422/pygzipf/pygzipf_libbfio.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/po/remove-potcdate.sin` & `libgzipf-20240422/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/po/Makefile.in.in` & `libgzipf-20240422/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/po/en@quot.header` & `libgzipf-20240422/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/po/en@boldquot.header` & `libgzipf-20240422/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/po/insert-header.sin` & `libgzipf-20240422/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/po/Makevars` & `libgzipf-20240422/po/Makevars`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/po/Makevars.in` & `libgzipf-20240422/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/po/Rules-quot` & `libgzipf-20240422/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_1251.c` & `libgzipf-20240422/libuna/libuna_codepage_windows_1251.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1251 codepage (Cyrillic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_utf16_string.c` & `libgzipf-20240422/libuna/libuna_utf16_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_base16_stream.c` & `libgzipf-20240422/libuna/libuna_base16_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base16 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_utf8_stream.h` & `libgzipf-20240422/libuna/libuna_utf8_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_iso_8859_2.h` & `libgzipf-20240422/libuna/libuna_codepage_iso_8859_2.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-2 codepage (Central European) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_932.c` & `libgzipf-20240422/libuna/libuna_codepage_windows_932.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 932 codepage (Japanese Shift-JIS) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_dingbats.h` & `libgzipf-20240422/libuna/libuna_codepage_mac_dingbats.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacDingbats codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_utf8_string.c` & `libgzipf-20240422/libuna/libuna_utf8_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_base64_stream.c` & `libgzipf-20240422/libuna/libuna_base64_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base64 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_error.h` & `libgzipf-20240422/libuna/libuna_error.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_turkish.h` & `libgzipf-20240422/libuna/libuna_codepage_mac_turkish.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacTurkish codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_unicode_character.c` & `libgzipf-20240422/libuna/libuna_unicode_character.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Unicode character functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_gaelic.c` & `libgzipf-20240422/libuna/libuna_codepage_mac_gaelic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacGaelic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_arabic.h` & `libgzipf-20240422/libuna/libuna_codepage_mac_arabic.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacArabic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_thai.c` & `libgzipf-20240422/libuna/libuna_codepage_mac_thai.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacThai codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_874.h` & `libgzipf-20240422/libuna/libuna_codepage_windows_874.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 874 codepage (Thai) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_iso_8859_15.h` & `libgzipf-20240422/libuna/libuna_codepage_iso_8859_9.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-15 codepage (Latin 9) functions
+ * ISO 8859-9 codepage (Turkish) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,31 +15,31 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_15_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_15_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_9_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_15_byte_stream_to_unicode_base_0xa0[ 32 ];
+const uint16_t libuna_codepage_iso_8859_9_byte_stream_to_unicode_base_0xd0[ 48 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_15_unicode_to_byte_stream_base_0x00a0[ 32 ];
+const uint8_t libuna_codepage_iso_8859_9_unicode_to_byte_stream_base_0x00d0[ 48 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_15_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H ) */
```

### Comparing `libgzipf-20240103/libuna/libuna_utf8_string.h` & `libgzipf-20240422/libuna/libuna_utf8_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_iso_8859_16.c` & `libgzipf-20240422/libuna/libuna_codepage_iso_8859_16.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-16 codepage (Latin 10) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_1255.c` & `libgzipf-20240422/libuna/libuna_codepage_windows_1255.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1255 codepage (Hebrew) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_utf7_stream.c` & `libgzipf-20240422/libuna/libuna_utf7_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-7 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_byte_stream.h` & `libgzipf-20240422/libuna/libuna_byte_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Byte stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_koi8_u.c` & `libgzipf-20240422/libuna/libuna_codepage_koi8_u.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-U codepage (Ukrainian Cyrillic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_unused.h` & `libgzipf-20240422/libuna/libuna_unused.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_iso_8859_6.c` & `libgzipf-20240422/libuna/libuna_codepage_iso_8859_6.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-6 codepage (Arabic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_iso_8859_14.c` & `libgzipf-20240422/libuna/libuna_codepage_iso_8859_14.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-14 codepage (Celtic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_base64_stream.h` & `libgzipf-20240422/libuna/libuna_base64_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base64 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_error.c` & `libgzipf-20240422/libuna/libuna_error.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_centraleurroman.h` & `libgzipf-20240422/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCentralEurRoman codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_romanian.c` & `libgzipf-20240422/libuna/libuna_codepage_mac_romanian.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRomanian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_iso_8859_6.h` & `libgzipf-20240422/libuna/libuna_codepage_iso_8859_6.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-6 codepage (Arabic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_iso_8859_9.c` & `libgzipf-20240422/libuna/libuna_codepage_iso_8859_9.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-9 codepage (Turkish) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_russian.h` & `libgzipf-20240422/libuna/libuna_codepage_mac_russian.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRussian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_dingbats.c` & `libgzipf-20240422/libuna/libuna_codepage_mac_dingbats.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacDingbats codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_iso_8859_15.c` & `libgzipf-20240422/libuna/libuna_codepage_iso_8859_15.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-15 codepage (Latin 9) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_936.c` & `libgzipf-20240422/libuna/libuna_codepage_windows_936.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 936 codepage (Chinese Simplified) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_croatian.h` & `libgzipf-20240422/libuna/libuna_codepage_mac_croatian.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCroatian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_scsu.h` & `libgzipf-20240422/libuna/libuna_scsu.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Standard Compression Scheme for Unicode (SCSU) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/Makefile.am` & `libgzipf-20240422/libuna/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBUNA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libuna.la
 
 libuna_la_SOURCES = \
 	libuna_base16_stream.c libuna_base16_stream.h \
 	libuna_base32_stream.c libuna_base32_stream.h \
@@ -73,17 +73,17 @@
 	libuna_utf32_stream.c libuna_utf32_stream.h \
 	libuna_utf32_string.c libuna_utf32_string.h \
 	libuna_utf7_stream.c libuna_utf7_stream.h \
 	libuna_utf8_stream.c libuna_utf8_stream.h \
 	libuna_utf8_string.c libuna_utf8_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
```

### Comparing `libgzipf-20240103/libuna/libuna_utf32_stream.c` & `libgzipf-20240422/libuna/libuna_utf32_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_936.h` & `libgzipf-20240422/libuna/libuna_codepage_windows_936.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 936 codepage (Chinese Simplified) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_iso_8859_10.c` & `libgzipf-20240422/libuna/libuna_codepage_iso_8859_10.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-10 codepage (Nordic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_roman.c` & `libgzipf-20240422/libuna/libuna_codepage_mac_roman.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRoman codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_utf7_stream.h` & `libgzipf-20240422/libuna/libuna_utf7_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-7 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_iso_8859_3.h` & `libgzipf-20240422/libuna/libuna_codepage_iso_8859_3.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-3 codepage (Latin 3) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_thai.h` & `libgzipf-20240422/libuna/libuna_codepage_mac_thai.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacThai codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_farsi.h` & `libgzipf-20240422/libuna/libuna_codepage_mac_farsi.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacFarsi codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_ukrainian.c` & `libgzipf-20240422/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacUkrainian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_inuit.c` & `libgzipf-20240422/libuna/libuna_codepage_mac_inuit.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacInuit codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_932.h` & `libgzipf-20240422/libuna/libuna_codepage_windows_932.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 932 codepage (Japanese Shift-JIS) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_874.c` & `libgzipf-20240422/libuna/libuna_codepage_windows_874.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 874 codepage (Thai) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_iso_8859_5.c` & `libgzipf-20240422/libuna/libuna_codepage_iso_8859_5.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-5 codepage (Cyrillic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_iso_8859_10.h` & `libgzipf-20240422/libuna/libuna_codepage_iso_8859_10.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-10 codepage (Nordic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_definitions.h` & `libgzipf-20240422/libuna/libuna_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -31,19 +31,19 @@
 
 /* The definitions in <libuna/definitions.h> are copied here
  * for local use of libuna
  */
 #else
 #include <byte_stream.h>
 
-#define LIBUNA_VERSION						20230710
+#define LIBUNA_VERSION						20240414
 
 /* The libuna version string
  */
-#define LIBUNA_VERSION_STRING					"20230710"
+#define LIBUNA_VERSION_STRING					"20240414"
 
 /* The endian definitions
  */
 #define	LIBUNA_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define	LIBUNA_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The codepage definitions
```

### Comparing `libgzipf-20240103/libuna/libuna_url_stream.h` & `libgzipf-20240422/libuna/libuna_url_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Percent or URL encoded stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_icelandic.h` & `libgzipf-20240422/libuna/libuna_codepage_mac_icelandic.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacIcelandic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_koi8_u.h` & `libgzipf-20240422/libuna/libuna_codepage_koi8_u.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-U codepage (Ukrainian Cyrillic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_utf16_stream.c` & `libgzipf-20240422/libuna/libuna_utf16_stream.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_1253.c` & `libgzipf-20240422/libuna/libuna_codepage_windows_1253.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1253 codepage (Greek) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_iso_8859_4.h` & `libgzipf-20240422/libuna/libuna_codepage_iso_8859_4.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-4 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_greek.c` & `libgzipf-20240422/libuna/libuna_codepage_mac_greek.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacGreek codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_libcerror.h` & `libgzipf-20240422/libuna/libuna_libcerror.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_centraleurroman.c` & `libgzipf-20240422/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCentralEurRoman codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_1254.c` & `libgzipf-20240422/libuna/libuna_codepage_windows_1254.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1254 codepage (Turkish) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_iso_8859_13.h` & `libgzipf-20240422/libuna/libuna_codepage_iso_8859_13.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-13 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_iso_8859_7.h` & `libgzipf-20240422/libuna/libuna_codepage_iso_8859_7.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-7 codepage (Greek) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_1255.h` & `libgzipf-20240422/libuna/libuna_codepage_windows_1251.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Windows 1255 codepage (Hebrew) functions
+ * Windows 1251 codepage (Cyrillic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1255_H )
-#define _LIBUNA_CODEPAGE_WINDOWS_1255_H
+#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1251_H )
+#define _LIBUNA_CODEPAGE_WINDOWS_1251_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_windows_1255_copy_from_byte_stream(
+int libuna_codepage_windows_1251_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_windows_1255_copy_to_byte_stream(
+int libuna_codepage_windows_1251_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1255_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1251_H ) */
```

### Comparing `libgzipf-20240103/libuna/libuna_unicode_character.h` & `libgzipf-20240422/libuna/libuna_unicode_character.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Unicode character functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_iso_8859_8.h` & `libgzipf-20240422/libuna/libuna_codepage_iso_8859_8.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-8 codepage (Hebrew) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_iso_8859_13.c` & `libgzipf-20240422/libuna/libuna_codepage_iso_8859_13.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-13 codepage (Baltic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_949.h` & `libgzipf-20240422/libuna/libuna_codepage_windows_949.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 949 codepage (Korean) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_cyrillic.c` & `libgzipf-20240422/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCyrillic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_celtic.c` & `libgzipf-20240422/libuna/libuna_codepage_mac_celtic.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCeltic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_support.h` & `libgzipf-20240422/libuna/libuna_support.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_iso_8859_4.c` & `libgzipf-20240422/libuna/libuna_codepage_iso_8859_4.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-4 codepage (Baltic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_949.c` & `libgzipf-20240422/libuna/libuna_codepage_windows_949.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 949 codepage (Korean) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_utf16_stream.h` & `libgzipf-20240422/libuna/libuna_utf16_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_symbol.c` & `libgzipf-20240422/libuna/libuna_codepage_mac_symbol.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacSymbol codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_roman.h` & `libgzipf-20240422/libuna/libuna_codepage_mac_roman.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRoman codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_1257.c` & `libgzipf-20240422/libuna/libuna_codepage_windows_1257.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1257 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_1254.h` & `libgzipf-20240422/libuna/libuna_codepage_windows_1254.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1254 codepage (Turkish) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_950.c` & `libgzipf-20240422/libuna/libuna_codepage_windows_950.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 950 codepage (Traditional Chinese) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_extern.h` & `libgzipf-20240422/libuna/libuna_extern.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_1256.c` & `libgzipf-20240422/libuna/libuna_codepage_windows_1256.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1256 codepage (Arabic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_types.h` & `libgzipf-20240422/libuna/libuna_types.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_base32_stream.h` & `libgzipf-20240422/libuna/libuna_base32_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base32 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_1253.h` & `libgzipf-20240422/libuna/libuna_codepage_windows_1253.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1253 codepage (Greek) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_iso_8859_16.h` & `libgzipf-20240422/libuna/libuna_codepage_iso_8859_16.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-16 codepage (Latin 10) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_utf8_stream.c` & `libgzipf-20240422/libuna/libuna_utf8_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_1250.h` & `libgzipf-20240422/libuna/libuna_codepage_windows_1250.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1250 codepage (Central European) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_iso_8859_2.c` & `libgzipf-20240422/libuna/libuna_codepage_iso_8859_2.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-2 codepage (Central European) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_support.c` & `libgzipf-20240422/libuna/libuna_support.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_koi8_r.c` & `libgzipf-20240422/libuna/libuna_codepage_koi8_r.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-R codepage (Russian Cyrillic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_iso_8859_5.h` & `libgzipf-20240422/libuna/libuna_codepage_iso_8859_15.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-5 codepage (Cyrillic) functions
+ * ISO 8859-15 codepage (Latin 9) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,31 +15,31 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_5_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_15_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_15_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_5_byte_stream_to_unicode_base_0xa0[ 96 ];
+const uint16_t libuna_codepage_iso_8859_15_byte_stream_to_unicode_base_0xa0[ 32 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_5_unicode_to_byte_stream_base_0x0400[ 96 ];
+const uint8_t libuna_codepage_iso_8859_15_unicode_to_byte_stream_base_0x00a0[ 32 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_15_H ) */
```

### Comparing `libgzipf-20240103/libuna/libuna_utf16_string.h` & `libgzipf-20240422/libuna/libuna_utf16_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_utf32_string.c` & `libgzipf-20240422/libuna/libuna_utf32_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_icelandic.c` & `libgzipf-20240422/libuna/libuna_codepage_mac_icelandic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacIcelandic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_1256.h` & `libgzipf-20240422/libuna/libuna_codepage_windows_1256.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1256 codepage (Arabic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_utf32_string.h` & `libgzipf-20240422/libuna/libuna_utf32_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_romanian.h` & `libgzipf-20240422/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacRomanian codepage functions
+ * MacCyrillic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H )
-#define _LIBUNA_CODEPAGE_MAC_ROMANIAN_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_CYRILLIC_H )
+#define _LIBUNA_CODEPAGE_MAC_CYRILLIC_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_romanian_copy_from_byte_stream(
+int libuna_codepage_mac_cyrillic_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_romanian_copy_to_byte_stream(
+int libuna_codepage_mac_cyrillic_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_CYRILLIC_H ) */
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_iso_8859_8.c` & `libgzipf-20240422/libuna/libuna_codepage_iso_8859_8.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-8 codepage (Hebrew) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_koi8_r.h` & `libgzipf-20240422/libuna/libuna_codepage_koi8_r.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-R codepage (Russian Cyrillic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_cyrillic.h` & `libgzipf-20240422/libuna/libuna_codepage_mac_gaelic.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacCyrillic codepage functions
+ * MacGaelic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_CYRILLIC_H )
-#define _LIBUNA_CODEPAGE_MAC_CYRILLIC_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_GAELIC_H )
+#define _LIBUNA_CODEPAGE_MAC_GAELIC_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_cyrillic_copy_from_byte_stream(
+int libuna_codepage_mac_gaelic_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_cyrillic_copy_to_byte_stream(
+int libuna_codepage_mac_gaelic_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_CYRILLIC_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_GAELIC_H ) */
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_arabic.c` & `libgzipf-20240422/libuna/libuna_codepage_mac_arabic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacArabic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_croatian.c` & `libgzipf-20240422/libuna/libuna_codepage_mac_croatian.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCroatian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_iso_8859_9.h` & `libgzipf-20240422/libuna/libuna_codepage_iso_8859_5.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-9 codepage (Turkish) functions
+ * ISO 8859-5 codepage (Cyrillic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,31 +15,31 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_9_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_5_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_9_byte_stream_to_unicode_base_0xd0[ 48 ];
+const uint16_t libuna_codepage_iso_8859_5_byte_stream_to_unicode_base_0xa0[ 96 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_9_unicode_to_byte_stream_base_0x00d0[ 48 ];
+const uint8_t libuna_codepage_iso_8859_5_unicode_to_byte_stream_base_0x0400[ 96 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H ) */
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_greek.h` & `libgzipf-20240422/libuna/libuna_codepage_mac_greek.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacGreek codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_1258.h` & `libgzipf-20240422/libuna/libuna_codepage_windows_1258.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1258 codepage (Vietnamese) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_iso_8859_7.c` & `libgzipf-20240422/libuna/libuna_codepage_iso_8859_7.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-7 codepage (Greek) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/Makefile.in` & `libgzipf-20240422/libuna/Makefile.in`

 * *Files 10% similar despite different names*

```diff
@@ -626,14 +626,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -690,16 +692,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBUNA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBUNA_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBUNA_TRUE@noinst_LTLIBRARIES = libuna.la
 @HAVE_LOCAL_LIBUNA_TRUE@libuna_la_SOURCES = \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base16_stream.c libuna_base16_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base32_stream.c libuna_base32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base64_stream.c libuna_base64_stream.h \
@@ -765,15 +767,16 @@
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf16_string.c libuna_utf16_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_stream.c libuna_utf32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_string.c libuna_utf32_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf7_stream.c libuna_utf7_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_stream.c libuna_utf8_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_string.c libuna_utf8_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -1035,24 +1038,89 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libuna_base16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base64_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_byte_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_10.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_13.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_14.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_15.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_16.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_2.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_3.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_4.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_5.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_6.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_7.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_8.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_9.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_r.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_u.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_arabic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_celtic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_centraleurroman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_croatian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_cyrillic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_dingbats.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_farsi.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_gaelic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_greek.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_icelandic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_inuit.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_roman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_romanian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_russian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_symbol.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_thai.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_turkish.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_ukrainian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1250.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1251.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1252.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1253.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1254.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1255.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1256.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1257.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1258.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_874.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_932.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_936.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_949.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_950.Plo
+	-rm -f ./$(DEPDIR)/libuna_error.Plo
+	-rm -f ./$(DEPDIR)/libuna_scsu.Plo
+	-rm -f ./$(DEPDIR)/libuna_support.Plo
+	-rm -f ./$(DEPDIR)/libuna_unicode_character.Plo
+	-rm -f ./$(DEPDIR)/libuna_url_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf7_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1172,14 +1240,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -1190,23 +1260,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_iso_8859_3.c` & `libgzipf-20240422/libuna/libuna_codepage_iso_8859_3.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-3 codepage (Latin 3) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_1250.c` & `libgzipf-20240422/libuna/libuna_codepage_windows_1250.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1250 codepage (Central European) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_scsu.c` & `libgzipf-20240422/libuna/libuna_scsu.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Standard Compression Scheme for Unicode (SCSU) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_1252.c` & `libgzipf-20240422/libuna/libuna_codepage_windows_1252.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1252 codepage (Western European/Latin 1) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_turkish.c` & `libgzipf-20240422/libuna/libuna_codepage_mac_turkish.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacTurkish codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_ukrainian.h` & `libgzipf-20240422/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacUkrainian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_russian.c` & `libgzipf-20240422/libuna/libuna_codepage_mac_russian.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRussian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_1258.c` & `libgzipf-20240422/libuna/libuna_codepage_windows_1258.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1258 codepage (Vietnamese) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_celtic.h` & `libgzipf-20240422/libuna/libuna_codepage_mac_celtic.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCeltic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_byte_stream.c` & `libgzipf-20240422/libuna/libuna_byte_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Byte stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_gaelic.h` & `libgzipf-20240422/libuna/libuna_codepage_windows_1257.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacGaelic codepage functions
+ * Windows 1257 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_GAELIC_H )
-#define _LIBUNA_CODEPAGE_MAC_GAELIC_H
+#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1257_H )
+#define _LIBUNA_CODEPAGE_WINDOWS_1257_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_gaelic_copy_from_byte_stream(
+int libuna_codepage_windows_1257_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_gaelic_copy_to_byte_stream(
+int libuna_codepage_windows_1257_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_GAELIC_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1257_H ) */
```

### Comparing `libgzipf-20240103/libuna/libuna_utf32_stream.h` & `libgzipf-20240422/libuna/libuna_utf32_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_symbol.h` & `libgzipf-20240422/libuna/libuna_codepage_mac_symbol.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacSymbol codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_1257.h` & `libgzipf-20240422/libuna/libuna_codepage_mac_inuit.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Windows 1257 codepage (Baltic) functions
+ * MacInuit codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1257_H )
-#define _LIBUNA_CODEPAGE_WINDOWS_1257_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_INUIT_H )
+#define _LIBUNA_CODEPAGE_MAC_INUIT_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_windows_1257_copy_from_byte_stream(
+int libuna_codepage_mac_inuit_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_windows_1257_copy_to_byte_stream(
+int libuna_codepage_mac_inuit_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1257_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_INUIT_H ) */
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_inuit.h` & `libgzipf-20240422/libuna/libuna_codepage_mac_romanian.h`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacInuit codepage functions
+ * MacRomanian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_INUIT_H )
-#define _LIBUNA_CODEPAGE_MAC_INUIT_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H )
+#define _LIBUNA_CODEPAGE_MAC_ROMANIAN_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_inuit_copy_from_byte_stream(
+int libuna_codepage_mac_romanian_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_inuit_copy_to_byte_stream(
+int libuna_codepage_mac_romanian_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_INUIT_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H ) */
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_mac_farsi.c` & `libgzipf-20240422/libuna/libuna_codepage_mac_farsi.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacFarsi codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_950.h` & `libgzipf-20240422/libuna/libuna_codepage_windows_950.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 950 codepage (Traditional Chinese) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_url_stream.c` & `libgzipf-20240422/libuna/libuna_url_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Percent or URL encoded stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_1251.h` & `libgzipf-20240422/libuna/libuna_codepage_windows_1255.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Windows 1251 codepage (Cyrillic) functions
+ * Windows 1255 codepage (Hebrew) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1251_H )
-#define _LIBUNA_CODEPAGE_WINDOWS_1251_H
+#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1255_H )
+#define _LIBUNA_CODEPAGE_WINDOWS_1255_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_windows_1251_copy_from_byte_stream(
+int libuna_codepage_windows_1255_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_windows_1251_copy_to_byte_stream(
+int libuna_codepage_windows_1255_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1251_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1255_H ) */
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_windows_1252.h` & `libgzipf-20240422/libuna/libuna_codepage_windows_1252.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1252 codepage (Western European/Latin 1) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_codepage_iso_8859_14.h` & `libgzipf-20240422/libuna/libuna_codepage_iso_8859_14.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-14 codepage (Celtic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_base16_stream.h` & `libgzipf-20240422/libuna/libuna_base16_stream.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base16 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libuna/libuna_base32_stream.c` & `libgzipf-20240422/libuna/libuna_base32_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base32 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/Makefile.in` & `libgzipf-20240422/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -508,14 +508,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -634,16 +636,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libgzipf.pc \
+	libgzipf.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libgzipf.pc
 
 all: all-recursive
 
@@ -1060,23 +1069,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-recursive
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-recursive
+	-rm -f $(am__CONFIG_DISTCLEAN_FILES)
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-libtool \
 	distclean-tags
 
 dvi: dvi-recursive
 
 dvi-am:
 
@@ -1186,22 +1198,10 @@
 	(cd $(srcdir)/libbfio && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfcache && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdata && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfdatetime && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libgzipf && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libgzipf.pc
-	-rm -f libgzipf.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libgzipf-20240103/libcnotify/libcnotify_definitions.h` & `libgzipf-20240422/libcnotify/libcnotify_definitions.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -31,19 +31,19 @@
 #include <libcnotify/definitions.h>
 
 /* The definitions in <libcnotify/definitions.h> are copied here
  * for local use of libcnotify
  */
 #else
 
-#define LIBCNOTIFY_VERSION				20220108
+#define LIBCNOTIFY_VERSION				20240414
 
 /* The libcnotify version string
  */
-#define LIBCNOTIFY_VERSION_STRING			"20220108"
+#define LIBCNOTIFY_VERSION_STRING			"20240414"
 
 /* The print data flags
  */
 enum LIBCNOTIFY_NOTIFY_PRINT_DATA_FLAGS
 {
 	LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA		= 0x01,
 };
```

### Comparing `libgzipf-20240103/libcnotify/libcnotify_extern.h` & `libgzipf-20240422/libcnotify/libcnotify_extern.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcnotify/libcnotify_support.c` & `libgzipf-20240422/libcerror/libcerror_support.c`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -18,22 +18,22 @@
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
 #include <types.h>
 
-#include "libcnotify_definitions.h"
-#include "libcnotify_support.h"
+#include "libcerror_definitions.h"
+#include "libcerror_support.h"
 
-#if !defined( HAVE_LOCAL_LIBCNOTIFY )
+#if !defined( HAVE_LOCAL_LIBCERROR )
 
 /* Returns the library version as a string
  */
-const char *libcnotify_get_version(
+const char *libcerror_get_version(
              void )
 {
-	return( (const char *) LIBCNOTIFY_VERSION_STRING );
+	return( (const char *) LIBCERROR_VERSION_STRING );
 }
 
-#endif /* !defined( HAVE_LOCAL_LIBCNOTIFY ) */
+#endif /* !defined( HAVE_LOCAL_LIBCERROR ) */
```

### Comparing `libgzipf-20240103/libcnotify/libcnotify_stream.h` & `libgzipf-20240422/libcnotify/libcnotify_stream.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Notification stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcnotify/Makefile.am` & `libgzipf-20240422/libcnotify/Makefile.am`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCNOTIFY
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcnotify.la
 
 libcnotify_la_SOURCES = \
 	libcnotify_definitions.h \
 	libcnotify_extern.h \
@@ -13,17 +13,17 @@
 	libcnotify_print.c libcnotify_print.h \
 	libcnotify_stream.c libcnotify_stream.h \
 	libcnotify_support.c libcnotify_support.h \
 	libcnotify_unused.h \
 	libcnotify_verbose.c libcnotify_verbose.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
```

### Comparing `libgzipf-20240103/libcnotify/libcnotify_unused.h` & `libgzipf-20240422/libcnotify/libcnotify_unused.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcnotify/libcnotify_verbose.h` & `libgzipf-20240422/libcnotify/libcnotify_verbose.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Verbose functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcnotify/libcnotify_print.h` & `libgzipf-20240422/libcnotify/libcnotify_print.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Notification print functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcnotify/libcnotify_stream.c` & `libgzipf-20240422/libcnotify/libcnotify_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Notification stream functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcnotify/libcnotify_support.h` & `libgzipf-20240422/libcnotify/libcnotify_support.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcnotify/libcnotify_verbose.c` & `libgzipf-20240422/libcnotify/libcnotify_verbose.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Verbose functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcnotify/Makefile.in` & `libgzipf-20240422/libcnotify/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -450,14 +450,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -514,30 +516,31 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@noinst_LTLIBRARIES = libcnotify.la
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@libcnotify_la_SOURCES = \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_definitions.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_extern.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_libcerror.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_print.c libcnotify_print.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_stream.c libcnotify_stream.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_support.c libcnotify_support.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_unused.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_verbose.c libcnotify_verbose.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -740,24 +743,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcnotify_print.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_stream.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_support.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_verbose.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -818,14 +827,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -836,23 +847,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libgzipf-20240103/libcnotify/libcnotify_libcerror.h` & `libgzipf-20240422/libfdatetime/libfdatetime_libcerror.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * The internal libcerror header
+ * The libcerror header wrapper
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBCNOTIFY_LIBCERROR_H )
-#define _LIBCNOTIFY_LIBCERROR_H
+#if !defined( _LIBFDATETIME_LIBCERROR_H )
+#define _LIBFDATETIME_LIBCERROR_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCERROR for local use of libcerror
  */
 #if defined( HAVE_LOCAL_LIBCERROR )
 
@@ -40,11 +40,11 @@
  */
 #if defined( _WIN32 ) && defined( DLL_IMPORT )
 #define LIBCERROR_DLL_IMPORT
 #endif
 
 #include <libcerror.h>
 
-#endif
+#endif /* defined( HAVE_LOCAL_LIBCERROR ) */
 
-#endif
+#endif /* !defined( _LIBFDATETIME_LIBCERROR_H ) */
```

### Comparing `libgzipf-20240103/libcnotify/libcnotify_print.c` & `libgzipf-20240422/libcnotify/libcnotify_print.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Notification print functions
  *
- * Copyright (C) 2008-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libcerror/libcerror_system.c` & `libgzipf-20240422/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcerror/libcerror_error.c` & `libgzipf-20240422/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcerror/libcerror_extern.h` & `libgzipf-20240422/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcerror/Makefile.am` & `libgzipf-20240422/libcerror/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 if HAVE_LOCAL_LIBCERROR
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common 
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common 
 
 noinst_LTLIBRARIES = libcerror.la
 
 libcerror_la_SOURCES = \
 	libcerror_definitions.h \
 	libcerror_extern.h \
 	libcerror_error.c libcerror_error.h \
 	libcerror_support.c libcerror_support.h \
 	libcerror_system.c libcerror_system.h \
 	libcerror_types.h \
 	libcerror_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
```

### Comparing `libgzipf-20240103/libcerror/libcerror_types.h` & `libgzipf-20240422/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcerror/libcerror_support.h` & `libgzipf-20240422/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcerror/libcerror_error.h` & `libgzipf-20240422/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcerror/libcerror_system.h` & `libgzipf-20240422/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcerror/libcerror_definitions.h` & `libgzipf-20240422/libcerror/libcerror_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcerror/definitions.h>
 
 /* The definitions in <libcerror/definitions.h> are copied here
  * for local use of libcerror
  */
 #else
 
-#define LIBCERROR_VERSION				20240101
+#define LIBCERROR_VERSION				20240413
 
 /* The libcerror version string
  */
-#define LIBCERROR_VERSION_STRING			"20240101"
+#define LIBCERROR_VERSION_STRING			"20240413"
 
 /* The error domains
  */
 enum LIBCERROR_ERROR_DOMAINS
 {
 	LIBCERROR_ERROR_DOMAIN_ARGUMENTS		= (int) 'a',
 	LIBCERROR_ERROR_DOMAIN_CONVERSION		= (int) 'c',
```

### Comparing `libgzipf-20240103/libcerror/libcerror_support.c` & `libgzipf-20240422/libfdatetime/libfdatetime_support.c`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -18,22 +18,24 @@
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
 #include <types.h>
 
-#include "libcerror_definitions.h"
-#include "libcerror_support.h"
+#include <stdio.h>
 
-#if !defined( HAVE_LOCAL_LIBCERROR )
+#include "libfdatetime_definitions.h"
+#include "libfdatetime_support.h"
+
+#if !defined( HAVE_LOCAL_LIBFDATETIME )
 
 /* Returns the library version as a string
  */
-const char *libcerror_get_version(
+const char *libfdatetime_get_version(
              void )
 {
-	return( (const char *) LIBCERROR_VERSION_STRING );
+	return( (const char *) LIBFDATETIME_VERSION_STRING );
 }
 
-#endif /* !defined( HAVE_LOCAL_LIBCERROR ) */
+#endif
```

### Comparing `libgzipf-20240103/libcerror/libcerror_unused.h` & `libgzipf-20240422/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/libcerror/Makefile.in` & `libgzipf-20240422/libcerror/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -447,14 +447,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -511,28 +513,29 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBCERROR_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/common 
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../common -I$(top_srcdir)/common 
 
 @HAVE_LOCAL_LIBCERROR_TRUE@noinst_LTLIBRARIES = libcerror.la
 @HAVE_LOCAL_LIBCERROR_TRUE@libcerror_la_SOURCES = \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_definitions.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_extern.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_error.c libcerror_error.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_support.c libcerror_support.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_system.c libcerror_system.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_types.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -734,24 +737,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcerror_error.Plo
+	-rm -f ./$(DEPDIR)/libcerror_support.Plo
+	-rm -f ./$(DEPDIR)/libcerror_system.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -837,17 +845,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libgzipf-20240103/libfdatetime/libfdatetime_floatingtime.h` & `libgzipf-20240422/libfdatetime/libfdatetime_floatingtime.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Floatingtime functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdatetime/libfdatetime_nsf_timedate.c` & `libgzipf-20240422/libfdatetime/libfdatetime_nsf_timedate.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Notes Storage Facility (NSF) timedate functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdatetime/libfdatetime_error.h` & `libgzipf-20240422/libfdatetime/libfdatetime_error.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdatetime/libfdatetime_floatingtime.c` & `libgzipf-20240422/libfdatetime/libfdatetime_floatingtime.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Floatingtime functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdatetime/libfdatetime_support.h` & `libgzipf-20240422/libfdatetime/libfdatetime_support.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdatetime/libfdatetime_hfs_time.h` & `libgzipf-20240422/libfdatetime/libfdatetime_hfs_time.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * HFS time functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdatetime/libfdatetime_definitions.h` & `libgzipf-20240422/libfdatetime/libfdatetime_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfdatetime/definitions.h> are copied here
  * for local use of libfdatetime
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFDATETIME_VERSION					20220112
+#define LIBFDATETIME_VERSION					20240415
 
 /* The version string
  */
-#define LIBFDATETIME_VERSION_STRING				"20220112"
+#define LIBFDATETIME_VERSION_STRING				"20240415"
 
 /* The byte order definitions
  */
 #define LIBFDATETIME_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFDATETIME_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The string format definition flags
```

### Comparing `libgzipf-20240103/libfdatetime/libfdatetime_hfs_time.c` & `libgzipf-20240422/libfdatetime/libfdatetime_hfs_time.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * HFS time functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdatetime/Makefile.am` & `libgzipf-20240422/libfdatetime/Makefile.am`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFDATETIME
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfdatetime.la
 
 libfdatetime_la_SOURCES = \
 	libfdatetime_date_time_values.c libfdatetime_date_time_values.h \
 	libfdatetime_definitions.h \
@@ -20,17 +20,17 @@
 	libfdatetime_posix_time.c libfdatetime_posix_time.h \
 	libfdatetime_support.c libfdatetime_support.h \
 	libfdatetime_systemtime.c libfdatetime_systemtime.h \
 	libfdatetime_types.h \
 	libfdatetime_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libfdatetime ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdatetime_la_SOURCES)
```

### Comparing `libgzipf-20240103/libfdatetime/libfdatetime_filetime.c` & `libgzipf-20240422/libfdatetime/libfdatetime_filetime.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * FILETIME functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdatetime/libfdatetime_systemtime.h` & `libgzipf-20240422/libfdatetime/libfdatetime_systemtime.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SYSTEMTIME functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdatetime/libfdatetime_extern.h` & `libgzipf-20240422/libfdatetime/libfdatetime_extern.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdatetime/libfdatetime_posix_time.c` & `libgzipf-20240422/libfdatetime/libfdatetime_posix_time.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * POSIX time functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdatetime/libfdatetime_unused.h` & `libgzipf-20240422/libfdatetime/libfdatetime_unused.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdatetime/libfdatetime_fat_date_time.h` & `libgzipf-20240422/libfdatetime/libfdatetime_fat_date_time.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * FAT date and time functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdatetime/libfdatetime_systemtime.c` & `libgzipf-20240422/libfdatetime/libfdatetime_systemtime.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SYSTEMTIME functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdatetime/libfdatetime_nsf_timedate.h` & `libgzipf-20240422/libfdatetime/libfdatetime_nsf_timedate.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Notes Storage Facility (NSF) timedate functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdatetime/libfdatetime_libcerror.h` & `libgzipf-20240422/libcnotify/libcnotify_libcerror.h`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * The libcerror header wrapper
+ * The internal libcerror header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBFDATETIME_LIBCERROR_H )
-#define _LIBFDATETIME_LIBCERROR_H
+#if !defined( _LIBCNOTIFY_LIBCERROR_H )
+#define _LIBCNOTIFY_LIBCERROR_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCERROR for local use of libcerror
  */
 #if defined( HAVE_LOCAL_LIBCERROR )
 
@@ -40,11 +40,11 @@
  */
 #if defined( _WIN32 ) && defined( DLL_IMPORT )
 #define LIBCERROR_DLL_IMPORT
 #endif
 
 #include <libcerror.h>
 
-#endif /* defined( HAVE_LOCAL_LIBCERROR ) */
+#endif
 
-#endif /* !defined( _LIBFDATETIME_LIBCERROR_H ) */
+#endif
```

### Comparing `libgzipf-20240103/libfdatetime/libfdatetime_support.c` & `libgzipf-20240422/libfdata/libfdata_support.c`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -20,22 +20,22 @@
  */
 
 #include <common.h>
 #include <types.h>
 
 #include <stdio.h>
 
-#include "libfdatetime_definitions.h"
-#include "libfdatetime_support.h"
+#include "libfdata_definitions.h"
+#include "libfdata_support.h"
 
-#if !defined( HAVE_LOCAL_LIBFDATETIME )
+#if !defined( HAVE_LOCAL_LIBFDATA )
 
 /* Returns the library version as a string
  */
-const char *libfdatetime_get_version(
+const char *libfdata_get_version(
              void )
 {
-	return( (const char *) LIBFDATETIME_VERSION_STRING );
+	return( (const char *) LIBFDATA_VERSION_STRING );
 }
 
-#endif
+#endif /* !defined( HAVE_LOCAL_LIBFDATA ) */
```

### Comparing `libgzipf-20240103/libfdatetime/libfdatetime_error.c` & `libgzipf-20240422/libfdatetime/libfdatetime_error.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdatetime/libfdatetime_posix_time.h` & `libgzipf-20240422/libfdatetime/libfdatetime_posix_time.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * POSIX time functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdatetime/libfdatetime_date_time_values.h` & `libgzipf-20240422/libfdatetime/libfdatetime_date_time_values.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Date and time values functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdatetime/libfdatetime_filetime.h` & `libgzipf-20240422/libfdatetime/libfdatetime_filetime.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * FILETIME functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdatetime/libfdatetime_date_time_values.c` & `libgzipf-20240422/libfdatetime/libfdatetime_date_time_values.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Date and time values functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdatetime/libfdatetime_types.h` & `libgzipf-20240422/libfdatetime/libfdatetime_types.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/libfdatetime/Makefile.in` & `libgzipf-20240422/libfdatetime/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -469,14 +469,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -533,16 +535,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBFDATETIME_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFDATETIME_TRUE@noinst_LTLIBRARIES = libfdatetime.la
 @HAVE_LOCAL_LIBFDATETIME_TRUE@libfdatetime_la_SOURCES = \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_date_time_values.c libfdatetime_date_time_values.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_definitions.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_extern.h \
@@ -555,15 +557,16 @@
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_nsf_timedate.c libfdatetime_nsf_timedate.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_posix_time.c libfdatetime_posix_time.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_support.c libfdatetime_support.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_systemtime.c libfdatetime_systemtime.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_types.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -772,24 +775,36 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfdatetime_date_time_values.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_error.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_fat_date_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_filetime.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_floatingtime.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_hfs_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_nsf_timedate.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_posix_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_support.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_systemtime.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -856,14 +871,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -874,23 +891,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libfdatetime ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdatetime_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libgzipf-20240103/libfdatetime/libfdatetime_fat_date_time.c` & `libgzipf-20240422/libfdatetime/libfdatetime_fat_date_time.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * FAT date and time functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libgzipf-20240103/aclocal.m4` & `libgzipf-20240422/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libgzipf-20240103/configure.ac` & `libgzipf-20240422/configure.ac`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libgzipf],
- [20240103],
+ [20240422],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libgzipf.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```


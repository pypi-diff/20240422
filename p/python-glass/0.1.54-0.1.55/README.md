# Comparing `tmp/python_glass-0.1.54.tar.gz` & `tmp/python_glass-0.1.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_glass-0.1.54.tar", last modified: Sun Mar  3 04:38:06 2024, max compression
+gzip compressed data, was "python_glass-0.1.55.tar", last modified: Mon Apr 22 03:49:48 2024, max compression
```

## Comparing `python_glass-0.1.54.tar` & `python_glass-0.1.55.tar`

### file list

```diff
@@ -1,121 +1,117 @@
-drwxrwxrwx   0        0        0        0 2024-03-03 04:38:06.335517 python_glass-0.1.54/
--rw-rw-rw-   0        0        0     1119 2024-02-29 03:02:51.000000 python_glass-0.1.54/LICENSE
--rw-rw-rw-   0        0        0       95 2024-03-03 04:38:05.000000 python_glass-0.1.54/MANIFEST.in
--rw-rw-rw-   0        0        0     3848 2024-03-03 04:38:06.333512 python_glass-0.1.54/PKG-INFO
--rw-rw-rw-   0        0        0     3322 2024-03-03 04:38:05.000000 python_glass-0.1.54/README.rst
-drwxrwxrwx   0        0        0        0 2024-03-03 04:38:06.258336 python_glass-0.1.54/glass/
--rw-rw-rw-   0        0        0     1833 2024-02-05 01:28:36.000000 python_glass-0.1.54/glass/ACBO.py
--rw-rw-rw-   0        0        0     4481 2024-02-29 01:20:56.000000 python_glass-0.1.54/glass/AttrList.py
--rw-rw-rw-   0        0        0    12541 2024-02-05 01:28:38.000000 python_glass-0.1.54/glass/BO.py
--rw-rw-rw-   0        0        0     7125 2024-02-17 05:21:41.000000 python_glass-0.1.54/glass/Block.py
--rw-rw-rw-   0        0        0     4143 2024-02-05 01:28:40.000000 python_glass-0.1.54/glass/CSRMat.py
--rw-rw-rw-   0        0        0     6625 2024-02-05 01:28:39.000000 python_glass-0.1.54/glass/ComputeProgram.py
--rw-rw-rw-   0        0        0    12647 2024-03-03 01:09:55.000000 python_glass-0.1.54/glass/DictList.py
--rw-rw-rw-   0        0        0      410 2024-02-05 01:28:41.000000 python_glass-0.1.54/glass/EBO.py
--rw-rw-rw-   0        0        0    36924 2024-02-05 01:28:42.000000 python_glass-0.1.54/glass/FBO.py
--rw-rw-rw-   0        0        0     3702 2024-02-05 01:28:42.000000 python_glass-0.1.54/glass/FBOAttachment.py
--rw-rw-rw-   0        0        0    25316 2024-02-28 14:34:33.000000 python_glass-0.1.54/glass/GLConfig.py
--rw-rw-rw-   0        0        0    36365 2024-02-29 01:38:55.000000 python_glass-0.1.54/glass/GLInfo.py
--rw-rw-rw-   0        0        0     4017 2024-02-05 01:28:45.000000 python_glass-0.1.54/glass/GLObject.py
--rw-rw-rw-   0        0        0    20193 2024-02-17 13:23:42.000000 python_glass-0.1.54/glass/GPUProgram.py
--rw-rw-rw-   0        0        0     1546 2024-02-16 23:00:33.000000 python_glass-0.1.54/glass/GlassConfig.py
--rw-rw-rw-   0        0        0     3967 2024-02-05 01:28:48.000000 python_glass-0.1.54/glass/ImageLoader.py
--rw-rw-rw-   0        0        0     1669 2024-02-05 01:28:48.000000 python_glass-0.1.54/glass/ImageUnits.py
--rw-rw-rw-   0        0        0     5181 2024-02-05 01:28:49.000000 python_glass-0.1.54/glass/Increment.py
--rw-rw-rw-   0        0        0     4798 2024-02-05 01:28:49.000000 python_glass-0.1.54/glass/Indices.py
--rw-rw-rw-   0        0        0     4527 2024-02-05 01:28:50.000000 python_glass-0.1.54/glass/Instances.py
--rw-rw-rw-   0        0        0     1119 2024-02-29 03:03:55.000000 python_glass-0.1.54/glass/LICENSE
--rw-rw-rw-   0        0        0     1197 2024-02-16 23:01:49.000000 python_glass-0.1.54/glass/MetaInstancesRecorder.py
--rw-rw-rw-   0        0        0     3335 2024-02-05 01:28:53.000000 python_glass-0.1.54/glass/RBO.py
--rw-rw-rw-   0        0        0     3118 2024-02-02 09:20:44.000000 python_glass-0.1.54/glass/README_PYPI.md
--rw-rw-rw-   0        0        0     1568 2024-02-05 01:28:53.000000 python_glass-0.1.54/glass/RenderHints.py
--rw-rw-rw-   0        0        0     3121 2024-02-05 01:29:31.000000 python_glass-0.1.54/glass/SSBO.py
--rw-rw-rw-   0        0        0    32440 2024-02-17 05:21:42.000000 python_glass-0.1.54/glass/SSUBO.py
--rw-rw-rw-   0        0        0    12019 2024-02-05 01:28:54.000000 python_glass-0.1.54/glass/SameTypeList.py
--rw-rw-rw-   0        0        0    23905 2024-02-23 03:54:15.000000 python_glass-0.1.54/glass/ShaderParser.py
-drwxrwxrwx   0        0        0        0 2024-03-03 04:38:06.266337 python_glass-0.1.54/glass/ShaderParser_/
--rw-rw-rw-   0        0        0   599097 2024-02-28 14:34:50.000000 python_glass-0.1.54/glass/ShaderParser_/ShaderBuiltins.py
--rw-rw-rw-   0        0        0    34970 2024-03-03 03:27:05.000000 python_glass-0.1.54/glass/ShaderParser_/ShaderParser_.py
--rw-rw-rw-   0        0        0     6832 2024-03-03 01:10:22.000000 python_glass-0.1.54/glass/ShaderParser_/ShaderSyntaxTokens.py
--rw-rw-rw-   0        0        0       41 2024-02-28 14:34:32.000000 python_glass-0.1.54/glass/ShaderParser_/__init__.py
--rw-rw-rw-   0        0        0    12982 2024-02-28 14:34:33.000000 python_glass-0.1.54/glass/ShaderParser_/generate_code.py
--rw-rw-rw-   0        0        0     6577 2024-02-28 14:34:32.000000 python_glass-0.1.54/glass/ShaderParser_/minifyc.py
-drwxrwxrwx   0        0        0        0 2024-03-03 04:38:06.275340 python_glass-0.1.54/glass/ShaderParser_/pcpp/
--rw-rw-rw-   0        0        0     1579 2024-02-17 04:03:25.000000 python_glass-0.1.54/glass/ShaderParser_/pcpp/LICENSE
--rw-rw-rw-   0        0        0      194 2024-02-05 01:29:30.000000 python_glass-0.1.54/glass/ShaderParser_/pcpp/__init__.py
--rw-rw-rw-   0        0        0    28226 2024-02-16 23:03:33.000000 python_glass-0.1.54/glass/ShaderParser_/pcpp/evaluator.py
--rw-rw-rw-   0        0        0     6599 2024-02-05 01:29:30.000000 python_glass-0.1.54/glass/ShaderParser_/pcpp/lextab.py
--rw-rw-rw-   0        0        0    15216 2024-02-16 23:04:12.000000 python_glass-0.1.54/glass/ShaderParser_/pcpp/parser.py
--rw-rw-rw-   0        0        0    49465 2024-02-05 01:29:32.000000 python_glass-0.1.54/glass/ShaderParser_/pcpp/parsetab.py
--rw-rw-rw-   0        0        0    18778 2024-02-05 01:29:32.000000 python_glass-0.1.54/glass/ShaderParser_/pcpp/pcmd.py
-drwxrwxrwx   0        0        0        0 2024-03-03 04:38:06.282515 python_glass-0.1.54/glass/ShaderParser_/pcpp/ply/
--rw-rw-rw-   0        0        0      109 2024-02-05 01:29:30.000000 python_glass-0.1.54/glass/ShaderParser_/pcpp/ply/__init__.py
--rw-rw-rw-   0        0        0    39408 2024-02-16 23:04:38.000000 python_glass-0.1.54/glass/ShaderParser_/pcpp/ply/cpp.py
--rw-rw-rw-   0        0        0     2988 2024-02-05 01:29:31.000000 python_glass-0.1.54/glass/ShaderParser_/pcpp/ply/ctokens.py
--rw-rw-rw-   0        0        0    46412 2024-02-05 01:29:32.000000 python_glass-0.1.54/glass/ShaderParser_/pcpp/ply/lex.py
--rw-rw-rw-   0        0        0   144595 2024-02-16 23:05:08.000000 python_glass-0.1.54/glass/ShaderParser_/pcpp/ply/yacc.py
--rw-rw-rw-   0        0        0     2341 2024-02-05 01:29:31.000000 python_glass-0.1.54/glass/ShaderParser_/pcpp/ply/ygen.py
--rw-rw-rw-   0        0        0    73751 2024-02-16 23:04:28.000000 python_glass-0.1.54/glass/ShaderParser_/pcpp/preprocessor.py
-drwxrwxrwx   0        0        0        0 2024-03-03 04:38:06.285102 python_glass-0.1.54/glass/ShaderParser_/tree-sitter-glsl/
--rw-rw-rw-   0        0        0      549 2021-09-28 16:35:06.000000 python_glass-0.1.54/glass/ShaderParser_/tree-sitter-glsl/README.md
-drwxrwxrwx   0        0        0        0 2024-03-03 04:38:06.180363 python_glass-0.1.54/glass/ShaderParser_/tree-sitter-glsl/lib/
-drwxrwxrwx   0        0        0        0 2024-03-03 04:38:06.180363 python_glass-0.1.54/glass/ShaderParser_/tree-sitter-glsl/lib/AMD64/
-drwxrwxrwx   0        0        0        0 2024-03-03 04:38:06.180363 python_glass-0.1.54/glass/ShaderParser_/tree-sitter-glsl/lib/AMD64/Windows/
-drwxrwxrwx   0        0        0        0 2024-03-03 04:38:06.286236 python_glass-0.1.54/glass/ShaderParser_/tree-sitter-glsl/lib/AMD64/Windows/32bit/
--rw-rw-rw-   0        0        0   140800 2024-03-03 03:03:13.000000 python_glass-0.1.54/glass/ShaderParser_/tree-sitter-glsl/lib/AMD64/Windows/32bit/glsl.dll
-drwxrwxrwx   0        0        0        0 2024-03-03 04:38:06.288487 python_glass-0.1.54/glass/ShaderParser_/tree-sitter-glsl/lib/AMD64/Windows/64bit/
--rw-rw-rw-   0        0        0   139776 2024-02-29 02:40:31.000000 python_glass-0.1.54/glass/ShaderParser_/tree-sitter-glsl/lib/AMD64/Windows/64bit/glsl.dll
-drwxrwxrwx   0        0        0        0 2024-03-03 04:38:06.180363 python_glass-0.1.54/glass/ShaderParser_/tree-sitter-glsl/lib/x86_64/
-drwxrwxrwx   0        0        0        0 2024-03-03 04:38:06.181771 python_glass-0.1.54/glass/ShaderParser_/tree-sitter-glsl/lib/x86_64/Linux/
-drwxrwxrwx   0        0        0        0 2024-03-03 04:38:06.289827 python_glass-0.1.54/glass/ShaderParser_/tree-sitter-glsl/lib/x86_64/Linux/64bit/
--rw-rw-rw-   0        0        0   151120 2024-03-03 04:13:39.000000 python_glass-0.1.54/glass/ShaderParser_/tree-sitter-glsl/lib/x86_64/Linux/64bit/glsl.so
-drwxrwxrwx   0        0        0        0 2024-03-03 04:38:06.291769 python_glass-0.1.54/glass/ShaderParser_/tree-sitter-glsl/src/
--rw-rw-rw-   0        0        0  1084386 2024-03-03 03:03:06.000000 python_glass-0.1.54/glass/ShaderParser_/tree-sitter-glsl/src/parser.c
-drwxrwxrwx   0        0        0        0 2024-03-03 04:38:06.295843 python_glass-0.1.54/glass/ShaderParser_/tree-sitter-glsl/src/tree_sitter/
--rw-rw-rw-   0        0        0     5340 2024-03-03 03:03:06.000000 python_glass-0.1.54/glass/ShaderParser_/tree-sitter-glsl/src/tree_sitter/parser.h
--rw-rw-rw-   0        0        0    70455 2024-02-29 02:35:32.000000 python_glass-0.1.54/glass/ShaderParser_/tree-sitter-glsl/src.zip
--rw-rw-rw-   0        0        0    39818 2024-02-28 14:34:33.000000 python_glass-0.1.54/glass/ShaderProgram.py
--rw-rw-rw-   0        0        0      180 2024-02-17 05:21:41.000000 python_glass-0.1.54/glass/ShaderStorageBlock.py
--rw-rw-rw-   0        0        0    23787 2024-03-03 02:11:44.000000 python_glass-0.1.54/glass/Shaders.py
--rw-rw-rw-   0        0        0     8610 2024-02-29 03:40:22.000000 python_glass-0.1.54/glass/TextLoader.py
--rw-rw-rw-   0        0        0     1970 2024-02-05 01:29:31.000000 python_glass-0.1.54/glass/TextureUnits.py
--rw-rw-rw-   0        0        0      471 2024-02-05 01:29:31.000000 python_glass-0.1.54/glass/UBO.py
--rw-rw-rw-   0        0        0    24157 2024-02-05 01:29:32.000000 python_glass-0.1.54/glass/Uniform.py
--rw-rw-rw-   0        0        0      185 2024-02-17 03:45:39.000000 python_glass-0.1.54/glass/UniformBlock.py
--rw-rw-rw-   0        0        0     4658 2024-02-28 14:26:22.000000 python_glass-0.1.54/glass/VAO.py
--rw-rw-rw-   0        0        0      423 2024-02-05 01:29:31.000000 python_glass-0.1.54/glass/VBO.py
--rw-rw-rw-   0        0        0    18042 2024-02-29 01:21:22.000000 python_glass-0.1.54/glass/Vertices.py
--rw-rw-rw-   0        0        0     3015 2024-02-05 01:29:31.000000 python_glass-0.1.54/glass/WeakDict.py
--rw-rw-rw-   0        0        0     2000 2024-03-03 01:10:10.000000 python_glass-0.1.54/glass/WeakList.py
--rw-rw-rw-   0        0        0      969 2024-03-03 01:10:14.000000 python_glass-0.1.54/glass/WeakRef.py
--rw-rw-rw-   0        0        0     2269 2024-02-05 01:29:31.000000 python_glass-0.1.54/glass/WeakSet.py
--rw-rw-rw-   0        0        0     1246 2024-03-03 02:31:48.000000 python_glass-0.1.54/glass/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-03 04:38:06.298444 python_glass-0.1.54/glass/__pyinstaller/
--rw-rw-rw-   0        0        0      113 2024-02-05 01:29:30.000000 python_glass-0.1.54/glass/__pyinstaller/__init__.py
--rw-rw-rw-   0        0        0     1431 2024-02-29 02:51:04.000000 python_glass-0.1.54/glass/__pyinstaller/hook-glass.py
--rw-rw-rw-   0        0        0     2718 2024-03-03 01:16:02.000000 python_glass-0.1.54/glass/download.py
-drwxrwxrwx   0        0        0        0 2024-03-03 04:38:06.301583 python_glass-0.1.54/glass/glsl/
--rw-rw-rw-   0        0        0      729 2024-02-02 07:40:56.000000 python_glass-0.1.54/glass/glsl/draw_frame.vs
--rw-rw-rw-   0        0        0      905 2024-02-02 07:40:56.000000 python_glass-0.1.54/glass/glsl/shadertoy_template.fs
--rw-rw-rw-   0        0        0     8019 2024-02-29 01:52:35.000000 python_glass-0.1.54/glass/helper.py
--rw-rw-rw-   0        0        0     1835 2024-02-05 01:28:47.000000 python_glass-0.1.54/glass/iimage2D.py
--rw-rw-rw-   0        0        0     1836 2024-02-05 01:28:48.000000 python_glass-0.1.54/glass/image2D.py
--rw-rw-rw-   0        0        0     1519 2024-02-05 01:28:51.000000 python_glass-0.1.54/glass/isampler2D.py
--rw-rw-rw-   0        0        0     1378 2024-02-05 01:28:51.000000 python_glass-0.1.54/glass/isampler2DMS.py
--rw-rw-rw-   0        0        0    20380 2024-02-17 14:14:40.000000 python_glass-0.1.54/glass/sampler2D.py
--rw-rw-rw-   0        0        0    17721 2024-02-05 01:29:31.000000 python_glass-0.1.54/glass/sampler2DArray.py
--rw-rw-rw-   0        0        0     4126 2024-02-05 01:29:30.000000 python_glass-0.1.54/glass/sampler2DMS.py
--rw-rw-rw-   0        0        0    15723 2024-02-05 01:29:31.000000 python_glass-0.1.54/glass/samplerCube.py
--rw-rw-rw-   0        0        0     1836 2024-02-05 01:29:31.000000 python_glass-0.1.54/glass/uimage2D.py
--rw-rw-rw-   0        0        0     1519 2024-02-05 01:29:31.000000 python_glass-0.1.54/glass/usampler2D.py
--rw-rw-rw-   0        0        0     1379 2024-02-05 01:29:31.000000 python_glass-0.1.54/glass/usampler2DMS.py
--rw-rw-rw-   0        0        0    23220 2024-03-03 01:57:21.000000 python_glass-0.1.54/glass/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-03 04:38:06.332183 python_glass-0.1.54/python_glass.egg-info/
--rw-rw-rw-   0        0        0     3848 2024-03-03 04:38:05.000000 python_glass-0.1.54/python_glass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2619 2024-03-03 04:38:06.000000 python_glass-0.1.54/python_glass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-03 04:38:05.000000 python_glass-0.1.54/python_glass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-03-03 04:38:05.000000 python_glass-0.1.54/python_glass.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      100 2024-03-03 04:38:05.000000 python_glass-0.1.54/python_glass.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-03 04:38:05.000000 python_glass-0.1.54/python_glass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-03 04:38:06.335517 python_glass-0.1.54/setup.cfg
--rw-rw-rw-   0        0        0     1890 2024-03-03 04:38:05.000000 python_glass-0.1.54/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:49:48.702266 python_glass-0.1.55/
+-rw-rw-rw-   0        0        0     1119 2024-02-29 03:02:51.000000 python_glass-0.1.55/LICENSE
+-rw-rw-rw-   0        0        0       95 2024-04-22 03:49:46.000000 python_glass-0.1.55/MANIFEST.in
+-rw-rw-rw-   0        0        0     3848 2024-04-22 03:49:48.701264 python_glass-0.1.55/PKG-INFO
+-rw-rw-rw-   0        0        0     3322 2024-04-22 03:49:46.000000 python_glass-0.1.55/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-22 03:49:48.595283 python_glass-0.1.55/glass/
+-rw-rw-rw-   0        0        0     1833 2024-04-19 06:46:58.000000 python_glass-0.1.55/glass/ACBO.py
+-rw-rw-rw-   0        0        0     4481 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/AttrList.py
+-rw-rw-rw-   0        0        0    12541 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/BO.py
+-rw-rw-rw-   0        0        0     7125 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/Block.py
+-rw-rw-rw-   0        0        0     4143 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/CSRMat.py
+-rw-rw-rw-   0        0        0     6625 2024-04-19 06:47:40.000000 python_glass-0.1.55/glass/ComputeProgram.py
+-rw-rw-rw-   0        0        0    12639 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/DictList.py
+-rw-rw-rw-   0        0        0      410 2024-04-19 06:47:48.000000 python_glass-0.1.55/glass/EBO.py
+-rw-rw-rw-   0        0        0    36924 2024-04-19 06:56:41.000000 python_glass-0.1.55/glass/FBO.py
+-rw-rw-rw-   0        0        0     3702 2024-02-05 01:28:42.000000 python_glass-0.1.55/glass/FBOAttachment.py
+-rw-rw-rw-   0        0        0    25316 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/GLConfig.py
+-rw-rw-rw-   0        0        0    36365 2024-04-19 06:46:36.000000 python_glass-0.1.55/glass/GLInfo.py
+-rw-rw-rw-   0        0        0     4017 2024-04-19 06:48:28.000000 python_glass-0.1.55/glass/GLObject.py
+-rw-rw-rw-   0        0        0    19837 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/GPUProgram.py
+-rw-rw-rw-   0        0        0     1546 2024-02-16 23:00:33.000000 python_glass-0.1.55/glass/GlassConfig.py
+-rw-rw-rw-   0        0        0     3967 2024-02-05 01:28:48.000000 python_glass-0.1.55/glass/ImageLoader.py
+-rw-rw-rw-   0        0        0     1669 2024-02-05 01:28:48.000000 python_glass-0.1.55/glass/ImageUnits.py
+-rw-rw-rw-   0        0        0     5181 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/Increment.py
+-rw-rw-rw-   0        0        0     4798 2024-04-19 06:49:14.000000 python_glass-0.1.55/glass/Indices.py
+-rw-rw-rw-   0        0        0     4527 2024-04-19 06:49:34.000000 python_glass-0.1.55/glass/Instances.py
+-rw-rw-rw-   0        0        0     1119 2024-02-29 03:03:55.000000 python_glass-0.1.55/glass/LICENSE
+-rw-rw-rw-   0        0        0     1197 2024-02-16 23:01:49.000000 python_glass-0.1.55/glass/MetaInstancesRecorder.py
+-rw-rw-rw-   0        0        0     3335 2024-04-19 06:50:01.000000 python_glass-0.1.55/glass/RBO.py
+-rw-rw-rw-   0        0        0     3118 2024-02-02 09:20:44.000000 python_glass-0.1.55/glass/README_PYPI.md
+-rw-rw-rw-   0        0        0     1568 2024-02-05 01:28:53.000000 python_glass-0.1.55/glass/RenderHints.py
+-rw-rw-rw-   0        0        0     3121 2024-04-19 06:51:09.000000 python_glass-0.1.55/glass/SSBO.py
+-rw-rw-rw-   0        0        0    32440 2024-04-19 06:51:20.000000 python_glass-0.1.55/glass/SSUBO.py
+-rw-rw-rw-   0        0        0    12019 2024-02-05 01:28:54.000000 python_glass-0.1.55/glass/SameTypeList.py
+-rw-rw-rw-   0        0        0    23907 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderParser.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:49:48.604284 python_glass-0.1.55/glass/ShaderParser_/
+-rw-rw-rw-   0        0        0   581459 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderParser_/ShaderBuiltins.py
+-rw-rw-rw-   0        0        0    34819 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderParser_/ShaderParser_.py
+-rw-rw-rw-   0        0        0     6828 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderParser_/ShaderSyntaxTokens.py
+-rw-rw-rw-   0        0        0       42 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderParser_/__init__.py
+-rw-rw-rw-   0        0        0    12921 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderParser_/generate_code.py
+-rw-rw-rw-   0        0        0     6565 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderParser_/minifyc.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:49:48.616701 python_glass-0.1.55/glass/ShaderParser_/pcpp/
+-rw-rw-rw-   0        0        0     1579 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderParser_/pcpp/LICENSE
+-rw-rw-rw-   0        0        0      194 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderParser_/pcpp/__init__.py
+-rw-rw-rw-   0        0        0    28226 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderParser_/pcpp/evaluator.py
+-rw-rw-rw-   0        0        0     6599 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderParser_/pcpp/lextab.py
+-rw-rw-rw-   0        0        0    15216 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderParser_/pcpp/parser.py
+-rw-rw-rw-   0        0        0    49465 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderParser_/pcpp/parsetab.py
+-rw-rw-rw-   0        0        0    18778 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderParser_/pcpp/pcmd.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:49:48.631710 python_glass-0.1.55/glass/ShaderParser_/pcpp/ply/
+-rw-rw-rw-   0        0        0      109 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderParser_/pcpp/ply/__init__.py
+-rw-rw-rw-   0        0        0    39408 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderParser_/pcpp/ply/cpp.py
+-rw-rw-rw-   0        0        0     2988 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderParser_/pcpp/ply/ctokens.py
+-rw-rw-rw-   0        0        0    46412 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderParser_/pcpp/ply/lex.py
+-rw-rw-rw-   0        0        0   144595 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderParser_/pcpp/ply/yacc.py
+-rw-rw-rw-   0        0        0     2341 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderParser_/pcpp/ply/ygen.py
+-rw-rw-rw-   0        0        0    73751 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderParser_/pcpp/preprocessor.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:49:48.635711 python_glass-0.1.55/glass/ShaderParser_/tree-sitter-glsl/
+-rw-rw-rw-   0        0        0      564 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderParser_/tree-sitter-glsl/README.md
+drwxrwxrwx   0        0        0        0 2024-04-22 03:49:48.489699 python_glass-0.1.55/glass/ShaderParser_/tree-sitter-glsl/lib/
+drwxrwxrwx   0        0        0        0 2024-04-22 03:49:48.488467 python_glass-0.1.55/glass/ShaderParser_/tree-sitter-glsl/lib/AMD64/
+drwxrwxrwx   0        0        0        0 2024-04-22 03:49:48.489699 python_glass-0.1.55/glass/ShaderParser_/tree-sitter-glsl/lib/AMD64/Windows/
+drwxrwxrwx   0        0        0        0 2024-04-22 03:49:48.637711 python_glass-0.1.55/glass/ShaderParser_/tree-sitter-glsl/lib/AMD64/Windows/32bit/
+-rw-rw-rw-   0        0        0   140800 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderParser_/tree-sitter-glsl/lib/AMD64/Windows/32bit/glsl.dll
+drwxrwxrwx   0        0        0        0 2024-04-22 03:49:48.643712 python_glass-0.1.55/glass/ShaderParser_/tree-sitter-glsl/lib/AMD64/Windows/64bit/
+-rw-rw-rw-   0        0        0   139776 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderParser_/tree-sitter-glsl/lib/AMD64/Windows/64bit/glsl.dll
+drwxrwxrwx   0        0        0        0 2024-04-22 03:49:48.489699 python_glass-0.1.55/glass/ShaderParser_/tree-sitter-glsl/lib/x86_64/
+drwxrwxrwx   0        0        0        0 2024-04-22 03:49:48.489699 python_glass-0.1.55/glass/ShaderParser_/tree-sitter-glsl/lib/x86_64/Linux/
+drwxrwxrwx   0        0        0        0 2024-04-22 03:49:48.646713 python_glass-0.1.55/glass/ShaderParser_/tree-sitter-glsl/lib/x86_64/Linux/64bit/
+-rw-rw-rw-   0        0        0   151120 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderParser_/tree-sitter-glsl/lib/x86_64/Linux/64bit/glsl.so
+-rw-rw-rw-   0        0        0    70455 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderParser_/tree-sitter-glsl/src.zip
+-rw-rw-rw-   0        0        0    39877 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/ShaderProgram.py
+-rw-rw-rw-   0        0        0      180 2024-02-17 05:21:41.000000 python_glass-0.1.55/glass/ShaderStorageBlock.py
+-rw-rw-rw-   0        0        0    23905 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/Shaders.py
+-rw-rw-rw-   0        0        0     8610 2024-02-29 03:40:22.000000 python_glass-0.1.55/glass/TextLoader.py
+-rw-rw-rw-   0        0        0     1970 2024-02-05 01:29:31.000000 python_glass-0.1.55/glass/TextureUnits.py
+-rw-rw-rw-   0        0        0      471 2024-04-19 06:51:32.000000 python_glass-0.1.55/glass/UBO.py
+-rw-rw-rw-   0        0        0    24157 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/Uniform.py
+-rw-rw-rw-   0        0        0      185 2024-02-17 03:45:39.000000 python_glass-0.1.55/glass/UniformBlock.py
+-rw-rw-rw-   0        0        0     4658 2024-04-19 06:52:26.000000 python_glass-0.1.55/glass/VAO.py
+-rw-rw-rw-   0        0        0      423 2024-04-19 06:52:32.000000 python_glass-0.1.55/glass/VBO.py
+-rw-rw-rw-   0        0        0    18042 2024-04-19 06:58:11.000000 python_glass-0.1.55/glass/Vertices.py
+-rw-rw-rw-   0        0        0     3015 2024-02-05 01:29:31.000000 python_glass-0.1.55/glass/WeakDict.py
+-rw-rw-rw-   0        0        0     2000 2024-03-03 01:10:10.000000 python_glass-0.1.55/glass/WeakList.py
+-rw-rw-rw-   0        0        0      969 2024-03-03 01:10:14.000000 python_glass-0.1.55/glass/WeakRef.py
+-rw-rw-rw-   0        0        0     2269 2024-02-05 01:29:31.000000 python_glass-0.1.55/glass/WeakSet.py
+-rw-rw-rw-   0        0        0     1248 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:49:48.650597 python_glass-0.1.55/glass/__pyinstaller/
+-rw-rw-rw-   0        0        0      113 2024-02-05 01:29:30.000000 python_glass-0.1.55/glass/__pyinstaller/__init__.py
+-rw-rw-rw-   0        0        0     1422 2024-04-22 03:18:34.000000 python_glass-0.1.55/glass/__pyinstaller/hook-glass.py
+-rw-rw-rw-   0        0        0     2781 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/download.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:49:48.668187 python_glass-0.1.55/glass/glsl/
+-rw-rw-rw-   0        0        0      729 2024-02-02 07:40:56.000000 python_glass-0.1.55/glass/glsl/draw_frame.vs
+-rw-rw-rw-   0        0        0      905 2024-02-02 07:40:56.000000 python_glass-0.1.55/glass/glsl/shadertoy_template.fs
+-rw-rw-rw-   0        0        0     7996 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/helper.py
+-rw-rw-rw-   0        0        0     1835 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/iimage2D.py
+-rw-rw-rw-   0        0        0     1836 2024-04-19 06:58:22.000000 python_glass-0.1.55/glass/image2D.py
+-rw-rw-rw-   0        0        0     1519 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/isampler2D.py
+-rw-rw-rw-   0        0        0     1378 2024-04-19 06:49:53.000000 python_glass-0.1.55/glass/isampler2DMS.py
+-rw-rw-rw-   0        0        0    20380 2024-04-19 06:50:07.000000 python_glass-0.1.55/glass/sampler2D.py
+-rw-rw-rw-   0        0        0    17721 2024-04-19 06:50:15.000000 python_glass-0.1.55/glass/sampler2DArray.py
+-rw-rw-rw-   0        0        0     4126 2024-04-19 06:50:26.000000 python_glass-0.1.55/glass/sampler2DMS.py
+-rw-rw-rw-   0        0        0    15723 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/samplerCube.py
+-rw-rw-rw-   0        0        0     1836 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/uimage2D.py
+-rw-rw-rw-   0        0        0     1519 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/usampler2D.py
+-rw-rw-rw-   0        0        0     1379 2024-04-19 06:52:20.000000 python_glass-0.1.55/glass/usampler2DMS.py
+-rw-rw-rw-   0        0        0    23220 2024-04-22 03:16:08.000000 python_glass-0.1.55/glass/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-22 03:49:48.700076 python_glass-0.1.55/python_glass.egg-info/
+-rw-rw-rw-   0        0        0     3848 2024-04-22 03:49:48.000000 python_glass-0.1.55/python_glass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2507 2024-04-22 03:49:48.000000 python_glass-0.1.55/python_glass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 03:49:48.000000 python_glass-0.1.55/python_glass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-22 03:49:48.000000 python_glass-0.1.55/python_glass.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      100 2024-04-22 03:49:48.000000 python_glass-0.1.55/python_glass.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-22 03:49:48.000000 python_glass-0.1.55/python_glass.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-22 03:49:48.702266 python_glass-0.1.55/setup.cfg
+-rw-rw-rw-   0        0        0     1890 2024-04-22 03:49:46.000000 python_glass-0.1.55/setup.py
```

### Comparing `python_glass-0.1.54/LICENSE` & `python_glass-0.1.55/LICENSE`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/PKG-INFO` & `python_glass-0.1.55/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_glass
-Version: 0.1.54
+Version: 0.1.55
 Summary: OpenGL wrapper for Glass-Engine
 Home-page: https://github.com/Time-Coder/Glass-Engine
 Author: 王炳辉 (BingHui-WANG)
 Author-email: binghui.wang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python_glass-0.1.54/README.rst` & `python_glass-0.1.55/README.rst`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/ACBO.py` & `python_glass-0.1.55/glass/ACBO.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/AttrList.py` & `python_glass-0.1.55/glass/AttrList.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/BO.py` & `python_glass-0.1.55/glass/BO.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/Block.py` & `python_glass-0.1.55/glass/Block.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/CSRMat.py` & `python_glass-0.1.55/glass/CSRMat.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/ComputeProgram.py` & `python_glass-0.1.55/glass/ComputeProgram.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/DictList.py` & `python_glass-0.1.55/glass/DictList.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 
 
 class ExtendableList:
 
     def __init__(
         self,
         weak_ref: bool = True,
-        before_item_add_callback = None,
-        before_item_remove_callback = None,
-        after_item_add_callback = None,
-        after_item_remove_callback = None,
+        before_item_add_callback=None,
+        before_item_remove_callback=None,
+        after_item_add_callback=None,
+        after_item_remove_callback=None,
     ) -> None:
         if weak_ref:
             self._list: Union[List[Any], WeakList] = WeakList()
         else:
             self._list: Union[List[Any], WeakList] = []
 
         self.before_item_add_callback: Union[
```

### Comparing `python_glass-0.1.54/glass/FBO.py` & `python_glass-0.1.55/glass/FBO.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/FBOAttachment.py` & `python_glass-0.1.55/glass/FBOAttachment.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/GLConfig.py` & `python_glass-0.1.55/glass/GLConfig.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/GLInfo.py` & `python_glass-0.1.55/glass/GLInfo.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/GLObject.py` & `python_glass-0.1.55/glass/GLObject.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/GPUProgram.py` & `python_glass-0.1.55/glass/GPUProgram.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import numpy as np
 import re
 from ctypes import c_int, pointer
 
 from .GLObject import GLObject
 from .GLInfo import GLInfo
 from .GlassConfig import GlassConfig
-from .GLConfig import GLConfig
 from .Uniform import Uniform
 from .UniformBlock import UniformBlock
 from .ShaderStorageBlock import ShaderStorageBlock
 from .ShaderParser import ShaderParser
 from .utils import LP_LP_c_char, delete, checktype
 
 _target_type_map = {
@@ -66,15 +65,14 @@
     )
     __message_prefix2 = re.compile(
         r"(?P<shader_type>\w+) info\n-{4,}\n(?P<message_type>\w+): "
     )
     __message_prefix3 = re.compile(
         r"\n0?\((?P<line_number>\d+)\) : (?P<message_type>\w+) "
     )
-    __active_program = {}
 
     def __init__(self):
         GLObject.__init__(self)
 
         self._attributes_info = {}
         self._acceptable_primitives = []
         self._uniforms_info = {}
@@ -183,21 +181,15 @@
     def collect_info(self):
         pass
 
     def use(self):
         self.collect_info()
         self._link()
 
-        current_context = GLConfig.buffered_current_context
-        if (
-            current_context not in GPUProgram.__active_program
-            or GPUProgram.__active_program[current_context] != self._id
-        ):
-            GL.glUseProgram(self._id)
-            GPUProgram.__active_program[current_context] = self._id
+        GL.glUseProgram(self._id)
 
     def stop_using(self):
         if not self.is_using:
             return
 
         GL.glUseProgram(0)
```

### Comparing `python_glass-0.1.54/glass/GlassConfig.py` & `python_glass-0.1.55/glass/GlassConfig.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/ImageLoader.py` & `python_glass-0.1.55/glass/ImageLoader.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/ImageUnits.py` & `python_glass-0.1.55/glass/ImageUnits.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/Increment.py` & `python_glass-0.1.55/glass/Increment.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/Indices.py` & `python_glass-0.1.55/glass/Indices.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/Instances.py` & `python_glass-0.1.55/glass/Instances.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/LICENSE` & `python_glass-0.1.55/glass/LICENSE`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/MetaInstancesRecorder.py` & `python_glass-0.1.55/glass/MetaInstancesRecorder.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/RBO.py` & `python_glass-0.1.55/glass/RBO.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/README_PYPI.md` & `python_glass-0.1.55/glass/README_PYPI.md`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/RenderHints.py` & `python_glass-0.1.55/glass/RenderHints.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/SSBO.py` & `python_glass-0.1.55/glass/SSBO.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/SSUBO.py` & `python_glass-0.1.55/glass/SSUBO.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/SameTypeList.py` & `python_glass-0.1.55/glass/SameTypeList.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/ShaderParser.py` & `python_glass-0.1.55/glass/ShaderParser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 from OpenGL import GL
+
 from .utils import has_valid
 from .helper import sizeof, type_from_str
 from .GLInfo import GLInfo
 
 
 class ShaderParser:
```

### Comparing `python_glass-0.1.54/glass/ShaderParser_/ShaderBuiltins.py` & `python_glass-0.1.55/glass/ShaderParser_/ShaderBuiltins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1116,23 +1116,14 @@
             name="clamp",
             args=[
                 Var(name="x", type="vec4"),
                 Var(name="minVal", type="vec4"),
                 Var(name="maxVal", type="vec4"),
             ],
         ),
-        "clamp(float, float, float)": Func(
-            return_type="float",
-            name="clamp",
-            args=[
-                Var(name="x", type="float"),
-                Var(name="minVal", type="float"),
-                Var(name="maxVal", type="float"),
-            ],
-        ),
         "clamp(vec2, float, float)": Func(
             return_type="vec2",
             name="clamp",
             args=[
                 Var(name="x", type="vec2"),
                 Var(name="minVal", type="float"),
                 Var(name="maxVal", type="float"),
@@ -1188,23 +1179,14 @@
             name="clamp",
             args=[
                 Var(name="x", type="dvec4"),
                 Var(name="minVal", type="dvec4"),
                 Var(name="maxVal", type="dvec4"),
             ],
         ),
-        "clamp(double, double, double)": Func(
-            return_type="double",
-            name="clamp",
-            args=[
-                Var(name="x", type="double"),
-                Var(name="minVal", type="double"),
-                Var(name="maxVal", type="double"),
-            ],
-        ),
         "clamp(dvec2, double, double)": Func(
             return_type="dvec2",
             name="clamp",
             args=[
                 Var(name="x", type="dvec2"),
                 Var(name="minVal", type="double"),
                 Var(name="maxVal", type="double"),
@@ -1260,23 +1242,14 @@
             name="clamp",
             args=[
                 Var(name="x", type="ivec4"),
                 Var(name="minVal", type="ivec4"),
                 Var(name="maxVal", type="ivec4"),
             ],
         ),
-        "clamp(int, int, int)": Func(
-            return_type="int",
-            name="clamp",
-            args=[
-                Var(name="x", type="int"),
-                Var(name="minVal", type="int"),
-                Var(name="maxVal", type="int"),
-            ],
-        ),
         "clamp(ivec2, int, int)": Func(
             return_type="ivec2",
             name="clamp",
             args=[
                 Var(name="x", type="ivec2"),
                 Var(name="minVal", type="int"),
                 Var(name="maxVal", type="int"),
@@ -1332,23 +1305,14 @@
             name="clamp",
             args=[
                 Var(name="x", type="uvec4"),
                 Var(name="minVal", type="uvec4"),
                 Var(name="maxVal", type="uvec4"),
             ],
         ),
-        "clamp(uint, uint, uint)": Func(
-            return_type="uint",
-            name="clamp",
-            args=[
-                Var(name="x", type="uint"),
-                Var(name="minVal", type="uint"),
-                Var(name="maxVal", type="uint"),
-            ],
-        ),
         "clamp(uvec2, uint, uint)": Func(
             return_type="uvec2",
             name="clamp",
             args=[
                 Var(name="x", type="uvec2"),
                 Var(name="minVal", type="uint"),
                 Var(name="maxVal", type="uint"),
@@ -2768,23 +2732,14 @@
             name="imageAtomicAdd",
             args=[
                 Var(name="image", type="iimage2DRect"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="uint"),
             ],
         ),
-        "imageAtomicAdd(iimage2DRect, ivec2, uint)": Func(
-            return_type="uint",
-            name="imageAtomicAdd",
-            args=[
-                Var(name="image", type="iimage2DRect"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="uint"),
-            ],
-        ),
         "imageAtomicAdd(imageCube, ivec3, uint)": Func(
             return_type="uint",
             name="imageAtomicAdd",
             args=[
                 Var(name="image", type="imageCube"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="uint"),
@@ -2849,23 +2804,14 @@
             name="imageAtomicAdd",
             args=[
                 Var(name="image", type="iimage1DArray"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="uint"),
             ],
         ),
-        "imageAtomicAdd(iimage1DArray, ivec2, uint)": Func(
-            return_type="uint",
-            name="imageAtomicAdd",
-            args=[
-                Var(name="image", type="iimage1DArray"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="uint"),
-            ],
-        ),
         "imageAtomicAdd(image2DArray, ivec3, uint)": Func(
             return_type="uint",
             name="imageAtomicAdd",
             args=[
                 Var(name="image", type="image2DArray"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="uint"),
@@ -3071,23 +3017,14 @@
             name="imageAtomicAdd",
             args=[
                 Var(name="image", type="iimage2DRect"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="int"),
             ],
         ),
-        "imageAtomicAdd(iimage2DRect, ivec2, int)": Func(
-            return_type="int",
-            name="imageAtomicAdd",
-            args=[
-                Var(name="image", type="iimage2DRect"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="int"),
-            ],
-        ),
         "imageAtomicAdd(imageCube, ivec3, int)": Func(
             return_type="int",
             name="imageAtomicAdd",
             args=[
                 Var(name="image", type="imageCube"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="int"),
@@ -3152,23 +3089,14 @@
             name="imageAtomicAdd",
             args=[
                 Var(name="image", type="iimage1DArray"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="int"),
             ],
         ),
-        "imageAtomicAdd(iimage1DArray, ivec2, int)": Func(
-            return_type="int",
-            name="imageAtomicAdd",
-            args=[
-                Var(name="image", type="iimage1DArray"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="int"),
-            ],
-        ),
         "imageAtomicAdd(image2DArray, ivec3, int)": Func(
             return_type="int",
             name="imageAtomicAdd",
             args=[
                 Var(name="image", type="image2DArray"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="int"),
@@ -3374,23 +3302,14 @@
             name="imageAtomicAnd",
             args=[
                 Var(name="image", type="iimage2DRect"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="uint"),
             ],
         ),
-        "imageAtomicAnd(iimage2DRect, ivec2, uint)": Func(
-            return_type="uint",
-            name="imageAtomicAnd",
-            args=[
-                Var(name="image", type="iimage2DRect"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="uint"),
-            ],
-        ),
         "imageAtomicAnd(imageCube, ivec3, uint)": Func(
             return_type="uint",
             name="imageAtomicAnd",
             args=[
                 Var(name="image", type="imageCube"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="uint"),
@@ -3455,23 +3374,14 @@
             name="imageAtomicAnd",
             args=[
                 Var(name="image", type="iimage1DArray"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="uint"),
             ],
         ),
-        "imageAtomicAnd(iimage1DArray, ivec2, uint)": Func(
-            return_type="uint",
-            name="imageAtomicAnd",
-            args=[
-                Var(name="image", type="iimage1DArray"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="uint"),
-            ],
-        ),
         "imageAtomicAnd(image2DArray, ivec3, uint)": Func(
             return_type="uint",
             name="imageAtomicAnd",
             args=[
                 Var(name="image", type="image2DArray"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="uint"),
@@ -3677,23 +3587,14 @@
             name="imageAtomicAnd",
             args=[
                 Var(name="image", type="iimage2DRect"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="int"),
             ],
         ),
-        "imageAtomicAnd(iimage2DRect, ivec2, int)": Func(
-            return_type="int",
-            name="imageAtomicAnd",
-            args=[
-                Var(name="image", type="iimage2DRect"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="int"),
-            ],
-        ),
         "imageAtomicAnd(imageCube, ivec3, int)": Func(
             return_type="int",
             name="imageAtomicAnd",
             args=[
                 Var(name="image", type="imageCube"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="int"),
@@ -3758,23 +3659,14 @@
             name="imageAtomicAnd",
             args=[
                 Var(name="image", type="iimage1DArray"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="int"),
             ],
         ),
-        "imageAtomicAnd(iimage1DArray, ivec2, int)": Func(
-            return_type="int",
-            name="imageAtomicAnd",
-            args=[
-                Var(name="image", type="iimage1DArray"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="int"),
-            ],
-        ),
         "imageAtomicAnd(image2DArray, ivec3, int)": Func(
             return_type="int",
             name="imageAtomicAnd",
             args=[
                 Var(name="image", type="image2DArray"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="int"),
@@ -3991,24 +3883,14 @@
             args=[
                 Var(name="image", type="iimage2DRect"),
                 Var(name="P", type="ivec2"),
                 Var(name="compare", type="uint"),
                 Var(name="data", type="uint"),
             ],
         ),
-        "imageAtomicCompSwap(iimage2DRect, ivec2, uint, uint)": Func(
-            return_type="uint",
-            name="imageAtomicCompSwap",
-            args=[
-                Var(name="image", type="iimage2DRect"),
-                Var(name="P", type="ivec2"),
-                Var(name="compare", type="uint"),
-                Var(name="data", type="uint"),
-            ],
-        ),
         "imageAtomicCompSwap(imageCube, ivec3, uint, uint)": Func(
             return_type="uint",
             name="imageAtomicCompSwap",
             args=[
                 Var(name="image", type="imageCube"),
                 Var(name="P", type="ivec3"),
                 Var(name="compare", type="uint"),
@@ -4081,24 +3963,14 @@
             args=[
                 Var(name="image", type="iimage1DArray"),
                 Var(name="P", type="ivec2"),
                 Var(name="compare", type="uint"),
                 Var(name="data", type="uint"),
             ],
         ),
-        "imageAtomicCompSwap(iimage1DArray, ivec2, uint, uint)": Func(
-            return_type="uint",
-            name="imageAtomicCompSwap",
-            args=[
-                Var(name="image", type="iimage1DArray"),
-                Var(name="P", type="ivec2"),
-                Var(name="compare", type="uint"),
-                Var(name="data", type="uint"),
-            ],
-        ),
         "imageAtomicCompSwap(image2DArray, ivec3, uint, uint)": Func(
             return_type="uint",
             name="imageAtomicCompSwap",
             args=[
                 Var(name="image", type="image2DArray"),
                 Var(name="P", type="ivec3"),
                 Var(name="compare", type="uint"),
@@ -4327,24 +4199,14 @@
             args=[
                 Var(name="image", type="iimage2DRect"),
                 Var(name="P", type="ivec2"),
                 Var(name="compare", type="int"),
                 Var(name="data", type="int"),
             ],
         ),
-        "imageAtomicCompSwap(iimage2DRect, ivec2, int, int)": Func(
-            return_type="int",
-            name="imageAtomicCompSwap",
-            args=[
-                Var(name="image", type="iimage2DRect"),
-                Var(name="P", type="ivec2"),
-                Var(name="compare", type="int"),
-                Var(name="data", type="int"),
-            ],
-        ),
         "imageAtomicCompSwap(imageCube, ivec3, int, int)": Func(
             return_type="int",
             name="imageAtomicCompSwap",
             args=[
                 Var(name="image", type="imageCube"),
                 Var(name="P", type="ivec3"),
                 Var(name="compare", type="int"),
@@ -4417,24 +4279,14 @@
             args=[
                 Var(name="image", type="iimage1DArray"),
                 Var(name="P", type="ivec2"),
                 Var(name="compare", type="int"),
                 Var(name="data", type="int"),
             ],
         ),
-        "imageAtomicCompSwap(iimage1DArray, ivec2, int, int)": Func(
-            return_type="int",
-            name="imageAtomicCompSwap",
-            args=[
-                Var(name="image", type="iimage1DArray"),
-                Var(name="P", type="ivec2"),
-                Var(name="compare", type="int"),
-                Var(name="data", type="int"),
-            ],
-        ),
         "imageAtomicCompSwap(image2DArray, ivec3, int, int)": Func(
             return_type="int",
             name="imageAtomicCompSwap",
             args=[
                 Var(name="image", type="image2DArray"),
                 Var(name="P", type="ivec3"),
                 Var(name="compare", type="int"),
@@ -4652,23 +4504,14 @@
             name="imageAtomicExchange",
             args=[
                 Var(name="image", type="iimage2DRect"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="uint"),
             ],
         ),
-        "imageAtomicExchange(iimage2DRect, ivec2, uint)": Func(
-            return_type="uint",
-            name="imageAtomicExchange",
-            args=[
-                Var(name="image", type="iimage2DRect"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="uint"),
-            ],
-        ),
         "imageAtomicExchange(imageCube, ivec3, uint)": Func(
             return_type="uint",
             name="imageAtomicExchange",
             args=[
                 Var(name="image", type="imageCube"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="uint"),
@@ -4733,23 +4576,14 @@
             name="imageAtomicExchange",
             args=[
                 Var(name="image", type="iimage1DArray"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="uint"),
             ],
         ),
-        "imageAtomicExchange(iimage1DArray, ivec2, uint)": Func(
-            return_type="uint",
-            name="imageAtomicExchange",
-            args=[
-                Var(name="image", type="iimage1DArray"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="uint"),
-            ],
-        ),
         "imageAtomicExchange(image2DArray, ivec3, uint)": Func(
             return_type="uint",
             name="imageAtomicExchange",
             args=[
                 Var(name="image", type="image2DArray"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="uint"),
@@ -4955,23 +4789,14 @@
             name="imageAtomicExchange",
             args=[
                 Var(name="image", type="iimage2DRect"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="int"),
             ],
         ),
-        "imageAtomicExchange(iimage2DRect, ivec2, int)": Func(
-            return_type="int",
-            name="imageAtomicExchange",
-            args=[
-                Var(name="image", type="iimage2DRect"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="int"),
-            ],
-        ),
         "imageAtomicExchange(imageCube, ivec3, int)": Func(
             return_type="int",
             name="imageAtomicExchange",
             args=[
                 Var(name="image", type="imageCube"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="int"),
@@ -5036,23 +4861,14 @@
             name="imageAtomicExchange",
             args=[
                 Var(name="image", type="iimage1DArray"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="int"),
             ],
         ),
-        "imageAtomicExchange(iimage1DArray, ivec2, int)": Func(
-            return_type="int",
-            name="imageAtomicExchange",
-            args=[
-                Var(name="image", type="iimage1DArray"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="int"),
-            ],
-        ),
         "imageAtomicExchange(image2DArray, ivec3, int)": Func(
             return_type="int",
             name="imageAtomicExchange",
             args=[
                 Var(name="image", type="image2DArray"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="int"),
@@ -5258,23 +5074,14 @@
             name="imageAtomicExchange",
             args=[
                 Var(name="image", type="iimage2DRect"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="float"),
             ],
         ),
-        "imageAtomicExchange(iimage2DRect, ivec2, float)": Func(
-            return_type="int",
-            name="imageAtomicExchange",
-            args=[
-                Var(name="image", type="iimage2DRect"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="float"),
-            ],
-        ),
         "imageAtomicExchange(imageCube, ivec3, float)": Func(
             return_type="int",
             name="imageAtomicExchange",
             args=[
                 Var(name="image", type="imageCube"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="float"),
@@ -5339,23 +5146,14 @@
             name="imageAtomicExchange",
             args=[
                 Var(name="image", type="iimage1DArray"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="float"),
             ],
         ),
-        "imageAtomicExchange(iimage1DArray, ivec2, float)": Func(
-            return_type="int",
-            name="imageAtomicExchange",
-            args=[
-                Var(name="image", type="iimage1DArray"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="float"),
-            ],
-        ),
         "imageAtomicExchange(image2DArray, ivec3, float)": Func(
             return_type="int",
             name="imageAtomicExchange",
             args=[
                 Var(name="image", type="image2DArray"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="float"),
@@ -5561,23 +5359,14 @@
             name="imageAtomicMax",
             args=[
                 Var(name="image", type="iimage2DRect"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="uint"),
             ],
         ),
-        "imageAtomicMax(iimage2DRect, ivec2, uint)": Func(
-            return_type="uint",
-            name="imageAtomicMax",
-            args=[
-                Var(name="image", type="iimage2DRect"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="uint"),
-            ],
-        ),
         "imageAtomicMax(imageCube, ivec3, uint)": Func(
             return_type="uint",
             name="imageAtomicMax",
             args=[
                 Var(name="image", type="imageCube"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="uint"),
@@ -5642,23 +5431,14 @@
             name="imageAtomicMax",
             args=[
                 Var(name="image", type="iimage1DArray"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="uint"),
             ],
         ),
-        "imageAtomicMax(iimage1DArray, ivec2, uint)": Func(
-            return_type="uint",
-            name="imageAtomicMax",
-            args=[
-                Var(name="image", type="iimage1DArray"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="uint"),
-            ],
-        ),
         "imageAtomicMax(image2DArray, ivec3, uint)": Func(
             return_type="uint",
             name="imageAtomicMax",
             args=[
                 Var(name="image", type="image2DArray"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="uint"),
@@ -5864,23 +5644,14 @@
             name="imageAtomicMax",
             args=[
                 Var(name="image", type="iimage2DRect"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="int"),
             ],
         ),
-        "imageAtomicMax(iimage2DRect, ivec2, int)": Func(
-            return_type="int",
-            name="imageAtomicMax",
-            args=[
-                Var(name="image", type="iimage2DRect"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="int"),
-            ],
-        ),
         "imageAtomicMax(imageCube, ivec3, int)": Func(
             return_type="int",
             name="imageAtomicMax",
             args=[
                 Var(name="image", type="imageCube"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="int"),
@@ -5945,23 +5716,14 @@
             name="imageAtomicMax",
             args=[
                 Var(name="image", type="iimage1DArray"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="int"),
             ],
         ),
-        "imageAtomicMax(iimage1DArray, ivec2, int)": Func(
-            return_type="int",
-            name="imageAtomicMax",
-            args=[
-                Var(name="image", type="iimage1DArray"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="int"),
-            ],
-        ),
         "imageAtomicMax(image2DArray, ivec3, int)": Func(
             return_type="int",
             name="imageAtomicMax",
             args=[
                 Var(name="image", type="image2DArray"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="int"),
@@ -6167,23 +5929,14 @@
             name="imageAtomicMin",
             args=[
                 Var(name="image", type="iimage2DRect"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="uint"),
             ],
         ),
-        "imageAtomicMin(iimage2DRect, ivec2, uint)": Func(
-            return_type="uint",
-            name="imageAtomicMin",
-            args=[
-                Var(name="image", type="iimage2DRect"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="uint"),
-            ],
-        ),
         "imageAtomicMin(imageCube, ivec3, uint)": Func(
             return_type="uint",
             name="imageAtomicMin",
             args=[
                 Var(name="image", type="imageCube"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="uint"),
@@ -6248,23 +6001,14 @@
             name="imageAtomicMin",
             args=[
                 Var(name="image", type="iimage1DArray"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="uint"),
             ],
         ),
-        "imageAtomicMin(iimage1DArray, ivec2, uint)": Func(
-            return_type="uint",
-            name="imageAtomicMin",
-            args=[
-                Var(name="image", type="iimage1DArray"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="uint"),
-            ],
-        ),
         "imageAtomicMin(image2DArray, ivec3, uint)": Func(
             return_type="uint",
             name="imageAtomicMin",
             args=[
                 Var(name="image", type="image2DArray"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="uint"),
@@ -6470,23 +6214,14 @@
             name="imageAtomicMin",
             args=[
                 Var(name="image", type="iimage2DRect"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="int"),
             ],
         ),
-        "imageAtomicMin(iimage2DRect, ivec2, int)": Func(
-            return_type="int",
-            name="imageAtomicMin",
-            args=[
-                Var(name="image", type="iimage2DRect"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="int"),
-            ],
-        ),
         "imageAtomicMin(imageCube, ivec3, int)": Func(
             return_type="int",
             name="imageAtomicMin",
             args=[
                 Var(name="image", type="imageCube"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="int"),
@@ -6551,23 +6286,14 @@
             name="imageAtomicMin",
             args=[
                 Var(name="image", type="iimage1DArray"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="int"),
             ],
         ),
-        "imageAtomicMin(iimage1DArray, ivec2, int)": Func(
-            return_type="int",
-            name="imageAtomicMin",
-            args=[
-                Var(name="image", type="iimage1DArray"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="int"),
-            ],
-        ),
         "imageAtomicMin(image2DArray, ivec3, int)": Func(
             return_type="int",
             name="imageAtomicMin",
             args=[
                 Var(name="image", type="image2DArray"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="int"),
@@ -6773,23 +6499,14 @@
             name="imageAtomicOr",
             args=[
                 Var(name="image", type="iimage2DRect"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="uint"),
             ],
         ),
-        "imageAtomicOr(iimage2DRect, ivec2, uint)": Func(
-            return_type="uint",
-            name="imageAtomicOr",
-            args=[
-                Var(name="image", type="iimage2DRect"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="uint"),
-            ],
-        ),
         "imageAtomicOr(imageCube, ivec3, uint)": Func(
             return_type="uint",
             name="imageAtomicOr",
             args=[
                 Var(name="image", type="imageCube"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="uint"),
@@ -6854,23 +6571,14 @@
             name="imageAtomicOr",
             args=[
                 Var(name="image", type="iimage1DArray"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="uint"),
             ],
         ),
-        "imageAtomicOr(iimage1DArray, ivec2, uint)": Func(
-            return_type="uint",
-            name="imageAtomicOr",
-            args=[
-                Var(name="image", type="iimage1DArray"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="uint"),
-            ],
-        ),
         "imageAtomicOr(image2DArray, ivec3, uint)": Func(
             return_type="uint",
             name="imageAtomicOr",
             args=[
                 Var(name="image", type="image2DArray"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="uint"),
@@ -7076,23 +6784,14 @@
             name="imageAtomicOr",
             args=[
                 Var(name="image", type="iimage2DRect"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="int"),
             ],
         ),
-        "imageAtomicOr(iimage2DRect, ivec2, int)": Func(
-            return_type="int",
-            name="imageAtomicOr",
-            args=[
-                Var(name="image", type="iimage2DRect"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="int"),
-            ],
-        ),
         "imageAtomicOr(imageCube, ivec3, int)": Func(
             return_type="int",
             name="imageAtomicOr",
             args=[
                 Var(name="image", type="imageCube"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="int"),
@@ -7157,23 +6856,14 @@
             name="imageAtomicOr",
             args=[
                 Var(name="image", type="iimage1DArray"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="int"),
             ],
         ),
-        "imageAtomicOr(iimage1DArray, ivec2, int)": Func(
-            return_type="int",
-            name="imageAtomicOr",
-            args=[
-                Var(name="image", type="iimage1DArray"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="int"),
-            ],
-        ),
         "imageAtomicOr(image2DArray, ivec3, int)": Func(
             return_type="int",
             name="imageAtomicOr",
             args=[
                 Var(name="image", type="image2DArray"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="int"),
@@ -7379,23 +7069,14 @@
             name="imageAtomicXor",
             args=[
                 Var(name="image", type="iimage2DRect"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="uint"),
             ],
         ),
-        "imageAtomicXor(iimage2DRect, ivec2, uint)": Func(
-            return_type="uint",
-            name="imageAtomicXor",
-            args=[
-                Var(name="image", type="iimage2DRect"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="uint"),
-            ],
-        ),
         "imageAtomicXor(imageCube, ivec3, uint)": Func(
             return_type="uint",
             name="imageAtomicXor",
             args=[
                 Var(name="image", type="imageCube"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="uint"),
@@ -7460,23 +7141,14 @@
             name="imageAtomicXor",
             args=[
                 Var(name="image", type="iimage1DArray"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="uint"),
             ],
         ),
-        "imageAtomicXor(iimage1DArray, ivec2, uint)": Func(
-            return_type="uint",
-            name="imageAtomicXor",
-            args=[
-                Var(name="image", type="iimage1DArray"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="uint"),
-            ],
-        ),
         "imageAtomicXor(image2DArray, ivec3, uint)": Func(
             return_type="uint",
             name="imageAtomicXor",
             args=[
                 Var(name="image", type="image2DArray"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="uint"),
@@ -7682,23 +7354,14 @@
             name="imageAtomicXor",
             args=[
                 Var(name="image", type="iimage2DRect"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="int"),
             ],
         ),
-        "imageAtomicXor(iimage2DRect, ivec2, int)": Func(
-            return_type="int",
-            name="imageAtomicXor",
-            args=[
-                Var(name="image", type="iimage2DRect"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="int"),
-            ],
-        ),
         "imageAtomicXor(imageCube, ivec3, int)": Func(
             return_type="int",
             name="imageAtomicXor",
             args=[
                 Var(name="image", type="imageCube"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="int"),
@@ -7763,23 +7426,14 @@
             name="imageAtomicXor",
             args=[
                 Var(name="image", type="iimage1DArray"),
                 Var(name="P", type="ivec2"),
                 Var(name="data", type="int"),
             ],
         ),
-        "imageAtomicXor(iimage1DArray, ivec2, int)": Func(
-            return_type="int",
-            name="imageAtomicXor",
-            args=[
-                Var(name="image", type="iimage1DArray"),
-                Var(name="P", type="ivec2"),
-                Var(name="data", type="int"),
-            ],
-        ),
         "imageAtomicXor(image2DArray, ivec3, int)": Func(
             return_type="int",
             name="imageAtomicXor",
             args=[
                 Var(name="image", type="image2DArray"),
                 Var(name="P", type="ivec3"),
                 Var(name="data", type="int"),
@@ -7967,22 +7621,14 @@
             name="imageLoad",
             args=[
                 Var(name="image", type="image2DRect"),
                 Var(name="P", type="ivec2"),
             ],
         ),
         "imageLoad(iimage2DRect, ivec2)": Func(
-            return_type="ivec4",
-            name="imageLoad",
-            args=[
-                Var(name="image", type="iimage2DRect"),
-                Var(name="P", type="ivec2"),
-            ],
-        ),
-        "imageLoad(iimage2DRect, ivec2)": Func(
             return_type="uvec4",
             name="imageLoad",
             args=[
                 Var(name="image", type="iimage2DRect"),
                 Var(name="P", type="ivec2"),
             ],
         ),
@@ -8039,22 +7685,14 @@
             name="imageLoad",
             args=[
                 Var(name="image", type="image1DArray"),
                 Var(name="P", type="ivec2"),
             ],
         ),
         "imageLoad(iimage1DArray, ivec2)": Func(
-            return_type="ivec4",
-            name="imageLoad",
-            args=[
-                Var(name="image", type="iimage1DArray"),
-                Var(name="P", type="ivec2"),
-            ],
-        ),
-        "imageLoad(iimage1DArray, ivec2)": Func(
             return_type="uvec4",
             name="imageLoad",
             args=[
                 Var(name="image", type="iimage1DArray"),
                 Var(name="P", type="ivec2"),
             ],
         ),
@@ -8317,42 +7955,28 @@
         "imageSize(iimage2DRect)": Func(
             return_type="ivec2",
             name="imageSize",
             args=[
                 Var(name="image", type="iimage2DRect"),
             ],
         ),
-        "imageSize(iimage2DRect)": Func(
-            return_type="ivec2",
-            name="imageSize",
-            args=[
-                Var(name="image", type="iimage2DRect"),
-            ],
-        ),
         "imageSize(image1DArray)": Func(
             return_type="ivec2",
             name="imageSize",
             args=[
                 Var(name="image", type="image1DArray"),
             ],
         ),
         "imageSize(iimage1DArray)": Func(
             return_type="ivec2",
             name="imageSize",
             args=[
                 Var(name="image", type="iimage1DArray"),
             ],
         ),
-        "imageSize(iimage1DArray)": Func(
-            return_type="ivec2",
-            name="imageSize",
-            args=[
-                Var(name="image", type="iimage1DArray"),
-            ],
-        ),
         "imageSize(image2DArray)": Func(
             return_type="ivec3",
             name="imageSize",
             args=[
                 Var(name="image", type="image2DArray"),
             ],
         ),
@@ -9490,22 +9114,14 @@
             return_type="vec4",
             name="max",
             args=[
                 Var(name="x", type="vec4"),
                 Var(name="y", type="vec4"),
             ],
         ),
-        "max(float, float)": Func(
-            return_type="float",
-            name="max",
-            args=[
-                Var(name="x", type="float"),
-                Var(name="y", type="float"),
-            ],
-        ),
         "max(vec2, float)": Func(
             return_type="vec2",
             name="max",
             args=[
                 Var(name="x", type="vec2"),
                 Var(name="y", type="float"),
             ],
@@ -9554,22 +9170,14 @@
             return_type="dvec4",
             name="max",
             args=[
                 Var(name="x", type="dvec4"),
                 Var(name="y", type="dvec4"),
             ],
         ),
-        "max(double, double)": Func(
-            return_type="double",
-            name="max",
-            args=[
-                Var(name="x", type="double"),
-                Var(name="y", type="double"),
-            ],
-        ),
         "max(dvec2, double)": Func(
             return_type="dvec2",
             name="max",
             args=[
                 Var(name="x", type="dvec2"),
                 Var(name="y", type="double"),
             ],
@@ -9618,22 +9226,14 @@
             return_type="ivec4",
             name="max",
             args=[
                 Var(name="x", type="ivec4"),
                 Var(name="y", type="ivec4"),
             ],
         ),
-        "max(int, int)": Func(
-            return_type="int",
-            name="max",
-            args=[
-                Var(name="x", type="int"),
-                Var(name="y", type="int"),
-            ],
-        ),
         "max(ivec2, int)": Func(
             return_type="ivec2",
             name="max",
             args=[
                 Var(name="x", type="ivec2"),
                 Var(name="y", type="int"),
             ],
@@ -9682,22 +9282,14 @@
             return_type="uvec4",
             name="max",
             args=[
                 Var(name="x", type="uvec4"),
                 Var(name="y", type="uvec4"),
             ],
         ),
-        "max(uint, uint)": Func(
-            return_type="uint",
-            name="max",
-            args=[
-                Var(name="x", type="uint"),
-                Var(name="y", type="uint"),
-            ],
-        ),
         "max(uvec2, uint)": Func(
             return_type="uvec2",
             name="max",
             args=[
                 Var(name="x", type="uvec2"),
                 Var(name="y", type="uint"),
             ],
@@ -9759,22 +9351,14 @@
             return_type="vec4",
             name="min",
             args=[
                 Var(name="x", type="vec4"),
                 Var(name="y", type="vec4"),
             ],
         ),
-        "min(float, float)": Func(
-            return_type="float",
-            name="min",
-            args=[
-                Var(name="x", type="float"),
-                Var(name="y", type="float"),
-            ],
-        ),
         "min(vec2, float)": Func(
             return_type="vec2",
             name="min",
             args=[
                 Var(name="x", type="vec2"),
                 Var(name="y", type="float"),
             ],
@@ -9823,22 +9407,14 @@
             return_type="dvec4",
             name="min",
             args=[
                 Var(name="x", type="dvec4"),
                 Var(name="y", type="dvec4"),
             ],
         ),
-        "min(double, double)": Func(
-            return_type="double",
-            name="min",
-            args=[
-                Var(name="x", type="double"),
-                Var(name="y", type="double"),
-            ],
-        ),
         "min(dvec2, double)": Func(
             return_type="dvec2",
             name="min",
             args=[
                 Var(name="x", type="dvec2"),
                 Var(name="y", type="double"),
             ],
@@ -9887,22 +9463,14 @@
             return_type="ivec4",
             name="min",
             args=[
                 Var(name="x", type="ivec4"),
                 Var(name="y", type="ivec4"),
             ],
         ),
-        "min(int, int)": Func(
-            return_type="int",
-            name="min",
-            args=[
-                Var(name="x", type="int"),
-                Var(name="y", type="int"),
-            ],
-        ),
         "min(ivec2, int)": Func(
             return_type="ivec2",
             name="min",
             args=[
                 Var(name="x", type="ivec2"),
                 Var(name="y", type="int"),
             ],
@@ -9951,22 +9519,14 @@
             return_type="uvec4",
             name="min",
             args=[
                 Var(name="x", type="uvec4"),
                 Var(name="y", type="uvec4"),
             ],
         ),
-        "min(uint, uint)": Func(
-            return_type="uint",
-            name="min",
-            args=[
-                Var(name="x", type="uint"),
-                Var(name="y", type="uint"),
-            ],
-        ),
         "min(uvec2, uint)": Func(
             return_type="uvec2",
             name="min",
             args=[
                 Var(name="x", type="uvec2"),
                 Var(name="y", type="uint"),
             ],
@@ -10019,23 +9579,14 @@
             name="mix",
             args=[
                 Var(name="x", type="vec4"),
                 Var(name="y", type="vec4"),
                 Var(name="a", type="vec4"),
             ],
         ),
-        "mix(float, float, float)": Func(
-            return_type="float",
-            name="mix",
-            args=[
-                Var(name="x", type="float"),
-                Var(name="y", type="float"),
-                Var(name="a", type="float"),
-            ],
-        ),
         "mix(vec2, vec2, float)": Func(
             return_type="vec2",
             name="mix",
             args=[
                 Var(name="x", type="vec2"),
                 Var(name="y", type="vec2"),
                 Var(name="a", type="float"),
@@ -10091,23 +9642,14 @@
             name="mix",
             args=[
                 Var(name="x", type="dvec4"),
                 Var(name="y", type="dvec4"),
                 Var(name="a", type="dvec4"),
             ],
         ),
-        "mix(double, double, double)": Func(
-            return_type="double",
-            name="mix",
-            args=[
-                Var(name="x", type="double"),
-                Var(name="y", type="double"),
-                Var(name="a", type="double"),
-            ],
-        ),
         "mix(dvec2, dvec2, double)": Func(
             return_type="dvec2",
             name="mix",
             args=[
                 Var(name="x", type="dvec2"),
                 Var(name="y", type="dvec2"),
                 Var(name="a", type="double"),
@@ -10339,22 +9881,14 @@
             return_type="vec4",
             name="mod",
             args=[
                 Var(name="x", type="vec4"),
                 Var(name="y", type="float"),
             ],
         ),
-        "mod(float, float)": Func(
-            return_type="float",
-            name="mod",
-            args=[
-                Var(name="x", type="float"),
-                Var(name="y", type="float"),
-            ],
-        ),
         "mod(vec2, vec2)": Func(
             return_type="vec2",
             name="mod",
             args=[
                 Var(name="x", type="vec2"),
                 Var(name="y", type="vec2"),
             ],
@@ -10403,22 +9937,14 @@
             return_type="dvec4",
             name="mod",
             args=[
                 Var(name="x", type="dvec4"),
                 Var(name="y", type="double"),
             ],
         ),
-        "mod(double, double)": Func(
-            return_type="double",
-            name="mod",
-            args=[
-                Var(name="x", type="double"),
-                Var(name="y", type="double"),
-            ],
-        ),
         "mod(dvec2, dvec2)": Func(
             return_type="dvec2",
             name="mod",
             args=[
                 Var(name="x", type="dvec2"),
                 Var(name="y", type="dvec2"),
             ],
@@ -11430,23 +10956,14 @@
             name="smoothstep",
             args=[
                 Var(name="edge0", type="vec4"),
                 Var(name="edge1", type="vec4"),
                 Var(name="x", type="vec4"),
             ],
         ),
-        "smoothstep(float, float, float)": Func(
-            return_type="float",
-            name="smoothstep",
-            args=[
-                Var(name="edge0", type="float"),
-                Var(name="edge1", type="float"),
-                Var(name="x", type="float"),
-            ],
-        ),
         "smoothstep(float, float, vec2)": Func(
             return_type="vec2",
             name="smoothstep",
             args=[
                 Var(name="edge0", type="float"),
                 Var(name="edge1", type="float"),
                 Var(name="x", type="vec2"),
@@ -11502,23 +11019,14 @@
             name="smoothstep",
             args=[
                 Var(name="edge0", type="dvec4"),
                 Var(name="edge1", type="dvec4"),
                 Var(name="x", type="dvec4"),
             ],
         ),
-        "smoothstep(double, double, double)": Func(
-            return_type="double",
-            name="smoothstep",
-            args=[
-                Var(name="edge0", type="double"),
-                Var(name="edge1", type="double"),
-                Var(name="x", type="double"),
-            ],
-        ),
         "smoothstep(double, double, dvec2)": Func(
             return_type="dvec2",
             name="smoothstep",
             args=[
                 Var(name="edge0", type="double"),
                 Var(name="edge1", type="double"),
                 Var(name="x", type="dvec2"),
@@ -11626,22 +11134,14 @@
             return_type="vec4",
             name="step",
             args=[
                 Var(name="edge", type="vec4"),
                 Var(name="x", type="vec4"),
             ],
         ),
-        "step(float, float)": Func(
-            return_type="float",
-            name="step",
-            args=[
-                Var(name="edge", type="float"),
-                Var(name="x", type="float"),
-            ],
-        ),
         "step(float, vec2)": Func(
             return_type="vec2",
             name="step",
             args=[
                 Var(name="edge", type="float"),
                 Var(name="x", type="vec2"),
             ],
@@ -11690,22 +11190,14 @@
             return_type="dvec4",
             name="step",
             args=[
                 Var(name="edge", type="dvec4"),
                 Var(name="x", type="dvec4"),
             ],
         ),
-        "step(double, double)": Func(
-            return_type="double",
-            name="step",
-            args=[
-                Var(name="edge", type="double"),
-                Var(name="x", type="double"),
-            ],
-        ),
         "step(double, dvec2)": Func(
             return_type="dvec2",
             name="step",
             args=[
                 Var(name="edge", type="double"),
                 Var(name="x", type="dvec2"),
             ],
```

### Comparing `python_glass-0.1.54/glass/ShaderParser_/ShaderParser_.py` & `python_glass-0.1.55/glass/ShaderParser_/ShaderParser_.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import sys
 import os
-import platform
 import glob
 import tree_sitter
-import re
 import zipfile
+import platform
 
 from ..GLInfo import GLInfo
 from .ShaderSyntaxTokens import Var, Attribute, Func, FuncCall, Struct, SimpleVar
 from .ShaderBuiltins import ShaderBuiltins
 
 from ..utils import resolve_array
 from ..helper import greater_type, type_list_distance, subscript_type
@@ -52,31 +51,27 @@
             dll_suffix = "dylib"
         else:
             dll_suffix = "dll"
 
         machine = platform.machine()
         bits = platform.architecture()[0]
 
-        dll_file = (
-            f"{self_folder}/tree-sitter-glsl/lib/{machine}/{platform_system}/{bits}/glsl.{dll_suffix}"
-        )
+        dll_file = f"{self_folder}/tree-sitter-glsl/lib/{machine}/{platform_system}/{bits}/glsl.{dll_suffix}"
         dll_folder = os.path.dirname(dll_file)
         if not os.path.isdir(dll_folder):
             os.makedirs(dll_folder)
 
         if not os.path.isfile(dll_file):
             if not os.path.isfile(self_folder + "/tree-sitter-glsl/src/parser.c"):
                 zip_file = zipfile.ZipFile(self_folder + "/tree-sitter-glsl/src.zip")
                 zip_file.extractall(self_folder + "/tree-sitter-glsl/src")
                 zip_file.close()
 
             Language.build_library(dll_file, [self_folder + "/tree-sitter-glsl"])
-            trash_files = glob.glob(
-                f"{dll_folder}/glsl.*"
-            )
+            trash_files = glob.glob(f"{dll_folder}/glsl.*")
             for trash_file in trash_files:
                 if os.path.abspath(trash_file) != os.path.abspath(dll_file):
                     os.remove(trash_file)
 
         GLSL_LANGUAGE = Language(dll_file, "glsl")
         ShaderParser_.__glsl_parser = Parser()
         ShaderParser_.__glsl_parser.set_language(GLSL_LANGUAGE)
@@ -622,18 +617,16 @@
 
         min_distance = None
         best_mached_func = None
         candidate_funcs = []
         for candidate_func in self.candidate_functions(func_call.name):
             if candidate_func.argc != len(arg_types):
                 continue
-            
-            current_distance = type_list_distance(
-                arg_types, candidate_func.arg_types
-            )
+
+            current_distance = type_list_distance(arg_types, candidate_func.arg_types)
             if isinstance(current_distance, int):
                 if current_distance == 0:
                     min_distance = 0
                     best_mached_func = candidate_func
                     break
 
                 if min_distance is None or current_distance < min_distance:
@@ -641,15 +634,15 @@
                     best_mached_func = candidate_func
             else:
                 if current_distance == "inf":
                     continue
 
                 candidate_funcs.append(candidate_func)
 
-        return (best_mached_func if best_mached_func is not None else candidate_funcs)
+        return best_mached_func if best_mached_func is not None else candidate_funcs
 
     def resolve_functions(self):
         if not ShaderBuiltins.function_groups:
             for func in ShaderBuiltins.functions.values():
                 if func.name not in ShaderBuiltins.function_groups:
                     ShaderBuiltins.function_groups[func.name] = []
                 ShaderBuiltins.function_groups[func.name].append(func)
@@ -676,26 +669,26 @@
         if func_name in ShaderBuiltins.function_groups:
             yield from ShaderBuiltins.function_groups[func_name]
 
     @staticmethod
     def get_return_type(func_list):
         if isinstance(func_list, Func):
             return func_list.return_type
-        
+
         if isinstance(func_list, list):
             common_return_type = ""
             for func in func_list:
                 if common_return_type == "":
                     common_return_type = func.return_type
                 else:
                     if common_return_type != func.return_type:
                         return ""
-                    
+
             return common_return_type
-        
+
         return ""
 
     def analyse_type(self, expression: tree_sitter.Node, func: Func) -> str:
         if expression.type == "number_literal":
             text = expression.text.decode("utf-8")
             if (
                 expression.next_sibling is not None
```

### Comparing `python_glass-0.1.54/glass/ShaderParser_/ShaderSyntaxTokens.py` & `python_glass-0.1.55/glass/ShaderParser_/ShaderSyntaxTokens.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,8 +222,7 @@
             struct.is_used = flag
 
     def __repr__(self):
         return f"{self.return_type} {self.signature}"
 
     def __bool__(self):
         return True
-
```

### Comparing `python_glass-0.1.54/glass/ShaderParser_/generate_code.py` & `python_glass-0.1.55/glass/ShaderParser_/generate_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -352,15 +352,15 @@
     "bvec": ["bvec2", "bvec3", "bvec4"],
     "vec": ["vec2", "vec3", "vec4"],
     "ivec": ["ivec2", "ivec3", "ivec4"],
     "uvec": ["uvec2", "uvec3", "uvec4"],
     "dvec": ["dvec2", "dvec3", "dvec4"],
 }
 
-definition_list = []
+definition_dict = {}
 
 for func_name in func_list:
     response = requests.get(
         f"https://registry.khronos.org/OpenGL-Refpages/gl4/html/{func_name}.xhtml"
     )
     soup = bs4.BeautifulSoup(response.text, "html.parser")
     code_block = soup.select(f"#{func_name} > div.refsynopsisdiv")
@@ -434,50 +434,48 @@
 
             for j in range(n_gen_types):
                 for i in range(n_optionals + 1):
                     local_arg_types = [
                         arg_type[j] for arg_type in arg_types[: argc - i]
                     ]
                     signature = f"{func_name_}({', '.join(local_arg_types)})"
-                    definition_list.append(
-                        {
-                            "name": func_name_,
-                            "return_type": return_type[j],
-                            "arg_types": local_arg_types,
-                            "arg_names": arg_names[: argc - i],
-                            "signature": signature,
-                        }
-                    )
+                    definition_dict[signature] = {
+                        "name": func_name_,
+                        "return_type": return_type[j],
+                        "arg_types": local_arg_types,
+                        "arg_names": arg_names[: argc - i],
+                        "signature": signature,
+                    }
 
             success = True
 
     if not success:
         print(func_name, "failed")
 
 self_folder = os.path.dirname(os.path.abspath(__file__))
 content = open(self_folder + "/ShaderBuiltins.py").read()
 pos_func = content.find("functions = ")
 if pos_func == -1:
     exit()
 
 content = content[:pos_func] + "functions = {\n"
-for func in definition_list:
+for func in definition_dict.values():
     content += f'        "{func["signature"]}": Func(\n'
     content += f'            return_type="{func["return_type"]}",\n'
     content += f'            name="{func["name"]}",\n'
-    content += f"            args=[\n"
+    content += "            args=[\n"
     for arg_name, arg_type in zip(func["arg_names"], func["arg_types"]):
         if arg_type not in atom_type_names:
             print(f"not supported type '{arg_type}'", func["name"])
 
         pos_bracket = arg_name.find("[")
         if pos_bracket != -1:
             arg_type += arg_name[pos_bracket:]
             arg_name = arg_name[:pos_bracket]
         content += f'                Var(name="{arg_name}", type="{arg_type}"),\n'
-    content += f"            ]\n"
-    content += f"        ),\n"
+    content += "            ]\n"
+    content += "        ),\n"
 content += "    }\n"
 
 out_file = open(self_folder + "/ShaderBuiltins.py", "w")
 out_file.write(content)
 out_file.close()
```

### Comparing `python_glass-0.1.54/glass/ShaderParser_/minifyc.py` & `python_glass-0.1.55/glass/ShaderParser_/minifyc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from .pcpp import pcmd
-import sys
 import io
 
 
 def is_space(char):
     return char in [" ", "\t", "\n", "\r", "\v", "\f"]
```

### Comparing `python_glass-0.1.54/glass/ShaderParser_/pcpp/LICENSE` & `python_glass-0.1.55/glass/ShaderParser_/pcpp/LICENSE`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/ShaderParser_/pcpp/evaluator.py` & `python_glass-0.1.55/glass/ShaderParser_/pcpp/evaluator.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/ShaderParser_/pcpp/lextab.py` & `python_glass-0.1.55/glass/ShaderParser_/pcpp/lextab.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/ShaderParser_/pcpp/parser.py` & `python_glass-0.1.55/glass/ShaderParser_/pcpp/parser.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/ShaderParser_/pcpp/parsetab.py` & `python_glass-0.1.55/glass/ShaderParser_/pcpp/parsetab.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/ShaderParser_/pcpp/pcmd.py` & `python_glass-0.1.55/glass/ShaderParser_/pcpp/pcmd.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/ShaderParser_/pcpp/ply/cpp.py` & `python_glass-0.1.55/glass/ShaderParser_/pcpp/ply/cpp.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/ShaderParser_/pcpp/ply/ctokens.py` & `python_glass-0.1.55/glass/ShaderParser_/pcpp/ply/ctokens.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/ShaderParser_/pcpp/ply/lex.py` & `python_glass-0.1.55/glass/ShaderParser_/pcpp/ply/lex.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/ShaderParser_/pcpp/ply/yacc.py` & `python_glass-0.1.55/glass/ShaderParser_/pcpp/ply/yacc.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/ShaderParser_/pcpp/ply/ygen.py` & `python_glass-0.1.55/glass/ShaderParser_/pcpp/ply/ygen.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/ShaderParser_/pcpp/preprocessor.py` & `python_glass-0.1.55/glass/ShaderParser_/pcpp/preprocessor.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/ShaderParser_/tree-sitter-glsl/lib/AMD64/Windows/32bit/glsl.dll` & `python_glass-0.1.55/glass/ShaderParser_/tree-sitter-glsl/lib/AMD64/Windows/32bit/glsl.dll`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/ShaderParser_/tree-sitter-glsl/lib/AMD64/Windows/64bit/glsl.dll` & `python_glass-0.1.55/glass/ShaderParser_/tree-sitter-glsl/lib/AMD64/Windows/64bit/glsl.dll`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/ShaderParser_/tree-sitter-glsl/lib/x86_64/Linux/64bit/glsl.so` & `python_glass-0.1.55/glass/ShaderParser_/tree-sitter-glsl/lib/x86_64/Linux/64bit/glsl.so`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/ShaderParser_/tree-sitter-glsl/src.zip` & `python_glass-0.1.55/glass/ShaderParser_/tree-sitter-glsl/src.zip`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/ShaderProgram.py` & `python_glass-0.1.55/glass/ShaderProgram.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-
 from OpenGL import GL
 import pathlib
 import warnings
 import struct
 import copy
 import ctypes
 
@@ -276,17 +275,20 @@
 
         related_files = "\n  " + "\n  ".join(
             [printable_path(file_name) for file_name in self.related_files]
         )
         if GlassConfig.print:
             print(f"linking program: {related_files}")
 
-        GL.glProgramParameteri(
-            self._id, GL.GL_PROGRAM_BINARY_RETRIEVABLE_HINT, GL.GL_TRUE
-        )
+        try:
+            GL.glProgramParameteri(
+                self._id, GL.GL_PROGRAM_BINARY_RETRIEVABLE_HINT, GL.GL_TRUE
+            )
+        except:
+            pass
         GL.glLinkProgram(self._id)
 
         message_bytes = GL.glGetProgramInfoLog(self._id)
         message = message_bytes
         if isinstance(message_bytes, bytes):
             message = str(message_bytes, encoding="utf-8")
```

### Comparing `python_glass-0.1.54/glass/Shaders.py` & `python_glass-0.1.55/glass/Shaders.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,16 +126,22 @@
         used_code = self._code
         if not GlassConfig.debug:
             used_code = minifyc(self._shader_parser.treeshake())
 
         version_pattern1 = r"#\s*version \d\d\d core"
         version_pattern2 = r"#\s*version \d\d\d"
         version_str = ""
-        if GLConfig.major_version > 3 or GLConfig.major_version == 3 and GLConfig.minor_version >= 3:
-            version_str = f"#version {GLConfig.major_version}{GLConfig.minor_version}0 core"
+        if (
+            GLConfig.major_version > 3
+            or GLConfig.major_version == 3
+            and GLConfig.minor_version >= 3
+        ):
+            version_str = (
+                f"#version {GLConfig.major_version}{GLConfig.minor_version}0 core"
+            )
         else:
             if GLConfig.major_version == 3:
                 if GLConfig.minor_version == 2:
                     version_str = "#version 150"
                 elif GLConfig.minor_version == 1:
                     version_str = "#version 140"
                 elif GLConfig.minor_version == 0:
@@ -143,15 +149,17 @@
             elif GLConfig.major_version == 2:
                 if GLConfig.minor_version == 1:
                     version_str = "#version 120"
                 elif GLConfig.minor_version == 0:
                     version_str = "#version 110"
 
         if not version_str:
-            raise RuntimeError(f"OpenGL version {GLConfig.major_version}.{GLConfig.minor_version} is not supported.")
+            raise RuntimeError(
+                f"OpenGL version {GLConfig.major_version}.{GLConfig.minor_version} is not supported."
+            )
 
         if re.search(version_pattern1, used_code):
             used_code = re.sub(version_pattern1, version_str, used_code)
         elif re.search(version_pattern2, used_code):
             used_code = re.sub(version_pattern2, version_str, used_code)
 
         if GlassConfig.print:
```

### Comparing `python_glass-0.1.54/glass/TextLoader.py` & `python_glass-0.1.55/glass/TextLoader.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/TextureUnits.py` & `python_glass-0.1.55/glass/TextureUnits.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/Uniform.py` & `python_glass-0.1.55/glass/Uniform.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/VAO.py` & `python_glass-0.1.55/glass/VAO.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/Vertices.py` & `python_glass-0.1.55/glass/Vertices.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/WeakDict.py` & `python_glass-0.1.55/glass/WeakDict.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/WeakList.py` & `python_glass-0.1.55/glass/WeakList.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/WeakRef.py` & `python_glass-0.1.55/glass/WeakRef.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/WeakSet.py` & `python_glass-0.1.55/glass/WeakSet.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/__init__.py` & `python_glass-0.1.55/glass/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,8 +36,9 @@
 
 from .GLConfig import GLConfig
 from .GlassConfig import GlassConfig
 from .GLInfo import GLInfo
 from .RenderHints import RenderHints
 from .download import download
 from .ImageLoader import ImageLoader
+
 # from .TextLoader import TextLoader, Font
```

### Comparing `python_glass-0.1.54/glass/__pyinstaller/hook-glass.py` & `python_glass-0.1.55/glass/__pyinstaller/hook-glass.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,26 +24,24 @@
                     len(abs_directory) : (-len(os.path.basename(file_path)) - 1)
                 ]
             )
             if "__glcache__" not in file_path:
                 file_list.append((file_path.replace("\\", "/"), target_path))
     return file_list
 
-
+self_folder = os.path.dirname(os.path.abspath(__file__))
 datas = find_files("glsl")
 datas += find_files("ShaderParser_/tree-sitter-glsl")
-datas.append(
-    (
-        os.path.abspath(
-            os.path.dirname(os.path.abspath(__file__)) + "/../LICENSE"
-        ).replace("\\", "/"),
-        "glass",
-    ),
-    (
-        os.path.abspath(
-            os.path.dirname(os.path.abspath(__file__)) + "/../ShaderParser_/pcpp/LICENSE"
-        ).replace("\\", "/"),
-        "glass/ShaderParser_/pcpp",
-    ),
+datas.extend(
+    [
+        (
+            os.path.abspath(self_folder + "/../LICENSE").replace("\\", "/"),
+            "glass",
+        ),
+        (
+            os.path.abspath(self_folder + "/../ShaderParser_/pcpp/LICENSE").replace("\\", "/"),
+            "glass/ShaderParser_/pcpp",
+        )
+    ]
 )
 if platform.system() == "Linux":
     hiddenimports = ["OpenGL.platform.egl"]
```

### Comparing `python_glass-0.1.54/glass/download.py` & `python_glass-0.1.55/glass/download.py`

 * *Files 7% similar despite different names*

```diff
@@ -82,23 +82,30 @@
 
 
 def is_China_user():
     return is_China_ip(public_ip())
 
 
 def pip_install(package_name: str):
-    install_cmd = [sys.executable, "-m", "pip", "install", package_name, "--no-warn-script-location"]
+    install_cmd = [
+        sys.executable,
+        "-m",
+        "pip",
+        "install",
+        package_name,
+        "--no-warn-script-location",
+    ]
     if is_China_user():
         install_cmd = [
             sys.executable,
             "-m",
             "pip",
             "install",
             package_name,
             "-i",
             "https://pypi.tuna.tsinghua.edu.cn/simple",
-            "--no-warn-script-location"
+            "--no-warn-script-location",
         ]
 
     return_code = subprocess.call(install_cmd)
     if return_code != 0:
         raise RuntimeError(f"failed to install {package_name}")
```

### Comparing `python_glass-0.1.54/glass/glsl/draw_frame.vs` & `python_glass-0.1.55/glass/glsl/draw_frame.vs`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/glsl/shadertoy_template.fs` & `python_glass-0.1.55/glass/glsl/shadertoy_template.fs`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/helper.py` & `python_glass-0.1.55/glass/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,18 +162,18 @@
 def get_dtype(internal_format):
     return GLInfo.format_info_map[internal_format][1]
 
 
 def type_distance(type1: str, type2: str):
     if type1 == type2:
         return 0
-    
+
     if type1 == "" or type2 == "":
         return "unknown"
-                
+
     def type_index(type_, types):
         for i, target_type in enumerate(types):
             if isinstance(target_type, tuple):
                 if type_ in target_type:
                     return i
             else:
                 if type_ == target_type:
@@ -187,15 +187,15 @@
         GLInfo.gvec4_types,
         GLInfo.gmat2x2_types,
         GLInfo.gmat3x2_types,
         GLInfo.gmat3x3_types,
         GLInfo.gmat3x4_types,
         GLInfo.gmat4x2_types,
         GLInfo.gmat4x3_types,
-        GLInfo.gmat4x4_types
+        GLInfo.gmat4x4_types,
     ]
 
     for target_types in all_types:
         type1_index = type_index(type1, target_types)
         type2_index = type_index(type2, target_types)
         if type1_index != -1 and type2_index != -1:
             return abs(type1_index - type2_index)
@@ -204,15 +204,15 @@
 
 
 def type_list_distance(type_list1, type_list2):
     for type1, type2 in zip(type_list1, type_list2):
         current_distance = type_distance(type1, type2)
         if current_distance == "inf":
             return "inf"
-    
+
     full_distance = 0
     for type1, type2 in zip(type_list1, type_list2):
         current_distance = type_distance(type1, type2)
         if current_distance == "unknown":
             return "unknown"
         full_distance += current_distance
```

### Comparing `python_glass-0.1.54/glass/iimage2D.py` & `python_glass-0.1.55/glass/iimage2D.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .sampler2D import sampler2D
 from .GLInfo import GLInfo
 from .utils import checktype
 from .isampler2D import isampler2D
 
-import numpy as np
 from OpenGL import GL
+import numpy as np
 
 
 class iimage2D(isampler2D):
 
     _default_internal_format = GL.GL_RGBA32I
     _default_filter_min = GL.GL_NEAREST
     _default_filter_mag = GL.GL_NEAREST
```

### Comparing `python_glass-0.1.54/glass/image2D.py` & `python_glass-0.1.55/glass/image2D.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/isampler2D.py` & `python_glass-0.1.55/glass/isampler2D.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .sampler2D import sampler2D
 from .GLInfo import GLInfo
 from .utils import checktype
 
-import numpy as np
 from OpenGL import GL
 import OpenGL.GL.ARB.bindless_texture as bt
+import numpy as np
 
 
 class isampler2D(sampler2D):
 
     _default_internal_format = GL.GL_RGBA32I
     _default_filter_min = GL.GL_NEAREST
     _default_filter_mag = GL.GL_NEAREST
```

### Comparing `python_glass-0.1.54/glass/isampler2DMS.py` & `python_glass-0.1.55/glass/isampler2DMS.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/sampler2D.py` & `python_glass-0.1.55/glass/sampler2D.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/sampler2DArray.py` & `python_glass-0.1.55/glass/sampler2DArray.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/sampler2DMS.py` & `python_glass-0.1.55/glass/sampler2DMS.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/samplerCube.py` & `python_glass-0.1.55/glass/samplerCube.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 os.environ["OPENCV_IO_ENABLE_OPENEXR"] = "1"
 import cv2
-import numpy as np
 import glm
+import numpy as np
 from OpenGL import GL
 import OpenGL.GL.ARB.bindless_texture as bt
 
 from .FBOAttachment import FBOAttachment
 from .GLInfo import GLInfo
 from .utils import checktype
 from .helper import get_dtype, get_channels, width_adapt, get_external_format
```

### Comparing `python_glass-0.1.54/glass/uimage2D.py` & `python_glass-0.1.55/glass/uimage2D.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .sampler2D import sampler2D
 from .GLInfo import GLInfo
 from .utils import checktype
 from .usampler2D import usampler2D
 
-import numpy as np
 from OpenGL import GL
+import numpy as np
 
 
 class uimage2D(usampler2D):
 
     _default_internal_format = GL.GL_RGBA32UI
     _default_filter_min = GL.GL_NEAREST
     _default_filter_mag = GL.GL_NEAREST
```

### Comparing `python_glass-0.1.54/glass/usampler2D.py` & `python_glass-0.1.55/glass/usampler2D.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .sampler2D import sampler2D
 from .GLInfo import GLInfo
 from .utils import checktype
 
-import numpy as np
 from OpenGL import GL
 import OpenGL.GL.ARB.bindless_texture as bt
+import numpy as np
 
 
 class usampler2D(sampler2D):
 
     _default_internal_format = GL.GL_RGBA32UI
     _default_filter_min = GL.GL_NEAREST
     _default_filter_mag = GL.GL_NEAREST
```

### Comparing `python_glass-0.1.54/glass/usampler2DMS.py` & `python_glass-0.1.55/glass/usampler2DMS.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/glass/utils.py` & `python_glass-0.1.55/glass/utils.py`

 * *Files identical despite different names*

### Comparing `python_glass-0.1.54/python_glass.egg-info/PKG-INFO` & `python_glass-0.1.55/python_glass.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python_glass
-Version: 0.1.54
+Version: 0.1.55
 Summary: OpenGL wrapper for Glass-Engine
 Home-page: https://github.com/Time-Coder/Glass-Engine
 Author: 王炳辉 (BingHui-WANG)
 Author-email: binghui.wang@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python_glass-0.1.54/python_glass.egg-info/SOURCES.txt` & `python_glass-0.1.55/python_glass.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -82,16 +82,14 @@
 glass/ShaderParser_/pcpp/ply/yacc.py
 glass/ShaderParser_/pcpp/ply/ygen.py
 glass/ShaderParser_/tree-sitter-glsl/README.md
 glass/ShaderParser_/tree-sitter-glsl/src.zip
 glass/ShaderParser_/tree-sitter-glsl/lib/AMD64/Windows/32bit/glsl.dll
 glass/ShaderParser_/tree-sitter-glsl/lib/AMD64/Windows/64bit/glsl.dll
 glass/ShaderParser_/tree-sitter-glsl/lib/x86_64/Linux/64bit/glsl.so
-glass/ShaderParser_/tree-sitter-glsl/src/parser.c
-glass/ShaderParser_/tree-sitter-glsl/src/tree_sitter/parser.h
 glass/__pyinstaller/__init__.py
 glass/__pyinstaller/hook-glass.py
 glass/glsl/draw_frame.vs
 glass/glsl/shadertoy_template.fs
 python_glass.egg-info/PKG-INFO
 python_glass.egg-info/SOURCES.txt
 python_glass.egg-info/dependency_links.txt
```

### Comparing `python_glass-0.1.54/setup.py` & `python_glass-0.1.55/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 extra_files += find_files("glass", "glass/ShaderParser_/tree-sitter-glsl")
 
 with open("glass/README_PYPI.md", "r", encoding='utf-8') as in_file:
     long_description = in_file.read()
 
 setuptools.setup(
     name="python_glass",
-    version="0.1.54",
+    version="0.1.55",
     author="王炳辉 (BingHui-WANG)",
     author_email="binghui.wang@foxmail.com",
     description="OpenGL wrapper for Glass-Engine",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Time-Coder/Glass-Engine",
     packages=setuptools.find_packages(exclude=['*glass_engine*', '*assimpy*']),
```


# Comparing `tmp/glass_engine-0.1.8.tar.gz` & `tmp/glass_engine-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glass_engine-0.1.8.tar", last modified: Sat Oct  7 14:07:38 2023, max compression
+gzip compressed data, was "glass_engine-0.1.9.tar", last modified: Sat Oct  7 14:23:33 2023, max compression
```

## Comparing `glass_engine-0.1.8.tar` & `glass_engine-0.1.9.tar`

### file list

```diff
@@ -1,313 +1,313 @@
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.905760 glass_engine-0.1.8/
--rw-rw-rw-   0        0        0     1082 2023-09-21 01:35:45.000000 glass_engine-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     3126 2023-10-07 14:07:38.904759 glass_engine-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2513 2023-10-07 11:44:15.000000 glass_engine-0.1.8/README.rst
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.062014 glass_engine-0.1.8/glass/
--rw-rw-rw-   0        0        0     1822 2023-08-27 13:23:22.000000 glass_engine-0.1.8/glass/ACBO.py
--rw-rw-rw-   0        0        0     3967 2023-09-22 12:23:56.000000 glass_engine-0.1.8/glass/AttrList.py
--rw-rw-rw-   0        0        0     8751 2023-09-22 11:12:35.000000 glass_engine-0.1.8/glass/BO.py
--rw-rw-rw-   0        0        0     4943 2023-08-28 03:35:09.000000 glass_engine-0.1.8/glass/Block.py
--rw-rw-rw-   0        0        0     4111 2023-09-22 12:32:47.000000 glass_engine-0.1.8/glass/CSRMat.py
--rw-rw-rw-   0        0        0     5134 2023-09-22 12:32:52.000000 glass_engine-0.1.8/glass/ComputeProgram.py
--rw-rw-rw-   0        0        0     5340 2023-09-22 12:24:53.000000 glass_engine-0.1.8/glass/DictList.py
--rw-rw-rw-   0        0        0      359 2023-07-12 03:51:26.000000 glass_engine-0.1.8/glass/EBO.py
--rw-rw-rw-   0        0        0    24712 2023-09-14 02:19:23.000000 glass_engine-0.1.8/glass/FBO.py
--rw-rw-rw-   0        0        0     3593 2023-09-22 11:53:18.000000 glass_engine-0.1.8/glass/FBOAttachment.py
--rw-rw-rw-   0        0        0    23953 2023-09-25 04:21:44.000000 glass_engine-0.1.8/glass/GLConfig.py
--rw-rw-rw-   0        0        0    25711 2023-09-22 11:12:38.000000 glass_engine-0.1.8/glass/GLInfo.py
--rw-rw-rw-   0        0        0     4497 2023-08-31 00:22:27.000000 glass_engine-0.1.8/glass/GLObject.py
--rw-rw-rw-   0        0        0    16769 2023-09-13 12:29:39.000000 glass_engine-0.1.8/glass/GPUProgram.py
--rw-rw-rw-   0        0        0     1417 2023-09-04 13:53:15.000000 glass_engine-0.1.8/glass/GlassConfig.py
--rw-rw-rw-   0        0        0     5192 2023-10-07 11:26:53.000000 glass_engine-0.1.8/glass/ImageLoader.py
--rw-rw-rw-   0        0        0     1705 2023-07-19 01:01:40.000000 glass_engine-0.1.8/glass/ImageUnits.py
--rw-rw-rw-   0        0        0     5469 2023-08-15 03:00:14.000000 glass_engine-0.1.8/glass/Increment.py
--rw-rw-rw-   0        0        0     3627 2023-08-13 15:33:49.000000 glass_engine-0.1.8/glass/Indices.py
--rw-rw-rw-   0        0        0     4543 2023-08-08 12:46:08.000000 glass_engine-0.1.8/glass/Instances.py
--rw-rw-rw-   0        0        0     2626 2023-08-09 01:59:26.000000 glass_engine-0.1.8/glass/RBO.py
--rw-rw-rw-   0        0        0     1381 2023-10-07 04:23:57.000000 glass_engine-0.1.8/glass/RenderHints.py
--rw-rw-rw-   0        0        0     2399 2023-07-12 03:52:09.000000 glass_engine-0.1.8/glass/SSBO.py
--rw-rw-rw-   0        0        0    27451 2023-08-22 08:26:27.000000 glass_engine-0.1.8/glass/SSUBO.py
--rw-rw-rw-   0        0        0    11786 2023-09-22 12:25:40.000000 glass_engine-0.1.8/glass/SameTypeList.py
--rw-rw-rw-   0        0        0    17767 2023-08-30 01:59:32.000000 glass_engine-0.1.8/glass/ShaderParser.py
--rw-rw-rw-   0        0        0    31959 2023-10-06 12:15:32.000000 glass_engine-0.1.8/glass/ShaderProgram.py
--rw-rw-rw-   0        0        0      787 2023-07-11 10:04:32.000000 glass_engine-0.1.8/glass/ShaderStorageBlock.py
--rw-rw-rw-   0        0        0    16500 2023-09-09 06:40:51.000000 glass_engine-0.1.8/glass/Shaders.py
--rw-rw-rw-   0        0        0     2009 2023-07-19 01:02:08.000000 glass_engine-0.1.8/glass/TextureUnits.py
--rw-rw-rw-   0        0        0      414 2023-07-12 03:52:14.000000 glass_engine-0.1.8/glass/UBO.py
--rw-rw-rw-   0        0        0    26296 2023-09-22 12:08:45.000000 glass_engine-0.1.8/glass/Uniform.py
--rw-rw-rw-   0        0        0      760 2023-08-08 12:54:43.000000 glass_engine-0.1.8/glass/UniformBlock.py
--rw-rw-rw-   0        0        0     3698 2023-09-22 12:07:29.000000 glass_engine-0.1.8/glass/VAO.py
--rw-rw-rw-   0        0        0      366 2023-07-12 03:52:29.000000 glass_engine-0.1.8/glass/VBO.py
--rw-rw-rw-   0        0        0    17438 2023-09-20 03:30:52.000000 glass_engine-0.1.8/glass/Vertices.py
--rw-rw-rw-   0        0        0     3082 2023-08-17 09:51:39.000000 glass_engine-0.1.8/glass/WeakDict.py
--rw-rw-rw-   0        0        0     1645 2023-08-17 09:40:26.000000 glass_engine-0.1.8/glass/WeakList.py
--rw-rw-rw-   0        0        0      670 2023-08-17 09:44:58.000000 glass_engine-0.1.8/glass/WeakRef.py
--rw-rw-rw-   0        0        0     2308 2023-08-17 09:41:15.000000 glass_engine-0.1.8/glass/WeakSet.py
--rw-rw-rw-   0        0        0     1110 2023-10-07 11:17:56.000000 glass_engine-0.1.8/glass/__init__.py
--rw-rw-rw-   0        0        0     1566 2023-10-07 11:27:55.000000 glass_engine-0.1.8/glass/download.py
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.067009 glass_engine-0.1.8/glass/glsl/
--rw-rw-rw-   0        0        0      201 2023-06-07 03:50:50.000000 glass_engine-0.1.8/glass/glsl/draw_frame.vs
--rw-rw-rw-   0        0        0      909 2023-08-25 14:34:49.000000 glass_engine-0.1.8/glass/glsl/shadertoy_template.glsl
--rw-rw-rw-   0        0        0     3620 2023-08-09 01:58:08.000000 glass_engine-0.1.8/glass/helper.py
--rw-rw-rw-   0        0        0     1769 2023-08-16 03:06:11.000000 glass_engine-0.1.8/glass/iimage2D.py
--rw-rw-rw-   0        0        0     1772 2023-08-16 03:10:26.000000 glass_engine-0.1.8/glass/image2D.py
--rw-rw-rw-   0        0        0     1396 2023-08-22 11:26:13.000000 glass_engine-0.1.8/glass/isampler2D.py
--rw-rw-rw-   0        0        0     1248 2023-08-22 11:25:55.000000 glass_engine-0.1.8/glass/isampler2DMS.py
--rw-rw-rw-   0        0        0    20950 2023-09-23 07:30:33.000000 glass_engine-0.1.8/glass/sampler2D.py
--rw-rw-rw-   0        0        0    16313 2023-08-15 15:22:30.000000 glass_engine-0.1.8/glass/sampler2DArray.py
--rw-rw-rw-   0        0        0     3316 2023-08-09 02:02:55.000000 glass_engine-0.1.8/glass/sampler2DMS.py
--rw-rw-rw-   0        0        0    12397 2023-08-09 02:04:02.000000 glass_engine-0.1.8/glass/samplerCube.py
--rw-rw-rw-   0        0        0     1770 2023-08-16 03:06:56.000000 glass_engine-0.1.8/glass/uimage2D.py
--rw-rw-rw-   0        0        0     1388 2023-08-22 11:26:31.000000 glass_engine-0.1.8/glass/usampler2D.py
--rw-rw-rw-   0        0        0     1243 2023-08-22 11:26:45.000000 glass_engine-0.1.8/glass/usampler2DMS.py
--rw-rw-rw-   0        0        0    18749 2023-10-07 11:16:40.000000 glass_engine-0.1.8/glass/utils.py
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.186682 glass_engine-0.1.8/glass_engine/
--rw-rw-rw-   0        0        0      680 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/AffineTransform.py
--rw-rw-rw-   0        0        0     1351 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Background.py
--rw-rw-rw-   0        0        0      990 2023-08-28 05:51:39.000000 glass_engine-0.1.8/glass_engine/BasicScene.py
--rw-rw-rw-   0        0        0     8371 2023-10-07 11:12:42.000000 glass_engine-0.1.8/glass_engine/Camera.py
--rw-rw-rw-   0        0        0    11033 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/ColorMap.py
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.212611 glass_engine-0.1.8/glass_engine/Demos/
--rw-rw-rw-   0        0        0       22 2023-08-25 06:06:39.000000 glass_engine-0.1.8/glass_engine/Demos/__init__.py
--rw-rw-rw-   0        0        0      120 2023-08-25 06:04:52.000000 glass_engine-0.1.8/glass_engine/Demos/demo.py
--rw-rw-rw-   0        0        0     9871 2023-10-07 14:04:33.000000 glass_engine-0.1.8/glass_engine/Demos/demo_transform.py
--rw-rw-rw-   0        0        0     2721 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Fog.py
--rw-rw-rw-   0        0        0     2635 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Frame.py
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.385151 glass_engine-0.1.8/glass_engine/Geometries/
--rw-rw-rw-   0        0        0    10002 2023-09-22 14:59:17.000000 glass_engine-0.1.8/glass_engine/Geometries/Box.py
--rw-rw-rw-   0        0        0     3015 2023-10-07 04:24:13.000000 glass_engine-0.1.8/glass_engine/Geometries/Circle.py
--rw-rw-rw-   0        0        0     4189 2023-09-22 14:59:17.000000 glass_engine-0.1.8/glass_engine/Geometries/CircleFace.py
--rw-rw-rw-   0        0        0     5390 2023-09-22 14:59:17.000000 glass_engine-0.1.8/glass_engine/Geometries/Cone.py
--rw-rw-rw-   0        0        0     4158 2023-09-22 14:59:17.000000 glass_engine-0.1.8/glass_engine/Geometries/ConeSide.py
--rw-rw-rw-   0        0        0     8113 2023-09-22 14:59:17.000000 glass_engine-0.1.8/glass_engine/Geometries/ConeTrustum.py
--rw-rw-rw-   0        0        0     5631 2023-09-22 14:59:17.000000 glass_engine-0.1.8/glass_engine/Geometries/ConeTrustumSide.py
--rw-rw-rw-   0        0        0     1066 2023-08-25 14:26:02.000000 glass_engine-0.1.8/glass_engine/Geometries/CoordSys.py
--rw-rw-rw-   0        0        0     6408 2023-09-22 14:59:17.000000 glass_engine-0.1.8/glass_engine/Geometries/Cylinder.py
--rw-rw-rw-   0        0        0     4228 2023-09-22 14:59:17.000000 glass_engine-0.1.8/glass_engine/Geometries/CylinderSide.py
--rw-rw-rw-   0        0        0     2794 2023-09-22 14:59:17.000000 glass_engine-0.1.8/glass_engine/Geometries/CylindricalFSurf.py
--rw-rw-rw-   0        0        0     6962 2023-09-22 14:59:17.000000 glass_engine-0.1.8/glass_engine/Geometries/Dodecahedron.py
--rw-rw-rw-   0        0        0     4489 2023-09-22 14:59:17.000000 glass_engine-0.1.8/glass_engine/Geometries/EllipseFace.py
--rw-rw-rw-   0        0        0    24519 2023-09-22 14:59:17.000000 glass_engine-0.1.8/glass_engine/Geometries/Extruder.py
--rw-rw-rw-   0        0        0     3788 2023-09-22 14:59:17.000000 glass_engine-0.1.8/glass_engine/Geometries/FSurf.py
--rw-rw-rw-   0        0        0     3179 2023-09-22 14:59:17.000000 glass_engine-0.1.8/glass_engine/Geometries/Floor.py
--rw-rw-rw-   0        0        0     4072 2023-09-22 14:59:17.000000 glass_engine-0.1.8/glass_engine/Geometries/Hexahedron.py
--rw-rw-rw-   0        0        0     5289 2023-09-22 14:59:17.000000 glass_engine-0.1.8/glass_engine/Geometries/HollowRPolygonFace.py
--rw-rw-rw-   0        0        0     5005 2023-09-22 14:59:17.000000 glass_engine-0.1.8/glass_engine/Geometries/Icosahedron.py
--rw-rw-rw-   0        0        0     8078 2023-09-22 14:59:17.000000 glass_engine-0.1.8/glass_engine/Geometries/Icosphere.py
--rw-rw-rw-   0        0        0     4529 2023-09-22 14:59:17.000000 glass_engine-0.1.8/glass_engine/Geometries/ImageQuad.py
--rw-rw-rw-   0        0        0     4088 2023-09-22 14:59:17.000000 glass_engine-0.1.8/glass_engine/Geometries/Octahedron.py
--rw-rw-rw-   0        0        0     1155 2023-10-07 04:24:13.000000 glass_engine-0.1.8/glass_engine/Geometries/Point.py
--rw-rw-rw-   0        0        0     1357 2023-10-07 04:24:13.000000 glass_engine-0.1.8/glass_engine/Geometries/Points.py
--rw-rw-rw-   0        0        0     1972 2023-10-07 04:24:13.000000 glass_engine-0.1.8/glass_engine/Geometries/Polyline.py
--rw-rw-rw-   0        0        0     7261 2023-09-22 14:59:17.000000 glass_engine-0.1.8/glass_engine/Geometries/Prism.py
--rw-rw-rw-   0        0        0     5078 2023-09-22 14:59:17.000000 glass_engine-0.1.8/glass_engine/Geometries/PrismSide.py
--rw-rw-rw-   0        0        0     5764 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Geometries/Pyramid.py
--rw-rw-rw-   0        0        0     4581 2023-09-22 14:59:17.000000 glass_engine-0.1.8/glass_engine/Geometries/PyramidSide.py
--rw-rw-rw-   0        0        0     8523 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Geometries/PyramidTrustum.py
--rw-rw-rw-   0        0        0     6023 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Geometries/PyramidTrustumSide.py
--rw-rw-rw-   0        0        0     4055 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Geometries/RPolygonFace.py
--rw-rw-rw-   0        0        0     3727 2023-09-27 07:04:21.000000 glass_engine-0.1.8/glass_engine/Geometries/RectFace.py
--rw-rw-rw-   0        0        0     6209 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Geometries/Rotator.py
--rw-rw-rw-   0        0        0     4535 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Geometries/Sphere.py
--rw-rw-rw-   0        0        0     5647 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Geometries/SphericalCap.py
--rw-rw-rw-   0        0        0     4502 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Geometries/SphericalCapTop.py
--rw-rw-rw-   0        0        0     2887 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Geometries/SphericalFSurf.py
--rw-rw-rw-   0        0        0     7270 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Geometries/Surf.py
--rw-rw-rw-   0        0        0     3488 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Geometries/Tetrahedron.py
--rw-rw-rw-   0        0        0     6030 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Geometries/Torus.py
--rw-rw-rw-   0        0        0     5405 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Geometries/TorusFace.py
--rw-rw-rw-   0        0        0     7108 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Geometries/TrefoilKnot.py
--rw-rw-rw-   0        0        0     1735 2023-09-27 07:04:43.000000 glass_engine-0.1.8/glass_engine/Geometries/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.400112 glass_engine-0.1.8/glass_engine/Lights/
--rw-rw-rw-   0        0        0     1346 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Lights/DirLight.py
--rw-rw-rw-   0        0        0     3529 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Lights/Light.py
--rw-rw-rw-   0        0        0     3719 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Lights/PointLight.py
--rw-rw-rw-   0        0        0     2991 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Lights/SpotLight.py
--rw-rw-rw-   0        0        0      100 2023-06-09 08:06:38.000000 glass_engine-0.1.8/glass_engine/Lights/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.414072 glass_engine-0.1.8/glass_engine/Manipulators/
--rw-rw-rw-   0        0        0    16527 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Manipulators/Manipulator.py
--rw-rw-rw-   0        0        0     8720 2023-10-07 04:24:13.000000 glass_engine-0.1.8/glass_engine/Manipulators/ModelViewManipulator.py
--rw-rw-rw-   0        0        0     7994 2023-10-07 04:24:13.000000 glass_engine-0.1.8/glass_engine/Manipulators/SceneRoamManipulator.py
--rw-rw-rw-   0        0        0      148 2023-06-09 08:07:20.000000 glass_engine-0.1.8/glass_engine/Manipulators/__init__.py
--rw-rw-rw-   0        0        0    33997 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Material.py
--rw-rw-rw-   0        0        0    29443 2023-10-07 04:25:57.000000 glass_engine-0.1.8/glass_engine/Mesh.py
--rw-rw-rw-   0        0        0    14936 2023-10-07 11:18:45.000000 glass_engine-0.1.8/glass_engine/Model.py
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.455960 glass_engine-0.1.8/glass_engine/PostProcessEffects/
--rw-rw-rw-   0        0        0      287 2023-09-11 03:30:22.000000 glass_engine-0.1.8/glass_engine/PostProcessEffects/ACESToneMapper.py
--rw-rw-rw-   0        0        0     6663 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/PostProcessEffects/BloomEffect.py
--rw-rw-rw-   0        0        0     4303 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/PostProcessEffects/DOFEffect.py
--rw-rw-rw-   0        0        0     1754 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/PostProcessEffects/ExplosureAdaptor.py
--rw-rw-rw-   0        0        0     4138 2023-10-07 05:00:54.000000 glass_engine-0.1.8/glass_engine/PostProcessEffects/FXAAEffect.py
--rw-rw-rw-   0        0        0    10800 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/PostProcessEffects/GaussBlur.py
--rw-rw-rw-   0        0        0     5775 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/PostProcessEffects/KernelFilter.py
--rw-rw-rw-   0        0        0     1478 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/PostProcessEffects/LUTEffect.py
--rw-rw-rw-   0        0        0      284 2023-09-12 02:12:58.000000 glass_engine-0.1.8/glass_engine/PostProcessEffects/MedianBlur.py
--rw-rw-rw-   0        0        0      276 2023-09-12 02:50:36.000000 glass_engine-0.1.8/glass_engine/PostProcessEffects/MulFilter.py
--rw-rw-rw-   0        0        0     1423 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/PostProcessEffects/PostProcessEffect.py
--rw-rw-rw-   0        0        0     3495 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/PostProcessEffects/PostProcessEffects.py
--rw-rw-rw-   0        0        0     2427 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/PostProcessEffects/SSAOEffect.py
--rw-rw-rw-   0        0        0     6646 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/PostProcessEffects/ShaderEffect.py
--rw-rw-rw-   0        0        0      520 2023-10-07 04:57:50.000000 glass_engine-0.1.8/glass_engine/PostProcessEffects/__init__.py
--rw-rw-rw-   0        0        0     2597 2023-10-07 11:48:12.000000 glass_engine-0.1.8/glass_engine/README_PYPI.md
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.471919 glass_engine-0.1.8/glass_engine/Renderers/
--rw-rw-rw-   0        0        0    47076 2023-10-07 04:59:21.000000 glass_engine-0.1.8/glass_engine/Renderers/CommonRenderer.py
--rw-rw-rw-   0        0        0    11866 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Renderers/DeferredRenderer.py
--rw-rw-rw-   0        0        0     2427 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Renderers/ForwardRenderer.py
--rw-rw-rw-   0        0        0      426 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Renderers/Renderer.py
--rw-rw-rw-   0        0        0      124 2023-06-19 05:45:46.000000 glass_engine-0.1.8/glass_engine/Renderers/__init__.py
--rw-rw-rw-   0        0        0    11431 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/Scene.py
--rw-rw-rw-   0        0        0    15984 2023-10-06 12:05:43.000000 glass_engine-0.1.8/glass_engine/SceneNode.py
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.497851 glass_engine-0.1.8/glass_engine/Screens/
--rw-rw-rw-   0        0        0     1065 2023-10-07 07:02:07.000000 glass_engine-0.1.8/glass_engine/Screens/PyQt5Screen.py
--rw-rw-rw-   0        0        0     1077 2023-10-07 07:23:24.000000 glass_engine-0.1.8/glass_engine/Screens/PyQt6Screen.py
--rw-rw-rw-   0        0        0     1069 2023-10-07 07:13:58.000000 glass_engine-0.1.8/glass_engine/Screens/PySide2Screen.py
--rw-rw-rw-   0        0        0     1069 2023-10-07 06:50:15.000000 glass_engine-0.1.8/glass_engine/Screens/PySide6Screen.py
--rw-rw-rw-   0        0        0    24595 2023-10-07 14:02:09.000000 glass_engine-0.1.8/glass_engine/Screens/QtScreen.py
--rw-rw-rw-   0        0        0        0 2023-10-07 12:29:23.000000 glass_engine-0.1.8/glass_engine/Screens/__init__.py
--rw-rw-rw-   0        0        0     4728 2023-10-07 04:24:13.000000 glass_engine-0.1.8/glass_engine/SkyBox.py
--rw-rw-rw-   0        0        0     4473 2023-10-07 04:24:12.000000 glass_engine-0.1.8/glass_engine/SkyDome.py
--rw-rw-rw-   0        0        0      750 2023-10-01 13:40:34.000000 glass_engine-0.1.8/glass_engine/SlideAverageFilter.py
--rw-rw-rw-   0        0        0     3553 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/VideoRecorder.py
--rw-rw-rw-   0        0        0     2458 2023-07-15 11:51:51.000000 glass_engine-0.1.8/glass_engine/WeightedIntegrator.py
--rw-rw-rw-   0        0        0      337 2023-10-07 07:22:21.000000 glass_engine-0.1.8/glass_engine/__init__.py
--rw-rw-rw-   0        0        0    15347 2023-09-22 14:59:15.000000 glass_engine-0.1.8/glass_engine/algorithm.py
--rw-rw-rw-   0        0        0     2144 2023-09-19 09:43:51.000000 glass_engine-0.1.8/glass_engine/callback_vec.py
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:37.864542 glass_engine-0.1.8/glass_engine/glsl/
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.520787 glass_engine-0.1.8/glass_engine/glsl/Lights/
--rw-rw-rw-   0        0        0     2948 2023-09-18 02:29:54.000000 glass_engine-0.1.8/glass_engine/glsl/Lights/DirLight.glsl
--rw-rw-rw-   0        0        0     5447 2023-09-19 12:18:26.000000 glass_engine-0.1.8/glass_engine/glsl/Lights/DirLight_shadow_mapping.glsl
--rw-rw-rw-   0        0        0     2958 2023-09-18 03:02:53.000000 glass_engine-0.1.8/glass_engine/glsl/Lights/Lights.glsl
--rw-rw-rw-   0        0        0     3730 2023-09-18 02:29:47.000000 glass_engine-0.1.8/glass_engine/glsl/Lights/PointLight.glsl
--rw-rw-rw-   0        0        0     2131 2023-09-06 05:17:49.000000 glass_engine-0.1.8/glass_engine/glsl/Lights/PointLight_shadow_mapping.glsl
--rw-rw-rw-   0        0        0     4439 2023-09-18 02:30:02.000000 glass_engine-0.1.8/glass_engine/glsl/Lights/SpotLight.glsl
--rw-rw-rw-   0        0        0     2627 2023-09-06 05:17:58.000000 glass_engine-0.1.8/glass_engine/glsl/Lights/SpotLight_shadow_mapping.glsl
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.537743 glass_engine-0.1.8/glass_engine/glsl/Pipelines/
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.554697 glass_engine-0.1.8/glass_engine/glsl/Pipelines/DirLight_depth/
--rw-rw-rw-   0        0        0      637 2023-09-02 13:21:30.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/DirLight_depth/DirLight_depth.fs
--rw-rw-rw-   0        0        0     1284 2023-09-02 12:57:44.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/DirLight_depth/DirLight_depth.gs
--rw-rw-rw-   0        0        0     1077 2023-09-07 04:19:48.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/DirLight_depth/DirLight_depth.vs
--rw-rw-rw-   0        0        0      967 2023-09-02 13:01:18.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/DirLight_depth/DirLight_depth_lines.gs
--rw-rw-rw-   0        0        0      891 2023-09-02 13:08:46.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/DirLight_depth/DirLight_depth_points.gs
--rw-rw-rw-   0        0        0      375 2023-07-27 08:40:27.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/OIT_blend.fs
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.573646 glass_engine-0.1.8/glass_engine/glsl/Pipelines/PointLight_depth/
--rw-rw-rw-   0        0        0      926 2023-09-02 13:21:41.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/PointLight_depth/PointLight_depth.fs
--rw-rw-rw-   0        0        0     1346 2023-09-07 11:35:41.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/PointLight_depth/PointLight_depth.gs
--rw-rw-rw-   0        0        0     1035 2023-09-07 04:24:02.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/PointLight_depth/PointLight_depth.vs
--rw-rw-rw-   0        0        0     1064 2023-09-07 11:36:44.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/PointLight_depth/PointLight_depth_lines.gs
--rw-rw-rw-   0        0        0      986 2023-09-07 11:36:36.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/PointLight_depth/PointLight_depth_points.gs
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.588605 glass_engine-0.1.8/glass_engine/glsl/Pipelines/SpotLight_depth/
--rw-rw-rw-   0        0        0      921 2023-09-07 12:35:57.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/SpotLight_depth/SpotLight_depth.fs
--rw-rw-rw-   0        0        0     1339 2023-09-07 11:35:58.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/SpotLight_depth/SpotLight_depth.gs
--rw-rw-rw-   0        0        0     1059 2023-09-07 11:36:21.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/SpotLight_depth/SpotLight_depth_lines.gs
--rw-rw-rw-   0        0        0      981 2023-09-07 11:36:11.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/SpotLight_depth/SpotLight_depth_points.gs
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.605565 glass_engine-0.1.8/glass_engine/glsl/Pipelines/deferred_rendering/
--rw-rw-rw-   0        0        0     1292 2023-09-18 05:04:16.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/deferred_rendering/deferred_rendering.fs
--rw-rw-rw-   0        0        0     1976 2023-09-12 06:54:50.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/deferred_rendering/draw_points_to_gbuffer.fs
--rw-rw-rw-   0        0        0     2451 2023-09-12 06:54:22.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/deferred_rendering/draw_to_gbuffer.fs
--rw-rw-rw-   0        0        0     4196 2023-09-15 06:39:26.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/deferred_rendering/read_from_gbuffer.glsl
--rw-rw-rw-   0        0        0     2733 2023-09-15 06:39:46.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/deferred_rendering/write_to_gbuffer.glsl
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.619524 glass_engine-0.1.8/glass_engine/glsl/Pipelines/draw_TBN/
--rw-rw-rw-   0        0        0     1382 2023-09-07 04:20:28.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/draw_TBN/draw_TBN.vs
--rw-rw-rw-   0        0        0      879 2023-07-05 08:14:07.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/draw_TBN/draw_bitangent.gs
--rw-rw-rw-   0        0        0      878 2023-07-05 08:14:03.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/draw_TBN/draw_normal.gs
--rw-rw-rw-   0        0        0      874 2023-07-05 08:14:00.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/draw_TBN/draw_tangent.gs
--rw-rw-rw-   0        0        0      738 2023-09-04 05:07:22.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/draw_frame.fs
--rw-rw-rw-   0        0        0      236 2023-07-27 09:10:55.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/draw_frame.vs
--rw-rw-rw-   0        0        0      457 2023-07-27 08:28:26.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/draw_frame_array.gs
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.640468 glass_engine-0.1.8/glass_engine/glsl/Pipelines/draw_geometry/
--rw-rw-rw-   0        0        0     1415 2023-09-12 01:24:06.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/draw_geometry/draw_geometry.fs
--rw-rw-rw-   0        0        0     3365 2023-09-12 01:26:59.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/draw_geometry/draw_geometry.gs
--rw-rw-rw-   0        0        0     1508 2023-09-12 01:28:54.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/draw_geometry/draw_geometry.vs
--rw-rw-rw-   0        0        0     1618 2023-09-12 01:09:23.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/draw_geometry/draw_geometry_lines.vs
--rw-rw-rw-   0        0        0      848 2023-09-12 01:24:34.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/draw_geometry/draw_geometry_points.fs
--rw-rw-rw-   0        0        0     1361 2023-09-12 01:28:46.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/draw_geometry/draw_geometry_points.vs
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.669389 glass_engine-0.1.8/glass_engine/glsl/Pipelines/env_mapping/
--rw-rw-rw-   0        0        0     1099 2023-09-04 05:42:27.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/env_mapping/env_OIT_blend.fs
--rw-rw-rw-   0        0        0     1688 2023-09-18 05:09:30.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/env_mapping/gen_env_map.fs
--rw-rw-rw-   0        0        0     5783 2023-09-12 03:00:10.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/env_mapping/gen_env_map.gs
--rw-rw-rw-   0        0        0     1459 2023-09-07 04:25:37.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/env_mapping/gen_env_map.vs
--rw-rw-rw-   0        0        0     2368 2023-09-12 03:01:41.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/env_mapping/gen_env_map_lines.gs
--rw-rw-rw-   0        0        0     1573 2023-09-27 05:47:51.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/env_mapping/gen_env_map_points.fs
--rw-rw-rw-   0        0        0     1974 2023-09-12 02:59:59.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/env_mapping/gen_env_map_points.gs
--rw-rw-rw-   0        0        0     1099 2023-09-07 04:21:13.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/env_mapping/gen_env_map_points.vs
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.697315 glass_engine-0.1.8/glass_engine/glsl/Pipelines/forward_rendering/
--rw-rw-rw-   0        0        0     2279 2023-09-12 03:00:21.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/forward_rendering/forward_draw_lines.vs
--rw-rw-rw-   0        0        0     1655 2023-09-27 05:43:51.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/forward_rendering/forward_draw_points.fs
--rw-rw-rw-   0        0        0     2016 2023-09-12 03:00:42.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/forward_rendering/forward_draw_points.vs
--rw-rw-rw-   0        0        0     1802 2023-09-19 09:22:13.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/forward_rendering/forward_rendering.fs
--rw-rw-rw-   0        0        0     5569 2023-09-12 03:01:03.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/forward_rendering/forward_rendering.gs
--rw-rw-rw-   0        0        0     1610 2023-09-07 04:23:33.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/forward_rendering/forward_rendering.vs
--rw-rw-rw-   0        0        0      324 2023-07-05 08:09:43.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/single_color.fs
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.704315 glass_engine-0.1.8/glass_engine/glsl/Pipelines/skybox/
--rw-rw-rw-   0        0        0      629 2023-09-20 01:23:35.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/skybox/skybox.fs
--rw-rw-rw-   0        0        0      450 2023-09-20 01:22:44.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/skybox/skybox.vs
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.711283 glass_engine-0.1.8/glass_engine/glsl/Pipelines/skydome/
--rw-rw-rw-   0        0        0      645 2023-09-20 01:26:33.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/skydome/skydome.fs
--rw-rw-rw-   0        0        0      433 2023-09-20 01:26:04.000000 glass_engine-0.1.8/glass_engine/glsl/Pipelines/skydome/skydome.vs
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.792061 glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/
--rw-rw-rw-   0        0        0     1677 2023-09-21 14:10:44.000000 glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/ACES_tone_mapper.glsl
--rw-rw-rw-   0        0        0      293 2023-09-04 06:04:10.000000 glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/FXAA.fs
--rw-rw-rw-   0        0        0      314 2023-09-04 05:56:42.000000 glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/FXAA_array.fs
--rw-rw-rw-   0        0        0      313 2023-09-04 05:58:59.000000 glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/FXAA_cube.fs
--rw-rw-rw-   0        0        0     2351 2023-09-21 14:10:44.000000 glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/SSAO_visibility.glsl
--rw-rw-rw-   0        0        0     2639 2023-09-12 08:48:17.000000 glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/bloom_downsampling.fs
--rw-rw-rw-   0        0        0      405 2023-09-04 04:59:59.000000 glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/bloom_mix.fs
--rw-rw-rw-   0        0        0     1647 2023-09-11 02:20:37.000000 glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/bloom_upsampling.fs
--rw-rw-rw-   0        0        0     3374 2023-09-20 01:14:35.000000 glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/dof.fs
--rw-rw-rw-   0        0        0     1779 2023-09-21 14:10:44.000000 glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/explosure_adaptor.glsl
--rw-rw-rw-   0        0        0     1919 2023-09-12 02:57:38.000000 glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/gauss_blur.fs
--rw-rw-rw-   0        0        0     1920 2023-09-12 02:57:53.000000 glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/gauss_blur_array.fs
--rw-rw-rw-   0        0        0     1927 2023-09-12 02:57:45.000000 glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/gauss_blur_cube.fs
--rw-rw-rw-   0        0        0      932 2023-09-12 02:57:00.000000 glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/kernel_filter.fs
--rw-rw-rw-   0        0        0      989 2023-09-12 02:57:24.000000 glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/kernel_filter_array.fs
--rw-rw-rw-   0        0        0      988 2023-09-12 02:57:11.000000 glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/kernel_filter_cube.fs
--rw-rw-rw-   0        0        0     1499 2023-09-21 14:10:45.000000 glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/lut.glsl
--rw-rw-rw-   0        0        0     1276 2023-09-21 14:10:44.000000 glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/median_gray_blur5.glsl
--rw-rw-rw-   0        0        0      397 2023-09-21 14:10:44.000000 glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/mul_filter.glsl
--rw-rw-rw-   0        0        0     1968 2023-09-21 14:10:44.000000 glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/shader_effect_template.glsl
--rw-rw-rw-   0        0        0      666 2023-09-21 14:10:44.000000 glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/slit_stretch.glsl
--rw-rw-rw-   0        0        0     1590 2023-09-21 14:10:44.000000 glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/star_field.glsl
--rw-rw-rw-   0        0        0      239 2023-09-21 14:10:44.000000 glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/water_wave.glsl
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.822978 glass_engine-0.1.8/glass_engine/glsl/ShadingModels/
--rw-rw-rw-   0        0        0     1553 2023-09-18 01:27:21.000000 glass_engine-0.1.8/glass_engine/glsl/ShadingModels/CookTorrance.glsl
--rw-rw-rw-   0        0        0      477 2023-09-18 01:27:27.000000 glass_engine-0.1.8/glass_engine/glsl/ShadingModels/Flat.glsl
--rw-rw-rw-   0        0        0      453 2023-09-18 01:27:40.000000 glass_engine-0.1.8/glass_engine/glsl/ShadingModels/Fresnel.glsl
--rw-rw-rw-   0        0        0      263 2023-08-24 02:34:04.000000 glass_engine-0.1.8/glass_engine/glsl/ShadingModels/Gouraud.glsl
--rw-rw-rw-   0        0        0      567 2023-09-18 01:27:47.000000 glass_engine-0.1.8/glass_engine/glsl/ShadingModels/Lambert.glsl
--rw-rw-rw-   0        0        0     1107 2023-09-20 11:03:01.000000 glass_engine-0.1.8/glass_engine/glsl/ShadingModels/Minnaert.glsl
--rw-rw-rw-   0        0        0     1976 2023-09-20 08:41:58.000000 glass_engine-0.1.8/glass_engine/glsl/ShadingModels/OrenNayar.glsl
--rw-rw-rw-   0        0        0      862 2023-09-18 01:27:08.000000 glass_engine-0.1.8/glass_engine/glsl/ShadingModels/Phong.glsl
--rw-rw-rw-   0        0        0      885 2023-09-18 01:28:12.000000 glass_engine-0.1.8/glass_engine/glsl/ShadingModels/PhongBlinn.glsl
--rw-rw-rw-   0        0        0     1064 2023-09-20 13:43:52.000000 glass_engine-0.1.8/glass_engine/glsl/ShadingModels/Toon.glsl
--rw-rw-rw-   0        0        0     1376 2023-08-28 08:32:31.000000 glass_engine-0.1.8/glass_engine/glsl/ShadingModels/lighting.glsl
--rw-rw-rw-   0        0        0      503 2023-08-28 08:35:59.000000 glass_engine-0.1.8/glass_engine/glsl/ShadingModels/rim.glsl
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.877836 glass_engine-0.1.8/glass_engine/glsl/include/
--rw-rw-rw-   0        0        0     6873 2023-09-20 01:20:38.000000 glass_engine-0.1.8/glass_engine/glsl/include/Camera.glsl
--rw-rw-rw-   0        0        0    12032 2023-09-04 06:06:21.000000 glass_engine-0.1.8/glass_engine/glsl/include/FXAA.glsl
--rw-rw-rw-   0        0        0     2141 2023-09-04 12:18:59.000000 glass_engine-0.1.8/glass_engine/glsl/include/FresnelRefract.glsl
--rw-rw-rw-   0        0        0     8532 2023-09-23 01:42:20.000000 glass_engine-0.1.8/glass_engine/glsl/include/Material.glsl
--rw-rw-rw-   0        0        0     1113 2023-07-03 04:27:35.000000 glass_engine-0.1.8/glass_engine/glsl/include/OIT.glsl
--rw-rw-rw-   0        0        0     1160 2023-09-18 05:01:49.000000 glass_engine-0.1.8/glass_engine/glsl/include/ShadingInfo.glsl
--rw-rw-rw-   0        0        0      187 2023-09-18 04:59:12.000000 glass_engine-0.1.8/glass_engine/glsl/include/background.glsl
--rw-rw-rw-   0        0        0     9495 2023-09-18 05:16:28.000000 glass_engine-0.1.8/glass_engine/glsl/include/env_mapping.glsl
--rw-rw-rw-   0        0        0     1151 2023-09-18 04:46:59.000000 glass_engine-0.1.8/glass_engine/glsl/include/fog.glsl
--rw-rw-rw-   0        0        0     2322 2023-08-16 02:37:59.000000 glass_engine-0.1.8/glass_engine/glsl/include/image_read_write.glsl
--rw-rw-rw-   0        0        0    12066 2023-09-20 13:28:40.000000 glass_engine-0.1.8/glass_engine/glsl/include/math.glsl
--rw-rw-rw-   0        0        0     4011 2023-09-11 04:57:47.000000 glass_engine-0.1.8/glass_engine/glsl/include/parallax_mapping.glsl
--rw-rw-rw-   0        0        0     1922 2023-06-13 08:24:20.000000 glass_engine-0.1.8/glass_engine/glsl/include/quat.glsl
--rw-rw-rw-   0        0        0     4749 2023-09-11 04:47:49.000000 glass_engine-0.1.8/glass_engine/glsl/include/sampling.glsl
--rw-rw-rw-   0        0        0     4742 2023-09-18 05:16:45.000000 glass_engine-0.1.8/glass_engine/glsl/include/shading_all.glsl
--rw-rw-rw-   0        0        0     1997 2023-09-05 02:15:38.000000 glass_engine-0.1.8/glass_engine/glsl/include/transform.glsl
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.902766 glass_engine-0.1.8/glass_engine/images/
--rw-rw-rw-   0        0        0   100665 2023-09-19 08:50:53.000000 glass_engine-0.1.8/glass_engine/images/glass_engine_logo256.png
--rw-rw-rw-   0        0        0    11211 2023-09-19 08:52:07.000000 glass_engine-0.1.8/glass_engine/images/glass_engine_logo64.png
--rw-rw-rw-   0        0        0    41344 2023-09-21 10:19:41.000000 glass_engine-0.1.8/glass_engine/images/start.png
--rw-rw-rw-   0        0        0     4121 2023-09-09 06:26:47.000000 glass_engine-0.1.8/glass_engine/lut.py
-drwxrwxrwx   0        0        0        0 2023-10-07 14:07:38.202639 glass_engine-0.1.8/glass_engine.egg-info/
--rw-rw-rw-   0        0        0     3126 2023-10-07 14:07:36.000000 glass_engine-0.1.8/glass_engine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11058 2023-10-07 14:07:37.000000 glass_engine-0.1.8/glass_engine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-07 14:07:36.000000 glass_engine-0.1.8/glass_engine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      141 2023-10-07 14:07:36.000000 glass_engine-0.1.8/glass_engine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-10-07 14:07:36.000000 glass_engine-0.1.8/glass_engine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-07 14:07:38.905760 glass_engine-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     2048 2023-10-07 14:06:01.000000 glass_engine-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:33.272184 glass_engine-0.1.9/
+-rw-rw-rw-   0        0        0     1082 2023-09-21 01:35:45.000000 glass_engine-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     3126 2023-10-07 14:23:33.271199 glass_engine-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2513 2023-10-07 11:44:15.000000 glass_engine-0.1.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:32.499251 glass_engine-0.1.9/glass/
+-rw-rw-rw-   0        0        0     1822 2023-08-27 13:23:22.000000 glass_engine-0.1.9/glass/ACBO.py
+-rw-rw-rw-   0        0        0     3967 2023-09-22 12:23:56.000000 glass_engine-0.1.9/glass/AttrList.py
+-rw-rw-rw-   0        0        0     8751 2023-09-22 11:12:35.000000 glass_engine-0.1.9/glass/BO.py
+-rw-rw-rw-   0        0        0     4943 2023-08-28 03:35:09.000000 glass_engine-0.1.9/glass/Block.py
+-rw-rw-rw-   0        0        0     4111 2023-09-22 12:32:47.000000 glass_engine-0.1.9/glass/CSRMat.py
+-rw-rw-rw-   0        0        0     5134 2023-09-22 12:32:52.000000 glass_engine-0.1.9/glass/ComputeProgram.py
+-rw-rw-rw-   0        0        0     5340 2023-09-22 12:24:53.000000 glass_engine-0.1.9/glass/DictList.py
+-rw-rw-rw-   0        0        0      359 2023-07-12 03:51:26.000000 glass_engine-0.1.9/glass/EBO.py
+-rw-rw-rw-   0        0        0    24712 2023-09-14 02:19:23.000000 glass_engine-0.1.9/glass/FBO.py
+-rw-rw-rw-   0        0        0     3593 2023-09-22 11:53:18.000000 glass_engine-0.1.9/glass/FBOAttachment.py
+-rw-rw-rw-   0        0        0    23953 2023-09-25 04:21:44.000000 glass_engine-0.1.9/glass/GLConfig.py
+-rw-rw-rw-   0        0        0    25711 2023-09-22 11:12:38.000000 glass_engine-0.1.9/glass/GLInfo.py
+-rw-rw-rw-   0        0        0     4497 2023-08-31 00:22:27.000000 glass_engine-0.1.9/glass/GLObject.py
+-rw-rw-rw-   0        0        0    16769 2023-09-13 12:29:39.000000 glass_engine-0.1.9/glass/GPUProgram.py
+-rw-rw-rw-   0        0        0     1384 2023-10-07 14:19:54.000000 glass_engine-0.1.9/glass/GlassConfig.py
+-rw-rw-rw-   0        0        0     5192 2023-10-07 11:26:53.000000 glass_engine-0.1.9/glass/ImageLoader.py
+-rw-rw-rw-   0        0        0     1705 2023-07-19 01:01:40.000000 glass_engine-0.1.9/glass/ImageUnits.py
+-rw-rw-rw-   0        0        0     5469 2023-08-15 03:00:14.000000 glass_engine-0.1.9/glass/Increment.py
+-rw-rw-rw-   0        0        0     3627 2023-08-13 15:33:49.000000 glass_engine-0.1.9/glass/Indices.py
+-rw-rw-rw-   0        0        0     4543 2023-08-08 12:46:08.000000 glass_engine-0.1.9/glass/Instances.py
+-rw-rw-rw-   0        0        0     2626 2023-08-09 01:59:26.000000 glass_engine-0.1.9/glass/RBO.py
+-rw-rw-rw-   0        0        0     1381 2023-10-07 04:23:57.000000 glass_engine-0.1.9/glass/RenderHints.py
+-rw-rw-rw-   0        0        0     2399 2023-07-12 03:52:09.000000 glass_engine-0.1.9/glass/SSBO.py
+-rw-rw-rw-   0        0        0    27451 2023-08-22 08:26:27.000000 glass_engine-0.1.9/glass/SSUBO.py
+-rw-rw-rw-   0        0        0    11786 2023-09-22 12:25:40.000000 glass_engine-0.1.9/glass/SameTypeList.py
+-rw-rw-rw-   0        0        0    17767 2023-08-30 01:59:32.000000 glass_engine-0.1.9/glass/ShaderParser.py
+-rw-rw-rw-   0        0        0    31959 2023-10-06 12:15:32.000000 glass_engine-0.1.9/glass/ShaderProgram.py
+-rw-rw-rw-   0        0        0      787 2023-07-11 10:04:32.000000 glass_engine-0.1.9/glass/ShaderStorageBlock.py
+-rw-rw-rw-   0        0        0    16500 2023-09-09 06:40:51.000000 glass_engine-0.1.9/glass/Shaders.py
+-rw-rw-rw-   0        0        0     2009 2023-07-19 01:02:08.000000 glass_engine-0.1.9/glass/TextureUnits.py
+-rw-rw-rw-   0        0        0      414 2023-07-12 03:52:14.000000 glass_engine-0.1.9/glass/UBO.py
+-rw-rw-rw-   0        0        0    26296 2023-09-22 12:08:45.000000 glass_engine-0.1.9/glass/Uniform.py
+-rw-rw-rw-   0        0        0      760 2023-08-08 12:54:43.000000 glass_engine-0.1.9/glass/UniformBlock.py
+-rw-rw-rw-   0        0        0     3698 2023-09-22 12:07:29.000000 glass_engine-0.1.9/glass/VAO.py
+-rw-rw-rw-   0        0        0      366 2023-07-12 03:52:29.000000 glass_engine-0.1.9/glass/VBO.py
+-rw-rw-rw-   0        0        0    17438 2023-09-20 03:30:52.000000 glass_engine-0.1.9/glass/Vertices.py
+-rw-rw-rw-   0        0        0     3082 2023-08-17 09:51:39.000000 glass_engine-0.1.9/glass/WeakDict.py
+-rw-rw-rw-   0        0        0     1645 2023-08-17 09:40:26.000000 glass_engine-0.1.9/glass/WeakList.py
+-rw-rw-rw-   0        0        0      670 2023-08-17 09:44:58.000000 glass_engine-0.1.9/glass/WeakRef.py
+-rw-rw-rw-   0        0        0     2308 2023-08-17 09:41:15.000000 glass_engine-0.1.9/glass/WeakSet.py
+-rw-rw-rw-   0        0        0     1110 2023-10-07 11:17:56.000000 glass_engine-0.1.9/glass/__init__.py
+-rw-rw-rw-   0        0        0     1566 2023-10-07 11:27:55.000000 glass_engine-0.1.9/glass/download.py
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:32.505237 glass_engine-0.1.9/glass/glsl/
+-rw-rw-rw-   0        0        0      201 2023-06-07 03:50:50.000000 glass_engine-0.1.9/glass/glsl/draw_frame.vs
+-rw-rw-rw-   0        0        0      909 2023-08-25 14:34:49.000000 glass_engine-0.1.9/glass/glsl/shadertoy_template.glsl
+-rw-rw-rw-   0        0        0     3620 2023-08-09 01:58:08.000000 glass_engine-0.1.9/glass/helper.py
+-rw-rw-rw-   0        0        0     1769 2023-08-16 03:06:11.000000 glass_engine-0.1.9/glass/iimage2D.py
+-rw-rw-rw-   0        0        0     1772 2023-08-16 03:10:26.000000 glass_engine-0.1.9/glass/image2D.py
+-rw-rw-rw-   0        0        0     1396 2023-08-22 11:26:13.000000 glass_engine-0.1.9/glass/isampler2D.py
+-rw-rw-rw-   0        0        0     1248 2023-08-22 11:25:55.000000 glass_engine-0.1.9/glass/isampler2DMS.py
+-rw-rw-rw-   0        0        0    20950 2023-09-23 07:30:33.000000 glass_engine-0.1.9/glass/sampler2D.py
+-rw-rw-rw-   0        0        0    16313 2023-08-15 15:22:30.000000 glass_engine-0.1.9/glass/sampler2DArray.py
+-rw-rw-rw-   0        0        0     3316 2023-08-09 02:02:55.000000 glass_engine-0.1.9/glass/sampler2DMS.py
+-rw-rw-rw-   0        0        0    12397 2023-08-09 02:04:02.000000 glass_engine-0.1.9/glass/samplerCube.py
+-rw-rw-rw-   0        0        0     1770 2023-08-16 03:06:56.000000 glass_engine-0.1.9/glass/uimage2D.py
+-rw-rw-rw-   0        0        0     1388 2023-08-22 11:26:31.000000 glass_engine-0.1.9/glass/usampler2D.py
+-rw-rw-rw-   0        0        0     1243 2023-08-22 11:26:45.000000 glass_engine-0.1.9/glass/usampler2DMS.py
+-rw-rw-rw-   0        0        0    18749 2023-10-07 11:16:40.000000 glass_engine-0.1.9/glass/utils.py
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:32.574057 glass_engine-0.1.9/glass_engine/
+-rw-rw-rw-   0        0        0      680 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/AffineTransform.py
+-rw-rw-rw-   0        0        0     1351 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Background.py
+-rw-rw-rw-   0        0        0      990 2023-08-28 05:51:39.000000 glass_engine-0.1.9/glass_engine/BasicScene.py
+-rw-rw-rw-   0        0        0     8371 2023-10-07 11:12:42.000000 glass_engine-0.1.9/glass_engine/Camera.py
+-rw-rw-rw-   0        0        0    11033 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/ColorMap.py
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:32.601975 glass_engine-0.1.9/glass_engine/Demos/
+-rw-rw-rw-   0        0        0       22 2023-08-25 06:06:39.000000 glass_engine-0.1.9/glass_engine/Demos/__init__.py
+-rw-rw-rw-   0        0        0      120 2023-08-25 06:04:52.000000 glass_engine-0.1.9/glass_engine/Demos/demo.py
+-rw-rw-rw-   0        0        0     9816 2023-10-07 14:22:19.000000 glass_engine-0.1.9/glass_engine/Demos/demo_transform.py
+-rw-rw-rw-   0        0        0     2721 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Fog.py
+-rw-rw-rw-   0        0        0     2635 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Frame.py
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:32.726643 glass_engine-0.1.9/glass_engine/Geometries/
+-rw-rw-rw-   0        0        0    10002 2023-09-22 14:59:17.000000 glass_engine-0.1.9/glass_engine/Geometries/Box.py
+-rw-rw-rw-   0        0        0     3015 2023-10-07 04:24:13.000000 glass_engine-0.1.9/glass_engine/Geometries/Circle.py
+-rw-rw-rw-   0        0        0     4189 2023-09-22 14:59:17.000000 glass_engine-0.1.9/glass_engine/Geometries/CircleFace.py
+-rw-rw-rw-   0        0        0     5390 2023-09-22 14:59:17.000000 glass_engine-0.1.9/glass_engine/Geometries/Cone.py
+-rw-rw-rw-   0        0        0     4158 2023-09-22 14:59:17.000000 glass_engine-0.1.9/glass_engine/Geometries/ConeSide.py
+-rw-rw-rw-   0        0        0     8113 2023-09-22 14:59:17.000000 glass_engine-0.1.9/glass_engine/Geometries/ConeTrustum.py
+-rw-rw-rw-   0        0        0     5631 2023-09-22 14:59:17.000000 glass_engine-0.1.9/glass_engine/Geometries/ConeTrustumSide.py
+-rw-rw-rw-   0        0        0     1066 2023-08-25 14:26:02.000000 glass_engine-0.1.9/glass_engine/Geometries/CoordSys.py
+-rw-rw-rw-   0        0        0     6408 2023-09-22 14:59:17.000000 glass_engine-0.1.9/glass_engine/Geometries/Cylinder.py
+-rw-rw-rw-   0        0        0     4228 2023-09-22 14:59:17.000000 glass_engine-0.1.9/glass_engine/Geometries/CylinderSide.py
+-rw-rw-rw-   0        0        0     2794 2023-09-22 14:59:17.000000 glass_engine-0.1.9/glass_engine/Geometries/CylindricalFSurf.py
+-rw-rw-rw-   0        0        0     6962 2023-09-22 14:59:17.000000 glass_engine-0.1.9/glass_engine/Geometries/Dodecahedron.py
+-rw-rw-rw-   0        0        0     4489 2023-09-22 14:59:17.000000 glass_engine-0.1.9/glass_engine/Geometries/EllipseFace.py
+-rw-rw-rw-   0        0        0    24519 2023-09-22 14:59:17.000000 glass_engine-0.1.9/glass_engine/Geometries/Extruder.py
+-rw-rw-rw-   0        0        0     3788 2023-09-22 14:59:17.000000 glass_engine-0.1.9/glass_engine/Geometries/FSurf.py
+-rw-rw-rw-   0        0        0     3179 2023-09-22 14:59:17.000000 glass_engine-0.1.9/glass_engine/Geometries/Floor.py
+-rw-rw-rw-   0        0        0     4072 2023-09-22 14:59:17.000000 glass_engine-0.1.9/glass_engine/Geometries/Hexahedron.py
+-rw-rw-rw-   0        0        0     5289 2023-09-22 14:59:17.000000 glass_engine-0.1.9/glass_engine/Geometries/HollowRPolygonFace.py
+-rw-rw-rw-   0        0        0     5005 2023-09-22 14:59:17.000000 glass_engine-0.1.9/glass_engine/Geometries/Icosahedron.py
+-rw-rw-rw-   0        0        0     8078 2023-09-22 14:59:17.000000 glass_engine-0.1.9/glass_engine/Geometries/Icosphere.py
+-rw-rw-rw-   0        0        0     4529 2023-09-22 14:59:17.000000 glass_engine-0.1.9/glass_engine/Geometries/ImageQuad.py
+-rw-rw-rw-   0        0        0     4088 2023-09-22 14:59:17.000000 glass_engine-0.1.9/glass_engine/Geometries/Octahedron.py
+-rw-rw-rw-   0        0        0     1155 2023-10-07 04:24:13.000000 glass_engine-0.1.9/glass_engine/Geometries/Point.py
+-rw-rw-rw-   0        0        0     1357 2023-10-07 04:24:13.000000 glass_engine-0.1.9/glass_engine/Geometries/Points.py
+-rw-rw-rw-   0        0        0     1972 2023-10-07 04:24:13.000000 glass_engine-0.1.9/glass_engine/Geometries/Polyline.py
+-rw-rw-rw-   0        0        0     7261 2023-09-22 14:59:17.000000 glass_engine-0.1.9/glass_engine/Geometries/Prism.py
+-rw-rw-rw-   0        0        0     5078 2023-09-22 14:59:17.000000 glass_engine-0.1.9/glass_engine/Geometries/PrismSide.py
+-rw-rw-rw-   0        0        0     5764 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Geometries/Pyramid.py
+-rw-rw-rw-   0        0        0     4581 2023-09-22 14:59:17.000000 glass_engine-0.1.9/glass_engine/Geometries/PyramidSide.py
+-rw-rw-rw-   0        0        0     8523 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Geometries/PyramidTrustum.py
+-rw-rw-rw-   0        0        0     6023 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Geometries/PyramidTrustumSide.py
+-rw-rw-rw-   0        0        0     4055 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Geometries/RPolygonFace.py
+-rw-rw-rw-   0        0        0     3727 2023-09-27 07:04:21.000000 glass_engine-0.1.9/glass_engine/Geometries/RectFace.py
+-rw-rw-rw-   0        0        0     6209 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Geometries/Rotator.py
+-rw-rw-rw-   0        0        0     4535 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Geometries/Sphere.py
+-rw-rw-rw-   0        0        0     5647 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Geometries/SphericalCap.py
+-rw-rw-rw-   0        0        0     4502 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Geometries/SphericalCapTop.py
+-rw-rw-rw-   0        0        0     2887 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Geometries/SphericalFSurf.py
+-rw-rw-rw-   0        0        0     7270 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Geometries/Surf.py
+-rw-rw-rw-   0        0        0     3488 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Geometries/Tetrahedron.py
+-rw-rw-rw-   0        0        0     6030 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Geometries/Torus.py
+-rw-rw-rw-   0        0        0     5405 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Geometries/TorusFace.py
+-rw-rw-rw-   0        0        0     7108 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Geometries/TrefoilKnot.py
+-rw-rw-rw-   0        0        0     1735 2023-09-27 07:04:43.000000 glass_engine-0.1.9/glass_engine/Geometries/__init__.py
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:32.745592 glass_engine-0.1.9/glass_engine/Lights/
+-rw-rw-rw-   0        0        0     1346 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Lights/DirLight.py
+-rw-rw-rw-   0        0        0     3529 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Lights/Light.py
+-rw-rw-rw-   0        0        0     3719 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Lights/PointLight.py
+-rw-rw-rw-   0        0        0     2991 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Lights/SpotLight.py
+-rw-rw-rw-   0        0        0      100 2023-06-09 08:06:38.000000 glass_engine-0.1.9/glass_engine/Lights/__init__.py
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:32.756563 glass_engine-0.1.9/glass_engine/Manipulators/
+-rw-rw-rw-   0        0        0    16527 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Manipulators/Manipulator.py
+-rw-rw-rw-   0        0        0     8720 2023-10-07 04:24:13.000000 glass_engine-0.1.9/glass_engine/Manipulators/ModelViewManipulator.py
+-rw-rw-rw-   0        0        0     7994 2023-10-07 04:24:13.000000 glass_engine-0.1.9/glass_engine/Manipulators/SceneRoamManipulator.py
+-rw-rw-rw-   0        0        0      148 2023-06-09 08:07:20.000000 glass_engine-0.1.9/glass_engine/Manipulators/__init__.py
+-rw-rw-rw-   0        0        0    33997 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Material.py
+-rw-rw-rw-   0        0        0    29443 2023-10-07 04:25:57.000000 glass_engine-0.1.9/glass_engine/Mesh.py
+-rw-rw-rw-   0        0        0    14936 2023-10-07 11:18:45.000000 glass_engine-0.1.9/glass_engine/Model.py
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:32.814421 glass_engine-0.1.9/glass_engine/PostProcessEffects/
+-rw-rw-rw-   0        0        0      287 2023-09-11 03:30:22.000000 glass_engine-0.1.9/glass_engine/PostProcessEffects/ACESToneMapper.py
+-rw-rw-rw-   0        0        0     6663 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/PostProcessEffects/BloomEffect.py
+-rw-rw-rw-   0        0        0     4303 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/PostProcessEffects/DOFEffect.py
+-rw-rw-rw-   0        0        0     1754 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/PostProcessEffects/ExplosureAdaptor.py
+-rw-rw-rw-   0        0        0     4138 2023-10-07 05:00:54.000000 glass_engine-0.1.9/glass_engine/PostProcessEffects/FXAAEffect.py
+-rw-rw-rw-   0        0        0    10800 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/PostProcessEffects/GaussBlur.py
+-rw-rw-rw-   0        0        0     5775 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/PostProcessEffects/KernelFilter.py
+-rw-rw-rw-   0        0        0     1478 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/PostProcessEffects/LUTEffect.py
+-rw-rw-rw-   0        0        0      284 2023-09-12 02:12:58.000000 glass_engine-0.1.9/glass_engine/PostProcessEffects/MedianBlur.py
+-rw-rw-rw-   0        0        0      276 2023-09-12 02:50:36.000000 glass_engine-0.1.9/glass_engine/PostProcessEffects/MulFilter.py
+-rw-rw-rw-   0        0        0     1423 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/PostProcessEffects/PostProcessEffect.py
+-rw-rw-rw-   0        0        0     3495 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/PostProcessEffects/PostProcessEffects.py
+-rw-rw-rw-   0        0        0     2427 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/PostProcessEffects/SSAOEffect.py
+-rw-rw-rw-   0        0        0     6646 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/PostProcessEffects/ShaderEffect.py
+-rw-rw-rw-   0        0        0      520 2023-10-07 04:57:50.000000 glass_engine-0.1.9/glass_engine/PostProcessEffects/__init__.py
+-rw-rw-rw-   0        0        0     2597 2023-10-07 11:48:12.000000 glass_engine-0.1.9/glass_engine/README_PYPI.md
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:32.845329 glass_engine-0.1.9/glass_engine/Renderers/
+-rw-rw-rw-   0        0        0    47076 2023-10-07 04:59:21.000000 glass_engine-0.1.9/glass_engine/Renderers/CommonRenderer.py
+-rw-rw-rw-   0        0        0    11866 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Renderers/DeferredRenderer.py
+-rw-rw-rw-   0        0        0     2427 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Renderers/ForwardRenderer.py
+-rw-rw-rw-   0        0        0      426 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Renderers/Renderer.py
+-rw-rw-rw-   0        0        0      124 2023-06-19 05:45:46.000000 glass_engine-0.1.9/glass_engine/Renderers/__init__.py
+-rw-rw-rw-   0        0        0    11431 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/Scene.py
+-rw-rw-rw-   0        0        0    15602 2023-10-07 14:22:01.000000 glass_engine-0.1.9/glass_engine/SceneNode.py
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:32.870262 glass_engine-0.1.9/glass_engine/Screens/
+-rw-rw-rw-   0        0        0     1065 2023-10-07 07:02:07.000000 glass_engine-0.1.9/glass_engine/Screens/PyQt5Screen.py
+-rw-rw-rw-   0        0        0     1077 2023-10-07 07:23:24.000000 glass_engine-0.1.9/glass_engine/Screens/PyQt6Screen.py
+-rw-rw-rw-   0        0        0     1069 2023-10-07 07:13:58.000000 glass_engine-0.1.9/glass_engine/Screens/PySide2Screen.py
+-rw-rw-rw-   0        0        0     1069 2023-10-07 06:50:15.000000 glass_engine-0.1.9/glass_engine/Screens/PySide6Screen.py
+-rw-rw-rw-   0        0        0    24595 2023-10-07 14:02:09.000000 glass_engine-0.1.9/glass_engine/Screens/QtScreen.py
+-rw-rw-rw-   0        0        0        0 2023-10-07 12:29:23.000000 glass_engine-0.1.9/glass_engine/Screens/__init__.py
+-rw-rw-rw-   0        0        0     4728 2023-10-07 04:24:13.000000 glass_engine-0.1.9/glass_engine/SkyBox.py
+-rw-rw-rw-   0        0        0     4473 2023-10-07 04:24:12.000000 glass_engine-0.1.9/glass_engine/SkyDome.py
+-rw-rw-rw-   0        0        0      750 2023-10-01 13:40:34.000000 glass_engine-0.1.9/glass_engine/SlideAverageFilter.py
+-rw-rw-rw-   0        0        0     3553 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/VideoRecorder.py
+-rw-rw-rw-   0        0        0     2458 2023-07-15 11:51:51.000000 glass_engine-0.1.9/glass_engine/WeightedIntegrator.py
+-rw-rw-rw-   0        0        0      337 2023-10-07 07:22:21.000000 glass_engine-0.1.9/glass_engine/__init__.py
+-rw-rw-rw-   0        0        0    15347 2023-09-22 14:59:15.000000 glass_engine-0.1.9/glass_engine/algorithm.py
+-rw-rw-rw-   0        0        0     2144 2023-09-19 09:43:51.000000 glass_engine-0.1.9/glass_engine/callback_vec.py
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:32.282829 glass_engine-0.1.9/glass_engine/glsl/
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:32.897187 glass_engine-0.1.9/glass_engine/glsl/Lights/
+-rw-rw-rw-   0        0        0     2948 2023-09-18 02:29:54.000000 glass_engine-0.1.9/glass_engine/glsl/Lights/DirLight.glsl
+-rw-rw-rw-   0        0        0     5447 2023-09-19 12:18:26.000000 glass_engine-0.1.9/glass_engine/glsl/Lights/DirLight_shadow_mapping.glsl
+-rw-rw-rw-   0        0        0     2958 2023-09-18 03:02:53.000000 glass_engine-0.1.9/glass_engine/glsl/Lights/Lights.glsl
+-rw-rw-rw-   0        0        0     3730 2023-09-18 02:29:47.000000 glass_engine-0.1.9/glass_engine/glsl/Lights/PointLight.glsl
+-rw-rw-rw-   0        0        0     2131 2023-09-06 05:17:49.000000 glass_engine-0.1.9/glass_engine/glsl/Lights/PointLight_shadow_mapping.glsl
+-rw-rw-rw-   0        0        0     4439 2023-09-18 02:30:02.000000 glass_engine-0.1.9/glass_engine/glsl/Lights/SpotLight.glsl
+-rw-rw-rw-   0        0        0     2627 2023-09-06 05:17:58.000000 glass_engine-0.1.9/glass_engine/glsl/Lights/SpotLight_shadow_mapping.glsl
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:32.915140 glass_engine-0.1.9/glass_engine/glsl/Pipelines/
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:32.932092 glass_engine-0.1.9/glass_engine/glsl/Pipelines/DirLight_depth/
+-rw-rw-rw-   0        0        0      637 2023-09-02 13:21:30.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/DirLight_depth/DirLight_depth.fs
+-rw-rw-rw-   0        0        0     1284 2023-09-02 12:57:44.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/DirLight_depth/DirLight_depth.gs
+-rw-rw-rw-   0        0        0     1077 2023-09-07 04:19:48.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/DirLight_depth/DirLight_depth.vs
+-rw-rw-rw-   0        0        0      967 2023-09-02 13:01:18.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/DirLight_depth/DirLight_depth_lines.gs
+-rw-rw-rw-   0        0        0      891 2023-09-02 13:08:46.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/DirLight_depth/DirLight_depth_points.gs
+-rw-rw-rw-   0        0        0      375 2023-07-27 08:40:27.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/OIT_blend.fs
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:32.948051 glass_engine-0.1.9/glass_engine/glsl/Pipelines/PointLight_depth/
+-rw-rw-rw-   0        0        0      926 2023-09-02 13:21:41.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/PointLight_depth/PointLight_depth.fs
+-rw-rw-rw-   0        0        0     1346 2023-09-07 11:35:41.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/PointLight_depth/PointLight_depth.gs
+-rw-rw-rw-   0        0        0     1035 2023-09-07 04:24:02.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/PointLight_depth/PointLight_depth.vs
+-rw-rw-rw-   0        0        0     1064 2023-09-07 11:36:44.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/PointLight_depth/PointLight_depth_lines.gs
+-rw-rw-rw-   0        0        0      986 2023-09-07 11:36:36.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/PointLight_depth/PointLight_depth_points.gs
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:32.964009 glass_engine-0.1.9/glass_engine/glsl/Pipelines/SpotLight_depth/
+-rw-rw-rw-   0        0        0      921 2023-09-07 12:35:57.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/SpotLight_depth/SpotLight_depth.fs
+-rw-rw-rw-   0        0        0     1339 2023-09-07 11:35:58.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/SpotLight_depth/SpotLight_depth.gs
+-rw-rw-rw-   0        0        0     1059 2023-09-07 11:36:21.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/SpotLight_depth/SpotLight_depth_lines.gs
+-rw-rw-rw-   0        0        0      981 2023-09-07 11:36:11.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/SpotLight_depth/SpotLight_depth_points.gs
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:32.983955 glass_engine-0.1.9/glass_engine/glsl/Pipelines/deferred_rendering/
+-rw-rw-rw-   0        0        0     1292 2023-09-18 05:04:16.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/deferred_rendering/deferred_rendering.fs
+-rw-rw-rw-   0        0        0     1976 2023-09-12 06:54:50.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/deferred_rendering/draw_points_to_gbuffer.fs
+-rw-rw-rw-   0        0        0     2451 2023-09-12 06:54:22.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/deferred_rendering/draw_to_gbuffer.fs
+-rw-rw-rw-   0        0        0     4196 2023-09-15 06:39:26.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/deferred_rendering/read_from_gbuffer.glsl
+-rw-rw-rw-   0        0        0     2733 2023-09-15 06:39:46.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/deferred_rendering/write_to_gbuffer.glsl
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:32.997918 glass_engine-0.1.9/glass_engine/glsl/Pipelines/draw_TBN/
+-rw-rw-rw-   0        0        0     1382 2023-09-07 04:20:28.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/draw_TBN/draw_TBN.vs
+-rw-rw-rw-   0        0        0      879 2023-07-05 08:14:07.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/draw_TBN/draw_bitangent.gs
+-rw-rw-rw-   0        0        0      878 2023-07-05 08:14:03.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/draw_TBN/draw_normal.gs
+-rw-rw-rw-   0        0        0      874 2023-07-05 08:14:00.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/draw_TBN/draw_tangent.gs
+-rw-rw-rw-   0        0        0      738 2023-09-04 05:07:22.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/draw_frame.fs
+-rw-rw-rw-   0        0        0      236 2023-07-27 09:10:55.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/draw_frame.vs
+-rw-rw-rw-   0        0        0      457 2023-07-27 08:28:26.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/draw_frame_array.gs
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:33.014872 glass_engine-0.1.9/glass_engine/glsl/Pipelines/draw_geometry/
+-rw-rw-rw-   0        0        0     1415 2023-09-12 01:24:06.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/draw_geometry/draw_geometry.fs
+-rw-rw-rw-   0        0        0     3365 2023-09-12 01:26:59.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/draw_geometry/draw_geometry.gs
+-rw-rw-rw-   0        0        0     1508 2023-09-12 01:28:54.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/draw_geometry/draw_geometry.vs
+-rw-rw-rw-   0        0        0     1618 2023-09-12 01:09:23.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/draw_geometry/draw_geometry_lines.vs
+-rw-rw-rw-   0        0        0      848 2023-09-12 01:24:34.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/draw_geometry/draw_geometry_points.fs
+-rw-rw-rw-   0        0        0     1361 2023-09-12 01:28:46.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/draw_geometry/draw_geometry_points.vs
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:33.047795 glass_engine-0.1.9/glass_engine/glsl/Pipelines/env_mapping/
+-rw-rw-rw-   0        0        0     1099 2023-09-04 05:42:27.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/env_mapping/env_OIT_blend.fs
+-rw-rw-rw-   0        0        0     1688 2023-09-18 05:09:30.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/env_mapping/gen_env_map.fs
+-rw-rw-rw-   0        0        0     5783 2023-09-12 03:00:10.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/env_mapping/gen_env_map.gs
+-rw-rw-rw-   0        0        0     1459 2023-09-07 04:25:37.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/env_mapping/gen_env_map.vs
+-rw-rw-rw-   0        0        0     2368 2023-09-12 03:01:41.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/env_mapping/gen_env_map_lines.gs
+-rw-rw-rw-   0        0        0     1573 2023-09-27 05:47:51.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/env_mapping/gen_env_map_points.fs
+-rw-rw-rw-   0        0        0     1974 2023-09-12 02:59:59.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/env_mapping/gen_env_map_points.gs
+-rw-rw-rw-   0        0        0     1099 2023-09-07 04:21:13.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/env_mapping/gen_env_map_points.vs
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:33.066733 glass_engine-0.1.9/glass_engine/glsl/Pipelines/forward_rendering/
+-rw-rw-rw-   0        0        0     2279 2023-09-12 03:00:21.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/forward_rendering/forward_draw_lines.vs
+-rw-rw-rw-   0        0        0     1655 2023-09-27 05:43:51.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/forward_rendering/forward_draw_points.fs
+-rw-rw-rw-   0        0        0     2016 2023-09-12 03:00:42.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/forward_rendering/forward_draw_points.vs
+-rw-rw-rw-   0        0        0     1802 2023-09-19 09:22:13.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/forward_rendering/forward_rendering.fs
+-rw-rw-rw-   0        0        0     5569 2023-09-12 03:01:03.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/forward_rendering/forward_rendering.gs
+-rw-rw-rw-   0        0        0     1610 2023-09-07 04:23:33.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/forward_rendering/forward_rendering.vs
+-rw-rw-rw-   0        0        0      324 2023-07-05 08:09:43.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/single_color.fs
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:33.071718 glass_engine-0.1.9/glass_engine/glsl/Pipelines/skybox/
+-rw-rw-rw-   0        0        0      629 2023-09-20 01:23:35.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/skybox/skybox.fs
+-rw-rw-rw-   0        0        0      450 2023-09-20 01:22:44.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/skybox/skybox.vs
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:33.078704 glass_engine-0.1.9/glass_engine/glsl/Pipelines/skydome/
+-rw-rw-rw-   0        0        0      645 2023-09-20 01:26:33.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/skydome/skydome.fs
+-rw-rw-rw-   0        0        0      433 2023-09-20 01:26:04.000000 glass_engine-0.1.9/glass_engine/glsl/Pipelines/skydome/skydome.vs
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:33.163474 glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/
+-rw-rw-rw-   0        0        0     1677 2023-09-21 14:10:44.000000 glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/ACES_tone_mapper.glsl
+-rw-rw-rw-   0        0        0      293 2023-09-04 06:04:10.000000 glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/FXAA.fs
+-rw-rw-rw-   0        0        0      314 2023-09-04 05:56:42.000000 glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/FXAA_array.fs
+-rw-rw-rw-   0        0        0      313 2023-09-04 05:58:59.000000 glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/FXAA_cube.fs
+-rw-rw-rw-   0        0        0     2351 2023-09-21 14:10:44.000000 glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/SSAO_visibility.glsl
+-rw-rw-rw-   0        0        0     2639 2023-09-12 08:48:17.000000 glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/bloom_downsampling.fs
+-rw-rw-rw-   0        0        0      405 2023-09-04 04:59:59.000000 glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/bloom_mix.fs
+-rw-rw-rw-   0        0        0     1647 2023-09-11 02:20:37.000000 glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/bloom_upsampling.fs
+-rw-rw-rw-   0        0        0     3374 2023-09-20 01:14:35.000000 glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/dof.fs
+-rw-rw-rw-   0        0        0     1779 2023-09-21 14:10:44.000000 glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/explosure_adaptor.glsl
+-rw-rw-rw-   0        0        0     1919 2023-09-12 02:57:38.000000 glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/gauss_blur.fs
+-rw-rw-rw-   0        0        0     1920 2023-09-12 02:57:53.000000 glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/gauss_blur_array.fs
+-rw-rw-rw-   0        0        0     1927 2023-09-12 02:57:45.000000 glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/gauss_blur_cube.fs
+-rw-rw-rw-   0        0        0      932 2023-09-12 02:57:00.000000 glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/kernel_filter.fs
+-rw-rw-rw-   0        0        0      989 2023-09-12 02:57:24.000000 glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/kernel_filter_array.fs
+-rw-rw-rw-   0        0        0      988 2023-09-12 02:57:11.000000 glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/kernel_filter_cube.fs
+-rw-rw-rw-   0        0        0     1499 2023-09-21 14:10:45.000000 glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/lut.glsl
+-rw-rw-rw-   0        0        0     1276 2023-09-21 14:10:44.000000 glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/median_gray_blur5.glsl
+-rw-rw-rw-   0        0        0      397 2023-09-21 14:10:44.000000 glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/mul_filter.glsl
+-rw-rw-rw-   0        0        0     1968 2023-09-21 14:10:44.000000 glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/shader_effect_template.glsl
+-rw-rw-rw-   0        0        0      666 2023-09-21 14:10:44.000000 glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/slit_stretch.glsl
+-rw-rw-rw-   0        0        0     1590 2023-09-21 14:10:44.000000 glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/star_field.glsl
+-rw-rw-rw-   0        0        0      239 2023-09-21 14:10:44.000000 glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/water_wave.glsl
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:33.202372 glass_engine-0.1.9/glass_engine/glsl/ShadingModels/
+-rw-rw-rw-   0        0        0     1553 2023-09-18 01:27:21.000000 glass_engine-0.1.9/glass_engine/glsl/ShadingModels/CookTorrance.glsl
+-rw-rw-rw-   0        0        0      477 2023-09-18 01:27:27.000000 glass_engine-0.1.9/glass_engine/glsl/ShadingModels/Flat.glsl
+-rw-rw-rw-   0        0        0      453 2023-09-18 01:27:40.000000 glass_engine-0.1.9/glass_engine/glsl/ShadingModels/Fresnel.glsl
+-rw-rw-rw-   0        0        0      263 2023-08-24 02:34:04.000000 glass_engine-0.1.9/glass_engine/glsl/ShadingModels/Gouraud.glsl
+-rw-rw-rw-   0        0        0      567 2023-09-18 01:27:47.000000 glass_engine-0.1.9/glass_engine/glsl/ShadingModels/Lambert.glsl
+-rw-rw-rw-   0        0        0     1107 2023-09-20 11:03:01.000000 glass_engine-0.1.9/glass_engine/glsl/ShadingModels/Minnaert.glsl
+-rw-rw-rw-   0        0        0     1976 2023-09-20 08:41:58.000000 glass_engine-0.1.9/glass_engine/glsl/ShadingModels/OrenNayar.glsl
+-rw-rw-rw-   0        0        0      862 2023-09-18 01:27:08.000000 glass_engine-0.1.9/glass_engine/glsl/ShadingModels/Phong.glsl
+-rw-rw-rw-   0        0        0      885 2023-09-18 01:28:12.000000 glass_engine-0.1.9/glass_engine/glsl/ShadingModels/PhongBlinn.glsl
+-rw-rw-rw-   0        0        0     1064 2023-09-20 13:43:52.000000 glass_engine-0.1.9/glass_engine/glsl/ShadingModels/Toon.glsl
+-rw-rw-rw-   0        0        0     1376 2023-08-28 08:32:31.000000 glass_engine-0.1.9/glass_engine/glsl/ShadingModels/lighting.glsl
+-rw-rw-rw-   0        0        0      503 2023-08-28 08:35:59.000000 glass_engine-0.1.9/glass_engine/glsl/ShadingModels/rim.glsl
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:33.256225 glass_engine-0.1.9/glass_engine/glsl/include/
+-rw-rw-rw-   0        0        0     6873 2023-09-20 01:20:38.000000 glass_engine-0.1.9/glass_engine/glsl/include/Camera.glsl
+-rw-rw-rw-   0        0        0    12032 2023-09-04 06:06:21.000000 glass_engine-0.1.9/glass_engine/glsl/include/FXAA.glsl
+-rw-rw-rw-   0        0        0     2141 2023-09-04 12:18:59.000000 glass_engine-0.1.9/glass_engine/glsl/include/FresnelRefract.glsl
+-rw-rw-rw-   0        0        0     8532 2023-09-23 01:42:20.000000 glass_engine-0.1.9/glass_engine/glsl/include/Material.glsl
+-rw-rw-rw-   0        0        0     1113 2023-07-03 04:27:35.000000 glass_engine-0.1.9/glass_engine/glsl/include/OIT.glsl
+-rw-rw-rw-   0        0        0     1160 2023-09-18 05:01:49.000000 glass_engine-0.1.9/glass_engine/glsl/include/ShadingInfo.glsl
+-rw-rw-rw-   0        0        0      187 2023-09-18 04:59:12.000000 glass_engine-0.1.9/glass_engine/glsl/include/background.glsl
+-rw-rw-rw-   0        0        0     9495 2023-09-18 05:16:28.000000 glass_engine-0.1.9/glass_engine/glsl/include/env_mapping.glsl
+-rw-rw-rw-   0        0        0     1151 2023-09-18 04:46:59.000000 glass_engine-0.1.9/glass_engine/glsl/include/fog.glsl
+-rw-rw-rw-   0        0        0     2322 2023-08-16 02:37:59.000000 glass_engine-0.1.9/glass_engine/glsl/include/image_read_write.glsl
+-rw-rw-rw-   0        0        0    12066 2023-09-20 13:28:40.000000 glass_engine-0.1.9/glass_engine/glsl/include/math.glsl
+-rw-rw-rw-   0        0        0     4011 2023-09-11 04:57:47.000000 glass_engine-0.1.9/glass_engine/glsl/include/parallax_mapping.glsl
+-rw-rw-rw-   0        0        0     1922 2023-06-13 08:24:20.000000 glass_engine-0.1.9/glass_engine/glsl/include/quat.glsl
+-rw-rw-rw-   0        0        0     4749 2023-09-11 04:47:49.000000 glass_engine-0.1.9/glass_engine/glsl/include/sampling.glsl
+-rw-rw-rw-   0        0        0     4742 2023-09-18 05:16:45.000000 glass_engine-0.1.9/glass_engine/glsl/include/shading_all.glsl
+-rw-rw-rw-   0        0        0     1997 2023-09-05 02:15:38.000000 glass_engine-0.1.9/glass_engine/glsl/include/transform.glsl
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:33.268195 glass_engine-0.1.9/glass_engine/images/
+-rw-rw-rw-   0        0        0   100665 2023-09-19 08:50:53.000000 glass_engine-0.1.9/glass_engine/images/glass_engine_logo256.png
+-rw-rw-rw-   0        0        0    11211 2023-09-19 08:52:07.000000 glass_engine-0.1.9/glass_engine/images/glass_engine_logo64.png
+-rw-rw-rw-   0        0        0    41344 2023-09-21 10:19:41.000000 glass_engine-0.1.9/glass_engine/images/start.png
+-rw-rw-rw-   0        0        0     4121 2023-09-09 06:26:47.000000 glass_engine-0.1.9/glass_engine/lut.py
+drwxrwxrwx   0        0        0        0 2023-10-07 14:23:32.590009 glass_engine-0.1.9/glass_engine.egg-info/
+-rw-rw-rw-   0        0        0     3126 2023-10-07 14:23:31.000000 glass_engine-0.1.9/glass_engine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11058 2023-10-07 14:23:32.000000 glass_engine-0.1.9/glass_engine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-10-07 14:23:31.000000 glass_engine-0.1.9/glass_engine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      141 2023-10-07 14:23:31.000000 glass_engine-0.1.9/glass_engine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-10-07 14:23:31.000000 glass_engine-0.1.9/glass_engine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-10-07 14:23:33.272184 glass_engine-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     2048 2023-10-07 14:23:09.000000 glass_engine-0.1.9/setup.py
```

### Comparing `glass_engine-0.1.8/LICENSE` & `glass_engine-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/PKG-INFO` & `glass_engine-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glass_engine
-Version: 0.1.8
+Version: 0.1.9
 Summary: An easy-to-use 3D rendering engine for Python
 Home-page: https://github.com/Time-Coder/Glass-Engine
 Author: 王炳辉 (BingHui-WANG)
 Author-email: binghui.wang@foxmail.com
 Platform: win_amd64
 Platform: win32
 Classifier: Programming Language :: Python :: 3
```

### Comparing `glass_engine-0.1.8/README.rst` & `glass_engine-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/ACBO.py` & `glass_engine-0.1.9/glass/ACBO.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/AttrList.py` & `glass_engine-0.1.9/glass/AttrList.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/BO.py` & `glass_engine-0.1.9/glass/BO.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/Block.py` & `glass_engine-0.1.9/glass/Block.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/CSRMat.py` & `glass_engine-0.1.9/glass/CSRMat.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/ComputeProgram.py` & `glass_engine-0.1.9/glass/ComputeProgram.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/DictList.py` & `glass_engine-0.1.9/glass/DictList.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/FBO.py` & `glass_engine-0.1.9/glass/FBO.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/FBOAttachment.py` & `glass_engine-0.1.9/glass/FBOAttachment.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/GLConfig.py` & `glass_engine-0.1.9/glass/GLConfig.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/GLInfo.py` & `glass_engine-0.1.9/glass/GLInfo.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/GLObject.py` & `glass_engine-0.1.9/glass/GLObject.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/GPUProgram.py` & `glass_engine-0.1.9/glass/GPUProgram.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/GlassConfig.py` & `glass_engine-0.1.9/glass/GlassConfig.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
-import sys
 
 class GlassConfig:
 
     def __init__(self):
-        glass_engine_glsl_folder = os.path.dirname(os.path.abspath(sys.argv[0])).replace("\\", "/") + "/../glass_engine/glsl"
-        glass_glsl_folder = os.path.dirname(os.path.abspath(sys.argv[0])).replace("\\", "/") + "/glsl"
+        self_folder = os.path.dirname(os.path.abspath(__file__)).replace("\\", "/")
+        glass_engine_glsl_folder = self_folder + "/../glass_engine/glsl"
+        glass_glsl_folder = self_folder + "/glsl"
         if os.path.isdir(glass_engine_glsl_folder):
             self.__cache_folder = glass_engine_glsl_folder + "/__glcache__"
         else:
             self.__cache_folder = glass_glsl_folder + "/__glcache__"
 
         self.__debug = True
         self.__print = True
```

### Comparing `glass_engine-0.1.8/glass/ImageLoader.py` & `glass_engine-0.1.9/glass/ImageLoader.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/ImageUnits.py` & `glass_engine-0.1.9/glass/ImageUnits.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/Increment.py` & `glass_engine-0.1.9/glass/Increment.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/Indices.py` & `glass_engine-0.1.9/glass/Indices.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/Instances.py` & `glass_engine-0.1.9/glass/Instances.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/RBO.py` & `glass_engine-0.1.9/glass/RBO.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/RenderHints.py` & `glass_engine-0.1.9/glass/RenderHints.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/SSBO.py` & `glass_engine-0.1.9/glass/SSBO.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/SSUBO.py` & `glass_engine-0.1.9/glass/SSUBO.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/SameTypeList.py` & `glass_engine-0.1.9/glass/SameTypeList.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/ShaderParser.py` & `glass_engine-0.1.9/glass/ShaderParser.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/ShaderProgram.py` & `glass_engine-0.1.9/glass/ShaderProgram.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/ShaderStorageBlock.py` & `glass_engine-0.1.9/glass/ShaderStorageBlock.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/Shaders.py` & `glass_engine-0.1.9/glass/Shaders.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/TextureUnits.py` & `glass_engine-0.1.9/glass/TextureUnits.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/Uniform.py` & `glass_engine-0.1.9/glass/Uniform.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/UniformBlock.py` & `glass_engine-0.1.9/glass/UniformBlock.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/VAO.py` & `glass_engine-0.1.9/glass/VAO.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/Vertices.py` & `glass_engine-0.1.9/glass/Vertices.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/WeakDict.py` & `glass_engine-0.1.9/glass/WeakDict.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/WeakList.py` & `glass_engine-0.1.9/glass/WeakList.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/WeakRef.py` & `glass_engine-0.1.9/glass/WeakRef.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/WeakSet.py` & `glass_engine-0.1.9/glass/WeakSet.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/__init__.py` & `glass_engine-0.1.9/glass/__init__.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/download.py` & `glass_engine-0.1.9/glass/download.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/glsl/shadertoy_template.glsl` & `glass_engine-0.1.9/glass/glsl/shadertoy_template.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/helper.py` & `glass_engine-0.1.9/glass/helper.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/iimage2D.py` & `glass_engine-0.1.9/glass/iimage2D.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/image2D.py` & `glass_engine-0.1.9/glass/image2D.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/isampler2D.py` & `glass_engine-0.1.9/glass/isampler2D.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/isampler2DMS.py` & `glass_engine-0.1.9/glass/isampler2DMS.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/sampler2D.py` & `glass_engine-0.1.9/glass/sampler2D.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/sampler2DArray.py` & `glass_engine-0.1.9/glass/sampler2DArray.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/sampler2DMS.py` & `glass_engine-0.1.9/glass/sampler2DMS.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/samplerCube.py` & `glass_engine-0.1.9/glass/samplerCube.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/uimage2D.py` & `glass_engine-0.1.9/glass/uimage2D.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/usampler2D.py` & `glass_engine-0.1.9/glass/usampler2D.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/usampler2DMS.py` & `glass_engine-0.1.9/glass/usampler2DMS.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass/utils.py` & `glass_engine-0.1.9/glass/utils.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/AffineTransform.py` & `glass_engine-0.1.9/glass_engine/AffineTransform.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Background.py` & `glass_engine-0.1.9/glass_engine/Background.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/BasicScene.py` & `glass_engine-0.1.9/glass_engine/BasicScene.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Camera.py` & `glass_engine-0.1.9/glass_engine/Camera.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/ColorMap.py` & `glass_engine-0.1.9/glass_engine/ColorMap.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Demos/demo_transform.py` & `glass_engine-0.1.9/glass_engine/Demos/demo_transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,15 +221,14 @@
     def scale_z_changed(self, value):
         self.model.scale.z = value
         self.camera.screen.update()
 
 def download_files():
     self_folder = os.path.dirname(os.path.abspath(__file__)).replace("\\", "/")
     model_folder = self_folder + "/assets/models/jet"
-    skydome_folder = self_folder + "/assets/skydomes"
 
     md5_map = \
     {
         "11805_airplane_v2_L2.mtl": "36059ea10e4a35955dc2ee6b1203f9c8",
         "11805_airplane_v2_L2.obj": "85bd6ac8fcc6c717ba5a96a7a065c0ec",
         "airplane_body_diffuse_v1.jpg": "e7b1c3492a69e81959ffc14af0ad8ed7",
         "airplane_wings_diffuse_v1.jpg": "c4ef09fd0825d5d97a1ba105775e253a",
```

### Comparing `glass_engine-0.1.8/glass_engine/Fog.py` & `glass_engine-0.1.9/glass_engine/Fog.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Frame.py` & `glass_engine-0.1.9/glass_engine/Frame.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/Box.py` & `glass_engine-0.1.9/glass_engine/Geometries/Box.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/Circle.py` & `glass_engine-0.1.9/glass_engine/Geometries/Circle.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/CircleFace.py` & `glass_engine-0.1.9/glass_engine/Geometries/CircleFace.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/Cone.py` & `glass_engine-0.1.9/glass_engine/Geometries/Cone.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/ConeSide.py` & `glass_engine-0.1.9/glass_engine/Geometries/ConeSide.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/ConeTrustum.py` & `glass_engine-0.1.9/glass_engine/Geometries/ConeTrustum.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/ConeTrustumSide.py` & `glass_engine-0.1.9/glass_engine/Geometries/ConeTrustumSide.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/CoordSys.py` & `glass_engine-0.1.9/glass_engine/Geometries/CoordSys.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/Cylinder.py` & `glass_engine-0.1.9/glass_engine/Geometries/Cylinder.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/CylinderSide.py` & `glass_engine-0.1.9/glass_engine/Geometries/CylinderSide.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/CylindricalFSurf.py` & `glass_engine-0.1.9/glass_engine/Geometries/CylindricalFSurf.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/Dodecahedron.py` & `glass_engine-0.1.9/glass_engine/Geometries/Dodecahedron.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/EllipseFace.py` & `glass_engine-0.1.9/glass_engine/Geometries/EllipseFace.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/Extruder.py` & `glass_engine-0.1.9/glass_engine/Geometries/Extruder.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/FSurf.py` & `glass_engine-0.1.9/glass_engine/Geometries/FSurf.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/Floor.py` & `glass_engine-0.1.9/glass_engine/Geometries/Floor.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/Hexahedron.py` & `glass_engine-0.1.9/glass_engine/Geometries/Hexahedron.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/HollowRPolygonFace.py` & `glass_engine-0.1.9/glass_engine/Geometries/HollowRPolygonFace.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/Icosahedron.py` & `glass_engine-0.1.9/glass_engine/Geometries/Icosahedron.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/Icosphere.py` & `glass_engine-0.1.9/glass_engine/Geometries/Icosphere.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/ImageQuad.py` & `glass_engine-0.1.9/glass_engine/Geometries/ImageQuad.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/Octahedron.py` & `glass_engine-0.1.9/glass_engine/Geometries/Octahedron.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/Point.py` & `glass_engine-0.1.9/glass_engine/Geometries/Point.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/Points.py` & `glass_engine-0.1.9/glass_engine/Geometries/Points.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/Polyline.py` & `glass_engine-0.1.9/glass_engine/Geometries/Polyline.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/Prism.py` & `glass_engine-0.1.9/glass_engine/Geometries/Prism.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/PrismSide.py` & `glass_engine-0.1.9/glass_engine/Geometries/PrismSide.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/Pyramid.py` & `glass_engine-0.1.9/glass_engine/Geometries/Pyramid.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/PyramidSide.py` & `glass_engine-0.1.9/glass_engine/Geometries/PyramidSide.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/PyramidTrustum.py` & `glass_engine-0.1.9/glass_engine/Geometries/PyramidTrustum.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/PyramidTrustumSide.py` & `glass_engine-0.1.9/glass_engine/Geometries/PyramidTrustumSide.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/RPolygonFace.py` & `glass_engine-0.1.9/glass_engine/Geometries/RPolygonFace.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/RectFace.py` & `glass_engine-0.1.9/glass_engine/Geometries/RectFace.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/Rotator.py` & `glass_engine-0.1.9/glass_engine/Geometries/Rotator.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/Sphere.py` & `glass_engine-0.1.9/glass_engine/Geometries/Sphere.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/SphericalCap.py` & `glass_engine-0.1.9/glass_engine/Geometries/SphericalCap.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/SphericalCapTop.py` & `glass_engine-0.1.9/glass_engine/Geometries/SphericalCapTop.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/SphericalFSurf.py` & `glass_engine-0.1.9/glass_engine/Geometries/SphericalFSurf.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/Surf.py` & `glass_engine-0.1.9/glass_engine/Geometries/Surf.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/Tetrahedron.py` & `glass_engine-0.1.9/glass_engine/Geometries/Tetrahedron.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/Torus.py` & `glass_engine-0.1.9/glass_engine/Geometries/Torus.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/TorusFace.py` & `glass_engine-0.1.9/glass_engine/Geometries/TorusFace.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/TrefoilKnot.py` & `glass_engine-0.1.9/glass_engine/Geometries/TrefoilKnot.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Geometries/__init__.py` & `glass_engine-0.1.9/glass_engine/Geometries/__init__.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Lights/DirLight.py` & `glass_engine-0.1.9/glass_engine/Lights/DirLight.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Lights/Light.py` & `glass_engine-0.1.9/glass_engine/Lights/Light.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Lights/PointLight.py` & `glass_engine-0.1.9/glass_engine/Lights/PointLight.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Lights/SpotLight.py` & `glass_engine-0.1.9/glass_engine/Lights/SpotLight.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Manipulators/Manipulator.py` & `glass_engine-0.1.9/glass_engine/Manipulators/Manipulator.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Manipulators/ModelViewManipulator.py` & `glass_engine-0.1.9/glass_engine/Manipulators/ModelViewManipulator.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Manipulators/SceneRoamManipulator.py` & `glass_engine-0.1.9/glass_engine/Manipulators/SceneRoamManipulator.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Material.py` & `glass_engine-0.1.9/glass_engine/Material.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Mesh.py` & `glass_engine-0.1.9/glass_engine/Mesh.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Model.py` & `glass_engine-0.1.9/glass_engine/Model.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/PostProcessEffects/BloomEffect.py` & `glass_engine-0.1.9/glass_engine/PostProcessEffects/BloomEffect.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/PostProcessEffects/DOFEffect.py` & `glass_engine-0.1.9/glass_engine/PostProcessEffects/DOFEffect.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/PostProcessEffects/ExplosureAdaptor.py` & `glass_engine-0.1.9/glass_engine/PostProcessEffects/ExplosureAdaptor.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/PostProcessEffects/FXAAEffect.py` & `glass_engine-0.1.9/glass_engine/PostProcessEffects/FXAAEffect.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/PostProcessEffects/GaussBlur.py` & `glass_engine-0.1.9/glass_engine/PostProcessEffects/GaussBlur.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/PostProcessEffects/KernelFilter.py` & `glass_engine-0.1.9/glass_engine/PostProcessEffects/KernelFilter.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/PostProcessEffects/LUTEffect.py` & `glass_engine-0.1.9/glass_engine/PostProcessEffects/LUTEffect.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/PostProcessEffects/PostProcessEffect.py` & `glass_engine-0.1.9/glass_engine/PostProcessEffects/PostProcessEffect.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/PostProcessEffects/PostProcessEffects.py` & `glass_engine-0.1.9/glass_engine/PostProcessEffects/PostProcessEffects.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/PostProcessEffects/SSAOEffect.py` & `glass_engine-0.1.9/glass_engine/PostProcessEffects/SSAOEffect.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/PostProcessEffects/ShaderEffect.py` & `glass_engine-0.1.9/glass_engine/PostProcessEffects/ShaderEffect.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/PostProcessEffects/__init__.py` & `glass_engine-0.1.9/glass_engine/PostProcessEffects/__init__.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/README_PYPI.md` & `glass_engine-0.1.9/glass_engine/README_PYPI.md`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Renderers/CommonRenderer.py` & `glass_engine-0.1.9/glass_engine/Renderers/CommonRenderer.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Renderers/DeferredRenderer.py` & `glass_engine-0.1.9/glass_engine/Renderers/DeferredRenderer.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Renderers/ForwardRenderer.py` & `glass_engine-0.1.9/glass_engine/Renderers/ForwardRenderer.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Scene.py` & `glass_engine-0.1.9/glass_engine/Scene.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/SceneNode.py` & `glass_engine-0.1.9/glass_engine/SceneNode.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,22 +324,14 @@
     def roll(self):
         return self._yaw_pitch_roll[2]
 
     @roll.setter
     def roll(self, roll:float):
         self._yaw_pitch_roll[2] = roll
         self._update_orientation()
-
-    @staticmethod
-    def path_str(node_path):
-        path = ""
-        for node in node_path:
-            path += ("/" + node.name)
-
-        return path
     
     @property
     def paths(self):
         if not self.parents:
             return [[self]]
         
         all_paths = []
@@ -445,22 +437,14 @@
     def path(self)->list:
         if self.parent is None:
             return [self]
         
         path = self.parent.paths[0]
         path.append(self)
         return path
-    
-    @property
-    def path_str(self)->str:
-        if self.parent is None:
-            return "/" + self.name
-        
-        path_str = self.parent.paths_str[0]
-        return path_str + "/" + self.name
 
     @staticmethod
     def __abs_orientation(node)->glm.quat:
         try:
             parent = node.parents[0]
         except IndexError:
             return node._orientation.flat
```

### Comparing `glass_engine-0.1.8/glass_engine/Screens/PyQt5Screen.py` & `glass_engine-0.1.9/glass_engine/Screens/PyQt5Screen.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Screens/PyQt6Screen.py` & `glass_engine-0.1.9/glass_engine/Screens/PyQt6Screen.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Screens/PySide2Screen.py` & `glass_engine-0.1.9/glass_engine/Screens/PySide2Screen.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Screens/PySide6Screen.py` & `glass_engine-0.1.9/glass_engine/Screens/PySide6Screen.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/Screens/QtScreen.py` & `glass_engine-0.1.9/glass_engine/Screens/QtScreen.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/SkyBox.py` & `glass_engine-0.1.9/glass_engine/SkyBox.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/SkyDome.py` & `glass_engine-0.1.9/glass_engine/SkyDome.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/SlideAverageFilter.py` & `glass_engine-0.1.9/glass_engine/SlideAverageFilter.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/VideoRecorder.py` & `glass_engine-0.1.9/glass_engine/VideoRecorder.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/WeightedIntegrator.py` & `glass_engine-0.1.9/glass_engine/WeightedIntegrator.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/algorithm.py` & `glass_engine-0.1.9/glass_engine/algorithm.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/callback_vec.py` & `glass_engine-0.1.9/glass_engine/callback_vec.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Lights/DirLight.glsl` & `glass_engine-0.1.9/glass_engine/glsl/Lights/DirLight.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Lights/DirLight_shadow_mapping.glsl` & `glass_engine-0.1.9/glass_engine/glsl/Lights/DirLight_shadow_mapping.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Lights/Lights.glsl` & `glass_engine-0.1.9/glass_engine/glsl/Lights/Lights.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Lights/PointLight.glsl` & `glass_engine-0.1.9/glass_engine/glsl/Lights/PointLight.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Lights/PointLight_shadow_mapping.glsl` & `glass_engine-0.1.9/glass_engine/glsl/Lights/PointLight_shadow_mapping.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Lights/SpotLight.glsl` & `glass_engine-0.1.9/glass_engine/glsl/Lights/SpotLight.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Lights/SpotLight_shadow_mapping.glsl` & `glass_engine-0.1.9/glass_engine/glsl/Lights/SpotLight_shadow_mapping.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/DirLight_depth/DirLight_depth.fs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/DirLight_depth/DirLight_depth.fs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/DirLight_depth/DirLight_depth.gs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/DirLight_depth/DirLight_depth.gs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/DirLight_depth/DirLight_depth.vs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/DirLight_depth/DirLight_depth.vs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/DirLight_depth/DirLight_depth_lines.gs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/DirLight_depth/DirLight_depth_lines.gs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/DirLight_depth/DirLight_depth_points.gs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/DirLight_depth/DirLight_depth_points.gs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/PointLight_depth/PointLight_depth.fs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/PointLight_depth/PointLight_depth.fs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/PointLight_depth/PointLight_depth.gs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/PointLight_depth/PointLight_depth.gs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/PointLight_depth/PointLight_depth.vs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/PointLight_depth/PointLight_depth.vs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/PointLight_depth/PointLight_depth_lines.gs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/PointLight_depth/PointLight_depth_lines.gs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/PointLight_depth/PointLight_depth_points.gs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/PointLight_depth/PointLight_depth_points.gs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/SpotLight_depth/SpotLight_depth.fs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/SpotLight_depth/SpotLight_depth.fs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/SpotLight_depth/SpotLight_depth.gs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/SpotLight_depth/SpotLight_depth.gs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/SpotLight_depth/SpotLight_depth_lines.gs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/SpotLight_depth/SpotLight_depth_lines.gs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/SpotLight_depth/SpotLight_depth_points.gs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/SpotLight_depth/SpotLight_depth_points.gs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/deferred_rendering/deferred_rendering.fs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/deferred_rendering/deferred_rendering.fs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/deferred_rendering/draw_points_to_gbuffer.fs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/deferred_rendering/draw_points_to_gbuffer.fs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/deferred_rendering/draw_to_gbuffer.fs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/deferred_rendering/draw_to_gbuffer.fs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/deferred_rendering/read_from_gbuffer.glsl` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/deferred_rendering/read_from_gbuffer.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/deferred_rendering/write_to_gbuffer.glsl` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/deferred_rendering/write_to_gbuffer.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/draw_TBN/draw_TBN.vs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/draw_TBN/draw_TBN.vs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/draw_TBN/draw_bitangent.gs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/draw_TBN/draw_bitangent.gs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/draw_TBN/draw_normal.gs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/draw_TBN/draw_normal.gs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/draw_TBN/draw_tangent.gs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/draw_TBN/draw_tangent.gs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/draw_frame.fs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/draw_frame.fs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/draw_geometry/draw_geometry.fs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/draw_geometry/draw_geometry.fs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/draw_geometry/draw_geometry.gs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/draw_geometry/draw_geometry.gs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/draw_geometry/draw_geometry.vs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/draw_geometry/draw_geometry.vs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/draw_geometry/draw_geometry_lines.vs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/draw_geometry/draw_geometry_lines.vs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/draw_geometry/draw_geometry_points.fs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/draw_geometry/draw_geometry_points.fs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/draw_geometry/draw_geometry_points.vs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/draw_geometry/draw_geometry_points.vs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/env_mapping/env_OIT_blend.fs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/env_mapping/env_OIT_blend.fs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/env_mapping/gen_env_map.fs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/env_mapping/gen_env_map.fs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/env_mapping/gen_env_map.gs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/env_mapping/gen_env_map.gs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/env_mapping/gen_env_map.vs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/env_mapping/gen_env_map.vs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/env_mapping/gen_env_map_lines.gs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/env_mapping/gen_env_map_lines.gs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/env_mapping/gen_env_map_points.fs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/env_mapping/gen_env_map_points.fs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/env_mapping/gen_env_map_points.gs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/env_mapping/gen_env_map_points.gs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/env_mapping/gen_env_map_points.vs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/env_mapping/gen_env_map_points.vs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/forward_rendering/forward_draw_lines.vs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/forward_rendering/forward_draw_lines.vs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/forward_rendering/forward_draw_points.fs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/forward_rendering/forward_draw_points.fs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/forward_rendering/forward_draw_points.vs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/forward_rendering/forward_draw_points.vs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/forward_rendering/forward_rendering.fs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/forward_rendering/forward_rendering.fs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/forward_rendering/forward_rendering.gs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/forward_rendering/forward_rendering.gs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/forward_rendering/forward_rendering.vs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/forward_rendering/forward_rendering.vs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/skybox/skybox.fs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/skybox/skybox.fs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/Pipelines/skydome/skydome.fs` & `glass_engine-0.1.9/glass_engine/glsl/Pipelines/skydome/skydome.fs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/ACES_tone_mapper.glsl` & `glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/ACES_tone_mapper.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/SSAO_visibility.glsl` & `glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/SSAO_visibility.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/bloom_downsampling.fs` & `glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/bloom_downsampling.fs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/bloom_upsampling.fs` & `glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/bloom_upsampling.fs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/dof.fs` & `glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/dof.fs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/explosure_adaptor.glsl` & `glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/explosure_adaptor.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/gauss_blur.fs` & `glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/gauss_blur.fs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/gauss_blur_array.fs` & `glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/gauss_blur_array.fs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/gauss_blur_cube.fs` & `glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/gauss_blur_cube.fs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/kernel_filter.fs` & `glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/kernel_filter.fs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/kernel_filter_array.fs` & `glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/kernel_filter_array.fs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/kernel_filter_cube.fs` & `glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/kernel_filter_cube.fs`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/lut.glsl` & `glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/lut.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/median_gray_blur5.glsl` & `glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/median_gray_blur5.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/shader_effect_template.glsl` & `glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/shader_effect_template.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/slit_stretch.glsl` & `glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/slit_stretch.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/PostProcessEffects/star_field.glsl` & `glass_engine-0.1.9/glass_engine/glsl/PostProcessEffects/star_field.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/ShadingModels/CookTorrance.glsl` & `glass_engine-0.1.9/glass_engine/glsl/ShadingModels/CookTorrance.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/ShadingModels/Lambert.glsl` & `glass_engine-0.1.9/glass_engine/glsl/ShadingModels/Lambert.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/ShadingModels/Minnaert.glsl` & `glass_engine-0.1.9/glass_engine/glsl/ShadingModels/Minnaert.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/ShadingModels/OrenNayar.glsl` & `glass_engine-0.1.9/glass_engine/glsl/ShadingModels/OrenNayar.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/ShadingModels/Phong.glsl` & `glass_engine-0.1.9/glass_engine/glsl/ShadingModels/Phong.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/ShadingModels/PhongBlinn.glsl` & `glass_engine-0.1.9/glass_engine/glsl/ShadingModels/PhongBlinn.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/ShadingModels/Toon.glsl` & `glass_engine-0.1.9/glass_engine/glsl/ShadingModels/Toon.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/ShadingModels/lighting.glsl` & `glass_engine-0.1.9/glass_engine/glsl/ShadingModels/lighting.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/include/Camera.glsl` & `glass_engine-0.1.9/glass_engine/glsl/include/Camera.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/include/FXAA.glsl` & `glass_engine-0.1.9/glass_engine/glsl/include/FXAA.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/include/FresnelRefract.glsl` & `glass_engine-0.1.9/glass_engine/glsl/include/FresnelRefract.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/include/Material.glsl` & `glass_engine-0.1.9/glass_engine/glsl/include/Material.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/include/OIT.glsl` & `glass_engine-0.1.9/glass_engine/glsl/include/OIT.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/include/ShadingInfo.glsl` & `glass_engine-0.1.9/glass_engine/glsl/include/ShadingInfo.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/include/env_mapping.glsl` & `glass_engine-0.1.9/glass_engine/glsl/include/env_mapping.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/include/fog.glsl` & `glass_engine-0.1.9/glass_engine/glsl/include/fog.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/include/image_read_write.glsl` & `glass_engine-0.1.9/glass_engine/glsl/include/image_read_write.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/include/math.glsl` & `glass_engine-0.1.9/glass_engine/glsl/include/math.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/include/parallax_mapping.glsl` & `glass_engine-0.1.9/glass_engine/glsl/include/parallax_mapping.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/include/quat.glsl` & `glass_engine-0.1.9/glass_engine/glsl/include/quat.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/include/sampling.glsl` & `glass_engine-0.1.9/glass_engine/glsl/include/sampling.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/include/shading_all.glsl` & `glass_engine-0.1.9/glass_engine/glsl/include/shading_all.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/glsl/include/transform.glsl` & `glass_engine-0.1.9/glass_engine/glsl/include/transform.glsl`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/images/glass_engine_logo256.png` & `glass_engine-0.1.9/glass_engine/images/glass_engine_logo256.png`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/images/glass_engine_logo64.png` & `glass_engine-0.1.9/glass_engine/images/glass_engine_logo64.png`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/images/start.png` & `glass_engine-0.1.9/glass_engine/images/start.png`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine/lut.py` & `glass_engine-0.1.9/glass_engine/lut.py`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/glass_engine.egg-info/PKG-INFO` & `glass_engine-0.1.9/glass_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glass-engine
-Version: 0.1.8
+Version: 0.1.9
 Summary: An easy-to-use 3D rendering engine for Python
 Home-page: https://github.com/Time-Coder/Glass-Engine
 Author: 王炳辉 (BingHui-WANG)
 Author-email: binghui.wang@foxmail.com
 Platform: win_amd64
 Platform: win32
 Classifier: Programming Language :: Python :: 3
```

### Comparing `glass_engine-0.1.8/glass_engine.egg-info/SOURCES.txt` & `glass_engine-0.1.9/glass_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glass_engine-0.1.8/setup.py` & `glass_engine-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     "README_PYPI.md"
 ]
 glass_engine_extra_files.extend(find_files("glass_engine", "glass_engine/glsl"))
 glass_extra_files = find_files("glass", "glass/glsl")
 
 setuptools.setup(
     name="glass_engine",
-    version="0.1.8",
+    version="0.1.9",
     author="王炳辉 (BingHui-WANG)",
     author_email="binghui.wang@foxmail.com",
     description="An easy-to-use 3D rendering engine for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Time-Coder/Glass-Engine",
     packages=setuptools.find_packages(),
```


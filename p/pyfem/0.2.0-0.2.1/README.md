# Comparing `tmp/pyfem-0.2.0.tar.gz` & `tmp/pyfem-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfem-0.2.0.tar", last modified: Thu Apr 18 07:48:12 2024, max compression
+gzip compressed data, was "pyfem-0.2.1.tar", last modified: Mon Apr 22 08:34:00 2024, max compression
```

## Comparing `pyfem-0.2.0.tar` & `pyfem-0.2.1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.193787 pyfem-0.2.0/
--rw-rw-rw-   0        0        0    11525 2023-08-17 09:47:31.000000 pyfem-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     3579 2024-04-18 07:48:12.193287 pyfem-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-18 07:48:12.193787 pyfem-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1115 2023-08-17 09:47:32.000000 pyfem-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.090787 pyfem-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.104787 pyfem-0.2.0/src/pyfem/
--rw-rw-rw-   0        0        0     2804 2023-11-01 09:09:41.000000 pyfem-0.2.0/src/pyfem/Job.py
--rw-rw-rw-   0        0        0       23 2024-04-18 07:25:48.000000 pyfem-0.2.0/src/pyfem/__init__.py
--rw-rw-rw-   0        0        0     1388 2023-11-02 07:31:58.000000 pyfem-0.2.0/src/pyfem/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.115287 pyfem-0.2.0/src/pyfem/amplitude/
--rw-rw-rw-   0        0        0     1403 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/amplitude/BaseAmplitude.py
--rw-rw-rw-   0        0        0     1892 2023-11-02 07:24:23.000000 pyfem-0.2.0/src/pyfem/amplitude/TabularAmplitude.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/amplitude/__init__.py
--rw-rw-rw-   0        0        0     1112 2023-11-02 07:24:12.000000 pyfem-0.2.0/src/pyfem/amplitude/get_amplitude_data.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.117287 pyfem-0.2.0/src/pyfem/assembly/
--rw-rw-rw-   0        0        0    14782 2024-04-18 07:46:32.000000 pyfem-0.2.0/src/pyfem/assembly/Assembly.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/assembly/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.124787 pyfem-0.2.0/src/pyfem/bc/
--rw-rw-rw-   0        0        0     4148 2024-04-15 03:43:05.000000 pyfem-0.2.0/src/pyfem/bc/BaseBC.py
--rw-rw-rw-   0        0        0     3003 2024-04-18 05:44:17.000000 pyfem-0.2.0/src/pyfem/bc/DirichletBC.py
--rw-rw-rw-   0        0        0     2984 2024-04-18 05:43:15.000000 pyfem-0.2.0/src/pyfem/bc/NeumannBCConcentrated.py
--rw-rw-rw-   0        0        0    27073 2024-04-18 05:15:08.000000 pyfem-0.2.0/src/pyfem/bc/NeumannBCDistributed.py
--rw-rw-rw-   0        0        0    13073 2024-04-18 07:30:11.000000 pyfem-0.2.0/src/pyfem/bc/NeumannBCPressure.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/bc/__init__.py
--rw-rw-rw-   0        0        0     1049 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/bc/derive_surface_integral.py
--rw-rw-rw-   0        0        0     2087 2023-11-02 07:24:23.000000 pyfem-0.2.0/src/pyfem/bc/get_bc_data.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.133787 pyfem-0.2.0/src/pyfem/elements/
--rw-rw-rw-   0        0        0    20823 2024-04-17 06:35:13.000000 pyfem-0.2.0/src/pyfem/elements/BaseElement.py
--rw-rw-rw-   0        0        0    10336 2024-04-18 04:21:42.000000 pyfem-0.2.0/src/pyfem/elements/Diffusion.py
--rw-rw-rw-   0        0        0    76446 2024-01-17 03:37:48.000000 pyfem-0.2.0/src/pyfem/elements/SolidFiniteStrain.py
--rw-rw-rw-   0        0        0    18380 2024-04-18 07:24:12.000000 pyfem-0.2.0/src/pyfem/elements/SolidPhaseDamageSmallStrain.py
--rw-rw-rw-   0        0        0    12457 2024-04-18 04:25:16.000000 pyfem-0.2.0/src/pyfem/elements/SolidSmallStrain.py
--rw-rw-rw-   0        0        0    16473 2023-11-02 07:24:23.000000 pyfem-0.2.0/src/pyfem/elements/SolidThermalSmallStrain.py
--rw-rw-rw-   0        0        0     8419 2023-11-02 07:24:23.000000 pyfem-0.2.0/src/pyfem/elements/Thermal.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/elements/__init__.py
--rw-rw-rw-   0        0        0     3324 2024-04-08 03:47:57.000000 pyfem-0.2.0/src/pyfem/elements/get_element_data.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.136287 pyfem-0.2.0/src/pyfem/fem/
--rw-rw-rw-   0        0        0     2085 2023-09-07 09:41:11.000000 pyfem-0.2.0/src/pyfem/fem/Timer.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/fem/__init__.py
--rw-rw-rw-   0        0        0      344 2024-04-15 03:43:05.000000 pyfem-0.2.0/src/pyfem/fem/constants.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.151287 pyfem-0.2.0/src/pyfem/io/
--rw-rw-rw-   0        0        0     1124 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/io/Amplitude.py
--rw-rw-rw-   0        0        0     2136 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/io/BC.py
--rw-rw-rw-   0        0        0     1781 2023-11-02 07:24:37.000000 pyfem-0.2.0/src/pyfem/io/BaseIO.py
--rw-rw-rw-   0        0        0      994 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/io/Dof.py
--rw-rw-rw-   0        0        0     3071 2024-04-08 03:47:57.000000 pyfem-0.2.0/src/pyfem/io/Material.py
--rw-rw-rw-   0        0        0      802 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/io/Mesh.py
--rw-rw-rw-   0        0        0     1573 2023-09-19 07:05:17.000000 pyfem-0.2.0/src/pyfem/io/Module.py
--rw-rw-rw-   0        0        0     1065 2023-09-21 04:09:47.000000 pyfem-0.2.0/src/pyfem/io/Output.py
--rw-rw-rw-   0        0        0      672 2023-10-30 08:41:09.000000 pyfem-0.2.0/src/pyfem/io/Parameter.py
--rw-rw-rw-   0        0        0    12038 2024-04-11 06:14:41.000000 pyfem-0.2.0/src/pyfem/io/Properties.py
--rw-rw-rw-   0        0        0     2149 2023-09-15 03:47:33.000000 pyfem-0.2.0/src/pyfem/io/Section.py
--rw-rw-rw-   0        0        0     1952 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/io/Solver.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/io/__init__.py
--rw-rw-rw-   0        0        0     1647 2023-12-20 04:03:58.000000 pyfem-0.2.0/src/pyfem/io/arguments.py
--rw-rw-rw-   0        0        0     5213 2023-11-03 06:49:39.000000 pyfem-0.2.0/src/pyfem/io/write_hdf5.py
--rw-rw-rw-   0        0        0     5839 2024-01-15 09:02:18.000000 pyfem-0.2.0/src/pyfem/io/write_vtk.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.156787 pyfem-0.2.0/src/pyfem/isoelements/
--rw-rw-rw-   0        0        0     2320 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/isoelements/IsoElementDiagram.py
--rw-rw-rw-   0        0        0    21867 2024-03-28 07:30:52.000000 pyfem-0.2.0/src/pyfem/isoelements/IsoElementShape.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/isoelements/__init__.py
--rw-rw-rw-   0        0        0     1297 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/isoelements/derive_shape_functions.py
--rw-rw-rw-   0        0        0     2153 2023-11-02 07:24:49.000000 pyfem-0.2.0/src/pyfem/isoelements/get_iso_element_type.py
--rw-rw-rw-   0        0        0    27934 2024-03-28 07:20:41.000000 pyfem-0.2.0/src/pyfem/isoelements/shape_functions.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.169787 pyfem-0.2.0/src/pyfem/materials/
--rw-rw-rw-   0        0        0     3385 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/materials/BaseMaterial.py
--rw-rw-rw-   0        0        0     3135 2024-04-17 07:21:32.000000 pyfem-0.2.0/src/pyfem/materials/DiffusionIsotropic.py
--rw-rw-rw-   0        0        0     8776 2024-03-11 03:57:52.000000 pyfem-0.2.0/src/pyfem/materials/ElasticIsotropic.py
--rw-rw-rw-   0        0        0     3135 2023-11-02 07:24:49.000000 pyfem-0.2.0/src/pyfem/materials/MechanicalThermalExpansion.py
--rw-rw-rw-   0        0        0     2174 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/materials/PhaseFieldDamage.py
--rw-rw-rw-   0        0        0    79933 2024-01-17 03:37:48.000000 pyfem-0.2.0/src/pyfem/materials/PlasticCrystal.py
--rw-rw-rw-   0        0        0    91044 2024-01-17 03:37:48.000000 pyfem-0.2.0/src/pyfem/materials/PlasticCrystalGNDs.py
--rw-rw-rw-   0        0        0     8404 2023-09-21 06:20:49.000000 pyfem-0.2.0/src/pyfem/materials/PlasticKinematicHardening.py
--rw-rw-rw-   0        0        0     2773 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/materials/ThermalIsotropic.py
--rw-rw-rw-   0        0        0     6137 2023-09-19 06:25:05.000000 pyfem-0.2.0/src/pyfem/materials/UMAT.py
--rw-rw-rw-   0        0        0    10058 2023-10-27 05:19:05.000000 pyfem-0.2.0/src/pyfem/materials/ViscoElasticMaxwell.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/materials/__init__.py
--rw-rw-rw-   0        0        0    41881 2023-09-26 03:18:28.000000 pyfem-0.2.0/src/pyfem/materials/crystal_slip_system.py
--rw-rw-rw-   0        0        0     2613 2024-04-08 03:47:57.000000 pyfem-0.2.0/src/pyfem/materials/get_material_data.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.171787 pyfem-0.2.0/src/pyfem/mesh/
--rw-rw-rw-   0        0        0     8071 2024-04-18 04:24:18.000000 pyfem-0.2.0/src/pyfem/mesh/MeshData.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/mesh/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.179287 pyfem-0.2.0/src/pyfem/quadrature/
--rw-rw-rw-   0        0        0     1657 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/quadrature/BaseQuadrature.py
--rw-rw-rw-   0        0        0     2824 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/quadrature/GaussLegendreQuadrature.py
--rw-rw-rw-   0        0        0     1129 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/quadrature/PyramidQuadrature.py
--rw-rw-rw-   0        0        0    22842 2024-03-28 07:28:06.000000 pyfem-0.2.0/src/pyfem/quadrature/TetrahedronQuadrature.py
--rw-rw-rw-   0        0        0    27075 2024-03-28 07:27:55.000000 pyfem-0.2.0/src/pyfem/quadrature/TetrahedronQuadratureBarycentric.py
--rw-rw-rw-   0        0        0    25700 2024-03-28 04:13:23.000000 pyfem-0.2.0/src/pyfem/quadrature/TriangleQuadrature.py
--rw-rw-rw-   0        0        0    31453 2024-03-28 04:11:40.000000 pyfem-0.2.0/src/pyfem/quadrature/TriangleQuadratureBarycentric.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/quadrature/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.185287 pyfem-0.2.0/src/pyfem/solvers/
--rw-rw-rw-   0        0        0    15033 2024-04-18 07:31:18.000000 pyfem-0.2.0/src/pyfem/solvers/ArcLengthSolver.py
--rw-rw-rw-   0        0        0     1450 2023-11-01 04:20:15.000000 pyfem-0.2.0/src/pyfem/solvers/BaseSolver.py
--rw-rw-rw-   0        0        0     2225 2024-04-18 04:22:23.000000 pyfem-0.2.0/src/pyfem/solvers/LinearSolver.py
--rw-rw-rw-   0        0        0    16306 2024-04-18 07:30:49.000000 pyfem-0.2.0/src/pyfem/solvers/NonlinearSolver.py
--rw-rw-rw-   0        0        0    17321 2024-04-18 07:30:42.000000 pyfem-0.2.0/src/pyfem/solvers/TimeIntegrationNonlinearSolver.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/solvers/__init__.py
--rw-rw-rw-   0        0        0     1618 2024-04-15 07:19:03.000000 pyfem-0.2.0/src/pyfem/solvers/get_solver_data.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.191787 pyfem-0.2.0/src/pyfem/utils/
--rw-rw-rw-   0        0        0     2443 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/utils/IntKeyDict.py
--rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/utils/__init__.py
--rw-rw-rw-   0        0        0      957 2023-11-02 07:37:35.000000 pyfem-0.2.0/src/pyfem/utils/colors.py
--rw-rw-rw-   0        0        0     3374 2023-11-02 07:09:57.000000 pyfem-0.2.0/src/pyfem/utils/logger.py
--rw-rw-rw-   0        0        0    28928 2024-01-17 03:42:50.000000 pyfem-0.2.0/src/pyfem/utils/mechanics.py
--rw-rw-rw-   0        0        0     3941 2023-08-17 09:47:32.000000 pyfem-0.2.0/src/pyfem/utils/visualization.py
--rw-rw-rw-   0        0        0     1183 2023-11-01 09:41:59.000000 pyfem-0.2.0/src/pyfem/utils/wrappers.py
-drwxrwxrwx   0        0        0        0 2024-04-18 07:48:12.111287 pyfem-0.2.0/src/pyfem.egg-info/
--rw-rw-rw-   0        0        0     3579 2024-04-18 07:48:12.000000 pyfem-0.2.0/src/pyfem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3243 2024-04-18 07:48:12.000000 pyfem-0.2.0/src/pyfem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 07:48:12.000000 pyfem-0.2.0/src/pyfem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-18 07:48:12.000000 pyfem-0.2.0/src/pyfem.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-04-18 07:48:12.000000 pyfem-0.2.0/src/pyfem.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-18 07:48:12.000000 pyfem-0.2.0/src/pyfem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-22 08:34:00.221618 pyfem-0.2.1/
+-rw-rw-rw-   0        0        0     1190 2024-04-22 05:18:42.000000 pyfem-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     3686 2024-04-22 08:34:00.220623 pyfem-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-22 08:34:00.221618 pyfem-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1115 2023-08-17 09:47:32.000000 pyfem-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:33:59.625612 pyfem-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-22 08:33:59.634595 pyfem-0.2.1/src/pyfem/
+-rw-rw-rw-   0        0        0     2804 2023-11-01 09:09:41.000000 pyfem-0.2.1/src/pyfem/Job.py
+-rw-rw-rw-   0        0        0       23 2024-04-22 08:32:37.000000 pyfem-0.2.1/src/pyfem/__init__.py
+-rw-rw-rw-   0        0        0     1388 2023-11-02 07:31:58.000000 pyfem-0.2.1/src/pyfem/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:33:59.687406 pyfem-0.2.1/src/pyfem/amplitude/
+-rw-rw-rw-   0        0        0     1403 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/amplitude/BaseAmplitude.py
+-rw-rw-rw-   0        0        0     1892 2023-11-02 07:24:23.000000 pyfem-0.2.1/src/pyfem/amplitude/TabularAmplitude.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/amplitude/__init__.py
+-rw-rw-rw-   0        0        0     1112 2023-11-02 07:24:12.000000 pyfem-0.2.1/src/pyfem/amplitude/get_amplitude_data.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:33:59.690396 pyfem-0.2.1/src/pyfem/assembly/
+-rw-rw-rw-   0        0        0    14782 2024-04-18 07:46:32.000000 pyfem-0.2.1/src/pyfem/assembly/Assembly.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/assembly/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:33:59.747204 pyfem-0.2.1/src/pyfem/bc/
+-rw-rw-rw-   0        0        0     4148 2024-04-15 03:43:05.000000 pyfem-0.2.1/src/pyfem/bc/BaseBC.py
+-rw-rw-rw-   0        0        0     3003 2024-04-18 05:44:17.000000 pyfem-0.2.1/src/pyfem/bc/DirichletBC.py
+-rw-rw-rw-   0        0        0     2984 2024-04-18 05:43:15.000000 pyfem-0.2.1/src/pyfem/bc/NeumannBCConcentrated.py
+-rw-rw-rw-   0        0        0    27073 2024-04-18 05:15:08.000000 pyfem-0.2.1/src/pyfem/bc/NeumannBCDistributed.py
+-rw-rw-rw-   0        0        0    13073 2024-04-18 07:30:11.000000 pyfem-0.2.1/src/pyfem/bc/NeumannBCPressure.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/bc/__init__.py
+-rw-rw-rw-   0        0        0     1049 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/bc/derive_surface_integral.py
+-rw-rw-rw-   0        0        0     2087 2023-11-02 07:24:23.000000 pyfem-0.2.1/src/pyfem/bc/get_bc_data.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:33:59.770208 pyfem-0.2.1/src/pyfem/elements/
+-rw-rw-rw-   0        0        0    20958 2024-04-22 08:22:10.000000 pyfem-0.2.1/src/pyfem/elements/BaseElement.py
+-rw-rw-rw-   0        0        0    10270 2024-04-22 06:34:05.000000 pyfem-0.2.1/src/pyfem/elements/Diffusion.py
+-rw-rw-rw-   0        0        0    76446 2024-01-17 03:37:48.000000 pyfem-0.2.1/src/pyfem/elements/SolidFiniteStrain.py
+-rw-rw-rw-   0        0        0    18134 2024-04-22 06:52:14.000000 pyfem-0.2.1/src/pyfem/elements/SolidPhaseDamageSmallStrain.py
+-rw-rw-rw-   0        0        0    12134 2024-04-22 08:23:28.000000 pyfem-0.2.1/src/pyfem/elements/SolidSmallStrain.py
+-rw-rw-rw-   0        0        0    16046 2024-04-22 06:32:26.000000 pyfem-0.2.1/src/pyfem/elements/SolidThermalSmallStrain.py
+-rw-rw-rw-   0        0        0     8255 2024-04-22 05:25:42.000000 pyfem-0.2.1/src/pyfem/elements/Thermal.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/elements/__init__.py
+-rw-rw-rw-   0        0        0     3324 2024-04-08 03:47:57.000000 pyfem-0.2.1/src/pyfem/elements/get_element_data.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:33:59.783088 pyfem-0.2.1/src/pyfem/fem/
+-rw-rw-rw-   0        0        0     2085 2023-09-07 09:41:11.000000 pyfem-0.2.1/src/pyfem/fem/Timer.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/fem/__init__.py
+-rw-rw-rw-   0        0        0      344 2024-04-15 03:43:05.000000 pyfem-0.2.1/src/pyfem/fem/constants.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:33:59.877771 pyfem-0.2.1/src/pyfem/io/
+-rw-rw-rw-   0        0        0     1124 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/io/Amplitude.py
+-rw-rw-rw-   0        0        0     2136 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/io/BC.py
+-rw-rw-rw-   0        0        0     1781 2023-11-02 07:24:37.000000 pyfem-0.2.1/src/pyfem/io/BaseIO.py
+-rw-rw-rw-   0        0        0      994 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/io/Dof.py
+-rw-rw-rw-   0        0        0     3071 2024-04-08 03:47:57.000000 pyfem-0.2.1/src/pyfem/io/Material.py
+-rw-rw-rw-   0        0        0      802 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/io/Mesh.py
+-rw-rw-rw-   0        0        0     1573 2023-09-19 07:05:17.000000 pyfem-0.2.1/src/pyfem/io/Module.py
+-rw-rw-rw-   0        0        0     1065 2023-09-21 04:09:47.000000 pyfem-0.2.1/src/pyfem/io/Output.py
+-rw-rw-rw-   0        0        0      672 2023-10-30 08:41:09.000000 pyfem-0.2.1/src/pyfem/io/Parameter.py
+-rw-rw-rw-   0        0        0    12038 2024-04-11 06:14:41.000000 pyfem-0.2.1/src/pyfem/io/Properties.py
+-rw-rw-rw-   0        0        0     2149 2023-09-15 03:47:33.000000 pyfem-0.2.1/src/pyfem/io/Section.py
+-rw-rw-rw-   0        0        0     1952 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/io/Solver.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/io/__init__.py
+-rw-rw-rw-   0        0        0     1647 2023-12-20 04:03:58.000000 pyfem-0.2.1/src/pyfem/io/arguments.py
+-rw-rw-rw-   0        0        0     5213 2023-11-03 06:49:39.000000 pyfem-0.2.1/src/pyfem/io/write_hdf5.py
+-rw-rw-rw-   0        0        0     5839 2024-01-15 09:02:18.000000 pyfem-0.2.1/src/pyfem/io/write_vtk.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:33:59.918631 pyfem-0.2.1/src/pyfem/isoelements/
+-rw-rw-rw-   0        0        0     2320 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/isoelements/IsoElementDiagram.py
+-rw-rw-rw-   0        0        0    21867 2024-03-28 07:30:52.000000 pyfem-0.2.1/src/pyfem/isoelements/IsoElementShape.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/isoelements/__init__.py
+-rw-rw-rw-   0        0        0     1297 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/isoelements/derive_shape_functions.py
+-rw-rw-rw-   0        0        0     2153 2023-11-02 07:24:49.000000 pyfem-0.2.1/src/pyfem/isoelements/get_iso_element_type.py
+-rw-rw-rw-   0        0        0    27934 2024-03-28 07:20:41.000000 pyfem-0.2.1/src/pyfem/isoelements/shape_functions.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:34:00.026271 pyfem-0.2.1/src/pyfem/materials/
+-rw-rw-rw-   0        0        0     3385 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/materials/BaseMaterial.py
+-rw-rw-rw-   0        0        0     3135 2024-04-17 07:21:32.000000 pyfem-0.2.1/src/pyfem/materials/DiffusionIsotropic.py
+-rw-rw-rw-   0        0        0     8776 2024-03-11 03:57:52.000000 pyfem-0.2.1/src/pyfem/materials/ElasticIsotropic.py
+-rw-rw-rw-   0        0        0     3135 2023-11-02 07:24:49.000000 pyfem-0.2.1/src/pyfem/materials/MechanicalThermalExpansion.py
+-rw-rw-rw-   0        0        0     2174 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/materials/PhaseFieldDamage.py
+-rw-rw-rw-   0        0        0    79933 2024-01-17 03:37:48.000000 pyfem-0.2.1/src/pyfem/materials/PlasticCrystal.py
+-rw-rw-rw-   0        0        0    91044 2024-01-17 03:37:48.000000 pyfem-0.2.1/src/pyfem/materials/PlasticCrystalGNDs.py
+-rw-rw-rw-   0        0        0     8404 2023-09-21 06:20:49.000000 pyfem-0.2.1/src/pyfem/materials/PlasticKinematicHardening.py
+-rw-rw-rw-   0        0        0     2773 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/materials/ThermalIsotropic.py
+-rw-rw-rw-   0        0        0     6137 2023-09-19 06:25:05.000000 pyfem-0.2.1/src/pyfem/materials/UMAT.py
+-rw-rw-rw-   0        0        0    10058 2023-10-27 05:19:05.000000 pyfem-0.2.1/src/pyfem/materials/ViscoElasticMaxwell.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/materials/__init__.py
+-rw-rw-rw-   0        0        0    41881 2023-09-26 03:18:28.000000 pyfem-0.2.1/src/pyfem/materials/crystal_slip_system.py
+-rw-rw-rw-   0        0        0     2613 2024-04-08 03:47:57.000000 pyfem-0.2.1/src/pyfem/materials/get_material_data.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:34:00.029261 pyfem-0.2.1/src/pyfem/mesh/
+-rw-rw-rw-   0        0        0     8071 2024-04-18 04:24:18.000000 pyfem-0.2.1/src/pyfem/mesh/MeshData.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/mesh/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:34:00.116971 pyfem-0.2.1/src/pyfem/quadrature/
+-rw-rw-rw-   0        0        0     1657 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/quadrature/BaseQuadrature.py
+-rw-rw-rw-   0        0        0     2824 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/quadrature/GaussLegendreQuadrature.py
+-rw-rw-rw-   0        0        0     1129 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/quadrature/PyramidQuadrature.py
+-rw-rw-rw-   0        0        0    22842 2024-03-28 07:28:06.000000 pyfem-0.2.1/src/pyfem/quadrature/TetrahedronQuadrature.py
+-rw-rw-rw-   0        0        0    27075 2024-03-28 07:27:55.000000 pyfem-0.2.1/src/pyfem/quadrature/TetrahedronQuadratureBarycentric.py
+-rw-rw-rw-   0        0        0    25700 2024-03-28 04:13:23.000000 pyfem-0.2.1/src/pyfem/quadrature/TriangleQuadrature.py
+-rw-rw-rw-   0        0        0    31453 2024-03-28 04:11:40.000000 pyfem-0.2.1/src/pyfem/quadrature/TriangleQuadratureBarycentric.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/quadrature/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:34:00.163811 pyfem-0.2.1/src/pyfem/solvers/
+-rw-rw-rw-   0        0        0    15033 2024-04-18 07:31:18.000000 pyfem-0.2.1/src/pyfem/solvers/ArcLengthSolver.py
+-rw-rw-rw-   0        0        0     1450 2023-11-01 04:20:15.000000 pyfem-0.2.1/src/pyfem/solvers/BaseSolver.py
+-rw-rw-rw-   0        0        0     2225 2024-04-18 04:22:23.000000 pyfem-0.2.1/src/pyfem/solvers/LinearSolver.py
+-rw-rw-rw-   0        0        0    16305 2024-04-22 08:32:01.000000 pyfem-0.2.1/src/pyfem/solvers/NonlinearSolver.py
+-rw-rw-rw-   0        0        0    17321 2024-04-18 07:30:42.000000 pyfem-0.2.1/src/pyfem/solvers/TimeIntegrationNonlinearSolver.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/solvers/__init__.py
+-rw-rw-rw-   0        0        0     1618 2024-04-15 07:19:03.000000 pyfem-0.2.1/src/pyfem/solvers/get_solver_data.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:34:00.218628 pyfem-0.2.1/src/pyfem/utils/
+-rw-rw-rw-   0        0        0     2443 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/utils/IntKeyDict.py
+-rw-rw-rw-   0        0        0        0 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/utils/__init__.py
+-rw-rw-rw-   0        0        0      957 2023-11-02 07:37:35.000000 pyfem-0.2.1/src/pyfem/utils/colors.py
+-rw-rw-rw-   0        0        0     3374 2023-11-02 07:09:57.000000 pyfem-0.2.1/src/pyfem/utils/logger.py
+-rw-rw-rw-   0        0        0    28928 2024-01-17 03:42:50.000000 pyfem-0.2.1/src/pyfem/utils/mechanics.py
+-rw-rw-rw-   0        0        0     3941 2023-08-17 09:47:32.000000 pyfem-0.2.1/src/pyfem/utils/visualization.py
+-rw-rw-rw-   0        0        0     1183 2023-11-01 09:41:59.000000 pyfem-0.2.1/src/pyfem/utils/wrappers.py
+drwxrwxrwx   0        0        0        0 2024-04-22 08:33:59.663484 pyfem-0.2.1/src/pyfem.egg-info/
+-rw-rw-rw-   0        0        0     3686 2024-04-22 08:33:59.000000 pyfem-0.2.1/src/pyfem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3243 2024-04-22 08:33:59.000000 pyfem-0.2.1/src/pyfem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 08:33:59.000000 pyfem-0.2.1/src/pyfem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-22 08:33:59.000000 pyfem-0.2.1/src/pyfem.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-04-22 08:33:59.000000 pyfem-0.2.1/src/pyfem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-22 08:33:59.000000 pyfem-0.2.1/src/pyfem.egg-info/top_level.txt
```

### Comparing `pyfem-0.2.0/PKG-INFO` & `pyfem-0.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfem
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python Finite Element Method
 Home-page: https://github.com/sunwhale/pyfem
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,34 +13,43 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyfem
 
 pyfem是一个完全基于python语言实现的极简有限元求解器。依赖的第三方库包括numpy、scipy和meshio等，主要用于有限元方法的学习、有限元算法验证和快速建立材料本构模型的程序原型。
 
+Github仓库：https://github.com/sunwhale/pyfem
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/ab5bca55d85d45d4aa4336ccae058316)](https://app.codacy.com/gh/sunwhale/pyfem/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 
+## Contact 联系方式
+电子邮箱 E-mail：sunjingyu@imech.ac.cn
+
+作者主页 Homepage: https://people.ucas.edu.cn/~sunjingyu
+
 ## Installation 安装
 
 支持的操作系统包括：Windows，Linux和MacOS。
 
 ### Recommend 推荐
 
 Use the package manager [pip](https://pypi.org/project/pyfem/) to install pyfem:
 
 使用pip命令安装:
 
 ```bash
-pip install pyfem
+pip install -U pyfem
 ```
 
 If you have no root access on Linux/MacOS, please try
+
+如果你在Linux/MacOS上没有root访问权限，请尝试
+
 ```bash
-python -m pip install pyfem
+python -m pip install -U pyfem
 ```
 
 Users in China can install pyfem from mirrors such as:
 
 中国用户可以使用以下镜像:
 - [Aliyun](https://developer.aliyun.com/mirror/pypi)
 - [Tsinghua](https://mirrors.tuna.tsinghua.edu.cn/help/pypi/)
@@ -56,15 +65,18 @@
 or 或者
 
 ```bash
 git clone https://github.com/sunwhale/pyfem.git
 cd pyfem
 python install.py
 ```
-采用第二种方法需要将可执行文件或批处理文件写入环境变量。
+
+Using the "From Source" approach will generate executable files or batch files, which can then have their paths added to the system environment variables.
+
+采用基于源代码的方法会生成可执行文件或批处理文件，可将其路径写入系统环境变量。
 
 ## Quickstart 快速开始
 
 ### Run in command line 在命令行运行:
 
 ```bash
 pyfem --help
@@ -75,42 +87,35 @@
 当前算例文件存储目录 examples/tutorial，该算例定义了一个二维平面应变模型，材料为塑性随动强化，载荷为y方向的循环拉伸-压缩。
 
 ```bash
 cd examples/tutorial
 pyfem -i Job-1.toml
 ```
 
-## 后处理
+## Postproc 后处理
 
 算例计算完成后将在配置文件所在目录下生成 .pvd 或 .vtu文件，可以使用开源可视化软件 [paraview](https://www.paraview.org/download/) 进行查看。
 
-## 前处理
+## Preproc 前处理
 
 本项目暂不提供前处理模块，基于 meshio 库，可以识别[gmsh](https://www.gmsh.info/)、abaqus 和 ansys等有限元软件的网格文件。
 
 ## Documents 帮助文档
-[https://pyfem-doc.readthedocs.io/](https://pyfem-doc.readthedocs.io/)
 
-## Development
+[帮助文档](https://pyfem-doc.readthedocs.io/)中给出了详细的理论公式和函数说明。
+
+
+
+## Development 开发
 
 ### ToDo list
 
-- [x] 增加Neumann边界条件，支持concentrated force，distributed和pressure定义方式
+- [ ] 增加如何建立toml算例文件的帮助文档
 - [ ] 增加hdf5计算结果输出格式
-- [ ] 完善帮助文档
-- [ ] 完善输入文件的校检
-- [x] 增加测试模块
-- [x] 增加日志模块
-- [x] 增加后台运行模式
 - [ ] 处理平面应力状态的面外应力平衡
-- [x] 增加粘弹性力学本构模型
-- [x] 增加晶体塑性力学本构模型
-- [x] 增加温度场求解单元
-- [x] 增加温度场-位移场耦合求解单元
-- [x] 增加相场-位移场耦合求解单元
 - [ ] 增加内聚区单元
 - [ ] 增加动力学求解器
 - [ ] 建立前处理界面
 
 ### Bug list
 
 - [ ] 采用abaqus网格文件时，如果存在node不属于任何element则在计算时会导致全局刚度矩阵奇异。
```

### Comparing `pyfem-0.2.0/setup.py` & `pyfem-0.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/Job.py` & `pyfem-0.2.1/src/pyfem/Job.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/__main__.py` & `pyfem-0.2.1/src/pyfem/__main__.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/amplitude/BaseAmplitude.py` & `pyfem-0.2.1/src/pyfem/amplitude/BaseAmplitude.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/amplitude/TabularAmplitude.py` & `pyfem-0.2.1/src/pyfem/amplitude/TabularAmplitude.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/amplitude/get_amplitude_data.py` & `pyfem-0.2.1/src/pyfem/amplitude/get_amplitude_data.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/assembly/Assembly.py` & `pyfem-0.2.1/src/pyfem/assembly/Assembly.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/bc/BaseBC.py` & `pyfem-0.2.1/src/pyfem/bc/BaseBC.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/bc/DirichletBC.py` & `pyfem-0.2.1/src/pyfem/bc/DirichletBC.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/bc/NeumannBCConcentrated.py` & `pyfem-0.2.1/src/pyfem/bc/NeumannBCConcentrated.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/bc/NeumannBCDistributed.py` & `pyfem-0.2.1/src/pyfem/bc/NeumannBCDistributed.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/bc/NeumannBCPressure.py` & `pyfem-0.2.1/src/pyfem/bc/NeumannBCPressure.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/bc/derive_surface_integral.py` & `pyfem-0.2.1/src/pyfem/bc/derive_surface_integral.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/bc/get_bc_data.py` & `pyfem-0.2.1/src/pyfem/bc/get_bc_data.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/elements/BaseElement.py` & `pyfem-0.2.1/src/pyfem/elements/BaseElement.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,15 +304,15 @@
             self.qp_jacobi_dets = det(self.qp_jacobis)
             # qp_jacobi通常为2×2或3×3的方阵，可以直接根据解析式求逆矩阵，计算效率比numpy.linalg.inv()函数更高
             self.qp_jacobi_invs = inverse(self.qp_jacobis, self.qp_jacobi_dets)
             self.qp_weight_times_jacobi_dets = self.iso_element_shape.qp_weights * self.qp_jacobi_dets
 
             # qp_dhdxes = []
             # for iqp, (qp_shape_gradient, qp_jacobi_inv) in enumerate(zip(self.iso_element_shape.qp_shape_gradients, self.qp_jacobi_invs)):
-            #     qp_dhdxes.append(dot(qp_shape_gradient.transpose(), qp_jacobi_inv))
+            #     qp_dhdxes.append(dot(qp_shape_gradient.transpose(), qp_jacobi_inv).transpose())
             # self.qp_dhdxes = array(qp_dhdxes)
             self.qp_dhdxes = einsum('...ij,...ik->...kj', self.iso_element_shape.qp_shape_gradients, self.qp_jacobi_invs)
 
         elif self.iso_element_shape.coord_type == 'barycentric':
             self.qp_jacobis = dot(self.iso_element_shape.qp_shape_gradients, self.node_coords).swapaxes(1, 2)
             new_rows = ones((self.qp_jacobis.shape[0], 1, self.qp_jacobis.shape[2]))
             self.qp_jacobis = concatenate((new_rows, self.qp_jacobis), axis=1)
@@ -321,14 +321,15 @@
             elif self.dimension == 3:
                 a = array([[0.0, 0.0, 0.0], [1.0, 0.0, 0.0], [0.0, 1.0, 0.0], [0.0, 0.0, 1.0]])
             else:
                 raise NotImplementedError(error_style(f'dimension {self.dimension} is not support for the barycentric coordinates'))
             self.qp_jacobi_dets = det(self.qp_jacobis)
             self.qp_jacobi_invs = inverse(self.qp_jacobis, self.qp_jacobi_dets)
             self.qp_jacobi_invs = dot(self.qp_jacobi_invs, a)
+            self.qp_dhdxes = einsum('...ij,...ik->...kj', self.iso_element_shape.qp_shape_gradients, self.qp_jacobi_invs)
             if self.dimension == 2:
                 self.qp_weight_times_jacobi_dets = self.iso_element_shape.qp_weights * self.qp_jacobi_dets / 2.0
             elif self.dimension == 3:
                 self.qp_weight_times_jacobi_dets = self.iso_element_shape.qp_weights * self.qp_jacobi_dets / 6.0
             else:
                 raise NotImplementedError(error_style(f'dimension {self.dimension} is not support for the barycentric coordinates'))
```

### Comparing `pyfem-0.2.0/src/pyfem/elements/Diffusion.py` & `pyfem-0.2.1/src/pyfem/elements/Diffusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,14 @@
         dtime = timer.dtime
 
         qp_number = self.qp_number
         qp_weight_times_jacobi_dets = self.qp_weight_times_jacobi_dets
         qp_shape_values = self.iso_element_shape.qp_shape_values
         qp_shape_gradients = self.iso_element_shape.qp_shape_gradients
         qp_dhdxex = self.qp_dhdxes
-        qp_jacobi_invs = self.qp_jacobi_invs
 
         qp_state_variables = self.qp_state_variables
         qp_state_variables_new = self.qp_state_variables_new
 
         element_dof_values = self.element_dof_values
         element_ddof_values = self.element_ddof_values
 
@@ -139,16 +138,16 @@
             if is_update_material:
                 qp_weight_times_jacobi_det = qp_weight_times_jacobi_dets[i]
                 qp_shape_value = qp_shape_values[i]
                 qp_shape_gradient = qp_shape_gradients[i]
                 qp_dhdx = qp_dhdxex[i]
                 qp_concentration = dot(qp_shape_value, element_dof_values)
                 qp_dconcentration = dot(qp_shape_value, element_ddof_values)
-                qp_concentration_gradient = dot(qp_shape_gradient, element_dof_values)
-                qp_dconcentration_gradient = dot(qp_shape_gradient, element_ddof_values)
+                qp_concentration_gradient = dot(qp_dhdx, element_dof_values)
+                qp_dconcentration_gradient = dot(qp_dhdx, element_ddof_values)
 
                 variable = {'concentration': qp_concentration,
                             'dconcentration': qp_dconcentration,
                             'concentration_gradient': qp_concentration_gradient,
                             'dconcentration_gradient': qp_dconcentration_gradient}
                 qp_ddsddc, qp_output = material_data.get_tangent(variable=variable,
                                                                  state_variable=qp_state_variables[i],
```

### Comparing `pyfem-0.2.0/src/pyfem/elements/SolidFiniteStrain.py` & `pyfem-0.2.1/src/pyfem/elements/SolidFiniteStrain.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/elements/SolidPhaseDamageSmallStrain.py` & `pyfem-0.2.1/src/pyfem/elements/SolidPhaseDamageSmallStrain.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,24 +234,23 @@
             self.qp_phase_fluxes = list()
             self.qp_energies = list()
 
         for i in range(qp_number):
             if is_update_material:
                 qp_weight_times_jacobi_det = qp_weight_times_jacobi_dets[i]
                 qp_shape_value = qp_shape_values[i]
-                qp_shape_gradient = qp_shape_gradients[i]
                 qp_dhdx = qp_dhdxes[i]
                 qp_b_matrix_transpose = qp_b_matrices_transpose[i]
                 qp_b_matrix = qp_b_matrices[i]
                 qp_strain = dot(qp_b_matrix, u)
                 qp_dstrain = dot(qp_b_matrix, du)
                 qp_phase = dot(qp_shape_value, phi)
                 qp_dphase = dot(qp_shape_value, dphi)
-                qp_phase_gradient = dot(qp_shape_gradient, phi)
-                qp_dphase_gradient = dot(qp_shape_gradient, dphi)
+                qp_phase_gradient = dot(qp_dhdx, phi)
+                qp_dphase_gradient = dot(qp_dhdx, dphi)
 
                 qp_degradation = (1.0 - qp_phase) ** 2 + 1.0e-8
                 qp_degradation = min(qp_degradation, 1.0)
                 qp_degradation = max(qp_degradation, 0.0)
 
                 variable = {'strain': qp_strain, 'dstrain': qp_dstrain}
                 qp_ddsdde, qp_output = solid_material_data.get_tangent(variable=variable,
@@ -271,25 +270,23 @@
                 self.qp_phases.append(qp_phase)
 
             else:
                 qp_b_matrix_transpose = qp_b_matrices_transpose[i]
                 qp_b_matrix = qp_b_matrices[i]
                 qp_weight_times_jacobi_det = qp_weight_times_jacobi_dets[i]
                 qp_shape_value = qp_shape_values[i]
-                qp_shape_gradient = qp_shape_gradients[i]
+                qp_dhdx = qp_dhdxes[i]
                 qp_ddsdde = self.qp_ddsddes[i]
                 qp_stress = self.qp_stresses[i]
                 qp_strain = dot(qp_b_matrix, u)
                 qp_dstrain = dot(qp_b_matrix, du)
                 qp_phase = dot(qp_shape_value, phi)
                 qp_dphase = dot(qp_shape_value, dphi)
-                qp_phase_gradient = dot(qp_shape_gradient, phi)
-                qp_dphase_gradient = dot(qp_shape_gradient, dphi)
-                qp_jacobi_inv = qp_jacobi_invs[i]
-                qp_dhdx = dot(qp_shape_gradient.transpose(), qp_jacobi_inv)
+                qp_phase_gradient = dot(qp_dhdx, phi)
+                qp_dphase_gradient = dot(qp_dhdx, dphi)
 
                 qp_degradation = (1.0 - qp_phase) ** 2 + 1.0e-8
                 qp_degradation = min(qp_degradation, 1.0)
                 qp_degradation = max(qp_degradation, 0.0)
 
             # energy_positive, energy_negative = get_decompose_energy(qp_strain + qp_dstrain, qp_stress, dimension)
             # energy_positive += qp_strain_energy
```

### Comparing `pyfem-0.2.0/src/pyfem/elements/SolidSmallStrain.py` & `pyfem-0.2.1/src/pyfem/elements/SolidSmallStrain.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,29 +116,25 @@
         self.qp_stresses: list[ndarray] = None  # type: ignore
 
         self.create_qp_b_matrices()
 
     def create_qp_b_matrices(self) -> None:
         if self.dimension == 2:
             self.qp_b_matrices = zeros(shape=(self.qp_number, 3, self.element_dof_number), dtype=DTYPE)
-            for iqp, (qp_shape_gradient, qp_jacobi_inv) in \
-                    enumerate(zip(self.iso_element_shape.qp_shape_gradients, self.qp_jacobi_invs)):
-                qp_dhdx = dot(qp_shape_gradient.transpose(), qp_jacobi_inv)
-                for i, val in enumerate(qp_dhdx):
+            for iqp, qp_dhdx in enumerate(self.qp_dhdxes):
+                for i, val in enumerate(qp_dhdx.transpose()):
                     self.qp_b_matrices[iqp, 0, i * 2 + 0] = val[0]
                     self.qp_b_matrices[iqp, 1, i * 2 + 1] = val[1]
                     self.qp_b_matrices[iqp, 2, i * 2 + 0] = val[1]
                     self.qp_b_matrices[iqp, 2, i * 2 + 1] = val[0]
 
         elif self.dimension == 3:
-            self.qp_b_matrices = zeros(shape=(self.iso_element_shape.qp_number, 6, self.element_dof_number))
-            for iqp, (qp_shape_gradient, qp_jacobi_inv) in \
-                    enumerate(zip(self.iso_element_shape.qp_shape_gradients, self.qp_jacobi_invs)):
-                qp_dhdx = dot(qp_shape_gradient.transpose(), qp_jacobi_inv)
-                for i, val in enumerate(qp_dhdx):
+            self.qp_b_matrices = zeros(shape=(self.iso_element_shape.qp_number, 6, self.element_dof_number), dtype=DTYPE)
+            for iqp, qp_dhdx in enumerate(self.qp_dhdxes):
+                for i, val in enumerate(qp_dhdx.transpose()):
                     self.qp_b_matrices[iqp, 0, i * 3 + 0] = val[0]
                     self.qp_b_matrices[iqp, 1, i * 3 + 1] = val[1]
                     self.qp_b_matrices[iqp, 2, i * 3 + 2] = val[2]
                     self.qp_b_matrices[iqp, 3, i * 3 + 0] = val[1]
                     self.qp_b_matrices[iqp, 3, i * 3 + 1] = val[0]
                     self.qp_b_matrices[iqp, 4, i * 3 + 0] = val[2]
                     self.qp_b_matrices[iqp, 4, i * 3 + 2] = val[0]
```

### Comparing `pyfem-0.2.0/src/pyfem/elements/SolidThermalSmallStrain.py` & `pyfem-0.2.1/src/pyfem/elements/SolidThermalSmallStrain.py`

 * *Files 5% similar despite different names*

```diff
@@ -122,35 +122,31 @@
             self.dof_T += [len(self.dof_names) * i + 2]
 
         self.create_qp_b_matrices()
 
     def create_qp_b_matrices(self) -> None:
         if self.dimension == 2:
             self.qp_b_matrices = zeros(shape=(self.qp_number, 3, len(self.dof_u)), dtype=DTYPE)
-            for iqp, (qp_shape_gradient, qp_jacobi_inv) in \
-                    enumerate(zip(self.iso_element_shape.qp_shape_gradients, self.qp_jacobi_invs)):
-                qp_dhdx = dot(qp_shape_gradient.transpose(), qp_jacobi_inv)
-                for i, val in enumerate(qp_dhdx):
-                    self.qp_b_matrices[iqp, 0, i * 2] = val[0]
+            for iqp, qp_dhdx in enumerate(self.qp_dhdxes):
+                for i, val in enumerate(qp_dhdx.transpose()):
+                    self.qp_b_matrices[iqp, 0, i * 2 + 0] = val[0]
                     self.qp_b_matrices[iqp, 1, i * 2 + 1] = val[1]
-                    self.qp_b_matrices[iqp, 2, i * 2] = val[1]
+                    self.qp_b_matrices[iqp, 2, i * 2 + 0] = val[1]
                     self.qp_b_matrices[iqp, 2, i * 2 + 1] = val[0]
 
         elif self.dimension == 3:
-            self.qp_b_matrices = zeros(shape=(self.iso_element_shape.qp_number, 6, len(self.dof_u)))
-            for iqp, (qp_shape_gradient, qp_jacobi_inv) in \
-                    enumerate(zip(self.iso_element_shape.qp_shape_gradients, self.qp_jacobi_invs)):
-                qp_dhdx = dot(qp_shape_gradient.transpose(), qp_jacobi_inv)
-                for i, val in enumerate(qp_dhdx):
-                    self.qp_b_matrices[iqp, 0, i * 3] = val[0]
+            self.qp_b_matrices = zeros(shape=(self.iso_element_shape.qp_number, 6, len(self.dof_u)), dtype=DTYPE)
+            for iqp, qp_dhdx in enumerate(self.qp_dhdxes):
+                for i, val in enumerate(qp_dhdx.transpose()):
+                    self.qp_b_matrices[iqp, 0, i * 3 + 0] = val[0]
                     self.qp_b_matrices[iqp, 1, i * 3 + 1] = val[1]
                     self.qp_b_matrices[iqp, 2, i * 3 + 2] = val[2]
-                    self.qp_b_matrices[iqp, 3, i * 3] = val[1]
+                    self.qp_b_matrices[iqp, 3, i * 3 + 0] = val[1]
                     self.qp_b_matrices[iqp, 3, i * 3 + 1] = val[0]
-                    self.qp_b_matrices[iqp, 4, i * 3] = val[2]
+                    self.qp_b_matrices[iqp, 4, i * 3 + 0] = val[2]
                     self.qp_b_matrices[iqp, 4, i * 3 + 2] = val[0]
                     self.qp_b_matrices[iqp, 5, i * 3 + 1] = val[2]
                     self.qp_b_matrices[iqp, 5, i * 3 + 2] = val[1]
 
         self.qp_b_matrices_transpose = array([qp_b_matrix.transpose() for qp_b_matrix in self.qp_b_matrices])
 
     def update_element_material_stiffness_fint(self,
@@ -161,15 +157,15 @@
         timer = self.timer
         ntens = self.ntens
         ndi = self.ndi
         nshr = self.nshr
 
         qp_number = self.qp_number
         qp_shape_values = self.iso_element_shape.qp_shape_values
-        qp_shape_gradients = self.iso_element_shape.qp_shape_gradients
+        qp_dhdxes = self.qp_dhdxes
         qp_b_matrices = self.qp_b_matrices
         qp_b_matrices_transpose = self.qp_b_matrices_transpose
         qp_weight_times_jacobi_dets = self.qp_weight_times_jacobi_dets
 
         qp_state_variables = self.qp_state_variables
         qp_state_variables_new = self.qp_state_variables_new
 
@@ -249,19 +245,19 @@
             self.qp_temperatures = list()
             self.qp_heat_fluxes = list()
 
         for i in range(qp_number):
             if is_update_material:
                 qp_weight_times_jacobi_det = qp_weight_times_jacobi_dets[i]
                 qp_shape_value = qp_shape_values[i]
-                qp_shape_gradient = qp_shape_gradients[i]
+                qp_dhdx = qp_dhdxes[i]
                 qp_temperature = dot(qp_shape_value, T)
                 qp_dtemperature = dot(qp_shape_value, dT)
-                qp_temperature_gradient = dot(qp_shape_gradient, T)
-                qp_dtemperature_gradient = dot(qp_shape_gradient, dT)
+                qp_temperature_gradient = dot(qp_dhdx, T)
+                qp_dtemperature_gradient = dot(qp_dhdx, dT)
 
                 variable = {'temperature': qp_temperature,
                             'dtemperature': qp_dtemperature,
                             'temperature_gradient': qp_temperature_gradient,
                             'dtemperature_gradient': qp_dtemperature_gradient}
                 qp_ddsddt, qp_output = thermal_material_data.get_tangent(variable=variable,
                                                                          state_variable=qp_state_variables[i],
@@ -274,25 +270,25 @@
                                                                          timer=timer)
                 qp_heat_flux = qp_output['heat_flux']
                 self.qp_ddsddts.append(qp_ddsddt)
                 self.qp_temperatures.append(qp_temperature)
                 self.qp_heat_fluxes.append(qp_heat_flux)
             else:
                 qp_weight_times_jacobi_det = qp_weight_times_jacobi_dets[i]
-                qp_shape_gradient = qp_shape_gradients[i]
+                qp_dhdx = qp_dhdxes[i]
                 qp_ddsddt = self.qp_ddsddts[i]
                 qp_heat_flux = self.qp_heat_fluxes[i]
 
             if is_update_stiffness:
                 self.element_stiffness[ix_(self.dof_T, self.dof_T)] += \
-                    dot(qp_shape_gradient.transpose(), dot(qp_ddsddt, qp_shape_gradient)) * qp_weight_times_jacobi_det
+                    dot(qp_dhdx.transpose(), dot(qp_ddsddt, qp_dhdx)) * qp_weight_times_jacobi_det
 
             if is_update_fint:
                 self.element_fint[self.dof_T] += \
-                    dot(qp_shape_gradient.transpose(), qp_heat_flux) * qp_weight_times_jacobi_det
+                    dot(qp_dhdx.transpose(), qp_heat_flux) * qp_weight_times_jacobi_det
 
     def update_element_field_variables(self) -> None:
         qp_stresses = self.qp_stresses
         qp_strains = self.qp_strains
 
         average_strain = average(qp_strains, axis=0)
         average_stress = average(qp_stresses, axis=0)
```

### Comparing `pyfem-0.2.0/src/pyfem/elements/Thermal.py` & `pyfem-0.2.1/src/pyfem/elements/Thermal.py`

 * *Files 7% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         ntens = self.ntens
         ndi = self.ndi
         nshr = self.nshr
 
         qp_number = self.qp_number
         qp_weight_times_jacobi_dets = self.qp_weight_times_jacobi_dets
         qp_shape_values = self.iso_element_shape.qp_shape_values
-        qp_shape_gradients = self.iso_element_shape.qp_shape_gradients
+        qp_dhdxex = self.qp_dhdxes
 
         qp_state_variables = self.qp_state_variables
         qp_state_variables_new = self.qp_state_variables_new
 
         element_dof_values = self.element_dof_values
         element_ddof_values = self.element_ddof_values
 
@@ -126,19 +126,19 @@
             self.qp_temperatures = list()
             self.qp_heat_fluxes = list()
 
         for i in range(qp_number):
             if is_update_material:
                 qp_weight_times_jacobi_det = qp_weight_times_jacobi_dets[i]
                 qp_shape_value = qp_shape_values[i]
-                qp_shape_gradient = qp_shape_gradients[i]
+                qp_dhdx = qp_dhdxex[i]
                 qp_temperature = dot(qp_shape_value, element_dof_values)
                 qp_dtemperature = dot(qp_shape_value, element_ddof_values)
-                qp_temperature_gradient = dot(qp_shape_gradient, element_dof_values)
-                qp_dtemperature_gradient = dot(qp_shape_gradient, element_ddof_values)
+                qp_temperature_gradient = dot(qp_dhdx, element_dof_values)
+                qp_dtemperature_gradient = dot(qp_dhdx, element_ddof_values)
 
                 variable = {'temperature': qp_temperature,
                             'dtemperature': qp_dtemperature,
                             'temperature_gradient': qp_temperature_gradient,
                             'dtemperature_gradient': qp_dtemperature_gradient}
                 qp_ddsddt, qp_output = material_data.get_tangent(variable=variable,
                                                                  state_variable=qp_state_variables[i],
@@ -150,25 +150,24 @@
                                                                  nshr=nshr,
                                                                  timer=timer)
                 qp_heat_flux = qp_output['heat_flux']
                 self.qp_ddsddts.append(qp_ddsddt)
                 self.qp_temperatures.append(qp_temperature)
                 self.qp_heat_fluxes.append(qp_heat_flux)
             else:
-                qp_shape_gradient = qp_shape_gradients[i]
                 qp_weight_times_jacobi_det = qp_weight_times_jacobi_dets[i]
                 qp_ddsddt = self.qp_ddsddts[i]
                 qp_heat_flux = self.qp_heat_fluxes[i]
 
             if is_update_stiffness:
-                self.element_stiffness += dot(qp_shape_gradient.transpose(), dot(qp_ddsddt, qp_shape_gradient)) * \
+                self.element_stiffness += dot(qp_dhdx.transpose(), dot(qp_ddsddt, qp_dhdx)) * \
                                           qp_weight_times_jacobi_det
 
             if is_update_fint:
-                self.element_fint += dot(qp_shape_gradient.transpose(), qp_heat_flux) * qp_weight_times_jacobi_det
+                self.element_fint += dot(qp_dhdx.transpose(), qp_heat_flux) * qp_weight_times_jacobi_det
 
     def update_element_field_variables(self) -> None:
         qp_temperatures = self.qp_temperatures
         qp_heat_fluxes = self.qp_heat_fluxes
 
         average_temperatures = average(qp_temperatures, axis=0)
         average_heat_fluxes = average(qp_heat_fluxes, axis=0)
```

### Comparing `pyfem-0.2.0/src/pyfem/elements/get_element_data.py` & `pyfem-0.2.1/src/pyfem/elements/get_element_data.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/fem/Timer.py` & `pyfem-0.2.1/src/pyfem/fem/Timer.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/io/Amplitude.py` & `pyfem-0.2.1/src/pyfem/io/Amplitude.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/io/BC.py` & `pyfem-0.2.1/src/pyfem/io/BC.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/io/BaseIO.py` & `pyfem-0.2.1/src/pyfem/io/BaseIO.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/io/Dof.py` & `pyfem-0.2.1/src/pyfem/io/Dof.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/io/Material.py` & `pyfem-0.2.1/src/pyfem/io/Material.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/io/Mesh.py` & `pyfem-0.2.1/src/pyfem/io/Mesh.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/io/Module.py` & `pyfem-0.2.1/src/pyfem/io/Module.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/io/Output.py` & `pyfem-0.2.1/src/pyfem/io/Output.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/io/Parameter.py` & `pyfem-0.2.1/src/pyfem/io/Parameter.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/io/Properties.py` & `pyfem-0.2.1/src/pyfem/io/Properties.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/io/Section.py` & `pyfem-0.2.1/src/pyfem/io/Section.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/io/Solver.py` & `pyfem-0.2.1/src/pyfem/io/Solver.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/io/arguments.py` & `pyfem-0.2.1/src/pyfem/io/arguments.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/io/write_hdf5.py` & `pyfem-0.2.1/src/pyfem/io/write_hdf5.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/io/write_vtk.py` & `pyfem-0.2.1/src/pyfem/io/write_vtk.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/isoelements/IsoElementDiagram.py` & `pyfem-0.2.1/src/pyfem/isoelements/IsoElementDiagram.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/isoelements/IsoElementShape.py` & `pyfem-0.2.1/src/pyfem/isoelements/IsoElementShape.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/isoelements/derive_shape_functions.py` & `pyfem-0.2.1/src/pyfem/isoelements/derive_shape_functions.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/isoelements/get_iso_element_type.py` & `pyfem-0.2.1/src/pyfem/isoelements/get_iso_element_type.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/isoelements/shape_functions.py` & `pyfem-0.2.1/src/pyfem/isoelements/shape_functions.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/materials/BaseMaterial.py` & `pyfem-0.2.1/src/pyfem/materials/BaseMaterial.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/materials/DiffusionIsotropic.py` & `pyfem-0.2.1/src/pyfem/materials/DiffusionIsotropic.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/materials/ElasticIsotropic.py` & `pyfem-0.2.1/src/pyfem/materials/ElasticIsotropic.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/materials/MechanicalThermalExpansion.py` & `pyfem-0.2.1/src/pyfem/materials/MechanicalThermalExpansion.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/materials/PhaseFieldDamage.py` & `pyfem-0.2.1/src/pyfem/materials/PhaseFieldDamage.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/materials/PlasticCrystal.py` & `pyfem-0.2.1/src/pyfem/materials/PlasticCrystal.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/materials/PlasticCrystalGNDs.py` & `pyfem-0.2.1/src/pyfem/materials/PlasticCrystalGNDs.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/materials/PlasticKinematicHardening.py` & `pyfem-0.2.1/src/pyfem/materials/PlasticKinematicHardening.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/materials/ThermalIsotropic.py` & `pyfem-0.2.1/src/pyfem/materials/ThermalIsotropic.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/materials/UMAT.py` & `pyfem-0.2.1/src/pyfem/materials/UMAT.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/materials/ViscoElasticMaxwell.py` & `pyfem-0.2.1/src/pyfem/materials/ViscoElasticMaxwell.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/materials/crystal_slip_system.py` & `pyfem-0.2.1/src/pyfem/materials/crystal_slip_system.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/materials/get_material_data.py` & `pyfem-0.2.1/src/pyfem/materials/get_material_data.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/mesh/MeshData.py` & `pyfem-0.2.1/src/pyfem/mesh/MeshData.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/quadrature/BaseQuadrature.py` & `pyfem-0.2.1/src/pyfem/quadrature/BaseQuadrature.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/quadrature/GaussLegendreQuadrature.py` & `pyfem-0.2.1/src/pyfem/quadrature/GaussLegendreQuadrature.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/quadrature/PyramidQuadrature.py` & `pyfem-0.2.1/src/pyfem/quadrature/PyramidQuadrature.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/quadrature/TetrahedronQuadrature.py` & `pyfem-0.2.1/src/pyfem/quadrature/TetrahedronQuadrature.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/quadrature/TetrahedronQuadratureBarycentric.py` & `pyfem-0.2.1/src/pyfem/quadrature/TetrahedronQuadratureBarycentric.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/quadrature/TriangleQuadrature.py` & `pyfem-0.2.1/src/pyfem/quadrature/TriangleQuadrature.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/quadrature/TriangleQuadratureBarycentric.py` & `pyfem-0.2.1/src/pyfem/quadrature/TriangleQuadratureBarycentric.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/solvers/ArcLengthSolver.py` & `pyfem-0.2.1/src/pyfem/solvers/ArcLengthSolver.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/solvers/BaseSolver.py` & `pyfem-0.2.1/src/pyfem/solvers/BaseSolver.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/solvers/LinearSolver.py` & `pyfem-0.2.1/src/pyfem/solvers/LinearSolver.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/solvers/NonlinearSolver.py` & `pyfem-0.2.1/src/pyfem/solvers/NonlinearSolver.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,16 +61,16 @@
 
     def __init__(self, assembly: Assembly, solver: Solver) -> None:
         super().__init__()
         self.assembly = assembly
         self.solver = solver
         self.dof_solution = zeros(self.assembly.total_dof_number)
         self.PENALTY: float = 1.0e128
-        self.FORCE_TOL: float = 1.0e-6
-        self.MAX_NITER: int = 128
+        self.FORCE_TOL: float = 1.0e-3
+        self.MAX_NITER: int = 16
         self.BC_METHOD: str = '01'
 
     def run(self) -> int:
         if self.assembly.props.solver.option in [None, '', 'NR', 'NewtonRaphson']:
             return self.incremental_iterative_solve('NR')
         elif self.assembly.props.solver.option in ['IT', 'InitialTangent']:
             return self.incremental_iterative_solve('IT')
```

### Comparing `pyfem-0.2.0/src/pyfem/solvers/TimeIntegrationNonlinearSolver.py` & `pyfem-0.2.1/src/pyfem/solvers/TimeIntegrationNonlinearSolver.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/solvers/get_solver_data.py` & `pyfem-0.2.1/src/pyfem/solvers/get_solver_data.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/utils/IntKeyDict.py` & `pyfem-0.2.1/src/pyfem/utils/IntKeyDict.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/utils/colors.py` & `pyfem-0.2.1/src/pyfem/utils/colors.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/utils/logger.py` & `pyfem-0.2.1/src/pyfem/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/utils/mechanics.py` & `pyfem-0.2.1/src/pyfem/utils/mechanics.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/utils/visualization.py` & `pyfem-0.2.1/src/pyfem/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem/utils/wrappers.py` & `pyfem-0.2.1/src/pyfem/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.2.0/src/pyfem.egg-info/PKG-INFO` & `pyfem-0.2.1/src/pyfem.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfem
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python Finite Element Method
 Home-page: https://github.com/sunwhale/pyfem
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,34 +13,43 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyfem
 
 pyfem是一个完全基于python语言实现的极简有限元求解器。依赖的第三方库包括numpy、scipy和meshio等，主要用于有限元方法的学习、有限元算法验证和快速建立材料本构模型的程序原型。
 
+Github仓库：https://github.com/sunwhale/pyfem
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/ab5bca55d85d45d4aa4336ccae058316)](https://app.codacy.com/gh/sunwhale/pyfem/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 
+## Contact 联系方式
+电子邮箱 E-mail：sunjingyu@imech.ac.cn
+
+作者主页 Homepage: https://people.ucas.edu.cn/~sunjingyu
+
 ## Installation 安装
 
 支持的操作系统包括：Windows，Linux和MacOS。
 
 ### Recommend 推荐
 
 Use the package manager [pip](https://pypi.org/project/pyfem/) to install pyfem:
 
 使用pip命令安装:
 
 ```bash
-pip install pyfem
+pip install -U pyfem
 ```
 
 If you have no root access on Linux/MacOS, please try
+
+如果你在Linux/MacOS上没有root访问权限，请尝试
+
 ```bash
-python -m pip install pyfem
+python -m pip install -U pyfem
 ```
 
 Users in China can install pyfem from mirrors such as:
 
 中国用户可以使用以下镜像:
 - [Aliyun](https://developer.aliyun.com/mirror/pypi)
 - [Tsinghua](https://mirrors.tuna.tsinghua.edu.cn/help/pypi/)
@@ -56,15 +65,18 @@
 or 或者
 
 ```bash
 git clone https://github.com/sunwhale/pyfem.git
 cd pyfem
 python install.py
 ```
-采用第二种方法需要将可执行文件或批处理文件写入环境变量。
+
+Using the "From Source" approach will generate executable files or batch files, which can then have their paths added to the system environment variables.
+
+采用基于源代码的方法会生成可执行文件或批处理文件，可将其路径写入系统环境变量。
 
 ## Quickstart 快速开始
 
 ### Run in command line 在命令行运行:
 
 ```bash
 pyfem --help
@@ -75,42 +87,35 @@
 当前算例文件存储目录 examples/tutorial，该算例定义了一个二维平面应变模型，材料为塑性随动强化，载荷为y方向的循环拉伸-压缩。
 
 ```bash
 cd examples/tutorial
 pyfem -i Job-1.toml
 ```
 
-## 后处理
+## Postproc 后处理
 
 算例计算完成后将在配置文件所在目录下生成 .pvd 或 .vtu文件，可以使用开源可视化软件 [paraview](https://www.paraview.org/download/) 进行查看。
 
-## 前处理
+## Preproc 前处理
 
 本项目暂不提供前处理模块，基于 meshio 库，可以识别[gmsh](https://www.gmsh.info/)、abaqus 和 ansys等有限元软件的网格文件。
 
 ## Documents 帮助文档
-[https://pyfem-doc.readthedocs.io/](https://pyfem-doc.readthedocs.io/)
 
-## Development
+[帮助文档](https://pyfem-doc.readthedocs.io/)中给出了详细的理论公式和函数说明。
+
+
+
+## Development 开发
 
 ### ToDo list
 
-- [x] 增加Neumann边界条件，支持concentrated force，distributed和pressure定义方式
+- [ ] 增加如何建立toml算例文件的帮助文档
 - [ ] 增加hdf5计算结果输出格式
-- [ ] 完善帮助文档
-- [ ] 完善输入文件的校检
-- [x] 增加测试模块
-- [x] 增加日志模块
-- [x] 增加后台运行模式
 - [ ] 处理平面应力状态的面外应力平衡
-- [x] 增加粘弹性力学本构模型
-- [x] 增加晶体塑性力学本构模型
-- [x] 增加温度场求解单元
-- [x] 增加温度场-位移场耦合求解单元
-- [x] 增加相场-位移场耦合求解单元
 - [ ] 增加内聚区单元
 - [ ] 增加动力学求解器
 - [ ] 建立前处理界面
 
 ### Bug list
 
 - [ ] 采用abaqus网格文件时，如果存在node不属于任何element则在计算时会导致全局刚度矩阵奇异。
```

### Comparing `pyfem-0.2.0/src/pyfem.egg-info/SOURCES.txt` & `pyfem-0.2.1/src/pyfem.egg-info/SOURCES.txt`

 * *Files identical despite different names*


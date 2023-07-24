# Comparing `tmp/pyfem-0.1.2.tar.gz` & `tmp/pyfem-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfem-0.1.2.tar", last modified: Wed Jul 19 05:49:14 2023, max compression
+gzip compressed data, was "pyfem-0.1.3.tar", last modified: Mon Jul 24 07:11:46 2023, max compression
```

## Comparing `pyfem-0.1.2.tar` & `pyfem-0.1.3.tar`

### file list

```diff
@@ -1,95 +1,96 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.262223 pyfem-0.1.2/
--rw-rw-rw-   0        0        0    11525 2023-05-04 02:49:52.000000 pyfem-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     4520 2023-07-19 05:49:14.262223 pyfem-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3997 2023-07-07 05:28:59.000000 pyfem-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-19 05:49:14.262223 pyfem-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1067 2023-07-19 05:46:31.000000 pyfem-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.179223 pyfem-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.189223 pyfem-0.1.2/src/pyfem/
--rw-rw-rw-   0        0        0     1407 2023-07-13 07:39:17.000000 pyfem-0.1.2/src/pyfem/Job.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.2/src/pyfem/__init__.py
--rw-rw-rw-   0        0        0      277 2023-05-22 03:59:51.000000 pyfem-0.1.2/src/pyfem/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.199223 pyfem-0.1.2/src/pyfem/amplitude/
--rw-rw-rw-   0        0        0      988 2023-07-13 06:20:15.000000 pyfem-0.1.2/src/pyfem/amplitude/BaseAmplitude.py
--rw-rw-rw-   0        0        0     1525 2023-07-19 05:47:27.000000 pyfem-0.1.2/src/pyfem/amplitude/TabularAmplitude.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.2/src/pyfem/amplitude/__init__.py
--rw-rw-rw-   0        0        0      818 2023-06-09 03:34:39.000000 pyfem-0.1.2/src/pyfem/amplitude/get_amplitude_data.py
-drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.202223 pyfem-0.1.2/src/pyfem/assembly/
--rw-rw-rw-   0        0        0    11052 2023-07-13 09:46:40.000000 pyfem-0.1.2/src/pyfem/assembly/Assembly.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.2/src/pyfem/assembly/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.208223 pyfem-0.1.2/src/pyfem/bc/
--rw-rw-rw-   0        0        0     2168 2023-07-13 09:46:40.000000 pyfem-0.1.2/src/pyfem/bc/BaseBC.py
--rw-rw-rw-   0        0        0     2200 2023-07-13 09:46:40.000000 pyfem-0.1.2/src/pyfem/bc/DirichletBC.py
--rw-rw-rw-   0        0        0     2648 2023-07-13 09:46:40.000000 pyfem-0.1.2/src/pyfem/bc/NeumannBCConcentrated.py
--rw-rw-rw-   0        0        0     8922 2023-07-14 04:08:19.000000 pyfem-0.1.2/src/pyfem/bc/NeumannBCDistributed.py
--rw-rw-rw-   0        0        0     9036 2023-07-13 09:46:40.000000 pyfem-0.1.2/src/pyfem/bc/NeumannBCPressure.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.2/src/pyfem/bc/__init__.py
--rw-rw-rw-   0        0        0     1484 2023-07-13 09:46:40.000000 pyfem-0.1.2/src/pyfem/bc/get_bc_data.py
-drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.220223 pyfem-0.1.2/src/pyfem/elements/
--rw-rw-rw-   0        0        0    14002 2023-07-16 23:42:08.000000 pyfem-0.1.2/src/pyfem/elements/BaseElement.py
--rw-rw-rw-   0        0        0     2311 2023-07-16 23:42:08.000000 pyfem-0.1.2/src/pyfem/elements/IsoElementDiagram.py
--rw-rw-rw-   0        0        0    40943 2023-07-19 05:47:27.000000 pyfem-0.1.2/src/pyfem/elements/IsoElementShape.py
--rw-rw-rw-   0        0        0    10577 2023-07-19 03:59:10.000000 pyfem-0.1.2/src/pyfem/elements/SolidPhaseFieldDamagePlaneSmallStrain.py
--rw-rw-rw-   0        0        0     9927 2023-07-16 23:42:08.000000 pyfem-0.1.2/src/pyfem/elements/SolidPlaneSmallStrain.py
--rw-rw-rw-   0        0        0    12780 2023-07-16 23:42:08.000000 pyfem-0.1.2/src/pyfem/elements/SolidThermalPlaneSmallStrain.py
--rw-rw-rw-   0        0        0    10689 2023-07-16 23:42:08.000000 pyfem-0.1.2/src/pyfem/elements/SolidVolumeSmallStrain.py
--rw-rw-rw-   0        0        0     7570 2023-07-16 23:42:08.000000 pyfem-0.1.2/src/pyfem/elements/Thermal.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.2/src/pyfem/elements/__init__.py
--rw-rw-rw-   0        0        0      939 2023-07-19 05:47:27.000000 pyfem-0.1.2/src/pyfem/elements/derive.py
--rw-rw-rw-   0        0        0     2829 2023-07-16 23:42:08.000000 pyfem-0.1.2/src/pyfem/elements/get_element_data.py
--rw-rw-rw-   0        0        0     1842 2023-06-08 06:40:10.000000 pyfem-0.1.2/src/pyfem/elements/get_iso_element_type.py
-drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.223223 pyfem-0.1.2/src/pyfem/fem/
--rw-rw-rw-   0        0        0     1148 2023-07-13 07:26:47.000000 pyfem-0.1.2/src/pyfem/fem/Timer.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.2/src/pyfem/fem/__init__.py
--rw-rw-rw-   0        0        0       68 2023-06-08 03:23:23.000000 pyfem-0.1.2/src/pyfem/fem/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.236225 pyfem-0.1.2/src/pyfem/io/
--rw-rw-rw-   0        0        0      596 2023-07-13 09:14:21.000000 pyfem-0.1.2/src/pyfem/io/Amplitude.py
--rw-rw-rw-   0        0        0     1077 2023-07-13 09:46:40.000000 pyfem-0.1.2/src/pyfem/io/BC.py
--rw-rw-rw-   0        0        0     1584 2023-07-13 09:07:55.000000 pyfem-0.1.2/src/pyfem/io/BaseIO.py
--rw-rw-rw-   0        0        0      511 2023-07-13 08:44:15.000000 pyfem-0.1.2/src/pyfem/io/Dof.py
--rw-rw-rw-   0        0        0     2586 2023-07-19 05:47:27.000000 pyfem-0.1.2/src/pyfem/io/Material.py
--rw-rw-rw-   0        0        0      417 2023-07-13 08:45:45.000000 pyfem-0.1.2/src/pyfem/io/Mesh.py
--rw-rw-rw-   0        0        0      534 2023-07-13 08:46:22.000000 pyfem-0.1.2/src/pyfem/io/Output.py
--rw-rw-rw-   0        0        0     7966 2023-07-19 05:47:27.000000 pyfem-0.1.2/src/pyfem/io/Properties.py
--rw-rw-rw-   0        0        0      900 2023-07-13 08:42:59.000000 pyfem-0.1.2/src/pyfem/io/Section.py
--rw-rw-rw-   0        0        0      999 2023-07-14 02:39:28.000000 pyfem-0.1.2/src/pyfem/io/Solver.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.2/src/pyfem/io/__init__.py
--rw-rw-rw-   0        0        0     1741 2023-07-19 05:46:59.000000 pyfem-0.1.2/src/pyfem/io/arguments.py
--rw-rw-rw-   0        0        0     5160 2023-07-19 03:59:10.000000 pyfem-0.1.2/src/pyfem/io/write_vtk.py
-drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.246223 pyfem-0.1.2/src/pyfem/materials/
--rw-rw-rw-   0        0        0     2290 2023-07-13 06:56:12.000000 pyfem-0.1.2/src/pyfem/materials/BaseMaterial.py
--rw-rw-rw-   0        0        0     7243 2023-07-14 03:34:03.000000 pyfem-0.1.2/src/pyfem/materials/ElasticIsotropic.py
--rw-rw-rw-   0        0        0     2699 2023-07-13 05:52:00.000000 pyfem-0.1.2/src/pyfem/materials/MechanicalThermalExpansion.py
--rw-rw-rw-   0        0        0     1509 2023-07-13 05:49:56.000000 pyfem-0.1.2/src/pyfem/materials/PhaseFieldDamage.py
--rw-rw-rw-   0        0        0     7668 2023-07-13 05:54:25.000000 pyfem-0.1.2/src/pyfem/materials/PlasticKinematicHardening.py
--rw-rw-rw-   0        0        0     2297 2023-07-13 05:55:59.000000 pyfem-0.1.2/src/pyfem/materials/ThermalIsotropic.py
--rw-rw-rw-   0        0        0     6221 2023-07-19 05:47:27.000000 pyfem-0.1.2/src/pyfem/materials/ViscoElasticMaxwell.py
--rw-rw-rw-   0        0        0     6248 2023-07-13 05:58:59.000000 pyfem-0.1.2/src/pyfem/materials/ViscoElasticMaxwellUMAT.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.2/src/pyfem/materials/__init__.py
--rw-rw-rw-   0        0        0     1801 2023-07-06 05:22:46.000000 pyfem-0.1.2/src/pyfem/materials/get_material_data.py
-drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.248223 pyfem-0.1.2/src/pyfem/mesh/
--rw-rw-rw-   0        0        0     6852 2023-07-19 05:47:27.000000 pyfem-0.1.2/src/pyfem/mesh/MeshData.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.2/src/pyfem/mesh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.252223 pyfem-0.1.2/src/pyfem/solvers/
--rw-rw-rw-   0        0        0      930 2023-07-13 06:55:29.000000 pyfem-0.1.2/src/pyfem/solvers/BaseSolver.py
--rw-rw-rw-   0        0        0     1838 2023-07-13 06:57:34.000000 pyfem-0.1.2/src/pyfem/solvers/LinearSolver.py
--rw-rw-rw-   0        0        0     9277 2023-07-13 06:58:09.000000 pyfem-0.1.2/src/pyfem/solvers/NonlinearSolver.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.2/src/pyfem/solvers/__init__.py
--rw-rw-rw-   0        0        0      991 2023-06-09 03:34:39.000000 pyfem-0.1.2/src/pyfem/solvers/get_solver_data.py
-drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.261223 pyfem-0.1.2/src/pyfem/utils/
--rw-rw-rw-   0        0        0     2443 2023-07-14 02:39:28.000000 pyfem-0.1.2/src/pyfem/utils/IntKeyDict.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.2/src/pyfem/utils/__init__.py
--rw-rw-rw-   0        0        0      795 2023-05-30 02:50:20.000000 pyfem-0.1.2/src/pyfem/utils/colors.py
--rw-rw-rw-   0        0        0      769 2023-07-19 05:47:27.000000 pyfem-0.1.2/src/pyfem/utils/data_types.py
--rw-rw-rw-   0        0        0     1814 2023-07-19 05:47:27.000000 pyfem-0.1.2/src/pyfem/utils/derive.py
--rw-rw-rw-   0        0        0     1518 2023-05-30 02:23:43.000000 pyfem-0.1.2/src/pyfem/utils/logger.py
--rw-rw-rw-   0        0        0     5032 2023-07-14 05:55:14.000000 pyfem-0.1.2/src/pyfem/utils/mechanics.py
--rw-rw-rw-   0        0        0     3722 2023-07-13 07:29:45.000000 pyfem-0.1.2/src/pyfem/utils/visualization.py
--rw-rw-rw-   0        0        0     1046 2023-05-30 02:47:20.000000 pyfem-0.1.2/src/pyfem/utils/wrappers.py
-drwxrwxrwx   0        0        0        0 2023-07-19 05:49:14.195222 pyfem-0.1.2/src/pyfem.egg-info/
--rw-rw-rw-   0        0        0     4520 2023-07-19 05:49:14.000000 pyfem-0.1.2/src/pyfem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2479 2023-07-19 05:49:14.000000 pyfem-0.1.2/src/pyfem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 05:49:14.000000 pyfem-0.1.2/src/pyfem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-19 05:49:14.000000 pyfem-0.1.2/src/pyfem.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2023-07-19 05:49:14.000000 pyfem-0.1.2/src/pyfem.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-19 05:49:14.000000 pyfem-0.1.2/src/pyfem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.650114 pyfem-0.1.3/
+-rw-rw-rw-   0        0        0    11525 2023-05-04 02:49:52.000000 pyfem-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     5000 2023-07-24 07:11:46.649121 pyfem-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4477 2023-07-21 05:51:34.000000 pyfem-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 07:11:46.650114 pyfem-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1106 2023-07-24 07:11:34.000000 pyfem-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.565120 pyfem-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.577113 pyfem-0.1.3/src/pyfem/
+-rw-rw-rw-   0        0        0     2370 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/Job.py
+-rw-rw-rw-   0        0        0       23 2023-07-24 07:09:24.000000 pyfem-0.1.3/src/pyfem/__init__.py
+-rw-rw-rw-   0        0        0      277 2023-05-22 03:59:51.000000 pyfem-0.1.3/src/pyfem/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.587120 pyfem-0.1.3/src/pyfem/amplitude/
+-rw-rw-rw-   0        0        0     1403 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/amplitude/BaseAmplitude.py
+-rw-rw-rw-   0        0        0     1892 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/amplitude/TabularAmplitude.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.3/src/pyfem/amplitude/__init__.py
+-rw-rw-rw-   0        0        0     1112 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/amplitude/get_amplitude_data.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.589113 pyfem-0.1.3/src/pyfem/assembly/
+-rw-rw-rw-   0        0        0    13349 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/assembly/Assembly.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.3/src/pyfem/assembly/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.597120 pyfem-0.1.3/src/pyfem/bc/
+-rw-rw-rw-   0        0        0     3725 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/bc/BaseBC.py
+-rw-rw-rw-   0        0        0     2250 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/bc/DirichletBC.py
+-rw-rw-rw-   0        0        0     2222 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/bc/NeumannBCConcentrated.py
+-rw-rw-rw-   0        0        0     8556 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/bc/NeumannBCDistributed.py
+-rw-rw-rw-   0        0        0     8667 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/bc/NeumannBCPressure.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.3/src/pyfem/bc/__init__.py
+-rw-rw-rw-   0        0        0     1965 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/bc/get_bc_data.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.604120 pyfem-0.1.3/src/pyfem/elements/
+-rw-rw-rw-   0        0        0    15918 2023-07-24 05:03:33.000000 pyfem-0.1.3/src/pyfem/elements/BaseElement.py
+-rw-rw-rw-   0        0        0    15924 2023-07-24 06:41:10.000000 pyfem-0.1.3/src/pyfem/elements/SolidPhaseDamageSmallStrain.py
+-rw-rw-rw-   0        0        0    11522 2023-07-24 06:42:53.000000 pyfem-0.1.3/src/pyfem/elements/SolidSmallStrain.py
+-rw-rw-rw-   0        0        0    16417 2023-07-24 06:30:08.000000 pyfem-0.1.3/src/pyfem/elements/SolidThermalSmallStrain.py
+-rw-rw-rw-   0        0        0     8363 2023-07-24 06:42:11.000000 pyfem-0.1.3/src/pyfem/elements/Thermal.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.3/src/pyfem/elements/__init__.py
+-rw-rw-rw-   0        0        0     3127 2023-07-24 06:54:28.000000 pyfem-0.1.3/src/pyfem/elements/get_element_data.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.606122 pyfem-0.1.3/src/pyfem/fem/
+-rw-rw-rw-   0        0        0     1866 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/fem/Timer.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.3/src/pyfem/fem/__init__.py
+-rw-rw-rw-   0        0        0       68 2023-06-08 03:23:23.000000 pyfem-0.1.3/src/pyfem/fem/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.619113 pyfem-0.1.3/src/pyfem/io/
+-rw-rw-rw-   0        0        0     1124 2023-07-21 09:01:29.000000 pyfem-0.1.3/src/pyfem/io/Amplitude.py
+-rw-rw-rw-   0        0        0     2136 2023-07-21 02:42:25.000000 pyfem-0.1.3/src/pyfem/io/BC.py
+-rw-rw-rw-   0        0        0     1781 2023-07-24 05:11:05.000000 pyfem-0.1.3/src/pyfem/io/BaseIO.py
+-rw-rw-rw-   0        0        0      994 2023-07-21 02:42:25.000000 pyfem-0.1.3/src/pyfem/io/Dof.py
+-rw-rw-rw-   0        0        0     2795 2023-07-21 04:25:39.000000 pyfem-0.1.3/src/pyfem/io/Material.py
+-rw-rw-rw-   0        0        0      802 2023-07-21 04:30:08.000000 pyfem-0.1.3/src/pyfem/io/Mesh.py
+-rw-rw-rw-   0        0        0     1073 2023-07-21 07:53:54.000000 pyfem-0.1.3/src/pyfem/io/Output.py
+-rw-rw-rw-   0        0        0     9316 2023-07-24 05:11:05.000000 pyfem-0.1.3/src/pyfem/io/Properties.py
+-rw-rw-rw-   0        0        0     1939 2023-07-21 05:12:54.000000 pyfem-0.1.3/src/pyfem/io/Section.py
+-rw-rw-rw-   0        0        0     1952 2023-07-21 05:18:19.000000 pyfem-0.1.3/src/pyfem/io/Solver.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.3/src/pyfem/io/__init__.py
+-rw-rw-rw-   0        0        0     1783 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/io/arguments.py
+-rw-rw-rw-   0        0        0     5230 2023-07-21 05:45:16.000000 pyfem-0.1.3/src/pyfem/io/write_vtk.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.625120 pyfem-0.1.3/src/pyfem/isoelements/
+-rw-rw-rw-   0        0        0     2320 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/isoelements/IsoElementDiagram.py
+-rw-rw-rw-   0        0        0    19943 2023-07-24 06:39:32.000000 pyfem-0.1.3/src/pyfem/isoelements/IsoElementShape.py
+-rw-rw-rw-   0        0        0        0 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/isoelements/__init__.py
+-rw-rw-rw-   0        0        0     1297 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/isoelements/derive_shape_functions.py
+-rw-rw-rw-   0        0        0     2153 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/isoelements/get_iso_element_type.py
+-rw-rw-rw-   0        0        0    23677 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/isoelements/shape_functions.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.634113 pyfem-0.1.3/src/pyfem/materials/
+-rw-rw-rw-   0        0        0     3385 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/materials/BaseMaterial.py
+-rw-rw-rw-   0        0        0     7734 2023-07-24 06:56:36.000000 pyfem-0.1.3/src/pyfem/materials/ElasticIsotropic.py
+-rw-rw-rw-   0        0        0     3135 2023-07-24 06:57:15.000000 pyfem-0.1.3/src/pyfem/materials/MechanicalThermalExpansion.py
+-rw-rw-rw-   0        0        0     2174 2023-07-24 06:57:15.000000 pyfem-0.1.3/src/pyfem/materials/PhaseFieldDamage.py
+-rw-rw-rw-   0        0        0     8629 2023-07-24 06:57:15.000000 pyfem-0.1.3/src/pyfem/materials/PlasticKinematicHardening.py
+-rw-rw-rw-   0        0        0     2773 2023-07-24 06:57:15.000000 pyfem-0.1.3/src/pyfem/materials/ThermalIsotropic.py
+-rw-rw-rw-   0        0        0     7283 2023-07-24 06:57:39.000000 pyfem-0.1.3/src/pyfem/materials/ViscoElasticMaxwell.py
+-rw-rw-rw-   0        0        0     7188 2023-07-24 06:57:39.000000 pyfem-0.1.3/src/pyfem/materials/ViscoElasticMaxwellUMAT.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.3/src/pyfem/materials/__init__.py
+-rw-rw-rw-   0        0        0     2266 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/materials/get_material_data.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.636124 pyfem-0.1.3/src/pyfem/mesh/
+-rw-rw-rw-   0        0        0     7874 2023-07-24 03:15:19.000000 pyfem-0.1.3/src/pyfem/mesh/MeshData.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.3/src/pyfem/mesh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.641120 pyfem-0.1.3/src/pyfem/solvers/
+-rw-rw-rw-   0        0        0     1450 2023-07-21 08:11:51.000000 pyfem-0.1.3/src/pyfem/solvers/BaseSolver.py
+-rw-rw-rw-   0        0        0     2168 2023-07-21 08:28:00.000000 pyfem-0.1.3/src/pyfem/solvers/LinearSolver.py
+-rw-rw-rw-   0        0        0     9830 2023-07-21 08:32:14.000000 pyfem-0.1.3/src/pyfem/solvers/NonlinearSolver.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.3/src/pyfem/solvers/__init__.py
+-rw-rw-rw-   0        0        0     1340 2023-07-21 08:57:15.000000 pyfem-0.1.3/src/pyfem/solvers/get_solver_data.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.648112 pyfem-0.1.3/src/pyfem/utils/
+-rw-rw-rw-   0        0        0     2443 2023-07-24 05:11:05.000000 pyfem-0.1.3/src/pyfem/utils/IntKeyDict.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.1.3/src/pyfem/utils/__init__.py
+-rw-rw-rw-   0        0        0      795 2023-05-30 02:50:20.000000 pyfem-0.1.3/src/pyfem/utils/colors.py
+-rw-rw-rw-   0        0        0     2672 2023-07-21 08:55:34.000000 pyfem-0.1.3/src/pyfem/utils/derive.py
+-rw-rw-rw-   0        0        0     1518 2023-05-30 02:23:43.000000 pyfem-0.1.3/src/pyfem/utils/logger.py
+-rw-rw-rw-   0        0        0     5032 2023-07-14 05:55:14.000000 pyfem-0.1.3/src/pyfem/utils/mechanics.py
+-rw-rw-rw-   0        0        0     3941 2023-07-20 05:58:39.000000 pyfem-0.1.3/src/pyfem/utils/visualization.py
+-rw-rw-rw-   0        0        0     1046 2023-05-30 02:47:20.000000 pyfem-0.1.3/src/pyfem/utils/wrappers.py
+drwxrwxrwx   0        0        0        0 2023-07-24 07:11:46.583125 pyfem-0.1.3/src/pyfem.egg-info/
+-rw-rw-rw-   0        0        0     5000 2023-07-24 07:11:46.000000 pyfem-0.1.3/src/pyfem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2487 2023-07-24 07:11:46.000000 pyfem-0.1.3/src/pyfem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 07:11:46.000000 pyfem-0.1.3/src/pyfem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-24 07:11:46.000000 pyfem-0.1.3/src/pyfem.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-07-24 07:11:46.000000 pyfem-0.1.3/src/pyfem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-24 07:11:46.000000 pyfem-0.1.3/src/pyfem.egg-info/top_level.txt
```

### Comparing `pyfem-0.1.2/LICENSE` & `pyfem-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.2/PKG-INFO` & `pyfem-0.1.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,66 +1,37 @@
-Metadata-Version: 2.1
-Name: pyfem
-Version: 0.1.2
-Summary: A finite element package for learning
-Home-page: https://github.com/sunwhale/pyfem
-Author: Jingyu Sun
-Author-email: sun.jingyu@outlook.com
-Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pyfem
 
-A finite element package in python.
+pyfem是一个完全基于python语言实现的极简有限元求解器。基于numpy、scipy和meshio等第三方库，主要用于有限元方法的学习、有限元算法验证和快速建立材料本构模型的程序原型。
+
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/ab5bca55d85d45d4aa4336ccae058316)](https://app.codacy.com/gh/sunwhale/pyfem/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 
-## Installation
+## Installation 安装
 
-Use the package manager [pip](https://pypi.org/project/pyfem/) to install pyfem.
+Use the package manager [pip](https://pypi.org/project/pyfem/) to install pyfem. 使用pip命令安装。
 
 ```bash
 pip install pyfem
 ```
 
-## Development
+## Tutorial 指南
 
-### ToDo list
+### Run in command line 在命令行运行:
 
-- [x] 增加Neumann边界条件，支持concentrated force，distributed和pressure定义方式
-- [ ] 增加hdf5计算结果输出格式
-- [ ] 完善帮助文档
-- [ ] 完善输入文件的校检
-- [x] 增加测试模块
-- [ ] 增加日志模块
-- [ ] 增加后台运行模式
-- [ ] 处理平面应力状态的面外应力平衡
-- [x] 增加粘弹性力学本构模型
-- [ ] 增加晶体塑性力学本构模型
-- [x] 增加温度场求解单元
-- [x] 增加温度场-位移场耦合求解单元
-- [x] 增加相场-位移场耦合求解单元
-- [ ] 增加内聚区单元
-- [ ] 增加动力学求解器
-- [ ] 建立前处理界面
-
-## Tutorial
+```bash
+pyfem --help
+```
 
-#### Run in command line:
+### Run the first example 执行第一个算例:
 
 ```bash
 pyfem -i Job-1.toml
 ```
 
-#### Job file Job-1.toml:
+#### 算例配置文件 Job-1.toml:
 
 ```toml
 title = "Job-1"
 
 [mesh]
 type = "abaqus"
 file = "hex8.inp"
@@ -106,14 +77,15 @@
 element_sets = ['Set-X1']
 value = 1.0
 
 [solver]
 type = "NonlinearSolver"
 option = "NewtonRaphson"
 total_time = 1.0
+start_time = 0.0
 max_increment = 1000000
 initial_dtime = 0.1
 max_dtime = 1.0
 min_dtime = 0.001
 
 [[materials]]
 name = "Material-1"
@@ -140,15 +112,15 @@
 
 [[outputs]]
 type = "vtk"
 field_outputs = ['S11', 'S22', 'S33', 'S12', 'S13', 'S23', 'E11', 'E22', 'E33', 'E12', 'E13', 'E23']
 on_screen = false
 ```
 
-#### abaqus geometry file hex8.inp:
+#### 采用abaqus格式的网格文件 hex8.inp:
 
 ```abaqus
 *Heading
 *Preprint, echo=NO, model=NO, history=NO, contact=NO
 **
 ** PARTS
 **
@@ -201,10 +173,34 @@
 **  
 *Instance, name=Part-1-1, part=Part-1
 *End Instance
 **  
 *End Assembly
 ```
 
+### Documents 帮助文档
+[https://pyfem-doc.readthedocs.io/](https://pyfem-doc.readthedocs.io/)
+
+## Development
+
+### ToDo list
+
+- [x] 增加Neumann边界条件，支持concentrated force，distributed和pressure定义方式
+- [ ] 增加hdf5计算结果输出格式
+- [ ] 完善帮助文档
+- [ ] 完善输入文件的校检
+- [x] 增加测试模块
+- [ ] 增加日志模块
+- [ ] 增加后台运行模式
+- [ ] 处理平面应力状态的面外应力平衡
+- [x] 增加粘弹性力学本构模型
+- [ ] 增加晶体塑性力学本构模型
+- [x] 增加温度场求解单元
+- [x] 增加温度场-位移场耦合求解单元
+- [x] 增加相场-位移场耦合求解单元
+- [ ] 增加内聚区单元
+- [ ] 增加动力学求解器
+- [ ] 建立前处理界面
+
 ### Bug list
 
 - [ ] 采用abaqus网格文件时，如果存在node不属于任何element则在计算时会导致全局刚度矩阵奇异。
```

### Comparing `pyfem-0.1.2/setup.py` & `pyfem-0.1.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import setuptools
+from src.pyfem import __version__
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyfem",
-    version="0.1.2",
+    version=__version__,
     author="Jingyu Sun",
     author_email="sun.jingyu@outlook.com",
     description="A finite element package for learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sunwhale/pyfem",
     project_urls={
```

### Comparing `pyfem-0.1.2/src/pyfem/amplitude/BaseAmplitude.py` & `pyfem-0.1.3/src/pyfem/amplitude/BaseAmplitude.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,53 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import List, Callable
+from typing import Callable
 
 from scipy.interpolate import interp1d  # type: ignore
 
 from pyfem.utils.visualization import object_slots_to_string_ndarray
 
 
 class BaseAmplitude:
-    __slots__ = ('start',
-                 'f_amplitude')
+    """
+    幅值基类。
+
+    :ivar start: 初值
+    :vartype start: float
+
+    :ivar f_amplitude: 幅值函数
+    :vartype f_amplitude: Callable
+    """
+
+    __slots_dict__: dict = {
+        'start': ('float', '初值'),
+        'f_amplitude': ('Callable', '幅值函数')
+    }
+
+    __slots__: list = [slot for slot in __slots_dict__.keys()]
 
     def __init__(self) -> None:
         self.start: float = 0.0
         self.f_amplitude: Callable = interp1d([0, 1], [0, 1], kind='linear', fill_value='extrapolate')
 
     def to_string(self, level: int = 1) -> str:
         return object_slots_to_string_ndarray(self, level)
 
     def show(self) -> None:
         print(self.to_string())
 
     def get_amplitude(self, time: float) -> float:
         return self.f_amplitude(time) + self.start
 
-    def set_f_amplitude(self, time: List[float], value: List[float]) -> None:
+    def set_f_amplitude(self, time: list[float], value: list[float]) -> None:
         self.f_amplitude = interp1d(time, value, kind='linear', fill_value='extrapolate')
 
 
 if __name__ == "__main__":
+    from pyfem.utils.visualization import print_slots_dict
+
+    print_slots_dict(BaseAmplitude.__slots_dict__)
+
     amp = BaseAmplitude()
     amp.show()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfem-0.1.2/src/pyfem/amplitude/TabularAmplitude.py` & `pyfem-0.1.3/src/pyfem/amplitude/TabularAmplitude.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,15 +9,26 @@
 
 from pyfem.amplitude.BaseAmplitude import BaseAmplitude
 from pyfem.io.Amplitude import Amplitude
 from pyfem.utils.colors import error_style
 
 
 class TabularAmplitude(BaseAmplitude):
-    __slots__ = BaseAmplitude.__slots__ + ('table',)
+    """
+    通过x-y数据表格定义的幅值。
+
+    :ivar table: x-y数据表格
+    :vartype table: ndarray
+    """
+
+    __slots_dict__: dict = {
+        'table': ('ndarray', 'x-y数据表格')
+    }
+
+    __slots__ = BaseAmplitude.__slots__ + [slot for slot in __slots_dict__.keys()]
 
     def __init__(self, amplitude: Amplitude) -> None:
         super().__init__()
         self.start = amplitude.start
         self.table: ndarray = array(amplitude.data)
         if self.table.ndim != 2:
             raise NotImplementedError(error_style('dimension of amplitude table must be 2'))
@@ -29,13 +40,17 @@
                                               fill_value='extrapolate')
 
     def get_amplitude(self, time: float) -> float:
         return self.f_amplitude(time) + self.start
 
 
 if __name__ == "__main__":
+    from pyfem.utils.visualization import print_slots_dict
+
+    print_slots_dict(TabularAmplitude.__slots_dict__)
+
     from pyfem.io.Properties import Properties
 
     props = Properties()
     props.read_file(r'..\..\..\examples\mechanical\plane\Job-1.toml')
     amp = TabularAmplitude(props.amplitudes[0])
     amp.show()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfem-0.1.2/src/pyfem/bc/DirichletBC.py` & `pyfem-0.1.3/src/pyfem/bc/DirichletBC.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,19 @@
 from pyfem.io.Dof import Dof
 from pyfem.io.Solver import Solver
 from pyfem.mesh.MeshData import MeshData
 from pyfem.utils.colors import error_style
 
 
 class DirichletBC(BaseBC):
-    __slots__ = BaseBC.__slots__ + ()
+    """
+    Dirichlet边界条件。
+    """
+
+    __slots__ = BaseBC.__slots__ + []
 
     def __init__(self, bc: BC, dof: Dof, mesh_data: MeshData, solver: Solver, amplitude: Optional[Amplitude]) -> None:
         super().__init__(bc, dof, mesh_data, solver, amplitude)
         self.create_dof_values()
 
     def create_dof_values(self) -> None:
         bc_node_sets = self.bc.node_sets
```

### Comparing `pyfem-0.1.2/src/pyfem/bc/NeumannBCConcentrated.py` & `pyfem-0.1.3/src/pyfem/bc/NeumannBCConcentrated.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,30 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import Dict, Optional
+from typing import Optional
 
 from numpy import array
 
 from pyfem.bc.BaseBC import BaseBC
-from pyfem.elements.IsoElementShape import IsoElementShape
 from pyfem.io.Amplitude import Amplitude
 from pyfem.io.BC import BC
 from pyfem.io.Dof import Dof
 from pyfem.io.Solver import Solver
 from pyfem.mesh.MeshData import MeshData
 from pyfem.utils.colors import error_style
 
-iso_element_shape_dict: Dict[str, IsoElementShape] = {
-    'line2': IsoElementShape('line2'),
-    'line3': IsoElementShape('line3'),
-    'tria3': IsoElementShape('tria3'),
-    'tria6': IsoElementShape('tria6'),
-    'quad4': IsoElementShape('quad4'),
-    'quad8': IsoElementShape('quad8'),
-    'tetra4': IsoElementShape('tetra4'),
-    'hex8': IsoElementShape('hex8'),
-    'hex20': IsoElementShape('hex20')
-}
-
 
 class NeumannBCConcentrated(BaseBC):
-    __slots__ = BaseBC.__slots__ + ()
+    """
+    Neumann边界条件：集中力。
+    """
+
+    __slots__ = BaseBC.__slots__ + []
 
     def __init__(self, bc: BC, dof: Dof, mesh_data: MeshData, solver: Solver, amplitude: Optional[Amplitude]) -> None:
         super().__init__(bc, dof, mesh_data, solver, amplitude)
         self.create_dof_values()
 
     def create_dof_values(self) -> None:
         bc_node_sets = self.bc.node_sets
```

### Comparing `pyfem-0.1.2/src/pyfem/bc/NeumannBCDistributed.py` & `pyfem-0.1.3/src/pyfem/bc/NeumannBCDistributed.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,84 +1,76 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import Dict, List, Optional, Tuple
+from typing import Optional
 
 from numpy import array, delete, dot, logical_and, ndarray, in1d, all, sqrt, zeros
 from numpy.linalg import det
 
 from pyfem.bc.BaseBC import BaseBC
-from pyfem.elements.IsoElementShape import IsoElementShape
-from pyfem.elements.get_iso_element_type import get_iso_element_type
 from pyfem.io.Amplitude import Amplitude
 from pyfem.io.BC import BC
 from pyfem.io.Dof import Dof
 from pyfem.io.Solver import Solver
+from pyfem.isoelements.IsoElementShape import iso_element_shape_dict
+from pyfem.isoelements.get_iso_element_type import get_iso_element_type
 from pyfem.mesh.MeshData import MeshData
 from pyfem.utils.colors import error_style
 from pyfem.utils.wrappers import show_running_time
 
-iso_element_shape_dict: Dict[str, IsoElementShape] = {
-    'line2': IsoElementShape('line2'),
-    'line3': IsoElementShape('line3'),
-    'tria3': IsoElementShape('tria3'),
-    'tria6': IsoElementShape('tria6'),
-    'quad4': IsoElementShape('quad4'),
-    'quad8': IsoElementShape('quad8'),
-    'tetra4': IsoElementShape('tetra4'),
-    'hex8': IsoElementShape('hex8'),
-    'hex20': IsoElementShape('hex20')
-}
-
 
 class NeumannBCDistributed(BaseBC):
-    __slots__ = BaseBC.__slots__ + ()
+    """
+    Neumann边界条件：分布力。
+    """
+
+    __slots__ = BaseBC.__slots__ + []
 
     def __init__(self, bc: BC, dof: Dof, mesh_data: MeshData, solver: Solver, amplitude: Optional[Amplitude]) -> None:
         super().__init__(bc, dof, mesh_data, solver, amplitude)
         self.create_dof_values()
 
     @show_running_time
-    def get_surface_from_bc_element(self, bc_element_id: int, bc_element: ndarray) -> List[Tuple[int, str]]:
+    def get_surface_from_bc_element(self, bc_element_id: int, bc_element: ndarray) -> list[tuple[int, str]]:
         nodes = self.mesh_data.nodes
         elements = self.mesh_data.elements
         element_surface = []
         for element_id, element in enumerate(elements):
             is_element_surface = all(in1d(bc_element, element))
             if is_element_surface:
                 nodes_in_element = in1d(element, bc_element)
                 connectivity = elements[element_id]
                 node_coords = nodes[connectivity]
                 iso_element_type = get_iso_element_type(node_coords)
                 iso_element_shape = iso_element_shape_dict[iso_element_type]
                 surface_names = [surface_name for surface_name, nodes_on_surface in
-                                 iso_element_shape.nodes_to_surface_dict.items() if
+                                 iso_element_shape.nodes_on_surface_dict.items() if
                                  all(nodes_on_surface == nodes_in_element)]
                 if len(surface_names) == 1:
                     element_surface.append((element_id, surface_names[0]))
                 else:
                     raise NotImplementedError(error_style(f'the surface of element {element_id} is wrong'))
 
         if len(element_surface) == 1:
             return element_surface
         else:
             raise NotImplementedError(error_style(f'the surface of bc_element {bc_element_id} is wrong'))
 
-    def get_surface_from_elements_nodes(self, element_id: int, node_ids: List[int]) -> List[Tuple[int, str]]:
+    def get_surface_from_elements_nodes(self, element_id: int, node_ids: list[int]) -> list[tuple[int, str]]:
         nodes = self.mesh_data.nodes
         elements = self.mesh_data.elements
         element_surface = []
         nodes_in_element = in1d(elements[element_id], node_ids)
         connectivity = elements[element_id]
         node_coords = nodes[connectivity]
         iso_element_type = get_iso_element_type(node_coords)
         iso_element_shape = iso_element_shape_dict[iso_element_type]
         surface_names = [surface_name for surface_name, nodes_on_surface in
-                         iso_element_shape.nodes_to_surface_dict.items() if
+                         iso_element_shape.nodes_on_surface_dict.items() if
                          sum(logical_and(nodes_in_element, nodes_on_surface)) == len(
                              iso_element_shape.bc_surface_nodes_dict[surface_name])]
 
         for surface_name in surface_names:
             element_surface.append((element_id, surface_name))
 
         if 1 <= len(element_surface) <= iso_element_shape.bc_surface_number:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfem-0.1.2/src/pyfem/bc/NeumannBCPressure.py` & `pyfem-0.1.3/src/pyfem/bc/NeumannBCPressure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,82 +1,74 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import Dict, List, Optional, Tuple
+from typing import Optional
 
 from numpy import array, delete, dot, logical_and, ndarray, in1d, all, sqrt, zeros
 from numpy.linalg import det
 
 from pyfem.bc.BaseBC import BaseBC
-from pyfem.elements.IsoElementShape import IsoElementShape
-from pyfem.elements.get_iso_element_type import get_iso_element_type
 from pyfem.io.Amplitude import Amplitude
 from pyfem.io.BC import BC
 from pyfem.io.Dof import Dof
 from pyfem.io.Solver import Solver
+from pyfem.isoelements.IsoElementShape import iso_element_shape_dict
+from pyfem.isoelements.get_iso_element_type import get_iso_element_type
 from pyfem.mesh.MeshData import MeshData
 from pyfem.utils.colors import error_style
 
-iso_element_shape_dict: Dict[str, IsoElementShape] = {
-    'line2': IsoElementShape('line2'),
-    'line3': IsoElementShape('line3'),
-    'tria3': IsoElementShape('tria3'),
-    'tria6': IsoElementShape('tria6'),
-    'quad4': IsoElementShape('quad4'),
-    'quad8': IsoElementShape('quad8'),
-    'tetra4': IsoElementShape('tetra4'),
-    'hex8': IsoElementShape('hex8'),
-    'hex20': IsoElementShape('hex20')
-}
-
 
 class NeumannBCPressure(BaseBC):
-    __slots__ = BaseBC.__slots__ + ()
+    """
+    Neumann边界条件：压力。
+    """
+
+    __slots__ = BaseBC.__slots__ + []
 
     def __init__(self, bc: BC, dof: Dof, mesh_data: MeshData, solver: Solver, amplitude: Optional[Amplitude]) -> None:
         super().__init__(bc, dof, mesh_data, solver, amplitude)
         self.create_dof_values()
 
-    def get_surface_from_bc_element(self, bc_element_id: int, bc_element: ndarray) -> List[Tuple[int, str]]:
+    def get_surface_from_bc_element(self, bc_element_id: int, bc_element: ndarray) -> list[tuple[int, str]]:
         nodes = self.mesh_data.nodes
         elements = self.mesh_data.elements
         element_surface = []
         for element_id, element in enumerate(elements):
             is_element_surface = all(in1d(bc_element, element))
             if is_element_surface:
                 nodes_in_element = in1d(element, bc_element)
                 connectivity = elements[element_id]
                 node_coords = nodes[connectivity]
                 iso_element_type = get_iso_element_type(node_coords)
                 iso_element_shape = iso_element_shape_dict[iso_element_type]
                 surface_names = [surface_name for surface_name, nodes_on_surface in
-                                 iso_element_shape.nodes_to_surface_dict.items() if
+                                 iso_element_shape.nodes_on_surface_dict.items() if
                                  all(nodes_on_surface == nodes_in_element)]
                 if len(surface_names) == 1:
                     element_surface.append((element_id, surface_names[0]))
                 else:
                     raise NotImplementedError(error_style(f'the surface of element {element_id} is wrong'))
 
         if len(element_surface) == 1:
             return element_surface
         else:
             raise NotImplementedError(error_style(f'the surface of bc_element {bc_element_id} is wrong'))
 
-    def get_surface_from_elements_nodes(self, element_id: int, node_ids: List[int]) -> List[Tuple[int, str]]:
+    def get_surface_from_elements_nodes(self, element_id: int, node_ids: list[int]) -> list[tuple[int, str]]:
         nodes = self.mesh_data.nodes
         elements = self.mesh_data.elements
         element_surface = []
         nodes_in_element = in1d(elements[element_id], node_ids)
         connectivity = elements[element_id]
         node_coords = nodes[connectivity]
         iso_element_type = get_iso_element_type(node_coords)
         iso_element_shape = iso_element_shape_dict[iso_element_type]
         surface_names = [surface_name for surface_name, nodes_on_surface in
-                         iso_element_shape.nodes_to_surface_dict.items() if
+                         iso_element_shape.nodes_on_surface_dict.items() if
                          sum(logical_and(nodes_in_element, nodes_on_surface)) == len(
                              iso_element_shape.bc_surface_nodes_dict[surface_name])]
 
         for surface_name in surface_names:
             element_surface.append((element_id, surface_name))
 
         if 1 <= len(element_surface) <= iso_element_shape.bc_surface_number:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfem-0.1.2/src/pyfem/bc/get_bc_data.py` & `pyfem-0.1.3/src/pyfem/bc/get_bc_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,52 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import Optional
+from typing import Union, Optional
 
 from pyfem.bc.BaseBC import BaseBC
 from pyfem.bc.DirichletBC import DirichletBC
 from pyfem.bc.NeumannBCConcentrated import NeumannBCConcentrated
 from pyfem.bc.NeumannBCDistributed import NeumannBCDistributed
 from pyfem.io.Amplitude import Amplitude
 from pyfem.io.BC import BC
 from pyfem.io.Dof import Dof
 from pyfem.io.Solver import Solver
 from pyfem.mesh.MeshData import MeshData
 from pyfem.utils.colors import error_style
 
+BCData = Union[BaseBC, DirichletBC, NeumannBCConcentrated, NeumannBCDistributed]
+
 bc_data_dict = {
     'DirichletBC': DirichletBC,
     'NeumannBCConcentrated': NeumannBCConcentrated,
     'NeumannBCDistributed': NeumannBCDistributed
 }
 
 
 def get_bc_data(bc: BC,
                 dof: Dof,
                 mesh_data: MeshData,
                 solver: Solver,
-                amplitude: Optional[Amplitude]) -> BaseBC:
+                amplitude: Optional[Amplitude]) -> BCData:
+    """
+    工厂函数，用于根据边界条件属性生产不同的边界条件对象。
+
+    Args:
+        bc(BC): 边界条件属性
+        dof(Dof): 自由度属性
+        mesh_data(MeshData): 网格数据对象
+        solver(Solver): 求解器属性
+        amplitude(Optional[Amplitude]): 幅值属性
+
+    :return: 边界条件对象
+    :rtype: BCData
+    """
+
     class_name = f'{bc.category}{bc.type}'.strip().replace(' ', '')
 
     if class_name in bc_data_dict:
         return bc_data_dict[class_name](bc=bc,
                                         dof=dof,
                                         mesh_data=mesh_data,
                                         solver=solver,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfem-0.1.2/src/pyfem/elements/BaseElement.py` & `pyfem-0.1.3/src/pyfem/elements/BaseElement.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,184 +1,195 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 from copy import deepcopy
-from typing import Dict, List, Tuple
 
 from numpy import dot, ndarray
 from numpy.linalg import det
 
-from pyfem.elements.IsoElementShape import IsoElementShape
 from pyfem.fem.Timer import Timer
 from pyfem.io.Dof import Dof
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
+from pyfem.isoelements.IsoElementShape import IsoElementShape
+from pyfem.materials.get_material_data import MaterialData
 from pyfem.utils.colors import error_style
-from pyfem.utils.data_types import MaterialData
 from pyfem.utils.mechanics import inverse
 from pyfem.utils.visualization import object_slots_to_string_ndarray, get_ordinal_number
 
 
 class BaseElement:
     """
-    单元数据的基类。
+    单元数据实体的基类。
 
     :ivar element_id: 单元序号
     :vartype element_id: int
 
     :ivar iso_element_shape: 等参元对象
     :vartype iso_element_shape: IsoElementShape
 
     :ivar connectivity: 单元节点序号列表
     :vartype connectivity: ndarray
 
     :ivar node_coords: 单元节点坐标列表
     :vartype node_coords: ndarray
 
+    :ivar assembly_conn: 全局单元节点序号列表
+    :vartype assembly_conn: ndarray
+
     :ivar dof: io.Dof的自由度对象
     :vartype dof: Dof
 
     :ivar materials: io.Material的材料对象列表
-    :vartype materials: List[Material]
+    :vartype materials: list[Material]
 
-    :ivar section: io.Section的截面对象
-    :vartype section: List[Section]
+    :ivar section: io.Section的截面对象列表
+    :vartype section: list[Section]
 
     :ivar material_data_list: 材料数据对象列表
-    :vartype material_data_list: List[MaterialData]
+    :vartype material_data_list: list[MaterialData]
 
     :ivar timer: 计时器对象
     :vartype timer: Timer
 
     :ivar dof_names: 自由度名称列表
-    :vartype dof_names: List[str]
+    :vartype dof_names: list[str]
 
     :ivar gp_number: 积分点个数
     :vartype gp_number: int
 
     :ivar gp_jacobis: 积分点处的雅克比矩阵列表
     :vartype gp_jacobis: ndarray(gp_number, 空间维度, 空间维度)
 
     :ivar gp_jacobi_invs: 积分点处的雅克比矩阵逆矩阵列表
-    :vartype gp_jacobi_invs: ndarray(gp_number, 空间维度, 空间维度)
+    :vartype gp_jacobi_invs: ndarray(gp_number,)
 
     :ivar gp_jacobi_dets: 积分点处的雅克比矩阵行列式列表
     :vartype gp_jacobi_dets: ndarray(gp_number,)
 
     :ivar gp_weight_times_jacobi_dets: 积分点处的雅克比矩阵行列式乘以积分权重列表
     :vartype gp_weight_times_jacobi_dets: ndarray(gp_number,)
 
     :ivar gp_ddsddes: 积分点处的材料刚度矩阵列表
     :vartype gp_ddsddes: ndarray
 
     :ivar gp_state_variables: 积分点处的状态变量列表
-    :vartype gp_state_variables: List[Dict[str, ndarray]]
+    :vartype gp_state_variables: list[dict[str, ndarray]]
 
     :ivar gp_state_variables_new: 积分点处局部增量时刻的状态变量列表
-    :vartype gp_state_variables_new: List[Dict[str, ndarray]]
+    :vartype gp_state_variables_new: list[dict[str, ndarray]]
 
     :ivar gp_field_variables: 积分点处场变量字典
-    :vartype gp_field_variables: Dict[str, ndarray]
+    :vartype gp_field_variables: dict[str, ndarray]
 
     :ivar element_dof_number: 单元自由度总数
     :vartype element_dof_number: int
 
     :ivar element_dof_ids: 单元全局自由度编号列表
-    :vartype element_dof_ids: List[int]
+    :vartype element_dof_ids: list[int]
 
     :ivar element_dof_values: 单元全局自由度数值列表
-    :vartype element_dof_values: ndarray(element_dof_number)
+    :vartype element_dof_values: ndarray(element_dof_number,)
 
     :ivar element_ddof_values: 单元全局自由度数值增量列表
-    :vartype element_ddof_values: ndarray(element_dof_number)
+    :vartype element_ddof_values: ndarray(element_dof_number,)
 
     :ivar element_fint: 单元内力列表
-    :vartype element_fint: ndarray(element_dof_number)
+    :vartype element_fint: ndarray(element_dof_number,)
 
     :ivar element_stiffness: 单元刚度矩阵
     :vartype element_stiffness: ndarray(element_dof_number, element_dof_number)
 
     :ivar element_average_field_variables: 单元磨平后的场变量字典
-    :vartype element_average_field_variables: Dict[str, ndarray]
+    :vartype element_average_field_variables: dict[str, ndarray]
 
     :ivar allowed_material_data_list: 许可的单元材料数据类名列表
-    :vartype allowed_material_data_list: List[Tuple]
+    :vartype allowed_material_data_list: list[Tuple]
 
     :ivar allowed_material_number: 许可的单元材料数量
     :vartype allowed_material_number: int
     """
-    __slots__: Tuple = ('element_id',
-                        'iso_element_shape',
-                        'connectivity',
-                        'node_coords',
-                        'assembly_conn',
-                        'dof',
-                        'materials',
-                        'section',
-                        'material_data_list',
-                        'timer',
-                        'dof_names',
-                        'gp_number',
-                        'gp_jacobis',
-                        'gp_jacobi_invs',
-                        'gp_jacobi_dets',
-                        'gp_weight_times_jacobi_dets',
-                        'gp_ddsddes',
-                        'gp_state_variables',
-                        'gp_state_variables_new',
-                        'gp_field_variables',
-                        'element_dof_number',
-                        'element_dof_ids',
-                        'element_dof_values',
-                        'element_ddof_values',
-                        'element_fint',
-                        'element_stiffness',
-                        'element_average_field_variables',
-                        'allowed_material_data_list',
-                        'allowed_material_number')
+
+    __slots_dict__: dict = {
+        'element_id': ('int', '单元序号'),
+        'iso_element_shape': ('IsoElementShape', '等参元对象'),
+        'dimension': ('int', '单元空间维度'),
+        'topological_dimension': ('int', '单元拓扑维度'),
+        'connectivity': ('ndarray', '单元节点序号列表'),
+        'node_coords': ('ndarray', '单元节点坐标列表'),
+        'assembly_conn': ('ndarray', '全局单元节点序号列表'),
+        'dof': ('Dof', 'io.Dof的自由度对象'),
+        'materials': ('list[Material]', 'io.Material的材料对象列表'),
+        'section': ('list[Section]', 'io.Section的截面对象列表'),
+        'material_data_list': ('list[MaterialData]', '材料数据对象列表'),
+        'timer': ('Timer', '计时器对象'),
+        'dof_names': ('list[str]', '自由度名称列表'),
+        'gp_number': ('int', '积分点个数'),
+        'gp_jacobis': ('ndarray(gp_number, 空间维度, 空间维度)', '积分点处的雅克比矩阵列表'),
+        'gp_jacobi_invs': ('ndarray(gp_number,)', '积分点处的雅克比矩阵逆矩阵列表'),
+        'gp_jacobi_dets': ('ndarray(gp_number,)', '积分点处的雅克比矩阵行列式列表'),
+        'gp_weight_times_jacobi_dets': ('ndarray(gp_number,)', '积分点处的雅克比矩阵行列式乘以积分权重列表'),
+        'gp_ddsddes': ('ndarray', '积分点处的材料刚度矩阵列表'),
+        'gp_state_variables': ('list[dict[str, ndarray]]', '积分点处的状态变量列表'),
+        'gp_state_variables_new': ('list[dict[str, ndarray]]', '积分点处局部增量时刻的状态变量列表'),
+        'gp_field_variables': ('dict[str, ndarray]', '积分点处场变量字典'),
+        'element_dof_number': ('int', '单元自由度总数'),
+        'element_dof_ids': ('list[int]', '单元全局自由度编号列表'),
+        'element_dof_values': ('ndarray(element_dof_number,)', '单元全局自由度数值列表'),
+        'element_ddof_values': ('ndarray(element_dof_number,)', '单元全局自由度数值增量列表'),
+        'element_fint': ('ndarray(element_dof_number,)', '单元内力列表'),
+        'element_stiffness': ('ndarray(element_dof_number, element_dof_number)', '单元刚度矩阵'),
+        'element_average_field_variables': ('dict[str, ndarray]', '单元磨平后的场变量字典'),
+        'allowed_material_data_list': ('list[Tuple]', '许可的单元材料数据类名列表'),
+        'allowed_material_number': ('int', '许可的单元材料数量')
+    }
+
+    __slots__: list = [slot for slot in __slots_dict__.keys()]
 
     def __init__(self, element_id: int,
                  iso_element_shape: IsoElementShape,
                  connectivity: ndarray,
                  node_coords: ndarray) -> None:
         self.element_id: int = element_id
         self.iso_element_shape: IsoElementShape = iso_element_shape
+        self.dimension: int = iso_element_shape.dimension
+        self.topological_dimension: int = iso_element_shape.topological_dimension
         self.connectivity: ndarray = connectivity
         self.node_coords: ndarray = node_coords
         self.assembly_conn: ndarray = None  # type: ignore
 
         self.dof: Dof = None  # type: ignore
-        self.materials: List[Material] = None  # type: ignore
+        self.materials: list[Material] = None  # type: ignore
         self.section: Section = None  # type: ignore
-        self.material_data_list: List[MaterialData] = None  # type: ignore
+        self.material_data_list: list[MaterialData] = None  # type: ignore
         self.timer: Timer = None  # type: ignore
 
-        self.dof_names: List[str] = list()
+        self.dof_names: list[str] = list()
 
         self.gp_number: int = self.iso_element_shape.gp_number
         self.gp_jacobis: ndarray = None  # type: ignore
         self.gp_jacobi_invs: ndarray = None  # type: ignore
         self.gp_jacobi_dets: ndarray = None  # type: ignore
         self.gp_weight_times_jacobi_dets: ndarray = None  # type: ignore
-        self.gp_ddsddes: List[ndarray] = list()
-        self.gp_state_variables: List[Dict[str, ndarray]] = [{} for _ in range(self.gp_number)]
-        self.gp_state_variables_new: List[Dict[str, ndarray]] = [{} for _ in range(self.gp_number)]
-        self.gp_field_variables: Dict[str, ndarray] = dict()
+        self.gp_ddsddes: list[ndarray] = list()
+        self.gp_state_variables: list[dict[str, ndarray]] = [{} for _ in range(self.gp_number)]
+        self.gp_state_variables_new: list[dict[str, ndarray]] = [{} for _ in range(self.gp_number)]
+        self.gp_field_variables: dict[str, ndarray] = dict()
         self.cal_jacobi()
 
         self.element_dof_number: int = 0
-        self.element_dof_ids: List[int] = list()
+        self.element_dof_ids: list[int] = list()
         self.element_dof_values: ndarray = None  # type: ignore
         self.element_ddof_values: ndarray = None  # type: ignore
         self.element_fint: ndarray = None  # type: ignore
         self.element_stiffness: ndarray = None  # type: ignore
-        self.element_average_field_variables: Dict[str, ndarray] = dict()
+        self.element_average_field_variables: dict[str, ndarray] = dict()
 
-        self.allowed_material_data_list: List[Tuple] = list()
+        self.allowed_material_data_list: list[tuple] = list()
         self.allowed_material_number: int = 0
 
     def to_string(self, level: int = 1) -> str:
         return object_slots_to_string_ndarray(self, level)
 
     def show(self) -> None:
         print(self.to_string())
@@ -268,15 +279,18 @@
 
     def update_element_ddof_values(self, global_ddof_values: ndarray) -> None:
         self.element_ddof_values = global_ddof_values[self.element_dof_ids]
 
     def update_element_state_variables(self) -> None:
         self.gp_state_variables = deepcopy(self.gp_state_variables_new)
 
-    def update_element_material_stiffness_fint(self) -> None:
+    def update_element_material_stiffness_fint(self,
+                                               is_update_material: bool = True,
+                                               is_update_stiffness: bool = True,
+                                               is_update_fint: bool = True, ) -> None:
         pass
 
     def update_material_state(self) -> None:
         pass
 
     def update_element_stiffness(self) -> None:
         pass
@@ -285,8 +299,10 @@
         pass
 
     def update_element_field_variables(self) -> None:
         pass
 
 
 if __name__ == "__main__":
-    pass
+    from pyfem.utils.visualization import print_slots_dict
+
+    print_slots_dict(BaseElement.__slots_dict__)
```

### Comparing `pyfem-0.1.2/src/pyfem/elements/IsoElementDiagram.py` & `pyfem-0.1.3/src/pyfem/isoelements/IsoElementDiagram.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 """
 
 """
 
 
 class IsoElementDiagram:
     """
-    等参元的形状示意图
+    等参元的形状示意图。
     """
 
-    __slots__ = ()
+    __slots__: list = []
 
     line2 = r"""
     0---------------1
             +-->x0"""
 
     line3 = r"""
     0-------1-------2
```

### Comparing `pyfem-0.1.2/src/pyfem/elements/SolidPhaseFieldDamagePlaneSmallStrain.py` & `pyfem-0.1.3/src/pyfem/elements/SolidSmallStrain.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,232 +1,251 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import List
-
-from numpy import array, zeros, dot, ndarray, average, ix_, outer
+from numpy import array, zeros, dot, ndarray, average
 
 from pyfem.elements.BaseElement import BaseElement
-from pyfem.elements.IsoElementShape import IsoElementShape
 from pyfem.fem.Timer import Timer
 from pyfem.fem.constants import DTYPE
 from pyfem.io.Dof import Dof
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
+from pyfem.isoelements.IsoElementShape import IsoElementShape
+from pyfem.materials.get_material_data import MaterialData
 from pyfem.utils.colors import error_style
-from pyfem.utils.data_types import MaterialData
-from pyfem.utils.mechanics import get_decompose_energy
 
 
-class SolidPhaseFieldDamagePlaneSmallStrain(BaseElement):
-    __slots__ = BaseElement.__slots__ + ('gp_b_matrices',
-                                         'gp_b_matrices_transpose',
-                                         'gp_strains',
-                                         'gp_stresses',
-                                         'gp_phases',
-                                         'gp_phase_fluxes',
-                                         'gp_ddsddps',
-                                         'dof_u',
-                                         'dof_p')
+class SolidSmallStrain(BaseElement):
+    """
+    固体小变形单元。
+
+    :ivar gp_b_matrices: 积分点处的B矩阵列表
+    :vartype gp_b_matrices: ndarray
+
+    :ivar gp_b_matrices_transpose: 积分点处的B矩阵转置列表
+    :vartype gp_b_matrices_transpose: ndarray
+
+    :ivar gp_strains: 积分点处的应变列表
+    :vartype gp_strains: list[ndarray]
+
+    :ivar gp_stresses: 积分点处的应力列表
+    :vartype gp_stresses: list[ndarray]
+
+    :ivar ntens: 总应力数量
+    :vartype ntens: int
+
+    :ivar ndi: 轴向应力数量
+    :vartype ndi: int
+
+    :ivar nshr: 剪切应力数量
+    :vartype nshr: int
+    """
+
+    __slots_dict__: dict = {
+        'gp_b_matrices': ('ndarray', '积分点处的B矩阵列表'),
+        'gp_b_matrices_transpose': ('ndarray', '积分点处的B矩阵转置列表'),
+        'gp_strains': ('list[ndarray]', '积分点处的应变列表'),
+        'gp_stresses': ('list[ndarray]', '积分点处的应力列表'),
+        'ntens': ('int', '总应力数量'),
+        'ndi': ('int', '轴向应力数量'),
+        'nshr': ('int', '剪切应力数量')
+    }
+
+    __slots__: list = BaseElement.__slots__ + [slot for slot in __slots_dict__.keys()]
 
     def __init__(self, element_id: int,
                  iso_element_shape: IsoElementShape,
                  connectivity: ndarray,
                  node_coords: ndarray,
                  dof: Dof,
-                 materials: List[Material],
+                 materials: list[Material],
                  section: Section,
-                 material_data_list: List[MaterialData],
+                 material_data_list: list[MaterialData],
                  timer: Timer) -> None:
 
         super().__init__(element_id, iso_element_shape, connectivity, node_coords)
 
-        self.allowed_material_data_list = [('ElasticIsotropic', 'PlasticKinematicHardening', 'ViscoElasticMaxwell'),
-                                           ('PhaseFieldDamage',)]
-        self.allowed_material_number = len(self.allowed_material_data_list)
+        self.allowed_material_data_list = [('ElasticIsotropic', 'PlasticKinematicHardening', 'ViscoElasticMaxwell')]
+        self.allowed_material_number = 1
 
         self.dof = dof
         self.materials = materials
         self.section = section
         self.material_data_list = material_data_list
         self.check_materials()
         self.timer = timer
 
-        self.dof_names = ['u1', 'u2', 'phi']
+        if self.dimension == 2:
+            self.dof_names = ['u1', 'u2']
+            self.ntens = 4
+            self.ndi = 3
+            self.nshr = 1
+        elif self.dimension == 3:
+            self.dof_names = ['u1', 'u2', 'u3']
+            self.ntens = 6
+            self.ndi = 3
+            self.nshr = 3
+        else:
+            error_msg = f'{self.dimension} is not the supported dimension'
+            raise NotImplementedError(error_style(error_msg))
+
         if dof.names != self.dof_names:
             error_msg = f'{dof.names} is not the supported dof of {type(self).__name__} element'
             raise NotImplementedError(error_style(error_msg))
 
         element_dof_number = len(self.dof_names) * self.iso_element_shape.nodes_number
         self.element_dof_number = element_dof_number
         self.element_dof_values = zeros(element_dof_number, dtype=DTYPE)
         self.element_ddof_values = zeros(element_dof_number, dtype=DTYPE)
         self.element_fint = zeros(element_dof_number, dtype=DTYPE)
         self.element_stiffness = None  # type: ignore
 
         self.gp_b_matrices: ndarray = None  # type: ignore
         self.gp_b_matrices_transpose: ndarray = None  # type: ignore
-        self.gp_strains: List[ndarray] = None  # type: ignore
-        self.gp_stresses: List[ndarray] = None  # type: ignore
-        self.gp_phases: List[ndarray] = None  # type: ignore
-        self.gp_phase_fluxes: List[ndarray] = None  # type: ignore
-        self.gp_ddsddps: List[ndarray] = None  # type: ignore
-
-        # for i in range(self.gp_number):
-        #     self.gp_state_variables[i]['history_energy'] = array([0.0])
-        #     self.gp_state_variables_new[i]['history_energy'] = array([0.0])
-
-        self.dof_u = []
-        self.dof_p = []
-        for i in range(self.iso_element_shape.nodes_number):
-            self.dof_u += [len(self.dof_names) * i + 0, len(self.dof_names) * i + 1]
-            self.dof_p += [len(self.dof_names) * i + 2]
+        self.gp_strains: list[ndarray] = None  # type: ignore
+        self.gp_stresses: list[ndarray] = None  # type: ignore
 
         self.create_gp_b_matrices()
 
     def create_gp_b_matrices(self) -> None:
-        self.gp_b_matrices = zeros(shape=(self.gp_number, 3, len(self.dof_u)), dtype=DTYPE)
-
-        for igp, (gp_shape_gradient, gp_jacobi_inv) in \
-                enumerate(zip(self.iso_element_shape.gp_shape_gradients, self.gp_jacobi_invs)):
-            gp_dhdx = dot(gp_shape_gradient.transpose(), gp_jacobi_inv)
-            for i, val in enumerate(gp_dhdx):
-                self.gp_b_matrices[igp, 0, i * 2] = val[0]
-                self.gp_b_matrices[igp, 1, i * 2 + 1] = val[1]
-                self.gp_b_matrices[igp, 2, i * 2] = val[1]
-                self.gp_b_matrices[igp, 2, i * 2 + 1] = val[0]
+        if self.dimension == 2:
+            self.gp_b_matrices = zeros(shape=(self.gp_number, 3, self.element_dof_number), dtype=DTYPE)
+            for igp, (gp_shape_gradient, gp_jacobi_inv) in \
+                    enumerate(zip(self.iso_element_shape.gp_shape_gradients, self.gp_jacobi_invs)):
+                gp_dhdx = dot(gp_shape_gradient.transpose(), gp_jacobi_inv)
+                for i, val in enumerate(gp_dhdx):
+                    self.gp_b_matrices[igp, 0, i * 2] = val[0]
+                    self.gp_b_matrices[igp, 1, i * 2 + 1] = val[1]
+                    self.gp_b_matrices[igp, 2, i * 2] = val[1]
+                    self.gp_b_matrices[igp, 2, i * 2 + 1] = val[0]
+
+        elif self.dimension == 3:
+            self.gp_b_matrices = zeros(shape=(self.iso_element_shape.gp_number, 6, self.element_dof_number))
+            for igp, (gp_shape_gradient, gp_jacobi_inv) in \
+                    enumerate(zip(self.iso_element_shape.gp_shape_gradients, self.gp_jacobi_invs)):
+                gp_dhdx = dot(gp_shape_gradient.transpose(), gp_jacobi_inv)
+                for i, val in enumerate(gp_dhdx):
+                    self.gp_b_matrices[igp, 0, i * 3] = val[0]
+                    self.gp_b_matrices[igp, 1, i * 3 + 1] = val[1]
+                    self.gp_b_matrices[igp, 2, i * 3 + 2] = val[2]
+                    self.gp_b_matrices[igp, 3, i * 3] = val[1]
+                    self.gp_b_matrices[igp, 3, i * 3 + 1] = val[0]
+                    self.gp_b_matrices[igp, 4, i * 3] = val[2]
+                    self.gp_b_matrices[igp, 4, i * 3 + 2] = val[0]
+                    self.gp_b_matrices[igp, 5, i * 3 + 1] = val[2]
+                    self.gp_b_matrices[igp, 5, i * 3 + 2] = val[1]
 
         self.gp_b_matrices_transpose = array([gp_b_matrix.transpose() for gp_b_matrix in self.gp_b_matrices])
 
-    def update_material_state(self) -> None:
-        pass
-
-    def update_element_material_stiffness_fint(self) -> None:
+    def update_element_material_stiffness_fint(self,
+                                               is_update_material: bool = True,
+                                               is_update_stiffness: bool = True,
+                                               is_update_fint: bool = True, ) -> None:
         element_id = self.element_id
         timer = self.timer
-
-        dimension = self.iso_element_shape.dimension
+        ntens = self.ntens
+        ndi = self.ndi
+        nshr = self.nshr
 
         gp_number = self.gp_number
-        gp_shape_values = self.iso_element_shape.gp_shape_values
-        gp_shape_gradients = self.iso_element_shape.gp_shape_gradients
         gp_b_matrices = self.gp_b_matrices
         gp_b_matrices_transpose = self.gp_b_matrices_transpose
         gp_weight_times_jacobi_dets = self.gp_weight_times_jacobi_dets
 
         gp_state_variables = self.gp_state_variables
         gp_state_variables_new = self.gp_state_variables_new
 
         element_dof_values = self.element_dof_values
         element_ddof_values = self.element_ddof_values
 
-        u = element_dof_values[self.dof_u]
-        phi = element_dof_values[self.dof_p]
+        material_data = self.material_data_list[0]
 
-        du = element_ddof_values[self.dof_u]
-        dphi = element_ddof_values[self.dof_p]
+        if is_update_stiffness:
+            self.element_stiffness = zeros(shape=(self.element_dof_number, self.element_dof_number), dtype=DTYPE)
 
-        self.element_stiffness = zeros(shape=(self.element_dof_number, self.element_dof_number), dtype=DTYPE)
-        self.element_fint = zeros(self.element_dof_number, dtype=DTYPE)
+        if is_update_fint:
+            self.element_fint = zeros(self.element_dof_number, dtype=DTYPE)
 
-        solid_material_data = self.material_data_list[0]
-        phase_material_data = self.material_data_list[1]
-
-        gc = phase_material_data.gc  # type: ignore
-        lc = phase_material_data.lc  # type: ignore
-
-        gp_ddsddes = []
-        gp_strains = []
-        gp_stresses = []
-        # gp_ddsddps = []
-        gp_phases = []
-        # gp_phase_fluxes = []
+        if is_update_material:
+            self.gp_ddsddes = list()
+            self.gp_strains = list()
+            self.gp_stresses = list()
 
         for i in range(gp_number):
-            gp_weight_times_jacobi_det = gp_weight_times_jacobi_dets[i]
-            gp_shape_value = gp_shape_values[i]
-            gp_shape_gradient = gp_shape_gradients[i]
-            gp_b_matrix_transpose = gp_b_matrices_transpose[i]
-            gp_b_matrix = gp_b_matrices[i]
-            gp_strain = dot(gp_b_matrix, u)
-            gp_dstrain = dot(gp_b_matrix, du)
-            gp_phase = dot(gp_shape_value, phi)
-            gp_dphase = dot(gp_shape_value, dphi)
-            gp_phase_gradient = dot(gp_shape_gradient, phi)
-            gp_dphase_gradient = dot(gp_shape_gradient, dphi)
-
-            degradation = min((1.0 - gp_phase) ** 2 + 1.0e-7, 1.0)
-
-            variable = {'strain': gp_strain, 'dstrain': gp_dstrain}
-            gp_ddsdde, gp_output = solid_material_data.get_tangent(variable=variable,
-                                                                   state_variable=gp_state_variables[i],
-                                                                   state_variable_new=gp_state_variables_new[i],
-                                                                   element_id=element_id,
-                                                                   igp=i,
-                                                                   ntens=4,
-                                                                   ndi=3,
-                                                                   nshr=1,
-                                                                   timer=timer)
-            gp_stress = gp_output['stress'] * degradation
-
-            energy_positive, energy_negative = get_decompose_energy(gp_strain + gp_dstrain, gp_stress, dimension)
-
-            # if energy_positive > gp_state_variables_new[i]['history_energy'][0]:
-            #     gp_state_variables_new[i]['history_energy'][0] = energy_positive
-            # else:
-            #     energy_positive = gp_state_variables_new[i]['history_energy'][0]
-
-            self.element_stiffness[ix_(self.dof_u, self.dof_u)] += \
-                dot(gp_b_matrix_transpose, dot(gp_ddsdde, gp_b_matrix)) * gp_weight_times_jacobi_det * degradation
-
-            self.element_fint[self.dof_u] += dot(gp_b_matrix_transpose, gp_stress) * gp_weight_times_jacobi_det
-
-            self.element_stiffness[ix_(self.dof_p, self.dof_p)] += \
-                ((gc / lc + 2.0 * energy_positive) * outer(gp_shape_value, gp_shape_value) +
-                 gc * lc * dot((gp_phase + gp_dphase), (gp_phase + gp_dphase).transpose())) * gp_weight_times_jacobi_det
-
-            self.element_fint[self.dof_p] += \
-                (gc * lc * dot(gp_shape_gradient.transpose(), gp_phase_gradient) +
-                 gc / lc * gp_shape_value * (gp_phase + gp_dphase) +
-                 2.0 * ((gp_phase + gp_dphase) - 1.0) * gp_shape_value * energy_positive) * gp_weight_times_jacobi_det
-
-            gp_ddsddes.append(gp_ddsdde)
-            gp_strains.append(gp_strain)
-            gp_stresses.append(gp_stress)
-            # gp_ddsddps.append(gp_ddsddp)
-            gp_phases.append(gp_phase)
-            # gp_phase_fluxes.append(gp_phase_flux)
-
-        self.gp_ddsddes = gp_ddsddes
-        self.gp_strains = gp_strains
-        self.gp_stresses = gp_stresses
-        # self.gp_ddsddps = gp_ddsddps
-        self.gp_phases = gp_phases
-        # self.gp_phase_fluxes = gp_phase_fluxes
-
-    def update_element_stiffness(self) -> None:
-        raise NotImplementedError()
+            if is_update_material:
+                gp_weight_times_jacobi_det = gp_weight_times_jacobi_dets[i]
+                gp_b_matrix_transpose = gp_b_matrices_transpose[i]
+                gp_b_matrix = gp_b_matrices[i]
+                gp_strain = dot(gp_b_matrix, element_dof_values)
+                gp_dstrain = dot(gp_b_matrix, element_ddof_values)
+                variable = {'strain': gp_strain, 'dstrain': gp_dstrain}
+                gp_ddsdde, gp_output = material_data.get_tangent(variable=variable,
+                                                                 state_variable=gp_state_variables[i],
+                                                                 state_variable_new=gp_state_variables_new[i],
+                                                                 element_id=element_id,
+                                                                 igp=i,
+                                                                 ntens=ntens,
+                                                                 ndi=ndi,
+                                                                 nshr=nshr,
+                                                                 timer=timer)
+                gp_stress = gp_output['stress']
+                self.gp_ddsddes.append(gp_ddsdde)
+                self.gp_strains.append(gp_strain)
+                self.gp_stresses.append(gp_stress)
+            else:
+                gp_b_matrix_transpose = gp_b_matrices_transpose[i]
+                gp_b_matrix = gp_b_matrices[i]
+                gp_weight_times_jacobi_det = gp_weight_times_jacobi_dets[i]
+                gp_ddsdde = self.gp_ddsddes[i]
+                gp_stress = self.gp_stresses[i]
+
+            if is_update_stiffness:
+                self.element_stiffness += dot(gp_b_matrix_transpose, dot(gp_ddsdde, gp_b_matrix)) * \
+                                          gp_weight_times_jacobi_det
 
-    def update_element_fint(self) -> None:
-        raise NotImplementedError()
+            if is_update_fint:
+                self.element_fint += dot(gp_b_matrix_transpose, gp_stress) * gp_weight_times_jacobi_det
 
     def update_element_field_variables(self) -> None:
         gp_stresses = self.gp_stresses
         gp_strains = self.gp_strains
 
         average_strain = average(gp_strains, axis=0)
         average_stress = average(gp_stresses, axis=0)
 
         self.gp_field_variables['strain'] = array(gp_strains, dtype=DTYPE)
         self.gp_field_variables['stress'] = array(gp_stresses, dtype=DTYPE)
 
-        self.element_average_field_variables['E11'] = average_strain[0]
-        self.element_average_field_variables['E22'] = average_strain[1]
-        self.element_average_field_variables['E12'] = average_strain[2]
-        self.element_average_field_variables['S11'] = average_stress[0]
-        self.element_average_field_variables['S22'] = average_stress[1]
-        self.element_average_field_variables['S12'] = average_stress[2]
+        if self.dimension == 2:
+            self.element_average_field_variables['E11'] = average_strain[0]
+            self.element_average_field_variables['E22'] = average_strain[1]
+            self.element_average_field_variables['E12'] = average_strain[2]
+            self.element_average_field_variables['S11'] = average_stress[0]
+            self.element_average_field_variables['S22'] = average_stress[1]
+            self.element_average_field_variables['S12'] = average_stress[2]
+
+        elif self.dimension == 3:
+            self.element_average_field_variables['E11'] = average_strain[0]
+            self.element_average_field_variables['E22'] = average_strain[1]
+            self.element_average_field_variables['E33'] = average_strain[2]
+            self.element_average_field_variables['E12'] = average_strain[3]
+            self.element_average_field_variables['E13'] = average_strain[4]
+            self.element_average_field_variables['E23'] = average_strain[5]
+            self.element_average_field_variables['S11'] = average_stress[0]
+            self.element_average_field_variables['S22'] = average_stress[1]
+            self.element_average_field_variables['S33'] = average_stress[2]
+            self.element_average_field_variables['S12'] = average_stress[3]
+            self.element_average_field_variables['S13'] = average_stress[4]
+            self.element_average_field_variables['S23'] = average_stress[5]
 
 
 if __name__ == "__main__":
-    pass
+    from pyfem.utils.visualization import print_slots_dict
+
+    print_slots_dict(SolidSmallStrain.__slots_dict__)
+
+    # from pyfem.Job import Job
+    #
+    # job = Job(r'..\..\..\examples\mechanical\1element\hex8\Job-1.toml')
+    #
+    # job.assembly.element_data_list[0].show()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfem-0.1.2/src/pyfem/elements/SolidThermalPlaneSmallStrain.py` & `pyfem-0.1.3/src/pyfem/elements/Thermal.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,269 +1,197 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import List
-
-from numpy import array, zeros, dot, ndarray, average, ix_, outer
+from numpy import array, zeros, dot, ndarray, average
 
 from pyfem.elements.BaseElement import BaseElement
-from pyfem.elements.IsoElementShape import IsoElementShape
 from pyfem.fem.Timer import Timer
 from pyfem.fem.constants import DTYPE
 from pyfem.io.Dof import Dof
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
+from pyfem.isoelements.IsoElementShape import IsoElementShape
+from pyfem.materials.get_material_data import MaterialData
 from pyfem.utils.colors import error_style
-from pyfem.utils.data_types import MaterialData
 
 
-class SolidThermalPlaneSmallStrain(BaseElement):
-    __slots__ = BaseElement.__slots__ + ('gp_b_matrices', 'gp_b_matrices_transpose', 'gp_strains', 'gp_stresses',
-                                         'gp_temperatures', 'gp_heat_fluxes', 'gp_ddsddts', 'dof_u', 'dof_T')
+class Thermal(BaseElement):
+    """
+    温度单元。
+
+    :ivar gp_temperatures: 积分点处的温度列表
+    :vartype gp_temperatures: ndarray
+
+    :ivar gp_heat_fluxes: 积分点处的热流密度列表
+    :vartype gp_heat_fluxes: ndarray
+
+    :ivar gp_ddsddts: 积分点处的材料热传导系数矩阵列表
+    :vartype gp_ddsddts: list[ndarray]
+
+    :ivar ntens: 总应力数量
+    :vartype ntens: int
+
+    :ivar ndi: 轴向应力数量
+    :vartype ndi: int
+
+    :ivar nshr: 剪切应力数量
+    :vartype nshr: int
+    """
+
+    __slots_dict__: dict = {
+        'gp_temperatures': ('ndarray', '积分点处的温度列表'),
+        'gp_heat_fluxes': ('ndarray', '积分点处的热流密度列表'),
+        'gp_ddsddts': ('list[ndarray]', '积分点处的材料热传导系数矩阵列表'),
+        'ntens': ('int', '总应力数量'),
+        'ndi': ('int', '轴向应力数量'),
+        'nshr': ('int', '剪切应力数量')
+    }
+
+    __slots__: list = BaseElement.__slots__ + [slot for slot in __slots_dict__.keys()]
 
     def __init__(self, element_id: int,
                  iso_element_shape: IsoElementShape,
                  connectivity: ndarray,
                  node_coords: ndarray,
                  dof: Dof,
-                 materials: List[Material],
+                 materials: list[Material],
                  section: Section,
-                 material_data_list: List[MaterialData],
+                 material_data_list: list[MaterialData],
                  timer: Timer) -> None:
 
         super().__init__(element_id, iso_element_shape, connectivity, node_coords)
 
-        self.allowed_material_data_list = [('ElasticIsotropic', 'PlasticKinematicHardening', 'ViscoElasticMaxwell'),
-                                           ('ThermalIsotropic',),
-                                           ('MechanicalThermalExpansion',)]
-        self.allowed_material_number = len(self.allowed_material_data_list)
+        self.allowed_material_data_list = [('ThermalIsotropic',)]
+        self.allowed_material_number = 1
 
         self.dof = dof
         self.materials = materials
         self.section = section
         self.material_data_list = material_data_list
         self.check_materials()
         self.timer = timer
 
-        self.dof_names = ['u1', 'u2', 'T']
+        self.dof_names = ['T']
+        self.ntens = 6
+        self.ndi = 3
+        self.nshr = 3
+
         if dof.names != self.dof_names:
             error_msg = f'{dof.names} is not the supported dof of {type(self).__name__} element'
             raise NotImplementedError(error_style(error_msg))
 
         element_dof_number = len(self.dof_names) * self.iso_element_shape.nodes_number
+
         self.element_dof_number = element_dof_number
         self.element_dof_values = zeros(element_dof_number, dtype=DTYPE)
         self.element_ddof_values = zeros(element_dof_number, dtype=DTYPE)
         self.element_fint = zeros(element_dof_number, dtype=DTYPE)
         self.element_stiffness = None  # type: ignore
 
-        self.gp_b_matrices: ndarray = None  # type: ignore
-        self.gp_b_matrices_transpose: ndarray = None  # type: ignore
-        self.gp_strains: List[ndarray] = []
-        self.gp_stresses: List[ndarray] = []
-        self.gp_heat_fluxes: List[ndarray] = None  # type: ignore
-        self.gp_temperatures: List[ndarray] = None  # type: ignore
-        self.gp_ddsddts: List[ndarray] = []
-
-        self.dof_u = []
-        self.dof_T = []
-        for i in range(self.iso_element_shape.nodes_number):
-            self.dof_u += [len(self.dof_names) * i + 0, len(self.dof_names) * i + 1]
-            self.dof_T += [len(self.dof_names) * i + 2]
-
-        self.create_gp_b_matrices()
-
-    def create_gp_b_matrices(self) -> None:
-        self.gp_b_matrices = zeros(shape=(self.gp_number, 3, len(self.dof_u)), dtype=DTYPE)
-
-        for igp, (gp_shape_gradient, gp_jacobi_inv) in \
-                enumerate(zip(self.iso_element_shape.gp_shape_gradients, self.gp_jacobi_invs)):
-            gp_dhdx = dot(gp_shape_gradient.transpose(), gp_jacobi_inv)
-            for i, val in enumerate(gp_dhdx):
-                self.gp_b_matrices[igp, 0, i * 2] = val[0]
-                self.gp_b_matrices[igp, 1, i * 2 + 1] = val[1]
-                self.gp_b_matrices[igp, 2, i * 2] = val[1]
-                self.gp_b_matrices[igp, 2, i * 2 + 1] = val[0]
-
-        self.gp_b_matrices_transpose = array([gp_b_matrix.transpose() for gp_b_matrix in self.gp_b_matrices])
-
-    def update_material_state(self) -> None:
-        pass
-
-    def update_element_material_stiffness_fint(self) -> None:
+        self.gp_temperatures: list[ndarray] = None  # type: ignore
+        self.gp_heat_fluxes: list[ndarray] = None  # type: ignore
+        self.gp_ddsddts: list[ndarray] = None  # type: ignore
+
+    def update_element_material_stiffness_fint(self,
+                                               is_update_material: bool = True,
+                                               is_update_stiffness: bool = True,
+                                               is_update_fint: bool = True, ) -> None:
         element_id = self.element_id
         timer = self.timer
+        ntens = self.ntens
+        ndi = self.ndi
+        nshr = self.nshr
 
         gp_number = self.gp_number
+        gp_weight_times_jacobi_dets = self.gp_weight_times_jacobi_dets
         gp_shape_values = self.iso_element_shape.gp_shape_values
         gp_shape_gradients = self.iso_element_shape.gp_shape_gradients
-        gp_b_matrices = self.gp_b_matrices
-        gp_b_matrices_transpose = self.gp_b_matrices_transpose
-        gp_weight_times_jacobi_dets = self.gp_weight_times_jacobi_dets
 
         gp_state_variables = self.gp_state_variables
         gp_state_variables_new = self.gp_state_variables_new
 
         element_dof_values = self.element_dof_values
         element_ddof_values = self.element_ddof_values
 
-        u = element_dof_values[self.dof_u]
-        T = element_dof_values[self.dof_T]
-
-        du = element_ddof_values[self.dof_u]
-        dT = element_ddof_values[self.dof_T]
+        material_data = self.material_data_list[0]
 
-        self.element_stiffness = zeros(shape=(self.element_dof_number, self.element_dof_number), dtype=DTYPE)
-        self.element_fint = zeros(self.element_dof_number, dtype=DTYPE)
+        if is_update_stiffness:
+            self.element_stiffness = zeros(shape=(self.element_dof_number, self.element_dof_number), dtype=DTYPE)
 
-        solid_material_data = self.material_data_list[0]
-        thermal_material_data = self.material_data_list[1]
-        solid_thermal_material_data = self.material_data_list[2]
+        if is_update_fint:
+            self.element_fint = zeros(self.element_dof_number, dtype=DTYPE)
 
-        alpha = solid_thermal_material_data.tangent
-
-        gp_ddsddes = []
-        gp_strains = []
-        gp_stresses = []
+        if is_update_material:
+            self.gp_ddsddts = list()
+            self.gp_temperatures = list()
+            self.gp_heat_fluxes = list()
 
         for i in range(gp_number):
-            gp_weight_times_jacobi_det = gp_weight_times_jacobi_dets[i]
-            gp_shape_value = gp_shape_values[i]
-            gp_b_matrix_transpose = gp_b_matrices_transpose[i]
-            gp_b_matrix = gp_b_matrices[i]
-            gp_strain = dot(gp_b_matrix, u)
-            gp_dstrain = dot(gp_b_matrix, du)
-            gp_temperature = dot(gp_shape_value, T)
-            gp_dtemperature = dot(gp_shape_value, dT)
-            gp_strain += (-alpha * gp_temperature)
-            gp_dstrain += (-alpha * gp_dtemperature)
-            variable = {'strain': gp_strain, 'dstrain': gp_dstrain}
-            gp_ddsdde, gp_output = solid_material_data.get_tangent(variable=variable,
-                                                                   state_variable=gp_state_variables[i],
-                                                                   state_variable_new=gp_state_variables_new[i],
-                                                                   element_id=element_id,
-                                                                   igp=i,
-                                                                   ntens=4,
-                                                                   ndi=3,
-                                                                   nshr=1,
-                                                                   timer=timer)
-            gp_stress = gp_output['stress']
-
-            self.element_stiffness[ix_(self.dof_u, self.dof_u)] += \
-                dot(gp_b_matrix_transpose, dot(gp_ddsdde, gp_b_matrix)) * gp_weight_times_jacobi_det
-
-            dsdt = -1.0 * dot(gp_ddsdde, alpha)
-            self.element_stiffness[ix_(self.dof_u, self.dof_T)] += \
-                dot(gp_b_matrix_transpose, outer(dsdt, gp_shape_value)) * gp_weight_times_jacobi_det
-
-            self.element_fint[self.dof_u] += dot(gp_b_matrix_transpose, gp_stress) * gp_weight_times_jacobi_det
-
-            gp_ddsddes.append(gp_ddsdde)
-            gp_strains.append(gp_strain)
-            gp_stresses.append(gp_stress)
-
-        self.gp_ddsddes = gp_ddsddes
-        self.gp_strains = gp_strains
-        self.gp_stresses = gp_stresses
-
-        gp_ddsddts = []
-        gp_temperatures = []
-        gp_heat_fluxes = []
+            if is_update_material:
+                gp_weight_times_jacobi_det = gp_weight_times_jacobi_dets[i]
+                gp_shape_value = gp_shape_values[i]
+                gp_shape_gradient = gp_shape_gradients[i]
+                gp_temperature = dot(gp_shape_value, element_dof_values)
+                gp_dtemperature = dot(gp_shape_value, element_ddof_values)
+                gp_temperature_gradient = dot(gp_shape_gradient, element_dof_values)
+                gp_dtemperature_gradient = dot(gp_shape_gradient, element_ddof_values)
+
+                variable = {'temperature': gp_temperature,
+                            'dtemperature': gp_dtemperature,
+                            'temperature_gradient': gp_temperature_gradient,
+                            'dtemperature_gradient': gp_dtemperature_gradient}
+                gp_ddsddt, gp_output = material_data.get_tangent(variable=variable,
+                                                                 state_variable=gp_state_variables[i],
+                                                                 state_variable_new=gp_state_variables_new[i],
+                                                                 element_id=element_id,
+                                                                 igp=i,
+                                                                 ntens=ntens,
+                                                                 ndi=ndi,
+                                                                 nshr=nshr,
+                                                                 timer=timer)
+                gp_heat_flux = gp_output['heat_flux']
+                self.gp_ddsddts.append(gp_ddsddt)
+                self.gp_temperatures.append(gp_temperature)
+                self.gp_heat_fluxes.append(gp_heat_flux)
+            else:
+                gp_shape_gradient = gp_shape_gradients[i]
+                gp_weight_times_jacobi_det = gp_weight_times_jacobi_dets[i]
+                gp_ddsddt = self.gp_ddsddts[i]
+                gp_heat_flux = self.gp_heat_fluxes[i]
+
+            if is_update_stiffness:
+                self.element_stiffness += dot(gp_shape_gradient.transpose(), dot(gp_ddsddt, gp_shape_gradient)) * \
+                                          gp_weight_times_jacobi_det
 
-        for i in range(gp_number):
-            gp_weight_times_jacobi_det = gp_weight_times_jacobi_dets[i]
-            gp_shape_value = gp_shape_values[i]
-            gp_shape_gradient = gp_shape_gradients[i]
-            gp_temperature = dot(gp_shape_value, T)
-            gp_dtemperature = dot(gp_shape_value, dT)
-            gp_temperature_gradient = dot(gp_shape_gradient, T)
-            gp_dtemperature_gradient = dot(gp_shape_gradient, dT)
-
-            variable = {'temperature': gp_temperature,
-                        'dtemperature': gp_dtemperature,
-                        'temperature_gradient': gp_temperature_gradient,
-                        'dtemperature_gradient': gp_dtemperature_gradient}
-            gp_ddsddt, gp_output = thermal_material_data.get_tangent(variable=variable,
-                                                                     state_variable=gp_state_variables[i],
-                                                                     state_variable_new=gp_state_variables_new[i],
-                                                                     element_id=element_id,
-                                                                     igp=i,
-                                                                     ntens=4,
-                                                                     ndi=3,
-                                                                     nshr=1,
-                                                                     timer=timer)
-            gp_heat_flux = gp_output['heat_flux']
-
-            self.element_stiffness[ix_(self.dof_T, self.dof_T)] += \
-                dot(gp_shape_gradient.transpose(), dot(gp_ddsddt, gp_shape_gradient)) * gp_weight_times_jacobi_det
-
-            self.element_fint[self.dof_T] += \
-                dot(gp_shape_gradient.transpose(), gp_heat_flux) * gp_weight_times_jacobi_det
-
-            gp_ddsddts.append(gp_ddsddt)
-            gp_temperatures.append(gp_temperature)
-            gp_heat_fluxes.append(gp_heat_flux)
-
-        self.gp_ddsddts = gp_ddsddts
-        self.gp_temperatures = gp_temperatures
-        self.gp_heat_fluxes = gp_heat_fluxes
+            if is_update_fint:
+                self.element_fint += dot(gp_shape_gradient.transpose(), gp_heat_flux) * gp_weight_times_jacobi_det
 
-    def update_element_stiffness(self) -> None:
-        self.element_stiffness = zeros(shape=(self.element_dof_number, self.element_dof_number), dtype=DTYPE)
-
-        gp_weight_times_jacobi_dets = self.gp_weight_times_jacobi_dets
-        gp_shape_gradients = self.iso_element_shape.gp_shape_gradients
-        gp_b_matrices = self.gp_b_matrices
-        gp_b_matrices_transpose = self.gp_b_matrices_transpose
-        gp_number = self.gp_number
-        gp_ddsddes = self.gp_ddsddes
-        gp_ddsddts = self.gp_ddsddts
-
-        for i in range(gp_number):
-            self.element_stiffness[ix_(self.dof_u, self.dof_u)] += \
-                dot(gp_b_matrices_transpose[i], dot(gp_ddsddes[i], gp_b_matrices[i])) * gp_weight_times_jacobi_dets[i]
-
-            self.element_stiffness[ix_(self.dof_T, self.dof_T)] += \
-                dot(gp_shape_gradients[i].transpose(), dot(gp_ddsddts[i], gp_shape_gradients[i])) * \
-                gp_weight_times_jacobi_dets[i]
-
-    def update_element_fint(self) -> None:
-        gp_weight_times_jacobi_dets = self.gp_weight_times_jacobi_dets
-        gp_shape_gradients = self.iso_element_shape.gp_shape_gradients
-        gp_b_matrices_transpose = self.gp_b_matrices_transpose
-        gp_number = self.gp_number
-        gp_stresses = self.gp_stresses
+    def update_element_field_variables(self) -> None:
+        gp_temperatures = self.gp_temperatures
         gp_heat_fluxes = self.gp_heat_fluxes
 
-        self.element_fint = zeros(self.element_dof_number, dtype=DTYPE)
-        for i in range(gp_number):
-            self.element_fint[self.dof_u] += dot(gp_b_matrices_transpose[i], gp_stresses[i]) * \
-                                             gp_weight_times_jacobi_dets[i]
+        average_temperatures = average(gp_temperatures, axis=0)
+        average_heat_fluxes = average(gp_heat_fluxes, axis=0)
 
-            self.element_fint[self.dof_T] += dot(gp_shape_gradients[i].transpose(), gp_heat_fluxes[i]) * \
-                                             gp_weight_times_jacobi_dets[i]
+        self.gp_field_variables['temperature'] = array(gp_temperatures, dtype=DTYPE)
+        self.gp_field_variables['heat_flux'] = array(gp_heat_fluxes, dtype=DTYPE)
 
-    def update_element_field_variables(self) -> None:
-        gp_stresses = self.gp_stresses
-        gp_strains = self.gp_strains
+        self.element_average_field_variables['T'] = average_temperatures
+        if len(average_heat_fluxes) >= 1:
+            self.element_average_field_variables['HFL1'] = average_heat_fluxes[0]
+        if len(average_heat_fluxes) >= 2:
+            self.element_average_field_variables['HFL2'] = average_heat_fluxes[1]
+        if len(average_heat_fluxes) >= 3:
+            self.element_average_field_variables['HFL3'] = average_heat_fluxes[2]
 
-        average_strain = average(gp_strains, axis=0)
-        average_stress = average(gp_stresses, axis=0)
 
-        self.gp_field_variables['strain'] = array(gp_strains, dtype=DTYPE)
-        self.gp_field_variables['stress'] = array(gp_stresses, dtype=DTYPE)
-
-        self.element_average_field_variables['E11'] = average_strain[0]
-        self.element_average_field_variables['E22'] = average_strain[1]
-        self.element_average_field_variables['E12'] = average_strain[2]
-        self.element_average_field_variables['S11'] = average_stress[0]
-        self.element_average_field_variables['S22'] = average_stress[1]
-        self.element_average_field_variables['S12'] = average_stress[2]
+if __name__ == "__main__":
+    from pyfem.utils.visualization import print_slots_dict
 
+    print_slots_dict(Thermal.__slots_dict__)
 
-if __name__ == "__main__":
     from pyfem.Job import Job
 
-    job = Job(r'F:\Github\pyfem\examples\1element\hex8\Job-1.toml')
+    job = Job(r'F:\Github\pyfem\examples\thermal\1element\hex8\Job-1.toml')
 
-    job.assembly.element_data_list[0].show()
+    job.run()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfem-0.1.2/src/pyfem/elements/get_element_data.py` & `pyfem-0.1.3/src/pyfem/elements/get_element_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,67 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import List
+from typing import Union
 
 from numpy import ndarray
 
 from pyfem.elements.BaseElement import BaseElement
-from pyfem.elements.IsoElementShape import IsoElementShape
-from pyfem.elements.SolidPhaseFieldDamagePlaneSmallStrain import SolidPhaseFieldDamagePlaneSmallStrain
-from pyfem.elements.SolidPlaneSmallStrain import SolidPlaneSmallStrain
-from pyfem.elements.SolidThermalPlaneSmallStrain import SolidThermalPlaneSmallStrain
-from pyfem.elements.SolidVolumeSmallStrain import SolidVolumeSmallStrain
+from pyfem.elements.SolidPhaseDamageSmallStrain import SolidPhaseDamageSmallStrain
+from pyfem.elements.SolidSmallStrain import SolidSmallStrain
+from pyfem.elements.SolidThermalSmallStrain import SolidThermalSmallStrain
 from pyfem.elements.Thermal import Thermal
 from pyfem.fem.Timer import Timer
 from pyfem.io.Dof import Dof
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
+from pyfem.isoelements.IsoElementShape import IsoElementShape
+from pyfem.materials.get_material_data import MaterialData
 from pyfem.utils.colors import error_style
-from pyfem.utils.data_types import MaterialData
+
+ElementData = Union[
+    BaseElement, SolidSmallStrain, SolidThermalSmallStrain, SolidPhaseDamageSmallStrain, Thermal]
 
 element_data_dict = {
-    'SolidPlaneStrainSmallStrain': SolidPlaneSmallStrain,
-    'SolidPlaneStressSmallStrain': SolidPlaneSmallStrain,
-    'SolidVolumeSmallStrain': SolidVolumeSmallStrain,
-    'SolidThermalPlaneStrainSmallStrain': SolidThermalPlaneSmallStrain,
-    'SolidThermalPlaneStressSmallStrain': SolidThermalPlaneSmallStrain,
-    'SolidPhaseFieldDamagePlaneStrainSmallStrain': SolidPhaseFieldDamagePlaneSmallStrain,
-    'SolidPhaseFieldDamagePlaneStressSmallStrain': SolidPhaseFieldDamagePlaneSmallStrain,
+    'SolidSmallStrain': SolidSmallStrain,
+    'SolidThermalSmallStrain': SolidThermalSmallStrain,
+    'SolidPhaseDamageSmallStrain': SolidPhaseDamageSmallStrain,
     'Thermal': Thermal,
 }
 
 
 def get_element_data(element_id: int,
                      iso_element_shape: IsoElementShape,
                      connectivity: ndarray,
                      node_coords: ndarray,
                      dof: Dof,
-                     materials: List[Material],
+                     materials: list[Material],
                      section: Section,
-                     material_data_list: List[MaterialData],
-                     timer: Timer) -> BaseElement:
-    class_name = f'{section.category}{section.type}{section.option}'.strip().replace(' ', '')
+                     material_data_list: list[MaterialData],
+                     timer: Timer) -> ElementData:
+    """
+    工厂函数，用于根据材料、截面和单元属性生产不同的单元对象。
+
+    Args:
+        element_id(int): 单元编号
+        iso_element_shape(IsoElementShape): 等参元对象
+        connectivity(ndarray): 单元节点序列
+        node_coords(ndarray): 单元坐标列表
+        dof(Dof): 自由度属性
+        materials(list[Material]): 材料属性列表
+        section(Section): 截面属性
+        material_data_list(list[MaterialData]): 材料数据对象列表
+        timer(Timer): 计时器对象
+
+    :return: 单元对象
+    :rtype: ElementData
+    """
+
+    class_name = f'{section.category}{section.option}'.strip().replace(' ', '')
 
     if class_name in element_data_dict:
         return element_data_dict[class_name](element_id=element_id,
                                              iso_element_shape=iso_element_shape,
                                              connectivity=connectivity,
                                              node_coords=node_coords,
                                              dof=dof,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfem-0.1.2/src/pyfem/elements/get_iso_element_type.py` & `pyfem-0.1.3/src/pyfem/isoelements/get_iso_element_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,30 @@
+# -*- coding: utf-8 -*-
+"""
+
+"""
 from numpy import ndarray
 
 from pyfem.utils.colors import error_style
 
 
 def get_iso_element_type(node_coords: ndarray, dimension: int = -1) -> str:
+    """
+    根据单元节点坐标数组和单元空间维度返回默认的等参元名称。
+
+    Args:
+        node_coords(ndarray): 单元节点坐标数组
+        dimension(int): 单元空间维度
+
+    :return: 等参元名称
+    :rtype: str
+    """
+
     element_node_number = node_coords.shape[0]
+
     if dimension == -1:
         dimension = node_coords.shape[1]
 
     if dimension == 1:
         if element_node_number == 2:
             return 'line2'
         elif element_node_number == 3:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfem-0.1.2/src/pyfem/fem/Timer.py` & `pyfem-0.1.3/src/pyfem/fem/Timer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,57 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import List, Tuple
-
 from pyfem.utils.visualization import object_slots_to_string_ndarray
 
 
 class Timer:
     """
     计时器类，用于存储求解过程中的时间信息。
+
+    :ivar total_time: 总时间
+    :vartype total_time: float
+
+    :ivar time0: 上一个载荷步的时间
+    :vartype time0: float
+
+    :ivar time1: 当前载荷步的时间
+    :vartype time1: float
+
+    :ivar dtime: 当前载荷步的时间增量
+    :vartype dtime: float
+
+    :ivar increment: 当前增量步
+    :vartype increment: int
+
+    :ivar frame_ids: 帧列表
+    :vartype frame_ids: list[int]
     """
-    __slots__: Tuple = ('total_time',
-                        'time0',
-                        'time1',
-                        'dtime',
-                        'increment',
-                        'frame_ids')
 
-    TOL_TIME: float = 1e-6
+    __slots_dict__: dict = {
+        'total_time': ('float', '总时间'),
+        'time0': ('float', '上一个载荷步的时间'),
+        'time1': ('float', '当前载荷步的时间'),
+        'dtime': ('float', '当前载荷步的时间增量'),
+        'increment': ('int', '当前增量步'),
+        'frame_ids': ('list[int]', '帧列表')
+    }
+
+    __slots__: list = [slot for slot in __slots_dict__.keys()]
+
+    TOL_TIME: float = 1e-9
 
     def __init__(self) -> None:
         self.total_time: float = 1.0
         self.time0: float = 0.0
         self.time1: float = 0.0
         self.dtime: float = 1.0
         self.increment: int = 0
-        self.frame_ids: List[int] = []
+        self.frame_ids: list[int] = []
 
     def to_string(self, level: int = 1) -> str:
         return object_slots_to_string_ndarray(self, level)
 
     def show(self) -> None:
         print(self.to_string())
 
@@ -38,9 +59,13 @@
         if self.time1 * (1.0 + self.TOL_TIME) >= self.total_time:
             return True
         else:
             return False
 
 
 if __name__ == "__main__":
+    from pyfem.utils.visualization import print_slots_dict
+
+    print_slots_dict(Timer.__slots_dict__)
+
     timer = Timer()
     timer.show()
```

### Comparing `pyfem-0.1.2/src/pyfem/io/BaseIO.py` & `pyfem-0.1.3/src/pyfem/io/BaseIO.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import Dict, Tuple
+from typing import Dict, List
 
 from pyfem.utils.colors import error_style
 from pyfem.utils.visualization import object_slots_to_string
 
 
 class BaseIO:
-    __slots__: Tuple = ()
+    """
+    属性配置基类。
+
+    当 self.is_read_only = True 时：BaseIO子类的所有属性在第一次被赋予非None值后变为只读状态，不能被修改或删除。
+
+    """
+    __slots__: List = []
 
     is_read_only: bool = True
 
     def __init__(self) -> None:
         pass
 
     def __setattr__(self, key, value):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfem-0.1.2/src/pyfem/io/Material.py` & `pyfem-0.1.3/src/pyfem/io/Material.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,54 +1,65 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import List, Tuple, Dict
-
 from pyfem.io.BaseIO import BaseIO
 from pyfem.utils.colors import error_style
 
 
 class Material(BaseIO):
     """
-    Material类用于存储配置文件中定义的材料属性。
+    定义材料属性。
+
+    :ivar name: 材料名称
+    :vartype name: str
+
+    :ivar category: 材料类别
+    :vartype category: str
 
-    当 self.is_read_only = True 时：
-        1. Material 类的所有属性在首次被赋非None值后不能再被修改和删除，
-        2. 此时许可的属性关键字存储在self.slots中。
+    :ivar type: 材料类型
+    :vartype type: str
+
+    :ivar data: 数据列表
+    :vartype data: list[float]
     """
-    __slots__: Tuple = ('name',
-                        'category',
-                        'type',
-                        'data')
 
-    allowed_categories_types: Dict = {
+    __slots_dict__: dict = {
+        'name': ('str', '材料名称'),
+        'category': ('str', '材料类别'),
+        'type': ('str', '材料类型'),
+        'data': ('list[float]', '数据列表')
+    }
+
+    __slots__: list = [slot for slot in __slots_dict__.keys()]
+
+    allowed_categories_types: dict = {
         None: [None],
         'Elastic': ['Isotropic'],
         'Plastic': ['KinematicHardening'],
         'ViscoElastic': ['Maxwell'],
         'Thermal': ['Isotropic'],
         'PhaseField': ['Damage'],
         'MechanicalThermal': ['Expansion']
     }
 
-    allowed_keys_values: Dict = {
+    allowed_keys_values: dict = {
         'category': allowed_categories_types.keys(),
         'type': []
     }
 
     for types in allowed_categories_types.values():
         allowed_keys_values['type'] += types
 
     def __init__(self) -> None:
         super().__init__()
         self.name: str = None  # type: ignore
         self.category: str = None  # type: ignore
         self.type: str = None  # type: ignore
-        self.data: List[float] = None  # type: ignore
+        self.data: list[float] = None  # type: ignore
 
     def __setattr__(self, key, value) -> None:
         if self.is_read_only:
             if key not in self.__slots__:
                 error_msg = f'{key} is not an allowable attribute keyword of {type(self).__name__}'
                 raise AttributeError(error_style(error_msg))
 
@@ -65,9 +76,13 @@
 
                 super().__setattr__(key, value)
         else:
             super().__setattr__(key, value)
 
 
 if __name__ == "__main__":
+    from pyfem.utils.visualization import print_slots_dict
+
+    print_slots_dict(Material.__slots_dict__)
+
     material = Material()
     material.show()
```

### Comparing `pyfem-0.1.2/src/pyfem/io/arguments.py` & `pyfem-0.1.3/src/pyfem/io/arguments.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 import sys
 from argparse import ArgumentParser, Namespace, SUPPRESS
 
+from pyfem import __version__
+
 
 def get_arguments() -> Namespace:
     logo = r"""
                      ____             
         ____  __  __/ __/__  ____ ___ 
        / __ \/ / / / /_/ _ \/ __ `__ \
       / /_/ / /_/ / __/  __/ / / / / /
@@ -35,15 +37,15 @@
 
     # 添加帮助选项
     parser.add_argument('-h', '--help', action='help', default=SUPPRESS,
                         help='Show this help message and exit.')
 
     # 添加版本选项
     parser.add_argument('-v', '--version', action='version', help='Show program\'s version number and exit.',
-                        version='pyfem 0.1.2')
+                        version=f'pyfem {__version__}')
 
     # 解析命令行参数
     args = parser.parse_args()
 
     # 如果未指定程序输入文件，则打印帮助并退出
     if not args.i:
         print('--------------------------------------')
```

### Comparing `pyfem-0.1.2/src/pyfem/io/write_vtk.py` & `pyfem-0.1.3/src/pyfem/io/write_vtk.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 from xml.etree.ElementTree import ElementTree, Element, SubElement
 
 from pyfem.assembly.Assembly import Assembly
-from pyfem.utils.wrappers import show_running_time
 
 
-@show_running_time
-def write_vtk(assembly: Assembly):
+def write_vtk(assembly: Assembly) -> None:
+    """
+    将计算结果过写入vtk文件。
+    """
     props = assembly.props
     timer = assembly.timer
     dimension = props.mesh_data.dimension
 
     root = Element("VTKFile", {
         "type": "UnstructuredGrid",
         "version": "0.1",
@@ -134,15 +135,18 @@
     job_name = props.input_file.stem
 
     output_file = props.work_path.joinpath(f'{job_name}-{timer.increment}.vtu')
 
     tree.write(output_file, xml_declaration=True, encoding='utf-8')
 
 
-def write_pvd(assembly: Assembly):
+def write_pvd(assembly: Assembly) -> None:
+    """
+    将多个vtk文件信息写入pvd文件。
+    """
     timer = assembly.timer
     job_name = assembly.props.input_file.stem
     output_file = assembly.props.work_path.joinpath(f'{job_name}.pvd')
 
     with open(output_file, 'w') as f:
         f.write("<VTKFile byte_order='LittleEndian' type='Collection' version='0.1'>\n")
         f.write("<Collection>\n")
```

### Comparing `pyfem-0.1.2/src/pyfem/materials/ElasticIsotropic.py` & `pyfem-0.1.3/src/pyfem/materials/ElasticIsotropic.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,40 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import Tuple, Dict
-
 from numpy import array, outer, diag, ndarray, dot
 
 from pyfem.fem.Timer import Timer
 from pyfem.fem.constants import DTYPE
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.utils.colors import error_style
 
 
 class ElasticIsotropic(BaseMaterial):
-    __slots__ = BaseMaterial.__slots__ + ('E', 'nu')
+    """
+    各项同性弹性材料。
+
+    支持的截面属性：('Volume', 'PlaneStress', 'PlaneStrain')
+
+    :ivar E: Young's modulus E
+    :vartype E: float
+
+    :ivar nu: Poisson's ratio nu
+    :vartype nu: float
+    """
+
+    __slots_dict__: dict = {
+        'E': ('float', 'Young\'s modulus E'),
+        'nu': ('float', 'Poisson\'s ratio nu'),
+    }
+
+    __slots__ = BaseMaterial.__slots__ + [slot for slot in __slots_dict__.keys()]
 
     def __init__(self, material: Material, dimension: int, section: Section) -> None:
         super().__init__(material, dimension, section)
         self.allowed_section_types = ('Volume', 'PlaneStress', 'PlaneStrain')
 
         self.data_keys = ['Young\'s modulus E', 'Poisson\'s ratio nu']
 
@@ -36,31 +51,31 @@
 
     def create_tangent(self):
         if self.section.type in self.allowed_section_types:
             self.tangent = get_stiffness_from_young_poisson(self.dimension, self.E, self.nu, self.section.type)
         else:
             raise NotImplementedError(error_style(self.get_section_type_error_msg()))
 
-    def get_tangent(self, variable: Dict[str, ndarray],
-                    state_variable: Dict[str, ndarray],
-                    state_variable_new: Dict[str, ndarray],
+    def get_tangent(self, variable: dict[str, ndarray],
+                    state_variable: dict[str, ndarray],
+                    state_variable_new: dict[str, ndarray],
                     element_id: int,
                     igp: int,
                     ntens: int,
                     ndi: int,
                     nshr: int,
-                    timer: Timer) -> Tuple[ndarray, Dict[str, ndarray]]:
+                    timer: Timer) -> tuple[ndarray, dict[str, ndarray]]:
         strain = variable['strain']
         dstrain = variable['dstrain']
         stress = dot(self.tangent, strain + dstrain)
         output = {'stress': stress}
         return self.tangent, output
 
 
-def get_lame_from_young_poisson(young: float, poisson: float, plane: str) -> Tuple[float, float]:
+def get_lame_from_young_poisson(young: float, poisson: float, plane: str) -> tuple[float, float]:
     r"""
     Compute Lamé parameters from Young's modulus and Poisson's ratio.
 
     The relationship between Lamé parameters and Young's modulus, Poisson's
     ratio (see [1],[2]):
 
     .. math::
@@ -173,38 +188,42 @@
     Compute bulk modulus corresponding to Young's modulus and Poisson's ratio.
     """
     lam, mu = get_lame_from_young_poisson(young, poisson, plane)
 
     return get_bulk_from_lame(lam, mu)
 
 
-def get_lame_from_stiffness(stiffness: ndarray, plane: str) -> Tuple[float, float]:
+def get_lame_from_stiffness(stiffness: ndarray, plane: str) -> tuple[float, float]:
     """
     Compute Lamé parameters from an isotropic stiffness tensor.
     """
     lam = float(stiffness[..., 0, 1])
     mu = float(stiffness[..., -1, -1])
     if plane == 'PlaneStress':
         lam = - 2.0 * mu * lam / (lam - 2.0 * mu)
 
     return lam, mu
 
 
-def get_young_poisson_from_stiffness(stiffness: ndarray, plane: str) -> Tuple[float, float]:
+def get_young_poisson_from_stiffness(stiffness: ndarray, plane: str) -> tuple[float, float]:
     """
     Compute Young's modulus and Poisson's ratio from an isotropic stiffness
     tensor.
     """
     lam, mu = get_lame_from_stiffness(stiffness, plane)
     young = (3 * lam * mu + 2 * mu ** 2) / (lam + mu)
     poisson = lam / (2 * lam + 2 * mu)
 
     return young, poisson
 
 
 if __name__ == "__main__":
+    from pyfem.utils.visualization import print_slots_dict
+
+    print_slots_dict(ElasticIsotropic.__slots_dict__)
+
     from pyfem.io.Properties import Properties
 
     props = Properties()
     props.read_file(r'..\..\..\examples\mechanical\plane\Job-1.toml')
     material_data = ElasticIsotropic(props.materials[1], 3, props.sections[0])
     material_data.show()
```

### Comparing `pyfem-0.1.2/src/pyfem/materials/MechanicalThermalExpansion.py` & `pyfem-0.1.3/src/pyfem/materials/MechanicalThermalExpansion.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,35 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import Tuple, Dict
-
 from numpy import ones, ndarray
 
 from pyfem.fem.Timer import Timer
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.utils.colors import error_style
 
 
 class MechanicalThermalExpansion(BaseMaterial):
-    __slots__ = BaseMaterial.__slots__ + ('alpha',)
+    """
+    热膨胀材料。
+
+    支持的截面属性：('Volume', 'PlaneStress', 'PlaneStrain')
+
+    :ivar alpha: Coefficient of thermal expansion alpha
+    :vartype alpha: float
+    """
+
+    __slots_dict__: dict = {
+        'alpha': ('float', 'Coefficient of thermal expansion alpha')
+    }
+
+    __slots__ = BaseMaterial.__slots__ + [slot for slot in __slots_dict__.keys()]
 
     def __init__(self, material: Material, dimension: int, section: Section) -> None:
         super().__init__(material, dimension, section)
         self.allowed_section_types = ('Volume', 'PlaneStress', 'PlaneStrain')
 
         self.data_keys = ['Coefficient of thermal expansion alpha']
 
@@ -40,29 +51,33 @@
             elif self.dimension == 3:
                 self.tangent = ones(6) * self.alpha
                 self.tangent[self.dimension:] = 0.0
         else:
             error_msg = f'{self.section.type} is not the allowed section types {self.allowed_section_types} of the material {type(self).__name__}, please check the definition of the section {self.section.name}'
             raise NotImplementedError(error_style(error_msg))
 
-    def get_tangent(self, variable: Dict[str, ndarray],
-                    state_variable: Dict[str, ndarray],
-                    state_variable_new: Dict[str, ndarray],
+    def get_tangent(self, variable: dict[str, ndarray],
+                    state_variable: dict[str, ndarray],
+                    state_variable_new: dict[str, ndarray],
                     element_id: int,
                     igp: int,
                     ntens: int,
                     ndi: int,
                     nshr: int,
-                    timer: Timer) -> Tuple[ndarray, Dict[str, ndarray]]:
+                    timer: Timer) -> tuple[ndarray, dict[str, ndarray]]:
         temperature = variable['temperature']
         thermal_strain = -self.tangent * temperature
         output = {'thermal_strain': thermal_strain}
         return self.tangent, output
 
 
 if __name__ == "__main__":
+    from pyfem.utils.visualization import print_slots_dict
+
+    print_slots_dict(MechanicalThermalExpansion.__slots_dict__)
+
     from pyfem.io.Properties import Properties
 
     props = Properties()
     props.read_file(r'..\..\..\examples\mechanical_thermal\rectangle\Job-1.toml')
     material_data = MechanicalThermalExpansion(props.materials[2], 3, props.sections[0])
     material_data.show()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfem-0.1.2/src/pyfem/materials/PhaseFieldDamage.py` & `pyfem-0.1.3/src/pyfem/materials/PhaseFieldDamage.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,15 +5,32 @@
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.utils.colors import error_style
 
 
 class PhaseFieldDamage(BaseMaterial):
-    __slots__ = BaseMaterial.__slots__ + ('gc', 'lc')
+    """
+    相场断裂材料。
+
+    支持的截面属性：('Volume', 'PlaneStress', 'PlaneStrain')
+
+    :ivar gc: surface energy to create a unit fracture surface gc
+    :vartype gc: float
+
+    :ivar lc: length scale parameter to measure the damage diffusion lc
+    :vartype lc: float
+    """
+
+    __slots_dict__: dict = {
+        'gc': ('float', 'surface energy to create a unit fracture surface gc'),
+        'lc': ('float', 'length scale parameter to measure the damage diffusion lc'),
+    }
+
+    __slots__ = BaseMaterial.__slots__ + [slot for slot in __slots_dict__.keys()]
 
     def __init__(self, material: Material, dimension: int, section: Section) -> None:
         super().__init__(material, dimension, section)
         self.allowed_section_types = ('Volume', 'PlaneStress', 'PlaneStrain')
 
         self.data_keys = ['surface energy to create a unit fracture surface gc',
                           'length scale parameter to measure the damage diffusion lc']
@@ -27,13 +44,17 @@
         self.gc: float = self.data_dict['surface energy to create a unit fracture surface gc']
         self.lc: float = self.data_dict['length scale parameter to measure the damage diffusion lc']
 
         self.create_tangent()
 
 
 if __name__ == "__main__":
+    from pyfem.utils.visualization import print_slots_dict
+
+    print_slots_dict(PhaseFieldDamage.__slots_dict__)
+
     from pyfem.io.Properties import Properties
 
     props = Properties()
     props.read_file(r'..\..\..\examples\mechanical_phase\rectangle\Job-1.toml')
     material_data = PhaseFieldDamage(props.materials[1], 3, props.sections[0])
     material_data.show()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfem-0.1.2/src/pyfem/materials/PlasticKinematicHardening.py` & `pyfem-0.1.3/src/pyfem/materials/PlasticKinematicHardening.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,75 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 from copy import deepcopy
-from typing import Dict, Tuple
 
 from numpy import zeros, ndarray, dot, sqrt, outer, insert, delete
 
 from pyfem.fem.Timer import Timer
 from pyfem.fem.constants import DTYPE
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.materials.ElasticIsotropic import get_stiffness_from_young_poisson
 from pyfem.utils.colors import error_style
 
 
 class PlasticKinematicHardening(BaseMaterial):
-    __slots__ = BaseMaterial.__slots__ + ('E',
-                                          'nu',
-                                          'yield_stress',
-                                          'hard',
-                                          'EBULK3',
-                                          'EG2',
-                                          'EG',
-                                          'EG3',
-                                          'ELAM',
-                                          'tolerance')
+    """
+    随动强化塑性材料。
+
+    支持的截面属性：('Volume', 'PlaneStress', 'PlaneStrain')
+
+    :ivar E: Young's modulus E
+    :vartype E: float
+
+    :ivar nu: Poisson's ratio nu
+    :vartype nu: float
+
+    :ivar yield_stress: Yield stress
+    :vartype yield_stress: float
+
+    :ivar hard: Hardening coefficient
+    :vartype hard: float
+
+    :ivar EBULK3: 3倍体积模量
+    :vartype EBULK3: float
+
+    :ivar EG: 剪切模量
+    :vartype EG: float
+
+    :ivar EG2: 2倍剪切模量
+    :vartype EG2: float
+
+    :ivar EG3: 3倍剪切模量
+    :vartype EG3: float
+
+    :ivar ELAM: 拉梅常数
+    :vartype ELAM: float
+
+    :ivar tolerance: 判断屈服的误差容限
+    :vartype tolerance: float
+    """
+
+    __slots_dict__: dict = {
+        'E': ('float', 'Young\'s modulus E'),
+        'nu': ('float', 'Poisson\'s ratio nu'),
+        'yield_stress': ('float', 'Yield stress'),
+        'hard': ('float', 'Hardening coefficient'),
+        'EBULK3': ('float', '3倍体积模量'),
+        'EG': ('float', '剪切模量'),
+        'EG2': ('float', '2倍剪切模量'),
+        'EG3': ('float', '3倍剪切模量'),
+        'ELAM': ('float', '拉梅常数'),
+        'tolerance': ('float', '判断屈服的误差容限'),
+    }
+
+    __slots__ = BaseMaterial.__slots__ + [slot for slot in __slots_dict__.keys()]
 
     def __init__(self, material: Material, dimension: int, section: Section) -> None:
         super().__init__(material, dimension, section)
         self.allowed_section_types = ('Volume', 'PlaneStress', 'PlaneStrain')
 
         self.data_keys = ['Young\'s modulus E', 'Poisson\'s ratio nu', 'Yield stress', 'Hardening coefficient']
 
@@ -56,23 +95,23 @@
 
     def create_tangent(self):
         if self.section.type in self.allowed_section_types:
             self.tangent = get_stiffness_from_young_poisson(self.dimension, self.E, self.nu, self.section.type)
         else:
             raise NotImplementedError(error_style(self.get_section_type_error_msg()))
 
-    def get_tangent(self, variable: Dict[str, ndarray],
-                    state_variable: Dict[str, ndarray],
-                    state_variable_new: Dict[str, ndarray],
+    def get_tangent(self, variable: dict[str, ndarray],
+                    state_variable: dict[str, ndarray],
+                    state_variable_new: dict[str, ndarray],
                     element_id: int,
                     igp: int,
                     ntens: int,
                     ndi: int,
                     nshr: int,
-                    timer: Timer) -> Tuple[ndarray, Dict[str, ndarray]]:
+                    timer: Timer) -> tuple[ndarray, dict[str, ndarray]]:
 
         if state_variable == {}:
             state_variable['elastic_strain'] = zeros(ntens, dtype=DTYPE)
             state_variable['plastic_strain'] = zeros(ntens, dtype=DTYPE)
             state_variable['back_stress'] = zeros(ntens, dtype=DTYPE)
             state_variable['stress'] = zeros(ntens, dtype=DTYPE)
 
@@ -186,13 +225,17 @@
         smises = sqrt(0.5 * smises)
         return float(smises)
     else:
         raise NotImplementedError(error_style(f'unsupported stress dimension {len(s)}'))
 
 
 if __name__ == "__main__":
+    from pyfem.utils.visualization import print_slots_dict
+
+    print_slots_dict(PlasticKinematicHardening.__slots_dict__)
+
     from pyfem.io.Properties import Properties
 
     props = Properties()
     props.read_file(r'..\..\..\examples\mechanical\plane\Job-1.toml')
     material_data = PlasticKinematicHardening(props.materials[0], 3, props.sections[0])
     material_data.show()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfem-0.1.2/src/pyfem/materials/ThermalIsotropic.py` & `pyfem-0.1.3/src/pyfem/materials/ThermalIsotropic.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,39 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import Tuple, Dict
-
 from numpy import eye, ndarray, dot
 
 from pyfem.fem.Timer import Timer
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.utils.colors import error_style
 
 
 class ThermalIsotropic(BaseMaterial):
-    __slots__ = BaseMaterial.__slots__ + ('k', 'cp')
+    """
+    各项同性热传导材料。
+
+    支持的截面属性：('', 'Volume', 'PlaneStress', 'PlaneStrain')
+
+    :ivar k: Conductivity k
+    :vartype k: float
+
+    :ivar cp: Capacity cp
+    :vartype cp: float
+    """
+
+    __slots_dict__: dict = {
+        'k': ('float', 'Conductivity k'),
+        'cp': ('float', 'Capacity cp'),
+    }
+
+    __slots__ = BaseMaterial.__slots__ + [slot for slot in __slots_dict__.keys()]
 
     def __init__(self, material: Material, dimension: int, section: Section) -> None:
         super().__init__(material, dimension, section)
         self.allowed_section_types = ('', 'Volume', 'PlaneStress', 'PlaneStrain')
 
         self.data_keys = ['Conductivity k', 'Capacity cp']
 
@@ -35,29 +50,33 @@
 
     def create_tangent(self):
         if self.section.type in self.allowed_section_types:
             self.tangent = eye(self.dimension) * self.k
         else:
             raise NotImplementedError(error_style(self.get_section_type_error_msg()))
 
-    def get_tangent(self, variable: Dict[str, ndarray],
-                    state_variable: Dict[str, ndarray],
-                    state_variable_new: Dict[str, ndarray],
+    def get_tangent(self, variable: dict[str, ndarray],
+                    state_variable: dict[str, ndarray],
+                    state_variable_new: dict[str, ndarray],
                     element_id: int,
                     igp: int,
                     ntens: int,
                     ndi: int,
                     nshr: int,
-                    timer: Timer) -> Tuple[ndarray, Dict[str, ndarray]]:
+                    timer: Timer) -> tuple[ndarray, dict[str, ndarray]]:
         temperature_gradient = variable['temperature_gradient']
         heat_flux = dot(-self.tangent, temperature_gradient)
         output = {'heat_flux': heat_flux}
         return self.tangent, output
 
 
 if __name__ == "__main__":
+    from pyfem.utils.visualization import print_slots_dict
+
+    print_slots_dict(ThermalIsotropic.__slots_dict__)
+
     from pyfem.io.Properties import Properties
 
     props = Properties()
     props.read_file(r'..\..\..\examples\thermal\1element\hex8\Job-1.toml')
     material_data = ThermalIsotropic(props.materials[0], 3, props.sections[0])
     material_data.show()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfem-0.1.2/src/pyfem/mesh/MeshData.py` & `pyfem-0.1.3/src/pyfem/mesh/MeshData.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,74 @@
 # -*- coding: utf-8 -*-
 """
 
 """
 from pathlib import Path
-from typing import List, Dict, Union
+from typing import Union
 
 import meshio  # type: ignore
 from numpy import ndarray, empty
 
 from pyfem.fem.constants import DTYPE
 from pyfem.utils.colors import BLUE, END
 from pyfem.utils.colors import error_style, info_style
 from pyfem.utils.wrappers import show_running_time
 
 
 class MeshData:
-    __slots__ = ('dimension',
-                 'mesh',
-                 'nodes',
-                 'elements',
-                 'bc_elements',
-                 'node_sets',
-                 'element_sets',
-                 'bc_element_sets')
+    """
+    网格数据类。
+
+    :ivar dimension: 空间维度
+    :vartype dimension: int
+
+    :ivar mesh: meshio返回的网格对象
+    :vartype mesh: meshio.Mesh
+
+    :ivar nodes: 节点数组
+    :vartype nodes: ndarray
+
+    :ivar elements: 单元数组列表
+    :vartype elements: list[ndarray]
+
+    :ivar bc_elements: 边界单元数组列表
+    :vartype bc_elements: list[ndarray]
+
+    :ivar node_sets: 节点集合字典
+    :vartype node_sets: dict[str, list[int]]
+
+    :ivar element_sets: 单元集合字典
+    :vartype element_sets: dict[str, list[int]]
+
+    :ivar bc_element_sets: 边界单元集合字典
+    :vartype bc_element_sets: dict[str, list[int]]
+    """
+
+    __slots_dict__: dict = {
+        'dimension': ('int', '空间维度'),
+        'mesh': ('meshio.Mesh', 'meshio返回的网格对象'),
+        'nodes': ('ndarray', '节点数组'),
+        'elements': ('list[ndarray]', '单元数组列表'),
+        'bc_elements': ('list[ndarray]', '边界单元数组列表'),
+        'node_sets': ('dict[str, list[int]]', '节点集合字典'),
+        'element_sets': ('dict[str, list[int]]', '单元集合字典'),
+        'bc_element_sets': ('dict[str, list[int]]', '边界单元集合字典')
+    }
+
+    __slots__: list = [slot for slot in __slots_dict__.keys()]
 
     def __init__(self) -> None:
         self.dimension: int = -1
         self.mesh: meshio.Mesh = None  # type: ignore
         self.nodes: ndarray = empty(0)
-        self.elements: List[ndarray] = []
-        self.bc_elements: List[ndarray] = []
-        self.node_sets: Dict[str, List[int]] = {}
-        self.element_sets: Dict[str, List[int]] = {}
-        self.bc_element_sets: Dict[str, List[int]] = {}
+        self.elements: list[ndarray] = list()
+        self.bc_elements: list[ndarray] = list()
+        self.node_sets: dict[str, list[int]] = dict()
+        self.element_sets: dict[str, list[int]] = dict()
+        self.bc_element_sets: dict[str, list[int]] = dict()
 
     def show(self) -> None:
         print(self.to_string(0))
 
     def to_string(self, level: int = 1) -> str:
         msg = BLUE + self.__str__() + END + '\n'
         space = '   ' * level
@@ -133,20 +165,22 @@
         for key in self.node_sets:
             self.node_sets[key] = list(set(self.node_sets[key]))
 
         # 添加用户定义的节点集合
         for point_set in self.mesh.point_sets:
             self.node_sets[point_set] = list(self.mesh.point_sets[point_set])
 
-    def add_to_node_sets(self, node_set_name: str, node_ids: List[int]) -> None:
+    def add_to_node_sets(self, node_set_name: str, node_ids: list[int]) -> None:
         if node_set_name not in self.node_sets:
             self.node_sets[node_set_name] = node_ids
         else:
             self.node_sets[node_set_name] += node_ids
 
 
 if __name__ == "__main__":
+    from pyfem.utils.visualization import print_slots_dict
+
+    print_slots_dict(MeshData.__slots_dict__)
+
     mesh_data = MeshData()
-    # mesh_data.read_file(r'F:\Github\pyfem\examples\rectangle\quad40000.msh', 'gmsh')
-    mesh_data.read_file(r'F:\Github\pyfem\examples\mechanical\rectangle_hole\rectangle_hole_quad4.inp', 'abaqus')
-    # mesh_data.read_file(r'F:\Github\pyfem\examples\quad_tria\Job-1.inp', 'abaqus')
+    mesh_data.read_file(r'..\..\..\examples\mechanical\rectangle_hole\rectangle_hole_quad4.inp', 'abaqus')
     mesh_data.show()
```

### Comparing `pyfem-0.1.2/src/pyfem/solvers/BaseSolver.py` & `pyfem-0.1.3/src/pyfem/solvers/BaseSolver.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,39 @@
 # -*- coding: utf-8 -*-
 """
 
 """
-from typing import Tuple
-
 from numpy import ndarray, empty
 
 from pyfem.assembly.Assembly import Assembly
 from pyfem.io.Solver import Solver
 from pyfem.utils.visualization import object_slots_to_string_ndarray
 
 
 class BaseSolver:
-    __slots__: Tuple = ('assembly',
-                        'solver',
-                        'dof_solution')
+    """
+    求解器基类。
+
+    :ivar assembly: 装配体对象
+    :vartype assembly: Assembly
+
+    :ivar solver: 求解器属性
+    :vartype solver: Solver
+
+    :ivar dof_solution: 求解得到自由度的值
+    :vartype dof_solution: ndarray
+    """
+
+    __slots_dict__: dict = {
+        'assembly': ('Assembly', '装配体对象'),
+        'solver': ('Solver', '求解器属性'),
+        'dof_solution': ('ndarray', '求解得到自由度的值')
+    }
+
+    __slots__: list = [slot for slot in __slots_dict__.keys()]
 
     def __init__(self) -> None:
         self.assembly: Assembly = None  # type: ignore
         self.solver: Solver = None  # type: ignore
         self.dof_solution: ndarray = empty(0)
 
     def to_string(self, level: int = 1) -> str:
@@ -31,9 +46,13 @@
         return -1
 
     def solve(self) -> int:
         return -1
 
 
 if __name__ == "__main__":
+    from pyfem.utils.visualization import print_slots_dict
+
+    print_slots_dict(BaseSolver.__slots_dict__)
+
     solver = BaseSolver()
     solver.show()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfem-0.1.2/src/pyfem/solvers/LinearSolver.py` & `pyfem-0.1.3/src/pyfem/solvers/LinearSolver.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,15 +9,26 @@
 from pyfem.fem.constants import DTYPE
 from pyfem.io.Solver import Solver
 from pyfem.io.write_vtk import write_vtk
 from pyfem.solvers.BaseSolver import BaseSolver
 
 
 class LinearSolver(BaseSolver):
-    __slots__ = BaseSolver.__slots__ + ('PENALTY',)
+    """
+    线性求解器。
+
+    :ivar PENALTY: 罚系数
+    :vartype PENALTY: float
+    """
+
+    __slots_dict__: dict = {
+        'PENALTY': ('float', '罚系数')
+    }
+
+    __slots__ = BaseSolver.__slots__ + [slot for slot in __slots_dict__.keys()]
 
     def __init__(self, assembly: Assembly, solver: Solver) -> None:
         super().__init__()
         self.assembly = assembly
         self.solver = solver
         self.dof_solution = empty(0, dtype=DTYPE)
         self.PENALTY: float = 1.0e16
@@ -47,12 +58,16 @@
         self.assembly.assembly_field_variables()
         write_vtk(self.assembly)
 
         return 0
 
 
 if __name__ == "__main__":
+    from pyfem.utils.visualization import print_slots_dict
+
+    print_slots_dict(LinearSolver.__slots_dict__)
+
     from pyfem.Job import Job
 
     job = Job(r'..\..\..\examples\mechanical\plane\Job-1.toml')
     solver = LinearSolver(job.assembly, job.props.solver)
     solver.show()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfem-0.1.2/src/pyfem/solvers/NonlinearSolver.py` & `pyfem-0.1.3/src/pyfem/solvers/NonlinearSolver.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,34 @@
 from pyfem.io.write_vtk import write_vtk, write_pvd
 from pyfem.solvers.BaseSolver import BaseSolver
 from pyfem.utils.colors import error_style
 from pyfem.utils.colors import info_style
 
 
 class NonlinearSolver(BaseSolver):
-    __slots__ = BaseSolver.__slots__ + ('PENALTY', 'FORCE_TOL', 'MAX_NITER')
+    """
+    非线性求解器。
+
+    :ivar PENALTY: 罚系数
+    :vartype PENALTY: float
+
+    :ivar FORCE_TOL: 残差容限
+    :vartype FORCE_TOL: float
+
+    :ivar MAX_NITER: 最大迭代次数
+    :vartype MAX_NITER: int
+    """
+
+    __slots_dict__: dict = {
+        'PENALTY': ('float', '罚系数'),
+        'FORCE_TOL': ('float', '残差容限'),
+        'MAX_NITER': ('int', '最大迭代次数')
+    }
+
+    __slots__ = BaseSolver.__slots__ + [slot for slot in __slots_dict__.keys()]
 
     def __init__(self, assembly: Assembly, solver: Solver) -> None:
         super().__init__()
         self.assembly = assembly
         self.solver = solver
         self.dof_solution = zeros(self.assembly.total_dof_number)
         self.PENALTY: float = 1.0e16
@@ -209,12 +228,16 @@
             print((error_style('maximum increment is reached')))
             return -1
         else:
             return 0
 
 
 if __name__ == "__main__":
+    from pyfem.utils.visualization import print_slots_dict
+
+    print_slots_dict(NonlinearSolver.__slots_dict__)
+
     from pyfem.Job import Job
 
     job = Job(r'..\..\..\examples\mechanical\plane\Job-1.toml')
     solver = NonlinearSolver(job.assembly, job.props.solver)
     solver.show()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfem-0.1.2/src/pyfem/solvers/get_solver_data.py` & `pyfem-0.1.3/src/pyfem/solvers/get_solver_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,40 @@
 # -*- coding: utf-8 -*-
 """
 
 """
+from typing import Union
+
 from pyfem.assembly.Assembly import Assembly
 from pyfem.io.Solver import Solver
 from pyfem.solvers.BaseSolver import BaseSolver
 from pyfem.solvers.LinearSolver import LinearSolver
 from pyfem.solvers.NonlinearSolver import NonlinearSolver
 from pyfem.utils.colors import error_style
 
+SolverData = Union[BaseSolver, LinearSolver, NonlinearSolver]
+
 solver_data_dict = {
     'LinearSolver': LinearSolver,
     'NonlinearSolver': NonlinearSolver
 }
 
 
-def get_solver_data(assembly: Assembly, solver: Solver) -> BaseSolver:
+def get_solver_data(assembly: Assembly, solver: Solver) -> SolverData:
+    """
+    工厂函数，用于根据求解器属性生产不同的求解器对象。
+
+    Args:
+        assembly(Assembly): 装配体对象
+        solver(Solver): 求解器属性
+
+    :return: 求解器对象
+    :rtype: SolverData
+    """
+
     class_name = f'{solver.type}'.strip().replace(' ', '')
 
     if class_name in solver_data_dict:
         return solver_data_dict[class_name](assembly=assembly,
                                             solver=solver)
     else:
         error_msg = f'{class_name} solver is not supported.\n'
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfem-0.1.2/src/pyfem/utils/IntKeyDict.py` & `pyfem-0.1.3/src/pyfem/utils/IntKeyDict.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.2/src/pyfem/utils/colors.py` & `pyfem-0.1.3/src/pyfem/utils/colors.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.2/src/pyfem/utils/logger.py` & `pyfem-0.1.3/src/pyfem/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.2/src/pyfem/utils/mechanics.py` & `pyfem-0.1.3/src/pyfem/utils/mechanics.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.2/src/pyfem/utils/visualization.py` & `pyfem-0.1.3/src/pyfem/utils/visualization.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 """
-定义一些函数用于程序的可视化。
+程序及对象的结构可视化，便于开发者查看数据结构。
 """
 from numpy import ndarray
 
 from pyfem.utils.colors import GREEN, BLUE, END
 
 
 def insert_spaces(n: int, text: str) -> str:
@@ -93,7 +93,13 @@
         return str(num) + "st"
     elif num % 10 == 2:
         return str(num) + "nd"
     elif num % 10 == 3:
         return str(num) + "rd"
     else:
         return str(num) + "th"
+
+
+def print_slots_dict(slots_dict: dict) -> None:
+    for key, item in slots_dict.items():
+        print(f'    :ivar {key}: {item[1]}')
+        print(f'    :vartype {key}: {item[0]}\n')
```

### Comparing `pyfem-0.1.2/src/pyfem/utils/wrappers.py` & `pyfem-0.1.3/src/pyfem/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.1.2/src/pyfem.egg-info/PKG-INFO` & `pyfem-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,52 @@
 Metadata-Version: 2.1
 Name: pyfem
-Version: 0.1.2
+Version: 0.1.3
 Summary: A finite element package for learning
 Home-page: https://github.com/sunwhale/pyfem
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyfem
 
-A finite element package in python.
+pyfem是一个完全基于python语言实现的极简有限元求解器。基于numpy、scipy和meshio等第三方库，主要用于有限元方法的学习、有限元算法验证和快速建立材料本构模型的程序原型。
+
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/ab5bca55d85d45d4aa4336ccae058316)](https://app.codacy.com/gh/sunwhale/pyfem/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 
-## Installation
+## Installation 安装
 
-Use the package manager [pip](https://pypi.org/project/pyfem/) to install pyfem.
+Use the package manager [pip](https://pypi.org/project/pyfem/) to install pyfem. 使用pip命令安装。
 
 ```bash
 pip install pyfem
 ```
 
-## Development
-
-### ToDo list
+## Tutorial 指南
 
-- [x] 增加Neumann边界条件，支持concentrated force，distributed和pressure定义方式
-- [ ] 增加hdf5计算结果输出格式
-- [ ] 完善帮助文档
-- [ ] 完善输入文件的校检
-- [x] 增加测试模块
-- [ ] 增加日志模块
-- [ ] 增加后台运行模式
-- [ ] 处理平面应力状态的面外应力平衡
-- [x] 增加粘弹性力学本构模型
-- [ ] 增加晶体塑性力学本构模型
-- [x] 增加温度场求解单元
-- [x] 增加温度场-位移场耦合求解单元
-- [x] 增加相场-位移场耦合求解单元
-- [ ] 增加内聚区单元
-- [ ] 增加动力学求解器
-- [ ] 建立前处理界面
+### Run in command line 在命令行运行:
 
-## Tutorial
+```bash
+pyfem --help
+```
 
-#### Run in command line:
+### Run the first example 执行第一个算例:
 
 ```bash
 pyfem -i Job-1.toml
 ```
 
-#### Job file Job-1.toml:
+#### 算例配置文件 Job-1.toml:
 
 ```toml
 title = "Job-1"
 
 [mesh]
 type = "abaqus"
 file = "hex8.inp"
@@ -106,14 +92,15 @@
 element_sets = ['Set-X1']
 value = 1.0
 
 [solver]
 type = "NonlinearSolver"
 option = "NewtonRaphson"
 total_time = 1.0
+start_time = 0.0
 max_increment = 1000000
 initial_dtime = 0.1
 max_dtime = 1.0
 min_dtime = 0.001
 
 [[materials]]
 name = "Material-1"
@@ -140,15 +127,15 @@
 
 [[outputs]]
 type = "vtk"
 field_outputs = ['S11', 'S22', 'S33', 'S12', 'S13', 'S23', 'E11', 'E22', 'E33', 'E12', 'E13', 'E23']
 on_screen = false
 ```
 
-#### abaqus geometry file hex8.inp:
+#### 采用abaqus格式的网格文件 hex8.inp:
 
 ```abaqus
 *Heading
 *Preprint, echo=NO, model=NO, history=NO, contact=NO
 **
 ** PARTS
 **
@@ -201,10 +188,34 @@
 **  
 *Instance, name=Part-1-1, part=Part-1
 *End Instance
 **  
 *End Assembly
 ```
 
+### Documents 帮助文档
+[https://pyfem-doc.readthedocs.io/](https://pyfem-doc.readthedocs.io/)
+
+## Development
+
+### ToDo list
+
+- [x] 增加Neumann边界条件，支持concentrated force，distributed和pressure定义方式
+- [ ] 增加hdf5计算结果输出格式
+- [ ] 完善帮助文档
+- [ ] 完善输入文件的校检
+- [x] 增加测试模块
+- [ ] 增加日志模块
+- [ ] 增加后台运行模式
+- [ ] 处理平面应力状态的面外应力平衡
+- [x] 增加粘弹性力学本构模型
+- [ ] 增加晶体塑性力学本构模型
+- [x] 增加温度场求解单元
+- [x] 增加温度场-位移场耦合求解单元
+- [x] 增加相场-位移场耦合求解单元
+- [ ] 增加内聚区单元
+- [ ] 增加动力学求解器
+- [ ] 建立前处理界面
+
 ### Bug list
 
 - [ ] 采用abaqus网格文件时，如果存在node不属于任何element则在计算时会导致全局刚度矩阵奇异。
```

### Comparing `pyfem-0.1.2/src/pyfem.egg-info/SOURCES.txt` & `pyfem-0.1.3/src/pyfem.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -20,25 +20,20 @@
 src/pyfem/bc/DirichletBC.py
 src/pyfem/bc/NeumannBCConcentrated.py
 src/pyfem/bc/NeumannBCDistributed.py
 src/pyfem/bc/NeumannBCPressure.py
 src/pyfem/bc/__init__.py
 src/pyfem/bc/get_bc_data.py
 src/pyfem/elements/BaseElement.py
-src/pyfem/elements/IsoElementDiagram.py
-src/pyfem/elements/IsoElementShape.py
-src/pyfem/elements/SolidPhaseFieldDamagePlaneSmallStrain.py
-src/pyfem/elements/SolidPlaneSmallStrain.py
-src/pyfem/elements/SolidThermalPlaneSmallStrain.py
-src/pyfem/elements/SolidVolumeSmallStrain.py
+src/pyfem/elements/SolidPhaseDamageSmallStrain.py
+src/pyfem/elements/SolidSmallStrain.py
+src/pyfem/elements/SolidThermalSmallStrain.py
 src/pyfem/elements/Thermal.py
 src/pyfem/elements/__init__.py
-src/pyfem/elements/derive.py
 src/pyfem/elements/get_element_data.py
-src/pyfem/elements/get_iso_element_type.py
 src/pyfem/fem/Timer.py
 src/pyfem/fem/__init__.py
 src/pyfem/fem/constants.py
 src/pyfem/io/Amplitude.py
 src/pyfem/io/BC.py
 src/pyfem/io/BaseIO.py
 src/pyfem/io/Dof.py
@@ -47,14 +42,20 @@
 src/pyfem/io/Output.py
 src/pyfem/io/Properties.py
 src/pyfem/io/Section.py
 src/pyfem/io/Solver.py
 src/pyfem/io/__init__.py
 src/pyfem/io/arguments.py
 src/pyfem/io/write_vtk.py
+src/pyfem/isoelements/IsoElementDiagram.py
+src/pyfem/isoelements/IsoElementShape.py
+src/pyfem/isoelements/__init__.py
+src/pyfem/isoelements/derive_shape_functions.py
+src/pyfem/isoelements/get_iso_element_type.py
+src/pyfem/isoelements/shape_functions.py
 src/pyfem/materials/BaseMaterial.py
 src/pyfem/materials/ElasticIsotropic.py
 src/pyfem/materials/MechanicalThermalExpansion.py
 src/pyfem/materials/PhaseFieldDamage.py
 src/pyfem/materials/PlasticKinematicHardening.py
 src/pyfem/materials/ThermalIsotropic.py
 src/pyfem/materials/ViscoElasticMaxwell.py
@@ -67,13 +68,12 @@
 src/pyfem/solvers/LinearSolver.py
 src/pyfem/solvers/NonlinearSolver.py
 src/pyfem/solvers/__init__.py
 src/pyfem/solvers/get_solver_data.py
 src/pyfem/utils/IntKeyDict.py
 src/pyfem/utils/__init__.py
 src/pyfem/utils/colors.py
-src/pyfem/utils/data_types.py
 src/pyfem/utils/derive.py
 src/pyfem/utils/logger.py
 src/pyfem/utils/mechanics.py
 src/pyfem/utils/visualization.py
 src/pyfem/utils/wrappers.py
```


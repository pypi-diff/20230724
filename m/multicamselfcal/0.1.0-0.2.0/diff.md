# Comparing `tmp/multicamselfcal-0.1.0.tar.gz` & `tmp/multicamselfcal-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\multicamselfcal-0.1.0.tar", last modified: Fri Dec 11 21:46:14 2020, max compression
+gzip compressed data, was "multicamselfcal-0.2.0.tar", last modified: Mon Jul 24 14:09:13 2023, max compression
```

## Comparing `multicamselfcal-0.1.0.tar` & `multicamselfcal-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,154 @@
-drwxrwxrwx   0        0        0        0 2020-12-11 21:46:14.199397 multicamselfcal-0.1.0/
--rw-rw-rw-   0        0        0      253 2020-12-11 21:46:14.198397 multicamselfcal-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2020-12-11 21:46:14.168398 multicamselfcal-0.1.0/multicamselfcal/
--rw-rw-rw-   0        0        0        0 2020-12-11 21:44:23.000000 multicamselfcal-0.1.0/multicamselfcal/__init__.py
--rw-rw-rw-   0        0        0     1955 2020-12-11 21:44:23.000000 multicamselfcal-0.1.0/multicamselfcal/align.py
--rw-rw-rw-   0        0        0    15182 2020-12-11 21:44:23.000000 multicamselfcal-0.1.0/multicamselfcal/execute.py
--rw-rw-rw-   0        0        0     6087 2020-12-11 21:44:23.000000 multicamselfcal-0.1.0/multicamselfcal/formats.py
--rw-rw-rw-   0        0        0      684 2020-12-11 21:44:23.000000 multicamselfcal-0.1.0/multicamselfcal/visualization.py
-drwxrwxrwx   0        0        0        0 2020-12-11 21:46:14.192397 multicamselfcal-0.1.0/multicamselfcal.egg-info/
--rw-rw-rw-   0        0        0      253 2020-12-11 21:46:14.000000 multicamselfcal-0.1.0/multicamselfcal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2020-12-11 21:46:14.000000 multicamselfcal-0.1.0/multicamselfcal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-12-11 21:46:14.000000 multicamselfcal-0.1.0/multicamselfcal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2020-12-11 21:46:14.000000 multicamselfcal-0.1.0/multicamselfcal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-12-11 21:46:14.200398 multicamselfcal-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      264 2020-12-11 21:46:04.000000 multicamselfcal-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2020-12-11 21:46:14.197397 multicamselfcal-0.1.0/test/
--rw-rw-rw-   0        0        0     1659 2020-12-11 21:44:23.000000 multicamselfcal-0.1.0/test/test_align.py
--rw-rw-rw-   0        0        0      998 2020-12-11 21:44:23.000000 multicamselfcal-0.1.0/test/test_mcsc.py
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.212528 multicamselfcal-0.2.0/
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.200528 multicamselfcal-0.2.0/CalTechCal/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     3925 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/analyse_error.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1675 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/apply_distortion.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)       45 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/check_active_images.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1233 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/comp_distortion_oulu.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1134 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/comp_error_calib.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     2151 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/comp_ext_calib.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     5138 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/compute_extrinsic_init.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     2768 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/compute_extrinsic_refine.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     5289 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/export_calib_data.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1509 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/extract_parameters.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     6543 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/ginput3.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)    19148 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/go_calib_optim_iter.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     2094 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/gorad.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     2454 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/goradf.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1203 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/normalize.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      424 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/preparedata.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     8737 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/project_points2.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     4136 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/quiver.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1730 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/rigid_motion.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     4773 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/rodrigues.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     6751 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/visualize_distortions.m
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.204528 multicamselfcal-0.2.0/CommonCfgAndIO/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1807 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CommonCfgAndIO/ConvertOldConfigToNew.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)    24912 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CommonCfgAndIO/configdata.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      809 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CommonCfgAndIO/expname.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     3623 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CommonCfgAndIO/loaddata.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     6625 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CommonCfgAndIO/oldexperiments.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)    11438 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CommonCfgAndIO/read_configuration.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     4852 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CommonCfgAndIO/read_generic_configuration.m
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.204528 multicamselfcal-0.2.0/MultiCamSelfCal/
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.204528 multicamselfcal-0.2.0/MultiCamSelfCal/BlueCLocal/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1186 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/BlueCLocal/align_existing_camera_centers.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     3118 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/BlueCLocal/bluechoengg.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     2938 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/BlueCLocal/bluecrz.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     5498 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/BlueCLocal/flydra.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1358 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/BlueCLocal/humdra.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     6781 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/BlueCLocal/mamarama.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1409 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/BlueCLocal/strawlab_test.m
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.204528 multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      130 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/align3d.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1684 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/estimateLambda.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     2056 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/estimatePX.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1405 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/estsimt.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     4642 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/euclidize.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1999 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/findinl.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      796 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/findoutl.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1082 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/reprerror.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      794 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/rq.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     2052 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/selfcalib.m
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.204528 multicamselfcal-0.2.0/MultiCamSelfCal/FindingPoints/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)    10807 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/FindingPoints/getpoint.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     4601 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/FindingPoints/im2imstat.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     6237 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/FindingPoints/im2points.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      498 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/FindingPoints/mycorr2.m
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.204528 multicamselfcal-0.2.0/MultiCamSelfCal/LocalAlignments/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1861 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/LocalAlignments/erlangen.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1482 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/LocalAlignments/g9.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     2096 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/LocalAlignments/joinoscars.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1104 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/LocalAlignments/nfi2r.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1579 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/LocalAlignments/planarcams.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1481 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/LocalAlignments/planarmove.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      364 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/LocalAlignments/planefit.m
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.204528 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.204528 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1651 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/L2depths.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1278 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/M2Fe.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     3820 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/approximate.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     3186 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/balance_triplets.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     5370 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/create_nullspace.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      928 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/depth_estimation.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)    12256 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/fill_mm.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1880 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/fill_mm_sub.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     3943 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/fill_prmm.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      644 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/normu.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      477 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/spread_depths_col.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      744 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/subseq_longest.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1511 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/u2FI.m
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.208528 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm_test/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     7003 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm_test/bundle_PX_proj.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     2535 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm_test/eval_y_and_dy.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1771 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm_test/fill_mm_bundle.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      403 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm_test/nhom.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     5594 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm_test/qPXbundle_cmp.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      265 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/setpaths.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      465 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/startup.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      189 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/test_.m
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.208528 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)       98 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/comb.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      263 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/combfirst.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      556 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/combnext.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      640 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/diff_rand_ints.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      735 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/dist.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      314 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/eucl_dist.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1049 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/eucl_dist_only.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      278 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/file_exists.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      390 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/k2i.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      124 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/kill_spaces.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     8233 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/load_scene.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      952 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/normalize.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      314 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/normalize_cut.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      410 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/p2e.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      160 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/random_int.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      321 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/str_cut.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      146 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/tiles_set.m
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.208528 multicamselfcal-0.2.0/MultiCamSelfCal/OutputFunctions/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      508 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/OutputFunctions/dispcamstats.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      546 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/OutputFunctions/drawcloud.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      974 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/OutputFunctions/drawobject.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1564 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/OutputFunctions/drawscene.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1656 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/OutputFunctions/evalreprerror.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     3461 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/OutputFunctions/savecalpar.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      508 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/OutputFunctions/showimg.m
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.208528 multicamselfcal-0.2.0/MultiCamSelfCal/Ransac/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      353 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/Ransac/FDs.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      401 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/Ransac/fu2F7.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      547 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/Ransac/mfFDs.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      571 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/Ransac/normu.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      294 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/Ransac/nsamples.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)       61 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/Ransac/p2e.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1617 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/Ransac/rEG.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      116 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/Ransac/seig.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      700 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/Ransac/u2F.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)    15929 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/gocal.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     3962 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/showpoints.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     5323 2023-07-24 14:09:13.212528 multicamselfcal-0.2.0/PKG-INFO
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     4996 2023-07-24 05:51:19.000000 multicamselfcal-0.2.0/README.md
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.208528 multicamselfcal-0.2.0/RadialDistortions/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1233 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/RadialDistortions/comp_distortion_oulu.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      706 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/RadialDistortions/isptnorm.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      899 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/RadialDistortions/readradfile.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1003 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/RadialDistortions/undoheikk.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      916 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/RadialDistortions/undoradial.m
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.208528 multicamselfcal-0.2.0/RansacM/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      481 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/RansacM/Fsampson.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      385 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/RansacM/nsamples.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      593 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/RansacM/pointnormiso.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1494 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/RansacM/rEG.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1058 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/RansacM/u2Fdlt.m
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.212528 multicamselfcal-0.2.0/multicamselfcal.egg-info/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     5323 2023-07-24 14:09:13.000000 multicamselfcal-0.2.0/multicamselfcal.egg-info/PKG-INFO
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     5166 2023-07-24 14:09:13.000000 multicamselfcal-0.2.0/multicamselfcal.egg-info/SOURCES.txt
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)        1 2023-07-24 14:09:13.000000 multicamselfcal-0.2.0/multicamselfcal.egg-info/dependency_links.txt
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)       84 2023-07-24 14:09:13.000000 multicamselfcal-0.2.0/multicamselfcal.egg-info/top_level.txt
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1311 2023-07-24 13:51:04.000000 multicamselfcal-0.2.0/pyproject.toml
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.200528 multicamselfcal-0.2.0/python/
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.212528 multicamselfcal-0.2.0/python/multicamselfcal/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)        0 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/python/multicamselfcal/__init__.py
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1952 2023-07-24 05:15:10.000000 multicamselfcal-0.2.0/python/multicamselfcal/align.py
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)    14115 2023-07-24 05:51:19.000000 multicamselfcal-0.2.0/python/multicamselfcal/execute.py
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     6092 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/python/multicamselfcal/formats.py
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      684 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/python/multicamselfcal/visualization.py
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)       38 2023-07-24 14:09:13.212528 multicamselfcal-0.2.0/setup.cfg
```

### Comparing `multicamselfcal-0.1.0/multicamselfcal/align.py` & `multicamselfcal-0.2.0/python/multicamselfcal/align.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     X = np.dot(V,U.T)
     R=X
 
     T = X2cent - s*np.dot(R,X1cent)
     return s,R,T
 
 def build_xform(s,R,t):
-    T = np.zeros((4,4),dtype=np.float)
+    T = np.zeros((4,4),dtype=float)
     T[:3,:3] = R
     T = s*T
     T[:3,3] = t
     T[3,3]=1.0
     return T
 
 def align_points( s,R,T, X ):
```

### Comparing `multicamselfcal-0.1.0/multicamselfcal/execute.py` & `multicamselfcal-0.2.0/python/multicamselfcal/execute.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,59 +3,33 @@
 import shlex
 import threading
 import os.path
 import logging
 logging.basicConfig()
 import tempfile
 import shutil
+import importlib_resources # backport of importlib.resources that works on Python 3.8 and 3.9
+import pathlib
 
 import numpy as np
 
 from .formats import camera_calibration_yaml_to_radfile
 from .visualization import create_pcd_file_from_points
 
-LOG = logging.getLogger('mcsc')
+# For the importlib.resources stuff to work, these must be
+# installed correctly by pip/etc.
+MCSC_DIRS = [
+    'MultiCamSelfCal',
+    'CommonCfgAndIO',
+    'RadialDistortions',
+    'CalTechCal',
+    'RansacM',
+    ]
 
-class ThreadedCommand(threading.Thread):
-    def __init__(self, cmds,cwd,stdout,stderr,stdin=None,shell=False,executable=None):
-        threading.Thread.__init__(self)
-        if not shell:
-            cmds = shlex.split(cmds)
-        self._cmds = cmds
-        self._cwd = cwd
-        self._stdin = stdin
-        self._stdout = stdout
-        self._stderr = stderr
-        self._shell=shell
-        self._executable=executable
-        self._cb = None
-        self._cbargs = tuple()
-
-    def run(self):
-        kwargs = dict(              stdin=self._stdin,
-                                    stdout=self._stdout,
-                                    stderr=self._stderr,
-                                    shell=self._shell,
-                                    executable=self._executable,
-                                    cwd=self._cwd)
-
-        logging.getLogger('mcsc.cmd').debug("running cmd %r kwargs: %r" % (
-            self._cmds,kwargs))
-
-        self._cmd = subprocess.Popen(self._cmds, **kwargs)
-
-        self.pid = self._cmd.pid
-        self.results = self._cmd.communicate(self._stdin)
-        self.returncode = self._cmd.returncode
-        if self._cb:
-            self._cb(self, *self._cbargs)
-
-    def set_finished_cb(self, cb, *args):
-        self._cb = cb
-        self._cbargs = args
+LOG = logging.getLogger('mcsc')
 
 _cfg_file = """[Files]
 Basename: {basename}
 Image-Extension: jpg
 
 [Images]
 Subpix: 0.5
@@ -89,15 +63,15 @@
     return np.array([map(float,line.split()) for line in lines])
 
 def save_ascii_matrix(arr,fd,isint=False):
     """
     write a np.ndarray with 2 dims
     """
     assert arr.ndim==2
-    if arr.dtype==np.bool:
+    if arr.dtype==bool:
         arr = arr.astype( np.uint8 )
 
     close_file = False
     if type(fd) == str:
         fd = open(fd,mode='w')
         close_file = True
 
@@ -105,44 +79,60 @@
         row_buf = ' '.join( map(repr,row) )
         fd.write(row_buf)
         fd.write('\n')
 
     if close_file:
         fd.close()
 
+def copy_traversable_tree(traversable, dest_path):
+    assert traversable.is_dir()
+    assert dest_path.is_dir()
+    for xap in traversable.iterdir():
+        xap_dest_path = dest_path / xap.name
+        if xap.is_file():
+            with importlib_resources.as_file(xap) as myfile:
+                shutil.copy(myfile, xap_dest_path)
+        else:
+            assert xap.is_dir()
+            xap_dest_path.mkdir()
+            copy_traversable_tree(xap, xap_dest_path )
+
 class _Calibrator:
     def __init__(self, out_dirname, **kwargs):
         if out_dirname:
             out_dirname = os.path.abspath(os.path.expanduser(out_dirname))
             if not os.path.isdir(out_dirname):
                 os.mkdir(out_dirname)
         else:
             out_dirname = tempfile.mkdtemp(prefix=self.__class__.__name__)
 
-        self.octave = kwargs.get('octave','/usr/bin/octave')
-        self.matlab = kwargs.get('matlab','/opt/matlab/R2011a/bin/matlab')
+        self.octave = kwargs.get('octave','octave')
+        self.matlab = kwargs.get('matlab','matlab')
         self.use_matlab = kwargs.get('use_matlab', False)
         self.out_dirname = out_dirname
 
     def create_from_cams(self, cam_ids=[], cam_resolutions={}, cam_points={}, cam_calibrations={}, **kwargs):
         raise NotImplementedError
 
 class MultiCamSelfCal(_Calibrator):
 
     INPUT = ("camera_order.txt","IdMat.dat","points.dat","Res.dat","multicamselfcal.cfg", "original_cam_centers.dat")
 
-    def __init__(self, out_dirname, basename='basename', use_nth_frame=1, mcscdir='/opt/multicamselfcal/MultiCamSelfCal/', **kwargs):
+    def __init__(self, out_dirname, basename='basename', use_nth_frame=1, **kwargs):
         _Calibrator.__init__(self, out_dirname, **kwargs)
-        self.mcscdir = mcscdir
+
+        # Get MCSC source as datafiles resource.
+        # https://setuptools.pypa.io/en/latest/userguide/datafiles.html
+
         self.basename = basename
         self.use_nth_frame = use_nth_frame
         self.align_existing = False
 
-        if not os.path.exists(os.path.join(self.mcscdir,'gocal.m')):
-            LOG.warn("could not find MultiCamSelfCal gocal.m in %s" % self.mcscdir)
+        # if not os.path.exists(os.path.join(self.mcscdir,'gocal.m')):
+        #     LOG.warning("could not find MultiCamSelfCal gocal.m in %s" % self.mcscdir)
 
     def _write_cam_ids(self, cam_ids):
         with open(os.path.join(self.out_dirname,'camera_order.txt'),'w') as f:
             for i,camid in enumerate(cam_ids):
                 if camid[0] == "/":
                     camid=camid[1:]
                 f.write("%s\n"%camid)
@@ -166,32 +156,20 @@
             f.write(_cfg_file.format(**var))
 
         LOG.debug("calibrate cams: %s" % ','.join(cam_ids))
         LOG.debug("undo radial: %s" % radial_distortion)
         LOG.debug("num_cameras_fill: %s" % num_cameras_fill)
         LOG.debug("wrote camera calibration directory: %s" % self.out_dirname)
 
-    def get_cmd_and_cwd(self, cfg):
-        if self.use_matlab:
-            cmds = '%s -nodesktop -nosplash -r "cd(\'%s\'); gocal_func(\'%s\'); exit"' % (
-                        self.matlab, self.mcscdir, cfg)
-            cwd = None
-        else:
-            cmds = '%s gocal.m --config=%s' % (
-                        self.octave, cfg)
-            cwd = self.mcscdir
-        return cmds,cwd
-
-    def execute(self, blocking=True, cb=None, dest=None, silent=True, copy_files=True):
+    def execute(self, dest=None, copy_files=True):
         """
         if dest is specified then all files are copied there unless copy is false. If dest is not
         specified then it is in a subdir of out_dirname called result
 
-        @returns: dest (or nothing if blocking is false). In that case cb is called when complete
-        and is passed the dest argument
+        @returns: dest.
         """
         if not dest:
             dest = os.path.join(self.out_dirname,'result')
             if not os.path.isdir(dest):
                 os.makedirs(dest)
 
         stdout_fname = os.path.join(dest,'STDOUT')
@@ -201,70 +179,61 @@
 
         for f in self.INPUT:
             src = os.path.join(self.out_dirname,f)
             if copy_files:
                 if os.path.isfile(src):
                     shutil.copy(src, dest)
                 else:
-                    LOG.warn("Could not find %s" % src)
+                    LOG.warning("Could not find %s" % src)
             else:
                 if not os.path.isfile(src):
-                    LOG.warn("Could not find %s" % src)
+                    LOG.warning("Could not find %s" % src)
 
         if copy_files:
             for k,v in self.get_camera_names_map().items():
                 src = os.path.join(self.out_dirname,v)
                 if os.path.isfile(src):
                     shutil.copy(src, dest)
                 else:
-                    LOG.warn("Could not find %s" % src)
+                    LOG.warning("Could not find %s" % src)
 
         cfg = os.path.abspath(os.path.join(dest, "multicamselfcal.cfg"))
 
-        cmds,cwd = self.get_cmd_and_cwd(cfg)
-
-        bash_path = '/bin/bash'
-        if os.path.exists(bash_path) and not silent:
-            shell=True
-            # http://stackoverflow.com/questions/692000
-            cmds = cmds + ' > >(tee %s) 2> >(tee %s >&2)'%(stdout_fname,stderr_fname)
-            executable = bash_path
-            stdout = stderr = None
-        else:
-            shell=False
-            executable=None
-            if not silent:
-                LOG.warn('you requested not silent, but bash is required to support that.')
-            stdout = open(stdout_fname,'w')
-            stderr = open(stderr_fname,'w')
-
-        cmd = ThreadedCommand(cmds,cwd=cwd,stdout=stdout,stderr=stderr,
-                              shell=shell,executable=executable)
-        cmd.set_finished_cb(cb,dest)
-        cmd.start()
-
-        if blocking:
-            cmd.join()
-            if cmd.returncode != 0:
-                raise RuntimeError('MCSC failed')
-            return dest
+        with tempfile.TemporaryDirectory() as mcscdir:
+            mcscdir = pathlib.Path(mcscdir)
+            for subdir in MCSC_DIRS:
+                copied_sub_dir = mcscdir/subdir
+                copied_sub_dir.mkdir()
+                traversable = importlib_resources.files(subdir)
+                copy_traversable_tree(traversable, copied_sub_dir)
+
+            if self.use_matlab:
+                cmds = '%s -nodesktop -nosplash -r "cd(\'%s\'); gocal_func(\'%s\'); exit"' % (
+                            self.matlab, mcscdir, cfg)
+                cwd = None
+            else:
+                cmds = '%s gocal.m --config=%s' % (
+                            self.octave, cfg)
+                cwd = mcscdir / 'MultiCamSelfCal'
+            subprocess.check_call(cmds, cwd=cwd, shell=True)
+        return dest
 
-    def create_from_cams(self, cam_ids=[], cam_resolutions={}, cam_points={}, cam_calibrations={}, num_cameras_fill=-1, **kwargs):
+    def create_from_cams(self, cam_ids=[], cam_resolutions={}, cam_points={}, cam_calibrations={}, num_cameras_fill=-1, initial_tolerance=10.0):
         #num_cameras_fill = -1 means use all cameras (= len(cam_ids))
 
         if not cam_ids:
             cam_ids = cam_points.keys()
 
         #remove cameras with no points
         cams_to_remove = []
         for cam in cam_ids:
             nvalid = np.count_nonzero(np.nan_to_num(np.array(cam_points[cam])))
             if nvalid == 0:
                 cams_to_remove.append(cam)
-                LOG.warn("removing cam %s - no points detected" % cam)
+                LOG.warning("removing cam %s - no points detected" % cam)
         map(cam_ids.remove, cams_to_remove)
 
         self._write_cam_ids(cam_ids)
 
         resfd = open(os.path.join(self.out_dirname,'Res.dat'), 'w')
         foundfd = open(os.path.join(self.out_dirname,'IdMat.dat'), 'w')
         pointsfd = open(os.path.join(self.out_dirname,'points.dat'), 'w')
@@ -312,15 +281,16 @@
         pointsfd.close()
 
         undo_radial = all([cam in cam_calibrations for cam in cam_ids])
         self._write_cfg(cam_ids,
                         undo_radial,
                         True,
                         num_cameras_fill,
-                        [])
+                        [],
+                        initial_tolerance)
         LOG.debug("dropped cams: %s" % ','.join(cams_to_remove))
 
     def create_calibration_directory(self, cam_ids, IdMat, points, Res, cam_calibrations=[], cam_centers=[], radial_distortion=0, square_pixels=1, num_cameras_fill=-1, initial_tolerance=10.0):
         assert len(Res) == len(cam_ids)
         if len(cam_calibrations): assert len(cam_ids) == len(cam_calibrations)
         if len(cam_centers): assert len(cam_ids) == len(cam_centers)
 
@@ -392,27 +362,29 @@
         create_pcd_file_from_points(fname,points)
 
 if __name__ == "__main__":
     import sys
 
     logging.basicConfig(level=logging.DEBUG)
 
-    mydir = os.path.split(__file__)[0]
-    SRC_PATH = os.path.abspath(os.path.join(mydir,'..','..'))
+    # mydir = os.path.split(__file__)[0]
+    # SRC_PATH = os.path.abspath(os.path.join(mydir,'..','..'))
+
+    data_dir = sys.argv[1]
+    data = os.path.abspath(os.path.expanduser(data_dir))
 
-    try:
-        data = os.path.abspath(os.path.expanduser(sys.argv[1]))
-    except IndexError:
-        data = os.path.abspath(
-                    os.path.join(SRC_PATH,
-                    'strawlab','test-data','DATA20100906_134124'))
-
-    mcscdir = os.path.join(SRC_PATH,'MultiCamSelfCal')
-    kwargs = {}
-    if os.path.exists(mcscdir):
-        # assume running from source
-        kwargs['mcscdir']=mcscdir
+    # try:
+    #     data = os.path.abspath(os.path.expanduser(sys.argv[1]))
+    # except IndexError:
+    #     data = os.path.abspath(
+    #                 os.path.join(SRC_PATH,
+    #                 'strawlab','test-data','DATA20100906_134124'))
+
+    # mcscdir = os.path.join(SRC_PATH,'MultiCamSelfCal')
+    # if os.path.exists(mcscdir):
+    #     # assume running from source
+    #     kwargs['mcscdir']=mcscdir
 
-    mcsc = MultiCamSelfCal(data, **kwargs)
-    caldir = mcsc.execute(silent=False)
+    mcsc = MultiCamSelfCal(data)#, **kwargs)
+    caldir = mcsc.execute()
 
     print("result:",caldir)
```

### Comparing `multicamselfcal-0.1.0/multicamselfcal/formats.py` & `multicamselfcal-0.2.0/python/multicamselfcal/formats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 
 import yaml
 
 def camera_calibration_yaml_to_radfile(yamlpath, radpath, lossy_ok=False):
     with open(yamlpath,'r') as yf:
-        y = yaml.load(yf)
+        y = yaml.safe_load(yf)
 
         K = y['camera_matrix']['data']
         Knp = np.array(K)
         Knp.shape = y['camera_matrix']['rows'],y['camera_matrix']['cols']
 
         P = y['projection_matrix']['data']
         P = np.array(P)
```

### Comparing `multicamselfcal-0.1.0/multicamselfcal/visualization.py` & `multicamselfcal-0.2.0/python/multicamselfcal/visualization.py`

 * *Files identical despite different names*


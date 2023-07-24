# Comparing `tmp/multicamselfcal-0.2.0.tar.gz` & `tmp/multicamselfcal-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multicamselfcal-0.2.0.tar", last modified: Mon Jul 24 14:09:13 2023, max compression
+gzip compressed data, was "multicamselfcal-0.2.1.tar", last modified: Mon Jul 24 15:30:42 2023, max compression
```

## Comparing `multicamselfcal-0.2.0.tar` & `multicamselfcal-0.2.1.tar`

### file list

```diff
@@ -1,154 +1,155 @@
-drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.212528 multicamselfcal-0.2.0/
-drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.200528 multicamselfcal-0.2.0/CalTechCal/
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     3925 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/analyse_error.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1675 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/apply_distortion.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)       45 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/check_active_images.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1233 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/comp_distortion_oulu.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1134 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/comp_error_calib.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     2151 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/comp_ext_calib.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     5138 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/compute_extrinsic_init.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     2768 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/compute_extrinsic_refine.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     5289 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/export_calib_data.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1509 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/extract_parameters.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     6543 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/ginput3.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)    19148 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/go_calib_optim_iter.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     2094 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/gorad.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     2454 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/goradf.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1203 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/normalize.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      424 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/preparedata.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     8737 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/project_points2.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     4136 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/quiver.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1730 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/rigid_motion.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     4773 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/rodrigues.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     6751 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CalTechCal/visualize_distortions.m
-drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.204528 multicamselfcal-0.2.0/CommonCfgAndIO/
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1807 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CommonCfgAndIO/ConvertOldConfigToNew.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)    24912 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CommonCfgAndIO/configdata.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      809 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CommonCfgAndIO/expname.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     3623 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CommonCfgAndIO/loaddata.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     6625 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CommonCfgAndIO/oldexperiments.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)    11438 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CommonCfgAndIO/read_configuration.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     4852 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/CommonCfgAndIO/read_generic_configuration.m
-drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.204528 multicamselfcal-0.2.0/MultiCamSelfCal/
-drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.204528 multicamselfcal-0.2.0/MultiCamSelfCal/BlueCLocal/
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1186 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/BlueCLocal/align_existing_camera_centers.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     3118 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/BlueCLocal/bluechoengg.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     2938 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/BlueCLocal/bluecrz.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     5498 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/BlueCLocal/flydra.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1358 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/BlueCLocal/humdra.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     6781 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/BlueCLocal/mamarama.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1409 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/BlueCLocal/strawlab_test.m
-drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.204528 multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      130 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/align3d.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1684 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/estimateLambda.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     2056 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/estimatePX.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1405 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/estsimt.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     4642 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/euclidize.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1999 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/findinl.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      796 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/findoutl.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1082 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/reprerror.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      794 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/rq.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     2052 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/selfcalib.m
-drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.204528 multicamselfcal-0.2.0/MultiCamSelfCal/FindingPoints/
--rw-rw-r--   0 astraw    (1000) astraw    (1000)    10807 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/FindingPoints/getpoint.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     4601 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/FindingPoints/im2imstat.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     6237 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/FindingPoints/im2points.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      498 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/FindingPoints/mycorr2.m
-drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.204528 multicamselfcal-0.2.0/MultiCamSelfCal/LocalAlignments/
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1861 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/LocalAlignments/erlangen.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1482 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/LocalAlignments/g9.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     2096 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/LocalAlignments/joinoscars.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1104 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/LocalAlignments/nfi2r.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1579 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/LocalAlignments/planarcams.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1481 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/LocalAlignments/planarmove.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      364 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/LocalAlignments/planefit.m
-drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.204528 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/
-drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.204528 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1651 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/L2depths.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1278 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/M2Fe.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     3820 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/approximate.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     3186 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/balance_triplets.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     5370 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/create_nullspace.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      928 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/depth_estimation.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)    12256 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/fill_mm.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1880 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/fill_mm_sub.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     3943 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/fill_prmm.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      644 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/normu.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      477 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/spread_depths_col.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      744 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/subseq_longest.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1511 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/u2FI.m
-drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.208528 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm_test/
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     7003 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm_test/bundle_PX_proj.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     2535 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm_test/eval_y_and_dy.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1771 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm_test/fill_mm_bundle.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      403 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm_test/nhom.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     5594 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm_test/qPXbundle_cmp.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      265 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/setpaths.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      465 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/startup.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      189 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/test_.m
-drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.208528 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/
--rw-rw-r--   0 astraw    (1000) astraw    (1000)       98 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/comb.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      263 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/combfirst.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      556 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/combnext.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      640 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/diff_rand_ints.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      735 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/dist.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      314 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/eucl_dist.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1049 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/eucl_dist_only.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      278 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/file_exists.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      390 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/k2i.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      124 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/kill_spaces.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     8233 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/load_scene.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      952 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/normalize.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      314 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/normalize_cut.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      410 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/p2e.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      160 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/random_int.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      321 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/str_cut.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      146 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/tiles_set.m
-drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.208528 multicamselfcal-0.2.0/MultiCamSelfCal/OutputFunctions/
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      508 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/OutputFunctions/dispcamstats.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      546 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/OutputFunctions/drawcloud.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      974 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/OutputFunctions/drawobject.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1564 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/OutputFunctions/drawscene.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1656 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/OutputFunctions/evalreprerror.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     3461 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/OutputFunctions/savecalpar.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      508 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/OutputFunctions/showimg.m
-drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.208528 multicamselfcal-0.2.0/MultiCamSelfCal/Ransac/
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      353 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/Ransac/FDs.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      401 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/Ransac/fu2F7.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      547 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/Ransac/mfFDs.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      571 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/Ransac/normu.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      294 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/Ransac/nsamples.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)       61 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/Ransac/p2e.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1617 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/Ransac/rEG.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      116 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/Ransac/seig.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      700 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/Ransac/u2F.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)    15929 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/gocal.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     3962 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/MultiCamSelfCal/showpoints.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     5323 2023-07-24 14:09:13.212528 multicamselfcal-0.2.0/PKG-INFO
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     4996 2023-07-24 05:51:19.000000 multicamselfcal-0.2.0/README.md
-drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.208528 multicamselfcal-0.2.0/RadialDistortions/
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1233 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/RadialDistortions/comp_distortion_oulu.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      706 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/RadialDistortions/isptnorm.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      899 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/RadialDistortions/readradfile.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1003 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/RadialDistortions/undoheikk.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      916 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/RadialDistortions/undoradial.m
-drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.208528 multicamselfcal-0.2.0/RansacM/
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      481 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/RansacM/Fsampson.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      385 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/RansacM/nsamples.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      593 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/RansacM/pointnormiso.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1494 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/RansacM/rEG.m
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1058 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/RansacM/u2Fdlt.m
-drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.212528 multicamselfcal-0.2.0/multicamselfcal.egg-info/
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     5323 2023-07-24 14:09:13.000000 multicamselfcal-0.2.0/multicamselfcal.egg-info/PKG-INFO
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     5166 2023-07-24 14:09:13.000000 multicamselfcal-0.2.0/multicamselfcal.egg-info/SOURCES.txt
--rw-rw-r--   0 astraw    (1000) astraw    (1000)        1 2023-07-24 14:09:13.000000 multicamselfcal-0.2.0/multicamselfcal.egg-info/dependency_links.txt
--rw-rw-r--   0 astraw    (1000) astraw    (1000)       84 2023-07-24 14:09:13.000000 multicamselfcal-0.2.0/multicamselfcal.egg-info/top_level.txt
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1311 2023-07-24 13:51:04.000000 multicamselfcal-0.2.0/pyproject.toml
-drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.200528 multicamselfcal-0.2.0/python/
-drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 14:09:13.212528 multicamselfcal-0.2.0/python/multicamselfcal/
--rw-rw-r--   0 astraw    (1000) astraw    (1000)        0 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/python/multicamselfcal/__init__.py
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     1952 2023-07-24 05:15:10.000000 multicamselfcal-0.2.0/python/multicamselfcal/align.py
--rw-rw-r--   0 astraw    (1000) astraw    (1000)    14115 2023-07-24 05:51:19.000000 multicamselfcal-0.2.0/python/multicamselfcal/execute.py
--rw-rw-r--   0 astraw    (1000) astraw    (1000)     6092 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/python/multicamselfcal/formats.py
--rw-rw-r--   0 astraw    (1000) astraw    (1000)      684 2023-07-22 16:07:32.000000 multicamselfcal-0.2.0/python/multicamselfcal/visualization.py
--rw-rw-r--   0 astraw    (1000) astraw    (1000)       38 2023-07-24 14:09:13.212528 multicamselfcal-0.2.0/setup.cfg
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 15:30:42.244518 multicamselfcal-0.2.1/
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 15:30:42.236518 multicamselfcal-0.2.1/CalTechCal/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     3925 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CalTechCal/analyse_error.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1675 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CalTechCal/apply_distortion.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)       45 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CalTechCal/check_active_images.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1233 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CalTechCal/comp_distortion_oulu.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1134 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CalTechCal/comp_error_calib.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     2151 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CalTechCal/comp_ext_calib.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     5138 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CalTechCal/compute_extrinsic_init.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     2768 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CalTechCal/compute_extrinsic_refine.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     5289 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CalTechCal/export_calib_data.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1509 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CalTechCal/extract_parameters.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     6543 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CalTechCal/ginput3.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)    19148 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CalTechCal/go_calib_optim_iter.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     2094 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CalTechCal/gorad.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     2454 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CalTechCal/goradf.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1203 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CalTechCal/normalize.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      424 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CalTechCal/preparedata.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     8737 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CalTechCal/project_points2.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     4136 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CalTechCal/quiver.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1730 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CalTechCal/rigid_motion.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     4773 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CalTechCal/rodrigues.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     6751 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CalTechCal/visualize_distortions.m
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 15:30:42.236518 multicamselfcal-0.2.1/CommonCfgAndIO/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1807 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CommonCfgAndIO/ConvertOldConfigToNew.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)    24912 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CommonCfgAndIO/configdata.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      809 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CommonCfgAndIO/expname.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     3623 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CommonCfgAndIO/loaddata.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     6625 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CommonCfgAndIO/oldexperiments.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)    11438 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CommonCfgAndIO/read_configuration.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     4852 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/CommonCfgAndIO/read_generic_configuration.m
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 15:30:42.236518 multicamselfcal-0.2.1/MultiCamSelfCal/
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 15:30:42.236518 multicamselfcal-0.2.1/MultiCamSelfCal/BlueCLocal/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1186 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/BlueCLocal/align_existing_camera_centers.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     3118 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/BlueCLocal/bluechoengg.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     2938 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/BlueCLocal/bluecrz.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     5498 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/BlueCLocal/flydra.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1358 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/BlueCLocal/humdra.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     6781 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/BlueCLocal/mamarama.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1409 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/BlueCLocal/strawlab_test.m
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 15:30:42.236518 multicamselfcal-0.2.1/MultiCamSelfCal/CoreFunctions/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      130 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/CoreFunctions/align3d.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1684 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/CoreFunctions/estimateLambda.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     2056 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/CoreFunctions/estimatePX.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1405 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/CoreFunctions/estsimt.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     4642 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/CoreFunctions/euclidize.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1999 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/CoreFunctions/findinl.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      796 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/CoreFunctions/findoutl.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1082 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/CoreFunctions/reprerror.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      794 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/CoreFunctions/rq.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     2052 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/CoreFunctions/selfcalib.m
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 15:30:42.236518 multicamselfcal-0.2.1/MultiCamSelfCal/FindingPoints/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)    10807 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/FindingPoints/getpoint.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     4601 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/FindingPoints/im2imstat.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     6237 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/FindingPoints/im2points.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      498 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/FindingPoints/mycorr2.m
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 15:30:42.236518 multicamselfcal-0.2.1/MultiCamSelfCal/LocalAlignments/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1861 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/LocalAlignments/erlangen.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1482 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/LocalAlignments/g9.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     2096 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/LocalAlignments/joinoscars.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1104 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/LocalAlignments/nfi2r.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1579 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/LocalAlignments/planarcams.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1481 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/LocalAlignments/planarmove.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      364 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/LocalAlignments/planefit.m
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 15:30:42.236518 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 15:30:42.240518 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1651 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm/L2depths.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1278 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm/M2Fe.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     3820 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm/approximate.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     3186 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm/balance_triplets.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     5370 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm/create_nullspace.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      928 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm/depth_estimation.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)    12256 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm/fill_mm.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1880 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm/fill_mm_sub.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     3943 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm/fill_prmm.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      644 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm/normu.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      477 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm/spread_depths_col.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      744 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm/subseq_longest.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1511 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm/u2FI.m
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 15:30:42.240518 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm_test/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     7003 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm_test/bundle_PX_proj.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     2535 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm_test/eval_y_and_dy.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1771 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm_test/fill_mm_bundle.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      403 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm_test/nhom.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     5594 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm_test/qPXbundle_cmp.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      265 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/setpaths.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      465 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/startup.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      189 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/test_.m
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 15:30:42.240518 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/utils/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)       98 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/utils/comb.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      263 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/utils/combfirst.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      556 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/utils/combnext.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      640 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/utils/diff_rand_ints.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      735 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/utils/dist.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      314 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/utils/eucl_dist.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1049 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/utils/eucl_dist_only.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      278 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/utils/file_exists.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      390 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/utils/k2i.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      124 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/utils/kill_spaces.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     8233 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/utils/load_scene.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      952 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/utils/normalize.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      314 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/utils/normalize_cut.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      410 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/utils/p2e.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      160 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/utils/random_int.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      321 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/utils/str_cut.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      146 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/utils/tiles_set.m
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 15:30:42.240518 multicamselfcal-0.2.1/MultiCamSelfCal/OutputFunctions/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      508 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/OutputFunctions/dispcamstats.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      546 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/OutputFunctions/drawcloud.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      974 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/OutputFunctions/drawobject.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1564 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/OutputFunctions/drawscene.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1656 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/OutputFunctions/evalreprerror.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     3461 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/OutputFunctions/savecalpar.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      508 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/OutputFunctions/showimg.m
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 15:30:42.240518 multicamselfcal-0.2.1/MultiCamSelfCal/Ransac/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      353 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/Ransac/FDs.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      401 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/Ransac/fu2F7.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      547 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/Ransac/mfFDs.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      571 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/Ransac/normu.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      294 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/Ransac/nsamples.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)       61 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/Ransac/p2e.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1617 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/Ransac/rEG.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      116 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/Ransac/seig.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      700 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/Ransac/u2F.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)    15929 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/gocal.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     3962 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/MultiCamSelfCal/showpoints.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     5323 2023-07-24 15:30:42.244518 multicamselfcal-0.2.1/PKG-INFO
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     4996 2023-07-24 14:10:10.000000 multicamselfcal-0.2.1/README.md
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 15:30:42.240518 multicamselfcal-0.2.1/RadialDistortions/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1233 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/RadialDistortions/comp_distortion_oulu.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      706 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/RadialDistortions/isptnorm.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      899 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/RadialDistortions/readradfile.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1003 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/RadialDistortions/undoheikk.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      916 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/RadialDistortions/undoradial.m
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 15:30:42.240518 multicamselfcal-0.2.1/RansacM/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      481 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/RansacM/Fsampson.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      385 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/RansacM/nsamples.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      593 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/RansacM/pointnormiso.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1494 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/RansacM/rEG.m
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1058 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/RansacM/u2Fdlt.m
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 15:30:42.244518 multicamselfcal-0.2.1/multicamselfcal.egg-info/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     5323 2023-07-24 15:30:42.000000 multicamselfcal-0.2.1/multicamselfcal.egg-info/PKG-INFO
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     5204 2023-07-24 15:30:42.000000 multicamselfcal-0.2.1/multicamselfcal.egg-info/SOURCES.txt
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)        1 2023-07-24 15:30:42.000000 multicamselfcal-0.2.1/multicamselfcal.egg-info/dependency_links.txt
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)       36 2023-07-24 15:30:42.000000 multicamselfcal-0.2.1/multicamselfcal.egg-info/requires.txt
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)       84 2023-07-24 15:30:42.000000 multicamselfcal-0.2.1/multicamselfcal.egg-info/top_level.txt
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1390 2023-07-24 15:29:44.000000 multicamselfcal-0.2.1/pyproject.toml
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 15:30:42.232518 multicamselfcal-0.2.1/python/
+drwxrwxr-x   0 astraw    (1000) astraw    (1000)        0 2023-07-24 15:30:42.244518 multicamselfcal-0.2.1/python/multicamselfcal/
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)        0 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/python/multicamselfcal/__init__.py
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     1952 2023-07-24 14:10:10.000000 multicamselfcal-0.2.1/python/multicamselfcal/align.py
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)    14115 2023-07-24 14:10:10.000000 multicamselfcal-0.2.1/python/multicamselfcal/execute.py
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)     6092 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/python/multicamselfcal/formats.py
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)      684 2023-07-22 16:07:32.000000 multicamselfcal-0.2.1/python/multicamselfcal/visualization.py
+-rw-rw-r--   0 astraw    (1000) astraw    (1000)       38 2023-07-24 15:30:42.244518 multicamselfcal-0.2.1/setup.cfg
```

### Comparing `multicamselfcal-0.2.0/CalTechCal/analyse_error.m` & `multicamselfcal-0.2.1/CalTechCal/analyse_error.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/CalTechCal/apply_distortion.m` & `multicamselfcal-0.2.1/CalTechCal/apply_distortion.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/CalTechCal/comp_distortion_oulu.m` & `multicamselfcal-0.2.1/CalTechCal/comp_distortion_oulu.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/CalTechCal/comp_error_calib.m` & `multicamselfcal-0.2.1/CalTechCal/comp_error_calib.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/CalTechCal/comp_ext_calib.m` & `multicamselfcal-0.2.1/CalTechCal/comp_ext_calib.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/CalTechCal/compute_extrinsic_init.m` & `multicamselfcal-0.2.1/CalTechCal/compute_extrinsic_init.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/CalTechCal/compute_extrinsic_refine.m` & `multicamselfcal-0.2.1/CalTechCal/compute_extrinsic_refine.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/CalTechCal/export_calib_data.m` & `multicamselfcal-0.2.1/CalTechCal/export_calib_data.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/CalTechCal/extract_parameters.m` & `multicamselfcal-0.2.1/CalTechCal/extract_parameters.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/CalTechCal/ginput3.m` & `multicamselfcal-0.2.1/CalTechCal/ginput3.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/CalTechCal/go_calib_optim_iter.m` & `multicamselfcal-0.2.1/CalTechCal/go_calib_optim_iter.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/CalTechCal/gorad.m` & `multicamselfcal-0.2.1/CalTechCal/gorad.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/CalTechCal/goradf.m` & `multicamselfcal-0.2.1/CalTechCal/goradf.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/CalTechCal/normalize.m` & `multicamselfcal-0.2.1/CalTechCal/normalize.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/CalTechCal/project_points2.m` & `multicamselfcal-0.2.1/CalTechCal/project_points2.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/CalTechCal/quiver.m` & `multicamselfcal-0.2.1/CalTechCal/quiver.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/CalTechCal/rigid_motion.m` & `multicamselfcal-0.2.1/CalTechCal/rigid_motion.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/CalTechCal/rodrigues.m` & `multicamselfcal-0.2.1/CalTechCal/rodrigues.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/CalTechCal/visualize_distortions.m` & `multicamselfcal-0.2.1/CalTechCal/visualize_distortions.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/CommonCfgAndIO/ConvertOldConfigToNew.m` & `multicamselfcal-0.2.1/CommonCfgAndIO/ConvertOldConfigToNew.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/CommonCfgAndIO/configdata.m` & `multicamselfcal-0.2.1/CommonCfgAndIO/configdata.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/CommonCfgAndIO/expname.m` & `multicamselfcal-0.2.1/CommonCfgAndIO/expname.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/CommonCfgAndIO/loaddata.m` & `multicamselfcal-0.2.1/CommonCfgAndIO/loaddata.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/CommonCfgAndIO/oldexperiments.m` & `multicamselfcal-0.2.1/CommonCfgAndIO/oldexperiments.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/CommonCfgAndIO/read_configuration.m` & `multicamselfcal-0.2.1/CommonCfgAndIO/read_configuration.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/CommonCfgAndIO/read_generic_configuration.m` & `multicamselfcal-0.2.1/CommonCfgAndIO/read_generic_configuration.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/BlueCLocal/align_existing_camera_centers.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/BlueCLocal/align_existing_camera_centers.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/BlueCLocal/bluechoengg.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/BlueCLocal/bluechoengg.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/BlueCLocal/bluecrz.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/BlueCLocal/bluecrz.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/BlueCLocal/flydra.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/BlueCLocal/flydra.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/BlueCLocal/humdra.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/BlueCLocal/humdra.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/BlueCLocal/mamarama.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/BlueCLocal/mamarama.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/BlueCLocal/strawlab_test.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/BlueCLocal/strawlab_test.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/estimateLambda.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/CoreFunctions/estimateLambda.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/estimatePX.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/CoreFunctions/estimatePX.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/estsimt.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/CoreFunctions/estsimt.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/euclidize.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/CoreFunctions/euclidize.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/findinl.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/CoreFunctions/findinl.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/findoutl.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/CoreFunctions/findoutl.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/reprerror.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/CoreFunctions/reprerror.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/rq.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/CoreFunctions/rq.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/CoreFunctions/selfcalib.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/CoreFunctions/selfcalib.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/FindingPoints/getpoint.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/FindingPoints/getpoint.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/FindingPoints/im2imstat.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/FindingPoints/im2imstat.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/FindingPoints/im2points.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/FindingPoints/im2points.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/LocalAlignments/erlangen.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/LocalAlignments/erlangen.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/LocalAlignments/g9.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/LocalAlignments/g9.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/LocalAlignments/joinoscars.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/LocalAlignments/joinoscars.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/LocalAlignments/nfi2r.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/LocalAlignments/nfi2r.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/LocalAlignments/planarcams.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/LocalAlignments/planarcams.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/LocalAlignments/planarmove.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/LocalAlignments/planarmove.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/L2depths.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm/L2depths.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/M2Fe.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm/M2Fe.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/approximate.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm/approximate.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/balance_triplets.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm/balance_triplets.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/create_nullspace.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm/create_nullspace.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/depth_estimation.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm/depth_estimation.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/fill_mm.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm/fill_mm.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/fill_mm_sub.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm/fill_mm_sub.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/fill_prmm.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm/fill_prmm.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/normu.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm/normu.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/subseq_longest.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm/subseq_longest.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm/u2FI.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm/u2FI.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm_test/bundle_PX_proj.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm_test/bundle_PX_proj.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm_test/eval_y_and_dy.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm_test/eval_y_and_dy.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm_test/fill_mm_bundle.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm_test/fill_mm_bundle.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/fill_mm_test/qPXbundle_cmp.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/fill_mm_test/qPXbundle_cmp.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/combnext.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/utils/combnext.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/diff_rand_ints.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/utils/diff_rand_ints.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/dist.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/utils/dist.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/eucl_dist_only.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/utils/eucl_dist_only.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/load_scene.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/utils/load_scene.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/MartinecPajdla/utils/normalize.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/MartinecPajdla/utils/normalize.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/OutputFunctions/drawcloud.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/OutputFunctions/drawcloud.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/OutputFunctions/drawobject.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/OutputFunctions/drawobject.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/OutputFunctions/drawscene.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/OutputFunctions/drawscene.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/OutputFunctions/evalreprerror.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/OutputFunctions/evalreprerror.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/OutputFunctions/savecalpar.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/OutputFunctions/savecalpar.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/Ransac/mfFDs.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/Ransac/mfFDs.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/Ransac/normu.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/Ransac/normu.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/Ransac/rEG.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/Ransac/rEG.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/Ransac/u2F.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/Ransac/u2F.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/gocal.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/gocal.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/MultiCamSelfCal/showpoints.m` & `multicamselfcal-0.2.1/MultiCamSelfCal/showpoints.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/PKG-INFO` & `multicamselfcal-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multicamselfcal
-Version: 0.2.0
+Version: 0.2.1
 Summary: wrapper for the Octave/Matlab multicamselfcal library
 Author: John Stowers
 Maintainer-email: Andrew Straw <strawman@astraw.com>
 Project-URL: homepage, https://github.com/strawlab/multicamselfcal
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `multicamselfcal-0.2.0/README.md` & `multicamselfcal-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/RadialDistortions/comp_distortion_oulu.m` & `multicamselfcal-0.2.1/RadialDistortions/comp_distortion_oulu.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/RadialDistortions/isptnorm.m` & `multicamselfcal-0.2.1/RadialDistortions/isptnorm.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/RadialDistortions/readradfile.m` & `multicamselfcal-0.2.1/RadialDistortions/readradfile.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/RadialDistortions/undoheikk.m` & `multicamselfcal-0.2.1/RadialDistortions/undoheikk.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/RadialDistortions/undoradial.m` & `multicamselfcal-0.2.1/RadialDistortions/undoradial.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/RansacM/pointnormiso.m` & `multicamselfcal-0.2.1/RansacM/pointnormiso.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/RansacM/rEG.m` & `multicamselfcal-0.2.1/RansacM/rEG.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/RansacM/u2Fdlt.m` & `multicamselfcal-0.2.1/RansacM/u2Fdlt.m`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/multicamselfcal.egg-info/PKG-INFO` & `multicamselfcal-0.2.1/multicamselfcal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multicamselfcal
-Version: 0.2.0
+Version: 0.2.1
 Summary: wrapper for the Octave/Matlab multicamselfcal library
 Author: John Stowers
 Maintainer-email: Andrew Straw <strawman@astraw.com>
 Project-URL: homepage, https://github.com/strawlab/multicamselfcal
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `multicamselfcal-0.2.0/multicamselfcal.egg-info/SOURCES.txt` & `multicamselfcal-0.2.1/multicamselfcal.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -121,13 +121,14 @@
 RansacM/nsamples.m
 RansacM/pointnormiso.m
 RansacM/rEG.m
 RansacM/u2Fdlt.m
 multicamselfcal.egg-info/PKG-INFO
 multicamselfcal.egg-info/SOURCES.txt
 multicamselfcal.egg-info/dependency_links.txt
+multicamselfcal.egg-info/requires.txt
 multicamselfcal.egg-info/top_level.txt
 python/multicamselfcal/__init__.py
 python/multicamselfcal/align.py
 python/multicamselfcal/execute.py
 python/multicamselfcal/formats.py
 python/multicamselfcal/visualization.py
```

### Comparing `multicamselfcal-0.2.0/pyproject.toml` & `multicamselfcal-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 [project]
 name = "multicamselfcal"
-version = "0.2.0"
+version = "0.2.1"
 description = "wrapper for the Octave/Matlab multicamselfcal library"
 authors = [{ name = "John Stowers"}]
 maintainers = [{ name = "Andrew Straw", email = "strawman@astraw.com" }]
 readme = "README.md"
 requires-python = ">=3.8"
 urls.homepage = "https://github.com/strawlab/multicamselfcal"
 
+dependencies = [
+    "numpy",
+    "PyYAML",
+    "importlib-resources >= 6",
+]
+
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 package-dir = {"multicamselfcal" = "python/multicamselfcal"}
 packages = [
```

### Comparing `multicamselfcal-0.2.0/python/multicamselfcal/align.py` & `multicamselfcal-0.2.1/python/multicamselfcal/align.py`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/python/multicamselfcal/execute.py` & `multicamselfcal-0.2.1/python/multicamselfcal/execute.py`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/python/multicamselfcal/formats.py` & `multicamselfcal-0.2.1/python/multicamselfcal/formats.py`

 * *Files identical despite different names*

### Comparing `multicamselfcal-0.2.0/python/multicamselfcal/visualization.py` & `multicamselfcal-0.2.1/python/multicamselfcal/visualization.py`

 * *Files identical despite different names*


# Comparing `tmp/simpa-0.8.7.tar.gz` & `tmp/simpa-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpa-0.8.7.tar", max compression
+gzip compressed data, was "simpa-0.8.9.tar", max compression
```

## Comparing `simpa-0.8.7.tar` & `simpa-0.8.9.tar`

### file list

```diff
@@ -1,185 +1,188 @@
--rw-r--r--   0        0        0      239 2022-08-18 14:33:22.782354 simpa-0.8.7/LICENSE.md
-drwxr-xr-x   0        0        0        0 2022-08-18 14:33:22.782354 simpa-0.8.7/LICENSES/
--rwxr-xr-x   0        0        0    11346 2022-08-18 14:33:22.782354 simpa-0.8.7/README.md
--rw-r--r--   0        0        0     1821 2022-08-18 14:33:22.782354 simpa-0.8.7/pyproject.toml
--rw-r--r--   0        0        0     3314 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/__init__.py
--rw-r--r--   0        0        0      968 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/__init__.py
--rw-r--r--   0        0        0     1549 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/device_digital_twins/__init__.py
--rw-r--r--   0        0        0      152 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/device_digital_twins/detection_geometries/__init__.py
--rw-r--r--   0        0        0     5560 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/device_digital_twins/detection_geometries/curved_array.py
--rw-r--r--   0        0        0     6116 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/device_digital_twins/detection_geometries/detection_geometry_base.py
--rw-r--r--   0        0        0     4072 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/device_digital_twins/detection_geometries/linear_array.py
--rw-r--r--   0        0        0     5497 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/device_digital_twins/detection_geometries/planar_array.py
--rw-r--r--   0        0        0    13842 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/device_digital_twins/digital_device_twin_base.py
--rw-r--r--   0        0        0      152 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/device_digital_twins/illumination_geometries/__init__.py
--rw-r--r--   0        0        0     2557 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/device_digital_twins/illumination_geometries/disk_illumination.py
--rw-r--r--   0        0        0     2666 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/device_digital_twins/illumination_geometries/gaussian_beam_illumination.py
--rw-r--r--   0        0        0     2987 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/device_digital_twins/illumination_geometries/illumination_geometry_base.py
--rw-r--r--   0        0        0     2347 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/device_digital_twins/illumination_geometries/ithera_msot_acuity_illumination.py
--rw-r--r--   0        0        0     3839 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/device_digital_twins/illumination_geometries/ithera_msot_invision_illumination.py
--rw-r--r--   0        0        0     3245 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/device_digital_twins/illumination_geometries/pencil_array_illumination.py
--rw-r--r--   0        0        0     1515 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/device_digital_twins/illumination_geometries/pencil_beam_illumination.py
--rw-r--r--   0        0        0     3520 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/device_digital_twins/illumination_geometries/slit_illumination.py
--rw-r--r--   0        0        0      152 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/device_digital_twins/pa_devices/__init__.py
--rw-r--r--   0        0        0    12676 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/device_digital_twins/pa_devices/ithera_msot_acuity.py
--rw-r--r--   0        0        0     3853 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/device_digital_twins/pa_devices/ithera_msot_invision.py
--rw-r--r--   0        0        0     4931 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/device_digital_twins/pa_devices/ithera_rsom.py
--rw-r--r--   0        0        0      764 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/processing_components/__init__.py
--rw-r--r--   0        0        0      152 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/processing_components/monospectral/__init__.py
--rw-r--r--   0        0        0     5333 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/processing_components/monospectral/field_of_view_cropping.py
--rw-r--r--   0        0        0    27765 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/processing_components/monospectral/iterative_qPAI_algorithm.py
--rw-r--r--   0        0        0      365 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/processing_components/monospectral/noise/__init__.py
--rw-r--r--   0        0        0     2557 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/processing_components/monospectral/noise/gamma_noise.py
--rw-r--r--   0        0        0     2976 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/processing_components/monospectral/noise/gaussian_noise.py
--rw-r--r--   0        0        0     2307 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/processing_components/monospectral/noise/poisson_noise.py
--rw-r--r--   0        0        0     2955 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/processing_components/monospectral/noise/salt_and_pepper_noise.py
--rw-r--r--   0        0        0     2690 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/processing_components/monospectral/noise/uniform_noise.py
--rw-r--r--   0        0        0     2353 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/processing_components/multispectral/__init__.py
--rw-r--r--   0        0        0    11937 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/processing_components/multispectral/linear_unmixing.py
--rw-r--r--   0        0        0     4877 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/simulation.py
--rw-r--r--   0        0        0      152 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/simulation_modules/__init__.py
--rw-r--r--   0        0        0     3351 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/simulation_modules/acoustic_forward_module/__init__.py
--rw-r--r--   0        0        0      685 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/simulation_modules/acoustic_forward_module/acoustic_forward_model_test_adapter.py
--rw-r--r--   0        0        0    18360 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/simulation_modules/acoustic_forward_module/acoustic_forward_module_k_wave_adapter.py
--rw-r--r--   0        0        0     5991 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/simulation_modules/acoustic_forward_module/simulate_2D.m
--rw-r--r--   0        0        0     6490 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/simulation_modules/acoustic_forward_module/simulate_3D.m
--rw-r--r--   0        0        0     7674 2022-08-18 14:33:22.782354 simpa-0.8.7/simpa/core/simulation_modules/optical_simulation_module/__init__.py
--rw-r--r--   0        0        0    13737 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/core/simulation_modules/optical_simulation_module/optical_forward_model_mcx_adapter.py
--rw-r--r--   0        0        0    15107 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/core/simulation_modules/optical_simulation_module/optical_forward_model_mcx_reflectance_adapter.py
--rw-r--r--   0        0        0      624 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/core/simulation_modules/optical_simulation_module/optical_forward_model_test_adapter.py
--rw-r--r--   0        0        0     6027 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/core/simulation_modules/reconstruction_module/__init__.py
--rw-r--r--   0        0        0     4771 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_delay_and_sum_adapter.py
--rw-r--r--   0        0        0     5526 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_delay_multiply_and_sum_adapter.py
--rw-r--r--   0        0        0     5621 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_signed_delay_multiply_and_sum_adapter.py
--rw-r--r--   0        0        0      445 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_test_adapter.py
--rw-r--r--   0        0        0    10940 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_time_reversal_adapter.py
--rw-r--r--   0        0        0    27121 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/core/simulation_modules/reconstruction_module/reconstruction_utils.py
--rw-r--r--   0        0        0     4140 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/core/simulation_modules/reconstruction_module/time_reversal_2D.m
--rw-r--r--   0        0        0     3953 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/core/simulation_modules/reconstruction_module/time_reversal_3D.m
--rw-r--r--   0        0        0     3189 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/core/simulation_modules/volume_creation_module/__init__.py
--rw-r--r--   0        0        0     4931 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/core/simulation_modules/volume_creation_module/volume_creation_module_model_based_adapter.py
--rw-r--r--   0        0        0     2363 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/core/simulation_modules/volume_creation_module/volume_creation_module_segmentation_based_adapter.py
--rw-r--r--   0        0        0      357 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/io_handling/__init__.py
--rw-r--r--   0        0        0     8177 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/io_handling/io_hdf5.py
--rw-r--r--   0        0        0     7737 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/io_handling/ipasc.py
--rw-r--r--   0        0        0      557 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/io_handling/serialization.py
--rw-r--r--   0        0        0     1054 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/io_handling/zenodo_download.py
--rw-r--r--   0        0        0      185 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/log/__init__.py
--rw-r--r--   0        0        0     4315 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/log/file_logger.py
--rw-r--r--   0        0        0     2962 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/__init__.py
--rw-r--r--   0        0        0     7555 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/calculate.py
--rw-r--r--   0        0        0      601 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/constants.py
--rw-r--r--   0        0        0     4064 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/deformation_manager.py
--rw-r--r--   0        0        0     4872 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/dict_path_manager.py
--rw-r--r--   0        0        0      152 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/__init__.py
--rw-r--r--   0        0        0     3412 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/absorption_spectra_data/Copper_Sulphide.npz
--rw-r--r--   0        0        0     7132 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/absorption_spectra_data/Deoxyhemoglobin.npz
--rw-r--r--   0        0        0     7132 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/absorption_spectra_data/Fat.npz
--rw-r--r--   0        0        0     7132 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/absorption_spectra_data/Melanin.npz
--rw-r--r--   0        0        0     3412 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/absorption_spectra_data/Nickel_Sulphide.npz
--rw-r--r--   0        0        0     7132 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/absorption_spectra_data/Oxyhemoglobin.npz
--rw-r--r--   0        0        0     7132 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/absorption_spectra_data/Skin_Baseline.npz
--rw-r--r--   0        0        0     7132 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/absorption_spectra_data/Water.npz
--rw-r--r--   0        0        0      258 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/absorption_spectra_data/__init__.py
--rw-r--r--   0        0        0      664 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/anisotropy_spectra_data/Epidermis_Anisotropy.npz
--rw-r--r--   0        0        0        1 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/anisotropy_spectra_data/__init__.py
--rw-r--r--   0        0        0    15838 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/literature_values.py
--rw-r--r--   0        0        0    23536 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/molecule_library.py
--rw-r--r--   0        0        0        0 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/scattering_spectra_data/__init__.py
--rw-r--r--   0        0        0     7132 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/scattering_spectra_data/background_scattering.npz
--rw-r--r--   0        0        0     7132 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/scattering_spectra_data/blood_scattering.npz
--rw-r--r--   0        0        0     7132 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/scattering_spectra_data/bone_scattering.npz
--rw-r--r--   0        0        0     7132 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/scattering_spectra_data/fat_scattering.npz
--rw-r--r--   0        0        0     7132 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/scattering_spectra_data/muscle_scattering.npz
--rw-r--r--   0        0        0     8119 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/spectrum_library.py
--rw-r--r--   0        0        0     1957 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/structure_library/BackgroundStructure.py
--rw-r--r--   0        0        0     5701 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/structure_library/CircularTubularStructure.py
--rw-r--r--   0        0        0     7317 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/structure_library/EllipticalTubularStructure.py
--rw-r--r--   0        0        0     5582 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/structure_library/HorizontalLayerStructure.py
--rw-r--r--   0        0        0     4204 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/structure_library/ParallelepipedStructure.py
--rw-r--r--   0        0        0     5643 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/structure_library/RectangularCuboidStructure.py
--rw-r--r--   0        0        0     3952 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/structure_library/SphericalStructure.py
--rw-r--r--   0        0        0     5523 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/structure_library/StructureBase.py
--rw-r--r--   0        0        0     9630 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/structure_library/VesselStructure.py
--rw-r--r--   0        0        0     3088 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/structure_library/__init__.py
--rw-r--r--   0        0        0    11795 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/libraries/tissue_library.py
--rw-r--r--   0        0        0     4841 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/path_manager.py
--rw-r--r--   0        0        0      152 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/quality_assurance/__init__.py
--rw-r--r--   0        0        0     2820 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/quality_assurance/data_sanity_testing.py
--rw-r--r--   0        0        0      424 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/serializer.py
--rw-r--r--   0        0        0     6282 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/settings.py
--rw-r--r--   0        0        0    49357 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/tags.py
--rw-r--r--   0        0        0     1627 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/utils/tissue_properties.py
--rw-r--r--   0        0        0      152 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/visualisation/__init__.py
--rw-r--r--   0        0        0    11487 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/visualisation/matplotlib_data_visualisation.py
--rw-r--r--   0        0        0     1792 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa/visualisation/matplotlib_device_visualisation.py
--rw-r--r--   0        0        0      702 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/__init__.py
--rw-r--r--   0        0        0      152 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/__init__.py
--rw-r--r--   0        0        0      152 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/device_tests/__init__.py
--rw-r--r--   0        0        0     3207 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/device_tests/test_curved_array.py
--rw-r--r--   0        0        0     2200 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/device_tests/test_linear_array.py
--rw-r--r--   0        0        0      152 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/structure_tests/__init__.py
--rw-r--r--   0        0        0     5541 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/structure_tests/test_boxes.py
--rw-r--r--   0        0        0     6709 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/structure_tests/test_elliptical_tubes.py
--rw-r--r--   0        0        0     4668 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/structure_tests/test_layers.py
--rw-r--r--   0        0        0     5959 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/structure_tests/test_parallel_epipeds.py
--rw-r--r--   0        0        0     4621 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/structure_tests/test_spheres.py
--rw-r--r--   0        0        0     5128 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/structure_tests/test_tubes.py
--rw-r--r--   0        0        0     1850 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/structure_tests/test_vesseltree.py
--rw-r--r--   0        0        0     7093 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/test_IPASC_export.py
--rw-r--r--   0        0        0     9686 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/test_bandpass_filter.py
--rw-r--r--   0        0        0     4442 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/test_calculation_utils.py
--rw-r--r--   0        0        0     1462 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/test_create_a_volume.py
--rw-r--r--   0        0        0     1931 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/test_device_UUID.py
--rw-r--r--   0        0        0     5296 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/test_io_handling.py
--rw-r--r--   0        0        0    13319 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/test_linear_unmixing.py
--rw-r--r--   0        0        0     1059 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/test_logging.py
--rw-r--r--   0        0        0    18204 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/test_noise_models.py
--rw-r--r--   0        0        0     4897 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/test_path_manager.py
--rw-r--r--   0        0        0     3299 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/test_pipeline.py
--rw-r--r--   0        0        0     4697 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/test_processing.py
--rw-r--r--   0        0        0     3137 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/test_quality_assurance.py
--rw-r--r--   0        0        0      152 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/tissue_library/__init__.py
--rw-r--r--   0        0        0     1164 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/tissue_library/test_core_assumptions.py
--rw-r--r--   0        0        0     1921 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/tissue_library/test_spectra_can_be_found.py
--rw-r--r--   0        0        0     2449 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/automatic_tests/tissue_library/test_tissue_library_against_literature_values.py
--rw-r--r--   0        0        0     1670 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/checklists/release_checklist.md
--rw-r--r--   0        0        0      744 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/do_coverage.py
--rw-r--r--   0        0        0     1643 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/full_integration_test.bat
--rw-r--r--   0        0        0    10704 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/manual_tests/__init__.py
--rw-r--r--   0        0        0    11140 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/manual_tests/acoustic_forward_models/KWaveAcousticForwardConvenienceFunction.py
--rw-r--r--   0        0        0     6534 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/manual_tests/acoustic_forward_models/MinimalKWaveTest.py
--rw-r--r--   0        0        0      152 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/manual_tests/acoustic_forward_models/__init__.py
--rw-r--r--   0        0        0    10714 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/manual_tests/digital_device_twins/SimulationWithMSOTInvision.py
--rw-r--r--   0        0        0     1139 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/manual_tests/digital_device_twins/VisualiseDevices.py
--rw-r--r--   0        0        0      152 2022-08-18 14:33:22.786354 simpa-0.8.7/simpa_tests/manual_tests/digital_device_twins/__init__.py
--rw-r--r--   0        0        0     3036 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/manual_tests/image_reconstruction/DelayAndSumReconstruction.py
--rw-r--r--   0        0        0     3085 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/manual_tests/image_reconstruction/DelayMultiplyAndSumReconstruction.py
--rw-r--r--   0        0        0    13986 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/manual_tests/image_reconstruction/PointSourceReconstruction.py
--rw-r--r--   0        0        0     3185 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/manual_tests/image_reconstruction/SignedDelayMultiplyAndSumReconstruction.py
--rw-r--r--   0        0        0     1893 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/manual_tests/image_reconstruction/TimeReversalReconstruction.py
--rw-r--r--   0        0        0      152 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/manual_tests/image_reconstruction/__init__.py
--rw-r--r--   0        0        0    13734 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/manual_tests/optical_forward_models/AbsorptionAndScatteringWithInifinitesimalSlabExperiment.py
--rw-r--r--   0        0        0    14750 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/manual_tests/optical_forward_models/AbsorptionAndScatteringWithinHomogenousMedium.py
--rw-r--r--   0        0        0     7829 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/manual_tests/optical_forward_models/CompareMCXResultsWithDiffusionTheory.py
--rw-r--r--   0        0        0     9406 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/manual_tests/optical_forward_models/ComputeDiffuseReflectance.py
--rw-r--r--   0        0        0      152 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/manual_tests/optical_forward_models/__init__.py
--rw-r--r--   0        0        0    13392 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/manual_tests/processing_components/QPAIReconstruction.py
--rw-r--r--   0        0        0     5322 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/manual_tests/processing_components/TestLinearUnmixingVisual.py
--rw-r--r--   0        0        0      152 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/manual_tests/processing_components/__init__.py
--rw-r--r--   0        0        0    14101 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/manual_tests/test_with_experimental_measurements/ReproduceDISMeasurements.py
--rw-r--r--   0        0        0      152 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/manual_tests/test_with_experimental_measurements/__init__.py
--rw-r--r--   0        0        0     5969 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_dark.rxt
--rw-r--r--   0        0        0     7652 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_dark_spectra.npz
--rw-r--r--   0        0        0     5969 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_light.rxt
--rw-r--r--   0        0        0     7652 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_light_spectra.npz
--rw-r--r--   0        0        0     5969 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/inclusion_material.rxt
--rw-r--r--   0        0        0     7652 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/inclusion_material_spectra.npz
--rw-r--r--   0        0        0     1254 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/manual_tests/test_with_experimental_measurements/utils.py
--rw-r--r--   0        0        0     5035 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/manual_tests/volume_creation/SegmentationLoader.py
--rw-r--r--   0        0        0      152 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/manual_tests/volume_creation/__init__.py
--rw-r--r--   0        0        0     5070 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/test_utils/__init__.py
--rw-r--r--   0        0        0    38791 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/test_utils/tissue_composition_tests.py
--rw-r--r--   0        0        0     2248 2022-08-18 14:33:22.790354 simpa-0.8.7/simpa_tests/test_utils/tissue_models.py
--rw-r--r--   0        0        0    14317 2022-08-18 14:38:58.871801 simpa-0.8.7/setup.py
--rw-r--r--   0        0        0    12658 2022-08-18 14:38:58.872363 simpa-0.8.7/PKG-INFO
+-rw-r--r--   0        0        0      239 2022-08-18 14:33:22.782354 simpa-0.8.9/LICENSE.md
+drwxr-xr-x   0        0        0        0 2022-08-18 14:33:22.782354 simpa-0.8.9/LICENSES/
+-rwxr-xr-x   0        0        0    11253 2022-09-23 14:43:05.747000 simpa-0.8.9/README.md
+-rw-r--r--   0        0        0     1930 2022-09-23 14:45:42.671002 simpa-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0     3314 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/__init__.py
+-rw-r--r--   0        0        0      968 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/__init__.py
+-rw-r--r--   0        0        0     1549 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/device_digital_twins/__init__.py
+-rw-r--r--   0        0        0      152 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/device_digital_twins/detection_geometries/__init__.py
+-rw-r--r--   0        0        0     5560 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/device_digital_twins/detection_geometries/curved_array.py
+-rw-r--r--   0        0        0     6116 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/device_digital_twins/detection_geometries/detection_geometry_base.py
+-rw-r--r--   0        0        0     4518 2022-09-23 14:44:49.307001 simpa-0.8.9/simpa/core/device_digital_twins/detection_geometries/linear_array.py
+-rw-r--r--   0        0        0     5497 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/device_digital_twins/detection_geometries/planar_array.py
+-rw-r--r--   0        0        0    13842 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/device_digital_twins/digital_device_twin_base.py
+-rw-r--r--   0        0        0      152 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/device_digital_twins/illumination_geometries/__init__.py
+-rw-r--r--   0        0        0     2557 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/device_digital_twins/illumination_geometries/disk_illumination.py
+-rw-r--r--   0        0        0     2666 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/device_digital_twins/illumination_geometries/gaussian_beam_illumination.py
+-rw-r--r--   0        0        0     2987 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/device_digital_twins/illumination_geometries/illumination_geometry_base.py
+-rw-r--r--   0        0        0     2347 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/device_digital_twins/illumination_geometries/ithera_msot_acuity_illumination.py
+-rw-r--r--   0        0        0     3839 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/device_digital_twins/illumination_geometries/ithera_msot_invision_illumination.py
+-rw-r--r--   0        0        0     3245 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/device_digital_twins/illumination_geometries/pencil_array_illumination.py
+-rw-r--r--   0        0        0     1515 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/device_digital_twins/illumination_geometries/pencil_beam_illumination.py
+-rw-r--r--   0        0        0     3520 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/device_digital_twins/illumination_geometries/slit_illumination.py
+-rw-r--r--   0        0        0      152 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/device_digital_twins/pa_devices/__init__.py
+-rw-r--r--   0        0        0    12676 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/device_digital_twins/pa_devices/ithera_msot_acuity.py
+-rw-r--r--   0        0        0     3853 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/device_digital_twins/pa_devices/ithera_msot_invision.py
+-rw-r--r--   0        0        0     4931 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/device_digital_twins/pa_devices/ithera_rsom.py
+-rw-r--r--   0        0        0      764 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/processing_components/__init__.py
+-rw-r--r--   0        0        0      152 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/processing_components/monospectral/__init__.py
+-rw-r--r--   0        0        0     5333 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/processing_components/monospectral/field_of_view_cropping.py
+-rw-r--r--   0        0        0    27653 2022-09-23 14:43:05.747000 simpa-0.8.9/simpa/core/processing_components/monospectral/iterative_qPAI_algorithm.py
+-rw-r--r--   0        0        0      365 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/processing_components/monospectral/noise/__init__.py
+-rw-r--r--   0        0        0     2557 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/processing_components/monospectral/noise/gamma_noise.py
+-rw-r--r--   0        0        0     2976 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/processing_components/monospectral/noise/gaussian_noise.py
+-rw-r--r--   0        0        0     2307 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/processing_components/monospectral/noise/poisson_noise.py
+-rw-r--r--   0        0        0     2955 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/processing_components/monospectral/noise/salt_and_pepper_noise.py
+-rw-r--r--   0        0        0     2690 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/processing_components/monospectral/noise/uniform_noise.py
+-rw-r--r--   0        0        0     2353 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/processing_components/multispectral/__init__.py
+-rw-r--r--   0        0        0    11830 2022-09-23 14:43:05.747000 simpa-0.8.9/simpa/core/processing_components/multispectral/linear_unmixing.py
+-rw-r--r--   0        0        0     4877 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/simulation.py
+-rw-r--r--   0        0        0      152 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/simulation_modules/__init__.py
+-rw-r--r--   0        0        0     3351 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/simulation_modules/acoustic_forward_module/__init__.py
+-rw-r--r--   0        0        0      685 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/simulation_modules/acoustic_forward_module/acoustic_forward_model_test_adapter.py
+-rw-r--r--   0        0        0    18360 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/simulation_modules/acoustic_forward_module/acoustic_forward_module_k_wave_adapter.py
+-rw-r--r--   0        0        0     5592 2022-09-23 14:44:49.307001 simpa-0.8.9/simpa/core/simulation_modules/acoustic_forward_module/simulate_2D.m
+-rw-r--r--   0        0        0     5963 2022-09-23 14:44:49.307001 simpa-0.8.9/simpa/core/simulation_modules/acoustic_forward_module/simulate_3D.m
+-rw-r--r--   0        0        0     7674 2022-08-18 14:33:22.782354 simpa-0.8.9/simpa/core/simulation_modules/optical_simulation_module/__init__.py
+-rw-r--r--   0        0        0    13737 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/core/simulation_modules/optical_simulation_module/optical_forward_model_mcx_adapter.py
+-rw-r--r--   0        0        0    15107 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/core/simulation_modules/optical_simulation_module/optical_forward_model_mcx_reflectance_adapter.py
+-rw-r--r--   0        0        0      624 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/core/simulation_modules/optical_simulation_module/optical_forward_model_test_adapter.py
+-rw-r--r--   0        0        0     6027 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/core/simulation_modules/reconstruction_module/__init__.py
+-rw-r--r--   0        0        0     4744 2022-09-23 14:44:49.307001 simpa-0.8.9/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_delay_and_sum_adapter.py
+-rw-r--r--   0        0        0     5499 2022-09-23 14:44:49.307001 simpa-0.8.9/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_delay_multiply_and_sum_adapter.py
+-rw-r--r--   0        0        0     5594 2022-09-23 14:44:49.307001 simpa-0.8.9/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_signed_delay_multiply_and_sum_adapter.py
+-rw-r--r--   0        0        0      445 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_test_adapter.py
+-rw-r--r--   0        0        0    10940 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_time_reversal_adapter.py
+-rw-r--r--   0        0        0    27620 2022-09-23 14:44:49.307001 simpa-0.8.9/simpa/core/simulation_modules/reconstruction_module/reconstruction_utils.py
+-rw-r--r--   0        0        0     4140 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/core/simulation_modules/reconstruction_module/time_reversal_2D.m
+-rw-r--r--   0        0        0     3953 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/core/simulation_modules/reconstruction_module/time_reversal_3D.m
+-rw-r--r--   0        0        0     3189 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/core/simulation_modules/volume_creation_module/__init__.py
+-rw-r--r--   0        0        0     4931 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/core/simulation_modules/volume_creation_module/volume_creation_module_model_based_adapter.py
+-rw-r--r--   0        0        0     2363 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/core/simulation_modules/volume_creation_module/volume_creation_module_segmentation_based_adapter.py
+-rw-r--r--   0        0        0      357 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/io_handling/__init__.py
+-rw-r--r--   0        0        0     8177 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/io_handling/io_hdf5.py
+-rw-r--r--   0        0        0     7737 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/io_handling/ipasc.py
+-rw-r--r--   0        0        0      557 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/io_handling/serialization.py
+-rw-r--r--   0        0        0     1054 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/io_handling/zenodo_download.py
+-rw-r--r--   0        0        0      185 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/log/__init__.py
+-rw-r--r--   0        0        0     4315 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/log/file_logger.py
+-rw-r--r--   0        0        0     2962 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/__init__.py
+-rw-r--r--   0        0        0     7555 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/calculate.py
+-rw-r--r--   0        0        0      601 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/constants.py
+-rw-r--r--   0        0        0     4064 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/deformation_manager.py
+-rw-r--r--   0        0        0     4872 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/dict_path_manager.py
+-rw-r--r--   0        0        0      152 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/__init__.py
+-rw-r--r--   0        0        0     3412 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/absorption_spectra_data/Copper_Sulphide.npz
+-rw-r--r--   0        0        0     7132 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/absorption_spectra_data/Deoxyhemoglobin.npz
+-rw-r--r--   0        0        0     7132 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/absorption_spectra_data/Fat.npz
+-rw-r--r--   0        0        0     7132 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/absorption_spectra_data/Melanin.npz
+-rw-r--r--   0        0        0     3412 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/absorption_spectra_data/Nickel_Sulphide.npz
+-rw-r--r--   0        0        0     7132 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/absorption_spectra_data/Oxyhemoglobin.npz
+-rw-r--r--   0        0        0     7132 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/absorption_spectra_data/Skin_Baseline.npz
+-rw-r--r--   0        0        0     7132 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/absorption_spectra_data/Water.npz
+-rw-r--r--   0        0        0      258 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/absorption_spectra_data/__init__.py
+-rw-r--r--   0        0        0      664 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/anisotropy_spectra_data/Epidermis_Anisotropy.npz
+-rw-r--r--   0        0        0        1 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/anisotropy_spectra_data/__init__.py
+-rw-r--r--   0        0        0    15838 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/literature_values.py
+-rw-r--r--   0        0        0    23536 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/molecule_library.py
+-rw-r--r--   0        0        0        0 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/scattering_spectra_data/__init__.py
+-rw-r--r--   0        0        0     7132 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/scattering_spectra_data/background_scattering.npz
+-rw-r--r--   0        0        0     7132 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/scattering_spectra_data/blood_scattering.npz
+-rw-r--r--   0        0        0     7132 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/scattering_spectra_data/bone_scattering.npz
+-rw-r--r--   0        0        0     7132 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/scattering_spectra_data/fat_scattering.npz
+-rw-r--r--   0        0        0     7132 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/scattering_spectra_data/muscle_scattering.npz
+-rw-r--r--   0        0        0     8119 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/spectrum_library.py
+-rw-r--r--   0        0        0     1957 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/structure_library/BackgroundStructure.py
+-rw-r--r--   0        0        0     5701 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/structure_library/CircularTubularStructure.py
+-rw-r--r--   0        0        0     7317 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/structure_library/EllipticalTubularStructure.py
+-rw-r--r--   0        0        0     5582 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/structure_library/HorizontalLayerStructure.py
+-rw-r--r--   0        0        0     4204 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/structure_library/ParallelepipedStructure.py
+-rw-r--r--   0        0        0     5643 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/structure_library/RectangularCuboidStructure.py
+-rw-r--r--   0        0        0     3952 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/structure_library/SphericalStructure.py
+-rw-r--r--   0        0        0     5523 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/structure_library/StructureBase.py
+-rw-r--r--   0        0        0     9630 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/structure_library/VesselStructure.py
+-rw-r--r--   0        0        0     3088 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/structure_library/__init__.py
+-rw-r--r--   0        0        0    11795 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/libraries/tissue_library.py
+-rw-r--r--   0        0        0     4841 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/path_manager.py
+-rw-r--r--   0        0        0     1502 2022-09-23 14:43:05.747000 simpa-0.8.9/simpa/utils/processing_device.py
+-rw-r--r--   0        0        0      152 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/quality_assurance/__init__.py
+-rw-r--r--   0        0        0     2820 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/quality_assurance/data_sanity_testing.py
+-rw-r--r--   0        0        0      424 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/serializer.py
+-rw-r--r--   0        0        0     6282 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/settings.py
+-rw-r--r--   0        0        0    49357 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/tags.py
+-rw-r--r--   0        0        0     1627 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/utils/tissue_properties.py
+-rw-r--r--   0        0        0      152 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/visualisation/__init__.py
+-rw-r--r--   0        0        0    11487 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/visualisation/matplotlib_data_visualisation.py
+-rw-r--r--   0        0        0     1792 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa/visualisation/matplotlib_device_visualisation.py
+-rw-r--r--   0        0        0      702 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/__init__.py
+-rw-r--r--   0        0        0      152 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/__init__.py
+-rw-r--r--   0        0        0      152 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/device_tests/__init__.py
+-rw-r--r--   0        0        0     3207 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/device_tests/test_curved_array.py
+-rw-r--r--   0        0        0     5471 2022-09-23 14:44:49.307001 simpa-0.8.9/simpa_tests/automatic_tests/device_tests/test_field_of_view.py
+-rw-r--r--   0        0        0     2200 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/device_tests/test_linear_array.py
+-rw-r--r--   0        0        0      152 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/structure_tests/__init__.py
+-rw-r--r--   0        0        0     5541 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/structure_tests/test_boxes.py
+-rw-r--r--   0        0        0     6709 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/structure_tests/test_elliptical_tubes.py
+-rw-r--r--   0        0        0     4668 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/structure_tests/test_layers.py
+-rw-r--r--   0        0        0     5959 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/structure_tests/test_parallel_epipeds.py
+-rw-r--r--   0        0        0     4621 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/structure_tests/test_spheres.py
+-rw-r--r--   0        0        0     5128 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/structure_tests/test_tubes.py
+-rw-r--r--   0        0        0     1850 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/structure_tests/test_vesseltree.py
+-rw-r--r--   0        0        0     7093 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/test_IPASC_export.py
+-rw-r--r--   0        0        0     9686 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/test_bandpass_filter.py
+-rw-r--r--   0        0        0     4442 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/test_calculation_utils.py
+-rw-r--r--   0        0        0     1462 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/test_create_a_volume.py
+-rw-r--r--   0        0        0     1931 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/test_device_UUID.py
+-rw-r--r--   0        0        0     5296 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/test_io_handling.py
+-rw-r--r--   0        0        0    13319 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/test_linear_unmixing.py
+-rw-r--r--   0        0        0     1059 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/test_logging.py
+-rw-r--r--   0        0        0    18204 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/test_noise_models.py
+-rw-r--r--   0        0        0     4897 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/test_path_manager.py
+-rw-r--r--   0        0        0     3299 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/test_pipeline.py
+-rw-r--r--   0        0        0     4697 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/test_processing.py
+-rw-r--r--   0        0        0     6609 2022-09-23 14:43:05.747000 simpa-0.8.9/simpa_tests/automatic_tests/test_processing_device.py
+-rw-r--r--   0        0        0     3137 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/test_quality_assurance.py
+-rw-r--r--   0        0        0      152 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/tissue_library/__init__.py
+-rw-r--r--   0        0        0     1164 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/tissue_library/test_core_assumptions.py
+-rw-r--r--   0        0        0     1921 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/tissue_library/test_spectra_can_be_found.py
+-rw-r--r--   0        0        0     2449 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/automatic_tests/tissue_library/test_tissue_library_against_literature_values.py
+-rw-r--r--   0        0        0     1670 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/checklists/release_checklist.md
+-rw-r--r--   0        0        0      744 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/do_coverage.py
+-rw-r--r--   0        0        0     1643 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/full_integration_test.bat
+-rw-r--r--   0        0        0    10704 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/manual_tests/__init__.py
+-rw-r--r--   0        0        0    11140 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/manual_tests/acoustic_forward_models/KWaveAcousticForwardConvenienceFunction.py
+-rw-r--r--   0        0        0     6534 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/manual_tests/acoustic_forward_models/MinimalKWaveTest.py
+-rw-r--r--   0        0        0      152 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/manual_tests/acoustic_forward_models/__init__.py
+-rw-r--r--   0        0        0    10714 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/manual_tests/digital_device_twins/SimulationWithMSOTInvision.py
+-rw-r--r--   0        0        0     1139 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/manual_tests/digital_device_twins/VisualiseDevices.py
+-rw-r--r--   0        0        0      152 2022-08-18 14:33:22.786354 simpa-0.8.9/simpa_tests/manual_tests/digital_device_twins/__init__.py
+-rw-r--r--   0        0        0     3036 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/manual_tests/image_reconstruction/DelayAndSumReconstruction.py
+-rw-r--r--   0        0        0     3085 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/manual_tests/image_reconstruction/DelayMultiplyAndSumReconstruction.py
+-rw-r--r--   0        0        0    13986 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/manual_tests/image_reconstruction/PointSourceReconstruction.py
+-rw-r--r--   0        0        0     3185 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/manual_tests/image_reconstruction/SignedDelayMultiplyAndSumReconstruction.py
+-rw-r--r--   0        0        0     1893 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/manual_tests/image_reconstruction/TimeReversalReconstruction.py
+-rw-r--r--   0        0        0      152 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/manual_tests/image_reconstruction/__init__.py
+-rw-r--r--   0        0        0    13734 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/manual_tests/optical_forward_models/AbsorptionAndScatteringWithInifinitesimalSlabExperiment.py
+-rw-r--r--   0        0        0    14750 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/manual_tests/optical_forward_models/AbsorptionAndScatteringWithinHomogenousMedium.py
+-rw-r--r--   0        0        0     7829 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/manual_tests/optical_forward_models/CompareMCXResultsWithDiffusionTheory.py
+-rw-r--r--   0        0        0     9406 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/manual_tests/optical_forward_models/ComputeDiffuseReflectance.py
+-rw-r--r--   0        0        0      152 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/manual_tests/optical_forward_models/__init__.py
+-rw-r--r--   0        0        0    13392 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/manual_tests/processing_components/QPAIReconstruction.py
+-rw-r--r--   0        0        0     5322 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/manual_tests/processing_components/TestLinearUnmixingVisual.py
+-rw-r--r--   0        0        0      152 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/manual_tests/processing_components/__init__.py
+-rw-r--r--   0        0        0    14101 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/manual_tests/test_with_experimental_measurements/ReproduceDISMeasurements.py
+-rw-r--r--   0        0        0      152 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/manual_tests/test_with_experimental_measurements/__init__.py
+-rw-r--r--   0        0        0     5969 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_dark.rxt
+-rw-r--r--   0        0        0     7652 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_dark_spectra.npz
+-rw-r--r--   0        0        0     5969 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_light.rxt
+-rw-r--r--   0        0        0     7652 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_light_spectra.npz
+-rw-r--r--   0        0        0     5969 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/inclusion_material.rxt
+-rw-r--r--   0        0        0     7652 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/inclusion_material_spectra.npz
+-rw-r--r--   0        0        0     1254 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/manual_tests/test_with_experimental_measurements/utils.py
+-rw-r--r--   0        0        0     5035 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/manual_tests/volume_creation/SegmentationLoader.py
+-rw-r--r--   0        0        0      152 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/manual_tests/volume_creation/__init__.py
+-rw-r--r--   0        0        0     5070 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/test_utils/__init__.py
+-rw-r--r--   0        0        0    38791 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/test_utils/tissue_composition_tests.py
+-rw-r--r--   0        0        0     2248 2022-08-18 14:33:22.790354 simpa-0.8.9/simpa_tests/test_utils/tissue_models.py
+-rw-r--r--   0        0        0    14227 1970-01-01 00:00:00.000000 simpa-0.8.9/setup.py
+-rw-r--r--   0        0        0    12565 1970-01-01 00:00:00.000000 simpa-0.8.9/PKG-INFO
```

### Comparing `simpa-0.8.7/README.md` & `simpa-0.8.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -47,17 +47,16 @@
 1. `git clone https://github.com/IMSY-DKFZ/simpa.git`
 2. `cd simpa`
 3. `git checkout main`
 4. `git pull`
 
 Now open a python instance in the 'simpa' folder that you have just downloaded. Make sure that you have your preferred
 virtual environment activated (we also recommend python 3.8)
-1. `pip install -r requirements.txt`
-2. `python setup.py install` (for developement: `python setup.py develop`)
-3. Test if the installation worked by using `python` followed by `import simpa` then `exit()`
+1. `pip install .`
+2. Test if the installation worked by using `python` followed by `import simpa` then `exit()`
 
 If no error messages arise, you are now setup to use SIMPA in your project.
 
 You can also install SIMPA with pip. Simply run:
 
 `pip install simpa`
```

### Comparing `simpa-0.8.7/pyproject.toml` & `simpa-0.8.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "simpa"
-version = "0.8.7"
+version = "0.8.9"
 description = "Simulation and Image Processing for Photonics and Acoustics"
 authors = [
     "Division of Intelligent Medical Systems (IMSY), DKFZ <k.dreher@dkfz-heidelberg.de>",
     "Janek Groehl <>"]
 license = "MIT"
 readme = "README.md"
 # requires-python = ">=3.7"
@@ -35,12 +35,17 @@
 torch = ">=1.10.0"           # Uses BSD-License (MIT compatible)
 python-dotenv = ">=0.19.2"   # Uses BSD-License (MIT compatible)
 ipasc-tool = ">=0.1.3"       # Uses BSD-License (MIT compatible)
 requests = ">=2.26.0"        # Uses Apache 2.0-License (MIT compatible)
 wget = ">=3.2"               # Is Public Domain (MIT compatible)
 jdata = ">=0.3.7"            # Uses Apache 2.0-License (MIT compatible)
 
+[tool.poetry.group.docs.dependencies]
+sphinx-rtd-theme = "^1.0.0"
+Sphinx = "^5.1.1"
+myst-parser = "^0.18.0"
+
 [build-system]
 requires = [
     "poetry >= 0.12"
 ]
 build-backend = "poetry.masonry.api"
```

### Comparing `simpa-0.8.7/simpa/__init__.py` & `simpa-0.8.9/simpa/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/__init__.py` & `simpa-0.8.9/simpa/core/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/device_digital_twins/__init__.py` & `simpa-0.8.9/simpa/core/device_digital_twins/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/device_digital_twins/detection_geometries/curved_array.py` & `simpa-0.8.9/simpa/core/device_digital_twins/detection_geometries/curved_array.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/device_digital_twins/detection_geometries/detection_geometry_base.py` & `simpa-0.8.9/simpa/core/device_digital_twins/detection_geometries/detection_geometry_base.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/device_digital_twins/detection_geometries/linear_array.py` & `simpa-0.8.9/simpa/core/device_digital_twins/detection_geometries/linear_array.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,22 +36,22 @@
         :param device_position_mm: Center of the linear array.
         """
         if field_of_view_extent_mm is None:
             field_of_view_extent_mm = np.asarray([-number_detector_elements * pitch_mm / 2,
                                                   number_detector_elements * pitch_mm / 2,
                                                   0, 0, 0, 50])
         super(LinearArrayDetectionGeometry, self).__init__(
-              number_detector_elements=number_detector_elements,
-              detector_element_width_mm=detector_element_width_mm,
-              detector_element_length_mm=detector_element_length_mm,
-              center_frequency_hz=center_frequency_hz,
-              bandwidth_percent=bandwidth_percent,
-              sampling_frequency_mhz=sampling_frequency_mhz,
-              device_position_mm=device_position_mm,
-              field_of_view_extent_mm=field_of_view_extent_mm)
+            number_detector_elements=number_detector_elements,
+            detector_element_width_mm=detector_element_width_mm,
+            detector_element_length_mm=detector_element_length_mm,
+            center_frequency_hz=center_frequency_hz,
+            bandwidth_percent=bandwidth_percent,
+            sampling_frequency_mhz=sampling_frequency_mhz,
+            device_position_mm=device_position_mm,
+            field_of_view_extent_mm=field_of_view_extent_mm)
         self.pitch_mm = pitch_mm
         self.probe_width_mm = (number_detector_elements - 1) * self.pitch_mm
 
     def check_settings_prerequisites(self, global_settings: Settings) -> bool:
         if global_settings[Tags.DIM_VOLUME_X_MM] < self.probe_width_mm + global_settings[Tags.SPACING_MM]:
             self.logger.error("Volume x dimension is too small to encompass MSOT device in simulation!"
                               "Must be at least {} mm but was {} mm"
@@ -63,16 +63,25 @@
     def update_settings_for_use_of_model_based_volume_creator(self, global_settings):
         pass
 
     def get_detector_element_positions_base_mm(self) -> np.ndarray:
 
         detector_positions = np.zeros((self.number_detector_elements, 3))
 
-        det_elements = np.arange(-int(self.number_detector_elements / 2),
-                                 int(self.number_detector_elements / 2)) * self.pitch_mm + 0.5 * self.pitch_mm
+        if self.number_detector_elements > 1:
+            if self.number_detector_elements % 2 == 0:
+                # even number of detector elements
+                det_elements = np.arange(-int(self.number_detector_elements / 2),
+                                         int(self.number_detector_elements / 2)) * self.pitch_mm + 0.5 * self.pitch_mm
+            else:
+                # odd number of detector elements
+                det_elements = np.arange(-int(self.number_detector_elements / 2),
+                                         int(self.number_detector_elements / 2) + 1) * self.pitch_mm
+        else:
+            det_elements = 0
 
         detector_positions[:, 0] = det_elements
 
         return detector_positions
 
     def get_detector_element_orientations(self) -> np.ndarray:
         detector_orientations = np.zeros((self.number_detector_elements, 3))
```

### Comparing `simpa-0.8.7/simpa/core/device_digital_twins/detection_geometries/planar_array.py` & `simpa-0.8.9/simpa/core/device_digital_twins/detection_geometries/planar_array.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/device_digital_twins/digital_device_twin_base.py` & `simpa-0.8.9/simpa/core/device_digital_twins/digital_device_twin_base.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/device_digital_twins/illumination_geometries/disk_illumination.py` & `simpa-0.8.9/simpa/core/device_digital_twins/illumination_geometries/disk_illumination.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/device_digital_twins/illumination_geometries/gaussian_beam_illumination.py` & `simpa-0.8.9/simpa/core/device_digital_twins/illumination_geometries/gaussian_beam_illumination.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/device_digital_twins/illumination_geometries/illumination_geometry_base.py` & `simpa-0.8.9/simpa/core/device_digital_twins/illumination_geometries/illumination_geometry_base.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/device_digital_twins/illumination_geometries/ithera_msot_acuity_illumination.py` & `simpa-0.8.9/simpa/core/device_digital_twins/illumination_geometries/ithera_msot_acuity_illumination.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/device_digital_twins/illumination_geometries/ithera_msot_invision_illumination.py` & `simpa-0.8.9/simpa/core/device_digital_twins/illumination_geometries/ithera_msot_invision_illumination.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/device_digital_twins/illumination_geometries/pencil_array_illumination.py` & `simpa-0.8.9/simpa/core/device_digital_twins/illumination_geometries/pencil_array_illumination.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/device_digital_twins/illumination_geometries/pencil_beam_illumination.py` & `simpa-0.8.9/simpa/core/device_digital_twins/illumination_geometries/pencil_beam_illumination.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/device_digital_twins/illumination_geometries/slit_illumination.py` & `simpa-0.8.9/simpa/core/device_digital_twins/illumination_geometries/slit_illumination.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/device_digital_twins/pa_devices/ithera_msot_acuity.py` & `simpa-0.8.9/simpa/core/device_digital_twins/pa_devices/ithera_msot_acuity.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/device_digital_twins/pa_devices/ithera_msot_invision.py` & `simpa-0.8.9/simpa/core/device_digital_twins/pa_devices/ithera_msot_invision.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/device_digital_twins/pa_devices/ithera_rsom.py` & `simpa-0.8.9/simpa/core/device_digital_twins/pa_devices/ithera_rsom.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/processing_components/__init__.py` & `simpa-0.8.9/simpa/core/processing_components/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/processing_components/monospectral/field_of_view_cropping.py` & `simpa-0.8.9/simpa/core/processing_components/monospectral/field_of_view_cropping.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/processing_components/monospectral/iterative_qPAI_algorithm.py` & `simpa-0.8.9/simpa/core/processing_components/monospectral/iterative_qPAI_algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,34 +18,34 @@
 from simpa.utils import TISSUE_LIBRARY
 from simpa.core.processing_components import ProcessingComponent
 import os
 
 
 class IterativeqPAI(ProcessingComponent):
     """
-        Applies iterative qPAI Algorithm [1] on simulated initial pressure map and saves the
-        reconstruction result in the hdf5 output file. If a 2-d map of initial_pressure is passed the algorithm saves
-        the reconstructed absorption coefficients as a 2-d map, else a 3-d absorption reconstruction is
-        saved.
-        The reconstruction result is saved as an image processing entry "iterative_qpai_result" in the hdf5 output file.
-        If intended (e.g. for testing) a list of intermediate iteration updates (only 2-d middle slices) can be saved
-        as a npy file.
-        To run the reconstruction the scattering coefficients must be known a priori.
-        :param kwargs:
-           **Tags.DOWNSCALE_FACTOR (default: 0.73)
-           **Tags.ITERATIVE_RECONSTRUCTION_CONSTANT_REGULARIZATION (default: False)
-           **Tags.ITERATIVE_RECONSTRUCTION_MAX_ITERATION_NUMBER (default: 10)
-           **Tags.ITERATIVE_RECONSTRUCTION_REGULARIZATION_SIGMA (default: 0.01)
-           **Tags.ITERATIVE_RECONSTRUCTION_SAVE_INTERMEDIATE_RESULTS (default: False)
-           **Tags.ITERATIVE_RECONSTRUCTION_STOPPING_LEVEL (default: 0.03)
-           **settings (required)
-           **component_settings_key (required)
+    Applies iterative qPAI Algorithm [1] on simulated initial pressure map and saves the
+    reconstruction result in the hdf5 output file. If a 2-d map of initial_pressure is passed the algorithm saves
+    the reconstructed absorption coefficients as a 2-d map, else a 3-d absorption reconstruction is
+    saved.
+    The reconstruction result is saved as an image processing entry "iterative_qpai_result" in the hdf5 output file.
+    If intended (e.g. for testing) a list of intermediate iteration updates (only 2-d middle slices) can be saved
+    as a npy file.
+    To run the reconstruction the scattering coefficients must be known a priori.
+    Parameters:
+    Tags.DOWNSCALE_FACTOR (default: 0.73)
+    Tags.ITERATIVE_RECONSTRUCTION_CONSTANT_REGULARIZATION (default: False)
+    Tags.ITERATIVE_RECONSTRUCTION_MAX_ITERATION_NUMBER (default: 10)
+    Tags.ITERATIVE_RECONSTRUCTION_REGULARIZATION_SIGMA (default: 0.01)
+    Tags.ITERATIVE_RECONSTRUCTION_SAVE_INTERMEDIATE_RESULTS (default: False)
+    Tags.ITERATIVE_RECONSTRUCTION_STOPPING_LEVEL (default: 0.03)
+    global_settings (required)
+    component_settings_key (required)
 
-        [1] B. T. Cox et al. 2006, "Two-dimensional quantitative photoacoustic image reconstruction of absorption
-        distributions in scattering media by use of a simple iterative method", https://doi.org/10.1364/ao.45.001866
+    [1] B. T. Cox et al. 2006, "Two-dimensional quantitative photoacoustic image reconstruction of absorption
+    distributions in scattering media by use of a simple iterative method", https://doi.org/10.1364/ao.45.001866
     """
 
     def __init__(self, global_settings, component_settings_key: str):
         super(ProcessingComponent, self).__init__(global_settings=global_settings)
 
         self.global_settings = global_settings
         self.optical_settings = global_settings.get_optical_settings()
```

### Comparing `simpa-0.8.7/simpa/core/processing_components/monospectral/noise/gamma_noise.py` & `simpa-0.8.9/simpa/core/processing_components/monospectral/noise/gamma_noise.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/processing_components/monospectral/noise/gaussian_noise.py` & `simpa-0.8.9/simpa/core/processing_components/monospectral/noise/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/processing_components/monospectral/noise/poisson_noise.py` & `simpa-0.8.9/simpa/core/processing_components/monospectral/noise/poisson_noise.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/processing_components/monospectral/noise/salt_and_pepper_noise.py` & `simpa-0.8.9/simpa/core/processing_components/monospectral/noise/salt_and_pepper_noise.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/processing_components/monospectral/noise/uniform_noise.py` & `simpa-0.8.9/simpa/core/processing_components/monospectral/noise/uniform_noise.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/processing_components/multispectral/__init__.py` & `simpa-0.8.9/simpa/core/processing_components/multispectral/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/processing_components/multispectral/linear_unmixing.py` & `simpa-0.8.9/simpa/core/processing_components/multispectral/linear_unmixing.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,36 +9,36 @@
 import numpy as np
 import scipy.linalg as linalg
 from scipy.optimize import nnls
 
 
 class LinearUnmixing(MultispectralProcessingAlgorithm):
     """
-        Performs linear spectral unmixing (LU) using Fast Linear Unmixing for PhotoAcoustic Imaging (FLUPAI)
-        on the defined data field for each chromophore specified in the component settings.
+    Performs linear spectral unmixing (LU) using Fast Linear Unmixing for PhotoAcoustic Imaging (FLUPAI)
+    on the defined data field for each chromophore specified in the component settings.
 
-        If tag LINEAR_UNMIXING_NON_NEGATIVE is set to True non-negative linear unmixing is performed, which solves the
-        KKT (Karush-Kuhn-Tucker) conditions for the non-negative least squares problem.
+    If tag LINEAR_UNMIXING_NON_NEGATIVE is set to True non-negative linear unmixing is performed, which solves the
+    KKT (Karush-Kuhn-Tucker) conditions for the non-negative least squares problem.
 
-        This component saves a dictionary containing the chromophore concentrations and corresponding wavelengths for
-        each chromophore. If the tag LINEAR_UNMIXING_COMPUTE_SO2 is set True the blood oxygen saturation
-        is saved as well, however, this is only possible if the chromophores oxy- and deoxyhemoglobin are specified.
-        IMPORTANT:
-        Linear unmixing should only be performed with at least two wavelengths:
-        e.g. Tags.WAVELENGTHS: [750, 800]
-
-        :param kwargs:
-           **Tags.DATA_FIELD (required)
-           **Tags.LINEAR_UNMIXING_SPECTRA (required)
-           **Tags.WAVELENGTHS (default: None, if None, then settings[Tags.WAVELENGTHS] will be used.)
-           **Tags.LINEAR_UNMIXING_COMPUTE_SO2 (default: False)
-           **Tags.LINEAR_UNMIXING_NON_NEGATIVE (default: False)
-           **settings (required)
-           **component_settings_key (required)
-        """
+    This component saves a dictionary containing the chromophore concentrations and corresponding wavelengths for
+    each chromophore. If the tag LINEAR_UNMIXING_COMPUTE_SO2 is set True the blood oxygen saturation
+    is saved as well, however, this is only possible if the chromophores oxy- and deoxyhemoglobin are specified.
+    IMPORTANT:
+    Linear unmixing should only be performed with at least two wavelengths:
+    e.g. Tags.WAVELENGTHS: [750, 800]
+
+    Parameters:
+    Tags.DATA_FIELD (required)
+    Tags.LINEAR_UNMIXING_SPECTRA (required)
+    Tags.WAVELENGTHS (default: None, if None, then settings[Tags.WAVELENGTHS] will be used.)
+    Tags.LINEAR_UNMIXING_COMPUTE_SO2 (default: False)
+    Tags.LINEAR_UNMIXING_NON_NEGATIVE (default: False)
+    global_settings (required)
+    component_settings_key (required)
+    """
 
     def __init__(self, global_settings, component_settings_key: str):
         super(LinearUnmixing, self).__init__(global_settings=global_settings,
                                              component_settings_key=component_settings_key)
 
         self.chromophore_spectra_dict = {}  # dictionary containing the spectrum for each chromophore and wavelength
         self.absorption_matrix = []  # endmember matrix needed in LU
```

### Comparing `simpa-0.8.7/simpa/core/simulation.py` & `simpa-0.8.9/simpa/core/simulation.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/simulation_modules/acoustic_forward_module/__init__.py` & `simpa-0.8.9/simpa/core/simulation_modules/acoustic_forward_module/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/simulation_modules/acoustic_forward_module/acoustic_forward_model_test_adapter.py` & `simpa-0.8.9/simpa/core/simulation_modules/acoustic_forward_module/acoustic_forward_model_test_adapter.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/simulation_modules/acoustic_forward_module/acoustic_forward_module_k_wave_adapter.py` & `simpa-0.8.9/simpa/core/simulation_modules/acoustic_forward_module/acoustic_forward_module_k_wave_adapter.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/simulation_modules/acoustic_forward_module/simulate_2D.m` & `simpa-0.8.9/simpa/core/simulation_modules/acoustic_forward_module/simulate_3D.m`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 %%SPDX-FileCopyrightText: 2021 Division of Intelligent Medical Systems, DKFZ
 %%SPDX-FileCopyrightText: 2021 Janek Groehl
 %%SPDX-License-Identifier: MIT
 
-function [] = simulate_2D(optical_path)
+function [] = simulate_3D(optical_path)
 
 %% In case of an error, make sure the matlab scripts exits anyway
 clean_up = onCleanup(@exit);
 
 %% Read settings file
 
 data = load(optical_path);
@@ -21,129 +21,115 @@
     p0_smoothing = settings.initial_pressure_smoothing;
 else
     p0_smoothing = true;
 end
 
 %% Define kWaveGrid
 
-% add N pixel "gel" to reduce Fourier artifact
+% add 2 pixel "gel" to reduce Fourier artifact
 GEL_LAYER_HEIGHT = 3;
 
-source.p0 = padarray(source.p0, [GEL_LAYER_HEIGHT 0], 0, 'pre');
-[Nx, Ny] = size(source.p0);
-disp(Nx);
-disp(Ny);
+%source.p0 = padarray(source.p0, [GEL_LAYER_HEIGHT 0], 0, 'pre');
+[Nx, Ny, Nz] = size(source.p0);
 if isfield(settings, 'sample') == true
     if settings.sample == true
-        dx = double(settings.voxel_spacing_mm) / (double(settings.upscale_factor) * 1000);
+        dx = double(settings.voxel_spacing_mm)/(double(settings.upscale_factor) * 1000);
     else
-        dx = double(settings.voxel_spacing_mm) / 1000;    % convert from mm to m
+        dx = double(settings.voxel_spacing_mm)/1000;    % convert from mm to m
     end
 else
-    dx = double(settings.voxel_spacing_mm) / 1000;    % convert from mm to m
+    dx = double(settings.voxel_spacing_mm)/1000;    % convert from mm to m
 end
-kgrid = kWaveGrid(Nx, dx, Ny, dx);
+kgrid = kWaveGrid(Nx, dx, Ny, dx, Nz, dx);
 
 %% Define medium
 
 % if a field of the struct "data" is given which describes the sound speed, the array is loaded and is used as medium.sound_speed
 if isfield(data, 'sos') == true
     medium.sound_speed = data.sos;
-    medium.sound_speed = padarray(medium.sound_speed, [GEL_LAYER_HEIGHT 0], 'replicate', 'pre');
+    % add 2 pixel "gel" to reduce Fourier artifact
+%    medium.sound_speed = padarray(medium.sound_speed, [GEL_LAYER_HEIGHT 0], 'replicate', 'pre');
 else
     medium.sound_speed = 1540;
 end
 
 % if a field of the struct "data" is given which describes the attenuation, the array is loaded and is used as medium.alpha_coeff
 if isfield(data, 'alpha_coeff') == true
  medium.alpha_coeff = data.alpha_coeff;
- medium.alpha_coeff = padarray(medium.alpha_coeff, [GEL_LAYER_HEIGHT 0], 'replicate', 'pre');
+ % add 2 pixel "gel" to reduce Fourier artifact
+% medium.alpha_coeff = padarray(medium.alpha_coeff, [GEL_LAYER_HEIGHT 0], 'replicate', 'pre');
 else
  medium.alpha_coeff = 0.01;
 end
 
 medium.alpha_power = double(settings.medium_alpha_power); % b for a * MHz ^ b
 medium.alpha_mode = 'no_dispersion';
 
 % if a field of the struct "data" is given which describes the density, the array is loaded and is used as medium.density
 if isfield(data, 'density') == true
     medium.density = data.density;
-    medium.density = padarray(medium.density, [GEL_LAYER_HEIGHT 0], 'replicate', 'pre');
+    % add 2 pixel "gel" to reduce Fourier artifact
+%    medium.density = padarray(medium.density, [GEL_LAYER_HEIGHT 0], 'replicate', 'pre');
 else
-    medium.density = 1000 * ones(Nx, Ny);
+    medium.density = 1000*ones(Nx, Ny, Nz);
 end
 
 %% Sampling rate
 
 % load sampling rate from settings
 dt = 1.0 / double(settings.sensor_sampling_rate_mhz * 1000000);
 
 % Simulate as many time steps as a wave takes to traverse diagonally through the entire tissue
-Nt = round((sqrt(Ny*Ny+Nx*Nx)*dx / mean(medium.sound_speed, 'all')) / dt);
+Nt = round((sqrt(Ny*Ny+Nx*Nx+Nz*Nz)*dx / mean(medium.sound_speed, 'all')) / dt);
 
 estimated_cfl_number = dt / dx * mean(medium.sound_speed, 'all');
-disp(estimated_cfl_number);
 
 % smaller time steps are better for numerical stability in time progressing simulations
 % A minimum CFL of 0.3 is advised in the kwave handbook.
 % In case we specify something larger, we use a higher sampling rate than anticipated.
 % Otherwise we simulate with the target sampling rate
 if estimated_cfl_number < 0.3
     kgrid.setTime(Nt, dt);
-    disp("Setting custom time!");
 else
     kgrid.t_array = makeTime(kgrid, medium.sound_speed, 0.3);
-    disp("Making time!");
 end
 
 %% Define sensor
 
 % create empty array
 karray = kWaveArray;
 
 elem_pos = data.sensor_element_positions/1000;
 
-% In case some detectors are defined at zeros or with negative values out
-% of bounds, correct all of them with minimum needed correction of
-% spacing dx.
-
-min_x_pos = find(elem_pos(1, :) <= 0);
-min_y_pos = find(elem_pos(2, :) <= 0);
-x_correction = 0;
-y_correction = 0;
-if size(min_x_pos) > 0
-   x_correction = dx;
-end
-
-if size(min_y_pos) > 0
-   y_correction = dx;
-end
-
-elem_pos(1, :) = elem_pos(1, :) - 0.5 * kgrid.x_size + x_correction + dx * GEL_LAYER_HEIGHT;
-elem_pos(2, :) = elem_pos(2, :) - 0.5 * kgrid.y_size + y_correction;
-
+elem_pos(1, :) = elem_pos(1, :) - 0.5 * kgrid.x_size + dx * GEL_LAYER_HEIGHT;
+elem_pos(2, :) = elem_pos(2, :) - 0.5 * kgrid.y_size;
+elem_pos(3, :) = elem_pos(3, :) - 0.5 * kgrid.z_size;
 num_elements = size(elem_pos, 2);
 
 element_width = double(settings.detector_element_width_mm)/1000;
-angles = data.directivity_angle;
+orientation_angles = data.directivity_angle;
+euler_angles = data.intrinsic_euler_angle;
 
 if isfield(settings, 'sensor_radius_mm') == true
     radius_of_curv = double(settings.sensor_radius_mm)/1000;
 end
 
+% For addArcElement orient all elements towards the focus
+% For the iThera MSOT Acuity Echo, it is [0.008, 0]
+
+%focus_pos = [0.008, 0];
 
 % add elements to the array
 
+%for ind = 1:num_elements
+%    karray.addArcElement(elem_pos(:, ind), radius_of_curv, element_width, focus_pos);
+%end
 for ind = 1:num_elements
-  x = elem_pos(1, ind);
-  y = elem_pos(2, ind);
-  alpha = angles(1, ind);
-  x = x + 0.5 * (element_width*sin(alpha));
-  y = y + 0.5 * (element_width*cos(alpha));
-  karray.addRectElement([x, y], element_width, 0.00001, [angles(1, ind)]);
+  elem_pos(:, ind) = elem_pos(:, ind) - 0.5*(element_width*sind(orientation_angles(:, ind)));
+  karray.addRectElement(elem_pos(:, ind), element_width, 0.0001, euler_angles(ind, :));
 end
 
 % assign binary mask from karray to the sensor mask
 sensor.mask = karray.getArrayBinaryMask(kgrid);
 
 % model sensor frequency response
 if isfield(settings, 'model_sensor_frequency_response') == true
@@ -159,29 +145,29 @@
 if settings.gpu == true
     datacast = 'gpuArray-single';
 else
     datacast = 'single';
 end
 
 input_args = {'DataCast', datacast, 'PMLInside', settings.pml_inside, ...
-               'PMLAlpha', settings.pml_alpha, 'PMLSize', 'auto', ...
-               'PlotPML', settings.plot_pml, 'RecordMovie', settings.record_movie, ...
-               'MovieName', settings.movie_name, 'PlotScale', [-1, 1], 'LogScale', settings.acoustic_log_scale, ...
-               'Smooth', p0_smoothing};
+              'PMLAlpha', double(settings.pml_alpha), 'PMLSize', 'auto', ...
+              'PlotPML', settings.plot_pml, 'RecordMovie', settings.record_movie, ...
+              'MovieName', settings.movie_name, 'PlotScale', [-1, 1], 'LogScale', settings.acoustic_log_scale, ...
+              'Smooth', p0_smoothing};
 
 if settings.gpu == true
-    time_series_data = kspaceFirstOrder2DG(kgrid, medium, source, sensor, input_args{:});
+    time_series_data = kspaceFirstOrder3DG(kgrid, medium, source, sensor, input_args{:});
     time_series_data = gather(time_series_data);
 else
-    time_series_data = kspaceFirstOrder2D(kgrid, medium, source, sensor, input_args{:});
+    time_series_data = kspaceFirstOrder3D(kgrid, medium, source, sensor, input_args{:});
 end
 
 % combine data to give one trace per physical array element
 time_series_data = karray.combineSensorData(kgrid, time_series_data);
 
 %% Write data to mat array
 save(optical_path, 'time_series_data')%, '-v7.3')
-time_step = kgrid.dt
-number_time_steps = kgrid.Nt
+time_step = kgrid.dt;
+number_time_steps = kgrid.Nt;
 save(strcat(optical_path, 'dt.mat'), 'time_step', 'number_time_steps');
 
-end
+end
```

### Comparing `simpa-0.8.7/simpa/core/simulation_modules/acoustic_forward_module/simulate_3D.m` & `simpa-0.8.9/simpa/core/simulation_modules/acoustic_forward_module/simulate_2D.m`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 %%SPDX-FileCopyrightText: 2021 Division of Intelligent Medical Systems, DKFZ
 %%SPDX-FileCopyrightText: 2021 Janek Groehl
 %%SPDX-License-Identifier: MIT
 
-function [] = simulate_3D(optical_path)
+function [] = simulate_2D(optical_path)
 
 %% In case of an error, make sure the matlab scripts exits anyway
 clean_up = onCleanup(@exit);
 
 %% Read settings file
 
 data = load(optical_path);
@@ -21,138 +21,114 @@
     p0_smoothing = settings.initial_pressure_smoothing;
 else
     p0_smoothing = true;
 end
 
 %% Define kWaveGrid
 
-% add 2 pixel "gel" to reduce Fourier artifact
+% add N pixel "gel" to reduce Fourier artifact
 GEL_LAYER_HEIGHT = 3;
 
-%source.p0 = padarray(source.p0, [GEL_LAYER_HEIGHT 0], 0, 'pre');
-[Nx, Ny, Nz] = size(source.p0);
+source.p0 = padarray(source.p0, [GEL_LAYER_HEIGHT 0], 0, 'pre');
+[Nx, Ny] = size(source.p0);
+disp(Nx);
+disp(Ny);
 if isfield(settings, 'sample') == true
     if settings.sample == true
-        dx = double(settings.voxel_spacing_mm)/(double(settings.upscale_factor) * 1000);
+        dx = double(settings.voxel_spacing_mm) / (double(settings.upscale_factor) * 1000);
     else
-        dx = double(settings.voxel_spacing_mm)/1000;    % convert from mm to m
+        dx = double(settings.voxel_spacing_mm) / 1000;    % convert from mm to m
     end
 else
-    dx = double(settings.voxel_spacing_mm)/1000;    % convert from mm to m
+    dx = double(settings.voxel_spacing_mm) / 1000;    % convert from mm to m
 end
-kgrid = kWaveGrid(Nx, dx, Ny, dx, Nz, dx);
+kgrid = kWaveGrid(Nx, dx, Ny, dx);
 
 %% Define medium
 
 % if a field of the struct "data" is given which describes the sound speed, the array is loaded and is used as medium.sound_speed
 if isfield(data, 'sos') == true
     medium.sound_speed = data.sos;
-    % add 2 pixel "gel" to reduce Fourier artifact
-%    medium.sound_speed = padarray(medium.sound_speed, [GEL_LAYER_HEIGHT 0], 'replicate', 'pre');
+    medium.sound_speed = padarray(medium.sound_speed, [GEL_LAYER_HEIGHT 0], 'replicate', 'pre');
 else
     medium.sound_speed = 1540;
 end
 
 % if a field of the struct "data" is given which describes the attenuation, the array is loaded and is used as medium.alpha_coeff
 if isfield(data, 'alpha_coeff') == true
  medium.alpha_coeff = data.alpha_coeff;
- % add 2 pixel "gel" to reduce Fourier artifact
-% medium.alpha_coeff = padarray(medium.alpha_coeff, [GEL_LAYER_HEIGHT 0], 'replicate', 'pre');
+ medium.alpha_coeff = padarray(medium.alpha_coeff, [GEL_LAYER_HEIGHT 0], 'replicate', 'pre');
 else
  medium.alpha_coeff = 0.01;
 end
 
 medium.alpha_power = double(settings.medium_alpha_power); % b for a * MHz ^ b
 medium.alpha_mode = 'no_dispersion';
 
 % if a field of the struct "data" is given which describes the density, the array is loaded and is used as medium.density
 if isfield(data, 'density') == true
     medium.density = data.density;
-    % add 2 pixel "gel" to reduce Fourier artifact
-%    medium.density = padarray(medium.density, [GEL_LAYER_HEIGHT 0], 'replicate', 'pre');
+    medium.density = padarray(medium.density, [GEL_LAYER_HEIGHT 0], 'replicate', 'pre');
 else
-    medium.density = 1000*ones(Nx, Ny, Nz);
+    medium.density = 1000 * ones(Nx, Ny);
 end
 
 %% Sampling rate
 
 % load sampling rate from settings
 dt = 1.0 / double(settings.sensor_sampling_rate_mhz * 1000000);
 
 % Simulate as many time steps as a wave takes to traverse diagonally through the entire tissue
-Nt = round((sqrt(Ny*Ny+Nx*Nx+Nz*Nz)*dx / mean(medium.sound_speed, 'all')) / dt);
+Nt = round((sqrt(Ny*Ny+Nx*Nx)*dx / mean(medium.sound_speed, 'all')) / dt);
 
 estimated_cfl_number = dt / dx * mean(medium.sound_speed, 'all');
+disp(estimated_cfl_number);
 
 % smaller time steps are better for numerical stability in time progressing simulations
 % A minimum CFL of 0.3 is advised in the kwave handbook.
 % In case we specify something larger, we use a higher sampling rate than anticipated.
 % Otherwise we simulate with the target sampling rate
 if estimated_cfl_number < 0.3
     kgrid.setTime(Nt, dt);
+    disp("Setting custom time!");
 else
     kgrid.t_array = makeTime(kgrid, medium.sound_speed, 0.3);
+    disp("Making time!");
 end
 
 %% Define sensor
 
 % create empty array
 karray = kWaveArray;
 
 elem_pos = data.sensor_element_positions/1000;
 
-% In case some detectors are defined at zeros or with negative values out
-% of bounds, correct all of them with minimum needed correction of the
-% spacing dx.
-
-min_x_pos = find(elem_pos(1, :) <= 0);
-min_y_pos = find(elem_pos(2, :) <= 0);
-min_z_pos = find(elem_pos(3, :) <= 0);
-x_correction = 0;
-y_correction = 0;
-z_correction = 0;
-if size(min_x_pos) > 0
-   x_correction = dx;
-end
-
-if size(min_y_pos) > 0
-   y_correction = dx;
-end
-
-if size(min_z_pos) > 0
-   z_correction = dx;
-end
 
+elem_pos(1, :) = elem_pos(1, :) - 0.5 * kgrid.x_size + dx * GEL_LAYER_HEIGHT;
+elem_pos(2, :) = elem_pos(2, :) - 0.5 * kgrid.y_size;
 
-elem_pos(1, :) = elem_pos(1, :) - 0.5 * kgrid.x_size + x_correction + dx * GEL_LAYER_HEIGHT;
-elem_pos(2, :) = elem_pos(2, :) - 0.5 * kgrid.y_size + y_correction;
-elem_pos(3, :) = elem_pos(3, :) - 0.5 * kgrid.z_size + z_correction;
 num_elements = size(elem_pos, 2);
 
 element_width = double(settings.detector_element_width_mm)/1000;
-orientation_angles = data.directivity_angle;
-euler_angles = data.intrinsic_euler_angle;
+angles = data.directivity_angle;
 
 if isfield(settings, 'sensor_radius_mm') == true
     radius_of_curv = double(settings.sensor_radius_mm)/1000;
 end
 
-% For addArcElement orient all elements towards the focus
-% For the iThera MSOT Acuity Echo, it is [0.008, 0]
-
-%focus_pos = [0.008, 0];
 
 % add elements to the array
 
-%for ind = 1:num_elements
-%    karray.addArcElement(elem_pos(:, ind), radius_of_curv, element_width, focus_pos);
-%end
 for ind = 1:num_elements
-  elem_pos(:, ind) = elem_pos(:, ind) - 0.5*(element_width*sind(orientation_angles(:, ind)));
-  karray.addRectElement(elem_pos(:, ind), element_width, 0.0001, euler_angles(ind, :));
+  x = elem_pos(1, ind);
+  y = elem_pos(2, ind);
+  alpha = angles(1, ind);
+  x = x + 0.5 * (element_width*sin(alpha));
+  y = y + 0.5 * (element_width*cos(alpha));
+  karray.addRectElement([x, y], element_width, 0.00001, [angles(1, ind)]);
 end
 
 % assign binary mask from karray to the sensor mask
 sensor.mask = karray.getArrayBinaryMask(kgrid);
 
 % model sensor frequency response
 if isfield(settings, 'model_sensor_frequency_response') == true
@@ -168,29 +144,29 @@
 if settings.gpu == true
     datacast = 'gpuArray-single';
 else
     datacast = 'single';
 end
 
 input_args = {'DataCast', datacast, 'PMLInside', settings.pml_inside, ...
-              'PMLAlpha', double(settings.pml_alpha), 'PMLSize', 'auto', ...
-              'PlotPML', settings.plot_pml, 'RecordMovie', settings.record_movie, ...
-              'MovieName', settings.movie_name, 'PlotScale', [-1, 1], 'LogScale', settings.acoustic_log_scale, ...
-              'Smooth', p0_smoothing};
+               'PMLAlpha', settings.pml_alpha, 'PMLSize', 'auto', ...
+               'PlotPML', settings.plot_pml, 'RecordMovie', settings.record_movie, ...
+               'MovieName', settings.movie_name, 'PlotScale', [-1, 1], 'LogScale', settings.acoustic_log_scale, ...
+               'Smooth', p0_smoothing};
 
 if settings.gpu == true
-    time_series_data = kspaceFirstOrder3DG(kgrid, medium, source, sensor, input_args{:});
+    time_series_data = kspaceFirstOrder2DG(kgrid, medium, source, sensor, input_args{:});
     time_series_data = gather(time_series_data);
 else
-    time_series_data = kspaceFirstOrder3D(kgrid, medium, source, sensor, input_args{:});
+    time_series_data = kspaceFirstOrder2D(kgrid, medium, source, sensor, input_args{:});
 end
 
 % combine data to give one trace per physical array element
 time_series_data = karray.combineSensorData(kgrid, time_series_data);
 
 %% Write data to mat array
 save(optical_path, 'time_series_data')%, '-v7.3')
-time_step = kgrid.dt;
-number_time_steps = kgrid.Nt;
+time_step = kgrid.dt
+number_time_steps = kgrid.Nt
 save(strcat(optical_path, 'dt.mat'), 'time_step', 'number_time_steps');
 
-end
+end
```

### Comparing `simpa-0.8.7/simpa/core/simulation_modules/optical_simulation_module/__init__.py` & `simpa-0.8.9/simpa/core/simulation_modules/optical_simulation_module/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/simulation_modules/optical_simulation_module/optical_forward_model_mcx_adapter.py` & `simpa-0.8.9/simpa/core/simulation_modules/optical_simulation_module/optical_forward_model_mcx_adapter.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/simulation_modules/optical_simulation_module/optical_forward_model_mcx_reflectance_adapter.py` & `simpa-0.8.9/simpa/core/simulation_modules/optical_simulation_module/optical_forward_model_mcx_reflectance_adapter.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/simulation_modules/optical_simulation_module/optical_forward_model_test_adapter.py` & `simpa-0.8.9/simpa/core/simulation_modules/optical_simulation_module/optical_forward_model_test_adapter.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/simulation_modules/reconstruction_module/__init__.py` & `simpa-0.8.9/simpa/core/simulation_modules/reconstruction_module/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_delay_and_sum_adapter.py` & `simpa-0.8.9/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_delay_and_sum_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
         time_series_sensor_data, sensor_positions, speed_of_sound_in_m_per_s, spacing_in_mm, time_spacing_in_ms, torch_device = preparing_reconstruction_and_obtaining_reconstruction_settings(
             time_series_sensor_data, self.component_settings, self.global_settings, detection_geometry, self.logger)
 
         ### ALGORITHM ITSELF ###
 
         xdim, zdim, ydim, xdim_start, xdim_end, ydim_start, ydim_end, zdim_start, zdim_end = compute_image_dimensions(
-            detection_geometry, spacing_in_mm, speed_of_sound_in_m_per_s, self.logger)
+            detection_geometry, spacing_in_mm, self.logger)
 
         if zdim == 1:
             sensor_positions[:, 1] = 0  # Assume imaging plane
 
         # construct output image
         output = torch.zeros((xdim, ydim, zdim), dtype=torch.float32, device=torch_device)
```

### Comparing `simpa-0.8.7/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_delay_multiply_and_sum_adapter.py` & `simpa-0.8.9/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_delay_multiply_and_sum_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
         time_series_sensor_data, sensor_positions, speed_of_sound_in_m_per_s, spacing_in_mm, time_spacing_in_ms, torch_device = preparing_reconstruction_and_obtaining_reconstruction_settings(
             time_series_sensor_data, self.component_settings, self.global_settings, detection_geometry, self.logger)
 
         ### ALGORITHM ITSELF ###
 
         xdim, zdim, ydim, xdim_start, xdim_end, ydim_start, ydim_end, zdim_start, zdim_end = compute_image_dimensions(
-            detection_geometry, spacing_in_mm, speed_of_sound_in_m_per_s, self.logger)
+            detection_geometry, spacing_in_mm, self.logger)
 
         if zdim == 1:
             sensor_positions[:, 1] = 0  # Assume imaging plane
 
         # construct output image
         output = torch.zeros((xdim, ydim, zdim), dtype=torch.float32, device=torch_device)
```

### Comparing `simpa-0.8.7/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_signed_delay_multiply_and_sum_adapter.py` & `simpa-0.8.9/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_signed_delay_multiply_and_sum_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
         time_series_sensor_data, sensor_positions, speed_of_sound_in_m_per_s, spacing_in_mm, time_spacing_in_ms, torch_device = preparing_reconstruction_and_obtaining_reconstruction_settings(
             time_series_sensor_data, self.component_settings, self.global_settings, detection_geometry, self.logger)
 
         ### ALGORITHM ITSELF ###
 
         xdim, zdim, ydim, xdim_start, xdim_end, ydim_start, ydim_end, zdim_start, zdim_end = compute_image_dimensions(
-            detection_geometry, spacing_in_mm, speed_of_sound_in_m_per_s, self.logger)
+            detection_geometry, spacing_in_mm, self.logger)
 
         if zdim == 1:
             sensor_positions[:, 1] = 0  # Assume imaging plane
 
         # construct output image
         output = torch.zeros((xdim, ydim, zdim), dtype=torch.float32, device=torch_device)
```

### Comparing `simpa-0.8.7/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_time_reversal_adapter.py` & `simpa-0.8.9/simpa/core/simulation_modules/reconstruction_module/reconstruction_module_time_reversal_adapter.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/simulation_modules/reconstruction_module/reconstruction_utils.py` & `simpa-0.8.9/simpa/core/simulation_modules/reconstruction_module/reconstruction_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # SPDX-FileCopyrightText: 2021 Division of Intelligent Medical Systems, DKFZ
 # SPDX-FileCopyrightText: 2021 Janek Groehl
 # SPDX-License-Identifier: MIT
 
 from typing import Tuple
 from simpa.log.file_logger import Logger
 from simpa.core.device_digital_twins import DetectionGeometryBase
+from simpa.utils.processing_device import get_processing_device
 from simpa.utils.settings import Settings
 from simpa.io_handling.io_hdf5 import load_data_field
 from simpa.utils import Tags
 import torch
 import torch.fft
 from torch import Tensor
 import numpy as np
@@ -45,37 +46,39 @@
         output = hamming.expand(dimensions + (n_sensor_elements,))
     # box window apodization as default
     else:
         output = torch.ones(dimensions + (n_sensor_elements,), device=device)
 
     return output
 
+
 def bandpass_filter_with_settings(data: np.ndarray, global_settings: Settings, component_settings: Settings,
-                                           device: DetectionGeometryBase) -> np.ndarray:
-        """
-        Applies corresponding bandpass filter which can be set in 
-        `component_settings[Tags.BANDPASS_FILTER_METHOD]`, using Tukey window-based filter as default.
+                                  device: DetectionGeometryBase) -> np.ndarray:
+    """
+    Applies corresponding bandpass filter which can be set in 
+    `component_settings[Tags.BANDPASS_FILTER_METHOD]`, using Tukey window-based filter as default.
 
-        :param data: (numpy array) data to be filtered
-        :param global_settings: (Settings) settings for the whole simulation
-        :param component_settings: (Settings) settings for the reconstruction module
-        :param device:
-        :return: (numpy array) filtered data
-        """
+    :param data: (numpy array) data to be filtered
+    :param global_settings: (Settings) settings for the whole simulation
+    :param component_settings: (Settings) settings for the reconstruction module
+    :param device:
+    :return: (numpy array) filtered data
+    """
 
-        # select corresponding filtering method depending on tag in settings
-        if Tags.BANDPASS_FILTER_METHOD in component_settings:
-            if component_settings[Tags.BANDPASS_FILTER_METHOD] == Tags.TUKEY_BANDPASS_FILTER:
-                return tukey_bandpass_filtering_with_settings(data, global_settings,component_settings, device)
-            elif component_settings[Tags.BANDPASS_FILTER_METHOD] == Tags.BUTTERWORTH_BANDPASS_FILTER:
-                return butter_bandpass_filtering_with_settings(data, global_settings,component_settings, device)
-            else:
-                return tukey_bandpass_filtering_with_settings(data, global_settings,component_settings, device)
+    # select corresponding filtering method depending on tag in settings
+    if Tags.BANDPASS_FILTER_METHOD in component_settings:
+        if component_settings[Tags.BANDPASS_FILTER_METHOD] == Tags.TUKEY_BANDPASS_FILTER:
+            return tukey_bandpass_filtering_with_settings(data, global_settings, component_settings, device)
+        elif component_settings[Tags.BANDPASS_FILTER_METHOD] == Tags.BUTTERWORTH_BANDPASS_FILTER:
+            return butter_bandpass_filtering_with_settings(data, global_settings, component_settings, device)
         else:
-            return tukey_bandpass_filtering_with_settings(data, global_settings,component_settings, device)
+            return tukey_bandpass_filtering_with_settings(data, global_settings, component_settings, device)
+    else:
+        return tukey_bandpass_filtering_with_settings(data, global_settings, component_settings, device)
+
 
 def butter_bandpass_filtering(data: np.array,  time_spacing_in_ms: float = None,
                               cutoff_lowpass: int = int(8e6), cutoff_highpass: int = int(0.1e6),
                               order: int = 1) -> np.ndarray:
     """
     Apply a butterworth bandpass filter of `order` with cutoff values at `cutoff_lowpass`
     and `cutoff_highpass` MHz on the `data` using the scipy.signal.butter filter.
@@ -96,22 +99,23 @@
         low = 0.000001
     else:
         low = (cutoff_lowpass / nyquist)
     if cutoff_highpass is None:
         high = 0.999999999
     else:
         high = (cutoff_highpass / nyquist)
-    
+
     b, a = butter(N=order, Wn=[high, low], btype='band')
     y = lfilter(b, a, data)
-    
+
     return y
 
+
 def butter_bandpass_filtering_with_settings(data: np.ndarray, global_settings: Settings, component_settings: Settings,
-                                           device: DetectionGeometryBase) -> np.ndarray:
+                                            device: DetectionGeometryBase) -> np.ndarray:
     """
     Apply a butterworth bandpass filter of `order` with cutoff values at `cutoff_lowpass`
     and `cutoff_highpass` MHz on the `data` using the scipy.signal.butter filter.
     Those values are obtained from the `global_settings`, `component_settings`, and `device`.
 
     :param data: (numpy array) data to be filtered
     :param global_settings: (Settings) settings for the whole simulation
@@ -137,16 +141,16 @@
     if data is None or time_spacing_in_ms is None:
         raise AttributeError("data and time spacing must be specified")
 
     return butter_bandpass_filtering(data, time_spacing_in_ms, cutoff_lowpass, cutoff_highpass, filter_order)
 
 
 def tukey_bandpass_filtering(data: np.ndarray, time_spacing_in_ms: float = None,
-                       cutoff_lowpass: int = int(8e6), cutoff_highpass: int = int(0.1e6),
-                       tukey_alpha: float = 0.5, resampling_for_fft: bool =False) -> np.ndarray:
+                             cutoff_lowpass: int = int(8e6), cutoff_highpass: int = int(0.1e6),
+                             tukey_alpha: float = 0.5, resampling_for_fft: bool = False) -> np.ndarray:
     """
     Apply a tukey bandpass filter with cutoff values at `cutoff_lowpass` and `cutoff_highpass` MHz 
     and a tukey window with alpha value of `tukey_alpha` inbetween on the `data` in Fourier space.
     Note that the filter operates on both, negative and positive frequencies similarly.
     Filtering is performed along the last dimension.
 
     :param data: (numpy array) data to be filtered
@@ -160,27 +164,27 @@
     """
 
     # input checking
     if cutoff_highpass > cutoff_lowpass:
         raise ValueError("The highpass cutoff value must be lower than the lowpass cutoff value.")
 
     # no resampling by default
-    resampling_factor = 1 
+    resampling_factor = 1
     original_size = data.shape[-1]
     target_size = original_size
 
     # resampling if requested
     if resampling_for_fft:
         # resampling settings
         order = 0
         mode = 'constant'
 
-        target_size = int(2**(np.ceil(np.log2(original_size)))) # compute next larger power of 2
+        target_size = int(2**(np.ceil(np.log2(original_size))))  # compute next larger power of 2
         resampling_factor = original_size/target_size
-        zoom_factors = [1]*data.ndim # resampling factor for each dimension
+        zoom_factors = [1]*data.ndim  # resampling factor for each dimension
         zoom_factors[-1] = 1.0/resampling_factor
 
         data = zoom(data, zoom_factors, order=order, mode=mode)
 
     # compute closest indices for cutoff frequencies, limited by the Nyquist frequency
     single_voxel = resampling_factor / (time_spacing_in_ms/1000 * target_size)
     small_index = int(np.minimum((cutoff_highpass / single_voxel), target_size/2.0))
@@ -194,15 +198,15 @@
         small_index = 1
         win = win[:-1]
     window[-large_index:-small_index] = win
 
     # transform data into Fourier space, multiply filter and transform back
     data_in_fourier_space = np.fft.fft(data)
     filtered_data_in_fourier_space = data_in_fourier_space * np.broadcast_to(window, np.shape(data_in_fourier_space))
-    filtered_data =  np.fft.ifft(filtered_data_in_fourier_space).real
+    filtered_data = np.fft.ifft(filtered_data_in_fourier_space).real
 
     # resample back to original size if necessary
     if resampling_for_fft:
         inverse_zoom_factors = [1.0/factor for factor in zoom_factors]
         return zoom(filtered_data, inverse_zoom_factors, order=order, mode=mode)
     else:
         return filtered_data
@@ -376,17 +380,19 @@
         sensor_positions = torch.from_numpy(sensor_positions)
     if isinstance(time_series_sensor_data, np.ndarray):
         time_series_sensor_data = torch.from_numpy(time_series_sensor_data)
     assert isinstance(time_series_sensor_data, torch.Tensor), \
         'The time series sensor data must have been converted to a tensor'
 
     # move tensors to GPU if available, otherwise use CPU
-    dev = get_reconstruction_processing_unit(global_settings)
+    torch_device = get_processing_device(global_settings)
+    
+    if torch_device == torch.device('cpu'):  # warn the user that CPU reconstruction is slow
+        logger.warning(f"Reconstructing on CPU is slow. Check if cuda is available 'torch.cuda.is_available()'.")
 
-    torch_device = torch.device(dev)
     sensor_positions = sensor_positions.to(torch_device)
     time_series_sensor_data = time_series_sensor_data.to(torch_device)
 
     # array must be of correct dimension
     assert time_series_sensor_data.ndim == 2, 'Time series data must have exactly 2 dimensions' \
                                               ', one for the sensor elements and one for time. ' \
                                               'Stack images and sensor positions for 3D reconstruction' \
@@ -398,62 +404,61 @@
     else:
         mode = Tags.RECONSTRUCTION_MODE_PRESSURE
     time_series_sensor_data = reconstruction_mode_transformation(time_series_sensor_data, mode=mode)
 
     return (time_series_sensor_data, sensor_positions, speed_of_sound_in_m_per_s, spacing_in_mm,
             time_spacing_in_ms, torch_device)
 
-
-def get_reconstruction_processing_unit(global_settings):
-    """
-    Get device (CPU/GPU) for reconstructing the image.
-    :param global_settings: global SIMPA settings
-    :return: device for reconstruction
-    """
-    logger = Logger()
-    # if no tag is set, try to use GPU if available
-    if Tags.GPU not in global_settings:
-        if torch.cuda.is_available():
-            dev = "cuda"
-        else:
-            dev = "cpu"
-    else:  # else set tag as user wants
-        dev = "cuda" if global_settings[Tags.GPU] else "cpu"
-
-    if dev == 'cuda' and not torch.cuda.is_available():
-        # torch will likely raise an error if no GPU is available but set as device -> log it to SIMPA log
-        logger.error('Cuda is not available! Check your torch/cuda version.')
-
-    if dev == 'cpu':  # warn the user that CPU reconstruction is slow
-        logger.warning(f"Reconstructing on CPU is slow. Check if cuda is available 'torch.cuda.is_available()'.")
-    return dev
-
-
 def compute_image_dimensions(detection_geometry: DetectionGeometryBase, spacing_in_mm: float,
-                             speed_of_sound_in_m_per_s: float, logger: Logger) -> Tuple[int, int, int, int, int,
-                                                                                        int, int, int, int]:
+                             logger: Logger) -> Tuple[int, int, int, np.float64, np.float64,
+                                                      np.float64, np.float64, np.float64, np.float64]:
     """
-    compute size of beamformed image from field of view of detection geometry
+    Computes size of beamformed image from field of view of detection geometry given the spacing.
 
-    Returns x,z,y dimensions of reconstructed image volume in pixels as well 
-    as the range for each dimension as start and end pixels.
+    :param detection_geometry: detection geometry with specified field of view
+    :type detection_geometry: DetectionGeometryBase
+    :param spacing_in_mm: space betwenn pixels in mm
+    :type spacing_in_mm: float
+    :param logger: logger for debugging purposes
+    :type logger: Logger
+    :returns: tuple with x,z,y dimensions of reconstructed image volume in pixels as well as the range for
+    each dimension as start and end pixels (xdim, zdim, ydim, xdim_start, xdim_end, ydim_start, ydim_end, 
+    zdim_start, zdim_end)
+    :rtype: Tuple[int, int, int, np.float64, np.float64, np.float64, np.float64, np.float64, np.float64]
     """
+
     field_of_view = detection_geometry.field_of_view_extent_mm
     logger.debug(f"Field of view: {field_of_view}")
 
-    xdim_start = int(np.round(field_of_view[0] / spacing_in_mm))
-    xdim_end = int(np.round(field_of_view[1] / spacing_in_mm))
-    zdim_start = int(np.round(field_of_view[2] / spacing_in_mm))
-    zdim_end = int(np.round(field_of_view[3] / spacing_in_mm))
-    ydim_start = int(np.round(field_of_view[4] / spacing_in_mm))
-    ydim_end = int(np.round(field_of_view[5] / spacing_in_mm))
-
-    xdim = (xdim_end - xdim_start)
-    ydim = (ydim_end - ydim_start)
-    zdim = (zdim_end - zdim_start)
+    def compute_for_one_dimension(start_in_mm: float, end_in_mm: float) -> Tuple[int, np.float64, np.float64]:
+        """
+        Helper function to compute the image dimensions for a single dimension given a start and end point in mm.
+        Makes sure that image dimesion is an integer by flooring. 
+        Spaces the pixels symmetrically between start and end.
+
+        :param start_in_mm: lower limit of the field of view in this dimension
+        :type start_in_mm: float
+        :param start_in_mm: upper limit of the field of view in this dimension
+        :type start_in_mm: float
+        :returns: tuple with number of pixels in dimension, lower and upper limit in pixels
+        :rtype: Tuple[int, np.float64, np.float64]
+        """
+
+        start_temp = start_in_mm / spacing_in_mm
+        end_temp = end_in_mm / spacing_in_mm
+        dim_temp = np.abs(end_temp - start_temp)
+        dim = int(np.floor(dim_temp))
+        diff = np.abs(dim_temp - dim)
+        start = start_temp - np.sign(start_temp) * diff/2
+        end = end_temp - np.sign(end_temp) * diff/2
+        return dim, start, end
+
+    xdim, xdim_start, xdim_end = compute_for_one_dimension(field_of_view[0], field_of_view[1])
+    zdim, zdim_start, zdim_end = compute_for_one_dimension(field_of_view[2], field_of_view[3])
+    ydim, ydim_start, ydim_end = compute_for_one_dimension(field_of_view[4], field_of_view[5])
 
     if xdim < 1:
         xdim = 1
     if ydim < 1:
         ydim = 1
     if zdim < 1:
         zdim = 1
@@ -483,24 +488,27 @@
                        "This might be due to a low simulated resolution, please increase it.")
 
     n_sensor_elements = time_series_sensor_data.shape[0]
 
     logger.debug(f'Number of pixels in X dimension: {xdim}, Y dimension: {ydim}, Z dimension: {zdim} '
                  f',number of sensor elements: {n_sensor_elements}')
 
+    x_offset = 0.5 if xdim % 2 == 0 else 0  # to ensure pixels are symmetrically arranged around the 0 like the
+    # sensor positions, add an offset of 0.5 pixels if the dimension is even
+
+    x = xdim_start + torch.arange(xdim, device=torch_device, dtype=torch.float32) + x_offset
+    y = ydim_start + torch.arange(ydim, device=torch_device, dtype=torch.float32)
     if zdim == 1:
-        xx, yy, zz, jj = torch.meshgrid(torch.arange(xdim_start, xdim_end, device=torch_device),
-                                        torch.arange(ydim_start, ydim_end, device=torch_device),
-                                        torch.arange(zdim, device=torch_device),
-                                        torch.arange(n_sensor_elements, device=torch_device))
-    else:
-        xx, yy, zz, jj = torch.meshgrid(torch.arange(xdim_start, xdim_end, device=torch_device),
-                                        torch.arange(ydim_start, ydim_end, device=torch_device),
-                                        torch.arange(zdim_start, zdim_end, device=torch_device),
-                                        torch.arange(n_sensor_elements, device=torch_device))
+        z = torch.arange(zdim, device=torch_device, dtype=torch.float32)
+    else:
+        z = zdim_start + torch.arange(zdim, device=torch_device, dtype=torch.float32)
+    j = torch.arange(n_sensor_elements, device=torch_device, dtype=torch.float32)
+
+    xx, yy, zz, jj = torch.meshgrid(x, y, z, j)
+    jj = jj.long()
 
     delays = torch.sqrt((yy * spacing_in_mm - sensor_positions[:, 2][jj]) ** 2 +
                         (xx * spacing_in_mm - sensor_positions[:, 0][jj]) ** 2 +
                         (zz * spacing_in_mm - sensor_positions[:, 1][jj]) ** 2) \
         / (speed_of_sound_in_m_per_s * time_spacing_in_ms)
 
     # perform index validation
```

### Comparing `simpa-0.8.7/simpa/core/simulation_modules/reconstruction_module/time_reversal_2D.m` & `simpa-0.8.9/simpa/core/simulation_modules/reconstruction_module/time_reversal_2D.m`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/simulation_modules/reconstruction_module/time_reversal_3D.m` & `simpa-0.8.9/simpa/core/simulation_modules/reconstruction_module/time_reversal_3D.m`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/simulation_modules/volume_creation_module/__init__.py` & `simpa-0.8.9/simpa/core/simulation_modules/volume_creation_module/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/simulation_modules/volume_creation_module/volume_creation_module_model_based_adapter.py` & `simpa-0.8.9/simpa/core/simulation_modules/volume_creation_module/volume_creation_module_model_based_adapter.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/core/simulation_modules/volume_creation_module/volume_creation_module_segmentation_based_adapter.py` & `simpa-0.8.9/simpa/core/simulation_modules/volume_creation_module/volume_creation_module_segmentation_based_adapter.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/io_handling/io_hdf5.py` & `simpa-0.8.9/simpa/io_handling/io_hdf5.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/io_handling/ipasc.py` & `simpa-0.8.9/simpa/io_handling/ipasc.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/io_handling/serialization.py` & `simpa-0.8.9/simpa/io_handling/serialization.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/io_handling/zenodo_download.py` & `simpa-0.8.9/simpa/io_handling/zenodo_download.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/log/file_logger.py` & `simpa-0.8.9/simpa/log/file_logger.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/__init__.py` & `simpa-0.8.9/simpa/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/calculate.py` & `simpa-0.8.9/simpa/utils/calculate.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/constants.py` & `simpa-0.8.9/simpa/utils/constants.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/deformation_manager.py` & `simpa-0.8.9/simpa/utils/deformation_manager.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/dict_path_manager.py` & `simpa-0.8.9/simpa/utils/dict_path_manager.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/absorption_spectra_data/Copper_Sulphide.npz` & `simpa-0.8.9/simpa/utils/libraries/absorption_spectra_data/Copper_Sulphide.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/absorption_spectra_data/Deoxyhemoglobin.npz` & `simpa-0.8.9/simpa/utils/libraries/absorption_spectra_data/Deoxyhemoglobin.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/absorption_spectra_data/Fat.npz` & `simpa-0.8.9/simpa/utils/libraries/absorption_spectra_data/Fat.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/absorption_spectra_data/Melanin.npz` & `simpa-0.8.9/simpa/utils/libraries/absorption_spectra_data/Melanin.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/absorption_spectra_data/Nickel_Sulphide.npz` & `simpa-0.8.9/simpa/utils/libraries/absorption_spectra_data/Nickel_Sulphide.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/absorption_spectra_data/Oxyhemoglobin.npz` & `simpa-0.8.9/simpa/utils/libraries/absorption_spectra_data/Oxyhemoglobin.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/absorption_spectra_data/Skin_Baseline.npz` & `simpa-0.8.9/simpa/utils/libraries/absorption_spectra_data/Skin_Baseline.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/absorption_spectra_data/Water.npz` & `simpa-0.8.9/simpa/utils/libraries/absorption_spectra_data/Water.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/anisotropy_spectra_data/Epidermis_Anisotropy.npz` & `simpa-0.8.9/simpa/utils/libraries/anisotropy_spectra_data/Epidermis_Anisotropy.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/literature_values.py` & `simpa-0.8.9/simpa/utils/libraries/literature_values.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/molecule_library.py` & `simpa-0.8.9/simpa/utils/libraries/molecule_library.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/scattering_spectra_data/background_scattering.npz` & `simpa-0.8.9/simpa/utils/libraries/scattering_spectra_data/background_scattering.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/scattering_spectra_data/blood_scattering.npz` & `simpa-0.8.9/simpa/utils/libraries/scattering_spectra_data/blood_scattering.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/scattering_spectra_data/bone_scattering.npz` & `simpa-0.8.9/simpa/utils/libraries/scattering_spectra_data/bone_scattering.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/scattering_spectra_data/fat_scattering.npz` & `simpa-0.8.9/simpa/utils/libraries/scattering_spectra_data/fat_scattering.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/scattering_spectra_data/muscle_scattering.npz` & `simpa-0.8.9/simpa/utils/libraries/scattering_spectra_data/muscle_scattering.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/spectrum_library.py` & `simpa-0.8.9/simpa/utils/libraries/spectrum_library.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/structure_library/BackgroundStructure.py` & `simpa-0.8.9/simpa/utils/libraries/structure_library/BackgroundStructure.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/structure_library/CircularTubularStructure.py` & `simpa-0.8.9/simpa/utils/libraries/structure_library/CircularTubularStructure.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/structure_library/EllipticalTubularStructure.py` & `simpa-0.8.9/simpa/utils/libraries/structure_library/EllipticalTubularStructure.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/structure_library/HorizontalLayerStructure.py` & `simpa-0.8.9/simpa/utils/libraries/structure_library/HorizontalLayerStructure.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/structure_library/ParallelepipedStructure.py` & `simpa-0.8.9/simpa/utils/libraries/structure_library/ParallelepipedStructure.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/structure_library/RectangularCuboidStructure.py` & `simpa-0.8.9/simpa/utils/libraries/structure_library/RectangularCuboidStructure.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/structure_library/SphericalStructure.py` & `simpa-0.8.9/simpa/utils/libraries/structure_library/SphericalStructure.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/structure_library/StructureBase.py` & `simpa-0.8.9/simpa/utils/libraries/structure_library/StructureBase.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/structure_library/VesselStructure.py` & `simpa-0.8.9/simpa/utils/libraries/structure_library/VesselStructure.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/structure_library/__init__.py` & `simpa-0.8.9/simpa/utils/libraries/structure_library/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/libraries/tissue_library.py` & `simpa-0.8.9/simpa/utils/libraries/tissue_library.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/path_manager.py` & `simpa-0.8.9/simpa/utils/path_manager.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/quality_assurance/data_sanity_testing.py` & `simpa-0.8.9/simpa/utils/quality_assurance/data_sanity_testing.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/settings.py` & `simpa-0.8.9/simpa/utils/settings.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/tags.py` & `simpa-0.8.9/simpa/utils/tags.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/utils/tissue_properties.py` & `simpa-0.8.9/simpa/utils/tissue_properties.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/visualisation/matplotlib_data_visualisation.py` & `simpa-0.8.9/simpa/visualisation/matplotlib_data_visualisation.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa/visualisation/matplotlib_device_visualisation.py` & `simpa-0.8.9/simpa/visualisation/matplotlib_device_visualisation.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/__init__.py` & `simpa-0.8.9/simpa_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/automatic_tests/device_tests/test_curved_array.py` & `simpa-0.8.9/simpa_tests/automatic_tests/device_tests/test_curved_array.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/automatic_tests/device_tests/test_linear_array.py` & `simpa-0.8.9/simpa_tests/automatic_tests/device_tests/test_linear_array.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/automatic_tests/structure_tests/test_boxes.py` & `simpa-0.8.9/simpa_tests/automatic_tests/structure_tests/test_boxes.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/automatic_tests/structure_tests/test_elliptical_tubes.py` & `simpa-0.8.9/simpa_tests/automatic_tests/structure_tests/test_elliptical_tubes.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/automatic_tests/structure_tests/test_layers.py` & `simpa-0.8.9/simpa_tests/automatic_tests/structure_tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/automatic_tests/structure_tests/test_parallel_epipeds.py` & `simpa-0.8.9/simpa_tests/automatic_tests/structure_tests/test_parallel_epipeds.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/automatic_tests/structure_tests/test_spheres.py` & `simpa-0.8.9/simpa_tests/automatic_tests/structure_tests/test_spheres.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/automatic_tests/structure_tests/test_tubes.py` & `simpa-0.8.9/simpa_tests/automatic_tests/structure_tests/test_tubes.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/automatic_tests/structure_tests/test_vesseltree.py` & `simpa-0.8.9/simpa_tests/automatic_tests/structure_tests/test_vesseltree.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/automatic_tests/test_IPASC_export.py` & `simpa-0.8.9/simpa_tests/automatic_tests/test_IPASC_export.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/automatic_tests/test_bandpass_filter.py` & `simpa-0.8.9/simpa_tests/automatic_tests/test_bandpass_filter.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/automatic_tests/test_calculation_utils.py` & `simpa-0.8.9/simpa_tests/automatic_tests/test_calculation_utils.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/automatic_tests/test_create_a_volume.py` & `simpa-0.8.9/simpa_tests/automatic_tests/test_create_a_volume.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/automatic_tests/test_device_UUID.py` & `simpa-0.8.9/simpa_tests/automatic_tests/test_device_UUID.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/automatic_tests/test_io_handling.py` & `simpa-0.8.9/simpa_tests/automatic_tests/test_io_handling.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/automatic_tests/test_linear_unmixing.py` & `simpa-0.8.9/simpa_tests/automatic_tests/test_linear_unmixing.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/automatic_tests/test_logging.py` & `simpa-0.8.9/simpa_tests/automatic_tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/automatic_tests/test_noise_models.py` & `simpa-0.8.9/simpa_tests/automatic_tests/test_noise_models.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/automatic_tests/test_path_manager.py` & `simpa-0.8.9/simpa_tests/automatic_tests/test_path_manager.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/automatic_tests/test_pipeline.py` & `simpa-0.8.9/simpa_tests/automatic_tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/automatic_tests/test_processing.py` & `simpa-0.8.9/simpa_tests/automatic_tests/test_processing.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/automatic_tests/test_quality_assurance.py` & `simpa-0.8.9/simpa_tests/automatic_tests/test_quality_assurance.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/automatic_tests/tissue_library/test_core_assumptions.py` & `simpa-0.8.9/simpa_tests/automatic_tests/tissue_library/test_core_assumptions.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/automatic_tests/tissue_library/test_spectra_can_be_found.py` & `simpa-0.8.9/simpa_tests/automatic_tests/tissue_library/test_spectra_can_be_found.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/automatic_tests/tissue_library/test_tissue_library_against_literature_values.py` & `simpa-0.8.9/simpa_tests/automatic_tests/tissue_library/test_tissue_library_against_literature_values.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/checklists/release_checklist.md` & `simpa-0.8.9/simpa_tests/checklists/release_checklist.md`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/do_coverage.py` & `simpa-0.8.9/simpa_tests/do_coverage.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/full_integration_test.bat` & `simpa-0.8.9/simpa_tests/full_integration_test.bat`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/manual_tests/__init__.py` & `simpa-0.8.9/simpa_tests/manual_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/manual_tests/acoustic_forward_models/KWaveAcousticForwardConvenienceFunction.py` & `simpa-0.8.9/simpa_tests/manual_tests/acoustic_forward_models/KWaveAcousticForwardConvenienceFunction.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/manual_tests/acoustic_forward_models/MinimalKWaveTest.py` & `simpa-0.8.9/simpa_tests/manual_tests/acoustic_forward_models/MinimalKWaveTest.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/manual_tests/digital_device_twins/SimulationWithMSOTInvision.py` & `simpa-0.8.9/simpa_tests/manual_tests/digital_device_twins/SimulationWithMSOTInvision.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/manual_tests/digital_device_twins/VisualiseDevices.py` & `simpa-0.8.9/simpa_tests/manual_tests/digital_device_twins/VisualiseDevices.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/manual_tests/image_reconstruction/DelayAndSumReconstruction.py` & `simpa-0.8.9/simpa_tests/manual_tests/image_reconstruction/DelayAndSumReconstruction.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/manual_tests/image_reconstruction/DelayMultiplyAndSumReconstruction.py` & `simpa-0.8.9/simpa_tests/manual_tests/image_reconstruction/DelayMultiplyAndSumReconstruction.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/manual_tests/image_reconstruction/PointSourceReconstruction.py` & `simpa-0.8.9/simpa_tests/manual_tests/image_reconstruction/PointSourceReconstruction.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/manual_tests/image_reconstruction/SignedDelayMultiplyAndSumReconstruction.py` & `simpa-0.8.9/simpa_tests/manual_tests/image_reconstruction/SignedDelayMultiplyAndSumReconstruction.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/manual_tests/image_reconstruction/TimeReversalReconstruction.py` & `simpa-0.8.9/simpa_tests/manual_tests/image_reconstruction/TimeReversalReconstruction.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/manual_tests/optical_forward_models/AbsorptionAndScatteringWithInifinitesimalSlabExperiment.py` & `simpa-0.8.9/simpa_tests/manual_tests/optical_forward_models/AbsorptionAndScatteringWithInifinitesimalSlabExperiment.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/manual_tests/optical_forward_models/AbsorptionAndScatteringWithinHomogenousMedium.py` & `simpa-0.8.9/simpa_tests/manual_tests/optical_forward_models/AbsorptionAndScatteringWithinHomogenousMedium.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/manual_tests/optical_forward_models/CompareMCXResultsWithDiffusionTheory.py` & `simpa-0.8.9/simpa_tests/manual_tests/optical_forward_models/CompareMCXResultsWithDiffusionTheory.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/manual_tests/optical_forward_models/ComputeDiffuseReflectance.py` & `simpa-0.8.9/simpa_tests/manual_tests/optical_forward_models/ComputeDiffuseReflectance.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/manual_tests/processing_components/QPAIReconstruction.py` & `simpa-0.8.9/simpa_tests/manual_tests/processing_components/QPAIReconstruction.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/manual_tests/processing_components/TestLinearUnmixingVisual.py` & `simpa-0.8.9/simpa_tests/manual_tests/processing_components/TestLinearUnmixingVisual.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/manual_tests/test_with_experimental_measurements/ReproduceDISMeasurements.py` & `simpa-0.8.9/simpa_tests/manual_tests/test_with_experimental_measurements/ReproduceDISMeasurements.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_dark.rxt` & `simpa-0.8.9/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_dark.rxt`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_dark_spectra.npz` & `simpa-0.8.9/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_dark_spectra.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_light.rxt` & `simpa-0.8.9/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_light.rxt`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_light_spectra.npz` & `simpa-0.8.9/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/background_material_light_spectra.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/inclusion_material.rxt` & `simpa-0.8.9/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/inclusion_material.rxt`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/inclusion_material_spectra.npz` & `simpa-0.8.9/simpa_tests/manual_tests/test_with_experimental_measurements/test_data/inclusion_material_spectra.npz`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/manual_tests/test_with_experimental_measurements/utils.py` & `simpa-0.8.9/simpa_tests/manual_tests/test_with_experimental_measurements/utils.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/manual_tests/volume_creation/SegmentationLoader.py` & `simpa-0.8.9/simpa_tests/manual_tests/volume_creation/SegmentationLoader.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/test_utils/__init__.py` & `simpa-0.8.9/simpa_tests/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/test_utils/tissue_composition_tests.py` & `simpa-0.8.9/simpa_tests/test_utils/tissue_composition_tests.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/simpa_tests/test_utils/tissue_models.py` & `simpa-0.8.9/simpa_tests/test_utils/tissue_models.py`

 * *Files identical despite different names*

### Comparing `simpa-0.8.7/setup.py` & `simpa-0.8.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,21 +63,21 @@
  'scipy>=1.7.2',
  'torch>=1.10.0',
  'wget>=3.2',
  'xmltodict>=0.12.0']
 
 setup_kwargs = {
     'name': 'simpa',
-    'version': '0.8.7',
+    'version': '0.8.9',
     'description': 'Simulation and Image Processing for Photonics and Acoustics',
-    'long_description': '[![Documentation Status](https://readthedocs.org/projects/simpa/badge/?version=develop)](https://simpa.readthedocs.io/en/develop/?badge=develop)\n![Build Status](https://github.com/IMSY-DKFZ/simpa/actions/workflows/automatic_testing.yml/badge.svg)\n[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/IMSY-DKFZ/simpa/blob/main/LICENSE.md)\n\n[![Pypi Badge](https://img.shields.io/pypi/v/simpa)](https://pypi.org/project/simpa/)\n[![PyPI downloads](https://img.shields.io/pypi/dw/simpa?color=gr&label=pypi%20downloads)](https://pypi.org/project/simpa/)\n\n![Logo](docs/source/images/simpa_logo.png?raw=true "Logo")\n\n# The toolkit for Simulation and Image Processing for Photonics and Acoustics (SIMPA)\n\nSIMPA aims to facilitate realistic image simulation for optical and acoustic imaging modalities by\nproviding adapters to crucial modelling steps, such as volume generation; optical modelling; acoustic\nmodelling; and image reconstruction. SIMPA provides a communication layer between various modules\nthat implement optical and acoustic forward and inverse models.\nNon-experts can use the toolkit to create sensible simulations from default parameters in an end-to-end fashion. Domain experts are provided with the functionality to set up a highly customisable\npipeline according to their specific use cases and tool requirements.\nThe paper that introduces SIMPA including visualisations and explanations can be found here: [https://doi.org/10.1117/1.JBO.27.8.083010](https://doi.org/10.1117/1.JBO.27.8.083010)\n\n* [Getting started](#getting-started)\n* [Simulation examples](#simulation-examples)\n* [Documentation](#documentation)\n* [Contributing](#how-to-contribute)\n* [Performance profiling](#performance-profiling)\n* [Troubleshooting](#troubleshooting)\n* [Citation](#citation)\n\nThe toolkit is still under development and is thus not fully tested and may contain bugs. \nPlease report any issues that you find in our Issue Tracker: https://github.com/IMSY-DKFZ/simpa/issues. \nAlso make sure to double check all value ranges of the optical and acoustic tissue properties \nand to assess all simulation results for plausibility.\n\n# Getting started\n\nIn order to use SIMPA in your project, SIMPA has to be installed as well as the external tools that make the actual simulations possible.\nFinally, to connect everything, SIMPA has to find all the binaries of the simulation modules you would like to use.\nThe SIMPA path management takes care of that.\n\n* [SIMPA installation instructions](#simpa-installation-instructions)\n* [External tools installation instructions](#external-tools-installation-instructions)\n* [Path Management](#path-management)\n\n## SIMPA installation instructions\n\nThe recommended way to install SIMPA is a manual installation from the GitHub repository, please follow steps 1 - 3:\n\n1. `git clone https://github.com/IMSY-DKFZ/simpa.git`\n2. `cd simpa`\n3. `git checkout main`\n4. `git pull`\n\nNow open a python instance in the \'simpa\' folder that you have just downloaded. Make sure that you have your preferred\nvirtual environment activated (we also recommend python 3.8)\n1. `pip install -r requirements.txt`\n2. `python setup.py install` (for developement: `python setup.py develop`)\n3. Test if the installation worked by using `python` followed by `import simpa` then `exit()`\n\nIf no error messages arise, you are now setup to use SIMPA in your project.\n\nYou can also install SIMPA with pip. Simply run:\n\n`pip install simpa`\n\nYou also need to manually install the pytorch library to use all features of SIMPA.\nTo this end, use the pytorch website tool to figure out which version to install:\n[https://pytorch.org/get-started/locally/](https://pytorch.org/get-started/locally/)\n\n## External tools installation instructions\n\nIn order to get the full SIMPA functionality, you should install all third party toolkits that make the optical and \nacoustic simulations possible. \n\n### mcx (Optical Forward Model)\n\nEither download suitable executables or build yourself from the following sources:\n\n[http://mcx.space/](http://mcx.space/)\n\nIn order to obtain access to all custom sources that we implemented, please build mcx yourself from the\nfollowing mcx Github fork:\n[https://github.com/IMSY-DKFZ/mcx](https://github.com/IMSY-DKFZ/mcx)\n\nFor the installation, please follow steps 1-4:\n1. `git clone https://github.com/IMSY-DKFZ/mcx.git`\n2. `cd mcx/src`\n3. In `MAKEFILE` adapt line 111 the sm version [according to your GPU](https://arnon.dk/matching-sm-architectures-arch-and-gencode-for-various-nvidia-cards/).\n4. `make`\n\nThe built binary can be found in `src/bin`.\nNote, in case you can’t build mcx with the GPU-specific sm version you need to install a more recent NVIDIA driver and nvcc toolkit. \nOne option would be to install cuda in a conda environment via `conda install cuda -c nvidia`.\nPlease note that there might be compatibility issues using mcx-cl with the MCX Adapter as this use case is not \nbeing tested and supported by the SIMPA developers.\n\n### k-Wave (Acoustic Forward Model)\n\nPlease follow the following steps and use the k-Wave install instructions \nfor further (and much better) guidance under:\n\n[http://www.k-wave.org/](http://www.k-wave.org/)\n\n1. Install MATLAB with the core, image processing and parallel computing toolboxes activated at the minimum.\n2. Download the kWave toolbox\n3. Add the kWave toolbox base path to the toolbox paths in MATLAB\n4. Download the kWaveArray addition from the link given in this user forum post [http://www.k-wave.org/forum/topic/alpha-version-of-kwavearray-off-grid-sources](http://www.k-wave.org/forum/topic/alpha-version-of-kwavearray-off-grid-sources)\n5. Add the kWaveArray folder to the toolbox paths in MATLAB as well\n6. If wanted: Download the CPP and CUDA binary files and place them in the k-Wave/binaries folder\n7. Note down the system path to the `matlab` executable file.\n\n## Path management\n\nAs a pipelining tool that serves as a communication layer between different numerical forward models and\nprocessing tools, SIMPA needs to be configured with the paths to these tools on your local hard drive.\nTo this end, we have implemented the `PathManager` class that you can import to your project using\n`from simpa.utils import PathManager`. The PathManager looks for a `path_config.env` file (just like the\none we provided in the `simpa_examples`) in the following places in this order:\n1. The optional path you give the PathManager\n2. Your $HOME$ directory\n3. The current working directory\n4. The SIMPA home directory path\n\nPlease follow the instructions in the `path_config.env` file in the `simpa_examples` folder. \n\n# Simulation examples\n\nTo get started with actual simulations, SIMPA provides an [example package](simpa_examples) of simple simulation \nscripts to build your custom simulations upon. The [minimal optical simulation](simpa_examples/minimal_optical_simulation.py)\nis a nice start if you have MCX installed.\n\nGenerally, the following pseudo code demonstrates the construction and run of a simulation pipeline:\n\n```python\nimport simpa as sp\n\n# Create general settings \nsettings = sp.Settings(general_settings)\n\n# Create specific settings for each pipeline element \n# in the simulation pipeline\nsettings.set_volume_creation_settings(volume_creation_settings)\nsettings.set_optical_settings(optical_settings)\nsettings.set_acoustic_settings(acoustic_settings)\nsettings.set_reconstruction_settings(reconstruction_settings)\n\n# Set the simulation pipeline\nsimulation_pipeline = [sp.VolumeCreatorModule(settings),\n    sp.OpticalForwardModule(settings),\n    sp.AcousticForwardModule(settings),\n    sp.ReconstructionModule(settings)]\n    \n# Choose a PA device with device position in the volume\ndevice = sp.CustomDevice()\n\n# Simulate the pipeline\nsp.simulate(simulation_pipeline, settings, device)\n```\n\n# Documentation\n\nThe updated version of the SIMPA documentation can be found at [https://simpa.readthedocs.io/en/develop](https://simpa.readthedocs.io/en/develop).\n\n## Building the documentation\n\nIt is also easily possible to build the SIMPA documentation from scratch.\nWhen the installation succeeded, and you want to make sure that you have the latest documentation\nyou should do the following steps in a command line:\n\n1. Navigate to the `simpa/docs` directory\n2. If you would like the documentation to have the https://readthedocs.org/ style, type `pip install sphinx-rtd-theme`\n3. Type `make html`\n4. Open the `index.html` file in the `simpa/docs/build/html` directory with your favourite browser.\n\n# How to contribute\n\nPlease find a more detailed description of how to contribute as well as code style references in our\n[contribution guidelines](CONTRIBUTING.md).\n\nTo contribute to SIMPA, please fork the SIMPA github repository and create a pull request with a branch containing your \nsuggested changes. The core developers will then review the suggested changes and integrate these into the code \nbase.\n\nPlease make sure that you have included unit tests for your code and that all previous tests still run through.\n\nThere is a regular SIMPA status meeting every Friday on even calendar weeks at 10:00 CET/CEST, and you are very welcome to participate and\nraise any issues or suggest new features. If you want to join this meeting, write one of the core developers.\n\nPlease see the github guidelines for creating pull requests: [https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests)\n\n\n# Performance profiling\n\nDo you wish to know which parts of the simulation pipeline cost the most amount of time? \nIf that is the case then you can use the following commands to profile the execution of your simulation script.\nYou simply need to replace the `myscript` name with your script name.\n\n`python -m cProfile -o myscript.cprof myscript.py`\n\n`pyprof2calltree -k -i myscript.cprof`\n\n# Troubleshooting\n\nIn this section, known problems are listed with their solutions (if available):\n\n## 1. Error reading hdf5-files when using k-Wave binaries:\n   \nIf you encounter an error similar to:\n\n    Error using h5readc\n    The filename specified was either not found on the MATLAB path or it contains unsupported characters.\n\nLook up the solution in [this thread of the k-Wave forum](http://www.k-wave.org/forum/topic/error-reading-h5-files-when-using-binaries).  \n      \n# Citation\n\nIf you use the SIMPA tool, we would appreciate if you cite our Journal publication in the Journal of Biomedical Optics:\n\nGröhl, Janek, Kris K. Dreher, Melanie Schellenberg, Tom Rix, Niklas Holzwarth, Patricia Vieten, Leonardo Ayala, Sarah E. Bohndiek, Alexander Seitel, and Lena Maier-Hein. *"SIMPA: an open-source toolkit for simulation and image processing for photonics and acoustics."* **Journal of Biomedical Optics** 27, no. 8 (2022).\n\n```Bibtex\n@article{2022simpatoolkit,\n  title={SIMPA: an open-source toolkit for simulation and image processing for photonics and acoustics},\n  author={Gr{\\"o}hl, Janek and Dreher, Kris K and Schellenberg, Melanie and Rix, Tom and Holzwarth, Niklas and Vieten, Patricia and Ayala, Leonardo and Bohndiek, Sarah E and Seitel, Alexander and Maier-Hein, Lena},\n  journal={Journal of Biomedical Optics},\n  volume={27},\n  number={8},\n  year={2022},\n  publisher={SPIE}\n}\n```\n',
+    'long_description': '[![Documentation Status](https://readthedocs.org/projects/simpa/badge/?version=develop)](https://simpa.readthedocs.io/en/develop/?badge=develop)\n![Build Status](https://github.com/IMSY-DKFZ/simpa/actions/workflows/automatic_testing.yml/badge.svg)\n[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/IMSY-DKFZ/simpa/blob/main/LICENSE.md)\n\n[![Pypi Badge](https://img.shields.io/pypi/v/simpa)](https://pypi.org/project/simpa/)\n[![PyPI downloads](https://img.shields.io/pypi/dw/simpa?color=gr&label=pypi%20downloads)](https://pypi.org/project/simpa/)\n\n![Logo](docs/source/images/simpa_logo.png?raw=true "Logo")\n\n# The toolkit for Simulation and Image Processing for Photonics and Acoustics (SIMPA)\n\nSIMPA aims to facilitate realistic image simulation for optical and acoustic imaging modalities by\nproviding adapters to crucial modelling steps, such as volume generation; optical modelling; acoustic\nmodelling; and image reconstruction. SIMPA provides a communication layer between various modules\nthat implement optical and acoustic forward and inverse models.\nNon-experts can use the toolkit to create sensible simulations from default parameters in an end-to-end fashion. Domain experts are provided with the functionality to set up a highly customisable\npipeline according to their specific use cases and tool requirements.\nThe paper that introduces SIMPA including visualisations and explanations can be found here: [https://doi.org/10.1117/1.JBO.27.8.083010](https://doi.org/10.1117/1.JBO.27.8.083010)\n\n* [Getting started](#getting-started)\n* [Simulation examples](#simulation-examples)\n* [Documentation](#documentation)\n* [Contributing](#how-to-contribute)\n* [Performance profiling](#performance-profiling)\n* [Troubleshooting](#troubleshooting)\n* [Citation](#citation)\n\nThe toolkit is still under development and is thus not fully tested and may contain bugs. \nPlease report any issues that you find in our Issue Tracker: https://github.com/IMSY-DKFZ/simpa/issues. \nAlso make sure to double check all value ranges of the optical and acoustic tissue properties \nand to assess all simulation results for plausibility.\n\n# Getting started\n\nIn order to use SIMPA in your project, SIMPA has to be installed as well as the external tools that make the actual simulations possible.\nFinally, to connect everything, SIMPA has to find all the binaries of the simulation modules you would like to use.\nThe SIMPA path management takes care of that.\n\n* [SIMPA installation instructions](#simpa-installation-instructions)\n* [External tools installation instructions](#external-tools-installation-instructions)\n* [Path Management](#path-management)\n\n## SIMPA installation instructions\n\nThe recommended way to install SIMPA is a manual installation from the GitHub repository, please follow steps 1 - 3:\n\n1. `git clone https://github.com/IMSY-DKFZ/simpa.git`\n2. `cd simpa`\n3. `git checkout main`\n4. `git pull`\n\nNow open a python instance in the \'simpa\' folder that you have just downloaded. Make sure that you have your preferred\nvirtual environment activated (we also recommend python 3.8)\n1. `pip install .`\n2. Test if the installation worked by using `python` followed by `import simpa` then `exit()`\n\nIf no error messages arise, you are now setup to use SIMPA in your project.\n\nYou can also install SIMPA with pip. Simply run:\n\n`pip install simpa`\n\nYou also need to manually install the pytorch library to use all features of SIMPA.\nTo this end, use the pytorch website tool to figure out which version to install:\n[https://pytorch.org/get-started/locally/](https://pytorch.org/get-started/locally/)\n\n## External tools installation instructions\n\nIn order to get the full SIMPA functionality, you should install all third party toolkits that make the optical and \nacoustic simulations possible. \n\n### mcx (Optical Forward Model)\n\nEither download suitable executables or build yourself from the following sources:\n\n[http://mcx.space/](http://mcx.space/)\n\nIn order to obtain access to all custom sources that we implemented, please build mcx yourself from the\nfollowing mcx Github fork:\n[https://github.com/IMSY-DKFZ/mcx](https://github.com/IMSY-DKFZ/mcx)\n\nFor the installation, please follow steps 1-4:\n1. `git clone https://github.com/IMSY-DKFZ/mcx.git`\n2. `cd mcx/src`\n3. In `MAKEFILE` adapt line 111 the sm version [according to your GPU](https://arnon.dk/matching-sm-architectures-arch-and-gencode-for-various-nvidia-cards/).\n4. `make`\n\nThe built binary can be found in `src/bin`.\nNote, in case you can’t build mcx with the GPU-specific sm version you need to install a more recent NVIDIA driver and nvcc toolkit. \nOne option would be to install cuda in a conda environment via `conda install cuda -c nvidia`.\nPlease note that there might be compatibility issues using mcx-cl with the MCX Adapter as this use case is not \nbeing tested and supported by the SIMPA developers.\n\n### k-Wave (Acoustic Forward Model)\n\nPlease follow the following steps and use the k-Wave install instructions \nfor further (and much better) guidance under:\n\n[http://www.k-wave.org/](http://www.k-wave.org/)\n\n1. Install MATLAB with the core, image processing and parallel computing toolboxes activated at the minimum.\n2. Download the kWave toolbox\n3. Add the kWave toolbox base path to the toolbox paths in MATLAB\n4. Download the kWaveArray addition from the link given in this user forum post [http://www.k-wave.org/forum/topic/alpha-version-of-kwavearray-off-grid-sources](http://www.k-wave.org/forum/topic/alpha-version-of-kwavearray-off-grid-sources)\n5. Add the kWaveArray folder to the toolbox paths in MATLAB as well\n6. If wanted: Download the CPP and CUDA binary files and place them in the k-Wave/binaries folder\n7. Note down the system path to the `matlab` executable file.\n\n## Path management\n\nAs a pipelining tool that serves as a communication layer between different numerical forward models and\nprocessing tools, SIMPA needs to be configured with the paths to these tools on your local hard drive.\nTo this end, we have implemented the `PathManager` class that you can import to your project using\n`from simpa.utils import PathManager`. The PathManager looks for a `path_config.env` file (just like the\none we provided in the `simpa_examples`) in the following places in this order:\n1. The optional path you give the PathManager\n2. Your $HOME$ directory\n3. The current working directory\n4. The SIMPA home directory path\n\nPlease follow the instructions in the `path_config.env` file in the `simpa_examples` folder. \n\n# Simulation examples\n\nTo get started with actual simulations, SIMPA provides an [example package](simpa_examples) of simple simulation \nscripts to build your custom simulations upon. The [minimal optical simulation](simpa_examples/minimal_optical_simulation.py)\nis a nice start if you have MCX installed.\n\nGenerally, the following pseudo code demonstrates the construction and run of a simulation pipeline:\n\n```python\nimport simpa as sp\n\n# Create general settings \nsettings = sp.Settings(general_settings)\n\n# Create specific settings for each pipeline element \n# in the simulation pipeline\nsettings.set_volume_creation_settings(volume_creation_settings)\nsettings.set_optical_settings(optical_settings)\nsettings.set_acoustic_settings(acoustic_settings)\nsettings.set_reconstruction_settings(reconstruction_settings)\n\n# Set the simulation pipeline\nsimulation_pipeline = [sp.VolumeCreatorModule(settings),\n    sp.OpticalForwardModule(settings),\n    sp.AcousticForwardModule(settings),\n    sp.ReconstructionModule(settings)]\n    \n# Choose a PA device with device position in the volume\ndevice = sp.CustomDevice()\n\n# Simulate the pipeline\nsp.simulate(simulation_pipeline, settings, device)\n```\n\n# Documentation\n\nThe updated version of the SIMPA documentation can be found at [https://simpa.readthedocs.io/en/develop](https://simpa.readthedocs.io/en/develop).\n\n## Building the documentation\n\nIt is also easily possible to build the SIMPA documentation from scratch.\nWhen the installation succeeded, and you want to make sure that you have the latest documentation\nyou should do the following steps in a command line:\n\n1. Navigate to the `simpa/docs` directory\n2. If you would like the documentation to have the https://readthedocs.org/ style, type `pip install sphinx-rtd-theme`\n3. Type `make html`\n4. Open the `index.html` file in the `simpa/docs/build/html` directory with your favourite browser.\n\n# How to contribute\n\nPlease find a more detailed description of how to contribute as well as code style references in our\n[contribution guidelines](CONTRIBUTING.md).\n\nTo contribute to SIMPA, please fork the SIMPA github repository and create a pull request with a branch containing your \nsuggested changes. The core developers will then review the suggested changes and integrate these into the code \nbase.\n\nPlease make sure that you have included unit tests for your code and that all previous tests still run through.\n\nThere is a regular SIMPA status meeting every Friday on even calendar weeks at 10:00 CET/CEST, and you are very welcome to participate and\nraise any issues or suggest new features. If you want to join this meeting, write one of the core developers.\n\nPlease see the github guidelines for creating pull requests: [https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-requests)\n\n\n# Performance profiling\n\nDo you wish to know which parts of the simulation pipeline cost the most amount of time? \nIf that is the case then you can use the following commands to profile the execution of your simulation script.\nYou simply need to replace the `myscript` name with your script name.\n\n`python -m cProfile -o myscript.cprof myscript.py`\n\n`pyprof2calltree -k -i myscript.cprof`\n\n# Troubleshooting\n\nIn this section, known problems are listed with their solutions (if available):\n\n## 1. Error reading hdf5-files when using k-Wave binaries:\n   \nIf you encounter an error similar to:\n\n    Error using h5readc\n    The filename specified was either not found on the MATLAB path or it contains unsupported characters.\n\nLook up the solution in [this thread of the k-Wave forum](http://www.k-wave.org/forum/topic/error-reading-h5-files-when-using-binaries).  \n      \n# Citation\n\nIf you use the SIMPA tool, we would appreciate if you cite our Journal publication in the Journal of Biomedical Optics:\n\nGröhl, Janek, Kris K. Dreher, Melanie Schellenberg, Tom Rix, Niklas Holzwarth, Patricia Vieten, Leonardo Ayala, Sarah E. Bohndiek, Alexander Seitel, and Lena Maier-Hein. *"SIMPA: an open-source toolkit for simulation and image processing for photonics and acoustics."* **Journal of Biomedical Optics** 27, no. 8 (2022).\n\n```Bibtex\n@article{2022simpatoolkit,\n  title={SIMPA: an open-source toolkit for simulation and image processing for photonics and acoustics},\n  author={Gr{\\"o}hl, Janek and Dreher, Kris K and Schellenberg, Melanie and Rix, Tom and Holzwarth, Niklas and Vieten, Patricia and Ayala, Leonardo and Bohndiek, Sarah E and Seitel, Alexander and Maier-Hein, Lena},\n  journal={Journal of Biomedical Optics},\n  volume={27},\n  number={8},\n  year={2022},\n  publisher={SPIE}\n}\n```\n',
     'author': 'Division of Intelligent Medical Systems (IMSY), DKFZ',
     'author_email': 'k.dreher@dkfz-heidelberg.de',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/IMSY-DKFZ/simpa',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<3.11',
 }
```

### Comparing `simpa-0.8.7/PKG-INFO` & `simpa-0.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: simpa
-Version: 0.8.7
+Version: 0.8.9
 Summary: Simulation and Image Processing for Photonics and Acoustics
 Home-page: https://github.com/IMSY-DKFZ/simpa
 License: MIT
 Keywords: simulation,photonics,acoustics
 Author: Division of Intelligent Medical Systems (IMSY), DKFZ
 Author-email: k.dreher@dkfz-heidelberg.de
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Deprecated (>=1.2.13)
 Requires-Dist: coverage (>=6.1.2)
 Requires-Dist: h5py (>=3.6.0)
 Requires-Dist: ipasc-tool (>=0.1.3)
 Requires-Dist: jdata (>=0.3.7)
 Requires-Dist: matplotlib (>=3.5.0)
 Requires-Dist: numpy (>=1.21.4)
@@ -82,17 +82,16 @@
 1. `git clone https://github.com/IMSY-DKFZ/simpa.git`
 2. `cd simpa`
 3. `git checkout main`
 4. `git pull`
 
 Now open a python instance in the 'simpa' folder that you have just downloaded. Make sure that you have your preferred
 virtual environment activated (we also recommend python 3.8)
-1. `pip install -r requirements.txt`
-2. `python setup.py install` (for developement: `python setup.py develop`)
-3. Test if the installation worked by using `python` followed by `import simpa` then `exit()`
+1. `pip install .`
+2. Test if the installation worked by using `python` followed by `import simpa` then `exit()`
 
 If no error messages arise, you are now setup to use SIMPA in your project.
 
 You can also install SIMPA with pip. Simply run:
 
 `pip install simpa`
```


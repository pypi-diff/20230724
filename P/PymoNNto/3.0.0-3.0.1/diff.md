# Comparing `tmp/PymoNNto-3.0.0.tar.gz` & `tmp/PymoNNto-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PymoNNto-3.0.0.tar", last modified: Tue Mar 28 23:19:08 2023, max compression
+gzip compressed data, was "PymoNNto-3.0.1.tar", last modified: Mon Jul 24 00:51:20 2023, max compression
```

## Comparing `PymoNNto-3.0.0.tar` & `PymoNNto-3.0.1.tar`

### file list

```diff
@@ -1,169 +1,170 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 23:19:08.911278 PymoNNto-3.0.0/
--rw-rw-rw-   0        0        0     1073 2020-12-02 18:45:09.000000 PymoNNto-3.0.0/LICENSE
--rw-rw-rw-   0        0        0      678 2023-03-28 23:19:08.911278 PymoNNto-3.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-28 23:19:08.152751 PymoNNto-3.0.0/PymoNNto/
--rw-rw-rw-   0        0        0      448 2023-03-22 16:38:59.000000 PymoNNto-3.0.0/PymoNNto/CLI.py
-drwxrwxrwx   0        0        0        0 2023-03-28 23:19:08.199626 PymoNNto-3.0.0/PymoNNto/Exploration/
-drwxrwxrwx   0        0        0        0 2023-03-28 23:19:08.230880 PymoNNto-3.0.0/PymoNNto/Exploration/AnalysisModules/
--rw-rw-rw-   0        0        0      548 2023-02-24 14:24:06.000000 PymoNNto-3.0.0/PymoNNto/Exploration/AnalysisModules/Static_Classification.py
--rw-rw-rw-   0        0        0     3571 2023-03-09 20:27:54.000000 PymoNNto-3.0.0/PymoNNto/Exploration/AnalysisModules/Weight_Classifier_Base.py
--rw-rw-rw-   0        0        0      289 2023-02-24 14:24:06.000000 PymoNNto-3.0.0/PymoNNto/Exploration/AnalysisModules/Weight_Classifier_Post.py
--rw-rw-rw-   0        0        0      288 2023-02-24 14:24:06.000000 PymoNNto-3.0.0/PymoNNto/Exploration/AnalysisModules/Weight_Classifier_Pre.py
--rw-rw-rw-   0        0        0      221 2022-07-29 10:15:40.000000 PymoNNto-3.0.0/PymoNNto/Exploration/AnalysisModules/__init__.py
--rw-rw-rw-   0        0        0    10819 2023-03-22 16:39:46.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Behaviour_UI.py
-drwxrwxrwx   0        0        0        0 2023-03-28 23:19:08.340262 PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/
--rw-rw-rw-   0        0        0     5032 2023-02-15 19:37:04.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/Breed_And_Selection_Module.py
-drwxrwxrwx   0        0        0        0 2023-03-28 23:19:08.371547 PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/Devices/
--rw-rw-rw-   0        0        0     2471 2023-03-07 13:25:34.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/Devices/Evolution_Device.py
--rw-rw-rw-   0        0        0     2205 2022-09-21 18:37:13.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/Devices/Evolution_Device_Multi_Thread.py
--rw-rw-rw-   0        0        0     2514 2022-12-08 02:47:35.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/Devices/Evolution_Device_SSH.py
--rw-rw-rw-   0        0        0      796 2022-09-21 17:40:35.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/Devices/Evolution_Device_Single_Thread.py
--rw-rw-rw-   0        0        0        0 2021-04-24 18:29:07.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/Devices/__init__.py
--rw-rw-rw-   0        0        0    11655 2023-01-15 20:43:33.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/Evolution.py
--rw-rw-rw-   0        0        0     9323 2022-09-22 13:04:38.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/EvolutionPlots.py
--rw-rw-rw-   0        0        0     1498 2022-09-22 17:48:30.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/Evolution_Individual.py
--rw-rw-rw-   0        0        0    21064 2023-03-08 16:39:15.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/Evolution_UI.py
--rw-rw-rw-   0        0        0     8026 2023-03-07 13:25:34.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/Interface_Functions.py
--rw-rw-rw-   0        0        0    15128 2023-02-26 19:43:49.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/PlotQTObjects.py
--rw-rw-rw-   0        0        0     9012 2023-03-08 16:36:32.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/SSH_Functions.py
--rw-rw-rw-   0        0        0     1974 2023-01-15 20:43:33.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/Single_Evolution_UI.py
--rw-rw-rw-   0        0        0     1237 2023-02-26 19:16:16.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/TxtHighlighter.py
--rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/__init__.py
--rw-rw-rw-   0        0        0    23680 2023-03-10 16:51:47.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/common_UI.py
--rw-rw-rw-   0        0        0     2156 2022-09-22 21:32:55.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/communication.py
--rw-rw-rw-   0        0        0      748 2022-09-22 20:08:23.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/example_master.py
--rw-rw-rw-   0        0        0      281 2022-09-22 20:20:34.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/example_slave.py
--rw-rw-rw-   0        0        0      906 2023-03-22 16:39:46.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/example_slave_2.py
--rw-rw-rw-   0        0        0      970 2022-09-22 21:43:43.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/genome_exchange_com.py
--rw-rw-rw-   0        0        0     7250 2023-03-11 23:57:28.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Execute_UI.py
-drwxrwxrwx   0        0        0        0 2023-03-28 23:19:08.402770 PymoNNto-3.0.0/PymoNNto/Exploration/HelperFunctions/
--rw-rw-rw-   0        0        0     3671 2023-03-12 21:59:55.000000 PymoNNto-3.0.0/PymoNNto/Exploration/HelperFunctions/IteratorFunctions.py
--rw-rw-rw-   0        0        0     2550 2023-02-24 14:22:23.000000 PymoNNto-3.0.0/PymoNNto/Exploration/HelperFunctions/Reconstruction.py
--rw-rw-rw-   0        0        0     4163 2023-03-09 17:40:13.000000 PymoNNto-3.0.0/PymoNNto/Exploration/HelperFunctions/Save_Load.py
--rw-rw-rw-   0        0        0     5057 2023-03-01 10:46:59.000000 PymoNNto-3.0.0/PymoNNto/Exploration/HelperFunctions/Synapses_And_Weights.py
--rw-rw-rw-   0        0        0      428 2023-03-22 16:39:46.000000 PymoNNto-3.0.0/PymoNNto/Exploration/HelperFunctions/Testing.py
--rw-rw-rw-   0        0        0      198 2021-10-07 21:32:07.000000 PymoNNto-3.0.0/PymoNNto/Exploration/HelperFunctions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 23:19:08.418410 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/
-drwxrwxrwx   0        0        0        0 2023-03-28 23:19:08.465293 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Advanced_Tabs/
-drwxrwxrwx   0        0        0        0 2023-03-28 23:19:08.480894 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Advanced_Tabs/Helper/
--rw-rw-rw-   0        0        0     1990 2020-10-28 21:40:32.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Advanced_Tabs/Helper/WP_testing.py
--rw-rw-rw-   0        0        0     8743 2022-04-26 14:19:19.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Advanced_Tabs/Helper/WiltingPriesemann.py
--rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Advanced_Tabs/Helper/__init__.py
--rw-rw-rw-   0        0        0      795 2022-07-31 17:28:29.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Advanced_Tabs/__init__.py
--rw-rw-rw-   0        0        0     2269 2023-02-24 14:50:37.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Advanced_Tabs/afferent_syn_attr_plot_tab.py
--rw-rw-rw-   0        0        0     2192 2021-03-02 21:33:38.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Advanced_Tabs/buffer_tab.py
--rw-rw-rw-   0        0        0     9817 2023-02-24 14:03:22.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Advanced_Tabs/criticality_tab.py
--rw-rw-rw-   0        0        0     1533 2023-03-09 00:40:54.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Advanced_Tabs/scatter_tab.py
--rw-rw-rw-   0        0        0     3675 2022-10-31 19:59:10.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Advanced_Tabs/similarity_matrix_tab.py
--rw-rw-rw-   0        0        0     7543 2021-11-01 17:39:30.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Advanced_Tabs/stdp_buffer_tab.py
-drwxrwxrwx   0        0        0        0 2023-03-28 23:19:08.629451 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/
--rw-rw-rw-   0        0        0     3093 2022-09-05 20:47:16.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/Analysis_Module_tab.py
-drwxrwxrwx   0        0        0        0 2023-03-28 23:19:08.645075 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/Helper/
--rw-rw-rw-   0        0        0      777 2020-10-28 21:40:32.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/Helper/PCA.py
--rw-rw-rw-   0        0        0        0 2022-07-29 09:15:28.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/Helper/__init__.py
--rw-rw-rw-   0        0        0     7050 2023-01-14 13:41:06.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/Helper/syntax.py
--rw-rw-rw-   0        0        0     2507 2023-03-01 10:32:49.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/PCA_tab.py
--rw-rw-rw-   0        0        0     3426 2023-03-08 20:40:16.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/__init__.py
--rw-rw-rw-   0        0        0     3466 2023-02-20 19:37:56.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/classifier_bar_tab.py
--rw-rw-rw-   0        0        0     6975 2023-01-14 13:56:41.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/code_execution_tab.py
--rw-rw-rw-   0        0        0     2201 2022-09-05 20:47:16.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/event_tab.py
--rw-rw-rw-   0        0        0     5013 2023-02-24 14:07:48.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/fourier_tab.py
--rw-rw-rw-   0        0        0     4806 2023-03-09 01:09:12.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/hist_tab.py
--rw-rw-rw-   0        0        0     4353 2023-03-22 16:39:46.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/individual_weight_tab.py
--rw-rw-rw-   0        0        0     5844 2023-03-22 16:39:46.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/info_tabs.py
--rw-rw-rw-   0        0        0     5731 2023-02-24 14:07:49.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/isi_tab.py
--rw-rw-rw-   0        0        0     5901 2023-03-22 16:39:46.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/module_visualizer_tab.py
--rw-rw-rw-   0        0        0     5995 2023-03-09 13:04:34.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/multi_group_plot_tab.py
--rw-rw-rw-   0        0        0     4727 2022-09-05 20:54:05.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/partition_tab.py
--rw-rw-rw-   0        0        0     5531 2023-03-22 16:39:46.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_fast_forward_module.py
--rw-rw-rw-   0        0        0     1175 2023-03-22 16:39:47.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_module_quick_access.py
--rw-rw-rw-   0        0        0    14977 2023-03-09 13:18:07.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_network_selector.py
--rw-rw-rw-   0        0        0     6429 2023-03-09 00:06:00.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_neuron_grid.py
--rw-rw-rw-   0        0        0     2219 2023-03-09 23:11:53.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_save_load_module.py
--rw-rw-rw-   0        0        0     4715 2023-03-07 17:46:14.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/single_group_plot_tab.py
--rw-rw-rw-   0        0        0     1728 2023-03-09 01:03:08.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/spiketrain_tab.py
--rw-rw-rw-   0        0        0     2479 2023-03-09 00:40:54.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/stability_tab.py
--rw-rw-rw-   0        0        0     3958 2023-03-01 10:25:35.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/weight_tab.py
--rw-rw-rw-   0        0        0     4557 2022-09-05 20:54:05.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/weight_tab_old.py
--rw-rw-rw-   0        0        0    11314 2023-03-22 16:39:46.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Network_UI.py
--rw-rw-rw-   0        0        0     2376 2022-07-29 08:17:09.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Neuron_Classification_Colorizer.py
-drwxrwxrwx   0        0        0        0 2023-03-28 23:19:08.708227 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/
--rw-rw-rw-   0        0        0     1020 2021-06-10 09:16:56.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/__init__.py
--rw-rw-rw-   0        0        0     5668 2021-11-01 17:39:29.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/chain_tab.py
--rw-rw-rw-   0        0        0     3296 2023-02-24 14:50:37.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/character_activation_tab.py
--rw-rw-rw-   0        0        0     9285 2023-02-24 14:22:23.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/reconstruction_tab.py
--rw-rw-rw-   0        0        0     1949 2023-03-22 16:39:46.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_drumbeat_module.py
--rw-rw-rw-   0        0        0    14649 2023-03-22 16:39:46.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_grammar_module.py
--rw-rw-rw-   0        0        0     3952 2023-03-22 16:39:46.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_image_module.py
--rw-rw-rw-   0        0        0     3360 2023-03-22 16:39:46.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_music_module.py
--rw-rw-rw-   0        0        0    24057 2023-03-09 00:40:54.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sun_gravity_plot_tab.py
--rw-rw-rw-   0        0        0      791 2023-02-24 14:36:01.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/TabBase.py
--rw-rw-rw-   0        0        0      116 2021-03-02 21:33:38.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/__init__.py
--rw-rw-rw-   0        0        0     4861 2023-01-15 20:43:33.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Overview_UI.py
-drwxrwxrwx   0        0        0        0 2023-03-28 23:19:08.723766 PymoNNto-3.0.0/PymoNNto/Exploration/StorageManager/
--rw-rw-rw-   0        0        0    22549 2023-03-26 19:12:40.000000 PymoNNto-3.0.0/PymoNNto/Exploration/StorageManager/StorageManager.py
--rw-rw-rw-   0        0        0     2665 2021-05-17 22:04:21.000000 PymoNNto-3.0.0/PymoNNto/Exploration/StorageManager/Storage_Manager_Dir_Select_Dialog.py
--rw-rw-rw-   0        0        0      506 2021-06-24 17:39:58.000000 PymoNNto-3.0.0/PymoNNto/Exploration/StorageManager/User_Input_SM_Writer.py
--rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.0/PymoNNto/Exploration/StorageManager/__init__.py
--rw-rw-rw-   0        0        0    27589 2023-03-09 11:16:10.000000 PymoNNto-3.0.0/PymoNNto/Exploration/UI_Base.py
-drwxrwxrwx   0        0        0        0 2023-03-28 23:19:08.755057 PymoNNto-3.0.0/PymoNNto/Exploration/Visualization/
--rw-rw-rw-   0        0        0     1329 2020-10-28 21:40:32.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Visualization/Analysis_Plots.py
--rw-rw-rw-   0        0        0    28252 2023-03-22 16:39:46.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Visualization/Module_visualizer.py
--rw-rw-rw-   0        0        0    14565 2023-03-22 16:39:47.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Visualization/Pyplot_visualizer.py
-drwxrwxrwx   0        0        0        0 2023-03-28 23:19:08.786283 PymoNNto-3.0.0/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/
--rw-rw-rw-   0        0        0     2228 2023-02-24 13:11:58.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/Plot_Synapse_Transition_scatter.py
--rw-rw-rw-   0        0        0     2451 2021-03-02 21:33:38.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/Plot_weights.py
--rw-rw-rw-   0        0        0    26954 2023-03-22 16:39:46.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/Reconstruct_Analyze_Label.py
--rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/__init__.py
--rw-rw-rw-   0        0        0    38124 2021-05-17 22:04:21.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Visualization/SORN_visualization.py
--rw-rw-rw-   0        0        0    12750 2021-07-27 11:37:19.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Visualization/Visualization_Helper.py
--rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Visualization/__init__.py
--rw-rw-rw-   0        0        0     1916 2023-02-24 14:22:23.000000 PymoNNto-3.0.0/PymoNNto/Exploration/Visualization/read_write_np_experiment.py
--rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.0/PymoNNto/Exploration/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 23:19:08.786283 PymoNNto-3.0.0/PymoNNto/NetworkBehavior/
-drwxrwxrwx   0        0        0        0 2023-03-28 23:19:08.801902 PymoNNto-3.0.0/PymoNNto/NetworkBehavior/Basics/
--rw-rw-rw-   0        0        0     4658 2023-03-22 16:38:01.000000 PymoNNto-3.0.0/PymoNNto/NetworkBehavior/Basics/BasicHomeostasis.py
--rw-rw-rw-   0        0        0     2167 2023-03-22 16:39:46.000000 PymoNNto-3.0.0/PymoNNto/NetworkBehavior/Basics/Normalization.py
--rw-rw-rw-   0        0        0      848 2023-02-24 14:22:23.000000 PymoNNto-3.0.0/PymoNNto/NetworkBehavior/Basics/Normalization_Sparse.py
--rw-rw-rw-   0        0        0     1360 2023-03-22 16:38:00.000000 PymoNNto-3.0.0/PymoNNto/NetworkBehavior/Basics/Normalization_Tensorflow.py
--rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.0/PymoNNto/NetworkBehavior/Basics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 23:19:08.833153 PymoNNto-3.0.0/PymoNNto/NetworkBehavior/EulerEquationModules/
--rw-rw-rw-   0        0        0     1334 2023-03-22 16:38:59.000000 PymoNNto-3.0.0/PymoNNto/NetworkBehavior/EulerEquationModules/Equation.py
--rw-rw-rw-   0        0        0      874 2023-03-22 16:38:00.000000 PymoNNto-3.0.0/PymoNNto/NetworkBehavior/EulerEquationModules/EulerClock.py
--rw-rw-rw-   0        0        0     1084 2020-11-11 00:49:45.000000 PymoNNto-3.0.0/PymoNNto/NetworkBehavior/EulerEquationModules/Helper.py
--rw-rw-rw-   0        0        0     1665 2023-03-22 16:39:00.000000 PymoNNto-3.0.0/PymoNNto/NetworkBehavior/EulerEquationModules/VariableInitializer.py
--rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.0/PymoNNto/NetworkBehavior/EulerEquationModules/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 23:19:08.848799 PymoNNto-3.0.0/PymoNNto/NetworkBehavior/Recorder/
--rw-rw-rw-   0        0        0     5903 2023-03-22 16:38:01.000000 PymoNNto-3.0.0/PymoNNto/NetworkBehavior/Recorder/Recorder.py
--rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.0/PymoNNto/NetworkBehavior/Recorder/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 23:19:08.864406 PymoNNto-3.0.0/PymoNNto/NetworkBehavior/Structure/
--rw-rw-rw-   0        0        0     2793 2023-03-22 16:38:01.000000 PymoNNto-3.0.0/PymoNNto/NetworkBehavior/Structure/Partition.py
--rw-rw-rw-   0        0        0     3751 2023-03-22 16:39:00.000000 PymoNNto-3.0.0/PymoNNto/NetworkBehavior/Structure/Receptive_Fields.py
--rw-rw-rw-   0        0        0     6616 2023-03-22 16:38:01.000000 PymoNNto-3.0.0/PymoNNto/NetworkBehavior/Structure/Structure.py
--rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.0/PymoNNto/NetworkBehavior/Structure/__init__.py
--rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.0/PymoNNto/NetworkBehavior/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 23:19:08.911278 PymoNNto-3.0.0/PymoNNto/NetworkCore/
--rw-rw-rw-   0        0        0     5305 2023-03-25 09:00:49.000000 PymoNNto-3.0.0/PymoNNto/NetworkCore/Analysis_Module.py
--rw-rw-rw-   0        0        0     9183 2023-03-25 08:52:17.000000 PymoNNto-3.0.0/PymoNNto/NetworkCore/Base_Attachable_Modules.py
--rw-rw-rw-   0        0        0     2392 2023-03-25 08:56:09.000000 PymoNNto-3.0.0/PymoNNto/NetworkCore/Base_Tagable_Object.py
--rw-rw-rw-   0        0        0     6858 2023-03-28 22:58:37.000000 PymoNNto-3.0.0/PymoNNto/NetworkCore/Behavior.py
--rw-rw-rw-   0        0        0    12315 2023-03-25 09:24:36.000000 PymoNNto-3.0.0/PymoNNto/NetworkCore/Network.py
--rw-rw-rw-   0        0        0    10832 2023-03-25 09:00:49.000000 PymoNNto-3.0.0/PymoNNto/NetworkCore/Neuron_Group.py
--rw-rw-rw-   0        0        0     6841 2023-03-25 09:00:49.000000 PymoNNto-3.0.0/PymoNNto/NetworkCore/Synapse_Group.py
--rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.0/PymoNNto/NetworkCore/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-28 23:19:08.911278 PymoNNto-3.0.0/PymoNNto/UI/
--rw-rw-rw-   0        0        0        2 2023-01-15 20:43:33.000000 PymoNNto-3.0.0/PymoNNto/UI/__init__.py
--rw-rw-rw-   0        0        0      836 2023-03-22 16:39:00.000000 PymoNNto-3.0.0/PymoNNto/__init__.py
--rw-rw-rw-   0        0        0      441 2021-05-06 16:02:17.000000 PymoNNto-3.0.0/PymoNNto/create_readme.py
--rw-rw-rw-   0        0        0     2438 2023-03-22 16:39:00.000000 PymoNNto-3.0.0/PymoNNto/sync_docs.py
--rw-rw-rw-   0        0        0     9014 2023-03-22 16:39:46.000000 PymoNNto-3.0.0/PymoNNto/test_pymoNNto.py
-drwxrwxrwx   0        0        0        0 2023-03-28 23:19:08.184002 PymoNNto-3.0.0/PymoNNto.egg-info/
--rw-rw-rw-   0        0        0      678 2023-03-28 23:19:07.000000 PymoNNto-3.0.0/PymoNNto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7731 2023-03-28 23:19:08.000000 PymoNNto-3.0.0/PymoNNto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 23:19:07.000000 PymoNNto-3.0.0/PymoNNto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      178 2023-03-28 23:19:07.000000 PymoNNto-3.0.0/PymoNNto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       87 2023-03-28 23:19:07.000000 PymoNNto-3.0.0/PymoNNto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-28 23:19:07.000000 PymoNNto-3.0.0/PymoNNto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      229 2021-03-04 15:34:19.000000 PymoNNto-3.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-03-28 23:19:08.911278 PymoNNto-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1098 2023-03-28 23:18:13.000000 PymoNNto-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-24 00:51:20.132420 PymoNNto-3.0.1/
+-rw-rw-rw-   0        0        0     1073 2020-12-02 18:45:09.000000 PymoNNto-3.0.1/LICENSE
+-rw-rw-rw-   0        0        0      678 2023-07-24 00:51:20.132420 PymoNNto-3.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-24 00:51:19.945112 PymoNNto-3.0.1/PymoNNto/
+-rw-rw-rw-   0        0        0      448 2023-03-22 16:38:59.000000 PymoNNto-3.0.1/PymoNNto/CLI.py
+drwxrwxrwx   0        0        0        0 2023-07-24 00:51:19.975764 PymoNNto-3.0.1/PymoNNto/Exploration/
+drwxrwxrwx   0        0        0        0 2023-07-24 00:51:19.975764 PymoNNto-3.0.1/PymoNNto/Exploration/AnalysisModules/
+-rw-rw-rw-   0        0        0      548 2023-02-24 14:24:06.000000 PymoNNto-3.0.1/PymoNNto/Exploration/AnalysisModules/Static_Classification.py
+-rw-rw-rw-   0        0        0     3571 2023-03-09 20:27:54.000000 PymoNNto-3.0.1/PymoNNto/Exploration/AnalysisModules/Weight_Classifier_Base.py
+-rw-rw-rw-   0        0        0      289 2023-02-24 14:24:06.000000 PymoNNto-3.0.1/PymoNNto/Exploration/AnalysisModules/Weight_Classifier_Post.py
+-rw-rw-rw-   0        0        0      288 2023-02-24 14:24:06.000000 PymoNNto-3.0.1/PymoNNto/Exploration/AnalysisModules/Weight_Classifier_Pre.py
+-rw-rw-rw-   0        0        0      221 2022-07-29 10:15:40.000000 PymoNNto-3.0.1/PymoNNto/Exploration/AnalysisModules/__init__.py
+-rw-rw-rw-   0        0        0    10819 2023-03-22 16:39:46.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Behaviour_UI.py
+drwxrwxrwx   0        0        0        0 2023-07-24 00:51:19.991388 PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/
+-rw-rw-rw-   0        0        0     5032 2023-02-15 19:37:04.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/Breed_And_Selection_Module.py
+drwxrwxrwx   0        0        0        0 2023-07-24 00:51:20.007018 PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/Devices/
+-rw-rw-rw-   0        0        0     2471 2023-03-07 13:25:34.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/Devices/Evolution_Device.py
+-rw-rw-rw-   0        0        0     2205 2022-09-21 18:37:13.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/Devices/Evolution_Device_Multi_Thread.py
+-rw-rw-rw-   0        0        0     2514 2022-12-08 02:47:35.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/Devices/Evolution_Device_SSH.py
+-rw-rw-rw-   0        0        0      796 2022-09-21 17:40:35.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/Devices/Evolution_Device_Single_Thread.py
+-rw-rw-rw-   0        0        0        0 2021-04-24 18:29:07.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/Devices/__init__.py
+-rw-rw-rw-   0        0        0    11655 2023-01-15 20:43:33.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/Evolution.py
+-rw-rw-rw-   0        0        0     9323 2022-09-22 13:04:38.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/EvolutionPlots.py
+-rw-rw-rw-   0        0        0     1498 2022-09-22 17:48:30.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/Evolution_Individual.py
+-rw-rw-rw-   0        0        0    21064 2023-03-08 16:39:15.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/Evolution_UI.py
+-rw-rw-rw-   0        0        0     8026 2023-03-07 13:25:34.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/Interface_Functions.py
+-rw-rw-rw-   0        0        0    15128 2023-02-26 19:43:49.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/PlotQTObjects.py
+-rw-rw-rw-   0        0        0     9012 2023-03-08 16:36:32.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/SSH_Functions.py
+-rw-rw-rw-   0        0        0     1974 2023-01-15 20:43:33.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/Single_Evolution_UI.py
+-rw-rw-rw-   0        0        0     1237 2023-02-26 19:16:16.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/TxtHighlighter.py
+-rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/__init__.py
+-rw-rw-rw-   0        0        0    23680 2023-03-10 16:51:47.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/common_UI.py
+-rw-rw-rw-   0        0        0     2156 2022-09-22 21:32:55.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/communication.py
+-rw-rw-rw-   0        0        0      748 2022-09-22 20:08:23.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/example_master.py
+-rw-rw-rw-   0        0        0      281 2022-09-22 20:20:34.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/example_slave.py
+-rw-rw-rw-   0        0        0      906 2023-03-22 16:39:46.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/example_slave_2.py
+-rw-rw-rw-   0        0        0      970 2022-09-22 21:43:43.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/genome_exchange_com.py
+-rw-rw-rw-   0        0        0     7250 2023-03-11 23:57:28.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Execute_UI.py
+drwxrwxrwx   0        0        0        0 2023-07-24 00:51:20.007018 PymoNNto-3.0.1/PymoNNto/Exploration/HelperFunctions/
+-rw-rw-rw-   0        0        0     3671 2023-03-12 21:59:55.000000 PymoNNto-3.0.1/PymoNNto/Exploration/HelperFunctions/IteratorFunctions.py
+-rw-rw-rw-   0        0        0     2550 2023-02-24 14:22:23.000000 PymoNNto-3.0.1/PymoNNto/Exploration/HelperFunctions/Reconstruction.py
+-rw-rw-rw-   0        0        0     4163 2023-03-09 17:40:13.000000 PymoNNto-3.0.1/PymoNNto/Exploration/HelperFunctions/Save_Load.py
+-rw-rw-rw-   0        0        0     5061 2023-04-27 08:20:12.000000 PymoNNto-3.0.1/PymoNNto/Exploration/HelperFunctions/Synapses_And_Weights.py
+-rw-rw-rw-   0        0        0      428 2023-03-22 16:39:46.000000 PymoNNto-3.0.1/PymoNNto/Exploration/HelperFunctions/Testing.py
+-rw-rw-rw-   0        0        0      198 2021-10-07 21:32:07.000000 PymoNNto-3.0.1/PymoNNto/Exploration/HelperFunctions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 00:51:20.022643 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/
+drwxrwxrwx   0        0        0        0 2023-07-24 00:51:20.022643 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Advanced_Tabs/
+drwxrwxrwx   0        0        0        0 2023-07-24 00:51:20.038262 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Advanced_Tabs/Helper/
+-rw-rw-rw-   0        0        0     1990 2020-10-28 21:40:32.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Advanced_Tabs/Helper/WP_testing.py
+-rw-rw-rw-   0        0        0     8743 2022-04-26 14:19:19.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Advanced_Tabs/Helper/WiltingPriesemann.py
+-rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Advanced_Tabs/Helper/__init__.py
+-rw-rw-rw-   0        0        0      795 2022-07-31 17:28:29.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Advanced_Tabs/__init__.py
+-rw-rw-rw-   0        0        0     2245 2023-04-27 08:23:13.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Advanced_Tabs/afferent_syn_attr_plot_tab.py
+-rw-rw-rw-   0        0        0     2192 2021-03-02 21:33:38.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Advanced_Tabs/buffer_tab.py
+-rw-rw-rw-   0        0        0     9817 2023-02-24 14:03:22.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Advanced_Tabs/criticality_tab.py
+-rw-rw-rw-   0        0        0     1533 2023-03-09 00:40:54.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Advanced_Tabs/scatter_tab.py
+-rw-rw-rw-   0        0        0     3675 2022-10-31 19:59:10.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Advanced_Tabs/similarity_matrix_tab.py
+-rw-rw-rw-   0        0        0     7537 2023-04-27 08:19:21.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Advanced_Tabs/stdp_buffer_tab.py
+drwxrwxrwx   0        0        0        0 2023-07-24 00:51:20.069926 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/
+-rw-rw-rw-   0        0        0     3093 2022-09-05 20:47:16.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/Analysis_Module_tab.py
+drwxrwxrwx   0        0        0        0 2023-07-24 00:51:20.069926 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/Helper/
+-rw-rw-rw-   0        0        0      777 2020-10-28 21:40:32.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/Helper/PCA.py
+-rw-rw-rw-   0        0        0        0 2022-07-29 09:15:28.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/Helper/__init__.py
+-rw-rw-rw-   0        0        0     7050 2023-01-14 13:41:06.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/Helper/syntax.py
+-rw-rw-rw-   0        0        0     2507 2023-03-01 10:32:49.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/PCA_tab.py
+-rw-rw-rw-   0        0        0     3426 2023-03-08 20:40:16.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/__init__.py
+-rw-rw-rw-   0        0        0     3466 2023-02-20 19:37:56.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/classifier_bar_tab.py
+-rw-rw-rw-   0        0        0     6977 2023-04-27 08:20:12.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/code_execution_tab.py
+-rw-rw-rw-   0        0        0     2201 2022-09-05 20:47:16.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/event_tab.py
+-rw-rw-rw-   0        0        0     5013 2023-02-24 14:07:48.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/fourier_tab.py
+-rw-rw-rw-   0        0        0     4807 2023-04-27 08:25:37.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/hist_tab.py
+-rw-rw-rw-   0        0        0     4329 2023-04-27 08:23:13.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/individual_weight_tab.py
+-rw-rw-rw-   0        0        0     5844 2023-03-22 16:39:46.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/info_tabs.py
+-rw-rw-rw-   0        0        0     5731 2023-02-24 14:07:49.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/isi_tab.py
+-rw-rw-rw-   0        0        0     5901 2023-03-22 16:39:46.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/module_visualizer_tab.py
+-rw-rw-rw-   0        0        0     5995 2023-03-09 13:04:34.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/multi_group_plot_tab.py
+-rw-rw-rw-   0        0        0     4728 2023-04-27 08:25:37.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/partition_tab.py
+-rw-rw-rw-   0        0        0     5531 2023-03-22 16:39:46.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_fast_forward_module.py
+-rw-rw-rw-   0        0        0     1175 2023-03-22 16:39:47.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_module_quick_access.py
+-rw-rw-rw-   0        0        0    14977 2023-03-09 13:18:07.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_network_selector.py
+-rw-rw-rw-   0        0        0     6429 2023-03-09 00:06:00.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_neuron_grid.py
+-rw-rw-rw-   0        0        0     2219 2023-03-09 23:11:53.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_save_load_module.py
+-rw-rw-rw-   0        0        0     4715 2023-03-07 17:46:14.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/single_group_plot_tab.py
+-rw-rw-rw-   0        0        0     1728 2023-03-09 01:03:08.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/spiketrain_tab.py
+-rw-rw-rw-   0        0        0     2479 2023-03-09 00:40:54.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/stability_tab.py
+-rw-rw-rw-   0        0        0     3962 2023-07-23 15:55:59.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/weight_tab.py
+-rw-rw-rw-   0        0        0     4559 2023-04-27 08:25:37.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/weight_tab_old.py
+-rw-rw-rw-   0        0        0    11308 2023-04-27 08:19:21.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Network_UI.py
+-rw-rw-rw-   0        0        0     2376 2022-07-29 08:17:09.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Neuron_Classification_Colorizer.py
+drwxrwxrwx   0        0        0        0 2023-07-24 00:51:20.085548 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/
+-rw-rw-rw-   0        0        0     1020 2021-06-10 09:16:56.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/__init__.py
+-rw-rw-rw-   0        0        0     5668 2021-11-01 17:39:29.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/chain_tab.py
+-rw-rw-rw-   0        0        0     3296 2023-02-24 14:50:37.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/character_activation_tab.py
+-rw-rw-rw-   0        0        0     9285 2023-02-24 14:22:23.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/reconstruction_tab.py
+-rw-rw-rw-   0        0        0     1949 2023-03-22 16:39:46.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_drumbeat_module.py
+-rw-rw-rw-   0        0        0    14649 2023-03-22 16:39:46.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_grammar_module.py
+-rw-rw-rw-   0        0        0     3952 2023-03-22 16:39:46.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_image_module.py
+-rw-rw-rw-   0        0        0     3360 2023-03-22 16:39:46.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_music_module.py
+-rw-rw-rw-   0        0        0    24060 2023-04-27 08:16:20.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sun_gravity_plot_tab.py
+-rw-rw-rw-   0        0        0      791 2023-02-24 14:36:01.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/TabBase.py
+-rw-rw-rw-   0        0        0      116 2021-03-02 21:33:38.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/__init__.py
+-rw-rw-rw-   0        0        0     4861 2023-01-15 20:43:33.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Overview_UI.py
+drwxrwxrwx   0        0        0        0 2023-07-24 00:51:20.085548 PymoNNto-3.0.1/PymoNNto/Exploration/StorageManager/
+-rw-rw-rw-   0        0        0     4333 2023-03-29 10:48:53.000000 PymoNNto-3.0.1/PymoNNto/Exploration/StorageManager/SM2.py
+-rw-rw-rw-   0        0        0    18314 2023-03-29 10:48:17.000000 PymoNNto-3.0.1/PymoNNto/Exploration/StorageManager/StorageManager.py
+-rw-rw-rw-   0        0        0     2665 2021-05-17 22:04:21.000000 PymoNNto-3.0.1/PymoNNto/Exploration/StorageManager/Storage_Manager_Dir_Select_Dialog.py
+-rw-rw-rw-   0        0        0      506 2021-06-24 17:39:58.000000 PymoNNto-3.0.1/PymoNNto/Exploration/StorageManager/User_Input_SM_Writer.py
+-rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.1/PymoNNto/Exploration/StorageManager/__init__.py
+-rw-rw-rw-   0        0        0    27589 2023-03-09 11:16:10.000000 PymoNNto-3.0.1/PymoNNto/Exploration/UI_Base.py
+drwxrwxrwx   0        0        0        0 2023-07-24 00:51:20.101173 PymoNNto-3.0.1/PymoNNto/Exploration/Visualization/
+-rw-rw-rw-   0        0        0     1329 2020-10-28 21:40:32.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Visualization/Analysis_Plots.py
+-rw-rw-rw-   0        0        0    28252 2023-04-27 08:28:05.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Visualization/Module_visualizer.py
+-rw-rw-rw-   0        0        0    14565 2023-03-22 16:39:47.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Visualization/Pyplot_visualizer.py
+drwxrwxrwx   0        0        0        0 2023-07-24 00:51:20.101173 PymoNNto-3.0.1/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/
+-rw-rw-rw-   0        0        0     2228 2023-02-24 13:11:58.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/Plot_Synapse_Transition_scatter.py
+-rw-rw-rw-   0        0        0     2451 2021-03-02 21:33:38.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/Plot_weights.py
+-rw-rw-rw-   0        0        0    27400 2023-05-04 13:11:42.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/Reconstruct_Analyze_Label.py
+-rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/__init__.py
+-rw-rw-rw-   0        0        0    38124 2021-05-17 22:04:21.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Visualization/SORN_visualization.py
+-rw-rw-rw-   0        0        0    12752 2023-04-27 08:22:49.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Visualization/Visualization_Helper.py
+-rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Visualization/__init__.py
+-rw-rw-rw-   0        0        0     1916 2023-02-24 14:22:23.000000 PymoNNto-3.0.1/PymoNNto/Exploration/Visualization/read_write_np_experiment.py
+-rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.1/PymoNNto/Exploration/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 00:51:20.101173 PymoNNto-3.0.1/PymoNNto/NetworkBehavior/
+drwxrwxrwx   0        0        0        0 2023-07-24 00:51:20.101173 PymoNNto-3.0.1/PymoNNto/NetworkBehavior/Basics/
+-rw-rw-rw-   0        0        0     4658 2023-03-22 16:38:01.000000 PymoNNto-3.0.1/PymoNNto/NetworkBehavior/Basics/BasicHomeostasis.py
+-rw-rw-rw-   0        0        0     2229 2023-05-04 13:41:26.000000 PymoNNto-3.0.1/PymoNNto/NetworkBehavior/Basics/Normalization.py
+-rw-rw-rw-   0        0        0      901 2023-05-04 13:41:26.000000 PymoNNto-3.0.1/PymoNNto/NetworkBehavior/Basics/Normalization_Sparse.py
+-rw-rw-rw-   0        0        0     1411 2023-05-04 13:41:26.000000 PymoNNto-3.0.1/PymoNNto/NetworkBehavior/Basics/Normalization_Tensorflow.py
+-rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.1/PymoNNto/NetworkBehavior/Basics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 00:51:20.116800 PymoNNto-3.0.1/PymoNNto/NetworkBehavior/EulerEquationModules/
+-rw-rw-rw-   0        0        0     1334 2023-03-22 16:38:59.000000 PymoNNto-3.0.1/PymoNNto/NetworkBehavior/EulerEquationModules/Equation.py
+-rw-rw-rw-   0        0        0      874 2023-03-22 16:38:00.000000 PymoNNto-3.0.1/PymoNNto/NetworkBehavior/EulerEquationModules/EulerClock.py
+-rw-rw-rw-   0        0        0     1084 2020-11-11 00:49:45.000000 PymoNNto-3.0.1/PymoNNto/NetworkBehavior/EulerEquationModules/Helper.py
+-rw-rw-rw-   0        0        0     1665 2023-03-22 16:39:00.000000 PymoNNto-3.0.1/PymoNNto/NetworkBehavior/EulerEquationModules/VariableInitializer.py
+-rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.1/PymoNNto/NetworkBehavior/EulerEquationModules/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 00:51:20.116800 PymoNNto-3.0.1/PymoNNto/NetworkBehavior/Recorder/
+-rw-rw-rw-   0        0        0     5905 2023-07-20 01:29:36.000000 PymoNNto-3.0.1/PymoNNto/NetworkBehavior/Recorder/Recorder.py
+-rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.1/PymoNNto/NetworkBehavior/Recorder/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 00:51:20.116800 PymoNNto-3.0.1/PymoNNto/NetworkBehavior/Structure/
+-rw-rw-rw-   0        0        0     2793 2023-03-22 16:38:01.000000 PymoNNto-3.0.1/PymoNNto/NetworkBehavior/Structure/Partition.py
+-rw-rw-rw-   0        0        0     3751 2023-03-22 16:39:00.000000 PymoNNto-3.0.1/PymoNNto/NetworkBehavior/Structure/Receptive_Fields.py
+-rw-rw-rw-   0        0        0     6616 2023-03-22 16:38:01.000000 PymoNNto-3.0.1/PymoNNto/NetworkBehavior/Structure/Structure.py
+-rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.1/PymoNNto/NetworkBehavior/Structure/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.1/PymoNNto/NetworkBehavior/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 00:51:20.132420 PymoNNto-3.0.1/PymoNNto/NetworkCore/
+-rw-rw-rw-   0        0        0     5305 2023-03-25 09:00:49.000000 PymoNNto-3.0.1/PymoNNto/NetworkCore/Analysis_Module.py
+-rw-rw-rw-   0        0        0     9245 2023-05-04 13:17:01.000000 PymoNNto-3.0.1/PymoNNto/NetworkCore/Base_Attachable_Modules.py
+-rw-rw-rw-   0        0        0     2392 2023-03-25 08:56:09.000000 PymoNNto-3.0.1/PymoNNto/NetworkCore/Base_Tagable_Object.py
+-rw-rw-rw-   0        0        0     6858 2023-03-28 22:58:37.000000 PymoNNto-3.0.1/PymoNNto/NetworkCore/Behavior.py
+-rw-rw-rw-   0        0        0    12338 2023-05-04 13:17:01.000000 PymoNNto-3.0.1/PymoNNto/NetworkCore/Network.py
+-rw-rw-rw-   0        0        0    10839 2023-05-04 09:09:31.000000 PymoNNto-3.0.1/PymoNNto/NetworkCore/Neuron_Group.py
+-rw-rw-rw-   0        0        0     6843 2023-05-04 08:17:05.000000 PymoNNto-3.0.1/PymoNNto/NetworkCore/Synapse_Group.py
+-rw-rw-rw-   0        0        0        0 2020-10-28 21:40:32.000000 PymoNNto-3.0.1/PymoNNto/NetworkCore/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-24 00:51:20.132420 PymoNNto-3.0.1/PymoNNto/UI/
+-rw-rw-rw-   0        0        0        2 2023-01-15 20:43:33.000000 PymoNNto-3.0.1/PymoNNto/UI/__init__.py
+-rw-rw-rw-   0        0        0      836 2023-03-22 16:39:00.000000 PymoNNto-3.0.1/PymoNNto/__init__.py
+-rw-rw-rw-   0        0        0      441 2021-05-06 16:02:17.000000 PymoNNto-3.0.1/PymoNNto/create_readme.py
+-rw-rw-rw-   0        0        0     2438 2023-03-22 16:39:00.000000 PymoNNto-3.0.1/PymoNNto/sync_docs.py
+-rw-rw-rw-   0        0        0     9015 2023-05-04 13:35:29.000000 PymoNNto-3.0.1/PymoNNto/test_pymoNNto.py
+drwxrwxrwx   0        0        0        0 2023-07-24 00:51:19.960124 PymoNNto-3.0.1/PymoNNto.egg-info/
+-rw-rw-rw-   0        0        0      678 2023-07-24 00:51:19.000000 PymoNNto-3.0.1/PymoNNto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7774 2023-07-24 00:51:19.000000 PymoNNto-3.0.1/PymoNNto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 00:51:19.000000 PymoNNto-3.0.1/PymoNNto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      178 2023-07-24 00:51:19.000000 PymoNNto-3.0.1/PymoNNto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       87 2023-07-24 00:51:19.000000 PymoNNto-3.0.1/PymoNNto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-24 00:51:19.000000 PymoNNto-3.0.1/PymoNNto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      229 2021-03-04 15:34:19.000000 PymoNNto-3.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-24 00:51:20.132420 PymoNNto-3.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1098 2023-07-24 00:51:13.000000 PymoNNto-3.0.1/setup.py
```

### Comparing `PymoNNto-3.0.0/LICENSE` & `PymoNNto-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PKG-INFO` & `PymoNNto-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PymoNNto
-Version: 3.0.0
+Version: 3.0.1
 Summary: Python Modular Neural Network Toolbox
 Home-page: https://github.com/trieschlab/PymoNNto
 Author: Marius Vieth
 Author-email: mv15go@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/AnalysisModules/Static_Classification.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/AnalysisModules/Static_Classification.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/AnalysisModules/Weight_Classifier_Base.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/AnalysisModules/Weight_Classifier_Base.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Behaviour_UI.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Behaviour_UI.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/Breed_And_Selection_Module.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/Breed_And_Selection_Module.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/Devices/Evolution_Device.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/Devices/Evolution_Device.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/Devices/Evolution_Device_Multi_Thread.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/Devices/Evolution_Device_Multi_Thread.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/Devices/Evolution_Device_SSH.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/Devices/Evolution_Device_SSH.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/Devices/Evolution_Device_Single_Thread.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/Devices/Evolution_Device_Single_Thread.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/Evolution.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/Evolution.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/EvolutionPlots.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/EvolutionPlots.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/Evolution_Individual.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/Evolution_Individual.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/Evolution_UI.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/Evolution_UI.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/Interface_Functions.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/Interface_Functions.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/PlotQTObjects.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/PlotQTObjects.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/SSH_Functions.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/SSH_Functions.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/Single_Evolution_UI.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/Single_Evolution_UI.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/TxtHighlighter.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/TxtHighlighter.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/common_UI.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/common_UI.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/communication.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/communication.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/example_master.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/example_master.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/example_slave_2.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/example_slave_2.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Evolution/genome_exchange_com.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Evolution/genome_exchange_com.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Execute_UI.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Execute_UI.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/HelperFunctions/IteratorFunctions.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/HelperFunctions/IteratorFunctions.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/HelperFunctions/Reconstruction.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/HelperFunctions/Reconstruction.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/HelperFunctions/Save_Load.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/HelperFunctions/Save_Load.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/HelperFunctions/Synapses_And_Weights.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/HelperFunctions/Synapses_And_Weights.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #########################################
 ####Partitioned
 #########################################
 
 def get_partitioned_synapse_matrix(neurons, synapse_tag, synapse_var, return_first=True):
     results = {}
     shapes = {}
-    for s in neurons.afferent_synapses[synapse_tag]:
+    for s in neurons.synapses(afferent, synapse_tag):
         base_src = s.src.group_without_subGroup()
         base_dst = s.dst.group_without_subGroup()
         key = ','.join(s.tags)
         if not key in results:
             results[key] = np.zeros((base_dst.size, base_src.size))
             shapes[key] = (base_src.height, base_src.width)
         try:
@@ -46,25 +46,25 @@
 
     if return_first:
         return list(results.values())[0]
     else:
         return results
 
 def set_partitioned_synapse_matrix(neurons, synapse_tag, synapse_var, mat):#warning! synapse_tag has to be unique and only used by partition synapses
-    for s in neurons.afferent_synapses[synapse_tag]:
+    for s in neurons.synapses(afferent, synapse_tag):
         try:
             mask = s.dst.mask[:, None] * s.src.mask[None, :]
             setattr(s, synapse_var, mat[mask].reshape(s.matrix_dim()))
         except:
             print(synapse_var, "cannot be set")
 
 
 def SingleNeuron_attached_SubSGs(neuron_group, synapse_tag, neuron_id):
     result = []
-    for s in neuron_group.afferent_synapses[synapse_tag]:
+    for s in neuron_group.synapses(afferent, synapse_tag):
         if neuron_id in s.dst.id:
             result.append(s)
     return result
 
 def get_single_neuron_combined_partition_matrix(neurons, synapse_tag, synapse_var, neuron_id, return_first=True):
     results = []
     for s in SingleNeuron_attached_SubSGs(neurons, synapse_tag, neuron_id):
@@ -91,15 +91,15 @@
 #            mask = s.dst.mask[:, None] * s.src.mask[None, :]
 #            setattr(s, synapse_var, mat[mask].reshape(s.matrix_dim()))
 #        except:
 #            print(synapse_var, "cannot be set")
 
 
 #def get_partitioned_matrix(neuron, synapse_tag, synapse_var):
-#    return list(get_combined_syn_mats(neuron.afferent_synapses[synapse_tag], None, synapse_var).values())[0]
+#    return list(get_combined_syn_mats(neuron.synapses(afferent, synapse_tag), None, synapse_var).values())[0]
 
 #def set_partitioned_matrix(neuron, synapse_tag, synapse_var, mat):
 
 
 
 #########################################
 ####Old
```

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Advanced_Tabs/Helper/WP_testing.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Advanced_Tabs/Helper/WP_testing.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Advanced_Tabs/Helper/WiltingPriesemann.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Advanced_Tabs/Helper/WiltingPriesemann.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Advanced_Tabs/__init__.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Advanced_Tabs/__init__.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Advanced_Tabs/afferent_syn_attr_plot_tab.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Advanced_Tabs/afferent_syn_attr_plot_tab.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,19 +8,19 @@
         self.syn_vars=syn_vars
         self.timesteps=timesteps
 
     def add_recorder_variables(self, neuron_group, Network_UI):
         self.check={}
         for syn_var in self.syn_vars:
             self.check[syn_var] = True
-            for syn in neuron_group.afferent_synapses["All"]:
+            for syn in neuron_group.synapses(afferent):
                 if not hasattr(syn, syn_var):
                     self.check[syn_var] = False
             if self.check[syn_var]:
-                Network_UI.add_recording_variable(neuron_group, '[np.sum(s.'+syn_var+') for s in n.afferent_synapses["All"]]', timesteps=self.timesteps)
+                Network_UI.add_recording_variable(neuron_group, '[np.sum(s.'+syn_var+') for s in n.synapses(afferent)]', timesteps=self.timesteps)
 
     def initialize(self, Network_UI):
         self.weight_tab = Network_UI.Next_Tab(self.title)
 
         self.plots = {}
         for syn_var in self.syn_vars:
             _, syn_plt = Network_UI.Add_plot_curve('Neuron Group average ' + syn_var, return_plot=True, x_label='t (iterations)', y_label='Input')
@@ -35,19 +35,19 @@
 
             for syn_var in self.syn_vars:
 
                 if self.check[syn_var]:
 
                     self.plots[syn_var].clear()
 
-                    recorded = group['[np.sum(s.'+syn_var+') for s in n.afferent_synapses["All"]]'][-self.timesteps:]
+                    recorded = group['[np.sum(s.'+syn_var+') for s in n.synapses(afferent)]'][-self.timesteps:]
                     iterations = group['iteration', 0, 'np'][-self.timesteps:]
                     if len(recorded) > 0:
                         inputs = np.array(recorded[0])
-                        ident=[s.src.group_without_subGroup() for s in group.afferent_synapses["All"]]
+                        ident=[s.src.group_without_subGroup() for s in group.synapses(afferent)]
                         single_ident = list(set(ident))
 
                         for i, si in enumerate(single_ident):
                             mask = [id == si for id in ident]
 
                             data = np.sum(inputs[:, mask], axis=1)
                             curve = pg.PlotCurveItem(iterations, data, name='', pen=si.color)#self.slow_input_colors[i]
```

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Advanced_Tabs/buffer_tab.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Advanced_Tabs/buffer_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Advanced_Tabs/criticality_tab.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Advanced_Tabs/criticality_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Advanced_Tabs/scatter_tab.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Advanced_Tabs/scatter_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Advanced_Tabs/similarity_matrix_tab.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Advanced_Tabs/similarity_matrix_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Advanced_Tabs/stdp_buffer_tab.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Advanced_Tabs/stdp_buffer_tab.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         y_zoom = p_t.y() - y_shift
         return x_shift, y_shift, x_zoom, y_zoom
 
     def update(self, Network_UI):
         if self.stdp_tab.isVisible():
 
             group = Network_UI.selected_neuron_group()
-            synapse_groups = group.afferent_synapses['All']
+            synapse_groups = group.synapses(afferent)
             #print(synapse_groups)
 
             if self.current_selector_group != group:
                 self.current_selector_group = group
                 self.select_syn_box.clear()
                 self.current_selector_index_dict.clear()
                 self.current_selector_index_dict[-1]=-1
```

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/Analysis_Module_tab.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/Analysis_Module_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/Helper/PCA.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/Helper/PCA.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/Helper/syntax.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/Helper/syntax.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/PCA_tab.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/PCA_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/__init__.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/__init__.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/classifier_bar_tab.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/classifier_bar_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/code_execution_tab.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/code_execution_tab.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 class code_execution_tab(TabBase):
 
     sample_code1='''import matplotlib.pyplot as plt
 
 synapse_tag='GLU'
 synapse_var='W'
 
-combined = get_combined_syn_mats(n.afferent_synapses[synapse_tag], None,synapse_var)
+combined = get_combined_syn_mats(n.synapses(afferent, synapse_tag), None,synapse_var)
 
 for mat in combined.values():
 
 	plt.imshow(mat, vmin=0, vmax=0.005)#cmap='gray', 
 	plt.show()
 '''
 
     sample_code2='''num=0
 
-for syn in n.afferent_synapses['GLU']:
+for syn in n.synapses(afferent, 'GLU'):
 
 	num+=np.sum(syn.W>0.001)
 
 print(num)
 '''
 
     base_code = '''###Quick Access Variables###
```

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/event_tab.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/event_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/fourier_tab.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/fourier_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/hist_tab.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/hist_tab.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         bins = self.bin_slider.sliderPosition()
 
         for transmitter in Network_UI.transmitters:
 
             self.net_weight_hist_plots[transmitter].clear()
             self.weight_hist_plots[transmitter].clear()
 
-            glu_syns = group.afferent_synapses[transmitter]
+            glu_syns = group.synapses(afferent, transmitter)
             if len(glu_syns) > 0:
 
                 GLU_syn_list = get_combined_syn_mats(glu_syns, None, self.weight_attr)
                 GLU_syn_list_en = get_combined_syn_mats(glu_syns, None, "enabled")
                 if len(GLU_syn_list) > 0:
                     GLU_syn = GLU_syn_list[list(GLU_syn_list.keys())[0]]
                     en_mask = GLU_syn_list_en[list(GLU_syn_list_en.keys())[0]].astype(bool)*(GLU_syn > min_weight)*(GLU_syn < max_weight)#GLU_syn > msl
```

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/individual_weight_tab.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/individual_weight_tab.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         Network_UI.Add_element(self.min_w_slider)
 
 
     def start_rec(self, group):
 
         if self.current_ng is not None and (self.neuron_index != self.Network_UI.selected_neuron_id() or self.current_ng != group):
 
-            for s in self.current_ng.afferent_synapses["All"]:
+            for s in self.current_ng.synapses(afferent):
                 s.UI_recorder = None
                 s.cb = None
                 self.Network_UI.network.remove_behaviors_from_object(s, tags=[self.key])
 
             self.listWidget.clear()
             self.plot.clear()
 
@@ -62,15 +62,15 @@
             self.plot.clear()
 
             self.key = self.weight_attr+'['+str(self.neuron_index)+']'
 
             self.checkboxes={}
             self.listWidget.clear()
 
-            for s in group.afferent_synapses["All"]:
+            for s in group.synapses(afferent):
                 s.UI_recorder = Recorder([self.key, 'iteration'], tag=self.rec_name, gapwidth=10, save_as_numpy=True)
                 s.add_behavior(10001, s.UI_recorder)
                 #self.Network_UI.network.add_behaviors_to_object({10001: s.UI_recorder}, s)
 
                 s.UI_curves = []
                 syn_data = eval(self.key)
 
@@ -90,25 +90,25 @@
     def update(self, Network_UI):
 
         if self.individual_weight_tab.isVisible():
 
             group = Network_UI.selected_neuron_group()
             self.start_rec(group)
 
-            for s in self.current_ng.afferent_synapses["All"]:
+            for s in self.current_ng.synapses(afferent):
                 if not s.UI_recorder.behavior_enabled:
                     s.UI_recorder.behavior_enabled = True
                     print('recorder started')
                 if s.cb.checkState() == 2:
                     if s.UI_recorder.is_new_data_available():
                         x_data = s.UI_recorder['iteration', 0]
                         y_data = s.UI_recorder[self.key, 0]
 
                         if len(x_data) > 0 and len(y_data) > 0:
                             for curve in s.UI_curves:
                                 curve.setData(x_data, y_data[:, curve.index])
         else:
             if self.current_ng is not None:
-                for s in self.current_ng.afferent_synapses["All"]:
+                for s in self.current_ng.synapses(afferent):
                     if s.UI_recorder.behavior_enabled:
                         s.UI_recorder.behavior_enabled=False
                         print('recorder paused')
```

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/info_tabs.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/info_tabs.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/isi_tab.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/isi_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/module_visualizer_tab.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/module_visualizer_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/multi_group_plot_tab.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/multi_group_plot_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/partition_tab.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/partition_tab.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,9 +114,9 @@
             self.plots[transmitter].addItem(self.draw_items[transmitter])
 
 
     def update(self, Network_UI):
         if self.partition_tab.isVisible():
             group=Network_UI.selected_neuron_group()
             for transmitter in Network_UI.transmitters:
-                self.draw_items[transmitter].update_pic(group.afferent_synapses[transmitter],group)
+                self.draw_items[transmitter].update_pic(group.synapses(afferent, transmitter),group)
                 self.plots[transmitter].update()
```

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_fast_forward_module.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_fast_forward_module.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_module_quick_access.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_module_quick_access.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_network_selector.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_network_selector.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_neuron_grid.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_neuron_grid.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_save_load_module.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/sidebar_save_load_module.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/single_group_plot_tab.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/single_group_plot_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/spiketrain_tab.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/spiketrain_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/stability_tab.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/stability_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/weight_tab.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/weight_tab.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,37 +39,37 @@
     def update(self, Network_UI):
         if self.weight_tab.isVisible():
             group = Network_UI.selected_neuron_group()
             selected = Network_UI.selected_neuron_id()
 
             self.main_plot.clear()
 
-            afferent=self.select_aff_eff.currentText() == 'afferent'
+            aff=self.select_aff_eff.currentText() == 'afferent'
             single = self.select_mode.currentText() != 'all'
             max_mode = self.select_max_box.currentText()
             min_mode = self.select_min_box.currentText()
 
             c = 0
             syns = []
             syn_tags=[]
             max_s = []
             min_s = []
 
-            if afferent:
-                for s in group.afferent_synapses['All']:
+            if aff:
+                for s in group.synapses(afferent):
                     w = s.ignore_transpose_mode(s.W)
 
                     if single:
                         data = np.rot90(w[selected].reshape(s.src.height, s.src.width), 3)
                     else:
                         data = w
                     syns.append(data)
                     syn_tags.append(s.tags)
             else:
-                for s in group.efferent_synapses['All']:
+                for s in group.synapses(efferent):#efferent_synapses['All']:
                     w = s.ignore_transpose_mode(s.W)
 
                     if single:
                         data = np.rot90(w[:, selected].reshape(s.dst.height, s.dst.width), 3)
                     else:
                         data = w
                     syns.append(data)
```

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Basic_Tabs/weight_tab_old.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Basic_Tabs/weight_tab_old.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,16 @@
             #collect all synapse information
             syn_dict = {}
 
             for transmitter in Network_UI.transmitters:
                 syn_dict[transmitter] = {}
                 for weight_attr in self.weight_attrs:
 
-                    if transmitter in group.afferent_synapses and len(group.afferent_synapses[transmitter])>0:
-                        syn_dict[transmitter][weight_attr] = {transmitter: get_single_neuron_combined_partition_matrix(group, transmitter, weight_attr, Network_UI.selected_neuron_id())}#group.afferent_synapses[transmitter][0].W[Network_UI.selected_neuron_id()
+                    if transmitter in group.afferent_synapses and len(group.synapses(afferent, transmitter))>0:
+                        syn_dict[transmitter][weight_attr] = {transmitter: get_single_neuron_combined_partition_matrix(group, transmitter, weight_attr, Network_UI.selected_neuron_id())}#group.synapses(afferent, transmitter)[0].W[Network_UI.selected_neuron_id()
 
             #determine ranges
             min_max_mode = self.select_min_max_box.currentText()
 
             glob_max=0
             tr_max={}
             var_max={}
```

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Network_UI.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Network_UI.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
             return syn_sgs[0]
         else:
             return None
 
     def get_selected_synapses(self):
         result = []
         group = self.selected_neuron_group()
-        synapse_groups = group.afferent_synapses['All']
+        synapse_groups = group.synapses(afferent)
         for i, s in enumerate(synapse_groups):
             if (type(s.dst.mask) == np.ndarray and s.dst.mask[self.selected_neuron_id()]) or (type(s.dst.mask) is bool and s.dst.mask == True):
                 result.append(synapse_groups[i].dst)
         return result
 
     def on_timer(self):
```

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Neuron_Classification_Colorizer.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Neuron_Classification_Colorizer.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/__init__.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/__init__.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/chain_tab.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/chain_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/character_activation_tab.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/character_activation_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/reconstruction_tab.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/reconstruction_tab.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_drumbeat_module.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_drumbeat_module.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_grammar_module.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_grammar_module.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_image_module.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_image_module.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_music_module.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_music_module.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sun_gravity_plot_tab.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sun_gravity_plot_tab.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
         #group.buffer_posx += (group.vector('uniform') - 0.5)*0.1
         #group.buffer_posy += (group.vector('uniform') - 0.5)*0.1
 
         group.add_x = (group.vector('uniform') - 0.5) * random_movement_fac# + (-group.buffer_posx)*p2
         group.add_y = (group.vector('uniform') - 0.5) * random_movement_fac# + (-group.buffer_posy)*p2#np.sin(group.buffer_posy/lb*2*np.pi)*10*p2
 
-        for sg in group.afferent_synapses['GLU']:
+        for sg in group.synapses(afferent, 'GLU'):
             theta_src, rho_src = cart2pol(sg.src.buffer_posx, sg.src.buffer_posy)
 
             if hasattr(group, 'timescale'):
                 step_factor = np.power(0.9, group.timescale)
             else:
                 step_factor = 0.9
 
@@ -194,15 +194,15 @@
         #for x, y in zip(group.buffer_posx[mask], group.buffer_posy[mask]):
         #    painter.drawEllipse(QtCore.QPointF(x, y), neuron_size, neuron_size)
 
     def draw_weights(self, painter, group, selected_neuron_id):
         painter.setPen(pg.mkPen(color=(255, 0, 0, 255)))
         painter.setBrush(pg.mkBrush(color=(0, 0, 0, 0)))
 
-        for sg in group.afferent_synapses['GLU']:
+        for sg in group.synapses(afferent, 'GLU'):
             temp = np.where(sg.dst.id == selected_neuron_id)[0]
             if len(temp) > 0:
                 indx = temp[0]
                 x = sg.dst.buffer_posx[indx]
                 y = sg.dst.buffer_posy[indx]
 
                 weights = sg.ignore_transpose_mode(sg.W)[indx, :]
@@ -250,15 +250,15 @@
         self.p3s = p3s
         self.p4s = p4s
         self.p5s = p5s
         self.label_cb = label_cb
 
     #def compute_similarity(self, group, neuron_index):
     #    group._syn_differences_ = group.vector()
-    #    for sg in group.afferent_synapses['GLU']:
+    #    for sg in group.synapses(afferent, 'GLU'):
     #        if neuron_index in sg.dst.id:
     #            sg.dst._syn_differences_ += np.sum(sg.W * sg.W[:,np.where(sg.dst.id==neuron_index)[0]], axis=1)
 
     #    m=np.max(group._syn_differences_)
     #    if m>0:
     #        group._syn_differences_=1.0-(group._syn_differences_/m)
```

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Network_UI/TabBase.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Network_UI/TabBase.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Overview_UI.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Overview_UI.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/StorageManager/StorageManager.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/StorageManager/StorageManager.py`

 * *Files 10% similar despite different names*

```diff
@@ -365,144 +365,14 @@
         self.absolute_path = folder
 
         self.config_file_name = 'config.ini'
         self.config = None
 
         self.frame_counter = {}
 
-class StorageManager2:
-                                            #%nr %rnd
-    def __init__(self, folder, subfolder='folder+"_"+id', mainfolder='StorageManager', datafolder=get_data_folder(), print_path=True):
-
-        if os.path.exists(folder):
-            path = folder
-        else:
-            self.path = self._ensure_folder(datafolder + '/')
-            self.path = self._ensure_folder(self.path + mainfolder + '/')
-            self.path = self._ensure_folder(self.path + folder + '/')
-
-            subfolder = self._eval_subfolder(folder, subfolder)
-            new = not os.path.exists(self.path + subfolder + '/')
-            self.path = self._ensure_folder(self.path + subfolder + '/')
-
-            if new:
-                self.save('time', time.time())
-
-        if print_path:
-            print(self.path)
-
-        self.config = ConfigParser()
-        self.config.read(self.path + 'config.ini')
-
-
-    def _eval_subfolder(self, folder, subfolder):
-        try:
-            if 'id' in subfolder:
-                id = len(os.listdir(self.path))
-
-            if 'rnd' in subfolder:
-                rnd = str(int(np.random.rand() * 10000))
-
-            subfolder = eval(subfolder)
-        except:
-            pass
-
-        return subfolder
-
-    @property
-    def folder(self):
-        return self.path
-
-    @property
-    def directory(self):
-        return self.path
-
-    def _ensure_folder(self, folder):
-        if not os.path.exists(folder):
-            try:
-                os.mkdir(folder)
-            except:
-                raise Exception(folder+' can not be created')
-        return folder
-
-    def _get_next_key_file(self, key):
-        result = self.path+key+ '.*'
-        i = 0
-        while len(glob.glob(result))>0:
-            result = self.path + key + '_' + str(i) + '.*'
-            i += 1
-        return result
-
-
-    # add network save pickle compile...
-    def save(self, key, data, mainkey='', ):
-        if type(data) == str or type(data) == int or type(data) == float or type(data) == bool:
-
-            value = str(data)
-
-            if not self.config.has_section(mainkey):
-                self.config.add_section(mainkey)
-            self.config.set(mainkey, key, str(value).replace('%', 'percent'))
-            with open(self.absolute_path + self.config_file_name, 'w') as configfile:
-                self.config.write(configfile)
-
-        else:
-            file = self._get_next_key_file(mainkey+key)
-
-            if type(data) == np.ndarray:
-                np.save(file + '.npy', arr=obj)
-
-            elif type(data) == image:
-                imageio.imwrite(file + '.png', image.astype(np.uint8))
-
-            else:#obj
-                pickle.dump(obj, open(file + '.obj', 'wb'))
-
-
-    def load(self, key, default=None, mainkey=''):
-        
-
-        try:
-            s = self.config.get(mainkey, key)
-        except:
-            return default
-        if len(s) > 0:
-            if s=='True':
-                return True
-            if s=='False':
-                return False
-            try:
-                if '.' in s:
-                    return float(s)
-                else:
-                    return int(s)
-            except:
-                return s
-        return s
-
-
-
-    #do not use! => render_video searches for key*.png (right order!!!) (creation date?)
-
-    #self.get_next_frame_name(key)
-    #def get_next_frame_key(self, videokey):
-    #    if not key in self.frame_counter:
-    #        self.frame_counter[key] = 0
-    #    self.frame_counter[key] += 1
-    #    return self.absolute_path+key+'{}'.format(self.frame_counter[key]-1)
-
-
-    def render_video(self, key, delete_images, reset_frame_counter=True):
-        call(['ffmpeg', '-i', self.path + key + '_%d.png', '-c:v', 'libx264', '-strict', '-2', '-preset', 'slow', '-pix_fmt', 'yuv420p', '-vf', 'scale=trunc(iw/2)*2:trunc(ih/2)*2', '-f', 'mp4', self.absolute_path + key + '.mp4'], shell=True)
-        if delete_images:
-            files = os.listdir(self.path)
-            for f in files:
-                if key in f and '.png' in f:
-                    os.remove(self.absolute_path + f)
-
 
 
 class StorageManagerGroup:
 
     def __iter__(self):
         return self.StorageManagerList.__iter__()
```

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/StorageManager/Storage_Manager_Dir_Select_Dialog.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/StorageManager/Storage_Manager_Dir_Select_Dialog.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/UI_Base.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/UI_Base.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Visualization/Analysis_Plots.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Visualization/Analysis_Plots.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Visualization/Module_visualizer.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Visualization/Module_visualizer.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Visualization/Pyplot_visualizer.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Visualization/Pyplot_visualizer.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/Plot_Synapse_Transition_scatter.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/Plot_Synapse_Transition_scatter.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/Plot_weights.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/Plot_weights.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/Reconstruct_Analyze_Label.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Visualization/Reconstruct_Analyze_Label/Reconstruct_Analyze_Label.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,18 +307,24 @@
                             # w_mul=w==w.max(axis=1)
                             w_mul = np.equal(w, np.tile(w.max(axis=1), (w.shape[1], 1)).transpose())  # better way!!!
                         if type(synapse_filter) == float:
                             # w_mul = w >= (w.max(axis=1)*synapse_filter)
                             w_mul = np.greater(w, np.tile(w.max(axis=1) * synapse_filter, (w.shape[1], 1)))
 
                         if propagation_mode == 'backward':
-                            syn.src.recon_temp += (w * w_mul).transpose().dot(syn.dst.recon)  # disabled???
+                            if self.network.transposed_synapse_matrix_mode:
+                                syn.dst.recon_temp += (w * w_mul).dot(syn.src.recon)  # disabled???
+                            else:
+                                syn.src.recon_temp += (w * w_mul).transpose().dot(syn.dst.recon)  # disabled???
 
                         if propagation_mode == 'forward':
-                            syn.dst.recon_temp += (w * w_mul).dot(syn.src.recon)  # disabled???
+                            if self.network.transposed_synapse_matrix_mode:
+                                syn.src.recon_temp += (w * w_mul).transpose().dot(syn.dst.recon)  # disabled???
+                            else:
+                                syn.dst.recon_temp += (w * w_mul).dot(syn.src.recon)  # disabled???
 
             if exponent is not None:
                 syn.dst.recon_temp = np.power(syn.dst.recon_temp, exponent)
 
             if filter_weakest_percent is not None:
                 recon_min = np.min(syn.dst.recon_temp)
                 recon_max = np.max(syn.dst.recon_temp)
```

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Visualization/SORN_visualization.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Visualization/SORN_visualization.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Visualization/Visualization_Helper.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Visualization/Visualization_Helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,17 +142,17 @@
 def get_whole_Network_weight_image(neuron_dst_group, plot_inh_synapses=False, neuron_src_groups=None, add_activity=False, individual_norm=False, exc_weight_attr='GLU_Synapses', inh_weight_attr='GABA_Synapses', activations=None):
 
     exc_synapses = []
     inh_synapses = []
 
     shapes = []
 
-    temp_inh_syns = neuron_dst_group.afferent_synapses['GABA']
+    temp_inh_syns = neuron_dst_group.synapses(afferent, 'GABA')
 
-    for syn in neuron_dst_group.afferent_synapses['GLU']:
+    for syn in neuron_dst_group.synapses(afferent, 'GLU'):
         if neuron_src_groups is None or syn.src in neuron_src_groups:
 
             found = None
             for inh_syn in temp_inh_syns:
                 if syn.src == inh_syn.src and syn.dst == inh_syn.dst:
                     found = inh_syn
```

### Comparing `PymoNNto-3.0.0/PymoNNto/Exploration/Visualization/read_write_np_experiment.py` & `PymoNNto-3.0.1/PymoNNto/Exploration/Visualization/read_write_np_experiment.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/NetworkBehavior/Basics/BasicHomeostasis.py` & `PymoNNto-3.0.1/PymoNNto/NetworkBehavior/Basics/BasicHomeostasis.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/NetworkBehavior/Basics/Normalization.py` & `PymoNNto-3.0.1/PymoNNto/NetworkBehavior/Basics/Normalization.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,51 @@
+from PymoNNto.NetworkCore.Neuron_Group import *
 from PymoNNto.NetworkCore.Behavior import *
 import numpy as np
 
 class Synaptic_Normalization(Behavior):
 
     def initialize(self, neurons):
         self.syn_type = self.parameter('syn_type', 'GLU', neurons)
         self.clip_max = self.parameter('clip_max', None, neurons)
         neurons.weight_norm_factor = neurons.vector()+self.parameter('norm_factor', 1.0, neurons)
 
     def iteration(self, neurons):
         normalize_synapse_attr('W', 'W', neurons.weight_norm_factor, neurons, self.syn_type)
-        for s in neurons.afferent_synapses[self.syn_type]:
+        for s in neurons.synapses(afferent, self.syn_type):
             s.W = np.clip(s.W, 0, self.clip_max)
 
 
 
 
 
 
 def normalize_synapse_attr(src_attr, target_attr, target_value, neurons, synapse_type):
     neurons.temp_weight_sum = neurons.vector()
 
-    for s in neurons.afferent_synapses[synapse_type]:
+    for s in neurons.synapses(afferent, synapse_type):
         s.dst.temp_weight_sum += np.sum(np.abs(getattr(s, src_attr)), axis=1)
 
     neurons.temp_weight_sum /= target_value
 
-    for s in neurons.afferent_synapses[synapse_type]:
+    for s in neurons.synapses(afferent, synapse_type):
         setattr(s, target_attr, getattr(s, target_attr) / (s.dst.temp_weight_sum[:, None] + (s.dst.temp_weight_sum[:, None] == 0)))
 
 
 
 
 def normalize_synapse_attr_efferent(src_attr, target_attr, target_value, neurons, synapse_type):
     neurons.temp_weight_sum = neurons.vector()
 
-    for s in neurons.efferent_synapses[synapse_type]:
+    for s in neurons.synapses(efferent, synapse_type):
         s.src.temp_weight_sum += np.sum(np.abs(getattr(s, target_attr)), axis=0)
 
     neurons.temp_weight_sum /= target_value
 
-    for s in neurons.efferent_synapses[synapse_type]:
+    for s in neurons.neurons.synapses(efferent, synapse_type):
         setattr(s, src_attr, getattr(s, src_attr) / (s.src.temp_weight_sum + (s.src.temp_weight_sum == 0)))
 
 '''
 from PymoNNto import *
 
 net = Network(tag='Network')
```

### Comparing `PymoNNto-3.0.0/PymoNNto/NetworkBehavior/Basics/Normalization_Sparse.py` & `PymoNNto-3.0.1/PymoNNto/NetworkBehavior/Basics/Normalization_Sparse.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+from PymoNNto.NetworkCore.Neuron_Group import *
 import numpy as np
 
+
 def normalize_synapse_attr_sparse(src_attr, target_attr, target_value, neurons, synapse_type):
 
     neurons.temp_weight_sum = neurons.vector()
 
-    for s in neurons.afferent_synapses[synapse_type]:
+    for s in neurons.synapses(afferent, synapse_type):
         if 'sparse' in s.tags:
             s.dst.temp_weight_sum += np.array(getattr(s, src_attr).sum(1)).flatten()
         else:
             s.dst.temp_weight_sum += np.sum(getattr(s, src_attr), axis=1)
 
     neurons.temp_weight_sum /= target_value
 
-    for s in neurons.afferent_synapses[synapse_type]:
+    for s in neurons.synapses(afferent, synapse_type):
         if 'sparse' in s.tags:
             W = getattr(s, target_attr)
             W.data /= np.array(neurons.temp_weight_sum[W.indices]).reshape(W.data.shape)
         else:
             setattr(s, target_attr, getattr(s, target_attr) / (s.dst.temp_weight_sum[:, None]+(s.dst.temp_weight_sum[:, None]==0)))
```

### Comparing `PymoNNto-3.0.0/PymoNNto/NetworkBehavior/Basics/Normalization_Tensorflow.py` & `PymoNNto-3.0.1/PymoNNto/NetworkBehavior/Basics/Normalization_Tensorflow.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from PymoNNto.NetworkCore.Neuron_Group import *
 from PymoNNto.NetworkCore.Behavior import *
 import numpy as np
 import tensorflow as tf
 
 class Synaptic_Normalization_TF(Behavior):
 
     def initialize(self, neurons):
@@ -15,16 +16,16 @@
         self.norm_factor = tf.constant(self.parameter('norm_factor', 1.0, neurons), dtype='float32')
 
         neurons.temp_weight_sum = tf.Variable(neurons.vector(), dtype='float32')
 
     def iteration(self, neurons):
         neurons.temp_weight_sum.assign(tf.multiply(neurons.temp_weight_sum, 0.0))
 
-        for s in neurons.afferent_synapses[self.syn_type]:
+        for s in neurons.synapses(afferent, self.syn_type):
             s.dst.temp_weight_sum.assign(tf.add(s.dst.temp_weight_sum, tf.math.reduce_sum(s.W, axis=1)))
 
         neurons.temp_weight_sum.assign(tf.divide(neurons.temp_weight_sum, self.norm_factor))
 
-        for s in neurons.afferent_synapses[self.syn_type]:
+        for s in neurons.synapses(afferent, self.syn_type):
             #d = tf.add(s.dst.temp_weight_sum, tf.cast(tf.math.equal(s.dst.temp_weight_sum, 0.0), dtype='float32'))
             d = s.dst.temp_weight_sum
             s.W.assign(tf.transpose(tf.divide(tf.transpose(s.W), d)))
```

### Comparing `PymoNNto-3.0.0/PymoNNto/NetworkBehavior/EulerEquationModules/Equation.py` & `PymoNNto-3.0.1/PymoNNto/NetworkBehavior/EulerEquationModules/Equation.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/NetworkBehavior/EulerEquationModules/EulerClock.py` & `PymoNNto-3.0.1/PymoNNto/NetworkBehavior/EulerEquationModules/EulerClock.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/NetworkBehavior/EulerEquationModules/Helper.py` & `PymoNNto-3.0.1/PymoNNto/NetworkBehavior/EulerEquationModules/Helper.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/NetworkBehavior/EulerEquationModules/VariableInitializer.py` & `PymoNNto-3.0.1/PymoNNto/NetworkBehavior/EulerEquationModules/VariableInitializer.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/NetworkBehavior/Recorder/Recorder.py` & `PymoNNto-3.0.1/PymoNNto/NetworkBehavior/Recorder/Recorder.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 import copy
 
 class Recorder(Behavior):
     initialize_last = True
 
     visualization_module_outputs = []
 
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.variables = {}
+
+
     def initialize(self, parent_obj):
         self.add_tag('recorder')
 
         variables = self.parameter('variables', None)
         if variables is None:
             variables = self.parameter('arg_0', None)
             if variables is None:
@@ -19,15 +24,14 @@
             variables = [variables]
 
         self.gapwidth = self.parameter('gapwidth', 0)
         self.save_as_numpy = self.parameter('save_as_numpy', False)
         self.max_length = self.parameter('max_length', None)
         self.counter = 0
         self.new_data_available=False
-        self.variables = {}
         self.compiled = {}
 
         self.add_variables(variables)
         self.reset()
 
     def iteration(self, parent_obj):
 
@@ -167,23 +171,19 @@
     def get_data_v(self, variable, parent_obj):
         n = parent_obj  # used for eval string "n.x"
         s = parent_obj
         neurons = parent_obj
         synapse = parent_obj
 
         data = eval(self.compiled[variable])
-        indices = np.where(data != 0)[0]
 
-        if len(indices) > 0:
-            result = []
-            for i in indices:
-                result.append([parent_obj.iteration, i])
-            return result
-        else:
-            return None
+        indices = np.where(data != 0)
+        iteration = np.ones_like(indices[0]) * parent_obj.iteration
+
+        return np.stack((iteration, *indices), axis=1)
 
     def save_data_v(self, data, variable):
         if len(self.variables[variable]) == 0:
             self.variables[variable] = np.array(data)
         else:
             self.variables[variable] = np.concatenate([self.variables[variable], data], axis=0)
```

### Comparing `PymoNNto-3.0.0/PymoNNto/NetworkBehavior/Structure/Partition.py` & `PymoNNto-3.0.1/PymoNNto/NetworkBehavior/Structure/Partition.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/NetworkBehavior/Structure/Receptive_Fields.py` & `PymoNNto-3.0.1/PymoNNto/NetworkBehavior/Structure/Receptive_Fields.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/NetworkBehavior/Structure/Structure.py` & `PymoNNto-3.0.1/PymoNNto/NetworkBehavior/Structure/Structure.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/NetworkCore/Analysis_Module.py` & `PymoNNto-3.0.1/PymoNNto/NetworkCore/Analysis_Module.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/NetworkCore/Base_Attachable_Modules.py` & `PymoNNto-3.0.1/PymoNNto/NetworkCore/Base_Attachable_Modules.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         remove_keys=[]
         for key in self.behavior:
             b = self.behavior[key]
             if key_tag_behavior_or_type == key or key_tag_behavior_or_type in b.tags or key_tag_behavior_or_type == b or key_tag_behavior_or_type == type(b):
                 remove_keys.append(key)
         for key in remove_keys:
             b=self.behavior.pop(key)
-            self.network._remove_behavior_from_sorted_execution_list(self, b)
+            self.network._remove_behavior_from_sorted_execution_list(key, self, b)
 
     def set_behaviors(self, tag, enabeled):
         if enabeled:
             print('activating', tag)
         else:
             print('deactivating', tag)
         for b in self[tag]:
@@ -198,20 +198,20 @@
 
     def get_nparray(self, dim):
         return np.zeros(dim).astype(self.def_dtype)
 
     def get_buffer_mat(self, dim, size):
         return np.array([self.get_nparray(dim) for _ in range(size)])
 
-    def buffer_roll(self, mat, new=None):
+    def buffer_roll(self, mat, new=None, counter=False):
         #return np.roll(mat, 1, axis=0)
-        mat[1:len(mat)] = mat[0:len(mat) - 1]
+        mat[1-counter : len(mat)-counter] = mat[0+counter : len(mat)-1+counter]
 
         if new is not None:
-            mat[0]=new
+            mat[0-counter]=new
 
         return mat
 
     ################################################################################################
     #deprecated#####################################################################################
     ################################################################################################
```

### Comparing `PymoNNto-3.0.0/PymoNNto/NetworkCore/Base_Tagable_Object.py` & `PymoNNto-3.0.1/PymoNNto/NetworkCore/Base_Tagable_Object.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/NetworkCore/Behavior.py` & `PymoNNto-3.0.1/PymoNNto/NetworkCore/Behavior.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/NetworkCore/Network.py` & `PymoNNto-3.0.1/PymoNNto/NetworkCore/Network.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,23 +13,24 @@
 SxD = 0
 DxS = 1
 
 class Network(NetworkObjectBase):
 
     def __init__(self, tag=None, behavior={}, settings={}):
         self.apply_settings(settings)
-        super().__init__(tag, self, behavior)
 
         self.NeuronGroups = []
         self.SynapseGroups = []
 
         self.iteration = 0
 
         self.behavior_timesteps = []
         self.sorted_behavior_execution_list = [] #stores (key, beh_parent, behavior) triplets
+        
+        super().__init__(tag, self, behavior)
 
     # {'dtype':float32, 'syn_dim':DxS}
     def apply_settings(self, settings):
         self.def_dtype = settings.get('dtype', float32)
         self.transposed_synapse_matrix_mode = settings.get('syn_dim', DxS)!=DxS
 
     def all_objects(self):
@@ -46,26 +47,26 @@
         for i,kpb in enumerate(self.sorted_behavior_execution_list):
             k, p, b = kpb
             if key>=k:
                 insert_indx = i+1
         self.sorted_behavior_execution_list.insert(insert_indx, (key, beh_parent, behavior))
         #print([k for k,_,_ in self.sorted_behavior_execution_list])
         
-    def _remove_behavior_from_sorted_execution_list(self, beh_parent, behavior):# removes SINGLE behavior!
+    def _remove_behavior_from_sorted_execution_list(self, key, beh_parent, behavior):
         rm_indx = -1
         for i,kpb in enumerate(self.sorted_behavior_execution_list):
             k, p, b = kpb
-            if beh_parent==p and behavior==b:
+            if key==k and beh_parent==p and behavior==b:
                 rm_indx = i
+                break
         if rm_indx>-1:
             self.sorted_behavior_execution_list.pop(rm_indx)
         else:
             raise Exception('behavior not found')
 
-
     #######################################
     #Behavior Management
     #######################################
 
     def set_behaviors(self, tag, enabeled):
         if enabeled:
             print('activating', tag)
@@ -324,19 +325,19 @@
     def set_synapses_to_neuron_groups(self):# todo: move to synapse group __init__
         for ng in self.NeuronGroups:
             ng.afferent_synapses = {}
             ng.efferent_synapses = {}
 
             for sg in self.SynapseGroups:
                 for tag in sg.tags+['All']:
-                    ng.afferent_synapses[tag] = []
+                    ng.synapses(afferent, tag) = []
                     ng.efferent_synapses[tag] = []
 
             for sg in self.SynapseGroups:
                 if sg.dst.BaseNeuronGroup == ng:
                     for tag in sg.tags+['All']:
-                        ng.afferent_synapses[tag].append(sg)
+                        ng.synapses(afferent, tag).append(sg)
 
                 if sg.src.BaseNeuronGroup == ng:
                     for tag in sg.tags+['All']:
                         ng.efferent_synapses[tag].append(sg)
     '''
```

### Comparing `PymoNNto-3.0.0/PymoNNto/NetworkCore/Neuron_Group.py` & `PymoNNto-3.0.1/PymoNNto/NetworkCore/Neuron_Group.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         self.mask = True#np.array([True for _ in range(size)]).astype(bool)#True#used for subgroup reconstruction
 
         self.id = np.arange(self.size)
 
         if color is not None:
             self.color = color
 
-    def synapses(self, mode, tag):#afferent=0, efferent=1
+    def synapses(self, mode, tag='All'):#afferent=0, efferent=1
         if mode==afferent:
             return self.afferent_synapses[tag]
         if mode==efferent:
             return self.efferent_synapses[tag]
 
     @property
     def def_dtype(self):
@@ -136,15 +136,15 @@
             search_NG(self)
 
         if efferent_NGs:
             for syn in self.efferent_synapses[syn_tag]:
                 search_NG(syn.dst)
 
         if afferent_NGs:
-            for syn in self.afferent_synapses[syn_tag]:
+            for syn in self.synapses(afferent, syn_tag):
                 search_NG(syn.src)
 
         return result
 
     def partition_size(self, block_size=7):
         w = block_size#int((self.src.width/block_size+self.dst.width/block_size)/2)
         h = block_size#int((self.src.height/block_size+self.dst.height/block_size)/2)
```

### Comparing `PymoNNto-3.0.0/PymoNNto/NetworkCore/Synapse_Group.py` & `PymoNNto-3.0.1/PymoNNto/NetworkCore/Synapse_Group.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,19 +104,19 @@
     matrix = matrix
     mat = matrix
     get_synapse_mat = matrix
 
     def get_synapse_group_size_factor(self, synapse_group, synapse_type):
 
         total_weighting = 0
-        for s in synapse_group.dst.afferent_synapses[synapse_type]:
+        for s in synapse_group.dst.synapses(afferent, synapse_type):
             total_weighting += s.group_weighting
 
         total = 0
-        for s in synapse_group.dst.afferent_synapses[synapse_type]:
+        for s in synapse_group.dst.synapses(afferent, synapse_type):
             total += s.src.size*s.src.group_weighting
 
         return total_weighting/total*synapse_group.src.size*synapse_group.group_weighting
 
     def get_distance_mat(self, radius, src_x=None, src_y=None, dst_x=None, dst_y=None):
         if src_x is None: src_x = self.src.x
         if src_y is None: src_y = self.src.y
```

### Comparing `PymoNNto-3.0.0/PymoNNto/__init__.py` & `PymoNNto-3.0.1/PymoNNto/__init__.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/sync_docs.py` & `PymoNNto-3.0.1/PymoNNto/sync_docs.py`

 * *Files identical despite different names*

### Comparing `PymoNNto-3.0.0/PymoNNto/test_pymoNNto.py` & `PymoNNto-3.0.1/PymoNNto/test_pymoNNto.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 
     assert My_Network.iteration == 1000+10+20+30
     assert np.mean(My_Neurons.count) == 1000+20+30
 
     assert My_Synapses.src == My_Neurons
     assert My_Synapses.dst == My_Neurons
 
-    assert My_Neurons.afferent_synapses['GLUTAMATE'] == [My_Synapses]
+    assert My_Neurons.synapses(afferent, 'GLUTAMATE') == [My_Synapses]
 
     assert len(My_Network.all_objects()) == 3
 
     #tagging system
     assert My_Network['my_neurons'] == [My_Neurons]
     assert len(My_Network['count', 0]) == My_Network.iteration-30
```

### Comparing `PymoNNto-3.0.0/PymoNNto.egg-info/PKG-INFO` & `PymoNNto-3.0.1/PymoNNto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PymoNNto
-Version: 3.0.0
+Version: 3.0.1
 Summary: Python Modular Neural Network Toolbox
 Home-page: https://github.com/trieschlab/PymoNNto
 Author: Marius Vieth
 Author-email: mv15go@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PymoNNto-3.0.0/PymoNNto.egg-info/SOURCES.txt` & `PymoNNto-3.0.1/PymoNNto.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,15 @@
 PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/character_activation_tab.py
 PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/reconstruction_tab.py
 PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_drumbeat_module.py
 PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_grammar_module.py
 PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_image_module.py
 PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sidebar_music_module.py
 PymoNNto/Exploration/Network_UI/Sequence_Activation_Tabs/sun_gravity_plot_tab.py
+PymoNNto/Exploration/StorageManager/SM2.py
 PymoNNto/Exploration/StorageManager/StorageManager.py
 PymoNNto/Exploration/StorageManager/Storage_Manager_Dir_Select_Dialog.py
 PymoNNto/Exploration/StorageManager/User_Input_SM_Writer.py
 PymoNNto/Exploration/StorageManager/__init__.py
 PymoNNto/Exploration/Visualization/Analysis_Plots.py
 PymoNNto/Exploration/Visualization/Module_visualizer.py
 PymoNNto/Exploration/Visualization/Pyplot_visualizer.py
```

### Comparing `PymoNNto-3.0.0/setup.py` & `PymoNNto-3.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PymoNNto",
-    version="3.0.0",
+    version="3.0.1",
     author="Marius Vieth",
     author_email="mv15go@gmail.com",
     description="Python Modular Neural Network Toolbox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/trieschlab/PymoNNto",
     packages=setuptools.find_packages(),
```


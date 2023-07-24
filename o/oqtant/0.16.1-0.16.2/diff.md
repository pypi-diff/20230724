# Comparing `tmp/oqtant-0.16.1.tar.gz` & `tmp/oqtant-0.16.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oqtant-0.16.1.tar", max compression
+gzip compressed data, was "oqtant-0.16.2.tar", max compression
```

## Comparing `oqtant-0.16.1.tar` & `oqtant-0.16.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11341 2023-05-02 20:10:18.126527 oqtant-0.16.1/LICENSE
--rw-r--r--   0        0        0     2348 2023-07-11 20:26:55.462428 oqtant-0.16.1/README.md
--rw-r--r--   0        0        0     8565 2023-07-11 20:26:55.462428 oqtant-0.16.1/documentation/INSTALL.md
--rw-r--r--   0        0        0    10906 2023-07-11 20:26:55.462428 oqtant-0.16.1/documentation/job_analysis_docs.md
--rw-r--r--   0        0        0    10378 2023-07-11 20:26:55.462428 oqtant-0.16.1/documentation/oqtant_client_docs.md
--rw-r--r--   0        0        0     4446 2023-07-11 20:26:55.462428 oqtant-0.16.1/documentation/oraqle_api_docs.md
--rw-r--r--   0        0        0    16157 2023-07-12 13:56:47.774863 oqtant-0.16.1/documentation/walkthroughs/walkthrough_1_bec_jobs.ipynb
--rw-r--r--   0        0        0    11171 2023-07-12 13:57:43.766666 oqtant-0.16.1/documentation/walkthroughs/walkthrough_1_bec_jobs.md
--rw-r--r--   0        0        0    16533 2023-07-12 14:00:04.078167 oqtant-0.16.1/documentation/walkthroughs/walkthrough_2_barrier_jobs.ipynb
--rw-r--r--   0        0        0    11526 2023-07-12 14:00:21.198106 oqtant-0.16.1/documentation/walkthroughs/walkthrough_2_barrier_jobs.md
--rw-r--r--   0        0        0    32239 2023-07-11 20:26:55.466428 oqtant-0.16.1/documentation/walkthroughs/walkthrough_3_abstractions.ipynb
--rw-r--r--   0        0        0    22278 2023-07-11 20:26:55.466428 oqtant-0.16.1/documentation/walkthroughs/walkthrough_3_abstractions.md
--rw-r--r--   0        0        0    16722 2023-07-12 14:00:57.121977 oqtant-0.16.1/documentation/walkthroughs/walkthrough_4_experiment.ipynb
--rw-r--r--   0        0        0    11727 2023-07-12 14:01:12.225922 oqtant-0.16.1/documentation/walkthroughs/walkthrough_4_experiment.md
--rw-r--r--   0        0        0    14777 2023-07-12 14:01:44.589805 oqtant-0.16.1/documentation/walkthroughs/walkthrough_5_optimization.ipynb
--rw-r--r--   0        0        0     9606 2023-07-12 14:01:58.045757 oqtant-0.16.1/documentation/walkthroughs/walkthrough_5_optimization.md
--rw-r--r--   0        0        0      512 2023-07-11 20:26:55.466428 oqtant-0.16.1/documentation/walkthroughs/walkthroughs.md
--rw-r--r--   0        0        0        0 2023-05-16 16:24:46.335446 oqtant-0.16.1/oqtant/__init__.py
--rw-r--r--   0        0        0    21875 2023-07-11 20:26:55.466428 oqtant-0.16.1/oqtant/oqtant_client.py
--rw-r--r--   0        0        0        0 2023-05-16 16:24:46.335446 oqtant-0.16.1/oqtant/schemas/__init__.py
--rw-r--r--   0        0        0    17813 2023-05-18 18:23:18.769901 oqtant-0.16.1/oqtant/schemas/job.py
--rw-r--r--   0        0        0      508 2023-07-11 20:26:55.466428 oqtant-0.16.1/oqtant/settings.py
--rw-r--r--   0        0        0        0 2023-05-16 16:24:46.335446 oqtant-0.16.1/oqtant/util/__init__.py
--rw-r--r--   0        0        0     3323 2023-07-11 20:26:55.470428 oqtant-0.16.1/oqtant/util/auth.py
--rw-r--r--   0        0        0     1023 2023-05-16 16:24:46.335446 oqtant-0.16.1/oqtant/util/exceptions.py
--rw-r--r--   0        0        0      474 2023-05-16 16:24:46.335446 oqtant-0.16.1/oqtant/util/server.py
--rw-r--r--   0        0        0     3310 2023-07-12 14:02:05.017732 oqtant-0.16.1/pyproject.toml
--rw-r--r--   0        0        0     3714 1970-01-01 00:00:00.000000 oqtant-0.16.1/setup.py
--rw-r--r--   0        0        0     3744 1970-01-01 00:00:00.000000 oqtant-0.16.1/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-05-02 20:10:18.126527 oqtant-0.16.2/LICENSE
+-rw-r--r--   0        0        0     2348 2023-07-11 20:26:55.462428 oqtant-0.16.2/README.md
+-rw-r--r--   0        0        0     8565 2023-07-11 20:26:55.462428 oqtant-0.16.2/documentation/INSTALL.md
+-rw-r--r--   0        0        0    10906 2023-07-11 20:26:55.462428 oqtant-0.16.2/documentation/job_analysis_docs.md
+-rw-r--r--   0        0        0    10378 2023-07-11 20:26:55.462428 oqtant-0.16.2/documentation/oqtant_client_docs.md
+-rw-r--r--   0        0        0     4446 2023-07-11 20:26:55.462428 oqtant-0.16.2/documentation/oraqle_api_docs.md
+-rw-r--r--   0        0        0    16244 2023-07-24 15:06:22.189717 oqtant-0.16.2/documentation/walkthroughs/walkthrough_1_bec_jobs.ipynb
+-rw-r--r--   0        0        0    11191 2023-07-24 15:05:40.997818 oqtant-0.16.2/documentation/walkthroughs/walkthrough_1_bec_jobs.md
+-rw-r--r--   0        0        0    18411 2023-07-24 15:01:28.074406 oqtant-0.16.2/documentation/walkthroughs/walkthrough_2_barrier_jobs.ipynb
+-rw-r--r--   0        0        0    12887 2023-07-24 14:59:10.850785 oqtant-0.16.2/documentation/walkthroughs/walkthrough_2_barrier_jobs.md
+-rw-r--r--   0        0        0    32166 2023-07-24 15:02:03.174329 oqtant-0.16.2/documentation/walkthroughs/walkthrough_3_abstractions.ipynb
+-rw-r--r--   0        0        0    22160 2023-07-24 14:59:42.350693 oqtant-0.16.2/documentation/walkthroughs/walkthrough_3_abstractions.md
+-rw-r--r--   0        0        0    16766 2023-07-24 15:02:03.178329 oqtant-0.16.2/documentation/walkthroughs/walkthrough_4_experiment.ipynb
+-rw-r--r--   0        0        0    11681 2023-07-24 15:00:08.074618 oqtant-0.16.2/documentation/walkthroughs/walkthrough_4_experiment.md
+-rw-r--r--   0        0        0    15164 2023-07-24 15:01:28.078407 oqtant-0.16.2/documentation/walkthroughs/walkthrough_5_optimization.ipynb
+-rw-r--r--   0        0        0     9769 2023-07-24 15:00:33.534543 oqtant-0.16.2/documentation/walkthroughs/walkthrough_5_optimization.md
+-rw-r--r--   0        0        0      512 2023-07-11 20:26:55.466428 oqtant-0.16.2/documentation/walkthroughs/walkthroughs.md
+-rw-r--r--   0        0        0      575 2023-07-24 13:38:42.017046 oqtant-0.16.2/oqtant/__init__.py
+-rw-r--r--   0        0        0    22451 2023-07-24 13:38:42.017046 oqtant-0.16.2/oqtant/oqtant_client.py
+-rw-r--r--   0        0        0      575 2023-07-24 13:38:42.017046 oqtant-0.16.2/oqtant/schemas/__init__.py
+-rw-r--r--   0        0        0    18389 2023-07-24 13:38:42.017046 oqtant-0.16.2/oqtant/schemas/job.py
+-rw-r--r--   0        0        0     1084 2023-07-24 13:38:42.017046 oqtant-0.16.2/oqtant/settings.py
+-rw-r--r--   0        0        0      575 2023-07-24 13:38:42.021046 oqtant-0.16.2/oqtant/util/__init__.py
+-rw-r--r--   0        0        0     3899 2023-07-24 13:38:42.021046 oqtant-0.16.2/oqtant/util/auth.py
+-rw-r--r--   0        0        0     1600 2023-07-24 13:38:42.021046 oqtant-0.16.2/oqtant/util/exceptions.py
+-rw-r--r--   0        0        0     1050 2023-07-24 13:38:42.021046 oqtant-0.16.2/oqtant/util/server.py
+-rw-r--r--   0        0        0     3324 2023-07-24 14:17:59.482343 oqtant-0.16.2/pyproject.toml
+-rw-r--r--   0        0        0     3714 1970-01-01 00:00:00.000000 oqtant-0.16.2/setup.py
+-rw-r--r--   0        0        0     3744 1970-01-01 00:00:00.000000 oqtant-0.16.2/PKG-INFO
```

### Comparing `oqtant-0.16.1/LICENSE` & `oqtant-0.16.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oqtant-0.16.1/README.md` & `oqtant-0.16.2/README.md`

 * *Files identical despite different names*

### Comparing `oqtant-0.16.1/documentation/INSTALL.md` & `oqtant-0.16.2/documentation/INSTALL.md`

 * *Files identical despite different names*

### Comparing `oqtant-0.16.1/documentation/job_analysis_docs.md` & `oqtant-0.16.2/documentation/job_analysis_docs.md`

 * *Files identical despite different names*

### Comparing `oqtant-0.16.1/documentation/oqtant_client_docs.md` & `oqtant-0.16.2/documentation/oqtant_client_docs.md`

 * *Files identical despite different names*

### Comparing `oqtant-0.16.1/documentation/oraqle_api_docs.md` & `oqtant-0.16.2/documentation/oraqle_api_docs.md`

 * *Files identical despite different names*

### Comparing `oqtant-0.16.1/documentation/walkthroughs/walkthrough_1_bec_jobs.ipynb` & `oqtant-0.16.2/documentation/walkthroughs/walkthrough_1_bec_jobs.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9983262285649026%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(11, '    round_sig,\\n')], delete: [11]}}, 8: {'source': "*

 * *            "{insert: [(2, 'ultracold_matter_job.inputs[\\n'), (3, '    0\\n'), (4, '].notes = "*

 * *            '"This is an Ultracold Matter job created from Oqtant walkthrough #1"\')], delete: '*

 * *            "[2]}}, 10: {'source': ['[ultracold_matter_job_uuid] = oqtant_client.run_jobs(\\n', "*

 * *            "'    job_list=[ultracold_matter_job], track_status=True\\n', ')']}, 12: {'source': "*

 * *            '{insert: [( […]*

```diff
@@ -39,15 +39,15 @@
                 "from oqtant.oqtant_client import get_oqtant_client\n",
                 "from oqtant.util.auth import get_user_token\n",
                 "from oqtant.schemas.job import (\n",
                 "    OqtantJob,\n",
                 "    Gaussian_dist_2D,\n",
                 "    TF_dist_2D,\n",
                 "    bimodal_dist_2D,\n",
-                "    round_sig\n",
+                "    round_sig,\n",
                 ")\n",
                 "\n",
                 "token = get_user_token(auth_server_port=8080)"
             ]
         },
         {
             "cell_type": "markdown",
@@ -127,15 +127,17 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# In this example we are only working with a single input\n",
                 "# so we will add the note to the first and only input in the array\n",
-                "ultracold_matter_job.inputs[0].notes = \"This is an Ultracold Matter job created from Oqtant walkthrough #1\""
+                "ultracold_matter_job.inputs[\n",
+                "    0\n",
+                "].notes = \"This is an Ultracold Matter job created from Oqtant walkthrough #1\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Submit the OqtantJob to run on the Oraqle hardware ##\n",
@@ -157,15 +159,17 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "[ultracold_matter_job_uuid] = oqtant_client.run_jobs(job_list=[ultracold_matter_job], track_status=True)"
+                "[ultracold_matter_job_uuid] = oqtant_client.run_jobs(\n",
+                "    job_list=[ultracold_matter_job], track_status=True\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Best practices for referencing ##\n",
@@ -177,15 +181,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "with open('walkthrough_1_ultracold_matter.txt', 'w') as f:\n",
+                "with open(\"walkthrough_1_ultracold_matter.txt\", \"w\") as f:\n",
                 "    f.write(ultracold_matter_job_uuid)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -302,24 +306,23 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "ultracold_matter_job.atoms_2dplot(figsize=(6,6))\n",
+                "ultracold_matter_job.atoms_2dplot(figsize=(6, 6))\n",
                 "\n",
                 "ultracold_matter_job.atoms_sliceplot()\n",
                 "\n",
                 "TOF_data = ultracold_matter_job.get_TOF()\n",
                 "\n",
-                "plt.figure(figsize=(6,6))\n",
+                "plt.figure(figsize=(6, 6))\n",
                 "plt.title(\"This is a customized plot of the same results\")\n",
-                "TOF_plot = plt.imshow(TOF_data,origin=\"lower\",\n",
-                "            cmap=\"nipy_spectral\")\n",
+                "TOF_plot = plt.imshow(TOF_data, origin=\"lower\", cmap=\"nipy_spectral\")\n",
                 "plt.grid(visible=True)\n",
                 "plt.colorbar(TOF_plot, shrink=0.8)\n",
                 "\n",
                 "plt.show()"
             ]
         },
         {
@@ -334,18 +337,18 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "output = ultracold_matter_job.inputs[0].output.values\n",
-                "print(\"temperature (nK):\"+ str(output.temperature_uk))\n",
-                "print(\"total atoms :\"+ str(output.tof_atom_number))\n",
-                "print(\"condensed atoms :\"+ str(output.condensed_atom_number))\n",
-                "print(\"thermal atoms :\"+ str(output.thermal_atom_number))"
+                "print(\"temperature (nK):\" + str(output.temperature_uk))\n",
+                "print(\"total atoms :\" + str(output.tof_atom_number))\n",
+                "print(\"condensed atoms :\" + str(output.condensed_atom_number))\n",
+                "print(\"thermal atoms :\" + str(output.thermal_atom_number))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Creating OqtantJobs based off previous ones ##\n",
@@ -361,15 +364,17 @@
             "source": [
                 "# identify the job you wish to copy, this can be any job id you want to use.\n",
                 "# the status of the job does not matter\n",
                 "already_submitted_job_id = ultracold_matter_job.external_id\n",
                 "\n",
                 "# for jobs with multiple input runs add `run=<int>` where <int> equals the input you wish to view.\n",
                 "# without a targeted input run oqtant will default to the first run\n",
-                "new_ultracold_matter_job_stub = oqtant_client.get_job_inputs_without_output(already_submitted_job_id, include_notes=False)\n",
+                "new_ultracold_matter_job_stub = oqtant_client.get_job_inputs_without_output(\n",
+                "    already_submitted_job_id, include_notes=False\n",
+                ")\n",
                 "\n",
                 "# at this point 'new_job_stub' is a python dict with the following keys\n",
                 "print(\"new ultracold matter job stub keys:\")\n",
                 "print(new_ultracold_matter_job_stub.keys())\n",
                 "print(\"\\n\")\n",
                 "\n",
                 "# if you wish to include any job notes associated with the existing job input you can run the\n",
@@ -377,15 +382,17 @@
                 "# new_job_stub = oqtant_client.get_job_inputs_without_output(already_submitted_job_id, include_notes=True)\n",
                 "\n",
                 "# from here you can update any of the inputs and the name of the job to your liking\n",
                 "new_ultracold_matter_job_stub[\"name\"] = \"this is a stub of another job\"\n",
                 "\n",
                 "# at this point 'new_job_stub' can be provided to the 'generate_oqtant_job' function and then submitted with\n",
                 "# the 'run_jobs' function as demonstrated in previous steps\n",
-                "new_ultracold_matter_job = oqtant_client.generate_oqtant_job(job=new_ultracold_matter_job_stub)\n",
+                "new_ultracold_matter_job = oqtant_client.generate_oqtant_job(\n",
+                "    job=new_ultracold_matter_job_stub\n",
+                ")\n",
                 "print(\"new ultracold matter job object:\")\n",
                 "print(new_ultracold_matter_job)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `oqtant-0.16.1/documentation/walkthroughs/walkthrough_1_bec_jobs.md` & `oqtant-0.16.2/documentation/walkthroughs/walkthrough_1_bec_jobs.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from oqtant.oqtant_client import get_oqtant_client
 from oqtant.util.auth import get_user_token
 from oqtant.schemas.job import (
     OqtantJob,
     Gaussian_dist_2D,
     TF_dist_2D,
     bimodal_dist_2D,
-    round_sig
+    round_sig,
 )
 
 token = get_user_token(auth_server_port=8080)
 ```
 
 ## Creating a OqtantClient Instance
 
@@ -83,15 +83,17 @@
 ## Add notes to your OqtantJob input (Optional)
 
 Every OqtantJob input can hold notes up to 500 characters long. These notes can be used to add context and additional information to each input. Notes remain tied to their inputs and can be referenced later. To add a note to a job input simply provide a string value to your desired input object like below:
 
 ```python
 # In this example we are only working with a single input
 # so we will add the note to the first and only input in the array
-ultracold_matter_job.inputs[0].notes = "This is an Ultracold Matter job created from Oqtant walkthrough #1"
+ultracold_matter_job.inputs[
+    0
+].notes = "This is an Ultracold Matter job created from Oqtant walkthrough #1"
 ```
 
 ## Submit the OqtantJob to run on the Oraqle hardware
 
 `OqtantClient.run_jobs()` takes a list of OqtantJob objects, `job_list=[*OqtantJob]` and submits them to the online queue. For each OqtantJob added to the queue a unique UUID is generated and associated to it.
 
 The output of `OqtantClient.run_jobs()` is a list of the unique UUIDs generated during submission.
@@ -103,25 +105,27 @@
 - `track_status=True`
 - `filename="name_of_file"`
 - `write=True`
 
 When writing to a file be sure to <span style="color:red">not overwrite it</span>
 
 ```python
-[ultracold_matter_job_uuid] = oqtant_client.run_jobs(job_list=[ultracold_matter_job], track_status=True)
+[ultracold_matter_job_uuid] = oqtant_client.run_jobs(
+    job_list=[ultracold_matter_job], track_status=True
+)
 ```
 
 ## Best practices for referencing
 
 To easily reference OqtantJobs from the current or previous sessions it is useful to write their ids to a file named after the job. This file can be used later to access the OqtantJob.
 
 In this case we are saving this OqtantJob's id under a file named after this walkthrough.
 
 ```python
-with open('walkthrough_1_ultracold_matter.txt', 'w') as f:
+with open("walkthrough_1_ultracold_matter.txt", "w") as f:
     f.write(ultracold_matter_job_uuid)
 ```
 
 ## Check the status of this session's active OqtantJobs
 
 The OqtantClient object contains a dictionary (indexed by job_id) of all the active OqtantJobs from the current session. To keep inputs and results organized, all jobs are handled as objects of the OqtantJob class.
 
@@ -187,54 +191,55 @@
 ## Viewing TOF images and slice plots
 
 The OqtantJob class automatically fits a bimodal distribution to TOF images. The parameters of the fit model are used to calculate statistics about your atom cloud: temperature, number of atoms per phase, and total number of atoms.
 
 To view the TOF results in 2D or 1D, use built in functions to plot or access the results directly and plot them yourself.
 
 ```python
-ultracold_matter_job.atoms_2dplot(figsize=(6,6))
+ultracold_matter_job.atoms_2dplot(figsize=(6, 6))
 
 ultracold_matter_job.atoms_sliceplot()
 
 TOF_data = ultracold_matter_job.get_TOF()
 
-plt.figure(figsize=(6,6))
+plt.figure(figsize=(6, 6))
 plt.title("This is a customized plot of the same results")
-TOF_plot = plt.imshow(TOF_data,origin="lower",
-            cmap="nipy_spectral")
+TOF_plot = plt.imshow(TOF_data, origin="lower", cmap="nipy_spectral")
 plt.grid(visible=True)
 plt.colorbar(TOF_plot, shrink=0.8)
 
 plt.show()
 ```
 
 ## Viewing atom cloud statistics
 
 The Oraqle service performs an automated fit to generate atom cloud statistics. To access the calculated atom number, cloud temperature etc:
 
 ```python
 output = ultracold_matter_job.inputs[0].output.values
-print("temperature (nK):"+ str(output.temperature_uk))
-print("total atoms :"+ str(output.tof_atom_number))
-print("condensed atoms :"+ str(output.condensed_atom_number))
-print("thermal atoms :"+ str(output.thermal_atom_number))
+print("temperature (nK):" + str(output.temperature_uk))
+print("total atoms :" + str(output.tof_atom_number))
+print("condensed atoms :" + str(output.condensed_atom_number))
+print("thermal atoms :" + str(output.thermal_atom_number))
 ```
 
 ## Creating OqtantJobs based off previous ones
 
 There may be times where you would like to create a new OqtantJob based off of a previous one. In these cases the OqtantClient class provides a method that retrieves an entire OqtantJob's input structure to allow for editing and submission. The steps to do this can be found below.
 
 ```python
 # identify the job you wish to copy, this can be any job id you want to use.
 # the status of the job does not matter
 already_submitted_job_id = ultracold_matter_job.external_id
 
 # for jobs with multiple input runs add `run=<int>` where <int> equals the input you wish to view.
 # without a targeted input run oqtant will default to the first run
-new_ultracold_matter_job_stub = oqtant_client.get_job_inputs_without_output(already_submitted_job_id, include_notes=False)
+new_ultracold_matter_job_stub = oqtant_client.get_job_inputs_without_output(
+    already_submitted_job_id, include_notes=False
+)
 
 # at this point 'new_job_stub' is a python dict with the following keys
 print("new ultracold matter job stub keys:")
 print(new_ultracold_matter_job_stub.keys())
 print("\n")
 
 # if you wish to include any job notes associated with the existing job input you can run the
@@ -242,15 +247,17 @@
 # new_job_stub = oqtant_client.get_job_inputs_without_output(already_submitted_job_id, include_notes=True)
 
 # from here you can update any of the inputs and the name of the job to your liking
 new_ultracold_matter_job_stub["name"] = "this is a stub of another job"
 
 # at this point 'new_job_stub' can be provided to the 'generate_oqtant_job' function and then submitted with
 # the 'run_jobs' function as demonstrated in previous steps
-new_ultracold_matter_job = oqtant_client.generate_oqtant_job(job=new_ultracold_matter_job_stub)
+new_ultracold_matter_job = oqtant_client.generate_oqtant_job(
+    job=new_ultracold_matter_job_stub
+)
 print("new ultracold matter job object:")
 print(new_ultracold_matter_job)
 ```
 
 ## View your current job limits
 
 Your account provides you with a limited number of jobs which you can run in a given period of time. You can check your limits and current status against those limits via the `OqtantClient.get_limits()` method:
```

### Comparing `oqtant-0.16.1/documentation/walkthroughs/walkthrough_2_barrier_jobs.ipynb` & `oqtant-0.16.2/documentation/walkthroughs/walkthrough_2_barrier_jobs.ipynb`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9983375414124126%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(11, '    round_sig,\\n')], delete: [11]}}, 6: {'source': "*

 * *            '{insert: [(17, \'                        "heights_khz": [\\n\'), (18, '*

 * *            "'                            0.0,\\n'), (19, '                            5.0,\\n'), "*

 * *            "(20, '                            10.0,\\n'), (21, '                            "*

 * *            "15.0,\\n'), (22, '                            20.0,\\n'), (23, "*

 * *            "'                            25.0,\\n'), (2 […]*

```diff
@@ -39,15 +39,15 @@
                 "from oqtant.oqtant_client import get_oqtant_client\n",
                 "from oqtant.util.auth import get_user_token\n",
                 "from oqtant.schemas.job import (\n",
                 "    OqtantJob,\n",
                 "    Gaussian_dist_2D,\n",
                 "    TF_dist_2D,\n",
                 "    bimodal_dist_2D,\n",
-                "    round_sig\n",
+                "    round_sig,\n",
                 ")\n",
                 "\n",
                 "token = get_user_token(auth_server_port=8080)"
             ]
         },
         {
             "cell_type": "markdown",
@@ -101,24 +101,72 @@
                 "                    \"powers_mw\": [500.0, 500.0, 475.0, 360.0, 220.0],\n",
                 "                    \"frequencies_mhz\": [17.0, 8.0, 4.0, 1.2, 0.1],\n",
                 "                    \"interpolation\": \"LINEAR\",\n",
                 "                    \"times_ms\": [-1600, -1200, -800, -400, 0],\n",
                 "                },\n",
                 "                \"optical_barriers\": [\n",
                 "                    {\n",
-                "                        \"heights_khz\": [0.0, 5.0, 10.0, 15.0, 20.0, 25.0, 25.0, 25.0, 25.0, 25.0, 25.0],\n",
-                "                        \"positions_um\": [-10.0, -10.0, -10.0, -10.0, -10.0, -10.0, -10.0, -10.0, -10.0, -10.0, -10.0],\n",
+                "                        \"heights_khz\": [\n",
+                "                            0.0,\n",
+                "                            5.0,\n",
+                "                            10.0,\n",
+                "                            15.0,\n",
+                "                            20.0,\n",
+                "                            25.0,\n",
+                "                            25.0,\n",
+                "                            25.0,\n",
+                "                            25.0,\n",
+                "                            25.0,\n",
+                "                            25.0,\n",
+                "                        ],\n",
+                "                        \"positions_um\": [\n",
+                "                            -10.0,\n",
+                "                            -10.0,\n",
+                "                            -10.0,\n",
+                "                            -10.0,\n",
+                "                            -10.0,\n",
+                "                            -10.0,\n",
+                "                            -10.0,\n",
+                "                            -10.0,\n",
+                "                            -10.0,\n",
+                "                            -10.0,\n",
+                "                            -10.0,\n",
+                "                        ],\n",
                 "                        \"interpolation\": \"OFF\",\n",
                 "                        \"widths_um\": [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],\n",
                 "                        \"times_ms\": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10],\n",
                 "                        \"shape\": \"GAUSSIAN\",\n",
                 "                    },\n",
                 "                    {\n",
-                "                        \"heights_khz\": [0.0, 5.0, 10.0, 15.0, 20.0, 25.0, 30.0, 35.0, 40.0, 40.0, 40.0],\n",
-                "                        \"positions_um\": [10.0, 10.0, 10.0, 10.0, 10.0, 10.0, 10.0, 10.0, 10.0, 10.0, 10.0],\n",
+                "                        \"heights_khz\": [\n",
+                "                            0.0,\n",
+                "                            5.0,\n",
+                "                            10.0,\n",
+                "                            15.0,\n",
+                "                            20.0,\n",
+                "                            25.0,\n",
+                "                            30.0,\n",
+                "                            35.0,\n",
+                "                            40.0,\n",
+                "                            40.0,\n",
+                "                            40.0,\n",
+                "                        ],\n",
+                "                        \"positions_um\": [\n",
+                "                            10.0,\n",
+                "                            10.0,\n",
+                "                            10.0,\n",
+                "                            10.0,\n",
+                "                            10.0,\n",
+                "                            10.0,\n",
+                "                            10.0,\n",
+                "                            10.0,\n",
+                "                            10.0,\n",
+                "                            10.0,\n",
+                "                            10.0,\n",
+                "                        ],\n",
                 "                        \"interpolation\": \"OFF\",\n",
                 "                        \"widths_um\": [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],\n",
                 "                        \"times_ms\": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10],\n",
                 "                        \"shape\": \"GAUSSIAN\",\n",
                 "                    },\n",
                 "                ],\n",
                 "                \"optical_landscape\": None,\n",
@@ -144,15 +192,17 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# In this example we are only working with a single input\n",
                 "# so we will add the note to the first and only input in the array\n",
-                "barrier_manipulator_job.inputs[0].notes = \"This is an Ultracold Matter job created from Oqtant walkthrough #1\""
+                "barrier_manipulator_job.inputs[\n",
+                "    0\n",
+                "].notes = \"This is an Ultracold Matter job created from Oqtant walkthrough #1\""
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Submit the OqtantJob to run on the Oraqle hardware ##\n",
@@ -174,15 +224,17 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "[barrier_manipulator_job_uuid] = oqtant_client.run_jobs(job_list=[barrier_manipulator_job], track_status=True)"
+                "[barrier_manipulator_job_uuid] = oqtant_client.run_jobs(\n",
+                "    job_list=[barrier_manipulator_job], track_status=True\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Best practices for referencing ##\n",
@@ -194,15 +246,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "with open('walkthrough_2_barrier_manipulator.txt', 'w') as f:\n",
+                "with open(\"walkthrough_2_barrier_manipulator.txt\", \"w\") as f:\n",
                 "    f.write(barrier_manipulator_job_uuid)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -319,18 +371,19 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "IT_OD = barrier_manipulator_job.get_IT()\n",
                 "pix_cal = barrier_manipulator_job.pix_cal\n",
                 "\n",
-                "plt.figure(figsize=(12,4))\n",
+                "plt.figure(figsize=(12, 4))\n",
                 "plt.title(\"In-Trap Optical Depth\")\n",
-                "IT_plot = plt.imshow(IT_OD,origin=\"lower\",\n",
-                "            cmap=\"nipy_spectral\", extent=[-256, 256, -74, 74])\n",
+                "IT_plot = plt.imshow(\n",
+                "    IT_OD, origin=\"lower\", cmap=\"nipy_spectral\", extent=[-256, 256, -74, 74]\n",
+                ")\n",
                 "plt.xlabel(\"X position (um)\")\n",
                 "plt.ylabel(\"Y position (um)\")\n",
                 "plt.grid(visible=True)\n",
                 "plt.colorbar(IT_plot)\n",
                 "\n",
                 "plt.show()"
             ]
@@ -352,15 +405,17 @@
             "source": [
                 "# identify the job you wish to copy, this can be any job id you want to use.\n",
                 "# the status of the job does not matter\n",
                 "already_submitted_job_id = barrier_manipulator_job.external_id\n",
                 "\n",
                 "# for jobs with multiple input runs add `run=<int>` where <int> equals the input you wish to view.\n",
                 "# without a targeted input run oqtant will default to the first run\n",
-                "new_barrier_manipulator_job_stub = oqtant_client.get_job_inputs_without_output(already_submitted_job_id, include_notes=False)\n",
+                "new_barrier_manipulator_job_stub = oqtant_client.get_job_inputs_without_output(\n",
+                "    already_submitted_job_id, include_notes=False\n",
+                ")\n",
                 "\n",
                 "# at this point 'new_job_stub' is a python dict with the following keys\n",
                 "print(\"new barrier manipulator job stub keys:\")\n",
                 "print(new_barrier_manipulator_job_stub.keys())\n",
                 "print(\"\\n\")\n",
                 "\n",
                 "# if you wish to include any job notes associated with the existing job input you can run the\n",
@@ -368,15 +423,17 @@
                 "# new_job_stub = oqtant_client.get_job_inputs_without_output(already_submitted_job_id, include_notes=True)\n",
                 "\n",
                 "# from here you can update any of the inputs and the name of the job to your liking\n",
                 "new_barrier_manipulator_job_stub[\"name\"] = \"this is a stub of another job\"\n",
                 "\n",
                 "# at this point 'new_job_stub' can be provided to the 'generate_octant_job' function and then submitted with\n",
                 "# the 'run_jobs' function as demonstrated in previous steps\n",
-                "new_barrier_manipulator_job = oqtant_client.generate_oqtant_job(job=new_barrier_manipulator_job_stub)\n",
+                "new_barrier_manipulator_job = oqtant_client.generate_oqtant_job(\n",
+                "    job=new_barrier_manipulator_job_stub\n",
+                ")\n",
                 "print(\"new barrier manipulator job object:\")\n",
                 "print(new_barrier_manipulator_job)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
```

### Comparing `oqtant-0.16.1/documentation/walkthroughs/walkthrough_2_barrier_jobs.md` & `oqtant-0.16.2/documentation/walkthroughs/walkthrough_2_barrier_jobs.md`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from oqtant.oqtant_client import get_oqtant_client
 from oqtant.util.auth import get_user_token
 from oqtant.schemas.job import (
     OqtantJob,
     Gaussian_dist_2D,
     TF_dist_2D,
     bimodal_dist_2D,
-    round_sig
+    round_sig,
 )
 
 token = get_user_token(auth_server_port=8080)
 ```
 
 ## Creating a OqtantClient Instance
 
@@ -66,24 +66,72 @@
                     "powers_mw": [500.0, 500.0, 475.0, 360.0, 220.0],
                     "frequencies_mhz": [17.0, 8.0, 4.0, 1.2, 0.1],
                     "interpolation": "LINEAR",
                     "times_ms": [-1600, -1200, -800, -400, 0],
                 },
                 "optical_barriers": [
                     {
-                        "heights_khz": [0.0, 5.0, 10.0, 15.0, 20.0, 25.0, 25.0, 25.0, 25.0, 25.0, 25.0],
-                        "positions_um": [-10.0, -10.0, -10.0, -10.0, -10.0, -10.0, -10.0, -10.0, -10.0, -10.0, -10.0],
+                        "heights_khz": [
+                            0.0,
+                            5.0,
+                            10.0,
+                            15.0,
+                            20.0,
+                            25.0,
+                            25.0,
+                            25.0,
+                            25.0,
+                            25.0,
+                            25.0,
+                        ],
+                        "positions_um": [
+                            -10.0,
+                            -10.0,
+                            -10.0,
+                            -10.0,
+                            -10.0,
+                            -10.0,
+                            -10.0,
+                            -10.0,
+                            -10.0,
+                            -10.0,
+                            -10.0,
+                        ],
                         "interpolation": "OFF",
                         "widths_um": [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
                         "times_ms": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
                         "shape": "GAUSSIAN",
                     },
                     {
-                        "heights_khz": [0.0, 5.0, 10.0, 15.0, 20.0, 25.0, 30.0, 35.0, 40.0, 40.0, 40.0],
-                        "positions_um": [10.0, 10.0, 10.0, 10.0, 10.0, 10.0, 10.0, 10.0, 10.0, 10.0, 10.0],
+                        "heights_khz": [
+                            0.0,
+                            5.0,
+                            10.0,
+                            15.0,
+                            20.0,
+                            25.0,
+                            30.0,
+                            35.0,
+                            40.0,
+                            40.0,
+                            40.0,
+                        ],
+                        "positions_um": [
+                            10.0,
+                            10.0,
+                            10.0,
+                            10.0,
+                            10.0,
+                            10.0,
+                            10.0,
+                            10.0,
+                            10.0,
+                            10.0,
+                            10.0,
+                        ],
                         "interpolation": "OFF",
                         "widths_um": [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
                         "times_ms": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
                         "shape": "GAUSSIAN",
                     },
                 ],
                 "optical_landscape": None,
@@ -100,15 +148,17 @@
 ## Add notes to your OqtantJob input (Optional)
 
 Every OqtantJob input can hold notes up to 500 characters long. These notes can be used to add context and additional information to each input. Notes remain tied to their inputs and can be referenced later. To add a note to a job input simply provide a string value to your desired input object like below:
 
 ```python
 # In this example we are only working with a single input
 # so we will add the note to the first and only input in the array
-barrier_manipulator_job.inputs[0].notes = "This is an Ultracold Matter job created from Oqtant walkthrough #1"
+barrier_manipulator_job.inputs[
+    0
+].notes = "This is an Ultracold Matter job created from Oqtant walkthrough #1"
 ```
 
 ## Submit the OqtantJob to run on the Oraqle hardware
 
 `OqtantClient.run_jobs()` takes a list of OqtantJob objects, `job_list=[*OqtantJob]` and submits them to the online queue. For each OqtantJob added to the queue a unique UUID is generated and associated to it.
 
 The output of `OqtantClient.run_jobs()` is a list of the unique UUIDs generated during submission.
@@ -120,25 +170,27 @@
 - `track_status=True`
 - `filename="name_of_file"`
 - `write=True`
 
 When writing to a file be sure to <span style="color:red">not overwrite it</span>
 
 ```python
-[barrier_manipulator_job_uuid] = oqtant_client.run_jobs(job_list=[barrier_manipulator_job], track_status=True)
+[barrier_manipulator_job_uuid] = oqtant_client.run_jobs(
+    job_list=[barrier_manipulator_job], track_status=True
+)
 ```
 
 ## Best practices for referencing
 
 To easily reference OqtantJobs from the current or previous sessions it is useful to write their ids to a file named after the job. This file can be used later to access the OqtantJob.
 
 In this case we are saving this OqtantJob's id under a file named after this walkthrough.
 
 ```python
-with open('walkthrough_2_barrier_manipulator.txt', 'w') as f:
+with open("walkthrough_2_barrier_manipulator.txt", "w") as f:
     f.write(barrier_manipulator_job_uuid)
 ```
 
 ## Check the status of this session's active OqtantJobs
 
 The OqtantClient object contains a dictionary (indexed by job_id) of all the active OqtantJobs from the current session. To keep inputs and results organized, all jobs are handled as objects of the OqtantJob class.
 
@@ -204,18 +256,19 @@
 
 To view the TOF results in 2D or 1D, use the built in functions of the OqtantJob class to plot or access the results directly and plot them yourself.
 
 ```python
 IT_OD = barrier_manipulator_job.get_IT()
 pix_cal = barrier_manipulator_job.pix_cal
 
-plt.figure(figsize=(12,4))
+plt.figure(figsize=(12, 4))
 plt.title("In-Trap Optical Depth")
-IT_plot = plt.imshow(IT_OD,origin="lower",
-            cmap="nipy_spectral", extent=[-256, 256, -74, 74])
+IT_plot = plt.imshow(
+    IT_OD, origin="lower", cmap="nipy_spectral", extent=[-256, 256, -74, 74]
+)
 plt.xlabel("X position (um)")
 plt.ylabel("Y position (um)")
 plt.grid(visible=True)
 plt.colorbar(IT_plot)
 
 plt.show()
 ```
@@ -227,15 +280,17 @@
 ```python
 # identify the job you wish to copy, this can be any job id you want to use.
 # the status of the job does not matter
 already_submitted_job_id = barrier_manipulator_job.external_id
 
 # for jobs with multiple input runs add `run=<int>` where <int> equals the input you wish to view.
 # without a targeted input run oqtant will default to the first run
-new_barrier_manipulator_job_stub = oqtant_client.get_job_inputs_without_output(already_submitted_job_id, include_notes=False)
+new_barrier_manipulator_job_stub = oqtant_client.get_job_inputs_without_output(
+    already_submitted_job_id, include_notes=False
+)
 
 # at this point 'new_job_stub' is a python dict with the following keys
 print("new barrier manipulator job stub keys:")
 print(new_barrier_manipulator_job_stub.keys())
 print("\n")
 
 # if you wish to include any job notes associated with the existing job input you can run the
@@ -243,15 +298,17 @@
 # new_job_stub = oqtant_client.get_job_inputs_without_output(already_submitted_job_id, include_notes=True)
 
 # from here you can update any of the inputs and the name of the job to your liking
 new_barrier_manipulator_job_stub["name"] = "this is a stub of another job"
 
 # at this point 'new_job_stub' can be provided to the 'generate_octant_job' function and then submitted with
 # the 'run_jobs' function as demonstrated in previous steps
-new_barrier_manipulator_job = oqtant_client.generate_oqtant_job(job=new_barrier_manipulator_job_stub)
+new_barrier_manipulator_job = oqtant_client.generate_oqtant_job(
+    job=new_barrier_manipulator_job_stub
+)
 print("new barrier manipulator job object:")
 print(new_barrier_manipulator_job)
 ```
 
 ## View your current job limits
 
 Your account provides you with a limited number of jobs which you can run in a given period of time. You can check your limits and current status against those limits via the `OqtantClient.get_limits()` method:
```

### Comparing `oqtant-0.16.1/documentation/walkthroughs/walkthrough_3_abstractions.ipynb` & `oqtant-0.16.2/documentation/walkthroughs/walkthrough_3_abstractions.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996714379104025%*

 * *Differences: {"'cells'": '{5: {\'source\': {insert: [(13, \'                    "times_ms": [-1600, -1200, '*

 * *            '-800, -400, 0],\\n\'), (17, \'                "lasers": None,\\n\'), (20, \'    '*

 * *            "],\\n')], delete: [20, 17, 13]}}, 11: {'source': {insert: [(1, '    times_ms=[-1600, "*

 * *            "-1200, -800, -400, 0],\\n'), (2, '    frequencies_mhz=[17.0, 8.0, 4.0, 1.2, "*

 * *            "0.045],\\n'), (3, '    powers_mw=[500.0, 500.0, 475.0, 360.0, 220.0],\\n'), (4, '    "*

 * *            'interpolation="LI […]*

```diff
@@ -59,22 +59,22 @@
                 "                \"time_of_flight_ms\": 8.0,\n",
                 "                \"image_type\": \"TIME_OF_FLIGHT\",\n",
                 "                \"end_time_ms\": 0.0,\n",
                 "                \"rf_evaporation\": {\n",
                 "                    \"frequencies_mhz\": [17.0, 8.0, 4.0, 1.2, 0.045],\n",
                 "                    \"powers_mw\": [500.0, 500.0, 475.0, 360.0, 220.0],\n",
                 "                    \"interpolation\": \"LINEAR\",\n",
-                "                    \"times_ms\": [-1600, -1200, -800, -400, 0]\n",
+                "                    \"times_ms\": [-1600, -1200, -800, -400, 0],\n",
                 "                },\n",
                 "                \"optical_barriers\": None,\n",
                 "                \"optical_landscape\": None,\n",
-                "                \"lasers\": None\n",
+                "                \"lasers\": None,\n",
                 "            }\n",
                 "        }\n",
-                "    ]\n",
+                "    ],\n",
                 "}"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "61960d47",
             "metadata": {},
@@ -134,18 +134,18 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "8eecbfcf",
             "metadata": {},
             "outputs": [],
             "source": [
                 "evap = JobSchema.RfEvaporation(\n",
-                "        times_ms = [-1600, -1200, -800, -400, 0],\n",
-                "        frequencies_mhz = [17.0, 8.0, 4.0, 1.2, 0.045],\n",
-                "        powers_mw = [500.0, 500.0, 475.0, 360.0, 220.0],\n",
-                "        interpolation = \"LINEAR\"\n",
+                "    times_ms=[-1600, -1200, -800, -400, 0],\n",
+                "    frequencies_mhz=[17.0, 8.0, 4.0, 1.2, 0.045],\n",
+                "    powers_mw=[500.0, 500.0, 475.0, 360.0, 220.0],\n",
+                "    interpolation=\"LINEAR\",\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "b419e866",
             "metadata": {},
@@ -156,20 +156,22 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "46013937",
             "metadata": {},
             "outputs": [],
             "source": [
-                "evap = JobSchema.RfEvaporation(**{\n",
+                "evap = JobSchema.RfEvaporation(\n",
+                "    **{\n",
                 "        \"times_ms\": [-1600, -1200, -800, -400, 0],\n",
                 "        \"frequencies_mhz\": [17.0, 8.0, 4.0, 1.2, 0.045],\n",
                 "        \"powers_mw\": [500.0, 490.0, 475.0, 360.0, 220.0],\n",
-                "        \"interpolation\": \"LINEAR\"\n",
-                "})"
+                "        \"interpolation\": \"LINEAR\",\n",
+                "    }\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "91e44d80",
             "metadata": {},
             "source": [
@@ -197,16 +199,16 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "c1454abe",
             "metadata": {},
             "outputs": [],
             "source": [
-                "print(evap.get_power(time = -100))\n",
-                "print(evap.get_frequency(time = -750))"
+                "print(evap.get_power(time=-100))\n",
+                "print(evap.get_frequency(time=-750))"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "5e1bbb11",
             "metadata": {},
             "source": [
@@ -216,16 +218,18 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "bc04d1bc",
             "metadata": {},
             "outputs": [],
             "source": [
-                "print(evap.get_power(time = 100))           # request after last defined object time of 0 ms -> 0.0\n",
-                "print(evap.get_frequency(time = -1800))     # request before first defined object time of -1600 ms -> 0.0"
+                "print(evap.get_power(time=100))  # request after last defined object time of 0 ms -> 0.0\n",
+                "print(\n",
+                "    evap.get_frequency(time=-1800)\n",
+                ")  # request before first defined object time of -1600 ms -> 0.0"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "0cfc0e41",
             "metadata": {},
             "source": [
@@ -237,16 +241,16 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "fb1cdf19",
             "metadata": {},
             "outputs": [],
             "source": [
-                "print(evap.get_powers(times = [-1600, -1000, -500, 0]))\n",
-                "print(evap.get_frequencies(times = [-1600, -1000, -600, 0]))"
+                "print(evap.get_powers(times=[-1600, -1000, -500, 0]))\n",
+                "print(evap.get_frequencies(times=[-1600, -1000, -600, 0]))"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "8e3c49f6",
             "metadata": {},
             "source": [
@@ -294,20 +298,20 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "dac67398",
             "metadata": {},
             "outputs": [],
             "source": [
                 "barr = JobSchema.Barrier(\n",
-                "    times_ms = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10], \n",
-                "    positions_um = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],\n",
-                "    heights_khz = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],\n",
-                "    widths_um = [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],\n",
-                "    interpolation = 'LINEAR',\n",
-                "    shape = 'GAUSSIAN'\n",
+                "    times_ms=[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10],\n",
+                "    positions_um=[1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],\n",
+                "    heights_khz=[1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],\n",
+                "    widths_um=[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],\n",
+                "    interpolation=\"LINEAR\",\n",
+                "    shape=\"GAUSSIAN\",\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f7b51028",
             "metadata": {},
@@ -318,22 +322,24 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "52d309d2",
             "metadata": {},
             "outputs": [],
             "source": [
-                "barr = JobSchema.Barrier(**{\n",
-                "    \"times_ms\": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10], \n",
-                "    \"positions_um\": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11], \n",
-                "    \"heights_khz\": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11], \n",
-                "    \"widths_um\": [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1], \n",
-                "    \"interpolation\": \"LINEAR\", \n",
-                "    \"shape\": \"GAUSSIAN\"\n",
-                "})"
+                "barr = JobSchema.Barrier(\n",
+                "    **{\n",
+                "        \"times_ms\": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10],\n",
+                "        \"positions_um\": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],\n",
+                "        \"heights_khz\": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],\n",
+                "        \"widths_um\": [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],\n",
+                "        \"interpolation\": \"LINEAR\",\n",
+                "        \"shape\": \"GAUSSIAN\",\n",
+                "    }\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d4951fca",
             "metadata": {},
             "source": [
@@ -359,16 +365,16 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "9f4d18c6",
             "metadata": {},
             "outputs": [],
             "source": [
-                "print(barr.get_position(time = 2))\n",
-                "print(barr.get_positions(times = [1,2,3]))"
+                "print(barr.get_position(time=2))\n",
+                "print(barr.get_positions(times=[1, 2, 3]))"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "811093a8",
             "metadata": {},
             "source": [
@@ -430,17 +436,17 @@
             "execution_count": null,
             "id": "69878534",
             "metadata": {},
             "outputs": [],
             "source": [
                 "xlim = [-5, 15]\n",
                 "ylim = [0, 12.5]\n",
-                "barr.plot_potential(time = 1, x_limits = xlim, y_limits = ylim)\n",
-                "barr.plot_potential(time = 5, x_limits = xlim, y_limits = ylim)\n",
-                "barr.plot_potential(time = 9, x_limits = xlim, y_limits = ylim)"
+                "barr.plot_potential(time=1, x_limits=xlim, y_limits=ylim)\n",
+                "barr.plot_potential(time=5, x_limits=xlim, y_limits=ylim)\n",
+                "barr.plot_potential(time=9, x_limits=xlim, y_limits=ylim)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "0250c6eb",
             "metadata": {},
             "source": [
@@ -471,18 +477,18 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "191c99c7",
             "metadata": {},
             "outputs": [],
             "source": [
                 "barr.shape = JobSchema.ShapeType.SQUARE\n",
-                "barr.plot_potential(time = 5, x_limits = [-25,25])\n",
+                "barr.plot_potential(time=5, x_limits=[-25, 25])\n",
                 "\n",
                 "barr.shape = JobSchema.ShapeType.LORENTZIAN\n",
-                "barr.plot_potential(time = 5, x_limits = [-25,25])"
+                "barr.plot_potential(time=5, x_limits=[-25, 25])"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "75e973a2",
             "metadata": {},
             "source": [
@@ -577,30 +583,29 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "3f95dd8f",
             "metadata": {},
             "outputs": [],
             "source": [
                 "landscape_1 = JobSchema.Landscape(\n",
-                "    time_ms = 1.0,\n",
-                "    positions_um = [-50, -25, 0, 25, 50],\n",
-                "    potentials_khz = [100, 50, 0, 50, 100],\n",
-                "    spatial_interpolation = 'LINEAR'\n",
+                "    time_ms=1.0,\n",
+                "    positions_um=[-50, -25, 0, 25, 50],\n",
+                "    potentials_khz=[100, 50, 0, 50, 100],\n",
+                "    spatial_interpolation=\"LINEAR\",\n",
                 ")\n",
                 "\n",
                 "landscape_2 = JobSchema.Landscape(\n",
-                "    time_ms = 10.0,\n",
-                "    positions_um = [-50, -25, 0, 25, 50],\n",
-                "    potentials_khz = [25, 12.5, 0, 12.5, 25],\n",
-                "    spatial_interpolation = 'LINEAR'\n",
+                "    time_ms=10.0,\n",
+                "    positions_um=[-50, -25, 0, 25, 50],\n",
+                "    potentials_khz=[25, 12.5, 0, 12.5, 25],\n",
+                "    spatial_interpolation=\"LINEAR\",\n",
                 ")\n",
                 "\n",
                 "optical_landscape = JobSchema.OpticalLandscape(\n",
-                "    interpolation = 'LINEAR',\n",
-                "    landscapes = [landscape_1, landscape_2]\n",
+                "    interpolation=\"LINEAR\", landscapes=[landscape_1, landscape_2]\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d806401b",
             "metadata": {},
@@ -623,15 +628,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "33a47e14",
             "metadata": {},
             "outputs": [],
             "source": [
                 "landscape_1.plot_potential()\n",
-                "landscape_2.plot_potential(y_limits = [-1, 101])"
+                "landscape_2.plot_potential(y_limits=[-1, 101])"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "1c3761b3",
             "metadata": {},
             "source": [
@@ -659,21 +664,21 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "84679acc",
             "metadata": {},
             "outputs": [],
             "source": [
-                "optical_landscape.plot_potential(time = 0.9)\n",
-                "optical_landscape.plot_potential(time = 1)\n",
-                "optical_landscape.plot_potential(time = 3)\n",
-                "optical_landscape.plot_potential(time = 5)\n",
-                "optical_landscape.plot_potential(time = 7)\n",
-                "optical_landscape.plot_potential(time = 9)\n",
-                "optical_landscape.plot_potential(time = 11)"
+                "optical_landscape.plot_potential(time=0.9)\n",
+                "optical_landscape.plot_potential(time=1)\n",
+                "optical_landscape.plot_potential(time=3)\n",
+                "optical_landscape.plot_potential(time=5)\n",
+                "optical_landscape.plot_potential(time=7)\n",
+                "optical_landscape.plot_potential(time=9)\n",
+                "optical_landscape.plot_potential(time=11)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "ea3712ef",
             "metadata": {},
             "source": [
@@ -718,38 +723,35 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "a0538c95",
             "metadata": {},
             "outputs": [],
             "source": [
                 "pulse_1 = JobSchema.Pulse(\n",
-                "    times_ms = [1, 1.5, 2, 3],\n",
-                "    intensities_mw_per_cm2 = [0, 10, 2, 0],\n",
-                "    detuning_mhz = 5,\n",
-                "    interpolation = 'SMOOTH'\n",
+                "    times_ms=[1, 1.5, 2, 3],\n",
+                "    intensities_mw_per_cm2=[0, 10, 2, 0],\n",
+                "    detuning_mhz=5,\n",
+                "    interpolation=\"SMOOTH\",\n",
                 ")\n",
                 "\n",
                 "pulse_2 = JobSchema.Pulse(\n",
-                "    times_ms = [5, 6, 7],\n",
-                "    intensities_mw_per_cm2 = [10, 5, 0],\n",
-                "    detuning_mhz = -10,\n",
-                "    interpolation = 'LINEAR'\n",
+                "    times_ms=[5, 6, 7],\n",
+                "    intensities_mw_per_cm2=[10, 5, 0],\n",
+                "    detuning_mhz=-10,\n",
+                "    interpolation=\"LINEAR\",\n",
                 ")\n",
                 "\n",
                 "pulse_3 = JobSchema.Pulse(\n",
-                "    times_ms = [9, 10, 11, 12],\n",
-                "    intensities_mw_per_cm2 = [0, 2.5, 2.5, 0],\n",
-                "    detuning_mhz = -5,\n",
-                "    interpolation = 'STEP'\n",
+                "    times_ms=[9, 10, 11, 12],\n",
+                "    intensities_mw_per_cm2=[0, 2.5, 2.5, 0],\n",
+                "    detuning_mhz=-5,\n",
+                "    interpolation=\"STEP\",\n",
                 ")\n",
                 "\n",
-                "laser = JobSchema.Laser(\n",
-                "    type = 'TERMINATOR',\n",
-                "    pulses = [pulse_1, pulse_2, pulse_3]\n",
-                ")"
+                "laser = JobSchema.Laser(type=\"TERMINATOR\", pulses=[pulse_1, pulse_2, pulse_3])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "663ea847",
             "metadata": {},
@@ -779,15 +781,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.11"
+            "version": "3.11.4"
         },
         "vscode": {
             "interpreter": {
                 "hash": "13fb51af87d45e56afa36501f99325526ec135b669e4eea3c0d0150b11fb593e"
             }
         }
     },
```

### Comparing `oqtant-0.16.1/documentation/walkthroughs/walkthrough_3_abstractions.md` & `oqtant-0.16.2/documentation/walkthroughs/walkthrough_3_abstractions.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,22 +21,22 @@
                 "time_of_flight_ms": 8.0,
                 "image_type": "TIME_OF_FLIGHT",
                 "end_time_ms": 0.0,
                 "rf_evaporation": {
                     "frequencies_mhz": [17.0, 8.0, 4.0, 1.2, 0.045],
                     "powers_mw": [500.0, 500.0, 475.0, 360.0, 220.0],
                     "interpolation": "LINEAR",
-                    "times_ms": [-1600, -1200, -800, -400, 0]
+                    "times_ms": [-1600, -1200, -800, -400, 0],
                 },
                 "optical_barriers": None,
                 "optical_landscape": None,
-                "lasers": None
+                "lasers": None,
             }
         }
-    ]
+    ],
 }
 ```
 
 We could then feed the above data structure to the API's _generate_oqtant_job()_ function to create the job object. Here, we would like to explore the contents of the underlying job data structure more in depth. The fields that control the behavior of the quantum matter machine are contained as _values_ in the _inputs_ list ([]). For now, we will only discuss cases where the _inputs_ list contains a single element. When this list's length is greater than one, it signifies a so-called _batch_ job, which will be discussed in a later walkthrough.
 
 The contents of _values_ includes directives on the type of imaging to perform (_image_type_ etc.) and how long to run the experiment (_end_time_ms_) after evaporation to BEC is complete. Also included are various job primitives that can be created and edited as programmable objects in their own right. These primitives include _rf_evaporation_, _optical_barriers_, _optical_landscape_, and _lasers_. Much like an _OqtantJob_ itself, these constituent primitives are programmatic objects in their own right and can be instantiated and manipulated outside of a job object. Although not shown explicitly in our simple job data structure above, both _optical_barriers_ and _lasers_ are lists containing _Barrier_ and _Laser_ objects, respectively. These objects will be explored below. You are likely already familiar with the structure of the _rf_evaporation_ data and how defining that data controls the evaporation to BEC in the experiment. The _optical_landscape_ data is a bit more complicated and will be explored in more detail below in a dedicated section.
 
@@ -60,59 +60,63 @@
 
 ### Construction
 
 Let us begin by constructing a stand-alone RfEvaporation object completely independently of any specific OqtantJob. We can create this object by either calling the constructor directly with the required data fields:
 
 ```python
 evap = JobSchema.RfEvaporation(
-        times_ms = [-1600, -1200, -800, -400, 0],
-        frequencies_mhz = [17.0, 8.0, 4.0, 1.2, 0.045],
-        powers_mw = [500.0, 500.0, 475.0, 360.0, 220.0],
-        interpolation = "LINEAR"
+    times_ms=[-1600, -1200, -800, -400, 0],
+    frequencies_mhz=[17.0, 8.0, 4.0, 1.2, 0.045],
+    powers_mw=[500.0, 500.0, 475.0, 360.0, 220.0],
+    interpolation="LINEAR",
 )
 ```
 
 or by placing the underlying data in a dictionary and unpacking that dictionary in order to pass it to the constructor:
 
 ```python
-evap = JobSchema.RfEvaporation(**{
+evap = JobSchema.RfEvaporation(
+    **{
         "times_ms": [-1600, -1200, -800, -400, 0],
         "frequencies_mhz": [17.0, 8.0, 4.0, 1.2, 0.045],
         "powers_mw": [500.0, 490.0, 475.0, 360.0, 220.0],
-        "interpolation": "LINEAR"
-})
+        "interpolation": "LINEAR",
+    }
+)
 ```
 
 Inherent to the RfEvaporation object are three lists, _times_ms_, _frequencies_mhz_, and _powers_mw_. The key prefix corresponds to the parameter being controlled, while the suffix refers to the associated units. In this case, we specify a list of times in milliseconds (ms), frequencies in MHz (mhz), and powers in milliwatts (mw). Note that all units are lower case, which can cause confusion if taken out of context. All three lists must share the same length as each time element is paired with the corresponding element of the frequencies/powers list(s). The specified behavior of the RF evaporation stage defind by the above data is as follows: At -1.6 seconds the RF power is set at 500 mW and the frequency (detuning) at 17 MHz. By the end of the evaporation period, defined by t=0, the frequency/detuning has decreased to 0.045 MHz = 45 kHz and the power has been reduced to 220 mW. Intermediate values of frequency and power are adopted between those two points in time, with the full time dependence being a result of the given data and chosen interpolation type, which controls how the RF fields behave between the given data points.
 
 Frequencies are given as a detuning with respect to the energetic trap bottom, so RF fields at a frequency/detuning of 0 would eliminate all atoms from the trap. Achieving final BEC temperatures on the order of 100 nK usually corresponds to final RF frequencies of a few tens of kHz. Powers refer to the amount of power delivered to an antenna that bathes the ultracold atoms with RF radiation. The actual local RF field experienced by the atoms depends on system losses and the exact geometry of the antenna.
 
 ### Time-dependent evaporation parameters
 
 We can explore the time-dependence of the RFEvaporation object frequency and power, as defined by the data structure above, using some useful functions included with oqtant. For example, we can query the object for the instantaneous power or frequency at any point in time. Recall that the units of power are mW and the units of frequency are MHz.
 
 ```python
-print(evap.get_power(time = -100))
-print(evap.get_frequency(time = -750))
+print(evap.get_power(time=-100))
+print(evap.get_frequency(time=-750))
 ```
 
 If we request the power or frequency for a time value outside the range of the underlying data, which would require extrapolation, we get 0.0:
 
 ```python
-print(evap.get_power(time = 100))           # request after last defined object time of 0 ms -> 0.0
-print(evap.get_frequency(time = -1800))     # request before first defined object time of -1600 ms -> 0.0
+print(evap.get_power(time=100))  # request after last defined object time of 0 ms -> 0.0
+print(
+    evap.get_frequency(time=-1800)
+)  # request before first defined object time of -1600 ms -> 0.0
 ```
 
 This behavior is generic to most objects in Oqtant -- any temporal or spatial extrapolation requests yield 0.0.
 
 There are also functions that extract the time-dependent parameters for a list of input times:
 
 ```python
-print(evap.get_powers(times = [-1600, -1000, -500, 0]))
-print(evap.get_frequencies(times = [-1600, -1000, -600, 0]))
+print(evap.get_powers(times=[-1600, -1000, -500, 0]))
+print(evap.get_frequencies(times=[-1600, -1000, -600, 0]))
 ```
 
 There are even useful plotting functions for visualizing these parameters over time.
 
 ```python
 evap.plot_power()
 evap.plot_frequency()
@@ -122,45 +126,47 @@
 
 ### Construction
 
 First, let us demonstrate the construction of a Barrier object, which represents a one-dimensional optical potential barrier to the BEC. A barrier is characterized by a shape, a time-dependent position, height, and width, and information on how to interpolate over the underlying data in time. For example, let us construct a Barrier object named _barr_ for which the center scans from 1-11 microns in the first 10 ms of an experiment. Over this same time period, the barrier height will increase from 1 kHz to 11 kHz. The width will remain constant at 1 micron throughout, as will the (fixed) Gaussian shape. In this case, the width parameter corresponds to the Gaussian width of the barrier.
 
 ```python
 barr = JobSchema.Barrier(
-    times_ms = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
-    positions_um = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],
-    heights_khz = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],
-    widths_um = [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
-    interpolation = 'LINEAR',
-    shape = 'GAUSSIAN'
+    times_ms=[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
+    positions_um=[1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],
+    heights_khz=[1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],
+    widths_um=[1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
+    interpolation="LINEAR",
+    shape="GAUSSIAN",
 )
 ```
 
 Alternatively, as above, we can create the same object by generating the underlying data in a dictionary and then unpacking that dictionary (using the \*\* prefix) when we pass it to the Barrier class constructor:
 
 ```python
-barr = JobSchema.Barrier(**{
-    "times_ms": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
-    "positions_um": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],
-    "heights_khz": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],
-    "widths_um": [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
-    "interpolation": "LINEAR",
-    "shape": "GAUSSIAN"
-})
+barr = JobSchema.Barrier(
+    **{
+        "times_ms": [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
+        "positions_um": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],
+        "heights_khz": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11],
+        "widths_um": [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
+        "interpolation": "LINEAR",
+        "shape": "GAUSSIAN",
+    }
+)
 ```
 
 The lists of time-dependent quantities (position, height, and width) used to define _barr_ must have the same length as the corresponding list of times. In this case, the ordered pairs consisting of a list of, e.g., [times, positions], will be linearly interpolated in time.
 
 ### Time-dependent barrier parameters
 
 We can explore the time-dependence of the barrier parameters using some in-built functions in pyubert. For example, we can retrieve and/or plot the barriers positions over time:
 
 ```python
-print(barr.get_position(time = 2))
-print(barr.get_positions(times = [1,2,3]))
+print(barr.get_position(time=2))
+print(barr.get_positions(times=[1, 2, 3]))
 ```
 
 Similarly, there are native functions for extracting a Barrier objects height and width at specified time(s). In our case, the width evolution is trivial (constant).
 
 ```python
 print(barr.get_height(1.5))
 print(barr.get_heights([1.5, 2.5, 3.5]))
@@ -180,17 +186,17 @@
 ### Plotting the potential energy for a barrier
 
 There are also methods native to oqtant for plotting Barrier object potential energies at different times of the experiment. Here, we will explicitly specify the positional range of the plot (x-axis domain) in order to better be able to see the barrier displacement.
 
 ```python
 xlim = [-5, 15]
 ylim = [0, 12.5]
-barr.plot_potential(time = 1, x_limits = xlim, y_limits = ylim)
-barr.plot_potential(time = 5, x_limits = xlim, y_limits = ylim)
-barr.plot_potential(time = 9, x_limits = xlim, y_limits = ylim)
+barr.plot_potential(time=1, x_limits=xlim, y_limits=ylim)
+barr.plot_potential(time=5, x_limits=xlim, y_limits=ylim)
+barr.plot_potential(time=9, x_limits=xlim, y_limits=ylim)
 ```
 
 ### Exploring Barrier shape options
 
 Supported Barrier shape options include GAUSSIAN, SQUARE, and LORENTZIAN. In all three cases, the "width_um" parameter list means something slightly different. For the GAUSSIAN case, the functional form of the barrier potential $U(x)$ follows the standard Gaussian formula
 
 $$
@@ -207,18 +213,18 @@
 
 i.e. our width parameter w(t) corresponds to the half-width half-max of the Lorentzian.
 
 For the SQUARE case, the potential is simple a flat-topped potential-energy hill of height H(t) and _full_ width w(t).
 
 ```python
 barr.shape = JobSchema.ShapeType.SQUARE
-barr.plot_potential(time = 5, x_limits = [-25,25])
+barr.plot_potential(time=5, x_limits=[-25, 25])
 
 barr.shape = JobSchema.ShapeType.LORENTZIAN
-barr.plot_potential(time = 5, x_limits = [-25,25])
+barr.plot_potential(time=5, x_limits=[-25, 25])
 ```
 
 Note that the resolution of the projected light optical system is on the order of 2 microns. Thus, _Barrier_ objects with small widths will all appear similar in reality (the experiment) even if they have different _shape_ settings.
 
 ### Exploring Barrier interpolation options
 
 A Barrier object's 'interpolation' style determines how the time-dependent position, height, and width are determined for intermediate times between the provided data points in the 'times_ms' list class member. At this time, the interpolation choice is _shared_ for all three time-dependent barrier parameters. Let us explore the effects of different interpolation choices by altering the time-dependent position of our barrier, to make it a little more interesting, and then plot the position over time for a few different interpolation choices.
@@ -247,61 +253,60 @@
 
 ### Construction
 
 We can directly compose an _OpticalLandscape_ object, as above with the _Barrier_ object(s), or we can compose the constituent Landscape objects and then compose the full _OpticalLandscape_ object accordingly:
 
 ```python
 landscape_1 = JobSchema.Landscape(
-    time_ms = 1.0,
-    positions_um = [-50, -25, 0, 25, 50],
-    potentials_khz = [100, 50, 0, 50, 100],
-    spatial_interpolation = 'LINEAR'
+    time_ms=1.0,
+    positions_um=[-50, -25, 0, 25, 50],
+    potentials_khz=[100, 50, 0, 50, 100],
+    spatial_interpolation="LINEAR",
 )
 
 landscape_2 = JobSchema.Landscape(
-    time_ms = 10.0,
-    positions_um = [-50, -25, 0, 25, 50],
-    potentials_khz = [25, 12.5, 0, 12.5, 25],
-    spatial_interpolation = 'LINEAR'
+    time_ms=10.0,
+    positions_um=[-50, -25, 0, 25, 50],
+    potentials_khz=[25, 12.5, 0, 12.5, 25],
+    spatial_interpolation="LINEAR",
 )
 
 optical_landscape = JobSchema.OpticalLandscape(
-    interpolation = 'LINEAR',
-    landscapes = [landscape_1, landscape_2]
+    interpolation="LINEAR", landscapes=[landscape_1, landscape_2]
 )
 ```
 
 ### Inspecting consituent 'Landscape' objects
 
 ```python
 print(landscape_1.get_potential_at_position(10))
 print(landscape_2.get_potential_at_positions([-75, -50, -25, 0, 25, 50, 75]))
 ```
 
 ```python
 landscape_1.plot_potential()
-landscape_2.plot_potential(y_limits = [-1, 101])
+landscape_2.plot_potential(y_limits=[-1, 101])
 ```
 
 In the plots above, you can see the potential energy profile specified by our two Landscape objects. The underlying data shows up as points, with the overall profile determined by the values of these points and the chosen value for _spatial_interpolation_. The same values are available here as were for (temporal) interpolation options for Barrier objects.
 
 ### Understanding the time dependence of the composed OpticalLandscape object
 
 The time-dependence of the overall optical potential-energy landscape, as derived from the individual _landscapes[]_ list, is somewhat complicated. As for _Barrier_ and other similar objects, any temporal extrapolation (behavior for data outside the defined time period, i.e. before the first or after the last elements of the _landscapes[]_ list) results in zero potential (in the absence of any other sources, such as Barriers). Therefore, the only way to get a non-zero painted potential optical landscape is to define at least two landscapes that can be interpolated between. To hold a static (unchanging) potential during a period of the experiment, one would define two elements of the _landscapes[]_ list with identical potential energy profiles but differing times, with the potential being applied between those two times. If one desires the potential to change dynamically, then adjacent elements of the _landscapes[]_ list (elements with the nearest _time_ms_ values) should define the snapshots of the desired potential at the temporal endpoints. In between these endpoints the potential landscape is interpolated point-by-point (in position) according to the user-specified value for _interpolation_. This process continues so that, at the specified times of the elements of _landscapes[]_, the overall optical potential energy landscape instantaneously equal to those individual landscapes.
 
 In our example above, with linear interpolation, this means that there will be a period of no optical potential between 0 and 1 ms, our _landscape_1_ potential will start being applied at 1 ms, this potential will smoothly (linearly, in this case) morph into the _landscape_2_ potential between 1 and 10 ms, and then this potential landscape will be held until the end of the experiment. Let us use oqtant's visualization functions to inspect this behavior to make it clear.
 
 ```python
-optical_landscape.plot_potential(time = 0.9)
-optical_landscape.plot_potential(time = 1)
-optical_landscape.plot_potential(time = 3)
-optical_landscape.plot_potential(time = 5)
-optical_landscape.plot_potential(time = 7)
-optical_landscape.plot_potential(time = 9)
-optical_landscape.plot_potential(time = 11)
+optical_landscape.plot_potential(time=0.9)
+optical_landscape.plot_potential(time=1)
+optical_landscape.plot_potential(time=3)
+optical_landscape.plot_potential(time=5)
+optical_landscape.plot_potential(time=7)
+optical_landscape.plot_potential(time=9)
+optical_landscape.plot_potential(time=11)
 ```
 
 As descibed above, we can see zero overall potential both before the first and after the last times of the individual Landscape objects. At 1 ms, the first Landscape is assumed. The potential landscape then morphs into our second Landscape object at t = 10 ms.
 
 ## Laser Objects
 
 The last data structure to explore here is the _lasers[]_ list in the job data. This is a list of _Laser_ objects. Currently, the user is limited to a single element/laser.
@@ -310,40 +315,33 @@
 
 Let us begin by constructing a _Laser_ object, which gives the user control over near-resonant laser light applied to the atoms over the course of the experiment. This differs from the painted potential laser, which is far off-resonance in order to apply potential energy landscapes and barriers to the trapped condensate. Resonant or near-resonant light, on the other hand, results in scattering of photons from the light field by the atoms. This is useful, for example, in TRANSISTOR jobs where we want to remove atoms from some spatial region of the trap using a so-called TERMINATOR laser.
 
 A _Laser_ object gives the user control of the time-dependence of laser light applied to the atomic ensemble, including the time-dependent intensity and detuning given by a series of _pulse_ objects specified by a _pulses[]_ list. We can construct such an object as follows:
 
 ```python
 pulse_1 = JobSchema.Pulse(
-    times_ms = [1, 1.5, 2, 3],
-    intensities_mw_per_cm2 = [0, 10, 2, 0],
-    detuning_mhz = 5,
-    interpolation = 'SMOOTH'
+    times_ms=[1, 1.5, 2, 3],
+    intensities_mw_per_cm2=[0, 10, 2, 0],
+    detuning_mhz=5,
+    interpolation="SMOOTH",
 )
 
 pulse_2 = JobSchema.Pulse(
-    times_ms = [5, 6, 7],
-    intensities_mw_per_cm2 = [10, 5, 0],
-    detuning_mhz = -10,
-    interpolation = 'LINEAR'
+    times_ms=[5, 6, 7],
+    intensities_mw_per_cm2=[10, 5, 0],
+    detuning_mhz=-10,
+    interpolation="LINEAR",
 )
 
 pulse_3 = JobSchema.Pulse(
-    times_ms = [9, 10, 11, 12],
-    intensities_mw_per_cm2 = [0, 2.5, 2.5, 0],
-    detuning_mhz = -5,
-    interpolation = 'STEP'
+    times_ms=[9, 10, 11, 12],
+    intensities_mw_per_cm2=[0, 2.5, 2.5, 0],
+    detuning_mhz=-5,
+    interpolation="STEP",
 )
 
-laser = JobSchema.Laser(
-    type = 'TERMINATOR',
-    pulses = [pulse_1, pulse_2, pulse_3]
-)
+laser = JobSchema.Laser(type="TERMINATOR", pulses=[pulse_1, pulse_2, pulse_3])
 ```
 
 ```python
 laser.plot_intensity()
 ```
-
-```python
-
-```
```

### Comparing `oqtant-0.16.1/documentation/walkthroughs/walkthrough_4_experiment.ipynb` & `oqtant-0.16.2/documentation/walkthroughs/walkthrough_4_experiment.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9931771164021164%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(10, '    round_sig,\\n')], delete: [10]}}, 11: {'source': "*

 * *            '{insert: [(4, \'    job["name"] = "RF sweep experiment step " + str(step + 1)\\n\'), '*

 * *            '(5, \'    job["notes"] = "RF sweep experiment step " + str(step + 1) + " of " + '*

 * *            "str(njobs)\\n'), (6, '    "*

 * *            'job["inputs"][0]["values"]["rf_evaporation"]["frequencies_mhz"][\\n\'), (7, \'        '*

 * *            "-1\\n'), (8, '    ] = final_rf_freqs_mhz[step]\\n'), (12, '\\n' […]*

```diff
@@ -38,15 +38,15 @@
                 "from oqtant.util.auth import get_user_token\n",
                 "from bert_schemas import job as JobSchema\n",
                 "from oqtant.schemas.job import (\n",
                 "    OqtantJob,\n",
                 "    Gaussian_dist_2D,\n",
                 "    TF_dist_2D,\n",
                 "    bimodal_dist_2D,\n",
-                "    round_sig\n",
+                "    round_sig,\n",
                 ")\n",
                 "\n",
                 "token = get_user_token(auth_server_port=8080)"
             ]
         },
         {
             "cell_type": "markdown",
@@ -165,30 +165,25 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "njobs = len(final_rf_freqs_mhz)\n",
                 "jobs = []\n",
                 "for step in range(njobs):\n",
                 "    job = copy.deepcopy(base_ultracold_matter_job)\n",
-                "    job[\"name\"] = \"RF sweep experiment step \" + str(step+1)\n",
-                "    job[\"notes\"] = \"RF sweep experiment step \" + str(step+1) + \" of \" + str(njobs)\n",
-                "    job[\"inputs\"][0][\"values\"][\"rf_evaporation\"][\"frequencies_mhz\"][-1] = final_rf_freqs_mhz[step]\n",
+                "    job[\"name\"] = \"RF sweep experiment step \" + str(step + 1)\n",
+                "    job[\"notes\"] = \"RF sweep experiment step \" + str(step + 1) + \" of \" + str(njobs)\n",
+                "    job[\"inputs\"][0][\"values\"][\"rf_evaporation\"][\"frequencies_mhz\"][\n",
+                "        -1\n",
+                "    ] = final_rf_freqs_mhz[step]\n",
                 "    jobs.append(job)\n",
                 "\n",
                 "jobs = [oqtant_client.generate_oqtant_job(job=job) for job in jobs]\n",
-                "    \n",
+                "\n",
                 "for job in jobs:\n",
-                "    print(\n",
-                "        job.name,\n",
-                "        \"\\n\",\n",
-                "        job.inputs[0].values,\n",
-                "        \"\\n\"\n",
-                "    )\n",
-                "    \n",
-                "batch_job = oqtant_client.generate_oqtant_job(job=batch_job)"
+                "    print(job.name, \"\\n\", job.inputs[0].values, \"\\n\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Generating OqtantJob parameters as EXPLORER / INNOVATOR ## \n",
@@ -212,19 +207,16 @@
                 "for step in range(njobs):\n",
                 "    input = copy.deepcopy(base_ultracold_matter_job[\"inputs\"][0])\n",
                 "    input[\"values\"][\"rf_evaporation\"][\"frequencies_mhz\"][-1] = final_rf_freqs_mhz[step]\n",
                 "    batch_job[\"inputs\"].append(input)\n",
                 "\n",
                 "print(batch_job[\"name\"])\n",
                 "for input in batch_job[\"inputs\"]:\n",
-                "    print(\n",
-                "        input,\n",
-                "        \"\\n\"\n",
-                "    )\n",
-                "    \n",
+                "    print(input, \"\\n\")\n",
+                "\n",
                 "batch_job = oqtant_client.generate_oqtant_job(job=batch_job)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -264,26 +256,26 @@
             "outputs": [],
             "source": [
                 "# if using the GROUND option\n",
                 "for job in jobs:\n",
                 "    print(\n",
                 "        job.name,\n",
                 "        job.inputs[0].values.rf_evaporation.frequencies_mhz[-1],\n",
-                "        job.inputs[0].values.time_of_flight_ms\n",
+                "        job.inputs[0].values.time_of_flight_ms,\n",
                 "    )\n",
                 "\n",
                 "print(\"\\n\")\n",
                 "\n",
                 "# if using the EXPLORER / INNOVATOR option\n",
                 "for i, input in enumerate(batch_job.inputs):\n",
                 "    print(\n",
                 "        batch_job.name,\n",
                 "        f\"input run #{i + 1}\",\n",
                 "        input.values.rf_evaporation.frequencies_mhz[-1],\n",
-                "        input.values.time_of_flight_ms\n",
+                "        input.values.time_of_flight_ms,\n",
                 "    )"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -302,21 +294,21 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# track the status \n",
+                "# track the status\n",
                 "rf_sweep_experiment_job_ids = oqtant_client.run_jobs(job_list=jobs, track_status=True)\n",
                 "\n",
-                "# dont track the status \n",
+                "# dont track the status\n",
                 "# rf_sweep_experiment_job_ids = oqtant_client.run_jobs(job_list=experiment_jobs, track_status=False)\n",
                 "\n",
-                "with open('bec_rf_sweep_experiment.txt', 'w') as filewriter:\n",
+                "with open(\"bec_rf_sweep_experiment.txt\", \"w\") as filewriter:\n",
                 "    for experiment_step_job_id in rf_sweep_experiment_job_ids:\n",
                 "        filewriter.write(experiment_step_job_id)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -336,21 +328,23 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# track the status \n",
-                "rf_sweep_experiment_job_id = oqtant_client.run_jobs(job_list=[batch_job], track_status=True)[0]\n",
+                "# track the status\n",
+                "rf_sweep_experiment_job_id = oqtant_client.run_jobs(\n",
+                "    job_list=[batch_job], track_status=True\n",
+                ")[0]\n",
                 "\n",
-                "# dont track the status \n",
+                "# dont track the status\n",
                 "# rf_sweep_experiment_job_id = oqtant_client.run_jobs(job_list=[experiment_job], track_status=False)[0]\n",
                 "\n",
-                "with open('bec_rf_sweep_experiment.txt', 'w') as filewriter:\n",
+                "with open(\"bec_rf_sweep_experiment.txt\", \"w\") as filewriter:\n",
                 "    filewriter.write(rf_sweep_experiment_job_id)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -361,19 +355,19 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "with open('bec_rf_sweep_experiment.txt', 'r') as filereader:\n",
+                "with open(\"bec_rf_sweep_experiment.txt\", \"r\") as filereader:\n",
                 "    for line in filereader:\n",
                 "        # remove linebreak which is the last character of the string\n",
                 "        oqtant_client.load_job_from_id(line)\n",
-                "        \n",
+                "\n",
                 "for job_id, job in oqtant_client.active_jobs.items():\n",
                 "    print(\"id: \", job_id, job.job_type, job.status)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -386,32 +380,45 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "for a, job in oqtant_client.active_jobs.items():\n",
-                "    if job.status == JobSchema.JobStatus.COMPLETE and job.job_type == JobSchema.JobType.BEC:\n",
+                "    if (\n",
+                "        job.status == JobSchema.JobStatus.COMPLETE\n",
+                "        and job.job_type == JobSchema.JobType.BEC\n",
+                "    ):\n",
                 "        job.atoms_2dplot()\n",
                 "        job.atoms_sliceplot()\n",
-                "        \n",
+                "\n",
                 "# by default jobs that are loaded will only contain the first input/output entry\n",
                 "# if you have more than one input for a job you can view its details by specifying the 'run' like below\n",
-                "desired_input_run = 2 # here we are asking for the second input/output entry\n",
-                "with open('bec_rf_sweep_experiment.txt', 'r') as filereader:\n",
+                "desired_input_run = 2  # here we are asking for the second input/output entry\n",
+                "with open(\"bec_rf_sweep_experiment.txt\", \"r\") as filereader:\n",
                 "    for line in filereader:\n",
                 "        # remove linebreak which is the last character of the string\n",
                 "        oqtant_client.load_job_from_id(line, run=desired_input_run)\n",
-                "        \n",
+                "\n",
                 "# now we can display the second input/output entry results\n",
                 "for a, job in oqtant_client.active_jobs.items():\n",
-                "    if job.status == JobSchema.JobStatus.COMPLETE and job.job_type == JobSchema.JobType.BEC:\n",
+                "    if (\n",
+                "        job.status == JobSchema.JobStatus.COMPLETE\n",
+                "        and job.job_type == JobSchema.JobType.BEC\n",
+                "    ):\n",
                 "        job.atoms_2dplot()\n",
                 "        job.atoms_sliceplot()"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
```

### Comparing `oqtant-0.16.1/documentation/walkthroughs/walkthrough_4_experiment.md` & `oqtant-0.16.2/documentation/walkthroughs/walkthrough_4_experiment.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from oqtant.util.auth import get_user_token
 from bert_schemas import job as JobSchema
 from oqtant.schemas.job import (
     OqtantJob,
     Gaussian_dist_2D,
     TF_dist_2D,
     bimodal_dist_2D,
-    round_sig
+    round_sig,
 )
 
 token = get_user_token(auth_server_port=8080)
 ```
 
 ## Creating a OqtantClient Instance
 
@@ -106,30 +106,25 @@
 Print out the OqtantJobs once updated to review the input parameters before submitting to run on the Oraqle hardware. Once a job is submitted, it can only be cancelled by contacting **albert@infleqtion.com**
 
 ```python
 njobs = len(final_rf_freqs_mhz)
 jobs = []
 for step in range(njobs):
     job = copy.deepcopy(base_ultracold_matter_job)
-    job["name"] = "RF sweep experiment step " + str(step+1)
-    job["notes"] = "RF sweep experiment step " + str(step+1) + " of " + str(njobs)
-    job["inputs"][0]["values"]["rf_evaporation"]["frequencies_mhz"][-1] = final_rf_freqs_mhz[step]
+    job["name"] = "RF sweep experiment step " + str(step + 1)
+    job["notes"] = "RF sweep experiment step " + str(step + 1) + " of " + str(njobs)
+    job["inputs"][0]["values"]["rf_evaporation"]["frequencies_mhz"][
+        -1
+    ] = final_rf_freqs_mhz[step]
     jobs.append(job)
 
 jobs = [oqtant_client.generate_oqtant_job(job=job) for job in jobs]
 
 for job in jobs:
-    print(
-        job.name,
-        "\n",
-        job.inputs[0].values,
-        "\n"
-    )
-
-batch_job = oqtant_client.generate_oqtant_job(job=batch_job)
+    print(job.name, "\n", job.inputs[0].values, "\n")
 ```
 
 ## Generating OqtantJob parameters as EXPLORER / INNOVATOR
 
 This experiment will consist of a single OqtantJob with 3 inputs and no repeated trials. Below we will create an input object with default Ultracold Matter parameters. Next we will copy this input three times and make updates to match the steps in the experiment.
 
 Print out the job inputs once updated to review the parameters before submitting to run on the Oraqle hardware. Once a job is submitted, it can only be cancelled by contacting **albert@infleqtion.com**
@@ -143,18 +138,15 @@
 for step in range(njobs):
     input = copy.deepcopy(base_ultracold_matter_job["inputs"][0])
     input["values"]["rf_evaporation"]["frequencies_mhz"][-1] = final_rf_freqs_mhz[step]
     batch_job["inputs"].append(input)
 
 print(batch_job["name"])
 for input in batch_job["inputs"]:
-    print(
-        input,
-        "\n"
-    )
+    print(input, "\n")
 
 batch_job = oqtant_client.generate_oqtant_job(job=batch_job)
 ```
 
 ## Accessing the fields of an OqtantJob
 
 The OqtantJob class is the python representation of an Oqtant job's input parameters and (if completed) it's output results. When working in Oqtant this class will be used to generate new jobs and interact with submitted jobs. You can access the information inside each OqtantJob using dot-notation.
@@ -184,26 +176,26 @@
 
 ```python
 # if using the GROUND option
 for job in jobs:
     print(
         job.name,
         job.inputs[0].values.rf_evaporation.frequencies_mhz[-1],
-        job.inputs[0].values.time_of_flight_ms
+        job.inputs[0].values.time_of_flight_ms,
     )
 
 print("\n")
 
 # if using the EXPLORER / INNOVATOR option
 for i, input in enumerate(batch_job.inputs):
     print(
         batch_job.name,
         f"input run #{i + 1}",
         input.values.rf_evaporation.frequencies_mhz[-1],
-        input.values.time_of_flight_ms
+        input.values.time_of_flight_ms,
     )
 ```
 
 ## Submiting OqtantJobs and storing the their IDs as GROUND
 
 Once you are ready to submit the experiment jobs you will have two options. One will be to track the status of them as they are processed and the other will be to not track their status. When you choose to track the status of your submitted jobs the function will not return immediately and will instead continuously ping the Oraqle service until all of the jobs have finished.
 
@@ -218,15 +210,15 @@
 ```python
 # track the status
 rf_sweep_experiment_job_ids = oqtant_client.run_jobs(job_list=jobs, track_status=True)
 
 # dont track the status
 # rf_sweep_experiment_job_ids = oqtant_client.run_jobs(job_list=experiment_jobs, track_status=False)
 
-with open('bec_rf_sweep_experiment.txt', 'w') as filewriter:
+with open("bec_rf_sweep_experiment.txt", "w") as filewriter:
     for experiment_step_job_id in rf_sweep_experiment_job_ids:
         filewriter.write(experiment_step_job_id)
 ```
 
 ## Submiting OqtantJobs and storing their IDs as EXPLORER / INNOVATOR
 
 Once you are ready to submit the experiment job you will have two options. One will be to track the status of it as it is being processed and the other will be to not track it's status. When you choose to track the status of your submitted job the function will not return immediately and will instead continuously ping the Oraqle service until the job has finished.
@@ -237,54 +229,62 @@
 
 Regardless of which method you choose, it is always a good idea to save the IDs of your jobs for future reference.
 
 Option to run the jobs and wait for results (`track_status=True`) OR submit the jobs and return later to retrieve the results (`track_status=False`). Either way, be sure to save the job ids to a file if you plan to retrieve the data for later processing.
 
 ```python
 # track the status
-rf_sweep_experiment_job_id = oqtant_client.run_jobs(job_list=[batch_job], track_status=True)[0]
+rf_sweep_experiment_job_id = oqtant_client.run_jobs(
+    job_list=[batch_job], track_status=True
+)[0]
 
 # dont track the status
 # rf_sweep_experiment_job_id = oqtant_client.run_jobs(job_list=[experiment_job], track_status=False)[0]
 
-with open('bec_rf_sweep_experiment.txt', 'w') as filewriter:
+with open("bec_rf_sweep_experiment.txt", "w") as filewriter:
     filewriter.write(rf_sweep_experiment_job_id)
 ```
 
 ## Load results from completed OqtantJobs
 
 Use `OqtantClient.load_jobs_from_id()` to retrieve jobs in any state from a previous run.
 
 ```python
-with open('bec_rf_sweep_experiment.txt', 'r') as filereader:
+with open("bec_rf_sweep_experiment.txt", "r") as filereader:
     for line in filereader:
         # remove linebreak which is the last character of the string
         oqtant_client.load_job_from_id(line)
 
 for job_id, job in oqtant_client.active_jobs.items():
     print("id: ", job_id, job.job_type, job.status)
 ```
 
 ## Plot completed OqtantJobs
 
 Once your OqtantJob(s) status is COMPLETE, plot the results
 
 ```python
 for a, job in oqtant_client.active_jobs.items():
-    if job.status == JobSchema.JobStatus.COMPLETE and job.job_type == JobSchema.JobType.BEC:
+    if (
+        job.status == JobSchema.JobStatus.COMPLETE
+        and job.job_type == JobSchema.JobType.BEC
+    ):
         job.atoms_2dplot()
         job.atoms_sliceplot()
 
 # by default jobs that are loaded will only contain the first input/output entry
 # if you have more than one input for a job you can view its details by specifying the 'run' like below
-desired_input_run = 2 # here we are asking for the second input/output entry
-with open('bec_rf_sweep_experiment.txt', 'r') as filereader:
+desired_input_run = 2  # here we are asking for the second input/output entry
+with open("bec_rf_sweep_experiment.txt", "r") as filereader:
     for line in filereader:
         # remove linebreak which is the last character of the string
         oqtant_client.load_job_from_id(line, run=desired_input_run)
 
 # now we can display the second input/output entry results
 for a, job in oqtant_client.active_jobs.items():
-    if job.status == JobSchema.JobStatus.COMPLETE and job.job_type == JobSchema.JobType.BEC:
+    if (
+        job.status == JobSchema.JobStatus.COMPLETE
+        and job.job_type == JobSchema.JobType.BEC
+    ):
         job.atoms_2dplot()
         job.atoms_sliceplot()
 ```
```

### Comparing `oqtant-0.16.1/documentation/walkthroughs/walkthrough_5_optimization.ipynb` & `oqtant-0.16.2/documentation/walkthroughs/walkthrough_5_optimization.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9979246156621641%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(18, '    round_sig,\\n')], delete: [18]}}, 6: {'source': "*

 * *            "{insert: [(25, '\\n'), (26, 'def cost_func_5D(RF_freqs=[17.0, 8.0, 4.0, 1.2, "*

 * *            "0.045]):  # added 5th power to default\\n'), (27, '    "*

 * *            'base_ultracold_matter_job["inputs"][0]["values"]["rf_evaporation"][\\n\'), (28, '*

 * *            '\'        "frequencies_mhz"\\n\'), (29, \'    ] = list(RF_freqs)\\n\'), (37, \'    C '*

 * *            "= (Nth * T) / Nc\\n')], delete: [34, 26, 25] […]*

```diff
@@ -46,15 +46,15 @@
                 "from oqtant.util.auth import get_user_token\n",
                 "from bert_schemas import job as JobSchema\n",
                 "from oqtant.schemas.job import (\n",
                 "    OqtantJob,\n",
                 "    Gaussian_dist_2D,\n",
                 "    TF_dist_2D,\n",
                 "    bimodal_dist_2D,\n",
-                "    round_sig\n",
+                "    round_sig,\n",
                 ")\n",
                 "import csv\n",
                 "\n",
                 "token = get_user_token(auth_server_port=8080)"
             ]
         },
         {
@@ -121,24 +121,27 @@
                 "                \"optical_landscape\": None,\n",
                 "                \"lasers\": None,\n",
                 "            },\n",
                 "        }\n",
                 "    ],\n",
                 "}\n",
                 "\n",
-                "def cost_func_5D(RF_freqs = [17.0, 8.0, 4.0, 1.2, 0.045]): # added 5th power to default\n",
-                "    base_ultracold_matter_job[\"inputs\"][0][\"values\"][\"rf_evaporation\"][\"frequencies_mhz\"] = list(RF_freqs)\n",
+                "\n",
+                "def cost_func_5D(RF_freqs=[17.0, 8.0, 4.0, 1.2, 0.045]):  # added 5th power to default\n",
+                "    base_ultracold_matter_job[\"inputs\"][0][\"values\"][\"rf_evaporation\"][\n",
+                "        \"frequencies_mhz\"\n",
+                "    ] = list(RF_freqs)\n",
                 "    print(base_ultracold_matter_job)\n",
                 "    job = oqtant_client.generate_oqtant_job(job=base_ultracold_matter_job)\n",
                 "    [job_id] = oqtant_client.run_jobs(job_list=[job], track_status=True)\n",
                 "    job_output = oqtant_client.active_jobs[job_id].inputs[0].output.values\n",
                 "    Nth = job_output.thermal_atom_number\n",
                 "    T = job_output.temperature_uk\n",
                 "    Nc = job_output.condensed_atom_number\n",
-                "    C = (Nth*T)/Nc\n",
+                "    C = (Nth * T) / Nc\n",
                 "    costs_5D.append(C)\n",
                 "    return C"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -150,15 +153,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "bnds_5d = ((0,50),(0,50),(0,50),(0,50),(0,50))"
+                "bnds_5d = ((0, 50), (0, 50), (0, 50), (0, 50), (0, 50))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Choose an optimization algorithm ##\n",
@@ -178,15 +181,21 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "res_5d = minimize(cost_func_5D, method=\"TNC\", bounds=bnds_5d, x0 = [17,8,4,1.2,0.05], options={'maxiter':10})\n",
+                "res_5d = minimize(\n",
+                "    cost_func_5D,\n",
+                "    method=\"TNC\",\n",
+                "    bounds=bnds_5d,\n",
+                "    x0=[17, 8, 4, 1.2, 0.05],\n",
+                "    options={\"maxiter\": 10},\n",
+                ")\n",
                 "\n",
                 "print(\"optimization results freq tuning:\")\n",
                 "print(res_5d)"
             ]
         },
         {
             "cell_type": "markdown",
@@ -218,15 +227,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def cost(Nc, Nth, T):\n",
-                "    C = (Nth*T)/Nc\n",
+                "    C = (Nth * T) / Nc\n",
                 "    return C"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -254,16 +263,15 @@
                 "    job = oqtant_client.active_jobs[job_id]\n",
                 "    output = job.inputs[0].output.values\n",
                 "    condensed_atom_number = output.condensed_atom_number\n",
                 "    thermal_atom_number = output.thermal_atom_number\n",
                 "    temperature_uk = output.temperature_uk\n",
                 "    input = job.inputs[0].values\n",
                 "    x_train.append(input.rf_evaporation.frequencies_mhz)\n",
-                "    y_train.append(cost(condensed_atom_number, thermal_atom_number, temperature_uk)) \n",
-                "    "
+                "    y_train.append(cost(condensed_atom_number, thermal_atom_number, temperature_uk))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -309,17 +317,17 @@
             "source": [
                 "def acquisition(X, Xsamples, model):\n",
                 "    # calculate the best surrogate score found so far\n",
                 "    yhat, _ = surrogate(model, X)\n",
                 "    best = max(yhat)\n",
                 "    # calculate mean and stdev via surrogate function\n",
                 "    mu, std = surrogate(model, Xsamples)\n",
-                "    #mu = mu[:, 0]\n",
+                "    # mu = mu[:, 0]\n",
                 "    # calculate the probability of improvement\n",
-                "    probs = norm.cdf((mu - best) / (std+1E-9))\n",
+                "    probs = norm.cdf((mu - best) / (std + 1e-9))\n",
                 "    return probs"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -330,21 +338,31 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "domain = [(20.,15.),(12.,5.),(5.,2.),(1.9,0.2),(0.2,0.01),\n",
-                "          (500.,470.),(470.,460.),(459.,420.),(420.,350.)]\n",
+                "domain = [\n",
+                "    (20.0, 15.0),\n",
+                "    (12.0, 5.0),\n",
+                "    (5.0, 2.0),\n",
+                "    (1.9, 0.2),\n",
+                "    (0.2, 0.01),\n",
+                "    (500.0, 470.0),\n",
+                "    (470.0, 460.0),\n",
+                "    (459.0, 420.0),\n",
+                "    (420.0, 350.0),\n",
+                "]\n",
+                "\n",
                 "\n",
                 "def rand_domain_sample(domain):\n",
-                "    scale = domain[0]-domain[1]\n",
-                "    random_number = np.random.uniform()+(1E-9)\n",
-                "    sample = scale*random_number+domain[1]\n",
+                "    scale = domain[0] - domain[1]\n",
+                "    random_number = np.random.uniform() + (1e-9)\n",
+                "    sample = scale * random_number + domain[1]\n",
                 "    return sample"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -357,15 +375,20 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def optimize_acquisition(X, y, model, sample_population):\n",
                 "    # random search, generate random samples\n",
-                "    Xsamples = np.asarray([[rand_domain_sample(domain[i]) for i in range(len(X[0]))] for j in range(sample_population)])\n",
+                "    Xsamples = np.asarray(\n",
+                "        [\n",
+                "            [rand_domain_sample(domain[i]) for i in range(len(X[0]))]\n",
+                "            for j in range(sample_population)\n",
+                "        ]\n",
+                "    )\n",
                 "    Xsamples = Xsamples.reshape(len(Xsamples), len(X[0]))\n",
                 "    # calculate the acquisition function for each sample\n",
                 "    scores = acquisition(X, Xsamples, model)\n",
                 "    # locate the index of the largest scores\n",
                 "    ix = np.argmax(scores)\n",
                 "    return Xsamples[ix]"
             ]
@@ -389,15 +412,15 @@
                 "Oqtant_model.fit(x_train, y_train)\n",
                 "\n",
                 "cost = []\n",
                 "\n",
                 "for i in range(10):\n",
                 "    # select the next point to sample\n",
                 "    x = optimize_acquisition(X, Y, Oqtant_model, 500)\n",
-                "    print('x', x)\n",
+                "    print(\"x\", x)\n",
                 "    # sample the point\n",
                 "    actual = cost_func_5D(x)\n",
                 "    cost.append(actual)\n",
                 "    # summarize the finding\n",
                 "    est, _ = surrogate(Oqtant_model, [x])\n",
                 "    print(x, est, actual)\n",
                 "    # add the data to the dataset\n",
@@ -411,23 +434,23 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# plot all samples and the final surrogate function\n",
                 "plt.plot(cost[5:])\n",
-                "#plt.yscale(\"log\")\n",
+                "# plt.yscale(\"log\")\n",
                 "plt.xlabel(\"function evaluations\")\n",
                 "plt.ylabel(\"Cost\")\n",
                 "plt.title(\"20 evaluations, 500 surrogate samples, 335pm 5_5_21\")\n",
                 "plt.savefig(\"335pm 5_5_21.png\")\n",
                 "plt.show()\n",
                 "# best result\n",
                 "ix = np.argmax(Y)\n",
-                "print('Best Result:'+str([X[ix], Y[ix]]))"
+                "print(\"Best Result:\" + str([X[ix], Y[ix]]))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
```

### Comparing `oqtant-0.16.1/documentation/walkthroughs/walkthrough_5_optimization.md` & `oqtant-0.16.2/documentation/walkthroughs/walkthrough_5_optimization.md`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from oqtant.util.auth import get_user_token
 from bert_schemas import job as JobSchema
 from oqtant.schemas.job import (
     OqtantJob,
     Gaussian_dist_2D,
     TF_dist_2D,
     bimodal_dist_2D,
-    round_sig
+    round_sig,
 )
 import csv
 
 token = get_user_token(auth_server_port=8080)
 ```
 
 ## Creating a OqtantClient Instance
@@ -86,34 +86,37 @@
                 "optical_landscape": None,
                 "lasers": None,
             },
         }
     ],
 }
 
-def cost_func_5D(RF_freqs = [17.0, 8.0, 4.0, 1.2, 0.045]): # added 5th power to default
-    base_ultracold_matter_job["inputs"][0]["values"]["rf_evaporation"]["frequencies_mhz"] = list(RF_freqs)
+
+def cost_func_5D(RF_freqs=[17.0, 8.0, 4.0, 1.2, 0.045]):  # added 5th power to default
+    base_ultracold_matter_job["inputs"][0]["values"]["rf_evaporation"][
+        "frequencies_mhz"
+    ] = list(RF_freqs)
     print(base_ultracold_matter_job)
     job = oqtant_client.generate_oqtant_job(job=base_ultracold_matter_job)
     [job_id] = oqtant_client.run_jobs(job_list=[job], track_status=True)
     job_output = oqtant_client.active_jobs[job_id].inputs[0].output.values
     Nth = job_output.thermal_atom_number
     T = job_output.temperature_uk
     Nc = job_output.condensed_atom_number
-    C = (Nth*T)/Nc
+    C = (Nth * T) / Nc
     costs_5D.append(C)
     return C
 ```
 
 ## Set bounds for optimization
 
 Bounds will prevent invalid jobs parameters from being submitted to the Oraqle.
 
 ```python
-bnds_5d = ((0,50),(0,50),(0,50),(0,50),(0,50))
+bnds_5d = ((0, 50), (0, 50), (0, 50), (0, 50), (0, 50))
 ```
 
 ## Choose an optimization algorithm
 
 Here, I chose a truncated Newton method (TNC). TNC uses a truncated Newton algorithm to minimize a function with variables subject to bounds. Within scipy.optimize.minimize there are several options for optimizers which allow for bounded variables:
 
 - L-BFGS-B
@@ -122,15 +125,21 @@
 - SLSQP
 
 ## Provide initial conditions and max iterations
 
 I chose the Oraqle web application's default parameters for a mixed cloud for the x0 initial conditions. Specify iterations with **options={'maxiter':10}**. Note that each iteration may involve several evaluations of the cost function (which means several jobs), so setting **'maxiter':30** will not run within a single 24 hour period.
 
 ```python
-res_5d = minimize(cost_func_5D, method="TNC", bounds=bnds_5d, x0 = [17,8,4,1.2,0.05], options={'maxiter':10})
+res_5d = minimize(
+    cost_func_5D,
+    method="TNC",
+    bounds=bnds_5d,
+    x0=[17, 8, 4, 1.2, 0.05],
+    options={"maxiter": 10},
+)
 
 print("optimization results freq tuning:")
 print(res_5d)
 ```
 
 ## Bayesian Optimization with a Gaussian Process model
 
@@ -142,15 +151,15 @@
 y_train : array-like of shape (n_samples,) or (n_samples, n_targets)
 Target values in training data (also required for prediction)
 
 ## Define a new target cost function
 
 ```python
 def cost(Nc, Nth, T):
-    C = (Nth*T)/Nc
+    C = (Nth * T) / Nc
     return C
 ```
 
 The optimization jobs run above will now be included in your list of currently active OqtantJobs:
 
 ```python
 oqtant_client.see_active_jobs()
@@ -164,15 +173,14 @@
     output = job.inputs[0].output.values
     condensed_atom_number = output.condensed_atom_number
     thermal_atom_number = output.thermal_atom_number
     temperature_uk = output.temperature_uk
     input = job.inputs[0].values
     x_train.append(input.rf_evaporation.frequencies_mhz)
     y_train.append(cost(condensed_atom_number, thermal_atom_number, temperature_uk))
-
 ```
 
 ```python
 # surrogate or approximation for the objective function
 def surrogate(model, X):
     # catch any warning generated when making a prediction
     with catch_warnings():
@@ -204,43 +212,58 @@
 ```python
 def acquisition(X, Xsamples, model):
     # calculate the best surrogate score found so far
     yhat, _ = surrogate(model, X)
     best = max(yhat)
     # calculate mean and stdev via surrogate function
     mu, std = surrogate(model, Xsamples)
-    #mu = mu[:, 0]
+    # mu = mu[:, 0]
     # calculate the probability of improvement
-    probs = norm.cdf((mu - best) / (std+1E-9))
+    probs = norm.cdf((mu - best) / (std + 1e-9))
     return probs
 ```
 
 ## Define a domain
 
 This is the domain of the samples. This one point where we inject prior knowledge of the system from previous experience
 
 ```python
-domain = [(20.,15.),(12.,5.),(5.,2.),(1.9,0.2),(0.2,0.01),
-          (500.,470.),(470.,460.),(459.,420.),(420.,350.)]
+domain = [
+    (20.0, 15.0),
+    (12.0, 5.0),
+    (5.0, 2.0),
+    (1.9, 0.2),
+    (0.2, 0.01),
+    (500.0, 470.0),
+    (470.0, 460.0),
+    (459.0, 420.0),
+    (420.0, 350.0),
+]
+
 
 def rand_domain_sample(domain):
-    scale = domain[0]-domain[1]
-    random_number = np.random.uniform()+(1E-9)
-    sample = scale*random_number+domain[1]
+    scale = domain[0] - domain[1]
+    random_number = np.random.uniform() + (1e-9)
+    sample = scale * random_number + domain[1]
     return sample
 ```
 
 ## Define an optimizer on the acquisition function
 
 Here I have chosen a random search over the domain, but other search algorithms can be used.
 
 ```python
 def optimize_acquisition(X, y, model, sample_population):
     # random search, generate random samples
-    Xsamples = np.asarray([[rand_domain_sample(domain[i]) for i in range(len(X[0]))] for j in range(sample_population)])
+    Xsamples = np.asarray(
+        [
+            [rand_domain_sample(domain[i]) for i in range(len(X[0]))]
+            for j in range(sample_population)
+        ]
+    )
     Xsamples = Xsamples.reshape(len(Xsamples), len(X[0]))
     # calculate the acquisition function for each sample
     scores = acquisition(X, Xsamples, model)
     # locate the index of the largest scores
     ix = np.argmax(scores)
     return Xsamples[ix]
 ```
@@ -254,15 +277,15 @@
 Oqtant_model.fit(x_train, y_train)
 
 cost = []
 
 for i in range(10):
     # select the next point to sample
     x = optimize_acquisition(X, Y, Oqtant_model, 500)
-    print('x', x)
+    print("x", x)
     # sample the point
     actual = cost_func_5D(x)
     cost.append(actual)
     # summarize the finding
     est, _ = surrogate(Oqtant_model, [x])
     print(x, est, actual)
     # add the data to the dataset
@@ -271,21 +294,17 @@
     # update the model
     Oqtant_model.fit(X, Y)
 ```
 
 ```python
 # plot all samples and the final surrogate function
 plt.plot(cost[5:])
-#plt.yscale("log")
+# plt.yscale("log")
 plt.xlabel("function evaluations")
 plt.ylabel("Cost")
 plt.title("20 evaluations, 500 surrogate samples, 335pm 5_5_21")
 plt.savefig("335pm 5_5_21.png")
 plt.show()
 # best result
 ix = np.argmax(Y)
-print('Best Result:'+str([X[ix], Y[ix]]))
-```
-
-```python
-
+print("Best Result:" + str([X[ix], Y[ix]]))
 ```
```

### Comparing `oqtant-0.16.1/documentation/walkthroughs/walkthroughs.md` & `oqtant-0.16.2/documentation/walkthroughs/walkthroughs.md`

 * *Files identical despite different names*

### Comparing `oqtant-0.16.1/oqtant/oqtant_client.py` & `oqtant-0.16.2/oqtant/oqtant_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2023 Infleqtion
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import json
 import os
 import sys
 import time
 import warnings
 from importlib.metadata import version
```

### Comparing `oqtant-0.16.1/oqtant/schemas/job.py` & `oqtant-0.16.2/oqtant/schemas/job.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+# Copyright 2023 Infleqtion
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from datetime import datetime
 from math import floor, log10, pi
 from uuid import UUID
 
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy.optimize as opt
```

### Comparing `oqtant-0.16.1/pyproject.toml` & `oqtant-0.16.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oqtant"
-version = "0.16.1"
+version = "0.16.2"
 description = "Oqtant Desktop Suite"
 authors = [
   "Larry Buza <lawrence.buza@coldquanta.com>",
   "Hannah North <hannah.north@coldquanta.com>",
   "Mike McGrath <michael.mcgrath@coldquanta.com>",
 ]
 license = "Apache-2.0"
@@ -50,15 +50,15 @@
 pytest-xdist = "^3.2.0"
 pytest-ordering = "^0.6"
 pytest-cov = "^4.0.0"
 pycodestyle = "^2.10.0"
 flake8 = "^6.0.0"
 lxml = "^4.9.1"
 mypy = "^1.0.0"
-black = "^23.1.0"
+black = {extras = ["jupyter"], version = "^23.7.0"}
 pre-commit = "^3.0.4"
 ipython = "^8.4.0"
 pydantic-factories = "^1.6.1"
 email-validator = "^1.2.1"
 isort = "^5.12.0"
 nbstripout = "^0.6.1"
 
@@ -77,15 +77,14 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 88
-include = '\.pyi?$'
 extend-exclude = '''
 /(
   # The following are specific to Black, you probably don't want those.
   | blib2to3
   | tests/data
   | profiling
 )/
```

### Comparing `oqtant-0.16.1/setup.py` & `oqtant-0.16.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 entry_points = \
 {'console_scripts': ['authorize = '
                      'oqtant.tests.integration.authorize:authorize']}
 
 setup_kwargs = {
     'name': 'oqtant',
-    'version': '0.16.1',
+    'version': '0.16.2',
     'description': 'Oqtant Desktop Suite',
     'long_description': "# Oqtant\n\n[![License: Apache](https://img.shields.io/badge/License-Apache-yellow.svg)](https://opensource.org/licenses/Apache-2.0)\n[![pypi](https://img.shields.io/pypi/v/oqtant.svg)](https://pypi.python.org/pypi/oqtant)\n[![versions](https://img.shields.io/pypi/pyversions/bert-schemas.svg)](https://pypi.python.org/pypi/bert-schemas)\n[![Twitter](https://img.shields.io/twitter/url/https/twitter.com/Infleqtion.svg?style=social&label=Follow%20%40Infleqtion)](https://twitter.com/Infleqtion)\n\n## 🚀 Quick Install\n\n```python\npip install oqtant\n```\n\n## 🧭 Introduction\n\nThis API contains tools to:\n\n- Access all the functionality of the Oraqle Web App (https://albert-dev.coldquanta.com)\n\n  - BARRIER (Barrier Manipulator) jobs\n  - BEC (Ultracold Matter) jobs\n\n- Build parameterized (i.e. optimization) experiments using OqtantJobs\n\n- Submit and retrieve OqtantJob results\n\n## 🤖 How Oqtant Works\n\n- Construct a single or list of jobs using the OqtantJob class\n\n  - 1D parameter sweeps are supported\n\n- Run a single or list of jobs using run_jobs(). The jobs are submitted to run on hardware in FIFO queue.\n\n  - job lists are run sequentially (uninterrupted) unless list exceeds 30 jobs\n\n- As jobs run, OqtantJob objects are created automatically and stored in active_jobs.\n\n  - View these jobs with see_active_jobs()\n  - These jobs are available until the python session ends.\n\n- To operate on jobs from a current or previous session, load them into active_jobs with\n\n  - load_job_from_id(), load_job_from_id_list(), load_job_from_file(), load_job_from_file_list()\n\n- To analyze job objects and use Oqtant's job analysis library, reference the OqtantJob class documentation.\n\nNeed help? Found a bug? Contact <albert@infleqtion.com> for support. Thank you!\n\n## 📓 Documentation\n\n- [Getting started](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/INSTALL.md) (installation, setting up the environment, how to run the walkthrough notebooks)\n- [Walkthroughs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/walkthroughs/walkthroughs.md) (demos for creating and submitting jobs)\n- [Oraqle API docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/oraqle_api_docs.md)\n- [Job Analysis docs](https://gitlab.com/infleqtion/albert/oqtant/-/blob/main/documentation/job_analysis_docs.md)\n",
     'author': 'Larry Buza',
     'author_email': 'lawrence.buza@coldquanta.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://albert-dev.coldquanta.com/',
```

### Comparing `oqtant-0.16.1/PKG-INFO` & `oqtant-0.16.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oqtant
-Version: 0.16.1
+Version: 0.16.2
 Summary: Oqtant Desktop Suite
 Home-page: https://albert-dev.coldquanta.com/
 License: Apache-2.0
 Author: Larry Buza
 Author-email: lawrence.buza@coldquanta.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
```


# Comparing `tmp/sleepeeg-0.3.2.tar.gz` & `tmp/sleepeeg-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepeeg-0.3.2.tar", last modified: Fri Jul  7 12:13:45 2023, max compression
+gzip compressed data, was "sleepeeg-0.3.3.tar", last modified: Mon Jul 24 14:48:49 2023, max compression
```

## Comparing `sleepeeg-0.3.2.tar` & `sleepeeg-0.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 12:13:45.069857 sleepeeg-0.3.2/
--rw-rw-rw-   0        0        0     1088 2023-03-20 20:54:05.000000 sleepeeg-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     1728 2023-07-07 12:13:45.069857 sleepeeg-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     1306 2023-06-09 12:52:22.000000 sleepeeg-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 12:13:45.035898 sleepeeg-0.3.2/docs/
--rw-rw-rw-   0        0        0     2433 2023-06-24 10:09:30.000000 sleepeeg-0.3.2/docs/conf.py
--rw-rw-rw-   0        0        0      839 2023-07-07 12:10:05.000000 sleepeeg-0.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-07 12:13:45.070804 sleepeeg-0.3.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-07 12:13:45.049894 sleepeeg-0.3.2/sleepeeg/
--rw-rw-rw-   0        0        0    48389 2023-06-28 12:51:11.000000 sleepeeg-0.3.2/sleepeeg/base.py
--rw-rw-rw-   0        0        0    12432 2023-07-07 11:38:44.000000 sleepeeg-0.3.2/sleepeeg/dashboard.py
--rw-rw-rw-   0        0        0    28533 2023-07-07 12:11:25.000000 sleepeeg-0.3.2/sleepeeg/pipeline.py
--rw-rw-rw-   0        0        0     2005 2023-06-24 08:52:40.000000 sleepeeg-0.3.2/sleepeeg/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-07 12:13:45.067844 sleepeeg-0.3.2/sleepeeg.egg-info/
--rw-rw-rw-   0        0        0     1728 2023-07-07 12:13:45.000000 sleepeeg-0.3.2/sleepeeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-07-07 12:13:45.000000 sleepeeg-0.3.2/sleepeeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 12:13:45.000000 sleepeeg-0.3.2/sleepeeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      118 2023-07-07 12:13:45.000000 sleepeeg-0.3.2/sleepeeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-07-07 12:13:45.000000 sleepeeg-0.3.2/sleepeeg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-24 14:48:49.947439 sleepeeg-0.3.3/
+-rw-rw-rw-   0        0        0     1088 2023-03-20 20:54:05.000000 sleepeeg-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0     1728 2023-07-24 14:48:49.946442 sleepeeg-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1306 2023-06-09 12:52:22.000000 sleepeeg-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-24 14:48:49.900565 sleepeeg-0.3.3/docs/
+-rw-rw-rw-   0        0        0     2433 2023-06-24 10:09:30.000000 sleepeeg-0.3.3/docs/conf.py
+-rw-rw-rw-   0        0        0      839 2023-07-24 14:47:33.000000 sleepeeg-0.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-24 14:48:49.947439 sleepeeg-0.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-24 14:48:49.925498 sleepeeg-0.3.3/sleepeeg/
+-rw-rw-rw-   0        0        0    49018 2023-07-24 14:22:26.000000 sleepeeg-0.3.3/sleepeeg/base.py
+-rw-rw-rw-   0        0        0    12430 2023-07-08 15:03:21.000000 sleepeeg-0.3.3/sleepeeg/dashboard.py
+-rw-rw-rw-   0        0        0    28552 2023-07-24 14:24:50.000000 sleepeeg-0.3.3/sleepeeg/pipeline.py
+-rw-rw-rw-   0        0        0     2005 2023-06-24 08:52:40.000000 sleepeeg-0.3.3/sleepeeg/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-24 14:48:49.944448 sleepeeg-0.3.3/sleepeeg.egg-info/
+-rw-rw-rw-   0        0        0     1728 2023-07-24 14:48:49.000000 sleepeeg-0.3.3/sleepeeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-07-24 14:48:49.000000 sleepeeg-0.3.3/sleepeeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-24 14:48:49.000000 sleepeeg-0.3.3/sleepeeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      118 2023-07-24 14:48:49.000000 sleepeeg-0.3.3/sleepeeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-24 14:48:49.000000 sleepeeg-0.3.3/sleepeeg.egg-info/top_level.txt
```

### Comparing `sleepeeg-0.3.2/LICENSE` & `sleepeeg-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sleepeeg-0.3.2/PKG-INFO` & `sleepeeg-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepeeg
-Version: 0.3.2
+Version: 0.3.3
 Summary: Sleep EEG preprocessing and analysis
 Author-email: Gennadiy Belonosov <gennadiyb@mail.tau.ac.il>
 License: MIT
 Project-URL: Homepage, https://github.com/NirLab-TAU/sleepeeg
 Project-URL: Documentation, https://nirlab-tau.github.io/sleepeeg/
 Keywords: sleep,eeg
 Requires-Python: >=3.10
```

### Comparing `sleepeeg-0.3.2/README.md` & `sleepeeg-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `sleepeeg-0.3.2/docs/conf.py` & `sleepeeg-0.3.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sleepeeg-0.3.2/pyproject.toml` & `sleepeeg-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 exclude = ["notebooks"]  # empty by default
 
 [project]
 name = "sleepeeg"
-version = "0.3.2"
+version = "0.3.3"
 authors = [
     {name = "Gennadiy Belonosov", email = "gennadiyb@mail.tau.ac.il"},
 ]
 description = "Sleep EEG preprocessing and analysis"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "MIT"}
```

### Comparing `sleepeeg-0.3.2/sleepeeg/base.py` & `sleepeeg-0.3.3/sleepeeg/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,45 +137,64 @@
             save_bad_channels: Whether to save bad channels as txt. Defaults to False.
             overwrite: Whether to overwrite annotations and bad_channels files if exist.
                 Defaults to False.
             **kwargs: Arguments passed to :py:meth:`mne:mne.io.Raw.plot`.
         """
         kwargs.setdefault("theme", "dark")
         kwargs.setdefault("bad_color", "r")
-        kwargs.setdefault("scalings", "auto")
         kwargs["block"] = True
 
         self.mne_raw.plot(**kwargs)
 
         if save_annotations:
-            self.mne_raw.annotations.save(
-                self.output_dir / self.__class__.__name__ / "annotations.txt",
-                overwrite=overwrite,
-            )
+            self.save_annotations(overwrite=overwrite)
 
         if save_bad_channels:
-            new_bads = self.mne_raw.info["bads"]
+            self.save_bad_channels(overwrite=overwrite)
 
-            if new_bads:
-                from natsort import natsorted
+    def save_bad_channels(self, overwrite=False):
+        """Adds bad channels from info["bads"] to the "bad_channels.txt" file.
 
-                fpath = self.output_dir / self.__class__.__name__ / "bad_channels.txt"
-                old_bads = []
-                if fpath.exists():
-                    with open(fpath, "r") as f:
-                        old_bads = f.read().split()
-
-                with open(fpath, "w") as f:
-                    bads = (
-                        natsorted(new_bads)
-                        if overwrite
-                        else natsorted(set(old_bads + new_bads))
-                    )
-                    for bad in bads:
-                        f.write(f"{bad}\n")
+        Args:
+            overwrite: Whether to overwrite the file if exists.
+                If False will add unique new channels to the file.
+                Defaults to False.
+        """
+        new_bads = self.mne_raw.info["bads"]
+
+        if new_bads:
+            from natsort import natsorted
+
+            fpath = self.output_dir / self.__class__.__name__ / "bad_channels.txt"
+            old_bads = []
+            if fpath.exists():
+                with open(fpath, "r") as f:
+                    old_bads = f.read().split()
+
+            with open(fpath, "w") as f:
+                bads = (
+                    natsorted(new_bads)
+                    if overwrite
+                    else natsorted(set(old_bads + new_bads))
+                )
+                for bad in bads:
+                    f.write(f"{bad}\n")
+
+    def save_annotations(self, overwrite=False):
+        """Writes annotations to "annotations.txt" file.
+
+        Args:
+            overwrite: Whether to overwrite the file if exists.
+                If False and the file exists will throw an exception.
+                Defaults to False.
+        """
+        self.mne_raw.annotations.save(
+            self.output_dir / self.__class__.__name__ / "annotations.txt",
+            overwrite=overwrite,
+        )
 
     def plot_sensors(
         self, legend: Iterable[str] = None, legend_args: dict = None, **kwargs
     ):
         """A wrapper for :py:func:`mne:mne.viz.plot_sensors` with a legend.
 
         Args:
@@ -1139,15 +1158,15 @@
 
         if save:
             fig.savefig(
                 self.output_dir / self.__class__.__name__ / f"topomap_psd_collage.png"
             )
 
     @logger_wraps()
-    def _save_psds(self, overwrite):
+    def save_psds(self, overwrite):
         import re
 
         for stage, spectrum in self.psds.items():
             stage = re.sub(r"[^\w\s-]", "_", stage)
             spectrum.save(
                 self.output_dir / self.__class__.__name__ / f"{stage}-psd.h5",
                 overwrite=overwrite,
```

### Comparing `sleepeeg-0.3.2/sleepeeg/dashboard.py` & `sleepeeg-0.3.3/sleepeeg/dashboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,25 +282,24 @@
     sfreq, fmin, fmax, notch_freqs = _filter(
         pipe,
         resampling_freq,
         bandpass_filter_freqs[0],
         bandpass_filter_freqs[1],
     )
 
-    pipe.set_eeg_reference(ref_channels=ref_channels)
-
     if path_to_bad_channels is not None:
         pipe.read_bad_channels(path=path_to_bad_channels)
         bads = pipe.mne_raw.info["bads"]
         pipe.interpolate_bads(reset_bads=True)
     else:
         from ast import literal_eval
 
         bads = literal_eval(pipe.mne_raw.info["description"])
 
+    pipe.set_eeg_reference(ref_channels=ref_channels)
     s_pipe, sleep_stages = _init_s_pipe(pipe, path_to_hypnogram, hypno_freq)
     min_psd, max_psd = _hypno_psd(
         s_pipe,
         sleep_stages,
         hypno_psd_pick,
         hypno_before,
         psd_before,
```

### Comparing `sleepeeg-0.3.2/sleepeeg/pipeline.py` & `sleepeeg-0.3.3/sleepeeg/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,23 +218,23 @@
             filtered_raw.filter(**filter_kwargs)
         else:
             filtered_raw = self.mne_raw
         self.mne_ica.fit(filtered_raw, **fit_kwargs)
 
     def plot_sources(self, **kwargs):
         """A wrapper for :py:meth:`mne:mne.preprocessing.ICA.plot_sources`."""
-        self.mne_ica.plot_sources(inst=self.mne_raw, **kwargs)
+        return self.mne_ica.plot_sources(inst=self.mne_raw, **kwargs)
 
     def plot_components(self, **kwargs):
         """A wrapper for :py:meth:`mne:mne.preprocessing.ICA.plot_components`."""
-        self.mne_ica.plot_components(inst=self.mne_raw, **kwargs)
+        return self.mne_ica.plot_components(inst=self.mne_raw, **kwargs)
 
     def plot_properties(self, picks=None, **kwargs):
         """A wrapper for :py:meth:`mne:mne.preprocessing.ICA.plot_properties`."""
-        self.mne_ica.plot_properties(self.mne_raw, picks=picks, **kwargs)
+        return self.mne_ica.plot_properties(self.mne_raw, picks=picks, **kwargs)
 
     @logger_wraps()
     def apply(self, exclude=None, **kwargs):
         """A wrapper for :py:meth:`mne:mne.preprocessing.ICA.apply`."""
         logger.info(
             f"Excluded ICA components: {list(set((exclude or [])+(self.mne_ica.exclude or [])))}"
         )
@@ -317,15 +317,15 @@
                 proj=False,
                 reject_by_annotation=reject_by_annotation,
                 n_jobs=n_jobs,
                 verbose=verbose,
                 **psd_kwargs,
             )
         if save:
-            self._save_psds(overwrite)
+            self.save_psds(overwrite)
 
     @logger_wraps()
     def read_spectra(self, dirpath: str | None = None):
         """Loads spectra stored in hdf5 files.
 
         Filenames should end with {sleep_stage}-psd.h5
 
@@ -736,8 +736,8 @@
             )
 
         for stage in sleep_stages:
             spectra = [pipe.psds[stage] for pipe in self.pipes]
             self.psds[stage] = avg_func(spectra, axis=0)
 
         if save:
-            self._save_psds(overwrite)
+            self.save_psds(overwrite)
```

### Comparing `sleepeeg-0.3.2/sleepeeg/utils.py` & `sleepeeg-0.3.3/sleepeeg/utils.py`

 * *Files identical despite different names*

### Comparing `sleepeeg-0.3.2/sleepeeg.egg-info/PKG-INFO` & `sleepeeg-0.3.3/sleepeeg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepeeg
-Version: 0.3.2
+Version: 0.3.3
 Summary: Sleep EEG preprocessing and analysis
 Author-email: Gennadiy Belonosov <gennadiyb@mail.tau.ac.il>
 License: MIT
 Project-URL: Homepage, https://github.com/NirLab-TAU/sleepeeg
 Project-URL: Documentation, https://nirlab-tau.github.io/sleepeeg/
 Keywords: sleep,eeg
 Requires-Python: >=3.10
```


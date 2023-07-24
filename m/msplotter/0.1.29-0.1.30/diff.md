# Comparing `tmp/msplotter-0.1.29.tar.gz` & `tmp/msplotter-0.1.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msplotter-0.1.29.tar", last modified: Thu Jul 20 07:20:10 2023, max compression
+gzip compressed data, was "msplotter-0.1.30.tar", last modified: Mon Jul 24 18:43:42 2023, max compression
```

## Comparing `msplotter-0.1.29.tar` & `msplotter-0.1.30.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-20 07:20:10.029296 msplotter-0.1.29/
--rw-r--r--   0 msp        (501) staff       (20)     1507 2023-01-12 04:50:28.000000 msplotter-0.1.29/LICENSE
--rw-r--r--   0 msp        (501) staff       (20)     5234 2023-07-20 07:20:10.028766 msplotter-0.1.29/PKG-INFO
--rw-r--r--   0 msp        (501) staff       (20)     4544 2023-06-08 15:44:32.000000 msplotter-0.1.29/README.md
--rw-r--r--   0 msp        (501) staff       (20)      961 2023-07-20 03:20:31.000000 msplotter-0.1.29/pyproject.toml
--rw-r--r--   0 msp        (501) staff       (20)       38 2023-07-20 07:20:10.029449 msplotter-0.1.29/setup.cfg
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-20 07:20:09.994495 msplotter-0.1.29/src/
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-20 07:20:10.005948 msplotter-0.1.29/src/msp/
--rw-r--r--   0 msp        (501) staff       (20)        0 2023-06-04 02:01:52.000000 msplotter-0.1.29/src/msp/__init__.py
--rw-r--r--   0 msp        (501) staff       (20)      431 2023-06-06 20:35:01.000000 msplotter-0.1.29/src/msp/__main__.py
--rw-r--r--   0 msp        (501) staff       (20)     5859 2023-06-04 00:27:56.000000 msplotter-0.1.29/src/msp/arrows.py
--rw-r--r--   0 msp        (501) staff       (20)     5096 2023-06-04 02:40:56.000000 msplotter-0.1.29/src/msp/colormap_picker.py
--rw-r--r--   0 msp        (501) staff       (20)    14508 2023-07-16 23:44:54.000000 msplotter-0.1.29/src/msp/gui.py
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-20 07:20:10.019673 msplotter-0.1.29/src/msp/images/
--rw-r--r--   0 msp        (501) staff       (20)      560 2023-03-28 02:55:33.000000 msplotter-0.1.29/src/msp/images/Blues.png
--rw-------   0 msp        (501) staff       (20)      614 2023-03-24 21:28:57.000000 msplotter-0.1.29/src/msp/images/BuGn.png
--rw-------   0 msp        (501) staff       (20)      593 2023-03-24 21:28:57.000000 msplotter-0.1.29/src/msp/images/BuPu.png
--rw-------   0 msp        (501) staff       (20)      617 2023-03-24 21:28:57.000000 msplotter-0.1.29/src/msp/images/GnBu.png
--rw-------   0 msp        (501) staff       (20)      575 2023-03-24 21:28:57.000000 msplotter-0.1.29/src/msp/images/Greens.png
--rw-------   0 msp        (501) staff       (20)      453 2023-03-24 21:28:57.000000 msplotter-0.1.29/src/msp/images/Greys.png
--rw-------   0 msp        (501) staff       (20)      592 2023-03-24 21:28:57.000000 msplotter-0.1.29/src/msp/images/OrRd.png
--rw-------   0 msp        (501) staff       (20)      569 2023-03-24 21:28:57.000000 msplotter-0.1.29/src/msp/images/Oranges.png
--rw-------   0 msp        (501) staff       (20)      591 2023-03-24 21:28:57.000000 msplotter-0.1.29/src/msp/images/PuBu.png
--rw-------   0 msp        (501) staff       (20)      609 2023-03-24 21:28:57.000000 msplotter-0.1.29/src/msp/images/PuBuGn.png
--rw-------   0 msp        (501) staff       (20)      662 2023-03-24 21:28:57.000000 msplotter-0.1.29/src/msp/images/PuRd.png
--rw-------   0 msp        (501) staff       (20)      557 2023-03-24 21:28:57.000000 msplotter-0.1.29/src/msp/images/Purples.png
--rw-------   0 msp        (501) staff       (20)      621 2023-03-24 21:28:57.000000 msplotter-0.1.29/src/msp/images/RdPu.png
--rw-------   0 msp        (501) staff       (20)      587 2023-03-24 21:28:57.000000 msplotter-0.1.29/src/msp/images/Reds.png
--rw-------   0 msp        (501) staff       (20)      618 2023-03-24 21:28:57.000000 msplotter-0.1.29/src/msp/images/YlGn.png
--rw-------   0 msp        (501) staff       (20)      624 2023-03-24 21:28:57.000000 msplotter-0.1.29/src/msp/images/YlGnBu.png
--rw-------   0 msp        (501) staff       (20)      592 2023-03-24 21:28:57.000000 msplotter-0.1.29/src/msp/images/YlOrBr.png
--rw-------   0 msp        (501) staff       (20)      596 2023-03-24 21:28:57.000000 msplotter-0.1.29/src/msp/images/YlOrRd.png
--rw-------   0 msp        (501) staff       (20)    25253 2023-03-24 21:28:57.000000 msplotter-0.1.29/src/msp/images/logo.png
--rw-r--r--   0 msp        (501) staff       (20)    34541 2023-07-20 07:12:48.000000 msplotter-0.1.29/src/msp/msplotter.py
--rw-r--r--   0 msp        (501) staff       (20)     3507 2023-07-08 00:04:00.000000 msplotter-0.1.29/src/msp/plot.py
--rw-r--r--   0 msp        (501) staff       (20)     7391 2023-06-04 02:29:49.000000 msplotter-0.1.29/src/msp/slider_widget.py
--rw-r--r--   0 msp        (501) staff       (20)     2958 2023-07-17 00:23:03.000000 msplotter-0.1.29/src/msp/spinbox.py
--rw-r--r--   0 msp        (501) staff       (20)    14329 2023-07-15 21:18:20.000000 msplotter-0.1.29/src/msp/user_input.py
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-20 07:20:10.027827 msplotter-0.1.29/src/msplotter.egg-info/
--rw-r--r--   0 msp        (501) staff       (20)     5234 2023-07-20 07:20:09.000000 msplotter-0.1.29/src/msplotter.egg-info/PKG-INFO
--rw-r--r--   0 msp        (501) staff       (20)      933 2023-07-20 07:20:09.000000 msplotter-0.1.29/src/msplotter.egg-info/SOURCES.txt
--rw-r--r--   0 msp        (501) staff       (20)        1 2023-07-20 07:20:09.000000 msplotter-0.1.29/src/msplotter.egg-info/dependency_links.txt
--rw-r--r--   0 msp        (501) staff       (20)       48 2023-07-20 07:20:09.000000 msplotter-0.1.29/src/msplotter.egg-info/entry_points.txt
--rw-r--r--   0 msp        (501) staff       (20)       55 2023-07-20 07:20:09.000000 msplotter-0.1.29/src/msplotter.egg-info/requires.txt
--rw-r--r--   0 msp        (501) staff       (20)        4 2023-07-20 07:20:09.000000 msplotter-0.1.29/src/msplotter.egg-info/top_level.txt
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-24 18:43:42.851086 msplotter-0.1.30/
+-rw-r--r--   0 msp        (501) staff       (20)     1507 2023-01-12 04:50:28.000000 msplotter-0.1.30/LICENSE
+-rw-r--r--   0 msp        (501) staff       (20)     4813 2023-07-24 18:43:42.850517 msplotter-0.1.30/PKG-INFO
+-rw-r--r--   0 msp        (501) staff       (20)     4123 2023-07-22 19:56:11.000000 msplotter-0.1.30/README.md
+-rw-r--r--   0 msp        (501) staff       (20)      961 2023-07-22 00:36:53.000000 msplotter-0.1.30/pyproject.toml
+-rw-r--r--   0 msp        (501) staff       (20)       38 2023-07-24 18:43:42.851261 msplotter-0.1.30/setup.cfg
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-24 18:43:42.808425 msplotter-0.1.30/src/
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-24 18:43:42.825260 msplotter-0.1.30/src/msp/
+-rw-r--r--   0 msp        (501) staff       (20)        0 2023-06-04 02:01:52.000000 msplotter-0.1.30/src/msp/__init__.py
+-rw-r--r--   0 msp        (501) staff       (20)      431 2023-06-06 20:35:01.000000 msplotter-0.1.30/src/msp/__main__.py
+-rw-r--r--   0 msp        (501) staff       (20)     5859 2023-06-04 00:27:56.000000 msplotter-0.1.30/src/msp/arrows.py
+-rw-r--r--   0 msp        (501) staff       (20)     5096 2023-06-04 02:40:56.000000 msplotter-0.1.30/src/msp/colormap_picker.py
+-rw-r--r--   0 msp        (501) staff       (20)    19061 2023-07-24 05:29:03.000000 msplotter-0.1.30/src/msp/gui.py
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-24 18:43:42.846279 msplotter-0.1.30/src/msp/images/
+-rw-r--r--   0 msp        (501) staff       (20)      560 2023-03-28 02:55:33.000000 msplotter-0.1.30/src/msp/images/Blues.png
+-rw-------   0 msp        (501) staff       (20)      614 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/BuGn.png
+-rw-------   0 msp        (501) staff       (20)      593 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/BuPu.png
+-rw-------   0 msp        (501) staff       (20)      617 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/GnBu.png
+-rw-------   0 msp        (501) staff       (20)      575 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/Greens.png
+-rw-------   0 msp        (501) staff       (20)      453 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/Greys.png
+-rw-r--r--   0 msp        (501) staff       (20)   353491 2023-07-22 04:33:21.000000 msplotter-0.1.30/src/msp/images/MSPlotter_gui.png
+-rw-------   0 msp        (501) staff       (20)      592 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/OrRd.png
+-rw-------   0 msp        (501) staff       (20)      569 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/Oranges.png
+-rw-------   0 msp        (501) staff       (20)      591 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/PuBu.png
+-rw-------   0 msp        (501) staff       (20)      609 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/PuBuGn.png
+-rw-------   0 msp        (501) staff       (20)      662 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/PuRd.png
+-rw-------   0 msp        (501) staff       (20)      557 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/Purples.png
+-rw-------   0 msp        (501) staff       (20)      621 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/RdPu.png
+-rw-------   0 msp        (501) staff       (20)      587 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/Reds.png
+-rw-------   0 msp        (501) staff       (20)      618 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/YlGn.png
+-rw-------   0 msp        (501) staff       (20)      624 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/YlGnBu.png
+-rw-------   0 msp        (501) staff       (20)      592 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/YlOrBr.png
+-rw-------   0 msp        (501) staff       (20)      596 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/YlOrRd.png
+-rw-------   0 msp        (501) staff       (20)    25253 2023-03-24 21:28:57.000000 msplotter-0.1.30/src/msp/images/logo.png
+-rw-r--r--   0 msp        (501) staff       (20)    36197 2023-07-24 05:39:10.000000 msplotter-0.1.30/src/msp/msplotter.py
+-rw-r--r--   0 msp        (501) staff       (20)     3507 2023-07-08 00:04:00.000000 msplotter-0.1.30/src/msp/plot.py
+-rw-r--r--   0 msp        (501) staff       (20)     7391 2023-06-04 02:29:49.000000 msplotter-0.1.30/src/msp/slider_widget.py
+-rw-r--r--   0 msp        (501) staff       (20)     2958 2023-07-17 00:23:03.000000 msplotter-0.1.30/src/msp/spinbox.py
+-rw-r--r--   0 msp        (501) staff       (20)    14329 2023-07-15 21:18:20.000000 msplotter-0.1.30/src/msp/user_input.py
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-24 18:43:42.849731 msplotter-0.1.30/src/msplotter.egg-info/
+-rw-r--r--   0 msp        (501) staff       (20)     4813 2023-07-24 18:43:42.000000 msplotter-0.1.30/src/msplotter.egg-info/PKG-INFO
+-rw-r--r--   0 msp        (501) staff       (20)      966 2023-07-24 18:43:42.000000 msplotter-0.1.30/src/msplotter.egg-info/SOURCES.txt
+-rw-r--r--   0 msp        (501) staff       (20)        1 2023-07-24 18:43:42.000000 msplotter-0.1.30/src/msplotter.egg-info/dependency_links.txt
+-rw-r--r--   0 msp        (501) staff       (20)       48 2023-07-24 18:43:42.000000 msplotter-0.1.30/src/msplotter.egg-info/entry_points.txt
+-rw-r--r--   0 msp        (501) staff       (20)       55 2023-07-24 18:43:42.000000 msplotter-0.1.30/src/msplotter.egg-info/requires.txt
+-rw-r--r--   0 msp        (501) staff       (20)        4 2023-07-24 18:43:42.000000 msplotter-0.1.30/src/msplotter.egg-info/top_level.txt
```

### Comparing `msplotter-0.1.29/LICENSE` & `msplotter-0.1.30/LICENSE`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.29/PKG-INFO` & `msplotter-0.1.30/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msplotter
-Version: 0.1.29
+Version: 0.1.30
 Summary: Make a graphical representation of a blastn alignment
 Author-email: Ivan Muñoz-Gutierrez <ivan.munoz.gutierrez@gmail.com>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/ivanmugu/MSPlotter
 Keywords: blast,alignment,graphical representation,DNA sequence,easyfig
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
@@ -15,55 +15,81 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
    <img src="./src/msp/images/logo.png" alt="MSPlotter" width="350">
 </p>
 
-# Make a graphical representation of a blantn alignment
+# Make a graphical representation of a blastn alignment
 
 Multiple Sequence Plotter (MSPlotter) uses GenBank files (.gb) to align the
-sequences and plot the genes. To plot the genes, MSPlotter uses the information
-from the `CDS` features section. To customize the colors for plotting genes,
-you can add a `Color` tag in the `CDS` features with a color in hexadecimal.
-For example, to show a gene in green add the tag `/Color="#00ff00"`. To avoid
-direct the manual manipulation of the GenBank file, you can edit the file with
+sequences and plot the genes. MSPlotter uses the information from the `CDS`
+features section to plot the genes. To customize the colors for plotting genes,
+you can add a `Color` tag in the `CDS` features with color in hexadecimal.
+For example, add the tag `/Color="#00ff00"` to show a gene in green. To avoid
+direct manual manipulation of the GenBank file, you can edit the file with
 `Geneious` or another software and export the file with the new annotations.
 
-MSPlotter uses `matplotlib`. Therefore, to customize your figure, you can
-modify the parameters in the `MakeFigure` class of the `msplotter` module.
+MSPlotter is an easy-to-use option for people with little coding knowledge or
+problems running the classic app `easyfig`. The program offers a graphical user
+interface (GUI) and a command line interface (CLI).
+
+If the user knows Python, MSPlotter uses `matplotlib`. Therefore, to customize
+your figure, the user can modify the parameters in the `MakeFigure` class of
+the `msplotter` module or make any necessary change in any part of the code.
+
+I am developing MSPlotter in my free time, therefore, if you find a bug, it may
+take me some time to fix it, but I will try to do my best to fix the problems
+as soon as possible. Also, if you have any suggestions, let me know, and I will
+try to implement them.
 
 ## Requirements
 
 - [Python](https://www.python.org/) 3.11 or later
 - [biopython](https://biopython.org/) 1.81 or later
 - [customtkinter](https://customtkinter.tomschimansky.com/) 5.1 or later
 - [matplotlib](https://matplotlib.org/) 3.7 or later
-- [blastn](https://www.ncbi.nlm.nih.gov/books/NBK569861/) must be installed locally and in the path
+- [blastn](https://www.ncbi.nlm.nih.gov/books/NBK569861/) must be installed
+  locally and in the path
+
+MSPlotter has been tested in macOS and Windows.
 
 ## Installation
 
-Create a virtual environment and install msplotter using pip as follows:
+First, create a virtual environment with `conda` or `venv`. Then, install
+msplotter using pip as follows:
 
 ```bash
 pip install msplotter
 ```
 
 ## Usage and options
 
+To run the GUI type:
+
+```bash
+msplotter --gui
+```
+
+Output GUI:
+
+<p align="center">
+   <img src="./src/msp/images/MSPlotter_gui.png" alt="MSPlotter" width="350">
+</p>
+
 To view all the options run:
 
 ```bash
 msplotter --help
 ```
 
-Output:
+Partial output CLI:
 
 ```console
-usage: msplotter [-h] [-v] [-i INPUT [INPUT ...]] [-o OUTPUT] [-n NAME] [-f FORMAT]
+usage: msplotter [-h] [-v] [-i INPUT [INPUT ...]] [-o OUTPUT] [-n NAME] [-f FORMAT] [-d DPI]
                  [--alignments_position ALIGNMENTS_POSITION] [--identity_color IDENTITY_COLOR]
                  [--annotate_sequences [ANNOTATE_SEQUENCES]] [--annotate_genes [ANNOTATE_GENES]] [-g]
 
 Make a graphical representation of a blastn alignment.
 
 Help:
   -h, --help            Show this help message and exit.
@@ -76,64 +102,38 @@
 Optional:
   -o OUTPUT, --output OUTPUT
                         Path to output folder.
                         Default: current working directory.
   -n NAME, --name NAME  Name of figure.
                         Default: `figure`.
   -f FORMAT, --format FORMAT
-                        Format of figure.
-                        Default: `pdf`.
-  --alignments_position ALIGNMENTS_POSITION
-                        Orientation of the alignments in the plot.
-                        Options: `left`, `center`, and `rigth`.
-                        Default: `left`.
-  --identity_color IDENTITY_COLOR
-                        Color map representing homology regions.
+                        Format of figure. Options: pdf, png, and svg.
                         For a complete list of valid options visit:
-                        https://matplotlib.org/stable/tutorials/colors/colormaps.html
-                        Some options: `Greys`, `Purples`, `Blues`, and `Oranges`.
-                        Default: `Greys`.
-  --annotate_sequences [ANNOTATE_SEQUENCES]
-                        Annotate sequences in the plot.
-                        Options: `accession`, `name`, and `fname`.
-                        `accession` and `name` are obtained from the `ACCESSION`
-                        and `LOCUS` gb file tags, repectively. `fname` is the file
-                        name.
-                        If the flag is provided without argument, the sequences will
-                        be annotated using `accession` numbers.
-  --annotate_genes [ANNOTATE_GENES]
-                        Annotate genes from top and bottom sequences.
-                        Options: `top`, `bottom`, and `both`.
-                        If the flag is provided without argument, only the genes at
-                        the top of the plot will be annotated.
+                        https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.savefig.html
+                        Default: `png`.
+  -d DPI, --dpi DPI     Resolution in dots per inch.
+                        Default: 300 (high resolution for print).
+  --alignments_position ALIGNMENTS_POSITION
 
-Graphic User Interfase:
-  -g, --gui             Run app in a graphic user interface.
 ```
 
-## Usage examples
+## Usage examples CLI
 
 To make a figure with default parameters:
 
 ```bash
 msplotter -i path/file_1.gb path/file_2.gb path/file_3.gb
 ```
 
 To save a figure in pdf format:
 
 ```bash
 msplotter -i path/file_1.gb path/file_2.gb path/file_3.gb -f pdf
 ```
 
-If you don't like the terminal and prefer a graphical user interface:
-
-```bash
-msplotter --gui
-```
-
 ## Notes
 
 I started this project to make a figure paper with three sequences with lengths
 between 8 to 23 kb. However, the matplotlib parameters can be adjusted for
 larger, smaller, or more sequences.
 
 ## Credits
```

### Comparing `msplotter-0.1.29/README.md` & `msplotter-0.1.30/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,78 @@
 <p align="center">
    <img src="./src/msp/images/logo.png" alt="MSPlotter" width="350">
 </p>
 
-# Make a graphical representation of a blantn alignment
+# Make a graphical representation of a blastn alignment
 
 Multiple Sequence Plotter (MSPlotter) uses GenBank files (.gb) to align the
-sequences and plot the genes. To plot the genes, MSPlotter uses the information
-from the `CDS` features section. To customize the colors for plotting genes,
-you can add a `Color` tag in the `CDS` features with a color in hexadecimal.
-For example, to show a gene in green add the tag `/Color="#00ff00"`. To avoid
-direct the manual manipulation of the GenBank file, you can edit the file with
+sequences and plot the genes. MSPlotter uses the information from the `CDS`
+features section to plot the genes. To customize the colors for plotting genes,
+you can add a `Color` tag in the `CDS` features with color in hexadecimal.
+For example, add the tag `/Color="#00ff00"` to show a gene in green. To avoid
+direct manual manipulation of the GenBank file, you can edit the file with
 `Geneious` or another software and export the file with the new annotations.
 
-MSPlotter uses `matplotlib`. Therefore, to customize your figure, you can
-modify the parameters in the `MakeFigure` class of the `msplotter` module.
+MSPlotter is an easy-to-use option for people with little coding knowledge or
+problems running the classic app `easyfig`. The program offers a graphical user
+interface (GUI) and a command line interface (CLI).
+
+If the user knows Python, MSPlotter uses `matplotlib`. Therefore, to customize
+your figure, the user can modify the parameters in the `MakeFigure` class of
+the `msplotter` module or make any necessary change in any part of the code.
+
+I am developing MSPlotter in my free time, therefore, if you find a bug, it may
+take me some time to fix it, but I will try to do my best to fix the problems
+as soon as possible. Also, if you have any suggestions, let me know, and I will
+try to implement them.
 
 ## Requirements
 
 - [Python](https://www.python.org/) 3.11 or later
 - [biopython](https://biopython.org/) 1.81 or later
 - [customtkinter](https://customtkinter.tomschimansky.com/) 5.1 or later
 - [matplotlib](https://matplotlib.org/) 3.7 or later
-- [blastn](https://www.ncbi.nlm.nih.gov/books/NBK569861/) must be installed locally and in the path
+- [blastn](https://www.ncbi.nlm.nih.gov/books/NBK569861/) must be installed
+  locally and in the path
+
+MSPlotter has been tested in macOS and Windows.
 
 ## Installation
 
-Create a virtual environment and install msplotter using pip as follows:
+First, create a virtual environment with `conda` or `venv`. Then, install
+msplotter using pip as follows:
 
 ```bash
 pip install msplotter
 ```
 
 ## Usage and options
 
+To run the GUI type:
+
+```bash
+msplotter --gui
+```
+
+Output GUI:
+
+<p align="center">
+   <img src="./src/msp/images/MSPlotter_gui.png" alt="MSPlotter" width="350">
+</p>
+
 To view all the options run:
 
 ```bash
 msplotter --help
 ```
 
-Output:
+Partial output CLI:
 
 ```console
-usage: msplotter [-h] [-v] [-i INPUT [INPUT ...]] [-o OUTPUT] [-n NAME] [-f FORMAT]
+usage: msplotter [-h] [-v] [-i INPUT [INPUT ...]] [-o OUTPUT] [-n NAME] [-f FORMAT] [-d DPI]
                  [--alignments_position ALIGNMENTS_POSITION] [--identity_color IDENTITY_COLOR]
                  [--annotate_sequences [ANNOTATE_SEQUENCES]] [--annotate_genes [ANNOTATE_GENES]] [-g]
 
 Make a graphical representation of a blastn alignment.
 
 Help:
   -h, --help            Show this help message and exit.
@@ -59,64 +85,38 @@
 Optional:
   -o OUTPUT, --output OUTPUT
                         Path to output folder.
                         Default: current working directory.
   -n NAME, --name NAME  Name of figure.
                         Default: `figure`.
   -f FORMAT, --format FORMAT
-                        Format of figure.
-                        Default: `pdf`.
-  --alignments_position ALIGNMENTS_POSITION
-                        Orientation of the alignments in the plot.
-                        Options: `left`, `center`, and `rigth`.
-                        Default: `left`.
-  --identity_color IDENTITY_COLOR
-                        Color map representing homology regions.
+                        Format of figure. Options: pdf, png, and svg.
                         For a complete list of valid options visit:
-                        https://matplotlib.org/stable/tutorials/colors/colormaps.html
-                        Some options: `Greys`, `Purples`, `Blues`, and `Oranges`.
-                        Default: `Greys`.
-  --annotate_sequences [ANNOTATE_SEQUENCES]
-                        Annotate sequences in the plot.
-                        Options: `accession`, `name`, and `fname`.
-                        `accession` and `name` are obtained from the `ACCESSION`
-                        and `LOCUS` gb file tags, repectively. `fname` is the file
-                        name.
-                        If the flag is provided without argument, the sequences will
-                        be annotated using `accession` numbers.
-  --annotate_genes [ANNOTATE_GENES]
-                        Annotate genes from top and bottom sequences.
-                        Options: `top`, `bottom`, and `both`.
-                        If the flag is provided without argument, only the genes at
-                        the top of the plot will be annotated.
+                        https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.savefig.html
+                        Default: `png`.
+  -d DPI, --dpi DPI     Resolution in dots per inch.
+                        Default: 300 (high resolution for print).
+  --alignments_position ALIGNMENTS_POSITION
 
-Graphic User Interfase:
-  -g, --gui             Run app in a graphic user interface.
 ```
 
-## Usage examples
+## Usage examples CLI
 
 To make a figure with default parameters:
 
 ```bash
 msplotter -i path/file_1.gb path/file_2.gb path/file_3.gb
 ```
 
 To save a figure in pdf format:
 
 ```bash
 msplotter -i path/file_1.gb path/file_2.gb path/file_3.gb -f pdf
 ```
 
-If you don't like the terminal and prefer a graphical user interface:
-
-```bash
-msplotter --gui
-```
-
 ## Notes
 
 I started this project to make a figure paper with three sequences with lengths
 between 8 to 23 kb. However, the matplotlib parameters can be adjusted for
 larger, smaller, or more sequences.
 
 ## Credits
```

### Comparing `msplotter-0.1.29/pyproject.toml` & `msplotter-0.1.30/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msplotter"
-version = "0.1.29"
+version = "0.1.30"
 authors = [
     {name = "Ivan Muñoz-Gutierrez", email = "ivan.munoz.gutierrez@gmail.com"},
 ]
 description = "Make a graphical representation of a blastn alignment"
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = [
```

### Comparing `msplotter-0.1.29/src/msp/arrows.py` & `msplotter-0.1.30/src/msp/arrows.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.29/src/msp/colormap_picker.py` & `msplotter-0.1.30/src/msp/colormap_picker.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.29/src/msp/gui.py` & `msplotter-0.1.30/src/msp/gui.py`

 * *Files 26% similar despite different names*

```diff
@@ -25,31 +25,36 @@
         self.gb_files: list = None
         self.figure_msp = None                 # msplotter object.
         self.identity_color: str = "Greys"
         self.colormap_range: tuple = (0, 0.75)
         self.y_limit: float = 0                # to adjust position of colormap
         self.scale_bar: bool = False
         self.annotate_sequences: bool = False
+        # if self.annotate_sequences is True, self.sequence_name is used for
+        # annotating the sequences.
+        self.sequence_name: str = "accession"
         self.annotate_genes: bool = False
+        self.annotate_genes_from: str = "gene_tag"
 
         # -- Set layout parameters --------------------------------------------
-        self.geometry('600x700')
+        self.geometry('750x600')
         self.title('MSPlotter')
         self.grid_rowconfigure(1, weight=1)
-        self.grid_columnconfigure(1, weight=1)
+        self.grid_columnconfigure((2,3), weight=1)
+        self.grid_columnconfigure((0,1), weight=0)
         # Protocol to close app, including plot if exist.
         self.protocol('WM_DELETE_WINDOW', self.on_closing)
         # Variable to store the ColormapPicker class used in the
         # launch_colormap_picker function.
         self.colormap_app = None
 
         # -- Navigation frame -------------------------------------------------
         # Create navigation frame.
         self.navigation_frame = customtkinter.CTkFrame(self, corner_radius=0)
-        self.navigation_frame.grid(row=0, column=0, columnspan=3, sticky='nsew')
+        self.navigation_frame.grid(row=0, column=0, columnspan=4, sticky='nsew')
         self.navigation_frame.grid_columnconfigure(0, weight=1)
         # Logo label
         self.logo_label = customtkinter.CTkLabel(
             self.navigation_frame, text='MSPloter',
             font=customtkinter.CTkFont(size=24, weight='bold')
         )
         self.logo_label.grid(row=0, column=0, padx=(10,5), pady=20)
@@ -59,143 +64,194 @@
             command=self.get_files_path
         )
         self.select_button.grid(row=0, column=1, padx=5, pady=20)
         # Clear button
         self.clear_button = customtkinter.CTkButton(
             self.navigation_frame, text='Clear',
             command=self.clear_input,
-            state='disabled'
+            state='disabled',
         )
         self.clear_button.grid(row=0, column=2, padx=5, pady=20)
         # Plot button
         self.plot_button = customtkinter.CTkButton(
             self.navigation_frame, text='Plot',
             command=self.plot_figure,
-            state='disabled'
+            state='disabled',
+            fg_color='#b300b3',
+            hover_color='#800080',
         )
         self.plot_button.grid(row=0, column=3, padx=(5,10), pady=20)
 
         # -- Appearance frame -------------------------------------------------
         self.appearance_frame = customtkinter.CTkFrame(
             self, corner_radius=5,
         )
         self.appearance_frame.grid(
-            row=1, column=0, padx=(10, 5), pady=10, sticky='nsew'
+            row=1, column=0, columnspan=2, padx=(10, 5), pady=10, sticky='nsew'
         )
-        self.appearance_frame.grid_rowconfigure(13, weight=1)
+        self.appearance_frame.grid_rowconfigure(9, weight=1)
+        self.appearance_frame.grid_columnconfigure((0,1), weight=0)
         # Appearance label
         self.appearance_label = customtkinter.CTkLabel(
             self.appearance_frame,
             text='Appearance',
             font=customtkinter.CTkFont(size=18, weight='bold'),
             width=120,
             height=50,
             corner_radius=5,
             # fg_color=self.appearance_fg_color,
         )
         self.appearance_label.grid(
-            row=0, column=0, pady=(10,10), sticky='nswe'
+            row=0, column=0, columnspan=2, pady=(10,10), sticky='nswe'
         )
-        # Homology color label
-        self.homology_label = customtkinter.CTkLabel(
-            self.appearance_frame, text='Homology color:',
-        )
-        self.homology_label.grid(row=1, column=0, pady=(10,0))
-        # Colormap picker
-        self.format_button = customtkinter.CTkButton(
-            self.appearance_frame,
-            text='Choose colormap',
-            command=self.launch_colormap_picker
-        )
-        self.format_button.grid(row=2, column=0, padx=20, pady=(0, 10))
         # Align plot label
         self.align_plot_label = customtkinter.CTkLabel(
             self.appearance_frame, text='Align plot:'
         )
-        self.align_plot_label.grid(row=3, column=0, pady=(10, 0))
+        self.align_plot_label.grid(row=1, column=0, pady=(10, 0))
         # Variable to store align_plot menu selection
         self.align_plot_var = customtkinter.StringVar(self, 'Left')
         # Align plot menu
         self.align_plot = customtkinter.CTkOptionMenu(
             self.appearance_frame,
             values=['Left', 'Center', 'Right'],
             variable=self.align_plot_var,
         )
-        self.align_plot.grid(row=4, column=0, padx=20, pady=(0, 10))
+        self.align_plot.grid(row=2, column=0, padx=20, pady=(0, 10))
         # Annotate sequences label
         self.annotate_seq_label = customtkinter.CTkLabel(
             self.appearance_frame, text='Annotate sequences:'
         )
-        self.annotate_seq_label.grid(row=5, column=0, pady=(10, 0))
+        self.annotate_seq_label.grid(row=3, column=0, pady=(10, 0))
         # Variable to store annotate_seq menu selection
         self.annotate_seq_var = customtkinter.StringVar(self, 'No')
         # Annotate sequences menu
         self.annotate_seq_menu = customtkinter.CTkOptionMenu(
             self.appearance_frame,
-            values=['No', 'Yes'],
+            values=['No', 'From acc number', 'From file name'],
             variable=self.annotate_seq_var,
             command=lambda _:self.update_annotate_seq()
         )
-        self.annotate_seq_menu.grid(row=6, column=0, pady=(0,10))
+        self.annotate_seq_menu.grid(row=4, column=0, pady=(0,10))
         # Annotate genes label
         self.annotate_genes_label = customtkinter.CTkLabel(
             self.appearance_frame, text='Annotate genes:'
         )
-        self.annotate_genes_label.grid(row=7, column=0, pady=(10,0))
+        self.annotate_genes_label.grid(row=5, column=0, pady=(10,0))
         # Variable to store annotate_genes menu selection
         self.annotate_genes_var = customtkinter.StringVar(self, 'No')
         # Annotate genes menu
         self.annotate_genes_menu = customtkinter.CTkOptionMenu(
             self.appearance_frame,
-            values=['No', 'Yes'],
+            values=['No', 'From gene tag', 'From product tag'],
             variable=self.annotate_genes_var,
             command=lambda _:self.update_annotate_genes()
         )
-        self.annotate_genes_menu.grid(row=8, column=0, pady=(0,10))
+        self.annotate_genes_menu.grid(row=6, column=0, pady=(0,10))
+        # Homology color label
+        self.homology_label = customtkinter.CTkLabel(
+            self.appearance_frame, text='Homology color:',
+        )
+        self.homology_label.grid(row=1, column=1, pady=(10,0))
+        # Colormap picker
+        self.format_button = customtkinter.CTkButton(
+            self.appearance_frame,
+            text='Choose colormap',
+            command=self.launch_colormap_picker
+        )
+        self.format_button.grid(row=2, column=1, padx=20, pady=(0, 10))
         # Scale bar label
         self.scale_bar_label = customtkinter.CTkLabel(
             self.appearance_frame, text='Scale bar:'
         )
-        self.scale_bar_label.grid(row=9, column=0, pady=(10,0))
+        self.scale_bar_label.grid(row=3, column=1, pady=(10,0))
         # Variable to store scale_bar menu selection
         self.scale_bar_var = customtkinter.StringVar(self, 'No')
         # Scale bar menu
         self.scale_bar_menu = customtkinter.CTkOptionMenu(
             self.appearance_frame,
             values=['No', 'Yes'],
             variable=self.scale_bar_var,
             command=lambda _:self.update_scale_bar()
         )
-        self.scale_bar_menu.grid(row=10, column=0, pady=(0,10))
+        self.scale_bar_menu.grid(row=4, column=1, pady=(0,10))
         # Color map position label
         self.cmap_position_label = customtkinter.CTkLabel(
             self.appearance_frame, text='Position colormap:'
         )
-        self.cmap_position_label.grid(row=11, column=0, pady=(10, 0))
+        self.cmap_position_label.grid(row=5, column=1, pady=(10, 0))
         # Color map position spinbox
         self.cmap_position_spinbox = FloatSpinbox(
             self.appearance_frame,
             width=140,
             height=28,
             command=self.update_y_limit
         )
-        self.cmap_position_spinbox.grid(row=12, column=0, pady=(0, 10))
+        self.cmap_position_spinbox.grid(row=6, column=1, pady=(0, 10))
+        # Create a validation function to check for float input in entry boxes
+        self.validation = self.register(self.validate_input)
+        # Change width check box variable
+        self.width_check_var = customtkinter.StringVar(value='off')
+        # Change width check box
+        self.width_check = customtkinter.CTkCheckBox(
+            self.appearance_frame,
+            text='Change figure width:',
+            variable=self.width_check_var,
+            onvalue='on',
+            offvalue='off',
+            command=self.change_figure_width_event
+        )
+        self.width_check.grid(
+            row=7, column=0, sticky='w', padx=(10,0), pady=(20, 10))
+        # Change width entry box
+        self.width_entry = customtkinter.CTkEntry(
+            self.appearance_frame,
+            validate='key',
+            validatecommand=(self.validation, '%P'),
+        )
+        self.width_entry.grid(
+            row=7, column=1, sticky='we', padx=(0,10), pady=(20, 10))
+        self.width_entry.configure(state='disabled')
+        # Change height check box variable
+        self.height_check_var = customtkinter.StringVar(value='off')
+        # Change height check box
+        self.height_check = customtkinter.CTkCheckBox(
+            self.appearance_frame,
+            text='Change figure height:',
+            variable=self.height_check_var,
+            onvalue='on',
+            offvalue='off',
+            command=self.change_figure_height_event
+        )
+        self.height_check.grid(
+            row=8, column=0, sticky='w', padx=(10,0), pady=(10))
+        # Change height entry box
+        self.height_entry = customtkinter.CTkEntry(
+            self.appearance_frame,
+            validate='key',
+            validatecommand=(self.validation, '%P'),
+        )
+        self.height_entry.grid(
+            row=8, column=1, sticky='we', padx=(0,10), pady=(10))
+        self.height_entry.configure(state='disabled')
         # Reset button
         self.reset_button = customtkinter.CTkButton(
-            self.appearance_frame, text='Reset', command=self.reset_appearance
+            self.appearance_frame, text='Reset', fg_color='transparent',
+            text_color=('gray10', '#DCE4EE'), border_width=2,
+            command=self.reset_appearance
         )
-        self.reset_button.grid(row=13, column=0, pady=(20, 10))
+        self.reset_button.grid(row=9, column=0, columnspan=2, pady=(10, 10))
 
         # -- Display frame ---------------------------------------------------
         # Create display frame
         self.display_frame = customtkinter.CTkFrame(
             self, corner_radius=0,
             fg_color='transparent'
         )
-        self.display_frame.grid(row=1, column=1, columnspan=2, sticky='nsew')
+        self.display_frame.grid(row=1, column=2, columnspan=2, sticky='nsew')
         self.display_frame.grid_rowconfigure(0, weight=1)
         self.display_frame.grid_columnconfigure(0, weight=1)
         self.display_window = customtkinter.CTkTextbox(
             self.display_frame, wrap='word'
         )
         self.display_window.grid(row=0, column=0, padx=(5, 10), pady=10,
             sticky='nsew'
@@ -272,34 +328,78 @@
             f'The homology regions are going to be shown in `{cmap_name}` ' +
             f'with a range of colors between `{round(cmap_range[0])}-'
             f'{round(cmap_range[1])}`.'
         )
         self.display_window.configure(state='disabled')
 
     def update_annotate_seq(self):
-        if self.annotate_seq_var.get() == 'No':
+        if (annotate := self.annotate_seq_var.get()) == 'No':
             self.annotate_sequences = False
+            return
         else:
             self.annotate_sequences = True
+        if annotate == "From acc number":
+            self.sequence_name = "accession"
+        else:
+            self.sequence_name = "fname"
 
     def update_annotate_genes(self):
-        if self.annotate_genes_var.get() == 'No':
+        if (annotate := self.annotate_genes_var.get()) == 'No':
             self.annotate_genes = False
+            return
         else:
             self.annotate_genes = True
+        if annotate == "From gene tag":
+            self.annotate_genes_from = "gene_tag"
+        else:
+            self.annotate_genes_from = "product_tag"
 
     def update_scale_bar(self):
         if self.scale_bar_var.get() == 'No':
             self.scale_bar = False
         else:
             self.scale_bar = True
 
     def update_y_limit(self):
         self.y_limit = self.cmap_position_spinbox.get()
 
+    def change_figure_width_event(self):
+        if self.width_check_var.get() == 'on':
+            self.width_entry.configure(state='normal')
+        else:
+            self.width_entry.configure(state='disabled')
+
+    def change_figure_height_event(self):
+        if self.height_check_var.get() == 'on':
+            self.height_entry.configure(state='normal')
+        else:
+            self.height_entry.configure(state='disabled')
+
+    def validate_input(self, value):
+        if value == "":
+            return True
+        try:
+            float(value)
+            return True
+        except ValueError:
+            return False
+
+    def get_figure_size(self) -> tuple[float, float]:
+        width = self.width_entry.get()
+        height = self.height_entry.get()
+        if not width:
+            width = None
+        else:
+            width = float(width)
+        if not height:
+            height = None
+        else:
+            height = float(height)
+        return (width, height)
+
     def reset_appearance(self):
         """Reset appearance parameters."""
         # Reset color map
         self.identity_color = "Greys"
         self.colormap_range = (0, 0.75)
         # Reset align plot
         self.align_plot_var.set('Left')
@@ -312,14 +412,23 @@
         self.annotate_genes_menu.configure(variable=self.annotate_genes_var)
         # Reset scale bar
         self.scale_bar_var.set('No')
         self.scale_bar_menu.configure(variable=self.scale_bar_var)
         # Reset y_limit
         self.y_limit = 0
         self.cmap_position_spinbox.set(0.0)
+        # Reset figure width and height functionality
+        self.width_check.deselect()
+        self.height_check.deselect()
+        self.width_entry.configure(state='normal')
+        self.width_entry.delete(0, 'end')
+        self.width_entry.configure(state='disabled')
+        self.height_entry.configure(state='normal')
+        self.height_entry.delete(0, 'end')
+        self.height_entry.configure(state='disabled')
 
     def plot_figure(self):
         """Plot alignments using msplotter."""
         # Create fasta files for BLASTing.
         faa_files = msp.make_fasta_file(self.gb_files)
         # Run blastn locally.
         xml_results = msp.run_blastn(faa_files)
@@ -327,23 +436,29 @@
         msp.delete_files(faa_files)
         # Make a list of `BlastnAlignment` classes from the xml blastn results.
         alignments = msp.get_alignment_records(xml_results)
         # Delete xml documents.
         msp.delete_files(xml_results)
         # Make a list of `GenBankRecord` classes from the gb files.
         gb_records = msp.get_gb_records(self.gb_files)
+        # Get figure size
+        width, height = self.get_figure_size()
         # Make figure.
         self.figure_msp = msp.MakeFigure(
             alignments,
             gb_records,
+            figure_width=width,
+            figure_height=height,
             alignments_position=self.align_plot_var.get().lower(),
             identity_color=self.identity_color,
             color_map_range=self.colormap_range,
             annotate_sequences=self.annotate_sequences,
+            sequence_name=self.sequence_name,
             annotate_genes=self.annotate_genes,
+            annotate_genes_from=self.annotate_genes_from,
             scale_bar=self.scale_bar,
             y_limit=self.y_limit,
             use_gui=True
         )
         # Plot figure using the Plot class
         self.figure_plt = self.figure_msp.make_figure()
         # Plot figure
```

### Comparing `msplotter-0.1.29/src/msp/images/Blues.png` & `msplotter-0.1.30/src/msp/images/Blues.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.29/src/msp/images/BuGn.png` & `msplotter-0.1.30/src/msp/images/BuGn.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.29/src/msp/images/BuPu.png` & `msplotter-0.1.30/src/msp/images/BuPu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.29/src/msp/images/GnBu.png` & `msplotter-0.1.30/src/msp/images/GnBu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.29/src/msp/images/Greens.png` & `msplotter-0.1.30/src/msp/images/Greens.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.29/src/msp/images/OrRd.png` & `msplotter-0.1.30/src/msp/images/OrRd.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.29/src/msp/images/Oranges.png` & `msplotter-0.1.30/src/msp/images/Oranges.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.29/src/msp/images/PuBu.png` & `msplotter-0.1.30/src/msp/images/PuBu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.29/src/msp/images/PuBuGn.png` & `msplotter-0.1.30/src/msp/images/PuBuGn.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.29/src/msp/images/PuRd.png` & `msplotter-0.1.30/src/msp/images/PuRd.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.29/src/msp/images/Purples.png` & `msplotter-0.1.30/src/msp/images/Purples.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.29/src/msp/images/RdPu.png` & `msplotter-0.1.30/src/msp/images/RdPu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.29/src/msp/images/Reds.png` & `msplotter-0.1.30/src/msp/images/Reds.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.29/src/msp/images/YlGn.png` & `msplotter-0.1.30/src/msp/images/YlGn.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.29/src/msp/images/YlGnBu.png` & `msplotter-0.1.30/src/msp/images/YlGnBu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.29/src/msp/images/YlOrBr.png` & `msplotter-0.1.30/src/msp/images/YlOrBr.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.29/src/msp/images/YlOrRd.png` & `msplotter-0.1.30/src/msp/images/YlOrRd.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.29/src/msp/images/logo.png` & `msplotter-0.1.30/src/msp/images/logo.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.29/src/msp/msplotter.py` & `msplotter-0.1.30/src/msp/msplotter.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,29 +15,30 @@
 -------
 This file is part of MSPloter
 BSD 3-Clause License
 Copyright (c) 2023, Ivan Munoz Gutierrez
 """
 import os
 import sys
+from pathlib import Path
+from typing import Union
 
 import matplotlib as mpl
 from matplotlib.axes import Axes
 import matplotlib.colors as colors
 from matplotlib.colors import Colormap
 import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
 from mpl_toolkits.axes_grid1.inset_locator import inset_axes
 import matplotlib.ticker as ticker
 import numpy as np
 from Bio import SeqIO
 from Bio.Blast import NCBIXML
 from Bio.Blast.Applications import NcbiblastnCommandline
 from Bio.SeqRecord import SeqRecord
-from pathlib import Path
 
 from msp.arrows import Arrow
 
 
 class GenBankRecord:
     """Store relevant info from a GenBank file.
 
@@ -95,43 +96,45 @@
         coding_sequences : list
             List of `CodingSequence` classes holding CDSs' information.
         """
         coding_sequences = []
         for feature in record.features:
             if feature.type != 'CDS':
                 continue
-            product = feature.qualifiers.get('product', None)
-            if product is not None:
+            if gene := feature.qualifiers.get('gene', None):
+                gene = gene[0]
+            if product := feature.qualifiers.get('product', None):
                 product = product[0]
-            if feature.qualifiers.get('Color', None) is None:
-                color = '#ffff00'    # Make yellow default color
-            else:
+            if color := feature.qualifiers.get('Color', None):
                 color = feature.qualifiers['Color'][0]
+            else:
+                color = '#ffff00'    # Make yellow default color
             # Some CDS are composed of more than one parts, like introns, or,
             # in the case of some bacteria, some genes have frameshifts as a
             # regulatory function (some transposase genes have frameshifts as
             # a regulatory function).
             for part in feature.location.parts:
                 strand = part._strand
                 if strand == -1:
                     start = part._end
                     end = part._start + 1
                 else:
                     start = part._start + 1
                     end = part._end
                 # Append cds.
                 coding_sequences.append(CodingSequence(
-                    product, start, end, strand, color
+                    gene, product, start, end, strand, color
                 ))
         return coding_sequences
 
 
 class CodingSequence:
     """Store Coding Sequence (CDS) information from gb file."""
-    def __init__(self, product, start, end, strand, color):
+    def __init__(self, gene, product, start, end, strand, color):
+        self.gene = gene
         self.product = product
         self.start = int(start)
         self.end = int(end)
         self.strand = int(strand)
         self.color = color
 
 
@@ -252,17 +255,17 @@
             query=faa_files[i],
             subject=faa_files[i+1],
             outfmt=5,
             out=output_file)
         stdout, stderr = blastn_cline()
         results.append(output_file)
         print(
-            f'BLASTing {faa_files[i]} (query) and {faa_files[i+1]} (subject)'
+            f'BLASTing {faa_files[i]} (query) and {faa_files[i+1]} (subject)\n'
         )
-        print(stdout + '\n' + stderr)
+        # print(stdout + '\n' + stderr)
     return results
 
 
 def delete_files(documents: list) -> None:
     """Delete the files from `documents` list."""
     for document in documents:
         if os.path.exists(document):
@@ -300,17 +303,20 @@
         Annotate genes in plot (default: False).
     annotate_genes_on_sequence : tuple with the str `top`, and/or `bottom`
         Annotate genes at the top, bottom or both.
     annotate_sequences : bool
         Annotate sequences in plot (defalult: False). If True, the `top` and
         `bottom` sequences are annotated.
     sequence_name : str
-        String to access either `name` or `accession` from GenBankRecord class
-        (default: `accession`). Either `name` or `accession` is used to
-        annotate the sequence if `add_annotations_sequences` attribute is True.
+        Option: `name`, `fname`, and `accession` (default: `accession`).
+        If `name` or `accession` is provided, their values are extracted from
+        the GenBankRecord class. If `fname` is provided, the value is obtained
+        from the file name. If `add_annotations_sequences` attribute is
+        True, either `name`, `fname` or `accession` is used for annotating the
+        sequence.
     y_separation : float
         Distance between sequences in the y-axis (default: 10).
     y_limit : float
         Lower limit to show in the plot (default: 5). Use this value to adjust
         the position of the color map and the scale bar.
     sequence_color : str
         Color used for lines representing sequences (default: `black`). You can
@@ -335,34 +341,57 @@
         y_separation.
     save_figure : bool
         Save plotted figure.
     figure_name : Path
         Output path with figure's name.
     figure_format : str
         Format to save figure.
+    figure_width : Union[None, float]
+        Width of figure in inches (default: None). If None, MSPlotter
+        determines the value.
+    figure_height : Union[None, float]
+        Height of figure in inches (default: None). If None, MSPlotter
+        determines the value.
     dpi : float
         Resolution of figure in dots per inch (default: 300.0).
     user_gui : bool
         Run app in a graphical user interface (default: False).
     """
     def __init__(
-        self, alignments, gb_records, alignments_position="left",
-        annotate_genes=False, annotate_genes_on_sequence=("top", "bottom"),
-        annotate_sequences=False, sequence_name="accession", y_separation=10,
-        y_limit=5, sequence_color="black", sequence_width=3,
-        identity_color="Greys", scale_bar=True, color_map_range=(0, 0.75),
-        homology_padding=0.1, figure_name=(Path.cwd() / 'figure.png'),
-        figure_format='png', dpi=300.0, use_gui=False
+        self,
+        alignments,
+        gb_records,
+        alignments_position: str = "left",
+        annotate_genes: bool = False,
+        annotate_genes_on_sequence: tuple[str] = ("top", "bottom"),
+        annotate_genes_from: str = "gene_tag",
+        annotate_sequences: bool = False,
+        sequence_name: str = "accession",
+        y_separation: int = 10,
+        y_limit: int = 5,
+        sequence_color: str = "black",
+        sequence_width: int = 3,
+        identity_color: str = "Greys",
+        scale_bar: bool = True,
+        color_map_range: tuple[float] = (0, 0.75),
+        homology_padding: float = 0.1,
+        figure_name: Path = (Path.cwd() / 'figure.png'),
+        figure_format: str = 'png',
+        figure_width: Union[None, float] = None,
+        figure_height: Union[None, float] = None,
+        dpi: float = 300.0,
+        use_gui: bool = False
     ):
         self.alignments = alignments
         self.num_alignments = len(alignments)
         self.gb_records = gb_records
         self.alignments_position = alignments_position
         self.annotate_genes = annotate_genes
         self.annotate_genes_on_sequence = annotate_genes_on_sequence
+        self.annotate_genes_from = annotate_genes_from
         self.annotate_sequences = annotate_sequences
         self.sequence_name = sequence_name
         self.y_separation = y_separation
         self.y_limit = y_limit
         self.sequence_color = sequence_color
         self.sequence_width = sequence_width
         self.identity_color = identity_color
@@ -380,14 +409,16 @@
             round(self.get_lowest_and_highest_homology()[0] * 100)
         )
         self.highest_homology = int(
             round(self.get_lowest_and_highest_homology()[1] * 100)
         )
         self.figure_name = figure_name
         self.figure_format = figure_format
+        self.figure_width = figure_width
+        self.figure_height = figure_height
         self.dpi = dpi
         self.save_figure = self.check_save_figure()
         self.use_gui = use_gui
 
     def get_lowest_and_highest_homology(self) -> tuple:
         """Get the lowest and highest homologies in the alignment."""
         lowest = 100
@@ -752,45 +783,61 @@
         for position in self.annotate_genes_on_sequence:
             if position == 'top':
                 parameters = top
             elif position == 'bottom':
                 parameters = bottom
             for gene in parameters["gb_record"].cds:
                 location_annotation = (gene.start + gene.end) / 2
+                if self.annotate_genes_from == "gene_tag":
+                    annotation = gene.gene
+                else:
+                    annotation = gene.product
                 ax.annotate(
-                    gene.product,
+                    annotation,
                     xy=(location_annotation, parameters["y_distance"]),
                     xytext=(0, parameters["y_text"]),
                     textcoords="offset points",
                     rotation=90,
                     ha="center",
                     horizontalalignment=parameters["h_alignment"],
                     verticalalignment=parameters["v_alignment"]
                 )
 
     def determine_figure_size(
-            self, num_alignments: int) -> tuple[float, float]:
-        """Determine figure size."""
-        # The Matplotlib default figure size is 6.4 x 4.8.
-        width = 6.4
-        height = 4.8
+            self, num_alignments: int
+        ) -> tuple[float, float]:
+        """Determine figure size.
+
+        If user doesn't provide height, adjust height by number of alignments.
+        """
+        # The Matplotlib default figure size is 6.4 x 4.8 inches.
+        if not self.figure_width:
+            width = 6.4
+        else:
+            width = self.figure_width
+        if not self.figure_height:
+            auto_height = True
+            height = 4.8
+        else:
+            auto_height = False
+            height = self.figure_height
         # Adjust height based on four alignments.
-        if num_alignments > 4:
+        if (auto_height) and (num_alignments > 4):
             height = height * (num_alignments / 4)
         return (width, height)
 
     def make_figure(self):
         """Make figure with matplotlib."""
         # -- Remove toolbar from plot -----------------------------------------
         mpl.rcParams['toolbar'] = 'None'
-        # -- Determine figure size by number of alignments --------------------
+        # -- Determine figure size --------------------------------------------
         width, height = self.determine_figure_size(self.num_alignments)
         # -- Change figure size -----------------------------------------------
-        # Matplotlib default size is 6.4 x 4.8.
         fig, ax = plt.subplots(
+            # Matplotlib default size is 6.4 x 4.8 inches
             figsize=(width, height),
             layout="constrained"
         )
         # -- Remove figure axis -----------------------------------------------
         ax.set_axis_off()
         # -- Plot DNA sequences -----------------------------------------------
         self.plot_dna_sequences(ax)
```

### Comparing `msplotter-0.1.29/src/msp/plot.py` & `msplotter-0.1.30/src/msp/plot.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.29/src/msp/slider_widget.py` & `msplotter-0.1.30/src/msp/slider_widget.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.29/src/msp/spinbox.py` & `msplotter-0.1.30/src/msp/spinbox.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.29/src/msp/user_input.py` & `msplotter-0.1.30/src/msp/user_input.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.29/src/msplotter.egg-info/PKG-INFO` & `msplotter-0.1.30/src/msplotter.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msplotter
-Version: 0.1.29
+Version: 0.1.30
 Summary: Make a graphical representation of a blastn alignment
 Author-email: Ivan Muñoz-Gutierrez <ivan.munoz.gutierrez@gmail.com>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/ivanmugu/MSPlotter
 Keywords: blast,alignment,graphical representation,DNA sequence,easyfig
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
@@ -15,55 +15,81 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
    <img src="./src/msp/images/logo.png" alt="MSPlotter" width="350">
 </p>
 
-# Make a graphical representation of a blantn alignment
+# Make a graphical representation of a blastn alignment
 
 Multiple Sequence Plotter (MSPlotter) uses GenBank files (.gb) to align the
-sequences and plot the genes. To plot the genes, MSPlotter uses the information
-from the `CDS` features section. To customize the colors for plotting genes,
-you can add a `Color` tag in the `CDS` features with a color in hexadecimal.
-For example, to show a gene in green add the tag `/Color="#00ff00"`. To avoid
-direct the manual manipulation of the GenBank file, you can edit the file with
+sequences and plot the genes. MSPlotter uses the information from the `CDS`
+features section to plot the genes. To customize the colors for plotting genes,
+you can add a `Color` tag in the `CDS` features with color in hexadecimal.
+For example, add the tag `/Color="#00ff00"` to show a gene in green. To avoid
+direct manual manipulation of the GenBank file, you can edit the file with
 `Geneious` or another software and export the file with the new annotations.
 
-MSPlotter uses `matplotlib`. Therefore, to customize your figure, you can
-modify the parameters in the `MakeFigure` class of the `msplotter` module.
+MSPlotter is an easy-to-use option for people with little coding knowledge or
+problems running the classic app `easyfig`. The program offers a graphical user
+interface (GUI) and a command line interface (CLI).
+
+If the user knows Python, MSPlotter uses `matplotlib`. Therefore, to customize
+your figure, the user can modify the parameters in the `MakeFigure` class of
+the `msplotter` module or make any necessary change in any part of the code.
+
+I am developing MSPlotter in my free time, therefore, if you find a bug, it may
+take me some time to fix it, but I will try to do my best to fix the problems
+as soon as possible. Also, if you have any suggestions, let me know, and I will
+try to implement them.
 
 ## Requirements
 
 - [Python](https://www.python.org/) 3.11 or later
 - [biopython](https://biopython.org/) 1.81 or later
 - [customtkinter](https://customtkinter.tomschimansky.com/) 5.1 or later
 - [matplotlib](https://matplotlib.org/) 3.7 or later
-- [blastn](https://www.ncbi.nlm.nih.gov/books/NBK569861/) must be installed locally and in the path
+- [blastn](https://www.ncbi.nlm.nih.gov/books/NBK569861/) must be installed
+  locally and in the path
+
+MSPlotter has been tested in macOS and Windows.
 
 ## Installation
 
-Create a virtual environment and install msplotter using pip as follows:
+First, create a virtual environment with `conda` or `venv`. Then, install
+msplotter using pip as follows:
 
 ```bash
 pip install msplotter
 ```
 
 ## Usage and options
 
+To run the GUI type:
+
+```bash
+msplotter --gui
+```
+
+Output GUI:
+
+<p align="center">
+   <img src="./src/msp/images/MSPlotter_gui.png" alt="MSPlotter" width="350">
+</p>
+
 To view all the options run:
 
 ```bash
 msplotter --help
 ```
 
-Output:
+Partial output CLI:
 
 ```console
-usage: msplotter [-h] [-v] [-i INPUT [INPUT ...]] [-o OUTPUT] [-n NAME] [-f FORMAT]
+usage: msplotter [-h] [-v] [-i INPUT [INPUT ...]] [-o OUTPUT] [-n NAME] [-f FORMAT] [-d DPI]
                  [--alignments_position ALIGNMENTS_POSITION] [--identity_color IDENTITY_COLOR]
                  [--annotate_sequences [ANNOTATE_SEQUENCES]] [--annotate_genes [ANNOTATE_GENES]] [-g]
 
 Make a graphical representation of a blastn alignment.
 
 Help:
   -h, --help            Show this help message and exit.
@@ -76,64 +102,38 @@
 Optional:
   -o OUTPUT, --output OUTPUT
                         Path to output folder.
                         Default: current working directory.
   -n NAME, --name NAME  Name of figure.
                         Default: `figure`.
   -f FORMAT, --format FORMAT
-                        Format of figure.
-                        Default: `pdf`.
-  --alignments_position ALIGNMENTS_POSITION
-                        Orientation of the alignments in the plot.
-                        Options: `left`, `center`, and `rigth`.
-                        Default: `left`.
-  --identity_color IDENTITY_COLOR
-                        Color map representing homology regions.
+                        Format of figure. Options: pdf, png, and svg.
                         For a complete list of valid options visit:
-                        https://matplotlib.org/stable/tutorials/colors/colormaps.html
-                        Some options: `Greys`, `Purples`, `Blues`, and `Oranges`.
-                        Default: `Greys`.
-  --annotate_sequences [ANNOTATE_SEQUENCES]
-                        Annotate sequences in the plot.
-                        Options: `accession`, `name`, and `fname`.
-                        `accession` and `name` are obtained from the `ACCESSION`
-                        and `LOCUS` gb file tags, repectively. `fname` is the file
-                        name.
-                        If the flag is provided without argument, the sequences will
-                        be annotated using `accession` numbers.
-  --annotate_genes [ANNOTATE_GENES]
-                        Annotate genes from top and bottom sequences.
-                        Options: `top`, `bottom`, and `both`.
-                        If the flag is provided without argument, only the genes at
-                        the top of the plot will be annotated.
+                        https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.savefig.html
+                        Default: `png`.
+  -d DPI, --dpi DPI     Resolution in dots per inch.
+                        Default: 300 (high resolution for print).
+  --alignments_position ALIGNMENTS_POSITION
 
-Graphic User Interfase:
-  -g, --gui             Run app in a graphic user interface.
 ```
 
-## Usage examples
+## Usage examples CLI
 
 To make a figure with default parameters:
 
 ```bash
 msplotter -i path/file_1.gb path/file_2.gb path/file_3.gb
 ```
 
 To save a figure in pdf format:
 
 ```bash
 msplotter -i path/file_1.gb path/file_2.gb path/file_3.gb -f pdf
 ```
 
-If you don't like the terminal and prefer a graphical user interface:
-
-```bash
-msplotter --gui
-```
-
 ## Notes
 
 I started this project to make a figure paper with three sequences with lengths
 between 8 to 23 kb. However, the matplotlib parameters can be adjusted for
 larger, smaller, or more sequences.
 
 ## Credits
```

### Comparing `msplotter-0.1.29/src/msplotter.egg-info/SOURCES.txt` & `msplotter-0.1.30/src/msplotter.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 src/msp/user_input.py
 src/msp/images/Blues.png
 src/msp/images/BuGn.png
 src/msp/images/BuPu.png
 src/msp/images/GnBu.png
 src/msp/images/Greens.png
 src/msp/images/Greys.png
+src/msp/images/MSPlotter_gui.png
 src/msp/images/OrRd.png
 src/msp/images/Oranges.png
 src/msp/images/PuBu.png
 src/msp/images/PuBuGn.png
 src/msp/images/PuRd.png
 src/msp/images/Purples.png
 src/msp/images/RdPu.png
```


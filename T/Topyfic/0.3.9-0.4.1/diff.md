# Comparing `tmp/Topyfic-0.3.9.tar.gz` & `tmp/Topyfic-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Topyfic-0.3.9.tar", last modified: Thu Jun  1 18:09:08 2023, max compression
+gzip compressed data, was "Topyfic-0.4.1.tar", last modified: Mon Jul 24 20:52:14 2023, max compression
```

## Comparing `Topyfic-0.3.9.tar` & `Topyfic-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-06-01 18:09:08.264098 Topyfic-0.3.9/
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     1067 2022-01-27 20:57:46.000000 Topyfic-0.3.9/LICENSE.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      903 2023-06-01 18:09:08.264175 Topyfic-0.3.9/PKG-INFO
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     3280 2023-04-27 22:47:11.000000 Topyfic-0.3.9/README.md
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-06-01 18:09:08.262975 Topyfic-0.3.9/Topyfic/
--rw-rw-r--   0 nargesrezaie   (501) staff       (20)      226 2023-06-01 18:08:21.000000 Topyfic-0.3.9/Topyfic/__init__.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    44516 2023-05-31 23:01:59.000000 Topyfic-0.3.9/Topyfic/analysis.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     4128 2023-05-31 23:11:38.000000 Topyfic-0.3.9/Topyfic/main.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    13297 2023-05-31 23:11:38.000000 Topyfic-0.3.9/Topyfic/topModel.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     8983 2023-05-31 23:11:38.000000 Topyfic-0.3.9/Topyfic/topic.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    10440 2023-05-31 22:59:19.000000 Topyfic-0.3.9/Topyfic/train.py
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-06-01 18:09:08.263956 Topyfic-0.3.9/Topyfic.egg-info/
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      903 2023-06-01 18:09:08.000000 Topyfic-0.3.9/Topyfic.egg-info/PKG-INFO
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      304 2023-06-01 18:09:08.000000 Topyfic-0.3.9/Topyfic.egg-info/SOURCES.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)        1 2023-06-01 18:09:08.000000 Topyfic-0.3.9/Topyfic.egg-info/dependency_links.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      269 2023-06-01 18:09:08.000000 Topyfic-0.3.9/Topyfic.egg-info/requires.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)        8 2023-06-01 18:09:08.000000 Topyfic-0.3.9/Topyfic.egg-info/top_level.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)       79 2023-06-01 18:09:08.264444 Topyfic-0.3.9/setup.cfg
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     1997 2023-06-01 18:08:34.000000 Topyfic-0.3.9/setup.py
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-07-24 20:52:14.447967 Topyfic-0.4.1/
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     1067 2022-01-27 20:57:46.000000 Topyfic-0.4.1/LICENSE.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      903 2023-07-24 20:52:14.448052 Topyfic-0.4.1/PKG-INFO
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     3280 2023-04-27 22:47:11.000000 Topyfic-0.4.1/README.md
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-07-24 20:52:14.446776 Topyfic-0.4.1/Topyfic/
+-rw-rw-r--   0 nargesrezaie   (501) staff       (20)      197 2023-06-01 18:15:16.000000 Topyfic-0.4.1/Topyfic/__init__.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    45131 2023-07-24 20:48:04.000000 Topyfic-0.4.1/Topyfic/analysis.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     4087 2023-06-01 18:15:16.000000 Topyfic-0.4.1/Topyfic/main.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    13776 2023-06-05 22:53:45.000000 Topyfic-0.4.1/Topyfic/topModel.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     8982 2023-06-01 18:15:16.000000 Topyfic-0.4.1/Topyfic/topic.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    10440 2023-05-31 22:59:19.000000 Topyfic-0.4.1/Topyfic/train.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    19189 2023-07-14 01:34:33.000000 Topyfic-0.4.1/Topyfic/utilsAnalyseModel.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    21371 2023-05-31 23:11:38.000000 Topyfic-0.4.1/Topyfic/utilsMakeModel.py
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-07-24 20:52:14.447828 Topyfic-0.4.1/Topyfic.egg-info/
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      903 2023-07-24 20:52:14.000000 Topyfic-0.4.1/Topyfic.egg-info/PKG-INFO
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      359 2023-07-24 20:52:14.000000 Topyfic-0.4.1/Topyfic.egg-info/SOURCES.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)        1 2023-07-24 20:52:14.000000 Topyfic-0.4.1/Topyfic.egg-info/dependency_links.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      280 2023-07-24 20:52:14.000000 Topyfic-0.4.1/Topyfic.egg-info/requires.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)        8 2023-07-24 20:52:14.000000 Topyfic-0.4.1/Topyfic.egg-info/top_level.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)       79 2023-07-24 20:52:14.448325 Topyfic-0.4.1/setup.cfg
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     2018 2023-07-24 20:48:58.000000 Topyfic-0.4.1/setup.py
```

### Comparing `Topyfic-0.3.9/LICENSE.txt` & `Topyfic-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Topyfic-0.3.9/PKG-INFO` & `Topyfic-0.4.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Topyfic
-Version: 0.3.9
+Version: 0.4.1
 Summary: Topyfic is a Python package designed to identify reproducible latent dirichlet allocation (LDA) using leiden clustering and harmony for single cell epigenomics data
 Home-page: https://github.com/mortazavilab/Topyfic
-Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.3.9.tar.gz
+Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.4.1.tar.gz
 Author: Narges Rezaie
 Author-email: nargesrezaie80@gmail.com
 License: MIT
 Keywords: Cellular Programs,Latent Dirichlet allocation,single-cell multiome,single-cell RNA-seq,gene regulatory network,Topic Modeling,single-nucleus RNA-seq
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research 
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `Topyfic-0.3.9/README.md` & `Topyfic-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `Topyfic-0.3.9/Topyfic/analysis.py` & `Topyfic-0.4.1/Topyfic/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         :type ascending: list of bool
         :param metaData: if you want to add annotation for each cell add column name of that information (make sure you have that inforamtion in your cell_participation.obs)
         :type metaData: list
         :param metaData_palette: color palette for each metaData you add
         :type metaData_palette: dict
         :param width: width ratios of each category (default is based on the number of the cells we have in each category)
         :type width: list of int
-        :param n: number of topics you want to annotate in pie charts (default: 5)
+        :param n: number of topics you want to sum if you used order_cell == 'sum' (default: 2)
         :type n: int
         :param order_cells: determine which kind of sorting options you want to use ('sum', 'hierarchy', sort by metaData); sum: sort cells by sum of top n topics; hierarchy: sort data by doing hierarchical clustring; metaData sort by metaData (default: ['hierarchy'])
         :type order_cells: list
         :param save: indicate if you want to save the plot or not (default: True)
         :type save: bool
         :param show: indicate if you want to show the plot or not (default: True)
         :type show: bool
@@ -212,32 +212,41 @@
         :type file_format: str
         :param file_name: name and path of the plot use for save (default: piechart_topicAvgCell)
         :type file_name: str
         """
         if figsize is None:
             figsize = (10 * (len(category) + 1), 10)
 
-        check = ["hierarchy", "sum"] + metaData
+        check = ["hierarchy", "sum"]
+        if metaData is not None:
+            check = check + metaData
         for order_cell in order_cells:
             if order_cell not in check:
                 return "order cell was not valid"
 
         a = []
         for i in range(len(category)):
             a.append(self.cell_participation.obs[self.cell_participation.obs[level] == category[i]].shape[0])
         a.append(min(a) / 2)
         if width is None:
             width = a
-        b = [8] + [1] * len(metaData)
-        fig, axs = plt.subplots(nrows=len(metaData) + 1,
-                                ncols=len(category) + 1,
-                                figsize=figsize,
-                                gridspec_kw={'width_ratios': width,
-                                             'height_ratios': b},
-                                facecolor='white')
+        if metaData is None:
+            fig, axs = plt.subplots(nrows=1,
+                                    ncols=len(category) + 1,
+                                    figsize=figsize,
+                                    gridspec_kw={'width_ratios': width},
+                                    facecolor='white')
+        else:
+            b = [8] + [1] * len(metaData)
+            fig, axs = plt.subplots(nrows=len(metaData) + 1,
+                                    ncols=len(category) + 1,
+                                    figsize=figsize,
+                                    gridspec_kw={'width_ratios': width,
+                                                 'height_ratios': b},
+                                    facecolor='white')
 
         colors = self.colors_topics
 
         if ascending is None:
             ascending = [True] * len(category)
 
         for i in range(len(category)):
@@ -312,36 +321,36 @@
 
                 axs[0, i].xaxis.set_ticks([])
                 axs[0, i].set_title(category[i], fontsize=40)
                 axs[0, i].set_ylim(0, 1)
                 axs[0, i].set_xlim(0, a[i])
                 axs[0, 0].set_ylabel("Topic proportion", fontsize=25)
 
-            tissue = tissue[metaData]
-            tissue = tissue.reindex(tmp.index.tolist())
-            for j in range(len(metaData)):
-                if type(metaData_palette[metaData[j]]) == dict:
-                    tissue.replace(metaData_palette[metaData[j]], inplace=True)
+                tissue = tissue[metaData]
+                tissue = tissue.reindex(tmp.index.tolist())
+                for j in range(len(metaData)):
+                    if type(metaData_palette[metaData[j]]) == dict:
+                        tissue.replace(metaData_palette[metaData[j]], inplace=True)
+
+                x = [i for i in range(tmp.shape[0])]
+                y = np.repeat(3000, len(x))
+                for j in range(len(metaData)):
+                    color = tissue[metaData[j]].values
+                    if type(metaData_palette[metaData[j]]) == dict:
+                        axs[j + 1, i].scatter(x, y, label=metaData_palette[metaData[j]],
+                                              c=color, s=1000, marker="|", alpha=1,
+                                              linewidths=1)
+                    else:
+                        axs[j + 1, i].scatter(x, y, label=metaData_palette[metaData[j]],
+                                              c=color, cmap=metaData_palette[metaData[j]].get_cmap(), s=1000, marker="|",
+                                              alpha=1,
+                                              linewidths=1)
 
-            x = [i for i in range(tmp.shape[0])]
-            y = np.repeat(3000, len(x))
-            for j in range(len(metaData)):
-                color = tissue[metaData[j]].values
-                if type(metaData_palette[metaData[j]]) == dict:
-                    axs[j + 1, i].scatter(x, y, label=metaData_palette[metaData[j]],
-                                          c=color, s=1000, marker="|", alpha=1,
-                                          linewidths=1)
-                else:
-                    axs[j + 1, i].scatter(x, y, label=metaData_palette[metaData[j]],
-                                          c=color, cmap=metaData_palette[metaData[j]].get_cmap(), s=1000, marker="|",
-                                          alpha=1,
-                                          linewidths=1)
-
-                axs[j + 1, i].axis('off')
-                axs[j + 1, i].set_xlim(0, a[i])
+                    axs[j + 1, i].axis('off')
+                    axs[j + 1, i].set_xlim(0, a[i])
 
         colors = self.colors_topics
 
         handles = []
         for n in range(colors.shape[0]):
             patch = mpatches.Patch(color=colors.colors[n], label=colors.index[n])
             handles.append(patch)
@@ -354,32 +363,33 @@
             else:
                 axs[0, len(category)].legend(loc='center left',
                                              title='Topic',
                                              ncol=4,
                                              handles=handles)
                 axs[0, len(category)].axis('off')
 
-        for j in range(len(metaData)):
-            handles = []
-            if type(metaData_palette[metaData[j]]) == dict:
-                for met in metaData_palette[metaData[j]].keys():
-                    patch = mpatches.Patch(color=metaData_palette[metaData[j]][met], label=met)
-                    handles.append(patch)
-                    axs[j + 1, len(category)].legend(loc='center left',
-                                                     title=metaData[j].capitalize(),
-                                                     ncol=4,
-                                                     handles=handles)
+        if metaData is not None:
+            for j in range(len(metaData)):
+                handles = []
+                if type(metaData_palette[metaData[j]]) == dict:
+                    for met in metaData_palette[metaData[j]].keys():
+                        patch = mpatches.Patch(color=metaData_palette[metaData[j]][met], label=met)
+                        handles.append(patch)
+                        axs[j + 1, len(category)].legend(loc='center left',
+                                                         title=metaData[j].capitalize(),
+                                                         ncol=4,
+                                                         handles=handles)
+                        axs[j + 1, len(category)].axis('off')
+                else:
+                    clb = fig.colorbar(mappable=metaData_palette[metaData[j]],
+                                       ax=axs[j + 1, len(category)],
+                                       orientation='horizontal',
+                                       fraction=0.9)
+                    clb.ax.set_title(metaData[j].capitalize())
                     axs[j + 1, len(category)].axis('off')
-            else:
-                clb = fig.colorbar(mappable=metaData_palette[metaData[j]],
-                                   ax=axs[j + 1, len(category)],
-                                   orientation='horizontal',
-                                   fraction=0.9)
-                clb.ax.set_title(metaData[j].capitalize())
-                axs[j + 1, len(category)].axis('off')
 
         if save:
             fig.savefig(f"{file_name}.{file_format}")
         if show:
             plt.show()
         else:
             plt.close()
```

### Comparing `Topyfic-0.3.9/Topyfic/main.py` & `Topyfic-0.4.1/Topyfic/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import click
-from Topyfic.utils.analyseModel import *
 
 
 @click.group()
 def cli():
     pass
```

### Comparing `Topyfic-0.3.9/Topyfic/topModel.py` & `Topyfic-0.4.1/Topyfic/topModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import matplotlib.pyplot as plt
 import seaborn as sns
 
 sns.set_context('paper')
 warnings.filterwarnings('ignore')
 
 from Topyfic.topic import Topic
-from Topyfic.utils.analyseModel import MA_plot
+from Topyfic.utilsAnalyseModel import MA_plot
 
 
 class TopModel:
     """
     A class that saved a model
 
     :param name: name of class
@@ -244,61 +244,69 @@
             plt.show()
         else:
             plt.close()
 
     def MA_plot(self,
                 topic1,
                 topic2,
+                size=None,
                 pseudocount=1,
                 threshold=1,
                 cutoff=2,
                 consistency_correction=1.4826,
+                topN=None,
                 labels=None,
                 save=True,
                 show=True,
                 file_format="pdf",
                 file_name="MA_plot"):
         """
         plot MA based on the gene weights on given topics
 
         :param topic1: first topic to be compared
         :type topic1: str
         :param topic2: second topic to be compared
         :type topic2: str
+        :param size: table contains size of dot for each genes (genes are index)
+        :type size: pandas dataframe
         :param pseudocount: pseudocount that you want to add (default: 1)
         :type pseudocount: float
         :param threshold: threshold to filter genes based on A values (default: 1)
         :type threshold: float
         :param cutoff: cutoff for categorized genes by modified z-score (default: 2)
         :type cutoff: float
         :param consistency_correction: the factor converts the MAD to the standard deviation for a given distribution. The default value (1.4826) is the conversion factor if the underlying data is normally distributed
         :type consistency_correction: float
+        :param topN: number of genes to be consider for calculating z-score based on the A value (if it's none is gonna be avarage of # genes in both topics with weights above threshold
+        :type topN: int
         :param labels: list of gene names wish to show in MA-plot
         :type labels: list
         :param save: indicate if you want to save the plot or not (default: True)
         :type save: bool
         :param show: indicate if you want to show the plot or not (default: True)
         :type show: bool
         :param file_format: indicate the format of plot (default: pdf)
         :type file_format: str
         :param file_name: name and path of the plot use for save (default: MA_plot)
         :type file_name: str
 
         :return: return M and A values
         """
-        gene_weights = self.get_gene_weights()
+        gene_weights = self.get_gene_weights().copy(deep=True)
         topic1 = gene_weights[topic1]
         topic2 = gene_weights[topic2]
 
         gene_zscore = MA_plot(topic1,
                               topic2,
+                              size=size,
                               pseudocount=pseudocount,
                               threshold=threshold,
                               cutoff=cutoff,
                               consistency_correction=consistency_correction,
+                              topN=topN,
                               labels=labels,
                               save=save,
                               show=show,
                               file_format=file_format,
                               file_name=file_name)
 
         return gene_zscore
```

### Comparing `Topyfic-0.3.9/Topyfic/topic.py` & `Topyfic-0.4.1/Topyfic/topic.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import seaborn as sns
 
 sns.set_context('paper')
 
 warnings.filterwarnings('ignore')
 
-from Topyfic.utils.analyseModel import GSEA, functional_enrichment_analysis
+from Topyfic.utilsAnalyseModel import GSEA, functional_enrichment_analysis
 
 
 class Topic:
     """
     A class saved topic along with other useful information
 
     :param topic_id: ID of topic which is unique
```

### Comparing `Topyfic-0.3.9/Topyfic/train.py` & `Topyfic-0.4.1/Topyfic/train.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.3.9/Topyfic.egg-info/PKG-INFO` & `Topyfic-0.4.1/Topyfic.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Topyfic
-Version: 0.3.9
+Version: 0.4.1
 Summary: Topyfic is a Python package designed to identify reproducible latent dirichlet allocation (LDA) using leiden clustering and harmony for single cell epigenomics data
 Home-page: https://github.com/mortazavilab/Topyfic
-Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.3.9.tar.gz
+Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.4.1.tar.gz
 Author: Narges Rezaie
 Author-email: nargesrezaie80@gmail.com
 License: MIT
 Keywords: Cellular Programs,Latent Dirichlet allocation,single-cell multiome,single-cell RNA-seq,gene regulatory network,Topic Modeling,single-nucleus RNA-seq
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research 
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `Topyfic-0.3.9/setup.py` & `Topyfic-0.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 setup(
     name='Topyfic',  # the name of your package
     packages=['Topyfic'],  # same as above
-    version='v0.3.9',  # version number
+    version='v0.4.1',  # version number
     license='MIT',  # license type
     description='Topyfic is a Python package designed to identify reproducible latent dirichlet allocation (LDA) '
                 'using leiden clustering and harmony for single cell epigenomics data',
     # short description
     author='Narges Rezaie',  # your name
     author_email='nargesrezaie80@gmail.com',  # your email
     url='https://github.com/mortazavilab/Topyfic',  # url to your git repo
-    download_url='https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.3.9.tar.gz',  # link to the tar.gz file associated with this release
+    download_url='https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.4.1.tar.gz',  # link to the tar.gz file associated with this release
     keywords=['Cellular Programs', 'Latent Dirichlet allocation', 'single-cell multiome', 'single-cell RNA-seq',
               'gene regulatory network', 'Topic Modeling', 'single-nucleus RNA-seq'],  #
     python_requires='>=3.8',
     install_requires=[  # these can also include >, <, == to enforce version compatibility
         'pandas>=1.4.4',  # make sure the packages you put here are those NOT included in the base python distribution
         'scikit-learn>=0.24.2',
         'pytest',
@@ -30,14 +30,15 @@
         'numpy>=1.23.2',
         'reactome2py>=3.0.0',
         'scanpy>=1.9.3',
         'scikit_learn>=1.2.2',
         'scipy>=1.9.1',
         'seaborn>=0.11.2',
         'statsmodels>=0.13.5',
+        'adjustText'
         #'harmonypy'
 
     ],
     classifiers=[  # choose from here: https://pypi.org/classifiers/
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research ',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
```


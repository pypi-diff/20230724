# Comparing `tmp/clfutils4r-0.0.2.tar.gz` & `tmp/clfutils4r-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clfutils4r-0.0.2.tar", last modified: Mon Jul 24 04:46:37 2023, max compression
+gzip compressed data, was "clfutils4r-0.0.3.tar", last modified: Mon Jul 24 04:56:10 2023, max compression
```

## Comparing `clfutils4r-0.0.2.tar` & `clfutils4r-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-24 04:46:37.453830 clfutils4r-0.0.2/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2022-07-24 06:54:15.000000 clfutils4r-0.0.2/LICENSE
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     6027 2023-07-24 04:46:37.453830 clfutils4r-0.0.2/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     5383 2023-07-17 04:00:59.000000 clfutils4r-0.0.2/README.md
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      673 2023-07-24 04:45:50.000000 clfutils4r-0.0.2/pyproject.toml
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2023-07-24 04:46:37.453830 clfutils4r-0.0.2/setup.cfg
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     1001 2023-07-24 04:46:00.000000 clfutils4r-0.0.2/setup.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-24 04:46:37.453830 clfutils4r-0.0.2/src/
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-24 04:46:37.453830 clfutils4r-0.0.2/src/clfutils4r/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2022-07-24 06:54:15.000000 clfutils4r-0.0.2/src/clfutils4r/__init__.py
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    19956 2023-07-24 04:40:58.000000 clfutils4r-0.0.2/src/clfutils4r/eval_classification.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-24 04:46:37.453830 clfutils4r-0.0.2/src/clfutils4r.egg-info/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     6027 2023-07-24 04:46:37.000000 clfutils4r-0.0.2/src/clfutils4r.egg-info/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      295 2023-07-24 04:46:37.000000 clfutils4r-0.0.2/src/clfutils4r.egg-info/SOURCES.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2023-07-24 04:46:37.000000 clfutils4r-0.0.2/src/clfutils4r.egg-info/dependency_links.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       50 2023-07-24 04:46:37.000000 clfutils4r-0.0.2/src/clfutils4r.egg-info/requires.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       11 2023-07-24 04:46:37.000000 clfutils4r-0.0.2/src/clfutils4r.egg-info/top_level.txt
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-24 04:56:10.970357 clfutils4r-0.0.3/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2022-07-24 06:54:15.000000 clfutils4r-0.0.3/LICENSE
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     6114 2023-07-24 04:56:10.970357 clfutils4r-0.0.3/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     5470 2023-07-24 04:53:33.000000 clfutils4r-0.0.3/README.md
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      673 2023-07-24 04:54:12.000000 clfutils4r-0.0.3/pyproject.toml
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2023-07-24 04:56:10.970357 clfutils4r-0.0.3/setup.cfg
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     1001 2023-07-24 04:54:18.000000 clfutils4r-0.0.3/setup.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-24 04:56:10.966357 clfutils4r-0.0.3/src/
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-24 04:56:10.970357 clfutils4r-0.0.3/src/clfutils4r/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2022-07-24 06:54:15.000000 clfutils4r-0.0.3/src/clfutils4r/__init__.py
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    19989 2023-07-24 04:53:38.000000 clfutils4r-0.0.3/src/clfutils4r/eval_classification.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-24 04:56:10.970357 clfutils4r-0.0.3/src/clfutils4r.egg-info/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     6114 2023-07-24 04:56:10.000000 clfutils4r-0.0.3/src/clfutils4r.egg-info/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      295 2023-07-24 04:56:10.000000 clfutils4r-0.0.3/src/clfutils4r.egg-info/SOURCES.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2023-07-24 04:56:10.000000 clfutils4r-0.0.3/src/clfutils4r.egg-info/dependency_links.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       50 2023-07-24 04:56:10.000000 clfutils4r-0.0.3/src/clfutils4r.egg-info/requires.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       11 2023-07-24 04:56:10.000000 clfutils4r-0.0.3/src/clfutils4r.egg-info/top_level.txt
```

### Comparing `clfutils4r-0.0.2/LICENSE` & `clfutils4r-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clfutils4r-0.0.2/PKG-INFO` & `clfutils4r-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clfutils4r
-Version: 0.0.2
+Version: 0.0.3
 Summary: Wrapper around some basic sklearn and scikit-plot utilities for classification.
 Home-page: https://github.com/rutujagurav/clfutils4r
 Author: Rutuja Gurav
 Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
 Project-URL: Homepage, https://github.com/rutujagurav/clfutils4r
 Project-URL: Bug Tracker, https://github.com/rutujagurav/clfutils4r/issues
 Classifier: Programming Language :: Python :: 3
@@ -112,49 +112,50 @@
 y_pred_proba = model.predict_proba(X_test)
 
 eval_classification(untrained_model=DecisionTreeClassifier().set_params(**model_params), 
                     n_splits=5, class_names=class_names, 
                     X=X, y=y, 
                     make_shap_plot=True, trained_model=model, X_train=X_train, X_test=X_test,
                     y_test=y_test, y_pred=y_pred, y_pred_proba=y_pred_proba, 
+                    titlestr="Breast Cancer Detection using Decision Tree Classifier",
                     show=True, save=True, RESULTS_DIR=os.getcwd()+'/results')
 
 ```
 <!-- ### Confusion Matrix -->
-<!-- ![cm](tests/example_classification/results/confusion_matrix.png) -->
-![cm](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/confusion_matrix.png)
+![cm](tests/example_classification/results/confusion_matrix.png)
+<!-- ![cm](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/confusion_matrix.png) -->
 
 <!-- ### Class-wise ROC curve -->
-<!-- ![roc](tests/example_classification/results/classwise_roc_curve.png) -->
-![roc](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/classwise_roc_curve.png)
+![roc](tests/example_classification/results/classwise_roc_curve.png)
+<!-- ![roc](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/classwise_roc_curve.png) -->
 
 <!-- ### Class-wise PR curve -->
-<!-- ![pr](tests/example_classification/results/classwise_pr_curve.png) -->
-![pr](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/classwise_pr_curve.png)
+![pr](tests/example_classification/results/classwise_pr_curve.png)
+<!-- ![pr](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/classwise_pr_curve.png) -->
 
 <!-- ### KS statistic  -->
-<!-- ![ks_stat](tests/example_classification/results/ks_stat.png) -->
-![ks_stat](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/ks_stat.png)
+![ks_stat](tests/example_classification/results/ks_stat.png)
+<!-- ![ks_stat](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/ks_stat.png) -->
 
 <!-- ### Lift Curve  -->
-<!-- ![lift](tests/example_classification/results/lift_curve.png) -->
-![lift](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/lift_curve.png)
+![lift](tests/example_classification/results/lift_curve.png)
+<!-- ![lift](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/lift_curve.png) -->
 
 <!-- ### Cumulative Gain Curve  -->
-<!-- ![lift](tests/example_classification/results/cumul_gain.png) -->
-![lift](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/cumul_gain.png)
+![lift](tests/example_classification/results/cumul_gain.png)
+<!-- ![lift](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/cumul_gain.png) -->
 
 <!-- ### Cross-validated ROC curves -->
-<!-- ![cv_roc](tests/example_classification/results/crossvalidation_roc_curve.png) -->
-![cv_roc](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/crossvalidation_roc_curve.png)
+![cv_roc](tests/example_classification/results/crossvalidation_roc_curve.png)
+<!-- ![cv_roc](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/crossvalidation_roc_curve.png) -->
 
 <!-- ### Cross-validated PR curves -->
-<!-- ![cv_pr](tests/example_classification/results/crossvalidation_pr_curve.png) -->
-![cv_pr](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/crossvalidation_pr_curve.png)
+![cv_pr](tests/example_classification/results/crossvalidation_pr_curve.png)
+<!-- ![cv_pr](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/crossvalidation_pr_curve.png) -->
 
 <!-- ### Shapley Analysis Summary Plot -->
-<!-- ![shap](tests/example_classification/results/shap_summary_plot.png) -->
-![shap](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/shap_summary_plot.png)
+![shap](tests/example_classification/results/shap_summary_plot.png)
+<!-- ![shap](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/shap_summary_plot.png) -->
 
 
 ## Developer Notes:
 This package is the updated version of `bcutils4r` which supported only binary classification. `bcutils4r` is now defunct.
```

### Comparing `clfutils4r-0.0.2/README.md` & `clfutils4r-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -96,49 +96,50 @@
 y_pred_proba = model.predict_proba(X_test)
 
 eval_classification(untrained_model=DecisionTreeClassifier().set_params(**model_params), 
                     n_splits=5, class_names=class_names, 
                     X=X, y=y, 
                     make_shap_plot=True, trained_model=model, X_train=X_train, X_test=X_test,
                     y_test=y_test, y_pred=y_pred, y_pred_proba=y_pred_proba, 
+                    titlestr="Breast Cancer Detection using Decision Tree Classifier",
                     show=True, save=True, RESULTS_DIR=os.getcwd()+'/results')
 
 ```
 <!-- ### Confusion Matrix -->
-<!-- ![cm](tests/example_classification/results/confusion_matrix.png) -->
-![cm](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/confusion_matrix.png)
+![cm](tests/example_classification/results/confusion_matrix.png)
+<!-- ![cm](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/confusion_matrix.png) -->
 
 <!-- ### Class-wise ROC curve -->
-<!-- ![roc](tests/example_classification/results/classwise_roc_curve.png) -->
-![roc](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/classwise_roc_curve.png)
+![roc](tests/example_classification/results/classwise_roc_curve.png)
+<!-- ![roc](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/classwise_roc_curve.png) -->
 
 <!-- ### Class-wise PR curve -->
-<!-- ![pr](tests/example_classification/results/classwise_pr_curve.png) -->
-![pr](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/classwise_pr_curve.png)
+![pr](tests/example_classification/results/classwise_pr_curve.png)
+<!-- ![pr](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/classwise_pr_curve.png) -->
 
 <!-- ### KS statistic  -->
-<!-- ![ks_stat](tests/example_classification/results/ks_stat.png) -->
-![ks_stat](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/ks_stat.png)
+![ks_stat](tests/example_classification/results/ks_stat.png)
+<!-- ![ks_stat](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/ks_stat.png) -->
 
 <!-- ### Lift Curve  -->
-<!-- ![lift](tests/example_classification/results/lift_curve.png) -->
-![lift](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/lift_curve.png)
+![lift](tests/example_classification/results/lift_curve.png)
+<!-- ![lift](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/lift_curve.png) -->
 
 <!-- ### Cumulative Gain Curve  -->
-<!-- ![lift](tests/example_classification/results/cumul_gain.png) -->
-![lift](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/cumul_gain.png)
+![lift](tests/example_classification/results/cumul_gain.png)
+<!-- ![lift](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/cumul_gain.png) -->
 
 <!-- ### Cross-validated ROC curves -->
-<!-- ![cv_roc](tests/example_classification/results/crossvalidation_roc_curve.png) -->
-![cv_roc](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/crossvalidation_roc_curve.png)
+![cv_roc](tests/example_classification/results/crossvalidation_roc_curve.png)
+<!-- ![cv_roc](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/crossvalidation_roc_curve.png) -->
 
 <!-- ### Cross-validated PR curves -->
-<!-- ![cv_pr](tests/example_classification/results/crossvalidation_pr_curve.png) -->
-![cv_pr](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/crossvalidation_pr_curve.png)
+![cv_pr](tests/example_classification/results/crossvalidation_pr_curve.png)
+<!-- ![cv_pr](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/crossvalidation_pr_curve.png) -->
 
 <!-- ### Shapley Analysis Summary Plot -->
-<!-- ![shap](tests/example_classification/results/shap_summary_plot.png) -->
-![shap](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/shap_summary_plot.png)
+![shap](tests/example_classification/results/shap_summary_plot.png)
+<!-- ![shap](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/shap_summary_plot.png) -->
 
 
 ## Developer Notes:
 This package is the updated version of `bcutils4r` which supported only binary classification. `bcutils4r` is now defunct.
```

### Comparing `clfutils4r-0.0.2/pyproject.toml` & `clfutils4r-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clfutils4r"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Rutuja Gurav", email="rutujagurav100@gmail.com" },
 ]
 description = "Wrapper around some basic sklearn and scikit-plot utilities for classification."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers=[
```

### Comparing `clfutils4r-0.0.2/setup.py` & `clfutils4r-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="clfutils4r", # Replace with your own username
-    version="0.0.2",
+    version="0.0.3",
     author="Rutuja Gurav",
     author_email="rutujagurav100@gmail.com",
     description="Wrapper around some basic sklearn and scikit-plot utilities for classification.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rutujagurav/clfutils4r",
     project_urls={
```

### Comparing `clfutils4r-0.0.2/src/clfutils4r/eval_classification.py` & `clfutils4r-0.0.3/src/clfutils4r/eval_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,19 +48,19 @@
     ax1.set(ylim=(0, 1))
 
     ax1.set_ylabel('precision', color='b')
     ax2 = ax1.twinx()
     ax1.plot(pct_above_per_thresh, recall_curve, 'r')
     ax2.set_ylabel('recall', color='r')
     plt.title('Precision Recall Curve')
-    if(show):
-        plt.show()
+    
     if(save):
         plt.savefig(RESULTS_DIR+'/precision_recall_curve.png', bbox_inches='tight',dpi=dpi)
-
+    if(show):
+        plt.show()
     plt.close()
 
 @deprecated
 def plot_ROC_curve(y_test=None, y_pred=None, RESULTS_DIR='', show=False, save=False, dpi=300):
     fpr,tpr,thresholds = roc_curve(y_test,y_pred)
     roc_auc = auc(fpr,tpr)
     plt.clf()
@@ -68,19 +68,19 @@
     plt.plot(fpr,tpr,'b',label='AUC = %0.2f' %roc_auc)
     plt.legend(loc='lower right')
     plt.plot([0,1],[0,1],'r--')
     plt.xlim([0,1])
     plt.ylim([0,1])
     plt.ylabel('True Positive Rate')
     plt.xlabel('False Positive Rate')
-    if(show):
-        plt.show()
+    
     if(save):
         plt.savefig(RESULTS_DIR+'/roc_curve.png', bbox_inches='tight',dpi=dpi)
-
+    if(show):
+        plt.show()
     plt.close()
 
 def plot_confusion_matrix(y_test=None, y_pred=None, labels=[], threshold = 0.5, RESULTS_DIR='', titlestr='', show=False, save=False, dpi=300):
     """
     Returns a matplotlib figure containing the plotted confusion matrix.
     
     Args:
@@ -132,108 +132,108 @@
     # ax.set_xlabel('Predicted Label', fontsize=15)
 
     s.set_ylabel('True Label') #, fontsize=15
     s.set_xlabel('Predicted Label')
     
     plt.title(titlestr+"Confusion Matrix")
     plt.tight_layout()
-    if show:
-        plt.show()
+    
     if save:
         plt.savefig(RESULTS_DIR+'/confusion_matrix.png', bbox_inches='tight',dpi=dpi)
-
+    if show:
+        plt.show()
     plt.close()
         
 def plot_ks_stat(y_test=None, y_pred=None, titlestr='', RESULTS_DIR='', show=False, save=False, dpi=300):
     fig, ax = plt.subplots()
     ax = scikitplot.metrics.plot_ks_statistic(y_test, y_pred, ax=ax)
     ax.set_xlim([-0.05, 1.05])
     ax.set_ylim([-0.05, 1.05])
     ax.set_facecolor('white')
     for l in ax.lines:
         l.set_lw(2)
     plt.title(titlestr+"KS Statistic Plot ")
     plt.grid()
     plt.legend(loc='best')
     plt.tight_layout()
-    if show:
-        plt.show()
+    
     if save:
         plt.savefig(RESULTS_DIR+'/ks_stat.png', bbox_inches='tight',dpi=dpi)
-
+    if show:
+        plt.show()
     plt.close()
 
 def plot_lift_curve(y_test=None, y_pred=None, titlestr='', RESULTS_DIR='', show=False, save=False, dpi=300):
     fig, ax = plt.subplots()
     ax = scikitplot.metrics.plot_lift_curve(y_test, y_pred, ax=ax)
     ax.set_facecolor('white')
     for l in ax.lines:
         l.set_lw(2)
     plt.title(titlestr+"Lift Curve ")
     # plt.grid()
     plt.legend(loc='best')
     plt.tight_layout()
-    if show:
-        plt.show()
+    
     if save:
         plt.savefig(RESULTS_DIR+'/lift_curve.png', bbox_inches='tight',dpi=dpi)
-    
+    if show:
+        plt.show()
     plt.close()
 
 def plot_cumul_gain(y_test=None, y_pred=None, titlestr='', RESULTS_DIR='', show=False, save=False, dpi=300):
     fig, ax = plt.subplots()
     ax = scikitplot.metrics.plot_cumulative_gain(y_test, y_pred, ax=ax)
     ax.set_facecolor('white')
     for l in ax.lines:
         l.set_lw(2)
     plt.title(titlestr+"Cumulative Gains Curve ")
     # plt.grid()
     plt.legend(loc='best')
     plt.tight_layout()
-    if show:
-        plt.show()
+    
     if save:
         plt.savefig(RESULTS_DIR+'/cumul_gain.png', bbox_inches='tight',dpi=dpi)
-    
+    if show:
+        plt.show()
     plt.close()
 
 def plot_classwise_pr_curve(y_test=None, y_pred=None, titlestr='', RESULTS_DIR='', show=False, save=False, dpi=300):
     fig, ax = plt.subplots()
     ax = scikitplot.metrics.plot_precision_recall(y_test, y_pred, ax=ax)
     ax.set_xlim([-0.05, 1.05])
     ax.set_ylim([-0.05, 1.05])
     ax.set_facecolor('white')
     for l in ax.lines:
         l.set_lw(2)
     plt.title(titlestr+"Precision-Recall Curve ")
     plt.grid()
     plt.tight_layout()
-    if show:
-        plt.show()
+    
     if save:
         plt.savefig(RESULTS_DIR+'/classwise_pr_curve.png', bbox_inches='tight',dpi=dpi)
-    
+    if show:
+        plt.show()
     plt.close()
 
 def plot_classwise_roc_curve(y_test=None, y_pred=None, titlestr='', RESULTS_DIR='', show=False, save=False, dpi=300):
     fig, ax = plt.subplots()
     ax = scikitplot.metrics.plot_roc(y_test, y_pred, ax=ax)
     ax.set_xlim([-0.05, 1.05])
     ax.set_ylim([-0.05, 1.05])
     ax.set_facecolor('white')
     for l in ax.lines:
         l.set_lw(2)
     plt.title(titlestr+"ROC Curves ")
     plt.grid()
     plt.tight_layout()
-    if show:
-        plt.show()
+    
     if save:
         plt.savefig(RESULTS_DIR+'/classwise_roc_curve.png', bbox_inches='tight', dpi=dpi)
- 
+    if show:
+        plt.show()
     plt.close()
 
 def generate_classification_report(y_test=None, y_pred=None, labels=[], RESULTS_DIR='', show=False, save=False):
     if(len(labels) !=0):
         report = classification_report(y_test, 
                                         y_pred, 
                                         target_names=[cl+'(class '+str(i)+')' for i, cl in enumerate(labels)], 
@@ -297,19 +297,19 @@
     plt.ylim([-0.05, 1.05])
     plt.xlabel('False Positive Rate')
     plt.ylabel('True Positive Rate')
     plt.title(titlestr+'Cross-Validated ROC Curve')
     plt.legend(bbox_to_anchor=(1, 1))
     # plt.tight_layout()
     plt.grid()
-    if(show):
-        plt.show()
+    
     if(save):
         plt.savefig(RESULTS_DIR+'/crossvalidation_roc_curve.png', bbox_inches='tight',dpi=dpi)
-
+    if(show):
+        plt.show()
     plt.close()
 
 def plot_cv_pr_curve(classifier=None, cv=None, n_splits=10, X=None, y=None, RESULTS_DIR='', titlestr='', show=False, save=False, dpi=300):
     """
     Draw a Cross Validated PR Curve.
     Keyword Args:
         classifier: Classifier Object
@@ -350,32 +350,34 @@
     plt.ylim([-0.05, 1.05])
     plt.xlabel('Recall')
     plt.ylabel('Precision')
     plt.title(titlestr+'Cross-Validated PR Curve')
     plt.legend(bbox_to_anchor=(1, 1))
     # plt.tight_layout()
     plt.grid()
-    if show:
-        plt.show()
+    
     if save:
         plt.savefig(RESULTS_DIR+'/crossvalidation_pr_curve.png', bbox_inches='tight',dpi=dpi)   
+    if show:
+        plt.show()
     plt.close()
 
 def plot_shap_summary(model=None, nsamples=50, X_train=None, X_test=None, titlestr='', show=False, save=False, RESULTS_DIR=None):
     print("No. of samples used to build explainer and generate shap values: ", nsamples)
     explainer = shap.KernelExplainer(model.predict, shap.sample(X_train, nsamples))
     shap_values = explainer.shap_values(X=X_test, nsamples=nsamples)
     shap.summary_plot(shap_values=shap_values, features=X_test, show=False)
     # shap.plots.violin(shap_values=shap_values, features=X_test, plot_type="layered_violin", show=False)
     plt.title(titlestr+'Shapley Analysis')
     plt.tight_layout()
-    if show:
-        plt.show()
+    
     if save:
         plt.savefig(RESULTS_DIR+'/shap_summary_plot.png', bbox_inches='tight',dpi=dpi)   
+    if show:
+        plt.show()
 
     plt.close()
     
 def eval_classification(untrained_model=None, n_splits=10,
                         X=None, y=None, 
                         make_shap_plot=False, trained_model=None, X_train=None, X_test=None, 
                         y_train=None, y_test=None, y_pred=None, y_pred_proba=None,
```

### Comparing `clfutils4r-0.0.2/src/clfutils4r.egg-info/PKG-INFO` & `clfutils4r-0.0.3/src/clfutils4r.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clfutils4r
-Version: 0.0.2
+Version: 0.0.3
 Summary: Wrapper around some basic sklearn and scikit-plot utilities for classification.
 Home-page: https://github.com/rutujagurav/clfutils4r
 Author: Rutuja Gurav
 Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
 Project-URL: Homepage, https://github.com/rutujagurav/clfutils4r
 Project-URL: Bug Tracker, https://github.com/rutujagurav/clfutils4r/issues
 Classifier: Programming Language :: Python :: 3
@@ -112,49 +112,50 @@
 y_pred_proba = model.predict_proba(X_test)
 
 eval_classification(untrained_model=DecisionTreeClassifier().set_params(**model_params), 
                     n_splits=5, class_names=class_names, 
                     X=X, y=y, 
                     make_shap_plot=True, trained_model=model, X_train=X_train, X_test=X_test,
                     y_test=y_test, y_pred=y_pred, y_pred_proba=y_pred_proba, 
+                    titlestr="Breast Cancer Detection using Decision Tree Classifier",
                     show=True, save=True, RESULTS_DIR=os.getcwd()+'/results')
 
 ```
 <!-- ### Confusion Matrix -->
-<!-- ![cm](tests/example_classification/results/confusion_matrix.png) -->
-![cm](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/confusion_matrix.png)
+![cm](tests/example_classification/results/confusion_matrix.png)
+<!-- ![cm](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/confusion_matrix.png) -->
 
 <!-- ### Class-wise ROC curve -->
-<!-- ![roc](tests/example_classification/results/classwise_roc_curve.png) -->
-![roc](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/classwise_roc_curve.png)
+![roc](tests/example_classification/results/classwise_roc_curve.png)
+<!-- ![roc](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/classwise_roc_curve.png) -->
 
 <!-- ### Class-wise PR curve -->
-<!-- ![pr](tests/example_classification/results/classwise_pr_curve.png) -->
-![pr](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/classwise_pr_curve.png)
+![pr](tests/example_classification/results/classwise_pr_curve.png)
+<!-- ![pr](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/classwise_pr_curve.png) -->
 
 <!-- ### KS statistic  -->
-<!-- ![ks_stat](tests/example_classification/results/ks_stat.png) -->
-![ks_stat](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/ks_stat.png)
+![ks_stat](tests/example_classification/results/ks_stat.png)
+<!-- ![ks_stat](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/ks_stat.png) -->
 
 <!-- ### Lift Curve  -->
-<!-- ![lift](tests/example_classification/results/lift_curve.png) -->
-![lift](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/lift_curve.png)
+![lift](tests/example_classification/results/lift_curve.png)
+<!-- ![lift](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/lift_curve.png) -->
 
 <!-- ### Cumulative Gain Curve  -->
-<!-- ![lift](tests/example_classification/results/cumul_gain.png) -->
-![lift](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/cumul_gain.png)
+![lift](tests/example_classification/results/cumul_gain.png)
+<!-- ![lift](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/cumul_gain.png) -->
 
 <!-- ### Cross-validated ROC curves -->
-<!-- ![cv_roc](tests/example_classification/results/crossvalidation_roc_curve.png) -->
-![cv_roc](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/crossvalidation_roc_curve.png)
+![cv_roc](tests/example_classification/results/crossvalidation_roc_curve.png)
+<!-- ![cv_roc](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/crossvalidation_roc_curve.png) -->
 
 <!-- ### Cross-validated PR curves -->
-<!-- ![cv_pr](tests/example_classification/results/crossvalidation_pr_curve.png) -->
-![cv_pr](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/crossvalidation_pr_curve.png)
+![cv_pr](tests/example_classification/results/crossvalidation_pr_curve.png)
+<!-- ![cv_pr](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/crossvalidation_pr_curve.png) -->
 
 <!-- ### Shapley Analysis Summary Plot -->
-<!-- ![shap](tests/example_classification/results/shap_summary_plot.png) -->
-![shap](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/shap_summary_plot.png)
+![shap](tests/example_classification/results/shap_summary_plot.png)
+<!-- ![shap](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/shap_summary_plot.png) -->
 
 
 ## Developer Notes:
 This package is the updated version of `bcutils4r` which supported only binary classification. `bcutils4r` is now defunct.
```


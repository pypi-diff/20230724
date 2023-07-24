# Comparing `tmp/clfutils4r-0.0.1.tar.gz` & `tmp/clfutils4r-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clfutils4r-0.0.1.tar", last modified: Mon Jul 17 03:56:33 2023, max compression
+gzip compressed data, was "clfutils4r-0.0.2.tar", last modified: Mon Jul 24 04:46:37 2023, max compression
```

## Comparing `clfutils4r-0.0.1.tar` & `clfutils4r-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-17 03:56:33.212237 clfutils4r-0.0.1/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2022-07-24 06:54:15.000000 clfutils4r-0.0.1/LICENSE
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     5882 2023-07-17 03:56:33.212237 clfutils4r-0.0.1/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     5238 2023-07-17 03:55:20.000000 clfutils4r-0.0.1/README.md
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      673 2023-07-17 03:32:05.000000 clfutils4r-0.0.1/pyproject.toml
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2023-07-17 03:56:33.212237 clfutils4r-0.0.1/setup.cfg
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     1001 2023-07-17 03:55:58.000000 clfutils4r-0.0.1/setup.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-17 03:56:33.208237 clfutils4r-0.0.1/src/
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-17 03:56:33.208237 clfutils4r-0.0.1/src/clfutils4r/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2022-07-24 06:54:15.000000 clfutils4r-0.0.1/src/clfutils4r/__init__.py
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    19538 2023-07-17 03:47:23.000000 clfutils4r-0.0.1/src/clfutils4r/eval_classification.py
-drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-17 03:56:33.208237 clfutils4r-0.0.1/src/clfutils4r.egg-info/
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     5882 2023-07-17 03:56:33.000000 clfutils4r-0.0.1/src/clfutils4r.egg-info/PKG-INFO
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      295 2023-07-17 03:56:33.000000 clfutils4r-0.0.1/src/clfutils4r.egg-info/SOURCES.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2023-07-17 03:56:33.000000 clfutils4r-0.0.1/src/clfutils4r.egg-info/dependency_links.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       50 2023-07-17 03:56:33.000000 clfutils4r-0.0.1/src/clfutils4r.egg-info/requires.txt
--rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       11 2023-07-17 03:56:33.000000 clfutils4r-0.0.1/src/clfutils4r.egg-info/top_level.txt
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-24 04:46:37.453830 clfutils4r-0.0.2/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    35128 2022-07-24 06:54:15.000000 clfutils4r-0.0.2/LICENSE
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     6027 2023-07-24 04:46:37.453830 clfutils4r-0.0.2/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     5383 2023-07-17 04:00:59.000000 clfutils4r-0.0.2/README.md
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      673 2023-07-24 04:45:50.000000 clfutils4r-0.0.2/pyproject.toml
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       38 2023-07-24 04:46:37.453830 clfutils4r-0.0.2/setup.cfg
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     1001 2023-07-24 04:46:00.000000 clfutils4r-0.0.2/setup.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-24 04:46:37.453830 clfutils4r-0.0.2/src/
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-24 04:46:37.453830 clfutils4r-0.0.2/src/clfutils4r/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        0 2022-07-24 06:54:15.000000 clfutils4r-0.0.2/src/clfutils4r/__init__.py
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)    19956 2023-07-24 04:40:58.000000 clfutils4r-0.0.2/src/clfutils4r/eval_classification.py
+drwxrwxr-x   0 rgura001 (52843) rgura001 (52843)        0 2023-07-24 04:46:37.453830 clfutils4r-0.0.2/src/clfutils4r.egg-info/
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)     6027 2023-07-24 04:46:37.000000 clfutils4r-0.0.2/src/clfutils4r.egg-info/PKG-INFO
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)      295 2023-07-24 04:46:37.000000 clfutils4r-0.0.2/src/clfutils4r.egg-info/SOURCES.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)        1 2023-07-24 04:46:37.000000 clfutils4r-0.0.2/src/clfutils4r.egg-info/dependency_links.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       50 2023-07-24 04:46:37.000000 clfutils4r-0.0.2/src/clfutils4r.egg-info/requires.txt
+-rw-rw-r--   0 rgura001 (52843) rgura001 (52843)       11 2023-07-24 04:46:37.000000 clfutils4r-0.0.2/src/clfutils4r.egg-info/top_level.txt
```

### Comparing `clfutils4r-0.0.1/LICENSE` & `clfutils4r-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clfutils4r-0.0.1/PKG-INFO` & `clfutils4r-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clfutils4r
-Version: 0.0.1
+Version: 0.0.2
 Summary: Wrapper around some basic sklearn and scikit-plot utilities for classification.
 Home-page: https://github.com/rutujagurav/clfutils4r
 Author: Rutuja Gurav
 Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
 Project-URL: Homepage, https://github.com/rutujagurav/clfutils4r
 Project-URL: Bug Tracker, https://github.com/rutujagurav/clfutils4r/issues
 Classifier: Programming Language :: Python :: 3
@@ -150,7 +150,11 @@
 <!-- ### Cross-validated PR curves -->
 <!-- ![cv_pr](tests/example_classification/results/crossvalidation_pr_curve.png) -->
 ![cv_pr](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/crossvalidation_pr_curve.png)
 
 <!-- ### Shapley Analysis Summary Plot -->
 <!-- ![shap](tests/example_classification/results/shap_summary_plot.png) -->
 ![shap](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/shap_summary_plot.png)
+
+
+## Developer Notes:
+This package is the updated version of `bcutils4r` which supported only binary classification. `bcutils4r` is now defunct.
```

### Comparing `clfutils4r-0.0.1/README.md` & `clfutils4r-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -133,8 +133,12 @@
 
 <!-- ### Cross-validated PR curves -->
 <!-- ![cv_pr](tests/example_classification/results/crossvalidation_pr_curve.png) -->
 ![cv_pr](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/crossvalidation_pr_curve.png)
 
 <!-- ### Shapley Analysis Summary Plot -->
 <!-- ![shap](tests/example_classification/results/shap_summary_plot.png) -->
-![shap](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/shap_summary_plot.png)
+![shap](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/shap_summary_plot.png)
+
+
+## Developer Notes:
+This package is the updated version of `bcutils4r` which supported only binary classification. `bcutils4r` is now defunct.
```

### Comparing `clfutils4r-0.0.1/pyproject.toml` & `clfutils4r-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clfutils4r"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Rutuja Gurav", email="rutujagurav100@gmail.com" },
 ]
 description = "Wrapper around some basic sklearn and scikit-plot utilities for classification."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers=[
```

### Comparing `clfutils4r-0.0.1/setup.py` & `clfutils4r-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="clfutils4r", # Replace with your own username
-    version="0.0.1",
+    version="0.0.2",
     author="Rutuja Gurav",
     author_email="rutujagurav100@gmail.com",
     description="Wrapper around some basic sklearn and scikit-plot utilities for classification.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rutujagurav/clfutils4r",
     project_urls={
```

### Comparing `clfutils4r-0.0.1/src/clfutils4r/eval_classification.py` & `clfutils4r-0.0.2/src/clfutils4r/eval_classification.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,19 +48,19 @@
     ax1.set(ylim=(0, 1))
 
     ax1.set_ylabel('precision', color='b')
     ax2 = ax1.twinx()
     ax1.plot(pct_above_per_thresh, recall_curve, 'r')
     ax2.set_ylabel('recall', color='r')
     plt.title('Precision Recall Curve')
-    
-    if(save):
-        plt.savefig(RESULTS_DIR+'/precision_recall_curve.png', bbox_inches='tight',dpi=dpi)
     if(show):
         plt.show()
+    if(save):
+        plt.savefig(RESULTS_DIR+'/precision_recall_curve.png', bbox_inches='tight',dpi=dpi)
+
     plt.close()
 
 @deprecated
 def plot_ROC_curve(y_test=None, y_pred=None, RESULTS_DIR='', show=False, save=False, dpi=300):
     fpr,tpr,thresholds = roc_curve(y_test,y_pred)
     roc_auc = auc(fpr,tpr)
     plt.clf()
@@ -68,21 +68,22 @@
     plt.plot(fpr,tpr,'b',label='AUC = %0.2f' %roc_auc)
     plt.legend(loc='lower right')
     plt.plot([0,1],[0,1],'r--')
     plt.xlim([0,1])
     plt.ylim([0,1])
     plt.ylabel('True Positive Rate')
     plt.xlabel('False Positive Rate')
-    if(save):
-        plt.savefig(RESULTS_DIR+'/roc_curve.png', bbox_inches='tight',dpi=dpi)
     if(show):
         plt.show()
+    if(save):
+        plt.savefig(RESULTS_DIR+'/roc_curve.png', bbox_inches='tight',dpi=dpi)
+
     plt.close()
 
-def plot_confusion_matrix(y_test=None, y_pred=None, RESULTS_DIR='', labels=[], threshold = 0.5, show=False, save=False, dpi=300):
+def plot_confusion_matrix(y_test=None, y_pred=None, labels=[], threshold = 0.5, RESULTS_DIR='', titlestr='', show=False, save=False, dpi=300):
     """
     Returns a matplotlib figure containing the plotted confusion matrix.
     
     Args:
        y_test: ground-truth labels
        y_pred: predicted labels
        labels: class_names since y_test, y_pred are encoded.
@@ -129,121 +130,128 @@
     #     ax.set_text(j, i, cm[i, j], horizontalalignment="center", color=color)
     # ax.set_ylabel('True Label', fontsize=15)
     # ax.set_xlabel('Predicted Label', fontsize=15)
 
     s.set_ylabel('True Label') #, fontsize=15
     s.set_xlabel('Predicted Label')
     
+    plt.title(titlestr+"Confusion Matrix")
     plt.tight_layout()
-    if save:
-        plt.savefig(RESULTS_DIR+'/confusion_matrix.png', bbox_inches='tight',dpi=dpi)
     if show:
         plt.show()
+    if save:
+        plt.savefig(RESULTS_DIR+'/confusion_matrix.png', bbox_inches='tight',dpi=dpi)
+
     plt.close()
         
 def plot_ks_stat(y_test=None, y_pred=None, titlestr='', RESULTS_DIR='', show=False, save=False, dpi=300):
     fig, ax = plt.subplots()
     ax = scikitplot.metrics.plot_ks_statistic(y_test, y_pred, ax=ax)
     ax.set_xlim([-0.05, 1.05])
     ax.set_ylim([-0.05, 1.05])
     ax.set_facecolor('white')
     for l in ax.lines:
         l.set_lw(2)
-    plt.title("KS Statistic Plot "+titlestr)
+    plt.title(titlestr+"KS Statistic Plot ")
     plt.grid()
     plt.legend(loc='best')
     plt.tight_layout()
-    if save:
-        plt.savefig(RESULTS_DIR+'/ks_stat.png', bbox_inches='tight',dpi=dpi)
     if show:
         plt.show()
+    if save:
+        plt.savefig(RESULTS_DIR+'/ks_stat.png', bbox_inches='tight',dpi=dpi)
+
     plt.close()
 
 def plot_lift_curve(y_test=None, y_pred=None, titlestr='', RESULTS_DIR='', show=False, save=False, dpi=300):
     fig, ax = plt.subplots()
     ax = scikitplot.metrics.plot_lift_curve(y_test, y_pred, ax=ax)
     ax.set_facecolor('white')
     for l in ax.lines:
         l.set_lw(2)
-    plt.title("Lift Curve "+titlestr)
+    plt.title(titlestr+"Lift Curve ")
     # plt.grid()
     plt.legend(loc='best')
     plt.tight_layout()
+    if show:
+        plt.show()
     if save:
         plt.savefig(RESULTS_DIR+'/lift_curve.png', bbox_inches='tight',dpi=dpi)
-    if show:
-        plt.show()    
+    
     plt.close()
 
 def plot_cumul_gain(y_test=None, y_pred=None, titlestr='', RESULTS_DIR='', show=False, save=False, dpi=300):
     fig, ax = plt.subplots()
     ax = scikitplot.metrics.plot_cumulative_gain(y_test, y_pred, ax=ax)
     ax.set_facecolor('white')
     for l in ax.lines:
         l.set_lw(2)
-    plt.title("Cumulative Gains Curve "+titlestr)
+    plt.title(titlestr+"Cumulative Gains Curve ")
     # plt.grid()
     plt.legend(loc='best')
     plt.tight_layout()
+    if show:
+        plt.show()
     if save:
         plt.savefig(RESULTS_DIR+'/cumul_gain.png', bbox_inches='tight',dpi=dpi)
-    if show:
-        plt.show()    
+    
     plt.close()
 
 def plot_classwise_pr_curve(y_test=None, y_pred=None, titlestr='', RESULTS_DIR='', show=False, save=False, dpi=300):
     fig, ax = plt.subplots()
     ax = scikitplot.metrics.plot_precision_recall(y_test, y_pred, ax=ax)
     ax.set_xlim([-0.05, 1.05])
     ax.set_ylim([-0.05, 1.05])
     ax.set_facecolor('white')
     for l in ax.lines:
         l.set_lw(2)
-    plt.title("Precision-Recall Curve "+titlestr)
+    plt.title(titlestr+"Precision-Recall Curve ")
     plt.grid()
     plt.tight_layout()
+    if show:
+        plt.show()
     if save:
         plt.savefig(RESULTS_DIR+'/classwise_pr_curve.png', bbox_inches='tight',dpi=dpi)
-    if show:
-        plt.show()    
+    
     plt.close()
 
 def plot_classwise_roc_curve(y_test=None, y_pred=None, titlestr='', RESULTS_DIR='', show=False, save=False, dpi=300):
     fig, ax = plt.subplots()
     ax = scikitplot.metrics.plot_roc(y_test, y_pred, ax=ax)
     ax.set_xlim([-0.05, 1.05])
     ax.set_ylim([-0.05, 1.05])
     ax.set_facecolor('white')
     for l in ax.lines:
         l.set_lw(2)
-    plt.title("ROC Curves "+titlestr)
+    plt.title(titlestr+"ROC Curves ")
     plt.grid()
     plt.tight_layout()
+    if show:
+        plt.show()
     if save:
         plt.savefig(RESULTS_DIR+'/classwise_roc_curve.png', bbox_inches='tight', dpi=dpi)
-    if show:
-        plt.show() 
+ 
     plt.close()
 
-def generate_classification_report(y_test=None, y_pred=None, RESULTS_DIR='', labels=[], show=False, save=False):
+def generate_classification_report(y_test=None, y_pred=None, labels=[], RESULTS_DIR='', show=False, save=False):
     if(len(labels) !=0):
         report = classification_report(y_test, 
                                         y_pred, 
                                         target_names=[cl+'(class '+str(i)+')' for i, cl in enumerate(labels)], 
                                         output_dict=True)
     else:
         report = classification_report(y_test, y_pred, output_dict=True)
     report_df = pd.DataFrame(report).transpose()
     
     if save:
         report_df.to_csv(RESULTS_DIR+'/classification_report.csv')
     if show:
         print(report_df)
 
-def plot_cv_roc_curve(classifier=None, cv=None, n_splits=10, X=None, y=None, RESULTS_DIR='', title='Cross-Validated ROC Curve', show=False, save=False, dpi=300):
+def plot_cv_roc_curve(classifier=None, cv=None, n_splits=10, X=None, y=None, RESULTS_DIR='', titlestr='', show=False, save=False, dpi=300):
     """
     Draw a Cross Validated ROC Curve.
     Keyword Args:
         classifier: Classifier Object
         cv: StratifiedKFold Object: (https://stats.stackexchange.com/questions/49540/understanding-stratified-cross-validation)
         X: Feature Pandas DataFrame
         y: Response Pandas Series
@@ -285,25 +293,26 @@
     plt.fill_between(mean_fpr, tprs_lower, tprs_upper, color='grey', alpha=.2,
                      label=r'$\pm$ 1 std. dev.')
 
     plt.xlim([-0.05, 1.05])
     plt.ylim([-0.05, 1.05])
     plt.xlabel('False Positive Rate')
     plt.ylabel('True Positive Rate')
-    plt.title(title)
+    plt.title(titlestr+'Cross-Validated ROC Curve')
     plt.legend(bbox_to_anchor=(1, 1))
     # plt.tight_layout()
     plt.grid()
-    if(save):
-        plt.savefig(RESULTS_DIR+'/crossvalidation_roc_curve.png', bbox_inches='tight',dpi=dpi)
     if(show):
         plt.show()
+    if(save):
+        plt.savefig(RESULTS_DIR+'/crossvalidation_roc_curve.png', bbox_inches='tight',dpi=dpi)
+
     plt.close()
 
-def plot_cv_pr_curve(classifier=None, cv=None, n_splits=10, X=None, y=None, RESULTS_DIR='', title='Cross-Validated PR Curve', show=False, save=False, dpi=300):
+def plot_cv_pr_curve(classifier=None, cv=None, n_splits=10, X=None, y=None, RESULTS_DIR='', titlestr='', show=False, save=False, dpi=300):
     """
     Draw a Cross Validated PR Curve.
     Keyword Args:
         classifier: Classifier Object
         cv: StratifiedKFold Object: (https://stats.stackexchange.com/questions/49540/understanding-stratified-cross-validation)
         X: Feature Pandas DataFrame
         y: Response Pandas Series
@@ -337,48 +346,56 @@
              label=r'Average Precision (AP = %0.2f)' % (average_precision_score(y_real, y_proba)),
              lw=2, alpha=.8)
 
     plt.xlim([-0.05, 1.05])
     plt.ylim([-0.05, 1.05])
     plt.xlabel('Recall')
     plt.ylabel('Precision')
-    plt.title(title)
+    plt.title(titlestr+'Cross-Validated PR Curve')
     plt.legend(bbox_to_anchor=(1, 1))
     # plt.tight_layout()
     plt.grid()
-    if save:
-        plt.savefig(RESULTS_DIR+'/crossvalidation_pr_curve.png', bbox_inches='tight',dpi=dpi)   
     if show:
         plt.show()
+    if save:
+        plt.savefig(RESULTS_DIR+'/crossvalidation_pr_curve.png', bbox_inches='tight',dpi=dpi)   
     plt.close()
 
-def plot_shap_summary(model=None, nsamples=50, X_train=None, X_test=None, show=False, save=False, RESULTS_DIR=None):
+def plot_shap_summary(model=None, nsamples=50, X_train=None, X_test=None, titlestr='', show=False, save=False, RESULTS_DIR=None):
     print("No. of samples used to build explainer and generate shap values: ", nsamples)
     explainer = shap.KernelExplainer(model.predict, shap.sample(X_train, nsamples))
     shap_values = explainer.shap_values(X=X_test, nsamples=nsamples)
     shap.summary_plot(shap_values=shap_values, features=X_test, show=False)
     # shap.plots.violin(shap_values=shap_values, features=X_test, plot_type="layered_violin", show=False)
-    plt.title('Shapley Analysis')
+    plt.title(titlestr+'Shapley Analysis')
     plt.tight_layout()
-    if save:
-        plt.savefig(RESULTS_DIR+'/shap_summary_plot.png', bbox_inches='tight',dpi=dpi)   
     if show:
         plt.show()
+    if save:
+        plt.savefig(RESULTS_DIR+'/shap_summary_plot.png', bbox_inches='tight',dpi=dpi)   
+
     plt.close()
     
 def eval_classification(untrained_model=None, n_splits=10,
                         X=None, y=None, 
                         make_shap_plot=False, trained_model=None, X_train=None, X_test=None, 
                         y_train=None, y_test=None, y_pred=None, y_pred_proba=None, 
                         class_names=None,
+                        titlestr="",
                         save=False, RESULTS_DIR=None,
                         show=False, dpi=300):
 
-    titlestr = ', '.join(["class {}: {}".format(i, cls_nm) for i, cls_nm in enumerate(class_names)])
-    titlestr = "\n("+titlestr+")"
+    classes_titlestr = ', '.join(["class {}: {}".format(i, cls_nm) for i, cls_nm in enumerate(class_names)])
+    if titlestr != "":
+        titlestr_cls = titlestr+"\n("+classes_titlestr+")\n\n"
+        titlestr_nocls = titlestr+"\n\n"
+    else:
+        titlestr_cls = "("+classes_titlestr+")\n\n"
+        titlestr_nocls = titlestr
+
     if save:
         if RESULTS_DIR is not None:
             if not os.path.exists(RESULTS_DIR):
                 os.makedirs(RESULTS_DIR)
             print("Saving results in {}".format(RESULTS_DIR))   
         else:
             print("Hey! You asked me to save results but did not provide a RESULTS_DIR !!!")
@@ -392,89 +409,90 @@
                                         show=show, 
                                         save=save)
 
         plot_confusion_matrix(y_test=y_test, 
                                 y_pred=y_pred, 
                                 RESULTS_DIR=RESULTS_DIR, 
                                 labels=class_names,
+                                titlestr=titlestr_nocls,
                                 dpi=dpi,
                                 show=show,  
                                 save=save)
 
     if y_test is not None and y_pred_proba is not None:
         assert len(y_test) == len(y_pred_proba), "[Length Mismatch]: Number of test samples not equal to number of predictions"
         
         if len(list(set(y_test))) == 2:
             plot_ks_stat(y_test=y_test,
                             y_pred=y_pred_proba, 
                             RESULTS_DIR=RESULTS_DIR, 
-                            titlestr=titlestr,
+                            titlestr=titlestr_cls,
                             dpi=dpi,
                             show=show, 
                             save=save)
             
             plot_lift_curve(y_test=y_test,
                                 y_pred=y_pred_proba, 
                                 RESULTS_DIR=RESULTS_DIR, 
-                                titlestr=titlestr,
+                                titlestr=titlestr_cls,
                                 dpi=dpi,
                                 show=show, 
                                 save=save)
 
             plot_cumul_gain(y_test=y_test,
                                 y_pred=y_pred_proba, 
                                 RESULTS_DIR=RESULTS_DIR, 
-                                titlestr=titlestr,
+                                titlestr=titlestr_cls,
                                 dpi=dpi,
                                 show=show, 
                                 save=save)
         else:
             print("Skipping KS, Lift and Cumulative Gain plots as number of classes is not 2")
         
         plot_classwise_pr_curve(y_test=y_test,
                                     y_pred=y_pred_proba, 
                                     RESULTS_DIR=RESULTS_DIR, 
-                                    titlestr=titlestr,
+                                    titlestr=titlestr_cls,
                                     dpi=dpi,
                                     show=show, 
                                     save=save)
         
         plot_classwise_roc_curve(y_test=y_test,
                                     y_pred=y_pred_proba, 
                                     RESULTS_DIR=RESULTS_DIR, 
-                                    titlestr=titlestr,
+                                    titlestr=titlestr_cls,
                                     dpi=dpi,
                                     show=show, 
                                     save=save)
 
     if untrained_model is not None and X is not None and y is not None:
         assert len(X) == len(y), "[Length Mismatch]: Number of samples not equal to number of class labels"    
         if len(list(set(y_test))) == 2:
             plot_cv_roc_curve(classifier=untrained_model, 
                                 X=X, 
                                 y=pd.Series(y), 
                                 n_splits=n_splits,
                                 RESULTS_DIR=RESULTS_DIR, 
-                                title='Cross Validated ROC Curve', 
+                                titlestr=titlestr_nocls, 
                                 dpi=dpi,
                                 show=show, 
                                 save=save)
             
             plot_cv_pr_curve(classifier=untrained_model,  
                                 X=X, 
                                 y=pd.Series(y), 
                                 n_splits=n_splits,
                                 RESULTS_DIR=RESULTS_DIR, 
-                                title='Cross Validated PR Curve', 
+                                titlestr=titlestr_nocls,
                                 dpi=dpi,
                                 show=show, 
                                 save=save)
         else:
             print("Skipping Cross Validated ROC and PR curves as number of classes is not 2")
     
     if make_shap_plot:
         if X_train is not None and X_test is not None and trained_model is not None:
             plot_shap_summary(model=trained_model, X_train=X_train, X_test=X_test,
-                                RESULTS_DIR=RESULTS_DIR, show=show, save=save)
+                                titlestr=titlestr_nocls, show=show, RESULTS_DIR=RESULTS_DIR, save=save)
         else:
             print("Hey! You asked me to make a shap plot but did not provide a trained model, X_train and X_test !!!")
```

### Comparing `clfutils4r-0.0.1/src/clfutils4r.egg-info/PKG-INFO` & `clfutils4r-0.0.2/src/clfutils4r.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clfutils4r
-Version: 0.0.1
+Version: 0.0.2
 Summary: Wrapper around some basic sklearn and scikit-plot utilities for classification.
 Home-page: https://github.com/rutujagurav/clfutils4r
 Author: Rutuja Gurav
 Author-email: Rutuja Gurav <rutujagurav100@gmail.com>
 Project-URL: Homepage, https://github.com/rutujagurav/clfutils4r
 Project-URL: Bug Tracker, https://github.com/rutujagurav/clfutils4r/issues
 Classifier: Programming Language :: Python :: 3
@@ -150,7 +150,11 @@
 <!-- ### Cross-validated PR curves -->
 <!-- ![cv_pr](tests/example_classification/results/crossvalidation_pr_curve.png) -->
 ![cv_pr](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/crossvalidation_pr_curve.png)
 
 <!-- ### Shapley Analysis Summary Plot -->
 <!-- ![shap](tests/example_classification/results/shap_summary_plot.png) -->
 ![shap](https://github.com/rutujagurav/clfutils4r/blob/main/tests/example_classification/results/shap_summary_plot.png)
+
+
+## Developer Notes:
+This package is the updated version of `bcutils4r` which supported only binary classification. `bcutils4r` is now defunct.
```


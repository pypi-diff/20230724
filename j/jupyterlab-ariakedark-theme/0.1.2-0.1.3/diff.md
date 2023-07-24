# Comparing `tmp/jupyterlab_ariakedark_theme-0.1.2.tar.gz` & `tmp/jupyterlab_ariakedark_theme-0.1.3.tar.gz`

## Comparing `jupyterlab_ariakedark_theme-0.1.2.tar` & `jupyterlab_ariakedark_theme-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/.copier-answers.yml
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/RELEASE.md
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/TODO.md
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/install.json
--rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/tsconfig.json
--rw-r--r--   0        0        0   194544 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/yarn.lock
--rw-r--r--   0        0        0    20317 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/images/badge_pypi.svg
--rw-r--r--   0        0        0   193370 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/images/jupyterlab_ariakedark_1.png
--rw-r--r--   0        0        0   362052 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/images/jupyterlab_ariakedark_2.png
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/_version.py
--rw-r--r--   0        0        0    21924 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/build_log.json
--rw-r--r--   0        0        0     5434 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/package.json
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/static/lib_index_js.ec0f4e74d248cc0e4f58.js
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/static/lib_index_js.ec0f4e74d248cc0e4f58.js.map
--rw-r--r--   0        0        0    27153 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/static/remoteEntry.84696dca1279b4b085e4.js
--rw-r--r--   0        0        0    26033 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/static/remoteEntry.84696dca1279b4b085e4.js.map
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/static/style.js
--rw-r--r--   0        0        0    13835 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/themes/jupyterlab_ariakedark_theme/index.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/themes/jupyterlab_ariakedark_theme/index.js
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/src/index.ts
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/style/index.css
--rw-r--r--   0        0        0    13623 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/style/variables.css
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/.gitignore
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/LICENSE
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/README.md
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/.copier-answers.yml
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/RELEASE.md
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/TODO.md
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/install.json
+-rw-r--r--   0        0        0     6154 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/tsconfig.json
+-rw-r--r--   0        0        0   194544 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/yarn.lock
+-rw-r--r--   0        0        0    21405 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/images/badge_pypi.svg
+-rw-r--r--   0        0        0   193370 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/images/jupyterlab_ariakedark_1.png
+-rw-r--r--   0        0        0   362052 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/images/jupyterlab_ariakedark_2.png
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/jupyterlab_ariakedark_theme/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/jupyterlab_ariakedark_theme/_version.py
+-rw-r--r--   0        0        0    22176 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/jupyterlab_ariakedark_theme/labextension/build_log.json
+-rw-r--r--   0        0        0     5434 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/jupyterlab_ariakedark_theme/labextension/package.json
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/jupyterlab_ariakedark_theme/labextension/static/lib_index_js.ec0f4e74d248cc0e4f58.js
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/jupyterlab_ariakedark_theme/labextension/static/lib_index_js.ec0f4e74d248cc0e4f58.js.map
+-rw-r--r--   0        0        0    27153 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/jupyterlab_ariakedark_theme/labextension/static/remoteEntry.d9c562f8c1deef008056.js
+-rw-r--r--   0        0        0    26033 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/jupyterlab_ariakedark_theme/labextension/static/remoteEntry.d9c562f8c1deef008056.js.map
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/jupyterlab_ariakedark_theme/labextension/static/style.js
+-rw-r--r--   0        0        0    13835 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/jupyterlab_ariakedark_theme/labextension/themes/jupyterlab_ariakedark_theme/index.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/jupyterlab_ariakedark_theme/labextension/themes/jupyterlab_ariakedark_theme/index.js
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/src/index.ts
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/style/index.css
+-rw-r--r--   0        0        0    13623 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/style/variables.css
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/README.md
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 jupyterlab_ariakedark_theme-0.1.3/PKG-INFO
```

### Comparing `jupyterlab_ariakedark_theme-0.1.2/RELEASE.md` & `jupyterlab_ariakedark_theme-0.1.3/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.2/package.json` & `jupyterlab_ariakedark_theme-0.1.3/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'0.1.3'"}*

```diff
@@ -172,9 +172,9 @@
             "color-function-notation": null,
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.2"
+    "version": "0.1.3"
 }
```

### Comparing `jupyterlab_ariakedark_theme-0.1.2/tsconfig.json` & `jupyterlab_ariakedark_theme-0.1.3/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.2/yarn.lock` & `jupyterlab_ariakedark_theme-0.1.3/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.2/images/badge_pypi.svg` & `jupyterlab_ariakedark_theme-0.1.3/images/badge_pypi.svg`

 * *Files 4% similar despite different names*

```diff
@@ -1152,119 +1152,187 @@
 000047f0: 3032 2e38 3539 3337 3520 3134 2e30 3836  02.859375 14.086
 00004800: 3931 3520 5a20 4d20 3130 392e 3636 3939  915 Z M 109.6699
 00004810: 3220 3133 2e36 3335 3734 3320 4c20 3131  2 13.635743 L 11
 00004820: 302e 3830 3332 3220 3133 2e36 3335 3734  0.80322 13.63574
 00004830: 3320 4c20 3131 302e 3830 3332 3220 3135  3 L 110.80322 15
 00004840: 204c 2031 3039 2e36 3639 3932 2031 3520   L 109.66992 15 
 00004850: 4c20 3130 392e 3636 3939 3220 3133 2e36  L 109.66992 13.6
-00004860: 3335 3734 3320 5a20 4d20 3131 332e 3335  35743 Z M 113.35
-00004870: 3434 3920 3134 2e30 3836 3931 3520 4c20  449 14.086915 L 
-00004880: 3131 352e 3132 3639 3620 3134 2e30 3836  115.12696 14.086
-00004890: 3931 3520 4c20 3131 352e 3132 3639 3620  915 L 115.12696 
-000048a0: 372e 3936 3932 3338 3320 4c20 3131 332e  7.9692383 L 113.
-000048b0: 3139 3837 3420 382e 3335 3539 3537 204c  19874 8.355957 L
-000048c0: 2031 3133 2e31 3938 3734 2037 2e33 3637   113.19874 7.367
-000048d0: 3637 3533 204c 2031 3135 2e31 3136 3220  6753 L 115.1162 
-000048e0: 362e 3938 3039 3537 204c 2031 3136 2e32  6.980957 L 116.2
-000048f0: 3031 3137 2036 2e39 3830 3935 3720 4c20  0117 6.980957 L 
-00004900: 3131 362e 3230 3131 3720 3134 2e30 3836  116.20117 14.086
-00004910: 3931 3520 4c20 3131 372e 3937 3336 3420  915 L 117.97364 
-00004920: 3134 2e30 3836 3931 3520 4c20 3131 372e  14.086915 L 117.
-00004930: 3937 3336 3420 3135 204c 2031 3133 2e33  97364 15 L 113.3
-00004940: 3534 3439 2031 3520 4c20 3131 332e 3335  5449 15 L 113.35
-00004950: 3434 3920 3134 2e30 3836 3931 3520 5a22  449 14.086915 Z"
-00004960: 2f3e 0a20 2020 203c 2f67 3e0a 2020 2020  />.    </g>.    
-00004970: 3c67 0a20 2020 2020 2069 643d 2276 5465  <g.      id="vTe
-00004980: 7874 223e 0a20 2020 2020 203c 7061 7468  xt">.      <path
-00004990: 0a20 2020 2020 2020 2066 696c 6c3d 2223  .        fill="#
-000049a0: 6666 6666 6666 220a 2020 2020 2020 2020  ffffff".        
-000049b0: 7374 726f 6b65 3d22 2366 6666 6666 6622  stroke="#ffffff"
-000049c0: 0a20 2020 2020 2020 2073 7472 6f6b 652d  .        stroke-
-000049d0: 7769 6474 683d 2230 2e33 220a 2020 2020  width="0.3".    
-000049e0: 2020 2020 643d 224d 2039 342e 3439 3635      d="M 94.4965
-000049f0: 3820 362e 3639 3533 3132 3520 5120 3933  8 6.6953125 Q 93
-00004a00: 2e36 3538 3720 362e 3639 3533 3132 3520  .6587 6.6953125 
-00004a10: 3933 2e32 3337 3036 2037 2e35 3139 3737  93.23706 7.51977
-00004a20: 3534 2051 2039 322e 3831 3534 3320 382e  54 Q 92.81543 8.
-00004a30: 3334 3432 3338 2039 322e 3831 3534 3320  344238 92.81543 
-00004a40: 392e 3939 3835 3335 2051 2039 322e 3831  9.998535 Q 92.81
-00004a50: 3534 3320 3131 2e36 3437 3436 3120 3933  543 11.647461 93
-00004a60: 2e32 3337 3036 2031 322e 3437 3139 3233  .23706 12.471923
-00004a70: 2051 2039 332e 3635 3837 2031 332e 3239   Q 93.6587 13.29
-00004a80: 3633 3837 2039 342e 3439 3635 3820 3133  6387 94.49658 13
-00004a90: 2e32 3936 3338 3720 5120 3935 2e33 3339  .296387 Q 95.339
-00004aa0: 3835 2031 332e 3239 3633 3837 2039 352e  85 13.296387 95.
-00004ab0: 3736 3134 3820 3132 2e34 3731 3932 3320  76148 12.471923 
-00004ac0: 5120 3936 2e31 3833 3120 3131 2e36 3437  Q 96.1831 11.647
-00004ad0: 3436 3120 3936 2e31 3833 3120 392e 3939  461 96.1831 9.99
-00004ae0: 3835 3335 2051 2039 362e 3138 3331 2038  8535 Q 96.1831 8
-00004af0: 2e33 3434 3233 3820 3935 2e37 3631 3438  .344238 95.76148
-00004b00: 2037 2e35 3139 3737 3534 2051 2039 352e   7.5197754 Q 95.
-00004b10: 3333 3938 3520 362e 3639 3533 3132 3520  33985 6.6953125 
-00004b20: 3934 2e34 3936 3538 2036 2e36 3935 3331  94.49658 6.69531
-00004b30: 3235 205a 204d 2039 342e 3439 3635 3820  25 Z M 94.49658 
-00004b40: 352e 3833 3539 3337 3520 5120 3935 2e38  5.8359375 Q 95.8
-00004b50: 3434 3733 3420 352e 3833 3539 3337 3520  44734 5.8359375 
-00004b60: 3936 2e35 3536 3430 3420 362e 3930 3230  96.556404 6.9020
-00004b70: 3939 3620 5120 3937 2e32 3638 3037 3420  996 Q 97.268074 
-00004b80: 372e 3936 3832 3631 3720 3937 2e32 3638  7.9682617 97.268
-00004b90: 3037 3420 392e 3939 3835 3335 2051 2039  074 9.998535 Q 9
-00004ba0: 372e 3236 3830 3734 2031 322e 3032 3334  7.268074 12.0234
-00004bb0: 3338 2039 362e 3535 3634 3034 2031 332e  38 96.556404 13.
-00004bc0: 3038 3936 2051 2039 352e 3834 3437 3334  0896 Q 95.844734
-00004bd0: 2031 342e 3135 3537 3632 2039 342e 3439   14.155762 94.49
-00004be0: 3635 3820 3134 2e31 3535 3736 3220 5120  658 14.155762 Q 
-00004bf0: 3933 2e31 3438 3434 2031 342e 3135 3537  93.14844 14.1557
-00004c00: 3632 2039 322e 3433 3637 3720 3133 2e30  62 92.43677 13.0
-00004c10: 3839 3620 5120 3931 2e37 3235 3120 3132  896 Q 91.7251 12
-00004c20: 2e30 3233 3433 3820 3931 2e37 3235 3120  .023438 91.7251 
-00004c30: 392e 3939 3835 3335 2051 2039 312e 3732  9.998535 Q 91.72
-00004c40: 3531 2037 2e39 3638 3236 3137 2039 322e  51 7.9682617 92.
-00004c50: 3433 3637 3720 362e 3930 3230 3939 3620  43677 6.9020996 
-00004c60: 5120 3933 2e31 3438 3434 2035 2e38 3335  Q 93.14844 5.835
-00004c70: 3933 3735 2039 342e 3439 3635 3820 352e  9375 94.49658 5.
-00004c80: 3833 3539 3337 3520 5a20 4d20 3939 2e31  8359375 Z M 99.1
-00004c90: 3734 3831 2031 322e 3633 3537 3433 204c  7481 12.635743 L
-00004ca0: 2031 3030 2e33 3038 3120 3132 2e36 3335   100.3081 12.635
-00004cb0: 3734 3320 4c20 3130 302e 3330 3831 2031  743 L 100.3081 1
-00004cc0: 3420 4c20 3939 2e31 3734 3831 2031 3420  4 L 99.17481 14 
-00004cd0: 4c20 3939 2e31 3734 3831 2031 322e 3633  L 99.17481 12.63
-00004ce0: 3537 3433 205a 204d 2031 3032 2e38 3539  5743 Z M 102.859
-00004cf0: 3337 3520 3133 2e30 3836 3931 3520 4c20  375 13.086915 L 
-00004d00: 3130 342e 3633 3138 3336 2031 332e 3038  104.631836 13.08
-00004d10: 3639 3135 204c 2031 3034 2e36 3331 3833  6915 L 104.63183
-00004d20: 3620 362e 3936 3932 3338 3320 4c20 3130  6 6.9692383 L 10
-00004d30: 322e 3730 3336 3120 372e 3335 3539 3537  2.70361 7.355957
-00004d40: 204c 2031 3032 2e37 3033 3631 2036 2e33   L 102.70361 6.3
-00004d50: 3637 3637 3533 204c 2031 3034 2e36 3231  676753 L 104.621
-00004d60: 3039 2035 2e39 3830 3935 3720 4c20 3130  09 5.980957 L 10
-00004d70: 352e 3730 3630 3535 2035 2e39 3830 3935  5.706055 5.98095
-00004d80: 3720 4c20 3130 352e 3730 3630 3535 2031  7 L 105.706055 1
-00004d90: 332e 3038 3639 3135 204c 2031 3037 2e34  3.086915 L 107.4
-00004da0: 3738 3531 3620 3133 2e30 3836 3931 3520  78516 13.086915 
-00004db0: 4c20 3130 372e 3437 3835 3136 2031 3420  L 107.478516 14 
-00004dc0: 4c20 3130 322e 3835 3933 3735 2031 3420  L 102.859375 14 
-00004dd0: 4c20 3130 322e 3835 3933 3735 2031 332e  L 102.859375 13.
-00004de0: 3038 3639 3135 205a 204d 2031 3039 2e36  086915 Z M 109.6
-00004df0: 3639 3932 2031 322e 3633 3537 3433 204c  6992 12.635743 L
-00004e00: 2031 3130 2e38 3033 3232 2031 322e 3633   110.80322 12.63
-00004e10: 3537 3433 204c 2031 3130 2e38 3033 3232  5743 L 110.80322
-00004e20: 2031 3420 4c20 3130 392e 3636 3939 3220   14 L 109.66992 
-00004e30: 3134 204c 2031 3039 2e36 3639 3932 2031  14 L 109.66992 1
-00004e40: 322e 3633 3537 3433 205a 204d 2031 3133  2.635743 Z M 113
-00004e50: 2e33 3534 3439 2031 332e 3038 3639 3135  .35449 13.086915
-00004e60: 204c 2031 3135 2e31 3236 3936 2031 332e   L 115.12696 13.
-00004e70: 3038 3639 3135 204c 2031 3135 2e31 3236  086915 L 115.126
-00004e80: 3936 2036 2e39 3639 3233 3833 204c 2031  96 6.9692383 L 1
-00004e90: 3133 2e31 3938 3734 2037 2e33 3535 3935  13.19874 7.35595
-00004ea0: 3720 4c20 3131 332e 3139 3837 3420 362e  7 L 113.19874 6.
-00004eb0: 3336 3736 3735 3320 4c20 3131 352e 3131  3676753 L 115.11
-00004ec0: 3632 2035 2e39 3830 3935 3720 4c20 3131  62 5.980957 L 11
-00004ed0: 362e 3230 3131 3720 352e 3938 3039 3537  6.20117 5.980957
-00004ee0: 204c 2031 3136 2e32 3031 3137 2031 332e   L 116.20117 13.
-00004ef0: 3038 3639 3135 204c 2031 3137 2e39 3733  086915 L 117.973
-00004f00: 3634 2031 332e 3038 3639 3135 204c 2031  64 13.086915 L 1
-00004f10: 3137 2e39 3733 3634 2031 3420 4c20 3131  17.97364 14 L 11
-00004f20: 332e 3335 3434 3920 3134 204c 2031 3133  3.35449 14 L 113
-00004f30: 2e33 3534 3439 2031 332e 3038 3639 3135  .35449 13.086915
-00004f40: 205a 222f 3e0a 2020 2020 3c2f 673e 0a20   Z"/>.    </g>. 
-00004f50: 203c 2f67 3e0a 3c2f 7376 673e 0a          </g>.</svg>.
+00004860: 3335 3734 3320 5a20 4d20 3131 342e 3130  35743 Z M 114.10
+00004870: 3130 3734 2031 342e 3038 3639 3135 204c  1074 14.086915 L
+00004880: 2031 3137 2e38 3837 3639 3520 3134 2e30   117.887695 14.0
+00004890: 3836 3931 3520 4c20 3131 372e 3838 3736  86915 L 117.8876
+000048a0: 3935 2031 3520 4c20 3131 322e 3739 3538  95 15 L 112.7958
+000048b0: 3920 3135 204c 2031 3132 2e37 3935 3839  9 15 L 112.79589
+000048c0: 2031 342e 3038 3639 3135 2051 2031 3133   14.086915 Q 113
+000048d0: 2e34 3133 3537 3420 3133 2e34 3437 3735  .413574 13.44775
+000048e0: 3420 3131 342e 3437 3937 3420 3132 2e33  4 114.47974 12.3
+000048f0: 3730 3835 2051 2031 3135 2e35 3435 3920  7085 Q 115.5459 
+00004900: 3131 2e32 3933 3934 3520 3131 352e 3831  11.293945 115.81
+00004910: 3938 3234 2031 302e 3938 3234 3232 2051  9824 10.982422 Q
+00004920: 2031 3136 2e33 3430 3832 2031 302e 3339   116.34082 10.39
+00004930: 3639 3733 2031 3136 2e35 3437 3631 2039  6973 116.54761 9
+00004940: 2e39 3931 3435 3520 5120 3131 362e 3735  .991455 Q 116.75
+00004950: 3433 3935 2039 2e35 3835 3933 3735 2031  4395 9.5859375 1
+00004960: 3136 2e37 3534 3339 3520 392e 3139 3338  16.754395 9.1938
+00004970: 3438 2051 2031 3136 2e37 3534 3339 3520  48 Q 116.754395 
+00004980: 382e 3535 3436 3837 3520 3131 362e 3330  8.5546875 116.30
+00004990: 3539 3120 382e 3135 3138 3535 2051 2031  591 8.151855 Q 1
+000049a0: 3135 2e38 3537 3432 2037 2e37 3439 3032  15.85742 7.74902
+000049b0: 3334 2031 3135 2e31 3337 3720 372e 3734  34 115.1377 7.74
+000049c0: 3930 3233 3420 5120 3131 342e 3632 3734  90234 Q 114.6274
+000049d0: 3420 372e 3734 3930 3233 3420 3131 342e  4 7.7490234 114.
+000049e0: 3036 3037 3920 372e 3932 3632 3639 3520  06079 7.9262695 
+000049f0: 5120 3131 332e 3439 3431 3420 382e 3130  Q 113.49414 8.10
+00004a00: 3335 3136 2031 3132 2e38 3439 3631 2038  3516 112.84961 8
+00004a10: 2e34 3633 3337 3920 4c20 3131 322e 3834  .463379 L 112.84
+00004a20: 3936 3120 372e 3336 3736 3735 3320 5120  961 7.3676753 Q 
+00004a30: 3131 332e 3530 3438 3820 372e 3130 3434  113.50488 7.1044
+00004a40: 3932 2031 3134 2e30 3734 3231 2036 2e39  92 114.07421 6.9
+00004a50: 3730 3231 3520 5120 3131 342e 3634 3335  70215 Q 114.6435
+00004a60: 3535 2036 2e38 3335 3933 3735 2031 3135  55 6.8359375 115
+00004a70: 2e31 3136 3220 362e 3833 3539 3337 3520  .1162 6.8359375 
+00004a80: 5120 3131 362e 3336 3233 3035 2036 2e38  Q 116.362305 6.8
+00004a90: 3335 3933 3735 2031 3137 2e31 3033 3531  359375 117.10351
+00004aa0: 3620 372e 3435 3839 3834 3420 5120 3131  6 7.4589844 Q 11
+00004ab0: 372e 3834 3437 3320 382e 3038 3230 3331  7.84473 8.082031
+00004ac0: 2031 3137 2e38 3434 3733 2039 2e31 3234   117.84473 9.124
+00004ad0: 3032 3320 5120 3131 372e 3834 3437 3320  023 Q 117.84473 
+00004ae0: 392e 3631 3831 3634 2031 3137 2e36 3539  9.618164 117.659
+00004af0: 3432 3420 3130 2e30 3631 3237 3920 5120  424 10.061279 Q 
+00004b00: 3131 372e 3437 3431 3220 3130 2e35 3034  117.47412 10.504
+00004b10: 3339 3520 3131 362e 3938 3533 3520 3131  395 116.98535 11
+00004b20: 2e31 3035 3935 3720 5120 3131 362e 3835  .105957 Q 116.85
+00004b30: 3130 3734 2031 312e 3236 3137 3139 2031  1074 11.261719 1
+00004b40: 3136 2e31 3331 3335 2031 322e 3030 3536  16.13135 12.0056
+00004b50: 3135 2051 2031 3135 2e34 3131 3632 2031  15 Q 115.41162 1
+00004b60: 322e 3734 3935 3132 2031 3134 2e31 3031  2.749512 114.101
+00004b70: 3037 3420 3134 2e30 3836 3931 3520 5a22  074 14.086915 Z"
+00004b80: 2f3e 0a20 2020 203c 2f67 3e0a 2020 2020  />.    </g>.    
+00004b90: 3c67 0a20 2020 2020 2069 643d 2276 5465  <g.      id="vTe
+00004ba0: 7874 223e 0a20 2020 2020 203c 7061 7468  xt">.      <path
+00004bb0: 0a20 2020 2020 2020 2066 696c 6c3d 2223  .        fill="#
+00004bc0: 6666 6666 6666 220a 2020 2020 2020 2020  ffffff".        
+00004bd0: 7374 726f 6b65 3d22 2366 6666 6666 6622  stroke="#ffffff"
+00004be0: 0a20 2020 2020 2020 2073 7472 6f6b 652d  .        stroke-
+00004bf0: 7769 6474 683d 2230 2e33 220a 2020 2020  width="0.3".    
+00004c00: 2020 2020 643d 224d 2039 342e 3439 3635      d="M 94.4965
+00004c10: 3820 362e 3639 3533 3132 3520 5120 3933  8 6.6953125 Q 93
+00004c20: 2e36 3538 3720 362e 3639 3533 3132 3520  .6587 6.6953125 
+00004c30: 3933 2e32 3337 3036 2037 2e35 3139 3737  93.23706 7.51977
+00004c40: 3534 2051 2039 322e 3831 3534 3320 382e  54 Q 92.81543 8.
+00004c50: 3334 3432 3338 2039 322e 3831 3534 3320  344238 92.81543 
+00004c60: 392e 3939 3835 3335 2051 2039 322e 3831  9.998535 Q 92.81
+00004c70: 3534 3320 3131 2e36 3437 3436 3120 3933  543 11.647461 93
+00004c80: 2e32 3337 3036 2031 322e 3437 3139 3233  .23706 12.471923
+00004c90: 2051 2039 332e 3635 3837 2031 332e 3239   Q 93.6587 13.29
+00004ca0: 3633 3837 2039 342e 3439 3635 3820 3133  6387 94.49658 13
+00004cb0: 2e32 3936 3338 3720 5120 3935 2e33 3339  .296387 Q 95.339
+00004cc0: 3835 2031 332e 3239 3633 3837 2039 352e  85 13.296387 95.
+00004cd0: 3736 3134 3820 3132 2e34 3731 3932 3320  76148 12.471923 
+00004ce0: 5120 3936 2e31 3833 3120 3131 2e36 3437  Q 96.1831 11.647
+00004cf0: 3436 3120 3936 2e31 3833 3120 392e 3939  461 96.1831 9.99
+00004d00: 3835 3335 2051 2039 362e 3138 3331 2038  8535 Q 96.1831 8
+00004d10: 2e33 3434 3233 3820 3935 2e37 3631 3438  .344238 95.76148
+00004d20: 2037 2e35 3139 3737 3534 2051 2039 352e   7.5197754 Q 95.
+00004d30: 3333 3938 3520 362e 3639 3533 3132 3520  33985 6.6953125 
+00004d40: 3934 2e34 3936 3538 2036 2e36 3935 3331  94.49658 6.69531
+00004d50: 3235 205a 204d 2039 342e 3439 3635 3820  25 Z M 94.49658 
+00004d60: 352e 3833 3539 3337 3520 5120 3935 2e38  5.8359375 Q 95.8
+00004d70: 3434 3733 3420 352e 3833 3539 3337 3520  44734 5.8359375 
+00004d80: 3936 2e35 3536 3430 3420 362e 3930 3230  96.556404 6.9020
+00004d90: 3939 3620 5120 3937 2e32 3638 3037 3420  996 Q 97.268074 
+00004da0: 372e 3936 3832 3631 3720 3937 2e32 3638  7.9682617 97.268
+00004db0: 3037 3420 392e 3939 3835 3335 2051 2039  074 9.998535 Q 9
+00004dc0: 372e 3236 3830 3734 2031 322e 3032 3334  7.268074 12.0234
+00004dd0: 3338 2039 362e 3535 3634 3034 2031 332e  38 96.556404 13.
+00004de0: 3038 3936 2051 2039 352e 3834 3437 3334  0896 Q 95.844734
+00004df0: 2031 342e 3135 3537 3632 2039 342e 3439   14.155762 94.49
+00004e00: 3635 3820 3134 2e31 3535 3736 3220 5120  658 14.155762 Q 
+00004e10: 3933 2e31 3438 3434 2031 342e 3135 3537  93.14844 14.1557
+00004e20: 3632 2039 322e 3433 3637 3720 3133 2e30  62 92.43677 13.0
+00004e30: 3839 3620 5120 3931 2e37 3235 3120 3132  896 Q 91.7251 12
+00004e40: 2e30 3233 3433 3820 3931 2e37 3235 3120  .023438 91.7251 
+00004e50: 392e 3939 3835 3335 2051 2039 312e 3732  9.998535 Q 91.72
+00004e60: 3531 2037 2e39 3638 3236 3137 2039 322e  51 7.9682617 92.
+00004e70: 3433 3637 3720 362e 3930 3230 3939 3620  43677 6.9020996 
+00004e80: 5120 3933 2e31 3438 3434 2035 2e38 3335  Q 93.14844 5.835
+00004e90: 3933 3735 2039 342e 3439 3635 3820 352e  9375 94.49658 5.
+00004ea0: 3833 3539 3337 3520 5a20 4d20 3939 2e31  8359375 Z M 99.1
+00004eb0: 3734 3831 2031 322e 3633 3537 3433 204c  7481 12.635743 L
+00004ec0: 2031 3030 2e33 3038 3120 3132 2e36 3335   100.3081 12.635
+00004ed0: 3734 3320 4c20 3130 302e 3330 3831 2031  743 L 100.3081 1
+00004ee0: 3420 4c20 3939 2e31 3734 3831 2031 3420  4 L 99.17481 14 
+00004ef0: 4c20 3939 2e31 3734 3831 2031 322e 3633  L 99.17481 12.63
+00004f00: 3537 3433 205a 204d 2031 3032 2e38 3539  5743 Z M 102.859
+00004f10: 3337 3520 3133 2e30 3836 3931 3520 4c20  375 13.086915 L 
+00004f20: 3130 342e 3633 3138 3336 2031 332e 3038  104.631836 13.08
+00004f30: 3639 3135 204c 2031 3034 2e36 3331 3833  6915 L 104.63183
+00004f40: 3620 362e 3936 3932 3338 3320 4c20 3130  6 6.9692383 L 10
+00004f50: 322e 3730 3336 3120 372e 3335 3539 3537  2.70361 7.355957
+00004f60: 204c 2031 3032 2e37 3033 3631 2036 2e33   L 102.70361 6.3
+00004f70: 3637 3637 3533 204c 2031 3034 2e36 3231  676753 L 104.621
+00004f80: 3039 2035 2e39 3830 3935 3720 4c20 3130  09 5.980957 L 10
+00004f90: 352e 3730 3630 3535 2035 2e39 3830 3935  5.706055 5.98095
+00004fa0: 3720 4c20 3130 352e 3730 3630 3535 2031  7 L 105.706055 1
+00004fb0: 332e 3038 3639 3135 204c 2031 3037 2e34  3.086915 L 107.4
+00004fc0: 3738 3531 3620 3133 2e30 3836 3931 3520  78516 13.086915 
+00004fd0: 4c20 3130 372e 3437 3835 3136 2031 3420  L 107.478516 14 
+00004fe0: 4c20 3130 322e 3835 3933 3735 2031 3420  L 102.859375 14 
+00004ff0: 4c20 3130 322e 3835 3933 3735 2031 332e  L 102.859375 13.
+00005000: 3038 3639 3135 205a 204d 2031 3039 2e36  086915 Z M 109.6
+00005010: 3639 3932 2031 322e 3633 3537 3433 204c  6992 12.635743 L
+00005020: 2031 3130 2e38 3033 3232 2031 322e 3633   110.80322 12.63
+00005030: 3537 3433 204c 2031 3130 2e38 3033 3232  5743 L 110.80322
+00005040: 2031 3420 4c20 3130 392e 3636 3939 3220   14 L 109.66992 
+00005050: 3134 204c 2031 3039 2e36 3639 3932 2031  14 L 109.66992 1
+00005060: 322e 3633 3537 3433 205a 204d 2031 3134  2.635743 Z M 114
+00005070: 2e31 3031 3037 3420 3133 2e30 3836 3931  .101074 13.08691
+00005080: 3520 4c20 3131 372e 3838 3736 3935 2031  5 L 117.887695 1
+00005090: 332e 3038 3639 3135 204c 2031 3137 2e38  3.086915 L 117.8
+000050a0: 3837 3639 3520 3134 204c 2031 3132 2e37  87695 14 L 112.7
+000050b0: 3935 3839 2031 3420 4c20 3131 322e 3739  9589 14 L 112.79
+000050c0: 3538 3920 3133 2e30 3836 3931 3520 5120  589 13.086915 Q 
+000050d0: 3131 332e 3431 3335 3734 2031 322e 3434  113.413574 12.44
+000050e0: 3737 3534 2031 3134 2e34 3739 3734 2031  7754 114.47974 1
+000050f0: 312e 3337 3038 3520 5120 3131 352e 3534  1.37085 Q 115.54
+00005100: 3539 2031 302e 3239 3339 3435 2031 3135  59 10.293945 115
+00005110: 2e38 3139 3832 3420 392e 3938 3234 3232  .819824 9.982422
+00005120: 2051 2031 3136 2e33 3430 3832 2039 2e33   Q 116.34082 9.3
+00005130: 3936 3937 3320 3131 362e 3534 3736 3120  96973 116.54761 
+00005140: 382e 3939 3134 3535 2051 2031 3136 2e37  8.991455 Q 116.7
+00005150: 3534 3339 3520 382e 3538 3539 3337 3520  54395 8.5859375 
+00005160: 3131 362e 3735 3433 3935 2038 2e31 3933  116.754395 8.193
+00005170: 3834 3820 5120 3131 362e 3735 3433 3935  848 Q 116.754395
+00005180: 2037 2e35 3534 3638 3735 2031 3136 2e33   7.5546875 116.3
+00005190: 3035 3931 2037 2e31 3531 3835 3535 2051  0591 7.1518555 Q
+000051a0: 2031 3135 2e38 3537 3432 2036 2e37 3439   115.85742 6.749
+000051b0: 3032 3334 2031 3135 2e31 3337 3720 362e  0234 115.1377 6.
+000051c0: 3734 3930 3233 3420 5120 3131 342e 3632  7490234 Q 114.62
+000051d0: 3734 3420 362e 3734 3930 3233 3420 3131  744 6.7490234 11
+000051e0: 342e 3036 3037 3920 362e 3932 3632 3639  4.06079 6.926269
+000051f0: 3520 5120 3131 332e 3439 3431 3420 372e  5 Q 113.49414 7.
+00005200: 3130 3335 3135 3620 3131 322e 3834 3936  1035156 112.8496
+00005210: 3120 372e 3436 3333 3739 3420 4c20 3131  1 7.4633794 L 11
+00005220: 322e 3834 3936 3120 362e 3336 3736 3735  2.84961 6.367675
+00005230: 3320 5120 3131 332e 3530 3438 3820 362e  3 Q 113.50488 6.
+00005240: 3130 3434 3932 2031 3134 2e30 3734 3231  104492 114.07421
+00005250: 2035 2e39 3730 3231 3520 5120 3131 342e   5.970215 Q 114.
+00005260: 3634 3335 3535 2035 2e38 3335 3933 3735  643555 5.8359375
+00005270: 2031 3135 2e31 3136 3220 352e 3833 3539   115.1162 5.8359
+00005280: 3337 3520 5120 3131 362e 3336 3233 3035  375 Q 116.362305
+00005290: 2035 2e38 3335 3933 3735 2031 3137 2e31   5.8359375 117.1
+000052a0: 3033 3531 3620 362e 3435 3839 3834 3420  03516 6.4589844 
+000052b0: 5120 3131 372e 3834 3437 3320 372e 3038  Q 117.84473 7.08
+000052c0: 3230 3331 3320 3131 372e 3834 3437 3320  20313 117.84473 
+000052d0: 382e 3132 3430 3233 2051 2031 3137 2e38  8.124023 Q 117.8
+000052e0: 3434 3733 2038 2e36 3138 3136 3420 3131  4473 8.618164 11
+000052f0: 372e 3635 3934 3234 2039 2e30 3631 3237  7.659424 9.06127
+00005300: 3920 5120 3131 372e 3437 3431 3220 392e  9 Q 117.47412 9.
+00005310: 3530 3433 3935 2031 3136 2e39 3835 3335  504395 116.98535
+00005320: 2031 302e 3130 3539 3537 2051 2031 3136   10.105957 Q 116
+00005330: 2e38 3531 3037 3420 3130 2e32 3631 3731  .851074 10.26171
+00005340: 3920 3131 362e 3133 3133 3520 3131 2e30  9 116.13135 11.0
+00005350: 3035 3631 3520 5120 3131 352e 3431 3136  05615 Q 115.4116
+00005360: 3220 3131 2e37 3439 3531 3220 3131 342e  2 11.749512 114.
+00005370: 3130 3130 3734 2031 332e 3038 3639 3135  101074 13.086915
+00005380: 205a 222f 3e0a 2020 2020 3c2f 673e 0a20   Z"/>.    </g>. 
+00005390: 203c 2f67 3e0a 3c2f 7376 673e 0a          </g>.</svg>.
```

### Comparing `jupyterlab_ariakedark_theme-0.1.2/images/jupyterlab_ariakedark_1.png` & `jupyterlab_ariakedark_theme-0.1.3/images/jupyterlab_ariakedark_1.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.2/images/jupyterlab_ariakedark_2.png` & `jupyterlab_ariakedark_theme-0.1.3/images/jupyterlab_ariakedark_2.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/__init__.py` & `jupyterlab_ariakedark_theme-0.1.3/jupyterlab_ariakedark_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/build_log.json` & `jupyterlab_ariakedark_theme-0.1.3/jupyterlab_ariakedark_theme/labextension/build_log.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9587956311196255%*

 * *Differences: {'0': "{'resolve': {'fallback': {'path': "*

 * *      "'/home/eduardotc/Programação/my_gits/jupyterlab_ariakedark_theme/jupyterlab_ariakedark_theme/node_modules/path-browserify/index.js', "*

 * *      "'process': "*

 * *      "'/home/eduardotc/Programação/my_gits/jupyterlab_ariakedark_theme/jupyterlab_ariakedark_theme/node_modules/process/browser.js'}}, "*

 * *      "'output': {'path': "*

 * *      "'/home/eduardotc/Programação/my_gits/jupyterlab_ariakedark_theme/jupyterlab_ariakedark_theme/jupyterlab_ariakedark_theme/labextension/ […]*

```diff
@@ -88,28 +88,28 @@
                     ]
                 }
             ]
         },
         "output": {
             "filename": "[name].[contenthash].js",
             "hashFunction": "sha256",
-            "path": "/home/eduardotc/Programa\u00e7\u00e3o/my_gits/jupyterlab_ariakedark_theme/jupyterlab_ariakedark_theme/labextension/static",
+            "path": "/home/eduardotc/Programa\u00e7\u00e3o/my_gits/jupyterlab_ariakedark_theme/jupyterlab_ariakedark_theme/jupyterlab_ariakedark_theme/labextension/static",
             "publicPath": "auto"
         },
         "plugins": [
             {
                 "definitions": {
                     "process": "process/browser"
                 }
             },
             {
                 "_options": {
                     "exposes": {
-                        "./extension": "/home/eduardotc/Programa\u00e7\u00e3o/my_gits/jupyterlab_ariakedark_theme/lib/index.js",
-                        "./index": "/home/eduardotc/Programa\u00e7\u00e3o/my_gits/jupyterlab_ariakedark_theme/lib/index.js"
+                        "./extension": "/home/eduardotc/Programa\u00e7\u00e3o/my_gits/jupyterlab_ariakedark_theme/jupyterlab_ariakedark_theme/lib/index.js",
+                        "./index": "/home/eduardotc/Programa\u00e7\u00e3o/my_gits/jupyterlab_ariakedark_theme/jupyterlab_ariakedark_theme/lib/index.js"
                     },
                     "filename": "remoteEntry.[contenthash].js",
                     "library": {
                         "name": [
                             "_JUPYTERLAB",
                             "jupyterlab_ariakedark_theme"
                         ],
@@ -619,17 +619,17 @@
                         },
                         "@lumino/widgets": {
                             "import": false,
                             "requiredVersion": "^2.0.1",
                             "singleton": true
                         },
                         "jupyterlab_ariakedark_theme": {
-                            "import": "/home/eduardotc/Programa\u00e7\u00e3o/my_gits/jupyterlab_ariakedark_theme/lib/index.js",
+                            "import": "/home/eduardotc/Programa\u00e7\u00e3o/my_gits/jupyterlab_ariakedark_theme/jupyterlab_ariakedark_theme/lib/index.js",
                             "singleton": true,
-                            "version": "0.1.1"
+                            "version": "0.1.2"
                         },
                         "react": {
                             "import": false,
                             "requiredVersion": "^18.2.0",
                             "singleton": true
                         },
                         "react-dom": {
@@ -647,35 +647,35 @@
             },
             {}
         ],
         "resolve": {
             "fallback": {
                 "buffer": false,
                 "crypto": false,
-                "path": "/home/eduardotc/Programa\u00e7\u00e3o/my_gits/jupyterlab_ariakedark_theme/node_modules/path-browserify/index.js",
-                "process": "/home/eduardotc/Programa\u00e7\u00e3o/my_gits/jupyterlab_ariakedark_theme/node_modules/process/browser.js",
+                "path": "/home/eduardotc/Programa\u00e7\u00e3o/my_gits/jupyterlab_ariakedark_theme/jupyterlab_ariakedark_theme/node_modules/path-browserify/index.js",
+                "process": "/home/eduardotc/Programa\u00e7\u00e3o/my_gits/jupyterlab_ariakedark_theme/jupyterlab_ariakedark_theme/node_modules/process/browser.js",
                 "url": false
             }
         },
         "watchOptions": {
             "aggregateTimeout": 1000,
             "poll": 500
         }
     },
     {
         "entry": {
-            "index": "/home/eduardotc/Programa\u00e7\u00e3o/my_gits/jupyterlab_ariakedark_theme/style/index.css"
+            "index": "/home/eduardotc/Programa\u00e7\u00e3o/my_gits/jupyterlab_ariakedark_theme/jupyterlab_ariakedark_theme/style/index.css"
         },
         "mode": "production",
         "module": {
             "rules": [
                 {
                     "test": "/\\.css$/",
                     "use": [
-                        "/home/eduardotc/Programa\u00e7\u00e3o/my_gits/jupyterlab_ariakedark_theme/node_modules/mini-css-extract-plugin/dist/loader.js",
+                        "/home/eduardotc/Programa\u00e7\u00e3o/my_gits/jupyterlab_ariakedark_theme/jupyterlab_ariakedark_theme/node_modules/mini-css-extract-plugin/dist/loader.js",
                         "css-loader"
                     ]
                 },
                 {
                     "generator": {},
                     "test": "/\\.svg/",
                     "type": "asset/inline"
@@ -685,15 +685,15 @@
                     "type": "asset"
                 }
             ]
         },
         "output": {
             "filename": "[name].js",
             "hashFunction": "sha256",
-            "path": "/home/eduardotc/Programa\u00e7\u00e3o/my_gits/jupyterlab_ariakedark_theme/jupyterlab_ariakedark_theme/labextension/themes/jupyterlab_ariakedark_theme"
+            "path": "/home/eduardotc/Programa\u00e7\u00e3o/my_gits/jupyterlab_ariakedark_theme/jupyterlab_ariakedark_theme/jupyterlab_ariakedark_theme/labextension/themes/jupyterlab_ariakedark_theme"
         },
         "plugins": [
             {
                 "_sortedModulesCache": {},
                 "options": {
                     "chunkFilename": "[id].css",
                     "filename": "[name].css",
```

### Comparing `jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/package.json` & `jupyterlab_ariakedark_theme-0.1.3/jupyterlab_ariakedark_theme/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9765625%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.d9c562f8c1deef008056.js'}}",*

 * * "'version'": "'0.1.2'"}*

```diff
@@ -97,15 +97,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/eduardotlc/jupyterlab_ariakedark_theme",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.84696dca1279b4b085e4.js"
+            "load": "static/remoteEntry.d9c562f8c1deef008056.js"
         },
         "extension": true,
         "outputDir": "jupyterlab_ariakedark_theme/labextension",
         "themePath": "style/index.css"
     },
     "keywords": [
         "jupyter",
@@ -176,9 +176,9 @@
             "color-function-notation": null,
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.1"
+    "version": "0.1.2"
 }
```

### Comparing `jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/static/lib_index_js.ec0f4e74d248cc0e4f58.js` & `jupyterlab_ariakedark_theme-0.1.3/jupyterlab_ariakedark_theme/labextension/static/lib_index_js.ec0f4e74d248cc0e4f58.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/static/lib_index_js.ec0f4e74d248cc0e4f58.js.map` & `jupyterlab_ariakedark_theme-0.1.3/jupyterlab_ariakedark_theme/labextension/static/lib_index_js.ec0f4e74d248cc0e4f58.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/static/remoteEntry.84696dca1279b4b085e4.js` & `jupyterlab_ariakedark_theme-0.1.3/jupyterlab_ariakedark_theme/labextension/static/remoteEntry.d9c562f8c1deef008056.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -420,15 +420,15 @@
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("jupyterlab_ariakedark_theme", "0.1.1", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("jupyterlab_ariakedark_theme", "0.1.2", () => (__webpack_require__.e("lib_index_js").then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -1056,8 +1056,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/jupyterlab_ariakedark_theme");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB).jupyterlab_ariakedark_theme = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.84696dca1279b4b085e4.js.map
+//# sourceMappingURL=remoteEntry.d9c562f8c1deef008056.js.map
```

### Comparing `jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/static/remoteEntry.84696dca1279b4b085e4.js.map` & `jupyterlab_ariakedark_theme-0.1.3/jupyterlab_ariakedark_theme/labextension/static/remoteEntry.d9c562f8c1deef008056.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9206349206349207%*

 * *Differences: {"'file'": "'remoteEntry.d9c562f8c1deef008056.js'",*

 * * "'sourcesContent'": "{insert: [(10, '__webpack_require__.S = {};\\nvar initPromises = {};\\nvar "*

 * *                     'initTokens = {};\\n__webpack_require__.I = (name, initScope) => '*

 * *                     '{\\n\\tif(!initScope) initScope = [];\\n\\t// handling circular init '*

 * *                     'calls\\n\\tvar initToken = initTokens[name];\\n\\tif(!initToken) initToken = '*

 * *                     'initTokens[name] = {};\\n\\tif(initScope.indexOf(initToke […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.84696dca1279b4b085e4.js",
+    "file": "remoteEntry.d9c562f8c1deef008056.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCjCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA;WACA;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC7CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WC1KA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;UErFA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab_ariakedark_theme/webpack/container-entry",
         "webpack://jupyterlab_ariakedark_theme/webpack/bootstrap",
         "webpack://jupyterlab_ariakedark_theme/webpack/runtime/compat get default export",
@@ -29,15 +29,15 @@
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
         "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + \"ec0f4e74d248cc0e4f58\" + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupyterlab_ariakedark_theme:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyterlab_ariakedark_theme\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab_ariakedark_theme\", \"0.1.1\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"jupyterlab_ariakedark_theme\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab_ariakedark_theme\", \"0.1.2\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && !scriptUrl) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
         "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,4,1,3]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"jupyterlab_ariakedark_theme\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkjupyterlab_ariakedark_theme\"] = self[\"webpackChunkjupyterlab_ariakedark_theme\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/jupyterlab_ariakedark_theme\");\n",
         ""
     ],
```

### Comparing `jupyterlab_ariakedark_theme-0.1.2/jupyterlab_ariakedark_theme/labextension/themes/jupyterlab_ariakedark_theme/index.css` & `jupyterlab_ariakedark_theme-0.1.3/jupyterlab_ariakedark_theme/labextension/themes/jupyterlab_ariakedark_theme/index.css`

 * *Files 0% similar despite different names*

```diff
@@ -329,26 +329,26 @@
   --jp-mirror-editor-atom-color: #93ddfb;
   --jp-mirror-editor-number-color: #dda2f6;
   --jp-mirror-editor-def-color: #85b1e0;
   --jp-mirror-editor-variable-color: #dda2f6;
   --jp-mirror-editor-variable-2-color: #85b1e0;
   --jp-mirror-editor-variable-3-color: #4d8acb;
   --jp-mirror-editor-punctuation-color: #93ddfb;
-  --jp-mirror-editor-property-color: #85b1e0;
+  --jp-mirror-editor-property-color: #7e7edd;
   --jp-mirror-editor-operator-color: #de97f2;
   --jp-mirror-editor-comment-color: #555c77;
   --jp-mirror-editor-string-color: #9aefea;
   --jp-mirror-editor-string-2-color: #93ddfb;
   --jp-mirror-editor-meta-color: #a571f4;
   --jp-mirror-editor-qualifier-color: #7e7edd;
   --jp-mirror-editor-builtin-color: #7673d0;
   --jp-mirror-editor-bracket-color: #6363ab;
   --jp-mirror-editor-tag-color: #85b1e0;
   --jp-mirror-editor-attribute-color: #7ea6d2;
-  --jp-mirror-editor-header-color: #4f5b66;
+  --jp-mirror-editor-header-color: #69f1ad;
   --jp-mirror-editor-quote-color: #dda2f6;
   --jp-mirror-editor-link-color: #7e7edd;
   --jp-mirror-editor-error-color: #e05252;
   --jp-mirror-editor-hr-color: #9aefea;
 
   /* User colors */
```

### Comparing `jupyterlab_ariakedark_theme-0.1.2/src/index.ts` & `jupyterlab_ariakedark_theme-0.1.3/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.2/style/variables.css` & `jupyterlab_ariakedark_theme-0.1.3/style/variables.css`

 * *Files 2% similar despite different names*

```diff
@@ -329,26 +329,26 @@
   --jp-mirror-editor-atom-color: #93ddfb;
   --jp-mirror-editor-number-color: #dda2f6;
   --jp-mirror-editor-def-color: #85b1e0;
   --jp-mirror-editor-variable-color: #dda2f6;
   --jp-mirror-editor-variable-2-color: #85b1e0;
   --jp-mirror-editor-variable-3-color: #4d8acb;
   --jp-mirror-editor-punctuation-color: #93ddfb;
-  --jp-mirror-editor-property-color: #85b1e0;
+  --jp-mirror-editor-property-color: #7e7edd;
   --jp-mirror-editor-operator-color: #de97f2;
   --jp-mirror-editor-comment-color: #555c77;
   --jp-mirror-editor-string-color: #9aefea;
   --jp-mirror-editor-string-2-color: #93ddfb;
   --jp-mirror-editor-meta-color: #a571f4;
   --jp-mirror-editor-qualifier-color: #7e7edd;
   --jp-mirror-editor-builtin-color: #7673d0;
   --jp-mirror-editor-bracket-color: #6363ab;
   --jp-mirror-editor-tag-color: #85b1e0;
   --jp-mirror-editor-attribute-color: #7ea6d2;
-  --jp-mirror-editor-header-color: #4f5b66;
+  --jp-mirror-editor-header-color: #69f1ad;
   --jp-mirror-editor-quote-color: #dda2f6;
   --jp-mirror-editor-link-color: #7e7edd;
   --jp-mirror-editor-error-color: #e05252;
   --jp-mirror-editor-hr-color: #9aefea;
 
   /* User colors */
```

### Comparing `jupyterlab_ariakedark_theme-0.1.2/.gitignore` & `jupyterlab_ariakedark_theme-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.2/LICENSE` & `jupyterlab_ariakedark_theme-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.2/README.md` & `jupyterlab_ariakedark_theme-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.2/pyproject.toml` & `jupyterlab_ariakedark_theme-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_ariakedark_theme-0.1.2/PKG-INFO` & `jupyterlab_ariakedark_theme-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_ariakedark_theme
-Version: 0.1.2
+Version: 0.1.3
 Summary: An ariake dark palette based JupyterLab theme extension.
 Project-URL: Homepage, https://github.com/eduardotlc/jupyterlab_ariakedark_theme
 Project-URL: Bug Tracker, https://github.com/eduardotlc/jupyterlab_ariakedark_theme/issues
 Project-URL: Repository, https://github.com/eduardotlc/jupyterlab_ariakedark_theme.git
 Author-email: Eduardo Campos <eduardotcampos@usp.br>
 License: BSD 3-Clause License
```


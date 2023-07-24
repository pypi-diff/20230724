# Comparing `tmp/yori-1.7.8-py3-none-any.whl.zip` & `tmp/yori-1.7.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 24148 bytes, number of entries: 17
--rwxr-xr-x  2.0 unx     6464 b- defN 20-Feb-02 00:00 yori/IOtools.py
+Zip file size: 24420 bytes, number of entries: 17
+-rwxr-xr-x  2.0 unx     6688 b- defN 20-Feb-02 00:00 yori/IOtools.py
 -rw-r--r--  2.0 unx       22 b- defN 20-Feb-02 00:00 yori/__init__.py
 -rw-r--r--  2.0 unx    14015 b- defN 20-Feb-02 00:00 yori/aggrtools.py
 -rw-r--r--  2.0 unx     4670 b- defN 20-Feb-02 00:00 yori/config_reader.py
 -rw-r--r--  2.0 unx    20221 b- defN 20-Feb-02 00:00 yori/gridtools.py
 -rwxr-xr-x  2.0 unx    10158 b- defN 20-Feb-02 00:00 yori/run_yori.py
--rw-r--r--  2.0 unx    11502 b- defN 20-Feb-02 00:00 yori/yori_aggregate.py
+-rw-r--r--  2.0 unx    12023 b- defN 20-Feb-02 00:00 yori/yori_aggregate.py
 -rw-r--r--  2.0 unx     5807 b- defN 20-Feb-02 00:00 yori/yori_merge.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 yori/tools/__init__.py
--rw-r--r--  2.0 unx     3540 b- defN 20-Feb-02 00:00 yori/tools/aggr.py
+-rw-r--r--  2.0 unx     3966 b- defN 20-Feb-02 00:00 yori/tools/aggr.py
 -rw-r--r--  2.0 unx     1305 b- defN 20-Feb-02 00:00 yori/tools/grid.py
 -rw-r--r--  2.0 unx     2268 b- defN 20-Feb-02 00:00 yori/tools/merge.py
-?rw-r--r--  2.0 unx     1179 b- defN 20-Feb-02 00:00 yori-1.7.8.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 yori-1.7.8.dist-info/WHEEL
-?rw-r--r--  2.0 unx      119 b- defN 20-Feb-02 00:00 yori-1.7.8.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1069 b- defN 20-Feb-02 00:00 yori-1.7.8.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1286 b- defN 20-Feb-02 00:00 yori-1.7.8.dist-info/RECORD
-17 files, 83712 bytes uncompressed, 22084 bytes compressed:  73.6%
+?rw-r--r--  2.0 unx     1179 b- defN 20-Feb-02 00:00 yori-1.7.9.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 yori-1.7.9.dist-info/WHEEL
+?rw-r--r--  2.0 unx      119 b- defN 20-Feb-02 00:00 yori-1.7.9.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1069 b- defN 20-Feb-02 00:00 yori-1.7.9.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1286 b- defN 20-Feb-02 00:00 yori-1.7.9.dist-info/RECORD
+17 files, 84883 bytes uncompressed, 22356 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: yori/tools/grid.py
 Comment: 
 
 Filename: yori/tools/merge.py
 Comment: 
 
-Filename: yori-1.7.8.dist-info/METADATA
+Filename: yori-1.7.9.dist-info/METADATA
 Comment: 
 
-Filename: yori-1.7.8.dist-info/WHEEL
+Filename: yori-1.7.9.dist-info/WHEEL
 Comment: 
 
-Filename: yori-1.7.8.dist-info/entry_points.txt
+Filename: yori-1.7.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: yori-1.7.8.dist-info/licenses/LICENSE
+Filename: yori-1.7.9.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: yori-1.7.8.dist-info/RECORD
+Filename: yori-1.7.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## yori/IOtools.py

```diff
@@ -82,44 +82,47 @@
         dims += (jhisto_primary_name, )
     if jhisto_joint_name != '':
         dims += (jhisto_joint_name, )
 
     return dims
 
 
-def append_attributes(fout, var_settings):
+def append_attributes(fout, var_settings, final=False):
     grp = fout.groups[var_settings['name_out']]
     for var in list(grp.variables):
         setattr(grp[var], 'title', var_settings['name_out'] + ': ' + var)
 
     for attr in var_settings.get('attributes', []):
         if re.search(_fv_re_str, attr['name']) is not None:
-            warnings.warn('FILLVALUE_MISMATCH: There is a mismatch between the FillValue defined ' +
-                          f'in the grid_settings and the {attr["name"]} defined in the attributes, ' +
-                          'please double check your configuration file. See documentation at ' +
-                          f'{_yori_doc} for more info about this warning',
-                          UserWarning)
+            if np.array(attr['name']).dtype == 'int64':
+                warnings.warn('FILLVALUE_MISMATCH: There is a mismatch between the FillValue defined ' +
+                              f'in the grid_settings and the {attr["name"]} defined in the attributes, ' +
+                              'please double check your configuration file. See documentation at ' +
+                              f'{_yori_doc} for more info about this warning',
+                              UserWarning)
         setattr(grp, attr['name'], attr['value'])
 
         if (attr['name'] == 'units'):
             if 'Mean' in list(grp.variables):
                 setattr(grp['Mean'], attr['name'], attr['value'])
             if 'Standard_Deviation' in list(grp.variables):
                 setattr(grp['Standard_Deviation'], attr['name'], attr['value'])
+            if 'Median' in list(grp.variables):
+                setattr(grp['Median'], attr['name'], attr['value'])
 
     if 'histograms' in var_settings:
         if 'edges' in var_settings['histograms']:
             hist_bins = var_settings['histograms']['edges']
             setattr(grp['Histogram_Counts'], 'Histogram_Bin_Boundaries',
                     np.array(hist_bins, dtype='f8'))
         else:
             setattr(grp['Histogram_Counts'], 'Histogram_Bin_Boundaries',
                     compute_hist_bins(var_settings['histograms']))
 
-    if 'median' in var_settings:
+    if 'median' in var_settings and final is False:
         setattr(grp['Median_Distribution'], 'Median_Bins',
                 compute_hist_bins(var_settings['median']))
 
     if '2D_histograms' in var_settings:
         for hist2d in var_settings['2D_histograms']:
             if 'edges' in hist2d['primary_var']:
                 setattr(grp[hist2d['name_out']], 'JHisto_Bin_Boundaries',
```

## yori/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.7.8"
+__version__ = "1.7.9"
```

## yori/yori_aggregate.py

```diff
@@ -19,15 +19,15 @@
 ########################################
 #               FUNCTION               #
 ########################################
 #
 def aggregate(flist, fname_out, satellite='', daily='',
               compression=5, verbose=False, force=False,
               use_min_pixel_counts=False, use_min_valid_days=False,
-              batch_size=2):
+              batch_size=2, final=False):
 
     warnings.simplefilter('module')
 
     f0 = nc.Dataset(flist[0])
     group_list = list(f0.groups)
 
     latdim = f0.dimensions['latitude'].size
@@ -237,14 +237,26 @@
             if 'min_valid_days' in list(grp):
                 grp.pop('min_valid_days')
             if 'Num_Days' in list(grp) and use_min_valid_days is False:
                 grp.pop('Num_Days')
             if 'edges' in list(grp):
                 grp.pop('edges')
 
+            if final is True:
+                if 'Sum' in list(grp):
+                    grp.pop('Sum')
+                if 'Sum_Squares' in list(grp):
+                    grp.pop('Sum_Squares')
+                if 'Weighted_Sum' in list(grp):
+                    grp.pop('Weighted_Sum')
+                if 'Weighted_Sum_Squares' in list(grp):
+                    grp.pop('Weighted_Sum_Squares')
+                if 'Median_Distribution' in list(grp):
+                    grp.pop('Median_Distribution')
+
         var_in = tools.restructDict(var_in)
 
         grid_size = ymlSet.grid_settings['gridsize']
         IO.write_output(nc0, var_in, compression, grid_size, ymlSet, fv)
 
     # write the config file into a variable inside the netcdf output file
     nc0.setncattr('YAML_config', ymlSet.yaml_str)
@@ -252,15 +264,15 @@
     nc0.setncattr('input_files', ','.join(flist))
     nc0.setncattr('daily_defn_of_day_adjustment', str(False))
     if daily != '':
         nc0.setncattr('daily_defn_of_day_adjustment', str(True))
 
     for i in range(len(ymlSet.var_settings)):
         settings = ymlSet.var_settings[i]
-        IO.append_attributes(nc0, settings)
+        IO.append_attributes(nc0, settings, final)
 
     setattr(nc0.variables[latkey], 'units', 'degrees_north')
     setattr(nc0.variables[lonkey], 'units', 'degrees_east')
 
     nc0.close()
```

## yori/tools/aggr.py

```diff
@@ -43,14 +43,19 @@
     parser.add_argument('--min-valid-days', help='set the minimum number of days with ' +
                         'non zero pixel counts in a grid cell in order to be included ' +
                         'in the M3 product', action='store_true')
     parser.add_argument('-b', '--batch-size', help='set batch size for the aggregation ' +
                         'process. Larger batch size can increase speed but requires ' +
                         'more memory. Default is 2, it should be changed with caution.',
                         default=2)
+    parser.add_argument('-F', '--final', help='Create final version of L3 file. All quantities ' +
+                        'used to propagate statistics are deleted (i.e. sum, sum_squares, ' +
+                        '... CAUTION: This operation is irreversible and finalized files ' +
+                        'cannot be processed by Yori anymore',
+                        action='store_true')
     args = parser.parse_args()
 
     # read file list from stdin
     if args.filelist == '-':
         inputs = [l.strip() for l in sys.stdin.read().split('\n') if l.strip()]
 
     # if the file exists, assume it is a file and try to fetch inputs
@@ -65,12 +70,13 @@
               verbose=args.verbose,
               daily=args.daily,
               satellite=args.method,
               force=args.force,
               compression=args.compression,
               use_min_pixel_counts=args.min_pixel_counts,
               use_min_valid_days=args.min_valid_days,
-              batch_size=args.batch_size)
+              batch_size=args.batch_size,
+              final=args.final)
 
 
 if __name__ == "__main__":
     main()
```

## Comparing `yori-1.7.8.dist-info/METADATA` & `yori-1.7.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yori
-Version: 1.7.8
+Version: 1.7.9
 Summary: User-customizable set of tools to easily grid satellite data
 Project-URL: Homepage, https://gitlab.ssec.wisc.edu/pveglio/yori
 Project-URL: Documentation, https://sips.ssec.wisc.edu/docs/yori.html
 Project-URL: Changelog, https://gitlab.ssec.wisc.edu/pveglio/yori/-/blob/master/CHANGELOG.md
 Author-email: Paolo Veglio <paolo.veglio@ssec.wisc.edu>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `yori-1.7.8.dist-info/licenses/LICENSE` & `yori-1.7.9.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `yori-1.7.8.dist-info/RECORD` & `yori-1.7.9.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-yori/IOtools.py,sha256=cgGHKfdloIM4O5RyvHntE8KYXzPWolqgIXlKCuN4eEI,6464
-yori/__init__.py,sha256=3Cq_Tw1FdZarh3Ntzs6fWGvwyLilf-7jlfBYIVOyiyo,22
+yori/IOtools.py,sha256=SoUZV7mC4ULl8EKP3AopsiJSEXTNQxcWR-qUTYD0Bj4,6688
+yori/__init__.py,sha256=YYbFJ4cD7llnUIa-5vWiR7eRAHHLLXAoo9AL_cn_51E,22
 yori/aggrtools.py,sha256=D1i60oCzO1umTAC-IZmDU4S-CSxiWQNPDmEaOUa9cq4,14015
 yori/config_reader.py,sha256=KM3OPxAbvsjxUNsbl_tDMW-Surp2bKt_J-wR3Ge8Vug,4670
 yori/gridtools.py,sha256=dBKJaCfHI5KlD_5rZrhJ9o8c3PivkPuo-EzBKOOmiYU,20221
 yori/run_yori.py,sha256=8QY5XzVmqKy0WQA2BfCgE15ynM4r1kiuvrDfSR38iv8,10158
-yori/yori_aggregate.py,sha256=Kkgi02-DMX0G_GfLbyazOw9VXDx6r40PHOIqD1RD52A,11502
+yori/yori_aggregate.py,sha256=CZSyy5SrdQgkdRLwLc5hmG-QHZHwtyyt7ED1UqsydPc,12023
 yori/yori_merge.py,sha256=QLe2V4N6vULqSEyW0R0XDDLQxf02nTBrNsMicJQBqrY,5807
 yori/tools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-yori/tools/aggr.py,sha256=d58Gd-qbTLyYrJgRjbOY8gcaGy6O0JhGw2jO7sZLuAw,3540
+yori/tools/aggr.py,sha256=NXYpOrI8G3LCRyTpwi95wM-45fMjiiM5CoRqalccSqE,3966
 yori/tools/grid.py,sha256=VbY_NSQnToIctDAB4ZxtDejbYgy7gx3NPW_uaQnNAsI,1305
 yori/tools/merge.py,sha256=CDSGN67OdrY3xAvyPyH6p2fMkmS7ssElv0eSA5sks00,2268
-yori-1.7.8.dist-info/METADATA,sha256=uQ7lFeoRJlVjaR5adYyt2iGrhcz-EdSfSRMAWcZYJhE,1179
-yori-1.7.8.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
-yori-1.7.8.dist-info/entry_points.txt,sha256=5hPsdZbRl0tMHWbUJV-FUkEVMr4C79BZUHDl6jqqtAQ,119
-yori-1.7.8.dist-info/licenses/LICENSE,sha256=ushvHBhEa4gm0SQ2DUAtI0N_ajIlmVfZHEl-VphTk5Y,1069
-yori-1.7.8.dist-info/RECORD,,
+yori-1.7.9.dist-info/METADATA,sha256=MWa3L0i9YkrnLHGa0QhdKW9kRF8pa7ZjfFiSrTG9B7Q,1179
+yori-1.7.9.dist-info/WHEEL,sha256=9QBuHhg6FNW7lppboF2vKVbCGTVzsFykgRQjjlajrhA,87
+yori-1.7.9.dist-info/entry_points.txt,sha256=5hPsdZbRl0tMHWbUJV-FUkEVMr4C79BZUHDl6jqqtAQ,119
+yori-1.7.9.dist-info/licenses/LICENSE,sha256=ushvHBhEa4gm0SQ2DUAtI0N_ajIlmVfZHEl-VphTk5Y,1069
+yori-1.7.9.dist-info/RECORD,,
```


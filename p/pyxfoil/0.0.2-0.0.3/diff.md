# Comparing `tmp/pyxfoil-0.0.2.tar.gz` & `tmp/pyxfoil-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxfoil-0.0.2.tar", last modified: Fri Feb 24 14:31:35 2023, max compression
+gzip compressed data, was "pyxfoil-0.0.3.tar", last modified: Mon Jul 24 16:00:44 2023, max compression
```

## Comparing `pyxfoil-0.0.2.tar` & `pyxfoil-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:31:35.881924 pyxfoil-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-02-24 14:31:25.000000 pyxfoil-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-02-24 14:31:35.881924 pyxfoil-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-02-24 14:31:25.000000 pyxfoil-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:31:35.881924 pyxfoil-0.0.2/pyxfoil/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-02-24 14:31:25.000000 pyxfoil-0.0.2/pyxfoil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-02-24 14:31:25.000000 pyxfoil-0.0.2/pyxfoil/xfoil.py
--rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-02-24 14:31:25.000000 pyxfoil-0.0.2/pyxfoil/xfoilpolar.py
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-02-24 14:31:25.000000 pyxfoil-0.0.2/pyxfoil/xfoilresult.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 14:31:35.881924 pyxfoil-0.0.2/pyxfoil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-02-24 14:31:35.000000 pyxfoil-0.0.2/pyxfoil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-24 14:31:35.000000 pyxfoil-0.0.2/pyxfoil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 14:31:35.000000 pyxfoil-0.0.2/pyxfoil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-24 14:31:35.000000 pyxfoil-0.0.2/pyxfoil.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 14:31:35.881924 pyxfoil-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-02-24 14:31:25.000000 pyxfoil-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:00:44.140273 pyxfoil-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-24 16:00:30.000000 pyxfoil-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-24 16:00:44.140273 pyxfoil-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-24 16:00:30.000000 pyxfoil-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:00:44.140273 pyxfoil-0.0.3/pyxfoil/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-24 16:00:30.000000 pyxfoil-0.0.3/pyxfoil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-07-24 16:00:30.000000 pyxfoil-0.0.3/pyxfoil/xfoil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-07-24 16:00:30.000000 pyxfoil-0.0.3/pyxfoil/xfoilpolar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-24 16:00:30.000000 pyxfoil-0.0.3/pyxfoil/xfoilresult.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:00:44.140273 pyxfoil-0.0.3/pyxfoil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-24 16:00:44.000000 pyxfoil-0.0.3/pyxfoil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-24 16:00:44.000000 pyxfoil-0.0.3/pyxfoil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:00:44.000000 pyxfoil-0.0.3/pyxfoil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-24 16:00:44.000000 pyxfoil-0.0.3/pyxfoil.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 16:00:44.140273 pyxfoil-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-24 16:00:30.000000 pyxfoil-0.0.3/setup.py
```

### Comparing `pyxfoil-0.0.2/LICENSE` & `pyxfoil-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxfoil-0.0.2/README.md` & `pyxfoil-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # pyxfoil
 Run XFoil from within Python and work with output results.
 
 See example below:
 
-
 #
 ``` python
 # Import Dependencies
-from pyxfoil import Xfoil, set_workdir
-set_workdir('C:/Xfoil_WIP') # Sets the working directory for pyxfoil
+from pyxfoil import Xfoil, set_workdir#, set_xfoilexe
+set_workdir('C:/Xfoil_WIP') # Sets the working directory for pyxfoil.
+# set_xfoilexe('C:/Xfoil-6.99/xfoil.exe') # Sets the path of the xfoil executable.
 ```
 
 #
 ``` python
 # Creates Xfoil object from reading dat file.
 xfoil = Xfoil('NACA 0012')
 xfoil.points_from_dat('../files/NACA_0012_180.dat')
```

### Comparing `pyxfoil-0.0.2/pyxfoil/__init__.py` & `pyxfoil-0.0.3/pyxfoil/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxfoil-0.0.2/pyxfoil/xfoil.py` & `pyxfoil-0.0.3/pyxfoil/xfoil.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,16 +9,18 @@
     name: 'str' = None
     ppar: 'int' = None
     x: List['float'] = None
     y: List['float'] = None
     results: Dict['str', 'XfoilResult'] = None
     polars: Dict['str', 'XfoilPolar'] = None
     _area: 'float' = None
+
     def __init__(self, name: 'str') -> None:
         self.name = name
+
     def points_from_dat(self, datfile: 'str') -> None:
         self.x = []
         self.y = []
         with open(datfile, 'rt') as file:
             for i, line in enumerate(file):
                 line = line.rstrip('\n')
                 if i == 0:
@@ -27,85 +29,114 @@
                     split = line.split()
                     if len(split) == 2:
                         x = float(split[0])
                         y = float(split[1])
                         self.x.append(x)
                         self.y.append(y)
         self._area = None
+
     def set_points(self, x: List['float'], y: List['float']) -> None:
         self.x = x
         self.y = y
         self._area = None
+
     def set_ppar(self, ppar: 'int') -> None:
         self.ppar = ppar
+
     @property
     def area(self) -> 'float':
         if self._area is None:
             self._area = 0.0
             for i in range(1, len(self.x)):
                 self._area += self.x[i]*self.y[i-1]-self.y[i]*self.x[i-1]
             if self.x[0] != self.x[-1] or self.y[0] != self.y[-1]:
                 self._area += self.x[0]*self.y[-1]-self.y[0]*self.x[-1]
         return self._area
+
     def write_dat(self) -> 'str':
+
         from pyxfoil import workdir
+
         datname = self.name.replace(' ', '_')
         filepath = join(workdir, datname)
         datfilepath = f'{filepath:s}.dat'
         num = len(self.x)
         if self.area >= 0:
             order = range(num-1, -1, -1)
         else:
             order = range(num)
         frmstr = '  {:11.6f} {:11.6f}\n'
         with open(datfilepath, 'wt') as file:
             file.write(self.name+'\n')
             for i in order:
                 file.write(frmstr.format(self.x[i], self.y[i]))
         return datfilepath
+
     def run_result(self, alfa: 'float', re: 'float'=None,
                    mach: 'float'=None) -> 'XfoilResult':
+
         from pyxfoil import xfoilexe
+
         datfilepath = self.write_dat()
         numpnl = len(self.x) - 1
         sesfilepath, resfilepath = write_result_session(self.name, datfilepath, numpnl,
                                                         alfa, mach=mach, re=re,
                                                         ppar=self.ppar)
+
         if isfile(resfilepath):
             remove(resfilepath)
+
+        if xfoilexe is None:
+            err = 'Cannot locate "xfoil.exe" in path. '
+            err += 'Import set_xfoilexe and use it to directly point to "xfoil.exe".'
+            raise SystemError(err)
+
         system('{:s} < {:s}'.format(xfoilexe, sesfilepath))
+
         res = split(resfilepath)[1]
         res = res.replace('.res', '')
         result = XfoilResult(res, numpnl)
         result.set_param(alfa, mach, re)
         result.read_result(resfilepath)
         if self.results is None:
             self.results = {}
         self.results[res] = result
         return result
+
     def run_polar(self, almin: 'float', almax: 'float', alint: 'float',
                   re: 'float'=None, mach: 'float'=None) -> 'XfoilPolar':
+
         from pyxfoil import xfoilexe
+
         datfilepath = self.write_dat()
         numpnl = len(self.x) - 1
         sesfilepath, polfilepath = write_polar_session(self.name, datfilepath,
                                                        numpnl, almin, almax, alint,
                                                        mach=mach, re=re,
                                                        ppar=self.ppar)
+
         if isfile(polfilepath):
             remove(polfilepath)
+
+        if xfoilexe is None:
+            err = 'Cannot locate "xfoil.exe" in path. '
+            err += 'Import set_xfoilexe and use it to directly point to "xfoil.exe".'
+            raise SystemError(err)
+
         system('{:s} < {:s}'.format(xfoilexe, sesfilepath))
+
         pol: 'str' = split(polfilepath)[1]
         pol = pol.replace('.pol', '')
         polar = XfoilPolar(pol, numpnl)
         polar.read_polar(polfilepath)
         if self.polars is None:
             self.polars = {}
         self.polars[pol] = polar
         return polar
+
     def plot_profile(self, *args, **kwargs):
         grid = kwargs.get('grid', True)
         aspect = kwargs.get('aspect', 'equal')
         figsize = kwargs.get('figsize', (12, 8))
         fig = figure(figsize=figsize)
         ax = fig.gca()
         ax.plot(self.x, self.y, *args, **kwargs)
```

### Comparing `pyxfoil-0.0.2/pyxfoil/xfoilpolar.py` & `pyxfoil-0.0.3/pyxfoil/xfoilpolar.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,19 @@
     alpha: List['float'] = None
     cl: List['float'] = None
     cd: List['float'] = None
     cdp: List['float'] = None
     cm: List['float'] = None
     trtop: List['float'] = None
     trbot: List['float'] = None
+
     def __init__(self, name: 'str', numpnl: 'int') -> None:
         self.name = name
         self.numpnl = numpnl
+
     def read_polar(self, filepath: str) -> None:
         self.alpha = []
         self.cl = []
         self.cd = []
         self.cdp = []
         self.cm = []
         self.trtop = []
@@ -50,19 +52,21 @@
                         self.alpha.append(float(line[0:8]))
                         self.cl.append(float(line[8:17]))
                         self.cd.append(float(line[17:27]))
                         self.cdp.append(float(line[27:37]))
                         self.cm.append(float(line[37:46]))
                         self.trtop.append(float(line[46:55]))
                         self.trbot.append(float(line[55:64]))
+
     @property
     def clocd(self) -> Optional[List['float']]:
         if self.cl is not None and self.cd is not None:
             clocdval = [cli/cdi for cli, cdi in zip(self.cl, self.cd)]
             return clocdval
+
     def plot_polar(self, xaxis='cd', yaxis='cl', ax=None, *args, **kwargs):
         figsize = kwargs.get('figsize', (12, 8))
         if ax is None:
             from matplotlib.pyplot import figure
             fig = figure(figsize=figsize)
             ax = fig.gca()
             title = r'Polar plot for $M = {:g}$ and $Re = {:.12g}$'
@@ -80,14 +84,15 @@
             label += r'; '
         if self.mach is not None:
             label += r'$M = {:g}$'.format(self.mach)
         xvalue = self.get_value(xaxis)
         yvalue = self.get_value(yaxis)
         ax.plot(xvalue, yvalue, *args, label=label)
         return ax
+
     def get_label(self, var: 'str') -> 'str':
         if var == 'alpha':
             label = r'$\alpha$'
         elif var == 'cl':
             label = '$C_l$'
         elif var == 'cd':
             label = '$C_d$'
@@ -100,14 +105,15 @@
         elif var == 'th':
             label = r'$Bottom X Transition$'
         elif var == 'clocd':
             label = r'$\frac{c_l}{c_d}$'
         else:
             raise ValueError(f'{var:s} does not exist in XfoilPolar.')
         return label
+
     def get_value(self, var: 'str') -> List['float']:
         if var == 'alpha':
             value = self.alpha
         elif var == 'cl':
             value = self.cl
         elif var == 'cd':
             value = self.cd
@@ -120,23 +126,26 @@
         elif var == 'th':
             value = self.trbot
         elif var == 'clocd':
             value = self.clocd
         else:
             raise ValueError(f'{var:s} does not exist in XfoilPolar.')
         return value
+
     def __repr__(self) -> str:
         return f'<pyxfoil.XfoilPolar {self.name:s}>'
 
 def write_polar_session(name: 'str', datfilepath: 'str', numpnl: 'int',
                         almin: 'float', almax: 'float', alint: 'float',
                         mach: Optional['float']=None,
                         re: Optional['float']=None,
                         ppar: Optional['int']=None) -> Tuple['str', 'str']:
+
     from pyxfoil import workdir
+    
     polname = name.replace(' ', '_') + f'_{numpnl:d}'
     if mach is not None:
         polname += f'_{mach:g}'
     if re is not None:
         polname += f'_{re:.12g}'
     filepath = join(workdir, polname)
     sesfilepath = f'{filepath:s}.ses'
```

### Comparing `pyxfoil-0.0.2/pyxfoil/xfoilresult.py` & `pyxfoil-0.0.3/pyxfoil/xfoilresult.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,21 +13,24 @@
     ue: List['float'] = None
     ds: List['float'] = None
     th: List['float'] = None
     cf: List['float'] = None
     h: List['float'] = None
     resfile: 'str' = None
     _cp: List['float'] = None
+
     def __init__(self, name: 'str', numpnl: 'int') -> None:
         self.name = name
         self.numpnl = numpnl
+
     def set_param(self, alpha: 'float', mach: 'float', re: 'float') -> None:
         self.alpha = alpha
         self.mach = mach
         self.re = re
+
     def read_result(self, resfile: 'str') -> None:
         with open(resfile, 'rt') as f:
             self.s = []
             self.x = []
             self.y = []
             self.ue = []
             self.ds = []
@@ -43,19 +46,21 @@
                         self.y.append(float(line[20:29]))
                         self.ue.append(float(line[29:38]))
                         self.ds.append(float(line[38:48]))
                         self.th.append(float(line[48:58]))
                         self.cf.append(float(line[58:68]))
                         self.h.append(float(line[68:78]))
         self._cp = None
+
     @property
     def cp(self) -> List['float']:
         if self._cp is None:
             self._cp = [1-uei**2 for uei in self.ue]
         return self._cp
+
     def plot_result(self, xaxis='x', yaxis='ue', ax=None, *args, **kwargs):
         figsize = kwargs.get('figsize', (12, 8))
         if ax is None:
             from matplotlib.pyplot import figure
             fig = figure(figsize=figsize)
             ax = fig.gca()
             grid = kwargs.get('grid', True)
@@ -77,27 +82,29 @@
             label += r'; $Re = {:.12g}$'.format(self.re)
         if self.mach is not None:
             label += r'; $M = {:g}$'.format(self.mach)
         xvalue = self.get_value(xaxis)
         yvalue = self.get_value(yaxis)
         ax.plot(xvalue, yvalue, *args, label=label)
         return ax
+
     def result(self, var: 'str', correct: 'bool'=False) -> List['float']:
         res = self.get_value(var)
         if correct:
             if var == 's':
                 offset = max(res[:self.numpnl+1])
                 val = [offset-resi for resi in res[:self.numpnl+1]]
             else:
                 val = [resi for resi in res[:self.numpnl+1]]
             val.reverse()
             val = val + res[self.numpnl+1:]
         else:
             val = res.copy()
         return val
+
     def get_label(self, var: 'str') -> 'str':
         if var == 'x':
             label = '$x$'
         elif var == 'y':
             label = '$y$'
         elif var == 's':
             label = '$s$'
@@ -112,14 +119,15 @@
         elif var == 'h':
             label = '$h$'
         elif var == 'cf':
             label = '$c_f$'
         else:
             raise ValueError(f'{var:s} does not exist in XfoilResult.')
         return label
+
     def get_value(self, var: 'str') -> List['float']:
         if var == 'x':
             value = self.x
         elif var == 'y':
             value = self.y
         elif var == 's':
             value = self.s
@@ -134,22 +142,25 @@
         elif var == 'h':
             value = self.h
         elif var == 'cf':
             value = self.cf
         else:
             raise ValueError(f'{var:s} does not exist in XfoilResult.')
         return value
+
     def __repr__(self) -> str:
         return f'<pyxfoil.XfoilResult {self.name:s}>'
 
 def write_result_session(name: 'str', datfilepath: 'str', numpnl: 'int',
                          alpha: 'float', mach: Optional['float']=None,
                          re: Optional['float']=None,
                          ppar: Optional['int']=None) -> Tuple['str', 'str']:
+
     from pyxfoil import workdir
+
     resname = name.replace(' ', '_')
     resname += f'_{numpnl:d}_{alpha:g}'
     if mach is not None:
         resname += f'_{mach:g}'
     if re is not None:
         resname += f'_{re:.12g}'
     filepath = join(workdir, resname)
```

### Comparing `pyxfoil-0.0.2/setup.py` & `pyxfoil-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = '''
     Run XFoil from within Python and work with output results.
     '''
 
 setup(
     name="pyxfoil",
-    version="0.0.2",
+    version="0.0.3",
     author="Xero64",
     author_email="xero64@gmail.com",
     description="Run XFoil from within Python and work with output results.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Xero64/pyxfoil",
     packages=find_packages(),
```


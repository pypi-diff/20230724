# Comparing `tmp/eztils-0.4.7.tar.gz` & `tmp/eztils-0.4.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eztils-0.4.7.tar", max compression
+gzip compressed data, was "eztils-0.4.71.tar", max compression
```

## Comparing `eztils-0.4.7.tar` & `eztils-0.4.71.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1075 2023-07-23 00:52:06.291815 eztils-0.4.7/LICENSE
--rw-r--r--   0        0        0    12741 2023-07-23 00:52:06.291815 eztils-0.4.7/README.md
--rw-r--r--   0        0        0      542 2023-07-23 00:52:06.291815 eztils-0.4.7/eztils/__init__.py
--rw-r--r--   0        0        0     2465 2023-07-23 00:52:06.291815 eztils-0.4.7/eztils/default/__init__.py
--rw-r--r--   0        0        0     3689 2023-07-23 00:52:06.291815 eztils-0.4.7/eztils/default/dict_operations.py
--rw-r--r--   0        0        0     2246 2023-07-23 00:52:06.291815 eztils-0.4.7/eztils/default/itertools.py
--rw-r--r--   0        0        0     2458 2023-07-23 00:52:06.291815 eztils-0.4.7/eztils/default/logging.py
--rw-r--r--   0        0        0     1432 2023-07-23 00:52:06.291815 eztils-0.4.7/eztils/default/math.py
--rw-r--r--   0        0        0     1091 2023-07-23 00:52:06.291815 eztils-0.4.7/eztils/default/structures.py
--rw-r--r--   0        0        0     4296 2023-07-23 00:52:06.291815 eztils-0.4.7/eztils/git/__init__.py
--rw-r--r--   0        0        0     1607 2023-07-23 00:52:06.291815 eztils-0.4.7/eztils/torch/__init__.py
--rw-r--r--   0        0        0    15657 2023-07-23 00:52:06.291815 eztils-0.4.7/eztils/torch/distributions.py
--rw-r--r--   0        0        0      155 2023-07-23 00:52:06.291815 eztils-0.4.7/eztils/torch/lightning.py
--rw-r--r--   0        0        0      173 2023-07-23 00:52:06.291815 eztils-0.4.7/eztils/torch/math.py
--rw-r--r--   0        0        0     2550 2023-07-23 00:52:06.291815 eztils-0.4.7/eztils/torch/modules.py
--rw-r--r--   0        0        0     1420 2023-07-23 00:52:06.291815 eztils-0.4.7/eztils/torch/parameters.py
--rw-r--r--   0        0        0     1746 2023-07-23 00:52:06.291815 eztils-0.4.7/eztils/torch/tensor_creators.py
--rw-r--r--   0        0        0     2929 2023-07-23 00:52:06.291815 eztils-0.4.7/eztils/torch/to.py
--rw-r--r--   0        0        0     3618 2023-07-23 00:52:06.291815 eztils-0.4.7/pyproject.toml
--rw-r--r--   0        0        0    13903 1970-01-01 00:00:00.000000 eztils-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-24 06:09:32.639912 eztils-0.4.71/LICENSE
+-rw-r--r--   0        0        0    12741 2023-07-24 06:09:32.639912 eztils-0.4.71/README.md
+-rw-r--r--   0        0        0      542 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/__init__.py
+-rw-r--r--   0        0        0     2494 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/default/__init__.py
+-rw-r--r--   0        0        0     3689 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/default/dict_operations.py
+-rw-r--r--   0        0        0     2246 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/default/itertools.py
+-rw-r--r--   0        0        0     2458 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/default/logging.py
+-rw-r--r--   0        0        0     1432 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/default/math.py
+-rw-r--r--   0        0        0     2812 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/default/serialization.py
+-rw-r--r--   0        0        0     1091 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/default/structures.py
+-rw-r--r--   0        0        0     4296 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/git/__init__.py
+-rw-r--r--   0        0        0     1779 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/torch/__init__.py
+-rw-r--r--   0        0        0    15657 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/torch/distributions.py
+-rw-r--r--   0        0        0      155 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/torch/lightning.py
+-rw-r--r--   0        0        0      173 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/torch/math.py
+-rw-r--r--   0        0        0     2550 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/torch/modules.py
+-rw-r--r--   0        0        0     1420 2023-07-24 06:09:32.639912 eztils-0.4.71/eztils/torch/parameters.py
+-rw-r--r--   0        0        0     1746 2023-07-24 06:09:32.643912 eztils-0.4.71/eztils/torch/tensor_creators.py
+-rw-r--r--   0        0        0     3001 2023-07-24 06:09:32.643912 eztils-0.4.71/eztils/torch/to.py
+-rw-r--r--   0        0        0     3611 2023-07-24 06:09:32.643912 eztils-0.4.71/pyproject.toml
+-rw-r--r--   0        0        0    13946 1970-01-01 00:00:00.000000 eztils-0.4.71/PKG-INFO
```

### Comparing `eztils-0.4.7/LICENSE` & `eztils-0.4.71/LICENSE`

 * *Files identical despite different names*

### Comparing `eztils-0.4.7/README.md` & `eztils-0.4.71/README.md`

 * *Files identical despite different names*

### Comparing `eztils-0.4.7/eztils/__init__.py` & `eztils-0.4.71/eztils/__init__.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.7/eztils/default/__init__.py` & `eztils-0.4.71/eztils/default/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,8 +77,9 @@
 frozen_enforced_dataclass = beartype(dataclass(frozen=True))
 
 
 from .dict_operations import *
 from .itertools import *
 from .logging import *
 from .math import *
+from .serialization import *
 from .structures import *
```

### Comparing `eztils-0.4.7/eztils/default/dict_operations.py` & `eztils-0.4.71/eztils/default/dict_operations.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.7/eztils/default/itertools.py` & `eztils-0.4.71/eztils/default/itertools.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.7/eztils/default/logging.py` & `eztils-0.4.71/eztils/default/logging.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.7/eztils/default/math.py` & `eztils-0.4.71/eztils/default/math.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.7/eztils/default/structures.py` & `eztils-0.4.71/eztils/default/structures.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.7/eztils/git/__init__.py` & `eztils-0.4.71/eztils/git/__init__.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.7/eztils/torch/__init__.py` & `eztils-0.4.71/eztils/torch/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """
 import often used modules
 """
 import random
-from pathlib import Path
+from functools import partial
 
 import numpy as np
 import torch
 from einops import rearrange as rea
 from einops import reduce
 
 try:
     from jaxtyping import Bool, Float, Float16, Float32, Int
 except RuntimeError:  # python < 3.9
     pass
 from torch import einsum, nn, tensor
 from torch.nn import functional as F
 from torchvision.utils import save_image
 
+from eztils import load, save
+
 """
 globals
 """
 USE_GPU = False
 DTYPE = torch.float
 GPU_ID = 0
 DEVICE = None
@@ -65,14 +67,18 @@
     np.random.seed(seed)
     torch.manual_seed(seed)
 
     if torch.cuda.is_available():
         torch.cuda.manual_seed_all(seed)
 
 
+save = partial(save, save_fn=torch.save)
+torch.load = partial(torch.load, map_location="cpu")
+load = partial(load, load_fn=torch.load)
+
 from .distributions import *
 from .lightning import *
 from .math import *
 from .modules import *
 from .parameters import *
 from .tensor_creators import *
 from .to import *
```

### Comparing `eztils-0.4.7/eztils/torch/distributions.py` & `eztils-0.4.71/eztils/torch/distributions.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.7/eztils/torch/modules.py` & `eztils-0.4.71/eztils/torch/modules.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.7/eztils/torch/parameters.py` & `eztils-0.4.71/eztils/torch/parameters.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.7/eztils/torch/tensor_creators.py` & `eztils-0.4.71/eztils/torch/tensor_creators.py`

 * *Files identical despite different names*

### Comparing `eztils-0.4.7/eztils/torch/to.py` & `eztils-0.4.71/eztils/torch/to.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Any, Union
 
+import functools
+
 import numpy as np
 import torch
 
 from eztils import normalize
 
 
 def to_np(x):
@@ -88,7 +90,10 @@
     elif hasattr(input, "to"):
         # noinspection PyCallingNonCallable
         return input.to(device=device, inplace=inplace)
     else:
         raise NotImplementedError(
             f"Sorry, value of type {type(input)} is not supported."
         )
+
+
+to_cpu = functools.partial(to_device, device="cpu")
```

### Comparing `eztils-0.4.7/pyproject.toml` & `eztils-0.4.71/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -7,22 +7,21 @@
 authors = ["ezhang7423 <ezhang7423@student.palomar.edu>"]
 description = "eds utilities"
 homepage = "https://github.com/ezhang7423/eztils"
 license = "MIT"
 name = "eztils"
 readme = "README.md"
 repository = "https://github.com/ezhang7423/eztils"
-version = "0.4.7"
+version = "0.4.71"
 
 # Keywords description https://python-poetry.org/docs/pyproject/#keywords
-keywords = [] #! Update me
+keywords = []
 
 # Pypi classifiers: https://pypi.org/classifiers/
 classifiers = [
-  #! Update me
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
@@ -35,14 +34,15 @@
 einops = "^0.6.1"
 ezjaxtyping = {version = "^0.2.20", optional = true}
 loguru = "^0.7.0"
 numpy = "^1.24.3"
 python = "^3.8"
 rich = "^13.3.3"
 tqdm = "^4.65.0"
+varname = "^0.11.2"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.5"
 black = "^23.3.0"
 coverage = "^7.2.2"
 coverage-badge = "^1.1.0"
 darglint = "^1.8.1"
```

### Comparing `eztils-0.4.7/PKG-INFO` & `eztils-0.4.71/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eztils
-Version: 0.4.7
+Version: 0.4.71
 Summary: eds utilities
 Home-page: https://github.com/ezhang7423/eztils
 License: MIT
 Author: ezhang7423
 Author-email: ezhang7423@student.palomar.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -21,14 +21,15 @@
 Requires-Dist: beartype (>=0.14.1,<0.15.0)
 Requires-Dist: einops (>=0.6.1,<0.7.0)
 Requires-Dist: ezjaxtyping (>=0.2.20,<0.3.0) ; extra == "torch"
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: rich (>=13.3.3,<14.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: varname (>=0.11.2,<0.12.0)
 Project-URL: Repository, https://github.com/ezhang7423/eztils
 Description-Content-Type: text/markdown
 
 # eztils
 
 <div align="center">
```


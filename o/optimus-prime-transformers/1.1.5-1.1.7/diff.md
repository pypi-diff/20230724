# Comparing `tmp/optimus-prime-transformers-1.1.5.tar.gz` & `tmp/optimus-prime-transformers-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimus-prime-transformers-1.1.5.tar", last modified: Sat May 27 08:35:10 2023, max compression
+gzip compressed data, was "optimus-prime-transformers-1.1.7.tar", last modified: Mon Jul 24 13:55:44 2023, max compression
```

## Comparing `optimus-prime-transformers-1.1.5.tar` & `optimus-prime-transformers-1.1.7.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:35:10.965114 optimus-prime-transformers-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-27 08:35:00.000000 optimus-prime-transformers-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-27 08:35:10.965114 optimus-prime-transformers-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    63442 2023-05-27 08:35:00.000000 optimus-prime-transformers-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:35:10.965114 optimus-prime-transformers-1.1.5/optimus_prime_transformers/
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-27 08:35:00.000000 optimus-prime-transformers-1.1.5/optimus_prime_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-05-27 08:35:00.000000 optimus-prime-transformers-1.1.5/optimus_prime_transformers/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-27 08:35:00.000000 optimus-prime-transformers-1.1.5/optimus_prime_transformers/autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-27 08:35:00.000000 optimus-prime-transformers-1.1.5/optimus_prime_transformers/continuous_autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-05-27 08:35:00.000000 optimus-prime-transformers-1.1.5/optimus_prime_transformers/nonautoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    54747 2023-05-27 08:35:00.000000 optimus-prime-transformers-1.1.5/optimus_prime_transformers/x_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-05-27 08:35:00.000000 optimus-prime-transformers-1.1.5/optimus_prime_transformers/xl_autoregressive_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:35:10.965114 optimus-prime-transformers-1.1.5/optimus_prime_transformers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-27 08:35:10.000000 optimus-prime-transformers-1.1.5/optimus_prime_transformers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-27 08:35:10.000000 optimus-prime-transformers-1.1.5/optimus_prime_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 08:35:10.000000 optimus-prime-transformers-1.1.5/optimus_prime_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-27 08:35:10.000000 optimus-prime-transformers-1.1.5/optimus_prime_transformers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-27 08:35:10.000000 optimus-prime-transformers-1.1.5/optimus_prime_transformers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 08:35:10.965114 optimus-prime-transformers-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-27 08:35:00.000000 optimus-prime-transformers-1.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:55:44.691435 optimus-prime-transformers-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-24 13:55:27.000000 optimus-prime-transformers-1.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-24 13:55:44.691435 optimus-prime-transformers-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    63442 2023-07-24 13:55:27.000000 optimus-prime-transformers-1.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:55:44.691435 optimus-prime-transformers-1.1.7/optimus_prime/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-24 13:55:27.000000 optimus-prime-transformers-1.1.7/optimus_prime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-07-24 13:55:27.000000 optimus-prime-transformers-1.1.7/optimus_prime/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-24 13:55:27.000000 optimus-prime-transformers-1.1.7/optimus_prime/autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-24 13:55:27.000000 optimus-prime-transformers-1.1.7/optimus_prime/continuous_autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-07-24 13:55:27.000000 optimus-prime-transformers-1.1.7/optimus_prime/flash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-07-24 13:55:27.000000 optimus-prime-transformers-1.1.7/optimus_prime/nonautoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55309 2023-07-24 13:55:27.000000 optimus-prime-transformers-1.1.7/optimus_prime/x_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-07-24 13:55:27.000000 optimus-prime-transformers-1.1.7/optimus_prime/xl_autoregressive_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:55:44.691435 optimus-prime-transformers-1.1.7/optimus_prime_transformers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-24 13:55:44.000000 optimus-prime-transformers-1.1.7/optimus_prime_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-24 13:55:44.000000 optimus-prime-transformers-1.1.7/optimus_prime_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:55:44.000000 optimus-prime-transformers-1.1.7/optimus_prime_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-24 13:55:44.000000 optimus-prime-transformers-1.1.7/optimus_prime_transformers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 13:55:44.000000 optimus-prime-transformers-1.1.7/optimus_prime_transformers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:55:44.691435 optimus-prime-transformers-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-24 13:55:27.000000 optimus-prime-transformers-1.1.7/setup.py
```

### Comparing `optimus-prime-transformers-1.1.5/LICENSE` & `optimus-prime-transformers-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.5/PKG-INFO` & `optimus-prime-transformers-1.1.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimus-prime-transformers
-Version: 1.1.5
+Version: 1.1.7
 Summary: optimus-prime - Pytorch
 Home-page: https://github.com/kyegomez/Optimus-Prime
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `optimus-prime-transformers-1.1.5/README.md` & `optimus-prime-transformers-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.5/optimus_prime_transformers/attend.py` & `optimus-prime-transformers-1.1.7/optimus_prime/attend.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from collections import namedtuple
 from functools import wraps
 from packaging import version
 from dataclasses import dataclass
 
 from einops import rearrange
 
+# from flash import FlashAttention
+
 # constants
 
 EfficientAttentionConfig = namedtuple('EfficientAttentionConfig', ['enable_flash', 'enable_math', 'enable_mem_efficient'])
 
 @dataclass
 class Intermediates:
     qk_similarities: Tensor = None
@@ -192,14 +194,15 @@
         n, device = q.shape[-2], q.device
 
         scale = default(self.scale, q.shape[-1] ** -0.5)
 
         if self.flash:
             assert not exists(prev_attn), 'residual attention not compatible with flash attention'
             return self.flash_attn(q, k, v, mask = mask, attn_bias = attn_bias)
+            # return FlashAttention(q, k, v, mask=mask, attn_bias=attn_bias )
 
         kv_einsum_eq = 'b j d' if k.ndim == 3 else 'b h j d'
 
         dots = einsum(f'b h i d, {kv_einsum_eq} -> b h i j', q, k) * scale
 
         if exists(prev_attn):
             dots = dots + prev_attn
```

### Comparing `optimus-prime-transformers-1.1.5/optimus_prime_transformers/autoregressive_wrapper.py` & `optimus-prime-transformers-1.1.7/optimus_prime/autoregressive_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 
         out = out[:, t:]
 
         out, = unpack(out, ps, '* n')
 
         return out
 
-    def forward(self, x, **kwargs):
+    def forward(self, x, return_loss=True, **kwargs):
         seq, ignore_index = x.shape[1], self.ignore_index
 
         inp, target = x[:, :-1], x[:, 1:]
 
         if self.mask_prob > 0.:
             rand = torch.randn(inp.shape, device = x.device)
             rand[:, 0] = -torch.finfo(rand.dtype).max # first token should not be masked out
@@ -142,8 +142,11 @@
 
         loss = F.cross_entropy(
             rearrange(logits, 'b n c -> b c n'),
             target,
             ignore_index = ignore_index
         )
 
-        return loss
+        if return_loss:
+            return logits, loss
+
+        return logits
```

### Comparing `optimus-prime-transformers-1.1.5/optimus_prime_transformers/continuous_autoregressive_wrapper.py` & `optimus-prime-transformers-1.1.7/optimus_prime/continuous_autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.1.5/optimus_prime_transformers/nonautoregressive_wrapper.py` & `optimus-prime-transformers-1.1.7/optimus_prime/nonautoregressive_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 import torch
 import torch.nn.functional as F
 from torch import nn
 
 from einops import rearrange, repeat, pack, unpack
 
-# from optimus_prime_transformers.optimus_prime import TransformerWrapper
-from x_transformers import TransformerWrapper
+
+from optimus_prime.x_transformers import TransformerWrapper
 from typing import Optional
 
 # constants
 
 Losses = namedtuple('Losses', ['loss', 'generator_loss', 'critic_loss'])
 
 # helper functions
```

### Comparing `optimus-prime-transformers-1.1.5/optimus_prime_transformers/x_transformers.py` & `optimus-prime-transformers-1.1.7/optimus_prime/x_transformers.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,26 +13,27 @@
 from collections import namedtuple
 from dataclasses import dataclass
 from typing import List
 
 from einops import rearrange, repeat, reduce
 from einops.layers.torch import Rearrange
 
-from optimus_prime_transformers.attend import Attend, Intermediates
-from optimus_prime_transformers.autoregressive_wrapper import AutoregressiveWrapper
+from optimus_prime.attend import Attend, Intermediates
+from optimus_prime.autoregressive_wrapper import AutoregressiveWrapper
 
 from abc import ABC, abstractmethod
+# import bitsandbytes as bnb
 
 # constants
 
 DEFAULT_DIM_HEAD = 64
 
 @dataclass
 class LayerIntermediates:
-    hiddens: List[Tensor] = None,
+    hiddens: List[Tensor] = None
     attn_intermediates: List[Intermediates] = None
 
 # helpers
 
 def exists(val):
     return val is not None
 
@@ -189,25 +190,37 @@
         return tokens
 
 # embedding
 
 class BaseEmbedding(ABC):
     @abstractmethod
     def get_embedding(self, num_tokens: int, dim: int) -> nn.Module:
-        #custom embedding function or model
+        # Custom embedding function or model
         embedding = ...
+        
+        return embedding
+
+class AndromedaEmbedding(BaseEmbedding):
+    def get_embedding(self, num_tokens: int, dim: int) -> nn.Module:
+        embedding = nn.Embedding(num_tokens, dim)
+
         return embedding
     
+# class AndromedaBnBEmbedding(BaseEmbedding):
+#     def get_embedding(self, num_tokens: int, dim: int, padding_idx: int = 0) -> bnb.nn.modules:
+#         embedding = bnb.nn.modules.Embedding(num_tokens, dim, padding_idx)
+
+#         return embedding
 
 class TokenEmbedding(nn.Module):
     def __init__(self, dim, num_tokens, embedding_provider: BaseEmbedding, l2norm_embed = False):
         super().__init__()
         self.l2norm_embed = l2norm_embed
         self.emb = embedding_provider.get_embedding(num_tokens, dim)
-            # nn.Embedding(num_tokens, dim)
+        # nn.Embedding(num_tokens, dim)
 
     def forward(self, x):
         token_emb = self.emb(x)
         return l2norm(token_emb) if self.l2norm_embed else token_emb
 
 # positional embeddings
 
@@ -885,15 +898,15 @@
         return out, intermediates
 
 class AttentionLayers(nn.Module):
     def __init__(
         self,
         dim,
         depth,
-        heads = 8,
+        heads = None,
         causal = False,
         cross_attend = False,
         only_cross = False,
         use_scalenorm = False,
         use_rmsnorm = False,
         alibi_pos_bias = False,
         alibi_num_heads = None,
@@ -975,14 +988,15 @@
             pre_norm = sandwich_norm = resi_dual = False
             scale_residual = True
             scale_residual_constant = (2 * depth) ** 0.25
 
         assert (int(sandwich_norm) + int(resi_dual)) <= 1, 'either sandwich norm or resiDual is selected, but not both'
         assert not (not pre_norm and sandwich_norm), 'sandwich norm cannot be used when not using prenorm'
         assert not (not pre_norm and resi_dual), 'resiDualcannot be used when not using prenorm'
+
         self.pre_norm = pre_norm
         self.sandwich_norm = sandwich_norm
         self.resi_dual = resi_dual
 
         self.residual_attn = residual_attn
         self.cross_residual_attn = cross_residual_attn
         self.cross_attend = cross_attend
@@ -1078,14 +1092,16 @@
 
             self.layers.append(nn.ModuleList([
                 norms,
                 layer,
                 residual
             ]))
 
+            self.layers_length = len(self.layers) # It doesn't work if called after
+
         if deepnorm:
             init_gain = (8 * depth) ** -0.25
             deepnorm_init(self, init_gain)
 
     def forward(
         self,
         x,
@@ -1110,15 +1126,15 @@
         if exists(self.rotary_pos_emb):
             max_rotary_emb_length = max(list(map(lambda m: (m.shape[1] if exists(m) else 0) + x.shape[1], mems)))
             rotary_pos_emb = self.rotary_pos_emb(max_rotary_emb_length, x.device)
 
         outer_residual = x
 
         for ind, (layer_type, (norm, block, residual_fn), layer_dropout) in enumerate(zip(self.layer_types, self.layers, self.layer_dropouts)):
-            is_last = ind == (len(self.layers) - 1)
+            is_last = ind == (self.layers_length - 1)
 
             if self.training and layer_dropout > 0. and random() < layer_dropout:
                 continue
 
             if layer_type == 'a':
                 if return_hiddens:
                     hiddens.append(x)
@@ -1253,15 +1269,15 @@
 class TransformerWrapper(nn.Module):
     def __init__(
         self,
         *,
         num_tokens,
         max_seq_len,
         attn_layers,
-        tokenizer: BaseTokenizer,
+        # tokenizer: BaseTokenizer,
         embedding_provider: BaseEmbedding,
         emb_dim = None,
         max_mem_len = 0.,
         shift_mem_down = 0,
         emb_dropout = 0.,
         post_emb_norm = False,
         num_memory_tokens = None,
@@ -1269,34 +1285,35 @@
         logits_dim = None,
         use_abs_pos_emb = True,
         scaled_sinu_pos_emb = False,
         l2norm_embed = False,
         emb_frac_gradient = 1. # GLM-130B and Cogview successfully used this, set at 0.1
     ):
         super().__init__()
+
         assert isinstance(attn_layers, AttentionLayers), 'attention layers must be one of Encoder or Decoder'
 
         dim = attn_layers.dim
         emb_dim = default(emb_dim, dim)
 
         # your own tokenizer
-        self.tokenizer = tokenizer
+        # self.tokenizer = tokenizer
 
         #your own embedding function
         self.token_emb = TokenEmbedding(emb_dim, num_tokens, embedding_provider, l2norm_embed=l2norm_embed)
 
         self.emb_dim = emb_dim
         self.num_tokens = num_tokens
 
         self.max_seq_len = max_seq_len
         self.max_mem_len = max_mem_len
         self.shift_mem_down = shift_mem_down
 
         self.l2norm_embed = l2norm_embed
-        self.token_emb = TokenEmbedding(emb_dim, num_tokens, l2norm_embed = l2norm_embed)
+        self.token_emb = TokenEmbedding(emb_dim, num_tokens, embedding_provider, l2norm_embed=l2norm_embed)
 
         if not (use_abs_pos_emb and not attn_layers.has_pos_emb):
             self.pos_emb = always(0)
         elif scaled_sinu_pos_emb:
             self.pos_emb = ScaledSinusoidalEmbedding(emb_dim)
         else:
             self.pos_emb = AbsolutePositionalEmbedding(emb_dim, max_seq_len, l2norm_embed = l2norm_embed)
@@ -1320,16 +1337,18 @@
         self.num_memory_tokens = num_memory_tokens
         if num_memory_tokens > 0:
             self.memory_tokens = nn.Parameter(torch.randn(num_memory_tokens, dim))
 
     def init_(self):
         if self.l2norm_embed:
             nn.init.normal_(self.token_emb.emb.weight, std = 1e-5)
+
             if not isinstance(self.pos_emb, always):
                 nn.init.normal_(self.pos_emb.emb.weight, std = 1e-5)
+
             return
 
         nn.init.kaiming_normal_(self.token_emb.emb.weight)
 
     def forward(
         self,
         x,
@@ -1363,22 +1382,24 @@
 
         x = self.post_emb_norm(x)
 
         # whether to append embeds, as in PaLI, for image embeddings
 
         if exists(prepend_embeds):
             prepend_seq, prepend_dim = prepend_embeds.shape[1:]
+
             assert prepend_dim == x.shape[-1], 'prepended embeddings need to have same dimensions as text model dimensions'
 
             x = torch.cat((prepend_embeds, x), dim = -2)
 
         # whether to reduce the gradient going to the embedding, from cogview paper, corroborated by GLM-130B model
 
         if emb_frac_gradient < 1:
             assert emb_frac_gradient > 0
+
             x = x * emb_frac_gradient + x.detach() * (1 - emb_frac_gradient)
 
         # embedding dropout
 
         x = self.emb_dropout(x)
 
         x = self.project_emb(x)
```

### Comparing `optimus-prime-transformers-1.1.5/optimus_prime_transformers/xl_autoregressive_wrapper.py` & `optimus-prime-transformers-1.1.7/optimus_prime/xl_autoregressive_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from math import ceil
 
 import torch
 from torch import nn
 import torch.nn.functional as F
 
 from einops import rearrange, pack, unpack
-from optimus_prime_transformers.autoregressive_wrapper import top_p, top_k, eval_decorator
+from optimus_prime.autoregressive_wrapper import top_p, top_k, eval_decorator
 
 # helper functions
 
 def exists(val):
     return val is not None
 
 def divisible_by(numer, denom):
```

### Comparing `optimus-prime-transformers-1.1.5/optimus_prime_transformers.egg-info/PKG-INFO` & `optimus-prime-transformers-1.1.7/optimus_prime_transformers.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimus-prime-transformers
-Version: 1.1.5
+Version: 1.1.7
 Summary: optimus-prime - Pytorch
 Home-page: https://github.com/kyegomez/Optimus-Prime
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `optimus-prime-transformers-1.1.5/setup.py` & `optimus-prime-transformers-1.1.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'optimus-prime-transformers',
   packages = find_packages(exclude=['examples']),
-  version = '1.1.5',
+  version = '1.1.7',
   license='MIT',
   description = 'optimus-prime - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   url = 'https://github.com/kyegomez/Optimus-Prime',
   long_description_content_type = 'text/markdown',
   keywords = [
     'artificial intelligence',
     'attention mechanism',
     'transformers'
   ],
   install_requires=[
-    'torch>=1.6',
-    'einops>=0.6.1'
+    'torch',
+    'einops'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
```


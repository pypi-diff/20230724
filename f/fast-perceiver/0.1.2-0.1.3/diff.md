# Comparing `tmp/fast_perceiver-0.1.2.tar.gz` & `tmp/fast_perceiver-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_perceiver-0.1.2.tar", max compression
+gzip compressed data, was "fast_perceiver-0.1.3.tar", max compression
```

## Comparing `fast_perceiver-0.1.2.tar` & `fast_perceiver-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     6395 2023-07-23 22:15:29.848472 fast_perceiver-0.1.2/README.md
--rw-r--r--   0        0        0       30 2023-07-23 21:11:38.318260 fast_perceiver-0.1.2/fast_perceiver/__init__.py
--rw-r--r--   0        0        0     6721 2023-07-23 22:19:23.326326 fast_perceiver-0.1.2/fast_perceiver/modules.py
--rw-r--r--   0        0        0      385 2023-07-23 20:57:41.749091 fast_perceiver-0.1.2/fast_perceiver/utils.py
--rw-r--r--   0        0        0      772 2023-07-23 22:40:16.435030 fast_perceiver-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6960 1970-01-01 00:00:00.000000 fast_perceiver-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     6699 2023-07-24 09:03:17.279724 fast_perceiver-0.1.3/README.md
+-rw-r--r--   0        0        0       30 2023-07-23 21:11:38.318260 fast_perceiver-0.1.3/fast_perceiver/__init__.py
+-rw-r--r--   0        0        0     8365 2023-07-24 09:03:36.051596 fast_perceiver-0.1.3/fast_perceiver/modules.py
+-rw-r--r--   0        0        0      385 2023-07-23 20:57:41.749091 fast_perceiver-0.1.3/fast_perceiver/utils.py
+-rw-r--r--   0        0        0      790 2023-07-24 09:20:23.487505 fast_perceiver-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7264 1970-01-01 00:00:00.000000 fast_perceiver-0.1.3/PKG-INFO
```

### Comparing `fast_perceiver-0.1.2/README.md` & `fast_perceiver-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -28,53 +28,60 @@
 ```python
 import torch
 
 from fast_perceiver import Perceiver
 
 in_dim = 256
 out_dim = 128
+seq_len = 128
 
 latent_dim = 512
 num_latents = 512
 
 model = Perceiver(
     input_dim=in_dim,
     depth=8,
     out_dim=out_dim,
     num_latents=num_latents,
     latent_dim=latent_dim,
     cross_heads=1,
     cross_head_dim=64,
+    cross_rotary_emb_dim=0,
+    cross_attn_dropout=0.0,
     latent_heads=8,
     latent_head_dim=64,
-    cross_attn_dropout=0.0,
-    self_attn_dropout=0.0,
+    latent_rotary_emb_dim=0,
+    latent_attn_dropout=0.0,
     weight_tie_layers=False,
     gated_mlp=True,
-).cuda()
+)
+
+# Note: FlashAttention only supports half-precision
+# We need to explicitly cast the model or alternative use torch.autocast
+model.to('cuda', torch.float16)
+
+x = torch.randn(32, seq_len, in_dim, dtype=torch.float16, device='cuda')
+
+seq_lens = torch.randint(1, seq_len + 1, (32,), device=x.device)
+mask = torch.arange(seq_len, device=x.device)[None, :] < seq_lens[:, None]
 
-x = torch.randn(32, 128, in_dim).cuda()
-mask = torch.rand(32, 128) > 0.5
 
-# FlashAttention only works with half-precision
-# Don't forget to autocast!
-with torch.autocast('cuda'):
-    # `out_dim` specified; averages and projects output
-    out = model(x)
+# `out_dim` specified; averages and projects output
+out = model(x)
 
-    assert out.shape == (32, out_dim)
+assert out.shape == (32, out_dim)
 
-    # A input element-wise mask can be provided
-    # All non-True elements will be ignored
-    out = model(x, mask=mask)
+# A input element-wise mask can be provided
+# All non-True elements will be ignored
+out = model(x, mask=mask)
 
-    # The raw final latents will be returned when `return_embeddings=True`
-    embeds = model(x, return_embeddings=True)
+# The raw final latents will be returned when `return_embeddings=True`
+embeds = model(x, return_embeddings=True)
 
-    assert embeds.shape == (32, num_latents, latent_dim)
+assert embeds.shape == (32, num_latents, latent_dim)
 ```
 
 Performance
 -----------
 
 The Perceiver is already designed and intended as a attention architecture with sub-quadratic compute and memory complexity in comparison to the quadratic requirements of a vanilla Transformer.
 
@@ -114,14 +121,15 @@
 
 - [ ] Perceiver IO [2] [WIP]
 - [ ] Perceiver AR [3] (or an AR demo in general)
 - [ ] Demos [WIP]
 - [ ] Tests [WIP]
 - [ ] Allow more flexible cross-attention configurations
 - [ ] Benchmarks against other Perceiver implementations, e.g. [DeepMind's](https://github.com/deepmind/deepmind-research/tree/master/perceiver) or [Krasser's](https://github.com/krasserm/perceiver-io)
+- [ ] If FA2 is eventuelly merged into PyTorch, drop the flash-attn dependency
 
 References
 ----------
 
 [1] Jaegle, Andrew, Felix Gimeno, Andrew Brock, Andrew Zisserman, Oriol Vinyals, and Joao Carreira. “Perceiver: General Perception with Iterative Attention.” arXiv, June 22, 2021. http://arxiv.org/abs/2103.03206.
 
 [2] Jaegle, Andrew, Sebastian Borgeaud, Jean-Baptiste Alayrac, Carl Doersch, Catalin Ionescu, David Ding, Skanda Koppula, et al. “Perceiver IO: A General Architecture for Structured Inputs & Outputs.” arXiv, March 15, 2022. http://arxiv.org/abs/2107.14795.
```

### Comparing `fast_perceiver-0.1.2/fast_perceiver/modules.py` & `fast_perceiver-0.1.3/fast_perceiver/modules.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,67 @@
+from typing import Optional
 import torch
 
 from functools import partial
 from torch import nn
 
 from einops import repeat
 from einops.layers.torch import Reduce
 
-from flash_attn.bert_padding import unpad_input
-from flash_attn.modules.mha import MHA
+from flash_attn.bert_padding import pad_input, unpad_input
+from flash_attn.modules.mha import MHA, ParallelMHA
 from flash_attn.modules.block import Block
 from flash_attn.modules.mlp import Mlp, GatedMlp
 
 from fast_perceiver.utils import cache_fn
 
 
-class BetterMHA(MHA):
-    """
-    Wrapper around FA's MHA to support separate q and kv dim and more API flexibility.
-    """
-    def __init__(self, embed_dim, *args, kv_dim=None, num_heads=8, head_dim=None, **kwargs):
-        if num_heads is None:
-            assert head_dim is not None, 'Must specify either num_heads or head_dim'
-            kwargs['num_heads'] = embed_dim // head_dim
-
-        super().__init__(embed_dim, num_heads, *args, **kwargs)
-
-        self.kv_dim = kv_dim or self.embed_dim
-
-        if head_dim is not None:
-            self.head_dim = head_dim
-        
-        inner_dim = self.num_heads * self.head_dim
-        linear_cls = self.out_proj.__class__
-
-        qkv_proj_bias = kwargs.get('qkv_proj_bias', True)
-        out_proj_bias = kwargs.get('out_proj_bias', True)
-
-        if self.cross_attn:
-            self.Wq = linear_cls(self.embed_dim, inner_dim, bias=qkv_proj_bias)
-            self.Wkv = linear_cls(self.kv_dim, 2 * inner_dim, bias=qkv_proj_bias)
-        else:
-            self.Wqkv = linear_cls(self.embed_dim, 3 * inner_dim, bias=qkv_proj_bias)
+def patched_mha(base_mha_cls):
+    class PatchedMHA(base_mha_cls):
+        """
+        Wrapper around FA's MHA to support separate q and kv dim and more API flexibility.
+        """
+        def __init__(
+            self,
+            embed_dim: int,
+            *args,
+            kv_dim: Optional[int] = None,
+            num_heads: Optional[int] = 8,
+            head_dim: Optional[int] = None,
+            **kwargs
+        ):
+            if num_heads is None:
+                assert head_dim is not None, 'Must specify either num_heads or head_dim'
+                kwargs['num_heads'] = embed_dim // head_dim
+
+            super().__init__(embed_dim, num_heads, *args, **kwargs)
+
+            self.kv_dim = kv_dim or self.embed_dim
+
+            if head_dim is not None:
+                self.head_dim = head_dim
+            
+            inner_dim = self.num_heads * self.head_dim
+            linear_cls = self.out_proj.__class__
+
+            qkv_proj_bias = kwargs.get('qkv_proj_bias', True)
+            out_proj_bias = kwargs.get('out_proj_bias', True)
+
+            if self.cross_attn:
+                self.Wq = linear_cls(self.embed_dim, inner_dim, bias=qkv_proj_bias)
+                self.Wkv = linear_cls(self.kv_dim, 2 * inner_dim, bias=qkv_proj_bias)
+            else:
+                self.Wqkv = linear_cls(self.embed_dim, 3 * inner_dim, bias=qkv_proj_bias)
+
+            self.out_proj = linear_cls(inner_dim, self.embed_dim, bias=out_proj_bias)
+
+    return PatchedMHA
 
-        self.out_proj = linear_cls(inner_dim, self.embed_dim, bias=out_proj_bias)
+PatchedMHA = patched_mha(MHA)
+PatchedParallelMHA = patched_mha(ParallelMHA)
 
 
 class Perceiver(nn.Module):
     """
     Fast and memory efficient [Perceiver](https://arxiv.org/abs/2103.03206) implementation in PyTorch
     with [FlashAttention](https://arxiv.org/abs/2205.14135) as the underlying attention implementation.
 
@@ -73,46 +88,53 @@
             in those layers. Defaults to True.
         self_per_cross_attn: Number of self-attention blocks per cross-attention block.
             Defaults to 1.
     """
     def __init__(
         self,
         *,
-        input_dim,
-        depth,
-        out_dim=None,
-        num_latents=512,
-        latent_dim=512,
-        cross_heads=1,
-        cross_head_dim=64,
-        cross_rotary_emb_dim=0,
-        cross_attn_dropout=0.0,
-        latent_heads=8,
-        latent_head_dim=64,
-        latent_rotary_emb_dim=0,
-        latent_attn_dropout=0.0,
-        weight_tie_layers=False,
-        gated_mlp=True,
-        self_per_cross_attn=1,
+        input_dim: int,
+        depth: int,
+        out_dim: Optional[int] = None,
+        num_latents: int = 512,
+        latent_dim: int = 512,
+        cross_heads: int = 1,
+        cross_head_dim: int = 64,
+        cross_rotary_emb_dim: int = 0,
+        cross_attn_dropout: float = 0.0,
+        latent_heads: int =8,
+        latent_head_dim: int = 64,
+        latent_rotary_emb_dim: int = 0,
+        latent_attn_dropout: float = 0.0,
+        weight_tie_layers: bool = False,
+        gated_mlp: bool = True,
+        use_parallel_mha: bool = False,
+        self_per_cross_attn: int = 1,
     ):
         super().__init__()
 
         self.input_dim = input_dim
 
+        self.num_latents = num_latents
         self.latents = nn.Parameter(torch.randn(num_latents, latent_dim))
 
         if gated_mlp:
             mlp_cls = partial(GatedMlp, hidden_features=latent_dim * 4)
         else:
             mlp_cls = Mlp
 
+        if use_parallel_mha:
+            mha_cls = PatchedParallelMHA
+        else:
+            mha_cls = PatchedMHA
+
         get_cross_attn_block = lambda: Block(
             dim=latent_dim,
             mixer_cls=partial(
-                BetterMHA,
+                mha_cls,
                 kv_dim=input_dim,
                 num_heads=cross_heads,
                 head_dim=cross_head_dim,
                 cross_attn=True,
                 dropout=cross_attn_dropout,
                 qkv_proj_bias=False,
                 rotary_emb_dim=cross_rotary_emb_dim,
@@ -120,15 +142,15 @@
             ),
             mlp_cls=mlp_cls
         )
 
         get_self_attn_block = lambda: Block(
             dim=latent_dim,
             mixer_cls=partial(
-                BetterMHA,
+                mha_cls,
                 num_heads=latent_heads,
                 head_dim=latent_head_dim,
                 dropout=latent_attn_dropout,
                 rotary_emb_dim=latent_rotary_emb_dim,
                 use_flash_attn=True
             ),
             mlp_cls=mlp_cls
@@ -173,26 +195,42 @@
         assert dim == self.input_dim, f'Input must have {self.input_dim} dimensions, but found {dim}'
 
         x = repeat(self.latents, 'n d -> b n d', b=batch_size)
 
         cross_block_kwargs = {'x_kv': data}
 
         if mask is not None:
-            data, _, cu_seqlens, max_seqlen_in_batch = unpad_input(data, ~mask)
+            data, _, cu_seqlens_k, max_seqlen_in_batch_k = unpad_input(data, mask)
 
             cross_block_kwargs = {
                 'x_kv': data,
-                'cu_seqlens_k': cu_seqlens,
-                'max_seqlen_k': max_seqlen_in_batch
+                'cu_seqlens_k': cu_seqlens_k,
+                'max_seqlen_k': max_seqlen_in_batch_k
             }
 
-            print(data.shape)
-
         for cross_block, self_attn_blocks in self.layers:
-            x = cross_block(x, mixer_kwargs=cross_block_kwargs)[0]
+            # FlashAttention currently does not support key-value-only padding
+            # We therefore have to _unpad_ the queries (aka latents) as well.
+            # In the future, this could be used for a Perceiver AR implementation.
+            # TODO: We could compuet the dummy mask tensors for the queries directly here
+            #  without calling the unpad_input function.
+            if mask is not None:
+                x_mask = torch.ones(x.shape[:2], dtype=torch.bool, device=x.device)
+                x_cross, indices, cu_seqlens, max_seqlen_in_batch = unpad_input(x, x_mask)
+                cross_block_kwargs.update({
+                    'cu_seqlens': cu_seqlens,
+                    'max_seqlen': max_seqlen_in_batch
+                })
+            else:
+                x_cross = x
+
+            x = cross_block(x_cross, mixer_kwargs=cross_block_kwargs)[0]
+
+            if mask is not None:
+                x = pad_input(x, indices, batch_size, self.num_latents)
 
             for self_attn_block in self_attn_blocks:
                 x = self_attn_block(x)[0]
 
         if return_embeddings:
             return x
```

### Comparing `fast_perceiver-0.1.2/pyproject.toml` & `fast_perceiver-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fast-perceiver"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Kristian Klemon <kristian.klemon@gmail.com>"]
 readme = "README.md"
 packages = [{include = "fast_perceiver"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -23,11 +23,12 @@
 
 [tool.poetry.group.dev.dependencies]
 tqdm = "^4.65.0"
 pandas = "^2.0.3"
 seaborn = "^0.12.2"
 jupyter = "^1.0.0"
 perceiver-pytorch = "^0.8.7"
+pytest = "^7.4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fast_perceiver-0.1.2/PKG-INFO` & `fast_perceiver-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-perceiver
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Kristian Klemon
 Author-email: kristian.klemon@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -45,53 +45,60 @@
 ```python
 import torch
 
 from fast_perceiver import Perceiver
 
 in_dim = 256
 out_dim = 128
+seq_len = 128
 
 latent_dim = 512
 num_latents = 512
 
 model = Perceiver(
     input_dim=in_dim,
     depth=8,
     out_dim=out_dim,
     num_latents=num_latents,
     latent_dim=latent_dim,
     cross_heads=1,
     cross_head_dim=64,
+    cross_rotary_emb_dim=0,
+    cross_attn_dropout=0.0,
     latent_heads=8,
     latent_head_dim=64,
-    cross_attn_dropout=0.0,
-    self_attn_dropout=0.0,
+    latent_rotary_emb_dim=0,
+    latent_attn_dropout=0.0,
     weight_tie_layers=False,
     gated_mlp=True,
-).cuda()
+)
+
+# Note: FlashAttention only supports half-precision
+# We need to explicitly cast the model or alternative use torch.autocast
+model.to('cuda', torch.float16)
+
+x = torch.randn(32, seq_len, in_dim, dtype=torch.float16, device='cuda')
+
+seq_lens = torch.randint(1, seq_len + 1, (32,), device=x.device)
+mask = torch.arange(seq_len, device=x.device)[None, :] < seq_lens[:, None]
 
-x = torch.randn(32, 128, in_dim).cuda()
-mask = torch.rand(32, 128) > 0.5
 
-# FlashAttention only works with half-precision
-# Don't forget to autocast!
-with torch.autocast('cuda'):
-    # `out_dim` specified; averages and projects output
-    out = model(x)
+# `out_dim` specified; averages and projects output
+out = model(x)
 
-    assert out.shape == (32, out_dim)
+assert out.shape == (32, out_dim)
 
-    # A input element-wise mask can be provided
-    # All non-True elements will be ignored
-    out = model(x, mask=mask)
+# A input element-wise mask can be provided
+# All non-True elements will be ignored
+out = model(x, mask=mask)
 
-    # The raw final latents will be returned when `return_embeddings=True`
-    embeds = model(x, return_embeddings=True)
+# The raw final latents will be returned when `return_embeddings=True`
+embeds = model(x, return_embeddings=True)
 
-    assert embeds.shape == (32, num_latents, latent_dim)
+assert embeds.shape == (32, num_latents, latent_dim)
 ```
 
 Performance
 -----------
 
 The Perceiver is already designed and intended as a attention architecture with sub-quadratic compute and memory complexity in comparison to the quadratic requirements of a vanilla Transformer.
 
@@ -131,14 +138,15 @@
 
 - [ ] Perceiver IO [2] [WIP]
 - [ ] Perceiver AR [3] (or an AR demo in general)
 - [ ] Demos [WIP]
 - [ ] Tests [WIP]
 - [ ] Allow more flexible cross-attention configurations
 - [ ] Benchmarks against other Perceiver implementations, e.g. [DeepMind's](https://github.com/deepmind/deepmind-research/tree/master/perceiver) or [Krasser's](https://github.com/krasserm/perceiver-io)
+- [ ] If FA2 is eventuelly merged into PyTorch, drop the flash-attn dependency
 
 References
 ----------
 
 [1] Jaegle, Andrew, Felix Gimeno, Andrew Brock, Andrew Zisserman, Oriol Vinyals, and Joao Carreira. “Perceiver: General Perception with Iterative Attention.” arXiv, June 22, 2021. http://arxiv.org/abs/2103.03206.
 
 [2] Jaegle, Andrew, Sebastian Borgeaud, Jean-Baptiste Alayrac, Carl Doersch, Catalin Ionescu, David Ding, Skanda Koppula, et al. “Perceiver IO: A General Architecture for Structured Inputs & Outputs.” arXiv, March 15, 2022. http://arxiv.org/abs/2107.14795.
```


# Comparing `tmp/unitorch-0.0.0.5.tar.gz` & `tmp/unitorch-0.0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitorch-0.0.0.5.tar", last modified: Fri Jul 14 20:43:03 2023, max compression
+gzip compressed data, was "unitorch-0.0.0.6.tar", last modified: Mon Jul 24 07:53:46 2023, max compression
```

## Comparing `unitorch-0.0.0.5.tar` & `unitorch-0.0.0.6.tar`

### file list

```diff
@@ -1,491 +1,490 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.757856 unitorch-0.0.0.5/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.549856 unitorch-0.0.0.5/.pytest_cache/
--rw-r--r--   0 root         (0) root         (0)      302 2023-07-14 20:42:54.000000 unitorch-0.0.0.5/.pytest_cache/README.md
--rw-r--r--   0 root         (0) root         (0)     1085 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      131 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9246 2023-07-14 20:43:03.757856 unitorch-0.0.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8187 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.549856 unitorch-0.0.0.5/benchmarks/
--rw-r--r--   0 root         (0) root         (0)       87 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/benchmarks/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.525856 unitorch-0.0.0.5/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.549856 unitorch-0.0.0.5/docs/search/
--rw-r--r--   0 root         (0) root         (0)  1081944 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/docs/search/search_index.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.553856 unitorch-0.0.0.5/examples/
--rw-r--r--   0 root         (0) root         (0)     2311 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.529856 unitorch-0.0.0.5/examples/configs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.557856 unitorch-0.0.0.5/examples/configs/caption/
--rw-r--r--   0 root         (0) root         (0)     1788 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/caption/blip.ini
--rw-r--r--   0 root         (0) root         (0)     2556 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/caption/minigpt4.ini
--rw-r--r--   0 root         (0) root         (0)     2692 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/caption/minigpt4_ds.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.561856 unitorch-0.0.0.5/examples/configs/classification/
--rw-r--r--   0 root         (0) root         (0)     1545 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/classification/bert.ini
--rw-r--r--   0 root         (0) root         (0)     1700 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/classification/clip.ini
--rw-r--r--   0 root         (0) root         (0)     1688 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/classification/image_clip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.561856 unitorch-0.0.0.5/examples/configs/classification/lora/
--rw-r--r--   0 root         (0) root         (0)     1639 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/classification/lora/bloom.ini
--rw-r--r--   0 root         (0) root         (0)     1615 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/classification/lora/bloom_ds.ini
--rw-r--r--   0 root         (0) root         (0)     1857 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/classification/lora/llama.ini
--rw-r--r--   0 root         (0) root         (0)     1810 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/classification/lora/llama_ds.ini
--rw-r--r--   0 root         (0) root         (0)     1556 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/classification/roberta.ini
--rw-r--r--   0 root         (0) root         (0)     1673 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/classification/swin.ini
--rw-r--r--   0 root         (0) root         (0)     1636 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/classification/text_clip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.561856 unitorch-0.0.0.5/examples/configs/deepspeed/
--rw-r--r--   0 root         (0) root         (0)      500 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/deepspeed/adamw.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.565856 unitorch-0.0.0.5/examples/configs/diffusion/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.565856 unitorch-0.0.0.5/examples/configs/diffusion/controlnet/
--rw-r--r--   0 root         (0) root         (0)     1925 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/diffusion/controlnet/canny.ini
--rw-r--r--   0 root         (0) root         (0)     1751 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/diffusion/stable-v1.5.ini
--rw-r--r--   0 root         (0) root         (0)     1751 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/diffusion/stable-v2.1.ini
--rw-r--r--   0 root         (0) root         (0)     1747 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/diffusion/stable-v2.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.569856 unitorch-0.0.0.5/examples/configs/generation/
--rw-r--r--   0 root         (0) root         (0)     1607 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/bart.ini
--rw-r--r--   0 root         (0) root         (0)     1651 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/bloom.ini
--rw-r--r--   0 root         (0) root         (0)     1667 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/chatglm.ini
--rw-r--r--   0 root         (0) root         (0)     1647 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/llama.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.577856 unitorch-0.0.0.5/examples/configs/generation/lora/
--rw-r--r--   0 root         (0) root         (0)     1608 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/lora/bloom.ini
--rw-r--r--   0 root         (0) root         (0)     1582 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/lora/bloom_ds.ini
--rw-r--r--   0 root         (0) root         (0)     1604 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/lora/llama.ini
--rw-r--r--   0 root         (0) root         (0)     1578 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/lora/llama_ds.ini
--rw-r--r--   0 root         (0) root         (0)     1659 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/mbart.ini
--rw-r--r--   0 root         (0) root         (0)     1597 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/mt5.ini
--rw-r--r--   0 root         (0) root         (0)     1655 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/pegasus.ini
--rw-r--r--   0 root         (0) root         (0)     1587 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/t5.ini
--rw-r--r--   0 root         (0) root         (0)     1647 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/xpegasus.ini
--rw-r--r--   0 root         (0) root         (0)     1745 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/generation/xprophetnet.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.577856 unitorch-0.0.0.5/examples/configs/pretrain/
--rw-r--r--   0 root         (0) root         (0)     1266 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/pretrain/clip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.529856 unitorch-0.0.0.5/examples/configs/services/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.577856 unitorch-0.0.0.5/examples/configs/services/zip_image/
--rw-r--r--   0 root         (0) root         (0)      148 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/services/zip_image/config.ini
--rw-r--r--   0 root         (0) root         (0)      240 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/configs/services/zip_image/config_v2.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.529856 unitorch-0.0.0.5/examples/hub/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.577856 unitorch-0.0.0.5/examples/hub/caption/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/hub/caption/blip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.577856 unitorch-0.0.0.5/examples/hub/classification/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/hub/classification/bert.ini
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/hub/classification/clip.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.581856 unitorch-0.0.0.5/examples/hub/generation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/hub/generation/bart.ini
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/hub/generation/llama.ini
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/examples/hub/generation/xpegasus.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.581856 unitorch-0.0.0.5/notebooks/
--rw-r--r--   0 root         (0) root         (0)      131 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/notebooks/README.md
--rw-r--r--   0 root         (0) root         (0)     1879 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      131 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 20:43:03.757856 unitorch-0.0.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1527 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.529856 unitorch-0.0.0.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.581856 unitorch-0.0.0.5/src/unitorch/
--rw-r--r--   0 root         (0) root         (0)     2670 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.581856 unitorch-0.0.0.5/src/unitorch/cli/
--rw-r--r--   0 root         (0) root         (0)     6024 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.585856 unitorch-0.0.0.5/src/unitorch/cli/console/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/console/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2092 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/console/eval.py
--rw-r--r--   0 root         (0) root         (0)      358 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/console/fastapi.py
--rw-r--r--   0 root         (0) root         (0)     2072 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/console/infer.py
--rw-r--r--   0 root         (0) root         (0)     2151 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/console/script.py
--rw-r--r--   0 root         (0) root         (0)     4683 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/console/service.py
--rw-r--r--   0 root         (0) root         (0)     2095 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/console/train.py
--rw-r--r--   0 root         (0) root         (0)     4397 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.585856 unitorch-0.0.0.5/src/unitorch/cli/datasets/
--rw-r--r--   0 root         (0) root         (0)       98 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12406 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/datasets/hf.py
--rw-r--r--   0 root         (0) root         (0)     2613 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.589856 unitorch-0.0.0.5/src/unitorch/cli/loss/
--rw-r--r--   0 root         (0) root         (0)     4063 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2857 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/loss/ranking.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.593856 unitorch-0.0.0.5/src/unitorch/cli/models/
--rw-r--r--   0 root         (0) root         (0)     2901 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.597856 unitorch-0.0.0.5/src/unitorch/cli/models/bart/
--rw-r--r--   0 root         (0) root         (0)     1378 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/bart/__init__.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/bart/fastapi.py
--rw-r--r--   0 root         (0) root         (0)     7012 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/bart/modeling.py
--rw-r--r--   0 root         (0) root         (0)     6140 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/bart/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.597856 unitorch-0.0.0.5/src/unitorch/cli/models/beit/
--rw-r--r--   0 root         (0) root         (0)     1390 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/beit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3142 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/beit/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2535 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/beit/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.597856 unitorch-0.0.0.5/src/unitorch/cli/models/bert/
--rw-r--r--   0 root         (0) root         (0)     1177 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/bert/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3903 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/bert/modeling.py
--rw-r--r--   0 root         (0) root         (0)     6128 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/bert/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.601856 unitorch-0.0.0.5/src/unitorch/cli/models/blip/
--rw-r--r--   0 root         (0) root         (0)     2196 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/blip/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22734 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/blip/modeling.py
--rw-r--r--   0 root         (0) root         (0)     7788 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/blip/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.601856 unitorch-0.0.0.5/src/unitorch/cli/models/bloom/
--rw-r--r--   0 root         (0) root         (0)     2570 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/bloom/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13074 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/bloom/modeling.py
--rw-r--r--   0 root         (0) root         (0)     8321 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/bloom/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.605856 unitorch-0.0.0.5/src/unitorch/cli/models/chatglm/
--rw-r--r--   0 root         (0) root         (0)     1201 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/chatglm/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13812 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/chatglm/modeling.py
--rw-r--r--   0 root         (0) root         (0)     8833 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/chatglm/processing.py
--rw-r--r--   0 root         (0) root         (0)     9143 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/classification_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.605856 unitorch-0.0.0.5/src/unitorch/cli/models/clip/
--rw-r--r--   0 root         (0) root         (0)     2514 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/clip/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16125 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/clip/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5565 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/clip/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.609856 unitorch-0.0.0.5/src/unitorch/cli/models/deberta/
--rw-r--r--   0 root         (0) root         (0)     4492 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/deberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4077 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/deberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     4021 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/deberta/modeling_v2.py
--rw-r--r--   0 root         (0) root         (0)     3801 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/deberta/processing.py
--rw-r--r--   0 root         (0) root         (0)     3434 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/deberta/processing_v2.py
--rw-r--r--   0 root         (0) root         (0)     2545 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/detection_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.609856 unitorch-0.0.0.5/src/unitorch/cli/models/diffusers/
--rw-r--r--   0 root         (0) root         (0)     2453 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/diffusers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7500 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/diffusers/modeling_controlnet.py
--rw-r--r--   0 root         (0) root         (0)     9444 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/diffusers/modeling_stable.py
--rw-r--r--   0 root         (0) root         (0)     3879 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/diffusers/processing_controlnet.py
--rw-r--r--   0 root         (0) root         (0)     3838 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/diffusers/processing_stable.py
--rw-r--r--   0 root         (0) root         (0)     3126 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/diffusion_utils.py
--rw-r--r--   0 root         (0) root         (0)     2961 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/generation_utils.py
--rw-r--r--   0 root         (0) root         (0)     5092 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/image_utils.py
--rw-r--r--   0 root         (0) root         (0)     4297 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/label_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.613856 unitorch-0.0.0.5/src/unitorch/cli/models/llama/
--rw-r--r--   0 root         (0) root         (0)     3445 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/llama/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14065 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/llama/modeling.py
--rw-r--r--   0 root         (0) root         (0)     8206 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/llama/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.613856 unitorch-0.0.0.5/src/unitorch/cli/models/mbart/
--rw-r--r--   0 root         (0) root         (0)      887 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/mbart/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7650 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/mbart/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5826 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/mbart/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.617856 unitorch-0.0.0.5/src/unitorch/cli/models/minigpt4/
--rw-r--r--   0 root         (0) root         (0)     2870 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/minigpt4/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10738 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/minigpt4/modeling.py
--rw-r--r--   0 root         (0) root         (0)    10044 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/minigpt4/processing.py
--rw-r--r--   0 root         (0) root         (0)    15281 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/modeling_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.617856 unitorch-0.0.0.5/src/unitorch/cli/models/mt5/
--rw-r--r--   0 root         (0) root         (0)     1381 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/mt5/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7173 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/mt5/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5815 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/mt5/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.617856 unitorch-0.0.0.5/src/unitorch/cli/models/peft/
--rw-r--r--   0 root         (0) root         (0)      524 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/peft/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30598 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/peft/modeling_bloom.py
--rw-r--r--   0 root         (0) root         (0)    30656 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/peft/modeling_llama.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.621856 unitorch-0.0.0.5/src/unitorch/cli/models/pegasus/
--rw-r--r--   0 root         (0) root         (0)     1213 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/pegasus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7281 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/pegasus/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5885 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/pegasus/processing.py
--rw-r--r--   0 root         (0) root         (0)     2834 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/processing_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.621856 unitorch-0.0.0.5/src/unitorch/cli/models/prophetnet/
--rw-r--r--   0 root         (0) root         (0)      162 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/prophetnet/__init__.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/prophetnet/modeling.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/prophetnet/processing.py
--rw-r--r--   0 root         (0) root         (0)      650 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/random_utils.py
--rw-r--r--   0 root         (0) root         (0)      535 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/ranking_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.625856 unitorch-0.0.0.5/src/unitorch/cli/models/roberta/
--rw-r--r--   0 root         (0) root         (0)     1347 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/roberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3967 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/roberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     3766 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/roberta/processing.py
--rw-r--r--   0 root         (0) root         (0)     2462 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/segmentation_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.625856 unitorch-0.0.0.5/src/unitorch/cli/models/swin/
--rw-r--r--   0 root         (0) root         (0)     3032 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/swin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3225 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/swin/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2564 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/swin/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.625856 unitorch-0.0.0.5/src/unitorch/cli/models/t5/
--rw-r--r--   0 root         (0) root         (0)     1282 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/t5/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7192 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/t5/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5811 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/t5/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.629856 unitorch-0.0.0.5/src/unitorch/cli/models/visualbert/
--rw-r--r--   0 root         (0) root         (0)     1310 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/visualbert/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8538 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/visualbert/modeling.py
--rw-r--r--   0 root         (0) root         (0)     6306 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/visualbert/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.629856 unitorch-0.0.0.5/src/unitorch/cli/models/vit/
--rw-r--r--   0 root         (0) root         (0)     4602 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/vit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3191 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/vit/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2583 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/vit/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.633856 unitorch-0.0.0.5/src/unitorch/cli/models/xlm_roberta/
--rw-r--r--   0 root         (0) root         (0)     2314 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/xlm_roberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7533 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/xlm_roberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     3408 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/xlm_roberta/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.633856 unitorch-0.0.0.5/src/unitorch/cli/models/xpegasus/
--rw-r--r--   0 root         (0) root         (0)     1189 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/xpegasus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7286 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/xpegasus/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5953 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/xpegasus/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.633856 unitorch-0.0.0.5/src/unitorch/cli/models/xprophetnet/
--rw-r--r--   0 root         (0) root         (0)     1034 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/xprophetnet/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7842 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/xprophetnet/modeling.py
--rw-r--r--   0 root         (0) root         (0)     5952 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/models/xprophetnet/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.637856 unitorch-0.0.0.5/src/unitorch/cli/optim/
--rw-r--r--   0 root         (0) root         (0)     1628 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/optim/__init__.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/optim/lion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.637856 unitorch-0.0.0.5/src/unitorch/cli/rl/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/rl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.637856 unitorch-0.0.0.5/src/unitorch/cli/scheduler/
--rw-r--r--   0 root         (0) root         (0)      141 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3084 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/scheduler/warmup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.637856 unitorch-0.0.0.5/src/unitorch/cli/score/
--rw-r--r--   0 root         (0) root         (0)    14139 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/score/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.641856 unitorch-0.0.0.5/src/unitorch/cli/scripts/
--rw-r--r--   0 root         (0) root         (0)      158 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/scripts/README.md
--rw-r--r--   0 root         (0) root         (0)      213 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/scripts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.641856 unitorch-0.0.0.5/src/unitorch/cli/services/
--rw-r--r--   0 root         (0) root         (0)      257 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)      223 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/services/readme.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.645856 unitorch-0.0.0.5/src/unitorch/cli/services/zip_image/
--rw-r--r--   0 root         (0) root         (0)      113 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/services/zip_image/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4866 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/services/zip_image/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.645856 unitorch-0.0.0.5/src/unitorch/cli/tasks/
--rw-r--r--   0 root         (0) root         (0)      457 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26512 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/tasks/deepspeed.py
--rw-r--r--   0 root         (0) root         (0)    31622 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/tasks/supervised.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.645856 unitorch-0.0.0.5/src/unitorch/cli/utils/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.645856 unitorch-0.0.0.5/src/unitorch/cli/writer/
--rw-r--r--   0 root         (0) root         (0)    10544 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/cli/writer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.649856 unitorch-0.0.0.5/src/unitorch/datasets/
--rw-r--r--   0 root         (0) root         (0)      130 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6832 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/datasets/hf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.649856 unitorch-0.0.0.5/src/unitorch/loss/
--rw-r--r--   0 root         (0) root         (0)     4712 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1559 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/loss/prophetnet.py
--rw-r--r--   0 root         (0) root         (0)     8411 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/loss/ranking.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.653856 unitorch-0.0.0.5/src/unitorch/models/
--rw-r--r--   0 root         (0) root         (0)     7498 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.653856 unitorch-0.0.0.5/src/unitorch/models/bart/
--rw-r--r--   0 root         (0) root         (0)      204 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/bart/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13719 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/bart/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1996 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/bart/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.657856 unitorch-0.0.0.5/src/unitorch/models/beit/
--rw-r--r--   0 root         (0) root         (0)      202 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/beit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1540 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/beit/modeling.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/beit/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.657856 unitorch-0.0.0.5/src/unitorch/models/bert/
--rw-r--r--   0 root         (0) root         (0)      208 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/bert/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2446 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/bert/modeling.py
--rw-r--r--   0 root         (0) root         (0)     8355 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/bert/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.661856 unitorch-0.0.0.5/src/unitorch/models/blip/
--rw-r--r--   0 root         (0) root         (0)      306 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/blip/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30337 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/blip/modeling.py
--rw-r--r--   0 root         (0) root         (0)     7704 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/blip/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.661856 unitorch-0.0.0.5/src/unitorch/models/blip2/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/blip2/__init__.py
--rw-r--r--   0 root         (0) root         (0)      606 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/blip2/modeling.py
--rw-r--r--   0 root         (0) root         (0)      663 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/blip2/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.665856 unitorch-0.0.0.5/src/unitorch/models/bloom/
--rw-r--r--   0 root         (0) root         (0)      247 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/bloom/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10885 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/bloom/modeling.py
--rw-r--r--   0 root         (0) root         (0)     9108 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/bloom/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.669856 unitorch-0.0.0.5/src/unitorch/models/chatglm/
--rw-r--r--   0 root         (0) root         (0)      259 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/chatglm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4201 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/chatglm/configuration_chatglm.py
--rw-r--r--   0 root         (0) root         (0)    11175 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/chatglm/modeling.py
--rw-r--r--   0 root         (0) root         (0)    55823 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/chatglm/modeling_chatglm.py
--rw-r--r--   0 root         (0) root         (0)    11091 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/chatglm/processing.py
--rw-r--r--   0 root         (0) root         (0)    15625 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/chatglm/quantization.py
--rw-r--r--   0 root         (0) root         (0)    16827 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/chatglm/tokenization_chatglm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.673856 unitorch-0.0.0.5/src/unitorch/models/clip/
--rw-r--r--   0 root         (0) root         (0)      281 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/clip/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15100 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/clip/modeling.py
--rw-r--r--   0 root         (0) root         (0)     4393 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/clip/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.673856 unitorch-0.0.0.5/src/unitorch/models/deberta/
--rw-r--r--   0 root         (0) root         (0)      424 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/deberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4503 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/deberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2568 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/deberta/modeling_v2.py
--rw-r--r--   0 root         (0) root         (0)     1744 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/deberta/processing.py
--rw-r--r--   0 root         (0) root         (0)     1603 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/deberta/processing_v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.677856 unitorch-0.0.0.5/src/unitorch/models/diffusers/
--rw-r--r--   0 root         (0) root         (0)      547 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/diffusers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6076 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/diffusers/modeling_controlnet.py
--rw-r--r--   0 root         (0) root         (0)     8201 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/diffusers/modeling_stable.py
--rw-r--r--   0 root         (0) root         (0)     3313 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/diffusers/processing_controlnet.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/diffusers/processing_stable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.677856 unitorch-0.0.0.5/src/unitorch/models/llama/
--rw-r--r--   0 root         (0) root         (0)      247 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/llama/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11394 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/llama/modeling.py
--rw-r--r--   0 root         (0) root         (0)     8944 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/llama/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.681856 unitorch-0.0.0.5/src/unitorch/models/mbart/
--rw-r--r--   0 root         (0) root         (0)      188 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/mbart/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13976 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/mbart/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2163 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/mbart/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.681856 unitorch-0.0.0.5/src/unitorch/models/minigpt4/
--rw-r--r--   0 root         (0) root         (0)      258 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/minigpt4/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16994 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/minigpt4/modeling.py
--rw-r--r--   0 root         (0) root         (0)    13727 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/minigpt4/processing.py
--rw-r--r--   0 root         (0) root         (0)     2140 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/modeling_ema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.681856 unitorch-0.0.0.5/src/unitorch/models/mt5/
--rw-r--r--   0 root         (0) root         (0)      180 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/mt5/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14250 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/mt5/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2272 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/mt5/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.685856 unitorch-0.0.0.5/src/unitorch/models/peft/
--rw-r--r--   0 root         (0) root         (0)     5424 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/peft/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9934 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/peft/modeling_bloom_adalora.py
--rw-r--r--   0 root         (0) root         (0)     9530 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/peft/modeling_bloom_lora.py
--rw-r--r--   0 root         (0) root         (0)    10125 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/peft/modeling_llama_adalora.py
--rw-r--r--   0 root         (0) root         (0)     9309 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/peft/modeling_llama_lora.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/peft/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.689856 unitorch-0.0.0.5/src/unitorch/models/pegasus/
--rw-r--r--   0 root         (0) root         (0)      196 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/pegasus/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13652 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/pegasus/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2307 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/pegasus/processing.py
--rw-r--r--   0 root         (0) root         (0)    13125 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/processing_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.689856 unitorch-0.0.0.5/src/unitorch/models/prophetnet/
--rw-r--r--   0 root         (0) root         (0)      179 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/prophetnet/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7435 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/prophetnet/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2095 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/prophetnet/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.693856 unitorch-0.0.0.5/src/unitorch/models/roberta/
--rw-r--r--   0 root         (0) root         (0)      218 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/roberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4281 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/roberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1992 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/roberta/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.693856 unitorch-0.0.0.5/src/unitorch/models/swin/
--rw-r--r--   0 root         (0) root         (0)      193 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/swin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1534 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/swin/modeling.py
--rw-r--r--   0 root         (0) root         (0)      998 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/swin/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.693856 unitorch-0.0.0.5/src/unitorch/models/t5/
--rw-r--r--   0 root         (0) root         (0)      194 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/t5/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13316 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/t5/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1924 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/t5/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.697856 unitorch-0.0.0.5/src/unitorch/models/visualbert/
--rw-r--r--   0 root         (0) root         (0)      248 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/visualbert/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6710 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/visualbert/modeling.py
--rw-r--r--   0 root         (0) root         (0)     2132 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/visualbert/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.697856 unitorch-0.0.0.5/src/unitorch/models/vit/
--rw-r--r--   0 root         (0) root         (0)      189 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/vit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1571 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/vit/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/vit/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.701856 unitorch-0.0.0.5/src/unitorch/models/xlm_roberta/
--rw-r--r--   0 root         (0) root         (0)      323 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/xlm_roberta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7381 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/xlm_roberta/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1576 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/xlm_roberta/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.701856 unitorch-0.0.0.5/src/unitorch/models/xpegasus/
--rw-r--r--   0 root         (0) root         (0)      237 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/xpegasus/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13741 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/xpegasus/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1464 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/xpegasus/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.701856 unitorch-0.0.0.5/src/unitorch/models/xprophetnet/
--rw-r--r--   0 root         (0) root         (0)      212 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/xprophetnet/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13545 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/xprophetnet/modeling.py
--rw-r--r--   0 root         (0) root         (0)     1335 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/models/xprophetnet/processing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.705856 unitorch-0.0.0.5/src/unitorch/modules/
--rw-r--r--   0 root         (0) root         (0)      133 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2453 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/modules/classifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.705856 unitorch-0.0.0.5/src/unitorch/modules/replace/
--rw-r--r--   0 root         (0) root         (0)      199 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/modules/replace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14643 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/modules/replace/beam_search_v2.py
--rw-r--r--   0 root         (0) root         (0)     2092 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/modules/replace/datasets_v2.py
--rw-r--r--   0 root         (0) root         (0)     4158 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/modules/replace/hf_hub_v2.py
--rw-r--r--   0 root         (0) root         (0)     2053 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/modules/timm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.709856 unitorch-0.0.0.5/src/unitorch/ops/
--rw-r--r--   0 root         (0) root         (0)      105 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/ops/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16794 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/ops/dyhead.py
--rw-r--r--   0 root         (0) root         (0)     1347 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/ops/ngram_repeat_block.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.709856 unitorch-0.0.0.5/src/unitorch/optim/
--rw-r--r--   0 root         (0) root         (0)      203 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/optim/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3201 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/optim/lion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.709856 unitorch-0.0.0.5/src/unitorch/rl/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/rl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.709856 unitorch-0.0.0.5/src/unitorch/rl/utils/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/rl/utils/buffer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.709856 unitorch-0.0.0.5/src/unitorch/scheduler/
--rw-r--r--   0 root         (0) root         (0)      149 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/scheduler/warmup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.713856 unitorch-0.0.0.5/src/unitorch/score/
--rw-r--r--   0 root         (0) root         (0)     1892 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/score/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4297 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/score/bleu.py
--rw-r--r--   0 root         (0) root         (0)     7852 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/score/map.py
--rw-r--r--   0 root         (0) root         (0)    13291 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/score/rouge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.713856 unitorch-0.0.0.5/src/unitorch/tasks/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.717856 unitorch-0.0.0.5/src/unitorch/utils/
--rw-r--r--   0 root         (0) root         (0)    13662 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2236 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/utils/decorators.py
--rw-r--r--   0 root         (0) root         (0)     2597 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/utils/functional.py
--rw-r--r--   0 root         (0) root         (0)     1240 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/utils/image_utils.py
--rw-r--r--   0 root         (0) root         (0)     2711 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/utils/import_utils.py
--rw-r--r--   0 root         (0) root         (0)     2639 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/utils/io.py
--rw-r--r--   0 root         (0) root         (0)     5027 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/utils/palette.py
--rw-r--r--   0 root         (0) root         (0)     3851 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/src/unitorch/utils/torch_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.581856 unitorch-0.0.0.5/src/unitorch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9246 2023-07-14 20:43:03.000000 unitorch-0.0.0.5/src/unitorch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13660 2023-07-14 20:43:03.000000 unitorch-0.0.0.5/src/unitorch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 20:43:03.000000 unitorch-0.0.0.5/src/unitorch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      344 2023-07-14 20:43:03.000000 unitorch-0.0.0.5/src/unitorch.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      383 2023-07-14 20:43:03.000000 unitorch-0.0.0.5/src/unitorch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-14 20:43:03.000000 unitorch-0.0.0.5/src/unitorch.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.721855 unitorch-0.0.0.5/wiki/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.721855 unitorch-0.0.0.5/wiki/benchmarks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/benchmarks/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.725856 unitorch-0.0.0.5/wiki/cli/
--rw-r--r--   0 root         (0) root         (0)      504 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/ast.md
--rw-r--r--   0 root         (0) root         (0)      173 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/csv.md
--rw-r--r--   0 root         (0) root         (0)      414 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/datatypes.md
--rw-r--r--   0 root         (0) root         (0)      197 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/deepspeed.md
--rw-r--r--   0 root         (0) root         (0)      181 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/jsonl.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.737856 unitorch-0.0.0.5/wiki/cli/models/
--rw-r--r--   0 root         (0) root         (0)      348 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/bart.md
--rw-r--r--   0 root         (0) root         (0)      379 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/beit.md
--rw-r--r--   0 root         (0) root         (0)      364 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/bert.md
--rw-r--r--   0 root         (0) root         (0)     1113 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/blip.md
--rw-r--r--   0 root         (0) root         (0)      719 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/bloom.md
--rw-r--r--   0 root         (0) root         (0)      761 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/chatglm.md
--rw-r--r--   0 root         (0) root         (0)      939 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/clip.md
--rw-r--r--   0 root         (0) root         (0)      783 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/deberta.md
--rw-r--r--   0 root         (0) root         (0)      353 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/diffusers.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/index.md
--rw-r--r--   0 root         (0) root         (0)      719 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/llama.md
--rw-r--r--   0 root         (0) root         (0)      359 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/mbart.md
--rw-r--r--   0 root         (0) root         (0)      227 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/minigpt4.md
--rw-r--r--   0 root         (0) root         (0)      337 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/mt5.md
--rw-r--r--   0 root         (0) root         (0)     1712 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/peft.md
--rw-r--r--   0 root         (0) root         (0)      381 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/pegasus.md
--rw-r--r--   0 root         (0) root         (0)       36 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/prophetnet.md
--rw-r--r--   0 root         (0) root         (0)      398 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/roberta.md
--rw-r--r--   0 root         (0) root         (0)      379 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/swin.md
--rw-r--r--   0 root         (0) root         (0)      326 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/t5.md
--rw-r--r--   0 root         (0) root         (0)      623 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/visualbert.md
--rw-r--r--   0 root         (0) root         (0)      368 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/vit.md
--rw-r--r--   0 root         (0) root         (0)      664 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/xlm_roberta.md
--rw-r--r--   0 root         (0) root         (0)      392 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/xpegasus.md
--rw-r--r--   0 root         (0) root         (0)      425 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/models/xprophetnet.md
--rw-r--r--   0 root         (0) root         (0)      189 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/parquet.md
--rw-r--r--   0 root         (0) root         (0)      851 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/postprocess.md
--rw-r--r--   0 root         (0) root         (0)      146 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/preprocess.md
--rw-r--r--   0 root         (0) root         (0)      192 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/cli/supervised.md
--rw-r--r--   0 root         (0) root         (0)     4600 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/configuration.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.545856 unitorch-0.0.0.5/wiki/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.737856 unitorch-0.0.0.5/wiki/examples/caption/
--rw-r--r--   0 root         (0) root         (0)     4659 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/examples/caption/blip.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.741855 unitorch-0.0.0.5/wiki/examples/classification/
--rw-r--r--   0 root         (0) root         (0)     4208 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/examples/classification/clip.md
--rw-r--r--   0 root         (0) root         (0)     4130 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/examples/classification/roberta.md
--rw-r--r--   0 root         (0) root         (0)     4525 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/examples/classification/swin.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.741855 unitorch-0.0.0.5/wiki/examples/diffusion/
--rw-r--r--   0 root         (0) root         (0)       32 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/examples/diffusion/controlnet.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.741855 unitorch-0.0.0.5/wiki/examples/generation/
--rw-r--r--   0 root         (0) root         (0)     4145 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/examples/generation/bart.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.741855 unitorch-0.0.0.5/wiki/examples/service/
--rw-r--r--   0 root         (0) root         (0)     1602 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/examples/service/zip_image.md
--rw-r--r--   0 root         (0) root         (0)     1346 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/index.md
--rw-r--r--   0 root         (0) root         (0)      890 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/installation.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.741855 unitorch-0.0.0.5/wiki/labs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/labs/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 20:43:03.753856 unitorch-0.0.0.5/wiki/models/
--rw-r--r--   0 root         (0) root         (0)      147 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/bart.md
--rw-r--r--   0 root         (0) root         (0)      165 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/beit.md
--rw-r--r--   0 root         (0) root         (0)      155 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/bert.md
--rw-r--r--   0 root         (0) root         (0)      453 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/blip.md
--rw-r--r--   0 root         (0) root         (0)      296 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/bloom.md
--rw-r--r--   0 root         (0) root         (0)      322 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/chatglm.md
--rw-r--r--   0 root         (0) root         (0)      383 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/clip.md
--rw-r--r--   0 root         (0) root         (0)      402 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/deberta.md
--rw-r--r--   0 root         (0) root         (0)      152 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/diffusers.md
--rw-r--r--   0 root         (0) root         (0)      450 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/index.md
--rw-r--r--   0 root         (0) root         (0)      296 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/llama.md
--rw-r--r--   0 root         (0) root         (0)      154 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/mbart.md
--rw-r--r--   0 root         (0) root         (0)      297 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/minigpt4.md
--rw-r--r--   0 root         (0) root         (0)      140 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/mt5.md
--rw-r--r--   0 root         (0) root         (0)      695 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/peft.md
--rw-r--r--   0 root         (0) root         (0)      168 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/pegasus.md
--rw-r--r--   0 root         (0) root         (0)      107 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/prophetnet.md
--rw-r--r--   0 root         (0) root         (0)      243 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/roberta.md
--rw-r--r--   0 root         (0) root         (0)      165 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/swin.md
--rw-r--r--   0 root         (0) root         (0)      133 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/t5.md
--rw-r--r--   0 root         (0) root         (0)      277 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/visualbert.md
--rw-r--r--   0 root         (0) root         (0)      158 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/vit.md
--rw-r--r--   0 root         (0) root         (0)      375 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/xlm_roberta.md
--rw-r--r--   0 root         (0) root         (0)      175 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/xpegasus.md
--rw-r--r--   0 root         (0) root         (0)      196 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/models/xprophetnet.md
--rw-r--r--   0 root         (0) root         (0)     4524 2023-07-14 20:34:48.000000 unitorch-0.0.0.5/wiki/overview.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.169260 unitorch-0.0.0.6/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.957258 unitorch-0.0.0.6/.pytest_cache/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-07-24 07:53:35.000000 unitorch-0.0.0.6/.pytest_cache/README.md
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      131 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9222 2023-07-24 07:53:46.169260 unitorch-0.0.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8187 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.957258 unitorch-0.0.0.6/benchmarks/
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/benchmarks/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.933258 unitorch-0.0.0.6/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.961258 unitorch-0.0.0.6/docs/search/
+-rw-r--r--   0 root         (0) root         (0)  1081944 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/docs/search/search_index.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.965258 unitorch-0.0.0.6/examples/
+-rw-r--r--   0 root         (0) root         (0)     2311 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.937258 unitorch-0.0.0.6/examples/configs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.965258 unitorch-0.0.0.6/examples/configs/caption/
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/caption/blip.ini
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/caption/minigpt4.ini
+-rw-r--r--   0 root         (0) root         (0)     2692 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/caption/minigpt4_ds.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.969258 unitorch-0.0.0.6/examples/configs/classification/
+-rw-r--r--   0 root         (0) root         (0)     1545 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/classification/bert.ini
+-rw-r--r--   0 root         (0) root         (0)     1700 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/classification/clip.ini
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/classification/image_clip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.973258 unitorch-0.0.0.6/examples/configs/classification/lora/
+-rw-r--r--   0 root         (0) root         (0)     1639 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/classification/lora/bloom.ini
+-rw-r--r--   0 root         (0) root         (0)     1615 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/classification/lora/bloom_ds.ini
+-rw-r--r--   0 root         (0) root         (0)     1857 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/classification/lora/llama.ini
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/classification/lora/llama_ds.ini
+-rw-r--r--   0 root         (0) root         (0)     1556 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/classification/roberta.ini
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/classification/swin.ini
+-rw-r--r--   0 root         (0) root         (0)     1636 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/classification/text_clip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.973258 unitorch-0.0.0.6/examples/configs/deepspeed/
+-rw-r--r--   0 root         (0) root         (0)      500 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/deepspeed/adamw.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.973258 unitorch-0.0.0.6/examples/configs/diffusion/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.977258 unitorch-0.0.0.6/examples/configs/diffusion/controlnet/
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/diffusion/controlnet/canny.ini
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/diffusion/stable-v1.5.ini
+-rw-r--r--   0 root         (0) root         (0)     1751 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/diffusion/stable-v2.1.ini
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/diffusion/stable-v2.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.981258 unitorch-0.0.0.6/examples/configs/generation/
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/bart.ini
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/bloom.ini
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/chatglm.ini
+-rw-r--r--   0 root         (0) root         (0)     1647 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/llama.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.981258 unitorch-0.0.0.6/examples/configs/generation/lora/
+-rw-r--r--   0 root         (0) root         (0)     1608 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/lora/bloom.ini
+-rw-r--r--   0 root         (0) root         (0)     1582 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/lora/bloom_ds.ini
+-rw-r--r--   0 root         (0) root         (0)     1604 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/lora/llama.ini
+-rw-r--r--   0 root         (0) root         (0)     1578 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/lora/llama_ds.ini
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/mbart.ini
+-rw-r--r--   0 root         (0) root         (0)     1597 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/mt5.ini
+-rw-r--r--   0 root         (0) root         (0)     1655 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/pegasus.ini
+-rw-r--r--   0 root         (0) root         (0)     1587 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/t5.ini
+-rw-r--r--   0 root         (0) root         (0)     1647 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/xpegasus.ini
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/generation/xprophetnet.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.985258 unitorch-0.0.0.6/examples/configs/pretrain/
+-rw-r--r--   0 root         (0) root         (0)     1266 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/pretrain/clip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.937258 unitorch-0.0.0.6/examples/configs/services/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.985258 unitorch-0.0.0.6/examples/configs/services/zip_image/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/services/zip_image/config.ini
+-rw-r--r--   0 root         (0) root         (0)      240 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/configs/services/zip_image/config_v2.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.937258 unitorch-0.0.0.6/examples/hub/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.985258 unitorch-0.0.0.6/examples/hub/caption/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/hub/caption/blip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.985258 unitorch-0.0.0.6/examples/hub/classification/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/hub/classification/bert.ini
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/hub/classification/clip.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.985258 unitorch-0.0.0.6/examples/hub/generation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/hub/generation/bart.ini
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/hub/generation/llama.ini
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/examples/hub/generation/xpegasus.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.985258 unitorch-0.0.0.6/notebooks/
+-rw-r--r--   0 root         (0) root         (0)      131 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/notebooks/README.md
+-rw-r--r--   0 root         (0) root         (0)     1790 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      131 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 07:53:46.173260 unitorch-0.0.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.937258 unitorch-0.0.0.6/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.985258 unitorch-0.0.0.6/src/unitorch/
+-rw-r--r--   0 root         (0) root         (0)     2670 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.989258 unitorch-0.0.0.6/src/unitorch/cli/
+-rw-r--r--   0 root         (0) root         (0)     6025 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.989258 unitorch-0.0.0.6/src/unitorch/cli/console/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/console/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/console/eval.py
+-rw-r--r--   0 root         (0) root         (0)     2072 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/console/infer.py
+-rw-r--r--   0 root         (0) root         (0)     2151 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/console/script.py
+-rw-r--r--   0 root         (0) root         (0)     4683 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/console/service.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/console/train.py
+-rw-r--r--   0 root         (0) root         (0)     4397 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.993258 unitorch-0.0.0.6/src/unitorch/cli/datasets/
+-rw-r--r--   0 root         (0) root         (0)       98 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12406 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/datasets/hf.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.993258 unitorch-0.0.0.6/src/unitorch/cli/loss/
+-rw-r--r--   0 root         (0) root         (0)     4063 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2857 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/loss/ranking.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.997258 unitorch-0.0.0.6/src/unitorch/cli/models/
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.001258 unitorch-0.0.0.6/src/unitorch/cli/models/bart/
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/bart/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/bart/fastapi.py
+-rw-r--r--   0 root         (0) root         (0)     7012 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/bart/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     6140 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/bart/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.001258 unitorch-0.0.0.6/src/unitorch/cli/models/beit/
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/beit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3142 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/beit/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/beit/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.005258 unitorch-0.0.0.6/src/unitorch/cli/models/bert/
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/bert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3903 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/bert/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     6128 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/bert/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.005258 unitorch-0.0.0.6/src/unitorch/cli/models/blip/
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/blip/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22734 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/blip/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     7788 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/blip/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.005258 unitorch-0.0.0.6/src/unitorch/cli/models/bloom/
+-rw-r--r--   0 root         (0) root         (0)     2570 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/bloom/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13074 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/bloom/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     8756 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/bloom/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.009258 unitorch-0.0.0.6/src/unitorch/cli/models/chatglm/
+-rw-r--r--   0 root         (0) root         (0)     1201 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/chatglm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13812 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/chatglm/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     8833 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/chatglm/processing.py
+-rw-r--r--   0 root         (0) root         (0)     9111 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/classification_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.009258 unitorch-0.0.0.6/src/unitorch/cli/models/clip/
+-rw-r--r--   0 root         (0) root         (0)     2514 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/clip/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16125 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/clip/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5565 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/clip/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.013258 unitorch-0.0.0.6/src/unitorch/cli/models/deberta/
+-rw-r--r--   0 root         (0) root         (0)     4492 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/deberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4077 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/deberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     4021 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/deberta/modeling_v2.py
+-rw-r--r--   0 root         (0) root         (0)     3801 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/deberta/processing.py
+-rw-r--r--   0 root         (0) root         (0)     3434 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/deberta/processing_v2.py
+-rw-r--r--   0 root         (0) root         (0)     2545 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/detection_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.017259 unitorch-0.0.0.6/src/unitorch/cli/models/diffusers/
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/diffusers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7500 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/diffusers/modeling_controlnet.py
+-rw-r--r--   0 root         (0) root         (0)     9444 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/diffusers/modeling_stable.py
+-rw-r--r--   0 root         (0) root         (0)     3879 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/diffusers/processing_controlnet.py
+-rw-r--r--   0 root         (0) root         (0)     3838 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/diffusers/processing_stable.py
+-rw-r--r--   0 root         (0) root         (0)     3126 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/diffusion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/generation_utils.py
+-rw-r--r--   0 root         (0) root         (0)     5092 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/image_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4297 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/label_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.021258 unitorch-0.0.0.6/src/unitorch/cli/models/llama/
+-rw-r--r--   0 root         (0) root         (0)     3445 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/llama/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14065 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/llama/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     8641 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/llama/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.021258 unitorch-0.0.0.6/src/unitorch/cli/models/mbart/
+-rw-r--r--   0 root         (0) root         (0)      887 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/mbart/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7650 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/mbart/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5826 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/mbart/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.021258 unitorch-0.0.0.6/src/unitorch/cli/models/minigpt4/
+-rw-r--r--   0 root         (0) root         (0)     2870 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/minigpt4/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10738 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/minigpt4/modeling.py
+-rw-r--r--   0 root         (0) root         (0)    10044 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/minigpt4/processing.py
+-rw-r--r--   0 root         (0) root         (0)    15281 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/modeling_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.025258 unitorch-0.0.0.6/src/unitorch/cli/models/mt5/
+-rw-r--r--   0 root         (0) root         (0)     1381 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/mt5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7173 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/mt5/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5815 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/mt5/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.025258 unitorch-0.0.0.6/src/unitorch/cli/models/peft/
+-rw-r--r--   0 root         (0) root         (0)      524 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/peft/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30598 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/peft/modeling_bloom.py
+-rw-r--r--   0 root         (0) root         (0)    30656 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/peft/modeling_llama.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.029259 unitorch-0.0.0.6/src/unitorch/cli/models/pegasus/
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/pegasus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7281 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/pegasus/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5885 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/pegasus/processing.py
+-rw-r--r--   0 root         (0) root         (0)     2834 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/processing_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.029259 unitorch-0.0.0.6/src/unitorch/cli/models/prophetnet/
+-rw-r--r--   0 root         (0) root         (0)      162 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/prophetnet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/prophetnet/modeling.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/prophetnet/processing.py
+-rw-r--r--   0 root         (0) root         (0)      650 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/random_utils.py
+-rw-r--r--   0 root         (0) root         (0)      535 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/ranking_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.029259 unitorch-0.0.0.6/src/unitorch/cli/models/roberta/
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/roberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/roberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     3766 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/roberta/processing.py
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/segmentation_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.033259 unitorch-0.0.0.6/src/unitorch/cli/models/swin/
+-rw-r--r--   0 root         (0) root         (0)     3032 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/swin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3225 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/swin/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2564 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/swin/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.033259 unitorch-0.0.0.6/src/unitorch/cli/models/t5/
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/t5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7192 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/t5/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5811 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/t5/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.037258 unitorch-0.0.0.6/src/unitorch/cli/models/visualbert/
+-rw-r--r--   0 root         (0) root         (0)     1310 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/visualbert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8538 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/visualbert/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     6306 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/visualbert/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.037258 unitorch-0.0.0.6/src/unitorch/cli/models/vit/
+-rw-r--r--   0 root         (0) root         (0)     4602 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/vit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3191 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/vit/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2583 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/vit/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.037258 unitorch-0.0.0.6/src/unitorch/cli/models/xlm_roberta/
+-rw-r--r--   0 root         (0) root         (0)     2314 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/xlm_roberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7533 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/xlm_roberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     3408 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/xlm_roberta/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.041259 unitorch-0.0.0.6/src/unitorch/cli/models/xpegasus/
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/xpegasus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7286 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/xpegasus/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5953 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/xpegasus/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.041259 unitorch-0.0.0.6/src/unitorch/cli/models/xprophetnet/
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/xprophetnet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7842 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/xprophetnet/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     5952 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/models/xprophetnet/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.041259 unitorch-0.0.0.6/src/unitorch/cli/optim/
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/optim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/optim/lion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.041259 unitorch-0.0.0.6/src/unitorch/cli/rl/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/rl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.045259 unitorch-0.0.0.6/src/unitorch/cli/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      141 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3084 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/scheduler/warmup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.045259 unitorch-0.0.0.6/src/unitorch/cli/score/
+-rw-r--r--   0 root         (0) root         (0)    14139 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/score/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.045259 unitorch-0.0.0.6/src/unitorch/cli/scripts/
+-rw-r--r--   0 root         (0) root         (0)      158 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/scripts/README.md
+-rw-r--r--   0 root         (0) root         (0)      213 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/scripts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.045259 unitorch-0.0.0.6/src/unitorch/cli/services/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      223 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/services/readme.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.049259 unitorch-0.0.0.6/src/unitorch/cli/services/zip_image/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/services/zip_image/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4866 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/services/zip_image/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.049259 unitorch-0.0.0.6/src/unitorch/cli/tasks/
+-rw-r--r--   0 root         (0) root         (0)      457 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26512 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/tasks/deepspeed.py
+-rw-r--r--   0 root         (0) root         (0)    31622 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/tasks/supervised.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.049259 unitorch-0.0.0.6/src/unitorch/cli/utils/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.049259 unitorch-0.0.0.6/src/unitorch/cli/writer/
+-rw-r--r--   0 root         (0) root         (0)    10544 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/cli/writer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.053259 unitorch-0.0.0.6/src/unitorch/datasets/
+-rw-r--r--   0 root         (0) root         (0)      130 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6832 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/datasets/hf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.057259 unitorch-0.0.0.6/src/unitorch/loss/
+-rw-r--r--   0 root         (0) root         (0)     4712 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1559 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/loss/prophetnet.py
+-rw-r--r--   0 root         (0) root         (0)     8411 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/loss/ranking.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.057259 unitorch-0.0.0.6/src/unitorch/models/
+-rw-r--r--   0 root         (0) root         (0)     7498 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.057259 unitorch-0.0.0.6/src/unitorch/models/bart/
+-rw-r--r--   0 root         (0) root         (0)      204 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/bart/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13719 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/bart/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/bart/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.061259 unitorch-0.0.0.6/src/unitorch/models/beit/
+-rw-r--r--   0 root         (0) root         (0)      202 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/beit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/beit/modeling.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/beit/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.061259 unitorch-0.0.0.6/src/unitorch/models/bert/
+-rw-r--r--   0 root         (0) root         (0)      208 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/bert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2446 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/bert/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     8355 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/bert/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.065259 unitorch-0.0.0.6/src/unitorch/models/blip/
+-rw-r--r--   0 root         (0) root         (0)      306 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/blip/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30337 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/blip/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     7704 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/blip/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.065259 unitorch-0.0.0.6/src/unitorch/models/blip2/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/blip2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      606 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/blip2/modeling.py
+-rw-r--r--   0 root         (0) root         (0)      663 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/blip2/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.069259 unitorch-0.0.0.6/src/unitorch/models/bloom/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/bloom/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10885 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/bloom/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     9108 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/bloom/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.073259 unitorch-0.0.0.6/src/unitorch/models/chatglm/
+-rw-r--r--   0 root         (0) root         (0)      259 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/chatglm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4201 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/chatglm/configuration_chatglm.py
+-rw-r--r--   0 root         (0) root         (0)    11175 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/chatglm/modeling.py
+-rw-r--r--   0 root         (0) root         (0)    55823 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/chatglm/modeling_chatglm.py
+-rw-r--r--   0 root         (0) root         (0)    11091 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/chatglm/processing.py
+-rw-r--r--   0 root         (0) root         (0)    15625 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/chatglm/quantization.py
+-rw-r--r--   0 root         (0) root         (0)    16827 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/chatglm/tokenization_chatglm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.077259 unitorch-0.0.0.6/src/unitorch/models/clip/
+-rw-r--r--   0 root         (0) root         (0)      281 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/clip/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15100 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/clip/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     4393 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/clip/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.077259 unitorch-0.0.0.6/src/unitorch/models/deberta/
+-rw-r--r--   0 root         (0) root         (0)      424 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/deberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4503 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/deberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2568 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/deberta/modeling_v2.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/deberta/processing.py
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/deberta/processing_v2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.081259 unitorch-0.0.0.6/src/unitorch/models/diffusers/
+-rw-r--r--   0 root         (0) root         (0)      547 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/diffusers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6076 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/diffusers/modeling_controlnet.py
+-rw-r--r--   0 root         (0) root         (0)     8201 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/diffusers/modeling_stable.py
+-rw-r--r--   0 root         (0) root         (0)     3313 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/diffusers/processing_controlnet.py
+-rw-r--r--   0 root         (0) root         (0)     3029 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/diffusers/processing_stable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.085259 unitorch-0.0.0.6/src/unitorch/models/llama/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/llama/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11394 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/llama/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     8944 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/llama/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.085259 unitorch-0.0.0.6/src/unitorch/models/mbart/
+-rw-r--r--   0 root         (0) root         (0)      188 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/mbart/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13976 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/mbart/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2163 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/mbart/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.089259 unitorch-0.0.0.6/src/unitorch/models/minigpt4/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/minigpt4/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17053 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/minigpt4/modeling.py
+-rw-r--r--   0 root         (0) root         (0)    13727 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/minigpt4/processing.py
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/modeling_ema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.089259 unitorch-0.0.0.6/src/unitorch/models/mt5/
+-rw-r--r--   0 root         (0) root         (0)      180 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/mt5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14250 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/mt5/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/mt5/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.093259 unitorch-0.0.0.6/src/unitorch/models/peft/
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/peft/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9934 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/peft/modeling_bloom_adalora.py
+-rw-r--r--   0 root         (0) root         (0)     9530 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/peft/modeling_bloom_lora.py
+-rw-r--r--   0 root         (0) root         (0)    10125 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/peft/modeling_llama_adalora.py
+-rw-r--r--   0 root         (0) root         (0)     9309 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/peft/modeling_llama_lora.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/peft/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.097259 unitorch-0.0.0.6/src/unitorch/models/pegasus/
+-rw-r--r--   0 root         (0) root         (0)      196 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/pegasus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13652 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/pegasus/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/pegasus/processing.py
+-rw-r--r--   0 root         (0) root         (0)    13125 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/processing_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.097259 unitorch-0.0.0.6/src/unitorch/models/prophetnet/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/prophetnet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7435 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/prophetnet/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/prophetnet/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.097259 unitorch-0.0.0.6/src/unitorch/models/roberta/
+-rw-r--r--   0 root         (0) root         (0)      218 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/roberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4281 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/roberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/roberta/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.101259 unitorch-0.0.0.6/src/unitorch/models/swin/
+-rw-r--r--   0 root         (0) root         (0)      193 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/swin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1534 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/swin/modeling.py
+-rw-r--r--   0 root         (0) root         (0)      998 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/swin/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.101259 unitorch-0.0.0.6/src/unitorch/models/t5/
+-rw-r--r--   0 root         (0) root         (0)      194 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/t5/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13316 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/t5/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/t5/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.105259 unitorch-0.0.0.6/src/unitorch/models/visualbert/
+-rw-r--r--   0 root         (0) root         (0)      248 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/visualbert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6710 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/visualbert/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     2132 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/visualbert/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.105259 unitorch-0.0.0.6/src/unitorch/models/vit/
+-rw-r--r--   0 root         (0) root         (0)      189 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/vit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/vit/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/vit/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.109259 unitorch-0.0.0.6/src/unitorch/models/xlm_roberta/
+-rw-r--r--   0 root         (0) root         (0)      323 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/xlm_roberta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7381 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/xlm_roberta/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/xlm_roberta/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.109259 unitorch-0.0.0.6/src/unitorch/models/xpegasus/
+-rw-r--r--   0 root         (0) root         (0)      237 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/xpegasus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13741 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/xpegasus/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/xpegasus/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.109259 unitorch-0.0.0.6/src/unitorch/models/xprophetnet/
+-rw-r--r--   0 root         (0) root         (0)      212 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/xprophetnet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13545 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/xprophetnet/modeling.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/models/xprophetnet/processing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.113259 unitorch-0.0.0.6/src/unitorch/modules/
+-rw-r--r--   0 root         (0) root         (0)      133 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/modules/classifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.117259 unitorch-0.0.0.6/src/unitorch/modules/replace/
+-rw-r--r--   0 root         (0) root         (0)      199 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/modules/replace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14643 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/modules/replace/beam_search_v2.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/modules/replace/datasets_v2.py
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/modules/replace/hf_hub_v2.py
+-rw-r--r--   0 root         (0) root         (0)     2053 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/modules/timm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.117259 unitorch-0.0.0.6/src/unitorch/ops/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/ops/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16794 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/ops/dyhead.py
+-rw-r--r--   0 root         (0) root         (0)     1347 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/ops/ngram_repeat_block.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.117259 unitorch-0.0.0.6/src/unitorch/optim/
+-rw-r--r--   0 root         (0) root         (0)      203 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/optim/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3201 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/optim/lion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.121259 unitorch-0.0.0.6/src/unitorch/rl/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/rl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.121259 unitorch-0.0.0.6/src/unitorch/rl/utils/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/rl/utils/buffer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.121259 unitorch-0.0.0.6/src/unitorch/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      149 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/scheduler/warmup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.125259 unitorch-0.0.0.6/src/unitorch/score/
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/score/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4297 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/score/bleu.py
+-rw-r--r--   0 root         (0) root         (0)     7852 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/score/map.py
+-rw-r--r--   0 root         (0) root         (0)    13291 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/score/rouge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.125259 unitorch-0.0.0.6/src/unitorch/tasks/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.129259 unitorch-0.0.0.6/src/unitorch/utils/
+-rw-r--r--   0 root         (0) root         (0)    13662 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2236 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/utils/decorators.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/utils/functional.py
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/utils/image_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2711 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/utils/import_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2639 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/utils/io.py
+-rw-r--r--   0 root         (0) root         (0)     5027 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/utils/palette.py
+-rw-r--r--   0 root         (0) root         (0)     3851 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/src/unitorch/utils/torch_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.985258 unitorch-0.0.0.6/src/unitorch.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9222 2023-07-24 07:53:45.000000 unitorch-0.0.0.6/src/unitorch.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13624 2023-07-24 07:53:45.000000 unitorch-0.0.0.6/src/unitorch.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 07:53:45.000000 unitorch-0.0.0.6/src/unitorch.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      287 2023-07-24 07:53:45.000000 unitorch-0.0.0.6/src/unitorch.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      356 2023-07-24 07:53:45.000000 unitorch-0.0.0.6/src/unitorch.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-24 07:53:45.000000 unitorch-0.0.0.6/src/unitorch.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.129259 unitorch-0.0.0.6/wiki/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.133259 unitorch-0.0.0.6/wiki/benchmarks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/benchmarks/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.141259 unitorch-0.0.0.6/wiki/cli/
+-rw-r--r--   0 root         (0) root         (0)      504 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/ast.md
+-rw-r--r--   0 root         (0) root         (0)      173 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/csv.md
+-rw-r--r--   0 root         (0) root         (0)      414 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/datatypes.md
+-rw-r--r--   0 root         (0) root         (0)      197 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/deepspeed.md
+-rw-r--r--   0 root         (0) root         (0)      181 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/jsonl.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.153259 unitorch-0.0.0.6/wiki/cli/models/
+-rw-r--r--   0 root         (0) root         (0)      348 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/bart.md
+-rw-r--r--   0 root         (0) root         (0)      379 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/beit.md
+-rw-r--r--   0 root         (0) root         (0)      364 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/bert.md
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/blip.md
+-rw-r--r--   0 root         (0) root         (0)      719 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/bloom.md
+-rw-r--r--   0 root         (0) root         (0)      761 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/chatglm.md
+-rw-r--r--   0 root         (0) root         (0)      939 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/clip.md
+-rw-r--r--   0 root         (0) root         (0)      783 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/deberta.md
+-rw-r--r--   0 root         (0) root         (0)      353 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/diffusers.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/index.md
+-rw-r--r--   0 root         (0) root         (0)      719 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/llama.md
+-rw-r--r--   0 root         (0) root         (0)      359 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/mbart.md
+-rw-r--r--   0 root         (0) root         (0)      227 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/minigpt4.md
+-rw-r--r--   0 root         (0) root         (0)      337 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/mt5.md
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/peft.md
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/pegasus.md
+-rw-r--r--   0 root         (0) root         (0)       36 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/prophetnet.md
+-rw-r--r--   0 root         (0) root         (0)      398 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/roberta.md
+-rw-r--r--   0 root         (0) root         (0)      379 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/swin.md
+-rw-r--r--   0 root         (0) root         (0)      326 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/t5.md
+-rw-r--r--   0 root         (0) root         (0)      623 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/visualbert.md
+-rw-r--r--   0 root         (0) root         (0)      368 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/vit.md
+-rw-r--r--   0 root         (0) root         (0)      664 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/xlm_roberta.md
+-rw-r--r--   0 root         (0) root         (0)      392 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/xpegasus.md
+-rw-r--r--   0 root         (0) root         (0)      425 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/models/xprophetnet.md
+-rw-r--r--   0 root         (0) root         (0)      189 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/parquet.md
+-rw-r--r--   0 root         (0) root         (0)      851 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/postprocess.md
+-rw-r--r--   0 root         (0) root         (0)      146 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/preprocess.md
+-rw-r--r--   0 root         (0) root         (0)      192 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/cli/supervised.md
+-rw-r--r--   0 root         (0) root         (0)     4600 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/configuration.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:45.957258 unitorch-0.0.0.6/wiki/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.153259 unitorch-0.0.0.6/wiki/examples/caption/
+-rw-r--r--   0 root         (0) root         (0)     4659 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/examples/caption/blip.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.153259 unitorch-0.0.0.6/wiki/examples/classification/
+-rw-r--r--   0 root         (0) root         (0)     4208 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/examples/classification/clip.md
+-rw-r--r--   0 root         (0) root         (0)     4130 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/examples/classification/roberta.md
+-rw-r--r--   0 root         (0) root         (0)     4525 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/examples/classification/swin.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.153259 unitorch-0.0.0.6/wiki/examples/diffusion/
+-rw-r--r--   0 root         (0) root         (0)       32 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/examples/diffusion/controlnet.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.157260 unitorch-0.0.0.6/wiki/examples/generation/
+-rw-r--r--   0 root         (0) root         (0)     4145 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/examples/generation/bart.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.157260 unitorch-0.0.0.6/wiki/examples/service/
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/examples/service/zip_image.md
+-rw-r--r--   0 root         (0) root         (0)     1346 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/index.md
+-rw-r--r--   0 root         (0) root         (0)      890 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/installation.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.157260 unitorch-0.0.0.6/wiki/labs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/labs/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 07:53:46.169260 unitorch-0.0.0.6/wiki/models/
+-rw-r--r--   0 root         (0) root         (0)      147 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/bart.md
+-rw-r--r--   0 root         (0) root         (0)      165 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/beit.md
+-rw-r--r--   0 root         (0) root         (0)      155 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/bert.md
+-rw-r--r--   0 root         (0) root         (0)      453 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/blip.md
+-rw-r--r--   0 root         (0) root         (0)      296 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/bloom.md
+-rw-r--r--   0 root         (0) root         (0)      322 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/chatglm.md
+-rw-r--r--   0 root         (0) root         (0)      383 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/clip.md
+-rw-r--r--   0 root         (0) root         (0)      402 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/deberta.md
+-rw-r--r--   0 root         (0) root         (0)      152 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/diffusers.md
+-rw-r--r--   0 root         (0) root         (0)      450 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/index.md
+-rw-r--r--   0 root         (0) root         (0)      296 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/llama.md
+-rw-r--r--   0 root         (0) root         (0)      154 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/mbart.md
+-rw-r--r--   0 root         (0) root         (0)      297 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/minigpt4.md
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/mt5.md
+-rw-r--r--   0 root         (0) root         (0)      695 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/peft.md
+-rw-r--r--   0 root         (0) root         (0)      168 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/pegasus.md
+-rw-r--r--   0 root         (0) root         (0)      107 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/prophetnet.md
+-rw-r--r--   0 root         (0) root         (0)      243 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/roberta.md
+-rw-r--r--   0 root         (0) root         (0)      165 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/swin.md
+-rw-r--r--   0 root         (0) root         (0)      133 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/t5.md
+-rw-r--r--   0 root         (0) root         (0)      277 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/visualbert.md
+-rw-r--r--   0 root         (0) root         (0)      158 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/vit.md
+-rw-r--r--   0 root         (0) root         (0)      375 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/xlm_roberta.md
+-rw-r--r--   0 root         (0) root         (0)      175 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/xpegasus.md
+-rw-r--r--   0 root         (0) root         (0)      196 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/models/xprophetnet.md
+-rw-r--r--   0 root         (0) root         (0)     4524 2023-07-24 07:44:56.000000 unitorch-0.0.0.6/wiki/overview.md
```

### Comparing `unitorch-0.0.0.5/LICENSE` & `unitorch-0.0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/PKG-INFO` & `unitorch-0.0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitorch
-Version: 0.0.0.5
+Version: 0.0.0.6
 Summary: unitorch provides efficient implementation of popular unified NLU / NLG / CV / CTR / MM / RL models with PyTorch.
 Author-email: fuliucansheng <fuliucansheng@gmail.com>
 License: MIT
 Keywords: PyTorch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -18,15 +18,14 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: deepspeed
 Provides-Extra: diffusers
 Provides-Extra: accelerate
 Provides-Extra: chatglm
-Provides-Extra: fastapi
 Provides-Extra: all
 License-File: LICENSE
 
 <div align="Center"> 
 
 ![unitorch](unitorch.png)
```

### Comparing `unitorch-0.0.0.5/README.md` & `unitorch-0.0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/docs/search/search_index.json` & `unitorch-0.0.0.6/docs/search/search_index.json`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/README.md` & `unitorch-0.0.0.6/examples/README.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/caption/blip.ini` & `unitorch-0.0.0.6/examples/configs/caption/blip.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/caption/minigpt4.ini` & `unitorch-0.0.0.6/examples/configs/caption/minigpt4.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/caption/minigpt4_ds.ini` & `unitorch-0.0.0.6/examples/configs/caption/minigpt4_ds.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/classification/bert.ini` & `unitorch-0.0.0.6/examples/configs/classification/bert.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/classification/clip.ini` & `unitorch-0.0.0.6/examples/configs/classification/clip.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/classification/image_clip.ini` & `unitorch-0.0.0.6/examples/configs/classification/image_clip.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/classification/lora/bloom.ini` & `unitorch-0.0.0.6/examples/configs/classification/lora/bloom.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/classification/lora/bloom_ds.ini` & `unitorch-0.0.0.6/examples/configs/classification/lora/bloom_ds.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/classification/lora/llama.ini` & `unitorch-0.0.0.6/examples/configs/classification/lora/llama.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/classification/lora/llama_ds.ini` & `unitorch-0.0.0.6/examples/configs/classification/lora/llama_ds.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/classification/roberta.ini` & `unitorch-0.0.0.6/examples/configs/classification/roberta.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/classification/swin.ini` & `unitorch-0.0.0.6/examples/configs/classification/swin.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/classification/text_clip.ini` & `unitorch-0.0.0.6/examples/configs/classification/text_clip.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/diffusion/controlnet/canny.ini` & `unitorch-0.0.0.6/examples/configs/diffusion/controlnet/canny.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/diffusion/stable-v1.5.ini` & `unitorch-0.0.0.6/examples/configs/diffusion/stable-v1.5.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/diffusion/stable-v2.1.ini` & `unitorch-0.0.0.6/examples/configs/diffusion/stable-v2.1.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/diffusion/stable-v2.ini` & `unitorch-0.0.0.6/examples/configs/diffusion/stable-v2.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/generation/bart.ini` & `unitorch-0.0.0.6/examples/configs/generation/bart.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/generation/bloom.ini` & `unitorch-0.0.0.6/examples/configs/generation/bloom.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/generation/chatglm.ini` & `unitorch-0.0.0.6/examples/configs/generation/chatglm.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/generation/llama.ini` & `unitorch-0.0.0.6/examples/configs/generation/llama.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/generation/lora/bloom.ini` & `unitorch-0.0.0.6/examples/configs/generation/lora/bloom.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/generation/lora/bloom_ds.ini` & `unitorch-0.0.0.6/examples/configs/generation/lora/bloom_ds.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/generation/lora/llama.ini` & `unitorch-0.0.0.6/examples/configs/generation/lora/llama.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/generation/lora/llama_ds.ini` & `unitorch-0.0.0.6/examples/configs/generation/lora/llama_ds.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/generation/mbart.ini` & `unitorch-0.0.0.6/examples/configs/generation/mbart.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/generation/mt5.ini` & `unitorch-0.0.0.6/examples/configs/generation/mt5.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/generation/pegasus.ini` & `unitorch-0.0.0.6/examples/configs/generation/pegasus.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/generation/t5.ini` & `unitorch-0.0.0.6/examples/configs/generation/t5.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/generation/xpegasus.ini` & `unitorch-0.0.0.6/examples/configs/generation/xpegasus.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/generation/xprophetnet.ini` & `unitorch-0.0.0.6/examples/configs/generation/xprophetnet.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/examples/configs/pretrain/clip.ini` & `unitorch-0.0.0.6/examples/configs/pretrain/clip.ini`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/pyproject.toml` & `unitorch-0.0.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -28,24 +28,22 @@
 dynamic = ["version", "dependencies"]
 
 [project.optional-dependencies]
 deepspeed = ["deepspeed==0.9.0", "mpi4py==3.1.4"]
 diffusers = ["diffusers==0.16.1"]
 accelerate = ["accelerate==0.20.3"]
 chatglm = ["protobuf==3.20.0", "icetk==0.0.4", "cpm_kernels==1.0.11"]
-fastapi = ["fastapi>=0.99.0"]
 all = ["unitorch[deepspeed,diffusers,accelerate,chatglm]"]
 
 [project.scripts]
 unitorch-train = "unitorch.cli.console.train:cli_main"
 unitorch-eval = "unitorch.cli.console.eval:cli_main"
 unitorch-infer = "unitorch.cli.console.infer:cli_main"
 unitorch-script= "unitorch.cli.console.script:cli_main"
 unitorch-service = "unitorch.cli.console.service:cli_main"
-unitorch-fastapi = "unitorch.cli.console.fastapi:cli_main"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
```

### Comparing `unitorch-0.0.0.5/setup.py` & `unitorch-0.0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/__init__.py` & `unitorch-0.0.0.6/src/unitorch/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 def get_cache_home():
     return UNITORCH_CACHE
 
 
 ### version
-VERSION = "0.0.0.5"
+VERSION = "0.0.0.6"
 
 ### is offline mode
 UNITORCH_OFFLINE = os.environ.get("UNITORCH_OFFLINE", "0").upper()
 
 
 def is_offline_mode():
     return UNITORCH_OFFLINE in ENV_VARS_TRUE_VALUES
```

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,14 +226,15 @@
 
 registered_service = dict()
 register_service = partial(
     registry_func,
     save_dict=registered_service,
 )
 
+
 # usful function
 from unitorch.cli.writer import WriterMixin, WriterOutputs
 
 # import cli modules
 import unitorch.cli.datasets
 import unitorch.cli.loss
 import unitorch.cli.models
```

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/console/eval.py` & `unitorch-0.0.0.6/src/unitorch/cli/console/eval.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/console/infer.py` & `unitorch-0.0.0.6/src/unitorch/cli/console/infer.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/console/script.py` & `unitorch-0.0.0.6/src/unitorch/cli/console/script.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/console/service.py` & `unitorch-0.0.0.6/src/unitorch/cli/console/service.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/console/train.py` & `unitorch-0.0.0.6/src/unitorch/cli/console/train.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/core.py` & `unitorch-0.0.0.6/src/unitorch/cli/core.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/datasets/hf.py` & `unitorch-0.0.0.6/src/unitorch/cli/datasets/hf.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/decorators.py` & `unitorch-0.0.0.6/src/unitorch/cli/decorators.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/loss/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/loss/ranking.py` & `unitorch-0.0.0.6/src/unitorch/cli/loss/ranking.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/bart/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/bart/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/bart/modeling.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/bart/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/bart/processing.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/bart/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/beit/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/beit/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/beit/modeling.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/beit/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/beit/processing.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/beit/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/bert/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/bert/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/bert/modeling.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/bert/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/bert/processing.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/bert/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/blip/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/blip/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/blip/modeling.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/blip/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/blip/processing.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/blip/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/bloom/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/bloom/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/bloom/modeling.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/bloom/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/bloom/processing.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/bloom/processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) FULIUCANSHENG.
 # Licensed under the MIT License.
 
+import re
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 from unitorch.utils import pop_value, nested_dict_value
 from unitorch.models.bloom import BloomProcessor as _BloomProcessor
 from unitorch.cli import (
     cached_path,
     add_default_section_for_init,
     add_default_section_for_function,
@@ -245,9 +246,18 @@
         Returns:
             WriterOutputs: The detokenized writer outputs.
         """
         results = outputs.to_pandas()
         assert results.shape[0] == 0 or results.shape[0] == outputs.sequences.shape[0]
 
         decoded = super().detokenize(sequences=outputs.sequences)
+        cleanup_string = lambda text: re.sub(r"\n", " ", text)
+        if isinstance(decoded[0], list):
+            decoded = [list(map(cleanup_string, sequence)) for sequence in decoded]
+        elif isinstance(decoded[0], str):
+            decoded = list(map(cleanup_string, decoded))
+        else:
+            raise ValueError(
+                f"Unsupported type for minigpt4 detokenize: {type(decoded[0])}"
+            )
         results["decoded"] = decoded
         return WriterOutputs(results)
```

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/chatglm/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/chatglm/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/chatglm/modeling.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/chatglm/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/chatglm/processing.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/chatglm/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/classification_utils.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/classification_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -109,26 +109,23 @@
             WriterOutputs: Processed outputs with scores.
         """
         assert outputs.outputs.dim() == 2
 
         results = outputs.to_pandas()
         assert results.shape[0] == 0 or results.shape[0] == outputs.outputs.shape[0]
 
+        outputs = outputs.outputs.numpy()
         if self.act_fn is not None:
-            outputs.outputs = self.act_fn(outputs.outputs)
+            outputs = self.act_fn(outputs)
 
-        if outputs.outputs.dim() == 2:
-            pscore = (
-                outputs.outputs[:, 1]
-                if outputs.outputs.size(-1) > 1
-                else outputs.outputs[:, 0]
-            )
+        if outputs.ndim == 2:
+            pscore = outputs[:, 1] if outputs.shape[-1] > 1 else outputs[:, 0]
             results["pscore"] = pscore.tolist()
         else:
-            results["pscore"] = outputs.outputs.tolist()
+            results["pscore"] = outputs.tolist()
         return WriterOutputs(results)
 
     @register_process("core/postprocess/classification/score")
     def _classifier_score(
         self,
         outputs: ClassificationOutputs,
     ):
@@ -168,40 +165,40 @@
 
         Returns:
             WriterOutputs: Processed outputs with embeddings.
         """
         results = outputs.to_pandas()
         assert results.shape[0] == 0 or results.shape[0] == outputs.embedding.shape[0]
 
-        embedding = outputs.embedding
-        if embedding.dim() > 2:
+        embedding = outputs.embedding.numpy()
+        if embedding.ndim > 2:
             embedding = embedding.reshape(embedding.size(0), -1)
         results["embedding"] = embedding.tolist()
 
-        embedding1 = outputs.embedding1
-        if embedding1.numel() > 0:
-            if embedding1.dim() > 2:
+        embedding1 = outputs.embedding1.numpy()
+        if embedding1.size > 0:
+            if embedding1.ndim > 2:
                 embedding1 = embedding1.reshape(embedding1.size(0), -1)
             results["embedding1"] = embedding1.tolist()
 
-        embedding2 = outputs.embedding2
-        if embedding2.numel() > 0:
-            if embedding2.dim() > 2:
+        embedding2 = outputs.embedding2.numpy()
+        if embedding2.size > 0:
+            if embedding2.ndim > 2:
                 embedding2 = embedding2.reshape(embedding2.size(0), -1)
             results["embedding2"] = embedding2.tolist()
 
-        embedding3 = outputs.embedding3
-        if embedding3.numel() > 0:
-            if embedding3.dim() > 2:
+        embedding3 = outputs.embedding3.numpy()
+        if embedding3.size > 0:
+            if embedding3.ndim > 2:
                 embedding3 = embedding3.reshape(embedding3.size(0), -1)
             results["embedding3"] = embedding3.tolist()
 
-        embedding4 = outputs.embedding4
-        if embedding4.numel() > 0:
-            if embedding4.dim() > 2:
+        embedding4 = outputs.embedding4.numpy()
+        if embedding4.size > 0:
+            if embedding4.ndim > 2:
                 embedding4 = embedding4.reshape(embedding4.size(0), -1)
             results["embedding4"] = embedding4.tolist()
 
         return WriterOutputs(results)
 
     @register_process("core/postprocess/classification/embedding/string")
     def _embedding_string(
@@ -216,52 +213,52 @@
 
         Returns:
             WriterOutputs: Processed outputs with string representations of embeddings.
         """
         results = outputs.to_pandas()
         assert results.shape[0] == 0 or results.shape[0] == outputs.embedding.shape[0]
 
-        embedding = outputs.embedding
-        if embedding.dim() > 2:
+        embedding = outputs.embedding.numpy()
+        if embedding.ndim > 2:
             embedding = embedding.reshape(embedding.size(0), -1)
         results["embedding"] = embedding.tolist()
         results["embedding"] = results["embedding"].map(
             lambda x: " ".join([str(i) for i in x])
         )
 
-        embedding1 = outputs.embedding1
-        if embedding1.numel() > 0:
-            if embedding1.dim() > 2:
+        embedding1 = outputs.embedding1.numpy()
+        if embedding1.size > 0:
+            if embedding1.ndim > 2:
                 embedding1 = embedding1.reshape(embedding1.size(0), -1)
             results["embedding1"] = embedding1.tolist()
             results["embedding1"] = results["embedding1"].map(
                 lambda x: " ".join([str(i) for i in x])
             )
 
-        embedding2 = outputs.embedding2
-        if embedding2.numel() > 0:
-            if embedding2.dim() > 2:
+        embedding2 = outputs.embedding2.numpy()
+        if embedding2.size > 0:
+            if embedding2.ndim > 2:
                 embedding2 = embedding2.reshape(embedding2.size(0), -1)
             results["embedding2"] = embedding2.tolist()
             results["embedding2"] = results["embedding2"].map(
                 lambda x: " ".join([str(i) for i in x])
             )
 
-        embedding3 = outputs.embedding3
-        if embedding3.numel() > 0:
-            if embedding3.dim() > 2:
+        embedding3 = outputs.embedding3.numpy()
+        if embedding3.size > 0:
+            if embedding3.ndim > 2:
                 embedding3 = embedding3.reshape(embedding3.size(0), -1)
             results["embedding3"] = embedding3.tolist()
             results["embedding3"] = results["embedding3"].map(
                 lambda x: " ".join([str(i) for i in x])
             )
 
-        embedding4 = outputs.embedding4
-        if embedding4.numel() > 0:
-            if embedding4.dim() > 2:
+        embedding4 = outputs.embedding4.numpy()
+        if embedding4.size > 0:
+            if embedding4.ndim > 2:
                 embedding4 = embedding4.reshape(embedding4.size(0), -1)
             results["embedding4"] = embedding4.tolist()
             results["embedding4"] = results["embedding4"].map(
                 lambda x: " ".join([str(i) for i in x])
             )
 
         return WriterOutputs(results)
```

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/clip/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/clip/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/clip/modeling.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/clip/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/clip/processing.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/clip/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/deberta/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/deberta/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/deberta/modeling.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/deberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/deberta/modeling_v2.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/deberta/modeling_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/deberta/processing.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/deberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/deberta/processing_v2.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/deberta/processing_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/detection_utils.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/detection_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/diffusers/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/diffusers/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/diffusers/modeling_controlnet.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/diffusers/modeling_controlnet.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/diffusers/modeling_stable.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/diffusers/modeling_stable.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/diffusers/processing_controlnet.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/diffusers/processing_controlnet.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/diffusers/processing_stable.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/diffusers/processing_stable.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/diffusion_utils.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/diffusion_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/generation_utils.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/generation_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/image_utils.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/image_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/label_utils.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/label_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/llama/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/llama/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/llama/modeling.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/llama/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/llama/processing.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/llama/processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Copyright (c) FULIUCANSHENG.
 # Licensed under the MIT License.
 
+import re
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 from unitorch.utils import pop_value, nested_dict_value
 from unitorch.models.llama import LlamaProcessor as _LlamaProcessor
 from unitorch.cli import (
     cached_path,
     add_default_section_for_init,
     add_default_section_for_function,
@@ -246,9 +247,18 @@
         Returns:
             WriterOutputs: The detokenized writer outputs.
         """
         results = outputs.to_pandas()
         assert results.shape[0] == 0 or results.shape[0] == outputs.sequences.shape[0]
 
         decoded = super().detokenize(sequences=outputs.sequences)
+        cleanup_string = lambda text: re.sub(r"\n", " ", text)
+        if isinstance(decoded[0], list):
+            decoded = [list(map(cleanup_string, sequence)) for sequence in decoded]
+        elif isinstance(decoded[0], str):
+            decoded = list(map(cleanup_string, decoded))
+        else:
+            raise ValueError(
+                f"Unsupported type for minigpt4 detokenize: {type(decoded[0])}"
+            )
         results["decoded"] = decoded
         return WriterOutputs(results)
```

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/mbart/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/mbart/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/mbart/modeling.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/mbart/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/mbart/processing.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/mbart/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/minigpt4/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/minigpt4/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/minigpt4/modeling.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/minigpt4/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/minigpt4/processing.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/minigpt4/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/modeling_utils.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/modeling_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/mt5/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/mt5/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/mt5/modeling.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/mt5/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/mt5/processing.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/mt5/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/peft/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/peft/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/peft/modeling_bloom.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/peft/modeling_bloom.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/peft/modeling_llama.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/peft/modeling_llama.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/pegasus/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/pegasus/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/pegasus/modeling.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/pegasus/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/pegasus/processing.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/pegasus/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/processing_utils.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/processing_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/random_utils.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/random_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/ranking_utils.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/ranking_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/roberta/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/roberta/modeling.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/roberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/roberta/processing.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/roberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/segmentation_utils.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/segmentation_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/swin/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/swin/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/swin/modeling.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/swin/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/swin/processing.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/swin/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/t5/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/t5/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/t5/modeling.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/t5/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/t5/processing.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/t5/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/visualbert/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/visualbert/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/visualbert/modeling.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/visualbert/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/visualbert/processing.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/visualbert/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/vit/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/vit/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/vit/modeling.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/vit/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/vit/processing.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/vit/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/xlm_roberta/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/xlm_roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/xlm_roberta/modeling.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/xlm_roberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/xlm_roberta/processing.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/xlm_roberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/xpegasus/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/xpegasus/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/xpegasus/modeling.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/xpegasus/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/xpegasus/processing.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/xpegasus/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/xprophetnet/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/xprophetnet/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/xprophetnet/modeling.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/xprophetnet/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/models/xprophetnet/processing.py` & `unitorch-0.0.0.6/src/unitorch/cli/models/xprophetnet/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/optim/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/optim/lion.py` & `unitorch-0.0.0.6/src/unitorch/cli/optim/lion.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/scheduler/warmup.py` & `unitorch-0.0.0.6/src/unitorch/cli/scheduler/warmup.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/score/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/score/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/services/zip_image/service.py` & `unitorch-0.0.0.6/src/unitorch/cli/services/zip_image/service.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/tasks/deepspeed.py` & `unitorch-0.0.0.6/src/unitorch/cli/tasks/deepspeed.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/tasks/supervised.py` & `unitorch-0.0.0.6/src/unitorch/cli/tasks/supervised.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/cli/writer/__init__.py` & `unitorch-0.0.0.6/src/unitorch/cli/writer/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/datasets/hf.py` & `unitorch-0.0.0.6/src/unitorch/datasets/hf.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/loss/__init__.py` & `unitorch-0.0.0.6/src/unitorch/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/loss/prophetnet.py` & `unitorch-0.0.0.6/src/unitorch/loss/prophetnet.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/loss/ranking.py` & `unitorch-0.0.0.6/src/unitorch/loss/ranking.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/__init__.py` & `unitorch-0.0.0.6/src/unitorch/models/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/bart/modeling.py` & `unitorch-0.0.0.6/src/unitorch/models/bart/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/bart/processing.py` & `unitorch-0.0.0.6/src/unitorch/models/bart/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/beit/modeling.py` & `unitorch-0.0.0.6/src/unitorch/models/beit/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/beit/processing.py` & `unitorch-0.0.0.6/src/unitorch/models/beit/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/bert/modeling.py` & `unitorch-0.0.0.6/src/unitorch/models/bert/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/bert/processing.py` & `unitorch-0.0.0.6/src/unitorch/models/bert/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/blip/modeling.py` & `unitorch-0.0.0.6/src/unitorch/models/blip/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/blip/processing.py` & `unitorch-0.0.0.6/src/unitorch/models/blip/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/blip2/modeling.py` & `unitorch-0.0.0.6/src/unitorch/models/blip2/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/blip2/processing.py` & `unitorch-0.0.0.6/src/unitorch/models/blip2/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/bloom/modeling.py` & `unitorch-0.0.0.6/src/unitorch/models/bloom/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/bloom/processing.py` & `unitorch-0.0.0.6/src/unitorch/models/bloom/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/chatglm/configuration_chatglm.py` & `unitorch-0.0.0.6/src/unitorch/models/chatglm/configuration_chatglm.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/chatglm/modeling.py` & `unitorch-0.0.0.6/src/unitorch/models/chatglm/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/chatglm/modeling_chatglm.py` & `unitorch-0.0.0.6/src/unitorch/models/chatglm/modeling_chatglm.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/chatglm/processing.py` & `unitorch-0.0.0.6/src/unitorch/models/chatglm/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/chatglm/quantization.py` & `unitorch-0.0.0.6/src/unitorch/models/chatglm/quantization.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/chatglm/tokenization_chatglm.py` & `unitorch-0.0.0.6/src/unitorch/models/chatglm/tokenization_chatglm.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/clip/modeling.py` & `unitorch-0.0.0.6/src/unitorch/models/clip/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/clip/processing.py` & `unitorch-0.0.0.6/src/unitorch/models/clip/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/deberta/modeling.py` & `unitorch-0.0.0.6/src/unitorch/models/deberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/deberta/modeling_v2.py` & `unitorch-0.0.0.6/src/unitorch/models/deberta/modeling_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/deberta/processing.py` & `unitorch-0.0.0.6/src/unitorch/models/deberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/deberta/processing_v2.py` & `unitorch-0.0.0.6/src/unitorch/models/deberta/processing_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/diffusers/__init__.py` & `unitorch-0.0.0.6/src/unitorch/models/diffusers/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/diffusers/modeling_controlnet.py` & `unitorch-0.0.0.6/src/unitorch/models/diffusers/modeling_controlnet.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/diffusers/modeling_stable.py` & `unitorch-0.0.0.6/src/unitorch/models/diffusers/modeling_stable.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/diffusers/processing_controlnet.py` & `unitorch-0.0.0.6/src/unitorch/models/diffusers/processing_controlnet.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/diffusers/processing_stable.py` & `unitorch-0.0.0.6/src/unitorch/models/diffusers/processing_stable.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/llama/modeling.py` & `unitorch-0.0.0.6/src/unitorch/models/llama/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/llama/processing.py` & `unitorch-0.0.0.6/src/unitorch/models/llama/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/mbart/modeling.py` & `unitorch-0.0.0.6/src/unitorch/models/mbart/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/mbart/processing.py` & `unitorch-0.0.0.6/src/unitorch/models/mbart/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/minigpt4/modeling.py` & `unitorch-0.0.0.6/src/unitorch/models/minigpt4/modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,15 +231,15 @@
     capabilities. It inherits from the GenericModel class.
     """
 
     prefix_keys_in_state_dict = {
         "^qformer.": "model.",
         "^query_tokens": "model.",
         "^vision_model.": "model.",
-        "^(?!model\.llama\.|model\.language_projection\.)model\.": "model.llama.",
+        "^(?!model\.llama\.|model\.language_projection\.|model\.qformer\.|model\.query_tokens|model\.vision_model\.)model\.": "model.llama.",
         "^lm_head.": "model.llama.",
     }
 
     def __init__(
         self,
         blip2_config_path: str,
         llama_config_path: str,
```

### Comparing `unitorch-0.0.0.5/src/unitorch/models/minigpt4/processing.py` & `unitorch-0.0.0.6/src/unitorch/models/minigpt4/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/modeling_ema.py` & `unitorch-0.0.0.6/src/unitorch/models/modeling_ema.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/mt5/modeling.py` & `unitorch-0.0.0.6/src/unitorch/models/mt5/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/mt5/processing.py` & `unitorch-0.0.0.6/src/unitorch/models/mt5/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/peft/__init__.py` & `unitorch-0.0.0.6/src/unitorch/models/peft/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/peft/modeling_bloom_adalora.py` & `unitorch-0.0.0.6/src/unitorch/models/peft/modeling_bloom_adalora.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/peft/modeling_bloom_lora.py` & `unitorch-0.0.0.6/src/unitorch/models/peft/modeling_bloom_lora.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/peft/modeling_llama_adalora.py` & `unitorch-0.0.0.6/src/unitorch/models/peft/modeling_llama_adalora.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/peft/modeling_llama_lora.py` & `unitorch-0.0.0.6/src/unitorch/models/peft/modeling_llama_lora.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/pegasus/modeling.py` & `unitorch-0.0.0.6/src/unitorch/models/pegasus/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/pegasus/processing.py` & `unitorch-0.0.0.6/src/unitorch/models/pegasus/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/processing_utils.py` & `unitorch-0.0.0.6/src/unitorch/models/processing_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/prophetnet/modeling.py` & `unitorch-0.0.0.6/src/unitorch/models/prophetnet/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/prophetnet/processing.py` & `unitorch-0.0.0.6/src/unitorch/models/prophetnet/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/roberta/modeling.py` & `unitorch-0.0.0.6/src/unitorch/models/roberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/roberta/processing.py` & `unitorch-0.0.0.6/src/unitorch/models/roberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/swin/modeling.py` & `unitorch-0.0.0.6/src/unitorch/models/swin/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/swin/processing.py` & `unitorch-0.0.0.6/src/unitorch/models/swin/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/t5/modeling.py` & `unitorch-0.0.0.6/src/unitorch/models/t5/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/t5/processing.py` & `unitorch-0.0.0.6/src/unitorch/models/t5/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/visualbert/modeling.py` & `unitorch-0.0.0.6/src/unitorch/models/visualbert/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/visualbert/processing.py` & `unitorch-0.0.0.6/src/unitorch/models/visualbert/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/vit/modeling.py` & `unitorch-0.0.0.6/src/unitorch/models/vit/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/vit/processing.py` & `unitorch-0.0.0.6/src/unitorch/models/vit/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/xlm_roberta/modeling.py` & `unitorch-0.0.0.6/src/unitorch/models/xlm_roberta/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/xlm_roberta/processing.py` & `unitorch-0.0.0.6/src/unitorch/models/xlm_roberta/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/xpegasus/modeling.py` & `unitorch-0.0.0.6/src/unitorch/models/xpegasus/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/xpegasus/processing.py` & `unitorch-0.0.0.6/src/unitorch/models/xpegasus/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/xprophetnet/modeling.py` & `unitorch-0.0.0.6/src/unitorch/models/xprophetnet/modeling.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/models/xprophetnet/processing.py` & `unitorch-0.0.0.6/src/unitorch/models/xprophetnet/processing.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/modules/classifier.py` & `unitorch-0.0.0.6/src/unitorch/modules/classifier.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/modules/replace/beam_search_v2.py` & `unitorch-0.0.0.6/src/unitorch/modules/replace/beam_search_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/modules/replace/datasets_v2.py` & `unitorch-0.0.0.6/src/unitorch/modules/replace/datasets_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/modules/replace/hf_hub_v2.py` & `unitorch-0.0.0.6/src/unitorch/modules/replace/hf_hub_v2.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/modules/timm.py` & `unitorch-0.0.0.6/src/unitorch/modules/timm.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/ops/dyhead.py` & `unitorch-0.0.0.6/src/unitorch/ops/dyhead.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/ops/ngram_repeat_block.py` & `unitorch-0.0.0.6/src/unitorch/ops/ngram_repeat_block.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/optim/lion.py` & `unitorch-0.0.0.6/src/unitorch/optim/lion.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/scheduler/warmup.py` & `unitorch-0.0.0.6/src/unitorch/scheduler/warmup.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/score/__init__.py` & `unitorch-0.0.0.6/src/unitorch/score/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/score/bleu.py` & `unitorch-0.0.0.6/src/unitorch/score/bleu.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/score/map.py` & `unitorch-0.0.0.6/src/unitorch/score/map.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/score/rouge.py` & `unitorch-0.0.0.6/src/unitorch/score/rouge.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/utils/__init__.py` & `unitorch-0.0.0.6/src/unitorch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/utils/decorators.py` & `unitorch-0.0.0.6/src/unitorch/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/utils/functional.py` & `unitorch-0.0.0.6/src/unitorch/utils/functional.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/utils/image_utils.py` & `unitorch-0.0.0.6/src/unitorch/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/utils/import_utils.py` & `unitorch-0.0.0.6/src/unitorch/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/utils/io.py` & `unitorch-0.0.0.6/src/unitorch/utils/io.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/utils/palette.py` & `unitorch-0.0.0.6/src/unitorch/utils/palette.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch/utils/torch_utils.py` & `unitorch-0.0.0.6/src/unitorch/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/src/unitorch.egg-info/PKG-INFO` & `unitorch-0.0.0.6/src/unitorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitorch
-Version: 0.0.0.5
+Version: 0.0.0.6
 Summary: unitorch provides efficient implementation of popular unified NLU / NLG / CV / CTR / MM / RL models with PyTorch.
 Author-email: fuliucansheng <fuliucansheng@gmail.com>
 License: MIT
 Keywords: PyTorch
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -18,15 +18,14 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: deepspeed
 Provides-Extra: diffusers
 Provides-Extra: accelerate
 Provides-Extra: chatglm
-Provides-Extra: fastapi
 Provides-Extra: all
 License-File: LICENSE
 
 <div align="Center"> 
 
 ![unitorch](unitorch.png)
```

### Comparing `unitorch-0.0.0.5/src/unitorch.egg-info/SOURCES.txt` & `unitorch-0.0.0.6/src/unitorch.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 src/unitorch.egg-info/requires.txt
 src/unitorch.egg-info/top_level.txt
 src/unitorch/cli/__init__.py
 src/unitorch/cli/core.py
 src/unitorch/cli/decorators.py
 src/unitorch/cli/console/__init__.py
 src/unitorch/cli/console/eval.py
-src/unitorch/cli/console/fastapi.py
 src/unitorch/cli/console/infer.py
 src/unitorch/cli/console/script.py
 src/unitorch/cli/console/service.py
 src/unitorch/cli/console/train.py
 src/unitorch/cli/datasets/__init__.py
 src/unitorch/cli/datasets/hf.py
 src/unitorch/cli/loss/__init__.py
```

### Comparing `unitorch-0.0.0.5/wiki/cli/models/blip.md` & `unitorch-0.0.0.6/wiki/cli/models/blip.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/wiki/cli/models/bloom.md` & `unitorch-0.0.0.6/wiki/cli/models/bloom.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/wiki/cli/models/chatglm.md` & `unitorch-0.0.0.6/wiki/cli/models/chatglm.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/wiki/cli/models/clip.md` & `unitorch-0.0.0.6/wiki/cli/models/clip.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/wiki/cli/models/deberta.md` & `unitorch-0.0.0.6/wiki/cli/models/deberta.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/wiki/cli/models/llama.md` & `unitorch-0.0.0.6/wiki/cli/models/llama.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/wiki/cli/models/peft.md` & `unitorch-0.0.0.6/wiki/cli/models/peft.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/wiki/cli/models/visualbert.md` & `unitorch-0.0.0.6/wiki/cli/models/visualbert.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/wiki/cli/models/xlm_roberta.md` & `unitorch-0.0.0.6/wiki/cli/models/xlm_roberta.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/wiki/cli/postprocess.md` & `unitorch-0.0.0.6/wiki/cli/postprocess.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/wiki/configuration.md` & `unitorch-0.0.0.6/wiki/configuration.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/wiki/examples/caption/blip.md` & `unitorch-0.0.0.6/wiki/examples/caption/blip.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/wiki/examples/classification/clip.md` & `unitorch-0.0.0.6/wiki/examples/classification/clip.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/wiki/examples/classification/roberta.md` & `unitorch-0.0.0.6/wiki/examples/classification/roberta.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/wiki/examples/classification/swin.md` & `unitorch-0.0.0.6/wiki/examples/classification/swin.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/wiki/examples/generation/bart.md` & `unitorch-0.0.0.6/wiki/examples/generation/bart.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/wiki/examples/service/zip_image.md` & `unitorch-0.0.0.6/wiki/examples/service/zip_image.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/wiki/index.md` & `unitorch-0.0.0.6/wiki/index.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/wiki/installation.md` & `unitorch-0.0.0.6/wiki/installation.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/wiki/models/peft.md` & `unitorch-0.0.0.6/wiki/models/peft.md`

 * *Files identical despite different names*

### Comparing `unitorch-0.0.0.5/wiki/overview.md` & `unitorch-0.0.0.6/wiki/overview.md`

 * *Files identical despite different names*


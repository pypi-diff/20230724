# Comparing `tmp/jax-md-0.2.5.tar.gz` & `tmp/jax-md-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jax-md-0.2.5.tar", last modified: Mon Nov 28 16:12:49 2022, max compression
+gzip compressed data, was "jax-md-0.2.6.tar", last modified: Mon Jul 24 14:35:23 2023, max compression
```

## Comparing `jax-md-0.2.5.tar` & `jax-md-0.2.6.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxr-xr-x   0 schsam   (393895) wheel        (0)        0 2022-11-28 16:12:49.246585 jax-md-0.2.5/
--rw-r--r--   0 schsam   (393895) wheel        (0)    20945 2022-11-28 16:12:49.246894 jax-md-0.2.5/PKG-INFO
--rw-r--r--   0 schsam   (393895) wheel        (0)    18222 2022-11-28 16:12:45.000000 jax-md-0.2.5/README.md
-drwxr-xr-x   0 schsam   (393895) wheel        (0)        0 2022-11-28 16:12:49.240622 jax-md-0.2.5/jax_md/
--rw-r--r--   0 schsam   (393895) wheel        (0)     1037 2022-11-28 16:12:45.000000 jax-md-0.2.5/jax_md/__init__.py
-drwxr-xr-x   0 schsam   (393895) wheel        (0)        0 2022-11-28 16:12:49.245309 jax-md-0.2.5/jax_md/_nn/
--rw-r--r--   0 schsam   (393895) wheel        (0)      667 2022-11-28 16:12:45.000000 jax-md-0.2.5/jax_md/_nn/__init__.py
--rw-r--r--   0 schsam   (393895) wheel        (0)    19618 2022-11-28 16:12:45.000000 jax-md-0.2.5/jax_md/_nn/behler_parrinello.py
--rw-r--r--   0 schsam   (393895) wheel        (0)    15108 2022-11-28 16:12:45.000000 jax-md-0.2.5/jax_md/_nn/e3nn_layer.py
--rw-r--r--   0 schsam   (393895) wheel        (0)     5592 2022-11-28 16:12:45.000000 jax-md-0.2.5/jax_md/_nn/gnome.py
--rw-r--r--   0 schsam   (393895) wheel        (0)    31945 2022-11-28 16:12:45.000000 jax-md-0.2.5/jax_md/_nn/nequip.py
--rw-r--r--   0 schsam   (393895) wheel        (0)     4914 2022-11-28 16:12:45.000000 jax-md-0.2.5/jax_md/_nn/util.py
-drwxr-xr-x   0 schsam   (393895) wheel        (0)        0 2022-11-28 16:12:49.246209 jax-md-0.2.5/jax_md/colab_tools/
--rw-r--r--   0 schsam   (393895) wheel        (0)      615 2022-11-28 16:12:45.000000 jax-md-0.2.5/jax_md/colab_tools/__init__.py
--rw-r--r--   0 schsam   (393895) wheel        (0)     9876 2022-11-28 16:12:45.000000 jax-md-0.2.5/jax_md/colab_tools/renderer.py
--rw-r--r--   0 schsam   (393895) wheel        (0)     2500 2022-11-28 16:12:45.000000 jax-md-0.2.5/jax_md/dataclasses.py
--rw-r--r--   0 schsam   (393895) wheel        (0)    23043 2022-11-28 16:12:45.000000 jax-md-0.2.5/jax_md/elasticity.py
--rw-r--r--   0 schsam   (393895) wheel        (0)    69154 2022-11-28 16:12:45.000000 jax-md-0.2.5/jax_md/energy.py
--rw-r--r--   0 schsam   (393895) wheel        (0)     2962 2022-11-28 16:12:45.000000 jax-md-0.2.5/jax_md/interpolate.py
--rw-r--r--   0 schsam   (393895) wheel        (0)     1367 2022-11-28 16:12:45.000000 jax-md-0.2.5/jax_md/io.py
--rw-r--r--   0 schsam   (393895) wheel        (0)     8067 2022-11-28 16:12:45.000000 jax-md-0.2.5/jax_md/minimize.py
--rw-r--r--   0 schsam   (393895) wheel        (0)    10567 2022-11-28 16:12:45.000000 jax-md-0.2.5/jax_md/nn.py
--rw-r--r--   0 schsam   (393895) wheel        (0)    41382 2022-11-28 16:12:45.000000 jax-md-0.2.5/jax_md/partition.py
--rw-r--r--   0 schsam   (393895) wheel        (0)    25680 2022-11-28 16:12:45.000000 jax-md-0.2.5/jax_md/quantity.py
--rw-r--r--   0 schsam   (393895) wheel        (0)    39839 2022-11-28 16:12:45.000000 jax-md-0.2.5/jax_md/rigid_body.py
--rw-r--r--   0 schsam   (393895) wheel        (0)    47018 2022-11-28 16:12:45.000000 jax-md-0.2.5/jax_md/simulate.py
--rw-r--r--   0 schsam   (393895) wheel        (0)    36532 2022-11-28 16:12:45.000000 jax-md-0.2.5/jax_md/smap.py
--rw-r--r--   0 schsam   (393895) wheel        (0)    16456 2022-11-28 16:12:45.000000 jax-md-0.2.5/jax_md/space.py
--rw-r--r--   0 schsam   (393895) wheel        (0)    11874 2022-11-28 16:12:45.000000 jax-md-0.2.5/jax_md/test_util.py
--rw-r--r--   0 schsam   (393895) wheel        (0)    58915 2022-11-28 16:12:45.000000 jax-md-0.2.5/jax_md/tpu.py
--rw-r--r--   0 schsam   (393895) wheel        (0)     2838 2022-11-28 16:12:45.000000 jax-md-0.2.5/jax_md/util.py
-drwxr-xr-x   0 schsam   (393895) wheel        (0)        0 2022-11-28 16:12:49.242711 jax-md-0.2.5/jax_md.egg-info/
--rw-r--r--   0 schsam   (393895) wheel        (0)    20945 2022-11-28 16:12:49.000000 jax-md-0.2.5/jax_md.egg-info/PKG-INFO
--rw-r--r--   0 schsam   (393895) wheel        (0)      684 2022-11-28 16:12:49.000000 jax-md-0.2.5/jax_md.egg-info/SOURCES.txt
--rw-r--r--   0 schsam   (393895) wheel        (0)        1 2022-11-28 16:12:49.000000 jax-md-0.2.5/jax_md.egg-info/dependency_links.txt
--rw-r--r--   0 schsam   (393895) wheel        (0)       94 2022-11-28 16:12:49.000000 jax-md-0.2.5/jax_md.egg-info/requires.txt
--rw-r--r--   0 schsam   (393895) wheel        (0)        7 2022-11-28 16:12:49.000000 jax-md-0.2.5/jax_md.egg-info/top_level.txt
--rw-r--r--   0 schsam   (393895) wheel        (0)      113 2022-11-28 16:12:49.247492 jax-md-0.2.5/setup.cfg
--rw-r--r--   0 schsam   (393895) wheel        (0)     2314 2022-11-28 16:12:45.000000 jax-md-0.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:35:23.346403 jax-md-0.2.6/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-07-20 17:59:08.000000 jax-md-0.2.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      574 2023-07-20 17:59:08.000000 jax-md-0.2.6/LICENSE_SHORT
+-rw-r--r--   0 root         (0) root         (0)    19228 2023-07-24 14:35:23.346403 jax-md-0.2.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    18222 2023-07-20 17:59:08.000000 jax-md-0.2.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:35:23.346403 jax-md-0.2.6/jax_md/
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:35:23.346403 jax-md-0.2.6/jax_md/_nn/
+-rw-r--r--   0 root         (0) root         (0)      667 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/_nn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19618 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/_nn/behler_parrinello.py
+-rw-r--r--   0 root         (0) root         (0)    15104 2023-07-24 14:23:56.000000 jax-md-0.2.6/jax_md/_nn/e3nn_layer.py
+-rw-r--r--   0 root         (0) root         (0)     5268 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/_nn/gnome.py
+-rw-r--r--   0 root         (0) root         (0)    15885 2023-07-24 14:23:56.000000 jax-md-0.2.6/jax_md/_nn/nequip.py
+-rw-r--r--   0 root         (0) root         (0)     4701 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/_nn/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:35:23.346403 jax-md-0.2.6/jax_md/colab_tools/
+-rw-r--r--   0 root         (0) root         (0)      615 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/colab_tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9876 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/colab_tools/renderer.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-07-24 14:23:51.000000 jax-md-0.2.6/jax_md/dataclasses.py
+-rw-r--r--   0 root         (0) root         (0)    23043 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/elasticity.py
+-rw-r--r--   0 root         (0) root         (0)    77180 2023-07-24 14:23:51.000000 jax-md-0.2.6/jax_md/energy.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/interpolate.py
+-rw-r--r--   0 root         (0) root         (0)     1367 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/io.py
+-rw-r--r--   0 root         (0) root         (0)     8067 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/minimize.py
+-rw-r--r--   0 root         (0) root         (0)    10567 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/nn.py
+-rw-r--r--   0 root         (0) root         (0)    41487 2023-07-24 14:23:56.000000 jax-md-0.2.6/jax_md/partition.py
+-rw-r--r--   0 root         (0) root         (0)    25660 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/quantity.py
+-rw-r--r--   0 root         (0) root         (0)    39882 2023-07-24 14:23:51.000000 jax-md-0.2.6/jax_md/rigid_body.py
+-rw-r--r--   0 root         (0) root         (0)    47018 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/simulate.py
+-rw-r--r--   0 root         (0) root         (0)    36532 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/smap.py
+-rw-r--r--   0 root         (0) root         (0)    16456 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/space.py
+-rw-r--r--   0 root         (0) root         (0)    11874 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/test_util.py
+-rw-r--r--   0 root         (0) root         (0)    58774 2023-07-24 14:23:56.000000 jax-md-0.2.6/jax_md/tpu.py
+-rw-r--r--   0 root         (0) root         (0)     4160 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/units.py
+-rw-r--r--   0 root         (0) root         (0)     2838 2023-07-20 17:59:08.000000 jax-md-0.2.6/jax_md/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:35:23.346403 jax-md-0.2.6/jax_md.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    19228 2023-07-24 14:35:23.000000 jax-md-0.2.6/jax_md.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      722 2023-07-24 14:35:23.000000 jax-md-0.2.6/jax_md.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 14:35:23.000000 jax-md-0.2.6/jax_md.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       94 2023-07-24 14:35:23.000000 jax-md-0.2.6/jax_md.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-24 14:35:23.000000 jax-md-0.2.6/jax_md.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      113 2023-07-24 14:35:23.346403 jax-md-0.2.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2314 2023-07-24 14:33:31.000000 jax-md-0.2.6/setup.py
```

### Comparing `jax-md-0.2.5/PKG-INFO` & `jax-md-0.2.6/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,242 +1,217 @@
-Metadata-Version: 2.1
-Name: jax-md
-Version: 0.2.5
-Summary: Differentiable, Hardware Accelerated, Molecular Dynamics
-Home-page: https://github.com/google/jax-md
-Author: Google
-Author-email: jax-md-dev@google.com
-License: Apache 2.0
-Download-URL: https://pypi.org/project/jax-md/
-Project-URL: Source Code, https://github.com/google/jax-md
-Project-URL: Documentation, https://arxiv.org/abs/1912.04232
-Project-URL: Bug Tracker, https://github.com/google/jax-md/issues
-Description: # JAX, M.D.
-        
-        ### Accelerated, Differentiable, Molecular Dynamics
-        [**Quickstart**](#getting-started) | [**Reference docs**](https://jax-md.readthedocs.io/en/main/) | [**Paper**](https://arxiv.org/pdf/1912.04232.pdf) | [**NeurIPS 2020**](https://neurips.cc/virtual/2020/public/poster_83d3d4b6c9579515e1679aca8cbc8033.html)
-        
-        ![Build Status](https://github.com/google/jax-md/workflows/Build/badge.svg?branch=main) [![Coverage](https://codecov.io/gh/google/jax-md/branch/main/graph/badge.svg?token=JYQpbNyICv)](https://codecov.io/gh/google/jax-md) [![PyPI](https://img.shields.io/pypi/v/jax-md)](https://pypi.org/project/jax-md/) [![PyPI - License](https://img.shields.io/pypi/l/jax_md)](https://github.com/google/jax-md/blob/main/LICENSE)
-        
-        Molecular dynamics is a workhorse of modern computational condensed matter physics. It is frequently used to simulate materials to observe how small scale interactions can give rise to complex large-scale phenomenology. Most molecular dynamics packages (e.g. HOOMD Blue or LAMMPS) are complicated, specialized pieces of code that are many thousands of lines long. They typically involve significant code duplication to allow for running simulations on CPU and GPU. Additionally, large amounts of code is often devoted to taking derivatives of quantities to compute functions of interest (e.g. gradients of energies to compute forces).
-        
-        However, recent work in machine learning has led to significant software developments that might make it possible to write more concise molecular dynamics simulations that offer a range of benefits. Here we target JAX, which allows us to write python code that gets compiled to XLA and allows us to run on CPU, GPU, or TPU. Moreover, JAX allows us to take derivatives of python code. Thus, not only is this molecular dynamics simulation automatically hardware accelerated, it is also __end-to-end__ differentiable. This should allow for some interesting experiments that we're excited to explore.
-        
-        JAX, MD is a research project that is currently under development. Expect sharp edges and possibly some API breaking changes as we continue to support a broader set of simulations. JAX MD is a functional and data driven library. Data is stored in arrays or tuples of arrays and functions transform data from one state to another.
-        
-        ### Getting Started
-        
-        For a video introducing JAX MD along with a [demo](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/talk_demo.ipynb), check out this talk from the Physics meets Machine Learning series:
-        
-        [![Science Meets ML Talk](https://img.youtube.com/vi/Bkm8tGET7-w/0.jpg)](https://www.youtube.com/watch?v=Bkm8tGET7-w)
-        
-        To get started playing around with JAX MD check out the following colab notebooks on Google Cloud without needing to install anything. For a very simple introduction, I would recommend the Minimization example. For an example of a bunch of the features of JAX MD, check out the JAX MD cookbook.
-        
-        - [JAX MD Cookbook](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/jax_md_cookbook.ipynb)
-        - [Minimization](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/minimization.ipynb)
-        - [NVE Simulation](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/nve_simulation.ipynb)
-        - [NVT Simulation](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/nvt_simulation.ipynb)
-        - [NPT Simulation](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/npt_simulation.ipynb)
-        - [NVE with Neighbor Lists](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/nve_neighbor_list.ipynb)
-        - [Custom Potentials](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/customizing_potentials_cookbook.ipynb)
-        - [Neural Network Potentials](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/neural_networks.ipynb)
-        - [Flocking](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/flocking.ipynb)
-        - [Meta Optimization](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/meta_optimization.ipynb)
-        - [Swap Monte Carlo (Cargese Summer School)](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/cargese_swap_mc.ipynb)
-        - [Implicit Differentiation](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/implicit_differentiation.ipynb)
-        - [Athermal Linear Elasticity](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/athermal_linear_elasticity.ipynb)
-        - [Smash a Sand Castle](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/sand_castle.ipynb)
-        
-        You can install JAX MD locally with pip,
-        ```
-        pip install jax-md --upgrade
-        ```
-        If you want to build the latest version then you can grab the most recent version from head,
-        ```
-        git clone https://github.com/google/jax-md
-        pip install -e jax-md
-        ```
-        
-        # Overview
-        
-        We now summarize the main components of the library.
-        
-        ## Spaces ([`space.py`](https://jax-md.readthedocs.io/en/main/jax_md.space.html))
-        
-        In general we must have a way of computing the pairwise distance between atoms. We must also have efficient strategies for moving atoms in some space that may or may not be globally isomorphic to R^N. For example, periodic boundary conditions are commonplace in simulations and must be respected. Spaces are defined as a pair of functions, `(displacement_fn, shift_fn)`. Given two points `displacement_fn(R_1, R_2)` computes the displacement vector between the two points. If you would like to compute displacement vectors between all pairs of points in a given `(N, dim)` matrix the function `space.map_product` appropriately vectorizes `displacement_fn`. It is often useful to define a metric instead of a displacement function in which case you can use the helper function `space.metric` to convert a displacement function to a metric function. Given a point and a shift `shift_fn(R, dR)` displaces the point `R` by an amount `dR`.
-        
-        The following spaces are currently supported:
-        - [`space.free()`](https://jax-md.readthedocs.io/en/main/jax_md.space.html?highlight=free#jax_md.space.free) specifies a space with free boundary conditions.
-        - [`space.periodic(box_size)`](https://jax-md.readthedocs.io/en/main/jax_md.space.html?highlight=periodic#jax_md.space.periodic) specifies a space with periodic boundary conditions of side length `box_size`.
-        - [`space.periodic_general(box)`](https://jax-md.readthedocs.io/en/main/jax_md.space.html?highlight=periodic_general#jax_md.space.periodic_general) specifies a space as a periodic parellelopiped formed by transforming the unit cube by an affine transformation `box`.
-        
-        Example:
-        
-        ```python
-        from jax_md import space
-        box_size = 25.0
-        displacement_fn, shift_fn = space.periodic(box_size)
-        ```
-        
-        ## Potential Energy ([`energy.py`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html))
-        
-        In the simplest case, molecular dynamics calculations are often based on a pair potential that is defined by a user. This then is used to compute a total energy whose negative gradient gives forces. One of the very nice things about JAX is that we get forces for free! The second part of the code is devoted to computing energies.
-        
-        We provide the following classical potentials:
-        - [`energy.soft_sphere`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=soft_sphere#jax_md.energy.soft_sphere) a soft sphere whose energy increases as the overlap of the spheres to some power, `alpha`.
-        - [`energy.lennard_jones`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=lennard_jones#jax_md.energy.lennard_jones) a standard 12-6 Lennard-Jones potential.
-        - [`energy.morse`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=morse#jax_md.energy.morse) a morse potential.
-        - [`energy.tersoff`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=tersoff#jax_md.energy.tersoff) the Tersoff potential for simulating semiconducting materials. Can load parameters from LAMMPS files.
-        - [`energy.eam`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=eam#jax_md.energy.eam) embedded atom model potential with ability to load parameters from LAMMPS files.
-        - [`energy.stillinger_weber`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=stillinger_weber#jax_md.energy.stillinger_weber) used to model Silicon-like systems.
-        - [`energy.bks`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=bks#jax_md.energy.bks) Beest-Kramer-van Santen potential used to model silica.
-        - [`energy.gupta`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=gupta#jax_md.energy.gupta) used to model gold nanoclusters.
-        
-        We also provide the following neural network potentials:
-        - [`energy.behler_parrinello`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=behler_parrinello#jax_md.energy.behler_parrinello) a widely used fixed-feature neural network architecture for molecular systems.
-        - [`energy.graph_network`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=graph_network#jax_md.energy.graph_network) a deep graph neural network designed for energy fitting.
-        
-        For finite-ranged potentials it is often useful to consider only interactions within a certain neighborhood. We include the `_neighbor_list` modifier to the above potentials that uses a list of neighbors (see below) for optimization.
-        
-        Example:
-        
-        ```python
-        import jax.numpy as np
-        from jax import random
-        from jax_md import energy, quantity
-        N = 1000
-        spatial_dimension = 2
-        key = random.PRNGKey(0)
-        R = random.uniform(key, (N, spatial_dimension), minval=0.0, maxval=1.0)
-        energy_fn = energy.lennard_jones_pair(displacement_fn)
-        print('E = {}'.format(energy_fn(R)))
-        force_fn = quantity.force(energy_fn)
-        print('Total Squared Force = {}'.format(np.sum(force_fn(R) ** 2)))
-        ```
-        
-        ## Dynamics ([`simulate.py`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html), [`minimize.py`](https://jax-md.readthedocs.io/en/main/jax_md.minimize.html))
-        
-        Given an energy function and a system, there are a number of dynamics are useful to simulate. The simulation code is based on the structure of the optimizers found in JAX. In particular, each simulation function returns an initialization function and an update function. The initialization function takes a set of positions and creates the necessary dynamical state variables. The update function does a single step of dynamics to the dynamical state variables and returns an updated state.
-        
-        We include a several different kinds of dynamics. However, there is certainly room to add more for e.g. constant strain simulations.
-        
-        It is often desirable to find an energy minimum of the system. We provide two methods to do this. We provide simple gradient descent minimization. This is mostly for pedagogical purposes, since it often performs poorly. We additionally include the FIRE algorithm which often sees significantly faster convergence. Moreover a common experiment to run in the context of molecular dynamics is to simulate a system with a fixed volume and temperature.
-        
-        We provide the following dynamics:
-        - [`simulate.nve`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html?highlight=nve#jax_md.simulate.nve) Constant energy simulation; numerically integrates Newton's laws directly.
-        - [`simulate.nvt_nose_hoover`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html?highlight=nvt_nose_hoover#jax_md.simulate.nvt_nose_hoover) Uses Nose-Hoover chain to simulate a constant temperature system.
-        - [`simulate.npt_nose_hoover`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html?highlight=nvp_nose_hoover#jax_md.simulate.nvp_nose_hoover) Uses Nose-Hoover chain to simulate a system at constant pressure and temperature.
-        - [`simulate.nvt_langevin`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html?highlight=nvt_langevin#jax_md.simulate.nvt_langevin) Simulates a system by numerically integrating the Langevin stochastic differential equation.
-        - [`simulate.hybrid_swap_mc`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html?highlight=hybrid_swap_mc#jax_md.simulate.hybrid_swap_mc) Alternates NVT dynamics with Monte-Carlo swapping moves to generate low energy glasses.
-        - [`simulate.brownian`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html?highlight=brownian#jax_md.simulate.brownian) Simulates brownian motion.
-        - [`minimize.gradient_descent`](https://jax-md.readthedocs.io/en/main/jax_md.minimize.html?highlight=gradient_descent#jax_md.minimize.gradient_descent) Minimizes a system using gradient descent.
-        - [`minimize.fire_descent`](https://jax-md.readthedocs.io/en/main/jax_md.minimize.html?highlight=fire_descent#jax_md.minimize.fire_descent) Minimizes a system using the fast inertial relaxation engine.
-        
-        Example:
-        
-        ```python
-        from jax_md import simulate
-        temperature = 1.0
-        dt = 1e-3
-        init, update = simulate.nvt_nose_hoover(energy_fn, shift_fn, dt, temperature)
-        state = init(key, R)
-        for _ in range(100):
-          state = update(state)
-        R = state.position
-        ```
-        
-        ## Spatial Partitioning ([`partition.py`](https://jax-md.readthedocs.io/en/main/jax_md.partition.html))
-        
-        In many applications, it is useful to construct spatial partitions of particles / objects in a simulation.
-        
-        We provide the following methods:
-        - [`partition.cell_list`](https://jax-md.readthedocs.io/en/main/jax_md.partition.html?highlight=cell_list#jax_md.partition.cell_list) Partitions objects (and metadata) into a grid of cells.
-        - [`partition.neighbor_list`](https://jax-md.readthedocs.io/en/main/jax_md.partition.html?highlight=neighbor_list#jax_md.partition.neighbor_list) Constructs a set of neighbors within some cutoff distance for each object in a simulation.
-        
-        Cell List Example:
-        ```python
-        from jax_md import partition
-        
-        cell_size = 5.0
-        capacity = 10
-        cell_list_fn = partition.cell_list(box_size, cell_size, capacity)
-        cell_list_data = cell_list_fn(R)
-        ```
-        
-        Neighbor List Example:
-        ```python
-        from jax_md import partition
-        
-        neighbor_list_fn = partition.neighbor_list(displacement_fn, box_size, cell_size)
-        neighbors = neighbor_list_fn.allocate(R) # Create a new neighbor list.
-        
-        # Do some simulating....
-        
-        neighbors = neighbors.update(R)  # Update the neighbor list without resizing.
-        if neighbors.did_buffer_overflow:  # Couldn't fit all the neighbors into the list.
-          neighbors = neighbor_list_fn.allocate(R)  # So create a new neighbor list.
-        ```
-        
-        There are three different formats of neighbor list supported: `Dense`, `Sparse`, and `OrderedSparse`. `Dense` neighbor lists store neighbors in an `(particle_count, neighbors_per_particle)` array, `Sparse` neighbor lists store neighbors in a `(2, total_neighbors)` array of pairs, `OrderedSparse` neighbor lists are like `Sparse` neighbor lists, but they only store pairs such that `i < j`.
-        
-        # Development
-        
-        JAX MD is under active development. We have very limited development resources and so we typically focus on adding features that will have high impact to researchers using JAX MD (including us). Please don't hesitate to open feature requests to help us guide development. We more than welcome contributions!
-        
-        ## Technical gotchas
-        
-        ### GPU
-        
-        You must follow [JAX's](https://www.github.com/google/jax/) GPU installation instructions to enable GPU support.
-        
-        
-        ### 64-bit precision
-        To enable 64-bit precision, set the respective JAX flag _before_ importing `jax_md` (see the JAX [guide](https://colab.research.google.com/github/google/jax/blob/main/notebooks/Common_Gotchas_in_JAX.ipynb#scrollTo=YTktlwTTMgFl)), for example:
-        
-        ```python
-        from jax.config import config
-        config.update("jax_enable_x64", True)
-        ```
-        
-        # Publications
-        
-        JAX MD has been used in the following publications. If you don't see your paper on the list, but you used JAX MD let us know and we'll add it to the list!
-        
-        1. [A Differentiable Neural-Network Force Field for Ionic Liquids. (J. Chem. Inf. Model. 2022)](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.1c01380)<br> H. Montes-Campos, J. Carrete, S. Bichelmaier, L. M. Varela, and G. K. H. Madsen
-        2. [Correlation Tracking: Using simulations to interpolate highly correlated particle tracks. (Phys. Rev. E. 2022)](https://journals.aps.org/pre/abstract/10.1103/PhysRevE.105.044608?ft=1)<br> E. M. King, Z. Wang, D. A. Weitz, F. Spaepen, and M. P. Brenner
-        3. [Optimal Control of Nonequilibrium Systems Through Automatic Differentiation.](https://arxiv.org/abs/2201.00098)<br> M. C. Engel, J. A. Smith, and M. P. Brenner
-        4. [Graph Neural Networks Accelerated Molecular Dynamics. (J. Chem. Phys. 2022)](https://aip.scitation.org/doi/10.1063/5.0083060)<br> Z. Li, K. Meidani, P. Yadav, and A. B. Farimani
-        5. [Gradients are Not All You Need.](https://arxiv.org/abs/2111.05803)<br> L. Metz, C. D. Freeman, S. S. Schoenholz, and T. Kachman
-        6. [Lagrangian Neural Network with Differential Symmetries and Relational Inductive Bias.](https://arxiv.org/abs/2110.03266)<br> R. Bhattoo, S. Ranu, and N. M. A. Krishnan
-        7. [Efficient and Modular Implicit Differentiation.](https://arxiv.org/abs/2105.15183)<br> M. Blondel, Q. Berthet, M. Cuturi, R. Frostig, S. Hoyer, F. Llinares-López, F. Pedregosa, and J.-P. Vert
-        8. [Learning neural network potentials from experimental data via Differentiable Trajectory Reweighting.<br>(Nature Communications 2021)](https://www.nature.com/articles/s41467-021-27241-4)<br> S. Thaler and J. Zavadlav
-        9. [Learn2Hop: Learned Optimization on Rough Landscapes. (ICML 2021)](http://proceedings.mlr.press/v139/merchant21a.html)<br> A. Merchant, L. Metz, S. S. Schoenholz, and E. D. Cubuk
-        10. [Designing self-assembling kinetics with differentiable statistical physics models. (PNAS 2021)](https://www.pnas.org/content/118/10/e2024083118.short)<br> C. P. Goodrich, E. M. King, S. S. Schoenholz, E. D. Cubuk, and  M. P. Brenner
-        
-        # Citation
-        
-        If you use the code in a publication, please cite the repo using the .bib,
-        
-        ```
-        @inproceedings{jaxmd2020,
-         author = {Schoenholz, Samuel S. and Cubuk, Ekin D.},
-         booktitle = {Advances in Neural Information Processing Systems},
-         publisher = {Curran Associates, Inc.},
-         title = {JAX M.D. A Framework for Differentiable Physics},
-         url = {https://papers.nips.cc/paper/2020/file/83d3d4b6c9579515e1679aca8cbc8033-Paper.pdf},
-         volume = {33},
-         year = {2020}
-        }
-        ```
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Topic :: Software Development
-Classifier: Topic :: Scientific/Engineering
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Requires-Python: >=2.7
-Description-Content-Type: text/markdown
+# JAX, M.D.
+
+### Accelerated, Differentiable, Molecular Dynamics
+[**Quickstart**](#getting-started) | [**Reference docs**](https://jax-md.readthedocs.io/en/main/) | [**Paper**](https://arxiv.org/pdf/1912.04232.pdf) | [**NeurIPS 2020**](https://neurips.cc/virtual/2020/public/poster_83d3d4b6c9579515e1679aca8cbc8033.html)
+
+![Build Status](https://github.com/google/jax-md/workflows/Build/badge.svg?branch=main) [![Coverage](https://codecov.io/gh/google/jax-md/branch/main/graph/badge.svg?token=JYQpbNyICv)](https://codecov.io/gh/google/jax-md) [![PyPI](https://img.shields.io/pypi/v/jax-md)](https://pypi.org/project/jax-md/) [![PyPI - License](https://img.shields.io/pypi/l/jax_md)](https://github.com/google/jax-md/blob/main/LICENSE)
+
+Molecular dynamics is a workhorse of modern computational condensed matter physics. It is frequently used to simulate materials to observe how small scale interactions can give rise to complex large-scale phenomenology. Most molecular dynamics packages (e.g. HOOMD Blue or LAMMPS) are complicated, specialized pieces of code that are many thousands of lines long. They typically involve significant code duplication to allow for running simulations on CPU and GPU. Additionally, large amounts of code is often devoted to taking derivatives of quantities to compute functions of interest (e.g. gradients of energies to compute forces).
+
+However, recent work in machine learning has led to significant software developments that might make it possible to write more concise molecular dynamics simulations that offer a range of benefits. Here we target JAX, which allows us to write python code that gets compiled to XLA and allows us to run on CPU, GPU, or TPU. Moreover, JAX allows us to take derivatives of python code. Thus, not only is this molecular dynamics simulation automatically hardware accelerated, it is also __end-to-end__ differentiable. This should allow for some interesting experiments that we're excited to explore.
+
+JAX, MD is a research project that is currently under development. Expect sharp edges and possibly some API breaking changes as we continue to support a broader set of simulations. JAX MD is a functional and data driven library. Data is stored in arrays or tuples of arrays and functions transform data from one state to another.
+
+### Getting Started
+
+For a video introducing JAX MD along with a [demo](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/talk_demo.ipynb), check out this talk from the Physics meets Machine Learning series:
+
+[![Science Meets ML Talk](https://img.youtube.com/vi/Bkm8tGET7-w/0.jpg)](https://www.youtube.com/watch?v=Bkm8tGET7-w)
+
+To get started playing around with JAX MD check out the following colab notebooks on Google Cloud without needing to install anything. For a very simple introduction, I would recommend the Minimization example. For an example of a bunch of the features of JAX MD, check out the JAX MD cookbook.
+
+- [JAX MD Cookbook](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/jax_md_cookbook.ipynb)
+- [Minimization](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/minimization.ipynb)
+- [NVE Simulation](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/nve_simulation.ipynb)
+- [NVT Simulation](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/nvt_simulation.ipynb)
+- [NPT Simulation](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/npt_simulation.ipynb)
+- [NVE with Neighbor Lists](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/nve_neighbor_list.ipynb)
+- [Custom Potentials](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/customizing_potentials_cookbook.ipynb)
+- [Neural Network Potentials](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/neural_networks.ipynb)
+- [Flocking](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/flocking.ipynb)
+- [Meta Optimization](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/meta_optimization.ipynb)
+- [Swap Monte Carlo (Cargese Summer School)](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/cargese_swap_mc.ipynb)
+- [Implicit Differentiation](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/implicit_differentiation.ipynb)
+- [Athermal Linear Elasticity](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/athermal_linear_elasticity.ipynb)
+- [Smash a Sand Castle](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/sand_castle.ipynb)
+
+You can install JAX MD locally with pip,
+```
+pip install jax-md --upgrade
+```
+If you want to build the latest version then you can grab the most recent version from head,
+```
+git clone https://github.com/google/jax-md
+pip install -e jax-md
+```
+
+# Overview
+
+We now summarize the main components of the library.
+
+## Spaces ([`space.py`](https://jax-md.readthedocs.io/en/main/jax_md.space.html))
+
+In general we must have a way of computing the pairwise distance between atoms. We must also have efficient strategies for moving atoms in some space that may or may not be globally isomorphic to R^N. For example, periodic boundary conditions are commonplace in simulations and must be respected. Spaces are defined as a pair of functions, `(displacement_fn, shift_fn)`. Given two points `displacement_fn(R_1, R_2)` computes the displacement vector between the two points. If you would like to compute displacement vectors between all pairs of points in a given `(N, dim)` matrix the function `space.map_product` appropriately vectorizes `displacement_fn`. It is often useful to define a metric instead of a displacement function in which case you can use the helper function `space.metric` to convert a displacement function to a metric function. Given a point and a shift `shift_fn(R, dR)` displaces the point `R` by an amount `dR`.
+
+The following spaces are currently supported:
+- [`space.free()`](https://jax-md.readthedocs.io/en/main/jax_md.space.html?highlight=free#jax_md.space.free) specifies a space with free boundary conditions.
+- [`space.periodic(box_size)`](https://jax-md.readthedocs.io/en/main/jax_md.space.html?highlight=periodic#jax_md.space.periodic) specifies a space with periodic boundary conditions of side length `box_size`.
+- [`space.periodic_general(box)`](https://jax-md.readthedocs.io/en/main/jax_md.space.html?highlight=periodic_general#jax_md.space.periodic_general) specifies a space as a periodic parellelopiped formed by transforming the unit cube by an affine transformation `box`.
+
+Example:
+
+```python
+from jax_md import space
+box_size = 25.0
+displacement_fn, shift_fn = space.periodic(box_size)
+```
+
+## Potential Energy ([`energy.py`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html))
+
+In the simplest case, molecular dynamics calculations are often based on a pair potential that is defined by a user. This then is used to compute a total energy whose negative gradient gives forces. One of the very nice things about JAX is that we get forces for free! The second part of the code is devoted to computing energies.
+
+We provide the following classical potentials:
+- [`energy.soft_sphere`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=soft_sphere#jax_md.energy.soft_sphere) a soft sphere whose energy increases as the overlap of the spheres to some power, `alpha`.
+- [`energy.lennard_jones`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=lennard_jones#jax_md.energy.lennard_jones) a standard 12-6 Lennard-Jones potential.
+- [`energy.morse`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=morse#jax_md.energy.morse) a morse potential.
+- [`energy.tersoff`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=tersoff#jax_md.energy.tersoff) the Tersoff potential for simulating semiconducting materials. Can load parameters from LAMMPS files.
+- [`energy.eam`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=eam#jax_md.energy.eam) embedded atom model potential with ability to load parameters from LAMMPS files.
+- [`energy.stillinger_weber`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=stillinger_weber#jax_md.energy.stillinger_weber) used to model Silicon-like systems.
+- [`energy.bks`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=bks#jax_md.energy.bks) Beest-Kramer-van Santen potential used to model silica.
+- [`energy.gupta`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=gupta#jax_md.energy.gupta) used to model gold nanoclusters.
+
+We also provide the following neural network potentials:
+- [`energy.behler_parrinello`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=behler_parrinello#jax_md.energy.behler_parrinello) a widely used fixed-feature neural network architecture for molecular systems.
+- [`energy.graph_network`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=graph_network#jax_md.energy.graph_network) a deep graph neural network designed for energy fitting.
+
+For finite-ranged potentials it is often useful to consider only interactions within a certain neighborhood. We include the `_neighbor_list` modifier to the above potentials that uses a list of neighbors (see below) for optimization.
+
+Example:
+
+```python
+import jax.numpy as np
+from jax import random
+from jax_md import energy, quantity
+N = 1000
+spatial_dimension = 2
+key = random.PRNGKey(0)
+R = random.uniform(key, (N, spatial_dimension), minval=0.0, maxval=1.0)
+energy_fn = energy.lennard_jones_pair(displacement_fn)
+print('E = {}'.format(energy_fn(R)))
+force_fn = quantity.force(energy_fn)
+print('Total Squared Force = {}'.format(np.sum(force_fn(R) ** 2)))
+```
+
+## Dynamics ([`simulate.py`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html), [`minimize.py`](https://jax-md.readthedocs.io/en/main/jax_md.minimize.html))
+
+Given an energy function and a system, there are a number of dynamics are useful to simulate. The simulation code is based on the structure of the optimizers found in JAX. In particular, each simulation function returns an initialization function and an update function. The initialization function takes a set of positions and creates the necessary dynamical state variables. The update function does a single step of dynamics to the dynamical state variables and returns an updated state.
+
+We include a several different kinds of dynamics. However, there is certainly room to add more for e.g. constant strain simulations.
+
+It is often desirable to find an energy minimum of the system. We provide two methods to do this. We provide simple gradient descent minimization. This is mostly for pedagogical purposes, since it often performs poorly. We additionally include the FIRE algorithm which often sees significantly faster convergence. Moreover a common experiment to run in the context of molecular dynamics is to simulate a system with a fixed volume and temperature.
+
+We provide the following dynamics:
+- [`simulate.nve`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html?highlight=nve#jax_md.simulate.nve) Constant energy simulation; numerically integrates Newton's laws directly.
+- [`simulate.nvt_nose_hoover`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html?highlight=nvt_nose_hoover#jax_md.simulate.nvt_nose_hoover) Uses Nose-Hoover chain to simulate a constant temperature system.
+- [`simulate.npt_nose_hoover`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html?highlight=nvp_nose_hoover#jax_md.simulate.nvp_nose_hoover) Uses Nose-Hoover chain to simulate a system at constant pressure and temperature.
+- [`simulate.nvt_langevin`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html?highlight=nvt_langevin#jax_md.simulate.nvt_langevin) Simulates a system by numerically integrating the Langevin stochastic differential equation.
+- [`simulate.hybrid_swap_mc`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html?highlight=hybrid_swap_mc#jax_md.simulate.hybrid_swap_mc) Alternates NVT dynamics with Monte-Carlo swapping moves to generate low energy glasses.
+- [`simulate.brownian`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html?highlight=brownian#jax_md.simulate.brownian) Simulates brownian motion.
+- [`minimize.gradient_descent`](https://jax-md.readthedocs.io/en/main/jax_md.minimize.html?highlight=gradient_descent#jax_md.minimize.gradient_descent) Minimizes a system using gradient descent.
+- [`minimize.fire_descent`](https://jax-md.readthedocs.io/en/main/jax_md.minimize.html?highlight=fire_descent#jax_md.minimize.fire_descent) Minimizes a system using the fast inertial relaxation engine.
+
+Example:
+
+```python
+from jax_md import simulate
+temperature = 1.0
+dt = 1e-3
+init, update = simulate.nvt_nose_hoover(energy_fn, shift_fn, dt, temperature)
+state = init(key, R)
+for _ in range(100):
+  state = update(state)
+R = state.position
+```
+
+## Spatial Partitioning ([`partition.py`](https://jax-md.readthedocs.io/en/main/jax_md.partition.html))
+
+In many applications, it is useful to construct spatial partitions of particles / objects in a simulation.
+
+We provide the following methods:
+- [`partition.cell_list`](https://jax-md.readthedocs.io/en/main/jax_md.partition.html?highlight=cell_list#jax_md.partition.cell_list) Partitions objects (and metadata) into a grid of cells.
+- [`partition.neighbor_list`](https://jax-md.readthedocs.io/en/main/jax_md.partition.html?highlight=neighbor_list#jax_md.partition.neighbor_list) Constructs a set of neighbors within some cutoff distance for each object in a simulation.
+
+Cell List Example:
+```python
+from jax_md import partition
+
+cell_size = 5.0
+capacity = 10
+cell_list_fn = partition.cell_list(box_size, cell_size, capacity)
+cell_list_data = cell_list_fn(R)
+```
+
+Neighbor List Example:
+```python
+from jax_md import partition
+
+neighbor_list_fn = partition.neighbor_list(displacement_fn, box_size, cell_size)
+neighbors = neighbor_list_fn.allocate(R) # Create a new neighbor list.
+
+# Do some simulating....
+
+neighbors = neighbors.update(R)  # Update the neighbor list without resizing.
+if neighbors.did_buffer_overflow:  # Couldn't fit all the neighbors into the list.
+  neighbors = neighbor_list_fn.allocate(R)  # So create a new neighbor list.
+```
+
+There are three different formats of neighbor list supported: `Dense`, `Sparse`, and `OrderedSparse`. `Dense` neighbor lists store neighbors in an `(particle_count, neighbors_per_particle)` array, `Sparse` neighbor lists store neighbors in a `(2, total_neighbors)` array of pairs, `OrderedSparse` neighbor lists are like `Sparse` neighbor lists, but they only store pairs such that `i < j`.
+
+# Development
+
+JAX MD is under active development. We have very limited development resources and so we typically focus on adding features that will have high impact to researchers using JAX MD (including us). Please don't hesitate to open feature requests to help us guide development. We more than welcome contributions!
+
+## Technical gotchas
+
+### GPU
+
+You must follow [JAX's](https://www.github.com/google/jax/) GPU installation instructions to enable GPU support.
+
+
+### 64-bit precision
+To enable 64-bit precision, set the respective JAX flag _before_ importing `jax_md` (see the JAX [guide](https://colab.research.google.com/github/google/jax/blob/main/notebooks/Common_Gotchas_in_JAX.ipynb#scrollTo=YTktlwTTMgFl)), for example:
+
+```python
+from jax.config import config
+config.update("jax_enable_x64", True)
+```
+
+# Publications
+
+JAX MD has been used in the following publications. If you don't see your paper on the list, but you used JAX MD let us know and we'll add it to the list!
+
+1. [A Differentiable Neural-Network Force Field for Ionic Liquids. (J. Chem. Inf. Model. 2022)](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.1c01380)<br> H. Montes-Campos, J. Carrete, S. Bichelmaier, L. M. Varela, and G. K. H. Madsen
+2. [Correlation Tracking: Using simulations to interpolate highly correlated particle tracks. (Phys. Rev. E. 2022)](https://journals.aps.org/pre/abstract/10.1103/PhysRevE.105.044608?ft=1)<br> E. M. King, Z. Wang, D. A. Weitz, F. Spaepen, and M. P. Brenner
+3. [Optimal Control of Nonequilibrium Systems Through Automatic Differentiation.](https://arxiv.org/abs/2201.00098)<br> M. C. Engel, J. A. Smith, and M. P. Brenner
+4. [Graph Neural Networks Accelerated Molecular Dynamics. (J. Chem. Phys. 2022)](https://aip.scitation.org/doi/10.1063/5.0083060)<br> Z. Li, K. Meidani, P. Yadav, and A. B. Farimani
+5. [Gradients are Not All You Need.](https://arxiv.org/abs/2111.05803)<br> L. Metz, C. D. Freeman, S. S. Schoenholz, and T. Kachman
+6. [Lagrangian Neural Network with Differential Symmetries and Relational Inductive Bias.](https://arxiv.org/abs/2110.03266)<br> R. Bhattoo, S. Ranu, and N. M. A. Krishnan
+7. [Efficient and Modular Implicit Differentiation.](https://arxiv.org/abs/2105.15183)<br> M. Blondel, Q. Berthet, M. Cuturi, R. Frostig, S. Hoyer, F. Llinares-López, F. Pedregosa, and J.-P. Vert
+8. [Learning neural network potentials from experimental data via Differentiable Trajectory Reweighting.<br>(Nature Communications 2021)](https://www.nature.com/articles/s41467-021-27241-4)<br> S. Thaler and J. Zavadlav
+9. [Learn2Hop: Learned Optimization on Rough Landscapes. (ICML 2021)](http://proceedings.mlr.press/v139/merchant21a.html)<br> A. Merchant, L. Metz, S. S. Schoenholz, and E. D. Cubuk
+10. [Designing self-assembling kinetics with differentiable statistical physics models. (PNAS 2021)](https://www.pnas.org/content/118/10/e2024083118.short)<br> C. P. Goodrich, E. M. King, S. S. Schoenholz, E. D. Cubuk, and  M. P. Brenner
+
+# Citation
+
+If you use the code in a publication, please cite the repo using the .bib,
+
+```
+@inproceedings{jaxmd2020,
+ author = {Schoenholz, Samuel S. and Cubuk, Ekin D.},
+ booktitle = {Advances in Neural Information Processing Systems},
+ publisher = {Curran Associates, Inc.},
+ title = {JAX M.D. A Framework for Differentiable Physics},
+ url = {https://papers.nips.cc/paper/2020/file/83d3d4b6c9579515e1679aca8cbc8033-Paper.pdf},
+ volume = {33},
+ year = {2020}
+}
+```
```

### Comparing `jax-md-0.2.5/README.md` & `jax-md-0.2.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: jax-md
+Version: 0.2.6
+Summary: Differentiable, Hardware Accelerated, Molecular Dynamics
+Home-page: https://github.com/google/jax-md
+Download-URL: https://pypi.org/project/jax-md/
+Author: Google
+Author-email: jax-md-dev@google.com
+License: Apache 2.0
+Project-URL: Source Code, https://github.com/google/jax-md
+Project-URL: Documentation, https://arxiv.org/abs/1912.04232
+Project-URL: Bug Tracker, https://github.com/google/jax-md/issues
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Topic :: Software Development
+Classifier: Topic :: Scientific/Engineering
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Requires-Python: >=2.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSE_SHORT
+
 # JAX, M.D.
 
 ### Accelerated, Differentiable, Molecular Dynamics
 [**Quickstart**](#getting-started) | [**Reference docs**](https://jax-md.readthedocs.io/en/main/) | [**Paper**](https://arxiv.org/pdf/1912.04232.pdf) | [**NeurIPS 2020**](https://neurips.cc/virtual/2020/public/poster_83d3d4b6c9579515e1679aca8cbc8033.html)
 
 ![Build Status](https://github.com/google/jax-md/workflows/Build/badge.svg?branch=main) [![Coverage](https://codecov.io/gh/google/jax-md/branch/main/graph/badge.svg?token=JYQpbNyICv)](https://codecov.io/gh/google/jax-md) [![PyPI](https://img.shields.io/pypi/v/jax-md)](https://pypi.org/project/jax-md/) [![PyPI - License](https://img.shields.io/pypi/l/jax_md)](https://github.com/google/jax-md/blob/main/LICENSE)
```

### Comparing `jax-md-0.2.5/jax_md/__init__.py` & `jax-md-0.2.6/jax_md/__init__.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.5/jax_md/_nn/__init__.py` & `jax-md-0.2.6/jax_md/_nn/__init__.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.5/jax_md/_nn/behler_parrinello.py` & `jax-md-0.2.6/jax_md/_nn/behler_parrinello.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.5/jax_md/_nn/e3nn_layer.py` & `jax-md-0.2.6/jax_md/_nn/e3nn_layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,15 @@
 """
 
 from typing import Optional
 
 from e3nn_jax import Irreps
 from e3nn_jax import IrrepsArray
 from e3nn_jax import FunctionalLinear
-from e3nn_jax import FunctionalFullyConnectedTensorProduct
+from e3nn_jax.legacy import FunctionalFullyConnectedTensorProduct
 
 import flax.linen as nn
 
 import jax
 import jax.numpy as jnp
 
 from jax.nn import initializers
@@ -226,15 +226,15 @@
 
 import numpy as onp
 
 
 def naive_broadcast_decorator(func):
   def wrapper(*args):
       leading_shape = jnp.broadcast_shapes(*(arg.shape[:-1] for arg in args))
-      args = [jnp.broadcast_to(arg, leading_shape + (-1,)) for arg in args]
+      args = [arg.broadcast_to(leading_shape + (-1,)) for arg in args]
       f = func
       for _ in range(len(leading_shape)):
           f = jax.vmap(f)
       return f(*args)
 
   return wrapper
 
@@ -282,15 +282,15 @@
             )
         for ins in tp.instructions
     ]
 
     f = naive_broadcast_decorator(lambda x1, x2: tp.left_right(ws, x1, x2))
     output = f(x1, x2)
     output = tree_map(lambda x: x.astype(x1.dtype), output)
-    return output._convert(self.irreps_out)
+    return output.rechunk(irreps_out)
 
 
 class Linear(nn.Module):
   """Flax module of an equivariant Linear."""
   irreps_out: Irreps
   irreps_in: Optional[Irreps] = None
```

### Comparing `jax-md-0.2.5/jax_md/_nn/gnome.py` & `jax-md-0.2.6/jax_md/_nn/gnome.py`

 * *Files 7% similar despite different names*

```diff
@@ -133,27 +133,20 @@
 
 def load_model(directory: str) -> Tuple[ConfigDict, nn.Module, PyTree]:
   with open(os.path.join(directory, 'config.json'), 'r') as f:
     c = json.loads(json.loads(f.read()))
     c = ConfigDict(c)
 
   # Now initialize the model and the optimizer functions.
-  featurizer, model = model_from_config(c)
+  model = model_from_config(c)
   opt_init, _ = optimizer(c)
 
-  # Create a dummy example to use for abstract initialization since we only need
-  # the PyTree structure to deserialize.
-  def make_irreps(x):
-    return IrrepsArray('0e + 1e', x)
-
   graph = GraphsTuple(
     ShapedArray((1, NUM_ELEMENTS), f32),    # Nodes     (nodes, features)
-    (ShapedArray((1, 3), f32),   # dR        (edges, spatial)
-     ShapedArray((1,), f32),      # dr
-     eval_shape(make_irreps, ShapedArray((1, 4), f32))),  # Spherical Harmonics
+    ShapedArray((1, 3), f32),   # dR        (edges, spatial)
     ShapedArray((1,), i32),      # senders   (edges,)
     ShapedArray((1,), i32),      # receivers (edges,)
     ShapedArray((1, 1), f32),      # globals   (graphs,)
     ShapedArray((1,), i32),      # n_node    (graphs,)
     ShapedArray((1,), i32))     # n_edge    (graphs,)
 
   def init_opt_and_model(graph):
@@ -172,8 +165,9 @@
 
   checkpoint = os.path.join(directory, checkpoints[0])
 
   with open(checkpoint, 'rb') as f:
     ckpt = serialization.from_bytes(ckpt_data, f.read())
 
   params = tree_map(lambda x: x.astype(f32), ckpt[1])
-  return c, featurizer, model, params
+  return c, model, params
+
```

### Comparing `jax-md-0.2.5/jax_md/_nn/util.py` & `jax-md-0.2.6/jax_md/_nn/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,32 +111,28 @@
     return jraph.concatenated_args(fn)(*args)
   return mlp_fn
 
 
 # Featurizers
 
 
-def neighbor_list_featurizer(displacement_fn,
-                             atom_feature_fn,
-                             edge_feature_fn,
-                             global_feature_fn):
+def neighbor_list_featurizer(displacement_fn):
   def featurize(atoms, position, neighbor, **kwargs):
     N = position.shape[0]
     graph = partition.to_jraph(neighbor, nodes=atoms)
     mask = partition.neighbor_list_mask(neighbor, True)
 
     Rb = position[graph.senders]
     Ra = position[graph.receivers]
 
     d = vmap(partial(displacement_fn, **kwargs))
     dR = d(Ra, Rb)
     dR = jnp.where(mask[:, None], dR, 1)
 
-    return graph._replace(nodes=atom_feature_fn(graph),
-                          edges=edge_feature_fn(dR))
+    return graph._replace(edges=dR)
   return featurize
 
 
 # Bessel Functions
 
 
 # Similar to the original Behler-Parinello features. Used by Nequip [1] and
```

### Comparing `jax-md-0.2.5/jax_md/colab_tools/__init__.py` & `jax-md-0.2.6/jax_md/colab_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.5/jax_md/colab_tools/renderer.py` & `jax-md-0.2.6/jax_md/colab_tools/renderer.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.5/jax_md/dataclasses.py` & `jax-md-0.2.6/jax_md/dataclasses.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,9 +70,10 @@
   return dataclasses.field(metadata={'static': True})
 
 replace = dataclasses.replace
 asdict = dataclasses.asdict
 astuple = dataclasses.astuple
 is_dataclass = dataclasses.is_dataclass
 fields = dataclasses.fields
+field = dataclasses.field
 def unpack(dc) -> tuple:
     return tuple(getattr(dc, field.name) for field in dataclasses.fields(dc))
```

### Comparing `jax-md-0.2.5/jax_md/elasticity.py` & `jax-md-0.2.6/jax_md/elasticity.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.5/jax_md/energy.py` & `jax-md-0.2.6/jax_md/energy.py`

 * *Files 4% similar despite different names*

```diff
@@ -939,15 +939,15 @@
 
     if nwords != params_per_line:
       raise ValueError('Incorrect format: %d not in %d'
         % (nwords, params_per_line))
     else:
       skip = False
 
-    words[3:] = f32(words[3:])
+    words[3:] = f64(words[3:])
     params.append({
         'element1': words[0],
         'element2': words[1],
         'element3': words[2],
         'mTf': words[3],
         'gamma': words[4],
         'lam3': words[5],
@@ -1264,14 +1264,182 @@
   return tersoff_neighbor_list(displacement,
                                box_size,
                                load_lammps_tersoff_parameters(f),
                                dr_threshold=dr_threshold,
                                fractional_coordinates=fractional_coordinates,
                                **neighbor_kwargs)
 
+# (EDIP) Environment-dependent interatomic potential
+
+def _edip_cutoff_function(r: Array, cutoff: f64, c: f64, alpha: f64) -> Array:
+    x_term = (r - c) / (cutoff - c)
+    expo_term = jnp.exp(alpha / (1 - (x_term ** (-3))))
+    outer = jnp.where(r > cutoff,
+                      0,
+                      expo_term)
+    inner = jnp.where(r > c, outer, 1)
+    return inner
+
+
+def _edip_radial_interaction(A: f64, B: f64, rho: f64, sigma: f64, c: f64,
+                             alpha: f64, beta: f64, cutoff: f64, mask,
+                             r: Array) -> Array:
+  within_cutoff = (r > 0) & (r < cutoff)
+  repul = (B / r) ** (rho)
+  r = jnp.where(within_cutoff, r, 0)
+  Z_i = util.high_precision_sum(_edip_cutoff_function(r, cutoff, c, alpha) * mask,
+                                axis=1, keepdims=True)
+  p_Z = jnp.exp(-beta * (Z_i ** 2))
+  term1 = repul - p_Z
+  term2 = jnp.exp(sigma / (r - cutoff))
+  return jnp.where(within_cutoff, A * term1 * term2, 0.0)
+
+
+def _edip_angle_interaction(lam: f64, gamma: f64, Q_0: f64, cutoff: f64,
+                            u1: f64, u2: f64, u3: f64, u4: f64, c: f64, eta: f64,
+                            alpha: f64, mu: f64, mask, dR12: Array, dR13: Array) -> Array:
+  dr12 = space.distance(dR12)
+  dr13 = space.distance(dR13)
+  dr12 = jnp.where(dr12 < cutoff, dr12, 0)
+  dr13 = jnp.where(dr13 < cutoff, dr13, 0)
+  term1 = jnp.exp(gamma / (dr12 - cutoff) + gamma / (dr13 - cutoff))
+  l_ijk = quantity.cosine_angle_between_two_vectors(dR12, dR13)
+  Z_i = util.high_precision_sum(_edip_cutoff_function(dr13, cutoff, c, alpha) * mask,
+                                keepdims=False)
+  tau_Z = u1 + u2 * ((u3 * jnp.exp(-u4 * Z_i)) - jnp.exp(-2 * u4 * Z_i))
+  Q_Z = Q_0 * jnp.exp(-mu * Z_i)
+  l_tau = (l_ijk + tau_Z) ** 2
+  term2 = ((1 - jnp.exp(-Q_Z * l_tau)) + (eta * Q_Z * l_tau))
+
+  within_cutoff = (dr12 > 0) & (dr13 > 0) & (jnp.linalg.norm(dR12 - dR13) > 1e-5)
+  return jnp.where(within_cutoff, lam * term1 * term2, 0)
+
+def edip(displacement: DisplacementFn,
+           u1: f64 = -0.165799,
+           u2: f64 = 32.557,
+           u3: f64 = 0.286198,
+           u4: f64 = 0.66,
+           rho: f64 = 1.2085196,
+           eta: f64 = 0.2523244,
+           Q_0: f64 = 312.1341346,
+           mu: f64 = 0.6966326,
+           beta: f64 = 0.0070975,
+           alpha: f64 = 3.1083847,
+           A: f64 = 7.9821730,
+           lam: f64 = 1.4533108,
+           B: f64 = 1.5075463,
+           gamma: f64 = 1.1247945,
+           sigma: f64 = 0.5774108,
+           c: f64 = 2.5609104,
+           cutoff: f64 = 3.1213820) -> Callable[[Array], Array]:
+    """
+    Computes the the Environment-dependent interatomic potential (EDIP).
+    The parameter values are for bulk Silicon [1,2]. The EDIP potential is a bond
+    order potential which depends on the local coordination number of the atom.
+
+    :param displacement: displacement function for the space.
+    :param u1: parameter for the three-body bond order function tau(Z) (pure number)
+    :param u2: parameter for the three-body bond order function tau(Z) (pure number)
+    :param u3: parameter for the three-body bond order function tau(Z) (pure number)
+    :param u4: parameter for the three-body bond order function tau(Z) (pure number)
+    :param rho: exponent for the repulsive part of two-body potential (pure number)
+    :param eta: parameter for the three-body term (pure number)
+    :param Q_0: parameter for the three-body bond order function Q(Z) (pure number)
+    :param mu: parameter for the three-body bond order function Q(Z) (pure number)
+    :param beta: parameter for the two-body bond order function p(Z) (pure number)
+    :param alpha: parameter for the cutoff function (pure number)
+    :param A: parameter that determines the energy scale of two-body term (eV)
+    :param lam: parameter that determines the energy scale of three-body term (eV)
+    :param B: parameter for the repulsive part of two-body potential (Angstrom)
+    :param gamma: parameter for the radial part of three-body term (Angstrom)
+    :param sigma: parameter that determines the distance scale between neighbors (Angstrom)
+    :param c: inner cutoff for the cutoff function f(r) (Angstrom)
+    :param cutoff: outer cutoff (a) for the cutoff function f(r) (Angstrom)
+    :return: A function that computes the potential energy.
+
+    References:
+    [1] - Martin Z. Bazant, Efthimios Kaxiras, and J. F. Justo.
+          "Environment-dependent interatomic potential for bulk silicon".
+          Phys. Rev. B 56, 8542 (1997).
+    [2] - João F. Justo, Martin Z. Bazant, Efthimios Kaxiras, V. V. Bulatov,
+          and Sidney Yip. "Interatomic potential for silicon defects and
+          disordered phases". Phys. Rev. B 58, 2539 (1998).
+    """
+    two_body_fn = partial(_edip_radial_interaction, A, B, rho, sigma, c, alpha, beta, cutoff)
+    three_body_fn = partial(_edip_angle_interaction, lam, gamma, Q_0, cutoff,
+                            u1, u2, u3, u4, c, eta,
+                            alpha, mu)
+
+    def compute_fn(R, **kwargs):
+      _three_body_fn = vmap(vmap(vmap(three_body_fn, (None, 0, None)), (None, None, 0)))
+      d = partial(displacement, **kwargs)
+      dR = space.map_product(d)(R, R)
+      dr = space.distance(dR)
+      N = R.shape[0]
+      mask = (1 - jnp.eye(N)) * (dr < cutoff)
+      first_term = util.high_precision_sum(two_body_fn(mask, dr))
+      second_term = util.high_precision_sum(_three_body_fn(mask, dR, dR)) / 2.0
+      return first_term + second_term
+
+    return compute_fn
+
+
+def edip_neighbor_list(displacement: DisplacementFn,
+                       box_size: f64,
+                       u1: f64 = -0.165799,
+                       u2: f64 = 32.557,
+                       u3: f64 = 0.286198,
+                       u4: f64 = 0.66,
+                       rho: f64 = 1.2085196,
+                       eta: f64 = 0.2523244,
+                       Q_0: f64 = 312.1341346,
+                       mu: f64 = 0.6966326,
+                       beta: f64 = 0.0070975,
+                       alpha: f64 = 3.1083847,
+                       A: f64 = 7.9821730,
+                       lam: f64 = 1.4533108,
+                       B: f64 = 1.5075463,
+                       gamma: f64 = 1.1247945,
+                       sigma: f64 = 0.5774108,
+                       c: f64 = 2.5609104,
+                       cutoff: f64 = 3.1213820,
+                       dr_threshold: f64 = 0.0,
+                       fractional_coordinates: bool = True,
+                       format: NeighborListFormat = partition.Dense,
+                       **neighbor_kwargs) -> Tuple[NeighborFn, Callable[[Array, NeighborList], Array]]:
+  two_body_fn = partial(_edip_radial_interaction, A, B, rho, sigma, c, alpha, beta, cutoff)
+  three_body_fn = partial(_edip_angle_interaction, lam, gamma, Q_0, cutoff,
+                          u1, u2, u3, u4, c, eta,
+                          alpha, mu)
+
+  neighbor_fn = partition.neighbor_list(displacement,
+                                        box_size,
+                                        cutoff,
+                                        dr_threshold,
+                                        format=format,
+                                        fractional_coordinates=fractional_coordinates,
+                                        **neighbor_kwargs)
+
+  def compute_fn(R, neighbor, **kwargs):
+    d = partial(displacement, **kwargs)
+    mask = partition.neighbor_list_mask(neighbor, mask_self=True)
+    if format is partition.Dense:
+      _three_body_fn = vmap(vmap(vmap(three_body_fn, (None, 0, None)), (None, None, 0)))
+      dR = space.map_neighbor(d)(R, R[neighbor.idx])
+      dr = space.distance(dR)
+      first_term = util.high_precision_sum(two_body_fn(mask, dr) * mask)
+      mask_ijk = mask[:, None, :] * mask[:, :, None]
+      second_term = util.high_precision_sum(_three_body_fn(mask, dR, dR) * mask_ijk) / 2.0
+    else:
+      raise NotImplementedError('EDIP potential only implemented '
+                                'with Dense neighbor lists.')
+
+    return first_term + second_term
+
+  return neighbor_fn, compute_fn
 
 # Embedded Atom Method
 
 
 def load_lammps_eam_parameters(file: TextIO) -> Tuple[Callable[[Array], Array],
                                                       Callable[[Array], Array],
                                                       Callable[[Array], Array],
@@ -1789,24 +1957,24 @@
 
 def nequip_neighbor_list(displacement_fn,
                          box,
                          cfg: ConfigDict=None,
                          atoms=None,
                          **nl_kwargs):
   cfg = nequip.default_config() if cfg is None else cfg
-  featurizer, model = nequip.model_from_config(cfg)
+  model = nequip.model_from_config(cfg)
 
   neighbor_fn = partition.neighbor_list(
     displacement_fn,
     box,
     cfg.r_max,
     format=partition.Sparse,
     **nl_kwargs)
 
-  featurizer = nn.util.neighbor_list_featurizer(displacement_fn, *featurizer)
+  featurizer = nn.util.neighbor_list_featurizer(displacement_fn)
 
   def init_fn(key, position, neighbor, **kwargs):
     _atoms = kwargs.pop('atoms', atoms)
     if _atoms is None:
       raise ValueError('A one-hot encoding of the atoms is required.')
     # TODO: It would be nicer to do this without computing flops
     # since we really only need the shape of the graph for initialization.
@@ -1826,24 +1994,24 @@
 def load_gnome_model_neighbor_list(
         displacement_fn,
         box,
         directory,
         atoms = None,
         **nl_kwargs):
   """Load a gnome model from a checkpoint."""
-  cfg, featurizer, model, params = gnome.load_model(directory)
+  cfg, model, params = gnome.load_model(directory)
 
   neighbor_fn = partition.neighbor_list(
     displacement_fn,
     box,
     cfg.r_max,
     format=partition.Sparse,
     **nl_kwargs)
 
-  featurizer = nn.util.neighbor_list_featurizer(displacement_fn, *featurizer)
+  featurizer = nn.util.neighbor_list_featurizer(displacement_fn)
 
   def energy_fn(position, neighbor, **kwargs):
     _atoms = kwargs.pop('atoms', atoms)
     if _atoms is None:
       raise ValueError('A one-hot encoding of the atoms is required.')
     graph = featurizer(_atoms, position, neighbor, **kwargs)
     return model.apply(params, graph)[0, 0]
```

### Comparing `jax-md-0.2.5/jax_md/interpolate.py` & `jax-md-0.2.6/jax_md/interpolate.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.5/jax_md/io.py` & `jax-md-0.2.6/jax_md/io.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.5/jax_md/minimize.py` & `jax-md-0.2.6/jax_md/minimize.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.5/jax_md/nn.py` & `jax-md-0.2.6/jax_md/nn.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.5/jax_md/partition.py` & `jax-md-0.2.6/jax_md/partition.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Code to transform functions on individual tuples of particles to sets."""
 
+import jax
 from absl import logging
 
 from functools import reduce, partial
 from collections import namedtuple
 
 from enum import Enum
 from enum import IntEnum
@@ -784,25 +785,25 @@
   box = f32(box)
 
   cutoff = r_cutoff + dr_threshold
   cutoff_sq = cutoff ** 2
   threshold_sq = (dr_threshold / f32(2)) ** 2
   metric_sq = _displacement_or_metric_to_metric_sq(displacement_or_metric)
 
-  @jit
-  def candidate_fn(position: Array) -> Array:
-    candidates = jnp.arange(position.shape[0])
+  @partial(jit, static_argnums=0)
+  def candidate_fn(positionShape) -> Array:
+    candidates = jnp.arange(positionShape[0])
     return jnp.broadcast_to(candidates[None, :],
-                            (position.shape[0], position.shape[0]))
+                            (positionShape[0], positionShape[0]))
 
-  @jit
-  def cell_list_candidate_fn(cl: CellList, position: Array) -> Array:
-    N, dim = position.shape
+  @partial(jit, static_argnums=1)
+  def cell_list_candidate_fn(cl_id_buffer, positionShape) -> Array:
+    N, dim = positionShape
 
-    idx = cl.id_buffer
+    idx = cl_id_buffer
 
     cell_idx = [idx]
 
     for dindex in _neighboring_cells(dim):
       if onp.all(dindex == 0):
         continue
       cell_idx += [_shift_array(idx, dindex)]
@@ -900,18 +901,18 @@
           cell_size = neighbors.cell_size
           cl_fn = neighbors.cell_list_fn
           if cl_fn is not None:
             cl = cl_fn.update(position, neighbors.cell_list_capacity)
 
       if cl is None:
         cl_capacity = None
-        idx = candidate_fn(position)
+        idx = candidate_fn(position.shape)
       else:
         err = err.update(PEC.CELL_LIST_OVERFLOW, cl.did_buffer_overflow)
-        idx = cell_list_candidate_fn(cl, position)
+        idx = cell_list_candidate_fn(cl.id_buffer, position.shape)
         cl_capacity = cl.cell_capacity
 
       if mask_self:
         idx = mask_self_fn(idx)
       if custom_mask_function is not None:
         idx = custom_mask_function(idx)
 
@@ -952,15 +953,15 @@
     if nbrs is None:
       return neighbor_fn((position, PartitionError(jnp.zeros((), jnp.uint8))))
 
     neighbor_fn = partial(neighbor_fn, max_occupancy=nbrs.max_occupancy)
 
     # If the box has been updated, then check that fractional coordinates are
     # enabled and that the cell list has big enough cells.
-    if 'box' in kwargs:
+    if 'box' in kwargs and not disable_cell_list:
       if not fractional_coordinates:
         raise ValueError('Neighbor list cannot accept a box keyword argument '
                          'if fractional_coordinates is not enabled.')
       # `cell_size` is really the minimum cell size.
       cur_cell_size = _cell_size(1.0, nbrs.cell_size)
       new_cell_size = _cell_size(1.0,
                                  _fractional_cell_size(kwargs['box'], cutoff))
```

### Comparing `jax-md-0.2.5/jax_md/quantity.py` & `jax-md-0.2.6/jax_md/quantity.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 from jax import grad, vmap, eval_shape
 from jax.tree_util import tree_map, tree_reduce
 import jax.numpy as jnp
 from jax import ops
 from jax import ShapeDtypeStruct
 from jax.tree_util import tree_map, tree_reduce
+from jax.scipy.special import gammaln
 
 from jax_md import space, dataclasses, partition, util
 
 import functools
 import operator
 
 partial = functools.partial
@@ -115,15 +116,15 @@
   raise ValueError(('Box must be either: a scalar, a vector, or a matrix. '
                     f'Found {box}.'))
 
 
 def kinetic_energy(*unused_args,
                    momentum: Array=None,
                    velocity: Array=None,
-                   mass: Array=f32(1.0)
+                   mass: Array=1.0,
                    ) -> float:
   """Computes the kinetic energy of a system.
 
   To avoid ambiguity, either momentum or velocity must be passed explicitly
   as a keyword argument.
 
   Args:
@@ -148,15 +149,15 @@
   ke = tree_map(lambda m, q: 0.5 * util.high_precision_sum(k(q, m)), mass, q)
   return tree_reduce(operator.add, ke, 0.0)
 
 
 def temperature(*unused_args,
                 momentum: Array=None,
                 velocity: Array=None,
-                mass: Array=f32(1.0)
+                mass: Array=1.0,
                 ) -> float:
   """Computes the temperature of a system.
 
   To avoid ambiguity, either momentum or velocity must be passed explicitly
   as a keyword argument.
 
   Args:
@@ -293,26 +294,26 @@
 
   When species=None, gofr is expected to be an array of shape (N,nr), where N is
   the number of species and nr is the number of radii to be considered. The
   average is calculated over all particles, so an array of shape (nr,) is
   returned.
 
   When species is specified, gofr is expected to be a list of nspecies arrays,
-  each of shape (N,nr), where nspecies is the number of unique species types. 
+  each of shape (N,nr), where nspecies is the number of unique species types.
   Here, the average is carried out separately for every pair of species, so the
-  returned array has shape (nspecies, nspecies, nr). 
+  returned array has shape (nspecies, nspecies, nr).
 
   Args:
     gofr: array of shape (N,nr) or a list of arrays of shape (N,nr), where nr is
       the number of radii for which :math:`g(r)` is calculated.
-    species: Optional. Array of shape (N,) specifying the species of each 
+    species: Optional. Array of shape (N,) specifying the species of each
       particle.
 
   Returns:
-    An array of shape (nr,) for species=None, otherwise an array of shape 
+    An array of shape (nr,) for species=None, otherwise an array of shape
       (nspecies, nspecies, nr), where nspecies is the number of unique species.
   """
   if species is None:
     return jnp.mean(gofr, axis=0)
   species_types = jnp.unique(species) #note: this returns in sorted order
   return jnp.array([ [ jnp.mean(gofr[si][species==s], axis=0) \
       for s in species_types] for si in range(species_types.size)])
@@ -349,24 +350,24 @@
       zero.
 
   Returns:
     A function `g_fn` that computes the pair correlation function for a
     collection of particles.
 
   :math:`g(r)` is calculated separately for each particle. For species=None, the
-  output of `g_fn` is an array of shape (N, nr), where N is the number of 
-  particles passed to `g_fn` and nr is the size of radii (the number of points 
+  output of `g_fn` is an array of shape (N, nr), where N is the number of
+  particles passed to `g_fn` and nr is the size of radii (the number of points
   at which we calculate :math:`g(r)`. When species is specified, the output is a
   list of nspecies arrays, each of shape (N, nr), where nspecies is the number
   of unique species. If `gofr` is the output of `g_fn`, then gofr[si][i] gives
   the :math:`g(r)` for particle i considering only pair particles of species si.
 
-  Note: when species is specified, the returned list is in the order of the 
-  sorted unique species indices, not the order in which they appear. 
-  
+  Note: when species is specified, the returned list is in the order of the
+  sorted unique species indices, not the order in which they appear.
+
   """
   d = space.canonicalize_displacement_or_metric(displacement_or_metric)
   d = space.map_product(d)
 
   inv_rad = 1 / (radii + eps)
 
   def pairwise(dr, dim):
@@ -410,19 +411,19 @@
     eps: float = 1e-7,
     fractional_coordinates: bool=False,
     format: partition.NeighborListFormat=partition.Dense,
     compute_average: bool = False):
   """Computes the pair correlation function at a mesh of distances.
 
   The pair correlation function measures the number of particles at a given
-  distance from a central particle. The pair correlation function is defined by 
-  
+  distance from a central particle. The pair correlation function is defined by
+
   .. math::
     g(r) = <\sum_{i \\neq j}\delta(r - |r_i - r_j|)>
-  
+
   We make the approximation,
 
   .. math::
     \delta(r) \\approx {1 \over \sqrt{2\pi\sigma^2}e^{-r / (2\sigma^2)}}
 
   This function uses neighbor lists to speed up the calculation.
 
@@ -445,23 +446,23 @@
   Returns:
     A pair of functions: `neighbor_fn` that constructs a neighbor list (see
     `neighbor_list` in `partition.py` for details). `g_fn` that computes the
     pair correlation function for a collection of particles given their
     position and a neighbor list.
 
   :math:`g(r)` is calculated separately for each particle. For species=None, the
-  output of `g_fn` is an array of shape (N, nr), where N is the number of 
-  particles passed to `g_fn` and nr is the size of radii (the number of points 
+  output of `g_fn` is an array of shape (N, nr), where N is the number of
+  particles passed to `g_fn` and nr is the size of radii (the number of points
   at which we calculate :math:`g(r)`. When species is specified, the output is a
   list of nspecies arrays, each of shape (N, nr), where nspecies is the number
   of unique species. If `gofr` is the output of `g_fn`, then gofr[si][i] gives
   the :math:`g(r)` for particle i considering only pair particles of species si.
 
   Note: when species is specified, the returned list is in the order of the
-  sorted unique species indices, not the order in which they appear. 
+  sorted unique species indices, not the order in which they appear.
   """
   metric = space.canonicalize_displacement_or_metric(displacement_or_metric)
   inv_rad = 1 / (radii + eps)
   def pairwise(dr, dim):
     return jnp.exp(-f32(0.5) * (dr - radii)**2 / sigma**2) * inv_rad**(dim - 1)
 
   neighbor_fn = partition.neighbor_list(displacement_or_metric,
@@ -530,52 +531,52 @@
       return g_R
   return neighbor_fn, g_fn
 
 def nball_unit_volume(spatial_dimension: int) -> float:
   """ Return the volume of a unit sphere in arbitrary dimensions
   """
   return jnp.power(jnp.pi, spatial_dimension / 2) / \
-    jnp.exp( jsp.special.gammaln(spatial_dimension / 2 + 1))
+    jnp.exp( gammaln(spatial_dimension / 2 + 1))
 
-def particle_volume(radii: Array, 
-                    spatial_dimension: int, 
-                    particle_count: Array = 1, 
+def particle_volume(radii: Array,
+                    spatial_dimension: int,
+                    particle_count: Array = 1,
                     species: Array = None) -> float:
   """ Calculate the volume of a collection of particles
 
   Args:
     radii: array of shape (n,) giving particle radii, where n can be 1, the
       number of species, or the number of particles depending on the values of
-      particle_count and species. 
+      particle_count and species.
     spatial_dimension: int giving the spatial dimension
     particle_count: number of particles with each radii. Broadcastable to radii.
-    species: list of particle species. If provided, this overrides 
+    species: list of particle species. If provided, this overrides
       particle_count and radii is expected to give per-species radii
-  
+
   Returns: the sum of the volume of all the particles
   """
   V_unit = nball_unit_volume(spatial_dimension)
   V_particle = V_unit * radii**spatial_dimension
 
   if species is not None:
     particle_count = jnp.bincount(species)
 
   return jnp.sum(particle_count * V_particle)
 
-def volume_fraction(box: Box, 
-                    radii: Array, 
-                    spatial_dimension: int, 
-                    particle_count: Array = 1, 
+def volume_fraction(box: Box,
+                    radii: Array,
+                    spatial_dimension: int,
+                    particle_count: Array = 1,
                     species: Array = None) -> float:
   """ Calculate the volume fraction
 
   See documentation for particle_volume for explanation of parameters
   """
   Vparticle = particle_volume(radii, spatial_dimension, particle_count, species)
-  return Vparticle / quantity.volume(spatial_dimension, box)
+  return Vparticle / volume(spatial_dimension, box)
 
 def box_size_at_volume_fraction(volume_fraction: float,
                                 radii: Array,
                                 spatial_dimension: int,
                                 particle_count: Array = 1,
                                 species: Array = None) -> float:
   """ Calculate box_size to obtain a desired volume fraction
```

### Comparing `jax-md-0.2.5/jax_md/rigid_body.py` & `jax-md-0.2.6/jax_md/rigid_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -700,15 +700,15 @@
   """
 
   points: Array
   masses: Array
   point_count: Array
   point_offset: Array
   point_species: Optional[Array] = None
-  point_radius: float = f32(0.5)
+  point_radius: float = dataclasses.field(default_factory=lambda: f32(0.5))
 
   def dimension(self) -> int:
     """Returns the spatial dimension of the shape."""
     return self.points.shape[-1]
 
   def _sum_over_shapes(self, x):
     shape_count = len(self.point_count)
```

### Comparing `jax-md-0.2.5/jax_md/simulate.py` & `jax-md-0.2.6/jax_md/simulate.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.5/jax_md/smap.py` & `jax-md-0.2.6/jax_md/smap.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.5/jax_md/space.py` & `jax-md-0.2.6/jax_md/space.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.5/jax_md/test_util.py` & `jax-md-0.2.6/jax_md/test_util.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.5/jax_md/tpu.py` & `jax-md-0.2.6/jax_md/tpu.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,16 +42,15 @@
 
 import jax
 from jax import jit, vmap, grad, pmap
 from jax import lax
 from jax import random
 from jax.experimental import maps
 from jax.experimental import mesh_utils
-from jax.experimental import PartitionSpec as P
-from jax.experimental.global_device_array import GlobalDeviceArray
+from jax.sharding import PartitionSpec as P
 
 import jax.numpy as np
 from jax.tree_util import tree_map, tree_flatten, tree_unflatten
 
 from jax_md import dataclasses
 from jax_md import energy
 from jax_md import simulate
@@ -336,18 +335,16 @@
 
   def create_instance(index):
     index_into_topology = index[:len(topology)]
     key = np.squeeze(pkeys[index_into_topology])
     return np.expand_dims(create_instance_by_key(key), range(len(topology)))
 
   mesh, axes = mesh_and_axes(topology)
-  cell_data = GlobalDeviceArray.from_callback(topology + arr_box_size + (num_dims + 1,),
-                                              mesh,
-                                              axes,
-                                              create_instance)
+  cell_data = jax.make_array_from_callback(topology + arr_box_size + (num_dims + 1,),
+                                           jax.sharding.NamedSharding(mesh, axes), create_instance)
 
   # Function to fold the grid on each device separately.
   inner_fold_fn = lambda grid: _fold_grid(grid, max_grid_distance, batch_size)
   inner_fold_fn = parallelize(inner_fold_fn, topology)
 
   cell_data, factors = inner_fold_fn(cell_data)
```

### Comparing `jax-md-0.2.5/jax_md/util.py` & `jax-md-0.2.6/jax_md/util.py`

 * *Files identical despite different names*

### Comparing `jax-md-0.2.5/jax_md.egg-info/PKG-INFO` & `jax-md-0.2.6/jax_md.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,242 +1,243 @@
 Metadata-Version: 2.1
 Name: jax-md
-Version: 0.2.5
+Version: 0.2.6
 Summary: Differentiable, Hardware Accelerated, Molecular Dynamics
 Home-page: https://github.com/google/jax-md
+Download-URL: https://pypi.org/project/jax-md/
 Author: Google
 Author-email: jax-md-dev@google.com
 License: Apache 2.0
-Download-URL: https://pypi.org/project/jax-md/
 Project-URL: Source Code, https://github.com/google/jax-md
 Project-URL: Documentation, https://arxiv.org/abs/1912.04232
 Project-URL: Bug Tracker, https://github.com/google/jax-md/issues
-Description: # JAX, M.D.
-        
-        ### Accelerated, Differentiable, Molecular Dynamics
-        [**Quickstart**](#getting-started) | [**Reference docs**](https://jax-md.readthedocs.io/en/main/) | [**Paper**](https://arxiv.org/pdf/1912.04232.pdf) | [**NeurIPS 2020**](https://neurips.cc/virtual/2020/public/poster_83d3d4b6c9579515e1679aca8cbc8033.html)
-        
-        ![Build Status](https://github.com/google/jax-md/workflows/Build/badge.svg?branch=main) [![Coverage](https://codecov.io/gh/google/jax-md/branch/main/graph/badge.svg?token=JYQpbNyICv)](https://codecov.io/gh/google/jax-md) [![PyPI](https://img.shields.io/pypi/v/jax-md)](https://pypi.org/project/jax-md/) [![PyPI - License](https://img.shields.io/pypi/l/jax_md)](https://github.com/google/jax-md/blob/main/LICENSE)
-        
-        Molecular dynamics is a workhorse of modern computational condensed matter physics. It is frequently used to simulate materials to observe how small scale interactions can give rise to complex large-scale phenomenology. Most molecular dynamics packages (e.g. HOOMD Blue or LAMMPS) are complicated, specialized pieces of code that are many thousands of lines long. They typically involve significant code duplication to allow for running simulations on CPU and GPU. Additionally, large amounts of code is often devoted to taking derivatives of quantities to compute functions of interest (e.g. gradients of energies to compute forces).
-        
-        However, recent work in machine learning has led to significant software developments that might make it possible to write more concise molecular dynamics simulations that offer a range of benefits. Here we target JAX, which allows us to write python code that gets compiled to XLA and allows us to run on CPU, GPU, or TPU. Moreover, JAX allows us to take derivatives of python code. Thus, not only is this molecular dynamics simulation automatically hardware accelerated, it is also __end-to-end__ differentiable. This should allow for some interesting experiments that we're excited to explore.
-        
-        JAX, MD is a research project that is currently under development. Expect sharp edges and possibly some API breaking changes as we continue to support a broader set of simulations. JAX MD is a functional and data driven library. Data is stored in arrays or tuples of arrays and functions transform data from one state to another.
-        
-        ### Getting Started
-        
-        For a video introducing JAX MD along with a [demo](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/talk_demo.ipynb), check out this talk from the Physics meets Machine Learning series:
-        
-        [![Science Meets ML Talk](https://img.youtube.com/vi/Bkm8tGET7-w/0.jpg)](https://www.youtube.com/watch?v=Bkm8tGET7-w)
-        
-        To get started playing around with JAX MD check out the following colab notebooks on Google Cloud without needing to install anything. For a very simple introduction, I would recommend the Minimization example. For an example of a bunch of the features of JAX MD, check out the JAX MD cookbook.
-        
-        - [JAX MD Cookbook](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/jax_md_cookbook.ipynb)
-        - [Minimization](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/minimization.ipynb)
-        - [NVE Simulation](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/nve_simulation.ipynb)
-        - [NVT Simulation](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/nvt_simulation.ipynb)
-        - [NPT Simulation](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/npt_simulation.ipynb)
-        - [NVE with Neighbor Lists](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/nve_neighbor_list.ipynb)
-        - [Custom Potentials](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/customizing_potentials_cookbook.ipynb)
-        - [Neural Network Potentials](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/neural_networks.ipynb)
-        - [Flocking](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/flocking.ipynb)
-        - [Meta Optimization](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/meta_optimization.ipynb)
-        - [Swap Monte Carlo (Cargese Summer School)](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/cargese_swap_mc.ipynb)
-        - [Implicit Differentiation](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/implicit_differentiation.ipynb)
-        - [Athermal Linear Elasticity](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/athermal_linear_elasticity.ipynb)
-        - [Smash a Sand Castle](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/sand_castle.ipynb)
-        
-        You can install JAX MD locally with pip,
-        ```
-        pip install jax-md --upgrade
-        ```
-        If you want to build the latest version then you can grab the most recent version from head,
-        ```
-        git clone https://github.com/google/jax-md
-        pip install -e jax-md
-        ```
-        
-        # Overview
-        
-        We now summarize the main components of the library.
-        
-        ## Spaces ([`space.py`](https://jax-md.readthedocs.io/en/main/jax_md.space.html))
-        
-        In general we must have a way of computing the pairwise distance between atoms. We must also have efficient strategies for moving atoms in some space that may or may not be globally isomorphic to R^N. For example, periodic boundary conditions are commonplace in simulations and must be respected. Spaces are defined as a pair of functions, `(displacement_fn, shift_fn)`. Given two points `displacement_fn(R_1, R_2)` computes the displacement vector between the two points. If you would like to compute displacement vectors between all pairs of points in a given `(N, dim)` matrix the function `space.map_product` appropriately vectorizes `displacement_fn`. It is often useful to define a metric instead of a displacement function in which case you can use the helper function `space.metric` to convert a displacement function to a metric function. Given a point and a shift `shift_fn(R, dR)` displaces the point `R` by an amount `dR`.
-        
-        The following spaces are currently supported:
-        - [`space.free()`](https://jax-md.readthedocs.io/en/main/jax_md.space.html?highlight=free#jax_md.space.free) specifies a space with free boundary conditions.
-        - [`space.periodic(box_size)`](https://jax-md.readthedocs.io/en/main/jax_md.space.html?highlight=periodic#jax_md.space.periodic) specifies a space with periodic boundary conditions of side length `box_size`.
-        - [`space.periodic_general(box)`](https://jax-md.readthedocs.io/en/main/jax_md.space.html?highlight=periodic_general#jax_md.space.periodic_general) specifies a space as a periodic parellelopiped formed by transforming the unit cube by an affine transformation `box`.
-        
-        Example:
-        
-        ```python
-        from jax_md import space
-        box_size = 25.0
-        displacement_fn, shift_fn = space.periodic(box_size)
-        ```
-        
-        ## Potential Energy ([`energy.py`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html))
-        
-        In the simplest case, molecular dynamics calculations are often based on a pair potential that is defined by a user. This then is used to compute a total energy whose negative gradient gives forces. One of the very nice things about JAX is that we get forces for free! The second part of the code is devoted to computing energies.
-        
-        We provide the following classical potentials:
-        - [`energy.soft_sphere`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=soft_sphere#jax_md.energy.soft_sphere) a soft sphere whose energy increases as the overlap of the spheres to some power, `alpha`.
-        - [`energy.lennard_jones`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=lennard_jones#jax_md.energy.lennard_jones) a standard 12-6 Lennard-Jones potential.
-        - [`energy.morse`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=morse#jax_md.energy.morse) a morse potential.
-        - [`energy.tersoff`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=tersoff#jax_md.energy.tersoff) the Tersoff potential for simulating semiconducting materials. Can load parameters from LAMMPS files.
-        - [`energy.eam`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=eam#jax_md.energy.eam) embedded atom model potential with ability to load parameters from LAMMPS files.
-        - [`energy.stillinger_weber`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=stillinger_weber#jax_md.energy.stillinger_weber) used to model Silicon-like systems.
-        - [`energy.bks`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=bks#jax_md.energy.bks) Beest-Kramer-van Santen potential used to model silica.
-        - [`energy.gupta`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=gupta#jax_md.energy.gupta) used to model gold nanoclusters.
-        
-        We also provide the following neural network potentials:
-        - [`energy.behler_parrinello`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=behler_parrinello#jax_md.energy.behler_parrinello) a widely used fixed-feature neural network architecture for molecular systems.
-        - [`energy.graph_network`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=graph_network#jax_md.energy.graph_network) a deep graph neural network designed for energy fitting.
-        
-        For finite-ranged potentials it is often useful to consider only interactions within a certain neighborhood. We include the `_neighbor_list` modifier to the above potentials that uses a list of neighbors (see below) for optimization.
-        
-        Example:
-        
-        ```python
-        import jax.numpy as np
-        from jax import random
-        from jax_md import energy, quantity
-        N = 1000
-        spatial_dimension = 2
-        key = random.PRNGKey(0)
-        R = random.uniform(key, (N, spatial_dimension), minval=0.0, maxval=1.0)
-        energy_fn = energy.lennard_jones_pair(displacement_fn)
-        print('E = {}'.format(energy_fn(R)))
-        force_fn = quantity.force(energy_fn)
-        print('Total Squared Force = {}'.format(np.sum(force_fn(R) ** 2)))
-        ```
-        
-        ## Dynamics ([`simulate.py`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html), [`minimize.py`](https://jax-md.readthedocs.io/en/main/jax_md.minimize.html))
-        
-        Given an energy function and a system, there are a number of dynamics are useful to simulate. The simulation code is based on the structure of the optimizers found in JAX. In particular, each simulation function returns an initialization function and an update function. The initialization function takes a set of positions and creates the necessary dynamical state variables. The update function does a single step of dynamics to the dynamical state variables and returns an updated state.
-        
-        We include a several different kinds of dynamics. However, there is certainly room to add more for e.g. constant strain simulations.
-        
-        It is often desirable to find an energy minimum of the system. We provide two methods to do this. We provide simple gradient descent minimization. This is mostly for pedagogical purposes, since it often performs poorly. We additionally include the FIRE algorithm which often sees significantly faster convergence. Moreover a common experiment to run in the context of molecular dynamics is to simulate a system with a fixed volume and temperature.
-        
-        We provide the following dynamics:
-        - [`simulate.nve`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html?highlight=nve#jax_md.simulate.nve) Constant energy simulation; numerically integrates Newton's laws directly.
-        - [`simulate.nvt_nose_hoover`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html?highlight=nvt_nose_hoover#jax_md.simulate.nvt_nose_hoover) Uses Nose-Hoover chain to simulate a constant temperature system.
-        - [`simulate.npt_nose_hoover`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html?highlight=nvp_nose_hoover#jax_md.simulate.nvp_nose_hoover) Uses Nose-Hoover chain to simulate a system at constant pressure and temperature.
-        - [`simulate.nvt_langevin`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html?highlight=nvt_langevin#jax_md.simulate.nvt_langevin) Simulates a system by numerically integrating the Langevin stochastic differential equation.
-        - [`simulate.hybrid_swap_mc`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html?highlight=hybrid_swap_mc#jax_md.simulate.hybrid_swap_mc) Alternates NVT dynamics with Monte-Carlo swapping moves to generate low energy glasses.
-        - [`simulate.brownian`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html?highlight=brownian#jax_md.simulate.brownian) Simulates brownian motion.
-        - [`minimize.gradient_descent`](https://jax-md.readthedocs.io/en/main/jax_md.minimize.html?highlight=gradient_descent#jax_md.minimize.gradient_descent) Minimizes a system using gradient descent.
-        - [`minimize.fire_descent`](https://jax-md.readthedocs.io/en/main/jax_md.minimize.html?highlight=fire_descent#jax_md.minimize.fire_descent) Minimizes a system using the fast inertial relaxation engine.
-        
-        Example:
-        
-        ```python
-        from jax_md import simulate
-        temperature = 1.0
-        dt = 1e-3
-        init, update = simulate.nvt_nose_hoover(energy_fn, shift_fn, dt, temperature)
-        state = init(key, R)
-        for _ in range(100):
-          state = update(state)
-        R = state.position
-        ```
-        
-        ## Spatial Partitioning ([`partition.py`](https://jax-md.readthedocs.io/en/main/jax_md.partition.html))
-        
-        In many applications, it is useful to construct spatial partitions of particles / objects in a simulation.
-        
-        We provide the following methods:
-        - [`partition.cell_list`](https://jax-md.readthedocs.io/en/main/jax_md.partition.html?highlight=cell_list#jax_md.partition.cell_list) Partitions objects (and metadata) into a grid of cells.
-        - [`partition.neighbor_list`](https://jax-md.readthedocs.io/en/main/jax_md.partition.html?highlight=neighbor_list#jax_md.partition.neighbor_list) Constructs a set of neighbors within some cutoff distance for each object in a simulation.
-        
-        Cell List Example:
-        ```python
-        from jax_md import partition
-        
-        cell_size = 5.0
-        capacity = 10
-        cell_list_fn = partition.cell_list(box_size, cell_size, capacity)
-        cell_list_data = cell_list_fn(R)
-        ```
-        
-        Neighbor List Example:
-        ```python
-        from jax_md import partition
-        
-        neighbor_list_fn = partition.neighbor_list(displacement_fn, box_size, cell_size)
-        neighbors = neighbor_list_fn.allocate(R) # Create a new neighbor list.
-        
-        # Do some simulating....
-        
-        neighbors = neighbors.update(R)  # Update the neighbor list without resizing.
-        if neighbors.did_buffer_overflow:  # Couldn't fit all the neighbors into the list.
-          neighbors = neighbor_list_fn.allocate(R)  # So create a new neighbor list.
-        ```
-        
-        There are three different formats of neighbor list supported: `Dense`, `Sparse`, and `OrderedSparse`. `Dense` neighbor lists store neighbors in an `(particle_count, neighbors_per_particle)` array, `Sparse` neighbor lists store neighbors in a `(2, total_neighbors)` array of pairs, `OrderedSparse` neighbor lists are like `Sparse` neighbor lists, but they only store pairs such that `i < j`.
-        
-        # Development
-        
-        JAX MD is under active development. We have very limited development resources and so we typically focus on adding features that will have high impact to researchers using JAX MD (including us). Please don't hesitate to open feature requests to help us guide development. We more than welcome contributions!
-        
-        ## Technical gotchas
-        
-        ### GPU
-        
-        You must follow [JAX's](https://www.github.com/google/jax/) GPU installation instructions to enable GPU support.
-        
-        
-        ### 64-bit precision
-        To enable 64-bit precision, set the respective JAX flag _before_ importing `jax_md` (see the JAX [guide](https://colab.research.google.com/github/google/jax/blob/main/notebooks/Common_Gotchas_in_JAX.ipynb#scrollTo=YTktlwTTMgFl)), for example:
-        
-        ```python
-        from jax.config import config
-        config.update("jax_enable_x64", True)
-        ```
-        
-        # Publications
-        
-        JAX MD has been used in the following publications. If you don't see your paper on the list, but you used JAX MD let us know and we'll add it to the list!
-        
-        1. [A Differentiable Neural-Network Force Field for Ionic Liquids. (J. Chem. Inf. Model. 2022)](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.1c01380)<br> H. Montes-Campos, J. Carrete, S. Bichelmaier, L. M. Varela, and G. K. H. Madsen
-        2. [Correlation Tracking: Using simulations to interpolate highly correlated particle tracks. (Phys. Rev. E. 2022)](https://journals.aps.org/pre/abstract/10.1103/PhysRevE.105.044608?ft=1)<br> E. M. King, Z. Wang, D. A. Weitz, F. Spaepen, and M. P. Brenner
-        3. [Optimal Control of Nonequilibrium Systems Through Automatic Differentiation.](https://arxiv.org/abs/2201.00098)<br> M. C. Engel, J. A. Smith, and M. P. Brenner
-        4. [Graph Neural Networks Accelerated Molecular Dynamics. (J. Chem. Phys. 2022)](https://aip.scitation.org/doi/10.1063/5.0083060)<br> Z. Li, K. Meidani, P. Yadav, and A. B. Farimani
-        5. [Gradients are Not All You Need.](https://arxiv.org/abs/2111.05803)<br> L. Metz, C. D. Freeman, S. S. Schoenholz, and T. Kachman
-        6. [Lagrangian Neural Network with Differential Symmetries and Relational Inductive Bias.](https://arxiv.org/abs/2110.03266)<br> R. Bhattoo, S. Ranu, and N. M. A. Krishnan
-        7. [Efficient and Modular Implicit Differentiation.](https://arxiv.org/abs/2105.15183)<br> M. Blondel, Q. Berthet, M. Cuturi, R. Frostig, S. Hoyer, F. Llinares-López, F. Pedregosa, and J.-P. Vert
-        8. [Learning neural network potentials from experimental data via Differentiable Trajectory Reweighting.<br>(Nature Communications 2021)](https://www.nature.com/articles/s41467-021-27241-4)<br> S. Thaler and J. Zavadlav
-        9. [Learn2Hop: Learned Optimization on Rough Landscapes. (ICML 2021)](http://proceedings.mlr.press/v139/merchant21a.html)<br> A. Merchant, L. Metz, S. S. Schoenholz, and E. D. Cubuk
-        10. [Designing self-assembling kinetics with differentiable statistical physics models. (PNAS 2021)](https://www.pnas.org/content/118/10/e2024083118.short)<br> C. P. Goodrich, E. M. King, S. S. Schoenholz, E. D. Cubuk, and  M. P. Brenner
-        
-        # Citation
-        
-        If you use the code in a publication, please cite the repo using the .bib,
-        
-        ```
-        @inproceedings{jaxmd2020,
-         author = {Schoenholz, Samuel S. and Cubuk, Ekin D.},
-         booktitle = {Advances in Neural Information Processing Systems},
-         publisher = {Curran Associates, Inc.},
-         title = {JAX M.D. A Framework for Differentiable Physics},
-         url = {https://papers.nips.cc/paper/2020/file/83d3d4b6c9579515e1679aca8cbc8033-Paper.pdf},
-         volume = {33},
-         year = {2020}
-        }
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSE_SHORT
+
+# JAX, M.D.
+
+### Accelerated, Differentiable, Molecular Dynamics
+[**Quickstart**](#getting-started) | [**Reference docs**](https://jax-md.readthedocs.io/en/main/) | [**Paper**](https://arxiv.org/pdf/1912.04232.pdf) | [**NeurIPS 2020**](https://neurips.cc/virtual/2020/public/poster_83d3d4b6c9579515e1679aca8cbc8033.html)
+
+![Build Status](https://github.com/google/jax-md/workflows/Build/badge.svg?branch=main) [![Coverage](https://codecov.io/gh/google/jax-md/branch/main/graph/badge.svg?token=JYQpbNyICv)](https://codecov.io/gh/google/jax-md) [![PyPI](https://img.shields.io/pypi/v/jax-md)](https://pypi.org/project/jax-md/) [![PyPI - License](https://img.shields.io/pypi/l/jax_md)](https://github.com/google/jax-md/blob/main/LICENSE)
+
+Molecular dynamics is a workhorse of modern computational condensed matter physics. It is frequently used to simulate materials to observe how small scale interactions can give rise to complex large-scale phenomenology. Most molecular dynamics packages (e.g. HOOMD Blue or LAMMPS) are complicated, specialized pieces of code that are many thousands of lines long. They typically involve significant code duplication to allow for running simulations on CPU and GPU. Additionally, large amounts of code is often devoted to taking derivatives of quantities to compute functions of interest (e.g. gradients of energies to compute forces).
+
+However, recent work in machine learning has led to significant software developments that might make it possible to write more concise molecular dynamics simulations that offer a range of benefits. Here we target JAX, which allows us to write python code that gets compiled to XLA and allows us to run on CPU, GPU, or TPU. Moreover, JAX allows us to take derivatives of python code. Thus, not only is this molecular dynamics simulation automatically hardware accelerated, it is also __end-to-end__ differentiable. This should allow for some interesting experiments that we're excited to explore.
+
+JAX, MD is a research project that is currently under development. Expect sharp edges and possibly some API breaking changes as we continue to support a broader set of simulations. JAX MD is a functional and data driven library. Data is stored in arrays or tuples of arrays and functions transform data from one state to another.
+
+### Getting Started
+
+For a video introducing JAX MD along with a [demo](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/talk_demo.ipynb), check out this talk from the Physics meets Machine Learning series:
+
+[![Science Meets ML Talk](https://img.youtube.com/vi/Bkm8tGET7-w/0.jpg)](https://www.youtube.com/watch?v=Bkm8tGET7-w)
+
+To get started playing around with JAX MD check out the following colab notebooks on Google Cloud without needing to install anything. For a very simple introduction, I would recommend the Minimization example. For an example of a bunch of the features of JAX MD, check out the JAX MD cookbook.
+
+- [JAX MD Cookbook](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/jax_md_cookbook.ipynb)
+- [Minimization](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/minimization.ipynb)
+- [NVE Simulation](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/nve_simulation.ipynb)
+- [NVT Simulation](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/nvt_simulation.ipynb)
+- [NPT Simulation](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/npt_simulation.ipynb)
+- [NVE with Neighbor Lists](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/nve_neighbor_list.ipynb)
+- [Custom Potentials](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/customizing_potentials_cookbook.ipynb)
+- [Neural Network Potentials](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/neural_networks.ipynb)
+- [Flocking](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/flocking.ipynb)
+- [Meta Optimization](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/meta_optimization.ipynb)
+- [Swap Monte Carlo (Cargese Summer School)](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/cargese_swap_mc.ipynb)
+- [Implicit Differentiation](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/implicit_differentiation.ipynb)
+- [Athermal Linear Elasticity](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/athermal_linear_elasticity.ipynb)
+- [Smash a Sand Castle](https://colab.research.google.com/github/google/jax-md/blob/main/notebooks/sand_castle.ipynb)
+
+You can install JAX MD locally with pip,
+```
+pip install jax-md --upgrade
+```
+If you want to build the latest version then you can grab the most recent version from head,
+```
+git clone https://github.com/google/jax-md
+pip install -e jax-md
+```
+
+# Overview
+
+We now summarize the main components of the library.
+
+## Spaces ([`space.py`](https://jax-md.readthedocs.io/en/main/jax_md.space.html))
+
+In general we must have a way of computing the pairwise distance between atoms. We must also have efficient strategies for moving atoms in some space that may or may not be globally isomorphic to R^N. For example, periodic boundary conditions are commonplace in simulations and must be respected. Spaces are defined as a pair of functions, `(displacement_fn, shift_fn)`. Given two points `displacement_fn(R_1, R_2)` computes the displacement vector between the two points. If you would like to compute displacement vectors between all pairs of points in a given `(N, dim)` matrix the function `space.map_product` appropriately vectorizes `displacement_fn`. It is often useful to define a metric instead of a displacement function in which case you can use the helper function `space.metric` to convert a displacement function to a metric function. Given a point and a shift `shift_fn(R, dR)` displaces the point `R` by an amount `dR`.
+
+The following spaces are currently supported:
+- [`space.free()`](https://jax-md.readthedocs.io/en/main/jax_md.space.html?highlight=free#jax_md.space.free) specifies a space with free boundary conditions.
+- [`space.periodic(box_size)`](https://jax-md.readthedocs.io/en/main/jax_md.space.html?highlight=periodic#jax_md.space.periodic) specifies a space with periodic boundary conditions of side length `box_size`.
+- [`space.periodic_general(box)`](https://jax-md.readthedocs.io/en/main/jax_md.space.html?highlight=periodic_general#jax_md.space.periodic_general) specifies a space as a periodic parellelopiped formed by transforming the unit cube by an affine transformation `box`.
+
+Example:
+
+```python
+from jax_md import space
+box_size = 25.0
+displacement_fn, shift_fn = space.periodic(box_size)
+```
+
+## Potential Energy ([`energy.py`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html))
+
+In the simplest case, molecular dynamics calculations are often based on a pair potential that is defined by a user. This then is used to compute a total energy whose negative gradient gives forces. One of the very nice things about JAX is that we get forces for free! The second part of the code is devoted to computing energies.
+
+We provide the following classical potentials:
+- [`energy.soft_sphere`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=soft_sphere#jax_md.energy.soft_sphere) a soft sphere whose energy increases as the overlap of the spheres to some power, `alpha`.
+- [`energy.lennard_jones`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=lennard_jones#jax_md.energy.lennard_jones) a standard 12-6 Lennard-Jones potential.
+- [`energy.morse`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=morse#jax_md.energy.morse) a morse potential.
+- [`energy.tersoff`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=tersoff#jax_md.energy.tersoff) the Tersoff potential for simulating semiconducting materials. Can load parameters from LAMMPS files.
+- [`energy.eam`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=eam#jax_md.energy.eam) embedded atom model potential with ability to load parameters from LAMMPS files.
+- [`energy.stillinger_weber`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=stillinger_weber#jax_md.energy.stillinger_weber) used to model Silicon-like systems.
+- [`energy.bks`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=bks#jax_md.energy.bks) Beest-Kramer-van Santen potential used to model silica.
+- [`energy.gupta`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=gupta#jax_md.energy.gupta) used to model gold nanoclusters.
+
+We also provide the following neural network potentials:
+- [`energy.behler_parrinello`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=behler_parrinello#jax_md.energy.behler_parrinello) a widely used fixed-feature neural network architecture for molecular systems.
+- [`energy.graph_network`](https://jax-md.readthedocs.io/en/main/jax_md.energy.html?highlight=graph_network#jax_md.energy.graph_network) a deep graph neural network designed for energy fitting.
+
+For finite-ranged potentials it is often useful to consider only interactions within a certain neighborhood. We include the `_neighbor_list` modifier to the above potentials that uses a list of neighbors (see below) for optimization.
+
+Example:
+
+```python
+import jax.numpy as np
+from jax import random
+from jax_md import energy, quantity
+N = 1000
+spatial_dimension = 2
+key = random.PRNGKey(0)
+R = random.uniform(key, (N, spatial_dimension), minval=0.0, maxval=1.0)
+energy_fn = energy.lennard_jones_pair(displacement_fn)
+print('E = {}'.format(energy_fn(R)))
+force_fn = quantity.force(energy_fn)
+print('Total Squared Force = {}'.format(np.sum(force_fn(R) ** 2)))
+```
+
+## Dynamics ([`simulate.py`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html), [`minimize.py`](https://jax-md.readthedocs.io/en/main/jax_md.minimize.html))
+
+Given an energy function and a system, there are a number of dynamics are useful to simulate. The simulation code is based on the structure of the optimizers found in JAX. In particular, each simulation function returns an initialization function and an update function. The initialization function takes a set of positions and creates the necessary dynamical state variables. The update function does a single step of dynamics to the dynamical state variables and returns an updated state.
+
+We include a several different kinds of dynamics. However, there is certainly room to add more for e.g. constant strain simulations.
+
+It is often desirable to find an energy minimum of the system. We provide two methods to do this. We provide simple gradient descent minimization. This is mostly for pedagogical purposes, since it often performs poorly. We additionally include the FIRE algorithm which often sees significantly faster convergence. Moreover a common experiment to run in the context of molecular dynamics is to simulate a system with a fixed volume and temperature.
+
+We provide the following dynamics:
+- [`simulate.nve`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html?highlight=nve#jax_md.simulate.nve) Constant energy simulation; numerically integrates Newton's laws directly.
+- [`simulate.nvt_nose_hoover`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html?highlight=nvt_nose_hoover#jax_md.simulate.nvt_nose_hoover) Uses Nose-Hoover chain to simulate a constant temperature system.
+- [`simulate.npt_nose_hoover`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html?highlight=nvp_nose_hoover#jax_md.simulate.nvp_nose_hoover) Uses Nose-Hoover chain to simulate a system at constant pressure and temperature.
+- [`simulate.nvt_langevin`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html?highlight=nvt_langevin#jax_md.simulate.nvt_langevin) Simulates a system by numerically integrating the Langevin stochastic differential equation.
+- [`simulate.hybrid_swap_mc`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html?highlight=hybrid_swap_mc#jax_md.simulate.hybrid_swap_mc) Alternates NVT dynamics with Monte-Carlo swapping moves to generate low energy glasses.
+- [`simulate.brownian`](https://jax-md.readthedocs.io/en/main/jax_md.simulate.html?highlight=brownian#jax_md.simulate.brownian) Simulates brownian motion.
+- [`minimize.gradient_descent`](https://jax-md.readthedocs.io/en/main/jax_md.minimize.html?highlight=gradient_descent#jax_md.minimize.gradient_descent) Minimizes a system using gradient descent.
+- [`minimize.fire_descent`](https://jax-md.readthedocs.io/en/main/jax_md.minimize.html?highlight=fire_descent#jax_md.minimize.fire_descent) Minimizes a system using the fast inertial relaxation engine.
+
+Example:
+
+```python
+from jax_md import simulate
+temperature = 1.0
+dt = 1e-3
+init, update = simulate.nvt_nose_hoover(energy_fn, shift_fn, dt, temperature)
+state = init(key, R)
+for _ in range(100):
+  state = update(state)
+R = state.position
+```
+
+## Spatial Partitioning ([`partition.py`](https://jax-md.readthedocs.io/en/main/jax_md.partition.html))
+
+In many applications, it is useful to construct spatial partitions of particles / objects in a simulation.
+
+We provide the following methods:
+- [`partition.cell_list`](https://jax-md.readthedocs.io/en/main/jax_md.partition.html?highlight=cell_list#jax_md.partition.cell_list) Partitions objects (and metadata) into a grid of cells.
+- [`partition.neighbor_list`](https://jax-md.readthedocs.io/en/main/jax_md.partition.html?highlight=neighbor_list#jax_md.partition.neighbor_list) Constructs a set of neighbors within some cutoff distance for each object in a simulation.
+
+Cell List Example:
+```python
+from jax_md import partition
+
+cell_size = 5.0
+capacity = 10
+cell_list_fn = partition.cell_list(box_size, cell_size, capacity)
+cell_list_data = cell_list_fn(R)
+```
+
+Neighbor List Example:
+```python
+from jax_md import partition
+
+neighbor_list_fn = partition.neighbor_list(displacement_fn, box_size, cell_size)
+neighbors = neighbor_list_fn.allocate(R) # Create a new neighbor list.
+
+# Do some simulating....
+
+neighbors = neighbors.update(R)  # Update the neighbor list without resizing.
+if neighbors.did_buffer_overflow:  # Couldn't fit all the neighbors into the list.
+  neighbors = neighbor_list_fn.allocate(R)  # So create a new neighbor list.
+```
+
+There are three different formats of neighbor list supported: `Dense`, `Sparse`, and `OrderedSparse`. `Dense` neighbor lists store neighbors in an `(particle_count, neighbors_per_particle)` array, `Sparse` neighbor lists store neighbors in a `(2, total_neighbors)` array of pairs, `OrderedSparse` neighbor lists are like `Sparse` neighbor lists, but they only store pairs such that `i < j`.
+
+# Development
+
+JAX MD is under active development. We have very limited development resources and so we typically focus on adding features that will have high impact to researchers using JAX MD (including us). Please don't hesitate to open feature requests to help us guide development. We more than welcome contributions!
+
+## Technical gotchas
+
+### GPU
+
+You must follow [JAX's](https://www.github.com/google/jax/) GPU installation instructions to enable GPU support.
+
+
+### 64-bit precision
+To enable 64-bit precision, set the respective JAX flag _before_ importing `jax_md` (see the JAX [guide](https://colab.research.google.com/github/google/jax/blob/main/notebooks/Common_Gotchas_in_JAX.ipynb#scrollTo=YTktlwTTMgFl)), for example:
+
+```python
+from jax.config import config
+config.update("jax_enable_x64", True)
+```
+
+# Publications
+
+JAX MD has been used in the following publications. If you don't see your paper on the list, but you used JAX MD let us know and we'll add it to the list!
+
+1. [A Differentiable Neural-Network Force Field for Ionic Liquids. (J. Chem. Inf. Model. 2022)](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.1c01380)<br> H. Montes-Campos, J. Carrete, S. Bichelmaier, L. M. Varela, and G. K. H. Madsen
+2. [Correlation Tracking: Using simulations to interpolate highly correlated particle tracks. (Phys. Rev. E. 2022)](https://journals.aps.org/pre/abstract/10.1103/PhysRevE.105.044608?ft=1)<br> E. M. King, Z. Wang, D. A. Weitz, F. Spaepen, and M. P. Brenner
+3. [Optimal Control of Nonequilibrium Systems Through Automatic Differentiation.](https://arxiv.org/abs/2201.00098)<br> M. C. Engel, J. A. Smith, and M. P. Brenner
+4. [Graph Neural Networks Accelerated Molecular Dynamics. (J. Chem. Phys. 2022)](https://aip.scitation.org/doi/10.1063/5.0083060)<br> Z. Li, K. Meidani, P. Yadav, and A. B. Farimani
+5. [Gradients are Not All You Need.](https://arxiv.org/abs/2111.05803)<br> L. Metz, C. D. Freeman, S. S. Schoenholz, and T. Kachman
+6. [Lagrangian Neural Network with Differential Symmetries and Relational Inductive Bias.](https://arxiv.org/abs/2110.03266)<br> R. Bhattoo, S. Ranu, and N. M. A. Krishnan
+7. [Efficient and Modular Implicit Differentiation.](https://arxiv.org/abs/2105.15183)<br> M. Blondel, Q. Berthet, M. Cuturi, R. Frostig, S. Hoyer, F. Llinares-López, F. Pedregosa, and J.-P. Vert
+8. [Learning neural network potentials from experimental data via Differentiable Trajectory Reweighting.<br>(Nature Communications 2021)](https://www.nature.com/articles/s41467-021-27241-4)<br> S. Thaler and J. Zavadlav
+9. [Learn2Hop: Learned Optimization on Rough Landscapes. (ICML 2021)](http://proceedings.mlr.press/v139/merchant21a.html)<br> A. Merchant, L. Metz, S. S. Schoenholz, and E. D. Cubuk
+10. [Designing self-assembling kinetics with differentiable statistical physics models. (PNAS 2021)](https://www.pnas.org/content/118/10/e2024083118.short)<br> C. P. Goodrich, E. M. King, S. S. Schoenholz, E. D. Cubuk, and  M. P. Brenner
+
+# Citation
+
+If you use the code in a publication, please cite the repo using the .bib,
+
+```
+@inproceedings{jaxmd2020,
+ author = {Schoenholz, Samuel S. and Cubuk, Ekin D.},
+ booktitle = {Advances in Neural Information Processing Systems},
+ publisher = {Curran Associates, Inc.},
+ title = {JAX M.D. A Framework for Differentiable Physics},
+ url = {https://papers.nips.cc/paper/2020/file/83d3d4b6c9579515e1679aca8cbc8033-Paper.pdf},
+ volume = {33},
+ year = {2020}
+}
+```
```

### Comparing `jax-md-0.2.5/jax_md.egg-info/SOURCES.txt` & `jax-md-0.2.6/jax_md.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+LICENSE
+LICENSE_SHORT
 README.md
 setup.cfg
 setup.py
 jax_md/__init__.py
 jax_md/dataclasses.py
 jax_md/elasticity.py
 jax_md/energy.py
@@ -13,14 +15,15 @@
 jax_md/quantity.py
 jax_md/rigid_body.py
 jax_md/simulate.py
 jax_md/smap.py
 jax_md/space.py
 jax_md/test_util.py
 jax_md/tpu.py
+jax_md/units.py
 jax_md/util.py
 jax_md.egg-info/PKG-INFO
 jax_md.egg-info/SOURCES.txt
 jax_md.egg-info/dependency_links.txt
 jax_md.egg-info/requires.txt
 jax_md.egg-info/top_level.txt
 jax_md/_nn/__init__.py
```

### Comparing `jax-md-0.2.5/setup.py` & `jax-md-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     'e3nn-jax',
     'dm-haiku',
     'optax',
 ]
 
 setuptools.setup(
     name='jax-md',
-    version='0.2.5',
+    version='0.2.6',
     license='Apache 2.0',
     author='Google',
     author_email='jax-md-dev@google.com',
     install_requires=INSTALL_REQUIRES,
     url='https://github.com/google/jax-md',
     packages=setuptools.find_packages(),
     download_url = "https://pypi.org/project/jax-md/",
```


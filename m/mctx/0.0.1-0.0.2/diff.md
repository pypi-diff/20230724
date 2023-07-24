# Comparing `tmp/mctx-0.0.1.tar.gz` & `tmp/mctx-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mctx-0.0.1.tar", last modified: Fri Mar  4 09:44:39 2022, max compression
+gzip compressed data, was "mctx-0.0.2.tar", last modified: Tue Jul 26 10:19:22 2022, max compression
```

## Comparing `mctx-0.0.1.tar` & `mctx-0.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 danihelka (236193) primarygroup (89939)        0 2022-03-04 09:44:39.761425 mctx-0.0.1/
--rw-r--r--   0 danihelka (236193) primarygroup (89939)    11358 2022-03-04 09:44:14.000000 mctx-0.0.1/LICENSE
--rw-r--r--   0 danihelka (236193) primarygroup (89939)       79 2022-03-04 09:44:14.000000 mctx-0.0.1/MANIFEST.in
--rw-r--r--   0 danihelka (236193) primarygroup (89939)     6941 2022-03-04 09:44:39.757425 mctx-0.0.1/PKG-INFO
--rw-r--r--   0 danihelka (236193) primarygroup (89939)     6170 2022-03-04 09:44:14.000000 mctx-0.0.1/README.md
-drwxr-xr-x   0 danihelka (236193) primarygroup (89939)        0 2022-03-04 09:44:39.757425 mctx-0.0.1/examples/
--rw-r--r--   0 danihelka (236193) primarygroup (89939)     5835 2022-03-04 09:44:14.000000 mctx-0.0.1/examples/policy_improvement_demo.py
--rw-r--r--   0 danihelka (236193) primarygroup (89939)     7051 2022-03-04 09:44:14.000000 mctx-0.0.1/examples/visualization_demo.py
-drwxr-xr-x   0 danihelka (236193) primarygroup (89939)        0 2022-03-04 09:44:39.757425 mctx-0.0.1/mctx/
--rw-r--r--   0 danihelka (236193) primarygroup (89939)     2421 2022-03-04 09:44:14.000000 mctx-0.0.1/mctx/__init__.py
-drwxr-xr-x   0 danihelka (236193) primarygroup (89939)        0 2022-03-04 09:44:39.757425 mctx-0.0.1/mctx/_src/
--rw-r--r--   0 danihelka (236193) primarygroup (89939)      696 2022-03-04 09:44:14.000000 mctx-0.0.1/mctx/_src/__init__.py
--rw-r--r--   0 danihelka (236193) primarygroup (89939)     8592 2022-03-04 09:44:14.000000 mctx-0.0.1/mctx/_src/action_selection.py
--rw-r--r--   0 danihelka (236193) primarygroup (89939)     3430 2022-03-04 09:44:14.000000 mctx-0.0.1/mctx/_src/base.py
--rw-r--r--   0 danihelka (236193) primarygroup (89939)    10759 2022-03-04 09:44:14.000000 mctx-0.0.1/mctx/_src/policies.py
--rw-r--r--   0 danihelka (236193) primarygroup (89939)     7053 2022-03-04 09:44:14.000000 mctx-0.0.1/mctx/_src/qtransforms.py
--rw-r--r--   0 danihelka (236193) primarygroup (89939)    14486 2022-03-04 09:44:14.000000 mctx-0.0.1/mctx/_src/search.py
--rw-r--r--   0 danihelka (236193) primarygroup (89939)     3414 2022-03-04 09:44:14.000000 mctx-0.0.1/mctx/_src/seq_halving.py
-drwxr-xr-x   0 danihelka (236193) primarygroup (89939)        0 2022-03-04 09:44:39.757425 mctx-0.0.1/mctx/_src/tests/
--rw-r--r--   0 danihelka (236193) primarygroup (89939)     1393 2022-03-04 09:44:14.000000 mctx-0.0.1/mctx/_src/tests/mctx_test.py
--rw-r--r--   0 danihelka (236193) primarygroup (89939)    10164 2022-03-04 09:44:14.000000 mctx-0.0.1/mctx/_src/tests/policies_test.py
--rw-r--r--   0 danihelka (236193) primarygroup (89939)     1627 2022-03-04 09:44:14.000000 mctx-0.0.1/mctx/_src/tests/qtransforms_test.py
--rw-r--r--   0 danihelka (236193) primarygroup (89939)     4021 2022-03-04 09:44:14.000000 mctx-0.0.1/mctx/_src/tests/seq_halving_test.py
--rw-r--r--   0 danihelka (236193) primarygroup (89939)     7560 2022-03-04 09:44:14.000000 mctx-0.0.1/mctx/_src/tests/tree_test.py
--rw-r--r--   0 danihelka (236193) primarygroup (89939)     5371 2022-03-04 09:44:14.000000 mctx-0.0.1/mctx/_src/tree.py
--rw-r--r--   0 danihelka (236193) primarygroup (89939)        0 2022-03-04 09:44:14.000000 mctx-0.0.1/mctx/py.typed
-drwxr-xr-x   0 danihelka (236193) primarygroup (89939)        0 2022-03-04 09:44:39.757425 mctx-0.0.1/mctx.egg-info/
--rw-r--r--   0 danihelka (236193) primarygroup (89939)     6941 2022-03-04 09:44:39.000000 mctx-0.0.1/mctx.egg-info/PKG-INFO
--rw-r--r--   0 danihelka (236193) primarygroup (89939)      749 2022-03-04 09:44:39.000000 mctx-0.0.1/mctx.egg-info/SOURCES.txt
--rw-r--r--   0 danihelka (236193) primarygroup (89939)        1 2022-03-04 09:44:39.000000 mctx-0.0.1/mctx.egg-info/dependency_links.txt
--rw-r--r--   0 danihelka (236193) primarygroup (89939)        1 2022-03-04 09:44:39.000000 mctx-0.0.1/mctx.egg-info/not-zip-safe
--rw-r--r--   0 danihelka (236193) primarygroup (89939)       39 2022-03-04 09:44:39.000000 mctx-0.0.1/mctx.egg-info/requires.txt
--rw-r--r--   0 danihelka (236193) primarygroup (89939)       27 2022-03-04 09:44:39.000000 mctx-0.0.1/mctx.egg-info/top_level.txt
-drwxr-xr-x   0 danihelka (236193) primarygroup (89939)        0 2022-03-04 09:44:39.757425 mctx-0.0.1/requirements/
--rw-r--r--   0 danihelka (236193) primarygroup (89939)       29 2022-03-04 09:44:14.000000 mctx-0.0.1/requirements/requirements-test.txt
--rw-r--r--   0 danihelka (236193) primarygroup (89939)       39 2022-03-04 09:44:14.000000 mctx-0.0.1/requirements/requirements.txt
--rw-r--r--   0 danihelka (236193) primarygroup (89939)       31 2022-03-04 09:44:14.000000 mctx-0.0.1/requirements/requirements_examples.txt
--rw-r--r--   0 danihelka (236193) primarygroup (89939)       38 2022-03-04 09:44:39.761425 mctx-0.0.1/setup.cfg
--rw-r--r--   0 danihelka (236193) primarygroup (89939)     2629 2022-03-04 09:44:14.000000 mctx-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 10:19:22.246559 mctx-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-07-26 10:19:08.000000 mctx-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-07-26 10:19:08.000000 mctx-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     7296 2022-07-26 10:19:22.246559 mctx-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6525 2022-07-26 10:19:08.000000 mctx-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 10:19:22.242559 mctx-0.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     5835 2022-07-26 10:19:08.000000 mctx-0.0.2/examples/policy_improvement_demo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7404 2022-07-26 10:19:08.000000 mctx-0.0.2/examples/visualization_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 10:19:22.242559 mctx-0.0.2/mctx/
+-rw-r--r--   0 runner    (1001) docker     (121)     2527 2022-07-26 10:19:08.000000 mctx-0.0.2/mctx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 10:19:22.246559 mctx-0.0.2/mctx/_src/
+-rw-r--r--   0 runner    (1001) docker     (121)      696 2022-07-26 10:19:08.000000 mctx-0.0.2/mctx/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8624 2022-07-26 10:19:08.000000 mctx-0.0.2/mctx/_src/action_selection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3383 2022-07-26 10:19:08.000000 mctx-0.0.2/mctx/_src/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11183 2022-07-26 10:19:08.000000 mctx-0.0.2/mctx/_src/policies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7087 2022-07-26 10:19:08.000000 mctx-0.0.2/mctx/_src/qtransforms.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14695 2022-07-26 10:19:08.000000 mctx-0.0.2/mctx/_src/search.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3414 2022-07-26 10:19:08.000000 mctx-0.0.2/mctx/_src/seq_halving.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 10:19:22.246559 mctx-0.0.2/mctx/_src/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1393 2022-07-26 10:19:08.000000 mctx-0.0.2/mctx/_src/tests/mctx_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10164 2022-07-26 10:19:08.000000 mctx-0.0.2/mctx/_src/tests/policies_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2133 2022-07-26 10:19:08.000000 mctx-0.0.2/mctx/_src/tests/qtransforms_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4021 2022-07-26 10:19:08.000000 mctx-0.0.2/mctx/_src/tests/seq_halving_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7560 2022-07-26 10:19:08.000000 mctx-0.0.2/mctx/_src/tests/tree_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5381 2022-07-26 10:19:08.000000 mctx-0.0.2/mctx/_src/tree.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-26 10:19:08.000000 mctx-0.0.2/mctx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 10:19:22.242559 mctx-0.0.2/mctx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     7296 2022-07-26 10:19:22.000000 mctx-0.0.2/mctx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      749 2022-07-26 10:19:22.000000 mctx-0.0.2/mctx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-26 10:19:22.000000 mctx-0.0.2/mctx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-26 10:19:22.000000 mctx-0.0.2/mctx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-07-26 10:19:22.000000 mctx-0.0.2/mctx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-07-26 10:19:22.000000 mctx-0.0.2/mctx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-26 10:19:22.246559 mctx-0.0.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-07-26 10:19:08.000000 mctx-0.0.2/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-07-26 10:19:08.000000 mctx-0.0.2/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-07-26 10:19:08.000000 mctx-0.0.2/requirements/requirements_examples.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-26 10:19:22.246559 mctx-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2629 2022-07-26 10:19:08.000000 mctx-0.0.2/setup.py
```

### Comparing `mctx-0.0.1/LICENSE` & `mctx-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mctx-0.0.1/PKG-INFO` & `mctx-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mctx
-Version: 0.0.1
+Version: 0.0.2
 Summary: Monte Carlo tree search in JAX.
 Home-page: https://github.com/deepmind/mctx
 Author: DeepMind
 Author-email: mctx-dev@google.com
 License: Apache 2.0
 Keywords: jax planning reinforcement-learning python machine learning
 Platform: UNKNOWN
@@ -29,22 +29,25 @@
 speed up, the implementation fully supports JIT-compilation. Search algorithms
 in Mctx are defined for and operate on batches of inputs, in parallel. This
 allows to make the most of the accelerators and enables the algorithms to work
 with large learned environment models parameterized by deep neural networks.
 
 ## Installation
 
-Mctx can be installed with `pip` directly from github, with the following command:
+You can install the latest released version of Mctx from PyPI via:
 
-`pip install git+git://github.com/deepmind/mctx.git`
-
-or from PyPI:
+```sh
+pip install mctx
+```
 
-`pip install mctx`
+or you can install the latest development version from GitHub:
 
+```sh
+pip install git+https://github.com/deepmind/mctx.git
+```
 
 ## Motivation
 
 Learning and search have been important topics since the early days of AI
 research. In the words of Rich Sutton: *One thing that should be learned [...]
 is the great power of general purpose methods, of methods that continue to scale
 with increased computation even as the available computation becomes very great.
@@ -106,15 +109,15 @@
 The dynamics environment model needs to be specified by a `recurrent_fn`.
 A `recurrent_fn(params, rng_key, action, embedding)` call takes an `action` and
 a state `embedding`. The call should return a tuple `(recurrent_fn_output,
 new_embedding)` with a `RecurrentFnOutput` and the embedding of the next state.
 The `RecurrentFnOutput` contains the `reward` and `discount` for the transition,
 and `prior_logits` and `value` for the new state.
 
-In [examples/visualization_demo.py](https://github.com/deepmind/mctx/blob/master/examples/visualization_demo.py)
+In [examples/visualization_demo.py](https://github.com/deepmind/mctx/blob/main/examples/visualization_demo.py)
 you can see calls to a policy:
 
 ```python
 policy_output = mctx.gumbel_muzero_policy(params, rng_key, root, recurrent_fn,
                                           num_simulations=32)
 ```
 
@@ -123,15 +126,25 @@
 `policy_output.action_weights` contain targets usable to train the policy
 probabilities.
 
 We recommend to use the `gumbel_muzero_policy`.
 [Gumbel MuZero](https://openreview.net/forum?id=bERaNdoegnO) guarantees a policy
 improvement if the action values are correctly evaluated. The policy improvement
 is demonstrated in
-[examples/policy_improvement_demo.py](https://github.com/deepmind/mctx/blob/master/examples/policy_improvement_demo.py).
+[examples/policy_improvement_demo.py](https://github.com/deepmind/mctx/blob/main/examples/policy_improvement_demo.py).
+
+### Example projects
+The following projects demonstrate the Mctx usage:
+
+- [Basic Learning Demo with Mctx](https://github.com/kenjyoung/mctx_learning_demo)
+... AlphaZero on random mazes.
+- [a0-jax](https://github.com/NTT123/a0-jax) ... AlphaZero on Connect Four,
+Gomoku, and Go.
+
+Tell us about your project.
 
 ## Citing Mctx
 
 This is not an officially supported Google product. Mctx is part of the
 [DeepMind JAX Ecosystem], to cite Mctx please use the [DeepMind JAX Ecosystem
 citation].
```

### Comparing `mctx-0.0.1/README.md` & `mctx-0.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -8,22 +8,25 @@
 speed up, the implementation fully supports JIT-compilation. Search algorithms
 in Mctx are defined for and operate on batches of inputs, in parallel. This
 allows to make the most of the accelerators and enables the algorithms to work
 with large learned environment models parameterized by deep neural networks.
 
 ## Installation
 
-Mctx can be installed with `pip` directly from github, with the following command:
+You can install the latest released version of Mctx from PyPI via:
 
-`pip install git+git://github.com/deepmind/mctx.git`
-
-or from PyPI:
+```sh
+pip install mctx
+```
 
-`pip install mctx`
+or you can install the latest development version from GitHub:
 
+```sh
+pip install git+https://github.com/deepmind/mctx.git
+```
 
 ## Motivation
 
 Learning and search have been important topics since the early days of AI
 research. In the words of Rich Sutton: *One thing that should be learned [...]
 is the great power of general purpose methods, of methods that continue to scale
 with increased computation even as the available computation becomes very great.
@@ -85,15 +88,15 @@
 The dynamics environment model needs to be specified by a `recurrent_fn`.
 A `recurrent_fn(params, rng_key, action, embedding)` call takes an `action` and
 a state `embedding`. The call should return a tuple `(recurrent_fn_output,
 new_embedding)` with a `RecurrentFnOutput` and the embedding of the next state.
 The `RecurrentFnOutput` contains the `reward` and `discount` for the transition,
 and `prior_logits` and `value` for the new state.
 
-In [examples/visualization_demo.py](https://github.com/deepmind/mctx/blob/master/examples/visualization_demo.py)
+In [examples/visualization_demo.py](https://github.com/deepmind/mctx/blob/main/examples/visualization_demo.py)
 you can see calls to a policy:
 
 ```python
 policy_output = mctx.gumbel_muzero_policy(params, rng_key, root, recurrent_fn,
                                           num_simulations=32)
 ```
 
@@ -102,15 +105,25 @@
 `policy_output.action_weights` contain targets usable to train the policy
 probabilities.
 
 We recommend to use the `gumbel_muzero_policy`.
 [Gumbel MuZero](https://openreview.net/forum?id=bERaNdoegnO) guarantees a policy
 improvement if the action values are correctly evaluated. The policy improvement
 is demonstrated in
-[examples/policy_improvement_demo.py](https://github.com/deepmind/mctx/blob/master/examples/policy_improvement_demo.py).
+[examples/policy_improvement_demo.py](https://github.com/deepmind/mctx/blob/main/examples/policy_improvement_demo.py).
+
+### Example projects
+The following projects demonstrate the Mctx usage:
+
+- [Basic Learning Demo with Mctx](https://github.com/kenjyoung/mctx_learning_demo)
+... AlphaZero on random mazes.
+- [a0-jax](https://github.com/NTT123/a0-jax) ... AlphaZero on Connect Four,
+Gomoku, and Go.
+
+Tell us about your project.
 
 ## Citing Mctx
 
 This is not an officially supported Google product. Mctx is part of the
 [DeepMind JAX Ecosystem], to cite Mctx please use the [DeepMind JAX Ecosystem
 citation].
```

### Comparing `mctx-0.0.1/examples/policy_improvement_demo.py` & `mctx-0.0.2/examples/policy_improvement_demo.py`

 * *Files identical despite different names*

### Comparing `mctx-0.0.1/examples/visualization_demo.py` & `mctx-0.0.2/examples/visualization_demo.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,15 +119,15 @@
       [0, 0, 0, 0],
       [0, 0, 0, 0],
       [10, 0, 20, 0],
   ], dtype=jnp.float32)
   num_states = rewards.shape[0]
   # The discount for each (s, a) pair.
   discounts = jnp.where(transition_matrix > 0, 1.0, 0.0)
-  # Using an optimistic initial values to encourage exploration.
+  # Using optimistic initial values to encourage exploration.
   values = jnp.full([num_states], 15.0)
   # The prior policies for each state.
   all_prior_logits = jnp.zeros_like(rewards)
   root, recurrent_fn = _make_batched_env_model(
       # Using batch_size=2 to test the batched search.
       batch_size=2,
       transition_matrix=transition_matrix,
@@ -188,15 +188,22 @@
 
 
 def main(_):
   rng_key = jax.random.PRNGKey(FLAGS.seed)
   jitted_run_demo = jax.jit(_run_demo)
   print("Starting search.")
   policy_output = jitted_run_demo(rng_key)
-  print("Selected action:", policy_output.action[0])
+  batch_index = 0
+  selected_action = policy_output.action[batch_index]
+  q_value = policy_output.search_tree.summary().qvalues[
+      batch_index, selected_action]
+  print("Selected action:", selected_action)
+  # To estimate the value of the root state, use the Q-value of the selected
+  # action. The Q-value is not affected by the exploration at the root node.
+  print("Selected action Q-value:", q_value)
   graph = convert_tree_to_graph(policy_output.search_tree)
   print("Saving tree diagram to:", FLAGS.output_file)
   graph.draw(FLAGS.output_file, prog="dot")
 
 
 if __name__ == "__main__":
   app.run(main)
```

### Comparing `mctx-0.0.1/mctx/__init__.py` & `mctx-0.0.2/mctx/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,32 +15,36 @@
 """Mctx: Monte Carlo tree search in JAX."""
 
 from mctx._src.action_selection import gumbel_muzero_interior_action_selection
 from mctx._src.action_selection import gumbel_muzero_root_action_selection
 from mctx._src.action_selection import GumbelMuZeroExtraData
 from mctx._src.action_selection import muzero_action_selection
 from mctx._src.base import InteriorActionSelectionFn
+from mctx._src.base import LoopFn
 from mctx._src.base import PolicyOutput
+from mctx._src.base import RecurrentFn
 from mctx._src.base import RecurrentFnOutput
 from mctx._src.base import RootActionSelectionFn
 from mctx._src.base import RootFnOutput
 from mctx._src.policies import gumbel_muzero_policy
 from mctx._src.policies import muzero_policy
 from mctx._src.qtransforms import qtransform_by_min_max
 from mctx._src.qtransforms import qtransform_by_parent_and_siblings
 from mctx._src.qtransforms import qtransform_completed_by_mix_value
 from mctx._src.search import search
 from mctx._src.tree import Tree
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 __all__ = (
     "GumbelMuZeroExtraData",
     "InteriorActionSelectionFn",
+    "LoopFn",
     "PolicyOutput",
+    "RecurrentFn",
     "RecurrentFnOutput",
     "RootActionSelectionFn",
     "RootFnOutput",
     "Tree",
     "gumbel_muzero_interior_action_selection",
     "gumbel_muzero_policy",
     "gumbel_muzero_root_action_selection",
```

### Comparing `mctx-0.0.1/mctx/_src/__init__.py` & `mctx-0.0.2/mctx/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `mctx-0.0.1/mctx/_src/action_selection.py` & `mctx-0.0.2/mctx/_src/action_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
 @chex.dataclass(frozen=True)
 class GumbelMuZeroExtraData:
   """Extra data for Gumbel MuZero search."""
   root_gumbel: chex.Array
 
 
-GumbelMuZeroExtraDataType = TypeVar(
+GumbelMuZeroExtraDataType = TypeVar(  # pylint: disable=invalid-name
     "GumbelMuZeroExtraDataType", bound=GumbelMuZeroExtraData)
 
 
 def gumbel_muzero_root_action_selection(
     rng_key: chex.PRNGKey,
     tree: tree_lib.Tree[GumbelMuZeroExtraDataType],
     node_index: chex.Numeric,
```

### Comparing `mctx-0.0.1/mctx/_src/base.py` & `mctx-0.0.2/mctx/_src/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,42 +49,40 @@
 Action = chex.Array
 RecurrentState = Any
 RecurrentFn = Callable[
     [Params, chex.PRNGKey, Action, RecurrentState],
     Tuple[RecurrentFnOutput, RecurrentState]]
 
 
-# The search takes as input an initial set of predictions made directly
-# from the raw data. These predictions are made by a `RootFn` with signature:
 @chex.dataclass(frozen=True)
 class RootFnOutput:
   """The output of a representation network.
 
   prior_logits: `[B, num_actions]` the logits produced by a policy network.
   value: `[B]` an approximate value of the current state.
   embedding: `[B, ...]` the inputs to the next `recurrent_fn` call.
   """
   prior_logits: chex.Array
   value: chex.Array
   embedding: RecurrentState
 
 
-RawData = Any
-RootFn = Callable[[Params, chex.PRNGKey, RawData], RootFnOutput]
-
-
 # Action selection functions specify how to pick nodes to expand in the tree.
 NodeIndices = chex.Array
 Depth = chex.Array
 RootActionSelectionFn = Callable[
     [chex.PRNGKey, tree.Tree, NodeIndices], chex.Array]
 InteriorActionSelectionFn = Callable[
     [chex.PRNGKey, tree.Tree, NodeIndices, Depth],
     chex.Array]
 QTransform = Callable[[tree.Tree, chex.Array], chex.Array]
+# LoopFn has the same interface as jax.lax.fori_loop.
+LoopFn = Callable[
+    [int, int, Callable[[Any, Any], Any], Tuple[chex.PRNGKey, tree.Tree]],
+    Tuple[chex.PRNGKey, tree.Tree]]
 
 T = TypeVar("T")
 
 
 @chex.dataclass(frozen=True)
 class PolicyOutput(Generic[T]):
   """The output of a policy.
```

### Comparing `mctx-0.0.1/mctx/_src/policies.py` & `mctx-0.0.2/mctx/_src/policies.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     params: base.Params,
     rng_key: chex.PRNGKey,
     root: base.RootFnOutput,
     recurrent_fn: base.RecurrentFn,
     num_simulations: int,
     invalid_actions: Optional[chex.Array] = None,
     max_depth: Optional[int] = None,
+    loop_fn: base.LoopFn = jax.lax.fori_loop,
     *,
     qtransform: base.QTransform = qtransforms.qtransform_by_parent_and_siblings,
     dirichlet_fraction: chex.Numeric = 0.25,
     dirichlet_alpha: chex.Numeric = 0.3,
     pb_c_init: chex.Numeric = 1.25,
     pb_c_base: chex.Numeric = 19652,
     temperature: chex.Numeric = 1.0) -> base.PolicyOutput[None]:
@@ -56,14 +57,16 @@
       actions retrieved by the simulation step, which takes as args
       `(params, rng_key, action, embedding)` and returns a `RecurrentFnOutput`
       and the new state embedding. The `rng_key` argument is consumed.
     num_simulations: the number of simulations.
     invalid_actions: a mask with invalid actions. Invalid actions
       have ones, valid actions have zeros in the mask. Shape `[B, num_actions]`.
     max_depth: maximum search tree depth allowed during simulation.
+    loop_fn: Function used to run the simulations. It may be required to pass
+      hk.fori_loop if using this function inside a Haiku module.
     qtransform: function to obtain completed Q-values for a node.
     dirichlet_fraction: float from 0 to 1 interpolating between using only the
       prior policy or just the Dirichlet noise.
     dirichlet_alpha: concentration parameter to parametrize the Dirichlet
       distribution.
     pb_c_init: constant c_1 in the PUCT formula.
     pb_c_base: constant c_2 in the PUCT formula.
@@ -100,15 +103,16 @@
       rng_key=search_rng_key,
       root=root,
       recurrent_fn=recurrent_fn,
       root_action_selection_fn=root_action_selection_fn,
       interior_action_selection_fn=interior_action_selection_fn,
       num_simulations=num_simulations,
       max_depth=max_depth,
-      invalid_actions=invalid_actions)
+      invalid_actions=invalid_actions,
+      loop_fn=loop_fn)
 
   # Sampling the proposed action proportionally to the visit counts.
   summary = search_tree.summary()
   action_weights = summary.visit_probs
   action_logits = _apply_temperature(
       _get_logits_from_probs(action_weights), temperature)
   action = jax.random.categorical(rng_key, action_logits)
@@ -122,14 +126,15 @@
     params: base.Params,
     rng_key: chex.PRNGKey,
     root: base.RootFnOutput,
     recurrent_fn: base.RecurrentFn,
     num_simulations: int,
     invalid_actions: Optional[chex.Array] = None,
     max_depth: Optional[int] = None,
+    loop_fn: base.LoopFn = jax.lax.fori_loop,
     *,
     qtransform: base.QTransform = qtransforms.qtransform_completed_by_mix_value,
     max_num_considered_actions: int = 16,
     gumbel_scale: chex.Numeric = 1.,
 ) -> base.PolicyOutput[action_selection.GumbelMuZeroExtraData]:
   """Runs Gumbel MuZero search and returns the `PolicyOutput`.
 
@@ -153,14 +158,16 @@
       actions retrieved by the simulation step, which takes as args
       `(params, rng_key, action, embedding)` and returns a `RecurrentFnOutput`
       and the new state embedding. The `rng_key` argument is consumed.
     num_simulations: the number of simulations.
     invalid_actions: a mask with invalid actions. Invalid actions
       have ones, valid actions have zeros in the mask. Shape `[B, num_actions]`.
     max_depth: maximum search tree depth allowed during simulation.
+    loop_fn: Function used to run the simulations. It may be required to pass
+      hk.fori_loop if using this function inside a Haiku module.
     qtransform: function to obtain completed Q-values for a node.
     max_num_considered_actions: the maximum number of actions expanded at the
       root node. A smaller number of actions will be expanded if the number of
       valid actions is smaller.
     gumbel_scale: scale for the Gumbel noise. Evalution on perfect-information
       games can use gumbel_scale=0.0.
 
@@ -193,15 +200,16 @@
       interior_action_selection_fn=functools.partial(
           action_selection.gumbel_muzero_interior_action_selection,
           qtransform=qtransform,
       ),
       num_simulations=num_simulations,
       max_depth=max_depth,
       invalid_actions=invalid_actions,
-      extra_data=extra_data)
+      extra_data=extra_data,
+      loop_fn=loop_fn)
   summary = search_tree.summary()
 
   # Acting with the best action from the most visited actions.
   # The "best" action has the highest `gumbel + logits + q`.
   # Inside the minibatch, the considered_visit can be different on states with
   # a smaller number of valid actions.
   considered_visit = jnp.max(summary.visit_counts, axis=-1, keepdims=True)
```

### Comparing `mctx-0.0.1/mctx/_src/qtransforms.py` & `mctx-0.0.2/mctx/_src/qtransforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,10 +184,10 @@
   # prior probability.
   prior_probs = jnp.maximum(jnp.finfo(prior_probs.dtype).tiny, prior_probs)
   # Summing the probabilities of the visited actions.
   sum_probs = jnp.sum(jnp.where(visit_counts > 0, prior_probs, 0.0),
                       axis=-1)
   weighted_q = jnp.sum(jnp.where(
       visit_counts > 0,
-      prior_probs * qvalues / sum_probs,
+      prior_probs * qvalues / jnp.where(visit_counts > 0, sum_probs, 1.0),
       0.0), axis=-1)
   return (raw_value + sum_visit_counts * weighted_q) / (sum_visit_counts + 1)
```

### Comparing `mctx-0.0.1/mctx/_src/search.py` & `mctx-0.0.2/mctx/_src/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,16 @@
     root: base.RootFnOutput,
     recurrent_fn: base.RecurrentFn,
     root_action_selection_fn: base.RootActionSelectionFn,
     interior_action_selection_fn: base.InteriorActionSelectionFn,
     num_simulations: int,
     max_depth: Optional[int] = None,
     invalid_actions: Optional[chex.Array] = None,
-    extra_data: Any = None) -> Tree:
+    extra_data: Any = None,
+    loop_fn: base.LoopFn = jax.lax.fori_loop) -> Tree:
   """Performs a full search and returns sampled actions.
 
   In the shape descriptions, `B` denotes the batch dimension.
 
   Args:
     params: params to be forwarded to root and recurrent functions.
     rng_key: random number generator state, the key is consumed.
@@ -60,14 +61,16 @@
     num_simulations: the number of simulations.
     max_depth: maximum search tree depth allowed during simulation, defined as
       the number of edges from the root to a leaf node.
     invalid_actions: a mask with invalid actions at the root. In the
       mask, invalid actions have ones, and valid actions have zeros.
       Shape `[B, num_actions]`.
     extra_data: extra data passed to `tree.extra_data`. Shape `[B, ...]`.
+    loop_fn: Function used to run the simulations. It may be required to pass
+      hk.fori_loop if using this function inside a Haiku module.
 
   Returns:
     `SearchResults` containing outcomes of the search, e.g. `visit_counts`
     `[B, num_actions]`.
   """
   action_selection_fn = action_selection.switching_action_selection_wrapper(
       root_action_selection_fn=root_action_selection_fn,
@@ -101,15 +104,15 @@
     loop_state = rng_key, tree
     return loop_state
 
   # Allocate all necessary storage.
   tree = instantiate_tree_from_root(root, num_simulations,
                                     root_invalid_actions=invalid_actions,
                                     extra_data=extra_data)
-  _, tree = jax.lax.fori_loop(
+  _, tree = loop_fn(
       0, num_simulations, body_fun, (rng_key, tree))
 
   return tree
 
 
 class _SimulationState(NamedTuple):
   """The state for the simulation while loop."""
@@ -210,15 +213,15 @@
     tree: updated MCTS tree state.
   """
   batch_size = tree_lib.infer_batch_size(tree)
   batch_range = jnp.arange(batch_size)
   chex.assert_shape([parent_index, action, next_node_index], (batch_size,))
 
   # Retrieve states for nodes to be evaluated.
-  embedding = jax.tree_map(
+  embedding = jax.tree_util.tree_map(
       lambda x: x[batch_range, parent_index], tree.embeddings)
 
   # Evaluate and create a new node.
   step, embedding = recurrent_fn(params, rng_key, action, embedding)
   chex.assert_shape(step.prior_logits, [batch_size, tree.num_actions])
   chex.assert_shape(step.reward, [batch_size])
   chex.assert_shape(step.discount, [batch_size])
@@ -326,15 +329,15 @@
           tree.children_prior_logits, prior_logits, node_index),
       raw_values=batch_update(
           tree.raw_values, value, node_index),
       node_values=batch_update(
           tree.node_values, value, node_index),
       node_visits=batch_update(
           tree.node_visits, new_visit, node_index),
-      embeddings=jax.tree_map(
+      embeddings=jax.tree_util.tree_map(
           lambda t, s: batch_update(t, s, node_index),
           tree.embeddings, embedding))
 
   return tree.replace(**updates)
 
 
 def instantiate_tree_from_root(
@@ -366,15 +369,15 @@
           batch_node_action, Tree.UNVISITED, dtype=jnp.int32),
       children_prior_logits=jnp.zeros(
           batch_node_action, dtype=root.prior_logits.dtype),
       children_values=jnp.zeros(batch_node_action, dtype=data_dtype),
       children_visits=jnp.zeros(batch_node_action, dtype=jnp.int32),
       children_rewards=jnp.zeros(batch_node_action, dtype=data_dtype),
       children_discounts=jnp.zeros(batch_node_action, dtype=data_dtype),
-      embeddings=jax.tree_map(_zeros, root.embedding),
+      embeddings=jax.tree_util.tree_map(_zeros, root.embedding),
       root_invalid_actions=root_invalid_actions,
       extra_data=extra_data)
 
   root_index = jnp.full([batch_size], Tree.ROOT_INDEX)
   tree = update_tree_node(
       tree, root_index, root.prior_logits, root.value, root.embedding)
   return tree
```

### Comparing `mctx-0.0.1/mctx/_src/seq_halving.py` & `mctx-0.0.2/mctx/_src/seq_halving.py`

 * *Files identical despite different names*

### Comparing `mctx-0.0.1/mctx/_src/tests/mctx_test.py` & `mctx-0.0.2/mctx/_src/tests/mctx_test.py`

 * *Files identical despite different names*

### Comparing `mctx-0.0.1/mctx/_src/tests/policies_test.py` & `mctx-0.0.2/mctx/_src/tests/policies_test.py`

 * *Files identical despite different names*

### Comparing `mctx-0.0.1/mctx/_src/tests/qtransforms_test.py` & `mctx-0.0.2/mctx/_src/tests/qtransforms_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,10 +34,23 @@
 
     num_simulations = jnp.sum(visit_counts)
     expected_mix_value = 1.0 / (num_simulations + 1) * (
         raw_value + num_simulations *
         (probs[1] * qvalues[1] + probs[2] * qvalues[2]))
     np.testing.assert_allclose(expected_mix_value, mix_value)
 
+  def test_mix_value_with_zero_visits(self):
+    """Tests that zero visit counts do not divide by zero."""
+    raw_value = jnp.array(-0.8)
+    prior_logits = jnp.array([-jnp.inf, -1.0, 2.0, -jnp.inf])
+    probs = jax.nn.softmax(prior_logits)
+    visit_counts = jnp.array([0, 0, 0, 0])
+    qvalues = jnp.zeros_like(probs)
+    with jax.debug_nans():
+      mix_value = qtransforms._compute_mixed_value(
+          raw_value, qvalues, visit_counts, probs)
+
+    np.testing.assert_allclose(raw_value, mix_value)
+
 
 if __name__ == "__main__":
   absltest.main()
```

### Comparing `mctx-0.0.1/mctx/_src/tests/seq_halving_test.py` & `mctx-0.0.2/mctx/_src/tests/seq_halving_test.py`

 * *Files identical despite different names*

### Comparing `mctx-0.0.1/mctx/_src/tests/tree_test.py` & `mctx-0.0.2/mctx/_src/tests/tree_test.py`

 * *Files identical despite different names*

### Comparing `mctx-0.0.1/mctx/_src/tree.py` & `mctx-0.0.2/mctx/_src/tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         qvalues=qvalues)
 
 
 def infer_batch_size(tree: Tree) -> int:
   """Recovers batch size from `Tree` data structure."""
   if tree.node_values.ndim != 2:
     raise ValueError("Input tree is not batched.")
-  chex.assert_equal_shape_prefix(jax.tree_leaves(tree), 1)
+  chex.assert_equal_shape_prefix(jax.tree_util.tree_leaves(tree), 1)
   return tree.node_values.shape[0]
 
 
 # A number of aggregate statistics and predictions are extracted from the
 # search data and returned to the user for further processing.
 @chex.dataclass(frozen=True)
 class SearchSummary:
```

### Comparing `mctx-0.0.1/mctx.egg-info/PKG-INFO` & `mctx-0.0.2/mctx.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mctx
-Version: 0.0.1
+Version: 0.0.2
 Summary: Monte Carlo tree search in JAX.
 Home-page: https://github.com/deepmind/mctx
 Author: DeepMind
 Author-email: mctx-dev@google.com
 License: Apache 2.0
 Keywords: jax planning reinforcement-learning python machine learning
 Platform: UNKNOWN
@@ -29,22 +29,25 @@
 speed up, the implementation fully supports JIT-compilation. Search algorithms
 in Mctx are defined for and operate on batches of inputs, in parallel. This
 allows to make the most of the accelerators and enables the algorithms to work
 with large learned environment models parameterized by deep neural networks.
 
 ## Installation
 
-Mctx can be installed with `pip` directly from github, with the following command:
+You can install the latest released version of Mctx from PyPI via:
 
-`pip install git+git://github.com/deepmind/mctx.git`
-
-or from PyPI:
+```sh
+pip install mctx
+```
 
-`pip install mctx`
+or you can install the latest development version from GitHub:
 
+```sh
+pip install git+https://github.com/deepmind/mctx.git
+```
 
 ## Motivation
 
 Learning and search have been important topics since the early days of AI
 research. In the words of Rich Sutton: *One thing that should be learned [...]
 is the great power of general purpose methods, of methods that continue to scale
 with increased computation even as the available computation becomes very great.
@@ -106,15 +109,15 @@
 The dynamics environment model needs to be specified by a `recurrent_fn`.
 A `recurrent_fn(params, rng_key, action, embedding)` call takes an `action` and
 a state `embedding`. The call should return a tuple `(recurrent_fn_output,
 new_embedding)` with a `RecurrentFnOutput` and the embedding of the next state.
 The `RecurrentFnOutput` contains the `reward` and `discount` for the transition,
 and `prior_logits` and `value` for the new state.
 
-In [examples/visualization_demo.py](https://github.com/deepmind/mctx/blob/master/examples/visualization_demo.py)
+In [examples/visualization_demo.py](https://github.com/deepmind/mctx/blob/main/examples/visualization_demo.py)
 you can see calls to a policy:
 
 ```python
 policy_output = mctx.gumbel_muzero_policy(params, rng_key, root, recurrent_fn,
                                           num_simulations=32)
 ```
 
@@ -123,15 +126,25 @@
 `policy_output.action_weights` contain targets usable to train the policy
 probabilities.
 
 We recommend to use the `gumbel_muzero_policy`.
 [Gumbel MuZero](https://openreview.net/forum?id=bERaNdoegnO) guarantees a policy
 improvement if the action values are correctly evaluated. The policy improvement
 is demonstrated in
-[examples/policy_improvement_demo.py](https://github.com/deepmind/mctx/blob/master/examples/policy_improvement_demo.py).
+[examples/policy_improvement_demo.py](https://github.com/deepmind/mctx/blob/main/examples/policy_improvement_demo.py).
+
+### Example projects
+The following projects demonstrate the Mctx usage:
+
+- [Basic Learning Demo with Mctx](https://github.com/kenjyoung/mctx_learning_demo)
+... AlphaZero on random mazes.
+- [a0-jax](https://github.com/NTT123/a0-jax) ... AlphaZero on Connect Four,
+Gomoku, and Go.
+
+Tell us about your project.
 
 ## Citing Mctx
 
 This is not an officially supported Google product. Mctx is part of the
 [DeepMind JAX Ecosystem], to cite Mctx please use the [DeepMind JAX Ecosystem
 citation].
```

### Comparing `mctx-0.0.1/mctx.egg-info/SOURCES.txt` & `mctx-0.0.2/mctx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mctx-0.0.1/setup.py` & `mctx-0.0.2/setup.py`

 * *Files identical despite different names*


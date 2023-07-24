# Comparing `tmp/netket-3.8.tar.gz` & `tmp/netket-3.9.tar.gz`

## Comparing `netket-3.8.tar` & `netket-3.9.tar`

### file list

```diff
@@ -1,247 +1,263 @@
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 netket-3.8/netket/__init__.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 netket-3.8/netket/_version.py
--rw-r--r--   0        0        0     8043 2020-02-02 00:00:00.000000 netket-3.8/netket/exact.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 netket-3.8/netket/callbacks/__init__.py
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 netket-3.8/netket/callbacks/earlystopping.py
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 netket-3.8/netket/callbacks/invalidlossstopping.py
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 netket-3.8/netket/callbacks/timeout.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 netket-3.8/netket/driver/__init__.py
--rw-r--r--   0        0        0    12221 2020-02-02 00:00:00.000000 netket-3.8/netket/driver/abstract_variational_driver.py
--rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 netket-3.8/netket/driver/steady_state.py
--rw-r--r--   0        0        0     5701 2020-02-02 00:00:00.000000 netket-3.8/netket/driver/vmc.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 netket-3.8/netket/driver/vmc_common.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/__init__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/driver/__init__.py
--rw-r--r--   0        0        0     7432 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/driver/tdvp.py
--rw-r--r--   0        0        0    17244 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/driver/tdvp_common.py
--rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/driver/tdvp_schmitt.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/dynamics/__init__.py
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/dynamics/_rk_solver.py
--rw-r--r--   0        0        0    13184 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/dynamics/_rk_solver_structures.py
--rw-r--r--   0        0        0    10730 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/dynamics/_rk_tableau.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/hilbert/__init__.py
--rw-r--r--   0        0        0     6822 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/hilbert/spin_orbital_fermions.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/hilbert/random/__init__.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/hilbert/random/spin_orbital_fermions.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/logging/__init__.py
--rw-r--r--   0        0        0     7361 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/logging/hdf5_log.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/operator/__init__.py
--rw-r--r--   0        0        0    24940 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/operator/_fermion_operator_2nd.py
--rw-r--r--   0        0        0    13155 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/operator/_fermion_operator_2nd_utils.py
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/operator/fermion.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/qsr/__init__.py
--rw-r--r--   0        0        0    13235 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/qsr/dataset.py
--rw-r--r--   0        0        0    19537 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/qsr/driver.py
--rw-r--r--   0        0        0     8050 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/qsr/logic_helpers.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/sampler/__init__.py
--rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/sampler/metropolis_pmap.py
--rw-r--r--   0        0        0    21399 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/sampler/metropolis_pt.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/vqs/__init__.py
--rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 netket-3.8/netket/experimental/vqs/io.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 netket-3.8/netket/graph/__init__.py
--rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 netket-3.8/netket/graph/_lattice_edge_logic.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 netket-3.8/netket/graph/abstract_graph.py
--rw-r--r--   0        0        0    19802 2020-02-02 00:00:00.000000 netket-3.8/netket/graph/common_lattices.py
--rw-r--r--   0        0        0     8816 2020-02-02 00:00:00.000000 netket-3.8/netket/graph/graph.py
--rw-r--r--   0        0        0    28276 2020-02-02 00:00:00.000000 netket-3.8/netket/graph/lattice.py
--rw-r--r--   0        0        0    12996 2020-02-02 00:00:00.000000 netket-3.8/netket/graph/space_group.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/__init__.py
--rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/abstract_hilbert.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/continuous_hilbert.py
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/custom_hilbert.py
--rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/discrete_hilbert.py
--rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/doubled_hilbert.py
--rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/fock.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/hilbert_index.py
--rw-r--r--   0        0        0     7328 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/homogeneous.py
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/particle.py
--rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/qubit.py
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/spin.py
--rw-r--r--   0        0        0     6965 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/tensor_hilbert.py
--rw-r--r--   0        0        0     5853 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/tensor_hilbert_discrete.py
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/random/__init__.py
--rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/random/base.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/random/custom.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/random/doubled.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/random/fock.py
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/random/particle.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/random/qubit.py
--rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/random/spin.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 netket-3.8/netket/hilbert/random/tensor_hilbert.py
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/__init__.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/_chunk_utils.py
--rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/_expect.py
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/_grad.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/_math.py
--rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/_scanmap.py
--rw-r--r--   0        0        0     5523 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/_vjp.py
--rw-r--r--   0        0        0     8560 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/_vjp_chunked.py
--rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/_vmap_chunked.py
--rw-r--r--   0        0        0    10602 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/utils.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/_jacobian/__init__.py
--rw-r--r--   0        0        0     5338 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/_jacobian/default_mode.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/_jacobian/jacobian_dense.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/_jacobian/jacobian_pytree.py
--rw-r--r--   0        0        0     7077 2020-02-02 00:00:00.000000 netket-3.8/netket/jax/_jacobian/logic.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 netket-3.8/netket/logging/__init__.py
--rw-r--r--   0        0        0     7404 2020-02-02 00:00:00.000000 netket-3.8/netket/logging/json_log.py
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 netket-3.8/netket/logging/runtime_log.py
--rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 netket-3.8/netket/logging/state_log.py
--rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 netket-3.8/netket/logging/tensorboard.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 netket-3.8/netket/models/README.md
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 netket-3.8/netket/models/__init__.py
--rw-r--r--   0        0        0    13327 2020-02-02 00:00:00.000000 netket-3.8/netket/models/autoreg.py
--rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 netket-3.8/netket/models/deepset.py
--rw-r--r--   0        0        0    33655 2020-02-02 00:00:00.000000 netket-3.8/netket/models/equivariant.py
--rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 netket-3.8/netket/models/fast_autoreg.py
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 netket-3.8/netket/models/full_space.py
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 netket-3.8/netket/models/gaussian.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 netket-3.8/netket/models/jastrow.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 netket-3.8/netket/models/mlp.py
--rw-r--r--   0        0        0     6429 2020-02-02 00:00:00.000000 netket-3.8/netket/models/mps.py
--rw-r--r--   0        0        0     7760 2020-02-02 00:00:00.000000 netket-3.8/netket/models/ndm.py
--rw-r--r--   0        0        0     9722 2020-02-02 00:00:00.000000 netket-3.8/netket/models/rbm.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 netket-3.8/netket/models/utils.py
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 netket-3.8/netket/nn/__init__.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 netket-3.8/netket/nn/activation.py
--rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 netket-3.8/netket/nn/deprecation.py
--rw-r--r--   0        0        0    16212 2020-02-02 00:00:00.000000 netket-3.8/netket/nn/fast_masked_linear.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 netket-3.8/netket/nn/initializers.py
--rw-r--r--   0        0        0    10675 2020-02-02 00:00:00.000000 netket-3.8/netket/nn/masked_linear.py
--rw-r--r--   0        0        0    35492 2020-02-02 00:00:00.000000 netket-3.8/netket/nn/symmetric_linear.py
--rw-r--r--   0        0        0     9758 2020-02-02 00:00:00.000000 netket-3.8/netket/nn/utils.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 netket-3.8/netket/nn/blocks/__init__.py
--rw-r--r--   0        0        0     3845 2020-02-02 00:00:00.000000 netket-3.8/netket/nn/blocks/deepset.py
--rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 netket-3.8/netket/nn/blocks/mlp.py
--rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 netket-3.8/netket/nn/blocks/symmetry_sum.py
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/__init__.py
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_abstract_operator.py
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_abstract_super_operator.py
--rw-r--r--   0        0        0    11185 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_bose_hubbard.py
--rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_continuous_operator.py
--rw-r--r--   0        0        0     9378 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_discrete_operator.py
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_graph_operator.py
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_hamiltonian.py
--rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_heisenberg.py
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_ising.py
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_kinetic.py
--rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_lazy.py
--rw-r--r--   0        0        0    16259 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_local_liouvillian.py
--rw-r--r--   0        0        0    25078 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_local_operator.py
--rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_local_operator_compile_helpers.py
--rw-r--r--   0        0        0     9788 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_local_operator_helpers.py
--rw-r--r--   0        0        0    23208 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_pauli_strings.py
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_potential.py
--rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/_sumoperators.py
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/boson.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 netket-3.8/netket/operator/spin.py
--rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/__init__.py
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/linear_operator.py
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/preconditioner.py
--rw-r--r--   0        0        0     7129 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/sr.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/qgt/__init__.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/qgt/common.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/qgt/default.py
--rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/qgt/qgt_jacobian_common.py
--rw-r--r--   0        0        0    10347 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/qgt/qgt_jacobian_dense.py
--rw-r--r--   0        0        0    10920 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/qgt/qgt_jacobian_pytree.py
--rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/qgt/qgt_jacobian_pytree_logic.py
--rw-r--r--   0        0        0     7183 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/qgt/qgt_onthefly.py
--rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/qgt/qgt_onthefly_logic.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/solver/__init__.py
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 netket-3.8/netket/optimizer/solver/solvers.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/__init__.py
--rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/autoreg.py
--rw-r--r--   0        0        0    18106 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/base.py
--rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/exact.py
--rw-r--r--   0        0        0    26652 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/metropolis.py
--rw-r--r--   0        0        0     9358 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/metropolis_numpy.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/rules/__init__.py
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/rules/base.py
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/rules/continuous_gaussian.py
--rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/rules/custom_numpy.py
--rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/rules/exchange.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/rules/fixed.py
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/rules/hamiltonian.py
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/rules/hamiltonian_numpy.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/rules/langevin.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/rules/local.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/rules/local_numpy.py
--rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/rules/multiple.py
--rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 netket-3.8/netket/sampler/rules/tensor.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 netket-3.8/netket/stats/__init__.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 netket-3.8/netket/stats/_autocorr.py
--rw-r--r--   0        0        0     9740 2020-02-02 00:00:00.000000 netket-3.8/netket/stats/mc_stats.py
--rw-r--r--   0        0        0     6922 2020-02-02 00:00:00.000000 netket-3.8/netket/stats/mc_stats_old.py
--rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 netket-3.8/netket/stats/mpi_stats.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netket-3.8/netket/tools/__init__.py
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 netket-3.8/netket/tools/_common.py
--rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 netket-3.8/netket/tools/_cpu_info.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 netket-3.8/netket/tools/_mpi_info.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 netket-3.8/netket/tools/check_mpi.py
--rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 netket-3.8/netket/tools/info.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/__init__.py
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/_dependencies_check.py
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/array.py
--rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/config_flags.py
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/deprecation.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/dispatch.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/errors.py
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/float.py
--rw-r--r--   0        0        0    12748 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/history.py
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/jax.py
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/moduletools.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/numbers.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/optional_deps.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/partial.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/seed.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/summation.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/types.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/version_check.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/group/__init__.py
--rw-r--r--   0        0        0    15118 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/group/_group.py
--rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/group/_permutation_group.py
--rw-r--r--   0        0        0    21830 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/group/_point_group.py
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/group/_semigroup.py
--rw-r--r--   0        0        0    10404 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/group/axial.py
--rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/group/cubic.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/group/icosa.py
--rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/group/planar.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/model_frameworks/__init__.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/model_frameworks/base.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/model_frameworks/flax.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/model_frameworks/haiku.py
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/model_frameworks/jax.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/mpi/__init__.py
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/mpi/mpi.py
--rw-r--r--   0        0        0     7319 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/mpi/primitives.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/struct/__init__.py
--rw-r--r--   0        0        0    16933 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/struct/dataclass.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 netket-3.8/netket/utils/struct/utils.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/__init__.py
--rw-r--r--   0        0        0    15652 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/base.py
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/experimental.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/exact/__init__.py
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/exact/expect.py
--rw-r--r--   0        0        0    12301 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/exact/state.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/__init__.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/common.py
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/kernels.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/mc_mixed_state/__init__.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/mc_mixed_state/expect.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/mc_mixed_state/expect_chunked.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/mc_mixed_state/expect_grad_chunked.py
--rw-r--r--   0        0        0    10497 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/mc_mixed_state/state.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/mc_state/__init__.py
--rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/mc_state/expect.py
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/mc_state/expect_chunked.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/mc_state/expect_forces.py
--rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/mc_state/expect_forces_chunked.py
--rw-r--r--   0        0        0     5440 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/mc_state/expect_grad.py
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/mc_state/expect_grad_chunked.py
--rw-r--r--   0        0        0    28665 2020-02-02 00:00:00.000000 netket-3.8/netket/vqs/mc/mc_state/state.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 netket-3.8/.gitignore
--rw-r--r--   0        0        0    10173 2020-02-02 00:00:00.000000 netket-3.8/LICENSE
--rw-r--r--   0        0        0     5877 2020-02-02 00:00:00.000000 netket-3.8/README.md
--rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 netket-3.8/pyproject.toml
--rw-r--r--   0        0        0     8730 2020-02-02 00:00:00.000000 netket-3.8/PKG-INFO
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 netket-3.9/netket/__init__.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 netket-3.9/netket/_version.py
+-rw-r--r--   0        0        0    25304 2020-02-02 00:00:00.000000 netket-3.9/netket/errors.py
+-rw-r--r--   0        0        0     8705 2020-02-02 00:00:00.000000 netket-3.9/netket/exact.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 netket-3.9/netket/callbacks/__init__.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 netket-3.9/netket/callbacks/convergence_stopping.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 netket-3.9/netket/callbacks/earlystopping.py
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 netket-3.9/netket/callbacks/invalidlossstopping.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 netket-3.9/netket/callbacks/timeout.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 netket-3.9/netket/driver/__init__.py
+-rw-r--r--   0        0        0    12221 2020-02-02 00:00:00.000000 netket-3.9/netket/driver/abstract_variational_driver.py
+-rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 netket-3.9/netket/driver/steady_state.py
+-rw-r--r--   0        0        0     5691 2020-02-02 00:00:00.000000 netket-3.9/netket/driver/vmc.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 netket-3.9/netket/driver/vmc_common.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/__init__.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/driver/__init__.py
+-rw-r--r--   0        0        0     7478 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/driver/tdvp.py
+-rw-r--r--   0        0        0    17314 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/driver/tdvp_common.py
+-rw-r--r--   0        0        0    11601 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/driver/tdvp_schmitt.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/dynamics/__init__.py
+-rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/dynamics/_rk_solver.py
+-rw-r--r--   0        0        0    13184 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/dynamics/_rk_solver_structures.py
+-rw-r--r--   0        0        0    10730 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/dynamics/_rk_tableau.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/hilbert/__init__.py
+-rw-r--r--   0        0        0     6814 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/hilbert/spin_orbital_fermions.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/hilbert/random/__init__.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/hilbert/random/spin_orbital_fermions.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/logging/__init__.py
+-rw-r--r--   0        0        0     7361 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/logging/hdf5_log.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/operator/__init__.py
+-rw-r--r--   0        0        0    25157 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/operator/_fermion_operator_2nd.py
+-rw-r--r--   0        0        0    13155 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/operator/_fermion_operator_2nd_utils.py
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/operator/fermion.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/qsr/__init__.py
+-rw-r--r--   0        0        0    13235 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/qsr/dataset.py
+-rw-r--r--   0        0        0    19562 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/qsr/driver.py
+-rw-r--r--   0        0        0     8058 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/qsr/logic_helpers.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/sampler/__init__.py
+-rw-r--r--   0        0        0     8540 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/sampler/metropolis_pmap.py
+-rw-r--r--   0        0        0    21309 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/sampler/metropolis_pt.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/vqs/__init__.py
+-rw-r--r--   0        0        0     3276 2020-02-02 00:00:00.000000 netket-3.9/netket/experimental/vqs/io.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 netket-3.9/netket/graph/__init__.py
+-rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 netket-3.9/netket/graph/_lattice_edge_logic.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 netket-3.9/netket/graph/abstract_graph.py
+-rw-r--r--   0        0        0    19802 2020-02-02 00:00:00.000000 netket-3.9/netket/graph/common_lattices.py
+-rw-r--r--   0        0        0     8811 2020-02-02 00:00:00.000000 netket-3.9/netket/graph/graph.py
+-rw-r--r--   0        0        0    28347 2020-02-02 00:00:00.000000 netket-3.9/netket/graph/lattice.py
+-rw-r--r--   0        0        0    12996 2020-02-02 00:00:00.000000 netket-3.9/netket/graph/space_group.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 netket-3.9/netket/hilbert/__init__.py
+-rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 netket-3.9/netket/hilbert/abstract_hilbert.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 netket-3.9/netket/hilbert/continuous_hilbert.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 netket-3.9/netket/hilbert/custom_hilbert.py
+-rw-r--r--   0        0        0     8590 2020-02-02 00:00:00.000000 netket-3.9/netket/hilbert/discrete_hilbert.py
+-rw-r--r--   0        0        0     4431 2020-02-02 00:00:00.000000 netket-3.9/netket/hilbert/doubled_hilbert.py
+-rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 netket-3.9/netket/hilbert/fock.py
+-rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 netket-3.9/netket/hilbert/homogeneous.py
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 netket-3.9/netket/hilbert/particle.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 netket-3.9/netket/hilbert/qubit.py
+-rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 netket-3.9/netket/hilbert/spin.py
+-rw-r--r--   0        0        0     6931 2020-02-02 00:00:00.000000 netket-3.9/netket/hilbert/tensor_hilbert.py
+-rw-r--r--   0        0        0     5853 2020-02-02 00:00:00.000000 netket-3.9/netket/hilbert/tensor_hilbert_discrete.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 netket-3.9/netket/hilbert/index/__init__.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 netket-3.9/netket/hilbert/index/base.py
+-rw-r--r--   0        0        0     3962 2020-02-02 00:00:00.000000 netket-3.9/netket/hilbert/index/constrained.py
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 netket-3.9/netket/hilbert/index/unconstrained.py
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 netket-3.9/netket/hilbert/random/__init__.py
+-rw-r--r--   0        0        0     4106 2020-02-02 00:00:00.000000 netket-3.9/netket/hilbert/random/base.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 netket-3.9/netket/hilbert/random/custom.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 netket-3.9/netket/hilbert/random/doubled.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 netket-3.9/netket/hilbert/random/fock.py
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 netket-3.9/netket/hilbert/random/particle.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 netket-3.9/netket/hilbert/random/qubit.py
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 netket-3.9/netket/hilbert/random/spin.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 netket-3.9/netket/hilbert/random/tensor_hilbert.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 netket-3.9/netket/jax/__init__.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 netket-3.9/netket/jax/_chunk_utils.py
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 netket-3.9/netket/jax/_expect.py
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 netket-3.9/netket/jax/_grad.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 netket-3.9/netket/jax/_math.py
+-rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 netket-3.9/netket/jax/_scanmap.py
+-rw-r--r--   0        0        0     5523 2020-02-02 00:00:00.000000 netket-3.9/netket/jax/_vjp.py
+-rw-r--r--   0        0        0     8560 2020-02-02 00:00:00.000000 netket-3.9/netket/jax/_vjp_chunked.py
+-rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 netket-3.9/netket/jax/_vmap_chunked.py
+-rw-r--r--   0        0        0    10586 2020-02-02 00:00:00.000000 netket-3.9/netket/jax/utils.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 netket-3.9/netket/jax/_jacobian/__init__.py
+-rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 netket-3.9/netket/jax/_jacobian/default_mode.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 netket-3.9/netket/jax/_jacobian/jacobian_dense.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 netket-3.9/netket/jax/_jacobian/jacobian_pytree.py
+-rw-r--r--   0        0        0    14994 2020-02-02 00:00:00.000000 netket-3.9/netket/jax/_jacobian/logic.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 netket-3.9/netket/logging/__init__.py
+-rw-r--r--   0        0        0     7466 2020-02-02 00:00:00.000000 netket-3.9/netket/logging/json_log.py
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 netket-3.9/netket/logging/runtime_log.py
+-rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 netket-3.9/netket/logging/state_log.py
+-rw-r--r--   0        0        0     5867 2020-02-02 00:00:00.000000 netket-3.9/netket/logging/tensorboard.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 netket-3.9/netket/models/README.md
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 netket-3.9/netket/models/__init__.py
+-rw-r--r--   0        0        0    13327 2020-02-02 00:00:00.000000 netket-3.9/netket/models/autoreg.py
+-rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 netket-3.9/netket/models/deepset.py
+-rw-r--r--   0        0        0    33559 2020-02-02 00:00:00.000000 netket-3.9/netket/models/equivariant.py
+-rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 netket-3.9/netket/models/fast_autoreg.py
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 netket-3.9/netket/models/full_space.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 netket-3.9/netket/models/gaussian.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 netket-3.9/netket/models/jastrow.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 netket-3.9/netket/models/mlp.py
+-rw-r--r--   0        0        0     6429 2020-02-02 00:00:00.000000 netket-3.9/netket/models/mps.py
+-rw-r--r--   0        0        0     7760 2020-02-02 00:00:00.000000 netket-3.9/netket/models/ndm.py
+-rw-r--r--   0        0        0     9722 2020-02-02 00:00:00.000000 netket-3.9/netket/models/rbm.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 netket-3.9/netket/models/utils.py
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 netket-3.9/netket/nn/__init__.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 netket-3.9/netket/nn/activation.py
+-rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 netket-3.9/netket/nn/deprecation.py
+-rw-r--r--   0        0        0    16212 2020-02-02 00:00:00.000000 netket-3.9/netket/nn/fast_masked_linear.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 netket-3.9/netket/nn/initializers.py
+-rw-r--r--   0        0        0    10675 2020-02-02 00:00:00.000000 netket-3.9/netket/nn/masked_linear.py
+-rw-r--r--   0        0        0    35416 2020-02-02 00:00:00.000000 netket-3.9/netket/nn/symmetric_linear.py
+-rw-r--r--   0        0        0     9473 2020-02-02 00:00:00.000000 netket-3.9/netket/nn/utils.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 netket-3.9/netket/nn/blocks/__init__.py
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 netket-3.9/netket/nn/blocks/deepset.py
+-rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 netket-3.9/netket/nn/blocks/mlp.py
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 netket-3.9/netket/nn/blocks/symmetry_sum.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/__init__.py
+-rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_abstract_operator.py
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_abstract_super_operator.py
+-rw-r--r--   0        0        0    11408 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_bose_hubbard.py
+-rw-r--r--   0        0        0     4600 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_continuous_operator.py
+-rw-r--r--   0        0        0    10630 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_discrete_operator.py
+-rw-r--r--   0        0        0     8590 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_discrete_operator_jax.py
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_graph_operator.py
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_hamiltonian.py
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_heisenberg.py
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_kinetic.py
+-rw-r--r--   0        0        0     6435 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_lazy.py
+-rw-r--r--   0        0        0    16259 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_local_liouvillian.py
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_potential.py
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_sumoperators.py
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/boson.py
+-rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/spin.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_ising/__init__.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_ising/base.py
+-rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_ising/jax.py
+-rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_ising/numba.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_local_operator/__init__.py
+-rw-r--r--   0        0        0    25787 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_local_operator/base.py
+-rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_local_operator/compile_helpers.py
+-rw-r--r--   0        0        0     6711 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_local_operator/convert.py
+-rw-r--r--   0        0        0     9879 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_local_operator/helpers.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_pauli_strings/__init__.py
+-rw-r--r--   0        0        0    17099 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_pauli_strings/base.py
+-rw-r--r--   0        0        0    14349 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_pauli_strings/jax.py
+-rw-r--r--   0        0        0    10370 2020-02-02 00:00:00.000000 netket-3.9/netket/operator/_pauli_strings/numba.py
+-rw-r--r--   0        0        0     6619 2020-02-02 00:00:00.000000 netket-3.9/netket/optimizer/__init__.py
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 netket-3.9/netket/optimizer/linear_operator.py
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 netket-3.9/netket/optimizer/preconditioner.py
+-rw-r--r--   0        0        0     7129 2020-02-02 00:00:00.000000 netket-3.9/netket/optimizer/sr.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 netket-3.9/netket/optimizer/qgt/__init__.py
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 netket-3.9/netket/optimizer/qgt/common.py
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 netket-3.9/netket/optimizer/qgt/default.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 netket-3.9/netket/optimizer/qgt/qgt_jacobian_common.py
+-rw-r--r--   0        0        0    10502 2020-02-02 00:00:00.000000 netket-3.9/netket/optimizer/qgt/qgt_jacobian_dense.py
+-rw-r--r--   0        0        0    11075 2020-02-02 00:00:00.000000 netket-3.9/netket/optimizer/qgt/qgt_jacobian_pytree.py
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 netket-3.9/netket/optimizer/qgt/qgt_jacobian_pytree_logic.py
+-rw-r--r--   0        0        0     9185 2020-02-02 00:00:00.000000 netket-3.9/netket/optimizer/qgt/qgt_onthefly.py
+-rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 netket-3.9/netket/optimizer/qgt/qgt_onthefly_logic.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 netket-3.9/netket/optimizer/solver/__init__.py
+-rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 netket-3.9/netket/optimizer/solver/solvers.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 netket-3.9/netket/sampler/__init__.py
+-rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 netket-3.9/netket/sampler/autoreg.py
+-rw-r--r--   0        0        0    18149 2020-02-02 00:00:00.000000 netket-3.9/netket/sampler/base.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 netket-3.9/netket/sampler/exact.py
+-rw-r--r--   0        0        0    27062 2020-02-02 00:00:00.000000 netket-3.9/netket/sampler/metropolis.py
+-rw-r--r--   0        0        0     9397 2020-02-02 00:00:00.000000 netket-3.9/netket/sampler/metropolis_numpy.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 netket-3.9/netket/sampler/rules/__init__.py
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 netket-3.9/netket/sampler/rules/base.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 netket-3.9/netket/sampler/rules/continuous_gaussian.py
+-rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 netket-3.9/netket/sampler/rules/custom_numpy.py
+-rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 netket-3.9/netket/sampler/rules/exchange.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 netket-3.9/netket/sampler/rules/fixed.py
+-rw-r--r--   0        0        0     7968 2020-02-02 00:00:00.000000 netket-3.9/netket/sampler/rules/hamiltonian.py
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 netket-3.9/netket/sampler/rules/hamiltonian_numpy.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 netket-3.9/netket/sampler/rules/langevin.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 netket-3.9/netket/sampler/rules/local.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 netket-3.9/netket/sampler/rules/local_numpy.py
+-rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 netket-3.9/netket/sampler/rules/multiple.py
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 netket-3.9/netket/sampler/rules/tensor.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 netket-3.9/netket/stats/__init__.py
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 netket-3.9/netket/stats/_autocorr.py
+-rw-r--r--   0        0        0     9643 2020-02-02 00:00:00.000000 netket-3.9/netket/stats/mc_stats.py
+-rw-r--r--   0        0        0     6922 2020-02-02 00:00:00.000000 netket-3.9/netket/stats/mc_stats_old.py
+-rw-r--r--   0        0        0     4955 2020-02-02 00:00:00.000000 netket-3.9/netket/stats/mpi_stats.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 netket-3.9/netket/tools/__init__.py
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 netket-3.9/netket/tools/_common.py
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 netket-3.9/netket/tools/_cpu_info.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 netket-3.9/netket/tools/_mpi_info.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 netket-3.9/netket/tools/check_mpi.py
+-rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 netket-3.9/netket/tools/info.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/__init__.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/_dependencies_check.py
+-rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/array.py
+-rw-r--r--   0        0        0     6614 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/config_flags.py
+-rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/deprecation.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/dispatch.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/float.py
+-rw-r--r--   0        0        0    12748 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/history.py
+-rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/holomorphic.py
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/jax.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/moduletools.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/numbers.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/optional_deps.py
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/partial.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/seed.py
+-rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/static_number.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/summation.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/types.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/version_check.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/group/__init__.py
+-rw-r--r--   0        0        0    15118 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/group/_group.py
+-rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/group/_permutation_group.py
+-rw-r--r--   0        0        0    21830 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/group/_point_group.py
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/group/_semigroup.py
+-rw-r--r--   0        0        0    10404 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/group/axial.py
+-rw-r--r--   0        0        0     3167 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/group/cubic.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/group/icosa.py
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/group/planar.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/model_frameworks/base.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/model_frameworks/flax.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/model_frameworks/haiku.py
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/model_frameworks/jax.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/mpi/__init__.py
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/mpi/mpi.py
+-rw-r--r--   0        0        0     7319 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/mpi/primitives.py
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/struct/__init__.py
+-rw-r--r--   0        0        0    16933 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/struct/dataclass.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 netket-3.9/netket/utils/struct/utils.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 netket-3.9/netket/vqs/__init__.py
+-rw-r--r--   0        0        0    15652 2020-02-02 00:00:00.000000 netket-3.9/netket/vqs/base.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 netket-3.9/netket/vqs/deprecated.py
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 netket-3.9/netket/vqs/experimental.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 netket-3.9/netket/vqs/full_summ/__init__.py
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 netket-3.9/netket/vqs/full_summ/expect.py
+-rw-r--r--   0        0        0    12303 2020-02-02 00:00:00.000000 netket-3.9/netket/vqs/full_summ/state.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 netket-3.9/netket/vqs/mc/__init__.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 netket-3.9/netket/vqs/mc/common.py
+-rw-r--r--   0        0        0     5344 2020-02-02 00:00:00.000000 netket-3.9/netket/vqs/mc/kernels.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 netket-3.9/netket/vqs/mc/mc_mixed_state/__init__.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 netket-3.9/netket/vqs/mc/mc_mixed_state/expect.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 netket-3.9/netket/vqs/mc/mc_mixed_state/expect_chunked.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 netket-3.9/netket/vqs/mc/mc_mixed_state/expect_grad_chunked.py
+-rw-r--r--   0        0        0    10393 2020-02-02 00:00:00.000000 netket-3.9/netket/vqs/mc/mc_mixed_state/state.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 netket-3.9/netket/vqs/mc/mc_state/__init__.py
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 netket-3.9/netket/vqs/mc/mc_state/expect.py
+-rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 netket-3.9/netket/vqs/mc/mc_state/expect_chunked.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 netket-3.9/netket/vqs/mc/mc_state/expect_forces.py
+-rw-r--r--   0        0        0     4182 2020-02-02 00:00:00.000000 netket-3.9/netket/vqs/mc/mc_state/expect_forces_chunked.py
+-rw-r--r--   0        0        0     5431 2020-02-02 00:00:00.000000 netket-3.9/netket/vqs/mc/mc_state/expect_grad.py
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 netket-3.9/netket/vqs/mc/mc_state/expect_grad_chunked.py
+-rw-r--r--   0        0        0    28586 2020-02-02 00:00:00.000000 netket-3.9/netket/vqs/mc/mc_state/state.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 netket-3.9/.gitignore
+-rw-r--r--   0        0        0    10173 2020-02-02 00:00:00.000000 netket-3.9/LICENSE
+-rw-r--r--   0        0        0     5877 2020-02-02 00:00:00.000000 netket-3.9/README.md
+-rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 netket-3.9/pyproject.toml
+-rw-r--r--   0        0        0     8644 2020-02-02 00:00:00.000000 netket-3.9/PKG-INFO
```

### Comparing `netket-3.8/netket/__init__.py` & `netket-3.9/netket/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,28 +20,31 @@
 del config
 
 from ._version import version as __version__  # noqa: F401
 
 from . import utils
 from .utils import config
 
+from . import errors
+
 __all__ = [
     "exact",
     "graph",
     "callbacks",
     "hilbert",
     "operator",
     "optimizer",
     "sampler",
     "stats",
     "utils",
     "vqs",
     "nn",
 ]
 
+
 from . import jax
 from . import stats
 
 from . import graph
 from . import hilbert
 
 from . import nn
```

### Comparing `netket-3.8/netket/exact.py` & `netket-3.9/netket/exact.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import numpy as _np
 from scipy.sparse.linalg import bicgstab as _bicgstab
+from scipy.sparse.linalg import LinearOperator as _LinearOperator
 
 from .operator import AbstractOperator as _AbstractOperator
+from jax.experimental.sparse import JAXSparse as _JAXSparse
 
 
 def lanczos_ed(
     operator: _AbstractOperator,
     *,
     k: int = 1,
     compute_eigenvectors: bool = False,
@@ -64,18 +66,31 @@
     actual_scipy_args = {}
     if scipy_args:
         actual_scipy_args.update(scipy_args)
     actual_scipy_args["which"] = "SA"
     actual_scipy_args["k"] = k
     actual_scipy_args["return_eigenvectors"] = compute_eigenvectors
 
-    result = eigsh(
-        operator.to_linear_operator() if matrix_free else operator.to_sparse(),
-        **actual_scipy_args,
-    )
+    if matrix_free:
+        # wrap the operator.to_linear_operator() in a scipy.sparse.linalg.LinearOperator
+        n = operator.hilbert.n_states
+        A = _LinearOperator(
+            (n, n),
+            operator.to_linear_operator().__matmul__,
+            dtype=operator.dtype,
+        )
+    else:
+        A = operator.to_sparse()
+        if isinstance(A, _JAXSparse):
+            # jax sparse arrays are not compatible with scipy eigsh.
+            # wrap them in a scipy.sparse.linalg.LinearOperator
+            A = _LinearOperator(A.shape, A.__matmul__, dtype=A.dtype)
+
+    result = eigsh(A, **actual_scipy_args)
+
     if not compute_eigenvectors:
         # The sort order of eigenvalues returned by scipy changes based on
         # `return_eigenvalues`. Therefore we invert the order here so that the
         # smallest eigenvalue is still the first one.
         return result[::-1]
     else:
         return result
@@ -157,15 +172,17 @@
 
             warn(
                 """For reasons unknown to me, using dense diagonalisation on this
                 matrix results in very low precision of the resulting steady-state
                 since the update to numpy 1.9.
                 We suggest using sparse=True, however, if you wish not to, you have
                 been warned.
-                Your digits are your responsibility now."""
+                Your digits are your responsibility now.
+                """,
+                stacklevel=2,
             )
 
             lind_mat = lindblad.to_dense()
 
             ldagl = lind_mat.T.conj() * lind_mat
             w, v = eigh(ldagl)
```

### Comparing `netket-3.8/netket/callbacks/__init__.py` & `netket-3.9/netket/driver/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# Copyright 2020, 2021 The NetKet Authors - All rights reserved.
+# Copyright 2021 The NetKet Authors - All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .earlystopping import EarlyStopping
-from .timeout import Timeout
-from .invalidlossstopping import InvalidLossStopping
+from .abstract_variational_driver import AbstractVariationalDriver
+from .vmc import VMC
+from .steady_state import SteadyState
 
 from netket.utils import _hide_submodules
 
 _hide_submodules(__name__)
```

### Comparing `netket-3.8/netket/callbacks/earlystopping.py` & `netket-3.9/netket/callbacks/invalidlossstopping.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,57 +8,46 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from dataclasses import dataclass
-from typing import Optional, Union
-
+from typing import Union
 import numpy as np
 
+from netket.utils import struct
+
 
-@dataclass
-class EarlyStopping:
+# Mark this class a NetKet dataclass so that it can automatically be serialized by Flax.
+@struct.dataclass(_frozen=False)
+class InvalidLossStopping:
     """A simple callback to stop NetKet if there are no more improvements in the training.
     based on `driver._loss_name`."""
 
-    min_delta: float = 0.0
-    """Minimum change in the monitored quantity to qualify as an improvement."""
-    patience: Union[int, float] = 0
-    """Number of epochs with no improvement after which training will be stopped."""
-    baseline: Optional[float] = None
-    """Baseline value for the monitored quantity. Training will stop if the driver hits the baseline."""
     monitor: str = "mean"
     """Loss statistic to monitor. Should be one of 'mean', 'variance', 'sigma'."""
+    patience: Union[int, float] = 0
+    """Number of epochs with invalid loss after which training will be stopped."""
 
-    def __post_init__(self):
-        self._best_val = np.infty
-        self._best_iter = 0
+    _last_valid_iter: int = 0
+    """Last valid iteration, to check against patience"""
 
     def __call__(self, step, log_data, driver):
         """
         A boolean function that determines whether or not to stop training.
 
         Args:
             step: An integer corresponding to the step (iteration or epoch) in training.
             log_data: A dictionary containing log data for training.
             driver: A NetKet variational driver.
 
         Returns:
             A boolean. If True, training continues, else, it does not.
         """
         loss = np.real(getattr(log_data[driver._loss_name], self.monitor))
-        if loss < self._best_val:
-            self._best_val = loss
-            self._best_iter = step
-        if self.baseline is not None:
-            if loss <= self.baseline:
+        if not np.isfinite(loss):
+            if step - self._last_valid_iter >= self.patience:
                 return False
-        if (
-            step - self._best_iter >= self.patience
-            and loss >= self._best_val - self.min_delta
-        ):
-            return False
         else:
-            return True
+            self._last_valid_iter = step
+        return True
```

### Comparing `netket-3.8/netket/callbacks/invalidlossstopping.py` & `netket-3.9/netket/callbacks/convergence_stopping.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,44 +9,62 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from dataclasses import dataclass
-from typing import Union
+
+from collections import deque
 
 import numpy as np
 
 
 @dataclass
-class InvalidLossStopping:
-    """A simple callback to stop NetKet if there are no more improvements in the training.
+class ConvergenceStopping:
+    """A simple callback to stop the optimisation if the loss gets below a certain threshold.
     based on `driver._loss_name`."""
 
+    target: float
+    """Target value for the monitored quantity. Training will stop if the driver hits the baseline."""
     monitor: str = "mean"
     """Loss statistic to monitor. Should be one of 'mean', 'variance', 'sigma'."""
-    patience: Union[int, float] = 0
-    """Number of epochs with invalid loss after which training will be stopped."""
+
+    smoothing_window: int = 10
+    """
+    The loss is smoothed over the last `smoothing_window` iterations to reduce statistical fluctuations
+    """
+    patience: int = 10
+    """
+    The loss must be consistently below this value for this number of iterations in order to stop the optimisation.
+    """
 
     def __post_init__(self):
-        self._last_valid_iter = 0
+        self._loss_window: deque = deque([], maxlen=self.smoothing_window)
+        self._patience_counter: int = 0
 
     def __call__(self, step, log_data, driver):
         """
         A boolean function that determines whether or not to stop training.
 
         Args:
             step: An integer corresponding to the step (iteration or epoch) in training.
             log_data: A dictionary containing log data for training.
             driver: A NetKet variational driver.
 
         Returns:
             A boolean. If True, training continues, else, it does not.
         """
         loss = np.real(getattr(log_data[driver._loss_name], self.monitor))
-        if not np.isfinite(loss):
-            if step - self._last_valid_iter >= self.patience:
-                return False
+
+        self._loss_window.append(loss)
+        loss_smooth = np.mean(self._loss_window)
+
+        if loss_smooth <= self.target:
+            self._patience_counter += 1
         else:
-            self._last_valid_iter = step
+            self._patience_counter = 0
+
+        if self._patience_counter > self.patience:
+            return False
+
         return True
```

### Comparing `netket-3.8/netket/driver/__init__.py` & `netket-3.9/netket/utils/struct/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-# Copyright 2021 The NetKet Authors - All rights reserved.
+# Copyright 2020, 2021 The NetKet Authors - All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .abstract_variational_driver import AbstractVariationalDriver
-from .vmc import VMC
-from .steady_state import SteadyState
+# flake8: noqa: F401
 
-from netket.utils import _hide_submodules
-
-_hide_submodules(__name__)
+from .dataclass import dataclass, field, property_cached, Uninitialized
```

### Comparing `netket-3.8/netket/driver/abstract_variational_driver.py` & `netket-3.9/netket/driver/abstract_variational_driver.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/driver/steady_state.py` & `netket-3.9/netket/driver/steady_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
             "SteadyState("
             + f"\n  step_count = {self.step_count},"
             + f"\n  state = {self.state})"
         )
 
     def info(self, depth=0):
         lines = [
-            "{}: {}".format(name, info(obj, depth=depth + 1))
+            f"{name}: {info(obj, depth=depth + 1)}"
             for name, obj in [
                 ("Lindbladian ", self._lind),
                 ("Optimizer   ", self._optimizer),
                 ("SR solver   ", self.sr),
             ]
         ]
         return "\n{}".format(" " * 3 * (depth + 1)).join([str(self)] + lines)
```

### Comparing `netket-3.8/netket/driver/vmc.py` & `netket-3.9/netket/driver/vmc.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,15 +157,15 @@
             "Vmc("
             + f"\n  step_count = {self.step_count},"
             + f"\n  state = {self.state})"
         )
 
     def info(self, depth=0):
         lines = [
-            "{}: {}".format(name, info(obj, depth=depth + 1))
+            f"{name}: {info(obj, depth=depth + 1)}"
             for name, obj in [
                 ("Hamiltonian    ", self._ham),
                 ("Optimizer      ", self._optimizer),
                 ("Preconditioner ", self.preconditioner),
                 ("State          ", self.state),
             ]
         ]
```

### Comparing `netket-3.8/netket/driver/vmc_common.py` & `netket-3.9/netket/driver/vmc_common.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/experimental/__init__.py` & `netket-3.9/netket/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/experimental/driver/__init__.py` & `netket-3.9/netket/experimental/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/experimental/driver/tdvp.py` & `netket-3.9/netket/experimental/driver/tdvp.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,20 @@
 import jax.numpy as jnp
 
 import netket as nk
 from netket.driver.vmc_common import info
 from netket.operator import AbstractOperator
 from netket.optimizer import LinearOperator
 from netket.optimizer.qgt import QGTAuto
-from netket.vqs import VariationalState, VariationalMixedState, MCState, ExactState
+from netket.vqs import (
+    VariationalState,
+    VariationalMixedState,
+    MCState,
+    FullSumState,
+)
 
 from netket.experimental.dynamics import RKIntegratorConfig
 
 from .tdvp_common import TDVPBaseDriver, odefun
 
 
 class TDVP(TDVPBaseDriver):
@@ -51,15 +56,15 @@
         operator: AbstractOperator,
         variational_state: VariationalState,
         integrator: RKIntegratorConfig,
         *,
         t0: float = 0.0,
         propagation_type="real",
         qgt: LinearOperator = None,
-        linear_solver=nk.optimizer.solver.svd,
+        linear_solver=nk.optimizer.solver.pinv_smooth,
         linear_solver_restart: bool = False,
         error_norm: Union[str, Callable] = "euclidean",
     ):
         r"""
         Initializes the time evolution driver.
 
         Args:
@@ -71,17 +76,17 @@
             propagation_type: Determines the equation of motion: "real"  for the
                 real-time Schrödinger equation (SE), "imag" for the imaginary-time SE.
             qgt: The QGT specification.
             linear_solver: The solver for solving the linear system determining the time evolution.
                 This must be a jax-jittable function :code:`f(A,b) -> x` that accepts a Matrix-like, Linear Operator
                 PyTree object :math:`A` and a vector-like PyTree :math:`b` and returns the PyTree :math:`x` solving
                 the system :math:`Ax=b`.
-                Defaults to :func:`nk.optimizer.solver.svd` with the default svd threshold of 1e-10.
+                Defaults to :func:`nk.optimizer.solver.pinv_smooth` with the default svd threshold of 1e-10.
                 To change the svd threshold you can use :func:`functools.partial` as follows:
-                :code:`functools.partial(nk.optimizer.solver.svd, rcond=1e-4)`.
+                :code:`functools.partial(nk.optimizer.solver.pinv_smooth, rcond_smooth=1e-5)`.
             linear_solver_restart: If False (default), the last solution of the linear system
                 is used as initial value in subsequent steps.
             error_norm: Norm function used to calculate the error with adaptive integrators.
                 Can be either "euclidean" for the standard L2 vector norm :math:`w^\dagger w`,
                 "maximum" for the maximum norm :math:`\max_i |w_i|`
                 or "qgt", in which case the scalar product induced by the QGT :math:`S` is used
                 to compute the norm :math:`\Vert w \Vert^2_S = w^\dagger S w` as suggested
@@ -118,28 +123,28 @@
 
         super().__init__(
             operator, variational_state, integrator, t0=t0, error_norm=error_norm
         )
 
     def info(self, depth=0):
         lines = [
-            "{}: {}".format(name, info(obj, depth=depth + 1))
+            f"{name}: {info(obj, depth=depth + 1)}"
             for name, obj in [
                 ("generator     ", self._generator_repr),
                 ("integrator    ", self._integrator),
                 ("linear solver ", self.linear_solver),
                 ("state         ", self.state),
             ]
         ]
         return "\n{}".format(" " * 3 * (depth + 1)).join([str(self)] + lines)
 
 
 @odefun.dispatch
 def odefun_tdvp(  # noqa: F811
-    state: Union[MCState, ExactState], driver: TDVP, t, w, *, stage=0
+    state: Union[MCState, FullSumState], driver: TDVP, t, w, *, stage=0
 ):
     # pylint: disable=protected-access
 
     state.parameters = w
     state.reset()
 
     op_t = driver.generator(t)
```

### Comparing `netket-3.8/netket/experimental/driver/tdvp_common.py` & `netket-3.9/netket/experimental/driver/tdvp_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import netket as nk
 from netket import config
 from netket.driver import AbstractVariationalDriver
 from netket.driver.abstract_variational_driver import _to_iterable
 from netket.jax import HashablePartial
 from netket.logging.json_log import JsonLog
 from netket.operator import AbstractOperator
-from netket.utils import mpi, pure_callback
+from netket.utils import mpi
 from netket.utils.dispatch import dispatch
 from netket.utils.types import PyTree
 from netket.vqs import VariationalState
 
 from netket.experimental.dynamics import RKIntegratorConfig
 from netket.experimental.dynamics._rk_solver_structures import (
     euclidean_norm,
@@ -166,15 +166,15 @@
             if config.netket_experimental_disable_ode_jit:
                 self._error_norm = HashablePartial(qgt_norm, self)
             else:
                 w = self.state.parameters
                 norm_dtype = nk.jax.dtype_real(nk.jax.tree_dot(w, w))
                 # QGT norm is called via host callback since it accesses the driver
                 # TODO: make this also an hashablepartial on self to reduce recompilation
-                self._error_norm = lambda x: pure_callback(
+                self._error_norm = lambda x: jax.pure_callback(
                     HashablePartial(qgt_norm, self),
                     jax.ShapeDtypeStruct((), norm_dtype),
                     x,
                 )
         else:
             raise ValueError(
                 "error_norm must be a callable or one of 'euclidean', 'qgt', 'maximum',"
@@ -247,20 +247,22 @@
                 if not always_stop and len(tstops) > 0:
                     max_dt = tstops[0] - self.t
                 else:
                     max_dt = None
                 step_accepted = self._integrator.step(max_dt=max_dt)
                 if self._integrator.errors:
                     raise RuntimeError(
-                        f"RK solver: {self._integrator.errors.message()}"
+                        f"RK solver: {self._integrator.errors.message()}",
+                        stacklevel=3,
                     )
                 elif self._integrator.warnings:
                     warnings.warn(
                         f"RK solver: {self._integrator.warnings.message()}",
                         UserWarning,
+                        stacklevel=3,
                     )
             self._step_count += 1
             # optionally call callback
             if callback:
                 callback()
 
         # Yield one last time if the remaining tstop is at t_end
@@ -475,14 +477,14 @@
         return odefun(state, driver, *args, **kwargs)
 
     result_shape = jax.tree_map(
         lambda x: jax.ShapeDtypeStruct(x.shape, x.dtype),
         state.parameters,
     )
 
-    return pure_callback(
+    return jax.pure_callback(
         lambda args_and_kw: odefun(state, driver, *args_and_kw[0], **args_and_kw[1]),
         result_shape,
         # pack args and kwargs together, since host_callback passes a single argument:
         (args, kwargs),
     )
     return odefun(state, driver, *args, **kwargs)
```

### Comparing `netket-3.8/netket/experimental/driver/tdvp_schmitt.py` & `netket-3.9/netket/experimental/driver/tdvp_schmitt.py`

 * *Files 20% similar despite different names*

```diff
@@ -39,47 +39,62 @@
     (t-VMC) method.
 
     This driver, which only works with standard MCState variational states, uses the regularization
     procedure described in `M. Schmitt's PRL 125 <https://journals.aps.org/prl/pdf/10.1103/PhysRevLett.125.100503>`_ .
 
     With the force vector
 
-        :math:`F_k=\langle \mathcal O_{\theta_k}^* E_{loc}^{\theta}\rangle_c`
+    .. math::
+
+        F_k=\langle \mathcal O_{\theta_k}^* E_{loc}^{\theta}\rangle_c
 
     and the quantum Fisher matrix
 
-        :math:`S_{k,k'} = \langle \mathcal O_{\theta_k} (\mathcal O_{\theta_{k'}})^*\rangle_c`
+    .. math::
+
+        S_{k,k'} = \langle \mathcal O_{\theta_k} (\mathcal O_{\theta_{k'}})^*\rangle_c
 
     and for real parameters :math:`\theta\in\mathbb R`, the TDVP equation reads
 
-        :math:`q\big[S_{k,k'}\big]\theta_{k'} = -q\big[xF_k\big]`
+    .. math::
+
+        q\big[S_{k,k'}\big]\theta_{k'} = -q\big[xF_k\big]
 
     Here, either :math:`q=\text{Re}` or :math:`q=\text{Im}` and :math:`x=1` for ground state
     search or :math:`x=i` (the imaginary unit) for real time dynamics.
 
     For ground state search a regularization controlled by a parameter :math:`\rho` can be included
     by increasing the diagonal entries and solving
 
-        :math:`q\big[(1+\rho\delta_{k,k'})S_{k,k'}\big]\theta_{k'} = -q\big[F_k\big]`
+    .. math::
+
+        q\big[(1+\rho\delta_{k,k'})S_{k,k'}\big]\theta_{k'} = -q\big[F_k\big]
 
     The `TDVP` class solves the TDVP equation by computing a pseudo-inverse of :math:`S` via
     eigendecomposition yielding
 
-        :math:`S = V\Sigma V^\dagger`
+    .. math::
+
+        S = V\Sigma V^\dagger
 
     with a diagonal matrix :math:`\Sigma_{kk}=\sigma_k`
     Assuming that :math:`\sigma_1` is the smallest eigenvalue, the pseudo-inverse is constructed
     from the regularized inverted eigenvalues
 
-        :math:`\tilde\sigma_k^{-1}=\frac{1}{\Big(1+\big(\frac{\epsilon_{SVD}}{\sigma_j/\sigma_1}\big)^6\Big)\Big(1+\big(\frac{\epsilon_{SNR}}{\text{SNR}(\rho_k)}\big)^6\Big)}`
+    .. math::
+
+        \tilde\sigma_k^{-1}=\frac{1}{\Big(1+\big(\frac{\epsilon_{SVD}}{\sigma_j/\sigma_1}\big)^6\Big)\Big(1+\big(\frac{\epsilon_{SNR}}{\text{SNR}(\rho_k)}\big)^6\Big)}
 
-    with :math:`\text{SNR}(\rho_k)` the signal-to-noise ratio of :math:`\rho_k=V_{k,k'}^{\dagger}F_{k'}` (see `[arXiv:1912.08828] <https://arxiv.org/pdf/1912.08828.pdf>`_ for details).
+    with :math:`\text{SNR}(\rho_k)` the signal-to-noise ratio of
+    :math:`\rho_k=V_{k,k'}^{\dagger}F_{k'}` (see
+    `[arXiv:1912.08828] <https://arxiv.org/pdf/1912.08828.pdf>`_ for details).
 
 
     .. note::
+
         This TDVP Driver uses the time-integrators from the `nkx.dynamics` module, which are
         automatically executed under a `jax.jit` context.
 
         When running computations on GPU, this can lead to infinite hangs or extremely long
         compilation times. In those cases, you might try setting the configuration variable
         `nk.config.netket_experimental_disable_ode_jit = True` to mitigate those issues.
 
@@ -93,17 +108,17 @@
         *,
         t0: float = 0.0,
         propagation_type="real",
         holomorphic: bool = None,
         diag_shift: float = 0.0,
         diag_scale: float = None,
         error_norm: Union[str, Callable] = "qgt",
-        num_tol: float = 1e-14,
-        svd_tol: float = 1e-8,
-        snr_tol: float = 1,
+        rcond: float = 1e-14,
+        rcond_smooth: float = 1e-8,
+        snr_atol: float = 1,
     ):
         r"""
         Initializes the time evolution driver.
 
         Args:
             operator: The generator of the dynamics (Hamiltonian for pure states,
                 Lindbladian for density operators).
@@ -121,16 +136,25 @@
                 Additionally, it possible to pass a custom function with signature
                 :code:`norm(x: PyTree) -> float`
                 which maps a PyTree of parameters :code:`x` to the corresponding norm.
                 Note that norm is used in jax.jit-compiled code.
             holomorphic: a flag to indicate that the wavefunction is holomorphic.
             diag_shift: diagonal shift of the quantum geometric tensor (QGT)
             diag_scale: If not None rescales the diagonal shift of the QGT
-            svd_tol: Regularization parameter :math:`\epsilon_{SVD}`, see above.
-            snr_tol: Regularization parameter :math:`\epsilon_{SNR}`, see above.
+            rcond : Cut-off ratio for small singular :math:`\sigma_k` values of the
+                Quantum Geometric Tensor. For the purposes of rank determination,
+                singular values are treated as zero if they are smaller than rcond times
+                the largest singular value :code:`\sigma_{max}`.
+            rcond_smooth : Smooth cut-off ratio for singular values of the Quantum Geometric
+                Tensor. This regularization parameter used with a similar effect to `rcond`
+                but with a softer curve. See :math:`\epsilon_{SVD}` in the formula
+                above.
+            snr_atol: Noise regularisation absolute tolerance, meaning that eigenvalues of
+                the S matrix that have a signal to noise ratio above this quantity will be
+                (soft) truncated. This is :math:`\epsilon_{SNR}` in the formulas above.
 
         """
         self.propagation_type = propagation_type
         if isinstance(variational_state, VariationalMixedState):
             # assuming Lindblad Dynamics
             # TODO: support density-matrix imaginary time evolution
             if propagation_type == "real":
@@ -143,29 +167,29 @@
             if propagation_type == "real":
                 self._loss_grad_factor = -1.0j
             elif propagation_type == "imag":
                 self._loss_grad_factor = -1.0
             else:
                 raise ValueError("propagation_type must be one of 'real', 'imag'")
 
-        self.num_tol = num_tol
-        self.svd_tol = svd_tol
-        self.snr_tol = snr_tol
+        self.rcond = rcond
+        self.rcond_smooth = rcond_smooth
+        self.snr_atol = snr_atol
 
         self.diag_shift = diag_shift
         self.holomorphic = holomorphic
         self.diag_scale = diag_scale
 
         super().__init__(
             operator, variational_state, integrator, t0=t0, error_norm=error_norm
         )
 
     def info(self, depth=0):
         lines = [
-            "{}: {}".format(name, info(obj, depth=depth + 1))
+            f"{name}: {info(obj, depth=depth + 1)}"
             for name, obj in [
                 ("generator     ", self._generator_repr),
                 ("integrator    ", self._integrator),
                 ("state         ", self.state),
             ]
         ]
         return "\n{}".format(" " * 3 * (depth + 1)).join([str(self)] + lines)
@@ -174,15 +198,15 @@
 # Copyright notice:
 # The function `_impl` below includes lines copied from the jVMC repository
 # found at github.com/markusschmitt/vmc_jax and licensed according to
 # MIT License, Copyright (c) 2021 Markus Schmitt
 
 
 @partial(jax.jit, static_argnames=("n_samples"))
-def _impl(parameters, n_samples, E_loc, S, rhs_coeff, num_tol, svd_tol, snr_tol):
+def _impl(parameters, n_samples, E_loc, S, rhs_coeff, rcond, rcond_smooth, snr_atol):
     E = stats.statistics(E_loc)
     ΔE_loc = E_loc.T.reshape(-1, 1) - E.mean
 
     stack_jacobian = S.mode == "complex"
 
     O = S.O / jnp.sqrt(n_samples)  # already divided by jnp.sqrt(n_s)
     if stack_jacobian:
@@ -203,19 +227,19 @@
     QEdata = Q.conj() * ΔE_loc
     rho = V.conj().T @ F
 
     # Compute the SNR according to Eq. 21
     snr = jnp.abs(rho) * jnp.sqrt(n_samples) / jnp.sqrt(stats.var(QEdata, axis=0))
 
     # Discard eigenvalues below numerical precision
-    ev_inv = jnp.where(jnp.abs(ev / ev[-1]) > num_tol, 1.0 / ev, 0.0)
+    ev_inv = jnp.where(jnp.abs(ev / ev[-1]) > rcond, 1.0 / ev, 0.0)
     # Set regularizer for singular value cutoff
-    regularizer = 1.0 / (1.0 + (svd_tol / jnp.abs(ev / ev[-1])) ** 6)
+    regularizer = 1.0 / (1.0 + (rcond_smooth / jnp.abs(ev / ev[-1])) ** 6)
     # Construct a soft cutoff based on the SNR
-    regularizer2 = regularizer * (1.0 / (1.0 + (snr_tol / snr) ** 6))
+    regularizer2 = regularizer * (1.0 / (1.0 + (snr_atol / snr) ** 6))
 
     # solve the linear system by hand
     eta_p = ev_inv * regularizer2 * rhs_coeff * rho
     # convert back to the parameter space
     update = V @ eta_p
 
     # remainder of the solution
@@ -254,17 +278,17 @@
 
     self._loss_stats, self._dw, self._rmd, self._snr = _impl(
         state.parameters,
         state.n_samples,
         E_loc,
         self._S,
         self._loss_grad_factor,
-        self.num_tol,
-        self.svd_tol,
-        self.snr_tol,
+        self.rcond,
+        self.rcond_smooth,
+        self.snr_atol,
     )
 
     if stage == 0:  # TODO: This does not work with FSAL.
         self._last_qgt = self._S
 
     return self._dw
```

### Comparing `netket-3.8/netket/experimental/dynamics/__init__.py` & `netket-3.9/netket/experimental/dynamics/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/experimental/dynamics/_rk_solver.py` & `netket-3.9/netket/experimental/dynamics/_rk_solver.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,14 +17,33 @@
 
 args_fixed_dt_docstring = """
     Args:
         dt: Timestep (floating-point number).
 """
 
 args_adaptive_docstring = """
+    This solver is adaptive, meaning that the time-step is changed at every
+    iteration in order to keep the error below a certain threshold.
+
+    In particular, given the variables at step :math:`t`, :math:`\\theta^{t}` and the
+    error at the same time-step, :math:`\\epsilon^t`, we compute a rescaled error by
+    using the absolute (**atol**) and relative (**reltol**) tolerances according
+    to this formula.
+
+    .. math::
+
+        \\epsilon^\\text{scaled} = \\text{Norm}(\\frac{\\epsilon^{t}}{\\epsilon_{atol} +
+            \\max(\\theta^t, \\theta^{t-1})\\epsilon_{reltol}}),
+
+    where :math:`\\text{Norm}` is a function that normalises the vector, usually a vector
+    norm but could be something else as well, and :math:`\\max` is an elementwise maximum
+    function (with lexicographical ordering for complex numbers).
+
+    Then, the integrator will attempt to keep `\\epsilon^\\text{scaled}<1`.
+
     Args:
         dt: Timestep (floating-point number). When :code:`adaptive==False` this value
             is never changed, when :code:`adaptive == True` this is the initial timestep.
         adaptive: Whether to use adaptive timestepping (Defaults to False).
             Not all integrators support adaptive timestepping.
         atol: Maximum absolute error at every time-step during adaptive timestepping.
             A larger value will lead to larger timestep. This option is ignored if
@@ -34,15 +53,15 @@
         rtol: Maximum relative error at every time-step during adaptive timestepping.
             A larger value will lead to larger timestep. This option is ignored if
             `adaptive=False`. Note that the `norm` used to compute the error can be
             changed in the :ref:`netket.experimental.TDVP` driver. (Defaults to 1e-7)
         dt_limits: A length-2 tuple of minimum and maximum timesteps considered by
             adaptive time-stepping. A value of None signals that there is no bound.
             Defaults to :code:`(None, 10*dt)`.
-"""
+    """
 
 
 def append_docstring(doc):
     """
     Decorator that appends the string `doc` to the decorated function.
 
     This is needed here because docstrings cannot be f-strings or manipulated strings.
```

### Comparing `netket-3.8/netket/experimental/dynamics/_rk_solver_structures.py` & `netket-3.9/netket/experimental/dynamics/_rk_solver_structures.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/experimental/dynamics/_rk_tableau.py` & `netket-3.9/netket/experimental/dynamics/_rk_tableau.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/experimental/hilbert/__init__.py` & `netket-3.9/netket/experimental/hilbert/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/experimental/hilbert/spin_orbital_fermions.py` & `netket-3.9/netket/experimental/hilbert/spin_orbital_fermions.py`

 * *Files 8% similar despite different names*

```diff
@@ -95,23 +95,24 @@
             hilbert = TensorDiscreteHilbert(*spin_hilberts)
 
         self._fock = hilbert
         """Internal representation of this Hilbert space (Fock or TensorHilbert)."""
         # local states are the occupation numbers (0, 1)
         local_states = np.array((0.0, 1.0))
 
-        # we use the constraints from the Fock spaces, and override is_constrained later
+        # we use the constraints from the Fock spaces, and override `constrained`
         super().__init__(local_states, N=total_size, constraint_fn=None)
         self._s = s
         self.n_fermions = n_fermions
-        self._is_constrained = n_fermions is not None
         self.n_orbitals = n_orbitals
+
         # we copy the respective functions, independent of what hilbert space they are
         self._numbers_to_states = self._fock._numbers_to_states
         self._states_to_numbers = self._fock._states_to_numbers
+        self.all_states = self._fock.all_states
 
     def __repr__(self):
         _str = f"SpinOrbitalFermions(n_orbitals={self.n_orbitals}"
         if self.n_fermions is not None:
             _str += f", n_fermions={self.n_fermions}"
         if self.spin is not None:
             _str += f", s={Fraction(self.spin)}"
@@ -130,16 +131,16 @@
         return self._fock.size
 
     @property
     def _attrs(self):
         return (self.spin, self.n_fermions, self.n_orbitals)
 
     @property
-    def is_constrained(self):
-        return self._is_constrained
+    def constrained(self):
+        return self.n_fermions is not None
 
     @property
     def is_finite(self) -> bool:
         return self._fock.is_finite
 
     @property
     def n_states(self) -> int:
```

### Comparing `netket-3.8/netket/experimental/hilbert/random/__init__.py` & `netket-3.9/netket/experimental/hilbert/random/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/experimental/hilbert/random/spin_orbital_fermions.py` & `netket-3.9/netket/experimental/hilbert/random/spin_orbital_fermions.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/experimental/logging/__init__.py` & `netket-3.9/netket/experimental/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/experimental/logging/hdf5_log.py` & `netket-3.9/netket/experimental/logging/hdf5_log.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/experimental/operator/__init__.py` & `netket-3.9/netket/experimental/operator/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/experimental/operator/_fermion_operator_2nd.py` & `netket-3.9/netket/experimental/operator/_fermion_operator_2nd.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 import numpy as np
 from jax.tree_util import tree_map
 import copy
 import numba
 
 from netket.utils.types import DType
 from netket.operator._discrete_operator import DiscreteOperator
-from netket.operator._pauli_strings import _count_of_locations
+from netket.operator._pauli_strings.base import _count_of_locations
 from netket.hilbert.abstract_hilbert import AbstractHilbert
 from netket.utils.numbers import is_scalar, dtype as _dtype
+from netket.errors import concrete_or_error, NumbaOperatorGetConnDuringTracingError
 
 from netket.experimental.hilbert import SpinOrbitalFermions
 
 from ._fermion_operator_2nd_utils import (
     _convert_terms_to_spin_blocks,
     _collect_constants,
     _canonicalize_input,
@@ -337,15 +338,22 @@
                 See numpy.split for the meaning of sections.
 
         Returns:
             matrix: The connected states x', flattened together in a single matrix.
             array: An array containing the matrix elements :math:`O(x,x')` associated to each x'.
         """
         self._setup()
-        x = np.array(x)
+
+        x = concrete_or_error(
+            np.asarray,
+            x,
+            NumbaOperatorGetConnDuringTracingError,
+            self,
+        )
+
         assert (
             x.shape[-1] == self.hilbert.size
         ), "size of hilbert space does not match size of x"
         return self._flattened_kernel(
             x,
             sections,
             self.max_conn_size,
```

### Comparing `netket-3.8/netket/experimental/operator/_fermion_operator_2nd_utils.py` & `netket-3.9/netket/experimental/operator/_fermion_operator_2nd_utils.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/experimental/operator/fermion.py` & `netket-3.9/netket/experimental/operator/fermion.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/experimental/qsr/__init__.py` & `netket-3.9/netket/experimental/qsr/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/experimental/qsr/dataset.py` & `netket-3.9/netket/experimental/qsr/dataset.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/experimental/qsr/driver.py` & `netket-3.9/netket/experimental/qsr/driver.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,16 @@
         self._chunk_size = chunk_size
 
         # chunk
         if self._chunk_size is not None:
             self.n_chunk = self.dataset.size // self._chunk_size
             if not self.n_chunk * self._chunk_size == self.dataset.size:
                 warnings.warn(
-                    "WARNING: chunk size does not divide the number of samples, the last few chunks will be smaller"
+                    "WARNING: chunk size does not divide the number of samples, the last few chunks will be smaller",
+                    stacklevel=2,
                 )
             self._chunked_indices = np.array_split(
                 np.arange(self.dataset.size), self.n_chunk
             )
 
     @property
     def dataset(self):
@@ -518,15 +519,15 @@
             "QSR("
             + f"\n  step_count = {self.step_count},"
             + f"\n  state = {self.state})"
         )
 
     def info(self, depth=0):
         lines = [
-            "{}: {}".format(name, info(obj, depth=depth + 1))
+            f"{name}: {info(obj, depth=depth + 1)}"
             for name, obj in [
                 ("Optimizer   ", self._optimizer),
                 ("SR solver   ", self.sr),
                 ("State       ", self.state),
             ]
         ]
         return "\n{}".format(" " * 3 * (depth + 1)).join([str(self)] + lines)
```

### Comparing `netket-3.8/netket/experimental/qsr/logic_helpers.py` & `netket-3.9/netket/experimental/qsr/logic_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import numpy as np
 import jax
 import jax.numpy as jnp
 
 from netket import jax as nkjax
 from netket.operator import AbstractOperator
 from netket.hilbert import AbstractHilbert
-from netket.vqs import ExactState
+from netket.vqs import FullSumState
 from netket.utils import mpi
 from netket.utils.types import Array
 from netket.utils.dispatch import dispatch
 
 BaseType = Union[AbstractOperator, np.ndarray, str]
 
 
@@ -72,29 +72,29 @@
         state_diag.samples,
     )
 
 
 @partial(jax.jit, static_argnums=(0, 1))
 def _avg_O_exact(hilbert: AbstractHilbert, afun, pars, model_state):
     r"""
-    Same as _avg_O, but for ExactState.
+    Same as _avg_O, but for FullSumState.
     """
     sigma = hilbert.all_states()
     sigma = sigma.reshape((-1, sigma.shape[-1]))
     _, vjp = nkjax.vjp(lambda W: afun({"params": W, **model_state}, sigma), pars)
     psi_2 = jnp.abs(jnp.exp(afun({"params": pars, **model_state}, sigma))) ** 2
     psi_2 /= jnp.sum(psi_2)
     (O_avg,) = vjp(psi_2)
     return jax.tree_map(lambda x: mpi.mpi_mean_jax(x)[0], O_avg)
 
 
 @dispatch
-def _grad_negative(state_diag: ExactState):  # noqa: F811
+def _grad_negative(state_diag: FullSumState):  # noqa: F811
     r"""
-    Same as _grad_negative, but for ExactState.
+    Same as _grad_negative, but for FullSumState.
     """
     return _avg_O_exact(
         state_diag._hilbert,
         state_diag._apply_fun,
         state_diag.parameters,
         state_diag.model_state,
     )
```

### Comparing `netket-3.8/netket/experimental/sampler/__init__.py` & `netket-3.9/netket/experimental/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/experimental/sampler/metropolis_pmap.py` & `netket-3.9/netket/experimental/sampler/metropolis_pmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,15 @@
         if kwargs["n_chains_per_rank"] != n_chains_per_device * n_devices:
             import warnings
 
             warnings.warn(
                 f"Using {n_chains_per_device*n_devices} chains "
                 f"({n_chains_per_device} chains on each of {n_devices} devices).",
                 category=UserWarning,
+                stacklevel=2,
             )
 
         return args, kwargs
 
     def __post_init__(self):
         super().__post_init__()
 
@@ -195,18 +196,15 @@
         state = MetropolisSamplerPmapState(
             σ=state.σ,
             rng=state.rng,
             rule_state=state.rule_state,
             n_steps_proc=state.n_steps_proc,
             n_accepted_proc=state.n_accepted_proc,
         )
-        return samples.reshape(samples.shape[0], -1, samples.shape[-1]), state
-
-    def _repr_pretty_(sampler, p, cycle):
-        super()._repr_pretty_(p, cycle)
+        return samples.reshape((-1,) + samples.shape[-2:]), state
 
 
 @partial(
     jax.pmap, in_axes=(None, None, None, 0), out_axes=0, static_broadcasted_argnums=1
 )
 def _init_state_pmap(sampler, machine, parameters, key):
     return sampler._init_state(machine, parameters, key)
@@ -228,12 +226,12 @@
 def _sample_next_pmap(sampler, machine, parameters, state):
     return sampler._sample_next(machine, parameters, state)
 
 
 @partial(
     jax.pmap,
     in_axes=(None, None, None, 0, None),
-    out_axes=(1, 0),
+    out_axes=(0, 0),
     static_broadcasted_argnums=(1, 4),
 )
 def _sample_chain_pmap(sampler, machine, parameters, state, chain_length):
     return sampler._sample_chain(machine, parameters, state, chain_length)
```

### Comparing `netket-3.8/netket/experimental/sampler/metropolis_pt.py` & `netket-3.9/netket/experimental/sampler/metropolis_pt.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,23 +41,17 @@
         if self.n_steps > 0:
             acc_string = "# accepted = {}/{} ({}%), ".format(
                 self.n_accepted, self.n_steps, self.acceptance * 100
             )
         else:
             acc_string = ""
 
-        text = (
-            "MetropolisNumpySamplerState("
-            + acc_string
-            + "rng state={})".format(self.rng)
-        )
+        text = "MetropolisNumpySamplerState(" + acc_string + f"rng state={self.rng})"
 
-        text = (
-            "MetropolisPtSamplerState(" + acc_string + "rng state={}".format(self.rng)
-        )
+        text = "MetropolisPtSamplerState(" + acc_string + f"rng state={self.rng}"
         return text
 
 
 _init_doc = r"""
 ``MetropolisSampler`` is a generic Metropolis-Hastings sampler using
 a transition rule to perform moves in the Markov Chain.
 The transition kernel is used to generate
@@ -157,15 +151,15 @@
             rule_state=rule_state,
             n_steps_proc=0,
             n_accepted_proc=0,
             n_accepted_per_beta=jnp.zeros(
                 (sampler.n_chains, sampler.n_replicas), dtype=jnp.int64
             ),
             beta_position=jnp.zeros((sampler.n_chains,)),
-            beta_diffusion=jnp.zeros((sampler.n_chains)),
+            beta_diffusion=jnp.zeros(sampler.n_chains),
             exchange_steps=0,
             # beta=beta,
             # beta_0_index=jnp.zeros((sampler.n_chains,), dtype=jnp.int64),
         )
 
     def _sample_next(
         sampler, machine, parameters: PyTree, state: MetropolisPtSamplerState
```

### Comparing `netket-3.8/netket/experimental/vqs/__init__.py` & `netket-3.9/netket/experimental/vqs/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/experimental/vqs/io.py` & `netket-3.9/netket/experimental/vqs/io.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/graph/__init__.py` & `netket-3.9/netket/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/graph/_lattice_edge_logic.py` & `netket-3.9/netket/graph/_lattice_edge_logic.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/graph/abstract_graph.py` & `netket-3.9/netket/graph/abstract_graph.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/graph/common_lattices.py` & `netket-3.9/netket/graph/common_lattices.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/graph/graph.py` & `netket-3.9/netket/graph/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
             return self._igraph.es.get_attribute_values("color")
         else:
             return []
 
     # Graph algorithms
     # ------------------------------------------------------------------------
     def distances(self) -> List[List]:
-        return np.array(self._igraph.shortest_paths())
+        return np.array(self._igraph.distances())
 
     def _compute_automorphisms(self):
         """
         Compute the graph autmorphisms of this graph.
         """
         colors = self.edge_colors
         result = self._igraph.get_isomorphisms_vf2(
```

### Comparing `netket-3.8/netket/graph/lattice.py` & `netket-3.9/netket/graph/lattice.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,27 +316,29 @@
             raise ValueError(
                 "'basis_vectors' must have ndim==2 (as array of primitive vectors)"
             )
         if basis_vectors.shape[0] != basis_vectors.shape[1]:
             raise ValueError("The number of primitive vectors must match their length")
         return basis_vectors
 
+    # TODO: remove atoms_coord argument.
     @staticmethod
     def _clean_site_offsets(site_offsets, atoms_coord, basis_vectors):
         """Check and convert `site_offsets` init argument."""
         if atoms_coord is not None and site_offsets is not None:
             raise ValueError(
                 "atoms_coord is deprecated and replaced by site_offsets, "
                 "so both cannot be specified at the same time."
             )
         if atoms_coord is not None:
             warnings.warn(
                 "atoms_coord is deprecated and may be removed in future versions, "
                 "please use site_offsets instead",
                 FutureWarning,
+                stacklevel=3,
             )
             site_offsets = atoms_coord
 
         if site_offsets is None:
             site_offsets = _np.zeros(basis_vectors.shape[0])[None, :]
 
         site_offsets = _np.asarray(site_offsets)
```

### Comparing `netket-3.8/netket/graph/space_group.py` & `netket-3.9/netket/graph/space_group.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/hilbert/__init__.py` & `netket-3.9/netket/hilbert/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/hilbert/abstract_hilbert.py` & `netket-3.9/netket/hilbert/abstract_hilbert.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/hilbert/continuous_hilbert.py` & `netket-3.9/netket/hilbert/continuous_hilbert.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/hilbert/custom_hilbert.py` & `netket-3.9/netket/hilbert/custom_hilbert.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/hilbert/discrete_hilbert.py` & `netket-3.9/netket/hilbert/discrete_hilbert.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from textwrap import dedent
 from functools import reduce
 
 import numpy as np
 
 from netket.utils.types import Array
 from netket.utils.numbers import is_scalar
+from netket.errors import HilbertIndexingDuringTracingError, concrete_or_error
 
 from .abstract_hilbert import AbstractHilbert
 
 max_states = np.iinfo(np.int32).max
 """int: Maximum number of states that can be indexed"""
 
 
@@ -117,14 +118,19 @@
         Throws an exception iff the space is not indexable.
 
         Args:
             numbers (numpy.array): Batch of input numbers to be converted into arrays of
                 quantum numbers.
             out: Optional Array of quantum numbers corresponding to numbers.
         """
+
+        numbers = concrete_or_error(
+            np.asarray, numbers, HilbertIndexingDuringTracingError
+        )
+
         if out is None:
             out = np.empty((np.atleast_1d(numbers).shape[0], self.size))
 
         if np.any(numbers >= self.n_states):
             raise ValueError("numbers outside the range of allowed states")
 
         if is_scalar(numbers):
@@ -149,14 +155,18 @@
         """
         if states.shape[-1] != self.size:
             raise ValueError(
                 f"Size of this state ({states.shape[-1]}) not"
                 f"corresponding to this hilbert space {self.size}"
             )
 
+        states = concrete_or_error(
+            np.asarray, states, HilbertIndexingDuringTracingError
+        )
+
         states_r = np.asarray(np.reshape(states, (-1, states.shape[-1])))
 
         if out is None:
             out = np.empty(states_r.shape[:-1], dtype=np.int64)
 
         out = self._states_to_numbers(states_r, out=out.reshape(-1))
```

### Comparing `netket-3.8/netket/hilbert/doubled_hilbert.py` & `netket-3.9/netket/hilbert/doubled_hilbert.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,12 +142,12 @@
 
         return out
 
     def states_to_local_indices(self, x):
         return self.physical.states_to_local_indices(x)
 
     def __repr__(self):
-        return "DoubledHilbert({})".format(self.physical)
+        return f"DoubledHilbert({self.physical})"
 
     @property
     def _attrs(self):
         return (self.physical,)
```

### Comparing `netket-3.8/netket/hilbert/fock.py` & `netket-3.9/netket/hilbert/fock.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,20 +143,20 @@
         if self.size - Nsites == 0:
             return None
         else:
             return Fock(self.n_max, N=self.size - Nsites)
 
     def __repr__(self):
         n_particles = (
-            ", n_particles={}".format(self._n_particles)
+            f", n_particles={self._n_particles}"
             if self._n_particles is not None
             else ""
         )
         nmax = self._n_max if self._n_max < FOCK_MAX else "FOCK_MAX"
-        return "Fock(n_max={}{}, N={})".format(nmax, n_particles, self.size)
+        return f"Fock(n_max={nmax}{n_particles}, N={self.size})"
 
     def states_to_local_indices(self, x):
         return x.astype(np.int32)
 
     @property
     def _attrs(self):
         return (self.size, self._n_max, self._n_particles)
```

### Comparing `netket-3.8/netket/hilbert/hilbert_index.py` & `netket-3.9/netket/hilbert/index/unconstrained.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,50 +22,44 @@
     ("_local_size", int64),
     ("_size", int64),
     ("_basis", int64[:]),
 ]
 
 
 @jitclass(spec)
-class HilbertIndex:
+class UnconstrainedHilbertIndex:
     def __init__(self, local_states, size):
-        self._local_states = np.sort(local_states)
+        self._local_states = np.sort(local_states).astype(np.float64)
         self._local_size = len(self._local_states)
         self._size = size
 
         self._basis = np.zeros(size, dtype=np.int64)
         ba = 1
         for s in range(size):
             self._basis[s] = ba
             ba *= self._local_size
 
     def _local_state_number(self, x):
         return np.searchsorted(self.local_states, x)
 
     @property
+    def size(self) -> int:
+        return self._size
+
+    @property
     def n_states(self):
         return self._local_size**self._size
 
     @property
     def local_states(self):
         return self._local_states
 
-    def state_to_number(self, state):
-        if state.ndim != 1:
-            raise RuntimeError("Invalid input shape, expecting a 1d array.")
-
-        # Converts a vector of quantum numbers into the unique integer identifier
-        number = 0
-
-        for i in range(self._size):
-            number += (
-                self._local_state_number(state[self._size - i - 1]) * self._basis[i]
-            )
-
-        return number
+    @property
+    def local_size(self) -> int:
+        return self._local_size
 
     def number_to_state(self, number, out=None):
 
         if out is None:
             out = np.empty(self._size)
         # else:
         #     assert out.size == self._size
@@ -104,16 +98,16 @@
             raise RuntimeError("Invalid input shape, expecting a 1d array.")
 
         if out is None:
             out = np.empty((numbers.shape[0], self._size))
         # else:
         #     assert out.shape == (numbers.shape[0], self._size)
 
-        for i in range(numbers.shape[0]):
-            out[i] = self.number_to_state(numbers[i])
+        for i, n in enumerate(numbers):
+            out[i] = self.number_to_state(n)
 
         return out
 
     def all_states(self, out=None):
         if out is None:
             out = np.empty((self.n_states, self._size))
```

### Comparing `netket-3.8/netket/hilbert/homogeneous.py` & `netket-3.9/netket/hilbert/homogeneous.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,57 +9,44 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Optional, List, Callable
-from functools import lru_cache
 
 from numbers import Real
 
 import numpy as np
 
 from .discrete_hilbert import DiscreteHilbert
-from .hilbert_index import HilbertIndex
-
-
-# This function has exponential runtime in self.size, so we cache it in order to
-# only compute it once.
-# TODO: distribute over MPI... chose better chunk size
-@lru_cache(maxsize=5)
-def compute_constrained_to_bare_conversion_table(self, *, chunk_size: int = 100000):
-    """
-    Computes the conversion table that converts the 'constrained' indices
-    of an hilbert space to bare indices, so that routines generating
-    only values in an unconstrained space can be used.
-
-    This function operates on blocks of `chunk_size` states at a time in order
-    to lower the memory cost. The default chunk size has been chosen by instinct
-    and is likely wrong.
-    """
-    n_chunks = int(np.ceil(self._hilbert_index.n_states / chunk_size))
-    bare_number_chunks = []
-    for i in range(n_chunks):
-        id_start = chunk_size * i
-        id_end = np.minimum(chunk_size * (i + 1), self._hilbert_index.n_states)
-        ids = np.arange(id_start, id_end)
-
-        states = self._hilbert_index.numbers_to_states(ids)
-        is_constrained = self._constraint_fn(states)
-        (chunk_bare_number,) = np.nonzero(is_constrained)
-        bare_number_chunks.append(chunk_bare_number + id_start)
-
-    return np.concatenate(bare_number_chunks)
+from .index import HilbertIndex, UnconstrainedHilbertIndex, ConstrainedHilbertIndex
 
 
 class HomogeneousHilbert(DiscreteHilbert):
     r"""The Abstract base class for homogeneous hilbert spaces.
 
     This class should only be subclassed and should not be instantiated directly.
+
+    .. note::
+
+        To override the logic to index into constrained hilbert spaces, it is
+        possible to use an informal interface built on top of non-public
+        indexing classes.
+
+        In particular, you can override the following properties and methods:
+
+            - Do not specify the {code}`constraint_fn` keyword argument when
+              calling the init method of this abstract class.
+            - Override the property {prop}`~nk.hilbert.HomogeneousHilbert.is_constrained`,
+              to return `True` or `False`depending on your own logic.
+            - Override the property {code}`~nk.hilbert.HomogeneousHilbert._hilbert_index`
+              to return an hilbert index object (see the discussion in the source code of
+              the folder {code}`netket/hilbert/index/__init__.py`).
+
     """
 
     def __init__(
         self,
         local_states: Optional[List[Real]],
         N: int = 1,
         constraint_fn: Optional[Callable] = None,
@@ -92,15 +79,14 @@
             self._local_states = None
             self._local_states_frozen = None
             self._local_size = np.iinfo(np.intp).max
 
         self._constraint_fn = constraint_fn
 
         self.__hilbert_index = None
-        self.__bare_numbers = None
 
         shape = tuple(self._local_size for _ in range(N))
         super().__init__(shape=shape)
 
     @property
     def size(self) -> int:
         r"""The total number number of degrees of freedom."""
@@ -123,80 +109,85 @@
     def states_at_index(self, i: int):
         return self.local_states
 
     @property
     def n_states(self) -> int:
         r"""The total dimension of the many-body Hilbert space.
         Throws an exception iff the space is not indexable."""
-        if not self.constrained:
-            return self._hilbert_index.n_states
-        else:
-            return self._bare_numbers.shape[0]
+        return self._hilbert_index.n_states
 
     @property
     def is_finite(self) -> bool:
         r"""Whether the local hilbert space is finite."""
         return self._is_finite
 
     @property
     def constrained(self) -> bool:
         r"""Returns True if the hilbert space is constrained."""
         return self._constraint_fn is not None
 
     def _numbers_to_states(self, numbers: np.ndarray, out: np.ndarray) -> np.ndarray:
-        if self.constrained:
-            numbers = self._bare_numbers[numbers]
 
-        return self._hilbert_index.numbers_to_states(np.asarray(numbers), out)
+        # this is guaranteed
+        # numbers = concrete_or_error(
+        #    np.asarray, numbers, HilbertIndexingDuringTracingError
+        # )
+
+        return self._hilbert_index.numbers_to_states(numbers, out)
 
     def _states_to_numbers(self, states: np.ndarray, out: np.ndarray):
-        self._hilbert_index.states_to_numbers(states, out)
 
-        if self.constrained:
-            out[:] = np.searchsorted(self._bare_numbers, out)
+        # guaranteed
+        # states = concrete_or_error(
+        #    np.asarray, states, HilbertIndexingDuringTracingError
+        # )
 
-            if np.max(out) >= self.n_states:
-                raise RuntimeError(
-                    "The required state does not satisfy " "the given constraints."
-                )
+        self._hilbert_index.states_to_numbers(states, out)
 
         return out
 
+    def all_states(self, out: Optional[np.ndarray] = None) -> np.ndarray:
+        r"""Returns all valid states of the Hilbert space.
+
+        Throws an exception if the space is not indexable.
+
+        Args:
+            out: an optional pre-allocated output array
+
+        Returns:
+            A (n_states x size) batch of states. this corresponds
+            to the pre-allocated array if it was passed.
+        """
+        return self._hilbert_index.all_states(out)
+
     @property
     def _hilbert_index(self) -> HilbertIndex:
         """
         Returns the `HilbertIndex` object, which is a numba jitclass used to convert
         integers to states and vice-versa.
         """
         if self.__hilbert_index is None:
             if not self.is_indexable:
                 raise RuntimeError("The hilbert space is too large to be indexed.")
 
-            self.__hilbert_index = HilbertIndex(
-                np.asarray(self.local_states, dtype=np.float64), self.size
-            )
+            if self.constrained:
+                self.__hilbert_index = ConstrainedHilbertIndex(
+                    np.asarray(self.local_states, dtype=np.float64),
+                    self.size,
+                    self._constraint_fn,
+                )
+            else:
+                self.__hilbert_index = UnconstrainedHilbertIndex(
+                    np.asarray(self.local_states, dtype=np.float64), self.size
+                )
 
         return self.__hilbert_index
 
-    @property
-    def _bare_numbers(self) -> np.ndarray:
-        """
-        Returns the conversion table between indices in the constrained space and
-        the corresponding unconstrained space.
-        """
-        if not self.constrained:
-            return None
-
-        if self.__bare_numbers is None:
-            self.__bare_numbers = compute_constrained_to_bare_conversion_table(self)
-
-        return self.__bare_numbers
-
     def __repr__(self):
-        constr = ", constrained={}".format(self.constrained) if self.constrained else ""
+        constr = f", constrained={self.constrained}" if self.constrained else ""
 
         clsname = type(self).__name__
         return f"{clsname}(local_size={self._local_size}, N={self.size}{constr})"
 
     @property
     def _attrs(self):
         return (
```

### Comparing `netket-3.8/netket/hilbert/particle.py` & `netket-3.9/netket/hilbert/particle.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/hilbert/qubit.py` & `netket-3.9/netket/hilbert/qubit.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,12 +62,12 @@
 
         if self.size - Nsites == 0:
             return None
         else:
             return Qubit(N=self.size - Nsites)
 
     def __repr__(self):
-        return "Qubit(N={})".format(self.size)
+        return f"Qubit(N={self.size})"
 
     @property
     def _attrs(self):
         return (self.size,)
```

### Comparing `netket-3.8/netket/hilbert/spin.py` & `netket-3.9/netket/hilbert/spin.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,15 +137,13 @@
             return Spin(s=self._s, N=self.size - Nsites)
 
     def states_to_local_indices(self, x):
         numbers = (x + self.local_size - 1) / 2
         return numbers.astype(np.int32)
 
     def __repr__(self):
-        total_sz = (
-            ", total_sz={}".format(self._total_sz) if self._total_sz is not None else ""
-        )
-        return "Spin(s={}{}, N={})".format(Fraction(self._s), total_sz, self.size)
+        total_sz = f", total_sz={self._total_sz}" if self._total_sz is not None else ""
+        return f"Spin(s={Fraction(self._s)}{total_sz}, N={self.size})"
 
     @property
     def _attrs(self):
         return (self.size, self._s, self._total_sz)
```

### Comparing `netket-3.8/netket/hilbert/tensor_hilbert.py` & `netket-3.9/netket/hilbert/tensor_hilbert.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
         if cls is TensorHilbert:
             if all(isinstance(hi, DiscreteHilbert) for hi in args):
                 cls = TensorDiscreteHilbert
             else:
                 cls = TensorGenericHilbert
 
-        return super(TensorHilbert, cls).__new__(cls)
+        return super().__new__(cls)
 
     def __init__(self, hilb_spaces: Iterable[AbstractHilbert], *args, **kwargs):
         r"""Constructs a tensor Hilbert space.
 
         Args:
             *hilb: An iterable object containing at least 1 hilbert space.
         """
@@ -154,17 +154,17 @@
 
                 return hilb
 
     def __repr__(self):
         if len(self._hilbert_spaces) == 1:
             return f"{type(self).__name__}({self._hilbert_spaces[0]})"
 
-        _str = "{}".format(self._hilbert_spaces[0])
+        _str = f"{self._hilbert_spaces[0]}"
         for hi in self._hilbert_spaces[1:]:
-            _str += "⊗{}".format(hi)
+            _str += f"⊗{hi}"
 
         return _str
 
 
 class TensorGenericHilbert(TensorHilbert, AbstractHilbert):
     def __init__(self, *hilb_spaces: AbstractHilbert):
         if not all(isinstance(hi, AbstractHilbert) for hi in hilb_spaces):
```

### Comparing `netket-3.8/netket/hilbert/tensor_hilbert_discrete.py` & `netket-3.9/netket/hilbert/tensor_hilbert_discrete.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/hilbert/random/__init__.py` & `netket-3.9/netket/hilbert/random/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/hilbert/random/base.py` & `netket-3.9/netket/hilbert/random/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,18 +25,18 @@
 
 @dispatch
 def random_state(hilb, key, *, size=None, dtype=np.float32):
     r"""Generates either a single or a batch of uniformly distributed random states.
 
     Args:
         hilb: The hilbert space
-        key: The Jax PRNGKey
-        size: If provided, returns a batch of configurations of the form (size, #) if
-            size is an integer or (*size, #) if it is a tuple and where # is the Hilbert
-            space size. By default, a single random configuration with shape (#,) is
+        key: The Jax :class:`jax.random.KeyArray` generated by :func:`jax.random.PRNGKey`.
+        size: If provided, returns a batch of configurations of the form `(size, #)` if
+            size is an integer or `(*size, #)` if it is a tuple and where `#` is the Hilbert
+            space size. By default, a single random configuration with shape `(#,)` is
             returned.
         dtype: The dtype of the resulting states.
 
     Example:
 
         >>> import netket, jax
         >>> hi = netket.hilbert.Qubit(N=2)
```

### Comparing `netket-3.8/netket/hilbert/random/custom.py` & `netket-3.9/netket/hilbert/random/custom.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/hilbert/random/doubled.py` & `netket-3.9/netket/hilbert/random/doubled.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/hilbert/random/fock.py` & `netket-3.9/netket/hilbert/random/fock.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,28 +14,27 @@
 
 import jax
 import numpy as np
 from jax import numpy as jnp
 
 from netket.hilbert import Fock
 from netket.utils.dispatch import dispatch
-from netket.utils import pure_callback
 
 
 @dispatch
 def random_state(hilb: Fock, key, batches: int, *, dtype=np.float32):
     shape = (batches, hilb.size)
 
     # If unconstrained space, use fast sampling
     if hilb.n_particles is None:
         rs = jax.random.randint(key, shape=shape, minval=0, maxval=hilb.n_max + 1)
         return jnp.asarray(rs, dtype=dtype)
 
     else:
-        state = pure_callback(
+        state = jax.pure_callback(
             lambda rng: _random_states_with_constraint(hilb, rng, batches, dtype),
             jax.ShapeDtypeStruct(shape, dtype),
             key,
         )
 
         return state
```

### Comparing `netket-3.8/netket/hilbert/random/particle.py` & `netket-3.9/netket/hilbert/random/particle.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,20 @@
     )
     return x[ind, :]
 
 
 @dispatch
 def random_state(hilb: Particle, key, batches: int, *, dtype):
     """If no periodic boundary conditions are present particles are positioned normally distributed around the origin.
+
     If periodic boundary conditions are present the particles are positioned uniformly inside the box and a small
     gaussian noise is added on top.
     If periodic boundary conditions are chosen only for certain dimensions, the periodic initialization is used for
-    all of those dimensions and the free initialization is used for all the other ones."""
+    all of those dimensions and the free initialization is used for all the other ones.
+    """
     pbc = np.array(hilb.n_particles * hilb.pbc)
     boundary = np.tile(pbc, (batches, 1))
 
     Ls = np.array(hilb.n_particles * hilb.extent)
 
     # If we have PBCs this defines the size of the Gaussian noise in the particle positions.
     # Without PBCs this is never needed (initialization with random Gaussian)
```

### Comparing `netket-3.8/netket/hilbert/random/qubit.py` & `netket-3.9/netket/hilbert/random/qubit.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/hilbert/random/spin.py` & `netket-3.9/netket/hilbert/random/spin.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 import jax
 import numpy as np
 from jax import numpy as jnp
 
 from netket.hilbert import Spin
 from netket.utils.dispatch import dispatch
-from netket.utils import pure_callback
 
 
 @dispatch
 def random_state(hilb: Spin, key, batches: int, *, dtype=np.float32):
     S = hilb._s
     shape = (batches, hilb.size)
 
@@ -59,15 +58,15 @@
             return jax.vmap(jax.random.permutation)(
                 jax.random.split(key, x.shape[0]), x
             )
 
         # if constrained and S != 1/2, then use a slow fallback algorithm
         # TODO: find better, faster way to sample constrained arbitrary spaces.
         else:
-            state = pure_callback(
+            state = jax.pure_callback(
                 lambda rng: _random_states_with_constraint(hilb, rng, batches, dtype),
                 jax.ShapeDtypeStruct(shape, dtype),
                 key,
             )
 
             return state
```

### Comparing `netket-3.8/netket/hilbert/random/tensor_hilbert.py` & `netket-3.9/netket/hilbert/random/tensor_hilbert.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/jax/__init__.py` & `netket-3.9/netket/jax/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from netket.utils import HashablePartial
 
 from .utils import (
     tree_ravel,
     is_complex_dtype,
     tree_size,
     eval_shape,
+    tree_leaf_isreal,
     tree_leaf_iscomplex,
     tree_ishomogeneous,
     dtype_complex,
     dtype_real,
     maybe_promote_to_complex,
     tree_conj,
     tree_dot,
```

### Comparing `netket-3.8/netket/jax/_chunk_utils.py` & `netket-3.9/netket/jax/_chunk_utils.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/jax/_expect.py` & `netket-3.9/netket/jax/_expect.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,28 +49,28 @@
 # Does not support higher-order derivatives yet
 @partial(jax.custom_vjp, nondiff_argnums=(0, 1, 2))
 def _expect(n_chains, log_pdf, expected_fun, pars, σ, *expected_fun_args):
     L_σ = expected_fun(pars, σ, *expected_fun_args)
     if n_chains is not None:
         L_σ = L_σ.reshape((n_chains, -1))
 
-    L̄_σ = mpi_statistics(L_σ.T)
+    L̄_σ = mpi_statistics(L_σ)
     # L̄_σ = L_σ.mean(axis=0)
 
     return L̄_σ.mean, L̄_σ
 
 
 def _expect_fwd(n_chains, log_pdf, expected_fun, pars, σ, *expected_fun_args):
     L_σ = expected_fun(pars, σ, *expected_fun_args)
     if n_chains is not None:
         L_σ_r = L_σ.reshape((n_chains, -1))
     else:
         L_σ_r = L_σ
 
-    L̄_stat = mpi_statistics(L_σ_r.T)
+    L̄_stat = mpi_statistics(L_σ_r)
 
     L̄_σ = L̄_stat.mean
     # L̄_σ = L_σ.mean(axis=0)
 
     # Use the baseline trick to reduce the variance
     ΔL_σ = L_σ - L̄_σ
```

### Comparing `netket-3.8/netket/jax/_grad.py` & `netket-3.9/netket/jax/_grad.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/jax/_math.py` & `netket-3.9/netket/jax/_math.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/jax/_scanmap.py` & `netket-3.9/netket/jax/_scanmap.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/jax/_vjp.py` & `netket-3.9/netket/jax/_vjp.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/jax/_vjp_chunked.py` & `netket-3.9/netket/jax/_vjp_chunked.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/jax/_vmap_chunked.py` & `netket-3.9/netket/jax/_vmap_chunked.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/jax/utils.py` & `netket-3.9/netket/jax/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     """
     if np.issubdtype(typ, np.complexfloating):
         if typ == np.dtype("complex64"):
             return np.dtype("float32")
         elif typ == np.dtype("complex128"):
             return np.dtype("float64")
         else:
-            raise TypeError("Unknown complex floating type {}".format(typ))
+            raise TypeError(f"Unknown complex floating type {typ}")
     else:
         return typ
 
 
 def tree_ishomogeneous(pars: PyTree) -> bool:
     """
     Returns true if all leaves have real dtype or all leaves have complex dtype.
@@ -142,15 +142,15 @@
     if is_complex_dtype(typ):
         return typ
     elif typ == np.dtype("float32"):
         return np.dtype("complex64")
     elif typ == np.dtype("float64"):
         return np.dtype("complex128")
     else:
-        raise TypeError("Unknown complex type for {}".format(typ))
+        raise TypeError(f"Unknown complex type for {typ}")
 
 
 def maybe_promote_to_complex(*types):
     """
     Maybe promotes the first argument to it's complex counterpart given by
     dtype_complex(typ) if any of the arguments is complex
     """
```

### Comparing `netket-3.8/netket/jax/_jacobian/default_mode.py` & `netket-3.9/netket/jax/_jacobian/default_mode.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,21 +11,24 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Callable, Optional
 from functools import partial
 import warnings
-from textwrap import dedent
 
 import jax
 
 import netket.jax as nkjax
 from netket.utils import struct
 from netket.utils.types import PyTree, Array
+from netket.errors import (
+    HolomorphicUndeclaredWarning,
+    IllegalHolomorphicDeclarationForRealParametersError,
+)
 
 
 @struct.dataclass
 class JacobianMode:
     """
     Jax-compatible string type, used to return static information from a jax-jitted
     function.
@@ -73,83 +76,57 @@
     In particular:
      - for functions with a real output, it will return `RealMode`.
      - for functions with a complex output, it will return:
        - If `holomorphic==False` or it not been specified, it will return
        `ComplexMode`, which will force the calculation of both the jacobian
        and adjoint jacobian. See the documentation of{func}`nk.jax.jacobian`
        for more details.
-        - If `holomorphic==True`, it will compute only the complex-valued
-        jacobian, and assumes the adjoint-jacobian to be zero.
+       - If `holomorphic==True`, it will compute only the complex-valued
+       jacobian, and assumes the adjoint-jacobian to be zero.
 
     This function will also raise an error if `holomorphic` is not specified
     but the output is complex.
 
     Args:
         apply_fun: A callable taking as input a pytree of parameters and the samples,
             and returning the output.
         pars: The Pytree of parameters.
         model_state: The optional `model_state`, according to the flax model definition.
         samples: An array of samples.
         holomorphic: A boolean specifying whether `apply_fun` is
             holomorphic or not (`None` by default).
+
     """
-    homogeneous_vars = nkjax.tree_ishomogeneous(pars)
-    leaf_iscomplex = nkjax.tree_leaf_iscomplex(pars)
+    nkjax.tree_ishomogeneous(pars)
+    nkjax.tree_leaf_iscomplex(pars)
+    leaf_isreal = nkjax.tree_leaf_isreal(pars)
 
     if holomorphic is True:
-        if homogeneous_vars and leaf_iscomplex:
-            ## all complex parameters
-            mode = HolomorphicMode
-        elif homogeneous_vars and not leaf_iscomplex:
-            # all real parameters
-            raise ValueError(
-                dedent(
-                    """
-                A function with real parameters cannot be holomorphic.
-
-                Please remove the kw-arg `holomorphic=True`.
-                """
-                )
-            )
+        if leaf_isreal:
+            # all real or mixed real/complex parameters. It's not holomorphic
+            raise IllegalHolomorphicDeclarationForRealParametersError()
         else:
-            # mixed complex and real parameters
-            warnings.warn(
-                dedent(
-                    """The ansatz has non homogeneous variables, which might not behave well with the
-                       holomorhic implementation.
-
-                       Use `holomorphic=False` or mode='complex' for more accurate results but
-                       lower performance.
-                    """
-                )
-            )
+            ## all complex parameters
             mode = HolomorphicMode
     else:
         complex_output = jax.numpy.iscomplexobj(
             jax.eval_shape(
                 apply_fun,
                 {"params": pars, **model_state},
                 samples.reshape(-1, samples.shape[-1]),
             )
         )
 
         if complex_output:
-            if leaf_iscomplex:
+            if not leaf_isreal:
                 if holomorphic is None:
                     warnings.warn(
-                        dedent(
-                            """
-                                Complex-to-Complex model detected. Defaulting to `holomorphic=False` for
-                                the calculation of its jacobian.
-                                If your model is holomorphic, specify `holomorphic=True` to use a more
-                                performant implementation.
-                                To suppress this warning specify `holomorphic`.
-                                """
-                        ),
+                        HolomorphicUndeclaredWarning(),
                         UserWarning,
+                        stacklevel=2,
                     )
                 mode = ComplexMode
             else:
                 mode = ComplexMode
         else:
             mode = RealMode
     return mode
```

### Comparing `netket-3.8/netket/jax/_jacobian/jacobian_dense.py` & `netket-3.9/netket/jax/_jacobian/jacobian_dense.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/jax/_jacobian/jacobian_pytree.py` & `netket-3.9/netket/jax/_jacobian/jacobian_pytree.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/logging/__init__.py` & `netket-3.9/netket/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/logging/json_log.py` & `netket-3.9/netket/logging/json_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         self._autoflush_cost = autoflush_cost
         self._last_flush_time = time.time()
         self._last_flush_runtime = 0.0
 
         self._flush_log_time = 0.0
         self._flush_pars_time = 0.0
 
-    def __call__(self, step, item, variational_state):
+    def __call__(self, step, item, variational_state=None):
         old_step = self._old_step
         super().__call__(step, item, variational_state)
 
         # Check if the time from the last flush is higher than the maximum
         # allowed runtime cost of flushing
         elapsed_time = time.time() - self._last_flush_time
         # On windows, the precision of `time.time` is much lower than that on Linux,
@@ -162,14 +162,16 @@
 
         self._flush_log_time += self._last_flush_runtime
         self._steps_notflushed_write = 0
 
     def _flush_params(self, variational_state):
         if not self._save_params:
             return
+        if variational_state is None:
+            return
 
         _time = time.time()
 
         binary_data = serialization.to_bytes(variational_state.variables)
         with open(self._prefix + ".mpack", "wb") as outfile:
             outfile.write(binary_data)
```

### Comparing `netket-3.8/netket/logging/runtime_log.py` & `netket-3.9/netket/logging/runtime_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     def __init__(self):
         """
         Crates a Runtime Logger.
         """
         self._data = None
         self._old_step = 0
 
-    def __call__(self, step, item, variational_state):
+    def __call__(self, step, item, variational_state=None):
         self._data = accum_histories_in_tree(self._data, item, step=step)
         self._old_step = step
 
     @property
     def data(self):
         """
         The dictionary of logged data.
```

### Comparing `netket-3.8/netket/logging/state_log.py` & `netket-3.9/netket/logging/state_log.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/logging/tensorboard.py` & `netket-3.9/netket/logging/tensorboard.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/models/__init__.py` & `netket-3.9/netket/models/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/models/autoreg.py` & `netket-3.9/netket/models/autoreg.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/models/deepset.py` & `netket-3.9/netket/models/deepset.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/models/equivariant.py` & `netket-3.9/netket/models/equivariant.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,19 +334,17 @@
     `characters` are negative."""
 
     def setup(self):
         # TODO: eventually remove this warning
         # supports a deprecated attribute
         if self.extra_bias:
             warn_deprecation(
-                (
-                    "`extra_bias` is detrimental for performance and is deprecated. "
-                    "Please switch to the default `extra_bias=False`. Previously saved "
-                    "parameters can be migrated using `nk.models.update_GCNN_parity`."
-                )
+                "`extra_bias` is detrimental for performance and is deprecated. "
+                "Please switch to the default `extra_bias=False`. Previously saved "
+                "parameters can be migrated using `nk.models.update_GCNN_parity`."
             )
 
         self.n_symm = np.asarray(self.symmetries).shape[0]
 
         self.dense_symm = DenseSymmFFT(
             space_group=self.symmetries,
             shape=self.shape,
@@ -521,19 +519,17 @@
     `characters` are negative."""
 
     def setup(self):
         # TODO: eventually remove this warning
         # supports a deprecated attribute
         if self.extra_bias:
             warn_deprecation(
-                (
-                    "`extra_bias` is detrimental for performance and is deprecated. "
-                    "Please switch to the default `extra_bias=False`. Previously saved "
-                    "parameters can be migrated using `nk.models.update_GCNN_parity`."
-                )
+                "`extra_bias` is detrimental for performance and is deprecated. "
+                "Please switch to the default `extra_bias=False`. Previously saved "
+                "parameters can be migrated using `nk.models.update_GCNN_parity`."
             )
 
         self.n_symm = np.asarray(self.symmetries).shape[0]
 
         self.dense_symm = DenseSymmMatrix(
             symmetries=self.symmetries,
             features=self.features[0],
```

### Comparing `netket-3.8/netket/models/fast_autoreg.py` & `netket-3.9/netket/models/fast_autoreg.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/models/full_space.py` & `netket-3.9/netket/models/full_space.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/models/gaussian.py` & `netket-3.9/netket/models/gaussian.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/models/jastrow.py` & `netket-3.9/netket/models/jastrow.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/models/mlp.py` & `netket-3.9/netket/models/mlp.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/models/mps.py` & `netket-3.9/netket/models/mps.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/models/ndm.py` & `netket-3.9/netket/models/ndm.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/models/rbm.py` & `netket-3.9/netket/models/rbm.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/models/utils.py` & `netket-3.9/netket/models/utils.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/nn/__init__.py` & `netket-3.9/netket/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/nn/activation.py` & `netket-3.9/netket/nn/activation.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/nn/deprecation.py` & `netket-3.9/netket/nn/deprecation.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/nn/fast_masked_linear.py` & `netket-3.9/netket/nn/fast_masked_linear.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/nn/initializers.py` & `netket-3.9/netket/nn/initializers.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/nn/masked_linear.py` & `netket-3.9/netket/nn/masked_linear.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/nn/symmetric_linear.py` & `netket-3.9/netket/nn/symmetric_linear.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,21 +30,19 @@
 
 # All layers defined here have kernels of shape [out_features, in_features, n_symm]
 default_equivariant_initializer = lecun_normal(in_axis=1, out_axis=0)
 
 
 def symm_input_warning(x_shape, new_x_shape, name):
     warn_deprecation(
-        (
-            f"{len(x_shape)}-dimensional input to {name} layer is deprecated.\n"
-            f"Input shape {x_shape} has been reshaped to {new_x_shape}, where "
-            "the middle dimension encodes different input channels.\n"
-            "Please provide a 3-dimensional input.\nThis warning will become an "
-            "error in the future."
-        )
+        f"{len(x_shape)}-dimensional input to {name} layer is deprecated.\n"
+        f"Input shape {x_shape} has been reshaped to {new_x_shape}, where "
+        "the middle dimension encodes different input channels.\n"
+        "Please provide a 3-dimensional input.\nThis warning will become an "
+        "error in the future."
     )
 
 
 class DenseSymmMatrix(Module):
     r"""Implements a symmetrized linear transformation over a permutation group
     using matrix multiplication."""
 
@@ -809,18 +807,16 @@
     """
     if mask is not None:
         mask = HashableArray(mask)
 
     # deprecate in_features
     if in_features is not None:
         warn_deprecation(
-            (
-                "`in_features` is now automatically detected from the input and deprecated."
-                "Please remove it when calling `DenseEquivariant`."
-            )
+            "`in_features` is now automatically detected from the input and deprecated."
+            "Please remove it when calling `DenseEquivariant`."
         )
     if "out_features" in kwargs:
         warn_deprecation(
             "`out_features` has been renamed to `features` and the old name is "
             "now deprecated. Please update your code."
         )
         if features is not None:
```

### Comparing `netket-3.8/netket/nn/utils.py` & `netket-3.9/netket/nn/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import operator
 
 import jax
 from jax import numpy as jnp
 import numpy as np
 
 from netket import jax as nkjax
-from netket.utils import get_afun_if_module, mpi, module_version
+from netket.utils import get_afun_if_module, mpi
 from netket.utils.types import Array, PyTree
 from netket.hilbert import DiscreteHilbert
 
 from flax.traverse_util import flatten_dict, unflatten_dict
 from flax.core import unfreeze
 
 
@@ -166,15 +166,15 @@
         trace = jnp.trace(rho)
         rho /= trace
 
     return rho
 
 
 # TODO: Deprecate: remove
-def update_dense_symm(params, names=["dense_symm", "Dense"]):
+def update_dense_symm(params, names=("dense_symm", "Dense")):
     """Updates DenseSymm kernels in pre-PR#1030 parameter pytrees to the new
     3D convention.
 
     Args:
         params: a parameter pytree
         names: layer names search for, default: those used in RBMSymm and GCNN*
     """
@@ -214,15 +214,15 @@
 ) -> Tuple[Tuple[int, ...], Tuple[int, ...]]:
     binary_indices = tuple([i for i in range(len(shape)) if shape[i] == 2])
     non_binary_indices = tuple([i for i in range(len(shape)) if shape[i] != 2])
     return binary_indices, non_binary_indices
 
 
 def _prod(iterable):
-    # This is a workaround for math.prod which is not defined for Python 3.7
+    # This is a workaround for math.prod which is not defined for Python 3.8
     return reduce(operator.mul, iterable, 1)
 
 
 @partial(jax.jit, static_argnames=("hilbert", "max_bits"))
 def binary_encoding(
     hilbert: DiscreteHilbert,
     x: Array,
@@ -276,21 +276,14 @@
     Args:
         hilbert: The Hilbert space
         σ: A single or a batch of configurations
 
     Returns:
         a single integer or a batch of integer indices.
     """
-    if module_version("jax") < (0, 3, 17):
-        raise RuntimeError(
-            "The jitted conversion of bit-strings to hilbert numbers"
-            "is only supported with jax.__version__ >= 0.3.17, but you "
-            f"have {module_version('jax')}"
-        )
-
     if not hilbert.is_indexable:
         raise ValueError(
             f"Hilbert space {hilbert} is too large to be indexed or "
             f"cannot be indexed at all."
         )
 
     # calls back into python
```

### Comparing `netket-3.8/netket/nn/blocks/__init__.py` & `netket-3.9/netket/nn/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/nn/blocks/deepset.py` & `netket-3.9/netket/nn/blocks/deepset.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,23 +27,22 @@
         feat, out = None, features[0]
     else:
         feat, out = tuple(features[:-1]), features[-1]
     return feat, out
 
 
 class DeepSetMLP(nn.Module):
-    r"""Implements the DeepSets architecture, which is permutation invariant.
+    r"""Implements the DeepSets architecture, which is permutation invariant
+    and is suitable for the encoding of bosonic systems.
 
-    .. math ::
+    .. math::
 
         f(x_1,...,x_N) = \rho\left(\sum_i \phi(x_i)\right)
 
-    that is suitable for the simulation of bosonic.
-
-    The input shape must have an axis that is reshaped to (..., N, D), where we pool over N.
+    The input shape must have an axis that is reshaped to `(..., N, D)`, where we pool over N.
 
     """
 
     features_phi: Optional[Union[int, Tuple[int, ...]]] = None
     """
     Number of features in each layer for phi network.
     When features_phi is None, no phi network is created.
@@ -70,15 +69,15 @@
     """if True uses a bias in all layers."""
 
     kernel_init: NNInitFunc = lecun_normal()
     """Initializer for the Dense layer matrix"""
     bias_init: NNInitFunc = zeros
     """Initializer for the hidden bias"""
     precision: Optional[jax.lax.Precision] = None
-    """numerical precision of the computation see `jax.lax.Precision`for details."""
+    """numerical precision of the computation see {ref}`jax.lax.Precision`for details."""
 
     def setup(self):
         def _create_mlp(features, output_activation, name):
             hidden_dims, out_dim = _process_features(features)
             if out_dim is None:
                 return None
             else:
```

### Comparing `netket-3.8/netket/nn/blocks/mlp.py` & `netket-3.9/netket/nn/blocks/mlp.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/nn/blocks/symmetry_sum.py` & `netket-3.9/netket/nn/blocks/symmetry_sum.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,22 +23,22 @@
 from netket.utils.group import PermutationGroup
 from netket.utils.types import Array
 
 
 class SymmExpSum(nn.Module):
     r"""
     A flax module symmetrizing the log-wavefunction :math:`\log\psi_\theta(\sigma)` encoded
-    into another flax module (:ref:`flax.linen.Module`) by summing over all possible symmetries
+    into another flax module (:class:`flax.linen.Module`) by summing over all possible symmetries
     :math:`g` in a certain discrete permutation group :math:`G`.
 
     .. math::
 
         \log\psi_\theta(\sigma) = \log\sum_{g\in G}\chi_g\exp[\log\psi_\theta(T_{g}\sigma)]
 
-    For the ground-state, it is usually found that :math:`\chi_g=1: :math:\forall g\in G`.
+    For the ground-state, it is usually found that :math:`\chi_g=1 \forall g\in G`.
 
     To construct this network, one has to specify the module, the symmetry group and (optionally)
     the id of the character to consider. The symmetry
 
     The module's :code:`.__call__` will be called.
     The :code:`symm_group` attribute
 
@@ -73,15 +73,15 @@
     module: nn.Module
     """The neural network architecture encoding the log-wavefunction
     to symmetrize in the :code:`.__call__` function."""
 
     symm_group: PermutationGroup
     """The symmetry group to use. It should be a valid :ref:`netket.utils.group.PermutationGroup`
     object. Can be easily extracted from a :ref:`netket.graph.Graph` object by calling
-    :ref:`~netket.graph.Graph.point_group` or :ref:`~netket.graph.Graph.translation_group`
+    :meth:`~netket.graph.Graph.point_group` or :meth:`~netket.graph.Graph.translation_group`
 
     .. code::
 
         graph = nk.graph.Square(3)
         symm_group = graph.point_group()
 
     """
```

### Comparing `netket-3.8/netket/operator/__init__.py` & `netket-3.9/netket/operator/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from ._abstract_operator import AbstractOperator
 
 from ._discrete_operator import DiscreteOperator
+from ._discrete_operator_jax import DiscreteJaxOperator
+
+from ._pauli_strings import PauliStrings, PauliStringsJax
 from ._local_operator import LocalOperator
 from ._graph_operator import GraphOperator
-from ._pauli_strings import PauliStrings
 from ._lazy import Adjoint, Transpose, Squared
 from ._heisenberg import Heisenberg
-from ._ising import Ising
+from ._ising import Ising, IsingJax
 from ._bose_hubbard import BoseHubbard
 
 from ._abstract_super_operator import AbstractSuperOperator
 from ._local_liouvillian import LocalLiouvillian
 
 from ._continuous_operator import ContinuousOperator
 from ._kinetic import KineticEnergy
```

### Comparing `netket-3.8/netket/operator/_abstract_operator.py` & `netket-3.9/netket/operator/_abstract_operator.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/operator/_abstract_super_operator.py` & `netket-3.9/netket/operator/_abstract_super_operator.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/operator/_bose_hubbard.py` & `netket-3.9/netket/operator/_bose_hubbard.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import jax.numpy as jnp
 import math
 
 from netket.graph import AbstractGraph, Graph
 from netket.hilbert import Fock
 from netket.utils.types import DType
 from netket.utils.numbers import dtype as _dtype
+from netket.errors import concrete_or_error, NumbaOperatorGetConnDuringTracingError
 
 from . import boson
 from ._local_operator import LocalOperator
 from ._hamiltonian import SpecialHamiltonian
 
 
 class BoseHubbard(SpecialHamiltonian):
@@ -306,16 +307,23 @@
         total_size = x.shape[0] * self._max_conn
         if self._max_mels.size < total_size:
             self._max_mels = np.empty(total_size, dtype=self._max_mels.dtype)
             self._max_xprime = np.empty((total_size, x.shape[1]), dtype=x.dtype)
         elif x.dtype != self._max_xprime.dtype:
             self._max_xprime = self._max_xprime.astype(x.dtype)
 
+        x = concrete_or_error(
+            np.asarray,
+            x,
+            NumbaOperatorGetConnDuringTracingError,
+            self,
+        )
+
         return self._flattened_kernel(
-            np.asarray(x),
+            x,
             sections,
             self._edges,
             self._U,
             self._V,
             self._J,
             self._mu,
             self._n_max,
```

### Comparing `netket-3.8/netket/operator/_continuous_operator.py` & `netket-3.9/netket/operator/_continuous_operator.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/operator/_discrete_operator.py` & `netket-3.9/netket/operator/_discrete_operator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,21 @@
-import abc
+# Copyright 2021-2023 The NetKet Authors - All rights reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from typing import Tuple
 import numpy as np
 import jax.numpy as jnp
 
 from numba import jit
 from scipy.sparse import csr_matrix as _csr_matrix
 
@@ -60,15 +73,14 @@
         n_primes = sections[0]
 
         x_primes_r = x_primes.reshape(*x.shape[:-1], n_primes, n_visible)
         mels_r = mels.reshape(*x.shape[:-1], n_primes)
 
         return x_primes_r, mels_r
 
-    @abc.abstractmethod
     def get_conn_flattened(
         self, x: np.ndarray, sections: np.ndarray
     ) -> Tuple[np.ndarray, np.ndarray]:
         r"""Finds the connected elements of the Operator.
 
         Starting from a given quantum number :math:`x`, it finds all
         other quantum numbers  :math:`x'` such that the matrix element
@@ -89,14 +101,27 @@
         Returns:
             (matrix, array): The connected states x', flattened together in
                 a single matrix.
                 An array containing the matrix elements :math:`O(x,x')`
                 associated to each x'.
 
         """
+        raise NotImplementedError(
+            f"""
+            The method get_conn_flattened has not been implemented for the object of
+            type {type(self)}.
+
+            This may happen if you defined a custom class inheriting from DiscreteOperator
+            and you have not implemented this method. In that case, you should define
+            `get_conn_flattened(self, x: array, sections: array)` according to the
+            docstring provided on the documentation.
+
+            Otherwise, please open an issue on netket's github repository.
+            """
+        )
 
     def get_conn(self, x: np.ndarray):
         r"""Finds the connected elements of the Operator. Starting
         from a given quantum number x, it finds all other quantum numbers x' such
         that the matrix element :math:`O(x,x')` is different from zero. In general there
         will be several different connected states x' satisfying this
         condition, and they are denoted here :math:`x'(k)`, for :math:`k=0,1...N_{\mathrm{connected}}`.
@@ -113,15 +138,16 @@
         """
         if x.ndim != 1:
             raise ValueError(
                 "get_conn does not support batches. Please use get_conn_flattened instead."
             )
         if x.shape[0] != self.hilbert.size:
             raise ValueError(
-                "The given quantum numbers do not match the hilbert space."
+                "The given quantum numbers do not match the hilbert space because"
+                f"it has shape {x.shape} of which[0] but expected {self.hilbert.size}."
             )
 
         return self.get_conn_flattened(
             x.reshape((1, -1)),
             np.ones(1),
         )
 
@@ -134,15 +160,15 @@
             out (array): If None an output array is allocated.
 
         Returns:
             array: The number of connected states x' for each x[i].
 
         """
         if out is None:
-            out = np.empty(x.shape[0], dtype=np.intc)
+            out = np.empty(x.shape[0], dtype=np.int32)
         self.get_conn_flattened(x, out)
         out = self._n_conn_from_sections(out)
 
         return out
 
     @staticmethod
     @jit(nopython=True)
@@ -219,15 +245,15 @@
         )
 
     def __call__(self, v: np.ndarray) -> np.ndarray:
         return self.apply(v)
 
     def apply(self, v: np.ndarray) -> np.ndarray:
         op = self.to_linear_operator()
-        return op.dot(v)
+        return op @ v
 
     def __matmul__(self, other):
         if isinstance(other, np.ndarray) or isinstance(other, jnp.ndarray):
             return self.apply(other)
         elif isinstance(other, AbstractOperator):
             return self._op__matmul__(other)
         else:
```

### Comparing `netket-3.8/netket/operator/_graph_operator.py` & `netket-3.9/netket/operator/_graph_operator.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/operator/_hamiltonian.py` & `netket-3.9/netket/operator/_hamiltonian.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from ._discrete_operator import DiscreteOperator
 
 
 class SpecialHamiltonian(DiscreteOperator):
     def to_local_operator(self):
         raise NotImplementedError(
-            "Must implemented to_local_operator for {}".format(type(self))
+            f"Must implemented to_local_operator for {type(self)}"
         )
 
     def conjugate(self, *, concrete: bool = True):
         return self.to_local_operator().conjugate(concrete=concrete)
 
     def __add__(self, other):
         if type(self) is type(other):
```

### Comparing `netket-3.8/netket/operator/_heisenberg.py` & `netket-3.9/netket/operator/_heisenberg.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/operator/_ising.py` & `netket-3.9/netket/operator/_ising/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,44 +8,44 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Optional
-from numba import jit
+from typing import Optional, Union
 
 import numpy as np
-import jax.numpy as jnp
 
-from netket.graph import AbstractGraph, Graph
+from jax import numpy as jnp
+
+from netket.graph import AbstractGraph
 from netket.hilbert import AbstractHilbert
 from netket.utils.numbers import dtype as _dtype
-from netket.utils.types import DType
+from netket.utils.types import Array, DType
 
-from . import spin
-from ._local_operator import LocalOperator
-from ._hamiltonian import SpecialHamiltonian
+from .. import spin
+from .._hamiltonian import SpecialHamiltonian
+from .._local_operator import LocalOperator
 
 
-class Ising(SpecialHamiltonian):
+class IsingBase(SpecialHamiltonian):
     r"""
     The Transverse-Field Ising Hamiltonian :math:`-h\sum_i \sigma_i^{(x)} +J\sum_{\langle i,j\rangle} \sigma_i^{(z)}\sigma_j^{(z)}`.
 
     This implementation is considerably faster than the Ising hamiltonian constructed by summing :class:`~netket.operator.LocalOperator` s.
     """
 
     def __init__(
         self,
         hilbert: AbstractHilbert,
-        graph: AbstractGraph,
+        graph: Union[AbstractGraph, Array],
         h: float,
-        J: float = 1.0,
-        dtype: Optional[DType] = None,
+        J: float,
+        dtype: DType,
     ):
         r"""
         Constructs the Ising Operator from an hilbert space and a
         graph specifying the connectivity.
 
         Args:
             hilbert: Hilbert space the operator acts on.
@@ -59,110 +59,129 @@
             >>> import netket as nk
             >>> g = nk.graph.Hypercube(length=20, n_dim=1, pbc=True)
             >>> hi = nk.hilbert.Spin(s=0.5, N=g.n_nodes)
             >>> op = nk.operator.Ising(h=1.321, hilbert=hi, J=0.5, graph=g)
             >>> print(op)
             Ising(J=0.5, h=1.321; dim=20)
         """
-        assert (
-            graph.n_nodes == hilbert.size
-        ), "The size of the graph must match the hilbert space"
-
         super().__init__(hilbert)
 
         if dtype is None:
             dtype = jnp.promote_types(_dtype(h), _dtype(J))
-        dtype = np.empty((), dtype=dtype).dtype
-        self._dtype = dtype
 
-        self._h = np.array(h, dtype=dtype)
-        self._J = np.array(J, dtype=dtype)
-        self._edges = np.asarray(
-            [[u, v] for u, v in graph.edges()],
-            dtype=np.intp,
-        )
+        if isinstance(graph, AbstractGraph):
+            if graph.n_nodes != hilbert.size:
+                raise ValueError(
+                    """
+                    The size of the graph must match the hilbert space.
+                    """
+                )
+            # support also a matrix input in here.
+            graph = graph.edges()
+
+        if isinstance(graph, list):
+            graph = np.asarray(
+                [[u, v] for u, v in graph],
+                dtype=np.intp,
+            )
+
+        if graph.ndim != 2 or graph.shape[1] != 2:
+            raise ValueError(
+                """
+                Graph should be one of:
+                    - NetKet graph type (nk.operator.AbstractGraph)
+                    - List of tuples, describing the edges
+                    - a (N,2) array of integers.
+                """
+            )
+
+        # Fallback to float32 when float64 is disabled in JAX
+        dtype = jnp.empty((), dtype=dtype).dtype
+
+        self._h = h.astype(dtype=dtype)
+        self._J = J.astype(dtype=dtype)
+        self._edges = graph.astype(np.intp)
 
     @property
     def h(self) -> float:
         """The magnitude of the transverse field"""
         return self._h
 
     @property
     def J(self) -> float:
         """The magnitude of the hopping"""
         return self._J
 
     @property
     def edges(self) -> np.ndarray:
+        """The (N_conns, 2) matrix of edges on which the interaction term
+        is non-zero.
+        """
         return self._edges
 
     @property
     def is_hermitian(self) -> bool:
+        """A boolean stating whether this hamiltonian is hermitian."""
         return True
 
     @property
     def dtype(self) -> DType:
-        return self._dtype
+        """The dtype of the matrix elements."""
+        return jnp.promote_types(_dtype(self.h), _dtype(self.J))
 
     def conjugate(self, *, concrete=True):
         # if real
         if isinstance(self.h, float) and isinstance(self.J, float):
             return self
         else:
             raise NotImplementedError
 
-    @staticmethod
-    @jit(nopython=True)
-    def n_conn(x, out):  # pragma: no cover
+    def n_conn(self, x, out=None):  # pragma: no cover
         r"""Return the number of states connected to x.
 
         Args:
             x (matrix): A matrix of shape (batch_size,hilbert.size) containing
                         the batch of quantum numbers x.
             out (array): If None an output array is allocated.
 
         Returns:
             array: The number of connected states x' for each x[i].
 
         """
         if out is None:
-            out = np.empty(
-                x.shape[0],
-                dtype=np.int32,
-            )
-
-        out.fill(x.shape[1] + 1)
-
+            out = np.empty(x.shape[0], dtype=np.int32)
+        out.fill((self.h != 0) * x.shape[1] + 1)
         return out
 
     @property
     def max_conn_size(self) -> int:
         """The maximum number of non zero ⟨x|O|x'⟩ for every x."""
         return self.hilbert.size + 1
 
     def copy(self, *, dtype: Optional[DType] = None):
         if dtype is None:
             dtype = self.dtype
 
-        graph = Graph(edges=[list(edge) for edge in self.edges])
-        return Ising(hilbert=self.hilbert, graph=graph, J=self.J, h=self.h, dtype=dtype)
+        return type(self)(
+            hilbert=self.hilbert, graph=self.edges, J=self.J, h=self.h, dtype=dtype
+        )
 
     def to_local_operator(self):
         # The hamiltonian
         ha = LocalOperator(self.hilbert, dtype=self.dtype)
 
         if self.h != 0:
             for i in range(self.hilbert.size):
-                ha -= self.h * spin.sigmax(self.hilbert, i, dtype=self.dtype)
+                ha -= self.h * spin.sigmax(self.hilbert, int(i), dtype=self.dtype)
 
         if self.J != 0:
             for (i, j) in self.edges:
                 ha += self.J * (
-                    spin.sigmaz(self.hilbert, i, dtype=self.dtype)
-                    * spin.sigmaz(self.hilbert, j, dtype=self.dtype)
+                    spin.sigmaz(self.hilbert, int(i), dtype=self.dtype)
+                    * spin.sigmaz(self.hilbert, int(j), dtype=self.dtype)
                 )
 
         return ha
 
     def _iadd_same_hamiltonian(self, other):
         if self.hilbert != other.hilbert:
             raise NotImplementedError(
@@ -177,85 +196,11 @@
             raise NotImplementedError(
                 "Cannot add hamiltonians on different hilbert spaces"
             )
 
         self._h -= other.h
         self._J -= other.J
 
-    @staticmethod
-    @jit(nopython=True)
-    def _flattened_kernel(x, sections, edges, h, J):  # pragma: no cover
-        n_sites = x.shape[1]
-        n_conn = n_sites + 1
-
-        x_prime = np.empty(
-            (
-                x.shape[0] * n_conn,
-                n_sites,
-            ),
-            dtype=x.dtype,
-        )
-        mels = np.empty(x.shape[0] * n_conn, dtype=h.dtype)
-
-        diag_ind = 0
-
-        for i in range(x.shape[0]):
-            mels[diag_ind] = 0.0
-            for k in range(edges.shape[0]):
-                mels[diag_ind] += J * x[i, edges[k, 0]] * x[i, edges[k, 1]]
-
-            odiag_ind = 1 + diag_ind
-
-            mels[odiag_ind : (odiag_ind + n_sites)].fill(-h)
-
-            x_prime[diag_ind : (diag_ind + n_conn)] = np.copy(x[i])
-
-            for j in range(n_sites):
-                x_prime[j + odiag_ind][j] *= -1.0
-
-            diag_ind += n_conn
-
-            sections[i] = diag_ind
-
-        return x_prime, mels
-
-    def get_conn_flattened(self, x, sections, pad=False):
-        r"""Finds the connected elements of the Operator. Starting
-        from a given quantum number x, it finds all other quantum numbers x' such
-        that the matrix element :math:`O(x,x')` is different from zero. In general there
-        will be several different connected states x' satisfying this
-        condition, and they are denoted here :math:`x'(k)`, for
-        :math:`k=0,1...N_{\mathrm{connected}}`.
-
-        This is a batched version, where x is a matrix of shape (batch_size,hilbert.size).
-
-        Args:
-            x (matrix): A matrix of shape (batch_size,hilbert.size) containing
-                        the batch of quantum numbers x.
-            sections (array): An array of size (batch_size) useful to unflatten
-                        the output of this function.
-                        See numpy.split for the meaning of sections.
-            pad (bool): no effect here
-
-        Returns:
-            matrix: The connected states x', flattened together in a single matrix.
-            array: An array containing the matrix elements :math:`O(x,x')` associated to each x'.
-
-        """
-
-        return self._flattened_kernel(
-            np.asarray(x), sections, self._edges, self._h, self._J
-        )
-
-    def _get_conn_flattened_closure(self):
-        _edges = self._edges
-        _h = self._h
-        _J = self._J
-        fun = self._flattened_kernel
-
-        def gccf_fun(x, sections):  # pragma: no cover
-            return fun(x, sections, _edges, _h, _J)
-
-        return jit(nopython=True)(gccf_fun)
-
     def __repr__(self):
-        return f"Ising(J={self._J}, h={self._h}; dim={self.hilbert.size})"
+        return (
+            f"{type(self).__name__}(J={self._J}, h={self._h}; dim={self.hilbert.size})"
+        )
```

### Comparing `netket-3.8/netket/operator/_kinetic.py` & `netket-3.9/netket/operator/_kinetic.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/operator/_lazy.py` & `netket-3.9/netket/operator/_lazy.py`

 * *Files 6% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         return self.parent.transpose(concrete=concrete)
 
     @property
     def H(self):
         return self.parent
 
     def __repr__(self):
-        return "Adjoint({})".format(self.parent)
+        return f"Adjoint({self.parent})"
 
     def __mul__(self, other):
         if self.parent == other:
             return Squared(other)
 
         return self.collect() * other
 
@@ -224,15 +224,15 @@
         return self
 
     @property
     def is_hermitian(self) -> bool:
         return True
 
     def __repr__(self):
-        return "Squared({})".format(self.parent)
+        return f"Squared({self.parent})"
 
     def __mul__(self, other):
         return self.collect() * other
 
     def __rmul__(self, other):
         return other * self.collect()
```

### Comparing `netket-3.8/netket/operator/_local_liouvillian.py` & `netket-3.9/netket/operator/_local_liouvillian.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/operator/_local_operator.py` & `netket-3.9/netket/operator/_local_operator/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,25 +20,27 @@
 
 import numpy as np
 import numba
 from scipy.sparse import issparse
 
 from netket.hilbert import AbstractHilbert
 from netket.utils.types import DType, Array
-from netket.utils.numbers import dtype as _dtype
+from netket.utils.numbers import dtype as _dtype, is_scalar
+from netket.errors import concrete_or_error, NumbaOperatorGetConnDuringTracingError
 
-from ._discrete_operator import DiscreteOperator
-from ._lazy import Transpose
+from .._discrete_operator import DiscreteOperator
+from .._lazy import Transpose
 
-from ._local_operator_helpers import (
+from .helpers import (
     canonicalize_input,
     _multiply_operators,
     cast_operator_matrix_dtype,
 )
-from ._local_operator_compile_helpers import pack_internals
+from .compile_helpers import pack_internals
+from .convert import local_operators_to_pauli_strings
 
 
 def is_hermitian(a: np.ndarray, rtol=1e-05, atol=1e-08) -> bool:
     if issparse(a):
         return np.allclose(a.todense(), a.T.conj().todense(), rtol=rtol, atol=atol)
     else:
         return np.allclose(a, a.T.conj(), rtol=rtol, atol=atol)
@@ -189,14 +191,20 @@
         self._mel_cutoff = mel_cutoff
         assert self.mel_cutoff >= 0
 
     @property
     def constant(self) -> numbers.Number:
         return self._constant
 
+    def to_pauli_strings(self) -> "PauliStrings":  # noqa: F821
+        """Convert to PauliStrings object"""
+        return local_operators_to_pauli_strings(
+            self.hilbert, self.operators, self.acting_on, self.constant, self.dtype
+        )
+
     def copy(self, *, dtype: Optional[DType] = None):
         """Returns a copy of the operator, while optionally changing the dtype
         of the operator.
 
         Args:
             dtype: optional dtype
         """
@@ -271,56 +279,57 @@
             assert other.mel_cutoff == self.mel_cutoff
             self._constant += other.constant.item()
             for (aon, op) in other._operators_dict.items():
                 self._add_operator(aon, op)
 
             self._reset_caches()
             return self
-        if isinstance(other, numbers.Number):
+        if is_scalar(other):
             if not np.can_cast(type(other), self.dtype, casting="same_kind"):
                 raise ValueError(
                     f"Cannot add inplace operator with dtype {type(other)} "
                     f"to operator with dtype {self.dtype}"
                 )
 
             self._reset_caches()
             self._constant += other
             return self
 
         return NotImplemented
 
     def __truediv__(self, other):
-        if not isinstance(other, numbers.Number):
+        if not is_scalar(other):
             raise TypeError("Only division by a scalar number is supported.")
 
         if other == 0:
             raise ValueError("Dividing by 0")
         return self.__mul__(1.0 / other)
 
     def __rmul__(self, other):
         return self.__mul__(other)
 
     def __mul__(self, other):
         if isinstance(other, DiscreteOperator):
             op = self.copy(dtype=np.promote_types(self.dtype, _dtype(other)))
             return op.__imatmul__(other)
-        elif isinstance(other, numbers.Number):
+        elif is_scalar(other):
             op = self.copy(dtype=np.promote_types(self.dtype, _dtype(other)))
             return op.__imul__(other)
         return NotImplemented
 
     def __imul__(self, other):
         if isinstance(other, DiscreteOperator):
             return self.__imatmul__(other)
-        elif isinstance(other, numbers.Number):
-            if not np.can_cast(type(other), self.dtype, casting="same_kind"):
+        elif is_scalar(other):
+            if not np.can_cast(_dtype(other), self.dtype, casting="same_kind"):
                 raise ValueError(
-                    f"Cannot add inplace operator with dtype {type(other)} "
-                    f"to operator with dtype {self.dtype}"
+                    f"Cannot add inplace operator of type {type(other)} and "
+                    f"dtype {_dtype(other)} to operator with dtype {self.dtype}"
                 )
+            other = np.asarray(other, dtype=np.promote_types(self.dtype, _dtype(other)))
 
             self._constant *= other
             if np.abs(other) <= self.mel_cutoff:
                 self._operators_dict = {}
             else:
                 for key in self._operators_dict:
                     self._operators_dict[key] = other * self._operators_dict[key]
@@ -444,16 +453,23 @@
         Returns:
             matrix: The connected states x', flattened together in a single matrix.
             array: An array containing the matrix elements :math:`O(x,x')` associated to each x'.
 
         """
         self._setup()
 
+        x = concrete_or_error(
+            np.asarray,
+            x,
+            NumbaOperatorGetConnDuringTracingError,
+            self,
+        )
+
         return self._get_conn_flattened_kernel(
-            np.asarray(x),
+            x,
             sections,
             self._local_states,
             self._basis,
             self._constant,
             self._diag_mels,
             self._n_conns,
             self._mels,
@@ -624,14 +640,22 @@
 
         Returns:
             matrix: The connected states x', flattened together in a single matrix.
             array: An array containing the matrix elements :math:`O(x,x')` associated to each x'.
 
         """
         self._setup()
+
+        x = concrete_or_error(
+            np.asarray,
+            x,
+            NumbaOperatorGetConnDuringTracingError,
+            self,
+        )
+
         return self._get_conn_filtered_kernel(
             x,
             sections,
             self._local_states,
             self._basis,
             self._constant,
             self._diag_mels,
```

### Comparing `netket-3.8/netket/operator/_local_operator_compile_helpers.py` & `netket-3.9/netket/operator/_local_operator/compile_helpers.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/operator/_local_operator_helpers.py` & `netket-3.9/netket/operator/_local_operator/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The NetKet Authors - All rights reserved.
+# Copyright 2022-23 The NetKet Authors - All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,14 +14,15 @@
 
 from typing import Tuple
 
 import functools
 import numbers
 
 import numpy as np
+from jax import numpy as jnp
 
 from scipy import sparse
 from scipy.sparse import spmatrix
 
 from netket.hilbert import AbstractHilbert, Fock
 from netket.utils.types import DType, Array
 from netket.utils.numbers import dtype as _dtype
@@ -113,15 +114,16 @@
 
     # If we asked for a specific dtype, enforce it.
     if dtype is None:
         dtype = np.promote_types(np.float32, _dtype(constant))
         dtype = functools.reduce(
             lambda dt, op: np.promote_types(dt, op.dtype), operators, dtype
         )
-    dtype = np.empty((), dtype=dtype).dtype
+    # Fallback to float32 when float64 is disabled in JAX
+    dtype = jnp.empty((), dtype=dtype).dtype
 
     canonicalized_operators = []
     canonicalized_acting_on = []
     for (operator, acting_on) in zip(operators, acting_on):
         check_valid_opmatrix(hilbert, operator, acting_on)
 
         if operator.dtype is not dtype:
```

### Comparing `netket-3.8/netket/operator/_pauli_strings.py` & `netket-3.9/netket/operator/_pauli_strings/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,41 +9,116 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import re
-from typing import List, Union
-from netket.utils.types import DType
+from typing import Iterable, List, Union, Optional
+from netket.utils.types import DType, Array
 
 import numpy as np
 from numba import jit
 from itertools import product
 
 from netket.hilbert import Qubit, AbstractHilbert
 from netket.utils.numbers import is_scalar
 
-from ._abstract_operator import AbstractOperator
-from ._discrete_operator import DiscreteOperator
+from .._abstract_operator import AbstractOperator
+from .._discrete_operator import DiscreteOperator
 
 valid_pauli_regex = re.compile(r"^[XYZI]+$")
 
 
-class PauliStrings(DiscreteOperator):
+def _standardize_matrix_input_type(op):
+    """
+    Standardize the structural type of operators stored in LocalOperator.
+
+    Eventually, we could also support spmatrices (but some work will be needed.)
+    """
+    if isinstance(op, list):
+        return np.asarray(op)
+    else:
+        return op
+
+
+def cast_operator_matrix_dtype(matrix: Array, dtype: DType):
+    """
+    Changes the dtype of a matrix, without changing the structural type of the object.
+
+    This makes sure that if you pass sparse arrays to a LocalOperator, they remain
+    sparse even if you change the dtype
+    """
+    # must copy
+    # return np.asarray(matrix, dtype=dtype)
+    return matrix.astype(dtype)
+
+
+def canonicalize_input(hilbert: AbstractHilbert, operators, weights, *, dtype=None):
+    if operators is None:
+        raise ValueError(
+            "None valued operators passed. (Might arise when passing None valued hilbert explicitly)"
+        )
+
+    # Support single-operator
+    if isinstance(operators, str):
+        operators = [operators]
+
+    if len(operators) == 0:
+        raise ValueError("No Pauli operators passed.")
+
+    # default weight is 1
+    if weights is None:
+        weights = True
+
+    if is_scalar(weights):
+        weights = [weights for _ in operators]
+
+    if len(weights) != len(operators):
+        raise ValueError("weights should have the same length as operators.")
+
+    _hilb_size = len(operators[0])
+    consistent = all(len(op) == _hilb_size for op in operators)
+    if not consistent:
+        raise ValueError("Pauli strings have inhomogeneous lengths.")
+
+    consistent = all(bool(valid_pauli_regex.search(op)) for op in operators)
+    if not consistent:
+        raise ValueError(
+            """Operators in string must be one of
+            the Pauli operators X,Y,Z, or the identity I"""
+        )
+
+    if hilbert is None:
+        hilbert = Qubit(_hilb_size)
+
+    if not np.allclose(hilbert.shape, 2):
+        raise ValueError(
+            "PauliStrings only work for local hilbert size 2 where PauliMatrices are defined"
+        )
+
+    weights = _standardize_matrix_input_type(weights)
+    weights = cast_operator_matrix_dtype(weights, dtype=dtype)
+
+    operators = np.asarray(operators, dtype=str)
+
+    return hilbert, operators, weights, weights.dtype
+
+
+class PauliStringsBase(DiscreteOperator):
     """A Hamiltonian consisting of the sum of products of Pauli operators."""
 
     def __init__(
         self,
         hilbert: AbstractHilbert,
         operators: Union[str, List[str]] = None,
         weights: Union[float, complex, List[Union[float, complex]]] = None,
         *,
         cutoff: float = 1.0e-10,
-        dtype: DType = complex,
+        dtype: Optional[DType] = None,
     ):
         """
         Constructs a new ``PauliStrings`` operator given a set of Pauli operators.
         This class has two possible forms for initialization: ``PauliStrings(hilbert, operators, ...)`` or  ``PauliStrings(operators, ...)``.
         When no hilbert argument is passed, the hilbert defaults to Qubit, where the number of qubits is automatically deduced from the operators.
 
         Args:
@@ -66,180 +141,56 @@
            >>> op = nk.operator.PauliStrings(hilbert, operators, weights)
            >>> op.hilbert
            Spin(s=1/2, N=2)
         """
         if hilbert is None:
             raise ValueError("None-valued hilbert passed.")
 
+        # if first argument is not Hilbert, then shift all arguments by one
+        # to support not declaring the Hilbert space
         if not isinstance(hilbert, AbstractHilbert):
-            # if first argument is not Hilbert, then shift all arguments by one
             hilbert, operators, weights = None, hilbert, operators
 
-        if operators is None:
-            raise ValueError(
-                "None valued operators passed. (Might arise when passing None valued hilbert explicitly)"
-            )
-
-        # Support single-operator
-        if isinstance(operators, str):
-            operators = [operators]
-
-        if len(operators) == 0:
-            raise ValueError("No Pauli operators passed.")
-
-        # default weight is 1
-        if weights is None:
-            weights = True
-
-        if is_scalar(weights):
-            weights = [weights for _ in operators]
-
-        if len(weights) != len(operators):
-            raise ValueError("weights should have the same length as operators.")
+        hilbert, operators, weights, dtype = canonicalize_input(
+            hilbert, operators, weights, dtype=dtype
+        )
 
         if not np.isscalar(cutoff) or cutoff < 0:
             raise ValueError("invalid cutoff in PauliStrings.")
 
-        _hilb_size = len(operators[0])
-        consistent = all(len(op) == _hilb_size for op in operators)
-        if not consistent:
-            raise ValueError("Pauli strings have inhomogeneous lengths.")
-
-        consistent = all(bool(valid_pauli_regex.search(op)) for op in operators)
-        if not consistent:
-            raise ValueError(
-                """Operators in string must be one of
-                the Pauli operators X,Y,Z, or the identity I"""
-            )
-
-        if hilbert is None:
-            hilbert = Qubit(_hilb_size)
-
-        if not np.allclose(hilbert.shape, 2):
-            raise ValueError(
-                "PauliStrings only work for local hilbert size 2 where PauliMatrices are defined"
-            )
         super().__init__(hilbert)
 
-        self._cutoff = cutoff
-        b_weights = np.asarray(weights, dtype=dtype)
-        self._is_hermitian = np.allclose(b_weights.imag, 0.0)
-
-        self._orig_operators = np.array(operators, dtype=str)
-        self._orig_weights = np.array(weights, dtype=dtype)
+        self._operators = operators
+        self._weights = weights
         self._dtype = dtype
 
-        self._initialized = False
+        self._cutoff = cutoff
 
-    @staticmethod
-    def identity(hilbert: AbstractHilbert, **kwargs):
-        return PauliStrings(hilbert, "I" * hilbert.size, **kwargs)
-
-    def _setup(self, force=False):
-        """Analyze the operator strings and precompute arrays for get_conn inference"""
-        if force or not self._initialized:
-
-            dtype = self._dtype
-            n_operators = len(self._orig_operators)
-            hilb_size = self.hilbert.size
-
-            b_to_change = [] * n_operators
-            b_z_check = [] * n_operators
-
-            acting = {}
-
-            def find_char(s, ch):
-                return [i for i, ltr in enumerate(s) if ltr == ch]
-
-            def append(key, k):
-                # convert list to tuple
-                key = tuple(sorted(key))  # order of X and Y does not matter
-                if key in acting:
-                    acting[key].append(k)
-                else:
-                    acting[key] = [k]
-
-            _n_z_check_max = 0
-
-            for i, op in enumerate(self._orig_operators):
-                b_to_change = []
-                b_z_check = []
-                b_weights = self._orig_weights[i]
-
-                x_ops = find_char(op, "X")
-                if len(x_ops):
-                    b_to_change += x_ops
-
-                y_ops = find_char(op, "Y")
-                if len(y_ops):
-                    b_to_change += y_ops
-                    b_weights *= (-1.0j) ** (len(y_ops))
-                    b_z_check += y_ops
-
-                z_ops = find_char(op, "Z")
-                if len(z_ops):
-                    b_z_check += z_ops
-
-                _n_z_check_max = max(_n_z_check_max, len(b_z_check))
-                append(b_to_change, (b_weights, b_z_check))
-
-            # now group together operators with same final state
-            n_operators = len(acting)
-            _n_op_max = max(
-                list(map(lambda x: len(x), list(acting.values()))), default=n_operators
-            )
+        self._is_hermitian = None
+
+    @property
+    def operators(self) -> Iterable[str]:
+        return self._operators
 
-            # unpacking the dictionary into fixed-size arrays
-            _sites = np.empty((n_operators, hilb_size), dtype=np.intp)
-            _ns = np.empty((n_operators), dtype=np.intp)
-            _n_op = np.empty(n_operators, dtype=np.intp)
-            _weights = np.empty((n_operators, _n_op_max), dtype=dtype)
-            _nz_check = np.empty((n_operators, _n_op_max), dtype=np.intp)
-            _z_check = np.empty((n_operators, _n_op_max, _n_z_check_max), dtype=np.intp)
-
-            for i, act in enumerate(acting.items()):
-                sites = act[0]
-                nsi = len(sites)
-                _sites[i, :nsi] = sites
-                _ns[i] = nsi
-                values = act[1]
-                _n_op[i] = len(values)
-                for j in range(_n_op[i]):
-                    _weights[i, j] = values[j][0]
-                    _nz_check[i, j] = len(values[j][1])
-                    _z_check[i, j, : _nz_check[i, j]] = values[j][1]
-
-            self._sites = _sites
-            self._ns = _ns
-            self._n_op = _n_op
-            self._weights = _weights
-            self._nz_check = _nz_check
-            self._z_check = _z_check
-
-            self._x_prime_max = np.empty((n_operators, hilb_size))
-            self._mels_max = np.empty((n_operators), dtype=dtype)
-            self._n_operators = n_operators
-
-            self._local_states = np.array(self.hilbert.states_at_index(0))
-            for i in range(1, self.hilbert.size):
-                if not np.allclose(self._local_states, self.hilbert.states_at_index(i)):
-                    raise ValueError(
-                        "Hilbert spaces with non homogeneous local_states are not "
-                        "yet supported."
-                    )
+    @property
+    def weights(self) -> Iterable[str]:
+        return self._weights
 
-            self._initialized = True
+    @classmethod
+    def identity(cls, hilbert: AbstractHilbert, **kwargs):
+        return cls(hilbert, "I" * hilbert.size, **kwargs)
 
-    @staticmethod
+    @classmethod
     def from_openfermion(
+        cls,
         hilbert: AbstractHilbert,
         of_qubit_operator=None,  # : "openfermion.ops.QubitOperator" type
         *,
         n_qubits: int = None,
-    ) -> "PauliStrings":
+    ) -> "PauliStringsBase":
         r"""
         Converts an openfermion QubitOperator into a netket PauliStrings.
 
         The hilbert first argument can be dropped, see :code:`__init__` for
         details and default value
 
         Args:
@@ -271,64 +222,87 @@
         if n_qubits is None:
             n_qubits = _count_of_locations(of_qubit_operator)
         for operator, weight in of_qubit_operator.terms.items():  # gives dict
             s = ["I"] * n_qubits
             for loc, op in operator:
                 assert (
                     loc < n_qubits
-                ), "operator index {} is longer than n_qubits={}".format(loc, n_qubits)
+                ), f"operator index {loc} is longer than n_qubits={n_qubits}"
                 s[loc] = op
             operators.append("".join(s))
             weights.append(weight)
 
         ps_args = (operators, weights)
         if hilbert is not None:
             ps_args = (hilbert,) + ps_args
-        return PauliStrings(*ps_args)
+        return cls(*ps_args)
 
     @property
     def dtype(self) -> DType:
         """The dtype of the operator's matrix elements ⟨σ|Ô|σ'⟩."""
         return self._dtype
 
     @property
     def is_hermitian(self) -> bool:
         """Returns true if this operator is hermitian."""
+        if self._is_hermitian is None:
+            self._is_hermitian = np.allclose(self._weights.imag, 0.0)
         return self._is_hermitian
 
-    @property
-    def max_conn_size(self) -> int:
-        """The maximum number of non zero ⟨x|O|x'⟩ for every x."""
-        # 1 connection for every operator X, Y, Z...
-        self._setup()
-        return self._n_operators
-
     def __repr__(self):
         print_list = []
-        for op, w in zip(self._orig_operators, self._orig_weights):
-            print_list.append("    {} : {}".format(op, str(w)))
-        s = "PauliStrings(hilbert={}, n_strings={}, dict(operators:weights)=\n{}\n)".format(
-            self.hilbert, len(self._orig_operators), ",\n".join(print_list)
+        for op, w in zip(self._operators, self._weights):
+            print_list.append(f"    {op} : {str(w)}")
+        s = "{}(hilbert={}, n_strings={}, dict(operators:weights)=\n{}\n)".format(
+            type(self).__name__,
+            self.hilbert,
+            len(self._operators),
+            ",\n".join(print_list),
         )
         return s
 
+    def copy(self, *, dtype: Optional[DType] = None):
+        """Returns a copy of the operator, while optionally changing the dtype
+        of the operator.
+
+        Args:
+            dtype: optional dtype
+        """
+
+        if dtype is None:
+            dtype = self.dtype
+
+        if not np.can_cast(self.dtype, dtype, casting="same_kind"):
+            raise ValueError(f"Cannot cast {self.dtype} to {dtype}")
+
+        new = type(self)(self.hilbert, dtype=dtype)
+        new.mel_cutoff = self.mel_cutoff
+        new._operators = self._operators
+
+        if dtype == self.dtype:
+            new._weights = self._weights.copy()
+        else:
+            new._weights = cast_operator_matrix_dtype(self._weights, dtype)
+
+        return new
+
     def _op__matmul__(self, other):
-        if not isinstance(other, PauliStrings):
+        if not isinstance(other, PauliStringsBase):
             return NotImplementedError
         if not self.hilbert == other.hilbert:
             raise ValueError(
                 f"Can only multiply identical hilbert spaces (got A@B, A={self.hilbert}, B={other.hilbert})"
             )
         operators, weights = _matmul(
-            self._orig_operators,
-            self._orig_weights,
-            other._orig_operators,
-            other._orig_weights,
+            self._operators,
+            self._weights,
+            other._operators,
+            other._weights,
         )
-        return PauliStrings(
+        return type(self)(
             self.hilbert,
             operators,
             weights,
             cutoff=max(self._cutoff, other._cutoff),
             dtype=self.dtype,
         )
 
@@ -344,18 +318,18 @@
                 "For example:\n\n"
                 ">>> nk.operator.PauliStrings('XY')@nk.operator.PauliStrings('ZY')"
                 "\n\n"
             )
 
         if not np.issubdtype(type(scalar), np.number):
             raise NotImplementedError
-        weights = self._orig_weights * scalar
-        return PauliStrings(
+        weights = self._weights * scalar
+        return type(self)(
             self.hilbert,
-            self._orig_operators,
+            self._operators,
             weights,
             dtype=self.dtype,
             cutoff=self._cutoff,
         )
 
     def __sub__(self, other):
         return self + (-other)
@@ -369,163 +343,33 @@
     def __radd__(self, other):
         return self + other
 
     def __add__(self, other):
         if np.issubdtype(type(other), np.number):
             if other != 0.0:
                 # adding a constant = adding IIII...III with weight being the constant
-                return self + PauliStrings.identity(self.hilbert) * other
+                return self + self.identity(self.hilbert) * other
             return self
-        if not isinstance(other, PauliStrings):
+        if not isinstance(other, PauliStringsBase):
             raise NotImplementedError
         if not self.hilbert == other.hilbert:
             raise ValueError(
                 f"Can only add identical hilbert spaces (got A+B, A={self.hilbert}, B={other.hilbert})"
             )
-        operators = np.concatenate((self._orig_operators, other._orig_operators))
-        weights = np.concatenate((self._orig_weights, other._orig_weights))
+        operators = np.concatenate((self._operators, other._operators))
+        weights = np.concatenate((self._weights, other._weights))
         operators, weights = _reduce_pauli_string(operators, weights)
-        return PauliStrings(
+        return type(self)(
             self.hilbert,
             operators,
             weights,
             dtype=self.dtype,
             cutoff=self._cutoff,
         )
 
-    @staticmethod
-    @jit(nopython=True)
-    def _flattened_kernel(
-        x,
-        sections,
-        x_prime,
-        mels,
-        sites,
-        ns,
-        n_op,
-        weights,
-        nz_check,
-        z_check,
-        cutoff,
-        max_conn,
-        local_states,
-        pad=False,
-    ):
-        x_prime = np.empty((x.shape[0] * max_conn, x_prime.shape[1]), dtype=x.dtype)
-        mels = np.zeros((x.shape[0] * max_conn), dtype=mels.dtype)
-        state_1 = local_states[-1]
-
-        n_c = 0
-        for b in range(x.shape[0]):
-            xb = x[b]
-            # initialize
-            x_prime[b * max_conn : (b + 1) * max_conn, :] = np.copy(xb)
-
-            for i in range(sites.shape[0]):
-                mel = 0.0
-                for j in range(n_op[i]):
-                    if nz_check[i, j] > 0:
-                        to_check = z_check[i, j, : nz_check[i, j]]
-                        n_z = np.count_nonzero(xb[to_check] == state_1)
-                    else:
-                        n_z = 0
-
-                    mel += weights[i, j] * (-1.0) ** n_z
-
-                if abs(mel) > cutoff:
-                    x_prime[n_c] = np.copy(xb)
-                    for site in sites[i, : ns[i]]:
-                        new_state_idx = int(x_prime[n_c, site] == local_states[0])
-                        x_prime[n_c, site] = local_states[new_state_idx]
-                    mels[n_c] = mel
-                    n_c += 1
-
-            if pad:
-                n_c = (b + 1) * max_conn
-
-            sections[b] = n_c
-        return x_prime[:n_c], mels[:n_c]
-
-    def get_conn_flattened(self, x, sections, pad=False):
-        r"""Finds the connected elements of the Operator. Starting
-        from a given quantum number x, it finds all other quantum numbers x' such
-        that the matrix element :math:`O(x,x')` is different from zero. In general there
-        will be several different connected states x' satisfying this
-        condition, and they are denoted here :math:`x'(k)`, for :math:`k=0,1...N_{\mathrm{connected}}`.
-
-        This is a batched version, where x is a matrix of shape (batch_size,hilbert.size).
-
-        Args:
-            x (matrix): A matrix of shape (batch_size,hilbert.size) containing
-                        the batch of quantum numbers x.
-            sections (array): An array of size (batch_size) useful to unflatten
-                        the output of this function.
-                        See numpy.split for the meaning of sections.
-
-        Returns:
-            matrix: The connected states x', flattened together in a single matrix.
-            array: An array containing the matrix elements :math:`O(x,x')` associated to each x'.
-
-        """
-        self._setup()
-        x = np.array(x)
-        assert (
-            x.shape[-1] == self.hilbert.size
-        ), "size of hilbert space does not match size of x"
-        return self._flattened_kernel(
-            x,
-            sections,
-            self._x_prime_max,
-            self._mels_max,
-            self._sites,
-            self._ns,
-            self._n_op,
-            self._weights,
-            self._nz_check,
-            self._z_check,
-            self._cutoff,
-            self._n_operators,
-            self._local_states,
-            pad,
-        )
-
-    def _get_conn_flattened_closure(self):
-        self._setup()
-        _x_prime_max = self._x_prime_max
-        _mels_max = self._mels_max
-        _sites = self._sites
-        _ns = self._ns
-        _n_op = self._n_op
-        _weights = self._weights
-        _nz_check = self._nz_check
-        _z_check = self._z_check
-        _cutoff = self._cutoff
-        _n_operators = self._n_operators
-        fun = self._flattened_kernel
-        _local_states = self._local_states
-
-        def gccf_fun(x, sections):
-            return fun(
-                x,
-                sections,
-                _x_prime_max,
-                _mels_max,
-                _sites,
-                _ns,
-                _n_op,
-                _weights,
-                _nz_check,
-                _z_check,
-                _cutoff,
-                _n_operators,
-                _local_states,
-            )
-
-        return jit(nopython=True)(gccf_fun)
-
 
 def _count_of_locations(of_qubit_operator):
     """Obtain the number of qubits in the openfermion QubitOperator. Openfermion builds operators from terms that store operators locations.
     Args:
         of_qubit_operator (openfermion.QubitOperator, openfermion.FermionOperator)
     Returns:
         n_qubits (int): number of qubits in the operator, which we can use to create a suitable hilbert space
```

### Comparing `netket-3.8/netket/operator/_potential.py` & `netket-3.9/netket/operator/_potential.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/operator/_sumoperators.py` & `netket-3.9/netket/operator/_sumoperators.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/operator/boson.py` & `netket-3.9/netket/operator/boson.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/operator/spin.py` & `netket-3.9/netket/operator/spin.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,16 @@
 
         old_dtype = dtype
         dtype = jnp.promote_types(complex, old_dtype)
         warnings.warn(
             np.ComplexWarning(
                 f"A complex dtype is required (dtype={old_dtype} specified). "
                 f"Promoting to dtype={dtype}."
-            )
+            ),
+            stacklevel=2,
         )
 
     N = hilbert.size_at_index(site)
     S = (N - 1) / 2
 
     D = np.array([1j * np.sqrt((S + 1) * 2 * a - a * (a + 1)) for a in np.arange(1, N)])
     mat = np.diag(D, -1) + np.diag(-D, 1)
```

### Comparing `netket-3.8/netket/optimizer/__init__.py` & `netket-3.9/netket/optimizer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from . import qgt, solver
+from . import solver
+from . import qgt
 
 from .linear_operator import LinearOperator
 from .preconditioner import (
     LinearPreconditioner,
     PreconditionerT,
     identity_preconditioner,
     DeprecatedPreconditionerSignature as _DeprecatedPreconditionerSignature,
```

### Comparing `netket-3.8/netket/optimizer/linear_operator.py` & `netket-3.9/netket/optimizer/linear_operator.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/optimizer/preconditioner.py` & `netket-3.9/netket/optimizer/preconditioner.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/optimizer/sr.py` & `netket-3.9/netket/optimizer/sr.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/optimizer/qgt/__init__.py` & `netket-3.9/netket/optimizer/qgt/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/optimizer/qgt/default.py` & `netket-3.9/netket/optimizer/qgt/default.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,17 +19,25 @@
 
 import netket.jax as nkjax
 
 from .qgt_jacobian_dense import QGTJacobianDense
 from .qgt_jacobian_pytree import QGTJacobianPyTree
 from .qgt_onthefly import QGTOnTheFly
 
-from ..solver import cholesky, svd, LU, solve
+from .. import solver as nk_solver_module
 
-solvers = [cholesky, svd, LU, solve]
+solvers = []
+
+for solver in dir(nk_solver_module):
+    # only add solvers, not random
+    # useless things
+    if solver[:2] == "__":
+        continue
+    else:
+        solvers.append(getattr(nk_solver_module, solver))
 
 
 def _is_dense_solver(solver: Any) -> bool:
     """
     Returns true if the solver is one of our known dense solvers
     """
     if isinstance(solver, partial):
@@ -41,17 +49,17 @@
     return False
 
 
 def default_qgt_matrix(variational_state, solver=False, **kwargs):
     """
     Determines default metric tensor depending on variational_state and solver
     """
-    from netket.vqs import ExactState
+    from netket.vqs import FullSumState
 
-    if isinstance(variational_state, ExactState):
+    if isinstance(variational_state, FullSumState):
         return partial(QGTJacobianPyTree, **kwargs)
 
     n_param_leaves = len(jax.tree_util.tree_leaves(variational_state.parameters))
     n_params = variational_state.n_parameters
 
     # those require dense matrix that is known to be faster for this qgt
     if _is_dense_solver(solver):
```

### Comparing `netket-3.8/netket/optimizer/qgt/qgt_jacobian_common.py` & `netket-3.9/netket/optimizer/qgt/qgt_jacobian_common.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,35 +13,15 @@
 # limitations under the License.
 
 from functools import partial
 
 import jax
 import jax.numpy as jnp
 
-from netket.utils import mpi, warn_deprecation, deprecated
-
-
-@deprecated(
-    """
-    It seems you're using the internal function
-
-        nk.optimizer.qgt.qgt_jacobian_common.choose_jacobian_mode
-
-    which has been moved to
-
-        nk.jax.jacobian_default_mode
-
-    please update the import location.
-    This deprecation warning will become an error in NetKet 3.9
-    """
-)
-def choose_jacobian_mode(*args, **kwargs):
-    from netket.jax import jacobian_default_mode
-
-    return jacobian_default_mode(*args, **kwargs)
+from netket.utils import mpi, warn_deprecation
 
 
 def sanitize_diag_shift(diag_shift, diag_scale, rescale_shift):
     """Sanitises different inputs for diag_shift etc.
 
 
     Also raises a deprecation warnings for `rescale_shift`.
```

### Comparing `netket-3.8/netket/optimizer/qgt/qgt_jacobian_dense.py` & `netket-3.9/netket/optimizer/qgt/qgt_jacobian_dense.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,21 +97,24 @@
             rescale_shift=rescale_shift,
             **kwargs,
         )
 
     diag_shift, diag_scale = sanitize_diag_shift(diag_shift, diag_scale, rescale_shift)
 
     # TODO: Find a better way to handle this case
-    from netket.vqs import ExactState
+    from netket.vqs import FullSumState
 
-    if isinstance(vstate, ExactState):
+    if isinstance(vstate, FullSumState):
         samples = split_array_mpi(vstate._all_states)
         pdf = split_array_mpi(vstate.probability_distribution())
     else:
         samples = vstate.samples
+        if samples.ndim >= 3:
+            # use jit so that we can do it on global shared array
+            samples = jax.jit(jax.lax.collapse, static_argnums=(1, 2))(samples, 0, 2)
         pdf = None
 
     if mode is None:
         mode = nkjax.jacobian_default_mode(
             vstate._apply_fun,
             vstate.parameters,
             vstate.model_state,
@@ -123,15 +126,15 @@
         chunk_size = vstate.chunk_size
 
     shift, offset = to_shift_offset(diag_shift, diag_scale)
 
     jacobians = nkjax.jacobian(
         vstate._apply_fun,
         vstate.parameters,
-        samples.reshape(-1, samples.shape[-1]),
+        samples,
         vstate.model_state,
         mode=mode,
         pdf=pdf,
         chunk_size=chunk_size,
         dense=True,
         center=True,
     )
```

### Comparing `netket-3.8/netket/optimizer/qgt/qgt_jacobian_pytree.py` & `netket-3.9/netket/optimizer/qgt/qgt_jacobian_pytree.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,21 +98,24 @@
             rescale_shift=rescale_shift,
             **kwargs,
         )
 
     diag_shift, diag_scale = sanitize_diag_shift(diag_shift, diag_scale, rescale_shift)
 
     # TODO: Find a better way to handle this case
-    from netket.vqs import ExactState
+    from netket.vqs import FullSumState
 
-    if isinstance(vstate, ExactState):
+    if isinstance(vstate, FullSumState):
         samples = split_array_mpi(vstate._all_states)
         pdf = split_array_mpi(vstate.probability_distribution())
     else:
         samples = vstate.samples
+        if samples.ndim >= 3:
+            # use jit so that we can do it on global shared array
+            samples = jax.jit(jax.lax.collapse, static_argnums=(1, 2))(samples, 0, 2)
         pdf = None
 
     # Choose sensible default mode
     if mode is None:
         mode = nkjax.jacobian_default_mode(
             vstate._apply_fun,
             vstate.parameters,
@@ -125,15 +128,15 @@
         chunk_size = vstate.chunk_size
 
     shift, offset = to_shift_offset(diag_shift, diag_scale)
 
     jacobians = nkjax.jacobian(
         vstate._apply_fun,
         vstate.parameters,
-        samples.reshape(-1, samples.shape[-1]),
+        samples,
         vstate.model_state,
         mode=mode,
         pdf=pdf,
         chunk_size=chunk_size,
         dense=False,
         center=True,
     )
```

### Comparing `netket-3.8/netket/optimizer/qgt/qgt_jacobian_pytree_logic.py` & `netket-3.9/netket/optimizer/qgt/qgt_jacobian_pytree_logic.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/optimizer/qgt/qgt_onthefly.py` & `netket-3.9/netket/optimizer/qgt/qgt_onthefly.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,31 +10,39 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Callable, Optional, Union
 from functools import partial
+import warnings
 
 import jax
 from jax import numpy as jnp
 from flax import struct
 
 import netket.jax as nkjax
 from netket.utils.types import PyTree
 
+from netket.errors import (
+    IllegalHolomorphicDeclarationForRealParametersError,
+    NonHolomorphicQGTOnTheFlyDenseRepresentationError,
+    HolomorphicUndeclaredWarning,
+)
 from netket.nn import split_array_mpi
 
 from .common import check_valid_vector_type
 from .qgt_onthefly_logic import mat_vec_factory, mat_vec_chunked_factory
 
 from ..linear_operator import LinearOperator, Uninitialized
 
 
-def QGTOnTheFly(vstate=None, *, chunk_size=None, **kwargs) -> "QGTOnTheFlyT":
+def QGTOnTheFly(
+    vstate=None, *, chunk_size=None, holomorphic: bool = None, **kwargs
+) -> "QGTOnTheFlyT":
     """
     Lazy representation of an S Matrix computed by performing 2 jvp
     and 1 vjp products, using the variational state's model, the
     samples that have already been computed, and the vector.
 
     The S matrix is not computed yet, but can be computed by calling
     :code:`to_dense`.
@@ -44,35 +52,37 @@
     Args:
         vstate: The variational State.
         chunk_size: If supplied, overrides the chunk size of the variational state
                     (useful for models where the backward pass requires more
                     memory than the forward pass).
     """
     if vstate is None:
-        return partial(QGTOnTheFly, chunk_size=chunk_size, **kwargs)
+        return partial(
+            QGTOnTheFly, chunk_size=chunk_size, holomorphic=holomorphic, **kwargs
+        )
 
     if kwargs.pop("diag_scale", None) is not None:
         raise NotImplementedError(
             "\n`diag_scale` argument is not yet supported by QGTOnTheFly."
             "Please use `QGTJacobianPyTree` or `QGTJacobianDense`.\n\n"
             "You are also encouraged to nag the developers to support "
             "this feature.\n\n"
         )
 
     # TODO: Find a better way to handle this case
-    from netket.vqs import ExactState
+    from netket.vqs import FullSumState
 
-    if isinstance(vstate, ExactState):
+    if isinstance(vstate, FullSumState):
         samples = split_array_mpi(vstate._all_states)
         pdf = split_array_mpi(vstate.probability_distribution())
     else:
-        if jnp.ndim(vstate.samples) == 2:
-            samples = vstate.samples
-        else:
-            samples = vstate.samples.reshape((-1, vstate.samples.shape[-1]))
+        samples = vstate.samples
+        if samples.ndim >= 3:
+            # use jit so that we can do it on global shared array
+            samples = jax.jit(jax.lax.collapse, static_argnums=(1, 2))(samples, 0, 2)
         pdf = None
 
     if chunk_size is None and hasattr(vstate, "chunk_size"):
         chunk_size = vstate.chunk_size
 
     n_samples = samples.shape[0]
 
@@ -82,25 +92,48 @@
     else:
         samples, _ = nkjax.chunk(samples, chunk_size)
         if pdf is not None:
             pdf, _ = nkjax.chunk(pdf, chunk_size)
         mv_factory = mat_vec_chunked_factory
         chunking = True
 
+    # check if holomorphic or not
+    if holomorphic:
+        if nkjax.tree_leaf_isreal(vstate.parameters):
+            raise IllegalHolomorphicDeclarationForRealParametersError()
+        else:
+            mode = "holomorphic"
+    else:
+        if not nkjax.tree_leaf_iscomplex(vstate.parameters):
+            mode = "real"
+        else:
+            if holomorphic is None:
+                warnings.warn(HolomorphicUndeclaredWarning(), UserWarning)
+            mode = "complex"
+
+    nkjax.jacobian_default_mode(
+        vstate._apply_fun,
+        vstate.parameters,
+        vstate.model_state,
+        samples,
+        holomorphic=holomorphic,
+    )
+
     mat_vec = mv_factory(
         forward_fn=vstate._apply_fun,
         params=vstate.parameters,
         model_state=vstate.model_state,
         samples=samples,
         pdf=pdf,
     )
     return QGTOnTheFlyT(
         _mat_vec=mat_vec,
         _params=vstate.parameters,
         _chunking=chunking,
+        _mode=mode,
         **kwargs,
     )
 
 
 @struct.dataclass
 class QGTOnTheFlyT(LinearOperator):
     """
@@ -121,27 +154,47 @@
     _params: PyTree = Uninitialized
     """The first input to apply_fun (parameters of the ansatz).
     Only used as a shape placeholder."""
 
     _chunking: bool = struct.field(pytree_node=False, default=False)
     """Whether the implementation with chunks is used which currently does not support vmapping over it"""
 
+    _mode: str = struct.field(pytree_node=False, default=None)
+    """Differentiation mode:
+        - "real": for real-valued R->R and C->R Ansätze, splits the complex inputs
+                  into real and imaginary part.
+        - "complex": for complex-valued R->C and C->C Ansätze, splits the complex
+                  inputs and outputs into real and imaginary part
+        - "holomorphic": for any Ansätze. Does not split complex values.
+        - "auto": autoselect real or complex.
+    """
+
     def __matmul__(self, y):
         return onthefly_mat_treevec(self, y)
 
     def _solve(self, solve_fun, y: PyTree, *, x0: Optional[PyTree], **kwargs) -> PyTree:
         return _solve(self, solve_fun, y, x0=x0)
 
     def to_dense(self) -> jnp.ndarray:
         """
         Convert the lazy matrix representation to a dense matrix representation.
 
         Returns:
             A dense matrix representation of this S matrix.
         """
+        # This condition will be true if the user specified `holomorphic=False` and
+        # if the parameters are complex. If the parameters are real and the user
+        # did not specify holomorphic we will have mode==real and if holomorphic is
+        # True mode==holomorphic.
+        #
+        # We must check this because the AD implementation will compute the wrong
+        # QGT in that case
+        if self._mode == "complex":
+            raise NonHolomorphicQGTOnTheFlyDenseRepresentationError()
+
         return _to_dense(self)
 
     def __repr__(self):
         return f"QGTOnTheFly(diag_shift={self.diag_shift})"
 
 
 @jax.jit
```

### Comparing `netket-3.8/netket/optimizer/qgt/qgt_onthefly_logic.py` & `netket-3.9/netket/optimizer/qgt/qgt_onthefly_logic.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/sampler/__init__.py` & `netket-3.9/netket/sampler/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/sampler/autoreg.py` & `netket-3.9/netket/sampler/autoreg.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,21 +153,21 @@
             return (σ, cache, new_key), None
 
         new_key, key_init, key_scan = jax.random.split(state.key, 3)
 
         # We just need a buffer for `σ` before generating each sample
         # The result does not depend on the initial contents in it
         σ = jnp.zeros(
-            (chain_length * sampler.n_chains_per_rank, sampler.hilbert.size),
+            (sampler.n_chains_per_rank * chain_length, sampler.hilbert.size),
             dtype=sampler.dtype,
         )
 
         # Initialize `cache` before generating each sample,
         # even if `variables` is not changed and `reset` is not called
         cache = sampler._init_cache(model, σ, key_init)
 
         indices = jnp.arange(sampler.hilbert.size)
         (σ, _, _), _ = jax.lax.scan(scan_fun, (σ, cache, key_scan), indices)
-        σ = σ.reshape((chain_length, sampler.n_chains_per_rank, sampler.hilbert.size))
+        σ = σ.reshape((sampler.n_chains_per_rank, chain_length, sampler.hilbert.size))
 
         new_state = state.replace(key=new_key)
         return σ, new_state
```

### Comparing `netket-3.8/netket/sampler/base.py` & `netket-3.9/netket/sampler/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,14 +103,15 @@
                             f"Using {n_chains_per_rank} chains per rank among {mpi.n_nodes} ranks "
                             f"(total={n_chains_per_rank * mpi.n_nodes} instead of n_chains={n_chains}). "
                             f"To directly control the number of chains on every rank, specify "
                             f"`n_chains_per_rank` when constructing the sampler. "
                             f"To silence this warning, either use `n_chains_per_rank` or use `n_chains` "
                             f"that is a multiple of the number of MPI ranks.",
                             category=UserWarning,
+                            stacklevel=2,
                         )
 
             kwargs["n_chains_per_rank"] = n_chains_per_rank
 
         return (hilbert,), kwargs
 
     def __post_init__(self):
@@ -294,17 +295,17 @@
             chain_length: The length of the chains (default = 1).
         """
         if state is None:
             state = sampler.reset(machine, parameters)
 
         machine = wrap_afun(machine)
 
-        for i in range(chain_length):
+        for _i in range(chain_length):
             samples, state = sampler._sample_chain(machine, parameters, state, 1)
-            yield samples[0, :, :]
+            yield samples[:, 0, :]
 
     @abc.abstractmethod
     def _sample_chain(
         sampler,
         machine: nn.Module,
         parameters: PyTree,
         state: SamplerState,
```

### Comparing `netket-3.8/netket/sampler/exact.py` & `netket-3.9/netket/sampler/exact.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from flax import linen as nn
 from jax import numpy as jnp
 
 from netket.nn import to_array
 from netket.utils import struct
 from netket.utils.deprecation import warn_deprecation
 from netket.utils.types import PyTree, SeedT
-from netket.utils import pure_callback
 
 from .base import Sampler, SamplerState
 
 
 @struct.dataclass
 class ExactSamplerState(SamplerState):
     pdf: Any
@@ -109,20 +108,20 @@
         # We use a host-callback to convert integers labelling states to
         # valid state-arrays because that code is written with numba and
         # we have not yet converted it to jax.
         #
         # For future investigators:
         # this will lead to a crash if numbers_to_state throws.
         # it throws if we feed it nans!
-        samples = pure_callback(
+        samples = jax.pure_callback(
             lambda numbers: sampler.hilbert.numbers_to_states(numbers),
             jax.ShapeDtypeStruct(
-                (chain_length * sampler.n_chains_per_rank, sampler.hilbert.size),
+                (sampler.n_chains_per_rank * chain_length, sampler.hilbert.size),
                 jnp.float64,
             ),
             numbers,
         )
         samples = jnp.asarray(samples, dtype=sampler.dtype).reshape(
-            chain_length, sampler.n_chains_per_rank, sampler.hilbert.size
+            sampler.n_chains_per_rank, chain_length, sampler.hilbert.size
         )
 
         return samples, state.replace(rng=new_rng)
```

### Comparing `netket-3.8/netket/sampler/metropolis.py` & `netket-3.9/netket/sampler/metropolis.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,19 +50,23 @@
 
     # those are initialised to 0. We want to initialise them to zero arrays because they can
     # be passed to jax jitted functions that require type invariance to avoid recompilation
     n_steps_proc: int = struct.field(
         default_factory=lambda: jnp.zeros((), dtype=jnp.int64)
     )
     """Number of moves performed along the chains in this process since the last reset."""
-    n_accepted_proc: int = struct.field(
-        default_factory=lambda: jnp.zeros((), dtype=jnp.int64)
-    )
+    n_accepted_proc: jnp.ndarray = None
     """Number of accepted transitions among the chains in this process since the last reset."""
 
+    def __post_init__(self):
+        if self.n_accepted_proc is None:
+            object.__setattr__(
+                self, "n_accepted_proc", jnp.zeros(self.σ.shape[0], dtype=jnp.int64)
+            )
+
     @property
     def acceptance(self) -> float:
         """The fraction of accepted moves across all chains and MPI processes.
 
         The rate is computed since the last reset of the sampler.
         Will return None if no sampling has been performed since then.
         """
@@ -75,15 +79,16 @@
     def n_steps(self) -> int:
         """Total number of moves performed across all processes since the last reset."""
         return self.n_steps_proc * mpi.n_nodes
 
     @property
     def n_accepted(self) -> int:
         """Total number of moves accepted across all processes since the last reset."""
-        res, _ = mpi.mpi_sum_jax(self.n_accepted_proc)
+        # jit sum for gda
+        res, _ = mpi.mpi_sum_jax(jax.jit(jnp.sum)(self.n_accepted_proc))
         return res
 
     def __repr__(self):
         if self.n_steps > 0:
             acc_string = "# accepted = {}/{} ({}%), ".format(
                 self.n_accepted, self.n_steps, self.acceptance * 100
             )
@@ -258,15 +263,17 @@
                 f"{sampler.rule}.random_state",
             )
             state = state.replace(σ=σ, rng=key_state)
 
         return state
 
     def _reset(sampler, machine, parameters, state):
-        new_rng, rng = jax.random.split(state.rng)
+        new_rng, rng = jax.jit(jax.random.split)(
+            state.rng
+        )  # use jit so that we can do it on global shared array
 
         if sampler.reset_chains:
             σ = sampler.rule.random_state(sampler, machine, parameters, state, rng)
             _assert_good_sample_shape(
                 σ,
                 (sampler.n_chains_per_rank, sampler.hilbert.size),
                 sampler.dtype,
@@ -274,15 +281,19 @@
             )
         else:
             σ = state.σ
 
         rule_state = sampler.rule.reset(sampler, machine, parameters, state)
 
         return state.replace(
-            σ=σ, rng=new_rng, rule_state=rule_state, n_steps_proc=0, n_accepted_proc=0
+            σ=σ,
+            rng=new_rng,
+            rule_state=rule_state,
+            n_steps_proc=jnp.zeros_like(state.n_steps_proc),
+            n_accepted_proc=jnp.zeros_like(state.n_accepted_proc),
         )
 
     def _sample_next(sampler, machine, parameters, state):
         """
         Implementation of `sample_next` for subclasses of `MetropolisSampler`.
 
         If you subclass `MetropolisSampler`, you should override this and not `sample_next`
@@ -313,15 +324,15 @@
                     proposal_log_prob - s["log_prob"] + log_prob_correction
                 )
             else:
                 do_accept = uniform < jnp.exp(proposal_log_prob - s["log_prob"])
 
             # do_accept must match ndim of proposal and state (which is 2)
             s["σ"] = jnp.where(do_accept.reshape(-1, 1), σp, s["σ"])
-            s["accepted"] += do_accept.sum()
+            s["accepted"] += do_accept
 
             s["log_prob"] = jax.numpy.where(
                 do_accept.reshape(-1), proposal_log_prob, s["log_prob"]
             )
 
             return s
 
@@ -366,39 +377,40 @@
         """
         state, samples = jax.lax.scan(
             lambda state, _: sampler.sample_next(machine, parameters, state),
             state,
             xs=None,
             length=chain_length,
         )
-
+        # make it (n_chains, n_samples_per_chain) as expected by netket.stats.statistics
+        samples = jnp.swapaxes(samples, 0, 1)
         return samples, state
 
     def __repr__(sampler):
         return (
             f"{type(sampler).__name__}("
-            + "\n  hilbert = {},".format(sampler.hilbert)
-            + "\n  rule = {},".format(sampler.rule)
-            + "\n  n_chains = {},".format(sampler.n_chains)
-            + "\n  n_sweeps = {},".format(sampler.n_sweeps)
-            + "\n  reset_chains = {},".format(sampler.reset_chains)
-            + "\n  machine_power = {},".format(sampler.machine_pow)
-            + "\n  dtype = {}".format(sampler.dtype)
+            + f"\n  hilbert = {sampler.hilbert},"
+            + f"\n  rule = {sampler.rule},"
+            + f"\n  n_chains = {sampler.n_chains},"
+            + f"\n  n_sweeps = {sampler.n_sweeps},"
+            + f"\n  reset_chains = {sampler.reset_chains},"
+            + f"\n  machine_power = {sampler.machine_pow},"
+            + f"\n  dtype = {sampler.dtype}"
             + ")"
         )
 
     def __str__(sampler):
         return (
             f"{type(sampler).__name__}("
-            + "rule = {}, ".format(sampler.rule)
-            + "n_chains = {}, ".format(sampler.n_chains)
-            + "n_sweeps = {}, ".format(sampler.n_sweeps)
-            + "reset_chains = {}, ".format(sampler.reset_chains)
-            + "machine_power = {}, ".format(sampler.machine_pow)
-            + "dtype = {})".format(sampler.dtype)
+            + f"rule = {sampler.rule}, "
+            + f"n_chains = {sampler.n_chains}, "
+            + f"n_sweeps = {sampler.n_sweeps}, "
+            + f"reset_chains = {sampler.reset_chains}, "
+            + f"machine_power = {sampler.machine_pow}, "
+            + f"dtype = {sampler.dtype})"
         )
 
 
 @deprecated(
     "The module function `sample_next` is deprecated in favor of the class method `sample_next`."
 )
 def sample_next(
@@ -561,15 +573,15 @@
        >>>
        >>> # Transverse-field Ising Hamiltonian
        >>> ha = nk.operator.Ising(hilbert=hi, h=1.0, graph=g)
        >>>
        >>> # Construct a MetropolisHamiltonian Sampler
        >>> sa = nk.sampler.MetropolisHamiltonian(hi, hamiltonian=ha)
        >>> print(sa)
-       MetropolisSampler(rule = HamiltonianRule(Ising(J=1.0, h=1.0; dim=100)), n_chains = 16, n_sweeps = 100, reset_chains = False, machine_power = 2, dtype = <class 'numpy.float64'>)
+       MetropolisSampler(rule = HamiltonianRuleNumba(Ising(J=1.0, h=1.0; dim=100)), n_chains = 16, n_sweeps = 100, reset_chains = False, machine_power = 2, dtype = <class 'numpy.float64'>)
     """
     from .rules import HamiltonianRule
 
     rule = HamiltonianRule(hamiltonian)
     return MetropolisSampler(hilbert, rule, **kwargs)
```

### Comparing `netket-3.8/netket/sampler/metropolis_numpy.py` & `netket-3.9/netket/sampler/metropolis_numpy.py`

 * *Files 6% similar despite different names*

```diff
@@ -210,37 +210,40 @@
             (chain_length, sampler.n_chains, sampler.hilbert.size), dtype=sampler.dtype
         )
 
         for i in range(chain_length):
             state, σ = sampler.sample_next(machine, parameters, state)
             samples[i] = σ
 
+        # make it (n_chains, n_samples_per_chain) as expected by netket.stats.statistics
+        samples = np.swapaxes(samples, 0, 1)
+
         return samples, state
 
     def __repr__(sampler):
         return (
             "MetropolisSamplerNumpy("
-            + "\n  hilbert = {},".format(sampler.hilbert)
-            + "\n  rule = {},".format(sampler.rule)
-            + "\n  n_chains = {},".format(sampler.n_chains)
-            + "\n  machine_power = {},".format(sampler.machine_pow)
-            + "\n  reset_chains = {},".format(sampler.reset_chains)
-            + "\n  n_sweeps = {},".format(sampler.n_sweeps)
-            + "\n  dtype = {},".format(sampler.dtype)
+            + f"\n  hilbert = {sampler.hilbert},"
+            + f"\n  rule = {sampler.rule},"
+            + f"\n  n_chains = {sampler.n_chains},"
+            + f"\n  machine_power = {sampler.machine_pow},"
+            + f"\n  reset_chains = {sampler.reset_chains},"
+            + f"\n  n_sweeps = {sampler.n_sweeps},"
+            + f"\n  dtype = {sampler.dtype},"
             + ")"
         )
 
     def __str__(sampler):
         return (
             "MetropolisSamplerNumpy("
-            + "rule = {}, ".format(sampler.rule)
-            + "n_chains = {}, ".format(sampler.n_chains)
-            + "machine_power = {}, ".format(sampler.machine_pow)
-            + "n_sweeps = {}, ".format(sampler.n_sweeps)
-            + "dtype = {})".format(sampler.dtype)
+            + f"rule = {sampler.rule}, "
+            + f"n_chains = {sampler.n_chains}, "
+            + f"machine_power = {sampler.machine_pow}, "
+            + f"n_sweeps = {sampler.n_sweeps}, "
+            + f"dtype = {sampler.dtype})"
         )
 
 
 @jit(nopython=True)
 def acceptance_kernel(
     σ, σ1, log_values, log_values_1, log_prob_corr, machine_pow, random_uniform
 ):
```

### Comparing `netket-3.8/netket/sampler/rules/__init__.py` & `netket-3.9/netket/sampler/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/sampler/rules/base.py` & `netket-3.9/netket/sampler/rules/base.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/sampler/rules/continuous_gaussian.py` & `netket-3.9/netket/sampler/rules/continuous_gaussian.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,8 +55,8 @@
         ) * jnp.asarray(rule.sigma, dtype=r.dtype)
 
         rp = jnp.where(np.equal(boundary, False), (r + prop), (r + prop) % modulus)
 
         return rp, None
 
     def __repr__(self):
-        return "GaussianRule(sigma={})".format(self.sigma)
+        return f"GaussianRule(sigma={self.sigma})"
```

### Comparing `netket-3.8/netket/sampler/rules/custom_numpy.py` & `netket-3.9/netket/sampler/rules/custom_numpy.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/sampler/rules/exchange.py` & `netket-3.9/netket/sampler/rules/exchange.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/sampler/rules/fixed.py` & `netket-3.9/netket/sampler/rules/fixed.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/sampler/rules/hamiltonian_numpy.py` & `netket-3.9/netket/sampler/rules/hamiltonian_numpy.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/sampler/rules/langevin.py` & `netket-3.9/netket/sampler/rules/langevin.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         )
 
         rp = jnp.where(np.equal(boundary, False), rp, rp % modulus)
 
         return rp, log_corr
 
     def __repr__(self):
-        return "LangevinRule(dt={})".format(self.dt)
+        return f"LangevinRule(dt={self.dt})"
 
 
 @partial(jax.jit, static_argnames=("apply_fun", "chunk_size", "return_log_corr"))
 def _langevin_step(
     key,
     r,
     apply_fun,
```

### Comparing `netket-3.8/netket/sampler/rules/local.py` & `netket-3.9/netket/sampler/rules/local.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/sampler/rules/local_numpy.py` & `netket-3.9/netket/sampler/rules/local_numpy.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/sampler/rules/multiple.py` & `netket-3.9/netket/sampler/rules/multiple.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/sampler/rules/tensor.py` & `netket-3.9/netket/sampler/rules/tensor.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/stats/__init__.py` & `netket-3.9/netket/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/stats/_autocorr.py` & `netket-3.9/netket/stats/_autocorr.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/stats/mc_stats.py` & `netket-3.9/netket/stats/mc_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,17 +33,17 @@
         return (
             "{0:.{1}f}".format(value, decimals + 1),
             "{0:.{1}f}".format(std, decimals + 1),
             "{0:.{1}f}".format(var, decimals + 1),
         )
     else:
         return (
-            "{0:.3e}".format(value),
-            "{0:.3e}".format(std),
-            "{0:.3e}".format(var),
+            f"{value:.3e}",
+            f"{std:.3e}",
+            f"{var:.3e}",
         )
 
 
 _NaN = float("NaN")
 
 
 def _maybe_item(x):
@@ -106,21 +106,21 @@
 
     def to_compound(self):
         return "Mean", self.to_dict()
 
     def __repr__(self):
         mean, err, var = _format_decimal(self.mean, self.error_of_mean, self.variance)
         if not math.isnan(self.R_hat):
-            ext = ", R̂={:.4f}".format(self.R_hat)
+            ext = f", R̂={self.R_hat:.4f}"
         else:
             ext = ""
         if config.netket_experimental_fft_autocorrelation:
             if not (math.isnan(self.tau_corr) and math.isnan(self.tau_corr_max)):
-                ext += ", τ={:.1f}<{:.1f}".format(self.tau_corr, self.tau_corr_max)
-        return "{} ± {} [σ²={}{}]".format(mean, err, var, ext)
+                ext += f", τ={self.tau_corr:.1f}<{self.tau_corr_max:.1f}"
+        return f"{mean} ± {err} [σ²={var}{ext}]"
 
     # Alias accessors
     def __getattr__(self, name):
         if name in ("mean", "Mean"):
             return self.mean
         elif name in ("variance", "Variance"):
             return self.variance
@@ -129,17 +129,15 @@
         elif name in ("R_hat", "R"):
             return self.R_hat
         elif name in ("tau_corr", "TauCorr"):
             return self.tau_corr
         elif name in ("tau_corr_max", "TauCorrMax"):
             return self.tau_corr_max
         else:
-            raise AttributeError(
-                "'Stats' object object has no attribute '{}'".format(name)
-            )
+            raise AttributeError(f"'Stats' object object has no attribute '{name}'")
 
     def real(self):
         return self.replace(mean=np.real(self.mean))
 
     def imag(self):
         return self.replace(mean=np.imag(self.mean))
```

### Comparing `netket-3.8/netket/stats/mc_stats_old.py` & `netket-3.9/netket/stats/mc_stats_old.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/stats/mpi_stats.py` & `netket-3.9/netket/stats/mpi_stats.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/tools/_common.py` & `netket-3.9/netket/tools/_common.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/tools/_cpu_info.py` & `netket-3.9/netket/tools/_cpu_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             m = re.search(
                 r"(?m)^Cpus_allowed:\s*(.*)$", open("/proc/self/status").read()
             )
             if m:
                 res = bin(int(m.group(1).replace(",", ""), 16)).count("1")
                 if res > 0:
                     return res
-        except IOError:
+        except OSError:
             pass
     else:
         import multiprocessing
 
         return multiprocessing.cpu_count()
 
 
@@ -92,15 +92,15 @@
     "model name": "brand",
     "cpu cores": "core_count",
     "cpu_cores": "core_count",
 }
 
 
 def get_proc_cpuinfo():
-    with open("/proc/cpuinfo", "rt") as fobj:
+    with open("/proc/cpuinfo") as fobj:
         pci_lines = fobj.readlines()
     info = {}
     for line in pci_lines:
         line = line.strip()
         if line == "":  # End of first processor
             break
         key, value = line.split(":", 1)
```

### Comparing `netket-3.8/netket/tools/_mpi_info.py` & `netket-3.9/netket/tools/_mpi_info.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/tools/check_mpi.py` & `netket-3.9/netket/tools/check_mpi.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/tools/info.py` & `netket-3.9/netket/tools/info.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/__init__.py` & `netket-3.9/netket/utils/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 from . import _dependencies_check
 
 from . import dispatch
 from . import struct
 from . import numbers
 from . import types
 from . import float
-from . import errors
 
 from .array import HashableArray
 from .partial import HashablePartial
 from .jax import get_afun_if_module, wrap_afun, wrap_to_support_scalar
 from .optional_deps import tensorboard_available
 from .seed import random_seed
 from .summation import KahanSum
 
+from .holomorphic import is_probably_holomorphic
+
 from .deprecation import (
     warn_deprecation,
     deprecated,
     deprecated_new_name,
     deprecate_dtype,
-    pure_callback,
 )
 
 from .model_frameworks import maybe_wrap_module
 
 from .history import History, accum_in_tree, accum_histories_in_tree
 
 from . import mpi
```

### Comparing `netket-3.8/netket/utils/_dependencies_check.py` & `netket-3.9/netket/utils/_dependencies_check.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 silently or unexpectedly.
 """
 
 from textwrap import dedent
 
 from .version_check import module_version, version_string
 
-# Check optax support for complex numbers.
-
 
 def create_msg(pkg_name, cur_version, desired_version, extra_msg=""):
     return dedent(
         f"""
 
         ##########################################################################################
 
@@ -46,14 +44,18 @@
 
         ##########################################################################################
 
         """
     )
 
 
+if not module_version("jax") >= (0, 4, 0):
+    cur_version = version_string("optax")
+    raise ImportError(create_msg("jax", cur_version, "0.4"))
+
 if not module_version("optax") >= (0, 1, 1):
     cur_version = version_string("optax")
     extra = """Reason: Optax is NetKet's provider of optimisers. Versions before 0.1.1 did not
                support complex numbers and silently returned wrong values, especially when
                using optimisers involving the norm of the gradient such as `Adam`.
                As recent versions of optax correctly work with complex numbers, please upgrade.
                """
```

### Comparing `netket-3.8/netket/utils/array.py` & `netket-3.9/netket/utils/array.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,31 +9,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import numpy as np
-
-from netket.utils import module_version
+import jax
 
 from .types import Array, DType, Shape
 from .struct import dataclass
 
-# TODO keep only  jax>=0.4 is required
-if module_version("jax") >= (0, 4, 0):
-    import jax
-
-    JaxArray = jax.Array
-else:
-    # pre jax 0.4
-    import jaxlib
-
-    JaxArray = jaxlib.xla_extension.DeviceArray
-
 
 @dataclass(cache_hash=True)
 class HashableArray:
     """
     This class wraps a numpy or jax array in order to make it hashable and
     equality comparable (which is necessary since a well-defined hashable object
     needs to satisfy :code:`obj1 == obj2` whenever :code:`hash(obj1) == hash(obj2)`.
@@ -44,15 +32,15 @@
     wrapped: Array
     """The wrapped array. Note that this array is read-only."""
 
     def __pre_init__(self, wrapped):
         if isinstance(wrapped, HashableArray):
             wrapped = wrapped.wrapped
         else:
-            if isinstance(wrapped, JaxArray):
+            if isinstance(wrapped, jax.Array):
                 # __array__ only works if it's a numpy array.
                 wrapped = np.array(wrapped)
             else:
                 wrapped = wrapped.copy()
             if isinstance(wrapped, np.ndarray):
                 wrapped.flags.writeable = False
```

### Comparing `netket-3.8/netket/utils/config_flags.py` & `netket-3.9/netket/utils/config_flags.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     val = os.getenv(varname, str(default))
     val = val.lower()
     if val in ("y", "yes", "t", "true", "on", "1"):
         return True
     elif val in ("n", "no", "f", "false", "off", "0"):
         return False
     else:
-        raise ValueError("invalid truth value %r for environment %r" % (val, varname))
+        raise ValueError(f"invalid truth value {val!r} for environment {varname!r}")
 
 
 def int_env(varname: str, default: int) -> int:
     """Read an environment variable and interpret it as an integer."""
     return int(os.getenv(varname, default))
```

### Comparing `netket-3.8/netket/utils/deprecation.py` & `netket-3.9/netket/utils/deprecation.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import warnings
 import functools
 import inspect
 
 from textwrap import dedent
 
 from .config_flags import config
-from .version_check import module_version
 
 
 def deprecated(reason=None, func_name=None):
     r"""
     This is a decorator which can be used to mark functions as deprecated. It
     will result in a warning being emitted when the function is used.
     """
@@ -53,24 +52,32 @@
     major release.
 
     :param message: A mandatory message documenting the deprecation.
     """
     warnings.warn(dedent(message), category=FutureWarning, stacklevel=2)
 
 
-def deprecated_new_name(message):
+def deprecated_new_name(func_name, reason=""):
     def deprecated_decorator(func):
         @functools.wraps(func)
         def deprecated_func(*args, **kwargs):
             warnings.warn(
-                (
-                    "{} has been renamed to {}. The old name is "
-                    "now deprecated and will be removed in the next minor version.\n"
-                    "Please update your code."
-                ).format(func.__name__, dedent(message)),
+                dedent(
+                    f"""
+
+    {func.__name__} has been renamed to {func_name}. The old name is
+    now deprecated and will be removed in the next minor version.
+
+    Please update your code by chaing occurences of `{func.__name__}` with
+    `{func_name}`.
+
+    {dedent(reason)}
+
+                    """
+                ),
                 category=FutureWarning,
                 stacklevel=2,
             )
             return func(*args, **kwargs)
 
         return deprecated_func
 
@@ -130,21 +137,7 @@
         if lazy:
             _clz = type(res)
             if not hasattr(_clz, "dtype"):
                 _clz.dtype = property(_dtype_deprecated)
         return res
 
     return helper
-
-
-# TODO: remove the switch when we support only jax >= 0.3.17
-
-
-def pure_callback(callback, result_shape_dtypes, *args):
-    if module_version("jax") >= (0, 3, 17):
-        from jax import pure_callback
-
-        return pure_callback(callback, result_shape_dtypes, *args)
-    else:
-        from jax.experimental.host_callback import call
-
-        return call(callback, *args, result_shape=result_shape_dtypes)
```

### Comparing `netket-3.8/netket/utils/dispatch.py` & `netket-3.9/netket/utils/dispatch.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/errors.py` & `netket-3.9/netket/utils/optional_deps.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,13 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+try:
+    import tensorboardX  # noqa
 
-class ComplexDomainError(Exception):
-    """
-    Error to be used when a complex value is used where a real value
-    was expected.
-    """
-
-    pass
+    tensorboard_available = True
+except ImportError:
+    tensorboard_available = False
```

### Comparing `netket-3.8/netket/utils/float.py` & `netket-3.9/netket/utils/float.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/history.py` & `netket-3.9/netket/utils/history.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/jax.py` & `netket-3.9/netket/utils/jax.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/moduletools.py` & `netket-3.9/netket/utils/moduletools.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/optional_deps.py` & `netket-3.9/netket/vqs/mc/mc_mixed_state/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,13 +8,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-try:
-    import tensorboardX  # noqa
+from .state import MCMixedState
 
-    tensorboard_available = True
-except ImportError:
-    tensorboard_available = False
+from . import expect
+
+from . import expect_chunked
```

### Comparing `netket-3.8/netket/utils/partial.py` & `netket-3.9/netket/utils/partial.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         while isinstance(
             func, partial if sys.version_info < (3, 10) else HashablePartial
         ):
             original_func = func
             func = original_func.func
             args = original_func.args + args
             keywords = {**original_func.keywords, **keywords}
-        return super(HashablePartial, cls).__new__(cls, func, *args, **keywords)
+        return super().__new__(cls, func, *args, **keywords)
 
     def __init__(self, *args, **kwargs):
         self._hash = None
 
     def __eq__(self, other):
         return (
             type(other) is HashablePartial
```

### Comparing `netket-3.8/netket/utils/seed.py` & `netket-3.9/netket/utils/seed.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/summation.py` & `netket-3.9/netket/utils/summation.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/types.py` & `netket-3.9/netket/utils/types.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,29 +12,24 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Any, Sequence, Callable, Union
 
 import optax as _optax
 import jax as _jax
-import jaxlib as _jaxlib
 import numpy as _np
 
 PRNGKeyT = Any
 SeedT = Union[int, PRNGKeyT]
 
 Shape = Sequence[int]
 DType = Any  # this could be a real type?
 
-if not hasattr(_jax, "Array"):
-    # pre jax 0.4
-    Array = Union[_np.ndarray, _jaxlib.xla_extension.DeviceArray, _jax.core.Tracer]
-else:
-    # TODO keep only this after jax>=0.4 is required
-    Array = Union[_np.ndarray, _jax.Array]
+Array = Union[_np.ndarray, _jax.Array]
+JaxArray = _jax.Array
 
 ArrayLike = Any  # Objects that are valid inputs to (np|jnp).asarray.
 
 NNInitFunc = Callable[[PRNGKeyT, Shape, DType], Array]
 
 PyTree = Any
```

### Comparing `netket-3.8/netket/utils/version_check.py` & `netket-3.9/netket/utils/version_check.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/group/__init__.py` & `netket-3.9/netket/utils/group/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/group/_group.py` & `netket-3.9/netket/utils/group/_group.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/group/_permutation_group.py` & `netket-3.9/netket/utils/group/_permutation_group.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/group/_point_group.py` & `netket-3.9/netket/utils/group/_point_group.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/group/_semigroup.py` & `netket-3.9/netket/utils/group/_semigroup.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/group/axial.py` & `netket-3.9/netket/utils/group/axial.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/group/cubic.py` & `netket-3.9/netket/utils/group/cubic.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/group/icosa.py` & `netket-3.9/netket/utils/group/icosa.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/group/planar.py` & `netket-3.9/netket/utils/group/planar.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/model_frameworks/__init__.py` & `netket-3.9/netket/utils/model_frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/model_frameworks/base.py` & `netket-3.9/netket/utils/model_frameworks/base.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/model_frameworks/flax.py` & `netket-3.9/netket/utils/model_frameworks/flax.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/model_frameworks/haiku.py` & `netket-3.9/netket/utils/model_frameworks/haiku.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/model_frameworks/jax.py` & `netket-3.9/netket/utils/model_frameworks/jax.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/mpi/__init__.py` & `netket-3.9/netket/utils/mpi/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/mpi/mpi.py` & `netket-3.9/netket/utils/mpi/mpi.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/mpi/primitives.py` & `netket-3.9/netket/utils/mpi/primitives.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/struct/__init__.py` & `netket-3.9/netket/callbacks/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,10 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# flake8: noqa: F401
+from .earlystopping import EarlyStopping
+from .timeout import Timeout
+from .invalidlossstopping import InvalidLossStopping
+from .convergence_stopping import ConvergenceStopping
 
-from .dataclass import dataclass, field, property_cached, Uninitialized
+from netket.utils import _hide_submodules
+
+_hide_submodules(__name__)
```

### Comparing `netket-3.8/netket/utils/struct/dataclass.py` & `netket-3.9/netket/utils/struct/dataclass.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/utils/struct/utils.py` & `netket-3.9/netket/utils/struct/utils.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/vqs/__init__.py` & `netket-3.9/netket/vqs/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,16 +17,19 @@
     VariationalMixedState,
     expect,
     expect_and_grad,
     expect_and_forces,
 )
 
 from .mc import MCState, MCMixedState, get_local_kernel_arguments, get_local_kernel
-from .exact import ExactState
+from .full_summ import FullSumState
 
 # TODO: this is deprecated in favour of netket.experimental.vqs
 # eventually remove this file and import
 from . import experimental
 
+# TODO: deprecated on May 2023
+from .deprecated import ExactState
+
 from netket.utils import _hide_submodules
 
 _hide_submodules(__name__, ignore=["experimental"], hide_folder=["mc"])
```

### Comparing `netket-3.8/netket/vqs/base.py` & `netket-3.9/netket/vqs/base.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/vqs/experimental.py` & `netket-3.9/netket/vqs/experimental.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/vqs/exact/__init__.py` & `netket-3.9/netket/vqs/full_summ/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .state import ExactState
+from .state import FullSumState
 
 from . import expect
 
 from .expect import expect_and_grad
```

### Comparing `netket-3.8/netket/vqs/exact/expect.py` & `netket-3.9/netket/vqs/full_summ/expect.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from netket.stats import Stats
 from netket.utils.types import PyTree
 from netket.utils.dispatch import dispatch, TrueT
 
 from netket.operator import DiscreteOperator
 
 
-from .state import ExactState
+from .state import FullSumState
 
 
 def _check_hilbert(A, B):
     if A.hilbert != B.hilbert:
         raise NotImplementedError(  # pragma: no cover
             f"Non matching hilbert spaces {A.hilbert} and {B.hilbert}"
         )
@@ -45,15 +45,15 @@
     """
     Converts to sparse but also cache the sparsificated result to speed up.
     """
     return Ô.to_sparse()
 
 
 @dispatch
-def expect(vstate: ExactState, Ô: DiscreteOperator) -> Stats:  # noqa: F811
+def expect(vstate: FullSumState, Ô: DiscreteOperator) -> Stats:  # noqa: F811
     _check_hilbert(vstate, Ô)
 
     O = sparsify(Ô)
     Ψ = vstate.to_array()
 
     # TODO: This performs the full computation on all MPI ranks.
     # It would be great if we could split the computation among ranks.
@@ -63,15 +63,15 @@
 
     variance = jnp.sum(jnp.abs(OΨ - expval_O * Ψ) ** 2)
     return Stats(mean=expval_O, error_of_mean=0.0, variance=variance)
 
 
 @dispatch
 def expect_and_forces(
-    vstate: ExactState,
+    vstate: FullSumState,
     Ô: DiscreteOperator,
     *,
     mutable: CollectionFilter,
 ) -> Tuple[Stats, PyTree]:
     if isinstance(Ô, Squared):
         raise NotImplementedError("expect_and_forces not yet implemented for `Squared`")
 
@@ -130,15 +130,15 @@
         Ō_grad,
         new_model_state,
     )
 
 
 @dispatch
 def expect_and_grad(
-    vstate: ExactState,
+    vstate: FullSumState,
     Ô: DiscreteOperator,
     use_covariance: TrueT,
     *,
     mutable: CollectionFilter,
 ) -> Tuple[Stats, PyTree]:
     Ō, Ō_grad = expect_and_forces(vstate, Ô, mutable=mutable)
     Ō_grad = _force_to_grad(Ō_grad, vstate.parameters)
```

### Comparing `netket-3.8/netket/vqs/exact/state.py` & `netket-3.9/netket/vqs/full_summ/state.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     Args:
         fun: the hashable callable to be evaluated.
         args: the arguments to the function.
     """
     return fun(*args)
 
 
-class ExactState(VariationalState):
+class FullSumState(VariationalState):
     """Variational State for a variational quantum state computed on the whole
     Hilbert space without Monte Carlo sampling.
 
     Expectation values and gradients are deterministic.
     The only non-deterministic part is due to the initialization seed used to generate
     the parameters.
     """
@@ -77,23 +77,23 @@
         apply_fun: Callable = None,
         seed: Optional[SeedT] = None,
         mutable: CollectionFilter = False,
         training_kwargs: Dict = {},
         dtype=float,
     ):
         """
-        Constructs the ExactState.
+        Constructs the FullSumState.
 
         Args:
             hilbert: The Hilbert space
             model: (Optional) The model. If not provided, you must provide init_fun and apply_fun.
             parameters: Optional PyTree of weights from which to start.
             seed: rng seed used to generate a set of parameters (only if parameters is not passed). Defaults to a random one.
             mutable: Name or list of names of mutable arguments. Use it to specify if the model has a state that can change
-                during evaluation, but that should not be optimised. See also flax.linen.module.apply documentation
+                during evaluation, but that should not be optimised. See also :meth:`flax.linen.Module.apply` documentation
                 (default=False)
             init_fun: Function of the signature f(model, shape, rng_key, dtype) -> Optional_state, parameters used to
                 initialise the parameters. Defaults to the standard flax initialiser. Only specify if your network has
                 a non-standard init method.
             variables: Optional initial value for the variables (parameters and model state) of the model.
             apply_fun: Function of the signature f(model, variables, σ) that should evaluate the model. Defaults to
                 `model.apply(variables, σ)`. specify only if your network has a non-standard apply method.
@@ -311,43 +311,43 @@
     def _all_states(self):
         if self._states is None:
             self._states = self.hilbert.all_states()
         return self._states
 
     def __repr__(self):
         return (
-            "ExactState("
-            + "\n  hilbert = {},".format(self.hilbert)
-            + "\n  n_parameters = {})".format(self.n_parameters)
+            "FullSumState("
+            + f"\n  hilbert = {self.hilbert},"
+            + f"\n  n_parameters = {self.n_parameters})"
         )
 
     def __str__(self):
-        return "ExactState(" + "hilbert = {}, ".format(self.hilbert)
+        return "FullSumState(" + f"hilbert = {self.hilbert}, "
 
 
 # serialization
 
 
-def serialize_ExactState(vstate):
+def serialize_FullSumState(vstate):
     state_dict = {
         "variables": serialization.to_state_dict(vstate.variables),
     }
     return state_dict
 
 
-def deserialize_ExactState(vstate, state_dict):
+def deserialize_FullSumState(vstate, state_dict):
     import copy
 
     new_vstate = copy.copy(vstate)
     new_vstate.reset()
 
     new_vstate.variables = serialization.from_state_dict(
         vstate.variables, state_dict["variables"]
     )
     return new_vstate
 
 
 serialization.register_serialization_state(
-    ExactState,
-    serialize_ExactState,
-    deserialize_ExactState,
+    FullSumState,
+    serialize_FullSumState,
+    deserialize_FullSumState,
 )
```

### Comparing `netket-3.8/netket/vqs/mc/__init__.py` & `netket-3.9/netket/vqs/mc/__init__.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/vqs/mc/common.py` & `netket-3.9/netket/vqs/mc/common.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/vqs/mc/kernels.py` & `netket-3.9/netket/vqs/mc/kernels.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from functools import partial
 
 import jax
 import jax.numpy as jnp
 
 from netket.utils.types import PyTree, Array
 import netket.jax as nkjax
+from netket.operator import DiscreteJaxOperator
 
 
 def batch_discrete_kernel(kernel):
     """
     Batch a kernel that only works with 1 sample so that it works with a
     batch of samples.
 
@@ -55,14 +56,26 @@
     """
     local_value kernel for MCState and generic operators
     """
     σp, mel = args
     return jnp.sum(mel * jnp.exp(logpsi(pars, σp) - logpsi(pars, σ)))
 
 
+def local_value_kernel_jax(
+    logpsi: Callable, pars: PyTree, σ: Array, O: DiscreteJaxOperator
+):
+    """
+    local_value kernel for MCState for jax-compatible operators
+    """
+    σp, mel = O.get_conn_padded(σ)
+    logpsi_σ = logpsi(pars, σ)
+    logpsi_σp = logpsi(pars, σp)
+    return jnp.sum(mel * jnp.exp(logpsi_σp - jnp.expand_dims(logpsi_σ, -1)), axis=-1)
+
+
 def local_value_squared_kernel(logpsi: Callable, pars: PyTree, σ: Array, args: PyTree):
     """
     local_value kernel for MCState and Squared (generic) operators
     """
     return jnp.abs(local_value_kernel(logpsi, pars, σ, args)) ** 2
 
 
@@ -153,7 +166,27 @@
         out_axes=0,
     )(σp, σ)
     σ_σ = jax.vmap(lambda σi: jnp.hstack((σi, σi)), in_axes=0)(σ)
 
     return local_value_kernel_chunked(
         logpsi, pars, σ_σ, (σ_σp, mels), chunk_size=chunk_size
     )
+
+
+def local_value_kernel_jax_chunked(
+    logpsi: Callable,
+    pars: PyTree,
+    σ: Array,
+    O: DiscreteJaxOperator,
+    *,
+    chunk_size: Optional[int] = None,
+):
+    """
+    local_value kernel for MCState and jaxcoompatible operators
+    """
+    local_value_kernel = lambda s: local_value_kernel_jax(logpsi, pars, s, O)
+
+    local_value_chunked = nkjax.vmap_chunked(
+        local_value_kernel, in_axes=0, chunk_size=chunk_size
+    )
+
+    return local_value_chunked(σ)
```

### Comparing `netket-3.8/netket/vqs/mc/mc_mixed_state/__init__.py` & `netket-3.9/netket/vqs/mc/mc_state/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,12 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .state import MCMixedState
+from .state import MCState
 
 from . import expect
+from . import expect_grad
+from . import expect_forces
 
 from . import expect_chunked
+from . import expect_grad_chunked
+from . import expect_forces_chunked
```

### Comparing `netket-3.8/netket/vqs/mc/mc_mixed_state/expect.py` & `netket-3.9/netket/vqs/mc/mc_mixed_state/expect.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/vqs/mc/mc_mixed_state/expect_chunked.py` & `netket-3.9/netket/vqs/mc/mc_mixed_state/expect_chunked.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/vqs/mc/mc_mixed_state/expect_grad_chunked.py` & `netket-3.9/netket/vqs/mc/mc_mixed_state/expect_grad_chunked.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/vqs/mc/mc_mixed_state/state.py` & `netket-3.9/netket/vqs/mc/mc_mixed_state/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -214,32 +214,32 @@
         return netket.nn.to_matrix(
             self.hilbert, self._apply_fun, self.variables, normalize=normalize
         )
 
     def __repr__(self):
         return (
             "MCMixedState("
-            + "\n  hilbert = {},".format(self.hilbert)
-            + "\n  sampler = {},".format(self.sampler)
-            + "\n  n_samples = {},".format(self.n_samples)
-            + "\n  n_discard_per_chain = {},".format(self.n_discard_per_chain)
-            + "\n  sampler_state = {},".format(self.sampler_state)
-            + "\n  sampler_diag = {},".format(self.sampler_diag)
-            + "\n  n_samples_diag = {},".format(self.n_samples_diag)
-            + "\n  n_discard_per_chain_diag = {},".format(self.n_discard_per_chain_diag)
-            + "\n  sampler_state_diag = {},".format(self.diagonal.sampler_state)
-            + "\n  n_parameters = {})".format(self.n_parameters)
+            + f"\n  hilbert = {self.hilbert},"
+            + f"\n  sampler = {self.sampler},"
+            + f"\n  n_samples = {self.n_samples},"
+            + f"\n  n_discard_per_chain = {self.n_discard_per_chain},"
+            + f"\n  sampler_state = {self.sampler_state},"
+            + f"\n  sampler_diag = {self.sampler_diag},"
+            + f"\n  n_samples_diag = {self.n_samples_diag},"
+            + f"\n  n_discard_per_chain_diag = {self.n_discard_per_chain_diag},"
+            + f"\n  sampler_state_diag = {self.diagonal.sampler_state},"
+            + f"\n  n_parameters = {self.n_parameters})"
         )
 
     def __str__(self):
         return (
             "MCMixedState("
-            + "hilbert = {}, ".format(self.hilbert)
-            + "sampler = {}, ".format(self.sampler)
-            + "n_samples = {})".format(self.n_samples)
+            + f"hilbert = {self.hilbert}, "
+            + f"sampler = {self.sampler}, "
+            + f"n_samples = {self.n_samples})"
         )
 
 
 # serialization
 
 
 def serialize_MCMixedState(vstate):
```

### Comparing `netket-3.8/netket/vqs/mc/mc_state/__init__.py` & `netket-3.9/netket/operator/_pauli_strings/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,17 @@
-# Copyright 2021 The NetKet Authors - All rights reserved.
+# Copyright 2023 The NetKet Authors - All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .state import MCState
-
-from . import expect
-from . import expect_grad
-from . import expect_forces
-
-from . import expect_chunked
-from . import expect_grad_chunked
-from . import expect_forces_chunked
+from .base import PauliStringsBase
+from .numba import PauliStrings
+from .jax import PauliStringsJax
```

### Comparing `netket-3.8/netket/vqs/mc/mc_state/expect.py` & `netket-3.9/netket/vqs/mc/mc_state/expect.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from netket.utils.dispatch import dispatch
 
 from netket.operator import (
     AbstractOperator,
     DiscreteOperator,
     Squared,
     ContinuousOperator,
+    DiscreteJaxOperator,
 )
 
 from netket.vqs.mc import (
     kernels,
     check_hilbert,
     get_local_kernel_arguments,
     get_local_kernel,
@@ -64,14 +65,27 @@
 
 @dispatch
 def get_local_kernel(vstate: MCState, Ô: DiscreteOperator):  # noqa: F811
     return kernels.local_value_kernel
 
 
 @dispatch
+def get_local_kernel_arguments(vstate: MCState, Ô: DiscreteJaxOperator):  # noqa: F811
+    check_hilbert(vstate.hilbert, Ô.hilbert)
+
+    σ = vstate.samples
+    return σ, Ô
+
+
+@dispatch
+def get_local_kernel(vstate: MCState, Ô: DiscreteJaxOperator):  # noqa: F811
+    return kernels.local_value_kernel_jax
+
+
+@dispatch
 def get_local_kernel_arguments(vstate: MCState, Ô: ContinuousOperator):  # noqa: F811
     check_hilbert(vstate.hilbert, Ô.hilbert)
 
     σ = vstate.samples
     args = Ô._pack_arguments()
     return σ, args
 
@@ -110,18 +124,18 @@
     model_apply_fun: Callable,
     machine_pow: int,
     parameters: PyTree,
     model_state: PyTree,
     σ: jnp.ndarray,
     local_value_args: PyTree,
 ) -> Stats:
-    σ_shape = σ.shape
 
-    if jnp.ndim(σ) != 2:
-        σ = σ.reshape((-1, σ_shape[-1]))
+    n_chains = σ.shape[0]
+    if σ.ndim >= 3:
+        σ = jax.lax.collapse(σ, 0, 2)
 
     def logpsi(w, σ):
         return model_apply_fun({"params": w, **model_state}, σ)
 
     def log_pdf(w, σ):
         return machine_pow * model_apply_fun({"params": w, **model_state}, σ).real
 
@@ -129,15 +143,14 @@
     # should uncomment and remove code below once this is fixed
     # _, Ō_stats = nkjax.expect(
     #    log_pdf,
     #    partial(local_value_kernel, logpsi),
     #    parameters,
     #    σ,
     #    local_value_args,
-    #    n_chains=σ_shape[0],
+    #    n_chains=n_chains,
     # )
 
     L_σ = local_value_kernel(logpsi, parameters, σ, local_value_args)
-    L_σ = L_σ.reshape((σ_shape[0], -1))
-    Ō_stats = mpi_statistics(L_σ.T)
+    Ō_stats = mpi_statistics(L_σ.reshape((n_chains, -1)))
 
     return Ō_stats
```

### Comparing `netket-3.8/netket/vqs/mc/mc_state/expect_chunked.py` & `netket-3.9/netket/vqs/mc/mc_state/expect_chunked.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from netket.stats import Stats
 from netket.utils.types import PyTree
 from netket.utils.dispatch import dispatch
 
 from netket.operator import (
     AbstractOperator,
     DiscreteOperator,
+    DiscreteJaxOperator,
     ContinuousOperator,
     Squared,
 )
 
 from netket.vqs import expect
 
 from netket.vqs.mc import (
@@ -46,14 +47,21 @@
 @dispatch
 def get_local_kernel(vstate: MCState, Ô: Squared, chunk_size: int):  # noqa: F811
     return kernels.local_value_squared_kernel_chunked
 
 
 @dispatch
 def get_local_kernel(  # noqa: F811
+    vstate: MCState, Ô: DiscreteJaxOperator, chunk_size: int
+):  # noqa: F811
+    return kernels.local_value_kernel_jax_chunked
+
+
+@dispatch
+def get_local_kernel(  # noqa: F811
     vstate: MCState, Ô: DiscreteOperator, chunk_size: int
 ):
     return kernels.local_value_kernel_chunked
 
 
 def _local_continuous_kernel(kernel, logpsi, pars, σ, args, *, chunk_size=None):
     def _kernel(σ):
```

### Comparing `netket-3.8/netket/vqs/mc/mc_state/expect_forces.py` & `netket-3.9/netket/vqs/mc/mc_state/expect_forces.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,28 +71,28 @@
     mutable: CollectionFilter,
     parameters: PyTree,
     model_state: PyTree,
     σ: jnp.ndarray,
     local_value_args: PyTree,
 ) -> Tuple[PyTree, PyTree]:
 
-    σ_shape = σ.shape
-    if jnp.ndim(σ) != 2:
-        σ = σ.reshape((-1, σ_shape[-1]))
+    n_chains = σ.shape[0]
+    if σ.ndim >= 3:
+        σ = jax.lax.collapse(σ, 0, 2)
 
     n_samples = σ.shape[0] * mpi.n_nodes
 
     O_loc = local_value_kernel(
         model_apply_fun,
         {"params": parameters, **model_state},
         σ,
         local_value_args,
     )
 
-    Ō = statistics(O_loc.reshape(σ_shape[:-1]).T)
+    Ō = statistics(O_loc.reshape((n_chains, -1)))
 
     O_loc -= Ō.mean
 
     # Then compute the vjp.
     # Code is a bit more complex than a standard one because we support
     # mutable state (if it's there)
     is_mutable = mutable is not False
```

### Comparing `netket-3.8/netket/vqs/mc/mc_state/expect_forces_chunked.py` & `netket-3.9/netket/vqs/mc/mc_state/expect_forces_chunked.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,16 @@
     chunk_size: Any,
     *args,
     **kwargs,
 ):
     warnings.warn(
         f"Ignoring chunk_size={chunk_size} for expect_and_forces method with signature "
         f"({type(vstate)}, {type(operator)}) because no implementation supporting "
-        f"chunking for this signature exists."
+        f"chunking for this signature exists.",
+        stacklevel=2,
     )
 
     return expect_and_forces(vstate, operator, *args, **kwargs)
 
 
 @expect_and_forces.dispatch
 def expect_and_forces_impl(  # noqa: F811
```

### Comparing `netket-3.8/netket/vqs/mc/mc_state/expect_grad.py` & `netket-3.9/netket/vqs/mc/mc_state/expect_grad.py`

 * *Files 3% similar despite different names*

```diff
@@ -132,17 +132,17 @@
     mutable: CollectionFilter,
     parameters: PyTree,
     model_state: PyTree,
     σ: jnp.ndarray,
     local_value_args: PyTree,
 ) -> Tuple[PyTree, PyTree, Stats]:
 
-    σ_shape = σ.shape
-    if jnp.ndim(σ) != 2:
-        σ = σ.reshape((-1, σ_shape[-1]))
+    n_chains = σ.shape[0]
+    if σ.ndim >= 3:
+        σ = jax.lax.collapse(σ, 0, 2)
 
     is_mutable = mutable is not False
     logpsi = lambda w, σ: model_apply_fun(
         {"params": w, **model_state}, σ, mutable=mutable
     )
     log_pdf = (
         lambda w, σ: machine_pow * model_apply_fun({"params": w, **model_state}, σ).real
@@ -151,15 +151,15 @@
     def expect_closure_pars(pars):
         return nkjax.expect(
             log_pdf,
             partial(local_value_kernel, logpsi),
             pars,
             σ,
             local_value_args,
-            n_chains=σ_shape[0],
+            n_chains=n_chains,
         )
 
     Ō, Ō_pb, Ō_stats = nkjax.vjp(
         expect_closure_pars, parameters, has_aux=True, conjugate=True
     )
     Ō_pars_grad = Ō_pb(jnp.ones_like(Ō))[0]
```

### Comparing `netket-3.8/netket/vqs/mc/mc_state/expect_grad_chunked.py` & `netket-3.9/netket/vqs/mc/mc_state/expect_grad_chunked.py`

 * *Files identical despite different names*

### Comparing `netket-3.8/netket/vqs/mc/mc_state/state.py` & `netket-3.9/netket/vqs/mc/mc_state/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,27 +42,29 @@
 
 from netket.vqs.base import VariationalState, expect, expect_and_grad, expect_and_forces
 from netket.vqs.mc import get_local_kernel, get_local_kernel_arguments
 
 
 def compute_chain_length(n_chains, n_samples):
     if n_samples <= 0:
-        raise ValueError("Invalid number of samples: n_samples={}".format(n_samples))
+        raise ValueError(f"Invalid number of samples: n_samples={n_samples}")
 
     chain_length = int(np.ceil(n_samples / n_chains))
 
     n_samples_new = chain_length * n_chains
     n_samples_per_rank_new = n_samples_new // mpi.n_nodes
 
     if n_samples_new != n_samples:
         n_samples_per_rank = n_samples // mpi.n_nodes
         warnings.warn(
             f"n_samples={n_samples} ({n_samples_per_rank} per MPI rank) does not "
             f"divide n_chains={n_chains}, increased to {n_samples_new} "
-            f"({n_samples_per_rank_new} per MPI rank)"
+            f"({n_samples_per_rank_new} per MPI rank)",
+            UserWarning,
+            stacklevel=3,
         )
 
     return chain_length
 
 
 def check_chunk_size(n_samples, chunk_size):
     n_samples_per_rank = n_samples // mpi.n_nodes
@@ -159,15 +161,15 @@
                 specified together with n_samples (default=None).
             n_discard_per_chain: number of discarded samples at the beginning of each monte-carlo chain (default=0 for exact sampler,
                 and n_samples/10 for approximate sampler).
             parameters: Optional PyTree of weights from which to start.
             seed: rng seed used to generate a set of parameters (only if parameters is not passed). Defaults to a random one.
             sampler_seed: rng seed used to initialise the sampler. Defaults to a random one.
             mutable: Name or list of names of mutable arguments. Use it to specify if the model has a state that can change
-                during evaluation, but that should not be optimised. See also flax.linen.module.apply documentation
+                during evaluation, but that should not be optimised. See also :meth:`flax.linen.Module.apply` documentation
                 (default=False)
             init_fun: Function of the signature f(model, shape, rng_key, dtype) -> Optional_state, parameters used to
                 initialise the parameters. Defaults to the standard flax initialiser. Only specify if your network has
                 a non-standard init method.
             variables: Optional initial value for the variables (parameters and model state) of the model.
             apply_fun: Function of the signature f(model, variables, σ) that should evaluate the model. Defaults to
                 `model.apply(variables, σ)`. specify only if your network has a non-standard apply method.
@@ -376,15 +378,16 @@
                 )
             )
 
         # don't discard if the sampler is exact
         if self.sampler.is_exact:
             if n_discard_per_chain is not None and n_discard_per_chain > 0:
                 warnings.warn(
-                    "An exact sampler does not need to discard samples. Setting n_discard_per_chain to 0."
+                    "An exact sampler does not need to discard samples. Setting n_discard_per_chain to 0.",
+                    stacklevel=2,
                 )
             n_discard_per_chain = 0
 
         self._n_discard_per_chain = (
             int(n_discard_per_chain)
             if n_discard_per_chain is not None
             else self.n_samples // 10
@@ -421,15 +424,16 @@
             return
 
         if chunk_size <= 0:
             raise ValueError("Chunk size must be a positive integer. ")
 
         if not _is_power_of_two(chunk_size):
             warnings.warn(
-                "For performance reasons, we suggest to use a power-of-two chunk size."
+                "For performance reasons, we suggest to use a power-of-two chunk size.",
+                stacklevel=2,
             )
 
         check_chunk_size(self.n_samples, chunk_size)
 
         self._chunk_size = chunk_size
 
     def reset(self):
@@ -631,15 +635,15 @@
 
         if mutable is None:
             mutable = self.mutable
 
         return expect_and_forces(self, Ô, self.chunk_size, mutable=mutable)
 
     def quantum_geometric_tensor(
-        self, qgt_T: LinearOperator = QGTAuto()
+        self, qgt_T: LinearOperator = QGTAuto
     ) -> LinearOperator:
         r"""Computes an estimate of the quantum geometric tensor G_ij.
         This function returns a linear operator that can be used to apply G_ij to a given vector
         or can be converted to a full matrix.
 
         Args:
             qgt_T: the optional type of the quantum geometric tensor. By default it's automatically selected.
@@ -659,38 +663,36 @@
             normalize=normalize,
             chunk_size=self.chunk_size,
         )
 
     def __repr__(self):
         return (
             "MCState("
-            + "\n  hilbert = {},".format(self.hilbert)
-            + "\n  sampler = {},".format(self.sampler)
-            + "\n  n_samples = {},".format(self.n_samples)
-            + "\n  n_discard_per_chain = {},".format(self.n_discard_per_chain)
-            + "\n  sampler_state = {},".format(self.sampler_state)
-            + "\n  n_parameters = {})".format(self.n_parameters)
+            + f"\n  hilbert = {self.hilbert},"
+            + f"\n  sampler = {self.sampler},"
+            + f"\n  n_samples = {self.n_samples},"
+            + f"\n  n_discard_per_chain = {self.n_discard_per_chain},"
+            + f"\n  sampler_state = {self.sampler_state},"
+            + f"\n  n_parameters = {self.n_parameters})"
         )
 
     def __str__(self):
         return (
             "MCState("
-            + "hilbert = {}, ".format(self.hilbert)
-            + "sampler = {}, ".format(self.sampler)
-            + "n_samples = {})".format(self.n_samples)
+            + f"hilbert = {self.hilbert}, "
+            + f"sampler = {self.sampler}, "
+            + f"n_samples = {self.n_samples})"
         )
 
 
 @partial(jax.jit, static_argnames=("kernel", "apply_fun", "shape"))
 def _local_estimators_kernel(kernel, apply_fun, shape, variables, samples, extra_args):
     O_loc = kernel(apply_fun, variables, samples, extra_args)
 
-    # transpose O_loc so it matches the (n_chains, n_samples_per_chain) shape
-    # expected by netket.stats.statistics.
-    return O_loc.reshape(shape).T
+    return O_loc.reshape(shape)
 
 
 def local_estimators(
     state: MCState, op: AbstractOperator, *, chunk_size: Optional[int]
 ):
     s, extra_args = get_local_kernel_arguments(state, op)
```

### Comparing `netket-3.8/.gitignore` & `netket-3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `netket-3.8/LICENSE` & `netket-3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `netket-3.8/README.md` & `netket-3.9/README.md`

 * *Files identical despite different names*

### Comparing `netket-3.8/pyproject.toml` & `netket-3.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -25,33 +25,33 @@
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: POSIX :: Linux",
     "Operating System :: Unix",
     "Topic :: Scientific/Engineering :: Physics",
 ]
 dynamic = ["version"]
 
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dependencies = [
     "numpy~=1.20",
     "scipy>=1.5.3, <2",
     "tqdm>=4.60, <5",
     "plum-dispatch>=1.5.1, <3",
     "numba>=0.52, <0.58",
-    "igraph>=0.9.8, <0.11.0",
-    "jax>=0.3.16, <0.5",
-    "jaxlib>=0.3.15, <0.5",
-    "flax>=0.6, <0.7",
+    "igraph>=0.10.0, <0.11.0",
+    "jax>=0.4.3, <0.5",
+    "jaxlib>=0.4.3, <0.5",
+    "flax>=0.6.5, <0.8",
     "orjson>=3.4, <4",
     "optax>=0.1.3, <0.2",
-    "numba4jax>=0.0.10, <0.1",
+    "numba4jax>=0.0.10.post1, <0.1",
 ]
 
 [project.optional-dependencies]
 mpi = [
-    "mpi4py>=3.0.1, <4", 
+    "mpi4py>=3.0.1, <4",
     "mpi4jax>=0.3.9, <0.4"
     ]
 extra = [
     "tensorboardx>=2.0.0",
     "openfermion>=1.0.0",
     "h5py>=3.7.0",
     ]
@@ -61,26 +61,25 @@
     "pytest>=6",
     "pytest-xdist[psutil]>=2",
     "pytest-cov>=2.10.1",
     "pytest-json-report>=1.3",
     "coverage>=5",
     "pre-commit>=2.7",
     "black==22.10.0",
-    "flake8==6.0.0; python_version >= '3.8'",
-    "flake8==5.0.4; python_version < '3.8'",
+    "ruff==0.0.278",
     "wheel",
     "build",
 ]
 docs = [
     "Sphinx>=5.3,<7.1",
     "sphinx-autodoc-typehints~=1.22",
     "sphinxcontrib-fulltoc~=1.2.0",
     "sphinxcontrib-jsmath~=1.0.1",
     "sphinxcontrib-napoleon==0.7",
-    "myst-parser~=0.18.1",
+    "myst-parser>=0.18.1,<2.1.0",
     "nbsphinx~=0.9.1",
     "myst-nb~=0.17.1",
     "sphinx-book-theme~=1.0.1",
 ]
 
 [project.urls]
  homepage = "https://www.netket.org"
@@ -136,7 +135,21 @@
     "ignore:`np.long`",
     "ignore:`np.int` is a deprecated alias for the builtin `int`",
     "ignore::DeprecationWarning:tensorboardX",
 ]
 testpaths = [
     "test",
 ]
+
+[tool.ruff]
+target-version = "py38"
+select = ["E", "F", "W"]
+fixable = ["E", "F", "W"]
+ignore = ["E501", "E731", "E741"]
+#ignore = ["E266"]
+line-length = 88
+exclude = ["Examples/Legacy"]
+
+[tool.ruff.per-file-ignores]
+"__init__.py" = ["E402","F401"]
+"netket/nn/activation.py" = ["F401"]
+"Examples/" = ["F401"]
```

### Comparing `netket-3.8/PKG-INFO` & `netket-3.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NetKet
-Version: 3.8
+Version: 3.9
 Summary: Netket : Machine Learning toolbox for many-body quantum systems.
 Project-URL: homepage, https://www.netket.org
 Project-URL: documentation, https://netket.readthedocs.io/en/latest/#
 Project-URL: repository, https://github.com/netket/netket
 Project-URL: changelog, https://netket.readthedocs.io/en/latest/docs/changelog.html
 Author: Giuseppe Carleo, Filippo Vicentini, The NetKet authors
 License: Apache 2.0
@@ -13,44 +13,43 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.7
-Requires-Dist: flax<0.7,>=0.6
-Requires-Dist: igraph<0.11.0,>=0.9.8
-Requires-Dist: jax<0.5,>=0.3.16
-Requires-Dist: jaxlib<0.5,>=0.3.15
-Requires-Dist: numba4jax<0.1,>=0.0.10
+Requires-Python: >=3.8
+Requires-Dist: flax<0.8,>=0.6.5
+Requires-Dist: igraph<0.11.0,>=0.10.0
+Requires-Dist: jax<0.5,>=0.4.3
+Requires-Dist: jaxlib<0.5,>=0.4.3
+Requires-Dist: numba4jax<0.1,>=0.0.10.post1
 Requires-Dist: numba<0.58,>=0.52
 Requires-Dist: numpy~=1.20
 Requires-Dist: optax<0.2,>=0.1.3
 Requires-Dist: orjson<4,>=3.4
 Requires-Dist: plum-dispatch<3,>=1.5.1
 Requires-Dist: scipy<2,>=1.5.3
 Requires-Dist: tqdm<5,>=4.60
 Provides-Extra: dev
 Requires-Dist: black==22.10.0; extra == 'dev'
 Requires-Dist: build; extra == 'dev'
 Requires-Dist: coverage>=5; extra == 'dev'
-Requires-Dist: flake8==5.0.4; python_version < '3.8' and extra == 'dev'
-Requires-Dist: flake8==6.0.0; python_version >= '3.8' and extra == 'dev'
 Requires-Dist: matplotlib>=3; extra == 'dev'
 Requires-Dist: networkx<4,>=2.4; extra == 'dev'
 Requires-Dist: pre-commit>=2.7; extra == 'dev'
 Requires-Dist: pytest-cov>=2.10.1; extra == 'dev'
 Requires-Dist: pytest-json-report>=1.3; extra == 'dev'
 Requires-Dist: pytest-xdist[psutil]>=2; extra == 'dev'
 Requires-Dist: pytest>=6; extra == 'dev'
+Requires-Dist: ruff==0.0.278; extra == 'dev'
 Requires-Dist: wheel; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: myst-nb~=0.17.1; extra == 'docs'
-Requires-Dist: myst-parser~=0.18.1; extra == 'docs'
+Requires-Dist: myst-parser<2.1.0,>=0.18.1; extra == 'docs'
 Requires-Dist: nbsphinx~=0.9.1; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints~=1.22; extra == 'docs'
 Requires-Dist: sphinx-book-theme~=1.0.1; extra == 'docs'
 Requires-Dist: sphinx<7.1,>=5.3; extra == 'docs'
 Requires-Dist: sphinxcontrib-fulltoc~=1.2.0; extra == 'docs'
 Requires-Dist: sphinxcontrib-jsmath~=1.0.1; extra == 'docs'
 Requires-Dist: sphinxcontrib-napoleon==0.7; extra == 'docs'
```


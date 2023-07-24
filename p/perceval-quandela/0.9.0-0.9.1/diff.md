# Comparing `tmp/perceval-quandela-0.9.0.tar.gz` & `tmp/perceval-quandela-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perceval-quandela-0.9.0.tar", last modified: Mon Jul 10 10:16:34 2023, max compression
+gzip compressed data, was "perceval-quandela-0.9.1.tar", last modified: Mon Jul 24 12:30:08 2023, max compression
```

## Comparing `perceval-quandela-0.9.0.tar` & `perceval-quandela-0.9.1.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.668261 perceval-quandela-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-07-10 10:16:34.668261 perceval-quandela-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.660261 perceval-quandela-0.9.0/perceval/
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.660261 perceval-quandela-0.9.0/perceval/algorithm/
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/algorithm/abstract_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/algorithm/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/algorithm/qrng.py
--rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/algorithm/sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.660261 perceval-quandela-0.9.0/perceval/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/backends/_abstract_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/backends/_clifford2017.py
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/backends/_mps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/backends/_naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/backends/_slos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.660261 perceval-quandela-0.9.0/perceval/components/
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/_mode_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/abstract_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    21723 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/abstract_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/component_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.660261 perceval-quandela-0.9.0/perceval/components/core_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/core_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/core_catalog/generic_2mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/core_catalog/heralded_cnot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/core_catalog/heralded_cz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/core_catalog/postprocessed_cnot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/detector.py
--rw-r--r--   0 runner    (1001) docker     (123)    35994 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/linear_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/non_unitary_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/port.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/predefined_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12442 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/source.py
--rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/components/unitary_components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.660261 perceval-quandela-0.9.0/perceval/converters/
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/converters/converter_statevector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/converters/qiskit_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.664261 perceval-quandela-0.9.0/perceval/rendering/
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/_mplot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/_processor_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.664261 perceval-quandela-0.9.0/perceval/rendering/canvas/
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/canvas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/canvas/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/canvas/latex_canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/canvas/mplot_canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/canvas/svg_canvas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.664261 perceval-quandela-0.9.0/perceval/rendering/circuit/
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/circuit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/circuit/abstract_skin.py
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/circuit/phys_skin.py
--rw-r--r--   0 runner    (1001) docker     (123)    22799 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/circuit/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/circuit/skin_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    16825 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/circuit/symb_skin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/format.py
--rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/rendering/pdisplay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.664261 perceval-quandela-0.9.0/perceval/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/runtime/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/runtime/job_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/runtime/local_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/runtime/remote_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/runtime/remote_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/runtime/rpc_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.664261 perceval-quandela-0.9.0/perceval/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/serialization/_circuit_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/serialization/_component_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/serialization/_matrix_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/serialization/_parameter_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/serialization/_schema_circuit_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/serialization/_state_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/serialization/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/serialization/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/serialization/serialize_binary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.664261 perceval-quandela-0.9.0/perceval/simulators/
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/simulators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/simulators/_simulator_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/simulators/delay_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/simulators/loss_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/simulators/polarization_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14820 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/simulators/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/simulators/simulator_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/simulators/simulator_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/simulators/stepper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.668261 perceval-quandela-0.9.0/perceval/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/_random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.668261 perceval-quandela-0.9.0/perceval/utils/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/algorithms/circuit_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/algorithms/decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/algorithms/match.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/algorithms/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/algorithms/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/algorithms/simplification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/algorithms/solve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/mlstr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/polarization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/postselect.py
--rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/stategenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22343 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/perceval/utils/statevector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:34.668261 perceval-quandela-0.9.0/perceval_quandela.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-07-10 10:16:34.000000 perceval-quandela-0.9.0/perceval_quandela.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-10 10:16:34.000000 perceval-quandela-0.9.0/perceval_quandela.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 10:16:34.000000 perceval-quandela-0.9.0/perceval_quandela.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-10 10:16:34.000000 perceval-quandela-0.9.0/perceval_quandela.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-10 10:16:34.000000 perceval-quandela-0.9.0/perceval_quandela.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-10 10:16:34.668261 perceval-quandela-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-10 10:16:31.000000 perceval-quandela-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:30:08.078047 perceval-quandela-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-07-24 12:30:08.078047 perceval-quandela-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:30:08.070047 perceval-quandela-0.9.1/perceval/
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:30:08.070047 perceval-quandela-0.9.1/perceval/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/algorithm/abstract_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/algorithm/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/algorithm/qrng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/algorithm/sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:30:08.070047 perceval-quandela-0.9.1/perceval/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/backends/_abstract_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/backends/_clifford2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/backends/_mps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/backends/_naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/backends/_slos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:30:08.070047 perceval-quandela-0.9.1/perceval/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/components/_mode_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/components/abstract_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21723 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/components/abstract_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/components/component_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:30:08.070047 perceval-quandela-0.9.1/perceval/components/core_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/components/core_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/components/core_catalog/generic_2mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/components/core_catalog/heralded_cnot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/components/core_catalog/heralded_cz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/components/core_catalog/postprocessed_cnot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/components/detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35994 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/components/linear_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/components/non_unitary_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/components/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/components/predefined_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12643 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/components/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/components/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/components/unitary_components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:30:08.074047 perceval-quandela-0.9.1/perceval/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/converters/converter_statevector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/converters/qiskit_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:30:08.074047 perceval-quandela-0.9.1/perceval/rendering/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/rendering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/rendering/_mplot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/rendering/_processor_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:30:08.074047 perceval-quandela-0.9.1/perceval/rendering/canvas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/rendering/canvas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/rendering/canvas/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/rendering/canvas/latex_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5916 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/rendering/canvas/mplot_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/rendering/canvas/svg_canvas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:30:08.074047 perceval-quandela-0.9.1/perceval/rendering/circuit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/rendering/circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/rendering/circuit/abstract_skin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/rendering/circuit/phys_skin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22799 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/rendering/circuit/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/rendering/circuit/skin_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16825 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/rendering/circuit/symb_skin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/rendering/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/rendering/pdisplay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:30:08.074047 perceval-quandela-0.9.1/perceval/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/runtime/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/runtime/job_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/runtime/local_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/runtime/remote_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/runtime/remote_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/runtime/rpc_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:30:08.074047 perceval-quandela-0.9.1/perceval/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/serialization/_circuit_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/serialization/_component_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/serialization/_matrix_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/serialization/_parameter_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/serialization/_schema_circuit_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/serialization/_state_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/serialization/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/serialization/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/serialization/serialize_binary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:30:08.078047 perceval-quandela-0.9.1/perceval/simulators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/simulators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/simulators/_simulator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/simulators/delay_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/simulators/loss_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/simulators/polarization_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17252 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/simulators/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/simulators/simulator_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/simulators/simulator_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6135 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/simulators/stepper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:30:08.078047 perceval-quandela-0.9.1/perceval/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/utils/_random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:30:08.078047 perceval-quandela-0.9.1/perceval/utils/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/utils/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/utils/algorithms/circuit_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/utils/algorithms/decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/utils/algorithms/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/utils/algorithms/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/utils/algorithms/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/utils/algorithms/simplification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/utils/algorithms/solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/utils/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/utils/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/utils/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/utils/mlstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/utils/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/utils/polarization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/utils/postselect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/utils/stategenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22330 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/perceval/utils/statevector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:30:08.078047 perceval-quandela-0.9.1/perceval_quandela.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-07-24 12:30:08.000000 perceval-quandela-0.9.1/perceval_quandela.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-24 12:30:08.000000 perceval-quandela-0.9.1/perceval_quandela.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:30:08.000000 perceval-quandela-0.9.1/perceval_quandela.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-24 12:30:08.000000 perceval-quandela-0.9.1/perceval_quandela.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-24 12:30:08.000000 perceval-quandela-0.9.1/perceval_quandela.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-24 12:30:08.082047 perceval-quandela-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-24 12:30:01.000000 perceval-quandela-0.9.1/setup.py
```

### Comparing `perceval-quandela-0.9.0/LICENSE` & `perceval-quandela-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/PKG-INFO` & `perceval-quandela-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perceval-quandela
-Version: 0.9.0
+Version: 0.9.1
 Summary: A powerful Quantum Photonic Framework
 Home-page: https://github.com/Quandela/Perceval
 Author: Perceval@Quandela.com
 Author-email: Perceval@Quandela.com
 Project-URL: Documentation, https://perceval.quandela.net/docs/
 Project-URL: Source, https://github.com/Quandela/Perceval
 Project-URL: Tracker, https://github.com/Quandela/Perceval/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: perceval-quandela Version: 0.9.0 Summary: A
+Metadata-Version: 2.1 Name: perceval-quandela Version: 0.9.1 Summary: A
 powerful Quantum Photonic Framework Home-page: https://github.com/Quandela/
 Perceval Author: Perceval@Quandela.com Author-email: Perceval@Quandela.com
 Project-URL: Documentation, https://perceval.quandela.net/docs/ Project-URL:
 Source, https://github.com/Quandela/Perceval Project-URL: Tracker, https://
 github.com/Quandela/Perceval/issues Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
```

### Comparing `perceval-quandela-0.9.0/README.md` & `perceval-quandela-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/__init__.py` & `perceval-quandela-0.9.1/perceval/__init__.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/algorithm/__init__.py` & `perceval-quandela-0.9.1/perceval/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/algorithm/abstract_algorithm.py` & `perceval-quandela-0.9.1/perceval/algorithm/abstract_algorithm.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/algorithm/analyzer.py` & `perceval-quandela-0.9.1/perceval/algorithm/analyzer.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/algorithm/qrng.py` & `perceval-quandela-0.9.1/perceval/algorithm/qrng.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/algorithm/sampler.py` & `perceval-quandela-0.9.1/perceval/algorithm/sampler.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/backends/__init__.py` & `perceval-quandela-0.9.1/perceval/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/backends/_abstract_backends.py` & `perceval-quandela-0.9.1/perceval/backends/_abstract_backends.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/backends/_clifford2017.py` & `perceval-quandela-0.9.1/perceval/backends/_clifford2017.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/backends/_mps.py` & `perceval-quandela-0.9.1/perceval/backends/_mps.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/backends/_naive.py` & `perceval-quandela-0.9.1/perceval/backends/_naive.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/backends/_slos.py` & `perceval-quandela-0.9.1/perceval/backends/_slos.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/components/__init__.py` & `perceval-quandela-0.9.1/perceval/components/__init__.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/components/_mode_connector.py` & `perceval-quandela-0.9.1/perceval/components/_mode_connector.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/components/abstract_component.py` & `perceval-quandela-0.9.1/perceval/components/abstract_component.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/components/abstract_processor.py` & `perceval-quandela-0.9.1/perceval/components/abstract_processor.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/components/component_catalog.py` & `perceval-quandela-0.9.1/perceval/components/component_catalog.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/components/core_catalog/__init__.py` & `perceval-quandela-0.9.1/perceval/components/core_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/components/core_catalog/generic_2mode.py` & `perceval-quandela-0.9.1/perceval/components/core_catalog/generic_2mode.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/components/core_catalog/heralded_cnot.py` & `perceval-quandela-0.9.1/perceval/components/core_catalog/heralded_cnot.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/components/core_catalog/heralded_cz.py` & `perceval-quandela-0.9.1/perceval/components/core_catalog/heralded_cz.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/components/core_catalog/postprocessed_cnot.py` & `perceval-quandela-0.9.1/perceval/components/core_catalog/postprocessed_cnot.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/components/detector.py` & `perceval-quandela-0.9.1/perceval/components/detector.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/components/linear_circuit.py` & `perceval-quandela-0.9.1/perceval/components/linear_circuit.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/components/non_unitary_components.py` & `perceval-quandela-0.9.1/perceval/components/non_unitary_components.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/components/port.py` & `perceval-quandela-0.9.1/perceval/components/port.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/components/predefined_circuit.py` & `perceval-quandela-0.9.1/perceval/components/predefined_circuit.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/components/processor.py` & `perceval-quandela-0.9.1/perceval/components/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         - an int: number of modes of interest (MOI). A mode of interest is any non-heralded mode.
         >>> p = Processor("SLOS", 5)
 
         - a circuit: the input circuit to start with. Other components can still be added afterwards with `add()`
         >>> p = Processor("SLOS", BS() // PS() // BS())
 
     :param source: the Source used by the processor (defaults to perfect source)
+    :param name: a textual name for the processor (defaults to "Local processor")
     """
     def __init__(self, backend: Union[ABackend, str], m_circuit: Union[int, ACircuit] = None, source: Source = Source(),
                  name: str = None):
         super().__init__()
         self._source = source
         self.name = "Local processor" if name is None else name
 
@@ -248,14 +249,17 @@
         return {'results': output, 'physical_perf': physical_perf, 'logical_perf': logical_perf}
 
     def probs(self, progress_callback: Callable = None) -> Dict:
         # assert self._inputs_map is not None, "Input is missing, please call with_inputs()"
         if self._simulator is None:
             from perceval.simulators import SimulatorFactory  # Avoids a circular import
             self._simulator = SimulatorFactory.build(self)
+        else:
+            self._simulator.set_circuit(self.linear_circuit() if self._is_unitary else self.components)
+
         res = self._simulator.probs_svd(self._inputs_map, progress_callback=progress_callback)
         lperf = 1
         pperf = 1
         postprocessed_res = BSDistribution()
         for state, prob in res['results'].items():
             if not self._state_selected_physical(state):
                 pperf -= prob
```

### Comparing `perceval-quandela-0.9.0/perceval/components/source.py` & `perceval-quandela-0.9.1/perceval/components/source.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/components/unitary_components.py` & `perceval-quandela-0.9.1/perceval/components/unitary_components.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/converters/__init__.py` & `perceval-quandela-0.9.1/perceval/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/converters/converter_statevector.py` & `perceval-quandela-0.9.1/perceval/converters/converter_statevector.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/converters/qiskit_converter.py` & `perceval-quandela-0.9.1/perceval/converters/qiskit_converter.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/rendering/__init__.py` & `perceval-quandela-0.9.1/perceval/rendering/__init__.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/rendering/_mplot_utils.py` & `perceval-quandela-0.9.1/perceval/rendering/_mplot_utils.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/rendering/_processor_utils.py` & `perceval-quandela-0.9.1/perceval/rendering/_processor_utils.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/rendering/canvas/__init__.py` & `perceval-quandela-0.9.1/perceval/rendering/canvas/__init__.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/rendering/canvas/canvas.py` & `perceval-quandela-0.9.1/perceval/rendering/canvas/canvas.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/rendering/canvas/latex_canvas.py` & `perceval-quandela-0.9.1/perceval/rendering/canvas/latex_canvas.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/rendering/canvas/mplot_canvas.py` & `perceval-quandela-0.9.1/perceval/rendering/canvas/mplot_canvas.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/rendering/canvas/svg_canvas.py` & `perceval-quandela-0.9.1/perceval/rendering/canvas/svg_canvas.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/rendering/circuit/__init__.py` & `perceval-quandela-0.9.1/perceval/rendering/circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/rendering/circuit/abstract_skin.py` & `perceval-quandela-0.9.1/perceval/rendering/circuit/abstract_skin.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/rendering/circuit/phys_skin.py` & `perceval-quandela-0.9.1/perceval/rendering/circuit/phys_skin.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/rendering/circuit/renderer.py` & `perceval-quandela-0.9.1/perceval/rendering/circuit/renderer.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/rendering/circuit/skin_common.py` & `perceval-quandela-0.9.1/perceval/rendering/circuit/skin_common.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/rendering/circuit/symb_skin.py` & `perceval-quandela-0.9.1/perceval/rendering/circuit/symb_skin.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/rendering/format.py` & `perceval-quandela-0.9.1/perceval/rendering/format.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/rendering/pdisplay.py` & `perceval-quandela-0.9.1/perceval/rendering/pdisplay.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/runtime/__init__.py` & `perceval-quandela-0.9.1/perceval/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/runtime/job.py` & `perceval-quandela-0.9.1/perceval/runtime/job.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/runtime/job_status.py` & `perceval-quandela-0.9.1/perceval/runtime/job_status.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/runtime/local_job.py` & `perceval-quandela-0.9.1/perceval/runtime/local_job.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/runtime/remote_job.py` & `perceval-quandela-0.9.1/perceval/runtime/remote_job.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/runtime/remote_processor.py` & `perceval-quandela-0.9.1/perceval/runtime/remote_processor.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/runtime/rpc_handler.py` & `perceval-quandela-0.9.1/perceval/runtime/rpc_handler.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/serialization/__init__.py` & `perceval-quandela-0.9.1/perceval/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/serialization/_circuit_serialization.py` & `perceval-quandela-0.9.1/perceval/serialization/_circuit_serialization.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/serialization/_component_deserialization.py` & `perceval-quandela-0.9.1/perceval/serialization/_component_deserialization.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/serialization/_matrix_serialization.py` & `perceval-quandela-0.9.1/perceval/serialization/_matrix_serialization.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/serialization/_parameter_serialization.py` & `perceval-quandela-0.9.1/perceval/serialization/_parameter_serialization.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/serialization/_schema_circuit_pb2.py` & `perceval-quandela-0.9.1/perceval/serialization/_schema_circuit_pb2.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/serialization/_state_serialization.py` & `perceval-quandela-0.9.1/perceval/serialization/_state_serialization.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/serialization/deserialize.py` & `perceval-quandela-0.9.1/perceval/serialization/deserialize.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/serialization/serialize.py` & `perceval-quandela-0.9.1/perceval/serialization/serialize.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/serialization/serialize_binary.py` & `perceval-quandela-0.9.1/perceval/serialization/serialize_binary.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/simulators/__init__.py` & `perceval-quandela-0.9.1/perceval/simulators/__init__.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/simulators/_simulator_utils.py` & `perceval-quandela-0.9.1/perceval/simulators/_simulator_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 from perceval.utils import BasicState, BSDistribution, StateVector, Annotation
 from perceval.components import Circuit
 from copy import copy
+from math import sqrt
 from typing import List
 
 
 def _to_bsd(sv: StateVector) -> BSDistribution:
     res = BSDistribution()
     sv_copy = copy(sv)
     sv_copy.normalize()
@@ -47,21 +48,24 @@
     res_sv = copy(sv)
     if str(annotation):  # len(annotation) not working on unix
         for s in res_sv:
             s.inject_annotation(annotation)
     return res_sv
 
 
-def _merge_sv(sv1: StateVector, sv2: StateVector) -> StateVector:
+def _merge_sv(sv1: StateVector, sv2: StateVector, prob_threshold: float = 0) -> StateVector:
     if not sv1:
         return sv2
+    pa_threshold = sqrt(prob_threshold)
     res = StateVector()
     for s1, pa1 in sv1.items():
         for s2, pa2 in sv2.items():
-            res[s1.merge(s2)] += pa1*pa2
+            pa = pa1*pa2
+            if abs(pa) > pa_threshold:
+                res[s1.merge(s2)] += pa
     return res
 
 
 def _annot_state_mapping(bs_with_annots: BasicState):
     bs_list = bs_with_annots.separate_state(keep_annotations=True)
     mapping = {}
     for bs in bs_list:
```

### Comparing `perceval-quandela-0.9.0/perceval/simulators/delay_simulator.py` & `perceval-quandela-0.9.1/perceval/simulators/delay_simulator.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/simulators/loss_simulator.py` & `perceval-quandela-0.9.1/perceval/simulators/loss_simulator.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/simulators/polarization_simulator.py` & `perceval-quandela-0.9.1/perceval/simulators/polarization_simulator.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/simulators/simulator.py` & `perceval-quandela-0.9.1/perceval/simulators/simulator.py`

 * *Files 4% similar despite different names*

```diff
@@ -163,32 +163,24 @@
             state.clear_annotations()
             if state == output_state:
                 result += abs(pa) ** 2
         return result
 
     def _invalidate_cache(self):
         self._evolve = {}
-        self._probd = {}
         self.DEBUG_evolve_count = 0
         self.DEBUG_merge_count = 0
 
     def _evolve_cache(self, input_list: Set[BasicState]):
         for state in input_list:
             if state not in self._evolve:
                 self._backend.set_input_state(state)
                 self._evolve[state] = self._backend.evolve()
                 self.DEBUG_evolve_count += 1
 
-    def _probs_cache(self, input_list: Set[BasicState]):
-        for state in input_list:
-            if state not in self._probd:
-                self._backend.set_input_state(state)
-                self._probd[state] = self._backend.prob_distribution()
-                self.DEBUG_evolve_count += 1
-
     def _merge_probability_dist(self, input_list) -> BSDistribution:
         results = BSDistribution()
         for input_state in input_list:
             results = BSDistribution.tensor_product(results, _to_bsd(self._evolve[input_state]), merge_modes=True)
             self.DEBUG_merge_count += 1
         return results
 
@@ -220,93 +212,158 @@
 
     @dispatch(StateVector)
     def probs(self, input_state: StateVector) -> BSDistribution:
         if len(input_state) == 1:
             return self.probs(input_state[0])
         return self._post_select_on_distribution(_to_bsd(self.evolve(input_state)))
 
-    def probs_svd(self, input_dist: SVDistribution, progress_callback: Optional[Callable] = None):
-        """
-        Compute the probability distribution from a SVDistribution input and as well as performance scores
-
-        :param input_dist: A state vector distribution describing the input to simulate
-        :param progress_callback: A function with the signature `func(progress: float, message: str)`
-
-        :return: A dictionary of the form { "results": BSDistribution, "physical_perf": float, "logical_perf": float }
-        * results is the post-selected output state distribution
-        * physical_perf is the performance computed from the detected photon filter
-        * logical_perf is the performance computed from the post-selection
-        """
-
-        """Trim input SVD given _rel_precision threshold"""
-        max_p = 0
-        for sv, p in input_dist.items():
-            if max(sv.n) >= self._min_detected_photons:
-                max_p = p
-                break
-        p_threshold = max(global_params['min_p'], max_p * self._rel_precision)
-        svd = SVDistribution({state: pr for state, pr in input_dist.items() if pr > p_threshold})
 
+    def _probs_svd_generic(self, input_dist, p_threshold, progress_callback: Optional[Callable] = None):
+        decomposed_input = []
         """decomposed input:
         From a SVD = {
             pa_11*bs_11 + ... + pa_n1*bs_n1: p1,
             pa_12*bs_12 + ... + pa_n2*bs_n2: p2,
             ...
             pa_1k*bs_1k + ... + pa_nk*bs_nk: pk
         }
         the following data structure is built:
         [
             (p1, [
-                    (pa_11, [bs_11,]),
+                    (pa_11, {annot_11*: bs_11*,..}),
                     ...
-                    (pa_n1, [bs_n1,])
+                    (pa_n1, {annot_n1*: bs_n1*,..})
                  ]
             ),
+            ...
             (pk, [
-                    (pa_1k, [bs_1k,]),
+                    (pa_1k, {annot_1k*: bs_1k*,..}),
                     ...
-                    (pa_nk, [bs_nk,])
+                    (pa_nk, {annot_nk*: bs_nk*,..})
                  ]
             )
         ]
-        where [bs_xy,] is the list of the un-annotated separated basic state (bs_xy.separate_state())
-        """
-        decomposed_input = []
-        for sv, prob in svd.items():
+        where {annot_xy*: bs_xy*,..} is a mapping between an annotation and a pure basic state"""
+        for sv, prob in input_dist.items():
             if min(sv.n) >= self._min_detected_photons:
-                decomposed_input.append((prob, [(abs(pa)**2, st.separate_state(keep_annotations=False)) for st, pa in sv.items()]))
+                decomposed_input.append((prob, [(pa, _annot_state_mapping(st)) for st, pa in sv.items()]))
             else:
                 self._physical_perf -= prob
-        input_set = set([state for s in decomposed_input for t in s[1] for state in t[1]])
-        self._probs_cache(input_set)
+        input_set = set([state for s in decomposed_input for t in s[1] for state in t[1].values()])
+        self._evolve_cache(input_set)
 
         """Reconstruct output probability distribution"""
         res = BSDistribution()
         for idx, (prob0, sv_data) in enumerate(decomposed_input):
             """First, recombine evolved state vectors given a single input"""
-            result_bsd = BSDistribution()
+            result_sv = StateVector()
             for probampli, instate_list in sv_data:
                 prob_sv = abs(probampli)**2
-                evolved_in_s = BSDistribution()
-                for in_s in instate_list:
-                    evolved_in_s = BSDistribution.tensor_product(evolved_in_s, self._probd[in_s],
-                                                                 merge_modes=True,
-                                                                 prob_threshold=p_threshold/(prob_sv*prob0))
+                evolved_in_s = StateVector()
+                for annot, in_s in instate_list.items():
+                    cached_res = _inject_annotation(self._evolve[in_s], annot)
+                    evolved_in_s = _merge_sv(evolved_in_s, cached_res, prob_threshold=p_threshold / (10 * prob_sv * prob0))
+                    if len(evolved_in_s) == 0:
+                        break
                     self.DEBUG_merge_count += 1
-                for bs, p in evolved_in_s.items():
-                    result_bsd[bs] += prob_sv*p
+                if evolved_in_s:
+                    result_sv += probampli*evolved_in_s
 
-            """Then, add the resulting distribution the """
-            for bs, p in result_bsd.items():
+            """Then, add the resulting distribution for a single input to the global distribution"""
+            for bs, p in _to_bsd(result_sv).items():
                 res[bs] += p*prob0
 
             if progress_callback:
                 exec_request = progress_callback((idx + 1) / len(decomposed_input), 'probs')
                 if exec_request is not None and 'cancel_requested' in exec_request and exec_request['cancel_requested']:
                     raise RuntimeError("Cancel requested")
+        return res
+
+    def _probs_svd_fast(self, input_dist, p_threshold, progress_callback: Optional[Callable] = None):
+        decomposed_input = []
+        """decomposed input:
+       From a SVD = {
+           bs_1: p1,
+           bs_2: p2,
+           ...
+           bs_k: pk
+       }
+       the following data structure is built:
+       [
+           (p1, [bs_1,]),
+           ...
+           (pk, [bs_k,])
+       ]
+       where [bs_x,] is the list of the un-annotated separated basic state (bs_x.separate_state())"""
+        for sv, prob in input_dist.items():
+            if min(sv.n) >= self._min_detected_photons:
+                decomposed_input.append(
+                    (prob, sv[0].separate_state(keep_annotations=False))
+                )
+            else:
+                self._physical_perf -= prob
+        input_set = set([state for s in decomposed_input for state in s[1]])
+        cache = {}
+        for state in input_set:
+            self._backend.set_input_state(state)
+            cache[state] = self._backend.prob_distribution()
+
+        """Reconstruct output probability distribution"""
+        res = BSDistribution()
+        for idx, (prob0, bs_data) in enumerate(decomposed_input):
+            """First, recombine evolved state vectors given a single input"""
+            probs_in_s = BSDistribution()
+            for in_s in bs_data:
+                probs_in_s = BSDistribution.tensor_product(probs_in_s, cache[in_s],
+                                                           merge_modes=True,
+                                                           prob_threshold=p_threshold / (10*prob0))
+                if len(probs_in_s) == 0:
+                    break
+                self.DEBUG_merge_count += 1
+
+            """Then, add the resulting distribution to the global distribution"""
+            if probs_in_s:
+                for bs, p in probs_in_s.items():
+                    res[bs] += p * prob0
+
+            if progress_callback:
+                exec_request = progress_callback((idx + 1) / len(decomposed_input), 'probs')
+                if exec_request is not None and 'cancel_requested' in exec_request and exec_request['cancel_requested']:
+                    raise RuntimeError("Cancel requested")
+        return res
+
+
+    def probs_svd(self, input_dist: SVDistribution, progress_callback: Optional[Callable] = None):
+        """
+        Compute the probability distribution from a SVDistribution input and as well as performance scores
+
+        :param input_dist: A state vector distribution describing the input to simulate
+        :param progress_callback: A function with the signature `func(progress: float, message: str)`
+
+        :return: A dictionary of the form { "results": BSDistribution, "physical_perf": float, "logical_perf": float }
+        * results is the post-selected output state distribution
+        * physical_perf is the performance computed from the detected photon filter
+        * logical_perf is the performance computed from the post-selection
+        """
+
+        """Trim input SVD given _rel_precision threshold"""
+        max_p = 0
+        has_superposed_states = False
+        for sv, p in input_dist.items():
+            if max(sv.n) >= self._min_detected_photons:
+                max_p = max(p, max_p)
+            if len(sv) > 1:
+                has_superposed_states = True
+        p_threshold = max(global_params['min_p'], max_p * self._rel_precision)
+        svd = SVDistribution({state: pr for state, pr in input_dist.items() if pr > p_threshold})
+        if has_superposed_states:
+            res = self._probs_svd_generic(svd, p_threshold, progress_callback)
+        else:
+            res = self._probs_svd_fast(svd, p_threshold, progress_callback)
+
         return {'results': self._post_select_on_distribution(res),
                 'physical_perf': self._physical_perf,
                 'logical_perf': self._logical_perf}
 
     def evolve(self, input_state: Union[BasicState, StateVector]) -> StateVector:
         """
         Evolve a state through the circuit
```

### Comparing `perceval-quandela-0.9.0/perceval/simulators/simulator_factory.py` & `perceval-quandela-0.9.1/perceval/simulators/simulator_factory.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/simulators/simulator_interface.py` & `perceval-quandela-0.9.1/perceval/simulators/simulator_interface.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/simulators/stepper.py` & `perceval-quandela-0.9.1/perceval/simulators/stepper.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/utils/__init__.py` & `perceval-quandela-0.9.1/perceval/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/utils/_random.py` & `perceval-quandela-0.9.1/perceval/utils/_random.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/utils/algorithms/__init__.py` & `perceval-quandela-0.9.1/perceval/utils/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/utils/algorithms/circuit_optimizer.py` & `perceval-quandela-0.9.1/perceval/utils/algorithms/circuit_optimizer.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/utils/algorithms/decomposition.py` & `perceval-quandela-0.9.1/perceval/utils/algorithms/decomposition.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/utils/algorithms/match.py` & `perceval-quandela-0.9.1/perceval/utils/algorithms/match.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/utils/algorithms/norm.py` & `perceval-quandela-0.9.1/perceval/utils/algorithms/norm.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/utils/algorithms/optimize.py` & `perceval-quandela-0.9.1/perceval/utils/algorithms/optimize.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/utils/algorithms/simplification.py` & `perceval-quandela-0.9.1/perceval/utils/algorithms/simplification.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/utils/algorithms/solve.py` & `perceval-quandela-0.9.1/perceval/utils/algorithms/solve.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/utils/conversion.py` & `perceval-quandela-0.9.1/perceval/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/utils/format.py` & `perceval-quandela-0.9.1/perceval/utils/format.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/utils/globals.py` & `perceval-quandela-0.9.1/perceval/utils/globals.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/utils/matrix.py` & `perceval-quandela-0.9.1/perceval/utils/matrix.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/utils/mlstr.py` & `perceval-quandela-0.9.1/perceval/utils/mlstr.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/utils/parameter.py` & `perceval-quandela-0.9.1/perceval/utils/parameter.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/utils/polarization.py` & `perceval-quandela-0.9.1/perceval/utils/polarization.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/utils/postselect.py` & `perceval-quandela-0.9.1/perceval/utils/postselect.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/utils/stategenerator.py` & `perceval-quandela-0.9.1/perceval/utils/stategenerator.py`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/perceval/utils/statevector.py` & `perceval-quandela-0.9.1/perceval/utils/statevector.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,15 +321,15 @@
 
     @property
     def n(self):
         r"""list the possible values of n in the different states"""
         return list(set([st.n for st in self.keys()]))
 
     def normalize(self):
-        r"""Normalize a non-normalized BasicState"""
+        r"""Normalize a state vector"""
         if not self._normalized:
             norm = 0
             to_remove = []
             for key in self.keys():
                 if (isinstance(self[key], (complex, float, int))
                         and abs(self[key]) < global_params["min_complex_component"]) or self[key] == 0:
                     to_remove.append(key)
```

### Comparing `perceval-quandela-0.9.0/perceval_quandela.egg-info/PKG-INFO` & `perceval-quandela-0.9.1/perceval_quandela.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perceval-quandela
-Version: 0.9.0
+Version: 0.9.1
 Summary: A powerful Quantum Photonic Framework
 Home-page: https://github.com/Quandela/Perceval
 Author: Perceval@Quandela.com
 Author-email: Perceval@Quandela.com
 Project-URL: Documentation, https://perceval.quandela.net/docs/
 Project-URL: Source, https://github.com/Quandela/Perceval
 Project-URL: Tracker, https://github.com/Quandela/Perceval/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: perceval-quandela Version: 0.9.0 Summary: A
+Metadata-Version: 2.1 Name: perceval-quandela Version: 0.9.1 Summary: A
 powerful Quantum Photonic Framework Home-page: https://github.com/Quandela/
 Perceval Author: Perceval@Quandela.com Author-email: Perceval@Quandela.com
 Project-URL: Documentation, https://perceval.quandela.net/docs/ Project-URL:
 Source, https://github.com/Quandela/Perceval Project-URL: Tracker, https://
 github.com/Quandela/Perceval/issues Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
```

### Comparing `perceval-quandela-0.9.0/perceval_quandela.egg-info/SOURCES.txt` & `perceval-quandela-0.9.1/perceval_quandela.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `perceval-quandela-0.9.0/setup.py` & `perceval-quandela-0.9.1/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/pyquil-4.0.0rc8.tar.gz` & `tmp/pyquil-4.0.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyquil-4.0.0rc8.tar", max compression
+gzip compressed data, was "pyquil-4.0.0rc9.tar", max compression
```

## Comparing `pyquil-4.0.0rc8.tar` & `pyquil-4.0.0rc9.tar`

### file list

```diff
@@ -1,74 +1,73 @@
--rw-r--r--   0        0        0    11358 2023-03-22 23:38:21.677140 pyquil-4.0.0rc8/LICENSE
--rw-r--r--   0        0        0     9158 2023-03-22 23:38:21.677140 pyquil-4.0.0rc8/README.md
--rw-r--r--   0        0        0     2217 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyproject.toml
--rw-r--r--   0        0        0      159 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/__init__.py
--rw-r--r--   0        0        0     2349 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/_memory.py
--rw-r--r--   0        0        0      487 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/_parser/README.md
--rw-r--r--   0        0        0        0 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/_parser/__init__.py
--rw-r--r--   0        0        0    10040 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/_parser/grammar.lark
--rw-r--r--   0        0        0    16369 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/_parser/parser.py
--rw-r--r--   0        0        0      844 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/_version.py
--rw-r--r--   0        0        0     1831 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/api/__init__.py
--rw-r--r--   0        0        0     9525 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/api/_abstract_compiler.py
--rw-r--r--   0        0        0     7388 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/api/_benchmark.py
--rw-r--r--   0        0        0     7769 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/api/_compiler.py
--rw-r--r--   0        0        0     8724 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/api/_compiler_client.py
--rw-r--r--   0        0        0     4265 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/api/_errors.py
--rw-r--r--   0        0        0     1010 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/api/_logger.py
--rw-r--r--   0        0        0     2601 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/api/_qam.py
--rw-r--r--   0        0        0     1750 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/api/_qcs_client.py
--rw-r--r--   0        0        0     7978 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/api/_qpu.py
--rw-r--r--   0        0        0    54520 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/api/_quantum_computer.py
--rw-r--r--   0        0        0    10574 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/api/_qvm.py
--rw-r--r--   0        0        0     9415 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/api/_qvm_client.py
--rw-r--r--   0        0        0     5536 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/api/_rewrite_arithmetic.py
--rw-r--r--   0        0        0    13285 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/api/_wavefunction_simulator.py
--rw-r--r--   0        0        0      859 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/compatibility/__init__.py
--rw-r--r--   0        0        0     1371 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/experiment/__init__.py
--rw-r--r--   0        0        0      896 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/experiment/_calibration.py
--rw-r--r--   0        0        0    15705 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/experiment/_group.py
--rw-r--r--   0        0        0    22783 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/experiment/_main.py
--rw-r--r--   0        0        0     8213 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/experiment/_memory.py
--rw-r--r--   0        0        0     5547 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/experiment/_program.py
--rw-r--r--   0        0        0     9047 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/experiment/_result.py
--rw-r--r--   0        0        0     7469 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/experiment/_setting.py
--rw-r--r--   0        0        0      934 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/experiment/_symmetrization.py
--rw-r--r--   0        0        0      282 2023-03-22 23:38:21.993153 pyquil-4.0.0rc8/pyquil/external/README.md
--rw-r--r--   0        0        0        0 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/external/__init__.py
--rw-r--r--   0        0        0     3474 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/external/rpcq.py
--rw-r--r--   0        0        0    36868 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/gates.py
--rw-r--r--   0        0        0      201 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/latex/__init__.py
--rw-r--r--   0        0        0    18772 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/latex/_diagram.py
--rw-r--r--   0        0        0     3452 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/latex/_ipython.py
--rw-r--r--   0        0        0     4041 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/latex/_main.py
--rw-r--r--   0        0        0     1266 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/latex/latex_generation.py
--rw-r--r--   0        0        0    31923 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/noise.py
--rw-r--r--   0        0        0     3346 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/noise_gates.py
--rw-r--r--   0        0        0    15865 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/operator_estimation.py
--rw-r--r--   0        0        0     1511 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/parser.py
--rw-r--r--   0        0        0    38551 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/paulis.py
--rw-r--r--   0        0        0        0 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/py.typed
--rw-r--r--   0        0        0    19258 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/pyqvm.py
--rw-r--r--   0        0        0      336 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/quantum_processor/__init__.py
--rw-r--r--   0        0        0     1662 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/quantum_processor/_base.py
--rw-r--r--   0        0        0        0 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/quantum_processor/_isa.py
--rw-r--r--   0        0        0      774 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/quantum_processor/compiler.py
--rw-r--r--   0        0        0     1856 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/quantum_processor/graph.py
--rw-r--r--   0        0        0     3048 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/quantum_processor/qcs.py
--rw-r--r--   0        0        0      417 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/quantum_processor/transformers/__init__.py
--rw-r--r--   0        0        0      331 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/quantum_processor/transformers/compiler_isa_to_graph.py
--rw-r--r--   0        0        0     5279 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/quantum_processor/transformers/graph_to_compiler_isa.py
--rw-r--r--   0        0        0    11776 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/quantum_processor/transformers/qcs_isa_to_compiler_isa.py
--rw-r--r--   0        0        0      230 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/quantum_processor/transformers/qcs_isa_to_graph.py
--rw-r--r--   0        0        0    53538 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/quil.py
--rw-r--r--   0        0        0    27030 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/quilatom.py
--rw-r--r--   0        0        0    40353 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/quilbase.py
--rw-r--r--   0        0        0     6107 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/quiltcalibrations.py
--rw-r--r--   0        0        0    11070 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/quiltwaveforms.py
--rw-r--r--   0        0        0      511 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/simulation/__init__.py
--rw-r--r--   0        0        0    13335 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/simulation/_numpy.py
--rw-r--r--   0        0        0    15747 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/simulation/_reference.py
--rw-r--r--   0        0        0    10159 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/simulation/matrices.py
--rw-r--r--   0        0        0    18875 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/simulation/tools.py
--rw-r--r--   0        0        0     8754 2023-03-22 23:38:21.997153 pyquil-4.0.0rc8/pyquil/wavefunction.py
--rw-r--r--   0        0        0    11064 1970-01-01 00:00:00.000000 pyquil-4.0.0rc8/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-03-28 21:14:14.649811 pyquil-4.0.0rc9/LICENSE
+-rw-r--r--   0        0        0     9158 2023-03-28 21:14:14.649811 pyquil-4.0.0rc9/README.md
+-rw-r--r--   0        0        0     2264 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyproject.toml
+-rw-r--r--   0        0        0      159 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/__init__.py
+-rw-r--r--   0        0        0     2349 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/_memory.py
+-rw-r--r--   0        0        0      487 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/_parser/README.md
+-rw-r--r--   0        0        0        0 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/_parser/__init__.py
+-rw-r--r--   0        0        0    10040 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/_parser/grammar.lark
+-rw-r--r--   0        0        0    16369 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/_parser/parser.py
+-rw-r--r--   0        0        0      844 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/_version.py
+-rw-r--r--   0        0        0     1791 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/api/__init__.py
+-rw-r--r--   0        0        0     8718 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/api/_abstract_compiler.py
+-rw-r--r--   0        0        0     7335 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/api/_benchmark.py
+-rw-r--r--   0        0        0     6633 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/api/_compiler.py
+-rw-r--r--   0        0        0     7753 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/api/_compiler_client.py
+-rw-r--r--   0        0        0     4265 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/api/_errors.py
+-rw-r--r--   0        0        0     1010 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/api/_logger.py
+-rw-r--r--   0        0        0     2601 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/api/_qam.py
+-rw-r--r--   0        0        0     7716 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/api/_qpu.py
+-rw-r--r--   0        0        0    53168 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/api/_quantum_computer.py
+-rw-r--r--   0        0        0    10522 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/api/_qvm.py
+-rw-r--r--   0        0        0     9348 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/api/_qvm_client.py
+-rw-r--r--   0        0        0     5536 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/api/_rewrite_arithmetic.py
+-rw-r--r--   0        0        0    13232 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/api/_wavefunction_simulator.py
+-rw-r--r--   0        0        0      859 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/compatibility/__init__.py
+-rw-r--r--   0        0        0     1371 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/experiment/__init__.py
+-rw-r--r--   0        0        0      896 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/experiment/_calibration.py
+-rw-r--r--   0        0        0    15705 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/experiment/_group.py
+-rw-r--r--   0        0        0    22783 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/experiment/_main.py
+-rw-r--r--   0        0        0     8213 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/experiment/_memory.py
+-rw-r--r--   0        0        0     5547 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/experiment/_program.py
+-rw-r--r--   0        0        0     9047 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/experiment/_result.py
+-rw-r--r--   0        0        0     7469 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/experiment/_setting.py
+-rw-r--r--   0        0        0      934 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/experiment/_symmetrization.py
+-rw-r--r--   0        0        0      282 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/external/README.md
+-rw-r--r--   0        0        0        0 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/external/__init__.py
+-rw-r--r--   0        0        0     3474 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/external/rpcq.py
+-rw-r--r--   0        0        0    36868 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/gates.py
+-rw-r--r--   0        0        0      201 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/latex/__init__.py
+-rw-r--r--   0        0        0    18772 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/latex/_diagram.py
+-rw-r--r--   0        0        0     3452 2023-03-28 21:14:14.965811 pyquil-4.0.0rc9/pyquil/latex/_ipython.py
+-rw-r--r--   0        0        0     4041 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/latex/_main.py
+-rw-r--r--   0        0        0     1266 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/latex/latex_generation.py
+-rw-r--r--   0        0        0    31923 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/noise.py
+-rw-r--r--   0        0        0     3346 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/noise_gates.py
+-rw-r--r--   0        0        0    15865 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/operator_estimation.py
+-rw-r--r--   0        0        0     1511 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/parser.py
+-rw-r--r--   0        0        0    38551 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/paulis.py
+-rw-r--r--   0        0        0        0 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/py.typed
+-rw-r--r--   0        0        0    19258 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/pyqvm.py
+-rw-r--r--   0        0        0      336 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/quantum_processor/__init__.py
+-rw-r--r--   0        0        0     1662 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/quantum_processor/_base.py
+-rw-r--r--   0        0        0        0 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/quantum_processor/_isa.py
+-rw-r--r--   0        0        0      774 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/quantum_processor/compiler.py
+-rw-r--r--   0        0        0     1856 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/quantum_processor/graph.py
+-rw-r--r--   0        0        0     2714 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/quantum_processor/qcs.py
+-rw-r--r--   0        0        0      417 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/quantum_processor/transformers/__init__.py
+-rw-r--r--   0        0        0      331 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/quantum_processor/transformers/compiler_isa_to_graph.py
+-rw-r--r--   0        0        0     5279 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/quantum_processor/transformers/graph_to_compiler_isa.py
+-rw-r--r--   0        0        0    11770 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/quantum_processor/transformers/qcs_isa_to_compiler_isa.py
+-rw-r--r--   0        0        0      224 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/quantum_processor/transformers/qcs_isa_to_graph.py
+-rw-r--r--   0        0        0    53538 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/quil.py
+-rw-r--r--   0        0        0    27030 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/quilatom.py
+-rw-r--r--   0        0        0    40353 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/quilbase.py
+-rw-r--r--   0        0        0     6107 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/quiltcalibrations.py
+-rw-r--r--   0        0        0    11070 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/quiltwaveforms.py
+-rw-r--r--   0        0        0      511 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/simulation/__init__.py
+-rw-r--r--   0        0        0    13335 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/simulation/_numpy.py
+-rw-r--r--   0        0        0    15747 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/simulation/_reference.py
+-rw-r--r--   0        0        0    10159 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/simulation/matrices.py
+-rw-r--r--   0        0        0    18875 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/simulation/tools.py
+-rw-r--r--   0        0        0     8754 2023-03-28 21:14:14.969811 pyquil-4.0.0rc9/pyquil/wavefunction.py
+-rw-r--r--   0        0        0    11115 1970-01-01 00:00:00.000000 pyquil-4.0.0rc9/PKG-INFO
```

### Comparing `pyquil-4.0.0rc8/LICENSE` & `pyquil-4.0.0rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/README.md` & `pyquil-4.0.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyproject.toml` & `pyquil-4.0.0rc9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyquil"
-version = "4.0.0-rc.8"
+version = "4.0.0-rc.9"
 description = "A Python library for creating Quantum Instruction Language (Quil) programs."
 authors = ["Rigetti Computing <softapps@rigetti.com>"]
 readme = "README.md"
 repository = "https://github.com/rigetti/pyquil.git"
 documentation = "https://pyquil-docs.rigetti.com"
 license = "Apache-2.0"
 classifiers = [
@@ -20,30 +20,31 @@
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.12"
 numpy = "^1.21"
 scipy = "^1.7.3"
 lark = "^0.11.1"
 rpcq = "^3.10.0"
+pydantic = "^1.10.7"
 networkx = "^2.5"
 importlib-metadata = { version = ">=3.7.3,<5", python = "<3.8" }
-qcs-sdk-python = "0.4.2"
-qcs-api-client = ">=0.21.0,<0.22.0"
+qcs-sdk-python = "0.5.0rc.17"
 retry = "^0.9.2"
 types-python-dateutil = "^2.8.19"
 types-retry = "^0.9.9"
 
 # latex extra
 ipython = { version = "^7.21.0", optional = true }
 
 # docs extra
 Sphinx = { version = "^4.0.2", optional = true }
 sphinx-rtd-theme = { version = "^0.5.2", optional = true }
 nbsphinx = { version = "^0.8.6", optional = true }
 recommonmark = { version = "^0.7.1", optional = true }
+pandoc = { version = "^2.3", optional = true }
 
 [tool.poetry.dev-dependencies]
 black = "^22.8.0"
 flake8 = "^3.8.1"
 pytest = "^6.2.2"
 pytest-cov = "^2.11.1"
 mypy = "0.981"
@@ -54,15 +55,15 @@
 pytest-freezegun = "^0.4.2"
 respx = "^0.20"
 nest-asyncio = "^1.5.6"
 mock = { version = "^4.0", python = "<3.8" }
 
 [tool.poetry.extras]
 latex = ["ipython"]
-docs = ["Sphinx", "sphinx-rtd-theme", "nbsphinx", "recommonmark"]
+docs = ["Sphinx", "sphinx-rtd-theme", "nbsphinx", "recommonmark", "pandoc"]
 
 [tool.black]
 line-length = 120
 target-version = ['py37']
 include = '\.pyi?$'
 exclude = '''
```

### Comparing `pyquil-4.0.0rc8/pyquil/_memory.py` & `pyquil-4.0.0rc9/pyquil/_memory.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/_parser/grammar.lark` & `pyquil-4.0.0rc9/pyquil/_parser/grammar.lark`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/_parser/parser.py` & `pyquil-4.0.0rc9/pyquil/_parser/parser.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/_version.py` & `pyquil-4.0.0rc9/pyquil/_version.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/api/__init__.py` & `pyquil-4.0.0rc9/pyquil/api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,26 +22,26 @@
     "BenchmarkConnection",
     "EncryptedProgram",
     "get_qc",
     "list_quantum_computers",
     "local_forest_runtime",
     "QAM",
     "QAMExecutionResult",
-    "QCSClientConfiguration",
+    "QCSClient",
     "QCSQuantumProcessor",
     "QPU",
     "QPUCompiler",
     "QuantumComputer",
     "QuantumExecutable",
     "QVM",
     "QVMCompiler",
     "WavefunctionSimulator",
 ]
 
-from qcs_api_client.client import QCSClientConfiguration
+from qcs_sdk import QCSClient
 
 from pyquil.api._benchmark import BenchmarkConnection
 from pyquil.api._compiler import QVMCompiler, QPUCompiler, QuantumExecutable, EncryptedProgram, AbstractCompiler
 from pyquil.api._qam import QAM, QAMExecutionResult
 from pyquil.api._qpu import QPU
 from pyquil.api._quantum_computer import (
     QuantumComputer,
```

### Comparing `pyquil-4.0.0rc8/pyquil/api/_benchmark.py` & `pyquil-4.0.0rc9/pyquil/api/_benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 ##############################################################################
 from typing import List, Optional, Sequence, cast
 
-from qcs_api_client.client import QCSClientConfiguration
+from qcs_sdk import QCSClient
 
 from pyquil.api._abstract_compiler import AbstractBenchmarker
 from pyquil.api._compiler_client import (
     GenerateRandomizedBenchmarkingSequenceRequest,
     ConjugatePauliByCliffordRequest,
     CompilerClient,
 )
@@ -30,24 +30,24 @@
 
 
 class BenchmarkConnection(AbstractBenchmarker):
     """
     Represents a connection to a server that generates benchmarking data.
     """
 
-    def __init__(self, *, timeout: float = 10.0, client_configuration: Optional[QCSClientConfiguration] = None):
+    def __init__(self, *, timeout: float = 10.0, client_configuration: Optional[QCSClient] = None):
         """
         Client to communicate with the benchmarking data endpoint.
 
         :param timeout: Time limit for requests, in seconds.
         :param client_configuration: Optional client configuration. If none is provided, a default one will be loaded.
         """
 
         self._compiler_client = CompilerClient(
-            client_configuration=client_configuration or QCSClientConfiguration.load(),
+            client_configuration=client_configuration or QCSClient.load(),
             request_timeout=timeout,
         )
 
     def apply_clifford_to_pauli(self, clifford: Program, pauli_in: PauliTerm) -> PauliTerm:
         r"""
         Given a circuit that consists only of elements of the Clifford group,
         return its action on a PauliTerm.
```

### Comparing `pyquil-4.0.0rc8/pyquil/api/_compiler.py` & `pyquil-4.0.0rc9/pyquil/api/_compiler.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,33 +9,27 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 ##############################################################################
-from contextlib import contextmanager
-from typing import Dict, Optional, Iterator
-import asyncio
+from typing import Dict, Optional
 
-import httpx
-from pyquil.parser import parse_program
-from pyquil.quilatom import MemoryReference
-from pyquil.quilbase import Declare
-import qcs_sdk
-from qcs_api_client.client import QCSClientConfiguration
-from qcs_api_client.operations.sync import (
-    get_quilt_calibrations,
-)
+from qcs_sdk import QCSClient
+from qcs_sdk.qpu.rewrite_arithmetic import rewrite_arithmetic
+from qcs_sdk.qpu.translation import get_quilt_calibrations, translate
 from rpcq.messages import ParameterSpec
 
-from pyquil.api._abstract_compiler import AbstractCompiler, QuantumExecutable, EncryptedProgram
-from pyquil.api._qcs_client import qcs_client
+from pyquil.api._abstract_compiler import AbstractCompiler, EncryptedProgram, QuantumExecutable
+from pyquil.parser import parse_program
 from pyquil.quantum_processor import AbstractQuantumProcessor
 from pyquil.quil import Program
+from pyquil.quilatom import MemoryReference
+from pyquil.quilbase import Declare
 
 
 class QPUCompilerNotRunning(Exception):
     pass
 
 
 def parse_mref(val: str) -> MemoryReference:
@@ -71,67 +65,59 @@
 
     def __init__(
         self,
         *,
         quantum_processor_id: str,
         quantum_processor: AbstractQuantumProcessor,
         timeout: float = 10.0,
-        client_configuration: Optional[QCSClientConfiguration] = None,
-        event_loop: Optional[asyncio.AbstractEventLoop] = None,
+        client_configuration: Optional[QCSClient] = None,
     ) -> None:
         """
         Instantiate a new QPU compiler client.
 
         :param quantum_processor_id: Processor to target.
         :param quantum_processor: Quantum processor to use as compilation target.
         :param timeout: Time limit for requests, in seconds.
         :param client_configuration: Optional client configuration. If none is provided, a default one will be loaded.
         """
         super().__init__(
             quantum_processor=quantum_processor,
             timeout=timeout,
             client_configuration=client_configuration,
-            event_loop=event_loop,
         )
 
         self.quantum_processor_id = quantum_processor_id
         self._calibration_program: Optional[Program] = None
 
     def native_quil_to_executable(self, nq_program: Program) -> QuantumExecutable:
         """
         Convert a native Quil program into an executable binary which can be executed by a QPU.
         """
-        rewrite_response = qcs_sdk.rewrite_arithmetic(nq_program.out())
+        rewrite_response = rewrite_arithmetic(nq_program.out())
 
-        # This is a work-around needed because calling `qcs_sdk.translate` happens _before_
-        # the event loop is available. Wrapping it in a Python async function ensures that
-        # the event loop is available. This is a limitation of pyo3:
-        # https://pyo3.rs/v0.17.1/ecosystem/async-await.html#a-note-about-asynciorun
-        async def _translate(*args):  # type: ignore
-            return await qcs_sdk.translate(*args)
-
-        translated_program = self._event_loop.run_until_complete(
-            _translate(  # type: ignore
-                rewrite_response["program"],
-                nq_program.num_shots,
-                self.quantum_processor_id,
-            )
+        translated_program = translate(
+            native_quil=rewrite_response.program,
+            num_shots=nq_program.num_shots,
+            quantum_processor_id=self.quantum_processor_id,
         )
 
+        ro_sources = translated_program.ro_sources or {}
+
         return EncryptedProgram(
-            program=translated_program["program"],
+            program=translated_program.program,
             memory_descriptors=_collect_memory_descriptors(nq_program),
-            ro_sources={parse_mref(mref): source for mref, source in translated_program["ro_sources"].items() or []},
-            recalculation_table=rewrite_response["recalculation_table"],
+            ro_sources={parse_mref(mref): source for mref, source in ro_sources.items() or []},
+            recalculation_table=rewrite_response.recalculation_table,
             _memory=nq_program._memory.copy(),
         )
 
     def _fetch_calibration_program(self) -> Program:
-        with self._qcs_client() as qcs_client:  # type: httpx.Client
-            response = get_quilt_calibrations(client=qcs_client, quantum_processor_id=self.quantum_processor_id).parsed
+        response = get_quilt_calibrations(
+            quantum_processor_id=self.quantum_processor_id,
+        )
         return parse_program(response.quilt)
 
     def get_calibration_program(self, force_refresh: bool = False) -> Program:
         """
         Get the Quil-T calibration program associated with the underlying QPU.
 
         This will return a cached copy of the calibration program if present.
@@ -157,44 +143,35 @@
     def reset(self) -> None:
         """
         Reset the state of the QPUCompiler.
         """
         super().reset()
         self._calibration_program = None
 
-    @contextmanager
-    def _qcs_client(self) -> Iterator[httpx.Client]:
-        with qcs_client(
-            client_configuration=self._client_configuration, request_timeout=self._timeout
-        ) as client:  # type: httpx.Client
-            yield client
-
 
 class QVMCompiler(AbstractCompiler):
     """
     Client to communicate with the compiler.
     """
 
     def __init__(
         self,
         *,
         quantum_processor: AbstractQuantumProcessor,
         timeout: float = 10.0,
-        client_configuration: Optional[QCSClientConfiguration] = None,
-        event_loop: Optional[asyncio.AbstractEventLoop] = None,
+        client_configuration: Optional[QCSClient] = None,
     ) -> None:
         """
         Client to communicate with compiler.
 
         :param quantum_processor: Quantum processor to use as compilation target.
         :param timeout: Number of seconds to wait for a response from the client.
         :param client_configuration: Optional client configuration. If none is provided, a default one will be loaded.
         """
         super().__init__(
             quantum_processor=quantum_processor,
             timeout=timeout,
             client_configuration=client_configuration,
-            event_loop=event_loop,
         )
 
     def native_quil_to_executable(self, nq_program: Program) -> QuantumExecutable:
         return nq_program
```

### Comparing `pyquil-4.0.0rc8/pyquil/api/_compiler_client.py` & `pyquil-4.0.0rc9/pyquil/api/_qvm_client.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,253 +9,287 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 ##############################################################################
-import asyncio
+import re
 from contextlib import contextmanager
 from dataclasses import dataclass
-from typing import Iterator, List, Optional
+from json.decoder import JSONDecodeError
+from typing import Iterator, Any, Dict, Union, Tuple, Optional, List, cast
 
-import qcs_sdk
-import rpcq
-from qcs_api_client.client import QCSClientConfiguration
-from rpcq.messages import TargetDevice as TargetQuantumProcessor
+import httpx
+
+from qcs_sdk import QCSClient
+
+from pyquil.api._errors import ApiError, UnknownApiError, TooManyQubitsError, error_mapping
 
 
 @dataclass
-class CompileToNativeQuilRequest:
+class RunProgramRequest:
     """
-    Request to compile to native Quil.
+    Request to run a Quil program.
     """
 
     program: str
-    """Program to compile."""
+    """Quil program to run."""
+
+    addresses: Dict[str, Union[bool, List[int]]]
+    """Memory addresses to be read and returned after execution. Mapped by region names to either:
+       - a numeric index, to return that particular value,
+       - `True` to return all memory in that region, or
+       - `False` to return no memory in that region (equivalent to missing entry)
+    """
 
-    target_quantum_processor: TargetQuantumProcessor
-    """Quantum processor to target."""
+    trials: int
+    """Number of times to run program and collect results."""
 
-    protoquil: Optional[bool]
-    """Whether or not to restrict to protoquil. Overrides server default when provided."""
+    measurement_noise: Optional[Tuple[float, float, float]]
+    """Simulated measurement noise for X, Y, and Z axes."""
+
+    gate_noise: Optional[Tuple[float, float, float]]
+    """Simulated gate noise for X, Y, and Z axes."""
+
+    seed: Optional[int]
+    """PRNG seed. Set this to guarantee repeatable results."""
 
 
 @dataclass
-class NativeQuilMetadataResponse:
+class RunProgramResponse:
     """
-    Metadata for a native Quil program.
+    Program run response.
     """
 
-    final_rewiring: List[int]
-    """Output qubit index relabeling due to SWAP insertion."""
+    results: Dict[str, List[List[int]]]
+    """Run results, by memory region name. Values are multi-dimensional arrays of size <trials>-by-<slots>."""
 
-    gate_depth: Optional[int]
-    """Maximum number of successive gates in the native Quil program."""
 
-    gate_volume: Optional[int]
-    """Total number of gates in the native Quil program."""
+@dataclass
+class RunAndMeasureProgramRequest:
+    """
+    Request to run and measure a Quil program.
+    """
 
-    multiqubit_gate_depth: Optional[int]
-    """Maximum number of successive two-qubit gates in the native Quil program."""
+    program: str
+    """Quil program to run."""
 
-    program_duration: Optional[float]
-    """Rough estimate of native Quil program length in nanoseconds."""
+    qubits: List[int]
+    """Qubits to measure."""
 
-    program_fidelity: Optional[float]
-    """Rough estimate of the fidelity of the full native Quil program."""
+    trials: int
+    """Number of times to run program and collect results."""
 
-    topological_swaps: Optional[int]
-    """Total number of SWAPs in the native Quil program."""
+    measurement_noise: Optional[Tuple[float, float, float]]
+    """Simulated measurement noise for X, Y, and Z axes."""
 
-    qpu_runtime_estimation: Optional[float]
-    """
-    The estimated runtime (milliseconds) on a Rigetti QPU (protoquil program). Available only for protoquil-compliant
-    programs.
-    """
+    gate_noise: Optional[Tuple[float, float, float]]
+    """Simulated gate noise for X, Y, and Z axes."""
+
+    seed: Optional[int]
+    """PRNG seed. Set this to guarantee repeatable results."""
 
 
 @dataclass
-class CompileToNativeQuilResponse:
+class RunAndMeasureProgramResponse:
     """
-    Compile to native Quil response.
+    Program run and measure response.
     """
 
-    native_program: str
-    """Native Quil program."""
-
-    metadata: Optional[NativeQuilMetadataResponse]
-    """Metadata for the returned Native Quil."""
+    results: List[List[int]]
+    """Resulting memory region value, a multi-dimensional array of size <trials>-by-<slots>."""
 
 
 @dataclass
-class ConjugatePauliByCliffordRequest:
+class MeasureExpectationRequest:
     """
-    Request to conjugate a Pauli element by a Clifford element.
+    Request to measure expectations of Pauli operators.
     """
 
-    pauli_indices: List[int]
-    """Qubit indices onto which the factors of the Pauli term are applied."""
+    prep_program: str
+    """Quil program to place QVM into a desired state before expectation measurement."""
 
-    pauli_symbols: List[str]
-    """Ordered factors of the Pauli term."""
+    pauli_operators: List[str]
+    """Quil programs representing Pauli operators for which to measure expectations."""
 
-    clifford: str
-    """Clifford element."""
+    seed: Optional[int]
+    """PRNG seed. Set this to guarantee repeatable results."""
 
 
 @dataclass
-class ConjugatePauliByCliffordResponse:
+class MeasureExpectationResponse:
     """
-    Conjugate Pauli by Clifford response.
+    Expectation measurement response.
     """
 
-    phase_factor: int
-    """Encoded global phase factor on the emitted Pauli."""
-
-    pauli: str
-    """Description of the encoded Pauli."""
+    expectations: List[float]
+    """Measured expectations, one for each Pauli operator in original request."""
 
 
 @dataclass
-class GenerateRandomizedBenchmarkingSequenceRequest:
+class GetWavefunctionRequest:
     """
-    Request to generate a randomized benchmarking sequence.
+    Request to run a program and retrieve the resulting wavefunction.
     """
 
-    depth: int
-    """Depth of the benchmarking sequence."""
+    program: str
+    """Quil program to run."""
 
-    num_qubits: int
-    """Number of qubits involved in the benchmarking sequence."""
+    measurement_noise: Optional[Tuple[float, float, float]]
+    """Simulated measurement noise for X, Y, and Z axes."""
 
-    gateset: List[str]
-    """List of Quil programs, each describing a Clifford."""
+    gate_noise: Optional[Tuple[float, float, float]]
+    """Simulated gate noise for X, Y, and Z axes."""
 
     seed: Optional[int]
     """PRNG seed. Set this to guarantee repeatable results."""
 
-    interleaver: Optional[str]
-    """Fixed Clifford, specified as a Quil string, to interleave through an RB sequence."""
-
 
 @dataclass
-class GenerateRandomizedBenchmarkingSequenceResponse:
+class GetWavefunctionResponse:
     """
-    Randomly generated benchmarking sequence response.
+    Get wavefunction response.
     """
 
-    sequence: List[List[int]]
-    """List of Cliffords, each expressed as a list of generator indices."""
+    wavefunction: bytes
+    """Bit-packed wavefunction string."""
 
 
-class CompilerClient:
+class QVMClient:
     """
-    Client for making requests to a Quil compiler.
+    Client for making requests to a Quantum Virtual Machine.
     """
 
-    def __init__(
-        self,
-        *,
-        client_configuration: QCSClientConfiguration,
-        request_timeout: float = 10.0,
-        event_loop: Optional[asyncio.AbstractEventLoop] = None,
-    ) -> None:
+    def __init__(self, *, client_configuration: QCSClient, request_timeout: float = 10.0) -> None:
         """
         Instantiate a new compiler client.
 
         :param client_configuration: Configuration for client.
         :param request_timeout: Timeout for requests, in seconds.
         """
-        base_url = client_configuration.profile.applications.pyquil.quilc_url
-        if not base_url.startswith("tcp://"):
-            raise ValueError(f"Expected compiler URL '{base_url}' to start with 'tcp://'")
-
-        self.base_url = base_url
+        self.base_url = client_configuration.qvm_url
         self.timeout = request_timeout
-        if event_loop is None:
-            event_loop = asyncio.get_event_loop()
-        self._event_loop = event_loop
 
     def get_version(self) -> str:
         """
-        Get version info for compiler server.
+        Get version info for QVM server.
+        """
+        return self._post_json({"type": "version"}).text.split()[0]
+
+    def run_program(self, request: RunProgramRequest) -> RunProgramResponse:
+        """
+        Run a Quil program and return its results.
         """
+        payload: Dict[str, Any] = {
+            "type": "multishot",
+            "compiled-quil": request.program,
+            "addresses": request.addresses,
+            "trials": request.trials,
+        }
 
-        async def _get_quilc_version() -> str:
-            return await qcs_sdk.get_quilc_version()
+        if request.measurement_noise is not None:
+            payload["measurement-noise"] = request.measurement_noise
 
-        return self._event_loop.run_until_complete(_get_quilc_version())
+        if request.gate_noise is not None:
+            payload["gate-noise"] = request.gate_noise
 
-    def compile_to_native_quil(self, request: CompileToNativeQuilRequest) -> CompileToNativeQuilResponse:
-        """
-        Compile Quil program to native Quil.
-        """
-        rpcq_request = rpcq.messages.NativeQuilRequest(
-            quil=request.program,
-            target_device=request.target_quantum_processor,
-        )
-        with self._rpcq_client() as rpcq_client:  # type: rpcq.Client
-            response: rpcq.messages.NativeQuilResponse = rpcq_client.call(
-                "quil_to_native_quil",
-                rpcq_request,
-                protoquil=request.protoquil,
-            )
-            metadata: Optional[NativeQuilMetadataResponse] = None
-            if response.metadata is not None:
-                metadata = NativeQuilMetadataResponse(
-                    final_rewiring=response.metadata.final_rewiring,
-                    gate_depth=response.metadata.gate_depth,
-                    gate_volume=response.metadata.gate_volume,
-                    multiqubit_gate_depth=response.metadata.multiqubit_gate_depth,
-                    program_duration=response.metadata.program_duration,
-                    program_fidelity=response.metadata.program_fidelity,
-                    topological_swaps=response.metadata.topological_swaps,
-                    qpu_runtime_estimation=response.metadata.qpu_runtime_estimation,
-                )
-            return CompileToNativeQuilResponse(native_program=response.quil, metadata=metadata)
-
-    def conjugate_pauli_by_clifford(self, request: ConjugatePauliByCliffordRequest) -> ConjugatePauliByCliffordResponse:
-        """
-        Conjugate a Pauli element by a Clifford element.
-        """
-        rpcq_request = rpcq.messages.ConjugateByCliffordRequest(
-            pauli=rpcq.messages.PauliTerm(indices=request.pauli_indices, symbols=request.pauli_symbols),
-            clifford=request.clifford,
-        )
-        with self._rpcq_client() as rpcq_client:  # type: rpcq.Client
-            response: rpcq.messages.ConjugateByCliffordResponse = rpcq_client.call(
-                "conjugate_pauli_by_clifford",
-                rpcq_request,
-            )
-            return ConjugatePauliByCliffordResponse(phase_factor=response.phase, pauli=response.pauli)
-
-    def generate_randomized_benchmarking_sequence(
-        self, request: GenerateRandomizedBenchmarkingSequenceRequest
-    ) -> GenerateRandomizedBenchmarkingSequenceResponse:
-        """
-        Generate a randomized benchmarking sequence.
-        """
-        rpcq_request = rpcq.messages.RandomizedBenchmarkingRequest(
-            depth=request.depth,
-            qubits=request.num_qubits,
-            gateset=request.gateset,
-            seed=request.seed,
-            interleaver=request.interleaver,
-        )
-        with self._rpcq_client() as rpcq_client:  # type: rpcq.Client
-            response: rpcq.messages.RandomizedBenchmarkingResponse = rpcq_client.call(
-                "generate_rb_sequence",
-                rpcq_request,
-            )
-            return GenerateRandomizedBenchmarkingSequenceResponse(sequence=response.sequence)
+        if request.seed is not None:
+            payload["rng-seed"] = request.seed
+
+        return RunProgramResponse(results=cast(Dict[str, List[List[int]]], self._post_json(payload).json()))
+
+    def run_and_measure_program(self, request: RunAndMeasureProgramRequest) -> RunAndMeasureProgramResponse:
+        """
+        Run and measure a Quil program, and return its results.
+        """
+        payload: Dict[str, Any] = {
+            "type": "multishot-measure",
+            "compiled-quil": request.program,
+            "qubits": request.qubits,
+            "trials": request.trials,
+        }
+
+        if request.measurement_noise is not None:
+            payload["measurement-noise"] = request.measurement_noise
+
+        if request.gate_noise is not None:
+            payload["gate-noise"] = request.gate_noise
+
+        if request.seed is not None:
+            payload["rng-seed"] = request.seed
+
+        return RunAndMeasureProgramResponse(results=cast(List[List[int]], self._post_json(payload).json()))
+
+    def measure_expectation(self, request: MeasureExpectationRequest) -> MeasureExpectationResponse:
+        """
+        Measure expectation value of Pauli operators given a defined state.
+        """
+        payload: Dict[str, Any] = {
+            "type": "expectation",
+            "state-preparation": request.prep_program,
+            "operators": request.pauli_operators,
+        }
+
+        if request.seed is not None:
+            payload["rng-seed"] = request.seed
+
+        return MeasureExpectationResponse(expectations=cast(List[float], self._post_json(payload).json()))
+
+    def get_wavefunction(self, request: GetWavefunctionRequest) -> GetWavefunctionResponse:
+        """
+        Run a program and retrieve the resulting wavefunction.
+        """
+        payload: Dict[str, Any] = {
+            "type": "wavefunction",
+            "compiled-quil": request.program,
+        }
+
+        if request.measurement_noise is not None:
+            payload["measurement-noise"] = request.measurement_noise
+
+        if request.gate_noise is not None:
+            payload["gate-noise"] = request.gate_noise
+
+        if request.seed is not None:
+            payload["rng-seed"] = request.seed
+
+        return GetWavefunctionResponse(wavefunction=self._post_json(payload).content)
+
+    def _post_json(self, json: Dict[str, Any]) -> httpx.Response:
+        with self._http_client() as http:  # type: httpx.Client
+            response = http.post("/", json=json)
+            if response.status_code >= 400:
+                raise self._parse_error(response)
+        return response
 
     @contextmanager
-    def _rpcq_client(self) -> Iterator[rpcq.Client]:
-        client = rpcq.Client(
-            endpoint=self.base_url,
-            timeout=self.timeout,
-        )
-        try:
+    def _http_client(self) -> Iterator[httpx.Client]:
+        with httpx.Client(base_url=self.base_url, timeout=self.timeout) as client:
             yield client
-        finally:
-            client.close()  # type: ignore
+
+    @staticmethod
+    def _parse_error(res: httpx.Response) -> ApiError:
+        """
+        Errors should contain a "status" field with a human readable explanation of
+        what went wrong as well as a "error_type" field indicating the kind of error that can be mapped
+        to a Python type.
+
+        There's a fallback error UnknownApiError for other types of exceptions (network issues, api
+        gateway problems, etc.)
+        """
+        try:
+            body = res.json()
+        except JSONDecodeError:
+            raise UnknownApiError(res.text)
+
+        if "error_type" not in body:
+            raise UnknownApiError(str(body))
+
+        error_type = body["error_type"]
+        status = body["status"]
+
+        if re.search(r"[0-9]+ qubits were requested, but the QVM is limited to [0-9]+ qubits.", status):
+            return TooManyQubitsError(status)
+
+        error_cls = error_mapping.get(error_type, UnknownApiError)
+        return error_cls(status)
```

### Comparing `pyquil-4.0.0rc8/pyquil/api/_errors.py` & `pyquil-4.0.0rc9/pyquil/api/_errors.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/api/_logger.py` & `pyquil-4.0.0rc9/pyquil/api/_logger.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/api/_qam.py` & `pyquil-4.0.0rc9/pyquil/api/_qam.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/api/_qpu.py` & `pyquil-4.0.0rc9/pyquil/api/_qpu.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,44 +10,44 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 ##############################################################################
 from dataclasses import dataclass
-import asyncio
 from collections import defaultdict
-from typing import Dict, Optional
+from typing import Dict, Optional, Union
 
 import numpy as np
-from qcs_api_client.client import QCSClientConfiguration
+from numpy.typing import NDArray
 from rpcq.messages import ParameterSpec
 
 from pyquil.api import QuantumExecutable, EncryptedProgram
 
 from pyquil.api._qam import QAM, QAMExecutionResult
 from pyquil.quilatom import (
     MemoryReference,
 )
-import qcs_sdk
+from qcs_sdk import QCSClient
+from qcs_sdk.qpu.api import submit, retrieve_results, ExecutionResult
+from qcs_sdk.qpu.rewrite_arithmetic import build_patch_values
 
 
-def decode_buffer(buffer: "qcs_sdk.ExecutionResult") -> np.ndarray:
+def decode_buffer(buffer: ExecutionResult) -> Union[NDArray[np.complex64], NDArray[np.int32]]:
     """
     Translate a DataBuffer into a numpy array.
 
     :param buffer: Dictionary with 'data' byte array, 'dtype', and 'shape' fields
     :return: NumPy array of decoded data
     """
-    if buffer["dtype"] == "complex":
-        buffer["data"] = [complex(re, im) for re, im in buffer["data"]]  # type: ignore
-        buffer["dtype"] = np.complex64  # type: ignore
-    elif buffer["dtype"] == "integer":
-        buffer["dtype"] = np.int32  # type: ignore
-    return np.array(buffer["data"], dtype=buffer["dtype"])
+    if buffer.dtype == "complex":
+        return np.array(buffer.data.to_complex32(), dtype=np.complex64)
+    elif buffer.dtype == "integer":
+        return np.array(buffer.data.to_i32(), dtype=np.int32)
+    return np.array([], np.int32)
 
 
 def _extract_memory_regions(
     memory_descriptors: Dict[str, ParameterSpec],
     ro_sources: Dict[MemoryReference, str],
     buffers: Dict[str, np.ndarray],
 ) -> Dict[str, np.ndarray]:
@@ -107,17 +107,16 @@
 class QPU(QAM[QPUExecuteResponse]):
     def __init__(
         self,
         *,
         quantum_processor_id: str,
         priority: int = 1,
         timeout: float = 10.0,
-        client_configuration: Optional[QCSClientConfiguration] = None,
+        client_configuration: Optional[QCSClient] = None,
         endpoint_id: Optional[str] = None,
-        event_loop: Optional[asyncio.AbstractEventLoop] = None,
         use_gateway: bool = True,
     ) -> None:
         """
         A connection to the QPU.
 
         :param quantum_processor_id: Processor to run against.
         :param priority: The priority with which to insert jobs into the QPU queue. Lower integers
@@ -127,23 +126,20 @@
         :param endpoint_id: Optional endpoint ID to be used for execution.
         :param use_gateway: Disable to skip the Gateway server and perform direct execution.
         """
         super().__init__()
 
         self.priority = priority
 
-        client_configuration = client_configuration or QCSClientConfiguration.load()
+        self._client_configuration = client_configuration or QCSClient.load()
         self._last_results: Dict[str, np.ndarray] = {}
         self._memory_results: Dict[str, Optional[np.ndarray]] = defaultdict(lambda: None)
         self._quantum_processor_id = quantum_processor_id
         self._endpoint_id = endpoint_id
 
-        if event_loop is None:
-            event_loop = asyncio.get_event_loop()
-        self._event_loop = event_loop
         self._use_gateway = use_gateway
 
     @property
     def quantum_processor_id(self) -> str:
         """ID of quantum processor targeted."""
         return self._quantum_processor_id
 
@@ -165,48 +161,48 @@
 
         # executable._memory.values is a dict of ParameterARef -> numbers,
         # where ParameterARef is data class w/ name and index
         # ParameterARef == Parameter on the Rust side
         mem_values = defaultdict(list)
         for k, v in executable._memory.values.items():
             mem_values[k.name].append(v)
-        patch_values = qcs_sdk.build_patch_values(executable.recalculation_table, mem_values)
+        patch_values = build_patch_values(executable.recalculation_table, mem_values)
 
-        async def _submit(*args) -> str:  # type: ignore
-            return await qcs_sdk.submit(*args)
-
-        job_id = self._event_loop.run_until_complete(
-            _submit(executable.program, patch_values, self.quantum_processor_id, self._use_gateway)
+        job_id = submit(
+            program=executable.program,
+            patch_values=patch_values,
+            quantum_processor_id=self.quantum_processor_id,
+            endpoint_id=self._endpoint_id,
+            client=self._client_configuration,
         )
 
         return QPUExecuteResponse(_executable=executable, job_id=job_id)
 
     def get_result(self, execute_response: QPUExecuteResponse) -> QAMExecutionResult:
         """
         Retrieve results from execution on the QPU.
         """
 
-        async def _get_result(*args):  # type: ignore
-            return await qcs_sdk.retrieve_results(*args)
-
-        results = self._event_loop.run_until_complete(
-            _get_result(execute_response.job_id, self.quantum_processor_id, self._use_gateway)  # type: ignore
+        results = retrieve_results(
+            job_id=execute_response.job_id,
+            quantum_processor_id=self.quantum_processor_id,
+            client=self._client_configuration,
         )
 
         ro_sources = execute_response._executable.ro_sources
-        decoded_buffers = {k: decode_buffer(v) for k, v in results["buffers"].items()}
+        decoded_buffers = {k: decode_buffer(v) for k, v in results.buffers.items()}
 
         result_memory = {}
         if len(decoded_buffers) != 0:
             extracted = _extract_memory_regions(
                 execute_response._executable.memory_descriptors, ro_sources, decoded_buffers
             )
             for name, array in extracted.items():
                 result_memory[name] = array
         elif not ro_sources:
             result_memory["ro"] = np.zeros((0, 0), dtype=np.int64)
 
         return QAMExecutionResult(
             executable=execute_response._executable,
             readout_data=result_memory,
-            execution_duration_microseconds=results["execution_duration_microseconds"],
+            execution_duration_microseconds=results.execution_duration_microseconds,
         )
```

### Comparing `pyquil-4.0.0rc8/pyquil/api/_quantum_computer.py` & `pyquil-4.0.0rc9/pyquil/api/_quantum_computer.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 ##############################################################################
-import asyncio
 import itertools
 import re
 import socket
 import subprocess
 import warnings
 from contextlib import contextmanager
 from math import pi, log
@@ -28,29 +27,27 @@
     Mapping,
     Optional,
     Sequence,
     Set,
     Union,
     cast,
     List,
-    TYPE_CHECKING,
 )
 
 import networkx as nx
 import numpy as np
-from qcs_api_client.client import QCSClientConfiguration
-from qcs_api_client.models import ListQuantumProcessorsResponse
-from qcs_api_client.operations.sync import list_quantum_processors
 from rpcq.messages import ParameterAref
 
+from qcs_sdk import QCSClient
+from qcs_sdk.qpu import list_quantum_processors
+
 from pyquil.api._abstract_compiler import AbstractCompiler, QuantumExecutable
 from pyquil.api._compiler import QPUCompiler, QVMCompiler
 
 from pyquil.api._qam import QAM, QAMExecutionResult
-from pyquil.api._qcs_client import qcs_client
 from pyquil.api._qpu import QPU
 from pyquil.api._qvm import QVM
 from pyquil.experiment._main import Experiment
 from pyquil.experiment._memory import merge_memory_map_lists
 from pyquil.experiment._result import ExperimentResult, bitstrings_to_expectations
 from pyquil.experiment._setting import ExperimentSetting
 from pyquil.external.rpcq import CompilerISA
@@ -62,17 +59,14 @@
     AbstractQuantumProcessor,
     QCSQuantumProcessor,
     NxQuantumProcessor,
     get_qcs_quantum_processor,
 )
 from pyquil.quil import Program
 
-if TYPE_CHECKING:
-    import httpx
-
 
 class QuantumComputer:
     def __init__(
         self,
         *,
         name: str,
         qam: QAM[Any],
@@ -412,33 +406,28 @@
         return f'QuantumComputer[name="{self.name}"]'
 
 
 def list_quantum_computers(
     qpus: bool = True,
     qvms: bool = True,
     timeout: float = 10.0,
-    client_configuration: Optional[QCSClientConfiguration] = None,
+    client_configuration: Optional[QCSClient] = None,
 ) -> List[str]:
     """
     List the names of available quantum computers
 
     :param qpus: Whether to include QPUs in the list.
     :param qvms: Whether to include QVMs in the list.
     :param timeout: Time limit for request, in seconds.
     :param client_configuration: Optional client configuration. If none is provided, a default one will be loaded.
     """
-    client_configuration = client_configuration or QCSClientConfiguration.load()
+    client_configuration = client_configuration or QCSClient.load()
     qc_names: List[str] = []
     if qpus:
-        with qcs_client(
-            client_configuration=client_configuration, request_timeout=timeout
-        ) as client:  # type: httpx.Client
-            qcs: ListQuantumProcessorsResponse = list_quantum_processors(client=client, page_size=100).parsed
-
-        qc_names += [qc.id for qc in qcs.quantum_processors]
+        qc_names += list_quantum_processors(client=client_configuration, timeout=timeout)
 
     if qvms:
         qc_names += ["9q-square-qvm", "9q-square-noisy-qvm"]
 
     return qc_names
 
 
@@ -506,15 +495,15 @@
 
     name = f"{prefix}{noise_suffix}{qvm_suffix}"
     return name
 
 
 def _get_qvm_or_pyqvm(
     *,
-    client_configuration: QCSClientConfiguration,
+    client_configuration: QCSClient,
     qvm_type: str,
     noise_model: Optional[NoiseModel],
     quantum_processor: Optional[AbstractQuantumProcessor],
     execution_timeout: float,
 ) -> Union[QVM, PyQVM]:
     if qvm_type == "qvm":
         return QVM(noise_model=noise_model, timeout=execution_timeout, client_configuration=client_configuration)
@@ -523,22 +512,21 @@
         return PyQVM(n_qubits=quantum_processor.qubit_topology().number_of_nodes())
 
     raise ValueError("Unknown qvm type {}".format(qvm_type))
 
 
 def _get_qvm_qc(
     *,
-    client_configuration: QCSClientConfiguration,
+    client_configuration: QCSClient,
     name: str,
     qvm_type: str,
     quantum_processor: AbstractQuantumProcessor,
     compiler_timeout: float,
     execution_timeout: float,
     noise_model: Optional[NoiseModel],
-    event_loop: Optional[asyncio.AbstractEventLoop] = None,
 ) -> QuantumComputer:
     """Construct a QuantumComputer backed by a QVM.
 
     This is a minimal wrapper over the QuantumComputer, QVM, and QVMCompiler constructors.
 
     :param client_configuration: Client configuration.
     :param name: A string identifying this particular quantum computer.
@@ -559,29 +547,27 @@
             quantum_processor=quantum_processor,
             execution_timeout=execution_timeout,
         ),
         compiler=QVMCompiler(
             quantum_processor=quantum_processor,
             timeout=compiler_timeout,
             client_configuration=client_configuration,
-            event_loop=event_loop,
         ),
     )
 
 
 def _get_qvm_with_topology(
     *,
-    client_configuration: QCSClientConfiguration,
+    client_configuration: QCSClient,
     name: str,
     topology: nx.Graph,
     noisy: bool,
     qvm_type: str,
     compiler_timeout: float,
     execution_timeout: float,
-    event_loop: Optional[asyncio.AbstractEventLoop] = None,
 ) -> QuantumComputer:
     """Construct a QVM with the provided topology.
 
     :param client_configuration: Client configuration.
     :param name: A name for your quantum computer. This field does not affect behavior of the
         constructed QuantumComputer.
     :param topology: A graph representing the desired qubit connectivity.
@@ -605,27 +591,25 @@
         client_configuration=client_configuration,
         name=name,
         qvm_type=qvm_type,
         quantum_processor=quantum_processor,
         noise_model=noise_model,
         compiler_timeout=compiler_timeout,
         execution_timeout=execution_timeout,
-        event_loop=event_loop,
     )
 
 
 def _get_9q_square_qvm(
     *,
-    client_configuration: QCSClientConfiguration,
+    client_configuration: QCSClient,
     name: str,
     noisy: bool,
     qvm_type: str,
     compiler_timeout: float,
     execution_timeout: float,
-    event_loop: Optional[asyncio.AbstractEventLoop] = None,
 ) -> QuantumComputer:
     """
     A nine-qubit 3x3 square lattice.
 
     This uses a "generic" lattice not tied to any specific quantum_processor. 9 qubits is large enough
     to do vaguely interesting algorithms and small enough to simulate quickly.
 
@@ -642,28 +626,26 @@
         client_configuration=client_configuration,
         name=name,
         topology=topology,
         noisy=noisy,
         qvm_type=qvm_type,
         compiler_timeout=compiler_timeout,
         execution_timeout=execution_timeout,
-        event_loop=event_loop,
     )
 
 
 def _get_unrestricted_qvm(
     *,
-    client_configuration: QCSClientConfiguration,
+    client_configuration: QCSClient,
     name: str,
     noisy: bool,
     n_qubits: int,
     qvm_type: str,
     compiler_timeout: float,
     execution_timeout: float,
-    event_loop: Optional[asyncio.AbstractEventLoop] = None,
 ) -> QuantumComputer:
     """
     A qvm with a fully-connected topology.
 
     This is obviously the least realistic QVM, but who am I to tell users what they want.
 
     :param client_configuration: Client configuration.
@@ -680,28 +662,26 @@
         client_configuration=client_configuration,
         name=name,
         topology=topology,
         noisy=noisy,
         qvm_type=qvm_type,
         compiler_timeout=compiler_timeout,
         execution_timeout=execution_timeout,
-        event_loop=event_loop,
     )
 
 
 def _get_qvm_based_on_real_quantum_processor(
     *,
-    client_configuration: QCSClientConfiguration,
+    client_configuration: QCSClient,
     name: str,
     quantum_processor: QCSQuantumProcessor,
     noisy: bool,
     qvm_type: str,
     compiler_timeout: float,
     execution_timeout: float,
-    event_loop: Optional[asyncio.AbstractEventLoop] = None,
 ) -> QuantumComputer:
     """
     A qvm with a based on a real quantum_processor.
 
     This is the most realistic QVM.
 
     :param client_configuration: Client configuration.
@@ -722,28 +702,26 @@
         client_configuration=client_configuration,
         name=name,
         quantum_processor=quantum_processor,
         noise_model=noise_model,
         qvm_type=qvm_type,
         compiler_timeout=compiler_timeout,
         execution_timeout=execution_timeout,
-        event_loop=event_loop,
     )
 
 
 def get_qc(
     name: str,
     *,
     as_qvm: Optional[bool] = None,
     noisy: Optional[bool] = None,
     compiler_timeout: float = 30.0,
     execution_timeout: float = 30.0,
-    client_configuration: Optional[QCSClientConfiguration] = None,
+    client_configuration: Optional[QCSClient] = None,
     endpoint_id: Optional[str] = None,
-    event_loop: Optional[asyncio.AbstractEventLoop] = None,
 ) -> QuantumComputer:
     """
     Get a quantum computer.
 
     A quantum computer is an object of type :py:class:`QuantumComputer` and can be backed
     either by a QVM simulator ("Quantum/Quil Virtual Machine") or a physical Rigetti QPU ("Quantum
     Processing Unit") made of superconducting qubits.
@@ -813,18 +791,15 @@
     :param endpoint_id: Optional quantum processor endpoint ID, as used in the `QCS API Docs`_.
 
     :return: A pre-configured QuantumComputer
 
     .. _QCS API Docs: https://docs.api.qcs.rigetti.com/#tag/endpoints
     """
 
-    client_configuration = client_configuration or QCSClientConfiguration.load()
-
-    if event_loop is None:
-        event_loop = asyncio.get_event_loop()
+    client_configuration = client_configuration or QCSClient.load()
 
     # 1. Parse name, check for redundant options, canonicalize names.
     prefix, qvm_type, noisy = _parse_name(name, as_qvm, noisy)
     del as_qvm  # do not use after _parse_name
     name = _canonicalize_name(prefix, qvm_type, noisy)
 
     # 2. Check for unrestricted {n}q-qvm
@@ -837,29 +812,27 @@
             client_configuration=client_configuration,
             name=name,
             noisy=noisy,
             n_qubits=n_qubits,
             qvm_type=qvm_type,
             compiler_timeout=compiler_timeout,
             execution_timeout=execution_timeout,
-            event_loop=event_loop,
         )
 
     # 3. Check for "9q-square" qvm
     if prefix == "9q-square":
         if qvm_type is None:
             raise ValueError("The quantum_processor '9q-square' is only available as a QVM")
         return _get_9q_square_qvm(
             client_configuration=client_configuration,
             name=name,
             noisy=noisy,
             qvm_type=qvm_type,
             compiler_timeout=compiler_timeout,
             execution_timeout=execution_timeout,
-            event_loop=event_loop,
         )
 
     if noisy:
         raise ValueError(
             "pyQuil currently does not support initializing a noisy QuantumComputer "
             "based on a QCSQuantumProcessor. Change noisy to False or specify the name of a QVM."
         )
@@ -874,30 +847,27 @@
             client_configuration=client_configuration,
             name=name,
             quantum_processor=quantum_processor,
             noisy=False,
             qvm_type=qvm_type,
             compiler_timeout=compiler_timeout,
             execution_timeout=execution_timeout,
-            event_loop=event_loop,
         )
     else:
         qpu = QPU(
             quantum_processor_id=quantum_processor.quantum_processor_id,
             timeout=execution_timeout,
             client_configuration=client_configuration,
             endpoint_id=endpoint_id,
-            event_loop=event_loop,
         )
         compiler = QPUCompiler(
             quantum_processor_id=prefix,
             quantum_processor=quantum_processor,
             timeout=compiler_timeout,
             client_configuration=client_configuration,
-            event_loop=event_loop,
         )
 
         return QuantumComputer(name=name, qam=qpu, compiler=compiler)
 
 
 def _port_used(host: str, port: int) -> bool:
     """Check if a (TCP) port is listening.
```

### Comparing `pyquil-4.0.0rc8/pyquil/api/_qvm.py` & `pyquil-4.0.0rc9/pyquil/api/_qvm.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 ##############################################################################
 from dataclasses import dataclass
 from typing import Dict, Mapping, Optional, Sequence, Union, Tuple
 
 import numpy as np
-from qcs_api_client.client import QCSClientConfiguration
+
+from qcs_sdk import QCSClient
 
 from pyquil._version import pyquil_version
 from pyquil.api import QuantumExecutable
 from pyquil.api._qam import QAM, QAMExecutionResult
 from pyquil.api._qvm_client import (
     QVMClient,
     RunProgramRequest,
@@ -61,15 +62,15 @@
     def __init__(
         self,
         noise_model: Optional[NoiseModel] = None,
         gate_noise: Optional[Tuple[float, float, float]] = None,
         measurement_noise: Optional[Tuple[float, float, float]] = None,
         random_seed: Optional[int] = None,
         timeout: float = 10.0,
-        client_configuration: Optional[QCSClientConfiguration] = None,
+        client_configuration: Optional[QCSClient] = None,
     ) -> None:
         """
         A virtual machine that classically emulates the execution of Quil programs.
 
         :param noise_model: A noise model that describes noise to apply when emulating a program's
             execution.
         :param gate_noise: A tuple of three numbers [Px, Py, Pz] indicating the probability of an X,
@@ -107,15 +108,15 @@
         if random_seed is None:
             self.random_seed = None
         elif isinstance(random_seed, int) and random_seed >= 0:
             self.random_seed = random_seed
         else:
             raise TypeError("random_seed should be None or a non-negative int")
 
-        client_configuration = client_configuration or QCSClientConfiguration.load()
+        client_configuration = client_configuration or QCSClient.load()
         self._qvm_client = QVMClient(client_configuration=client_configuration, request_timeout=timeout)
         self.connect()
 
     def connect(self) -> None:
         try:
             version = self.get_version_info()
             check_qvm_version(version)
```

### Comparing `pyquil-4.0.0rc8/pyquil/api/_rewrite_arithmetic.py` & `pyquil-4.0.0rc9/pyquil/api/_rewrite_arithmetic.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/api/_wavefunction_simulator.py` & `pyquil-4.0.0rc9/pyquil/api/_wavefunction_simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 ##############################################################################
 import warnings
 from typing import Dict, List, Union, Optional, Set, cast, Iterable, Sequence, Tuple
 
 import numpy as np
-from qcs_api_client.client import QCSClientConfiguration
 
+from qcs_sdk import QCSClient
 
 from pyquil.api._qvm import (
     validate_qubit_list,
     validate_noise_probabilities,
 )
 from pyquil.api._qvm_client import (
     MeasureExpectationRequest,
@@ -41,15 +41,15 @@
     def __init__(
         self,
         *,
         gate_noise: Optional[Tuple[float, float, float]] = None,
         measurement_noise: Optional[Tuple[float, float, float]] = None,
         random_seed: Optional[int] = None,
         timeout: float = 10.0,
-        client_configuration: Optional[QCSClientConfiguration] = None,
+        client_configuration: Optional[QCSClient] = None,
     ) -> None:
         """
         A simulator that propagates a wavefunction representation of a quantum state.
 
         :param gate_noise: A tuple of three numbers [Px, Py, Pz] indicating the probability of an X,
             Y, or Z gate getting applied to each qubit after a gate application or reset.
         :param measurement_noise: A tuple of three numbers [Px, Py, Pz] indicating the probability
@@ -68,15 +68,15 @@
         if random_seed is None:
             self.random_seed = None
         elif isinstance(random_seed, int) and random_seed >= 0:
             self.random_seed = random_seed
         else:
             raise TypeError("random_seed should be None or a non-negative int")
 
-        client_configuration = client_configuration or QCSClientConfiguration.load()
+        client_configuration = client_configuration or QCSClient.load()
         self._qvm_client = QVMClient(client_configuration=client_configuration, request_timeout=timeout)
 
     def wavefunction(
         self, quil_program: Program, memory_map: Optional[Dict[str, List[Union[int, float]]]] = None
     ) -> Wavefunction:
         """
         Simulate a Quil program and return the wavefunction.
```

### Comparing `pyquil-4.0.0rc8/pyquil/compatibility/__init__.py` & `pyquil-4.0.0rc9/pyquil/compatibility/__init__.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/experiment/__init__.py` & `pyquil-4.0.0rc9/pyquil/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/experiment/_calibration.py` & `pyquil-4.0.0rc9/pyquil/experiment/_calibration.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/experiment/_group.py` & `pyquil-4.0.0rc9/pyquil/experiment/_group.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/experiment/_main.py` & `pyquil-4.0.0rc9/pyquil/experiment/_main.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/experiment/_memory.py` & `pyquil-4.0.0rc9/pyquil/experiment/_memory.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/experiment/_program.py` & `pyquil-4.0.0rc9/pyquil/experiment/_program.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/experiment/_result.py` & `pyquil-4.0.0rc9/pyquil/experiment/_result.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/experiment/_setting.py` & `pyquil-4.0.0rc9/pyquil/experiment/_setting.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/experiment/_symmetrization.py` & `pyquil-4.0.0rc9/pyquil/experiment/_symmetrization.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/external/rpcq.py` & `pyquil-4.0.0rc9/pyquil/external/rpcq.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/gates.py` & `pyquil-4.0.0rc9/pyquil/gates.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/latex/_diagram.py` & `pyquil-4.0.0rc9/pyquil/latex/_diagram.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/latex/_ipython.py` & `pyquil-4.0.0rc9/pyquil/latex/_ipython.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/latex/_main.py` & `pyquil-4.0.0rc9/pyquil/latex/_main.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/latex/latex_generation.py` & `pyquil-4.0.0rc9/pyquil/latex/latex_generation.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/noise.py` & `pyquil-4.0.0rc9/pyquil/noise.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/noise_gates.py` & `pyquil-4.0.0rc9/pyquil/noise_gates.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/operator_estimation.py` & `pyquil-4.0.0rc9/pyquil/operator_estimation.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/parser.py` & `pyquil-4.0.0rc9/pyquil/parser.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/paulis.py` & `pyquil-4.0.0rc9/pyquil/paulis.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/pyqvm.py` & `pyquil-4.0.0rc9/pyquil/pyqvm.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/quantum_processor/_base.py` & `pyquil-4.0.0rc9/pyquil/quantum_processor/_base.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/quantum_processor/compiler.py` & `pyquil-4.0.0rc9/pyquil/quantum_processor/compiler.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/quantum_processor/graph.py` & `pyquil-4.0.0rc9/pyquil/quantum_processor/graph.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/quantum_processor/qcs.py` & `pyquil-4.0.0rc9/pyquil/quantum_processor/qcs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from typing import List, Optional
 
-import httpx
 import networkx as nx
-from qcs_api_client.models import InstructionSetArchitecture
-from qcs_api_client.operations.sync import get_instruction_set_architecture
 
-from pyquil.api import QCSClientConfiguration
-from pyquil.api._qcs_client import qcs_client
+from qcs_sdk import QCSClient
+from qcs_sdk.qpu.isa import InstructionSetArchitecture, get_instruction_set_architecture
+
 from pyquil.external.rpcq import CompilerISA
 from pyquil.noise import NoiseModel
 from pyquil.quantum_processor import AbstractQuantumProcessor
 from pyquil.quantum_processor.transformers import qcs_isa_to_compiler_isa, qcs_isa_to_graph
 
 
 class QCSQuantumProcessor(AbstractQuantumProcessor):
@@ -56,26 +54,24 @@
 
     def __repr__(self) -> str:
         return str(self)
 
 
 def get_qcs_quantum_processor(
     quantum_processor_id: str,
-    client_configuration: Optional[QCSClientConfiguration] = None,
+    client_configuration: Optional[QCSClient] = None,
     timeout: float = 10.0,
 ) -> QCSQuantumProcessor:
     """
     Retrieve an instruction set architecture for the specified ``quantum_processor_id`` and initialize a
     ``QCSQuantumProcessor`` with it.
 
     :param quantum_processor_id: QCS ID for the quantum processor.
     :param timeout: Time limit for request, in seconds.
     :param client_configuration: Optional client configuration. If none is provided, a default one will
            be loaded.
 
     :return: A ``QCSQuantumProcessor`` with the requested ISA.
     """
-    client_configuration = client_configuration or QCSClientConfiguration.load()
-    with qcs_client(client_configuration=client_configuration, request_timeout=timeout) as client:  # type: httpx.Client
-        isa = get_instruction_set_architecture(client=client, quantum_processor_id=quantum_processor_id).parsed
+    isa = get_instruction_set_architecture(client=client_configuration, quantum_processor_id=quantum_processor_id)
 
     return QCSQuantumProcessor(quantum_processor_id=quantum_processor_id, isa=isa)
```

### Comparing `pyquil-4.0.0rc8/pyquil/quantum_processor/transformers/graph_to_compiler_isa.py` & `pyquil-4.0.0rc9/pyquil/quantum_processor/transformers/graph_to_compiler_isa.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/quantum_processor/transformers/qcs_isa_to_compiler_isa.py` & `pyquil-4.0.0rc9/pyquil/quantum_processor/transformers/qcs_isa_to_compiler_isa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from qcs_api_client.models import InstructionSetArchitecture, Characteristic, Operation
+from qcs_sdk.qpu.isa import InstructionSetArchitecture, Characteristic, Operation
 from pyquil.external.rpcq import CompilerISA, add_edge, add_qubit, get_qubit, get_edge
 import numpy as np
 from pyquil.external.rpcq import (
     GateInfo,
     MeasureInfo,
     Supported1QGate,
     Supported2QGate,
```

### Comparing `pyquil-4.0.0rc8/pyquil/quil.py` & `pyquil-4.0.0rc9/pyquil/quil.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/quilatom.py` & `pyquil-4.0.0rc9/pyquil/quilatom.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/quilbase.py` & `pyquil-4.0.0rc9/pyquil/quilbase.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/quiltcalibrations.py` & `pyquil-4.0.0rc9/pyquil/quiltcalibrations.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/quiltwaveforms.py` & `pyquil-4.0.0rc9/pyquil/quiltwaveforms.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/simulation/_numpy.py` & `pyquil-4.0.0rc9/pyquil/simulation/_numpy.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/simulation/_reference.py` & `pyquil-4.0.0rc9/pyquil/simulation/_reference.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/simulation/matrices.py` & `pyquil-4.0.0rc9/pyquil/simulation/matrices.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/simulation/tools.py` & `pyquil-4.0.0rc9/pyquil/simulation/tools.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/pyquil/wavefunction.py` & `pyquil-4.0.0rc9/pyquil/wavefunction.py`

 * *Files identical despite different names*

### Comparing `pyquil-4.0.0rc8/PKG-INFO` & `pyquil-4.0.0rc9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquil
-Version: 4.0.0rc8
+Version: 4.0.0rc9
 Summary: A Python library for creating Quantum Instruction Language (Quil) programs.
 Home-page: https://github.com/rigetti/pyquil.git
 License: Apache-2.0
 Keywords: quantum,quil,programming,hybrid
 Author: Rigetti Computing
 Author-email: softapps@rigetti.com
 Requires-Python: >=3.8,<3.12
@@ -24,16 +24,17 @@
 Requires-Dist: Sphinx (>=4.0.2,<5.0.0) ; extra == "docs"
 Requires-Dist: importlib-metadata (>=3.7.3,<5) ; python_version < "3.8"
 Requires-Dist: ipython (>=7.21.0,<8.0.0) ; extra == "latex"
 Requires-Dist: lark (>=0.11.1,<0.12.0)
 Requires-Dist: nbsphinx (>=0.8.6,<0.9.0) ; extra == "docs"
 Requires-Dist: networkx (>=2.5,<3.0)
 Requires-Dist: numpy (>=1.21,<2.0)
-Requires-Dist: qcs-api-client (>=0.21.0,<0.22.0)
-Requires-Dist: qcs-sdk-python (==0.4.2)
+Requires-Dist: pandoc (>=2.3,<3.0) ; extra == "docs"
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: qcs-sdk-python (==0.5.0rc.17)
 Requires-Dist: recommonmark (>=0.7.1,<0.8.0) ; extra == "docs"
 Requires-Dist: retry (>=0.9.2,<0.10.0)
 Requires-Dist: rpcq (>=3.10.0,<4.0.0)
 Requires-Dist: scipy (>=1.7.3,<2.0.0)
 Requires-Dist: sphinx-rtd-theme (>=0.5.2,<0.6.0) ; extra == "docs"
 Requires-Dist: types-python-dateutil (>=2.8.19,<3.0.0)
 Requires-Dist: types-retry (>=0.9.9,<0.10.0)
```


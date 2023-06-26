# Comparing `tmp/pydelling-1.9.tar.gz` & `tmp/pydelling-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydelling-1.9.tar", max compression
+gzip compressed data, was "pydelling-1.9.1.tar", max compression
```

## Comparing `pydelling-1.9.tar` & `pydelling-1.9.1.tar`

### file list

```diff
@@ -1,226 +1,226 @@
--rw-r--r--   0        0        0     1061 2022-11-07 19:53:46.355707 pydelling-1.9/LICENSE.txt
--rw-r--r--   0        0        0     1155 2022-11-07 19:53:46.355877 pydelling-1.9/README.md
--rw-r--r--   0        0        0      171 2022-11-07 19:53:46.469084 pydelling-1.9/pydelling/__init__.py
--rw-r--r--   0        0        0     2338 2022-11-07 19:53:46.469199 pydelling-1.9/pydelling/config/__init__.py
--rw-r--r--   0        0        0     2847 2022-11-07 19:53:46.469287 pydelling-1.9/pydelling/config/conda_env.yaml
--rw-r--r--   0        0        0      386 2022-11-07 19:53:46.469356 pydelling-1.9/pydelling/config/global_config.yaml
--rw-r--r--   0        0        0      370 2022-11-07 19:53:46.469431 pydelling-1.9/pydelling/config/local_config.yaml
--rw-r--r--   0        0        0      675 2022-11-07 19:53:46.469506 pydelling-1.9/pydelling/config/logger_config.yaml
--rw-r--r--   0        0        0     6243 2022-11-07 19:53:46.469631 pydelling-1.9/pydelling/interpolation/BaseInterpolator.py
--rw-r--r--   0        0        0     5402 2022-11-07 19:53:46.469712 pydelling-1.9/pydelling/interpolation/KdeEstimator.py
--rw-r--r--   0        0        0     3637 2022-11-07 19:53:46.469786 pydelling-1.9/pydelling/interpolation/SparseDataInterpolator.py
--rw-r--r--   0        0        0      145 2022-11-07 19:53:46.469861 pydelling-1.9/pydelling/interpolation/__init__.py
--rw-r--r--   0        0        0     4633 2022-11-21 17:12:37.745906 pydelling-1.9/pydelling/managers/BaseManager.py
--rw-r--r--   0        0        0     9252 2022-11-21 17:12:37.746059 pydelling-1.9/pydelling/managers/BaseStudy.py
--rw-r--r--   0        0        0     5724 2022-11-21 17:12:37.746200 pydelling-1.9/pydelling/managers/PflotranManager.py
--rw-r--r--   0        0        0    11793 2022-11-07 19:53:46.470323 pydelling-1.9/pydelling/managers/PflotranPostprocessing.py
--rw-r--r--   0        0        0    10477 2022-11-21 17:12:37.746348 pydelling-1.9/pydelling/managers/PflotranStudy.py
--rw-r--r--   0        0        0      241 2022-11-07 19:53:46.470486 pydelling-1.9/pydelling/managers/__init__.py
--rw-r--r--   0        0        0      909 2022-11-07 19:53:46.470601 pydelling-1.9/pydelling/managers/callbacks/BaseCallback.py
--rw-r--r--   0        0        0     1250 2022-11-21 17:12:37.746560 pydelling-1.9/pydelling/managers/callbacks/PflotranRestartCallback.py
--rw-r--r--   0        0        0     2339 2022-11-07 19:53:46.470800 pydelling-1.9/pydelling/managers/callbacks/PflotranSaveResultsCallback.py
--rw-r--r--   0        0        0      168 2022-11-07 19:53:46.470881 pydelling-1.9/pydelling/managers/callbacks/__init__.py
--rw-r--r--   0        0        0    17057 2022-11-07 19:53:46.471041 pydelling-1.9/pydelling/paraview_processor/ParaviewProcessor.py
--rw-r--r--   0        0        0       48 2022-11-07 19:53:46.471131 pydelling-1.9/pydelling/paraview_processor/__init__.py
--rw-r--r--   0        0        0      475 2022-11-07 19:53:46.471254 pydelling-1.9/pydelling/paraview_processor/filters/AppendArcLengthFilter.py
--rw-r--r--   0        0        0     4162 2022-11-07 19:53:46.471346 pydelling-1.9/pydelling/paraview_processor/filters/BaseFilter.py
--rw-r--r--   0        0        0     1225 2022-11-07 19:53:46.471470 pydelling-1.9/pydelling/paraview_processor/filters/CalculatorFilter.py
--rw-r--r--   0        0        0      507 2022-11-07 19:53:46.471550 pydelling-1.9/pydelling/paraview_processor/filters/CellDataToPointDataFilter.py
--rw-r--r--   0        0        0     1070 2022-11-07 19:53:46.471644 pydelling-1.9/pydelling/paraview_processor/filters/ClipFilter.py
--rw-r--r--   0        0        0     1411 2022-11-07 19:53:46.471733 pydelling-1.9/pydelling/paraview_processor/filters/CsvReaderFilter.py
--rw-r--r--   0        0        0      712 2022-11-07 19:53:46.471831 pydelling-1.9/pydelling/paraview_processor/filters/IntegrateVariablesFilter.py
--rw-r--r--   0        0        0     2332 2022-11-07 19:53:46.472080 pydelling-1.9/pydelling/paraview_processor/filters/PlotOverLineFilter.py
--rw-r--r--   0        0        0      638 2022-11-07 19:53:46.472259 pydelling-1.9/pydelling/paraview_processor/filters/SaveDataFilter.py
--rw-r--r--   0        0        0      907 2022-11-07 19:53:46.472353 pydelling-1.9/pydelling/paraview_processor/filters/StreamTracerWithCustomSourceFilter.py
--rw-r--r--   0        0        0      805 2022-11-07 19:53:46.472434 pydelling-1.9/pydelling/paraview_processor/filters/TableToPointsFilter.py
--rw-r--r--   0        0        0      386 2022-11-07 19:53:46.472521 pydelling-1.9/pydelling/paraview_processor/filters/TecplotFilter.py
--rw-r--r--   0        0        0      823 2022-11-07 19:53:46.472611 pydelling-1.9/pydelling/paraview_processor/filters/VtkFilter.py
--rw-r--r--   0        0        0      821 2022-11-07 19:53:46.472697 pydelling-1.9/pydelling/paraview_processor/filters/XDMFFilter.py
--rw-r--r--   0        0        0      686 2022-11-07 19:53:46.472777 pydelling-1.9/pydelling/paraview_processor/filters/__init__.py
--rw-r--r--   0        0        0      535 2022-11-07 19:53:46.472929 pydelling-1.9/pydelling/preprocessing/BasePreprocessing.py
--rw-r--r--   0        0        0    11578 2022-11-07 19:53:46.473055 pydelling-1.9/pydelling/preprocessing/ClosedStlGenerator.py
--rw-r--r--   0        0        0        0 2022-11-07 19:53:46.473091 pydelling-1.9/pydelling/preprocessing/GidPreprocessor.py
--rw-r--r--   0        0        0     8506 2022-11-07 19:53:46.473320 pydelling-1.9/pydelling/preprocessing/STLFromPointCloud.py
--rw-r--r--   0        0        0      246 2022-11-07 19:53:46.473398 pydelling-1.9/pydelling/preprocessing/__init__.py
--rw-r--r--   0        0        0    15467 2022-11-07 19:53:46.473549 pydelling-1.9/pydelling/preprocessing/dfn_preprocessor/DfnPreprocessor.py
--rw-r--r--   0        0        0    33675 2022-11-07 19:53:46.473786 pydelling-1.9/pydelling/preprocessing/dfn_preprocessor/DfnUpscaler.py
--rw-r--r--   0        0        0     3275 2022-11-07 19:53:46.473893 pydelling-1.9/pydelling/preprocessing/dfn_preprocessor/Fault.py
--rw-r--r--   0        0        0    15024 2022-11-07 19:53:46.474027 pydelling-1.9/pydelling/preprocessing/dfn_preprocessor/Fracture.py
--rw-r--r--   0        0        0     8983 2022-11-07 19:53:46.474095 pydelling-1.9/pydelling/preprocessing/dfn_preprocessor/PolygonFracture.py
--rw-r--r--   0        0        0      183 2022-11-07 19:53:46.474159 pydelling-1.9/pydelling/preprocessing/dfn_preprocessor/__init__.py
--rw-r--r--   0        0        0     3711 2022-11-07 19:53:46.474275 pydelling-1.9/pydelling/preprocessing/gid_preprocessor/GidObject.py
--rw-r--r--   0        0        0     1849 2022-11-07 19:53:46.474351 pydelling-1.9/pydelling/preprocessing/gid_preprocessor/Line.py
--rw-r--r--   0        0        0     1456 2022-11-07 19:53:46.474427 pydelling-1.9/pydelling/preprocessing/gid_preprocessor/Point.py
--rw-r--r--   0        0        0     1768 2022-11-07 19:53:46.474497 pydelling-1.9/pydelling/preprocessing/gid_preprocessor/Surface.py
--rw-r--r--   0        0        0      352 2022-11-07 19:53:46.474566 pydelling-1.9/pydelling/preprocessing/gid_preprocessor/_AbstractGidObject.py
--rw-r--r--   0        0        0      136 2022-11-07 19:53:46.474625 pydelling-1.9/pydelling/preprocessing/gid_preprocessor/__init__.py
--rw-r--r--   0        0        0      970 2022-11-07 19:53:46.474690 pydelling-1.9/pydelling/preprocessing/gid_preprocessor/gidobjects.py
--rw-r--r--   0        0        0    20486 2022-11-07 19:53:46.474864 pydelling-1.9/pydelling/preprocessing/mesh_preprocessor/MeshPreprocessor.py
--rw-r--r--   0        0        0       46 2022-11-07 19:53:46.474946 pydelling-1.9/pydelling/preprocessing/mesh_preprocessor/__init__.py
--rw-r--r--   0        0        0      588 2022-11-07 19:53:46.475063 pydelling-1.9/pydelling/preprocessing/mesh_preprocessor/geometry/BaseAbstractMeshObject.py
--rw-r--r--   0        0        0    13746 2022-11-07 19:53:46.475194 pydelling-1.9/pydelling/preprocessing/mesh_preprocessor/geometry/BaseElement.py
--rw-r--r--   0        0        0     3805 2022-11-07 19:53:46.475278 pydelling-1.9/pydelling/preprocessing/mesh_preprocessor/geometry/BaseFace.py
--rw-r--r--   0        0        0     5760 2022-11-07 19:53:46.475385 pydelling-1.9/pydelling/preprocessing/mesh_preprocessor/geometry/HexahedraElement.py
--rw-r--r--   0        0        0     3912 2022-11-07 19:53:46.475469 pydelling-1.9/pydelling/preprocessing/mesh_preprocessor/geometry/PyramidElement.py
--rw-r--r--   0        0        0     1881 2022-11-07 19:53:46.475549 pydelling-1.9/pydelling/preprocessing/mesh_preprocessor/geometry/QuadrilateralFace.py
--rw-r--r--   0        0        0     3627 2022-11-07 19:53:46.475627 pydelling-1.9/pydelling/preprocessing/mesh_preprocessor/geometry/TetrahedraElement.py
--rw-r--r--   0        0        0      725 2022-11-07 19:53:46.475698 pydelling-1.9/pydelling/preprocessing/mesh_preprocessor/geometry/TriangleFace.py
--rw-r--r--   0        0        0     4782 2022-11-07 19:53:46.475767 pydelling-1.9/pydelling/preprocessing/mesh_preprocessor/geometry/WedgeElement.py
--rw-r--r--   0        0        0      393 2022-11-07 19:53:46.475853 pydelling-1.9/pydelling/preprocessing/mesh_preprocessor/geometry/__init__.py
--rw-r--r--   0        0        0     3656 2022-11-07 19:53:46.475973 pydelling-1.9/pydelling/readers/BaseReader.py
--rw-r--r--   0        0        0     3608 2022-11-07 19:53:46.476046 pydelling-1.9/pydelling/readers/CentroidReader.py
--rw-r--r--   0        0        0     2799 2022-11-07 19:53:46.476132 pydelling-1.9/pydelling/readers/ConnectFlowReader.py
--rw-r--r--   0        0        0     6305 2022-11-07 19:53:46.476229 pydelling-1.9/pydelling/readers/FemReader.py
--rw-r--r--   0        0        0     2245 2022-11-07 19:53:46.476307 pydelling-1.9/pydelling/readers/OpenFoamReader.py
--rw-r--r--   0        0        0     1049 2022-11-07 19:53:46.476392 pydelling-1.9/pydelling/readers/PflotranMassBalanceFileReader.py
--rw-r--r--   0        0        0     5662 2022-11-07 19:53:46.476478 pydelling-1.9/pydelling/readers/PflotranObservationPointReader.py
--rw-r--r--   0        0        0     4047 2022-11-07 19:53:46.476551 pydelling-1.9/pydelling/readers/PflotranProcessingUtils.py
--rw-r--r--   0        0        0    16747 2022-11-07 19:53:46.476684 pydelling-1.9/pydelling/readers/PflotranReader.py
--rw-r--r--   0        0        0    14870 2022-11-07 19:53:46.476809 pydelling-1.9/pydelling/readers/RasterFileReader.py
--rw-r--r--   0        0        0     3127 2022-11-07 19:53:46.476881 pydelling-1.9/pydelling/readers/SmeshReader.py
--rw-r--r--   0        0        0    19446 2022-11-07 19:53:46.476992 pydelling-1.9/pydelling/readers/StreamlineReader.py
--rw-r--r--   0        0        0     2256 2022-11-07 19:53:46.477090 pydelling-1.9/pydelling/readers/StructuredGridReader.py
--rw-r--r--   0        0        0     3872 2022-11-07 19:53:46.477164 pydelling-1.9/pydelling/readers/StructuredListReader.py
--rw-r--r--   0        0        0      249 2022-11-07 19:53:46.477234 pydelling-1.9/pydelling/readers/UnstructuredMeshReader.py
--rw-r--r--   0        0        0     5886 2022-11-07 19:53:46.477325 pydelling-1.9/pydelling/readers/VTKMeshReader.py
--rw-r--r--   0        0        0     1512 2022-11-07 19:53:46.477399 pydelling-1.9/pydelling/readers/VtkReader.py
--rw-r--r--   0        0        0      875 2022-11-07 19:53:46.477473 pydelling-1.9/pydelling/readers/__init__.py
--rw-r--r--   0        0        0       36 2022-11-07 19:53:46.477584 pydelling-1.9/pydelling/readers/iGPReader/__init__.py
--rw-r--r--   0        0        0    10497 2022-11-07 19:53:46.477726 pydelling-1.9/pydelling/readers/iGPReader/engines/PostProcessingEngine.py
--rw-r--r--   0        0        0       54 2022-11-07 19:53:46.477795 pydelling-1.9/pydelling/readers/iGPReader/engines/__init__.py
--rw-r--r--   0        0        0     1540 2022-11-07 19:53:46.477927 pydelling-1.9/pydelling/readers/iGPReader/geometry/BaseElement.py
--rw-r--r--   0        0        0     2673 2022-11-07 19:53:46.478007 pydelling-1.9/pydelling/readers/iGPReader/geometry/BaseFace.py
--rw-r--r--   0        0        0     5280 2022-11-07 19:53:46.478084 pydelling-1.9/pydelling/readers/iGPReader/geometry/HexahedraElement.py
--rw-r--r--   0        0        0     1363 2022-11-07 19:53:46.478156 pydelling-1.9/pydelling/readers/iGPReader/geometry/QuadrilateralFace.py
--rw-r--r--   0        0        0     3318 2022-11-07 19:53:46.478224 pydelling-1.9/pydelling/readers/iGPReader/geometry/TetrahedraElement.py
--rw-r--r--   0        0        0      297 2022-11-07 19:53:46.478452 pydelling-1.9/pydelling/readers/iGPReader/geometry/TriangleFace.py
--rw-r--r--   0        0        0     4356 2022-11-07 19:53:46.478566 pydelling-1.9/pydelling/readers/iGPReader/geometry/WedgeElement.py
--rw-r--r--   0        0        0      291 2022-11-07 19:53:46.478658 pydelling-1.9/pydelling/readers/iGPReader/geometry/__init__.py
--rw-r--r--   0        0        0     6138 2022-11-07 19:53:46.478845 pydelling-1.9/pydelling/readers/iGPReader/io/AscReader.py
--rw-r--r--   0        0        0      426 2022-11-07 19:53:46.478921 pydelling-1.9/pydelling/readers/iGPReader/io/BaseReader.py
--rw-r--r--   0        0        0       27 2022-11-07 19:53:46.478995 pydelling-1.9/pydelling/readers/iGPReader/io/BaseWriter.py
--rw-r--r--   0        0        0    10264 2022-11-07 19:53:46.479096 pydelling-1.9/pydelling/readers/iGPReader/io/BoreholeReader.py
--rw-r--r--   0        0        0     2111 2022-11-07 19:53:46.479168 pydelling-1.9/pydelling/readers/iGPReader/io/CsvWriter.py
--rw-r--r--   0        0        0     4874 2022-11-07 19:53:46.479263 pydelling-1.9/pydelling/readers/iGPReader/io/PflotranExplicitWriter.py
--rw-r--r--   0        0        0     3447 2022-11-07 19:53:46.479356 pydelling-1.9/pydelling/readers/iGPReader/io/PflotranImplicitWriter.py
--rw-r--r--   0        0        0      330 2022-11-07 19:53:46.479441 pydelling-1.9/pydelling/readers/iGPReader/io/__init__.py
--rw-r--r--   0        0        0    45831 2022-11-07 19:53:46.479665 pydelling-1.9/pydelling/readers/iGPReader/io/iGPReader.py
--rw-r--r--   0        0        0     2683 2022-11-07 19:53:46.479843 pydelling-1.9/pydelling/readers/iGPReader/utils/RegionOperations.py
--rw-r--r--   0        0        0       67 2022-11-07 19:53:46.479944 pydelling-1.9/pydelling/readers/iGPReader/utils/__init__.py
--rw-r--r--   0        0        0      978 2022-11-07 19:53:46.480029 pydelling-1.9/pydelling/readers/iGPReader/utils/decorators.py
--rw-r--r--   0        0        0     1024 2022-11-07 19:53:46.480110 pydelling-1.9/pydelling/readers/iGPReader/utils/geometry_utils.py
--rw-r--r--   0        0        0     1234 2022-11-07 19:53:46.480185 pydelling-1.9/pydelling/readers/iGPReader/utils/utils.py
--rw-r--r--   0        0        0     8533 2022-11-07 19:53:46.480340 pydelling-1.9/pydelling/tests/Pwall.ex
--rw-r--r--   0        0        0        0 2022-11-07 19:53:46.480376 pydelling-1.9/pydelling/tests/__init__.py
--rw-r--r--   0        0        0      182 2022-11-07 19:53:46.480490 pydelling-1.9/pydelling/tests/_trial_temp/custom_edge_intersections.txt
--rw-r--r--   0        0        0      179 2022-11-07 19:53:46.480559 pydelling-1.9/pydelling/tests/_trial_temp/fracture.obj
--rw-r--r--   0        0        0       52 2022-11-07 19:53:46.480620 pydelling-1.9/pydelling/tests/_trial_temp/gid_batch.bch
--rw-r--r--   0        0        0      457 2022-11-07 19:53:46.480691 pydelling-1.9/pydelling/tests/_trial_temp/test.json
--rw-r--r--   0        0        0      382 2022-11-07 19:53:46.480750 pydelling-1.9/pydelling/tests/_trial_temp/test_dfn.vtk
--rw-r--r--   0        0        0      282 2022-11-07 19:53:46.480828 pydelling-1.9/pydelling/tests/_trial_temp/test_element.obj
--rw-r--r--   0        0        0      451 2022-11-07 19:53:46.480896 pydelling-1.9/pydelling/tests/_trial_temp/test_mesh.vtk
--rw-r--r--   0        0        0        0 2022-11-07 19:53:46.480980 pydelling-1.9/pydelling/tests/interpolation/__init__.py
--rw-r--r--   0        0        0     1065 2022-11-07 19:53:46.481090 pydelling-1.9/pydelling/tests/interpolation/test_base_interpolator.py
--rw-r--r--   0        0        0      623 2022-11-07 19:53:46.481170 pydelling-1.9/pydelling/tests/interpolation/test_kde_estimator.py
--rw-r--r--   0        0        0      981 2022-11-07 19:53:46.481244 pydelling-1.9/pydelling/tests/interpolation/test_sparse_data_interpolator.py
--rw-r--r--   0        0        0        0 2022-11-07 19:53:46.481330 pydelling-1.9/pydelling/tests/managers/__init__.py
--rw-r--r--   0        0        0     1320 2022-11-07 19:53:46.481425 pydelling-1.9/pydelling/tests/managers/test_base_study.py
--rw-r--r--   0        0        0     2694 2022-11-07 19:53:46.481509 pydelling-1.9/pydelling/tests/managers/test_pflotran_study.py
--rw-r--r--   0        0        0        0 2022-11-07 19:53:46.481681 pydelling-1.9/pydelling/tests/preprocessing/DfnPreprocessor/__init__.py
--rw-r--r--   0        0        0      179 2022-11-07 19:53:46.481758 pydelling-1.9/pydelling/tests/preprocessing/DfnPreprocessor/fracture.obj
--rw-r--r--   0        0        0     2283 2022-11-07 19:53:46.481834 pydelling-1.9/pydelling/tests/preprocessing/DfnPreprocessor/test_dfn_preprocessor.py
--rw-r--r--   0        0        0      151 2022-11-07 19:53:46.481919 pydelling-1.9/pydelling/tests/preprocessing/DfnPreprocessor/test_fracture_object.py
--rw-r--r--   0        0        0    12580 2022-11-07 19:53:46.482014 pydelling-1.9/pydelling/tests/preprocessing/DfnPreprocessor/test_intersection.py
--rw-r--r--   0        0        0     3766 2022-11-07 19:53:46.482093 pydelling-1.9/pydelling/tests/preprocessing/DfnPreprocessor/test_upscaling.py
--rw-r--r--   0        0        0        0 2022-11-07 19:53:46.482161 pydelling-1.9/pydelling/tests/preprocessing/MeshPreprocessor/__init__.py
--rw-r--r--   0        0        0     4144 2022-11-07 19:53:46.482250 pydelling-1.9/pydelling/tests/preprocessing/MeshPreprocessor/test_mesh_preprocessor.py
--rw-r--r--   0        0        0        0 2022-11-07 19:53:46.482278 pydelling-1.9/pydelling/tests/preprocessing/__init__.py
--rw-r--r--   0        0        0      154 2022-11-07 19:53:46.482356 pydelling-1.9/pydelling/tests/preprocessing/test_base_preprocessing.py
--rw-r--r--   0        0        0      152 2022-11-07 19:53:46.482426 pydelling-1.9/pydelling/tests/preprocessing/test_dfn_preprocessor.py
--rw-r--r--   0        0        0     3415 2022-11-07 19:53:46.482510 pydelling-1.9/pydelling/tests/preprocessing/test_gid_preprocessor.py
--rw-r--r--   0        0        0        0 2022-11-07 19:53:46.482594 pydelling-1.9/pydelling/tests/readers/__init__.py
--rwxr-xr-x   0        0        0        0 2022-11-07 19:53:46.482698 pydelling-1.9/pydelling/tests/readers/_trial_temp/_trial_marker
--rw-r--r--   0        0        0      175 2022-11-07 19:53:46.482780 pydelling-1.9/pydelling/tests/readers/test_BaseReader.py
--rw-r--r--   0        0        0      875 2022-11-07 19:53:46.482922 pydelling-1.9/pydelling/tests/readers/test_CentroidReader.py
--rw-r--r--   0        0        0      144 2022-11-07 19:53:46.482989 pydelling-1.9/pydelling/tests/readers/test_PflotranReader.py
--rw-r--r--   0        0        0     1945 2022-11-07 19:53:46.483067 pydelling-1.9/pydelling/tests/readers/test_RasterFileReader.py
--rw-r--r--   0        0        0      412 2022-11-07 19:53:46.483144 pydelling-1.9/pydelling/tests/readers/test_SmeshReader.py
--rw-r--r--   0        0        0      993 2022-11-07 19:53:46.483224 pydelling-1.9/pydelling/tests/readers/test_StreamlineReader.py
--rw-r--r--   0        0        0      407 2022-11-07 19:53:46.483319 pydelling-1.9/pydelling/tests/readers/test_fem_reader.py
--rw-r--r--   0        0        0     3746 2022-11-07 19:53:46.483407 pydelling-1.9/pydelling/tests/readers/test_iGPReader.py
--rw-r--r--   0        0        0       90 2022-11-07 19:53:46.483482 pydelling-1.9/pydelling/tests/silly_test.py
--rw-r--r--   0        0        0      457 2022-11-07 19:53:46.483566 pydelling-1.9/pydelling/tests/test.json
--rw-r--r--   0        0        0  1429424 2022-11-07 19:53:46.489794 pydelling-1.9/pydelling/tests/test_data/bottom_surface.asc
--rw-r--r--   0        0        0       81 2022-11-07 19:53:46.489946 pydelling-1.9/pydelling/tests/test_data/centroid_reader_data.csv
--rwxr-xr-x   0        0        0   267949 2022-11-07 19:53:46.490702 pydelling-1.9/pydelling/tests/test_data/fem_reader_data.fem
--rw-r--r--   0        0        0     1651 2022-11-07 19:53:46.490871 pydelling-1.9/pydelling/tests/test_data/problematic_fractures/issue_element_1.pkl
--rw-r--r--   0        0        0     2356 2022-11-07 19:53:46.490956 pydelling-1.9/pydelling/tests/test_data/problematic_fractures/issue_element_2.pkl
--rw-r--r--   0        0        0     4974 2022-11-07 19:53:46.491051 pydelling-1.9/pydelling/tests/test_data/problematic_fractures/issue_fracture_1.pkl
--rw-r--r--   0        0        0    10207 2022-11-07 19:53:46.491154 pydelling-1.9/pydelling/tests/test_data/problematic_fractures/issue_fracture_2.pkl
--rw-r--r--   0        0        0       81 2022-11-07 19:53:46.491239 pydelling-1.9/pydelling/tests/test_data/smesh_test_data.smesh
--rw-r--r--   0        0        0   132941 2022-11-07 19:53:46.491798 pydelling-1.9/pydelling/tests/test_data/streamline_test_data.csv
--rwxr-xr-x   0        0        0    84084 2022-11-07 19:53:46.492154 pydelling-1.9/pydelling/tests/test_data/test_fault.stl
--rw-r--r--   0        0        0        0 2022-11-07 19:53:46.492416 pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/PFLOTRAN/PFLOTRANrun/OutputScreen.dat
--rw-r--r--   0        0        0     3685 2022-11-07 19:53:46.492555 pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/PFLOTRAN/PFLOTRANrun/test_implicit_to_explicit.in
--rw-r--r--   0        0        0     3685 2022-11-07 19:53:46.492654 pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/PFLOTRAN/test_implicit_to_explicit.in
--rw-r--r--   0        0        0    28492 2022-11-07 19:53:46.492802 pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/centroid.dat
--rw-r--r--   0        0        0    30249 2022-11-07 19:53:46.493252 pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/data.mesh
--rw-r--r--   0        0        0   137588 2022-11-07 19:53:46.493450 pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/explicit_mesh.mesh
--rw-r--r--   0        0        0     2890 2022-11-07 19:53:46.493561 pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/source.ss
--rw-r--r--   0        0        0     3599 2022-11-07 19:53:46.493651 pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/test_implicit_to_explicit-4.dat
--rw-r--r--   0        0        0     3815 2022-11-07 19:53:46.493739 pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/test_implicit_to_explicit.geo
--rw-r--r--   0        0        0    63980 2022-11-07 19:53:46.493950 pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/test_implicit_to_explicit.msh
--rw-r--r--   0        0        0    10426 2022-11-07 19:53:46.494092 pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/test_implicit_to_explicit.png
--rw-r--r--   0        0        0     1098 2022-11-07 19:53:46.494169 pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/test_implicit_to_explicit.rdr
--rw-r--r--   0        0        0      143 2022-11-07 19:53:46.494259 pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/test_implicit_to_explicit.tree
--rw-r--r--   0        0        0     1492 2022-11-07 19:53:46.494361 pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/test_implicit_to_explicit.vv
--rw-r--r--   0        0        0    10439 2022-11-07 19:53:46.494476 pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/top_surface.ex
--rw-r--r--   0        0        0     5125 2022-11-07 19:53:46.494584 pydelling-1.9/pydelling/tests/test_data/test_manager.in
--rw-r--r--   0        0        0     5075 2022-11-07 19:53:46.494663 pydelling-1.9/pydelling/tests/test_data/test_pflotran_manager_nocheckpoint.in
--rw-r--r--   0        0        0  1429989 2022-11-07 19:53:46.495599 pydelling-1.9/pydelling/tests/test_data/top_surface.asc
--rw-r--r--   0        0        0        0 2022-11-07 19:53:46.495740 pydelling-1.9/pydelling/tests/utils/__init__.py
--rw-r--r--   0        0        0        0 2022-11-07 19:53:46.495854 pydelling-1.9/pydelling/tests/utils/geometry/__init__.py
--rwxr-xr-x   0        0        0        0 2022-11-07 19:53:46.495956 pydelling-1.9/pydelling/tests/utils/geometry/_trial_temp/_trial_marker
--rw-r--r--   0        0        0      755 2022-11-07 19:53:46.496529 pydelling-1.9/pydelling/tests/utils/geometry/random_test.py
--rw-r--r--   0        0        0     3011 2022-11-07 19:53:46.497211 pydelling-1.9/pydelling/tests/utils/geometry/test_Line.py
--rw-r--r--   0        0        0      600 2022-11-07 19:53:46.497338 pydelling-1.9/pydelling/tests/utils/geometry/test_Plane.py
--rw-r--r--   0        0        0      517 2022-11-07 19:53:46.497436 pydelling-1.9/pydelling/tests/utils/geometry/test_Point.py
--rw-r--r--   0        0        0     2209 2022-11-07 19:53:46.497550 pydelling-1.9/pydelling/tests/utils/test_geometry_utils.py
--rw-r--r--   0        0        0        0 2022-11-07 19:53:46.497798 pydelling-1.9/pydelling/tests/writers/__init__.py
--rw-r--r--   0        0        0     3021 2022-11-07 19:53:46.498029 pydelling-1.9/pydelling/utils/SubFishModule.py
--rw-r--r--   0        0        0       94 2022-11-07 19:53:46.498129 pydelling-1.9/pydelling/utils/__init__.py
--rw-r--r--   0        0        0     1621 2022-11-21 17:12:37.746977 pydelling-1.9/pydelling/utils/configuration_utils.py
--rw-r--r--   0        0        0      214 2022-11-07 19:53:46.498353 pydelling-1.9/pydelling/utils/decorators.py
--rw-r--r--   0        0        0       73 2022-11-07 19:53:46.498506 pydelling-1.9/pydelling/utils/geometry/BasePrimitive.py
--rw-r--r--   0        0        0     2311 2022-11-07 19:53:46.498610 pydelling-1.9/pydelling/utils/geometry/Line.py
--rw-r--r--   0        0        0     1516 2022-11-07 19:53:46.498717 pydelling-1.9/pydelling/utils/geometry/Plane.py
--rw-r--r--   0        0        0     1056 2022-11-07 19:53:46.498807 pydelling-1.9/pydelling/utils/geometry/Point.py
--rw-r--r--   0        0        0      924 2022-11-07 19:53:46.498893 pydelling-1.9/pydelling/utils/geometry/Polygon.py
--rw-r--r--   0        0        0      204 2022-11-07 19:53:46.498965 pydelling-1.9/pydelling/utils/geometry/Scalar.py
--rw-r--r--   0        0        0     1098 2022-11-07 19:53:46.499062 pydelling-1.9/pydelling/utils/geometry/Segment.py
--rw-r--r--   0        0        0      967 2022-11-07 19:53:46.499249 pydelling-1.9/pydelling/utils/geometry/Vector.py
--rw-r--r--   0        0        0      196 2022-11-07 19:53:46.499442 pydelling-1.9/pydelling/utils/geometry/__init__.py
--rw-r--r--   0        0        0     2432 2022-11-07 19:53:46.499582 pydelling-1.9/pydelling/utils/geometry/intersections.py
--rw-r--r--   0        0        0     3569 2022-11-07 19:53:46.499711 pydelling-1.9/pydelling/utils/geometry_utils.py
--rw-r--r--   0        0        0     2166 2022-11-07 19:53:46.499844 pydelling-1.9/pydelling/utils/utility_subclasses.py
--rw-r--r--   0        0        0    11921 2022-11-07 19:53:46.499970 pydelling-1.9/pydelling/utils/utils.py
--rw-r--r--   0        0        0       74 2022-11-07 19:53:46.500147 pydelling-1.9/pydelling/webapps/.streamlit/config.toml
--rw-r--r--   0        0        0      998 2022-11-07 19:53:46.500260 pydelling-1.9/pydelling/webapps/BaseStreamlitUtilityClass.py
--rw-r--r--   0        0        0      992 2022-11-07 19:53:46.500345 pydelling-1.9/pydelling/webapps/WebAppRunner.py
--rw-r--r--   0        0        0      103 2022-11-07 19:53:46.500420 pydelling-1.9/pydelling/webapps/__init__.py
--rw-r--r--   0        0        0     1280 2022-11-07 19:53:46.500537 pydelling-1.9/pydelling/webapps/components/BaseComponent.py
--rw-r--r--   0        0        0     5974 2022-11-07 19:53:46.500631 pydelling-1.9/pydelling/webapps/components/InputComponent.py
--rw-r--r--   0        0        0     4095 2022-11-07 19:53:46.500723 pydelling-1.9/pydelling/webapps/components/RemoteLoginComponent.py
--rw-r--r--   0        0        0      138 2022-11-07 19:53:46.500799 pydelling-1.9/pydelling/webapps/components/__init__.py
--rw-r--r--   0        0        0      765 2022-11-07 19:53:46.500936 pydelling-1.9/pydelling/webapps/webapps/pflotran_runner_webapp.py
--rw-r--r--   0        0        0     8480 2022-11-07 19:53:46.501128 pydelling-1.9/pydelling/webapps/webapps/sparse_interpolator_webapp.py
--rw-r--r--   0        0        0      771 2022-11-07 19:53:46.501335 pydelling-1.9/pydelling/webapps/webapps/test_bash_vtk.py
--rw-r--r--   0        0        0      236 2022-11-07 19:53:46.501431 pydelling-1.9/pydelling/webapps/webapps/test_webapp.py
--rw-r--r--   0        0        0     3093 2022-11-07 19:53:46.501654 pydelling-1.9/pydelling/writers/BaseWriter.py
--rw-r--r--   0        0        0     5586 2022-11-07 19:53:46.501786 pydelling-1.9/pydelling/writers/HDF5CentroidWriter.py
--rw-r--r--   0        0        0     5126 2022-11-21 17:12:37.747099 pydelling-1.9/pydelling/writers/HDF5RasterWriter.py
--rw-r--r--   0        0        0     3791 2022-11-07 19:53:46.502078 pydelling-1.9/pydelling/writers/OpenFoamVariableWriter.py
--rw-r--r--   0        0        0      191 2022-11-07 19:53:46.502172 pydelling-1.9/pydelling/writers/__init__.py
--rw-r--r--   0        0        0      834 2022-11-21 17:29:46.694611 pydelling-1.9/pyproject.toml
--rw-r--r--   0        0        0     3845 1970-01-01 00:00:00.000000 pydelling-1.9/setup.py
--rw-r--r--   0        0        0     2457 1970-01-01 00:00:00.000000 pydelling-1.9/PKG-INFO
+-rw-r--r--   0        0        0     1061 2022-11-07 19:53:46.355707 pydelling-1.9.1/LICENSE.txt
+-rw-r--r--   0        0        0     1155 2022-11-07 19:53:46.355877 pydelling-1.9.1/README.md
+-rw-r--r--   0        0        0      171 2022-11-07 19:53:46.469084 pydelling-1.9.1/pydelling/__init__.py
+-rw-r--r--   0        0        0     2338 2022-11-07 19:53:46.469199 pydelling-1.9.1/pydelling/config/__init__.py
+-rw-r--r--   0        0        0     2847 2022-11-07 19:53:46.469287 pydelling-1.9.1/pydelling/config/conda_env.yaml
+-rw-r--r--   0        0        0      386 2022-11-07 19:53:46.469356 pydelling-1.9.1/pydelling/config/global_config.yaml
+-rw-r--r--   0        0        0      370 2022-11-07 19:53:46.469431 pydelling-1.9.1/pydelling/config/local_config.yaml
+-rw-r--r--   0        0        0      675 2022-11-07 19:53:46.469506 pydelling-1.9.1/pydelling/config/logger_config.yaml
+-rw-r--r--   0        0        0     6243 2022-11-07 19:53:46.469631 pydelling-1.9.1/pydelling/interpolation/BaseInterpolator.py
+-rw-r--r--   0        0        0     5402 2022-11-07 19:53:46.469712 pydelling-1.9.1/pydelling/interpolation/KdeEstimator.py
+-rw-r--r--   0        0        0     3637 2022-11-07 19:53:46.469786 pydelling-1.9.1/pydelling/interpolation/SparseDataInterpolator.py
+-rw-r--r--   0        0        0      145 2022-11-07 19:53:46.469861 pydelling-1.9.1/pydelling/interpolation/__init__.py
+-rw-r--r--   0        0        0     4633 2022-11-21 17:12:37.745906 pydelling-1.9.1/pydelling/managers/BaseManager.py
+-rw-r--r--   0        0        0     9252 2022-11-21 17:12:37.746059 pydelling-1.9.1/pydelling/managers/BaseStudy.py
+-rw-r--r--   0        0        0     5724 2022-11-21 17:12:37.746200 pydelling-1.9.1/pydelling/managers/PflotranManager.py
+-rw-r--r--   0        0        0    11793 2022-11-07 19:53:46.470323 pydelling-1.9.1/pydelling/managers/PflotranPostprocessing.py
+-rw-r--r--   0        0        0    10477 2022-11-21 17:12:37.746348 pydelling-1.9.1/pydelling/managers/PflotranStudy.py
+-rw-r--r--   0        0        0      241 2022-11-07 19:53:46.470486 pydelling-1.9.1/pydelling/managers/__init__.py
+-rw-r--r--   0        0        0      909 2022-11-07 19:53:46.470601 pydelling-1.9.1/pydelling/managers/callbacks/BaseCallback.py
+-rw-r--r--   0        0        0     1250 2022-11-21 17:12:37.746560 pydelling-1.9.1/pydelling/managers/callbacks/PflotranRestartCallback.py
+-rw-r--r--   0        0        0     2339 2022-11-07 19:53:46.470800 pydelling-1.9.1/pydelling/managers/callbacks/PflotranSaveResultsCallback.py
+-rw-r--r--   0        0        0      168 2022-11-07 19:53:46.470881 pydelling-1.9.1/pydelling/managers/callbacks/__init__.py
+-rw-r--r--   0        0        0    17057 2022-11-07 19:53:46.471041 pydelling-1.9.1/pydelling/paraview_processor/ParaviewProcessor.py
+-rw-r--r--   0        0        0       48 2022-11-07 19:53:46.471131 pydelling-1.9.1/pydelling/paraview_processor/__init__.py
+-rw-r--r--   0        0        0      475 2022-11-07 19:53:46.471254 pydelling-1.9.1/pydelling/paraview_processor/filters/AppendArcLengthFilter.py
+-rw-r--r--   0        0        0     4162 2022-11-07 19:53:46.471346 pydelling-1.9.1/pydelling/paraview_processor/filters/BaseFilter.py
+-rw-r--r--   0        0        0     1225 2022-11-07 19:53:46.471470 pydelling-1.9.1/pydelling/paraview_processor/filters/CalculatorFilter.py
+-rw-r--r--   0        0        0      507 2022-11-07 19:53:46.471550 pydelling-1.9.1/pydelling/paraview_processor/filters/CellDataToPointDataFilter.py
+-rw-r--r--   0        0        0     1070 2022-11-07 19:53:46.471644 pydelling-1.9.1/pydelling/paraview_processor/filters/ClipFilter.py
+-rw-r--r--   0        0        0     1411 2022-11-07 19:53:46.471733 pydelling-1.9.1/pydelling/paraview_processor/filters/CsvReaderFilter.py
+-rw-r--r--   0        0        0      712 2022-11-07 19:53:46.471831 pydelling-1.9.1/pydelling/paraview_processor/filters/IntegrateVariablesFilter.py
+-rw-r--r--   0        0        0     2332 2022-11-07 19:53:46.472080 pydelling-1.9.1/pydelling/paraview_processor/filters/PlotOverLineFilter.py
+-rw-r--r--   0        0        0      638 2022-11-07 19:53:46.472259 pydelling-1.9.1/pydelling/paraview_processor/filters/SaveDataFilter.py
+-rw-r--r--   0        0        0      907 2022-11-07 19:53:46.472353 pydelling-1.9.1/pydelling/paraview_processor/filters/StreamTracerWithCustomSourceFilter.py
+-rw-r--r--   0        0        0      805 2022-11-07 19:53:46.472434 pydelling-1.9.1/pydelling/paraview_processor/filters/TableToPointsFilter.py
+-rw-r--r--   0        0        0      386 2022-11-07 19:53:46.472521 pydelling-1.9.1/pydelling/paraview_processor/filters/TecplotFilter.py
+-rw-r--r--   0        0        0      823 2022-11-07 19:53:46.472611 pydelling-1.9.1/pydelling/paraview_processor/filters/VtkFilter.py
+-rw-r--r--   0        0        0      821 2022-11-07 19:53:46.472697 pydelling-1.9.1/pydelling/paraview_processor/filters/XDMFFilter.py
+-rw-r--r--   0        0        0      686 2022-11-07 19:53:46.472777 pydelling-1.9.1/pydelling/paraview_processor/filters/__init__.py
+-rw-r--r--   0        0        0      535 2022-11-07 19:53:46.472929 pydelling-1.9.1/pydelling/preprocessing/BasePreprocessing.py
+-rw-r--r--   0        0        0    11578 2022-11-07 19:53:46.473055 pydelling-1.9.1/pydelling/preprocessing/ClosedStlGenerator.py
+-rw-r--r--   0        0        0        0 2022-11-07 19:53:46.473091 pydelling-1.9.1/pydelling/preprocessing/GidPreprocessor.py
+-rw-r--r--   0        0        0     8506 2022-11-07 19:53:46.473320 pydelling-1.9.1/pydelling/preprocessing/STLFromPointCloud.py
+-rw-r--r--   0        0        0      246 2022-11-07 19:53:46.473398 pydelling-1.9.1/pydelling/preprocessing/__init__.py
+-rw-r--r--   0        0        0    15467 2022-11-07 19:53:46.473549 pydelling-1.9.1/pydelling/preprocessing/dfn_preprocessor/DfnPreprocessor.py
+-rw-r--r--   0        0        0    33675 2022-11-07 19:53:46.473786 pydelling-1.9.1/pydelling/preprocessing/dfn_preprocessor/DfnUpscaler.py
+-rw-r--r--   0        0        0     3275 2022-11-07 19:53:46.473893 pydelling-1.9.1/pydelling/preprocessing/dfn_preprocessor/Fault.py
+-rw-r--r--   0        0        0    15024 2022-11-07 19:53:46.474027 pydelling-1.9.1/pydelling/preprocessing/dfn_preprocessor/Fracture.py
+-rw-r--r--   0        0        0     8983 2022-11-07 19:53:46.474095 pydelling-1.9.1/pydelling/preprocessing/dfn_preprocessor/PolygonFracture.py
+-rw-r--r--   0        0        0      183 2022-11-07 19:53:46.474159 pydelling-1.9.1/pydelling/preprocessing/dfn_preprocessor/__init__.py
+-rw-r--r--   0        0        0     3711 2022-11-07 19:53:46.474275 pydelling-1.9.1/pydelling/preprocessing/gid_preprocessor/GidObject.py
+-rw-r--r--   0        0        0     1849 2022-11-07 19:53:46.474351 pydelling-1.9.1/pydelling/preprocessing/gid_preprocessor/Line.py
+-rw-r--r--   0        0        0     1456 2022-11-07 19:53:46.474427 pydelling-1.9.1/pydelling/preprocessing/gid_preprocessor/Point.py
+-rw-r--r--   0        0        0     1768 2022-11-07 19:53:46.474497 pydelling-1.9.1/pydelling/preprocessing/gid_preprocessor/Surface.py
+-rw-r--r--   0        0        0      352 2022-11-07 19:53:46.474566 pydelling-1.9.1/pydelling/preprocessing/gid_preprocessor/_AbstractGidObject.py
+-rw-r--r--   0        0        0      136 2022-11-07 19:53:46.474625 pydelling-1.9.1/pydelling/preprocessing/gid_preprocessor/__init__.py
+-rw-r--r--   0        0        0      970 2022-11-07 19:53:46.474690 pydelling-1.9.1/pydelling/preprocessing/gid_preprocessor/gidobjects.py
+-rw-r--r--   0        0        0    20486 2022-11-07 19:53:46.474864 pydelling-1.9.1/pydelling/preprocessing/mesh_preprocessor/MeshPreprocessor.py
+-rw-r--r--   0        0        0       46 2022-11-07 19:53:46.474946 pydelling-1.9.1/pydelling/preprocessing/mesh_preprocessor/__init__.py
+-rw-r--r--   0        0        0      588 2022-11-07 19:53:46.475063 pydelling-1.9.1/pydelling/preprocessing/mesh_preprocessor/geometry/BaseAbstractMeshObject.py
+-rw-r--r--   0        0        0    13746 2022-11-07 19:53:46.475194 pydelling-1.9.1/pydelling/preprocessing/mesh_preprocessor/geometry/BaseElement.py
+-rw-r--r--   0        0        0     3805 2022-11-07 19:53:46.475278 pydelling-1.9.1/pydelling/preprocessing/mesh_preprocessor/geometry/BaseFace.py
+-rw-r--r--   0        0        0     5760 2022-11-07 19:53:46.475385 pydelling-1.9.1/pydelling/preprocessing/mesh_preprocessor/geometry/HexahedraElement.py
+-rw-r--r--   0        0        0     3912 2022-11-07 19:53:46.475469 pydelling-1.9.1/pydelling/preprocessing/mesh_preprocessor/geometry/PyramidElement.py
+-rw-r--r--   0        0        0     1881 2022-11-07 19:53:46.475549 pydelling-1.9.1/pydelling/preprocessing/mesh_preprocessor/geometry/QuadrilateralFace.py
+-rw-r--r--   0        0        0     3627 2022-11-07 19:53:46.475627 pydelling-1.9.1/pydelling/preprocessing/mesh_preprocessor/geometry/TetrahedraElement.py
+-rw-r--r--   0        0        0      725 2022-11-07 19:53:46.475698 pydelling-1.9.1/pydelling/preprocessing/mesh_preprocessor/geometry/TriangleFace.py
+-rw-r--r--   0        0        0     4782 2022-11-07 19:53:46.475767 pydelling-1.9.1/pydelling/preprocessing/mesh_preprocessor/geometry/WedgeElement.py
+-rw-r--r--   0        0        0      393 2022-11-07 19:53:46.475853 pydelling-1.9.1/pydelling/preprocessing/mesh_preprocessor/geometry/__init__.py
+-rw-r--r--   0        0        0     3656 2022-11-07 19:53:46.475973 pydelling-1.9.1/pydelling/readers/BaseReader.py
+-rw-r--r--   0        0        0     3608 2022-11-07 19:53:46.476046 pydelling-1.9.1/pydelling/readers/CentroidReader.py
+-rw-r--r--   0        0        0     2799 2022-11-07 19:53:46.476132 pydelling-1.9.1/pydelling/readers/ConnectFlowReader.py
+-rw-r--r--   0        0        0     6305 2022-11-07 19:53:46.476229 pydelling-1.9.1/pydelling/readers/FemReader.py
+-rw-r--r--   0        0        0     2245 2022-11-07 19:53:46.476307 pydelling-1.9.1/pydelling/readers/OpenFoamReader.py
+-rw-r--r--   0        0        0     1049 2022-11-07 19:53:46.476392 pydelling-1.9.1/pydelling/readers/PflotranMassBalanceFileReader.py
+-rw-r--r--   0        0        0     5662 2022-11-07 19:53:46.476478 pydelling-1.9.1/pydelling/readers/PflotranObservationPointReader.py
+-rw-r--r--   0        0        0     4047 2022-11-07 19:53:46.476551 pydelling-1.9.1/pydelling/readers/PflotranProcessingUtils.py
+-rw-r--r--   0        0        0    16747 2022-11-07 19:53:46.476684 pydelling-1.9.1/pydelling/readers/PflotranReader.py
+-rw-r--r--   0        0        0    14870 2022-11-07 19:53:46.476809 pydelling-1.9.1/pydelling/readers/RasterFileReader.py
+-rw-r--r--   0        0        0     3127 2022-11-07 19:53:46.476881 pydelling-1.9.1/pydelling/readers/SmeshReader.py
+-rw-r--r--   0        0        0    19446 2022-11-07 19:53:46.476992 pydelling-1.9.1/pydelling/readers/StreamlineReader.py
+-rw-r--r--   0        0        0     2256 2022-11-07 19:53:46.477090 pydelling-1.9.1/pydelling/readers/StructuredGridReader.py
+-rw-r--r--   0        0        0     3872 2022-11-07 19:53:46.477164 pydelling-1.9.1/pydelling/readers/StructuredListReader.py
+-rw-r--r--   0        0        0      249 2022-11-07 19:53:46.477234 pydelling-1.9.1/pydelling/readers/UnstructuredMeshReader.py
+-rw-r--r--   0        0        0     5886 2022-11-07 19:53:46.477325 pydelling-1.9.1/pydelling/readers/VTKMeshReader.py
+-rw-r--r--   0        0        0     1512 2022-11-07 19:53:46.477399 pydelling-1.9.1/pydelling/readers/VtkReader.py
+-rw-r--r--   0        0        0      875 2022-11-07 19:53:46.477473 pydelling-1.9.1/pydelling/readers/__init__.py
+-rw-r--r--   0        0        0       36 2022-11-07 19:53:46.477584 pydelling-1.9.1/pydelling/readers/iGPReader/__init__.py
+-rw-r--r--   0        0        0    10497 2022-11-07 19:53:46.477726 pydelling-1.9.1/pydelling/readers/iGPReader/engines/PostProcessingEngine.py
+-rw-r--r--   0        0        0       54 2022-11-07 19:53:46.477795 pydelling-1.9.1/pydelling/readers/iGPReader/engines/__init__.py
+-rw-r--r--   0        0        0     1540 2022-11-07 19:53:46.477927 pydelling-1.9.1/pydelling/readers/iGPReader/geometry/BaseElement.py
+-rw-r--r--   0        0        0     2673 2022-11-07 19:53:46.478007 pydelling-1.9.1/pydelling/readers/iGPReader/geometry/BaseFace.py
+-rw-r--r--   0        0        0     5280 2022-11-07 19:53:46.478084 pydelling-1.9.1/pydelling/readers/iGPReader/geometry/HexahedraElement.py
+-rw-r--r--   0        0        0     1363 2022-11-07 19:53:46.478156 pydelling-1.9.1/pydelling/readers/iGPReader/geometry/QuadrilateralFace.py
+-rw-r--r--   0        0        0     3318 2022-11-07 19:53:46.478224 pydelling-1.9.1/pydelling/readers/iGPReader/geometry/TetrahedraElement.py
+-rw-r--r--   0        0        0      297 2022-11-07 19:53:46.478452 pydelling-1.9.1/pydelling/readers/iGPReader/geometry/TriangleFace.py
+-rw-r--r--   0        0        0     4356 2022-11-07 19:53:46.478566 pydelling-1.9.1/pydelling/readers/iGPReader/geometry/WedgeElement.py
+-rw-r--r--   0        0        0      291 2022-11-07 19:53:46.478658 pydelling-1.9.1/pydelling/readers/iGPReader/geometry/__init__.py
+-rw-r--r--   0        0        0     6138 2022-11-07 19:53:46.478845 pydelling-1.9.1/pydelling/readers/iGPReader/io/AscReader.py
+-rw-r--r--   0        0        0      426 2022-11-07 19:53:46.478921 pydelling-1.9.1/pydelling/readers/iGPReader/io/BaseReader.py
+-rw-r--r--   0        0        0       27 2022-11-07 19:53:46.478995 pydelling-1.9.1/pydelling/readers/iGPReader/io/BaseWriter.py
+-rw-r--r--   0        0        0    10264 2022-11-07 19:53:46.479096 pydelling-1.9.1/pydelling/readers/iGPReader/io/BoreholeReader.py
+-rw-r--r--   0        0        0     2111 2022-11-07 19:53:46.479168 pydelling-1.9.1/pydelling/readers/iGPReader/io/CsvWriter.py
+-rw-r--r--   0        0        0     4874 2022-11-07 19:53:46.479263 pydelling-1.9.1/pydelling/readers/iGPReader/io/PflotranExplicitWriter.py
+-rw-r--r--   0        0        0     3447 2022-11-07 19:53:46.479356 pydelling-1.9.1/pydelling/readers/iGPReader/io/PflotranImplicitWriter.py
+-rw-r--r--   0        0        0      330 2022-11-07 19:53:46.479441 pydelling-1.9.1/pydelling/readers/iGPReader/io/__init__.py
+-rw-r--r--   0        0        0    45831 2022-11-07 19:53:46.479665 pydelling-1.9.1/pydelling/readers/iGPReader/io/iGPReader.py
+-rw-r--r--   0        0        0     2683 2022-11-07 19:53:46.479843 pydelling-1.9.1/pydelling/readers/iGPReader/utils/RegionOperations.py
+-rw-r--r--   0        0        0       67 2022-11-07 19:53:46.479944 pydelling-1.9.1/pydelling/readers/iGPReader/utils/__init__.py
+-rw-r--r--   0        0        0      978 2022-11-07 19:53:46.480029 pydelling-1.9.1/pydelling/readers/iGPReader/utils/decorators.py
+-rw-r--r--   0        0        0     1024 2022-11-07 19:53:46.480110 pydelling-1.9.1/pydelling/readers/iGPReader/utils/geometry_utils.py
+-rw-r--r--   0        0        0     1234 2022-11-07 19:53:46.480185 pydelling-1.9.1/pydelling/readers/iGPReader/utils/utils.py
+-rw-r--r--   0        0        0     8533 2022-11-07 19:53:46.480340 pydelling-1.9.1/pydelling/tests/Pwall.ex
+-rw-r--r--   0        0        0        0 2022-11-07 19:53:46.480376 pydelling-1.9.1/pydelling/tests/__init__.py
+-rw-r--r--   0        0        0      182 2022-11-07 19:53:46.480490 pydelling-1.9.1/pydelling/tests/_trial_temp/custom_edge_intersections.txt
+-rw-r--r--   0        0        0      179 2022-11-07 19:53:46.480559 pydelling-1.9.1/pydelling/tests/_trial_temp/fracture.obj
+-rw-r--r--   0        0        0       52 2022-11-07 19:53:46.480620 pydelling-1.9.1/pydelling/tests/_trial_temp/gid_batch.bch
+-rw-r--r--   0        0        0      457 2022-11-07 19:53:46.480691 pydelling-1.9.1/pydelling/tests/_trial_temp/test.json
+-rw-r--r--   0        0        0      382 2022-11-07 19:53:46.480750 pydelling-1.9.1/pydelling/tests/_trial_temp/test_dfn.vtk
+-rw-r--r--   0        0        0      282 2022-11-07 19:53:46.480828 pydelling-1.9.1/pydelling/tests/_trial_temp/test_element.obj
+-rw-r--r--   0        0        0      451 2022-11-07 19:53:46.480896 pydelling-1.9.1/pydelling/tests/_trial_temp/test_mesh.vtk
+-rw-r--r--   0        0        0        0 2022-11-07 19:53:46.480980 pydelling-1.9.1/pydelling/tests/interpolation/__init__.py
+-rw-r--r--   0        0        0     1065 2022-11-07 19:53:46.481090 pydelling-1.9.1/pydelling/tests/interpolation/test_base_interpolator.py
+-rw-r--r--   0        0        0      623 2022-11-07 19:53:46.481170 pydelling-1.9.1/pydelling/tests/interpolation/test_kde_estimator.py
+-rw-r--r--   0        0        0      981 2022-11-07 19:53:46.481244 pydelling-1.9.1/pydelling/tests/interpolation/test_sparse_data_interpolator.py
+-rw-r--r--   0        0        0        0 2022-11-07 19:53:46.481330 pydelling-1.9.1/pydelling/tests/managers/__init__.py
+-rw-r--r--   0        0        0     1320 2022-11-07 19:53:46.481425 pydelling-1.9.1/pydelling/tests/managers/test_base_study.py
+-rw-r--r--   0        0        0     2694 2022-11-07 19:53:46.481509 pydelling-1.9.1/pydelling/tests/managers/test_pflotran_study.py
+-rw-r--r--   0        0        0        0 2022-11-07 19:53:46.481681 pydelling-1.9.1/pydelling/tests/preprocessing/DfnPreprocessor/__init__.py
+-rw-r--r--   0        0        0      179 2022-11-07 19:53:46.481758 pydelling-1.9.1/pydelling/tests/preprocessing/DfnPreprocessor/fracture.obj
+-rw-r--r--   0        0        0     2283 2022-11-07 19:53:46.481834 pydelling-1.9.1/pydelling/tests/preprocessing/DfnPreprocessor/test_dfn_preprocessor.py
+-rw-r--r--   0        0        0      151 2022-11-07 19:53:46.481919 pydelling-1.9.1/pydelling/tests/preprocessing/DfnPreprocessor/test_fracture_object.py
+-rw-r--r--   0        0        0    12580 2022-11-07 19:53:46.482014 pydelling-1.9.1/pydelling/tests/preprocessing/DfnPreprocessor/test_intersection.py
+-rw-r--r--   0        0        0     3766 2022-11-07 19:53:46.482093 pydelling-1.9.1/pydelling/tests/preprocessing/DfnPreprocessor/test_upscaling.py
+-rw-r--r--   0        0        0        0 2022-11-07 19:53:46.482161 pydelling-1.9.1/pydelling/tests/preprocessing/MeshPreprocessor/__init__.py
+-rw-r--r--   0        0        0     4144 2022-11-07 19:53:46.482250 pydelling-1.9.1/pydelling/tests/preprocessing/MeshPreprocessor/test_mesh_preprocessor.py
+-rw-r--r--   0        0        0        0 2022-11-07 19:53:46.482278 pydelling-1.9.1/pydelling/tests/preprocessing/__init__.py
+-rw-r--r--   0        0        0      154 2022-11-07 19:53:46.482356 pydelling-1.9.1/pydelling/tests/preprocessing/test_base_preprocessing.py
+-rw-r--r--   0        0        0      152 2022-11-07 19:53:46.482426 pydelling-1.9.1/pydelling/tests/preprocessing/test_dfn_preprocessor.py
+-rw-r--r--   0        0        0     3415 2022-11-07 19:53:46.482510 pydelling-1.9.1/pydelling/tests/preprocessing/test_gid_preprocessor.py
+-rw-r--r--   0        0        0        0 2022-11-07 19:53:46.482594 pydelling-1.9.1/pydelling/tests/readers/__init__.py
+-rwxr-xr-x   0        0        0        0 2022-11-07 19:53:46.482698 pydelling-1.9.1/pydelling/tests/readers/_trial_temp/_trial_marker
+-rw-r--r--   0        0        0      175 2022-11-07 19:53:46.482780 pydelling-1.9.1/pydelling/tests/readers/test_BaseReader.py
+-rw-r--r--   0        0        0      875 2022-11-07 19:53:46.482922 pydelling-1.9.1/pydelling/tests/readers/test_CentroidReader.py
+-rw-r--r--   0        0        0      144 2022-11-07 19:53:46.482989 pydelling-1.9.1/pydelling/tests/readers/test_PflotranReader.py
+-rw-r--r--   0        0        0     1945 2022-11-07 19:53:46.483067 pydelling-1.9.1/pydelling/tests/readers/test_RasterFileReader.py
+-rw-r--r--   0        0        0      412 2022-11-07 19:53:46.483144 pydelling-1.9.1/pydelling/tests/readers/test_SmeshReader.py
+-rw-r--r--   0        0        0      993 2022-11-07 19:53:46.483224 pydelling-1.9.1/pydelling/tests/readers/test_StreamlineReader.py
+-rw-r--r--   0        0        0      407 2022-11-07 19:53:46.483319 pydelling-1.9.1/pydelling/tests/readers/test_fem_reader.py
+-rw-r--r--   0        0        0     3746 2022-11-07 19:53:46.483407 pydelling-1.9.1/pydelling/tests/readers/test_iGPReader.py
+-rw-r--r--   0        0        0       90 2022-11-07 19:53:46.483482 pydelling-1.9.1/pydelling/tests/silly_test.py
+-rw-r--r--   0        0        0      457 2022-11-07 19:53:46.483566 pydelling-1.9.1/pydelling/tests/test.json
+-rw-r--r--   0        0        0  1429424 2022-11-07 19:53:46.489794 pydelling-1.9.1/pydelling/tests/test_data/bottom_surface.asc
+-rw-r--r--   0        0        0       81 2022-11-07 19:53:46.489946 pydelling-1.9.1/pydelling/tests/test_data/centroid_reader_data.csv
+-rwxr-xr-x   0        0        0   267949 2022-11-07 19:53:46.490702 pydelling-1.9.1/pydelling/tests/test_data/fem_reader_data.fem
+-rw-r--r--   0        0        0     1651 2022-11-07 19:53:46.490871 pydelling-1.9.1/pydelling/tests/test_data/problematic_fractures/issue_element_1.pkl
+-rw-r--r--   0        0        0     2356 2022-11-07 19:53:46.490956 pydelling-1.9.1/pydelling/tests/test_data/problematic_fractures/issue_element_2.pkl
+-rw-r--r--   0        0        0     4974 2022-11-07 19:53:46.491051 pydelling-1.9.1/pydelling/tests/test_data/problematic_fractures/issue_fracture_1.pkl
+-rw-r--r--   0        0        0    10207 2022-11-07 19:53:46.491154 pydelling-1.9.1/pydelling/tests/test_data/problematic_fractures/issue_fracture_2.pkl
+-rw-r--r--   0        0        0       81 2022-11-07 19:53:46.491239 pydelling-1.9.1/pydelling/tests/test_data/smesh_test_data.smesh
+-rw-r--r--   0        0        0   132941 2022-11-07 19:53:46.491798 pydelling-1.9.1/pydelling/tests/test_data/streamline_test_data.csv
+-rwxr-xr-x   0        0        0    84084 2022-11-07 19:53:46.492154 pydelling-1.9.1/pydelling/tests/test_data/test_fault.stl
+-rw-r--r--   0        0        0        0 2022-11-07 19:53:46.492416 pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/PFLOTRAN/PFLOTRANrun/OutputScreen.dat
+-rw-r--r--   0        0        0     3685 2022-11-07 19:53:46.492555 pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/PFLOTRAN/PFLOTRANrun/test_implicit_to_explicit.in
+-rw-r--r--   0        0        0     3685 2022-11-07 19:53:46.492654 pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/PFLOTRAN/test_implicit_to_explicit.in
+-rw-r--r--   0        0        0    28492 2022-11-07 19:53:46.492802 pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/centroid.dat
+-rw-r--r--   0        0        0    30249 2022-11-07 19:53:46.493252 pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/data.mesh
+-rw-r--r--   0        0        0   137588 2022-11-07 19:53:46.493450 pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/explicit_mesh.mesh
+-rw-r--r--   0        0        0     2890 2022-11-07 19:53:46.493561 pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/source.ss
+-rw-r--r--   0        0        0     3599 2022-11-07 19:53:46.493651 pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/test_implicit_to_explicit-4.dat
+-rw-r--r--   0        0        0     3815 2022-11-07 19:53:46.493739 pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/test_implicit_to_explicit.geo
+-rw-r--r--   0        0        0    63980 2022-11-07 19:53:46.493950 pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/test_implicit_to_explicit.msh
+-rw-r--r--   0        0        0    10426 2022-11-07 19:53:46.494092 pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/test_implicit_to_explicit.png
+-rw-r--r--   0        0        0     1098 2022-11-07 19:53:46.494169 pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/test_implicit_to_explicit.rdr
+-rw-r--r--   0        0        0      143 2022-11-07 19:53:46.494259 pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/test_implicit_to_explicit.tree
+-rw-r--r--   0        0        0     1492 2022-11-07 19:53:46.494361 pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/test_implicit_to_explicit.vv
+-rw-r--r--   0        0        0    10439 2022-11-07 19:53:46.494476 pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/top_surface.ex
+-rw-r--r--   0        0        0     5125 2022-11-07 19:53:46.494584 pydelling-1.9.1/pydelling/tests/test_data/test_manager.in
+-rw-r--r--   0        0        0     5075 2022-11-07 19:53:46.494663 pydelling-1.9.1/pydelling/tests/test_data/test_pflotran_manager_nocheckpoint.in
+-rw-r--r--   0        0        0  1429989 2022-11-07 19:53:46.495599 pydelling-1.9.1/pydelling/tests/test_data/top_surface.asc
+-rw-r--r--   0        0        0        0 2022-11-07 19:53:46.495740 pydelling-1.9.1/pydelling/tests/utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-07 19:53:46.495854 pydelling-1.9.1/pydelling/tests/utils/geometry/__init__.py
+-rwxr-xr-x   0        0        0        0 2022-11-07 19:53:46.495956 pydelling-1.9.1/pydelling/tests/utils/geometry/_trial_temp/_trial_marker
+-rw-r--r--   0        0        0      755 2022-11-07 19:53:46.496529 pydelling-1.9.1/pydelling/tests/utils/geometry/random_test.py
+-rw-r--r--   0        0        0     3011 2022-11-07 19:53:46.497211 pydelling-1.9.1/pydelling/tests/utils/geometry/test_Line.py
+-rw-r--r--   0        0        0      600 2022-11-07 19:53:46.497338 pydelling-1.9.1/pydelling/tests/utils/geometry/test_Plane.py
+-rw-r--r--   0        0        0      517 2022-11-07 19:53:46.497436 pydelling-1.9.1/pydelling/tests/utils/geometry/test_Point.py
+-rw-r--r--   0        0        0     2209 2022-11-07 19:53:46.497550 pydelling-1.9.1/pydelling/tests/utils/test_geometry_utils.py
+-rw-r--r--   0        0        0        0 2022-11-07 19:53:46.497798 pydelling-1.9.1/pydelling/tests/writers/__init__.py
+-rw-r--r--   0        0        0     3021 2022-11-07 19:53:46.498029 pydelling-1.9.1/pydelling/utils/SubFishModule.py
+-rw-r--r--   0        0        0       94 2022-11-07 19:53:46.498129 pydelling-1.9.1/pydelling/utils/__init__.py
+-rw-r--r--   0        0        0     1621 2022-11-21 17:12:37.746977 pydelling-1.9.1/pydelling/utils/configuration_utils.py
+-rw-r--r--   0        0        0      214 2022-11-07 19:53:46.498353 pydelling-1.9.1/pydelling/utils/decorators.py
+-rw-r--r--   0        0        0       73 2022-11-07 19:53:46.498506 pydelling-1.9.1/pydelling/utils/geometry/BasePrimitive.py
+-rw-r--r--   0        0        0     2311 2022-11-07 19:53:46.498610 pydelling-1.9.1/pydelling/utils/geometry/Line.py
+-rw-r--r--   0        0        0     1516 2022-11-07 19:53:46.498717 pydelling-1.9.1/pydelling/utils/geometry/Plane.py
+-rw-r--r--   0        0        0     1056 2022-11-07 19:53:46.498807 pydelling-1.9.1/pydelling/utils/geometry/Point.py
+-rw-r--r--   0        0        0      924 2022-11-07 19:53:46.498893 pydelling-1.9.1/pydelling/utils/geometry/Polygon.py
+-rw-r--r--   0        0        0      204 2022-11-07 19:53:46.498965 pydelling-1.9.1/pydelling/utils/geometry/Scalar.py
+-rw-r--r--   0        0        0     1098 2022-11-07 19:53:46.499062 pydelling-1.9.1/pydelling/utils/geometry/Segment.py
+-rw-r--r--   0        0        0      967 2022-11-07 19:53:46.499249 pydelling-1.9.1/pydelling/utils/geometry/Vector.py
+-rw-r--r--   0        0        0      196 2022-11-07 19:53:46.499442 pydelling-1.9.1/pydelling/utils/geometry/__init__.py
+-rw-r--r--   0        0        0     2432 2022-11-07 19:53:46.499582 pydelling-1.9.1/pydelling/utils/geometry/intersections.py
+-rw-r--r--   0        0        0     3569 2022-11-07 19:53:46.499711 pydelling-1.9.1/pydelling/utils/geometry_utils.py
+-rw-r--r--   0        0        0     2166 2022-11-07 19:53:46.499844 pydelling-1.9.1/pydelling/utils/utility_subclasses.py
+-rw-r--r--   0        0        0    11921 2022-11-07 19:53:46.499970 pydelling-1.9.1/pydelling/utils/utils.py
+-rw-r--r--   0        0        0       74 2022-11-07 19:53:46.500147 pydelling-1.9.1/pydelling/webapps/.streamlit/config.toml
+-rw-r--r--   0        0        0      998 2022-11-07 19:53:46.500260 pydelling-1.9.1/pydelling/webapps/BaseStreamlitUtilityClass.py
+-rw-r--r--   0        0        0      992 2022-11-07 19:53:46.500345 pydelling-1.9.1/pydelling/webapps/WebAppRunner.py
+-rw-r--r--   0        0        0      103 2022-11-07 19:53:46.500420 pydelling-1.9.1/pydelling/webapps/__init__.py
+-rw-r--r--   0        0        0     1280 2022-11-07 19:53:46.500537 pydelling-1.9.1/pydelling/webapps/components/BaseComponent.py
+-rw-r--r--   0        0        0     5974 2022-11-07 19:53:46.500631 pydelling-1.9.1/pydelling/webapps/components/InputComponent.py
+-rw-r--r--   0        0        0     4095 2022-11-07 19:53:46.500723 pydelling-1.9.1/pydelling/webapps/components/RemoteLoginComponent.py
+-rw-r--r--   0        0        0      138 2022-11-07 19:53:46.500799 pydelling-1.9.1/pydelling/webapps/components/__init__.py
+-rw-r--r--   0        0        0      765 2022-11-07 19:53:46.500936 pydelling-1.9.1/pydelling/webapps/webapps/pflotran_runner_webapp.py
+-rw-r--r--   0        0        0     8480 2022-11-07 19:53:46.501128 pydelling-1.9.1/pydelling/webapps/webapps/sparse_interpolator_webapp.py
+-rw-r--r--   0        0        0      771 2022-11-07 19:53:46.501335 pydelling-1.9.1/pydelling/webapps/webapps/test_bash_vtk.py
+-rw-r--r--   0        0        0      236 2022-11-07 19:53:46.501431 pydelling-1.9.1/pydelling/webapps/webapps/test_webapp.py
+-rw-r--r--   0        0        0     3093 2022-11-07 19:53:46.501654 pydelling-1.9.1/pydelling/writers/BaseWriter.py
+-rw-r--r--   0        0        0     5586 2022-11-07 19:53:46.501786 pydelling-1.9.1/pydelling/writers/HDF5CentroidWriter.py
+-rw-r--r--   0        0        0     5126 2022-11-21 17:12:37.747099 pydelling-1.9.1/pydelling/writers/HDF5RasterWriter.py
+-rw-r--r--   0        0        0     3791 2022-11-07 19:53:46.502078 pydelling-1.9.1/pydelling/writers/OpenFoamVariableWriter.py
+-rw-r--r--   0        0        0      191 2022-11-07 19:53:46.502172 pydelling-1.9.1/pydelling/writers/__init__.py
+-rw-r--r--   0        0        0      836 2022-11-21 17:31:58.879743 pydelling-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     3847 1970-01-01 00:00:00.000000 pydelling-1.9.1/setup.py
+-rw-r--r--   0        0        0     2459 1970-01-01 00:00:00.000000 pydelling-1.9.1/PKG-INFO
```

### Comparing `pydelling-1.9/LICENSE.txt` & `pydelling-1.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/README.md` & `pydelling-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/config/__init__.py` & `pydelling-1.9.1/pydelling/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/config/conda_env.yaml` & `pydelling-1.9.1/pydelling/config/conda_env.yaml`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/config/logger_config.yaml` & `pydelling-1.9.1/pydelling/config/logger_config.yaml`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/interpolation/BaseInterpolator.py` & `pydelling-1.9.1/pydelling/interpolation/BaseInterpolator.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/interpolation/KdeEstimator.py` & `pydelling-1.9.1/pydelling/interpolation/KdeEstimator.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/interpolation/SparseDataInterpolator.py` & `pydelling-1.9.1/pydelling/interpolation/SparseDataInterpolator.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/managers/BaseManager.py` & `pydelling-1.9.1/pydelling/managers/BaseManager.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/managers/BaseStudy.py` & `pydelling-1.9.1/pydelling/managers/BaseStudy.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/managers/PflotranManager.py` & `pydelling-1.9.1/pydelling/managers/PflotranManager.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/managers/PflotranPostprocessing.py` & `pydelling-1.9.1/pydelling/managers/PflotranPostprocessing.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/managers/PflotranStudy.py` & `pydelling-1.9.1/pydelling/managers/PflotranStudy.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/managers/callbacks/BaseCallback.py` & `pydelling-1.9.1/pydelling/managers/callbacks/BaseCallback.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/managers/callbacks/PflotranRestartCallback.py` & `pydelling-1.9.1/pydelling/managers/callbacks/PflotranRestartCallback.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/managers/callbacks/PflotranSaveResultsCallback.py` & `pydelling-1.9.1/pydelling/managers/callbacks/PflotranSaveResultsCallback.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/paraview_processor/ParaviewProcessor.py` & `pydelling-1.9.1/pydelling/paraview_processor/ParaviewProcessor.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/paraview_processor/filters/BaseFilter.py` & `pydelling-1.9.1/pydelling/paraview_processor/filters/BaseFilter.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/paraview_processor/filters/CalculatorFilter.py` & `pydelling-1.9.1/pydelling/paraview_processor/filters/CalculatorFilter.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/paraview_processor/filters/ClipFilter.py` & `pydelling-1.9.1/pydelling/paraview_processor/filters/ClipFilter.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/paraview_processor/filters/CsvReaderFilter.py` & `pydelling-1.9.1/pydelling/paraview_processor/filters/CsvReaderFilter.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/paraview_processor/filters/IntegrateVariablesFilter.py` & `pydelling-1.9.1/pydelling/paraview_processor/filters/IntegrateVariablesFilter.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/paraview_processor/filters/PlotOverLineFilter.py` & `pydelling-1.9.1/pydelling/paraview_processor/filters/PlotOverLineFilter.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/paraview_processor/filters/SaveDataFilter.py` & `pydelling-1.9.1/pydelling/paraview_processor/filters/SaveDataFilter.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/paraview_processor/filters/StreamTracerWithCustomSourceFilter.py` & `pydelling-1.9.1/pydelling/paraview_processor/filters/StreamTracerWithCustomSourceFilter.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/paraview_processor/filters/TableToPointsFilter.py` & `pydelling-1.9.1/pydelling/paraview_processor/filters/TableToPointsFilter.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/paraview_processor/filters/VtkFilter.py` & `pydelling-1.9.1/pydelling/paraview_processor/filters/VtkFilter.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/paraview_processor/filters/XDMFFilter.py` & `pydelling-1.9.1/pydelling/paraview_processor/filters/XDMFFilter.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/paraview_processor/filters/__init__.py` & `pydelling-1.9.1/pydelling/paraview_processor/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/preprocessing/BasePreprocessing.py` & `pydelling-1.9.1/pydelling/preprocessing/BasePreprocessing.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/preprocessing/ClosedStlGenerator.py` & `pydelling-1.9.1/pydelling/preprocessing/ClosedStlGenerator.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/preprocessing/STLFromPointCloud.py` & `pydelling-1.9.1/pydelling/preprocessing/STLFromPointCloud.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/preprocessing/dfn_preprocessor/DfnPreprocessor.py` & `pydelling-1.9.1/pydelling/preprocessing/dfn_preprocessor/DfnPreprocessor.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/preprocessing/dfn_preprocessor/DfnUpscaler.py` & `pydelling-1.9.1/pydelling/preprocessing/dfn_preprocessor/DfnUpscaler.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/preprocessing/dfn_preprocessor/Fault.py` & `pydelling-1.9.1/pydelling/preprocessing/dfn_preprocessor/Fault.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/preprocessing/dfn_preprocessor/Fracture.py` & `pydelling-1.9.1/pydelling/preprocessing/dfn_preprocessor/Fracture.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/preprocessing/dfn_preprocessor/PolygonFracture.py` & `pydelling-1.9.1/pydelling/preprocessing/dfn_preprocessor/PolygonFracture.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/preprocessing/gid_preprocessor/GidObject.py` & `pydelling-1.9.1/pydelling/preprocessing/gid_preprocessor/GidObject.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/preprocessing/gid_preprocessor/Line.py` & `pydelling-1.9.1/pydelling/preprocessing/gid_preprocessor/Line.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/preprocessing/gid_preprocessor/Point.py` & `pydelling-1.9.1/pydelling/preprocessing/gid_preprocessor/Point.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/preprocessing/gid_preprocessor/Surface.py` & `pydelling-1.9.1/pydelling/preprocessing/gid_preprocessor/Surface.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/preprocessing/gid_preprocessor/gidobjects.py` & `pydelling-1.9.1/pydelling/preprocessing/gid_preprocessor/gidobjects.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/preprocessing/mesh_preprocessor/MeshPreprocessor.py` & `pydelling-1.9.1/pydelling/preprocessing/mesh_preprocessor/MeshPreprocessor.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/preprocessing/mesh_preprocessor/geometry/BaseAbstractMeshObject.py` & `pydelling-1.9.1/pydelling/preprocessing/mesh_preprocessor/geometry/BaseAbstractMeshObject.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/preprocessing/mesh_preprocessor/geometry/BaseElement.py` & `pydelling-1.9.1/pydelling/preprocessing/mesh_preprocessor/geometry/BaseElement.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/preprocessing/mesh_preprocessor/geometry/BaseFace.py` & `pydelling-1.9.1/pydelling/preprocessing/mesh_preprocessor/geometry/BaseFace.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/preprocessing/mesh_preprocessor/geometry/HexahedraElement.py` & `pydelling-1.9.1/pydelling/preprocessing/mesh_preprocessor/geometry/HexahedraElement.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/preprocessing/mesh_preprocessor/geometry/PyramidElement.py` & `pydelling-1.9.1/pydelling/preprocessing/mesh_preprocessor/geometry/PyramidElement.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/preprocessing/mesh_preprocessor/geometry/QuadrilateralFace.py` & `pydelling-1.9.1/pydelling/preprocessing/mesh_preprocessor/geometry/QuadrilateralFace.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/preprocessing/mesh_preprocessor/geometry/TetrahedraElement.py` & `pydelling-1.9.1/pydelling/preprocessing/mesh_preprocessor/geometry/TetrahedraElement.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/preprocessing/mesh_preprocessor/geometry/TriangleFace.py` & `pydelling-1.9.1/pydelling/preprocessing/mesh_preprocessor/geometry/TriangleFace.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/preprocessing/mesh_preprocessor/geometry/WedgeElement.py` & `pydelling-1.9.1/pydelling/preprocessing/mesh_preprocessor/geometry/WedgeElement.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/BaseReader.py` & `pydelling-1.9.1/pydelling/readers/BaseReader.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/CentroidReader.py` & `pydelling-1.9.1/pydelling/readers/CentroidReader.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/ConnectFlowReader.py` & `pydelling-1.9.1/pydelling/readers/ConnectFlowReader.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/FemReader.py` & `pydelling-1.9.1/pydelling/readers/FemReader.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/OpenFoamReader.py` & `pydelling-1.9.1/pydelling/readers/OpenFoamReader.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/PflotranMassBalanceFileReader.py` & `pydelling-1.9.1/pydelling/readers/PflotranMassBalanceFileReader.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/PflotranObservationPointReader.py` & `pydelling-1.9.1/pydelling/readers/PflotranObservationPointReader.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/PflotranProcessingUtils.py` & `pydelling-1.9.1/pydelling/readers/PflotranProcessingUtils.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/PflotranReader.py` & `pydelling-1.9.1/pydelling/readers/PflotranReader.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/RasterFileReader.py` & `pydelling-1.9.1/pydelling/readers/RasterFileReader.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/SmeshReader.py` & `pydelling-1.9.1/pydelling/readers/SmeshReader.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/StreamlineReader.py` & `pydelling-1.9.1/pydelling/readers/StreamlineReader.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/StructuredGridReader.py` & `pydelling-1.9.1/pydelling/readers/StructuredGridReader.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/StructuredListReader.py` & `pydelling-1.9.1/pydelling/readers/StructuredListReader.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/VTKMeshReader.py` & `pydelling-1.9.1/pydelling/readers/VTKMeshReader.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/VtkReader.py` & `pydelling-1.9.1/pydelling/readers/VtkReader.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/__init__.py` & `pydelling-1.9.1/pydelling/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/iGPReader/engines/PostProcessingEngine.py` & `pydelling-1.9.1/pydelling/readers/iGPReader/engines/PostProcessingEngine.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/iGPReader/geometry/BaseElement.py` & `pydelling-1.9.1/pydelling/readers/iGPReader/geometry/BaseElement.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/iGPReader/geometry/BaseFace.py` & `pydelling-1.9.1/pydelling/readers/iGPReader/geometry/BaseFace.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/iGPReader/geometry/HexahedraElement.py` & `pydelling-1.9.1/pydelling/readers/iGPReader/geometry/HexahedraElement.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/iGPReader/geometry/QuadrilateralFace.py` & `pydelling-1.9.1/pydelling/readers/iGPReader/geometry/QuadrilateralFace.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/iGPReader/geometry/TetrahedraElement.py` & `pydelling-1.9.1/pydelling/readers/iGPReader/geometry/TetrahedraElement.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/iGPReader/geometry/WedgeElement.py` & `pydelling-1.9.1/pydelling/readers/iGPReader/geometry/WedgeElement.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/iGPReader/io/AscReader.py` & `pydelling-1.9.1/pydelling/readers/iGPReader/io/AscReader.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/iGPReader/io/BoreholeReader.py` & `pydelling-1.9.1/pydelling/readers/iGPReader/io/BoreholeReader.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/iGPReader/io/CsvWriter.py` & `pydelling-1.9.1/pydelling/readers/iGPReader/io/CsvWriter.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/iGPReader/io/PflotranExplicitWriter.py` & `pydelling-1.9.1/pydelling/readers/iGPReader/io/PflotranExplicitWriter.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/iGPReader/io/PflotranImplicitWriter.py` & `pydelling-1.9.1/pydelling/readers/iGPReader/io/PflotranImplicitWriter.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/iGPReader/io/iGPReader.py` & `pydelling-1.9.1/pydelling/readers/iGPReader/io/iGPReader.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/iGPReader/utils/RegionOperations.py` & `pydelling-1.9.1/pydelling/readers/iGPReader/utils/RegionOperations.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/iGPReader/utils/decorators.py` & `pydelling-1.9.1/pydelling/readers/iGPReader/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/iGPReader/utils/geometry_utils.py` & `pydelling-1.9.1/pydelling/readers/iGPReader/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/readers/iGPReader/utils/utils.py` & `pydelling-1.9.1/pydelling/readers/iGPReader/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/Pwall.ex` & `pydelling-1.9.1/pydelling/tests/Pwall.ex`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/interpolation/test_base_interpolator.py` & `pydelling-1.9.1/pydelling/tests/interpolation/test_base_interpolator.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/interpolation/test_kde_estimator.py` & `pydelling-1.9.1/pydelling/tests/interpolation/test_kde_estimator.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/interpolation/test_sparse_data_interpolator.py` & `pydelling-1.9.1/pydelling/tests/interpolation/test_sparse_data_interpolator.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/managers/test_base_study.py` & `pydelling-1.9.1/pydelling/tests/managers/test_base_study.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/managers/test_pflotran_study.py` & `pydelling-1.9.1/pydelling/tests/managers/test_pflotran_study.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/preprocessing/DfnPreprocessor/test_dfn_preprocessor.py` & `pydelling-1.9.1/pydelling/tests/preprocessing/DfnPreprocessor/test_dfn_preprocessor.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/preprocessing/DfnPreprocessor/test_intersection.py` & `pydelling-1.9.1/pydelling/tests/preprocessing/DfnPreprocessor/test_intersection.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/preprocessing/DfnPreprocessor/test_upscaling.py` & `pydelling-1.9.1/pydelling/tests/preprocessing/DfnPreprocessor/test_upscaling.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/preprocessing/MeshPreprocessor/test_mesh_preprocessor.py` & `pydelling-1.9.1/pydelling/tests/preprocessing/MeshPreprocessor/test_mesh_preprocessor.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/preprocessing/test_gid_preprocessor.py` & `pydelling-1.9.1/pydelling/tests/preprocessing/test_gid_preprocessor.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/readers/test_CentroidReader.py` & `pydelling-1.9.1/pydelling/tests/readers/test_CentroidReader.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/readers/test_RasterFileReader.py` & `pydelling-1.9.1/pydelling/tests/readers/test_RasterFileReader.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/readers/test_StreamlineReader.py` & `pydelling-1.9.1/pydelling/tests/readers/test_StreamlineReader.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/readers/test_iGPReader.py` & `pydelling-1.9.1/pydelling/tests/readers/test_iGPReader.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/test_data/bottom_surface.asc` & `pydelling-1.9.1/pydelling/tests/test_data/bottom_surface.asc`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/test_data/fem_reader_data.fem` & `pydelling-1.9.1/pydelling/tests/test_data/fem_reader_data.fem`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/test_data/problematic_fractures/issue_element_1.pkl` & `pydelling-1.9.1/pydelling/tests/test_data/problematic_fractures/issue_element_1.pkl`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/test_data/problematic_fractures/issue_element_2.pkl` & `pydelling-1.9.1/pydelling/tests/test_data/problematic_fractures/issue_element_2.pkl`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/test_data/problematic_fractures/issue_fracture_1.pkl` & `pydelling-1.9.1/pydelling/tests/test_data/problematic_fractures/issue_fracture_1.pkl`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/test_data/problematic_fractures/issue_fracture_2.pkl` & `pydelling-1.9.1/pydelling/tests/test_data/problematic_fractures/issue_fracture_2.pkl`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/test_data/streamline_test_data.csv` & `pydelling-1.9.1/pydelling/tests/test_data/streamline_test_data.csv`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/test_data/test_fault.stl` & `pydelling-1.9.1/pydelling/tests/test_data/test_fault.stl`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/PFLOTRAN/PFLOTRANrun/test_implicit_to_explicit.in` & `pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/PFLOTRAN/PFLOTRANrun/test_implicit_to_explicit.in`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/PFLOTRAN/test_implicit_to_explicit.in` & `pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/PFLOTRAN/test_implicit_to_explicit.in`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/centroid.dat` & `pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/centroid.dat`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/data.mesh` & `pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/data.mesh`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/explicit_mesh.mesh` & `pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/explicit_mesh.mesh`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/source.ss` & `pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/source.ss`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/test_implicit_to_explicit-4.dat` & `pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/test_implicit_to_explicit-4.dat`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/test_implicit_to_explicit.geo` & `pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/test_implicit_to_explicit.geo`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/test_implicit_to_explicit.msh` & `pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/test_implicit_to_explicit.msh`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/test_implicit_to_explicit.png` & `pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/test_implicit_to_explicit.png`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/test_implicit_to_explicit.rdr` & `pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/test_implicit_to_explicit.rdr`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/test_implicit_to_explicit.vv` & `pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/test_implicit_to_explicit.vv`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/test_data/test_implicit_to_explicit.gid/top_surface.ex` & `pydelling-1.9.1/pydelling/tests/test_data/test_implicit_to_explicit.gid/top_surface.ex`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/test_data/test_manager.in` & `pydelling-1.9.1/pydelling/tests/test_data/test_manager.in`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/test_data/test_pflotran_manager_nocheckpoint.in` & `pydelling-1.9.1/pydelling/tests/test_data/test_pflotran_manager_nocheckpoint.in`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/test_data/top_surface.asc` & `pydelling-1.9.1/pydelling/tests/test_data/top_surface.asc`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/utils/geometry/random_test.py` & `pydelling-1.9.1/pydelling/tests/utils/geometry/random_test.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/utils/geometry/test_Line.py` & `pydelling-1.9.1/pydelling/tests/utils/geometry/test_Line.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/utils/geometry/test_Plane.py` & `pydelling-1.9.1/pydelling/tests/utils/geometry/test_Plane.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/utils/geometry/test_Point.py` & `pydelling-1.9.1/pydelling/tests/utils/geometry/test_Point.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/tests/utils/test_geometry_utils.py` & `pydelling-1.9.1/pydelling/tests/utils/test_geometry_utils.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/utils/SubFishModule.py` & `pydelling-1.9.1/pydelling/utils/SubFishModule.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/utils/configuration_utils.py` & `pydelling-1.9.1/pydelling/utils/configuration_utils.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/utils/geometry/Line.py` & `pydelling-1.9.1/pydelling/utils/geometry/Line.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/utils/geometry/Plane.py` & `pydelling-1.9.1/pydelling/utils/geometry/Plane.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/utils/geometry/Point.py` & `pydelling-1.9.1/pydelling/utils/geometry/Point.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/utils/geometry/Polygon.py` & `pydelling-1.9.1/pydelling/utils/geometry/Polygon.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/utils/geometry/Segment.py` & `pydelling-1.9.1/pydelling/utils/geometry/Segment.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/utils/geometry/Vector.py` & `pydelling-1.9.1/pydelling/utils/geometry/Vector.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/utils/geometry/intersections.py` & `pydelling-1.9.1/pydelling/utils/geometry/intersections.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/utils/geometry_utils.py` & `pydelling-1.9.1/pydelling/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/utils/utility_subclasses.py` & `pydelling-1.9.1/pydelling/utils/utility_subclasses.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/utils/utils.py` & `pydelling-1.9.1/pydelling/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/webapps/BaseStreamlitUtilityClass.py` & `pydelling-1.9.1/pydelling/webapps/BaseStreamlitUtilityClass.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/webapps/WebAppRunner.py` & `pydelling-1.9.1/pydelling/webapps/WebAppRunner.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/webapps/components/BaseComponent.py` & `pydelling-1.9.1/pydelling/webapps/components/BaseComponent.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/webapps/components/InputComponent.py` & `pydelling-1.9.1/pydelling/webapps/components/InputComponent.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/webapps/components/RemoteLoginComponent.py` & `pydelling-1.9.1/pydelling/webapps/components/RemoteLoginComponent.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/webapps/webapps/pflotran_runner_webapp.py` & `pydelling-1.9.1/pydelling/webapps/webapps/pflotran_runner_webapp.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/webapps/webapps/sparse_interpolator_webapp.py` & `pydelling-1.9.1/pydelling/webapps/webapps/sparse_interpolator_webapp.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/webapps/webapps/test_bash_vtk.py` & `pydelling-1.9.1/pydelling/webapps/webapps/test_bash_vtk.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/writers/BaseWriter.py` & `pydelling-1.9.1/pydelling/writers/BaseWriter.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/writers/HDF5CentroidWriter.py` & `pydelling-1.9.1/pydelling/writers/HDF5CentroidWriter.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/writers/HDF5RasterWriter.py` & `pydelling-1.9.1/pydelling/writers/HDF5RasterWriter.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pydelling/writers/OpenFoamVariableWriter.py` & `pydelling-1.9.1/pydelling/writers/OpenFoamVariableWriter.py`

 * *Files identical despite different names*

### Comparing `pydelling-1.9/pyproject.toml` & `pydelling-1.9.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydelling"
-version = "1.9"
+version = "1.9.1"
 description = "Package providing a variety of utility methods for mathematical modelling"
 authors = ["Aitor <aitirga@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
```

### Comparing `pydelling-1.9/setup.py` & `pydelling-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
  'tqdm',
  'trimesh',
  'vtk',
  'xlrd']
 
 setup_kwargs = {
     'name': 'pydelling',
-    'version': '1.9',
+    'version': '1.9.1',
     'description': 'Package providing a variety of utility methods for mathematical modelling',
     'long_description': ' # Pydelling\nSet of pre- and post-processing scripts for modelling\n\n\n## Recommendations\n\nUsing and IDE like PyCharm is recommended to keep things easy. It may be useful if you need to debug your scripts,\nor edit them.\n\nUsing PyCharm, you can follow the installation step and then run your scripts in pydelling env automatically.\nOtherwise, you can follow the steps below to run pydelling manually. \n\n\n## Installation\nConfigure the conda environment running\n\n`conda env create --file environment.yaml`\n\nRegular pip dependencies can be found at `requirements.txt`\n\n\n## Templates and Examples\n\nSome examples of usage of pydelling may be found inside `templates` folder. Use `config.yaml` to setup data sources and \nother variables.\n\n\n## Running template scripts\n\nIn order to execute pydelling, `pydelling` conda env needs to be loaded.\n\n\n### Loading conda environment\n\n`conda activate pydelling`\n\n### Running script\n\nRun the script and set the config file as argument. If the config file is not specified, `./config.yaml` will be taken as default.\n\nExample: \n\n`python templates\\interpolate_top_BC\\interpolate_BC.py templates\\interpolate_top_BC\\config.yaml`\n\n',
     'author': 'Aitor',
     'author_email': 'aitirga@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pydelling-1.9/PKG-INFO` & `pydelling-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydelling
-Version: 1.9
+Version: 1.9.1
 Summary: Package providing a variety of utility methods for mathematical modelling
 License: MIT
 Author: Aitor
 Author-email: aitirga@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


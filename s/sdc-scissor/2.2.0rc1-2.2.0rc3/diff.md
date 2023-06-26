# Comparing `tmp/sdc_scissor-2.2.0rc1.tar.gz` & `tmp/sdc_scissor-2.2.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdc_scissor-2.2.0rc1.tar", max compression
+gzip compressed data, was "sdc_scissor-2.2.0rc3.tar", max compression
```

## Comparing `sdc_scissor-2.2.0rc1.tar` & `sdc_scissor-2.2.0rc3.tar`

### file list

```diff
@@ -1,127 +1,127 @@
--rw-r--r--   0        0        0    34916 2023-05-24 05:30:02.113529 sdc_scissor-2.2.0rc1/LICENSE.md
--rw-r--r--   0        0        0    10829 2023-05-24 05:30:02.113529 sdc_scissor-2.2.0rc1/README.md
--rw-r--r--   0        0        0     1461 2023-05-24 05:30:02.205530 sdc_scissor-2.2.0rc1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/can_api/__init__.py
--rw-r--r--   0        0        0     4671 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/can_api/can_bus_handler.py
--rw-r--r--   0        0        0     1730 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/can_api/can_msg_generator.py
--rw-r--r--   0        0        0     3907 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/can_api/can_output.py
--rw-r--r--   0        0        0    18875 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/cli.py
--rw-r--r--   0        0        0     1448 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/config.py
--rw-r--r--   0        0        0        0 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/feature_extraction_api/__init__.py
--rw-r--r--   0        0        0     4763 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/feature_extraction_api/angle_based_strategy.py
--rw-r--r--   0        0        0     3980 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/feature_extraction_api/equi_distance_strategy.py
--rw-r--r--   0        0        0    10519 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/feature_extraction_api/feature_extraction.py
--rw-r--r--   0        0        0     2587 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/feature_extraction_api/parameterized_uniform_strategy.py
--rw-r--r--   0        0        0     3203 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/feature_extraction_api/road_geometry_calculator.py
--rw-r--r--   0        0        0      401 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/feature_extraction_api/segmentation_strategy.py
--rw-r--r--   0        0        0        0 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/machine_learning_api/__init__.py
--rw-r--r--   0        0        0     9597 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/machine_learning_api/cost_effectiveness_evaluator.py
--rw-r--r--   0        0        0      255 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/machine_learning_api/csv_loader.py
--rw-r--r--   0        0        0     7726 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/machine_learning_api/model_evaluator.py
--rw-r--r--   0        0        0     2382 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/machine_learning_api/predictor.py
--rw-r--r--   0        0        0        0 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/obstacle_api/__init__.py
--rw-r--r--   0        0        0      643 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/obstacle_api/beamng_bump.py
--rw-r--r--   0        0        0      569 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/obstacle_api/beamng_delineator.py
--rw-r--r--   0        0        0      764 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/obstacle_api/beamng_obstacle_factory.py
--rw-r--r--   0        0        0      675 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/obstacle_api/beamng_tree.py
--rw-r--r--   0        0        0      828 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/obstacle_api/bump.py
--rw-r--r--   0        0        0      160 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/obstacle_api/carla_bump.py
--rw-r--r--   0        0        0      190 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/obstacle_api/carla_delineator.py
--rw-r--r--   0        0        0      753 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/obstacle_api/carla_obstacle_factory.py
--rw-r--r--   0        0        0      160 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/obstacle_api/carla_tree.py
--rw-r--r--   0        0        0      664 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/obstacle_api/delineator.py
--rw-r--r--   0        0        0      522 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/obstacle_api/obstacle_factory.py
--rw-r--r--   0        0        0      709 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/obstacle_api/tree.py
--rw-r--r--   0        0        0      966 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/Dockerfile.testPrioritization
--rw-r--r--   0        0        0       95 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/README.md
--rw-r--r--   0        0        0        0 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/__init__.py
--rw-r--r--   0        0        0      510 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/faultDetection.m
--rw-r--r--   0        0        0     6298 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/faultDetectionRatePlots.m
--rw-r--r--   0        0        0      463 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/featureSelection.m
--rw-r--r--   0        0        0      391 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/fitness.m
--rw-r--r--   0        0        0     1075 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/initialPopulation.m
--rw-r--r--   0        0        0      574 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/main.m
--rw-r--r--   0        0        0      609 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/mainGreedy.m
--rw-r--r--   0        0        0      220 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/objectives.m
--rw-r--r--   0        0        0      750 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/permutationCrossover.m
--rw-r--r--   0        0        0     1501 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/permutationMutation.m
--rw-r--r--   0        0        0      302 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/plotResults.m
--rw-r--r--   0        0        0     1367 2023-05-24 05:30:02.249531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/python/make-single-csv.py
--rw-r--r--   0        0        0    10251 2023-05-24 05:30:02.253531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/r-script/analysis.R
--rw-r--r--   0        0        0     5034 2023-05-24 05:30:02.253531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/r-script/better_rate.pdf
--rw-r--r--   0        0        0     2128 2023-05-24 05:30:02.253531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/r-script/gavsga.csv
--rw-r--r--   0        0        0      125 2023-05-24 05:30:02.253531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/r-script/medians_APFDc.csv
--rw-r--r--   0        0        0     1869 2023-05-24 05:30:02.253531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/r-script/plot.R
--rw-r--r--   0        0        0     1694 2023-05-24 05:30:02.253531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/r-script/table.R
--rw-r--r--   0        0        0      395 2023-05-24 05:30:02.253531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/r-script/utils.R
--rw-r--r--   0        0        0      584 2023-05-24 05:30:02.253531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/r-script/vsbl.csv
--rw-r--r--   0        0        0      958 2023-05-24 05:30:02.253531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/r-script/vsrand.csv
--rw-r--r--   0        0        0     1051 2023-05-24 05:30:02.253531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/runGreedy.m
--rw-r--r--   0        0        0     4258 2023-05-24 05:30:02.253531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/runMOSearch.m
--rw-r--r--   0        0        0     3480 2023-05-24 05:30:02.253531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/runSearch.m
--rw-r--r--   0        0        0   239182 2023-05-24 05:30:02.253531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1/BeamNG_RF_1_Complete.csv
--rw-r--r--   0        0        0  1146691 2023-05-24 05:30:02.261531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_Complete.csv
--rw-r--r--   0        0        0   440097 2023-05-24 05:30:02.265531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_selected.csv
--rw-r--r--   0        0        0     1070 2023-05-24 05:30:02.265531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/filter.py
--rw-r--r--   0        0        0   353423 2023-05-24 05:30:02.265531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_2/BeamNG_RF_2_Complete.csv
--rw-r--r--   0        0        0      660 2023-05-24 05:30:02.265531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/README.md
--rw-r--r--   0        0        0  1142098 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/datasets/fullroad/Driver_AI/DriverAI_Complete.csv
--rw-r--r--   0        0        0     4431 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/datasets/fullroad/README.md
--rw-r--r--   0        0        0      650 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/docker_scripts/build-test-prioritization-image.sh
--rw-r--r--   0        0        0      725 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/docker_scripts/run-test-prioritization-container.sh
--rw-r--r--   0        0        0       65 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/requirements.txt
--rw-r--r--   0        0        0      324 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/setup.cfg
--rw-r--r--   0        0        0       38 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/setup.py
--rw-r--r--   0        0        0     2413 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/testPrioritization/README.md
--rw-r--r--   0        0        0        0 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/testPrioritization/__init__.py
--rw-r--r--   0        0        0      780 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/testPrioritization/crossover/PMX.py
--rw-r--r--   0        0        0     1306 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/testPrioritization/mutation/HybridMut.py
--rw-r--r--   0        0        0      843 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/testPrioritization/problem/TestPrioritizationMultiObjectiveProblem.py
--rw-r--r--   0        0        0     7798 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/testPrioritization/run.py
--rw-r--r--   0        0        0        0 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/simulator_api/__init__.py
--rw-r--r--   0        0        0     1661 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/simulator_api/abstract_simulator.py
--rw-r--r--   0        0        0     6672 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/simulator_api/beamng_simulator.py
--rw-r--r--   0        0        0      807 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/simulator_api/simulator_factory.py
--rw-r--r--   0        0        0        0 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/__init__.py
--rw-r--r--   0        0        0      424 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/road_model.py
--rw-r--r--   0        0        0     2323 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test.py
--rw-r--r--   0        0        0     5482 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generator.py
--rw-r--r--   0        0        0    13513 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/ambiegen/Utils/car_road.py
--rw-r--r--   0        0        0      304 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/ambiegen/Utils/duplicate_elimination.py
--rw-r--r--   0        0        0      862 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/ambiegen/Utils/generate_test_case_sampling.py
--rw-r--r--   0        0        0    13276 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/ambiegen/Utils/road_gen.py
--rw-r--r--   0        0        0     2443 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/ambiegen/Utils/solution.py
--rw-r--r--   0        0        0     2580 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_crossover.py
--rw-r--r--   0        0        0     3786 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_mutation.py
--rw-r--r--   0        0        0      587 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_problem.py
--rw-r--r--   0        0        0     8854 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/ambiegen/Utils/vehicle.py
--rw-r--r--   0        0        0        0 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/ambiegen/__init__.py
--rw-r--r--   0        0        0     2829 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/ambiegen/ambiegen_generator.py
--rw-r--r--   0        0        0      575 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/ambiegen/config.py
--rw-r--r--   0        0        0        0 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic/__init__.py
--rw-r--r--   0        0        0     1067 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic/src/LICENSE
--rw-r--r--   0        0        0        0 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic/src/__init__.py
--rw-r--r--   0        0        0   372723 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic/src/frenetic-sbst21-preprint.pdf
--rw-r--r--   0        0        0        0 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic/src/generators/__init__.py
--rw-r--r--   0        0        0     2658 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_frenet_generator.py
--rw-r--r--   0        0        0     4908 2023-05-24 05:30:02.269531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_generator.py
--rw-r--r--   0        0        0    14117 2023-05-24 05:30:02.273531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic/src/generators/random_frenet_generator.py
--rw-r--r--   0        0        0        0 2023-05-24 05:30:02.273531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic/src/utils/__init__.py
--rw-r--r--   0        0        0      731 2023-05-24 05:30:02.273531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic/src/utils/frenet.py
--rw-r--r--   0        0        0        0 2023-05-24 05:30:02.273531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic_v/__init__.py
--rw-r--r--   0        0        0     1067 2023-05-24 05:30:02.273531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic_v/src/LICENSE
--rw-r--r--   0        0        0        0 2023-05-24 05:30:02.273531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic_v/src/__init__.py
--rw-r--r--   0        0        0   372723 2023-05-24 05:30:02.273531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic_v/src/frenetic-sbst21-preprint.pdf
--rw-r--r--   0        0        0        0 2023-05-24 05:30:02.273531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/__init__.py
--rw-r--r--   0        0        0     5693 2023-05-24 05:30:02.273531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_frenet_generator.py
--rw-r--r--   0        0        0     5135 2023-05-24 05:30:02.273531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_generator.py
--rw-r--r--   0        0        0    14499 2023-05-24 05:30:02.273531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/random_frenet_generator.py
--rw-r--r--   0        0        0        0 2023-05-24 05:30:02.273531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic_v/src/utils/__init__.py
--rw-r--r--   0        0        0      694 2023-05-24 05:30:02.273531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic_v/src/utils/frenet.py
--rw-r--r--   0        0        0     2762 2023-05-24 05:30:02.273531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_loader.py
--rw-r--r--   0        0        0     6630 2023-05-24 05:30:02.273531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_monitor.py
--rw-r--r--   0        0        0     1843 2023-05-24 05:30:02.273531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_plotter.py
--rw-r--r--   0        0        0     6954 2023-05-24 05:30:02.273531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_runner.py
--rw-r--r--   0        0        0     3150 2023-05-24 05:30:02.273531 sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_validator.py
--rw-r--r--   0        0        0    11963 1970-01-01 00:00:00.000000 sdc_scissor-2.2.0rc1/PKG-INFO
+-rw-r--r--   0        0        0    34916 2023-06-26 07:55:12.158999 sdc_scissor-2.2.0rc3/LICENSE.md
+-rw-r--r--   0        0        0    10961 2023-06-26 07:55:12.158999 sdc_scissor-2.2.0rc3/README.md
+-rw-r--r--   0        0        0     1494 2023-06-26 07:55:12.262998 sdc_scissor-2.2.0rc3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-26 07:55:12.310998 sdc_scissor-2.2.0rc3/sdc_scissor/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:55:12.310998 sdc_scissor-2.2.0rc3/sdc_scissor/can_api/__init__.py
+-rw-r--r--   0        0        0     4671 2023-06-26 07:55:12.310998 sdc_scissor-2.2.0rc3/sdc_scissor/can_api/can_bus_handler.py
+-rw-r--r--   0        0        0     1730 2023-06-26 07:55:12.310998 sdc_scissor-2.2.0rc3/sdc_scissor/can_api/can_msg_generator.py
+-rw-r--r--   0        0        0     3907 2023-06-26 07:55:12.310998 sdc_scissor-2.2.0rc3/sdc_scissor/can_api/can_output.py
+-rw-r--r--   0        0        0    18875 2023-06-26 07:55:12.310998 sdc_scissor-2.2.0rc3/sdc_scissor/cli.py
+-rw-r--r--   0        0        0     1448 2023-06-26 07:55:12.310998 sdc_scissor-2.2.0rc3/sdc_scissor/config.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/feature_extraction_api/__init__.py
+-rw-r--r--   0        0        0     4763 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/feature_extraction_api/angle_based_strategy.py
+-rw-r--r--   0        0        0     3980 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/feature_extraction_api/equi_distance_strategy.py
+-rw-r--r--   0        0        0    10519 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/feature_extraction_api/feature_extraction.py
+-rw-r--r--   0        0        0     2587 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/feature_extraction_api/parameterized_uniform_strategy.py
+-rw-r--r--   0        0        0     3203 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/feature_extraction_api/road_geometry_calculator.py
+-rw-r--r--   0        0        0      401 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/feature_extraction_api/segmentation_strategy.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/machine_learning_api/__init__.py
+-rw-r--r--   0        0        0     9597 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/machine_learning_api/cost_effectiveness_evaluator.py
+-rw-r--r--   0        0        0      255 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/machine_learning_api/csv_loader.py
+-rw-r--r--   0        0        0     7726 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/machine_learning_api/model_evaluator.py
+-rw-r--r--   0        0        0     2382 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/machine_learning_api/predictor.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/obstacle_api/__init__.py
+-rw-r--r--   0        0        0      643 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/obstacle_api/beamng_bump.py
+-rw-r--r--   0        0        0      569 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/obstacle_api/beamng_delineator.py
+-rw-r--r--   0        0        0      764 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/obstacle_api/beamng_obstacle_factory.py
+-rw-r--r--   0        0        0      675 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/obstacle_api/beamng_tree.py
+-rw-r--r--   0        0        0      828 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/obstacle_api/bump.py
+-rw-r--r--   0        0        0      160 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/obstacle_api/carla_bump.py
+-rw-r--r--   0        0        0      190 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/obstacle_api/carla_delineator.py
+-rw-r--r--   0        0        0      753 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/obstacle_api/carla_obstacle_factory.py
+-rw-r--r--   0        0        0      160 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/obstacle_api/carla_tree.py
+-rw-r--r--   0        0        0      664 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/obstacle_api/delineator.py
+-rw-r--r--   0        0        0      522 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/obstacle_api/obstacle_factory.py
+-rw-r--r--   0        0        0      709 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/obstacle_api/tree.py
+-rw-r--r--   0        0        0      966 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/Dockerfile.testPrioritization
+-rw-r--r--   0        0        0       95 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/README.md
+-rw-r--r--   0        0        0        0 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/__init__.py
+-rw-r--r--   0        0        0      510 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/faultDetection.m
+-rw-r--r--   0        0        0     6298 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/faultDetectionRatePlots.m
+-rw-r--r--   0        0        0      463 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/featureSelection.m
+-rw-r--r--   0        0        0      391 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/fitness.m
+-rw-r--r--   0        0        0     1075 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/initialPopulation.m
+-rw-r--r--   0        0        0      574 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/main.m
+-rw-r--r--   0        0        0      609 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/mainGreedy.m
+-rw-r--r--   0        0        0      220 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/objectives.m
+-rw-r--r--   0        0        0      750 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/permutationCrossover.m
+-rw-r--r--   0        0        0     1501 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/permutationMutation.m
+-rw-r--r--   0        0        0      302 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/plotResults.m
+-rw-r--r--   0        0        0     1367 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/python/make-single-csv.py
+-rw-r--r--   0        0        0    10251 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/r-script/analysis.R
+-rw-r--r--   0        0        0     5034 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/r-script/better_rate.pdf
+-rw-r--r--   0        0        0     2128 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/r-script/gavsga.csv
+-rw-r--r--   0        0        0      125 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/r-script/medians_APFDc.csv
+-rw-r--r--   0        0        0     1869 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/r-script/plot.R
+-rw-r--r--   0        0        0     1694 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/r-script/table.R
+-rw-r--r--   0        0        0      395 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/r-script/utils.R
+-rw-r--r--   0        0        0      584 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/r-script/vsbl.csv
+-rw-r--r--   0        0        0      958 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/r-script/vsrand.csv
+-rw-r--r--   0        0        0     1051 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/runGreedy.m
+-rw-r--r--   0        0        0     4258 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/runMOSearch.m
+-rw-r--r--   0        0        0     3480 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/runSearch.m
+-rw-r--r--   0        0        0   239182 2023-06-26 07:55:12.314998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1/BeamNG_RF_1_Complete.csv
+-rw-r--r--   0        0        0  1146691 2023-06-26 07:55:12.326998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_Complete.csv
+-rw-r--r--   0        0        0   440097 2023-06-26 07:55:12.326998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_selected.csv
+-rw-r--r--   0        0        0     1070 2023-06-26 07:55:12.326998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/filter.py
+-rw-r--r--   0        0        0   353423 2023-06-26 07:55:12.330998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_2/BeamNG_RF_2_Complete.csv
+-rw-r--r--   0        0        0      660 2023-06-26 07:55:12.330998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/README.md
+-rw-r--r--   0        0        0  1142098 2023-06-26 07:55:12.330998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/datasets/fullroad/Driver_AI/DriverAI_Complete.csv
+-rw-r--r--   0        0        0     4431 2023-06-26 07:55:12.330998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/datasets/fullroad/README.md
+-rwxr-xr-x   0        0        0      650 2023-06-26 07:55:12.330998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/docker_scripts/build-test-prioritization-image.sh
+-rwxr-xr-x   0        0        0      729 2023-06-26 07:55:12.330998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/docker_scripts/run-test-prioritization-container.sh
+-rw-r--r--   0        0        0       65 2023-06-26 07:55:12.330998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/requirements.txt
+-rw-r--r--   0        0        0      324 2023-06-26 07:55:12.330998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/setup.cfg
+-rw-r--r--   0        0        0       38 2023-06-26 07:55:12.330998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/setup.py
+-rw-r--r--   0        0        0     2413 2023-06-26 07:55:12.330998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/testPrioritization/README.md
+-rw-r--r--   0        0        0        0 2023-06-26 07:55:12.330998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/testPrioritization/__init__.py
+-rw-r--r--   0        0        0      780 2023-06-26 07:55:12.330998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/testPrioritization/crossover/PMX.py
+-rw-r--r--   0        0        0     1306 2023-06-26 07:55:12.330998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/testPrioritization/mutation/HybridMut.py
+-rw-r--r--   0        0        0      843 2023-06-26 07:55:12.330998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/testPrioritization/problem/TestPrioritizationMultiObjectiveProblem.py
+-rw-r--r--   0        0        0     7798 2023-06-26 07:55:12.330998 sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/testPrioritization/run.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:55:12.330998 sdc_scissor-2.2.0rc3/sdc_scissor/simulator_api/__init__.py
+-rw-r--r--   0        0        0     1661 2023-06-26 07:55:12.330998 sdc_scissor-2.2.0rc3/sdc_scissor/simulator_api/abstract_simulator.py
+-rw-r--r--   0        0        0     6672 2023-06-26 07:55:12.330998 sdc_scissor-2.2.0rc3/sdc_scissor/simulator_api/beamng_simulator.py
+-rw-r--r--   0        0        0      807 2023-06-26 07:55:12.330998 sdc_scissor-2.2.0rc3/sdc_scissor/simulator_api/simulator_factory.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:55:12.330998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/__init__.py
+-rw-r--r--   0        0        0      424 2023-06-26 07:55:12.330998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/road_model.py
+-rw-r--r--   0        0        0     2323 2023-06-26 07:55:12.330998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test.py
+-rw-r--r--   0        0        0     5482 2023-06-26 07:55:12.330998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generator.py
+-rw-r--r--   0        0        0    13513 2023-06-26 07:55:12.334998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/car_road.py
+-rw-r--r--   0        0        0      304 2023-06-26 07:55:12.334998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/duplicate_elimination.py
+-rw-r--r--   0        0        0      862 2023-06-26 07:55:12.334998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/generate_test_case_sampling.py
+-rw-r--r--   0        0        0    13276 2023-06-26 07:55:12.334998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/road_gen.py
+-rw-r--r--   0        0        0     2443 2023-06-26 07:55:12.334998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/solution.py
+-rw-r--r--   0        0        0     2580 2023-06-26 07:55:12.334998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_crossover.py
+-rw-r--r--   0        0        0     3786 2023-06-26 07:55:12.334998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_mutation.py
+-rw-r--r--   0        0        0      587 2023-06-26 07:55:12.334998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_problem.py
+-rw-r--r--   0        0        0     8854 2023-06-26 07:55:12.334998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/vehicle.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:55:12.334998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/ambiegen/__init__.py
+-rw-r--r--   0        0        0     2829 2023-06-26 07:55:12.334998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/ambiegen/ambiegen_generator.py
+-rw-r--r--   0        0        0      575 2023-06-26 07:55:12.334998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/ambiegen/config.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:55:12.334998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic/__init__.py
+-rw-r--r--   0        0        0     1067 2023-06-26 07:55:12.334998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic/src/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-26 07:55:12.334998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic/src/__init__.py
+-rw-r--r--   0        0        0   372723 2023-06-26 07:55:12.334998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic/src/frenetic-sbst21-preprint.pdf
+-rw-r--r--   0        0        0        0 2023-06-26 07:55:12.334998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic/src/generators/__init__.py
+-rw-r--r--   0        0        0     2658 2023-06-26 07:55:12.334998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_frenet_generator.py
+-rw-r--r--   0        0        0     4908 2023-06-26 07:55:12.334998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_generator.py
+-rw-r--r--   0        0        0    14117 2023-06-26 07:55:12.334998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic/src/generators/random_frenet_generator.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:55:12.334998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic/src/utils/__init__.py
+-rw-r--r--   0        0        0      731 2023-06-26 07:55:12.334998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic/src/utils/frenet.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:55:12.334998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic_v/__init__.py
+-rw-r--r--   0        0        0     1067 2023-06-26 07:55:12.334998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic_v/src/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-26 07:55:12.334998 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic_v/src/__init__.py
+-rw-r--r--   0        0        0   372723 2023-06-26 07:55:12.338997 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic_v/src/frenetic-sbst21-preprint.pdf
+-rw-r--r--   0        0        0        0 2023-06-26 07:55:12.338997 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/__init__.py
+-rw-r--r--   0        0        0     5693 2023-06-26 07:55:12.338997 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_frenet_generator.py
+-rw-r--r--   0        0        0     5135 2023-06-26 07:55:12.338997 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_generator.py
+-rw-r--r--   0        0        0    14499 2023-06-26 07:55:12.338997 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/random_frenet_generator.py
+-rw-r--r--   0        0        0        0 2023-06-26 07:55:12.338997 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic_v/src/utils/__init__.py
+-rw-r--r--   0        0        0      694 2023-06-26 07:55:12.338997 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic_v/src/utils/frenet.py
+-rw-r--r--   0        0        0     2762 2023-06-26 07:55:12.338997 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_loader.py
+-rw-r--r--   0        0        0     6630 2023-06-26 07:55:12.338997 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_monitor.py
+-rw-r--r--   0        0        0     1843 2023-06-26 07:55:12.338997 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_plotter.py
+-rw-r--r--   0        0        0     6954 2023-06-26 07:55:12.338997 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_runner.py
+-rw-r--r--   0        0        0     3150 2023-06-26 07:55:12.338997 sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_validator.py
+-rw-r--r--   0        0        0    12095 1970-01-01 00:00:00.000000 sdc_scissor-2.2.0rc3/PKG-INFO
```

### Comparing `sdc_scissor-2.2.0rc1/LICENSE.md` & `sdc_scissor-2.2.0rc3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/pyproject.toml` & `sdc_scissor-2.2.0rc3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SDC-Scissor"
-version = "2.2.0-rc.1"
+version = "2.2.0-rc.3"
 description = "A cost-effective test selection for self-driving cars in virtual environments"
 authors = ["Christian Birchler <birchler.chr@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/ChristianBirchler/sdc-scissor"
 documentation = "https://sdc-scissor.readthedocs.io/"
 packages = [
@@ -41,14 +41,15 @@
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = "^4.5.0"
 myst-parser = "^0.18.0"
 sphinx-rtd-theme = "^1.0.0"
 sphinxcontrib-mermaid = "^0.8.1"
 pylint = "^2.16.2"
+sphinxcontrib-youtube = "^1.2.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/can_api/can_bus_handler.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/can_api/can_bus_handler.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/can_api/can_msg_generator.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/can_api/can_msg_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/can_api/can_output.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/can_api/can_output.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/cli.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/cli.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/config.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/config.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/feature_extraction_api/angle_based_strategy.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/feature_extraction_api/angle_based_strategy.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/feature_extraction_api/equi_distance_strategy.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/feature_extraction_api/equi_distance_strategy.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/feature_extraction_api/feature_extraction.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/feature_extraction_api/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/feature_extraction_api/parameterized_uniform_strategy.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/feature_extraction_api/parameterized_uniform_strategy.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/feature_extraction_api/road_geometry_calculator.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/feature_extraction_api/road_geometry_calculator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/machine_learning_api/cost_effectiveness_evaluator.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/machine_learning_api/cost_effectiveness_evaluator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/machine_learning_api/model_evaluator.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/machine_learning_api/model_evaluator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/machine_learning_api/predictor.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/machine_learning_api/predictor.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/obstacle_api/beamng_bump.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/obstacle_api/beamng_bump.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/obstacle_api/beamng_delineator.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/obstacle_api/beamng_delineator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/obstacle_api/beamng_obstacle_factory.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/obstacle_api/beamng_obstacle_factory.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/obstacle_api/beamng_tree.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/obstacle_api/beamng_tree.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/obstacle_api/bump.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/obstacle_api/bump.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/obstacle_api/carla_obstacle_factory.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/obstacle_api/carla_obstacle_factory.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/obstacle_api/delineator.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/obstacle_api/delineator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/obstacle_api/obstacle_factory.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/obstacle_api/obstacle_factory.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/obstacle_api/tree.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/obstacle_api/tree.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/Dockerfile.testPrioritization` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/Dockerfile.testPrioritization`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/faultDetectionRatePlots.m` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/faultDetectionRatePlots.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/initialPopulation.m` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/initialPopulation.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/main.m` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/main.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/mainGreedy.m` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/mainGreedy.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/permutationCrossover.m` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/permutationCrossover.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/permutationMutation.m` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/permutationMutation.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/python/make-single-csv.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/python/make-single-csv.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/r-script/analysis.R` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/r-script/analysis.R`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/r-script/better_rate.pdf` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/r-script/better_rate.pdf`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/r-script/gavsga.csv` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/r-script/gavsga.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/r-script/plot.R` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/r-script/plot.R`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/r-script/table.R` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/r-script/table.R`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/r-script/vsbl.csv` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/r-script/vsbl.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/r-script/vsrand.csv` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/r-script/vsrand.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/runGreedy.m` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/runGreedy.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/runMOSearch.m` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/runMOSearch.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/code/runSearch.m` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/code/runSearch.m`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1/BeamNG_RF_1_Complete.csv` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1/BeamNG_RF_1_Complete.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_Complete.csv` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_Complete.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_selected.csv` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/BeamNG_RF_1_5_selected.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/filter.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_1_5/filter.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_2/BeamNG_RF_2_Complete.csv` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/BeamNG_RF_2/BeamNG_RF_2_Complete.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/README.md` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/datasets/fullroad/BeamNG_AI/README.md`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/datasets/fullroad/Driver_AI/DriverAI_Complete.csv` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/datasets/fullroad/Driver_AI/DriverAI_Complete.csv`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/datasets/fullroad/README.md` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/datasets/fullroad/README.md`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/docker_scripts/build-test-prioritization-image.sh` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/docker_scripts/build-test-prioritization-image.sh`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/docker_scripts/run-test-prioritization-container.sh` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/docker_scripts/run-test-prioritization-container.sh`

 * *Files 0% similar despite different names*

```diff
@@ -7,12 +7,12 @@
 fi
 
 
 # Run a new docker container.
 docker run -dit --name test-prioritization-container \
 --mount type=bind,source="$(pwd)/data",target=/home/user/experiment/data \
 --mount type=bind,source="$(pwd)/testPrioritization",target=/home/user/experiment/testPrioritization \
-test-prioritization-image
+test-prioritization-image bash
 
 
 
- docker exec -it test-prioritization-container bash -c "pip install --editable /home/user/experiment"
+docker exec -it test-prioritization-container bash -c "pip install --editable /home/user/experiment"
```

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/testPrioritization/README.md` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/testPrioritization/README.md`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/testPrioritization/crossover/PMX.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/testPrioritization/crossover/PMX.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/testPrioritization/mutation/HybridMut.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/testPrioritization/mutation/HybridMut.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/testPrioritization/problem/TestPrioritizationMultiObjectiveProblem.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/testPrioritization/problem/TestPrioritizationMultiObjectiveProblem.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/sdc_prioritizer/testPrioritization/run.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/sdc_prioritizer/testPrioritization/run.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/simulator_api/abstract_simulator.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/simulator_api/abstract_simulator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/simulator_api/beamng_simulator.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/simulator_api/beamng_simulator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/simulator_api/simulator_factory.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/simulator_api/simulator_factory.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generator.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/ambiegen/Utils/car_road.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/car_road.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/ambiegen/Utils/generate_test_case_sampling.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/generate_test_case_sampling.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/ambiegen/Utils/road_gen.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/road_gen.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/ambiegen/Utils/solution.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/solution.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_crossover.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_crossover.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_mutation.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_mutation.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_problem.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/test_case_problem.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/ambiegen/Utils/vehicle.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/ambiegen/Utils/vehicle.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/ambiegen/ambiegen_generator.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/ambiegen/ambiegen_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/ambiegen/config.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/ambiegen/config.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic/src/LICENSE` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic/src/LICENSE`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic/src/frenetic-sbst21-preprint.pdf` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic/src/frenetic-sbst21-preprint.pdf`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_frenet_generator.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_frenet_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_generator.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic/src/generators/base_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic/src/generators/random_frenet_generator.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic/src/generators/random_frenet_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic/src/utils/frenet.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic/src/utils/frenet.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic_v/src/LICENSE` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic_v/src/LICENSE`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic_v/src/frenetic-sbst21-preprint.pdf` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic_v/src/frenetic-sbst21-preprint.pdf`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_frenet_generator.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_frenet_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_generator.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/base_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/random_frenet_generator.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic_v/src/generators/random_frenet_generator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_generators/frenetic_v/src/utils/frenet.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_generators/frenetic_v/src/utils/frenet.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_loader.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_loader.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_monitor.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_monitor.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_plotter.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_plotter.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_runner.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_runner.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/sdc_scissor/testing_api/test_validator.py` & `sdc_scissor-2.2.0rc3/sdc_scissor/testing_api/test_validator.py`

 * *Files identical despite different names*

### Comparing `sdc_scissor-2.2.0rc1/PKG-INFO` & `sdc_scissor-2.2.0rc3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,96 +1,69 @@
-Metadata-Version: 2.1
-Name: sdc-scissor
-Version: 2.2.0rc1
-Summary: A cost-effective test selection for self-driving cars in virtual environments
-Home-page: https://github.com/ChristianBirchler/sdc-scissor
-License: GPL-3.0-or-later
-Author: Christian Birchler
-Author-email: birchler.chr@gmail.com
-Requires-Python: >=3.10,<3.11
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: Shapely (>=1.8.1,<2.0.0)
-Requires-Dist: beamngpy (==1.22)
-Requires-Dist: cantools (>=38.0.1,<39.0.0)
-Requires-Dist: click (>=8.0.4,<9.0.0)
-Requires-Dist: icontract (>=2.6.2,<3.0.0)
-Requires-Dist: influxdb-client (>=1.36.1,<2.0.0)
-Requires-Dist: pandas (>=1.4.1,<2.0.0)
-Requires-Dist: pymoo (==0.4.2.2)
-Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: scikit-learn (>=1.0.2,<2.0.0)
-Project-URL: Documentation, https://sdc-scissor.readthedocs.io/
-Project-URL: Repository, https://github.com/ChristianBirchler/sdc-scissor
-Description-Content-Type: text/markdown
-
 # SDC-Scissor
 ```{code-block} text
  ____    ____    ____              ____
 /\  _`\ /\  _`\ /\  _`\           /\  _`\           __
 \ \,\L\_\ \ \/\ \ \ \/\_\         \ \,\L\_\    ___ /\_\    ____    ____    ___   _ __
  \/_\__ \\ \ \ \ \ \ \/_/_  _______\/_\__ \   /'___\/\ \  /',__\  /',__\  / __`\/\`'__\
    /\ \L\ \ \ \_\ \ \ \L\ \/\______\ /\ \L\ \/\ \__/\ \ \/\__, `\/\__, `\/\ \L\ \ \ \/
    \ `\____\ \____/\ \____/\/______/ \ `\____\ \____\\ \_\/\____/\/\____/\ \____/\ \_\
     \/_____/\/___/  \/___/            \/_____/\/____/ \/_/\/___/  \/___/  \/___/  \/_/
 
 
 ```
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white)](https://conventionalcommits.org)
-[![GitHub issues](https://img.shields.io/github/issues/ChristianBirchler/sdc-scissor)](https://github.com/ChristianBirchler/sdc-scissor/issues)
-[![GitHub forks](https://img.shields.io/github/forks/ChristianBirchler/sdc-scissor)](https://github.com/ChristianBirchler/sdc-scissor/network)
-[![GitHub stars](https://img.shields.io/github/stars/ChristianBirchler/sdc-scissor)](https://github.com/ChristianBirchler/sdc-scissor/stargazers)
-[![](https://github.com/ChristianBirchler/sdc-scissor/actions/workflows/ci.yml/badge.svg)](https://github.com/ChristianBirchler/sdc-scissor/actions/workflows/ci.yml)
-[![CD](https://github.com/ChristianBirchler/sdc-scissor/actions/workflows/cd.yml/badge.svg)](https://github.com/ChristianBirchler/sdc-scissor/actions/workflows/cd.yml)
+[![GitHub issues](https://img.shields.io/github/issues/ChristianBirchler/sdc-scissor)](https://github.com/christianbirchler-org/sdc-scissor/issues)
+[![GitHub forks](https://img.shields.io/github/forks/ChristianBirchler/sdc-scissor)](https://github.com/christianbirchler-org/sdc-scissor/network)
+[![GitHub stars](https://img.shields.io/github/stars/ChristianBirchler/sdc-scissor)](https://github.com/christianbirchler-org/sdc-scissor/stargazers)
+[![](https://github.com/ChristianBirchler/sdc-scissor/actions/workflows/ci.yml/badge.svg)](https://github.com/christianbirchler-org/sdc-scissor/actions/workflows/ci.yml)
+[![CD](https://github.com/ChristianBirchler/sdc-scissor/actions/workflows/cd.yml/badge.svg)](https://github.com/christianbirchler-org/sdc-scissor/actions/workflows/cd.yml)
 [![PyPI](https://img.shields.io/pypi/v/sdc-scissor)](https://pypi.org/project/sdc-scissor/)
 [![](https://readthedocs.org/projects/sdc-scissor/badge)](https://sdc-scissor.readthedocs.io)
 [![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://black.readthedocs.io/)
-[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=alert_status)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)
-[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=ncloc)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)
-[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=coverage)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)
-[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=sqale_index)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)
-[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=reliability_rating)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)
-[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=duplicated_lines_density)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)
-[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=vulnerabilities)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)
-[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=bugs)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)
-[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=security_rating)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)
-[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=sqale_rating)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)
-[![](https://sonarcloud.io/api/project_badges/measure?project=ChristianBirchler_sdc-scissor&metric=code_smells)](https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor)
+[![](https://sonarcloud.io/api/project_badges/measure?project=christianbirchler-org_sdc-scissor&metric=alert_status)](https://sonarcloud.io/summary/overall?id=christianbirchler-org_sdc-scissor)
+[![](https://sonarcloud.io/api/project_badges/measure?project=christianbirchler-org_sdc-scissor&metric=ncloc)](https://sonarcloud.io/summary/overall?id=christianbirchler-org_sdc-scissor)
+[![](https://sonarcloud.io/api/project_badges/measure?project=christianbirchler-org_sdc-scissor&metric=coverage)](https://sonarcloud.io/summary/overall?id=christianbirchler-org_sdc-scissor)
+[![](https://sonarcloud.io/api/project_badges/measure?project=christianbirchler-org_sdc-scissor&metric=sqale_index)](https://sonarcloud.io/summary/overall?id=christianbirchler-org_sdc-scissor)
+[![](https://sonarcloud.io/api/project_badges/measure?project=christianbirchler-org_sdc-scissor&metric=reliability_rating)](https://sonarcloud.io/summary/overall?id=christianbirchler-org_sdc-scissor)
+[![](https://sonarcloud.io/api/project_badges/measure?project=christianbirchler-org_sdc-scissor&metric=duplicated_lines_density)](https://sonarcloud.io/summary/overall?id=christianbirchler-org_sdc-scissor)
+[![](https://sonarcloud.io/api/project_badges/measure?project=christianbirchler-org_sdc-scissor&metric=vulnerabilities)](https://sonarcloud.io/summary/overall?id=christianbirchler-org_sdc-scissor)
+[![](https://sonarcloud.io/api/project_badges/measure?project=christianbirchler-org_sdc-scissor&metric=bugs)](https://sonarcloud.io/summary/overall?id=christianbirchler-org_sdc-scissor)
+[![](https://sonarcloud.io/api/project_badges/measure?project=christianbirchler-org_sdc-scissor&metric=security_rating)](https://sonarcloud.io/summary/overall?id=christianbirchler-org_sdc-scissor)
+[![](https://sonarcloud.io/api/project_badges/measure?project=christianbirchler-org_sdc-scissor&metric=sqale_rating)](https://sonarcloud.io/summary/overall?id=christianbirchler-org_sdc-scissor)
+[![](https://sonarcloud.io/api/project_badges/measure?project=christianbirchler-org_sdc-scissor&metric=code_smells)](https://sonarcloud.io/summary/overall?id=christianbirchler-org_sdc-scissor)
 [![DOI](https://zenodo.org/badge/363107094.svg)](https://zenodo.org/badge/latestdoi/363107094)
 <div style="text-align: center;">
-<a href="https://github.com/ChristianBirchler/sdc-scissor">
-<img src="https://raw.githubusercontent.com/ChristianBirchler/sdc-scissor/main/docs/images/github_logo_icon.png">
+<a href="https://github.com/christianbirchler-org/sdc-scissor">
+<img src="https://raw.githubusercontent.com/christianbirchler-org/sdc-scissor/main/docs/images/github_logo_icon.png">
 </a>
-<a href="https://sonarcloud.io/summary/overall?id=ChristianBirchler_sdc-scissor">
+<a href="https://sonarcloud.io/summary/overall?id=christianbirchler-org_sdc-scissor">
 <img src="https://sonarcloud.io/images/project_badges/sonarcloud-black.svg">
 </a>
 </div>
 
 ## A Tool for Cost-effective Simulation-based Test Selection in Self-driving Cars Software
 SDC-Scissor is a tool that let you test self-driving cars more efficiently in simulation. It uses a machine-learning
 approach to select only relevant test scenarios so that the testing process is faster. Furthermore, the selected tests
 are diverse and try to challenge the car with corner cases.
 
 Furthermore, this repository contains also code for test multi-objective test case prioritization with an evolutionary
 genetic search algorithm. If you are interested in prioritizing test cases, then you should read the dedicated
-[README.md](https://github.com/ChristianBirchler/sdc-scissor/blob/main/sdc_scissor/sdc_prioritizer/testPrioritization/README.md)
+[README.md](https://github.com/christianbirchler-org/sdc-scissor/blob/main/sdc_scissor/sdc_prioritizer/testPrioritization/README.md)
 for this. If you use the prioritization technique then also cite the papers from the reference section!
 
 ## Support
-We use [GitHub Discussions](https://github.com/ChristianBirchler/sdc-scissor/discussions) as a community platform. You
+We use [GitHub Discussions](https://github.com/christianbirchler-org/sdc-scissor/discussions) as a community platform. You
 can ask questions and get support there from the community. Furthermore, new features and releases will be discussed and
 announced there.
 
 ## Documentation
 For the documentation follow the link: [sdc-scissor.readthedocs.io](https://sdc-scissor.readthedocs.io/en/latest/)
 
-[![](https://raw.githubusercontent.com/ChristianBirchler/sdc-scissor/main/docs/images/readthedocs.png)](https://sdc-scissor.readthedocs.io/en/latest/)
+[![](https://raw.githubusercontent.com/christianbirchler-org/sdc-scissor/main/docs/images/readthedocs.png)](https://sdc-scissor.readthedocs.io/en/latest/)
 
 ## License
 ```{code-block} text
 SDC-Scissor tool for cost-effective simulation-based test selection
 in self-driving cars software.
 Copyright (C) 2022  Christian Birchler
 
@@ -176,8 +149,7 @@
     * Zurich University of Applied Sciences (ZHAW), Switzerland - gann@zhaw.ch
 * Sajad Khatiri
     * Zurich University of Applied Sciences (ZHAW), Switzerland - mazr@zhaw.ch
 * Dr. Alessio Gambi
     * IMC University Of Applied Sciences Krems, Austria - alessio.gambi@fh-krems.ac.at
 * Dr. Sebastiano Panichella
     * Zurich University of Applied Sciences (ZHAW), Switzerland - panc@zhaw.ch
-
```


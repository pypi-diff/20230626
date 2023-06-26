# Comparing `tmp/commonroad_io-2023.1.tar.gz` & `tmp/commonroad_io-2023.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonroad_io-2023.1.tar", max compression
+gzip compressed data, was "commonroad_io-2023.2.tar", max compression
```

## Comparing `commonroad_io-2023.1.tar` & `commonroad_io-2023.2.tar`

### file list

```diff
@@ -1,640 +1,643 @@
--rw-r--r--   0        0        0     1554 2023-02-01 09:07:46.236367 commonroad_io-2023.1/LICENSE.txt
--rw-r--r--   0        0        0     7698 2023-03-05 16:45:57.221377 commonroad_io-2023.1/README.md
--rw-r--r--   0        0        0      218 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/__init__.py
--rw-r--r--   0        0        0        0 2023-02-01 09:07:46.236367 commonroad_io-2023.1/commonroad/common/__init__.py
--rw-r--r--   0        0        0     1743 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/common/file_reader.py
--rw-r--r--   0        0        0     3809 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/common/file_writer.py
--rw-r--r--   0        0        0        0 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/common/reader/__init__.py
--rw-r--r--   0        0        0      630 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/common/reader/file_reader_interface.py
--rw-r--r--   0        0        0    41811 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/common/reader/file_reader_protobuf.py
--rw-r--r--   0        0        0    73782 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/common/reader/file_reader_xml.py
--rw-r--r--   0        0        0    35068 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/common/solution.py
--rw-r--r--   0        0        0     8508 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/common/util.py
--rw-r--r--   0        0        0    10617 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/common/validity.py
--rw-r--r--   0        0        0        0 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/common/writer/__init__.py
--rw-r--r--   0        0        0     4716 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/common/writer/file_writer_interface.py
--rw-r--r--   0        0        0    38519 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/common/writer/file_writer_protobuf.py
--rw-r--r--   0        0        0    51502 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/common/writer/file_writer_xml.py
--rw-r--r--   0        0        0        0 2023-02-01 09:07:46.236367 commonroad_io-2023.1/commonroad/geometry/__init__.py
--rw-r--r--   0        0        0    15029 2023-02-01 09:07:46.236367 commonroad_io-2023.1/commonroad/geometry/polyline_util.py
--rw-r--r--   0        0        0    28507 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/geometry/shape.py
--rw-r--r--   0        0        0     3870 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/geometry/transform.py
--rw-r--r--   0        0        0        0 2023-02-01 09:07:46.236367 commonroad_io-2023.1/commonroad/planning/__init__.py
--rw-r--r--   0        0        0    10244 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/planning/goal.py
--rw-r--r--   0        0        0     8567 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/planning/planning_problem.py
--rw-r--r--   0        0        0        0 2023-02-01 09:07:46.240367 commonroad_io-2023.1/commonroad/prediction/__init__.py
--rw-r--r--   0        0        0    17002 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/prediction/prediction.py
--rw-r--r--   0        0        0        0 2023-02-01 09:07:46.240367 commonroad_io-2023.1/commonroad/scenario/__init__.py
--rw-r--r--   0        0        0    10399 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario/intersection.py
--rw-r--r--   0        0        0    76454 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario/lanelet.py
--rw-r--r--   0        0        0    36682 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario/obstacle.py
--rw-r--r--   0        0        0    55471 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario/scenario.py
--rw-r--r--   0        0        0    18723 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario/state.py
--rw-r--r--   0        0        0    41285 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario/traffic_sign.py
--rw-r--r--   0        0        0     3982 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario/traffic_sign_interpreter.py
--rw-r--r--   0        0        0    12767 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario/trajectory.py
--rw-r--r--   0        0        0        0 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario_definition/__init__.py
--rw-r--r--   0        0        0        0 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/__init__.py
--rw-r--r--   0        0        0     4718 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/convert_xml_to_pb.py
--rw-r--r--   0        0        0     1280 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/definition_files/commonroad.proto
--rw-r--r--   0        0        0      523 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/definition_files/dynamic_obstacle.proto
--rw-r--r--   0        0        0      269 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/definition_files/environment_obstacle.proto
--rw-r--r--   0        0        0      452 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/definition_files/intersection.proto
--rw-r--r--   0        0        0     2134 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/definition_files/lanelet.proto
--rw-r--r--   0        0        0     1217 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/definition_files/location.proto
--rw-r--r--   0        0        0     3442 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/definition_files/obstacle.proto
--rw-r--r--   0        0        0      179 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/definition_files/phantom_obstacle.proto
--rw-r--r--   0        0        0      318 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/definition_files/planning_problem.proto
--rw-r--r--   0        0        0      844 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/definition_files/scenario_tags.proto
--rw-r--r--   0        0        0      383 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/definition_files/static_obstacle.proto
--rw-r--r--   0        0        0      880 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/definition_files/traffic_light.proto
--rw-r--r--   0        0        0    22979 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/definition_files/traffic_sign.proto
--rw-r--r--   0        0        0     1353 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/definition_files/util.proto
--rw-r--r--   0        0        0        0 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/__init__.py
--rw-r--r--   0        0        0    15076 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/commonroad_pb2.py
--rw-r--r--   0        0        0     7351 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/dynamic_obstacle_pb2.py
--rw-r--r--   0        0        0     3688 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/environment_obstacle_pb2.py
--rw-r--r--   0        0        0     6602 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/intersection_pb2.py
--rw-r--r--   0        0        0    27162 2023-03-05 16:45:57.225377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/lanelet_pb2.py
--rw-r--r--   0        0        0    17811 2023-03-05 16:45:57.229377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/location_pb2.py
--rw-r--r--   0        0        0    43107 2023-03-05 16:45:57.229377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/obstacle_pb2.py
--rw-r--r--   0        0        0     2824 2023-03-05 16:45:57.229377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/phantom_obstacle_pb2.py
--rw-r--r--   0        0        0     5197 2023-03-05 16:45:57.229377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/planning_problem_pb2.py
--rw-r--r--   0        0        0     9253 2023-03-05 16:45:57.229377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/scenario_tags_pb2.py
--rw-r--r--   0        0        0     5311 2023-03-05 16:45:57.229377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/static_obstacle_pb2.py
--rw-r--r--   0        0        0    12268 2023-03-05 16:45:57.229377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/traffic_light_pb2.py
--rw-r--r--   0        0        0   169832 2023-03-05 16:45:57.229377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/traffic_sign_pb2.py
--rw-r--r--   0        0        0    27145 2023-03-05 16:45:57.229377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/util_pb2.py
--rw-r--r--   0        0        0     1120 2023-03-05 16:45:57.229377 commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/how_to_protobuf.md
--rw-r--r--   0        0        0     7849 2023-03-05 16:45:57.229377 commonroad_io-2023.1/commonroad/scenario_definition/xml_definition_files/CommonRoadSolution_schema.xsd
--rw-r--r--   0        0        0    42394 2023-03-05 16:45:57.229377 commonroad_io-2023.1/commonroad/scenario_definition/xml_definition_files/XML_commonRoad_XSD.xsd
--rw-r--r--   0        0        0        0 2023-02-01 09:07:46.244367 commonroad_io-2023.1/commonroad/visualization/__init__.py
--rw-r--r--   0        0        0    14598 2023-03-05 16:45:57.229377 commonroad_io-2023.1/commonroad/visualization/draw_params.py
--rw-r--r--   0        0        0      598 2023-03-05 16:45:57.229377 commonroad_io-2023.1/commonroad/visualization/drawable.py
--rw-r--r--   0        0        0    12857 2023-03-05 16:45:57.229377 commonroad_io-2023.1/commonroad/visualization/icons.py
--rw-r--r--   0        0        0    65902 2023-03-05 16:45:57.229377 commonroad_io-2023.1/commonroad/visualization/mp_renderer.py
--rw-r--r--   0        0        0     6115 2023-03-05 16:45:57.229377 commonroad_io-2023.1/commonroad/visualization/renderer.py
--rw-r--r--   0        0        0    21494 2023-03-05 16:45:57.229377 commonroad_io-2023.1/commonroad/visualization/traffic_sign.py
--rw-r--r--   0        0        0     3377 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDChina/.png
--rw-r--r--   0        0        0     3377 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/.png
--rw-r--r--   0        0        0     3513 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000-10.png
--rw-r--r--   0        0        0     4708 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000-11.png
--rw-r--r--   0        0        0     3627 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000-20.png
--rw-r--r--   0        0        0     4340 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000-21.png
--rw-r--r--   0        0        0     4898 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000-30.png
--rw-r--r--   0        0        0     4788 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000-31.png
--rw-r--r--   0        0        0     1312 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000.png
--rw-r--r--   0        0        0     4181 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1001-30.png
--rw-r--r--   0        0        0     4687 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1001-31.png
--rw-r--r--   0        0        0     3091 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-10.png
--rw-r--r--   0        0        0     2965 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-11.png
--rw-r--r--   0        0        0     3006 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-12.png
--rw-r--r--   0        0        0     3044 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-13.png
--rw-r--r--   0        0        0     2957 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-14.png
--rw-r--r--   0        0        0     2937 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-20.png
--rw-r--r--   0        0        0     3005 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-21.png
--rw-r--r--   0        0        0     2873 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-22.png
--rw-r--r--   0        0        0     2872 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-23.png
--rw-r--r--   0        0        0     2944 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-24.png
--rw-r--r--   0        0        0     3147 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1004-30.png
--rw-r--r--   0        0        0     3678 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1004-31.png
--rw-r--r--   0        0        0     4872 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1004-32.png
--rw-r--r--   0        0        0     2960 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1004-33.png
--rw-r--r--   0        0        0     2939 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1004-34.png
--rw-r--r--   0        0        0     2385 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1004-35.png
--rw-r--r--   0        0        0     2985 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-30.png
--rw-r--r--   0        0        0     2792 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-31.png
--rw-r--r--   0        0        0     3037 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-32.png
--rw-r--r--   0        0        0     4135 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-33.png
--rw-r--r--   0        0        0     4419 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-34.png
--rw-r--r--   0        0        0     4321 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-35.png
--rw-r--r--   0        0        0     4095 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-36.png
--rw-r--r--   0        0        0     3849 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-37.png
--rw-r--r--   0        0        0     2317 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-38.png
--rw-r--r--   0        0        0     3612 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-39.png
--rw-r--r--   0        0        0     2188 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1007-31.png
--rw-r--r--   0        0        0     6916 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/101.png
--rw-r--r--   0        0        0     2147 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1010-10.png
--rw-r--r--   0        0        0     2873 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1010-11.png
--rw-r--r--   0        0        0     1827 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1010-12.png
--rw-r--r--   0        0        0     2819 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1010-13.png
--rw-r--r--   0        0        0     3029 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1010-14.png
--rw-r--r--   0        0        0     1704 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-30.png
--rw-r--r--   0        0        0     1418 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-31.png
--rw-r--r--   0        0        0     3480 2023-02-01 09:07:46.248367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-32.png
--rw-r--r--   0        0        0     2572 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-33.png
--rw-r--r--   0        0        0     3343 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-34.png
--rw-r--r--   0        0        0     2933 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-35.png
--rw-r--r--   0        0        0     2066 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-36.png
--rw-r--r--   0        0        0     3120 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-37.png
--rw-r--r--   0        0        0     2050 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-38.png
--rw-r--r--   0        0        0     2112 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-50.png
--rw-r--r--   0        0        0     2485 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-51.png
--rw-r--r--   0        0        0     2339 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-52.png
--rw-r--r--   0        0        0     2516 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-53.png
--rw-r--r--   0        0        0     6735 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/102.png
--rw-r--r--   0        0        0     5597 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1020-30.png
--rw-r--r--   0        0        0     6417 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1022-10.png
--rw-r--r--   0        0        0     5950 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1024-10.png
--rw-r--r--   0        0        0     8026 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1026-36.png
--rw-r--r--   0        0        0     8026 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1026-37.png
--rw-r--r--   0        0        0     8026 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1026-38.png
--rw-r--r--   0        0        0     8666 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/103-10.png
--rw-r--r--   0        0        0     7320 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/103-20.png
--rw-r--r--   0        0        0     4042 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1031-52.png
--rw-r--r--   0        0        0     2650 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1040-30.png
--rw-r--r--   0        0        0     3159 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1048-12.png
--rw-r--r--   0        0        0     5224 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1049-13.png
--rw-r--r--   0        0        0     3680 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1052-31.png
--rw-r--r--   0        0        0     4316 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1053-33.png
--rw-r--r--   0        0        0     2901 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1053-34.png
--rw-r--r--   0        0        0     3762 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1053-35.png
--rw-r--r--   0        0        0    12644 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/108.png
--rw-r--r--   0        0        0     8398 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/114.png
--rw-r--r--   0        0        0     5977 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/120.png
--rw-r--r--   0        0        0    13791 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/123.png
--rw-r--r--   0        0        0     9003 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/124.png
--rw-r--r--   0        0        0     8510 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/125.png
--rw-r--r--   0        0        0     6937 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/131.png
--rw-r--r--   0        0        0     9228 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/133-10.png
--rw-r--r--   0        0        0     9320 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/133-20.png
--rw-r--r--   0        0        0     8610 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/138.png
--rw-r--r--   0        0        0    11307 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/142-10.png
--rw-r--r--   0        0        0     6381 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/145-50.png
--rw-r--r--   0        0        0    12735 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/201.png
--rw-r--r--   0        0        0     5582 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/205.png
--rw-r--r--   0        0        0     5067 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/206.png
--rw-r--r--   0        0        0    13812 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/208.png
--rw-r--r--   0        0        0     7132 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/209-10.png
--rw-r--r--   0        0        0    11978 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/209-20.png
--rw-r--r--   0        0        0     6924 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/209-30.png
--rw-r--r--   0        0        0     7083 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/209.png
--rw-r--r--   0        0        0     6937 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/211-10.png
--rw-r--r--   0        0        0     6249 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/211-20.png
--rw-r--r--   0        0        0     6920 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/211.png
--rw-r--r--   0        0        0    16931 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/2113.png
--rw-r--r--   0        0        0     7799 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/214-10.png
--rw-r--r--   0        0        0     7333 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/214-30.png
--rw-r--r--   0        0        0     7769 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/214.png
--rw-r--r--   0        0        0    11470 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/215.png
--rw-r--r--   0        0        0     5287 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/220-10.png
--rw-r--r--   0        0        0     5359 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/220-20.png
--rw-r--r--   0        0        0     8269 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/222-10.png
--rw-r--r--   0        0        0     8297 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/222-20.png
--rw-r--r--   0        0        0     4342 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/223.2-50.png
--rw-r--r--   0        0        0     5405 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/223.2-51.png
--rw-r--r--   0        0        0     4747 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/223.2.png
--rw-r--r--   0        0        0     6167 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/224-50.png
--rw-r--r--   0        0        0    17675 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/237.png
--rw-r--r--   0        0        0    15792 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/239.png
--rw-r--r--   0        0        0    15236 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/240.png
--rw-r--r--   0        0        0    11564 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/242.1.png
--rw-r--r--   0        0        0    10015 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/242.2.png
--rw-r--r--   0        0        0    13431 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/244.1.png
--rw-r--r--   0        0        0    10786 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/244.2.png
--rw-r--r--   0        0        0    14243 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/245.png
--rw-r--r--   0        0        0    12752 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/250.png
--rw-r--r--   0        0        0     8903 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/251.png
--rw-r--r--   0        0        0    14665 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/253.png
--rw-r--r--   0        0        0    10381 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/254.png
--rw-r--r--   0        0        0    16226 2023-02-01 09:07:46.252367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/255.png
--rw-r--r--   0        0        0    15152 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/257-54.png
--rw-r--r--   0        0        0     9437 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/259.png
--rw-r--r--   0        0        0    18193 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/260.png
--rw-r--r--   0        0        0    14767 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/261.png
--rw-r--r--   0        0        0    13173 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/262.png
--rw-r--r--   0        0        0    13739 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/264.png
--rw-r--r--   0        0        0    13764 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/265.png
--rw-r--r--   0        0        0    15436 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/266.png
--rw-r--r--   0        0        0     6366 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/267.png
--rw-r--r--   0        0        0     6424 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/270.1.png
--rw-r--r--   0        0        0     6871 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/270.2.png
--rw-r--r--   0        0        0    10406 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/272.png
--rw-r--r--   0        0        0     4996 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/274.1.png
--rw-r--r--   0        0        0     7607 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/274.2.png
--rw-r--r--   0        0        0     7804 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/274.png
--rw-r--r--   0        0        0     6449 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/275.png
--rw-r--r--   0        0        0     8759 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/276.png
--rw-r--r--   0        0        0     9330 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/277.png
--rw-r--r--   0        0        0     6601 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/278.png
--rw-r--r--   0        0        0     6835 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/279.png
--rw-r--r--   0        0        0     8452 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/280.png
--rw-r--r--   0        0        0     8087 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/281.png
--rw-r--r--   0        0        0     6469 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/282.png
--rw-r--r--   0        0        0    11770 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/283-10.png
--rw-r--r--   0        0        0    12188 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/283-30.png
--rw-r--r--   0        0        0    12156 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/286-30.png
--rw-r--r--   0        0        0     8130 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/286.png
--rw-r--r--   0        0        0     5908 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/301.png
--rw-r--r--   0        0        0     3956 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/306.png
--rw-r--r--   0        0        0     5671 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/308.png
--rw-r--r--   0        0        0     5401 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/310.png
--rw-r--r--   0        0        0     7203 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/311.png
--rw-r--r--   0        0        0     2529 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/314-10.png
--rw-r--r--   0        0        0     2569 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/314-20.png
--rw-r--r--   0        0        0     2705 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/314-30.png
--rw-r--r--   0        0        0     2317 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/314.png
--rw-r--r--   0        0        0    10625 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/325.1.png
--rw-r--r--   0        0        0    12383 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/325.2.png
--rw-r--r--   0        0        0     5815 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/327.png
--rw-r--r--   0        0        0     2544 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/328.png
--rw-r--r--   0        0        0     2225 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/330.1.png
--rw-r--r--   0        0        0     8637 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/330.2.png
--rw-r--r--   0        0        0     3567 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/331.1.png
--rw-r--r--   0        0        0     4310 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/331.2.png
--rw-r--r--   0        0        0     3983 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/332.1.png
--rw-r--r--   0        0        0     7257 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/332.png
--rw-r--r--   0        0        0     4616 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/333-20.png
--rw-r--r--   0        0        0     3350 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/333-21.png
--rw-r--r--   0        0        0     2663 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/333-22.png
--rw-r--r--   0        0        0     4496 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/333.png
--rw-r--r--   0        0        0     5223 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/350.png
--rw-r--r--   0        0        0     8456 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/354.png
--rw-r--r--   0        0        0     5080 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/356.png
--rw-r--r--   0        0        0     3049 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/357.png
--rw-r--r--   0        0        0     1854 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/363.png
--rw-r--r--   0        0        0     5740 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/365-51.png
--rw-r--r--   0        0        0     3878 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/365-52.png
--rw-r--r--   0        0        0     3515 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/365-60.png
--rw-r--r--   0        0        0     1124 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/380.png
--rw-r--r--   0        0        0     1588 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/381.png
--rw-r--r--   0        0        0     2438 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/386.1.png
--rw-r--r--   0        0        0     4572 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/386.2.png
--rw-r--r--   0        0        0     4247 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/386.3.png
--rw-r--r--   0        0        0    11292 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/406-50.png
--rw-r--r--   0        0        0     2691 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/418-20.png
--rw-r--r--   0        0        0     1852 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/419-20.png
--rw-r--r--   0        0        0     2638 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/430-20.png
--rw-r--r--   0        0        0     1709 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/432-10.png
--rw-r--r--   0        0        0     2271 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/432-20.png
--rw-r--r--   0        0        0     6106 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/434-50.png
--rw-r--r--   0        0        0     8563 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/434.png
--rw-r--r--   0        0        0     3168 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/438.png
--rw-r--r--   0        0        0     3361 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/439.png
--rw-r--r--   0        0        0     5870 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/440.png
--rw-r--r--   0        0        0     7617 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/448.png
--rw-r--r--   0        0        0     9309 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/449.png
--rw-r--r--   0        0        0     3520 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/450-50.png
--rw-r--r--   0        0        0     4770 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/450-51.png
--rw-r--r--   0        0        0     5217 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/450-52.png
--rw-r--r--   0        0        0     4938 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/450-53.png
--rw-r--r--   0        0        0     6058 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/450-54.png
--rw-r--r--   0        0        0     6767 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/450-55.png
--rw-r--r--   0        0        0     6353 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/453.png
--rw-r--r--   0        0        0     2018 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/455.1-30.png
--rw-r--r--   0        0        0     5836 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/458.png
--rw-r--r--   0        0        0     3959 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/460-10.png
--rw-r--r--   0        0        0     3966 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/460-12.png
--rw-r--r--   0        0        0     1865 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/460-20.png
--rw-r--r--   0        0        0     1728 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/460-21.png
--rw-r--r--   0        0        0     1815 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/460-22.png
--rw-r--r--   0        0        0     1775 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/460-30.png
--rw-r--r--   0        0        0     3619 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/501-15.png
--rw-r--r--   0        0        0     2458 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/501-16.png
--rw-r--r--   0        0        0    45510 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/511-22.png
--rw-r--r--   0        0        0     1985 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/521-30.png
--rw-r--r--   0        0        0     2171 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/521-31.png
--rw-r--r--   0        0        0     2388 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/521-32.png
--rw-r--r--   0        0        0     2587 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/521-33.png
--rw-r--r--   0        0        0     6797 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/525.png
--rw-r--r--   0        0        0     2186 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/531-10.png
--rw-r--r--   0        0        0     2097 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/531-20.png
--rw-r--r--   0        0        0     1390 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/531-21.png
--rw-r--r--   0        0        0     2239 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/533-22.png
--rw-r--r--   0        0        0     1279 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/550-20.png
--rw-r--r--   0        0        0     1180 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/600-30.png
--rw-r--r--   0        0        0     1562 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/600-31.png
--rw-r--r--   0        0        0      958 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/600-32.png
--rw-r--r--   0        0        0      848 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/600-34.png
--rw-r--r--   0        0        0      633 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/600-35.png
--rw-r--r--   0        0        0      729 2023-02-01 09:07:46.256367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/600-38.png
--rw-r--r--   0        0        0     5294 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/605-10.png
--rw-r--r--   0        0        0     2361 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/605-11.png
--rw-r--r--   0        0        0     5294 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/605-20.png
--rw-r--r--   0        0        0    16340 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/605-21.png
--rw-r--r--   0        0        0    10798 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/605-31.png
--rw-r--r--   0        0        0     3546 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-10.png
--rw-r--r--   0        0        0      960 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-11.png
--rw-r--r--   0        0        0     3499 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-12.png
--rw-r--r--   0        0        0     4442 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-13.png
--rw-r--r--   0        0        0     3518 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-20.png
--rw-r--r--   0        0        0      952 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-21.png
--rw-r--r--   0        0        0     3426 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-22.png
--rw-r--r--   0        0        0     4550 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-23.png
--rw-r--r--   0        0        0     3053 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/626-10.png
--rw-r--r--   0        0        0     3254 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/626-20.png
--rw-r--r--   0        0        0     1784 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/626-30.png
--rw-r--r--   0        0        0     1569 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/626-31.png
--rw-r--r--   0        0        0    58145 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/626-32.png
--rw-r--r--   0        0        0     2639 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/628-10.png
--rw-r--r--   0        0        0     3163 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/629-10.png
--rw-r--r--   0        0        0     5889 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/629-20.png
--rw-r--r--   0        0        0     4609 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/720.png
--rw-r--r--   0        0        0     3377 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDRussia/.png
--rw-r--r--   0        0        0     3377 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDSpain/.png
--rw-r--r--   0        0        0     5275 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r1.png
--rw-r--r--   0        0        0     6767 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r100.png
--rw-r--r--   0        0        0     4672 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r101.png
--rw-r--r--   0        0        0     7762 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r106.png
--rw-r--r--   0        0        0     9177 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r107.png
--rw-r--r--   0        0        0     4678 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r2.png
--rw-r--r--   0        0        0     7978 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r205.png
--rw-r--r--   0        0        0     7738 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r301.png
--rw-r--r--   0        0        0     8609 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r305.png
--rw-r--r--   0        0        0     7639 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r307.png
--rw-r--r--   0        0        0     7220 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r308.png
--rw-r--r--   0        0        0     9567 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDSpain/s13.png
--rw-r--r--   0        0        0     3377 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/.png
--rw-r--r--   0        0        0    11013 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/CW20-1.png
--rw-r--r--   0        0        0     5884 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/D1-2.png
--rw-r--r--   0        0        0     1961 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/M6-2aL.png
--rw-r--r--   0        0        0    73748 2023-03-05 16:45:57.229377 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R1-3.png
--rw-r--r--   0        0        0    51437 2023-03-05 16:45:57.229377 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R10-11.png
--rw-r--r--   0        0        0    11452 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R10-7.png
--rw-r--r--   0        0        0     2653 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R2-1.png
--rw-r--r--   0        0        0     8495 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-1.png
--rw-r--r--   0        0        0     8784 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-2.png
--rw-r--r--   0        0        0    11718 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-27.png
--rw-r--r--   0        0        0     9546 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-4.png
--rw-r--r--   0        0        0     8410 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-5L.png
--rw-r--r--   0        0        0     2705 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-5R.png
--rw-r--r--   0        0        0     3191 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-8b.png
--rw-r--r--   0        0        0     2702 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R4-7.png
--rw-r--r--   0        0        0     9439 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R5-1.png
--rw-r--r--   0        0        0     2129 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R6-1L.png
--rw-r--r--   0        0        0     2038 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R6-1R.png
--rw-r--r--   0        0        0     7606 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R7-1.png
--rw-r--r--   0        0        0     7189 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R7-107.png
--rw-r--r--   0        0        0     2983 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R7-201a.png
--rw-r--r--   0        0        0     7476 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R7-4.png
--rw-r--r--   0        0        0     8741 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R7-8.png
--rw-r--r--   0        0        0     7082 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R8-3.png
--rw-r--r--   0        0        0     5076 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R8-3C.png
--rw-r--r--   0        0        0     5343 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R8-3gP.png
--rw-r--r--   0        0        0    14945 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/W1-3L.png
--rw-r--r--   0        0        0     6551 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/W1-6L.png
--rw-r--r--   0        0        0    10176 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/W11-2.png
--rw-r--r--   0        0        0    10807 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/W3-3.png
--rw-r--r--   0        0        0    16719 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/W4-2R.png
--rw-r--r--   0        0        0     3377 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/.png
--rw-r--r--   0        0        0     3513 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000-10.png
--rw-r--r--   0        0        0     4708 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000-11.png
--rw-r--r--   0        0        0     3627 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000-20.png
--rw-r--r--   0        0        0     4340 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000-21.png
--rw-r--r--   0        0        0     4898 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000-30.png
--rw-r--r--   0        0        0     4788 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000-31.png
--rw-r--r--   0        0        0     1312 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000.png
--rw-r--r--   0        0        0     4181 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1001-30.png
--rw-r--r--   0        0        0     4687 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1001-31.png
--rw-r--r--   0        0        0     3091 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-10.png
--rw-r--r--   0        0        0     2965 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-11.png
--rw-r--r--   0        0        0     3006 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-12.png
--rw-r--r--   0        0        0     3044 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-13.png
--rw-r--r--   0        0        0     2957 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-14.png
--rw-r--r--   0        0        0     2937 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-20.png
--rw-r--r--   0        0        0     3005 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-21.png
--rw-r--r--   0        0        0     2873 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-22.png
--rw-r--r--   0        0        0     2872 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-23.png
--rw-r--r--   0        0        0     2944 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-24.png
--rw-r--r--   0        0        0     3147 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1004-30.png
--rw-r--r--   0        0        0     3678 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1004-31.png
--rw-r--r--   0        0        0     4872 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1004-32.png
--rw-r--r--   0        0        0     2960 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1004-33.png
--rw-r--r--   0        0        0     2939 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1004-34.png
--rw-r--r--   0        0        0     2385 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1004-35.png
--rw-r--r--   0        0        0     2985 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-30.png
--rw-r--r--   0        0        0     2792 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-31.png
--rw-r--r--   0        0        0     3037 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-32.png
--rw-r--r--   0        0        0     4135 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-33.png
--rw-r--r--   0        0        0     4419 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-34.png
--rw-r--r--   0        0        0     4321 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-35.png
--rw-r--r--   0        0        0     4095 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-36.png
--rw-r--r--   0        0        0     3849 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-37.png
--rw-r--r--   0        0        0     2317 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-38.png
--rw-r--r--   0        0        0     3612 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-39.png
--rw-r--r--   0        0        0     2188 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1007-31.png
--rw-r--r--   0        0        0     6916 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/101.png
--rw-r--r--   0        0        0     2147 2023-02-01 09:07:46.260367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1010-10.png
--rw-r--r--   0        0        0     2873 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1010-11.png
--rw-r--r--   0        0        0     1827 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1010-12.png
--rw-r--r--   0        0        0     2819 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1010-13.png
--rw-r--r--   0        0        0     3029 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1010-14.png
--rw-r--r--   0        0        0     1704 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-30.png
--rw-r--r--   0        0        0     1418 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-31.png
--rw-r--r--   0        0        0     3480 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-32.png
--rw-r--r--   0        0        0     2572 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-33.png
--rw-r--r--   0        0        0     3343 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-34.png
--rw-r--r--   0        0        0     2933 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-35.png
--rw-r--r--   0        0        0     2066 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-36.png
--rw-r--r--   0        0        0     3120 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-37.png
--rw-r--r--   0        0        0     2050 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-38.png
--rw-r--r--   0        0        0     2112 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-50.png
--rw-r--r--   0        0        0     2485 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-51.png
--rw-r--r--   0        0        0     2339 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-52.png
--rw-r--r--   0        0        0     2516 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-53.png
--rw-r--r--   0        0        0     6735 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/102.png
--rw-r--r--   0        0        0     5597 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1020-30.png
--rw-r--r--   0        0        0     6417 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1022-10.png
--rw-r--r--   0        0        0     5950 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1024-10.png
--rw-r--r--   0        0        0     8026 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1026-36.png
--rw-r--r--   0        0        0     8026 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1026-37.png
--rw-r--r--   0        0        0     8026 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1026-38.png
--rw-r--r--   0        0        0     8666 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/103-10.png
--rw-r--r--   0        0        0     7320 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/103-20.png
--rw-r--r--   0        0        0     4042 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1031-52.png
--rw-r--r--   0        0        0     2650 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1040-30.png
--rw-r--r--   0        0        0     3159 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1048-12.png
--rw-r--r--   0        0        0     5224 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1049-13.png
--rw-r--r--   0        0        0     3680 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1052-31.png
--rw-r--r--   0        0        0     4316 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1053-33.png
--rw-r--r--   0        0        0     2901 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1053-34.png
--rw-r--r--   0        0        0     3762 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1053-35.png
--rw-r--r--   0        0        0    12644 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/108.png
--rw-r--r--   0        0        0     8398 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/114.png
--rw-r--r--   0        0        0     5977 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/120.png
--rw-r--r--   0        0        0    13791 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/123.png
--rw-r--r--   0        0        0     9003 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/124.png
--rw-r--r--   0        0        0     8510 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/125.png
--rw-r--r--   0        0        0     6937 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/131.png
--rw-r--r--   0        0        0     9228 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/133-10.png
--rw-r--r--   0        0        0     9320 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/133-20.png
--rw-r--r--   0        0        0     8610 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/138.png
--rw-r--r--   0        0        0    11307 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/142-10.png
--rw-r--r--   0        0        0     6381 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/145-50.png
--rw-r--r--   0        0        0    12735 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/201.png
--rw-r--r--   0        0        0     5582 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/205.png
--rw-r--r--   0        0        0     5067 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/206.png
--rw-r--r--   0        0        0    13812 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/208.png
--rw-r--r--   0        0        0     7132 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/209-10.png
--rw-r--r--   0        0        0    11978 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/209-20.png
--rw-r--r--   0        0        0     6924 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/209-30.png
--rw-r--r--   0        0        0     7083 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/209.png
--rw-r--r--   0        0        0     6937 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/211-10.png
--rw-r--r--   0        0        0     6249 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/211-20.png
--rw-r--r--   0        0        0     6920 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/211.png
--rw-r--r--   0        0        0    16931 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/2113.png
--rw-r--r--   0        0        0     7799 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/214-10.png
--rw-r--r--   0        0        0     7333 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/214-30.png
--rw-r--r--   0        0        0     7769 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/214.png
--rw-r--r--   0        0        0    11470 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/215.png
--rw-r--r--   0        0        0     5287 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/220-10.png
--rw-r--r--   0        0        0     5359 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/220-20.png
--rw-r--r--   0        0        0     8269 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/222-10.png
--rw-r--r--   0        0        0     8297 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/222-20.png
--rw-r--r--   0        0        0     4342 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/223.2-50.png
--rw-r--r--   0        0        0     5405 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/223.2-51.png
--rw-r--r--   0        0        0     4747 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/223.2.png
--rw-r--r--   0        0        0     6167 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/224-50.png
--rw-r--r--   0        0        0    17675 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/237.png
--rw-r--r--   0        0        0    15792 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/239.png
--rw-r--r--   0        0        0    15236 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/240.png
--rw-r--r--   0        0        0    11564 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/242.1.png
--rw-r--r--   0        0        0    10015 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/242.2.png
--rw-r--r--   0        0        0    13431 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/244.1.png
--rw-r--r--   0        0        0    10786 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/244.2.png
--rw-r--r--   0        0        0    14243 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/245.png
--rw-r--r--   0        0        0    12752 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/250.png
--rw-r--r--   0        0        0     8903 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/251.png
--rw-r--r--   0        0        0    14665 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/253.png
--rw-r--r--   0        0        0    10381 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/254.png
--rw-r--r--   0        0        0    16226 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/255.png
--rw-r--r--   0        0        0    15152 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/257-54.png
--rw-r--r--   0        0        0     9437 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/259.png
--rw-r--r--   0        0        0    18193 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/260.png
--rw-r--r--   0        0        0    14767 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/261.png
--rw-r--r--   0        0        0    13173 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/262.png
--rw-r--r--   0        0        0    13739 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/264.png
--rw-r--r--   0        0        0    13764 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/265.png
--rw-r--r--   0        0        0    15436 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/266.png
--rw-r--r--   0        0        0     6366 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/267.png
--rw-r--r--   0        0        0     6424 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/270.1.png
--rw-r--r--   0        0        0     6871 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/270.2.png
--rw-r--r--   0        0        0    10406 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/272.png
--rw-r--r--   0        0        0     4996 2023-02-01 09:07:46.264367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/274.1.png
--rw-r--r--   0        0        0     7607 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/274.2.png
--rw-r--r--   0        0        0     7804 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/274.png
--rw-r--r--   0        0        0     6449 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/275.png
--rw-r--r--   0        0        0     8759 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/276.png
--rw-r--r--   0        0        0     9330 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/277.png
--rw-r--r--   0        0        0     6601 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/278.png
--rw-r--r--   0        0        0     6835 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/279.png
--rw-r--r--   0        0        0     8452 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/280.png
--rw-r--r--   0        0        0     8087 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/281.png
--rw-r--r--   0        0        0     6469 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/282.png
--rw-r--r--   0        0        0    11770 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/283-10.png
--rw-r--r--   0        0        0    12188 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/283-30.png
--rw-r--r--   0        0        0    12156 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/286-30.png
--rw-r--r--   0        0        0     8130 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/286.png
--rw-r--r--   0        0        0     5908 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/301.png
--rw-r--r--   0        0        0     3956 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/306.png
--rw-r--r--   0        0        0     5671 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/308.png
--rw-r--r--   0        0        0     5401 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/310.png
--rw-r--r--   0        0        0     7203 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/311.png
--rw-r--r--   0        0        0     2529 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/314-10.png
--rw-r--r--   0        0        0     2569 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/314-20.png
--rw-r--r--   0        0        0     2705 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/314-30.png
--rw-r--r--   0        0        0     2317 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/314.png
--rw-r--r--   0        0        0    10625 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/325.1.png
--rw-r--r--   0        0        0    12383 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/325.2.png
--rw-r--r--   0        0        0     5815 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/327.png
--rw-r--r--   0        0        0     2544 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/328.png
--rw-r--r--   0        0        0     2225 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/330.1.png
--rw-r--r--   0        0        0     8637 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/330.2.png
--rw-r--r--   0        0        0     3567 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/331.1.png
--rw-r--r--   0        0        0     4310 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/331.2.png
--rw-r--r--   0        0        0     3983 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/332.1.png
--rw-r--r--   0        0        0     7257 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/332.png
--rw-r--r--   0        0        0     4616 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/333-20.png
--rw-r--r--   0        0        0     3350 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/333-21.png
--rw-r--r--   0        0        0     2663 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/333-22.png
--rw-r--r--   0        0        0     4496 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/333.png
--rw-r--r--   0        0        0     5223 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/350.png
--rw-r--r--   0        0        0     8456 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/354.png
--rw-r--r--   0        0        0     5080 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/356.png
--rw-r--r--   0        0        0     3049 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/357.png
--rw-r--r--   0        0        0     1854 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/363.png
--rw-r--r--   0        0        0     5740 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/365-51.png
--rw-r--r--   0        0        0     3878 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/365-52.png
--rw-r--r--   0        0        0     3515 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/365-60.png
--rw-r--r--   0        0        0     1124 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/380.png
--rw-r--r--   0        0        0     1588 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/381.png
--rw-r--r--   0        0        0     2438 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/386.1.png
--rw-r--r--   0        0        0     4572 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/386.2.png
--rw-r--r--   0        0        0     4247 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/386.3.png
--rw-r--r--   0        0        0    11292 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/406-50.png
--rw-r--r--   0        0        0     2691 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/418-20.png
--rw-r--r--   0        0        0     1852 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/419-20.png
--rw-r--r--   0        0        0     2638 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/430-20.png
--rw-r--r--   0        0        0     1709 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/432-10.png
--rw-r--r--   0        0        0     2271 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/432-20.png
--rw-r--r--   0        0        0     6106 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/434-50.png
--rw-r--r--   0        0        0     8563 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/434.png
--rw-r--r--   0        0        0     3168 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/438.png
--rw-r--r--   0        0        0     3361 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/439.png
--rw-r--r--   0        0        0     5870 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/440.png
--rw-r--r--   0        0        0     7617 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/448.png
--rw-r--r--   0        0        0     9309 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/449.png
--rw-r--r--   0        0        0     3520 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/450-50.png
--rw-r--r--   0        0        0     4770 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/450-51.png
--rw-r--r--   0        0        0     5217 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/450-52.png
--rw-r--r--   0        0        0     4938 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/450-53.png
--rw-r--r--   0        0        0     6058 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/450-54.png
--rw-r--r--   0        0        0     6767 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/450-55.png
--rw-r--r--   0        0        0     6353 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/453.png
--rw-r--r--   0        0        0     2018 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/455.1-30.png
--rw-r--r--   0        0        0     5836 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/458.png
--rw-r--r--   0        0        0     3959 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/460-10.png
--rw-r--r--   0        0        0     3966 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/460-12.png
--rw-r--r--   0        0        0     1865 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/460-20.png
--rw-r--r--   0        0        0     1728 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/460-21.png
--rw-r--r--   0        0        0     1815 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/460-22.png
--rw-r--r--   0        0        0     1775 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/460-30.png
--rw-r--r--   0        0        0     3619 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/501-15.png
--rw-r--r--   0        0        0     2458 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/501-16.png
--rw-r--r--   0        0        0    45510 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/511-22.png
--rw-r--r--   0        0        0     1985 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/521-30.png
--rw-r--r--   0        0        0     2171 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/521-31.png
--rw-r--r--   0        0        0     2388 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/521-32.png
--rw-r--r--   0        0        0     2587 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/521-33.png
--rw-r--r--   0        0        0     6797 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/525.png
--rw-r--r--   0        0        0     2186 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/531-10.png
--rw-r--r--   0        0        0     2097 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/531-20.png
--rw-r--r--   0        0        0     1390 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/531-21.png
--rw-r--r--   0        0        0     2239 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/533-22.png
--rw-r--r--   0        0        0     1279 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/550-20.png
--rw-r--r--   0        0        0     1180 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/600-30.png
--rw-r--r--   0        0        0     1562 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/600-31.png
--rw-r--r--   0        0        0      958 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/600-32.png
--rw-r--r--   0        0        0      848 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/600-34.png
--rw-r--r--   0        0        0      633 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/600-35.png
--rw-r--r--   0        0        0      729 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/600-38.png
--rw-r--r--   0        0        0     5294 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/605-10.png
--rw-r--r--   0        0        0     2361 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/605-11.png
--rw-r--r--   0        0        0     5294 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/605-20.png
--rw-r--r--   0        0        0    16340 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/605-21.png
--rw-r--r--   0        0        0    10798 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/605-31.png
--rw-r--r--   0        0        0     3546 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-10.png
--rw-r--r--   0        0        0      960 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-11.png
--rw-r--r--   0        0        0     3499 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-12.png
--rw-r--r--   0        0        0     4442 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-13.png
--rw-r--r--   0        0        0     3518 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-20.png
--rw-r--r--   0        0        0      952 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-21.png
--rw-r--r--   0        0        0     3426 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-22.png
--rw-r--r--   0        0        0     4550 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-23.png
--rw-r--r--   0        0        0     3053 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/626-10.png
--rw-r--r--   0        0        0     3254 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/626-20.png
--rw-r--r--   0        0        0     1784 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/626-30.png
--rw-r--r--   0        0        0     1569 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/626-31.png
--rw-r--r--   0        0        0    58145 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/626-32.png
--rw-r--r--   0        0        0     2639 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/628-10.png
--rw-r--r--   0        0        0     3163 2023-02-01 09:07:46.268367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/629-10.png
--rw-r--r--   0        0        0     5889 2023-02-01 09:07:46.272367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/629-20.png
--rw-r--r--   0        0        0     4609 2023-02-01 09:07:46.272367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/720.png
--rw-r--r--   0        0        0     5312 2023-02-01 09:07:46.272367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/traffic_light_state_green.png
--rw-r--r--   0        0        0     5157 2023-02-01 09:07:46.272367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/traffic_light_state_inactive.png
--rw-r--r--   0        0        0     4943 2023-02-01 09:07:46.272367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/traffic_light_state_red.png
--rw-r--r--   0        0        0     4872 2023-02-01 09:07:46.272367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/traffic_light_state_redYellow.png
--rw-r--r--   0        0        0     5093 2023-02-01 09:07:46.272367 commonroad_io-2023.1/commonroad/visualization/traffic_signs/traffic_light_state_yellow.png
--rw-r--r--   0        0        0    12053 2023-03-05 16:45:57.229377 commonroad_io-2023.1/commonroad/visualization/util.py
--rw-r--r--   0        0        0     2243 2023-03-05 16:45:57.233378 commonroad_io-2023.1/pyproject.toml
--rw-r--r--   0        0        0     9887 1970-01-01 00:00:00.000000 commonroad_io-2023.1/PKG-INFO
+-rw-r--r--   0        0        0     1554 2023-05-04 10:35:48.062737 commonroad_io-2023.2/LICENSE.txt
+-rw-r--r--   0        0        0     8478 2023-06-26 05:26:51.184356 commonroad_io-2023.2/README.md
+-rw-r--r--   0        0        0      218 2023-05-04 10:35:48.062737 commonroad_io-2023.2/commonroad/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 05:32:06.468806 commonroad_io-2023.2/commonroad/common/__init__.py
+-rw-r--r--   0        0        0     5985 2023-06-26 01:03:15.666438 commonroad_io-2023.2/commonroad/common/common_lanelet.py
+-rw-r--r--   0        0        0     1913 2023-06-26 01:03:15.666438 commonroad_io-2023.2/commonroad/common/file_reader.py
+-rw-r--r--   0        0        0     3772 2023-06-26 01:03:15.666438 commonroad_io-2023.2/commonroad/common/file_writer.py
+-rw-r--r--   0        0        0        0 2023-06-26 05:32:06.468806 commonroad_io-2023.2/commonroad/common/reader/__init__.py
+-rw-r--r--   0        0        0      675 2023-06-26 01:03:15.666438 commonroad_io-2023.2/commonroad/common/reader/file_reader_interface.py
+-rw-r--r--   0        0        0    41904 2023-06-26 01:03:15.666438 commonroad_io-2023.2/commonroad/common/reader/file_reader_protobuf.py
+-rw-r--r--   0        0        0    74164 2023-06-26 01:03:15.666438 commonroad_io-2023.2/commonroad/common/reader/file_reader_xml.py
+-rw-r--r--   0        0        0    34706 2023-06-01 14:46:40.318919 commonroad_io-2023.2/commonroad/common/solution.py
+-rw-r--r--   0        0        0    10970 2023-05-08 01:03:25.435708 commonroad_io-2023.2/commonroad/common/util.py
+-rw-r--r--   0        0        0    11492 2023-05-08 01:03:25.435708 commonroad_io-2023.2/commonroad/common/validity.py
+-rw-r--r--   0        0        0        0 2023-06-26 05:32:06.468806 commonroad_io-2023.2/commonroad/common/writer/__init__.py
+-rw-r--r--   0        0        0     4796 2023-06-26 01:03:15.666438 commonroad_io-2023.2/commonroad/common/writer/file_writer_interface.py
+-rw-r--r--   0        0        0    38622 2023-06-26 01:03:15.666438 commonroad_io-2023.2/commonroad/common/writer/file_writer_protobuf.py
+-rw-r--r--   0        0        0    52138 2023-06-26 01:03:15.666438 commonroad_io-2023.2/commonroad/common/writer/file_writer_xml.py
+-rw-r--r--   0        0        0        0 2023-06-26 05:32:06.468806 commonroad_io-2023.2/commonroad/geometry/__init__.py
+-rw-r--r--   0        0        0    15029 2023-05-04 10:35:48.066737 commonroad_io-2023.2/commonroad/geometry/polyline_util.py
+-rw-r--r--   0        0        0    28507 2023-05-08 01:03:25.435708 commonroad_io-2023.2/commonroad/geometry/shape.py
+-rw-r--r--   0        0        0     3870 2023-05-04 10:35:48.066737 commonroad_io-2023.2/commonroad/geometry/transform.py
+-rw-r--r--   0        0        0        0 2023-06-26 05:32:06.468806 commonroad_io-2023.2/commonroad/planning/__init__.py
+-rw-r--r--   0        0        0    10244 2023-05-04 10:35:48.066737 commonroad_io-2023.2/commonroad/planning/goal.py
+-rw-r--r--   0        0        0     8567 2023-06-26 01:03:15.666438 commonroad_io-2023.2/commonroad/planning/planning_problem.py
+-rw-r--r--   0        0        0        0 2023-06-26 05:32:06.468806 commonroad_io-2023.2/commonroad/prediction/__init__.py
+-rw-r--r--   0        0        0    16224 2023-06-01 14:46:40.318919 commonroad_io-2023.2/commonroad/prediction/prediction.py
+-rw-r--r--   0        0        0        0 2023-06-26 05:32:06.468806 commonroad_io-2023.2/commonroad/scenario/__init__.py
+-rw-r--r--   0        0        0     4757 2023-06-26 01:03:15.666438 commonroad_io-2023.2/commonroad/scenario/area.py
+-rw-r--r--   0        0        0    10257 2023-06-26 01:03:15.666438 commonroad_io-2023.2/commonroad/scenario/intersection.py
+-rw-r--r--   0        0        0    81359 2023-06-26 05:26:51.184356 commonroad_io-2023.2/commonroad/scenario/lanelet.py
+-rw-r--r--   0        0        0    42531 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario/obstacle.py
+-rw-r--r--   0        0        0    54698 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario/scenario.py
+-rw-r--r--   0        0        0    18687 2023-06-01 14:46:40.318919 commonroad_io-2023.2/commonroad/scenario/state.py
+-rw-r--r--   0        0        0    11970 2023-05-26 16:09:26.974367 commonroad_io-2023.2/commonroad/scenario/traffic_light.py
+-rw-r--r--   0        0        0    32306 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario/traffic_sign.py
+-rw-r--r--   0        0        0     3982 2023-05-04 10:35:48.066737 commonroad_io-2023.2/commonroad/scenario/traffic_sign_interpreter.py
+-rw-r--r--   0        0        0    12767 2023-05-08 01:03:25.435708 commonroad_io-2023.2/commonroad/scenario/trajectory.py
+-rw-r--r--   0        0        0        0 2023-06-26 05:32:06.468806 commonroad_io-2023.2/commonroad/scenario_definition/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-26 05:32:06.468806 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/__init__.py
+-rw-r--r--   0        0        0     4752 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/convert_xml_to_pb.py
+-rw-r--r--   0        0        0     1280 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/definition_files/commonroad.proto
+-rw-r--r--   0        0        0      523 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/definition_files/dynamic_obstacle.proto
+-rw-r--r--   0        0        0      269 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/definition_files/environment_obstacle.proto
+-rw-r--r--   0        0        0      452 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/definition_files/intersection.proto
+-rw-r--r--   0        0        0     2134 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/definition_files/lanelet.proto
+-rw-r--r--   0        0        0     1217 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/definition_files/location.proto
+-rw-r--r--   0        0        0     3442 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/definition_files/obstacle.proto
+-rw-r--r--   0        0        0      179 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/definition_files/phantom_obstacle.proto
+-rw-r--r--   0        0        0      318 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/definition_files/planning_problem.proto
+-rw-r--r--   0        0        0      844 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/definition_files/scenario_tags.proto
+-rw-r--r--   0        0        0      383 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/definition_files/static_obstacle.proto
+-rw-r--r--   0        0        0      880 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/definition_files/traffic_light.proto
+-rw-r--r--   0        0        0    22979 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/definition_files/traffic_sign.proto
+-rw-r--r--   0        0        0     1353 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/definition_files/util.proto
+-rw-r--r--   0        0        0        0 2023-06-26 05:32:06.472806 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/__init__.py
+-rw-r--r--   0        0        0    15076 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/commonroad_pb2.py
+-rw-r--r--   0        0        0     7351 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/dynamic_obstacle_pb2.py
+-rw-r--r--   0        0        0     3688 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/environment_obstacle_pb2.py
+-rw-r--r--   0        0        0     6602 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/intersection_pb2.py
+-rw-r--r--   0        0        0    27162 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/lanelet_pb2.py
+-rw-r--r--   0        0        0    17811 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/location_pb2.py
+-rw-r--r--   0        0        0    43107 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/obstacle_pb2.py
+-rw-r--r--   0        0        0     2824 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/phantom_obstacle_pb2.py
+-rw-r--r--   0        0        0     5197 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/planning_problem_pb2.py
+-rw-r--r--   0        0        0     9253 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/scenario_tags_pb2.py
+-rw-r--r--   0        0        0     5311 2023-06-26 01:03:15.670438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/static_obstacle_pb2.py
+-rw-r--r--   0        0        0    12268 2023-06-26 01:03:15.674438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/traffic_light_pb2.py
+-rw-r--r--   0        0        0   169832 2023-06-26 01:03:15.674438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/traffic_sign_pb2.py
+-rw-r--r--   0        0        0    27145 2023-06-26 01:03:15.674438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/util_pb2.py
+-rw-r--r--   0        0        0     1120 2023-06-26 01:03:15.674438 commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/how_to_protobuf.md
+-rw-r--r--   0        0        0     7849 2023-06-26 01:03:15.674438 commonroad_io-2023.2/commonroad/scenario_definition/xml_definition_files/CommonRoadSolution_schema.xsd
+-rw-r--r--   0        0        0    42394 2023-06-26 01:03:15.674438 commonroad_io-2023.2/commonroad/scenario_definition/xml_definition_files/XML_commonRoad_XSD.xsd
+-rw-r--r--   0        0        0        0 2023-06-26 05:32:06.472806 commonroad_io-2023.2/commonroad/visualization/__init__.py
+-rw-r--r--   0        0        0    14598 2023-05-04 10:35:48.070737 commonroad_io-2023.2/commonroad/visualization/draw_params.py
+-rw-r--r--   0        0        0      598 2023-05-04 10:35:48.070737 commonroad_io-2023.2/commonroad/visualization/drawable.py
+-rw-r--r--   0        0        0    12857 2023-05-04 10:35:48.070737 commonroad_io-2023.2/commonroad/visualization/icons.py
+-rw-r--r--   0        0        0    66222 2023-06-26 01:03:15.674438 commonroad_io-2023.2/commonroad/visualization/mp_renderer.py
+-rw-r--r--   0        0        0     6115 2023-05-04 10:35:48.070737 commonroad_io-2023.2/commonroad/visualization/renderer.py
+-rw-r--r--   0        0        0    21544 2023-05-08 01:03:25.439708 commonroad_io-2023.2/commonroad/visualization/traffic_sign.py
+-rw-r--r--   0        0        0     3377 2023-05-04 10:35:48.070737 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDChina/.png
+-rw-r--r--   0        0        0     3377 2023-05-04 10:35:48.070737 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/.png
+-rw-r--r--   0        0        0     3513 2023-05-04 10:35:48.070737 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000-10.png
+-rw-r--r--   0        0        0     4708 2023-05-04 10:35:48.070737 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000-11.png
+-rw-r--r--   0        0        0     3627 2023-05-04 10:35:48.070737 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000-20.png
+-rw-r--r--   0        0        0     4340 2023-05-04 10:35:48.070737 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000-21.png
+-rw-r--r--   0        0        0     4898 2023-05-04 10:35:48.070737 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000-30.png
+-rw-r--r--   0        0        0     4788 2023-05-04 10:35:48.070737 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000-31.png
+-rw-r--r--   0        0        0     1312 2023-05-04 10:35:48.070737 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000.png
+-rw-r--r--   0        0        0     4181 2023-05-04 10:35:48.070737 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1001-30.png
+-rw-r--r--   0        0        0     4687 2023-05-04 10:35:48.070737 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1001-31.png
+-rw-r--r--   0        0        0     3091 2023-05-04 10:35:48.070737 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-10.png
+-rw-r--r--   0        0        0     2965 2023-05-04 10:35:48.070737 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-11.png
+-rw-r--r--   0        0        0     3006 2023-05-04 10:35:48.070737 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-12.png
+-rw-r--r--   0        0        0     3044 2023-05-04 10:35:48.070737 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-13.png
+-rw-r--r--   0        0        0     2957 2023-05-04 10:35:48.070737 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-14.png
+-rw-r--r--   0        0        0     2937 2023-05-04 10:35:48.070737 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-20.png
+-rw-r--r--   0        0        0     3005 2023-05-04 10:35:48.070737 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-21.png
+-rw-r--r--   0        0        0     2873 2023-05-04 10:35:48.070737 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-22.png
+-rw-r--r--   0        0        0     2872 2023-05-04 10:35:48.070737 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-23.png
+-rw-r--r--   0        0        0     2944 2023-05-04 10:35:48.070737 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-24.png
+-rw-r--r--   0        0        0     3147 2023-05-04 10:35:48.070737 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1004-30.png
+-rw-r--r--   0        0        0     3678 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1004-31.png
+-rw-r--r--   0        0        0     4872 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1004-32.png
+-rw-r--r--   0        0        0     2960 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1004-33.png
+-rw-r--r--   0        0        0     2939 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1004-34.png
+-rw-r--r--   0        0        0     2385 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1004-35.png
+-rw-r--r--   0        0        0     2985 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-30.png
+-rw-r--r--   0        0        0     2792 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-31.png
+-rw-r--r--   0        0        0     3037 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-32.png
+-rw-r--r--   0        0        0     4135 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-33.png
+-rw-r--r--   0        0        0     4419 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-34.png
+-rw-r--r--   0        0        0     4321 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-35.png
+-rw-r--r--   0        0        0     4095 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-36.png
+-rw-r--r--   0        0        0     3849 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-37.png
+-rw-r--r--   0        0        0     2317 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-38.png
+-rw-r--r--   0        0        0     3612 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-39.png
+-rw-r--r--   0        0        0     2188 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1007-31.png
+-rw-r--r--   0        0        0     6916 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/101.png
+-rw-r--r--   0        0        0     2147 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1010-10.png
+-rw-r--r--   0        0        0     2873 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1010-11.png
+-rw-r--r--   0        0        0     1827 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1010-12.png
+-rw-r--r--   0        0        0     2819 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1010-13.png
+-rw-r--r--   0        0        0     3029 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1010-14.png
+-rw-r--r--   0        0        0     1704 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-30.png
+-rw-r--r--   0        0        0     1418 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-31.png
+-rw-r--r--   0        0        0     3480 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-32.png
+-rw-r--r--   0        0        0     2572 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-33.png
+-rw-r--r--   0        0        0     3343 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-34.png
+-rw-r--r--   0        0        0     2933 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-35.png
+-rw-r--r--   0        0        0     2066 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-36.png
+-rw-r--r--   0        0        0     3120 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-37.png
+-rw-r--r--   0        0        0     2050 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-38.png
+-rw-r--r--   0        0        0     2112 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-50.png
+-rw-r--r--   0        0        0     2485 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-51.png
+-rw-r--r--   0        0        0     2339 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-52.png
+-rw-r--r--   0        0        0     2516 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-53.png
+-rw-r--r--   0        0        0     6735 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/102.png
+-rw-r--r--   0        0        0     5597 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1020-30.png
+-rw-r--r--   0        0        0     6417 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1022-10.png
+-rw-r--r--   0        0        0     5950 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1024-10.png
+-rw-r--r--   0        0        0     8026 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1026-36.png
+-rw-r--r--   0        0        0     8026 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1026-37.png
+-rw-r--r--   0        0        0     8026 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1026-38.png
+-rw-r--r--   0        0        0     8666 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/103-10.png
+-rw-r--r--   0        0        0     7320 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/103-20.png
+-rw-r--r--   0        0        0     4042 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1031-52.png
+-rw-r--r--   0        0        0     2650 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1040-30.png
+-rw-r--r--   0        0        0     3159 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1048-12.png
+-rw-r--r--   0        0        0     5224 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1049-13.png
+-rw-r--r--   0        0        0     3680 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1052-31.png
+-rw-r--r--   0        0        0     4316 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1053-33.png
+-rw-r--r--   0        0        0     2901 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1053-34.png
+-rw-r--r--   0        0        0     3762 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1053-35.png
+-rw-r--r--   0        0        0    12644 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/108.png
+-rw-r--r--   0        0        0     8398 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/114.png
+-rw-r--r--   0        0        0     5977 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/120.png
+-rw-r--r--   0        0        0    13791 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/123.png
+-rw-r--r--   0        0        0     9003 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/124.png
+-rw-r--r--   0        0        0     8510 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/125.png
+-rw-r--r--   0        0        0     6937 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/131.png
+-rw-r--r--   0        0        0     9228 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/133-10.png
+-rw-r--r--   0        0        0     9320 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/133-20.png
+-rw-r--r--   0        0        0     8610 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/138.png
+-rw-r--r--   0        0        0    11307 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/142-10.png
+-rw-r--r--   0        0        0     6381 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/145-50.png
+-rw-r--r--   0        0        0    12735 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/201.png
+-rw-r--r--   0        0        0     5582 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/205.png
+-rw-r--r--   0        0        0     5067 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/206.png
+-rw-r--r--   0        0        0    13812 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/208.png
+-rw-r--r--   0        0        0     7132 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/209-10.png
+-rw-r--r--   0        0        0    11978 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/209-20.png
+-rw-r--r--   0        0        0     6924 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/209-30.png
+-rw-r--r--   0        0        0     7083 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/209.png
+-rw-r--r--   0        0        0     6937 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/211-10.png
+-rw-r--r--   0        0        0     6249 2023-05-04 10:35:48.074736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/211-20.png
+-rw-r--r--   0        0        0     6920 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/211.png
+-rw-r--r--   0        0        0    16931 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/2113.png
+-rw-r--r--   0        0        0     7799 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/214-10.png
+-rw-r--r--   0        0        0     7333 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/214-30.png
+-rw-r--r--   0        0        0     7769 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/214.png
+-rw-r--r--   0        0        0    11470 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/215.png
+-rw-r--r--   0        0        0     5287 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/220-10.png
+-rw-r--r--   0        0        0     5359 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/220-20.png
+-rw-r--r--   0        0        0     8269 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/222-10.png
+-rw-r--r--   0        0        0     8297 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/222-20.png
+-rw-r--r--   0        0        0     4342 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/223.2-50.png
+-rw-r--r--   0        0        0     5405 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/223.2-51.png
+-rw-r--r--   0        0        0     4747 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/223.2.png
+-rw-r--r--   0        0        0     6167 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/224-50.png
+-rw-r--r--   0        0        0    17675 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/237.png
+-rw-r--r--   0        0        0    15792 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/239.png
+-rw-r--r--   0        0        0    15236 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/240.png
+-rw-r--r--   0        0        0    11564 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/242.1.png
+-rw-r--r--   0        0        0    10015 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/242.2.png
+-rw-r--r--   0        0        0    13431 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/244.1.png
+-rw-r--r--   0        0        0    10786 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/244.2.png
+-rw-r--r--   0        0        0    14243 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/245.png
+-rw-r--r--   0        0        0    12752 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/250.png
+-rw-r--r--   0        0        0     8903 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/251.png
+-rw-r--r--   0        0        0    14665 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/253.png
+-rw-r--r--   0        0        0    10381 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/254.png
+-rw-r--r--   0        0        0    16226 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/255.png
+-rw-r--r--   0        0        0    15152 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/257-54.png
+-rw-r--r--   0        0        0     9437 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/259.png
+-rw-r--r--   0        0        0    18193 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/260.png
+-rw-r--r--   0        0        0    14767 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/261.png
+-rw-r--r--   0        0        0    13173 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/262.png
+-rw-r--r--   0        0        0    13739 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/264.png
+-rw-r--r--   0        0        0    13764 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/265.png
+-rw-r--r--   0        0        0    15436 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/266.png
+-rw-r--r--   0        0        0     6366 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/267.png
+-rw-r--r--   0        0        0     6424 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/270.1.png
+-rw-r--r--   0        0        0     6871 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/270.2.png
+-rw-r--r--   0        0        0    10406 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/272.png
+-rw-r--r--   0        0        0     4996 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/274.1.png
+-rw-r--r--   0        0        0     7607 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/274.2.png
+-rw-r--r--   0        0        0     7804 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/274.png
+-rw-r--r--   0        0        0     6449 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/275.png
+-rw-r--r--   0        0        0     8759 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/276.png
+-rw-r--r--   0        0        0     9330 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/277.png
+-rw-r--r--   0        0        0     6601 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/278.png
+-rw-r--r--   0        0        0     6835 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/279.png
+-rw-r--r--   0        0        0     8452 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/280.png
+-rw-r--r--   0        0        0     8087 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/281.png
+-rw-r--r--   0        0        0     6469 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/282.png
+-rw-r--r--   0        0        0    11770 2023-05-04 10:35:48.078736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/283-10.png
+-rw-r--r--   0        0        0    12188 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/283-30.png
+-rw-r--r--   0        0        0    12156 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/286-30.png
+-rw-r--r--   0        0        0     8130 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/286.png
+-rw-r--r--   0        0        0     5908 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/301.png
+-rw-r--r--   0        0        0     3956 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/306.png
+-rw-r--r--   0        0        0     5671 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/308.png
+-rw-r--r--   0        0        0     5401 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/310.png
+-rw-r--r--   0        0        0     7203 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/311.png
+-rw-r--r--   0        0        0     2529 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/314-10.png
+-rw-r--r--   0        0        0     2569 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/314-20.png
+-rw-r--r--   0        0        0     2705 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/314-30.png
+-rw-r--r--   0        0        0     2317 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/314.png
+-rw-r--r--   0        0        0    10625 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/325.1.png
+-rw-r--r--   0        0        0    12383 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/325.2.png
+-rw-r--r--   0        0        0     5815 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/327.png
+-rw-r--r--   0        0        0     2544 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/328.png
+-rw-r--r--   0        0        0     2225 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/330.1.png
+-rw-r--r--   0        0        0     8637 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/330.2.png
+-rw-r--r--   0        0        0     3567 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/331.1.png
+-rw-r--r--   0        0        0     4310 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/331.2.png
+-rw-r--r--   0        0        0     3983 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/332.1.png
+-rw-r--r--   0        0        0     7257 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/332.png
+-rw-r--r--   0        0        0     4616 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/333-20.png
+-rw-r--r--   0        0        0     3350 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/333-21.png
+-rw-r--r--   0        0        0     2663 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/333-22.png
+-rw-r--r--   0        0        0     4496 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/333.png
+-rw-r--r--   0        0        0     5223 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/350.png
+-rw-r--r--   0        0        0     8456 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/354.png
+-rw-r--r--   0        0        0     5080 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/356.png
+-rw-r--r--   0        0        0     3049 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/357.png
+-rw-r--r--   0        0        0     1854 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/363.png
+-rw-r--r--   0        0        0     5740 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/365-51.png
+-rw-r--r--   0        0        0     3878 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/365-52.png
+-rw-r--r--   0        0        0     3515 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/365-60.png
+-rw-r--r--   0        0        0     1124 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/380.png
+-rw-r--r--   0        0        0     1588 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/381.png
+-rw-r--r--   0        0        0     2438 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/386.1.png
+-rw-r--r--   0        0        0     4572 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/386.2.png
+-rw-r--r--   0        0        0     4247 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/386.3.png
+-rw-r--r--   0        0        0    11292 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/406-50.png
+-rw-r--r--   0        0        0     2691 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/418-20.png
+-rw-r--r--   0        0        0     1852 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/419-20.png
+-rw-r--r--   0        0        0     2638 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/430-20.png
+-rw-r--r--   0        0        0     1709 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/432-10.png
+-rw-r--r--   0        0        0     2271 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/432-20.png
+-rw-r--r--   0        0        0     6106 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/434-50.png
+-rw-r--r--   0        0        0     8563 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/434.png
+-rw-r--r--   0        0        0     3168 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/438.png
+-rw-r--r--   0        0        0     3361 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/439.png
+-rw-r--r--   0        0        0     5870 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/440.png
+-rw-r--r--   0        0        0     7617 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/448.png
+-rw-r--r--   0        0        0     9309 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/449.png
+-rw-r--r--   0        0        0     3520 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/450-50.png
+-rw-r--r--   0        0        0     4770 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/450-51.png
+-rw-r--r--   0        0        0     5217 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/450-52.png
+-rw-r--r--   0        0        0     4938 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/450-53.png
+-rw-r--r--   0        0        0     6058 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/450-54.png
+-rw-r--r--   0        0        0     6767 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/450-55.png
+-rw-r--r--   0        0        0     6353 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/453.png
+-rw-r--r--   0        0        0     2018 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/455.1-30.png
+-rw-r--r--   0        0        0     5836 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/458.png
+-rw-r--r--   0        0        0     3959 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/460-10.png
+-rw-r--r--   0        0        0     3966 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/460-12.png
+-rw-r--r--   0        0        0     1865 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/460-20.png
+-rw-r--r--   0        0        0     1728 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/460-21.png
+-rw-r--r--   0        0        0     1815 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/460-22.png
+-rw-r--r--   0        0        0     1775 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/460-30.png
+-rw-r--r--   0        0        0     3619 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/501-15.png
+-rw-r--r--   0        0        0     2458 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/501-16.png
+-rw-r--r--   0        0        0    45510 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/511-22.png
+-rw-r--r--   0        0        0     1985 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/521-30.png
+-rw-r--r--   0        0        0     2171 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/521-31.png
+-rw-r--r--   0        0        0     2388 2023-05-04 10:35:48.082736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/521-32.png
+-rw-r--r--   0        0        0     2587 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/521-33.png
+-rw-r--r--   0        0        0     6797 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/525.png
+-rw-r--r--   0        0        0     2186 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/531-10.png
+-rw-r--r--   0        0        0     2097 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/531-20.png
+-rw-r--r--   0        0        0     1390 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/531-21.png
+-rw-r--r--   0        0        0     2239 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/533-22.png
+-rw-r--r--   0        0        0     1279 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/550-20.png
+-rw-r--r--   0        0        0     1180 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/600-30.png
+-rw-r--r--   0        0        0     1562 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/600-31.png
+-rw-r--r--   0        0        0      958 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/600-32.png
+-rw-r--r--   0        0        0      848 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/600-34.png
+-rw-r--r--   0        0        0      633 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/600-35.png
+-rw-r--r--   0        0        0      729 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/600-38.png
+-rw-r--r--   0        0        0     5294 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/605-10.png
+-rw-r--r--   0        0        0     2361 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/605-11.png
+-rw-r--r--   0        0        0     5294 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/605-20.png
+-rw-r--r--   0        0        0    16340 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/605-21.png
+-rw-r--r--   0        0        0    10798 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/605-31.png
+-rw-r--r--   0        0        0     3546 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-10.png
+-rw-r--r--   0        0        0      960 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-11.png
+-rw-r--r--   0        0        0     3499 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-12.png
+-rw-r--r--   0        0        0     4442 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-13.png
+-rw-r--r--   0        0        0     3518 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-20.png
+-rw-r--r--   0        0        0      952 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-21.png
+-rw-r--r--   0        0        0     3426 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-22.png
+-rw-r--r--   0        0        0     4550 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-23.png
+-rw-r--r--   0        0        0     3053 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/626-10.png
+-rw-r--r--   0        0        0     3254 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/626-20.png
+-rw-r--r--   0        0        0     1784 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/626-30.png
+-rw-r--r--   0        0        0     1569 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/626-31.png
+-rw-r--r--   0        0        0    58145 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/626-32.png
+-rw-r--r--   0        0        0     2639 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/628-10.png
+-rw-r--r--   0        0        0     3163 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/629-10.png
+-rw-r--r--   0        0        0     5889 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/629-20.png
+-rw-r--r--   0        0        0     4609 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/720.png
+-rw-r--r--   0        0        0     3377 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDRussia/.png
+-rw-r--r--   0        0        0     3377 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDSpain/.png
+-rw-r--r--   0        0        0     5275 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r1.png
+-rw-r--r--   0        0        0     6767 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r100.png
+-rw-r--r--   0        0        0     4672 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r101.png
+-rw-r--r--   0        0        0     7762 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r106.png
+-rw-r--r--   0        0        0     9177 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r107.png
+-rw-r--r--   0        0        0     4678 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r2.png
+-rw-r--r--   0        0        0     7978 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r205.png
+-rw-r--r--   0        0        0     7738 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r301.png
+-rw-r--r--   0        0        0     8609 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r305.png
+-rw-r--r--   0        0        0     7639 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r307.png
+-rw-r--r--   0        0        0     7220 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r308.png
+-rw-r--r--   0        0        0     9567 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDSpain/s13.png
+-rw-r--r--   0        0        0     3377 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/.png
+-rw-r--r--   0        0        0    11013 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/CW20-1.png
+-rw-r--r--   0        0        0     5884 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/D1-2.png
+-rw-r--r--   0        0        0     1961 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/M6-2aL.png
+-rw-r--r--   0        0        0    73748 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R1-3.png
+-rw-r--r--   0        0        0    51437 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R10-11.png
+-rw-r--r--   0        0        0    11452 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R10-7.png
+-rw-r--r--   0        0        0     2653 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R2-1.png
+-rw-r--r--   0        0        0     8495 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-1.png
+-rw-r--r--   0        0        0     8784 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-2.png
+-rw-r--r--   0        0        0    11718 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-27.png
+-rw-r--r--   0        0        0     9546 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-4.png
+-rw-r--r--   0        0        0     8410 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-5L.png
+-rw-r--r--   0        0        0     2705 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-5R.png
+-rw-r--r--   0        0        0     3191 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-8b.png
+-rw-r--r--   0        0        0     2702 2023-05-04 10:35:48.086736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R4-7.png
+-rw-r--r--   0        0        0     9439 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R5-1.png
+-rw-r--r--   0        0        0     2129 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R6-1L.png
+-rw-r--r--   0        0        0     2038 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R6-1R.png
+-rw-r--r--   0        0        0     7606 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R7-1.png
+-rw-r--r--   0        0        0     7189 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R7-107.png
+-rw-r--r--   0        0        0     2983 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R7-201a.png
+-rw-r--r--   0        0        0     7476 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R7-4.png
+-rw-r--r--   0        0        0     8741 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R7-8.png
+-rw-r--r--   0        0        0     7082 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R8-3.png
+-rw-r--r--   0        0        0     5076 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R8-3C.png
+-rw-r--r--   0        0        0     5343 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R8-3gP.png
+-rw-r--r--   0        0        0    14945 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/W1-3L.png
+-rw-r--r--   0        0        0     6551 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/W1-6L.png
+-rw-r--r--   0        0        0    10176 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/W11-2.png
+-rw-r--r--   0        0        0    10807 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/W3-3.png
+-rw-r--r--   0        0        0    16719 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/W4-2R.png
+-rw-r--r--   0        0        0     3377 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/.png
+-rw-r--r--   0        0        0     3513 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000-10.png
+-rw-r--r--   0        0        0     4708 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000-11.png
+-rw-r--r--   0        0        0     3627 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000-20.png
+-rw-r--r--   0        0        0     4340 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000-21.png
+-rw-r--r--   0        0        0     4898 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000-30.png
+-rw-r--r--   0        0        0     4788 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000-31.png
+-rw-r--r--   0        0        0     1312 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000.png
+-rw-r--r--   0        0        0     4181 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1001-30.png
+-rw-r--r--   0        0        0     4687 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1001-31.png
+-rw-r--r--   0        0        0     3091 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-10.png
+-rw-r--r--   0        0        0     2965 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-11.png
+-rw-r--r--   0        0        0     3006 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-12.png
+-rw-r--r--   0        0        0     3044 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-13.png
+-rw-r--r--   0        0        0     2957 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-14.png
+-rw-r--r--   0        0        0     2937 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-20.png
+-rw-r--r--   0        0        0     3005 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-21.png
+-rw-r--r--   0        0        0     2873 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-22.png
+-rw-r--r--   0        0        0     2872 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-23.png
+-rw-r--r--   0        0        0     2944 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-24.png
+-rw-r--r--   0        0        0     3147 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1004-30.png
+-rw-r--r--   0        0        0     3678 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1004-31.png
+-rw-r--r--   0        0        0     4872 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1004-32.png
+-rw-r--r--   0        0        0     2960 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1004-33.png
+-rw-r--r--   0        0        0     2939 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1004-34.png
+-rw-r--r--   0        0        0     2385 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1004-35.png
+-rw-r--r--   0        0        0     2985 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-30.png
+-rw-r--r--   0        0        0     2792 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-31.png
+-rw-r--r--   0        0        0     3037 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-32.png
+-rw-r--r--   0        0        0     4135 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-33.png
+-rw-r--r--   0        0        0     4419 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-34.png
+-rw-r--r--   0        0        0     4321 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-35.png
+-rw-r--r--   0        0        0     4095 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-36.png
+-rw-r--r--   0        0        0     3849 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-37.png
+-rw-r--r--   0        0        0     2317 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-38.png
+-rw-r--r--   0        0        0     3612 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-39.png
+-rw-r--r--   0        0        0     2188 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1007-31.png
+-rw-r--r--   0        0        0     6916 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/101.png
+-rw-r--r--   0        0        0     2147 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1010-10.png
+-rw-r--r--   0        0        0     2873 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1010-11.png
+-rw-r--r--   0        0        0     1827 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1010-12.png
+-rw-r--r--   0        0        0     2819 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1010-13.png
+-rw-r--r--   0        0        0     3029 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1010-14.png
+-rw-r--r--   0        0        0     1704 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-30.png
+-rw-r--r--   0        0        0     1418 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-31.png
+-rw-r--r--   0        0        0     3480 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-32.png
+-rw-r--r--   0        0        0     2572 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-33.png
+-rw-r--r--   0        0        0     3343 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-34.png
+-rw-r--r--   0        0        0     2933 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-35.png
+-rw-r--r--   0        0        0     2066 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-36.png
+-rw-r--r--   0        0        0     3120 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-37.png
+-rw-r--r--   0        0        0     2050 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-38.png
+-rw-r--r--   0        0        0     2112 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-50.png
+-rw-r--r--   0        0        0     2485 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-51.png
+-rw-r--r--   0        0        0     2339 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-52.png
+-rw-r--r--   0        0        0     2516 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-53.png
+-rw-r--r--   0        0        0     6735 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/102.png
+-rw-r--r--   0        0        0     5597 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1020-30.png
+-rw-r--r--   0        0        0     6417 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1022-10.png
+-rw-r--r--   0        0        0     5950 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1024-10.png
+-rw-r--r--   0        0        0     8026 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1026-36.png
+-rw-r--r--   0        0        0     8026 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1026-37.png
+-rw-r--r--   0        0        0     8026 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1026-38.png
+-rw-r--r--   0        0        0     8666 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/103-10.png
+-rw-r--r--   0        0        0     7320 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/103-20.png
+-rw-r--r--   0        0        0     4042 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1031-52.png
+-rw-r--r--   0        0        0     2650 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1040-30.png
+-rw-r--r--   0        0        0     3159 2023-05-04 10:35:48.090736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1048-12.png
+-rw-r--r--   0        0        0     5224 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1049-13.png
+-rw-r--r--   0        0        0     3680 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1052-31.png
+-rw-r--r--   0        0        0     4316 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1053-33.png
+-rw-r--r--   0        0        0     2901 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1053-34.png
+-rw-r--r--   0        0        0     3762 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1053-35.png
+-rw-r--r--   0        0        0    12644 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/108.png
+-rw-r--r--   0        0        0     8398 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/114.png
+-rw-r--r--   0        0        0     5977 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/120.png
+-rw-r--r--   0        0        0    13791 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/123.png
+-rw-r--r--   0        0        0     9003 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/124.png
+-rw-r--r--   0        0        0     8510 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/125.png
+-rw-r--r--   0        0        0     6937 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/131.png
+-rw-r--r--   0        0        0     9228 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/133-10.png
+-rw-r--r--   0        0        0     9320 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/133-20.png
+-rw-r--r--   0        0        0     8610 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/138.png
+-rw-r--r--   0        0        0    11307 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/142-10.png
+-rw-r--r--   0        0        0     6381 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/145-50.png
+-rw-r--r--   0        0        0    12735 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/201.png
+-rw-r--r--   0        0        0     5582 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/205.png
+-rw-r--r--   0        0        0     5067 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/206.png
+-rw-r--r--   0        0        0    13812 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/208.png
+-rw-r--r--   0        0        0     7132 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/209-10.png
+-rw-r--r--   0        0        0    11978 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/209-20.png
+-rw-r--r--   0        0        0     6924 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/209-30.png
+-rw-r--r--   0        0        0     7083 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/209.png
+-rw-r--r--   0        0        0     6937 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/211-10.png
+-rw-r--r--   0        0        0     6249 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/211-20.png
+-rw-r--r--   0        0        0     6920 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/211.png
+-rw-r--r--   0        0        0    16931 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/2113.png
+-rw-r--r--   0        0        0     7799 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/214-10.png
+-rw-r--r--   0        0        0     7333 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/214-30.png
+-rw-r--r--   0        0        0     7769 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/214.png
+-rw-r--r--   0        0        0    11470 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/215.png
+-rw-r--r--   0        0        0     5287 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/220-10.png
+-rw-r--r--   0        0        0     5359 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/220-20.png
+-rw-r--r--   0        0        0     8269 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/222-10.png
+-rw-r--r--   0        0        0     8297 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/222-20.png
+-rw-r--r--   0        0        0     4342 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/223.2-50.png
+-rw-r--r--   0        0        0     5405 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/223.2-51.png
+-rw-r--r--   0        0        0     4747 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/223.2.png
+-rw-r--r--   0        0        0     6167 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/224-50.png
+-rw-r--r--   0        0        0    17675 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/237.png
+-rw-r--r--   0        0        0    15792 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/239.png
+-rw-r--r--   0        0        0    15236 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/240.png
+-rw-r--r--   0        0        0    11564 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/242.1.png
+-rw-r--r--   0        0        0    10015 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/242.2.png
+-rw-r--r--   0        0        0    13431 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/244.1.png
+-rw-r--r--   0        0        0    10786 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/244.2.png
+-rw-r--r--   0        0        0    14243 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/245.png
+-rw-r--r--   0        0        0    12752 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/250.png
+-rw-r--r--   0        0        0     8903 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/251.png
+-rw-r--r--   0        0        0    14665 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/253.png
+-rw-r--r--   0        0        0    10381 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/254.png
+-rw-r--r--   0        0        0    16226 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/255.png
+-rw-r--r--   0        0        0    15152 2023-05-04 10:35:48.094736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/257-54.png
+-rw-r--r--   0        0        0     9437 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/259.png
+-rw-r--r--   0        0        0    18193 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/260.png
+-rw-r--r--   0        0        0    14767 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/261.png
+-rw-r--r--   0        0        0    13173 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/262.png
+-rw-r--r--   0        0        0    13739 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/264.png
+-rw-r--r--   0        0        0    13764 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/265.png
+-rw-r--r--   0        0        0    15436 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/266.png
+-rw-r--r--   0        0        0     6366 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/267.png
+-rw-r--r--   0        0        0     6424 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/270.1.png
+-rw-r--r--   0        0        0     6871 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/270.2.png
+-rw-r--r--   0        0        0    10406 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/272.png
+-rw-r--r--   0        0        0     4996 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/274.1.png
+-rw-r--r--   0        0        0     7607 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/274.2.png
+-rw-r--r--   0        0        0     7804 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/274.png
+-rw-r--r--   0        0        0     6449 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/275.png
+-rw-r--r--   0        0        0     8759 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/276.png
+-rw-r--r--   0        0        0     9330 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/277.png
+-rw-r--r--   0        0        0     6601 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/278.png
+-rw-r--r--   0        0        0     6835 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/279.png
+-rw-r--r--   0        0        0     8452 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/280.png
+-rw-r--r--   0        0        0     8087 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/281.png
+-rw-r--r--   0        0        0     6469 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/282.png
+-rw-r--r--   0        0        0    11770 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/283-10.png
+-rw-r--r--   0        0        0    12188 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/283-30.png
+-rw-r--r--   0        0        0    12156 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/286-30.png
+-rw-r--r--   0        0        0     8130 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/286.png
+-rw-r--r--   0        0        0     5908 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/301.png
+-rw-r--r--   0        0        0     3956 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/306.png
+-rw-r--r--   0        0        0     5671 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/308.png
+-rw-r--r--   0        0        0     5401 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/310.png
+-rw-r--r--   0        0        0     7203 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/311.png
+-rw-r--r--   0        0        0     2529 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/314-10.png
+-rw-r--r--   0        0        0     2569 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/314-20.png
+-rw-r--r--   0        0        0     2705 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/314-30.png
+-rw-r--r--   0        0        0     2317 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/314.png
+-rw-r--r--   0        0        0    10625 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/325.1.png
+-rw-r--r--   0        0        0    12383 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/325.2.png
+-rw-r--r--   0        0        0     5815 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/327.png
+-rw-r--r--   0        0        0     2544 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/328.png
+-rw-r--r--   0        0        0     2225 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/330.1.png
+-rw-r--r--   0        0        0     8637 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/330.2.png
+-rw-r--r--   0        0        0     3567 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/331.1.png
+-rw-r--r--   0        0        0     4310 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/331.2.png
+-rw-r--r--   0        0        0     3983 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/332.1.png
+-rw-r--r--   0        0        0     7257 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/332.png
+-rw-r--r--   0        0        0     4616 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/333-20.png
+-rw-r--r--   0        0        0     3350 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/333-21.png
+-rw-r--r--   0        0        0     2663 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/333-22.png
+-rw-r--r--   0        0        0     4496 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/333.png
+-rw-r--r--   0        0        0     5223 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/350.png
+-rw-r--r--   0        0        0     8456 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/354.png
+-rw-r--r--   0        0        0     5080 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/356.png
+-rw-r--r--   0        0        0     3049 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/357.png
+-rw-r--r--   0        0        0     1854 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/363.png
+-rw-r--r--   0        0        0     5740 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/365-51.png
+-rw-r--r--   0        0        0     3878 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/365-52.png
+-rw-r--r--   0        0        0     3515 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/365-60.png
+-rw-r--r--   0        0        0     1124 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/380.png
+-rw-r--r--   0        0        0     1588 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/381.png
+-rw-r--r--   0        0        0     2438 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/386.1.png
+-rw-r--r--   0        0        0     4572 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/386.2.png
+-rw-r--r--   0        0        0     4247 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/386.3.png
+-rw-r--r--   0        0        0    11292 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/406-50.png
+-rw-r--r--   0        0        0     2691 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/418-20.png
+-rw-r--r--   0        0        0     1852 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/419-20.png
+-rw-r--r--   0        0        0     2638 2023-05-04 10:35:48.098736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/430-20.png
+-rw-r--r--   0        0        0     1709 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/432-10.png
+-rw-r--r--   0        0        0     2271 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/432-20.png
+-rw-r--r--   0        0        0     6106 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/434-50.png
+-rw-r--r--   0        0        0     8563 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/434.png
+-rw-r--r--   0        0        0     3168 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/438.png
+-rw-r--r--   0        0        0     3361 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/439.png
+-rw-r--r--   0        0        0     5870 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/440.png
+-rw-r--r--   0        0        0     7617 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/448.png
+-rw-r--r--   0        0        0     9309 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/449.png
+-rw-r--r--   0        0        0     3520 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/450-50.png
+-rw-r--r--   0        0        0     4770 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/450-51.png
+-rw-r--r--   0        0        0     5217 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/450-52.png
+-rw-r--r--   0        0        0     4938 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/450-53.png
+-rw-r--r--   0        0        0     6058 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/450-54.png
+-rw-r--r--   0        0        0     6767 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/450-55.png
+-rw-r--r--   0        0        0     6353 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/453.png
+-rw-r--r--   0        0        0     2018 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/455.1-30.png
+-rw-r--r--   0        0        0     5836 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/458.png
+-rw-r--r--   0        0        0     3959 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/460-10.png
+-rw-r--r--   0        0        0     3966 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/460-12.png
+-rw-r--r--   0        0        0     1865 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/460-20.png
+-rw-r--r--   0        0        0     1728 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/460-21.png
+-rw-r--r--   0        0        0     1815 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/460-22.png
+-rw-r--r--   0        0        0     1775 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/460-30.png
+-rw-r--r--   0        0        0     3619 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/501-15.png
+-rw-r--r--   0        0        0     2458 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/501-16.png
+-rw-r--r--   0        0        0    45510 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/511-22.png
+-rw-r--r--   0        0        0     1985 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/521-30.png
+-rw-r--r--   0        0        0     2171 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/521-31.png
+-rw-r--r--   0        0        0     2388 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/521-32.png
+-rw-r--r--   0        0        0     2587 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/521-33.png
+-rw-r--r--   0        0        0     6797 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/525.png
+-rw-r--r--   0        0        0     2186 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/531-10.png
+-rw-r--r--   0        0        0     2097 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/531-20.png
+-rw-r--r--   0        0        0     1390 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/531-21.png
+-rw-r--r--   0        0        0     2239 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/533-22.png
+-rw-r--r--   0        0        0     1279 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/550-20.png
+-rw-r--r--   0        0        0     1180 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/600-30.png
+-rw-r--r--   0        0        0     1562 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/600-31.png
+-rw-r--r--   0        0        0      958 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/600-32.png
+-rw-r--r--   0        0        0      848 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/600-34.png
+-rw-r--r--   0        0        0      633 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/600-35.png
+-rw-r--r--   0        0        0      729 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/600-38.png
+-rw-r--r--   0        0        0     5294 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/605-10.png
+-rw-r--r--   0        0        0     2361 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/605-11.png
+-rw-r--r--   0        0        0     5294 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/605-20.png
+-rw-r--r--   0        0        0    16340 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/605-21.png
+-rw-r--r--   0        0        0    10798 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/605-31.png
+-rw-r--r--   0        0        0     3546 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-10.png
+-rw-r--r--   0        0        0      960 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-11.png
+-rw-r--r--   0        0        0     3499 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-12.png
+-rw-r--r--   0        0        0     4442 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-13.png
+-rw-r--r--   0        0        0     3518 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-20.png
+-rw-r--r--   0        0        0      952 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-21.png
+-rw-r--r--   0        0        0     3426 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-22.png
+-rw-r--r--   0        0        0     4550 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-23.png
+-rw-r--r--   0        0        0     3053 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/626-10.png
+-rw-r--r--   0        0        0     3254 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/626-20.png
+-rw-r--r--   0        0        0     1784 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/626-30.png
+-rw-r--r--   0        0        0     1569 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/626-31.png
+-rw-r--r--   0        0        0    58145 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/626-32.png
+-rw-r--r--   0        0        0     2639 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/628-10.png
+-rw-r--r--   0        0        0     3163 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/629-10.png
+-rw-r--r--   0        0        0     5889 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/629-20.png
+-rw-r--r--   0        0        0     4609 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/720.png
+-rw-r--r--   0        0        0     5312 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/traffic_light_state_green.png
+-rw-r--r--   0        0        0     5157 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/traffic_light_state_inactive.png
+-rw-r--r--   0        0        0     4943 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/traffic_light_state_red.png
+-rw-r--r--   0        0        0     4872 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/traffic_light_state_redYellow.png
+-rw-r--r--   0        0        0     5093 2023-05-04 10:35:48.102736 commonroad_io-2023.2/commonroad/visualization/traffic_signs/traffic_light_state_yellow.png
+-rw-r--r--   0        0        0    11888 2023-06-26 01:03:15.674438 commonroad_io-2023.2/commonroad/visualization/util.py
+-rw-r--r--   0        0        0     2148 2023-06-26 05:26:51.184356 commonroad_io-2023.2/pyproject.toml
+-rw-r--r--   0        0        0    10304 1970-01-01 00:00:00.000000 commonroad_io-2023.2/PKG-INFO
```

### Comparing `commonroad_io-2023.1/LICENSE.txt` & `commonroad_io-2023.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/README.md` & `commonroad_io-2023.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 [![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
 [![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)  
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/commonroad-io.svg)](https://pypi.python.org/pypi/commonroad-io/)  
 [![PyPI version fury.io](https://badge.fury.io/py/commonroad-io.svg)](https://pypi.python.org/pypi/commonroad-io/)
 [![PyPI download month](https://img.shields.io/pypi/dm/commonroad-io.svg?label=PyPI%20downloads)](https://pypi.python.org/pypi/commonroad-io/) 
 [![PyPI download week](https://img.shields.io/pypi/dw/commonroad-io.svg?label=PyPI%20downloads)](https://pypi.python.org/pypi/commonroad-io/)   
 [![PyPI license](https://img.shields.io/pypi/l/commonroad-io.svg)](https://pypi.python.org/pypi/commonroad-io/)
-[![Documentation Status](https://readthedocs.org/projects/commonroad-io/badge/?version=latest)](http://commonroad-io.readthedocs.io/?badge=latest) 
 
 
 Numerical experiments for motion planning of road vehicles require numerous ingredients: vehicle dynamics, 
 a road network, static obstacles, dynamic obstacles and their movement over time, goal regions, a cost function, etc. 
 Providing a description of the numerical experiment precise enough to reproduce it might require several pages of 
 information. 
 Thus, only key aspects are typically described in scientific publications, making it impossible to reproduce 
@@ -29,15 +28,15 @@
 # commonroad-io
 
 The commonroad-io package provides methods to read, write, and visualize CommonRoad scenarios and planning problems. Furthermore, it can be used as a framework for implementing motion planning algorithms to solve CommonRoad Benchmarks and is the basis for other tools of the CommonRoad Framework.
 With commonroad-io, those solutions can be written to xml-files for uploading them on [commonroad.in.tum.de](https://commonroad.in.tum.de/).
 
 commonroad-io 2023.1 is compatible with CommonRoad scenarios in version 2020a and supports reading 2018b scenarios.
 
-The software is written in Python and tested on Linux for the Python 3.7, 3.8, 3.9, 3.10, and 3.11.
+The software is written in Python and tested on Linux for the Python 3.8, 3.9, 3.10, and 3.11.
 
 
 ## Documentation
 
 The full documentation of the API and introducing examples can be found under [commonroad.in.tum.de](https://commonroad-io.readthedocs.io/en/latest/).
 
 For getting started, we recommend our [tutorials](https://commonroad.in.tum.de/commonroad-io).
@@ -77,14 +76,42 @@
 Alternatively, clone from our gitlab repository::
 
 	git clone https://gitlab.lrz.de/tum-cps/commonroad_io.git
 
 and add the folder commonroad-io to your Python environment.
 
 ## Changelog
+Compared to version 2023.1, the following features have been added or changed:
+
+### Added
+- Area for modelling drivable areas which cannot be represented by lanelets
+- New weather and time of day options
+- Allow file reader to determine format based on suffix 
+
+### Fixed
+
+- Visualization of all traffic signs by setting `show_traffic_signs = None` in draw parameters
+- Validity functions to support z-axis
+- Unreferenced traffic signs for lanelet networks filtered by lanelet type
+
+### Changed
+
+- Visualization of direction arrow of narrow lanelets
+- Traffic light cycle optional
+- Traffic light in separate python file
+- Allow file reader to determine format based on suffix 
+- Broaden types allowed as file names 
+- Open files safely by using a context manager 
+- Use correct suffix when inferring filename from scenario id
+
+### Removed
+
+- function get_default_cycle for traffic lights
+- support for Python 3.7
+
 Compared to version 2022.3, the following features have been added or changed:
 
 ### Added
 - Support for shapely>=2.0.0
 
 ### Fixed
 
@@ -93,14 +120,15 @@
 - Default plot limits for focused obstacle
 - Use dt from scenario as default for video creation
 - Apply axis visible-option also for video creation
 - Protobuf FileReader marking road network related IDs as used
 - State attribute comparison
 
 ### Changed
+>>>>>>> README.md
 
 - Name of SIDEWALK and BUSLANE traffic signs to PEDESTRIAN_SIDEWALK and BUS_LANE
 - Packaging and dependency management using poetry
 
 
 ## Authors
 Contribution (in alphabetic order by last name): Yannick Ballnath, Behtarin Ferdousi, Luis Gressenbuch, Moritz Klischat,
```

### Comparing `commonroad_io-2023.1/commonroad/common/file_reader.py` & `commonroad_io-2023.2/commonroad/common/file_reader.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,37 @@
-from typing import Tuple
+from pathlib import Path
+from typing import Tuple, Optional
 
-from commonroad.common.file_writer import FileFormat
+from commonroad.common.util import FileFormat, Path_T
 from commonroad.common.reader.file_reader_protobuf import ProtobufFileReader
 from commonroad.common.reader.file_reader_xml import XMLFileReader
 from commonroad.planning.planning_problem import PlanningProblemSet
 from commonroad.scenario.lanelet import LaneletNetwork
 from commonroad.scenario.scenario import Scenario
 from commonroad.scenario.traffic_sign import *
 
 
 class CommonRoadFileReader:
     """
     Reads CommonRoad files in XML or protobuf format. The corresponding stored scenario and planning problem set
     are created by the reader.
     """
-    def __init__(self, filename: str, file_format: FileFormat = FileFormat.XML):
+    def __init__(self, filename: Path_T, file_format: Optional[FileFormat] = None):
         """
         Initializes the FileReader for CommonRoad files.
 
         :param filename: Name of file
-        :param file_format: Format of file
+        :param file_format: Format of file. If None, inferred from file suffix.
         :return:
         """
         self._file_reader = None
+
+        if file_format is None:
+            file_format = FileFormat(Path(filename).suffix)
+
         if file_format == FileFormat.XML:
             self._file_reader = XMLFileReader(filename)
         elif file_format == FileFormat.PROTOBUF:
             self._file_reader = ProtobufFileReader(filename)
 
     def open(self, lanelet_assignment: bool = False) -> Tuple[Scenario, PlanningProblemSet]:
         """
```

### Comparing `commonroad_io-2023.1/commonroad/common/file_writer.py` & `commonroad_io-2023.2/commonroad/common/file_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,17 @@
-import enum
 from typing import Union, Set
 
+from commonroad.common.util import FileFormat
 from commonroad.common.writer.file_writer_interface import OverwriteExistingFile
 from commonroad.common.writer.file_writer_protobuf import ProtobufFileWriter
 from commonroad.common.writer.file_writer_xml import XMLFileWriter
 from commonroad.planning.planning_problem import PlanningProblemSet
 from commonroad.scenario.scenario import Scenario, Tag, Location
 
 
-class FileFormat(enum.Enum):
-    """
-    Specifies the format of file.
-    """
-
-    XML = 0
-    PROTOBUF = 1
-
-
 class CommonRoadFileWriter:
     """
     Writes CommonRoad files in XML or protobuf format. The corresponding scenario and planning problem set
     are stored by the writer.
     """
 
     def __init__(self, scenario: Scenario, planning_problem_set: PlanningProblemSet, author: str = None,
@@ -35,14 +26,15 @@
         :param affiliation: Affiliation of author
         :param source: Source of dataset, e.g., database, handcrafted, etc.
         :param tags: Keywords describing the scenario
         :param decimal_precision: Number of decimal places used when writing float values
         :param file_format: Format of file
         :return:
         """
+        self._file_format = file_format
         self._file_writer = None
         if file_format == FileFormat.XML:
             self._file_writer = XMLFileWriter(scenario, planning_problem_set, author, affiliation,
                                               source, tags, location, decimal_precision)
         elif file_format == FileFormat.PROTOBUF:
             self._file_writer = ProtobufFileWriter(scenario, planning_problem_set, author, affiliation,
                                                    source, tags, location, decimal_precision)
```

### Comparing `commonroad_io-2023.1/commonroad/common/reader/file_reader_interface.py` & `commonroad_io-2023.2/commonroad/common/reader/file_reader_interface.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from abc import ABC, abstractmethod
 from typing import Tuple
 
+from commonroad.common.util import Path_T
 from commonroad.planning.planning_problem import PlanningProblemSet
 from commonroad.scenario.lanelet import LaneletNetwork
 from commonroad.scenario.scenario import Scenario
 
 
 class FileReader(ABC):
     """
     Interface for reading CommonRoad files in a specific format.
     """
 
-    def __init__(self, filename: str):
+    def __init__(self, filename: Path_T):
         self._filename = filename
 
     @abstractmethod
     def open(self, lanelet_assignment: bool = False) -> Tuple[Scenario, PlanningProblemSet]:
         pass
 
     @abstractmethod
```

### Comparing `commonroad_io-2023.1/commonroad/common/reader/file_reader_protobuf.py` & `commonroad_io-2023.2/commonroad/common/reader/file_reader_protobuf.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,32 +2,34 @@
 import logging
 import re
 from typing import Tuple, List, Set, Union, Dict
 
 import numpy as np
 
 from commonroad.common.reader.file_reader_interface import FileReader
-from commonroad.common.util import Interval, AngleInterval
+from commonroad.common.util import Interval, AngleInterval, Path_T, Time
 from commonroad.geometry.shape import Rectangle, Circle, Polygon, Shape, ShapeGroup
 from commonroad.planning.goal import GoalRegion
 from commonroad.planning.planning_problem import PlanningProblemSet, PlanningProblem
 from commonroad.prediction.prediction import Occupancy, TrajectoryPrediction, SetBasedPrediction
 from commonroad.scenario.intersection import Intersection, IntersectionIncomingElement
-from commonroad.scenario.lanelet import LaneletNetwork, Lanelet, StopLine, LineMarking, LaneletType, RoadUser
+from commonroad.scenario.lanelet import LaneletNetwork, Lanelet
+from commonroad.common.common_lanelet import RoadUser, StopLine, LineMarking, LaneletType
 from commonroad.scenario.obstacle import StaticObstacle, DynamicObstacle, EnvironmentObstacle, PhantomObstacle, \
     SignalState, ObstacleType
 from commonroad.scenario.scenario import Scenario, ScenarioID, Tag, GeoTransformation, Location, Environment, \
     TimeOfDay, \
-    Weather, Underground, Time
+    Weather, Underground
 from commonroad.scenario.state import InitialState, TraceState, CustomState, SpecificStateClasses
 from commonroad.scenario.traffic_sign import TrafficSignElement, TrafficSignIDGermany, TrafficSignIDZamunda, \
     TrafficSignIDUsa, TrafficSignIDChina, TrafficSignIDSpain, TrafficSignIDRussia, TrafficSignIDArgentina, \
     TrafficSignIDBelgium, TrafficSignIDFrance, TrafficSignIDGreece, TrafficSignIDCroatia, TrafficSignIDItaly, \
-    TrafficSignIDPuertoRico, TrafficSign, TrafficLight, TrafficLightCycleElement, TrafficLightDirection, \
-    TrafficLightState
+    TrafficSignIDPuertoRico, TrafficSign
+from commonroad.scenario.traffic_light import TrafficLightState, TrafficLightDirection, \
+    TrafficLightCycleElement,  TrafficLight, TrafficLightCycle
 from commonroad.scenario.trajectory import Trajectory
 from commonroad.scenario_definition.protobuf_format.generated_scripts import commonroad_pb2, util_pb2, \
     phantom_obstacle_pb2
 from commonroad.scenario_definition.protobuf_format.generated_scripts import lanelet_pb2, planning_problem_pb2, \
     traffic_sign_pb2, scenario_tags_pb2, environment_obstacle_pb2, obstacle_pb2, intersection_pb2, \
     dynamic_obstacle_pb2, \
     static_obstacle_pb2, traffic_light_pb2, location_pb2
@@ -36,39 +38,39 @@
 
 
 class ProtobufFileReader(FileReader):
     """
     Reader for CommonRoad file stored in protobuf format.
     """
 
-    def __init__(self, filename: str):
+    def __init__(self, filename: Path_T):
         super().__init__(filename)
 
     def open(self, lanelet_assignment: bool = False) -> Tuple[Scenario, PlanningProblemSet]:
         """
         Reads a CommonRoad file in protobuf format.
 
         :param lanelet_assignment: Activates calculation of lanelets occupied by obstacles
         :return: Scenario and planning problems
         """
-        file = open(self._filename, "rb")
-        commonroad_msg = commonroad_pb2.CommonRoad()
-        commonroad_msg.ParseFromString(file.read())
+        with open(self._filename, "rb") as file:
+            commonroad_msg = commonroad_pb2.CommonRoad()
+            commonroad_msg.ParseFromString(file.read())
 
         return CommonRoadFactory.create_from_message(commonroad_msg, lanelet_assignment)
 
     def open_lanelet_network(self) -> LaneletNetwork:
         """
         Reads a CommonRoad file in protobuf format.
 
         :return: Lanelet network
         """
-        file = open(self._filename, "rb")
-        commonroad_msg = commonroad_pb2.CommonRoad()
-        commonroad_msg.ParseFromString(file.read())
+        with open(self._filename, "rb") as file:
+            commonroad_msg = commonroad_pb2.CommonRoad()
+            commonroad_msg.ParseFromString(file.read())
 
         scenario, _ = CommonRoadFactory.create_from_message(commonroad_msg, False)
 
         return scenario.lanelet_network
 
 
 class CommonRoadFactory:
@@ -341,23 +343,17 @@
         traffic_sign_id = traffic_sign_msg.traffic_sign_id
 
         traffic_sign_elements = list()
         for traffic_sign_element_msg in traffic_sign_msg.traffic_sign_elements:
             traffic_sign_element = TrafficSignElementFactory.create_from_message(traffic_sign_element_msg)
             traffic_sign_elements.append(traffic_sign_element)
 
-        first_occurrences = set()
-        for first_occurrence in traffic_sign_msg.first_occurrences:
-            first_occurrences.add(first_occurrence)
-
-        traffic_sign = TrafficSign(traffic_sign_id, traffic_sign_elements, first_occurrences)
-
-        if traffic_sign_msg.HasField('position'):
-            point = PointFactory.create_from_message(traffic_sign_msg.position)
-            traffic_sign.position = point
+        point = PointFactory.create_from_message(traffic_sign_msg.position)
+
+        traffic_sign = TrafficSign(traffic_sign_id, traffic_sign_elements, set(), point)
 
         if traffic_sign_msg.HasField('virtual'):
             traffic_sign.virtual = traffic_sign_msg.virtual
 
         return traffic_sign
 
 
@@ -420,22 +416,27 @@
         traffic_light_id = traffic_light_msg.traffic_light_id
 
         cycle_elements = list()
         for cycle_element_msg in traffic_light_msg.cycle_elements:
             cycle_element = CycleElementFactory.create_from_message(cycle_element_msg)
             cycle_elements.append(cycle_element)
 
-        traffic_light = TrafficLight(traffic_light_id, cycle_elements)
-
-        if traffic_light_msg.HasField('position'):
-            point = PointFactory.create_from_message(traffic_light_msg.position)
-            traffic_light.position = point
+        point = PointFactory.create_from_message(traffic_light_msg.position)
 
+        traffic_light_cycle = TrafficLightCycle(cycle_elements)
         if traffic_light_msg.HasField('time_offset'):
-            traffic_light.time_offset = traffic_light_msg.time_offset
+            traffic_light_cycle.time_offset = traffic_light_msg.time_offset
+
+        # extracting the color list from the traffic light cycle
+        color = []
+        if len(cycle_elements) > 0:
+            for element in cycle_elements:
+                color.append(element.state)
+
+        traffic_light = TrafficLight(traffic_light_id, point, traffic_light_cycle, color)
 
         if traffic_light_msg.HasField('direction'):
             traffic_light.direction = TrafficLightDirection[
                 traffic_light_pb2.TrafficLightDirectionEnum.TrafficLightDirection.Name(traffic_light_msg.direction)]
 
         if traffic_light_msg.HasField('active'):
             traffic_light.active = traffic_light_msg.active
```

### Comparing `commonroad_io-2023.1/commonroad/common/reader/file_reader_xml.py` & `commonroad_io-2023.2/commonroad/common/reader/file_reader_xml.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 from abc import ABC
 from collections import defaultdict
 from typing import Dict, Tuple
 from xml.etree import ElementTree
 
 from commonroad import SUPPORTED_COMMONROAD_VERSIONS
 from commonroad.common.reader.file_reader_interface import FileReader
-from commonroad.common.util import Interval, AngleInterval
+from commonroad.common.util import Interval, AngleInterval, Path_T, Time
 from commonroad.geometry.shape import Rectangle, Circle, Polygon, ShapeGroup, Shape
 from commonroad.planning.goal import GoalRegion
 from commonroad.planning.planning_problem import PlanningProblemSet, PlanningProblem
 from commonroad.prediction.prediction import Occupancy, SetBasedPrediction, TrajectoryPrediction
 from commonroad.scenario.intersection import Intersection, IntersectionIncomingElement
-from commonroad.scenario.lanelet import Lanelet, LaneletNetwork, LineMarking, LaneletType, RoadUser, StopLine
+from commonroad.scenario.lanelet import Lanelet, LaneletNetwork
+from commonroad.common.common_lanelet import RoadUser, StopLine, LineMarking, LaneletType
 from commonroad.scenario.obstacle import ObstacleType, StaticObstacle, DynamicObstacle, Obstacle, EnvironmentObstacle, \
     SignalState, PhantomObstacle
-from commonroad.scenario.scenario import Scenario, Tag, GeoTransformation, Location, Environment, Time, TimeOfDay, \
+from commonroad.scenario.scenario import Scenario, Tag, GeoTransformation, Location, Environment, TimeOfDay, \
     Weather, Underground, ScenarioID
 from commonroad.scenario.state import InitialState, TraceState, CustomState, SpecificStateClasses
 from commonroad.scenario.traffic_sign import *
+from commonroad.scenario.traffic_light import *
 from commonroad.scenario.trajectory import Trajectory
 
 logger = logging.getLogger(__name__)
 
 
 def read_value_exact_or_interval(xml_node: ElementTree.Element)\
         -> Union[float, Interval]:
@@ -53,15 +55,15 @@
 
 
 class XMLFileReader(FileReader):
     """ Class which reads CommonRoad XML-files. The XML-files are composed of
     (1) a formal representation of the road network,
     (2) static and dynamic obstacles,
     (3) the planning problem of the ego vehicle(s). """
-    def __init__(self, filename: str):
+    def __init__(self, filename: Path_T):
         """
         :param filename: full path + filename of the CommonRoad XML-file,
         """
         super().__init__(filename)
 
         self._tree = None
         self._dt = None
@@ -802,15 +804,15 @@
                 virtual = False
             else:
                 raise ValueError()
         else:
             virtual = False
 
         return TrafficSign(traffic_sign_id=traffic_sign_id, position=position,
-                           first_occurrence=first_traffic_sign_occurence[traffic_sign_id],
+                           first_occurrence=set(),
                            traffic_sign_elements=traffic_sign_elements, virtual=virtual)
 
 
 class TrafficSignElementFactory:
     """ Class to create an object of class TrafficSignElement from an XML element."""
     @classmethod
     def create_from_xml_node(cls, xml_node: ElementTree.Element,
@@ -926,41 +928,49 @@
             elif xml_node.find('direction').text == "all":
                 direction = TrafficLightDirection.ALL
             else:
                 direction = TrafficLightDirection.ALL
         else:
             direction = TrafficLightDirection.ALL
 
-        traffic_ligth_cycle, time_offset = TrafficLightCycleFactory.create_from_xml_node(xml_node.find('cycle'))
+        traffic_light_cycles, time_offset = TrafficLightCycleFactory.create_from_xml_node(xml_node.find('cycle'))
 
-        return TrafficLight(traffic_light_id=traffic_light_id, cycle=traffic_ligth_cycle, position=position,
-                            direction=direction, active=active, time_offset=time_offset)
+        traffic_light_cycle = TrafficLightCycle(traffic_light_cycles, time_offset)
+
+        # extracting the color list from the traffic light cycle
+        color = []
+        if len(traffic_light_cycles) > 0:
+            for cycle_element in traffic_light_cycles:
+                color.append(cycle_element.state)
+
+        return TrafficLight(traffic_light_id=traffic_light_id, position=position,
+                            traffic_light_cycle=traffic_light_cycle, color=color, direction=direction, active=active)
 
 
 class TrafficLightCycleFactory:
     """ Class to create an object of class TrafficLightCycleElement from an XML element."""
     @classmethod
     def create_from_xml_node(cls, xml_node: ElementTree.Element) -> Tuple[List[TrafficLightCycleElement], int]:
         """
         :param xml_node: XML element
         :return: list of objects of class TrafficLightCycleElement according to the CommonRoad specification.
         """
-        traffic_ligth_cycle_elements = []
+        traffic_light_cycle_elements = []
         for cycleElement in xml_node.findall('cycleElement'):
             state = cycleElement.find('color').text
             duration = int(cycleElement.find('duration').text)
-            traffic_ligth_cycle_elements.append(TrafficLightCycleElement(state=TrafficLightState(state),
+            traffic_light_cycle_elements.append(TrafficLightCycleElement(state=TrafficLightState(state),
                                                                          duration=duration))
 
         if xml_node.find('timeOffset') is not None:
             time_offset = int(xml_node.find('timeOffset').text)
         else:
             time_offset = 0
 
-        return traffic_ligth_cycle_elements, time_offset
+        return traffic_light_cycle_elements, time_offset
 
 
 class IntersectionFactory:
     """ Class to create an object of class Intersection from an XML element."""
     @classmethod
     def create_from_xml_node(cls, xml_node: ElementTree.Element) -> Intersection:
         """
```

### Comparing `commonroad_io-2023.1/commonroad/common/solution.py` & `commonroad_io-2023.2/commonroad/common/solution.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,28 +147,20 @@
     KST = 'kstState'
     PM = 'pmState'
     Input = 'input'
     PMInput = 'pmInput'
 
     @property
     def fields(self) -> List[str]:
-        """
-        Returns the state fields for the state type.
-
-        :return: State fields as list
-        """
+        """ Returns the state fields for the state type. """
         return StateFields[self.name].value
 
     @property
     def xml_fields(self) -> List[str]:
-        """
-        Returns the xml state fields for the state type.
-
-        :return: XML names of the state fields as list
-        """
+        """ Returns the xml state fields for the state type. """
         return XMLStateFields[self.name].value
 
     @classmethod
     def get_state_type(cls, state: TraceState, desired_vehicle_model: VehicleModel = None) -> 'StateType':
         """
         Returns the corresponding StateType for the given State object by matching State object's attributes
         to the state fields.
@@ -231,19 +223,15 @@
     KST = 'kstTrajectory'
     PM = 'pmTrajectory'
     Input = 'inputVector'
     PMInput = 'pmInputVector'
 
     @property
     def state_type(self) -> StateType:
-        """
-        Returns the StateType corresponding to the TrajectoryType
-
-        :return: StateType
-        """
+        """ Returns the StateType corresponding to the TrajectoryType. """
         return StateType[self.name]
 
     @classmethod
     def get_trajectory_type(cls, trajectory: Trajectory,
                             desired_vehicle_model: VehicleModel = None) -> 'TrajectoryType':
         """
         Returns the corresponding TrajectoryType for the given Trajectory object based on the StateType of its states.
@@ -388,16 +376,14 @@
         """
         Returns the vehicle id as string.
 
         Example:
             VehicleModel = PM
             VehicleType = FORD_ESCORT
             Vehicle ID = PM1
-
-        :return: Vehicle model ID
         """
         return self.vehicle_model.name + str(self.vehicle_type.value)
 
     @property
     def cost_id(self) -> str:
         """
         Returns cost function id as str.
@@ -466,16 +452,14 @@
             1st CostFunction = JB1
             2nd VehicleModel = PM
             2nd VehicleType = VW_VANAGON
             2nd CostFunction = SA1
             Version = 2020a
 
             Benchmark ID = [PM1,PM3]:[JB1,SA1]:TEST:2020a
-
-        :return: Benchmark ID
         """
         vehicle_ids = self.vehicle_ids
         cost_ids = self.cost_ids
         vehicles_str = vehicle_ids[0] if len(vehicle_ids) == 1 else '[%s]' % ','.join(vehicle_ids)
         costs_str = cost_ids[0] if len(cost_ids) == 1 else '[%s]' % ','.join(cost_ids)
         return '%s:%s:%s:%s' % (vehicles_str, costs_str, str(self.scenario_id), self.scenario_id.scenario_version)
 
@@ -500,31 +484,27 @@
         Returns the list of cost ids of all PlanningProblemSolutions of the Solution
 
         Example:
             1st PlanningProblemSolution Cost ID = JB1
             2nd PlanningProblemSolution Cost ID = SA1
 
             Cost IDS = [JB1, SA1]
-
-        :return: List of cost function IDs
         """
         return [pp_solution.cost_id for pp_solution in self.planning_problem_solutions]
 
     @property
     def planning_problem_ids(self) -> List[int]:
         """
         Returns the list of planning problem ids of all PlanningProblemSolutions of the Solution
 
         Example:
             1st PlanningProblemSolution planning_problem_id = 0
             2nd PlanningProblemSolution planning_problem_id = 1
 
             planning_problem_ids = [0, 1]
-
-        :return: List of planning problem ids
         """
         return [pp_solution.planning_problem_id for pp_solution in self.planning_problem_solutions]
 
     @property
     def trajectory_types(self) -> List[TrajectoryType]:
         """
         Returns the list of trajectory types of all PlanningProblemSolutions of the Solution
@@ -539,16 +519,14 @@
         """
         return [pp_solution.trajectory_type for pp_solution in self.planning_problem_solutions]
 
     @property
     def computation_time(self) -> Union[None, float]:
         """
         Return the computation time [s] for the trajectory.
-
-        :return:
         """
         return self._computation_time
 
     @computation_time.setter
     def computation_time(self, computation_time):
         if computation_time is not None:
             assert is_real_number(computation_time), "<Solution> computation_time provided as type {}," \
@@ -557,15 +535,14 @@
             assert is_positive(computation_time), "<Solution> computation_time needs to be positive!"\
                 .format(type(computation_time))
         self._computation_time = computation_time
 
     def create_dynamic_obstacle(self) -> Dict[int, DynamicObstacle]:
         """
         Creates dynamic obstacle(s) from solution(s) for every planning problem.
-        :return:
         """
         obs = {}
         for pp_id, solution in self._planning_problem_solutions.items():
             shape = Rectangle(length=vehicle_parameters[solution.vehicle_type].l,
                               width=vehicle_parameters[solution.vehicle_type].w)
             trajectory = Trajectory(initial_time_step=solution.trajectory.initial_time_step + 1,
                                     state_list=solution.trajectory.state_list[1:])
```

### Comparing `commonroad_io-2023.1/commonroad/common/util.py` & `commonroad_io-2023.2/commonroad/common/util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,22 @@
+import enum
+
+import enum
+from pathlib import Path
+
 import numpy as np
 import math
 from scipy.spatial.transform.rotation import Rotation
 from scipy.spatial.transform import Slerp
 from typing import Tuple
 from commonroad.common import validity
 from commonroad.common.validity import *
 
+Path_T = Union[str, bytes, Path]
+
 
 def interpolate_angle(x: Union[float, np.array], xp: np.array, fp: np.array, degrees=False):
     """
     :param x: The x-coordinates at which to evaluate the interpolated values.
     :param xp: The x-coordinates of the data points.
     :param fp: The y-coordinates (angles) of the data points, same length as xp.
     :param degrees: True if the input and returned angles are in degrees
@@ -219,7 +226,96 @@
         return 0 <= start_diff <= interval_diff and 0 <= end_diff <= interval_diff
 
     def __contains__(self, value: Union[int, float]):
         interval_diff = vectorized_angle_difference(self.end, self.start)
         assert interval_diff >= 0
         diff = vectorized_angle_difference(value, self.start)
         return 0 <= diff <= interval_diff
+
+
+class FileFormat(enum.Enum):
+    """
+    Specifies the format of file.
+    """
+    XML = ".xml"
+    PROTOBUF = ".pb"
+
+
+class Time:
+    """
+    Class which describes the fictive time when a scenario starts.
+    """
+
+    def __init__(self, hours: int, minutes: int, day: int = None, month: int = None, year: int = None):
+        """
+        Constructor of a time object
+
+        :param hours: hours at start of scenario (0-24)
+        :param minutes: minutes at start of scenario (0-60)
+        :param day: day at start of scenario (1-31)
+        :param month: month at start of scenario (1-12)
+        :param year: year at start of scenario
+        """
+        self._hours = hours
+        self._minutes = minutes
+        self._day = day
+        self._month = month
+        self._year = year
+
+    def __eq__(self, other):
+        if not isinstance(other, Time):
+            return False
+
+        return self._hours == other.hours and self._minutes == other.minutes and self._day == other.day and \
+            self._month == other.month and self._year == other.year
+
+    def __str__(self):
+        return f"Year {self._year}, month {self._month}, day {self._day}, hour {self._hours}, minute {self.minutes}"
+
+    def __hash__(self):
+        return hash((self._hours, self._minutes, self._day, self._month, self._year))
+
+    @property
+    def hours(self) -> int:
+        """ Hours at start of scenario (0-24)"""
+        return self._hours
+
+    @hours.setter
+    def hours(self, hours: int):
+        self._hours = hours
+
+    @property
+    def minutes(self) -> int:
+        """ Minutes at start of scenario (0-60)"""
+        return self._minutes
+
+    @minutes.setter
+    def minutes(self, minutes: int):
+        self._minutes = minutes
+
+    @property
+    def day(self) -> Union[None, int]:
+        """ Day at start of scenario (1-31)"""
+        return self._day
+
+    @day.setter
+    def day(self, day: Union[None, int]):
+        self._day = day
+
+    @property
+    def month(self) -> Union[None, int]:
+        """ Month at start of scenario (1-12)"""
+        return self._month
+
+    @month.setter
+    def month(self, month: Union[None, int]):
+        self._month = month
+
+    @property
+    def year(self) -> Union[None, int]:
+        """ Year at start of scenario"""
+        return self._year
+
+    @year.setter
+    def year(self, year: Union[None, int]):
+        self._year = year
+
```

### Comparing `commonroad_io-2023.1/commonroad/common/validity.py` & `commonroad_io-2023.2/commonroad/common/validity.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     return isinstance(n, ValidTypes.NUMBERS)
 
 
 def is_integer_number(n: int) -> bool:
     """
     Checks if a provided variable is an integer number
     :param n: The number to check
-    :return: True if the provided variable is a integer number, False otherwise
+    :return: True if the provided variable is an integer number, False otherwise
     """
     return isinstance(n, ValidTypes.INT_NUMBERS)
 
 
 def is_natural_number(n: int) -> bool:
     """
     Checks if a provided variable is a natural number
@@ -107,15 +107,15 @@
 def is_list_of_numbers(x: list, length=None):
     """
     Checks if a provided variable is a list of numbers
     :param x: The variable to check
     :param length: optional parameter which tests if the list is a list of specified length
     :return: True if the specified variable is a list of numbers
     """
-    return isinstance(x, list) and is_real_number_vector(npy.array(x), length)
+    return isinstance(x, ValidTypes.LISTS) and is_real_number_vector(npy.array(x), length)
 
 
 def is_list_of_integer_numbers(x: list, length=None):
     """
     Checks if a provided variable is a list of numbers
     :param x: The variable to check
     :param length: optional parameter which tests if the list is a list of specified length
@@ -206,54 +206,61 @@
     :return: True if the orientation is a valid orientation (radian), False otherwise
     """
     return is_in_interval(theta, -TWO_PI, TWO_PI)
 
 
 def is_valid_polyline(polyline: npy.ndarray, length=None):
     """
-    Checks if a provided polyline is a valid polyline, i.e. it is a list of points (xi,yi)^T.
-    The list must have a shape of (2,n), resulting in [[x0,x1,...,xn],[y0,y1,...,yn]].
+    Checks if a provided polyline is a valid polyline, i.e. it is a list of points (xi,yi)^T or (xi,yi,zi)^T.
+    The list must have a shape of (n,2) or (n,3), resulting in [[x0, y0], [x1, y1], ...] or
+    [[x0, y0, z0], [x1, y1, z1], ...]
     By providing the optional parameter length, it is checked whether the provided has the desired length.
     :param polyline: The polyline to check
     :param length: The assumed length of the polyline
     :return: True if the polyline is a valid polyline, False otherwise
     """
     if length is not None:
         assert is_valid_length(length)
 
     return isinstance(polyline, ValidTypes.ARRAY) and len(polyline) >= 2 and all(
-            is_real_number_vector(elem, 2) for elem in polyline) and (
+            #  it is not possible (ValueError) to create a polyline (np.array) with different sized vectors,
+            #  so all the polyline points will either be 2d (without z-coordinate) or 3d (with z-coordinate)
+            is_real_number_vector(elem, 2) or is_real_number_vector(elem, 3) for elem in polyline) and (
                len(polyline) == length if length is not None else True)
 
 
-def is_valid_list_of_vertices(vertices: npy.ndarray, number_of_vertices=None):
+def is_valid_list_of_vertices(vertices: list, number_of_vertices=None):
     """
-    Checks if a provided list of vertices is a valid, i.e., it is a list of points (xi,yi). The list must
-    have a shape of (n, 2), resulting in [[x0, y0], [x1, y1], ...]. The number of vertices can be checked with the
-    provided parameter number_of_vertices.
+    Checks if a provided list of vertices is a valid, i.e., it is a list of points (xi,yi), or (xi,yi,zi). The list must
+    have a shape of (n, 2) or (n, 3), resulting in [[x0, y0], [x1, y1], ...] or [[x0, y0, z0], [x1, y1, z1], ...].
+    The number of vertices can be checked with the provided parameter number_of_vertices.
     :param vertices: list of vertices [[x0, y0], [x1, y1], ...]
     :param number_of_vertices: The assumed number of vertices
     :return: True if vertices is a valid list of vertices, False otherwise
     """
     if number_of_vertices is not None:
         assert is_valid_length(number_of_vertices)
 
     return isinstance(vertices, ValidTypes.LISTS) and len(vertices) >= 1 and all(
-            is_real_number_vector(elem, 2) for elem in vertices) and (
+            # it is possible to create a list with different sized elements, i.e. [[x1,y1],[x1,y1,z1]],
+            # there is no value error, as the lists are not np.arrays
+            is_list_of_numbers(elem, 2) or is_list_of_numbers(elem, 3) for elem in vertices) and (
                len(vertices) == number_of_vertices if number_of_vertices is not None else True)
 
 
 def is_valid_array_of_vertices(vertices: npy.ndarray, number_of_vertices=None):
     """
-    Checks if a provided array of vertices is a valid, i.e., it is a array of points (xi,yi). The array must
-    have a shape of (n, 2), resulting in [[x0, y0], [x1, y1], ...]. The number of vertices can be checked with the
-    provided parameter number_of_vertices.
+    Checks if a provided array of vertices is a valid, i.e., it is na array of points (xi,yi) or (xi,yi,zi).
+    The array must have a shape of (n, 2), resulting in [[x0, y0], [x1, y1], ...] or [[x0, y0, z0], [x1, y1, z1], ...].
+    The number of vertices can be checked with the provided parameter number_of_vertices.
     :param vertices: array of vertices [[x0, y0], [x1, y1], ...]
     :param number_of_vertices: The assumed number of vertices
     :return: True if vertices is a valid array of vertices, False otherwise
     """
     if number_of_vertices is not None:
         assert is_valid_length(number_of_vertices)
 
     return isinstance(vertices, ValidTypes.ARRAY) and len(vertices) >= 1 and all(
-            is_real_number_vector(elem, 2) for elem in vertices) and (
+            #  it is not possible (ValueError) to create am array (np.array) with different sized vectors,
+            #  so all the vectors will either be 2d (without z-coordinate) or 3d (with z-coordinate)
+            is_real_number_vector(elem, 2) or is_real_number_vector(elem, 3) for elem in vertices) and (
                len(vertices) == number_of_vertices if number_of_vertices is not None else True)
```

### Comparing `commonroad_io-2023.1/commonroad/common/writer/file_writer_interface.py` & `commonroad_io-2023.2/commonroad/common/writer/file_writer_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,17 +111,21 @@
                                overwrite_existing_file: OverwriteExistingFile = OverwriteExistingFile.ASK_USER_INPUT):
         pass
 
     @staticmethod
     def check_validity_of_commonroad_file(commonroad_str: Union[str, bytes]) -> bool:
         pass
 
+    @abstractmethod
+    def _get_suffix(self) -> str:
+        pass
+
     def _handle_file_path(self, filename: Union[str, None], overwrite_existing_file: OverwriteExistingFile) -> str:
         if filename is None:
-            filename = str(self.scenario.scenario_id) + ".xml"
+            filename = str(self.scenario.scenario_id) + self._get_suffix()
 
         if pathlib.Path(filename).is_file():
             if overwrite_existing_file is OverwriteExistingFile.ASK_USER_INPUT:
                 overwrite = input('File {} already exists, replace old file (or else skip)? (y/n)'.format(filename))
             elif overwrite_existing_file is OverwriteExistingFile.SKIP:
                 overwrite = 'n'
             else:
```

### Comparing `commonroad_io-2023.1/commonroad/common/writer/file_writer_protobuf.py` & `commonroad_io-2023.2/commonroad/common/writer/file_writer_protobuf.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,33 +2,35 @@
 import re
 from typing import Set, Union, List
 import logging
 
 import numpy as np
 from google.protobuf.message import DecodeError
 
-from commonroad.common.util import Interval
+from commonroad.common.util import Interval, FileFormat, Time
 from commonroad.common.writer.file_writer_interface import FileWriter, OverwriteExistingFile
 from commonroad.geometry.shape import Rectangle, Circle, Polygon, ShapeGroup, Shape
 from commonroad.planning.planning_problem import PlanningProblemSet, PlanningProblem
 from commonroad.prediction.prediction import Occupancy, TrajectoryPrediction, SetBasedPrediction
 from commonroad.scenario_definition.protobuf_format.generated_scripts import commonroad_pb2, util_pb2, \
     phantom_obstacle_pb2
 from commonroad.scenario_definition.protobuf_format.generated_scripts import lanelet_pb2, planning_problem_pb2, \
     traffic_sign_pb2, scenario_tags_pb2, environment_obstacle_pb2, obstacle_pb2, intersection_pb2, \
     dynamic_obstacle_pb2, static_obstacle_pb2, traffic_light_pb2, location_pb2
 from commonroad.scenario.intersection import Intersection, IntersectionIncomingElement
-from commonroad.scenario.lanelet import Lanelet, LineMarking, StopLine
+from commonroad.scenario.lanelet import Lanelet
+from commonroad.common.common_lanelet import StopLine, LineMarking
 from commonroad.scenario.obstacle import StaticObstacle, DynamicObstacle, EnvironmentObstacle, SignalState, \
     PhantomObstacle
-from commonroad.scenario.scenario import Scenario, Tag, Location, GeoTransformation, Environment, Time
-from commonroad.scenario.traffic_sign import TrafficSign, TrafficLight, TrafficSignElement, TrafficLightCycleElement, \
+from commonroad.scenario.scenario import Scenario, Tag, Location, GeoTransformation, Environment
+from commonroad.scenario.traffic_sign import TrafficSign, TrafficSignElement, \
     TrafficSignIDGermany, TrafficSignIDFrance, TrafficSignIDZamunda, TrafficSignIDUsa, TrafficSignIDChina, \
     TrafficSignIDSpain, TrafficSignIDRussia, TrafficSignIDArgentina, TrafficSignIDBelgium, TrafficSignIDGreece, \
     TrafficSignIDCroatia, TrafficSignIDItaly
+from commonroad.scenario.traffic_light import TrafficLightCycleElement, TrafficLight
 from commonroad.scenario.trajectory import Trajectory
 from commonroad.scenario.state import State
 
 logger = logging.getLogger(__name__)
 
 
 class ProtobufFileWriter(FileWriter):
@@ -116,17 +118,19 @@
     def _serialize_write_msg(self, filename: str):
         """
         Serializes the message of type commonroad and writes into file.
 
         :param filename: Name of file
         :return:
         """
-        f = open(filename, "wb")
-        f.write(self._commonroad_msg.SerializeToString())
-        f.close()
+        with open(filename, "wb") as f:
+            f.write(self._commonroad_msg.SerializeToString())
+
+    def _get_suffix(self) -> str:
+        return FileFormat.PROTOBUF.value
 
     def write_to_file(self, filename: Union[str, None] = None,
                       overwrite_existing_file: OverwriteExistingFile = OverwriteExistingFile.ASK_USER_INPUT,
                       check_validity: bool = False):
         """
         Writes message of type commonroad into file.
 
@@ -381,17 +385,14 @@
 
         traffic_sign_msg.traffic_sign_id = traffic_sign.traffic_sign_id
 
         for traffic_sign_element in traffic_sign.traffic_sign_elements:
             traffic_sign_element_msg = TrafficSignElementMessage.create_message(traffic_sign_element)
             traffic_sign_msg.traffic_sign_elements.append(traffic_sign_element_msg)
 
-        for first_occurrence in traffic_sign.first_occurrence:
-            traffic_sign_msg.first_occurrences.append(first_occurrence)
-
         if traffic_sign.position is not None:
             point_msg = PointMessage.create_message(traffic_sign.position)
             traffic_sign_msg.position.CopyFrom(point_msg)
 
         if traffic_sign.virtual is not None:
             traffic_sign_msg.virtual = traffic_sign.virtual
 
@@ -455,24 +456,24 @@
 
     @classmethod
     def create_message(cls, traffic_light: TrafficLight) -> traffic_light_pb2.TrafficLight:
         traffic_light_msg = traffic_light_pb2.TrafficLight()
 
         traffic_light_msg.traffic_light_id = traffic_light.traffic_light_id
 
-        for cycle_element in traffic_light.cycle:
+        for cycle_element in traffic_light.traffic_light_cycle.cycle_elements:
             cycle_element_msg = CycleElementMessage.create_message(cycle_element)
             traffic_light_msg.cycle_elements.append(cycle_element_msg)
 
         if traffic_light.position is not None:
             point_msg = PointMessage.create_message(traffic_light.position)
             traffic_light_msg.position.CopyFrom(point_msg)
 
-        if traffic_light.time_offset is not None:
-            traffic_light_msg.time_offset = traffic_light.time_offset
+        if traffic_light.traffic_light_cycle.time_offset is not None:
+            traffic_light_msg.time_offset = traffic_light.traffic_light_cycle.time_offset
 
         if traffic_light.direction is not None:
             traffic_light_msg.direction = traffic_light_pb2.TrafficLightDirectionEnum.TrafficLightDirection \
                 .Value(traffic_light.direction.name)
 
         if traffic_light.active is not None:
             traffic_light_msg.active = traffic_light.active
```

### Comparing `commonroad_io-2023.1/commonroad/common/writer/file_writer_xml.py` & `commonroad_io-2023.2/commonroad/common/writer/file_writer_xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,28 @@
 import warnings
 from typing import Set, Union, List
 import numpy as np
 from lxml import etree, objectify
 import logging
 
 from commonroad import SCENARIO_VERSION
-from commonroad.common.util import Interval
+from commonroad.common.util import Interval, FileFormat
 from commonroad.geometry.shape import ShapeGroup, Shape, Circle, Rectangle, Polygon
 from commonroad.planning.planning_problem import PlanningProblem, PlanningProblemSet
 from commonroad.prediction.prediction import SetBasedPrediction, TrajectoryPrediction, Occupancy
 from commonroad.scenario.intersection import Intersection
-from commonroad.scenario.lanelet import Lanelet, LineMarking, LaneletType, StopLine
+from commonroad.scenario.lanelet import Lanelet
+from commonroad.common.common_lanelet import StopLine, LineMarking, LaneletType
 from commonroad.scenario.obstacle import Obstacle, DynamicObstacle, StaticObstacle, EnvironmentObstacle, \
     PhantomObstacle, ObstacleRole, ObstacleType, SignalState
 from commonroad.scenario.scenario import Location, GeoTransformation, Environment, TimeOfDay, Weather, Underground, \
     Tag, Scenario
-from commonroad.scenario.traffic_sign import TrafficSign, TrafficLight, TrafficLightCycleElement, TrafficLightDirection
+from commonroad.scenario.traffic_sign import TrafficSign
+from commonroad.scenario.traffic_light import TrafficLightDirection, TrafficLightCycleElement, TrafficLight, \
+    TrafficLightCycle
 from commonroad.scenario.trajectory import Trajectory
 from commonroad.scenario.state import State
 from commonroad.common.writer.file_writer_interface import FileWriter, precision, OverwriteExistingFile
 
 logger = logging.getLogger(__name__)
 
 
@@ -162,14 +165,17 @@
             self._root_node.append(PlanningProblemXMLNode.create_node(planning_problem))
 
     def _dump(self):
         rough_string = etree.tostring(self._root_node, pretty_print=True, encoding='UTF-8')
         rough_string = rough_string
         return rough_string
 
+    def _get_suffix(self) -> str:
+        return FileFormat.XML.value
+
     def write_to_file(self, filename: Union[str, None] = None,
                       overwrite_existing_file: OverwriteExistingFile = OverwriteExistingFile.ASK_USER_INPUT,
                       check_validity: bool = False):
         """
         Write a scenario including planning-problem. If file already exists, it will be overwritten of skipped
 
         :param filename: filename of the xml output file. If 'None', the Benchmark ID is taken
@@ -1139,23 +1145,18 @@
 
 
 class TrafficLightXMLNode:
     @classmethod
     def create_node(cls, traffic_light: TrafficLight) -> etree.Element:
         traffic_light_node = etree.Element('trafficLight')
         traffic_light_node.set('id', str(traffic_light.traffic_light_id))
-        cycle_node = etree.Element('cycle')
-        for state in traffic_light.cycle:
-            element_node = TrafficLightCycleElementXMLNode.create_node(state)
-            cycle_node.append(element_node)
-        if traffic_light.time_offset is not None and traffic_light.time_offset > 0:
-            offset_node = etree.Element('timeOffset')
-            offset_node.text = str(traffic_light.time_offset)
-            cycle_node.append(offset_node)
-        traffic_light_node.append(cycle_node)
+        if traffic_light.traffic_light_cycle is not None:
+            traffic_light_cycle_node = TrafficLightCycleXMLNode.create_node(traffic_light.traffic_light_cycle)
+
+            traffic_light_node.append(traffic_light_cycle_node)
 
         if traffic_light.position is not None:
             position_node = etree.Element('position')
             position_node.append(Point(traffic_light.position[0],
                                        traffic_light.position[1]).create_node())
             traffic_light_node.append(position_node)
 
@@ -1174,14 +1175,30 @@
     @classmethod
     def create_ref_node(cls, traffic_light_ref) -> etree.Element:
         traffic_light_ref_node = etree.Element('trafficLightRef')
         traffic_light_ref_node.set('ref', str(traffic_light_ref))
         return traffic_light_ref_node
 
 
+class TrafficLightCycleXMLNode:
+    @classmethod
+    def create_node(cls, traffic_light_cycle: TrafficLightCycle) -> etree.Element:
+        traffic_light_cycle_node = etree.Element("cycle")
+        for state in traffic_light_cycle.cycle_elements:
+            element_node = TrafficLightCycleElementXMLNode.create_node(state)
+            traffic_light_cycle_node.append(element_node)
+
+        if traffic_light_cycle.time_offset is not None and traffic_light_cycle.time_offset > 0:
+            offset_node = etree.Element('timeOffset')
+            offset_node.text = str(traffic_light_cycle.time_offset)
+            traffic_light_cycle_node.append(offset_node)
+
+        return traffic_light_cycle_node
+
+
 class TrafficLightCycleElementXMLNode:
     @classmethod
     def create_node(cls, cycle_element: TrafficLightCycleElement) -> etree.Element:
         element_node = etree.Element("cycleElement")
         duration_node = etree.Element("duration")
         duration_node.text = str(cycle_element.duration)
         element_node.append(duration_node)
```

### Comparing `commonroad_io-2023.1/commonroad/geometry/polyline_util.py` & `commonroad_io-2023.2/commonroad/geometry/polyline_util.py`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/geometry/shape.py` & `commonroad_io-2023.2/commonroad/geometry/shape.py`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/geometry/transform.py` & `commonroad_io-2023.2/commonroad/geometry/transform.py`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/planning/goal.py` & `commonroad_io-2023.2/commonroad/planning/goal.py`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/planning/planning_problem.py` & `commonroad_io-2023.2/commonroad/planning/planning_problem.py`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/prediction/prediction.py` & `commonroad_io-2023.2/commonroad/prediction/prediction.py`

 * *Files 3% similar despite different names*

```diff
@@ -225,27 +225,17 @@
         Prediction.__init__(self, self._trajectory.initial_time_step, self._create_occupancy_set())
 
     def __eq__(self, other):
         if not isinstance(other, TrajectoryPrediction):
             warnings.warn(f"Inequality between TrajectoryPrediction {repr(self)} and different type {type(other)}")
             return False
 
-        center_lanelet_assignment = None if self._center_lanelet_assignment is None \
-            else dict((key, list(value)) for key, value in self._center_lanelet_assignment.items()).items()
-        center_lanelet_assignment_other = None if other._center_lanelet_assignment is None \
-            else dict((key, list(value)) for key, value in other._center_lanelet_assignment.items()).items()
-
-        shape_lanelet_assignment = None if self._shape_lanelet_assignment is None \
-            else dict((key, list(value)) for key, value in self._shape_lanelet_assignment.items()).items()
-        shape_lanelet_assignment_other = None if other._shape_lanelet_assignment is None \
-            else dict((key, list(value)) for key, value in other._shape_lanelet_assignment.items()).items()
-
-        prediction_eq = self._trajectory == other.trajectory and self._shape == other.shape and \
-            center_lanelet_assignment == center_lanelet_assignment_other and \
-            shape_lanelet_assignment == shape_lanelet_assignment_other and Prediction.__eq__(self, other)
+        prediction_eq = self._shape == other.shape and self._trajectory == other.trajectory and \
+            self.center_lanelet_assignment == other.center_lanelet_assignment and \
+            self.shape_lanelet_assignment == other.shape_lanelet_assignment and Prediction.__eq__(self, other)
 
         return prediction_eq
 
     def __hash__(self):
         center_lanelet_assignment = None if self._center_lanelet_assignment is None \
             else dict((key, list(value)) for key, value in self._center_lanelet_assignment.items()).items()
         shape_lanelet_assignment = None if self._shape_lanelet_assignment is None \
```

### Comparing `commonroad_io-2023.1/commonroad/scenario/intersection.py` & `commonroad_io-2023.2/commonroad/scenario/intersection.py`

 * *Files 9% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                f"incoming_lanelets={self._incoming_lanelets}, successors_right={self._successors_right}, " \
                f"successors_straight={self._successors_straight}, successors_left={self._successors_left}, " \
                f"left_of={self._left_of})"
 
     @property
     def incoming_id(self) -> int:
         """
-        :returns ID of incoming
+        ID of incoming
         """
         return self._incoming_id
 
     @incoming_id.setter
     def incoming_id(self, i_id: int):
         """
         :param i_id ID of incoming
@@ -76,29 +76,29 @@
         assert is_natural_number(i_id), '<IntersectionIncomingElement/incoming_id>: Provided incoming_id is not ' \
                                         'valid! id={}'.format(i_id)
         self._incoming_id = i_id
 
     @property
     def incoming_lanelets(self) -> Set[int]:
         """
-        :returns set of IDs of incoming lanelets
+        set of IDs of incoming lanelets
         """
         return self._incoming_lanelets
 
     @incoming_lanelets.setter
     def incoming_lanelets(self, incoming_lanelets: Set[int]):
         """
         :param incoming_lanelets: set of IDs of incoming lanelets
         """
         self._incoming_lanelets = incoming_lanelets
 
     @property
     def successors_right(self) -> Set[int]:
         """
-        :returns set of IDs of incoming lanelets which turn right
+        set of IDs of incoming lanelets which turn right
         """
         return self._successors_right
 
     @successors_right.setter
     def successors_right(self, successors_right: Set[int]):
         """
         :param successors_right: set of IDs of incoming lanelets which turn right
@@ -107,15 +107,15 @@
             self._successors_right = set()
         else:
             self._successors_right = successors_right
 
     @property
     def successors_straight(self) -> Set[int]:
         """
-        :returns set of IDs of incoming lanelets which go straight
+        set of IDs of incoming lanelets which go straight
         """
         return self._successors_straight
 
     @successors_straight.setter
     def successors_straight(self, successors_straight: Set[int]):
         """
         :param successors_straight: set of IDs of incoming lanelets which go straight
@@ -124,15 +124,15 @@
             self._successors_straight = set()
         else:
             self._successors_straight = successors_straight
 
     @property
     def successors_left(self) -> Set[int]:
         """
-        :returns set of IDs of incoming lanelets which turn left
+        set of IDs of incoming lanelets which turn left
         """
         return self._successors_left
 
     @successors_left.setter
     def successors_left(self, successors_left: Set[int]):
         """
         :param successors_left: set of IDs of incoming lanelets which turn left
@@ -141,15 +141,15 @@
             self._successors_left = set()
         else:
             self._successors_left = successors_left
 
     @property
     def left_of(self) -> int:
         """
-        :returns incoming element ID of incoming element located left of this incoming element
+        incoming element ID of incoming element located left of this incoming element
         """
         return self._left_of
 
     @left_of.setter
     def left_of(self, left_of: int):
         """
         :param left_of: incoming element ID of incoming element located left of this incoming element
@@ -210,15 +210,15 @@
     def __repr__(self):
         return f"Intersection(intersection_id={self._intersection_id}, incomings={repr(self._incomings)}, " \
                f"crossings={self._crossings})"
 
     @property
     def intersection_id(self) -> int:
         """
-        :returns ID of intersection element
+        ID of intersection element
         """
         return self._intersection_id
 
     @intersection_id.setter
     def intersection_id(self, i_id: int):
         """
         :param i_id ID of intersection element
@@ -226,29 +226,29 @@
         assert is_natural_number(i_id), '<Intersection/intersection_id>: Provided intersection_id is not ' \
                                         'valid! id={}'.format(i_id)
         self._intersection_id = i_id
 
     @property
     def incomings(self) -> List[IntersectionIncomingElement]:
         """
-        :returns set of incoming elements in intersection
+        set of incoming elements in intersection
         """
         return self._incomings
 
     @incomings.setter
     def incomings(self, incomings: List[IntersectionIncomingElement]):
         """
         :param incomings: i_id ID of intersection element
         """
         self._incomings = incomings
 
     @property
     def crossings(self) -> Set[int]:
         """
-        :returns set of crossing elements in intersection
+        set of crossing elements in intersection
         """
         return self._crossings
 
     @crossings.setter
     def crossings(self, crossings: Set[int]):
         """
         :param crossings: set of crossing elements in intersection
@@ -258,10 +258,9 @@
         else:
             self._crossings = crossings
 
     @property
     def map_incoming_lanelets(self) -> Dict[int, IntersectionIncomingElement]:
         """
         Maps all incoming lanelet ids to IntersectionIncomingElement
-        :returns dictionary mapping lanelet IDs to incomings
         """
         return {l_id: inc for inc in self.incomings for l_id in inc.incoming_lanelets}
```

### Comparing `commonroad_io-2023.1/commonroad/scenario/lanelet.py` & `commonroad_io-2023.2/commonroad/scenario/lanelet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,216 +1,56 @@
 import copy
 import enum
+from collections import defaultdict
 from typing import *
 
 import numpy as np
+from datetime import datetime
 from shapely.geometry import Point as ShapelyPoint
 from shapely.geometry import Polygon as ShapelyPolygon
 from shapely.strtree import STRtree
 
 import commonroad.geometry.transform
-from commonroad.common.util import subtract_orientations
+from commonroad.common.util import subtract_orientations, Time
 from commonroad.common.validity import *
 from commonroad.geometry.shape import Polygon, ShapeGroup, Circle, Rectangle, Shape
 from commonroad.scenario.intersection import Intersection
 from commonroad.scenario.obstacle import Obstacle
 from commonroad.scenario.state import TraceState
-from commonroad.scenario.traffic_sign import TrafficSign, TrafficLight
+from commonroad.scenario.traffic_sign import TrafficSign
+from commonroad.scenario.traffic_light import TrafficLight
+from commonroad.scenario.area import Area
 from commonroad.visualization.drawable import IDrawable
 from commonroad.visualization.renderer import IRenderer
 from commonroad.visualization.draw_params import OptionalSpecificOrAllDrawParams, LaneletNetworkParams
+from commonroad.common.common_lanelet import RoadUser, StopLine, LineMarking, LaneletType
 
 
 __author__ = "Christian Pek, Sebastian Maierhofer"
 __copyright__ = "TUM Cyber-Physical Systems Group"
 __credits__ = ["BMW CAR@TUM"]
 __version__ = "2023.1"
 __maintainer__ = "Sebastian Maierhofer"
 __email__ = "commonroad@lists.lrz.de"
 __status__ = "released"
 
 
-class LineMarking(enum.Enum):
-    """
-    Enum describing different types of line markings, i.e. dashed or solid lines
-    """
-    DASHED = 'dashed'
-    SOLID = 'solid'
-    BROAD_DASHED = 'broad_dashed'
-    BROAD_SOLID = 'broad_solid'
-    UNKNOWN = 'unknown'
-    NO_MARKING = 'no_marking'
-
-
-class LaneletType(enum.Enum):
-    """
-    Enum describing different types of lanelets
-    """
-    URBAN = 'urban'
-    COUNTRY = 'country'
-    HIGHWAY = 'highway'
-    DRIVE_WAY = 'driveWay'
-    MAIN_CARRIAGE_WAY = 'mainCarriageWay'
-    ACCESS_RAMP = 'accessRamp'
-    EXIT_RAMP = 'exitRamp'
-    SHOULDER = 'shoulder'
-    BUS_LANE = 'busLane'
-    BUS_STOP = 'busStop'
-    BICYCLE_LANE = 'bicycleLane'
-    SIDEWALK = 'sidewalk'
-    CROSSWALK = 'crosswalk'
-    INTERSTATE = 'interstate'
-    INTERSECTION = 'intersection'
-    BORDER = 'border'
-    PARKING = 'parking'
-    RESTRICTED = 'restricted'  # cars not allowed, e.g., special lanes for busses
-    UNKNOWN = 'unknown'
-
-
-class RoadUser(enum.Enum):
-    """
-    Enum describing different types of road users
-    """
-    VEHICLE = 'vehicle'
-    CAR = 'car'
-    TRUCK = 'truck'
-    BUS = 'bus'
-    PRIORITY_VEHICLE = 'priorityVehicle'
-    MOTORCYCLE = 'motorcycle'
-    BICYCLE = 'bicycle'
-    PEDESTRIAN = 'pedestrian'
-    TRAIN = 'train'
-    TAXI = 'taxi'
-
-
-class StopLine:
-    """Class which describes the stop line of a lanelet"""
-
-    def __init__(self, start: np.ndarray, end: np.ndarray, line_marking: LineMarking, traffic_sign_ref: Set[int] = None,
-                 traffic_light_ref: Set[int] = None):
-        self._start = start
-        self._end = end
-        self._line_marking = line_marking
-        self._traffic_sign_ref = traffic_sign_ref
-        self._traffic_light_ref = traffic_light_ref
-
-    def __eq__(self, other):
-        if not isinstance(other, StopLine):
-            warnings.warn(f"Inequality between StopLine {repr(self)} and different type {type(other)}")
-            return False
-
-        prec = 10
-        start_string = np.array2string(np.around(self._start.astype(float), prec), precision=prec)
-        start_other_string = np.array2string(np.around(other.start.astype(float), prec), precision=prec)
-        end_string = np.array2string(np.around(self._end.astype(float), prec), precision=prec)
-        end_other_string = np.array2string(np.around(other.end.astype(float), prec), precision=prec)
-
-        if start_string == start_other_string and end_string == end_other_string and self._line_marking == \
-                other.line_marking and self._traffic_sign_ref == other.traffic_sign_ref and self._traffic_light_ref \
-                == other.traffic_light_ref:
-            return True
-
-        warnings.warn(f"Inequality of StopLine {repr(self)} and the other one {repr(other)}")
-        return False
-
-    def __hash__(self):
-        if self._start is None:
-            start_string = None
-        else:
-            start_string = np.array2string(np.around(self._start.astype(float), 10), precision=10)
-        if self._end is None:
-            end_string = None
-        else:
-            end_string = np.array2string(np.around(self._end.astype(float), 10), precision=10)
-        sign_ref = None if self._traffic_sign_ref is None else frozenset(self._traffic_sign_ref)
-        light_ref = None if self._traffic_light_ref is None else frozenset(self._traffic_light_ref)
-        return hash((start_string, end_string, self._line_marking, sign_ref, light_ref))
-
-    def __str__(self):
-        return f'StopLine from {self._start} to {self._end}'
-
-    def __repr__(self):
-        return f"StopLine(start={self._start.tolist()}, end={self._end.tolist()}, line_marking={self._line_marking}, " \
-               f"traffic_sign_ref={self._traffic_sign_ref}, traffic_light_ref={self._traffic_light_ref})"
-
-    @property
-    def start(self) -> np.ndarray:
-        return self._start
-
-    @start.setter
-    def start(self, value: np.ndarray):
-        self._start = value
-
-    @property
-    def end(self) -> np.ndarray:
-        return self._end
-
-    @end.setter
-    def end(self, value: np.ndarray):
-        self._end = value
-
-    @property
-    def line_marking(self) -> LineMarking:
-        return self._line_marking
-
-    @line_marking.setter
-    def line_marking(self, marking: LineMarking):
-        self._line_marking = marking
-
-    @property
-    def traffic_sign_ref(self) -> Set[int]:
-        return self._traffic_sign_ref
-
-    @traffic_sign_ref.setter
-    def traffic_sign_ref(self, references: Set[int]):
-        self._traffic_sign_ref = references
-
-    @property
-    def traffic_light_ref(self) -> Set[int]:
-        return self._traffic_light_ref
-
-    @traffic_light_ref.setter
-    def traffic_light_ref(self, references: Set[int]):
-        self._traffic_light_ref = references
-
-    def translate_rotate(self, translation: np.ndarray, angle: float):
-        """
-        This method translates and rotates a stop line
-
-        :param translation: The translation given as [x_off,y_off] for the x and y translation
-        :param angle: The rotation angle in radian (counter-clockwise defined)
-        """
-
-        assert is_real_number_vector(translation, 2), '<Lanelet/translate_rotate>: provided translation ' \
-                                                      'is not valid! translation = {}'.format(translation)
-        assert is_valid_orientation(
-                angle), '<Lanelet/translate_rotate>: provided angle is not valid! angle = {}'.format(angle)
-
-        # create transformation matrix
-        t_m = commonroad.geometry.transform.translation_rotation_matrix(translation, angle)
-        line_vertices = np.array([self._start, self._end])
-        # transform center vertices
-        tmp = t_m.dot(np.vstack((line_vertices.transpose(), np.ones((1, line_vertices.shape[0])))))
-        tmp = tmp[0:2, :].transpose()
-        self._start, self._end = tmp[0], tmp[1]
-
-
 class Lanelet:
     """
     Class which describes a Lanelet entity according to the CommonRoad specification. Each lanelet is described by a
     left and right boundary (polylines). Furthermore, lanelets have relations to other lanelets, e.g. an adjacent left
     neighbor or a predecessor.
     """
 
     def __init__(self, left_vertices: np.ndarray, center_vertices: np.ndarray, right_vertices: np.ndarray,
                  lanelet_id: int, predecessor=None, successor=None, adjacent_left=None,
                  adjacent_left_same_direction=None, adjacent_right=None, adjacent_right_same_direction=None,
                  line_marking_left_vertices=LineMarking.NO_MARKING, line_marking_right_vertices=LineMarking.NO_MARKING,
                  stop_line=None, lanelet_type=None, user_one_way=None, user_bidirectional=None, traffic_signs=None,
-                 traffic_lights=None, ):
+                 traffic_lights=None, adjacent_areas=None):
         """
         Constructor of a Lanelet object
         :param left_vertices: The vertices of the left boundary of the Lanelet described as a
         polyline [[x0,y0],[x1,y1],...,[xn,yn]]
         :param center_vertices: The vertices of the center line of the Lanelet described as a
         polyline [[x0,y0],[x1,y1],...,[xn,yn]]
         :param right_vertices: The vertices of the right boundary of the Lanelet described as a
@@ -228,14 +68,15 @@
         :param line_marking_right_vertices: The type of line marking of the right boundary
         :param stop_line: The stop line of the lanelet
         :param lanelet_type: The types of lanelet applicable here
         :param user_one_way: type of users that will use the lanelet as one-way
         :param user_bidirectional: type of users that will use the lanelet as bidirectional way
         :param traffic_signs: Traffic signs to be applied
         :param traffic_lights: Traffic lights to follow
+        :param adjacent_areas: Areas that are adjacent to the lanelet
         """
 
         # Set required properties
         self._left_vertices = None
         self._right_vertices = None
         self._center_vertices = None
         self._lanelet_id = None
@@ -316,14 +157,20 @@
 
         self._traffic_lights = None
         if traffic_lights is None:
             self._traffic_lights = set()
         else:
             self.traffic_lights = traffic_lights
 
+        self._adjacent_areas = None
+        if adjacent_areas is None:
+            self._adjacent_areas = set()
+        else:
+            self.adjacent_areas = adjacent_areas
+
     def __eq__(self, other):
         if not isinstance(other, Lanelet):
             warnings.warn(f"Inequality between Lanelet {repr(self)} and different type {type(other)}")
             return False
 
         list_elements_eq = self._stop_line == other.stop_line
 
@@ -342,29 +189,30 @@
                 other.line_marking_left_vertices and self._line_marking_right_vertices == \
                 other.line_marking_right_vertices and set(
                 self._predecessor) == set(other.predecessor) and set(self._successor) == set(
                 other.successor) and self._adj_left == other.adj_left and self._adj_right == other.adj_right and \
                 self._adj_left_same_direction == other.adj_left_same_direction and self._adj_right_same_direction == \
                 other.adj_right_same_direction and self._lanelet_type == other.lanelet_type and self._user_one_way ==\
                 self.user_one_way and self._user_bidirectional == other.user_bidirectional and self._traffic_signs ==\
-                other.traffic_signs and self._traffic_lights == other.traffic_lights:
+                other.traffic_signs and self._traffic_lights == other.traffic_lights and self._adjacent_areas == \
+                other.adjacent_areas:
             return list_elements_eq
 
         warnings.warn(f"Inequality of Lanelet {repr(self)} and the other one {repr(other)}")
         return False
 
     def __hash__(self):
         polylines = [self._left_vertices, self._right_vertices, self._center_vertices]
         polyline_strings = []
         for polyline in polylines:
             polyline_string = np.array2string(np.around(polyline.astype(float), 10), precision=10)
             polyline_strings.append(polyline_string)
 
         elements = [self._predecessor, self._successor, self._lanelet_type, self._user_one_way,
-                    self._user_bidirectional, self._traffic_signs, self._traffic_lights]
+                    self._user_bidirectional, self._traffic_signs, self._traffic_lights, self._adjacent_areas]
         frozen_elements = [frozenset(e) for e in elements]
 
         return hash((self._lanelet_id, tuple(polyline_strings), self._line_marking_left_vertices,
                      self._line_marking_right_vertices, self._stop_line, self._adj_left, self._adj_right,
                      self._adj_left_same_direction, self._adj_right_same_direction, tuple(frozen_elements)))
 
     def __str__(self):
@@ -381,33 +229,34 @@
                f"adjacent_left_same_direction={self._adj_left_same_direction}, adjacent_right={self._adj_right}, " \
                f"adjacent_right_same_direction={self._adj_right_same_direction}, " \
                f"line_marking_left_vertices={self._line_marking_left_vertices}, " \
                f"line_marking_right_vertices={self._line_marking_right_vertices}), " \
                f"stop_line={repr(self._stop_line)}, lanelet_type={self._lanelet_type}, " \
                f"user_one_way={self._user_one_way}, " \
                f"user_bidirectional={self._user_bidirectional}, traffic_signs={self._traffic_signs}, " \
-               f"traffic_lights={self._traffic_lights}"
+               f"traffic_lights={self._traffic_lights}, "\
+               f"adjacent_areas={self._adjacent_areas}"
 
     @property
     def distance(self) -> np.ndarray:
         """
-        :returns cumulative distance along center vertices
+        cumulative distance along center vertices
         """
         if self._distance is None:
             self._distance = self._compute_polyline_cumsum_dist([self.center_vertices])
         return self._distance
 
     @distance.setter
     def distance(self, distance: np.ndarray):
         self._distance = distance
 
     @property
     def inner_distance(self) -> np.ndarray:
         """
-        :returns minimum cumulative distance along left and right vertices, i.e., along the inner curve:
+        minimum cumulative distance along left and right vertices, i.e., along the inner curve:
         """
         if self._inner_distance is None:
             self._inner_distance = self._compute_polyline_cumsum_dist([self.left_vertices, self.right_vertices])
 
         return self._inner_distance
 
     @property
@@ -630,14 +479,24 @@
     @traffic_lights.setter
     def traffic_lights(self, traffic_light_ids: Set[int]):
         assert isinstance(traffic_light_ids, set), '<Lanelet/traffic_lights>: provided list of ids is not a ' \
                                                    'set! type = {}'.format(type(traffic_light_ids))
         self._traffic_lights = traffic_light_ids
 
     @property
+    def adjacent_areas(self) -> Set[int]:
+        return self._adjacent_areas
+
+    @adjacent_areas.setter
+    def adjacent_areas(self, value: Set[int]):
+        assert isinstance(value, set), '<Lanelet/adjacent_areas>: provided list of ids is not a ' \
+                                                   'set! type = {}'.format(type(value))
+        self._adjacent_areas = value
+
+    @property
     def polygon(self) -> Polygon:
         return self._polygon
 
     def add_predecessor(self, lanelet: int):
         """
         Adds the ID of a predecessor lanelet to the list of predecessors.
         :param lanelet: Predecessor lanelet ID.
@@ -984,14 +843,22 @@
         """
         Adds a traffic light ID to lanelet
 
         :param traffic_light_id: traffic light ID to add
         """
         self.traffic_lights.add(traffic_light_id)
 
+    def add_adjacent_area_to_lanelet(self, area_id: int):
+        """
+        Adds an area ID to lanelet
+
+        :param area_id: adjacent area ID to add
+        """
+        self.adjacent_areas.add(area_id)
+
     def dynamic_obstacle_by_time_step(self, time_step) -> Set[int]:
         """
         Returns all dynamic obstacles on lanelet at specific time step
 
         :param time_step: time step of interest
         :returns: list of obstacle IDs
         """
@@ -1035,33 +902,184 @@
             vertex2 = self.center_vertices[closest_vertex_index + 1, :]
 
         direction_vector = vertex2 - vertex1
 
         return np.arctan2(direction_vector[1], direction_vector[0])
 
 
+class MapInformation:
+    """
+    Class which represents additional information about Lanelet Network
+    """
+    def __init__(self, commonroad_version: str = "2023a", map_id: str = "map_id", date: Time = None,
+                 author: str = "author", affiliation: str = "affiliation", source: str = "source",
+                 licence_name: str = "licence_name", licence_text: str = None):
+        """
+        Constructor for MapInformation
+
+        :param commonroad_version: version of CommonRoad
+        :param map_id: the id of the lanelet network
+        :param date: date of the lanelet network
+        :param author: author of the lanelet network
+        :param affiliation: affiliation of the lanelet network
+        :param source: source of the lanelet network
+        :param licence_name: licence name of the lanelet network
+        :param licence_text: licence text of the lanelet network
+        """
+        self._commonroad_version = commonroad_version
+        self._map_id = map_id
+        if date is None:
+            time = datetime.now()
+            self._date = Time(time.hour, time.minute, time.day, time.month, time.year)
+        else:
+            self._date = date
+        self._author = author
+        self._affiliation = affiliation
+        self._source = source
+        self._licence_name = licence_name
+        if licence_text is None:
+            self._licence_text = ""
+        else:
+            self._licence_text = licence_text
+
+    def __eq__(self, other):
+        if not isinstance(other, MapInformation):
+            warnings.warn(f"Inequality between MapInformation {repr(self)} and different type {type(other)}")
+            return False
+
+        if self._commonroad_version == other.commonroad_version and self._map_id == other.map_id and \
+           self._date == other.date and self._author == other.author and self._affiliation == other.affiliation and \
+           self._source == other.source and self._licence_name == other.licence_name and \
+           self._licence_text == other.licence_text:
+            return True
+
+        warnings.warn(f"Inequality of MapInformation {repr(self)} and the other one {repr(other)}")
+        return False
+
+    def __repr__(self):
+        return f"MapInformation(commonroad_version={self._commonroad_version}, map_id={self._map_id}," \
+               f" date={self._date}, author={self._author}, affiliation={self._affiliation}, source={self._source}," \
+               f" licence_name={self._licence_name}, licence_text={self._licence_text}"
+
+    def __str__(self):
+        return f"MapInformation with commonroad version {self._commonroad_version}, map_id {self._map_id}," \
+               f" date {self._date}, author {self._author}, affiliation {self._affiliation}, source {self._source}," \
+               f" licence name {self._licence_name} and licence text {self._licence_text}"
+
+    def __hash__(self):
+        return hash((self._commonroad_version, self._map_id, self._date, self._author, self._affiliation,
+                     self._source, self._licence_name, self._licence_text))
+
+    @property
+    def commonroad_version(self) -> str:
+        """ Version of CommonRoad."""
+        return self._commonroad_version
+
+    @commonroad_version.setter
+    def commonroad_version(self, commonroad_version: str):
+        assert isinstance(commonroad_version, str), '<MapInformation/commonroad_version>: ' \
+                                            'Provided commonroad_version is not valid! id={}'.format(commonroad_version)
+        self._commonroad_version = commonroad_version
+
+    @property
+    def map_id(self) -> str:
+        """ The id of the lanelet network."""
+        return self._map_id
+
+    @map_id.setter
+    def map_id(self, map_id: str):
+        assert isinstance(map_id, str), '<MapInformation/map_id>: Provided map_id is not valid! id={}'.format(map_id)
+        self._map_id = map_id
+
+    @property
+    def date(self) -> Time:
+        """ Date of the lanelet network."""
+        return self._date
+
+    @date.setter
+    def date(self, date: Time):
+        assert isinstance(date, Time), '<MapInformation/date>: Provided date is not valid! id={}'.format(date)
+        self._date = date
+
+    @property
+    def author(self) -> str:
+        """ Author of the lanelet network."""
+        return self._author
+
+    @author.setter
+    def author(self, author: str):
+        assert isinstance(author, str), '<MapInformation/author>: Provided author is not valid! id={}'.format(author)
+        self._author = author
+
+    @property
+    def affiliation(self) -> str:
+        """ Affiliation of the lanelet network."""
+        return self._affiliation
+
+    @affiliation.setter
+    def affiliation(self, affiliation: str):
+        assert isinstance(affiliation, str), '<MapInformation/affiliation>: ' \
+                                             'Provided affiliation is not valid! id={}'.format(affiliation)
+        self._affiliation = affiliation
+
+    @property
+    def source(self) -> str:
+        """ Source of the lanelet network."""
+        return self._source
+
+    @source.setter
+    def source(self, source: str):
+        assert isinstance(source, str), '<MapInformation/source>: ' \
+                                             'Provided source is not valid! id={}'.format(source)
+        self._source = source
+
+    @property
+    def licence_name(self) -> str:
+        """ Licence name of the lanelet network."""
+        return self._licence_name
+
+    @licence_name.setter
+    def licence_name(self, licence_name: str):
+        assert isinstance(licence_name, str), '<MapInformation/licence_name>: ' \
+                                        'Provided licence_name is not valid! id={}'.format(licence_name)
+        self._licence_name = licence_name
+
+    @property
+    def licence_text(self) -> Union[None, str]:
+        """ Licence text of the lanelet network."""
+        return self._licence_text
+
+    @licence_text.setter
+    def licence_text(self, licence_text: Union[None, str]):
+        self._licence_text = licence_text
+
+
 class LaneletNetwork(IDrawable):
     """
     Class which represents a network of connected lanelets
     """
 
-    def __init__(self):
+    def __init__(self, information: MapInformation = MapInformation()):
         """
         Constructor for LaneletNetwork
+
+        :param information: map information of the lanelet network
         """
+        self._information = information
         self._lanelets: Dict[int, Lanelet] = {}
         # lanelet_id, shapely_polygon
         self._buffered_polygons: Dict[int, ShapelyPolygon] = {}
         self._strtee = None
         # id(shapely_polygon), lanelet_id
         self._lanelet_id_index_by_id: Dict[int, int] = {}
 
         self._intersections: Dict[int, Intersection] = {}
         self._traffic_signs: Dict[int, TrafficSign] = {}
         self._traffic_lights: Dict[int, TrafficLight] = {}
+        self._areas: Dict[int, Area] = {}
 
     # pickling of STRtree is not supported by shapely at the moment
     # use this workaround described in this issue:
     # https://github.com/Toblerity/Shapely/issues/1033
     def __getstate__(self):
         state = self.__dict__.copy()
         del state["_strtee"]
@@ -1090,72 +1108,101 @@
     def __eq__(self, other):
         if not isinstance(other, LaneletNetwork):
             warnings.warn(f"Inequality between LaneletNetwork {repr(self)} and different type {type(other)}")
             return False
 
         list_elements_eq = True
         lanelet_network_eq = True
-        elements = [self._lanelets, self._intersections, self._traffic_signs, self._traffic_lights]
-        elements_other = [other._lanelets, other._intersections, other._traffic_signs, other._traffic_lights]
+        elements = [self._lanelets, self._intersections, self._traffic_signs, self._traffic_lights,
+                    self._areas]
+        elements_other = [other._lanelets, other._intersections, other._traffic_signs,
+                          other._traffic_lights, other._areas]
         for i in range(0, len(elements)):
             e = elements[i]
             e_other = elements_other[i]
             lanelet_network_eq = lanelet_network_eq and len(e) == len(e_other)
             for k in e.keys():
                 if k not in e_other:
                     lanelet_network_eq = False
                     continue
                 if e.get(k) != e_other.get(k):
                     list_elements_eq = False
+        if self._information != other._information:
+            lanelet_network_eq = False
 
         if not lanelet_network_eq:
             warnings.warn(f"Inequality of LaneletNetwork {repr(self)} and the other one {repr(other)}")
 
         return lanelet_network_eq and list_elements_eq
 
     def __hash__(self):
-        return hash((frozenset(self._lanelets.items()), frozenset(self._intersections.items()),
-                     frozenset(self._traffic_signs.items()), frozenset(self._traffic_lights.items())))
+        return hash((self._information, frozenset(self._lanelets.items()), frozenset(self._intersections.items()),
+                     frozenset(self._traffic_signs.items()), frozenset(self._traffic_lights.items()),
+                     frozenset(self._areas.items())))
 
     def __str__(self):
         return f"LaneletNetwork consists of lanelets {set(self._lanelets.keys())}, " \
                f"intersections {set(self._intersections.keys())}, " \
-               f"traffic signs {set(self._traffic_signs.keys())}, and traffic lights {set(self._traffic_lights.keys())}"
+               f"traffic signs {set(self._traffic_signs.keys())}," \
+               f"traffic lights {set(self._traffic_lights.keys())}" \
+               f"and adjacent areas {set(self._areas.keys())}"
 
     def __repr__(self):
-        return f"LaneletNetwork(lanelets={repr(self._lanelets)}, intersections={repr(self._intersections)}, " \
-               f"traffic_signs={repr(self._traffic_signs)}, traffic_lights={repr(self._traffic_lights)})"
+        return f"LaneletNetwork(information={self._information}, lanelets={repr(self._lanelets)}, " \
+               f"intersections={repr(self._intersections)}, traffic_signs={repr(self._traffic_signs)}, " \
+               f"traffic_lights={repr(self._traffic_lights)}), areas={repr(self._areas)}"
 
     def _get_lanelet_id_by_shapely_polygon(self, polygon: ShapelyPolygon) -> int:
         return self._lanelet_id_index_by_id[id(polygon)]
 
     @property
+    def information(self) -> MapInformation:
+        """ Map information of the lanelet network."""
+        return self._information
+
+    @information.setter
+    def information(self, information: MapInformation):
+        assert isinstance(information, MapInformation), '<LaneletNetwork/information>: provided information is not ' \
+                                                        'valid! information = {}'.format(information)
+        self._information = information
+
+    @property
     def lanelets(self) -> List[Lanelet]:
+        """ List of lanelets of the lanelet network."""
         return list(self._lanelets.values())
 
     @property
     def lanelet_polygons(self) -> List[Polygon]:
+        """ List of polygons of the lanelet network."""
         return [la.polygon for la in self.lanelets]
 
     @property
     def intersections(self) -> List[Intersection]:
+        """ List of intersections of the lanelet network."""
         return list(self._intersections.values())
 
     @property
     def traffic_signs(self) -> List[TrafficSign]:
+        """ List of traffic signs of the lanelet network."""
         return list(self._traffic_signs.values())
 
     @property
     def traffic_lights(self) -> List[TrafficLight]:
+        """ List of traffic lights of the lanelet network."""
         return list(self._traffic_lights.values())
 
     @property
+    def areas(self) -> List[Area]:
+        """ List of areas of the lanelet network."""
+        return list(self._areas.values())
+
+    @property
     def map_inc_lanelets_to_intersections(self) -> Dict[int, Intersection]:
         """
-        :returns: dict that maps lanelet ids to the intersection of which it is an incoming lanelet.
+        dict that maps lanelet ids to the intersection of which it is an incoming lanelet.
         """
         return {l_id: intersection for intersection in self.intersections for l_id in
                 list(intersection.map_incoming_lanelets.keys())}
 
     @classmethod
     def create_from_lanelet_list(cls, lanelets: list, cleanup_ids: bool = False):
         """
@@ -1198,41 +1245,40 @@
         :return: The new lanelet network
         """
         if exclude_lanelet_types is None:
             exclude_lanelet_types = set()
         new_lanelet_network = cls()
         traffic_sign_ids = set()
         traffic_light_ids = set()
+        area_ids = set()
         lanelets = set()
 
-        if shape_input is not None:
-            for la in lanelet_network.lanelets:
-                if la.lanelet_type.intersection(exclude_lanelet_types) == set():
-                    lanelet_polygon = la.polygon.shapely_object
-                    if shape_input.shapely_object.intersects(lanelet_polygon):
-                        for sign_id in la.traffic_signs:
-                            traffic_sign_ids.add(sign_id)
-                        for light_id in la.traffic_lights:
-                            traffic_light_ids.add(light_id)
-                        lanelets.add(la)
-
-        else:
-            for la in lanelet_network.lanelets:
-                if la.lanelet_type.intersection(exclude_lanelet_types) == set():
-                    lanelets.add(la)
-                for sign_id in la.traffic_signs:
-                    traffic_sign_ids.add(sign_id)
-                for light_id in la.traffic_lights:
-                    traffic_light_ids.add(light_id)
+        for la in lanelet_network.lanelets:
+            if len(la.lanelet_type.intersection(
+                    exclude_lanelet_types)) > 0 or shape_input is not None and not \
+                    shape_input.shapely_object.intersects(
+                    la.polygon.shapely_object):
+                continue
+
+            lanelets.add(la)
+            for sign_id in la.traffic_signs:
+                traffic_sign_ids.add(sign_id)
+            for light_id in la.traffic_lights:
+                traffic_light_ids.add(light_id)
+            for area_id in la.adjacent_areas:
+                area_ids.add(area_id)
 
         for sign_id in traffic_sign_ids:
             new_lanelet_network.add_traffic_sign(copy.deepcopy(lanelet_network.find_traffic_sign_by_id(sign_id)), set())
         for light_id in traffic_light_ids:
             new_lanelet_network.add_traffic_light(copy.deepcopy(lanelet_network.find_traffic_light_by_id(light_id)),
                                                   set())
+        for area_id in area_ids:
+            new_lanelet_network.add_area(copy.deepcopy(lanelet_network.find_area_by_id(area_id)),
+                                         set())
         for la in lanelets:
             new_lanelet_network.add_lanelet(copy.deepcopy(la), rtree=False)
         new_lanelet_network._create_strtree()
 
         return new_lanelet_network
 
     def _create_strtree(self):
@@ -1262,16 +1308,16 @@
                                         in self._buffered_polygons.items()}
         self._strtee = STRtree(list(self._buffered_polygons.values()))
 
     def remove_lanelet(self, lanelet_id: int, rtree: bool = True):
         """
         Removes a lanelet from a lanelet network and deletes all references.
 
-        @param lanelet_id: ID of lanelet which should be removed.
-        @param rtree: Boolean indicating whether rtree should be initialized
+        :param lanelet_id: ID of lanelet which should be removed.
+        :param rtree: Boolean indicating whether rtree should be initialized
         """
         if lanelet_id in self._lanelets.keys():
             del self._lanelets[lanelet_id]
             del self._buffered_polygons[lanelet_id]
             self.cleanup_lanelet_references()
 
         if rtree:
@@ -1302,15 +1348,15 @@
                 inc._successors_left = set(inc.successors_left).intersection(existing_ids)
             inter._crossings = set(inter.crossings).intersection(existing_ids)
 
     def remove_traffic_sign(self, traffic_sign_id: int):
         """
         Removes a traffic sign from a lanelet network and deletes all references.
 
-        @param traffic_sign_id: ID of traffic sign which should be removed.
+        :param traffic_sign_id: ID of traffic sign which should be removed.
         """
         if traffic_sign_id in self._traffic_signs.keys():
             del self._traffic_signs[traffic_sign_id]
             self.cleanup_traffic_sign_references()
 
     def cleanup_traffic_sign_references(self):
         """
@@ -1322,15 +1368,15 @@
             if la.stop_line is not None and la.stop_line.traffic_sign_ref is not None:
                 la.stop_line._traffic_sign_ref = la.stop_line.traffic_sign_ref.intersection(existing_ids)
 
     def remove_traffic_light(self, traffic_light_id: int):
         """
         Removes a traffic light from a lanelet network and deletes all references.
 
-        @param traffic_light_id: ID of traffic sign which should be removed.
+        :param traffic_light_id: ID of traffic sign which should be removed.
         """
         if traffic_light_id in self._traffic_lights.keys():
             del self._traffic_lights[traffic_light_id]
         self.cleanup_traffic_light_references()
 
     def cleanup_traffic_light_references(self):
         """
@@ -1338,19 +1384,28 @@
         """
         existing_ids = set(self._traffic_lights.keys())
         for la in self.lanelets:
             la._traffic_lights = la.traffic_lights.intersection(existing_ids)
             if la.stop_line is not None and la.stop_line.traffic_light_ref is not None:
                 la.stop_line._traffic_light_ref = la.stop_line.traffic_light_ref.intersection(existing_ids)
 
+    def remove_area(self, area_id: int):
+        """
+        Removes an area from a lanelet network and deletes all references.
+
+        @param area_id: ID of area which should be removed.
+        """
+        if area_id in self._areas.keys():
+            del self._areas[area_id]
+
     def remove_intersection(self, intersection_id: int):
         """
-        Removes a intersection from a lanelet network and deletes all references.
+        Removes an intersection from a lanelet network and deletes all references.
 
-        @param intersection_id: ID of intersection which should be removed.
+        :param intersection_id: ID of intersection which should be removed.
         """
         if intersection_id in self._intersections.keys():
             del self._intersections[intersection_id]
 
     def find_lanelet_by_id(self, lanelet_id: int) -> Lanelet:
         """
         Finds a lanelet for a given lanelet_id
@@ -1385,14 +1440,27 @@
         """
         assert is_natural_number(
                 traffic_light_id), '<LaneletNetwork/find_traffic_light_by_id>: provided id is not valid! ' \
                                    'id = {}'.format(traffic_light_id)
 
         return self._traffic_lights[traffic_light_id] if traffic_light_id in self._traffic_lights else None
 
+    def find_area_by_id(self, area_id: int) -> Area:
+        """
+        Finds an area for a given area id
+
+        :param area_id: The id of the area to find
+        :return: The area object if the id exists and None otherwise
+        """
+        assert is_natural_number(
+                area_id), '<LaneletNetwork/find_area_by_id>: provided id is not valid! ' \
+                          'id = {}'.format(area_id)
+
+        return self._areas[area_id] if area_id in self._areas else None
+
     def find_intersection_by_id(self, intersection_id: int) -> Intersection:
         """
         Finds a intersection for a given intersection_id
 
         :param intersection_id: The id of the intersection to find
         :return: The intersection object if the id exists and None otherwise
         """
@@ -1474,14 +1542,41 @@
                 lanelet = self.find_lanelet_by_id(lanelet_id)
                 if lanelet is not None:
                     lanelet.add_traffic_light_to_lanelet(traffic_light.traffic_light_id)
                 else:
                     warnings.warn('Traffic light cannot be referenced to lanelet because the lanelet does not exist.')
             return True
 
+    def add_area(self, area: Area, lanelet_ids: Set[int]):
+        """
+        Adds an area to the LaneletNetwork
+
+        :param area: The area to add
+        :param lanelet_ids: Lanelets the area should be referenced from
+        :return: True if the area has successfully been added to the network, false otherwise
+        """
+
+        assert isinstance(area, Area), '<LaneletNetwork/add_area>: provided area ' \
+                                       'is not of type area! ' \
+                                       'type = {}'.format(type(area))
+
+        # check if adjacent area already exists in network and warn user
+        if area.area_id in self._areas.keys():
+            warnings.warn('Area already exists in network! No changes are made.')
+            return False
+        else:
+            self._areas[area.area_id] = area
+            for lanelet_id in lanelet_ids:
+                lanelet = self.find_lanelet_by_id(lanelet_id)
+                if lanelet is not None:
+                    lanelet.add_adjacent_area_to_lanelet(area.area_id)
+                else:
+                    warnings.warn('Area cannot be referenced to lanelet because the lanelet does not exist.')
+            return True
+
     def add_intersection(self, intersection: Intersection):
         """
         Adds an intersection to the LaneletNetwork
 
         :param intersection: The intersection to add
         :return: True if the traffic light has successfully been added to the network, false otherwise
         """
@@ -1541,25 +1636,26 @@
 
         :param point_list: The list of positions to check
         :return: A list of lanelet ids. If the position could not be matched to a lanelet, an empty list is returned
         """
         assert isinstance(point_list,
                           ValidTypes.LISTS), '<Lanelet/contains_points>: provided list of points is not a list! type ' \
                                              '= {}'.format(type(point_list))
-
-        res = []
-        for point in point_list:
-            shapely_point = ShapelyPoint(point)
-            inner_res = []
-            for idx in self._strtee.query(shapely_point):
-                lanelet_shapely_polygon = self._strtee.geometries[idx]
-                if lanelet_shapely_polygon.intersects(shapely_point) \
-                        or lanelet_shapely_polygon.buffer(1e-15).intersects(shapely_point):
-                    inner_res.append(self._get_lanelet_id_by_shapely_polygon(lanelet_shapely_polygon))
-            res.append(inner_res)
+        shapely_points = [ShapelyPoint(p) for p in point_list]
+        # Accepted tolerance
+        tolerance = 1.0e-15
+        geometry_ids = self._strtee.query(shapely_points, predicate="dwithin", distance=tolerance)
+        # Convert from [[input_index, str_geometry_id], ...] to
+        # [[lanlet_id, ...], ...]
+        lanelet_ids = defaultdict(list)
+        for input_id, geom_id in zip(*geometry_ids):
+            lanelet_shapely_polygon = self._strtee.geometries[geom_id]
+            lanelet_id = self._get_lanelet_id_by_shapely_polygon(lanelet_shapely_polygon)
+            lanelet_ids[input_id].append(lanelet_id)
+        res = [lanelet_ids[i] for i, _ in enumerate(point_list)]
         return res
 
     def find_lanelet_by_shape(self, shape: Shape) -> List[int]:
         """
         Finds the lanelet id of a given shape
 
         :param shape: The shape to check
```

### Comparing `commonroad_io-2023.1/commonroad/scenario/obstacle.py` & `commonroad_io-2023.2/commonroad/scenario/obstacle.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import enum
 import warnings
 import math
 import numpy as np
-from typing import Union, Set, List, Optional, Tuple
+from typing import Union, Set, List, Dict, Optional, Tuple
 from abc import abstractmethod
 
-import numpy as np
 
 from commonroad.common.validity import is_valid_orientation, is_real_number_vector, is_real_number
 from commonroad.geometry.shape import Shape, \
     Rectangle, \
     Circle, \
     Polygon, \
     ShapeGroup, \
@@ -49,14 +48,77 @@
     MOTORCYCLE = "motorcycle"
     TAXI = "taxi"
     BUILDING = "building"
     PILLAR = "pillar"
     MEDIAN_STRIP = "median_strip"
 
 
+class MetaInformationState:
+    """
+    Class that keeps the meta information state of an obstacle.
+    It freely allows to set attributes on a dynamic obstacle.
+    """
+    def __init__(self, meta_data_str: Dict[str, str] = None, meta_data_int: Dict[str, int] = None,
+                 meta_data_float: Dict[str, float] = None, meta_data_bool: Dict[str, bool] = None):
+        """
+        :param meta_data_str: dictionary of a key and a string
+        :param meta_data_int: dictionary of a key and an int
+        :param meta_data_float: dictionary of a key and a float
+        :param meta_data_bool: dictionary of a key and a bool
+        """
+        self._meta_data_str = meta_data_str
+        self._meta_data_int = meta_data_int
+        self._meta_data_float = meta_data_float
+        self._meta_data_bool = meta_data_bool
+
+    @property
+    def meta_data_str(self) -> Dict[str, str]:
+        """ Dictionary of a key and a string. """
+        return self._meta_data_str
+
+    @meta_data_str.setter
+    def meta_data_str(self, meta_data_str: Dict[str, str]):
+        assert isinstance(meta_data_str, Dict), '<MetaInformationState/meta_data_str>: Provided meta_data_str ' \
+                                                'is not valid! id={}'.format(meta_data_str)
+        self._meta_data_str = meta_data_str
+
+    @property
+    def meta_data_int(self) -> Dict[str, int]:
+        """ Dictionary of a key and an int. """
+        return self._meta_data_int
+
+    @meta_data_int.setter
+    def meta_data_int(self, meta_data_int: Dict[str, int]):
+        assert isinstance(meta_data_int, Dict), '<MetaInformationState/meta_data_int>: Provided meta_data_int ' \
+                                                'is not valid! id={}'.format(meta_data_int)
+        self._meta_data_int = meta_data_int
+
+    @property
+    def meta_data_float(self) -> Dict[str, float]:
+        """ Dictionary of a key and a float. """
+        return self._meta_data_float
+
+    @meta_data_float.setter
+    def meta_data_float(self, meta_data_float: Dict[str, float]):
+        assert isinstance(meta_data_float, Dict), '<MetaInformationState/meta_data_float>: Provided meta_data_float ' \
+                                                'is not valid! id={}'.format(meta_data_float)
+        self._meta_data_float = meta_data_float
+
+    @property
+    def meta_data_bool(self) -> Dict[str, bool]:
+        """ Dictionary of a key and a bool. """
+        return self._meta_data_bool
+
+    @meta_data_bool.setter
+    def meta_data_bool(self, meta_data_bool: Dict[str, bool]):
+        assert isinstance(meta_data_bool, Dict), '<MetaInformationState/meta_data_bool>: Provided meta_data_bool ' \
+                                                'is not valid! id={}'.format(meta_data_bool)
+        self._meta_data_bool = meta_data_bool
+
+
 class SignalState:
     """ A signal state is a boolean value indicating the activity of the signal source at a time step.
         The possible signal state elements are defined as slots:
 
         :ivar horn: boolean indicating activity of horn
         :ivar indicator_left: boolean indicating activity of left indicator
         :ivar indicator_right: boolean indicating activity of right indicator
@@ -424,50 +486,65 @@
 
 class DynamicObstacle(Obstacle):
     """ Class representing dynamic obstacles as defined in CommonRoad. Each dynamic obstacle has stored its predicted
     movement in future time steps.
     """
 
     def __init__(self, obstacle_id: int, obstacle_type: ObstacleType,
-                 obstacle_shape: Shape, initial_state: TraceState,
+                 obstacle_shape: Shape,
+                 initial_state: TraceState,
                  prediction: Union[None, Prediction, TrajectoryPrediction, SetBasedPrediction] = None,
                  initial_center_lanelet_ids: Union[None, Set[int]] = None,
                  initial_shape_lanelet_ids: Union[None, Set[int]] = None,
-                 initial_signal_state: Union[None, SignalState] = None, signal_series: List[SignalState] = None,
+                 initial_signal_state: Union[None, SignalState] = None,
+                 signal_series: List[SignalState] = None,
+                 initial_meta_information_state: MetaInformationState = None,
+                 meta_information_series: List[MetaInformationState] = None,
+                 external_dataset_id: int = None,
                  **kwargs):
         """
             :param obstacle_id: unique ID of the obstacle
             :param obstacle_type: type of obstacle (e.g. PARKED_VEHICLE)
             :param obstacle_shape: shape of the static obstacle
             :param initial_state: initial state of the static obstacle
             :param prediction: predicted movement of the dynamic obstacle
             :param initial_center_lanelet_ids: initial IDs of lanelets the obstacle center is on
             :param initial_shape_lanelet_ids: initial IDs of lanelets the obstacle shape is on
             :param initial_signal_state: initial signal state of static obstacle
             :param signal_series: list of signal states over time
             :param wheelbase: list of wheelbase lengths
+            :param initial_meta_information_state: meta information of the dynamic obstacle
+            :param meta_information_series: list of meta information
+            :param external_dataset_id: ID of the external dataset
         """
         for (field, value) in kwargs.items():
             setattr(self, field, value)
         Obstacle.__init__(self, obstacle_id=obstacle_id, obstacle_role=ObstacleRole.DYNAMIC,
                           obstacle_type=obstacle_type, obstacle_shape=obstacle_shape, initial_state=initial_state,
                           initial_center_lanelet_ids=initial_center_lanelet_ids,
                           initial_shape_lanelet_ids=initial_shape_lanelet_ids,
                           initial_signal_state=initial_signal_state, signal_series=signal_series)
         self.prediction: Prediction = prediction
+        self.initial_meta_information_state = initial_meta_information_state
+        self.meta_information_series = meta_information_series
+        self.external_dataset_id = external_dataset_id
 
     def __eq__(self, other):
         if not isinstance(other, DynamicObstacle):
             warnings.warn(f"Inequality between DynamicObstacle {repr(self)} and different type {type(other)}")
             return False
 
-        return self._prediction == other.prediction and Obstacle.__eq__(self, other)
+        return self._prediction == other.prediction and Obstacle.__eq__(self, other) and \
+            self._initial_meta_information_state == other.initial_meta_information_state and \
+            self._meta_information_series == other.meta_information_series and \
+            self._external_dataset_id == other.external_dataset_id
 
     def __hash__(self):
-        return hash((self._prediction, Obstacle.__hash__(self)))
+        return hash((self._prediction, self._initial_meta_information_state, self._meta_information_series,
+                     self._external_dataset_id, Obstacle.__hash__(self)))
 
     @property
     def initial_state(self) -> State:
         """ Initial state of the obstacle, e.g., obtained through sensor measurements."""
         return self._initial_state
 
     @initial_state.setter
@@ -490,14 +567,54 @@
     @prediction.setter
     def prediction(self, prediction: Union[Prediction, TrajectoryPrediction, SetBasedPrediction,  None]):
         assert isinstance(prediction, (Prediction, type(None))), '<DynamicObstacle/prediction>: argument prediction ' \
                                                                  'of wrong type. Expected types: %s, %s. Got type: ' \
                                                                  '%s.' % (Prediction, type(None), type(prediction))
         self._prediction = prediction
 
+    @property
+    def initial_meta_information_state(self) -> Union[None, MetaInformationState]:
+        """ Meta information of the dynamic obstacle. """
+        return self._initial_meta_information_state
+
+    @initial_meta_information_state.setter
+    def initial_meta_information_state(self, initial_meta_information_state: Union[MetaInformationState, None]):
+        assert isinstance(initial_meta_information_state, (MetaInformationState, type(None))), \
+            '<DynamicObstacle/initial_meta_information_state>: argument prediction ' \
+            'of wrong type. Expected types: %s, %s. Got type: %s.' \
+            % (MetaInformationState, type(None), type(initial_meta_information_state))
+
+        self._initial_meta_information_state = initial_meta_information_state
+
+    @property
+    def meta_information_series(self) -> Union[None, List[MetaInformationState]]:
+        """ List of meta information."""
+        return self._meta_information_series
+
+    @meta_information_series.setter
+    def meta_information_series(self, meta_information_series: Union[List[MetaInformationState], None]):
+        assert isinstance(meta_information_series, (List, type(None))), \
+            '<DynamicObstacle/meta_information_series>: argument prediction ' \
+            'of wrong type. Expected types: %s, %s. Got type: %s.' \
+            % (List, type(None), type(meta_information_series))
+
+        self._meta_information_series = meta_information_series
+
+    @property
+    def external_dataset_id(self) -> Union[int, None]:
+        """ ID of the external dataset."""
+        return self._external_dataset_id
+
+    @external_dataset_id.setter
+    def external_dataset_id(self, external_dataset_id: Union[int, None]):
+        assert isinstance(external_dataset_id, (int, type(None))), \
+            '<DynamicObstacle/external_dataset_id>: argument prediction of wrong type. ' \
+            'Expected types: %s, %s. Got type: %s.' % (int, type(None), type(external_dataset_id))
+        self._external_dataset_id = external_dataset_id
+
     def occupancy_at_time(self, time_step: int) -> Union[None, Occupancy]:
         """
         Returns the predicted occupancy of the obstacle at a specific time step.
 
         :param time_step: discrete time step
         :return: predicted occupancy of the obstacle at time step
         """
```

### Comparing `commonroad_io-2023.1/commonroad/scenario/scenario.py` & `commonroad_io-2023.2/commonroad/scenario/scenario.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,27 +5,28 @@
 from collections import defaultdict
 from typing import Union, List, Set, Dict, Tuple
 
 import iso3166
 import numpy as np
 
 from commonroad import SCENARIO_VERSION, SUPPORTED_COMMONROAD_VERSIONS
-from commonroad.common.util import Interval
+from commonroad.common.util import Interval, Time
 from commonroad.common.validity import is_real_number, is_real_number_vector, is_valid_orientation, is_natural_number, \
     is_integer_number
 from commonroad.prediction.prediction import Occupancy, SetBasedPrediction, TrajectoryPrediction
 from commonroad.scenario.intersection import Intersection
 from commonroad.scenario.lanelet import Lanelet
 from commonroad.scenario.lanelet import LaneletNetwork
 from commonroad.scenario.obstacle import ObstacleRole
 from commonroad.scenario.obstacle import ObstacleType
 from commonroad.scenario.obstacle import StaticObstacle, DynamicObstacle, EnvironmentObstacle, Obstacle, \
     PhantomObstacle
 from commonroad.scenario.state import TraceState
-from commonroad.scenario.traffic_sign import TrafficSign, TrafficLight
+from commonroad.scenario.traffic_sign import TrafficSign
+from commonroad.scenario.traffic_light import TrafficLight
 from commonroad.visualization.drawable import IDrawable
 from commonroad.visualization.renderer import IRenderer
 from commonroad.visualization.draw_params import OptionalSpecificOrAllDrawParams, MPDrawParams
 
 
 @enum.unique
 class Tag(enum.Enum):
@@ -59,28 +60,33 @@
     TWO_LANE = "two_lane"
     EMERGENCY_BRAKING = "emergency_braking"
 
 
 @enum.unique
 class TimeOfDay(enum.Enum):
     """ Enum containing all possible time of days."""
-    DAY = "day"
     NIGHT = "night"
+    SUNSET = "sunset"
+    AFTERNOON = "afternoon"
+    NOON = "noon"
+    MORNING = "morning"
     UNKNOWN = "unknown"
 
 
 @enum.unique
 class Weather(enum.Enum):
     """ Enum containing all possible weathers."""
-    SUNNY = "sunny"
+    CLEAR = "clear"
     LIGHT_RAIN = "light_rain"
+    MID_RAIN = "mid_rain"
     HEAVY_RAIN = "heavy_rain"
     FOG = "fog"
     SNOW = "snow"
     HAIL = "hail"
+    CLOUDY = "cloudy"
     UNKNOWN = "unknown"
 
 
 @enum.unique
 class Underground(enum.Enum):
     """ Enum containing all possible undergrounds."""
     WET = "wet"
@@ -88,55 +94,14 @@
     DIRTY = "dirty"
     DAMAGED = "damaged"
     SNOW = "snow"
     ICE = "ice"
     UNKNOWN = "unknown"
 
 
-class Time:
-    """
-    Class which describes the fictive time when a scenario starts.
-    """
-
-    def __init__(self, hours: int, minutes: int):
-        """
-        Constructor of a time object
-
-        :param hours: hours at start of scenario (0-24)
-        :param minutes: minutes at start of scenario (0-60)
-        """
-        self._hours = hours
-        self._minutes = minutes
-
-    def __eq__(self, other):
-        if not isinstance(other, Time):
-            return False
-
-        return self._hours == other.hours and self._minutes == other.minutes
-
-    def __hash__(self):
-        return hash((self._hours, self._minutes))
-
-    @property
-    def hours(self) -> int:
-        return self._hours
-
-    @hours.setter
-    def hours(self, hours: int):
-        self._hours = hours
-
-    @property
-    def minutes(self) -> int:
-        return self._minutes
-
-    @minutes.setter
-    def minutes(self, minutes: int):
-        self._minutes = minutes
-
-
 class GeoTransformation:
     """
     Class which describes the transformation from geodetic to projected Cartesian coordinates according to the
     CommonRoad specification
     """
 
     def __init__(self, geo_reference: str = None, x_translation: float = None, y_translation: float = None,
```

### Comparing `commonroad_io-2023.1/commonroad/scenario/state.py` & `commonroad_io-2023.2/commonroad/scenario/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,51 +90,51 @@
         return np.array(values)
 
     @property
     def attributes(self) -> List[str]:
         """
         Returns all attributes used in state space.
 
-        :return: Attributes
+        Attributes
         """
         fields = self.__dict__
 
         return [field_name for field_name in fields]
 
     @property
     def used_attributes(self) -> List[str]:
         """
         Returns all initialized attributed in state space.
 
-        :return: Initialized attributes
+        Initialized attributes
         """
         used_fields = list()
         for field_name in self.attributes:
             if getattr(self, field_name) is not None:
                 used_fields.append(field_name)
 
         return used_fields
 
     @property
     def is_uncertain_position(self) -> bool:
         """
         Checks whether the position is uncertain.
 
-        :return: Uncertain or not
+        Uncertain or not
         """
         if hasattr(self, "position"):
             return isinstance(getattr(self, "position"), Shape)
         return False
 
     @property
     def is_uncertain_orientation(self):
         """
         Checks whether the orientation is uncertain.
 
-        :return: Uncertain or not
+        Uncertain or not
         """
         if hasattr(self, "orientation"):
             return isinstance(getattr(self, "orientation"), AngleInterval)
         return False
 
     def has_value(self, attr: str) -> bool:
         """
```

### Comparing `commonroad_io-2023.1/commonroad/scenario/traffic_sign.py` & `commonroad_io-2023.2/commonroad/scenario/traffic_sign.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import List, Set
 import numpy as np
 
 import commonroad.geometry.transform
 from commonroad.common.validity import *
 from commonroad.visualization.drawable import IDrawable
 from commonroad.visualization.renderer import IRenderer
-from commonroad.visualization.draw_params import TrafficLightParams, TrafficSignParams, OptionalSpecificOrAllDrawParams
+from commonroad.visualization.draw_params import TrafficSignParams, OptionalSpecificOrAllDrawParams
 
 TRAFFIC_SIGN_VALIDITY_START = {'WARNING_DANGER_SPOT', 'WARNING_RIGHT_BEFORE_LEFT', 'WARNING_STEEP_HILL_DOWNWARDS',
                                'WARNING_SLIPPERY_ROAD', 'WARNING_CONSTRUCTION_SITE', 'WARNING_CROSSING_CYCLIST',
                                'WARNING_ANIMAL_CROSSING_RIGHT', 'RAILWAY', 'PRIORITY_OPPOSITE_DIRECTION',
                                'TURN_RIGHT_AHEAD', 'TURN_LEFT_AHEAD', 'ONEWAY_RIGHT', 'ONEWAY_LEFT',
                                'PRESCRIBED_PASSING_LEFT', 'PRESCRIBED_PASSING_RIGHT', 'BIKEWAY', 'PEDESTRIAN_SIDEWALK',
                                'PEDESTRIAN_ZONE_START', 'BICYCLE_ROAD_START', 'BUS_LANE', 'BAN_ALL_VEHICLES',
@@ -637,40 +637,14 @@
 
 @enum.unique
 class TrafficSignIDPuertoRico(enum.Enum):
     MAX_SPEED = '274'  # TODO: change to actual ID
     UNKNOWN = ''  # TODO: add actual IDs
 
 
-@enum.unique
-class TrafficLightDirection(enum.Enum):
-    """
-    Enum for all the possible directions for a traffic signal
-    """
-    RIGHT = "right"
-    STRAIGHT = "straight"
-    LEFT = "left"
-    LEFT_STRAIGHT = "leftStraight"
-    STRAIGHT_RIGHT = "straightRight"
-    LEFT_RIGHT = "leftRight"
-    ALL = "all"
-
-
-@enum.unique
-class TrafficLightState(enum.Enum):
-    """
-    Enum for the possible types of traffic light in signals
-    """
-    RED = "red"
-    YELLOW = "yellow"
-    RED_YELLOW = "redYellow"
-    GREEN = "green"
-    INACTIVE = "inactive"
-
-
 class TrafficSignElement:
     """ Class which represents a collection of traffic signs at one position"""
 
     def __init__(self, traffic_sign_element_id: Union[
         TrafficSignIDZamunda, TrafficSignIDUsa, TrafficSignIDSpain, TrafficSignIDGermany, TrafficSignIDChina,
         TrafficSignIDRussia],
                  additional_values: List[str] = []):
@@ -724,22 +698,22 @@
         self._additional_values = additional_values
 
 
 class TrafficSign(IDrawable):
     """Class to represent a traffic sign"""
 
     def __init__(self, traffic_sign_id: int, traffic_sign_elements: List[TrafficSignElement],
-                 first_occurrence: Set[int], position: np.ndarray = None, virtual: bool = False):
+                 first_occurrence: Set[int], position: np.ndarray, virtual: bool = False):
         """
         :param traffic_sign_id: ID of traffic sign
         :param traffic_sign_elements: list of traffic sign elements
         :param first_occurrence: lanelet ID where traffic sign first appears
         :param position: position of traffic sign
         :param virtual: boolean indicating if this traffic sign is also
-        placed there in the real environment or it
+        placed there in the real environment, or it
         is added for other reasons (e.g., completeness of scenario)
         """
         self._traffic_sign_id = traffic_sign_id
         self._position = position
         self._traffic_sign_elements = traffic_sign_elements
         self._virtual = virtual
         self._first_occurrence = first_occurrence
@@ -758,56 +732,53 @@
         for k in traffic_sign_elements.keys():
             if k not in traffic_sign_elements_other:
                 traffic_sign_eq = False
                 continue
             if traffic_sign_elements.get(k) != traffic_sign_elements_other.get(k):
                 list_elements_eq = False
 
-        position_string = None if self._position is None else \
-            np.array2string(np.around(self._position.astype(float), 10), precision=10)
-        position_other_string = None if other._position is None else \
-            np.array2string(np.around(other.position.astype(float), 10), precision=10)
+        position_string = np.array2string(np.around(self._position.astype(float), 10), precision=10)
+        position_other_string = np.array2string(np.around(other.position.astype(float), 10), precision=10)
 
         if traffic_sign_eq and self._traffic_sign_id == other.traffic_sign_id \
                 and position_string == position_other_string and self._virtual == other.virtual \
                 and self._first_occurrence == other.first_occurrence:
             return list_elements_eq
 
         warnings.warn(f"Inequality of TrafficSign {repr(self)} and the other one {repr(other)}")
         return False
 
     def __hash__(self):
-        position_string = None if self._position is None else \
-            np.array2string(np.around(self._position.astype(float), 10), precision=10)
+        position_string = np.array2string(np.around(self._position.astype(float), 10), precision=10)
         return hash((self._traffic_sign_id, position_string, frozenset(self._traffic_sign_elements), self._virtual,
                      frozenset(self._first_occurrence)))
 
     def __str__(self):
         return f"TrafficSign with id {self._traffic_sign_id} placed at {self._position}"
 
     def __repr__(self):
         return f"TrafficSign(traffic_sign_id={self._traffic_sign_id}, " \
                f"traffic_sign_elements={repr(self._traffic_sign_elements)}, " \
                f"first_occurrence={self._first_occurrence}, " \
-               f"position={None if self._position is None else self._position.tolist()}, virtual={self._virtual})"
+               f"position={self._position.tolist()}, virtual={self._virtual})"
 
     @property
     def traffic_sign_id(self) -> int:
         return self._traffic_sign_id
 
     @traffic_sign_id.setter
     def traffic_sign_id(self, traffic_sign_id: int):
         self._traffic_sign_id = traffic_sign_id
 
     @property
-    def position(self) -> Union[None, np.ndarray]:
+    def position(self) -> np.ndarray:
         return self._position
 
     @position.setter
-    def position(self, position: Union[None, np.ndarray]):
+    def position(self, position: np.ndarray):
         self._position = position
 
     @property
     def traffic_sign_elements(self) -> List[TrafficSignElement]:
         return self._traffic_sign_elements
 
     @traffic_sign_elements.setter
@@ -849,213 +820,7 @@
                                             'within the ' \
                                             'interval [-2pi, 2pi]. angle = %s' % angle
         self._position = commonroad.geometry.transform.translate_rotate(np.array([self._position]), translation, angle)[
             0]
 
     def draw(self, renderer: IRenderer, draw_params: OptionalSpecificOrAllDrawParams[TrafficSignParams] = None):
         renderer.draw_traffic_light_sign(self, draw_params)
-
-
-class TrafficLightCycleElement:
-    """Class to represent a traffic light cycle"""
-
-    def __init__(self, state: TrafficLightState, duration: int):
-        """
-        :param state: state of a traffic light cycle element
-        :param duration: duration of traffic light cycle element
-        """
-        self._state = state
-        self._duration = duration
-
-    def __eq__(self, other):
-        if not isinstance(other, TrafficLightCycleElement):
-            warnings.warn(f"Inequality between TrafficLightCycleElement {repr(self)} and different type {type(other)}")
-            return False
-
-        if self._state == other.state and self._duration == other.duration:
-            return True
-
-        warnings.warn(f"Inequality of TrafficLightCycleElement {repr(self)} and the other one {repr(other)}")
-        return False
-
-    def __hash__(self):
-        return hash((self._state, self._duration))
-
-    def __str__(self):
-        return f"TrafficLightCycleElement with state {self._state} and duration {self._duration}"
-
-    def __repr__(self):
-        return f"TrafficLightCycleElement(state={self._state}, duration={self._duration})"
-
-    @property
-    def state(self) -> TrafficLightState:
-        return self._state
-
-    @state.setter
-    def state(self, state: TrafficLightState):
-        self._state = state
-
-    @property
-    def duration(self) -> int:
-        return self._duration
-
-    @duration.setter
-    def duration(self, duration: int):
-        self._duration = duration
-
-
-class TrafficLight(IDrawable):
-    """ Class to represent a traffic light"""
-
-    def __init__(self, traffic_light_id: int, cycle: List[TrafficLightCycleElement], position: np.ndarray = None,
-                 time_offset: int = 0, direction: TrafficLightDirection = TrafficLightDirection.ALL,
-                 active: bool = True):
-        """
-        :param traffic_light_id: ID of traffic light
-        :param cycle: list of traffic light cycle elements
-        :param time_offset: offset of traffic light cycle
-        :param position: position of traffic light
-        :param direction: driving directions for which the traffic light is valid
-        :param active: boolean indicating if traffic light is currently active
-        """
-        self._traffic_light_id = traffic_light_id
-        if len(cycle) == 0:
-            self._cycle = get_default_cycle()
-        else:
-            self._cycle = cycle
-        self._time_offset = time_offset
-        self._position = position
-        self._direction = direction
-        self._active = active
-
-    def __eq__(self, other):
-        if not isinstance(other, TrafficLight):
-            warnings.warn(f"Inequality between TrafficLight {repr(self)} and different type {type(other)}")
-            return False
-
-        position_string = None if self._position is None else \
-            np.array2string(np.around(self._position.astype(float), 10), precision=10)
-        position_other_string = None if other._position is None else \
-            np.array2string(np.around(other.position.astype(float), 10), precision=10)
-
-        if self._traffic_light_id == other.traffic_light_id and set(self._cycle) == set(other.cycle) \
-                and self._time_offset == other.time_offset and position_string == position_other_string \
-                and self._direction == other.direction and self._active == other.active:
-            return True
-
-        warnings.warn(f"Inequality of TrafficLight {repr(self)} and the other one {repr(other)}")
-        return False
-
-    def __hash__(self):
-        position_string = None if self._position is None else \
-            np.array2string(np.around(self._position.astype(float), 10), precision=10)
-        return hash((self._traffic_light_id, frozenset(self._cycle), self._time_offset, position_string,
-                     self._direction, self._active))
-
-    def __str__(self):
-        return f"TrafficLight with id {self._traffic_light_id} placed at {self._position}"
-
-    def __repr__(self):
-        return f"TrafficLight(traffic_light_id={self._traffic_light_id}, cycle={repr(self._cycle)}, " \
-               f"time_offset={self._time_offset}, " \
-               f"position={None if self._position is None else self._position.tolist()}, " \
-               f"direction={self._direction}, active={self._active})"
-
-    @property
-    def traffic_light_id(self) -> int:
-        return self._traffic_light_id
-
-    @traffic_light_id.setter
-    def traffic_light_id(self, traffic_light_id: int):
-        self._traffic_light_id = traffic_light_id
-
-    @property
-    def cycle(self) -> List[TrafficLightCycleElement]:
-        return self._cycle
-
-    @cycle.setter
-    def cycle(self, cycle: List[TrafficLightCycleElement]):
-        self._cycle = cycle
-
-    def get_state_at_time_step(self, time_step: int) -> TrafficLightState:
-        time_step_mod = ((time_step - self.time_offset) % (
-                    self.cycle_init_timesteps[-1] - self.time_offset)) + self.time_offset
-        i_cycle = np.argmax(time_step_mod < self.cycle_init_timesteps) - 1
-        return self.cycle[i_cycle].state
-
-    @property
-    def cycle_init_timesteps(self):
-        if not hasattr(self, '_cycle_init_timesteps'):
-            durations = [cycle_el.duration for cycle_el in self._cycle]
-            self._cycle_init_timesteps = np.cumsum(durations) + self.time_offset
-            self._cycle_init_timesteps = np.insert(self._cycle_init_timesteps, 0, self.time_offset)
-        return self._cycle_init_timesteps
-
-    @property
-    def time_offset(self) -> int:
-        return self._time_offset
-
-    @time_offset.setter
-    def time_offset(self, time_offset: int):
-        self._time_offset = time_offset
-
-    @property
-    def position(self) -> np.ndarray:
-        return self._position
-
-    @position.setter
-    def position(self, position: np.ndarray):
-        self._position = position
-
-    @property
-    def direction(self) -> TrafficLightDirection:
-        return self._direction
-
-    @direction.setter
-    def direction(self, direction: TrafficLightDirection):
-        self._direction = direction
-
-    @property
-    def active(self) -> bool:
-        return self._active
-
-    @active.setter
-    def active(self, active: bool):
-        self._active = active
-
-    def translate_rotate(self, translation: np.ndarray, angle: float):
-        """
-        This method translates and rotates a traffic light
-
-        :param translation: The translation given as [x_off,y_off] for the x and y translation
-        :param angle: The rotation angle in radian (counter-clockwise defined)
-        """
-
-        assert is_real_number_vector(translation, 2), '<TrafficLight/translate_rotate>: ' \
-                                                      'argument translation is ' \
-                                                      'not a vector of real numbers of ' \
-                                                      'length 2.'
-        assert is_real_number(angle), '<TrafficLight/translate_rotate>: argument angle must ' \
-                                      'be ' \
-                                      'a scalar. ' \
-                                      'angle = %s' % angle
-        assert is_valid_orientation(angle), '<TrafficLight/translate_rotate>: argument angle must ' \
-                                            'be ' \
-                                            'within the ' \
-                                            'interval [-2pi, 2pi]. angle = %s' % angle
-        self._position = commonroad.geometry.transform.translate_rotate(np.array([self._position]), translation, angle)[
-            0]
-
-    def draw(self, renderer: IRenderer, draw_params: OptionalSpecificOrAllDrawParams[TrafficLightParams] = None):
-        renderer.draw_traffic_light_sign(self, draw_params)
-
-
-def get_default_cycle():
-    """
-    Defines default traffic light cycle in case no cycle is provided
-
-    _:returns traffic light cycle element
-    """
-    cycle = [(TrafficLightState.RED, 60), (TrafficLightState.RED_YELLOW, 10), (TrafficLightState.GREEN, 60),
-             (TrafficLightState.YELLOW, 10)]
-    cycle_element_list = [TrafficLightCycleElement(state[0], state[1]) for state in cycle]
-    return cycle_element_list
```

### Comparing `commonroad_io-2023.1/commonroad/scenario/traffic_sign_interpreter.py` & `commonroad_io-2023.2/commonroad/scenario/traffic_sign_interpreter.py`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario/trajectory.py` & `commonroad_io-2023.2/commonroad/scenario/trajectory.py`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/convert_xml_to_pb.py` & `commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/convert_xml_to_pb.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import shutil
 from os.path import isfile, join, isdir
 
 from commonroad.common.file_reader import CommonRoadFileReader
-from commonroad.common.file_writer import FileFormat, CommonRoadFileWriter
+from commonroad.common.file_writer import CommonRoadFileWriter
+from commonroad.common.util import FileFormat
 from commonroad.common.writer.file_writer_interface import OverwriteExistingFile
 
 
 def convert_xml_to_pb(src_file_path: str, dest_file_path: str, invalid_conversion_path: str = None):
     """
     Converts CommonRoad file from XML to protobuf format. Invalid converted files can be stored in a desired directory.
```

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/definition_files/commonroad.proto` & `commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/definition_files/commonroad.proto`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/definition_files/dynamic_obstacle.proto` & `commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/definition_files/dynamic_obstacle.proto`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/definition_files/lanelet.proto` & `commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/definition_files/lanelet.proto`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/definition_files/location.proto` & `commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/definition_files/location.proto`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/definition_files/obstacle.proto` & `commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/definition_files/obstacle.proto`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/definition_files/scenario_tags.proto` & `commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/definition_files/scenario_tags.proto`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/definition_files/traffic_light.proto` & `commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/definition_files/traffic_light.proto`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/definition_files/traffic_sign.proto` & `commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/definition_files/traffic_sign.proto`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/definition_files/util.proto` & `commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/definition_files/util.proto`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/commonroad_pb2.py` & `commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/commonroad_pb2.py`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/dynamic_obstacle_pb2.py` & `commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/dynamic_obstacle_pb2.py`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/environment_obstacle_pb2.py` & `commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/environment_obstacle_pb2.py`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/intersection_pb2.py` & `commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/intersection_pb2.py`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/lanelet_pb2.py` & `commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/lanelet_pb2.py`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/location_pb2.py` & `commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/location_pb2.py`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/obstacle_pb2.py` & `commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/obstacle_pb2.py`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/phantom_obstacle_pb2.py` & `commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/phantom_obstacle_pb2.py`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/planning_problem_pb2.py` & `commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/planning_problem_pb2.py`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/scenario_tags_pb2.py` & `commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/scenario_tags_pb2.py`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/static_obstacle_pb2.py` & `commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/static_obstacle_pb2.py`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/traffic_light_pb2.py` & `commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/traffic_light_pb2.py`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/traffic_sign_pb2.py` & `commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/traffic_sign_pb2.py`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/generated_scripts/util_pb2.py` & `commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/generated_scripts/util_pb2.py`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/protobuf_format/how_to_protobuf.md` & `commonroad_io-2023.2/commonroad/scenario_definition/protobuf_format/how_to_protobuf.md`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/xml_definition_files/CommonRoadSolution_schema.xsd` & `commonroad_io-2023.2/commonroad/scenario_definition/xml_definition_files/CommonRoadSolution_schema.xsd`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/scenario_definition/xml_definition_files/XML_commonRoad_XSD.xsd` & `commonroad_io-2023.2/commonroad/scenario_definition/xml_definition_files/XML_commonRoad_XSD.xsd`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/draw_params.py` & `commonroad_io-2023.2/commonroad/visualization/draw_params.py`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/drawable.py` & `commonroad_io-2023.2/commonroad/visualization/drawable.py`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/icons.py` & `commonroad_io-2023.2/commonroad/visualization/icons.py`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/mp_renderer.py` & `commonroad_io-2023.2/commonroad/visualization/mp_renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,20 +21,23 @@
 import commonroad.prediction.prediction
 import commonroad.scenario.obstacle
 from commonroad.common.util import Interval
 from commonroad.geometry.shape import *
 from commonroad.planning.goal import GoalRegion
 from commonroad.planning.planning_problem import PlanningProblemSet, PlanningProblem
 from commonroad.prediction.prediction import Occupancy, TrajectoryPrediction
-from commonroad.scenario.lanelet import LaneletNetwork, LineMarking
+from commonroad.scenario.lanelet import LaneletNetwork
+from commonroad.common.common_lanelet import LineMarking
 from commonroad.scenario.obstacle import DynamicObstacle, StaticObstacle, SignalState, PhantomObstacle, \
     EnvironmentObstacle, Obstacle
 from commonroad.scenario.scenario import Scenario
 from commonroad.scenario.state import TraceState
-from commonroad.scenario.traffic_sign import TrafficLightState, TrafficLight, TrafficSign
+from commonroad.scenario.traffic_sign import TrafficSign
+from commonroad.scenario.traffic_light import TrafficLight
+from commonroad.scenario.traffic_light import TrafficLightState
 from commonroad.scenario.trajectory import Trajectory
 from commonroad.visualization.draw_params import *
 from commonroad.visualization.icons import supported_icons, get_obstacle_icon_patch
 from commonroad.visualization.traffic_sign import draw_traffic_light_signs
 from commonroad.visualization.util import LineDataUnits, collect_center_line_colors, get_arrow_path_at, colormap_idx, \
     line_marking_to_linestyle, traffic_light_color_dict, get_tangent_angle, approximate_bounding_box_dyn_obstacles, \
     get_vehicle_direction_triangle, LineCollectionDataUnits
@@ -136,15 +139,15 @@
             self._plot_limits = val
         elif val is not None:
             raise ValueError(f"Invalid plot_limit: {val}")
 
     @property
     def plot_limits_focused(self):
         """
-        :returns: plot limits centered around focus_obstacle_id defined in draw_params
+        plot limits centered around focus_obstacle_id defined in draw_params
         """
         if self.plot_limits is not None and (self.plot_limits == "auto" or self.plot_center is None):
             return self.plot_limits
         elif self.plot_center is not None:
             plot_limits_f = np.array(self.plot_limits, dtype=int)
             plot_limits_f[:2] += int(self.plot_center[0])
             plot_limits_f[2:] += int(self.plot_center[1])
@@ -665,14 +668,15 @@
                         mpl.patches.PathPatch(path, color=draw_params.facecolor, lw=draw_params.line_width,
                                               zorder=draw_params.zorder, fill=False))
             else:
                 self.dynamic_collections.append(
                         collections.EllipseCollection(np.ones([traj_points.shape[0], 1]) * draw_params.line_width,
                                                       np.ones([traj_points.shape[0], 1]) * draw_params.line_width,
                                                       np.zeros([traj_points.shape[0], 1]), offsets=traj_points,
+                                                      offset_transform=self.ax.transData,
                                                       units='xy', linewidths=0, zorder=draw_params.zorder,
                                                       facecolor=draw_params.facecolor))
 
         # Draw uncertain states
         for pset in position_sets:
             pset.draw(self, draw_params.shape)
 
@@ -975,16 +979,18 @@
             if unique_colors:
                 # set center bound color to unique value
                 center_bound_color = cmap_lanelet(i_lanelet)
 
             # direction arrow
             if draw_start_and_direction:
                 center = lanelet.center_vertices[0]
-                tan_vec = np.array(lanelet.right_vertices[0]) - np.array(lanelet.left_vertices[0])
-                path = get_arrow_path_at(center[0], center[1], math.atan2(tan_vec[1], tan_vec[0]) + 0.5 * np.pi)
+                orientation = math.atan2(*(lanelet.center_vertices[1] - center)[::-1])
+                lanelet_width = np.linalg.norm(lanelet.right_vertices[0] - lanelet.left_vertices[0])
+                arrow_width = min(lanelet_width, 1.5)
+                path = get_arrow_path_at(*center, orientation, arrow_width)
                 if unique_colors:
                     direction_list.append(mpl.patches.PathPatch(path, color=center_bound_color, lw=0.5,
                                                                 zorder=ZOrders.DIRECTION_ARROW,
                                                                 antialiased=antialiased))
                 else:
                     direction_list.append(path)
```

### Comparing `commonroad_io-2023.1/commonroad/visualization/renderer.py` & `commonroad_io-2023.2/commonroad/visualization/renderer.py`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_sign.py` & `commonroad_io-2023.2/commonroad/visualization/traffic_sign.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 from PIL import Image
 from matplotlib.axes import Axes, mtext
 from matplotlib.offsetbox import OffsetImage, AnnotationBbox, HPacker, TextArea, VPacker, OffsetBox
 from scipy.cluster.hierarchy import linkage, fcluster
 
 from commonroad.geometry.shape import *
-from commonroad.scenario.traffic_sign import TrafficSign, TrafficLight, TrafficSignIDUsa
+from commonroad.scenario.traffic_sign import TrafficSign, TrafficSignIDUsa
+from commonroad.scenario.traffic_light import TrafficLight
 from commonroad.visualization.draw_params import TrafficLightParams, TrafficSignParams
 
 # path to traffic sign .png files
 traffic_sign_path = os.path.join(os.path.dirname(__file__), 'traffic_signs/')
 
 speed_limit_factors = {'mph': 2.23694, 'kmh': 3.6, 'ms': 1.0}
 
@@ -109,17 +110,17 @@
     def set_ax_lims(self, dx_m, dy_m, dx_pix, dy_pix):
         self.dx_m = dx_m
         self.dy_m = dy_m
         self.dx_pix = dx_pix
         self.dy_pix = dy_pix
 
     def ax_update(self, ax: Axes):
-        '''
+        """
         Update image size based on axes limits and window size in pixels
-        '''
+        """
         bbox = ax.get_window_extent()
         width_px, height_px = bbox.width, bbox.height
         # Get the range for the new area
         _, _, xdelta, ydelta = ax.viewLim.bounds
         self.set_ax_lims(xdelta, ydelta, width_px, height_px)
         self.text_area.set_ax_lims(xdelta, ydelta, width_px, height_px)
 
@@ -265,15 +266,15 @@
 
     for traffic_sign in traffic_signs:
         if traffic_sign.virtual is True or traffic_sign.position is None:
             continue
         imageboxes = []
         for element in traffic_sign.traffic_sign_elements:
             el_id = element.traffic_sign_element_id
-            if show_traffic_signs is None or el_id.value not in show_traffic_signs:
+            if show_traffic_signs is not None and el_id.value not in show_traffic_signs:
                 continue
             show_label = show_label_default
             path = os.path.join(traffic_sign_path, el_id.__class__.__name__, el_id.value + '.png')
             plot_img = True
             # get png image
             if not os.path.exists(path):
                 warnings.warn(f"File for traffic sign {element} at {path} does not exist!")
```

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDChina/.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDChina/.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000-11.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000-11.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000-21.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000-21.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000-31.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000-31.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1000.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1001-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1001-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1001-31.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1001-31.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-11.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-11.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-12.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-12.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-13.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-13.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-14.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-14.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-21.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-21.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-22.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-22.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-23.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-23.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-24.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1002-24.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1004-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1004-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1004-31.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1004-31.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1004-32.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1004-32.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1004-33.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1004-33.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1004-34.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1004-34.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1004-35.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1004-35.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-31.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-31.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-32.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-32.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-33.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-33.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-34.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-34.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-35.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-35.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-36.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-36.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-37.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-37.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-38.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-38.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-39.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1006-39.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1007-31.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1007-31.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/101.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/101.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1010-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1010-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1010-11.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1010-11.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1010-12.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1010-12.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1010-13.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1010-13.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1010-14.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1010-14.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-31.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-31.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-32.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-32.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-33.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-33.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-34.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-34.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-35.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-35.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-36.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-36.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-37.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-37.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-38.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-38.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-50.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-50.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-51.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-51.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-52.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-52.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-53.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1012-53.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/102.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/102.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1020-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1020-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1022-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1022-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1024-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1024-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1026-36.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1026-36.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1026-37.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1026-37.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1026-38.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1026-38.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/103-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/103-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/103-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/103-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1031-52.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1031-52.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1040-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1040-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1048-12.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1048-12.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1049-13.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1049-13.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1052-31.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1052-31.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1053-33.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1053-33.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1053-34.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1053-34.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1053-35.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/1053-35.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/108.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/108.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/114.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/114.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/120.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/120.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/123.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/123.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/124.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/124.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/125.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/125.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/131.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/131.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/133-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/133-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/133-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/133-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/138.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/138.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/142-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/142-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/145-50.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/145-50.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/201.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/201.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/205.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/205.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/206.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/206.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/208.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/208.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/209-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/209-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/209-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/209-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/209-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/209-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/209.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/209.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/211-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/211-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/211-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/211-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/211.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/211.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/2113.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/2113.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/214-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/214-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/214-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/214-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/214.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/214.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/215.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/215.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/220-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/220-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/220-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/220-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/222-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/222-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/222-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/222-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/223.2-50.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/223.2-50.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/223.2-51.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/223.2-51.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/223.2.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/223.2.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/224-50.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/224-50.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/237.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/237.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/239.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/239.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/240.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/240.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/242.1.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/242.1.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/242.2.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/242.2.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/244.1.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/244.1.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/244.2.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/244.2.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/245.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/245.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/250.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/250.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/251.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/251.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/253.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/253.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/254.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/254.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/255.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/255.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/257-54.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/257-54.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/259.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/259.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/260.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/260.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/261.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/261.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/262.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/262.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/264.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/264.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/265.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/265.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/266.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/266.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/267.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/267.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/270.1.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/270.1.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/270.2.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/270.2.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/272.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/272.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/274.1.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/274.1.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/274.2.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/274.2.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/274.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/274.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/275.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/275.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/276.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/276.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/277.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/277.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/278.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/278.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/279.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/279.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/280.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/280.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/281.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/281.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/282.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/282.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/283-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/283-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/283-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/283-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/286-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/286-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/286.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/286.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/301.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/301.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/306.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/306.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/308.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/308.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/310.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/310.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/311.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/311.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/314-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/314-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/314-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/314-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/314-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/314-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/314.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/314.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/325.1.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/325.1.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/325.2.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/325.2.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/327.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/327.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/328.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/328.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/330.1.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/330.1.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/330.2.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/330.2.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/331.1.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/331.1.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/331.2.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/331.2.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/332.1.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/332.1.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/332.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/332.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/333-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/333-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/333-21.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/333-21.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/333-22.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/333-22.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/333.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/333.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/350.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/350.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/354.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/354.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/356.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/356.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/357.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/357.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/363.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/363.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/365-51.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/365-51.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/365-52.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/365-52.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/365-60.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/365-60.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/380.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/380.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/381.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/381.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/386.1.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/386.1.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/386.2.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/386.2.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/386.3.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/386.3.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/406-50.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/406-50.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/418-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/418-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/419-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/419-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/430-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/430-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/432-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/432-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/432-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/432-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/434-50.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/434-50.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/434.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/434.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/438.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/438.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/439.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/439.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/440.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/440.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/448.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/448.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/449.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/449.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/450-50.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/450-50.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/450-51.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/450-51.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/450-52.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/450-52.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/450-53.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/450-53.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/450-54.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/450-54.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/450-55.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/450-55.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/453.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/453.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/455.1-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/455.1-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/458.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/458.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/460-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/460-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/460-12.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/460-12.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/460-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/460-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/460-21.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/460-21.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/460-22.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/460-22.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/460-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/460-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/501-15.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/501-15.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/501-16.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/501-16.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/511-22.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/511-22.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/521-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/521-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/521-31.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/521-31.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/521-32.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/521-32.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/521-33.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/521-33.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/525.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/525.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/531-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/531-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/531-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/531-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/531-21.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/531-21.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/533-22.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/533-22.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/550-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/550-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/600-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/600-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/600-31.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/600-31.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/600-32.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/600-32.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/600-34.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/600-34.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/600-35.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/600-35.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/600-38.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/600-38.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/605-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/605-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/605-11.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/605-11.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/605-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/605-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/605-21.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/605-21.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/605-31.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/605-31.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-11.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-11.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-12.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-12.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-13.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-13.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-21.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-21.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-22.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-22.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-23.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/625-23.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/626-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/626-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/626-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/626-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/626-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/626-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/626-31.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/626-31.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/626-32.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/626-32.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/628-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/628-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/629-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/629-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/629-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/629-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDGermany/720.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDGermany/720.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDRussia/.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDRussia/.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDSpain/.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDSpain/.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r1.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r1.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r100.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r100.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r101.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r101.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r106.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r106.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r107.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r107.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r2.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r2.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r205.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r205.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r301.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r301.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r305.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r305.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r307.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r307.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r308.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDSpain/r308.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDSpain/s13.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDSpain/s13.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/CW20-1.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/CW20-1.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/D1-2.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/D1-2.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/M6-2aL.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/M6-2aL.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R1-3.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R1-3.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R10-11.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R10-11.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R10-7.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R10-7.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R2-1.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R2-1.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-1.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-1.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-2.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-2.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-27.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-27.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-4.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-4.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-5L.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-5L.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-5R.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-5R.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-8b.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R3-8b.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R4-7.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R4-7.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R5-1.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R5-1.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R6-1L.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R6-1L.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R6-1R.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R6-1R.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R7-1.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R7-1.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R7-107.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R7-107.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R7-201a.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R7-201a.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R7-4.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R7-4.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R7-8.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R7-8.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R8-3.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R8-3.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R8-3C.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R8-3C.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R8-3gP.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/R8-3gP.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/W1-3L.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/W1-3L.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/W1-6L.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/W1-6L.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/W11-2.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/W11-2.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/W3-3.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/W3-3.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDUsa/W4-2R.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDUsa/W4-2R.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000-11.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000-11.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000-21.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000-21.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000-31.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000-31.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1000.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1001-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1001-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1001-31.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1001-31.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-11.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-11.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-12.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-12.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-13.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-13.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-14.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-14.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-21.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-21.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-22.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-22.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-23.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-23.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-24.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1002-24.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1004-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1004-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1004-31.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1004-31.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1004-32.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1004-32.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1004-33.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1004-33.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1004-34.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1004-34.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1004-35.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1004-35.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-31.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-31.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-32.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-32.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-33.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-33.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-34.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-34.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-35.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-35.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-36.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-36.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-37.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-37.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-38.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-38.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-39.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1006-39.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1007-31.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1007-31.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/101.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/101.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1010-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1010-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1010-11.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1010-11.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1010-12.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1010-12.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1010-13.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1010-13.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1010-14.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1010-14.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-31.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-31.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-32.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-32.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-33.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-33.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-34.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-34.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-35.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-35.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-36.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-36.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-37.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-37.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-38.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-38.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-50.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-50.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-51.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-51.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-52.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-52.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-53.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1012-53.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/102.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/102.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1020-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1020-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1022-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1022-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1024-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1024-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1026-36.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1026-36.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1026-37.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1026-37.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1026-38.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1026-38.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/103-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/103-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/103-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/103-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1031-52.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1031-52.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1040-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1040-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1048-12.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1048-12.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1049-13.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1049-13.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1052-31.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1052-31.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1053-33.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1053-33.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1053-34.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1053-34.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1053-35.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/1053-35.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/108.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/108.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/114.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/114.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/120.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/120.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/123.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/123.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/124.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/124.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/125.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/125.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/131.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/131.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/133-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/133-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/133-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/133-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/138.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/138.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/142-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/142-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/145-50.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/145-50.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/201.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/201.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/205.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/205.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/206.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/206.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/208.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/208.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/209-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/209-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/209-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/209-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/209-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/209-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/209.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/209.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/211-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/211-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/211-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/211-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/211.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/211.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/2113.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/2113.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/214-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/214-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/214-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/214-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/214.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/214.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/215.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/215.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/220-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/220-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/220-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/220-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/222-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/222-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/222-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/222-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/223.2-50.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/223.2-50.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/223.2-51.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/223.2-51.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/223.2.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/223.2.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/224-50.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/224-50.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/237.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/237.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/239.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/239.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/240.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/240.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/242.1.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/242.1.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/242.2.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/242.2.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/244.1.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/244.1.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/244.2.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/244.2.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/245.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/245.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/250.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/250.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/251.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/251.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/253.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/253.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/254.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/254.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/255.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/255.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/257-54.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/257-54.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/259.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/259.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/260.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/260.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/261.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/261.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/262.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/262.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/264.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/264.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/265.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/265.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/266.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/266.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/267.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/267.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/270.1.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/270.1.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/270.2.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/270.2.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/272.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/272.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/274.1.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/274.1.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/274.2.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/274.2.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/274.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/274.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/275.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/275.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/276.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/276.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/277.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/277.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/278.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/278.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/279.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/279.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/280.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/280.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/281.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/281.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/282.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/282.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/283-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/283-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/283-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/283-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/286-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/286-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/286.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/286.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/301.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/301.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/306.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/306.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/308.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/308.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/310.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/310.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/311.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/311.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/314-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/314-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/314-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/314-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/314-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/314-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/314.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/314.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/325.1.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/325.1.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/325.2.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/325.2.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/327.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/327.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/328.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/328.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/330.1.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/330.1.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/330.2.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/330.2.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/331.1.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/331.1.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/331.2.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/331.2.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/332.1.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/332.1.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/332.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/332.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/333-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/333-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/333-21.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/333-21.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/333-22.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/333-22.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/333.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/333.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/350.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/350.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/354.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/354.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/356.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/356.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/357.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/357.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/363.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/363.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/365-51.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/365-51.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/365-52.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/365-52.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/365-60.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/365-60.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/380.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/380.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/381.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/381.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/386.1.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/386.1.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/386.2.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/386.2.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/386.3.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/386.3.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/406-50.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/406-50.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/418-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/418-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/419-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/419-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/430-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/430-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/432-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/432-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/432-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/432-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/434-50.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/434-50.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/434.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/434.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/438.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/438.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/439.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/439.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/440.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/440.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/448.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/448.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/449.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/449.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/450-50.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/450-50.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/450-51.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/450-51.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/450-52.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/450-52.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/450-53.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/450-53.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/450-54.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/450-54.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/450-55.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/450-55.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/453.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/453.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/455.1-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/455.1-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/458.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/458.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/460-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/460-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/460-12.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/460-12.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/460-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/460-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/460-21.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/460-21.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/460-22.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/460-22.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/460-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/460-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/501-15.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/501-15.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/501-16.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/501-16.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/511-22.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/511-22.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/521-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/521-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/521-31.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/521-31.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/521-32.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/521-32.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/521-33.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/521-33.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/525.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/525.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/531-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/531-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/531-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/531-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/531-21.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/531-21.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/533-22.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/533-22.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/550-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/550-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/600-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/600-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/600-31.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/600-31.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/600-32.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/600-32.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/600-34.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/600-34.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/600-35.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/600-35.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/600-38.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/600-38.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/605-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/605-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/605-11.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/605-11.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/605-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/605-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/605-21.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/605-21.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/605-31.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/605-31.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-11.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-11.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-12.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-12.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-13.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-13.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-21.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-21.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-22.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-22.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-23.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/625-23.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/626-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/626-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/626-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/626-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/626-30.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/626-30.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/626-31.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/626-31.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/626-32.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/626-32.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/628-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/628-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/629-10.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/629-10.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/629-20.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/629-20.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/720.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/TrafficSignIDZamunda/720.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/traffic_light_state_green.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/traffic_light_state_green.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/traffic_light_state_inactive.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/traffic_light_state_inactive.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/traffic_light_state_red.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/traffic_light_state_red.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/traffic_light_state_redYellow.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/traffic_light_state_redYellow.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/traffic_signs/traffic_light_state_yellow.png` & `commonroad_io-2023.2/commonroad/visualization/traffic_signs/traffic_light_state_yellow.png`

 * *Files identical despite different names*

### Comparing `commonroad_io-2023.1/commonroad/visualization/util.py` & `commonroad_io-2023.2/commonroad/visualization/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,20 +7,19 @@
 import matplotlib.patches as patches
 import matplotlib.pyplot as plt
 import numpy as np
 import math
 
 from commonroad.geometry.shape import Rectangle
 from commonroad.geometry.transform import rotate_translate
-from commonroad.scenario.lanelet import LaneletNetwork, LineMarking
+from commonroad.scenario.lanelet import LaneletNetwork
+from commonroad.common.common_lanelet import LineMarking
 from commonroad.scenario.obstacle import DynamicObstacle
 from commonroad.scenario.scenario import Scenario
-from commonroad.scenario.traffic_sign import TrafficLightState, \
-    TrafficLight, \
-    TrafficLightDirection
+from commonroad.scenario.traffic_light import TrafficLightState, TrafficLightDirection, TrafficLight
 from matplotlib.lines import Line2D
 from matplotlib.path import Path
 from matplotlib.axes import Axes
 
 
 def _data_units_to_pt(axes: Axes, lw_meter: float) -> float:
     """Convert data (axis) unit to line width. """
@@ -233,29 +232,24 @@
     if np.inf in bounds[0] or -np.inf in bounds[0] or np.inf in bounds[
         1] or -np.inf in bounds[1]:
         return None
     else:
         return tuple(bounds)
 
 
-def get_arrow_path_at(x, y, angle):
+def get_arrow_path_at(x: float, y: float, angle: float, scale_direction: float = 1.5) -> Path:
     """Returns path of arrow shape"""
     # direction arrow
     codes_direction = [Path.MOVETO, Path.LINETO, Path.LINETO, Path.CLOSEPOLY]
 
-    scale_direction = 1.5
-    pts = np.array([[0.0, -0.5, 1.0], [1.0, 0.0, 1.0], [0.0, 0.5, 1.0],
-                    [0.0, -0.5, 1.0]])
-    scale_m = np.array(
-            [[scale_direction, 0, 0], [0, scale_direction, 0], [0, 0, 1]])
-    transform = np.array([[math.cos(angle), -math.sin(angle), x],
-                          [math.sin(angle), math.cos(angle), y], [0, 0, 1]])
-    ptr_trans = transform.dot(scale_m.dot(pts.transpose()))
-    ptr_trans = ptr_trans[0:2, :]
-    ptr_trans = ptr_trans.transpose()
+    pts = np.array([[0.0, -0.5], [1.0, 0.0], [0.0, 0.5], [0.0, -0.5]])
+    pts *= scale_direction
+    transform = np.array([[math.cos(angle), math.sin(angle)], [-math.sin(angle), math.cos(angle)]])
+    ptr_trans = pts @ transform
+    ptr_trans += [x, y]
 
     path = Path(ptr_trans, codes_direction)
     return path
 
 
 def colormap_idx(max_x):
     norm = mpl.colors.Normalize(vmin=0, vmax=max_x)
```

### Comparing `commonroad_io-2023.1/pyproject.toml` & `commonroad_io-2023.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 [tool.poetry]
 name = "commonroad-io"
-version = "2023.1"
+version = "2023.2"
 description = "Python tool to read, write, and visualize CommonRoad scenarios and solutions for automated vehicles."
 authors = ["Cyber-Physical Systems Group, Technical University of Munich <commonroad@lists.lrz.de>"]
 license = "BSD"
 readme = "README.md"
 homepage = "https://commonroad.in.tum.de"
 keywords= ["autonomous", "automated", "vehicles", "driving", "motion", "planning"]
 classifiers = [
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: BSD License",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS",
@@ -22,17 +21,16 @@
 
 [tool.poetry.urls]
 Documentation = "https://commonroad.in.tum.de/static/docs/commonroad-io/index.html"
 Forum = "https://commonroad.in.tum.de/forum/c/commonroad-io"
 Source = "https://gitlab.lrz.de/tum-cps/commonroad_io"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 numpy = [
-    {version = ">=1.13,<1.22", python = "<3.8"},
     {version = ">=1.22", python = ">=3.8,<3.11"},
     {version = "^1.24", python = ">=3.11"}
 ]
 scipy = [
     {version = ">=1.5.2", python = "<3.11"},
     {version = "^1.9", python = ">=3.11"}
 ]
@@ -45,15 +43,14 @@
 commonroad-vehicle-models = ">=2.0.0"
 rtree = ">=0.8.3"
 protobuf = "==3.20.1"
 omegaconf = ">=2.0"
 tqdm = ">=4.64"
 
 
-
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = ">=1.3.6"
 graphviz = ">=0.3"
 sphinx-autodoc-typehints = ">=1.3.0"
```

### Comparing `commonroad_io-2023.1/PKG-INFO` & `commonroad_io-2023.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,33 @@
 Metadata-Version: 2.1
 Name: commonroad-io
-Version: 2023.1
+Version: 2023.2
 Summary: Python tool to read, write, and visualize CommonRoad scenarios and solutions for automated vehicles.
 Home-page: https://commonroad.in.tum.de
 License: BSD
 Keywords: autonomous,automated,vehicles,driving,motion,planning
 Author: Cyber-Physical Systems Group, Technical University of Munich
 Author-email: commonroad@lists.lrz.de
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Pillow (>=7.0.0)
 Requires-Dist: commonroad-vehicle-models (>=2.0.0)
 Requires-Dist: iso3166 (>=1.0.1)
 Requires-Dist: lxml (>=4.2.2)
 Requires-Dist: matplotlib (>=3.0.0)
 Requires-Dist: networkx (>=2.2)
-Requires-Dist: numpy (>=1.13,<1.22) ; python_version < "3.8"
 Requires-Dist: numpy (>=1.22) ; python_version >= "3.8" and python_version < "3.11"
 Requires-Dist: numpy (>=1.24,<2.0) ; python_version >= "3.11"
 Requires-Dist: omegaconf (>=2.0)
 Requires-Dist: protobuf (==3.20.1)
 Requires-Dist: rtree (>=0.8.3)
 Requires-Dist: scipy (>=1.5.2) ; python_version < "3.11"
 Requires-Dist: scipy (>=1.9,<2.0) ; python_version >= "3.11"
@@ -50,15 +43,14 @@
 [![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
 [![Windows](https://svgshare.com/i/ZhY.svg)](https://svgshare.com/i/ZhY.svg)  
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/commonroad-io.svg)](https://pypi.python.org/pypi/commonroad-io/)  
 [![PyPI version fury.io](https://badge.fury.io/py/commonroad-io.svg)](https://pypi.python.org/pypi/commonroad-io/)
 [![PyPI download month](https://img.shields.io/pypi/dm/commonroad-io.svg?label=PyPI%20downloads)](https://pypi.python.org/pypi/commonroad-io/) 
 [![PyPI download week](https://img.shields.io/pypi/dw/commonroad-io.svg?label=PyPI%20downloads)](https://pypi.python.org/pypi/commonroad-io/)   
 [![PyPI license](https://img.shields.io/pypi/l/commonroad-io.svg)](https://pypi.python.org/pypi/commonroad-io/)
-[![Documentation Status](https://readthedocs.org/projects/commonroad-io/badge/?version=latest)](http://commonroad-io.readthedocs.io/?badge=latest) 
 
 
 Numerical experiments for motion planning of road vehicles require numerous ingredients: vehicle dynamics, 
 a road network, static obstacles, dynamic obstacles and their movement over time, goal regions, a cost function, etc. 
 Providing a description of the numerical experiment precise enough to reproduce it might require several pages of 
 information. 
 Thus, only key aspects are typically described in scientific publications, making it impossible to reproduce 
@@ -76,15 +68,15 @@
 # commonroad-io
 
 The commonroad-io package provides methods to read, write, and visualize CommonRoad scenarios and planning problems. Furthermore, it can be used as a framework for implementing motion planning algorithms to solve CommonRoad Benchmarks and is the basis for other tools of the CommonRoad Framework.
 With commonroad-io, those solutions can be written to xml-files for uploading them on [commonroad.in.tum.de](https://commonroad.in.tum.de/).
 
 commonroad-io 2023.1 is compatible with CommonRoad scenarios in version 2020a and supports reading 2018b scenarios.
 
-The software is written in Python and tested on Linux for the Python 3.7, 3.8, 3.9, 3.10, and 3.11.
+The software is written in Python and tested on Linux for the Python 3.8, 3.9, 3.10, and 3.11.
 
 
 ## Documentation
 
 The full documentation of the API and introducing examples can be found under [commonroad.in.tum.de](https://commonroad-io.readthedocs.io/en/latest/).
 
 For getting started, we recommend our [tutorials](https://commonroad.in.tum.de/commonroad-io).
@@ -124,14 +116,42 @@
 Alternatively, clone from our gitlab repository::
 
 	git clone https://gitlab.lrz.de/tum-cps/commonroad_io.git
 
 and add the folder commonroad-io to your Python environment.
 
 ## Changelog
+Compared to version 2023.1, the following features have been added or changed:
+
+### Added
+- Area for modelling drivable areas which cannot be represented by lanelets
+- New weather and time of day options
+- Allow file reader to determine format based on suffix 
+
+### Fixed
+
+- Visualization of all traffic signs by setting `show_traffic_signs = None` in draw parameters
+- Validity functions to support z-axis
+- Unreferenced traffic signs for lanelet networks filtered by lanelet type
+
+### Changed
+
+- Visualization of direction arrow of narrow lanelets
+- Traffic light cycle optional
+- Traffic light in separate python file
+- Allow file reader to determine format based on suffix 
+- Broaden types allowed as file names 
+- Open files safely by using a context manager 
+- Use correct suffix when inferring filename from scenario id
+
+### Removed
+
+- function get_default_cycle for traffic lights
+- support for Python 3.7
+
 Compared to version 2022.3, the following features have been added or changed:
 
 ### Added
 - Support for shapely>=2.0.0
 
 ### Fixed
 
@@ -140,14 +160,15 @@
 - Default plot limits for focused obstacle
 - Use dt from scenario as default for video creation
 - Apply axis visible-option also for video creation
 - Protobuf FileReader marking road network related IDs as used
 - State attribute comparison
 
 ### Changed
+>>>>>>> README.md
 
 - Name of SIDEWALK and BUSLANE traffic signs to PEDESTRIAN_SIDEWALK and BUS_LANE
 - Packaging and dependency management using poetry
 
 
 ## Authors
 Contribution (in alphabetic order by last name): Yannick Ballnath, Behtarin Ferdousi, Luis Gressenbuch, Moritz Klischat,
```


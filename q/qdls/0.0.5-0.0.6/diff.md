# Comparing `tmp/qdls-0.0.5.tar.gz` & `tmp/qdls-0.0.6.tar.gz`

## Comparing `qdls-0.0.5.tar` & `qdls-0.0.6.tar`

### file list

```diff
@@ -1,67 +1,69 @@
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 qdls-0.0.5/build_upload.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.5/src/__init__.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/__init__.py
--rw-r--r--   0        0        0    11695 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/data.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/loggers.py
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/losses.py
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/metrics.py
--rw-r--r--   0        0        0    13330 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/object.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/optim.py
--rw-r--r--   0        0        0    13611 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/pretrains.py
--rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/tensor_ops.py
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/test.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/train.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/draw/__init__.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/draw/experiment.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/draw/stats.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/__init__.py
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/process_utils.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/cypher/__init__.py
--rw-r--r--   0        0        0    61918 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/cypher/grammar/Cypher.interp
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/cypher/grammar/Cypher.tokens
--rw-r--r--   0        0        0    61096 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/cypher/grammar/CypherLexer.interp
--rw-r--r--   0        0        0    72699 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/cypher/grammar/CypherLexer.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/cypher/grammar/CypherLexer.tokens
--rw-r--r--   0        0        0    33891 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/cypher/grammar/CypherListener.py
--rw-r--r--   0        0        0   413383 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/cypher/grammar/CypherParser.py
--rw-r--r--   0        0        0    19984 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/cypher/grammar/CypherVisitor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/cypher/grammar/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/cypher/utils/__init__.py
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/cypher/utils/execute.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/cypher/utils/parse.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/cypher/utils/syntax.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/sparql/__init__.py
--rw-r--r--   0        0        0    57079 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/sparql/grammar/Sparql.interp
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/sparql/grammar/Sparql.tokens
--rw-r--r--   0        0        0    52018 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/sparql/grammar/SparqlLexer.interp
--rw-r--r--   0        0        0    62363 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/sparql/grammar/SparqlLexer.py
--rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/sparql/grammar/SparqlLexer.tokens
--rw-r--r--   0        0        0    44193 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/sparql/grammar/SparqlListener.py
--rw-r--r--   0        0        0   497844 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/sparql/grammar/SparqlParser.py
--rw-r--r--   0        0        0    26235 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/sparql/grammar/SparqlVisitor.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/sparql/grammar/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/sparql/utils/__init__.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/sparql/utils/parse.py
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/gql/sparql/utils/syntax.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/reg/__init__.py
--rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/reg/register.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/reg/collators/__init__.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/reg/collators/common_collators.py
--rw-r--r--   0        0        0     3979 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/reg/datamodules/base_dm.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/reg/datamodules/dataset_builder.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/reg/models/__init__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/reg/models/test_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/reg/process_functions/__init__.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/reg/process_functions/common.py
--rw-r--r--   0        0        0     7909 2020-02-02 00:00:00.000000 qdls-0.0.5/src/qdls/reg/process_functions/kqa.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 qdls-0.0.5/test/btest.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 qdls-0.0.5/test/example_config.yaml
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 qdls-0.0.5/test/test_draw.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 qdls-0.0.5/test/test_reg.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 qdls-0.0.5/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 qdls-0.0.5/LICENSE
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 qdls-0.0.5/README.md
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 qdls-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 qdls-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 qdls-0.0.6/build_upload.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.6/src/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/__init__.py
+-rw-r--r--   0        0        0    11695 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/data.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/loggers.py
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/losses.py
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/metrics.py
+-rw-r--r--   0        0        0    13330 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/object.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/optim.py
+-rw-r--r--   0        0        0    13611 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/pretrains.py
+-rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/tensor_ops.py
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/test.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/train.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/draw/__init__.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/draw/experiment.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/draw/stats.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/__init__.py
+-rw-r--r--   0        0        0     6932 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/process_utils.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/__init__.py
+-rw-r--r--   0        0        0    61918 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/grammar/Cypher.interp
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/grammar/Cypher.tokens
+-rw-r--r--   0        0        0    61096 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/grammar/CypherLexer.interp
+-rw-r--r--   0        0        0    72699 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/grammar/CypherLexer.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/grammar/CypherLexer.tokens
+-rw-r--r--   0        0        0    33891 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/grammar/CypherListener.py
+-rw-r--r--   0        0        0   413383 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/grammar/CypherParser.py
+-rw-r--r--   0        0        0    19984 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/grammar/CypherVisitor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/grammar/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/utils/__init__.py
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/utils/execute.py
+-rw-r--r--   0        0        0     9099 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/utils/kqa_eval.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/utils/parse.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/cypher/utils/syntax.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/__init__.py
+-rw-r--r--   0        0        0    57079 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/grammar/Sparql.interp
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/grammar/Sparql.tokens
+-rw-r--r--   0        0        0    52018 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/grammar/SparqlLexer.interp
+-rw-r--r--   0        0        0    62363 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/grammar/SparqlLexer.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/grammar/SparqlLexer.tokens
+-rw-r--r--   0        0        0    44193 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/grammar/SparqlListener.py
+-rw-r--r--   0        0        0   497844 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/grammar/SparqlParser.py
+-rw-r--r--   0        0        0    26235 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/grammar/SparqlVisitor.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/grammar/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/utils/__init__.py
+-rw-r--r--   0        0        0    24277 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/utils/kqa_eval.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/utils/parse.py
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/gql/sparql/utils/syntax.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/reg/__init__.py
+-rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/reg/register.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/reg/collators/__init__.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/reg/collators/common_collators.py
+-rw-r--r--   0        0        0     4588 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/reg/datamodules/base_dm.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/reg/datamodules/dataset_builder.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/reg/models/__init__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/reg/models/test_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/reg/process_functions/__init__.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/reg/process_functions/common.py
+-rw-r--r--   0        0        0     7909 2020-02-02 00:00:00.000000 qdls-0.0.6/src/qdls/reg/process_functions/kqa.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 qdls-0.0.6/test/btest.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 qdls-0.0.6/test/example_config.yaml
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 qdls-0.0.6/test/test_draw.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 qdls-0.0.6/test/test_reg.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 qdls-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 qdls-0.0.6/LICENSE
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 qdls-0.0.6/README.md
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 qdls-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 qdls-0.0.6/PKG-INFO
```

### Comparing `qdls-0.0.5/src/qdls/data.py` & `qdls-0.0.6/src/qdls/data.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/loggers.py` & `qdls-0.0.6/src/qdls/loggers.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/losses.py` & `qdls-0.0.6/src/qdls/losses.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/metrics.py` & `qdls-0.0.6/src/qdls/metrics.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/object.py` & `qdls-0.0.6/src/qdls/object.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/optim.py` & `qdls-0.0.6/src/qdls/optim.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/pretrains.py` & `qdls-0.0.6/src/qdls/pretrains.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/tensor_ops.py` & `qdls-0.0.6/src/qdls/tensor_ops.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/test.py` & `qdls-0.0.6/src/qdls/test.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/utils.py` & `qdls-0.0.6/src/qdls/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,26 +42,26 @@
         if type(v) is Namespace:
             d[k] = config2dict(v)
         else:
             d[k] = v 
     return d 
 
 
-def print_string(string):
+def print_string(string, color="yellow"):
     """ 在命令行以黄色字体打印 string 
         eg: ====================  string  ====================
     """
     if type(string) is not str:
         try:
             string = str(string)
         except:
             raise Exception("Input must be str or can be converted to str")
 
     s = "="*20 + string.center(len(string)+10,) + "="*20
-    cprint(s, "yellow", attrs=["bold"])
+    cprint(s, color, attrs=["bold"])
 
 
 def print_config(config, title=None):
     """在命令行以 json 格式打印 config 绿色字体;   
 
     Args:
         config:  Config object
```

### Comparing `qdls-0.0.5/src/qdls/draw/experiment.py` & `qdls-0.0.6/src/qdls/draw/experiment.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/draw/stats.py` & `qdls-0.0.6/src/qdls/draw/stats.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/gql/process_utils.py` & `qdls-0.0.6/src/qdls/gql/process_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     # 'oC_Expression', 
     'oC_Literal'                    # "a string or number"
 ]
 
 _SP_NODES = [
     # 'var',                          # ?v ?pv
     # 'pathPrimary',                  # <pred:value> date name fact_r h t 
-    # 'iri',                          #  <for_work>
+    'iri',                          #  <for_work>
     'string',                       # "a string"
     'numericLiteralUnsigned',       # 1895
     'numericLiteralNegative'        # -192
 ]
 
 def parse_subtree(tree, parts):
     if tree.getText() == "<EOF>":
@@ -115,15 +115,15 @@
     # print(parts)
     # print(d)
     nodes, relations = [], []
     for k,v in d.items():
         nonterm_name, values = v 
         if nonterm_name in ["numericLiteralUnsigned", "numericLiteralNegative", "string"]:
             nodes.append( "".join(values) )
-        elif nonterm_name == "not decided":
+        elif nonterm_name in ['iri']:
             relations.append( "".join(values) )
         else:
             raise Exception(f'{nonterm_name} not handled!')
     
     # print(nodes)
     # print(relations)
     return nodes, relations
```

### Comparing `qdls-0.0.5/src/qdls/gql/utils.py` & `qdls-0.0.6/src/qdls/gql/utils.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/gql/cypher/grammar/Cypher.interp` & `qdls-0.0.6/src/qdls/gql/cypher/grammar/Cypher.interp`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/gql/cypher/grammar/Cypher.tokens` & `qdls-0.0.6/src/qdls/gql/cypher/grammar/Cypher.tokens`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/gql/cypher/grammar/CypherLexer.interp` & `qdls-0.0.6/src/qdls/gql/cypher/grammar/CypherLexer.interp`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/gql/cypher/grammar/CypherLexer.py` & `qdls-0.0.6/src/qdls/gql/cypher/grammar/CypherLexer.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/gql/cypher/grammar/CypherLexer.tokens` & `qdls-0.0.6/src/qdls/gql/cypher/grammar/CypherLexer.tokens`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/gql/cypher/grammar/CypherListener.py` & `qdls-0.0.6/src/qdls/gql/cypher/grammar/CypherListener.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/gql/cypher/grammar/CypherParser.py` & `qdls-0.0.6/src/qdls/gql/cypher/grammar/CypherParser.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/gql/cypher/grammar/CypherVisitor.py` & `qdls-0.0.6/src/qdls/gql/cypher/grammar/CypherVisitor.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/gql/cypher/utils/execute.py` & `qdls-0.0.6/src/qdls/gql/cypher/utils/execute.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/gql/cypher/utils/parse.py` & `qdls-0.0.6/src/qdls/gql/cypher/utils/parse.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/gql/cypher/utils/syntax.py` & `qdls-0.0.6/src/qdls/gql/cypher/utils/syntax.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/gql/sparql/grammar/Sparql.interp` & `qdls-0.0.6/src/qdls/gql/sparql/grammar/Sparql.interp`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/gql/sparql/grammar/Sparql.tokens` & `qdls-0.0.6/src/qdls/gql/sparql/grammar/Sparql.tokens`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/gql/sparql/grammar/SparqlLexer.interp` & `qdls-0.0.6/src/qdls/gql/sparql/grammar/SparqlLexer.interp`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/gql/sparql/grammar/SparqlLexer.py` & `qdls-0.0.6/src/qdls/gql/sparql/grammar/SparqlLexer.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/gql/sparql/grammar/SparqlLexer.tokens` & `qdls-0.0.6/src/qdls/gql/sparql/grammar/SparqlLexer.tokens`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/gql/sparql/grammar/SparqlListener.py` & `qdls-0.0.6/src/qdls/gql/sparql/grammar/SparqlListener.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/gql/sparql/grammar/SparqlParser.py` & `qdls-0.0.6/src/qdls/gql/sparql/grammar/SparqlParser.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/gql/sparql/grammar/SparqlVisitor.py` & `qdls-0.0.6/src/qdls/gql/sparql/grammar/SparqlVisitor.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/gql/sparql/utils/parse.py` & `qdls-0.0.6/src/qdls/gql/sparql/utils/parse.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/gql/sparql/utils/syntax.py` & `qdls-0.0.6/src/qdls/gql/sparql/utils/syntax.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/reg/register.py` & `qdls-0.0.6/src/qdls/reg/register.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/reg/collators/common_collators.py` & `qdls-0.0.6/src/qdls/reg/collators/common_collators.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/src/qdls/reg/datamodules/base_dm.py` & `qdls-0.0.6/src/qdls/reg/datamodules/base_dm.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,29 @@
 from ...utils import print_string, print_config
 from .dataset_builder import DatasetBuilder
 from ..register import registers
 
 
 @registers.datamodule.register("base_dm")
 class BaseDataModule(pl.LightningDataModule):
+    """ 
+        config:
+            pretrained
+            data:
+                train_bsz
+                val_bsz
+                test_bsz
+                padding_side
+                collator_name
+                tokenize_fn_name
+                cache_dir
+                force_reload
+        需要先在registers中注册collator和process_function
+        DataBuilder 需要 train_path val_path test_path 或者 dataset_name
+    """
     def __init__(self, config, **kwargs) -> None:
         super().__init__() 
 
         self.config = config 
         print_string("configuration of datamodule")
         print_config(self.config)
 
@@ -53,20 +68,23 @@
         # 强制 or 训练时没有self.cached_train or 预测时没有self.cached_test
         if self.config.data.force_reload or ( (not os.path.exists(self.cached_train)) and mode=='train') \
             or ( (not os.path.exists(self.cached_test)) and mode =='test'):
             ds = DatasetBuilder(self.config)
             if mode == 'train':
                 trainset = ds.build('train', self.tokenizer, self.tokenize_fn)
                 valset =  ds.build('val', self.tokenizer, self.tokenize_fn)
-
-                trainset.save_to_disk(self.cached_train)
-                valset.save_to_disk(self.cached_val)
+                
+                if trainset is not None:
+                    trainset.save_to_disk(self.cached_train)
+                if valset is not None:
+                    valset.save_to_disk(self.cached_val)
             elif mode == 'test':
             
                 testset = ds.build('test', self.tokenizer, self.tokenize_fn)
+                assert testset is not None 
                 testset.save_to_disk(self.cached_test)
             else:
                 raise Exception(f'mode {mode} not imple')
             
             print_string("Data cache re-generated!")
 
     def setup(self, stage: Optional[str] = None) -> None:
@@ -74,15 +92,15 @@
         if stage == 'fit' or stage is None:
             self.trainset = datasets.load_from_disk(self.cached_train)
             self.valset = datasets.load_from_disk(self.cached_val)
 
         if stage == 'test' or stage is None:
             self.testset = datasets.load_from_disk(self.cached_test)
         
-        print("End setup")
+        print_string("Datasets setup finished!")
 
     def train_dataloader(self):
         return DataLoader(self.trainset, batch_size=self.config.data.train_bsz,
             shuffle=True,
             collate_fn=self.collator_cls(self.tokenizer, mode='train'),
             num_workers=self.num_workers,
         )
```

### Comparing `qdls-0.0.5/src/qdls/reg/datamodules/dataset_builder.py` & `qdls-0.0.6/src/qdls/reg/datamodules/dataset_builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 
 from qdls.data import load_json
 import datasets 
 
 
 class DatasetBuilder():
+    """ 
+        data:
+            train_path  : local file path 
+            val_path   : local file path
+            test_path  : local file path
+            dataset_name: huggingface dataset name
+    """
     def __init__(self, config) -> None:
         """
            应当支持初始化两种方式
             1.huggingface 在线dataset
             2.本地文件 train_path val_path test_path
         """
         if not hasattr(config.data, 'dataset_name'):
@@ -18,21 +25,25 @@
             self._init_from_paths(config)
         else:
             assert hasattr(config.data, 'dataset_name'), \
             f"you should provide dataset_name since no train_path, val_path, test_path is provided"
             self._init_from_hf(config)
 
         self.config = config 
+        if hasattr(config.data, 'num_proc'):
+            self.num_proc = config.data.num_proc
+        else:
+            self.num_proc = 4
 
     
     def _init_from_paths(self, config):
-        """ 从本地文件加载数据 """
-        self.trainset = load_json(config.data.train_path)
-        self.valset = load_json(config.data.val_path)
-        self.testset = load_json(config.data.test_path)
+        """ 从本地文件加载数据, 允许'' """
+        self.trainset = load_json(config.data.train_path) if config.data.train_path else []
+        self.valset = load_json(config.data.val_path) if config.data.val_path else []
+        self.testset = load_json(config.data.test_path) if config.data.test_path else []
 
         
     def _init_from_hf(self, config, proportion=0.8):
         """ 如果只有两个字段（大概率train test）则将train划分为train val """
         ds = datasets.load_dataset(config.data.dataset_name)
         if len(ds) == 2:
             train_ds = ds['train'].train_test_split(test_size=1-proportion)
@@ -50,18 +61,28 @@
             data  = self.trainset
         elif mode == 'val':
             data  = self.valset 
         elif mode == 'test':
             data  = self.testset
         else:
             raise Exception(f"{mode} is not implemented!")
+        
+        if data == []:      # 对应的 trainset or valset or testset 为空
+            return None 
+
         if type(data) is list:                              # 本地加载的数据是list
             dataset = datasets.Dataset.from_list(data)
+        elif type(data) is datasets.Dataset:
+            dataset = data 
         else:
             dataset = datasets.Dataset.from_dict(data)
         dataset = dataset.map(
             tokenize_fn, 
             batched=False,
-            num_proc=self.config.data.num_proc, 
+            num_proc=self.num_proc, 
             fn_kwargs={'tokenizer': tokenizer, 'mode': mode}
         )
-        return dataset
+        return dataset
+    
+    def data_stat(self):
+
+        pass
```

### Comparing `qdls-0.0.5/src/qdls/reg/process_functions/kqa.py` & `qdls-0.0.6/src/qdls/reg/process_functions/kqa.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/test/test_draw.py` & `qdls-0.0.6/test/test_draw.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/test/test_reg.py` & `qdls-0.0.6/test/test_reg.py`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/.gitignore` & `qdls-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/LICENSE` & `qdls-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qdls-0.0.5/pyproject.toml` & `qdls-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "qdls"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Qing25", email="aqsz2526@outlook.com" },
 ]
 description = "Q-Deep Learning Snippets, my working code snippets"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `qdls-0.0.5/PKG-INFO` & `qdls-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdls
-Version: 0.0.5
+Version: 0.0.6
 Summary: Q-Deep Learning Snippets, my working code snippets
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Qing25 <aqsz2526@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


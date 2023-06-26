# Comparing `tmp/clairvoyance_feature_selection-2023.6.26.tar.gz` & `tmp/clairvoyance_feature_selection-2023.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clairvoyance_feature_selection-2023.6.26.tar", last modified: Mon Jun 26 21:24:37 2023, max compression
+gzip compressed data, was "clairvoyance_feature_selection-2023.6.9.tar", last modified: Fri Jun  9 22:37:52 2023, max compression
```

## Comparing `clairvoyance_feature_selection-2023.6.26.tar` & `clairvoyance_feature_selection-2023.6.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-06-26 21:24:37.928255 clairvoyance_feature_selection-2023.6.26/
--rw-------   0 jespinoz  (3456) staff       (20)    34519 2023-06-26 21:05:44.000000 clairvoyance_feature_selection-2023.6.26/LICENSE
--rw-------   0 jespinoz  (3456) staff       (20)      197 2022-12-27 22:26:50.000000 clairvoyance_feature_selection-2023.6.26/MANIFEST.in
--rw-r--r--   0 jespinoz  (3456) staff       (20)      283 2023-06-26 21:24:37.927873 clairvoyance_feature_selection-2023.6.26/PKG-INFO
--rw-------   0 jespinoz  (3456) staff       (20)    13016 2023-06-26 21:03:15.000000 clairvoyance_feature_selection-2023.6.26/README.md
-drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-06-26 21:24:37.921951 clairvoyance_feature_selection-2023.6.26/bin/
--rw-------   0 jespinoz  (3456) staff       (20)    87658 2022-12-27 22:53:11.000000 clairvoyance_feature_selection-2023.6.26/bin/clairvoyance_v1.py
-drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-06-26 21:24:37.924802 clairvoyance_feature_selection-2023.6.26/clairvoyance/
--rw-------   0 jespinoz  (3456) staff       (20)     1741 2023-06-26 21:06:52.000000 clairvoyance_feature_selection-2023.6.26/clairvoyance/__init__.py
--rw-------   0 jespinoz  (3456) staff       (20)   108522 2023-06-26 21:24:00.000000 clairvoyance_feature_selection-2023.6.26/clairvoyance/clairvoyance.py
-drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-06-26 21:24:37.927365 clairvoyance_feature_selection-2023.6.26/clairvoyance_feature_selection.egg-info/
--rw-------   0 jespinoz  (3456) staff       (20)      283 2023-06-26 21:24:37.000000 clairvoyance_feature_selection-2023.6.26/clairvoyance_feature_selection.egg-info/PKG-INFO
--rw-------   0 jespinoz  (3456) staff       (20)      384 2023-06-26 21:24:37.000000 clairvoyance_feature_selection-2023.6.26/clairvoyance_feature_selection.egg-info/SOURCES.txt
--rw-------   0 jespinoz  (3456) staff       (20)        1 2023-06-26 21:24:37.000000 clairvoyance_feature_selection-2023.6.26/clairvoyance_feature_selection.egg-info/dependency_links.txt
--rw-------   0 jespinoz  (3456) staff       (20)      139 2023-06-26 21:24:37.000000 clairvoyance_feature_selection-2023.6.26/clairvoyance_feature_selection.egg-info/requires.txt
--rw-------   0 jespinoz  (3456) staff       (20)       13 2023-06-26 21:24:37.000000 clairvoyance_feature_selection-2023.6.26/clairvoyance_feature_selection.egg-info/top_level.txt
--rw-r--r--   0 jespinoz  (3456) staff       (20)       38 2023-06-26 21:24:37.928378 clairvoyance_feature_selection-2023.6.26/setup.cfg
--rw-------   0 jespinoz  (3456) staff       (20)     1026 2022-12-27 22:38:27.000000 clairvoyance_feature_selection-2023.6.26/setup.py
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-06-09 22:37:52.495942 clairvoyance_feature_selection-2023.6.9/
+-rw-------   0 jespinoz  (3456) staff       (20)     1563 2022-12-27 22:25:44.000000 clairvoyance_feature_selection-2023.6.9/LICENSE.txt
+-rw-------   0 jespinoz  (3456) staff       (20)      197 2022-12-27 22:26:50.000000 clairvoyance_feature_selection-2023.6.9/MANIFEST.in
+-rw-r--r--   0 jespinoz  (3456) staff       (20)      314 2023-06-09 22:37:52.495622 clairvoyance_feature_selection-2023.6.9/PKG-INFO
+-rw-------   0 jespinoz  (3456) staff       (20)    11934 2023-06-09 22:36:15.000000 clairvoyance_feature_selection-2023.6.9/README.md
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-06-09 22:37:52.489595 clairvoyance_feature_selection-2023.6.9/bin/
+-rw-------   0 jespinoz  (3456) staff       (20)    87658 2022-12-27 22:53:11.000000 clairvoyance_feature_selection-2023.6.9/bin/clairvoyance_v1.py
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-06-09 22:37:52.491586 clairvoyance_feature_selection-2023.6.9/clairvoyance/
+-rw-------   0 jespinoz  (3456) staff       (20)     2968 2023-06-09 21:31:53.000000 clairvoyance_feature_selection-2023.6.9/clairvoyance/__init__.py
+-rw-------   0 jespinoz  (3456) staff       (20)   106647 2023-06-09 21:31:32.000000 clairvoyance_feature_selection-2023.6.9/clairvoyance/clairvoyance.py
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-06-09 22:37:52.495156 clairvoyance_feature_selection-2023.6.9/clairvoyance_feature_selection.egg-info/
+-rw-------   0 jespinoz  (3456) staff       (20)      314 2023-06-09 22:37:52.000000 clairvoyance_feature_selection-2023.6.9/clairvoyance_feature_selection.egg-info/PKG-INFO
+-rw-------   0 jespinoz  (3456) staff       (20)      388 2023-06-09 22:37:52.000000 clairvoyance_feature_selection-2023.6.9/clairvoyance_feature_selection.egg-info/SOURCES.txt
+-rw-------   0 jespinoz  (3456) staff       (20)        1 2023-06-09 22:37:52.000000 clairvoyance_feature_selection-2023.6.9/clairvoyance_feature_selection.egg-info/dependency_links.txt
+-rw-------   0 jespinoz  (3456) staff       (20)      139 2023-06-09 22:37:52.000000 clairvoyance_feature_selection-2023.6.9/clairvoyance_feature_selection.egg-info/requires.txt
+-rw-------   0 jespinoz  (3456) staff       (20)       13 2023-06-09 22:37:52.000000 clairvoyance_feature_selection-2023.6.9/clairvoyance_feature_selection.egg-info/top_level.txt
+-rw-r--r--   0 jespinoz  (3456) staff       (20)       38 2023-06-09 22:37:52.496064 clairvoyance_feature_selection-2023.6.9/setup.cfg
+-rw-------   0 jespinoz  (3456) staff       (20)     1026 2022-12-27 22:38:27.000000 clairvoyance_feature_selection-2023.6.9/setup.py
```

### Comparing `clairvoyance_feature_selection-2023.6.26/README.md` & `clairvoyance_feature_selection-2023.6.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Reimplementation for `Clairvoyance` from [Espinoza & Dupont et al. 2021](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1008857).  The updated version includes regression support, support for all linear/tree-based models, and improved visualizations.  `Clairvoyance` is currently in active development.   
 
 
 #### Details:
 `import clairvoyance as cy`
 
-`__version__ = "2023.6.26"`
+`__version__ = "2023.6.9"`
 
 #### Installation
 
 ```
 # Stable:
 pip install clairvoyance_feature_selection
 conda install -c jolespin clairvoyance
@@ -36,15 +36,15 @@
 *  Supports any `Scikit-Learn` compatible performance metric
 *  Supports regression (in addition to classification as in original implementation)
 *  Properly implements transformations for compositional data (e.g., CLR and closure) based on the query features for each iteration
 *  Added option to remove zero weighted features and redundant feature sets
 *  Added asymmetric mode in addition to the symmetric mode from the original implementation
 *  Added informative publication-ready plots
 *  Outputs multiple combinations of hyperparameters and scores for each feature combination
-*  Option to use testing sets or alternative models for recursive feature inclusion
+*  Option to use validation sets or alternative models for recursive feature inclusion
 
 
 #### Usage
 
 
 
 ##### Feature selection based on classification tasks
@@ -160,34 +160,31 @@
 
 ##### Feature selection based on regression tasks
 Here's a basic regression using a `DecisionTreeRegressor` model and a grid search for different `min_samples_leaf` and `min_samples_split` parameters. We add 87 noise variables and normalize all of the features so their scale is standardized.  In this case, we are optimizing for `neg_root_mean_squared_error`.  We are using a validation set of ~16% of the data during our recursive feature inclusion. For decision trees, we have the issue of getting zero-weighted features which are uninformative and misleading for RCI.  To get around this, we implement a recursive feature removal that only keeps non-zero weighted features.  We can turn this on via `remove_zero_weighted_features=True`.  This also ensures that there are no redundant feature sets (not an issue when `remove_zero_weighted_features=False` because they are recursively added).  
 
 Note: When we use `remove_zero_weighted_features=True`, we get a scatter plot instead of a line plot with error because there are multiple feature sets (each with their own performance distribution on the CV set) that may have the same number of features.
 
 ```python
+from sklearn.datasets import load_boston
 from sklearn.tree import DecisionTreeRegressor
 from sklearn.model_selection import train_test_split
 
 # Load Boston data
-# from sklearn.datasets import load_boston; boston = load_boston() # Deprecated
-data_url = "http://lib.stat.cmu.edu/datasets/boston"
-raw_df = pd.read_csv(data_url, sep="\s+", skiprows=22, header=None)
-data = np.hstack([raw_df.values[::2, :], raw_df.values[1::2, :2]])
-target = raw_df.values[1::2, 2]
-X = pd.DataFrame(data, columns=['CRIM', 'ZN', 'INDUS', 'CHAS', 'NOX', 'RM', 'AGE', 'DIS', 'RAD', 'TAX', 'PTRATIO', 'B', 'LSTAT'])
-y = pd.Series(target)
+boston = load_boston()
+X = pd.DataFrame(boston.data, columns=boston.feature_names)
+y = pd.Series(boston.target)
 
 number_of_noise_features = 100 - X.shape[1]
 X_noise = pd.DataFrame(np.random.RandomState(0).normal(size=(X.shape[0], number_of_noise_features)),  columns=map(lambda j: f"noise_{j}", range(number_of_noise_features)))
 X_boston_with_noise = pd.concat([X, X_noise], axis=1)
 X_normalized = X_boston_with_noise - X_boston_with_noise.mean(axis=0).values
 X_normalized = X_normalized/X_normalized.std(axis=0).values
 
-# Let's fit the model but leave a held out testing set
-X_training, X_testing, y_training, y_testing = train_test_split(X_normalized, y, random_state=0, test_size=0.3)
+# Let's fit the model but leave a held out validation set
+X_training, X_validation, y_training, y_validation = train_test_split(X_normalized, y, random_state=0, test_size=0.1618)
 
 # Get parameters
 estimator = DecisionTreeRegressor(random_state=0)
 param_grid = {"min_samples_leaf":[1,2,3,5,8],"min_samples_split":{ 0.1618, 0.382, 0.5, 0.618}}
 
 # Fit model
 reg = cy.ClairvoyanceRegression(
@@ -196,88 +193,81 @@
 	n_draws=10, 
 	estimator=estimator, 
 	param_grid=param_grid, 
 	verbose=1,
 	remove_zero_weighted_features=True,
 )
 reg.fit(X_training, y_training)
-history = reg.recursive_feature_inclusion(early_stopping=10, X=X_training, y=y_training, X_testing=X_testing, y_testing=y_testing)
+history = reg.recursive_feature_inclusion(early_stopping=10, X=X_validation, y=y_validation)
 history.head()
 ```
 ![](images/6.png)
 
 ```python
 reg.plot_scores(title="Boston", xtick_rotation=90)
 reg.plot_weights()
 reg.plot_weights(weight_type="cross_validation")
 ```
 ![](images/7.png)
 
-Let's see if we can increase the performance using the weights fitted with a `DecisionTreeRegressor` but with an ensemble `GradientBoostingRegressor` for the actual feature inclusion algorithm. 
+There's some noise features that make it through using `DecisionTreeRegressor` models.  Instead of adding a penalty, let's use the weights fitted with a `DecisionTreeRegressor` but use an ensemble `RandomForestRegressor` for the actual feature inclusion algorithm. 
 
 ```python
-from sklearn.ensemble import GradientBoostingRegressor
-# Get the relevant parameters from the DecisionTreeRegressor that will be be applicable to the ensemble
-relevant_params_from_best_decisiontree_estimator = {k:reg.best_estimator_.get_params()[k] for k in ["criterion", "min_samples_split"]}
-# Get estimator
-estimator = GradientBoostingRegressor(random_state=0, **relevant_params_from_best_decisiontree_estimator)
-# Recursive feature inclusion using ensemble 
-history = reg.recursive_feature_inclusion(early_stopping=10, estimator=estimator, X=X_training, y=y_training, X_testing=X_testing, y_testing=y_testing)
+from sklearn.ensemble import RandomForestRegressor
+history = reg.recursive_feature_inclusion(early_stopping=10, estimator=RandomForestRegressor(random_state=0), X=X_validation, y=y_validation)
 reg.plot_scores(title="Boston", xtick_rotation=90)
 reg.plot_weights()
 reg.plot_weights(weight_type="cross_validation")
-
-
 ```
 ![](images/8.png)
 
-RMSE is looking better.
+That's much better...
 
 ##### Recursive feature selection based on classification tasks
 Here we are running `Clairvoyance` recursively identifying several feature sets that work with different hyperparameters to get a range of feature sets to select from in the end.  We will iterate through all of the hyperparamater configurations, recursively feed in the data using different percentiles of the weights, and use different score thresholds from the random draws.  The recursive usage is similar to the legacy implementation used in [Espinoza & Dupont et al. 2021](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1008857) (which is still provided as an executable).
 
 ```python
-# Get the iris data (again)
+# Get the iris data again
 X_normalized = X_iris_with_noise - X_iris_with_noise.mean(axis=0).values
 X_normalized = X_normalized/X_normalized.std(axis=0).values
 target_names = load_iris().target_names
 y = pd.Series(load_iris().target)
 y = y.map(lambda i: target_names[i])
 
 # Specify model algorithm and parameter grid
 estimator=LogisticRegression(max_iter=1000, solver="liblinear", multi_class="ovr")
 param_grid={
     "C":[1e-10] + (np.arange(1,11)/10).tolist(),
     "penalty":["l1", "l2"],
 }
 
 # Instantiate model
-X_training, X_testing, y_training, y_testing = train_test_split(X_normalized, y, random_state=0, test_size=0.3)
-
 rci = cy.ClairvoyanceRecursive(
     n_jobs=-1, 
     scorer="accuracy", 
     n_draws=10, 
     estimator=estimator, 
     param_grid=param_grid, 
     percentiles=[0.0, 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 0.925, 0.95, 0.975, 0.99],
     minimum_scores=[-np.inf, 0.382, 0.5],
     verbose=0,
     remove_zero_weighted_features=False,
 )
-rci.fit(X=X_training, y=y_training, X_testing=X_testing, y_testing=y_testing, sort_hyperparameters_by=["C", "penalty"], ascending=[True, True])
+rci.fit(X_normalized, y, sort_hyperparameters_by=["C", "penalty"], ascending=[True, True])
 rci.plot_recursive_feature_selection()
 
 ```
+
+We observe a nice separate around 10 features, so let's use that as a maximum. 
+
 ![](images/9.png)
 
 ```python
-# Plot score comparisons
-rci.plot_scores_comparison()
-rci.get_history().head()
-```
+# Plot the features with a maximum of 10
+rci.plot_recursive_feature_selection(max_features=10)
 
-Let's see which feature sets have the highest validation score (i.e., average cross-validation score) and highest testing score (not used during RCI) while also considering the number of features.
+# Filter out all the results that have more than 10 features
+rci.results_.query("number_of_features <= 10").sort_values("score", ascending=False).head()
+```
 
 ![](images/10.png)
 
-Looks like there are several hyperparameter sets that can predict at > 92% accuracy on the cross-validation and > 95% accuracy on the testing set using just the `petal_length` and `petal_width`.  This was able to filter out both the 96 noise features and the 2 non-informative real features.
```

### Comparing `clairvoyance_feature_selection-2023.6.26/bin/clairvoyance_v1.py` & `clairvoyance_feature_selection-2023.6.9/bin/clairvoyance_v1.py`

 * *Files identical despite different names*

### Comparing `clairvoyance_feature_selection-2023.6.26/clairvoyance/clairvoyance.py` & `clairvoyance_feature_selection-2023.6.9/clairvoyance/clairvoyance.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 import matplotlib.pyplot as plt
 import seaborn as sns
 
 # Machine learning
 from scipy import stats
 from sklearn.metrics import get_scorer, make_scorer
 from sklearn.model_selection import cross_val_score, train_test_split, RepeatedStratifiedKFold, StratifiedKFold, RepeatedKFold, KFold
+from sklearn.linear_model import LogisticRegression
+from sklearn.tree import DecisionTreeClassifier
 from sklearn.base import clone, is_classifier, is_regressor
 from sklearn.exceptions import ConvergenceWarning, UndefinedMetricWarning
 
 # # Parallel
 # import ray
 # from ray.air.config import ScalingConfig
 # from ray.train.sklearn import SklearnTrainer
@@ -277,15 +279,14 @@
     index = list()
     for id_class in y.unique():
         class_samples = y[lambda x: x == id_class].index
         assert len(class_samples) >= subset_size_per_class
         subset = np.random.RandomState(random_state).choice(class_samples, size=subset_size_per_class, replace=False)
         index += subset.tolist()
     return index
-
 def recursive_feature_inclusion(
     estimator, 
     X:pd.DataFrame, 
     y:pd.Series, 
     scorer,
     initial_feature_weights:pd.Series, 
     initial_feature_weights_name:str="initial_feature_weights",
@@ -307,43 +308,43 @@
     testing_column="testing_index", 
     cv_prefix="cv=",
     verbose=0,
     log=sys.stdout,
     progress_message="Recursive feature inclusion",
     remove_zero_weighted_features=True,
     maximum_tries_to_remove_zero_weighted_features=1000,
-    X_testing:pd.DataFrame=None,
-    y_testing:pd.Series=None,
-    # optimize_testing_score = "auto",
+    X_validation:pd.DataFrame=None,
+    y_validation:pd.Series=None,
+    # optimize_validation_score = "auto",
     ) -> pd.Series:
 
     assert len(set(X.columns)) == X.shape[1], "Cannot have duplicate feature names in `X`"
     if additional_feature_penalty is None:
         additional_feature_penalty = lambda number_of_features: 0.0
 
-    # Testing
-    X_testing_is_provided = X_testing is not None
-    y_testing_is_provided = y_testing is not None
-
-    if X_testing_is_provided is not None:
-        assert y_testing_is_provided is not None, "If `X_testing` is provided then `y_testing` must be provided"
-
-    if y_testing_is_provided is not None:
-        assert X_testing_is_provided is not None, "If `y_testing` is provided then `X_testing` must be provided"
-
-    testing_set_provided = False
-    if all([X_testing_is_provided, y_testing_is_provided]):
-        assert np.all(X_testing.index == y_testing.index), "X_testing.index and y_testing.index must have the same ordering"
-        assert np.all(X_testing.columns == X.columns), "X_testing.columns and X.columns must have the same ordering"
-        testing_set_provided = True
-    # if optimize_testing_score == "auto":
-    #     if testing_set_provided:
-    #         optimize_testing_score = True
+    # Validation
+    X_validation_is_provided = X_validation is not None
+    y_validation_is_provided = y_validation is not None
+
+    if X_validation_is_provided is not None:
+        assert y_validation_is_provided is not None, "If `X_validation` is provided then `y_validation` must be provided"
+
+    if y_validation_is_provided is not None:
+        assert X_validation_is_provided is not None, "If `y_validation` is provided then `X_validation` must be provided"
+
+    validation_set_provided = False
+    if all([X_validation_is_provided, y_validation_is_provided]):
+        assert np.all(X_validation.index == y_validation.index), "X_validation.index and y_validation.index must have the same ordering"
+        assert np.all(X_validation.columns == X.columns), "X_validation.columns and X.columns must have the same ordering"
+        validation_set_provided = True
+    # if optimize_validation_score == "auto":
+    #     if validation_set_provided:
+    #         optimize_validation_score = True
     #     else:
-    #         optimize_testing_score = False
+    #         optimize_validation_score = False
 
     # Transformations
     assert_acceptable_arguments(transformation, {None,"clr","closure"})
     if multiplicative_replacement is None:
         multiplicative_replacement = 0.0
     if isinstance(multiplicative_replacement, str):
         assert multiplicative_replacement == "auto", "If `multiplicative_replacement` is a string, it must be `auto`"
@@ -369,15 +370,15 @@
         maximum_number_of_features = X.shape[1]
     if maximum_number_of_features is None:
         maximum_number_of_features = X.shape[1]
     assert maximum_number_of_features > 0, "maximum_number_of_features must be greater than 0"
 
     # Best results
     history = OrderedDict()
-    testing_scores = OrderedDict()
+    validation_scores = OrderedDict()
 
     best_features = None
     best_score = target_score
 
     # Feature tracker
     feature_tuples = list()
     unique_feature_sets = list()
@@ -443,47 +444,47 @@
                 # Training/Testing Scores
                 scores = cross_val_score(estimator=estimator, X=X_rfi, y=y, cv=cv_splits, n_jobs=n_jobs, scoring=scorer)
 
                 average_score = np.mean(scores)
                 history[i] = scores #{"average_score":average_score, "sem":sem}
 
                 #! ---
-                # Testing Score
+                # Validation Score
                 query_score = average_score
-                testing_score = np.nan
-                if testing_set_provided:
+                validation_score = np.nan
+                if validation_set_provided:
                     estimator.fit(
                         X=X_rfi, 
                         y=y,
                     )
                     
                     # Transform features (if transformation = None, then there is no transformation)
-                    X_testing_rfi = transform(X=X_testing.loc[:,features], method=transformation, multiplicative_replacement=multiplicative_replacement, axis=1)
-                    testing_score = scorer(estimator=estimator, X=X_testing_rfi, y_true=y_testing)
-                    testing_scores[i] = testing_score
-                    # if optimize_testing_score:
-                    #     query_score = testing_score
+                    X_validation_rfi = transform(X=X_validation.loc[:,features], method=transformation, multiplicative_replacement=multiplicative_replacement, axis=1)
+                    validation_score = scorer(estimator=estimator, X=X_validation_rfi, y_true=y_validation)
+                    validation_scores[i] = validation_score
+                    # if optimize_validation_score:
+                    #     query_score = validation_score
                 #! ---
 
                 # Add penalties to score target
                 penalty_adjusted_score_target = (best_score + minimum_improvement_in_score + additional_feature_penalty(len(features)))
                 
                 if query_score <= penalty_adjusted_score_target:
                     if verbose > 1:
-                        # if optimize_testing_score:
-                        #     print("Current iteration {} of N={} features has not improved score: Testing Score[{} ≤ {}]".format(i, len(features), testing_score, best_score), file=log)
+                        # if optimize_validation_score:
+                        #     print("Current iteration {} of N={} features has not improved score: Validation Score[{} ≤ {}]".format(i, len(features), validation_score, best_score), file=log)
                         # else:
                         print("Current iteration {} of N={} features has not improved score: Average Score[{} ≤ {}]".format(i, len(features), average_score, best_score), file=log)
 
                     no_progress += 1
                 else:
-                    # if optimize_testing_score:
+                    # if optimize_validation_score:
                     #     if verbose > 0:
-                    #         print("Updating best score with N={} features : Testing Score[{} -> {}]".format(len(features), best_score, testing_score), file=log)
-                    #     best_score = testing_score
+                    #         print("Updating best score with N={} features : Validation Score[{} -> {}]".format(len(features), best_score, validation_score), file=log)
+                    #     best_score = validation_score
                     # else:
                     if verbose > 0:
                         print("Updating best score with N={} features : Average Score[{} -> {}]".format(len(features), best_score, average_score), file=log)
                     best_score = average_score
                     best_features = features
                     no_progress = 0
                 if no_progress >= early_stopping:
@@ -495,67 +496,60 @@
     if verbose > 0:
         if best_features is None:
             print("Terminating algorithm after {} iterations with a best score of {} as no feature set improved the score with current parameters".format(i+1, best_score), file=log)
         else:
             print("Terminating algorithm at N={} features after {} iterations with a best score of {}".format(len(best_features), i+1, best_score), file=log)
     
     history = pd.DataFrame(history, index=list(map(lambda x: ("splits", x), cv_labels))).T
-    # if testing_set_provided:
-    #     history[("testing","score")] = pd.Series(testing_scores)
+    # if validation_set_provided:
+    #     history[("validation","score")] = pd.Series(validation_scores)
     history.index = feature_tuples
     history.index.name = "features"
     
     # Summary
     average_scores = history.mean(axis=1)
     sems = history.sem(axis=1)
-    if testing_set_provided:
-        testing_scores = pd.Series(testing_scores)
-        testing_scores.index = feature_tuples
+    if validation_set_provided:
+        validation_scores = pd.Series(validation_scores)
+        validation_scores.index = feature_tuples
     else:
-        testing_scores = pd.Series([np.nan]*len(feature_tuples), index=feature_tuples)
+        validation_scores = pd.Series([np.nan]*len(feature_tuples), index=feature_tuples)
     
     history.insert(loc=0, column=("summary", "number_of_features"),value = history.index.map(len))
     history.insert(loc=1, column=("summary", "average_score"),value = average_scores)
     history.insert(loc=2, column=("summary", "sem"),value = sems)
-    history.insert(loc=3, column=("summary", "testing_score"), value = testing_scores)
-    history.insert(loc=4, column=("summary", "∆(testing_score-average_score)"), value = average_scores - testing_scores)
+    history.insert(loc=3, column=("summary", "validation_score"), value = validation_scores)
+    history.insert(loc=4, column=("summary", "∆(validation_score-average_score)"), value = average_scores - validation_scores)
 
     history.columns = pd.MultiIndex.from_tuples(history.columns)
 
     
     # Highest scoring features (not necessarily the best since there can be many features added with minimal gains)
-    # if optimize_testing_score:
-    #     highest_score = history[("summary", "testing_score")].max()
-    #     highest_scoring_features = list(history.loc[history[("summary", "testing_score")] == highest_score].sort_values(
+    # if optimize_validation_score:
+    #     highest_score = history[("summary", "validation_score")].max()
+    #     highest_scoring_features = list(history.loc[history[("summary", "validation_score")] == highest_score].sort_values(
     #         by=[("summary", "average_score"), ("summary", "number_of_features")], 
     #         ascending=[False, less_features_is_better]).index[0])
     # else:
     highest_score = history[("summary", "average_score")].max()
     highest_scoring_features = list(history.loc[history[("summary", "average_score")] == highest_score, ("summary", "number_of_features")].sort_values(ascending=less_features_is_better).index[0])
     
     # # Best results
-    # if optimize_testing_score:
-    #     # best_features = list(history.loc[history[("summary", "testing_score")] == best_score].sort_values(
+    # if optimize_validation_score:
+    #     # best_features = list(history.loc[history[("summary", "validation_score")] == best_score].sort_values(
     #     #     by=[("summary", "average_score"), ("summary", "number_of_features")], 
     #     #     ascending=[False, less_features_is_better]).index[0])
     # else:
     #     best_features = list(history.loc[history[("summary", "average_score")] == best_score, ("summary", "number_of_features")].sort_values(ascending=less_features_is_better).index[0])
-
-    if testing_set_provided:
-        best_features = list(history.sort_values(
-            by=[("summary", "testing_score"), ("summary", "average_score"), ("summary", "number_of_features")], 
-            ascending=[False, False, less_features_is_better]).index[0])
-
-    else:
-        best_features = list(history.loc[history[("summary", "average_score")] == best_score].sort_values(
-            by=[("summary", "testing_score"), ("summary", "average_score"), ("summary", "number_of_features")], 
-            ascending=[False, False, less_features_is_better]).index[0])
+    best_features = list(history.loc[history[("summary", "average_score")] == best_score].sort_values(
+        by=[("summary", "validation_score"), ("summary", "average_score"), ("summary", "number_of_features")], 
+        ascending=[False, False, less_features_is_better]).index[0])
     
     best_estimator_sem = history.loc[[tuple(best_features)],("summary","sem")].values[0]
-    best_estimator_testing_score = history.loc[[tuple(best_features)],("summary","testing_score")].values[0]
+    best_estimator_validation_score = history.loc[[tuple(best_features)],("summary","validation_score")].values[0]
 
     best_estimator_rci = clone(estimator)
     X_best_features = transform(X=X.loc[:,best_features], method=transformation, multiplicative_replacement=multiplicative_replacement, axis=1)
 
     with warnings.catch_warnings():
         warnings.filterwarnings("ignore", category=ConvergenceWarning)
         best_estimator_rci.fit(X_best_features, y)
@@ -598,33 +592,33 @@
         best_features=best_features,
         best_estimator_rci=best_estimator_rci,
         feature_weights=feature_weights,
         highest_score=highest_score,
         highest_scoring_features=highest_scoring_features,
         cv_splits=cv_splits, 
         cv_labels=cv_labels,
-        testing_scores=testing_scores,
-        best_estimator_testing_score=best_estimator_testing_score,
+        validation_scores=validation_scores,
+        best_estimator_validation_score=best_estimator_validation_score,
         ),
         name="recursive_feature_elimination",
     )
 
 
 # Plotting
 def plot_scores_line(
     average_scores:pd.Series, 
     sem:pd.Series, 
-    testing_scores:pd.Series=None, 
+    validation_scores:pd.Series=None, 
     horizontal_lines=True,
     vertical_lines="auto",
     title=None,
     figsize=(13,3), 
     linecolor="black",
     errorcolor="gray",
-    testing_linecolor="red",
+    validation_linecolor="red",
     style="seaborn-white",
     xlim=None,
     ylim=None,
     ax=None, 
     alpha=0.382, 
     xlabel="$N_{Features}$", 
     ylabel="Score", 
@@ -652,17 +646,17 @@
             fig, ax = plt.subplots(figsize=figsize)
         else:
             fig = plt.gcf()
         
         average_scores.plot(ax=ax, color=linecolor, label="Average score", **kwargs)
         x_grid = np.arange(average_scores.size)
         ax.fill_between(x_grid, y1=average_scores-sem, y2=average_scores+sem, alpha=alpha, color=errorcolor, label="SEM")
-        if testing_scores is not None:
-            if not np.all(testing_scores.isnull()):
-                testing_scores.plot(ax=ax, color=testing_linecolor, label="Testing score", **kwargs)
+        if validation_scores is not None:
+            if not np.all(validation_scores.isnull()):
+                validation_scores.plot(ax=ax, color=validation_linecolor, label="Validation score", **kwargs)
 
         rci = np.argmax(average_scores.values) 
         if vertical_lines == "auto":
             vertical_lines = rci
         if isinstance(vertical_lines, (float,np.floating, int, np.integer)):
             vertical_lines = [vertical_lines]
         
@@ -835,22 +829,22 @@
             ax.yaxis.grid(True)
         return fig, ax
 
 def plot_recursive_feature_selection(
     number_of_features:pd.Series, 
     average_scores:pd.Series, 
     # sem:pd.Series=None, 
-    # Testing_scores:pd.Series=None,
+    # validation_scores:pd.Series=None,
     min_features:int=None,
     max_features:int=None,
     min_score:float=None,
     max_score:float=None,
     ax=None,
     color="darkslategray",
-    color_testing="red",
+    color_validation="red",
     linewidth=0.618,
     alpha=0.618,
     edgecolor="black", 
     style="seaborn-white",
     figsize=(8,3),
     title=None,
     xlabel="$N_{Features}$",
@@ -915,40 +909,39 @@
         if show_ygrid:
             ax.yaxis.grid(True)
         return fig, ax
     
 def plot_scores_comparison(
     number_of_features:pd.Series, 
     average_scores:pd.Series, 
-    testing_scores:pd.Series=None,
+    validation_scores:pd.Series=None,
     min_features:int=None,
     max_features:int=None,
     min_score:float=None,
     max_score:float=None,
     ax=None,
     color="darkslategray",
     linewidth=0.618,
     alpha=0.618,
     edgecolor="black", 
     style="seaborn-white",
     figsize=(8,5),
     title=None,
     xlabel="Average Score",
-    ylabel="Testing Score",
+    ylabel="Validation Score",
 
     feature_to_size_function = "auto",
 
     xtick_rotation=0,
-    show_xgrid=True,
+    show_xgrid=False,
     show_ygrid=True,
     # show_zgrid=True,
 
     show_xticks=True, 
     show_legend=True,
-    legend_markers=["min", "25%", "50%", "75%", "max"],
     xlabel_kws=dict(), 
     ylabel_kws=dict(), 
     # zlabel_kws=dict(), 
 
     xticklabel_kws=dict(), 
     yticklabel_kws=dict(),
     # zticklabel_kws=dict(),
@@ -956,41 +949,39 @@
     title_kws=dict(),
     legend_kws=dict(),
     **kwargs,
     ):
 
     assert isinstance(number_of_features, pd.Series)
     assert isinstance(average_scores, pd.Series)
-    assert isinstance(testing_scores, pd.Series)
-    assert set(legend_markers) <= set(["min", "25%", "50%", "75%", "max"]), 'legend_markers must be a subset of ["min", "25%", "50%", "75%", "max"]'
-    legend_markers = sorted(legend_markers, key=lambda x:["min", "25%", "50%", "75%", "max"].index(x))
+    assert isinstance(validation_scores, pd.Series)
 
     assert np.all(number_of_features.index == average_scores.index)
-    assert np.all(number_of_features.index == testing_scores.index)
+    assert np.all(number_of_features.index == validation_scores.index)
 
-    df = pd.DataFrame([number_of_features, average_scores, testing_scores], index=["number_of_features", "average_scores", "testing_scores"]).T
+    df = pd.DataFrame([number_of_features, average_scores, validation_scores], index=["number_of_features", "average_scores", "validation_scores"]).T
 
     if min_features:
         df = df.query("number_of_features >= {}".format(min_features))
     if max_features:
         df = df.query("number_of_features <= {}".format(max_features))
     if min_score:
         df = df.query("average_scores >= {}".format(min_score))
     if max_score:
         df = df.query("average_scores <= {}".format(max_score))
     if min_score:
-        df = df.query("testing_scores >= {}".format(min_score))
+        df = df.query("validation_scores >= {}".format(min_score))
     if max_score:
-        df = df.query("testing_scores <= {}".format(max_score))
+        df = df.query("validation_scores <= {}".format(max_score))
 
     if feature_to_size_function == "auto":
         def feature_to_size_function(n):
             return 100/n
     assert hasattr(feature_to_size_function, "__call__")
-    marker_sizes = feature_to_size_function(number_of_features)
+    s = feature_to_size_function(number_of_features)
 
     with plt.style.context(style):
         _title_kws = {"fontsize":16, "fontweight":"bold"}; _title_kws.update(title_kws)
         _xlabel_kws = {"fontsize":15}; _xlabel_kws.update(xlabel_kws)
         _ylabel_kws = {"fontsize":15}; _ylabel_kws.update(ylabel_kws)
         # _zlabel_kws = {"fontsize":15}; _zlabel_kws.update(zlabel_kws)
 
@@ -1002,38 +993,34 @@
         if ax is None:
             fig, ax = plt.subplots(figsize=figsize)
 
         else:
             fig = plt.gcf()
 
 
-        # ax.scatter(xs=df["number_of_features"].values, ys=df["average_scores"].values, zs=df["testing_scores"], edgecolor=edgecolor, alpha=alpha, linewidth=linewidth, color=color, **kwargs)
-        ax.scatter(x=df["average_scores"].values, y=df["testing_scores"], s=marker_sizes, edgecolor=edgecolor, alpha=alpha, linewidth=linewidth, color=color, **kwargs)
+        # ax.scatter(xs=df["number_of_features"].values, ys=df["average_scores"].values, zs=df["validation_scores"], edgecolor=edgecolor, alpha=alpha, linewidth=linewidth, color=color, **kwargs)
+        ax.scatter(x=df["average_scores"].values, y=df["validation_scores"], s=s, edgecolor=edgecolor, alpha=alpha, linewidth=linewidth, color=color, **kwargs)
 
 
         ax.set_xlabel(xlabel, **_xlabel_kws)
         ax.set_ylabel(ylabel, **_ylabel_kws)
         # ax.set_zlabel(zlabel, **_zlabel_kws)
 
         # ax.set_yticklabels(map(lambda x:"%0.2f"%x, ax.get_yticks()), **_yticklabel_kws)
         if title:
             ax.set_title(title, **_title_kws)
         if show_legend:
-            legendary_features = number_of_features.describe()[legend_markers].astype(int)
+            legendary_features = number_of_features.describe()[["25%", "50%", "75%", "max"]].astype(int)
             
             legend_elements = list()
-            for i,n in legendary_features.items():
-                # marker = plt.Line2D([], [], color=color, marker='o', linestyle='None', markersize=feature_to_size_function(n), label="$N$ = %d"%(n))
-                # legend_elements.append(marker)
-                i = i.replace("%","\%")
-                legend_marker = ax.scatter([], [], s=feature_to_size_function(n), label="$N_{%s}$ = %d"%(i,n), color=color, marker='o')
-                legend_elements.append(legend_marker)
-
+            for n in legendary_features.values:
+                marker = plt.Line2D([], [], color=color, marker='o', linestyle='None', markersize=feature_to_size_function(n), label="$N$ = %d"%(n))
+                legend_elements.append(marker)
 
-            legend = ax.legend(handles=legend_elements,  title="$N_{Features}$",  markerscale=1, **_legend_kws)
+            legend = ax.legend(handles=legend_elements, markerscale=1,title="$N_{Features}$",  **_legend_kws)
             
         if show_xgrid:
             ax.xaxis.grid(True)
         if show_ygrid:
             ax.yaxis.grid(True)
         # if show_zgrid:
         #     ax.zaxis.grid(True)
@@ -1103,15 +1090,15 @@
         # Set attributes
         self.name = name
         self.observation_type = observation_type
         self.feature_type = feature_type
         self.target_type = target_type
         self.is_fitted_weights = False
         self.is_fitted_rci = False
-        self.testing_set_provided = False
+        self.validation_set_provided = False
         self.n_draws = n_draws
         self.n_jobs = n_jobs
         self.random_state = random_state
         if isinstance(scorer, str):
             scorer = get_scorer(scorer)
         self.scorer = scorer
         self.scorer_name = scorer._score_func.__name__
@@ -1430,31 +1417,31 @@
     
     
     def recursive_feature_inclusion(
         self, 
         estimator=None, 
         X:pd.DataFrame=None, 
         y:pd.Series=None, 
-        X_testing:pd.DataFrame=None,
-        y_testing:pd.Series=None,
+        X_validation:pd.DataFrame=None,
+        y_validation:pd.Series=None,
         cv=(5,3), 
         minimum_score=None, 
         metric=np.mean, 
         early_stopping=25, 
         target_score=-np.inf, 
         minimum_improvement_in_score=0.0, 
         additional_feature_penalty=None,
         maximum_number_of_features=np.inf,
         less_features_is_better=True, 
         training_column="training_index", 
         testing_column="testing_index", 
         cv_prefix="cv=", 
         copy_X_rci=True,
         progress_message="Recursive feature inclusion",
-        # optimize_testing_score = "auto",
+        # optimize_validation_score = "auto",
 
         ):
         assert self.is_fitted_weights, "Please `fit` model before proceeding."
 
         if X is None:
             X = self.X_.copy()
         else:
@@ -1468,29 +1455,29 @@
 
         if estimator is None:
             estimator = self.best_estimator_
 
         self.clairvoyance_feature_weights_ = self.get_weights(minimum_score=minimum_score, metrics=metric).sort_values(ascending=False)
         self.rci_parameters_ = {"estimator":estimator, "cv":cv, "minimum_score":minimum_score, "metric":metric, "early_stopping":early_stopping, "target_score":target_score, "less_features_is_better":less_features_is_better}
         
-        # Testing
-        X_testing_is_provided = X_testing is not None
-        y_testing_is_provided = y_testing is not None
-
-        if X_testing_is_provided is not None:
-            assert y_testing_is_provided is not None, "If `X_testing` is provided then `y_testing` must be provided"
-
-        if y_testing_is_provided is not None:
-            assert X_testing_is_provided is not None, "If `y_testing` is provided then `X_testing` must be provided"
-
-        self.testing_set_provided = False
-        if all([X_testing_is_provided, y_testing_is_provided]):
-            assert np.all(X_testing.index == y_testing.index), "X_testing.index and y_testing.index must have the same ordering"
-            assert np.all(X_testing.columns == X.columns), "X_testing.columns and X.columns must have the same ordering"
-            self.testing_set_provided = True
+        # Validation
+        X_validation_is_provided = X_validation is not None
+        y_validation_is_provided = y_validation is not None
+
+        if X_validation_is_provided is not None:
+            assert y_validation_is_provided is not None, "If `X_validation` is provided then `y_validation` must be provided"
+
+        if y_validation_is_provided is not None:
+            assert X_validation_is_provided is not None, "If `y_validation` is provided then `X_validation` must be provided"
+
+        self.validation_set_provided = False
+        if all([X_validation_is_provided, y_validation_is_provided]):
+            assert np.all(X_validation.index == y_validation.index), "X_validation.index and y_validation.index must have the same ordering"
+            assert np.all(X_validation.columns == X.columns), "X_validation.columns and X.columns must have the same ordering"
+            self.validation_set_provided = True
 
 
         # Recursive feature incusion
         rci_results = recursive_feature_inclusion(
             estimator=estimator, 
             X=X, 
             y=y, 
@@ -1514,34 +1501,34 @@
             training_column=training_column, 
             testing_column=testing_column, 
             cv_prefix=cv_prefix,
             verbose=self.verbose,
             progress_message=progress_message,
             remove_zero_weighted_features=self.remove_zero_weighted_features,
             maximum_tries_to_remove_zero_weighted_features=self.maximum_tries_to_remove_zero_weighted_features,
-            X_testing=X_testing,
-            y_testing=y_testing,
-            # optimize_testing_score=optimize_testing_score,
+            X_validation=X_validation,
+            y_validation=y_validation,
+            # optimize_validation_score=optimize_validation_score,
             )
         
         # Results
-        # self.testing_scores_ = rci_results["testing_scores"]
+        # self.validation_scores_ = rci_results["validation_scores"]
         self.history_ = rci_results["history"]
         if self.remove_zero_weighted_features:
-            if self.testing_set_provided:
-                self.history_ = self.history_.sort_values([("summary", "testing_score"), ("summary", "average_score"), ("summary", "number_of_features")], ascending=[False, False, less_features_is_better])
+            if self.validation_set_provided:
+                self.history_ = self.history_.sort_values([("summary", "validation_score"), ("summary", "average_score"), ("summary", "number_of_features")], ascending=[False, False, less_features_is_better])
             else:
                 self.history_ = self.history_.sort_values([("summary", "average_score"), ("summary", "number_of_features")], ascending=[False, less_features_is_better])
         self.highest_score_ = rci_results["highest_score"]
         self.highest_scoring_features_ = rci_results["highest_scoring_features"]
         self.best_score_ = rci_results["best_score"]
         self.best_estimator_sem_ = rci_results["best_estimator_sem"]
         self.best_features_ = rci_results["best_features"]
         self.best_estimator_rci_ = clone(estimator)
-        self.best_estimator_testing_score_ = rci_results["best_estimator_testing_score"]
+        self.best_estimator_validation_score_ = rci_results["best_estimator_validation_score"]
 
         X_rci = transform(X=X.loc[:,self.best_features_], method=self.transformation, multiplicative_replacement=self.multiplicative_replacement, axis=1)
         with warnings.catch_warnings(): #!
             warnings.filterwarnings("ignore", category=ConvergenceWarning)
             self.best_estimator_rci_.fit(X_rci, y)
         self.feature_weights_ =  rci_results["feature_weights"]
         self.rci_feature_weights_ = rci_results["feature_weights"][("full_dataset", "rci_weights")].loc[self.best_features_]
@@ -1550,26 +1537,14 @@
         
         if copy_X_rci:
             self.X_rci_ = X_rci.copy()
             
         self.is_fitted_rci = True
         
         return self.history_
-
-    def get_history(self, sort_values_by=[("summary", "testing_score"), ("summary", "average_score"), ("summary", "number_of_features")], ascending=[False, False, True], summary=True):
-        assert self.is_fitted_rci, "Please run `fit` before proceeding."
-
-        df_history = self.history_.copy()
-
-        if sort_values_by is not None:
-            df_history = df_history.sort_values(by=sort_values_by, ascending=ascending)
-        if summary:
-            df_history = df_history["summary"]
-            
-        return df_history
     
     def plot_scores(
         self,
         ylabel="auto",
         **kwargs,
         ):
         if ylabel == "auto":
@@ -1580,15 +1555,15 @@
             vertical_lines = [len(self.best_features_)-1, len(self.highest_scoring_features_)-1]
         else:
             vertical_lines = [len(self.best_features_)-1]
 
         if self.remove_zero_weighted_features:
             return plot_recursive_feature_selection(number_of_features=self.history_[("summary", "number_of_features")], average_scores=self.history_[("summary", "average_score")],  **kwargs)
         else:
-            return plot_scores_line(average_scores=self.history_[("summary", "average_score")], sem=self.history_[("summary", "sem")], testing_scores=self.history_[("summary", "testing_score")], vertical_lines=vertical_lines, **kwargs)
+            return plot_scores_line(average_scores=self.history_[("summary", "average_score")], sem=self.history_[("summary", "sem")], validation_scores=self.history_[("summary", "validation_score")], vertical_lines=vertical_lines, **kwargs)
         
     def plot_weights(
         self,
         weight_type=("full_dataset","rci_weights"),
         **kwargs,
         ):
         assert self.is_fitted_rci, "Please run `recursive_feature_inclusion` before proceeding."
@@ -1601,16 +1576,16 @@
         return fig, ax
     
     def plot_scores_comparison(
         self,
         **kwargs,
         ):
         assert self.is_fitted_rci, "Please run `recursive_feature_inclusion` before proceeding."
-        assert self.testing_set_provided, "Please run `recursive_feature_inclusion` with a testing set before proceeding."
-        return plot_scores_comparison(number_of_features=self.history_[("summary", "number_of_features")], average_scores=self.history_[("summary", "average_score")],   testing_scores=self.history_[("summary", "testing_score")], **kwargs)
+        assert self.validation_set_provided, "Please run `recursive_feature_inclusion` with a validation set before proceeding."
+        return plot_recursive_feature_selection(number_of_features=self.history_[("summary", "number_of_features")], average_scores=self.history_[("summary", "average_score")],   validation_scores=self.history_[("summary", "validation_score")], **kwargs)
 
     def copy(self):
         return copy.deepcopy(self)
     
     # def to_file(self, path:str):
     #     write_object(self, path)  
         
@@ -1835,15 +1810,15 @@
         # Set attributes
         self.name = name
         self.observation_type = observation_type
         self.feature_type = feature_type
         self.target_type = target_type
         # self.is_fitted_weights = False
         self.is_fitted_rci = False
-        self.testing_set_provided = False
+        self.validation_set_provided = False
         self.n_draws = n_draws
         self.n_jobs = n_jobs
         self.random_state = random_state
         if isinstance(scorer, str):
             scorer = get_scorer(scorer)
         self.scorer = scorer
         self.scorer_name = scorer._score_func.__name__
@@ -1914,16 +1889,16 @@
 
         return "\n".join(fields)
     
     def fit(
         self, 
         X:pd.DataFrame, 
         y:pd.Series, 
-        X_testing:pd.DataFrame=None,
-        y_testing:pd.Series=None,
+        X_validation:pd.DataFrame=None,
+        y_validation:pd.Series=None,
         stratify="auto", 
         split_size=0.618033, 
         cv=(5,3),
         training_column="training_index", 
         testing_column="testing_index", 
         cv_prefix="cv=",
         sort_hyperparameters_by:list=None, 
@@ -1943,29 +1918,29 @@
         self.observation_ids_ = X.index
         self.feature_ids_initial_ = X.columns
         self.number_of_observations_, self.number_of_initial_features_ = X.shape
         self.stratify_ = format_stratify(stratify, estimator_type=self.estimator_type, y=self.y_)
         self.split_size = split_size
         self.maximum_number_of_features = maximum_number_of_features
 
-        # Testing
-        X_testing_is_provided = X_testing is not None
-        y_testing_is_provided = y_testing is not None
-
-        if X_testing_is_provided is not None:
-            assert y_testing_is_provided is not None, "If `X_testing` is provided then `y_testing` must be provided"
-
-        if y_testing_is_provided is not None:
-            assert X_testing_is_provided is not None, "If `y_testing` is provided then `X_testing` must be provided"
-
-        self.testing_set_provided = False
-        if all([X_testing_is_provided, y_testing_is_provided]):
-            assert np.all(X_testing.index == y_testing.index), "X_testing.index and y_testing.index must have the same ordering"
-            assert np.all(X_testing.columns == X.columns), "X_testing.columns and X.columns must have the same ordering"
-            self.testing_set_provided = True
+        # Validation
+        X_validation_is_provided = X_validation is not None
+        y_validation_is_provided = y_validation is not None
+
+        if X_validation_is_provided is not None:
+            assert y_validation_is_provided is not None, "If `X_validation` is provided then `y_validation` must be provided"
+
+        if y_validation_is_provided is not None:
+            assert X_validation_is_provided is not None, "If `y_validation` is provided then `X_validation` must be provided"
+
+        self.validation_set_provided = False
+        if all([X_validation_is_provided, y_validation_is_provided]):
+            assert np.all(X_validation.index == y_validation.index), "X_validation.index and y_validation.index must have the same ordering"
+            assert np.all(X_validation.columns == X.columns), "X_validation.columns and X.columns must have the same ordering"
+            self.validation_set_provided = True
             
         # Get cross-validation splits
         self.cv_splits_, self.cv_labels_ = format_cross_validation(cv, X, self.y_, stratify=self.stratify_, random_state=self.random_state, cv_prefix=cv_prefix, training_column=training_column, testing_column=testing_column)
 
         self.history_ = OrderedDict()
         self.results_ = OrderedDict()
         self.results_baseline_ = OrderedDict()
@@ -2040,23 +2015,23 @@
                             warnings.filterwarnings("ignore", category=ConvergenceWarning)
                             baseline_rci_weights = getattr(estimator.fit(X_query, self.y_), self.feature_weight_attribute)
                         if np.all(baseline_rci_weights == 0):
                             if self.verbose > 2:
                                 print("Excluding results from [percentile={}, estimator_params={}] becaue baseline model could not be fit with parameter set".format(pctl, params), file=self.log)
                         else:
 
-                            baseline_testing_score = np.nan
-                            if self.testing_set_provided:
+                            baseline_validation_score = np.nan
+                            if self.validation_set_provided:
                                 # Transform features (if transformation = None, then there is no transformation)
-                                X_testing_query = transform(X=X_testing.loc[:,current_features_for_percentile], method=self.transformation, multiplicative_replacement=self.multiplicative_replacement, axis=1)
-                                baseline_testing_score = self.scorer(estimator=estimator, X=X_testing_query, y_true=y_testing)
+                                X_validation_query = transform(X=X_validation.loc[:,current_features_for_percentile], method=self.transformation, multiplicative_replacement=self.multiplicative_replacement, axis=1)
+                                baseline_validation_score = self.scorer(estimator=estimator, X=X_validation_query, y_true=y_validation)
 
                             baseline_rci_weights = format_weights(baseline_rci_weights)
                             self.results_baseline_[(pctl,"baseline", params)] = {
-                                "testing_score":baseline_testing_score,
+                                "validation_score":baseline_validation_score,
                                 "average_score":np.nanmean(baseline_scores_for_percentile), 
                                 "sem":stats.sem(baseline_scores_for_percentile),
                                 "number_of_features":X_query.shape[1], 
                                 "features":X_query.columns.tolist(), 
                                 "clairvoyance_weights":np.nan,
                                 "rci_weights":baseline_rci_weights, 
                                 "estimator":estimator,
@@ -2076,19 +2051,19 @@
                                         minimum_improvement_in_score=self.minimum_improvement_in_score, 
                                         additional_feature_penalty=self.additional_feature_penalty,
                                         maximum_number_of_features=self.maximum_number_of_features,
                                         target_score=-np.inf, 
                                         less_features_is_better=less_features_is_better, 
                                         progress_message=progress_message,
                                 )
-                                if self.testing_set_provided:
+                                if self.validation_set_provided:
                                     rci_params.update(
                                         dict(
-                                        X_testing=X_testing.loc[:,current_features_for_percentile],
-                                        y_testing=y_testing,
+                                        X_validation=X_validation.loc[:,current_features_for_percentile],
+                                        y_validation=y_validation,
                                         )
                                     )
 
                                 rci_history = model.recursive_feature_inclusion(**rci_params)
 
 
 
@@ -2100,15 +2075,15 @@
                                     best_minimum_score_for_percentile = s
                                     best_clairvoyance_feature_weights_for_percentile = model.clairvoyance_feature_weights_.copy()
 
                                 # Store results
                                 rci_feature_weights = model.rci_feature_weights_[model.best_features_]
                                 if not np.any(rci_feature_weights.isnull()) and np.any(rci_feature_weights > 0):
                                     self.results_[(pctl, params, s)] = {
-                                        "testing_score":model.best_estimator_testing_score_,
+                                        "validation_score":model.best_estimator_validation_score_,
                                         "average_score":model.best_score_, 
                                         "sem":model.best_estimator_sem_,
                                         "number_of_features":len(model.best_features_), 
                                         "features":list(model.best_features_), 
                                         "clairvoyance_weights":model.clairvoyance_feature_weights_[model.best_features_].values.tolist(),
                                         "rci_weights":rci_feature_weights.values.tolist(), 
                                         "estimator":estimator,
@@ -2132,21 +2107,21 @@
                         if self.verbose > 0:
                             print("Terminating algorithm. Last percentile has been processed.", file=self.log)
                 else:
                     if self.verbose > 0:
                         print("Terminating algorithm. Only 1 feature remains.", file=self.log)
                     break
 
-            self.results_ = pd.DataFrame(self.results_).T.sort_values(["testing_score", "average_score", "number_of_features", "sem"], ascending=[False, False,less_features_is_better, True])
+            self.results_ = pd.DataFrame(self.results_).T.sort_values(["validation_score", "average_score", "number_of_features", "sem"], ascending=[False, False,less_features_is_better, True])
             self.results_.index.names = ["percentile", "hyperparameters", "minimum_score"]
 
-            self.results_ = self.results_.loc[:,["testing_score", "average_score", "sem", "number_of_features", "features", "clairvoyance_weights", "rci_weights", "estimator"]]
+            self.results_ = self.results_.loc[:,["validation_score", "average_score", "sem", "number_of_features", "features", "clairvoyance_weights", "rci_weights", "estimator"]]
 
             # Dtypes
-            for field in ["testing_score", "average_score", "sem"]:
+            for field in ["validation_score", "average_score", "sem"]:
                 self.results_[field] = self.results_[field].astype(float)
             for field in ["number_of_features"]:
                 self.results_[field] = self.results_[field].astype(int)
 
             # Remove redundancy
             if remove_redundancy:
                 unique_results = set()
@@ -2162,29 +2137,26 @@
                 self.results_ = self.results_.loc[unique_index]
             self.results_baseline_ = pd.DataFrame(self.results_baseline_).T
             self.results_baseline_.index.names = ["percentile", "hyperparameters", "minimum_score"]
 
             self.is_fitted_rci = True
             return self
 
-    def get_history(self, sort_values_by=[("summary", "testing_score"), ("summary", "average_score"), ("summary", "number_of_features")], ascending=[False, False, True], summary=True):
+    def get_history(self, sort_values_by=[("summary", "validation_score"), ("summary", "average_score"), ("summary", "number_of_features")], ascending=[False, False, True]):
         assert self.is_fitted_rci, "Please run `fit` before proceeding."
 
         dataframes = list()
         for params, df in self.history_.items(): # self.history_[(pctl,params, s)] = rci_history
-            df = df.copy()
             df.index = df.index.map(lambda x: (*params, x))
             df.index.names = ["percentile", "hyperparameters", "minimum_score", "features"]
             dataframes.append(df)
 
         df_concatenated = pd.concat(dataframes, axis=0)
         if sort_values_by is not None:
             df_concatenated = df_concatenated.sort_values(by=sort_values_by, ascending=ascending)
-        if summary:
-            df_concatenated = df_concatenated["summary"]
             
         return df_concatenated
 
 
     def plot_recursive_feature_selection(
         self,
         ylabel="auto",
@@ -2194,46 +2166,46 @@
         ):
         if ylabel == "auto":
             ylabel = self.scorer_name
         kwargs["ylabel"] = ylabel
         assert self.is_fitted_rci, "Please run `fit` before proceeding."
         
         if comprehensive == "auto":
-            if self.testing_set_provided:
+            if self.validation_set_provided:
                 comprehensive = True 
             else:
                 comprehensive = False
             
         if comprehensive:
-            df = self.get_history(summary=True)
-            number_of_features = df["number_of_features"]
-            average_scores = df["average_score"]
-            # Testing_scores = df[("summary", "testing_score")]
+            df = self.get_history()
+            number_of_features = df[("summary","number_of_features")]
+            average_scores = df[("summary", "average_score")]
+            # validation_scores = df[("summary", "validation_score")]
         else:
             number_of_features = self.results_["number_of_features"]
             average_scores = self.results_["average_score"]
-            testing_scores = self.results_["testing_score"]
+            validation_scores = self.results_["validation_score"]
             if include_baseline:
                 number_of_features = pd.concat([number_of_features, self.results_baseline_["number_of_features"]])
                 average_scores = pd.concat([average_scores, self.results_baseline_["average_score"]])
-                # Testing_scores = pd.concat([testing_scores, self.results_baseline_["testing_score"]])
+                # validation_scores = pd.concat([validation_scores, self.results_baseline_["validation_score"]])
 
         return plot_recursive_feature_selection(number_of_features=number_of_features, average_scores=average_scores,  **kwargs)
 
     def plot_scores_comparison(
         self,
         **kwargs,
         ):
         assert self.is_fitted_rci, "Please run `recursive_feature_inclusion` before proceeding."
-        assert self.testing_set_provided, "Please run `recursive_feature_inclusion` with a testing set before proceeding."
-        df = self.get_history(summary=True)
-        number_of_features = df["number_of_features"]
-        average_scores = df["average_score"]
-        testing_scores = df["testing_score"]
-        return plot_scores_comparison(number_of_features=number_of_features, average_scores=average_scores,   testing_scores=testing_scores, **kwargs)
+        assert self.validation_set_provided, "Please run `recursive_feature_inclusion` with a validation set before proceeding."
+        df = self.get_history()
+        number_of_features = df[("summary","number_of_features")]
+        average_scores = df[("summary", "average_score")]
+        validation_scores = df[("summary", "validation_score")]
+        return plot_scores_comparison(number_of_features=number_of_features, average_scores=average_scores,   validation_scores=validation_scores, **kwargs)
 
     def to_file(self, path:str):
         write_object(self, path)  
 
 
         
     @classmethod
@@ -2246,37 +2218,32 @@
 _______        _______ _____  ______ _    _  _____  __   __ _______ __   _ _______ _______
 |       |      |_____|   |   |_____/  \  /  |     |   \_/   |_____| | \  | |       |______
 |_____  |_____ |     | __|__ |    \_   \/   |_____|    |    |     | |  \_| |_____  |______
     """
     print(s, file=sys.stderr)
     print("Hello There.\nI live here: https://github.com/jolespin/clairvoyance", file=sys.stderr)
     if len(sys.argv) > 0:
-        if sys.argv[1] in {"--test", "-t"}:
-            from sklearn.linear_model import LogisticRegression
-            from sklearn.tree import DecisionTreeClassifier
-
-            # 1.
-
+        if sys.argv[1] == "test":
             # Classification
-            print(format_header("1. Running test for `ClairvoyanceClassification` on iris dataset with noise"), file=sys.stderr)
+            print("\nRunning test for `ClairvoyanceClassification`", file=sys.stderr)
             import numpy as np
             import pandas as pd
             from sklearn.datasets import load_iris
             from sklearn.linear_model import LogisticRegression
 
             # Load iris dataset
             X, y = load_iris(return_X_y=True, as_frame=True)
             X.columns = X.columns.map(lambda j: j.split(" (cm")[0].replace(" ","_"))
 
             # Relabel targets
             target_names = load_iris().target_names
             y = y.map(lambda i: target_names[i])
 
-            # Add 21 noise features (total = 25 features) in the same range of values as the original features
-            number_of_noise_features = 21
+            # Add 996 noise features (total = 1000 features) in the same range of values as the original features
+            number_of_noise_features = 46
             vmin = X.values.ravel().min()
             vmax = X.values.ravel().max()
             X_noise = pd.DataFrame(
                 data=np.random.RandomState(0).randint(low=int(vmin*10), high=int(vmax*10), size=(150, number_of_noise_features))/10,
                 columns=map(lambda j:"noise_{}".format(j+1), range(number_of_noise_features)),
             )
 
@@ -2300,97 +2267,76 @@
                 param_grid=param_grid, 
                 verbose=1,
             )
             clf.fit(X_normalized, y)#, sort_hyperparameters_by=["C", "penalty"], ascending=[True, False])
             history = clf.recursive_feature_inclusion(early_stopping=10)
             print(history.head(), file=sys.stdout)
 
-            # 2.
             # Regression
-            print(format_header("2. Running test for `ClairvoyanceRegression` on boston dataset with noise"), file=sys.stderr)
+            print("\nRunning test for `ClairvoyanceRegression`", file=sys.stderr)
             # from sklearn.datasets import fetch_openml
             from sklearn.tree import DecisionTreeRegressor
             from sklearn.model_selection import train_test_split
 
             # Load housing data
             # housing = fetch_openml(name="house_prices", as_frame=True)
             data_url = "http://lib.stat.cmu.edu/datasets/boston"
             raw_df = pd.read_csv(data_url, sep="\s+", skiprows=22, header=None)
             data = np.hstack([raw_df.values[::2, :], raw_df.values[1::2, :2]])
             target = raw_df.values[1::2, 2]
             X = pd.DataFrame(data, columns=['CRIM', 'ZN', 'INDUS', 'CHAS', 'NOX', 'RM', 'AGE', 'DIS', 'RAD', 'TAX', 'PTRATIO', 'B', 'LSTAT'])
             y = pd.Series(target)
 
-            number_of_noise_features = 25 - X.shape[1]
+            number_of_noise_features = 50 - X.shape[1]
             X_noise = pd.DataFrame(np.random.RandomState(0).normal(size=(X.shape[0], number_of_noise_features)),  columns=map(lambda j: f"noise_{j}", range(number_of_noise_features)))
             X_housing_with_noise = pd.concat([X, X_noise], axis=1)
             X_normalized = X_housing_with_noise - X_housing_with_noise.mean(axis=0).values
             X_normalized = X_normalized/X_normalized.std(axis=0).values
 
-            # Let's fit the model but leave a held out testing set
-            X_training, X_testing, y_training, y_testing = train_test_split(X_normalized, y, random_state=0, test_size=0.1618)
+            # Let's fit the model but leave a held out validation set
+            X_training, X_validation, y_training, y_validation = train_test_split(X_normalized, y, random_state=0, test_size=0.1618)
 
             # Get parameters
             estimator = DecisionTreeRegressor(random_state=0)
             param_grid = {"min_samples_leaf":[1,2,3,5,8],"min_samples_split":{ 0.1618, 0.382, 0.5, 0.618}}
 
             # Fit model
             reg = ClairvoyanceRegression(name="Housing", n_jobs=-1, n_draws=10, estimator=estimator, param_grid=param_grid, verbose=1)
             reg.fit(X_training, y_training)
-            history = reg.recursive_feature_inclusion(early_stopping=10, X=X_training, y=y_training, X_testing=X_testing, y_testing=y_testing)
+            history = reg.recursive_feature_inclusion(early_stopping=10, X=X_training, y=y_training, X_validation=X_validation, y_validation=y_validation)
             print(history.head(), file=sys.stdout)
 
-            # 3.
             # Recursive
-            print(format_header("3. Running test for `ClairvoyanceRecursive` on iris dataset with noise"), file=sys.stderr)
+            print("\nRunning test for `ClairvoyanceRecursive`", file=sys.stderr)
             from sklearn.tree import DecisionTreeClassifier
 
             X_normalized = X_iris_with_noise - X_iris_with_noise.mean(axis=0).values
             X_normalized = X_normalized/X_normalized.std(axis=0).values
             target_names = load_iris().target_names
             y = pd.Series(load_iris().target)
             y = y.map(lambda i: target_names[i])
 
             # Specify model algorithm and parameter grid
             estimator=DecisionTreeClassifier()
             param_grid={
                 "criterion":["gini","entropy"],
-                "max_features":["log2", "sqrt", 0.382, 0.618],
-                "min_samples_leaf":[1,2,3,5,8],
+                "max_features":["log2", "sqrt", None, 0.382, 0.618],
+                "min_samples_leaf":[1,2,3,5,8, 13],
             }
 
             # Instantiate model
             rci = ClairvoyanceRecursive(
                 n_jobs=-1, 
                 scorer="accuracy", 
                 n_draws=10, 
                 estimator=estimator, 
                 param_grid=param_grid, 
-                percentiles=[0.0, 0.25, 0.5, 0.75, 0.9, 0.925, 0.95, 0.975, 0.99],
-                minimum_scores=[-np.inf, 0.382],
+                percentiles=[0.0, 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 0.925, 0.95, 0.975, 0.99],
+                minimum_scores=[-np.inf, 0.382, 0.5],
                 verbose=0,
             )
             rci.fit(X_normalized, y)
             print(rci.results_.head(), file=sys.stdout)
-
-            # 4.
-            print(format_header("4. Running test for `ClairvoyanceRecursive` on iris dataset with noise [includes testing data]"), file=sys.stderr)
-
-            X_training, X_testing, y_training, y_testing = train_test_split(X_normalized, y, random_state=0, test_size=0.1618)
-
-            # Instantiate model
-            rci = ClairvoyanceRecursive(
-                n_jobs=-1, 
-                scorer="accuracy", 
-                n_draws=10, 
-                estimator=estimator, 
-                param_grid=param_grid, 
-                percentiles=[0.0, 0.25, 0.5, 0.75, 0.9, 0.925, 0.95, 0.975, 0.99],
-                minimum_scores=[-np.inf, 0.382],
-                verbose=0,
-            )
-            rci.fit(X=X_training, y=y_training, X_testing=X_testing, y_testing=y_testing)
-            print(rci.results_.head(), file=sys.stdout)
         else:
-            print("Unrecognized command.  Available commands {--test|-t}", file=sys.stderr)
+            print("Unrecognized command.  Available commands {test}", file=sys.stderr)
 if __name__ == "__main__":
     main()
```

### Comparing `clairvoyance_feature_selection-2023.6.26/setup.py` & `clairvoyance_feature_selection-2023.6.9/setup.py`

 * *Files identical despite different names*


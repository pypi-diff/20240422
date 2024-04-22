# Comparing `tmp/te2rules-0.8.1.tar.gz` & `tmp/te2rules-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/rlal/TE2Rules/dist/tmpatw9ep7u/te2rules-0.8.1.tar", last modified: Wed Mar 27 04:59:14 2024, max compression
+gzip compressed data, was "/Users/rlal/TE2Rules/dist/tmpe76zc22o/te2rules-1.0.0.tar", last modified: Mon Apr 22 08:37:01 2024, max compression
```

## Comparing `te2rules-0.8.1.tar` & `te2rules-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-03-27 04:59:14.642790 te2rules-0.8.1/
--rw-r--r--   0 root         (0) staff       (20)    19404 2022-10-25 22:55:59.000000 te2rules-0.8.1/LICENSE
--rw-r--r--   0 root         (0) staff       (20)     6655 2024-03-27 04:59:14.643055 te2rules-0.8.1/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     5880 2024-01-04 01:01:56.000000 te2rules-0.8.1/README.md
--rw-r--r--   0 root         (0) staff       (20)      126 2022-10-23 05:45:05.000000 te2rules-0.8.1/pyproject.toml
--rw-r--r--   0 root         (0) staff       (20)     1245 2024-03-27 04:59:14.643813 te2rules-0.8.1/setup.cfg
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-03-27 04:59:14.640528 te2rules-0.8.1/te2rules/
--rw-r--r--   0 root         (0) staff       (20)       91 2024-03-27 04:38:15.000000 te2rules-0.8.1/te2rules/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     8287 2022-10-23 05:45:05.000000 te2rules-0.8.1/te2rules/adapter.py
--rw-r--r--   0 root         (0) staff       (20)    42903 2024-03-27 04:52:59.000000 te2rules-0.8.1/te2rules/explainer.py
--rw-r--r--   0 root         (0) staff       (20)     9181 2022-10-23 05:45:05.000000 te2rules-0.8.1/te2rules/rule.py
--rw-r--r--   0 root         (0) staff       (20)    16978 2022-10-23 05:45:05.000000 te2rules-0.8.1/te2rules/tree.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-03-27 04:59:14.642489 te2rules-0.8.1/te2rules.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     6655 2024-03-27 04:59:14.000000 te2rules-0.8.1/te2rules.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      298 2024-03-27 04:59:14.000000 te2rules-0.8.1/te2rules.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-03-27 04:59:14.000000 te2rules-0.8.1/te2rules.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       88 2024-03-27 04:59:14.000000 te2rules-0.8.1/te2rules.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        9 2024-03-27 04:59:14.000000 te2rules-0.8.1/te2rules.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-22 08:37:01.581188 te2rules-1.0.0/
+-rw-r--r--   0 root         (0) staff       (20)    19404 2022-10-25 22:55:59.000000 te2rules-1.0.0/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)    10216 2024-04-22 08:37:01.581477 te2rules-1.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     9441 2024-04-22 08:24:40.000000 te2rules-1.0.0/README.md
+-rw-r--r--   0 root         (0) staff       (20)      126 2022-10-23 05:45:05.000000 te2rules-1.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) staff       (20)     1245 2024-04-22 08:37:01.582288 te2rules-1.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-22 08:37:01.578690 te2rules-1.0.0/te2rules/
+-rw-r--r--   0 root         (0) staff       (20)       91 2024-04-22 08:27:00.000000 te2rules-1.0.0/te2rules/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    10698 2024-04-22 07:51:49.000000 te2rules-1.0.0/te2rules/adapter.py
+-rw-r--r--   0 root         (0) staff       (20)    43047 2024-04-22 07:57:45.000000 te2rules-1.0.0/te2rules/explainer.py
+-rw-r--r--   0 root         (0) staff       (20)     9182 2024-04-21 05:48:05.000000 te2rules-1.0.0/te2rules/rule.py
+-rw-r--r--   0 root         (0) staff       (20)    17859 2024-04-21 05:48:10.000000 te2rules-1.0.0/te2rules/tree.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-22 08:37:01.580855 te2rules-1.0.0/te2rules.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)    10216 2024-04-22 08:37:01.000000 te2rules-1.0.0/te2rules.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      298 2024-04-22 08:37:01.000000 te2rules-1.0.0/te2rules.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-04-22 08:37:01.000000 te2rules-1.0.0/te2rules.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       88 2024-04-22 08:37:01.000000 te2rules-1.0.0/te2rules.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        9 2024-04-22 08:37:01.000000 te2rules-1.0.0/te2rules.egg-info/top_level.txt
```

### Comparing `te2rules-0.8.1/LICENSE` & `te2rules-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `te2rules-0.8.1/PKG-INFO` & `te2rules-1.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: te2rules
-Version: 0.8.1
+Version: 1.0.0
 Summary: Python Library to explain tree ensembles using rules
 Home-page: https://github.com/linkedin/TE2Rules
 Author: G Roshan Lal
 Author-email: groshanlal@gmail.com
 License: Creative Commons Attribution-NonCommercial 4.0 International Public License
 Project-URL: Bug Tracker, https://github.com/linkedin/TE2Rules/issues
 Project-URL: Source Code, https://github.com/linkedin/TE2Rules
@@ -60,14 +60,39 @@
 The tree ensemble model used in this notebook is a XGBoost model with 10 trees.
 ![TE2Rules Adult Screenshot3](https://raw.githubusercontent.com/linkedin/TE2Rules/main/docs/images/3-train.png)
 
 Let us use TE2Rules ```ModelExplainer``` to explain the positive class prediciton by the XGBoost model. We observe that TE2Rules extracts 5 rules to explain more than 99% of the positive class prediction by the tree ensemble model. In this usgae, we use the default values of ```min_precision``` (0.95) and  ```num_stages``` (10), since the algorithm runs quickly for a tree ensemble with 10 trees.
 ![TE2Rules Adult Screenshot4](https://raw.githubusercontent.com/linkedin/TE2Rules/main/docs/images/4-explain.png)
 ![TE2Rules Adult Screenshot5](https://raw.githubusercontent.com/linkedin/TE2Rules/main/docs/images/5-evaluate.png)
 
+These are not the only possible way to explain the model prediction. TE2Rules generates all possible explanations that can be extracted out of the tree ensemble model and then selects a short subset of rules out of all the possible rules such that the selected subset is small while explaining most of the positive class prediction by the model.
+
+However, we need not settle with the subset of rules selected by TE2Rules. To see all the possible explanations, we can use ```longer_rules``` as shown below. From this set of rules, a domain expert can go through them and select their own small subset of rules that explains most of the positive model predictions and also aligns with the decision-making process often used in that domain. This way TE2Rules offers the flexibility to choose the explanations that most closely aligns with the human decision making process.
+![TE2Rules Adult Screenshot6a](https://raw.githubusercontent.com/linkedin/TE2Rules/main/docs/images/all-explanations-6a.png)
+![TE2Rules Adult Screenshot6b](https://raw.githubusercontent.com/linkedin/TE2Rules/main/docs/images/all-explanations-6b.png)
+
+
+The longer set of all possible explanations would have significant overlap among the rules. For a given input to the model, multiple rules satisfying the input can be used to explain the input. The ```explain_instance_with_rules``` method provides one way to show all the possible rules that can explain each input instance. Again, a domain expert can pick the rule that is most suitable to explain that instance.
+![TE2Rules Adult Screenshot7](https://raw.githubusercontent.com/linkedin/TE2Rules/main/docs/images/local-7.png)
+![TE2Rules Adult Screenshot8a](https://raw.githubusercontent.com/linkedin/TE2Rules/main/docs/images/local-8a.png)
+![TE2Rules Adult Screenshot8b](https://raw.githubusercontent.com/linkedin/TE2Rules/main/docs/images/local-8b.png)
+![TE2Rules Adult Screenshot8c](https://raw.githubusercontent.com/linkedin/TE2Rules/main/docs/images/local-8c.png)
+![TE2Rules Adult Screenshot8d](https://raw.githubusercontent.com/linkedin/TE2Rules/main/docs/images/local-8d.png)
+
+## Some popular applications of TE2Rules
+
+Here is a list of some applications of TE2Rules in high-stake domains like healthcare, where understanding why a ML model made a particular decision is critical in developing trust on the system.
+
+ - An Explainable Artificial Intelligence model in the assessment of Brain MRI Lesions in Multiple Sclerosis using Amplitude Modulation – Frequency Modulation multi-scale feature sets, Andria Nicolaou, Antonis Kakas et al, 2023 24th International Conference on Digital Signal Processing (DSP), https://ieeexplore.ieee.org/abstract/document/10167888
+ - Emergency Department Triage Hospitalization Prediction Based on Machine Learning and Rule Extraction, Waqar A. Sulaiman, Andria Nicolaou et al, 2023 IEEE EMBS Special Topic Conference on Data Science and Engineering in Healthcare, Medicine and Biology, https://ieeexplore.ieee.org/abstract/document/10405176
+ - An Explainable AI model in the assessment of Multiple Sclerosis using clinical data and Brain MRI lesion texture features, A. Nicolaou, M. Pantzaris et al, 2023 IEEE EMBS International Conference on Biomedical and Health Informatics (BHI), https://ieeexplore.ieee.org/abstract/document/10313379
+ - A Comparative Study of Explainable AI models in the Assessment of Multiple Sclerosis, Andria Nicolaou, Nicoletta Prentzas et al, 2023 Computer Analysis of Images and Patterns
+(CAIP 2023), https://link.springer.com/chapter/10.1007/978-3-031-44240-7_14
+
+
 ## For reproducing results in the paper
 
 Run the follwing python scripts to generate the results in the [paper](https://arxiv.org/abs/2206.14359):
 
 ```bash
 python3 demo/demo/run_te2rules.py
 python3 demo/demo/run_defrag.py
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `te2rules-0.8.1/setup.cfg` & `te2rules-1.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `te2rules-0.8.1/te2rules/adapter.py` & `te2rules-1.0.0/te2rules/adapter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """
-This file contains adapters to convert scikit learn tree ensemble models
+This file contains adapters to convert scikit learn and xgboost tree ensemble models
 into corresponding te2rules tree ensemble models. The tree ensemble models
 of te2rules have the necessary structure for explaining itself using rules.
 """
 from __future__ import annotations
 
-from typing import List
+import json
+from typing import Any, Dict, List
 
 import numpy as np
 from sklearn.ensemble import GradientBoostingClassifier, RandomForestClassifier
 from sklearn.tree import DecisionTreeClassifier, DecisionTreeRegressor, _tree
+from xgboost import XGBClassifier
 
 from te2rules.tree import DecisionTree, LeafNode, RandomForest, TreeNode
 
 
 class ScikitGradientBoostingClassifierAdapter:
     """
     Class to convert sklearn.ensemble.GradientBoostingClassifier
@@ -225,7 +227,73 @@
                 left_node = nodes[self.children_left[i]]
                 nodes[i].left = left_node
                 right_node = nodes[self.children_right[i]]
                 nodes[i].right = right_node
 
         root_node = nodes[0]
         return root_node
+
+
+class XgboostXGBClassifierAdapter:
+    """
+    Class to convert xgboost.sklearn.XGBClassifier
+    into a te2rules.tree.RandomForest object.
+
+    Usage:
+    adapter = XgboostXGBClassifierAdapter(model, feature_names)
+    adapted_model = adapter.random_forest
+    """
+
+    def __init__(self, xgb_model: XGBClassifier, feature_names: List[str]):
+        self.xgb_model_json = xgb_model.get_booster().get_dump(dump_format="json")
+        self.feature_names = feature_names
+
+        self.bias = 0.0
+        self.weight = 1.0
+        self.activation = "sigmoid"
+
+        self.random_forest = self._convert()
+
+    def _build_tree(self, tree_dict: Dict[str, Any]) -> DecisionTree:
+        """
+        Private method to perform a DFS traversal of the model json
+        and build the te2rules.tree.DecisionTree object.
+        """
+        if "leaf" in tree_dict:
+            node = DecisionTree(LeafNode(value=float(tree_dict["leaf"])))
+        else:
+            # Get feature index. Ex: feature-21 would be
+            # represented as f21. Get index 21 from f21.
+            i = int(tree_dict["split"][1:])
+
+            # XGBoost and Scikit Learn treat splits differently.
+            # Scikit Learn uses left node for f1 <= threshold while
+            # XGBoost uses left node for f1 < threshold
+            node = DecisionTree(
+                TreeNode(
+                    node_name=self.feature_names[i],
+                    threshold=float(tree_dict["split_condition"]),
+                    equality_on_left=False,
+                )
+            )
+            node.left = self._build_tree(tree_dict["children"][0])
+            node.right = self._build_tree(tree_dict["children"][1])
+        return node
+
+    def _convert(self) -> RandomForest:
+        """
+        Private method to create the te2rules.tree.RandomForest
+        from the xgboost.sklearn.XGBClassifier object.
+        """
+        self.tree_ensemble = []
+        for i in range(len(self.xgb_model_json)):
+            tree_dict = json.loads(self.xgb_model_json[i])
+            node = self._build_tree(tree_dict)
+            self.tree_ensemble.append(node)
+
+        return RandomForest(
+            list(self.tree_ensemble),
+            weight=self.weight,
+            bias=self.bias,
+            feature_names=self.feature_names,
+            activation=self.activation,
+        )
```

### Comparing `te2rules-0.8.1/te2rules/explainer.py` & `te2rules-1.0.0/te2rules/explainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 """
 This file contains ModelExplainer and RuleBuilder classes that explain a tree ensemble
 model by extracting rules to explain the positive class. This file contains the
 implementation of TE2Rules Algorithm described in the paper:
 "TE2Rules: Explaining Tree Ensembles using Rules"
 (https://arxiv.org/abs/2206.14359/).
 """
+
 from __future__ import annotations
 
 import logging
 import re
-from typing import Dict, List, Set, Tuple
+from typing import Dict, List, Optional, Set, Tuple
 
 import pandas as pd
 import sklearn
 from sklearn.ensemble import GradientBoostingClassifier, RandomForestClassifier
 from tqdm import tqdm
+from xgboost import XGBClassifier
 
 from te2rules.adapter import (
     ScikitGradientBoostingClassifierAdapter,
     ScikitRandomForestClassifierAdapter,
+    XgboostXGBClassifierAdapter,
 )
 from te2rules.rule import Rule
 from te2rules.tree import RandomForest
 
 log = logging.getLogger()
 
 
@@ -34,26 +37,30 @@
     used by TE2Rules is based on Apriori Rule Mining.
     For more details on the algorithm, please check out our paper
     `TE2Rules: Explaining Tree Ensembles using Rules
     <https://arxiv.org/abs/2206.14359/>`_.
     """
 
     def __init__(
-        self, model: sklearn.ensemble, feature_names: List[str], verbose: bool = False
+        self,
+        model: sklearn.ensemble | XGBClassifier,
+        feature_names: List[str],
+        verbose: bool = False,
     ):
         """
         Initialize the explainer with the trained tree ensemble model
         and feature names used by the model.
 
         Returns a ModelExplainer object
 
         Parameters
         ----------
         model: sklearn.ensemble.GradientBoostingClassifier or \
-            sklearn.ensemble.RandomForestClassifier
+            sklearn.ensemble.RandomForestClassifier or \
+            xgboost.XGBClassifier
             The trained Tree Ensemble model to be explained.
             The model is expected to be a binary classifier.
         feature_name: List[str]
             List of feature names used by the `model`. Only alphanumeric characters and
             underscores are allowed in feature names.
         verbose: bool, optional
             Optional boolean value to give more insights on the running of the
@@ -65,26 +72,21 @@
         self: te2rules.explainer.ModelExplainer
             A ModelExplainer object initialized with the model to be explained.
 
         Raises
         ------
         ValueError:
             when `model` is not a supported Tree Ensemble Model.
-            Currently, only Scikit Learn's GradientBoostingClassifier and
-            RandomForestClassifier are supported.
+            Currently, only scikit-learn's GradientBoostingClassifier,
+            RandomForestClassifier and xgboost's XGBClassifier are supported.
 
         ValueError:
             when `feature_name` list contains a name that has any character other
             than alphanumeric characters or underscore.
 
-        Warning
-        ------
-        The implementation works fine with scikit learn's GradientBoostingClassifier.
-        For now, we are still testing the case when the `model` is scikit learn's
-        RandomForestClassifier.
         """
         self.feature_names = feature_names
         for f in feature_names:
             if re.search("[^a-zA-Z0-9_]", f):
                 raise ValueError(
                     "Only alphanumeric characters and underscores are allowed "
                     + "in feature names. But found feature name: "
@@ -100,26 +102,31 @@
             self.random_forest = ScikitGradientBoostingClassifierAdapter(
                 model, feature_names
             ).random_forest
         elif isinstance(model, RandomForestClassifier):
             self.random_forest = ScikitRandomForestClassifierAdapter(
                 model, feature_names
             ).random_forest
+        elif isinstance(model, XGBClassifier):
+            self.random_forest = XgboostXGBClassifierAdapter(
+                model, feature_names
+            ).random_forest
         else:
             raise ValueError(
-                "Only GradientBoostingClassifier and RandomForestClassifier "
+                "Only GradientBoostingClassifier, RandomForestClassifier "
+                + "and XGBClassifier "
                 + "are supported. But received "
                 + str(type(model))
             )
 
     def explain(
         self,
         X: List[List[float]],
         y: List[int],
-        num_stages: int = None,
+        num_stages: Optional[int] = None,
         min_precision: float = 0.95,
         jaccard_threshold: float = 0.20,
     ) -> List[str]:
         """
         A method to extract rule list from the tree ensemble model.
         This method takes in input features used by the model and predicted class
         output by the model.
@@ -332,15 +339,15 @@
             raise AttributeError(
                 "rules to explain the tree ensemble are not set. "
                 + "Call explain() before calling apply()"
             )
         return y_rules
 
     def get_fidelity(
-        self, X: List[List[float]] = None, y: List[int] = None
+        self, X: Optional[List[List[float]]] = None, y: Optional[List[int]] = None
     ) -> Tuple[float, float, float]:
         """
         A method to evaluate the rule list extracted by the `explain` method
 
         Returns a fidelity on positives, negative, overall
 
         Parameters
@@ -465,15 +472,15 @@
     explains the tree ensemble using rules for the postive class
     prediction.
     """
 
     def __init__(
         self,
         random_forest: RandomForest,
-        num_stages: int = None,
+        num_stages: Optional[int] = None,
         min_precision: float = 0.95,
         jaccard_threshold: float = 0.20,
     ):
         self.random_forest = random_forest
         # if num_stages not set by user, will set it to the number of trees
         # note that we neednum_stages <= num_trees
         if num_stages is not None:
@@ -677,15 +684,15 @@
                     )
                     if is_solution is True:
                         new_solutions.append(r)
                     if keep_candidate is True:
                         new_candidates.append(r)
             else:
                 join_indices = self._get_join_indices(self.candidate_rules)
-                for (i, j) in tqdm(join_indices):
+                for i, j in tqdm(join_indices):
                     joined_rule = self.candidate_rules[i].join(self.candidate_rules[j])
                     if joined_rule is not None:
                         is_solution, keep_candidate = self._filter_candidates(
                             joined_rule, self.labels
                         )
                         if is_solution is True:
                             new_solutions.append(joined_rule)
@@ -815,15 +822,15 @@
                 keep_candidate = False
                 return is_solution, keep_candidate
             else:
                 # keep candidate: it can become a solution
                 keep_candidate = True
                 return is_solution, keep_candidate
 
-    def get_fidelity(self, use_top: int = None) -> Tuple[float, float, float]:
+    def get_fidelity(self, use_top: Optional[int] = None) -> Tuple[float, float, float]:
         """
         A method to compute fidelity of the rule list.
         Fidelity is defined as the fraction of data on which the
         explanation (rule list) agrees with the tree ensemble.
         This method returns the fidelity on the overall data,
         data with positive class predictions and negative class
         predictions, respectively by the tree ensemble model.
@@ -907,15 +914,15 @@
                         pred_dict[(f, op_type)] = (op, val)
                     elif (op_type == "less than" and val < old_val) or (
                         op_type == "greater than" and val > old_val
                     ):
                         pred_dict[(f, op_type)] = (op, val)
             # make shorter rule from predicate list
             final_rule = []
-            for (f, _) in pred_dict:
+            for f, _ in pred_dict:
                 op, val = pred_dict[(f, _)]
                 final_rule.append((" ").join([f, op, val]))
             rules[i].decision_rule = final_rule
         return rules
 
     def apply(self, df: pd.DataFrame) -> List[int]:
         """
@@ -1028,19 +1035,16 @@
                         if len(pos_support_intersection_jk) > 0:
                             if (jaccard_similarity_score > 0) and (
                                 jaccard_similarity_score <= self.jaccard_threshold
                             ):
                                 pairs.add((j, k))
                                 count_valid = count_valid + 1
 
-        if count_all > 0:
-            log.info(
-                "Using only " + str(int(count_valid / count_all * 100)) + "% pairs"
-            )
-            log.info("Using only " + str(int(len(pairs) / count_all * 100)) + "% pairs")
+        log.info("Using only " + str(int(count_valid / count_all * 100)) + "% pairs")
+        log.info("Using only " + str(int(len(pairs) / count_all * 100)) + "% pairs")
 
         pairs_list = list(pairs)
         # pairs_list.sort()  # can be removed
         return pairs_list
 
     def _prune(self, rules: List[Rule], positives: List[int]) -> List[Rule]:
         """
```

### Comparing `te2rules-0.8.1/te2rules/rule.py` & `te2rules-1.0.0/te2rules/rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 This file defines the rule object used in explaining te2rules tree ensemble models.
 """
+
 from __future__ import annotations
 
 from typing import Dict, List, Optional
 
 
 class Rule:
     """
```

### Comparing `te2rules-0.8.1/te2rules/tree.py` & `te2rules-1.0.0/te2rules/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 This file contains the tree and tree ensemble objects in te2rules.
 The tree ensemble models of te2rules have the necessary structure for
 explaining itself using rules.
 """
+
 from __future__ import annotations
 
 from typing import Dict, List, Optional
 
 from te2rules.rule import Rule
 
 
@@ -22,31 +23,43 @@
 
 class TreeNode(Node):
     """
     Class of internal (non-leaf) nodes in decision trees.
     Each internal node has a feature name and threshold value
     on which the split is performed.
 
-    The left split is taken when feature value <= threshold value
-    and the right split is taken when feature value > threshold value.
+    By default, equality_on_left = True, the left split is taken
+    when feature value <= threshold value and the right split is
+    taken when feature value > threshold value.
+
+    When equality_on_left = False, the left split is taken
+    when feature value < threshold value and the right split is
+    taken when feature value >= threshold value.
     """
 
-    def __init__(self, node_name: str, threshold: float):
+    def __init__(self, node_name: str, threshold: float, equality_on_left: bool = True):
         super().__init__(is_leaf=False)
         self.node_name = node_name
         self.threshold = threshold
+        self.equality_on_left = equality_on_left
 
     def __str__(self) -> str:
         return self.node_name
 
     def get_left_clause(self) -> str:
-        return self.node_name + " <= " + str(self.threshold)
+        if self.equality_on_left is True:
+            return self.node_name + " <= " + str(self.threshold)
+        else:
+            return self.node_name + " < " + str(self.threshold)
 
     def get_right_clause(self) -> str:
-        return self.node_name + " > " + str(self.threshold)
+        if self.equality_on_left is True:
+            return self.node_name + " > " + str(self.threshold)
+        else:
+            return self.node_name + " >= " + str(self.threshold)
 
 
 class LeafNode(Node):
     """
     Class of terminal (leaf) nodes in decision trees.
     Each leaf node has a value assigned to data reaching the leaf.
     """
@@ -188,18 +201,24 @@
             if (self.left is None) or (self.right is None):
                 raise ValueError("TreeNode cannot have None as children")
             else:
                 feature_index = feature_names.index(self.node.node_name)
                 left_decision_support = []
                 right_decision_support = []
                 for index in self.decision_support:
-                    if data[index][feature_index] <= self.node.threshold:
-                        left_decision_support.append(index)
+                    if self.node.equality_on_left is True:
+                        if data[index][feature_index] <= self.node.threshold:
+                            left_decision_support.append(index)
+                        else:
+                            right_decision_support.append(index)
                     else:
-                        right_decision_support.append(index)
+                        if data[index][feature_index] < self.node.threshold:
+                            left_decision_support.append(index)
+                        else:
+                            right_decision_support.append(index)
                 self.left._propagate_decision_support(
                     data, feature_names, left_decision_support
                 )
                 self.right._propagate_decision_support(
                     data, feature_names, right_decision_support
                 )
         else:
```

### Comparing `te2rules-0.8.1/te2rules.egg-info/PKG-INFO` & `te2rules-1.0.0/te2rules.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: te2rules
-Version: 0.8.1
+Version: 1.0.0
 Summary: Python Library to explain tree ensembles using rules
 Home-page: https://github.com/linkedin/TE2Rules
 Author: G Roshan Lal
 Author-email: groshanlal@gmail.com
 License: Creative Commons Attribution-NonCommercial 4.0 International Public License
 Project-URL: Bug Tracker, https://github.com/linkedin/TE2Rules/issues
 Project-URL: Source Code, https://github.com/linkedin/TE2Rules
@@ -60,14 +60,39 @@
 The tree ensemble model used in this notebook is a XGBoost model with 10 trees.
 ![TE2Rules Adult Screenshot3](https://raw.githubusercontent.com/linkedin/TE2Rules/main/docs/images/3-train.png)
 
 Let us use TE2Rules ```ModelExplainer``` to explain the positive class prediciton by the XGBoost model. We observe that TE2Rules extracts 5 rules to explain more than 99% of the positive class prediction by the tree ensemble model. In this usgae, we use the default values of ```min_precision``` (0.95) and  ```num_stages``` (10), since the algorithm runs quickly for a tree ensemble with 10 trees.
 ![TE2Rules Adult Screenshot4](https://raw.githubusercontent.com/linkedin/TE2Rules/main/docs/images/4-explain.png)
 ![TE2Rules Adult Screenshot5](https://raw.githubusercontent.com/linkedin/TE2Rules/main/docs/images/5-evaluate.png)
 
+These are not the only possible way to explain the model prediction. TE2Rules generates all possible explanations that can be extracted out of the tree ensemble model and then selects a short subset of rules out of all the possible rules such that the selected subset is small while explaining most of the positive class prediction by the model.
+
+However, we need not settle with the subset of rules selected by TE2Rules. To see all the possible explanations, we can use ```longer_rules``` as shown below. From this set of rules, a domain expert can go through them and select their own small subset of rules that explains most of the positive model predictions and also aligns with the decision-making process often used in that domain. This way TE2Rules offers the flexibility to choose the explanations that most closely aligns with the human decision making process.
+![TE2Rules Adult Screenshot6a](https://raw.githubusercontent.com/linkedin/TE2Rules/main/docs/images/all-explanations-6a.png)
+![TE2Rules Adult Screenshot6b](https://raw.githubusercontent.com/linkedin/TE2Rules/main/docs/images/all-explanations-6b.png)
+
+
+The longer set of all possible explanations would have significant overlap among the rules. For a given input to the model, multiple rules satisfying the input can be used to explain the input. The ```explain_instance_with_rules``` method provides one way to show all the possible rules that can explain each input instance. Again, a domain expert can pick the rule that is most suitable to explain that instance.
+![TE2Rules Adult Screenshot7](https://raw.githubusercontent.com/linkedin/TE2Rules/main/docs/images/local-7.png)
+![TE2Rules Adult Screenshot8a](https://raw.githubusercontent.com/linkedin/TE2Rules/main/docs/images/local-8a.png)
+![TE2Rules Adult Screenshot8b](https://raw.githubusercontent.com/linkedin/TE2Rules/main/docs/images/local-8b.png)
+![TE2Rules Adult Screenshot8c](https://raw.githubusercontent.com/linkedin/TE2Rules/main/docs/images/local-8c.png)
+![TE2Rules Adult Screenshot8d](https://raw.githubusercontent.com/linkedin/TE2Rules/main/docs/images/local-8d.png)
+
+## Some popular applications of TE2Rules
+
+Here is a list of some applications of TE2Rules in high-stake domains like healthcare, where understanding why a ML model made a particular decision is critical in developing trust on the system.
+
+ - An Explainable Artificial Intelligence model in the assessment of Brain MRI Lesions in Multiple Sclerosis using Amplitude Modulation – Frequency Modulation multi-scale feature sets, Andria Nicolaou, Antonis Kakas et al, 2023 24th International Conference on Digital Signal Processing (DSP), https://ieeexplore.ieee.org/abstract/document/10167888
+ - Emergency Department Triage Hospitalization Prediction Based on Machine Learning and Rule Extraction, Waqar A. Sulaiman, Andria Nicolaou et al, 2023 IEEE EMBS Special Topic Conference on Data Science and Engineering in Healthcare, Medicine and Biology, https://ieeexplore.ieee.org/abstract/document/10405176
+ - An Explainable AI model in the assessment of Multiple Sclerosis using clinical data and Brain MRI lesion texture features, A. Nicolaou, M. Pantzaris et al, 2023 IEEE EMBS International Conference on Biomedical and Health Informatics (BHI), https://ieeexplore.ieee.org/abstract/document/10313379
+ - A Comparative Study of Explainable AI models in the Assessment of Multiple Sclerosis, Andria Nicolaou, Nicoletta Prentzas et al, 2023 Computer Analysis of Images and Patterns
+(CAIP 2023), https://link.springer.com/chapter/10.1007/978-3-031-44240-7_14
+
+
 ## For reproducing results in the paper
 
 Run the follwing python scripts to generate the results in the [paper](https://arxiv.org/abs/2206.14359):
 
 ```bash
 python3 demo/demo/run_te2rules.py
 python3 demo/demo/run_defrag.py
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```


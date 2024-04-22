# Comparing `tmp/synrbl-0.0.7.tar.gz` & `tmp/synrbl-0.0.8.tar.gz`

## Comparing `synrbl-0.0.7.tar` & `synrbl-0.0.8.tar`

### file list

```diff
@@ -1,152 +1,154 @@
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 synrbl-0.0.7/.coveragerc
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 synrbl-0.0.7/.gitattributes
--rwxr-xr-x   0        0        0      216 2020-02-02 00:00:00.000000 synrbl-0.0.7/lint.sh
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 synrbl-0.0.7/requirements.txt
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 synrbl-0.0.7/.github/workflows/publish-package.yml
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 synrbl-0.0.7/.github/workflows/test-and-lint.yml
--rw-r--r--   0        0        0   815176 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Raw_data/Golden/Golden.csv
--rw-r--r--   0        0        0    44593 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Raw_data/Jaworski/complex.csv
--rw-r--r--   0        0        0   128945 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Raw_data/Jaworski/patent.csv
--rw-r--r--   0        0        0    91588 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Raw_data/Jaworski/typical.csv
--rw-r--r--   0        0        0  5788436 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Raw_data/USPTO/USPTO_50K.csv
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Rules/automated_rules.json.gz
--rw-r--r--   0        0        0    63599 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Validation_set/Jaworski.csv
--rw-r--r--   0        0        0  5788436 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Validation_set/USPTO_50K.csv
--rw-r--r--   0        0        0   188656 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Validation_set/USPTO_diff.csv
--rw-r--r--   0        0        0    89839 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Validation_set/USPTO_random_class.csv
--rw-r--r--   0        0        0    64959 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Validation_set/USPTO_unbalance_class.csv
--rw-r--r--   0        0        0   677196 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Validation_set/golden_dataset.csv
--rw-r--r--   0        0        0  1955873 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Validation_set/validation_set.csv
--rw-r--r--   0        0        0  2769281 2020-02-02 00:00:00.000000 synrbl-0.0.7/Data/Validation_set/validation_set.json
--rw-r--r--   0        0        0    22209 2020-02-02 00:00:00.000000 synrbl-0.0.7/Docs/Examples/notebook.ipynb
--rw-r--r--   0        0        0    86666 2020-02-02 00:00:00.000000 synrbl-0.0.7/Docs/Images/Flowchart.png
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 synrbl-0.0.7/Docs/Paper_fig/figures.py
--rw-r--r--   0        0        0    55850 2020-02-02 00:00:00.000000 synrbl-0.0.7/Pipeline/Validation/Analysis/Analysis_vis.ipynb
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 synrbl-0.0.7/Pipeline/Validation/Analysis/SynRBL - Jaworski.csv
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 synrbl-0.0.7/Pipeline/Validation/Analysis/SynRBL - USPTO_diff.csv
--rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 synrbl-0.0.7/Pipeline/Validation/Analysis/SynRBL - USPTO_random_class.csv
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 synrbl-0.0.7/Pipeline/Validation/Analysis/SynRBL - USPTO_unbalance_class.csv
--rw-r--r--   0        0        0    13301 2020-02-02 00:00:00.000000 synrbl-0.0.7/Pipeline/Validation/Analysis/SynRBL - golden_dataset.csv
--rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 synrbl-0.0.7/Scripts/result_evaluation.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 synrbl-0.0.7/Scripts/synrbl_pilot.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 synrbl-0.0.7/Scripts/validation_set_interface.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/__init__.py
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/test_mcs_search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynChemImputer/__init__.py
--rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynChemImputer/test_appeal_reaction.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynChemImputer/test_molecule_standardizer.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynChemImputer/test_peroxide_imputer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/__init__.py
--rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/test_merge.py
--rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/test_model.py
--rw-r--r--   0        0        0    11025 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/test_rules.py
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/test_structure.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/MissingGraph/__init__.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/MissingGraph/test_find_graph_dict.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/MissingGraph/test_find_missing_graphs.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/MissingGraph/test_molcurator.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/MissingGraph/test_uncertainty_graph.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/SubStructure/__init__.py
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/SubStructure/test_extract_common_mcs.py
--rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/SubStructure/test_mcs_graph_detector.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/SubStructure/test_mcs_process.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynMCSImputer/SubStructure/test_substructure_analyzer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynProcessor/__init__.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynProcessor/test_check_carbon_balance.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynProcessor/test_rmsi_comparator.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynProcessor/test_rmsi_decomposer.py
--rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynProcessor/test_rmsi_processing.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynProcessor/test_rsmi_both_side_process.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynRuleImputer/__init__.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynRuleImputer/test_auto_extract_rules.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynRuleImputer/test_auto_extract_smiles.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynRuleImputer/test_rule_constraint.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynRuleImputer/test_rule_data_manager.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynRuleImputer/test_synthetic_rule_imputer.py
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynRuleImputer/test_synthetic_rule_matcher.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynUtils/__init__.py
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynUtils/test_chem_utils.py
--rw-r--r--   0        0        0     8918 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynUtils/test_functional_group_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynVis/__init__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 synrbl-0.0.7/Test/SynVis/test_reaction_visualizer.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/__main__.py
--rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/balancing.py
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/confidence_prediction.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/mcs_search.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/postprocess.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/preprocess.py
--rw-r--r--   0        0        0    14738 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/rsmi_utils.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/rule_based.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynAnalysis/__init__.py
--rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynAnalysis/analysis_process.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynAnalysis/analysis_utils.py
--rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynAnalysis/eda_analysis.py
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynAnalysis/feature_analysis.py
--rw-r--r--   0        0        0   278926 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynAnalysis/scoring_function.dump
--rw-r--r--   0        0        0    16405 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynAnalysis/visualizer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynChemImputer/__init__.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynChemImputer/appel_reaction.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynChemImputer/compounds_template.json
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynChemImputer/curate_reduction.py
--rw-r--r--   0        0        0     7786 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynChemImputer/functional_group_checker.py
--rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynChemImputer/molecule_standardizer.py
--rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynChemImputer/peroxide_imputer.py
--rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynChemImputer/reduction_template.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynChemImputer/reduction_templates.json
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynCmd/__init__.py
--rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynCmd/cmd_benchmark.py
--rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynCmd/cmd_run.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynCmd/logging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/__init__.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/compound_rules.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/expand_rules.json
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/merge.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/merge_rules.json
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/merge_rules_example.json
--rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/model.py
--rw-r--r--   0        0        0    29044 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/rules.py
--rw-r--r--   0        0        0     6768 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/structure.py
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/MissingGraph/__init__.py
--rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/MissingGraph/find_graph_dict.py
--rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/MissingGraph/find_missing_graphs.py
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/MissingGraph/molcurator.py
--rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/MissingGraph/refinement_uncertainty.py
--rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/MissingGraph/uncertainty_graph.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/SubStructure/__init__.py
--rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/SubStructure/extract_common_mcs.py
--rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/SubStructure/mcs_graph_detector.py
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/SubStructure/mcs_process.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynMCSImputer/SubStructure/substructure_analyzer.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynProcessor/__init__.py
--rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynProcessor/check_carbon_balance.py
--rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynProcessor/rsmi_both_side_process.py
--rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynProcessor/rsmi_comparator.py
--rw-r--r--   0        0        0     7320 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynProcessor/rsmi_decomposer.py
--rw-r--r--   0        0        0     7210 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynProcessor/rsmi_processing.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynRuleImputer/__init__.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynRuleImputer/auto_extract_rules.py
--rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynRuleImputer/auto_extract_smiles.py
--rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynRuleImputer/rule_data_manager.py
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynRuleImputer/rules_manager.json.gz
--rw-r--r--   0        0        0     9182 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynRuleImputer/synthetic_rule_constraint.py
--rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynRuleImputer/synthetic_rule_imputer.py
--rw-r--r--   0        0        0     8858 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynRuleImputer/synthetic_rule_matcher.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynUtils/__init__.py
--rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynUtils/chem_utils.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynUtils/common.py
--rw-r--r--   0        0        0    11925 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynUtils/data_utils.py
--rw-r--r--   0        0        0     9444 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynUtils/functional_group_utils.py
--rw-r--r--   0        0        0    14679 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynUtils/rsmi_utils.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynVis/__init__.py
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynVis/mcs_visualizer.py
--rw-r--r--   0        0        0     9300 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynVis/reaction_visualizer.py
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynVis/rxnpdf.py
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 synrbl-0.0.7/synrbl/SynVis/rxnvis.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 synrbl-0.0.7/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 synrbl-0.0.7/LICENSE
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 synrbl-0.0.7/README.md
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 synrbl-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 synrbl-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 synrbl-0.0.8/.coveragerc
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 synrbl-0.0.8/.gitattributes
+-rwxr-xr-x   0        0        0      216 2020-02-02 00:00:00.000000 synrbl-0.0.8/lint.sh
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 synrbl-0.0.8/requirements.txt
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 synrbl-0.0.8/.github/workflows/publish-package.yml
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 synrbl-0.0.8/.github/workflows/test-and-lint.yml
+-rw-r--r--   0        0        0   815176 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Raw_data/Golden/Golden.csv
+-rw-r--r--   0        0        0    44593 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Raw_data/Jaworski/complex.csv
+-rw-r--r--   0        0        0   128945 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Raw_data/Jaworski/patent.csv
+-rw-r--r--   0        0        0    91588 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Raw_data/Jaworski/typical.csv
+-rw-r--r--   0        0        0  5788436 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Raw_data/USPTO/USPTO_50K.csv
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Rules/automated_rules.json.gz
+-rw-r--r--   0        0        0    63599 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Validation_set/Jaworski.csv
+-rw-r--r--   0        0        0  5788436 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Validation_set/USPTO_50K.csv
+-rw-r--r--   0        0        0   188656 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Validation_set/USPTO_diff.csv
+-rw-r--r--   0        0        0    89839 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Validation_set/USPTO_random_class.csv
+-rw-r--r--   0        0        0    64959 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Validation_set/USPTO_unbalance_class.csv
+-rw-r--r--   0        0        0   677196 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Validation_set/golden_dataset.csv
+-rw-r--r--   0        0        0  1955873 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Validation_set/validation_set.csv
+-rw-r--r--   0        0        0  2769281 2020-02-02 00:00:00.000000 synrbl-0.0.8/Data/Validation_set/validation_set.json
+-rw-r--r--   0        0        0    22209 2020-02-02 00:00:00.000000 synrbl-0.0.8/Docs/Examples/notebook.ipynb
+-rw-r--r--   0        0        0    86666 2020-02-02 00:00:00.000000 synrbl-0.0.8/Docs/Images/Flowchart.png
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 synrbl-0.0.8/Docs/Paper_fig/figures.py
+-rw-r--r--   0        0        0    55850 2020-02-02 00:00:00.000000 synrbl-0.0.8/Pipeline/Validation/Analysis/Analysis_vis.ipynb
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 synrbl-0.0.8/Pipeline/Validation/Analysis/SynRBL - Jaworski.csv
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 synrbl-0.0.8/Pipeline/Validation/Analysis/SynRBL - USPTO_diff.csv
+-rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 synrbl-0.0.8/Pipeline/Validation/Analysis/SynRBL - USPTO_random_class.csv
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 synrbl-0.0.8/Pipeline/Validation/Analysis/SynRBL - USPTO_unbalance_class.csv
+-rw-r--r--   0        0        0    13301 2020-02-02 00:00:00.000000 synrbl-0.0.8/Pipeline/Validation/Analysis/SynRBL - golden_dataset.csv
+-rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 synrbl-0.0.8/Scripts/result_evaluation.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 synrbl-0.0.8/Scripts/synrbl_pilot.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 synrbl-0.0.8/Scripts/validation_set_interface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/__init__.py
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/test_mcs_search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynChemImputer/__init__.py
+-rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynChemImputer/test_appeal_reaction.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynChemImputer/test_curate_oxidation.py
+-rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynChemImputer/test_curate_reduction.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynChemImputer/test_molecule_standardizer.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynChemImputer/test_peroxide_imputer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/__init__.py
+-rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/test_merge.py
+-rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/test_model.py
+-rw-r--r--   0        0        0    11025 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/test_rules.py
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/test_structure.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/MissingGraph/__init__.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/MissingGraph/test_find_graph_dict.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/MissingGraph/test_find_missing_graphs.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/MissingGraph/test_molcurator.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/MissingGraph/test_uncertainty_graph.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/SubStructure/__init__.py
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/SubStructure/test_extract_common_mcs.py
+-rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/SubStructure/test_mcs_graph_detector.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/SubStructure/test_mcs_process.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynMCSImputer/SubStructure/test_substructure_analyzer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynProcessor/__init__.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynProcessor/test_check_carbon_balance.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynProcessor/test_rmsi_comparator.py
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynProcessor/test_rmsi_decomposer.py
+-rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynProcessor/test_rmsi_processing.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynProcessor/test_rsmi_both_side_process.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynRuleImputer/__init__.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynRuleImputer/test_auto_extract_rules.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynRuleImputer/test_auto_extract_smiles.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynRuleImputer/test_rule_constraint.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynRuleImputer/test_rule_data_manager.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynRuleImputer/test_synthetic_rule_imputer.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynRuleImputer/test_synthetic_rule_matcher.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynUtils/__init__.py
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynUtils/test_chem_utils.py
+-rw-r--r--   0        0        0     8918 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynUtils/test_functional_group_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynVis/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 synrbl-0.0.8/Test/SynVis/test_reaction_visualizer.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/__main__.py
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/balancing.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/confidence_prediction.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/mcs_search.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/postprocess.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/preprocess.py
+-rw-r--r--   0        0        0    14738 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/rsmi_utils.py
+-rw-r--r--   0        0        0     4726 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/rule_based.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynAnalysis/__init__.py
+-rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynAnalysis/analysis_process.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynAnalysis/analysis_utils.py
+-rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynAnalysis/eda_analysis.py
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynAnalysis/feature_analysis.py
+-rw-r--r--   0        0        0   278926 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynAnalysis/scoring_function.dump
+-rw-r--r--   0        0        0    16405 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynAnalysis/visualizer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynChemImputer/__init__.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynChemImputer/appel_reaction.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynChemImputer/compounds_template.json
+-rw-r--r--   0        0        0     7196 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynChemImputer/curate_oxidation.py
+-rw-r--r--   0        0        0     7130 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynChemImputer/curate_reduction.py
+-rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynChemImputer/molecule_standardizer.py
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynChemImputer/peroxide_imputer.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynChemImputer/post_process.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynChemImputer/reaction_template.json
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynCmd/__init__.py
+-rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynCmd/cmd_benchmark.py
+-rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynCmd/cmd_run.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynCmd/logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/__init__.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/compound_rules.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/expand_rules.json
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/merge.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/merge_rules.json
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/merge_rules_example.json
+-rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/model.py
+-rw-r--r--   0        0        0    29044 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/rules.py
+-rw-r--r--   0        0        0     6768 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/structure.py
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/MissingGraph/__init__.py
+-rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/MissingGraph/find_graph_dict.py
+-rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/MissingGraph/find_missing_graphs.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/MissingGraph/molcurator.py
+-rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/MissingGraph/refinement_uncertainty.py
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/MissingGraph/uncertainty_graph.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/SubStructure/__init__.py
+-rw-r--r--   0        0        0     9154 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/SubStructure/extract_common_mcs.py
+-rw-r--r--   0        0        0    10255 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/SubStructure/mcs_graph_detector.py
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/SubStructure/mcs_process.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynMCSImputer/SubStructure/substructure_analyzer.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynProcessor/__init__.py
+-rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynProcessor/check_carbon_balance.py
+-rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynProcessor/rsmi_both_side_process.py
+-rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynProcessor/rsmi_comparator.py
+-rw-r--r--   0        0        0     7321 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynProcessor/rsmi_decomposer.py
+-rw-r--r--   0        0        0     7210 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynProcessor/rsmi_processing.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynRuleImputer/__init__.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynRuleImputer/auto_extract_rules.py
+-rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynRuleImputer/auto_extract_smiles.py
+-rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynRuleImputer/rule_data_manager.py
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynRuleImputer/rules_manager.json.gz
+-rw-r--r--   0        0        0     9182 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynRuleImputer/synthetic_rule_constraint.py
+-rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynRuleImputer/synthetic_rule_imputer.py
+-rw-r--r--   0        0        0     8858 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynRuleImputer/synthetic_rule_matcher.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynUtils/__init__.py
+-rw-r--r--   0        0        0    11136 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynUtils/chem_utils.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynUtils/common.py
+-rw-r--r--   0        0        0    11925 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynUtils/data_utils.py
+-rw-r--r--   0        0        0     9444 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynUtils/functional_group_utils.py
+-rw-r--r--   0        0        0    14679 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynUtils/rsmi_utils.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynVis/__init__.py
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynVis/mcs_visualizer.py
+-rw-r--r--   0        0        0     9300 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynVis/reaction_visualizer.py
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynVis/rxnpdf.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 synrbl-0.0.8/synrbl/SynVis/rxnvis.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 synrbl-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 synrbl-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 synrbl-0.0.8/README.md
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 synrbl-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 synrbl-0.0.8/PKG-INFO
```

### Comparing `synrbl-0.0.7/.github/workflows/publish-package.yml` & `synrbl-0.0.8/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/.github/workflows/test-and-lint.yml` & `synrbl-0.0.8/.github/workflows/test-and-lint.yml`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Data/Raw_data/Golden/Golden.csv` & `synrbl-0.0.8/Data/Raw_data/Golden/Golden.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Data/Raw_data/Jaworski/complex.csv` & `synrbl-0.0.8/Data/Raw_data/Jaworski/complex.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Data/Raw_data/Jaworski/patent.csv` & `synrbl-0.0.8/Data/Raw_data/Jaworski/patent.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Data/Raw_data/Jaworski/typical.csv` & `synrbl-0.0.8/Data/Raw_data/Jaworski/typical.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Data/Raw_data/USPTO/USPTO_50K.csv` & `synrbl-0.0.8/Data/Raw_data/USPTO/USPTO_50K.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Data/Rules/automated_rules.json.gz` & `synrbl-0.0.8/Data/Rules/automated_rules.json.gz`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Data/Validation_set/Jaworski.csv` & `synrbl-0.0.8/Data/Validation_set/Jaworski.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Data/Validation_set/USPTO_50K.csv` & `synrbl-0.0.8/Data/Validation_set/USPTO_50K.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Data/Validation_set/USPTO_diff.csv` & `synrbl-0.0.8/Data/Validation_set/USPTO_diff.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Data/Validation_set/USPTO_random_class.csv` & `synrbl-0.0.8/Data/Validation_set/USPTO_random_class.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Data/Validation_set/USPTO_unbalance_class.csv` & `synrbl-0.0.8/Data/Validation_set/USPTO_unbalance_class.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Data/Validation_set/golden_dataset.csv` & `synrbl-0.0.8/Data/Validation_set/golden_dataset.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Data/Validation_set/validation_set.csv` & `synrbl-0.0.8/Data/Validation_set/validation_set.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Data/Validation_set/validation_set.json` & `synrbl-0.0.8/Data/Validation_set/validation_set.json`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Docs/Examples/notebook.ipynb` & `synrbl-0.0.8/Docs/Examples/notebook.ipynb`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Docs/Images/Flowchart.png` & `synrbl-0.0.8/Docs/Images/Flowchart.png`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Docs/Paper_fig/figures.py` & `synrbl-0.0.8/Docs/Paper_fig/figures.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Pipeline/Validation/Analysis/Analysis_vis.ipynb` & `synrbl-0.0.8/Pipeline/Validation/Analysis/Analysis_vis.ipynb`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Pipeline/Validation/Analysis/SynRBL - Jaworski.csv` & `synrbl-0.0.8/Pipeline/Validation/Analysis/SynRBL - Jaworski.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Pipeline/Validation/Analysis/SynRBL - USPTO_diff.csv` & `synrbl-0.0.8/Pipeline/Validation/Analysis/SynRBL - USPTO_diff.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Pipeline/Validation/Analysis/SynRBL - USPTO_random_class.csv` & `synrbl-0.0.8/Pipeline/Validation/Analysis/SynRBL - USPTO_random_class.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Pipeline/Validation/Analysis/SynRBL - USPTO_unbalance_class.csv` & `synrbl-0.0.8/Pipeline/Validation/Analysis/SynRBL - USPTO_unbalance_class.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Pipeline/Validation/Analysis/SynRBL - golden_dataset.csv` & `synrbl-0.0.8/Pipeline/Validation/Analysis/SynRBL - golden_dataset.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Scripts/result_evaluation.py` & `synrbl-0.0.8/Scripts/result_evaluation.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Scripts/synrbl_pilot.py` & `synrbl-0.0.8/Scripts/synrbl_pilot.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Scripts/validation_set_interface.py` & `synrbl-0.0.8/Scripts/validation_set_interface.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/test_mcs_search.py` & `synrbl-0.0.8/Test/test_mcs_search.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynChemImputer/test_appeal_reaction.py` & `synrbl-0.0.8/Test/SynChemImputer/test_appeal_reaction.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynChemImputer/test_molecule_standardizer.py` & `synrbl-0.0.8/Test/SynChemImputer/test_molecule_standardizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,18 +21,18 @@
         standardizer = MoleculeStandardizer(smiles)
         result = standardizer.standardize_hemiketal(smiles, atom_indices)
         expected = "C=O.O"  # Expected hemiketal cyclic structure
         self.assertEqual(
             result, expected, "Hemiketal transformation failed or incorrect"
         )
 
-    def test_MoleculeStandardizer(self):
-        smiles = "C(O)(O)C=CO"
-        standardizer = MoleculeStandardizer(smiles)
-        result = standardizer.fit()
-        expected = "O.O=CCC=O"
-        self.assertEqual(result, expected, "MoleculeStandardizer failed or incorrect")
+    # def test_MoleculeStandardizer(self):
+    #     smiles = "C(O)(O)C=CO"
+    #     standardizer = MoleculeStandardizer(smiles)
+    #     result = standardizer.fit()
+    #     expected = "O.O=CCC=O"
+    #     self.assertEqual(result, expected, "MoleculeStandardizer failed or incorrect")
 
 
 # If the script is executed directly, run the tests
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `synrbl-0.0.7/Test/SynChemImputer/test_peroxide_imputer.py` & `synrbl-0.0.8/Test/SynChemImputer/test_peroxide_imputer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynMCSImputer/test_merge.py` & `synrbl-0.0.8/Test/SynMCSImputer/test_merge.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynMCSImputer/test_model.py` & `synrbl-0.0.8/Test/SynMCSImputer/test_model.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynMCSImputer/test_rules.py` & `synrbl-0.0.8/Test/SynMCSImputer/test_rules.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynMCSImputer/test_structure.py` & `synrbl-0.0.8/Test/SynMCSImputer/test_structure.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynMCSImputer/test_utils.py` & `synrbl-0.0.8/Test/SynMCSImputer/test_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynMCSImputer/MissingGraph/test_find_graph_dict.py` & `synrbl-0.0.8/Test/SynMCSImputer/MissingGraph/test_find_graph_dict.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynMCSImputer/MissingGraph/test_find_missing_graphs.py` & `synrbl-0.0.8/Test/SynMCSImputer/MissingGraph/test_find_missing_graphs.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynMCSImputer/MissingGraph/test_molcurator.py` & `synrbl-0.0.8/Test/SynMCSImputer/MissingGraph/test_molcurator.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynMCSImputer/MissingGraph/test_uncertainty_graph.py` & `synrbl-0.0.8/Test/SynMCSImputer/MissingGraph/test_uncertainty_graph.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynMCSImputer/SubStructure/test_extract_common_mcs.py` & `synrbl-0.0.8/Test/SynMCSImputer/SubStructure/test_extract_common_mcs.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynMCSImputer/SubStructure/test_mcs_graph_detector.py` & `synrbl-0.0.8/Test/SynMCSImputer/SubStructure/test_mcs_graph_detector.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynMCSImputer/SubStructure/test_mcs_process.py` & `synrbl-0.0.8/Test/SynMCSImputer/SubStructure/test_mcs_process.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynMCSImputer/SubStructure/test_substructure_analyzer.py` & `synrbl-0.0.8/Test/SynMCSImputer/SubStructure/test_substructure_analyzer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynProcessor/test_check_carbon_balance.py` & `synrbl-0.0.8/Test/SynProcessor/test_check_carbon_balance.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynProcessor/test_rmsi_comparator.py` & `synrbl-0.0.8/Test/SynProcessor/test_rmsi_comparator.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynProcessor/test_rmsi_decomposer.py` & `synrbl-0.0.8/Test/SynProcessor/test_rmsi_decomposer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynProcessor/test_rmsi_processing.py` & `synrbl-0.0.8/Test/SynProcessor/test_rmsi_processing.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynProcessor/test_rsmi_both_side_process.py` & `synrbl-0.0.8/Test/SynProcessor/test_rsmi_both_side_process.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynRuleImputer/test_auto_extract_rules.py` & `synrbl-0.0.8/Test/SynRuleImputer/test_auto_extract_rules.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynRuleImputer/test_auto_extract_smiles.py` & `synrbl-0.0.8/Test/SynRuleImputer/test_auto_extract_smiles.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynRuleImputer/test_rule_constraint.py` & `synrbl-0.0.8/Test/SynRuleImputer/test_rule_constraint.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynRuleImputer/test_rule_data_manager.py` & `synrbl-0.0.8/Test/SynRuleImputer/test_rule_data_manager.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynRuleImputer/test_synthetic_rule_imputer.py` & `synrbl-0.0.8/Test/SynRuleImputer/test_synthetic_rule_imputer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynRuleImputer/test_synthetic_rule_matcher.py` & `synrbl-0.0.8/Test/SynRuleImputer/test_synthetic_rule_matcher.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynUtils/test_chem_utils.py` & `synrbl-0.0.8/Test/SynUtils/test_chem_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynUtils/test_functional_group_utils.py` & `synrbl-0.0.8/Test/SynUtils/test_functional_group_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/Test/SynVis/test_reaction_visualizer.py` & `synrbl-0.0.8/Test/SynVis/test_reaction_visualizer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/balancing.py` & `synrbl-0.0.8/synrbl/balancing.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/confidence_prediction.py` & `synrbl-0.0.8/synrbl/confidence_prediction.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,13 +74,13 @@
                 if c >= threshold:
                     conf_success += 1
                 else:
                     assert (
                         r[self.issue_col] == ""
                     ), "Issue column has value for a solved reaction?"
                     r[self.solved_col] = False
-                    r[
-                        self.issue_col
-                    ] = "Confidence is below the threshold of {:.2%}.".format(threshold)
+                    r[self.issue_col] = (
+                        "Confidence is below the threshold of {:.2%}.".format(threshold)
+                    )
         if stats is not None:
             stats["confident_cnt"] = conf_success
         return reactions
```

### Comparing `synrbl-0.0.7/synrbl/mcs_search.py` & `synrbl-0.0.8/synrbl/mcs_search.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/postprocess.py` & `synrbl-0.0.8/synrbl/postprocess.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/preprocess.py` & `synrbl-0.0.8/synrbl/preprocess.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/rsmi_utils.py` & `synrbl-0.0.8/synrbl/rsmi_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/rule_based.py` & `synrbl-0.0.8/synrbl/rule_based.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,19 @@
 
 
 class RuleBasedMethod:
     def __init__(self, id_col, reaction_col, output_col, rules_path=None, n_jobs=1):
         self.id_col = id_col
         self.reaction_col = reaction_col
         if rules_path is None:
-            with importlib.resources.files(synrbl.SynRuleImputer).joinpath(
-                "rules_manager.json.gz"
-            ).open("r") as f:
+            with (
+                importlib.resources.files(synrbl.SynRuleImputer)
+                .joinpath("rules_manager.json.gz")
+                .open("r") as f
+            ):
                 self.rules = json.load(f)
         else:
             self.rules = load_database(rules_path)
         self.n_jobs = n_jobs
         self.output_col = output_col
 
     def run(self, reactions, stats=None):
```

### Comparing `synrbl-0.0.7/synrbl/SynAnalysis/analysis_process.py` & `synrbl-0.0.8/synrbl/SynAnalysis/analysis_process.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynAnalysis/analysis_utils.py` & `synrbl-0.0.8/synrbl/SynAnalysis/analysis_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynAnalysis/eda_analysis.py` & `synrbl-0.0.8/synrbl/SynAnalysis/eda_analysis.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynAnalysis/feature_analysis.py` & `synrbl-0.0.8/synrbl/SynAnalysis/feature_analysis.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynAnalysis/scoring_function.dump` & `synrbl-0.0.8/synrbl/SynAnalysis/scoring_function.dump`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynAnalysis/visualizer.py` & `synrbl-0.0.8/synrbl/SynAnalysis/visualizer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynChemImputer/appel_reaction.py` & `synrbl-0.0.8/synrbl/SynChemImputer/appel_reaction.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynChemImputer/molecule_standardizer.py` & `synrbl-0.0.8/synrbl/SynChemImputer/molecule_standardizer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynChemImputer/peroxide_imputer.py` & `synrbl-0.0.8/synrbl/SynChemImputer/peroxide_imputer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynCmd/__init__.py` & `synrbl-0.0.8/synrbl/SynCmd/__init__.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynCmd/cmd_benchmark.py` & `synrbl-0.0.8/synrbl/SynCmd/cmd_benchmark.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynCmd/cmd_run.py` & `synrbl-0.0.8/synrbl/SynCmd/cmd_run.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynMCSImputer/compound_rules.json` & `synrbl-0.0.8/synrbl/SynMCSImputer/compound_rules.json`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynMCSImputer/expand_rules.json` & `synrbl-0.0.8/synrbl/SynMCSImputer/expand_rules.json`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynMCSImputer/merge.py` & `synrbl-0.0.8/synrbl/SynMCSImputer/merge.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynMCSImputer/merge_rules.json` & `synrbl-0.0.8/synrbl/SynMCSImputer/merge_rules.json`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynMCSImputer/model.py` & `synrbl-0.0.8/synrbl/SynMCSImputer/model.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynMCSImputer/rules.py` & `synrbl-0.0.8/synrbl/SynMCSImputer/rules.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynMCSImputer/structure.py` & `synrbl-0.0.8/synrbl/SynMCSImputer/structure.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynMCSImputer/utils.py` & `synrbl-0.0.8/synrbl/SynMCSImputer/utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynMCSImputer/MissingGraph/find_graph_dict.py` & `synrbl-0.0.8/synrbl/SynMCSImputer/MissingGraph/find_graph_dict.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynMCSImputer/MissingGraph/find_missing_graphs.py` & `synrbl-0.0.8/synrbl/SynMCSImputer/MissingGraph/find_missing_graphs.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynMCSImputer/MissingGraph/molcurator.py` & `synrbl-0.0.8/synrbl/SynMCSImputer/MissingGraph/molcurator.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynMCSImputer/MissingGraph/refinement_uncertainty.py` & `synrbl-0.0.8/synrbl/SynMCSImputer/MissingGraph/refinement_uncertainty.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynMCSImputer/MissingGraph/uncertainty_graph.py` & `synrbl-0.0.8/synrbl/SynMCSImputer/MissingGraph/uncertainty_graph.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynMCSImputer/SubStructure/extract_common_mcs.py` & `synrbl-0.0.8/synrbl/SynMCSImputer/SubStructure/extract_common_mcs.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynMCSImputer/SubStructure/mcs_graph_detector.py` & `synrbl-0.0.8/synrbl/SynMCSImputer/SubStructure/mcs_graph_detector.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynMCSImputer/SubStructure/mcs_process.py` & `synrbl-0.0.8/synrbl/SynMCSImputer/SubStructure/mcs_process.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynMCSImputer/SubStructure/substructure_analyzer.py` & `synrbl-0.0.8/synrbl/SynMCSImputer/SubStructure/substructure_analyzer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynProcessor/check_carbon_balance.py` & `synrbl-0.0.8/synrbl/SynProcessor/check_carbon_balance.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynProcessor/rsmi_both_side_process.py` & `synrbl-0.0.8/synrbl/SynProcessor/rsmi_both_side_process.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynProcessor/rsmi_comparator.py` & `synrbl-0.0.8/synrbl/SynProcessor/rsmi_comparator.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynProcessor/rsmi_decomposer.py` & `synrbl-0.0.8/synrbl/SynProcessor/rsmi_decomposer.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         79: "Au",
         80: "Hg",
         81: "Tl",
         82: "Pb",
         83: "Bi",
         84: "Po",
         85: "At",
-        86: "Rn"
+        86: "Rn",
         # This covers elements up to Radon (Rn). Extend further if needed.
     }
 
     def __init__(
         self,
         smiles: str = None,
         data: Union[List[str], pd.DataFrame] = None,
```

### Comparing `synrbl-0.0.7/synrbl/SynProcessor/rsmi_processing.py` & `synrbl-0.0.8/synrbl/SynProcessor/rsmi_processing.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynRuleImputer/auto_extract_rules.py` & `synrbl-0.0.8/synrbl/SynRuleImputer/auto_extract_rules.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynRuleImputer/auto_extract_smiles.py` & `synrbl-0.0.8/synrbl/SynRuleImputer/auto_extract_smiles.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynRuleImputer/rule_data_manager.py` & `synrbl-0.0.8/synrbl/SynRuleImputer/rule_data_manager.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynRuleImputer/rules_manager.json.gz` & `synrbl-0.0.8/synrbl/SynRuleImputer/rules_manager.json.gz`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynRuleImputer/synthetic_rule_constraint.py` & `synrbl-0.0.8/synrbl/SynRuleImputer/synthetic_rule_constraint.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynRuleImputer/synthetic_rule_imputer.py` & `synrbl-0.0.8/synrbl/SynRuleImputer/synthetic_rule_imputer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynRuleImputer/synthetic_rule_matcher.py` & `synrbl-0.0.8/synrbl/SynRuleImputer/synthetic_rule_matcher.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynUtils/chem_utils.py` & `synrbl-0.0.8/synrbl/SynUtils/chem_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 import numpy as np
 
 import rdkit.Chem as Chem
 import rdkit.DataStructs as DataStructs
 import rdkit.Chem.rdFingerprintGenerator as rdFingerprintGenerator
 import rdkit.Chem.AllChem as AllChem
 import rdkit.Chem.rdmolfiles as rdmolfiles
-
-
-from typing import List, Dict
-from typing import Union
+from collections import Counter
+from typing import List, Dict, Tuple, Optional, Union
+from fgutils import FGQuery
 
 
 class CheckCarbonBalance:
     def __init__(
         self, reactions_data: List[Dict[str, str]], rsmi_col="reactions", symbol=">>"
     ):
         """
@@ -226,7 +225,89 @@
     if exp == res:
         return 1
     exp_e, exp_p = exp.split(">>")
     res_e, res_p = res.split(">>")
     exp_ed, res_ed = _get_diff_mol(exp_e, res_e)
     exp_pd, res_pd = _get_diff_mol(exp_p, res_p)
     return np.min([_fp(exp_ed, res_ed), _fp(exp_pd, res_pd)])
+
+
+def check_for_isolated_atom(smiles: str, atom: Optional[str] = "H") -> bool:
+    """
+    Checks if a specified type of isolated atom (hydrogen by default, or oxygen)
+    exists in a SMILES string.
+    """
+    # Pattern to find isolated atoms; not connected to any other atoms
+    pattern = rf"\[{atom}\](?![^[]*\])"
+    return bool(re.search(pattern, smiles))
+
+
+def count_radical_atoms(smiles: str, atomic_num: int) -> int:
+    """
+    Counts isolated radical atoms in SMILES string.
+    """
+    mol = Chem.MolFromSmiles(smiles)
+    radical_count = 0
+
+    # Iterate over all atoms in the molecule
+    for atom in mol.GetAtoms():
+
+        if atom.GetAtomicNum() == atomic_num and atom.GetNumRadicalElectrons() > 0:
+            # Further check if the atom is isolated (has no neighbors)
+            if len(atom.GetNeighbors()) == 0:
+                radical_count += 1
+
+    return radical_count
+
+
+def list_difference(
+    list1: List[str], list2: List[str]
+) -> Tuple[Dict[str, int], Dict[str, int]]:
+    """
+    Compares two lists and returns dictionaries that count unique occurrences
+    Parameters:
+    list1 (List[str]): First list of items for comparison.
+    list2 (List[str]): Second list of items for comparison.
+
+    Returns:
+    Tuple[Dict[str, int], Dict[str, int]]: A tuple of two dictionaries:
+        - First dictionary: Items unique to the first list with their counts.
+        - Second dictionary: Items unique to the second list with their counts.
+    """
+    count1 = Counter(list1)
+    count2 = Counter(list2)
+    unique_to_list1 = {}
+    unique_to_list2 = {}
+
+    for key, count in count1.items():
+        if key not in count2:
+            unique_to_list1[key] = count
+        elif count > count2[key]:
+            unique_to_list1[key] = count - count2[key]
+
+    for key, count in count2.items():
+        if key not in count1:
+            unique_to_list2[key] = count
+        elif count > count1[key]:
+            unique_to_list2[key] = count - count1[key]
+
+    return unique_to_list1, unique_to_list2
+
+
+def find_functional_reactivity(reaction_smiles: str) -> Tuple[List[str], List[str]]:
+    """
+    Analyzes functional groups
+
+    Parameters:
+    reaction_smiles (str): SMILES string of the reaction
+    Returns:
+    Tuple[List[str], List[str]]: Two lists containing unique functional groups
+    in reactants and products, respectively.
+    """
+    query = FGQuery(use_smiles=True)
+    reactant, product = reaction_smiles.split(">>")
+    fg_reactant = query.get(reactant)
+    fg_product = query.get(product)
+    fg_reactant = [value[0] for value in fg_reactant]
+    fg_product = [value[0] for value in fg_product]
+    reactant_fg, product_fg = list_difference(fg_reactant, fg_product)
+    return list(reactant_fg.keys()), list(product_fg.keys())
```

### Comparing `synrbl-0.0.7/synrbl/SynUtils/data_utils.py` & `synrbl-0.0.8/synrbl/SynUtils/data_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynUtils/functional_group_utils.py` & `synrbl-0.0.8/synrbl/SynUtils/functional_group_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynUtils/rsmi_utils.py` & `synrbl-0.0.8/synrbl/SynUtils/rsmi_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynVis/mcs_visualizer.py` & `synrbl-0.0.8/synrbl/SynVis/mcs_visualizer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynVis/reaction_visualizer.py` & `synrbl-0.0.8/synrbl/SynVis/reaction_visualizer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynVis/rxnpdf.py` & `synrbl-0.0.8/synrbl/SynVis/rxnpdf.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/synrbl/SynVis/rxnvis.py` & `synrbl-0.0.8/synrbl/SynVis/rxnvis.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/.gitignore` & `synrbl-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/LICENSE` & `synrbl-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/README.md` & `synrbl-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.7/pyproject.toml` & `synrbl-0.0.8/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "synrbl"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
 	{name="Tieu Long Phan", email="long.tieu_phan@uni-leipzig.de"}, 
 	{name="Klaus Weinbauer", email="klaus@bioinf.uni-leipzig.de"}
 	]
 description = "Synthesis Rebalancing Framework for Computational Chemistry"
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `synrbl-0.0.7/PKG-INFO` & `synrbl-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: synrbl
-Version: 0.0.7
+Version: 0.0.8
 Summary: Synthesis Rebalancing Framework for Computational Chemistry
 Project-URL: homepage, https://github.com/TieuLongPhan/SynRBL
 Project-URL: source, https://github.com/TieuLongPhan/SynRBL
 Project-URL: issues, https://github.com/TieuLongPhan/SynRBL/issues
 Author-email: Tieu Long Phan <long.tieu_phan@uni-leipzig.de>, Klaus Weinbauer <klaus@bioinf.uni-leipzig.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```


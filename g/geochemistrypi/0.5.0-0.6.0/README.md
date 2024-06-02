# Comparing `tmp/geochemistrypi-0.5.0.tar.gz` & `tmp/geochemistrypi-0.6.0.tar.gz`

## Comparing `geochemistrypi-0.5.0.tar` & `geochemistrypi-0.6.0.tar`

### file list

```diff
@@ -1,200 +1,198 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/.flake8
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/.readthedocs.yaml
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/Dockerfile
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/.github/CODEOWNERES
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/.github/workflows/geochemistrypi.yml
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/Geochemistry π.ico
--rw-r--r--   0        0        0   285992 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/Geochemistry π.png
--rw-r--r--   0        0        0   255925 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/Geochemistryπ-Activity Diagram_v1.png
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/Makefile
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/make.bat
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/conf.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/contact us.rst
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/contributing.rst
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/index.rst
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/model example.rst
--rw-r--r--   0        0        0    13006 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/For Developer/A Completed Pull Request.md
--rw-r--r--   0        0        0    15265 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/For Developer/Add New Model To Framework.md
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/For Developer/Developer Docs link.md
--rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/For Developer/Docker Deployment.md
--rw-r--r--   0        0        0     6673 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/For Developer/Local Deployment.md
--rw-r--r--   0        0        0    14020 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/For Developer/Contributing/Code_of_Conduct.md
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/For Developer/Contributing/Contributor.md
--rw-r--r--   0        0        0    15403 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/For Developer/Developer Guide/Developer Manual.md
--rw-r--r--   0        0        0     5480 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/For User/Installation Manual.md
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/For User/User Docs link.md
--rw-r--r--   0        0        0    16645 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/For User/User Guide.md
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/For User/Contact us/Join us.md
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/For User/Contact us/Q&A.md
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/For User/Contact us/bug_report.md
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/For User/Contact us/bug_template.md
--rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/For User/Model Example/Classification/classification.md
--rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/For User/Model Example/Clustering/Clustering.md
--rw-r--r--   0        0        0    11187 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/For User/Model Example/Data_Preprocessing/Data Preprocessing.md
--rw-r--r--   0        0        0    19824 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/For User/Model Example/Decomposition/decomposition.md
--rw-r--r--   0        0        0    24306 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/For User/Model Example/Regression/Regression.md
--rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/Home/CHANGELOG.md
--rw-r--r--   0        0        0     6029 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/Home/Introduction.md
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/python_apis/api.rst
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/python_apis/geochemistrypi.auth.rst
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/python_apis/geochemistrypi.data_mining.data.rst
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/python_apis/geochemistrypi.data_mining.model.func.algo_classification.rst
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/python_apis/geochemistrypi.data_mining.model.func.algo_clustering.rst
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/python_apis/geochemistrypi.data_mining.model.func.algo_decomposition.rst
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/python_apis/geochemistrypi.data_mining.model.func.algo_regression.rst
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/python_apis/geochemistrypi.data_mining.model.func.rst
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/python_apis/geochemistrypi.data_mining.model.rst
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/python_apis/geochemistrypi.data_mining.plot.rst
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/python_apis/geochemistrypi.data_mining.process.rst
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/python_apis/geochemistrypi.data_mining.rst
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/python_apis/geochemistrypi.data_mining.tests.rst
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/python_apis/geochemistrypi.data_mining.tests.test_data.rst
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/python_apis/geochemistrypi.data_mining.utils.rst
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/python_apis/geochemistrypi.rst
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/docs/source/python_apis/modules.rst
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/_version.py
--rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/cli.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/database.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/start_cli_pipeline.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/start_dash_pipeline.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/auth/__init__.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/auth/constants.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/auth/dependencies.py
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/auth/router.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/auth/schemas.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/auth/service.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/auth/sql_models.py
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/auth/utils.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/__init__.py
--rw-r--r--   0        0        0    37658 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/cli_pipeline.py
--rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/constants.py
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/dash_pipeline.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/router.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/schemas.py
--rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/service.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/sql_models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/data/__init__.py
--rw-r--r--   0        0        0    17073 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/data/data_readiness.py
--rw-r--r--   0        0        0     9149 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/data/feature_engineering.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/data/imputation.py
--rw-r--r--   0        0        0     5762 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/data/inference.py
--rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/data/preprocessing.py
--rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/data/statistic.py
--rw-r--r--   0        0        0   223070 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/data/dataset/Data_Classification.xlsx
--rw-r--r--   0        0        0   225363 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/data/dataset/Data_Clustering.xlsx
--rw-r--r--   0        0        0    44562 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/data/dataset/Data_Decomposition.xlsx
--rw-r--r--   0        0        0    44562 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/data/dataset/Data_Regression.xlsx
--rw-r--r--   0        0        0   173418 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/data/dataset/InferenceData_Classification.xlsx
--rw-r--r--   0        0        0   225363 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/data/dataset/InferenceData_Clustering.xlsx
--rw-r--r--   0        0        0    44562 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/data/dataset/InferenceData_Decomposition.xlsx
--rw-r--r--   0        0        0    21185 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/data/dataset/InferenceData_Regression.xlsx
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/data/dataset/~$Data_Classification.xlsx
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/__init__.py
--rw-r--r--   0        0        0    16495 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/_base.py
--rw-r--r--   0        0        0   158038 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/classification.py
--rw-r--r--   0        0        0    26774 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/clustering.py
--rw-r--r--   0        0        0    28209 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/decomposition.py
--rw-r--r--   0        0        0   180657 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/regression.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/__init__.py
--rw-r--r--   0        0        0     9502 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/_common_supervised.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_classification/__init__.py
--rw-r--r--   0        0        0    19352 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_classification/_common.py
--rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_classification/_decision_tree.py
--rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_classification/_extra_trees.py
--rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_classification/_gradient_boosting.py
--rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_classification/_knn.py
--rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_classification/_logistic_regression.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_classification/_multi_layer_perceptron.py
--rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_classification/_rf.py
--rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_classification/_sgd_classification.py
--rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_classification/_svc.py
--rw-r--r--   0        0        0     8891 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_classification/_xgboost.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_clustering/__init__.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_clustering/_agglomerative.py
--rw-r--r--   0        0        0    10724 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_clustering/_common.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_clustering/_dbscan.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_clustering/_kmeans.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_decomposition/__init__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_decomposition/_common.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_decomposition/_mds.py
--rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_decomposition/_pca.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_decomposition/_tsne.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/__init__.py
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_bayesianridge_regression.py
--rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_common.py
--rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_decision_tree.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_elastic_net.py
--rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_extra_tree.py
--rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_gradient_boosting.py
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_knn.py
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_lasso_regression.py
--rw-r--r--   0        0        0     4554 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_linear_regression.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_multi_layer_perceptron.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_polynomial_regression.py
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_rf.py
--rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_sgd_regression.py
--rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_svr.py
--rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_xgboost.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/plot/__init__.py
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/plot/geochemistry_plot.py
--rw-r--r--   0        0        0     9017 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/plot/map_plot.py
--rw-r--r--   0        0        0     5917 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/plot/statistic_plot.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/process/__init__.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/process/_base.py
--rw-r--r--   0        0        0    12488 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/process/classify.py
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/process/cluster.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/process/decompose.py
--rw-r--r--   0        0        0    14234 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/process/regress.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/tests/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/tests/test_data/__init__.py
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/tests/test_data/test_data_readiness.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/utils/__init__.py
--rw-r--r--   0        0        0    11067 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/utils/base.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/utils/exceptions.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/data_mining/utils/mlflow_utils.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/frontend/.babelrc
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/frontend/.eslintrc.js
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/frontend/.prettierrc.js
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/frontend/package.json
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/frontend/tsconfig.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/frontend/webpack.config.js
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/frontend/public/index.html
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/frontend/src/App.tsx
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/frontend/src/index.tsx
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/frontend/src/types.d.ts
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/frontend/src/components/Dashboard.tsx
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/frontend/src/components/DataFrame.tsx
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/frontend/src/components/Dataset.tsx
--rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/frontend/src/components/DatasetDisplay.tsx
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/frontend/src/components/Header.tsx
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/frontend/src/components/Login.tsx
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/frontend/src/components/Profile.tsx
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/frontend/src/components/RefreshHandler.tsx
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/frontend/src/components/Register.tsx
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/frontend/src/helpers/apiCall.ts
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/frontend/src/helpers/apiCallWrappers.ts
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/frontend/src/helpers/constants.ts
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/frontend/src/helpers/cookies.ts
--rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/frontend/src/pages/HomePage.tsx
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/geochemistrypi/frontend/src/pages/LoginPage.tsx
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/requirements/development.txt
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/requirements/production.txt
--rw-r--r--   0        0        0   225291 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/test/Data_Binary_Classification.xlsx
--rw-r--r--   0        0        0   225291 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/test/Data_Classification.xlsx
--rw-r--r--   0        0        0   223282 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/test/Data_Multi_Classification.xlsx
--rw-r--r--   0        0        0    44525 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/test/Data_Regression.xlsx
--rw-r--r--   0        0        0     7467 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/test/Data_Regression_Clean.xlsx
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/test/test1.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/test/test2.py
--rw-r--r--   0        0        0     6198 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/test_python/auto_0.py
--rw-r--r--   0        0        0    15210 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/test_python/test.xlsx
--rw-r--r--   0        0        0   225291 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/test_python/test_data/Data_Binary_Classification.xlsx
--rw-r--r--   0        0        0   223282 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/test_python/test_data/Data_Multi_Classification.xlsx
--rw-r--r--   0        0        0   173418 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/test_python/test_data/InferenceData_Classification.xlsx
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/LICENSE
--rw-r--r--   0        0        0    15915 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/README.md
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    18733 2020-02-02 00:00:00.000000 geochemistrypi-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/.flake8
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/Dockerfile
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/.github/CODEOWNERES
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/.github/workflows/geochemistrypi.yml
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/Geochemistry π.ico
+-rw-r--r--   0        0        0   285992 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/Geochemistry π.png
+-rw-r--r--   0        0        0   255925 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/Geochemistryπ-Activity Diagram_v1.png
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/Makefile
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/make.bat
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/conf.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/contact us.rst
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/contributing.rst
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/deployment.rst
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/index.rst
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/model example.rst
+-rw-r--r--   0        0        0    13006 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/For Developer/A Completed Pull Request.md
+-rw-r--r--   0        0        0    23492 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/For Developer/Add New Model To Framework.md
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/For Developer/Developer Docs link.md
+-rw-r--r--   0        0        0    14019 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/For Developer/Contributing/Code_of_Conduct.md
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/For Developer/Contributing/Contributor.md
+-rw-r--r--   0        0        0     5320 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/For Developer/Deployment/Docker Deployment.md
+-rw-r--r--   0        0        0     6673 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/For Developer/Deployment/Local Deployment.md
+-rw-r--r--   0        0        0    15403 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/For Developer/Developer Guide/Developer Manual.md
+-rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/For User/Installation Manual.md
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/For User/User Docs link.md
+-rw-r--r--   0        0        0    17047 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/For User/User Guide.md
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/For User/Contact us/Join us.md
+-rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/For User/Contact us/Q&A.md
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/For User/Contact us/bug_report.md
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/For User/Contact us/bug_template.md
+-rw-r--r--   0        0        0    22624 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/For User/Model Example/Abnormal_Detection/abnormal_detection.md
+-rw-r--r--   0        0        0    25352 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/For User/Model Example/Classification/classification.md
+-rw-r--r--   0        0        0    21232 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/For User/Model Example/Clustering/Clustering.md
+-rw-r--r--   0        0        0    14566 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/For User/Model Example/Data_Preprocessing/Data Preprocessing.md
+-rw-r--r--   0        0        0    19712 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/For User/Model Example/Decomposition/decomposition.md
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/For User/Model Example/Network_Analysis/Network Analysis.md
+-rw-r--r--   0        0        0    24306 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/For User/Model Example/Regression/Regression.md
+-rw-r--r--   0        0        0     3841 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/Home/CHANGELOG.md
+-rw-r--r--   0        0        0    20837 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/Home/Introduction.md
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/python_apis/api.rst
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/python_apis/geochemistrypi.auth.rst
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/python_apis/geochemistrypi.data_mining.data.rst
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/python_apis/geochemistrypi.data_mining.model.func.algo_abnormaldetection.rst
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/python_apis/geochemistrypi.data_mining.model.func.algo_classification.rst
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/python_apis/geochemistrypi.data_mining.model.func.algo_clustering.rst
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/python_apis/geochemistrypi.data_mining.model.func.algo_decomposition.rst
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/python_apis/geochemistrypi.data_mining.model.func.algo_regression.rst
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/python_apis/geochemistrypi.data_mining.model.func.rst
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/python_apis/geochemistrypi.data_mining.model.rst
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/python_apis/geochemistrypi.data_mining.plot.rst
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/python_apis/geochemistrypi.data_mining.process.rst
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/python_apis/geochemistrypi.data_mining.rst
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/python_apis/geochemistrypi.data_mining.tests.rst
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/python_apis/geochemistrypi.data_mining.tests.test_data.rst
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/python_apis/geochemistrypi.data_mining.utils.rst
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/python_apis/geochemistrypi.rst
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/docs/source/python_apis/modules.rst
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/_version.py
+-rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/cli.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/database.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/start_cli_pipeline.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/start_dash_pipeline.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/auth/__init__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/auth/constants.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/auth/dependencies.py
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/auth/router.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/auth/schemas.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/auth/service.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/auth/sql_models.py
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/auth/utils.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/__init__.py
+-rw-r--r--   0        0        0    41037 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/cli_pipeline.py
+-rw-r--r--   0        0        0     3841 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/constants.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/dash_pipeline.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/enum.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/router.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/schemas.py
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/service.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/sql_models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/data/__init__.py
+-rw-r--r--   0        0        0    17355 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/data/data_readiness.py
+-rw-r--r--   0        0        0     9149 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/data/feature_engineering.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/data/imputation.py
+-rw-r--r--   0        0        0     5762 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/data/inference.py
+-rw-r--r--   0        0        0     3217 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/data/preprocessing.py
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/data/statistic.py
+-rw-r--r--   0        0        0   173418 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/data/dataset/ApplicationData_Classification.xlsx
+-rw-r--r--   0        0        0    21185 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/data/dataset/ApplicationData_Regression.xlsx
+-rw-r--r--   0        0        0    44562 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/data/dataset/Data_AbnormalDetection.xlsx
+-rw-r--r--   0        0        0   225291 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/data/dataset/Data_Classification.xlsx
+-rw-r--r--   0        0        0   225363 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/data/dataset/Data_Clustering.xlsx
+-rw-r--r--   0        0        0    44562 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/data/dataset/Data_Decomposition.xlsx
+-rw-r--r--   0        0        0    44562 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/data/dataset/Data_Regression.xlsx
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/data/dataset/~$Data_Decomposition.xlsx
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/__init__.py
+-rw-r--r--   0        0        0    16755 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/_base.py
+-rw-r--r--   0        0        0   158420 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/classification.py
+-rw-r--r--   0        0        0    29544 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/clustering.py
+-rw-r--r--   0        0        0    30846 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/decomposition.py
+-rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/detection.py
+-rw-r--r--   0        0        0   198125 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/regression.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/__init__.py
+-rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/_common_supervised.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_abnormaldetection/__init__.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_abnormaldetection/_iforest.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_classification/__init__.py
+-rw-r--r--   0        0        0    19352 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_classification/_common.py
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_classification/_decision_tree.py
+-rw-r--r--   0        0        0     4114 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_classification/_extra_trees.py
+-rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_classification/_gradient_boosting.py
+-rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_classification/_knn.py
+-rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_classification/_logistic_regression.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_classification/_multi_layer_perceptron.py
+-rw-r--r--   0        0        0     4141 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_classification/_rf.py
+-rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_classification/_sgd_classification.py
+-rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_classification/_svc.py
+-rw-r--r--   0        0        0     8891 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_classification/_xgboost.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_clustering/__init__.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_clustering/_affinitypropagation.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_clustering/_agglomerative.py
+-rw-r--r--   0        0        0    10724 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_clustering/_common.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_clustering/_dbscan.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_clustering/_kmeans.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_decomposition/__init__.py
+-rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_decomposition/_common.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_decomposition/_mds.py
+-rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_decomposition/_pca.py
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_decomposition/_tsne.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/__init__.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_bayesianridge_regression.py
+-rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_common.py
+-rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_decision_tree.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_elastic_net.py
+-rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_extra_tree.py
+-rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_gradient_boosting.py
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_knn.py
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_lasso_regression.py
+-rw-r--r--   0        0        0     4554 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_linear_regression.py
+-rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_multi_layer_perceptron.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_polynomial_regression.py
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_rf.py
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_ridge_regression.py
+-rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_sgd_regression.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_svr.py
+-rw-r--r--   0        0        0     4000 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_xgboost.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/plot/__init__.py
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/plot/geochemistry_plot.py
+-rw-r--r--   0        0        0     9017 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/plot/map_plot.py
+-rw-r--r--   0        0        0     5917 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/plot/statistic_plot.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/process/__init__.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/process/_base.py
+-rw-r--r--   0        0        0    13285 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/process/classify.py
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/process/cluster.py
+-rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/process/decompose.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/process/detect.py
+-rw-r--r--   0        0        0    15556 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/process/regress.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/tests/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/tests/test_data/__init__.py
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/tests/test_data/test_data_readiness.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/utils/__init__.py
+-rw-r--r--   0        0        0    12238 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/utils/base.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/utils/exceptions.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/data_mining/utils/mlflow_utils.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/frontend/.babelrc
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/frontend/.eslintrc.js
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/frontend/.prettierrc.js
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/frontend/package.json
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/frontend/tsconfig.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/frontend/webpack.config.js
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/frontend/public/index.html
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/frontend/src/App.tsx
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/frontend/src/index.tsx
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/frontend/src/types.d.ts
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/frontend/src/components/Dashboard.tsx
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/frontend/src/components/DataFrame.tsx
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/frontend/src/components/Dataset.tsx
+-rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/frontend/src/components/DatasetDisplay.tsx
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/frontend/src/components/Header.tsx
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/frontend/src/components/Login.tsx
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/frontend/src/components/Profile.tsx
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/frontend/src/components/RefreshHandler.tsx
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/frontend/src/components/Register.tsx
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/frontend/src/helpers/apiCall.ts
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/frontend/src/helpers/apiCallWrappers.ts
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/frontend/src/helpers/constants.ts
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/frontend/src/helpers/cookies.ts
+-rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/frontend/src/pages/HomePage.tsx
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/geochemistrypi/frontend/src/pages/LoginPage.tsx
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/requirements/development.txt
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/requirements/production.txt
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/LICENSE
+-rw-r--r--   0        0        0    20642 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/README.md
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    23518 2020-02-02 00:00:00.000000 geochemistrypi-0.6.0/PKG-INFO
```

### Comparing `geochemistrypi-0.5.0/.pre-commit-config.yaml` & `geochemistrypi-0.6.0/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -54,23 +54,23 @@
         description: Check Python code for style and possible errors
         files: \.(py|pyx)$
         # args: [--max-line-length=200, --max-complexity=100, --ignore=F811,W605]
         # Use config file to pass multiple values to the argument
         args: [--config=.flake8]
         exclude: ^node_modules/
 
-  - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v2.7.1
-    hooks:
-      - id: prettier
-        name: Frontend Code Formatter
-        description: Apply the Prettier code formatter
-        files: \.(js|jsx|css|ts|tsx)$
-        args: [--write, --semi=true, --single-quote=true, --trailing-comma=all, --print-width=200, --tab-width=4, --jsx-single-quote=false]
-        exclude: ^node_modules/
+  # - repo: https://github.com/pre-commit/mirrors-prettier
+  #   rev: v2.7.1
+  #   hooks:
+  #     - id: prettier
+  #       name: Frontend Code Formatter
+  #       description: Apply the Prettier code formatter
+  #       files: \.(js|jsx|css|ts|tsx)$
+  #       args: [--write, --semi=true, --single-quote=true, --trailing-comma=all, --print-width=200, --tab-width=4, --jsx-single-quote=false]
+  #       exclude: ^node_modules/
 
   # Problem: some dependencies cannot be installed with pre-commit
   # - repo: https://github.com/pre-commit/mirrors-eslint
   #   rev: v7.32.0
   #   hooks:
   #     - id: eslint
   #       name: ESlint Linter
```

### Comparing `geochemistrypi-0.5.0/.readthedocs.yaml` & `geochemistrypi-0.6.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/Dockerfile` & `geochemistrypi-0.6.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/.github/workflows/geochemistrypi.yml` & `geochemistrypi-0.6.0/.github/workflows/geochemistrypi.yml`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/docs/Geochemistry π.ico` & `geochemistrypi-0.6.0/docs/Geochemistry π.ico`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/docs/Geochemistry π.png` & `geochemistrypi-0.6.0/docs/Geochemistry π.png`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/docs/Geochemistryπ-Activity Diagram_v1.png` & `geochemistrypi-0.6.0/docs/Geochemistryπ-Activity Diagram_v1.png`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/docs/Makefile` & `geochemistrypi-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/docs/make.bat` & `geochemistrypi-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/docs/source/conf.py` & `geochemistrypi-0.6.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/docs/source/index.rst` & `geochemistrypi-0.6.0/docs/source/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -26,16 +26,15 @@
 
 .. toctree::
    :maxdepth: 3
    :caption: For Developer
 
    Developer Guide <For Developer/Developer Guide/Developer Manual.md>
    Contributing <contributing.rst>
-   Local Deployment <For Developer/Local Deployment.md>
-   Docker Deployment <For Developer/Docker Deployment.md>
+   Deployment <deployment.rst>
    Complete Pull Request <For Developer/A Completed Pull Request.md>
    Add New Model To Framework <For Developer/Add New Model To Framework.md>
    Docs Link <For Developer/Developer Docs link.md>
 
 Indices and tables
 ==================
```

### Comparing `geochemistrypi-0.5.0/docs/source/For Developer/A Completed Pull Request.md` & `geochemistrypi-0.6.0/docs/source/For Developer/A Completed Pull Request.md`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/docs/source/For Developer/Add New Model To Framework.md` & `geochemistrypi-0.6.0/docs/source/For Developer/Add New Model To Framework.md`

 * *Files 27% similar despite different names*

```diff
@@ -3,34 +3,50 @@
 
 
 
 
 ## Table of Contents
 
 - [1. Understand the model](#1-understand-the-model)
+
 - [2. Add Model](#2-add-model)
   - [2.1 Add The Model Class](#21-add-the-model-class)
     - [2.1.1 Find Add File](#211-find-add-file)
     - [2.1.2 Define class properties and constructors, etc.](#212-define-class-properties-and-constructors-etc)
     - [2.1.3 Define manual\_hyper\_parameters](#213-define-manual_hyper_parameters)
     - [2.1.4 Define special\_components](#214-define-special_components)
+
   - [2.2 Add AutoML](#22-add-automl)
     - [2.2.1 Add AutoML code to class](#221-add-automl-code-to-class)
+
   - [2.3 Get the hyperparameter value through interactive methods](#23-get-the-hyperparameter-value-through-interactive-methods)
     - [2.3.1 Find file](#231-find-file)
     - [2.3.2 Create the .py file and add content](#232-create-the-py-file-and-add-content)
     - [2.3.3 Import in the file that defines the model class](#233-import-in-the-file-that-defines-the-model-class)
+
   - [2.4 Call Model](#24-call-model)
     - [2.4.1 Find file](#241-find-file)
     - [2.4.2 Import module](#242-import-module)
     - [2.4.3 Call model](#243-call-model)
+
   - [2.5 Add the algorithm list and set NON\_AUTOML\_MODELS](#25-add-the-algorithm-list-and-set-non_automl_models)
     - [2.5.1 Find file](#251-find-file)
+
+  -  [2.6 Add Functionality](#26-add-functionality)
+
+      - [2.6.1 Model Research](#261-model-research)
+
+     - [2.6.2 Add Common_component](#262-add-common_component)
+
+      - [2.6.3 Add Special_component](#263-add-special_component)
+
 - [3. Test model](#3-test-model)
+
 - [4. Completed Pull Request](#4-completed-pull-request)
+
 - [5. Precautions](#5-precautions)
 
 
 ## 1. Understand the model
 You need to understand the general meaning of the model, determine which algorithm the model belongs to and the role of each parameter.
 + You can choose to learn about the relevant knowledge on the [scikit-learn official website](https://scikit-learn.org/stable/index.html).
 
@@ -361,14 +377,298 @@
 ![image12](https://github.com/ZJUEarthData/geochemistrypi/assets/97781484/ec647037-2467-4a86-b7bb-e009a48cb964)
 
 （2）set NON_AUTOML_MODELS
 Because this is a tutorial without automatic parameters, you need to add the model name in the NON_AUTOML_MODELS.
 **eg:**
 ![image13](https://github.com/ZJUEarthData/geochemistrypi/assets/97781484/d6b03566-a833-4868-8738-be09d7356c9c)
 
+
+
+
+
+### 2.6 Add Functionality
+
+#### 2.6.1 Model Research
+
+Conduct research on the corresponding model and confirm the functions that need to be added.
+
+\+ You can confirm the functions that need to be added on the official website of the model (such as scikit learn), search engines (such as Google), chatGPT, etc.
+
+(1) Common_component is a public function in a class, and all functions in each class can be used, so they need to be added in the parent class，Each of the parent classes can call Common_component.
+
+(2) Special_component is unique to the model, so they need to be added in a specific model，Only they can use it.
+
+![Image1](https://github.com/ZJUEarthData/geochemistrypi/assets/113361635/3f983a7a-3b0d-4c7b-b7b7-31b317f4d9d0)
+
+
+
+#### 2.6.2 Add Common_component
+
+Common_component refer to functions that can be used by all internal submodels, so it is necessary to consider the situation of each submodel when adding them.
+
+***\*1. Add corresponding functionality to the parent class\****
+
+Once you've identified the features you want to add, you can define the corresponding functions in the parent class.
+
+The code format is:
+
+(1) Define the function name and add the required parameters.
+
+(2) Use annotations to describe function functionsUse annotations to describe function functions.
+
+(3) Referencing specific functions to implement functionality.
+
+(4) Change the format of data acquisition and save data or images.
+
+
+
+***\*2. Define Common_component\****
+
+(1) Define the common_components in the parent class, its role is to set where the output is saved.
+
+(2) Set the parameter source for the added function.
+
+
+
+***\*3. Implement function functions\****
+
+Some functions may use large code due to their complexity. To ensure the style and readability of the code, you need to put the specific function implementation into the corresponding `_common` files and call it.
+
+It includes:
+
+(1) Explain the significance of each parameter.
+
+(2) Implement functionality.
+
+(3) Returns the required parameters.
+
+
+
+***\*eg:\**** You want to add model evaluation to your clustering.
+
+First, you need to find the parent class to clustering.
+
+![Image2](https://github.com/ZJUEarthData/geochemistrypi/assets/113361635/b41a5af8-6cf3-4747-8c83-e613a3fee04b)
+
+![Image3](https://github.com/ZJUEarthData/geochemistrypi/assets/113361635/e81f3c96-f90d-49c8-b2e9-e8675d41cf90)
+
+***\*1. Add the clustering score function in class ClusteringWorkflowBase (WorkflowBase).\****
+
+
+```python
+
+@staticmethod
+def _score(data: pd.DataFrame, labels: pd.DataFrame, algorithm_name: str, store_path: str) -> None:
+
+    """Calculate the score of the model."""
+
+    print("-----* Model Score *-----")
+
+    scores = score(data, labels)
+
+    scores_str = json.dumps(scores, indent=4)
+
+    save_text(scores_str, f"Model Score - {algorithm_name}", store_path)
+
+    mlflow.log_metrics(scores)
+
+```
+
+
+(1) Define the function name and add the required parameters.
+
+(2) Use annotations to describe function functionsUse annotations to describe function functions.
+
+(3) Referencing specific functions to implement functionality (Reference 3.2.3).
+
+(4) Change the format of data acquisition and save data or images.
+
+***\*Note:\**** Make sure that the code style of the added function is consistent.
+
+***\*2. Define common_components below the added function to define the output position and parameter source for the added function.\****
+
+```python
+
+def common_components(self) -> None:
+
+    """Invoke all common application functions for clustering algorithms."""
+
+    GEOPI_OUTPUT_METRICS_PATH = os.getenv("GEOPI_OUTPUT_METRICS_PATH")
+
+    GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH")
+
+    self._score(
+
+      data=self.X,
+
+      labels=self.clustering_result["clustering result"],
+
+      algorithm_name=self.naming,
+
+      store_path=GEOPI_OUTPUT_METRICS_PATH,
+
+    )
+
+```
+
+The positional relationship is shown in Figure 4.
+
+![Image4](https://github.com/ZJUEarthData/geochemistrypi/assets/113361635/5e3eac82-19f8-4ef3-87a6-701ce6f9ac1b)
+
+***\*3. You need to add the specific function implementation to the corresponding `_commom` file.\****
+
+![Image5](https://github.com/ZJUEarthData/geochemistrypi/assets/113361635/ee6bb43e-f30e-47b6-8d78-13f017994a44)
+
+```python
+
+def score(data: pd.DataFrame, labels: pd.DataFrame) -> Dict:
+
+    """Calculate the scores of the clustering model.
+
+      Parameters
+
+      ----------
+
+      data : pd.DataFrame (n_samples, n_components)
+
+        The true values.
+
+      labels : pd.DataFrame (n_samples, n_components)
+
+        Labels of each point.
+
+      Returns
+
+      -------
+
+      scores : dict
+
+        The scores of the clustering model.
+
+    """
+
+    silhouette = silhouette_score(data, labels)
+
+    calinski_harabaz = calinski_harabasz_score(data, labels)
+
+    print("silhouette_score: ", silhouette)
+
+    print("calinski_harabasz_score:", calinski_harabaz)
+
+    scores = {
+
+        "silhouette_score": silhouette,
+
+        "calinski_harabasz_score": calinski_harabaz,
+
+    }
+
+    return scores
+
+```
+
+(1) Explain the significance of each parameter.
+
+(2) Implement functionality.
+
+(3) Returns the required parameters.
+
+
+
+#### 2.6.3 Add Special_component
+
+Special_components is a feature that is unique to each specific model.
+
+The process of adding a Special_components is similar to that of a Common_component.
+
+
+
+The process is as follows:
+
+(1) Find the location that needs to be added.
+
+(2) Defined function.
+
+(3) Define Special_components and add a parametric function to it.
+
+(4) Add the corresponding specific function implementation function to the `corresponding manual parameter tuning` file.
+
+
+
+***\*eg:\**** An example is to add a score evaluation function to k-means clustering.
+
+***\*1. Find the location that needs to be added.\****
+
+We add his own unique score to the k-means.
+
+![Image2](https://github.com/ZJUEarthData/geochemistrypi/assets/113361635/b41a5af8-6cf3-4747-8c83-e613a3fee04b)
+
+![Image6](https://github.com/ZJUEarthData/geochemistrypi/assets/113361635/34f1b0f8-9809-4ba6-86d5-aa28a565abc9)
+
+***\*2. Defined function.\****
+
+```python
+
+def _get_inertia_scores(self, algorithm_name: str, store_path: str) -> None:
+
+    """Get the scores of the clustering result."""
+
+    print("-----* KMeans Inertia Scores *-----")
+
+    print("Inertia Score: ", self.model.inertia_)
+
+    inertia_scores = {"Inertia Score": self.model.inertia_}
+
+    mlflow.log_metrics(inertia_scores)
+
+    inertia_scores_str = json.dumps(inertia_scores, indent=4)
+
+    save_text(inertia_scores_str, f"KMeans Inertia Scores - {algorithm_name}", store_path)
+
+```
+
+(1) Define the function name and add the required parameters.
+
+(2) Use annotations to describe function functionsUse annotations to describe function functions.
+
+(3) Referencing specific functions to implement functionality.
+
+(4) Change the format of data acquisition and save data or images.
+
+***\*3. Define Special_components and add a parametric function to it.\****
+
+
+```python
+
+def special_components(self, **kwargs: Union[Dict, np.ndarray, int]) -> None:
+
+	  """Invoke all special application functions for this algorithms by Scikit-learn framework."""
+
+	   GEOPI_OUTPUT_METRICS_PATH = os.getenv("GEOPI_OUTPUT_METRICS_PATH")
+
+	   self._get_inertia_scores(
+
+	   algorithm_name=self.naming,
+
+	   store_path=GEOPI_OUTPUT_METRICS_PATH,
+
+	 )
+
+```
+
+The positional relationship is shown in Figure 7.
+
+![Image7](https://github.com/ZJUEarthData/geochemistrypi/assets/113361635/18dec84b-44ae-4883-a5b8-db2c6e0ef5c8)
+
+***\*4. Add the corresponding specific function implementation function to the `corresponding manual parameter tuning` file.\****
+
+If the defined function has complex functions, it is necessary to further improve its function content in the manual parameter file, and the code format should refer to Common_component.
+
+![Image](https://github.com/ZJUEarthData/geochemistrypi/assets/113361635/a3ea82c2-9c20-49f4-bf3e-354b012aff7c)
+
 ## 3. Test model
 After the model is added, it can be tested. If the test reports an error, it needs to be checked. If there is no error, it can be submitted.
 
 ## 4. Completed Pull Request
 After the model test is correct, you can complete the pull request according to the puu document instructions in [Geochemistry π](https://geochemistrypi.readthedocs.io/en/latest/index.html)
 ![image](https://github.com/ZJUEarthData/geochemistrypi/assets/97781484/e95c2e44-21f7-44af-8e32-e857189a5204)
```

### Comparing `geochemistrypi-0.5.0/docs/source/For Developer/Developer Docs link.md` & `geochemistrypi-0.6.0/docs/source/For Developer/Developer Docs link.md`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/docs/source/For Developer/Docker Deployment.md` & `geochemistrypi-0.6.0/docs/source/For Developer/Deployment/Docker Deployment.md`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/docs/source/For Developer/Local Deployment.md` & `geochemistrypi-0.6.0/docs/source/For Developer/Deployment/Local Deployment.md`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/docs/source/For Developer/Contributing/Code_of_Conduct.md` & `geochemistrypi-0.6.0/docs/source/For Developer/Contributing/Code_of_Conduct.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Code of Conduct
+# Code of Conduct
 
 Contents：
 
 1. Naming Conventions
 2. Space Usage
 3. Variable Type Hint
 4. TODO or FIXME Comments
```

### Comparing `geochemistrypi-0.5.0/docs/source/For Developer/Contributing/Contributor.md` & `geochemistrypi-0.6.0/docs/source/For Developer/Contributing/Contributor.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Contributors
+
 ## Leader:
 + Can He (Sany, National University of Singapore, Singapore)
   Email: sanyhew1097618435@163.com
 
 ## Technical Group:
 + Jianming Zhao (Jamie, Jilin University, Changchun, China)
 + Jianhao Sun (Jin, China University of Geosciences, Wuhan, China)
```

### Comparing `geochemistrypi-0.5.0/docs/source/For Developer/Developer Guide/Developer Manual.md` & `geochemistrypi-0.6.0/docs/source/For Developer/Developer Guide/Developer Manual.md`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/docs/source/For User/Installation Manual.md` & `geochemistrypi-0.6.0/docs/source/For User/Installation Manual.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,162 +1,323 @@
-<p style="text-align: center; font-size: 38px; font-weight: bold;">
-Installation Manual
-</p>
+# Installation Manual
 
 #### Contents
 
 1. [Preparation](#Preparation)
+
 2. [Download Geochemistry π](#Download-Geichemistry—π)
+
 3. [Solutions and Suggestions for Installation Failure](#Solutions)
 
 
+
+
+
 ## 1. Preparation <a name="Preparation"> </a>
 
+
+
 ### 1.1 Install Python Interpreter
 
-A Python interpreter is a program that reads and executes Python code. When you write Python code in a text file with a `.py` extension, you can run that file using the Python interpreter.  For example, use `python main.py` to executes the codes inside main.py file in command line or terminal.
+
+
+A Python interpreter is a program that reads and executes Python code. When you write Python code in a text file with a `.py` extension, you can run that file using the Python interpreter. For example, use `python main.py` to executes the codes inside main.py file in command line or terminal.
+
+
 
 The normal ways to install Python interpreter:
 
+
+
 (1) If you are a Windows user, you can use Microsoft Store App to download directly by searching Python.
 
+
+
 (2) Refer to the download section in [Python official documentation](https://www.python.org).
 
+
+
 (3) If you are Chinese users, you can refer to this blog [Python Download - RUNOOB](https://www.runoob.com/python/python-install.html) to download too.
 
-### 1.2  Install Conda
 
-Conda allows you to easily install, update, and manage Python packages and dependencies. Usually,  Conda is included the software Anaconda. Hence, by downloading Anaconda, you can install Conda too.
+
+### 1.2 Install Conda
+
+
+
+Conda allows you to easily install, update, and manage Python packages and dependencies. Usually, Conda is included the software Anaconda. Hence, by downloading Anaconda, you can install Conda too.
+
+
 
 The normal ways to install Anaconda:
 
+
+
 (1) Refer to the download section in [Anaconda website](https://www.anaconda.com).
 
+
+
 (2) If you are Chinese users, you can refer to [Anaconda Download - Zhihu](https://zhuanlan.zhihu.com/p/459601766) to download Anaconda using Tsinghua mirror source Anaconda. Also, if you are not familiar with Command Prompt (CMD) in Windows, you can reference to [Frequently Used Commands on Windows - Zhihu](https://zhuanlan.zhihu.com/p/67513308).
 
 
+
+
+
 ## 2. Download Geochemistry π in Virtual Environment <a name="Download-Geichemistry—π"> </a>
 
+
+
 ### 2.1 Create A Virtual Environment
 
+
+
 Use Conda to manage virtual environments (recommended) :
 
+
+
 (1) Creates a virtual environment by installing the python interpreter, for example, to install a version 3.9 python interpreter, where `env_name` is the name of the created environment. To avoid version problems, it is better to use 3.9 version of python.
 
+
+
 On Mac Terminal:
 
+
+
 ```
+
 conda create -n vir_env_name python=3.9
+
 ```
 
+
+
 On Windows Command Prompt:
 
+
+
 ```
+
 conda create -n vir_env_name python=3.9
+
 ```
 
+***\*Note:\****
+
+1. In the command, 'vir_env_name' can be replaced by any name you want, like 'Geochemical_project'. Remember it's better not using Chinese characters.
+
+2. Please remember that our project are stable in 'python=3.9'. Other versions would make unkown mistakes.
+
+3. When meeting problems in the installation. Please check the python version first.
+
+
+
 For the prompting information, input `y` to continue until the configuration is done.
 
+
+
 (2) Activate the created virtual environment.
 
+
+
 On Mac Terminal:
 
+
+
 ```
+
 conda activate vir_env_name
+
 ```
 
+
+
 On Windows Command Prompt:
 
+
+
 ```
+
 conda activate vir_env_name
+
 ```
 
-For more useful Conda commands,  please search online.
+
+
+For more useful Conda commands, please search online.
+
+
 
 ### 2.2 Use pip to Download
 
+
+
 After the virtual environment is activated on your computer, you can follow the steps below to download our software:
 
+
+
 (1) Clear the cache packages:
 
+
+
 On Mac Terminal:
 
+
+
 ```
+
 pip cache purge
+
 ```
 
+
+
 On Windows Command Prompt:
 
+
+
 ```
+
 pip cache purge
+
 ```
 
+
+
 (2) Download our software:
 
+
+
 On Mac Terminal:
 
+
+
 ```
+
 pip install geochemistrypi
+
 ```
 
+
+
 On Windows Command Prompt:
 
+
+
 ```
+
 pip install geochemistrypi
+
 ```
 
+
+
 (3) Check the latest version of our software:
 
+
+
 On Mac Terminal:
 
+
+
 ```
+
 geochemistrypi --version
+
 ```
 
+
+
 On Windows Command Prompt:
 
+
+
 ```
+
 geochemistrypi --version
+
 ```
 
-**Note**: Domestic direct installation may stop because of network speed problems in ray or Fiona package installation failure. You can reference the following video to resolve the problem.
+
+
+***\*Note\****: Domestic direct installation may stop because of network speed problems in ray or Fiona package installation failure. You can reference the following video to resolve the problem.
+
+
 
 + [Possible Scenarios When Installing via pip Directly in China.mp4](https://www.bilibili.com/video/BV1Gs4y1d7Cm/?spm_id_from=333.999.0.0&vd_source=350db2ec0e0c3ee7f424928a21e82674)
 
 
+
+
+
 ## 3. Solutions and Suggestions for Installation Failure <a name="Solutions"> </a>
 
+
+
 ### 3.1 Use Tsinghua Mirror Source
 
+
+
 If you cannot download our software because Ray/Fiona downloads are too slow or just fail , you can use the pip with Tsinghua mirror source to re-download the package in terms of the specific error.
+
 ```
+
 pip install ray -i https://pypi.tuna.tsinghua.edu.cn/simple
+
 ```
+
 + Reference video: [Solutions to Failures in Direct pip Installation in China.mp4](https://www.bilibili.com/video/BV1zg4y1j7bx/?spm_id_from=333.999.0.0&vd_source=350db2ec0e0c3ee7f424928a21e82674).
 
+
+
 ### 3.2 Use 'pip install -r requirements/production.txt'
 
+
+
 Another way to download related dependecies is to clone the source code from GitHub or Gitee repository firstly:
 
+
+
 GitHub Link: https://github.com/ZJUEarthData/geochemistrypi
 
+
+
 Gitee Link: https://gitee.com/zju-earth-data/geochemistrypi
 
-After that, unpacking the source code file. Open Terminal on Mac or Command Promt on Window and navigate to the directory to the source code file, use the following command to download the dependency  :
+
+
+After that, unpacking the source code file. Open Terminal on Mac or Command Promt on Window and navigate to the directory to the source code file, use the following command to download the dependency :
+
+
 
 ```
+
 pip install -r requirements/production.txt
+
 ```
 
+
+
 Or use the Tsinghua mirror source to download:
 
+
+
 ```
+
 pip install -r requirements/production.txt -i https://pypi.tuna.tsinghua.edu.cn/simple
+
 ```
 
-+ Reference video:  [The Fastest Currently Feasible Installation Method in China—Installing from GitHub Using requirements.mp4](https://www.bilibili.com/video/BV1pM411V7iR/?spm_id_from=333.999.0.0&vd_source=350db2ec0e0c3ee7f424928a21e82674)
 
-**Note**: Actually this method can be used for developers to test our latest updates. For more information, please refer to our online documentation in **Local Deployment** under the section of **FOR DEVELOPER**.
+
++ Reference video: [The Fastest Currently Feasible Installation Method in China—Installing from GitHub Using requirements.mp4](https://www.bilibili.com/video/BV1pM411V7iR/?spm_id_from=333.999.0.0&vd_source=350db2ec0e0c3ee7f424928a21e82674)
+
+
+
+***\*Note\****: Actually this method can be used for developers to test our latest updates. For more information, please refer to our online documentation in ***\*Local Deployment\**** under the section of ***\*FOR DEVELOPER\****.
+
+
 
 ### 3.3 Report An Error to Our Team
 
-You can refer to our online documentation in **Contact Us** under the section of **FOR USER**.
+
+
+You can refer to our online documentation in ***\*Contact Us\**** under the section of ****FOR USER****.
```

### Comparing `geochemistrypi-0.5.0/docs/source/For User/User Docs link.md` & `geochemistrypi-0.6.0/docs/source/For User/User Docs link.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## User Documents Link
+# User Documents Link
 
 ### 1. Geochemistry π Project Introduction
 
 + [Project Introduction](https://geochemistrypi.readthedocs.io/en/latest/Introduction/Introduction.html)
 
 ### 2. Code Download Link
 + [Github link](https://github.com/ZJUEarthData/geochemistrypi)
```

### Comparing `geochemistrypi-0.5.0/docs/source/For User/User Guide.md` & `geochemistrypi-0.6.0/docs/source/For User/User Guide.md`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,23 @@
 6. [How to use pickle and joblib](#joblib)
 7. [Advice](#advice)
 
 
 ## 1. Installation <a name="installation"> </a>
 
 Requirements: Python 3.9
+
+The normal ways to install Python Python 3.9:
+
+(1) If you are a Windows user, you can use Microsoft Store App to download directly by searching Python.
+
+(2) Refer to the download section in [Python official documentation](https://www.python.org).
+
+(3) If you are Chinese users, you can refer to this blog [Python Download - RUNOOB](https://www.runoob.com/python/python-install.html) to download too.
+
 **Note**:You must have Python 3.9 installed on your computer to use the software.
 
 ### 1.1 Check Environment
 
 You need to ensure that pip is installed.
 You can view it by typing instructions on the command line.
```

### Comparing `geochemistrypi-0.5.0/docs/source/For User/Contact us/Join us.md` & `geochemistrypi-0.6.0/docs/source/For User/Contact us/Join us.md`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/docs/source/For User/Contact us/bug_report.md` & `geochemistrypi-0.6.0/docs/source/For User/Contact us/bug_report.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## Bug Reports
+# Bug Reports
 
 If you find <font color=pink>Geochemistry Py</font> does not work well with you, in the meantime, googling error messages cannot help. Please check the Q&A first to see if similar questions have already been posted, and there may already be valid comments. If not, please contact us and send the details of bug. Our experts are willing to solve the problems for you as soon as we can. Here is a toturial posted on Youtube [“Geochemistry π-How to use Github for collaboration and Bug reporting-Sany”](https://www.youtube.com/watch?v=1DWoEsqsfvQ&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM&index=4).
 
 **Ways to report other bugs** (downloading or running the software):
 
 1. Contact Sany (Email: sanyhew1097618435@163.com) with the title as "Bug: Geochemistry Pi".
 2. Open our GitHub issue (channel: ZJUEarthData) and follow the [template](https://github.com/ZJUEarthData/geochemistrypi/issues/26) to detail the problem.
```

### Comparing `geochemistrypi-0.5.0/docs/source/For User/Contact us/bug_template.md` & `geochemistrypi-0.6.0/docs/source/For User/Contact us/bug_template.md`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/docs/source/For User/Model Example/Decomposition/decomposition.md` & `geochemistrypi-0.6.0/docs/source/For User/Model Example/Decomposition/decomposition.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 # Decomposition
 
+## Table of Contents
 
-## T-distributed Stochastic Neighbor Embedding （T-SNE）
-
-
-
-### Table of Contents
-
-- [Table of Contents](#table-of-contents)
 - [1. t-distributed Stochastic Neighbor Embedding (T-SNE)](#1-t-distributed-stochastic-neighbor-embedding-t-sne)
 - [2. Preparation](#2-preparation)
 - [3. NAN value process](#3-nan-value-process)
 - [4. Feature engineering](#4-feature-engineering)
 - [5. Model Selection](#5-model-selection)
 - [6. T-SNE](#6-t-sne)
 
-### 1. T-distributed Stochastic Neighbor Embedding (T-SNE)
+## 1. T-distributed Stochastic Neighbor Embedding (T-SNE)
 
 **t-distributed Stochastic Neighbor Embedding** is usually known as T-SNE. T-SNE is an unsupervised learning method, in which the training data we feed to the algorithm does not need the desired labels. T-SNE is a machine learning algorithm used for dimensionality reduction and visualization of high-dimensional data.
 It represents the similarity between data points in the high-dimensional space using a Gaussian distribution, creating a probability distribution by measuring this similarity. In the low-dimensional space, T-SNE reconstructs this similarity distribution using the t-distribution. T-SNE aims to preserve the local relationships between data points, ensuring that similar points in the high-dimensional space remain similar in the low-dimensional space.
 
 **Note:**  This part would show the whole process of T-SNE, including data-processing and model-running.
 
-### 2. Preparation
+## 2. Preparation
 
 First, after ensuring the Geochemistry Pi framework has been installed successfully (if not, please see docs ), we run the python framework in command line interface to process our program: If you do not input own data, you can run:
 
 ```
 geochemistrypi data-mining
 ```
 
@@ -172,15 +166,15 @@
 Successfully draw the distribution plot after log transformation of the selected columns.
 Save figure 'Distribution Histogram After Log Transformation' in  dir.
 Successfully store 'Distribution Histogram After Log Transformation' in 'Distribution Histogram After Log Transformation.xlsx' in dir.
 Successfully store 'Data Original' in 'Data Original.xlsx' in  dir.
 Successfully store 'Data Selected' in 'Data Selected.xlsx' in  dir.
 ```
 
-### 3. NAN value process
+## 3. NAN value process
 
 Check the NAN values would be helpful for later analysis. In Geochemistry π frame, this option is finished automatically.
 
 ```
 -*-*- Imputation -*-*-
 Check which column has null values:
 --------------------
@@ -267,15 +261,15 @@
 25%      3.110977    0.680000    2.350000   20.310000   15.300000    0.063075
 50%      4.720000    0.956426    2.690000   21.223500   15.920000    0.090000
 75%      6.233341    1.170000    3.330000   22.185450   16.816000    0.110000
 max      8.110000    3.869550    8.145000   25.362000   23.528382    0.400000
 Successfully store 'Data Selected Imputed' in 'Data Selected Imputed.xlsx' in dir.
 ```
 
-### 4. Feature engineering
+## 4. Feature engineering
 
 The next step is the feature engineering options.
 
 ```python
 -*-*- Feature Engineering -*-*-
 The Selected Data Set:
 --------------------
@@ -407,15 +401,15 @@
 1 - Yes
 2 - No
 (Data) ➜ @Number: 2
 Successfully store 'Data Selected Imputed Feature-Engineering' in 'Data Selected Imputed Feature-Engineering.xlsx' in dir.
 Exit Feature Engineering Mode.
 ```
 
-### 5. Model Selection
+## 5. Model Selection
 
 Select dimensionality reduction
 
 ```python
 -*-*- Mode Selection -*-*-
 1 - Regression
 2 - Classification
@@ -468,15 +462,15 @@
 75%    8.563927e-01  4.089238e-01  3.257487e-01  5.470608e-01  4.472813e-01  3.332377e-01
 max    1.813530e+00  5.577677e+00  4.591518e+00  2.171605e+00  5.153439e+00  5.728214e+00
 Successfully store 'X With Scaling' in 'X With Scaling.xlsx' in dir.
 ```
 
 
 
-### 6. T-SNE
+## 6. T-SNE
 
 Select T-SNE.
 
 ```python
 -*-*- Model Selection -*-*-:
 1 - PCA
 2 - T-SNE
```

### Comparing `geochemistrypi-0.5.0/docs/source/For User/Model Example/Regression/Regression.md` & `geochemistrypi-0.6.0/docs/source/For User/Model Example/Regression/Regression.md`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/docs/source/Home/CHANGELOG.md` & `geochemistrypi-0.6.0/docs/source/Home/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 
 ## [Unreleased]
 
 + MLOps core of continuous training in web interface
 
-## [0.5.0] - 2023-01-14
+## [0.5.0] - 2024-01-14
 
 ### Added
 
 + Missing value process with three options
 + Fixed random state for all models
 + New Models:
   + Regression Models
@@ -124,12 +124,13 @@
   + Decomposition Models
     + Principle Component Analysis
 + Build up continuous integration (CI) after git commit using Git Action
 
 
 
 [ unreleased ]: https://github.com/ZJUEarthData/geochemistrypi
+[ 0.5.0 ]: https://github.com/ZJUEarthData/geochemistrypi/compare/v0.4.0...v0.5.0
 [ 0.4.0 ]: https://github.com/ZJUEarthData/geochemistrypi/compare/v0.3.0...v0.4.0
 [ 0.3.0 ]: https://github.com/ZJUEarthData/geochemistrypi/compare/v0.2.1...v0.3.0
 [ 0.2.1 ]: https://github.com/ZJUEarthData/geochemistrypi/compare/v0.2.0...v0.2.1
 [ 0.2.0 ]: https://github.com/ZJUEarthData/geochemistrypi/compare/v0.1.0...v0.2.0
 [ 0.1.0 ]: https://github.com/ZJUEarthData/geochemistrypi/releases/tag/v0.1.0
```

### Comparing `geochemistrypi-0.5.0/docs/source/python_apis/api.rst` & `geochemistrypi-0.6.0/docs/source/python_apis/api.rst`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/docs/source/python_apis/geochemistrypi.auth.rst` & `geochemistrypi-0.6.0/docs/source/python_apis/geochemistrypi.auth.rst`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/docs/source/python_apis/geochemistrypi.data_mining.data.rst` & `geochemistrypi-0.6.0/docs/source/python_apis/geochemistrypi.data_mining.data.rst`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/docs/source/python_apis/geochemistrypi.data_mining.model.rst` & `geochemistrypi-0.6.0/docs/source/python_apis/geochemistrypi.data_mining.model.rst`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,22 @@
 ------------------------------------------------------
 
 .. automodule:: geochemistrypi.data_mining.model.decomposition
    :members:
    :undoc-members:
    :show-inheritance:
 
+geochemistrypi.data\_mining.model.detection module
+--------------------------------------------------
+
+.. automodule:: geochemistrypi.data_mining.model.detection
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 geochemistrypi.data\_mining.model.regression module
 ---------------------------------------------------
 
 .. automodule:: geochemistrypi.data_mining.model.regression
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `geochemistrypi-0.5.0/docs/source/python_apis/geochemistrypi.data_mining.plot.rst` & `geochemistrypi-0.6.0/docs/source/python_apis/geochemistrypi.data_mining.plot.rst`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/docs/source/python_apis/geochemistrypi.data_mining.process.rst` & `geochemistrypi-0.6.0/docs/source/python_apis/geochemistrypi.data_mining.process.rst`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,22 @@
 ----------------------------------------------------
 
 .. automodule:: geochemistrypi.data_mining.process.decompose
    :members:
    :undoc-members:
    :show-inheritance:
 
+geochemistrypi.data\_mining.process.detect module
+-------------------------------------------------
+
+.. automodule:: geochemistrypi.data_mining.process.detect
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 geochemistrypi.data\_mining.process.regress module
 --------------------------------------------------
 
 .. automodule:: geochemistrypi.data_mining.process.regress
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `geochemistrypi-0.5.0/docs/source/python_apis/geochemistrypi.data_mining.rst` & `geochemistrypi-0.6.0/docs/source/python_apis/geochemistrypi.data_mining.rst`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/docs/source/python_apis/geochemistrypi.data_mining.tests.test_data.rst` & `geochemistrypi-0.6.0/docs/source/python_apis/geochemistrypi.data_mining.tests.test_data.rst`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/docs/source/python_apis/geochemistrypi.data_mining.utils.rst` & `geochemistrypi-0.6.0/docs/source/python_apis/geochemistrypi.data_mining.utils.rst`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/docs/source/python_apis/geochemistrypi.rst` & `geochemistrypi-0.6.0/docs/source/python_apis/geochemistrypi.rst`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/cli.py` & `geochemistrypi-0.6.0/geochemistrypi/cli.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/database.py` & `geochemistrypi-0.6.0/geochemistrypi/database.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/start_dash_pipeline.py` & `geochemistrypi-0.6.0/geochemistrypi/start_dash_pipeline.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/auth/dependencies.py` & `geochemistrypi-0.6.0/geochemistrypi/auth/dependencies.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/auth/router.py` & `geochemistrypi-0.6.0/geochemistrypi/auth/router.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/auth/service.py` & `geochemistrypi-0.6.0/geochemistrypi/auth/service.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/auth/sql_models.py` & `geochemistrypi-0.6.0/geochemistrypi/auth/sql_models.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/auth/utils.py` & `geochemistrypi-0.6.0/geochemistrypi/auth/utils.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/cli_pipeline.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/cli_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,28 @@
 
 import mlflow
 from rich import print
 from rich.console import Console
 from rich.prompt import Confirm, Prompt
 
 from .constants import (
+    ABNORMALDETECTION_MODELS,
     CLASSIFICATION_MODELS,
     CLASSIFICATION_MODELS_WITH_MISSING_VALUES,
     CLUSTERING_MODELS,
     CLUSTERING_MODELS_WITH_MISSING_VALUES,
     DECOMPOSITION_MODELS,
+    DROP_MISSING_VALUE_STRATEGY,
     FEATURE_SCALING_STRATEGY,
     FEATURE_SELECTION_STRATEGY,
     IMPUTING_STRATEGY,
     MISSING_VALUE_STRATEGY,
     MLFLOW_ARTIFACT_DATA_PATH,
     MODE_OPTION,
+    MODE_OPTION_WITH_MISSING_VALUES,
     NON_AUTOML_MODELS,
     OPTION,
     OUTPUT_PATH,
     REGRESSION_MODELS,
     REGRESSION_MODELS_WITH_MISSING_VALUES,
     SECTION,
     TEST_DATA_OPTION,
@@ -36,16 +39,17 @@
 from .data.preprocessing import feature_scaler, feature_selector
 from .data.statistic import monte_carlo_simulator
 from .plot.map_plot import process_world_map
 from .plot.statistic_plot import basic_statistic, check_missing_value, correlation_plot, distribution_plot, is_null_value, log_distribution_plot, probability_plot, ratio_null_vs_filled
 from .process.classify import ClassificationModelSelection
 from .process.cluster import ClusteringModelSelection
 from .process.decompose import DecompositionModelSelection
+from .process.detect import AbnormalDetectionModelSelection
 from .process.regress import RegressionModelSelection
-from .utils.base import check_package, clear_output, create_geopi_output_dir, get_os, install_package, log, save_data, show_warning
+from .utils.base import check_package, clear_output, copy_files, create_geopi_output_dir, get_os, install_package, log, save_data, show_warning
 from .utils.mlflow_utils import retrieve_previous_experiment_id
 
 
 def cli_pipeline(training_data_path: str, application_data_path: Optional[str] = None) -> None:
     """The command line interface software for Geochemistry π.
     The business logic of this CLI software can be found in the figures in the README.md file.
     It provides three  MLOps core functionalities:
@@ -133,16 +137,16 @@
     # <--- Experiment Setup --->
     logger.debug("Experiment Setup")
     console.print("✨ Press [bold magenta]Ctrl + C[/bold magenta] to exit our software at any time.")
     console.print("✨ Input Template [bold magenta][Option1/Option2][/bold magenta] [bold cyan](Default Value)[/bold cyan]: Input Value")
     # Create a new experiment or use the previous experiment
     is_used_previous_experiment = Confirm.ask("✨ Use Previous Experiment", default=False)
     # Set the tracking uri to the local directory, in the future, we can set it to the remote server.
-    artifact_localtion = f"file:{WORKING_PATH}/geopi_tracking"
-    mlflow.set_tracking_uri(artifact_localtion)
+    experiments_localtion = f"file:{WORKING_PATH}/geopi_tracking"
+    mlflow.set_tracking_uri(experiments_localtion)
     # Print the tracking uri for debugging.
     # print("tracking uri:", mlflow.get_tracking_uri())
     if is_used_previous_experiment:
         # List all existing experiment names
         existing_experiments = mlflow.search_experiments()
         print("   [underline]Experiment Index: Experiment Name[/underline]")
         for idx, exp in enumerate(existing_experiments):
@@ -155,15 +159,15 @@
         mlflow.set_experiment(experiment_id=old_experiment_id)
         experiment = mlflow.get_experiment(experiment_id=old_experiment_id)
     else:
         new_experiment_name = Prompt.ask("✨ New Experiment", default="GeoPi - Rock Classification")
         # new_experiment_tag = Prompt.ask("✨ Experiment Tag Version", default="E - v1.0.0")
         try:
             # new_experiment_id = mlflow.create_experiment(name=new_experiment_name, artifact_location=artifact_localtion, tags={"version": new_experiment_tag})
-            new_experiment_id = mlflow.create_experiment(name=new_experiment_name, artifact_location=artifact_localtion)
+            new_experiment_id = mlflow.create_experiment(name=new_experiment_name)
         except mlflow.exceptions.MlflowException as e:
             if "already exists" in str(e):
                 console.print("   The experiment name already exists.", style="bold red")
                 console.print("   Use the existing experiment.", style="bold red")
                 console.print(f"   '{new_experiment_name}' is activated.", style="bold red")
                 new_experiment_id = mlflow.get_experiment_by_name(name=new_experiment_name).experiment_id
             else:
@@ -189,49 +193,53 @@
             training_data_path = "Data_Regression.xlsx"
         elif built_in_training_data_num == 2:
             training_data_path = "Data_Classification.xlsx"
         elif built_in_training_data_num == 3:
             training_data_path = "Data_Clustering.xlsx"
         elif built_in_training_data_num == 4:
             training_data_path = "Data_Decomposition.xlsx"
+        elif built_in_training_data_num == 5:
+            training_data_path = "Data_AbnormalDetection.xlsx"
         data = read_data(file_path=training_data_path)
         print(f"Successfully loading the built-in training data set '{training_data_path}'.")
         show_data_columns(data.columns)
         clear_output()
 
     # <--- Built-in Application Data Loading --->
     logger.debug("Built-in Application Data Loading")
     # If the user doesn't provide training data path and inference data path, then use the built-in inference data.
-    if is_built_in_inference_data:
-        print("-*-*- Built-in Application Data Option-*-*-")
-        num2option(TEST_DATA_OPTION)
-        built_in_inference_data_num = limit_num_input(TEST_DATA_OPTION, SECTION[0], num_input)
-        if built_in_inference_data_num == 1:
-            application_data_path = "InferenceData_Regression.xlsx"
-        elif built_in_inference_data_num == 2:
-            application_data_path = "InferenceData_Classification.xlsx"
-        elif built_in_inference_data_num == 3:
-            application_data_path = "InferenceData_Clustering.xlsx"
-        elif built_in_inference_data_num == 4:
-            application_data_path = "InferenceData_Decomposition.xlsx"
+    if is_built_in_inference_data and built_in_training_data_num == 1:
+        application_data_path = "ApplicationData_Regression.xlsx"
+        inference_data = read_data(file_path=application_data_path)
+        print(f"Successfully loading the built-in application data set '{application_data_path}'.")
+        show_data_columns(inference_data.columns)
+        clear_output()
+    elif is_built_in_inference_data and built_in_training_data_num == 2:
+        application_data_path = "ApplicationData_Classification.xlsx"
         inference_data = read_data(file_path=application_data_path)
-        print(f"Successfully loading the built-in inference data set '{application_data_path}'.")
+        print(f"Successfully loading the built-in application data set '{application_data_path}'.")
         show_data_columns(inference_data.columns)
         clear_output()
+    elif is_built_in_inference_data and built_in_training_data_num == 3:
+        inference_data = None
+    elif is_built_in_inference_data and built_in_training_data_num == 4:
+        inference_data = None
+    elif is_built_in_inference_data and built_in_training_data_num == 5:
+        inference_data = None
 
     # <--- World Map Projection --->
     logger.debug("World Map Projection")
     print("-*-*- World Map Projection -*-*-")
     process_world_map(data)
 
     # <--- Data Selection --->
     logger.debug("Data Selection")
     print("-*-*- Data Selection -*-*-")
     show_data_columns(data.columns)
-    data_selected = create_sub_data_set(data)
+    data_selected = create_sub_data_set(data, allow_empty_columns=False)
     clear_output()
     print("The Selected Data Set:")
     print(data_selected)
     clear_output()
     print("-*-*- Basic Statistical Information -*-*-")
     basic_info(data_selected)
     basic_statistic(data_selected)
@@ -265,37 +273,67 @@
     # Because dropping the rows with missing values use pandas.DataFrame.dropna() method, while imputing the missing values use sklearn.impute.SimpleImputer() method.
     drop_rows_with_missing_value_flag = False
     # clear_output()
     if missing_value_flag:
         clear_output()
         # Ask the user whether to use imputation techniques to deal with the missing values.
         print("-*-*- Missing Values Process -*-*-")
+        print("[bold red]Caution: Only some algorithms can process the data with missing value, such as XGBoost for regression and classification![/bold red]")
         print("Do you want to deal with the missing values?")
         num2option(OPTION)
         is_process_missing_value = limit_num_input(OPTION, SECTION[1], num_input)
         if is_process_missing_value == 1:
             process_missing_value_flag = True
             # If the user wants to deal with the missing values, then ask the user which strategy to use.
+            clear_output()
             print("-*-*- Strategy for Missing Values -*-*-")
             num2option(MISSING_VALUE_STRATEGY)
             print("Notice: Drop the rows with missing values may lead to a significant loss of data if too many features are chosen.")
             print("Which strategy do you want to apply?")
             missing_value_strategy_num = limit_num_input(MISSING_VALUE_STRATEGY, SECTION[1], num_input)
+            clear_output()
             if missing_value_strategy_num == 1:
-                # Drop the rows with missing values
-                data_selected_dropped = data_selected.dropna()
-                # Reset the index of the data set after dropping the rows with missing values.
-                data_selected_dropped = data_selected_dropped.reset_index(drop=True)
-                print("Successfully drop the rows with missing values.")
-                print("The Selected Data Set After Dropping:")
-                print(data_selected_dropped)
-                print("Basic Statistical Information:")
-                save_data(data_selected_dropped, "Data Selected Dropped-Imputed", GEOPI_OUTPUT_ARTIFACTS_DATA_PATH, MLFLOW_ARTIFACT_DATA_PATH)
-                drop_rows_with_missing_value_flag = True
-                imputed_flag = False
+                print("-*-*- Drop the rows with Missing Values -*-*-")
+                num2option(DROP_MISSING_VALUE_STRATEGY)
+                print("Notice: Drop the rows with missing values may lead to a significant loss of data if too many features are chosen.")
+                print("Which strategy do you want to apply?")
+                drop_missing_value_strategy_num = limit_num_input(DROP_MISSING_VALUE_STRATEGY, SECTION[1], num_input)
+                if drop_missing_value_strategy_num == 1:
+                    # Drop the rows with missing values
+                    data_selected_dropped = data_selected.dropna()
+                    # Reset the index of the data set after dropping the rows with missing values.
+                    data_selected_dropped = data_selected_dropped.reset_index(drop=True)
+                    print("Successfully drop the rows with missing values.")
+                    print("The Selected Data Set After Dropping:")
+                    print(data_selected_dropped)
+                    print("Basic Statistical Information:")
+                    save_data(data_selected_dropped, "Data Selected Dropped-Imputed", GEOPI_OUTPUT_ARTIFACTS_DATA_PATH, MLFLOW_ARTIFACT_DATA_PATH)
+                    drop_rows_with_missing_value_flag = True
+                    imputed_flag = False
+                elif drop_missing_value_strategy_num == 2:
+                    is_null_value(data_selected)
+                    show_data_columns(data_selected.columns)
+                    print("Note: The data set schema will remain the same after dropping the rows with missing values by specific columns.")
+                    drop_data_selected = create_sub_data_set(data_selected)
+                    data_selected_dropped = data_selected
+                    for column_name in drop_data_selected.columns:
+                        # Drop the rows with missing values
+                        data_selected_dropped = data_selected_dropped.dropna(subset=[column_name])
+                        # Reset the index of the data set after dropping the rows with missing values.
+                        data_selected_dropped = data_selected_dropped.reset_index(drop=True)
+                    print("Successfully drop the rows with missing values.")
+                    print("The Selected Data Set After Dropping:")
+                    print(data_selected_dropped)
+                    print("Basic Statistical Information:")
+                    save_data(data_selected_dropped, "Data Selected Dropped-Imputed", GEOPI_OUTPUT_ARTIFACTS_DATA_PATH, MLFLOW_ARTIFACT_DATA_PATH)
+                    drop_rows_with_missing_value_flag = True
+                    imputed_flag = False
+                    missing_value_flag = check_missing_value(data_selected_dropped)
+                    if missing_value_flag:
+                        process_missing_value_flag = False
             elif missing_value_strategy_num == 2:
                 # Don't drop the rows with missing values but use imputation techniques to deal with the missing values later.
                 # No need to save the data set here because it will be saved after imputation.
                 imputed_flag = True
             clear_output()
         else:
             # Don't deal with the missing values, which means neither drop the rows with missing values nor use imputation techniques.
@@ -361,18 +399,17 @@
     # Because finally, the data is complete.
     # 1. missing value flag = True, process_missing_value_flag = True, drop rows with missing values flag = True, imputed flag = False
     # 2. missing value flag = True, process_missing_value_flag = True, drop rows with missing values flag = False, imputed flag = True
     # 3. missing value flag = False, process_missing_value_flag = False, drop rows with missing values flag = False, imputed flag = False
     # If the selected data set is with missing values and is not been imputed, then only allow the user to choose regression, classification and clustering models.
     # Otherwise, allow the user to choose decomposition models.
     if missing_value_flag and not process_missing_value_flag:
-        # Delete the decomposition mode because it doesn't support missing values.
-        MODE_OPTION.remove("Dimensional Reduction")
-        num2option(MODE_OPTION)
-        mode_num = limit_num_input(MODE_OPTION, SECTION[2], num_input)
+        # The abnormal detection mode and decomposition mode don't support missing values.
+        num2option(MODE_OPTION_WITH_MISSING_VALUES)
+        mode_num = limit_num_input(MODE_OPTION_WITH_MISSING_VALUES, SECTION[2], num_input)
     else:
         num2option(MODE_OPTION)
         mode_num = limit_num_input(MODE_OPTION, SECTION[2], num_input)
     clear_output()
 
     # <--- Data Segmentation --->
     # divide X and y data set when it is supervised learning
@@ -381,15 +418,15 @@
         # Supervised learning
         print("-*-*- Data Segmentation - X Set and Y Set -*-*-")
         print("Divide the processing data set into X (feature value) and Y (target value) respectively.")
         # create X data set
         print("Selected sub data set to create X data set:")
         show_data_columns(data_selected_imputed_fe.columns)
         print("The selected X data set:")
-        X = create_sub_data_set(data_selected_imputed_fe)
+        X = create_sub_data_set(data_selected_imputed_fe, allow_empty_columns=False)
         print("Successfully create X data set.")
         print("The Selected Data Set:")
         print(X)
         print("Basic Statistical Information: ")
         basic_statistic(X)
         save_data(X, "X Without Scaling", GEOPI_OUTPUT_ARTIFACTS_DATA_PATH, MLFLOW_ARTIFACT_DATA_PATH)
         clear_output()
@@ -397,15 +434,15 @@
         # Create Y data set
         print("-*-*- Data Segmentation - X Set and Y Set-*-*-")
         print("Selected sub data set to create Y data set:")
         show_data_columns(data_selected_imputed_fe.columns)
         print("The selected Y data set:")
         print("Notice: Normally, please choose only one column to be tag column Y, not multiple columns.")
         print("Notice: For classification model training, please choose the label column which has distinctive integers.")
-        y = create_sub_data_set(data_selected_imputed_fe)
+        y = create_sub_data_set(data_selected_imputed_fe, allow_empty_columns=False)
         print("Successfully create Y data set.")
         print("The Selected Data Set:")
         print(y)
         print("Basic Statistical Information: ")
         basic_statistic(y)
         save_data(y, "Y", GEOPI_OUTPUT_ARTIFACTS_DATA_PATH, MLFLOW_ARTIFACT_DATA_PATH)
         clear_output()
@@ -504,20 +541,21 @@
     # 3. missing value flag = False, process_missing_value_flag = False, drop rows with missing values flag = False, imputed flag = False
     # If the selected data set is with missing values and is not been imputed, then only allow the user to choose regression, classification and clustering models.
     # Otherwise, allow the user to choose decomposition models.
     if missing_value_flag and not process_missing_value_flag:
         Modes2Models = {1: REGRESSION_MODELS_WITH_MISSING_VALUES, 2: CLASSIFICATION_MODELS_WITH_MISSING_VALUES, 3: CLUSTERING_MODELS_WITH_MISSING_VALUES}
         Modes2Initiators = {1: RegressionModelSelection, 2: ClassificationModelSelection, 3: ClusteringModelSelection}
     else:
-        Modes2Models = {1: REGRESSION_MODELS, 2: CLASSIFICATION_MODELS, 3: CLUSTERING_MODELS, 4: DECOMPOSITION_MODELS}
+        Modes2Models = {1: REGRESSION_MODELS, 2: CLASSIFICATION_MODELS, 3: CLUSTERING_MODELS, 4: DECOMPOSITION_MODELS, 5: ABNORMALDETECTION_MODELS}
         Modes2Initiators = {
             1: RegressionModelSelection,
             2: ClassificationModelSelection,
             3: ClusteringModelSelection,
             4: DecompositionModelSelection,
+            5: AbnormalDetectionModelSelection,
         }
     MODELS = Modes2Models[mode_num]
     num2option(MODELS)
     # Add the option of all models
     all_models_num = len(MODELS) + 1
     print(str(all_models_num) + " - All models above to be trained")
     print("Which model do you want to apply?(Enter the Corresponding Number)")
@@ -641,8 +679,16 @@
                     if drop_rows_with_missing_value_flag:
                         inference_data_fe_selected_dropped = inference_data_fe_selected.dropna()
                         model_inference(inference_data_fe_selected_dropped, is_inference, run, transformer_config, transform_pipeline)
                         save_data(inference_data_fe_selected_dropped, "Application Data Feature-Engineering Selected Dropped-Imputed", GEOPI_OUTPUT_ARTIFACTS_DATA_PATH, MLFLOW_ARTIFACT_DATA_PATH)
                     else:
                         model_inference(inference_data_fe_selected, is_inference, run, transformer_config, transform_pipeline)
                     clear_output()
+
+    # <--- Data Dumping --->
+    # In this section, convert the data in the output to the summary.
+    GEOPI_OUTPUT_SUMMARY_PATH = os.getenv("GEOPI_OUTPUT_SUMMARY_PATH")
+    GEOPI_OUTPUT_ARTIFACTS_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_PATH")
+    GEOPI_OUTPUT_METRICS_PATH = os.getenv("GEOPI_OUTPUT_METRICS_PATH")
+    GEOPI_OUTPUT_PARAMETERS_PATH = os.getenv("GEOPI_OUTPUT_PARAMETERS_PATH")
+    copy_files(GEOPI_OUTPUT_ARTIFACTS_PATH, GEOPI_OUTPUT_METRICS_PATH, GEOPI_OUTPUT_PARAMETERS_PATH, GEOPI_OUTPUT_SUMMARY_PATH)
     mlflow.end_run()
```

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/constants.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,16 +22,17 @@
 MLFLOW_ARTIFACT_IMAGE_MAP_PATH = os.path.join("image", "map")
 
 # Tell which section the user is currently in on the UML
 SECTION = ["User", "Data", "Model", "Plot"]
 
 OPTION = ["Yes", "No"]
 DATA_OPTION = ["Own Data", "Testing Data (Built-in)"]
-TEST_DATA_OPTION = ["Data For Regression", "Data For Classification", "Data For Clustering", "Data For Dimensional Reduction"]
-MODE_OPTION = ["Regression", "Classification", "Clustering", "Dimensional Reduction"]
+TEST_DATA_OPTION = ["Data For Regression", "Data For Classification", "Data For Clustering", "Data For Dimensional Reduction", "Data For Abnormal Detection"]
+MODE_OPTION = ["Regression", "Classification", "Clustering", "Dimensional Reduction", "Abnormal Detection"]
+MODE_OPTION_WITH_MISSING_VALUES = ["Regression", "Classification", "Clustering"]
 
 # The model provided to use
 REGRESSION_MODELS = [
     "Linear Regression",
     "Polynomial Regression",
     "K-Nearest Neighbors",
     "Support Vector Machine",
@@ -41,14 +42,15 @@
     "Gradient Boosting",
     "XGBoost",
     "Multi-layer Perceptron",
     "Lasso Regression",
     "Elastic Net",
     "SGD Regression",
     "BayesianRidge Regression",
+    "Ridge Regression",
     # "Bagging Regression",
     # "Decision Tree",
     # Histogram-based Gradient Boosting,
 ]
 CLASSIFICATION_MODELS = [
     "Logistic Regression",
     "Support Vector Machine",
@@ -60,16 +62,17 @@
     "Gradient Boosting",
     "K-Nearest Neighbors",
     "Stochastic Gradient Descent",
     # "Bagging Classification",
     # "Decision Tree",
     # Histogram-based Gradient Boosting,
 ]
-CLUSTERING_MODELS = ["KMeans", "DBSCAN", "Agglomerative"]
+CLUSTERING_MODELS = ["KMeans", "DBSCAN", "Agglomerative", "AffinityPropagation"]
 DECOMPOSITION_MODELS = ["PCA", "T-SNE", "MDS"]
+ABNORMALDETECTION_MODELS = ["Isolation Forest"]
 
 # The model can deal with missing values
 # Reference: https://scikit-learn.org/stable/modules/impute.html#estimators-that-handle-nan-values
 REGRESSION_MODELS_WITH_MISSING_VALUES = [
     "XGBoost",
     # "Bagging Regression",
     # "Decision Tree",
@@ -99,7 +102,9 @@
 SAMPLE_BALANCE_STRATEGY = ["Over Sampling", "Under Sampling", "Oversampling and Undersampling"]
 
 CUSTOMIZE_LABEL_STRATEGY = ["Automatic Coding", "Custom Numeric Labels", "Custom Non-numeric Labels"]
 
 FEATURE_SELECTION_STRATEGY = ["Generic Univariate Select", "Select K Best"]
 
 CALCULATION_METHOD_OPTION = ["Micro", "Macro", "Weighted"]
+
+DROP_MISSING_VALUE_STRATEGY = ["Drop All Rows with Missing Values", "Drop Rows with Missing Values by Specific Columns"]
```

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/dash_pipeline.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/dash_pipeline.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/router.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/router.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/service.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/service.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/sql_models.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/sql_models.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/data/data_readiness.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/data/data_readiness.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,34 +127,37 @@
     # sort the index list
     columns_selected.sort()
     # reindex by subtracting 1 due to python list traits
     columns_selected = [columns_selected[i] - 1 for i in range(len(columns_selected))]
     return columns_selected
 
 
-def create_sub_data_set(data: pd.DataFrame) -> pd.DataFrame:
+def create_sub_data_set(data: pd.DataFrame, allow_empty_columns: bool = False) -> pd.DataFrame:
     """Create a sub data set.
 
     Parameters
     ----------
     data : pd.DataFrame
         The data set to be processed.
 
+    allow_empty_columns : bool, optional
+        Whether to include empty columns in the sub data set. The default is False.
+
     Returns
     -------
     pd.DataFrame
         The sub data set.
     """
     sub_data_set_columns_range = str(
         input(
             "Select the data range you want to process.\n"
             "Input format:\n"
             'Format 1: "[**, **]; **; [**, **]", such as "[1, 3]; 7; [10, 13]" '
             "--> you want to deal with the columns 1, 2, 3, 7, 10, 11, 12, 13 \n"
-            'Format 2: "xx", such as "7" --> you want to deal with the columns 7 \n'
+            'Format 2: "**", such as "7" --> you want to deal with the columns 7 \n'
             "@input: "
         )
     )
     while True:
         if ("【" in sub_data_set_columns_range) or ("】" in sub_data_set_columns_range):
             print("There is a problem with the format of the parentheses entered !")
             time.sleep(0.5)
@@ -238,29 +241,30 @@
             sub_data_set_columns_range = str(input("@input: "))
         else:
             data_checking = data.iloc[:, sub_data_set_columns_selected]
             for i in data_checking.columns.values:
                 df_test = pd.DataFrame(data_checking[i])
                 test_columns = df_test.columns
                 v_value = int(df_test.isnull().sum())
-                if v_value == len(df_test):
-                    print(f"Warning: The selected column {df_test.columns.values} is an empty column!")
-                    judge = True
-                elif df_test[test_columns[0]].dtype in ["int64", "float64"]:
+                if not allow_empty_columns and v_value == len(df_test):
+                    print(f"Warning: The selected column {df_test.columns.values} is an empty column! It will be automatically removed.")
+                if df_test[test_columns[0]].dtype in ["int64", "float64"]:
                     continue
                 else:
                     print(f"Warning: The data type of selected column {df_test.columns.values} is not numeric!" " Please make sure that the selected data type is numeric and re-enter.")
                     judge = True
             if judge is True:
                 sub_data_set_columns_range = str(input("@input: "))
         if judge is False:
             break
 
     # select designated column
     sub_data_set = data.iloc[:, sub_data_set_columns_selected]
+    if not allow_empty_columns:
+        sub_data_set = sub_data_set.dropna(axis=1, how="all")
     show_data_columns(sub_data_set.columns, sub_data_set_columns_selected)
     return sub_data_set
 
 
 def data_split(X: pd.DataFrame, y: Union[pd.DataFrame, pd.Series], test_size: float = 0.2) -> Dict:
     """Split arrays or matrices into random train and test subsets.
```

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/data/feature_engineering.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/data/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/data/imputation.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/data/imputation.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/data/inference.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/data/inference.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/data/preprocessing.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/data/preprocessing.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/data/statistic.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/data/statistic.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/data/dataset/Data_Clustering.xlsx` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/data/dataset/Data_Clustering.xlsx`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/data/dataset/Data_Decomposition.xlsx` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/data/dataset/Data_AbnormalDetection.xlsx`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/data/dataset/Data_Regression.xlsx` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/data/dataset/Data_Decomposition.xlsx`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/data/dataset/InferenceData_Classification.xlsx` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/data/dataset/ApplicationData_Classification.xlsx`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/data/dataset/InferenceData_Decomposition.xlsx` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/data/dataset/Data_Regression.xlsx`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/data/dataset/InferenceData_Regression.xlsx` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/data/dataset/ApplicationData_Regression.xlsx`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/_base.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,14 +198,15 @@
     def data_upload(
         X: Optional[pd.DataFrame] = None,
         y: Optional[pd.DataFrame] = None,
         X_train: Optional[pd.DataFrame] = None,
         X_test: Optional[pd.DataFrame] = None,
         y_train: Optional[pd.DataFrame] = None,
         y_test: Optional[pd.DataFrame] = None,
+        y_train_predict: Optional[pd.DataFrame] = None,
         y_test_predict: Optional[pd.DataFrame] = None,
     ) -> None:
         """This method loads the required data into the base class's attributes."""
         if X is not None:
             WorkflowBase.X = X
         if y is not None:
             WorkflowBase.y = y
@@ -215,14 +216,16 @@
             WorkflowBase.X_test = X_test
         if y_train is not None:
             WorkflowBase.y_train = y_train
         if y_test is not None:
             WorkflowBase.y_test = y_test
         if y_test_predict is not None:
             WorkflowBase.y_test_predict = y_test_predict
+        if y_train_predict is not None:
+            WorkflowBase.y_train_predict = y_train_predict
 
     @staticmethod
     def data_save(df: pd.DataFrame, df_name: str, local_path: str, mlflow_path: str, slogan: str) -> None:
         """This method saves the data into the local path and the mlflow path.
 
         Parameters
         ----------
@@ -320,18 +323,20 @@
         save_fig(f"Tree Diagram - {algorithm_name}", local_path, mlflow_path)
 
 
 class LinearWorkflowMixin:
     """Mixin class for linear models."""
 
     @staticmethod
-    def _show_formula(coef: np.ndarray, intercept: np.ndarray, features_name: np.ndarray, algorithm_name: str, local_path: str, mlflow_path: str) -> None:
+    def _show_formula(
+        coef: np.ndarray, intercept: np.ndarray, features_name: np.ndarray, algorithm_name: str, regression_classification: str, y_train: pd.DataFrame, local_path: str, mlflow_path: str
+    ) -> None:
         """Show the formula."""
         print(f"-----* {algorithm_name} Formula *-----")
-        formula = show_formula(coef, intercept, features_name)
+        formula = show_formula(coef, intercept, features_name, regression_classification, y_train)
         formula_str = json.dumps(formula, indent=4)
         save_text(formula_str, f"{algorithm_name} Formula", local_path, mlflow_path)
 
     @staticmethod
     def _plot_2d_scatter_diagram(feature_data: pd.DataFrame, target_data: pd.DataFrame, algorithm_name: str, local_path: str, mlflow_path: str) -> None:
         """Plot the 2D graph of the linear regression model."""
         print("-----* 2D Scatter Diagram *-----")
```

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/classification.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1832,14 +1832,16 @@
         """Invoke all special application functions for this algorithms by Scikit-learn framework."""
         GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH")
         GEOPI_OUTPUT_ARTIFACTS_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_PATH")
         self._show_formula(
             coef=self.model.coef_,
             intercept=self.model.intercept_,
             features_name=LogisticRegressionClassification.X.columns,
+            regression_classification="Classification",
+            y_train=LogisticRegressionClassification.y,
             algorithm_name=self.naming,
             local_path=GEOPI_OUTPUT_ARTIFACTS_PATH,
             mlflow_path="root",
         )
         self._plot_feature_importance(
             columns_name=LogisticRegressionClassification.X.columns,
             trained_model=self.model,
@@ -1853,14 +1855,16 @@
         """Invoke all special application functions for this algorithms by FLAML framework."""
         GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH")
         GEOPI_OUTPUT_ARTIFACTS_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_PATH")
         self._show_formula(
             coef=self.auto_model.coef_,
             intercept=self.auto_model.intercept_,
             features_name=LogisticRegressionClassification.X.columns,
+            regression_classification="Classification",
+            y_train=LogisticRegressionClassification.y,
             algorithm_name=self.naming,
             local_path=GEOPI_OUTPUT_ARTIFACTS_PATH,
             mlflow_path="root",
         )
         self._plot_feature_importance(
             columns_name=LogisticRegressionClassification.X.columns,
             trained_model=self.auto_model,
@@ -3346,29 +3350,33 @@
         hyper_parameters = sgd_classificaiton_manual_hyper_parameters()
         clear_output()
         return hyper_parameters
 
     @dispatch()
     def special_components(self, **kwargs) -> None:
         """Invoke all special application functions for this algorithms by Scikit-learn framework."""
-        # GEOPI_OUTPUT_ARTIFACTS_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_PATH")
-        # self._show_formula(
-        #     coef=[self.model.coef_],
-        #     intercept=self.model.intercept_,
-        #     features_name=SGDClassification.X_train.columns,
-        #     algorithm_name=self.naming,
-        #     local_path=GEOPI_OUTPUT_ARTIFACTS_PATH,
-        #     mlflow_path="root",
-        # )
+        GEOPI_OUTPUT_ARTIFACTS_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_PATH")
+        self._show_formula(
+            coef=[self.model.coef_],
+            intercept=self.model.intercept_,
+            features_name=SGDClassification.X_train.columns,
+            regression_classification="Classification",
+            y_train=SGDClassification.y,
+            algorithm_name=self.naming,
+            local_path=GEOPI_OUTPUT_ARTIFACTS_PATH,
+            mlflow_path="root",
+        )
 
     @dispatch(bool)
     def special_components(self, is_automl: bool = False, **kwargs) -> None:
         """Invoke all special application functions for this algorithms by FLAML framework."""
-        # GEOPI_OUTPUT_ARTIFACTS_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_PATH")
-        # self._show_formula(
-        #     coef=self.auto_model.coef_,
-        #     intercept=self.auto_model.intercept_,
-        #     features_name=SGDClassification.X.columns,
-        #     algorithm_name=self.naming,
-        #     local_path=GEOPI_OUTPUT_ARTIFACTS_PATH,
-        #     mlflow_path="root",
-        # )
+        GEOPI_OUTPUT_ARTIFACTS_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_PATH")
+        self._show_formula(
+            coef=self.auto_model.coef_,
+            intercept=self.auto_model.intercept_,
+            features_name=SGDClassification.X.columns,
+            regression_classification="Classification",
+            y_train=SGDClassification.y,
+            algorithm_name=self.naming,
+            local_path=GEOPI_OUTPUT_ARTIFACTS_PATH,
+            mlflow_path="root",
+        )
```

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/clustering.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/clustering.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from numpy.typing import ArrayLike
 from rich import print
 from sklearn.cluster import DBSCAN, AffinityPropagation, AgglomerativeClustering, KMeans
 
 from ..constants import MLFLOW_ARTIFACT_DATA_PATH, MLFLOW_ARTIFACT_IMAGE_MODEL_OUTPUT_PATH
 from ..utils.base import clear_output, save_data, save_fig, save_text
 from ._base import WorkflowBase
+from .func.algo_clustering._affinitypropagation import affinitypropagation_manual_hyper_parameters
 from .func.algo_clustering._agglomerative import agglomerative_manual_hyper_parameters
 from .func.algo_clustering._common import plot_silhouette_diagram, plot_silhouette_value_diagram, scatter2d, scatter3d, score
 from .func.algo_clustering._dbscan import dbscan_manual_hyper_parameters
 from .func.algo_clustering._kmeans import kmeans_manual_hyper_parameters
 
 
 class ClusteringWorkflowBase(WorkflowBase):
@@ -553,23 +554,71 @@
 
 class AffinityPropagationClustering(ClusteringWorkflowBase):
     name = "AffinityPropagation"
 
     def __init__(
         self,
         *,
-        damping=0.5,
-        max_iter=200,
-        convergence_iter=15,
-        copy=True,
-        preference=None,
-        affinity="euclidean",
-        verbose=False,
-        random_state=None,
-    ):
+        damping: float = 0.5,
+        max_iter: int = 200,
+        convergence_iter: int = 15,
+        copy: bool = True,
+        preference: Optional[Dict] = None,
+        affinity: str = "euclidean",
+        verbose: bool = False,
+        random_state: Optional[Dict] = None,
+    ) -> None:
+        """
+        Parameters
+        ----------
+        damping : float, default=0.5
+            Damping factor in the range `[0.5, 1.0)` is the extent to
+            which the current value is maintained relative to
+            incoming values (weighted 1 - damping). This in order
+            to avoid numerical oscillations when updating these
+            values (messages).
+
+        max_iter : int, default=200
+            Maximum number of iterations.
+
+        convergence_iter : int, default=15
+            Number of iterations with no change in the number
+            of estimated clusters that stops the convergence.
+
+        copy : bool, default=True
+            Make a copy of input data.
+
+        preference : array-like of shape (n_samples,) or float, default=None
+            Preferences for each point - points with larger values of
+            preferences are more likely to be chosen as exemplars. The number
+            of exemplars, ie of clusters, is influenced by the input
+            preferences value. If the preferences are not passed as arguments,
+            they will be set to the median of the input similarities.
+
+        affinity : {'euclidean', 'precomputed'}, default='euclidean'
+            Which affinity to use. At the moment 'precomputed' and
+            ``euclidean`` are supported. 'euclidean' uses the
+            negative squared euclidean distance between points.
+
+        verbose : bool, default=False
+            Whether to be verbose.
+
+        random_state : int, RandomState instance or None, default=None
+            Pseudo-random number generator to control the starting state.
+            Use an int for reproducible results across function calls.
+            See the :term:`Glossary <random_state>`.
+
+            .. versionadded:: 0.23
+                this parameter was previously hardcoded as 0.
+
+        References
+        ----------------------------------------
+        Scikit-learn API: sklearn.cluster.AffinityPropagation
+        https://scikit-learn.org/stable/modules/generated/sklearn.cluster.AffinityPropagation
+        """
 
         super().__init__()
         self.damping = damping
         self.max_iter = max_iter
         self.convergence_iter = convergence_iter
         self.copy = copy
         self.verbose = verbose
@@ -588,15 +637,24 @@
             preference=self.preference,
             affinity=self.affinity,
             verbose=self.verbose,
             random_state=self.random_state,
         )
         self.naming = AffinityPropagationClustering.name
 
-    pass
+    @classmethod
+    def manual_hyper_parameters(cls) -> Dict:
+        """Manual hyper-parameters specification."""
+        print(f"-*-*- {cls.name} - Hyper-parameters Specification -*-*-")
+        hyper_parameters = affinitypropagation_manual_hyper_parameters()
+        clear_output()
+        return hyper_parameters
+
+    def special_components(self, **kwargs: Union[Dict, np.ndarray, int]) -> None:
+        """Invoke all special application functions for this algorithms by Scikit-learn framework."""
 
 
 class MeanShiftClustering(ClusteringWorkflowBase):
     name = "MeanShift"
     pass
```

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/decomposition.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/decomposition.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,1764 +1,1928 @@
 00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 696d 706f 7274 206f  f-8 -*-.import o
-00000020: 730a 6672 6f6d 2074 7970 696e 6720 696d  s.from typing im
-00000030: 706f 7274 2044 6963 742c 204f 7074 696f  port Dict, Optio
-00000040: 6e61 6c2c 2055 6e69 6f6e 0a0a 696d 706f  nal, Union..impo
-00000050: 7274 206e 756d 7079 2061 7320 6e70 0a69  rt numpy as np.i
-00000060: 6d70 6f72 7420 7061 6e64 6173 2061 7320  mport pandas as 
-00000070: 7064 0a66 726f 6d20 7269 6368 2069 6d70  pd.from rich imp
-00000080: 6f72 7420 7072 696e 740a 6672 6f6d 2073  ort print.from s
-00000090: 6b6c 6561 726e 2e64 6563 6f6d 706f 7369  klearn.decomposi
-000000a0: 7469 6f6e 2069 6d70 6f72 7420 5043 410a  tion import PCA.
-000000b0: 6672 6f6d 2073 6b6c 6561 726e 2e6d 616e  from sklearn.man
-000000c0: 6966 6f6c 6420 696d 706f 7274 204d 4453  ifold import MDS
-000000d0: 2c20 5453 4e45 0a0a 6672 6f6d 202e 2e63  , TSNE..from ..c
-000000e0: 6f6e 7374 616e 7473 2069 6d70 6f72 7420  onstants import 
-000000f0: 4d4c 464c 4f57 5f41 5254 4946 4143 545f  MLFLOW_ARTIFACT_
-00000100: 494d 4147 455f 4d4f 4445 4c5f 4f55 5450  IMAGE_MODEL_OUTP
-00000110: 5554 5f50 4154 480a 6672 6f6d 202e 2e75  UT_PATH.from ..u
-00000120: 7469 6c73 2e62 6173 6520 696d 706f 7274  tils.base import
-00000130: 2063 6c65 6172 5f6f 7574 7075 742c 2073   clear_output, s
-00000140: 6176 655f 6461 7461 2c20 7361 7665 5f66  ave_data, save_f
-00000150: 6967 0a66 726f 6d20 2e5f 6261 7365 2069  ig.from ._base i
-00000160: 6d70 6f72 7420 576f 726b 666c 6f77 4261  mport WorkflowBa
-00000170: 7365 0a66 726f 6d20 2e66 756e 632e 616c  se.from .func.al
-00000180: 676f 5f64 6563 6f6d 706f 7369 7469 6f6e  go_decomposition
-00000190: 2e5f 6d64 7320 696d 706f 7274 206d 6473  ._mds import mds
-000001a0: 5f6d 616e 7561 6c5f 6879 7065 725f 7061  _manual_hyper_pa
-000001b0: 7261 6d65 7465 7273 0a66 726f 6d20 2e66  rameters.from .f
-000001c0: 756e 632e 616c 676f 5f64 6563 6f6d 706f  unc.algo_decompo
-000001d0: 7369 7469 6f6e 2e5f 7063 6120 696d 706f  sition._pca impo
-000001e0: 7274 2062 6970 6c6f 742c 2070 6361 5f6d  rt biplot, pca_m
-000001f0: 616e 7561 6c5f 6879 7065 725f 7061 7261  anual_hyper_para
-00000200: 6d65 7465 7273 2c20 7472 6970 6c6f 740a  meters, triplot.
-00000210: 6672 6f6d 202e 6675 6e63 2e61 6c67 6f5f  from .func.algo_
-00000220: 6465 636f 6d70 6f73 6974 696f 6e2e 5f74  decomposition._t
-00000230: 736e 6520 696d 706f 7274 2074 736e 655f  sne import tsne_
-00000240: 6d61 6e75 616c 5f68 7970 6572 5f70 6172  manual_hyper_par
-00000250: 616d 6574 6572 730a 0a0a 636c 6173 7320  ameters...class 
-00000260: 4465 636f 6d70 6f73 6974 696f 6e57 6f72  DecompositionWor
-00000270: 6b66 6c6f 7742 6173 6528 576f 726b 666c  kflowBase(Workfl
-00000280: 6f77 4261 7365 293a 0a20 2020 2022 2222  owBase):.    """
-00000290: 5468 6520 6261 7365 2077 6f72 6b66 6c6f  The base workflo
-000002a0: 7720 636c 6173 7320 6f66 2064 6563 6f6d  w class of decom
-000002b0: 706f 7369 7469 6f6e 2061 6c67 6f72 6974  position algorit
-000002c0: 686d 732e 2222 220a 0a20 2020 2063 6f6d  hms."""..    com
-000002d0: 6d6f 6e5f 6675 6e63 7469 6f6e 203d 205b  mon_function = [
-000002e0: 224d 6f64 656c 2050 6572 7369 7374 656e  "Model Persisten
-000002f0: 6365 225d 2020 2320 2744 6563 6f6d 706f  ce"]  # 'Decompo
-00000300: 7369 7469 6f6e 2052 6573 756c 7427 2c0a  sition Result',.
-00000310: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00000320: 5f28 7365 6c66 2920 2d3e 204e 6f6e 653a  _(self) -> None:
-00000330: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
-00000340: 2e5f 5f69 6e69 745f 5f28 290a 0a20 2020  .__init__()..   
-00000350: 2020 2020 2023 2074 6865 2065 7874 7261       # the extra
-00000360: 2061 7474 7269 6275 7465 7320 7468 6174   attributes that
-00000370: 2064 6563 6f6d 706f 7369 7469 6f6e 2061   decomposition a
-00000380: 6c67 6f72 6974 686d 206e 6565 6473 0a20  lgorithm needs. 
-00000390: 2020 2020 2020 2073 656c 662e 585f 7265         self.X_re
-000003a0: 6475 6365 6420 3d20 4e6f 6e65 0a20 2020  duced = None.   
-000003b0: 2020 2020 2073 656c 662e 6d6f 6465 203d       self.mode =
-000003c0: 2022 4465 636f 6d70 6f73 6974 696f 6e22   "Decomposition"
-000003d0: 0a0a 2020 2020 6465 6620 6669 7428 7365  ..    def fit(se
-000003e0: 6c66 2c20 583a 2070 642e 4461 7461 4672  lf, X: pd.DataFr
-000003f0: 616d 652c 2079 3a20 4f70 7469 6f6e 616c  ame, y: Optional
-00000400: 5b70 642e 4461 7461 4672 616d 655d 203d  [pd.DataFrame] =
-00000410: 204e 6f6e 6529 202d 3e20 4e6f 6e65 3a0a   None) -> None:.
-00000420: 2020 2020 2020 2020 2222 2246 6974 2074          """Fit t
-00000430: 6865 206d 6f64 656c 2e22 2222 0a20 2020  he model.""".   
-00000440: 2020 2020 2073 656c 662e 6d6f 6465 6c2e       self.model.
-00000450: 6669 7428 5829 0a0a 2020 2020 6465 6620  fit(X)..    def 
-00000460: 7472 616e 7366 6f72 6d28 7365 6c66 2c20  transform(self, 
-00000470: 583a 2070 642e 4461 7461 4672 616d 6529  X: pd.DataFrame)
-00000480: 202d 3e20 7064 2e44 6174 6146 7261 6d65   -> pd.DataFrame
-00000490: 3a0a 2020 2020 2020 2020 2222 2241 7070  :.        """App
-000004a0: 6c79 2064 696d 656e 7369 6f6e 616c 6974  ly dimensionalit
-000004b0: 7920 7265 6475 6374 696f 6e20 746f 2058  y reduction to X
-000004c0: 2e22 2222 0a20 2020 2020 2020 2072 6574  .""".        ret
-000004d0: 7572 6e20 7365 6c66 2e6d 6f64 656c 2e74  urn self.model.t
-000004e0: 7261 6e73 666f 726d 2858 290a 0a20 2020  ransform(X)..   
-000004f0: 2064 6566 2066 6974 5f74 7261 6e73 666f   def fit_transfo
-00000500: 726d 2873 656c 662c 2058 3a20 7064 2e44  rm(self, X: pd.D
-00000510: 6174 6146 7261 6d65 2c20 793a 204f 7074  ataFrame, y: Opt
-00000520: 696f 6e61 6c5b 7064 2e44 6174 6146 7261  ional[pd.DataFra
-00000530: 6d65 5d20 3d20 4e6f 6e65 2920 2d3e 2070  me] = None) -> p
-00000540: 642e 4461 7461 4672 616d 653a 0a20 2020  d.DataFrame:.   
-00000550: 2020 2020 2022 2222 4669 7420 7468 6520       """Fit the 
-00000560: 6d6f 6465 6c20 7769 7468 2058 2061 6e64  model with X and
-00000570: 2061 7070 6c79 2074 6865 2064 696d 656e   apply the dimen
-00000580: 7369 6f6e 616c 6974 7920 7265 6475 6374  sionality reduct
-00000590: 696f 6e20 6f6e 2058 2e22 2222 0a20 2020  ion on X.""".   
-000005a0: 2020 2020 2023 2054 4f44 4f28 4361 6e20       # TODO(Can 
-000005b0: 4865 2853 616e 7929 2073 616e 6865 3130  He(Sany) sanhe10
-000005c0: 3937 3631 3834 3335 4031 3633 2e63 6f6d  97618435@163.com
-000005d0: 293a 2063 6865 636b 2069 6620 7765 206e  ): check if we n
-000005e0: 6565 6420 746f 2070 7574 2074 6869 7320  eed to put this 
-000005f0: 6675 6e63 7469 6f6e 2069 6e20 7468 6520  function in the 
-00000600: 6261 7365 2063 6c61 7373 0a20 2020 2020  base class.     
-00000610: 2020 2072 6574 7572 6e20 7365 6c66 2e6d     return self.m
-00000620: 6f64 656c 2e66 6974 5f74 7261 6e73 666f  odel.fit_transfo
-00000630: 726d 2858 290a 0a20 2020 2040 636c 6173  rm(X)..    @clas
-00000640: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
-00000650: 6d61 6e75 616c 5f68 7970 6572 5f70 6172  manual_hyper_par
-00000660: 616d 6574 6572 7328 636c 7329 202d 3e20  ameters(cls) -> 
-00000670: 4469 6374 3a0a 2020 2020 2020 2020 2222  Dict:.        ""
-00000680: 224d 616e 7561 6c20 6879 7065 722d 7061  "Manual hyper-pa
-00000690: 7261 6d65 7465 7273 2073 7065 6369 6669  rameters specifi
-000006a0: 6361 7469 6f6e 2e22 2222 0a20 2020 2020  cation.""".     
-000006b0: 2020 2072 6574 7572 6e20 6469 6374 2829     return dict()
-000006c0: 0a0a 2020 2020 6465 6620 5f72 6564 7563  ..    def _reduc
-000006d0: 6564 5f64 6174 6132 7064 2873 656c 662c  ed_data2pd(self,
-000006e0: 2072 6564 7563 6564 5f64 6174 613a 206e   reduced_data: n
-000006f0: 702e 6e64 6172 7261 792c 2063 6f6d 706f  p.ndarray, compo
-00000700: 6e65 6e74 735f 6e75 6d3a 2069 6e74 2920  nents_num: int) 
-00000710: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-00000720: 2022 2222 5472 616e 7366 6f72 6d20 7265   """Transform re
-00000730: 6475 6365 6420 6461 7461 2069 6e74 6f20  duced data into 
-00000740: 7468 6520 666f 726d 6174 206f 6620 7064  the format of pd
-00000750: 2e44 6174 6146 7261 6d65 2e0a 0a20 2020  .DataFrame...   
-00000760: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00000770: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00000780: 2d2d 0a20 2020 2020 2020 2072 6564 7563  --.        reduc
-00000790: 6564 5f64 6174 6120 3a20 6e70 2e6e 6461  ed_data : np.nda
-000007a0: 7272 6179 0a20 2020 2020 2020 2020 2020  rray.           
-000007b0: 2054 6865 2064 6174 6120 5820 6166 7465   The data X afte
-000007c0: 7220 6469 6d65 6e73 696f 6e20 7265 6475  r dimension redu
-000007d0: 6374 696f 6e2e 0a0a 2020 2020 2020 2020  ction...        
-000007e0: 636f 6d70 6f6e 656e 7473 5f6e 756d 203a  components_num :
-000007f0: 2069 6e74 0a20 2020 2020 2020 2020 2020   int.           
-00000800: 2054 6865 206e 756d 6265 7273 206f 6620   The numbers of 
-00000810: 7468 6520 7072 696e 6369 7061 6c20 636f  the principal co
-00000820: 6d70 6f6e 656e 7473 2e0a 2020 2020 2020  mponents..      
-00000830: 2020 2222 220a 2020 2020 2020 2020 7061    """.        pa
-00000840: 5f6e 616d 6520 3d20 5b5d 0a20 2020 2020  _name = [].     
-00000850: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00000860: 6528 636f 6d70 6f6e 656e 7473 5f6e 756d  e(components_num
-00000870: 293a 0a20 2020 2020 2020 2020 2020 2070  ):.            p
-00000880: 615f 6e61 6d65 2e61 7070 656e 6428 6622  a_name.append(f"
-00000890: 5072 696e 6369 7061 6c20 4178 6973 207b  Principal Axis {
-000008a0: 692b 317d 2229 0a20 2020 2020 2020 2073  i+1}").        s
-000008b0: 656c 662e 585f 7265 6475 6365 6420 3d20  elf.X_reduced = 
-000008c0: 7064 2e44 6174 6146 7261 6d65 2872 6564  pd.DataFrame(red
-000008d0: 7563 6564 5f64 6174 6129 0a20 2020 2020  uced_data).     
-000008e0: 2020 2073 656c 662e 585f 7265 6475 6365     self.X_reduce
-000008f0: 642e 636f 6c75 6d6e 7320 3d20 7061 5f6e  d.columns = pa_n
-00000900: 616d 650a 0a0a 636c 6173 7320 5043 4144  ame...class PCAD
-00000910: 6563 6f6d 706f 7369 7469 6f6e 2844 6563  ecomposition(Dec
-00000920: 6f6d 706f 7369 7469 6f6e 576f 726b 666c  ompositionWorkfl
-00000930: 6f77 4261 7365 293a 0a20 2020 2022 2222  owBase):.    """
-00000940: 5468 6520 6175 746f 6d61 7469 6f6e 2077  The automation w
-00000950: 6f72 6b66 6c6f 7720 6f66 2075 7369 6e67  orkflow of using
-00000960: 2050 4341 2061 6c67 6f72 6974 686d 2074   PCA algorithm t
-00000970: 6f20 6d61 6b65 2069 6e73 6967 6874 6675  o make insightfu
-00000980: 6c20 7072 6f64 7563 7473 2e22 2222 0a0a  l products."""..
-00000990: 2020 2020 6e61 6d65 203d 2022 5043 4122      name = "PCA"
-000009a0: 0a20 2020 2073 7065 6369 616c 5f66 756e  .    special_fun
-000009b0: 6374 696f 6e20 3d20 5b22 5072 696e 6369  ction = ["Princi
-000009c0: 7061 6c20 436f 6d70 6f6e 656e 7473 222c  pal Components",
-000009d0: 2022 4578 706c 6169 6e65 6420 5661 7269   "Explained Vari
-000009e0: 616e 6365 2052 6174 696f 222c 2022 436f  ance Ratio", "Co
-000009f0: 6d70 6f73 6974 696f 6e61 6c20 4269 2d70  mpositional Bi-p
-00000a00: 6c6f 7422 2c20 2243 6f6d 706f 7369 7469  lot", "Compositi
-00000a10: 6f6e 616c 2054 7269 2d70 6c6f 7422 5d0a  onal Tri-plot"].
-00000a20: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00000a30: 5f28 0a20 2020 2020 2020 2073 656c 662c  _(.        self,
-00000a40: 0a20 2020 2020 2020 206e 5f63 6f6d 706f  .        n_compo
-00000a50: 6e65 6e74 733a 204f 7074 696f 6e61 6c5b  nents: Optional[
-00000a60: 696e 745d 203d 204e 6f6e 652c 0a20 2020  int] = None,.   
-00000a70: 2020 2020 2063 6f70 793a 2062 6f6f 6c20       copy: bool 
-00000a80: 3d20 5472 7565 2c0a 2020 2020 2020 2020  = True,.        
-00000a90: 7768 6974 656e 3a20 626f 6f6c 203d 2046  whiten: bool = F
-00000aa0: 616c 7365 2c0a 2020 2020 2020 2020 7376  alse,.        sv
-00000ab0: 645f 736f 6c76 6572 3a20 7374 7220 3d20  d_solver: str = 
-00000ac0: 2261 7574 6f22 2c0a 2020 2020 2020 2020  "auto",.        
-00000ad0: 746f 6c3a 2066 6c6f 6174 203d 2030 2e30  tol: float = 0.0
-00000ae0: 2c0a 2020 2020 2020 2020 6974 6572 6174  ,.        iterat
-00000af0: 6564 5f70 6f77 6572 3a20 556e 696f 6e5b  ed_power: Union[
-00000b00: 696e 742c 2073 7472 5d20 3d20 2261 7574  int, str] = "aut
-00000b10: 6f22 2c0a 2020 2020 2020 2020 6e5f 6f76  o",.        n_ov
-00000b20: 6572 7361 6d70 6c65 733a 2069 6e74 203d  ersamples: int =
-00000b30: 2031 302c 0a20 2020 2020 2020 2070 6f77   10,.        pow
-00000b40: 6572 5f69 7465 7261 7469 6f6e 5f6e 6f72  er_iteration_nor
-00000b50: 6d61 6c69 7a65 723a 2073 7472 203d 2022  malizer: str = "
-00000b60: 6175 746f 222c 0a20 2020 2020 2020 2072  auto",.        r
-00000b70: 616e 646f 6d5f 7374 6174 653a 204f 7074  andom_state: Opt
-00000b80: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
-00000b90: 652c 0a20 2020 2029 202d 3e20 4e6f 6e65  e,.    ) -> None
-00000ba0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00000bb0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00000bc0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00000bd0: 2d2d 2d0a 2020 2020 2020 2020 6e5f 636f  ---.        n_co
-00000be0: 6d70 6f6e 656e 7473 203a 2069 6e74 2c20  mponents : int, 
-00000bf0: 666c 6f61 7420 6f72 2027 6d6c 6527 2c20  float or 'mle', 
-00000c00: 6465 6661 756c 743d 4e6f 6e65 0a20 2020  default=None.   
-00000c10: 2020 2020 2020 2020 204e 756d 6265 7220           Number 
-00000c20: 6f66 2063 6f6d 706f 6e65 6e74 7320 746f  of components to
-00000c30: 206b 6565 702e 0a20 2020 2020 2020 2020   keep..         
-00000c40: 2020 2069 6620 6e5f 636f 6d70 6f6e 656e     if n_componen
-00000c50: 7473 2069 7320 6e6f 7420 7365 7420 616c  ts is not set al
-00000c60: 6c20 636f 6d70 6f6e 656e 7473 2061 7265  l components are
-00000c70: 206b 6570 743a 3a0a 0a20 2020 2020 2020   kept::..       
-00000c80: 2020 2020 2020 2020 206e 5f63 6f6d 706f           n_compo
-00000c90: 6e65 6e74 7320 3d3d 206d 696e 286e 5f73  nents == min(n_s
-00000ca0: 616d 706c 6573 2c20 6e5f 6665 6174 7572  amples, n_featur
-00000cb0: 6573 290a 0a20 2020 2020 2020 2020 2020  es)..           
-00000cc0: 2049 6620 6060 6e5f 636f 6d70 6f6e 656e   If ``n_componen
-00000cd0: 7473 203d 3d20 276d 6c65 2760 6020 616e  ts == 'mle'`` an
-00000ce0: 6420 6060 7376 645f 736f 6c76 6572 203d  d ``svd_solver =
-00000cf0: 3d20 2766 756c 6c27 6060 2c20 4d69 6e6b  = 'full'``, Mink
-00000d00: 6127 730a 2020 2020 2020 2020 2020 2020  a's.            
-00000d10: 4d4c 4520 6973 2075 7365 6420 746f 2067  MLE is used to g
-00000d20: 7565 7373 2074 6865 2064 696d 656e 7369  uess the dimensi
-00000d30: 6f6e 2e20 5573 6520 6f66 2060 606e 5f63  on. Use of ``n_c
-00000d40: 6f6d 706f 6e65 6e74 7320 3d3d 2027 6d6c  omponents == 'ml
-00000d50: 6527 6060 0a20 2020 2020 2020 2020 2020  e'``.           
-00000d60: 2077 696c 6c20 696e 7465 7270 7265 7420   will interpret 
-00000d70: 6060 7376 645f 736f 6c76 6572 203d 3d20  ``svd_solver == 
-00000d80: 2761 7574 6f27 6060 2061 7320 6060 7376  'auto'`` as ``sv
-00000d90: 645f 736f 6c76 6572 203d 3d20 2766 756c  d_solver == 'ful
-00000da0: 6c27 6060 2e0a 0a20 2020 2020 2020 2020  l'``...         
-00000db0: 2020 2049 6620 6060 3020 3c20 6e5f 636f     If ``0 < n_co
-00000dc0: 6d70 6f6e 656e 7473 203c 2031 6060 2061  mponents < 1`` a
-00000dd0: 6e64 2060 6073 7664 5f73 6f6c 7665 7220  nd ``svd_solver 
-00000de0: 3d3d 2027 6675 6c6c 2760 602c 2073 656c  == 'full'``, sel
-00000df0: 6563 7420 7468 650a 2020 2020 2020 2020  ect the.        
-00000e00: 2020 2020 6e75 6d62 6572 206f 6620 636f      number of co
-00000e10: 6d70 6f6e 656e 7473 2073 7563 6820 7468  mponents such th
-00000e20: 6174 2074 6865 2061 6d6f 756e 7420 6f66  at the amount of
-00000e30: 2076 6172 6961 6e63 6520 7468 6174 206e   variance that n
-00000e40: 6565 6473 2074 6f20 6265 0a20 2020 2020  eeds to be.     
-00000e50: 2020 2020 2020 2065 7870 6c61 696e 6564         explained
-00000e60: 2069 7320 6772 6561 7465 7220 7468 616e   is greater than
-00000e70: 2074 6865 2070 6572 6365 6e74 6167 6520   the percentage 
-00000e80: 7370 6563 6966 6965 6420 6279 206e 5f63  specified by n_c
-00000e90: 6f6d 706f 6e65 6e74 732e 0a0a 2020 2020  omponents...    
-00000ea0: 2020 2020 2020 2020 4966 2060 6073 7664          If ``svd
-00000eb0: 5f73 6f6c 7665 7220 3d3d 2027 6172 7061  _solver == 'arpa
-00000ec0: 636b 2760 602c 2074 6865 206e 756d 6265  ck'``, the numbe
-00000ed0: 7220 6f66 2063 6f6d 706f 6e65 6e74 7320  r of components 
-00000ee0: 6d75 7374 2062 650a 2020 2020 2020 2020  must be.        
-00000ef0: 2020 2020 7374 7269 6374 6c79 206c 6573      strictly les
-00000f00: 7320 7468 616e 2074 6865 206d 696e 696d  s than the minim
-00000f10: 756d 206f 6620 6e5f 6665 6174 7572 6573  um of n_features
-00000f20: 2061 6e64 206e 5f73 616d 706c 6573 2e0a   and n_samples..
-00000f30: 0a20 2020 2020 2020 2020 2020 2048 656e  .            Hen
-00000f40: 6365 2c20 7468 6520 4e6f 6e65 2063 6173  ce, the None cas
-00000f50: 6520 7265 7375 6c74 7320 696e 3a3a 0a0a  e results in::..
-00000f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f70: 6e5f 636f 6d70 6f6e 656e 7473 203d 3d20  n_components == 
-00000f80: 6d69 6e28 6e5f 7361 6d70 6c65 732c 206e  min(n_samples, n
-00000f90: 5f66 6561 7475 7265 7329 202d 2031 0a0a  _features) - 1..
-00000fa0: 2020 2020 2020 2020 636f 7079 203a 2062          copy : b
-00000fb0: 6f6f 6c2c 2064 6566 6175 6c74 3d54 7275  ool, default=Tru
-00000fc0: 650a 2020 2020 2020 2020 2020 2020 4966  e.            If
-00000fd0: 2046 616c 7365 2c20 6461 7461 2070 6173   False, data pas
-00000fe0: 7365 6420 746f 2066 6974 2061 7265 206f  sed to fit are o
-00000ff0: 7665 7277 7269 7474 656e 2061 6e64 2072  verwritten and r
-00001000: 756e 6e69 6e67 0a20 2020 2020 2020 2020  unning.         
-00001010: 2020 2066 6974 2858 292e 7472 616e 7366     fit(X).transf
-00001020: 6f72 6d28 5829 2077 696c 6c20 6e6f 7420  orm(X) will not 
-00001030: 7969 656c 6420 7468 6520 6578 7065 6374  yield the expect
-00001040: 6564 2072 6573 756c 7473 2c0a 2020 2020  ed results,.    
-00001050: 2020 2020 2020 2020 7573 6520 6669 745f          use fit_
-00001060: 7472 616e 7366 6f72 6d28 5829 2069 6e73  transform(X) ins
-00001070: 7465 6164 2e0a 0a20 2020 2020 2020 2077  tead...        w
-00001080: 6869 7465 6e20 3a20 626f 6f6c 2c20 6465  hiten : bool, de
-00001090: 6661 756c 743d 4661 6c73 650a 2020 2020  fault=False.    
-000010a0: 2020 2020 2020 2020 5768 656e 2054 7275          When Tru
-000010b0: 6520 2846 616c 7365 2062 7920 6465 6661  e (False by defa
-000010c0: 756c 7429 2074 6865 2060 636f 6d70 6f6e  ult) the `compon
-000010d0: 656e 7473 5f60 2076 6563 746f 7273 2061  ents_` vectors a
-000010e0: 7265 206d 756c 7469 706c 6965 640a 2020  re multiplied.  
-000010f0: 2020 2020 2020 2020 2020 6279 2074 6865            by the
-00001100: 2073 7175 6172 6520 726f 6f74 206f 6620   square root of 
-00001110: 6e5f 7361 6d70 6c65 7320 616e 6420 7468  n_samples and th
-00001120: 656e 2064 6976 6964 6564 2062 7920 7468  en divided by th
-00001130: 6520 7369 6e67 756c 6172 2076 616c 7565  e singular value
-00001140: 730a 2020 2020 2020 2020 2020 2020 746f  s.            to
-00001150: 2065 6e73 7572 6520 756e 636f 7272 656c   ensure uncorrel
-00001160: 6174 6564 206f 7574 7075 7473 2077 6974  ated outputs wit
-00001170: 6820 756e 6974 2063 6f6d 706f 6e65 6e74  h unit component
-00001180: 2d77 6973 6520 7661 7269 616e 6365 732e  -wise variances.
-00001190: 0a20 2020 2020 2020 2020 2020 2057 6869  .            Whi
-000011a0: 7465 6e69 6e67 2077 696c 6c20 7265 6d6f  tening will remo
-000011b0: 7665 2073 6f6d 6520 696e 666f 726d 6174  ve some informat
-000011c0: 696f 6e20 6672 6f6d 2074 6865 2074 7261  ion from the tra
-000011d0: 6e73 666f 726d 6564 2073 6967 6e61 6c0a  nsformed signal.
-000011e0: 2020 2020 2020 2020 2020 2020 2874 6865              (the
-000011f0: 2072 656c 6174 6976 6520 7661 7269 616e   relative varian
-00001200: 6365 2073 6361 6c65 7320 6f66 2074 6865  ce scales of the
-00001210: 2063 6f6d 706f 6e65 6e74 7329 2062 7574   components) but
-00001220: 2063 616e 2073 6f6d 6574 696d 650a 2020   can sometime.  
-00001230: 2020 2020 2020 2020 2020 696d 7072 6f76            improv
-00001240: 6520 7468 6520 7072 6564 6963 7469 7665  e the predictive
-00001250: 2061 6363 7572 6163 7920 6f66 2074 6865   accuracy of the
-00001260: 2064 6f77 6e73 7472 6561 6d20 6573 7469   downstream esti
-00001270: 6d61 746f 7273 2062 790a 2020 2020 2020  mators by.      
-00001280: 2020 2020 2020 6d61 6b69 6e67 2074 6865        making the
-00001290: 6972 2064 6174 6120 7265 7370 6563 7420  ir data respect 
-000012a0: 736f 6d65 2068 6172 642d 7769 7265 6420  some hard-wired 
-000012b0: 6173 7375 6d70 7469 6f6e 732e 0a0a 2020  assumptions...  
-000012c0: 2020 2020 2020 7376 645f 736f 6c76 6572        svd_solver
-000012d0: 203a 207b 2761 7574 6f27 2c20 2766 756c   : {'auto', 'ful
-000012e0: 6c27 2c20 2761 7270 6163 6b27 2c20 2772  l', 'arpack', 'r
-000012f0: 616e 646f 6d69 7a65 6427 7d2c 2064 6566  andomized'}, def
-00001300: 6175 6c74 3d27 6175 746f 270a 2020 2020  ault='auto'.    
-00001310: 2020 2020 2020 2020 4966 2061 7574 6f20          If auto 
-00001320: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00001330: 2020 5468 6520 736f 6c76 6572 2069 7320    The solver is 
-00001340: 7365 6c65 6374 6564 2062 7920 6120 6465  selected by a de
-00001350: 6661 756c 7420 706f 6c69 6379 2062 6173  fault policy bas
-00001360: 6564 206f 6e20 6058 2e73 6861 7065 6020  ed on `X.shape` 
-00001370: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
-00001380: 2020 2020 606e 5f63 6f6d 706f 6e65 6e74      `n_component
-00001390: 7360 3a20 6966 2074 6865 2069 6e70 7574  s`: if the input
-000013a0: 2064 6174 6120 6973 206c 6172 6765 7220   data is larger 
-000013b0: 7468 616e 2035 3030 7835 3030 2061 6e64  than 500x500 and
-000013c0: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
-000013d0: 2020 2020 206e 756d 6265 7220 6f66 2063       number of c
-000013e0: 6f6d 706f 6e65 6e74 7320 746f 2065 7874  omponents to ext
-000013f0: 7261 6374 2069 7320 6c6f 7765 7220 7468  ract is lower th
-00001400: 616e 2038 3025 206f 6620 7468 6520 736d  an 80% of the sm
-00001410: 616c 6c65 7374 0a20 2020 2020 2020 2020  allest.         
-00001420: 2020 2020 2020 2064 696d 656e 7369 6f6e         dimension
-00001430: 206f 6620 7468 6520 6461 7461 2c20 7468   of the data, th
-00001440: 656e 2074 6865 206d 6f72 6520 6566 6669  en the more effi
-00001450: 6369 656e 7420 2772 616e 646f 6d69 7a65  cient 'randomize
-00001460: 6427 0a20 2020 2020 2020 2020 2020 2020  d'.             
-00001470: 2020 206d 6574 686f 6420 6973 2065 6e61     method is ena
-00001480: 626c 6564 2e20 4f74 6865 7277 6973 6520  bled. Otherwise 
-00001490: 7468 6520 6578 6163 7420 6675 6c6c 2053  the exact full S
-000014a0: 5644 2069 7320 636f 6d70 7574 6564 2061  VD is computed a
-000014b0: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
-000014c0: 2020 206f 7074 696f 6e61 6c6c 7920 7472     optionally tr
-000014d0: 756e 6361 7465 6420 6166 7465 7277 6172  uncated afterwar
-000014e0: 6473 2e0a 2020 2020 2020 2020 2020 2020  ds..            
-000014f0: 4966 2066 756c 6c20 3a0a 2020 2020 2020  If full :.      
-00001500: 2020 2020 2020 2020 2020 7275 6e20 6578            run ex
-00001510: 6163 7420 6675 6c6c 2053 5644 2063 616c  act full SVD cal
-00001520: 6c69 6e67 2074 6865 2073 7461 6e64 6172  ling the standar
-00001530: 6420 4c41 5041 434b 2073 6f6c 7665 7220  d LAPACK solver 
-00001540: 7669 610a 2020 2020 2020 2020 2020 2020  via.            
-00001550: 2020 2020 6073 6369 7079 2e6c 696e 616c      `scipy.linal
-00001560: 672e 7376 6460 2061 6e64 2073 656c 6563  g.svd` and selec
-00001570: 7420 7468 6520 636f 6d70 6f6e 656e 7473  t the components
-00001580: 2062 7920 706f 7374 7072 6f63 6573 7369   by postprocessi
-00001590: 6e67 0a20 2020 2020 2020 2020 2020 2049  ng.            I
-000015a0: 6620 6172 7061 636b 203a 0a20 2020 2020  f arpack :.     
-000015b0: 2020 2020 2020 2020 2020 2072 756e 2053             run S
-000015c0: 5644 2074 7275 6e63 6174 6564 2074 6f20  VD truncated to 
-000015d0: 6e5f 636f 6d70 6f6e 656e 7473 2063 616c  n_components cal
-000015e0: 6c69 6e67 2041 5250 4143 4b20 736f 6c76  ling ARPACK solv
-000015f0: 6572 2076 6961 0a20 2020 2020 2020 2020  er via.         
-00001600: 2020 2020 2020 2060 7363 6970 792e 7370         `scipy.sp
-00001610: 6172 7365 2e6c 696e 616c 672e 7376 6473  arse.linalg.svds
-00001620: 602e 2049 7420 7265 7175 6972 6573 2073  `. It requires s
-00001630: 7472 6963 746c 790a 2020 2020 2020 2020  trictly.        
-00001640: 2020 2020 2020 2020 3020 3c20 6e5f 636f          0 < n_co
-00001650: 6d70 6f6e 656e 7473 203c 206d 696e 2858  mponents < min(X
-00001660: 2e73 6861 7065 290a 2020 2020 2020 2020  .shape).        
-00001670: 2020 2020 4966 2072 616e 646f 6d69 7a65      If randomize
-00001680: 6420 3a0a 2020 2020 2020 2020 2020 2020  d :.            
-00001690: 2020 2020 7275 6e20 7261 6e64 6f6d 697a      run randomiz
-000016a0: 6564 2053 5644 2062 7920 7468 6520 6d65  ed SVD by the me
-000016b0: 7468 6f64 206f 6620 4861 6c6b 6f20 6574  thod of Halko et
-000016c0: 2061 6c2e 0a0a 2020 2020 2020 2020 2020   al...          
-000016d0: 2020 2e2e 2076 6572 7369 6f6e 6164 6465    .. versionadde
-000016e0: 643a 3a20 302e 3138 2e30 0a0a 2020 2020  d:: 0.18.0..    
-000016f0: 2020 2020 746f 6c20 3a20 666c 6f61 742c      tol : float,
-00001700: 2064 6566 6175 6c74 3d30 2e30 0a20 2020   default=0.0.   
-00001710: 2020 2020 2020 2020 2054 6f6c 6572 616e           Toleran
-00001720: 6365 2066 6f72 2073 696e 6775 6c61 7220  ce for singular 
-00001730: 7661 6c75 6573 2063 6f6d 7075 7465 6420  values computed 
-00001740: 6279 2073 7664 5f73 6f6c 7665 7220 3d3d  by svd_solver ==
-00001750: 2027 6172 7061 636b 272e 0a20 2020 2020   'arpack'..     
-00001760: 2020 2020 2020 204d 7573 7420 6265 206f         Must be o
-00001770: 6620 7261 6e67 6520 5b30 2e30 2c20 696e  f range [0.0, in
-00001780: 6669 6e69 7479 292e 0a0a 2020 2020 2020  finity)...      
-00001790: 2020 2020 2020 2e2e 2076 6572 7369 6f6e        .. version
-000017a0: 6164 6465 643a 3a20 302e 3138 2e30 0a0a  added:: 0.18.0..
-000017b0: 2020 2020 2020 2020 6974 6572 6174 6564          iterated
-000017c0: 5f70 6f77 6572 203a 2069 6e74 206f 7220  _power : int or 
-000017d0: 2761 7574 6f27 2c20 6465 6661 756c 743d  'auto', default=
-000017e0: 2761 7574 6f27 0a20 2020 2020 2020 2020  'auto'.         
-000017f0: 2020 204e 756d 6265 7220 6f66 2069 7465     Number of ite
-00001800: 7261 7469 6f6e 7320 666f 7220 7468 6520  rations for the 
-00001810: 706f 7765 7220 6d65 7468 6f64 2063 6f6d  power method com
-00001820: 7075 7465 6420 6279 0a20 2020 2020 2020  puted by.       
-00001830: 2020 2020 2073 7664 5f73 6f6c 7665 7220       svd_solver 
-00001840: 3d3d 2027 7261 6e64 6f6d 697a 6564 272e  == 'randomized'.
-00001850: 0a20 2020 2020 2020 2020 2020 204d 7573  .            Mus
-00001860: 7420 6265 206f 6620 7261 6e67 6520 5b30  t be of range [0
-00001870: 2c20 696e 6669 6e69 7479 292e 0a0a 2020  , infinity)...  
-00001880: 2020 2020 2020 2020 2020 2e2e 2076 6572            .. ver
-00001890: 7369 6f6e 6164 6465 643a 3a20 302e 3138  sionadded:: 0.18
-000018a0: 2e30 0a0a 2020 2020 2020 2020 6e5f 6f76  .0..        n_ov
-000018b0: 6572 7361 6d70 6c65 7320 3a20 696e 742c  ersamples : int,
-000018c0: 2064 6566 6175 6c74 3d31 300a 2020 2020   default=10.    
-000018d0: 2020 2020 2020 2020 5468 6973 2070 6172          This par
-000018e0: 616d 6574 6572 2069 7320 6f6e 6c79 2072  ameter is only r
-000018f0: 656c 6576 616e 7420 7768 656e 2060 7376  elevant when `sv
-00001900: 645f 736f 6c76 6572 3d22 7261 6e64 6f6d  d_solver="random
-00001910: 697a 6564 2260 2e0a 2020 2020 2020 2020  ized"`..        
-00001920: 2020 2020 4974 2063 6f72 7265 7370 6f6e      It correspon
-00001930: 6473 2074 6f20 7468 6520 6164 6469 7469  ds to the additi
-00001940: 6f6e 616c 206e 756d 6265 7220 6f66 2072  onal number of r
-00001950: 616e 646f 6d20 7665 6374 6f72 7320 746f  andom vectors to
-00001960: 2073 616d 706c 6520 7468 650a 2020 2020   sample the.    
-00001970: 2020 2020 2020 2020 7261 6e67 6520 6f66          range of
-00001980: 2060 5860 2073 6f20 6173 2074 6f20 656e   `X` so as to en
-00001990: 7375 7265 2070 726f 7065 7220 636f 6e64  sure proper cond
-000019a0: 6974 696f 6e69 6e67 2e20 5365 650a 2020  itioning. See.  
-000019b0: 2020 2020 2020 2020 2020 3a66 756e 633a            :func:
-000019c0: 607e 736b 6c65 6172 6e2e 7574 696c 732e  `~sklearn.utils.
-000019d0: 6578 746d 6174 682e 7261 6e64 6f6d 697a  extmath.randomiz
-000019e0: 6564 5f73 7664 6020 666f 7220 6d6f 7265  ed_svd` for more
-000019f0: 2064 6574 6169 6c73 2e0a 0a20 2020 2020   details...     
-00001a00: 2020 2020 2020 202e 2e20 7665 7273 696f         .. versio
-00001a10: 6e61 6464 6564 3a3a 2031 2e31 0a0a 2020  nadded:: 1.1..  
-00001a20: 2020 2020 2020 706f 7765 725f 6974 6572        power_iter
-00001a30: 6174 696f 6e5f 6e6f 726d 616c 697a 6572  ation_normalizer
-00001a40: 203a 207b 2761 7574 6f27 2c20 2751 5227   : {'auto', 'QR'
-00001a50: 2c20 274c 5527 2c20 276e 6f6e 6527 7d2c  , 'LU', 'none'},
-00001a60: 2064 6566 6175 6c74 3d27 6175 746f 270a   default='auto'.
-00001a70: 2020 2020 2020 2020 2020 2020 506f 7765              Powe
-00001a80: 7220 6974 6572 6174 696f 6e20 6e6f 726d  r iteration norm
-00001a90: 616c 697a 6572 2066 6f72 2072 616e 646f  alizer for rando
-00001aa0: 6d69 7a65 6420 5356 4420 736f 6c76 6572  mized SVD solver
-00001ab0: 2e0a 2020 2020 2020 2020 2020 2020 4e6f  ..            No
-00001ac0: 7420 7573 6564 2062 7920 4152 5041 434b  t used by ARPACK
-00001ad0: 2e20 5365 6520 3a66 756e 633a 607e 736b  . See :func:`~sk
-00001ae0: 6c65 6172 6e2e 7574 696c 732e 6578 746d  learn.utils.extm
-00001af0: 6174 682e 7261 6e64 6f6d 697a 6564 5f73  ath.randomized_s
-00001b00: 7664 600a 2020 2020 2020 2020 2020 2020  vd`.            
-00001b10: 666f 7220 6d6f 7265 2064 6574 6169 6c73  for more details
-00001b20: 2e0a 0a20 2020 2020 2020 2020 2020 202e  ...            .
-00001b30: 2e20 7665 7273 696f 6e61 6464 6564 3a3a  . versionadded::
-00001b40: 2031 2e31 0a0a 2020 2020 2020 2020 7261   1.1..        ra
-00001b50: 6e64 6f6d 5f73 7461 7465 203a 2069 6e74  ndom_state : int
-00001b60: 2c20 5261 6e64 6f6d 5374 6174 6520 696e  , RandomState in
-00001b70: 7374 616e 6365 206f 7220 4e6f 6e65 2c20  stance or None, 
-00001b80: 6465 6661 756c 743d 4e6f 6e65 0a20 2020  default=None.   
-00001b90: 2020 2020 2020 2020 2055 7365 6420 7768           Used wh
-00001ba0: 656e 2074 6865 2027 6172 7061 636b 2720  en the 'arpack' 
-00001bb0: 6f72 2027 7261 6e64 6f6d 697a 6564 2720  or 'randomized' 
-00001bc0: 736f 6c76 6572 7320 6172 6520 7573 6564  solvers are used
-00001bd0: 2e20 5061 7373 2061 6e20 696e 740a 2020  . Pass an int.  
-00001be0: 2020 2020 2020 2020 2020 666f 7220 7265            for re
-00001bf0: 7072 6f64 7563 6962 6c65 2072 6573 756c  producible resul
-00001c00: 7473 2061 6372 6f73 7320 6d75 6c74 6970  ts across multip
-00001c10: 6c65 2066 756e 6374 696f 6e20 6361 6c6c  le function call
-00001c20: 732e 0a20 2020 2020 2020 2020 2020 2053  s..            S
-00001c30: 6565 203a 7465 726d 3a60 476c 6f73 7361  ee :term:`Glossa
-00001c40: 7279 203c 7261 6e64 6f6d 5f73 7461 7465  ry <random_state
-00001c50: 3e60 2e0a 0a20 2020 2020 2020 2020 2020  >`...           
-00001c60: 202e 2e20 7665 7273 696f 6e61 6464 6564   .. versionadded
-00001c70: 3a3a 2030 2e31 382e 300a 0a20 2020 2020  :: 0.18.0..     
-00001c80: 2020 2052 6566 6572 656e 6365 730a 2020     References.  
-00001c90: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-00001ca0: 0a20 2020 2020 2020 2053 6369 6b69 742d  .        Scikit-
-00001cb0: 6c65 6172 6e20 4150 493a 2073 6b6c 6561  learn API: sklea
-00001cc0: 726e 2e64 6563 6f6d 706f 7369 7469 6f6e  rn.decomposition
-00001cd0: 2e50 4341 0a20 2020 2020 2020 2068 7474  .PCA.        htt
-00001ce0: 7073 3a2f 2f73 6369 6b69 742d 6c65 6172  ps://scikit-lear
-00001cf0: 6e2e 6f72 672f 7374 6162 6c65 2f6d 6f64  n.org/stable/mod
-00001d00: 756c 6573 2f67 656e 6572 6174 6564 2f73  ules/generated/s
-00001d10: 6b6c 6561 726e 2e64 6563 6f6d 706f 7369  klearn.decomposi
-00001d20: 7469 6f6e 2e50 4341 2e68 746d 6c0a 2020  tion.PCA.html.  
-00001d30: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00001d40: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
-00001d50: 5f5f 2829 0a20 2020 2020 2020 2073 656c  __().        sel
-00001d60: 662e 6e5f 636f 6d70 6f6e 656e 7473 203d  f.n_components =
-00001d70: 206e 5f63 6f6d 706f 6e65 6e74 730a 2020   n_components.  
-00001d80: 2020 2020 2020 7365 6c66 2e63 6f70 7920        self.copy 
-00001d90: 3d20 636f 7079 0a20 2020 2020 2020 2073  = copy.        s
-00001da0: 656c 662e 7768 6974 656e 203d 2077 6869  elf.whiten = whi
-00001db0: 7465 6e0a 2020 2020 2020 2020 7365 6c66  ten.        self
-00001dc0: 2e73 7664 5f73 6f6c 7665 7220 3d20 7376  .svd_solver = sv
-00001dd0: 645f 736f 6c76 6572 0a20 2020 2020 2020  d_solver.       
-00001de0: 2073 656c 662e 746f 6c20 3d20 746f 6c0a   self.tol = tol.
-00001df0: 2020 2020 2020 2020 7365 6c66 2e69 7465          self.ite
-00001e00: 7261 7465 645f 706f 7765 7220 3d20 6974  rated_power = it
-00001e10: 6572 6174 6564 5f70 6f77 6572 0a20 2020  erated_power.   
-00001e20: 2020 2020 2023 2073 656c 662e 6e5f 6f76       # self.n_ov
-00001e30: 6572 7361 6d70 6c65 7320 3d20 6e5f 6f76  ersamples = n_ov
-00001e40: 6572 7361 6d70 6c65 730a 2020 2020 2020  ersamples.      
-00001e50: 2020 2320 7365 6c66 2e70 6f77 6572 5f69    # self.power_i
-00001e60: 7465 7261 7469 6f6e 5f6e 6f72 6d61 6c69  teration_normali
-00001e70: 7a65 7220 3d20 706f 7765 725f 6974 6572  zer = power_iter
-00001e80: 6174 696f 6e5f 6e6f 726d 616c 697a 6572  ation_normalizer
-00001e90: 0a0a 2020 2020 2020 2020 6966 2072 616e  ..        if ran
-00001ea0: 646f 6d5f 7374 6174 653a 0a20 2020 2020  dom_state:.     
-00001eb0: 2020 2020 2020 2073 656c 662e 7261 6e64         self.rand
-00001ec0: 6f6d 5f73 7461 7465 203d 2072 616e 646f  om_state = rando
-00001ed0: 6d5f 7374 6174 650a 0a20 2020 2020 2020  m_state..       
-00001ee0: 2023 2049 6620 2772 616e 646f 6d5f 7374   # If 'random_st
-00001ef0: 6174 6527 2069 7320 4e6f 6e65 2c20 2773  ate' is None, 's
-00001f00: 656c 662e 7261 6e64 6f6d 5f73 7461 7465  elf.random_state
-00001f10: 2720 636f 6d65 7320 6672 6f6d 2074 6865  ' comes from the
-00001f20: 2070 6172 656e 7420 636c 6173 7320 2757   parent class 'W
-00001f30: 6f72 6b66 6c6f 7742 6173 6527 0a20 2020  orkflowBase'.   
-00001f40: 2020 2020 2073 656c 662e 6d6f 6465 6c20       self.model 
-00001f50: 3d20 5043 4128 0a20 2020 2020 2020 2020  = PCA(.         
-00001f60: 2020 206e 5f63 6f6d 706f 6e65 6e74 733d     n_components=
-00001f70: 7365 6c66 2e6e 5f63 6f6d 706f 6e65 6e74  self.n_component
-00001f80: 732c 0a20 2020 2020 2020 2020 2020 2063  s,.            c
-00001f90: 6f70 793d 7365 6c66 2e63 6f70 792c 0a20  opy=self.copy,. 
-00001fa0: 2020 2020 2020 2020 2020 2077 6869 7465             white
-00001fb0: 6e3d 7365 6c66 2e77 6869 7465 6e2c 0a20  n=self.whiten,. 
-00001fc0: 2020 2020 2020 2020 2020 2073 7664 5f73             svd_s
-00001fd0: 6f6c 7665 723d 7365 6c66 2e73 7664 5f73  olver=self.svd_s
-00001fe0: 6f6c 7665 722c 0a20 2020 2020 2020 2020  olver,.         
-00001ff0: 2020 2074 6f6c 3d73 656c 662e 746f 6c2c     tol=self.tol,
-00002000: 0a20 2020 2020 2020 2020 2020 2069 7465  .            ite
-00002010: 7261 7465 645f 706f 7765 723d 7365 6c66  rated_power=self
-00002020: 2e69 7465 7261 7465 645f 706f 7765 722c  .iterated_power,
-00002030: 0a20 2020 2020 2020 2020 2020 2023 206e  .            # n
-00002040: 5f6f 7665 7273 616d 706c 6573 3d73 656c  _oversamples=sel
-00002050: 662e 6e5f 6f76 6572 7361 6d70 6c65 732c  f.n_oversamples,
-00002060: 0a20 2020 2020 2020 2020 2020 2023 2070  .            # p
-00002070: 6f77 6572 5f69 7465 7261 7469 6f6e 5f6e  ower_iteration_n
-00002080: 6f72 6d61 6c69 7a65 723d 7365 6c66 2e70  ormalizer=self.p
-00002090: 6f77 6572 5f69 7465 7261 7469 6f6e 5f6e  ower_iteration_n
-000020a0: 6f72 6d61 6c69 7a65 722c 0a20 2020 2020  ormalizer,.     
-000020b0: 2020 2020 2020 2072 616e 646f 6d5f 7374         random_st
-000020c0: 6174 653d 7365 6c66 2e72 616e 646f 6d5f  ate=self.random_
-000020d0: 7374 6174 652c 0a20 2020 2020 2020 2029  state,.        )
-000020e0: 0a0a 2020 2020 2020 2020 7365 6c66 2e6e  ..        self.n
-000020f0: 616d 696e 6720 3d20 5043 4144 6563 6f6d  aming = PCADecom
-00002100: 706f 7369 7469 6f6e 2e6e 616d 650a 0a20  position.name.. 
-00002110: 2020 2020 2020 2023 2073 7065 6369 616c         # special
-00002120: 2061 7474 7269 6275 7465 730a 2020 2020   attributes.    
-00002130: 2020 2020 7365 6c66 2e70 635f 6461 7461      self.pc_data
-00002140: 203d 204e 6f6e 650a 0a20 2020 2040 636c   = None..    @cl
-00002150: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
-00002160: 6620 6d61 6e75 616c 5f68 7970 6572 5f70  f manual_hyper_p
-00002170: 6172 616d 6574 6572 7328 636c 7329 202d  arameters(cls) -
-00002180: 3e20 4469 6374 3a0a 2020 2020 2020 2020  > Dict:.        
-00002190: 2222 224d 616e 7561 6c20 6879 7065 722d  """Manual hyper-
-000021a0: 7061 7261 6d65 7465 7273 2073 7065 6369  parameters speci
-000021b0: 6669 6361 7469 6f6e 2e22 2222 0a20 2020  fication.""".   
-000021c0: 2020 2020 2070 7269 6e74 2866 222d 2a2d       print(f"-*-
-000021d0: 2a2d 207b 636c 732e 6e61 6d65 7d20 2d20  *- {cls.name} - 
-000021e0: 4879 7065 722d 7061 7261 6d65 7465 7273  Hyper-parameters
-000021f0: 2053 7065 6369 6669 6361 7469 6f6e 202d   Specification -
-00002200: 2a2d 2a2d 2229 0a20 2020 2020 2020 2068  *-*-").        h
-00002210: 7970 6572 5f70 6172 616d 6574 6572 7320  yper_parameters 
-00002220: 3d20 7063 615f 6d61 6e75 616c 5f68 7970  = pca_manual_hyp
-00002230: 6572 5f70 6172 616d 6574 6572 7328 290a  er_parameters().
-00002240: 2020 2020 2020 2020 636c 6561 725f 6f75          clear_ou
-00002250: 7470 7574 2829 0a20 2020 2020 2020 2072  tput().        r
-00002260: 6574 7572 6e20 6879 7065 725f 7061 7261  eturn hyper_para
-00002270: 6d65 7465 7273 0a0a 2020 2020 6465 6620  meters..    def 
-00002280: 5f67 6574 5f70 7269 6e63 6970 616c 5f63  _get_principal_c
-00002290: 6f6d 706f 6e65 6e74 7328 7365 6c66 2920  omponents(self) 
-000022a0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-000022b0: 2022 2222 4765 7420 7072 696e 6369 7061   """Get principa
-000022c0: 6c20 636f 6d70 6f6e 656e 7473 2e22 2222  l components."""
-000022d0: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
-000022e0: 2d2d 2d2d 2d2a 2050 7269 6e63 6970 616c  -----* Principal
-000022f0: 2043 6f6d 706f 6e65 6e74 7320 2a2d 2d2d   Components *---
-00002300: 2d2d 2229 0a20 2020 2020 2020 2070 7269  --").        pri
-00002310: 6e74 2822 4576 6572 7920 636f 6c75 6d6e  nt("Every column
-00002320: 2072 6570 7265 7365 6e74 7320 6f6e 6520   represents one 
-00002330: 7072 696e 6369 7061 6c20 636f 6d70 6f6e  principal compon
-00002340: 656e 7420 7265 7370 6563 7469 7665 6c79  ent respectively
-00002350: 2e22 290a 2020 2020 2020 2020 7072 696e  .").        prin
-00002360: 7428 2245 7665 7279 2072 6f77 2072 6570  t("Every row rep
-00002370: 7265 7365 6e74 7320 686f 7720 6d75 6368  resents how much
-00002380: 2074 6861 7420 726f 7720 6665 6174 7572   that row featur
-00002390: 6520 636f 6e74 7269 6275 7465 7320 746f  e contributes to
-000023a0: 2065 6163 6820 7072 696e 6369 7061 6c20   each principal 
-000023b0: 636f 6d70 6f6e 656e 7420 7265 7370 6563  component respec
-000023c0: 7469 7665 6c79 2e22 290a 2020 2020 2020  tively.").      
-000023d0: 2020 7072 696e 7428 2254 6865 2074 6162    print("The tab
-000023e0: 756c 6172 2064 6174 6120 6c6f 6f6b 7320  ular data looks 
-000023f0: 6c69 6b65 2069 6e20 666f 726d 6174 3a20  like in format: 
-00002400: 2772 6f77 7320 7820 636f 6c75 6d6e 7320  'rows x columns 
-00002410: 3d20 2766 6561 7475 7265 7320 7820 7072  = 'features x pr
-00002420: 696e 6369 7061 6c20 636f 6d70 6f6e 656e  incipal componen
-00002430: 7473 272e 2229 0a20 2020 2020 2020 2070  ts'.").        p
-00002440: 635f 6e61 6d65 203d 205b 5d0a 2020 2020  c_name = [].    
-00002450: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00002460: 6765 2873 656c 662e 6e5f 636f 6d70 6f6e  ge(self.n_compon
-00002470: 656e 7473 293a 0a20 2020 2020 2020 2020  ents):.         
-00002480: 2020 2070 635f 6e61 6d65 2e61 7070 656e     pc_name.appen
-00002490: 6428 6622 5043 7b69 2b31 7d22 290a 2020  d(f"PC{i+1}").  
-000024a0: 2020 2020 2020 7365 6c66 2e70 635f 6461        self.pc_da
-000024b0: 7461 203d 2070 642e 4461 7461 4672 616d  ta = pd.DataFram
-000024c0: 6528 7365 6c66 2e6d 6f64 656c 2e63 6f6d  e(self.model.com
-000024d0: 706f 6e65 6e74 735f 2e54 290a 2020 2020  ponents_.T).    
-000024e0: 2020 2020 7365 6c66 2e70 635f 6461 7461      self.pc_data
-000024f0: 2e63 6f6c 756d 6e73 203d 2070 635f 6e61  .columns = pc_na
-00002500: 6d65 0a20 2020 2020 2020 2073 656c 662e  me.        self.
-00002510: 7063 5f64 6174 612e 7365 745f 696e 6465  pc_data.set_inde
-00002520: 7828 4465 636f 6d70 6f73 6974 696f 6e57  x(DecompositionW
-00002530: 6f72 6b66 6c6f 7742 6173 652e 582e 636f  orkflowBase.X.co
-00002540: 6c75 6d6e 732c 2069 6e70 6c61 6365 3d54  lumns, inplace=T
-00002550: 7275 6529 0a20 2020 2020 2020 2070 7269  rue).        pri
-00002560: 6e74 2873 656c 662e 7063 5f64 6174 6129  nt(self.pc_data)
-00002570: 0a0a 2020 2020 6465 6620 5f67 6574 5f65  ..    def _get_e
-00002580: 7870 6c61 696e 6564 5f76 6172 6961 6e63  xplained_varianc
-00002590: 655f 7261 7469 6f28 7365 6c66 2920 2d3e  e_ratio(self) ->
-000025a0: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-000025b0: 2222 4765 7420 6578 706c 6169 6e65 6420  ""Get explained 
-000025c0: 7661 7269 616e 6365 2072 6174 696f 2e22  variance ratio."
-000025d0: 2222 0a20 2020 2020 2020 2070 7269 6e74  "".        print
-000025e0: 2822 2d2d 2d2d 2d2a 2045 7870 6c61 696e  ("-----* Explain
-000025f0: 6564 2056 6172 6961 6e63 6520 5261 7469  ed Variance Rati
-00002600: 6f20 2a2d 2d2d 2d2d 2229 0a20 2020 2020  o *-----").     
-00002610: 2020 2070 7269 6e74 2873 656c 662e 6d6f     print(self.mo
-00002620: 6465 6c2e 6578 706c 6169 6e65 645f 7661  del.explained_va
-00002630: 7269 616e 6365 5f72 6174 696f 5f29 0a0a  riance_ratio_)..
-00002640: 2020 2020 4073 7461 7469 636d 6574 686f      @staticmetho
-00002650: 640a 2020 2020 6465 6620 5f62 6970 6c6f  d.    def _biplo
-00002660: 7428 7265 6475 6365 645f 6461 7461 3a20  t(reduced_data: 
-00002670: 7064 2e44 6174 6146 7261 6d65 2c20 7063  pd.DataFrame, pc
-00002680: 5f64 6174 613a 2070 642e 4461 7461 4672  _data: pd.DataFr
-00002690: 616d 652c 2061 6c67 6f72 6974 686d 5f6e  ame, algorithm_n
-000026a0: 616d 653a 2073 7472 2c20 6c6f 6361 6c5f  ame: str, local_
-000026b0: 7061 7468 3a20 7374 722c 206d 6c66 6c6f  path: str, mlflo
-000026c0: 775f 7061 7468 3a20 7374 7229 202d 3e20  w_path: str) -> 
-000026d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
-000026e0: 2244 7261 7720 6269 2d70 6c6f 742e 2222  "Draw bi-plot.""
-000026f0: 220a 2020 2020 2020 2020 7072 696e 7428  ".        print(
-00002700: 222d 2d2d 2d2d 2a20 436f 6d70 6f73 6974  "-----* Composit
-00002710: 696f 6e61 6c20 4269 2d70 6c6f 7420 2a2d  ional Bi-plot *-
-00002720: 2d2d 2d2d 2229 0a20 2020 2020 2020 2062  ----").        b
-00002730: 6970 6c6f 7428 7265 6475 6365 645f 6461  iplot(reduced_da
-00002740: 7461 2c20 7063 5f64 6174 612c 2061 6c67  ta, pc_data, alg
-00002750: 6f72 6974 686d 5f6e 616d 6529 0a20 2020  orithm_name).   
-00002760: 2020 2020 2073 6176 655f 6669 6728 6622       save_fig(f"
-00002770: 436f 6d70 6f73 6974 696f 6e61 6c20 4269  Compositional Bi
-00002780: 2d70 6c6f 7420 2d20 7b61 6c67 6f72 6974  -plot - {algorit
-00002790: 686d 5f6e 616d 657d 222c 206c 6f63 616c  hm_name}", local
-000027a0: 5f70 6174 682c 206d 6c66 6c6f 775f 7061  _path, mlflow_pa
-000027b0: 7468 290a 2020 2020 2020 2020 7361 7665  th).        save
-000027c0: 5f64 6174 6128 7265 6475 6365 645f 6461  _data(reduced_da
-000027d0: 7461 2c20 2243 6f6d 706f 7369 7469 6f6e  ta, "Composition
-000027e0: 616c 2042 692d 706c 6f74 202d 2052 6564  al Bi-plot - Red
-000027f0: 7563 6564 2044 6174 6122 2c20 6c6f 6361  uced Data", loca
-00002800: 6c5f 7061 7468 2c20 6d6c 666c 6f77 5f70  l_path, mlflow_p
-00002810: 6174 6829 0a20 2020 2020 2020 2073 6176  ath).        sav
-00002820: 655f 6461 7461 2870 635f 6461 7461 2c20  e_data(pc_data, 
-00002830: 2243 6f6d 706f 7369 7469 6f6e 616c 2042  "Compositional B
-00002840: 692d 706c 6f74 202d 2050 4320 4461 7461  i-plot - PC Data
-00002850: 222c 206c 6f63 616c 5f70 6174 682c 206d  ", local_path, m
-00002860: 6c66 6c6f 775f 7061 7468 290a 0a20 2020  lflow_path)..   
-00002870: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
-00002880: 2020 2064 6566 205f 7472 6970 6c6f 7428     def _triplot(
-00002890: 7265 6475 6365 645f 6461 7461 3a20 7064  reduced_data: pd
-000028a0: 2e44 6174 6146 7261 6d65 2c20 7063 5f64  .DataFrame, pc_d
-000028b0: 6174 613a 2070 642e 4461 7461 4672 616d  ata: pd.DataFram
-000028c0: 652c 2061 6c67 6f72 6974 686d 5f6e 616d  e, algorithm_nam
-000028d0: 653a 2073 7472 2c20 6c6f 6361 6c5f 7061  e: str, local_pa
-000028e0: 7468 3a20 7374 722c 206d 6c66 6c6f 775f  th: str, mlflow_
-000028f0: 7061 7468 3a20 7374 7229 202d 3e20 4e6f  path: str) -> No
-00002900: 6e65 3a0a 2020 2020 2020 2020 2222 2244  ne:.        """D
-00002910: 7261 7720 7472 692d 706c 6f74 2e22 2222  raw tri-plot."""
-00002920: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
-00002930: 2d2d 2d2d 2d2a 2043 6f6d 706f 7369 7469  -----* Compositi
-00002940: 6f6e 616c 2054 7269 2d70 6c6f 7420 2a2d  onal Tri-plot *-
-00002950: 2d2d 2d2d 2229 0a20 2020 2020 2020 2074  ----").        t
-00002960: 7269 706c 6f74 2872 6564 7563 6564 5f64  riplot(reduced_d
-00002970: 6174 612c 2070 635f 6461 7461 2c20 616c  ata, pc_data, al
-00002980: 676f 7269 7468 6d5f 6e61 6d65 290a 2020  gorithm_name).  
-00002990: 2020 2020 2020 7361 7665 5f66 6967 2866        save_fig(f
-000029a0: 2243 6f6d 706f 7369 7469 6f6e 616c 2054  "Compositional T
-000029b0: 7269 2d70 6c6f 7420 2d20 7b61 6c67 6f72  ri-plot - {algor
-000029c0: 6974 686d 5f6e 616d 657d 222c 206c 6f63  ithm_name}", loc
-000029d0: 616c 5f70 6174 682c 206d 6c66 6c6f 775f  al_path, mlflow_
-000029e0: 7061 7468 290a 2020 2020 2020 2020 7361  path).        sa
-000029f0: 7665 5f64 6174 6128 7265 6475 6365 645f  ve_data(reduced_
-00002a00: 6461 7461 2c20 2243 6f6d 706f 7369 7469  data, "Compositi
-00002a10: 6f6e 616c 2054 7269 2d70 6c6f 7420 2d20  onal Tri-plot - 
-00002a20: 5265 6475 6365 6420 4461 7461 222c 206c  Reduced Data", l
-00002a30: 6f63 616c 5f70 6174 682c 206d 6c66 6c6f  ocal_path, mlflo
-00002a40: 775f 7061 7468 290a 2020 2020 2020 2020  w_path).        
-00002a50: 7361 7665 5f64 6174 6128 7063 5f64 6174  save_data(pc_dat
-00002a60: 612c 2022 436f 6d70 6f73 6974 696f 6e61  a, "Compositiona
-00002a70: 6c20 5472 692d 706c 6f74 202d 2050 4320  l Tri-plot - PC 
-00002a80: 4461 7461 222c 206c 6f63 616c 5f70 6174  Data", local_pat
-00002a90: 682c 206d 6c66 6c6f 775f 7061 7468 290a  h, mlflow_path).
-00002aa0: 0a20 2020 2064 6566 2073 7065 6369 616c  .    def special
-00002ab0: 5f63 6f6d 706f 6e65 6e74 7328 7365 6c66  _components(self
-00002ac0: 2c20 2a2a 6b77 6172 6773 3a20 556e 696f  , **kwargs: Unio
-00002ad0: 6e5b 4469 6374 2c20 6e70 2e6e 6461 7272  n[Dict, np.ndarr
-00002ae0: 6179 2c20 696e 745d 2920 2d3e 204e 6f6e  ay, int]) -> Non
-00002af0: 653a 0a20 2020 2020 2020 2022 2222 496e  e:.        """In
-00002b00: 766f 6b65 2061 6c6c 2073 7065 6369 616c  voke all special
-00002b10: 2061 7070 6c69 6361 7469 6f6e 2066 756e   application fun
-00002b20: 6374 696f 6e73 2066 6f72 2074 6869 7320  ctions for this 
-00002b30: 616c 676f 7269 7468 6d73 2062 7920 5363  algorithms by Sc
-00002b40: 696b 6974 2d6c 6561 726e 2066 7261 6d65  ikit-learn frame
-00002b50: 776f 726b 2e22 2222 0a20 2020 2020 2020  work.""".       
-00002b60: 2073 656c 662e 5f72 6564 7563 6564 5f64   self._reduced_d
-00002b70: 6174 6132 7064 286b 7761 7267 735b 2272  ata2pd(kwargs["r
-00002b80: 6564 7563 6564 5f64 6174 6122 5d2c 206b  educed_data"], k
-00002b90: 7761 7267 735b 2263 6f6d 706f 6e65 6e74  wargs["component
-00002ba0: 735f 6e75 6d22 5d29 0a20 2020 2020 2020  s_num"]).       
-00002bb0: 2073 656c 662e 5f67 6574 5f70 7269 6e63   self._get_princ
-00002bc0: 6970 616c 5f63 6f6d 706f 6e65 6e74 7328  ipal_components(
-00002bd0: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
-00002be0: 6765 745f 6578 706c 6169 6e65 645f 7661  get_explained_va
-00002bf0: 7269 616e 6365 5f72 6174 696f 2829 0a0a  riance_ratio()..
-00002c00: 2020 2020 2020 2020 4745 4f50 495f 4f55          GEOPI_OU
-00002c10: 5450 5554 5f41 5254 4946 4143 5453 5f49  TPUT_ARTIFACTS_I
-00002c20: 4d41 4745 5f4d 4f44 454c 5f4f 5554 5055  MAGE_MODEL_OUTPU
-00002c30: 545f 5041 5448 203d 206f 732e 6765 7465  T_PATH = os.gete
-00002c40: 6e76 2822 4745 4f50 495f 4f55 5450 5554  nv("GEOPI_OUTPUT
-00002c50: 5f41 5254 4946 4143 5453 5f49 4d41 4745  _ARTIFACTS_IMAGE
-00002c60: 5f4d 4f44 454c 5f4f 5554 5055 545f 5041  _MODEL_OUTPUT_PA
-00002c70: 5448 2229 0a20 2020 2020 2020 2023 2044  TH").        # D
-00002c80: 7261 7720 6772 6170 6873 2077 6865 6e20  raw graphs when 
-00002c90: 7468 6520 6e75 6d62 6572 206f 6620 7072  the number of pr
-00002ca0: 696e 6369 7061 6c20 636f 6d70 6f6e 656e  incipal componen
-00002cb0: 7473 203e 2033 0a20 2020 2020 2020 2069  ts > 3.        i
-00002cc0: 6620 6b77 6172 6773 5b22 636f 6d70 6f6e  f kwargs["compon
-00002cd0: 656e 7473 5f6e 756d 225d 203e 2033 3a0a  ents_num"] > 3:.
-00002ce0: 2020 2020 2020 2020 2020 2020 2320 6368              # ch
-00002cf0: 6f6f 7365 2074 776f 206f 6620 6469 6d65  oose two of dime
-00002d00: 6e73 696f 6e73 2074 6f20 6472 6177 0a20  nsions to draw. 
-00002d10: 2020 2020 2020 2020 2020 2074 776f 5f64             two_d
-00002d20: 696d 656e 5f61 7869 735f 696e 6465 782c  imen_axis_index,
-00002d30: 2074 776f 5f64 696d 656e 5f70 635f 6461   two_dimen_pc_da
-00002d40: 7461 203d 2073 656c 662e 6368 6f6f 7365  ta = self.choose
-00002d50: 5f64 696d 656e 7369 6f6e 5f64 6174 6128  _dimension_data(
-00002d60: 7365 6c66 2e70 635f 6461 7461 2c20 3229  self.pc_data, 2)
-00002d70: 0a20 2020 2020 2020 2020 2020 2074 776f  .            two
-00002d80: 5f64 696d 656e 5f72 6564 7563 6564 5f64  _dimen_reduced_d
-00002d90: 6174 6120 3d20 7365 6c66 2e58 5f72 6564  ata = self.X_red
-00002da0: 7563 6564 2e69 6c6f 635b 3a2c 2074 776f  uced.iloc[:, two
-00002db0: 5f64 696d 656e 5f61 7869 735f 696e 6465  _dimen_axis_inde
-00002dc0: 785d 0a20 2020 2020 2020 2020 2020 2073  x].            s
-00002dd0: 656c 662e 5f62 6970 6c6f 7428 0a20 2020  elf._biplot(.   
-00002de0: 2020 2020 2020 2020 2020 2020 2072 6564               red
-00002df0: 7563 6564 5f64 6174 613d 7477 6f5f 6469  uced_data=two_di
-00002e00: 6d65 6e5f 7265 6475 6365 645f 6461 7461  men_reduced_data
-00002e10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002e20: 2020 7063 5f64 6174 613d 7477 6f5f 6469    pc_data=two_di
-00002e30: 6d65 6e5f 7063 5f64 6174 612c 0a20 2020  men_pc_data,.   
-00002e40: 2020 2020 2020 2020 2020 2020 2061 6c67               alg
-00002e50: 6f72 6974 686d 5f6e 616d 653d 7365 6c66  orithm_name=self
-00002e60: 2e6e 616d 696e 672c 0a20 2020 2020 2020  .naming,.       
-00002e70: 2020 2020 2020 2020 206c 6f63 616c 5f70           local_p
-00002e80: 6174 683d 4745 4f50 495f 4f55 5450 5554  ath=GEOPI_OUTPUT
-00002e90: 5f41 5254 4946 4143 5453 5f49 4d41 4745  _ARTIFACTS_IMAGE
-00002ea0: 5f4d 4f44 454c 5f4f 5554 5055 545f 5041  _MODEL_OUTPUT_PA
-00002eb0: 5448 2c0a 2020 2020 2020 2020 2020 2020  TH,.            
-00002ec0: 2020 2020 6d6c 666c 6f77 5f70 6174 683d      mlflow_path=
-00002ed0: 4d4c 464c 4f57 5f41 5254 4946 4143 545f  MLFLOW_ARTIFACT_
-00002ee0: 494d 4147 455f 4d4f 4445 4c5f 4f55 5450  IMAGE_MODEL_OUTP
-00002ef0: 5554 5f50 4154 482c 0a20 2020 2020 2020  UT_PATH,.       
-00002f00: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00002f10: 2020 2020 2320 6368 6f6f 7365 2074 6872      # choose thr
-00002f20: 6565 206f 6620 6469 6d65 6e73 696f 6e73  ee of dimensions
-00002f30: 2074 6f20 6472 6177 0a20 2020 2020 2020   to draw.       
-00002f40: 2020 2020 2074 6872 6565 5f64 696d 656e       three_dimen
-00002f50: 5f61 7869 735f 696e 6465 782c 2074 6872  _axis_index, thr
-00002f60: 6565 5f64 696d 656e 5f70 635f 6461 7461  ee_dimen_pc_data
-00002f70: 203d 2073 656c 662e 6368 6f6f 7365 5f64   = self.choose_d
-00002f80: 696d 656e 7369 6f6e 5f64 6174 6128 7365  imension_data(se
-00002f90: 6c66 2e70 635f 6461 7461 2c20 3329 0a20  lf.pc_data, 3). 
-00002fa0: 2020 2020 2020 2020 2020 2074 6872 6565             three
-00002fb0: 5f64 696d 656e 5f72 6564 7563 6564 5f64  _dimen_reduced_d
-00002fc0: 6174 6120 3d20 7365 6c66 2e58 5f72 6564  ata = self.X_red
-00002fd0: 7563 6564 2e69 6c6f 635b 3a2c 2074 6872  uced.iloc[:, thr
-00002fe0: 6565 5f64 696d 656e 5f61 7869 735f 696e  ee_dimen_axis_in
-00002ff0: 6465 785d 0a20 2020 2020 2020 2020 2020  dex].           
-00003000: 2073 656c 662e 5f74 7269 706c 6f74 280a   self._triplot(.
-00003010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003020: 7265 6475 6365 645f 6461 7461 3d74 6872  reduced_data=thr
-00003030: 6565 5f64 696d 656e 5f72 6564 7563 6564  ee_dimen_reduced
-00003040: 5f64 6174 612c 0a20 2020 2020 2020 2020  _data,.         
-00003050: 2020 2020 2020 2070 635f 6461 7461 3d74         pc_data=t
-00003060: 6872 6565 5f64 696d 656e 5f70 635f 6461  hree_dimen_pc_da
-00003070: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
-00003080: 2020 2020 616c 676f 7269 7468 6d5f 6e61      algorithm_na
-00003090: 6d65 3d73 656c 662e 6e61 6d69 6e67 2c0a  me=self.naming,.
-000030a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030b0: 6c6f 6361 6c5f 7061 7468 3d47 454f 5049  local_path=GEOPI
-000030c0: 5f4f 5554 5055 545f 4152 5449 4641 4354  _OUTPUT_ARTIFACT
-000030d0: 535f 494d 4147 455f 4d4f 4445 4c5f 4f55  S_IMAGE_MODEL_OU
-000030e0: 5450 5554 5f50 4154 482c 0a20 2020 2020  TPUT_PATH,.     
-000030f0: 2020 2020 2020 2020 2020 206d 6c66 6c6f             mlflo
-00003100: 775f 7061 7468 3d4d 4c46 4c4f 575f 4152  w_path=MLFLOW_AR
-00003110: 5449 4641 4354 5f49 4d41 4745 5f4d 4f44  TIFACT_IMAGE_MOD
-00003120: 454c 5f4f 5554 5055 545f 5041 5448 2c0a  EL_OUTPUT_PATH,.
-00003130: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00003140: 2020 2020 2020 656c 6966 206b 7761 7267        elif kwarg
-00003150: 735b 2263 6f6d 706f 6e65 6e74 735f 6e75  s["components_nu
-00003160: 6d22 5d20 3d3d 2033 3a0a 2020 2020 2020  m"] == 3:.      
-00003170: 2020 2020 2020 2320 6368 6f6f 7365 2074        # choose t
-00003180: 776f 206f 6620 6469 6d65 6e73 696f 6e73  wo of dimensions
-00003190: 2074 6f20 6472 6177 0a20 2020 2020 2020   to draw.       
-000031a0: 2020 2020 2074 776f 5f64 696d 656e 5f61       two_dimen_a
-000031b0: 7869 735f 696e 6465 782c 2074 776f 5f64  xis_index, two_d
-000031c0: 696d 656e 5f70 635f 6461 7461 203d 2073  imen_pc_data = s
-000031d0: 656c 662e 6368 6f6f 7365 5f64 696d 656e  elf.choose_dimen
-000031e0: 7369 6f6e 5f64 6174 6128 7365 6c66 2e70  sion_data(self.p
-000031f0: 635f 6461 7461 2c20 3229 0a20 2020 2020  c_data, 2).     
-00003200: 2020 2020 2020 2074 776f 5f64 696d 656e         two_dimen
-00003210: 5f72 6564 7563 6564 5f64 6174 6120 3d20  _reduced_data = 
-00003220: 7365 6c66 2e58 5f72 6564 7563 6564 2e69  self.X_reduced.i
-00003230: 6c6f 635b 3a2c 2074 776f 5f64 696d 656e  loc[:, two_dimen
-00003240: 5f61 7869 735f 696e 6465 785d 0a20 2020  _axis_index].   
-00003250: 2020 2020 2020 2020 2073 656c 662e 5f62           self._b
-00003260: 6970 6c6f 7428 0a20 2020 2020 2020 2020  iplot(.         
-00003270: 2020 2020 2020 2072 6564 7563 6564 5f64         reduced_d
-00003280: 6174 613d 7477 6f5f 6469 6d65 6e5f 7265  ata=two_dimen_re
-00003290: 6475 6365 645f 6461 7461 2c0a 2020 2020  duced_data,.    
-000032a0: 2020 2020 2020 2020 2020 2020 7063 5f64              pc_d
-000032b0: 6174 613d 7477 6f5f 6469 6d65 6e5f 7063  ata=two_dimen_pc
-000032c0: 5f64 6174 612c 0a20 2020 2020 2020 2020  _data,.         
-000032d0: 2020 2020 2020 2061 6c67 6f72 6974 686d         algorithm
-000032e0: 5f6e 616d 653d 7365 6c66 2e6e 616d 696e  _name=self.namin
-000032f0: 672c 0a20 2020 2020 2020 2020 2020 2020  g,.             
-00003300: 2020 206c 6f63 616c 5f70 6174 683d 4745     local_path=GE
-00003310: 4f50 495f 4f55 5450 5554 5f41 5254 4946  OPI_OUTPUT_ARTIF
-00003320: 4143 5453 5f49 4d41 4745 5f4d 4f44 454c  ACTS_IMAGE_MODEL
-00003330: 5f4f 5554 5055 545f 5041 5448 2c0a 2020  _OUTPUT_PATH,.  
-00003340: 2020 2020 2020 2020 2020 2020 2020 6d6c                ml
-00003350: 666c 6f77 5f70 6174 683d 4d4c 464c 4f57  flow_path=MLFLOW
-00003360: 5f41 5254 4946 4143 545f 494d 4147 455f  _ARTIFACT_IMAGE_
-00003370: 4d4f 4445 4c5f 4f55 5450 5554 5f50 4154  MODEL_OUTPUT_PAT
-00003380: 482c 0a20 2020 2020 2020 2020 2020 2029  H,.            )
-00003390: 0a20 2020 2020 2020 2020 2020 2023 206e  .            # n
-000033a0: 6f20 6e65 6564 2074 6f20 6368 6f6f 7365  o need to choose
-000033b0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000033c0: 662e 5f74 7269 706c 6f74 280a 2020 2020  f._triplot(.    
-000033d0: 2020 2020 2020 2020 2020 2020 7265 6475              redu
-000033e0: 6365 645f 6461 7461 3d73 656c 662e 585f  ced_data=self.X_
-000033f0: 7265 6475 6365 642c 0a20 2020 2020 2020  reduced,.       
-00003400: 2020 2020 2020 2020 2070 635f 6461 7461           pc_data
-00003410: 3d73 656c 662e 7063 5f64 6174 612c 0a20  =self.pc_data,. 
-00003420: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00003430: 6c67 6f72 6974 686d 5f6e 616d 653d 7365  lgorithm_name=se
-00003440: 6c66 2e6e 616d 696e 672c 0a20 2020 2020  lf.naming,.     
-00003450: 2020 2020 2020 2020 2020 206c 6f63 616c             local
-00003460: 5f70 6174 683d 4745 4f50 495f 4f55 5450  _path=GEOPI_OUTP
-00003470: 5554 5f41 5254 4946 4143 5453 5f49 4d41  UT_ARTIFACTS_IMA
-00003480: 4745 5f4d 4f44 454c 5f4f 5554 5055 545f  GE_MODEL_OUTPUT_
-00003490: 5041 5448 2c0a 2020 2020 2020 2020 2020  PATH,.          
-000034a0: 2020 2020 2020 6d6c 666c 6f77 5f70 6174        mlflow_pat
-000034b0: 683d 4d4c 464c 4f57 5f41 5254 4946 4143  h=MLFLOW_ARTIFAC
-000034c0: 545f 494d 4147 455f 4d4f 4445 4c5f 4f55  T_IMAGE_MODEL_OU
-000034d0: 5450 5554 5f50 4154 482c 0a20 2020 2020  TPUT_PATH,.     
-000034e0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000034f0: 2065 6c69 6620 6b77 6172 6773 5b22 636f   elif kwargs["co
-00003500: 6d70 6f6e 656e 7473 5f6e 756d 225d 203d  mponents_num"] =
-00003510: 3d20 323a 0a20 2020 2020 2020 2020 2020  = 2:.           
-00003520: 2073 656c 662e 5f62 6970 6c6f 7428 0a20   self._biplot(. 
-00003530: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00003540: 6564 7563 6564 5f64 6174 613d 7365 6c66  educed_data=self
-00003550: 2e58 5f72 6564 7563 6564 2c0a 2020 2020  .X_reduced,.    
-00003560: 2020 2020 2020 2020 2020 2020 7063 5f64              pc_d
-00003570: 6174 613d 7365 6c66 2e70 635f 6461 7461  ata=self.pc_data
-00003580: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003590: 2020 616c 676f 7269 7468 6d5f 6e61 6d65    algorithm_name
-000035a0: 3d73 656c 662e 6e61 6d69 6e67 2c0a 2020  =self.naming,.  
-000035b0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-000035c0: 6361 6c5f 7061 7468 3d47 454f 5049 5f4f  cal_path=GEOPI_O
-000035d0: 5554 5055 545f 4152 5449 4641 4354 535f  UTPUT_ARTIFACTS_
-000035e0: 494d 4147 455f 4d4f 4445 4c5f 4f55 5450  IMAGE_MODEL_OUTP
-000035f0: 5554 5f50 4154 482c 0a20 2020 2020 2020  UT_PATH,.       
-00003600: 2020 2020 2020 2020 206d 6c66 6c6f 775f           mlflow_
-00003610: 7061 7468 3d4d 4c46 4c4f 575f 4152 5449  path=MLFLOW_ARTI
-00003620: 4641 4354 5f49 4d41 4745 5f4d 4f44 454c  FACT_IMAGE_MODEL
-00003630: 5f4f 5554 5055 545f 5041 5448 2c0a 2020  _OUTPUT_PATH,.  
-00003640: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00003650: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00003660: 2020 2020 2020 7061 7373 0a0a 0a63 6c61        pass...cla
-00003670: 7373 2054 534e 4544 6563 6f6d 706f 7369  ss TSNEDecomposi
-00003680: 7469 6f6e 2844 6563 6f6d 706f 7369 7469  tion(Decompositi
-00003690: 6f6e 576f 726b 666c 6f77 4261 7365 293a  onWorkflowBase):
-000036a0: 0a20 2020 2022 2222 5468 6520 6175 746f  .    """The auto
-000036b0: 6d61 7469 6f6e 2077 6f72 6b66 6c6f 7720  mation workflow 
-000036c0: 6f66 2075 7369 6e67 2054 2d53 4e45 2061  of using T-SNE a
-000036d0: 6c67 6f72 6974 686d 2074 6f20 6d61 6b65  lgorithm to make
-000036e0: 2069 6e73 6967 6874 6675 6c20 7072 6f64   insightful prod
-000036f0: 7563 7473 2e22 2222 0a0a 2020 2020 6e61  ucts."""..    na
-00003700: 6d65 203d 2022 542d 534e 4522 0a20 2020  me = "T-SNE".   
-00003710: 2073 7065 6369 616c 5f66 756e 6374 696f   special_functio
-00003720: 6e20 3d20 5b5d 0a0a 2020 2020 6465 6620  n = []..    def 
-00003730: 5f5f 696e 6974 5f5f 280a 2020 2020 2020  __init__(.      
-00003740: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00003750: 6e5f 636f 6d70 6f6e 656e 7473 3a20 696e  n_components: in
-00003760: 7420 3d20 322c 0a20 2020 2020 2020 202a  t = 2,.        *
-00003770: 2c0a 2020 2020 2020 2020 7065 7270 6c65  ,.        perple
-00003780: 7869 7479 3a20 666c 6f61 7420 3d20 3330  xity: float = 30
-00003790: 2e30 2c0a 2020 2020 2020 2020 6561 726c  .0,.        earl
-000037a0: 795f 6578 6167 6765 7261 7469 6f6e 3a20  y_exaggeration: 
-000037b0: 666c 6f61 7420 3d20 3132 2e30 2c0a 2020  float = 12.0,.  
-000037c0: 2020 2020 2020 6c65 6172 6e69 6e67 5f72        learning_r
-000037d0: 6174 653a 2055 6e69 6f6e 5b66 6c6f 6174  ate: Union[float
-000037e0: 2c20 7374 725d 203d 2022 6175 746f 222c  , str] = "auto",
-000037f0: 0a20 2020 2020 2020 206e 5f69 7465 723a  .        n_iter:
-00003800: 2069 6e74 203d 2031 3030 302c 0a20 2020   int = 1000,.   
-00003810: 2020 2020 206e 5f69 7465 725f 7769 7468       n_iter_with
-00003820: 6f75 745f 7072 6f67 7265 7373 3a20 696e  out_progress: in
-00003830: 7420 3d20 3330 302c 0a20 2020 2020 2020  t = 300,.       
-00003840: 206d 696e 5f67 7261 645f 6e6f 726d 3a20   min_grad_norm: 
-00003850: 666c 6f61 7420 3d20 3165 2d37 2c0a 2020  float = 1e-7,.  
-00003860: 2020 2020 2020 6d65 7472 6963 3a20 7374        metric: st
-00003870: 7220 3d20 2265 7563 6c69 6465 616e 222c  r = "euclidean",
-00003880: 0a20 2020 2020 2020 206d 6574 7269 635f  .        metric_
-00003890: 7061 7261 6d73 3a20 4f70 7469 6f6e 616c  params: Optional
-000038a0: 5b44 6963 745d 203d 204e 6f6e 652c 0a20  [Dict] = None,. 
-000038b0: 2020 2020 2020 2069 6e69 743a 2073 7472         init: str
-000038c0: 203d 2022 7063 6122 2c0a 2020 2020 2020   = "pca",.      
-000038d0: 2020 7665 7262 6f73 653a 2069 6e74 203d    verbose: int =
-000038e0: 2030 2c0a 2020 2020 2020 2020 7261 6e64   0,.        rand
-000038f0: 6f6d 5f73 7461 7465 3a20 4f70 7469 6f6e  om_state: Option
-00003900: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a  al[int] = None,.
-00003910: 2020 2020 2020 2020 6d65 7468 6f64 3a20          method: 
-00003920: 7374 7220 3d20 2265 7861 6374 222c 0a20  str = "exact",. 
-00003930: 2020 2020 2020 2061 6e67 6c65 3a20 666c         angle: fl
-00003940: 6f61 7420 3d20 302e 352c 0a20 2020 2020  oat = 0.5,.     
-00003950: 2020 206e 5f6a 6f62 733a 2069 6e74 203d     n_jobs: int =
-00003960: 204e 6f6e 652c 0a20 2020 2020 2020 2073   None,.        s
-00003970: 7175 6172 655f 6469 7374 616e 6365 733a  quare_distances:
-00003980: 2055 6e69 6f6e 5b62 6f6f 6c2c 2073 7472   Union[bool, str
-00003990: 5d20 3d20 2264 6570 7265 6361 7465 6422  ] = "deprecated"
-000039a0: 2c0a 2020 2020 2920 2d3e 204e 6f6e 653a  ,.    ) -> None:
-000039b0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000039c0: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-000039d0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-000039e0: 2d2d 0a20 2020 2020 2020 206e 5f63 6f6d  --.        n_com
-000039f0: 706f 6e65 6e74 7320 3a20 696e 742c 2064  ponents : int, d
-00003a00: 6566 6175 6c74 3d32 0a20 2020 2020 2020  efault=2.       
-00003a10: 2020 2020 2044 696d 656e 7369 6f6e 206f       Dimension o
-00003a20: 6620 7468 6520 656d 6265 6464 6564 2073  f the embedded s
-00003a30: 7061 6365 2e0a 0a20 2020 2020 2020 2070  pace...        p
-00003a40: 6572 706c 6578 6974 7920 3a20 666c 6f61  erplexity : floa
-00003a50: 742c 2064 6566 6175 6c74 3d33 302e 300a  t, default=30.0.
-00003a60: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00003a70: 7065 7270 6c65 7869 7479 2069 7320 7265  perplexity is re
-00003a80: 6c61 7465 6420 746f 2074 6865 206e 756d  lated to the num
-00003a90: 6265 7220 6f66 206e 6561 7265 7374 206e  ber of nearest n
-00003aa0: 6569 6768 626f 7273 2074 6861 740a 2020  eighbors that.  
-00003ab0: 2020 2020 2020 2020 2020 6973 2075 7365            is use
-00003ac0: 6420 696e 206f 7468 6572 206d 616e 6966  d in other manif
-00003ad0: 6f6c 6420 6c65 6172 6e69 6e67 2061 6c67  old learning alg
-00003ae0: 6f72 6974 686d 732e 204c 6172 6765 7220  orithms. Larger 
-00003af0: 6461 7461 7365 7473 0a20 2020 2020 2020  datasets.       
-00003b00: 2020 2020 2075 7375 616c 6c79 2072 6571       usually req
-00003b10: 7569 7265 2061 206c 6172 6765 7220 7065  uire a larger pe
-00003b20: 7270 6c65 7869 7479 2e20 436f 6e73 6964  rplexity. Consid
-00003b30: 6572 2073 656c 6563 7469 6e67 2061 2076  er selecting a v
-00003b40: 616c 7565 0a20 2020 2020 2020 2020 2020  alue.           
-00003b50: 2062 6574 7765 656e 2035 2061 6e64 2035   between 5 and 5
-00003b60: 302e 2044 6966 6665 7265 6e74 2076 616c  0. Different val
-00003b70: 7565 7320 6361 6e20 7265 7375 6c74 2069  ues can result i
-00003b80: 6e20 7369 676e 6966 6963 616e 746c 790a  n significantly.
-00003b90: 2020 2020 2020 2020 2020 2020 6469 6666              diff
-00003ba0: 6572 656e 7420 7265 7375 6c74 732e 2054  erent results. T
-00003bb0: 6865 2070 6572 706c 6578 6974 7920 6d75  he perplexity mu
-00003bc0: 7374 2062 6520 6c65 7373 2074 6861 6e20  st be less than 
-00003bd0: 7468 6520 6e75 6d62 6572 0a20 2020 2020  the number.     
-00003be0: 2020 2020 2020 206f 6620 7361 6d70 6c65         of sample
-00003bf0: 732e 0a0a 2020 2020 2020 2020 6561 726c  s...        earl
-00003c00: 795f 6578 6167 6765 7261 7469 6f6e 203a  y_exaggeration :
-00003c10: 2066 6c6f 6174 2c20 6465 6661 756c 743d   float, default=
-00003c20: 3132 2e30 0a20 2020 2020 2020 2020 2020  12.0.           
-00003c30: 2043 6f6e 7472 6f6c 7320 686f 7720 7469   Controls how ti
-00003c40: 6768 7420 6e61 7475 7261 6c20 636c 7573  ght natural clus
-00003c50: 7465 7273 2069 6e20 7468 6520 6f72 6967  ters in the orig
-00003c60: 696e 616c 2073 7061 6365 2061 7265 2069  inal space are i
-00003c70: 6e0a 2020 2020 2020 2020 2020 2020 7468  n.            th
-00003c80: 6520 656d 6265 6464 6564 2073 7061 6365  e embedded space
-00003c90: 2061 6e64 2068 6f77 206d 7563 6820 7370   and how much sp
-00003ca0: 6163 6520 7769 6c6c 2062 6520 6265 7477  ace will be betw
-00003cb0: 6565 6e20 7468 656d 2e20 466f 720a 2020  een them. For.  
-00003cc0: 2020 2020 2020 2020 2020 6c61 7267 6572            larger
-00003cd0: 2076 616c 7565 732c 2074 6865 2073 7061   values, the spa
-00003ce0: 6365 2062 6574 7765 656e 206e 6174 7572  ce between natur
-00003cf0: 616c 2063 6c75 7374 6572 7320 7769 6c6c  al clusters will
-00003d00: 2062 6520 6c61 7267 6572 0a20 2020 2020   be larger.     
-00003d10: 2020 2020 2020 2069 6e20 7468 6520 656d         in the em
-00003d20: 6265 6464 6564 2073 7061 6365 2e20 4167  bedded space. Ag
-00003d30: 6169 6e2c 2074 6865 2063 686f 6963 6520  ain, the choice 
-00003d40: 6f66 2074 6869 7320 7061 7261 6d65 7465  of this paramete
-00003d50: 7220 6973 206e 6f74 0a20 2020 2020 2020  r is not.       
-00003d60: 2020 2020 2076 6572 7920 6372 6974 6963       very critic
-00003d70: 616c 2e20 4966 2074 6865 2063 6f73 7420  al. If the cost 
-00003d80: 6675 6e63 7469 6f6e 2069 6e63 7265 6173  function increas
-00003d90: 6573 2064 7572 696e 6720 696e 6974 6961  es during initia
-00003da0: 6c0a 2020 2020 2020 2020 2020 2020 6f70  l.            op
-00003db0: 7469 6d69 7a61 7469 6f6e 2c20 7468 6520  timization, the 
-00003dc0: 6561 726c 7920 6578 6167 6765 7261 7469  early exaggerati
-00003dd0: 6f6e 2066 6163 746f 7220 6f72 2074 6865  on factor or the
-00003de0: 206c 6561 726e 696e 6720 7261 7465 0a20   learning rate. 
-00003df0: 2020 2020 2020 2020 2020 206d 6967 6874             might
-00003e00: 2062 6520 746f 6f20 6869 6768 2e0a 0a20   be too high... 
-00003e10: 2020 2020 2020 206c 6561 726e 696e 675f         learning_
-00003e20: 7261 7465 203a 2066 6c6f 6174 206f 7220  rate : float or 
-00003e30: 2261 7574 6f22 2c20 6465 6661 756c 743d  "auto", default=
-00003e40: 2261 7574 6f22 0a20 2020 2020 2020 2020  "auto".         
-00003e50: 2020 2054 6865 206c 6561 726e 696e 6720     The learning 
-00003e60: 7261 7465 2066 6f72 2074 2d53 4e45 2069  rate for t-SNE i
-00003e70: 7320 7573 7561 6c6c 7920 696e 2074 6865  s usually in the
-00003e80: 2072 616e 6765 205b 3130 2e30 2c20 3130   range [10.0, 10
-00003e90: 3030 2e30 5d2e 2049 660a 2020 2020 2020  00.0]. If.      
-00003ea0: 2020 2020 2020 7468 6520 6c65 6172 6e69        the learni
-00003eb0: 6e67 2072 6174 6520 6973 2074 6f6f 2068  ng rate is too h
-00003ec0: 6967 682c 2074 6865 2064 6174 6120 6d61  igh, the data ma
-00003ed0: 7920 6c6f 6f6b 206c 696b 6520 6120 2762  y look like a 'b
-00003ee0: 616c 6c27 2077 6974 6820 616e 790a 2020  all' with any.  
-00003ef0: 2020 2020 2020 2020 2020 706f 696e 7420            point 
-00003f00: 6170 7072 6f78 696d 6174 656c 7920 6571  approximately eq
-00003f10: 7569 6469 7374 616e 7420 6672 6f6d 2069  uidistant from i
-00003f20: 7473 206e 6561 7265 7374 206e 6569 6768  ts nearest neigh
-00003f30: 626f 7572 732e 2049 6620 7468 650a 2020  bours. If the.  
-00003f40: 2020 2020 2020 2020 2020 6c65 6172 6e69            learni
-00003f50: 6e67 2072 6174 6520 6973 2074 6f6f 206c  ng rate is too l
-00003f60: 6f77 2c20 6d6f 7374 2070 6f69 6e74 7320  ow, most points 
-00003f70: 6d61 7920 6c6f 6f6b 2063 6f6d 7072 6573  may look compres
-00003f80: 7365 6420 696e 2061 2064 656e 7365 0a20  sed in a dense. 
-00003f90: 2020 2020 2020 2020 2020 2063 6c6f 7564             cloud
-00003fa0: 2077 6974 6820 6665 7720 6f75 746c 6965   with few outlie
-00003fb0: 7273 2e20 4966 2074 6865 2063 6f73 7420  rs. If the cost 
-00003fc0: 6675 6e63 7469 6f6e 2067 6574 7320 7374  function gets st
-00003fd0: 7563 6b20 696e 2061 2062 6164 206c 6f63  uck in a bad loc
-00003fe0: 616c 0a20 2020 2020 2020 2020 2020 206d  al.            m
-00003ff0: 696e 696d 756d 2069 6e63 7265 6173 696e  inimum increasin
-00004000: 6720 7468 6520 6c65 6172 6e69 6e67 2072  g the learning r
-00004010: 6174 6520 6d61 7920 6865 6c70 2e0a 2020  ate may help..  
-00004020: 2020 2020 2020 2020 2020 4e6f 7465 2074            Note t
-00004030: 6861 7420 6d61 6e79 206f 7468 6572 2074  hat many other t
-00004040: 2d53 4e45 2069 6d70 6c65 6d65 6e74 6174  -SNE implementat
-00004050: 696f 6e73 2028 6268 7473 6e65 2c20 4649  ions (bhtsne, FI
-00004060: 742d 534e 452c 206f 7065 6e54 534e 452c  t-SNE, openTSNE,
-00004070: 0a20 2020 2020 2020 2020 2020 2065 7463  .            etc
-00004080: 2e29 2075 7365 2061 2064 6566 696e 6974  .) use a definit
-00004090: 696f 6e20 6f66 206c 6561 726e 696e 675f  ion of learning_
-000040a0: 7261 7465 2074 6861 7420 6973 2034 2074  rate that is 4 t
-000040b0: 696d 6573 2073 6d61 6c6c 6572 2074 6861  imes smaller tha
-000040c0: 6e0a 2020 2020 2020 2020 2020 2020 6f75  n.            ou
-000040d0: 7273 2e20 536f 206f 7572 206c 6561 726e  rs. So our learn
-000040e0: 696e 675f 7261 7465 3d32 3030 2063 6f72  ing_rate=200 cor
-000040f0: 7265 7370 6f6e 6473 2074 6f20 6c65 6172  responds to lear
-00004100: 6e69 6e67 5f72 6174 653d 3830 3020 696e  ning_rate=800 in
-00004110: 0a20 2020 2020 2020 2020 2020 2074 686f  .            tho
-00004120: 7365 206f 7468 6572 2069 6d70 6c65 6d65  se other impleme
-00004130: 6e74 6174 696f 6e73 2e20 5468 6520 2761  ntations. The 'a
-00004140: 7574 6f27 206f 7074 696f 6e20 7365 7473  uto' option sets
-00004150: 2074 6865 206c 6561 726e 696e 675f 7261   the learning_ra
-00004160: 7465 0a20 2020 2020 2020 2020 2020 2074  te.            t
-00004170: 6f20 606d 6178 284e 202f 2065 6172 6c79  o `max(N / early
-00004180: 5f65 7861 6767 6572 6174 696f 6e20 2f20  _exaggeration / 
-00004190: 342c 2035 3029 6020 7768 6572 6520 4e20  4, 50)` where N 
-000041a0: 6973 2074 6865 2073 616d 706c 6520 7369  is the sample si
-000041b0: 7a65 2c0a 2020 2020 2020 2020 2020 2020  ze,.            
-000041c0: 666f 6c6c 6f77 696e 6720 5b34 5d20 616e  following [4] an
-000041d0: 6420 5b35 5d2e 0a0a 2020 2020 2020 2020  d [5]...        
-000041e0: 2020 2020 2e2e 2076 6572 7369 6f6e 6368      .. versionch
-000041f0: 616e 6765 643a 3a20 312e 320a 2020 2020  anged:: 1.2.    
-00004200: 2020 2020 2020 2020 5468 6520 6465 6661          The defa
-00004210: 756c 7420 7661 6c75 6520 6368 616e 6765  ult value change
-00004220: 6420 746f 2060 2261 7574 6f22 602e 0a0a  d to `"auto"`...
-00004230: 2020 2020 2020 2020 6e5f 6974 6572 203a          n_iter :
-00004240: 2069 6e74 2c20 6465 6661 756c 743d 3130   int, default=10
-00004250: 3030 0a20 2020 2020 2020 2020 2020 204d  00.            M
-00004260: 6178 696d 756d 206e 756d 6265 7220 6f66  aximum number of
-00004270: 2069 7465 7261 7469 6f6e 7320 666f 7220   iterations for 
-00004280: 7468 6520 6f70 7469 6d69 7a61 7469 6f6e  the optimization
-00004290: 2e20 5368 6f75 6c64 2062 6520 6174 0a20  . Should be at. 
-000042a0: 2020 2020 2020 2020 2020 206c 6561 7374             least
-000042b0: 2032 3530 2e0a 0a20 2020 2020 2020 206e   250...        n
-000042c0: 5f69 7465 725f 7769 7468 6f75 745f 7072  _iter_without_pr
-000042d0: 6f67 7265 7373 203a 2069 6e74 2c20 6465  ogress : int, de
-000042e0: 6661 756c 743d 3330 300a 2020 2020 2020  fault=300.      
-000042f0: 2020 2020 2020 4d61 7869 6d75 6d20 6e75        Maximum nu
-00004300: 6d62 6572 206f 6620 6974 6572 6174 696f  mber of iteratio
-00004310: 6e73 2077 6974 686f 7574 2070 726f 6772  ns without progr
-00004320: 6573 7320 6265 666f 7265 2077 6520 6162  ess before we ab
-00004330: 6f72 7420 7468 650a 2020 2020 2020 2020  ort the.        
-00004340: 2020 2020 6f70 7469 6d69 7a61 7469 6f6e      optimization
-00004350: 2c20 7573 6564 2061 6674 6572 2032 3530  , used after 250
-00004360: 2069 6e69 7469 616c 2069 7465 7261 7469   initial iterati
-00004370: 6f6e 7320 7769 7468 2065 6172 6c79 0a20  ons with early. 
-00004380: 2020 2020 2020 2020 2020 2065 7861 6767             exagg
-00004390: 6572 6174 696f 6e2e 204e 6f74 6520 7468  eration. Note th
-000043a0: 6174 2070 726f 6772 6573 7320 6973 206f  at progress is o
-000043b0: 6e6c 7920 6368 6563 6b65 6420 6576 6572  nly checked ever
-000043c0: 7920 3530 2069 7465 7261 7469 6f6e 7320  y 50 iterations 
-000043d0: 736f 0a20 2020 2020 2020 2020 2020 2074  so.            t
-000043e0: 6869 7320 7661 6c75 6520 6973 2072 6f75  his value is rou
-000043f0: 6e64 6564 2074 6f20 7468 6520 6e65 7874  nded to the next
-00004400: 206d 756c 7469 706c 6520 6f66 2035 302e   multiple of 50.
-00004410: 0a0a 2020 2020 2020 2020 2020 2020 2e2e  ..            ..
-00004420: 2076 6572 7369 6f6e 6164 6465 643a 3a20   versionadded:: 
-00004430: 302e 3137 0a20 2020 2020 2020 2020 2020  0.17.           
-00004440: 2070 6172 616d 6574 6572 202a 6e5f 6974   parameter *n_it
-00004450: 6572 5f77 6974 686f 7574 5f70 726f 6772  er_without_progr
-00004460: 6573 732a 2074 6f20 636f 6e74 726f 6c20  ess* to control 
-00004470: 7374 6f70 7069 6e67 2063 7269 7465 7269  stopping criteri
-00004480: 612e 0a0a 2020 2020 2020 2020 6d69 6e5f  a...        min_
-00004490: 6772 6164 5f6e 6f72 6d20 3a20 666c 6f61  grad_norm : floa
-000044a0: 742c 2064 6566 6175 6c74 3d31 652d 370a  t, default=1e-7.
-000044b0: 2020 2020 2020 2020 2020 2020 4966 2074              If t
-000044c0: 6865 2067 7261 6469 656e 7420 6e6f 726d  he gradient norm
-000044d0: 2069 7320 6265 6c6f 7720 7468 6973 2074   is below this t
-000044e0: 6872 6573 686f 6c64 2c20 7468 6520 6f70  hreshold, the op
-000044f0: 7469 6d69 7a61 7469 6f6e 2077 696c 6c0a  timization will.
-00004500: 2020 2020 2020 2020 2020 2020 6265 2073              be s
-00004510: 746f 7070 6564 2e0a 0a20 2020 2020 2020  topped...       
-00004520: 206d 6574 7269 6320 3a20 7374 7220 6f72   metric : str or
-00004530: 2063 616c 6c61 626c 652c 2064 6566 6175   callable, defau
-00004540: 6c74 3d27 6575 636c 6964 6561 6e27 0a20  lt='euclidean'. 
-00004550: 2020 2020 2020 2020 2020 2054 6865 206d             The m
-00004560: 6574 7269 6320 746f 2075 7365 2077 6865  etric to use whe
-00004570: 6e20 6361 6c63 756c 6174 696e 6720 6469  n calculating di
-00004580: 7374 616e 6365 2062 6574 7765 656e 2069  stance between i
-00004590: 6e73 7461 6e63 6573 2069 6e20 610a 2020  nstances in a.  
-000045a0: 2020 2020 2020 2020 2020 6665 6174 7572            featur
-000045b0: 6520 6172 7261 792e 2049 6620 6d65 7472  e array. If metr
-000045c0: 6963 2069 7320 6120 7374 7269 6e67 2c20  ic is a string, 
-000045d0: 6974 206d 7573 7420 6265 206f 6e65 206f  it must be one o
-000045e0: 6620 7468 6520 6f70 7469 6f6e 730a 2020  f the options.  
-000045f0: 2020 2020 2020 2020 2020 616c 6c6f 7765            allowe
-00004600: 6420 6279 2073 6369 7079 2e73 7061 7469  d by scipy.spati
-00004610: 616c 2e64 6973 7461 6e63 652e 7064 6973  al.distance.pdis
-00004620: 7420 666f 7220 6974 7320 6d65 7472 6963  t for its metric
-00004630: 2070 6172 616d 6574 6572 2c20 6f72 0a20   parameter, or. 
-00004640: 2020 2020 2020 2020 2020 2061 206d 6574             a met
-00004650: 7269 6320 6c69 7374 6564 2069 6e20 7061  ric listed in pa
-00004660: 6972 7769 7365 2e50 4149 5257 4953 455f  irwise.PAIRWISE_
-00004670: 4449 5354 414e 4345 5f46 554e 4354 494f  DISTANCE_FUNCTIO
-00004680: 4e53 2e0a 2020 2020 2020 2020 2020 2020  NS..            
-00004690: 4966 206d 6574 7269 6320 6973 2022 7072  If metric is "pr
-000046a0: 6563 6f6d 7075 7465 6422 2c20 5820 6973  ecomputed", X is
-000046b0: 2061 7373 756d 6564 2074 6f20 6265 2061   assumed to be a
-000046c0: 2064 6973 7461 6e63 6520 6d61 7472 6978   distance matrix
-000046d0: 2e0a 2020 2020 2020 2020 2020 2020 416c  ..            Al
-000046e0: 7465 726e 6174 6976 656c 792c 2069 6620  ternatively, if 
-000046f0: 6d65 7472 6963 2069 7320 6120 6361 6c6c  metric is a call
-00004700: 6162 6c65 2066 756e 6374 696f 6e2c 2069  able function, i
-00004710: 7420 6973 2063 616c 6c65 6420 6f6e 2065  t is called on e
-00004720: 6163 680a 2020 2020 2020 2020 2020 2020  ach.            
-00004730: 7061 6972 206f 6620 696e 7374 616e 6365  pair of instance
-00004740: 7320 2872 6f77 7329 2061 6e64 2074 6865  s (rows) and the
-00004750: 2072 6573 756c 7469 6e67 2076 616c 7565   resulting value
-00004760: 2072 6563 6f72 6465 642e 2054 6865 2063   recorded. The c
-00004770: 616c 6c61 626c 650a 2020 2020 2020 2020  allable.        
-00004780: 2020 2020 7368 6f75 6c64 2074 616b 6520      should take 
-00004790: 7477 6f20 6172 7261 7973 2066 726f 6d20  two arrays from 
-000047a0: 5820 6173 2069 6e70 7574 2061 6e64 2072  X as input and r
-000047b0: 6574 7572 6e20 6120 7661 6c75 6520 696e  eturn a value in
-000047c0: 6469 6361 7469 6e67 0a20 2020 2020 2020  dicating.       
-000047d0: 2020 2020 2074 6865 2064 6973 7461 6e63       the distanc
-000047e0: 6520 6265 7477 6565 6e20 7468 656d 2e20  e between them. 
-000047f0: 5468 6520 6465 6661 756c 7420 6973 2022  The default is "
-00004800: 6575 636c 6964 6561 6e22 2077 6869 6368  euclidean" which
-00004810: 2069 730a 2020 2020 2020 2020 2020 2020   is.            
-00004820: 696e 7465 7270 7265 7465 6420 6173 2073  interpreted as s
-00004830: 7175 6172 6564 2065 7563 6c69 6465 616e  quared euclidean
-00004840: 2064 6973 7461 6e63 652e 0a0a 2020 2020   distance...    
-00004850: 2020 2020 6d65 7472 6963 5f70 6172 616d      metric_param
-00004860: 7320 3a20 6469 6374 2c20 6465 6661 756c  s : dict, defaul
-00004870: 743d 4e6f 6e65 0a20 2020 2020 2020 2020  t=None.         
-00004880: 2020 2041 6464 6974 696f 6e61 6c20 6b65     Additional ke
-00004890: 7977 6f72 6420 6172 6775 6d65 6e74 7320  yword arguments 
-000048a0: 666f 7220 7468 6520 6d65 7472 6963 2066  for the metric f
-000048b0: 756e 6374 696f 6e2e 0a0a 2020 2020 2020  unction...      
-000048c0: 2020 2020 2020 2e2e 2076 6572 7369 6f6e        .. version
-000048d0: 6164 6465 643a 3a20 312e 310a 0a20 2020  added:: 1.1..   
-000048e0: 2020 2020 2069 6e69 7420 3a20 7b22 7261       init : {"ra
-000048f0: 6e64 6f6d 222c 2022 7063 6122 7d20 6f72  ndom", "pca"} or
-00004900: 206e 6461 7272 6179 206f 6620 7368 6170   ndarray of shap
-00004910: 6520 286e 5f73 616d 706c 6573 2c20 6e5f  e (n_samples, n_
-00004920: 636f 6d70 6f6e 656e 7473 292c 205c 0a20  components), \. 
-00004930: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00004940: 6566 6175 6c74 3d22 7063 6122 0a20 2020  efault="pca".   
-00004950: 2020 2020 2020 2020 2049 6e69 7469 616c           Initial
-00004960: 697a 6174 696f 6e20 6f66 2065 6d62 6564  ization of embed
-00004970: 6469 6e67 2e0a 2020 2020 2020 2020 2020  ding..          
-00004980: 2020 5043 4120 696e 6974 6961 6c69 7a61    PCA initializa
-00004990: 7469 6f6e 2063 616e 6e6f 7420 6265 2075  tion cannot be u
-000049a0: 7365 6420 7769 7468 2070 7265 636f 6d70  sed with precomp
-000049b0: 7574 6564 2064 6973 7461 6e63 6573 2061  uted distances a
-000049c0: 6e64 2069 730a 2020 2020 2020 2020 2020  nd is.          
-000049d0: 2020 7573 7561 6c6c 7920 6d6f 7265 2067    usually more g
-000049e0: 6c6f 6261 6c6c 7920 7374 6162 6c65 2074  lobally stable t
-000049f0: 6861 6e20 7261 6e64 6f6d 2069 6e69 7469  han random initi
-00004a00: 616c 697a 6174 696f 6e2e 0a0a 2020 2020  alization...    
-00004a10: 2020 2020 2020 2020 2e2e 2076 6572 7369          .. versi
-00004a20: 6f6e 6368 616e 6765 643a 3a20 312e 320a  onchanged:: 1.2.
-00004a30: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00004a40: 6465 6661 756c 7420 7661 6c75 6520 6368  default value ch
-00004a50: 616e 6765 6420 746f 2060 2270 6361 2260  anged to `"pca"`
-00004a60: 2e0a 0a20 2020 2020 2020 2076 6572 626f  ...        verbo
-00004a70: 7365 203a 2069 6e74 2c20 6465 6661 756c  se : int, defaul
-00004a80: 743d 300a 2020 2020 2020 2020 2020 2020  t=0.            
-00004a90: 5665 7262 6f73 6974 7920 6c65 7665 6c2e  Verbosity level.
-00004aa0: 0a0a 2020 2020 2020 2020 7261 6e64 6f6d  ..        random
-00004ab0: 5f73 7461 7465 203a 2069 6e74 2c20 5261  _state : int, Ra
-00004ac0: 6e64 6f6d 5374 6174 6520 696e 7374 616e  ndomState instan
-00004ad0: 6365 206f 7220 4e6f 6e65 2c20 6465 6661  ce or None, defa
-00004ae0: 756c 743d 4e6f 6e65 0a20 2020 2020 2020  ult=None.       
-00004af0: 2020 2020 2044 6574 6572 6d69 6e65 7320       Determines 
-00004b00: 7468 6520 7261 6e64 6f6d 206e 756d 6265  the random numbe
-00004b10: 7220 6765 6e65 7261 746f 722e 2050 6173  r generator. Pas
-00004b20: 7320 616e 2069 6e74 2066 6f72 2072 6570  s an int for rep
-00004b30: 726f 6475 6369 626c 650a 2020 2020 2020  roducible.      
-00004b40: 2020 2020 2020 7265 7375 6c74 7320 6163        results ac
-00004b50: 726f 7373 206d 756c 7469 706c 6520 6675  ross multiple fu
-00004b60: 6e63 7469 6f6e 2063 616c 6c73 2e20 4e6f  nction calls. No
-00004b70: 7465 2074 6861 7420 6469 6666 6572 656e  te that differen
-00004b80: 740a 2020 2020 2020 2020 2020 2020 696e  t.            in
-00004b90: 6974 6961 6c69 7a61 7469 6f6e 7320 6d69  itializations mi
-00004ba0: 6768 7420 7265 7375 6c74 2069 6e20 6469  ght result in di
-00004bb0: 6666 6572 656e 7420 6c6f 6361 6c20 6d69  fferent local mi
-00004bc0: 6e69 6d61 206f 6620 7468 6520 636f 7374  nima of the cost
-00004bd0: 0a20 2020 2020 2020 2020 2020 2066 756e  .            fun
-00004be0: 6374 696f 6e2e 2053 6565 203a 7465 726d  ction. See :term
-00004bf0: 3a60 476c 6f73 7361 7279 203c 7261 6e64  :`Glossary <rand
-00004c00: 6f6d 5f73 7461 7465 3e60 2e0a 0a20 2020  om_state>`...   
-00004c10: 2020 2020 206d 6574 686f 6420 3a20 7b27       method : {'
-00004c20: 6261 726e 6573 5f68 7574 272c 2027 6578  barnes_hut', 'ex
-00004c30: 6163 7427 7d2c 2064 6566 6175 6c74 3d27  act'}, default='
-00004c40: 6261 726e 6573 5f68 7574 270a 2020 2020  barnes_hut'.    
-00004c50: 2020 2020 2020 2020 4279 2064 6566 6175          By defau
-00004c60: 6c74 2074 6865 2067 7261 6469 656e 7420  lt the gradient 
-00004c70: 6361 6c63 756c 6174 696f 6e20 616c 676f  calculation algo
-00004c80: 7269 7468 6d20 7573 6573 2042 6172 6e65  rithm uses Barne
-00004c90: 732d 4875 740a 2020 2020 2020 2020 2020  s-Hut.          
-00004ca0: 2020 6170 7072 6f78 696d 6174 696f 6e20    approximation 
-00004cb0: 7275 6e6e 696e 6720 696e 204f 284e 6c6f  running in O(Nlo
-00004cc0: 674e 2920 7469 6d65 2e20 6d65 7468 6f64  gN) time. method
-00004cd0: 3d27 6578 6163 7427 0a20 2020 2020 2020  ='exact'.       
-00004ce0: 2020 2020 2077 696c 6c20 7275 6e20 6f6e       will run on
-00004cf0: 2074 6865 2073 6c6f 7765 722c 2062 7574   the slower, but
-00004d00: 2065 7861 6374 2c20 616c 676f 7269 7468   exact, algorith
-00004d10: 6d20 696e 204f 284e 5e32 2920 7469 6d65  m in O(N^2) time
-00004d20: 2e20 5468 650a 2020 2020 2020 2020 2020  . The.          
-00004d30: 2020 6578 6163 7420 616c 676f 7269 7468    exact algorith
-00004d40: 6d20 7368 6f75 6c64 2062 6520 7573 6564  m should be used
-00004d50: 2077 6865 6e20 6e65 6172 6573 742d 6e65   when nearest-ne
-00004d60: 6967 6862 6f72 2065 7272 6f72 7320 6e65  ighbor errors ne
-00004d70: 6564 0a20 2020 2020 2020 2020 2020 2074  ed.            t
-00004d80: 6f20 6265 2062 6574 7465 7220 7468 616e  o be better than
-00004d90: 2033 252e 2048 6f77 6576 6572 2c20 7468   3%. However, th
-00004da0: 6520 6578 6163 7420 6d65 7468 6f64 2063  e exact method c
-00004db0: 616e 6e6f 7420 7363 616c 6520 746f 0a20  annot scale to. 
-00004dc0: 2020 2020 2020 2020 2020 206d 696c 6c69             milli
-00004dd0: 6f6e 7320 6f66 2065 7861 6d70 6c65 732e  ons of examples.
-00004de0: 0a0a 2020 2020 2020 2020 2020 2020 2e2e  ..            ..
-00004df0: 2076 6572 7369 6f6e 6164 6465 643a 3a20   versionadded:: 
-00004e00: 302e 3137 0a20 2020 2020 2020 2020 2020  0.17.           
-00004e10: 2041 7070 726f 7869 6d61 7465 206f 7074   Approximate opt
-00004e20: 696d 697a 6174 696f 6e20 2a6d 6574 686f  imization *metho
-00004e30: 642a 2076 6961 2074 6865 2042 6172 6e65  d* via the Barne
-00004e40: 732d 4875 742e 0a0a 2020 2020 2020 2020  s-Hut...        
-00004e50: 616e 676c 6520 3a20 666c 6f61 742c 2064  angle : float, d
-00004e60: 6566 6175 6c74 3d30 2e35 0a20 2020 2020  efault=0.5.     
-00004e70: 2020 2020 2020 204f 6e6c 7920 7573 6564         Only used
-00004e80: 2069 6620 6d65 7468 6f64 3d27 6261 726e   if method='barn
-00004e90: 6573 5f68 7574 270a 2020 2020 2020 2020  es_hut'.        
-00004ea0: 2020 2020 5468 6973 2069 7320 7468 6520      This is the 
-00004eb0: 7472 6164 652d 6f66 6620 6265 7477 6565  trade-off betwee
-00004ec0: 6e20 7370 6565 6420 616e 6420 6163 6375  n speed and accu
-00004ed0: 7261 6379 2066 6f72 2042 6172 6e65 732d  racy for Barnes-
-00004ee0: 4875 7420 542d 534e 452e 0a20 2020 2020  Hut T-SNE..     
-00004ef0: 2020 2020 2020 2027 616e 676c 6527 2069         'angle' i
-00004f00: 7320 7468 6520 616e 6775 6c61 7220 7369  s the angular si
-00004f10: 7a65 2028 7265 6665 7272 6564 2074 6f20  ze (referred to 
-00004f20: 6173 2074 6865 7461 2069 6e20 5b33 5d29  as theta in [3])
-00004f30: 206f 6620 6120 6469 7374 616e 740a 2020   of a distant.  
-00004f40: 2020 2020 2020 2020 2020 6e6f 6465 2061            node a
-00004f50: 7320 6d65 6173 7572 6564 2066 726f 6d20  s measured from 
-00004f60: 6120 706f 696e 742e 2049 6620 7468 6973  a point. If this
-00004f70: 2073 697a 6520 6973 2062 656c 6f77 2027   size is below '
-00004f80: 616e 676c 6527 2074 6865 6e20 6974 2069  angle' then it i
-00004f90: 730a 2020 2020 2020 2020 2020 2020 7573  s.            us
-00004fa0: 6564 2061 7320 6120 7375 6d6d 6172 7920  ed as a summary 
-00004fb0: 6e6f 6465 206f 6620 616c 6c20 706f 696e  node of all poin
-00004fc0: 7473 2063 6f6e 7461 696e 6564 2077 6974  ts contained wit
-00004fd0: 6869 6e20 6974 2e0a 2020 2020 2020 2020  hin it..        
-00004fe0: 2020 2020 5468 6973 206d 6574 686f 6420      This method 
-00004ff0: 6973 206e 6f74 2076 6572 7920 7365 6e73  is not very sens
-00005000: 6974 6976 6520 746f 2063 6861 6e67 6573  itive to changes
-00005010: 2069 6e20 7468 6973 2070 6172 616d 6574   in this paramet
-00005020: 6572 0a20 2020 2020 2020 2020 2020 2069  er.            i
-00005030: 6e20 7468 6520 7261 6e67 6520 6f66 2030  n the range of 0
-00005040: 2e32 202d 2030 2e38 2e20 416e 676c 6520  .2 - 0.8. Angle 
-00005050: 6c65 7373 2074 6861 6e20 302e 3220 6861  less than 0.2 ha
-00005060: 7320 7175 6963 6b6c 7920 696e 6372 6561  s quickly increa
-00005070: 7369 6e67 0a20 2020 2020 2020 2020 2020  sing.           
-00005080: 2063 6f6d 7075 7461 7469 6f6e 2074 696d   computation tim
-00005090: 6520 616e 6420 616e 676c 6520 6772 6561  e and angle grea
-000050a0: 7465 7220 302e 3820 6861 7320 7175 6963  ter 0.8 has quic
-000050b0: 6b6c 7920 696e 6372 6561 7369 6e67 2065  kly increasing e
-000050c0: 7272 6f72 2e0a 0a20 2020 2020 2020 206e  rror...        n
-000050d0: 5f6a 6f62 7320 3a20 696e 742c 2064 6566  _jobs : int, def
-000050e0: 6175 6c74 3d4e 6f6e 650a 2020 2020 2020  ault=None.      
-000050f0: 2020 2020 2020 5468 6520 6e75 6d62 6572        The number
-00005100: 206f 6620 7061 7261 6c6c 656c 206a 6f62   of parallel job
-00005110: 7320 746f 2072 756e 2066 6f72 206e 6569  s to run for nei
-00005120: 6768 626f 7273 2073 6561 7263 682e 2054  ghbors search. T
-00005130: 6869 7320 7061 7261 6d65 7465 720a 2020  his parameter.  
-00005140: 2020 2020 2020 2020 2020 6861 7320 6e6f            has no
-00005150: 2069 6d70 6163 7420 7768 656e 2060 606d   impact when ``m
-00005160: 6574 7269 633d 2270 7265 636f 6d70 7574  etric="precomput
-00005170: 6564 2260 6020 6f72 0a20 2020 2020 2020  ed"`` or.       
-00005180: 2020 2020 2028 6060 6d65 7472 6963 3d22       (``metric="
-00005190: 6575 636c 6964 6561 6e22 6060 2061 6e64  euclidean"`` and
-000051a0: 2060 606d 6574 686f 643d 2265 7861 6374   ``method="exact
-000051b0: 2260 6029 2e0a 2020 2020 2020 2020 2020  "``)..          
-000051c0: 2020 6060 4e6f 6e65 6060 206d 6561 6e73    ``None`` means
-000051d0: 2031 2075 6e6c 6573 7320 696e 2061 203a   1 unless in a :
-000051e0: 6f62 6a3a 606a 6f62 6c69 622e 7061 7261  obj:`joblib.para
-000051f0: 6c6c 656c 5f62 6163 6b65 6e64 6020 636f  llel_backend` co
-00005200: 6e74 6578 742e 0a20 2020 2020 2020 2020  ntext..         
-00005210: 2020 2060 602d 3160 6020 6d65 616e 7320     ``-1`` means 
-00005220: 7573 696e 6720 616c 6c20 7072 6f63 6573  using all proces
-00005230: 736f 7273 2e20 5365 6520 3a74 6572 6d3a  sors. See :term:
-00005240: 6047 6c6f 7373 6172 7920 3c6e 5f6a 6f62  `Glossary <n_job
-00005250: 733e 600a 2020 2020 2020 2020 2020 2020  s>`.            
-00005260: 666f 7220 6d6f 7265 2064 6574 6169 6c73  for more details
-00005270: 2e0a 0a20 2020 2020 2020 2020 2020 202e  ...            .
-00005280: 2e20 7665 7273 696f 6e61 6464 6564 3a3a  . versionadded::
-00005290: 2030 2e32 320a 0a20 2020 2020 2020 2073   0.22..        s
-000052a0: 7175 6172 655f 6469 7374 616e 6365 7320  quare_distances 
-000052b0: 3a20 5472 7565 2c20 6465 6661 756c 743d  : True, default=
-000052c0: 2764 6570 7265 6361 7465 6427 0a20 2020  'deprecated'.   
-000052d0: 2020 2020 2020 2020 2054 6869 7320 7061           This pa
-000052e0: 7261 6d65 7465 7220 6861 7320 6e6f 2065  rameter has no e
-000052f0: 6666 6563 7420 7369 6e63 6520 6469 7374  ffect since dist
-00005300: 616e 6365 2076 616c 7565 7320 6172 6520  ance values are 
-00005310: 616c 7761 7973 2073 7175 6172 6564 0a20  always squared. 
-00005320: 2020 2020 2020 2020 2020 2073 696e 6365             since
-00005330: 2031 2e31 2e0a 0a20 2020 2020 2020 2020   1.1...         
-00005340: 2020 202e 2e20 6465 7072 6563 6174 6564     .. deprecated
-00005350: 3a3a 2031 2e31 0a20 2020 2020 2020 2020  :: 1.1.         
-00005360: 2020 2020 2020 2060 7371 7561 7265 5f64         `square_d
-00005370: 6973 7461 6e63 6573 6020 6861 7320 6e6f  istances` has no
-00005380: 2065 6666 6563 7420 6672 6f6d 2031 2e31   effect from 1.1
-00005390: 2061 6e64 2077 696c 6c20 6265 2072 656d   and will be rem
-000053a0: 6f76 6564 2069 6e0a 2020 2020 2020 2020  oved in.        
-000053b0: 2020 2020 2020 2020 312e 332e 0a0a 2020          1.3...  
-000053c0: 2020 2020 2020 5265 6665 7265 6e63 6573        References
-000053d0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-000053e0: 2d2d 2d0a 2020 2020 2020 2020 5363 696b  ---.        Scik
-000053f0: 6974 2d6c 6561 726e 2041 5049 3a20 736b  it-learn API: sk
-00005400: 6c65 6172 6e2e 6d61 6e69 666f 6c64 2e54  learn.manifold.T
-00005410: 534e 450a 2020 2020 2020 2020 6874 7470  SNE.        http
-00005420: 733a 2f2f 7363 696b 6974 2d6c 6561 726e  s://scikit-learn
-00005430: 2e6f 7267 2f73 7461 626c 652f 6d6f 6475  .org/stable/modu
-00005440: 6c65 732f 6765 6e65 7261 7465 642f 736b  les/generated/sk
-00005450: 6c65 6172 6e2e 6d61 6e69 666f 6c64 2e54  learn.manifold.T
-00005460: 534e 452e 6874 6d6c 0a20 2020 2020 2020  SNE.html.       
-00005470: 2022 2222 0a20 2020 2020 2020 2073 7570   """.        sup
-00005480: 6572 2829 2e5f 5f69 6e69 745f 5f28 290a  er().__init__().
-00005490: 2020 2020 2020 2020 7365 6c66 2e6e 5f63          self.n_c
-000054a0: 6f6d 706f 6e65 6e74 7320 3d20 6e5f 636f  omponents = n_co
-000054b0: 6d70 6f6e 656e 7473 0a20 2020 2020 2020  mponents.       
-000054c0: 2073 656c 662e 7065 7270 6c65 7869 7479   self.perplexity
-000054d0: 203d 2070 6572 706c 6578 6974 790a 2020   = perplexity.  
-000054e0: 2020 2020 2020 7365 6c66 2e65 6172 6c79        self.early
-000054f0: 5f65 7861 6767 6572 6174 696f 6e20 3d20  _exaggeration = 
-00005500: 6561 726c 795f 6578 6167 6765 7261 7469  early_exaggerati
-00005510: 6f6e 0a20 2020 2020 2020 2073 656c 662e  on.        self.
-00005520: 6c65 6172 6e69 6e67 5f72 6174 6520 3d20  learning_rate = 
-00005530: 6c65 6172 6e69 6e67 5f72 6174 650a 2020  learning_rate.  
-00005540: 2020 2020 2020 7365 6c66 2e6e 5f69 7465        self.n_ite
-00005550: 7220 3d20 6e5f 6974 6572 0a20 2020 2020  r = n_iter.     
-00005560: 2020 2073 656c 662e 6e5f 6974 6572 5f77     self.n_iter_w
-00005570: 6974 686f 7574 5f70 726f 6772 6573 7320  ithout_progress 
-00005580: 3d20 6e5f 6974 6572 5f77 6974 686f 7574  = n_iter_without
-00005590: 5f70 726f 6772 6573 730a 2020 2020 2020  _progress.      
-000055a0: 2020 7365 6c66 2e6d 696e 5f67 7261 645f    self.min_grad_
-000055b0: 6e6f 726d 203d 206d 696e 5f67 7261 645f  norm = min_grad_
-000055c0: 6e6f 726d 0a20 2020 2020 2020 2073 656c  norm.        sel
-000055d0: 662e 6d65 7472 6963 203d 206d 6574 7269  f.metric = metri
-000055e0: 630a 2020 2020 2020 2020 7365 6c66 2e6d  c.        self.m
-000055f0: 6574 7269 635f 7061 7261 6d73 203d 206d  etric_params = m
-00005600: 6574 7269 635f 7061 7261 6d73 0a20 2020  etric_params.   
-00005610: 2020 2020 2073 656c 662e 696e 6974 203d       self.init =
-00005620: 2069 6e69 740a 2020 2020 2020 2020 7365   init.        se
-00005630: 6c66 2e76 6572 626f 7365 203d 2076 6572  lf.verbose = ver
-00005640: 626f 7365 0a20 2020 2020 2020 2073 656c  bose.        sel
-00005650: 662e 6d65 7468 6f64 203d 206d 6574 686f  f.method = metho
-00005660: 640a 2020 2020 2020 2020 7365 6c66 2e61  d.        self.a
-00005670: 6e67 6c65 203d 2061 6e67 6c65 0a20 2020  ngle = angle.   
-00005680: 2020 2020 2073 656c 662e 6e5f 6a6f 6273       self.n_jobs
-00005690: 203d 206e 5f6a 6f62 730a 2020 2020 2020   = n_jobs.      
-000056a0: 2020 7365 6c66 2e73 7175 6172 655f 6469    self.square_di
-000056b0: 7374 616e 6365 7320 3d20 7371 7561 7265  stances = square
-000056c0: 5f64 6973 7461 6e63 6573 0a0a 2020 2020  _distances..    
-000056d0: 2020 2020 6966 2072 616e 646f 6d5f 7374      if random_st
-000056e0: 6174 653a 0a20 2020 2020 2020 2020 2020  ate:.           
-000056f0: 2073 656c 662e 7261 6e64 6f6d 5f73 7461   self.random_sta
-00005700: 7465 203d 2072 616e 646f 6d5f 7374 6174  te = random_stat
-00005710: 650a 0a20 2020 2020 2020 2023 2049 6620  e..        # If 
-00005720: 2772 616e 646f 6d5f 7374 6174 6527 2069  'random_state' i
-00005730: 7320 4e6f 6e65 2c20 2773 656c 662e 7261  s None, 'self.ra
-00005740: 6e64 6f6d 5f73 7461 7465 2720 636f 6d65  ndom_state' come
-00005750: 7320 6672 6f6d 2074 6865 2070 6172 656e  s from the paren
-00005760: 7420 636c 6173 7320 2757 6f72 6b66 6c6f  t class 'Workflo
-00005770: 7742 6173 6527 0a20 2020 2020 2020 2073  wBase'.        s
-00005780: 656c 662e 6d6f 6465 6c20 3d20 5453 4e45  elf.model = TSNE
-00005790: 280a 2020 2020 2020 2020 2020 2020 6e5f  (.            n_
-000057a0: 636f 6d70 6f6e 656e 7473 3d73 656c 662e  components=self.
-000057b0: 6e5f 636f 6d70 6f6e 656e 7473 2c0a 2020  n_components,.  
-000057c0: 2020 2020 2020 2020 2020 7065 7270 6c65            perple
-000057d0: 7869 7479 3d73 656c 662e 7065 7270 6c65  xity=self.perple
-000057e0: 7869 7479 2c0a 2020 2020 2020 2020 2020  xity,.          
-000057f0: 2020 6561 726c 795f 6578 6167 6765 7261    early_exaggera
-00005800: 7469 6f6e 3d73 656c 662e 6561 726c 795f  tion=self.early_
-00005810: 6578 6167 6765 7261 7469 6f6e 2c0a 2020  exaggeration,.  
-00005820: 2020 2020 2020 2020 2020 6c65 6172 6e69            learni
-00005830: 6e67 5f72 6174 653d 7365 6c66 2e6c 6561  ng_rate=self.lea
-00005840: 726e 696e 675f 7261 7465 2c0a 2020 2020  rning_rate,.    
-00005850: 2020 2020 2020 2020 6e5f 6974 6572 3d73          n_iter=s
-00005860: 656c 662e 6e5f 6974 6572 2c0a 2020 2020  elf.n_iter,.    
-00005870: 2020 2020 2020 2020 6e5f 6974 6572 5f77          n_iter_w
-00005880: 6974 686f 7574 5f70 726f 6772 6573 733d  ithout_progress=
-00005890: 7365 6c66 2e6e 5f69 7465 725f 7769 7468  self.n_iter_with
-000058a0: 6f75 745f 7072 6f67 7265 7373 2c0a 2020  out_progress,.  
-000058b0: 2020 2020 2020 2020 2020 6d69 6e5f 6772            min_gr
-000058c0: 6164 5f6e 6f72 6d3d 7365 6c66 2e6d 696e  ad_norm=self.min
-000058d0: 5f67 7261 645f 6e6f 726d 2c0a 2020 2020  _grad_norm,.    
-000058e0: 2020 2020 2020 2020 6d65 7472 6963 3d73          metric=s
-000058f0: 656c 662e 6d65 7472 6963 2c0a 2020 2020  elf.metric,.    
-00005900: 2020 2020 2020 2020 6d65 7472 6963 5f70          metric_p
-00005910: 6172 616d 733d 7365 6c66 2e6d 6574 7269  arams=self.metri
-00005920: 635f 7061 7261 6d73 2c0a 2020 2020 2020  c_params,.      
-00005930: 2020 2020 2020 696e 6974 3d73 656c 662e        init=self.
-00005940: 696e 6974 2c0a 2020 2020 2020 2020 2020  init,.          
-00005950: 2020 7665 7262 6f73 653d 7365 6c66 2e76    verbose=self.v
-00005960: 6572 626f 7365 2c0a 2020 2020 2020 2020  erbose,.        
-00005970: 2020 2020 7261 6e64 6f6d 5f73 7461 7465      random_state
-00005980: 3d73 656c 662e 7261 6e64 6f6d 5f73 7461  =self.random_sta
-00005990: 7465 2c0a 2020 2020 2020 2020 2020 2020  te,.            
-000059a0: 6d65 7468 6f64 3d73 656c 662e 6d65 7468  method=self.meth
-000059b0: 6f64 2c0a 2020 2020 2020 2020 2020 2020  od,.            
-000059c0: 616e 676c 653d 7365 6c66 2e61 6e67 6c65  angle=self.angle
-000059d0: 2c0a 2020 2020 2020 2020 2020 2020 6e5f  ,.            n_
-000059e0: 6a6f 6273 3d73 656c 662e 6e5f 6a6f 6273  jobs=self.n_jobs
-000059f0: 2c0a 2020 2020 2020 2020 2020 2020 7371  ,.            sq
-00005a00: 7561 7265 5f64 6973 7461 6e63 6573 3d73  uare_distances=s
-00005a10: 656c 662e 7371 7561 7265 5f64 6973 7461  elf.square_dista
-00005a20: 6e63 6573 2c0a 2020 2020 2020 2020 290a  nces,.        ).
-00005a30: 0a20 2020 2020 2020 2073 656c 662e 6e61  .        self.na
-00005a40: 6d69 6e67 203d 2054 534e 4544 6563 6f6d  ming = TSNEDecom
-00005a50: 706f 7369 7469 6f6e 2e6e 616d 650a 0a20  position.name.. 
-00005a60: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
-00005a70: 2020 2020 6465 6620 6d61 6e75 616c 5f68      def manual_h
-00005a80: 7970 6572 5f70 6172 616d 6574 6572 7328  yper_parameters(
-00005a90: 636c 7329 202d 3e20 4469 6374 3a0a 2020  cls) -> Dict:.  
-00005aa0: 2020 2020 2020 2222 224d 616e 7561 6c20        """Manual 
-00005ab0: 6879 7065 722d 7061 7261 6d65 7465 7273  hyper-parameters
-00005ac0: 2073 7065 6369 6669 6361 7469 6f6e 2e22   specification."
-00005ad0: 2222 0a20 2020 2020 2020 2070 7269 6e74  "".        print
-00005ae0: 2866 222d 2a2d 2a2d 207b 636c 732e 6e61  (f"-*-*- {cls.na
-00005af0: 6d65 7d20 2d20 4879 7065 722d 7061 7261  me} - Hyper-para
-00005b00: 6d65 7465 7273 2053 7065 6369 6669 6361  meters Specifica
-00005b10: 7469 6f6e 202d 2a2d 2a2d 2229 0a20 2020  tion -*-*-").   
-00005b20: 2020 2020 2068 7970 6572 5f70 6172 616d       hyper_param
-00005b30: 6574 6572 7320 3d20 7473 6e65 5f6d 616e  eters = tsne_man
-00005b40: 7561 6c5f 6879 7065 725f 7061 7261 6d65  ual_hyper_parame
-00005b50: 7465 7273 2829 0a20 2020 2020 2020 2063  ters().        c
-00005b60: 6c65 6172 5f6f 7574 7075 7428 290a 2020  lear_output().  
-00005b70: 2020 2020 2020 7265 7475 726e 2068 7970        return hyp
-00005b80: 6572 5f70 6172 616d 6574 6572 730a 0a20  er_parameters.. 
-00005b90: 2020 2064 6566 2073 7065 6369 616c 5f63     def special_c
-00005ba0: 6f6d 706f 6e65 6e74 7328 7365 6c66 2c20  omponents(self, 
-00005bb0: 2a2a 6b77 6172 6773 2920 2d3e 204e 6f6e  **kwargs) -> Non
-00005bc0: 653a 0a20 2020 2020 2020 2022 2222 496e  e:.        """In
-00005bd0: 766f 6b65 2061 6c6c 2073 7065 6369 616c  voke all special
-00005be0: 2061 7070 6c69 6361 7469 6f6e 2066 756e   application fun
-00005bf0: 6374 696f 6e73 2066 6f72 2074 6869 7320  ctions for this 
-00005c00: 616c 676f 7269 7468 6d73 2062 7920 5363  algorithms by Sc
-00005c10: 696b 6974 2d6c 6561 726e 2066 7261 6d65  ikit-learn frame
-00005c20: 776f 726b 2e22 2222 0a20 2020 2020 2020  work.""".       
-00005c30: 2070 6173 730a 0a0a 636c 6173 7320 4d44   pass...class MD
-00005c40: 5344 6563 6f6d 706f 7369 7469 6f6e 2844  SDecomposition(D
-00005c50: 6563 6f6d 706f 7369 7469 6f6e 576f 726b  ecompositionWork
-00005c60: 666c 6f77 4261 7365 293a 0a20 2020 2022  flowBase):.    "
-00005c70: 2222 5468 6520 6175 746f 6d61 7469 6f6e  ""The automation
-00005c80: 2077 6f72 6b66 6c6f 7720 6f66 2075 7369   workflow of usi
-00005c90: 6e67 204d 4453 2061 6c67 6f72 6974 686d  ng MDS algorithm
-00005ca0: 2074 6f20 6d61 6b65 2069 6e73 6967 6874   to make insight
-00005cb0: 6675 6c20 7072 6f64 7563 7473 2e22 2222  ful products."""
-00005cc0: 0a0a 2020 2020 6e61 6d65 203d 2022 4d44  ..    name = "MD
-00005cd0: 5322 0a20 2020 2073 7065 6369 616c 5f66  S".    special_f
-00005ce0: 756e 6374 696f 6e20 3d20 5b5d 0a0a 2020  unction = []..  
-00005cf0: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
-00005d00: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00005d10: 2020 2020 2020 6e5f 636f 6d70 6f6e 656e        n_componen
-00005d20: 7473 3a20 696e 7420 3d20 322c 0a20 2020  ts: int = 2,.   
-00005d30: 2020 2020 202a 2c0a 2020 2020 2020 2020       *,.        
-00005d40: 6d65 7472 6963 3a20 626f 6f6c 203d 2054  metric: bool = T
-00005d50: 7275 652c 0a20 2020 2020 2020 206e 5f69  rue,.        n_i
-00005d60: 6e69 743a 2069 6e74 203d 2034 2c0a 2020  nit: int = 4,.  
-00005d70: 2020 2020 2020 6d61 785f 6974 6572 3a20        max_iter: 
-00005d80: 696e 7420 3d20 3330 302c 0a20 2020 2020  int = 300,.     
-00005d90: 2020 2076 6572 626f 7365 3a20 696e 7420     verbose: int 
-00005da0: 3d20 302c 0a20 2020 2020 2020 2065 7073  = 0,.        eps
-00005db0: 3a20 666c 6f61 7420 3d20 3165 2d33 2c0a  : float = 1e-3,.
-00005dc0: 2020 2020 2020 2020 6e5f 6a6f 6273 3a20          n_jobs: 
-00005dd0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
-00005de0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7261  None,.        ra
-00005df0: 6e64 6f6d 5f73 7461 7465 3a20 4f70 7469  ndom_state: Opti
-00005e00: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-00005e10: 2c0a 2020 2020 2020 2020 6469 7373 696d  ,.        dissim
-00005e20: 696c 6172 6974 793a 2073 7472 203d 2022  ilarity: str = "
-00005e30: 6575 636c 6964 6561 6e22 2c0a 2020 2020  euclidean",.    
-00005e40: 2020 2020 2320 6e6f 726d 616c 697a 6564      # normalized
-00005e50: 5f73 7472 6573 733d 2277 6172 6e22 2c0a  _stress="warn",.
-00005e60: 2020 2020 2920 2d3e 204e 6f6e 653a 0a20      ) -> None:. 
-00005e70: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00005e80: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-00005e90: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-00005ea0: 0a20 2020 2020 2020 206e 5f63 6f6d 706f  .        n_compo
-00005eb0: 6e65 6e74 7320 3a20 696e 742c 2064 6566  nents : int, def
-00005ec0: 6175 6c74 3d32 0a20 2020 2020 2020 2020  ault=2.         
-00005ed0: 2020 204e 756d 6265 7220 6f66 2064 696d     Number of dim
-00005ee0: 656e 7369 6f6e 7320 696e 2077 6869 6368  ensions in which
-00005ef0: 2074 6f20 696d 6d65 7273 6520 7468 6520   to immerse the 
-00005f00: 6469 7373 696d 696c 6172 6974 6965 732e  dissimilarities.
-00005f10: 0a0a 2020 2020 2020 2020 6d65 7472 6963  ..        metric
-00005f20: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
-00005f30: 3d54 7275 650a 2020 2020 2020 2020 2020  =True.          
-00005f40: 2020 4966 2060 6054 7275 6560 602c 2070    If ``True``, p
-00005f50: 6572 666f 726d 206d 6574 7269 6320 4d44  erform metric MD
-00005f60: 533b 206f 7468 6572 7769 7365 2c20 7065  S; otherwise, pe
-00005f70: 7266 6f72 6d20 6e6f 6e6d 6574 7269 6320  rform nonmetric 
-00005f80: 4d44 532e 0a20 2020 2020 2020 2020 2020  MDS..           
-00005f90: 2057 6865 6e20 6060 4661 6c73 6560 6020   When ``False`` 
-00005fa0: 2869 2e65 2e20 6e6f 6e2d 6d65 7472 6963  (i.e. non-metric
-00005fb0: 204d 4453 292c 2064 6973 7369 6d69 6c61   MDS), dissimila
-00005fc0: 7269 7469 6573 2077 6974 6820 3020 6172  rities with 0 ar
-00005fd0: 6520 636f 6e73 6964 6572 6564 2061 730a  e considered as.
-00005fe0: 2020 2020 2020 2020 2020 2020 6d69 7373              miss
-00005ff0: 696e 6720 7661 6c75 6573 2e0a 0a20 2020  ing values...   
-00006000: 2020 2020 206e 5f69 6e69 7420 3a20 696e       n_init : in
-00006010: 742c 2064 6566 6175 6c74 3d34 0a20 2020  t, default=4.   
-00006020: 2020 2020 2020 2020 204e 756d 6265 7220           Number 
-00006030: 6f66 2074 696d 6573 2074 6865 2053 4d41  of times the SMA
-00006040: 434f 4620 616c 676f 7269 7468 6d20 7769  COF algorithm wi
-00006050: 6c6c 2062 6520 7275 6e20 7769 7468 2064  ll be run with d
-00006060: 6966 6665 7265 6e74 0a20 2020 2020 2020  ifferent.       
-00006070: 2020 2020 2069 6e69 7469 616c 697a 6174       initializat
-00006080: 696f 6e73 2e20 5468 6520 6669 6e61 6c20  ions. The final 
-00006090: 7265 7375 6c74 7320 7769 6c6c 2062 6520  results will be 
-000060a0: 7468 6520 6265 7374 206f 7574 7075 7420  the best output 
-000060b0: 6f66 2074 6865 2072 756e 732c 0a20 2020  of the runs,.   
-000060c0: 2020 2020 2020 2020 2064 6574 6572 6d69           determi
-000060d0: 6e65 6420 6279 2074 6865 2072 756e 2077  ned by the run w
-000060e0: 6974 6820 7468 6520 736d 616c 6c65 7374  ith the smallest
-000060f0: 2066 696e 616c 2073 7472 6573 732e 0a0a   final stress...
-00006100: 2020 2020 2020 2020 6d61 785f 6974 6572          max_iter
-00006110: 203a 2069 6e74 2c20 6465 6661 756c 743d   : int, default=
-00006120: 3330 300a 2020 2020 2020 2020 2020 2020  300.            
-00006130: 4d61 7869 6d75 6d20 6e75 6d62 6572 206f  Maximum number o
-00006140: 6620 6974 6572 6174 696f 6e73 206f 6620  f iterations of 
-00006150: 7468 6520 534d 4143 4f46 2061 6c67 6f72  the SMACOF algor
-00006160: 6974 686d 2066 6f72 2061 2073 696e 676c  ithm for a singl
-00006170: 6520 7275 6e2e 0a0a 2020 2020 2020 2020  e run...        
-00006180: 7665 7262 6f73 6520 3a20 696e 742c 2064  verbose : int, d
-00006190: 6566 6175 6c74 3d30 0a20 2020 2020 2020  efault=0.       
-000061a0: 2020 2020 204c 6576 656c 206f 6620 7665       Level of ve
-000061b0: 7262 6f73 6974 792e 0a0a 2020 2020 2020  rbosity...      
-000061c0: 2020 6570 7320 3a20 666c 6f61 742c 2064    eps : float, d
-000061d0: 6566 6175 6c74 3d31 652d 330a 2020 2020  efault=1e-3.    
-000061e0: 2020 2020 2020 2020 5265 6c61 7469 7665          Relative
-000061f0: 2074 6f6c 6572 616e 6365 2077 6974 6820   tolerance with 
-00006200: 7265 7370 6563 7420 746f 2073 7472 6573  respect to stres
-00006210: 7320 6174 2077 6869 6368 2074 6f20 6465  s at which to de
-00006220: 636c 6172 650a 2020 2020 2020 2020 2020  clare.          
-00006230: 2020 636f 6e76 6572 6765 6e63 652e 2054    convergence. T
-00006240: 6865 2076 616c 7565 206f 6620 6065 7073  he value of `eps
-00006250: 6020 7368 6f75 6c64 2062 6520 7475 6e65  ` should be tune
-00006260: 6420 7365 7061 7261 7465 6c79 2064 6570  d separately dep
-00006270: 656e 6469 6e67 0a20 2020 2020 2020 2020  ending.         
-00006280: 2020 206f 6e20 7768 6574 6865 7220 6f72     on whether or
-00006290: 206e 6f74 2060 6e6f 726d 616c 697a 6564   not `normalized
-000062a0: 5f73 7472 6573 7360 2069 7320 6265 696e  _stress` is bein
-000062b0: 6720 7573 6564 2e0a 0a20 2020 2020 2020  g used...       
-000062c0: 206e 5f6a 6f62 7320 3a20 696e 742c 2064   n_jobs : int, d
-000062d0: 6566 6175 6c74 3d4e 6f6e 650a 2020 2020  efault=None.    
-000062e0: 2020 2020 2020 2020 5468 6520 6e75 6d62          The numb
-000062f0: 6572 206f 6620 6a6f 6273 2074 6f20 7573  er of jobs to us
-00006300: 6520 666f 7220 7468 6520 636f 6d70 7574  e for the comput
-00006310: 6174 696f 6e2e 2049 6620 6d75 6c74 6970  ation. If multip
-00006320: 6c65 0a20 2020 2020 2020 2020 2020 2069  le.            i
-00006330: 6e69 7469 616c 697a 6174 696f 6e73 2061  nitializations a
-00006340: 7265 2075 7365 6420 2860 606e 5f69 6e69  re used (``n_ini
-00006350: 7460 6029 2c20 6561 6368 2072 756e 206f  t``), each run o
-00006360: 6620 7468 6520 616c 676f 7269 7468 6d20  f the algorithm 
-00006370: 6973 0a20 2020 2020 2020 2020 2020 2063  is.            c
-00006380: 6f6d 7075 7465 6420 696e 2070 6172 616c  omputed in paral
-00006390: 6c65 6c2e 0a0a 2020 2020 2020 2020 2020  lel...          
-000063a0: 2020 6060 4e6f 6e65 6060 206d 6561 6e73    ``None`` means
-000063b0: 2031 2075 6e6c 6573 7320 696e 2061 203a   1 unless in a :
-000063c0: 6f62 6a3a 606a 6f62 6c69 622e 7061 7261  obj:`joblib.para
-000063d0: 6c6c 656c 5f62 6163 6b65 6e64 6020 636f  llel_backend` co
-000063e0: 6e74 6578 742e 0a20 2020 2020 2020 2020  ntext..         
-000063f0: 2020 2060 602d 3160 6020 6d65 616e 7320     ``-1`` means 
-00006400: 7573 696e 6720 616c 6c20 7072 6f63 6573  using all proces
-00006410: 736f 7273 2e20 5365 6520 3a74 6572 6d3a  sors. See :term:
-00006420: 6047 6c6f 7373 6172 7920 3c6e 5f6a 6f62  `Glossary <n_job
-00006430: 733e 600a 2020 2020 2020 2020 2020 2020  s>`.            
-00006440: 666f 7220 6d6f 7265 2064 6574 6169 6c73  for more details
-00006450: 2e0a 0a20 2020 2020 2020 2072 616e 646f  ...        rando
-00006460: 6d5f 7374 6174 6520 3a20 696e 742c 2052  m_state : int, R
-00006470: 616e 646f 6d53 7461 7465 2069 6e73 7461  andomState insta
-00006480: 6e63 6520 6f72 204e 6f6e 652c 2064 6566  nce or None, def
-00006490: 6175 6c74 3d4e 6f6e 650a 2020 2020 2020  ault=None.      
-000064a0: 2020 2020 2020 4465 7465 726d 696e 6573        Determines
-000064b0: 2074 6865 2072 616e 646f 6d20 6e75 6d62   the random numb
-000064c0: 6572 2067 656e 6572 6174 6f72 2075 7365  er generator use
-000064d0: 6420 746f 2069 6e69 7469 616c 697a 6520  d to initialize 
-000064e0: 7468 6520 6365 6e74 6572 732e 0a20 2020  the centers..   
-000064f0: 2020 2020 2020 2020 2050 6173 7320 616e           Pass an
-00006500: 2069 6e74 2066 6f72 2072 6570 726f 6475   int for reprodu
-00006510: 6369 626c 6520 7265 7375 6c74 7320 6163  cible results ac
-00006520: 726f 7373 206d 756c 7469 706c 6520 6675  ross multiple fu
-00006530: 6e63 7469 6f6e 2063 616c 6c73 2e0a 2020  nction calls..  
-00006540: 2020 2020 2020 2020 2020 5365 6520 3a74            See :t
-00006550: 6572 6d3a 6047 6c6f 7373 6172 7920 3c72  erm:`Glossary <r
-00006560: 616e 646f 6d5f 7374 6174 653e 602e 0a0a  andom_state>`...
-00006570: 2020 2020 2020 2020 6469 7373 696d 696c          dissimil
-00006580: 6172 6974 7920 3a20 7b27 6575 636c 6964  arity : {'euclid
-00006590: 6561 6e27 2c20 2770 7265 636f 6d70 7574  ean', 'precomput
-000065a0: 6564 277d 2c20 6465 6661 756c 743d 2765  ed'}, default='e
-000065b0: 7563 6c69 6465 616e 270a 2020 2020 2020  uclidean'.      
-000065c0: 2020 2020 2020 4469 7373 696d 696c 6172        Dissimilar
-000065d0: 6974 7920 6d65 6173 7572 6520 746f 2075  ity measure to u
-000065e0: 7365 3a0a 0a20 2020 2020 2020 2020 2020  se:..           
-000065f0: 202d 2027 6575 636c 6964 6561 6e27 3a0a   - 'euclidean':.
-00006600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006610: 5061 6972 7769 7365 2045 7563 6c69 6465  Pairwise Euclide
-00006620: 616e 2064 6973 7461 6e63 6573 2062 6574  an distances bet
-00006630: 7765 656e 2070 6f69 6e74 7320 696e 2074  ween points in t
-00006640: 6865 2064 6174 6173 6574 2e0a 0a20 2020  he dataset...   
-00006650: 2020 2020 2020 2020 202d 2027 7072 6563           - 'prec
-00006660: 6f6d 7075 7465 6427 3a0a 2020 2020 2020  omputed':.      
-00006670: 2020 2020 2020 2020 2020 5072 652d 636f            Pre-co
-00006680: 6d70 7574 6564 2064 6973 7369 6d69 6c61  mputed dissimila
-00006690: 7269 7469 6573 2061 7265 2070 6173 7365  rities are passe
-000066a0: 6420 6469 7265 6374 6c79 2074 6f20 6060  d directly to ``
-000066b0: 6669 7460 6020 616e 640a 2020 2020 2020  fit`` and.      
-000066c0: 2020 2020 2020 2020 2020 6060 6669 745f            ``fit_
-000066d0: 7472 616e 7366 6f72 6d60 602e 0a0a 2020  transform``...  
-000066e0: 2020 2020 2020 6e6f 726d 616c 697a 6564        normalized
-000066f0: 5f73 7472 6573 7320 3a20 626f 6f6c 206f  _stress : bool o
-00006700: 7220 2261 7574 6f22 2064 6566 6175 6c74  r "auto" default
-00006710: 3d46 616c 7365 0a20 2020 2020 2020 2020  =False.         
-00006720: 2020 2057 6865 7468 6572 2075 7365 2061     Whether use a
-00006730: 6e64 2072 6574 7572 6e20 6e6f 726d 6564  nd return normed
-00006740: 2073 7472 6573 7320 7661 6c75 6520 2853   stress value (S
-00006750: 7472 6573 732d 3129 2069 6e73 7465 6164  tress-1) instead
-00006760: 206f 6620 7261 770a 2020 2020 2020 2020   of raw.        
-00006770: 2020 2020 7374 7265 7373 2063 616c 6375      stress calcu
-00006780: 6c61 7465 6420 6279 2064 6566 6175 6c74  lated by default
-00006790: 2e20 4f6e 6c79 2073 7570 706f 7274 6564  . Only supported
-000067a0: 2069 6e20 6e6f 6e2d 6d65 7472 6963 204d   in non-metric M
-000067b0: 4453 2e0a 0a20 2020 2020 2020 2020 2020  DS...           
-000067c0: 202e 2e20 7665 7273 696f 6e61 6464 6564   .. versionadded
-000067d0: 3a3a 2031 2e32 0a0a 2020 2020 2020 2020  :: 1.2..        
-000067e0: 5265 6665 7265 6e63 6573 0a20 2020 2020  References.     
-000067f0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00006800: 2020 2020 2020 5363 696b 6974 2d6c 6561        Scikit-lea
-00006810: 726e 2041 5049 3a20 736b 6c65 6172 6e2e  rn API: sklearn.
-00006820: 6d61 6e69 666f 6c64 2e4d 4453 0a20 2020  manifold.MDS.   
-00006830: 2020 2020 2068 7474 7073 3a2f 2f73 6369       https://sci
-00006840: 6b69 742d 6c65 6172 6e2e 6f72 672f 7374  kit-learn.org/st
-00006850: 6162 6c65 2f6d 6f64 756c 6573 2f67 656e  able/modules/gen
-00006860: 6572 6174 6564 2f73 6b6c 6561 726e 2e6d  erated/sklearn.m
-00006870: 616e 6966 6f6c 642e 4d44 532e 6874 6d6c  anifold.MDS.html
-00006880: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00006890: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
-000068a0: 6e69 745f 5f28 290a 2020 2020 2020 2020  nit__().        
-000068b0: 7365 6c66 2e6e 5f63 6f6d 706f 6e65 6e74  self.n_component
-000068c0: 7320 3d20 6e5f 636f 6d70 6f6e 656e 7473  s = n_components
-000068d0: 0a20 2020 2020 2020 2073 656c 662e 6d65  .        self.me
-000068e0: 7472 6963 203d 206d 6574 7269 630a 2020  tric = metric.  
-000068f0: 2020 2020 2020 7365 6c66 2e6e 5f69 6e69        self.n_ini
-00006900: 7420 3d20 6e5f 696e 6974 0a20 2020 2020  t = n_init.     
-00006910: 2020 2073 656c 662e 6d61 785f 6974 6572     self.max_iter
-00006920: 203d 206d 6178 5f69 7465 720a 2020 2020   = max_iter.    
-00006930: 2020 2020 7365 6c66 2e76 6572 626f 7365      self.verbose
-00006940: 203d 2076 6572 626f 7365 0a20 2020 2020   = verbose.     
-00006950: 2020 2073 656c 662e 6570 7320 3d20 6570     self.eps = ep
-00006960: 730a 2020 2020 2020 2020 7365 6c66 2e6e  s.        self.n
-00006970: 5f6a 6f62 7320 3d20 6e5f 6a6f 6273 0a20  _jobs = n_jobs. 
-00006980: 2020 2020 2020 2073 656c 662e 6469 7373         self.diss
-00006990: 696d 696c 6172 6974 7920 3d20 6469 7373  imilarity = diss
-000069a0: 696d 696c 6172 6974 790a 2020 2020 2020  imilarity.      
-000069b0: 2020 2320 7365 6c66 2e6e 6f72 6d61 6c69    # self.normali
-000069c0: 7a65 645f 7374 7265 7373 203d 206e 6f72  zed_stress = nor
-000069d0: 6d61 6c69 7a65 645f 7374 7265 7373 0a0a  malized_stress..
-000069e0: 2020 2020 2020 2020 6966 2072 616e 646f          if rando
-000069f0: 6d5f 7374 6174 653a 0a20 2020 2020 2020  m_state:.       
-00006a00: 2020 2020 2073 656c 662e 7261 6e64 6f6d       self.random
-00006a10: 5f73 7461 7465 203d 2072 616e 646f 6d5f  _state = random_
-00006a20: 7374 6174 650a 0a20 2020 2020 2020 2023  state..        #
-00006a30: 2049 6620 2772 616e 646f 6d5f 7374 6174   If 'random_stat
-00006a40: 6527 2069 7320 4e6f 6e65 2c20 2773 656c  e' is None, 'sel
-00006a50: 662e 7261 6e64 6f6d 5f73 7461 7465 2720  f.random_state' 
-00006a60: 636f 6d65 7320 6672 6f6d 2074 6865 2070  comes from the p
-00006a70: 6172 656e 7420 636c 6173 7320 2757 6f72  arent class 'Wor
-00006a80: 6b66 6c6f 7742 6173 6527 0a20 2020 2020  kflowBase'.     
-00006a90: 2020 2073 656c 662e 6d6f 6465 6c20 3d20     self.model = 
-00006aa0: 4d44 5328 0a20 2020 2020 2020 2020 2020  MDS(.           
-00006ab0: 206e 5f63 6f6d 706f 6e65 6e74 733d 7365   n_components=se
-00006ac0: 6c66 2e6e 5f63 6f6d 706f 6e65 6e74 732c  lf.n_components,
-00006ad0: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
-00006ae0: 7269 633d 7365 6c66 2e6d 6574 7269 632c  ric=self.metric,
-00006af0: 0a20 2020 2020 2020 2020 2020 206e 5f69  .            n_i
-00006b00: 6e69 743d 7365 6c66 2e6e 5f69 6e69 742c  nit=self.n_init,
-00006b10: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
-00006b20: 5f69 7465 723d 7365 6c66 2e6d 6178 5f69  _iter=self.max_i
-00006b30: 7465 722c 0a20 2020 2020 2020 2020 2020  ter,.           
-00006b40: 2076 6572 626f 7365 3d73 656c 662e 7665   verbose=self.ve
-00006b50: 7262 6f73 652c 0a20 2020 2020 2020 2020  rbose,.         
-00006b60: 2020 2065 7073 3d73 656c 662e 6570 732c     eps=self.eps,
-00006b70: 0a20 2020 2020 2020 2020 2020 206e 5f6a  .            n_j
-00006b80: 6f62 733d 7365 6c66 2e6e 5f6a 6f62 732c  obs=self.n_jobs,
-00006b90: 0a20 2020 2020 2020 2020 2020 2072 616e  .            ran
-00006ba0: 646f 6d5f 7374 6174 653d 7365 6c66 2e72  dom_state=self.r
-00006bb0: 616e 646f 6d5f 7374 6174 652c 0a20 2020  andom_state,.   
-00006bc0: 2020 2020 2020 2020 2064 6973 7369 6d69           dissimi
-00006bd0: 6c61 7269 7479 3d73 656c 662e 6469 7373  larity=self.diss
-00006be0: 696d 696c 6172 6974 792c 0a20 2020 2020  imilarity,.     
-00006bf0: 2020 2020 2020 2023 206e 6f72 6d61 6c69         # normali
-00006c00: 7a65 645f 7374 7265 7373 3d73 656c 662e  zed_stress=self.
-00006c10: 6e6f 726d 616c 697a 6564 5f73 7472 6573  normalized_stres
-00006c20: 732c 0a20 2020 2020 2020 2029 0a0a 2020  s,.        )..  
-00006c30: 2020 2020 2020 7365 6c66 2e6e 616d 696e        self.namin
-00006c40: 6720 3d20 4d44 5344 6563 6f6d 706f 7369  g = MDSDecomposi
-00006c50: 7469 6f6e 2e6e 616d 650a 0a20 2020 2040  tion.name..    @
-00006c60: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
-00006c70: 6465 6620 6d61 6e75 616c 5f68 7970 6572  def manual_hyper
-00006c80: 5f70 6172 616d 6574 6572 7328 636c 7329  _parameters(cls)
-00006c90: 202d 3e20 4469 6374 3a0a 2020 2020 2020   -> Dict:.      
-00006ca0: 2020 2222 224d 616e 7561 6c20 6879 7065    """Manual hype
-00006cb0: 722d 7061 7261 6d65 7465 7273 2073 7065  r-parameters spe
-00006cc0: 6369 6669 6361 7469 6f6e 2e22 2222 0a20  cification.""". 
-00006cd0: 2020 2020 2020 2070 7269 6e74 2866 222d         print(f"-
-00006ce0: 2a2d 2a2d 207b 636c 732e 6e61 6d65 7d20  *-*- {cls.name} 
-00006cf0: 2d20 4879 7065 722d 7061 7261 6d65 7465  - Hyper-paramete
-00006d00: 7273 2053 7065 6369 6669 6361 7469 6f6e  rs Specification
-00006d10: 202d 2a2d 2a2d 2229 0a20 2020 2020 2020   -*-*-").       
-00006d20: 2068 7970 6572 5f70 6172 616d 6574 6572   hyper_parameter
-00006d30: 7320 3d20 6d64 735f 6d61 6e75 616c 5f68  s = mds_manual_h
-00006d40: 7970 6572 5f70 6172 616d 6574 6572 7328  yper_parameters(
-00006d50: 290a 2020 2020 2020 2020 636c 6561 725f  ).        clear_
-00006d60: 6f75 7470 7574 2829 0a20 2020 2020 2020  output().       
-00006d70: 2072 6574 7572 6e20 6879 7065 725f 7061   return hyper_pa
-00006d80: 7261 6d65 7465 7273 0a0a 2020 2020 6465  rameters..    de
-00006d90: 6620 7370 6563 6961 6c5f 636f 6d70 6f6e  f special_compon
-00006da0: 656e 7473 2873 656c 662c 202a 2a6b 7761  ents(self, **kwa
-00006db0: 7267 7329 202d 3e20 4e6f 6e65 3a0a 2020  rgs) -> None:.  
-00006dc0: 2020 2020 2020 2222 2249 6e76 6f6b 6520        """Invoke 
-00006dd0: 616c 6c20 7370 6563 6961 6c20 6170 706c  all special appl
-00006de0: 6963 6174 696f 6e20 6675 6e63 7469 6f6e  ication function
-00006df0: 7320 666f 7220 7468 6973 2061 6c67 6f72  s for this algor
-00006e00: 6974 686d 7320 6279 2053 6369 6b69 742d  ithms by Scikit-
-00006e10: 6c65 6172 6e20 6672 616d 6577 6f72 6b2e  learn framework.
-00006e20: 2222 220a 2020 2020 2020 2020 7061 7373  """.        pass
-00006e30: 0a                                       .
+00000010: 662d 3820 2d2a 2d0a 0a69 6d70 6f72 7420  f-8 -*-..import 
+00000020: 6f73 0a66 726f 6d20 7479 7069 6e67 2069  os.from typing i
+00000030: 6d70 6f72 7420 4469 6374 2c20 4f70 7469  mport Dict, Opti
+00000040: 6f6e 616c 2c20 556e 696f 6e0a 0a69 6d70  onal, Union..imp
+00000050: 6f72 7420 6e75 6d70 7920 6173 206e 700a  ort numpy as np.
+00000060: 696d 706f 7274 2070 616e 6461 7320 6173  import pandas as
+00000070: 2070 640a 6672 6f6d 2072 6963 6820 696d   pd.from rich im
+00000080: 706f 7274 2070 7269 6e74 0a66 726f 6d20  port print.from 
+00000090: 736b 6c65 6172 6e2e 6465 636f 6d70 6f73  sklearn.decompos
+000000a0: 6974 696f 6e20 696d 706f 7274 2050 4341  ition import PCA
+000000b0: 0a66 726f 6d20 736b 6c65 6172 6e2e 6d61  .from sklearn.ma
+000000c0: 6e69 666f 6c64 2069 6d70 6f72 7420 4d44  nifold import MD
+000000d0: 532c 2054 534e 450a 0a66 726f 6d20 2e2e  S, TSNE..from ..
+000000e0: 636f 6e73 7461 6e74 7320 696d 706f 7274  constants import
+000000f0: 204d 4c46 4c4f 575f 4152 5449 4641 4354   MLFLOW_ARTIFACT
+00000100: 5f49 4d41 4745 5f4d 4f44 454c 5f4f 5554  _IMAGE_MODEL_OUT
+00000110: 5055 545f 5041 5448 0a66 726f 6d20 2e2e  PUT_PATH.from ..
+00000120: 7574 696c 732e 6261 7365 2069 6d70 6f72  utils.base impor
+00000130: 7420 636c 6561 725f 6f75 7470 7574 2c20  t clear_output, 
+00000140: 7361 7665 5f64 6174 612c 2073 6176 655f  save_data, save_
+00000150: 6669 670a 6672 6f6d 202e 5f62 6173 6520  fig.from ._base 
+00000160: 696d 706f 7274 2057 6f72 6b66 6c6f 7742  import WorkflowB
+00000170: 6173 650a 6672 6f6d 202e 6675 6e63 2e61  ase.from .func.a
+00000180: 6c67 6f5f 6465 636f 6d70 6f73 6974 696f  lgo_decompositio
+00000190: 6e2e 5f63 6f6d 6d6f 6e20 696d 706f 7274  n._common import
+000001a0: 2070 6c6f 745f 3264 5f73 6361 7474 6572   plot_2d_scatter
+000001b0: 5f64 6961 6772 616d 2c20 706c 6f74 5f63  _diagram, plot_c
+000001c0: 6f6e 746f 7572 2c20 706c 6f74 5f68 6561  ontour, plot_hea
+000001d0: 746d 6170 0a66 726f 6d20 2e66 756e 632e  tmap.from .func.
+000001e0: 616c 676f 5f64 6563 6f6d 706f 7369 7469  algo_decompositi
+000001f0: 6f6e 2e5f 6d64 7320 696d 706f 7274 206d  on._mds import m
+00000200: 6473 5f6d 616e 7561 6c5f 6879 7065 725f  ds_manual_hyper_
+00000210: 7061 7261 6d65 7465 7273 0a66 726f 6d20  parameters.from 
+00000220: 2e66 756e 632e 616c 676f 5f64 6563 6f6d  .func.algo_decom
+00000230: 706f 7369 7469 6f6e 2e5f 7063 6120 696d  position._pca im
+00000240: 706f 7274 2062 6970 6c6f 742c 2070 6361  port biplot, pca
+00000250: 5f6d 616e 7561 6c5f 6879 7065 725f 7061  _manual_hyper_pa
+00000260: 7261 6d65 7465 7273 2c20 7472 6970 6c6f  rameters, triplo
+00000270: 740a 6672 6f6d 202e 6675 6e63 2e61 6c67  t.from .func.alg
+00000280: 6f5f 6465 636f 6d70 6f73 6974 696f 6e2e  o_decomposition.
+00000290: 5f74 736e 6520 696d 706f 7274 2074 736e  _tsne import tsn
+000002a0: 655f 6d61 6e75 616c 5f68 7970 6572 5f70  e_manual_hyper_p
+000002b0: 6172 616d 6574 6572 730a 0a0a 636c 6173  arameters...clas
+000002c0: 7320 4465 636f 6d70 6f73 6974 696f 6e57  s DecompositionW
+000002d0: 6f72 6b66 6c6f 7742 6173 6528 576f 726b  orkflowBase(Work
+000002e0: 666c 6f77 4261 7365 293a 0a20 2020 2022  flowBase):.    "
+000002f0: 2222 5468 6520 6261 7365 2077 6f72 6b66  ""The base workf
+00000300: 6c6f 7720 636c 6173 7320 6f66 2064 6563  low class of dec
+00000310: 6f6d 706f 7369 7469 6f6e 2061 6c67 6f72  omposition algor
+00000320: 6974 686d 732e 2222 220a 0a20 2020 2063  ithms."""..    c
+00000330: 6f6d 6d6f 6e5f 6675 6e63 7469 6f6e 203d  ommon_function =
+00000340: 205b 224d 6f64 656c 2050 6572 7369 7374   ["Model Persist
+00000350: 656e 6365 225d 2020 2320 2744 6563 6f6d  ence"]  # 'Decom
+00000360: 706f 7369 7469 6f6e 2052 6573 756c 7427  position Result'
+00000370: 2c0a 0a20 2020 2064 6566 205f 5f69 6e69  ,..    def __ini
+00000380: 745f 5f28 7365 6c66 2920 2d3e 204e 6f6e  t__(self) -> Non
+00000390: 653a 0a20 2020 2020 2020 2073 7570 6572  e:.        super
+000003a0: 2829 2e5f 5f69 6e69 745f 5f28 290a 0a20  ().__init__().. 
+000003b0: 2020 2020 2020 2023 2074 6865 2065 7874         # the ext
+000003c0: 7261 2061 7474 7269 6275 7465 7320 7468  ra attributes th
+000003d0: 6174 2064 6563 6f6d 706f 7369 7469 6f6e  at decomposition
+000003e0: 2061 6c67 6f72 6974 686d 206e 6565 6473   algorithm needs
+000003f0: 0a20 2020 2020 2020 2073 656c 662e 585f  .        self.X_
+00000400: 7265 6475 6365 6420 3d20 4e6f 6e65 0a20  reduced = None. 
+00000410: 2020 2020 2020 2073 656c 662e 6d6f 6465         self.mode
+00000420: 203d 2022 4465 636f 6d70 6f73 6974 696f   = "Decompositio
+00000430: 6e22 0a0a 2020 2020 6465 6620 6669 7428  n"..    def fit(
+00000440: 7365 6c66 2c20 583a 2070 642e 4461 7461  self, X: pd.Data
+00000450: 4672 616d 652c 2079 3a20 4f70 7469 6f6e  Frame, y: Option
+00000460: 616c 5b70 642e 4461 7461 4672 616d 655d  al[pd.DataFrame]
+00000470: 203d 204e 6f6e 6529 202d 3e20 4e6f 6e65   = None) -> None
+00000480: 3a0a 2020 2020 2020 2020 2222 2246 6974  :.        """Fit
+00000490: 2074 6865 206d 6f64 656c 2e22 2222 0a20   the model.""". 
+000004a0: 2020 2020 2020 2073 656c 662e 6d6f 6465         self.mode
+000004b0: 6c2e 6669 7428 5829 0a0a 2020 2020 6465  l.fit(X)..    de
+000004c0: 6620 7472 616e 7366 6f72 6d28 7365 6c66  f transform(self
+000004d0: 2c20 583a 2070 642e 4461 7461 4672 616d  , X: pd.DataFram
+000004e0: 6529 202d 3e20 7064 2e44 6174 6146 7261  e) -> pd.DataFra
+000004f0: 6d65 3a0a 2020 2020 2020 2020 2222 2241  me:.        """A
+00000500: 7070 6c79 2064 696d 656e 7369 6f6e 616c  pply dimensional
+00000510: 6974 7920 7265 6475 6374 696f 6e20 746f  ity reduction to
+00000520: 2058 2e22 2222 0a20 2020 2020 2020 2072   X.""".        r
+00000530: 6574 7572 6e20 7365 6c66 2e6d 6f64 656c  eturn self.model
+00000540: 2e74 7261 6e73 666f 726d 2858 290a 0a20  .transform(X).. 
+00000550: 2020 2064 6566 2066 6974 5f74 7261 6e73     def fit_trans
+00000560: 666f 726d 2873 656c 662c 2058 3a20 7064  form(self, X: pd
+00000570: 2e44 6174 6146 7261 6d65 2c20 793a 204f  .DataFrame, y: O
+00000580: 7074 696f 6e61 6c5b 7064 2e44 6174 6146  ptional[pd.DataF
+00000590: 7261 6d65 5d20 3d20 4e6f 6e65 2920 2d3e  rame] = None) ->
+000005a0: 2070 642e 4461 7461 4672 616d 653a 0a20   pd.DataFrame:. 
+000005b0: 2020 2020 2020 2022 2222 4669 7420 7468         """Fit th
+000005c0: 6520 6d6f 6465 6c20 7769 7468 2058 2061  e model with X a
+000005d0: 6e64 2061 7070 6c79 2074 6865 2064 696d  nd apply the dim
+000005e0: 656e 7369 6f6e 616c 6974 7920 7265 6475  ensionality redu
+000005f0: 6374 696f 6e20 6f6e 2058 2e22 2222 0a20  ction on X.""". 
+00000600: 2020 2020 2020 2023 2054 4f44 4f28 4361         # TODO(Ca
+00000610: 6e20 4865 2853 616e 7929 2073 616e 6865  n He(Sany) sanhe
+00000620: 3130 3937 3631 3834 3335 4031 3633 2e63  1097618435@163.c
+00000630: 6f6d 293a 2063 6865 636b 2069 6620 7765  om): check if we
+00000640: 206e 6565 6420 746f 2070 7574 2074 6869   need to put thi
+00000650: 7320 6675 6e63 7469 6f6e 2069 6e20 7468  s function in th
+00000660: 6520 6261 7365 2063 6c61 7373 0a20 2020  e base class.   
+00000670: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00000680: 2e6d 6f64 656c 2e66 6974 5f74 7261 6e73  .model.fit_trans
+00000690: 666f 726d 2858 290a 0a20 2020 2040 636c  form(X)..    @cl
+000006a0: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
+000006b0: 6620 6d61 6e75 616c 5f68 7970 6572 5f70  f manual_hyper_p
+000006c0: 6172 616d 6574 6572 7328 636c 7329 202d  arameters(cls) -
+000006d0: 3e20 4469 6374 3a0a 2020 2020 2020 2020  > Dict:.        
+000006e0: 2222 224d 616e 7561 6c20 6879 7065 722d  """Manual hyper-
+000006f0: 7061 7261 6d65 7465 7273 2073 7065 6369  parameters speci
+00000700: 6669 6361 7469 6f6e 2e22 2222 0a20 2020  fication.""".   
+00000710: 2020 2020 2072 6574 7572 6e20 6469 6374       return dict
+00000720: 2829 0a0a 2020 2020 6465 6620 5f72 6564  ()..    def _red
+00000730: 7563 6564 5f64 6174 6132 7064 2873 656c  uced_data2pd(sel
+00000740: 662c 2072 6564 7563 6564 5f64 6174 613a  f, reduced_data:
+00000750: 206e 702e 6e64 6172 7261 792c 2063 6f6d   np.ndarray, com
+00000760: 706f 6e65 6e74 735f 6e75 6d3a 2069 6e74  ponents_num: int
+00000770: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00000780: 2020 2022 2222 5472 616e 7366 6f72 6d20     """Transform 
+00000790: 7265 6475 6365 6420 6461 7461 2069 6e74  reduced data int
+000007a0: 6f20 7468 6520 666f 726d 6174 206f 6620  o the format of 
+000007b0: 7064 2e44 6174 6146 7261 6d65 2e0a 0a20  pd.DataFrame... 
+000007c0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+000007d0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+000007e0: 2d2d 2d2d 0a20 2020 2020 2020 2072 6564  ----.        red
+000007f0: 7563 6564 5f64 6174 6120 3a20 6e70 2e6e  uced_data : np.n
+00000800: 6461 7272 6179 0a20 2020 2020 2020 2020  darray.         
+00000810: 2020 2054 6865 2064 6174 6120 5820 6166     The data X af
+00000820: 7465 7220 6469 6d65 6e73 696f 6e20 7265  ter dimension re
+00000830: 6475 6374 696f 6e2e 0a0a 2020 2020 2020  duction...      
+00000840: 2020 636f 6d70 6f6e 656e 7473 5f6e 756d    components_num
+00000850: 203a 2069 6e74 0a20 2020 2020 2020 2020   : int.         
+00000860: 2020 2054 6865 206e 756d 6265 7273 206f     The numbers o
+00000870: 6620 7468 6520 7072 696e 6369 7061 6c20  f the principal 
+00000880: 636f 6d70 6f6e 656e 7473 2e0a 2020 2020  components..    
+00000890: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000008a0: 7061 5f6e 616d 6520 3d20 5b5d 0a20 2020  pa_name = [].   
+000008b0: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+000008c0: 6e67 6528 636f 6d70 6f6e 656e 7473 5f6e  nge(components_n
+000008d0: 756d 293a 0a20 2020 2020 2020 2020 2020  um):.           
+000008e0: 2070 615f 6e61 6d65 2e61 7070 656e 6428   pa_name.append(
+000008f0: 6622 5072 696e 6369 7061 6c20 4178 6973  f"Principal Axis
+00000900: 207b 692b 317d 2229 0a20 2020 2020 2020   {i+1}").       
+00000910: 2073 656c 662e 585f 7265 6475 6365 6420   self.X_reduced 
+00000920: 3d20 7064 2e44 6174 6146 7261 6d65 2872  = pd.DataFrame(r
+00000930: 6564 7563 6564 5f64 6174 6129 0a20 2020  educed_data).   
+00000940: 2020 2020 2073 656c 662e 585f 7265 6475       self.X_redu
+00000950: 6365 642e 636f 6c75 6d6e 7320 3d20 7061  ced.columns = pa
+00000960: 5f6e 616d 650a 0a20 2020 2040 7374 6174  _name..    @stat
+00000970: 6963 6d65 7468 6f64 0a20 2020 2064 6566  icmethod.    def
+00000980: 205f 706c 6f74 5f32 645f 7363 6174 7465   _plot_2d_scatte
+00000990: 725f 6469 6167 7261 6d28 6461 7461 3a20  r_diagram(data: 
+000009a0: 7064 2e44 6174 6146 7261 6d65 2c20 616c  pd.DataFrame, al
+000009b0: 676f 7269 7468 6d5f 6e61 6d65 3a20 7374  gorithm_name: st
+000009c0: 722c 206c 6f63 616c 5f70 6174 683a 2073  r, local_path: s
+000009d0: 7472 2c20 6d6c 666c 6f77 5f70 6174 683a  tr, mlflow_path:
+000009e0: 2073 7472 2920 2d3e 204e 6f6e 653a 0a20   str) -> None:. 
+000009f0: 2020 2020 2020 2022 2222 506c 6f74 2074         """Plot t
+00000a00: 6865 2074 776f 2d64 696d 656e 7369 6f6e  he two-dimension
+00000a10: 616c 2064 6961 6772 616d 206f 6620 7468  al diagram of th
+00000a20: 6520 6465 636f 6d70 6f73 6974 696f 6e20  e decomposition 
+00000a30: 7265 7375 6c74 2e22 2222 0a20 2020 2020  result.""".     
+00000a40: 2020 2070 7269 6e74 2822 2d2d 2d2d 2d2a     print("-----*
+00000a50: 2044 6563 6f6d 706f 7369 7469 6f6e 2054   Decomposition T
+00000a60: 776f 2d44 696d 656e 7369 6f6e 616c 2044  wo-Dimensional D
+00000a70: 6961 6772 616d 202a 2d2d 2d2d 2d22 290a  iagram *-----").
+00000a80: 2020 2020 2020 2020 706c 6f74 5f32 645f          plot_2d_
+00000a90: 7363 6174 7465 725f 6469 6167 7261 6d28  scatter_diagram(
+00000aa0: 6461 7461 2c20 616c 676f 7269 7468 6d5f  data, algorithm_
+00000ab0: 6e61 6d65 290a 2020 2020 2020 2020 7361  name).        sa
+00000ac0: 7665 5f66 6967 2866 2244 6563 6f6d 706f  ve_fig(f"Decompo
+00000ad0: 7369 7469 6f6e 2054 776f 2d44 696d 656e  sition Two-Dimen
+00000ae0: 7369 6f6e 616c 2044 6961 6772 616d 202d  sional Diagram -
+00000af0: 207b 616c 676f 7269 7468 6d5f 6e61 6d65   {algorithm_name
+00000b00: 7d22 2c20 6c6f 6361 6c5f 7061 7468 2c20  }", local_path, 
+00000b10: 6d6c 666c 6f77 5f70 6174 6829 0a20 2020  mlflow_path).   
+00000b20: 2020 2020 2073 6176 655f 6461 7461 2864       save_data(d
+00000b30: 6174 612c 2066 2244 6563 6f6d 706f 7369  ata, f"Decomposi
+00000b40: 7469 6f6e 2054 776f 2d44 696d 656e 7369  tion Two-Dimensi
+00000b50: 6f6e 616c 2044 6174 6120 2d20 7b61 6c67  onal Data - {alg
+00000b60: 6f72 6974 686d 5f6e 616d 657d 222c 206c  orithm_name}", l
+00000b70: 6f63 616c 5f70 6174 682c 206d 6c66 6c6f  ocal_path, mlflo
+00000b80: 775f 7061 7468 290a 0a20 2020 2040 7374  w_path)..    @st
+00000b90: 6174 6963 6d65 7468 6f64 0a20 2020 2064  aticmethod.    d
+00000ba0: 6566 205f 706c 6f74 5f68 6561 746d 6170  ef _plot_heatmap
+00000bb0: 2864 6174 613a 2070 642e 4461 7461 4672  (data: pd.DataFr
+00000bc0: 616d 652c 2061 6c67 6f72 6974 686d 5f6e  ame, algorithm_n
+00000bd0: 616d 653a 2073 7472 2c20 6c6f 6361 6c5f  ame: str, local_
+00000be0: 7061 7468 3a20 7374 722c 206d 6c66 6c6f  path: str, mlflo
+00000bf0: 775f 7061 7468 3a20 7374 7229 202d 3e20  w_path: str) -> 
+00000c00: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00000c10: 2250 6c6f 7420 6120 6865 6174 6d61 7020  "Plot a heatmap 
+00000c20: 666f 7220 7468 6520 6465 636f 6d70 6f73  for the decompos
+00000c30: 6974 696f 6e20 7265 7375 6c74 2e22 2222  ition result."""
+00000c40: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+00000c50: 2d2d 2d2d 2d2a 2044 6563 6f6d 706f 7369  -----* Decomposi
+00000c60: 7469 6f6e 2048 6561 746d 6170 202a 2d2d  tion Heatmap *--
+00000c70: 2d2d 2d22 290a 2020 2020 2020 2020 706c  ---").        pl
+00000c80: 6f74 5f68 6561 746d 6170 2864 6174 612c  ot_heatmap(data,
+00000c90: 2061 6c67 6f72 6974 686d 5f6e 616d 6529   algorithm_name)
+00000ca0: 0a20 2020 2020 2020 2073 6176 655f 6669  .        save_fi
+00000cb0: 6728 6622 4465 636f 6d70 6f73 6974 696f  g(f"Decompositio
+00000cc0: 6e20 4865 6174 6d61 7020 2d20 7b61 6c67  n Heatmap - {alg
+00000cd0: 6f72 6974 686d 5f6e 616d 657d 222c 206c  orithm_name}", l
+00000ce0: 6f63 616c 5f70 6174 682c 206d 6c66 6c6f  ocal_path, mlflo
+00000cf0: 775f 7061 7468 290a 2020 2020 2020 2020  w_path).        
+00000d00: 7361 7665 5f64 6174 6128 6461 7461 2c20  save_data(data, 
+00000d10: 6622 4465 636f 6d70 6f73 6974 696f 6e20  f"Decomposition 
+00000d20: 4865 6174 6d61 7020 4461 7461 202d 207b  Heatmap Data - {
+00000d30: 616c 676f 7269 7468 6d5f 6e61 6d65 7d22  algorithm_name}"
+00000d40: 2c20 6c6f 6361 6c5f 7061 7468 2c20 6d6c  , local_path, ml
+00000d50: 666c 6f77 5f70 6174 6829 0a0a 2020 2020  flow_path)..    
+00000d60: 4073 7461 7469 636d 6574 686f 640a 2020  @staticmethod.  
+00000d70: 2020 6465 6620 5f70 6c6f 745f 636f 6e74    def _plot_cont
+00000d80: 6f75 7228 6461 7461 3a20 7064 2e44 6174  our(data: pd.Dat
+00000d90: 6146 7261 6d65 2c20 616c 676f 7269 7468  aFrame, algorith
+00000da0: 6d5f 6e61 6d65 3a20 7374 722c 206c 6f63  m_name: str, loc
+00000db0: 616c 5f70 6174 683a 2073 7472 2c20 6d6c  al_path: str, ml
+00000dc0: 666c 6f77 5f70 6174 683a 2073 7472 2920  flow_path: str) 
+00000dd0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+00000de0: 2022 2222 506c 6f74 2061 2063 6f6e 746f   """Plot a conto
+00000df0: 7572 2070 6c6f 7420 666f 7220 6469 6d65  ur plot for dime
+00000e00: 6e73 696f 6e61 6c69 7479 2072 6564 7563  nsionality reduc
+00000e10: 7469 6f6e 2072 6573 756c 7473 2e22 2222  tion results."""
+00000e20: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+00000e30: 2d2d 2d2d 2d2a 2044 696d 656e 7369 6f6e  -----* Dimension
+00000e40: 616c 6974 7920 5265 6475 6374 696f 6e20  ality Reduction 
+00000e50: 436f 6e74 6f75 7220 506c 6f74 202a 2d2d  Contour Plot *--
+00000e60: 2d2d 2d22 290a 2020 2020 2020 2020 706c  ---").        pl
+00000e70: 6f74 5f63 6f6e 746f 7572 2864 6174 612c  ot_contour(data,
+00000e80: 2061 6c67 6f72 6974 686d 5f6e 616d 6529   algorithm_name)
+00000e90: 0a20 2020 2020 2020 2073 6176 655f 6669  .        save_fi
+00000ea0: 6728 6622 4469 6d65 6e73 696f 6e61 6c69  g(f"Dimensionali
+00000eb0: 7479 2052 6564 7563 7469 6f6e 2043 6f6e  ty Reduction Con
+00000ec0: 746f 7572 2050 6c6f 7420 2d20 7b61 6c67  tour Plot - {alg
+00000ed0: 6f72 6974 686d 5f6e 616d 657d 222c 206c  orithm_name}", l
+00000ee0: 6f63 616c 5f70 6174 682c 206d 6c66 6c6f  ocal_path, mlflo
+00000ef0: 775f 7061 7468 290a 2020 2020 2020 2020  w_path).        
+00000f00: 7361 7665 5f64 6174 6128 6461 7461 2c20  save_data(data, 
+00000f10: 6622 4469 6d65 6e73 696f 6e61 6c69 7479  f"Dimensionality
+00000f20: 2052 6564 7563 7469 6f6e 2043 6f6e 746f   Reduction Conto
+00000f30: 7572 2050 6c6f 7420 4461 7461 202d 207b  ur Plot Data - {
+00000f40: 616c 676f 7269 7468 6d5f 6e61 6d65 7d22  algorithm_name}"
+00000f50: 2c20 6c6f 6361 6c5f 7061 7468 2c20 6d6c  , local_path, ml
+00000f60: 666c 6f77 5f70 6174 6829 0a0a 2020 2020  flow_path)..    
+00000f70: 6465 6620 636f 6d6d 6f6e 5f63 6f6d 706f  def common_compo
+00000f80: 6e65 6e74 7328 7365 6c66 2920 2d3e 204e  nents(self) -> N
+00000f90: 6f6e 653a 0a20 2020 2020 2020 2022 2222  one:.        """
+00000fa0: 496e 766f 6b65 2061 6c6c 2063 6f6d 6d6f  Invoke all commo
+00000fb0: 6e20 6170 706c 6963 6174 696f 6e20 6675  n application fu
+00000fc0: 6e63 7469 6f6e 7320 666f 7220 6465 636f  nctions for deco
+00000fd0: 6d70 6f73 6974 696f 6e20 616c 676f 7269  mposition algori
+00000fe0: 7468 6d73 2062 7920 5363 696b 6974 2d6c  thms by Scikit-l
+00000ff0: 6561 726e 2066 7261 6d65 776f 726b 2e22  earn framework."
+00001000: 2222 0a0a 2020 2020 2020 2020 4745 4f50  ""..        GEOP
+00001010: 495f 4f55 5450 5554 5f41 5254 4946 4143  I_OUTPUT_ARTIFAC
+00001020: 5453 5f49 4d41 4745 5f4d 4f44 454c 5f4f  TS_IMAGE_MODEL_O
+00001030: 5554 5055 545f 5041 5448 203d 206f 732e  UTPUT_PATH = os.
+00001040: 6765 7465 6e76 2822 4745 4f50 495f 4f55  getenv("GEOPI_OU
+00001050: 5450 5554 5f41 5254 4946 4143 5453 5f49  TPUT_ARTIFACTS_I
+00001060: 4d41 4745 5f4d 4f44 454c 5f4f 5554 5055  MAGE_MODEL_OUTPU
+00001070: 545f 5041 5448 2229 0a20 2020 2020 2020  T_PATH").       
+00001080: 2073 656c 662e 5f70 6c6f 745f 3264 5f73   self._plot_2d_s
+00001090: 6361 7474 6572 5f64 6961 6772 616d 280a  catter_diagram(.
+000010a0: 2020 2020 2020 2020 2020 2020 6461 7461              data
+000010b0: 3d73 656c 662e 582c 0a20 2020 2020 2020  =self.X,.       
+000010c0: 2020 2020 2061 6c67 6f72 6974 686d 5f6e       algorithm_n
+000010d0: 616d 653d 7365 6c66 2e6e 616d 696e 672c  ame=self.naming,
+000010e0: 0a20 2020 2020 2020 2020 2020 206c 6f63  .            loc
+000010f0: 616c 5f70 6174 683d 4745 4f50 495f 4f55  al_path=GEOPI_OU
+00001100: 5450 5554 5f41 5254 4946 4143 5453 5f49  TPUT_ARTIFACTS_I
+00001110: 4d41 4745 5f4d 4f44 454c 5f4f 5554 5055  MAGE_MODEL_OUTPU
+00001120: 545f 5041 5448 2c0a 2020 2020 2020 2020  T_PATH,.        
+00001130: 2020 2020 6d6c 666c 6f77 5f70 6174 683d      mlflow_path=
+00001140: 4d4c 464c 4f57 5f41 5254 4946 4143 545f  MLFLOW_ARTIFACT_
+00001150: 494d 4147 455f 4d4f 4445 4c5f 4f55 5450  IMAGE_MODEL_OUTP
+00001160: 5554 5f50 4154 482c 0a20 2020 2020 2020  UT_PATH,.       
+00001170: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
+00001180: 5f70 6c6f 745f 6865 6174 6d61 7028 0a20  _plot_heatmap(. 
+00001190: 2020 2020 2020 2020 2020 2064 6174 613d             data=
+000011a0: 7365 6c66 2e58 2c0a 2020 2020 2020 2020  self.X,.        
+000011b0: 2020 2020 616c 676f 7269 7468 6d5f 6e61      algorithm_na
+000011c0: 6d65 3d73 656c 662e 6e61 6d69 6e67 2c0a  me=self.naming,.
+000011d0: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
+000011e0: 6c5f 7061 7468 3d47 454f 5049 5f4f 5554  l_path=GEOPI_OUT
+000011f0: 5055 545f 4152 5449 4641 4354 535f 494d  PUT_ARTIFACTS_IM
+00001200: 4147 455f 4d4f 4445 4c5f 4f55 5450 5554  AGE_MODEL_OUTPUT
+00001210: 5f50 4154 482c 0a20 2020 2020 2020 2020  _PATH,.         
+00001220: 2020 206d 6c66 6c6f 775f 7061 7468 3d4d     mlflow_path=M
+00001230: 4c46 4c4f 575f 4152 5449 4641 4354 5f49  LFLOW_ARTIFACT_I
+00001240: 4d41 4745 5f4d 4f44 454c 5f4f 5554 5055  MAGE_MODEL_OUTPU
+00001250: 545f 5041 5448 2c0a 2020 2020 2020 2020  T_PATH,.        
+00001260: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
+00001270: 706c 6f74 5f63 6f6e 746f 7572 280a 2020  plot_contour(.  
+00001280: 2020 2020 2020 2020 2020 6461 7461 3d73            data=s
+00001290: 656c 662e 582c 0a20 2020 2020 2020 2020  elf.X,.         
+000012a0: 2020 2061 6c67 6f72 6974 686d 5f6e 616d     algorithm_nam
+000012b0: 653d 7365 6c66 2e6e 616d 696e 672c 0a20  e=self.naming,. 
+000012c0: 2020 2020 2020 2020 2020 206c 6f63 616c             local
+000012d0: 5f70 6174 683d 4745 4f50 495f 4f55 5450  _path=GEOPI_OUTP
+000012e0: 5554 5f41 5254 4946 4143 5453 5f49 4d41  UT_ARTIFACTS_IMA
+000012f0: 4745 5f4d 4f44 454c 5f4f 5554 5055 545f  GE_MODEL_OUTPUT_
+00001300: 5041 5448 2c0a 2020 2020 2020 2020 2020  PATH,.          
+00001310: 2020 6d6c 666c 6f77 5f70 6174 683d 4d4c    mlflow_path=ML
+00001320: 464c 4f57 5f41 5254 4946 4143 545f 494d  FLOW_ARTIFACT_IM
+00001330: 4147 455f 4d4f 4445 4c5f 4f55 5450 5554  AGE_MODEL_OUTPUT
+00001340: 5f50 4154 482c 0a20 2020 2020 2020 2029  _PATH,.        )
+00001350: 0a0a 0a63 6c61 7373 2050 4341 4465 636f  ...class PCADeco
+00001360: 6d70 6f73 6974 696f 6e28 4465 636f 6d70  mposition(Decomp
+00001370: 6f73 6974 696f 6e57 6f72 6b66 6c6f 7742  ositionWorkflowB
+00001380: 6173 6529 3a0a 2020 2020 2222 2254 6865  ase):.    """The
+00001390: 2061 7574 6f6d 6174 696f 6e20 776f 726b   automation work
+000013a0: 666c 6f77 206f 6620 7573 696e 6720 5043  flow of using PC
+000013b0: 4120 616c 676f 7269 7468 6d20 746f 206d  A algorithm to m
+000013c0: 616b 6520 696e 7369 6768 7466 756c 2070  ake insightful p
+000013d0: 726f 6475 6374 732e 2222 220a 0a20 2020  roducts."""..   
+000013e0: 206e 616d 6520 3d20 2250 4341 220a 2020   name = "PCA".  
+000013f0: 2020 7370 6563 6961 6c5f 6675 6e63 7469    special_functi
+00001400: 6f6e 203d 205b 2250 7269 6e63 6970 616c  on = ["Principal
+00001410: 2043 6f6d 706f 6e65 6e74 7322 2c20 2245   Components", "E
+00001420: 7870 6c61 696e 6564 2056 6172 6961 6e63  xplained Varianc
+00001430: 6520 5261 7469 6f22 2c20 2243 6f6d 706f  e Ratio", "Compo
+00001440: 7369 7469 6f6e 616c 2042 692d 706c 6f74  sitional Bi-plot
+00001450: 222c 2022 436f 6d70 6f73 6974 696f 6e61  ", "Compositiona
+00001460: 6c20 5472 692d 706c 6f74 225d 0a0a 2020  l Tri-plot"]..  
+00001470: 2020 6465 6620 5f5f 696e 6974 5f5f 280a    def __init__(.
+00001480: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+00001490: 2020 2020 2020 6e5f 636f 6d70 6f6e 656e        n_componen
+000014a0: 7473 3a20 4f70 7469 6f6e 616c 5b69 6e74  ts: Optional[int
+000014b0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+000014c0: 2020 636f 7079 3a20 626f 6f6c 203d 2054    copy: bool = T
+000014d0: 7275 652c 0a20 2020 2020 2020 2077 6869  rue,.        whi
+000014e0: 7465 6e3a 2062 6f6f 6c20 3d20 4661 6c73  ten: bool = Fals
+000014f0: 652c 0a20 2020 2020 2020 2073 7664 5f73  e,.        svd_s
+00001500: 6f6c 7665 723a 2073 7472 203d 2022 6175  olver: str = "au
+00001510: 746f 222c 0a20 2020 2020 2020 2074 6f6c  to",.        tol
+00001520: 3a20 666c 6f61 7420 3d20 302e 302c 0a20  : float = 0.0,. 
+00001530: 2020 2020 2020 2069 7465 7261 7465 645f         iterated_
+00001540: 706f 7765 723a 2055 6e69 6f6e 5b69 6e74  power: Union[int
+00001550: 2c20 7374 725d 203d 2022 6175 746f 222c  , str] = "auto",
+00001560: 0a20 2020 2020 2020 206e 5f6f 7665 7273  .        n_overs
+00001570: 616d 706c 6573 3a20 696e 7420 3d20 3130  amples: int = 10
+00001580: 2c0a 2020 2020 2020 2020 706f 7765 725f  ,.        power_
+00001590: 6974 6572 6174 696f 6e5f 6e6f 726d 616c  iteration_normal
+000015a0: 697a 6572 3a20 7374 7220 3d20 2261 7574  izer: str = "aut
+000015b0: 6f22 2c0a 2020 2020 2020 2020 7261 6e64  o",.        rand
+000015c0: 6f6d 5f73 7461 7465 3a20 4f70 7469 6f6e  om_state: Option
+000015d0: 616c 5b69 6e74 5d20 3d20 4e6f 6e65 2c0a  al[int] = None,.
+000015e0: 2020 2020 2920 2d3e 204e 6f6e 653a 0a20      ) -> None:. 
+000015f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00001600: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00001610: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00001620: 0a20 2020 2020 2020 206e 5f63 6f6d 706f  .        n_compo
+00001630: 6e65 6e74 7320 3a20 696e 742c 2066 6c6f  nents : int, flo
+00001640: 6174 206f 7220 276d 6c65 272c 2064 6566  at or 'mle', def
+00001650: 6175 6c74 3d4e 6f6e 650a 2020 2020 2020  ault=None.      
+00001660: 2020 2020 2020 4e75 6d62 6572 206f 6620        Number of 
+00001670: 636f 6d70 6f6e 656e 7473 2074 6f20 6b65  components to ke
+00001680: 6570 2e0a 2020 2020 2020 2020 2020 2020  ep..            
+00001690: 6966 206e 5f63 6f6d 706f 6e65 6e74 7320  if n_components 
+000016a0: 6973 206e 6f74 2073 6574 2061 6c6c 2063  is not set all c
+000016b0: 6f6d 706f 6e65 6e74 7320 6172 6520 6b65  omponents are ke
+000016c0: 7074 3a3a 0a0a 2020 2020 2020 2020 2020  pt::..          
+000016d0: 2020 2020 2020 6e5f 636f 6d70 6f6e 656e        n_componen
+000016e0: 7473 203d 3d20 6d69 6e28 6e5f 7361 6d70  ts == min(n_samp
+000016f0: 6c65 732c 206e 5f66 6561 7475 7265 7329  les, n_features)
+00001700: 0a0a 2020 2020 2020 2020 2020 2020 4966  ..            If
+00001710: 2060 606e 5f63 6f6d 706f 6e65 6e74 7320   ``n_components 
+00001720: 3d3d 2027 6d6c 6527 6060 2061 6e64 2060  == 'mle'`` and `
+00001730: 6073 7664 5f73 6f6c 7665 7220 3d3d 2027  `svd_solver == '
+00001740: 6675 6c6c 2760 602c 204d 696e 6b61 2773  full'``, Minka's
+00001750: 0a20 2020 2020 2020 2020 2020 204d 4c45  .            MLE
+00001760: 2069 7320 7573 6564 2074 6f20 6775 6573   is used to gues
+00001770: 7320 7468 6520 6469 6d65 6e73 696f 6e2e  s the dimension.
+00001780: 2055 7365 206f 6620 6060 6e5f 636f 6d70   Use of ``n_comp
+00001790: 6f6e 656e 7473 203d 3d20 276d 6c65 2760  onents == 'mle'`
+000017a0: 600a 2020 2020 2020 2020 2020 2020 7769  `.            wi
+000017b0: 6c6c 2069 6e74 6572 7072 6574 2060 6073  ll interpret ``s
+000017c0: 7664 5f73 6f6c 7665 7220 3d3d 2027 6175  vd_solver == 'au
+000017d0: 746f 2760 6020 6173 2060 6073 7664 5f73  to'`` as ``svd_s
+000017e0: 6f6c 7665 7220 3d3d 2027 6675 6c6c 2760  olver == 'full'`
+000017f0: 602e 0a0a 2020 2020 2020 2020 2020 2020  `...            
+00001800: 4966 2060 6030 203c 206e 5f63 6f6d 706f  If ``0 < n_compo
+00001810: 6e65 6e74 7320 3c20 3160 6020 616e 6420  nents < 1`` and 
+00001820: 6060 7376 645f 736f 6c76 6572 203d 3d20  ``svd_solver == 
+00001830: 2766 756c 6c27 6060 2c20 7365 6c65 6374  'full'``, select
+00001840: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
+00001850: 206e 756d 6265 7220 6f66 2063 6f6d 706f   number of compo
+00001860: 6e65 6e74 7320 7375 6368 2074 6861 7420  nents such that 
+00001870: 7468 6520 616d 6f75 6e74 206f 6620 7661  the amount of va
+00001880: 7269 616e 6365 2074 6861 7420 6e65 6564  riance that need
+00001890: 7320 746f 2062 650a 2020 2020 2020 2020  s to be.        
+000018a0: 2020 2020 6578 706c 6169 6e65 6420 6973      explained is
+000018b0: 2067 7265 6174 6572 2074 6861 6e20 7468   greater than th
+000018c0: 6520 7065 7263 656e 7461 6765 2073 7065  e percentage spe
+000018d0: 6369 6669 6564 2062 7920 6e5f 636f 6d70  cified by n_comp
+000018e0: 6f6e 656e 7473 2e0a 0a20 2020 2020 2020  onents...       
+000018f0: 2020 2020 2049 6620 6060 7376 645f 736f       If ``svd_so
+00001900: 6c76 6572 203d 3d20 2761 7270 6163 6b27  lver == 'arpack'
+00001910: 6060 2c20 7468 6520 6e75 6d62 6572 206f  ``, the number o
+00001920: 6620 636f 6d70 6f6e 656e 7473 206d 7573  f components mus
+00001930: 7420 6265 0a20 2020 2020 2020 2020 2020  t be.           
+00001940: 2073 7472 6963 746c 7920 6c65 7373 2074   strictly less t
+00001950: 6861 6e20 7468 6520 6d69 6e69 6d75 6d20  han the minimum 
+00001960: 6f66 206e 5f66 6561 7475 7265 7320 616e  of n_features an
+00001970: 6420 6e5f 7361 6d70 6c65 732e 0a0a 2020  d n_samples...  
+00001980: 2020 2020 2020 2020 2020 4865 6e63 652c            Hence,
+00001990: 2074 6865 204e 6f6e 6520 6361 7365 2072   the None case r
+000019a0: 6573 756c 7473 2069 6e3a 3a0a 0a20 2020  esults in::..   
+000019b0: 2020 2020 2020 2020 2020 2020 206e 5f63               n_c
+000019c0: 6f6d 706f 6e65 6e74 7320 3d3d 206d 696e  omponents == min
+000019d0: 286e 5f73 616d 706c 6573 2c20 6e5f 6665  (n_samples, n_fe
+000019e0: 6174 7572 6573 2920 2d20 310a 0a20 2020  atures) - 1..   
+000019f0: 2020 2020 2063 6f70 7920 3a20 626f 6f6c       copy : bool
+00001a00: 2c20 6465 6661 756c 743d 5472 7565 0a20  , default=True. 
+00001a10: 2020 2020 2020 2020 2020 2049 6620 4661             If Fa
+00001a20: 6c73 652c 2064 6174 6120 7061 7373 6564  lse, data passed
+00001a30: 2074 6f20 6669 7420 6172 6520 6f76 6572   to fit are over
+00001a40: 7772 6974 7465 6e20 616e 6420 7275 6e6e  written and runn
+00001a50: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+00001a60: 6669 7428 5829 2e74 7261 6e73 666f 726d  fit(X).transform
+00001a70: 2858 2920 7769 6c6c 206e 6f74 2079 6965  (X) will not yie
+00001a80: 6c64 2074 6865 2065 7870 6563 7465 6420  ld the expected 
+00001a90: 7265 7375 6c74 732c 0a20 2020 2020 2020  results,.       
+00001aa0: 2020 2020 2075 7365 2066 6974 5f74 7261       use fit_tra
+00001ab0: 6e73 666f 726d 2858 2920 696e 7374 6561  nsform(X) instea
+00001ac0: 642e 0a0a 2020 2020 2020 2020 7768 6974  d...        whit
+00001ad0: 656e 203a 2062 6f6f 6c2c 2064 6566 6175  en : bool, defau
+00001ae0: 6c74 3d46 616c 7365 0a20 2020 2020 2020  lt=False.       
+00001af0: 2020 2020 2057 6865 6e20 5472 7565 2028       When True (
+00001b00: 4661 6c73 6520 6279 2064 6566 6175 6c74  False by default
+00001b10: 2920 7468 6520 6063 6f6d 706f 6e65 6e74  ) the `component
+00001b20: 735f 6020 7665 6374 6f72 7320 6172 6520  s_` vectors are 
+00001b30: 6d75 6c74 6970 6c69 6564 0a20 2020 2020  multiplied.     
+00001b40: 2020 2020 2020 2062 7920 7468 6520 7371         by the sq
+00001b50: 7561 7265 2072 6f6f 7420 6f66 206e 5f73  uare root of n_s
+00001b60: 616d 706c 6573 2061 6e64 2074 6865 6e20  amples and then 
+00001b70: 6469 7669 6465 6420 6279 2074 6865 2073  divided by the s
+00001b80: 696e 6775 6c61 7220 7661 6c75 6573 0a20  ingular values. 
+00001b90: 2020 2020 2020 2020 2020 2074 6f20 656e             to en
+00001ba0: 7375 7265 2075 6e63 6f72 7265 6c61 7465  sure uncorrelate
+00001bb0: 6420 6f75 7470 7574 7320 7769 7468 2075  d outputs with u
+00001bc0: 6e69 7420 636f 6d70 6f6e 656e 742d 7769  nit component-wi
+00001bd0: 7365 2076 6172 6961 6e63 6573 2e0a 2020  se variances..  
+00001be0: 2020 2020 2020 2020 2020 5768 6974 656e            Whiten
+00001bf0: 696e 6720 7769 6c6c 2072 656d 6f76 6520  ing will remove 
+00001c00: 736f 6d65 2069 6e66 6f72 6d61 7469 6f6e  some information
+00001c10: 2066 726f 6d20 7468 6520 7472 616e 7366   from the transf
+00001c20: 6f72 6d65 6420 7369 676e 616c 0a20 2020  ormed signal.   
+00001c30: 2020 2020 2020 2020 2028 7468 6520 7265           (the re
+00001c40: 6c61 7469 7665 2076 6172 6961 6e63 6520  lative variance 
+00001c50: 7363 616c 6573 206f 6620 7468 6520 636f  scales of the co
+00001c60: 6d70 6f6e 656e 7473 2920 6275 7420 6361  mponents) but ca
+00001c70: 6e20 736f 6d65 7469 6d65 0a20 2020 2020  n sometime.     
+00001c80: 2020 2020 2020 2069 6d70 726f 7665 2074         improve t
+00001c90: 6865 2070 7265 6469 6374 6976 6520 6163  he predictive ac
+00001ca0: 6375 7261 6379 206f 6620 7468 6520 646f  curacy of the do
+00001cb0: 776e 7374 7265 616d 2065 7374 696d 6174  wnstream estimat
+00001cc0: 6f72 7320 6279 0a20 2020 2020 2020 2020  ors by.         
+00001cd0: 2020 206d 616b 696e 6720 7468 6569 7220     making their 
+00001ce0: 6461 7461 2072 6573 7065 6374 2073 6f6d  data respect som
+00001cf0: 6520 6861 7264 2d77 6972 6564 2061 7373  e hard-wired ass
+00001d00: 756d 7074 696f 6e73 2e0a 0a20 2020 2020  umptions...     
+00001d10: 2020 2073 7664 5f73 6f6c 7665 7220 3a20     svd_solver : 
+00001d20: 7b27 6175 746f 272c 2027 6675 6c6c 272c  {'auto', 'full',
+00001d30: 2027 6172 7061 636b 272c 2027 7261 6e64   'arpack', 'rand
+00001d40: 6f6d 697a 6564 277d 2c20 6465 6661 756c  omized'}, defaul
+00001d50: 743d 2761 7574 6f27 0a20 2020 2020 2020  t='auto'.       
+00001d60: 2020 2020 2049 6620 6175 746f 203a 0a20       If auto :. 
+00001d70: 2020 2020 2020 2020 2020 2020 2020 2054                 T
+00001d80: 6865 2073 6f6c 7665 7220 6973 2073 656c  he solver is sel
+00001d90: 6563 7465 6420 6279 2061 2064 6566 6175  ected by a defau
+00001da0: 6c74 2070 6f6c 6963 7920 6261 7365 6420  lt policy based 
+00001db0: 6f6e 2060 582e 7368 6170 6560 2061 6e64  on `X.shape` and
+00001dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001dd0: 2060 6e5f 636f 6d70 6f6e 656e 7473 603a   `n_components`:
+00001de0: 2069 6620 7468 6520 696e 7075 7420 6461   if the input da
+00001df0: 7461 2069 7320 6c61 7267 6572 2074 6861  ta is larger tha
+00001e00: 6e20 3530 3078 3530 3020 616e 6420 7468  n 500x500 and th
+00001e10: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00001e20: 2020 6e75 6d62 6572 206f 6620 636f 6d70    number of comp
+00001e30: 6f6e 656e 7473 2074 6f20 6578 7472 6163  onents to extrac
+00001e40: 7420 6973 206c 6f77 6572 2074 6861 6e20  t is lower than 
+00001e50: 3830 2520 6f66 2074 6865 2073 6d61 6c6c  80% of the small
+00001e60: 6573 740a 2020 2020 2020 2020 2020 2020  est.            
+00001e70: 2020 2020 6469 6d65 6e73 696f 6e20 6f66      dimension of
+00001e80: 2074 6865 2064 6174 612c 2074 6865 6e20   the data, then 
+00001e90: 7468 6520 6d6f 7265 2065 6666 6963 6965  the more efficie
+00001ea0: 6e74 2027 7261 6e64 6f6d 697a 6564 270a  nt 'randomized'.
+00001eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ec0: 6d65 7468 6f64 2069 7320 656e 6162 6c65  method is enable
+00001ed0: 642e 204f 7468 6572 7769 7365 2074 6865  d. Otherwise the
+00001ee0: 2065 7861 6374 2066 756c 6c20 5356 4420   exact full SVD 
+00001ef0: 6973 2063 6f6d 7075 7465 6420 616e 640a  is computed and.
+00001f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f10: 6f70 7469 6f6e 616c 6c79 2074 7275 6e63  optionally trunc
+00001f20: 6174 6564 2061 6674 6572 7761 7264 732e  ated afterwards.
+00001f30: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
+00001f40: 6675 6c6c 203a 0a20 2020 2020 2020 2020  full :.         
+00001f50: 2020 2020 2020 2072 756e 2065 7861 6374         run exact
+00001f60: 2066 756c 6c20 5356 4420 6361 6c6c 696e   full SVD callin
+00001f70: 6720 7468 6520 7374 616e 6461 7264 204c  g the standard L
+00001f80: 4150 4143 4b20 736f 6c76 6572 2076 6961  APACK solver via
+00001f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001fa0: 2060 7363 6970 792e 6c69 6e61 6c67 2e73   `scipy.linalg.s
+00001fb0: 7664 6020 616e 6420 7365 6c65 6374 2074  vd` and select t
+00001fc0: 6865 2063 6f6d 706f 6e65 6e74 7320 6279  he components by
+00001fd0: 2070 6f73 7470 726f 6365 7373 696e 670a   postprocessing.
+00001fe0: 2020 2020 2020 2020 2020 2020 4966 2061              If a
+00001ff0: 7270 6163 6b20 3a0a 2020 2020 2020 2020  rpack :.        
+00002000: 2020 2020 2020 2020 7275 6e20 5356 4420          run SVD 
+00002010: 7472 756e 6361 7465 6420 746f 206e 5f63  truncated to n_c
+00002020: 6f6d 706f 6e65 6e74 7320 6361 6c6c 696e  omponents callin
+00002030: 6720 4152 5041 434b 2073 6f6c 7665 7220  g ARPACK solver 
+00002040: 7669 610a 2020 2020 2020 2020 2020 2020  via.            
+00002050: 2020 2020 6073 6369 7079 2e73 7061 7273      `scipy.spars
+00002060: 652e 6c69 6e61 6c67 2e73 7664 7360 2e20  e.linalg.svds`. 
+00002070: 4974 2072 6571 7569 7265 7320 7374 7269  It requires stri
+00002080: 6374 6c79 0a20 2020 2020 2020 2020 2020  ctly.           
+00002090: 2020 2020 2030 203c 206e 5f63 6f6d 706f       0 < n_compo
+000020a0: 6e65 6e74 7320 3c20 6d69 6e28 582e 7368  nents < min(X.sh
+000020b0: 6170 6529 0a20 2020 2020 2020 2020 2020  ape).           
+000020c0: 2049 6620 7261 6e64 6f6d 697a 6564 203a   If randomized :
+000020d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000020e0: 2072 756e 2072 616e 646f 6d69 7a65 6420   run randomized 
+000020f0: 5356 4420 6279 2074 6865 206d 6574 686f  SVD by the metho
+00002100: 6420 6f66 2048 616c 6b6f 2065 7420 616c  d of Halko et al
+00002110: 2e0a 0a20 2020 2020 2020 2020 2020 202e  ...            .
+00002120: 2e20 7665 7273 696f 6e61 6464 6564 3a3a  . versionadded::
+00002130: 2030 2e31 382e 300a 0a20 2020 2020 2020   0.18.0..       
+00002140: 2074 6f6c 203a 2066 6c6f 6174 2c20 6465   tol : float, de
+00002150: 6661 756c 743d 302e 300a 2020 2020 2020  fault=0.0.      
+00002160: 2020 2020 2020 546f 6c65 7261 6e63 6520        Tolerance 
+00002170: 666f 7220 7369 6e67 756c 6172 2076 616c  for singular val
+00002180: 7565 7320 636f 6d70 7574 6564 2062 7920  ues computed by 
+00002190: 7376 645f 736f 6c76 6572 203d 3d20 2761  svd_solver == 'a
+000021a0: 7270 6163 6b27 2e0a 2020 2020 2020 2020  rpack'..        
+000021b0: 2020 2020 4d75 7374 2062 6520 6f66 2072      Must be of r
+000021c0: 616e 6765 205b 302e 302c 2069 6e66 696e  ange [0.0, infin
+000021d0: 6974 7929 2e0a 0a20 2020 2020 2020 2020  ity)...         
+000021e0: 2020 202e 2e20 7665 7273 696f 6e61 6464     .. versionadd
+000021f0: 6564 3a3a 2030 2e31 382e 300a 0a20 2020  ed:: 0.18.0..   
+00002200: 2020 2020 2069 7465 7261 7465 645f 706f       iterated_po
+00002210: 7765 7220 3a20 696e 7420 6f72 2027 6175  wer : int or 'au
+00002220: 746f 272c 2064 6566 6175 6c74 3d27 6175  to', default='au
+00002230: 746f 270a 2020 2020 2020 2020 2020 2020  to'.            
+00002240: 4e75 6d62 6572 206f 6620 6974 6572 6174  Number of iterat
+00002250: 696f 6e73 2066 6f72 2074 6865 2070 6f77  ions for the pow
+00002260: 6572 206d 6574 686f 6420 636f 6d70 7574  er method comput
+00002270: 6564 2062 790a 2020 2020 2020 2020 2020  ed by.          
+00002280: 2020 7376 645f 736f 6c76 6572 203d 3d20    svd_solver == 
+00002290: 2772 616e 646f 6d69 7a65 6427 2e0a 2020  'randomized'..  
+000022a0: 2020 2020 2020 2020 2020 4d75 7374 2062            Must b
+000022b0: 6520 6f66 2072 616e 6765 205b 302c 2069  e of range [0, i
+000022c0: 6e66 696e 6974 7929 2e0a 0a20 2020 2020  nfinity)...     
+000022d0: 2020 2020 2020 202e 2e20 7665 7273 696f         .. versio
+000022e0: 6e61 6464 6564 3a3a 2030 2e31 382e 300a  nadded:: 0.18.0.
+000022f0: 0a20 2020 2020 2020 206e 5f6f 7665 7273  .        n_overs
+00002300: 616d 706c 6573 203a 2069 6e74 2c20 6465  amples : int, de
+00002310: 6661 756c 743d 3130 0a20 2020 2020 2020  fault=10.       
+00002320: 2020 2020 2054 6869 7320 7061 7261 6d65       This parame
+00002330: 7465 7220 6973 206f 6e6c 7920 7265 6c65  ter is only rele
+00002340: 7661 6e74 2077 6865 6e20 6073 7664 5f73  vant when `svd_s
+00002350: 6f6c 7665 723d 2272 616e 646f 6d69 7a65  olver="randomize
+00002360: 6422 602e 0a20 2020 2020 2020 2020 2020  d"`..           
+00002370: 2049 7420 636f 7272 6573 706f 6e64 7320   It corresponds 
+00002380: 746f 2074 6865 2061 6464 6974 696f 6e61  to the additiona
+00002390: 6c20 6e75 6d62 6572 206f 6620 7261 6e64  l number of rand
+000023a0: 6f6d 2076 6563 746f 7273 2074 6f20 7361  om vectors to sa
+000023b0: 6d70 6c65 2074 6865 0a20 2020 2020 2020  mple the.       
+000023c0: 2020 2020 2072 616e 6765 206f 6620 6058       range of `X
+000023d0: 6020 736f 2061 7320 746f 2065 6e73 7572  ` so as to ensur
+000023e0: 6520 7072 6f70 6572 2063 6f6e 6469 7469  e proper conditi
+000023f0: 6f6e 696e 672e 2053 6565 0a20 2020 2020  oning. See.     
+00002400: 2020 2020 2020 203a 6675 6e63 3a60 7e73         :func:`~s
+00002410: 6b6c 6561 726e 2e75 7469 6c73 2e65 7874  klearn.utils.ext
+00002420: 6d61 7468 2e72 616e 646f 6d69 7a65 645f  math.randomized_
+00002430: 7376 6460 2066 6f72 206d 6f72 6520 6465  svd` for more de
+00002440: 7461 696c 732e 0a0a 2020 2020 2020 2020  tails...        
+00002450: 2020 2020 2e2e 2076 6572 7369 6f6e 6164      .. versionad
+00002460: 6465 643a 3a20 312e 310a 0a20 2020 2020  ded:: 1.1..     
+00002470: 2020 2070 6f77 6572 5f69 7465 7261 7469     power_iterati
+00002480: 6f6e 5f6e 6f72 6d61 6c69 7a65 7220 3a20  on_normalizer : 
+00002490: 7b27 6175 746f 272c 2027 5152 272c 2027  {'auto', 'QR', '
+000024a0: 4c55 272c 2027 6e6f 6e65 277d 2c20 6465  LU', 'none'}, de
+000024b0: 6661 756c 743d 2761 7574 6f27 0a20 2020  fault='auto'.   
+000024c0: 2020 2020 2020 2020 2050 6f77 6572 2069           Power i
+000024d0: 7465 7261 7469 6f6e 206e 6f72 6d61 6c69  teration normali
+000024e0: 7a65 7220 666f 7220 7261 6e64 6f6d 697a  zer for randomiz
+000024f0: 6564 2053 5644 2073 6f6c 7665 722e 0a20  ed SVD solver.. 
+00002500: 2020 2020 2020 2020 2020 204e 6f74 2075             Not u
+00002510: 7365 6420 6279 2041 5250 4143 4b2e 2053  sed by ARPACK. S
+00002520: 6565 203a 6675 6e63 3a60 7e73 6b6c 6561  ee :func:`~sklea
+00002530: 726e 2e75 7469 6c73 2e65 7874 6d61 7468  rn.utils.extmath
+00002540: 2e72 616e 646f 6d69 7a65 645f 7376 6460  .randomized_svd`
+00002550: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00002560: 206d 6f72 6520 6465 7461 696c 732e 0a0a   more details...
+00002570: 2020 2020 2020 2020 2020 2020 2e2e 2076              .. v
+00002580: 6572 7369 6f6e 6164 6465 643a 3a20 312e  ersionadded:: 1.
+00002590: 310a 0a20 2020 2020 2020 2072 616e 646f  1..        rando
+000025a0: 6d5f 7374 6174 6520 3a20 696e 742c 2052  m_state : int, R
+000025b0: 616e 646f 6d53 7461 7465 2069 6e73 7461  andomState insta
+000025c0: 6e63 6520 6f72 204e 6f6e 652c 2064 6566  nce or None, def
+000025d0: 6175 6c74 3d4e 6f6e 650a 2020 2020 2020  ault=None.      
+000025e0: 2020 2020 2020 5573 6564 2077 6865 6e20        Used when 
+000025f0: 7468 6520 2761 7270 6163 6b27 206f 7220  the 'arpack' or 
+00002600: 2772 616e 646f 6d69 7a65 6427 2073 6f6c  'randomized' sol
+00002610: 7665 7273 2061 7265 2075 7365 642e 2050  vers are used. P
+00002620: 6173 7320 616e 2069 6e74 0a20 2020 2020  ass an int.     
+00002630: 2020 2020 2020 2066 6f72 2072 6570 726f         for repro
+00002640: 6475 6369 626c 6520 7265 7375 6c74 7320  ducible results 
+00002650: 6163 726f 7373 206d 756c 7469 706c 6520  across multiple 
+00002660: 6675 6e63 7469 6f6e 2063 616c 6c73 2e0a  function calls..
+00002670: 2020 2020 2020 2020 2020 2020 5365 6520              See 
+00002680: 3a74 6572 6d3a 6047 6c6f 7373 6172 7920  :term:`Glossary 
+00002690: 3c72 616e 646f 6d5f 7374 6174 653e 602e  <random_state>`.
+000026a0: 0a0a 2020 2020 2020 2020 2020 2020 2e2e  ..            ..
+000026b0: 2076 6572 7369 6f6e 6164 6465 643a 3a20   versionadded:: 
+000026c0: 302e 3138 2e30 0a0a 2020 2020 2020 2020  0.18.0..        
+000026d0: 5265 6665 7265 6e63 6573 0a20 2020 2020  References.     
+000026e0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+000026f0: 2020 2020 2020 5363 696b 6974 2d6c 6561        Scikit-lea
+00002700: 726e 2041 5049 3a20 736b 6c65 6172 6e2e  rn API: sklearn.
+00002710: 6465 636f 6d70 6f73 6974 696f 6e2e 5043  decomposition.PC
+00002720: 410a 2020 2020 2020 2020 6874 7470 733a  A.        https:
+00002730: 2f2f 7363 696b 6974 2d6c 6561 726e 2e6f  //scikit-learn.o
+00002740: 7267 2f73 7461 626c 652f 6d6f 6475 6c65  rg/stable/module
+00002750: 732f 6765 6e65 7261 7465 642f 736b 6c65  s/generated/skle
+00002760: 6172 6e2e 6465 636f 6d70 6f73 6974 696f  arn.decompositio
+00002770: 6e2e 5043 412e 6874 6d6c 0a20 2020 2020  n.PCA.html.     
+00002780: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
+00002790: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
+000027a0: 290a 2020 2020 2020 2020 7365 6c66 2e6e  ).        self.n
+000027b0: 5f63 6f6d 706f 6e65 6e74 7320 3d20 6e5f  _components = n_
+000027c0: 636f 6d70 6f6e 656e 7473 0a20 2020 2020  components.     
+000027d0: 2020 2073 656c 662e 636f 7079 203d 2063     self.copy = c
+000027e0: 6f70 790a 2020 2020 2020 2020 7365 6c66  opy.        self
+000027f0: 2e77 6869 7465 6e20 3d20 7768 6974 656e  .whiten = whiten
+00002800: 0a20 2020 2020 2020 2073 656c 662e 7376  .        self.sv
+00002810: 645f 736f 6c76 6572 203d 2073 7664 5f73  d_solver = svd_s
+00002820: 6f6c 7665 720a 2020 2020 2020 2020 7365  olver.        se
+00002830: 6c66 2e74 6f6c 203d 2074 6f6c 0a20 2020  lf.tol = tol.   
+00002840: 2020 2020 2073 656c 662e 6974 6572 6174       self.iterat
+00002850: 6564 5f70 6f77 6572 203d 2069 7465 7261  ed_power = itera
+00002860: 7465 645f 706f 7765 720a 2020 2020 2020  ted_power.      
+00002870: 2020 2320 7365 6c66 2e6e 5f6f 7665 7273    # self.n_overs
+00002880: 616d 706c 6573 203d 206e 5f6f 7665 7273  amples = n_overs
+00002890: 616d 706c 6573 0a20 2020 2020 2020 2023  amples.        #
+000028a0: 2073 656c 662e 706f 7765 725f 6974 6572   self.power_iter
+000028b0: 6174 696f 6e5f 6e6f 726d 616c 697a 6572  ation_normalizer
+000028c0: 203d 2070 6f77 6572 5f69 7465 7261 7469   = power_iterati
+000028d0: 6f6e 5f6e 6f72 6d61 6c69 7a65 720a 0a20  on_normalizer.. 
+000028e0: 2020 2020 2020 2069 6620 7261 6e64 6f6d         if random
+000028f0: 5f73 7461 7465 3a0a 2020 2020 2020 2020  _state:.        
+00002900: 2020 2020 7365 6c66 2e72 616e 646f 6d5f      self.random_
+00002910: 7374 6174 6520 3d20 7261 6e64 6f6d 5f73  state = random_s
+00002920: 7461 7465 0a0a 2020 2020 2020 2020 2320  tate..        # 
+00002930: 4966 2027 7261 6e64 6f6d 5f73 7461 7465  If 'random_state
+00002940: 2720 6973 204e 6f6e 652c 2027 7365 6c66  ' is None, 'self
+00002950: 2e72 616e 646f 6d5f 7374 6174 6527 2063  .random_state' c
+00002960: 6f6d 6573 2066 726f 6d20 7468 6520 7061  omes from the pa
+00002970: 7265 6e74 2063 6c61 7373 2027 576f 726b  rent class 'Work
+00002980: 666c 6f77 4261 7365 270a 2020 2020 2020  flowBase'.      
+00002990: 2020 7365 6c66 2e6d 6f64 656c 203d 2050    self.model = P
+000029a0: 4341 280a 2020 2020 2020 2020 2020 2020  CA(.            
+000029b0: 6e5f 636f 6d70 6f6e 656e 7473 3d73 656c  n_components=sel
+000029c0: 662e 6e5f 636f 6d70 6f6e 656e 7473 2c0a  f.n_components,.
+000029d0: 2020 2020 2020 2020 2020 2020 636f 7079              copy
+000029e0: 3d73 656c 662e 636f 7079 2c0a 2020 2020  =self.copy,.    
+000029f0: 2020 2020 2020 2020 7768 6974 656e 3d73          whiten=s
+00002a00: 656c 662e 7768 6974 656e 2c0a 2020 2020  elf.whiten,.    
+00002a10: 2020 2020 2020 2020 7376 645f 736f 6c76          svd_solv
+00002a20: 6572 3d73 656c 662e 7376 645f 736f 6c76  er=self.svd_solv
+00002a30: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+00002a40: 746f 6c3d 7365 6c66 2e74 6f6c 2c0a 2020  tol=self.tol,.  
+00002a50: 2020 2020 2020 2020 2020 6974 6572 6174            iterat
+00002a60: 6564 5f70 6f77 6572 3d73 656c 662e 6974  ed_power=self.it
+00002a70: 6572 6174 6564 5f70 6f77 6572 2c0a 2020  erated_power,.  
+00002a80: 2020 2020 2020 2020 2020 2320 6e5f 6f76            # n_ov
+00002a90: 6572 7361 6d70 6c65 733d 7365 6c66 2e6e  ersamples=self.n
+00002aa0: 5f6f 7665 7273 616d 706c 6573 2c0a 2020  _oversamples,.  
+00002ab0: 2020 2020 2020 2020 2020 2320 706f 7765            # powe
+00002ac0: 725f 6974 6572 6174 696f 6e5f 6e6f 726d  r_iteration_norm
+00002ad0: 616c 697a 6572 3d73 656c 662e 706f 7765  alizer=self.powe
+00002ae0: 725f 6974 6572 6174 696f 6e5f 6e6f 726d  r_iteration_norm
+00002af0: 616c 697a 6572 2c0a 2020 2020 2020 2020  alizer,.        
+00002b00: 2020 2020 7261 6e64 6f6d 5f73 7461 7465      random_state
+00002b10: 3d73 656c 662e 7261 6e64 6f6d 5f73 7461  =self.random_sta
+00002b20: 7465 2c0a 2020 2020 2020 2020 290a 0a20  te,.        ).. 
+00002b30: 2020 2020 2020 2073 656c 662e 6e61 6d69         self.nami
+00002b40: 6e67 203d 2050 4341 4465 636f 6d70 6f73  ng = PCADecompos
+00002b50: 6974 696f 6e2e 6e61 6d65 0a0a 2020 2020  ition.name..    
+00002b60: 2020 2020 2320 7370 6563 6961 6c20 6174      # special at
+00002b70: 7472 6962 7574 6573 0a20 2020 2020 2020  tributes.       
+00002b80: 2073 656c 662e 7063 5f64 6174 6120 3d20   self.pc_data = 
+00002b90: 4e6f 6e65 0a0a 2020 2020 4063 6c61 7373  None..    @class
+00002ba0: 6d65 7468 6f64 0a20 2020 2064 6566 206d  method.    def m
+00002bb0: 616e 7561 6c5f 6879 7065 725f 7061 7261  anual_hyper_para
+00002bc0: 6d65 7465 7273 2863 6c73 2920 2d3e 2044  meters(cls) -> D
+00002bd0: 6963 743a 0a20 2020 2020 2020 2022 2222  ict:.        """
+00002be0: 4d61 6e75 616c 2068 7970 6572 2d70 6172  Manual hyper-par
+00002bf0: 616d 6574 6572 7320 7370 6563 6966 6963  ameters specific
+00002c00: 6174 696f 6e2e 2222 220a 2020 2020 2020  ation.""".      
+00002c10: 2020 7072 696e 7428 6622 2d2a 2d2a 2d20    print(f"-*-*- 
+00002c20: 7b63 6c73 2e6e 616d 657d 202d 2048 7970  {cls.name} - Hyp
+00002c30: 6572 2d70 6172 616d 6574 6572 7320 5370  er-parameters Sp
+00002c40: 6563 6966 6963 6174 696f 6e20 2d2a 2d2a  ecification -*-*
+00002c50: 2d22 290a 2020 2020 2020 2020 6879 7065  -").        hype
+00002c60: 725f 7061 7261 6d65 7465 7273 203d 2070  r_parameters = p
+00002c70: 6361 5f6d 616e 7561 6c5f 6879 7065 725f  ca_manual_hyper_
+00002c80: 7061 7261 6d65 7465 7273 2829 0a20 2020  parameters().   
+00002c90: 2020 2020 2063 6c65 6172 5f6f 7574 7075       clear_outpu
+00002ca0: 7428 290a 2020 2020 2020 2020 7265 7475  t().        retu
+00002cb0: 726e 2068 7970 6572 5f70 6172 616d 6574  rn hyper_paramet
+00002cc0: 6572 730a 0a20 2020 2064 6566 205f 6765  ers..    def _ge
+00002cd0: 745f 7072 696e 6369 7061 6c5f 636f 6d70  t_principal_comp
+00002ce0: 6f6e 656e 7473 2873 656c 6629 202d 3e20  onents(self) -> 
+00002cf0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00002d00: 2247 6574 2070 7269 6e63 6970 616c 2063  "Get principal c
+00002d10: 6f6d 706f 6e65 6e74 732e 2222 220a 2020  omponents.""".  
+00002d20: 2020 2020 2020 7072 696e 7428 222d 2d2d        print("---
+00002d30: 2d2d 2a20 5072 696e 6369 7061 6c20 436f  --* Principal Co
+00002d40: 6d70 6f6e 656e 7473 202a 2d2d 2d2d 2d22  mponents *-----"
+00002d50: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
+00002d60: 2245 7665 7279 2063 6f6c 756d 6e20 7265  "Every column re
+00002d70: 7072 6573 656e 7473 206f 6e65 2070 7269  presents one pri
+00002d80: 6e63 6970 616c 2063 6f6d 706f 6e65 6e74  ncipal component
+00002d90: 2072 6573 7065 6374 6976 656c 792e 2229   respectively.")
+00002da0: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+00002db0: 4576 6572 7920 726f 7720 7265 7072 6573  Every row repres
+00002dc0: 656e 7473 2068 6f77 206d 7563 6820 7468  ents how much th
+00002dd0: 6174 2072 6f77 2066 6561 7475 7265 2063  at row feature c
+00002de0: 6f6e 7472 6962 7574 6573 2074 6f20 6561  ontributes to ea
+00002df0: 6368 2070 7269 6e63 6970 616c 2063 6f6d  ch principal com
+00002e00: 706f 6e65 6e74 2072 6573 7065 6374 6976  ponent respectiv
+00002e10: 656c 792e 2229 0a20 2020 2020 2020 2070  ely.").        p
+00002e20: 7269 6e74 2822 5468 6520 7461 6275 6c61  rint("The tabula
+00002e30: 7220 6461 7461 206c 6f6f 6b73 206c 696b  r data looks lik
+00002e40: 6520 696e 2066 6f72 6d61 743a 2027 726f  e in format: 'ro
+00002e50: 7773 2078 2063 6f6c 756d 6e73 203d 2027  ws x columns = '
+00002e60: 6665 6174 7572 6573 2078 2070 7269 6e63  features x princ
+00002e70: 6970 616c 2063 6f6d 706f 6e65 6e74 7327  ipal components'
+00002e80: 2e22 290a 2020 2020 2020 2020 7063 5f6e  .").        pc_n
+00002e90: 616d 6520 3d20 5b5d 0a20 2020 2020 2020  ame = [].       
+00002ea0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00002eb0: 7365 6c66 2e6e 5f63 6f6d 706f 6e65 6e74  self.n_component
+00002ec0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00002ed0: 7063 5f6e 616d 652e 6170 7065 6e64 2866  pc_name.append(f
+00002ee0: 2250 437b 692b 317d 2229 0a20 2020 2020  "PC{i+1}").     
+00002ef0: 2020 2073 656c 662e 7063 5f64 6174 6120     self.pc_data 
+00002f00: 3d20 7064 2e44 6174 6146 7261 6d65 2873  = pd.DataFrame(s
+00002f10: 656c 662e 6d6f 6465 6c2e 636f 6d70 6f6e  elf.model.compon
+00002f20: 656e 7473 5f2e 5429 0a20 2020 2020 2020  ents_.T).       
+00002f30: 2073 656c 662e 7063 5f64 6174 612e 636f   self.pc_data.co
+00002f40: 6c75 6d6e 7320 3d20 7063 5f6e 616d 650a  lumns = pc_name.
+00002f50: 2020 2020 2020 2020 7365 6c66 2e70 635f          self.pc_
+00002f60: 6461 7461 2e73 6574 5f69 6e64 6578 2844  data.set_index(D
+00002f70: 6563 6f6d 706f 7369 7469 6f6e 576f 726b  ecompositionWork
+00002f80: 666c 6f77 4261 7365 2e58 2e63 6f6c 756d  flowBase.X.colum
+00002f90: 6e73 2c20 696e 706c 6163 653d 5472 7565  ns, inplace=True
+00002fa0: 290a 2020 2020 2020 2020 7072 696e 7428  ).        print(
+00002fb0: 7365 6c66 2e70 635f 6461 7461 290a 0a20  self.pc_data).. 
+00002fc0: 2020 2064 6566 205f 6765 745f 6578 706c     def _get_expl
+00002fd0: 6169 6e65 645f 7661 7269 616e 6365 5f72  ained_variance_r
+00002fe0: 6174 696f 2873 656c 6629 202d 3e20 4e6f  atio(self) -> No
+00002ff0: 6e65 3a0a 2020 2020 2020 2020 2222 2247  ne:.        """G
+00003000: 6574 2065 7870 6c61 696e 6564 2076 6172  et explained var
+00003010: 6961 6e63 6520 7261 7469 6f2e 2222 220a  iance ratio.""".
+00003020: 2020 2020 2020 2020 7072 696e 7428 222d          print("-
+00003030: 2d2d 2d2d 2a20 4578 706c 6169 6e65 6420  ----* Explained 
+00003040: 5661 7269 616e 6365 2052 6174 696f 202a  Variance Ratio *
+00003050: 2d2d 2d2d 2d22 290a 2020 2020 2020 2020  -----").        
+00003060: 7072 696e 7428 7365 6c66 2e6d 6f64 656c  print(self.model
+00003070: 2e65 7870 6c61 696e 6564 5f76 6172 6961  .explained_varia
+00003080: 6e63 655f 7261 7469 6f5f 290a 0a20 2020  nce_ratio_)..   
+00003090: 2040 7374 6174 6963 6d65 7468 6f64 0a20   @staticmethod. 
+000030a0: 2020 2064 6566 205f 6269 706c 6f74 2872     def _biplot(r
+000030b0: 6564 7563 6564 5f64 6174 613a 2070 642e  educed_data: pd.
+000030c0: 4461 7461 4672 616d 652c 2070 635f 6461  DataFrame, pc_da
+000030d0: 7461 3a20 7064 2e44 6174 6146 7261 6d65  ta: pd.DataFrame
+000030e0: 2c20 616c 676f 7269 7468 6d5f 6e61 6d65  , algorithm_name
+000030f0: 3a20 7374 722c 206c 6f63 616c 5f70 6174  : str, local_pat
+00003100: 683a 2073 7472 2c20 6d6c 666c 6f77 5f70  h: str, mlflow_p
+00003110: 6174 683a 2073 7472 2920 2d3e 204e 6f6e  ath: str) -> Non
+00003120: 653a 0a20 2020 2020 2020 2022 2222 4472  e:.        """Dr
+00003130: 6177 2062 692d 706c 6f74 2e22 2222 0a20  aw bi-plot.""". 
+00003140: 2020 2020 2020 2070 7269 6e74 2822 2d2d         print("--
+00003150: 2d2d 2d2a 2043 6f6d 706f 7369 7469 6f6e  ---* Composition
+00003160: 616c 2042 692d 706c 6f74 202a 2d2d 2d2d  al Bi-plot *----
+00003170: 2d22 290a 2020 2020 2020 2020 6269 706c  -").        bipl
+00003180: 6f74 2872 6564 7563 6564 5f64 6174 612c  ot(reduced_data,
+00003190: 2070 635f 6461 7461 2c20 616c 676f 7269   pc_data, algori
+000031a0: 7468 6d5f 6e61 6d65 290a 2020 2020 2020  thm_name).      
+000031b0: 2020 7361 7665 5f66 6967 2866 2243 6f6d    save_fig(f"Com
+000031c0: 706f 7369 7469 6f6e 616c 2042 692d 706c  positional Bi-pl
+000031d0: 6f74 202d 207b 616c 676f 7269 7468 6d5f  ot - {algorithm_
+000031e0: 6e61 6d65 7d22 2c20 6c6f 6361 6c5f 7061  name}", local_pa
+000031f0: 7468 2c20 6d6c 666c 6f77 5f70 6174 6829  th, mlflow_path)
+00003200: 0a20 2020 2020 2020 2073 6176 655f 6461  .        save_da
+00003210: 7461 2872 6564 7563 6564 5f64 6174 612c  ta(reduced_data,
+00003220: 2022 436f 6d70 6f73 6974 696f 6e61 6c20   "Compositional 
+00003230: 4269 2d70 6c6f 7420 2d20 5265 6475 6365  Bi-plot - Reduce
+00003240: 6420 4461 7461 222c 206c 6f63 616c 5f70  d Data", local_p
+00003250: 6174 682c 206d 6c66 6c6f 775f 7061 7468  ath, mlflow_path
+00003260: 290a 2020 2020 2020 2020 7361 7665 5f64  ).        save_d
+00003270: 6174 6128 7063 5f64 6174 612c 2022 436f  ata(pc_data, "Co
+00003280: 6d70 6f73 6974 696f 6e61 6c20 4269 2d70  mpositional Bi-p
+00003290: 6c6f 7420 2d20 5043 2044 6174 6122 2c20  lot - PC Data", 
+000032a0: 6c6f 6361 6c5f 7061 7468 2c20 6d6c 666c  local_path, mlfl
+000032b0: 6f77 5f70 6174 6829 0a0a 2020 2020 4073  ow_path)..    @s
+000032c0: 7461 7469 636d 6574 686f 640a 2020 2020  taticmethod.    
+000032d0: 6465 6620 5f74 7269 706c 6f74 2872 6564  def _triplot(red
+000032e0: 7563 6564 5f64 6174 613a 2070 642e 4461  uced_data: pd.Da
+000032f0: 7461 4672 616d 652c 2070 635f 6461 7461  taFrame, pc_data
+00003300: 3a20 7064 2e44 6174 6146 7261 6d65 2c20  : pd.DataFrame, 
+00003310: 616c 676f 7269 7468 6d5f 6e61 6d65 3a20  algorithm_name: 
+00003320: 7374 722c 206c 6f63 616c 5f70 6174 683a  str, local_path:
+00003330: 2073 7472 2c20 6d6c 666c 6f77 5f70 6174   str, mlflow_pat
+00003340: 683a 2073 7472 2920 2d3e 204e 6f6e 653a  h: str) -> None:
+00003350: 0a20 2020 2020 2020 2022 2222 4472 6177  .        """Draw
+00003360: 2074 7269 2d70 6c6f 742e 2222 220a 2020   tri-plot.""".  
+00003370: 2020 2020 2020 7072 696e 7428 222d 2d2d        print("---
+00003380: 2d2d 2a20 436f 6d70 6f73 6974 696f 6e61  --* Compositiona
+00003390: 6c20 5472 692d 706c 6f74 202a 2d2d 2d2d  l Tri-plot *----
+000033a0: 2d22 290a 2020 2020 2020 2020 7472 6970  -").        trip
+000033b0: 6c6f 7428 7265 6475 6365 645f 6461 7461  lot(reduced_data
+000033c0: 2c20 7063 5f64 6174 612c 2061 6c67 6f72  , pc_data, algor
+000033d0: 6974 686d 5f6e 616d 6529 0a20 2020 2020  ithm_name).     
+000033e0: 2020 2073 6176 655f 6669 6728 6622 436f     save_fig(f"Co
+000033f0: 6d70 6f73 6974 696f 6e61 6c20 5472 692d  mpositional Tri-
+00003400: 706c 6f74 202d 207b 616c 676f 7269 7468  plot - {algorith
+00003410: 6d5f 6e61 6d65 7d22 2c20 6c6f 6361 6c5f  m_name}", local_
+00003420: 7061 7468 2c20 6d6c 666c 6f77 5f70 6174  path, mlflow_pat
+00003430: 6829 0a20 2020 2020 2020 2073 6176 655f  h).        save_
+00003440: 6461 7461 2872 6564 7563 6564 5f64 6174  data(reduced_dat
+00003450: 612c 2022 436f 6d70 6f73 6974 696f 6e61  a, "Compositiona
+00003460: 6c20 5472 692d 706c 6f74 202d 2052 6564  l Tri-plot - Red
+00003470: 7563 6564 2044 6174 6122 2c20 6c6f 6361  uced Data", loca
+00003480: 6c5f 7061 7468 2c20 6d6c 666c 6f77 5f70  l_path, mlflow_p
+00003490: 6174 6829 0a20 2020 2020 2020 2073 6176  ath).        sav
+000034a0: 655f 6461 7461 2870 635f 6461 7461 2c20  e_data(pc_data, 
+000034b0: 2243 6f6d 706f 7369 7469 6f6e 616c 2054  "Compositional T
+000034c0: 7269 2d70 6c6f 7420 2d20 5043 2044 6174  ri-plot - PC Dat
+000034d0: 6122 2c20 6c6f 6361 6c5f 7061 7468 2c20  a", local_path, 
+000034e0: 6d6c 666c 6f77 5f70 6174 6829 0a0a 2020  mlflow_path)..  
+000034f0: 2020 6465 6620 7370 6563 6961 6c5f 636f    def special_co
+00003500: 6d70 6f6e 656e 7473 2873 656c 662c 202a  mponents(self, *
+00003510: 2a6b 7761 7267 733a 2055 6e69 6f6e 5b44  *kwargs: Union[D
+00003520: 6963 742c 206e 702e 6e64 6172 7261 792c  ict, np.ndarray,
+00003530: 2069 6e74 5d29 202d 3e20 4e6f 6e65 3a0a   int]) -> None:.
+00003540: 2020 2020 2020 2020 2222 2249 6e76 6f6b          """Invok
+00003550: 6520 616c 6c20 7370 6563 6961 6c20 6170  e all special ap
+00003560: 706c 6963 6174 696f 6e20 6675 6e63 7469  plication functi
+00003570: 6f6e 7320 666f 7220 7468 6973 2061 6c67  ons for this alg
+00003580: 6f72 6974 686d 7320 6279 2053 6369 6b69  orithms by Sciki
+00003590: 742d 6c65 6172 6e20 6672 616d 6577 6f72  t-learn framewor
+000035a0: 6b2e 2222 220a 2020 2020 2020 2020 7365  k.""".        se
+000035b0: 6c66 2e5f 7265 6475 6365 645f 6461 7461  lf._reduced_data
+000035c0: 3270 6428 6b77 6172 6773 5b22 7265 6475  2pd(kwargs["redu
+000035d0: 6365 645f 6461 7461 225d 2c20 6b77 6172  ced_data"], kwar
+000035e0: 6773 5b22 636f 6d70 6f6e 656e 7473 5f6e  gs["components_n
+000035f0: 756d 225d 290a 2020 2020 2020 2020 7365  um"]).        se
+00003600: 6c66 2e5f 6765 745f 7072 696e 6369 7061  lf._get_principa
+00003610: 6c5f 636f 6d70 6f6e 656e 7473 2829 0a20  l_components(). 
+00003620: 2020 2020 2020 2073 656c 662e 5f67 6574         self._get
+00003630: 5f65 7870 6c61 696e 6564 5f76 6172 6961  _explained_varia
+00003640: 6e63 655f 7261 7469 6f28 290a 0a20 2020  nce_ratio()..   
+00003650: 2020 2020 2047 454f 5049 5f4f 5554 5055       GEOPI_OUTPU
+00003660: 545f 4152 5449 4641 4354 535f 494d 4147  T_ARTIFACTS_IMAG
+00003670: 455f 4d4f 4445 4c5f 4f55 5450 5554 5f50  E_MODEL_OUTPUT_P
+00003680: 4154 4820 3d20 6f73 2e67 6574 656e 7628  ATH = os.getenv(
+00003690: 2247 454f 5049 5f4f 5554 5055 545f 4152  "GEOPI_OUTPUT_AR
+000036a0: 5449 4641 4354 535f 494d 4147 455f 4d4f  TIFACTS_IMAGE_MO
+000036b0: 4445 4c5f 4f55 5450 5554 5f50 4154 4822  DEL_OUTPUT_PATH"
+000036c0: 290a 2020 2020 2020 2020 2320 4472 6177  ).        # Draw
+000036d0: 2067 7261 7068 7320 7768 656e 2074 6865   graphs when the
+000036e0: 206e 756d 6265 7220 6f66 2070 7269 6e63   number of princ
+000036f0: 6970 616c 2063 6f6d 706f 6e65 6e74 7320  ipal components 
+00003700: 3e20 330a 2020 2020 2020 2020 6966 206b  > 3.        if k
+00003710: 7761 7267 735b 2263 6f6d 706f 6e65 6e74  wargs["component
+00003720: 735f 6e75 6d22 5d20 3e20 333a 0a20 2020  s_num"] > 3:.   
+00003730: 2020 2020 2020 2020 2023 2063 686f 6f73           # choos
+00003740: 6520 7477 6f20 6f66 2064 696d 656e 7369  e two of dimensi
+00003750: 6f6e 7320 746f 2064 7261 770a 2020 2020  ons to draw.    
+00003760: 2020 2020 2020 2020 7477 6f5f 6469 6d65          two_dime
+00003770: 6e5f 6178 6973 5f69 6e64 6578 2c20 7477  n_axis_index, tw
+00003780: 6f5f 6469 6d65 6e5f 7063 5f64 6174 6120  o_dimen_pc_data 
+00003790: 3d20 7365 6c66 2e63 686f 6f73 655f 6469  = self.choose_di
+000037a0: 6d65 6e73 696f 6e5f 6461 7461 2873 656c  mension_data(sel
+000037b0: 662e 7063 5f64 6174 612c 2032 290a 2020  f.pc_data, 2).  
+000037c0: 2020 2020 2020 2020 2020 7477 6f5f 6469            two_di
+000037d0: 6d65 6e5f 7265 6475 6365 645f 6461 7461  men_reduced_data
+000037e0: 203d 2073 656c 662e 585f 7265 6475 6365   = self.X_reduce
+000037f0: 642e 696c 6f63 5b3a 2c20 7477 6f5f 6469  d.iloc[:, two_di
+00003800: 6d65 6e5f 6178 6973 5f69 6e64 6578 5d0a  men_axis_index].
+00003810: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003820: 2e5f 6269 706c 6f74 280a 2020 2020 2020  ._biplot(.      
+00003830: 2020 2020 2020 2020 2020 7265 6475 6365            reduce
+00003840: 645f 6461 7461 3d74 776f 5f64 696d 656e  d_data=two_dimen
+00003850: 5f72 6564 7563 6564 5f64 6174 612c 0a20  _reduced_data,. 
+00003860: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00003870: 635f 6461 7461 3d74 776f 5f64 696d 656e  c_data=two_dimen
+00003880: 5f70 635f 6461 7461 2c0a 2020 2020 2020  _pc_data,.      
+00003890: 2020 2020 2020 2020 2020 616c 676f 7269            algori
+000038a0: 7468 6d5f 6e61 6d65 3d73 656c 662e 6e61  thm_name=self.na
+000038b0: 6d69 6e67 2c0a 2020 2020 2020 2020 2020  ming,.          
+000038c0: 2020 2020 2020 6c6f 6361 6c5f 7061 7468        local_path
+000038d0: 3d47 454f 5049 5f4f 5554 5055 545f 4152  =GEOPI_OUTPUT_AR
+000038e0: 5449 4641 4354 535f 494d 4147 455f 4d4f  TIFACTS_IMAGE_MO
+000038f0: 4445 4c5f 4f55 5450 5554 5f50 4154 482c  DEL_OUTPUT_PATH,
+00003900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003910: 206d 6c66 6c6f 775f 7061 7468 3d4d 4c46   mlflow_path=MLF
+00003920: 4c4f 575f 4152 5449 4641 4354 5f49 4d41  LOW_ARTIFACT_IMA
+00003930: 4745 5f4d 4f44 454c 5f4f 5554 5055 545f  GE_MODEL_OUTPUT_
+00003940: 5041 5448 2c0a 2020 2020 2020 2020 2020  PATH,.          
+00003950: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
+00003960: 2023 2063 686f 6f73 6520 7468 7265 6520   # choose three 
+00003970: 6f66 2064 696d 656e 7369 6f6e 7320 746f  of dimensions to
+00003980: 2064 7261 770a 2020 2020 2020 2020 2020   draw.          
+00003990: 2020 7468 7265 655f 6469 6d65 6e5f 6178    three_dimen_ax
+000039a0: 6973 5f69 6e64 6578 2c20 7468 7265 655f  is_index, three_
+000039b0: 6469 6d65 6e5f 7063 5f64 6174 6120 3d20  dimen_pc_data = 
+000039c0: 7365 6c66 2e63 686f 6f73 655f 6469 6d65  self.choose_dime
+000039d0: 6e73 696f 6e5f 6461 7461 2873 656c 662e  nsion_data(self.
+000039e0: 7063 5f64 6174 612c 2033 290a 2020 2020  pc_data, 3).    
+000039f0: 2020 2020 2020 2020 7468 7265 655f 6469          three_di
+00003a00: 6d65 6e5f 7265 6475 6365 645f 6461 7461  men_reduced_data
+00003a10: 203d 2073 656c 662e 585f 7265 6475 6365   = self.X_reduce
+00003a20: 642e 696c 6f63 5b3a 2c20 7468 7265 655f  d.iloc[:, three_
+00003a30: 6469 6d65 6e5f 6178 6973 5f69 6e64 6578  dimen_axis_index
+00003a40: 5d0a 2020 2020 2020 2020 2020 2020 7365  ].            se
+00003a50: 6c66 2e5f 7472 6970 6c6f 7428 0a20 2020  lf._triplot(.   
+00003a60: 2020 2020 2020 2020 2020 2020 2072 6564               red
+00003a70: 7563 6564 5f64 6174 613d 7468 7265 655f  uced_data=three_
+00003a80: 6469 6d65 6e5f 7265 6475 6365 645f 6461  dimen_reduced_da
+00003a90: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
+00003aa0: 2020 2020 7063 5f64 6174 613d 7468 7265      pc_data=thre
+00003ab0: 655f 6469 6d65 6e5f 7063 5f64 6174 612c  e_dimen_pc_data,
+00003ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003ad0: 2061 6c67 6f72 6974 686d 5f6e 616d 653d   algorithm_name=
+00003ae0: 7365 6c66 2e6e 616d 696e 672c 0a20 2020  self.naming,.   
+00003af0: 2020 2020 2020 2020 2020 2020 206c 6f63               loc
+00003b00: 616c 5f70 6174 683d 4745 4f50 495f 4f55  al_path=GEOPI_OU
+00003b10: 5450 5554 5f41 5254 4946 4143 5453 5f49  TPUT_ARTIFACTS_I
+00003b20: 4d41 4745 5f4d 4f44 454c 5f4f 5554 5055  MAGE_MODEL_OUTPU
+00003b30: 545f 5041 5448 2c0a 2020 2020 2020 2020  T_PATH,.        
+00003b40: 2020 2020 2020 2020 6d6c 666c 6f77 5f70          mlflow_p
+00003b50: 6174 683d 4d4c 464c 4f57 5f41 5254 4946  ath=MLFLOW_ARTIF
+00003b60: 4143 545f 494d 4147 455f 4d4f 4445 4c5f  ACT_IMAGE_MODEL_
+00003b70: 4f55 5450 5554 5f50 4154 482c 0a20 2020  OUTPUT_PATH,.   
+00003b80: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00003b90: 2020 2065 6c69 6620 6b77 6172 6773 5b22     elif kwargs["
+00003ba0: 636f 6d70 6f6e 656e 7473 5f6e 756d 225d  components_num"]
+00003bb0: 203d 3d20 333a 0a20 2020 2020 2020 2020   == 3:.         
+00003bc0: 2020 2023 2063 686f 6f73 6520 7477 6f20     # choose two 
+00003bd0: 6f66 2064 696d 656e 7369 6f6e 7320 746f  of dimensions to
+00003be0: 2064 7261 770a 2020 2020 2020 2020 2020   draw.          
+00003bf0: 2020 7477 6f5f 6469 6d65 6e5f 6178 6973    two_dimen_axis
+00003c00: 5f69 6e64 6578 2c20 7477 6f5f 6469 6d65  _index, two_dime
+00003c10: 6e5f 7063 5f64 6174 6120 3d20 7365 6c66  n_pc_data = self
+00003c20: 2e63 686f 6f73 655f 6469 6d65 6e73 696f  .choose_dimensio
+00003c30: 6e5f 6461 7461 2873 656c 662e 7063 5f64  n_data(self.pc_d
+00003c40: 6174 612c 2032 290a 2020 2020 2020 2020  ata, 2).        
+00003c50: 2020 2020 7477 6f5f 6469 6d65 6e5f 7265      two_dimen_re
+00003c60: 6475 6365 645f 6461 7461 203d 2073 656c  duced_data = sel
+00003c70: 662e 585f 7265 6475 6365 642e 696c 6f63  f.X_reduced.iloc
+00003c80: 5b3a 2c20 7477 6f5f 6469 6d65 6e5f 6178  [:, two_dimen_ax
+00003c90: 6973 5f69 6e64 6578 5d0a 2020 2020 2020  is_index].      
+00003ca0: 2020 2020 2020 7365 6c66 2e5f 6269 706c        self._bipl
+00003cb0: 6f74 280a 2020 2020 2020 2020 2020 2020  ot(.            
+00003cc0: 2020 2020 7265 6475 6365 645f 6461 7461      reduced_data
+00003cd0: 3d74 776f 5f64 696d 656e 5f72 6564 7563  =two_dimen_reduc
+00003ce0: 6564 5f64 6174 612c 0a20 2020 2020 2020  ed_data,.       
+00003cf0: 2020 2020 2020 2020 2070 635f 6461 7461           pc_data
+00003d00: 3d74 776f 5f64 696d 656e 5f70 635f 6461  =two_dimen_pc_da
+00003d10: 7461 2c0a 2020 2020 2020 2020 2020 2020  ta,.            
+00003d20: 2020 2020 616c 676f 7269 7468 6d5f 6e61      algorithm_na
+00003d30: 6d65 3d73 656c 662e 6e61 6d69 6e67 2c0a  me=self.naming,.
+00003d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d50: 6c6f 6361 6c5f 7061 7468 3d47 454f 5049  local_path=GEOPI
+00003d60: 5f4f 5554 5055 545f 4152 5449 4641 4354  _OUTPUT_ARTIFACT
+00003d70: 535f 494d 4147 455f 4d4f 4445 4c5f 4f55  S_IMAGE_MODEL_OU
+00003d80: 5450 5554 5f50 4154 482c 0a20 2020 2020  TPUT_PATH,.     
+00003d90: 2020 2020 2020 2020 2020 206d 6c66 6c6f             mlflo
+00003da0: 775f 7061 7468 3d4d 4c46 4c4f 575f 4152  w_path=MLFLOW_AR
+00003db0: 5449 4641 4354 5f49 4d41 4745 5f4d 4f44  TIFACT_IMAGE_MOD
+00003dc0: 454c 5f4f 5554 5055 545f 5041 5448 2c0a  EL_OUTPUT_PATH,.
+00003dd0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00003de0: 2020 2020 2020 2020 2020 2320 6e6f 206e            # no n
+00003df0: 6565 6420 746f 2063 686f 6f73 650a 2020  eed to choose.  
+00003e00: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+00003e10: 7472 6970 6c6f 7428 0a20 2020 2020 2020  triplot(.       
+00003e20: 2020 2020 2020 2020 2072 6564 7563 6564           reduced
+00003e30: 5f64 6174 613d 7365 6c66 2e58 5f72 6564  _data=self.X_red
+00003e40: 7563 6564 2c0a 2020 2020 2020 2020 2020  uced,.          
+00003e50: 2020 2020 2020 7063 5f64 6174 613d 7365        pc_data=se
+00003e60: 6c66 2e70 635f 6461 7461 2c0a 2020 2020  lf.pc_data,.    
+00003e70: 2020 2020 2020 2020 2020 2020 616c 676f              algo
+00003e80: 7269 7468 6d5f 6e61 6d65 3d73 656c 662e  rithm_name=self.
+00003e90: 6e61 6d69 6e67 2c0a 2020 2020 2020 2020  naming,.        
+00003ea0: 2020 2020 2020 2020 6c6f 6361 6c5f 7061          local_pa
+00003eb0: 7468 3d47 454f 5049 5f4f 5554 5055 545f  th=GEOPI_OUTPUT_
+00003ec0: 4152 5449 4641 4354 535f 494d 4147 455f  ARTIFACTS_IMAGE_
+00003ed0: 4d4f 4445 4c5f 4f55 5450 5554 5f50 4154  MODEL_OUTPUT_PAT
+00003ee0: 482c 0a20 2020 2020 2020 2020 2020 2020  H,.             
+00003ef0: 2020 206d 6c66 6c6f 775f 7061 7468 3d4d     mlflow_path=M
+00003f00: 4c46 4c4f 575f 4152 5449 4641 4354 5f49  LFLOW_ARTIFACT_I
+00003f10: 4d41 4745 5f4d 4f44 454c 5f4f 5554 5055  MAGE_MODEL_OUTPU
+00003f20: 545f 5041 5448 2c0a 2020 2020 2020 2020  T_PATH,.        
+00003f30: 2020 2020 290a 2020 2020 2020 2020 656c      ).        el
+00003f40: 6966 206b 7761 7267 735b 2263 6f6d 706f  if kwargs["compo
+00003f50: 6e65 6e74 735f 6e75 6d22 5d20 3d3d 2032  nents_num"] == 2
+00003f60: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00003f70: 6c66 2e5f 6269 706c 6f74 280a 2020 2020  lf._biplot(.    
+00003f80: 2020 2020 2020 2020 2020 2020 7265 6475              redu
+00003f90: 6365 645f 6461 7461 3d73 656c 662e 585f  ced_data=self.X_
+00003fa0: 7265 6475 6365 642c 0a20 2020 2020 2020  reduced,.       
+00003fb0: 2020 2020 2020 2020 2070 635f 6461 7461           pc_data
+00003fc0: 3d73 656c 662e 7063 5f64 6174 612c 0a20  =self.pc_data,. 
+00003fd0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00003fe0: 6c67 6f72 6974 686d 5f6e 616d 653d 7365  lgorithm_name=se
+00003ff0: 6c66 2e6e 616d 696e 672c 0a20 2020 2020  lf.naming,.     
+00004000: 2020 2020 2020 2020 2020 206c 6f63 616c             local
+00004010: 5f70 6174 683d 4745 4f50 495f 4f55 5450  _path=GEOPI_OUTP
+00004020: 5554 5f41 5254 4946 4143 5453 5f49 4d41  UT_ARTIFACTS_IMA
+00004030: 4745 5f4d 4f44 454c 5f4f 5554 5055 545f  GE_MODEL_OUTPUT_
+00004040: 5041 5448 2c0a 2020 2020 2020 2020 2020  PATH,.          
+00004050: 2020 2020 2020 6d6c 666c 6f77 5f70 6174        mlflow_pat
+00004060: 683d 4d4c 464c 4f57 5f41 5254 4946 4143  h=MLFLOW_ARTIFAC
+00004070: 545f 494d 4147 455f 4d4f 4445 4c5f 4f55  T_IMAGE_MODEL_OU
+00004080: 5450 5554 5f50 4154 482c 0a20 2020 2020  TPUT_PATH,.     
+00004090: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000040a0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000040b0: 2020 2070 6173 730a 0a0a 636c 6173 7320     pass...class 
+000040c0: 5453 4e45 4465 636f 6d70 6f73 6974 696f  TSNEDecompositio
+000040d0: 6e28 4465 636f 6d70 6f73 6974 696f 6e57  n(DecompositionW
+000040e0: 6f72 6b66 6c6f 7742 6173 6529 3a0a 2020  orkflowBase):.  
+000040f0: 2020 2222 2254 6865 2061 7574 6f6d 6174    """The automat
+00004100: 696f 6e20 776f 726b 666c 6f77 206f 6620  ion workflow of 
+00004110: 7573 696e 6720 542d 534e 4520 616c 676f  using T-SNE algo
+00004120: 7269 7468 6d20 746f 206d 616b 6520 696e  rithm to make in
+00004130: 7369 6768 7466 756c 2070 726f 6475 6374  sightful product
+00004140: 732e 2222 220a 0a20 2020 206e 616d 6520  s."""..    name 
+00004150: 3d20 2254 2d53 4e45 220a 2020 2020 7370  = "T-SNE".    sp
+00004160: 6563 6961 6c5f 6675 6e63 7469 6f6e 203d  ecial_function =
+00004170: 205b 5d0a 0a20 2020 2064 6566 205f 5f69   []..    def __i
+00004180: 6e69 745f 5f28 0a20 2020 2020 2020 2073  nit__(.        s
+00004190: 656c 662c 0a20 2020 2020 2020 206e 5f63  elf,.        n_c
+000041a0: 6f6d 706f 6e65 6e74 733a 2069 6e74 203d  omponents: int =
+000041b0: 2032 2c0a 2020 2020 2020 2020 2a2c 0a20   2,.        *,. 
+000041c0: 2020 2020 2020 2070 6572 706c 6578 6974         perplexit
+000041d0: 793a 2066 6c6f 6174 203d 2033 302e 302c  y: float = 30.0,
+000041e0: 0a20 2020 2020 2020 2065 6172 6c79 5f65  .        early_e
+000041f0: 7861 6767 6572 6174 696f 6e3a 2066 6c6f  xaggeration: flo
+00004200: 6174 203d 2031 322e 302c 0a20 2020 2020  at = 12.0,.     
+00004210: 2020 206c 6561 726e 696e 675f 7261 7465     learning_rate
+00004220: 3a20 556e 696f 6e5b 666c 6f61 742c 2073  : Union[float, s
+00004230: 7472 5d20 3d20 2261 7574 6f22 2c0a 2020  tr] = "auto",.  
+00004240: 2020 2020 2020 6e5f 6974 6572 3a20 696e        n_iter: in
+00004250: 7420 3d20 3130 3030 2c0a 2020 2020 2020  t = 1000,.      
+00004260: 2020 6e5f 6974 6572 5f77 6974 686f 7574    n_iter_without
+00004270: 5f70 726f 6772 6573 733a 2069 6e74 203d  _progress: int =
+00004280: 2033 3030 2c0a 2020 2020 2020 2020 6d69   300,.        mi
+00004290: 6e5f 6772 6164 5f6e 6f72 6d3a 2066 6c6f  n_grad_norm: flo
+000042a0: 6174 203d 2031 652d 372c 0a20 2020 2020  at = 1e-7,.     
+000042b0: 2020 206d 6574 7269 633a 2073 7472 203d     metric: str =
+000042c0: 2022 6575 636c 6964 6561 6e22 2c0a 2020   "euclidean",.  
+000042d0: 2020 2020 2020 6d65 7472 6963 5f70 6172        metric_par
+000042e0: 616d 733a 204f 7074 696f 6e61 6c5b 4469  ams: Optional[Di
+000042f0: 6374 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ct] = None,.    
+00004300: 2020 2020 696e 6974 3a20 7374 7220 3d20      init: str = 
+00004310: 2270 6361 222c 0a20 2020 2020 2020 2076  "pca",.        v
+00004320: 6572 626f 7365 3a20 696e 7420 3d20 302c  erbose: int = 0,
+00004330: 0a20 2020 2020 2020 2072 616e 646f 6d5f  .        random_
+00004340: 7374 6174 653a 204f 7074 696f 6e61 6c5b  state: Optional[
+00004350: 696e 745d 203d 204e 6f6e 652c 0a20 2020  int] = None,.   
+00004360: 2020 2020 206d 6574 686f 643a 2073 7472       method: str
+00004370: 203d 2022 6578 6163 7422 2c0a 2020 2020   = "exact",.    
+00004380: 2020 2020 616e 676c 653a 2066 6c6f 6174      angle: float
+00004390: 203d 2030 2e35 2c0a 2020 2020 2020 2020   = 0.5,.        
+000043a0: 6e5f 6a6f 6273 3a20 696e 7420 3d20 4e6f  n_jobs: int = No
+000043b0: 6e65 2c0a 2020 2020 2020 2020 7371 7561  ne,.        squa
+000043c0: 7265 5f64 6973 7461 6e63 6573 3a20 556e  re_distances: Un
+000043d0: 696f 6e5b 626f 6f6c 2c20 7374 725d 203d  ion[bool, str] =
+000043e0: 2022 6465 7072 6563 6174 6564 222c 0a20   "deprecated",. 
+000043f0: 2020 2029 202d 3e20 4e6f 6e65 3a0a 2020     ) -> None:.  
+00004400: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00004410: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00004420: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+00004430: 2020 2020 2020 2020 6e5f 636f 6d70 6f6e          n_compon
+00004440: 656e 7473 203a 2069 6e74 2c20 6465 6661  ents : int, defa
+00004450: 756c 743d 320a 2020 2020 2020 2020 2020  ult=2.          
+00004460: 2020 4469 6d65 6e73 696f 6e20 6f66 2074    Dimension of t
+00004470: 6865 2065 6d62 6564 6465 6420 7370 6163  he embedded spac
+00004480: 652e 0a0a 2020 2020 2020 2020 7065 7270  e...        perp
+00004490: 6c65 7869 7479 203a 2066 6c6f 6174 2c20  lexity : float, 
+000044a0: 6465 6661 756c 743d 3330 2e30 0a20 2020  default=30.0.   
+000044b0: 2020 2020 2020 2020 2054 6865 2070 6572           The per
+000044c0: 706c 6578 6974 7920 6973 2072 656c 6174  plexity is relat
+000044d0: 6564 2074 6f20 7468 6520 6e75 6d62 6572  ed to the number
+000044e0: 206f 6620 6e65 6172 6573 7420 6e65 6967   of nearest neig
+000044f0: 6862 6f72 7320 7468 6174 0a20 2020 2020  hbors that.     
+00004500: 2020 2020 2020 2069 7320 7573 6564 2069         is used i
+00004510: 6e20 6f74 6865 7220 6d61 6e69 666f 6c64  n other manifold
+00004520: 206c 6561 726e 696e 6720 616c 676f 7269   learning algori
+00004530: 7468 6d73 2e20 4c61 7267 6572 2064 6174  thms. Larger dat
+00004540: 6173 6574 730a 2020 2020 2020 2020 2020  asets.          
+00004550: 2020 7573 7561 6c6c 7920 7265 7175 6972    usually requir
+00004560: 6520 6120 6c61 7267 6572 2070 6572 706c  e a larger perpl
+00004570: 6578 6974 792e 2043 6f6e 7369 6465 7220  exity. Consider 
+00004580: 7365 6c65 6374 696e 6720 6120 7661 6c75  selecting a valu
+00004590: 650a 2020 2020 2020 2020 2020 2020 6265  e.            be
+000045a0: 7477 6565 6e20 3520 616e 6420 3530 2e20  tween 5 and 50. 
+000045b0: 4469 6666 6572 656e 7420 7661 6c75 6573  Different values
+000045c0: 2063 616e 2072 6573 756c 7420 696e 2073   can result in s
+000045d0: 6967 6e69 6669 6361 6e74 6c79 0a20 2020  ignificantly.   
+000045e0: 2020 2020 2020 2020 2064 6966 6665 7265           differe
+000045f0: 6e74 2072 6573 756c 7473 2e20 5468 6520  nt results. The 
+00004600: 7065 7270 6c65 7869 7479 206d 7573 7420  perplexity must 
+00004610: 6265 206c 6573 7320 7468 616e 2074 6865  be less than the
+00004620: 206e 756d 6265 720a 2020 2020 2020 2020   number.        
+00004630: 2020 2020 6f66 2073 616d 706c 6573 2e0a      of samples..
+00004640: 0a20 2020 2020 2020 2065 6172 6c79 5f65  .        early_e
+00004650: 7861 6767 6572 6174 696f 6e20 3a20 666c  xaggeration : fl
+00004660: 6f61 742c 2064 6566 6175 6c74 3d31 322e  oat, default=12.
+00004670: 300a 2020 2020 2020 2020 2020 2020 436f  0.            Co
+00004680: 6e74 726f 6c73 2068 6f77 2074 6967 6874  ntrols how tight
+00004690: 206e 6174 7572 616c 2063 6c75 7374 6572   natural cluster
+000046a0: 7320 696e 2074 6865 206f 7269 6769 6e61  s in the origina
+000046b0: 6c20 7370 6163 6520 6172 6520 696e 0a20  l space are in. 
+000046c0: 2020 2020 2020 2020 2020 2074 6865 2065             the e
+000046d0: 6d62 6564 6465 6420 7370 6163 6520 616e  mbedded space an
+000046e0: 6420 686f 7720 6d75 6368 2073 7061 6365  d how much space
+000046f0: 2077 696c 6c20 6265 2062 6574 7765 656e   will be between
+00004700: 2074 6865 6d2e 2046 6f72 0a20 2020 2020   them. For.     
+00004710: 2020 2020 2020 206c 6172 6765 7220 7661         larger va
+00004720: 6c75 6573 2c20 7468 6520 7370 6163 6520  lues, the space 
+00004730: 6265 7477 6565 6e20 6e61 7475 7261 6c20  between natural 
+00004740: 636c 7573 7465 7273 2077 696c 6c20 6265  clusters will be
+00004750: 206c 6172 6765 720a 2020 2020 2020 2020   larger.        
+00004760: 2020 2020 696e 2074 6865 2065 6d62 6564      in the embed
+00004770: 6465 6420 7370 6163 652e 2041 6761 696e  ded space. Again
+00004780: 2c20 7468 6520 6368 6f69 6365 206f 6620  , the choice of 
+00004790: 7468 6973 2070 6172 616d 6574 6572 2069  this parameter i
+000047a0: 7320 6e6f 740a 2020 2020 2020 2020 2020  s not.          
+000047b0: 2020 7665 7279 2063 7269 7469 6361 6c2e    very critical.
+000047c0: 2049 6620 7468 6520 636f 7374 2066 756e   If the cost fun
+000047d0: 6374 696f 6e20 696e 6372 6561 7365 7320  ction increases 
+000047e0: 6475 7269 6e67 2069 6e69 7469 616c 0a20  during initial. 
+000047f0: 2020 2020 2020 2020 2020 206f 7074 696d             optim
+00004800: 697a 6174 696f 6e2c 2074 6865 2065 6172  ization, the ear
+00004810: 6c79 2065 7861 6767 6572 6174 696f 6e20  ly exaggeration 
+00004820: 6661 6374 6f72 206f 7220 7468 6520 6c65  factor or the le
+00004830: 6172 6e69 6e67 2072 6174 650a 2020 2020  arning rate.    
+00004840: 2020 2020 2020 2020 6d69 6768 7420 6265          might be
+00004850: 2074 6f6f 2068 6967 682e 0a0a 2020 2020   too high...    
+00004860: 2020 2020 6c65 6172 6e69 6e67 5f72 6174      learning_rat
+00004870: 6520 3a20 666c 6f61 7420 6f72 2022 6175  e : float or "au
+00004880: 746f 222c 2064 6566 6175 6c74 3d22 6175  to", default="au
+00004890: 746f 220a 2020 2020 2020 2020 2020 2020  to".            
+000048a0: 5468 6520 6c65 6172 6e69 6e67 2072 6174  The learning rat
+000048b0: 6520 666f 7220 742d 534e 4520 6973 2075  e for t-SNE is u
+000048c0: 7375 616c 6c79 2069 6e20 7468 6520 7261  sually in the ra
+000048d0: 6e67 6520 5b31 302e 302c 2031 3030 302e  nge [10.0, 1000.
+000048e0: 305d 2e20 4966 0a20 2020 2020 2020 2020  0]. If.         
+000048f0: 2020 2074 6865 206c 6561 726e 696e 6720     the learning 
+00004900: 7261 7465 2069 7320 746f 6f20 6869 6768  rate is too high
+00004910: 2c20 7468 6520 6461 7461 206d 6179 206c  , the data may l
+00004920: 6f6f 6b20 6c69 6b65 2061 2027 6261 6c6c  ook like a 'ball
+00004930: 2720 7769 7468 2061 6e79 0a20 2020 2020  ' with any.     
+00004940: 2020 2020 2020 2070 6f69 6e74 2061 7070         point app
+00004950: 726f 7869 6d61 7465 6c79 2065 7175 6964  roximately equid
+00004960: 6973 7461 6e74 2066 726f 6d20 6974 7320  istant from its 
+00004970: 6e65 6172 6573 7420 6e65 6967 6862 6f75  nearest neighbou
+00004980: 7273 2e20 4966 2074 6865 0a20 2020 2020  rs. If the.     
+00004990: 2020 2020 2020 206c 6561 726e 696e 6720         learning 
+000049a0: 7261 7465 2069 7320 746f 6f20 6c6f 772c  rate is too low,
+000049b0: 206d 6f73 7420 706f 696e 7473 206d 6179   most points may
+000049c0: 206c 6f6f 6b20 636f 6d70 7265 7373 6564   look compressed
+000049d0: 2069 6e20 6120 6465 6e73 650a 2020 2020   in a dense.    
+000049e0: 2020 2020 2020 2020 636c 6f75 6420 7769          cloud wi
+000049f0: 7468 2066 6577 206f 7574 6c69 6572 732e  th few outliers.
+00004a00: 2049 6620 7468 6520 636f 7374 2066 756e   If the cost fun
+00004a10: 6374 696f 6e20 6765 7473 2073 7475 636b  ction gets stuck
+00004a20: 2069 6e20 6120 6261 6420 6c6f 6361 6c0a   in a bad local.
+00004a30: 2020 2020 2020 2020 2020 2020 6d69 6e69              mini
+00004a40: 6d75 6d20 696e 6372 6561 7369 6e67 2074  mum increasing t
+00004a50: 6865 206c 6561 726e 696e 6720 7261 7465  he learning rate
+00004a60: 206d 6179 2068 656c 702e 0a20 2020 2020   may help..     
+00004a70: 2020 2020 2020 204e 6f74 6520 7468 6174         Note that
+00004a80: 206d 616e 7920 6f74 6865 7220 742d 534e   many other t-SN
+00004a90: 4520 696d 706c 656d 656e 7461 7469 6f6e  E implementation
+00004aa0: 7320 2862 6874 736e 652c 2046 4974 2d53  s (bhtsne, FIt-S
+00004ab0: 4e45 2c20 6f70 656e 5453 4e45 2c0a 2020  NE, openTSNE,.  
+00004ac0: 2020 2020 2020 2020 2020 6574 632e 2920            etc.) 
+00004ad0: 7573 6520 6120 6465 6669 6e69 7469 6f6e  use a definition
+00004ae0: 206f 6620 6c65 6172 6e69 6e67 5f72 6174   of learning_rat
+00004af0: 6520 7468 6174 2069 7320 3420 7469 6d65  e that is 4 time
+00004b00: 7320 736d 616c 6c65 7220 7468 616e 0a20  s smaller than. 
+00004b10: 2020 2020 2020 2020 2020 206f 7572 732e             ours.
+00004b20: 2053 6f20 6f75 7220 6c65 6172 6e69 6e67   So our learning
+00004b30: 5f72 6174 653d 3230 3020 636f 7272 6573  _rate=200 corres
+00004b40: 706f 6e64 7320 746f 206c 6561 726e 696e  ponds to learnin
+00004b50: 675f 7261 7465 3d38 3030 2069 6e0a 2020  g_rate=800 in.  
+00004b60: 2020 2020 2020 2020 2020 7468 6f73 6520            those 
+00004b70: 6f74 6865 7220 696d 706c 656d 656e 7461  other implementa
+00004b80: 7469 6f6e 732e 2054 6865 2027 6175 746f  tions. The 'auto
+00004b90: 2720 6f70 7469 6f6e 2073 6574 7320 7468  ' option sets th
+00004ba0: 6520 6c65 6172 6e69 6e67 5f72 6174 650a  e learning_rate.
+00004bb0: 2020 2020 2020 2020 2020 2020 746f 2060              to `
+00004bc0: 6d61 7828 4e20 2f20 6561 726c 795f 6578  max(N / early_ex
+00004bd0: 6167 6765 7261 7469 6f6e 202f 2034 2c20  aggeration / 4, 
+00004be0: 3530 2960 2077 6865 7265 204e 2069 7320  50)` where N is 
+00004bf0: 7468 6520 7361 6d70 6c65 2073 697a 652c  the sample size,
+00004c00: 0a20 2020 2020 2020 2020 2020 2066 6f6c  .            fol
+00004c10: 6c6f 7769 6e67 205b 345d 2061 6e64 205b  lowing [4] and [
+00004c20: 355d 2e0a 0a20 2020 2020 2020 2020 2020  5]...           
+00004c30: 202e 2e20 7665 7273 696f 6e63 6861 6e67   .. versionchang
+00004c40: 6564 3a3a 2031 2e32 0a20 2020 2020 2020  ed:: 1.2.       
+00004c50: 2020 2020 2054 6865 2064 6566 6175 6c74       The default
+00004c60: 2076 616c 7565 2063 6861 6e67 6564 2074   value changed t
+00004c70: 6f20 6022 6175 746f 2260 2e0a 0a20 2020  o `"auto"`...   
+00004c80: 2020 2020 206e 5f69 7465 7220 3a20 696e       n_iter : in
+00004c90: 742c 2064 6566 6175 6c74 3d31 3030 300a  t, default=1000.
+00004ca0: 2020 2020 2020 2020 2020 2020 4d61 7869              Maxi
+00004cb0: 6d75 6d20 6e75 6d62 6572 206f 6620 6974  mum number of it
+00004cc0: 6572 6174 696f 6e73 2066 6f72 2074 6865  erations for the
+00004cd0: 206f 7074 696d 697a 6174 696f 6e2e 2053   optimization. S
+00004ce0: 686f 756c 6420 6265 2061 740a 2020 2020  hould be at.    
+00004cf0: 2020 2020 2020 2020 6c65 6173 7420 3235          least 25
+00004d00: 302e 0a0a 2020 2020 2020 2020 6e5f 6974  0...        n_it
+00004d10: 6572 5f77 6974 686f 7574 5f70 726f 6772  er_without_progr
+00004d20: 6573 7320 3a20 696e 742c 2064 6566 6175  ess : int, defau
+00004d30: 6c74 3d33 3030 0a20 2020 2020 2020 2020  lt=300.         
+00004d40: 2020 204d 6178 696d 756d 206e 756d 6265     Maximum numbe
+00004d50: 7220 6f66 2069 7465 7261 7469 6f6e 7320  r of iterations 
+00004d60: 7769 7468 6f75 7420 7072 6f67 7265 7373  without progress
+00004d70: 2062 6566 6f72 6520 7765 2061 626f 7274   before we abort
+00004d80: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
+00004d90: 206f 7074 696d 697a 6174 696f 6e2c 2075   optimization, u
+00004da0: 7365 6420 6166 7465 7220 3235 3020 696e  sed after 250 in
+00004db0: 6974 6961 6c20 6974 6572 6174 696f 6e73  itial iterations
+00004dc0: 2077 6974 6820 6561 726c 790a 2020 2020   with early.    
+00004dd0: 2020 2020 2020 2020 6578 6167 6765 7261          exaggera
+00004de0: 7469 6f6e 2e20 4e6f 7465 2074 6861 7420  tion. Note that 
+00004df0: 7072 6f67 7265 7373 2069 7320 6f6e 6c79  progress is only
+00004e00: 2063 6865 636b 6564 2065 7665 7279 2035   checked every 5
+00004e10: 3020 6974 6572 6174 696f 6e73 2073 6f0a  0 iterations so.
+00004e20: 2020 2020 2020 2020 2020 2020 7468 6973              this
+00004e30: 2076 616c 7565 2069 7320 726f 756e 6465   value is rounde
+00004e40: 6420 746f 2074 6865 206e 6578 7420 6d75  d to the next mu
+00004e50: 6c74 6970 6c65 206f 6620 3530 2e0a 0a20  ltiple of 50... 
+00004e60: 2020 2020 2020 2020 2020 202e 2e20 7665             .. ve
+00004e70: 7273 696f 6e61 6464 6564 3a3a 2030 2e31  rsionadded:: 0.1
+00004e80: 370a 2020 2020 2020 2020 2020 2020 7061  7.            pa
+00004e90: 7261 6d65 7465 7220 2a6e 5f69 7465 725f  rameter *n_iter_
+00004ea0: 7769 7468 6f75 745f 7072 6f67 7265 7373  without_progress
+00004eb0: 2a20 746f 2063 6f6e 7472 6f6c 2073 746f  * to control sto
+00004ec0: 7070 696e 6720 6372 6974 6572 6961 2e0a  pping criteria..
+00004ed0: 0a20 2020 2020 2020 206d 696e 5f67 7261  .        min_gra
+00004ee0: 645f 6e6f 726d 203a 2066 6c6f 6174 2c20  d_norm : float, 
+00004ef0: 6465 6661 756c 743d 3165 2d37 0a20 2020  default=1e-7.   
+00004f00: 2020 2020 2020 2020 2049 6620 7468 6520           If the 
+00004f10: 6772 6164 6965 6e74 206e 6f72 6d20 6973  gradient norm is
+00004f20: 2062 656c 6f77 2074 6869 7320 7468 7265   below this thre
+00004f30: 7368 6f6c 642c 2074 6865 206f 7074 696d  shold, the optim
+00004f40: 697a 6174 696f 6e20 7769 6c6c 0a20 2020  ization will.   
+00004f50: 2020 2020 2020 2020 2062 6520 7374 6f70           be stop
+00004f60: 7065 642e 0a0a 2020 2020 2020 2020 6d65  ped...        me
+00004f70: 7472 6963 203a 2073 7472 206f 7220 6361  tric : str or ca
+00004f80: 6c6c 6162 6c65 2c20 6465 6661 756c 743d  llable, default=
+00004f90: 2765 7563 6c69 6465 616e 270a 2020 2020  'euclidean'.    
+00004fa0: 2020 2020 2020 2020 5468 6520 6d65 7472          The metr
+00004fb0: 6963 2074 6f20 7573 6520 7768 656e 2063  ic to use when c
+00004fc0: 616c 6375 6c61 7469 6e67 2064 6973 7461  alculating dista
+00004fd0: 6e63 6520 6265 7477 6565 6e20 696e 7374  nce between inst
+00004fe0: 616e 6365 7320 696e 2061 0a20 2020 2020  ances in a.     
+00004ff0: 2020 2020 2020 2066 6561 7475 7265 2061         feature a
+00005000: 7272 6179 2e20 4966 206d 6574 7269 6320  rray. If metric 
+00005010: 6973 2061 2073 7472 696e 672c 2069 7420  is a string, it 
+00005020: 6d75 7374 2062 6520 6f6e 6520 6f66 2074  must be one of t
+00005030: 6865 206f 7074 696f 6e73 0a20 2020 2020  he options.     
+00005040: 2020 2020 2020 2061 6c6c 6f77 6564 2062         allowed b
+00005050: 7920 7363 6970 792e 7370 6174 6961 6c2e  y scipy.spatial.
+00005060: 6469 7374 616e 6365 2e70 6469 7374 2066  distance.pdist f
+00005070: 6f72 2069 7473 206d 6574 7269 6320 7061  or its metric pa
+00005080: 7261 6d65 7465 722c 206f 720a 2020 2020  rameter, or.    
+00005090: 2020 2020 2020 2020 6120 6d65 7472 6963          a metric
+000050a0: 206c 6973 7465 6420 696e 2070 6169 7277   listed in pairw
+000050b0: 6973 652e 5041 4952 5749 5345 5f44 4953  ise.PAIRWISE_DIS
+000050c0: 5441 4e43 455f 4655 4e43 5449 4f4e 532e  TANCE_FUNCTIONS.
+000050d0: 0a20 2020 2020 2020 2020 2020 2049 6620  .            If 
+000050e0: 6d65 7472 6963 2069 7320 2270 7265 636f  metric is "preco
+000050f0: 6d70 7574 6564 222c 2058 2069 7320 6173  mputed", X is as
+00005100: 7375 6d65 6420 746f 2062 6520 6120 6469  sumed to be a di
+00005110: 7374 616e 6365 206d 6174 7269 782e 0a20  stance matrix.. 
+00005120: 2020 2020 2020 2020 2020 2041 6c74 6572             Alter
+00005130: 6e61 7469 7665 6c79 2c20 6966 206d 6574  natively, if met
+00005140: 7269 6320 6973 2061 2063 616c 6c61 626c  ric is a callabl
+00005150: 6520 6675 6e63 7469 6f6e 2c20 6974 2069  e function, it i
+00005160: 7320 6361 6c6c 6564 206f 6e20 6561 6368  s called on each
+00005170: 0a20 2020 2020 2020 2020 2020 2070 6169  .            pai
+00005180: 7220 6f66 2069 6e73 7461 6e63 6573 2028  r of instances (
+00005190: 726f 7773 2920 616e 6420 7468 6520 7265  rows) and the re
+000051a0: 7375 6c74 696e 6720 7661 6c75 6520 7265  sulting value re
+000051b0: 636f 7264 6564 2e20 5468 6520 6361 6c6c  corded. The call
+000051c0: 6162 6c65 0a20 2020 2020 2020 2020 2020  able.           
+000051d0: 2073 686f 756c 6420 7461 6b65 2074 776f   should take two
+000051e0: 2061 7272 6179 7320 6672 6f6d 2058 2061   arrays from X a
+000051f0: 7320 696e 7075 7420 616e 6420 7265 7475  s input and retu
+00005200: 726e 2061 2076 616c 7565 2069 6e64 6963  rn a value indic
+00005210: 6174 696e 670a 2020 2020 2020 2020 2020  ating.          
+00005220: 2020 7468 6520 6469 7374 616e 6365 2062    the distance b
+00005230: 6574 7765 656e 2074 6865 6d2e 2054 6865  etween them. The
+00005240: 2064 6566 6175 6c74 2069 7320 2265 7563   default is "euc
+00005250: 6c69 6465 616e 2220 7768 6963 6820 6973  lidean" which is
+00005260: 0a20 2020 2020 2020 2020 2020 2069 6e74  .            int
+00005270: 6572 7072 6574 6564 2061 7320 7371 7561  erpreted as squa
+00005280: 7265 6420 6575 636c 6964 6561 6e20 6469  red euclidean di
+00005290: 7374 616e 6365 2e0a 0a20 2020 2020 2020  stance...       
+000052a0: 206d 6574 7269 635f 7061 7261 6d73 203a   metric_params :
+000052b0: 2064 6963 742c 2064 6566 6175 6c74 3d4e   dict, default=N
+000052c0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+000052d0: 4164 6469 7469 6f6e 616c 206b 6579 776f  Additional keywo
+000052e0: 7264 2061 7267 756d 656e 7473 2066 6f72  rd arguments for
+000052f0: 2074 6865 206d 6574 7269 6320 6675 6e63   the metric func
+00005300: 7469 6f6e 2e0a 0a20 2020 2020 2020 2020  tion...         
+00005310: 2020 202e 2e20 7665 7273 696f 6e61 6464     .. versionadd
+00005320: 6564 3a3a 2031 2e31 0a0a 2020 2020 2020  ed:: 1.1..      
+00005330: 2020 696e 6974 203a 207b 2272 616e 646f    init : {"rando
+00005340: 6d22 2c20 2270 6361 227d 206f 7220 6e64  m", "pca"} or nd
+00005350: 6172 7261 7920 6f66 2073 6861 7065 2028  array of shape (
+00005360: 6e5f 7361 6d70 6c65 732c 206e 5f63 6f6d  n_samples, n_com
+00005370: 706f 6e65 6e74 7329 2c20 5c0a 2020 2020  ponents), \.    
+00005380: 2020 2020 2020 2020 2020 2020 6465 6661              defa
+00005390: 756c 743d 2270 6361 220a 2020 2020 2020  ult="pca".      
+000053a0: 2020 2020 2020 496e 6974 6961 6c69 7a61        Initializa
+000053b0: 7469 6f6e 206f 6620 656d 6265 6464 696e  tion of embeddin
+000053c0: 672e 0a20 2020 2020 2020 2020 2020 2050  g..            P
+000053d0: 4341 2069 6e69 7469 616c 697a 6174 696f  CA initializatio
+000053e0: 6e20 6361 6e6e 6f74 2062 6520 7573 6564  n cannot be used
+000053f0: 2077 6974 6820 7072 6563 6f6d 7075 7465   with precompute
+00005400: 6420 6469 7374 616e 6365 7320 616e 6420  d distances and 
+00005410: 6973 0a20 2020 2020 2020 2020 2020 2075  is.            u
+00005420: 7375 616c 6c79 206d 6f72 6520 676c 6f62  sually more glob
+00005430: 616c 6c79 2073 7461 626c 6520 7468 616e  ally stable than
+00005440: 2072 616e 646f 6d20 696e 6974 6961 6c69   random initiali
+00005450: 7a61 7469 6f6e 2e0a 0a20 2020 2020 2020  zation...       
+00005460: 2020 2020 202e 2e20 7665 7273 696f 6e63       .. versionc
+00005470: 6861 6e67 6564 3a3a 2031 2e32 0a20 2020  hanged:: 1.2.   
+00005480: 2020 2020 2020 2020 2054 6865 2064 6566           The def
+00005490: 6175 6c74 2076 616c 7565 2063 6861 6e67  ault value chang
+000054a0: 6564 2074 6f20 6022 7063 6122 602e 0a0a  ed to `"pca"`...
+000054b0: 2020 2020 2020 2020 7665 7262 6f73 6520          verbose 
+000054c0: 3a20 696e 742c 2064 6566 6175 6c74 3d30  : int, default=0
+000054d0: 0a20 2020 2020 2020 2020 2020 2056 6572  .            Ver
+000054e0: 626f 7369 7479 206c 6576 656c 2e0a 0a20  bosity level... 
+000054f0: 2020 2020 2020 2072 616e 646f 6d5f 7374         random_st
+00005500: 6174 6520 3a20 696e 742c 2052 616e 646f  ate : int, Rando
+00005510: 6d53 7461 7465 2069 6e73 7461 6e63 6520  mState instance 
+00005520: 6f72 204e 6f6e 652c 2064 6566 6175 6c74  or None, default
+00005530: 3d4e 6f6e 650a 2020 2020 2020 2020 2020  =None.          
+00005540: 2020 4465 7465 726d 696e 6573 2074 6865    Determines the
+00005550: 2072 616e 646f 6d20 6e75 6d62 6572 2067   random number g
+00005560: 656e 6572 6174 6f72 2e20 5061 7373 2061  enerator. Pass a
+00005570: 6e20 696e 7420 666f 7220 7265 7072 6f64  n int for reprod
+00005580: 7563 6962 6c65 0a20 2020 2020 2020 2020  ucible.         
+00005590: 2020 2072 6573 756c 7473 2061 6372 6f73     results acros
+000055a0: 7320 6d75 6c74 6970 6c65 2066 756e 6374  s multiple funct
+000055b0: 696f 6e20 6361 6c6c 732e 204e 6f74 6520  ion calls. Note 
+000055c0: 7468 6174 2064 6966 6665 7265 6e74 0a20  that different. 
+000055d0: 2020 2020 2020 2020 2020 2069 6e69 7469             initi
+000055e0: 616c 697a 6174 696f 6e73 206d 6967 6874  alizations might
+000055f0: 2072 6573 756c 7420 696e 2064 6966 6665   result in diffe
+00005600: 7265 6e74 206c 6f63 616c 206d 696e 696d  rent local minim
+00005610: 6120 6f66 2074 6865 2063 6f73 740a 2020  a of the cost.  
+00005620: 2020 2020 2020 2020 2020 6675 6e63 7469            functi
+00005630: 6f6e 2e20 5365 6520 3a74 6572 6d3a 6047  on. See :term:`G
+00005640: 6c6f 7373 6172 7920 3c72 616e 646f 6d5f  lossary <random_
+00005650: 7374 6174 653e 602e 0a0a 2020 2020 2020  state>`...      
+00005660: 2020 6d65 7468 6f64 203a 207b 2762 6172    method : {'bar
+00005670: 6e65 735f 6875 7427 2c20 2765 7861 6374  nes_hut', 'exact
+00005680: 277d 2c20 6465 6661 756c 743d 2762 6172  '}, default='bar
+00005690: 6e65 735f 6875 7427 0a20 2020 2020 2020  nes_hut'.       
+000056a0: 2020 2020 2042 7920 6465 6661 756c 7420       By default 
+000056b0: 7468 6520 6772 6164 6965 6e74 2063 616c  the gradient cal
+000056c0: 6375 6c61 7469 6f6e 2061 6c67 6f72 6974  culation algorit
+000056d0: 686d 2075 7365 7320 4261 726e 6573 2d48  hm uses Barnes-H
+000056e0: 7574 0a20 2020 2020 2020 2020 2020 2061  ut.            a
+000056f0: 7070 726f 7869 6d61 7469 6f6e 2072 756e  pproximation run
+00005700: 6e69 6e67 2069 6e20 4f28 4e6c 6f67 4e29  ning in O(NlogN)
+00005710: 2074 696d 652e 206d 6574 686f 643d 2765   time. method='e
+00005720: 7861 6374 270a 2020 2020 2020 2020 2020  xact'.          
+00005730: 2020 7769 6c6c 2072 756e 206f 6e20 7468    will run on th
+00005740: 6520 736c 6f77 6572 2c20 6275 7420 6578  e slower, but ex
+00005750: 6163 742c 2061 6c67 6f72 6974 686d 2069  act, algorithm i
+00005760: 6e20 4f28 4e5e 3229 2074 696d 652e 2054  n O(N^2) time. T
+00005770: 6865 0a20 2020 2020 2020 2020 2020 2065  he.            e
+00005780: 7861 6374 2061 6c67 6f72 6974 686d 2073  xact algorithm s
+00005790: 686f 756c 6420 6265 2075 7365 6420 7768  hould be used wh
+000057a0: 656e 206e 6561 7265 7374 2d6e 6569 6768  en nearest-neigh
+000057b0: 626f 7220 6572 726f 7273 206e 6565 640a  bor errors need.
+000057c0: 2020 2020 2020 2020 2020 2020 746f 2062              to b
+000057d0: 6520 6265 7474 6572 2074 6861 6e20 3325  e better than 3%
+000057e0: 2e20 486f 7765 7665 722c 2074 6865 2065  . However, the e
+000057f0: 7861 6374 206d 6574 686f 6420 6361 6e6e  xact method cann
+00005800: 6f74 2073 6361 6c65 2074 6f0a 2020 2020  ot scale to.    
+00005810: 2020 2020 2020 2020 6d69 6c6c 696f 6e73          millions
+00005820: 206f 6620 6578 616d 706c 6573 2e0a 0a20   of examples... 
+00005830: 2020 2020 2020 2020 2020 202e 2e20 7665             .. ve
+00005840: 7273 696f 6e61 6464 6564 3a3a 2030 2e31  rsionadded:: 0.1
+00005850: 370a 2020 2020 2020 2020 2020 2020 4170  7.            Ap
+00005860: 7072 6f78 696d 6174 6520 6f70 7469 6d69  proximate optimi
+00005870: 7a61 7469 6f6e 202a 6d65 7468 6f64 2a20  zation *method* 
+00005880: 7669 6120 7468 6520 4261 726e 6573 2d48  via the Barnes-H
+00005890: 7574 2e0a 0a20 2020 2020 2020 2061 6e67  ut...        ang
+000058a0: 6c65 203a 2066 6c6f 6174 2c20 6465 6661  le : float, defa
+000058b0: 756c 743d 302e 350a 2020 2020 2020 2020  ult=0.5.        
+000058c0: 2020 2020 4f6e 6c79 2075 7365 6420 6966      Only used if
+000058d0: 206d 6574 686f 643d 2762 6172 6e65 735f   method='barnes_
+000058e0: 6875 7427 0a20 2020 2020 2020 2020 2020  hut'.           
+000058f0: 2054 6869 7320 6973 2074 6865 2074 7261   This is the tra
+00005900: 6465 2d6f 6666 2062 6574 7765 656e 2073  de-off between s
+00005910: 7065 6564 2061 6e64 2061 6363 7572 6163  peed and accurac
+00005920: 7920 666f 7220 4261 726e 6573 2d48 7574  y for Barnes-Hut
+00005930: 2054 2d53 4e45 2e0a 2020 2020 2020 2020   T-SNE..        
+00005940: 2020 2020 2761 6e67 6c65 2720 6973 2074      'angle' is t
+00005950: 6865 2061 6e67 756c 6172 2073 697a 6520  he angular size 
+00005960: 2872 6566 6572 7265 6420 746f 2061 7320  (referred to as 
+00005970: 7468 6574 6120 696e 205b 335d 2920 6f66  theta in [3]) of
+00005980: 2061 2064 6973 7461 6e74 0a20 2020 2020   a distant.     
+00005990: 2020 2020 2020 206e 6f64 6520 6173 206d         node as m
+000059a0: 6561 7375 7265 6420 6672 6f6d 2061 2070  easured from a p
+000059b0: 6f69 6e74 2e20 4966 2074 6869 7320 7369  oint. If this si
+000059c0: 7a65 2069 7320 6265 6c6f 7720 2761 6e67  ze is below 'ang
+000059d0: 6c65 2720 7468 656e 2069 7420 6973 0a20  le' then it is. 
+000059e0: 2020 2020 2020 2020 2020 2075 7365 6420             used 
+000059f0: 6173 2061 2073 756d 6d61 7279 206e 6f64  as a summary nod
+00005a00: 6520 6f66 2061 6c6c 2070 6f69 6e74 7320  e of all points 
+00005a10: 636f 6e74 6169 6e65 6420 7769 7468 696e  contained within
+00005a20: 2069 742e 0a20 2020 2020 2020 2020 2020   it..           
+00005a30: 2054 6869 7320 6d65 7468 6f64 2069 7320   This method is 
+00005a40: 6e6f 7420 7665 7279 2073 656e 7369 7469  not very sensiti
+00005a50: 7665 2074 6f20 6368 616e 6765 7320 696e  ve to changes in
+00005a60: 2074 6869 7320 7061 7261 6d65 7465 720a   this parameter.
+00005a70: 2020 2020 2020 2020 2020 2020 696e 2074              in t
+00005a80: 6865 2072 616e 6765 206f 6620 302e 3220  he range of 0.2 
+00005a90: 2d20 302e 382e 2041 6e67 6c65 206c 6573  - 0.8. Angle les
+00005aa0: 7320 7468 616e 2030 2e32 2068 6173 2071  s than 0.2 has q
+00005ab0: 7569 636b 6c79 2069 6e63 7265 6173 696e  uickly increasin
+00005ac0: 670a 2020 2020 2020 2020 2020 2020 636f  g.            co
+00005ad0: 6d70 7574 6174 696f 6e20 7469 6d65 2061  mputation time a
+00005ae0: 6e64 2061 6e67 6c65 2067 7265 6174 6572  nd angle greater
+00005af0: 2030 2e38 2068 6173 2071 7569 636b 6c79   0.8 has quickly
+00005b00: 2069 6e63 7265 6173 696e 6720 6572 726f   increasing erro
+00005b10: 722e 0a0a 2020 2020 2020 2020 6e5f 6a6f  r...        n_jo
+00005b20: 6273 203a 2069 6e74 2c20 6465 6661 756c  bs : int, defaul
+00005b30: 743d 4e6f 6e65 0a20 2020 2020 2020 2020  t=None.         
+00005b40: 2020 2054 6865 206e 756d 6265 7220 6f66     The number of
+00005b50: 2070 6172 616c 6c65 6c20 6a6f 6273 2074   parallel jobs t
+00005b60: 6f20 7275 6e20 666f 7220 6e65 6967 6862  o run for neighb
+00005b70: 6f72 7320 7365 6172 6368 2e20 5468 6973  ors search. This
+00005b80: 2070 6172 616d 6574 6572 0a20 2020 2020   parameter.     
+00005b90: 2020 2020 2020 2068 6173 206e 6f20 696d         has no im
+00005ba0: 7061 6374 2077 6865 6e20 6060 6d65 7472  pact when ``metr
+00005bb0: 6963 3d22 7072 6563 6f6d 7075 7465 6422  ic="precomputed"
+00005bc0: 6060 206f 720a 2020 2020 2020 2020 2020  `` or.          
+00005bd0: 2020 2860 606d 6574 7269 633d 2265 7563    (``metric="euc
+00005be0: 6c69 6465 616e 2260 6020 616e 6420 6060  lidean"`` and ``
+00005bf0: 6d65 7468 6f64 3d22 6578 6163 7422 6060  method="exact"``
+00005c00: 292e 0a20 2020 2020 2020 2020 2020 2060  )..            `
+00005c10: 604e 6f6e 6560 6020 6d65 616e 7320 3120  `None`` means 1 
+00005c20: 756e 6c65 7373 2069 6e20 6120 3a6f 626a  unless in a :obj
+00005c30: 3a60 6a6f 626c 6962 2e70 6172 616c 6c65  :`joblib.paralle
+00005c40: 6c5f 6261 636b 656e 6460 2063 6f6e 7465  l_backend` conte
+00005c50: 7874 2e0a 2020 2020 2020 2020 2020 2020  xt..            
+00005c60: 6060 2d31 6060 206d 6561 6e73 2075 7369  ``-1`` means usi
+00005c70: 6e67 2061 6c6c 2070 726f 6365 7373 6f72  ng all processor
+00005c80: 732e 2053 6565 203a 7465 726d 3a60 476c  s. See :term:`Gl
+00005c90: 6f73 7361 7279 203c 6e5f 6a6f 6273 3e60  ossary <n_jobs>`
+00005ca0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00005cb0: 206d 6f72 6520 6465 7461 696c 732e 0a0a   more details...
+00005cc0: 2020 2020 2020 2020 2020 2020 2e2e 2076              .. v
+00005cd0: 6572 7369 6f6e 6164 6465 643a 3a20 302e  ersionadded:: 0.
+00005ce0: 3232 0a0a 2020 2020 2020 2020 7371 7561  22..        squa
+00005cf0: 7265 5f64 6973 7461 6e63 6573 203a 2054  re_distances : T
+00005d00: 7275 652c 2064 6566 6175 6c74 3d27 6465  rue, default='de
+00005d10: 7072 6563 6174 6564 270a 2020 2020 2020  precated'.      
+00005d20: 2020 2020 2020 5468 6973 2070 6172 616d        This param
+00005d30: 6574 6572 2068 6173 206e 6f20 6566 6665  eter has no effe
+00005d40: 6374 2073 696e 6365 2064 6973 7461 6e63  ct since distanc
+00005d50: 6520 7661 6c75 6573 2061 7265 2061 6c77  e values are alw
+00005d60: 6179 7320 7371 7561 7265 640a 2020 2020  ays squared.    
+00005d70: 2020 2020 2020 2020 7369 6e63 6520 312e          since 1.
+00005d80: 312e 0a0a 2020 2020 2020 2020 2020 2020  1...            
+00005d90: 2e2e 2064 6570 7265 6361 7465 643a 3a20  .. deprecated:: 
+00005da0: 312e 310a 2020 2020 2020 2020 2020 2020  1.1.            
+00005db0: 2020 2020 6073 7175 6172 655f 6469 7374      `square_dist
+00005dc0: 616e 6365 7360 2068 6173 206e 6f20 6566  ances` has no ef
+00005dd0: 6665 6374 2066 726f 6d20 312e 3120 616e  fect from 1.1 an
+00005de0: 6420 7769 6c6c 2062 6520 7265 6d6f 7665  d will be remove
+00005df0: 6420 696e 0a20 2020 2020 2020 2020 2020  d in.           
+00005e00: 2020 2020 2031 2e33 2e0a 0a20 2020 2020       1.3...     
+00005e10: 2020 2052 6566 6572 656e 6365 730a 2020     References.  
+00005e20: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00005e30: 0a20 2020 2020 2020 2053 6369 6b69 742d  .        Scikit-
+00005e40: 6c65 6172 6e20 4150 493a 2073 6b6c 6561  learn API: sklea
+00005e50: 726e 2e6d 616e 6966 6f6c 642e 5453 4e45  rn.manifold.TSNE
+00005e60: 0a20 2020 2020 2020 2068 7474 7073 3a2f  .        https:/
+00005e70: 2f73 6369 6b69 742d 6c65 6172 6e2e 6f72  /scikit-learn.or
+00005e80: 672f 7374 6162 6c65 2f6d 6f64 756c 6573  g/stable/modules
+00005e90: 2f67 656e 6572 6174 6564 2f73 6b6c 6561  /generated/sklea
+00005ea0: 726e 2e6d 616e 6966 6f6c 642e 5453 4e45  rn.manifold.TSNE
+00005eb0: 2e68 746d 6c0a 2020 2020 2020 2020 2222  .html.        ""
+00005ec0: 220a 2020 2020 2020 2020 7375 7065 7228  ".        super(
+00005ed0: 292e 5f5f 696e 6974 5f5f 2829 0a20 2020  ).__init__().   
+00005ee0: 2020 2020 2073 656c 662e 6e5f 636f 6d70       self.n_comp
+00005ef0: 6f6e 656e 7473 203d 206e 5f63 6f6d 706f  onents = n_compo
+00005f00: 6e65 6e74 730a 2020 2020 2020 2020 7365  nents.        se
+00005f10: 6c66 2e70 6572 706c 6578 6974 7920 3d20  lf.perplexity = 
+00005f20: 7065 7270 6c65 7869 7479 0a20 2020 2020  perplexity.     
+00005f30: 2020 2073 656c 662e 6561 726c 795f 6578     self.early_ex
+00005f40: 6167 6765 7261 7469 6f6e 203d 2065 6172  aggeration = ear
+00005f50: 6c79 5f65 7861 6767 6572 6174 696f 6e0a  ly_exaggeration.
+00005f60: 2020 2020 2020 2020 7365 6c66 2e6c 6561          self.lea
+00005f70: 726e 696e 675f 7261 7465 203d 206c 6561  rning_rate = lea
+00005f80: 726e 696e 675f 7261 7465 0a20 2020 2020  rning_rate.     
+00005f90: 2020 2073 656c 662e 6e5f 6974 6572 203d     self.n_iter =
+00005fa0: 206e 5f69 7465 720a 2020 2020 2020 2020   n_iter.        
+00005fb0: 7365 6c66 2e6e 5f69 7465 725f 7769 7468  self.n_iter_with
+00005fc0: 6f75 745f 7072 6f67 7265 7373 203d 206e  out_progress = n
+00005fd0: 5f69 7465 725f 7769 7468 6f75 745f 7072  _iter_without_pr
+00005fe0: 6f67 7265 7373 0a20 2020 2020 2020 2073  ogress.        s
+00005ff0: 656c 662e 6d69 6e5f 6772 6164 5f6e 6f72  elf.min_grad_nor
+00006000: 6d20 3d20 6d69 6e5f 6772 6164 5f6e 6f72  m = min_grad_nor
+00006010: 6d0a 2020 2020 2020 2020 7365 6c66 2e6d  m.        self.m
+00006020: 6574 7269 6320 3d20 6d65 7472 6963 0a20  etric = metric. 
+00006030: 2020 2020 2020 2073 656c 662e 6d65 7472         self.metr
+00006040: 6963 5f70 6172 616d 7320 3d20 6d65 7472  ic_params = metr
+00006050: 6963 5f70 6172 616d 730a 2020 2020 2020  ic_params.      
+00006060: 2020 7365 6c66 2e69 6e69 7420 3d20 696e    self.init = in
+00006070: 6974 0a20 2020 2020 2020 2073 656c 662e  it.        self.
+00006080: 7665 7262 6f73 6520 3d20 7665 7262 6f73  verbose = verbos
+00006090: 650a 2020 2020 2020 2020 7365 6c66 2e6d  e.        self.m
+000060a0: 6574 686f 6420 3d20 6d65 7468 6f64 0a20  ethod = method. 
+000060b0: 2020 2020 2020 2073 656c 662e 616e 676c         self.angl
+000060c0: 6520 3d20 616e 676c 650a 2020 2020 2020  e = angle.      
+000060d0: 2020 7365 6c66 2e6e 5f6a 6f62 7320 3d20    self.n_jobs = 
+000060e0: 6e5f 6a6f 6273 0a20 2020 2020 2020 2073  n_jobs.        s
+000060f0: 656c 662e 7371 7561 7265 5f64 6973 7461  elf.square_dista
+00006100: 6e63 6573 203d 2073 7175 6172 655f 6469  nces = square_di
+00006110: 7374 616e 6365 730a 0a20 2020 2020 2020  stances..       
+00006120: 2069 6620 7261 6e64 6f6d 5f73 7461 7465   if random_state
+00006130: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00006140: 6c66 2e72 616e 646f 6d5f 7374 6174 6520  lf.random_state 
+00006150: 3d20 7261 6e64 6f6d 5f73 7461 7465 0a0a  = random_state..
+00006160: 2020 2020 2020 2020 2320 4966 2027 7261          # If 'ra
+00006170: 6e64 6f6d 5f73 7461 7465 2720 6973 204e  ndom_state' is N
+00006180: 6f6e 652c 2027 7365 6c66 2e72 616e 646f  one, 'self.rando
+00006190: 6d5f 7374 6174 6527 2063 6f6d 6573 2066  m_state' comes f
+000061a0: 726f 6d20 7468 6520 7061 7265 6e74 2063  rom the parent c
+000061b0: 6c61 7373 2027 576f 726b 666c 6f77 4261  lass 'WorkflowBa
+000061c0: 7365 270a 2020 2020 2020 2020 7365 6c66  se'.        self
+000061d0: 2e6d 6f64 656c 203d 2054 534e 4528 0a20  .model = TSNE(. 
+000061e0: 2020 2020 2020 2020 2020 206e 5f63 6f6d             n_com
+000061f0: 706f 6e65 6e74 733d 7365 6c66 2e6e 5f63  ponents=self.n_c
+00006200: 6f6d 706f 6e65 6e74 732c 0a20 2020 2020  omponents,.     
+00006210: 2020 2020 2020 2070 6572 706c 6578 6974         perplexit
+00006220: 793d 7365 6c66 2e70 6572 706c 6578 6974  y=self.perplexit
+00006230: 792c 0a20 2020 2020 2020 2020 2020 2065  y,.            e
+00006240: 6172 6c79 5f65 7861 6767 6572 6174 696f  arly_exaggeratio
+00006250: 6e3d 7365 6c66 2e65 6172 6c79 5f65 7861  n=self.early_exa
+00006260: 6767 6572 6174 696f 6e2c 0a20 2020 2020  ggeration,.     
+00006270: 2020 2020 2020 206c 6561 726e 696e 675f         learning_
+00006280: 7261 7465 3d73 656c 662e 6c65 6172 6e69  rate=self.learni
+00006290: 6e67 5f72 6174 652c 0a20 2020 2020 2020  ng_rate,.       
+000062a0: 2020 2020 206e 5f69 7465 723d 7365 6c66       n_iter=self
+000062b0: 2e6e 5f69 7465 722c 0a20 2020 2020 2020  .n_iter,.       
+000062c0: 2020 2020 206e 5f69 7465 725f 7769 7468       n_iter_with
+000062d0: 6f75 745f 7072 6f67 7265 7373 3d73 656c  out_progress=sel
+000062e0: 662e 6e5f 6974 6572 5f77 6974 686f 7574  f.n_iter_without
+000062f0: 5f70 726f 6772 6573 732c 0a20 2020 2020  _progress,.     
+00006300: 2020 2020 2020 206d 696e 5f67 7261 645f         min_grad_
+00006310: 6e6f 726d 3d73 656c 662e 6d69 6e5f 6772  norm=self.min_gr
+00006320: 6164 5f6e 6f72 6d2c 0a20 2020 2020 2020  ad_norm,.       
+00006330: 2020 2020 206d 6574 7269 633d 7365 6c66       metric=self
+00006340: 2e6d 6574 7269 632c 0a20 2020 2020 2020  .metric,.       
+00006350: 2020 2020 206d 6574 7269 635f 7061 7261       metric_para
+00006360: 6d73 3d73 656c 662e 6d65 7472 6963 5f70  ms=self.metric_p
+00006370: 6172 616d 732c 0a20 2020 2020 2020 2020  arams,.         
+00006380: 2020 2069 6e69 743d 7365 6c66 2e69 6e69     init=self.ini
+00006390: 742c 0a20 2020 2020 2020 2020 2020 2076  t,.            v
+000063a0: 6572 626f 7365 3d73 656c 662e 7665 7262  erbose=self.verb
+000063b0: 6f73 652c 0a20 2020 2020 2020 2020 2020  ose,.           
+000063c0: 2072 616e 646f 6d5f 7374 6174 653d 7365   random_state=se
+000063d0: 6c66 2e72 616e 646f 6d5f 7374 6174 652c  lf.random_state,
+000063e0: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
+000063f0: 686f 643d 7365 6c66 2e6d 6574 686f 642c  hod=self.method,
+00006400: 0a20 2020 2020 2020 2020 2020 2061 6e67  .            ang
+00006410: 6c65 3d73 656c 662e 616e 676c 652c 0a20  le=self.angle,. 
+00006420: 2020 2020 2020 2020 2020 206e 5f6a 6f62             n_job
+00006430: 733d 7365 6c66 2e6e 5f6a 6f62 732c 0a20  s=self.n_jobs,. 
+00006440: 2020 2020 2020 2020 2020 2073 7175 6172             squar
+00006450: 655f 6469 7374 616e 6365 733d 7365 6c66  e_distances=self
+00006460: 2e73 7175 6172 655f 6469 7374 616e 6365  .square_distance
+00006470: 732c 0a20 2020 2020 2020 2029 0a0a 2020  s,.        )..  
+00006480: 2020 2020 2020 7365 6c66 2e6e 616d 696e        self.namin
+00006490: 6720 3d20 5453 4e45 4465 636f 6d70 6f73  g = TSNEDecompos
+000064a0: 6974 696f 6e2e 6e61 6d65 0a0a 2020 2020  ition.name..    
+000064b0: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
+000064c0: 2064 6566 206d 616e 7561 6c5f 6879 7065   def manual_hype
+000064d0: 725f 7061 7261 6d65 7465 7273 2863 6c73  r_parameters(cls
+000064e0: 2920 2d3e 2044 6963 743a 0a20 2020 2020  ) -> Dict:.     
+000064f0: 2020 2022 2222 4d61 6e75 616c 2068 7970     """Manual hyp
+00006500: 6572 2d70 6172 616d 6574 6572 7320 7370  er-parameters sp
+00006510: 6563 6966 6963 6174 696f 6e2e 2222 220a  ecification.""".
+00006520: 2020 2020 2020 2020 7072 696e 7428 6622          print(f"
+00006530: 2d2a 2d2a 2d20 7b63 6c73 2e6e 616d 657d  -*-*- {cls.name}
+00006540: 202d 2048 7970 6572 2d70 6172 616d 6574   - Hyper-paramet
+00006550: 6572 7320 5370 6563 6966 6963 6174 696f  ers Specificatio
+00006560: 6e20 2d2a 2d2a 2d22 290a 2020 2020 2020  n -*-*-").      
+00006570: 2020 6879 7065 725f 7061 7261 6d65 7465    hyper_paramete
+00006580: 7273 203d 2074 736e 655f 6d61 6e75 616c  rs = tsne_manual
+00006590: 5f68 7970 6572 5f70 6172 616d 6574 6572  _hyper_parameter
+000065a0: 7328 290a 2020 2020 2020 2020 636c 6561  s().        clea
+000065b0: 725f 6f75 7470 7574 2829 0a20 2020 2020  r_output().     
+000065c0: 2020 2072 6574 7572 6e20 6879 7065 725f     return hyper_
+000065d0: 7061 7261 6d65 7465 7273 0a0a 2020 2020  parameters..    
+000065e0: 6465 6620 7370 6563 6961 6c5f 636f 6d70  def special_comp
+000065f0: 6f6e 656e 7473 2873 656c 662c 202a 2a6b  onents(self, **k
+00006600: 7761 7267 7329 202d 3e20 4e6f 6e65 3a0a  wargs) -> None:.
+00006610: 2020 2020 2020 2020 2222 2249 6e76 6f6b          """Invok
+00006620: 6520 616c 6c20 7370 6563 6961 6c20 6170  e all special ap
+00006630: 706c 6963 6174 696f 6e20 6675 6e63 7469  plication functi
+00006640: 6f6e 7320 666f 7220 7468 6973 2061 6c67  ons for this alg
+00006650: 6f72 6974 686d 7320 6279 2053 6369 6b69  orithms by Sciki
+00006660: 742d 6c65 6172 6e20 6672 616d 6577 6f72  t-learn framewor
+00006670: 6b2e 2222 220a 2020 2020 2020 2020 7061  k.""".        pa
+00006680: 7373 0a0a 0a63 6c61 7373 204d 4453 4465  ss...class MDSDe
+00006690: 636f 6d70 6f73 6974 696f 6e28 4465 636f  composition(Deco
+000066a0: 6d70 6f73 6974 696f 6e57 6f72 6b66 6c6f  mpositionWorkflo
+000066b0: 7742 6173 6529 3a0a 2020 2020 2222 2254  wBase):.    """T
+000066c0: 6865 2061 7574 6f6d 6174 696f 6e20 776f  he automation wo
+000066d0: 726b 666c 6f77 206f 6620 7573 696e 6720  rkflow of using 
+000066e0: 4d44 5320 616c 676f 7269 7468 6d20 746f  MDS algorithm to
+000066f0: 206d 616b 6520 696e 7369 6768 7466 756c   make insightful
+00006700: 2070 726f 6475 6374 732e 2222 220a 0a20   products.""".. 
+00006710: 2020 206e 616d 6520 3d20 224d 4453 220a     name = "MDS".
+00006720: 2020 2020 7370 6563 6961 6c5f 6675 6e63      special_func
+00006730: 7469 6f6e 203d 205b 5d0a 0a20 2020 2064  tion = []..    d
+00006740: 6566 205f 5f69 6e69 745f 5f28 0a20 2020  ef __init__(.   
+00006750: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00006760: 2020 206e 5f63 6f6d 706f 6e65 6e74 733a     n_components:
+00006770: 2069 6e74 203d 2032 2c0a 2020 2020 2020   int = 2,.      
+00006780: 2020 2a2c 0a20 2020 2020 2020 206d 6574    *,.        met
+00006790: 7269 633a 2062 6f6f 6c20 3d20 5472 7565  ric: bool = True
+000067a0: 2c0a 2020 2020 2020 2020 6e5f 696e 6974  ,.        n_init
+000067b0: 3a20 696e 7420 3d20 342c 0a20 2020 2020  : int = 4,.     
+000067c0: 2020 206d 6178 5f69 7465 723a 2069 6e74     max_iter: int
+000067d0: 203d 2033 3030 2c0a 2020 2020 2020 2020   = 300,.        
+000067e0: 7665 7262 6f73 653a 2069 6e74 203d 2030  verbose: int = 0
+000067f0: 2c0a 2020 2020 2020 2020 6570 733a 2066  ,.        eps: f
+00006800: 6c6f 6174 203d 2031 652d 332c 0a20 2020  loat = 1e-3,.   
+00006810: 2020 2020 206e 5f6a 6f62 733a 204f 7074       n_jobs: Opt
+00006820: 696f 6e61 6c5b 696e 745d 203d 204e 6f6e  ional[int] = Non
+00006830: 652c 0a20 2020 2020 2020 2072 616e 646f  e,.        rando
+00006840: 6d5f 7374 6174 653a 204f 7074 696f 6e61  m_state: Optiona
+00006850: 6c5b 696e 745d 203d 204e 6f6e 652c 0a20  l[int] = None,. 
+00006860: 2020 2020 2020 2064 6973 7369 6d69 6c61         dissimila
+00006870: 7269 7479 3a20 7374 7220 3d20 2265 7563  rity: str = "euc
+00006880: 6c69 6465 616e 222c 0a20 2020 2020 2020  lidean",.       
+00006890: 2023 206e 6f72 6d61 6c69 7a65 645f 7374   # normalized_st
+000068a0: 7265 7373 3d22 7761 726e 222c 0a20 2020  ress="warn",.   
+000068b0: 2029 202d 3e20 4e6f 6e65 3a0a 2020 2020   ) -> None:.    
+000068c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000068d0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+000068e0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+000068f0: 2020 2020 2020 6e5f 636f 6d70 6f6e 656e        n_componen
+00006900: 7473 203a 2069 6e74 2c20 6465 6661 756c  ts : int, defaul
+00006910: 743d 320a 2020 2020 2020 2020 2020 2020  t=2.            
+00006920: 4e75 6d62 6572 206f 6620 6469 6d65 6e73  Number of dimens
+00006930: 696f 6e73 2069 6e20 7768 6963 6820 746f  ions in which to
+00006940: 2069 6d6d 6572 7365 2074 6865 2064 6973   immerse the dis
+00006950: 7369 6d69 6c61 7269 7469 6573 2e0a 0a20  similarities... 
+00006960: 2020 2020 2020 206d 6574 7269 6320 3a20         metric : 
+00006970: 626f 6f6c 2c20 6465 6661 756c 743d 5472  bool, default=Tr
+00006980: 7565 0a20 2020 2020 2020 2020 2020 2049  ue.            I
+00006990: 6620 6060 5472 7565 6060 2c20 7065 7266  f ``True``, perf
+000069a0: 6f72 6d20 6d65 7472 6963 204d 4453 3b20  orm metric MDS; 
+000069b0: 6f74 6865 7277 6973 652c 2070 6572 666f  otherwise, perfo
+000069c0: 726d 206e 6f6e 6d65 7472 6963 204d 4453  rm nonmetric MDS
+000069d0: 2e0a 2020 2020 2020 2020 2020 2020 5768  ..            Wh
+000069e0: 656e 2060 6046 616c 7365 6060 2028 692e  en ``False`` (i.
+000069f0: 652e 206e 6f6e 2d6d 6574 7269 6320 4d44  e. non-metric MD
+00006a00: 5329 2c20 6469 7373 696d 696c 6172 6974  S), dissimilarit
+00006a10: 6965 7320 7769 7468 2030 2061 7265 2063  ies with 0 are c
+00006a20: 6f6e 7369 6465 7265 6420 6173 0a20 2020  onsidered as.   
+00006a30: 2020 2020 2020 2020 206d 6973 7369 6e67           missing
+00006a40: 2076 616c 7565 732e 0a0a 2020 2020 2020   values...      
+00006a50: 2020 6e5f 696e 6974 203a 2069 6e74 2c20    n_init : int, 
+00006a60: 6465 6661 756c 743d 340a 2020 2020 2020  default=4.      
+00006a70: 2020 2020 2020 4e75 6d62 6572 206f 6620        Number of 
+00006a80: 7469 6d65 7320 7468 6520 534d 4143 4f46  times the SMACOF
+00006a90: 2061 6c67 6f72 6974 686d 2077 696c 6c20   algorithm will 
+00006aa0: 6265 2072 756e 2077 6974 6820 6469 6666  be run with diff
+00006ab0: 6572 656e 740a 2020 2020 2020 2020 2020  erent.          
+00006ac0: 2020 696e 6974 6961 6c69 7a61 7469 6f6e    initialization
+00006ad0: 732e 2054 6865 2066 696e 616c 2072 6573  s. The final res
+00006ae0: 756c 7473 2077 696c 6c20 6265 2074 6865  ults will be the
+00006af0: 2062 6573 7420 6f75 7470 7574 206f 6620   best output of 
+00006b00: 7468 6520 7275 6e73 2c0a 2020 2020 2020  the runs,.      
+00006b10: 2020 2020 2020 6465 7465 726d 696e 6564        determined
+00006b20: 2062 7920 7468 6520 7275 6e20 7769 7468   by the run with
+00006b30: 2074 6865 2073 6d61 6c6c 6573 7420 6669   the smallest fi
+00006b40: 6e61 6c20 7374 7265 7373 2e0a 0a20 2020  nal stress...   
+00006b50: 2020 2020 206d 6178 5f69 7465 7220 3a20       max_iter : 
+00006b60: 696e 742c 2064 6566 6175 6c74 3d33 3030  int, default=300
+00006b70: 0a20 2020 2020 2020 2020 2020 204d 6178  .            Max
+00006b80: 696d 756d 206e 756d 6265 7220 6f66 2069  imum number of i
+00006b90: 7465 7261 7469 6f6e 7320 6f66 2074 6865  terations of the
+00006ba0: 2053 4d41 434f 4620 616c 676f 7269 7468   SMACOF algorith
+00006bb0: 6d20 666f 7220 6120 7369 6e67 6c65 2072  m for a single r
+00006bc0: 756e 2e0a 0a20 2020 2020 2020 2076 6572  un...        ver
+00006bd0: 626f 7365 203a 2069 6e74 2c20 6465 6661  bose : int, defa
+00006be0: 756c 743d 300a 2020 2020 2020 2020 2020  ult=0.          
+00006bf0: 2020 4c65 7665 6c20 6f66 2076 6572 626f    Level of verbo
+00006c00: 7369 7479 2e0a 0a20 2020 2020 2020 2065  sity...        e
+00006c10: 7073 203a 2066 6c6f 6174 2c20 6465 6661  ps : float, defa
+00006c20: 756c 743d 3165 2d33 0a20 2020 2020 2020  ult=1e-3.       
+00006c30: 2020 2020 2052 656c 6174 6976 6520 746f       Relative to
+00006c40: 6c65 7261 6e63 6520 7769 7468 2072 6573  lerance with res
+00006c50: 7065 6374 2074 6f20 7374 7265 7373 2061  pect to stress a
+00006c60: 7420 7768 6963 6820 746f 2064 6563 6c61  t which to decla
+00006c70: 7265 0a20 2020 2020 2020 2020 2020 2063  re.            c
+00006c80: 6f6e 7665 7267 656e 6365 2e20 5468 6520  onvergence. The 
+00006c90: 7661 6c75 6520 6f66 2060 6570 7360 2073  value of `eps` s
+00006ca0: 686f 756c 6420 6265 2074 756e 6564 2073  hould be tuned s
+00006cb0: 6570 6172 6174 656c 7920 6465 7065 6e64  eparately depend
+00006cc0: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+00006cd0: 6f6e 2077 6865 7468 6572 206f 7220 6e6f  on whether or no
+00006ce0: 7420 606e 6f72 6d61 6c69 7a65 645f 7374  t `normalized_st
+00006cf0: 7265 7373 6020 6973 2062 6569 6e67 2075  ress` is being u
+00006d00: 7365 642e 0a0a 2020 2020 2020 2020 6e5f  sed...        n_
+00006d10: 6a6f 6273 203a 2069 6e74 2c20 6465 6661  jobs : int, defa
+00006d20: 756c 743d 4e6f 6e65 0a20 2020 2020 2020  ult=None.       
+00006d30: 2020 2020 2054 6865 206e 756d 6265 7220       The number 
+00006d40: 6f66 206a 6f62 7320 746f 2075 7365 2066  of jobs to use f
+00006d50: 6f72 2074 6865 2063 6f6d 7075 7461 7469  or the computati
+00006d60: 6f6e 2e20 4966 206d 756c 7469 706c 650a  on. If multiple.
+00006d70: 2020 2020 2020 2020 2020 2020 696e 6974              init
+00006d80: 6961 6c69 7a61 7469 6f6e 7320 6172 6520  ializations are 
+00006d90: 7573 6564 2028 6060 6e5f 696e 6974 6060  used (``n_init``
+00006da0: 292c 2065 6163 6820 7275 6e20 6f66 2074  ), each run of t
+00006db0: 6865 2061 6c67 6f72 6974 686d 2069 730a  he algorithm is.
+00006dc0: 2020 2020 2020 2020 2020 2020 636f 6d70              comp
+00006dd0: 7574 6564 2069 6e20 7061 7261 6c6c 656c  uted in parallel
+00006de0: 2e0a 0a20 2020 2020 2020 2020 2020 2060  ...            `
+00006df0: 604e 6f6e 6560 6020 6d65 616e 7320 3120  `None`` means 1 
+00006e00: 756e 6c65 7373 2069 6e20 6120 3a6f 626a  unless in a :obj
+00006e10: 3a60 6a6f 626c 6962 2e70 6172 616c 6c65  :`joblib.paralle
+00006e20: 6c5f 6261 636b 656e 6460 2063 6f6e 7465  l_backend` conte
+00006e30: 7874 2e0a 2020 2020 2020 2020 2020 2020  xt..            
+00006e40: 6060 2d31 6060 206d 6561 6e73 2075 7369  ``-1`` means usi
+00006e50: 6e67 2061 6c6c 2070 726f 6365 7373 6f72  ng all processor
+00006e60: 732e 2053 6565 203a 7465 726d 3a60 476c  s. See :term:`Gl
+00006e70: 6f73 7361 7279 203c 6e5f 6a6f 6273 3e60  ossary <n_jobs>`
+00006e80: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00006e90: 206d 6f72 6520 6465 7461 696c 732e 0a0a   more details...
+00006ea0: 2020 2020 2020 2020 7261 6e64 6f6d 5f73          random_s
+00006eb0: 7461 7465 203a 2069 6e74 2c20 5261 6e64  tate : int, Rand
+00006ec0: 6f6d 5374 6174 6520 696e 7374 616e 6365  omState instance
+00006ed0: 206f 7220 4e6f 6e65 2c20 6465 6661 756c   or None, defaul
+00006ee0: 743d 4e6f 6e65 0a20 2020 2020 2020 2020  t=None.         
+00006ef0: 2020 2044 6574 6572 6d69 6e65 7320 7468     Determines th
+00006f00: 6520 7261 6e64 6f6d 206e 756d 6265 7220  e random number 
+00006f10: 6765 6e65 7261 746f 7220 7573 6564 2074  generator used t
+00006f20: 6f20 696e 6974 6961 6c69 7a65 2074 6865  o initialize the
+00006f30: 2063 656e 7465 7273 2e0a 2020 2020 2020   centers..      
+00006f40: 2020 2020 2020 5061 7373 2061 6e20 696e        Pass an in
+00006f50: 7420 666f 7220 7265 7072 6f64 7563 6962  t for reproducib
+00006f60: 6c65 2072 6573 756c 7473 2061 6372 6f73  le results acros
+00006f70: 7320 6d75 6c74 6970 6c65 2066 756e 6374  s multiple funct
+00006f80: 696f 6e20 6361 6c6c 732e 0a20 2020 2020  ion calls..     
+00006f90: 2020 2020 2020 2053 6565 203a 7465 726d         See :term
+00006fa0: 3a60 476c 6f73 7361 7279 203c 7261 6e64  :`Glossary <rand
+00006fb0: 6f6d 5f73 7461 7465 3e60 2e0a 0a20 2020  om_state>`...   
+00006fc0: 2020 2020 2064 6973 7369 6d69 6c61 7269       dissimilari
+00006fd0: 7479 203a 207b 2765 7563 6c69 6465 616e  ty : {'euclidean
+00006fe0: 272c 2027 7072 6563 6f6d 7075 7465 6427  ', 'precomputed'
+00006ff0: 7d2c 2064 6566 6175 6c74 3d27 6575 636c  }, default='eucl
+00007000: 6964 6561 6e27 0a20 2020 2020 2020 2020  idean'.         
+00007010: 2020 2044 6973 7369 6d69 6c61 7269 7479     Dissimilarity
+00007020: 206d 6561 7375 7265 2074 6f20 7573 653a   measure to use:
+00007030: 0a0a 2020 2020 2020 2020 2020 2020 2d20  ..            - 
+00007040: 2765 7563 6c69 6465 616e 273a 0a20 2020  'euclidean':.   
+00007050: 2020 2020 2020 2020 2020 2020 2050 6169               Pai
+00007060: 7277 6973 6520 4575 636c 6964 6561 6e20  rwise Euclidean 
+00007070: 6469 7374 616e 6365 7320 6265 7477 6565  distances betwee
+00007080: 6e20 706f 696e 7473 2069 6e20 7468 6520  n points in the 
+00007090: 6461 7461 7365 742e 0a0a 2020 2020 2020  dataset...      
+000070a0: 2020 2020 2020 2d20 2770 7265 636f 6d70        - 'precomp
+000070b0: 7574 6564 273a 0a20 2020 2020 2020 2020  uted':.         
+000070c0: 2020 2020 2020 2050 7265 2d63 6f6d 7075         Pre-compu
+000070d0: 7465 6420 6469 7373 696d 696c 6172 6974  ted dissimilarit
+000070e0: 6965 7320 6172 6520 7061 7373 6564 2064  ies are passed d
+000070f0: 6972 6563 746c 7920 746f 2060 6066 6974  irectly to ``fit
+00007100: 6060 2061 6e64 0a20 2020 2020 2020 2020  `` and.         
+00007110: 2020 2020 2020 2060 6066 6974 5f74 7261         ``fit_tra
+00007120: 6e73 666f 726d 6060 2e0a 0a20 2020 2020  nsform``...     
+00007130: 2020 206e 6f72 6d61 6c69 7a65 645f 7374     normalized_st
+00007140: 7265 7373 203a 2062 6f6f 6c20 6f72 2022  ress : bool or "
+00007150: 6175 746f 2220 6465 6661 756c 743d 4661  auto" default=Fa
+00007160: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
+00007170: 5768 6574 6865 7220 7573 6520 616e 6420  Whether use and 
+00007180: 7265 7475 726e 206e 6f72 6d65 6420 7374  return normed st
+00007190: 7265 7373 2076 616c 7565 2028 5374 7265  ress value (Stre
+000071a0: 7373 2d31 2920 696e 7374 6561 6420 6f66  ss-1) instead of
+000071b0: 2072 6177 0a20 2020 2020 2020 2020 2020   raw.           
+000071c0: 2073 7472 6573 7320 6361 6c63 756c 6174   stress calculat
+000071d0: 6564 2062 7920 6465 6661 756c 742e 204f  ed by default. O
+000071e0: 6e6c 7920 7375 7070 6f72 7465 6420 696e  nly supported in
+000071f0: 206e 6f6e 2d6d 6574 7269 6320 4d44 532e   non-metric MDS.
+00007200: 0a0a 2020 2020 2020 2020 2020 2020 2e2e  ..            ..
+00007210: 2076 6572 7369 6f6e 6164 6465 643a 3a20   versionadded:: 
+00007220: 312e 320a 0a20 2020 2020 2020 2052 6566  1.2..        Ref
+00007230: 6572 656e 6365 730a 2020 2020 2020 2020  erences.        
+00007240: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00007250: 2020 2053 6369 6b69 742d 6c65 6172 6e20     Scikit-learn 
+00007260: 4150 493a 2073 6b6c 6561 726e 2e6d 616e  API: sklearn.man
+00007270: 6966 6f6c 642e 4d44 530a 2020 2020 2020  ifold.MDS.      
+00007280: 2020 6874 7470 733a 2f2f 7363 696b 6974    https://scikit
+00007290: 2d6c 6561 726e 2e6f 7267 2f73 7461 626c  -learn.org/stabl
+000072a0: 652f 6d6f 6475 6c65 732f 6765 6e65 7261  e/modules/genera
+000072b0: 7465 642f 736b 6c65 6172 6e2e 6d61 6e69  ted/sklearn.mani
+000072c0: 666f 6c64 2e4d 4453 2e68 746d 6c0a 2020  fold.MDS.html.  
+000072d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000072e0: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
+000072f0: 5f5f 2829 0a20 2020 2020 2020 2073 656c  __().        sel
+00007300: 662e 6e5f 636f 6d70 6f6e 656e 7473 203d  f.n_components =
+00007310: 206e 5f63 6f6d 706f 6e65 6e74 730a 2020   n_components.  
+00007320: 2020 2020 2020 7365 6c66 2e6d 6574 7269        self.metri
+00007330: 6320 3d20 6d65 7472 6963 0a20 2020 2020  c = metric.     
+00007340: 2020 2073 656c 662e 6e5f 696e 6974 203d     self.n_init =
+00007350: 206e 5f69 6e69 740a 2020 2020 2020 2020   n_init.        
+00007360: 7365 6c66 2e6d 6178 5f69 7465 7220 3d20  self.max_iter = 
+00007370: 6d61 785f 6974 6572 0a20 2020 2020 2020  max_iter.       
+00007380: 2073 656c 662e 7665 7262 6f73 6520 3d20   self.verbose = 
+00007390: 7665 7262 6f73 650a 2020 2020 2020 2020  verbose.        
+000073a0: 7365 6c66 2e65 7073 203d 2065 7073 0a20  self.eps = eps. 
+000073b0: 2020 2020 2020 2073 656c 662e 6e5f 6a6f         self.n_jo
+000073c0: 6273 203d 206e 5f6a 6f62 730a 2020 2020  bs = n_jobs.    
+000073d0: 2020 2020 7365 6c66 2e64 6973 7369 6d69      self.dissimi
+000073e0: 6c61 7269 7479 203d 2064 6973 7369 6d69  larity = dissimi
+000073f0: 6c61 7269 7479 0a20 2020 2020 2020 2023  larity.        #
+00007400: 2073 656c 662e 6e6f 726d 616c 697a 6564   self.normalized
+00007410: 5f73 7472 6573 7320 3d20 6e6f 726d 616c  _stress = normal
+00007420: 697a 6564 5f73 7472 6573 730a 0a20 2020  ized_stress..   
+00007430: 2020 2020 2069 6620 7261 6e64 6f6d 5f73       if random_s
+00007440: 7461 7465 3a0a 2020 2020 2020 2020 2020  tate:.          
+00007450: 2020 7365 6c66 2e72 616e 646f 6d5f 7374    self.random_st
+00007460: 6174 6520 3d20 7261 6e64 6f6d 5f73 7461  ate = random_sta
+00007470: 7465 0a0a 2020 2020 2020 2020 2320 4966  te..        # If
+00007480: 2027 7261 6e64 6f6d 5f73 7461 7465 2720   'random_state' 
+00007490: 6973 204e 6f6e 652c 2027 7365 6c66 2e72  is None, 'self.r
+000074a0: 616e 646f 6d5f 7374 6174 6527 2063 6f6d  andom_state' com
+000074b0: 6573 2066 726f 6d20 7468 6520 7061 7265  es from the pare
+000074c0: 6e74 2063 6c61 7373 2027 576f 726b 666c  nt class 'Workfl
+000074d0: 6f77 4261 7365 270a 2020 2020 2020 2020  owBase'.        
+000074e0: 7365 6c66 2e6d 6f64 656c 203d 204d 4453  self.model = MDS
+000074f0: 280a 2020 2020 2020 2020 2020 2020 6e5f  (.            n_
+00007500: 636f 6d70 6f6e 656e 7473 3d73 656c 662e  components=self.
+00007510: 6e5f 636f 6d70 6f6e 656e 7473 2c0a 2020  n_components,.  
+00007520: 2020 2020 2020 2020 2020 6d65 7472 6963            metric
+00007530: 3d73 656c 662e 6d65 7472 6963 2c0a 2020  =self.metric,.  
+00007540: 2020 2020 2020 2020 2020 6e5f 696e 6974            n_init
+00007550: 3d73 656c 662e 6e5f 696e 6974 2c0a 2020  =self.n_init,.  
+00007560: 2020 2020 2020 2020 2020 6d61 785f 6974            max_it
+00007570: 6572 3d73 656c 662e 6d61 785f 6974 6572  er=self.max_iter
+00007580: 2c0a 2020 2020 2020 2020 2020 2020 7665  ,.            ve
+00007590: 7262 6f73 653d 7365 6c66 2e76 6572 626f  rbose=self.verbo
+000075a0: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+000075b0: 6570 733d 7365 6c66 2e65 7073 2c0a 2020  eps=self.eps,.  
+000075c0: 2020 2020 2020 2020 2020 6e5f 6a6f 6273            n_jobs
+000075d0: 3d73 656c 662e 6e5f 6a6f 6273 2c0a 2020  =self.n_jobs,.  
+000075e0: 2020 2020 2020 2020 2020 7261 6e64 6f6d            random
+000075f0: 5f73 7461 7465 3d73 656c 662e 7261 6e64  _state=self.rand
+00007600: 6f6d 5f73 7461 7465 2c0a 2020 2020 2020  om_state,.      
+00007610: 2020 2020 2020 6469 7373 696d 696c 6172        dissimilar
+00007620: 6974 793d 7365 6c66 2e64 6973 7369 6d69  ity=self.dissimi
+00007630: 6c61 7269 7479 2c0a 2020 2020 2020 2020  larity,.        
+00007640: 2020 2020 2320 6e6f 726d 616c 697a 6564      # normalized
+00007650: 5f73 7472 6573 733d 7365 6c66 2e6e 6f72  _stress=self.nor
+00007660: 6d61 6c69 7a65 645f 7374 7265 7373 2c0a  malized_stress,.
+00007670: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00007680: 2020 2073 656c 662e 6e61 6d69 6e67 203d     self.naming =
+00007690: 204d 4453 4465 636f 6d70 6f73 6974 696f   MDSDecompositio
+000076a0: 6e2e 6e61 6d65 0a0a 2020 2020 4063 6c61  n.name..    @cla
+000076b0: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
+000076c0: 206d 616e 7561 6c5f 6879 7065 725f 7061   manual_hyper_pa
+000076d0: 7261 6d65 7465 7273 2863 6c73 2920 2d3e  rameters(cls) ->
+000076e0: 2044 6963 743a 0a20 2020 2020 2020 2022   Dict:.        "
+000076f0: 2222 4d61 6e75 616c 2068 7970 6572 2d70  ""Manual hyper-p
+00007700: 6172 616d 6574 6572 7320 7370 6563 6966  arameters specif
+00007710: 6963 6174 696f 6e2e 2222 220a 2020 2020  ication.""".    
+00007720: 2020 2020 7072 696e 7428 6622 2d2a 2d2a      print(f"-*-*
+00007730: 2d20 7b63 6c73 2e6e 616d 657d 202d 2048  - {cls.name} - H
+00007740: 7970 6572 2d70 6172 616d 6574 6572 7320  yper-parameters 
+00007750: 5370 6563 6966 6963 6174 696f 6e20 2d2a  Specification -*
+00007760: 2d2a 2d22 290a 2020 2020 2020 2020 6879  -*-").        hy
+00007770: 7065 725f 7061 7261 6d65 7465 7273 203d  per_parameters =
+00007780: 206d 6473 5f6d 616e 7561 6c5f 6879 7065   mds_manual_hype
+00007790: 725f 7061 7261 6d65 7465 7273 2829 0a20  r_parameters(). 
+000077a0: 2020 2020 2020 2063 6c65 6172 5f6f 7574         clear_out
+000077b0: 7075 7428 290a 2020 2020 2020 2020 7265  put().        re
+000077c0: 7475 726e 2068 7970 6572 5f70 6172 616d  turn hyper_param
+000077d0: 6574 6572 730a 0a20 2020 2064 6566 2073  eters..    def s
+000077e0: 7065 6369 616c 5f63 6f6d 706f 6e65 6e74  pecial_component
+000077f0: 7328 7365 6c66 2c20 2a2a 6b77 6172 6773  s(self, **kwargs
+00007800: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+00007810: 2020 2022 2222 496e 766f 6b65 2061 6c6c     """Invoke all
+00007820: 2073 7065 6369 616c 2061 7070 6c69 6361   special applica
+00007830: 7469 6f6e 2066 756e 6374 696f 6e73 2066  tion functions f
+00007840: 6f72 2074 6869 7320 616c 676f 7269 7468  or this algorith
+00007850: 6d73 2062 7920 5363 696b 6974 2d6c 6561  ms by Scikit-lea
+00007860: 726e 2066 7261 6d65 776f 726b 2e22 2222  rn framework."""
+00007870: 0a20 2020 2020 2020 2070 6173 730a       .        pass.
```

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/regression.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import numpy as np
 import pandas as pd
 import xgboost
 from flaml import AutoML
 from multipledispatch import dispatch
 from rich import print
 from sklearn.ensemble import ExtraTreesRegressor, GradientBoostingRegressor, RandomForestRegressor
-from sklearn.linear_model import BayesianRidge, ElasticNet, Lasso, LinearRegression, SGDRegressor
+from sklearn.linear_model import BayesianRidge, ElasticNet, Lasso, LinearRegression, Ridge, SGDRegressor
 from sklearn.neighbors import KNeighborsRegressor
 from sklearn.neural_network import MLPRegressor
 from sklearn.preprocessing import PolynomialFeatures
 from sklearn.svm import SVR
 from sklearn.tree import DecisionTreeRegressor
 
 from ..constants import MLFLOW_ARTIFACT_IMAGE_MODEL_OUTPUT_PATH, RAY_FLAML
@@ -29,14 +29,15 @@
 from .func.algo_regression._gradient_boosting import gradient_boosting_manual_hyper_parameters
 from .func.algo_regression._knn import knn_manual_hyper_parameters
 from .func.algo_regression._lasso_regression import lasso_regression_manual_hyper_parameters
 from .func.algo_regression._linear_regression import linear_regression_manual_hyper_parameters
 from .func.algo_regression._multi_layer_perceptron import multi_layer_perceptron_manual_hyper_parameters
 from .func.algo_regression._polynomial_regression import polynomial_regression_manual_hyper_parameters
 from .func.algo_regression._rf import random_forest_manual_hyper_parameters
+from .func.algo_regression._ridge_regression import ridge_regression_manual_hyper_parameters
 from .func.algo_regression._sgd_regression import sgd_regression_manual_hyper_parameters
 from .func.algo_regression._svr import svr_manual_hyper_parameters
 from .func.algo_regression._xgboost import xgboost_manual_hyper_parameters
 
 
 class RegressionWorkflowBase(WorkflowBase):
     """The base workflow class of regression algorithms."""
@@ -300,14 +301,16 @@
     def special_components(self, **kwargs) -> None:
         """Invoke all special application functions for this algorithms by Scikit-learn framework."""
         GEOPI_OUTPUT_ARTIFACTS_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_PATH")
         self._show_formula(
             coef=self.model.coef_,
             intercept=self.model.intercept_,
             features_name=self._features_name,
+            regression_classification="Regression",
+            y_train=PolynomialRegression.y,
             algorithm_name=self.naming,
             local_path=GEOPI_OUTPUT_ARTIFACTS_PATH,
             mlflow_path="root",
         )
 
 
 class XGBoostRegression(TreeWorkflowMixin, RegressionWorkflowBase):
@@ -2103,14 +2106,16 @@
         """Invoke all special application functions for this algorithms by Scikit-learn framework."""
         GEOPI_OUTPUT_ARTIFACTS_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_PATH")
         GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH")
         self._show_formula(
             coef=self.model.coef_,
             intercept=self.model.intercept_,
             features_name=ClassicalLinearRegression.X_train.columns,
+            regression_classification="Regression",
+            y_train=ClassicalLinearRegression.y,
             algorithm_name=self.naming,
             local_path=GEOPI_OUTPUT_ARTIFACTS_PATH,
             mlflow_path="root",
         )
         columns_num = ClassicalLinearRegression.X.shape[1]
         if columns_num > 2:
             # choose one of dimensions to draw
@@ -2862,14 +2867,16 @@
         """Invoke all special application functions for this algorithms by Scikit-learn framework."""
         GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH")
         GEOPI_OUTPUT_ARTIFACTS_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_PATH")
         self._show_formula(
             coef=[self.model.coef_],
             intercept=self.model.intercept_,
             features_name=LassoRegression.X_train.columns,
+            regression_classification="Regression",
+            y_train=LassoRegression.y,
             algorithm_name=self.naming,
             local_path=GEOPI_OUTPUT_ARTIFACTS_PATH,
             mlflow_path="root",
         )
         columns_num = LassoRegression.X.shape[1]
         if columns_num > 2:
             # choose one of dimensions to draw
@@ -2941,14 +2948,16 @@
         """Invoke all special application functions for this algorithms by FLAML framework."""
         GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH")
         GEOPI_OUTPUT_ARTIFACTS_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_PATH")
         self._show_formula(
             coef=[self.auto_model.coef_],
             intercept=self.auto_model.intercept_,
             features_name=LassoRegression.X_train.columns,
+            regression_classification="Regression",
+            y_train=LassoRegression.y,
             algorithm_name=self.naming,
             local_path=GEOPI_OUTPUT_ARTIFACTS_PATH,
             mlflow_path="root",
         )
         columns_num = LassoRegression.X.shape[1]
         if columns_num > 2:
             # choose one of dimensions to draw
@@ -3188,14 +3197,16 @@
         """Invoke all special application functions for this algorithms by Scikit-learn framework."""
         GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH")
         GEOPI_OUTPUT_ARTIFACTS_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_PATH")
         self._show_formula(
             coef=[self.model.coef_],
             intercept=self.model.intercept_,
             features_name=ElasticNetRegression.X_train.columns,
+            regression_classification="Regression",
+            y_train=ElasticNetRegression.y,
             algorithm_name=self.naming,
             local_path=GEOPI_OUTPUT_ARTIFACTS_PATH,
             mlflow_path="root",
         )
         columns_num = ElasticNetRegression.X.shape[1]
         if columns_num > 2:
             # choose one of dimensions to draw
@@ -3267,14 +3278,16 @@
         """Invoke all special application functions for this algorithms by FLAML framework."""
         GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH")
         GEOPI_OUTPUT_ARTIFACTS_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_PATH")
         self._show_formula(
             coef=[self.auto_model.coef_],
             intercept=self.auto_model.intercept_,
             features_name=ElasticNetRegression.X_train.columns,
+            regression_classification="Regression",
+            y_train=ElasticNetRegression.y,
             algorithm_name=self.naming,
             local_path=GEOPI_OUTPUT_ARTIFACTS_PATH,
             mlflow_path="root",
         )
         columns_num = ElasticNetRegression.X.shape[1]
         if columns_num > 2:
             # choose one of dimensions to draw
@@ -3618,14 +3631,16 @@
         """Invoke all special application functions for this algorithms by Scikit-learn framework."""
         GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH")
         GEOPI_OUTPUT_ARTIFACTS_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_PATH")
         self._show_formula(
             coef=[self.model.coef_],
             intercept=self.model.intercept_,
             features_name=SGDRegression.X_train.columns,
+            regression_classification="Regression",
+            y_train=SGDRegression.y,
             algorithm_name=self.naming,
             local_path=GEOPI_OUTPUT_ARTIFACTS_PATH,
             mlflow_path="root",
         )
         columns_num = SGDRegression.X.shape[1]
         if columns_num > 2:
             # choose one of dimensions to draw
@@ -3697,14 +3712,16 @@
         """Invoke all special application functions for this algorithms by Scikit-learn framework."""
         GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH")
         GEOPI_OUTPUT_ARTIFACTS_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_PATH")
         self._show_formula(
             coef=[self.auto_model.coef_],
             intercept=self.auto_model.intercept_,
             features_name=SGDRegression.X_train.columns,
+            regression_classification="Regression",
+            y_train=SGDRegression.y,
             algorithm_name=self.naming,
             local_path=GEOPI_OUTPUT_ARTIFACTS_PATH,
             mlflow_path="root",
         )
         columns_num = SGDRegression.X.shape[1]
         if columns_num > 2:
             # choose one of dimensions to draw
@@ -3935,7 +3952,374 @@
     @dispatch()
     def special_components(self, **kwargs) -> None:
         pass
 
     @dispatch(bool)
     def special_components(self, is_automl: bool, **kwargs) -> None:
         pass
+
+
+class RidgeRegression(LinearWorkflowMixin, RegressionWorkflowBase):
+    """The automation workflow of using Lasso to make insightful products."""
+
+    name = "Ridge Regression"
+    special_function = ["Ridge Regression Formula", "2D Scatter Diagram", "3D Scatter Diagram", "2D Line Diagram", "3D Surface Diagram"]
+
+    def __init__(
+        self,
+        alpha: float = 1.0,
+        *,
+        fit_intercept: bool = True,
+        copy_X: bool = True,
+        max_iter: int = 1000,
+        tol: float = 1e-4,
+        solver: str = "auto",
+        positive: bool = False,
+        random_state: Optional[int] = None,
+    ) -> None:
+        """
+        Parameters
+        ----------
+        alpha : {float, ndarray of shape (n_targets,)}, default=1.0
+            Constant that multiplies the L2 term, controlling regularization
+            strength. `alpha` must be a non-negative float i.e. in `[0, inf)`.
+
+            When `alpha = 0`, the objective is equivalent to ordinary least
+            squares, solved by the :class:`LinearRegression` object. For numerical
+            reasons, using `alpha = 0` with the `Ridge` object is not advised.
+            Instead, you should use the :class:`LinearRegression` object.
+
+            If an array is passed, penalties are assumed to be specific to the
+            targets. Hence they must correspond in number.
+
+        fit_intercept : bool, default=True
+            Whether to fit the intercept for this model. If set
+            to false, no intercept will be used in calculations
+            (i.e. ``X`` and ``y`` are expected to be centered).
+
+        copy_X : bool, default=True
+            If True, X will be copied; else, it may be overwritten.
+
+        max_iter : int, default=None
+            Maximum number of iterations for conjugate gradient solver.
+            For 'sparse_cg' and 'lsqr' solvers, the default value is determined
+            by scipy.sparse.linalg. For 'sag' solver, the default value is 1000.
+            For 'lbfgs' solver, the default value is 15000.
+
+        tol : float, default=1e-4
+            The precision of the solution (`coef_`) is determined by `tol` which
+            specifies a different convergence criterion for each solver:
+
+            - 'svd': `tol` has no impact.
+
+            - 'cholesky': `tol` has no impact.
+
+            - 'sparse_cg': norm of residuals smaller than `tol`.
+
+            - 'lsqr': `tol` is set as atol and btol of scipy.sparse.linalg.lsqr,
+              which control the norm of the residual vector in terms of the norms of
+              matrix and coefficients.
+
+            - 'sag' and 'saga': relative change of coef smaller than `tol`.
+
+            - 'lbfgs': maximum of the absolute (projected) gradient=max|residuals|
+              smaller than `tol`.
+
+            .. versionchanged:: 1.2
+               Default value changed from 1e-3 to 1e-4 for consistency with other linear
+               models.
+
+        solver : {'auto', 'svd', 'cholesky', 'lsqr', 'sparse_cg', \
+                'sag', 'saga', 'lbfgs'}, default='auto'
+            Solver to use in the computational routines:
+
+            - 'auto' chooses the solver automatically based on the type of data.
+
+            - 'svd' uses a Singular Value Decomposition of X to compute the Ridge
+              coefficients. It is the most stable solver, in particular more stable
+              for singular matrices than 'cholesky' at the cost of being slower.
+
+            - 'cholesky' uses the standard scipy.linalg.solve function to
+              obtain a closed-form solution.
+
+            - 'sparse_cg' uses the conjugate gradient solver as found in
+              scipy.sparse.linalg.cg. As an iterative algorithm, this solver is
+              more appropriate than 'cholesky' for large-scale data
+              (possibility to set `tol` and `max_iter`).
+
+            - 'lsqr' uses the dedicated regularized least-squares routine
+              scipy.sparse.linalg.lsqr. It is the fastest and uses an iterative
+              procedure.
+
+            - 'sag' uses a Stochastic Average Gradient descent, and 'saga' uses
+              its improved, unbiased version named SAGA. Both methods also use an
+              iterative procedure, and are often faster than other solvers when
+              both n_samples and n_features are large. Note that 'sag' and
+              'saga' fast convergence is only guaranteed on features with
+              approximately the same scale. You can preprocess the data with a
+              scaler from sklearn.preprocessing.
+
+            - 'lbfgs' uses L-BFGS-B algorithm implemented in
+              `scipy.optimize.minimize`. It can be used only when `positive`
+              is True.
+
+            All solvers except 'svd' support both dense and sparse data. However, only
+            'lsqr', 'sag', 'sparse_cg', and 'lbfgs' support sparse input when
+            `fit_intercept` is True.
+
+            .. versionadded:: 0.17
+               Stochastic Average Gradient descent solver.
+            .. versionadded:: 0.19
+               SAGA solver.
+
+        positive : bool, default=False
+            When set to ``True``, forces the coefficients to be positive.
+            Only 'lbfgs' solver is supported in this case.
+
+        random_state : int, RandomState instance, default=None
+            Used when ``solver`` == 'sag' or 'saga' to shuffle the data.
+            See :term:`Glossary <random_state>` for details.
+
+            .. versionadded:: 0.17
+               `random_state` to support Stochastic Average Gradient.
+
+        References
+        ----------
+        Scikit-learn API: sklearn.linear_model.Lasso
+        https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.Ridge.html
+
+        """
+        super().__init__()
+        self.alpha = alpha
+        self.fit_intercept = fit_intercept
+        self.copy_X = copy_X
+        self.max_iter = max_iter
+        self.tol = tol
+        self.solver = solver
+        self.positive = positive
+        self.random_state = random_state
+
+        self.model = Ridge(
+            alpha=self.alpha,
+            fit_intercept=self.fit_intercept,
+            copy_X=self.copy_X,
+            max_iter=self.max_iter,
+            tol=self.tol,
+            solver=self.solver,
+            positive=self.positive,
+            random_state=self.random_state,
+        )
+
+        self.naming = RidgeRegression.name
+        self.customized = True
+        self.customized_name = "Ridge"
+
+    @property
+    def settings(self) -> Dict:
+        """The configuration of Ridge to implement AutoML by FLAML framework."""
+        configuration = {
+            "time_budget": 10,  # total running time in seconds
+            "metric": "r2",
+            "estimator_list": [self.customized_name],  # list of ML learners
+            "task": "regression",  # task type
+            # "log_file_name": f'{self.naming} - automl.log',  # flaml log file
+            # "log_training_metric": True,  # whether to log training metric
+        }
+        return configuration
+
+    @property
+    def customization(self) -> object:
+        """The customized Ridge of FLAML framework."""
+        from flaml import tune
+        from flaml.data import REGRESSION
+        from flaml.model import SKLearnEstimator
+        from sklearn.linear_model import Ridge
+
+        class MyRidgeRegression(SKLearnEstimator):
+            def __init__(self, task="regression", n_jobs=None, **config):
+                super().__init__(task, **config)
+                if task in REGRESSION:
+                    self.estimator_class = Ridge
+
+            @classmethod
+            def search_space(cls, data_size, task):
+                space = {
+                    "alpha": {"domain": tune.uniform(lower=0.001, upper=10), "init_value": 1},
+                    "fit_intercept": {"domain": tune.choice([True, False])},
+                    "max_iter": {"domain": tune.randint(lower=500, upper=2000), "init_value": 1000},
+                    "tol": {"domain": tune.uniform(lower=1e-5, upper=1e-3), "init_value": 1e-4},
+                    # "selection": {"domain": tune.choice(["cyclic", "random"])},
+                    # "random_state": {'domain': tune.choice(["", ""])}
+                }
+                return space
+
+        return MyRidgeRegression
+
+    @classmethod
+    def manual_hyper_parameters(cls) -> Dict:
+        """Manual hyper-parameters specification."""
+        print(f"-*-*- {cls.name} - Hyper-parameters Specification -*-*-")
+        hyper_parameters = ridge_regression_manual_hyper_parameters()
+        clear_output()
+        return hyper_parameters
+
+    @dispatch()
+    def special_components(self, **kwargs) -> None:
+        """Invoke all special application functions for this algorithms by Scikit-learn framework."""
+        GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH")
+        GEOPI_OUTPUT_ARTIFACTS_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_PATH")
+        self._show_formula(
+            coef=[self.model.coef_],
+            intercept=self.model.intercept_,
+            features_name=RidgeRegression.X_train.columns,
+            regression_classification="Regression",
+            y_train=RidgeRegression.y,
+            algorithm_name=self.naming,
+            local_path=GEOPI_OUTPUT_ARTIFACTS_PATH,
+            mlflow_path="root",
+        )
+        columns_num = RidgeRegression.X.shape[1]
+        if columns_num > 2:
+            # choose one of dimensions to draw
+            two_dimen_axis_index, two_dimen_data = self.choose_dimension_data(RidgeRegression.X_test, 1)
+            self._plot_2d_scatter_diagram(
+                feature_data=two_dimen_data,
+                target_data=RidgeRegression.y_test,
+                algorithm_name=self.naming,
+                local_path=GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH,
+                mlflow_path=MLFLOW_ARTIFACT_IMAGE_MODEL_OUTPUT_PATH,
+            )
+            # choose two of dimensions to draw
+            three_dimen_axis_index, three_dimen_data = self.choose_dimension_data(RidgeRegression.X_test, 2)
+            self._plot_3d_scatter_diagram(
+                feature_data=three_dimen_data,
+                target_data=RidgeRegression.y_test,
+                algorithm_name=self.naming,
+                local_path=GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH,
+                mlflow_path=MLFLOW_ARTIFACT_IMAGE_MODEL_OUTPUT_PATH,
+            )
+        elif columns_num == 2:
+            # choose one of dimensions to draw
+            two_dimen_axis_index, two_dimen_data = self.choose_dimension_data(RidgeRegression.X_test, 1)
+            self._plot_2d_scatter_diagram(
+                feature_data=two_dimen_data,
+                target_data=RidgeRegression.y_test,
+                algorithm_name=self.naming,
+                local_path=GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH,
+                mlflow_path=MLFLOW_ARTIFACT_IMAGE_MODEL_OUTPUT_PATH,
+            )
+            # no need to choose
+            self._plot_3d_scatter_diagram(
+                feature_data=RidgeRegression.X_test,
+                target_data=RidgeRegression.y_test,
+                algorithm_name=self.naming,
+                local_path=GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH,
+                mlflow_path=MLFLOW_ARTIFACT_IMAGE_MODEL_OUTPUT_PATH,
+            )
+            self._plot_3d_surface_diagram(
+                feature_data=RidgeRegression.X_test,
+                target_data=RidgeRegression.y_test,
+                y_test_predict=RidgeRegression.y_test_predict,
+                algorithm_name=self.naming,
+                local_path=GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH,
+                mlflow_path=MLFLOW_ARTIFACT_IMAGE_MODEL_OUTPUT_PATH,
+            )
+        elif columns_num == 1:
+            # no need to choose
+            self._plot_2d_scatter_diagram(
+                feature_data=RidgeRegression.X_test,
+                target_data=RidgeRegression.y_test,
+                algorithm_name=self.naming,
+                local_path=GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH,
+                mlflow_path=MLFLOW_ARTIFACT_IMAGE_MODEL_OUTPUT_PATH,
+            )
+            self._plot_2d_line_diagram(
+                feature_data=RidgeRegression.X_test,
+                target_data=RidgeRegression.y_test,
+                y_test_predict=RidgeRegression.y_test_predict,
+                algorithm_name=self.naming,
+                local_path=GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH,
+                mlflow_path=MLFLOW_ARTIFACT_IMAGE_MODEL_OUTPUT_PATH,
+            )
+        else:
+            pass
+
+    @dispatch(bool)
+    def special_components(self, is_automl: bool, **kwargs) -> None:
+        """Invoke all special application functions for this algorithms by FLAML framework."""
+        GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH")
+        GEOPI_OUTPUT_ARTIFACTS_PATH = os.getenv("GEOPI_OUTPUT_ARTIFACTS_PATH")
+        self._show_formula(
+            coef=[self.auto_model.coef_],
+            intercept=self.auto_model.intercept_,
+            features_name=RidgeRegression.X_train.columns,
+            regression_classification="Regression",
+            y_train=RidgeRegression.y,
+            algorithm_name=self.naming,
+            local_path=GEOPI_OUTPUT_ARTIFACTS_PATH,
+            mlflow_path="root",
+        )
+        columns_num = RidgeRegression.X.shape[1]
+        if columns_num > 2:
+            # choose one of dimensions to draw
+            two_dimen_axis_index, two_dimen_data = self.choose_dimension_data(RidgeRegression.X_test, 1)
+            self._plot_2d_scatter_diagram(
+                feature_data=two_dimen_data,
+                target_data=RidgeRegression.y_test,
+                algorithm_name=self.naming,
+                local_path=GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH,
+                mlflow_path=MLFLOW_ARTIFACT_IMAGE_MODEL_OUTPUT_PATH,
+            )
+            # choose two of dimensions to draw
+            three_dimen_axis_index, three_dimen_data = self.choose_dimension_data(RidgeRegression.X_test, 2)
+            self._plot_3d_scatter_diagram(
+                feature_data=three_dimen_data,
+                target_data=RidgeRegression.y_test,
+                algorithm_name=self.naming,
+                local_path=GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH,
+                mlflow_path=MLFLOW_ARTIFACT_IMAGE_MODEL_OUTPUT_PATH,
+            )
+        elif columns_num == 2:
+            # choose one of dimensions to draw
+            two_dimen_axis_index, two_dimen_data = self.choose_dimension_data(RidgeRegression.X_test, 1)
+            self._plot_2d_scatter_diagram(
+                feature_data=two_dimen_data,
+                target_data=RidgeRegression.y_test,
+                algorithm_name=self.naming,
+                local_path=GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH,
+                mlflow_path=MLFLOW_ARTIFACT_IMAGE_MODEL_OUTPUT_PATH,
+            )
+            # no need to choose
+            self._plot_3d_scatter_diagram(
+                feature_data=RidgeRegression.X_test,
+                target_data=RidgeRegression.y_test,
+                algorithm_name=self.naming,
+                local_path=GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH,
+                mlflow_path=MLFLOW_ARTIFACT_IMAGE_MODEL_OUTPUT_PATH,
+            )
+            self._plot_3d_surface_diagram(
+                feature_data=RidgeRegression.X_test,
+                target_data=RidgeRegression.y_test,
+                y_test_predict=RidgeRegression.y_test_predict,
+                algorithm_name=self.naming,
+                local_path=GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH,
+                mlflow_path=MLFLOW_ARTIFACT_IMAGE_MODEL_OUTPUT_PATH,
+            )
+        elif columns_num == 1:
+            # no need to choose
+            self._plot_2d_scatter_diagram(
+                feature_data=RidgeRegression.X_test,
+                target_data=RidgeRegression.y_test,
+                algorithm_name=self.naming,
+                local_path=GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH,
+                mlflow_path=MLFLOW_ARTIFACT_IMAGE_MODEL_OUTPUT_PATH,
+            )
+            self._plot_2d_line_diagram(
+                feature_data=RidgeRegression.X_test,
+                target_data=RidgeRegression.y_test,
+                y_test_predict=RidgeRegression.y_test_predict,
+                algorithm_name=self.naming,
+                local_path=GEOPI_OUTPUT_ARTIFACTS_IMAGE_MODEL_OUTPUT_PATH,
+                mlflow_path=MLFLOW_ARTIFACT_IMAGE_MODEL_OUTPUT_PATH,
+            )
+        else:
+            pass
```

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_classification/_common.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_classification/_common.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_classification/_decision_tree.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_classification/_decision_tree.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_classification/_extra_trees.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_classification/_extra_trees.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_classification/_gradient_boosting.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_classification/_gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_classification/_knn.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_classification/_knn.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_classification/_logistic_regression.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_classification/_logistic_regression.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_classification/_multi_layer_perceptron.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_classification/_multi_layer_perceptron.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_classification/_rf.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_classification/_rf.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_classification/_sgd_classification.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_classification/_sgd_classification.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_classification/_svc.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_classification/_svc.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_classification/_xgboost.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_classification/_xgboost.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_clustering/_agglomerative.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_clustering/_agglomerative.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_clustering/_common.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_clustering/_common.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_clustering/_dbscan.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_clustering/_dbscan.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_clustering/_kmeans.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_clustering/_kmeans.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_decomposition/_mds.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_decomposition/_mds.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_decomposition/_pca.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_decomposition/_pca.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_decomposition/_tsne.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_decomposition/_tsne.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_bayesianridge_regression.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_bayesianridge_regression.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_common.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_common.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_decision_tree.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_decision_tree.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_elastic_net.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_elastic_net.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_extra_tree.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_extra_tree.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_gradient_boosting.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_knn.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_knn.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_lasso_regression.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_lasso_regression.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_linear_regression.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_linear_regression.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_multi_layer_perceptron.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_multi_layer_perceptron.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_polynomial_regression.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_polynomial_regression.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_rf.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_rf.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_sgd_regression.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_sgd_regression.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_svr.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_svr.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/model/func/algo_regression/_xgboost.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/model/func/algo_regression/_xgboost.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/plot/geochemistry_plot.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/plot/geochemistry_plot.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/plot/map_plot.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/plot/map_plot.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/plot/statistic_plot.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/plot/statistic_plot.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/process/classify.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/process/classify.py`

 * *Files 7% similar despite different names*

```diff
@@ -163,29 +163,33 @@
                 validation_fraction=hyper_parameters["validation_fraction"],
                 n_iter_no_change=hyper_parameters["n_iter_no_change"],
             )
         self.clf_workflow.show_info()
 
         # Use Scikit-learn style API to process input data
         self.clf_workflow.fit(X_train, y_train)
+        y_train_predict = self.clf_workflow.predict(X_train)
+        y_train_predict = self.clf_workflow.np2pd(y_train_predict, y_train.columns)
+        self.clf_workflow.data_upload(y_train_predict=y_train_predict)
         y_test_predict = self.clf_workflow.predict(X_test)
         y_test_predict = self.clf_workflow.np2pd(y_test_predict, y_test.columns)
         self.clf_workflow.data_upload(X=X, y=y, X_train=X_train, X_test=X_test, y_train=y_train, y_test=y_test, y_test_predict=y_test_predict)
 
         # Save the model hyper-parameters
         self.clf_workflow.save_hyper_parameters(hyper_parameters, self.model_name, os.getenv("GEOPI_OUTPUT_PARAMETERS_PATH"))
 
         # Common components for every classification algorithm
         self.clf_workflow.common_components()
 
         # Special components of different algorithms
         self.clf_workflow.special_components()
 
         # Save the prediction result
-        self.clf_workflow.data_save(y_test_predict, "Y Test Predict", os.getenv("GEOPI_OUTPUT_ARTIFACTS_DATA_PATH"), MLFLOW_ARTIFACT_DATA_PATH, "Model Prediction")
+        self.clf_workflow.data_save(y_train_predict, "Y Train Predict", os.getenv("GEOPI_OUTPUT_ARTIFACTS_DATA_PATH"), MLFLOW_ARTIFACT_DATA_PATH, "Model Train Prediction")
+        self.clf_workflow.data_save(y_test_predict, "Y Test Predict", os.getenv("GEOPI_OUTPUT_ARTIFACTS_DATA_PATH"), MLFLOW_ARTIFACT_DATA_PATH, "Model Test Prediction")
 
         # Save the trained model
         self.clf_workflow.model_save()
 
     @dispatch(object, object, object, object, object, object, bool)
     def activate(
         self,
@@ -229,14 +233,17 @@
         elif self.model_name == "Stochastic Gradient Descent":
             self.clf_workflow = SGDClassification()
 
         self.clf_workflow.show_info()
 
         # Use Scikit-learn style API to process input data
         self.clf_workflow.fit(X_train, y_train, is_automl)
+        y_train_predict = self.clf_workflow.predict(X_train, is_automl)
+        y_train_predict = self.clf_workflow.np2pd(y_train_predict, y_train.columns)
+        self.clf_workflow.data_upload(y_train_predict=y_train_predict)
         y_test_predict = self.clf_workflow.predict(X_test, is_automl)
         y_test_predict = self.clf_workflow.np2pd(y_test_predict, y_test.columns)
         self.clf_workflow.data_upload(X=X, y=y, X_train=X_train, X_test=X_test, y_train=y_train, y_test=y_test, y_test_predict=y_test_predict)
 
         # Save the model hyper-parameters
         if self.clf_workflow.ray_best_model is not None:
             self.clf_workflow.save_hyper_parameters(self.clf_workflow.ray_best_model.get_params(), self.model_name, os.getenv("GEOPI_OUTPUT_PARAMETERS_PATH"))
@@ -246,11 +253,12 @@
         # Common components for every classification algorithm
         self.clf_workflow.common_components(is_automl)
 
         # Special components of different algorithms
         self.clf_workflow.special_components(is_automl)
 
         # Save the prediction result
-        self.clf_workflow.data_save(y_test_predict, "Y Test Predict", os.getenv("GEOPI_OUTPUT_ARTIFACTS_DATA_PATH"), MLFLOW_ARTIFACT_DATA_PATH, "Model Prediction")
+        self.clf_workflow.data_save(y_train_predict, "Y Train Predict", os.getenv("GEOPI_OUTPUT_ARTIFACTS_DATA_PATH"), MLFLOW_ARTIFACT_DATA_PATH, "Model Train Prediction")
+        self.clf_workflow.data_save(y_test_predict, "Y Test Predict", os.getenv("GEOPI_OUTPUT_ARTIFACTS_DATA_PATH"), MLFLOW_ARTIFACT_DATA_PATH, "Model Test Prediction")
 
         # Save the trained model
         self.clf_workflow.model_save(is_automl)
```

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/process/cluster.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/process/cluster.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 import os
 from typing import Optional
 
 import pandas as pd
 
-from ..model.clustering import Agglomerative, ClusteringWorkflowBase, DBSCANClustering, KMeansClustering
+from ..model.clustering import AffinityPropagationClustering, Agglomerative, ClusteringWorkflowBase, DBSCANClustering, KMeansClustering
 from ._base import ModelSelectionBase
 
 
 class ClusteringModelSelection(ModelSelectionBase):
     """Simulate the normal way of invoking scikit-learn clustering algorithms."""
 
     def __init__(self, model_name: str) -> None:
@@ -50,14 +50,22 @@
             )
         elif self.model_name == "Agglomerative":
             hyper_parameters = Agglomerative.manual_hyper_parameters()
             self.clt_workflow = Agglomerative(
                 n_clusters=hyper_parameters["n_clusters"],
                 linkage=hyper_parameters["linkage"],
             )
+        elif self.model_name == "AffinityPropagation":
+            hyper_parameters = AffinityPropagationClustering.manual_hyper_parameters()
+            self.clt_workflow = AffinityPropagationClustering(
+                damping=hyper_parameters["damping"],
+                max_iter=hyper_parameters["max_iter"],
+                convergence_iter=hyper_parameters["convergence_iter"],
+                affinity=hyper_parameters["affinity"],
+            )
         elif self.model_name == "":
             pass
 
         self.clt_workflow.show_info()
 
         # Use Scikit-learn style API to process input data
         self.clt_workflow.fit(X)
```

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/process/decompose.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/process/decompose.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,17 @@
         X_reduced = self.dcp_workflow.fit_transform(X)
         X_reduced = self.dcp_workflow.np2pd(X_reduced, [f"Dimension {i+1}" for i in range(X_reduced.shape[1])])
         self.dcp_workflow.data_upload(X=X)
 
         # Save the model hyper-parameters
         self.dcp_workflow.save_hyper_parameters(hyper_parameters, self.model_name, os.getenv("GEOPI_OUTPUT_PARAMETERS_PATH"))
 
+        # Common components for every decomposition algorithm
+        self.dcp_workflow.common_components()
+
         # special components of different algorithms
         self.dcp_workflow.special_components(components_num=hyper_parameters["n_components"], reduced_data=X_reduced)
 
         # Save decomposition result
         self.dcp_workflow.data_save(X_reduced, "X Reduced", os.getenv("GEOPI_OUTPUT_ARTIFACTS_DATA_PATH"), MLFLOW_ARTIFACT_DATA_PATH, "Reduced Data")
 
         # Save the trained model
```

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/process/regress.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/process/regress.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     GradientBoostingRegression,
     KNNRegression,
     LassoRegression,
     MLPRegression,
     PolynomialRegression,
     RandomForestRegression,
     RegressionWorkflowBase,
+    RidgeRegression,
     SGDRegression,
     SVMRegression,
     XGBoostRegression,
 )
 from ._base import ModelSelectionBase
 
 
@@ -193,34 +194,46 @@
                 alpha_init=hyper_parameters["alpha_init"],
                 lambda_init=hyper_parameters["lambda_init"],
                 compute_score=hyper_parameters["compute_score"],
                 fit_intercept=hyper_parameters["fit_intercept"],
                 copy_X=hyper_parameters["copy_X"],
                 verbose=hyper_parameters["verbose"],
             )
+        elif self.model_name == "Ridge Regression":
+            hyper_parameters = RidgeRegression.manual_hyper_parameters()
+            self.reg_workflow = RidgeRegression(
+                alpha=hyper_parameters["alpha"],
+                fit_intercept=hyper_parameters["fit_intercept"],
+                max_iter=hyper_parameters["max_iter"],
+                tol=hyper_parameters["tol"],
+            )
 
         self.reg_workflow.show_info()
 
         # Use Scikit-learn style API to process input data
         self.reg_workflow.fit(X_train, y_train)
+        y_train_predict = self.reg_workflow.predict(X_train)
+        y_train_predict = self.reg_workflow.np2pd(y_train_predict, y_train.columns)
+        self.reg_workflow.data_upload(y_train_predict=y_train_predict)
         y_test_predict = self.reg_workflow.predict(X_test)
         y_test_predict = self.reg_workflow.np2pd(y_test_predict, y_test.columns)
         self.reg_workflow.data_upload(y_test_predict=y_test_predict)
 
         # Save the model hyper-parameters
         self.reg_workflow.save_hyper_parameters(hyper_parameters, self.model_name, os.getenv("GEOPI_OUTPUT_PARAMETERS_PATH"))
 
         # Common components for every regression algorithm
         self.reg_workflow.common_components()
 
         # Special components of different algorithms
         self.reg_workflow.special_components()
 
         # Save the prediction result
-        self.reg_workflow.data_save(y_test_predict, "Y Test Predict", os.getenv("GEOPI_OUTPUT_ARTIFACTS_DATA_PATH"), MLFLOW_ARTIFACT_DATA_PATH, "Model Prediction")
+        self.reg_workflow.data_save(y_train_predict, "Y Train Predict", os.getenv("GEOPI_OUTPUT_ARTIFACTS_DATA_PATH"), MLFLOW_ARTIFACT_DATA_PATH, "Model Train Prediction")
+        self.reg_workflow.data_save(y_test_predict, "Y Test Predict", os.getenv("GEOPI_OUTPUT_ARTIFACTS_DATA_PATH"), MLFLOW_ARTIFACT_DATA_PATH, "Model Test Prediction")
 
         # Save the trained model
         self.reg_workflow.model_save()
 
     @dispatch(object, object, object, object, object, object, bool)
     def activate(
         self,
@@ -266,19 +279,24 @@
             self.reg_workflow = LassoRegression()
         elif self.model_name == "Elastic Net":
             self.reg_workflow = ElasticNetRegression()
         elif self.model_name == "SGD Regression":
             self.reg_workflow = SGDRegression()
         elif self.model_name == "BayesianRidge Regression":
             self.reg_workflow = BayesianRidgeRegression()
+        elif self.model_name == "Ridge Regression":
+            self.reg_workflow = RidgeRegression()
 
         self.reg_workflow.show_info()
 
         # Use Scikit-learn style API to process input data
         self.reg_workflow.fit(X_train, y_train, is_automl)
+        y_train_predict = self.reg_workflow.predict(X_train, is_automl)
+        y_train_predict = self.reg_workflow.np2pd(y_train_predict, y_train.columns)
+        self.reg_workflow.data_upload(y_train_predict=y_train_predict)
         y_test_predict = self.reg_workflow.predict(X_test, is_automl)
         y_test_predict = self.reg_workflow.np2pd(y_test_predict, y_test.columns)
         self.reg_workflow.data_upload(y_test_predict=y_test_predict)
 
         # Save the model hyper-parameters
         if self.reg_workflow.ray_best_model is not None:
             self.reg_workflow.save_hyper_parameters(self.reg_workflow.ray_best_model.get_params(), self.model_name, os.getenv("GEOPI_OUTPUT_PARAMETERS_PATH"))
@@ -288,11 +306,12 @@
         # Common components for every regression algorithm
         self.reg_workflow.common_components(is_automl)
 
         # Special components of different algorithms
         self.reg_workflow.special_components(is_automl)
 
         # Save the prediction result
-        self.reg_workflow.data_save(y_test_predict, "Y Test Predict", os.getenv("GEOPI_OUTPUT_ARTIFACTS_DATA_PATH"), MLFLOW_ARTIFACT_DATA_PATH, "Model Prediction")
+        self.reg_workflow.data_save(y_train_predict, "Y Train Predict", os.getenv("GEOPI_OUTPUT_ARTIFACTS_DATA_PATH"), MLFLOW_ARTIFACT_DATA_PATH, "Model Train Prediction")
+        self.reg_workflow.data_save(y_test_predict, "Y Test Predict", os.getenv("GEOPI_OUTPUT_ARTIFACTS_DATA_PATH"), MLFLOW_ARTIFACT_DATA_PATH, "Model Test Prediction")
 
         # Save the trained model
         self.reg_workflow.model_save(is_automl)
```

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/tests/test_data/test_data_readiness.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/tests/test_data/test_data_readiness.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/utils/base.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/utils/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 import logging
 import os
 import pickle
 import platform
+import shutil
 from typing import Optional
 
 import joblib
 import mlflow
 import pandas as pd
 from matplotlib import pyplot as plt
 from rich import print
@@ -78,14 +79,19 @@
     os.makedirs(geopi_output_parameters_path, exist_ok=True)
 
     # Set the outout metrics path for the current run
     geopi_output_metrics_path = os.path.join(geopi_output_path, "metrics")
     os.environ["GEOPI_OUTPUT_METRICS_PATH"] = geopi_output_metrics_path
     os.makedirs(geopi_output_metrics_path, exist_ok=True)
 
+    # Set the summary outout path for the current run
+    geopi_output_summary_path = os.path.join(geopi_output_path, "summary")
+    os.environ["GEOPI_OUTPUT_SUMMARY_PATH"] = geopi_output_summary_path
+    os.makedirs(geopi_output_summary_path, exist_ok=True)
+
 
 def get_os() -> str:
     """Get the operating system.
 
     Returns
     -------
     str
@@ -305,7 +311,32 @@
 
     if not is_show:
         if not sys.warnoptions:
             import os
 
             os.environ["PYTHONWARNINGS"] = "ignore"
             # os.environ["PYTHONWARNINGS"] = "default"
+
+
+def copy_files(GEOPI_OUTPUT_ARTIFACTS_PATH: str, GEOPI_OUTPUT_METRICS_PATH: str, GEOPI_OUTPUT_PARAMETERS_PATH: str, GEOPI_OUTPUT_SUMMARY_PATH: str) -> None:
+    """Copy all files from the source folder to the destination folder.
+
+    Parameters
+    ----------
+    GEOPI_OUTPUT_ARTIFACTS_PATH: str
+        Source folder path.
+
+    GEOPI_OUTPUT_METRICS_PATH: str
+        Source folder path.
+
+    GEOPI_OUTPUT_PARAMETERS_PATH: str
+        Source folder path.
+
+    GEOPI_OUTPUT_SUMMARY_PATH: str
+        Destination folder path
+    """
+    source_paths = [GEOPI_OUTPUT_ARTIFACTS_PATH, GEOPI_OUTPUT_METRICS_PATH, GEOPI_OUTPUT_PARAMETERS_PATH]
+    for source_path in source_paths:
+        for root, dirs, files in os.walk(source_path):
+            for file in files:
+                source_file_path = os.path.join(root, file)
+                shutil.copy2(source_file_path, GEOPI_OUTPUT_SUMMARY_PATH)
```

### Comparing `geochemistrypi-0.5.0/geochemistrypi/data_mining/utils/mlflow_utils.py` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/utils/mlflow_utils.py`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/frontend/.eslintrc.js` & `geochemistrypi-0.6.0/geochemistrypi/frontend/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/frontend/package.json` & `geochemistrypi-0.6.0/geochemistrypi/frontend/package.json`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/frontend/tsconfig.json` & `geochemistrypi-0.6.0/geochemistrypi/frontend/tsconfig.json`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/frontend/webpack.config.js` & `geochemistrypi-0.6.0/geochemistrypi/frontend/webpack.config.js`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/frontend/src/App.tsx` & `geochemistrypi-0.6.0/geochemistrypi/frontend/src/App.tsx`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/frontend/src/components/DataFrame.tsx` & `geochemistrypi-0.6.0/geochemistrypi/frontend/src/components/DataFrame.tsx`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/frontend/src/components/Dataset.tsx` & `geochemistrypi-0.6.0/geochemistrypi/frontend/src/components/Dataset.tsx`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/frontend/src/components/DatasetDisplay.tsx` & `geochemistrypi-0.6.0/geochemistrypi/frontend/src/components/DatasetDisplay.tsx`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/frontend/src/components/Header.tsx` & `geochemistrypi-0.6.0/geochemistrypi/frontend/src/components/Header.tsx`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/frontend/src/components/Login.tsx` & `geochemistrypi-0.6.0/geochemistrypi/frontend/src/components/Login.tsx`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/frontend/src/components/Profile.tsx` & `geochemistrypi-0.6.0/geochemistrypi/frontend/src/components/Profile.tsx`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/frontend/src/components/RefreshHandler.tsx` & `geochemistrypi-0.6.0/geochemistrypi/frontend/src/components/RefreshHandler.tsx`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/frontend/src/components/Register.tsx` & `geochemistrypi-0.6.0/geochemistrypi/frontend/src/components/Register.tsx`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/frontend/src/helpers/apiCall.ts` & `geochemistrypi-0.6.0/geochemistrypi/frontend/src/helpers/apiCall.ts`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/frontend/src/helpers/apiCallWrappers.ts` & `geochemistrypi-0.6.0/geochemistrypi/frontend/src/helpers/apiCallWrappers.ts`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/frontend/src/pages/HomePage.tsx` & `geochemistrypi-0.6.0/geochemistrypi/frontend/src/pages/HomePage.tsx`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/geochemistrypi/frontend/src/pages/LoginPage.tsx` & `geochemistrypi-0.6.0/geochemistrypi/frontend/src/pages/LoginPage.tsx`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/requirements/development.txt` & `geochemistrypi-0.6.0/requirements/development.txt`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/test/Data_Binary_Classification.xlsx` & `geochemistrypi-0.6.0/geochemistrypi/data_mining/data/dataset/Data_Classification.xlsx`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/.gitignore` & `geochemistrypi-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/LICENSE` & `geochemistrypi-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geochemistrypi-0.5.0/README.md` & `geochemistrypi-0.6.0/docs/source/Home/Introduction.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-<p>
-<img src="https://github.com/ZJUEarthData/geochemistrypi/assets/47497750/6f970708-7811-40bb-8172-9b98563c7659" class="center"/>
-</p>
+![Geochemistry π.png](https://github.com/ZJUEarthData/geochemistrypi/assets/66779478/8b8c9a61-68bb-40ca-8545-c96e6802bda5)
 <p align="center">
-<img src="https://img.shields.io/github/actions/workflow/status/ZJUEarthData/geochemistrypi/geochemistrypi.yml?logo=github">
+<img src="https://img.shields.io/github/actions/workflow/status/ZJUEarthData/geochemistrypi/geochemistrypy.yml?logo=github">
 <img src="https://img.shields.io/github/license/ZJUEarthData/geochemistrypi">
 <img src="https://img.shields.io/github/v/release/ZJUEarthData/geochemistrypi?include_prereleases">
 <img src="https://static.pepy.tech/personalized-badge/geochemistrypi?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads">
-<img src="https://img.shields.io/pypi/pyversions/geochemistrypi">
 </p>
 
 ---
 
 **Documentation**: <a href="https://geochemistrypi.readthedocs.io" target="_blank">https://geochemistrypi.readthedocs.io</a>
 
- **Source Code**: <a href="https://github.com/ZJUEarthData/geochemistrypi" target="_blank">https://github.com/ZJUEarthData/geochemistrypi</a>
+**Source Code**: <a href="https://github.com/ZJUEarthData/geochemistrypi" target="_blank">https://github.com/ZJUEarthData/geochemistrypi</a>
 
 ---
 
+# Introduction
+
+## What it is
+
 Geochemistry π is an **open-sourced highly automated machine learning Python framework** dedicating to build up MLOps level 1 software product for data-driven geochemistry discovery on tabular data.
 
 Core capabilities are:
 
 + **Continous Training**
 + **Machine Learning Lifecycle Management**
 + **Model Inference**
@@ -41,29 +42,53 @@
 
 The following figure is the frontend-backend separation architecture of Geochemistry: <br>
 
 <p align="center">
   <img src="https://github.com/ZJUEarthData/geochemistrypi/assets/47497750/3b27cbdb-ff50-4fa6-b1d1-4c75b253fdff" alt="Frontend-backend separation architecture of Geochemistry" width="450" />
 </p>
 
+
+**If the software contributes to your research, cite the work as :**
+
+ZhangZhou J\*, He Can\*, Sun Jianhao, Zhao Jianming, Lyu Yang, Wang Shengxin, Zhao Wenyu, Li Anzhou, Ji Xiaohui. Geochemistry π: Automated machine learning python framework for tabular data (2024). Geochemistry, Geophysics,
+Geosystems, 25, e2023GC011324
+
+Download link: https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2023GC011324
+
+**Related report:**
+
+Geochemistry π was selected for featuring as an Editor’s Highlight in EOS magazine by American Geophysical Union (fewer than 2 percent of paper are selected) and quoted in Geochemical NEWS by Geochemical Society.
+
+Eos Website: https://eos.org/editor-highlights/machine-learning-for-geochemists-who-dont-want-to-code.
+
 ## Quick Installation
 
+Our software is well tested on **macOS** and **Windows** system with **Python 3.9**. Other systems and Python version are not guranteed.
+
 One instruction to download on **command line**, such as Terminal on macOS, Power Shell on Windows.
 
 ```
 pip install geochemistrypi
 ```
 
+Download the latest version to avoid some old version issues, such as dependency downloading.
+```
+pip install "geochemistrypi==0.5.0"
+```
+
 One instruction to download on **Jupyter Notebook** or **Google Colab**.
 
 ```
 !pip install geochemistrypi
 ```
-
-Check the latest version of our software:
+Download the latest version to avoid some old version issues, such as dependency downloading.
+```
+!pip install "geochemistrypi==0.5.0"
+```
+Check the downloaded version of our software:
 
 ```
 geochemistrypi --version
 ```
 
 **Note**: For more detail on installation, please refer to our online documentation in **Installation Manual** under the section of **FOR USER**. Over there, we highly recommend to use virtual environment (Conda) to avoid dependency version problems.
 
@@ -77,21 +102,60 @@
 
 One instruction to download on **Jupyter Notebook** or **Google Colab**.
 
 ```
 !pip install --upgrade geochemistrypi
 ```
 
-Check the latest version of our software:
+Check the updated version of our software:
 
 ```
 geochemistrypi --version
 ```
 
-## Example
+## Data Preparation
+
+In order to utilize the functions provided by our software, your own data set should satisfy:
+
+- be with the suffix **.xlsx** or **.csv**, which is supported by Microsoft Excel.
+- be comprise of location information **LATITUDE** and **LONGITUDE**, two columns respectively. It is optional.
+
+If you want to run **classification** algorithm, you data set should satisfy:
+
+- a label column. You can name it as you wish, such as **Label**.
+
+Column name specification:
+
+- No restriction on the column names.  You can name them as you want except for two special and optional column **LATITUDE** and **LONGITUDE**.
+
+- every column can only one column name. Multi level column names are not allowed.
+
+- Between two columns with values, a completed void column can exists.
+
+The following are seven built-in data sets in our software stored on Google Drive and Tecent Docs, have a look on them. For the algorithm you intend to run, you can refer to the data format of the corresponding dataset.
+
++ Data_Regression.xlsx [[Google Drive]](https://docs.google.com/spreadsheets/d/13MB4t_2PiZ90tTMJKw7HcBUi2sb3tXej/edit?usp=sharing&ouid=110717816678586054594&rtpof=true&sd=true) | [[Tencent Docs]](https://docs.qq.com/document/DQ3VmdWZCTGV3bmpM?&u=6868f96d4a384b309036e04e637e367a)
+
++ ApplicationData_Regression.xlsx [[Google Drive]](https://docs.google.com/spreadsheets/d/1FCek2OOYQD887jfQz21g0ovqVuUJIjVoNI77D-Ufr9Y/edit?usp=sharing) | [[Tencent Docs]](
+https://docs.qq.com/document/DQ3BDeHhxRGNzSXZN)
+
++ Data_Classification.xlsx [[Google Drive]](https://docs.google.com/spreadsheets/d/1xFBCYVmtZfuEAbeBljUlzqBjxVuLAt8x/edit?usp=sharing&ouid=110717816678586054594&rtpof=true&sd=true) | [[Tencent Docs]](https://docs.qq.com/document/DQ0JUaUFsZnRaZkNG?&u=6868f96d4a384b309036e04e637e367a)
+
++ ApplicationData_Classification.xlsx [[Google Drive]](https://docs.google.com/spreadsheets/d/1J7QvdvbbHJMlKtiumBgKDW7ALghfQQZyKGEoOqhKQjw/edit?usp=sharing) | [[Tencent Docs]](https://docs.qq.com/document/DQ2dnQWtubHRBTGtB)
+
++ Data_Clustering.xlsx [[Google Drive]](https://docs.google.com/spreadsheets/d/1sbuJdOzGNQ2Pk-bVURfPYg1rltyBbn5J/edit?usp=sharing&ouid=110717816678586054594&rtpof=true&sd=true) | [[Tencent Docs]](https://docs.qq.com/document/DQ3dKdGtlWkhZS2xR?&u=6868f96d4a384b309036e04e637e367a)
+
++ Data_Decomposition.xlsx [[Google Drive]](https://docs.google.com/spreadsheets/d/1kix82qj5--vhnm8-KhuUBH9dqYH6zcY8/edit?usp=sharing&ouid=110717816678586054594&rtpof=true&sd=true) | [[Tencent Docs]](https://docs.qq.com/document/DQ29oZ0lhUGtZUmdN?&u=6868f96d4a384b309036e04e637e367a)
+
++  Data_AbnormalDetectioon.xlsx [[Google Drive]](https://docs.google.com/spreadsheets/d/1NqTQZCkv74Sn_iOJOKRc-QnJzpaWmnzC_lET_0ZreiQ/edit?usp=sharing) | [[Tencent Docs]](
+https://docs.qq.com/document/DQ2hqQ2N2ZGlOUWlT)
+
+**Note**: For more detail on data preparation, please refer to our online documentation in **Model Example** under the section of **FOR USER**.
+
+## Running Example
 
 **How to run:** After successfully downloading, run this instruction on **command line / Jupyter Notebook / Google Colab** whatever directory it is.
 
 ### Case 1: Run with built-in data set for testing
 
 On command line:
 
@@ -157,18 +221,25 @@
 
 **Note**: Once you run our software, there are two folders (`geopi_output` and `geopi_tracking`) generated automatically. Make sure the directory where you execute using the above command should have the genereted file `geopi_tracking`.
 
 Copy the URL shown on the console into any browser to open the MLflow web interface. The URL is normally like this http://127.0.0.1:5000. Search MLflow online to see more operations and usages.
 
 For more details: Please refer to:
 
-+ [Manual v1.1.0 for Geochemistry π - Beta (International - Google drive)](https://drive.google.com/file/d/1yryykCyWKM-Sj88fOYbOba6QkB_fu2ws/view?usp=sharing)
-+ [Manual v1.1.0 for Geochemistry π - Beta (China - Tencent Docs)](https://docs.qq.com/pdf/DQ0l5d2xVd2VwcnVW?&u=6868f96d4a384b309036e04e637e367a)
-+ [Geochemistry π - Download and Run the Beta Version (International - Youtube)](https://www.youtube.com/watch?v=EeVaJ3H7_AU&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM&index=9)
-+ [Geochemistry π - Download and Run the Beta Version (China - Bilibili)](https://www.bilibili.com/video/BV1UM4y1Q7Ju/?spm_id_from=333.999.0.0&vd_source=27944ab3b73a78970c1a52a5dcbb9140)
+- Manual v1.1.0 for Geochemistry π - Beta [[Tencent Docs]](https://docs.qq.com/pdf/DQ0l5d2xVd2VwcnVW?&u=6868f96d4a384b309036e04e637e367a) | [[Google drive]](https://drive.google.com/file/d/1yryykCyWKM-Sj88fOYbOba6QkB_fu2ws/view?usp=sharing)
+
+- Geochemistry π - Download and Run the Beta Version [[Bilibili]](https://www.bilibili.com/video/BV1UM4y1Q7Ju/?spm_id_from=333.999.0.0&vd_source=27944ab3b73a78970c1a52a5dcbb9140) | [[YouTube]](https://www.youtube.com/watch?v=EeVaJ3H7_AU&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM&index=9)
+
+- MLflow UI user guide - Geochemistry π v0.5.0 [[Bilibili]](https://b23.tv/CW5Rjmo) | [[YouTube]](https://www.youtube.com/watch?v=Yu1nzNeLfRY)
+
+The following screenshot shows the downloads and launching of our software on macOS:
+
+<p align="center">
+  <img src="https://github.com/ZJUEarthData/geochemistrypi/assets/47497750/70728795-59b7-4741-ab5b-9e63d284ad37" alt="Downloads and Launching on macOS" width="450" />
+</p>
 
 ## Roadmap
 
 ### First Phase
 
 It works as a **software application** with a command-line interface (CLI) to automate **data mining** process with frequently-used **machine learning algorithms** and **statistical analysis methods**, which would further lower the threshold for the geochemists.
 
@@ -211,43 +282,48 @@
 
 <p align="center">
   <img src="https://github.com/ZJUEarthData/geochemistrypi/assets/47497750/401f3429-c44f-4b76-b085-7a9dcc987cde" alt="Storage Mechanism" width="500" />
 </p>
 
 The whole package is under construction and the documentation is progressively evolving.
 
+## Geochemistry π Mind Map
+
+[→ Click here for more details](https://docs.qq.com/mind/DZnhoa2NPamFYZHR6?u=40ac0718eb494b008b2f072197ea95db)
+
+![Geochemistry π.png](https://github.com/ZJUEarthData/geochemistrypi/assets/97781484/e77b1f11-41ab-4354-9064-6d62cc1bf1e4)
+
 ## Team Info
 
 **Leader:**
 
 + Can He (Sany, National University of Singapore, Singapore)
   Email: sanyhew1097618435@163.com
 
 **Technical Group:**
 
 + Jianming Zhao (Jamie, Zhejiang University, China)
 + Jianhao Sun (Jin, China University of Geosciences, Wuhan, China)
-+ Kaixin Zheng (Hayne, Sun Yat-sen University, China)
-+ Jianing Wang (National University of Singapore, Singapore)
 + Yongkang Chan (Kill-virus, Lanzhou University, China)
 + Mengying Ye (Mary, Jilin University, China)
 + Mengqi Gao (China University of Geosciences, Beijing, China)
 + Chengtu Li（Trenki, Henan Polytechnic University, Beijing, China）
++ Yucheng Yan (Andy, University of Sydney, Australia)
 
 **Product Group**:
 
 + Yang Lyu (Daisy, Zhejiang University, China)
-+ Wenyu Zhao (Molly, Zhejiang University, China)
-+ Keran Li (Kirk, Chengdu University of Technology, China)
-+ Aixiwake·Janganuer (Ayshuak, Sun Yat-sen University, China)
 + Bailun Jiang (EPSI / Lille University, France)
-+ Yucheng Yan (Andy, University of Sydney, Australia)
 + Ruitao Chang (China University of Geosciences Beijing, China)
-+ Zhenglin Xu (Garry, Jilin University, China)
 + Junchi Liao(Roceda, University of Electronic Science and Technology of China, China)
++ Panyan Weng (The University of Sydney, Australia)
++ Siqi Yao (Clara, Dongguan University of Technology, China)
++ Zhelan Lin（Lan, Fuzhou University, China）
++ ShuYi Li (Communication University Of China, Beijing, China)
++ Junbo Wang (China University Of Geosciences, Beijing, China)
 
 ## Join Us :)
 
 **The recruitment of research interns is ongoing !!!**
 
 **Key Point: All things are done online, remote work (\*^▽^\*)**
 
@@ -304,15 +380,21 @@
 5. [How to use Github-Desktop in conflict resolution - Qiuhao Zhao (Brad)](https://www.youtube.com/watch?v=KT1g5JpuUVI&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM)
 6. [Virtual Environment &amp; Packages On Windows - Jianming Zhao (Jamie)](https://www.youtube.com/watch?v=e4VqSBuNp_o&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM&index=2)
 7. [Git Workflow &amp; Coordinating Synchronization - Jianming Zhao (Jamie)](https://www.bilibili.com/video/BV1Sa4y1f74k?spm_id_from=333.999.0.0&vd_source=9adcf2c5fdeffe1d11c89d441ef598ba)
 
 ## Contributors
 
 + Shengxin Wang (Samson, Lanzhou University, China)
++ Wenyu Zhao (Molly, Zhejiang University, China)
 + Qiuhao Zhao (Brad, Zhejiang University, China)
++ Kaixin Zheng (Hayne, Sun Yat-sen University, China)
 + Anzhou Li (Andrian, Zhejiang University, China)
++ Keran Li (Kirk, Chengdu University of Technology, China)
 + Dan Hu (Notre Dame University, United States)
 + Xunxin Liu (Tante, China University of Geosciences, Wuhan, China)
 + Fang Li (liv, Shenzhen University, China)
 + Xin Li (The University of Manchester, United Kingdom)
 + Ting Liu (Kira, Sun Yat-sen University, China)
 + Xirui Zhu (Rae, University of York, United Kingdom)
++ Aixiwake·Janganuer (Ayshuak, Sun Yat-sen University, China)
++ Zhenglin Xu (Garry, Jilin University, China)
++ Jianing Wang (National University of Singapore, Singapore)
```

#### html2text {}

```diff
@@ -1,57 +1,116 @@
-[https://github.com/ZJUEarthData/geochemistrypi/assets/47497750/6f970708-7811-
-40bb-8172-9b98563c7659]
+![Geochemistry Ï.png](https://github.com/ZJUEarthData/geochemistrypi/assets/
+66779478/8b8c9a61-68bb-40ca-8545-c96e6802bda5)
      [https://img.shields.io/github/actions/workflow/status/ZJUEarthData/
- geochemistrypi/geochemistrypi.yml?logo=github][https://img.shields.io/github/
+ geochemistrypi/geochemistrypy.yml?logo=github][https://img.shields.io/github/
  license/ZJUEarthData/geochemistrypi][https://img.shields.io/github/v/release/
   ZJUEarthData/geochemistrypi?include_prereleases][https://static.pepy.tech/
                               personalized-badge/
 geochemistrypi?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads]
-            [https://img.shields.io/pypi/pyversions/geochemistrypi]
 --- **Documentation**: _h_t_t_p_s_:_/_/_g_e_o_c_h_e_m_i_s_t_r_y_p_i_._r_e_a_d_t_h_e_d_o_c_s_._i_o **Source Code**:
-_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_Z_J_U_E_a_r_t_h_D_a_t_a_/_g_e_o_c_h_e_m_i_s_t_r_y_p_i --- Geochemistry Ï is an
-**open-sourced highly automated machine learning Python framework** dedicating
-to build up MLOps level 1 software product for data-driven geochemistry
-discovery on tabular data. Core capabilities are: + **Continous Training** +
-**Machine Learning Lifecycle Management** + **Model Inference** Key features
-are: + **Easy to use:** The automation of data mining process provides the
-users with simple number options to choose. + **Extensible:** It allows
-appending new algorithms through Scikit-learn with automatic hyper parameter
-searching by FLAML and Ray. + **Traceable**: It integrates MLflow to build
-special storage mechanism to streamline the end-to-end machine learning
-lifecycle. Latest Update: follow up by clicking `Starred` and `Watch` on our
-[GitHub repository](https://github.com/ZJUEarthData/geochemistrypi), then get
-email notifications of the newest features automatically. The following figure
-is the simplified overview of Geochemistry Ï:
+_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_Z_J_U_E_a_r_t_h_D_a_t_a_/_g_e_o_c_h_e_m_i_s_t_r_y_p_i --- # Introduction ## What it is
+Geochemistry Ï is an **open-sourced highly automated machine learning Python
+framework** dedicating to build up MLOps level 1 software product for data-
+driven geochemistry discovery on tabular data. Core capabilities are: +
+**Continous Training** + **Machine Learning Lifecycle Management** + **Model
+Inference** Key features are: + **Easy to use:** The automation of data mining
+process provides the users with simple number options to choose. +
+**Extensible:** It allows appending new algorithms through Scikit-learn with
+automatic hyper parameter searching by FLAML and Ray. + **Traceable**: It
+integrates MLflow to build special storage mechanism to streamline the end-to-
+end machine learning lifecycle. Latest Update: follow up by clicking `Starred`
+and `Watch` on our [GitHub repository](https://github.com/ZJUEarthData/
+geochemistrypi), then get email notifications of the newest features
+automatically. The following figure is the simplified overview of Geochemistry
+Ï:
                             [Overview of workflow]
 The following figure is the frontend-backend separation architecture of
 Geochemistry:
           [Frontend-backend separation architecture of Geochemistry]
-## Quick Installation One instruction to download on **command line**, such as
-Terminal on macOS, Power Shell on Windows. ``` pip install geochemistrypi ```
-One instruction to download on **Jupyter Notebook** or **Google Colab**. ```
-!pip install geochemistrypi ``` Check the latest version of our software: ```
-geochemistrypi --version ``` **Note**: For more detail on installation, please
-refer to our online documentation in **Installation Manual** under the section
-of **FOR USER**. Over there, we highly recommend to use virtual environment
-(Conda) to avoid dependency version problems. ## Quick Update One instruction
-to update the software to the latest version on **command line**, such as
-Terminal on macOS, Power Shell on Windows. ``` pip install --upgrade
-geochemistrypi ``` One instruction to download on **Jupyter Notebook** or
-**Google Colab**. ``` !pip install --upgrade geochemistrypi ``` Check the
-latest version of our software: ``` geochemistrypi --version ``` ## Example
-**How to run:** After successfully downloading, run this instruction on
-**command line / Jupyter Notebook / Google Colab** whatever directory it is.
-### Case 1: Run with built-in data set for testing On command line: ```
-geochemistrypi data-mining ``` On Jupyter Notebook / Google Colab: ```
-!geochemistrypi data-mining ``` **Note**: There are four built-in data sets
-corresponding to four kinds of model pattern. ### Case 2: Run with your own
-data set without model inference On command line: ``` geochemistrypi data-
-mining --data your_own_data_set.xlsx ``` On Jupyter Notebook / Google Colab:
-``` !geochemistrypi data-mining --data your_own_data_set.xlsx ``` **Note**:
+**If the software contributes to your research, cite the work as :** ZhangZhou
+J\*, He Can\*, Sun Jianhao, Zhao Jianming, Lyu Yang, Wang Shengxin, Zhao Wenyu,
+Li Anzhou, Ji Xiaohui. Geochemistry Ï: Automated machine learning python
+framework for tabular data (2024). Geochemistry, Geophysics, Geosystems, 25,
+e2023GC011324 Download link: https://agupubs.onlinelibrary.wiley.com/doi/
+10.1029/2023GC011324 **Related report:** Geochemistry Ï was selected for
+featuringÂ asÂ an EditorâsÂ Highlight in EOS magazine by American Geophysical
+Union (fewer than 2 percent of paper are selected) and quoted in Geochemical
+NEWS by Geochemical Society. Eos Website:Â https://eos.org/editor-highlights/
+machine-learning-for-geochemists-who-dont-want-to-code. ## Quick Installation
+Our software is well tested on **macOS** and **Windows** system with **Python
+3.9**. Other systems and Python version are not guranteed. One instruction to
+download on **command line**, such as Terminal on macOS, Power Shell on
+Windows. ``` pip install geochemistrypi ``` Download the latest version to
+avoid some old version issues, such as dependency downloading. ``` pip install
+"geochemistrypi==0.5.0" ``` One instruction to download on **Jupyter Notebook**
+or **Google Colab**. ``` !pip install geochemistrypi ``` Download the latest
+version to avoid some old version issues, such as dependency downloading. ```
+!pip install "geochemistrypi==0.5.0" ``` Check the downloaded version of our
+software: ``` geochemistrypi --version ``` **Note**: For more detail on
+installation, please refer to our online documentation in **Installation
+Manual** under the section of **FOR USER**. Over there, we highly recommend to
+use virtual environment (Conda) to avoid dependency version problems. ## Quick
+Update One instruction to update the software to the latest version on
+**command line**, such as Terminal on macOS, Power Shell on Windows. ``` pip
+install --upgrade geochemistrypi ``` One instruction to download on **Jupyter
+Notebook** or **Google Colab**. ``` !pip install --upgrade geochemistrypi ```
+Check the updated version of our software: ``` geochemistrypi --version ``` ##
+Data Preparation In order to utilize the functions provided by our software,
+your own data set should satisfy: - be with the suffix **.xlsx** or **.csv**,
+which is supported by Microsoft Excel. - be comprise of location information
+**LATITUDE** and **LONGITUDE**, two columns respectively. It is optional. If
+you want to run **classification** algorithm, you data set should satisfy: - a
+label column. You can name it as you wish, such as **Label**. Column name
+specification: - No restriction on the column names. You can name them as you
+want except for two special and optional column **LATITUDE** and **LONGITUDE**.
+- every column can only one column name. Multi level column names are not
+allowed. - Between two columns with values, a completed void column can exists.
+The following are seven built-in data sets in our software stored on Google
+Drive and Tecent Docs, have a look on them. For the algorithm you intend to
+run, you can refer to the data format of the corresponding dataset. +
+Data_Regression.xlsx [[Google Drive]](https://docs.google.com/spreadsheets/d/
+13MB4t_2PiZ90tTMJKw7HcBUi2sb3tXej/
+edit?usp=sharing&ouid=110717816678586054594&rtpof=true&sd=true) | [[Tencent
+Docs]](https://docs.qq.com/document/
+DQ3VmdWZCTGV3bmpM?&u=6868f96d4a384b309036e04e637e367a) +
+ApplicationData_Regression.xlsx [[Google Drive]](https://docs.google.com/
+spreadsheets/d/1FCek2OOYQD887jfQz21g0ovqVuUJIjVoNI77D-Ufr9Y/edit?usp=sharing) |
+[[Tencent Docs]]( https://docs.qq.com/document/DQ3BDeHhxRGNzSXZN) +
+Data_Classification.xlsx [[Google Drive]](https://docs.google.com/spreadsheets/
+d/1xFBCYVmtZfuEAbeBljUlzqBjxVuLAt8x/
+edit?usp=sharing&ouid=110717816678586054594&rtpof=true&sd=true) | [[Tencent
+Docs]](https://docs.qq.com/document/
+DQ0JUaUFsZnRaZkNG?&u=6868f96d4a384b309036e04e637e367a) +
+ApplicationData_Classification.xlsx [[Google Drive]](https://docs.google.com/
+spreadsheets/d/1J7QvdvbbHJMlKtiumBgKDW7ALghfQQZyKGEoOqhKQjw/edit?usp=sharing) |
+[[Tencent Docs]](https://docs.qq.com/document/DQ2dnQWtubHRBTGtB) +
+Data_Clustering.xlsx [[Google Drive]](https://docs.google.com/spreadsheets/d/
+1sbuJdOzGNQ2Pk-bVURfPYg1rltyBbn5J/
+edit?usp=sharing&ouid=110717816678586054594&rtpof=true&sd=true) | [[Tencent
+Docs]](https://docs.qq.com/document/
+DQ3dKdGtlWkhZS2xR?&u=6868f96d4a384b309036e04e637e367a) +
+Data_Decomposition.xlsx [[Google Drive]](https://docs.google.com/spreadsheets/
+d/1kix82qj5--vhnm8-KhuUBH9dqYH6zcY8/
+edit?usp=sharing&ouid=110717816678586054594&rtpof=true&sd=true) | [[Tencent
+Docs]](https://docs.qq.com/document/
+DQ29oZ0lhUGtZUmdN?&u=6868f96d4a384b309036e04e637e367a) +
+Data_AbnormalDetectioon.xlsx [[Google Drive]](https://docs.google.com/
+spreadsheets/d/1NqTQZCkv74Sn_iOJOKRc-QnJzpaWmnzC_lET_0ZreiQ/edit?usp=sharing) |
+[[Tencent Docs]]( https://docs.qq.com/document/DQ2hqQ2N2ZGlOUWlT) **Note**: For
+more detail on data preparation, please refer to our online documentation in
+**Model Example** under the section of **FOR USER**. ## Running Example **How
+to run:** After successfully downloading, run this instruction on **command
+line / Jupyter Notebook / Google Colab** whatever directory it is. ### Case 1:
+Run with built-in data set for testing On command line: ``` geochemistrypi
+data-mining ``` On Jupyter Notebook / Google Colab: ``` !geochemistrypi data-
+mining ``` **Note**: There are four built-in data sets corresponding to four
+kinds of model pattern. ### Case 2: Run with your own data set without model
+inference On command line: ``` geochemistrypi data-mining --data
+your_own_data_set.xlsx ``` On Jupyter Notebook / Google Colab: ```
+!geochemistrypi data-mining --data your_own_data_set.xlsx ``` **Note**:
 Currently, `.xlsx` and `.csv` files are supported. Please specify the path your
 data file exists. For Google Colab, don't forget to upload your dataset first.
 ### Case 3: Implement model inference on application data On command line: ```
 geochemistrypi data-mining --training your_own_training_data.xlsx --application
 your_own_application_data.xlsx ``` On Jupyter Notebook / Google Colab: ```
 !geochemistrypi data-mining --training your_own_training_data.xlsx --
 application your_own_application_data.xlsx ``` **Note**: Please make sure the
@@ -67,45 +126,46 @@
 ``` On Jupyter Notebook / Google Colab: ``` !geochemistrypi data-mining --
 mlflow ``` **Note**: Once you run our software, there are two folders
 (`geopi_output` and `geopi_tracking`) generated automatically. Make sure the
 directory where you execute using the above command should have the genereted
 file `geopi_tracking`. Copy the URL shown on the console into any browser to
 open the MLflow web interface. The URL is normally like this http://127.0.0.1:
 5000. Search MLflow online to see more operations and usages. For more details:
-Please refer to: + [Manual v1.1.0 for Geochemistry Ï - Beta (International -
-Google drive)](https://drive.google.com/file/d/1yryykCyWKM-
-Sj88fOYbOba6QkB_fu2ws/view?usp=sharing) + [Manual v1.1.0 for Geochemistry Ï -
-Beta (China - Tencent Docs)](https://docs.qq.com/pdf/
-DQ0l5d2xVd2VwcnVW?&u=6868f96d4a384b309036e04e637e367a) + [Geochemistry Ï -
-Download and Run the Beta Version (International - Youtube)](https://
-www.youtube.com/
-watch?v=EeVaJ3H7_AU&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM&index=9) +
-[Geochemistry Ï - Download and Run the Beta Version (China - Bilibili)](https:
-//www.bilibili.com/video/BV1UM4y1Q7Ju/
-?spm_id_from=333.999.0.0&vd_source=27944ab3b73a78970c1a52a5dcbb9140) ## Roadmap
-### First Phase It works as a **software application** with a command-line
-interface (CLI) to automate **data mining** process with frequently-used
-**machine learning algorithms** and **statistical analysis methods**, which
-would further lower the threshold for the geochemists. The highlight is that
-through choosing **simple number options**, the users are able to implement a
-full cycle of data mining **without knowledge of** SciPy, NumPy, Pandas,
-Scikit-learn, FLAML, Ray packages. The following figure is the activity diagram
-of automated ML pipeline in Geochemistry Ï: [https://github.com/ZJUEarthData/
-geochemistrypi/assets/47497750/d7b45a7d-4c6d-472b-9498-c9ccb992212e]Its data
-section provides feature engineering based on **arithmatic operation**. It
-allows the users to have a statistic analysis on the data set as well as on the
-imputation result, which is supported by the combination of **Monte Carlo
-simulation** and **hypothesis testing**. Its models section provides both
-**supervised learning** and **unsupervised learning** methods from **Scikit-
-learn** framework, including four types of algorithms, regression,
-classification, clustering, and dimensional reduction. Integrated with
-**FLAML** and **Ray** framework, it allows the users to run AutoML easily,
-fastly and cost-effectively on the built-in supervised learning algorithms in
-our framework. The following figure is the hierarchical architecture of
-Geochemistry Ï:
+Please refer to: - Manual v1.1.0 for Geochemistry Ï - Beta [[Tencent Docs]]
+(https://docs.qq.com/pdf/DQ0l5d2xVd2VwcnVW?&u=6868f96d4a384b309036e04e637e367a)
+| [[Google drive]](https://drive.google.com/file/d/1yryykCyWKM-
+Sj88fOYbOba6QkB_fu2ws/view?usp=sharing) - Geochemistry Ï - Download and Run
+the Beta Version [[Bilibili]](https://www.bilibili.com/video/BV1UM4y1Q7Ju/
+?spm_id_from=333.999.0.0&vd_source=27944ab3b73a78970c1a52a5dcbb9140) | [
+[YouTube]](https://www.youtube.com/
+watch?v=EeVaJ3H7_AU&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM&index=9) - MLflow
+UI user guide - Geochemistry Ï v0.5.0 [[Bilibili]](https://b23.tv/CW5Rjmo) | [
+[YouTube]](https://www.youtube.com/watch?v=Yu1nzNeLfRY) The following
+screenshot shows the downloads and launching of our software on macOS:
+                      [Downloads and Launching on macOS]
+## Roadmap ### First Phase It works as a **software application** with a
+command-line interface (CLI) to automate **data mining** process with
+frequently-used **machine learning algorithms** and **statistical analysis
+methods**, which would further lower the threshold for the geochemists. The
+highlight is that through choosing **simple number options**, the users are
+able to implement a full cycle of data mining **without knowledge of** SciPy,
+NumPy, Pandas, Scikit-learn, FLAML, Ray packages. The following figure is the
+activity diagram of automated ML pipeline in Geochemistry Ï: [https://
+github.com/ZJUEarthData/geochemistrypi/assets/47497750/d7b45a7d-4c6d-472b-9498-
+c9ccb992212e]Its data section provides feature engineering based on
+**arithmatic operation**. It allows the users to have a statistic analysis on
+the data set as well as on the imputation result, which is supported by the
+combination of **Monte Carlo simulation** and **hypothesis testing**. Its
+models section provides both **supervised learning** and **unsupervised
+learning** methods from **Scikit-learn** framework, including four types of
+algorithms, regression, classification, clustering, and dimensional reduction.
+Integrated with **FLAML** and **Ray** framework, it allows the users to run
+AutoML easily, fastly and cost-effectively on the built-in supervised learning
+algorithms in our framework. The following figure is the hierarchical
+architecture of Geochemistry Ï:
                           [Hierarchical Architecture]
 ### Second Phase Currently, we are building three access ways to provide more
 user-friendly service, including **web portal**, **CLI package** and **API**.
 It allows the user to perform **continuous training** and **model inference**
 by automating the ML pipeline and **machine learning lifecycle management** by
 unique storage mechanism in different access layers. The following figure is
 the system architecture diagram:
@@ -116,29 +176,32 @@
 The following figure is the design pattern hierarchical architecture:
 ![Design Pattern](https://github.com/ZJUEarthData/geochemistrypi/assets/
 47497750/aa84ab12-c95e-4282-a60e-64ba2858c437) ![Workflow Object](https://
 github.com/ZJUEarthData/geochemistrypi/assets/47497750/f08885bf-1bec-4045-bf6b-
 82c5c18d3f8f) The following figure is the storage mechanism:
                               [Storage Mechanism]
 The whole package is under construction and the documentation is progressively
-evolving. ## Team Info **Leader:** + Can He (Sany, National University of
-Singapore, Singapore) Email: sanyhew1097618435@163.com **Technical Group:** +
-Jianming Zhao (Jamie, Zhejiang University, China) + Jianhao Sun (Jin, China
-University of Geosciences, Wuhan, China) + Kaixin Zheng (Hayne, Sun Yat-sen
-University, China) + Jianing Wang (National University of Singapore, Singapore)
-+ Yongkang Chan (Kill-virus, Lanzhou University, China) + Mengying Ye (Mary,
-Jilin University, China) + Mengqi Gao (China University of Geosciences,
+evolving. ## Geochemistry Ï Mind Map [â Click here for more details](https:/
+/docs.qq.com/mind/DZnhoa2NPamFYZHR6?u=40ac0718eb494b008b2f072197ea95db) !
+[Geochemistry Ï.png](https://github.com/ZJUEarthData/geochemistrypi/assets/
+97781484/e77b1f11-41ab-4354-9064-6d62cc1bf1e4) ## Team Info **Leader:** + Can
+He (Sany, National University of Singapore, Singapore) Email:
+sanyhew1097618435@163.com **Technical Group:** + Jianming Zhao (Jamie, Zhejiang
+University, China) + Jianhao Sun (Jin, China University of Geosciences, Wuhan,
+China) + Yongkang Chan (Kill-virus, Lanzhou University, China) + Mengying Ye
+(Mary, Jilin University, China) + Mengqi Gao (China University of Geosciences,
 Beijing, China) + Chengtu Liï¼Trenki, Henan Polytechnic University, Beijing,
-Chinaï¼ **Product Group**: + Yang Lyu (Daisy, Zhejiang University, China) +
-Wenyu Zhao (Molly, Zhejiang University, China) + Keran Li (Kirk, Chengdu
-University of Technology, China) + AixiwakeÂ·Janganuer (Ayshuak, Sun Yat-sen
-University, China) + Bailun Jiang (EPSI / Lille University, France) + Yucheng
-Yan (Andy, University of Sydney, Australia) + Ruitao Chang (China University of
-Geosciences Beijing, China) + Zhenglin Xu (Garry, Jilin University, China) +
-Junchi Liao(Roceda, University of Electronic Science and Technology of China,
+Chinaï¼ + Yucheng Yan (Andy, University of Sydney, Australia) **Product
+Group**: + Yang Lyu (Daisy, Zhejiang University, China) + Bailun Jiang (EPSI /
+Lille University, France) + Ruitao Chang (China University of Geosciences
+Beijing, China) + Junchi Liao(Roceda, University of Electronic Science and
+Technology of China, China) + Panyan Weng (The University of Sydney, Australia)
++ Siqi Yao (Clara, Dongguan University of Technology, China) + Zhelan
+Linï¼Lan, Fuzhou University, Chinaï¼ + ShuYi Li (Communication University Of
+China, Beijing, China) + Junbo Wang (China University Of Geosciences, Beijing,
 China) ## Join Us :) **The recruitment of research interns is ongoing !!!**
 **Key Point: All things are done online, remote work (\*^â½^\*)** **What can
 you learn?** + Learning the full cycle of data mining (Scikit-learn, Ray,
 Mlflow) on tabular data, including the algorithms in regression,classification,
 clustering, and decomposition. + Learning to be a qualified Python developer,
 including any Python programing contents towards data mining, basic software
 engineering techniques like frontend (React, Typescript, Ant Design scaffold)
@@ -194,14 +257,18 @@
 watch?v=KT1g5JpuUVI&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM) 6. [Virtual
 Environment & Packages On Windows - Jianming Zhao (Jamie)](https://
 www.youtube.com/
 watch?v=e4VqSBuNp_o&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM&index=2) 7. [Git
 Workflow & Coordinating Synchronization - Jianming Zhao (Jamie)](https://
 www.bilibili.com/video/
 BV1Sa4y1f74k?spm_id_from=333.999.0.0&vd_source=9adcf2c5fdeffe1d11c89d441ef598ba)
-## Contributors + Shengxin Wang (Samson, Lanzhou University, China) + Qiuhao
-Zhao (Brad, Zhejiang University, China) + Anzhou Li (Andrian, Zhejiang
-University, China) + Dan Hu (Notre Dame University, United States) + Xunxin Liu
-(Tante, China University of Geosciences, Wuhan, China) + Fang Li (liv, Shenzhen
-University, China) + Xin Li (The University of Manchester, United Kingdom) +
-Ting Liu (Kira, Sun Yat-sen University, China) + Xirui Zhu (Rae, University of
-York, United Kingdom)
+## Contributors + Shengxin Wang (Samson, Lanzhou University, China) + Wenyu
+Zhao (Molly, Zhejiang University, China) + Qiuhao Zhao (Brad, Zhejiang
+University, China) + Kaixin Zheng (Hayne, Sun Yat-sen University, China) +
+Anzhou Li (Andrian, Zhejiang University, China) + Keran Li (Kirk, Chengdu
+University of Technology, China) + Dan Hu (Notre Dame University, United
+States) + Xunxin Liu (Tante, China University of Geosciences, Wuhan, China) +
+Fang Li (liv, Shenzhen University, China) + Xin Li (The University of
+Manchester, United Kingdom) + Ting Liu (Kira, Sun Yat-sen University, China) +
+Xirui Zhu (Rae, University of York, United Kingdom) + AixiwakeÂ·Janganuer
+(Ayshuak, Sun Yat-sen University, China) + Zhenglin Xu (Garry, Jilin
+University, China) + Jianing Wang (National University of Singapore, Singapore)
```

### Comparing `geochemistrypi-0.5.0/pyproject.toml` & `geochemistrypi-0.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "geochemistrypi"
-version = "0.5.0"
+version = "0.6.0"
 authors = [
   { name="Can He", email="sanyhew1097618435@163.com" },
 ]
 maintainers = [] 
 description = "A highly automated machine learning Python framework for data-driven geochemistry discovery"
 readme = "README.md"
 license = { file="LICENSE" }
@@ -48,31 +48,20 @@
     "bcrypt",                       # required to run bcrypt
     "python-dotenv",                # required to run python-dotenv
     "rich",                         # color print
     "mlflow",                       # required to run mlflow
     "imblearn",
 ]
 
-[tool.black]
-line-length = "200"
-
-[tool.isort]
-line_length = "200"
-profile = "black"
-
-[tool.flake8]
-max-line-length = "200"
-max-complexity = "20"
-ignore = "F811,W605"
-
 [project.optional-dependencies]
 test = [
     "pytest"
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/ZJUEarthData/geochemistrypi"
+"Homepage" = "https://geochemistrypi.deep-time.org"
+"GitHub" = "https://github.com/ZJUEarthData/geochemistrypi"
 "Bug Tracker" = "https://github.com/ZJUEarthData/geochemistrypi/issues"
 "Online Documentation" = "https://geochemistrypi.readthedocs.io/en/latest/"
 
 [project.scripts]
 geochemistrypi = "geochemistrypi.cli:app"
```

### Comparing `geochemistrypi-0.5.0/PKG-INFO` & `geochemistrypi-0.6.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,75 +1,7 @@
-Metadata-Version: 2.1
-Name: geochemistrypi
-Version: 0.5.0
-Summary: A highly automated machine learning Python framework for data-driven geochemistry discovery
-Project-URL: Homepage, https://github.com/ZJUEarthData/geochemistrypi
-Project-URL: Bug Tracker, https://github.com/ZJUEarthData/geochemistrypi/issues
-Project-URL: Online Documentation, https://geochemistrypi.readthedocs.io/en/latest/
-Author-email: Can He <sanyhew1097618435@163.com>
-License: MIT License
-        
-        Copyright (c) 2021 ZJUEarthData
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: ~=3.9
-Requires-Dist: bcrypt
-Requires-Dist: dash
-Requires-Dist: fastapi
-Requires-Dist: flaml==1.0.14
-Requires-Dist: imblearn
-Requires-Dist: joblib==1.2.0
-Requires-Dist: matplotlib==3.5.2
-Requires-Dist: mlflow
-Requires-Dist: multipledispatch==0.6.0
-Requires-Dist: numpy==1.23.5
-Requires-Dist: openpyxl==3.0.10
-Requires-Dist: optuna
-Requires-Dist: pandas==1.5.2
-Requires-Dist: passlib
-Requires-Dist: pydantic<2.0.0
-Requires-Dist: python-dotenv
-Requires-Dist: python-jose[cryptography]
-Requires-Dist: python-multipart
-Requires-Dist: ray==2.2.0
-Requires-Dist: ray[tune]
-Requires-Dist: rich
-Requires-Dist: scikit-learn==1.1.3
-Requires-Dist: scipy
-Requires-Dist: seaborn==0.11.0
-Requires-Dist: sqlalchemy
-Requires-Dist: statsmodels==0.13.2
-Requires-Dist: threadpoolctl==3.1.0
-Requires-Dist: typer==0.7.0
-Requires-Dist: uvicorn
-Requires-Dist: xgboost==1.6.2
-Provides-Extra: test
-Requires-Dist: pytest; extra == 'test'
-Description-Content-Type: text/markdown
-
 <p>
 <img src="https://github.com/ZJUEarthData/geochemistrypi/assets/47497750/6f970708-7811-40bb-8172-9b98563c7659" class="center"/>
 </p>
 <p align="center">
 <img src="https://img.shields.io/github/actions/workflow/status/ZJUEarthData/geochemistrypi/geochemistrypi.yml?logo=github">
 <img src="https://img.shields.io/github/license/ZJUEarthData/geochemistrypi">
 <img src="https://img.shields.io/github/v/release/ZJUEarthData/geochemistrypi?include_prereleases">
@@ -77,15 +9,15 @@
 <img src="https://img.shields.io/pypi/pyversions/geochemistrypi">
 </p>
 
 ---
 
 **Documentation**: <a href="https://geochemistrypi.readthedocs.io" target="_blank">https://geochemistrypi.readthedocs.io</a>
 
- **Source Code**: <a href="https://github.com/ZJUEarthData/geochemistrypi" target="_blank">https://github.com/ZJUEarthData/geochemistrypi</a>
+**Source Code**: <a href="https://github.com/ZJUEarthData/geochemistrypi" target="_blank">https://github.com/ZJUEarthData/geochemistrypi</a>
 
 ---
 
 Geochemistry π is an **open-sourced highly automated machine learning Python framework** dedicating to build up MLOps level 1 software product for data-driven geochemistry discovery on tabular data.
 
 Core capabilities are:
 
@@ -109,29 +41,53 @@
 
 The following figure is the frontend-backend separation architecture of Geochemistry: <br>
 
 <p align="center">
   <img src="https://github.com/ZJUEarthData/geochemistrypi/assets/47497750/3b27cbdb-ff50-4fa6-b1d1-4c75b253fdff" alt="Frontend-backend separation architecture of Geochemistry" width="450" />
 </p>
 
+
+**If the software contributes to your research, cite the work as :**
+
+ZhangZhou J\*, He Can\*, Sun Jianhao, Zhao Jianming, Lyu Yang, Wang Shengxin, Zhao Wenyu, Li Anzhou, Ji Xiaohui. Geochemistry π: Automated machine learning python framework for tabular data (2024). Geochemistry, Geophysics,
+Geosystems, 25, e2023GC011324
+
+Download link: https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2023GC011324
+
+**Related report:**
+
+Geochemistry π was selected for featuring as an Editor’s Highlight in EOS magazine by American Geophysical Union (fewer than 2 percent of paper are selected) and quoted in Geochemical NEWS by Geochemical Society.
+
+Eos Website: https://eos.org/editor-highlights/machine-learning-for-geochemists-who-dont-want-to-code.
+
 ## Quick Installation
 
+Our software is well tested on **macOS** and **Windows** system with **Python 3.9**. Other systems and Python version are not guranteed.
+
 One instruction to download on **command line**, such as Terminal on macOS, Power Shell on Windows.
 
 ```
 pip install geochemistrypi
 ```
 
+Download the latest version to avoid some old version issues, such as dependency downloading.
+```
+pip install "geochemistrypi==0.5.0"
+```
+
 One instruction to download on **Jupyter Notebook** or **Google Colab**.
 
 ```
 !pip install geochemistrypi
 ```
-
-Check the latest version of our software:
+Download the latest version to avoid some old version issues, such as dependency downloading.
+```
+!pip install "geochemistrypi==0.5.0"
+```
+Check the downloaded version of our software:
 
 ```
 geochemistrypi --version
 ```
 
 **Note**: For more detail on installation, please refer to our online documentation in **Installation Manual** under the section of **FOR USER**. Over there, we highly recommend to use virtual environment (Conda) to avoid dependency version problems.
 
@@ -145,21 +101,60 @@
 
 One instruction to download on **Jupyter Notebook** or **Google Colab**.
 
 ```
 !pip install --upgrade geochemistrypi
 ```
 
-Check the latest version of our software:
+Check the updated version of our software:
 
 ```
 geochemistrypi --version
 ```
 
-## Example
+## Data Preparation
+
+In order to utilize the functions provided by our software, your own data set should satisfy:
+
+- be with the suffix **.xlsx** or **.csv**, which is supported by Microsoft Excel.
+- be comprise of location information **LATITUDE** and **LONGITUDE**, two columns respectively. It is optional.
+
+If you want to run **classification** algorithm, you data set should satisfy:
+
+- a label column. You can name it as you wish, such as **Label**.
+
+Column name specification:
+
+- No restriction on the column names.  You can name them as you want except for two special and optional column **LATITUDE** and **LONGITUDE**.
+
+- every column can only one column name. Multi level column names are not allowed.
+
+- Between two columns with values, a completed void column can exists.
+
+The following are seven built-in data sets in our software stored on Google Drive and Tecent Docs, have a look on them. For the algorithm you intend to run, you can refer to the data format of the corresponding dataset.
+
++ Data_Regression.xlsx [[Google Drive]](https://docs.google.com/spreadsheets/d/13MB4t_2PiZ90tTMJKw7HcBUi2sb3tXej/edit?usp=sharing&ouid=110717816678586054594&rtpof=true&sd=true) | [[Tencent Docs]](https://docs.qq.com/document/DQ3VmdWZCTGV3bmpM?&u=6868f96d4a384b309036e04e637e367a)
+
++ ApplicationData_Regression.xlsx [[Google Drive]](https://docs.google.com/spreadsheets/d/1FCek2OOYQD887jfQz21g0ovqVuUJIjVoNI77D-Ufr9Y/edit?usp=sharing) | [[Tencent Docs]](
+https://docs.qq.com/document/DQ3BDeHhxRGNzSXZN)
+
++ Data_Classification.xlsx [[Google Drive]](https://docs.google.com/spreadsheets/d/1xFBCYVmtZfuEAbeBljUlzqBjxVuLAt8x/edit?usp=sharing&ouid=110717816678586054594&rtpof=true&sd=true) | [[Tencent Docs]](https://docs.qq.com/document/DQ0JUaUFsZnRaZkNG?&u=6868f96d4a384b309036e04e637e367a)
+
++ ApplicationData_Classification.xlsx [[Google Drive]](https://docs.google.com/spreadsheets/d/1J7QvdvbbHJMlKtiumBgKDW7ALghfQQZyKGEoOqhKQjw/edit?usp=sharing) | [[Tencent Docs]](https://docs.qq.com/document/DQ2dnQWtubHRBTGtB)
+
++ Data_Clustering.xlsx [[Google Drive]](https://docs.google.com/spreadsheets/d/1sbuJdOzGNQ2Pk-bVURfPYg1rltyBbn5J/edit?usp=sharing&ouid=110717816678586054594&rtpof=true&sd=true) | [[Tencent Docs]](https://docs.qq.com/document/DQ3dKdGtlWkhZS2xR?&u=6868f96d4a384b309036e04e637e367a)
+
++ Data_Decomposition.xlsx [[Google Drive]](https://docs.google.com/spreadsheets/d/1kix82qj5--vhnm8-KhuUBH9dqYH6zcY8/edit?usp=sharing&ouid=110717816678586054594&rtpof=true&sd=true) | [[Tencent Docs]](https://docs.qq.com/document/DQ29oZ0lhUGtZUmdN?&u=6868f96d4a384b309036e04e637e367a)
+
++  Data_AbnormalDetectioon.xlsx [[Google Drive]](https://docs.google.com/spreadsheets/d/1NqTQZCkv74Sn_iOJOKRc-QnJzpaWmnzC_lET_0ZreiQ/edit?usp=sharing) | [[Tencent Docs]](
+https://docs.qq.com/document/DQ2hqQ2N2ZGlOUWlT)
+
+**Note**: For more detail on data preparation, please refer to our online documentation in **Model Example** under the section of **FOR USER**.
+
+## Running Example
 
 **How to run:** After successfully downloading, run this instruction on **command line / Jupyter Notebook / Google Colab** whatever directory it is.
 
 ### Case 1: Run with built-in data set for testing
 
 On command line:
 
@@ -225,18 +220,23 @@
 
 **Note**: Once you run our software, there are two folders (`geopi_output` and `geopi_tracking`) generated automatically. Make sure the directory where you execute using the above command should have the genereted file `geopi_tracking`.
 
 Copy the URL shown on the console into any browser to open the MLflow web interface. The URL is normally like this http://127.0.0.1:5000. Search MLflow online to see more operations and usages.
 
 For more details: Please refer to:
 
-+ [Manual v1.1.0 for Geochemistry π - Beta (International - Google drive)](https://drive.google.com/file/d/1yryykCyWKM-Sj88fOYbOba6QkB_fu2ws/view?usp=sharing)
-+ [Manual v1.1.0 for Geochemistry π - Beta (China - Tencent Docs)](https://docs.qq.com/pdf/DQ0l5d2xVd2VwcnVW?&u=6868f96d4a384b309036e04e637e367a)
-+ [Geochemistry π - Download and Run the Beta Version (International - Youtube)](https://www.youtube.com/watch?v=EeVaJ3H7_AU&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM&index=9)
-+ [Geochemistry π - Download and Run the Beta Version (China - Bilibili)](https://www.bilibili.com/video/BV1UM4y1Q7Ju/?spm_id_from=333.999.0.0&vd_source=27944ab3b73a78970c1a52a5dcbb9140)
+- Geochemistry π - Download and Run the Beta Version [[Bilibili]](https://www.bilibili.com/video/BV1UM4y1Q7Ju/?spm_id_from=333.999.0.0&vd_source=27944ab3b73a78970c1a52a5dcbb9140) | [[YouTube]](https://www.youtube.com/watch?v=EeVaJ3H7_AU&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM&index=9)
+
+- MLflow UI user guide - Geochemistry π v0.5.0 [[Bilibili]](https://b23.tv/CW5Rjmo) | [[YouTube]](https://www.youtube.com/watch?v=Yu1nzNeLfRY)
+
+The following screenshot shows the downloads and launching of our software on macOS:
+
+<p align="center">
+  <img src="https://github.com/ZJUEarthData/geochemistrypi/assets/47497750/70728795-59b7-4741-ab5b-9e63d284ad37" alt="Downloads and Launching on macOS" width="450" />
+</p>
 
 ## Roadmap
 
 ### First Phase
 
 It works as a **software application** with a command-line interface (CLI) to automate **data mining** process with frequently-used **machine learning algorithms** and **statistical analysis methods**, which would further lower the threshold for the geochemists.
 
@@ -279,43 +279,47 @@
 
 <p align="center">
   <img src="https://github.com/ZJUEarthData/geochemistrypi/assets/47497750/401f3429-c44f-4b76-b085-7a9dcc987cde" alt="Storage Mechanism" width="500" />
 </p>
 
 The whole package is under construction and the documentation is progressively evolving.
 
+## Geochemistry π Mind Map
+
+[→ Click here for more details](https://docs.qq.com/mind/DZnhoa2NPamFYZHR6?u=40ac0718eb494b008b2f072197ea95db)
+
+![Geochemistry π.png](https://github.com/ZJUEarthData/geochemistrypi/assets/97781484/e77b1f11-41ab-4354-9064-6d62cc1bf1e4)
+
 ## Team Info
 
 **Leader:**
 
 + Can He (Sany, National University of Singapore, Singapore)
   Email: sanyhew1097618435@163.com
 
 **Technical Group:**
 
 + Jianming Zhao (Jamie, Zhejiang University, China)
 + Jianhao Sun (Jin, China University of Geosciences, Wuhan, China)
-+ Kaixin Zheng (Hayne, Sun Yat-sen University, China)
-+ Jianing Wang (National University of Singapore, Singapore)
 + Yongkang Chan (Kill-virus, Lanzhou University, China)
 + Mengying Ye (Mary, Jilin University, China)
 + Mengqi Gao (China University of Geosciences, Beijing, China)
 + Chengtu Li（Trenki, Henan Polytechnic University, Beijing, China）
++ Yucheng Yan (Andy, University of Sydney, Australia)
 
 **Product Group**:
 
 + Yang Lyu (Daisy, Zhejiang University, China)
-+ Wenyu Zhao (Molly, Zhejiang University, China)
-+ Keran Li (Kirk, Chengdu University of Technology, China)
-+ Aixiwake·Janganuer (Ayshuak, Sun Yat-sen University, China)
 + Bailun Jiang (EPSI / Lille University, France)
-+ Yucheng Yan (Andy, University of Sydney, Australia)
 + Ruitao Chang (China University of Geosciences Beijing, China)
-+ Zhenglin Xu (Garry, Jilin University, China)
-+ Junchi Liao(Roceda, University of Electronic Science and Technology of China, China)
++ Panyan Weng (The University of Sydney, Australia)
++ Siqi Yao (Clara, Dongguan University of Technology, China)
++ Zhelan Lin（Lan, Fuzhou University, China）
++ ShuYi Li (Communication University Of China, Beijing, China)
++ Junbo Wang (China University Of Geosciences, Beijing, China)
 
 ## Join Us :)
 
 **The recruitment of research interns is ongoing !!!**
 
 **Key Point: All things are done online, remote work (\*^▽^\*)**
 
@@ -372,15 +376,22 @@
 5. [How to use Github-Desktop in conflict resolution - Qiuhao Zhao (Brad)](https://www.youtube.com/watch?v=KT1g5JpuUVI&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM)
 6. [Virtual Environment &amp; Packages On Windows - Jianming Zhao (Jamie)](https://www.youtube.com/watch?v=e4VqSBuNp_o&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM&index=2)
 7. [Git Workflow &amp; Coordinating Synchronization - Jianming Zhao (Jamie)](https://www.bilibili.com/video/BV1Sa4y1f74k?spm_id_from=333.999.0.0&vd_source=9adcf2c5fdeffe1d11c89d441ef598ba)
 
 ## Contributors
 
 + Shengxin Wang (Samson, Lanzhou University, China)
++ Wenyu Zhao (Molly, Zhejiang University, China)
 + Qiuhao Zhao (Brad, Zhejiang University, China)
++ Kaixin Zheng (Hayne, Sun Yat-sen University, China)
 + Anzhou Li (Andrian, Zhejiang University, China)
++ Keran Li (Kirk, Chengdu University of Technology, China)
 + Dan Hu (Notre Dame University, United States)
 + Xunxin Liu (Tante, China University of Geosciences, Wuhan, China)
 + Fang Li (liv, Shenzhen University, China)
 + Xin Li (The University of Manchester, United Kingdom)
 + Ting Liu (Kira, Sun Yat-sen University, China)
 + Xirui Zhu (Rae, University of York, United Kingdom)
++ Aixiwake·Janganuer (Ayshuak, Sun Yat-sen University, China)
++ Zhenglin Xu (Garry, Jilin University, China)
++ Jianing Wang (National University of Singapore, Singapore)
++ Junchi Liao(Roceda, University of Electronic Science and Technology of China, China)
```

#### html2text {}

```diff
@@ -1,43 +1,7 @@
-Metadata-Version: 2.1 Name: geochemistrypi Version: 0.5.0 Summary: A highly
-automated machine learning Python framework for data-driven geochemistry
-discovery Project-URL: Homepage, https://github.com/ZJUEarthData/geochemistrypi
-Project-URL: Bug Tracker, https://github.com/ZJUEarthData/geochemistrypi/issues
-Project-URL: Online Documentation, https://geochemistrypi.readthedocs.io/en/
-latest/ Author-email: Can He
-163.com> License: MIT License Copyright (c) 2021 ZJUEarthData Permission is
-hereby granted, free of charge, to any person obtaining a copy of this software
-and associated documentation files (the "Software"), to deal in the Software
-without restriction, including without limitation the rights to use, copy,
-modify, merge, publish, distribute, sublicense, and/or sell copies of the
-Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions: The above copyright notice and this
-permission notice shall be included in all copies or substantial portions of
-the Software. THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO
-EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES
-OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE. License-File: LICENSE Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.9 Requires-Python: ~=3.9
-Requires-Dist: bcrypt Requires-Dist: dash Requires-Dist: fastapi Requires-Dist:
-flaml==1.0.14 Requires-Dist: imblearn Requires-Dist: joblib==1.2.0 Requires-
-Dist: matplotlib==3.5.2 Requires-Dist: mlflow Requires-Dist:
-multipledispatch==0.6.0 Requires-Dist: numpy==1.23.5 Requires-Dist:
-openpyxl==3.0.10 Requires-Dist: optuna Requires-Dist: pandas==1.5.2 Requires-
-Dist: passlib Requires-Dist: pydantic<2.0.0 Requires-Dist: python-dotenv
-Requires-Dist: python-jose[cryptography] Requires-Dist: python-multipart
-Requires-Dist: ray==2.2.0 Requires-Dist: ray[tune] Requires-Dist: rich
-Requires-Dist: scikit-learn==1.1.3 Requires-Dist: scipy Requires-Dist:
-seaborn==0.11.0 Requires-Dist: sqlalchemy Requires-Dist: statsmodels==0.13.2
-Requires-Dist: threadpoolctl==3.1.0 Requires-Dist: typer==0.7.0 Requires-Dist:
-uvicorn Requires-Dist: xgboost==1.6.2 Provides-Extra: test Requires-Dist:
-pytest; extra == 'test' Description-Content-Type: text/markdown
 [https://github.com/ZJUEarthData/geochemistrypi/assets/47497750/6f970708-7811-
 40bb-8172-9b98563c7659]
      [https://img.shields.io/github/actions/workflow/status/ZJUEarthData/
  geochemistrypi/geochemistrypi.yml?logo=github][https://img.shields.io/github/
  license/ZJUEarthData/geochemistrypi][https://img.shields.io/github/v/release/
   ZJUEarthData/geochemistrypi?include_prereleases][https://static.pepy.tech/
                               personalized-badge/
@@ -58,36 +22,95 @@
 [GitHub repository](https://github.com/ZJUEarthData/geochemistrypi), then get
 email notifications of the newest features automatically. The following figure
 is the simplified overview of Geochemistry Ï:
                             [Overview of workflow]
 The following figure is the frontend-backend separation architecture of
 Geochemistry:
           [Frontend-backend separation architecture of Geochemistry]
-## Quick Installation One instruction to download on **command line**, such as
-Terminal on macOS, Power Shell on Windows. ``` pip install geochemistrypi ```
-One instruction to download on **Jupyter Notebook** or **Google Colab**. ```
-!pip install geochemistrypi ``` Check the latest version of our software: ```
-geochemistrypi --version ``` **Note**: For more detail on installation, please
-refer to our online documentation in **Installation Manual** under the section
-of **FOR USER**. Over there, we highly recommend to use virtual environment
-(Conda) to avoid dependency version problems. ## Quick Update One instruction
-to update the software to the latest version on **command line**, such as
-Terminal on macOS, Power Shell on Windows. ``` pip install --upgrade
-geochemistrypi ``` One instruction to download on **Jupyter Notebook** or
-**Google Colab**. ``` !pip install --upgrade geochemistrypi ``` Check the
-latest version of our software: ``` geochemistrypi --version ``` ## Example
-**How to run:** After successfully downloading, run this instruction on
-**command line / Jupyter Notebook / Google Colab** whatever directory it is.
-### Case 1: Run with built-in data set for testing On command line: ```
-geochemistrypi data-mining ``` On Jupyter Notebook / Google Colab: ```
-!geochemistrypi data-mining ``` **Note**: There are four built-in data sets
-corresponding to four kinds of model pattern. ### Case 2: Run with your own
-data set without model inference On command line: ``` geochemistrypi data-
-mining --data your_own_data_set.xlsx ``` On Jupyter Notebook / Google Colab:
-``` !geochemistrypi data-mining --data your_own_data_set.xlsx ``` **Note**:
+**If the software contributes to your research, cite the work as :** ZhangZhou
+J\*, He Can\*, Sun Jianhao, Zhao Jianming, Lyu Yang, Wang Shengxin, Zhao Wenyu,
+Li Anzhou, Ji Xiaohui. Geochemistry Ï: Automated machine learning python
+framework for tabular data (2024). Geochemistry, Geophysics, Geosystems, 25,
+e2023GC011324 Download link: https://agupubs.onlinelibrary.wiley.com/doi/
+10.1029/2023GC011324 **Related report:** Geochemistry Ï was selected for
+featuringÂ asÂ an EditorâsÂ Highlight in EOS magazine by American Geophysical
+Union (fewer than 2 percent of paper are selected) and quoted in Geochemical
+NEWS by Geochemical Society. Eos Website:Â https://eos.org/editor-highlights/
+machine-learning-for-geochemists-who-dont-want-to-code. ## Quick Installation
+Our software is well tested on **macOS** and **Windows** system with **Python
+3.9**. Other systems and Python version are not guranteed. One instruction to
+download on **command line**, such as Terminal on macOS, Power Shell on
+Windows. ``` pip install geochemistrypi ``` Download the latest version to
+avoid some old version issues, such as dependency downloading. ``` pip install
+"geochemistrypi==0.5.0" ``` One instruction to download on **Jupyter Notebook**
+or **Google Colab**. ``` !pip install geochemistrypi ``` Download the latest
+version to avoid some old version issues, such as dependency downloading. ```
+!pip install "geochemistrypi==0.5.0" ``` Check the downloaded version of our
+software: ``` geochemistrypi --version ``` **Note**: For more detail on
+installation, please refer to our online documentation in **Installation
+Manual** under the section of **FOR USER**. Over there, we highly recommend to
+use virtual environment (Conda) to avoid dependency version problems. ## Quick
+Update One instruction to update the software to the latest version on
+**command line**, such as Terminal on macOS, Power Shell on Windows. ``` pip
+install --upgrade geochemistrypi ``` One instruction to download on **Jupyter
+Notebook** or **Google Colab**. ``` !pip install --upgrade geochemistrypi ```
+Check the updated version of our software: ``` geochemistrypi --version ``` ##
+Data Preparation In order to utilize the functions provided by our software,
+your own data set should satisfy: - be with the suffix **.xlsx** or **.csv**,
+which is supported by Microsoft Excel. - be comprise of location information
+**LATITUDE** and **LONGITUDE**, two columns respectively. It is optional. If
+you want to run **classification** algorithm, you data set should satisfy: - a
+label column. You can name it as you wish, such as **Label**. Column name
+specification: - No restriction on the column names. You can name them as you
+want except for two special and optional column **LATITUDE** and **LONGITUDE**.
+- every column can only one column name. Multi level column names are not
+allowed. - Between two columns with values, a completed void column can exists.
+The following are seven built-in data sets in our software stored on Google
+Drive and Tecent Docs, have a look on them. For the algorithm you intend to
+run, you can refer to the data format of the corresponding dataset. +
+Data_Regression.xlsx [[Google Drive]](https://docs.google.com/spreadsheets/d/
+13MB4t_2PiZ90tTMJKw7HcBUi2sb3tXej/
+edit?usp=sharing&ouid=110717816678586054594&rtpof=true&sd=true) | [[Tencent
+Docs]](https://docs.qq.com/document/
+DQ3VmdWZCTGV3bmpM?&u=6868f96d4a384b309036e04e637e367a) +
+ApplicationData_Regression.xlsx [[Google Drive]](https://docs.google.com/
+spreadsheets/d/1FCek2OOYQD887jfQz21g0ovqVuUJIjVoNI77D-Ufr9Y/edit?usp=sharing) |
+[[Tencent Docs]]( https://docs.qq.com/document/DQ3BDeHhxRGNzSXZN) +
+Data_Classification.xlsx [[Google Drive]](https://docs.google.com/spreadsheets/
+d/1xFBCYVmtZfuEAbeBljUlzqBjxVuLAt8x/
+edit?usp=sharing&ouid=110717816678586054594&rtpof=true&sd=true) | [[Tencent
+Docs]](https://docs.qq.com/document/
+DQ0JUaUFsZnRaZkNG?&u=6868f96d4a384b309036e04e637e367a) +
+ApplicationData_Classification.xlsx [[Google Drive]](https://docs.google.com/
+spreadsheets/d/1J7QvdvbbHJMlKtiumBgKDW7ALghfQQZyKGEoOqhKQjw/edit?usp=sharing) |
+[[Tencent Docs]](https://docs.qq.com/document/DQ2dnQWtubHRBTGtB) +
+Data_Clustering.xlsx [[Google Drive]](https://docs.google.com/spreadsheets/d/
+1sbuJdOzGNQ2Pk-bVURfPYg1rltyBbn5J/
+edit?usp=sharing&ouid=110717816678586054594&rtpof=true&sd=true) | [[Tencent
+Docs]](https://docs.qq.com/document/
+DQ3dKdGtlWkhZS2xR?&u=6868f96d4a384b309036e04e637e367a) +
+Data_Decomposition.xlsx [[Google Drive]](https://docs.google.com/spreadsheets/
+d/1kix82qj5--vhnm8-KhuUBH9dqYH6zcY8/
+edit?usp=sharing&ouid=110717816678586054594&rtpof=true&sd=true) | [[Tencent
+Docs]](https://docs.qq.com/document/
+DQ29oZ0lhUGtZUmdN?&u=6868f96d4a384b309036e04e637e367a) +
+Data_AbnormalDetectioon.xlsx [[Google Drive]](https://docs.google.com/
+spreadsheets/d/1NqTQZCkv74Sn_iOJOKRc-QnJzpaWmnzC_lET_0ZreiQ/edit?usp=sharing) |
+[[Tencent Docs]]( https://docs.qq.com/document/DQ2hqQ2N2ZGlOUWlT) **Note**: For
+more detail on data preparation, please refer to our online documentation in
+**Model Example** under the section of **FOR USER**. ## Running Example **How
+to run:** After successfully downloading, run this instruction on **command
+line / Jupyter Notebook / Google Colab** whatever directory it is. ### Case 1:
+Run with built-in data set for testing On command line: ``` geochemistrypi
+data-mining ``` On Jupyter Notebook / Google Colab: ``` !geochemistrypi data-
+mining ``` **Note**: There are four built-in data sets corresponding to four
+kinds of model pattern. ### Case 2: Run with your own data set without model
+inference On command line: ``` geochemistrypi data-mining --data
+your_own_data_set.xlsx ``` On Jupyter Notebook / Google Colab: ```
+!geochemistrypi data-mining --data your_own_data_set.xlsx ``` **Note**:
 Currently, `.xlsx` and `.csv` files are supported. Please specify the path your
 data file exists. For Google Colab, don't forget to upload your dataset first.
 ### Case 3: Implement model inference on application data On command line: ```
 geochemistrypi data-mining --training your_own_training_data.xlsx --application
 your_own_application_data.xlsx ``` On Jupyter Notebook / Google Colab: ```
 !geochemistrypi data-mining --training your_own_training_data.xlsx --
 application your_own_application_data.xlsx ``` **Note**: Please make sure the
@@ -103,45 +126,43 @@
 ``` On Jupyter Notebook / Google Colab: ``` !geochemistrypi data-mining --
 mlflow ``` **Note**: Once you run our software, there are two folders
 (`geopi_output` and `geopi_tracking`) generated automatically. Make sure the
 directory where you execute using the above command should have the genereted
 file `geopi_tracking`. Copy the URL shown on the console into any browser to
 open the MLflow web interface. The URL is normally like this http://127.0.0.1:
 5000. Search MLflow online to see more operations and usages. For more details:
-Please refer to: + [Manual v1.1.0 for Geochemistry Ï - Beta (International -
-Google drive)](https://drive.google.com/file/d/1yryykCyWKM-
-Sj88fOYbOba6QkB_fu2ws/view?usp=sharing) + [Manual v1.1.0 for Geochemistry Ï -
-Beta (China - Tencent Docs)](https://docs.qq.com/pdf/
-DQ0l5d2xVd2VwcnVW?&u=6868f96d4a384b309036e04e637e367a) + [Geochemistry Ï -
-Download and Run the Beta Version (International - Youtube)](https://
-www.youtube.com/
-watch?v=EeVaJ3H7_AU&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM&index=9) +
-[Geochemistry Ï - Download and Run the Beta Version (China - Bilibili)](https:
-//www.bilibili.com/video/BV1UM4y1Q7Ju/
-?spm_id_from=333.999.0.0&vd_source=27944ab3b73a78970c1a52a5dcbb9140) ## Roadmap
-### First Phase It works as a **software application** with a command-line
-interface (CLI) to automate **data mining** process with frequently-used
-**machine learning algorithms** and **statistical analysis methods**, which
-would further lower the threshold for the geochemists. The highlight is that
-through choosing **simple number options**, the users are able to implement a
-full cycle of data mining **without knowledge of** SciPy, NumPy, Pandas,
-Scikit-learn, FLAML, Ray packages. The following figure is the activity diagram
-of automated ML pipeline in Geochemistry Ï: [https://github.com/ZJUEarthData/
-geochemistrypi/assets/47497750/d7b45a7d-4c6d-472b-9498-c9ccb992212e]Its data
-section provides feature engineering based on **arithmatic operation**. It
-allows the users to have a statistic analysis on the data set as well as on the
-imputation result, which is supported by the combination of **Monte Carlo
-simulation** and **hypothesis testing**. Its models section provides both
-**supervised learning** and **unsupervised learning** methods from **Scikit-
-learn** framework, including four types of algorithms, regression,
-classification, clustering, and dimensional reduction. Integrated with
-**FLAML** and **Ray** framework, it allows the users to run AutoML easily,
-fastly and cost-effectively on the built-in supervised learning algorithms in
-our framework. The following figure is the hierarchical architecture of
-Geochemistry Ï:
+Please refer to: - Geochemistry Ï - Download and Run the Beta Version [
+[Bilibili]](https://www.bilibili.com/video/BV1UM4y1Q7Ju/
+?spm_id_from=333.999.0.0&vd_source=27944ab3b73a78970c1a52a5dcbb9140) | [
+[YouTube]](https://www.youtube.com/
+watch?v=EeVaJ3H7_AU&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM&index=9) - MLflow
+UI user guide - Geochemistry Ï v0.5.0 [[Bilibili]](https://b23.tv/CW5Rjmo) | [
+[YouTube]](https://www.youtube.com/watch?v=Yu1nzNeLfRY) The following
+screenshot shows the downloads and launching of our software on macOS:
+                      [Downloads and Launching on macOS]
+## Roadmap ### First Phase It works as a **software application** with a
+command-line interface (CLI) to automate **data mining** process with
+frequently-used **machine learning algorithms** and **statistical analysis
+methods**, which would further lower the threshold for the geochemists. The
+highlight is that through choosing **simple number options**, the users are
+able to implement a full cycle of data mining **without knowledge of** SciPy,
+NumPy, Pandas, Scikit-learn, FLAML, Ray packages. The following figure is the
+activity diagram of automated ML pipeline in Geochemistry Ï: [https://
+github.com/ZJUEarthData/geochemistrypi/assets/47497750/d7b45a7d-4c6d-472b-9498-
+c9ccb992212e]Its data section provides feature engineering based on
+**arithmatic operation**. It allows the users to have a statistic analysis on
+the data set as well as on the imputation result, which is supported by the
+combination of **Monte Carlo simulation** and **hypothesis testing**. Its
+models section provides both **supervised learning** and **unsupervised
+learning** methods from **Scikit-learn** framework, including four types of
+algorithms, regression, classification, clustering, and dimensional reduction.
+Integrated with **FLAML** and **Ray** framework, it allows the users to run
+AutoML easily, fastly and cost-effectively on the built-in supervised learning
+algorithms in our framework. The following figure is the hierarchical
+architecture of Geochemistry Ï:
                           [Hierarchical Architecture]
 ### Second Phase Currently, we are building three access ways to provide more
 user-friendly service, including **web portal**, **CLI package** and **API**.
 It allows the user to perform **continuous training** and **model inference**
 by automating the ML pipeline and **machine learning lifecycle management** by
 unique storage mechanism in different access layers. The following figure is
 the system architecture diagram:
@@ -152,43 +173,45 @@
 The following figure is the design pattern hierarchical architecture:
 ![Design Pattern](https://github.com/ZJUEarthData/geochemistrypi/assets/
 47497750/aa84ab12-c95e-4282-a60e-64ba2858c437) ![Workflow Object](https://
 github.com/ZJUEarthData/geochemistrypi/assets/47497750/f08885bf-1bec-4045-bf6b-
 82c5c18d3f8f) The following figure is the storage mechanism:
                               [Storage Mechanism]
 The whole package is under construction and the documentation is progressively
-evolving. ## Team Info **Leader:** + Can He (Sany, National University of
-Singapore, Singapore) Email: sanyhew1097618435@163.com **Technical Group:** +
-Jianming Zhao (Jamie, Zhejiang University, China) + Jianhao Sun (Jin, China
-University of Geosciences, Wuhan, China) + Kaixin Zheng (Hayne, Sun Yat-sen
-University, China) + Jianing Wang (National University of Singapore, Singapore)
-+ Yongkang Chan (Kill-virus, Lanzhou University, China) + Mengying Ye (Mary,
-Jilin University, China) + Mengqi Gao (China University of Geosciences,
+evolving. ## Geochemistry Ï Mind Map [â Click here for more details](https:/
+/docs.qq.com/mind/DZnhoa2NPamFYZHR6?u=40ac0718eb494b008b2f072197ea95db) !
+[Geochemistry Ï.png](https://github.com/ZJUEarthData/geochemistrypi/assets/
+97781484/e77b1f11-41ab-4354-9064-6d62cc1bf1e4) ## Team Info **Leader:** + Can
+He (Sany, National University of Singapore, Singapore) Email:
+sanyhew1097618435@163.com **Technical Group:** + Jianming Zhao (Jamie, Zhejiang
+University, China) + Jianhao Sun (Jin, China University of Geosciences, Wuhan,
+China) + Yongkang Chan (Kill-virus, Lanzhou University, China) + Mengying Ye
+(Mary, Jilin University, China) + Mengqi Gao (China University of Geosciences,
 Beijing, China) + Chengtu Liï¼Trenki, Henan Polytechnic University, Beijing,
-Chinaï¼ **Product Group**: + Yang Lyu (Daisy, Zhejiang University, China) +
-Wenyu Zhao (Molly, Zhejiang University, China) + Keran Li (Kirk, Chengdu
-University of Technology, China) + AixiwakeÂ·Janganuer (Ayshuak, Sun Yat-sen
-University, China) + Bailun Jiang (EPSI / Lille University, France) + Yucheng
-Yan (Andy, University of Sydney, Australia) + Ruitao Chang (China University of
-Geosciences Beijing, China) + Zhenglin Xu (Garry, Jilin University, China) +
-Junchi Liao(Roceda, University of Electronic Science and Technology of China,
-China) ## Join Us :) **The recruitment of research interns is ongoing !!!**
-**Key Point: All things are done online, remote work (\*^â½^\*)** **What can
-you learn?** + Learning the full cycle of data mining (Scikit-learn, Ray,
-Mlflow) on tabular data, including the algorithms in regression,classification,
-clustering, and decomposition. + Learning to be a qualified Python developer,
-including any Python programing contents towards data mining, basic software
-engineering techniques like frontend (React, Typescript, Ant Design scaffold)
-and backend (SQL & NoSQL database, RESFful API, FastAPI) development, and
-cooperation tools like Git. **What can you get?** + Research internship proof
-and reference letter after working for >> 100 hours. + Chance to pay a visit to
-Hangzhou, China, sponsored by ZJU Earth Data. + Chance to be guided by the
-experts from IT companies in Silicon Valley and Hangzhou. + Bonus depending on
-your performance. **Current Working Pattern:** + Online working and cooperation
-+ Three weeks per working cycle -> One online meeting per working cycle + One
+Chinaï¼ + Yucheng Yan (Andy, University of Sydney, Australia) **Product
+Group**: + Yang Lyu (Daisy, Zhejiang University, China) + Bailun Jiang (EPSI /
+Lille University, France) + Ruitao Chang (China University of Geosciences
+Beijing, China) + Panyan Weng (The University of Sydney, Australia) + Siqi Yao
+(Clara, Dongguan University of Technology, China) + Zhelan Linï¼Lan, Fuzhou
+University, Chinaï¼ + ShuYi Li (Communication University Of China, Beijing,
+China) + Junbo Wang (China University Of Geosciences, Beijing, China) ## Join
+Us :) **The recruitment of research interns is ongoing !!!** **Key Point: All
+things are done online, remote work (\*^â½^\*)** **What can you learn?** +
+Learning the full cycle of data mining (Scikit-learn, Ray, Mlflow) on tabular
+data, including the algorithms in regression,classification, clustering, and
+decomposition. + Learning to be a qualified Python developer, including any
+Python programing contents towards data mining, basic software engineering
+techniques like frontend (React, Typescript, Ant Design scaffold) and backend
+(SQL & NoSQL database, RESFful API, FastAPI) development, and cooperation tools
+like Git. **What can you get?** + Research internship proof and reference
+letter after working for >> 100 hours. + Chance to pay a visit to Hangzhou,
+China, sponsored by ZJU Earth Data. + Chance to be guided by the experts from
+IT companies in Silicon Valley and Hangzhou. + Bonus depending on your
+performance. **Current Working Pattern:** + Online working and cooperation +
+Three weeks per working cycle -> One online meeting per working cycle + One
 cycle report (see below) per cycle - 5 mins to finish Even if you are not
 familiar with topics above, but if you are interested in and have plenty of
 time to do it. That's enough. We have a full-developed training system to help
 you, as a newbie of data mining or Python developer, learn steps by steps with
 seniors until you can make a significant contribution to our project. **More
 details about the project?** Please refer to: English Page: https://
 person.zju.edu.cn/en/zhangzhou Chinese Page: https://person.zju.edu.cn/
@@ -230,14 +253,20 @@
 watch?v=KT1g5JpuUVI&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM) 6. [Virtual
 Environment & Packages On Windows - Jianming Zhao (Jamie)](https://
 www.youtube.com/
 watch?v=e4VqSBuNp_o&list=PLy8hNsI55lvh1UHjhVhqNUj3xPdV9sEiM&index=2) 7. [Git
 Workflow & Coordinating Synchronization - Jianming Zhao (Jamie)](https://
 www.bilibili.com/video/
 BV1Sa4y1f74k?spm_id_from=333.999.0.0&vd_source=9adcf2c5fdeffe1d11c89d441ef598ba)
-## Contributors + Shengxin Wang (Samson, Lanzhou University, China) + Qiuhao
-Zhao (Brad, Zhejiang University, China) + Anzhou Li (Andrian, Zhejiang
-University, China) + Dan Hu (Notre Dame University, United States) + Xunxin Liu
-(Tante, China University of Geosciences, Wuhan, China) + Fang Li (liv, Shenzhen
-University, China) + Xin Li (The University of Manchester, United Kingdom) +
-Ting Liu (Kira, Sun Yat-sen University, China) + Xirui Zhu (Rae, University of
-York, United Kingdom)
+## Contributors + Shengxin Wang (Samson, Lanzhou University, China) + Wenyu
+Zhao (Molly, Zhejiang University, China) + Qiuhao Zhao (Brad, Zhejiang
+University, China) + Kaixin Zheng (Hayne, Sun Yat-sen University, China) +
+Anzhou Li (Andrian, Zhejiang University, China) + Keran Li (Kirk, Chengdu
+University of Technology, China) + Dan Hu (Notre Dame University, United
+States) + Xunxin Liu (Tante, China University of Geosciences, Wuhan, China) +
+Fang Li (liv, Shenzhen University, China) + Xin Li (The University of
+Manchester, United Kingdom) + Ting Liu (Kira, Sun Yat-sen University, China) +
+Xirui Zhu (Rae, University of York, United Kingdom) + AixiwakeÂ·Janganuer
+(Ayshuak, Sun Yat-sen University, China) + Zhenglin Xu (Garry, Jilin
+University, China) + Jianing Wang (National University of Singapore, Singapore)
++ Junchi Liao(Roceda, University of Electronic Science and Technology of China,
+China)
```


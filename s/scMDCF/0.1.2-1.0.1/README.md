# Comparing `tmp/scMDCF-0.1.2.tar.gz` & `tmp/scMDCF-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scMDCF-0.1.2.tar", last modified: Tue Feb 27 07:37:00 2024, max compression
+gzip compressed data, was "scMDCF-1.0.1.tar", last modified: Mon Apr 22 02:40:06 2024, max compression
```

## Comparing `scMDCF-0.1.2.tar` & `scMDCF-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 chengyue  (2018) chengyue  (2018)        0 2024-02-27 07:37:00.209613 scMDCF-0.1.2/
--rw-r--r--   0 chengyue  (2018) chengyue  (2018)     6363 2024-02-27 07:37:00.209613 scMDCF-0.1.2/PKG-INFO
--rw-rw-r--   0 chengyue  (2018) chengyue  (2018)     3833 2024-02-27 07:35:42.000000 scMDCF-0.1.2/README.md
-drwxrwxr-x   0 chengyue  (2018) chengyue  (2018)        0 2024-02-27 07:37:00.209613 scMDCF-0.1.2/scMDCF/
--rw-rw-r--   0 chengyue  (2018) chengyue  (2018)       13 2024-02-25 11:21:49.000000 scMDCF-0.1.2/scMDCF/__init__.py
--rw-rw-r--   0 chengyue  (2018) chengyue  (2018)     4293 2024-02-27 07:09:47.000000 scMDCF-0.1.2/scMDCF/layer.py
--rw-rw-r--   0 chengyue  (2018) chengyue  (2018)     2875 2024-02-27 06:48:17.000000 scMDCF-0.1.2/scMDCF/train.py
--rw-rw-r--   0 chengyue  (2018) chengyue  (2018)     5062 2024-02-27 06:54:50.000000 scMDCF-0.1.2/scMDCF/utils.py
-drwxrwxr-x   0 chengyue  (2018) chengyue  (2018)        0 2024-02-27 07:37:00.209613 scMDCF-0.1.2/scMDCF.egg-info/
--rw-r--r--   0 chengyue  (2018) chengyue  (2018)     6363 2024-02-27 07:37:00.000000 scMDCF-0.1.2/scMDCF.egg-info/PKG-INFO
--rw-rw-r--   0 chengyue  (2018) chengyue  (2018)      234 2024-02-27 07:37:00.000000 scMDCF-0.1.2/scMDCF.egg-info/SOURCES.txt
--rw-rw-r--   0 chengyue  (2018) chengyue  (2018)        1 2024-02-27 07:37:00.000000 scMDCF-0.1.2/scMDCF.egg-info/dependency_links.txt
--rw-rw-r--   0 chengyue  (2018) chengyue  (2018)     1172 2024-02-27 07:37:00.000000 scMDCF-0.1.2/scMDCF.egg-info/requires.txt
--rw-rw-r--   0 chengyue  (2018) chengyue  (2018)        7 2024-02-27 07:37:00.000000 scMDCF-0.1.2/scMDCF.egg-info/top_level.txt
--rw-rw-r--   0 chengyue  (2018) chengyue  (2018)       38 2024-02-27 07:37:00.209613 scMDCF-0.1.2/setup.cfg
--rw-rw-r--   0 chengyue  (2018) chengyue  (2018)     3274 2024-02-27 07:35:47.000000 scMDCF-0.1.2/setup.py
+drwxrwxr-x   0 chengyue (20222007) chengyue (20222007)        0 2024-04-22 02:40:06.001649 scMDCF-1.0.1/
+-rw-rw-r--   0 chengyue (20222007) chengyue (20222007)     1064 2024-04-22 02:34:44.000000 scMDCF-1.0.1/LICENSE
+-rw-r--r--   0 chengyue (20222007) chengyue (20222007)     6450 2024-04-22 02:40:06.001649 scMDCF-1.0.1/PKG-INFO
+-rw-rw-r--   0 chengyue (20222007) chengyue (20222007)     3888 2024-04-22 02:38:34.000000 scMDCF-1.0.1/README.md
+drwxrwxr-x   0 chengyue (20222007) chengyue (20222007)        0 2024-04-22 02:40:06.001649 scMDCF-1.0.1/scMDCF/
+-rw-rw-r--   0 chengyue (20222007) chengyue (20222007)       13 2024-04-22 02:34:44.000000 scMDCF-1.0.1/scMDCF/__init__.py
+-rw-rw-r--   0 chengyue (20222007) chengyue (20222007)     4293 2024-04-22 02:34:44.000000 scMDCF-1.0.1/scMDCF/layer.py
+-rw-rw-r--   0 chengyue (20222007) chengyue (20222007)     2875 2024-04-22 02:34:44.000000 scMDCF-1.0.1/scMDCF/train.py
+-rw-rw-r--   0 chengyue (20222007) chengyue (20222007)     4940 2024-04-22 02:36:22.000000 scMDCF-1.0.1/scMDCF/utils.py
+drwxrwxr-x   0 chengyue (20222007) chengyue (20222007)        0 2024-04-22 02:40:06.001649 scMDCF-1.0.1/scMDCF.egg-info/
+-rw-r--r--   0 chengyue (20222007) chengyue (20222007)     6450 2024-04-22 02:40:05.000000 scMDCF-1.0.1/scMDCF.egg-info/PKG-INFO
+-rw-rw-r--   0 chengyue (20222007) chengyue (20222007)      242 2024-04-22 02:40:05.000000 scMDCF-1.0.1/scMDCF.egg-info/SOURCES.txt
+-rw-rw-r--   0 chengyue (20222007) chengyue (20222007)        1 2024-04-22 02:40:05.000000 scMDCF-1.0.1/scMDCF.egg-info/dependency_links.txt
+-rw-rw-r--   0 chengyue (20222007) chengyue (20222007)     1172 2024-04-22 02:40:05.000000 scMDCF-1.0.1/scMDCF.egg-info/requires.txt
+-rw-rw-r--   0 chengyue (20222007) chengyue (20222007)        7 2024-04-22 02:40:05.000000 scMDCF-1.0.1/scMDCF.egg-info/top_level.txt
+-rw-rw-r--   0 chengyue (20222007) chengyue (20222007)       38 2024-04-22 02:40:06.001649 scMDCF-1.0.1/setup.cfg
+-rw-rw-r--   0 chengyue (20222007) chengyue (20222007)     3285 2024-04-22 02:38:32.000000 scMDCF-1.0.1/setup.py
```

### Comparing `scMDCF-0.1.2/PKG-INFO` & `scMDCF-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: scMDCF
-Version: 0.1.2
-Summary: Integrative and Cross-Modality Analysis of Single-Cell Data Across Multiomic Profiles Using scMDCF
+Version: 1.0.1
+Summary: Unified Cross-modality Integration and Inference of Single-Cell Multiomic Data with Deep Contrastive Learning
 Home-page: https://github.com/DARKpmm/scMDCF
 Author: Yue Cheng
 Author-email: chengyue22@mails.jlu.edu.cn
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: anndata==0.10.5.post1
 Requires-Dist: array_api_compat==1.4.1
 Requires-Dist: contourpy==1.2.0
 Requires-Dist: cycler==0.12.1
 Requires-Dist: exceptiongroup==1.2.0
 Requires-Dist: filelock==3.13.1
 Requires-Dist: fonttools==4.49.0
@@ -81,15 +82,15 @@
 - [System Requirements](#system-requirements)
 - [Installation Guide](#installation-guide)
 - [Usage](#usage)
 - [Data Availability](#data-availability)
 - [License](#license)
 
 # Overview
-Single-cell multi-omics (scMulti-omics) technologies enable simultaneous measurements of diverse modalities within individual cells and have the potential to comprehensively unravel cellular functions and interactions. Despite this promise, the complexity, high-dimensionality, and heterogeneity of the datasets pose significant challenges to integrative analysis. Here, we develop a single-cell multi-omics deep learning model (scMDCF) based on contrastive learning that is designed to efficiently characterize different types of omics data and capture potential features in the data through deep embedding for a complete and integrated analysis. In scMDCF, we propose a cross-modality contrastive learning module to unify representations from various omics types to ensure consistency, while the cross-modality feature fusion module utilizes conditional entropy to preserve the heterogeneity information. Extensive empirical studies have confirmed that scMDCF outperforms other state-of-the-art scMulti-omics models across various types of scMulti-omics data. In particular, scMDCF demonstrates advanced capability in determining the vital cell-type specific peak-gene associations and cis-regulatory elements from SNARE-seq data as well as surmizing immune regulation within cellular differentiation pathways from CITE-seq data. In addition, we demonstrate that in the post-SARS-CoV-2 vaccination dataset, scMDCF successfully provides annotations on the specific vaccine-induced B cell subpopulations in each modality and reveals the dynamic interactions and regulatory mechanisms within the post-vaccination immune system after vaccination.
+Single-cell multi-omics (scMulti-omics) technologies have revolutionized our understanding of cellular functions and interactions by enabling the simultaneous measurement of diverse cellular modalities. However, the inherent complexity, high-dimensionality, and heterogeneity of these datasets pose substantial challenges for integration and analysis across different modalities. To address these challenges, we develop a single-cell multi-omics deep learning model (scMDCF) based on contrastive learning, tailored for the efficient characterization and integration of scMulti-omics data. scMDCF features a cross-modality contrastive learning module that harmonizes data representations across different omics types, ensuring consistency while accommodating conditional entropy to preserve data heterogeneity. Furthermore, a cross-modality feature fusion module is designed to extract common low-dimensional latent representations of scMulti-omics data, effectively balancing the characteristics of these diverse omics data. Extensive empirical studies demonstrate that scMDCF outperforms existing state-of-the-art scMulti-omics models across various types of scMulti-omics data. In particular, scMDCF exhibits progressive capability in extracting cell-type specific peak-gene associations and cis-regulatory elements from SNARE-seq data, as well as in elucidating immune regulation from CITE-seq data. Furthermore, we demonstrate that in the COVID-19 post-BNT162b2 mRNA vaccination dataset, scMDCF successfully annotates specific vaccine-induced B cell subpopulations across multiple modalities, uncovering dynamic interactions and regulatory mechanisms within the immune system after vaccination.
 ![The framework plot of scMDCF](https://github.com/DARKpmm/scMDCF/raw/main/scMDCF.png)
 
 # System Requirements
 ## Hardware requirements
 `scMDCF` package requires only a standard computer with enough RAM to support the in-memory operations.
 
 ## Software requirements
@@ -106,15 +107,15 @@
     scikit-learn
 For specific setting, please see <a href="https://github.com/DARKpmm/scMDCF/blob/main/requirements.txt">requirements</a>.
 
 # Installation Guide
 ## Install from PyPi
     conda create -n scMDCF_env python=3.9.16
     conda activate scMDCF_env
-    pip install scMDCF==0.1.2
+    pip install scMDCF==0.1.1
 
 # Usage
 `scMDCF` is a deep embedding learning method for single-cell multi-omics data clustering, which can be used to:
 * CITE-seq dataset clustering. The example can be seen in the <a href="https://github.com/DARKpmm/scMDCF/tree/main/tutorial/main_CITE.py">main_CITE.py</a>
 * SNARE-seq (paired RNA-seq and ATAC-seq) dataset clustering. The example can be seen in the <a href="https://github.com/DARKpmm/scMDCF/tree/main/tutorial/main_SNARE.py">main_SNARE.py</a>
 
 # Data Availability
```

### Comparing `scMDCF-0.1.2/README.md` & `scMDCF-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 - [System Requirements](#system-requirements)
 - [Installation Guide](#installation-guide)
 - [Usage](#usage)
 - [Data Availability](#data-availability)
 - [License](#license)
 
 # Overview
-Single-cell multi-omics (scMulti-omics) technologies enable simultaneous measurements of diverse modalities within individual cells and have the potential to comprehensively unravel cellular functions and interactions. Despite this promise, the complexity, high-dimensionality, and heterogeneity of the datasets pose significant challenges to integrative analysis. Here, we develop a single-cell multi-omics deep learning model (scMDCF) based on contrastive learning that is designed to efficiently characterize different types of omics data and capture potential features in the data through deep embedding for a complete and integrated analysis. In scMDCF, we propose a cross-modality contrastive learning module to unify representations from various omics types to ensure consistency, while the cross-modality feature fusion module utilizes conditional entropy to preserve the heterogeneity information. Extensive empirical studies have confirmed that scMDCF outperforms other state-of-the-art scMulti-omics models across various types of scMulti-omics data. In particular, scMDCF demonstrates advanced capability in determining the vital cell-type specific peak-gene associations and cis-regulatory elements from SNARE-seq data as well as surmizing immune regulation within cellular differentiation pathways from CITE-seq data. In addition, we demonstrate that in the post-SARS-CoV-2 vaccination dataset, scMDCF successfully provides annotations on the specific vaccine-induced B cell subpopulations in each modality and reveals the dynamic interactions and regulatory mechanisms within the post-vaccination immune system after vaccination.
+Single-cell multi-omics (scMulti-omics) technologies have revolutionized our understanding of cellular functions and interactions by enabling the simultaneous measurement of diverse cellular modalities. However, the inherent complexity, high-dimensionality, and heterogeneity of these datasets pose substantial challenges for integration and analysis across different modalities. To address these challenges, we develop a single-cell multi-omics deep learning model (scMDCF) based on contrastive learning, tailored for the efficient characterization and integration of scMulti-omics data. scMDCF features a cross-modality contrastive learning module that harmonizes data representations across different omics types, ensuring consistency while accommodating conditional entropy to preserve data heterogeneity. Furthermore, a cross-modality feature fusion module is designed to extract common low-dimensional latent representations of scMulti-omics data, effectively balancing the characteristics of these diverse omics data. Extensive empirical studies demonstrate that scMDCF outperforms existing state-of-the-art scMulti-omics models across various types of scMulti-omics data. In particular, scMDCF exhibits progressive capability in extracting cell-type specific peak-gene associations and cis-regulatory elements from SNARE-seq data, as well as in elucidating immune regulation from CITE-seq data. Furthermore, we demonstrate that in the COVID-19 post-BNT162b2 mRNA vaccination dataset, scMDCF successfully annotates specific vaccine-induced B cell subpopulations across multiple modalities, uncovering dynamic interactions and regulatory mechanisms within the immune system after vaccination.
 ![The framework plot of scMDCF](https://github.com/DARKpmm/scMDCF/raw/main/scMDCF.png)
 
 # System Requirements
 ## Hardware requirements
 `scMDCF` package requires only a standard computer with enough RAM to support the in-memory operations.
 
 ## Software requirements
@@ -35,19 +35,19 @@
     scikit-learn
 For specific setting, please see <a href="https://github.com/DARKpmm/scMDCF/blob/main/requirements.txt">requirements</a>.
 
 # Installation Guide
 ## Install from PyPi
     conda create -n scMDCF_env python=3.9.16
     conda activate scMDCF_env
-    pip install scMDCF==0.1.2
+    pip install scMDCF==0.1.1
 
 # Usage
 `scMDCF` is a deep embedding learning method for single-cell multi-omics data clustering, which can be used to:
 * CITE-seq dataset clustering. The example can be seen in the <a href="https://github.com/DARKpmm/scMDCF/tree/main/tutorial/main_CITE.py">main_CITE.py</a>
 * SNARE-seq (paired RNA-seq and ATAC-seq) dataset clustering. The example can be seen in the <a href="https://github.com/DARKpmm/scMDCF/tree/main/tutorial/main_SNARE.py">main_SNARE.py</a>
 
 # Data Availability
 The datasets we used can be download in <a href="https://github.com/DARKpmm/scMDCF/tree/main/dataset">dataset</a>
 
 # License
-This project is covered under the **MIT License**.
+This project is covered under the **MIT License**.
```

#### html2text {}

```diff
@@ -4,44 +4,44 @@
 img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/
 MIT) `scMDCF` is a python package containing tools for clustering single cell
 multi-omics data based on cross-modality contrastive learning to learn the
 common latent representation and assign clustering. - [Overview](#overview) -
 [System Requirements](#system-requirements) - [Installation Guide]
 (#installation-guide) - [Usage](#usage) - [Data Availability](#data-
 availability) - [License](#license) # Overview Single-cell multi-omics
-(scMulti-omics) technologies enable simultaneous measurements of diverse
-modalities within individual cells and have the potential to comprehensively
-unravel cellular functions and interactions. Despite this promise, the
-complexity, high-dimensionality, and heterogeneity of the datasets pose
-significant challenges to integrative analysis. Here, we develop a single-cell
-multi-omics deep learning model (scMDCF) based on contrastive learning that is
-designed to efficiently characterize different types of omics data and capture
-potential features in the data through deep embedding for a complete and
-integrated analysis. In scMDCF, we propose a cross-modality contrastive
-learning module to unify representations from various omics types to ensure
-consistency, while the cross-modality feature fusion module utilizes
-conditional entropy to preserve the heterogeneity information. Extensive
-empirical studies have confirmed that scMDCF outperforms other state-of-the-art
-scMulti-omics models across various types of scMulti-omics data. In particular,
-scMDCF demonstrates advanced capability in determining the vital cell-type
-specific peak-gene associations and cis-regulatory elements from SNARE-seq data
-as well as surmizing immune regulation within cellular differentiation pathways
-from CITE-seq data. In addition, we demonstrate that in the post-SARS-CoV-
-2 vaccination dataset, scMDCF successfully provides annotations on the specific
-vaccine-induced B cell subpopulations in each modality and reveals the dynamic
-interactions and regulatory mechanisms within the post-vaccination immune
-system after vaccination. ![The framework plot of scMDCF](https://github.com/
-DARKpmm/scMDCF/raw/main/scMDCF.png) # System Requirements ## Hardware
-requirements `scMDCF` package requires only a standard computer with enough RAM
-to support the in-memory operations. ## Software requirements ### OS
-requirements This package is supported for *Linux*. The package has been tested
-on the following systems: * Linux: Ubuntu 18.04 ### Python Dependencies
-`scMDCF` mainly depends on the Python scientific stack. numpy pytorch scanpy
-pandas scikit-learn For specific setting, please see _r_e_q_u_i_r_e_m_e_n_t_s. #
-Installation Guide ## Install from PyPi conda create -n scMDCF_env
-python=3.9.16 conda activate scMDCF_env pip install scMDCF==0.1.2 # Usage
-`scMDCF` is a deep embedding learning method for single-cell multi-omics data
-clustering, which can be used to: * CITE-seq dataset clustering. The example
-can be seen in the _m_a_i_n___C_I_T_E_._p_y * SNARE-seq (paired RNA-seq and ATAC-seq)
-dataset clustering. The example can be seen in the _m_a_i_n___S_N_A_R_E_._p_y # Data
-Availability The datasets we used can be download in _d_a_t_a_s_e_t # License This
-project is covered under the **MIT License**.
+(scMulti-omics) technologies have revolutionized our understanding of cellular
+functions and interactions by enabling the simultaneous measurement of diverse
+cellular modalities. However, the inherent complexity, high-dimensionality, and
+heterogeneity of these datasets pose substantial challenges for integration and
+analysis across different modalities. To address these challenges, we develop a
+single-cell multi-omics deep learning model (scMDCF) based on contrastive
+learning, tailored for the efficient characterization and integration of
+scMulti-omics data. scMDCF features a cross-modality contrastive learning
+module that harmonizes data representations across different omics types,
+ensuring consistency while accommodating conditional entropy to preserve data
+heterogeneity. Furthermore, a cross-modality feature fusion module is designed
+to extract common low-dimensional latent representations of scMulti-omics data,
+effectively balancing the characteristics of these diverse omics data.
+Extensive empirical studies demonstrate that scMDCF outperforms existing state-
+of-the-art scMulti-omics models across various types of scMulti-omics data. In
+particular, scMDCF exhibits progressive capability in extracting cell-type
+specific peak-gene associations and cis-regulatory elements from SNARE-seq
+data, as well as in elucidating immune regulation from CITE-seq data.
+Furthermore, we demonstrate that in the COVID-19 post-BNT162b2 mRNA vaccination
+dataset, scMDCF successfully annotates specific vaccine-induced B cell
+subpopulations across multiple modalities, uncovering dynamic interactions and
+regulatory mechanisms within the immune system after vaccination. ![The
+framework plot of scMDCF](https://github.com/DARKpmm/scMDCF/raw/main/
+scMDCF.png) # System Requirements ## Hardware requirements `scMDCF` package
+requires only a standard computer with enough RAM to support the in-memory
+operations. ## Software requirements ### OS requirements This package is
+supported for *Linux*. The package has been tested on the following systems: *
+Linux: Ubuntu 18.04 ### Python Dependencies `scMDCF` mainly depends on the
+Python scientific stack. numpy pytorch scanpy pandas scikit-learn For specific
+setting, please see _r_e_q_u_i_r_e_m_e_n_t_s. # Installation Guide ## Install from PyPi
+conda create -n scMDCF_env python=3.9.16 conda activate scMDCF_env pip install
+scMDCF==0.1.1 # Usage `scMDCF` is a deep embedding learning method for single-
+cell multi-omics data clustering, which can be used to: * CITE-seq dataset
+clustering. The example can be seen in the _m_a_i_n___C_I_T_E_._p_y * SNARE-seq (paired
+RNA-seq and ATAC-seq) dataset clustering. The example can be seen in the
+_m_a_i_n___S_N_A_R_E_._p_y # Data Availability The datasets we used can be download in
+_d_a_t_a_s_e_t # License This project is covered under the **MIT License**.
```

### Comparing `scMDCF-0.1.2/scMDCF/layer.py` & `scMDCF-1.0.1/scMDCF/layer.py`

 * *Files identical despite different names*

### Comparing `scMDCF-0.1.2/scMDCF/train.py` & `scMDCF-1.0.1/scMDCF/train.py`

 * *Files identical despite different names*

### Comparing `scMDCF-0.1.2/scMDCF/utils.py` & `scMDCF-1.0.1/scMDCF/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,14 @@
         adata_ATAC = sc.AnnData(atac_X)
     elif file_type=='h5':
         data_mat = h5py.File(file_path1)#SMAGESeq; pbmc_spector 49; GSE128639_BMNC; spleen_lymph 112; 
         rna_X = np.array(data_mat['X1'])
         atac_X = np.array(data_mat['X1'])
         y = np.array(data_mat['Y'])
         data_mat.close()
-        cell_name = pd.read_csv(label_file, header=None)
-        cell_type, y = np.unique(cell_name, return_inverse=True)
         cluster_number = int(max(y) - min(y) + 1) 
         adata_RNA = sc.AnnData(rna_X)
         adata_ATAC = sc.AnnData(atac_X)
     elif file_type=='loom':
         adata_RNA=sc.read_loom(file_path1)
         adata_ATAC=sc.read_loom(file_path2)
         cell_name = pd.read_csv(label_file, usecols=[1])
```

### Comparing `scMDCF-0.1.2/scMDCF.egg-info/PKG-INFO` & `scMDCF-1.0.1/scMDCF.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: scMDCF
-Version: 0.1.2
-Summary: Integrative and Cross-Modality Analysis of Single-Cell Data Across Multiomic Profiles Using scMDCF
+Version: 1.0.1
+Summary: Unified Cross-modality Integration and Inference of Single-Cell Multiomic Data with Deep Contrastive Learning
 Home-page: https://github.com/DARKpmm/scMDCF
 Author: Yue Cheng
 Author-email: chengyue22@mails.jlu.edu.cn
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: anndata==0.10.5.post1
 Requires-Dist: array_api_compat==1.4.1
 Requires-Dist: contourpy==1.2.0
 Requires-Dist: cycler==0.12.1
 Requires-Dist: exceptiongroup==1.2.0
 Requires-Dist: filelock==3.13.1
 Requires-Dist: fonttools==4.49.0
@@ -81,15 +82,15 @@
 - [System Requirements](#system-requirements)
 - [Installation Guide](#installation-guide)
 - [Usage](#usage)
 - [Data Availability](#data-availability)
 - [License](#license)
 
 # Overview
-Single-cell multi-omics (scMulti-omics) technologies enable simultaneous measurements of diverse modalities within individual cells and have the potential to comprehensively unravel cellular functions and interactions. Despite this promise, the complexity, high-dimensionality, and heterogeneity of the datasets pose significant challenges to integrative analysis. Here, we develop a single-cell multi-omics deep learning model (scMDCF) based on contrastive learning that is designed to efficiently characterize different types of omics data and capture potential features in the data through deep embedding for a complete and integrated analysis. In scMDCF, we propose a cross-modality contrastive learning module to unify representations from various omics types to ensure consistency, while the cross-modality feature fusion module utilizes conditional entropy to preserve the heterogeneity information. Extensive empirical studies have confirmed that scMDCF outperforms other state-of-the-art scMulti-omics models across various types of scMulti-omics data. In particular, scMDCF demonstrates advanced capability in determining the vital cell-type specific peak-gene associations and cis-regulatory elements from SNARE-seq data as well as surmizing immune regulation within cellular differentiation pathways from CITE-seq data. In addition, we demonstrate that in the post-SARS-CoV-2 vaccination dataset, scMDCF successfully provides annotations on the specific vaccine-induced B cell subpopulations in each modality and reveals the dynamic interactions and regulatory mechanisms within the post-vaccination immune system after vaccination.
+Single-cell multi-omics (scMulti-omics) technologies have revolutionized our understanding of cellular functions and interactions by enabling the simultaneous measurement of diverse cellular modalities. However, the inherent complexity, high-dimensionality, and heterogeneity of these datasets pose substantial challenges for integration and analysis across different modalities. To address these challenges, we develop a single-cell multi-omics deep learning model (scMDCF) based on contrastive learning, tailored for the efficient characterization and integration of scMulti-omics data. scMDCF features a cross-modality contrastive learning module that harmonizes data representations across different omics types, ensuring consistency while accommodating conditional entropy to preserve data heterogeneity. Furthermore, a cross-modality feature fusion module is designed to extract common low-dimensional latent representations of scMulti-omics data, effectively balancing the characteristics of these diverse omics data. Extensive empirical studies demonstrate that scMDCF outperforms existing state-of-the-art scMulti-omics models across various types of scMulti-omics data. In particular, scMDCF exhibits progressive capability in extracting cell-type specific peak-gene associations and cis-regulatory elements from SNARE-seq data, as well as in elucidating immune regulation from CITE-seq data. Furthermore, we demonstrate that in the COVID-19 post-BNT162b2 mRNA vaccination dataset, scMDCF successfully annotates specific vaccine-induced B cell subpopulations across multiple modalities, uncovering dynamic interactions and regulatory mechanisms within the immune system after vaccination.
 ![The framework plot of scMDCF](https://github.com/DARKpmm/scMDCF/raw/main/scMDCF.png)
 
 # System Requirements
 ## Hardware requirements
 `scMDCF` package requires only a standard computer with enough RAM to support the in-memory operations.
 
 ## Software requirements
@@ -106,15 +107,15 @@
     scikit-learn
 For specific setting, please see <a href="https://github.com/DARKpmm/scMDCF/blob/main/requirements.txt">requirements</a>.
 
 # Installation Guide
 ## Install from PyPi
     conda create -n scMDCF_env python=3.9.16
     conda activate scMDCF_env
-    pip install scMDCF==0.1.2
+    pip install scMDCF==0.1.1
 
 # Usage
 `scMDCF` is a deep embedding learning method for single-cell multi-omics data clustering, which can be used to:
 * CITE-seq dataset clustering. The example can be seen in the <a href="https://github.com/DARKpmm/scMDCF/tree/main/tutorial/main_CITE.py">main_CITE.py</a>
 * SNARE-seq (paired RNA-seq and ATAC-seq) dataset clustering. The example can be seen in the <a href="https://github.com/DARKpmm/scMDCF/tree/main/tutorial/main_SNARE.py">main_SNARE.py</a>
 
 # Data Availability
```

### Comparing `scMDCF-0.1.2/scMDCF.egg-info/requires.txt` & `scMDCF-1.0.1/scMDCF.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `scMDCF-0.1.2/setup.py` & `scMDCF-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 setuptools.setup(
     name="scMDCF",
-    version="0.1.2",
+    version="1.0.1",
     author="Yue Cheng",
     author_email="chengyue22@mails.jlu.edu.cn",
-    description="Integrative and Cross-Modality Analysis of Single-Cell Data Across Multiomic Profiles Using scMDCF",
+    description="Unified Cross-modality Integration and Inference of Single-Cell Multiomic Data with Deep Contrastive Learning",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/DARKpmm/scMDCF",
     install_requires=["anndata==0.10.5.post1",
                       "array_api_compat==1.4.1",
                       "contourpy==1.2.0",
                       "cycler==0.12.1",
```


# Comparing `tmp/grainlearning-2.0.1.tar.gz` & `tmp/grainlearning-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grainlearning-2.0.1.tar", max compression
+gzip compressed data, was "grainlearning-2.0.3.tar", max compression
```

## Comparing `grainlearning-2.0.1.tar` & `grainlearning-2.0.3.tar`

### file list

```diff
@@ -1,12 +1,38 @@
--rw-r--r--   0        0        0    18121 2022-11-15 22:24:57.704036 grainlearning-2.0.1/LICENSE
--rw-r--r--   0        0        0     5354 2022-11-15 22:24:57.704036 grainlearning-2.0.1/README.md
--rw-r--r--   0        0        0      552 2022-11-15 23:17:30.084934 grainlearning-2.0.1/grainlearning/__init__.py
--rw-r--r--   0        0        0     7326 2022-11-15 23:17:30.068934 grainlearning-2.0.1/grainlearning/calibrationtoolbox.py
--rw-r--r--   0        0        0     7485 2022-11-15 23:17:30.064934 grainlearning-2.0.1/grainlearning/inference.py
--rw-r--r--   0        0        0     6230 2022-11-15 23:17:30.076934 grainlearning-2.0.1/grainlearning/iterativebayesianfilter.py
--rw-r--r--   0        0        0    18624 2022-11-15 23:17:30.056933 grainlearning-2.0.1/grainlearning/models.py
--rw-r--r--   0        0        0     9076 2022-11-15 23:47:48.166189 grainlearning-2.0.1/grainlearning/sampling.py
--rw-r--r--   0        0        0    17045 2022-11-15 23:17:30.048933 grainlearning-2.0.1/grainlearning/tools.py
--rw-r--r--   0        0        0      836 2022-11-15 23:18:48.382369 grainlearning-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     6080 1970-01-01 00:00:00.000000 grainlearning-2.0.1/setup.py
--rw-r--r--   0        0        0     5902 1970-01-01 00:00:00.000000 grainlearning-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    18121 2024-04-20 08:24:00.506228 grainlearning-2.0.3/LICENSE
+-rw-r--r--   0        0        0       81 2024-04-20 08:24:00.506228 grainlearning-2.0.3/NOTICE
+-rw-r--r--   0        0        0     7839 2024-04-20 08:24:00.506228 grainlearning-2.0.3/README.md
+-rw-r--r--   0        0        0      787 2024-04-20 08:24:00.514228 grainlearning-2.0.3/grainlearning/__init__.py
+-rw-r--r--   0        0        0    11740 2024-04-20 08:24:00.514228 grainlearning-2.0.3/grainlearning/bayesian_calibration.py
+-rw-r--r--   0        0        0    24018 2024-04-20 08:24:00.514228 grainlearning-2.0.3/grainlearning/dynamic_systems.py
+-rw-r--r--   0        0        0     7294 2024-04-20 08:24:00.514228 grainlearning-2.0.3/grainlearning/inference.py
+-rw-r--r--   0        0        0     9318 2024-04-20 08:24:00.514228 grainlearning-2.0.3/grainlearning/iterative_bayesian_filter.py
+-rw-r--r--   0        0        0     1682 2024-04-20 08:24:00.514228 grainlearning-2.0.3/grainlearning/rnn/README.md
+-rw-r--r--   0        0        0      324 2024-04-20 08:24:00.514228 grainlearning-2.0.3/grainlearning/rnn/__init__.py
+-rw-r--r--   0        0        0     7103 2024-04-20 08:24:00.514228 grainlearning-2.0.3/grainlearning/rnn/evaluate_model.py
+-rw-r--r--   0        0        0     2005 2024-04-20 08:24:00.514228 grainlearning-2.0.3/grainlearning/rnn/models.py
+-rw-r--r--   0        0        0     8753 2024-04-20 08:24:00.514228 grainlearning-2.0.3/grainlearning/rnn/predict.py
+-rw-r--r--   0        0        0    19827 2024-04-20 08:24:00.514228 grainlearning-2.0.3/grainlearning/rnn/preprocessor.py
+-rw-r--r--   0        0        0      740 2024-04-20 08:24:00.514228 grainlearning-2.0.3/grainlearning/rnn/sweep/example_sweep.yaml
+-rw-r--r--   0        0        0      813 2024-04-20 08:24:00.514228 grainlearning-2.0.3/grainlearning/rnn/sweep/run_sweep.sh
+-rw-r--r--   0        0        0    10382 2024-04-20 08:24:00.514228 grainlearning-2.0.3/grainlearning/rnn/train.py
+-rw-r--r--   0        0        0     1388 2024-04-20 08:24:00.522228 grainlearning-2.0.3/grainlearning/rnn/trained_models/rnn_triaxial_drained/config.yml
+-rw-r--r--   0        0        0   848920 2024-04-20 08:24:00.526228 grainlearning-2.0.3/grainlearning/rnn/trained_models/rnn_triaxial_drained/model-best.h5
+-rw-r--r--   0        0        0    17857 2024-04-20 08:24:00.526228 grainlearning-2.0.3/grainlearning/rnn/trained_models/rnn_triaxial_drained/requirements.txt
+-rw-r--r--   0        0        0      630 2024-04-20 08:24:00.526228 grainlearning-2.0.3/grainlearning/rnn/trained_models/rnn_triaxial_drained/train_stats.npy
+-rw-r--r--   0        0        0     1375 2024-04-20 08:24:00.514228 grainlearning-2.0.3/grainlearning/rnn/trained_models/rnn_triaxial_drained+e0/config.yml
+-rw-r--r--   0        0        0  1059520 2024-04-20 08:24:00.522228 grainlearning-2.0.3/grainlearning/rnn/trained_models/rnn_triaxial_drained+e0/model-best.h5
+-rw-r--r--   0        0        0    17857 2024-04-20 08:24:00.522228 grainlearning-2.0.3/grainlearning/rnn/trained_models/rnn_triaxial_drained+e0/requirements.txt
+-rw-r--r--   0        0        0      630 2024-04-20 08:24:00.522228 grainlearning-2.0.3/grainlearning/rnn/trained_models/rnn_triaxial_drained+e0/train_stats.npy
+-rw-r--r--   0        0        0     1428 2024-04-20 08:24:00.542228 grainlearning-2.0.3/grainlearning/rnn/trained_models/rnn_triaxial_undrained/config.yml
+-rw-r--r--   0        0        0   855320 2024-04-20 08:24:00.546228 grainlearning-2.0.3/grainlearning/rnn/trained_models/rnn_triaxial_undrained/model-best.h5
+-rw-r--r--   0        0        0    17480 2024-04-20 08:24:00.546228 grainlearning-2.0.3/grainlearning/rnn/trained_models/rnn_triaxial_undrained/requirements.txt
+-rw-r--r--   0        0        0      630 2024-04-20 08:24:00.546228 grainlearning-2.0.3/grainlearning/rnn/trained_models/rnn_triaxial_undrained/train_stats.npy
+-rw-r--r--   0        0        0     1380 2024-04-20 08:24:00.526228 grainlearning-2.0.3/grainlearning/rnn/trained_models/rnn_triaxial_undrained+e0/config.yml
+-rw-r--r--   0        0        0  2644536 2024-04-20 08:24:00.542228 grainlearning-2.0.3/grainlearning/rnn/trained_models/rnn_triaxial_undrained+e0/model-best.h5
+-rw-r--r--   0        0        0    17857 2024-04-20 08:24:00.542228 grainlearning-2.0.3/grainlearning/rnn/trained_models/rnn_triaxial_undrained+e0/requirements.txt
+-rw-r--r--   0        0        0      630 2024-04-20 08:24:00.542228 grainlearning-2.0.3/grainlearning/rnn/trained_models/rnn_triaxial_undrained+e0/train_stats.npy
+-rw-r--r--   0        0        0     5052 2024-04-20 08:24:00.546228 grainlearning-2.0.3/grainlearning/rnn/windows.py
+-rw-r--r--   0        0        0    14396 2024-04-20 08:24:00.546228 grainlearning-2.0.3/grainlearning/sampling.py
+-rw-r--r--   0        0        0    21588 2024-04-20 08:24:00.546228 grainlearning-2.0.3/grainlearning/tools.py
+-rw-r--r--   0        0        0     1876 2024-04-20 08:24:00.546228 grainlearning-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     9792 1970-01-01 00:00:00.000000 grainlearning-2.0.3/PKG-INFO
```

### Comparing `grainlearning-2.0.1/LICENSE` & `grainlearning-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `grainlearning-2.0.1/grainlearning/__init__.py` & `grainlearning-2.0.3/grainlearning/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-from .models import Model, IOModel
-from .calibrationtoolbox import CalibrationToolbox
-from .iterativebayesianfilter import IterativeBayesianFilter
-from .sampling import GaussianMixtureModel, generate_params_qmc
-from .inference import SMC
-from .tools import (
+"""GrainLearning: A Python package for Bayesian calibration and uncertainty quantification
+   of granular material models.
+"""
+from grainlearning.dynamic_systems import DynamicSystem, IODynamicSystem
+from grainlearning.sampling import GaussianMixtureModel, generate_params_qmc
+from grainlearning.inference import SMC
+from grainlearning.iterative_bayesian_filter import IterativeBayesianFilter
+from grainlearning.bayesian_calibration import BayesianCalibration
+from grainlearning.tools import (
     write_to_table,
     get_keys_and_data,
     regenerate_params_with_gmm,
     get_pool,
     residual_resample,
     stratified_resample,
     systematic_resample,
```

### Comparing `grainlearning-2.0.1/grainlearning/inference.py` & `grainlearning-2.0.3/grainlearning/inference.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,227 +1,194 @@
+"""
+This module contains various methods for performing statistical and Bayesian inference
+"""
 from typing import Type
 import numpy as np
-
-from .models import Model
-
 from scipy.stats import multivariate_normal
+from grainlearning.dynamic_systems import DynamicSystem
 
 
 class SMC:
     """This is the Sequential Monte Carlo class that recursively
-    update the model state and model parameters based on Bayes' theorem
+    update model states based on sequential observations using the Bayes' theorem
 
     There are two ways of initializing the class.
 
     Method 1 - dictionary style
 
     .. highlight:: python
     .. code-block:: python
 
-        model_cls = SMC.from_dict(
+        system_cls = SMC.from_dict(
             {
                 "ess_target": 0.3,
-                "scale_cov_with_max": True
+                "scale_cov_with_max": False
             }
         )
 
     or
 
     Method 2 - class style
 
     .. highlight:: python
     .. code-block:: python
 
-        model_cls = SMC(
+        system_cls = SMC(
                 ess_target = 0.3,
-                scale_cov_with_max = True
+                scale_cov_with_max = False
         )
 
-    :param ess_target: Target effective sample size (what we want)
-    :param scale_cov_with_max: Flag if the covariance matrix should scale with the maximum accross the loading steps, defaults to True
+    :param ess_target: Target effective sample size (w_0 / sum_i w_i^2)
+        where w_0 = 1 / N_p, defaults to 0.3
+    :param scale_cov_with_max: True if the covariance matrix is scaled
+        with the maxima of the observations, defaults to True
+    :param cov_matrices: Covariance matrices of shape (num_steps, num_obs, num_obs),
+        defaults to None, Optional
+    :param likelihoods: Likelihood distributions of shape (num_steps, num_samples)
+    :param posteriors: Posterior distributions of shape (num_steps, num_samples)
+    :param ess: Time evolution of the effective sample size
     """
-
-    #: Target effective sample size.
-    ess_target: float
-
-    #: Flag if the covariance matrix should be scaled with the maximum values of the observations
-    scale_cov_with_max: bool = True
-
-    #: Covariance matricies of shape (num_steps,num_obs,num_obs)
-    cov_matrices: np.array
-
-    #: Likelihoods of shape (num_steps, num_samples)
-    likelihoods: np.array
-
-    #: Posteriors of shape (num_steps, num_samples)
-    posteriors: np.array
-
-    #: Array containing ips of (num_steps, num_params)
-    ips: np.array
-
-    #: Array containing covs of (num_steps, num_params)
-    covs: np.array
-
-    #: Calculated effective sample size
-    ess: float
-
     def __init__(
         self,
         ess_target: float,
-        scale_cov_with_max: bool = True,
+        scale_cov_with_max: bool = False,
+        cov_matrices: np.array = None,
     ):
-        """Initialize the variables."""
+        """Initialize the SMC class"""
         self.ess_target = ess_target
+
         self.scale_cov_with_max = scale_cov_with_max
 
+        self.cov_matrices = cov_matrices
+
+        self.likelihoods = None
+
+        self.posteriors = None
+
+        self.ess = None
+
     @classmethod
     def from_dict(cls: Type["SMC"], obj: dict):
-        """Initialize the class using a dictionary style"""
+        """Initialize the class using a dictionary style
+
+        :param obj: a dictionary containing the keys and values to construct an SMC object
+        :return: an SMC object
+        """
         return cls(
             ess_target=obj["ess_target"],
-            scale_cov_with_max=obj.get("scale_cov_with_max", True),
+            scale_cov_with_max=obj.get("scale_cov_with_max", False),
+            cov_matrices=obj.get("cov_matrices", None),
         )
 
-    def get_covariance_matrices(
-        self, sigma_guess: float, model: Type["Model"]
-    ) -> np.array:
-        """Compute the diagonal covariance matrices from a given input sigma.
+    def get_covariance_matrices(self, sigma: float, system: Type["DynamicSystem"]):
+        """Compute the (diagonal) covariance matrices from an uncertainty that is either
+        assumed by the user or updated by SMC to satisfy the target effective sample size.
 
-        This function is vectorized for all loading steps
+        This function is vectorized for all time steps
 
-        :param sigma_guess: input sigma
-        :param model: Model class
-        :return: Covariance matrices for all loading steps
+        :param sigma: Uncertainty
+        :param system: Dynamic system
+        :return: Covariance matrices for all time steps
         """
-        cov_matrix = sigma_guess * model._inv_normalized_sigma
+        cov_matrix = sigma * system.get_inv_normalized_sigma()
 
-        # duplicated covariant matrix to loading step
-        cov_matrices = cov_matrix[None, :].repeat(model.num_steps, axis=0)
+        # duplicated the covariant matrix in time
+        cov_matrices = cov_matrix[None, :].repeat(system.num_steps, axis=0)
 
-        # scale with the maximum of the loading steps
         if self.scale_cov_with_max:
-            cov_matrices *= model.obs_data.max(axis=1)[:, None] ** 2
+            # scale with the maxima of the observations
+            cov_matrices *= system.obs_data.max(axis=1)[:, None] ** 2
         else:
-            # or element wise multiplication of covariant matrix with observables of all loading steps
-            cov_matrices *= model.obs_data.T[:, None] ** 2
+            # or element wise multiplication of covariant matrix with observables of all time steps
+            cov_matrices *= system.obs_data.T[:, None] ** 2
 
         return cov_matrices
 
-    def get_likelihoods(self, model: Type["Model"], cov_matrices: np.array) -> np.array:
-        """Compute the likelihoods as a multivariate normal of the simulation data centered around the observations.
+    @staticmethod
+    def get_likelihoods(system: Type["DynamicSystem"], cov_matrices: np.array):
+        """Compute the likelihood distributions of simulation data as a multivariate normal
+        centered around the observation.
 
-        This function is vectorized for all loading steps
+        This function is vectorized for all time steps
 
-        :param model: Model class
-        :param cov_matrices: covariance matricies
-        :return: Likelihood matrices for all loading steps
+        :param system: Dynamic system class
+        :param cov_matrices: Covariance matrices of shape (num_steps, num_obs, num_obs)
+        :return: Likelihood matrices of shape (num_steps, num_samples) considering all time steps
         """
-        likelihoods = np.zeros((model.num_steps, model.num_samples))
+        likelihoods = np.zeros((system.num_steps, system.num_samples))
 
-        for stp_id in range(model.num_steps):
+        for stp_id in range(system.num_steps):
             # see https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.multivariate_normal.html
             likelihood = multivariate_normal.pdf(
-                model.sim_data[:, :, stp_id],
-                mean=model.obs_data[:, stp_id],
+                system.sim_data[:, :, stp_id],
+                mean=system.obs_data[:, stp_id],
                 cov=cov_matrices[stp_id],
             )
             likelihoods[stp_id, :] = likelihood / likelihood.sum()
 
         return likelihoods
 
-    def get_posterors(
-        self, model: Type["Model"], likelihoods: np.array, proposal_ibf: np.array = None
-    ) -> np.array:
-        """Compute the posteriors for all the loading steps
-
-        This function is vectorized for all loading steps
-
-        :param model: Model class
-        :param likelihoods: Likelihood matrices
-        :param proposal_ibf: Optional input proposal
-        :return: Posterior distributions for all loading steps
+    @staticmethod
+    def get_posteriors(system: Type["DynamicSystem"], likelihoods: np.array, proposal: np.array = None):
+        """Compute the posterior distributions from the likelihood for all the time steps
+
+        This function is vectorized for all time steps
+
+        :param system: Dynamic system class
+        :param likelihoods: Likelihood matrices of shape (num_steps, num_samples)
+        :param proposal: Proposal distribution at the initial time step, defaults to None, optional
+        :return: Posterior matrices of shape (num_steps, num_samples) considering all time steps
         """
-        posteriors = np.zeros((model.num_steps, model.num_samples))
+        posteriors = np.zeros((system.num_steps, system.num_samples))
 
-        if proposal_ibf is None:
-            proposal = np.ones([model.num_samples]) / model.num_samples
-        else:
-            proposal = proposal_ibf
+        if proposal is None:
+            proposal = np.ones([system.num_samples]) / system.num_samples
 
         posteriors[0, :] = likelihoods[0, :] / proposal
         posteriors[0, :] /= posteriors[0, :].sum()
 
-        for stp_id in range(1, model.num_steps):
+        for stp_id in range(1, system.num_steps):
             posteriors[stp_id, :] = posteriors[stp_id - 1, :] * likelihoods[stp_id, :]
             posteriors[stp_id, :] /= posteriors[stp_id, :].sum()
 
         return posteriors
 
-    def get_ensemble_ips_covs(
-        self,
-        model: Type["Model"],
-        posteriors: np.array,
-    ) -> np.array:
-        """Compute the ensemble averages for parameters. (Used for post-processing)
-
-        This function is vectorized for all loading steps
-
-        :param model: Model class
-        :param posteriors: Posterior distributions
-        :return: Ensemble averages
-        """
-        ips = np.zeros((model.num_steps, model.num_params))
-        covs = np.zeros((model.num_steps, model.num_params))
-
-        for stp_id in range(model.num_steps):
-            ips[stp_id, :] = posteriors[stp_id, :] @ model.param_data
-
-            covs[stp_id, :] = (
-                posteriors[stp_id, :] @ (ips[stp_id, :] - model.param_data) ** 2
-            )
-
-            covs[stp_id, :] = np.sqrt(covs[stp_id, :]) / ips[stp_id, :]
-
-        return ips, covs
-
-    def give_posterior(self, loading_step=-1):
-        """Give posterior distribution of a loading step
+    def get_posterior_at_time(self, time_step: int = -1):
+        """Get the posterior distribution at a certain time step
 
-        :param loading_step: Optional input loading step, defaults to -1 (last value)
-        :return: Posterior distribution for a single step
+        :param time_step: input time step, defaults to -1 (the last step in time), optional
+        :return: Posterior distribution at a certain time step
         """
-        return self.posteriors[loading_step, :]
+        return self.posteriors[time_step, :]
 
-    def data_assimilation_loop(
-        self, sigma_guess: float, model: Type["Model"], proposal_ibf: np.ndarray = None
-    ):
+    def data_assimilation_loop(self, sigma: float, system: Type["DynamicSystem"], proposal: np.ndarray = None):
         """Perform data assimilation loop
 
-        :param sigma_guess: Guess of sigma
-        :param proposal_ibf: Input distribution
-        :param model: Model class
+        :param sigma: Uncertainty
+        :param proposal: Proposal distribution from which the samples are sampled from, defaults to None, optional
+        :param system: Dynamic system class
         :return: Result of the objective function which converges to a user defined effective sample size
         """
         self.cov_matrices = self.get_covariance_matrices(
-            sigma_guess=sigma_guess, model=model
+            sigma=sigma, system=system
         )
         self.likelihoods = self.get_likelihoods(
-            model=model, cov_matrices=self.cov_matrices
+            system=system, cov_matrices=self.cov_matrices
         )
 
-        self.posteriors = self.get_posterors(
-            model=model, likelihoods=self.likelihoods, proposal_ibf=proposal_ibf
-        )
-
-        self.ips, self.covs = self.get_ensemble_ips_covs(
-            model=model, posteriors=self.posteriors
-        )
-
-        # TODO: I (Hongyang) would save the whole effective sample size sequence in time.
-        #  Examining the evolution of eff gives you a good idea how your filtering algorithm is doing.
-        self.ess = 1.0 / np.sum(
-            self.posteriors[-1, :] ** 2,
-        )
+        self.posteriors = self.get_posteriors(system=system, likelihoods=self.likelihoods, proposal=proposal)
 
-        self.ess /= model.num_samples
+        self.compute_effective_sample_size()
+        return (self.ess[-1] - self.ess_target) ** 2
 
-        return (self.ess - self.ess_target) ** 2
+    def set_posteriors(self, posteriors: np.ndarray = None):
+        """Set the posterior distribution"""
+        self.posteriors = posteriors
+
+    def compute_effective_sample_size(self):
+        """Compute the effective sample size"""
+        # compute the effective sample size for every time step
+        num_steps, num_samples = self.posteriors.shape
+        ess = 1.0 / np.sum(self.posteriors ** 2, axis=1)
+        ess /= num_samples
+        ess = ess.reshape(num_steps, 1)
+        self.ess = ess
```

### Comparing `grainlearning-2.0.1/grainlearning/models.py` & `grainlearning-2.0.3/grainlearning/dynamic_systems.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,168 +1,139 @@
-from typing import Type, List, Callable, Tuple
+"""
+This module contains various classes of state-space systems that describe
+the time evolution of the system's hidden state based on partial observations from the real world.
+"""
+from typing import Type, List, Callable
+import os
+from datetime import datetime
+from math import floor, log
+from glob import glob
 import numpy as np
-from .tools import get_keys_and_data, write_to_table
+from grainlearning.tools import get_keys_and_data, write_to_table
 
 
-class Model:
-    """
-    This is the probabalistic model class. It contains information on the observation (or reference) data, simulation data, parameters and reference. It is also used to run a callback for the simulations.
+class DynamicSystem:
+    """This is the dynamical system class.
+
+    A dynamical system (also known as a state-space system) describes
+    the time evolution of the system's (hidden) state and observation using the following equations:
+
+    .. math::
+        x_t & = f(x_{t−1}) + q_{t−1}
+
+        y_t & = h(x_t) + r_t
+
+    where
+    :math:`x_t` is the hidden state,
+    :math:`y_t` is the observation, both represented as random processes,
+    :math:`f` is the state transition function,
+    :math:`h` is the observation function,
+    :math:`q_{t−1}` is the process noise, and :math:`r_t` is the observation noise.
+
+    In the context of Bayesian parameter estimation, :math:`f` is the model
+    that describe the physical process and :math:`h` is the model that describe
+    the relationship between the hidden state and observation.
+    In the simplest case, :math:`h` is an identity matrix which indicate the one-to-one relationship
+    between :math:`x_t` and :math:`y_t`.
+
+    Therefore, the :class:`.DynamicSystem` class is used to encapsulate the observation data
+    and the simulation data, which require specifying the number of samples and
+    the lower and upper bound of the parameters.
 
     There are two ways of initializing the class.
 
     Method 1 - dictionary style
 
     .. highlight:: python
     .. code-block:: python
 
-        model_cls = Model.from_dict(
+        system_cls = DynamicSystem.from_dict(
             {
-
-                "param_mins": [0, 0],
-                "param_maxs": [1, 10],
+                "param_names": ["a", "b"],
+                "param_min": [0, 0],
+                "param_max": [1, 10],
                 "num_samples": 14,
                 "obs_data": y_obs,
-                "ctrl_data": x_ctrl,
-                "callback": run_sim
+                "ctrl_data": y_ctrl,
             }
         )
 
     or
 
     Method 2 - class style
 
     .. highlight:: python
     .. code-block:: python
 
-        model_cls = Model(
-                param_mins = [0, 0],
-                param_maxs = [1, 10],
-                num_samples = 14,
-                obs_data = y_obs,
-                ctrl_data = x_ctrl,
-                callback = run_sim
+        system_cls = DynamicSystem(
+            param_names = ["a", "b"],
+            param_min = [0, 0],
+            param_max = [1, 10],
+            num_samples = 14,
+            obs_data = y_obs,
+            ctrl_data = y_ctrl,
         )
 
-    y_obs is the observation data, x_ctrl is the control data. The callback function inputs the model as an argument, where one can modify the model.sim_data.
-
-    :param obs_data: Observation or reference data
-    :param num_samples: Sample size
-    :param param_mins: List of parameter lower bounds
-    :param param_maxs: List of parameter Upper bounds
-    :param ctrl_data: Optional control data (e.g, time), defaults to None
-    :param obs_names: Column names of the observation data, defaults to None
-    :param ctrl_name: Coloumn name of the control data, defaults to None
-    :param inv_obs_weight: Inverse of the observation weight, defaults to None
-    :param param_data: Parameter data, defaults to None
-    :param param_names: Parameter names, defaults to None
-    :param sim_data: Simulation data, defaults to None
-    :param callback: Callback function, defaults to None
-    :param sigma_max: Uncertainty, defaults to 1.0e6
-    """
-
-    ##### Parameters #####
-
-    #: Parameter data of shape (num_samples, num_params)
-    param_data: np.ndarray
-
-    #: Parameter data of previous iteration
-    param_data_prev: np.ndarray
-
-    #: Number of parameters
-    num_params: int
-
-    #: Minimum values of the parameters
-    param_mins: List
-
-    #: Maximum number of parameters
-    param_maxs: List
-
-    #: Names of the parameters.
-    param_names: List[str]
-
-    ##### Observations #####
-
-    #: Observation (or reference) data of shape (num_obs,num_steps)
-    obs_data: np.ndarray
-
-    #: Observation keys
-    obs_names: List[str]
-
-    #: Inverse observation weight
-    inv_obs_weight: List[float]
-
-    #: Number of steps or sequence size in the dataset
-    num_steps: int
-
-    #: Number of observations in the dataset
-    num_obs: int
-
-    #: Control data (num_control,num_steps)
-    ctrl_data = np.ndarray
-
-    #: Observation control (e.g., time)
-    ctrl_name: str
-
-    #: Number of control data
-    num_ctrl: int
-
-    ##### Simulations #####
+    You can pass the simulation data to the class using the :meth:`.DynamicSystem.set_sim_data` method.
 
-    #: Name of the simulation (e.g., sim)
-    sim_name: str = 'sim'
-
-    #: Simulation data of shape (num_samples,num_obs,num_steps)
-    sim_data: np.ndarray
-
-    #: Number of samples (usually specified by user)
-    num_samples: int
-
-    #: Callback function. The input arugment is the model where model.sim_data is modified
-    callback: Callable
-
-    ##### Uncertainty #####
-
-    #: Minimum value of the uncertainty
-    sigma_min: float = 1.0e-6
-
-    #: Maximum value of the uncertainty
-    sigma_max: float = 1.0e6
+    .. highlight:: python
+    .. code-block:: python
 
-    #: Sigma tolerance
-    sigma_tol: float = 1.0e-3
+        system_cls.set_sim_data(x)
 
-    #: Calculated normalized sigma to weigh the covariance matrix
-    _inv_normalized_sigma: np.array
+    The simulation data is a numpy array of shape (num_samples, num_obs, num_steps).
 
+    :param obs_data: observation or reference data
+    :param num_samples: Sample size of the ensemble of model evaluations
+    :param num_steps: Number of steps or sequence size in the dataset
+    :param num_obs:  Number of observations in the dataset
+    :param num_ctrl: Number of control data (identical between simulation and observation)
+    :param param_min: List of parameter lower bounds
+    :param param_max: List of parameter Upper bounds
+    :param curr_iter: current iteration ID, defaults to 0
+    :param ctrl_data: control data (e.g, time), defaults to None, optional
+    :param obs_names: Column names of the observation data, defaults to None, optional
+    :param ctrl_name: Column name of the control data, defaults to None, optional
+    :param inv_obs_weight: Inverse of the observation weight, defaults to None, optional
+    :param param_data: Parameter data, defaults to None, optional
+    :param param_names: Parameter names, defaults to None, optional
+    :param sim_data: Simulation data, defaults to None, optional
+    :param sigma_max: Maximum uncertainty, defaults to 1.0e6, optional
+    :param sigma_tol: Tolerance of the estimated uncertainty, defaults to 1.0e-3, optional
+    :param sim_name: Name of the simulation, defaults to 'sim', optional
+    :param sigma_min: Minimum uncertainty, defaults to 1.0e-6, optional
+    :param _inv_normalized_sigma:  Calculated normalized sigma to weigh the covariance matrix
+    :param estimated_params: Estimated parameter as the first moment of the distribution (:math:`x_\mu = \sum_i w_i * x_i`), defaults to None, optional
+    :param estimated_params_cv: Estimated parameter coefficient of variation as the second moment of the distribution (:math:`x_\sigma = \sqrt{\sum_i w_i * (x_i - x_\mu)^2} / x_\mu`), defaults to None, optional
+    """
     def __init__(
         self,
         obs_data: np.ndarray,
         num_samples: int,
-        param_mins: List[float],
-        param_maxs: List[float],
+        param_min: List[float],
+        param_max: List[float],
         ctrl_data: np.ndarray = None,
         obs_names: List[str] = None,
         ctrl_name: str = None,
         inv_obs_weight: List[float] = None,
-        sim_name: str = None,
+        sim_name: str = 'sim',
         sim_data: np.ndarray = None,
-        callback: Callable = None,
+        curr_iter: int = 0,
         param_data: np.ndarray = None,
         param_names: List[str] = None,
         sigma_max: float = 1.0e6,
         sigma_tol: float = 1.0e-3
     ):
-        """Initialize the Model class"""
+        """Initialize the dynamic system class"""
         #### Observations ####
         self.obs_data = np.array(
             obs_data, ndmin=2
         )  # ensure data is of shape (num_obs,num_step).
 
-        if ctrl_data is not None:
-            self.ctrl_data = ctrl_data
+        self.ctrl_data = ctrl_data
 
         self.obs_names = obs_names
 
         self.ctrl_name = ctrl_name
 
         self.num_obs, self.num_steps = self.obs_data.shape
 
@@ -177,376 +148,477 @@
 
         self.num_samples = num_samples
 
         self.sim_name = sim_name
 
         self.sim_data = sim_data
 
-        self.callback = callback
+        self.curr_iter = curr_iter
 
-        self.param_mins = param_mins
+        self.param_min = param_min
 
-        self.param_maxs = param_maxs
+        self.param_max = param_max
 
         #### Parameters ####
 
-        if param_mins: self.num_params = len(param_mins)
+        if param_min:
+            self.num_params = len(param_min)
+        else:
+            self.num_params = 0
 
         self.param_data = param_data
 
         self.param_names = param_names
 
         #### Uncertainty ####
 
+        self.sigma_min =  1.0e-6
+
         self.sigma_max = sigma_max
 
         self.sigma_tol = sigma_tol
 
-        self.get_inv_normalized_sigma()
+        self._inv_normalized_sigma = None
+
+        self.compute_inv_normalized_sigma()
+
+        self.estimated_params = None
+
+        self.estimated_params_cv = None
 
     @classmethod
-    def from_dict(cls: Type["Model"], obj: dict) -> Type["Model"]:
-        """ Initialize the class using a dictionary style"""
+    def from_dict(cls: Type["DynamicSystem"], obj: dict):
+        """ Initialize the class using a dictionary style
+
+        :param obj: Dictionary object
+        :return: DynamicSystem: DynamicSystem object
+        """
 
-        # TODO do proper error checking on the input
         assert "obs_data" in obj.keys(), "Error no obs_data key found in input"
         assert "num_samples" in obj.keys(), "Error no num_samples key found in input"
-        assert "param_mins" in obj.keys(), "Error no param_mins key found in input"
-        assert "param_maxs" in obj.keys(), "Error no param_maxs key found in input"
+        assert "param_min" in obj.keys(), "Error no param_min key found in input"
+        assert "param_max" in obj.keys(), "Error no param_max key found in input"
 
         return cls(
             obs_data=obj["obs_data"],
             num_samples=obj["num_samples"],
-            param_mins=obj["param_mins"],
-            param_maxs=obj["param_maxs"],
+            param_min=obj["param_min"],
+            param_max=obj["param_max"],
             ctrl_data=obj.get("ctrl_data", None),
             obs_names=obj.get("obs_names", None),
             ctrl_name=obj.get("ctrl_name", None),
             inv_obs_weight=obj.get("inv_obs_weight", None),
-            sim_name=obj.get("sim_name", None),
+            sim_name=obj.get("sim_name", 'sim'),
             sim_data=obj.get("sim_data", None),
-            callback=obj.get("callback", None),
             param_data=obj.get("param_data", None),
             param_names=obj.get("param_names", None),
             sigma_tol=obj.get("sigma_tol", 0.001),
         )
 
-    def run(self, **kwargs):
-        """This function runs the callback function"""
+    def set_sim_data(self, data: list):
+        """Set the simulation data
 
-        if self.callback is None:
-            raise ValueError("No callback function defined")
+        :param data: simulation data of shape (num_samples, num_obs, num_steps)
+        """
+        self.sim_data = np.array(data)
 
-        self.callback(self, **kwargs)
+    def set_param_data(self, data: list):
+        """Set the simulation data
 
-    def get_inv_normalized_sigma(self):
-        inv_obs_mat = np.diagflat(self.inv_obs_weight)
-        self._inv_normalized_sigma = inv_obs_mat * np.linalg.det(inv_obs_mat) ** (
-            -1.0 / inv_obs_mat.shape[0]
+        :param data: parameter data of shape (num_samples, num_params)
+        """
+        self.param_data = np.array(data)
+
+    def set_obs_data(self, data: list):
+        """Set the observation data
+        :param data: observation data of shape (num_obs, num_steps)
+        """
+        self.obs_data = np.array(data,ndmin=2)
+
+    def set_ctrl_data(self, data: list):
+        """Set the control data
+        :param data: control data of shape (num_ctrl, num_steps)
+        """
+        self.ctrl_data = np.array(data)
+
+    def compute_inv_normalized_sigma(self):
+        """Compute the inverse of the matrix that apply different weights on the observables"""
+        inv_obs_weight = np.diagflat(self.inv_obs_weight)
+        self._inv_normalized_sigma = inv_obs_weight * np.linalg.det(inv_obs_weight) ** (
+            -1.0 / inv_obs_weight.shape[0]
         )
 
+    def reset_inv_normalized_sigma(self):
+        """Reset the inverse of the weighting matrix to None"""
+        self._inv_normalized_sigma = None
+
+    def get_inv_normalized_sigma(self):
+        """Get the inverse of the matrix that apply different weights on the observables"""
+        return self._inv_normalized_sigma
+
+    def compute_estimated_params(self, posteriors: np.array):
+        """Compute the estimated means and uncertainties for the parameters.
+
+        This function is vectorized for all time steps
+
+        :param posteriors: Posterior distribution of shape (num_steps, num_samples)
+        """
+        self.estimated_params = np.zeros((self.num_steps, self.num_params))
+        self.estimated_params_cv = np.zeros((self.num_steps, self.num_params))
+
+        for stp_id in range(self.num_steps):
+            self.estimated_params[stp_id, :] = posteriors[stp_id, :] @ self.param_data
+
+            self.estimated_params_cv[stp_id, :] = (
+                posteriors[stp_id, :] @ (self.estimated_params[stp_id, :] - self.param_data) ** 2
+            )
+
+            self.estimated_params_cv[stp_id, :] = np.sqrt(
+                self.estimated_params_cv[stp_id, :]) / self.estimated_params[stp_id, :]
+
+    @classmethod
+    def load_param_data(cls: Type["DynamicSystem"]):
+        """Virtual function to load param data from disk"""
+
+    @classmethod
+    def get_sim_data_files(cls: Type["DynamicSystem"]):
+        """Virtual function to get simulation data files from disk"""
+
+    @classmethod
+    def load_sim_data(cls: Type["DynamicSystem"]):
+        """Virtual function to load simulation data"""
+
+    @classmethod
+    def write_params_to_table(cls: Type["DynamicSystem"]):
+        """Write the parameter data into a text file"""
+
+    @classmethod
+    def backup_sim_data(cls: Type["DynamicSystem"]):
+        """Virtual function to backup simulation data"""
+
+    @classmethod
+    def set_up_sim_dir(cls: Type["DynamicSystem"]):
+        """Virtual function to set up simulation directory"""
+    @classmethod
+    def move_data_to_sim_dir(cls: Type["DynamicSystem"]):
+        """Virtual function to move data into simulation directory"""
 
-class IOModel(Model):
+
+class IODynamicSystem(DynamicSystem):
     """
-    This is the IOModel class to compute the posterior distribution from an existing dataset,
-    and generate new parameter values for additional simulation runs.
+    This is the I/O dynamic system class derived from the dynamic system class.
+    Extra functionalities are added to handle I/O operations.
 
     There are two ways of initializing the class.
 
     Method 1 - dictionary style
 
     .. highlight:: python
     .. code-block:: python
 
-        model_cls = Model.from_dict(
+        system_cls = IODynamicSystem.from_dict(
             {
-                "param_mins": [0, 0],
-                "param_maxs": [1, 10],
+                "system_type": IODynamicSystem,
+                "param_min": [0, 0],
+                "param_max": [1, 10],
+                "param_names": ['a', 'b'],
                 "num_samples": 14,
-                "obs_data": y_obs,
-                "ctrl_data": x_ctrl,
-                "callback": run_sim
+                "obs_data_file": 'obs_data.txt',
+                "obs_names": ['y_obs'],
+                "ctrl_name": 'y_ctrl
+                "sim_name": 'linear',
+                "sim_data_file_ext": '.txt',
             }
         )
 
     or
 
     Method 2 - class style
 
     .. highlight:: python
     .. code-block:: python
 
-        model_cls = Model(
-                param_mins = [0, 0],
-                param_maxs = [1, 10],
+        system_cls = IODynamicSystem(
+                param_min = [0, 0],
+                param_max = [1, 10],
+                param_names = ['a', 'b'],
                 num_samples = 14,
-                obs_data = y_obs,
-                ctrl_data = x_ctrl,
-                callback = run_sim
+                obs_data_file = 'obs_data.txt',
+                obs_names = ['y_obs'],
+                ctrl_name = 'y_ctrl',
+                sim_name = 'linear',
+                sim_data_file_ext = '.txt',
         )
 
-    y_obs is the observation data, x_ctrl is the control data. The callback function inputs the model as an argument, where one can modify the model.sim_data.
-
-    :param obs_data: Observation or reference data
-    :param num_samples: Sample size
-    :param param_mins: List of parameter lower bounds
-    :param param_maxs: List of parameter Upper bounds
-    :param ctrl_data: Optional control data (e.g, time), defaults to None
-    :param obs_names: Column names of the observation data, defaults to None
-    :param ctrl_name: Coloumn name of the control data, defaults to None
-    :param inv_obs_weight: Inverse of the observation weight, defaults to None
-    :param param_data: Parameter data, defaults to None
+    :param param_min: List of parameter lower bounds
+    :param param_max: List of parameter Upper bounds
     :param param_names: Parameter names, defaults to None
-    :param sim_data_files: Simulation data files, defaults to None
-    :param sim_data: Simulation data, defaults to None
-    :param callback: Callback function, defaults to None
-    :param sigma_max: Uncertainty, defaults to 1.0e6
+    :param num_samples: Sample size of the ensemble of model evaluations
+    :param obs_data_file: Observation data file, defaults to None
+    :param obs_names: Column names of the observation data, defaults to None
+    :param ctrl_name: Column name of the control data, defaults to None
+    :param sim_name: Name of the simulation, defaults to 'sim'
+    :param sim_data_dir: Simulation data directory, defaults to './sim_data'
+    :param sim_data_file_ext: Simulation data file extension, defaults to '.npy'
+    :param curr_iter: Current iteration ID, defaults to 0
+    :param param_data_file: Parameter data file, defaults to None, optional
+    :param obs_data: observation or reference data, optional
+    :param ctrl_data: Control data (e.g, time), defaults to None, optional
+    :param inv_obs_weight: Inverse of the observation weight, defaults to None, optional
+    :param param_data: Parameter data, defaults to None, optional
+    :param sim_data: Simulation data, defaults to None, optional
+    :param sim_data_files: List of simulation data files (num_samples), defaults to None, optional
     """
 
-    ##### Parameters #####
-
-    #: Name of the parameter data file
-    param_data_file: str
-
-    ##### Observations #####
-
-    #: Name of the observation data file
-    obs_data_file: str
-
-    ##### Simulations #####
-
-    #: Simulation data files (num_samples)
-    sim_data_files: List[str]
-
-    #: Name of the directory where simulation data is stored
-    sim_data_dir: str = './sim_data'
-
-    #: Extension of simulation data files
-    sim_data_file_ext: str = '.npy'
-
     def __init__(
         self,
         sim_name: str,
         sim_data_dir: str,
         sim_data_file_ext: str,
         obs_data_file: str,
         obs_names: List[str],
         ctrl_name: str,
-        param_data_file: str,
-        obs_data: np.ndarray,
         num_samples: int,
-        param_mins: List[float],
-        param_maxs: List[float],
+        param_min: List[float],
+        param_max: List[float],
+        obs_data: np.ndarray = None,
         ctrl_data: np.ndarray = None,
         inv_obs_weight: List[float] = None,
         sim_data: np.ndarray = None,
-        callback: Callable = None,
+        curr_iter: int = 0,
+        param_data_file: str = '',
         param_data: np.ndarray = None,
         param_names: List[str] = None,
     ):
-        """Initialize the IOModel class"""
+        """Initialize the IO dynamic system class"""
 
         #### Calling base constructor ####
 
         super().__init__(
             obs_data,
             num_samples,
-            param_mins,
-            param_maxs,
+            param_min,
+            param_max,
             ctrl_data,
             obs_names,
             ctrl_name,
             inv_obs_weight,
             sim_name,
             sim_data,
-            callback,
+            curr_iter,
             param_data,
             param_names
         )
+        # TODO: reuse initialization from base class
 
         ##### Parameters #####
 
         self.num_params = len(param_names)
 
         self.param_data_file = param_data_file
 
         #### Simulations ####
 
         self.sim_name = sim_name
 
         self.sim_data_dir = sim_data_dir
 
+        self.sim_data_sub_dir = None
+
         self.sim_data_file_ext = sim_data_file_ext
 
         #### Observations ####
 
-        self.obs_data_file = sim_data_dir + '/' + obs_data_file
+        self.obs_data_file = obs_data_file
 
         self.ctrl_name = ctrl_name
 
         self.obs_names = obs_names
 
         self.get_obs_data()
 
         if inv_obs_weight is None:
             self.inv_obs_weight = list(np.ones(self.num_obs))
         else:
             self.inv_obs_weight = inv_obs_weight
 
-        self.get_inv_normalized_sigma()
+        self.compute_inv_normalized_sigma()
+
+        self.sim_data_files = []
 
     @classmethod
-    def from_dict(cls: Type["IOModel"], obj: dict) -> Type["IOModel"]:
-        """ Initialize the class using a dictionary style"""
+    def from_dict(cls: Type["IODynamicSystem"], obj: dict):
+        """ Initialize the class using a dictionary style
 
-        # TODO do proper error checking on the input
-        assert "sim_name" in obj.keys(), "Error no sim_name key found in input"
-        assert "sim_data_dir" in obj.keys(), "Error no sim_data_dir key found in input"
+        :param obj: Dictionary object
+        :return IODynamicSystem: IODynamicSystem object
+        """
+        assert "param_names" in obj.keys(), "Error no param_names key found in input"
         assert "obs_data_file" in obj.keys(), "Error no obs_data_file key found in input"
         assert "obs_names" in obj.keys(), "Error no obs_names key found in input"
         assert "ctrl_name" in obj.keys(), "Error no ctrl_name key found in input"
-        if "param_data_file" not in obj.keys(): obj["param_data_file"] = None
+        assert "sim_name" in obj.keys(), "Error no sim_name key found in input"
+        assert "sim_data_dir" in obj.keys(), "Error no sim_data_dir key found in input"
 
         return cls(
             sim_name=obj["sim_name"],
             sim_data_dir=obj["sim_data_dir"],
             sim_data_file_ext=obj.get("sim_data_file_ext", '.npy'),
             obs_data_file=obj["obs_data_file"],
             obs_names=obj["obs_names"],
             ctrl_name=obj["ctrl_name"],
-            param_data_file=obj["param_data_file"],
+            param_data_file=obj.get("param_data_file", ''),
             obs_data=obj.get("obs_data", None),
             num_samples=obj.get("num_samples", None),
-            param_mins=obj.get("param_mins", None),
-            param_maxs=obj.get("param_maxs", None),
+            param_min=obj.get("param_min", None),
+            param_max=obj.get("param_max", None),
             ctrl_data=obj.get("ctrl_data", None),
             inv_obs_weight=obj.get("inv_obs_weight", None),
             sim_data=obj.get("sim_data", None),
-            callback=obj.get("callback", None),
             param_data=obj.get("param_data", None),
             param_names=obj.get("param_names", None),
         )
 
     def get_obs_data(self):
-        # if self.ctrl_name specifies the control variable during the observation
+        """Get the observation data from the observation data file.
+
+        Separate the control data from the observation data if the name of control variable is given.
+        Otherwise, the observation data is the entire data in the observation data file.
+        """
+        # if self.ctrl_name is given, separate the observation data into control and observation data
         if self.ctrl_name:
             keys_and_data = get_keys_and_data(self.obs_data_file)
             # separate the control data sequence from the observation data
             self.ctrl_data = keys_and_data.pop(self.ctrl_name)
             self.num_steps = len(self.ctrl_data)
-            # remove data not used by the calibration
+            # remove the data not used by Bayesian filtering
             self.num_obs = len(self.obs_names)
-            for key in keys_and_data.keys():
-                if key not in self.obs_names: keys_and_data.pop(key)
+            keys_and_data = {key: keys_and_data[key] for key in self.obs_names}
             # assign the obs_data array
             self.obs_data = np.zeros([self.num_obs, self.num_steps])
             for i, key in enumerate(self.obs_names):
                 self.obs_data[i, :] = keys_and_data[key]
         else:
             self.obs_data = np.genfromtxt(self.obs_data_file)
             # if only one observation data vector exists, reshape it with (1, num_steps)
-            if len(data) == 1:
+            if len(self.obs_data) == 1:
                 self.obs_data = self.obs_data.reshape([1, self.obs_data.shape[0]])
 
-    def get_sim_data_files(self, curr_iter: int = 0):
-        from math import floor, log
-        from glob import glob
-
-        magn = floor(log(self.num_samples, 10)) + 1
+    def get_sim_data_files(self):
+        """
+        Get the simulation data files from the simulation data directory.
+        """
+        mag = floor(log(self.num_samples, 10)) + 1
         self.sim_data_files = []
 
         for i in range(self.num_samples):
             if self.sim_data_file_ext != '.npy':
-                sim_data_file_ext = '_sim*' + self.sim_data_file_ext
+                sim_data_file_ext = '_sim' + self.sim_data_file_ext
             else:
                 sim_data_file_ext = self.sim_data_file_ext
-            file_name = self.sim_data_dir + f'/iter{curr_iter}/{self.sim_name}*' \
-                        + str(i).zfill(magn) + '*' + sim_data_file_ext
+            file_name = self.sim_data_dir.rstrip('/') + f'/iter{self.curr_iter}/{self.sim_name}*Iter{self.curr_iter}*' \
+                        + str(i).zfill(mag) + '*' + sim_data_file_ext
             files = glob(file_name)
 
             if not files:
                 raise RuntimeError("No data files with name " + file_name + ' found')
-            elif len(files) > 1:
+            if len(files) > 1:
                 raise RuntimeError("Found more than one files with the name " + file_name)
             self.sim_data_files.append(files[0])
 
     def load_sim_data(self):
-        """
-        1. Read simulation data into self.model.sim_data and remove the observation data sequence
+        """Load the simulation data from the simulation data files.
+
+        The function does the following:
+        1. Load simulation data into an IO dynamic system object
         2. Check if parameter values read from the table matches those used to creat the simulation data
         """
         self.sim_data = np.zeros([self.num_samples, self.num_obs, self.num_steps])
-        for i, f in enumerate(self.sim_data_files):
+        for i, sim_data_file in enumerate(self.sim_data_files):
             if self.sim_data_file_ext != '.npy':
-                data = get_keys_and_data(f)
-                param_data = np.genfromtxt(f.split('_sim')[0] + f'_param{self.sim_data_file_ext}')
-                for j, key in enumerate(self.param_names):
-                    data[key] = param_data[j]
+                data = get_keys_and_data(sim_data_file)
+                param_data = get_keys_and_data(sim_data_file.split('_sim')[0] + f'_param{self.sim_data_file_ext}')
+                for key in self.param_names:
+                    data[key] = param_data[key][0]
             else:
-                data = np.load(f, allow_pickle=True).item()
+                data = np.load(sim_data_file, allow_pickle=True).item()
 
             for j, key in enumerate(self.obs_names):
                 self.sim_data[i, j, :] = data[key]
 
-            params = [data[key] for key in self.param_names]
-            if not (np.abs((params - self.param_data[i, :])
-                           / self.param_data[i, :] < 1e-5).all()):
-                raise RuntimeError(
-                    "Parameters [" + ", ".join(
-                        ["%s" % v for v in self.param_data[i, :]])
-                    + '] vs [' + \
-                    ", ".join("%s" % v for v in params) + \
-                    f"] from the simulation data file {f} and the parameter table do not match")
+            params = np.array([data[key] for key in self.param_names])
+            np.testing.assert_allclose(params, self.param_data[i, :], rtol=1e-5)
 
-    def load_param_data(self, curr_iter: int = 0):
+    def load_param_data(self):
         """
-        Load parameter data from a table written in a txt file
+        Load parameter data from a table written in a text file.
         """
-        import os
-        from glob import glob
-
         if os.path.exists(self.param_data_file):
-            # we assumes parameter data in the last columns.
+            # we assume parameter data are always in the last columns.
             self.param_data = np.genfromtxt(self.param_data_file, comments='!')[:, -self.num_params:]
             self.num_samples = self.param_data.shape[0]
         else:
-            # get all simulation data files
-            files = glob(self.sim_data_dir + f'/iter{curr_iter}/{self.sim_name}*{self.sim_data_file_ext}')
+            # if param_data_file does not exit, get parameter data from text files
+            files = glob(self.sim_data_dir + f'/iter{self.curr_iter}/{self.sim_name}*_param*{self.sim_data_file_ext}')
             self.num_samples = len(files)
-            self.sim_data_files = sorted(files)
-            self.param_data = np.zeros([self.num_samples, self.num_params])
-            for i, f in enumerate(self.sim_data_files):
-                data = np.load(f, allow_pickle=True).item()
-                params = [data[key] for key in self.param_names]
-                self.param_data[i, :] = params
-
-    def run(self, **kwargs):
-        """This function runs the callback function"""
-
-        if self.callback is None:
-            raise ValueError("No callback function defined")
+            # if the number of files found is non-zero
+            if self.num_samples != 0:
+                self.sim_data_files = sorted(files)
+                self.param_data = np.zeros([self.num_samples, self.num_params])
+                for i, sim_data_file in enumerate(self.sim_data_files):
+                    if self.sim_data_file_ext == '.npy':
+                        data = np.load(sim_data_file, allow_pickle=True).item()
+                    else:
+                        data = get_keys_and_data(sim_data_file)
+                    params = [data[key][0] for key in self.param_names]
+                    self.param_data[i, :] = params
+            else:
+                raise RuntimeError(f'No data found for iteration {self.curr_iter}')
 
+    def set_up_sim_dir(self):
+        """
+        Create a directory to store simulation data and write the parameter data into a text file
+        """
         # create a directory to store simulation data
-        import os
-        from glob import glob
-        curr_iter = kwargs['curr_iter']
-        sim_data_sub_dir = f'{self.sim_data_dir}/iter{curr_iter}'
-        if not os.path.exists(sim_data_sub_dir):
-            os.makedirs(sim_data_sub_dir)
-        else:
-            input(f'Removing existing simulation data in {sim_data_sub_dir}?\n')
-            files = glob(sim_data_sub_dir + '/*')
-            for f in files: os.remove(f)
+        sim_data_dir = self.sim_data_dir.rstrip('/')
+        sim_data_sub_dir = f'{sim_data_dir}/iter{self.curr_iter}'
+        self.sim_data_sub_dir = sim_data_sub_dir
+        os.makedirs(sim_data_sub_dir)
+
+        # write the parameter data into a text file
+        self.write_params_to_table()
 
-        # write the parameter table to a text file
-        self.write_to_table(curr_iter)
+    def move_data_to_sim_dir(self):
+        """
+        Move simulation data files and corresponding parameter table into the directory defined per iteration
+        """
+        # move simulation data files and corresponding parameter table into the directory defined per iteration
+        files = glob(f'{os.getcwd()}/{self.sim_name}_Iter{self.curr_iter}*{self.sim_data_file_ext}')
+        for file in files:
+            f_name = os.path.relpath(file, os.getcwd())
+            os.replace(f'{file}', f'{self.sim_data_sub_dir}/{f_name}')
 
-        # run the callback function
-        self.callback(self, **kwargs)
+        # redefine the parameter data file since its location is changed
+        self.param_data_file = f'{self.sim_data_sub_dir}/' + os.path.relpath(self.param_data_file, os.getcwd())
 
-        # move simulation data files into the directory per iteration
-        files = glob(f'{self.sim_name}_Iter{curr_iter}*{self.sim_data_file_ext}')
-        for f in files: os.replace(f'./{f}', f'./{sim_data_sub_dir}/{f}')
+    def write_params_to_table(self):
+        """Write the parameter data into a text file.
 
-    def write_to_table(self, curr_iter: int):
+        :return param_data_file: The name of the parameter data file
+        """
         self.param_data_file = write_to_table(
-            f'{self.sim_data_dir}/iter{curr_iter}/{self.sim_name}', self.param_data, self.param_names, curr_iter)
+            self.sim_name,
+            self.param_data,
+            self.param_names,
+            self.curr_iter)
+
+    def backup_sim_data(self):
+        """Backup simulation data files to a backup directory."""
+        # create a directory to store simulation data
+        if os.path.exists(self.sim_data_dir):
+            print(f'Moving existing simulation data in {self.sim_data_dir} into a backup directory\n')
+            timestamp = os.path.getmtime(self.sim_data_dir)
+            formatted_time = datetime.fromtimestamp(timestamp).strftime('%Y_%m_%d_%H_%M_%S')
+            path = self.sim_data_dir.rstrip('/')
+            backup_dir = f'{path}_backup_{formatted_time}'
+            os.makedirs(backup_dir, exist_ok=True)
+            os.rename(self.sim_data_dir, backup_dir)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `grainlearning-2.0.1/grainlearning/tools.py` & `grainlearning-2.0.3/grainlearning/tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,105 +1,107 @@
-""" Author: Hongyang Cheng <chyalexcheng@gmail.com>
-     A collection of all kins of helper functions (IO, plotting, ...)
 """
-
-from math import *
-import sys, os
+This module contains tools for the GrainLearning project.
+"""
+import sys
+import os
+import math
+import subprocess
+from typing import List, Callable
 import numpy as np
-import matplotlib.pylab as plt
-
 from sklearn.mixture import BayesianGaussianMixture
-
-import subprocess
-from typing import Type, List, Callable, Tuple
+from scipy.spatial import Voronoi, ConvexHull
 
 
-def startSimulations(platform, software, tableName, fileName):
-    # platform desktop, aws or rcg    # software so far only yade
-    argument = tableName + " " + fileName
-    if platform == 'desktop':
-        # Definition where shell script can be found
-        path_to_shell = os.getcwd() + '/platform_shells/desktop'
-        if software == 'yade':
-            command = 'sh ' + path_to_shell + '/yadeDesktop.sh' + " " + argument
-            subprocess.call(command, shell=True)
-        else:
-            print(Fore.RED + "Chosen 'software' has not been implemented yet. Check 'startSimulations()' in 'tools.py'")
-            sys.exit
-
-    elif platform == 'aws':
-        path_to_shell = os.getcwd() + '/platform_shells/aws'
-        if software == 'yade':
-            command = 'sh ' + path_to_shell + '/yadeAWS.sh' + " " + argument
-            subprocess.call(command, shell=True)
-        else:
-            print(Fore.RED + "Chosen 'software' has not been implemented yet. Check 'startSimulations()' in 'tools.py'")
-            sys.exit
-
-    elif platform == 'rcg':
-        path_to_shell = os.getcwd() + '/platform_shells/rcg'
-        if software == 'yade':
-            command = 'sh ' + path_to_shell + '/yadeRCG.sh' + " " + argument
-            subprocess.call(command, shell=True)
-        else:
-            print(Fore.RED + "Chosen 'software' has not been implemented yet. Check 'startSimulations()' in 'tools.py'")
-            sys.exit
-    else:
-        print('Exit code. Hardware for yade simulations not properly defined')
-        quit()
+# def startSimulations(platform, software, tableName, fileName):
+#     # platform desktop, aws or rcg    # software so far only yade
+#     argument = tableName + " " + fileName
+#     if platform == 'desktop':
+#         # Definition where shell script can be found
+#         path_to_shell = os.getcwd() + '/platform_shells/desktop'
+#         if software == 'yade':
+#             command = 'sh ' + path_to_shell + '/yadeDesktop.sh' + " " + argument
+#             subprocess.call(command, shell=True)
+#         else:
+#             print(Fore.RED + "Chosen 'software' has not been implemented yet. Check 'startSimulations()' in 'tools.py'")
+#             sys.exit
+#
+#     elif platform == 'aws':
+#         path_to_shell = os.getcwd() + '/platform_shells/aws'
+#         if software == 'yade':
+#             command = 'sh ' + path_to_shell + '/yadeAWS.sh' + " " + argument
+#             subprocess.call(command, shell=True)
+#         else:
+#             print(Fore.RED + "Chosen 'software' has not been implemented yet. Check 'startSimulations()' in 'tools.py'")
+#             sys.exit
+#
+#     elif platform == 'rcg':
+#         path_to_shell = os.getcwd() + '/platform_shells/rcg'
+#         if software == 'yade':
+#             command = 'sh ' + path_to_shell + '/yadeRCG.sh' + " " + argument
+#             subprocess.call(command, shell=True)
+#         else:
+#             print(Fore.RED + "Chosen 'software' has not been implemented yet. Check 'startSimulations()' in 'tools.py'")
+#             sys.exit
+#     else:
+#         print('Exit code. Hardware for yade simulations not properly defined')
+#         quit()
 
 
 def write_to_table(sim_name, table, names, curr_iter=0, threads=8):
     """
     write parameter samples into a text file
+
+    :param sim_name: string
+    :param table: numpy array
+    :param names: list of strings
+    :param curr_iter: int
+    :param threads: int
+    :return: string
     """
 
     # Computation of decimal number for unique key
-    table_file_name = f'{sim_name}_Iter{curr_iter}_samples.txt'
+    table_file_name = f'{os.getcwd()}/{sim_name}_Iter{curr_iter}_Samples.txt'
 
-    fout = open(table_file_name, 'w')
-    num, dim = table.shape
-    magn = floor(log(num, 10)) + 1
-    fout.write(' '.join(['!OMP_NUM_THREADS', 'description', 'key'] + names + ['\n']))
-    for j in range(num):
-        description = 'Iter' + str(curr_iter) + '-Sample' + str(j).zfill(magn)
-        fout.write(' '.join(
-            ['%2i' % threads] + [description] + ['%9i' % j] + ['%20.10e' % table[j][i] for i in range(dim)] + ['\n']))
-    fout.close()
+    with open(table_file_name, 'w') as f_out:
+        num, dim = table.shape
+        mag = math.floor(math.log(num, 10)) + 1
+        f_out.write(' '.join(['!OMP_NUM_THREADS', 'description', 'key'] + names + ['\n']))
+        for j in range(num):
+            description = f'{sim_name}_Iter' + str(curr_iter) + '_Sample' + str(j).zfill(mag)
+            f_out.write(' '.join(
+                [f'{threads:2d}'] + [description] +
+                [f'{j:9d}'] + [f'{table[j][i]:20.10e}' for i in range(dim)] + ['\n']))
     return table_file_name
 
 
-def get_keys_and_data(fileName, delimiters=['\t', ' ', ',']):
+def get_keys_and_data(file_name: str, delimiters=None):
     """
     Get keys and corresponding data sequence from a text file
 
-    :param fileName: string
-
+    :param file_name: string
+    :param delimiters: list of strings, default = ['\t', ' ', ',']
     :return: keys_and_data: dictionary
     """
-    data = np.genfromtxt(fileName)
-
-    try:
-        ncols = data.shape[1]
-    except IndexError:
-        nrows = data.shape[0]
-        ncols = 1
-        data = data.reshape([nrows, 1])
-
-    fopen = open(fileName, 'r')
-    first_line = fopen.read().splitlines()[0]
-    for d in delimiters:
-        keys = first_line.split(d)
-        # remove # in the header line
-        if '#' in keys: keys.remove('#')
-        # remove empty strings from the list
-        keys = list(filter(None, keys))
-        if len(keys) == ncols: break
+    if delimiters is None:
+        delimiters = ['\t', ' ', ',']
+    data = np.genfromtxt(file_name, ndmin=2)
+
+    with open(file_name, 'r') as f_open:
+        first_line = f_open.read().splitlines()[0]
+        for d in delimiters:
+            keys = first_line.split(d)
+            # remove # in the header line
+            if '#' in keys:
+                keys.remove('#')
+            # remove empty strings from the list
+            keys = list(filter(None, keys))
+            if len(keys) == data.shape[1]:
+                break
 
-    # store data in a dictory
+    # store data in a dictionary
     keys_and_data = {}
     for key in keys:
         if '#' in key:
             key_no_hash = key.split(' ')[-1]
         else:
             key_no_hash = key
         keys_and_data[key_no_hash] = data[:, keys.index(key)]
@@ -111,28 +113,28 @@
     proposal: np.ndarray,
     param_data: np.ndarray,
     num: int,
     max_num_components: int,
     prior_weight: float,
     cov_type: str = "full",
     resample_to_unweighted: Callable = None,
-    param_mins: List[float] = None,
-    param_maxs: List[float] = None,
+    param_min: List[float] = None,
+    param_max: List[float] = None,
     n_init=1,
     tol=0.001,
     max_iter=100,
     seed=None,
 ) -> np.ndarray:
     """
     Resample parameters using a variational Gaussian mixture model
 
-    :param proposal: ndarray of shape model.num_samples
+    :param proposal: ndarray of shape system.num_samples
         proposal probability distribution associated to the current parameter data
 
-    :param param_data: ndarray of shape (model.num_samples, model.num_params)
+    :param param_data: ndarray of shape (system.num_samples, system.num_params)
         current parameter data
 
     :param num: int
         number of samples for the resampling
 
     :param max_num_components: int, default = num/10
 
@@ -152,22 +154,31 @@
         'diag' (each component has its own diagonal covariance matrix),
         'spherical' (each component has its own single variance).
         (https://scikit-learn.org/stable/modules/generated/sklearn.mixture.BayesianGaussianMixture.html)
 
     :param resample_to_unweighted: Callable
         Function to expand samples from weighted to unweighted
 
-    :param param_mins: list
+    :param param_min: list
         lower bound of the parameter values
 
-    :param param_maxs: list
-        uper bound of the parameter values
+    :param param_max: list
+        upper bound of the parameter values
 
     :param seed: int
-        random generation seed, defaults to None
+        random generation random_state, defaults to None
+
+    :param n_init: int, default = 1
+        Number of initializations to perform. The best results are kept.
+
+    :param tol: float, default = 0.001
+        Convergence threshold. EM iterations will stop when the lower bound average gain is below this threshold.
+
+    :param max_iter: int, default = 100
+        Number of EM iterations to perform.
 
     :return:
         new_param_data: ndarray, parameter samples for the next iteration
 
         gmm: BayesianGaussianMixture
             A variational Gaussian mixture model trained with current parameter samples and proposal probabilities
     """
@@ -198,67 +209,85 @@
     new_param_data *= max_params
 
     return new_param_data, gmm
 
 
 def get_pool(mpi=False, threads=1):
     """
-    Create a thread pool for paralleling DEM simulations within GrainLearning
+    Create a thread pool for paralleling model evaluations within GrainLearning
 
-    :param mpi: bool, default=False
+    TODO improve the scheduler for running simulation instances in parallel
+    1. On Desktop: use multiprocessing
+    2. On HPC: use MPI or multiprocessing
+    3. On Cloud (e.g. AWS)
 
+    :param mpi: bool, default=False
     :param threads: int, default=1
     """
-    if mpi:  # using MPI
-        from mpipool import MPIPool
-        pool = MPIPool()
-        pool.start()
-        if not pool.is_master():
-            sys.exit(0)
-    elif threads > 1:  # using multiprocessing
+    # if mpi:  # using MPI
+    #     from mpipool import MPIPool
+    #     pool = MPIPool()
+    #     pool.start()
+    #     if not pool.is_master():
+    #         sys.exit(0)
+    if threads > 1:  # using multiprocessing
         from multiprocessing import Pool
         pool = Pool(processes=threads, maxtasksperchild=10)
-    else:
+    if not mpi and threads == 1:
         raise RuntimeError("Wrong arguments: either mpi=True or threads>1.")
     return pool
 
 
 def unweighted_resample(weights, expand_num=10):
-    # take int(N*w) copies of each weight, which ensures particles with the same weight are drawn uniformly
-    N = len(weights) * expand_num
-    num_copies = (np.floor(N * np.asarray(weights))).astype(int)
+    """
+    Resample from the weighted samples to unweighted samples
+
+    Take int(N*w) copies of each weight, which ensures particles with the same weight are drawn uniformly
+    :param weights: ndarray of shape (N,)
+    :param expand_num: int, default=10
+    :return: ndarray of shape (N*expand_num,)
+    """
+    n = len(weights) * expand_num
+    num_copies = (np.floor(n * np.asarray(weights))).astype(int)
     indexes = np.zeros(sum(num_copies), 'i')
     k = 0
     for i in range(len(weights)):
         for _ in range(num_copies[i]):  # make n copies
             indexes[k] = i
             k += 1
     return indexes
 
 
 def residual_resample(weights, expand_num=10):
-    N = len(weights) * expand_num
-    indexes = np.zeros(N, 'i')
+    """
+    Resample from the weighted samples to unweighted samples using the residual resampling algorithm
+
+    :param weights: ndarray of shape (N,)
+    :param expand_num: int, default=10
+    :return: ndarray of shape (N*expand_num,)
+    """
+    n = len(weights) * expand_num
+    indexes = np.zeros(n, 'i')
 
     # take int(N*w) copies of each weight, which ensures particles with the
     # same weight are drawn uniformly
-    num_copies = (np.floor(N * np.asarray(weights))).astype(int)
+    num_copies = (np.floor(n * np.asarray(weights))).astype(int)
     k = 0
     for i in range(len(weights)):
         for _ in range(num_copies[i]):  # make n copies
             indexes[k] = i
             k += 1
 
     # use multinormal resample on the residual to fill up the rest. This
     # maximizes the variance of the samples
     residual = weights - num_copies  # get fractional part
     residual /= sum(residual)  # normalize
     cumulative_sum = np.cumsum(residual)
     cumulative_sum[-1] = 1.  # avoid round-off errors: ensures sum is exactly one
-    indexes[k:N] = np.searchsorted(cumulative_sum, np.random.random(N - k))
+    indexes[k:n] = np.searchsorted(cumulative_sum, np.random.random(n - k))
 
     return indexes
 
 
 def stratified_resample(weights, expand_num=10):
     """ Performs the stratified resampling algorithm used by particle filters.
     This algorithms aims to make selections relatively uniformly across the
@@ -272,22 +301,22 @@
     Returns
     -------
     indexes : ndarray of ints
         array of indexes into the weights defining the resample. i.e. the
         index of the zeroth resample is indexes[0], etc.
     """
 
-    N = len(weights)
+    n = len(weights)
     # make N subdivisions, and chose a random position within each one
-    positions = (np.random.random(N) + range(N)) / N
+    positions = (np.random.random(n) + range(n)) / n
 
-    indexes = np.zeros(N, 'i')
+    indexes = np.zeros(n, 'i')
     cumulative_sum = np.cumsum(weights)
     i, j = 0, 0
-    while i < N:
+    while i < n:
         if positions[i] < cumulative_sum[j]:
             indexes[i] = j
             i += 1
         else:
             j += 1
     return indexes
 
@@ -303,23 +332,23 @@
         list of weights as floats
     Returns
     -------
     indexes : ndarray of ints
         array of indexes into the weights defining the resample. i.e. the
         index of the zeroth resample is indexes[0], etc.
     """
-    N = len(weights)
+    n = len(weights)
 
     # make N subdivisions, and choose positions with a consistent random offset
-    positions = (np.random.random() + np.arange(N)) / N
+    positions = (np.random.random() + np.arange(n)) / n
 
-    indexes = np.zeros(N, 'i')
+    indexes = np.zeros(n, 'i')
     cumulative_sum = np.cumsum(weights)
     i, j = 0, 0
-    while i < N:
+    while i < n:
         if positions[i] < cumulative_sum[j]:
             indexes[i] = j
             i += 1
         else:
             j += 1
     return indexes
 
@@ -343,126 +372,130 @@
     """
     cumulative_sum = np.cumsum(weights)
     cumulative_sum[-1] = 1.  # avoid round-off errors: ensures sum is exactly one
     return np.searchsorted(cumulative_sum, np.random.random(len(weights) * expand_num))
 
 
 def voronoi_vols(samples: np.ndarray):
-    from scipy.spatial import Voronoi, ConvexHull
+    """Compute the volumes of the Voronoi cells associated with a set of points.
+
+    :param samples: ndarray of shape (N, D)
+    :return: ndarray of shape (N,)
+    """
     v = Voronoi(samples)
     vol = np.zeros(v.npoints)
     for i, reg_num in enumerate(v.point_region):
         indices = v.regions[reg_num]
         if -1 in indices:
             vol[i] = -1.0
         else:
             vol[i] = ConvexHull(v.vertices[indices]).volume
     return vol
 
 
-def plot_param_stats(fig_name, param_names, means, covs, savefig=0):
+def plot_param_stats(fig_name, param_names, means, covs, save_fig=0):
     """
     Plot the posterior means and coefficients of variation of the model parameters over time.
     :param fig_name: string
     :param param_names: parameter names
     :param means: ndarray
     :param covs: ndarray
-    :param savefig: bool defaults to False
+    :param save_fig: bool defaults to False
     """
+    import matplotlib.pylab as plt
     num = len(param_names)
-    ncols = int(np.ceil(num / 2))
+    n_cols = int(np.ceil(num / 2))
     plt.figure('Posterior means of the parameters')
     for i in range(num):
-        plt.subplot(2, ncols, i + 1)
+        plt.subplot(2, n_cols, i + 1)
         plt.plot(means[:, i])
         plt.xlabel("'Time' step")
-        plt.ylabel(r'$|' + param_names[i] + r'|$')
+        plt.ylabel(f'Mean of {param_names[i]}')
         plt.grid(True)
     plt.tight_layout()
-    if savefig:
+    if save_fig:
         plt.savefig(f'{fig_name}_param_means.png')
-    else:
-        plt.show()
-    plt.close()
 
     plt.figure('Posterior coefficients of variance of the parameters')
     for i in range(num):
-        plt.subplot(2, ncols, i + 1)
+        plt.subplot(2, n_cols, i + 1)
         plt.plot(covs[:, i])
         plt.xlabel("'Time' step")
-        plt.ylabel(r'$COV(' + param_names[i] + ')$')
+        plt.ylabel(f'Coefficient of variation of {param_names[i]}')
         plt.grid(True)
     plt.tight_layout()
-    if savefig:
+    if save_fig:
         plt.savefig(f'{fig_name}_param_covs.png')
-    else:
-        plt.show()
-    plt.close()
 
 
-def plot_posterior(fig_name, param_names, param_data, posterior, savefig=0):
+def plot_posterior(fig_name, param_names, param_data, posterior, save_fig=0):
     """
     Plot the evolution of discrete posterior distribution over the parameters in time.
     :param fig_name: string
     :param param_names: parameter names
     :param param_data: ndarray
     :param posterior: ndarray
-    :param savefig: bool defaults to False
+    :param save_fig: bool defaults to False
     """
+    try:
+        import matplotlib.pylab as plt
+    except ImportError:
+        print(
+            'matplotlib is not installed, cannot plot posterior distribution. Please install with grainlearning[plot]')
     num_steps = posterior.shape[0]
     for i, name in enumerate(param_names):
         plt.figure(f'Posterior distribution of {name}')
         for j in range(6):
             plt.subplot(2, 3, j + 1)
             plt.plot(param_data[:, i], posterior[int(num_steps * (j + 1) / 6 - 1), :], 'o')
-            plt.title("'Time' step No.%3i " % (int(num_steps * (j + 1) / 6 - 1)))
+            plt.title(f"'Time' step {int(num_steps * (j + 1) / 6 - 1):3d} ")
             plt.xlabel(r'$' + name + '$')
-            plt.ylabel('Posterior distribution')
+            plt.ylabel('Posterior probability mass')
             plt.grid(True)
         plt.tight_layout()
-        if savefig:
+        if save_fig:
             plt.savefig(f'{fig_name}_posterior_{name}.png')
-        else:
-            plt.show()
-        plt.close()
 
 
-def plot_param_data(fig_name, param_names, param_data_list, savefig=0):
+def plot_param_data(fig_name, param_names, param_data_list, save_fig=0):
+    import matplotlib.pylab as plt
+    import seaborn as sns
+    flare_cmap = sns.color_palette("flare", as_cmap=True)
     num = len(param_names)
-    ncols = int(np.ceil(num / 2))
+    n_cols = int(np.ceil(num / 2))
     num = num - 1
     num_iter = len(param_data_list)
     plt.figure('Resampling the parameter space')
     for j in range(num):
-        plt.subplot(2, ncols, j + 1)
+        plt.subplot(2, n_cols, j + 1)
         for i in range(num_iter):
-            plt.plot(param_data_list[i][:, j], param_data_list[i][:, j + 1], 'o', label='iterNo. %.2i' % i)
+            plt.scatter(param_data_list[i][:, j], param_data_list[i][:, j + 1], edgecolors='white',
+                        color=flare_cmap(i / (num_iter - 1)), label=f'Iter No. {i:d}')
             plt.xlabel(r'$' + param_names[j] + '$')
             plt.ylabel(r'$' + param_names[j + 1] + '$')
             plt.legend()
         plt.legend()
         plt.tight_layout()
-    if savefig:
+    if save_fig:
         plt.savefig(f'{fig_name}_param_space.png')
-    else:
-        plt.show()
 
 
-def plot_obs_and_sim(fig_name, ctrl_name, obs_names, ctrl_data, obs_data, sim_data, posteriors, savefig=0):
+def plot_obs_and_sim(fig_name, ctrl_name, obs_names, ctrl_data, obs_data, sim_data, posteriors, save_fig=0):
     """
     Plot the ensemble prediction, observation data, and top three best-fits
     :param fig_name: string
     :param ctrl_name: name of the control variable
     :param obs_names: names of the observables
     :param ctrl_data: ndarray
     :param obs_data: ndarray
     :param sim_data: ndarray
     :param posterior: ndarray
-    :param savefig: bool defaults to False
+    :param save_fig: bool defaults to False
     """
+    import matplotlib.pylab as plt
     ensemble_mean = np.einsum('ijk, ki->jk', sim_data, posteriors)
     ensemble_std = np.einsum('ijk, ki->jk', (sim_data - ensemble_mean) ** 2, posteriors)
     ensemble_std = np.sqrt(ensemble_std)
     num = len(obs_names)
     ncols = int(np.ceil(num / 2)) if num > 1 else 1
     plt.figure('Model prediction versus observation')
     for i in range(num):
@@ -473,26 +506,95 @@
             ensemble_mean[i, :] - 2 * ensemble_std[i, :],
             ensemble_mean[i, :] + 2 * ensemble_std[i, :],
             color='darkred',
             label='ensemble prediction'
         )
 
         for j in (-posteriors[-1, :]).argsort()[:3]:
-            plt.plot(ctrl_data, sim_data[j, i, :], label='sim No. %i' % j)
+            plt.plot(ctrl_data, sim_data[j, i, :], label=f'sim No. {j:d}')
+
+        if len(ctrl_data) < 20:
+            markevery = 1
+        else:
+            markevery = int(len(ctrl_data) / 10.)
 
         plt.plot(ctrl_data,
                  obs_data[i, :], 'ok',
                  label='obs.',
-                 markevery=int(len(ctrl_data) / 10.)
+                 markevery=markevery
                  )
 
         plt.xlabel(ctrl_name)
         plt.ylabel(obs_names[i])
         plt.legend()
         plt.grid(True)
 
     plt.tight_layout()
-    if savefig:
+    if save_fig:
         plt.savefig(f'{fig_name}_obs_and_sim.png')
-    else:
+
+
+def plot_pdf(fig_name, param_names, samples, save_fig=0):
+    """
+    Plot the posterior density function of the parameter distribution
+    :param fig_name: string
+    :param sim_name: string
+    :param param_names: list of strings containing parameter names
+    :param samples: list of ndarray of shape (num_samples, self.num_params)
+    :param save_fig: bool defaults to False
+    """
+    import seaborn as sns
+    import pandas as pd
+    import matplotlib.pylab as plt
+
+    # create a deep copy of the samples (FIXME: this is a workaround for a bug in iBF constructor)
+    new_samples = [np.copy(sample) for sample in samples]
+    # pad with NaNs to make all samples have the same length
+    max_len = int(max([len(sample) for sample in new_samples]))
+    for i in range(len(new_samples)):
+        new_samples[i] = np.pad(new_samples[i], ((0, max_len - len(new_samples[i])), (0, 0)), 'constant',
+                                constant_values=np.nan)
+    # fill the third dimension with iteration number
+    stacked_samples = np.vstack([new_samples[i] for i in range(len(new_samples))])
+    third_dim_indices = np.repeat(np.arange(len(new_samples)), new_samples[0].shape[0])
+    new_samples = np.hstack([stacked_samples, third_dim_indices[:, np.newaxis]])
+
+    # convert the array into a pandas dataframe
+    new_names = param_names + ['Iter']
+    df = pd.DataFrame(new_samples, columns=new_names)
+
+    # plot the parameter distribution in a scatter plot
+    fig = sns.PairGrid(df, diag_sharey=False, hue="Iter", palette='flare')
+    fig.map_upper(sns.scatterplot, s=15)
+    fig.map_lower(sns.kdeplot, thresh=1e-3, levels=5)
+    fig.map_diag(sns.kdeplot, lw=2)
+    fig.add_legend(loc='upper right')
+    fig.fig.canvas.manager.set_window_title('Estimated posterior probability density function')
+
+    fig.tight_layout()
+    if save_fig:
+        fig.savefig(f'{fig_name}_scatterplot.png')
+
+
+def close_plots(save_fig=0):
+    import matplotlib.pylab as plt
+    if not save_fig:
         plt.show()
-    plt.close()
+    plt.close('all')
+
+
+def write_dict_to_file(data, file_name):
+    """Write a python dictionary data into a text file
+
+    :param data: dictionary, keys are the names of the columns, values are the data
+    :param file_name: string, name of the file
+    """
+    with open(file_name, 'w') as f:
+        keys = data.keys()
+        f.write('# ' + ' '.join(keys) + '\n')
+        # check if data[list(keys)[0]] is a list
+        if isinstance(data[list(keys)[0]], list):
+            num = len(data[list(keys)[0]])
+            for i in range(num):
+                f.write(' '.join([str(data[key][i]) for key in keys]) + '\n')
+        else:
+            f.write(' '.join([str(data[key]) for key in keys]) + '\n')
```


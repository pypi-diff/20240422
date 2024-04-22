# Comparing `tmp/mace_models-0.1.2.tar.gz` & `tmp/mace_models-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mace_models-0.1.2.tar", max compression
+gzip compressed data, was "mace_models-0.1.3.tar", max compression
```

## Comparing `mace_models-0.1.2.tar` & `mace_models-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2024-01-05 14:15:28.881262 mace_models-0.1.2/LICENSE
--rw-r--r--   0        0        0     2987 2024-01-05 15:55:40.965419 mace_models-0.1.2/README.md
--rw-r--r--   0        0        0     2713 2024-01-05 15:52:00.877200 mace_models-0.1.2/mace_models/__init__.py
--rw-r--r--   0        0        0      644 2024-01-05 15:52:00.878705 mace_models-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3620 1970-01-01 00:00:00.000000 mace_models-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-01-05 14:15:28.881262 mace_models-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4724 2024-04-22 05:46:24.268551 mace_models-0.1.3/README.md
+-rw-r--r--   0        0        0     2720 2024-04-22 05:41:52.825171 mace_models-0.1.3/mace_models/__init__.py
+-rw-r--r--   0        0        0      613 2024-04-22 05:44:44.682057 mace_models-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5357 1970-01-01 00:00:00.000000 mace_models-0.1.3/PKG-INFO
```

### Comparing `mace_models-0.1.2/LICENSE` & `mace_models-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mace_models-0.1.2/mace_models/__init__.py` & `mace_models-0.1.3/mace_models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             if kwargs.get("device", None) is None:
                 return torch.load(f)
             else:
                 model = torch.load(f, map_location=kwargs["device"])
                 model.to(kwargs["device"])
                 return model
 
-    def get_calculator(self, device=None, dtype="float32") -> MACECalculator:
+    def get_calculator(self, device=None, dtype="float32", **kwargs) -> MACECalculator:
         """Return the ASE calculator."""
         if device is None:
             device = "cuda" if torch.cuda.is_available() else "cpu"
 
         with self.state.use_tmp_path():
             return MACECalculator(
                 model_paths=self.model_path,
@@ -70,15 +70,15 @@
     def get_atoms(self):
         with self.state.fs.open(self.data_path, "r") as f:
             return aio.read(f, format="extxyz", index=":")
 
 
 @functools.wraps(LoadModel.from_rev)
 def load(
-    name: str = "medium_spice",
+    name: str = "MACE-MP-0",
     remote: str = "https://github.com/RokasEl/MACE-Models",
     rev: str = None,
 ) -> LoadModel:
     """Load a pre-trained MACE model.
 
     Parameters
     ----------
```

### Comparing `mace_models-0.1.2/pyproject.toml` & `mace_models-0.1.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [tool.poetry]
 name = "mace-models"
-version = "0.1.2"
+version = "0.1.3"
 description = "Access pre-trained MACE models"
 authors = ["Rokas Elijošius <re344@cam.ac.uk>", "Fabian Zills <fzills@icp.uni-stuttgart.de>"]
 readme = "README.md"
 packages = [{include = "mace_models"}]
 
 [tool.poetry.urls]
 repository = "https://github.com/RokasEl/MACE-Models"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-zntrack = "^0.7.2"
+zntrack = "^0.7"
 dvc-s3 = "^3"
 ase = "^3.22.1"
-pytest = "^7.4.4"
-
-[tool.poetry.group.mace.dependencies]
-mace = {git = "https://github.com/ACEsuit/mace"}
+mace-torch = "^0.3.4"
 
+[tool.poetry.group.dev.dependencies]
+pytest = "^8.1.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.ruff]
```


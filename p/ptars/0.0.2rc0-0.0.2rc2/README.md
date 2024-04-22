# Comparing `tmp/ptars-0.0.2rc0.tar.gz` & `tmp/ptars-0.0.2rc2.tar.gz`

## Comparing `ptars-0.0.2rc0.tar` & `ptars-0.0.2rc2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      828 1970-01-01 00:00:00.000000 ptars-0.0.2rc0/Cargo.toml
--rw-r--r--   0     1001      127     1124 2024-04-09 17:47:57.000000 ptars-0.0.2rc0/DEVELOPMENT.md
--rw-r--r--   0     1001      127    11357 2024-04-09 17:47:57.000000 ptars-0.0.2rc0/LICENSE
--rw-r--r--   0     1001      127      701 2024-04-09 17:47:57.000000 ptars-0.0.2rc0/Makefile
--rw-r--r--   0     1001      127     2620 2024-04-09 17:47:57.000000 ptars-0.0.2rc0/README.md
--rw-r--r--   0     1001      127   170098 2024-04-09 17:47:57.000000 ptars-0.0.2rc0/poetry.lock
--rw-r--r--   0     1001      127     7016 2024-04-09 17:47:57.000000 ptars-0.0.2rc0/protos/ptars_protos/bench.proto
--rw-r--r--   0     1001      127      439 2024-04-09 17:47:57.000000 ptars-0.0.2rc0/protos/ptars_protos/imported.proto
--rw-r--r--   0     1001      127      427 2024-04-09 17:47:57.000000 ptars-0.0.2rc0/protos/ptars_protos/importer.proto
--rw-r--r--   0     1001      127     3465 2024-04-09 17:47:57.000000 ptars-0.0.2rc0/protos/ptars_protos/simple.proto
--rw-r--r--   0     1001      127        0 2024-04-09 17:47:57.000000 ptars-0.0.2rc0/python/__init__.py
--rw-r--r--   0     1001      127       66 2024-04-09 17:47:57.000000 ptars-0.0.2rc0/python/ptars/__init__.py
--rw-r--r--   0     1001      127     2332 2024-04-09 17:47:57.000000 ptars-0.0.2rc0/python/ptars/internal.py
--rw-r--r--   0     1001      127     1382 2024-04-09 17:47:57.000000 ptars-0.0.2rc0/scripts/protoc.py
--rw-r--r--   0     1001      127    24603 2024-04-09 17:47:57.000000 ptars-0.0.2rc0/src/lib.rs
--rw-r--r--   0     1001      127    30657 2024-04-09 17:47:57.000000 ptars-0.0.2rc0/Cargo.lock
--rw-r--r--   0     1001      127     2219 2024-04-09 17:47:57.000000 ptars-0.0.2rc0/pyproject.toml
--rw-r--r--   0        0        0     3196 1970-01-01 00:00:00.000000 ptars-0.0.2rc0/PKG-INFO
+-rw-r--r--   0        0        0      828 1970-01-01 00:00:00.000000 ptars-0.0.2rc2/Cargo.toml
+-rw-r--r--   0     1001      127     1446 2024-04-22 07:16:10.000000 ptars-0.0.2rc2/DEVELOPMENT.md
+-rw-r--r--   0     1001      127    11357 2024-04-22 07:16:10.000000 ptars-0.0.2rc2/LICENSE
+-rw-r--r--   0     1001      127      701 2024-04-22 07:16:10.000000 ptars-0.0.2rc2/Makefile
+-rw-r--r--   0     1001      127     2620 2024-04-22 07:16:10.000000 ptars-0.0.2rc2/README.md
+-rw-r--r--   0     1001      127   170098 2024-04-22 07:16:10.000000 ptars-0.0.2rc2/poetry.lock
+-rw-r--r--   0     1001      127     7016 2024-04-22 07:16:10.000000 ptars-0.0.2rc2/protos/ptars_protos/bench.proto
+-rw-r--r--   0     1001      127      439 2024-04-22 07:16:10.000000 ptars-0.0.2rc2/protos/ptars_protos/imported.proto
+-rw-r--r--   0     1001      127      427 2024-04-22 07:16:10.000000 ptars-0.0.2rc2/protos/ptars_protos/importer.proto
+-rw-r--r--   0     1001      127     3465 2024-04-22 07:16:10.000000 ptars-0.0.2rc2/protos/ptars_protos/simple.proto
+-rw-r--r--   0     1001      127        0 2024-04-22 07:16:10.000000 ptars-0.0.2rc2/python/__init__.py
+-rw-r--r--   0     1001      127       66 2024-04-22 07:16:10.000000 ptars-0.0.2rc2/python/ptars/__init__.py
+-rw-r--r--   0     1001      127     2332 2024-04-22 07:16:10.000000 ptars-0.0.2rc2/python/ptars/internal.py
+-rw-r--r--   0     1001      127     1382 2024-04-22 07:16:10.000000 ptars-0.0.2rc2/scripts/protoc.py
+-rw-r--r--   0     1001      127    24937 2024-04-22 07:16:10.000000 ptars-0.0.2rc2/src/lib.rs
+-rw-r--r--   0     1001      127    30887 2024-04-22 07:16:10.000000 ptars-0.0.2rc2/Cargo.lock
+-rw-r--r--   0     1001      127     2219 2024-04-22 07:16:10.000000 ptars-0.0.2rc2/pyproject.toml
+-rw-r--r--   0        0        0     3196 1970-01-01 00:00:00.000000 ptars-0.0.2rc2/PKG-INFO
```

### Comparing `ptars-0.0.2rc0/Cargo.toml` & `ptars-0.0.2rc2/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ptarslib"
-version = "0.0.2-rc0"
+version = "0.0.2-rc2"
 authors = ["0x26res <0x26res@gmail.net>"]
 edition = "2021"
 description = "Fast python conversion from protobuf to arrow using rust"
 homepage = "https://github.com/0x26res/ptars"
 repository = "https://github.com/0x26res/ptars"
 readme = "README.md"
 license = "Apache-2.0"
@@ -23,12 +23,12 @@
 name = "ptars"
 
 [dependencies]
 pyo3 = { version = "0.20.3" }
 arrow = { version = "51.0.0", features = ["pyarrow"] }
 arrow-array = { version = "51.0.0" }
 arrow-schema = { version = "51.0.0" }
-protobuf = { version = "3.3.0" }
-chrono = { version = "0.4.31" }
+protobuf = { version = "3.4.0" }
+chrono = { version = "0.4.38" }
 [features]
 extension-module = ["pyo3/extension-module"]
 default = ["extension-module"]
```

### Comparing `ptars-0.0.2rc0/LICENSE` & `ptars-0.0.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `ptars-0.0.2rc0/Makefile` & `ptars-0.0.2rc2/Makefile`

 * *Files identical despite different names*

### Comparing `ptars-0.0.2rc0/README.md` & `ptars-0.0.2rc2/README.md`

 * *Files identical despite different names*

### Comparing `ptars-0.0.2rc0/poetry.lock` & `ptars-0.0.2rc2/poetry.lock`

 * *Files identical despite different names*

### Comparing `ptars-0.0.2rc0/protos/ptars_protos/bench.proto` & `ptars-0.0.2rc2/protos/ptars_protos/bench.proto`

 * *Files identical despite different names*

### Comparing `ptars-0.0.2rc0/protos/ptars_protos/simple.proto` & `ptars-0.0.2rc2/protos/ptars_protos/simple.proto`

 * *Files identical despite different names*

### Comparing `ptars-0.0.2rc0/python/ptars/internal.py` & `ptars-0.0.2rc2/python/ptars/internal.py`

 * *Files identical despite different names*

### Comparing `ptars-0.0.2rc0/scripts/protoc.py` & `ptars-0.0.2rc2/scripts/protoc.py`

 * *Files identical despite different names*

### Comparing `ptars-0.0.2rc0/src/lib.rs` & `ptars-0.0.2rc2/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -561,14 +561,25 @@
         } else {
             StructArray::from(arrays)
         };
         let batch = RecordBatch::from(struct_array);
         batch.to_pyarrow(py)
     }
 
+    fn just_convert(&self, values: Vec<Vec<u8>>, _py: Python<'_>) {
+        let _unused: Vec<Box<dyn MessageDyn>> = values
+            .iter()
+            .map(|x| {
+                self.message_descriptor
+                    .parse_from_bytes(x.as_slice())
+                    .unwrap()
+            })
+            .collect();
+    }
+
     fn record_batch_to_array(&self, record_batch: &PyAny, py: Python<'_>) -> PyResult<PyObject> {
         let _arrow_record_batch = RecordBatch::from_pyarrow(record_batch);
 
         let results = BinaryBuilder::new().build();
         results.to_data().to_pyarrow(py)
     }
 }
```

### Comparing `ptars-0.0.2rc0/Cargo.lock` & `ptars-0.0.2rc2/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -302,36 +302,36 @@
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.92"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2678b2e3449475e95b0aa6f9b506a28e61b3dc8996592b983695e8ebb58a8b41"
+checksum = "d32a725bc159af97c3e629873bb9f88fb8cf8a4867175f76dc987815ea07c83b"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.37"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
  "wasm-bindgen",
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "const-random"
 version = "0.1.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87e00182fe74b066627d63b85fd550ac2998d4b0bd86bfed477a0ae4c7c71359"
@@ -598,17 +598,17 @@
 checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num"
-version = "0.4.1"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b05180d69e3da0e530ba2a1dae5110317e49e3b7f3d41be227dc5f92e49ee7af"
+checksum = "3135b08af27d103b0a51f2ae0f8632117b7b185ccf931445affa8df530576a41"
 dependencies = [
  "num-bigint",
  "num-complex",
  "num-integer",
  "num-iter",
  "num-rational",
  "num-traits",
@@ -709,17 +709,17 @@
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "protobuf"
 version = "3.4.0"
@@ -738,15 +738,15 @@
 checksum = "e1ed294a835b0f30810e13616b1cd34943c6d1e84a8f3b0dcfe466d256c3e7e7"
 dependencies = [
  "thiserror",
 ]
 
 [[package]]
 name = "ptarslib"
-version = "0.0.2-rc0"
+version = "0.0.2-rc2"
 dependencies = [
  "arrow",
  "arrow-array",
  "arrow-schema",
  "chrono",
  "protobuf",
  "pyo3",
@@ -813,17 +813,17 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.4.1"
@@ -887,37 +887,37 @@
 name = "semver"
 version = "1.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.198"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.115"
+version = "1.0.116"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
+checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -930,43 +930,43 @@
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
 [[package]]
 name = "syn"
-version = "2.0.58"
+version = "2.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
+checksum = "909518bc7b1c9b779f1bbf07f2929d35af9f0f37e47c6e9ef7f9dddc1e1821f3"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "f0126ad08bff79f29fc3ae6a55cc72352056dfff61e3ff8bb7129476d44b23aa"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "d1cd413b5d558b4c5bf3680e324a6fa5014e7b7c067a51e69dbdf47eb7148b66"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -1058,15 +1058,15 @@
 
 [[package]]
 name = "windows-core"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -1078,110 +1078,117 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "zerocopy"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "74d4d3961e53fa4c9a25a8637fc2bfaf2595b3d3ae34875568a5cf64787716be"
 dependencies = [
```

### Comparing `ptars-0.0.2rc0/pyproject.toml` & `ptars-0.0.2rc2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 dependencies = [
     'protobuf > 3',
     "pyarrow > 15",
 ]
 
 [tool.poetry]
 name = "ptars"
-version = "0.0.2-rc0"
+version = "0.0.2-rc2"
 description = "Convert from protobuf to arrow and back in rust"
 authors = ["Tradewell Tech <engineering@tradewelltech.co>"]
 maintainers = ["0x26res <0x26res@gmail.com>"]
 packages = [    { include = "ptars", from = "python" } ]
 include = ["ptars/*",  "ptarslib/*", "ptarslib/src/*"]
 readme = "README.md"
 license = "Apache-2.0"
```

### Comparing `ptars-0.0.2rc0/PKG-INFO` & `ptars-0.0.2rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ptars
-Version: 0.0.2rc0
+Version: 0.0.2rc2
 Classifier: Programming Language :: Rust
 Classifier: Operating System :: POSIX :: Linux
 Requires-Dist: protobuf >3
 Requires-Dist: pyarrow >15
 License-File: LICENSE
 Summary: Fast python conversion from protobuf to arrow using rust
 Home-Page: https://github.com/0x26res/ptars
```


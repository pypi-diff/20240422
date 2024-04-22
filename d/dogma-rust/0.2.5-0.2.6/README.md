# Comparing `tmp/dogma_rust-0.2.5.tar.gz` & `tmp/dogma_rust-0.2.6.tar.gz`

## Comparing `dogma_rust-0.2.5.tar` & `dogma_rust-0.2.6.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 dogma_rust-0.2.5/Cargo.toml
--rw-r--r--   0    23269        0     3526 2024-04-10 03:45:24.000000 dogma_rust-0.2.5/.github/workflows/CI.yml
--rw-r--r--   0    23269        0      686 2024-04-10 03:45:24.000000 dogma_rust-0.2.5/.gitignore
--rw-r--r--   0    23269        0      377 2024-04-10 03:45:24.000000 dogma_rust-0.2.5/README.md
--rw-r--r--   0    23269        0     2405 2024-04-19 17:16:04.000000 dogma_rust-0.2.5/src/data.rs
--rw-r--r--   0    23269        0     5191 2024-04-19 17:27:38.000000 dogma_rust-0.2.5/src/fasta.rs
--rw-r--r--   0    23269        0     5877 2024-04-19 18:38:50.000000 dogma_rust-0.2.5/src/lib.rs
--rw-r--r--   0    23269        0     3125 2024-04-19 17:54:10.000000 dogma_rust-0.2.5/src/parallel.rs
--rw-r--r--   0    23269        0    19296 2024-04-19 17:56:30.000000 dogma_rust-0.2.5/Cargo.lock
--rw-r--r--   0    23269        0      538 2024-04-10 03:45:24.000000 dogma_rust-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 dogma_rust-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 dogma_rust-0.2.6/Cargo.toml
+-rw-r--r--   0    23269        0     3526 2024-04-10 03:45:24.000000 dogma_rust-0.2.6/.github/workflows/CI.yml
+-rw-r--r--   0    23269        0      686 2024-04-10 03:45:24.000000 dogma_rust-0.2.6/.gitignore
+-rw-r--r--   0    23269        0      472 2024-04-22 00:16:02.000000 dogma_rust-0.2.6/README.md
+-rw-r--r--   0    23269        0      499 2024-04-22 00:34:05.000000 dogma_rust-0.2.6/dogma_rust.pyi
+-rw-r--r--   0    23269        0     2395 2024-04-21 23:47:49.000000 dogma_rust-0.2.6/src/data.rs
+-rw-r--r--   0    23269        0     5150 2024-04-21 23:48:09.000000 dogma_rust-0.2.6/src/fasta.rs
+-rw-r--r--   0    23269        0     5714 2024-04-22 00:14:58.000000 dogma_rust-0.2.6/src/lib.rs
+-rw-r--r--   0    23269        0     3254 2024-04-22 00:02:26.000000 dogma_rust-0.2.6/src/parallel.rs
+-rw-r--r--   0    23269        0    19526 2024-04-21 21:48:52.000000 dogma_rust-0.2.6/Cargo.lock
+-rw-r--r--   0    23269        0      538 2024-04-21 21:31:45.000000 dogma_rust-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 dogma_rust-0.2.6/PKG-INFO
```

### Comparing `dogma_rust-0.2.5/.github/workflows/CI.yml` & `dogma_rust-0.2.6/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `dogma_rust-0.2.5/.gitignore` & `dogma_rust-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `dogma_rust-0.2.5/src/data.rs` & `dogma_rust-0.2.6/src/data.rs`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             Some(start)
         }).collect();
 
         let shifted_cu_seqlens = arrs.par_iter().zip(cu_seqlen_offsets).map(|(arr, offset)| {
             if offset == 0 {
                 arr.cu_seqlens.to_vec()
             } else {
-                let mut shifted = (&arr.cu_seqlens[1..]).to_vec(); // Skip the first element
+                let mut shifted = (arr.cu_seqlens[1..]).to_vec(); // Skip the first element
                 shifted.iter_mut().for_each(|cu_seqlen| *cu_seqlen += offset);
                 shifted
             }
         }).collect::<Vec<_>>();
 
         let shifted_cu_seqlens_refs: Vec<&[isize]> = shifted_cu_seqlens.iter().map(|cu_seqlens| {
             cu_seqlens.as_slice()
@@ -58,10 +58,10 @@
 impl<'a, T> TreatAsByteSlice<'a, T> for Bound<'a, PyUntypedArray> {
     unsafe fn as_slice(&self) -> PyResult<&'a [T]> {
         if !self.is_contiguous(){
             return Err(PyValueError::new_err("Array is not contiguous"));
         }
         let arr = *self.as_array_ptr();
         let dtype_width = self.dtype().itemsize();
-        Ok(std::slice::from_raw_parts(arr.data as *const T, self.len() * dtype_width as usize / std::mem::size_of::<T>()))
+        Ok(std::slice::from_raw_parts(arr.data as *const T, self.len() * dtype_width / std::mem::size_of::<T>()))
     }
 }
```

### Comparing `dogma_rust-0.2.5/src/fasta.rs` & `dogma_rust-0.2.6/src/fasta.rs`

 * *Files 2% similar despite different names*

```diff
@@ -147,16 +147,15 @@
     let char_mapping = CharMapping::from_pairs(&mapping_pairs, if is_rna {3} else {29});
 
     println!("Parsing file {path} in chunks");
 
     let chunk_results: Vec<ParsedFasta> = (0..n_threads).par_bridge().map(|i| {
         let start_i = i * chunk_size;
         let end_i = std::cmp::min((i + 1) * chunk_size, total_length);
-        let chunk_result = parse_fasta_chunk(&data, start_i, end_i, &char_mapping);
-        chunk_result
+        parse_fasta_chunk(&data, start_i, end_i, &char_mapping)
     }).collect();
 
 
     println!("Merging result");
     let sequences_refs = chunk_results.iter().map(|pf| &pf.sequences).collect::<Vec<_>>();
     let taxon_ids = chunk_results.iter().map(|pf| pf.taxon_ids.as_slice()).collect::<Vec<_>>();
```

### Comparing `dogma_rust-0.2.5/src/lib.rs` & `dogma_rust-0.2.6/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,18 @@
+#![allow(clippy::type_complexity)]
 mod fasta;
 mod data;
 pub mod parallel;
 
 use fasta::ParsedFasta;
 use pyo3::prelude::*;
 use pyo3::types::{PyList, PyTuple};
 use numpy::{IntoPyArray, PyArray1, PyArrayDescrMethods, PyReadonlyArray1, PyUntypedArray, PyUntypedArrayMethods};
 use crate::data::{AwkwardArray, TreatAsByteSlice};
 
-/// Formats the sum of two numbers as string.
-#[pyfunction]
-fn sum_as_string(a: usize, b: usize) -> PyResult<String> {
-    Ok((a + b).to_string())
-}
 
 impl<'a, T: Clone + Sync> From<Bound<'a, PyTuple>> for AwkwardArray<'a, T> {
     fn from(value: Bound<'a, PyTuple>) -> Self {
         let _content = value.get_item(0);
         todo!()
     }
 }
@@ -52,15 +48,15 @@
     let AwkwardArray {content, cu_seqlens} = AwkwardArray::parallel_concatenate(&awkward_refs);
 
     Ok((content.into_owned().into_pyarray_bound(py), cu_seqlens.into_owned().into_pyarray_bound(py)))
 }
 
 
 #[pyfunction]
-fn concatenate_numpy<'py>(py: Python<'py>, arrays: Bound<'py, PyList>) -> PyResult<(Bound<'py, PyArray1<u8>>, Bound<'py, PyArray1<usize>>)> {
+fn concatenate_numpy<'py>(py: Python<'py>, arrays: Bound<'py, PyList>) -> PyResult<(Bound<'py, PyArray1<u8>>, Bound<'py, PyArray1<isize>>)> {
     // Takes in a list of numpy arrays of the same dtype, and concatenates them into a single numpy array
     // The output array is always of dtype u8, so must be casted to the correct dtype after concatenation using `numpy.ndarray.view(dtype)`
     
     let buf_refs: Vec<_> = arrays.iter().map(|obj| -> PyResult<_> {
         let arr = obj.downcast::<PyUntypedArray>()?;
         Ok((arr.dtype(), unsafe{let arr = *arr.as_array_ptr(); arr.data}, arr.len(), arr.is_contiguous()))
     }).collect::<PyResult<_>>()?;
@@ -115,26 +111,25 @@
     let first_dtype = first_dtype.unwrap();
 
     let itemsize: usize = first_dtype.itemsize();
 
     let slices: Vec<&[u8]> = buf_refs.into_iter().map(|arr| unsafe { std::slice::from_raw_parts(arr.data, arr.len * itemsize) }).collect();
 
     let (content, mut cu_seqlens) = parallel::parallel_concatenate_buffers(&slices);
-    cu_seqlens.push(content.len());  // Add the final index
+    cu_seqlens.push(content.len() as isize);  // Add the final index
 
     let content_arr = content.into_pyarray_bound(py);
     let cu_seqlens_arr = cu_seqlens.into_pyarray_bound(py);
 
     Ok(PyTuple::new_bound(py, &[content_arr.to_object(py), cu_seqlens_arr.to_object(py)]))
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
 fn dogma_rust(_py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
-    m.add_function(wrap_pyfunction!(sum_as_string, m)?)?;
     m.add_function(wrap_pyfunction!(parse_fasta, m)?)?;
     m.add_function(wrap_pyfunction!(concatenate_numpy, m)?)?;
     m.add_function(wrap_pyfunction!(concatenate_awkward, m)?)?;
     m.add_function(wrap_pyfunction!(awkward_from_list_of_numpy, m)?)?;
     // m.add_function
     Ok(())
 }
```

### Comparing `dogma_rust-0.2.5/src/parallel.rs` & `dogma_rust-0.2.6/src/parallel.rs`

 * *Files 4% similar despite different names*

```diff
@@ -2,48 +2,50 @@
 
 struct SendPtr<T>(*mut T);
 
 // unsafe impl<T> Send for SendPtr<T> {}
 unsafe impl<T> Sync for SendPtr<T> {}
 
 pub trait ParallelConcatenate<T>{
-    fn parallel_concatenate(self) -> (Vec<T>, Vec<usize>);
+    fn parallel_concatenate(self) -> (Vec<T>, Vec<isize>);
 }
 
 impl<T, C> ParallelConcatenate<T> for C
 where
 C: ParallelIterator,
 T: Sync,
 C::Item: AsRef<[T]> + Sync, {
-    fn parallel_concatenate(self) -> (Vec<T>, Vec<usize>) {
+    fn parallel_concatenate(self) -> (Vec<T>, Vec<isize>) {
         let bufs: Vec<C::Item> = self.collect();
         parallel_concatenate_buffers(&bufs)
     }
 }
 
-pub fn parallel_concatenate_buffers<T: Sync>(bufs: &[impl AsRef<[T]> + Sync]) -> (Vec<T>, Vec<usize>) {
+#[allow(clippy::uninit_vec)] // OK because we are initializing _all_ elements before reading or dropping them
+pub fn parallel_concatenate_buffers<T: Sync>(bufs: &[impl AsRef<[T]> + Sync]) -> (Vec<T>, Vec<isize>) {
     let out_buf_size = bufs.iter().map(|buf| buf.as_ref().len()).sum();
 
     let mut out_buf = Vec::with_capacity(out_buf_size);
     unsafe {out_buf.set_len(out_buf_size);}
+
     let data = SendPtr(out_buf.as_mut_ptr());
 
-    let starting_indices: Vec<usize> = bufs.iter().scan(0, |acc, buf| {
+    let starting_indices: Vec<isize> = bufs.iter().scan(0, |acc, buf| {
         let start = *acc;
-        *acc += buf.as_ref().len();
+        *acc += buf.as_ref().len() as isize;
         Some(start)
     }).collect();
 
     starting_indices.par_iter().zip(bufs).for_each(|(&start, buf)| {
         let buf_len = buf.as_ref().len();
         let buf_ptr = buf.as_ref().as_ptr();
         unsafe {
             let send_dest = &data;
             let dest_base: *mut T = send_dest.0;
-            let dest: *mut T = dest_base.add(start);
+            let dest: *mut T = dest_base.add(start as usize);
             let src = buf_ptr;
             std::ptr::copy_nonoverlapping(src, dest, buf_len);
         }
     });
     
     (out_buf, starting_indices)
 }
```

### Comparing `dogma_rust-0.2.5/Cargo.lock` & `dogma_rust-0.2.6/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.81"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0952808a6c2afd1aa8947271f3a60f1a6763c7b912d210184c5149b5cf147247"
+checksum = "f538837af36e6f6a9be0faa67f9a314f8119e4e4b5867c6ab40ed60360142519"
 
 [[package]]
 name = "autocfg"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
@@ -39,36 +39,36 @@
 name = "bumpalo"
 version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
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
 name = "core-foundation-sys"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
@@ -96,31 +96,31 @@
 name = "crossbeam-utils"
 version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
 
 [[package]]
 name = "dogma-rust"
-version = "0.2.5"
+version = "0.2.6"
 dependencies = [
  "anyhow",
  "chrono",
  "eyre",
  "num-bigint",
  "numpy",
  "pyo3",
  "rand",
  "rayon",
 ]
 
 [[package]]
 name = "either"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "eyre"
 version = "0.6.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7cd915d99f24784cdc19fd37ef22b97e3ff0ae756c7e492e9fbfe897d61e2aec"
 dependencies = [
@@ -335,26 +335,26 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
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
 name = "pyo3"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -362,62 +362,62 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.21.1"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
  "heck",
  "proc-macro2",
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
 name = "rand"
 version = "0.8.5"
@@ -499,17 +499,17 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
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
@@ -592,15 +592,15 @@
 
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
@@ -612,103 +612,110 @@
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
```

### Comparing `dogma_rust-0.2.5/pyproject.toml` & `dogma_rust-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dogma_rust-0.2.5/PKG-INFO` & `dogma_rust-0.2.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dogma_rust
-Version: 0.2.5
+Version: 0.2.6
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: homepage, https://github.com/marcelroed/dogma-data
 Project-URL: repository, https://github.com/marcelroed/dogma-data
@@ -14,12 +14,16 @@
 
 ## Installation
 Dogma Rust can be installed from PyPI or from source. To install from PyPI, run:
 ```bash
 pip install dogma-rust
 ```
 
-
 To install from source, clone the repository and install the local package using `pip`:
 ```bash
 pip install -e .
 ```
+
+The library can also be installed using maturin directly
+```bash
+maturin develop --release
+```
```


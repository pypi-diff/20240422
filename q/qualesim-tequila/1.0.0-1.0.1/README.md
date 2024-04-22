# Comparing `tmp/qualesim-tequila-1.0.0.tar.gz` & `tmp/qualesim-tequila-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qualesim-tequila-1.0.0.tar", last modified: Wed Apr 17 03:28:01 2024, max compression
+gzip compressed data, was "qualesim-tequila-1.0.1.tar", last modified: Mon Apr 22 07:43:35 2024, max compression
```

## Comparing `qualesim-tequila-1.0.0.tar` & `qualesim-tequila-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 03:28:01.011781 qualesim-tequila-1.0.0/
--rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)     2808 2024-04-17 03:28:01.011781 qualesim-tequila-1.0.0/PKG-INFO
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     2292 2023-09-28 07:00:22.000000 qualesim-tequila-1.0.0/README.md
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 03:28:01.007781 qualesim-tequila-1.0.0/data/
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 03:28:01.007781 qualesim-tequila-1.0.0/data/bin/
--rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)      104 2024-03-15 09:02:38.000000 qualesim-tequila-1.0.0/data/bin/dqcsbetequila
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 03:28:01.007781 qualesim-tequila-1.0.0/qualesim_tequila/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2023-07-06 01:42:02.000000 qualesim-tequila-1.0.0/qualesim_tequila/__init__.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      102 2023-07-06 02:29:24.000000 qualesim-tequila-1.0.0/qualesim_tequila/__main__.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    17152 2024-04-17 03:27:10.000000 qualesim-tequila-1.0.0/qualesim_tequila/backend.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     2875 2024-03-29 07:51:37.000000 qualesim-tequila-1.0.0/qualesim_tequila/test.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 03:28:01.007781 qualesim-tequila-1.0.0/qualesim_tequila.egg-info/
--rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)     2808 2024-04-17 03:28:00.000000 qualesim-tequila-1.0.0/qualesim_tequila.egg-info/PKG-INFO
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      352 2024-04-17 03:28:00.000000 qualesim-tequila-1.0.0/qualesim_tequila.egg-info/SOURCES.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        1 2024-04-17 03:28:00.000000 qualesim-tequila-1.0.0/qualesim_tequila.egg-info/dependency_links.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       17 2024-04-17 03:28:00.000000 qualesim-tequila-1.0.0/qualesim_tequila.egg-info/top_level.txt
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       38 2024-04-17 03:28:01.011781 qualesim-tequila-1.0.0/setup.cfg
--rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)     1108 2024-04-17 03:26:17.000000 qualesim-tequila-1.0.0/setup.py
-drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-17 03:28:01.011781 qualesim-tequila-1.0.0/tests/
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    25164 2024-03-29 07:51:37.000000 qualesim-tequila-1.0.0/tests/test_gate.py
--rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     2526 2024-03-29 07:51:37.000000 qualesim-tequila-1.0.0/tests/test_qifile.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-22 07:43:35.553117 qualesim-tequila-1.0.1/
+-rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      660 2024-04-22 07:43:35.553117 qualesim-tequila-1.0.1/PKG-INFO
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      143 2024-04-22 07:43:07.000000 qualesim-tequila-1.0.1/README.md
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-22 07:43:35.549116 qualesim-tequila-1.0.1/data/
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-22 07:43:35.549116 qualesim-tequila-1.0.1/data/bin/
+-rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)      104 2024-03-15 09:02:38.000000 qualesim-tequila-1.0.1/data/bin/dqcsbetequila
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-22 07:43:35.549116 qualesim-tequila-1.0.1/qualesim_tequila/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        0 2023-07-06 01:42:02.000000 qualesim-tequila-1.0.1/qualesim_tequila/__init__.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      102 2023-07-06 02:29:24.000000 qualesim-tequila-1.0.1/qualesim_tequila/__main__.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    16487 2024-04-22 07:41:26.000000 qualesim-tequila-1.0.1/qualesim_tequila/backend.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     2875 2024-03-29 07:51:37.000000 qualesim-tequila-1.0.1/qualesim_tequila/test.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-22 07:43:35.549116 qualesim-tequila-1.0.1/qualesim_tequila.egg-info/
+-rw-r--r--   0 liudingdong  (1004) liudingdong  (1004)      660 2024-04-22 07:43:35.000000 qualesim-tequila-1.0.1/qualesim_tequila.egg-info/PKG-INFO
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)      352 2024-04-22 07:43:35.000000 qualesim-tequila-1.0.1/qualesim_tequila.egg-info/SOURCES.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)        1 2024-04-22 07:43:35.000000 qualesim-tequila-1.0.1/qualesim_tequila.egg-info/dependency_links.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       17 2024-04-22 07:43:35.000000 qualesim-tequila-1.0.1/qualesim_tequila.egg-info/top_level.txt
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)       38 2024-04-22 07:43:35.553117 qualesim-tequila-1.0.1/setup.cfg
+-rwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)     1108 2024-04-22 07:42:08.000000 qualesim-tequila-1.0.1/setup.py
+drwxrwxr-x   0 liudingdong  (1004) liudingdong  (1004)        0 2024-04-22 07:43:35.553117 qualesim-tequila-1.0.1/tests/
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)    25164 2024-03-29 07:51:37.000000 qualesim-tequila-1.0.1/tests/test_gate.py
+-rw-rw-r--   0 liudingdong  (1004) liudingdong  (1004)     2526 2024-03-29 07:51:37.000000 qualesim-tequila-1.0.1/tests/test_qifile.py
```

### Comparing `qualesim-tequila-1.0.0/qualesim_tequila/backend.py` & `qualesim-tequila-1.0.1/qualesim_tequila/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,26 @@
 def bitwise_reverse_sort(lst, k):
     sorted_lst = []
     for i in range(len(lst)):
         sorted_lst.append(lst[int("0b" + bin(i)[2:].zfill(k)[::-1], 2)])
     return sorted_lst
 
 
+def get_qubit_prob(lst, k, n):
+    prob = [[0], [0]]
+    for i in range(len(lst)):
+        if (i >> (n - k - 1)) & 1 == 0:
+            prob[0][0] += lst[i][0] ** 2
+        else:
+            prob[1][0] += lst[i][0] ** 2
+    prob[0][0] = prob[0][0] ** 0.5
+    prob[1][0] = prob[1][0] ** 0.5
+    return prob
+
+
 @plugin("Tequila interface", "Liu Dingdong", "0.0.1")
 class TequilaInterface(Backend):
     """Tequila Backend for DQCsim."""
 
     # ==========================================================================
     # Init the plugin
     # ==========================================================================
@@ -33,14 +45,15 @@
         self.gate = None
 
         # self.qubits is the index of qubits.
         self.qubits = {}
         self.typ = "CQInstr"
 
         self.cls_dict = dict()
+        self.state_res = dict()
 
         # self.qubits_ismeasured = {}
         # self.qubits_ismeasured_value = {}
 
     def handle_init(self, cmds):
         """handle_init the backend plugin with the given cmds.
         Here we initial the circuit to qubit(1,0) since the proj_norm func has
@@ -96,21 +109,17 @@
             qubit_refs (list): a list of qubits' index, start from 1.
             cmds (ArbCmd): send ArbCmd to the backend plugin.
         """
         # we allocate the qubits below using qubit(1, 0) to init the qubit as state |0>.
         for qubit_ref in qubit_refs:
             qu = self.states.qubit(1, 0)
             self.circuit.add_qubits_on_back([qu])
-
             # the index of qubit_ref is store in self.qubits.
             self.qubits[qubit_ref] = self.circuit.n - 1
 
-            # self.qubits_ismeasured is unused.
-            # self.qubits_ismeasured[qubit_ref] = 0
-
     def handle_free(self, qubit_refs):
         """use trace to proj the qubits into base to free it.
         now we should proj the qubit_ref in the end of program.
         using arb in the handle_measure to proj may be better.
 
         Args:
             qubit_refs (list): a list of qubit to be free.
@@ -153,17 +162,14 @@
         cls_list = []
 
         # measure_targets is the qubit index of qubit_refs.
         measure_targets = []
         for i in qubit_refs:
             measure_targets.append(self.qubits[i])
 
-        # get the statevector before measure.
-        # TODO the state_res should be rerange, deprecate parentheses.
-        # if measure_mod == "measureforres":
         circuit = self.states.qubit(self.circuit.n, self.circuit.data)
         loc = [0]
         bse = [0]
         for i in self.cls_dict.keys():
             loc.append(self.qubits[i])
             bse.append(self.cls_dict[i])
         circuit.proj_norm(loc, bse)
@@ -200,23 +206,23 @@
             # choose the max value as the cls_list to project.
             max_re = max(measure_res.values())
             for key in measure_res.keys():
                 if measure_res[key] == max_re:
                     for j in key:
                         cls_list.append(int(j))
         if measure_mod == "state_vector":
-           circuit = self.states.qubit(self.circuit.n, self.circuit.data)
-           loc = [0]
-           bse = [0]
-           for i in self.cls_dict.keys():
-               loc.append(self.qubits[i])
-               bse.append(self.cls_dict[i])
-           circuit.proj_norm(loc, bse)
-           state_res_after = [i[0] for i in circuit.vec().tolist()]
-           state_res = str([self.cls_dict, state_res_after])
+            circuit = self.states.qubit(self.circuit.n, self.circuit.data)
+            loc = [0]
+            bse = [0]
+            for i in self.cls_dict.keys():
+                loc.append(self.qubits[i])
+                bse.append(self.cls_dict[i])
+            circuit.proj_norm(loc, bse)
+            state_res_after = [i[0] for i in circuit.vec().tolist()]
+            state_res = str([self.cls_dict, state_res_after])
 
         # handle free, use proj_norm to proj the circuit, and rerange the index of qubits.
         if measure_mod == "free":
             self.circuit.proj_norm(measure_targets, cls_list)
             for j in qubit_refs:
                 for i in self.qubits.keys():
                     if i > j and self.qubits[i] != -1:
@@ -269,28 +275,14 @@
                 raise ValueError("method key does not have the right list size")
         elif isinstance(methods, str):
             methods = [methods] * len(qubit_refs)
         elif isinstance(methods, int):
             methods = [(methods >> i) & 1 for i in reversed(range(len(qubit_refs)))]
         else:
             raise ValueError("failed to parse method key")
-        # < ======================================================================
-        # methos is unused in the Tequila Backend. the codes above is of no sense.
-        # < ======================================================================
-
-        """ We have not define different measure basis here so the basis_hermetian
-        is unused here.
-
-        basis_hermetian = [
-            basis[0].real - basis[0].imag * 1j,
-            basis[2].real - basis[2].imag * 1j,
-            basis[1].real - basis[1].imag * 1j,
-            basis[3].real - basis[3].imag * 1j,
-        ]
-        """
 
         # get the measure_mod from input ArbData.
         if "measure_mod" in arb:
             measure_mod = arb["measure_mod"]
         else:
             measure_mod = "final_state"
         if "get_probability" in arb:
@@ -305,29 +297,23 @@
         cls_list = []
 
         # measure_targets is the qubit index of qubit_refs.
         measure_targets = []
         for i in qubit_refs:
             measure_targets.append(self.qubits[i])
 
-        # get the statevector before measure.
-        if measure_mod == "measureforres":
-            circuit = self.states.qubit(self.circuit.n, self.circuit.data)
-            loc = [0]
-            bse = [0]
-            for i in self.cls_dict.keys():
-                loc.append(self.qubits[i])
-                bse.append(self.cls_dict[i])
-            circuit.proj_norm(loc, bse)
-            state_res_before = bitwise_reverse_sort(
-                [i[0] for i in circuit.vec().tolist()], circuit.n
-            )
-            state_res = str([self.cls_dict, state_res_before])
+        circuit = self.states.qubit(self.circuit.n, self.circuit.data)
+        loc = [0]
+        bse = [0]
+        for i in self.cls_dict.keys():
+            loc.append(self.qubits[i])
+            bse.append(self.cls_dict[i])
+        circuit.proj_norm(loc, bse)
+        state_res_before = str([self.cls_dict, circuit.vec().tolist()])
 
-        # if measure_mod
         if (
             measure_mod == "one_shot"
             or measure_mod == "state_vector"
             or measure_mod == "free"
         ):
             # use meas_rej to measure the one_shot and state_vector measure_mod
             repn = 1
@@ -340,56 +326,56 @@
             # use others to handle other type of measure.
             repn = 1000
             if len(measure_targets) <= 3:
                 measure_res = self.circuit.meas_minor(measure_targets, repn)
             else:
                 measure_res = self.circuit.meas_mcmc(measure_targets, repn)
 
-            # choose the max value as the cls_list to project.
             max_re = max(measure_res.values())
             for key in measure_res.keys():
                 if measure_res[key] == max_re:
                     for j in key:
                         cls_list.append(int(j))
 
-        if measure_mod == "state_vector":
-            circuit = self.states.qubit(self.circuit.n, self.circuit.data)
-            loc = [0]
-            bse = [0]
-            for i in self.cls_dict.keys():
-                loc.append(self.qubits[i])
-                bse.append(self.cls_dict[i])
-            circuit.proj_norm(loc, bse)
-            state_res_after = bitwise_reverse_sort(
-                [i[0] for i in circuit.vec().tolist()], circuit.n
-            )
-            state_res = str([self.cls_dict, state_res_after])
         # handle free, use proj_norm to proj the circuit, and rerange the index of qubits.
         if measure_mod == "free":
             self.circuit.proj_norm(measure_targets, cls_list)
             for j in qubit_refs:
                 for i in self.qubits.keys():
                     if i > j and self.qubits[i] != -1:
                         self.qubits[i] = self.qubits[i] - 1
                 self.qubits[j] = -1
-
-        # use proj_site to proj it into cls_list and retain the original index.
         else:
             for i in range(len(cls_list)):
+                if (
+                    self.circuit.data[measure_targets[i]].shape[0] == 1
+                    and self.circuit.data[measure_targets[i]].shape[2] == 1
+                ):
+                    self.state_res[measure_targets[i]] = [
+                        list(i) for i in self.circuit.data[measure_targets[i]][0]
+                    ]
+                else:
+                    self.state_res[measure_targets[i]] = get_qubit_prob(
+                        self.circuit.vec().tolist(), measure_targets[i], self.circuit.n
+                    )
                 self.circuit.proj_site(measure_targets[i], cls_list[i])
 
         # form the Measurement and send it to upsteam plugins.
         for it in range(len(qubit_refs)):
+            state_res = str([self.cls_dict, self.state_res[qubit_refs[it]]])
             measurements.append(
                 Measurement(
                     qubit_refs[it],
                     cls_list[it],
                     struct.pack("<d", 1),
-                    probability=1,
+                    probability=abs(
+                        self.state_res[qubit_refs[it]][cls_list[it]][0] ** 2
+                    ),
                     state_vector=state_res,
+                    state_for_res=state_res_before,
                 )
             )
         return measurements
 
     def handle_prepare_gate(self, qubit_refs, basis, _arb):
         """the prepare gate is about the initial of gates. now default is qubit(1,0) to
         construct a qubit .
```

### Comparing `qualesim-tequila-1.0.0/qualesim_tequila/test.py` & `qualesim-tequila-1.0.1/qualesim_tequila/test.py`

 * *Files identical despite different names*

### Comparing `qualesim-tequila-1.0.0/setup.py` & `qualesim-tequila-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def read(fname):
     with open(os.path.join(os.path.dirname(__file__), fname)) as f:
         return f.read()
 
 
 setup(
     name="qualesim-tequila",
-    version="1.0.0",
+    version="1.0.1",
     author="Dingdong Liu",
     author_email="dingdongliu@quanta.org.cn",
     description="DQCsim backend for tequila.",
     license="GPLv3",
     keywords="qualesim tequila",
     url="https://gitee.com/hpcl_quanta/dqcsim-tequila.git",
     long_description=read("README.md"),
```

### Comparing `qualesim-tequila-1.0.0/tests/test_gate.py` & `qualesim-tequila-1.0.1/tests/test_gate.py`

 * *Files identical despite different names*

### Comparing `qualesim-tequila-1.0.0/tests/test_qifile.py` & `qualesim-tequila-1.0.1/tests/test_qifile.py`

 * *Files identical despite different names*


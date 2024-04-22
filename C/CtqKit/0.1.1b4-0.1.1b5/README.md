# Comparing `tmp/ctqkit-0.1.1b4.tar.gz` & `tmp/ctqkit-0.1.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctqkit-0.1.1b4.tar", max compression
+gzip compressed data, was "ctqkit-0.1.1b5.tar", max compression
```

## Comparing `ctqkit-0.1.1b4.tar` & `ctqkit-0.1.1b5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1060 2024-03-05 02:31:31.872856 ctqkit-0.1.1b4/LICENSE.txt
--rw-r--r--   0        0        0      953 2024-04-08 02:27:27.634900 ctqkit-0.1.1b4/pyproject.toml
--rw-r--r--   0        0        0       42 2024-03-04 09:21:32.455518 ctqkit-0.1.1b4/README.md
--rw-r--r--   0        0        0       62 2024-03-28 02:46:26.350830 ctqkit-0.1.1b4/src/CtqKit/__init__.py
--rw-r--r--   0        0        0     2919 2024-04-02 07:04:18.419446 ctqkit-0.1.1b4/src/CtqKit/account.py
--rw-r--r--   0        0        0    31334 2024-04-08 02:25:24.690537 ctqkit-0.1.1b4/src/CtqKit/platform.py
--rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 ctqkit-0.1.1b4/PKG-INFO
+-rw-r--r--   0        0        0     1060 2024-03-05 02:31:31.872856 ctqkit-0.1.1b5/LICENSE.txt
+-rw-r--r--   0        0        0      953 2024-04-22 02:57:48.361735 ctqkit-0.1.1b5/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-03-04 09:21:32.455518 ctqkit-0.1.1b5/README.md
+-rw-r--r--   0        0        0       62 2024-03-28 02:46:26.350830 ctqkit-0.1.1b5/src/CtqKit/__init__.py
+-rw-r--r--   0        0        0     2919 2024-04-02 07:04:18.419446 ctqkit-0.1.1b5/src/CtqKit/account.py
+-rw-r--r--   0        0        0    31282 2024-04-22 02:55:12.067746 ctqkit-0.1.1b5/src/CtqKit/platform.py
+-rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 ctqkit-0.1.1b5/PKG-INFO
```

### Comparing `ctqkit-0.1.1b4/LICENSE.txt` & `ctqkit-0.1.1b5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ctqkit-0.1.1b4/pyproject.toml` & `ctqkit-0.1.1b5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "CtqKit"
-version = "0.1.1-beta.4"
+version = "0.1.1-beta.5"
 description = "中国电信天衍量子计算云平台 Python SDK (ChinaTelecom Quantum Kit)"
 authors = ["Gao Jianjian <jianjian001@outlook.com>"]
 readme = "README.md"
 license = "Apache 2.0"
 documentation = "https://qc.zdxlz.com/informationSpace"
 homepage = "https://qc.zdxlz.com/"
 classifiers = [
```

### Comparing `ctqkit-0.1.1b4/src/CtqKit/account.py` & `ctqkit-0.1.1b5/src/CtqKit/account.py`

 * *Files identical despite different names*

### Comparing `ctqkit-0.1.1b4/src/CtqKit/platform.py` & `ctqkit-0.1.1b5/src/CtqKit/platform.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         Quantum or simulator machine list
 
         :return:
         """
         if self._cache_machine_list and isinstance(self._cache_machine_list, list):
             return self._cache_machine_list
         resp = requests.get(
-            f'{self.account.base_url}/qccp-quantum/experiment/quantum/computer/by/user',
+            f'{self.account.base_url}/qccp-quantum/experiment/sdk/quantum/computer',
             headers={
                 'Authorization': f'Bearer {self.account.access_token}',
                 'ApiCode': 'byUser',
                 'RequestTime': datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
             }
         )
         data = resp.json()
@@ -77,49 +77,42 @@
         quantum language list
 
         :return:
         """
         if self._cache_language_list and isinstance(self._cache_language_list, list):
             return self._cache_language_list
         resp = requests.get(
-            f'{self.account.base_url}/qccp-quantum/experiment/quantum/language/findAll',
+            f'{self.account.base_url}/qccp-quantum/experiment/sdk/quantum/language',
             headers={
                 'Authorization': f'Bearer {self.account.access_token}',
                 'ApiCode': 'findAll',
                 'RequestTime': datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
             }
         )
         data = resp.json()
         if data.get('code') != self.SUCCESS_CODE:
             raise RequestError(f"get language list failed: {data.get('msg')}")
         d = data.get('data')
         if cache:
             self._cache_language_list = d
         return d
 
-    def isq_to_qcis(self, circuit: str) -> list:
-        """
-        编译
-        :param circuit:
-        :return:
-        """
-
     def create_experiment_collection(
             self,
             name: str,
             remark: Optional[str] = ""
     ):
         """create a new collection of experiments.
 
         :param name: new experiment collection Name.
         :param remark: experimental remarks.
 
         :return: new experimental collection id
         """
-        url = f'{self.account.base_url}/qccp-quantum/experiment/create'
+        url = f'{self.account.base_url}/qccp-quantum/experiment/sdk/create'
         data = {"name": name, "remark": remark}
         headers = {
             "Authorization": f'Bearer {self.account.access_token}',
             'ApiCode': 'experimentCreate',
             'RequestTime': datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
         }
         res = requests.post(url, json=data, headers=headers)
@@ -144,21 +137,25 @@
         :param count: query count.
 
         :returns data:
             records: collection list.
             total: total count of experiments collection list.
 
         """
-        url = f'{self.account.base_url}/qccp-quantum/experiment/byUser?current={start}&size={count}'
+        url = f'{self.account.base_url}/qccp-quantum/experiment/sdk/byUser'
         headers = {
             "Authorization": f'Bearer {self.account.access_token}',
             'ApiCode': 'getExperimentByUser',
             'RequestTime': datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
         }
-        res = requests.get(url, headers=headers)
+        params = {
+            'current': start,
+            'size': count
+        }
+        res = requests.get(url, headers=headers, params=params)
         if res.status_code != self.SUCCESS_CODE:
             raise RequestError(f'create experiment failed, status code:{res.status_code}')
         result = res.json()
         code = result.get('code', -1)
         msg = result.get('msg', 'query failed')
         if code != self.SUCCESS_CODE:
             raise RequestError(f'create experiment failed: {msg}')
@@ -196,15 +193,15 @@
         for line in exp_data.split('\n'):
             lines.append(' '.join([word for word in line.strip().split() if word]))
         exp_data = '\n'.join(lines)
 
         if language == 'qcis':
             exp_data = exp_data.upper()
 
-        url = f'{self.account.base_url}/qccp-quantum/experiment/experiment/detail'
+        url = f'{self.account.base_url}/qccp-quantum/experiment/sdk/detail'
         data = {
             "inputCode": exp_data,
             "experimentId": collection_id,
             "languageCode": language,
             "name": name,
             "source": "SDK",
             "computerCode": machine_code
@@ -235,15 +232,15 @@
         """
         get experiment list for collection_id
         :param collection_id: collection id
         :param start: start index
         :param count: count
 
         """
-        url = f'{self.account.base_url}/qccp-quantum/experiment/detailList'
+        url = f'{self.account.base_url}/qccp-quantum/experiment/sdk/detailList'
         headers = {
             "Authorization": f'Bearer {self.account.access_token}',
             'ApiCode': 'experimentDetailList',
             'RequestTime': datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
         }
         params = {
             'current': start,
@@ -290,30 +287,30 @@
     def _run_experiment(self, data):
         """
         提交任务，并运行
 
         :param data:
         :return:
         """
-        url = f'{self.account.base_url}/qccp-quantum/experiment/sdkCommit'
+        url = f'{self.account.base_url}/qccp-quantum/experiment/sdk/sdkCommit'
         headers = {
             "Authorization": f'Bearer {self.account.access_token}',
             'ApiCode': 'commit',
             'RequestTime': datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
         }
         res = requests.post(url, json=data, headers=headers)
         status_code = res.status_code
         if status_code != 200:
             raise RequestError(f'运行实验接口请求失败, status_code:{status_code}')
         result = res.json()
         code = result.get('code', -1)
         msg = result.get('msg', '运行实验失败')
         if code != self.SUCCESS_CODE:
             raise RequestError(f'运行实验失败：{msg}')
-        task_id = result.get('data').get('experimentTaskId')
+        task_id = result.get('data').get('task_id')
         return task_id
 
     def submit_job(
             self,
             circuit: Optional[Union[List, str]] = None,
             exp_name: Optional[str] = "exp0",
             parameters: Optional[List[List]] = None,
@@ -401,15 +398,15 @@
         """
         批量提交任务，返回任务 id 列表，并后台排队运行
         todo: 接口未完成
 
         :param data:
         :return:
         """
-        url = f'{self.account.base_url}/qccp-quantum/experiment/runContentList'
+        url = f'{self.account.base_url}/qccp-quantum/experiment/sdk/runContentList'
         headers = {
             "Authorization": f'Bearer {self.account.access_token}',
             'ApiCode': 'QuantumRunContentList',
             'RequestTime': datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
         }
         res = requests.post(url, json=data, headers=headers)
         status_code = res.status_code
@@ -501,15 +498,15 @@
 
         :param circuit: circuit
         :param language: circuit language
         :return:
         """
         languages = ['isq']
         assert language in languages, f'language must be {languages}'
-        url = f'{self.account.base_url}/qccp-quantum/experiment/experiment/compile'
+        url = f'{self.account.base_url}/qccp-quantum/experiment/sdk/compile'
         headers = {
             "Authorization": f'Bearer {self.account.access_token}',
             'ApiCode': 'quantumComputerZDX',
             'RequestTime': datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
         }
         data = {
             "source": "sdk",
@@ -547,15 +544,15 @@
             Union[int, str]: 0 failed, not 0 successful, success returns the experimental result
         """
         if isinstance(query_id, str):
             query_id = [query_id]
         t0 = time()
         while time() - t0 < max_wait_time:
             try:
-                url = f'{self.account.base_url}/qccp-quantum/experiment/getResultByIds'
+                url = f'{self.account.base_url}/qccp-quantum/experiment/sdk/getResultByIds'
                 headers = {
                     "Authorization": f'Bearer {self.account.access_token}',
                     'ApiCode': 'getResultByIds',
                     'RequestTime': self.current_datetime()
                 }
                 # data = {"query_ids": query_id}
                 data = query_id
@@ -751,10 +748,11 @@
         qubits_used = config_json['qubit']['singleQubit']['gate error']['qubit_used']
         disable_qubits = [q for q in qubits if q not in qubits_used]
         coupler_map = config_json['overview']['coupler_map']
         adjacency_list = []
         for Q1, Q2 in coupler_map.values():
             q1 = int(Q1[1:])
             q2 = int(Q2[1:])
-            if Q1 in disable_qubits or Q2 in disable_qubits: continue
+            if Q1 in disable_qubits or Q2 in disable_qubits:
+                continue
             adjacency_list.append([q1, q2])
         return adjacency_list
```

### Comparing `ctqkit-0.1.1b4/PKG-INFO` & `ctqkit-0.1.1b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CtqKit
-Version: 0.1.1b4
+Version: 0.1.1b5
 Summary: 中国电信天衍量子计算云平台 Python SDK (ChinaTelecom Quantum Kit)
 Home-page: https://qc.zdxlz.com/
 License: Apache 2.0
 Author: Gao Jianjian
 Author-email: jianjian001@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


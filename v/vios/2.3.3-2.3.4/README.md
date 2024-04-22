# Comparing `tmp/vios-2.3.3-py3-none-any.whl.zip` & `tmp/vios-2.3.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,27 @@
-Zip file size: 46797 bytes, number of entries: 25
+Zip file size: 46821 bytes, number of entries: 25
 -rw-rw-rw-  2.0 fat     2858 b- defN 24-Mar-19 07:04 quark/__main__.py
--rw-rw-rw-  2.0 fat    19127 b- defN 24-Apr-12 01:40 quark/proxy.py
+-rw-rw-rw-  2.0 fat    19343 b- defN 24-Apr-22 01:34 quark/proxy.py
 -rw-rw-rw-  2.0 fat    18861 b- defN 24-Mar-21 01:49 quark/app/__init__.py
--rw-rw-rw-  2.0 fat     2575 b- defN 24-Apr-10 00:45 quark/app/_data.py
+-rw-rw-rw-  2.0 fat     2575 b- defN 24-Apr-18 07:42 quark/app/_data.py
 -rw-rw-rw-  2.0 fat    10205 b- defN 24-Mar-19 07:04 quark/app/demo.py
 -rw-rw-rw-  2.0 fat     9043 b- defN 24-Mar-19 07:04 quark/app/task.py
 -rw-rw-rw-  2.0 fat     5876 b- defN 24-Mar-19 07:16 quark/app/uapi.py
--rw-rw-rw-  2.0 fat     7914 b- defN 24-Mar-19 07:04 quark/driver/VirtualDevice.py
+-rw-rw-rw-  2.0 fat     7914 b- defN 24-Apr-12 08:12 quark/driver/VirtualDevice.py
 -rw-rw-rw-  2.0 fat      386 b- defN 24-Mar-19 07:04 quark/driver/__init__.py
 -rw-rw-rw-  2.0 fat      217 b- defN 24-Mar-19 07:04 quark/driver/common/__init__.py
 -rw-rw-rw-  2.0 fat     4478 b- defN 24-Mar-19 07:04 quark/driver/common/basedriver.py
 -rw-rw-rw-  2.0 fat     4663 b- defN 24-Mar-19 07:04 quark/driver/common/quantity.py
 -rw-rw-rw-  2.0 fat     5432 b- defN 24-Mar-19 07:04 quark/driver/common/visadriver.py
 -rw-rw-rw-  2.0 fat     1188 b- defN 24-Mar-19 07:04 quark/envelope/__init__.py
 -rw-rw-rw-  2.0 fat    15111 b- defN 24-Mar-19 07:04 quark/envelope/assembler.py
 -rw-rw-rw-  2.0 fat     4322 b- defN 24-Mar-19 07:04 quark/envelope/calculator.py
 -rw-rw-rw-  2.0 fat     1106 b- defN 24-Mar-19 07:04 quark/envelope/device.py
 -rw-rw-rw-  2.0 fat     3758 b- defN 24-Mar-25 01:32 quark/envelope/processor.py
 -rw-rw-rw-  2.0 fat     4324 b- defN 24-Apr-11 01:52 quark/envelope/router.py
 -rw-rw-rw-  2.0 fat     2841 b- defN 24-Mar-25 01:32 quark/envelope/systemq.py
--rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-12 03:17 vios-2.3.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1215 b- defN 24-Apr-12 03:17 vios-2.3.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-12 03:17 vios-2.3.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-12 03:17 vios-2.3.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1995 b- defN 24-Apr-12 03:17 vios-2.3.3.dist-info/RECORD
-25 files, 128678 bytes uncompressed, 43621 bytes compressed:  66.1%
+-rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-22 01:35 vios-2.3.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1215 b- defN 24-Apr-22 01:35 vios-2.3.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-22 01:35 vios-2.3.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-22 01:35 vios-2.3.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1995 b- defN 24-Apr-22 01:35 vios-2.3.4.dist-info/RECORD
+25 files, 128894 bytes uncompressed, 43645 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -54,23 +54,23 @@
 
 Filename: quark/envelope/router.py
 Comment: 
 
 Filename: quark/envelope/systemq.py
 Comment: 
 
-Filename: vios-2.3.3.dist-info/LICENSE
+Filename: vios-2.3.4.dist-info/LICENSE
 Comment: 
 
-Filename: vios-2.3.3.dist-info/METADATA
+Filename: vios-2.3.4.dist-info/METADATA
 Comment: 
 
-Filename: vios-2.3.3.dist-info/WHEEL
+Filename: vios-2.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: vios-2.3.3.dist-info/top_level.txt
+Filename: vios-2.3.4.dist-info/top_level.txt
 Comment: 
 
-Filename: vios-2.3.3.dist-info/RECORD
+Filename: vios-2.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## quark/proxy.py

```diff
@@ -251,15 +251,15 @@
             - ctx: 编译所用的上下文环境(ctx)
             - debug: 由设备返回的原始数据
             - trace: 每个指令执行所用时间
 
         Returns:
             _type_: _description_
         """
-        if stage in ['ini', 'raw', 'ctx']:
+        if stage in ['ini', 'raw', 'ctx', 'byp']:
             return self.server.review(self.tid, index)[stage]
         elif stage in ['debug', 'trace']:
             return self.server.track(self.tid, index)[stage]
 
     def process(self, data: list[dict]):
         for dat in data:
             for k, v in dat.items():
@@ -350,15 +350,15 @@
             self.progress.display()
             return
         self.handles[self.tid] = asyncio.get_running_loop(
         ).call_later(interval, self.refresh, *(interval,))
 
 
 def transpile(task: dict):
-    quafuos = str(Path.home()/'Desktop/qusteed/0.1.4')
+    quafuos = str(Path.home()/'Desktop/qusteed/0.1.6')
     if quafuos not in sys.path:
         print('adding quafuos', quafuos)
         sys.path.append(quafuos)
 
     circuit = task.get('circuit', '')
     qasm = ''
     if not isinstance(circuit, list):
@@ -370,18 +370,25 @@
             compile=task.get('compile', True),
             backend=task.get('chip', ''))
         # import compiler
         # transpile
         # else:
         #     print('nononononoonoo compile')
         #     qasm = circuit
-        if task['chip'] == 'Haituo':
-            QMAP = {i: f'Q{i+39}' for i in range(156)}
-        else:
-            QMAP = {i: f'Q{i+0}' for i in range(156)}
+        mapping = {}
+        try:
+            with open(Path.home()/'Desktop/home/mapping.json', 'r') as f:
+                mapping = json.loads(f.read())
+        except Exception as e:
+            if task['chip'] == 'Haituo':
+                mapping[task['chip']] = {
+                    str(i): f'Q{i+39}' for i in range(156)}
+            else:
+                mapping[task['chip']] = {str(i): f'Q{i+0}' for i in range(156)}
+        QMAP = mapping[task['chip']]
 
         circuit, qubits = openqasm_to_qlisp(qasm, QMAP=QMAP)
 
     qlisp = ',\n'.join([str(op) for op in circuit])
     logger.info(f"\n{'>'*36}qasm:\n{qasm}\n{'>'*36}qlisp:\n[{qlisp}]")
 
     measure = []
@@ -389,15 +396,15 @@
         if isinstance(ops[0], tuple) and ops[0][0] == 'Measure':
             measure.append((ops[0][1], ops[1]))
     return qasm, [circuit], measure
 
 
 def update(backend: str, info: dict, token: str = ''):
 
-    quafuos = str(Path.home()/'Desktop/qusteed/0.1.4')
+    quafuos = str(Path.home()/'Desktop/qusteed/0.1.6')
     if quafuos not in sys.path:
         print('adding quafuos', quafuos)
         sys.path.append(quafuos)
     with open(f'{backend}.json', 'w') as f:
         f.write(json.dumps(info, indent=4))
     from qusteedAPIs import call_local_backend_api
     call_local_backend_api(backend=backend, chip_info_dict=info)
@@ -460,15 +467,15 @@
 
         # return ret, t.status()['status']
 
     def cancel(self, tid: int):
         return self.server.cancel(tid)
 
     def status(self, tid: int = 0):
-        self.server.query('etc.cloud.online')
+        pass
 
     def result(self, tid: int, raw: bool = False):
         """根据任务id获取结果
 
         Args:
             tid (int): 任务id
 
@@ -541,12 +548,9 @@
                'tid': meta['tid'],
                'error': meta.get('error', ''),
                'status': status,
                'finished': meta['finished'],
                }
         return ret
 
-    def sysinfo(self):
-        return self.server.sysinfo(False)
-
     def snr(self, data):
         return data
```

## Comparing `vios-2.3.3.dist-info/LICENSE` & `vios-2.3.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vios-2.3.3.dist-info/METADATA` & `vios-2.3.4.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vios
-Version: 2.3.3
+Version: 2.3.4
 Summary: runtime requirements for systemq
 Author-email: YL Feng <fengyl@baqis.ac.cn>
 Project-URL: homepage, https://gitee.com
 Project-URL: bugs, https://gitee.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

## Comparing `vios-2.3.3.dist-info/RECORD` & `vios-2.3.4.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 quark/__main__.py,sha256=ky318p_RHmGRdMyzIL2meu-JOgqzRrH-hWfFvhceZGE,2858
-quark/proxy.py,sha256=TYqs3xJ4fBfwWCUWqmRQDyBtA0IHm0wEUev4HvXV0XA,19127
+quark/proxy.py,sha256=Raj5V0uqtfn-9fWFWb-kzx4DcS2PTzej3gwen0VSj1k,19343
 quark/app/__init__.py,sha256=MjOh4mkjvwFzEEfPNv-dMOcoktAtYCBtl-P5_UA7MzQ,18861
 quark/app/_data.py,sha256=EGGTD2FrZ8vlbMh4jlmWhYk4fEG3FolGoWaQ26qxoss,2575
 quark/app/demo.py,sha256=eod5vSXKB0XI-Rr8UVKkNc9tOUfWCjI109Imd8bKmuo,10205
 quark/app/task.py,sha256=QEZuNia59sLEWa8pl2XIjItx2NismSTPZFnFt8-90HM,9043
 quark/app/uapi.py,sha256=itjEa89SUXozZqBGLH-3o4mKtRssNQODDj60knC-cGE,5876
 quark/driver/VirtualDevice.py,sha256=Cswl_ykFhIsocGV6Okh_YS1b48FeLm2fh1ruXqmNoyw,7914
 quark/driver/__init__.py,sha256=p1pVx1xTulBT8-qdp_zJ859tdIsA92XdvwrkqcVHL4s,386
@@ -14,12 +14,12 @@
 quark/envelope/__init__.py,sha256=5_cs0tZ7mV4GjOsY2isx8sUQu4u6Y3WN-9DUGG27SQM,1188
 quark/envelope/assembler.py,sha256=ENwX7FutJvpg6_Wcm42_Zx-ddq40JozuYqHPwJp09ZA,15111
 quark/envelope/calculator.py,sha256=0rZAA46sWh_X8wOBmpBvmljqCV53ID4VHPX1cE_abEc,4322
 quark/envelope/device.py,sha256=5E3oWZ84IYnQdzlmzltgPyayYz_au7p7UIbFVpJUa0Q,1106
 quark/envelope/processor.py,sha256=uMIwu83a4SDZVM3OE5_WrBya_4jxtdcXPd6pYa0osrk,3758
 quark/envelope/router.py,sha256=w3PiOCtc0YZZapwut2jWYf5vISTdZQWOGT_6bXTjCmI,4324
 quark/envelope/systemq.py,sha256=QAaHLv68C9UjMp9qHt9t-HJkOTpCkbHZTlNVOsAzIBc,2841
-vios-2.3.3.dist-info/LICENSE,sha256=B_BP5ebph3-SqRxXvo-6Bh7vzPL2nPY5qSFQfr7xM_s,1085
-vios-2.3.3.dist-info/METADATA,sha256=fkePnVnm9df9_oasYTVVGig8LqvujlXksLBIgq_Jf3Q,1215
-vios-2.3.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-vios-2.3.3.dist-info/top_level.txt,sha256=7SspgYXMW_50_NVkPj0EbFg4jFlGVsaIDfpqNsA1IMY,6
-vios-2.3.3.dist-info/RECORD,,
+vios-2.3.4.dist-info/LICENSE,sha256=B_BP5ebph3-SqRxXvo-6Bh7vzPL2nPY5qSFQfr7xM_s,1085
+vios-2.3.4.dist-info/METADATA,sha256=UMbZlfWCNYvi0xchpmbK3Gnjdxc1z00dnXHzGv8IKSE,1215
+vios-2.3.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+vios-2.3.4.dist-info/top_level.txt,sha256=7SspgYXMW_50_NVkPj0EbFg4jFlGVsaIDfpqNsA1IMY,6
+vios-2.3.4.dist-info/RECORD,,
```


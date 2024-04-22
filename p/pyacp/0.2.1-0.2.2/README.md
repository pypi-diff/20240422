# Comparing `tmp/pyacp-0.2.1.tar.gz` & `tmp/pyacp-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyacp-0.2.1.tar", last modified: Tue Apr 16 08:51:38 2024, max compression
+gzip compressed data, was "pyacp-0.2.2.tar", last modified: Mon Apr 22 09:34:42 2024, max compression
```

## Comparing `pyacp-0.2.1.tar` & `pyacp-0.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 08:51:38.744910 pyacp-0.2.1/
--rw-rw-rw-   0        0        0     2174 2024-04-16 03:34:16.000000 pyacp-0.2.1/AcpHub.py
--rw-rw-rw-   0        0        0     7447 2024-04-16 08:51:38.744408 pyacp-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     7205 2024-04-16 08:51:21.000000 pyacp-0.2.1/README.md
--rw-rw-rw-   0        0        0        0 2024-04-16 03:34:16.000000 pyacp-0.2.1/__init__.py
--rw-rw-rw-   0        0        0     1993 2024-04-16 03:34:16.000000 pyacp-0.2.1/acp_idl.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:51:38.669179 pyacp-0.2.1/acp_libs/
-drwxrwxrwx   0        0        0        0 2024-04-16 08:51:38.691226 pyacp-0.2.1/acp_libs/lib/
--rw-rw-rw-   0        0        0        0 2024-04-16 03:34:16.000000 pyacp-0.2.1/acp_libs/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:51:38.715946 pyacp-0.2.1/acp_libs/lib/linux/
--rw-rw-rw-   0        0        0        0 2024-04-16 03:34:16.000000 pyacp-0.2.1/acp_libs/lib/linux/__init__ .py
--rw-rw-rw-   0        0        0 11777056 2024-04-16 03:34:16.000000 pyacp-0.2.1/acp_libs/lib/linux/libacp-c.so
--rw-rw-rw-   0        0        0    29288 2024-04-16 03:34:16.000000 pyacp-0.2.1/acp_libs/lib/linux/libacp-core.so
-drwxrwxrwx   0        0        0        0 2024-04-16 08:51:38.733925 pyacp-0.2.1/acp_libs/lib/win/
--rw-rw-rw-   0        0        0        0 2024-04-16 03:34:16.000000 pyacp-0.2.1/acp_libs/lib/win/__init__.py
--rw-rw-rw-   0        0        0  6911488 2024-04-16 03:34:16.000000 pyacp-0.2.1/acp_libs/lib/win/acp-c.dll
--rw-rw-rw-   0        0        0   111616 2024-04-16 03:34:16.000000 pyacp-0.2.1/acp_libs/lib/win/acp-core.dll
--rw-rw-rw-   0        0        0     1798 2024-04-16 03:34:16.000000 pyacp-0.2.1/enumdef.py
--rw-rw-rw-   0        0        0     1065 2024-04-16 03:34:16.000000 pyacp-0.2.1/notify.py
-drwxrwxrwx   0        0        0        0 2024-04-16 08:51:38.743207 pyacp-0.2.1/pyacp.egg-info/
--rw-rw-rw-   0        0        0     7447 2024-04-16 08:51:38.000000 pyacp-0.2.1/pyacp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      514 2024-04-16 08:51:38.000000 pyacp-0.2.1/pyacp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 08:51:38.000000 pyacp-0.2.1/pyacp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-04-16 08:51:38.000000 pyacp-0.2.1/pyacp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       53 2024-04-16 08:51:38.000000 pyacp-0.2.1/pyacp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6307 2024-04-16 08:33:11.000000 pyacp-0.2.1/pyacp.py
--rw-rw-rw-   0        0        0      609 2024-04-16 03:34:16.000000 pyacp-0.2.1/read.py
--rw-rw-rw-   0        0        0      508 2024-04-16 03:34:16.000000 pyacp-0.2.1/read_state.py
--rw-rw-rw-   0        0        0      625 2024-04-16 03:34:16.000000 pyacp-0.2.1/readwrite.py
--rw-rw-rw-   0        0        0     1057 2024-04-16 03:34:16.000000 pyacp-0.2.1/resettime.py
--rw-rw-rw-   0        0        0      113 2024-04-16 08:51:38.745913 pyacp-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      720 2024-04-16 08:47:55.000000 pyacp-0.2.1/setup.py
--rw-rw-rw-   0        0        0      566 2024-04-16 03:34:16.000000 pyacp-0.2.1/write.py
--rw-rw-rw-   0        0        0      638 2024-04-16 03:34:16.000000 pyacp-0.2.1/write_ctrl.py
+drwxrwxrwx   0        0        0        0 2024-04-22 09:34:42.443132 pyacp-0.2.2/
+-rw-rw-rw-   0        0        0     2174 2024-04-16 03:34:16.000000 pyacp-0.2.2/AcpHub.py
+-rw-rw-rw-   0        0        0     7933 2024-04-22 09:34:42.443132 pyacp-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7689 2024-04-22 09:28:37.000000 pyacp-0.2.2/README.md
+-rw-rw-rw-   0        0        0        0 2024-04-16 03:34:16.000000 pyacp-0.2.2/__init__.py
+-rw-rw-rw-   0        0        0     1993 2024-04-16 03:34:16.000000 pyacp-0.2.2/acp_idl.py
+drwxrwxrwx   0        0        0        0 2024-04-22 09:34:42.375784 pyacp-0.2.2/acp_libs/
+drwxrwxrwx   0        0        0        0 2024-04-22 09:34:42.396167 pyacp-0.2.2/acp_libs/lib/
+-rw-rw-rw-   0        0        0        0 2024-04-16 03:34:16.000000 pyacp-0.2.2/acp_libs/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-22 09:34:42.419189 pyacp-0.2.2/acp_libs/lib/linux/
+-rw-rw-rw-   0        0        0        0 2024-04-16 03:34:16.000000 pyacp-0.2.2/acp_libs/lib/linux/__init__ .py
+-rw-rw-rw-   0        0        0 11777056 2024-04-16 03:34:16.000000 pyacp-0.2.2/acp_libs/lib/linux/libacp-c.so
+-rw-rw-rw-   0        0        0    29288 2024-04-16 03:34:16.000000 pyacp-0.2.2/acp_libs/lib/linux/libacp-core.so
+drwxrwxrwx   0        0        0        0 2024-04-22 09:34:42.435257 pyacp-0.2.2/acp_libs/lib/win/
+-rw-rw-rw-   0        0        0        0 2024-04-16 03:34:16.000000 pyacp-0.2.2/acp_libs/lib/win/__init__.py
+-rw-rw-rw-   0        0        0  6911488 2024-04-16 03:34:16.000000 pyacp-0.2.2/acp_libs/lib/win/acp-c.dll
+-rw-rw-rw-   0        0        0   111616 2024-04-16 03:34:16.000000 pyacp-0.2.2/acp_libs/lib/win/acp-core.dll
+-rw-rw-rw-   0        0        0     1798 2024-04-16 03:34:16.000000 pyacp-0.2.2/enumdef.py
+-rw-rw-rw-   0        0        0     1054 2024-04-22 09:28:37.000000 pyacp-0.2.2/notify.py
+drwxrwxrwx   0        0        0        0 2024-04-22 09:34:42.441818 pyacp-0.2.2/pyacp.egg-info/
+-rw-rw-rw-   0        0        0     7933 2024-04-22 09:34:42.000000 pyacp-0.2.2/pyacp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      514 2024-04-22 09:34:42.000000 pyacp-0.2.2/pyacp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-22 09:34:42.000000 pyacp-0.2.2/pyacp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-22 09:34:42.000000 pyacp-0.2.2/pyacp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       53 2024-04-22 09:34:42.000000 pyacp-0.2.2/pyacp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6307 2024-04-16 08:33:11.000000 pyacp-0.2.2/pyacp.py
+-rw-rw-rw-   0        0        0      598 2024-04-22 09:28:37.000000 pyacp-0.2.2/read.py
+-rw-rw-rw-   0        0        0      508 2024-04-16 03:34:16.000000 pyacp-0.2.2/read_state.py
+-rw-rw-rw-   0        0        0      614 2024-04-22 09:28:37.000000 pyacp-0.2.2/readwrite.py
+-rw-rw-rw-   0        0        0     1057 2024-04-16 03:34:16.000000 pyacp-0.2.2/resettime.py
+-rw-rw-rw-   0        0        0      113 2024-04-22 09:34:42.444136 pyacp-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      713 2024-04-22 09:29:32.000000 pyacp-0.2.2/setup.py
+-rw-rw-rw-   0        0        0      555 2024-04-22 09:28:37.000000 pyacp-0.2.2/write.py
+-rw-rw-rw-   0        0        0      638 2024-04-16 03:34:16.000000 pyacp-0.2.2/write_ctrl.py
```

### Comparing `pyacp-0.2.1/AcpHub.py` & `pyacp-0.2.2/AcpHub.py`

 * *Files identical despite different names*

### Comparing `pyacp-0.2.1/PKG-INFO` & `pyacp-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,24 @@
 Metadata-Version: 2.1
 Name: pyacp
-Version: 0.2.1
+Version: 0.2.2
 Summary: python fastdds acp api
 Author: Li Meng
 Description-Content-Type: text/markdown
 Requires-Dist: protobuf==3.19.5
 Requires-Dist: cffi==1.15.1
 Requires-Dist: betterproto==1.2.5
 
-***Attention:***
+# ACP HELLO
 
-1.下载方法：pip install pyacp
+## 一.**Python ****ACP**** overview**
 
-2.引用时需要：import AcpHub
+Acp 提供了多语言的接口版本，本文在于详细描述各个接口作用，以及使用方法和依赖。
 
-3.pyacp:默认下载了cffi,betterproto,protobuf,且指定版本，请自行避免版本冲突（建议在venv中操作）
-
-4.特别需要注意的是：AcpHub包中已经包含了所有需要的包，引用时请直接：
-
-AcpHub.pyacp.ffi.callback（用于注册callback） 或者Acp.acp\_idl（用于引用协议内容）等等
-
-# **一**.  **Python ****ACP**** overview**
-
-Acp 提供了多语言的接口版本，本章在于详细描述各个接口作用，以及使用方法和依赖。
-
-具体有关基本协议部分请参考：[ACP 通信协议详解](https://bd3ubzo9h2.feishu.cn/docx/EmGxdor9Zoqp4px30zhcT1kJnvf)
-
-# **二. 数据流转与关键接口流程图：**
-
-1. ## **c/s架构下的流程图**
-
-**暂时无法在飞书文档外展示此内容**
-
-2. ## **发布订阅模式下的流程图：**
-
-**暂时无法在飞书文档外展示此内容**
-
-# **三. 关键接口汇总与解析：**
+## **二. 关键接口汇总与解析：**
 
 ```Python
 import pyacp
 import acp_idl # 此包为内置包，数据协议的基本，使用response与request时请引用
                #举例：AcpHub.acp_idl.Request() 等等
 from typing import Union
 class AcpClient:#Client类，客户端类，作为客户端主动请求Server
@@ -61,38 +39,78 @@
     def __init__(self,device_id: Union[int],topic: Union[str],callback,resp_data_size:Union[int]):
     #run方法： 启动server的监听机制，启动后进程需主动操作使其常驻而不退出。
     def run(self):
     #stop方法：server 端主动停止监听
     def stop(self):
     #destroy方法：server主动销毁本server
     def destroy(self):
-  
+
 class AcpSubscriber:#发布订阅模式下的订阅端，用于接收发布者发布的数据
     #构造函数：device id与topic 确定唯一通信端，callback为回调函数，在流程图中有具体的声明与实现方法。
     def __init__(self,device_id: Union[int],topic: Union[str],callback):
     #listen：开启对发布者发布数据的监听
     def listen(self):
     #stop：主动停止监听
     def stop(self):
     #destory:销毁当前订阅端
     def destory(self):
-      
+
 class AcpPublisher:#发布订阅模式下的发布端，用于发布数据给接受者，支持一对多
-  
+
     #构造函数： device id与topic唯一确定通信端。
     def __init__(self,device_id: Union[int],topic: Union[str]):
     #publish：主动推送数据，数据类型要和订阅端一致。ps:Request 和Response在这里不是请求和响应的意思，而是为了统一数据类型。换而言之，用Request和Response完全取决于用户需要
     def publish(self,message : Union[acp_idl.Request,acp_idl.Response]):
     #hassubscribers： 查看是否有订阅端等待接收数据，建议在真正发布数据前使用，并在检查到订阅端后再发布数据，避免不必要的资源浪费。
     def hassubscribers(self):
     #destroy：主动销毁发布端。
     def destroy(self):
 ```
 
-四.具体的代码示例，请结合上述所有资料理解。
+## 三. 协议描述
+
+acp 整体 具备cs请求应答模式以及发布订阅模式，其通信规则由proto协定。
+
+基础通信框架下需要以AcpHub.acp_idl中定义好的Request以及Response为数据载体，其中包含data字段的协议模块，用户可以自己使用proto定义自己的协议内容并通过序列化放置在载体内。
+
+其中request和response载体模块中，定义了一系列针对不同场景的协议块，如下
+
+```
+read_req <--------> read_resp
+write_req <------->write_resp
+add_notify_req<------->add_notify_resp
+del_notify_req<------->del_notify_resp
+read_state_req<------->read_state_resp
+write_ctrl_req<------->write_ctrl_resp
+read_write_req<------->read_write_resp
+```
+
+用户可以自行选择需要的模块进行通信。
+
+以write_req举例：
+
+write_req包含如下字段：
+
+```
+id_group uint64 #使用时用于标记请求的具体目标，请自行定义枚举传入或使用已经定义好的业务方的枚举
+offset   int    # 数据偏移量
+length   int    # 数据长度
+data     bytes  # 用于传入业务方协议定义后的序列化数据
+
+```
+
+代码如下：
+
+```
+    req = pyacp.acp_idl.Request()
+    req.write_req.id_group = pyacp.acp_idl.enumdef.Idgroups.IGR_INVALID
+    req.write_req.length = 123
+```
+
+## 四.具体的代码示例，请结合上述所有资料理解。
 
 client:
 
 ```Python
 from datetime import date
 import sys
 import AcpHub
@@ -104,19 +122,19 @@
     # #################################@####################################################
     timeout_ms = 200
     max_retry = 3
     req = AcpHub.acp_idl.Request()
     req.read_req.length = 1234
     response = AcpHub.acp_idl.Response()
     req.read_req.id_group = AcpHub.acp_idl.enumdef.Idgroups.IGR_INVALID
-  
+
     acpclient = AcpHub.AcpClient(0,"CSRCL")
     acpclient.call(req,response,timeout_ms,max_retry)
     print(response.read_resp)
-  
+
 if __name__ == "__main__":
     main()
 ```
 
 Server:
 
 ```Python
@@ -130,21 +148,21 @@
     request.parse(data_bytes[:])
     response = AcpHub.acp_idl.Response()
     testresponse = AcpHub.acp_idl.Response()
     response.read_resp.result = AcpHub.acp_idl.enumdef.Errors.ACP_ERR_OK
     response.read_resp.data = b'application111'
     stream = response.SerializeToString()
     print(stream)
-  
+
     response_len = len(stream)
     AcpHub.pyacp.ffi.memmove(resp, stream, response_len)
 
     resp_len[0] = response_len
     RESPBYTES = AcpHub.pyacp.ffi.buffer(resp,resp_len[0])
-  
+
 def main():
     print("server")
     server = AcpHub.AcpServer(0,"CSRCL",server_callback,1000)
     server.run()
     while True:
         time.sleep(1)
 
@@ -162,15 +180,15 @@
 def main():
     print("publisher")
     publish = AcpHub.AcpPublisher(0,"PubSub")
     req = AcpHub.acp_idl.Request()
     req.read_req.id_group = AcpHub.acp_idl.enumdef.Idgroups.IGR_INVALID
     req.read_req.offset = 0
     req.read_req.length = 1111
-  
+
     while publish.hassubscribers() != True :
         print("has no subscribers")
         time.sleep(1)
     i = 0
     while (True):
         i+=1
         publish.publish(req)
@@ -190,23 +208,22 @@
 import time
 import AcpHub
 @AcpHub.pyacp.ffi.callback("void(const char *msg, uint64_t msg_len)")
 def sub_callback(msg, msg_len):
     requset = AcpHub.acp_idl.Request()
     requset.parse(AcpHub.pyacp.ffi.string(msg))
     print("Request length : ",requset.read_req.length)
-  
+
 def main():
     print("Sub")
     subscribe = AcpHub.AcpSubscriber(0,"PubSub",sub_callback)
     if AcpHub.acp_idl.enumdef.Errors.ACP_ERR_OK != subscribe.listen():
         print("Error subscription")
         return
     i = 0
     while True:
         i+=1
         time.sleep(0.5)
-  
-  
+
+
 if __name__ == "__main__":
     main()
-```
```

### Comparing `pyacp-0.2.1/README.md` & `pyacp-0.2.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,14 @@
-***Attention:***
+# ACP HELLO
 
-1.下载方法：pip install pyacp
+## 一.**Python ****ACP**** overview**
 
-2.引用时需要：import AcpHub
+Acp 提供了多语言的接口版本，本文在于详细描述各个接口作用，以及使用方法和依赖。
 
-3.pyacp:默认下载了cffi,betterproto,protobuf,且指定版本，请自行避免版本冲突（建议在venv中操作）
-
-4.特别需要注意的是：AcpHub包中已经包含了所有需要的包，引用时请直接：
-
-AcpHub.pyacp.ffi.callback（用于注册callback） 或者Acp.acp\_idl（用于引用协议内容）等等
-
-# **一**.  **Python ****ACP**** overview**
-
-Acp 提供了多语言的接口版本，本章在于详细描述各个接口作用，以及使用方法和依赖。
-
-具体有关基本协议部分请参考：[ACP 通信协议详解](https://bd3ubzo9h2.feishu.cn/docx/EmGxdor9Zoqp4px30zhcT1kJnvf)
-
-# **二. 数据流转与关键接口流程图：**
-
-1. ## **c/s架构下的流程图**
-
-**暂时无法在飞书文档外展示此内容**
-
-2. ## **发布订阅模式下的流程图：**
-
-**暂时无法在飞书文档外展示此内容**
-
-# **三. 关键接口汇总与解析：**
+## **二. 关键接口汇总与解析：**
 
 ```Python
 import pyacp
 import acp_idl # 此包为内置包，数据协议的基本，使用response与request时请引用
                #举例：AcpHub.acp_idl.Request() 等等
 from typing import Union
 class AcpClient:#Client类，客户端类，作为客户端主动请求Server
@@ -51,38 +29,78 @@
     def __init__(self,device_id: Union[int],topic: Union[str],callback,resp_data_size:Union[int]):
     #run方法： 启动server的监听机制，启动后进程需主动操作使其常驻而不退出。
     def run(self):
     #stop方法：server 端主动停止监听
     def stop(self):
     #destroy方法：server主动销毁本server
     def destroy(self):
-  
+
 class AcpSubscriber:#发布订阅模式下的订阅端，用于接收发布者发布的数据
     #构造函数：device id与topic 确定唯一通信端，callback为回调函数，在流程图中有具体的声明与实现方法。
     def __init__(self,device_id: Union[int],topic: Union[str],callback):
     #listen：开启对发布者发布数据的监听
     def listen(self):
     #stop：主动停止监听
     def stop(self):
     #destory:销毁当前订阅端
     def destory(self):
-      
+
 class AcpPublisher:#发布订阅模式下的发布端，用于发布数据给接受者，支持一对多
-  
+
     #构造函数： device id与topic唯一确定通信端。
     def __init__(self,device_id: Union[int],topic: Union[str]):
     #publish：主动推送数据，数据类型要和订阅端一致。ps:Request 和Response在这里不是请求和响应的意思，而是为了统一数据类型。换而言之，用Request和Response完全取决于用户需要
     def publish(self,message : Union[acp_idl.Request,acp_idl.Response]):
     #hassubscribers： 查看是否有订阅端等待接收数据，建议在真正发布数据前使用，并在检查到订阅端后再发布数据，避免不必要的资源浪费。
     def hassubscribers(self):
     #destroy：主动销毁发布端。
     def destroy(self):
 ```
 
-四.具体的代码示例，请结合上述所有资料理解。
+## 三. 协议描述
+
+acp 整体 具备cs请求应答模式以及发布订阅模式，其通信规则由proto协定。
+
+基础通信框架下需要以AcpHub.acp_idl中定义好的Request以及Response为数据载体，其中包含data字段的协议模块，用户可以自己使用proto定义自己的协议内容并通过序列化放置在载体内。
+
+其中request和response载体模块中，定义了一系列针对不同场景的协议块，如下
+
+```
+read_req <--------> read_resp
+write_req <------->write_resp
+add_notify_req<------->add_notify_resp
+del_notify_req<------->del_notify_resp
+read_state_req<------->read_state_resp
+write_ctrl_req<------->write_ctrl_resp
+read_write_req<------->read_write_resp
+```
+
+用户可以自行选择需要的模块进行通信。
+
+以write_req举例：
+
+write_req包含如下字段：
+
+```
+id_group uint64 #使用时用于标记请求的具体目标，请自行定义枚举传入或使用已经定义好的业务方的枚举
+offset   int    # 数据偏移量
+length   int    # 数据长度
+data     bytes  # 用于传入业务方协议定义后的序列化数据
+
+```
+
+代码如下：
+
+```
+    req = pyacp.acp_idl.Request()
+    req.write_req.id_group = pyacp.acp_idl.enumdef.Idgroups.IGR_INVALID
+    req.write_req.length = 123
+```
+
+## 四.具体的代码示例，请结合上述所有资料理解。
 
 client:
 
 ```Python
 from datetime import date
 import sys
 import AcpHub
@@ -94,19 +112,19 @@
     # #################################@####################################################
     timeout_ms = 200
     max_retry = 3
     req = AcpHub.acp_idl.Request()
     req.read_req.length = 1234
     response = AcpHub.acp_idl.Response()
     req.read_req.id_group = AcpHub.acp_idl.enumdef.Idgroups.IGR_INVALID
-  
+
     acpclient = AcpHub.AcpClient(0,"CSRCL")
     acpclient.call(req,response,timeout_ms,max_retry)
     print(response.read_resp)
-  
+
 if __name__ == "__main__":
     main()
 ```
 
 Server:
 
 ```Python
@@ -120,21 +138,21 @@
     request.parse(data_bytes[:])
     response = AcpHub.acp_idl.Response()
     testresponse = AcpHub.acp_idl.Response()
     response.read_resp.result = AcpHub.acp_idl.enumdef.Errors.ACP_ERR_OK
     response.read_resp.data = b'application111'
     stream = response.SerializeToString()
     print(stream)
-  
+
     response_len = len(stream)
     AcpHub.pyacp.ffi.memmove(resp, stream, response_len)
 
     resp_len[0] = response_len
     RESPBYTES = AcpHub.pyacp.ffi.buffer(resp,resp_len[0])
-  
+
 def main():
     print("server")
     server = AcpHub.AcpServer(0,"CSRCL",server_callback,1000)
     server.run()
     while True:
         time.sleep(1)
 
@@ -152,15 +170,15 @@
 def main():
     print("publisher")
     publish = AcpHub.AcpPublisher(0,"PubSub")
     req = AcpHub.acp_idl.Request()
     req.read_req.id_group = AcpHub.acp_idl.enumdef.Idgroups.IGR_INVALID
     req.read_req.offset = 0
     req.read_req.length = 1111
-  
+
     while publish.hassubscribers() != True :
         print("has no subscribers")
         time.sleep(1)
     i = 0
     while (True):
         i+=1
         publish.publish(req)
@@ -180,23 +198,22 @@
 import time
 import AcpHub
 @AcpHub.pyacp.ffi.callback("void(const char *msg, uint64_t msg_len)")
 def sub_callback(msg, msg_len):
     requset = AcpHub.acp_idl.Request()
     requset.parse(AcpHub.pyacp.ffi.string(msg))
     print("Request length : ",requset.read_req.length)
-  
+
 def main():
     print("Sub")
     subscribe = AcpHub.AcpSubscriber(0,"PubSub",sub_callback)
     if AcpHub.acp_idl.enumdef.Errors.ACP_ERR_OK != subscribe.listen():
         print("Error subscription")
         return
     i = 0
     while True:
         i+=1
         time.sleep(0.5)
-  
-  
+
+
 if __name__ == "__main__":
-    main()
-```
+    main()
```

### Comparing `pyacp-0.2.1/acp_idl.py` & `pyacp-0.2.2/acp_idl.py`

 * *Files identical despite different names*

### Comparing `pyacp-0.2.1/acp_libs/lib/linux/libacp-c.so` & `pyacp-0.2.2/acp_libs/lib/linux/libacp-c.so`

 * *Files identical despite different names*

### Comparing `pyacp-0.2.1/acp_libs/lib/linux/libacp-core.so` & `pyacp-0.2.2/acp_libs/lib/linux/libacp-core.so`

 * *Files identical despite different names*

### Comparing `pyacp-0.2.1/acp_libs/lib/win/acp-c.dll` & `pyacp-0.2.2/acp_libs/lib/win/acp-c.dll`

 * *Files identical despite different names*

### Comparing `pyacp-0.2.1/acp_libs/lib/win/acp-core.dll` & `pyacp-0.2.2/acp_libs/lib/win/acp-core.dll`

 * *Files identical despite different names*

### Comparing `pyacp-0.2.1/enumdef.py` & `pyacp-0.2.2/enumdef.py`

 * *Files identical despite different names*

### Comparing `pyacp-0.2.1/notify.py` & `pyacp-0.2.2/notify.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import betterproto
 
 import enumdef
 
 
 @dataclass
 class AddNotificationRequest(betterproto.Message):
-    id_group: enumdef.Idgroups = betterproto.enum_field(1)
+    id_group: int = betterproto.uint64_field(1)
     offset: int = betterproto.uint32_field(2)
     length: int = betterproto.uint32_field(3)
     max_delay: int = betterproto.uint32_field(4)
     cycle_time: int = betterproto.uint32_field(5)
     data: bytes = betterproto.bytes_field(6)
```

### Comparing `pyacp-0.2.1/pyacp.egg-info/PKG-INFO` & `pyacp-0.2.2/pyacp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,24 @@
 Metadata-Version: 2.1
 Name: pyacp
-Version: 0.2.1
+Version: 0.2.2
 Summary: python fastdds acp api
 Author: Li Meng
 Description-Content-Type: text/markdown
 Requires-Dist: protobuf==3.19.5
 Requires-Dist: cffi==1.15.1
 Requires-Dist: betterproto==1.2.5
 
-***Attention:***
+# ACP HELLO
 
-1.下载方法：pip install pyacp
+## 一.**Python ****ACP**** overview**
 
-2.引用时需要：import AcpHub
+Acp 提供了多语言的接口版本，本文在于详细描述各个接口作用，以及使用方法和依赖。
 
-3.pyacp:默认下载了cffi,betterproto,protobuf,且指定版本，请自行避免版本冲突（建议在venv中操作）
-
-4.特别需要注意的是：AcpHub包中已经包含了所有需要的包，引用时请直接：
-
-AcpHub.pyacp.ffi.callback（用于注册callback） 或者Acp.acp\_idl（用于引用协议内容）等等
-
-# **一**.  **Python ****ACP**** overview**
-
-Acp 提供了多语言的接口版本，本章在于详细描述各个接口作用，以及使用方法和依赖。
-
-具体有关基本协议部分请参考：[ACP 通信协议详解](https://bd3ubzo9h2.feishu.cn/docx/EmGxdor9Zoqp4px30zhcT1kJnvf)
-
-# **二. 数据流转与关键接口流程图：**
-
-1. ## **c/s架构下的流程图**
-
-**暂时无法在飞书文档外展示此内容**
-
-2. ## **发布订阅模式下的流程图：**
-
-**暂时无法在飞书文档外展示此内容**
-
-# **三. 关键接口汇总与解析：**
+## **二. 关键接口汇总与解析：**
 
 ```Python
 import pyacp
 import acp_idl # 此包为内置包，数据协议的基本，使用response与request时请引用
                #举例：AcpHub.acp_idl.Request() 等等
 from typing import Union
 class AcpClient:#Client类，客户端类，作为客户端主动请求Server
@@ -61,38 +39,78 @@
     def __init__(self,device_id: Union[int],topic: Union[str],callback,resp_data_size:Union[int]):
     #run方法： 启动server的监听机制，启动后进程需主动操作使其常驻而不退出。
     def run(self):
     #stop方法：server 端主动停止监听
     def stop(self):
     #destroy方法：server主动销毁本server
     def destroy(self):
-  
+
 class AcpSubscriber:#发布订阅模式下的订阅端，用于接收发布者发布的数据
     #构造函数：device id与topic 确定唯一通信端，callback为回调函数，在流程图中有具体的声明与实现方法。
     def __init__(self,device_id: Union[int],topic: Union[str],callback):
     #listen：开启对发布者发布数据的监听
     def listen(self):
     #stop：主动停止监听
     def stop(self):
     #destory:销毁当前订阅端
     def destory(self):
-      
+
 class AcpPublisher:#发布订阅模式下的发布端，用于发布数据给接受者，支持一对多
-  
+
     #构造函数： device id与topic唯一确定通信端。
     def __init__(self,device_id: Union[int],topic: Union[str]):
     #publish：主动推送数据，数据类型要和订阅端一致。ps:Request 和Response在这里不是请求和响应的意思，而是为了统一数据类型。换而言之，用Request和Response完全取决于用户需要
     def publish(self,message : Union[acp_idl.Request,acp_idl.Response]):
     #hassubscribers： 查看是否有订阅端等待接收数据，建议在真正发布数据前使用，并在检查到订阅端后再发布数据，避免不必要的资源浪费。
     def hassubscribers(self):
     #destroy：主动销毁发布端。
     def destroy(self):
 ```
 
-四.具体的代码示例，请结合上述所有资料理解。
+## 三. 协议描述
+
+acp 整体 具备cs请求应答模式以及发布订阅模式，其通信规则由proto协定。
+
+基础通信框架下需要以AcpHub.acp_idl中定义好的Request以及Response为数据载体，其中包含data字段的协议模块，用户可以自己使用proto定义自己的协议内容并通过序列化放置在载体内。
+
+其中request和response载体模块中，定义了一系列针对不同场景的协议块，如下
+
+```
+read_req <--------> read_resp
+write_req <------->write_resp
+add_notify_req<------->add_notify_resp
+del_notify_req<------->del_notify_resp
+read_state_req<------->read_state_resp
+write_ctrl_req<------->write_ctrl_resp
+read_write_req<------->read_write_resp
+```
+
+用户可以自行选择需要的模块进行通信。
+
+以write_req举例：
+
+write_req包含如下字段：
+
+```
+id_group uint64 #使用时用于标记请求的具体目标，请自行定义枚举传入或使用已经定义好的业务方的枚举
+offset   int    # 数据偏移量
+length   int    # 数据长度
+data     bytes  # 用于传入业务方协议定义后的序列化数据
+
+```
+
+代码如下：
+
+```
+    req = pyacp.acp_idl.Request()
+    req.write_req.id_group = pyacp.acp_idl.enumdef.Idgroups.IGR_INVALID
+    req.write_req.length = 123
+```
+
+## 四.具体的代码示例，请结合上述所有资料理解。
 
 client:
 
 ```Python
 from datetime import date
 import sys
 import AcpHub
@@ -104,19 +122,19 @@
     # #################################@####################################################
     timeout_ms = 200
     max_retry = 3
     req = AcpHub.acp_idl.Request()
     req.read_req.length = 1234
     response = AcpHub.acp_idl.Response()
     req.read_req.id_group = AcpHub.acp_idl.enumdef.Idgroups.IGR_INVALID
-  
+
     acpclient = AcpHub.AcpClient(0,"CSRCL")
     acpclient.call(req,response,timeout_ms,max_retry)
     print(response.read_resp)
-  
+
 if __name__ == "__main__":
     main()
 ```
 
 Server:
 
 ```Python
@@ -130,21 +148,21 @@
     request.parse(data_bytes[:])
     response = AcpHub.acp_idl.Response()
     testresponse = AcpHub.acp_idl.Response()
     response.read_resp.result = AcpHub.acp_idl.enumdef.Errors.ACP_ERR_OK
     response.read_resp.data = b'application111'
     stream = response.SerializeToString()
     print(stream)
-  
+
     response_len = len(stream)
     AcpHub.pyacp.ffi.memmove(resp, stream, response_len)
 
     resp_len[0] = response_len
     RESPBYTES = AcpHub.pyacp.ffi.buffer(resp,resp_len[0])
-  
+
 def main():
     print("server")
     server = AcpHub.AcpServer(0,"CSRCL",server_callback,1000)
     server.run()
     while True:
         time.sleep(1)
 
@@ -162,15 +180,15 @@
 def main():
     print("publisher")
     publish = AcpHub.AcpPublisher(0,"PubSub")
     req = AcpHub.acp_idl.Request()
     req.read_req.id_group = AcpHub.acp_idl.enumdef.Idgroups.IGR_INVALID
     req.read_req.offset = 0
     req.read_req.length = 1111
-  
+
     while publish.hassubscribers() != True :
         print("has no subscribers")
         time.sleep(1)
     i = 0
     while (True):
         i+=1
         publish.publish(req)
@@ -190,23 +208,22 @@
 import time
 import AcpHub
 @AcpHub.pyacp.ffi.callback("void(const char *msg, uint64_t msg_len)")
 def sub_callback(msg, msg_len):
     requset = AcpHub.acp_idl.Request()
     requset.parse(AcpHub.pyacp.ffi.string(msg))
     print("Request length : ",requset.read_req.length)
-  
+
 def main():
     print("Sub")
     subscribe = AcpHub.AcpSubscriber(0,"PubSub",sub_callback)
     if AcpHub.acp_idl.enumdef.Errors.ACP_ERR_OK != subscribe.listen():
         print("Error subscription")
         return
     i = 0
     while True:
         i+=1
         time.sleep(0.5)
-  
-  
+
+
 if __name__ == "__main__":
     main()
-```
```

### Comparing `pyacp-0.2.1/pyacp.egg-info/SOURCES.txt` & `pyacp-0.2.2/pyacp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyacp-0.2.1/pyacp.py` & `pyacp-0.2.2/pyacp.py`

 * *Files identical despite different names*

### Comparing `pyacp-0.2.1/read.py` & `pyacp-0.2.2/read.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import betterproto
 
 import enumdef
 
 
 @dataclass
 class ReadRequest(betterproto.Message):
-    id_group: enumdef.Idgroups = betterproto.enum_field(1)
+    id_group: int = betterproto.uint64_field(1)
     offset: int = betterproto.uint32_field(2)
     length: int = betterproto.uint32_field(3)
     data: bytes = betterproto.bytes_field(4)
 
 
 @dataclass
 class ReadResponse(betterproto.Message):
```

### Comparing `pyacp-0.2.1/readwrite.py` & `pyacp-0.2.2/write.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# sources: acp_read_write.proto
+# sources: acp_write.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
 
 import betterproto
 
 import enumdef
 
 
 @dataclass
-class ReadWriteRequest(betterproto.Message):
-    id_group: enumdef.Idgroups = betterproto.enum_field(1)
+class WriteRequest(betterproto.Message):
+    id_group: int = betterproto.uint64_field(1)
     offset: int = betterproto.uint32_field(2)
     length: int = betterproto.uint32_field(3)
     data: bytes = betterproto.bytes_field(4)
 
 
 @dataclass
-class ReadWriteResponse(betterproto.Message):
+class WriteResponse(betterproto.Message):
     result: enumdef.Errors = betterproto.enum_field(1)
-    data: bytes = betterproto.bytes_field(2)
```

### Comparing `pyacp-0.2.1/resettime.py` & `pyacp-0.2.2/resettime.py`

 * *Files identical despite different names*

### Comparing `pyacp-0.2.1/setup.py` & `pyacp-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 setup(
     name='pyacp',
-    version='0.2.1',
+    version='0.2.2',
     author='Li Meng',
     description='python fastdds acp api',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=['.',"acp_libs/lib/","acp_libs/lib/linux/","acp_libs/lib/win/"],
     package_data={
         'acp_libs/lib/linux/': ['libacp-c.so','libacp-core.so'],  # 包含的文件列表
         'acp_libs/lib/win/' : ['acp-c.dll','acp-core.dll']
     },
     install_requires=[
         'protobuf==3.19.5',
         'cffi==1.15.1',
         'betterproto==1.2.5'
     ],
-)       
+)
```

### Comparing `pyacp-0.2.1/write.py` & `pyacp-0.2.2/readwrite.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# sources: acp_write.proto
+# sources: acp_read_write.proto
 # plugin: python-betterproto
 from dataclasses import dataclass
 
 import betterproto
 
 import enumdef
 
 
 @dataclass
-class WriteRequest(betterproto.Message):
-    id_group: enumdef.Idgroups = betterproto.enum_field(1)
+class ReadWriteRequest(betterproto.Message):
+    id_group: int = betterproto.uint64_field(1)
     offset: int = betterproto.uint32_field(2)
     length: int = betterproto.uint32_field(3)
     data: bytes = betterproto.bytes_field(4)
 
 
 @dataclass
-class WriteResponse(betterproto.Message):
+class ReadWriteResponse(betterproto.Message):
     result: enumdef.Errors = betterproto.enum_field(1)
+    data: bytes = betterproto.bytes_field(2)
```

### Comparing `pyacp-0.2.1/write_ctrl.py` & `pyacp-0.2.2/write_ctrl.py`

 * *Files identical despite different names*


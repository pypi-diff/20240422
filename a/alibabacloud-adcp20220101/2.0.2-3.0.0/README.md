# Comparing `tmp/alibabacloud_adcp20220101-2.0.2.tar.gz` & `tmp/alibabacloud_adcp20220101-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_adcp20220101-2.0.2.tar", last modified: Thu Oct 12 17:16:35 2023, max compression
+gzip compressed data, was "dist/alibabacloud_adcp20220101-3.0.0.tar", last modified: Mon Apr 22 02:57:54 2024, max compression
```

## Comparing `alibabacloud_adcp20220101-2.0.2.tar` & `alibabacloud_adcp20220101-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-12 17:16:35.000000 alibabacloud_adcp20220101-2.0.2/
--rw-r--r--   0 root         (0) root         (0)     1074 2023-10-12 17:16:34.000000 alibabacloud_adcp20220101-2.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-10-12 17:16:34.000000 alibabacloud_adcp20220101-2.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-10-12 17:16:34.000000 alibabacloud_adcp20220101-2.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2334 2023-10-12 17:16:35.000000 alibabacloud_adcp20220101-2.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2023-10-12 17:16:34.000000 alibabacloud_adcp20220101-2.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1110 2023-10-12 17:16:34.000000 alibabacloud_adcp20220101-2.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-12 17:16:35.000000 alibabacloud_adcp20220101-2.0.2/alibabacloud_adcp20220101/
--rw-r--r--   0 root         (0) root         (0)       21 2023-10-12 17:16:34.000000 alibabacloud_adcp20220101-2.0.2/alibabacloud_adcp20220101/__init__.py
--rw-r--r--   0 root         (0) root         (0)    79838 2023-10-12 17:16:34.000000 alibabacloud_adcp20220101-2.0.2/alibabacloud_adcp20220101/client.py
--rw-r--r--   0 root         (0) root         (0)   197635 2023-10-12 17:16:34.000000 alibabacloud_adcp20220101-2.0.2/alibabacloud_adcp20220101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-12 17:16:35.000000 alibabacloud_adcp20220101-2.0.2/alibabacloud_adcp20220101.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2334 2023-10-12 17:16:35.000000 alibabacloud_adcp20220101-2.0.2/alibabacloud_adcp20220101.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2023-10-12 17:16:35.000000 alibabacloud_adcp20220101-2.0.2/alibabacloud_adcp20220101.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-12 17:16:35.000000 alibabacloud_adcp20220101-2.0.2/alibabacloud_adcp20220101.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-10-12 17:16:35.000000 alibabacloud_adcp20220101-2.0.2/alibabacloud_adcp20220101.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-10-12 17:16:35.000000 alibabacloud_adcp20220101-2.0.2/alibabacloud_adcp20220101.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-10-12 17:16:35.000000 alibabacloud_adcp20220101-2.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2616 2023-10-12 17:16:34.000000 alibabacloud_adcp20220101-2.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 02:57:54.000000 alibabacloud_adcp20220101-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-04-22 02:57:53.000000 alibabacloud_adcp20220101-3.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-22 02:57:53.000000 alibabacloud_adcp20220101-3.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-22 02:57:53.000000 alibabacloud_adcp20220101-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-04-22 02:57:54.000000 alibabacloud_adcp20220101-3.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1099 2024-04-22 02:57:53.000000 alibabacloud_adcp20220101-3.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-04-22 02:57:53.000000 alibabacloud_adcp20220101-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 02:57:54.000000 alibabacloud_adcp20220101-3.0.0/alibabacloud_adcp20220101/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-22 02:57:53.000000 alibabacloud_adcp20220101-3.0.0/alibabacloud_adcp20220101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81543 2024-04-22 02:57:53.000000 alibabacloud_adcp20220101-3.0.0/alibabacloud_adcp20220101/client.py
+-rw-r--r--   0 root         (0) root         (0)   208339 2024-04-22 02:57:53.000000 alibabacloud_adcp20220101-3.0.0/alibabacloud_adcp20220101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 02:57:54.000000 alibabacloud_adcp20220101-3.0.0/alibabacloud_adcp20220101.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-04-22 02:57:54.000000 alibabacloud_adcp20220101-3.0.0/alibabacloud_adcp20220101.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2024-04-22 02:57:54.000000 alibabacloud_adcp20220101-3.0.0/alibabacloud_adcp20220101.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 02:57:54.000000 alibabacloud_adcp20220101-3.0.0/alibabacloud_adcp20220101.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-22 02:57:54.000000 alibabacloud_adcp20220101-3.0.0/alibabacloud_adcp20220101.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-22 02:57:54.000000 alibabacloud_adcp20220101-3.0.0/alibabacloud_adcp20220101.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-22 02:57:54.000000 alibabacloud_adcp20220101-3.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2616 2024-04-22 02:57:53.000000 alibabacloud_adcp20220101-3.0.0/setup.py
```

### Comparing `alibabacloud_adcp20220101-2.0.2/ChangeLog.md` & `alibabacloud_adcp20220101-3.0.0/ChangeLog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-10-12 Version: 2.0.2
+- Generated python 2022-01-01 for adcp.
+
 2023-09-13 Version: 2.0.1
 - Generated python 2022-01-01 for adcp.
 
 2023-08-10 Version: 2.0.0
 - UpdateHubClusterFeature support ArgoCDHAEnabled.
```

### Comparing `alibabacloud_adcp20220101-2.0.2/LICENSE` & `alibabacloud_adcp20220101-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_adcp20220101-2.0.2/PKG-INFO` & `alibabacloud_adcp20220101-3.0.0/alibabacloud_adcp20220101.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_adcp20220101
-Version: 2.0.2
+Name: alibabacloud-adcp20220101
+Version: 3.0.0
 Summary: Alibaba Cloud adcp (20220101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/adcp-20220101/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_adcp20220101-2.0.2/README-CN.md` & `alibabacloud_adcp20220101-3.0.0/README-CN.md`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ## 使用说明
 
 [快速使用](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-CN.md#%E5%BF%AB%E9%80%9F%E4%BD%BF%E7%94%A8)
 
 ## 发行说明
 
-每个版本的详细更改记录在[发行说明](./ChangeLog.md)中。
+每个版本的详细更改记录在[发行说明](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/adcp-20220101/ChangeLog.md)中。
 
 ## 相关
 
 - [最新源码](https://github.com/aliyun/alibabacloud-python-sdk/)
 
 ## 许可证
```

### Comparing `alibabacloud_adcp20220101-2.0.2/README.md` & `alibabacloud_adcp20220101-3.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ## Usage
 
 [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
 
 ## Changelog
 
-Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/adcp-20220101/ChangeLog.md).
 
 ## References
 
 - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
 
 ## License
```

### Comparing `alibabacloud_adcp20220101-2.0.2/alibabacloud_adcp20220101/client.py` & `alibabacloud_adcp20220101-3.0.0/alibabacloud_adcp20220101/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     *\
     """
     def __init__(
         self, 
         config: open_api_models.Config,
     ):
         super().__init__(config)
-        self._signature_algorithm = 'v2'
         self._endpoint_rule = 'central'
         self._endpoint_map = {
             'cn-beijing': 'adcp.cn-beijing.aliyuncs.com',
             'cn-zhangjiakou': 'adcp.cn-zhangjiakou.aliyuncs.com',
             'cn-hangzhou': 'adcp.cn-hangzhou.aliyuncs.com',
             'cn-shanghai': 'adcp.cn-shanghai.aliyuncs.com',
             'cn-shenzhen': 'adcp.cn-shenzhen.aliyuncs.com',
@@ -168,14 +167,16 @@
             body['Name'] = request.name
         if not UtilClient.is_unset(request.price_limit):
             body['PriceLimit'] = request.price_limit
         if not UtilClient.is_unset(request.profile):
             body['Profile'] = request.profile
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_group_id):
+            body['ResourceGroupID'] = request.resource_group_id
         if not UtilClient.is_unset(request.v_switches):
             body['VSwitches'] = request.v_switches
         if not UtilClient.is_unset(request.vpc_id):
             body['VpcId'] = request.vpc_id
         if not UtilClient.is_unset(request.workflow_schedule_mode):
             body['WorkflowScheduleMode'] = request.workflow_schedule_mode
         req = open_api_models.OpenApiRequest(
@@ -216,14 +217,16 @@
             body['Name'] = request.name
         if not UtilClient.is_unset(request.price_limit):
             body['PriceLimit'] = request.price_limit
         if not UtilClient.is_unset(request.profile):
             body['Profile'] = request.profile
         if not UtilClient.is_unset(request.region_id):
             body['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_group_id):
+            body['ResourceGroupID'] = request.resource_group_id
         if not UtilClient.is_unset(request.v_switches):
             body['VSwitches'] = request.v_switches
         if not UtilClient.is_unset(request.vpc_id):
             body['VpcId'] = request.vpc_id
         if not UtilClient.is_unset(request.workflow_schedule_mode):
             body['WorkflowScheduleMode'] = request.workflow_schedule_mode
         req = open_api_models.OpenApiRequest(
@@ -822,14 +825,16 @@
         request: adcp_20220101_models.DescribeHubClustersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> adcp_20220101_models.DescribeHubClustersResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.profile):
             query['Profile'] = request.profile
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeHubClusters',
             version='2022-01-01',
             protocol='HTTPS',
@@ -850,14 +855,16 @@
         request: adcp_20220101_models.DescribeHubClustersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> adcp_20220101_models.DescribeHubClustersResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.profile):
             query['Profile'] = request.profile
+        if not UtilClient.is_unset(request.resource_group_id):
+            query['ResourceGroupId'] = request.resource_group_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeHubClusters',
             version='2022-01-01',
             protocol='HTTPS',
@@ -1600,14 +1607,22 @@
         return await self.grant_user_permission_with_options_async(request, runtime)
 
     def grant_user_permissions_with_options(
         self,
         tmp_req: adcp_20220101_models.GrantUserPermissionsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> adcp_20220101_models.GrantUserPermissionsResponse:
+        """
+        @deprecated : GrantUserPermissions is deprecated, please use adcp::2022-01-01::GrantUserPermission instead.
+        
+        @param tmp_req: GrantUserPermissionsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GrantUserPermissionsResponse
+        Deprecated
+        """
         UtilClient.validate_model(tmp_req)
         request = adcp_20220101_models.GrantUserPermissionsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.permissions):
             request.permissions_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.permissions, 'Permissions', 'json')
         query = {}
         if not UtilClient.is_unset(request.permissions_shrink):
@@ -1634,14 +1649,22 @@
         )
 
     async def grant_user_permissions_with_options_async(
         self,
         tmp_req: adcp_20220101_models.GrantUserPermissionsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> adcp_20220101_models.GrantUserPermissionsResponse:
+        """
+        @deprecated : GrantUserPermissions is deprecated, please use adcp::2022-01-01::GrantUserPermission instead.
+        
+        @param tmp_req: GrantUserPermissionsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GrantUserPermissionsResponse
+        Deprecated
+        """
         UtilClient.validate_model(tmp_req)
         request = adcp_20220101_models.GrantUserPermissionsShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.permissions):
             request.permissions_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.permissions, 'Permissions', 'json')
         query = {}
         if not UtilClient.is_unset(request.permissions_shrink):
@@ -1667,21 +1690,35 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def grant_user_permissions(
         self,
         request: adcp_20220101_models.GrantUserPermissionsRequest,
     ) -> adcp_20220101_models.GrantUserPermissionsResponse:
+        """
+        @deprecated : GrantUserPermissions is deprecated, please use adcp::2022-01-01::GrantUserPermission instead.
+        
+        @param request: GrantUserPermissionsRequest
+        @return: GrantUserPermissionsResponse
+        Deprecated
+        """
         runtime = util_models.RuntimeOptions()
         return self.grant_user_permissions_with_options(request, runtime)
 
     async def grant_user_permissions_async(
         self,
         request: adcp_20220101_models.GrantUserPermissionsRequest,
     ) -> adcp_20220101_models.GrantUserPermissionsResponse:
+        """
+        @deprecated : GrantUserPermissions is deprecated, please use adcp::2022-01-01::GrantUserPermission instead.
+        
+        @param request: GrantUserPermissionsRequest
+        @return: GrantUserPermissionsResponse
+        Deprecated
+        """
         runtime = util_models.RuntimeOptions()
         return await self.grant_user_permissions_with_options_async(request, runtime)
 
     def update_hub_cluster_feature_with_options(
         self,
         tmp_req: adcp_20220101_models.UpdateHubClusterFeatureRequest,
         runtime: util_models.RuntimeOptions,
@@ -1710,16 +1747,16 @@
             query['AuditLogEnabled'] = request.audit_log_enabled
         if not UtilClient.is_unset(request.cluster_id):
             query['ClusterId'] = request.cluster_id
         if not UtilClient.is_unset(request.deletion_protection):
             query['DeletionProtection'] = request.deletion_protection
         if not UtilClient.is_unset(request.enable_mesh):
             query['EnableMesh'] = request.enable_mesh
-        if not UtilClient.is_unset(request.mseenabled):
-            query['MSEEnabled'] = request.mseenabled
+        if not UtilClient.is_unset(request.gateway_enabled):
+            query['GatewayEnabled'] = request.gateway_enabled
         if not UtilClient.is_unset(request.monitor_enabled):
             query['MonitorEnabled'] = request.monitor_enabled
         if not UtilClient.is_unset(request.name):
             query['Name'] = request.name
         if not UtilClient.is_unset(request.price_limit):
             query['PriceLimit'] = request.price_limit
         if not UtilClient.is_unset(request.public_access_enabled):
@@ -1778,16 +1815,16 @@
             query['AuditLogEnabled'] = request.audit_log_enabled
         if not UtilClient.is_unset(request.cluster_id):
             query['ClusterId'] = request.cluster_id
         if not UtilClient.is_unset(request.deletion_protection):
             query['DeletionProtection'] = request.deletion_protection
         if not UtilClient.is_unset(request.enable_mesh):
             query['EnableMesh'] = request.enable_mesh
-        if not UtilClient.is_unset(request.mseenabled):
-            query['MSEEnabled'] = request.mseenabled
+        if not UtilClient.is_unset(request.gateway_enabled):
+            query['GatewayEnabled'] = request.gateway_enabled
         if not UtilClient.is_unset(request.monitor_enabled):
             query['MonitorEnabled'] = request.monitor_enabled
         if not UtilClient.is_unset(request.name):
             query['Name'] = request.name
         if not UtilClient.is_unset(request.price_limit):
             query['PriceLimit'] = request.price_limit
         if not UtilClient.is_unset(request.public_access_enabled):
```

### Comparing `alibabacloud_adcp20220101-2.0.2/alibabacloud_adcp20220101/models.py` & `alibabacloud_adcp20220101-3.0.0/alibabacloud_adcp20220101/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,17 +102,14 @@
         body: AttachClusterToHubResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -145,47 +142,59 @@
         argo_server_enabled: bool = None,
         audit_log_enabled: bool = None,
         is_enterprise_security_group: bool = None,
         name: str = None,
         price_limit: str = None,
         profile: str = None,
         region_id: str = None,
+        resource_group_id: str = None,
         v_switches: str = None,
         vpc_id: str = None,
         workflow_schedule_mode: str = None,
     ):
         # Specifies whether to expose the API server to the Internet. Valid values:
         # 
         # *   true: exposes the API server to the Internet.
         # *   false: exposes the API server to the internal network.
         self.api_server_public_eip = api_server_public_eip
+        # Specifies whether to enable the workflow instance UI. This parameter takes effect only if Profile is set to XFlow. Valid values:
+        # 
+        # *   true
+        # *   false
         self.argo_server_enabled = argo_server_enabled
         # Specifies whether to enable the audit log feature. Valid values:
         # 
         # *   true: enables the audit log feature.
         # *   false: disables the audit log feature.
         self.audit_log_enabled = audit_log_enabled
         # Specifies whether to use an advanced security group.
         self.is_enterprise_security_group = is_enterprise_security_group
         # The name of the master instance.
         self.name = name
+        # The limit on the prices of containers in the workflow. This parameter takes effect only if the WorkflowScheduleMode parameter is set to cost-optimized.
         self.price_limit = price_limit
         # The type of scenario for which the master instance is suitable. Valid values:
         # 
         # *   `Default`: The master instance is suitable for standard scenarios.
         # *   `XFlow`: The master instance is suitable for workflow scenarios.
         # 
         # Default value: `Default`.
         self.profile = profile
         # The ID of the region. You can call the DescribeRegions operation to query available regions.
         self.region_id = region_id
+        # The Resource Group ID.
+        self.resource_group_id = resource_group_id
         # The ID of the vSwitch.
         self.v_switches = v_switches
         # The ID of the virtual private cloud (VPC) to which the master instance belongs. You can call the DescribeVpcs operation to query available VPCs.
         self.vpc_id = vpc_id
+        # The scheduling mode of the workflow. This parameter takes effect only if Profile is set to XFlow. Valid values:
+        # 
+        # *   cost-optimized: cost-prioritized scheduling mode.
+        # *   stock-optimized: inventory-prioritized scheduling mode.
         self.workflow_schedule_mode = workflow_schedule_mode
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -205,14 +214,16 @@
             result['Name'] = self.name
         if self.price_limit is not None:
             result['PriceLimit'] = self.price_limit
         if self.profile is not None:
             result['Profile'] = self.profile
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.resource_group_id is not None:
+            result['ResourceGroupID'] = self.resource_group_id
         if self.v_switches is not None:
             result['VSwitches'] = self.v_switches
         if self.vpc_id is not None:
             result['VpcId'] = self.vpc_id
         if self.workflow_schedule_mode is not None:
             result['WorkflowScheduleMode'] = self.workflow_schedule_mode
         return result
@@ -231,14 +242,16 @@
             self.name = m.get('Name')
         if m.get('PriceLimit') is not None:
             self.price_limit = m.get('PriceLimit')
         if m.get('Profile') is not None:
             self.profile = m.get('Profile')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('ResourceGroupID') is not None:
+            self.resource_group_id = m.get('ResourceGroupID')
         if m.get('VSwitches') is not None:
             self.v_switches = m.get('VSwitches')
         if m.get('VpcId') is not None:
             self.vpc_id = m.get('VpcId')
         if m.get('WorkflowScheduleMode') is not None:
             self.workflow_schedule_mode = m.get('WorkflowScheduleMode')
         return self
@@ -294,17 +307,14 @@
         body: CreateHubClusterResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -474,17 +484,14 @@
         body: DeleteHubClusterResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -630,17 +637,14 @@
         body: DeletePolicyInstanceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -737,17 +741,14 @@
         body: DeleteUserPermissionResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -927,17 +928,14 @@
         body: DeployPolicyInstanceResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1032,44 +1030,266 @@
         if m.get('EnabledPublic') is not None:
             self.enabled_public = m.get('EnabledPublic')
         if m.get('LoadBalancerId') is not None:
             self.load_balancer_id = m.get('LoadBalancerId')
         return self
 
 
+class DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaDataACKOneGitOps(TeaModel):
+    def __init__(
+        self,
+        access_control_list: List[str] = None,
+        enabled: bool = None,
+        haenabled: bool = None,
+        public_access_enabled: bool = None,
+    ):
+        # The Internet access control list (ACL). This parameter takes effect only if PublicAccessEnabled is set to true.
+        self.access_control_list = access_control_list
+        # Indicates whether GitOps is enabled. Valid values:
+        # 
+        # *   true: GitOps is enabled.
+        # *   false: GitOps is disabled.
+        self.enabled = enabled
+        # Indicates whether GitOps High Availability is enabled. Valid values:
+        # 
+        # *   true:  GitOps High Availability is enabled.
+        # *   false:  GitOps High Availability is disabled.
+        self.haenabled = haenabled
+        # Specifies whether to enable public domain name resolution in the Argo CD or Argo Workflow console. Valid values:
+        # 
+        # *   true
+        # *   false
+        self.public_access_enabled = public_access_enabled
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.access_control_list is not None:
+            result['AccessControlList'] = self.access_control_list
+        if self.enabled is not None:
+            result['Enabled'] = self.enabled
+        if self.haenabled is not None:
+            result['HAEnabled'] = self.haenabled
+        if self.public_access_enabled is not None:
+            result['PublicAccessEnabled'] = self.public_access_enabled
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AccessControlList') is not None:
+            self.access_control_list = m.get('AccessControlList')
+        if m.get('Enabled') is not None:
+            self.enabled = m.get('Enabled')
+        if m.get('HAEnabled') is not None:
+            self.haenabled = m.get('HAEnabled')
+        if m.get('PublicAccessEnabled') is not None:
+            self.public_access_enabled = m.get('PublicAccessEnabled')
+        return self
+
+
+class DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaDataACKOneWorkFlowArgoWorkflow(TeaModel):
+    def __init__(
+        self,
+        access_control_list: List[str] = None,
+        enabled: bool = None,
+        public_access_enabled: bool = None,
+        server_enabled: str = None,
+    ):
+        # The Internet access control list (ACL). This parameter takes effect only if PublicAccessEnabled is set to true.
+        self.access_control_list = access_control_list
+        # Specifies whether to enable the argo workflow. Valid values:
+        # 
+        # *   **false** (default)
+        # *   **true**\
+        self.enabled = enabled
+        # Specifies whether to enable public domain name resolution in the Argo CD or Argo Workflow console. Valid values:
+        # 
+        # *   true
+        # *   false
+        self.public_access_enabled = public_access_enabled
+        # Specifies whether to enable the argo workflow. UI Valid values:
+        # 
+        # *   **false** (default)
+        # *   **true**\
+        self.server_enabled = server_enabled
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.access_control_list is not None:
+            result['AccessControlList'] = self.access_control_list
+        if self.enabled is not None:
+            result['Enabled'] = self.enabled
+        if self.public_access_enabled is not None:
+            result['PublicAccessEnabled'] = self.public_access_enabled
+        if self.server_enabled is not None:
+            result['ServerEnabled'] = self.server_enabled
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AccessControlList') is not None:
+            self.access_control_list = m.get('AccessControlList')
+        if m.get('Enabled') is not None:
+            self.enabled = m.get('Enabled')
+        if m.get('PublicAccessEnabled') is not None:
+            self.public_access_enabled = m.get('PublicAccessEnabled')
+        if m.get('ServerEnabled') is not None:
+            self.server_enabled = m.get('ServerEnabled')
+        return self
+
+
+class DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaDataACKOneWorkFlow(TeaModel):
+    def __init__(
+        self,
+        argo_workflow: DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaDataACKOneWorkFlowArgoWorkflow = None,
+    ):
+        # The Argo workflow metadata.
+        self.argo_workflow = argo_workflow
+
+    def validate(self):
+        if self.argo_workflow:
+            self.argo_workflow.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.argo_workflow is not None:
+            result['ArgoWorkflow'] = self.argo_workflow.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ArgoWorkflow') is not None:
+            temp_model = DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaDataACKOneWorkFlowArgoWorkflow()
+            self.argo_workflow = temp_model.from_map(m['ArgoWorkflow'])
+        return self
+
+
+class DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaDataACKOne(TeaModel):
+    def __init__(
+        self,
+        git_ops: DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaDataACKOneGitOps = None,
+        work_flow: DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaDataACKOneWorkFlow = None,
+    ):
+        # The GitOps metadata.
+        self.git_ops = git_ops
+        # The workflow metadata.
+        self.work_flow = work_flow
+
+    def validate(self):
+        if self.git_ops:
+            self.git_ops.validate()
+        if self.work_flow:
+            self.work_flow.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.git_ops is not None:
+            result['GitOps'] = self.git_ops.to_map()
+        if self.work_flow is not None:
+            result['WorkFlow'] = self.work_flow.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('GitOps') is not None:
+            temp_model = DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaDataACKOneGitOps()
+            self.git_ops = temp_model.from_map(m['GitOps'])
+        if m.get('WorkFlow') is not None:
+            temp_model = DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaDataACKOneWorkFlow()
+            self.work_flow = temp_model.from_map(m['WorkFlow'])
+        return self
+
+
+class DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaData(TeaModel):
+    def __init__(
+        self,
+        ackone: DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaDataACKOne = None,
+    ):
+        # The cluster metadata.
+        self.ackone = ackone
+
+    def validate(self):
+        if self.ackone:
+            self.ackone.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.ackone is not None:
+            result['ACKOne'] = self.ackone.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ACKOne') is not None:
+            temp_model = DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaDataACKOne()
+            self.ackone = temp_model.from_map(m['ACKOne'])
+        return self
+
+
 class DescribeHubClusterDetailsResponseBodyClusterClusterInfo(TeaModel):
     def __init__(
         self,
         cluster_id: str = None,
         cluster_spec: str = None,
         creation_time: str = None,
         error_message: str = None,
+        meta_data: DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaData = None,
         name: str = None,
         profile: str = None,
         region_id: str = None,
+        resource_group_id: str = None,
         state: str = None,
         update_time: str = None,
         version: str = None,
     ):
         # The ID of the master instance.
         self.cluster_id = cluster_id
         # The specification of the master instance. Valid value:
         # 
         # *   ack.pro.small: ACK Pro cluster
         self.cluster_spec = cluster_spec
         # The time when the master instance was created.
         self.creation_time = creation_time
         # The error message returned when the master instance failed to be created.
         self.error_message = error_message
+        # The cluster metadata.
+        self.meta_data = meta_data
         # The name of the master instance.
         self.name = name
         # The configurations of the master instance.
         self.profile = profile
         # The ID of the region in which the master instance resides.
         self.region_id = region_id
+        # The ID of Resource Group.
+        self.resource_group_id = resource_group_id
         # The status of the master instance. Valid values:
         # 
         # *   initial: The master instance is being initialized.
         # *   failed: The master instance failed to be created.
         # *   running: The master instance is running
         # *   inactive: The master instance is pending.
         # *   deleting: The master instance is being deleted.
@@ -1078,15 +1298,16 @@
         self.state = state
         # The time when the master instance was updated.
         self.update_time = update_time
         # The version of the master instance.
         self.version = version
 
     def validate(self):
-        pass
+        if self.meta_data:
+            self.meta_data.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -1094,20 +1315,24 @@
             result['ClusterId'] = self.cluster_id
         if self.cluster_spec is not None:
             result['ClusterSpec'] = self.cluster_spec
         if self.creation_time is not None:
             result['CreationTime'] = self.creation_time
         if self.error_message is not None:
             result['ErrorMessage'] = self.error_message
+        if self.meta_data is not None:
+            result['MetaData'] = self.meta_data.to_map()
         if self.name is not None:
             result['Name'] = self.name
         if self.profile is not None:
             result['Profile'] = self.profile
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.resource_group_id is not None:
+            result['ResourceGroupID'] = self.resource_group_id
         if self.state is not None:
             result['State'] = self.state
         if self.update_time is not None:
             result['UpdateTime'] = self.update_time
         if self.version is not None:
             result['Version'] = self.version
         return result
@@ -1118,20 +1343,25 @@
             self.cluster_id = m.get('ClusterId')
         if m.get('ClusterSpec') is not None:
             self.cluster_spec = m.get('ClusterSpec')
         if m.get('CreationTime') is not None:
             self.creation_time = m.get('CreationTime')
         if m.get('ErrorMessage') is not None:
             self.error_message = m.get('ErrorMessage')
+        if m.get('MetaData') is not None:
+            temp_model = DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaData()
+            self.meta_data = temp_model.from_map(m['MetaData'])
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('Profile') is not None:
             self.profile = m.get('Profile')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('ResourceGroupID') is not None:
+            self.resource_group_id = m.get('ResourceGroupID')
         if m.get('State') is not None:
             self.state = m.get('State')
         if m.get('UpdateTime') is not None:
             self.update_time = m.get('UpdateTime')
         if m.get('Version') is not None:
             self.version = m.get('Version')
         return self
@@ -1370,15 +1600,19 @@
 
 class DescribeHubClusterDetailsResponseBodyClusterWorkflowConfigWorkflowUnitsVSwitches(TeaModel):
     def __init__(
         self,
         vswitch_id: str = None,
         zone_id: str = None,
     ):
+        # The ID of the vSwitch.
         self.vswitch_id = vswitch_id
+        # The zone ID of the cluster.
+        # 
+        # > You can call the [DescribeRegions](~~143074~~) operation to query the most recent zone list.
         self.zone_id = zone_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1404,16 +1638,21 @@
 class DescribeHubClusterDetailsResponseBodyClusterWorkflowConfigWorkflowUnits(TeaModel):
     def __init__(
         self,
         region_id: str = None,
         v_switches: List[DescribeHubClusterDetailsResponseBodyClusterWorkflowConfigWorkflowUnitsVSwitches] = None,
         vpc_id: str = None,
     ):
+        # The region ID of the cluster.
+        # 
+        # >  You can call the [DescribeRegions](~~143074~~) operation to query the most recent region list.
         self.region_id = region_id
+        # The vSwitches.
         self.v_switches = v_switches
+        # The ID of the VPC.
         self.vpc_id = vpc_id
 
     def validate(self):
         if self.v_switches:
             for k in self.v_switches:
                 if k:
                     k.validate()
@@ -1452,17 +1691,27 @@
     def __init__(
         self,
         argo_server_enabled: bool = None,
         price_limit: str = None,
         workflow_schedule_mode: str = None,
         workflow_units: List[DescribeHubClusterDetailsResponseBodyClusterWorkflowConfigWorkflowUnits] = None,
     ):
+        # Specifies whether to enable the workflow instance UI. This parameter takes effect only if Profile is set to XFlow. Valid values:
+        # 
+        # *   true
+        # *   false
         self.argo_server_enabled = argo_server_enabled
+        # The limit on the prices of containers in the workflow. This parameter takes effect only if the WorkflowScheduleMode parameter is set to cost-optimized.
         self.price_limit = price_limit
+        # The scheduling mode of the workflow. This parameter takes effect only if Profile is set to XFlow. Valid values:
+        # 
+        # *   cost-optimized: cost-prioritized scheduling mode.
+        # *   stock-optimized: inventory-prioritized scheduling mode.
         self.workflow_schedule_mode = workflow_schedule_mode
+        # The Argo workflow regions  configuration.
         self.workflow_units = workflow_units
 
     def validate(self):
         if self.workflow_units:
             for k in self.workflow_units:
                 if k:
                     k.validate()
@@ -1523,14 +1772,15 @@
         self.endpoints = endpoints
         # The logging configuration.
         self.log_config = log_config
         # The configurations of Alibaba Cloud Service Mesh (ASM).
         self.mesh_config = mesh_config
         # The network configurations of the master instance.
         self.network = network
+        # The Argo workflow configuration.
         self.workflow_config = workflow_config
 
     def validate(self):
         if self.api_server:
             self.api_server.validate()
         if self.cluster_info:
             self.cluster_info.validate()
@@ -1651,17 +1901,14 @@
         body: DescribeHubClusterDetailsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1770,17 +2017,14 @@
         body: DescribeHubClusterKubeconfigResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1934,17 +2178,14 @@
         body: DescribeHubClusterLogsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -1970,46 +2211,60 @@
         return self
 
 
 class DescribeHubClustersRequest(TeaModel):
     def __init__(
         self,
         profile: str = None,
+        resource_group_id: str = None,
     ):
+        # The configurations of the cluster.
         self.profile = profile
+        # The resource group ID.
+        self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.profile is not None:
             result['Profile'] = self.profile
+        if self.resource_group_id is not None:
+            result['ResourceGroupId'] = self.resource_group_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Profile') is not None:
             self.profile = m.get('Profile')
+        if m.get('ResourceGroupId') is not None:
+            self.resource_group_id = m.get('ResourceGroupId')
         return self
 
 
 class DescribeHubClustersResponseBodyClustersApiServer(TeaModel):
     def __init__(
         self,
         api_server_eip_id: str = None,
         enabled_public: bool = None,
         load_balancer_id: str = None,
     ):
+        # The elastic IP address (EIP) ID.
         self.api_server_eip_id = api_server_eip_id
+        # Indicates whether public endpoint is enabled for the API server. Valid values:
+        # 
+        # *   true
+        # *   false
         self.enabled_public = enabled_public
+        # The ID of the Server Load Balancer (SLB) instance that is associated with the cluster.
         self.load_balancer_id = load_balancer_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2042,27 +2297,50 @@
         cluster_id: str = None,
         cluster_spec: str = None,
         creation_time: str = None,
         error_message: str = None,
         name: str = None,
         profile: str = None,
         region_id: str = None,
+        resource_group_id: str = None,
         state: str = None,
         update_time: str = None,
         version: str = None,
     ):
+        # The cluster ID.
         self.cluster_id = cluster_id
+        # The specification of the cluster.
+        # 
+        # *   Only ack.pro.small is returned.
         self.cluster_spec = cluster_spec
+        # The time when the cluster was created.
         self.creation_time = creation_time
+        # The error message that is returned if the cluster failed to be created.
         self.error_message = error_message
+        # The name of the cluster.
         self.name = name
+        # The configurations of the cluster.
         self.profile = profile
+        # The region ID.
         self.region_id = region_id
+        # The ID of Resource Group.
+        self.resource_group_id = resource_group_id
+        # The status of the cluster. Valid values:
+        # 
+        # *   initial: The cluster is being initialized.
+        # *   failed: The cluster failed to be created.
+        # *   running: The cluster is running
+        # *   inactive: The cluster is pending.
+        # *   deleting: The cluster is being deleted.
+        # *   delete_failed: The cluster failed to be deleted.
+        # *   deleted: The cluster is deleted.
         self.state = state
+        # The time when the cluster was last updated.
         self.update_time = update_time
+        # The Kubernetes version of the cluster.
         self.version = version
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2080,14 +2358,16 @@
             result['ErrorMessage'] = self.error_message
         if self.name is not None:
             result['Name'] = self.name
         if self.profile is not None:
             result['Profile'] = self.profile
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.resource_group_id is not None:
+            result['ResourceGroupID'] = self.resource_group_id
         if self.state is not None:
             result['State'] = self.state
         if self.update_time is not None:
             result['UpdateTime'] = self.update_time
         if self.version is not None:
             result['Version'] = self.version
         return result
@@ -2104,14 +2384,16 @@
             self.error_message = m.get('ErrorMessage')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('Profile') is not None:
             self.profile = m.get('Profile')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('ResourceGroupID') is not None:
+            self.resource_group_id = m.get('ResourceGroupID')
         if m.get('State') is not None:
             self.state = m.get('State')
         if m.get('UpdateTime') is not None:
             self.update_time = m.get('UpdateTime')
         if m.get('Version') is not None:
             self.version = m.get('Version')
         return self
@@ -2121,17 +2403,25 @@
     def __init__(
         self,
         message: str = None,
         reason: str = None,
         status: str = None,
         type: str = None,
     ):
+        # The error message that is returned.
         self.message = message
+        # The reason for the deletion condition.
         self.reason = reason
+        # The status of the cluster that the deletion condition indicates. Valid values:
+        # 
+        # *   True: The cluster cannot be deleted.
+        # *   False: The cluster can be deleted.
+        # *   Unknow: Whether the cluster can be deleted is unknown.
         self.status = status
+        # The type of deletion condition.
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2164,15 +2454,17 @@
 
 class DescribeHubClustersResponseBodyClustersEndpoints(TeaModel):
     def __init__(
         self,
         intranet_api_server_endpoint: str = None,
         public_api_server_endpoint: str = None,
     ):
+        # The internal endpoint of the API server.
         self.intranet_api_server_endpoint = intranet_api_server_endpoint
+        # The public endpoint of the API server.
         self.public_api_server_endpoint = public_api_server_endpoint
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2198,16 +2490,22 @@
 class DescribeHubClustersResponseBodyClustersLogConfig(TeaModel):
     def __init__(
         self,
         enable_log: bool = None,
         log_project: str = None,
         log_store_ttl: str = None,
     ):
+        # Indicates whether the audit logging feature is enabled. Valid values:
+        # 
+        # *   true
+        # *   false
         self.enable_log = enable_log
+        # The name of the project in Simple Log Service.
         self.log_project = log_project
+        # The number of days that logs are retained by Simple Log Service.
         self.log_store_ttl = log_store_ttl
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2236,15 +2534,20 @@
 
 class DescribeHubClustersResponseBodyClustersMeshConfig(TeaModel):
     def __init__(
         self,
         enable_mesh: bool = None,
         mesh_id: str = None,
     ):
+        # Indicates whether ASM is enabled. Valid values:
+        # 
+        # *   true
+        # *   false
         self.enable_mesh = enable_mesh
+        # The ASM instance ID.
         self.mesh_id = mesh_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2271,17 +2574,21 @@
     def __init__(
         self,
         cluster_domain: str = None,
         security_group_ids: List[str] = None,
         v_switches: List[str] = None,
         vpc_id: str = None,
     ):
+        # The domain name of the cluster.
         self.cluster_domain = cluster_domain
+        # The security group IDs.
         self.security_group_ids = security_group_ids
+        # The IDs of vSwitches to which the cluster belongs.
         self.v_switches = v_switches
+        # The ID of the virtual private cloud (VPC) to which the cluster belongs.
         self.vpc_id = vpc_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2319,20 +2626,27 @@
         cluster_info: DescribeHubClustersResponseBodyClustersClusterInfo = None,
         conditions: List[DescribeHubClustersResponseBodyClustersConditions] = None,
         endpoints: DescribeHubClustersResponseBodyClustersEndpoints = None,
         log_config: DescribeHubClustersResponseBodyClustersLogConfig = None,
         mesh_config: DescribeHubClustersResponseBodyClustersMeshConfig = None,
         network: DescribeHubClustersResponseBodyClustersNetwork = None,
     ):
+        # The information about the API server.
         self.api_server = api_server
+        # The details of the cluster.
         self.cluster_info = cluster_info
+        # The deletion conditions of the cluster.
         self.conditions = conditions
+        # The endpoint of the cluster.
         self.endpoints = endpoints
+        # The logging configurations.
         self.log_config = log_config
+        # The configurations of Alibaba Cloud Service Mesh (ASM).
         self.mesh_config = mesh_config
+        # The network configurations of the cluster.
         self.network = network
 
     def validate(self):
         if self.api_server:
             self.api_server.validate()
         if self.cluster_info:
             self.cluster_info.validate()
@@ -2403,15 +2717,17 @@
 
 class DescribeHubClustersResponseBody(TeaModel):
     def __init__(
         self,
         clusters: List[DescribeHubClustersResponseBodyClusters] = None,
         request_id: str = None,
     ):
+        # The information about clusters.
         self.clusters = clusters
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         if self.clusters:
             for k in self.clusters:
                 if k:
                     k.validate()
@@ -2450,17 +2766,14 @@
         body: DescribeHubClustersResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2796,17 +3109,14 @@
         body: DescribeManagedClustersResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2918,17 +3228,14 @@
         body: DescribePoliciesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -2955,15 +3262,15 @@
 
 
 class DescribePolicyDetailsRequest(TeaModel):
     def __init__(
         self,
         policy_name: str = None,
     ):
-        # The name of the policy.
+        # The policy name.
         self.policy_name = policy_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3007,15 +3314,15 @@
         # The description of the policy.
         self.description = description
         # The name of the policy.
         self.name = name
         # Indicates whether parameters are required. Valid values:
         # 
         # *   0: Parameters are required.
-        # *   1: Parameters are optional.
+        # *   1: Parameters are not required.
         self.no_config = no_config
         # The severity level of the policy.
         self.severity = severity
         # The content of the policy.
         self.template = template
         # The time when the policy was last updated.
         self.updated = updated
@@ -3074,15 +3381,15 @@
 
 class DescribePolicyDetailsResponseBody(TeaModel):
     def __init__(
         self,
         policy: DescribePolicyDetailsResponseBodyPolicy = None,
         request_id: str = None,
     ):
-        # Detailed information about the policy.
+        # The policies.
         self.policy = policy
         # The request ID.
         self.request_id = request_id
 
     def validate(self):
         if self.policy:
             self.policy.validate()
@@ -3117,17 +3424,14 @@
         body: DescribePolicyDetailsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -3811,17 +4115,14 @@
         body: DescribePolicyGovernanceInClusterResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4031,17 +4332,14 @@
         body: DescribePolicyInstancesResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4333,17 +4631,14 @@
         body: DescribePolicyInstancesStatusResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4483,17 +4778,14 @@
         body: DescribeRegionsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4657,17 +4949,14 @@
         body: DescribeUserPermissionsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4790,17 +5079,14 @@
         body: DetachClusterFromHubResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4832,49 +5118,29 @@
         cluster_id: str = None,
         is_ram_role: bool = None,
         namespace: str = None,
         role_name: str = None,
         role_type: str = None,
         user_id: str = None,
     ):
+        # The ID of the cluster.
         self.cluster_id = cluster_id
         # The entity to which the permissions are granted. A value of `true` indicates that the permissions are granted to a RAM user. A value of `false` indicates that the permissions are granted to a RAM role.
         self.is_ram_role = is_ram_role
+        # The namespace to which the permissions are scoped. By default, this parameter is empty when you set RoleType to cluster.
         self.namespace = namespace
         # The predefined role that you want to assign. Valid values:
         # 
         # *   admin: the administrator role.
         # *   dev: the developer role.
-        # 
-        # Enumerated values:
-        # 
-        # *   arms-admin
-        # 
-        #     <!-- -->
-        # 
-        #     <!-- -->
-        # 
-        #     <!-- -->
-        # 
-        # *   dev
-        # 
-        #     <!-- -->
-        # 
-        #     <!-- -->
-        # 
-        #     <!-- -->
-        # 
-        # *   admin
-        # 
-        #     <!-- -->
-        # 
-        #     <!-- -->
-        # 
-        #     <!-- -->
         self.role_name = role_name
+        # The authorization type. Valid values:
+        # 
+        # *   cluster: specifies that the permissions are scoped to a master instance.
+        # *   namespace: specifies that the permissions are scoped to a namespace of a cluster.
         self.role_type = role_type
         # The ID of the RAM user or RAM role.
         self.user_id = user_id
 
     def validate(self):
         pass
 
@@ -4916,14 +5182,15 @@
 
 
 class GrantUserPermissionResponseBody(TeaModel):
     def __init__(
         self,
         request_id: str = None,
     ):
+        # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4950,17 +5217,14 @@
         body: GrantUserPermissionResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -4995,14 +5259,15 @@
         role_name: str = None,
         role_type: str = None,
     ):
         # The master instance ID.
         # 
         # *   When the role_type parameter is set to all-clusters, set the parameter to an empty string.
         self.cluster_id = cluster_id
+        # The entity to which the permissions are granted. A value of `true` indicates that the permissions are granted to a RAM user. A value of `false` indicates that the permissions are granted to a RAM role.
         self.is_ram_role = is_ram_role
         # The namespace to which the permissions are scoped. By default, this parameter is empty when you set RoleType to cluster.
         self.namespace = namespace
         # The predefined role that you want to assign. Valid values:
         # 
         # *   admin: the administrator role.
         # *   dev: the developer role.
@@ -5164,17 +5429,14 @@
         body: GrantUserPermissionsResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -5209,15 +5471,15 @@
         argo_cdhaenabled: bool = None,
         argo_events_enabled: bool = None,
         argo_server_enabled: bool = None,
         audit_log_enabled: bool = None,
         cluster_id: str = None,
         deletion_protection: bool = None,
         enable_mesh: bool = None,
-        mseenabled: bool = None,
+        gateway_enabled: bool = None,
         monitor_enabled: bool = None,
         name: str = None,
         price_limit: str = None,
         public_access_enabled: bool = None,
         public_api_server_enabled: bool = None,
         v_switches: List[str] = None,
         workflow_schedule_mode: str = None,
@@ -5261,15 +5523,18 @@
         # Default value: false.
         self.deletion_protection = deletion_protection
         # Specifies whether to enable Service Mesh (ASM). Valid values:
         # 
         # *   true
         # *   false
         self.enable_mesh = enable_mesh
-        self.mseenabled = mseenabled
+        # Specifies whether to enable Gateway. Valid values:
+        # - true
+        # - false
+        self.gateway_enabled = gateway_enabled
         # Specifies whether to enable the monitoring dashboard feature for the workflow instance. This parameter takes effect only if Profile is set to XFlow. Valid values:
         # 
         # *   true
         # *   false
         self.monitor_enabled = monitor_enabled
         # The name of the master instance. The name must be 1 to 63 characters in length. It must start with a letter, and can contain letters, digits, underscores (\_), and hyphens (-).
         self.name = name
@@ -5318,16 +5583,16 @@
             result['AuditLogEnabled'] = self.audit_log_enabled
         if self.cluster_id is not None:
             result['ClusterId'] = self.cluster_id
         if self.deletion_protection is not None:
             result['DeletionProtection'] = self.deletion_protection
         if self.enable_mesh is not None:
             result['EnableMesh'] = self.enable_mesh
-        if self.mseenabled is not None:
-            result['MSEEnabled'] = self.mseenabled
+        if self.gateway_enabled is not None:
+            result['GatewayEnabled'] = self.gateway_enabled
         if self.monitor_enabled is not None:
             result['MonitorEnabled'] = self.monitor_enabled
         if self.name is not None:
             result['Name'] = self.name
         if self.price_limit is not None:
             result['PriceLimit'] = self.price_limit
         if self.public_access_enabled is not None:
@@ -5358,16 +5623,16 @@
             self.audit_log_enabled = m.get('AuditLogEnabled')
         if m.get('ClusterId') is not None:
             self.cluster_id = m.get('ClusterId')
         if m.get('DeletionProtection') is not None:
             self.deletion_protection = m.get('DeletionProtection')
         if m.get('EnableMesh') is not None:
             self.enable_mesh = m.get('EnableMesh')
-        if m.get('MSEEnabled') is not None:
-            self.mseenabled = m.get('MSEEnabled')
+        if m.get('GatewayEnabled') is not None:
+            self.gateway_enabled = m.get('GatewayEnabled')
         if m.get('MonitorEnabled') is not None:
             self.monitor_enabled = m.get('MonitorEnabled')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('PriceLimit') is not None:
             self.price_limit = m.get('PriceLimit')
         if m.get('PublicAccessEnabled') is not None:
@@ -5390,15 +5655,15 @@
         argo_cdhaenabled: bool = None,
         argo_events_enabled: bool = None,
         argo_server_enabled: bool = None,
         audit_log_enabled: bool = None,
         cluster_id: str = None,
         deletion_protection: bool = None,
         enable_mesh: bool = None,
-        mseenabled: bool = None,
+        gateway_enabled: bool = None,
         monitor_enabled: bool = None,
         name: str = None,
         price_limit: str = None,
         public_access_enabled: bool = None,
         public_api_server_enabled: bool = None,
         v_switches_shrink: str = None,
         workflow_schedule_mode: str = None,
@@ -5442,15 +5707,18 @@
         # Default value: false.
         self.deletion_protection = deletion_protection
         # Specifies whether to enable Service Mesh (ASM). Valid values:
         # 
         # *   true
         # *   false
         self.enable_mesh = enable_mesh
-        self.mseenabled = mseenabled
+        # Specifies whether to enable Gateway. Valid values:
+        # - true
+        # - false
+        self.gateway_enabled = gateway_enabled
         # Specifies whether to enable the monitoring dashboard feature for the workflow instance. This parameter takes effect only if Profile is set to XFlow. Valid values:
         # 
         # *   true
         # *   false
         self.monitor_enabled = monitor_enabled
         # The name of the master instance. The name must be 1 to 63 characters in length. It must start with a letter, and can contain letters, digits, underscores (\_), and hyphens (-).
         self.name = name
@@ -5499,16 +5767,16 @@
             result['AuditLogEnabled'] = self.audit_log_enabled
         if self.cluster_id is not None:
             result['ClusterId'] = self.cluster_id
         if self.deletion_protection is not None:
             result['DeletionProtection'] = self.deletion_protection
         if self.enable_mesh is not None:
             result['EnableMesh'] = self.enable_mesh
-        if self.mseenabled is not None:
-            result['MSEEnabled'] = self.mseenabled
+        if self.gateway_enabled is not None:
+            result['GatewayEnabled'] = self.gateway_enabled
         if self.monitor_enabled is not None:
             result['MonitorEnabled'] = self.monitor_enabled
         if self.name is not None:
             result['Name'] = self.name
         if self.price_limit is not None:
             result['PriceLimit'] = self.price_limit
         if self.public_access_enabled is not None:
@@ -5539,16 +5807,16 @@
             self.audit_log_enabled = m.get('AuditLogEnabled')
         if m.get('ClusterId') is not None:
             self.cluster_id = m.get('ClusterId')
         if m.get('DeletionProtection') is not None:
             self.deletion_protection = m.get('DeletionProtection')
         if m.get('EnableMesh') is not None:
             self.enable_mesh = m.get('EnableMesh')
-        if m.get('MSEEnabled') is not None:
-            self.mseenabled = m.get('MSEEnabled')
+        if m.get('GatewayEnabled') is not None:
+            self.gateway_enabled = m.get('GatewayEnabled')
         if m.get('MonitorEnabled') is not None:
             self.monitor_enabled = m.get('MonitorEnabled')
         if m.get('Name') is not None:
             self.name = m.get('Name')
         if m.get('PriceLimit') is not None:
             self.price_limit = m.get('PriceLimit')
         if m.get('PublicAccessEnabled') is not None:
@@ -5598,17 +5866,14 @@
         body: UpdateHubClusterFeatureResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
@@ -5732,17 +5997,14 @@
         body: UpdateUserPermissionResponseBody = None,
     ):
         self.headers = headers
         self.status_code = status_code
         self.body = body
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
```

### Comparing `alibabacloud_adcp20220101-2.0.2/alibabacloud_adcp20220101.egg-info/PKG-INFO` & `alibabacloud_adcp20220101-3.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-adcp20220101
-Version: 2.0.2
+Name: alibabacloud_adcp20220101
+Version: 3.0.0
 Summary: Alibaba Cloud adcp (20220101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
@@ -32,15 +32,15 @@
         
         ## Usage
         
         [Quick Examples](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/docs/0-Usage-EN.md#quick-examples)
         
         ## Changelog
         
-        Detailed changes for each release are documented in the [release notes](./ChangeLog.md).
+        Detailed changes for each release are documented in the [release notes](https://github.com/aliyun/alibabacloud-python-sdk/blob/master/adcp-20220101/ChangeLog.md).
         
         ## References
         
         - [Latest Release](https://github.com/aliyun/alibabacloud-sdk/tree/master/python)
         
         ## License
```

### Comparing `alibabacloud_adcp20220101-2.0.2/setup.py` & `alibabacloud_adcp20220101-3.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_adcp20220101.
 
-Created on 12/10/2023
+Created on 22/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_adcp20220101"
 NAME = "alibabacloud_adcp20220101" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud adcp (20220101) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.11, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```


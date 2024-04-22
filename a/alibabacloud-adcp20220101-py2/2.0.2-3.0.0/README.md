# Comparing `tmp/alibabacloud_adcp20220101_py2-2.0.2.tar.gz` & `tmp/alibabacloud_adcp20220101_py2-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_adcp20220101_py2-2.0.2.tar", last modified: Thu Oct 12 17:17:29 2023, max compression
+gzip compressed data, was "dist/alibabacloud_adcp20220101_py2-3.0.0.tar", last modified: Mon Apr 22 02:56:58 2024, max compression
```

## Comparing `alibabacloud_adcp20220101_py2-2.0.2.tar` & `alibabacloud_adcp20220101_py2-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-12 17:17:29.000000 alibabacloud_adcp20220101_py2-2.0.2/
--rw-r--r--   0 root         (0) root         (0)     1075 2023-10-12 17:17:29.000000 alibabacloud_adcp20220101_py2-2.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-10-12 17:17:29.000000 alibabacloud_adcp20220101_py2-2.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-10-12 17:17:29.000000 alibabacloud_adcp20220101_py2-2.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2478 2023-10-12 17:17:29.000000 alibabacloud_adcp20220101_py2-2.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1036 2023-10-12 17:17:29.000000 alibabacloud_adcp20220101_py2-2.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2023-10-12 17:17:29.000000 alibabacloud_adcp20220101_py2-2.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-12 17:17:29.000000 alibabacloud_adcp20220101_py2-2.0.2/alibabacloud_adcp20220101/
--rw-r--r--   0 root         (0) root         (0)       21 2023-10-12 17:17:29.000000 alibabacloud_adcp20220101_py2-2.0.2/alibabacloud_adcp20220101/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34139 2023-10-12 17:17:29.000000 alibabacloud_adcp20220101_py2-2.0.2/alibabacloud_adcp20220101/client.py
--rw-r--r--   0 root         (0) root         (0)   200184 2023-10-12 17:17:29.000000 alibabacloud_adcp20220101_py2-2.0.2/alibabacloud_adcp20220101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-12 17:17:29.000000 alibabacloud_adcp20220101_py2-2.0.2/alibabacloud_adcp20220101_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2478 2023-10-12 17:17:29.000000 alibabacloud_adcp20220101_py2-2.0.2/alibabacloud_adcp20220101_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      448 2023-10-12 17:17:29.000000 alibabacloud_adcp20220101_py2-2.0.2/alibabacloud_adcp20220101_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-12 17:17:29.000000 alibabacloud_adcp20220101_py2-2.0.2/alibabacloud_adcp20220101_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-10-12 17:17:29.000000 alibabacloud_adcp20220101_py2-2.0.2/alibabacloud_adcp20220101_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-10-12 17:17:29.000000 alibabacloud_adcp20220101_py2-2.0.2/alibabacloud_adcp20220101_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-10-12 17:17:29.000000 alibabacloud_adcp20220101_py2-2.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2908 2023-10-12 17:17:29.000000 alibabacloud_adcp20220101_py2-2.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 02:56:58.000000 alibabacloud_adcp20220101_py2-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1211 2024-04-22 02:56:57.000000 alibabacloud_adcp20220101_py2-3.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-22 02:56:57.000000 alibabacloud_adcp20220101_py2-3.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-22 02:56:57.000000 alibabacloud_adcp20220101_py2-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2478 2024-04-22 02:56:58.000000 alibabacloud_adcp20220101_py2-3.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1036 2024-04-22 02:56:57.000000 alibabacloud_adcp20220101_py2-3.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2024-04-22 02:56:57.000000 alibabacloud_adcp20220101_py2-3.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 02:56:58.000000 alibabacloud_adcp20220101_py2-3.0.0/alibabacloud_adcp20220101/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-22 02:56:57.000000 alibabacloud_adcp20220101_py2-3.0.0/alibabacloud_adcp20220101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34976 2024-04-22 02:56:57.000000 alibabacloud_adcp20220101_py2-3.0.0/alibabacloud_adcp20220101/client.py
+-rw-r--r--   0 root         (0) root         (0)   211159 2024-04-22 02:56:57.000000 alibabacloud_adcp20220101_py2-3.0.0/alibabacloud_adcp20220101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 02:56:58.000000 alibabacloud_adcp20220101_py2-3.0.0/alibabacloud_adcp20220101_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2478 2024-04-22 02:56:57.000000 alibabacloud_adcp20220101_py2-3.0.0/alibabacloud_adcp20220101_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      448 2024-04-22 02:56:57.000000 alibabacloud_adcp20220101_py2-3.0.0/alibabacloud_adcp20220101_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 02:56:57.000000 alibabacloud_adcp20220101_py2-3.0.0/alibabacloud_adcp20220101_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-22 02:56:57.000000 alibabacloud_adcp20220101_py2-3.0.0/alibabacloud_adcp20220101_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-22 02:56:57.000000 alibabacloud_adcp20220101_py2-3.0.0/alibabacloud_adcp20220101_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-22 02:56:58.000000 alibabacloud_adcp20220101_py2-3.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2908 2024-04-22 02:56:57.000000 alibabacloud_adcp20220101_py2-3.0.0/setup.py
```

### Comparing `alibabacloud_adcp20220101_py2-2.0.2/ChangeLog.md` & `alibabacloud_adcp20220101_py2-3.0.0/ChangeLog.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+2023-10-12 Version: 2.0.2
+- Generated python2 2022-01-01 for adcp.
+
+2023-10-12 Version: 2.0.2
+- Generated python2 2022-01-01 for adcp.
+
 2023-09-13 Version: 2.0.1
 - Generated python2 2022-01-01 for adcp.
 
 2023-08-10 Version: 2.0.0
 - UpdateHubClusterFeature support ArgoCDHAEnabled.
```

### Comparing `alibabacloud_adcp20220101_py2-2.0.2/LICENSE` & `alibabacloud_adcp20220101_py2-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_adcp20220101_py2-2.0.2/PKG-INFO` & `alibabacloud_adcp20220101_py2-3.0.0/alibabacloud_adcp20220101_py2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_adcp20220101_py2
-Version: 2.0.2
+Name: alibabacloud-adcp20220101-py2
+Version: 3.0.0
 Summary: Alibaba Cloud adcp (20220101) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_adcp20220101_py2-2.0.2/README-CN.md` & `alibabacloud_adcp20220101_py2-3.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_adcp20220101_py2-2.0.2/README.md` & `alibabacloud_adcp20220101_py2-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_adcp20220101_py2-2.0.2/alibabacloud_adcp20220101/client.py` & `alibabacloud_adcp20220101_py2-3.0.0/alibabacloud_adcp20220101/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
 class Client(OpenApiClient):
     """
     *\
     """
     def __init__(self, config):
         super(Client, self).__init__(config)
-        self._signature_algorithm = 'v2'
         self._endpoint_rule = 'central'
         self._endpoint_map = {
             'cn-beijing': 'adcp.cn-beijing.aliyuncs.com',
             'cn-zhangjiakou': 'adcp.cn-zhangjiakou.aliyuncs.com',
             'cn-hangzhou': 'adcp.cn-hangzhou.aliyuncs.com',
             'cn-shanghai': 'adcp.cn-shanghai.aliyuncs.com',
             'cn-shenzhen': 'adcp.cn-shenzhen.aliyuncs.com',
@@ -105,14 +104,16 @@
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
@@ -369,14 +370,16 @@
         return self.describe_hub_cluster_logs_with_options(request, runtime)
 
     def describe_hub_clusters_with_options(self, request, runtime):
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
@@ -683,14 +686,25 @@
         )
 
     def grant_user_permission(self, request):
         runtime = util_models.RuntimeOptions()
         return self.grant_user_permission_with_options(request, runtime)
 
     def grant_user_permissions_with_options(self, tmp_req, runtime):
+        """
+        @deprecated : GrantUserPermissions is deprecated, please use adcp::2022-01-01::GrantUserPermission instead.
+        
+
+        @param tmp_req: GrantUserPermissionsRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
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
@@ -713,14 +727,23 @@
         )
         return TeaCore.from_map(
             adcp_20220101_models.GrantUserPermissionsResponse(),
             self.call_api(params, req, runtime)
         )
 
     def grant_user_permissions(self, request):
+        """
+        @deprecated : GrantUserPermissions is deprecated, please use adcp::2022-01-01::GrantUserPermission instead.
+        
+
+        @param request: GrantUserPermissionsRequest
+
+        @return: GrantUserPermissionsResponse
+        Deprecated
+        """
         runtime = util_models.RuntimeOptions()
         return self.grant_user_permissions_with_options(request, runtime)
 
     def update_hub_cluster_feature_with_options(self, tmp_req, runtime):
         UtilClient.validate_model(tmp_req)
         request = adcp_20220101_models.UpdateHubClusterFeatureShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
@@ -745,16 +768,16 @@
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

### Comparing `alibabacloud_adcp20220101_py2-2.0.2/alibabacloud_adcp20220101/models.py` & `alibabacloud_adcp20220101_py2-3.0.0/alibabacloud_adcp20220101/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,17 +85,14 @@
 class AttachClusterToHubResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: AttachClusterToHubResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(AttachClusterToHubResponse, self).to_map()
         if _map is not None:
             return _map
@@ -119,45 +116,56 @@
             temp_model = AttachClusterToHubResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class CreateHubClusterRequest(TeaModel):
     def __init__(self, api_server_public_eip=None, argo_server_enabled=None, audit_log_enabled=None,
-                 is_enterprise_security_group=None, name=None, price_limit=None, profile=None, region_id=None, v_switches=None, vpc_id=None,
-                 workflow_schedule_mode=None):
+                 is_enterprise_security_group=None, name=None, price_limit=None, profile=None, region_id=None, resource_group_id=None,
+                 v_switches=None, vpc_id=None, workflow_schedule_mode=None):
         # Specifies whether to expose the API server to the Internet. Valid values:
         # 
         # *   true: exposes the API server to the Internet.
         # *   false: exposes the API server to the internal network.
         self.api_server_public_eip = api_server_public_eip  # type: bool
+        # Specifies whether to enable the workflow instance UI. This parameter takes effect only if Profile is set to XFlow. Valid values:
+        # 
+        # *   true
+        # *   false
         self.argo_server_enabled = argo_server_enabled  # type: bool
         # Specifies whether to enable the audit log feature. Valid values:
         # 
         # *   true: enables the audit log feature.
         # *   false: disables the audit log feature.
         self.audit_log_enabled = audit_log_enabled  # type: bool
         # Specifies whether to use an advanced security group.
         self.is_enterprise_security_group = is_enterprise_security_group  # type: bool
         # The name of the master instance.
         self.name = name  # type: str
+        # The limit on the prices of containers in the workflow. This parameter takes effect only if the WorkflowScheduleMode parameter is set to cost-optimized.
         self.price_limit = price_limit  # type: str
         # The type of scenario for which the master instance is suitable. Valid values:
         # 
         # *   `Default`: The master instance is suitable for standard scenarios.
         # *   `XFlow`: The master instance is suitable for workflow scenarios.
         # 
         # Default value: `Default`.
         self.profile = profile  # type: str
         # The ID of the region. You can call the DescribeRegions operation to query available regions.
         self.region_id = region_id  # type: str
+        # The Resource Group ID.
+        self.resource_group_id = resource_group_id  # type: str
         # The ID of the vSwitch.
         self.v_switches = v_switches  # type: str
         # The ID of the virtual private cloud (VPC) to which the master instance belongs. You can call the DescribeVpcs operation to query available VPCs.
         self.vpc_id = vpc_id  # type: str
+        # The scheduling mode of the workflow. This parameter takes effect only if Profile is set to XFlow. Valid values:
+        # 
+        # *   cost-optimized: cost-prioritized scheduling mode.
+        # *   stock-optimized: inventory-prioritized scheduling mode.
         self.workflow_schedule_mode = workflow_schedule_mode  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateHubClusterRequest, self).to_map()
@@ -177,14 +185,16 @@
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
@@ -203,14 +213,16 @@
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
@@ -256,17 +268,14 @@
 class CreateHubClusterResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: CreateHubClusterResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(CreateHubClusterResponse, self).to_map()
         if _map is not None:
             return _map
@@ -416,17 +425,14 @@
 class DeleteHubClusterResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DeleteHubClusterResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteHubClusterResponse, self).to_map()
         if _map is not None:
             return _map
@@ -554,17 +560,14 @@
 class DeletePolicyInstanceResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DeletePolicyInstanceResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeletePolicyInstanceResponse, self).to_map()
         if _map is not None:
             return _map
@@ -649,17 +652,14 @@
 class DeleteUserPermissionResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DeleteUserPermissionResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeleteUserPermissionResponse, self).to_map()
         if _map is not None:
             return _map
@@ -818,17 +818,14 @@
 class DeployPolicyInstanceResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DeployPolicyInstanceResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DeployPolicyInstanceResponse, self).to_map()
         if _map is not None:
             return _map
@@ -915,33 +912,232 @@
         if m.get('EnabledPublic') is not None:
             self.enabled_public = m.get('EnabledPublic')
         if m.get('LoadBalancerId') is not None:
             self.load_balancer_id = m.get('LoadBalancerId')
         return self
 
 
+class DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaDataACKOneGitOps(TeaModel):
+    def __init__(self, access_control_list=None, enabled=None, haenabled=None, public_access_enabled=None):
+        # The Internet access control list (ACL). This parameter takes effect only if PublicAccessEnabled is set to true.
+        self.access_control_list = access_control_list  # type: list[str]
+        # Indicates whether GitOps is enabled. Valid values:
+        # 
+        # *   true: GitOps is enabled.
+        # *   false: GitOps is disabled.
+        self.enabled = enabled  # type: bool
+        # Indicates whether GitOps High Availability is enabled. Valid values:
+        # 
+        # *   true:  GitOps High Availability is enabled.
+        # *   false:  GitOps High Availability is disabled.
+        self.haenabled = haenabled  # type: bool
+        # Specifies whether to enable public domain name resolution in the Argo CD or Argo Workflow console. Valid values:
+        # 
+        # *   true
+        # *   false
+        self.public_access_enabled = public_access_enabled  # type: bool
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaDataACKOneGitOps, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, access_control_list=None, enabled=None, public_access_enabled=None, server_enabled=None):
+        # The Internet access control list (ACL). This parameter takes effect only if PublicAccessEnabled is set to true.
+        self.access_control_list = access_control_list  # type: list[str]
+        # Specifies whether to enable the argo workflow. Valid values:
+        # 
+        # *   **false** (default)
+        # *   **true**\
+        self.enabled = enabled  # type: bool
+        # Specifies whether to enable public domain name resolution in the Argo CD or Argo Workflow console. Valid values:
+        # 
+        # *   true
+        # *   false
+        self.public_access_enabled = public_access_enabled  # type: bool
+        # Specifies whether to enable the argo workflow. UI Valid values:
+        # 
+        # *   **false** (default)
+        # *   **true**\
+        self.server_enabled = server_enabled  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaDataACKOneWorkFlowArgoWorkflow, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, argo_workflow=None):
+        # The Argo workflow metadata.
+        self.argo_workflow = argo_workflow  # type: DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaDataACKOneWorkFlowArgoWorkflow
+
+    def validate(self):
+        if self.argo_workflow:
+            self.argo_workflow.validate()
+
+    def to_map(self):
+        _map = super(DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaDataACKOneWorkFlow, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.argo_workflow is not None:
+            result['ArgoWorkflow'] = self.argo_workflow.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ArgoWorkflow') is not None:
+            temp_model = DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaDataACKOneWorkFlowArgoWorkflow()
+            self.argo_workflow = temp_model.from_map(m['ArgoWorkflow'])
+        return self
+
+
+class DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaDataACKOne(TeaModel):
+    def __init__(self, git_ops=None, work_flow=None):
+        # The GitOps metadata.
+        self.git_ops = git_ops  # type: DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaDataACKOneGitOps
+        # The workflow metadata.
+        self.work_flow = work_flow  # type: DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaDataACKOneWorkFlow
+
+    def validate(self):
+        if self.git_ops:
+            self.git_ops.validate()
+        if self.work_flow:
+            self.work_flow.validate()
+
+    def to_map(self):
+        _map = super(DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaDataACKOne, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, ackone=None):
+        # The cluster metadata.
+        self.ackone = ackone  # type: DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaDataACKOne
+
+    def validate(self):
+        if self.ackone:
+            self.ackone.validate()
+
+    def to_map(self):
+        _map = super(DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaData, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.ackone is not None:
+            result['ACKOne'] = self.ackone.to_map()
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('ACKOne') is not None:
+            temp_model = DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaDataACKOne()
+            self.ackone = temp_model.from_map(m['ACKOne'])
+        return self
+
+
 class DescribeHubClusterDetailsResponseBodyClusterClusterInfo(TeaModel):
-    def __init__(self, cluster_id=None, cluster_spec=None, creation_time=None, error_message=None, name=None,
-                 profile=None, region_id=None, state=None, update_time=None, version=None):
+    def __init__(self, cluster_id=None, cluster_spec=None, creation_time=None, error_message=None, meta_data=None,
+                 name=None, profile=None, region_id=None, resource_group_id=None, state=None, update_time=None,
+                 version=None):
         # The ID of the master instance.
         self.cluster_id = cluster_id  # type: str
         # The specification of the master instance. Valid value:
         # 
         # *   ack.pro.small: ACK Pro cluster
         self.cluster_spec = cluster_spec  # type: str
         # The time when the master instance was created.
         self.creation_time = creation_time  # type: str
         # The error message returned when the master instance failed to be created.
         self.error_message = error_message  # type: str
+        # The cluster metadata.
+        self.meta_data = meta_data  # type: DescribeHubClusterDetailsResponseBodyClusterClusterInfoMetaData
         # The name of the master instance.
         self.name = name  # type: str
         # The configurations of the master instance.
         self.profile = profile  # type: str
         # The ID of the region in which the master instance resides.
         self.region_id = region_id  # type: str
+        # The ID of Resource Group.
+        self.resource_group_id = resource_group_id  # type: str
         # The status of the master instance. Valid values:
         # 
         # *   initial: The master instance is being initialized.
         # *   failed: The master instance failed to be created.
         # *   running: The master instance is running
         # *   inactive: The master instance is pending.
         # *   deleting: The master instance is being deleted.
@@ -950,15 +1146,16 @@
         self.state = state  # type: str
         # The time when the master instance was updated.
         self.update_time = update_time  # type: str
         # The version of the master instance.
         self.version = version  # type: str
 
     def validate(self):
-        pass
+        if self.meta_data:
+            self.meta_data.validate()
 
     def to_map(self):
         _map = super(DescribeHubClusterDetailsResponseBodyClusterClusterInfo, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
@@ -966,20 +1163,24 @@
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
@@ -990,20 +1191,25 @@
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
@@ -1212,15 +1418,19 @@
         if m.get('VpcId') is not None:
             self.vpc_id = m.get('VpcId')
         return self
 
 
 class DescribeHubClusterDetailsResponseBodyClusterWorkflowConfigWorkflowUnitsVSwitches(TeaModel):
     def __init__(self, vswitch_id=None, zone_id=None):
+        # The ID of the vSwitch.
         self.vswitch_id = vswitch_id  # type: str
+        # The zone ID of the cluster.
+        # 
+        # > You can call the [DescribeRegions](~~143074~~) operation to query the most recent zone list.
         self.zone_id = zone_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeHubClusterDetailsResponseBodyClusterWorkflowConfigWorkflowUnitsVSwitches, self).to_map()
@@ -1241,16 +1451,21 @@
         if m.get('ZoneId') is not None:
             self.zone_id = m.get('ZoneId')
         return self
 
 
 class DescribeHubClusterDetailsResponseBodyClusterWorkflowConfigWorkflowUnits(TeaModel):
     def __init__(self, region_id=None, v_switches=None, vpc_id=None):
+        # The region ID of the cluster.
+        # 
+        # >  You can call the [DescribeRegions](~~143074~~) operation to query the most recent region list.
         self.region_id = region_id  # type: str
+        # The vSwitches.
         self.v_switches = v_switches  # type: list[DescribeHubClusterDetailsResponseBodyClusterWorkflowConfigWorkflowUnitsVSwitches]
+        # The ID of the VPC.
         self.vpc_id = vpc_id  # type: str
 
     def validate(self):
         if self.v_switches:
             for k in self.v_switches:
                 if k:
                     k.validate()
@@ -1284,17 +1499,27 @@
             self.vpc_id = m.get('VpcId')
         return self
 
 
 class DescribeHubClusterDetailsResponseBodyClusterWorkflowConfig(TeaModel):
     def __init__(self, argo_server_enabled=None, price_limit=None, workflow_schedule_mode=None,
                  workflow_units=None):
+        # Specifies whether to enable the workflow instance UI. This parameter takes effect only if Profile is set to XFlow. Valid values:
+        # 
+        # *   true
+        # *   false
         self.argo_server_enabled = argo_server_enabled  # type: bool
+        # The limit on the prices of containers in the workflow. This parameter takes effect only if the WorkflowScheduleMode parameter is set to cost-optimized.
         self.price_limit = price_limit  # type: str
+        # The scheduling mode of the workflow. This parameter takes effect only if Profile is set to XFlow. Valid values:
+        # 
+        # *   cost-optimized: cost-prioritized scheduling mode.
+        # *   stock-optimized: inventory-prioritized scheduling mode.
         self.workflow_schedule_mode = workflow_schedule_mode  # type: str
+        # The Argo workflow regions  configuration.
         self.workflow_units = workflow_units  # type: list[DescribeHubClusterDetailsResponseBodyClusterWorkflowConfigWorkflowUnits]
 
     def validate(self):
         if self.workflow_units:
             for k in self.workflow_units:
                 if k:
                     k.validate()
@@ -1346,14 +1571,15 @@
         self.endpoints = endpoints  # type: DescribeHubClusterDetailsResponseBodyClusterEndpoints
         # The logging configuration.
         self.log_config = log_config  # type: DescribeHubClusterDetailsResponseBodyClusterLogConfig
         # The configurations of Alibaba Cloud Service Mesh (ASM).
         self.mesh_config = mesh_config  # type: DescribeHubClusterDetailsResponseBodyClusterMeshConfig
         # The network configurations of the master instance.
         self.network = network  # type: DescribeHubClusterDetailsResponseBodyClusterNetwork
+        # The Argo workflow configuration.
         self.workflow_config = workflow_config  # type: DescribeHubClusterDetailsResponseBodyClusterWorkflowConfig
 
     def validate(self):
         if self.api_server:
             self.api_server.validate()
         if self.cluster_info:
             self.cluster_info.validate()
@@ -1465,17 +1691,14 @@
 class DescribeHubClusterDetailsResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DescribeHubClusterDetailsResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeHubClusterDetailsResponse, self).to_map()
         if _map is not None:
             return _map
@@ -1571,17 +1794,14 @@
 class DescribeHubClusterKubeconfigResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DescribeHubClusterKubeconfigResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeHubClusterKubeconfigResponse, self).to_map()
         if _map is not None:
             return _map
@@ -1717,17 +1937,14 @@
 class DescribeHubClusterLogsResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DescribeHubClusterLogsResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeHubClusterLogsResponse, self).to_map()
         if _map is not None:
             return _map
@@ -1750,41 +1967,54 @@
         if m.get('body') is not None:
             temp_model = DescribeHubClusterLogsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribeHubClustersRequest(TeaModel):
-    def __init__(self, profile=None):
+    def __init__(self, profile=None, resource_group_id=None):
+        # The configurations of the cluster.
         self.profile = profile  # type: str
+        # The resource group ID.
+        self.resource_group_id = resource_group_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeHubClustersRequest, self).to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.profile is not None:
             result['Profile'] = self.profile
+        if self.resource_group_id is not None:
+            result['ResourceGroupId'] = self.resource_group_id
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('Profile') is not None:
             self.profile = m.get('Profile')
+        if m.get('ResourceGroupId') is not None:
+            self.resource_group_id = m.get('ResourceGroupId')
         return self
 
 
 class DescribeHubClustersResponseBodyClustersApiServer(TeaModel):
     def __init__(self, api_server_eip_id=None, enabled_public=None, load_balancer_id=None):
+        # The elastic IP address (EIP) ID.
         self.api_server_eip_id = api_server_eip_id  # type: str
+        # Indicates whether public endpoint is enabled for the API server. Valid values:
+        # 
+        # *   true
+        # *   false
         self.enabled_public = enabled_public  # type: bool
+        # The ID of the Server Load Balancer (SLB) instance that is associated with the cluster.
         self.load_balancer_id = load_balancer_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeHubClustersResponseBodyClustersApiServer, self).to_map()
@@ -1809,24 +2039,46 @@
         if m.get('LoadBalancerId') is not None:
             self.load_balancer_id = m.get('LoadBalancerId')
         return self
 
 
 class DescribeHubClustersResponseBodyClustersClusterInfo(TeaModel):
     def __init__(self, cluster_id=None, cluster_spec=None, creation_time=None, error_message=None, name=None,
-                 profile=None, region_id=None, state=None, update_time=None, version=None):
+                 profile=None, region_id=None, resource_group_id=None, state=None, update_time=None, version=None):
+        # The cluster ID.
         self.cluster_id = cluster_id  # type: str
+        # The specification of the cluster.
+        # 
+        # *   Only ack.pro.small is returned.
         self.cluster_spec = cluster_spec  # type: str
+        # The time when the cluster was created.
         self.creation_time = creation_time  # type: str
+        # The error message that is returned if the cluster failed to be created.
         self.error_message = error_message  # type: str
+        # The name of the cluster.
         self.name = name  # type: str
+        # The configurations of the cluster.
         self.profile = profile  # type: str
+        # The region ID.
         self.region_id = region_id  # type: str
+        # The ID of Resource Group.
+        self.resource_group_id = resource_group_id  # type: str
+        # The status of the cluster. Valid values:
+        # 
+        # *   initial: The cluster is being initialized.
+        # *   failed: The cluster failed to be created.
+        # *   running: The cluster is running
+        # *   inactive: The cluster is pending.
+        # *   deleting: The cluster is being deleted.
+        # *   delete_failed: The cluster failed to be deleted.
+        # *   deleted: The cluster is deleted.
         self.state = state  # type: str
+        # The time when the cluster was last updated.
         self.update_time = update_time  # type: str
+        # The Kubernetes version of the cluster.
         self.version = version  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeHubClustersResponseBodyClustersClusterInfo, self).to_map()
@@ -1844,14 +2096,16 @@
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
@@ -1868,28 +2122,38 @@
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
 
 
 class DescribeHubClustersResponseBodyClustersConditions(TeaModel):
     def __init__(self, message=None, reason=None, status=None, type=None):
+        # The error message that is returned.
         self.message = message  # type: str
+        # The reason for the deletion condition.
         self.reason = reason  # type: str
+        # The status of the cluster that the deletion condition indicates. Valid values:
+        # 
+        # *   True: The cluster cannot be deleted.
+        # *   False: The cluster can be deleted.
+        # *   Unknow: Whether the cluster can be deleted is unknown.
         self.status = status  # type: str
+        # The type of deletion condition.
         self.type = type  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeHubClustersResponseBodyClustersConditions, self).to_map()
@@ -1918,15 +2182,17 @@
         if m.get('Type') is not None:
             self.type = m.get('Type')
         return self
 
 
 class DescribeHubClustersResponseBodyClustersEndpoints(TeaModel):
     def __init__(self, intranet_api_server_endpoint=None, public_api_server_endpoint=None):
+        # The internal endpoint of the API server.
         self.intranet_api_server_endpoint = intranet_api_server_endpoint  # type: str
+        # The public endpoint of the API server.
         self.public_api_server_endpoint = public_api_server_endpoint  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeHubClustersResponseBodyClustersEndpoints, self).to_map()
@@ -1947,16 +2213,22 @@
         if m.get('PublicApiServerEndpoint') is not None:
             self.public_api_server_endpoint = m.get('PublicApiServerEndpoint')
         return self
 
 
 class DescribeHubClustersResponseBodyClustersLogConfig(TeaModel):
     def __init__(self, enable_log=None, log_project=None, log_store_ttl=None):
+        # Indicates whether the audit logging feature is enabled. Valid values:
+        # 
+        # *   true
+        # *   false
         self.enable_log = enable_log  # type: bool
+        # The name of the project in Simple Log Service.
         self.log_project = log_project  # type: str
+        # The number of days that logs are retained by Simple Log Service.
         self.log_store_ttl = log_store_ttl  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeHubClustersResponseBodyClustersLogConfig, self).to_map()
@@ -1981,15 +2253,20 @@
         if m.get('LogStoreTTL') is not None:
             self.log_store_ttl = m.get('LogStoreTTL')
         return self
 
 
 class DescribeHubClustersResponseBodyClustersMeshConfig(TeaModel):
     def __init__(self, enable_mesh=None, mesh_id=None):
+        # Indicates whether ASM is enabled. Valid values:
+        # 
+        # *   true
+        # *   false
         self.enable_mesh = enable_mesh  # type: bool
+        # The ASM instance ID.
         self.mesh_id = mesh_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeHubClustersResponseBodyClustersMeshConfig, self).to_map()
@@ -2010,17 +2287,21 @@
         if m.get('MeshId') is not None:
             self.mesh_id = m.get('MeshId')
         return self
 
 
 class DescribeHubClustersResponseBodyClustersNetwork(TeaModel):
     def __init__(self, cluster_domain=None, security_group_ids=None, v_switches=None, vpc_id=None):
+        # The domain name of the cluster.
         self.cluster_domain = cluster_domain  # type: str
+        # The security group IDs.
         self.security_group_ids = security_group_ids  # type: list[str]
+        # The IDs of vSwitches to which the cluster belongs.
         self.v_switches = v_switches  # type: list[str]
+        # The ID of the virtual private cloud (VPC) to which the cluster belongs.
         self.vpc_id = vpc_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribeHubClustersResponseBodyClustersNetwork, self).to_map()
@@ -2050,20 +2331,27 @@
             self.vpc_id = m.get('VpcId')
         return self
 
 
 class DescribeHubClustersResponseBodyClusters(TeaModel):
     def __init__(self, api_server=None, cluster_info=None, conditions=None, endpoints=None, log_config=None,
                  mesh_config=None, network=None):
+        # The information about the API server.
         self.api_server = api_server  # type: DescribeHubClustersResponseBodyClustersApiServer
+        # The details of the cluster.
         self.cluster_info = cluster_info  # type: DescribeHubClustersResponseBodyClustersClusterInfo
+        # The deletion conditions of the cluster.
         self.conditions = conditions  # type: list[DescribeHubClustersResponseBodyClustersConditions]
+        # The endpoint of the cluster.
         self.endpoints = endpoints  # type: DescribeHubClustersResponseBodyClustersEndpoints
+        # The logging configurations.
         self.log_config = log_config  # type: DescribeHubClustersResponseBodyClustersLogConfig
+        # The configurations of Alibaba Cloud Service Mesh (ASM).
         self.mesh_config = mesh_config  # type: DescribeHubClustersResponseBodyClustersMeshConfig
+        # The network configurations of the cluster.
         self.network = network  # type: DescribeHubClustersResponseBodyClustersNetwork
 
     def validate(self):
         if self.api_server:
             self.api_server.validate()
         if self.cluster_info:
             self.cluster_info.validate()
@@ -2130,15 +2418,17 @@
             temp_model = DescribeHubClustersResponseBodyClustersNetwork()
             self.network = temp_model.from_map(m['Network'])
         return self
 
 
 class DescribeHubClustersResponseBody(TeaModel):
     def __init__(self, clusters=None, request_id=None):
+        # The information about clusters.
         self.clusters = clusters  # type: list[DescribeHubClustersResponseBodyClusters]
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.clusters:
             for k in self.clusters:
                 if k:
                     k.validate()
@@ -2172,17 +2462,14 @@
 class DescribeHubClustersResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DescribeHubClustersResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeHubClustersResponse, self).to_map()
         if _map is not None:
             return _map
@@ -2480,17 +2767,14 @@
 class DescribeManagedClustersResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DescribeManagedClustersResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeManagedClustersResponse, self).to_map()
         if _map is not None:
             return _map
@@ -2589,17 +2873,14 @@
 class DescribePoliciesResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DescribePoliciesResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribePoliciesResponse, self).to_map()
         if _map is not None:
             return _map
@@ -2623,15 +2904,15 @@
             temp_model = DescribePoliciesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DescribePolicyDetailsRequest(TeaModel):
     def __init__(self, policy_name=None):
-        # The name of the policy.
+        # The policy name.
         self.policy_name = policy_name  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(DescribePolicyDetailsRequest, self).to_map()
@@ -2665,15 +2946,15 @@
         # The description of the policy.
         self.description = description  # type: str
         # The name of the policy.
         self.name = name  # type: str
         # Indicates whether parameters are required. Valid values:
         # 
         # *   0: Parameters are required.
-        # *   1: Parameters are optional.
+        # *   1: Parameters are not required.
         self.no_config = no_config  # type: int
         # The severity level of the policy.
         self.severity = severity  # type: str
         # The content of the policy.
         self.template = template  # type: str
         # The time when the policy was last updated.
         self.updated = updated  # type: str
@@ -2728,15 +3009,15 @@
         if m.get('Updated') is not None:
             self.updated = m.get('Updated')
         return self
 
 
 class DescribePolicyDetailsResponseBody(TeaModel):
     def __init__(self, policy=None, request_id=None):
-        # Detailed information about the policy.
+        # The policies.
         self.policy = policy  # type: DescribePolicyDetailsResponseBodyPolicy
         # The request ID.
         self.request_id = request_id  # type: str
 
     def validate(self):
         if self.policy:
             self.policy.validate()
@@ -2766,17 +3047,14 @@
 class DescribePolicyDetailsResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DescribePolicyDetailsResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribePolicyDetailsResponse, self).to_map()
         if _map is not None:
             return _map
@@ -3387,17 +3665,14 @@
 class DescribePolicyGovernanceInClusterResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DescribePolicyGovernanceInClusterResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribePolicyGovernanceInClusterResponse, self).to_map()
         if _map is not None:
             return _map
@@ -3584,17 +3859,14 @@
 class DescribePolicyInstancesResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DescribePolicyInstancesResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribePolicyInstancesResponse, self).to_map()
         if _map is not None:
             return _map
@@ -3855,17 +4127,14 @@
 class DescribePolicyInstancesStatusResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DescribePolicyInstancesStatusResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribePolicyInstancesStatusResponse, self).to_map()
         if _map is not None:
             return _map
@@ -3989,17 +4258,14 @@
 class DescribeRegionsResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DescribeRegionsResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeRegionsResponse, self).to_map()
         if _map is not None:
             return _map
@@ -4145,17 +4411,14 @@
 class DescribeUserPermissionsResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DescribeUserPermissionsResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DescribeUserPermissionsResponse, self).to_map()
         if _map is not None:
             return _map
@@ -4262,17 +4525,14 @@
 class DetachClusterFromHubResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: DetachClusterFromHubResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(DetachClusterFromHubResponse, self).to_map()
         if _map is not None:
             return _map
@@ -4297,49 +4557,29 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class GrantUserPermissionRequest(TeaModel):
     def __init__(self, cluster_id=None, is_ram_role=None, namespace=None, role_name=None, role_type=None,
                  user_id=None):
+        # The ID of the cluster.
         self.cluster_id = cluster_id  # type: str
         # The entity to which the permissions are granted. A value of `true` indicates that the permissions are granted to a RAM user. A value of `false` indicates that the permissions are granted to a RAM role.
         self.is_ram_role = is_ram_role  # type: bool
+        # The namespace to which the permissions are scoped. By default, this parameter is empty when you set RoleType to cluster.
         self.namespace = namespace  # type: str
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
         self.role_name = role_name  # type: str
+        # The authorization type. Valid values:
+        # 
+        # *   cluster: specifies that the permissions are scoped to a master instance.
+        # *   namespace: specifies that the permissions are scoped to a namespace of a cluster.
         self.role_type = role_type  # type: str
         # The ID of the RAM user or RAM role.
         self.user_id = user_id  # type: str
 
     def validate(self):
         pass
 
@@ -4378,14 +4618,15 @@
         if m.get('UserId') is not None:
             self.user_id = m.get('UserId')
         return self
 
 
 class GrantUserPermissionResponseBody(TeaModel):
     def __init__(self, request_id=None):
+        # The ID of the request.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(GrantUserPermissionResponseBody, self).to_map()
@@ -4407,17 +4648,14 @@
 class GrantUserPermissionResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GrantUserPermissionResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GrantUserPermissionResponse, self).to_map()
         if _map is not None:
             return _map
@@ -4445,14 +4683,15 @@
 
 class GrantUserPermissionsRequestPermissions(TeaModel):
     def __init__(self, cluster_id=None, is_ram_role=None, namespace=None, role_name=None, role_type=None):
         # The master instance ID.
         # 
         # *   When the role_type parameter is set to all-clusters, set the parameter to an empty string.
         self.cluster_id = cluster_id  # type: str
+        # The entity to which the permissions are granted. A value of `true` indicates that the permissions are granted to a RAM user. A value of `false` indicates that the permissions are granted to a RAM role.
         self.is_ram_role = is_ram_role  # type: bool
         # The namespace to which the permissions are scoped. By default, this parameter is empty when you set RoleType to cluster.
         self.namespace = namespace  # type: str
         # The predefined role that you want to assign. Valid values:
         # 
         # *   admin: the administrator role.
         # *   dev: the developer role.
@@ -4598,17 +4837,14 @@
 class GrantUserPermissionsResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: GrantUserPermissionsResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(GrantUserPermissionsResponse, self).to_map()
         if _map is not None:
             return _map
@@ -4633,15 +4869,15 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class UpdateHubClusterFeatureRequest(TeaModel):
     def __init__(self, access_control_list=None, api_server_eip_id=None, argo_cdenabled=None,
                  argo_cdhaenabled=None, argo_events_enabled=None, argo_server_enabled=None, audit_log_enabled=None, cluster_id=None,
-                 deletion_protection=None, enable_mesh=None, mseenabled=None, monitor_enabled=None, name=None, price_limit=None,
+                 deletion_protection=None, enable_mesh=None, gateway_enabled=None, monitor_enabled=None, name=None, price_limit=None,
                  public_access_enabled=None, public_api_server_enabled=None, v_switches=None, workflow_schedule_mode=None):
         # The Internet access control list (ACL). This parameter takes effect only if PublicAccessEnabled is set to true.
         self.access_control_list = access_control_list  # type: list[str]
         # The ID of the EIP.
         self.api_server_eip_id = api_server_eip_id  # type: str
         # Specifies whether to enable Argo CD. This parameter takes effect only if Profile is set to XFlow. Valid values:
         # 
@@ -4678,15 +4914,18 @@
         # Default value: false.
         self.deletion_protection = deletion_protection  # type: bool
         # Specifies whether to enable Service Mesh (ASM). Valid values:
         # 
         # *   true
         # *   false
         self.enable_mesh = enable_mesh  # type: bool
-        self.mseenabled = mseenabled  # type: bool
+        # Specifies whether to enable Gateway. Valid values:
+        # - true
+        # - false
+        self.gateway_enabled = gateway_enabled  # type: bool
         # Specifies whether to enable the monitoring dashboard feature for the workflow instance. This parameter takes effect only if Profile is set to XFlow. Valid values:
         # 
         # *   true
         # *   false
         self.monitor_enabled = monitor_enabled  # type: bool
         # The name of the master instance. The name must be 1 to 63 characters in length. It must start with a letter, and can contain letters, digits, underscores (\_), and hyphens (-).
         self.name = name  # type: str
@@ -4735,16 +4974,16 @@
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
@@ -4775,16 +5014,16 @@
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
@@ -4797,15 +5036,15 @@
             self.workflow_schedule_mode = m.get('WorkflowScheduleMode')
         return self
 
 
 class UpdateHubClusterFeatureShrinkRequest(TeaModel):
     def __init__(self, access_control_list_shrink=None, api_server_eip_id=None, argo_cdenabled=None,
                  argo_cdhaenabled=None, argo_events_enabled=None, argo_server_enabled=None, audit_log_enabled=None, cluster_id=None,
-                 deletion_protection=None, enable_mesh=None, mseenabled=None, monitor_enabled=None, name=None, price_limit=None,
+                 deletion_protection=None, enable_mesh=None, gateway_enabled=None, monitor_enabled=None, name=None, price_limit=None,
                  public_access_enabled=None, public_api_server_enabled=None, v_switches_shrink=None, workflow_schedule_mode=None):
         # The Internet access control list (ACL). This parameter takes effect only if PublicAccessEnabled is set to true.
         self.access_control_list_shrink = access_control_list_shrink  # type: str
         # The ID of the EIP.
         self.api_server_eip_id = api_server_eip_id  # type: str
         # Specifies whether to enable Argo CD. This parameter takes effect only if Profile is set to XFlow. Valid values:
         # 
@@ -4842,15 +5081,18 @@
         # Default value: false.
         self.deletion_protection = deletion_protection  # type: bool
         # Specifies whether to enable Service Mesh (ASM). Valid values:
         # 
         # *   true
         # *   false
         self.enable_mesh = enable_mesh  # type: bool
-        self.mseenabled = mseenabled  # type: bool
+        # Specifies whether to enable Gateway. Valid values:
+        # - true
+        # - false
+        self.gateway_enabled = gateway_enabled  # type: bool
         # Specifies whether to enable the monitoring dashboard feature for the workflow instance. This parameter takes effect only if Profile is set to XFlow. Valid values:
         # 
         # *   true
         # *   false
         self.monitor_enabled = monitor_enabled  # type: bool
         # The name of the master instance. The name must be 1 to 63 characters in length. It must start with a letter, and can contain letters, digits, underscores (\_), and hyphens (-).
         self.name = name  # type: str
@@ -4899,16 +5141,16 @@
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
@@ -4939,16 +5181,16 @@
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
@@ -4990,17 +5232,14 @@
 class UpdateHubClusterFeatureResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: UpdateHubClusterFeatureResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(UpdateHubClusterFeatureResponse, self).to_map()
         if _map is not None:
             return _map
@@ -5109,17 +5348,14 @@
 class UpdateUserPermissionResponse(TeaModel):
     def __init__(self, headers=None, status_code=None, body=None):
         self.headers = headers  # type: dict[str, str]
         self.status_code = status_code  # type: int
         self.body = body  # type: UpdateUserPermissionResponseBody
 
     def validate(self):
-        self.validate_required(self.headers, 'headers')
-        self.validate_required(self.status_code, 'status_code')
-        self.validate_required(self.body, 'body')
         if self.body:
             self.body.validate()
 
     def to_map(self):
         _map = super(UpdateUserPermissionResponse, self).to_map()
         if _map is not None:
             return _map
```

### Comparing `alibabacloud_adcp20220101_py2-2.0.2/alibabacloud_adcp20220101_py2.egg-info/PKG-INFO` & `alibabacloud_adcp20220101_py2-3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-adcp20220101-py2
-Version: 2.0.2
+Name: alibabacloud_adcp20220101_py2
+Version: 3.0.0
 Summary: Alibaba Cloud adcp (20220101) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_adcp20220101_py2-2.0.2/setup.py` & `alibabacloud_adcp20220101_py2-3.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,29 +21,29 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_adcp20220101_py2.
 
-Created on 12/10/2023
+Created on 22/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_adcp20220101"
 NAME = "alibabacloud_adcp20220101_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud adcp (20220101) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util_py2>=0.0.9, <1.0.0",
-    "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
+    "alibabacloud_tea_openapi_py2>=0.1.8, <1.0.0",
     "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
```


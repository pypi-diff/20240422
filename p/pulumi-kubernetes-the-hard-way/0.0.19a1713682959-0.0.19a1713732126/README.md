# Comparing `tmp/pulumi_kubernetes_the_hard_way-0.0.19a1713682959.tar.gz` & `tmp/pulumi_kubernetes_the_hard_way-0.0.19a1713732126.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.19a1713682959.tar", last modified: Sun Apr 21 07:05:19 2024, max compression
+gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.19a1713732126.tar", last modified: Sun Apr 21 20:44:39 2024, max compression
```

## Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959.tar` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:05:19.176870 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-21 07:05:19.176870 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:05:19.164870 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/
--rw-------   0 runner    (1001) docker     (127)     4080 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/__init__.py
--rw-------   0 runner    (1001) docker     (127)     9268 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:05:19.164870 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/config/
--rw-------   0 runner    (1001) docker     (127)      418 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      427 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/config/_enums.py
--rw-------   0 runner    (1001) docker     (127)    21101 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/config/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     8728 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)     3426 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
--rw-------   0 runner    (1001) docker     (127)    23922 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)    29159 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/config/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2783 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/provider.py
--rw-------   0 runner    (1001) docker     (127)      116 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:05:19.168870 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/
--rw-------   0 runner    (1001) docker     (127)      940 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1095 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/_enums.py
--rw-------   0 runner    (1001) docker     (127)    15965 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    19229 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
--rw-------   0 runner    (1001) docker     (127)    10255 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
--rw-------   0 runner    (1001) docker     (127)    10159 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
--rw-------   0 runner    (1001) docker     (127)     8328 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/download.py
--rw-------   0 runner    (1001) docker     (127)    12377 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
--rw-------   0 runner    (1001) docker     (127)    14905 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
--rw-------   0 runner    (1001) docker     (127)    10651 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
--rw-------   0 runner    (1001) docker     (127)    14696 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
--rw-------   0 runner    (1001) docker     (127)     7339 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/file.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
--rw-------   0 runner    (1001) docker     (127)     9822 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
--rw-------   0 runner    (1001) docker     (127)     9652 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
--rw-------   0 runner    (1001) docker     (127)    15536 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/outputs.py
--rw-------   0 runner    (1001) docker     (127)    13390 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
--rw-------   0 runner    (1001) docker     (127)     9580 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/runc_install.py
--rw-------   0 runner    (1001) docker     (127)     5113 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
--rw-------   0 runner    (1001) docker     (127)     7429 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/static_pod.py
--rw-------   0 runner    (1001) docker     (127)    10944 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:05:19.172870 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tls/
--rw-------   0 runner    (1001) docker     (127)      425 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tls/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1000 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tls/_enums.py
--rw-------   0 runner    (1001) docker     (127)     3019 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tls/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    30597 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tls/certificate.py
--rw-------   0 runner    (1001) docker     (127)    15919 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
--rw-------   0 runner    (1001) docker     (127)     4450 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
--rw-------   0 runner    (1001) docker     (127)     2983 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tls/outputs.py
--rw-------   0 runner    (1001) docker     (127)    27130 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tls/root_ca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:05:19.176870 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/
--rw-------   0 runner    (1001) docker     (127)      590 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/__init__.py
--rw-------   0 runner    (1001) docker     (127)     3166 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/_enums.py
--rw-------   0 runner    (1001) docker     (127)   108421 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    14165 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/chmod.py
--rw-------   0 runner    (1001) docker     (127)    14181 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/curl.py
--rw-------   0 runner    (1001) docker     (127)    14263 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
--rw-------   0 runner    (1001) docker     (127)    14415 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
--rw-------   0 runner    (1001) docker     (127)    14165 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/mkdir.py
--rw-------   0 runner    (1001) docker     (127)    14203 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/mktemp.py
--rw-------   0 runner    (1001) docker     (127)    14051 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/mv.py
--rw-------   0 runner    (1001) docker     (127)    91760 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/outputs.py
--rw-------   0 runner    (1001) docker     (127)    14051 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/rm.py
--rw-------   0 runner    (1001) docker     (127)    14089 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/sed.py
--rw-------   0 runner    (1001) docker     (127)    14339 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/systemctl.py
--rw-------   0 runner    (1001) docker     (127)    14089 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/tar.py
--rw-------   0 runner    (1001) docker     (127)    14109 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/tee.py
--rw-------   0 runner    (1001) docker     (127)    14127 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/wget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 07:05:19.176870 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-21 07:05:19.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-21 07:05:19.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 07:05:19.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-21 07:05:19.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-21 07:05:19.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      899 2024-04-21 07:05:11.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 07:05:19.176870 pulumi_kubernetes_the_hard_way-0.0.19a1713682959/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:44:39.282924 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-21 20:44:39.282924 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:44:39.266924 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/
+-rw-------   0 runner    (1001) docker     (127)     4080 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9268 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:44:39.270923 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/config/
+-rw-------   0 runner    (1001) docker     (127)      418 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/config/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      427 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/config/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    21101 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/config/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     8728 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)     3426 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
+-rw-------   0 runner    (1001) docker     (127)    23922 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)    29159 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/config/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2783 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/provider.py
+-rw-------   0 runner    (1001) docker     (127)      116 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:44:39.274924 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/
+-rw-------   0 runner    (1001) docker     (127)      940 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1095 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    15965 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    19229 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
+-rw-------   0 runner    (1001) docker     (127)    10255 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
+-rw-------   0 runner    (1001) docker     (127)    10159 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
+-rw-------   0 runner    (1001) docker     (127)     8328 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/download.py
+-rw-------   0 runner    (1001) docker     (127)    12377 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
+-rw-------   0 runner    (1001) docker     (127)    14905 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    10651 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
+-rw-------   0 runner    (1001) docker     (127)    14696 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
+-rw-------   0 runner    (1001) docker     (127)     7339 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/file.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
+-rw-------   0 runner    (1001) docker     (127)     9822 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
+-rw-------   0 runner    (1001) docker     (127)     9652 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
+-rw-------   0 runner    (1001) docker     (127)    15536 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    13390 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     9580 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/runc_install.py
+-rw-------   0 runner    (1001) docker     (127)     5113 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     7429 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/static_pod.py
+-rw-------   0 runner    (1001) docker     (127)    10944 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:44:39.278924 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tls/
+-rw-------   0 runner    (1001) docker     (127)      425 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tls/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1000 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tls/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     3019 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tls/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    30597 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tls/certificate.py
+-rw-------   0 runner    (1001) docker     (127)    15919 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
+-rw-------   0 runner    (1001) docker     (127)     4450 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
+-rw-------   0 runner    (1001) docker     (127)     2983 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tls/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    27130 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tls/root_ca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:44:39.278924 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/
+-rw-------   0 runner    (1001) docker     (127)      590 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     3166 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/_enums.py
+-rw-------   0 runner    (1001) docker     (127)   108421 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    14957 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/chmod.py
+-rw-------   0 runner    (1001) docker     (127)    14976 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/curl.py
+-rw-------   0 runner    (1001) docker     (127)    15049 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
+-rw-------   0 runner    (1001) docker     (127)    15189 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
+-rw-------   0 runner    (1001) docker     (127)    14957 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/mkdir.py
+-rw-------   0 runner    (1001) docker     (127)    14992 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/mktemp.py
+-rw-------   0 runner    (1001) docker     (127)    14852 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/mv.py
+-rw-------   0 runner    (1001) docker     (127)    91760 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    14852 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/rm.py
+-rw-------   0 runner    (1001) docker     (127)    14887 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/sed.py
+-rw-------   0 runner    (1001) docker     (127)    15119 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/systemctl.py
+-rw-------   0 runner    (1001) docker     (127)    14887 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/tar.py
+-rw-------   0 runner    (1001) docker     (127)    14907 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/tee.py
+-rw-------   0 runner    (1001) docker     (127)    14922 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/wget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 20:44:39.282924 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-21 20:44:39.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-21 20:44:39.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 20:44:39.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-21 20:44:39.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-21 20:44:39.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      899 2024-04-21 20:44:29.000000 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 20:44:39.282924 pulumi_kubernetes_the_hard_way-0.0.19a1713732126/setup.cfg
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.19a1713682959
+Version: 0.0.19a1713732126
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/README.md` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/_utilities.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/config/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/config/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/config/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/provider.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/containerd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/containerd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/crictl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/crictl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/download.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/download.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/etcd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/etcd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/etcd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/etcd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/file.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/runc_install.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/runc_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/start_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/start_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/static_pod.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/static_pod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/remote/systemd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/remote/systemd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tls/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tls/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tls/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tls/certificate.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tls/encryption_key.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tls/encryption_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tls/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tls/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tls/root_ca.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tls/root_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/chmod.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/chmod.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,32 +15,32 @@
 __all__ = ['ChmodArgs', 'Chmod']
 
 @pulumi.input_type
 class ChmodArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 create: Optional['ChmodOptsArgs'] = None,
-                 delete: Optional['ChmodOptsArgs'] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input['ChmodOptsArgs']]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input['ChmodOptsArgs']]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional['ChmodOptsArgs'] = None):
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input['ChmodOptsArgs']]] = None):
         """
         The set of arguments for constructing a Chmod resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param 'ChmodOptsArgs' create: The command to run on create.
-        :param 'ChmodOptsArgs' delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input['ChmodOptsArgs']] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input['ChmodOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param 'ChmodOptsArgs' update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input['ChmodOptsArgs']] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
@@ -79,36 +79,36 @@
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def create(self) -> Optional['ChmodOptsArgs']:
+    def create(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['ChmodOptsArgs']]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @create.setter
-    def create(self, value: Optional['ChmodOptsArgs']):
+    def create(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['ChmodOptsArgs']]]):
         pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def delete(self) -> Optional['ChmodOptsArgs']:
+    def delete(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['ChmodOptsArgs']]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
     @delete.setter
-    def delete(self, value: Optional['ChmodOptsArgs']):
+    def delete(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['ChmodOptsArgs']]]):
         pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
     def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Environment variables
@@ -141,57 +141,57 @@
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
     @property
     @pulumi.getter
-    def update(self) -> Optional['ChmodOptsArgs']:
+    def update(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['ChmodOptsArgs']]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
 
     @update.setter
-    def update(self, value: Optional['ChmodOptsArgs']):
+    def update(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['ChmodOptsArgs']]]):
         pulumi.set(self, "update", value)
 
 
 class Chmod(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[pulumi.InputType['ChmodOptsArgs']] = None,
-                 delete: Optional[pulumi.InputType['ChmodOptsArgs']] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['ChmodOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['ChmodOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[pulumi.InputType['ChmodOptsArgs']] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['ChmodOptsArgs']]]] = None,
                  __props__=None):
         """
         Abstraction over the `chmod` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
-        :param pulumi.InputType['ChmodOptsArgs'] create: The command to run on create.
-        :param pulumi.InputType['ChmodOptsArgs'] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['ChmodOptsArgs']]] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['ChmodOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param pulumi.InputType['ChmodOptsArgs'] update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['ChmodOptsArgs']]] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
@@ -214,20 +214,20 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[pulumi.InputType['ChmodOptsArgs']] = None,
-                 delete: Optional[pulumi.InputType['ChmodOptsArgs']] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['ChmodOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['ChmodOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[pulumi.InputType['ChmodOptsArgs']] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['ChmodOptsArgs']]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
@@ -277,23 +277,23 @@
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter
-    def create(self) -> pulumi.Output[Optional['outputs.ChmodOpts']]:
+    def create(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @property
     @pulumi.getter
-    def delete(self) -> pulumi.Output[Optional['outputs.ChmodOpts']]:
+    def delete(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
@@ -335,15 +335,15 @@
         """
         TODO
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
-    def update(self) -> pulumi.Output[Optional['outputs.ChmodOpts']]:
+    def update(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/curl.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/mv.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,43 +5,42 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
-from ._enums import *
 from ._inputs import *
 import pulumi_command
 
-__all__ = ['CurlArgs', 'Curl']
+__all__ = ['MvArgs', 'Mv']
 
 @pulumi.input_type
-class CurlArgs:
+class MvArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 create: Optional['CurlOptsArgs'] = None,
-                 delete: Optional['CurlOptsArgs'] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional['CurlOptsArgs'] = None):
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]] = None):
         """
-        The set of arguments for constructing a Curl resource.
+        The set of arguments for constructing a Mv resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param 'CurlOptsArgs' create: The command to run on create.
-        :param 'CurlOptsArgs' delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param 'CurlOptsArgs' update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
@@ -80,36 +79,36 @@
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def create(self) -> Optional['CurlOptsArgs']:
+    def create(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @create.setter
-    def create(self, value: Optional['CurlOptsArgs']):
+    def create(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]]):
         pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def delete(self) -> Optional['CurlOptsArgs']:
+    def delete(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
     @delete.setter
-    def delete(self, value: Optional['CurlOptsArgs']):
+    def delete(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]]):
         pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
     def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Environment variables
@@ -142,119 +141,119 @@
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
     @property
     @pulumi.getter
-    def update(self) -> Optional['CurlOptsArgs']:
+    def update(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
 
     @update.setter
-    def update(self, value: Optional['CurlOptsArgs']):
+    def update(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MvOptsArgs']]]):
         pulumi.set(self, "update", value)
 
 
-class Curl(pulumi.ComponentResource):
+class Mv(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[pulumi.InputType['CurlOptsArgs']] = None,
-                 delete: Optional[pulumi.InputType['CurlOptsArgs']] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[pulumi.InputType['CurlOptsArgs']] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]]] = None,
                  __props__=None):
         """
-        Abstraction over the `curl` utility on a remote system. Transfer a URL.
+        Abstraction over the `mv` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
-        :param pulumi.InputType['CurlOptsArgs'] create: The command to run on create.
-        :param pulumi.InputType['CurlOptsArgs'] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param pulumi.InputType['CurlOptsArgs'] update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: CurlArgs,
+                 args: MvArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Abstraction over the `curl` utility on a remote system. Transfer a URL.
+        Abstraction over the `mv` utility on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param CurlArgs args: The arguments to use to populate this resource's properties.
+        :param MvArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(CurlArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(MvArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[pulumi.InputType['CurlOptsArgs']] = None,
-                 delete: Optional[pulumi.InputType['CurlOptsArgs']] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[pulumi.InputType['CurlOptsArgs']] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MvOptsArgs']]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = CurlArgs.__new__(CurlArgs)
+            __props__ = MvArgs.__new__(MvArgs)
 
             __props__.__dict__["binary_path"] = binary_path
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
             __props__.__dict__["create"] = create
             __props__.__dict__["delete"] = delete
             __props__.__dict__["environment"] = environment
             __props__.__dict__["stdin"] = stdin
             __props__.__dict__["triggers"] = triggers
             __props__.__dict__["update"] = update
             __props__.__dict__["command"] = None
             __props__.__dict__["stderr"] = None
             __props__.__dict__["stdout"] = None
-        super(Curl, __self__).__init__(
-            'kubernetes-the-hard-way:tools:Curl',
+        super(Mv, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Mv',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter(name="binaryPath")
@@ -278,23 +277,23 @@
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter
-    def create(self) -> pulumi.Output[Optional['outputs.CurlOpts']]:
+    def create(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @property
     @pulumi.getter
-    def delete(self) -> pulumi.Output[Optional['outputs.CurlOpts']]:
+    def delete(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
@@ -336,15 +335,15 @@
         """
         TODO
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
-    def update(self) -> pulumi.Output[Optional['outputs.CurlOpts']]:
+    def update(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/etcdctl.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/etcdctl.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,32 +16,32 @@
 __all__ = ['EtcdctlArgs', 'Etcdctl']
 
 @pulumi.input_type
 class EtcdctlArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 create: Optional['EtcdctlOptsArgs'] = None,
-                 delete: Optional['EtcdctlOptsArgs'] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input['EtcdctlOptsArgs']]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input['EtcdctlOptsArgs']]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional['EtcdctlOptsArgs'] = None):
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input['EtcdctlOptsArgs']]] = None):
         """
         The set of arguments for constructing a Etcdctl resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param 'EtcdctlOptsArgs' create: The command to run on create.
-        :param 'EtcdctlOptsArgs' delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input['EtcdctlOptsArgs']] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input['EtcdctlOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param 'EtcdctlOptsArgs' update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input['EtcdctlOptsArgs']] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
@@ -80,36 +80,36 @@
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def create(self) -> Optional['EtcdctlOptsArgs']:
+    def create(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['EtcdctlOptsArgs']]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @create.setter
-    def create(self, value: Optional['EtcdctlOptsArgs']):
+    def create(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['EtcdctlOptsArgs']]]):
         pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def delete(self) -> Optional['EtcdctlOptsArgs']:
+    def delete(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['EtcdctlOptsArgs']]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
     @delete.setter
-    def delete(self, value: Optional['EtcdctlOptsArgs']):
+    def delete(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['EtcdctlOptsArgs']]]):
         pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
     def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Environment variables
@@ -142,57 +142,57 @@
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
     @property
     @pulumi.getter
-    def update(self) -> Optional['EtcdctlOptsArgs']:
+    def update(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['EtcdctlOptsArgs']]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
 
     @update.setter
-    def update(self, value: Optional['EtcdctlOptsArgs']):
+    def update(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['EtcdctlOptsArgs']]]):
         pulumi.set(self, "update", value)
 
 
 class Etcdctl(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[pulumi.InputType['EtcdctlOptsArgs']] = None,
-                 delete: Optional[pulumi.InputType['EtcdctlOptsArgs']] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['EtcdctlOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['EtcdctlOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[pulumi.InputType['EtcdctlOptsArgs']] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['EtcdctlOptsArgs']]]] = None,
                  __props__=None):
         """
         Abstraction over the `etcdctl` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
-        :param pulumi.InputType['EtcdctlOptsArgs'] create: The command to run on create.
-        :param pulumi.InputType['EtcdctlOptsArgs'] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['EtcdctlOptsArgs']]] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['EtcdctlOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param pulumi.InputType['EtcdctlOptsArgs'] update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['EtcdctlOptsArgs']]] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
@@ -215,20 +215,20 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[pulumi.InputType['EtcdctlOptsArgs']] = None,
-                 delete: Optional[pulumi.InputType['EtcdctlOptsArgs']] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['EtcdctlOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['EtcdctlOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[pulumi.InputType['EtcdctlOptsArgs']] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['EtcdctlOptsArgs']]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
@@ -278,23 +278,23 @@
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter
-    def create(self) -> pulumi.Output[Optional['outputs.EtcdctlOpts']]:
+    def create(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @property
     @pulumi.getter
-    def delete(self) -> pulumi.Output[Optional['outputs.EtcdctlOpts']]:
+    def delete(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
@@ -336,15 +336,15 @@
         """
         TODO
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
-    def update(self) -> pulumi.Output[Optional['outputs.EtcdctlOpts']]:
+    def update(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/tar.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,43 +5,42 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
-from ._enums import *
 from ._inputs import *
 import pulumi_command
 
-__all__ = ['HostnamectlArgs', 'Hostnamectl']
+__all__ = ['TarArgs', 'Tar']
 
 @pulumi.input_type
-class HostnamectlArgs:
+class TarArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 create: Optional['HostnamectlOptsArgs'] = None,
-                 delete: Optional['HostnamectlOptsArgs'] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input['TarOptsArgs']]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input['TarOptsArgs']]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional['HostnamectlOptsArgs'] = None):
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input['TarOptsArgs']]] = None):
         """
-        The set of arguments for constructing a Hostnamectl resource.
+        The set of arguments for constructing a Tar resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param 'HostnamectlOptsArgs' create: The command to run on create.
-        :param 'HostnamectlOptsArgs' delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input['TarOptsArgs']] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input['TarOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param 'HostnamectlOptsArgs' update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input['TarOptsArgs']] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
@@ -80,36 +79,36 @@
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def create(self) -> Optional['HostnamectlOptsArgs']:
+    def create(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['TarOptsArgs']]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @create.setter
-    def create(self, value: Optional['HostnamectlOptsArgs']):
+    def create(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['TarOptsArgs']]]):
         pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def delete(self) -> Optional['HostnamectlOptsArgs']:
+    def delete(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['TarOptsArgs']]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
     @delete.setter
-    def delete(self, value: Optional['HostnamectlOptsArgs']):
+    def delete(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['TarOptsArgs']]]):
         pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
     def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Environment variables
@@ -142,119 +141,119 @@
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
     @property
     @pulumi.getter
-    def update(self) -> Optional['HostnamectlOptsArgs']:
+    def update(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['TarOptsArgs']]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
 
     @update.setter
-    def update(self, value: Optional['HostnamectlOptsArgs']):
+    def update(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['TarOptsArgs']]]):
         pulumi.set(self, "update", value)
 
 
-class Hostnamectl(pulumi.ComponentResource):
+class Tar(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[pulumi.InputType['HostnamectlOptsArgs']] = None,
-                 delete: Optional[pulumi.InputType['HostnamectlOptsArgs']] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TarOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TarOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[pulumi.InputType['HostnamectlOptsArgs']] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TarOptsArgs']]]] = None,
                  __props__=None):
         """
-        Abstraction over the `hostnamectl` utility on a remote system.
+        Abstraction over the `tar` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
-        :param pulumi.InputType['HostnamectlOptsArgs'] create: The command to run on create.
-        :param pulumi.InputType['HostnamectlOptsArgs'] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TarOptsArgs']]] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TarOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param pulumi.InputType['HostnamectlOptsArgs'] update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TarOptsArgs']]] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: HostnamectlArgs,
+                 args: TarArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Abstraction over the `hostnamectl` utility on a remote system.
+        Abstraction over the `tar` utility on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param HostnamectlArgs args: The arguments to use to populate this resource's properties.
+        :param TarArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(HostnamectlArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(TarArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[pulumi.InputType['HostnamectlOptsArgs']] = None,
-                 delete: Optional[pulumi.InputType['HostnamectlOptsArgs']] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TarOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TarOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[pulumi.InputType['HostnamectlOptsArgs']] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TarOptsArgs']]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = HostnamectlArgs.__new__(HostnamectlArgs)
+            __props__ = TarArgs.__new__(TarArgs)
 
             __props__.__dict__["binary_path"] = binary_path
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
             __props__.__dict__["create"] = create
             __props__.__dict__["delete"] = delete
             __props__.__dict__["environment"] = environment
             __props__.__dict__["stdin"] = stdin
             __props__.__dict__["triggers"] = triggers
             __props__.__dict__["update"] = update
             __props__.__dict__["command"] = None
             __props__.__dict__["stderr"] = None
             __props__.__dict__["stdout"] = None
-        super(Hostnamectl, __self__).__init__(
-            'kubernetes-the-hard-way:tools:Hostnamectl',
+        super(Tar, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Tar',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter(name="binaryPath")
@@ -278,23 +277,23 @@
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter
-    def create(self) -> pulumi.Output[Optional['outputs.HostnamectlOpts']]:
+    def create(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @property
     @pulumi.getter
-    def delete(self) -> pulumi.Output[Optional['outputs.HostnamectlOpts']]:
+    def delete(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
@@ -336,15 +335,15 @@
         """
         TODO
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
-    def update(self) -> pulumi.Output[Optional['outputs.HostnamectlOpts']]:
+    def update(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/mkdir.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/mkdir.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,32 +15,32 @@
 __all__ = ['MkdirArgs', 'Mkdir']
 
 @pulumi.input_type
 class MkdirArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 create: Optional['MkdirOptsArgs'] = None,
-                 delete: Optional['MkdirOptsArgs'] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional['MkdirOptsArgs'] = None):
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]] = None):
         """
         The set of arguments for constructing a Mkdir resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param 'MkdirOptsArgs' create: The command to run on create.
-        :param 'MkdirOptsArgs' delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param 'MkdirOptsArgs' update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
@@ -79,36 +79,36 @@
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def create(self) -> Optional['MkdirOptsArgs']:
+    def create(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @create.setter
-    def create(self, value: Optional['MkdirOptsArgs']):
+    def create(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]]):
         pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def delete(self) -> Optional['MkdirOptsArgs']:
+    def delete(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
     @delete.setter
-    def delete(self, value: Optional['MkdirOptsArgs']):
+    def delete(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]]):
         pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
     def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Environment variables
@@ -141,57 +141,57 @@
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
     @property
     @pulumi.getter
-    def update(self) -> Optional['MkdirOptsArgs']:
+    def update(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
 
     @update.setter
-    def update(self, value: Optional['MkdirOptsArgs']):
+    def update(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MkdirOptsArgs']]]):
         pulumi.set(self, "update", value)
 
 
 class Mkdir(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[pulumi.InputType['MkdirOptsArgs']] = None,
-                 delete: Optional[pulumi.InputType['MkdirOptsArgs']] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[pulumi.InputType['MkdirOptsArgs']] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]]] = None,
                  __props__=None):
         """
         Abstraction over the `mkdir` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
-        :param pulumi.InputType['MkdirOptsArgs'] create: The command to run on create.
-        :param pulumi.InputType['MkdirOptsArgs'] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param pulumi.InputType['MkdirOptsArgs'] update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
@@ -214,20 +214,20 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[pulumi.InputType['MkdirOptsArgs']] = None,
-                 delete: Optional[pulumi.InputType['MkdirOptsArgs']] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[pulumi.InputType['MkdirOptsArgs']] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MkdirOptsArgs']]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
@@ -277,23 +277,23 @@
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter
-    def create(self) -> pulumi.Output[Optional['outputs.MkdirOpts']]:
+    def create(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @property
     @pulumi.getter
-    def delete(self) -> pulumi.Output[Optional['outputs.MkdirOpts']]:
+    def delete(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
@@ -335,15 +335,15 @@
         """
         TODO
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
-    def update(self) -> pulumi.Output[Optional['outputs.MkdirOpts']]:
+    def update(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/mktemp.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/mktemp.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,32 +15,32 @@
 __all__ = ['MktempArgs', 'Mktemp']
 
 @pulumi.input_type
 class MktempArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 create: Optional['MktempOptsArgs'] = None,
-                 delete: Optional['MktempOptsArgs'] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional['MktempOptsArgs'] = None):
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]] = None):
         """
         The set of arguments for constructing a Mktemp resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param 'MktempOptsArgs' create: The command to run on create.
-        :param 'MktempOptsArgs' delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param 'MktempOptsArgs' update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
@@ -79,36 +79,36 @@
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def create(self) -> Optional['MktempOptsArgs']:
+    def create(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @create.setter
-    def create(self, value: Optional['MktempOptsArgs']):
+    def create(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]]):
         pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def delete(self) -> Optional['MktempOptsArgs']:
+    def delete(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
     @delete.setter
-    def delete(self, value: Optional['MktempOptsArgs']):
+    def delete(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]]):
         pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
     def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Environment variables
@@ -141,57 +141,57 @@
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
     @property
     @pulumi.getter
-    def update(self) -> Optional['MktempOptsArgs']:
+    def update(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
 
     @update.setter
-    def update(self, value: Optional['MktempOptsArgs']):
+    def update(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['MktempOptsArgs']]]):
         pulumi.set(self, "update", value)
 
 
 class Mktemp(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[pulumi.InputType['MktempOptsArgs']] = None,
-                 delete: Optional[pulumi.InputType['MktempOptsArgs']] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[pulumi.InputType['MktempOptsArgs']] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]]] = None,
                  __props__=None):
         """
         Abstraction over the `mktemp` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
-        :param pulumi.InputType['MktempOptsArgs'] create: The command to run on create.
-        :param pulumi.InputType['MktempOptsArgs'] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param pulumi.InputType['MktempOptsArgs'] update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
@@ -214,20 +214,20 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[pulumi.InputType['MktempOptsArgs']] = None,
-                 delete: Optional[pulumi.InputType['MktempOptsArgs']] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[pulumi.InputType['MktempOptsArgs']] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['MktempOptsArgs']]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
@@ -277,23 +277,23 @@
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter
-    def create(self) -> pulumi.Output[Optional['outputs.MktempOpts']]:
+    def create(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @property
     @pulumi.getter
-    def delete(self) -> pulumi.Output[Optional['outputs.MktempOpts']]:
+    def delete(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
@@ -335,15 +335,15 @@
         """
         TODO
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
-    def update(self) -> pulumi.Output[Optional['outputs.MktempOpts']]:
+    def update(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/mv.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,42 +5,43 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
+from ._enums import *
 from ._inputs import *
 import pulumi_command
 
-__all__ = ['MvArgs', 'Mv']
+__all__ = ['HostnamectlArgs', 'Hostnamectl']
 
 @pulumi.input_type
-class MvArgs:
+class HostnamectlArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 create: Optional['MvOptsArgs'] = None,
-                 delete: Optional['MvOptsArgs'] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input['HostnamectlOptsArgs']]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input['HostnamectlOptsArgs']]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional['MvOptsArgs'] = None):
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input['HostnamectlOptsArgs']]] = None):
         """
-        The set of arguments for constructing a Mv resource.
+        The set of arguments for constructing a Hostnamectl resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param 'MvOptsArgs' create: The command to run on create.
-        :param 'MvOptsArgs' delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input['HostnamectlOptsArgs']] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input['HostnamectlOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param 'MvOptsArgs' update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input['HostnamectlOptsArgs']] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
@@ -79,36 +80,36 @@
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def create(self) -> Optional['MvOptsArgs']:
+    def create(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['HostnamectlOptsArgs']]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @create.setter
-    def create(self, value: Optional['MvOptsArgs']):
+    def create(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['HostnamectlOptsArgs']]]):
         pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def delete(self) -> Optional['MvOptsArgs']:
+    def delete(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['HostnamectlOptsArgs']]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
     @delete.setter
-    def delete(self, value: Optional['MvOptsArgs']):
+    def delete(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['HostnamectlOptsArgs']]]):
         pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
     def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Environment variables
@@ -141,119 +142,119 @@
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
     @property
     @pulumi.getter
-    def update(self) -> Optional['MvOptsArgs']:
+    def update(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['HostnamectlOptsArgs']]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
 
     @update.setter
-    def update(self, value: Optional['MvOptsArgs']):
+    def update(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['HostnamectlOptsArgs']]]):
         pulumi.set(self, "update", value)
 
 
-class Mv(pulumi.ComponentResource):
+class Hostnamectl(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[pulumi.InputType['MvOptsArgs']] = None,
-                 delete: Optional[pulumi.InputType['MvOptsArgs']] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['HostnamectlOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['HostnamectlOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[pulumi.InputType['MvOptsArgs']] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['HostnamectlOptsArgs']]]] = None,
                  __props__=None):
         """
-        Abstraction over the `mv` utility on a remote system.
+        Abstraction over the `hostnamectl` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
-        :param pulumi.InputType['MvOptsArgs'] create: The command to run on create.
-        :param pulumi.InputType['MvOptsArgs'] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['HostnamectlOptsArgs']]] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['HostnamectlOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param pulumi.InputType['MvOptsArgs'] update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['HostnamectlOptsArgs']]] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: MvArgs,
+                 args: HostnamectlArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Abstraction over the `mv` utility on a remote system.
+        Abstraction over the `hostnamectl` utility on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param MvArgs args: The arguments to use to populate this resource's properties.
+        :param HostnamectlArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(MvArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(HostnamectlArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[pulumi.InputType['MvOptsArgs']] = None,
-                 delete: Optional[pulumi.InputType['MvOptsArgs']] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['HostnamectlOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['HostnamectlOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[pulumi.InputType['MvOptsArgs']] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['HostnamectlOptsArgs']]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = MvArgs.__new__(MvArgs)
+            __props__ = HostnamectlArgs.__new__(HostnamectlArgs)
 
             __props__.__dict__["binary_path"] = binary_path
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
             __props__.__dict__["create"] = create
             __props__.__dict__["delete"] = delete
             __props__.__dict__["environment"] = environment
             __props__.__dict__["stdin"] = stdin
             __props__.__dict__["triggers"] = triggers
             __props__.__dict__["update"] = update
             __props__.__dict__["command"] = None
             __props__.__dict__["stderr"] = None
             __props__.__dict__["stdout"] = None
-        super(Mv, __self__).__init__(
-            'kubernetes-the-hard-way:tools:Mv',
+        super(Hostnamectl, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Hostnamectl',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter(name="binaryPath")
@@ -277,23 +278,23 @@
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter
-    def create(self) -> pulumi.Output[Optional['outputs.MvOpts']]:
+    def create(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @property
     @pulumi.getter
-    def delete(self) -> pulumi.Output[Optional['outputs.MvOpts']]:
+    def delete(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
@@ -335,15 +336,15 @@
         """
         TODO
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
-    def update(self) -> pulumi.Output[Optional['outputs.MvOpts']]:
+    def update(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/rm.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/rm.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,32 +15,32 @@
 __all__ = ['RmArgs', 'Rm']
 
 @pulumi.input_type
 class RmArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 create: Optional['RmOptsArgs'] = None,
-                 delete: Optional['RmOptsArgs'] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input['RmOptsArgs']]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input['RmOptsArgs']]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional['RmOptsArgs'] = None):
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input['RmOptsArgs']]] = None):
         """
         The set of arguments for constructing a Rm resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param 'RmOptsArgs' create: The command to run on create.
-        :param 'RmOptsArgs' delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input['RmOptsArgs']] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input['RmOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param 'RmOptsArgs' update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input['RmOptsArgs']] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
@@ -79,36 +79,36 @@
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def create(self) -> Optional['RmOptsArgs']:
+    def create(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['RmOptsArgs']]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @create.setter
-    def create(self, value: Optional['RmOptsArgs']):
+    def create(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['RmOptsArgs']]]):
         pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def delete(self) -> Optional['RmOptsArgs']:
+    def delete(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['RmOptsArgs']]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
     @delete.setter
-    def delete(self, value: Optional['RmOptsArgs']):
+    def delete(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['RmOptsArgs']]]):
         pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
     def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Environment variables
@@ -141,57 +141,57 @@
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
     @property
     @pulumi.getter
-    def update(self) -> Optional['RmOptsArgs']:
+    def update(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['RmOptsArgs']]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
 
     @update.setter
-    def update(self, value: Optional['RmOptsArgs']):
+    def update(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['RmOptsArgs']]]):
         pulumi.set(self, "update", value)
 
 
 class Rm(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[pulumi.InputType['RmOptsArgs']] = None,
-                 delete: Optional[pulumi.InputType['RmOptsArgs']] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['RmOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['RmOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[pulumi.InputType['RmOptsArgs']] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['RmOptsArgs']]]] = None,
                  __props__=None):
         """
         Abstraction over the `rm` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
-        :param pulumi.InputType['RmOptsArgs'] create: The command to run on create.
-        :param pulumi.InputType['RmOptsArgs'] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['RmOptsArgs']]] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['RmOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param pulumi.InputType['RmOptsArgs'] update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['RmOptsArgs']]] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
@@ -214,20 +214,20 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[pulumi.InputType['RmOptsArgs']] = None,
-                 delete: Optional[pulumi.InputType['RmOptsArgs']] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['RmOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['RmOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[pulumi.InputType['RmOptsArgs']] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['RmOptsArgs']]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
@@ -277,23 +277,23 @@
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter
-    def create(self) -> pulumi.Output[Optional['outputs.RmOpts']]:
+    def create(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @property
     @pulumi.getter
-    def delete(self) -> pulumi.Output[Optional['outputs.RmOpts']]:
+    def delete(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
@@ -335,15 +335,15 @@
         """
         TODO
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
-    def update(self) -> pulumi.Output[Optional['outputs.RmOpts']]:
+    def update(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/sed.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/tee.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,42 +5,43 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
+from ._enums import *
 from ._inputs import *
 import pulumi_command
 
-__all__ = ['SedArgs', 'Sed']
+__all__ = ['TeeArgs', 'Tee']
 
 @pulumi.input_type
-class SedArgs:
+class TeeArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 create: Optional['SedOptsArgs'] = None,
-                 delete: Optional['SedOptsArgs'] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional['SedOptsArgs'] = None):
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]] = None):
         """
-        The set of arguments for constructing a Sed resource.
+        The set of arguments for constructing a Tee resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param 'SedOptsArgs' create: The command to run on create.
-        :param 'SedOptsArgs' delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param 'SedOptsArgs' update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
@@ -79,36 +80,36 @@
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def create(self) -> Optional['SedOptsArgs']:
+    def create(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @create.setter
-    def create(self, value: Optional['SedOptsArgs']):
+    def create(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]):
         pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def delete(self) -> Optional['SedOptsArgs']:
+    def delete(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
     @delete.setter
-    def delete(self, value: Optional['SedOptsArgs']):
+    def delete(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]):
         pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
     def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Environment variables
@@ -141,119 +142,119 @@
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
     @property
     @pulumi.getter
-    def update(self) -> Optional['SedOptsArgs']:
+    def update(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
 
     @update.setter
-    def update(self, value: Optional['SedOptsArgs']):
+    def update(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['TeeOptsArgs']]]):
         pulumi.set(self, "update", value)
 
 
-class Sed(pulumi.ComponentResource):
+class Tee(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[pulumi.InputType['SedOptsArgs']] = None,
-                 delete: Optional[pulumi.InputType['SedOptsArgs']] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[pulumi.InputType['SedOptsArgs']] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
                  __props__=None):
         """
-        Abstraction over the `sed` utility on a remote system.
+        Abstraction over the `rm` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
-        :param pulumi.InputType['SedOptsArgs'] create: The command to run on create.
-        :param pulumi.InputType['SedOptsArgs'] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param pulumi.InputType['SedOptsArgs'] update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: SedArgs,
+                 args: TeeArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Abstraction over the `sed` utility on a remote system.
+        Abstraction over the `rm` utility on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param SedArgs args: The arguments to use to populate this resource's properties.
+        :param TeeArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(SedArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(TeeArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[pulumi.InputType['SedOptsArgs']] = None,
-                 delete: Optional[pulumi.InputType['SedOptsArgs']] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[pulumi.InputType['SedOptsArgs']] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['TeeOptsArgs']]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = SedArgs.__new__(SedArgs)
+            __props__ = TeeArgs.__new__(TeeArgs)
 
             __props__.__dict__["binary_path"] = binary_path
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
             __props__.__dict__["create"] = create
             __props__.__dict__["delete"] = delete
             __props__.__dict__["environment"] = environment
             __props__.__dict__["stdin"] = stdin
             __props__.__dict__["triggers"] = triggers
             __props__.__dict__["update"] = update
             __props__.__dict__["command"] = None
             __props__.__dict__["stderr"] = None
             __props__.__dict__["stdout"] = None
-        super(Sed, __self__).__init__(
-            'kubernetes-the-hard-way:tools:Sed',
+        super(Tee, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Tee',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter(name="binaryPath")
@@ -277,23 +278,23 @@
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter
-    def create(self) -> pulumi.Output[Optional['outputs.SedOpts']]:
+    def create(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @property
     @pulumi.getter
-    def delete(self) -> pulumi.Output[Optional['outputs.SedOpts']]:
+    def delete(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
@@ -335,15 +336,15 @@
         """
         TODO
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
-    def update(self) -> pulumi.Output[Optional['outputs.SedOpts']]:
+    def update(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/systemctl.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/wget.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,43 +5,42 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
-from ._enums import *
 from ._inputs import *
 import pulumi_command
 
-__all__ = ['SystemctlArgs', 'Systemctl']
+__all__ = ['WgetArgs', 'Wget']
 
 @pulumi.input_type
-class SystemctlArgs:
+class WgetArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 create: Optional['SystemctlOptsArgs'] = None,
-                 delete: Optional['SystemctlOptsArgs'] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional['SystemctlOptsArgs'] = None):
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]] = None):
         """
-        The set of arguments for constructing a Systemctl resource.
+        The set of arguments for constructing a Wget resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param 'SystemctlOptsArgs' create: The command to run on create.
-        :param 'SystemctlOptsArgs' delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param 'SystemctlOptsArgs' update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
@@ -80,36 +79,36 @@
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def create(self) -> Optional['SystemctlOptsArgs']:
+    def create(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @create.setter
-    def create(self, value: Optional['SystemctlOptsArgs']):
+    def create(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]]):
         pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def delete(self) -> Optional['SystemctlOptsArgs']:
+    def delete(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
     @delete.setter
-    def delete(self, value: Optional['SystemctlOptsArgs']):
+    def delete(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]]):
         pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
     def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Environment variables
@@ -142,119 +141,119 @@
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
     @property
     @pulumi.getter
-    def update(self) -> Optional['SystemctlOptsArgs']:
+    def update(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
 
     @update.setter
-    def update(self, value: Optional['SystemctlOptsArgs']):
+    def update(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['WgetOptsArgs']]]):
         pulumi.set(self, "update", value)
 
 
-class Systemctl(pulumi.ComponentResource):
+class Wget(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[pulumi.InputType['SystemctlOptsArgs']] = None,
-                 delete: Optional[pulumi.InputType['SystemctlOptsArgs']] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[pulumi.InputType['SystemctlOptsArgs']] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]]] = None,
                  __props__=None):
         """
-        Abstraction over the `systemctl` utility on a remote system.
+        Abstraction over the `wget` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
-        :param pulumi.InputType['SystemctlOptsArgs'] create: The command to run on create.
-        :param pulumi.InputType['SystemctlOptsArgs'] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param pulumi.InputType['SystemctlOptsArgs'] update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: SystemctlArgs,
+                 args: WgetArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Abstraction over the `systemctl` utility on a remote system.
+        Abstraction over the `wget` utility on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param SystemctlArgs args: The arguments to use to populate this resource's properties.
+        :param WgetArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(SystemctlArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(WgetArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[pulumi.InputType['SystemctlOptsArgs']] = None,
-                 delete: Optional[pulumi.InputType['SystemctlOptsArgs']] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[pulumi.InputType['SystemctlOptsArgs']] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['WgetOptsArgs']]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = SystemctlArgs.__new__(SystemctlArgs)
+            __props__ = WgetArgs.__new__(WgetArgs)
 
             __props__.__dict__["binary_path"] = binary_path
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
             __props__.__dict__["create"] = create
             __props__.__dict__["delete"] = delete
             __props__.__dict__["environment"] = environment
             __props__.__dict__["stdin"] = stdin
             __props__.__dict__["triggers"] = triggers
             __props__.__dict__["update"] = update
             __props__.__dict__["command"] = None
             __props__.__dict__["stderr"] = None
             __props__.__dict__["stdout"] = None
-        super(Systemctl, __self__).__init__(
-            'kubernetes-the-hard-way:tools:Systemctl',
+        super(Wget, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Wget',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter(name="binaryPath")
@@ -278,23 +277,23 @@
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter
-    def create(self) -> pulumi.Output[Optional['outputs.SystemctlOpts']]:
+    def create(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @property
     @pulumi.getter
-    def delete(self) -> pulumi.Output[Optional['outputs.SystemctlOpts']]:
+    def delete(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
@@ -336,15 +335,15 @@
         """
         TODO
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
-    def update(self) -> pulumi.Output[Optional['outputs.SystemctlOpts']]:
+    def update(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/tar.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/curl.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,42 +5,43 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
+from ._enums import *
 from ._inputs import *
 import pulumi_command
 
-__all__ = ['TarArgs', 'Tar']
+__all__ = ['CurlArgs', 'Curl']
 
 @pulumi.input_type
-class TarArgs:
+class CurlArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 create: Optional['TarOptsArgs'] = None,
-                 delete: Optional['TarOptsArgs'] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input['CurlOptsArgs']]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input['CurlOptsArgs']]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional['TarOptsArgs'] = None):
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input['CurlOptsArgs']]] = None):
         """
-        The set of arguments for constructing a Tar resource.
+        The set of arguments for constructing a Curl resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param 'TarOptsArgs' create: The command to run on create.
-        :param 'TarOptsArgs' delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input['CurlOptsArgs']] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input['CurlOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param 'TarOptsArgs' update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input['CurlOptsArgs']] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
@@ -79,36 +80,36 @@
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def create(self) -> Optional['TarOptsArgs']:
+    def create(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['CurlOptsArgs']]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @create.setter
-    def create(self, value: Optional['TarOptsArgs']):
+    def create(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['CurlOptsArgs']]]):
         pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def delete(self) -> Optional['TarOptsArgs']:
+    def delete(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['CurlOptsArgs']]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
     @delete.setter
-    def delete(self, value: Optional['TarOptsArgs']):
+    def delete(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['CurlOptsArgs']]]):
         pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
     def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Environment variables
@@ -141,119 +142,119 @@
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
     @property
     @pulumi.getter
-    def update(self) -> Optional['TarOptsArgs']:
+    def update(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['CurlOptsArgs']]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
 
     @update.setter
-    def update(self, value: Optional['TarOptsArgs']):
+    def update(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['CurlOptsArgs']]]):
         pulumi.set(self, "update", value)
 
 
-class Tar(pulumi.ComponentResource):
+class Curl(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[pulumi.InputType['TarOptsArgs']] = None,
-                 delete: Optional[pulumi.InputType['TarOptsArgs']] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['CurlOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['CurlOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[pulumi.InputType['TarOptsArgs']] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['CurlOptsArgs']]]] = None,
                  __props__=None):
         """
-        Abstraction over the `tar` utility on a remote system.
+        Abstraction over the `curl` utility on a remote system. Transfer a URL.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
-        :param pulumi.InputType['TarOptsArgs'] create: The command to run on create.
-        :param pulumi.InputType['TarOptsArgs'] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['CurlOptsArgs']]] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['CurlOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param pulumi.InputType['TarOptsArgs'] update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['CurlOptsArgs']]] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: TarArgs,
+                 args: CurlArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Abstraction over the `tar` utility on a remote system.
+        Abstraction over the `curl` utility on a remote system. Transfer a URL.
 
         :param str resource_name: The name of the resource.
-        :param TarArgs args: The arguments to use to populate this resource's properties.
+        :param CurlArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(TarArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(CurlArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[pulumi.InputType['TarOptsArgs']] = None,
-                 delete: Optional[pulumi.InputType['TarOptsArgs']] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['CurlOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['CurlOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[pulumi.InputType['TarOptsArgs']] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['CurlOptsArgs']]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = TarArgs.__new__(TarArgs)
+            __props__ = CurlArgs.__new__(CurlArgs)
 
             __props__.__dict__["binary_path"] = binary_path
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
             __props__.__dict__["create"] = create
             __props__.__dict__["delete"] = delete
             __props__.__dict__["environment"] = environment
             __props__.__dict__["stdin"] = stdin
             __props__.__dict__["triggers"] = triggers
             __props__.__dict__["update"] = update
             __props__.__dict__["command"] = None
             __props__.__dict__["stderr"] = None
             __props__.__dict__["stdout"] = None
-        super(Tar, __self__).__init__(
-            'kubernetes-the-hard-way:tools:Tar',
+        super(Curl, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Curl',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter(name="binaryPath")
@@ -277,23 +278,23 @@
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter
-    def create(self) -> pulumi.Output[Optional['outputs.TarOpts']]:
+    def create(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @property
     @pulumi.getter
-    def delete(self) -> pulumi.Output[Optional['outputs.TarOpts']]:
+    def delete(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
@@ -335,15 +336,15 @@
         """
         TODO
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
-    def update(self) -> pulumi.Output[Optional['outputs.TarOpts']]:
+    def update(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/tee.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/sed.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,43 +5,42 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
-from ._enums import *
 from ._inputs import *
 import pulumi_command
 
-__all__ = ['TeeArgs', 'Tee']
+__all__ = ['SedArgs', 'Sed']
 
 @pulumi.input_type
-class TeeArgs:
+class SedArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 create: Optional['TeeOptsArgs'] = None,
-                 delete: Optional['TeeOptsArgs'] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input['SedOptsArgs']]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input['SedOptsArgs']]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional['TeeOptsArgs'] = None):
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input['SedOptsArgs']]] = None):
         """
-        The set of arguments for constructing a Tee resource.
+        The set of arguments for constructing a Sed resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param 'TeeOptsArgs' create: The command to run on create.
-        :param 'TeeOptsArgs' delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input['SedOptsArgs']] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input['SedOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param 'TeeOptsArgs' update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input['SedOptsArgs']] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
@@ -80,36 +79,36 @@
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def create(self) -> Optional['TeeOptsArgs']:
+    def create(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['SedOptsArgs']]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @create.setter
-    def create(self, value: Optional['TeeOptsArgs']):
+    def create(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['SedOptsArgs']]]):
         pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def delete(self) -> Optional['TeeOptsArgs']:
+    def delete(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['SedOptsArgs']]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
     @delete.setter
-    def delete(self, value: Optional['TeeOptsArgs']):
+    def delete(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['SedOptsArgs']]]):
         pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
     def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Environment variables
@@ -142,119 +141,119 @@
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
     @property
     @pulumi.getter
-    def update(self) -> Optional['TeeOptsArgs']:
+    def update(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['SedOptsArgs']]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
 
     @update.setter
-    def update(self, value: Optional['TeeOptsArgs']):
+    def update(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['SedOptsArgs']]]):
         pulumi.set(self, "update", value)
 
 
-class Tee(pulumi.ComponentResource):
+class Sed(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[pulumi.InputType['TeeOptsArgs']] = None,
-                 delete: Optional[pulumi.InputType['TeeOptsArgs']] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['SedOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['SedOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[pulumi.InputType['TeeOptsArgs']] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['SedOptsArgs']]]] = None,
                  __props__=None):
         """
-        Abstraction over the `rm` utility on a remote system.
+        Abstraction over the `sed` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
-        :param pulumi.InputType['TeeOptsArgs'] create: The command to run on create.
-        :param pulumi.InputType['TeeOptsArgs'] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['SedOptsArgs']]] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['SedOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param pulumi.InputType['TeeOptsArgs'] update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['SedOptsArgs']]] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: TeeArgs,
+                 args: SedArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Abstraction over the `rm` utility on a remote system.
+        Abstraction over the `sed` utility on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param TeeArgs args: The arguments to use to populate this resource's properties.
+        :param SedArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(TeeArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(SedArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[pulumi.InputType['TeeOptsArgs']] = None,
-                 delete: Optional[pulumi.InputType['TeeOptsArgs']] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['SedOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['SedOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[pulumi.InputType['TeeOptsArgs']] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['SedOptsArgs']]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = TeeArgs.__new__(TeeArgs)
+            __props__ = SedArgs.__new__(SedArgs)
 
             __props__.__dict__["binary_path"] = binary_path
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
             __props__.__dict__["create"] = create
             __props__.__dict__["delete"] = delete
             __props__.__dict__["environment"] = environment
             __props__.__dict__["stdin"] = stdin
             __props__.__dict__["triggers"] = triggers
             __props__.__dict__["update"] = update
             __props__.__dict__["command"] = None
             __props__.__dict__["stderr"] = None
             __props__.__dict__["stdout"] = None
-        super(Tee, __self__).__init__(
-            'kubernetes-the-hard-way:tools:Tee',
+        super(Sed, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Sed',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter(name="binaryPath")
@@ -278,23 +277,23 @@
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter
-    def create(self) -> pulumi.Output[Optional['outputs.TeeOpts']]:
+    def create(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @property
     @pulumi.getter
-    def delete(self) -> pulumi.Output[Optional['outputs.TeeOpts']]:
+    def delete(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
@@ -336,15 +335,15 @@
         """
         TODO
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
-    def update(self) -> pulumi.Output[Optional['outputs.TeeOpts']]:
+    def update(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way/tools/wget.py` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way/tools/systemctl.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,42 +5,43 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from . import outputs
+from ._enums import *
 from ._inputs import *
 import pulumi_command
 
-__all__ = ['WgetArgs', 'Wget']
+__all__ = ['SystemctlArgs', 'Systemctl']
 
 @pulumi.input_type
-class WgetArgs:
+class SystemctlArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 create: Optional['WgetOptsArgs'] = None,
-                 delete: Optional['WgetOptsArgs'] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input['SystemctlOptsArgs']]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input['SystemctlOptsArgs']]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional['WgetOptsArgs'] = None):
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input['SystemctlOptsArgs']]] = None):
         """
-        The set of arguments for constructing a Wget resource.
+        The set of arguments for constructing a Systemctl resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param 'WgetOptsArgs' create: The command to run on create.
-        :param 'WgetOptsArgs' delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input['SystemctlOptsArgs']] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input['SystemctlOptsArgs']] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param 'WgetOptsArgs' update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input['SystemctlOptsArgs']] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
@@ -79,36 +80,36 @@
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def create(self) -> Optional['WgetOptsArgs']:
+    def create(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['SystemctlOptsArgs']]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @create.setter
-    def create(self, value: Optional['WgetOptsArgs']):
+    def create(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['SystemctlOptsArgs']]]):
         pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def delete(self) -> Optional['WgetOptsArgs']:
+    def delete(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['SystemctlOptsArgs']]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
     @delete.setter
-    def delete(self, value: Optional['WgetOptsArgs']):
+    def delete(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['SystemctlOptsArgs']]]):
         pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
     def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Environment variables
@@ -141,119 +142,119 @@
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
     @property
     @pulumi.getter
-    def update(self) -> Optional['WgetOptsArgs']:
+    def update(self) -> Optional[Union[pulumi.Input[str], pulumi.Input['SystemctlOptsArgs']]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
 
     @update.setter
-    def update(self, value: Optional['WgetOptsArgs']):
+    def update(self, value: Optional[Union[pulumi.Input[str], pulumi.Input['SystemctlOptsArgs']]]):
         pulumi.set(self, "update", value)
 
 
-class Wget(pulumi.ComponentResource):
+class Systemctl(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[pulumi.InputType['WgetOptsArgs']] = None,
-                 delete: Optional[pulumi.InputType['WgetOptsArgs']] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['SystemctlOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['SystemctlOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[pulumi.InputType['WgetOptsArgs']] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['SystemctlOptsArgs']]]] = None,
                  __props__=None):
         """
-        Abstraction over the `wget` utility on a remote system.
+        Abstraction over the `systemctl` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
-        :param pulumi.InputType['WgetOptsArgs'] create: The command to run on create.
-        :param pulumi.InputType['WgetOptsArgs'] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['SystemctlOptsArgs']]] create: The command to run on create.
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['SystemctlOptsArgs']]] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
                and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
                Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param pulumi.InputType['WgetOptsArgs'] update: The command to run on update, if empty, create will 
+        :param Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['SystemctlOptsArgs']]] update: The command to run on update, if empty, create will 
                run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
                are set to the stdout and stderr properties of the Command resource from previous 
                create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: WgetArgs,
+                 args: SystemctlArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Abstraction over the `wget` utility on a remote system.
+        Abstraction over the `systemctl` utility on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param WgetArgs args: The arguments to use to populate this resource's properties.
+        :param SystemctlArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(WgetArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(SystemctlArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 create: Optional[pulumi.InputType['WgetOptsArgs']] = None,
-                 delete: Optional[pulumi.InputType['WgetOptsArgs']] = None,
+                 create: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['SystemctlOptsArgs']]]] = None,
+                 delete: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['SystemctlOptsArgs']]]] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 update: Optional[pulumi.InputType['WgetOptsArgs']] = None,
+                 update: Optional[Union[pulumi.Input[str], pulumi.Input[pulumi.InputType['SystemctlOptsArgs']]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = WgetArgs.__new__(WgetArgs)
+            __props__ = SystemctlArgs.__new__(SystemctlArgs)
 
             __props__.__dict__["binary_path"] = binary_path
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
             __props__.__dict__["create"] = create
             __props__.__dict__["delete"] = delete
             __props__.__dict__["environment"] = environment
             __props__.__dict__["stdin"] = stdin
             __props__.__dict__["triggers"] = triggers
             __props__.__dict__["update"] = update
             __props__.__dict__["command"] = None
             __props__.__dict__["stderr"] = None
             __props__.__dict__["stdout"] = None
-        super(Wget, __self__).__init__(
-            'kubernetes-the-hard-way:tools:Wget',
+        super(Systemctl, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Systemctl',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter(name="binaryPath")
@@ -277,23 +278,23 @@
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter
-    def create(self) -> pulumi.Output[Optional['outputs.WgetOpts']]:
+    def create(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on create.
         """
         return pulumi.get(self, "create")
 
     @property
     @pulumi.getter
-    def delete(self) -> pulumi.Output[Optional['outputs.WgetOpts']]:
+    def delete(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
         and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
         Command resource from previous create or update steps.
         """
         return pulumi.get(self, "delete")
 
@@ -335,15 +336,15 @@
         """
         TODO
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
-    def update(self) -> pulumi.Output[Optional['outputs.WgetOpts']]:
+    def update(self) -> pulumi.Output[Optional[Any]]:
         """
         The command to run on update, if empty, create will 
         run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
         are set to the stdout and stderr properties of the Command resource from previous 
         create or update steps.
         """
         return pulumi.get(self, "update")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.19a1713682959
+Version: 0.0.19a1713732126
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.19a1713682959/pyproject.toml` & `pulumi_kubernetes_the_hard_way-0.0.19a1713732126/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kubernetes_the_hard_way"
   description = "A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way"
   dependencies = ["parver>=0.2.1", "pulumi>=3.91.1,<4.0.0", "pulumi-command>=0.10.0,<1.0.0", "pulumi-kubernetes>=4.11.0,<5.0.0", "pulumi-random>=4.16.1,<5.0.0", "pulumi-tls>=5.0.2,<6.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "command", "tls", "kubernetes", "category/utility", "kind/component"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.19a1713682959"
+  version = "0.0.19a1713732126"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```


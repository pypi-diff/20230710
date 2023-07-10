# Comparing `tmp/network-config-analyzer-1.9.2.tar.gz` & `tmp/network-config-analyzer-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "network-config-analyzer-1.9.2.tar", last modified: Tue Feb 14 14:47:50 2023, max compression
+gzip compressed data, was "network-config-analyzer-1.9.3.tar", last modified: Mon Jul 10 14:10:26 2023, max compression
```

## Comparing `network-config-analyzer-1.9.2.tar` & `network-config-analyzer-1.9.3.tar`

### file list

```diff
@@ -1,93 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:47:50.634441 network-config-analyzer-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-02-14 14:47:50.634441 network-config-analyzer-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:47:50.622441 network-config-analyzer-1.9.2/nca/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:47:50.626441 network-config-analyzer-1.9.2/nca/CoreDS/
--rw-r--r--   0 runner    (1001) docker     (123)    41525 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/CoreDS/CanonicalHyperCubeSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    13675 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/CoreDS/CanonicalIntervalSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    23906 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/CoreDS/ConnectionSet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/CoreDS/DimensionsManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/CoreDS/ICMPDataSet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/CoreDS/MethodSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/CoreDS/MinDFA.py
--rw-r--r--   0 runner    (1001) docker     (123)    23354 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/CoreDS/Peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/CoreDS/PortSet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/CoreDS/ProtocolNameResolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    15023 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/CoreDS/TcpLikeProperties.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/CoreDS/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:47:50.626441 network-config-analyzer-1.9.2/nca/FWRules/
--rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/FWRules/ClusterInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    12856 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/FWRules/ConnectivityGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    22273 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/FWRules/FWRule.py
--rw-r--r--   0 runner    (1001) docker     (123)    41302 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/FWRules/MinimizeFWRules.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/FWRules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:47:50.626441 network-config-analyzer-1.9.2/nca/FileScanners/
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/FileScanners/DirScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/FileScanners/GenericTreeScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/FileScanners/GitScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/FileScanners/HelmScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/FileScanners/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:47:50.626441 network-config-analyzer-1.9.2/nca/NetworkConfig/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:47:50.622441 network-config-analyzer-1.9.2/nca/NetworkConfig/LiveSim/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:47:50.626441 network-config-analyzer-1.9.2/nca/NetworkConfig/LiveSim/dns/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/NetworkConfig/LiveSim/dns/dns_pods.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:47:50.626441 network-config-analyzer-1.9.2/nca/NetworkConfig/LiveSim/ingress_controller/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/NetworkConfig/LiveSim/ingress_controller/ingress_controller.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:47:50.630441 network-config-analyzer-1.9.2/nca/NetworkConfig/LiveSim/istio_gateway/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/NetworkConfig/LiveSim/istio_gateway/istio_custom_gateway.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/NetworkConfig/LiveSim/istio_gateway/istio_gateway.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/NetworkConfig/NetworkConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    86879 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/NetworkConfig/NetworkConfigQuery.py
--rw-r--r--   0 runner    (1001) docker     (123)    12417 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/NetworkConfig/NetworkConfigQueryRunner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/NetworkConfig/NetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15477 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/NetworkConfig/PeerContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/NetworkConfig/PoliciesFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)    17002 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/NetworkConfig/QueryOutputHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    25842 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/NetworkConfig/ResourcesHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    15342 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/NetworkConfig/TopologyObjectsFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/NetworkConfig/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:47:50.630441 network-config-analyzer-1.9.2/nca/Parsers/
--rw-r--r--   0 runner    (1001) docker     (123)    31838 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/Parsers/CalicoPolicyYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/Parsers/GenericIngressLikeYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/Parsers/GenericYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/Parsers/IngressPolicyYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/Parsers/IstioGenericYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/Parsers/IstioPolicyYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/Parsers/IstioSidecarYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    20463 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/Parsers/IstioTrafficResourcesYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    22622 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/Parsers/K8sPolicyYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/Parsers/K8sServiceYamlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/Parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:47:50.630441 network-config-analyzer-1.9.2/nca/Resources/
--rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/Resources/CalicoNetworkPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/Resources/IngressPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8174 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/Resources/IstioNetworkPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/Resources/IstioSidecar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/Resources/IstioTrafficResources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/Resources/K8sNamespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/Resources/K8sNetworkPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/Resources/K8sService.py
--rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/Resources/NetworkPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/Resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10937 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/SchemeRunner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:47:50.634441 network-config-analyzer-1.9.2/nca/Utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/Utils/CmdlineRunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/Utils/NcaLogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/Utils/OutputConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/Utils/OutputFilesFlags.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/nca/nca_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 14:47:50.634441 network-config-analyzer-1.9.2/network_config_analyzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-02-14 14:47:50.000000 network-config-analyzer-1.9.2/network_config_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-02-14 14:47:50.000000 network-config-analyzer-1.9.2/network_config_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 14:47:50.000000 network-config-analyzer-1.9.2/network_config_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-14 14:47:50.000000 network-config-analyzer-1.9.2/network_config_analyzer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-14 14:47:50.000000 network-config-analyzer-1.9.2/network_config_analyzer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-14 14:47:50.000000 network-config-analyzer-1.9.2/network_config_analyzer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-14 14:46:31.000000 network-config-analyzer-1.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-02-14 14:47:50.634441 network-config-analyzer-1.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.964907 network-config-analyzer-1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-07-10 14:10:26.964907 network-config-analyzer-1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.936906 network-config-analyzer-1.9.3/nca/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.944906 network-config-analyzer-1.9.3/nca/CoreDS/
+-rw-r--r--   0 runner    (1001) docker     (123)    41559 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/CoreDS/CanonicalHyperCubeSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/CoreDS/CanonicalIntervalSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31031 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/CoreDS/ConnectionSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/CoreDS/ConnectivityCube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23486 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/CoreDS/ConnectivityProperties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/CoreDS/DimensionsManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/CoreDS/MethodSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/CoreDS/MinDFA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30879 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/CoreDS/Peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/CoreDS/PortSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/CoreDS/ProtocolNameResolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/CoreDS/ProtocolSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/CoreDS/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.944906 network-config-analyzer-1.9.3/nca/FWRules/
+-rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/FWRules/ClusterInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28220 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/FWRules/ConnectivityGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10917 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/FWRules/DotGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28290 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/FWRules/FWRule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31821 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/FWRules/InteractiveConnectivityGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42145 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/FWRules/MinimizeFWRules.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/FWRules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.948907 network-config-analyzer-1.9.3/nca/FileScanners/
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/FileScanners/DirScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/FileScanners/GenericTreeScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/FileScanners/GitScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/FileScanners/HelmScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/FileScanners/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.952906 network-config-analyzer-1.9.3/nca/NetworkConfig/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.932906 network-config-analyzer-1.9.3/nca/NetworkConfig/LiveSim/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.952906 network-config-analyzer-1.9.3/nca/NetworkConfig/LiveSim/dns/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/LiveSim/dns/dns_pods.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.952906 network-config-analyzer-1.9.3/nca/NetworkConfig/LiveSim/ingress_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/LiveSim/ingress_controller/ingress_controller.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.952906 network-config-analyzer-1.9.3/nca/NetworkConfig/LiveSim/istio_gateway/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/LiveSim/istio_gateway/istio_custom_gateway.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/LiveSim/istio_gateway/istio_gateway.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17846 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/NetworkConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113771 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/NetworkConfigQuery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12897 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/NetworkConfigQueryRunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24609 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/NetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17500 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/PeerContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/PoliciesFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16993 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/QueryOutputHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26159 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/ResourcesHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17050 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/TopologyObjectsFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/NetworkConfig/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.956906 network-config-analyzer-1.9.3/nca/Parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)    37209 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Parsers/CalicoPolicyYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Parsers/GenericIngressLikeYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Parsers/GenericYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Parsers/IngressPolicyYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Parsers/IstioGenericYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29222 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Parsers/IstioPolicyYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Parsers/IstioServiceEntryYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16326 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Parsers/IstioSidecarYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20740 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Parsers/IstioTrafficResourcesYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24720 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Parsers/K8sPolicyYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Parsers/K8sServiceYamlParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.960907 network-config-analyzer-1.9.3/nca/Resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Resources/CalicoNetworkPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Resources/IngressPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10426 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Resources/IstioNetworkPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9967 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Resources/IstioSidecar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Resources/IstioTrafficResources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Resources/K8sNamespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Resources/K8sNetworkPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Resources/K8sService.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16397 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Resources/NetworkPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12379 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/SchemeRunner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.964907 network-config-analyzer-1.9.3/nca/Utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Utils/CmdlineRunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23062 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Utils/ExplTracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Utils/NcaLogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Utils/OutputConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Utils/OutputFilesFlags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Utils/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18776 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/nca/nca_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:10:26.964907 network-config-analyzer-1.9.3/network_config_analyzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11426 2023-07-10 14:10:26.000000 network-config-analyzer-1.9.3/network_config_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-10 14:10:26.000000 network-config-analyzer-1.9.3/network_config_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:10:26.000000 network-config-analyzer-1.9.3/network_config_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-10 14:10:26.000000 network-config-analyzer-1.9.3/network_config_analyzer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-10 14:10:26.000000 network-config-analyzer-1.9.3/network_config_analyzer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-10 14:10:26.000000 network-config-analyzer-1.9.3/network_config_analyzer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-10 14:08:54.000000 network-config-analyzer-1.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-10 14:10:26.964907 network-config-analyzer-1.9.3/setup.cfg
```

### Comparing `network-config-analyzer-1.9.2/LICENSE` & `network-config-analyzer-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.2/PKG-INFO` & `network-config-analyzer-1.9.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: network-config-analyzer
-Version: 1.9.2
+Version: 1.9.3
 Summary: An analyzer for Network Policies and other connectivity-configuration resources
 Home-page: https://github.com/IBM/network-config-analyzer
 Author: Ziv Nevo
 Author-email: nevo@il.ibm.com
 Project-URL: Bug Tracker, https://github.com/IBM/network-config-analyzer/issues
 Project-URL: NP-Guard Home, https://np-guard.github.io
 Classifier: Programming Language :: Python :: 3
@@ -97,29 +97,35 @@
 - `--label_subset  <A comma separated list of pairs (key:value) of labels (no spaces allowed)>`\
   Specifies the labels to include in the 'connectivity' query results. An element should include all the labels in this list to be included in the subset and in the results (AND operation). This switch may be specified multiple times and an element will be included if it matches one of the label-sets given in one of the switches (OR operation).
 - `--ghe_token <token>`\
   A valid token to access a GHE repository
 - `--period <minutes>`\
   Run NCA with given arguments every specified number of minutes
 - `--output_format <format>`\
-  Output format specification (txt/yaml/csv/md/dot/jpg).\
-  For jpg format, Graphviz executables must be installed and on user systems' PATH.\
+  Output format specification (txt/yaml/csv/md/dot/jpg/txt_no_fw_rules).\
+  `jpg` : Graphviz executables must be installed and on user systems' PATH.\
+  `txt_no_fw_rules`: supported for ConnectivityMap and SemanticDiff queries, printing connectivity rules for each pair of peers, without minimization and grouping of rules. (excluding  connections between workload to itself).
   *default:* txt\
   *shorthand:* `-o`
 - `--file_out <file name>`\
   A file path to redirect output into.\
   *shorthand* `-f`
 - `--expected_output <file name>`\
   A file path to the expected query output (for connectivity or semantic_diff queries).\
 - `--pr_url <URL>`\
    Write output as GitHub PR comment. URL points to the relevant `comments` resource in the GitHub API.\
    e.g., https://api.github.com/repos/shift-left-netconfig/online-boutique/issues/1/comments
 - `--output_endpoints`\
   Choose endpoints type in output (pods/deployments).\
   *default:* deployments
+  - `--explain`\
+  A pair of node names (comma separated) to explain the policies affecting their connection or lack of it. Relevant only for connectivity query.\
+  Connections including IP-Blocks will show only the configurations of the node in that connection (since, IP-Blocks does
+  not have configurations). IP-Blocks should be places in CIDR format as seen in the query results (run the connectivity query first, to see the nodes there).\
+  e.g. default/pod-A1,default/deployment-B1.
   - `--print_ipv6`\
   include IPv6 range in the query results even when the policies of the config do not contain any IPv6 addresses.
   
 
 For more information on command-line switches combinations, see [Common Query Patterns](docs/CommonQueryPatterns.md#cmdline-queries)
 
 ##### Simulating live cluster missing resources:
```

### Comparing `network-config-analyzer-1.9.2/README.md` & `network-config-analyzer-1.9.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -81,29 +81,35 @@
 - `--label_subset  <A comma separated list of pairs (key:value) of labels (no spaces allowed)>`\
   Specifies the labels to include in the 'connectivity' query results. An element should include all the labels in this list to be included in the subset and in the results (AND operation). This switch may be specified multiple times and an element will be included if it matches one of the label-sets given in one of the switches (OR operation).
 - `--ghe_token <token>`\
   A valid token to access a GHE repository
 - `--period <minutes>`\
   Run NCA with given arguments every specified number of minutes
 - `--output_format <format>`\
-  Output format specification (txt/yaml/csv/md/dot/jpg).\
-  For jpg format, Graphviz executables must be installed and on user systems' PATH.\
+  Output format specification (txt/yaml/csv/md/dot/jpg/txt_no_fw_rules).\
+  `jpg` : Graphviz executables must be installed and on user systems' PATH.\
+  `txt_no_fw_rules`: supported for ConnectivityMap and SemanticDiff queries, printing connectivity rules for each pair of peers, without minimization and grouping of rules. (excluding  connections between workload to itself).
   *default:* txt\
   *shorthand:* `-o`
 - `--file_out <file name>`\
   A file path to redirect output into.\
   *shorthand* `-f`
 - `--expected_output <file name>`\
   A file path to the expected query output (for connectivity or semantic_diff queries).\
 - `--pr_url <URL>`\
    Write output as GitHub PR comment. URL points to the relevant `comments` resource in the GitHub API.\
    e.g., https://api.github.com/repos/shift-left-netconfig/online-boutique/issues/1/comments
 - `--output_endpoints`\
   Choose endpoints type in output (pods/deployments).\
   *default:* deployments
+  - `--explain`\
+  A pair of node names (comma separated) to explain the policies affecting their connection or lack of it. Relevant only for connectivity query.\
+  Connections including IP-Blocks will show only the configurations of the node in that connection (since, IP-Blocks does
+  not have configurations). IP-Blocks should be places in CIDR format as seen in the query results (run the connectivity query first, to see the nodes there).\
+  e.g. default/pod-A1,default/deployment-B1.
   - `--print_ipv6`\
   include IPv6 range in the query results even when the policies of the config do not contain any IPv6 addresses.
   
 
 For more information on command-line switches combinations, see [Common Query Patterns](docs/CommonQueryPatterns.md#cmdline-queries)
 
 ##### Simulating live cluster missing resources:
```

### Comparing `network-config-analyzer-1.9.2/nca/CoreDS/CanonicalHyperCubeSet.py` & `network-config-analyzer-1.9.3/nca/CoreDS/CanonicalHyperCubeSet.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,16 @@
     """
 
     empty_interval = CanonicalIntervalSet()
 
     # TODO: should move dimensions order to DimensionsManager?
     def __init__(self, dimensions, allow_all=False):
         self.layers = dict()  # layers are w.r.t active dimensions
-        self.dimensions_manager = DimensionsManager()
         self.all_dimensions_list = dimensions  # ordered list of all dimensions
-        self.all_dim_types = [self.dimensions_manager.get_dimension_type_by_name(dim_name) for dim_name in dimensions]
+        self.all_dim_types = [DimensionsManager().get_dimension_type_by_name(dim_name) for dim_name in dimensions]
         # init ordered list of active dimensions:
         if allow_all:
             self.active_dimensions = []  # names (for non-active dimensions everything is allowed)
         else:
             # initialize as empty with all dimensions considered active.
             # in the next operations reducing to relevant active dimensions
             self.active_dimensions = self.all_dimensions_list
@@ -170,15 +169,15 @@
         :return: a cube (as a list) with all domain values, per required dimensions.
         """
         if dimensions_list_restriction is None:
             dimensions_list_restriction = self.all_dimensions_list
         dimensions_list_ordered = self._get_dimensions_subset_by_order(dimensions_list_restriction)
         cube_res = []
         for dim_name in dimensions_list_ordered:
-            cube_res.append(self.dimensions_manager.get_dimension_domain_by_name(dim_name))
+            cube_res.append(DimensionsManager().get_dimension_domain_by_name(dim_name, True))
         return cube_res
 
     def __len__(self):
         """
         :return: int: number of cubes in self.
         """
         if not self.active_dimensions:
@@ -262,15 +261,15 @@
         if self.is_all():
             self._override_by_other(other.copy())
             return self
         other_copy = self._prepare_common_active_dimensions(other)
         res = self._and_aux(other_copy)
         self.layers = res.layers
         self.active_dimensions = res.active_dimensions
-        self._reduce_active_dimensions()
+        self.reduce_active_dimensions()
         return self
 
     def _and_aux(self, other):
         """
         Recursive function to compute 'and' between two CanonicalHyperCubeSet objects.
         Assuming that self and other have common active dimensions.
         :type other: CanonicalHyperCubeSet
@@ -313,15 +312,15 @@
         if not self:
             self._override_by_other(other.copy())
             return self
         other_copy = self._prepare_common_active_dimensions(other)
         res = self.or_aux(other_copy)
         self.layers = res.layers
         self.active_dimensions = res.active_dimensions
-        self._reduce_active_dimensions()
+        self.reduce_active_dimensions()
         return self
 
     def or_aux(self, other):
         """
         Recursive function to compute 'or' between two CanonicalHyperCubeSet objects.
         Assuming that self and other have common active dimensions.
         :type other: CanonicalHyperCubeSet
@@ -366,15 +365,15 @@
             self.clear()
         if not other:
             return self
         other_copy = self._prepare_common_active_dimensions(other)
         res = self.sub_aux(other_copy)
         self.layers = res.layers
         self.active_dimensions = res.active_dimensions
-        self._reduce_active_dimensions()
+        self.reduce_active_dimensions()
         return self
 
     def sub_aux(self, other):
         """
         Recursive function to compute 'sub' between two CanonicalHyperCubeSet objects.
         Assuming that self and other have common active dimensions.
         :type other: CanonicalHyperCubeSet
@@ -520,15 +519,15 @@
                 if not self._contained_in_aux(sub_elem, all_active_dims[1:]):
                     return False
                 if covered_elem_res is None:
                     covered_elem_res = self._copy_layer_elem(elem)
                 else:
                     covered_elem_res |= elem
             # since the current dim is inactive for self, the covered_elem_res should equal the entire dim's domain
-            return covered_elem_res == self.dimensions_manager.get_dimension_domain_by_name(current_dim)
+            return covered_elem_res == DimensionsManager().get_dimension_domain_by_name(current_dim)
 
         # case 3: current_dim is common to both self and other
         assert current_dim in self.active_dimensions and current_dim in other.active_dimensions
         # sub-case (a): current_dim is last for both self and other : simple containment check
         if self._is_last_dimension() and other._is_last_dimension():
             return (self._get_last_dim_cube_value()).contained_in(other._get_last_dim_cube_value())
 
@@ -600,15 +599,15 @@
         for an input cube, get representing str (corresponding to active dimensions)
         :param cube: list representing a cube with dimensions from self.active_dimensions
         :return: str representation for cube's values
         """
         res = ""
         for dim_index, dim_values in enumerate(cube):
             dim_name = self.active_dimensions[dim_index]
-            res += self.dimensions_manager.get_dim_values_str(dim_values, dim_name) + ", "
+            res += DimensionsManager().get_dim_values_str(dim_values, dim_name) + ", "
         return f"({res})"
 
     def _is_last_dimension(self):
         """
         :return: bool indicating if current active dimension (self.active_dimensions[0]) is considered last dimension.
         """
         return len(self.active_dimensions) == 1
@@ -664,15 +663,15 @@
         for index, dim_name in enumerate(current_active_dimensions):
             current_active_dimensions_dict[dim_name] = index
         aligned_cube_values = []
         for active_dim_name in new_active_dimensions:
             if active_dim_name in current_active_dimensions_dict:
                 aligned_cube_values.append(cube[current_active_dimensions_dict[active_dim_name]])
             else:
-                aligned_cube_values.append(DimensionsManager().get_dimension_domain_by_name(active_dim_name))
+                aligned_cube_values.append(DimensionsManager().get_dimension_domain_by_name(active_dim_name, True))
         return aligned_cube_values
 
     def _set_active_dimensions(self, dim_names_set):
         """
         update self with active dimensions from dim_names_set.
         :param set[str] dim_names_set: set of dimension names
         """
@@ -714,24 +713,24 @@
                 self.active_dimensions = new_active_dimensions
                 return
             else:
                 # handle last dimension
                 self.active_dimensions = new_active_dimensions
                 new_sub_elem = CanonicalHyperCubeSet(self.all_dimensions_list)
                 new_sub_elem.active_dimensions = [new_active_dimensions[1]]
-                dim_all_values = self.dimensions_manager.get_dimension_domain_by_name(new_active_dimensions[1])
+                dim_all_values = DimensionsManager().get_dimension_domain_by_name(new_active_dimensions[1], True)
                 new_sub_elem.layers[dim_all_values] = CanonicalHyperCubeSet.empty_interval
                 new_sub_elem.build_new_active_dimensions(new_active_dimensions[1:])
                 for layer_elem in self.layers:
                     self.layers[layer_elem] = new_sub_elem
                 return
         # build new layer for new dimension: new_active_dimensions[0]
         new_layers = dict()
         new_dim = new_active_dimensions[0]
-        dim_all_values = self.dimensions_manager.get_dimension_domain_by_name(new_dim)
+        dim_all_values = DimensionsManager().get_dimension_domain_by_name(new_dim, True)
         new_layers[dim_all_values] = self.copy()
         self.active_dimensions = new_active_dimensions
         new_layers[dim_all_values].build_new_active_dimensions(new_active_dimensions[1:])
         self.layers = new_layers
 
     def _check_active_dimensions(self):
         """
@@ -812,26 +811,26 @@
             for (dim, dim_values) in sub_res.items():
                 if dim not in res:
                     res[dim] = dim_values
                 else:
                     res[dim] |= dim_values
         return res
 
-    def _reduce_active_dimensions(self):
+    def reduce_active_dimensions(self):
         """
         Change self so that its active dimensions are as minimal as possible:
         Inactivate dimensions for which every cube in self allows all its domain.
         """
         if not self or not self.active_dimensions:
             return
         # reduce by searching for active dimensions on which entire domain is allowed for all the cubes
         dimensions_to_reduce = []
         values_per_dimension = self._get_values_sets_per_active_dimension()
         for dim_name, values_set in values_per_dimension.items():
-            dim_domain = self.dimensions_manager.get_dimension_domain_by_name(dim_name)
+            dim_domain = DimensionsManager().get_dimension_domain_by_name(dim_name)
             if {dim_domain} == values_set:
                 dimensions_to_reduce.append(dim_name)
         dimensions_to_reduce = self._get_dimensions_subset_by_order(dimensions_to_reduce)
         self._set_inactive_dimensions(dimensions_to_reduce)
 
     def _apply_layer_elements_union(self):
         """
@@ -847,7 +846,10 @@
                 equiv_classes[layer1] = [layer0]
         for layer_1_elem, layer_0_elem_list in equiv_classes.items():
             layer_0_new_elem = layer_0_elem_list[0]
             for elem in layer_0_elem_list[1:]:
                 layer_0_new_elem |= elem
             new_layers[layer_0_new_elem] = layer_1_elem
         self.layers = new_layers
+
+    def is_active_dimension(self, dim_name):
+        return dim_name in self.active_dimensions
```

### Comparing `network-config-analyzer-1.9.2/nca/CoreDS/CanonicalIntervalSet.py` & `network-config-analyzer-1.9.3/nca/CoreDS/CanonicalIntervalSet.py`

 * *Files 5% similar despite different names*

```diff
@@ -216,14 +216,20 @@
             """
             :param other: another interval
             :return: Whether 'self' is a subset of 'other'
             :rtype: bool
             """
             return other.start <= self.start and other.end >= self.end
 
+        def is_single_value(self):
+            """
+            :return: Whether the interval contains a single value
+            """
+            return self.start == self.end
+
     def find_interval_left(self, interval):
         """
         find from left to right the last interval which is lower than the input interval,
         without overlapping/touching it
         :param CanonicalIntervalSet.Interval interval: the input interval to search for
         :return: the index of the interval in the interval set if found or -1 if not found
         :rtype: int
@@ -350,7 +356,17 @@
         res = []
         for interval in self:
             if interval.start == interval.end:
                 res.append(interval.start)
             else:
                 res.append(f'{interval.start}-{interval.end}')
         return res
+
+    def is_single_value(self):
+        """
+        :return: Whether the interval set contains a single value
+        """
+        return len(self) == 1 and list(self)[0].is_single_value()
+
+    def validate_and_get_single_value(self):
+        assert self.is_single_value()
+        return list(self)[0].start
```

### Comparing `network-config-analyzer-1.9.2/nca/CoreDS/ConnectionSet.py` & `network-config-analyzer-1.9.3/nca/CoreDS/ConnectionSet.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 #
 # Copyright 2020- IBM Inc. All rights reserved
 # SPDX-License-Identifier: Apache2.0
 #
+
+from collections import defaultdict
 from .CanonicalIntervalSet import CanonicalIntervalSet
-from .PortSet import PortSet
-from .TcpLikeProperties import TcpLikeProperties
-from .ICMPDataSet import ICMPDataSet
+from .ConnectivityProperties import ConnectivityProperties
 from .ProtocolNameResolver import ProtocolNameResolver
+from .ProtocolSet import ProtocolSet
+from .Peer import PeerSet, IpBlock
+from nca.FWRules import FWRule
 
 
 class ConnectionSet:
     """
     This class holds a set of connections and allows several manipulations on this set such as union, intersection, ...
     """
     _icmp_protocols = {1, 58}
     port_supporting_protocols = {6, 17, 132}
     _max_protocol_num = 255
-    _min_protocol_num = 1
+    _min_protocol_num = 0
 
     def __init__(self, allow_all=False):
-        self.allowed_protocols = {}  # a map from protocol number (1-255) to allowed properties (ports, icmp)
+        self.allowed_protocols = {}  # a map from protocol number (0-255) to allowed properties (ports, icmp)
         self.allow_all = allow_all  # Shortcut to represent all connections, and then allowed_protocols is to be ignored
 
     def __bool__(self):
         return self.allow_all or bool(self.allowed_protocols)
 
     def __eq__(self, other):
         if isinstance(other, ConnectionSet):
@@ -153,15 +156,15 @@
         return str(aggregated_properties), protocols_not_aggregated
 
     @staticmethod
     def _get_protocol_with_properties_representation(is_str, protocol_text, properties):
         """
         :param bool is_str: should get str representation (True) or list representation (False)
         :param str protocol_text: str description of protocol
-        :param Union[bool, TcpLikeProperties, ICMPDataSet] properties: properties object of the protocol
+        :param Union[bool, ConnectivityProperties] properties: properties object of the protocol
         :return: representation required for a given pair of protocol and its properties
         :rtype: Union[dict, str]
         """
         if not is_str:
             protocol_obj = {'Protocol': protocol_text}
             if not isinstance(properties, bool):
                 protocol_obj.update(properties.get_properties_obj())
@@ -191,23 +194,20 @@
             return 'No connections'
 
         if len(self.allowed_protocols) == 1:
             protocol_num = next(iter(self.allowed_protocols))
             protocol_text = 'Protocol: ' + ProtocolNameResolver.get_protocol_name(protocol_num)
             properties = self.allowed_protocols[protocol_num]
             properties_text = ''
-            if not isinstance(properties, bool):
+            if not isinstance(properties, bool) and str(properties):
                 properties_text = ', ' + str(properties)
             return protocol_text + properties_text
 
         protocol_text = 'Protocols: '
         for idx, protocol in enumerate(self.allowed_protocols.keys()):
-            if idx > 5:
-                protocol_text += ', ...'
-                break
             if idx > 0:
                 protocol_text += ', '
             protocol_text += ProtocolNameResolver.get_protocol_name(protocol)
 
             # add properties:
             properties = self.allowed_protocols[protocol]
             properties_text = ''
@@ -373,72 +373,76 @@
         for protocol, properties in self.allowed_protocols.items():
             res.allowed_protocols[protocol] = self.copy_properties(properties)
         return res
 
     @staticmethod
     def protocol_supports_ports(protocol):
         """
-        :param protocol: Protocol number
+        :param protocol: Protocol number or name
         :return: Whether the given protocol has ports
         :rtype: bool
         """
-        return protocol in ConnectionSet.port_supporting_protocols
+        prot = protocol
+        if isinstance(protocol, str):
+            prot = ProtocolNameResolver.get_protocol_number(protocol)
+        return prot in ConnectionSet.port_supporting_protocols
 
     @staticmethod
     def protocol_is_icmp(protocol):
         """
-        :param protocol: Protocol number
+        :param protocol: Protocol number or name
         :return: Whether the protocol is icmp or icmpv6
         :rtype: bool
         """
-        return protocol in ConnectionSet._icmp_protocols
+        prot = protocol
+        if isinstance(protocol, str):
+            prot = ProtocolNameResolver.get_protocol_number(protocol)
+        return prot in ConnectionSet._icmp_protocols
 
     def add_connections(self, protocol, properties=True):
         """
         Add connections to the set of connections
         :param int,str protocol: protocol number of the connections to add
         :param properties: an object with protocol properties (e.g., ports), if relevant
-        :type properties: Union[bool, TcpLikeProperties, ICMPDataSet]
+        :type properties: Union[bool, ConnectivityProperties]
         :return: None
         """
         if isinstance(protocol, str):
             protocol = ProtocolNameResolver.get_protocol_number(protocol)
-        if protocol < 1 or protocol > 255:
-            raise Exception('Protocol must be in the range 1-255')
+        if not ProtocolNameResolver.is_valid_protocol(protocol):
+            raise Exception('Protocol must be in the range 0-255')
         if not bool(properties):  # if properties are empty, there is nothing to add
             return
         if protocol in self.allowed_protocols:
             self.allowed_protocols[protocol] |= properties
         else:
-            self.allowed_protocols[protocol] = properties
+            self.allowed_protocols[protocol] = properties if isinstance(properties, bool) else properties.copy()
 
     def remove_protocol(self, protocol):
         """
         Remove a protocol from the set of connections
         :param int,str protocol: The protocol to remove
         :return: None
         """
         if isinstance(protocol, str):
             protocol = ProtocolNameResolver.get_protocol_number(protocol)
-        if protocol < 1 or protocol > 255:
-            raise Exception('Protocol must be in the range 1-255')
+        if not ProtocolNameResolver.is_valid_protocol(protocol):
+            raise Exception('Protocol must be in the range 0-255')
         if protocol not in self.allowed_protocols:
             return
         del self.allowed_protocols[protocol]
 
     def _add_all_connections_of_protocol(self, protocol):
         """
         Add all possible connections to the connection set for a given protocol
         :param protocol: the given protocol number
         :return: None
         """
-        if self.protocol_supports_ports(protocol):
-            self.allowed_protocols[protocol] = TcpLikeProperties(PortSet(True), PortSet(True))
-        elif self.protocol_is_icmp(protocol):
-            self.allowed_protocols[protocol] = ICMPDataSet(add_all=True)
+        if self.protocol_supports_ports(protocol) or self.protocol_is_icmp(protocol):
+            self.allowed_protocols[protocol] = ConnectivityProperties.make_all_props()
         else:
             self.allowed_protocols[protocol] = True
 
     def add_all_connections(self, excluded_protocols=None):
         """
         Add all possible connections to the connection set
         :param list[int] excluded_protocols: (optional) list of protocol numbers to exclude
@@ -534,19 +538,154 @@
         for protocol in other.allowed_protocols:
             if protocol not in self.allowed_protocols:
                 return other_name + ' allows communication using protocol ' + \
                     ProtocolNameResolver.get_protocol_name(protocol) + ' while ' + self_name + ' does not.'
 
         return 'No diff.'
 
+    def convert_to_connectivity_properties(self, peer_container):
+        """
+        Convert the current ConnectionSet to ConnectivityProperties format.
+        This function is used for comparing fw-rules output between original and optimized implementation,
+        when optimized_run == 'debug'
+        :param PeerContainer peer_container: the peer container
+        :return: the connection set in ConnectivityProperties format
+        """
+        if self.allow_all:
+            return ConnectivityProperties.get_all_conns_props_per_config_peers(peer_container)
+
+        res = ConnectivityProperties.make_empty_props()
+        for protocol, properties in self.allowed_protocols.items():
+            protocols = ProtocolSet.get_protocol_set_with_single_protocol(protocol)
+            this_prop = ConnectivityProperties.make_conn_props_from_dict({"protocols": protocols})
+            if isinstance(properties, bool):
+                if properties:
+                    res |= this_prop
+            else:
+                res |= (this_prop & properties)
+        return res
+
     @staticmethod
     def get_all_tcp_connections():
         tcp_conns = ConnectionSet()
-        tcp_conns.add_connections('TCP', TcpLikeProperties(PortSet(True), PortSet(True)))
+        tcp_conns.add_connections('TCP', ConnectivityProperties.make_all_props())
         return tcp_conns
 
     @staticmethod
     def get_non_tcp_connections():
         res = ConnectionSet()
         res.add_all_connections([ProtocolNameResolver.get_protocol_number('TCP')])
         return res
         # return ConnectionSet(True) - ConnectionSet.get_all_TCP_connections()
+
+    # TODO - after moving to the optimized HC set implementation,
+    #  get rid of ConnectionSet and move the code below to ConnectivityProperties.py
+
+    @staticmethod
+    def get_connection_set_and_peers_from_cube(conn_cube, peer_container,
+                                               relevant_protocols=ProtocolSet(True)):
+        src_peers = conn_cube["src_peers"] or peer_container.get_all_peers_group(True)
+        conn_cube.unset_dim("src_peers")
+        dst_peers = conn_cube["dst_peers"] or peer_container.get_all_peers_group(True)
+        conn_cube.unset_dim("dst_peers")
+        protocols = conn_cube["protocols"]
+        conn_cube.unset_dim("protocols")
+        if not conn_cube.has_active_dim() and (protocols.is_whole_range() or protocols == relevant_protocols):
+            conns = ConnectionSet(True)
+        else:
+            conns = ConnectionSet()
+            protocol_names = ProtocolSet.get_protocol_names_from_interval_set(protocols)
+            for protocol in protocol_names:
+                if conn_cube.has_active_dim():
+                    conns.add_connections(protocol, ConnectivityProperties.make_conn_props(conn_cube))
+                else:
+                    if ConnectionSet.protocol_supports_ports(protocol) or ConnectionSet.protocol_is_icmp(protocol):
+                        conns.add_connections(protocol,
+                                              ConnectivityProperties.get_all_conns_props_per_config_peers(peer_container))
+                    else:
+                        conns.add_connections(protocol, True)
+        return conns, src_peers, dst_peers
+
+    @staticmethod
+    def conn_props_to_fw_rules(conn_props, cluster_info, peer_container,
+                               connectivity_restriction):
+        """
+        Build FWRules from the given ConnectivityProperties
+        :param ConnectivityProperties conn_props: properties describing allowed connections
+        :param ClusterInfo cluster_info: the cluster info
+        :param PeerContainer peer_container: the peer container
+         whereas all other values should be filtered out in the output
+        :param Union[str,None] connectivity_restriction: specify if connectivity is restricted to
+               TCP / non-TCP , or not
+        :return: FWRules map
+        """
+        relevant_protocols = ProtocolSet()
+        if connectivity_restriction:
+            if connectivity_restriction == 'TCP':
+                relevant_protocols.add_protocol('TCP')
+            else:  # connectivity_restriction == 'non-TCP'
+                relevant_protocols = ProtocolSet.get_non_tcp_protocols()
+
+        fw_rules_map = defaultdict(list)
+        for cube in conn_props:
+            conn_cube = conn_props.get_connectivity_cube(cube)
+            conns, src_peers, dst_peers = \
+                ConnectionSet.get_connection_set_and_peers_from_cube(conn_cube, peer_container, relevant_protocols)
+            # create FWRules for src_peers and dst_peers
+            fw_rules_map[conns] += ConnectionSet.create_fw_rules_list_from_conns(conns, src_peers, dst_peers,
+                                                                                 cluster_info)
+        return fw_rules_map
+
+    @staticmethod
+    def create_fw_rules_list_from_conns(conns, src_peers, dst_peers, cluster_info):
+        src_fw_elements = ConnectionSet.split_peer_set_to_fw_rule_elements(src_peers, cluster_info)
+        dst_fw_elements = ConnectionSet.split_peer_set_to_fw_rule_elements(dst_peers, cluster_info)
+        fw_rules_list = []
+        for src_elem in src_fw_elements:
+            for dst_elem in dst_fw_elements:
+                fw_rules_list.append(FWRule.FWRule(src_elem, dst_elem, conns))
+        return fw_rules_list
+
+    @staticmethod
+    def split_peer_set_to_fw_rule_elements(peer_set, cluster_info):
+        res = []
+        peer_set_copy = peer_set.copy()
+        ns_set = set()
+        # first, split by namespaces
+        while peer_set_copy:
+            peer = list(peer_set_copy)[0]
+            if isinstance(peer, IpBlock):
+                res.append(FWRule.IPBlockElement(peer))
+                peer_set_copy.remove(peer)
+                continue
+            ns_peers = PeerSet(cluster_info.ns_dict[peer.namespace])
+            if ns_peers.issubset(peer_set_copy):
+                ns_set.add(peer.namespace)
+            else:
+                # TODO try to split the element below by labels
+                res.append(FWRule.PeerSetElement(ns_peers & peer_set_copy))
+            peer_set_copy -= ns_peers
+        if ns_set:
+            res.append(FWRule.FWRuleElement(ns_set))
+
+        return res
+
+    @staticmethod
+    def fw_rules_to_conn_props(fw_rules, peer_container):
+        """
+        Converting FWRules to ConnectivityProperties format.
+        This function is used for comparing FWRules output between original and optimized solutions,
+        when optimized_run == 'debug'
+        :param MinimizeFWRules fw_rules: the given FWRules.
+        :param PeerContainer peer_container: the peer container
+        :return: the resulting ConnectivityProperties.
+        """
+        res = ConnectivityProperties.make_empty_props()
+        for fw_rules_list in fw_rules.fw_rules_map.values():
+            for fw_rule in fw_rules_list:
+                conn_props = fw_rule.conn.convert_to_connectivity_properties(peer_container)
+                src_peers = PeerSet(fw_rule.src.get_peer_set(fw_rules.cluster_info))
+                dst_peers = PeerSet(fw_rule.dst.get_peer_set(fw_rules.cluster_info))
+                rule_props = ConnectivityProperties.make_conn_props_from_dict({"src_peers": src_peers,
+                                                                               "dst_peers": dst_peers}) & conn_props
+                res |= rule_props
+        return res
```

### Comparing `network-config-analyzer-1.9.2/nca/CoreDS/DimensionsManager.py` & `network-config-analyzer-1.9.3/nca/CoreDS/DimensionsManager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,36 @@
 #
 # Copyright 2020- IBM Inc. All rights reserved
 # SPDX-License-Identifier: Apache2.0
 #
 from enum import Enum
 from .CanonicalIntervalSet import CanonicalIntervalSet
 from .MethodSet import MethodSet
+from .ProtocolSet import ProtocolSet
+from .Peer import BasePeerSet
 from .MinDFA import MinDFA
 
 
 class DimensionsManager:
     """
     A singleton class to manage dimensions names and their association to type and domain.
-    The dimensions are related to certain protocol's properties in ConnectionSet.
+    The dimensions are related to certain protocol's properties in ConnectionSet / ConnectivityProperties.
     They are used for allowed connection representation, as protocols properties, within CanonicalHyperCubeSet objects.
+
+    The src_peers and dst_peers are special dimensions, they do not have constant domain.
+    Their domain depends on the current set of peers in the system (as appears in BasePeerSet singleton).
+    This set grows when adding more configurations.
+    Thus, there is no unique 'all values' representation. In particular, those dimensions are never reduced to inactive.
+    A mechanism to allow such reduction to `inactive`: per query context, set these dimensions domains to the set of
+    peers from the query's config(s) only.
+    The goal is to avoid having potential two representations of the same object (one with inactive domain and one with
+    an active domain containing all possible relevant peers, that was not reduced to inactive).
+    This mechanism is implemented at the execute_and_compute_output_in_required_format() method of the BaseNetworkQuery
+    class.
+
     """
 
     class DimensionType(Enum):
         IntervalSet = 0
         DFA = 1
 
     # the inner class is needed to make the outer class a singleton
@@ -26,27 +40,42 @@
             #  currently valid chars are: ['.', '/', '-', 0-9, a-z, A-Z ]
             self.default_interval_domain_tuple = (0, 100000)
             self.domain_str_to_dfa_map = dict()
             dfa_all_words_default = self._get_dfa_from_alphabet_str(MinDFA.default_alphabet_regex)
             dfa_all_words_path_domain = self._get_dfa_path_domain()
             ports_interval = CanonicalIntervalSet.get_interval_set(1, 65535)
             all_methods_interval = MethodSet(True)
-            all_peers_interval = CanonicalIntervalSet.get_interval_set(0, 10000)  # assuming max possible peer number
+            all_protocols_interval = ProtocolSet(True)
+            all_peers_interval = BasePeerSet.get_all_peers_and_ip_blocks_interval()
+            # dim_dict is a map from a dimension name to a tuple
+            # (dimension type, dimension full domain, dimension empty value)
             self.dim_dict = dict()
-            self.dim_dict["src_ports"] = (DimensionsManager.DimensionType.IntervalSet, ports_interval)
-            self.dim_dict["dst_ports"] = (DimensionsManager.DimensionType.IntervalSet, ports_interval)
-            self.dim_dict["methods"] = (DimensionsManager.DimensionType.IntervalSet, all_methods_interval)
-            self.dim_dict["peers"] = (DimensionsManager.DimensionType.IntervalSet, all_peers_interval)
-            self.dim_dict["paths"] = (DimensionsManager.DimensionType.DFA, dfa_all_words_path_domain)
-            self.dim_dict["hosts"] = (DimensionsManager.DimensionType.DFA, dfa_all_words_default)
+            self.dim_dict["src_ports"] = \
+                (DimensionsManager.DimensionType.IntervalSet, ports_interval, CanonicalIntervalSet())
+            self.dim_dict["dst_ports"] = \
+                (DimensionsManager.DimensionType.IntervalSet, ports_interval, CanonicalIntervalSet())
+            self.dim_dict["methods"] = \
+                (DimensionsManager.DimensionType.IntervalSet, all_methods_interval, MethodSet())
+            self.dim_dict["protocols"] = \
+                (DimensionsManager.DimensionType.IntervalSet, all_protocols_interval, ProtocolSet())
+            self.dim_dict["src_peers"] = \
+                (DimensionsManager.DimensionType.IntervalSet, all_peers_interval, CanonicalIntervalSet())
+            self.dim_dict["dst_peers"] = \
+                (DimensionsManager.DimensionType.IntervalSet, all_peers_interval, CanonicalIntervalSet())
+            self.dim_dict["paths"] = \
+                (DimensionsManager.DimensionType.DFA, dfa_all_words_path_domain, MinDFA.dfa_from_regex(""))
+            self.dim_dict["hosts"] = \
+                (DimensionsManager.DimensionType.DFA, dfa_all_words_default, MinDFA.dfa_from_regex(""))
 
             icmp_type_interval = CanonicalIntervalSet.get_interval_set(0, 254)
             icmp_code_interval = CanonicalIntervalSet.get_interval_set(0, 255)
-            self.dim_dict["icmp_type"] = (DimensionsManager.DimensionType.IntervalSet, icmp_type_interval)
-            self.dim_dict["icmp_code"] = (DimensionsManager.DimensionType.IntervalSet, icmp_code_interval)
+            self.dim_dict["icmp_type"] = \
+                (DimensionsManager.DimensionType.IntervalSet, icmp_type_interval, CanonicalIntervalSet())
+            self.dim_dict["icmp_code"] =\
+                (DimensionsManager.DimensionType.IntervalSet, icmp_code_interval, CanonicalIntervalSet())
 
         def _get_dfa_from_alphabet_str(self, alphabet_str):
             """
             get a MinDFA object for an input alphabet_str
             :param alphabet_str: regex in greenery format to express the str dimension domain
             :return: MinDFA object
             """
@@ -70,48 +99,74 @@
 
     instance = None
 
     def __init__(self):
         if not DimensionsManager.instance:
             DimensionsManager.instance = DimensionsManager.__DimensionsManager()
 
+    @staticmethod
+    def reset():
+        # used by unit tests to clean their local changes to DimensionsManager singleton
+        # also used by execute_and_compute_output_in_required_format to restore "src_peers"/"dst_peers"
+        # domains to a general domain value (after setting to a query-related specific domain value before
+        # the query computation)
+        DimensionsManager.instance = None
+
     def __getattr__(self, name):
         return getattr(self.instance, name)
 
     def get_dimension_type_by_name(self, dim_name):
         """
         get dimension's type from its name
         :param str dim_name: dimension name
         :return:  DimensionsManager.DimensionType: the type value
         """
         return self.dim_dict[dim_name][0]
 
-    def get_dimension_domain_by_name(self, dim_name):
+    def get_dimension_domain_by_name(self, dim_name, make_copy=False):
         """
         get dimensions domain from its name
         :param str dim_name: dimension name
+        :param bool make_copy: whether to copy the domain value
+        :return: CanonicalIntervalSet object or MinDFA object  (depends on dimension type)
+        """
+        res = self.dim_dict[dim_name][1]
+        if make_copy and not isinstance(res, MinDFA):
+            return res.copy()
+        else:
+            return res
+
+    def get_empty_dimension_by_name(self, dim_name):
+        """
+        get empty dimension value from its name
+        :param str dim_name: dimension name
         :return: CanonicalIntervalSet object or MinDFA object  (depends on dimension type)
         """
-        return self.dim_dict[dim_name][1]
+        return self.dim_dict[dim_name][2]
 
-    def set_domain(self, dim_name, dim_type, interval_tuple=None, alphabet_str=None):
+    def set_domain(self, dim_name, dim_type, interval_tuple_or_set=None, alphabet_str=None):
         """
         set a new dimension, or change an existing dimension
         :param str dim_name: dimension name
         :param DimensionsManager.DimensionType dim_type: dimension type
-        :param tuple(int,int) interval_tuple:  for interval domain value
+        :param tuple(int,int) interval_tuple_or_set:  for interval domain value
         :param str alphabet_str: regex in greenery format to express the str dimension domain
         """
         if dim_type == DimensionsManager.DimensionType.IntervalSet:
-            interval = interval_tuple if interval_tuple is not None else self.default_interval_domain_tuple
-            domain = CanonicalIntervalSet.get_interval_set(interval[0], interval[1])
+            if isinstance(interval_tuple_or_set, CanonicalIntervalSet):
+                domain = interval_tuple_or_set
+            else:
+                interval = interval_tuple_or_set if interval_tuple_or_set is not None else self.default_interval_domain_tuple
+                domain = CanonicalIntervalSet.get_interval_set(interval[0], interval[1])
+            empty_val = CanonicalIntervalSet()
         else:
             alphabet = alphabet_str if alphabet_str is not None else MinDFA.default_alphabet_regex
             domain = self._get_dfa_from_alphabet_str(alphabet)
-        self.dim_dict[dim_name] = (dim_type, domain)
+            empty_val = MinDFA.dfa_from_regex("")
+        self.dim_dict[dim_name] = (dim_type, domain, empty_val)
 
     def validate_value_by_domain(self, value, dim_name, value_name):
         """
         validate that value is valid, within the defined set of values by the dimension domain
         return validation result and error str if invalid
         :param Union[int,str] value: a value to validate (int or str, depends on the dimension type)
         :param str dim_name: dimension name
```

### Comparing `network-config-analyzer-1.9.2/nca/CoreDS/MethodSet.py` & `network-config-analyzer-1.9.3/nca/CoreDS/MethodSet.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,15 @@
 
     def add_method(self, method):
         """
         Adds a given method to the MethodSet if the method is one of the eligible methods (in all_methods_list);
         otherwise raises ValueError exception
         :param str method: the method to add
         """
-        try:
-            index = self.all_methods_list.index(method)
-        except ValueError:
-            assert False
+        index = self.all_methods_list.index(method)
         self.add_interval(self.Interval(index, index))
 
     def add_methods_from_regex(self, methods_regex):
         """
         Adds all methods in methods_regex to the MethodSet
         :param str methods_regex:
         """
```

### Comparing `network-config-analyzer-1.9.2/nca/CoreDS/MinDFA.py` & `network-config-analyzer-1.9.3/nca/CoreDS/MinDFA.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.2/nca/CoreDS/Peer.py` & `network-config-analyzer-1.9.3/nca/CoreDS/Peer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #
 # Copyright 2020- IBM Inc. All rights reserved
 # SPDX-License-Identifier: Apache2.0
 #
 import copy
 import ipaddress
+import re
 from ipaddress import ip_network
 from sys import stderr
 from string import hexdigits
 from .CanonicalIntervalSet import CanonicalIntervalSet
 
 
 class Peer:
@@ -16,15 +17,14 @@
     """
 
     def __init__(self, name, namespace):
         self.name = name
         self.namespace = namespace
         self.labels = {}  # Storing the endpoint's labels in a dict as key-value pairs
         self.extra_labels = {}  # for labels coming from 'labelsToApply' field in Profiles (Calico only)
-        self.prior_sidecar = None  # the first injected sidecar with workloadSelector selecting current peer
 
     def full_name(self):
         return self.namespace.name + '/' + self.name if self.namespace else self.name
 
     def set_label(self, key, value):
         """
         Add a label to the endpoint
@@ -145,18 +145,19 @@
         :param str owner_name: The name of the Pod's owner
         :param str owner_kind: The kind of the Pod's owner
         """
         super().__init__(name, namespace)
         self.owner_name = owner_name
         self.service_account_name = service_account_name
         self.full_name_str = self.namespace.name + '/' + self.name
-
+        self.replicaset_name = None
         if not owner_name:  # no owner
             self.workload_name = f'{namespace.name}/{name}(Pod)'
         elif owner_kind == 'ReplicaSet':
+            self.replicaset_name = f'{namespace.name}/{owner_name}(ReplicaSet)'
             # if owner name ends with hex-suffix, assume the pod is generated indirectly
             # by Deployment or StatefulSet; and remove the hex-suffix from workload name
             suffix = owner_name[owner_name.rfind('-') + 1:]
             if all(c in hexdigits for c in suffix):
                 self.workload_name = f'{namespace.name}/{owner_name[:owner_name.rfind("-")]}(Deployment-StatefulSet)'
             else:  # else, assume the pod is generated directly by a ReplicaSet
                 self.workload_name = f'{namespace.name}/{owner_name}(ReplicaSet)'
@@ -311,46 +312,51 @@
             cidr_list += [str(cidr) for cidr in cidrs]
         return cidr_list
 
     def get_cidr_list_str(self):
         cidr_list = self.get_cidr_list()
         return ','.join(str(cidr) for cidr in cidr_list)
 
-    def get_ip_range_or_cidr_str(self):
+    def get_ip_range_or_cidr_str(self, range_only=False):
         """
         Get str for self with shorter notation - either as ip range or as cidr
+        :param bool range_only: indicates if to return the self str as ip range only
         :rtype str
         """
         num_cidrs = len(self.get_cidr_list())
         num_ranges = len(self.interval_set)
-        if num_ranges * 2 <= num_cidrs:
+        if num_ranges * 2 <= num_cidrs or range_only:
             return str(self)
         return self.get_cidr_list_str()
 
     @staticmethod
-    def get_all_ips_block(exclude_ipv6=False):
+    def get_all_ips_block(exclude_ipv6=False, exclude_ipv4=False):
         """
         :return: The full range of ipv4 and ipv6 addresses if exclude_ipv6 is False
         :param bool exclude_ipv6: indicates if to exclude the IPv6 addresses
+        :param bool exclude_ipv4: indicates if to exclude the IPv4 addresses
         :rtype: IpBlock
         """
-        res = IpBlock('0.0.0.0/0')
+        assert not exclude_ipv6 or not exclude_ipv4
+        res = IpBlock()
+        if not exclude_ipv4:
+            res.add_cidr('0.0.0.0/0')
         if not exclude_ipv6:
             res.add_cidr('::/0')
         return res
 
     @staticmethod
     def get_all_ips_block_peer_set(exclude_ipv6=False):
         """
         :return: The full range of ipv4 and ipv6 addresses (ipv6 if exclude_ipv6 is False)
         :param bool exclude_ipv6: indicates if to exclude the IPv6 addresses
         :rtype: PeerSet
         """
         res = PeerSet()
-        res.add(IpBlock.get_all_ips_block(exclude_ipv6))
+        res.add(IpBlock.get_all_ips_block(exclude_ipv6=exclude_ipv6))
         return res
 
     def split(self):
         """
         Splits self's set of ip ranges into multiple IpBlock objects, each containing a single range
         :return PeerSet: A set of IpBlock objects, each with a single range of ips
         """
@@ -377,14 +383,20 @@
             exception_n = ip_network(exception, False)
             # the following line has no effect - only used to raise an exception when exception_n is not within cidr
             exception_n.subnet_of(ipn)
             hole = CanonicalIntervalSet.Interval(IPNetworkAddress(exception_n.network_address),
                                                  IPNetworkAddress(exception_n.broadcast_address))
             self.add_hole(hole)
 
+    def remove_cidr(self, cidr):
+        ipn = ip_network(cidr, False)  # strict is False as k8s API shows an example CIDR where host bits are set
+        hole = CanonicalIntervalSet.Interval(IPNetworkAddress(ipn.network_address),
+                                             IPNetworkAddress(ipn.broadcast_address))
+        self.add_hole(hole)
+
     def get_peer_set(self):
         """
         :return: get PeerSet from IpBlock (empty set if IpBlock is empty)
         """
         return PeerSet({self}) if self else PeerSet()
 
     @staticmethod
@@ -454,25 +466,103 @@
             ip_address = interval.start
             if isinstance(ip_address, IPNetworkAddress) and isinstance(ip_address.address, ipaddress.IPv4Address) or \
                     isinstance(ip_address, ipaddress.IPv4Address):
                 cnt += 1
         return cnt == len(self.interval_set)
 
 
+"""
+The following class DNSEntry; represents another type of external peer which is produced from istio ServiceEntry objects.
+Note: connectivity of DNSEntry peers is considered only for NetworkLayerName.Istio
+a DNSEntry peer is created from a single host in the serviceEntry object
+
+example: from this ServiceEntry yaml object:
+    `
+    apiVersion: networking.istio.io/v1alpha3
+    kind: ServiceEntry
+    metadata:
+        name: external-svc-first-test
+    spec:
+        hosts:
+            - www.slack.com
+            - www.google.com
+        location: MESH_EXTERNAL
+        ports:
+            - name: https-443
+              number: 443
+              protocol: HTTPS
+        resolution: NONE
+    `
+two DNSEntry peers will be created :
+1.DNSEntry(name=www.slack.com)
+2.DNSEntry(name=www.google.com)
+"""
+
+
+class DNSEntry(Peer):
+    """
+    represents DNS entries, produced by istio ServiceEntry objects.
+    A DNSEntry peer is created from single host in the service-entry hosts' list
+    """
+    # a dns entry pattern matches the following re-pattern
+    dns_pattern = r"(([A-Za-z0-9][-A-Za-z0-9_.]*)?[A-Za-z0-9])?"
+
+    def __init__(self, name=None, namespace=None):
+        """
+        Constructs a DNSEntry from the host name provided
+        currently: each DNSEntry peer is exported to all namespaces
+        """
+        Peer.__init__(self, name, namespace)
+
+    def __str__(self):
+        return self.name
+
+    def __repr__(self):
+        return self.name
+
+    def __hash__(self):
+        return hash(self.name)
+
+    def __eq__(self, other):
+        if isinstance(other, type(self)):
+            return self.name == other.name
+        return False
+
+    def canonical_form(self):
+        if self.namespace is None:
+            return self.name
+        else:
+            return self.namespace.name + '_' + self.name
+
+    @staticmethod
+    def compute_re_pattern_from_host_name(host_name):
+        """
+        translates the host name (dns) to a pattern that may be used with re library methods
+         - "*" at the beginning of the host name will be replaced with an FQDN pattern
+         - the "." in the host name may not be replaced by any other character
+         :param str host_name: the host name
+         :return: the re-pattern of the host name
+         :rtype: str
+        """
+        if host_name.startswith('*'):
+            name_suffix = re.escape(host_name[1:])
+            return DNSEntry.dns_pattern + name_suffix
+        return re.escape(host_name)
+
+
 class PeerSet(set):
     """
     A container to hold a set of Peer objects
 
     Note #1: objects of type IpBlock are not transformed into canonical form
     Note #2: __contains__ is implemented under the assumption that item arg is from disjoint_ip_blocks()
     """
 
     def __init__(self, peer_set=None):
         super().__init__(peer_set or set())
-        self.sorted_peer_list = []  # for converting PeerSet to CanonicalIntervalSet
 
     def __contains__(self, item):
         if isinstance(item, IpBlock):  # a special check here because an IpBlock may be contained in another IpBlock
             for peer in self:
                 if isinstance(peer, IpBlock) and item.contained_in(peer):
                     return True
             return False
@@ -490,15 +580,14 @@
     def copy(self):
         """
         :rtype: PeerSet
         """
         # TODO: shallow copy or deep copy?
         # res = PeerSet(set(elem.copy() for elem in self))
         res = PeerSet(super().copy())
-        res.sorted_peer_list = self.sorted_peer_list
         return res
 
     # TODO: what is expected for ipblock name/namespace result on intersection?
     def __iand__(self, other):
         # intersection of IpBlocks (canonical interval set)
         self_ip_block = self.get_ip_block_canonical_form()
         other_ip_block = other.get_ip_block_canonical_form()
@@ -512,18 +601,20 @@
 
     def __and__(self, other):
         res = self.copy()
         res &= other
         return res
 
     def __ior__(self, other):
-        return PeerSet(super().__ior__(other))
+        res = PeerSet(super().__ior__(other))
+        return res
 
     def __or__(self, other):
-        return PeerSet(super().__or__(other))
+        res = PeerSet(super().__or__(other))
+        return res
 
     def __isub__(self, other):
         # subtraction on IpBlocks
         self_ip_block = self.get_ip_block_canonical_form()
         other_ip_block = other.get_ip_block_canonical_form()
         res_peer_set_ip_block = (self_ip_block - other_ip_block).get_peer_set()
         # set subtraction
@@ -539,16 +630,15 @@
         return res
 
     def __hash__(self):
         """
         Note: PeerSet is a mutable type. Use with caution!
         :return: hash value for this object.
         """
-        self.update_sorted_peer_list()
-        return hash(','.join(str(peer.full_name()) for peer in self.sorted_peer_list))
+        return hash(','.join(str(peer.full_name()) for peer in sorted(list(elem for elem in self), key=by_full_name)))
 
     def rep(self):
         """
         Returns a representing peer from the set of peers
         :return str: The name of the representing peer. An empty string if set is empty
         """
         if not bool(self):
@@ -568,66 +658,150 @@
         """
         res = IpBlock()
         for elem in self:
             if isinstance(elem, IpBlock):
                 res |= elem
         return res
 
-    def update_sorted_peer_list(self):
-        """
-        create self.sorted_peer_list from non IpBlock pods
-        :return: None
-        """
-        self.sorted_peer_list = sorted(list(elem for elem in self), key=by_full_name)
-
-    def get_peer_interval_of(self, peer_set):
-        """
-        Calculates interval set of a given peer_set, based on the self peer_set
-        :param PeerSet peer_set: the peer_set to be converted to the interval set
-        :return: CanonicalIntervalSet for the peer_set
-        """
-        res = CanonicalIntervalSet()
-        if len(self.sorted_peer_list) != len(self):
-            # should update sorted_peer_list
-            self.update_sorted_peer_list()
-        for index, peer in enumerate(self.sorted_peer_list):
-            if peer in peer_set:
-                res.add_interval(CanonicalIntervalSet.Interval(index, index))
-        return res
-
-    def get_peer_list_by_indices(self, peer_inteval_set):
-        """
-        Return peer list from interval set of indices
-        :param peer_inteval_set: the interval set of indices into the sorted peer list
-        :return: the list of peers referenced by the indices in the interval set
-        """
-        assert len(self.sorted_peer_list) == len(self)
-        res = []
-        for interval in peer_inteval_set:
-            for ind in range(interval.start, interval.end + 1):
-                res.append(self.sorted_peer_list[ind])
-        return res
-
-    def get_all_peers_interval(self):
-        """
-        Returns the interval of all peers
-        :return: CanonicalIntervalSet of all peers
-        """
-        assert len(self.sorted_peer_list) == len(self)
-        return CanonicalIntervalSet.get_interval_set(0, len(self.sorted_peer_list) - 1)
-
-    def is_whole_range(self, peer_interval_set):
+    def filter_ipv6_blocks(self, ip_blocks_mask):
         """
-        Returns True iff the given peer interval set includes all peers
-        :param peer_interval_set: the given peer interval set
-        :return: bool whether the given interval set includes all peers
+        Update ip blocks in the peer set by keeping only parts overlapping with the given mask.
+        :param ip_blocks_mask: the mask according to which ip blocks should be updated
         """
-        return peer_interval_set == self.get_all_peers_interval()
+        peers_to_remove = []
+        peers_to_add = []
+        for peer in self:
+            if isinstance(peer, IpBlock):
+                peers_to_remove.append(peer)
+                if peer.overlaps(ip_blocks_mask):
+                    new_peer = peer.copy()
+                    new_peer &= ip_blocks_mask
+                    peers_to_add.append(new_peer)
+
+        for peer in peers_to_remove:
+            self.remove(peer)
+        for peer in peers_to_add:
+            self.add(peer)
 
 
 def by_full_name(elem):
     """
     Used for sorting peer list
     :param elem: Peer
     :return: Peer's name (the key being used by the sort)
     """
     return elem.full_name()
+
+
+class BasePeerSet:
+    """
+    A singleton class that keeps the set of all possible pods in the system (from all configs),
+    and translates PeerSets to CanonicalIntervalSets and vice versa.
+    """
+
+    # the inner class is needed to make the outer class a singleton
+    class __BasePeerSet:
+
+        ipv4_highest_number = int(ip_network('0.0.0.0/0').broadcast_address)
+        ipv6_highest_number = int(ip_network('::/0').broadcast_address)
+        max_num_of_pods = 10000
+        gap_width = 5  # the gap is needed to avoid mixed-type intervals union
+        min_ipv4_index = 0
+        max_ipv4_index = min_ipv4_index + ipv4_highest_number
+        min_ipv6_index = max_ipv4_index + gap_width
+        max_ipv6_index = min_ipv6_index + ipv6_highest_number
+        min_pod_index = max_ipv6_index + gap_width
+        max_pod_index = min_pod_index + max_num_of_pods - 1
+
+        def __init__(self):
+            self.ordered_peer_list = []  # for converting PeerSet to CanonicalIntervalSet
+            self.peer_to_index = dict()  # a map from peer name to index in self.ordered_peer_list
+
+        def add_peer(self, peer):
+            """
+            Adds a given peer to self peers.
+            :param peer: the peer to add.
+            """
+            if not isinstance(peer, IpBlock) and peer not in self.peer_to_index:
+                assert len(self.ordered_peer_list) < self.max_num_of_pods
+                self.peer_to_index[peer] = len(self.ordered_peer_list)
+                self.ordered_peer_list.append(peer)
+
+        def get_peer_interval_of(self, peer_set):
+            """
+            Translates the given peer_set to an interval set of indices
+            :param PeerSet peer_set: the peer_set to be converted to the interval set
+            :return: CanonicalIntervalSet for the peer_set
+            """
+            res = CanonicalIntervalSet()
+            for peer in peer_set:
+                if isinstance(peer, IpBlock):
+                    for cidr in peer:
+                        if isinstance(cidr.start.address, ipaddress.IPv4Address):
+                            res.add_interval(CanonicalIntervalSet.Interval(self.min_ipv4_index + int(cidr.start),
+                                                                           self.min_ipv4_index + int(cidr.end)))
+                        elif isinstance(cidr.start.address, ipaddress.IPv6Address):
+                            res.add_interval(CanonicalIntervalSet.Interval(self.min_ipv6_index + int(cidr.start),
+                                                                           self.min_ipv6_index + int(cidr.end)))
+                        else:
+                            assert False
+                else:
+                    index = self.peer_to_index.get(peer)
+                    assert index is not None
+                    res.add_interval(CanonicalIntervalSet.Interval(self.min_pod_index + index,
+                                                                   self.min_pod_index + index))
+            return res
+
+        def get_peer_set_by_indices(self, peer_interval_set):
+            """
+            Translates the given interval set of indices to a peer set.
+            :param peer_interval_set: the interval set of indices
+            :return: the PeerSet of peers referenced by the indices in the interval set
+            """
+            peer_set = PeerSet()
+            for interval in peer_interval_set:
+                if interval.end <= self.max_ipv4_index:
+                    # this is IPv4Address
+                    start = ipaddress.IPv4Address(interval.start - self.min_ipv4_index)
+                    end = ipaddress.IPv4Address(interval.end - self.min_ipv4_index)
+                    ipb = IpBlock(
+                        interval=CanonicalIntervalSet.Interval(IPNetworkAddress(start), IPNetworkAddress(end)))
+                    peer_set.add(ipb)
+                elif interval.end <= self.max_ipv6_index:
+                    # this is IPv6Address
+                    start = ipaddress.IPv6Address(interval.start - self.min_ipv6_index)
+                    end = ipaddress.IPv6Address(interval.end - self.min_ipv6_index)
+                    ipb = IpBlock(
+                        interval=CanonicalIntervalSet.Interval(IPNetworkAddress(start), IPNetworkAddress(end)))
+                    peer_set.add(ipb)
+                else:
+                    # this is Pod
+                    assert interval.end <= self.max_pod_index
+                    curr_pods_max_ind = len(self.ordered_peer_list) - 1
+                    for ind in range(min(interval.start - self.min_pod_index, curr_pods_max_ind),
+                                     min(interval.end - self.min_pod_index, curr_pods_max_ind) + 1):
+                        peer_set.add(self.ordered_peer_list[ind])
+            return peer_set
+
+    instance = None
+
+    def __init__(self):
+        if not BasePeerSet.instance:
+            BasePeerSet.instance = BasePeerSet.__BasePeerSet()
+
+    @staticmethod
+    def reset():
+        BasePeerSet.instance = None
+
+    def __getattr__(self, name):
+        return getattr(self.instance, name)
+
+    @staticmethod
+    def get_all_peers_and_ip_blocks_interval():
+        res = CanonicalIntervalSet()
+        res.add_interval(CanonicalIntervalSet.Interval(BasePeerSet.__BasePeerSet.min_ipv4_index,
+                                                       BasePeerSet.__BasePeerSet.max_ipv4_index))
+        res.add_interval(CanonicalIntervalSet.Interval(BasePeerSet.__BasePeerSet.min_ipv6_index,
+                                                       BasePeerSet.__BasePeerSet.max_ipv6_index))
+        res.add_interval(CanonicalIntervalSet.Interval(BasePeerSet.__BasePeerSet.min_pod_index,
+                                                       BasePeerSet.__BasePeerSet.max_pod_index))
+        return res
```

### Comparing `network-config-analyzer-1.9.2/nca/CoreDS/PortSet.py` & `network-config-analyzer-1.9.3/nca/CoreDS/PortSet.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,14 +52,17 @@
         if isinstance(port, str):
             self.named_ports.add(port)
             self.excluded_named_ports.discard(port)
         else:
             interval = CanonicalIntervalSet.Interval(port, port)
             self.port_set.add_interval(interval)
 
+    def add_ports(self, port_set):
+        self.port_set |= port_set
+
     def remove_port(self, port):
         if isinstance(port, str):
             self.named_ports.discard(port)
             self.excluded_named_ports.add(port)
         else:
             interval = CanonicalIntervalSet.Interval(port, port)
             self.port_set.add_hole(interval)
@@ -78,7 +81,16 @@
         self.port_set -= other.port_set
         self.named_ports -= other.named_ports
         self.excluded_named_ports |= other.named_ports
         return self
 
     def is_all(self):
         return self.port_set == PortSet.all_ports_interval
+
+    def is_empty(self):
+        return not self.port_set and not self.named_ports
+
+    @staticmethod
+    def make_port_set_with_range(min_port, max_port):
+        res = PortSet()
+        res.add_port_range(min_port, max_port)
+        return res
```

### Comparing `network-config-analyzer-1.9.2/nca/CoreDS/ProtocolNameResolver.py` & `network-config-analyzer-1.9.3/nca/CoreDS/ProtocolNameResolver.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,39 +53,49 @@
                                      119: 'SRP', 120: 'UTI', 121: 'SMP', 122: 'SMdeprecated', 123: 'PTP',
                                      124: 'ISISoverIPv4', 125: 'FIRE', 126: 'CRTP', 127: 'CRUDP', 128: 'SSCOPMCE',
                                      129: 'IPLT', 130: 'SPS', 131: 'PIPE', 132: 'SCTP', 133: 'FC', 134: 'RSVPE2EIGNORE',
                                      135: 'MobilityHeader', 136: 'UDPLite', 137: 'MPLSinIP', 138: 'manet', 139: 'HIP',
                                      140: 'Shim6', 141: 'WESP', 142: 'ROHC', 143: 'Ethernet'}
 
     @staticmethod
+    def is_valid_protocol(protocol):
+        return protocol >= 0 and protocol <= 255
+
+    @staticmethod
+    def get_all_protocols_list():
+        return list(ProtocolNameResolver._protocol_name_to_number_dict.keys())
+
+    @staticmethod
     def get_protocol_name(protocol_number: int) -> str:
         """
         :param protocol_number: Protocol number
         :return: The protocol name. If the protocol is not in the DB the protocol's number is returned as string, deeming it \
                  its 'name' for lack of a specific one.
         :rtype: str
         """
-        if protocol_number < 1 or protocol_number > 255:
-            raise Exception('Protocol number must be in the range 1-255')
+        if not ProtocolNameResolver.is_valid_protocol(protocol_number):
+            raise Exception('Protocol number must be in the range 0-255')
 
         return ProtocolNameResolver._protocol_number_to_name_dict.get(protocol_number, str(protocol_number))
 
     @staticmethod
     def get_protocol_number(protocol_name: str) -> int:
         """
         :param protocol_name: Protocol name
         :return: The protocol number
         :rtype: int
         """
         if isinstance(protocol_name, int):
             return protocol_name
 
         protocol_num = ProtocolNameResolver._protocol_name_to_number_dict.get(protocol_name)
-        if not protocol_num:
-            raise Exception('Unknown protocol name: ' + protocol_name)
+        if protocol_num is None:
+            protocol_num = int(protocol_name)
+            if not ProtocolNameResolver.is_valid_protocol(protocol_num):
+                raise Exception('Unknown protocol name: ' + protocol_name)
 
         return protocol_num
 
     @staticmethod
     def is_standard_protocol(protocol: int) -> bool:
         """
         :param protocol: Protocol number
```

### Comparing `network-config-analyzer-1.9.2/nca/FWRules/ClusterInfo.py` & `network-config-analyzer-1.9.3/nca/FWRules/ClusterInfo.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.2/nca/FWRules/FWRule.py` & `network-config-analyzer-1.9.3/nca/FWRules/FWRule.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #
 # Copyright 2020- IBM Inc. All rights reserved
 # SPDX-License-Identifier: Apache2.0
 #
 
-from nca.CoreDS.Peer import ClusterEP, IpBlock, Pod
+from nca.CoreDS.Peer import ClusterEP, IpBlock, Pod, PeerSet, DNSEntry
 from nca.Resources.K8sNamespace import K8sNamespace
 from .ClusterInfo import ClusterInfo
 
 
 class LabelExpr:
     """
     a class for representing a label expression
@@ -199,27 +199,36 @@
         :return: a set of pods in the cluster represented by this element
         """
         res = set()
         for ns in self.ns_info:
             res |= cluster_info.ns_dict[ns]
         return res
 
+    def get_peer_set(self, cluster_info):
+        """
+        :param cluster_info: an object of type ClusterInfo, with relevant cluster topology info
+        :return: a PeerSet (pods and/or IpBlocks)  represented by this element
+        """
+        return PeerSet(self.get_pods_set(cluster_info))
+
     @staticmethod
     def create_fw_elements_from_base_element(base_elem):
         """
         create a list of fw-rule-elements from base-element
-        :param base_elem: of type ClusterEP/IpBlock/K8sNamespace
-        :return: list fw-rule-elements of type:  list[PodElement]/list[IPBlockElement]/list[FWRuleElement]
+        :param base_elem: of type ClusterEP/IpBlock/K8sNamespace/DNSEntry
+        :return: list fw-rule-elements of type:  list[PodElement]/list[IPBlockElement]/list[FWRuleElement]/list[DNSElement]
         """
         if isinstance(base_elem, ClusterEP):
             return [PodElement(base_elem)]
         elif isinstance(base_elem, IpBlock):
             return [IPBlockElement(ip) for ip in base_elem.split()]
         elif isinstance(base_elem, K8sNamespace):
             return [FWRuleElement({base_elem})]
+        elif isinstance(base_elem, DNSEntry):
+            return [DNSElement(base_elem)]
         # unknown base-elem type
         return None
 
 
 class PodElement(FWRuleElement):
     """
     This is the class for single pod element in fw-rule
@@ -346,14 +355,90 @@
         values = self.element.values
         for v in values:
             pods_with_label_val_in_ns = cluster_info.pods_labels_map[(key, v)] & ns_pods
             res |= pods_with_label_val_in_ns
         return res
 
 
+class PeerSetElement(FWRuleElement):
+    """
+    This is the class for PeerSet element in fw rule
+    """
+
+    def __init__(self, element, output_as_deployment=True):
+        """
+        Create an object of type PeerSetElement
+        :param element: an element of type PeerSet
+        """
+        super().__init__({list(element)[0].namespace})
+        self.element = element
+        self.output_as_deployment = output_as_deployment
+
+    def get_elem_list_obj(self):
+        """
+        :return: list[string] for the field src_pods or dst_pods in representation for yaml/json object
+        """
+        return [str(self._get_pods_names())]
+
+    def get_pod_str(self):
+        """
+        :return: string for the field src_pods or dst_pods in representation for txt rule format
+        """
+        sorted_pods_names = ', '.join(sorted(self._get_pods_names().split(', ')))
+        return f'[{sorted_pods_names}]'
+
+    def _get_pods_names(self):
+        res = ''
+        unique_names = set()
+        for peer in self.element:
+            if self.output_as_deployment and isinstance(peer, Pod) and peer.owner_name:
+                if peer.owner_name not in unique_names:
+                    res += (', ' if res else '') + peer.owner_name
+                    unique_names.add(peer.owner_name)
+            else:
+                res += (', ' if res else '') + peer.name
+        return res
+
+    def __str__(self):
+        """
+        :return: string of the represented element
+        """
+        return f'ns: {self.get_ns_str()}, pods: {self.get_pod_str()}'
+
+    def get_elem_str(self, is_src):
+        """
+        :param is_src: bool flag to indicate if element is src (True) or dst (False)
+        :return: string of the represented element with src or dst description of fields
+        """
+        ns_prefix = 'src_ns: ' if is_src else 'dst_ns: '
+        pods_prefix = ' src_pods: ' if is_src else ' dst_pods: '
+        suffix = ' ' if is_src else ''
+        return ns_prefix + self.get_ns_str() + pods_prefix + self.get_pod_str() + suffix
+
+    def __hash__(self):
+        return hash(str(self))
+
+    def __eq__(self, other):
+        return isinstance(other, PeerSetElement) and self.element == other.element and super().__eq__(other)
+
+    def get_pods_set(self, cluster_info):
+        """
+        :param cluster_info: an object of type ClusterInfo, with relevant cluster topology info
+        :return: a set of pods in the cluster represented by this element
+        """
+        return self.element
+
+    def get_peer_set(self, cluster_info):
+        """
+        :param cluster_info: an object of type ClusterInfo, with relevant cluster topology info
+        :return: a PeerSet (pods and/or IpBlocks)  represented by this element
+        """
+        return self.get_pods_set(cluster_info)
+
+
 # TODO: should it be a sub-type of FWRuleElement?
 class IPBlockElement(FWRuleElement):
     """
     Class for ip-block element in a fw-rule
     """
 
     def __init__(self, element):
@@ -404,14 +489,87 @@
         """
         :param cluster_info: an object of type ClusterInfo, with relevant cluster topology info
         :return: a set of pods in the cluster represented by this element
         """
         # an ip block element does not represent any pods
         return set()
 
+    def get_peer_set(self, cluster_info):
+        """
+        :param cluster_info: an object of type ClusterInfo, with relevant cluster topology info
+        :return: a PeerSet (pods and/or IpBlocks)  represented by this element
+        """
+        return PeerSet({self.element})
+
+
+class DNSElement(FWRuleElement):
+    """
+    class for single dnsEntry element in fw-rule
+    """
+
+    def __init__(self, element):
+        """
+        Create an object of DNSElement
+        :param element: an element of type DNSEntry
+        """
+        super().__init__(set())  # no ns for DNSEntry
+        self.element = element
+
+    def get_ns_str(self):
+        return ''
+
+    def get_pod_str(self):
+        """
+        :return: string for the field src_pods or dst_pods in representation for txt rule format
+        """
+        return ''
+
+    def get_elem_list_obj(self):
+        """
+        :return: list[string] for the host name
+        """
+        return [self.element.name]
+
+    def __str__(self):
+        """
+        :return: string of the represented element
+        """
+        return self.element.name
+
+    def get_elem_str(self, is_src):
+        """
+        :param is_src: bool flag to indicate if element is src (True) or dst (False), always False
+        :return: string of the represented element with src or dst description of fields
+        """
+        assert not is_src  # currently we don't support DNSEntry as src peer
+        prefix = 'src: ' if is_src else 'dst: '
+        suffix = ' ' if is_src else ''
+        return prefix + str(self) + suffix
+
+    def __hash__(self):
+        return hash(str(self))
+
+    def __eq__(self, other):
+        return isinstance(other, DNSElement) and self.element == other.element and super().__eq__(other)
+
+    def get_pods_set(self, cluster_info):
+        """
+        :param cluster_info: an object of type ClusterInfo, with relevant cluster topology info
+        :return: a set of pods in the cluster represented by this element
+        """
+        # an dns-entry element does not represent any pods
+        return set()
+
+    def get_peer_set(self, cluster_info):
+        """
+        :param cluster_info: an object of type ClusterInfo, with relevant cluster topology info
+        :return: a PeerSet (pods and/or IpBlocks)  represented by this element
+        """
+        return PeerSet({self.element})
+
 
 class FWRule:
     """
     Class for holding a fw-rule: src, dst, connection-set
     """
 
     rule_csv_header = ['query', 'src_ns', 'src_pods', 'dst_ns', 'dst_pods', 'connection']
@@ -474,19 +632,19 @@
         This function is used to produce a csv row for a fw-rule
         :param str component: a fw-rule required component  from components in rule_csv_header
         :return: string of the required rule component
         """
         if component == 'src_ns':
             return self.src.get_ns_str()
         elif component == 'src_pods':
-            return str(self.src) if isinstance(self.src, IPBlockElement) else self.src.get_pod_str()
+            return str(self.src) if isinstance(self.src, (IPBlockElement, DNSElement)) else self.src.get_pod_str()
         elif component == 'dst_ns':
             return self.dst.get_ns_str()
         elif component == 'dst_pods':
-            return str(self.dst) if isinstance(self.dst, IPBlockElement) else self.dst.get_pod_str()
+            return str(self.dst) if isinstance(self.dst, (IPBlockElement, DNSElement)) else self.dst.get_pod_str()
         elif component == 'connection':
             return self.conn.get_simplified_connections_representation(True)
         return ''
 
     def get_rule_csv_row(self):
         """
         :return: a list of strings, representing the csv row for this fw-rule
@@ -498,22 +656,23 @@
 
     def get_rule_dict_obj(self):
         """
         :return:  a dict with content representing the fw-rule, for output in yaml/ json format
         """
         src_ns_list = sorted([str(ns) for ns in self.src.ns_info])
         dst_ns_list = sorted([str(ns) for ns in self.dst.ns_info])
-        src_pods_list = self.src.get_elem_list_obj() if not isinstance(self.src, IPBlockElement) else None
-        dst_pods_list = self.dst.get_elem_list_obj() if not isinstance(self.dst, IPBlockElement) else None
+        src_pods_list = self.src.get_elem_list_obj() if not isinstance(self.src, (IPBlockElement, DNSElement)) else None
+        dst_pods_list = self.dst.get_elem_list_obj() if not isinstance(self.dst, (IPBlockElement, DNSElement)) else None
         src_ip_block_list = sorted(self.src.get_elem_list_obj()) if isinstance(self.src, IPBlockElement) else None
         dst_ip_block_list = sorted(self.dst.get_elem_list_obj()) if isinstance(self.dst, IPBlockElement) else None
+        dst_dns_entry_list = sorted(self.dst.get_elem_list_obj()) if isinstance(self.dst, DNSElement) else None
         conn_list = self.conn.get_simplified_connections_representation(False)
 
         rule_obj = {}
-        if src_ip_block_list is None and dst_ip_block_list is None:
+        if src_ip_block_list is None and dst_ip_block_list is None and dst_dns_entry_list is None:
             rule_obj = {'src_ns': src_ns_list,
                         'src_pods': src_pods_list,
                         'dst_ns': dst_ns_list,
                         'dst_pods': dst_pods_list,
                         'connection': conn_list}
         elif src_ip_block_list is not None:
             rule_obj = {'src_ip_block': src_ip_block_list,
@@ -522,14 +681,20 @@
                         'connection': conn_list}
 
         elif dst_ip_block_list is not None:
             rule_obj = {'src_ns': src_ns_list,
                         'src_pods': src_pods_list,
                         'dst_ip_block': dst_ip_block_list,
                         'connection': conn_list}
+
+        elif dst_dns_entry_list is not None:
+            rule_obj = {'src_ns': src_ns_list,
+                        'src_pods': src_pods_list,
+                        'dst_dns_entry': dst_dns_entry_list,
+                        'connection': conn_list}
         return rule_obj
 
     def get_rule_in_req_format(self, req_format):
         """
         get fw-rule representation according to required format :
         yaml/ json: dict object
         csv: list of strings
```

### Comparing `network-config-analyzer-1.9.2/nca/FWRules/MinimizeFWRules.py` & `network-config-analyzer-1.9.3/nca/FWRules/MinimizeFWRules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
 # Copyright 2020- IBM Inc. All rights reserved
 # SPDX-License-Identifier: Apache2.0
 #
 
 from nca.CoreDS.ConnectionSet import ConnectionSet
-from nca.CoreDS.Peer import IpBlock, ClusterEP, Pod, HostEP
-from .FWRule import FWRuleElement, FWRule, PodElement, LabelExpr, PodLabelsElement, IPBlockElement
+from nca.CoreDS.Peer import IpBlock, ClusterEP, Pod, HostEP, DNSEntry
+from .FWRule import FWRuleElement, FWRule, PodElement, LabelExpr, PodLabelsElement, IPBlockElement, DNSElement
 
 
 class MinimizeCsFwRules:
     """
     This is a class for minimizing fw-rules within a specific connection-set
     """
 
@@ -102,16 +102,17 @@
                                        self.cluster_info.ns_dict[dst_ns])
                 if ns_product_pairs.issubset(self.covered_peer_pairs_union):
                     self.ns_pairs |= {(src_ns, dst_ns)}
                 else:
                     self.peer_pairs_without_ns_expr |= ns_product_pairs & self.peer_pairs
 
         # TODO: what about peer pairs with ip blocks from containing connections, not only peer_pairs for this connection?
-        pairs_with_elems_without_ns = set((src, dst) for (src, dst) in self.peer_pairs
-                                          if isinstance(src, (IpBlock, HostEP)) or isinstance(dst, (IpBlock, HostEP)))
+        pairs_with_elems_without_ns = \
+            set((src, dst) for (src, dst) in self.peer_pairs
+                if isinstance(src, (IpBlock, HostEP, DNSEntry)) or isinstance(dst, (IpBlock, HostEP, DNSEntry)))
         self.peer_pairs_without_ns_expr |= pairs_with_elems_without_ns
         # compute pairs with src as pod/ip-block and dest as namespace
         self._compute_ns_pairs_with_partial_ns_expr(False)
         # compute pairs with src as pod/ip-block namespace dest as pod
         self._compute_ns_pairs_with_partial_ns_expr(True)
         # remove pairs of (pod,pod) for trivial cases of communication from pod to itself
         self._remove_trivial_rules_from_peer_pairs_without_ns_expr()
@@ -358,15 +359,15 @@
         res = []
         for (src, dst) in base_elems_pairs:
             res.extend(FWRule.create_fw_rules_from_base_elements(src, dst, self.connections))
         return res
 
     def _create_all_initial_fw_rules(self):
         """
-        Creating initial fw-rules from base-elements pairs (pod/ns/ip-block)
+        Creating initial fw-rules from base-elements pairs (pod/ns/ip-block/dns-entry)
         :return: a list of initial fw-rules of type FWRule
         :rtype list[FWRule]
         """
         initial_fw_rules = []
         initial_fw_rules.extend(self._create_initial_fw_rules_from_base_elements_list(self.ns_pairs))
         initial_fw_rules.extend(self._create_initial_fw_rules_from_base_elements_list(self.peer_pairs_without_ns_expr))
         initial_fw_rules.extend(
@@ -426,15 +427,16 @@
         :return: A list of fw-rules after possible grouping operations
         """
         res = []
         # partition set_for_grouping_elems into: (1) ns_elems, (2) pod_and_pod_labels_elems, (3) ip_block_elems
         pod_and_pod_labels_elems = set(elem for elem in set_for_grouping_elems if
                                        isinstance(elem, (PodElement, PodLabelsElement)))
         ip_block_elems = set(elem for elem in set_for_grouping_elems if isinstance(elem, IPBlockElement))
-        ns_elems = set_for_grouping_elems - (pod_and_pod_labels_elems | ip_block_elems)
+        dns_elems = set(elem for elem in set_for_grouping_elems if isinstance(elem, DNSElement))
+        ns_elems = set_for_grouping_elems - (pod_and_pod_labels_elems | ip_block_elems | dns_elems)
 
         if ns_elems:
             # grouping of ns elements is straight-forward
             ns_set = set.union(*(f.ns_info for f in ns_elems))
             res.extend(self.get_ns_fw_rules_grouped_by_common_elem(src_first, ns_set, fixed_elem))
 
         if pod_and_pod_labels_elems:
@@ -475,14 +477,21 @@
             # currently no grouping for ip blocks
             for elem in ip_block_elems:
                 if src_first:
                     res.append(FWRule(fixed_elem, elem, self.connections))
                 else:
                     res.append(FWRule(elem, fixed_elem, self.connections))
 
+        if dns_elems:
+            for elem in dns_elems:
+                if src_first:  # do we need both if else? , dns_elem may be a dst always
+                    res.append(FWRule(fixed_elem, elem, self.connections))
+                else:
+                    res.append(FWRule(elem, fixed_elem, self.connections))
+
         return res
 
     def _create_merged_rules_set(self, is_src_first, fw_rules):
         """
         Computing a minimized set of fw-rules by merging src/dst elements iteratively
         :param is_src_first: a bool flag to indicate if merge process starts with src or dest
         :param fw_rules: a list of initial fw-rules
@@ -541,35 +550,39 @@
             #    continue
             print(rule)
 
     def get_src_dest_pairs_from_fw_rules(self, rules):
         src_dest_pairs = []
         for rule in rules:
             # compute set of pods derived from rule src and rule dest
-            if not isinstance(rule.src, IPBlockElement) and not isinstance(rule.dst, IPBlockElement):
+            if not isinstance(rule.src, (IPBlockElement, DNSElement)) and \
+                    not isinstance(rule.dst, (IPBlockElement, DNSElement)):
                 src_set = rule.src.get_pods_set(self.cluster_info)
                 dest_set = rule.dst.get_pods_set(self.cluster_info)
 
                 for src in src_set:
                     for dst in dest_set:
                         src_dest_pairs.append((src, dst))
 
-            elif isinstance(rule.src, IPBlockElement) and not isinstance(rule.dst, IPBlockElement):
+            elif isinstance(rule.src, IPBlockElement) and not isinstance(rule.dst, (IPBlockElement, DNSElement)):
                 dest_set = rule.dst.get_pods_set(self.cluster_info)
                 for dst in dest_set:
                     src_dest_pairs.append((rule.src.element, dst))
 
-            elif not isinstance(rule.src, IPBlockElement) and isinstance(rule.dst, IPBlockElement):
+            elif not isinstance(rule.src, (IPBlockElement, DNSElement)) and \
+                    isinstance(rule.dst, (IPBlockElement, DNSElement)):
                 src_set = rule.src.get_pods_set(self.cluster_info)
                 for src in src_set:
                     src_dest_pairs.append((src, rule.dst.element))
 
         for (src, dst) in src_dest_pairs:
             if isinstance(src, IpBlock) and isinstance(dst, IpBlock):
                 src_dest_pairs.remove((src, dst))
+            if isinstance(src, DNSEntry):  # we should not get here but if somehow the src is dns-entry it will be removed
+                src_dest_pairs.remove((src, dst))
 
         return set(src_dest_pairs)
 
     @staticmethod
     def validate_ip_blocks(ips_list_1, ips_list_2):
         ip_block_1 = IpBlock()
         ip_block_2 = IpBlock()
@@ -664,15 +677,16 @@
         :rtype: Union[str, dict]
         """
         query_name = self.output_config.queryName
         if self.output_config.configName:
             query_name += ', config: ' + self.output_config.configName
         output_format = self.output_config.outputFormat
         if output_format not in FWRule.supported_formats:
-            print(f'error: unexpected outputFormat in output configuration value [should be txt/yaml/csv],  '
+            supported_formats_joined = '\\'.join(FWRule.supported_formats)
+            print(f'error: unexpected outputFormat in output configuration value [should be {supported_formats_joined}], '
                   f'value is: {output_format}')
         return self.get_fw_rules_content(query_name, output_format, add_txt_header, add_csv_header, connectivity_restriction)
 
     def get_fw_rules_content(self, query_name, req_format, add_txt_header, add_csv_header, connectivity_restriction):
         """
         :param query_name: a string of the query name
         :param req_format: a string of the required format, should be in FWRule.supported_formats
```

### Comparing `network-config-analyzer-1.9.2/nca/FileScanners/DirScanner.py` & `network-config-analyzer-1.9.3/nca/FileScanners/DirScanner.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.2/nca/FileScanners/GenericTreeScanner.py` & `network-config-analyzer-1.9.3/nca/FileScanners/GenericTreeScanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     """
     data: object
     path: str
 
 
 class ObjectWithLocation:
     line_number = 0
+    path = ''
     column_number = 0
 
 
 class YamlDict(dict, ObjectWithLocation):
     pass
 
 
@@ -32,21 +33,23 @@
     pass
 
 
 def to_yaml_objects(yaml_node):
     if isinstance(yaml_node, yaml.SequenceNode):
         res = YamlList()
         res.line_number = yaml_node.start_mark.line
+        res.path = yaml_node.start_mark.name
         res.column_number = yaml_node.start_mark.column
         for obj in yaml_node.value:
             res.append(to_yaml_objects(obj))
         return res
     if isinstance(yaml_node, yaml.MappingNode):
         res = YamlDict()
         res.line_number = yaml_node.start_mark.line + 1
+        res.path = yaml_node.start_mark.name
         res.column_number = yaml_node.start_mark.column + 1
         for obj in yaml_node.value:
             res[obj[0].value] = to_yaml_objects(obj[1])
         return res
 
     # Node is a ScalarNode. First check if it can be interpreted as an int (e.g., port number)
     try:
```

### Comparing `network-config-analyzer-1.9.2/nca/FileScanners/GitScanner.py` & `network-config-analyzer-1.9.3/nca/FileScanners/GitScanner.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.2/nca/FileScanners/HelmScanner.py` & `network-config-analyzer-1.9.3/nca/FileScanners/HelmScanner.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.2/nca/NetworkConfig/NetworkConfig.py` & `network-config-analyzer-1.9.3/nca/NetworkConfig/NetworkConfig.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 # Copyright 2020- IBM Inc. All rights reserved
 # SPDX-License-Identifier: Apache2.0
 #
 
 from dataclasses import dataclass, field
 from nca.CoreDS import Peer
 from nca.CoreDS.ConnectionSet import ConnectionSet
-from nca.Resources.NetworkPolicy import NetworkPolicy
+from nca.CoreDS.ConnectivityProperties import ConnectivityProperties
+from nca.Resources.NetworkPolicy import NetworkPolicy, OptimizedPolicyConnections
 from .NetworkLayer import NetworkLayersContainer, NetworkLayerName
+from nca.Utils.ExplTracker import ExplTracker
 
 
 @dataclass
 class PoliciesContainer:
     """
     A class for holding policies map and layers map containing sorted policies per layer
     policies: map from tuples (policy name, policy type) to policy objects
@@ -43,22 +45,23 @@
 class NetworkConfig:
     """
     Represents a network configuration - the set of endpoints, their partitioning to namespaces and a set of policies
     that limit the allowed connectivity.
     The class also contains the core algorithm of computing allowed connections between two endpoints.
     """
 
-    def __init__(self, name, peer_container, policies_container):
+    def __init__(self, name, peer_container, policies_container, optimized_run='false'):
         """
         :param str name: A name for this config
         :param PeerContainer peer_container: The set of endpoints and their namespaces
         """
         self.name = name
         self.peer_container = peer_container
         self.policies_container = policies_container
+        self.optimized_run = optimized_run
         self.allowed_labels = None
         self.referenced_ip_blocks = None
 
     def __eq__(self, other):
         if not isinstance(other, NetworkConfig):
             return False
         return self.name == other.name and self.peer_container == other.peer_container and \
@@ -100,15 +103,16 @@
 
     def clone_without_policies(self, name):
         """
         :return: A clone of the config without any policies
         :rtype: NetworkConfig
         """
         policies_container = PoliciesContainer()
-        res = NetworkConfig(name, peer_container=self.peer_container, policies_container=policies_container)
+        res = NetworkConfig(name, peer_container=self.peer_container, policies_container=policies_container,
+                            optimized_run=self.optimized_run)
         return res
 
     def clone_without_policy(self, policy_to_exclude):
         """
         :param NetworkPolicy policy_to_exclude: A policy object to exclude from the clone
         :return: A clone of the config having all policies but the one specified
         :rtype: NetworkConfig
@@ -261,14 +265,88 @@
             denied_conns_res |= denied_conns_per_layer
 
         # an allowed captured conn (by at least one layer) has to be allowed by all layers (either implicitly or explicitly)
         allowed_captured_conns_res &= allowed_conns_res
 
         return allowed_conns_res, captured_flag_res, allowed_captured_conns_res, denied_conns_res
 
+    def allowed_connections_optimized(self, layer_name=None):
+        """
+        Computes the set of allowed connections between any relevant peers.
+        :param NetworkLayerName layer_name: The name of the layer to use, if requested to use a specific layer only
+        :return: allowed_conns: all allowed connections for relevant peers.
+        :rtype: OptimizedPolicyConnections
+        """
+        if ExplTracker().is_active():
+            ExplTracker().set_peers(self.peer_container.peer_set)
+        if layer_name is not None:
+            if layer_name not in self.policies_container.layers:
+                return self.policies_container.layers.empty_layer_allowed_connections_optimized(self.peer_container,
+                                                                                                layer_name)
+            return self.policies_container.layers[layer_name].allowed_connections_optimized(self.peer_container)
+
+        all_peers = self.peer_container.get_all_peers_group()
+        host_eps = Peer.PeerSet(set([peer for peer in all_peers if isinstance(peer, Peer.HostEP)]))
+        # all possible connections involving hostEndpoints
+        conn_hep = ConnectivityProperties.make_conn_props_from_dict({"src_peers": host_eps}) | \
+            ConnectivityProperties.make_conn_props_from_dict({"dst_peers": host_eps})
+        if host_eps and NetworkLayerName.K8s_Calico not in self.policies_container.layers:
+            # maintain K8s_Calico layer as active if peer container has hostEndpoint
+            conns_res = \
+                self.policies_container.layers.empty_layer_allowed_connections_optimized(self.peer_container,
+                                                                                         NetworkLayerName.K8s_Calico)
+            conns_res.allowed_conns &= conn_hep
+            conns_res.denied_conns &= conn_hep
+            conns_res.pass_conns &= conn_hep
+        else:
+            conns_res = OptimizedPolicyConnections()
+            conns_res.all_allowed_conns = ConnectivityProperties.get_all_conns_props_per_config_peers(self.peer_container)
+        for layer, layer_obj in self.policies_container.layers.items():
+            conns_per_layer = layer_obj.allowed_connections_optimized(self.peer_container)
+            # only K8s_Calico layer handles host_eps
+            if layer != NetworkLayerName.K8s_Calico:
+                # connectivity of hostEndpoints is only determined by calico layer
+                conns_per_layer.allowed_conns -= conn_hep
+                conns_per_layer.denied_conns -= conn_hep
+                conns_per_layer.pass_conns -= conn_hep
+
+            # all allowed connections: intersection of all allowed connections from all layers
+            conns_res.all_allowed_conns &= conns_per_layer.all_allowed_conns
+            # all allowed captured connections: should be captured by at least one layer
+            conns_res.allowed_conns |= conns_per_layer.allowed_conns
+            conns_res.captured |= conns_per_layer.captured
+            # denied conns: should be denied by at least one layer
+            conns_res.denied_conns |= conns_per_layer.denied_conns
+
+        # allowed captured conn (by at least one layer) has to be allowed by all layers (either implicitly or explicitly)
+        conns_res.allowed_conns &= conns_res.all_allowed_conns
+        return conns_res
+
     def append_policy_to_config(self, policy):
         """
         appends a policy to an existing config
         :param NetworkPolicy.NetworkPolicy policy: The policy to append
         :return: None
         """
         self.policies_container.append_policy(policy)
+
+    def filter_conns_by_peer_types(self, conns, all_peers):
+        """
+        Filter the given connections by removing several connection kinds that are never allowed
+        (such as IpBlock to IpBlock connections, connections from DNSEntries, and more).
+        :param ConnectivityProperties conns: the given connections.
+        :param PeerSet all_peers: all peers in the system.
+        :return The resulting connections.
+        :rtype ConnectivityProperties
+        """
+        res = conns
+        # avoid IpBlock -> {IpBlock, DNSEntry} connections
+        all_ips = Peer.IpBlock.get_all_ips_block_peer_set()
+        all_dns_entries = self.peer_container.get_all_dns_entries()
+        ip_to_ip_or_dns_conns = ConnectivityProperties.make_conn_props_from_dict({"src_peers": all_ips,
+                                                                                  "dst_peers": all_ips | all_dns_entries})
+        res -= ip_to_ip_or_dns_conns
+        # avoid DNSEntry->anything connections
+        dns_to_any_conns = ConnectivityProperties.make_conn_props_from_dict({"src_peers": all_dns_entries,
+                                                                             "dst_peers": all_peers})
+        res -= dns_to_any_conns
+        return res
```

### Comparing `network-config-analyzer-1.9.2/nca/NetworkConfig/NetworkConfigQuery.py` & `network-config-analyzer-1.9.3/nca/NetworkConfig/NetworkConfigQuery.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 #
 # Copyright 2020- IBM Inc. All rights reserved
 # SPDX-License-Identifier: Apache2.0
 #
 import itertools
 import os
+import time
 from abc import abstractmethod
 from collections import defaultdict
 from enum import Enum
 
 from nca.CoreDS.ConnectionSet import ConnectionSet
-from nca.CoreDS.Peer import PeerSet, IpBlock, Pod, Peer
+from nca.CoreDS.Peer import PeerSet, IpBlock, Pod, Peer, DNSEntry, BasePeerSet
+from nca.CoreDS.ProtocolSet import ProtocolSet
+from nca.CoreDS.ConnectivityProperties import ConnectivityProperties
+from nca.CoreDS.DimensionsManager import DimensionsManager
 from nca.FWRules.ConnectivityGraph import ConnectivityGraph
+from nca.FWRules.MinimizeFWRules import MinimizeFWRules
+from nca.FWRules.ClusterInfo import ClusterInfo
 from nca.Resources.CalicoNetworkPolicy import CalicoNetworkPolicy
 from nca.Resources.IngressPolicy import IngressPolicy
 from nca.Utils.OutputConfiguration import OutputConfiguration
 from .QueryOutputHandler import QueryAnswer, DictOutputHandler, StringOutputHandler, \
     PoliciesAndRulesExplanations, PodsListsExplanations, ConnectionsDiffExplanation, IntersectPodsExplanation, \
     PoliciesWithCommonPods, PeersAndConnections, ComputedExplanation
 from .NetworkLayer import NetworkLayerName
+from nca.Utils.ExplTracker import ExplTracker
 
 
 class QueryType(Enum):
     SingleConfigQuery = 0
     ComparisonToBaseConfigQuery = 1
     PairComparisonQuery = 2
     PairwiseComparisonQuery = 3
@@ -49,32 +56,51 @@
         :param policy: the given policy
         :return: the title of the policy
         """
         return f'{policy.policy_type_str()} {policy.full_name()}'
 
     def execute_and_compute_output_in_required_format(self, cmd_line_flag=False):
         """
-        calls the exec def of the running query, computes its output to fit the required format and returns query results
-        and output
+        calls the exec def of the running query, computes its output to fit the required format and returns query
+        results and output
         :param cmd_line_flag: indicates if the query is running from a cmd-line, since it affects computing the
         numerical result of some of TwoNetworkConfigsQuery queries
         :return: the numerical result of the query,
         the query output in form to be written in required format if supported (otherwise empty string),
         and bool indicator if the query was not executed
         :rtype: int, Union[dict, str], bool
         """
+        # peer_set collects the set of peers from the config(s) related to current query
+        peer_set = PeerSet()
         for config in self.get_configs():
             if not config.peer_container.get_num_peers():
                 error_msg = f'Error: Network configuration \'{config.name}\' does not have any peers. Can not run Query'
                 query_answer = QueryAnswer(output_result=error_msg, query_not_executed=True)
                 return query_answer.numerical_result, self._handle_output(query_answer), query_answer.query_not_executed
-        query_answer = self.execute(cmd_line_flag)
+            peer_set |= config.peer_container.get_all_peers_group(True, True, True)
         if self.output_config.outputFormat not in self.get_supported_output_formats():
+            query_answer = QueryAnswer(query_not_executed=True)
             return query_answer.numerical_result, '', query_answer.query_not_executed
-
+        # update domains src_peers/dst_peers with domains specific to current peer_set of current query
+        DimensionsManager().set_domain("src_peers", DimensionsManager.DimensionType.IntervalSet,
+                                       BasePeerSet().get_peer_interval_of(peer_set))
+        DimensionsManager().set_domain("dst_peers", DimensionsManager.DimensionType.IntervalSet,
+                                       BasePeerSet().get_peer_interval_of(peer_set))
+        # update all optimized connectivity properties by reducing full src_peers/dst_peers dimensions
+        # according to their updated domains (above)
+        for config in self.get_configs():
+            for policy in config.policies_container.policies.values():
+                policy.reorganize_opt_props_by_new_domains()
+        # run the query
+        query_answer = self.execute(cmd_line_flag)
+        # restore peers domains and optimized connectivity properties original values
+        DimensionsManager.reset()
+        for config in self.get_configs():
+            for policy in config.policies_container.policies.values():
+                policy.restore_opt_props()
         return query_answer.numerical_result, self._handle_output(query_answer), query_answer.query_not_executed
 
     def _handle_output(self, query_answer):
         """
         handles returning the output of the running query in a form that matches writing required format
         Using the relevant OutputHandler class
         :param QueryAnswer query_answer: the query result of running its exec def
@@ -100,14 +126,31 @@
     def get_configs_names(self):
         raise NotImplementedError
 
     @abstractmethod
     def get_configs(self):
         raise NotImplementedError
 
+    # this def contains conditions that should be checked every time before computing
+    # allowed connections of two peers, so added it here to avoid duplications in the queries code
+    @staticmethod
+    def determine_whether_to_compute_allowed_conns_for_peer_types(peer1, peer2):
+        """
+        determines if to continue to compute allowed connections for the given
+        pair of peers based on their types
+        :param Peer peer1: the src peer
+        :param Peer peer2: the dst peer
+        :rtype: bool
+        """
+        if isinstance(peer1, DNSEntry):  # connections from DNSEntry are not relevant
+            return False
+        if isinstance(peer1, IpBlock) and isinstance(peer2, (IpBlock, DNSEntry)):
+            return False  # connectivity between external peers is not relevant either
+        return True
+
 
 class NetworkConfigQuery(BaseNetworkQuery):
     """
     A base class for queries that inspect only a single network config
     """
 
     def __init__(self, config, output_config_obj=None):
@@ -393,15 +436,16 @@
         :param NetworkConfig config_with_self_policy: A network config with self_policy as its single policy
         :param NetworkLayerName layer_name: The layer name of the policy
         :return: A policy containing self_policy's allowed connections if exist, None otherwise
         :rtype: NetworkPolicy
         """
         policies_list = self.config.policies_container.layers[layer_name].policies_list
         for other_policy in policies_list:
-            if other_policy.get_order() and self_policy.get_order() and other_policy.get_order() < self_policy.get_order():
+            if other_policy.get_order() and self_policy.get_order() and \
+                    other_policy.get_order() < self_policy.get_order():
                 return None  # All other policies have a lower order and cannot contain self_policy
             if other_policy == self_policy:
                 continue
             if not self_policy.selected_peers.issubset(other_policy.selected_peers):
                 continue
             config_with_other_policy = self.config.clone_with_just_one_policy(other_policy.full_name())
             if ContainmentQuery(config_with_self_policy, config_with_other_policy).exec(only_captured=True).bool_result:
@@ -415,21 +459,24 @@
         :param NetworkConfig config_with_self_policy: A network config with self_policy as its single policy
         :param NetworkLayerName layer_name: The layer name of the policy
         :return: A policy containing self_policy's denied connections if exist, None otherwise
         :rtype: NetworkPolicy
         """
         policies_list = self.config.policies_container.layers[layer_name].policies_list
         for other_policy in policies_list:
-            if other_policy.get_order() and self_policy.get_order() and other_policy.get_order() < self_policy.get_order():
+            if other_policy.get_order() and self_policy.get_order() and \
+                    other_policy.get_order() < self_policy.get_order():
                 return None  # not checking lower priority for Calico
             if other_policy == self_policy:
                 continue
             if not other_policy.has_deny_rules():
                 continue
             config_with_other_policy = self.config.clone_with_just_one_policy(other_policy.full_name())
+            # calling get_all_peers_group does not require getting dnsEntry peers, since they are not relevant when computing
+            # deny connections
             pods_to_compare = self.config.peer_container.get_all_peers_group()
             pods_to_compare |= TwoNetworkConfigsQuery(self.config,
                                                       config_with_other_policy).disjoint_referenced_ip_blocks()
             for pod1 in pods_to_compare:
                 for pod2 in pods_to_compare:
                     if isinstance(pod1, IpBlock) and isinstance(pod2, IpBlock):
                         continue
@@ -452,15 +499,16 @@
         :param bool is_ingress: Whether this is an ingress rule or an egress rule
         :param NetworkLayerName layer_name: The layer name of the policy
         :return: If a containing rule is found, return its policy, its index and whether it contradicts the input rule
         :rtype: NetworkPolicy, int, bool
         """
         policies_list = self.config.policies_container.layers[layer_name].policies_list
         for other_policy in policies_list:
-            if other_policy.get_order() and self_policy.get_order() and other_policy.get_order() < self_policy.get_order():
+            if other_policy.get_order() and self_policy.get_order() and \
+                    other_policy.get_order() < self_policy.get_order():
                 return None, None, None  # All following policies have a lower order - containment is not interesting
             if is_ingress:
                 found_index, contradict = other_policy.ingress_rule_containing(self_policy, self_rule_index)
             else:
                 found_index, contradict = other_policy.egress_rule_containing(self_policy, self_rule_index)
             if found_index:
                 return other_policy, found_index, contradict
@@ -617,15 +665,15 @@
 class ConnectivityMapQuery(NetworkConfigQuery):
     """
     Print the connectivity graph in the form of firewall rules
     """
 
     @staticmethod
     def get_supported_output_formats():
-        return {'txt', 'yaml', 'csv', 'md', 'dot', 'json', 'jpg'}
+        return {'txt', 'yaml', 'csv', 'md', 'dot', 'json', 'jpg', 'txt_no_fw_rules'}
 
     def is_in_subset(self, peer):
         """
         returns indication if the peer element is in the defined subset
         Please note: Subset is a sort of a filter. It filters out elements which WERE DEFINED and do
         not match the settings.
         Thus, the function returns True if no subset was defined
@@ -659,144 +707,395 @@
             # go over the labels and see if all of them are defined
             for single_label_subset in list(subset['label_subset']):
                 if self.are_labels_all_included(single_label_subset, peer.labels):
                     return True
 
         return False
 
+    def compute_subset(self, peers):
+        """
+        Computes all peers that are in the defined subset out of the given peer set
+        :param PeerSet peers: the given peer set
+        :return: peers in the defined subset
+        """
+        if not self.output_config.subset:
+            return peers
+        res = PeerSet()
+        for peer in peers:
+            if self.is_in_subset(peer):
+                res.add(peer)
+        return res
+
     @staticmethod
     def are_labels_all_included(target_labels, pool_labels):
         for key, val in target_labels.items():
             if pool_labels.get(key) != val:
                 return False
         return True
 
-    def exec(self):
-        self.output_config.fullExplanation = True  # assign true for this query - it is always ok to compare its results
-        self.output_config.configName = os.path.basename(self.config.name) if self.config.name.startswith('./') else \
-            self.config.name
-        peers_to_compare = self.config.peer_container.get_all_peers_group()
-
+    def compute_connectivity_output_original(self):
+        """
+        Compute connectivity output with original implementation (running for every pair of peers).
+        :return: a tuple of output result (in a required format), FwRules, tcp FWRules and non-tcp FWRules.
+        :rtype ([Union[str, dict], MinimizeFWRules, MinimizeFWRules], MinimizeFWRules)
+        """
+        fw_rules = None
+        fw_rules_tcp = None
+        fw_rules_non_tcp = None
         exclude_ipv6 = self.output_config.excludeIPv6Range
-        ref_ip_blocks = IpBlock.disjoint_ip_blocks(self.config.get_referenced_ip_blocks(exclude_ipv6),
-                                                   IpBlock.get_all_ips_block_peer_set(exclude_ipv6),
-                                                   exclude_ipv6)
         connections = defaultdict(list)
-        peers = PeerSet()
+        # if dns entry peers exist but no istio policies are configured,
+        # then actually istio layer exists implicitly, connections to these peers will be considered with the
+        # default Istio outbound traffic mode - allow any
+        peers_to_compare = self.config.peer_container.get_all_peers_group(include_dns_entries=True)
+        ref_ip_blocks = IpBlock.disjoint_ip_blocks(self.config.get_referenced_ip_blocks(exclude_ipv6),
+                                                   IpBlock.get_all_ips_block_peer_set(exclude_ipv6), exclude_ipv6)
         peers_to_compare |= ref_ip_blocks
-
+        peers = PeerSet()
         for peer1 in peers_to_compare:
             for peer2 in peers_to_compare:
                 if self.is_in_subset(peer1):
                     peers.add(peer1)
                 elif not self.is_in_subset(peer2):
                     continue  # skipping pairs if none of them are in the given subset
-                if isinstance(peer1, IpBlock) and isinstance(peer2, IpBlock):
-                    continue  # skipping pairs with ip-blocks for both src and dst
+                if not self.determine_whether_to_compute_allowed_conns_for_peer_types(peer1, peer2):
+                    continue
                 if peer1 == peer2:
                     # cannot restrict pod's connection to itself
                     connections[ConnectionSet(True)].append((peer1, peer2))
                 else:
                     conns, _, _, _ = self.config.allowed_connections(peer1, peer2)
                     if conns:
                         connections[conns].append((peer1, peer2))
                         # collect both peers, even if one of them is not in the subset
                         peers.add(peer1)
                         peers.add(peer2)
-
         # if Istio is a layer in the network config - produce 2 maps, for TCP and for non-TCP
         # because Istio policies can only capture TCP connectivity
         if self.config.policies_container.layers.does_contain_layer(NetworkLayerName.Istio):
-            output_res = self.get_connectivity_output_split_by_tcp(connections, peers, peers_to_compare)
+            output_res, fw_rules_tcp, fw_rules_non_tcp = \
+                self.get_connectivity_output_split_by_tcp(connections, peers, peers_to_compare)
         else:
-            output_res = self.get_connectivity_output_full(connections, peers, peers_to_compare)
+            output_res, fw_rules = self.get_connectivity_output_full(connections, peers, peers_to_compare)
+        return output_res, fw_rules, fw_rules_tcp, fw_rules_non_tcp
 
-        res = QueryAnswer(True)
-        if self.output_config.outputFormat in ['json', 'yaml']:
-            res.output_explanation = [ComputedExplanation(dict_explanation=output_res)]
+    def compute_connectivity_output_optimized(self):
+        """
+        Compute connectivity output with optimized implementation.
+        :return: a tuple of output result (in a required format), FwRules, tcp FWRules and non-tcp FWRules.
+        :rtype: ([Union[str, dict], MinimizeFWRules, MinimizeFWRules, MinimizeFWRules)
+        """
+        opt_fw_rules = None
+        opt_fw_rules_tcp = None
+        opt_fw_rules_non_tcp = None
+        exclude_ipv6 = self.output_config.excludeIPv6Range
+        opt_conns = self.config.allowed_connections_optimized()
+        all_conns_opt = opt_conns.all_allowed_conns
+        opt_peers_to_compare = self.config.peer_container.get_all_peers_group(include_dns_entries=True)
+        # add all relevant IpBlocks, used in connections
+        opt_peers_to_compare |= all_conns_opt.project_on_one_dimension('src_peers') | \
+            all_conns_opt.project_on_one_dimension('dst_peers')
+        if exclude_ipv6:
+            ip_blocks_mask = IpBlock.get_all_ips_block(exclude_ipv6=True)
+            ref_ip_blocks = self.config.get_referenced_ip_blocks(exclude_ipv6)
+            for ip_block in ref_ip_blocks:
+                ip_blocks_mask |= ip_block
+            opt_peers_to_compare.filter_ipv6_blocks(ip_blocks_mask)
+            # remove connections where any of src_peers or dst_peers contains automatically-added IPv6 blocks,
+            # while keeping connections with IPv6 blocks directly referenced in policies
+            all_conns_opt &= ConnectivityProperties.make_conn_props_from_dict({"src_peers": opt_peers_to_compare,
+                                                                               "dst_peers": opt_peers_to_compare})
+        base_peers_num = len(opt_peers_to_compare)
+        subset_peers = self.compute_subset(opt_peers_to_compare)
+        all_peers = subset_peers
+        if len(subset_peers) != base_peers_num:
+            # remove connections where both of src_peers and dst_peers are out of the subset
+            subset_conns = ConnectivityProperties.make_conn_props_from_dict({"src_peers": subset_peers}) | \
+                           ConnectivityProperties.make_conn_props_from_dict({"dst_peers": subset_peers})
+            all_conns_opt &= subset_conns
+            src_peers, dst_peers = ExplTracker().extract_peers(all_conns_opt)
+            all_peers = src_peers | dst_peers
+        all_conns_opt = self.config.filter_conns_by_peer_types(all_conns_opt, opt_peers_to_compare)
+        expl_conns = all_conns_opt
+        if self.config.policies_container.layers.does_contain_layer(NetworkLayerName.Istio):
+            output_res, opt_fw_rules_tcp, opt_fw_rules_non_tcp = \
+                self.get_props_output_split_by_tcp(all_conns_opt, opt_peers_to_compare)
+            expl_conns, _ = self.convert_props_to_split_by_tcp(all_conns_opt)
         else:
-            res.output_explanation = [ComputedExplanation(str_explanation=output_res)]
+            output_res, opt_fw_rules = self.get_props_output_full(all_conns_opt, opt_peers_to_compare)
+        if ExplTracker().is_active():
+            ExplTracker().set_connections_and_peers(expl_conns, all_peers)
+        return output_res, opt_fw_rules, opt_fw_rules_tcp, opt_fw_rules_non_tcp
+
+    def exec(self):
+        self.output_config.fullExplanation = True  # assign true for this query - it is always ok to compare its results
+        self.output_config.configName = os.path.basename(self.config.name) if self.config.name.startswith('./') else \
+            self.config.name
+        res = QueryAnswer(True)
+        fw_rules = None
+        fw_rules_tcp = None
+        fw_rules_non_tcp = None
+        if self.config.optimized_run != 'true':
+            orig_start = time.time()
+            output_res, fw_rules, fw_rules_tcp, fw_rules_non_tcp = self.compute_connectivity_output_original()
+            orig_end = time.time()
+            print(f'Original loop: time: {(orig_end - orig_start):6.2f} seconds')
+            if self.output_config.outputFormat in ['json', 'yaml']:
+                res.output_explanation = [ComputedExplanation(dict_explanation=output_res)]
+            else:
+                res.output_explanation = [ComputedExplanation(str_explanation=output_res)]
+
+        if self.config.optimized_run != 'false':
+            opt_start = time.time()
+            output_res, opt_fw_rules, opt_fw_rules_tcp, opt_fw_rules_non_tcp = \
+                self.compute_connectivity_output_optimized()
+            opt_end = time.time()
+            print(f'Opt time: {(opt_end - opt_start):6.2f} seconds')
+            if self.config.optimized_run == 'debug':
+                if fw_rules and fw_rules.fw_rules_map and opt_fw_rules and opt_fw_rules.fw_rules_map:
+                    self.compare_fw_rules(fw_rules, opt_fw_rules)
+                if fw_rules_tcp and fw_rules_tcp.fw_rules_map and \
+                        opt_fw_rules_tcp and opt_fw_rules_tcp.fw_rules_map:
+                    self.compare_fw_rules(fw_rules_tcp, opt_fw_rules_tcp)
+                if fw_rules_non_tcp and fw_rules_non_tcp.fw_rules_map and \
+                        opt_fw_rules_non_tcp and opt_fw_rules_non_tcp.fw_rules_map:
+                    self.compare_fw_rules(fw_rules_non_tcp, opt_fw_rules_non_tcp)
+            else:  # self.config.optimized_run == 'true':
+                if self.output_config.outputFormat in ['json', 'yaml']:
+                    res.output_explanation = [ComputedExplanation(dict_explanation=output_res)]
+                else:
+                    res.output_explanation = [ComputedExplanation(str_explanation=output_res)]
         return res
 
+    def compare_fw_rules(self, fw_rules1, fw_rules2):
+        conn_props1 = ConnectionSet.fw_rules_to_conn_props(fw_rules1, self.config.peer_container)
+        conn_props2 = ConnectionSet.fw_rules_to_conn_props(fw_rules2, self.config.peer_container)
+        if conn_props1 == conn_props2:
+            print("Original and optimized fw-rules are semantically equivalent")
+        else:
+            diff_prop = (conn_props1 - conn_props2) | (conn_props2 - conn_props1)
+            if diff_prop.are_auto_conns():
+                print("Original and optimized fw-rules differ only in auto-connections")
+            else:
+                print("Error: original and optimized fw-rules are different")
+                assert False
+
     def get_connectivity_output_full(self, connections, peers, peers_to_compare):
         """
         get the connectivity map output considering all connections in the output
         :param dict connections: the connections' dict (map from connection-set to peer pairs)
-        :param PeerSet peers: the peers to consider for dot output
+        :param PeerSet peers: the peers to consider for dot and txt_no_fw_rules output
         :param PeerSet peers_to_compare: the peers to consider for fw-rules output
-        :rtype Union[str,dict]
+        :rtype (Union[str,dict], MinimizeFWRules)
         """
         if self.output_config.outputFormat in ['dot', 'jpg']:
             dot_full = self.dot_format_from_connections_dict(connections, peers)
-            return dot_full
-        # handle formats other than dot
-        formatted_rules = self.fw_rules_from_connections_dict(connections, peers_to_compare)
-        return formatted_rules
+            return dot_full, None
+        if self.output_config.outputFormat == 'txt_no_fw_rules':
+            conns_wo_fw_rules = self._txt_no_fw_rules_format_from_connections_dict(connections, peers)
+            return conns_wo_fw_rules, None
+        # handle other formats
+        formatted_rules, fw_rules = self.fw_rules_from_connections_dict(connections, peers_to_compare)
+        return formatted_rules, fw_rules
+
+    def get_props_output_full(self, props, peers_to_compare):
+        """
+        get the connectivity map output considering all connections in the output
+        :param ConnectivityProperties props: properties describing allowed connections
+        :param PeerSet peers_to_compare: the peers to consider for dot/fw-rules output
+         whereas all other values should be filtered out in the output
+        :rtype ([Union[str, dict], MinimizeFWRules])
+        """
+        if self.output_config.outputFormat in ['dot', 'jpg']:
+            dot_full = self.dot_format_from_props(props, peers_to_compare)
+            return dot_full, None
+        if self.output_config.outputFormat == 'txt_no_fw_rules':
+            conns_wo_fw_rules = self.txt_no_fw_rules_format_from_props(props, peers_to_compare)
+            return conns_wo_fw_rules, None
+        # handle other formats
+        formatted_rules, fw_rules = self.fw_rules_from_props(props, peers_to_compare)
+        return formatted_rules, fw_rules
 
     def get_connectivity_output_split_by_tcp(self, connections, peers, peers_to_compare):
         """
         get the connectivity map output as two parts: TCP and non-TCP
         :param dict connections: the connections' dict (map from connection-set to peer pairs)
         :param PeerSet peers: the peers to consider for dot output
         :param PeerSet peers_to_compare: the peers to consider for fw-rules output
-        :rtype Union[str,dict]
+        :rtype (Union[str, dict], MinimizeFWRules, MinimizeFWRules)
         """
         connectivity_tcp_str = 'TCP'
         connectivity_non_tcp_str = 'non-TCP'
         connections_tcp, connections_non_tcp = self.convert_connections_to_split_by_tcp(connections)
         if self.output_config.outputFormat in ['dot', 'jpg']:
             dot_tcp = self.dot_format_from_connections_dict(connections_tcp, peers, connectivity_tcp_str)
             dot_non_tcp = self.dot_format_from_connections_dict(connections_non_tcp, peers, connectivity_non_tcp_str)
             # concatenate the two graphs into one dot file
             res_str = dot_tcp + dot_non_tcp
-            return res_str
-        # handle formats other than dot
-        formatted_rules_tcp = self.fw_rules_from_connections_dict(connections_tcp, peers_to_compare,
-                                                                  connectivity_tcp_str)
-        formatted_rules_non_tcp = self.fw_rules_from_connections_dict(connections_non_tcp, peers_to_compare,
-                                                                      connectivity_non_tcp_str)
+            return res_str, None, None
+
+        if self.output_config.outputFormat == 'txt_no_fw_rules':
+            conns_msg_suffix = ' Connections:'
+            tcp_conns_wo_fw_rules = \
+                self._txt_no_fw_rules_format_from_connections_dict(connections_tcp, peers,
+                                                                   connectivity_tcp_str + conns_msg_suffix)
+            non_tcp_conns_wo_fw_rules = \
+                self._txt_no_fw_rules_format_from_connections_dict(connections_non_tcp, peers,
+                                                                   connectivity_non_tcp_str + conns_msg_suffix)
+            return tcp_conns_wo_fw_rules + '\n\n' + non_tcp_conns_wo_fw_rules, None, None
+        # handle formats other than dot and txt_no_fw_rules
+        formatted_rules_tcp, fw_rules_tcp = \
+            self.fw_rules_from_connections_dict(connections_tcp, peers_to_compare, connectivity_tcp_str)
+        formatted_rules_non_tcp, fw_rules_non_tcp = \
+            self.fw_rules_from_connections_dict(connections_non_tcp, peers_to_compare, connectivity_non_tcp_str)
         if self.output_config.outputFormat in ['json', 'yaml']:
             # get a dict object containing the two maps on different keys (TCP_rules and non-TCP_rules)
             rules = formatted_rules_tcp
             rules.update(formatted_rules_non_tcp)
-            return rules
+            return rules, fw_rules_tcp, fw_rules_non_tcp
         # remaining formats: txt / csv / md : concatenate the two strings of the conn-maps
         if self.output_config.outputFormat == 'txt':
             res_str = f'{formatted_rules_tcp}\n{formatted_rules_non_tcp}'
         else:
             res_str = formatted_rules_tcp + formatted_rules_non_tcp
-        return res_str
+        return res_str, fw_rules_tcp, fw_rules_non_tcp
+
+    def get_props_output_split_by_tcp(self, props, peers_to_compare):
+        """
+        get the connectivity map output as two parts: TCP and non-TCP
+        :param ConnectivityProperties props: properties describing allowed connections
+        :param PeerSet peers_to_compare: the peers to consider for dot/fw-rules output
+         whereas all other values should be filtered out in the output
+        :rtype (Union[str, dict], MinimizeFWRules, MinimizeFWRules)
+        """
+        connectivity_tcp_str = 'TCP'
+        connectivity_non_tcp_str = 'non-TCP'
+        props_tcp, props_non_tcp = self.convert_props_to_split_by_tcp(props)
+        if self.output_config.outputFormat in ['dot', 'jpg']:
+            dot_tcp = self.dot_format_from_props(props_tcp, peers_to_compare, connectivity_tcp_str)
+            dot_non_tcp = self.dot_format_from_props(props_non_tcp, peers_to_compare, connectivity_non_tcp_str)
+            # concatenate the two graphs into one dot file
+            res_str = dot_tcp + dot_non_tcp
+            return res_str, None, None
+        if self.output_config.outputFormat in ['txt_no_fw_rules']:
+            txt_no_fw_rules_tcp = self.txt_no_fw_rules_format_from_props(props_tcp, peers_to_compare, connectivity_tcp_str)
+            txt_no_fw_rules_non_tcp = self.txt_no_fw_rules_format_from_props(props_non_tcp, peers_to_compare,
+                                                                             connectivity_non_tcp_str)
+            res_str = txt_no_fw_rules_tcp + txt_no_fw_rules_non_tcp
+            return res_str, None, None
+        # handle formats other than dot and txt_no_fw_rules
+        formatted_rules_tcp, fw_rules_tcp = self.fw_rules_from_props(props_tcp, peers_to_compare, connectivity_tcp_str)
+        formatted_rules_non_tcp, fw_rules_non_tcp = self.fw_rules_from_props(props_non_tcp, peers_to_compare,
+                                                                             connectivity_non_tcp_str)
+        if self.output_config.outputFormat in ['json', 'yaml']:
+            # get a dict object containing the two maps on different keys (TCP_rules and non-TCP_rules)
+            rules = formatted_rules_tcp
+            rules.update(formatted_rules_non_tcp)
+            return rules, fw_rules_tcp, fw_rules_non_tcp
+        # remaining formats: txt / csv / md : concatenate the two strings of the conn-maps
+        if self.output_config.outputFormat == 'txt':
+            res_str = f'{formatted_rules_tcp}\n{formatted_rules_non_tcp}'
+        else:
+            res_str = formatted_rules_tcp + formatted_rules_non_tcp
+        return res_str, fw_rules_tcp, fw_rules_non_tcp
+
+    def _get_conn_graph(self, connections, peers):
+        """
+        :param dict connections: the connections' dict (map from connection-set to peer pairs)
+        :param PeerSet peers: the peers to consider for building connectivity graph
+        :rtype:  ConnectivityGraph
+        :return the connectivity graph of the given connections and peers
+        """
+        conn_graph = ConnectivityGraph(peers, self.config.get_allowed_labels(), self.output_config)
+        conn_graph.add_edges(connections)
+        return conn_graph
+
+    def _txt_no_fw_rules_format_from_connections_dict(self, connections, peers, connectivity_restriction=None):
+        """
+        :param dict connections: the connections' dict (map from connection-set to peer pairs)
+        :param PeerSet peers: the peers to consider for dot output
+        :param Union[str,None] connectivity_restriction: specify if connectivity is restricted to TCP / non-TCP , or not
+        :rtype:  str
+        :return the connectivity map in txt_no_fw_rules format: the connections between peers excluding connections between
+        workload to itself (without grouping as fw-rules).
+        """
+        conn_graph = self._get_conn_graph(connections, peers)
+        return conn_graph.get_connections_without_fw_rules_txt_format(connectivity_restriction)
 
     def dot_format_from_connections_dict(self, connections, peers, connectivity_restriction=None):
         """
         :param dict connections: the connections' dict (map from connection-set to peer pairs)
         :param PeerSet peers: the peers to consider for dot output
         :param Union[str,None] connectivity_restriction: specify if connectivity is restricted to
                TCP / non-TCP , or not
         :rtype str
         :return the connectivity map in dot-format, considering connectivity_restriction if required
         """
+        conn_graph = self._get_conn_graph(connections, peers)
+        return conn_graph.get_connectivity_dot_format_str(connectivity_restriction)
+
+    def dot_format_from_props(self, props, peers, connectivity_restriction=None):
+        """
+        :param ConnectivityProperties props: properties describing allowed connections
+        :param PeerSet peers: the peers to consider for dot output
+         whereas all other values should be filtered out in the output
+        :param Union[str,None] connectivity_restriction: specify if connectivity is restricted to
+               TCP / non-TCP , or not
+        :rtype str
+        :return the connectivity map in dot-format, considering connectivity_restriction if required
+        """
         conn_graph = ConnectivityGraph(peers, self.config.get_allowed_labels(), self.output_config)
-        conn_graph.add_edges(connections)
+        for cube in props:
+            conn_graph.add_edges_from_cube_dict(props.get_connectivity_cube(cube), self.config.peer_container)
         return conn_graph.get_connectivity_dot_format_str(connectivity_restriction)
 
+    def txt_no_fw_rules_format_from_props(self, props, peers, connectivity_restriction=None):
+        """
+        :param ConnectivityProperties props: properties describing allowed connections
+        :param PeerSet peers: the peers to consider for dot output
+        :param Union[str,None] connectivity_restriction: specify if connectivity is restricted to
+               TCP / non-TCP , or not
+        :rtype str
+        :return the connectivity map in txt_no_fw_rules format, considering connectivity_restriction if required
+        """
+        conn_graph = ConnectivityGraph(peers, self.config.get_allowed_labels(), self.output_config)
+        for cube in props:
+            conn_graph.add_edges_from_cube_dict(props.get_connectivity_cube(cube), self.config.peer_container)
+        return conn_graph.get_connections_without_fw_rules_txt_format(connectivity_restriction)
+
     def fw_rules_from_connections_dict(self, connections, peers_to_compare, connectivity_restriction=None):
         """
         :param dict connections: the connections' dict (map from connection-set to peer pairs)
         :param PeerSet peers_to_compare: the peers to consider for fw-rules output
         :param Union[str,None] connectivity_restriction: specify if connectivity is restricted to
                TCP / non-TCP , or not
         :return the connectivity map in fw-rules, considering connectivity_restriction if required
-        :rtype: Union[str, dict]
+        :rtype: (Union[str, dict], MinimizeFWRules)
         """
-        conn_graph = ConnectivityGraph(peers_to_compare, self.config.get_allowed_labels(), self.output_config)
-        conn_graph.add_edges(connections)
+        conn_graph = self._get_conn_graph(connections, peers_to_compare)
         fw_rules = conn_graph.get_minimized_firewall_rules()
         formatted_rules = fw_rules.get_fw_rules_in_required_format(connectivity_restriction=connectivity_restriction)
-        return formatted_rules
+        return formatted_rules, fw_rules
+
+    def fw_rules_from_props(self, props, peers_to_compare, connectivity_restriction=None):
+        """
+        :param ConnectivityProperties props: properties describing allowed connections
+        :param PeerSet peers_to_compare: the peers to consider for fw-rules output
+         whereas all other values should be filtered out in the output
+        :param Union[str,None] connectivity_restriction: specify if connectivity is restricted to
+               TCP / non-TCP , or not
+        :return the connectivity map in fw-rules, considering connectivity_restriction if required
+        :rtype: (Union[str, dict], MinimizeFWRules)
+        """
+        cluster_info = ClusterInfo(peers_to_compare, self.config.get_allowed_labels())
+        fw_rules_map = ConnectionSet.conn_props_to_fw_rules(props, cluster_info, self.config.peer_container,
+                                                            connectivity_restriction)
+        fw_rules = MinimizeFWRules(fw_rules_map, cluster_info, self.output_config, {})
+        formatted_rules = fw_rules.get_fw_rules_in_required_format(connectivity_restriction=connectivity_restriction)
+        return formatted_rules, fw_rules
 
     def convert_connections_to_split_by_tcp(self, connections):
         """
         given the connections' dict , convert it to two connection maps, one for TCP only, and the other
         for non-TCP only.
         :param dict connections: the connections' dict (map from connection-set to peer pairs)
         :return: a tuple of the two connection maps : first for TCP, second for non-TCP
@@ -824,14 +1123,28 @@
         if non_tcp_conns == ConnectionSet.get_non_tcp_connections():
             non_tcp_conns = ConnectionSet(True)  # all connections in terms of non-TCP
         if tcp_conns == ConnectionSet.get_all_tcp_connections():
             tcp_conns = ConnectionSet(True)  # all connections in terms of TCP
 
         return tcp_conns, non_tcp_conns
 
+    @staticmethod
+    def convert_props_to_split_by_tcp(props):
+        """
+        given the ConnectivityProperties properties set, convert it to two properties sets, one for TCP only, and the other
+        for non-TCP only.
+        :param ConnectivityProperties props: properties describing allowed connections
+        :return: a tuple of the two properties sets: first for TCP, second for non-TCP
+        :rtype: tuple(ConnectivityProperties, ConnectivityProperties)
+        """
+        tcp_protocol = ProtocolSet.get_protocol_set_with_single_protocol('TCP')
+        tcp_props = props & ConnectivityProperties.make_conn_props_from_dict({"protocols": tcp_protocol})
+        non_tcp_props = props - tcp_props
+        return tcp_props, non_tcp_props
+
 
 class TwoNetworkConfigsQuery(BaseNetworkQuery):
     """
     A base class for queries that inspect two network configs
     """
 
     def __init__(self, config1, config2, output_config_obj=None):
@@ -875,17 +1188,44 @@
     def disjoint_referenced_ip_blocks(self):
         """
         Returns disjoint ip-blocks in the policies of both configs
         :return: A set of disjoint ip-blocks
         :rtype: PeerSet
         """
         exclude_ipv6 = self.output_config.excludeIPv6Range
+        # TODO - consider including also non referenced IPBlocks, as in ConnectivityMapQuery
+        #  (see issue https://github.com/IBM/network-config-analyzer/issues/522)
         return IpBlock.disjoint_ip_blocks(self.config1.get_referenced_ip_blocks(exclude_ipv6),
                                           self.config2.get_referenced_ip_blocks(exclude_ipv6), exclude_ipv6)
 
+    def filter_conns_by_input_or_internal_constraints(self, conns1, conns2):
+        """
+        Given two allowed connections (in config1 and in config2 respectively), filter those connections
+        according to required IP blocks (external constrain - excludeIPv6Range option) and
+        peer types (internal constraints).
+        :param conns1: the first config allowed connections
+        :param conns2: the second config allowed connections
+        :rtype: [ConnectivityProperties, ConnectivityProperties]
+        :return: two resulting allowed connections
+        """
+        peers_to_compare = conns1.project_on_one_dimension('src_peers') | conns1.project_on_one_dimension('dst_peers') | \
+            conns2.project_on_one_dimension('src_peers') | conns2.project_on_one_dimension('dst_peers')
+        exclude_ipv6 = self.output_config.excludeIPv6Range
+        ref_ip_blocks = self.config1.get_referenced_ip_blocks(exclude_ipv6) | \
+            self.config2.get_referenced_ip_blocks(exclude_ipv6)
+        ip_blocks_mask = IpBlock() if ref_ip_blocks else IpBlock.get_all_ips_block(exclude_ipv6)
+        for ip_block in ref_ip_blocks:
+            ip_blocks_mask |= ip_block
+        peers_to_compare.filter_ipv6_blocks(ip_blocks_mask)
+        conns_filter = ConnectivityProperties.make_conn_props_from_dict({"src_peers": peers_to_compare,
+                                                                         "dst_peers": peers_to_compare})
+        res_conns1 = self.config1.filter_conns_by_peer_types(conns1, peers_to_compare) & conns_filter
+        res_conns2 = self.config2.filter_conns_by_peer_types(conns2, peers_to_compare) & conns_filter
+        return res_conns1, res_conns2
+
     @staticmethod
     def clone_without_ingress(config):
         """
         Clone config without ingress policies
         :param NetworkConfig config: the config to clone
         :return: resulting config without ingress policies
         :rtype: NetworkConfig
@@ -917,36 +1257,87 @@
         return QueryType.PairComparisonQuery
 
     def exec(self, cmd_line_flag=False, layer_name=None):
         query_answer = self.is_identical_topologies(True)
         if query_answer.output_result:
             query_answer.numerical_result = not query_answer.bool_result
             return query_answer
+        if self.config1.optimized_run == 'false':
+            return self.check_equivalence_original(layer_name)
+        else:
+            return self.check_equivalence_optimized(layer_name)
 
-        peers_to_compare = self.config1.peer_container.get_all_peers_group()
+    def check_equivalence_original(self, layer_name=None):
+        peers_to_compare = \
+            self.config1.peer_container.get_all_peers_group(include_dns_entries=True)
         peers_to_compare |= self.disjoint_referenced_ip_blocks()
         captured_pods = self.config1.get_captured_pods(layer_name) | self.config2.get_captured_pods(layer_name)
         different_conns_list = []
         for peer1 in peers_to_compare:
             for peer2 in peers_to_compare if peer1 in captured_pods else captured_pods:
                 if peer1 == peer2:
                     continue
+                if not self.determine_whether_to_compute_allowed_conns_for_peer_types(peer1, peer2):
+                    continue
                 conns1, _, _, _ = self.config1.allowed_connections(peer1, peer2, layer_name)
                 conns2, _, _, _ = self.config2.allowed_connections(peer1, peer2, layer_name)
                 if conns1 != conns2:
                     different_conns_list.append(PeersAndConnections(str(peer1), str(peer2), conns1, conns2))
                     if not self.output_config.fullExplanation:
                         return self._query_answer_with_relevant_explanation(different_conns_list)
 
         if different_conns_list:
             return self._query_answer_with_relevant_explanation(sorted(different_conns_list))
 
         return QueryAnswer(True, self.name1 + ' and ' + self.name2 + ' are semantically equivalent.',
                            numerical_result=0)
 
+    def _append_different_conns_to_list(self, conn_props, different_conns_list, props_based_on_config1):
+        """
+        Adds difference between config1 and config2 connectivities into the list of differences
+        :param ConnectivityProperties conn_props: connectivity properties representing a difference between config1 and config2
+        :param list different_conns_list: the list to add differences to
+        :param bool props_based_on_config1: whether conn_props represent connections present in config1 but not in config2
+        (the value True) or connections present in config2 but not in config1 (the value False)
+        """
+        no_conns = ConnectionSet()
+        for cube in conn_props:
+            conn_cube = conn_props.get_connectivity_cube(cube)
+            conns, src_peers, dst_peers = \
+                ConnectionSet.get_connection_set_and_peers_from_cube(conn_cube, self.config1.peer_container)
+            conns1 = conns if props_based_on_config1 else no_conns
+            conns2 = no_conns if props_based_on_config1 else conns
+            if self.output_config.fullExplanation:
+                if self.config1.optimized_run == 'true':
+                    different_conns_list.append(PeersAndConnections(str(src_peers), str(dst_peers), conns1, conns2))
+                else:  # 'debug': produce the same output format as in the original implementation (per peer pairs)
+                    for src_peer in src_peers:
+                        for dst_peer in dst_peers:
+                            if src_peer != dst_peer:
+                                different_conns_list.append(PeersAndConnections(str(src_peer), str(dst_peer),
+                                                                                conns1, conns2))
+            else:
+                different_conns_list.append(PeersAndConnections(src_peers.rep(), dst_peers.rep(), conns1, conns2))
+
+    def check_equivalence_optimized(self, layer_name=None):
+        conn_props1 = self.config1.allowed_connections_optimized(layer_name)
+        conn_props2 = self.config2.allowed_connections_optimized(layer_name)
+        all_conns1, all_conns2 = self.filter_conns_by_input_or_internal_constraints(conn_props1.all_allowed_conns,
+                                                                                    conn_props2.all_allowed_conns)
+        if all_conns1 == all_conns2:
+            return QueryAnswer(True, self.name1 + ' and ' + self.name2 + ' are semantically equivalent.',
+                               numerical_result=0)
+
+        conns1_not_in_conns2 = all_conns1 - all_conns2
+        conns2_not_in_conns1 = all_conns2 - all_conns1
+        different_conns_list = []
+        self._append_different_conns_to_list(conns1_not_in_conns2, different_conns_list, True)
+        self._append_different_conns_to_list(conns2_not_in_conns1, different_conns_list, False)
+        return self._query_answer_with_relevant_explanation(sorted(different_conns_list))
+
     def _query_answer_with_relevant_explanation(self, explanation_list):
         output_result = self.name1 + ' and ' + self.name2 + ' are not semantically equivalent.'
         explanation_description = f'Connections allowed in {self.name1} which are different in {self.name2}'
         final_explanation = ConnectionsDiffExplanation(explanation_description=explanation_description,
                                                        peers_diff_connections_list=explanation_list,
                                                        configs=self.get_configs_names(), conns_diff=True)
         return QueryAnswer(False, output_result, output_explanation=[final_explanation], numerical_result=1)
@@ -959,15 +1350,15 @@
 
     @staticmethod
     def get_query_type():
         return QueryType.PairComparisonQuery
 
     @staticmethod
     def get_supported_output_formats():
-        return {'txt', 'yaml', 'csv', 'md', 'json'}
+        return {'txt', 'yaml', 'csv', 'md', 'json', 'txt_no_fw_rules'}
 
     @staticmethod
     def _get_updated_key(key, is_added):
         """
         updates given key if needed, by replacing Changed with Added/ Removed based on the is_added flag value
         :param str key: a key string describing connectivity changes
         :param bool is_added: a bool flag indicating if connections are added or removed
@@ -1002,23 +1393,27 @@
         :param bool is_first_connectivity_result: flag indicating if this is the first connectivity fw-rules computation
                for the current semantic-diff query
         :return the computedExplanation of the current key and conn_graph considering the outputFormat
         :rtype: ComputedExplanation
         """
         updated_key = self._get_updated_key(key, is_added)
         topology_config_name = self.name2 if is_added else self.name1
-        conn_graph_explanation = self.get_explanation_from_conn_graph(conn_graph, is_first_connectivity_result)
+        connectivity_changes_header = f'{updated_key} (based on topology from config: {topology_config_name}) :'
+        if self.output_config.outputFormat == 'txt_no_fw_rules':
+            conn_graph_explanation = conn_graph.get_connections_without_fw_rules_txt_format(
+                connectivity_changes_header, exclude_self_loop_conns=False) + '\n'
+        else:
+            conn_graph_explanation = self.get_explanation_from_conn_graph(conn_graph, is_first_connectivity_result)
 
         if self.output_config.outputFormat in ['json', 'yaml']:
             explanation_dict = {'description': updated_key}
             explanation_dict.update(conn_graph_explanation)
             key_explanation = ComputedExplanation(dict_explanation=explanation_dict)
         else:
-            str_explanation = f'\n{updated_key} (based on topology from config: {topology_config_name}) :\n' \
-                if self.output_config.outputFormat == 'txt' else ''
+            str_explanation = f'\n{connectivity_changes_header}\n' if self.output_config.outputFormat == 'txt' else ''
             str_explanation += conn_graph_explanation
             key_explanation = ComputedExplanation(str_explanation=str_explanation)
 
         return key_explanation
 
     def get_results_for_computed_fw_rules(self, keys_list, conn_graph_removed_per_key, conn_graph_added_per_key):
         """
@@ -1049,22 +1444,22 @@
                     explanation.append(self.compute_explanation_for_key(key, False, conn_graph_removed_conns, res == 0))
                 res += 1
 
         return res, explanation
 
     def get_conn_graph_changed_conns(self, key, ip_blocks, is_added):
         """
-        create a ConnectivityGraph for chnged (added/removed) connections per given key
+        create a ConnectivityGraph for changed (added/removed) connections per given key
         :param key: the key (category) of changed connections
         :param ip_blocks: a PeerSet of ip-blocks to be added for the topology peers
         :param is_added: a bool flag indicating if connections are added or removed
         :return: a ConnectivityGraph object
         """
-        old_peers = self.config1.peer_container.get_all_peers_group()
-        new_peers = self.config2.peer_container.get_all_peers_group()
+        old_peers = self.config1.peer_container.get_all_peers_group(include_dns_entries=True)
+        new_peers = self.config2.peer_container.get_all_peers_group(include_dns_entries=True)
         allowed_labels = (self.config1.get_allowed_labels()).union(self.config2.get_allowed_labels())
         topology_peers = new_peers | ip_blocks if is_added else old_peers | ip_blocks
         # following query_name update is for adding query line descriptions for csv and md formats
         updated_key = self._get_updated_key(key, is_added)
         if self.output_config.queryName:
             query_name = f'semantic_diff, config1: {self.config1.name}, config2: {self.config2.name}, key: {updated_key}'
         else:
@@ -1093,16 +1488,16 @@
         Some sections might be empty and can be dropped.
 
         :return:
         res (int): number of categories with diffs
         explanation (list): list of diff explanations - one for each category
         :rtype: int, list[ComputedExplanation]
         """
-        old_peers = self.config1.peer_container.get_all_peers_group()
-        new_peers = self.config2.peer_container.get_all_peers_group()
+        old_peers = self.config1.peer_container.get_all_peers_group(include_dns_entries=True)
+        new_peers = self.config2.peer_container.get_all_peers_group(include_dns_entries=True)
         intersected_peers = old_peers & new_peers
         removed_peers = old_peers - intersected_peers
         added_peers = new_peers - intersected_peers
         captured_pods = (self.config1.get_captured_pods() | self.config2.get_captured_pods()) & intersected_peers
         exclude_ipv6 = self.output_config.excludeIPv6Range
         old_ip_blocks = IpBlock.disjoint_ip_blocks(self.config1.get_referenced_ip_blocks(exclude_ipv6),
                                                    IpBlock.get_all_ips_block_peer_set(exclude_ipv6),
@@ -1117,111 +1512,135 @@
 
         # 1.1. lost connections between removed peers
         key = 'Lost connections between removed peers'
         keys_list.append(key)
         conn_graph_removed_per_key[key] = self.get_conn_graph_changed_conns(key, PeerSet(), False)
         conn_graph_added_per_key[key] = None
         for pair in itertools.permutations(removed_peers, 2):
+            if not self.determine_whether_to_compute_allowed_conns_for_peer_types(pair[0], pair[1]):
+                continue
             lost_conns, _, _, _ = self.config1.allowed_connections(pair[0], pair[1])
             if lost_conns:
                 conn_graph_removed_per_key[key].add_edge(pair[0], pair[1], lost_conns)
 
         # 1.2. lost connections between removed peers and ipBlocks
         key = 'Lost connections between removed peers and ipBlocks'
         keys_list.append(key)
         conn_graph_removed_per_key[key] = self.get_conn_graph_changed_conns(key, old_ip_blocks, False)
         conn_graph_added_per_key[key] = None
         for pair in itertools.product(removed_peers, old_ip_blocks):
+            if not self.determine_whether_to_compute_allowed_conns_for_peer_types(pair[0], pair[1]):
+                continue
             lost_conns, _, _, _ = self.config1.allowed_connections(pair[0], pair[1])
             if lost_conns:
                 conn_graph_removed_per_key[key].add_edge(pair[0], pair[1], lost_conns)
 
+            if not self.determine_whether_to_compute_allowed_conns_for_peer_types(pair[1], pair[0]):
+                continue
             lost_conns, _, _, _ = self.config1.allowed_connections(pair[1], pair[0])
             if lost_conns:
                 conn_graph_removed_per_key[key].add_edge(pair[1], pair[0], lost_conns)
 
         # 2.1. lost connections between removed peers and intersected peers
         key = 'Lost connections between removed peers and persistent peers'
         keys_list.append(key)
         conn_graph_removed_per_key[key] = self.get_conn_graph_changed_conns(key, PeerSet(), False)
         conn_graph_added_per_key[key] = None
         for pair in itertools.product(removed_peers, intersected_peers):
+            if not self.determine_whether_to_compute_allowed_conns_for_peer_types(pair[0], pair[1]):
+                continue
             lost_conns, _, _, _ = self.config1.allowed_connections(pair[0], pair[1])
             if lost_conns:
                 conn_graph_removed_per_key[key].add_edge(pair[0], pair[1], lost_conns)
 
+            if not self.determine_whether_to_compute_allowed_conns_for_peer_types(pair[1], pair[0]):
+                continue
             lost_conns, _, _, _ = self.config1.allowed_connections(pair[1], pair[0])
             if lost_conns:
                 conn_graph_removed_per_key[key].add_edge(pair[1], pair[0], lost_conns)
 
         # 3.1. lost/new connections between intersected peers due to changes in policies and labels of pods/namespaces
         key = 'Changed connections between persistent peers'
         keys_list.append(key)
         conn_graph_removed_per_key[key] = self.get_conn_graph_changed_conns(key, PeerSet(), False)
         conn_graph_added_per_key[key] = self.get_conn_graph_changed_conns(key, PeerSet(), True)
-        for pod1 in intersected_peers:
-            for pod2 in intersected_peers if pod1 in captured_pods else captured_pods:
-                if pod1 == pod2:
+        for peer1 in intersected_peers:
+            for peer2 in intersected_peers if peer1 in captured_pods else captured_pods:
+                if peer1 == peer2:
                     continue
-                old_conns, _, _, _ = self.config1.allowed_connections(pod1, pod2)
-                new_conns, _, _, _ = self.config2.allowed_connections(pod1, pod2)
+                if not self.determine_whether_to_compute_allowed_conns_for_peer_types(peer1, peer2):
+                    continue
+                old_conns, _, _, _ = self.config1.allowed_connections(peer1, peer2)
+                new_conns, _, _, _ = self.config2.allowed_connections(peer1, peer2)
                 if new_conns != old_conns:
-                    conn_graph_removed_per_key[key].add_edge(pod1, pod2, old_conns - new_conns)
-                    conn_graph_added_per_key[key].add_edge(pod1, pod2, new_conns - old_conns)
+                    conn_graph_removed_per_key[key].add_edge(peer1, peer2, old_conns - new_conns)
+                    conn_graph_added_per_key[key].add_edge(peer1, peer2, new_conns - old_conns)
 
         # 3.2. lost/new connections between intersected peers and ipBlocks due to changes in policies and labels
         key = 'Changed connections between persistent peers and ipBlocks'
         disjoint_ip_blocks = IpBlock.disjoint_ip_blocks(old_ip_blocks, new_ip_blocks, exclude_ipv6)
         peers = captured_pods | disjoint_ip_blocks
         keys_list.append(key)
         conn_graph_removed_per_key[key] = self.get_conn_graph_changed_conns(key, disjoint_ip_blocks, False)
         conn_graph_added_per_key[key] = self.get_conn_graph_changed_conns(key, disjoint_ip_blocks, True)
-        for pod1 in peers:
-            for pod2 in disjoint_ip_blocks if pod1 in captured_pods else captured_pods:
-                old_conns, _, _, _ = self.config1.allowed_connections(pod1, pod2)
-                new_conns, _, _, _ = self.config2.allowed_connections(pod1, pod2)
+        for peer1 in peers:
+            for peer2 in disjoint_ip_blocks if peer1 in captured_pods else captured_pods:
+                if not self.determine_whether_to_compute_allowed_conns_for_peer_types(peer1, peer2):
+                    continue
+                old_conns, _, _, _ = self.config1.allowed_connections(peer1, peer2)
+                new_conns, _, _, _ = self.config2.allowed_connections(peer1, peer2)
                 if new_conns != old_conns:
-                    conn_graph_removed_per_key[key].add_edge(pod1, pod2, old_conns - new_conns)
-                    conn_graph_added_per_key[key].add_edge(pod1, pod2, new_conns - old_conns)
+                    conn_graph_removed_per_key[key].add_edge(peer1, peer2, old_conns - new_conns)
+                    conn_graph_added_per_key[key].add_edge(peer1, peer2, new_conns - old_conns)
 
         # 4.1. new connections between intersected peers and added peers
         key = 'New connections between persistent peers and added peers'
         keys_list.append(key)
         conn_graph_removed_per_key[key] = None
         conn_graph_added_per_key[key] = self.get_conn_graph_changed_conns(key, PeerSet(), True)
         for pair in itertools.product(intersected_peers, added_peers):
+            if not self.determine_whether_to_compute_allowed_conns_for_peer_types(pair[0], pair[1]):
+                continue
             new_conns, _, _, _ = self.config2.allowed_connections(pair[0], pair[1])
             if new_conns:
                 conn_graph_added_per_key[key].add_edge(pair[0], pair[1], new_conns)
 
+            if not self.determine_whether_to_compute_allowed_conns_for_peer_types(pair[1], pair[0]):
+                continue
             new_conns, _, _, _ = self.config2.allowed_connections(pair[1], pair[0])
             if new_conns:
                 conn_graph_added_per_key[key].add_edge(pair[1], pair[0], new_conns)
 
         # 5.1. new connections between added peers
         key = 'New connections between added peers'
         keys_list.append(key)
         conn_graph_removed_per_key[key] = None
         conn_graph_added_per_key[key] = self.get_conn_graph_changed_conns(key, PeerSet(), True)
         for pair in itertools.permutations(added_peers, 2):
+            if not self.determine_whether_to_compute_allowed_conns_for_peer_types(pair[0], pair[1]):
+                continue
             new_conns, _, _, _ = self.config2.allowed_connections(pair[0], pair[1])
             if new_conns:
                 conn_graph_added_per_key[key].add_edge(pair[0], pair[1], new_conns)
 
         # 5.2. new connections between added peers and ipBlocks
         key = 'New connections between added peers and ipBlocks'
         keys_list.append(key)
         conn_graph_removed_per_key[key] = None
         conn_graph_added_per_key[key] = self.get_conn_graph_changed_conns(key, new_ip_blocks, True)
 
         for pair in itertools.product(added_peers, new_ip_blocks):
+            if not self.determine_whether_to_compute_allowed_conns_for_peer_types(pair[0], pair[1]):
+                continue
             new_conns, _, _, _ = self.config2.allowed_connections(pair[0], pair[1])
             if new_conns:
                 conn_graph_added_per_key[key].add_edge(pair[0], pair[1], new_conns)
 
+            if not self.determine_whether_to_compute_allowed_conns_for_peer_types(pair[1], pair[0]):
+                continue
             new_conns, _, _, _ = self.config2.allowed_connections(pair[1], pair[0])
             if new_conns:
                 conn_graph_added_per_key[key].add_edge(pair[1], pair[0], new_conns)
 
         return self.get_results_for_computed_fw_rules(keys_list, conn_graph_removed_per_key,
                                                       conn_graph_added_per_key)
 
@@ -1288,31 +1707,34 @@
 
 class ContainmentQuery(TwoNetworkConfigsQuery):
     """
     Checking whether the connections allowed by config1 are contained in those allowed by config2
     """
 
     def exec(self, cmd_line_flag=False, only_captured=False):
-        config1_peers = self.config1.peer_container.get_all_peers_group()
-        peers_in_config1_not_in_config2 = config1_peers - self.config2.peer_container.get_all_peers_group()
+        config1_peers = self.config1.peer_container.get_all_peers_group(include_dns_entries=True)
+        peers_in_config1_not_in_config2 = config1_peers - \
+            self.config2.peer_container.get_all_peers_group(include_dns_entries=True)
         if peers_in_config1_not_in_config2:
             peers_list = [str(e) for e in peers_in_config1_not_in_config2]
             final_explanation = \
-                PodsListsExplanations(explanation_description=f'Pods in {self.name1} which are not in {self.name2}',
+                PodsListsExplanations(explanation_description=f'Peers in {self.name1} which are not in {self.name2}',
                                       pods_list=sorted(peers_list))
             return QueryAnswer(False, f'{self.name1} is not contained in {self.name2} ',
                                output_explanation=[final_explanation], numerical_result=0 if not cmd_line_flag else 1)
 
         peers_to_compare = config1_peers | self.disjoint_referenced_ip_blocks()
         captured_pods = self.config1.get_captured_pods() | self.config2.get_captured_pods()
         not_contained_list = []
         for peer1 in peers_to_compare:
             for peer2 in peers_to_compare if peer1 in captured_pods else captured_pods:
                 if peer1 == peer2:
                     continue
+                if not self.determine_whether_to_compute_allowed_conns_for_peer_types(peer1, peer2):
+                    continue
                 conns1_all, captured1_flag, conns1_captured, _ = self.config1.allowed_connections(peer1, peer2)
                 if only_captured and not captured1_flag:
                     continue
                 conns1 = conns1_captured if only_captured else conns1_all
                 conns2, _, _, _ = self.config2.allowed_connections(peer1, peer2)
                 if not conns1.contained_in(conns2):
                     not_contained_list.append(PeersAndConnections(str(peer1), str(peer2), conns1))
@@ -1420,23 +1842,25 @@
     def exec(self, cmd_line_flag):
         query_answer = self.is_identical_topologies()
         if query_answer.output_result:
             query_answer.numerical_result = query_answer.bool_result if not cmd_line_flag \
                 else not query_answer.bool_result
             return query_answer
 
-        peers_to_compare = self.config2.peer_container.get_all_peers_group()
+        peers_to_compare = \
+            self.config2.peer_container.get_all_peers_group(include_dns_entries=True)
         peers_to_compare |= self.disjoint_referenced_ip_blocks()
         captured_pods = self.config2.get_captured_pods() | self.config1.get_captured_pods()
         extended_conns_list = []
         for peer1 in peers_to_compare:
             for peer2 in peers_to_compare if peer1 in captured_pods else captured_pods:
                 if peer1 == peer2:
                     continue
-
+                if not self.determine_whether_to_compute_allowed_conns_for_peer_types(peer1, peer2):
+                    continue
                 _, captured2_flag, conns2_captured, _ = self.config2.allowed_connections(peer1, peer2)
                 if not captured2_flag:
                     continue
                 _, captured1_flag, conns1_captured, _ = self.config1.allowed_connections(peer1, peer2)
                 if captured1_flag and not conns1_captured.contained_in(conns2_captured):
                     extended_conns_list.append(PeersAndConnections(str(peer1), str(peer2), conns1_captured,
                                                                    conns2_captured))
@@ -1475,22 +1899,25 @@
     """
 
     def exec(self, cmd_line_flag=False, only_captured=True):
         query_answer = self.is_identical_topologies()
         if query_answer.output_result:
             return query_answer
 
-        peers_to_compare = self.config1.peer_container.get_all_peers_group()
+        peers_to_compare = \
+            self.config1.peer_container.get_all_peers_group(include_dns_entries=True)
         peers_to_compare |= self.disjoint_referenced_ip_blocks()
         captured_pods = self.config1.get_captured_pods() | self.config2.get_captured_pods()
         intersect_connections_list = []
         for peer1 in peers_to_compare:
             for peer2 in peers_to_compare if peer1 in captured_pods else captured_pods:
                 if peer1 == peer2:
                     continue
+                if not self.determine_whether_to_compute_allowed_conns_for_peer_types(peer1, peer2):
+                    continue
                 conns1_all, captured1_flag, conns1_captured, _ = self.config1.allowed_connections(peer1, peer2)
                 if only_captured and not captured1_flag:
                     continue
                 conns1 = conns1_captured if only_captured else conns1_all
                 conns2, _, _, _ = self.config2.allowed_connections(peer1, peer2)
                 conns_in_both = conns2 & conns1
                 if bool(conns_in_both):
@@ -1559,14 +1986,15 @@
         returns the uncaptured ingress/egress pods set and its length for the given layer
         :param NetworkLayerName layer_name: the layer to check uncaptured pods in
         :param bool is_ingress: indicates if to check pods affected by ingress/egress
         :return: - number of uncaptured pod
                  - set of the uncaptured pods
         :rtype: (int,set[str])
         """
+        # get_all_peers_group() does not require getting dnsEntry peers, since they are not ClusterEP (pods)
         existing_pods = self.config.peer_container.get_all_peers_group()
         uncaptured_xgress_pods = existing_pods - self.config.get_affected_pods(is_ingress, layer_name)
         if not uncaptured_xgress_pods:
             return 0, set()
         uncaptured_resources = set(self._get_pod_name(pod) for pod in uncaptured_xgress_pods)  # no duplicate resources in set
         return len(uncaptured_resources), uncaptured_resources
 
@@ -1599,26 +2027,22 @@
                                                   pods_list=list(sorted(uncaptured_ingress_pods_set)),
                                                   egress_pods_list=list(sorted(uncaptured_egress_pods_set)),
                                                   add_xgress_suffix=True)
         return layer_explanation, layer_res
 
     def exec(self):
         self.output_config.fullExplanation = True  # assign true for this query - it is always ok to compare its results
+        # get_all_peers_group() does not require getting dnsEntry peers, since they are not ClusterEP (pods)
         existing_pods = self.config.peer_container.get_all_peers_group()
-        if not self.config:
+        if not self.config or self.config.policies_container.layers.does_contain_single_layer(NetworkLayerName.Ingress):
             return QueryAnswer(bool_result=False,
                                output_result=f'There are no network policies in {self.config.name}. '
                                              f'All workload resources are non captured',
                                numerical_result=len(existing_pods))
 
-        if self.config.policies_container.layers.does_contain_single_layer(NetworkLayerName.Ingress):
-            return QueryAnswer(bool_result=False,
-                               output_result='AllCapturedQuery cannot be applied using Ingress resources only',
-                               query_not_executed=True)
-
         k8s_calico_pods_list_explanation, k8s_calico_res = self._compute_uncaptured_pods_by_layer(NetworkLayerName.K8s_Calico)
         istio_pods_list_explanation, istio_res = self._compute_uncaptured_pods_by_layer(NetworkLayerName.Istio, True)
 
         if k8s_calico_res == 0 and istio_res == 0:
             output_str = f'All pods are captured by at least one policy in {self.config.name}'
             return QueryAnswer(bool_result=True, output_result=output_str, numerical_result=0)
```

### Comparing `network-config-analyzer-1.9.2/nca/NetworkConfig/NetworkConfigQueryRunner.py` & `network-config-analyzer-1.9.3/nca/NetworkConfig/NetworkConfigQueryRunner.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from dataclasses import dataclass, field
 import yaml
 
 from nca.Utils.OutputFilesFlags import OutputFilesFlags
 from nca.Resources.NetworkPolicy import NetworkPolicy
 from .NetworkConfig import NetworkConfig
 from . import NetworkConfigQuery
+from nca.Utils.ExplTracker import ExplTracker
 
 
 @dataclass
 class QueryResult:
     """
     A class for storing the intermediate results of running iterations of a query
     """
@@ -36,17 +37,17 @@
         self.num_not_executed += iteration_results[2]
 
     def compute_final_results(self, output_format):
         """
         extracts the final query results from self variables
         from self.query_iterations_output computes the final str output of the query,
         other results returned as is from query_result.
-        :param str output_format: the output format to form the final output
-        if output format is json, dumps the output list into one-top-leveled string
-        if output format is yaml, dumps the output list into str of a list of yaml objects
+        :param str output_format: the output format to form the final output.
+        if output format is json, dumps the output list into one-top-leveled string.
+        if output format is yaml, dumps the output list into str of a list of yaml objects.
         otherwise, writes the output list items split by \n
         :return the results: numerical result, output - str , num of not executed
         :rtype: int, str, int
         """
         if output_format == 'json':
             output = json.dumps(self.query_iterations_output, sort_keys=False, indent=2)
         elif output_format == 'yaml':
@@ -165,15 +166,20 @@
         query_to_exec = getattr(NetworkConfigQuery, query_type)(config1, config2, self.output_configuration)
         return query_to_exec.execute_and_compute_output_in_required_format(cmd_line_flag)
 
     def _run_query_for_each_config(self):
         query_result = QueryResult()
         for config in self.configs_array:
             query_result.update(self._execute_one_config_query(self.query_name, self._get_config(config)))
-        return query_result.compute_final_results(self.output_configuration.outputFormat)
+        expl_out = ''
+        if ExplTracker().is_active() and self.output_configuration.explain and \
+                ExplTracker().is_output_format_supported(self.output_configuration.outputFormat):
+            expl_out = '\n\nExplainability results:\n'+ExplTracker().explain(self.output_configuration.explain.split(','))
+        numerical_result, output, num_not_executed = query_result.compute_final_results(self.output_configuration.outputFormat)
+        return numerical_result, output + expl_out, num_not_executed
 
     def _run_query_on_configs_vs_base_config(self, cmd_line_flag):
         query_result = QueryResult()
         base_config = self._get_config(self.configs_array[0])
         for config in self.configs_array[1:]:
             query_result.update(self._execute_pair_configs_query(
                 self.query_name, self._get_config(config), base_config, cmd_line_flag))
```

### Comparing `network-config-analyzer-1.9.2/nca/NetworkConfig/PeerContainer.py` & `network-config-analyzer-1.9.3/nca/NetworkConfig/PeerContainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # Copyright 2020- IBM Inc. All rights reserved
 # SPDX-License-Identifier: Apache2.0
 #
-
+import re
 from sys import stderr
-from nca.CoreDS.Peer import PeerSet, Pod, IpBlock
+from nca.CoreDS.Peer import PeerSet, Pod, IpBlock, DNSEntry
 from nca.Resources.K8sNamespace import K8sNamespace
 from nca.Resources.K8sService import K8sService
 from nca.Parsers.GenericYamlParser import GenericYamlParser
 
 
 class PeerContainer:
     """
@@ -200,46 +200,76 @@
         """
         res = PeerSet()
         for service in self.services.values():
             if service.name == service_name:
                 res |= service.target_pods
         return res
 
+    def get_dns_entry_peers_matching_host_name(self, host_name):
+        """
+        returns all DNSentry peers which are equal/contained in the host_name
+        :param str host_name: the host name as it appears in the policy's hosts list
+        :rtype: PeerSet
+        """
+        res = PeerSet()
+        # re.fullmatch behavior in accordance with live-cluster behaviour.
+        # only sidecar host should contain the service-entry host.
+        # the opposite containment direction is not considered for connections
+        # (detailed examples in:
+        # tests/istio_testcases/example_policies/bookinfo-demo/sidecar_examples/bookinfo-test-sidecar-connectivity-scheme.yaml)
+        # queries: - connectivity-sidecar-host-name-does-not-contain-service-entry-hosts
+        # - connectivity-sidecar-host-name-contains-service-entry-hosts
+        host_pattern = DNSEntry.compute_re_pattern_from_host_name(host_name)
+        for peer in self.peer_set:
+            if isinstance(peer, DNSEntry) and (peer.name == host_name or re.fullmatch(host_pattern, peer.name)):
+                res.add(peer)
+        return res
+
     def get_pods_with_service_name_containing_given_string(self, name_substring):
         """
         Returns all pods that belong to services whose name contains the given substring
         :param str name_substring: the service name substring
         :return: PeerSet
         """
         res = PeerSet()
         for key, val in self.services.items():
             if name_substring in key:
                 res |= val.target_pods
         return res
 
-    def get_all_services_target_pods(self):
+    def get_all_services_target_peers(self):
         """
-        Returns all pods that belong to services
+        Returns all pods that belong to services and all DNSEntry peers (if exist) as this type of peers
+        is produced by ServiceEntry objects
         :rtype: PeerSet
         """
         res = PeerSet()
         for service in self.services.values():
             res |= service.target_pods
+        for peer in self.peer_set:
+            if isinstance(peer, DNSEntry):
+                res.add(peer)
         return res
 
-    def get_services_target_pods_in_namespace(self, namespace):
+    def get_services_target_peers_in_namespace(self, namespace):
         """
-        Returns all pods that belong to services in the given namespace
-        :param K8sNamespace namespace:   namespace object
+        Returns all peers that belong to services in/ exported to the given namespace
+        (i.e. pods that belong to k8s services in the given namespace,
+        or DNSEntry peers)
+        currently assuming DNSEntry peers are exported to all namespaces
+        :param K8sNamespace namespace: namespace object
         :rtype: PeerSet
         """
         res = PeerSet()
         for service in self.services.values():
             if service.namespace == namespace:
                 res |= service.target_pods
+        for peer in self.peer_set:
+            if isinstance(peer, DNSEntry):
+                res.add(peer)
         return res
 
     def get_pods_with_service_account_name(self, sa_name, namespace_str):
         """
         Return all pods that are with a service account name in a given namespace
         :param sa_name: string  the service account name
         :param namespace_str:  string  the namespace str
@@ -265,29 +295,39 @@
                     if peer.get_first_profile_name() == profile_name:
                         res.add(peer)
                 else:
                     if profile_name in peer.profiles:
                         res.add(peer)
         return res
 
-    def get_all_peers_group(self, add_external_ips=False, include_globals=True):
+    def get_all_peers_group(self, add_external_ips=False, include_globals=True, include_dns_entries=False):
         """
         Return all peers known in the system
         :param bool add_external_ips: Whether to also add the full range of ips
         :param bool include_globals: Whether to include global peers
+        :param bool include_dns_entries: Whether to include DNSEntry peers
         :return PeerSet: The required set of peers
         """
         res = PeerSet()
         for peer in self.peer_set:
+            if isinstance(peer, DNSEntry) and not include_dns_entries:
+                continue
             if include_globals or not peer.is_global_peer():
                 res.add(peer)
         if add_external_ips:
             res.add(IpBlock.get_all_ips_block())
         return res
 
+    def get_all_dns_entries(self):
+        res = PeerSet()
+        for peer in self.peer_set:
+            if isinstance(peer, DNSEntry):
+                res.add(peer)
+        return res
+
     def get_all_global_peers(self):
         """
         Return all global peers known in the system
         :return PeerSet: The required set of peers
         """
         res = PeerSet()
         for peer in self.peer_set:
```

### Comparing `network-config-analyzer-1.9.2/nca/NetworkConfig/QueryOutputHandler.py` & `network-config-analyzer-1.9.3/nca/NetworkConfig/QueryOutputHandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,26 +157,26 @@
         :param str prefix: indicates if rules types are ingress or egress
         :return the str form of the explanation dict
         :rtype: str
         """
         res = '\n' + self._get_xgress_description(prefix) + ':\n'
         for policy_title, rules_indexes_list in xgress_rules_dict.items():
             res += policy_title + ', ' + prefix + ' rules indexes: ' +\
-                   ', '.join(str(idx) for idx in rules_indexes_list) + '\n'
+                ', '.join(str(idx) for idx in rules_indexes_list) + '\n'
         return res
 
     def get_explanation_in_str(self):
         """
         returns self type of OutputExplanation written in str form
         :rtype: str
         """
         result = ''
         if self.policies_list:
             result += self._get_policies_description() + ':\n' +\
-                      ', '.join(self.policies_list) + '\n'
+                ', '.join(self.policies_list) + '\n'
         if self.policies_to_ingress_rules_dict:
             result += self._add_rules_to_str_explanation(self.policies_to_ingress_rules_dict)
         if self.policies_to_egress_rules_dict:
             result += self._add_rules_to_str_explanation(self.policies_to_egress_rules_dict, 'egress')
         return result
```

### Comparing `network-config-analyzer-1.9.2/nca/NetworkConfig/ResourcesHandler.py` & `network-config-analyzer-1.9.3/nca/NetworkConfig/ResourcesHandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from nca.FileScanners.GenericTreeScanner import TreeScannerFactory
 from nca.Utils.CmdlineRunner import CmdlineRunner
 from nca.Utils.NcaLogger import NcaLogger
 from .NetworkConfig import NetworkConfig
 from .PoliciesFinder import PoliciesFinder
 from .TopologyObjectsFinder import PodsFinder, NamespacesFinder, ServicesFinder
 from .PeerContainer import PeerContainer
+from nca.Utils.ExplTracker import ExplTracker
 
 
 class ResourceType(Enum):
     Unknown = 0
     Pods = 1
     Namespaces = 2
     Policies = 3
@@ -39,25 +40,25 @@
     """
 
     def __init__(self):
         self.global_peer_container = None
         self.global_pods_finder = None
         self.global_ns_finder = None
 
-    def set_global_peer_container(self, global_ns_list, global_pod_list, global_resource_list):
+    def set_global_peer_container(self, global_ns_list, global_pod_list, global_resource_list, optimized_run='false'):
         """
         builds the global peer container based on global input resources,
         it also saves the global pods and namespaces finder, to use in case specific configs missing one of them.
         Note: if there are no input resources at all, loads them from k8s live cluster
         :param Union[list[str], None] global_ns_list: global namespaces entries
         :param Union[list[str], None] global_pod_list: global pods entries
         :param Union[list[str], None] global_resource_list: list of global entries of namespaces/pods to handle
         in case specific list is None
         """
-        global_resources_parser = ResourcesParser()
+        global_resources_parser = ResourcesParser(optimized_run)
         self._set_config_peer_container(global_ns_list, global_pod_list, global_resource_list,
                                         'global', True, global_resources_parser)
 
     @staticmethod
     def livesim_information_message(elements_type):
         message = f'Found missing elements - adding complementary {elements_type} elements'
         NcaLogger().log_message(message, level='I')
@@ -117,38 +118,39 @@
             LiveSimPaths.IstioGwCfgPath, policy_finder.missing_istio_gw_pods_with_labels)
         if istio_gateway_added_resources:
             livesim_configuration_addons += istio_gateway_added_resources
             ResourcesHandler.livesim_information_message('Istio-ingress-gateway')
 
         return livesim_configuration_addons
 
-    def parse_elements(self, ns_list, pod_list, resource_list, config_name, save_flag, np_list):
+    def parse_elements(self, ns_list, pod_list, resource_list, config_name, save_flag, np_list, optimized_run):
         """
         Parse the elements and build peer container.
         :param Union[list[str], None] ns_list: namespaces entries
         :param Union[list[str], None] pod_list: pods and services entries
         :param Union[list[str], None] resource_list: entries to read pods/namespaces/policies from
         if the specific list is None
         :param str config_name: name of the config
         :param bool save_flag: used in cmdline queries with two configs, if save flag is True
          will save the peer container as global to use it for base config's peer resources in case are missing
         :param Union[list[str], None] np_list: networkPolicies entries
         :return:  PeerContainer, ResourcesParser, str
         """
-        resources_parser = ResourcesParser()
+        resources_parser = ResourcesParser(optimized_run)
         # build peer container
         peer_container = \
             self._set_config_peer_container(ns_list, pod_list, resource_list, config_name, save_flag, resources_parser)
 
         # parse for policies
         cfg = resources_parser.parse_lists_for_policies(np_list, resource_list, peer_container)
 
         return peer_container, resources_parser, cfg
 
-    def get_network_config(self, np_list, ns_list, pod_list, resource_list, config_name='global', save_flag=False):
+    def get_network_config(self, np_list, ns_list, pod_list, resource_list, config_name='global', save_flag=False,
+                           optimized_run='false'):
         """
         First tries to build a peer_container using the input resources (NetworkConfigs's resources)
         If fails, it uses the global peer container.
         Then parse the input resources for policies and builds the network config accordingly.
         :param Union[list[str], None] np_list: networkPolicies entries
         :param Union[list[str], None] ns_list: namespaces entries
         :param Union[list[str], None] pod_list: pods and services entries
@@ -161,16 +163,16 @@
         """
         NcaLogger().mute()
         peer_container, resources_parser, cfg = self.parse_elements(ns_list,
                                                                     pod_list,
                                                                     resource_list,
                                                                     config_name,
                                                                     save_flag,
-                                                                    np_list
-                                                                    )
+                                                                    np_list,
+                                                                    optimized_run)
         NcaLogger().unmute()
         # check if LiveSim can add anything.
         livesim_addons = self.analyze_livesim(resources_parser.policies_finder)
         if livesim_addons:
             NcaLogger().flush_messages(silent=True)
             if ns_list:
                 ns_list += livesim_addons
@@ -183,26 +185,27 @@
 
             # second attempt of parsing: input config + added livesim resources
             peer_container, resources_parser, cfg = self.parse_elements(ns_list,
                                                                         pod_list,
                                                                         resource_list,
                                                                         config_name,
                                                                         save_flag,
-                                                                        np_list
-                                                                        )
+                                                                        np_list,
+                                                                        optimized_run)
         else:
             # no relevant livesim resources to add
             NcaLogger().flush_messages()
 
         if cfg and config_name == 'global':
             config_name = cfg
 
         # build and return the networkConfig
         return NetworkConfig(name=config_name, peer_container=peer_container,
-                             policies_container=resources_parser.policies_finder.policies_container)
+                             policies_container=resources_parser.policies_finder.policies_container,
+                             optimized_run=optimized_run)
 
     def _set_config_peer_container(self, ns_list, pod_list, resource_list, config_name, save_flag, resources_parser):
         success, res_type = resources_parser.parse_lists_for_topology(ns_list, pod_list, resource_list)
         if success or res_type:
             if res_type:
                 self._fill_empty_finder(res_type, resources_parser)
             peer_container = resources_parser.build_peer_container(config_name)
@@ -246,17 +249,16 @@
             resources_parser.pods_finder = self.global_pods_finder
 
 
 class ResourcesParser:
     """
     This class parses the input resources for topology (pods, namespaces, services) and policies.
     """
-
-    def __init__(self):
-        self.policies_finder = PoliciesFinder()
+    def __init__(self, optimized_run='false'):
+        self.policies_finder = PoliciesFinder(optimized_run)
         self.pods_finder = PodsFinder()
         self.ns_finder = NamespacesFinder()
         self.services_finder = ServicesFinder()
 
     @staticmethod
     def _determine_topology_resource(topology_list, resource_list, res_type):
         specific_resource_flag = True
@@ -391,15 +393,15 @@
             if resource_item == 'k8s':
                 self.load_resources_from_k8s_live_cluster(resource_flags)
             elif resource_item == 'calico':
                 self._handle_calico_inputs(resource_flags)
             elif resource_item == 'istio':
                 self._handle_istio_inputs(resource_flags)
             else:
-                fast_load = ResourceType.Policies not in resource_flags
+                fast_load = (ResourceType.Policies not in resource_flags) and not ExplTracker().is_active()
                 resource_scanner = TreeScannerFactory.get_scanner(resource_item, fast_load=fast_load)
                 if resource_scanner is None:
                     continue
                 yaml_files = resource_scanner.get_yamls()
                 if not yaml_files:
                     continue
                 for yaml_file in yaml_files:
```

### Comparing `network-config-analyzer-1.9.2/nca/NetworkConfig/TopologyObjectsFinder.py` & `network-config-analyzer-1.9.3/nca/NetworkConfig/TopologyObjectsFinder.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 # Copyright 2020- IBM Inc. All rights reserved
 # SPDX-License-Identifier: Apache2.0
 #
 
 from sys import stderr
 import yaml
 from nca.Utils.CmdlineRunner import CmdlineRunner
-from nca.CoreDS.Peer import PeerSet, Pod, IpBlock, HostEP
+from nca.CoreDS.Peer import PeerSet, Pod, IpBlock, HostEP, BasePeerSet
 from nca.Resources.K8sNamespace import K8sNamespace
+from nca.Parsers.IstioServiceEntryYamlParser import IstioServiceEntryYamlParser
 from nca.Parsers.K8sServiceYamlParser import K8sServiceYamlParser
 from nca.Utils.NcaLogger import NcaLogger
+from nca.Utils.ExplTracker import ExplTracker
 
 
 class PodsFinder:
     """
     This class is responsible for populating the pods from the relevant input resources
     it builds a PeerSet and map of representative_peers to be used in the PeerContainer later.
     Resources that contain eps, may be:
@@ -64,14 +66,16 @@
             self._add_pod_from_workload_yaml(yaml_obj)
         elif kind == 'WorkloadEndpoint':
             self._add_wep_from_yaml(yaml_obj)
         elif kind == 'HostEndpoint':
             self._add_hep_from_yaml(yaml_obj)
         elif kind in ['NetworkSet', 'GlobalNetworkSet']:
             self._add_networkset_from_yaml(yaml_obj)
+        elif kind == 'ServiceEntry':
+            self._add_dns_entries_from_yaml(yaml_obj)
 
     def _add_pod_from_yaml(self, pod_object):
         """
         Add a K8s Pod to the container based on the given resource instance
         :param dict pod_object: The pod object to add
         :return: None
         """
@@ -102,28 +106,31 @@
             pod.set_label(key, val)
 
         containers = pod_object['spec'].get('containers', {})
         for container in containers:
             for port in container.get('ports') or []:
                 pod.add_named_port(port.get('name'), port.get('containerPort'), port.get('protocol', 'TCP'))
         self._add_peer(pod)
+        if ExplTracker().is_active():
+            ExplTracker().add_item(pod_object.path, pod_object.line_number, pod.full_name(), pod.workload_name)
 
     def _add_peer(self, peer):
         """
         Adds a specific peer to the container. Makes sure that no more than two isomorphic peers are added
         (we leave two isomorphic peers to model the connections between them)
         :param Endpoint peer: The peer to add
         :return: None
         """
         canonical_form = peer.canonical_form()
         peers_with_same_canonical_form = self.representative_peers.get(canonical_form, 0)
         if peers_with_same_canonical_form >= 2:  # We allow at most 2 peers from each equivalence group
             return
         self.representative_peers[canonical_form] = peers_with_same_canonical_form + 1
         self.peer_set.add(peer)
+        BasePeerSet().add_peer(peer)
 
     def _add_pod_from_workload_yaml(self, workload_resource):
         """
         Add K8s Pods to the container based on the given workload resource
         Reference: https://kubernetes.io/docs/reference/generated/kubernetes-api/v1.20/#podtemplatespec-v1-core
         :param workload_resource: A workload resource object
         :return: None
@@ -156,14 +163,20 @@
             for key, val in labels.items():
                 pod.set_label(key, val)
             pod_containers = pod_template.get('spec', {}).get('containers', [])
             for container in pod_containers:
                 for port in container.get('ports') or []:
                     pod.add_named_port(port.get('name'), port.get('containerPort'), port.get('protocol', 'TCP'))
             self._add_peer(pod)
+            if ExplTracker().is_active():
+                ExplTracker().add_item(workload_resource.path,
+                                       workload_resource.line_number,
+                                       pod.full_name(),
+                                       pod.workload_name
+                                       )
 
     def _add_networkset_from_yaml(self, networkset_object):
         """
         Add a Calico NetworkSet to the container based on the given resource instance
         :param dict networkset_object: The networkSet object to add
         :return: None
         """
@@ -186,14 +199,16 @@
             print(f'NetworkSet {name} should have labels', file=stderr)
         for key, val in labels.items():
             ipb.set_label(key, val)
         cidrs = spec.get('nets', {})
         for cidr in cidrs:
             ipb.add_cidr(cidr)
         self._add_peer(ipb)
+        if ExplTracker().is_active():
+            ExplTracker().add_item(networkset_object.path, networkset_object.line_number, ipb.full_name())
 
     def _add_hep_from_yaml(self, hep_object):
         """
         Add a Calico HostEndpoint to the container based on the given resource instance
         :param dict hep_object: The hep object to add
         :return: None
         """
@@ -209,14 +224,16 @@
         for port in spec.get('ports') or []:
             hep.add_named_port(port.get('name'), port.get('port'), port.get('protocol', 'TCP'))
 
         for profile in spec.get('profiles') or []:
             hep.add_profile(profile)
 
         self._add_peer(hep)
+        if ExplTracker().is_active():
+            ExplTracker().add_item(hep_object.path, hep_object.line_number, hep.full_name())
 
     def _add_wep_from_yaml(self, wep_object):
         """
         Add a Calico WorkloadEndpoint to the container based on the given resource instance
         :param dict wep_object: The wep object to add
         :return: None
         """
@@ -235,14 +252,27 @@
         for port in spec.get('ports') or []:
             wep.add_named_port(port.get('name'), port.get('port'), port.get('protocol', 'TCP'))
 
         for profile in spec.get('profiles') or []:
             wep.add_profile(profile)
 
         self._add_peer(wep)
+        if ExplTracker().is_active():
+            ExplTracker().add_item(wep_object.path, wep_object.line_number, wep.full_name(), wep.workload_name)
+
+    def _add_dns_entries_from_yaml(self, srv_entry_object):
+        """
+        Add DNSEntry peers to the container based on the given istio ServiceEntry resource instance
+        :param dict srv_entry_object: The service-entry object to parse for dns-entry peers
+        :return: None
+        """
+        parser = IstioServiceEntryYamlParser()
+        dns_entries = parser.parse_serviceentry(srv_entry_object, self.peer_set)
+        for dns_entry in dns_entries:
+            self._add_peer(dns_entry)
 
 
 class NamespacesFinder:
     """
     This class is responsible for populating the namespaces from relevant input resources.
     Resources that contain namespaces, may be:
     - git path of yaml file or a directory with yamls
@@ -306,15 +336,15 @@
             namespace = K8sNamespace(ns_name)
             self.namespaces[ns_name] = namespace
         return self.namespaces[ns_name]
 
 
 class ServicesFinder:
     """
-    This class is responsible for populating the services in the relevant input resources
+    This class is responsible for populating the services in the relevant input resources.
     Resources that contain services, may be:
     - git path of yaml file or a directory with yamls
     - local file (yaml or json) or a local directory containing yamls
     """
 
     def __init__(self):
         self.namespaces_finder = None
@@ -327,29 +357,31 @@
         """
         yaml_file = CmdlineRunner.get_k8s_resources('service')
         srv_resources = yaml.load(yaml_file, Loader=yaml.CSafeLoader)
         if not isinstance(srv_resources, dict):
             return
         parser = K8sServiceYamlParser('k8s')
         for srv_code in srv_resources.get('items', []):
-            service = parser.parse_service(srv_code)
-            if service:
-                service.namespace = self.namespaces_finder.get_or_update_namespace(service.namespace_name)
-                self.services_list.append(service)
+            self._parse_and_update_services_list(srv_code, parser)
 
     def parse_yaml_code_for_service(self, res_code, yaml_file):
         parser = K8sServiceYamlParser(yaml_file)
         if not isinstance(res_code, dict):
             return
         kind = res_code.get('kind')
         if kind in {'List'}:
             for srv_item in res_code.get('items', []):
-                if isinstance(srv_item, dict) and srv_item.get('kind') in {'Service'}:
-                    service = parser.parse_service(srv_item)
-                    if service:
-                        service.namespace = self.namespaces_finder.get_or_update_namespace(service.namespace_name)
-                        self.services_list.append(service)
-        elif kind in {'Service'}:
-            service = parser.parse_service(res_code)
-            if service:
-                service.namespace = self.namespaces_finder.get_or_update_namespace(service.namespace_name)
-                self.services_list.append(service)
+                if isinstance(srv_item, dict) and srv_item.get('kind') in ['Service']:
+                    self._parse_and_update_services_list(srv_item, parser)
+        elif kind in ['Service']:
+            self._parse_and_update_services_list(res_code, parser)
+
+    def _parse_and_update_services_list(self, srv_object, parser):
+        """
+        parses the service object using the given parser and updates the services_list accordingly
+        :param dict srv_object: the service object code from the yaml content
+        :param K8sServiceYamlParser parser: the service object parser
+        """
+        service = parser.parse_service(srv_object)
+        if service:
+            service.namespace = self.namespaces_finder.get_or_update_namespace(service.namespace_name)
+            self.services_list.append(service)
```

### Comparing `network-config-analyzer-1.9.2/nca/Parsers/CalicoPolicyYamlParser.py` & `network-config-analyzer-1.9.3/nca/Parsers/CalicoPolicyYamlParser.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,39 +3,42 @@
 # SPDX-License-Identifier: Apache2.0
 #
 
 import re
 from nca.CoreDS.ProtocolNameResolver import ProtocolNameResolver
 from nca.CoreDS.Peer import PeerSet, IpBlock
 from nca.CoreDS.PortSet import PortSet
-from nca.CoreDS.TcpLikeProperties import TcpLikeProperties
-from nca.CoreDS.ICMPDataSet import ICMPDataSet
+from nca.CoreDS.ConnectivityCube import ConnectivityCube
+from nca.CoreDS.ConnectivityProperties import ConnectivityProperties
+from nca.CoreDS.ProtocolSet import ProtocolSet
+from nca.CoreDS.DimensionsManager import DimensionsManager
 from nca.CoreDS.ConnectionSet import ConnectionSet
 from nca.Resources.NetworkPolicy import NetworkPolicy
 from nca.Resources.CalicoNetworkPolicy import CalicoNetworkPolicy, CalicoPolicyRule
 from .GenericYamlParser import GenericYamlParser
 
 
 class CalicoPolicyYamlParser(GenericYamlParser):
     """
     A parser for Calico NetworkPolicy/GlobalNetworkPolicy/Profile objects
     """
 
-    def __init__(self, policy, peer_container, policy_file_name=''):
+    def __init__(self, policy, peer_container, policy_file_name='', optimized_run='false'):
         """
         :param dict policy: The policy object as provided by the yaml parser
         :param PeerContainer peer_container: The policy will be evaluated against this set of peers
         :param str policy_file_name: The name of the file in which the policy resides
         """
         GenericYamlParser.__init__(self, policy_file_name)
         self.policy = policy
         self.peer_container = peer_container
         self.namespace = None
         # collecting labels used in calico network policy for fw-rules computation
         self.referenced_labels = set()
+        self.optimized_run = optimized_run
 
     def _parse_selector_expr(self, expr, origin_map, namespace, is_namespace_selector):
         """
         Parses an atomic expression (not containing a && or ||)
         :param str expr: The string expression to parse
         :param dict origin_map: The EntityRule object in which those expressions reside (for reporting errors)
         :param K8sNamespace namespace: Restrict pods to this given Namespace
@@ -344,85 +347,141 @@
         """
         allowed_elements = {'nets': 0, 'notNets': 0, 'selector': 0, 'notSelector': 0,
                             'namespaceSelector': 0, 'ports': 0, 'notPorts': 0, 'serviceAccounts': 2}
         self.check_fields_validity(entity_rule, 'network policy peer', allowed_elements)
 
         return self._get_rule_peers(entity_rule), self._get_rule_ports(entity_rule, protocol_supports_ports)
 
-    def _parse_icmp(self, icmp_data, not_icmp_data):
+    @staticmethod
+    def check_icmp_code_type_validity(icmp_type, icmp_code):
+        """
+        Checks that the type,code pair is a valid combination for an ICMP connection
+        :param int icmp_type: Connection type
+        :param int icmp_code: Connection code
+        :return: A string with an error if the pair is invalid. An empty string otherwise
+        :rtype: str
+        """
+        if icmp_code is not None and icmp_type is None:
+            return 'ICMP code cannot be specified without a type'
+
+        is_valid, err_message = DimensionsManager().validate_value_by_domain(icmp_type, 'icmp_type', 'ICMP type')
+        if not is_valid:
+            return err_message
+        if icmp_code is not None:
+            is_valid, err_message = DimensionsManager().validate_value_by_domain(icmp_code, 'icmp_code', 'ICMP code')
+            if not is_valid:
+                return err_message
+        return ''
+
+    def _parse_icmp(self, icmp_data, not_icmp_data, protocol, src_pods, dst_pods):  # noqa: C901
         """
         Parse the icmp and notICMP parts of a rule
         :param dict icmp_data:
         :param dict not_icmp_data:
-        :return: an ICMPDataSet object representing the allowed ICMP connections
-        :rtype: ICMPDataSet
+        :param: str protocol: the ICMP-like protocol
+        :param PeerSet src_pods: the source pods
+        :param PeerSet dst_pods: the destination pods
+        :return: a tuple (ConnectivityProperties, ConnectivityProperties),
+        where the first ConnectivityProperties is an original-format ICMP connections,
+        and the second ConnectivityProperties is an optimized-format ICMP connections, including src and dst pods.
+        :rtype: tuple (ConnectivityProperties, ConnectivityProperties)
         """
         icmp_type = icmp_data.get('type') if icmp_data is not None else None
         icmp_code = icmp_data.get('code') if icmp_data is not None else None
         not_icmp_type = not_icmp_data.get('type') if not_icmp_data is not None else None
         not_icmp_code = not_icmp_data.get('code') if not_icmp_data is not None else None
 
         allowed_keys = {'type': 0, 'code': 0}
         if icmp_data is not None:
             self.check_fields_validity(icmp_data, 'ICMP', allowed_keys)
-            err = ICMPDataSet.check_code_type_validity(icmp_type, icmp_code)
+            err = self.check_icmp_code_type_validity(icmp_type, icmp_code)
             if err:
                 self.syntax_error(err, icmp_data)
         if not_icmp_data is not None:
             self.check_fields_validity(not_icmp_data, 'notICMP', allowed_keys)
-            err = ICMPDataSet.check_code_type_validity(not_icmp_type, not_icmp_code)
+            err = self.check_icmp_code_type_validity(not_icmp_type, not_icmp_code)
             if err:
                 self.syntax_error(err, not_icmp_data)
 
-        res = ICMPDataSet(icmp_data is None and not_icmp_data is None)
+        protocols = ProtocolSet.get_protocol_set_with_single_protocol(protocol)
+        conn_cube = ConnectivityCube()
+        if icmp_type:
+            conn_cube["icmp_type"] = icmp_type
+            if icmp_code:
+                conn_cube["icmp_code"] = icmp_code
+        not_conn_cube = ConnectivityCube()
+        if not_icmp_type:
+            not_conn_cube["icmp_type"] = not_icmp_type
+            if not_icmp_code:
+                not_conn_cube["icmp_code"] = not_icmp_code
+        opt_conn_cube = conn_cube.copy()
+        opt_not_conn_cube = not_conn_cube.copy()
+        if self.optimized_run != 'false':
+            opt_conn_cube.update({"src_peers": src_pods, "dst_peers": dst_pods, "protocols": protocols})
+            opt_not_conn_cube.update({"src_peers": src_pods, "dst_peers": dst_pods, "protocols": protocols})
+
+        opt_props = ConnectivityProperties.make_empty_props()
         if icmp_data is not None:
-            res.add_to_set(icmp_type, icmp_code)
+            res = ConnectivityProperties.make_conn_props(conn_cube)
+            if self.optimized_run != 'false':
+                opt_props = ConnectivityProperties.make_conn_props(opt_conn_cube)
             if not_icmp_data is not None:
                 if icmp_type == not_icmp_type and icmp_code == not_icmp_code:
-                    res = ICMPDataSet()
+                    res = ConnectivityProperties.make_empty_props()
                     self.warning('icmp and notICMP are conflicting - no traffic will be matched', not_icmp_data)
                 elif icmp_type == not_icmp_type and icmp_code is None:
-                    tmp = ICMPDataSet()  # this is the only case where it makes sense to combine icmp and notICMP
-                    tmp.add_to_set(not_icmp_type, not_icmp_code)
+                    # this is the only case where it makes sense to combine icmp and notICMP
+                    tmp = ConnectivityProperties.make_conn_props(not_conn_cube)
                     res -= tmp
+                    if self.optimized_run != 'false':
+                        tmp_opt_props = ConnectivityProperties.make_conn_props(opt_not_conn_cube)
+                        opt_props -= tmp_opt_props
                 else:
                     self.warning('notICMP has no effect', not_icmp_data)
         elif not_icmp_data is not None:
-            res.add_all_but_given_pair(not_icmp_type, not_icmp_code)
-
-        return res
+            res = ConnectivityProperties.make_conn_props(conn_cube) - \
+                  ConnectivityProperties.make_conn_props(not_conn_cube)
+            if self.optimized_run != 'false':
+                opt_props = ConnectivityProperties.make_conn_props(opt_conn_cube) - \
+                            ConnectivityProperties.make_conn_props(opt_not_conn_cube)
+        else:  # no icmp_data or no_icmp_data; only protocol
+            res = ConnectivityProperties.make_conn_props(conn_cube)
+            if self.optimized_run != 'false':
+                opt_props = ConnectivityProperties.make_conn_props(opt_conn_cube)
+        return res, opt_props
 
     def _parse_protocol(self, protocol, rule):
         """
         Parse the protocol/notProtocol field in a rule
         :param protocol: The protocol (a string or an int)
         :param dict rule: The parsed rule object (for context)
         :return: The protocol number
         :rtype: int
         """
-        if not protocol:
+        if protocol is None:
             return None
         if isinstance(protocol, int):
-            if protocol < 1 or protocol > 255:
-                self.syntax_error('protocol must be a string or an integer in the range 1-255', rule)
+            if not ProtocolNameResolver.is_valid_protocol(protocol):
+                self.syntax_error('protocol must be a string or an integer in the range 0-255', rule)
             return protocol
 
         if protocol not in ['TCP', 'UDP', 'ICMP', 'ICMPv6', 'SCTP', 'UDPLite']:
             self.syntax_error('invalid protocol name: ' + protocol, rule)
         return ProtocolNameResolver.get_protocol_number(protocol)
 
-    def _parse_xgress_rule(self, rule, is_ingress, policy_selected_eps, is_profile):
+    def _parse_xgress_rule(self, rule, is_ingress, policy_selected_eps, is_profile):  # noqa: C901
         """
         Parse a single ingres/egress rule, producing a CalicoPolicyRule
         :param dict rule: The rule element to parse
         :param bool is_ingress: Whether this is an ingress rule
         :param PeerSet policy_selected_eps: The endpoints the policy captured
         :param bool is_profile: Whether the parsed policy is a Profile object
-        :return: A CalicoPolicyRule with the proper PeerSets, ConnectionSets and Action
-        :rtype: CalicoPolicyRule
+        :return: A tuple (CalicoPolicyRule, ConnectivityProperties) with the proper PeerSets, ConnectionSets and Action,
+        where ConnectivityProperties is an optimized rule format with protocols, src_peers and dst_peers in a HyperCubeSet
+        :rtype: tuple(CalicoPolicyRule, ConnectivityProperties)
         """
         allowed_keys = {'action': 1, 'protocol': 0, 'notProtocol': 0, 'icmp': 0, 'notICMP': 0, 'ipVersion': 0,
                         'source': 0, 'destination': 0, 'http': 2}
         self.check_fields_validity(rule, 'ingress/egress rule', allowed_keys)
 
         action = CalicoPolicyRule.action_str_to_action_type(rule['action'])
         if action is None:
@@ -449,41 +508,61 @@
 
         if is_ingress:  # FIXME: We do not handle well the case where dst_res_pods or src_res_pods contain ipBlocks
             dst_res_pods &= policy_selected_eps
         else:
             src_res_pods &= policy_selected_eps
 
         connections = ConnectionSet()
+        conn_props = ConnectivityProperties.make_empty_props()
         if protocol is not None:
+            protocols = ProtocolSet.get_protocol_set_with_single_protocol(protocol)
             if not_protocol is not None:
                 if protocol == not_protocol:
                     self.warning('Protocol and notProtocol are conflicting, no traffic will be matched', rule)
                 else:
                     self.warning('notProtocol field has no effect', rule)
             else:
                 if protocol_supports_ports:
-                    connections.add_connections(protocol, TcpLikeProperties(src_res_ports, dst_res_ports))
+                    conn_cube = ConnectivityCube.make_from_dict({"src_ports": src_res_ports, "dst_ports": dst_res_ports})
+                    connections.add_connections(protocol, ConnectivityProperties.make_conn_props(conn_cube))
+                    if self.optimized_run != 'false':
+                        conn_cube.update({"protocols": protocols, "src_peers": src_res_pods, "dst_peers": dst_res_pods})
+                        conn_props = ConnectivityProperties.make_conn_props(conn_cube)
                 elif ConnectionSet.protocol_is_icmp(protocol):
-                    connections.add_connections(protocol, self._parse_icmp(rule.get('icmp'), rule.get('notICMP')))
+                    icmp_props, conn_props = self._parse_icmp(rule.get('icmp'), rule.get('notICMP'),
+                                                              protocol, src_res_pods, dst_res_pods)
+                    connections.add_connections(protocol, icmp_props)
                 else:
                     connections.add_connections(protocol, True)
+                    if self.optimized_run != 'false':
+                        conn_props = ConnectivityProperties.make_conn_props_from_dict({"protocols": protocols,
+                                                                                       "src_peers": src_res_pods,
+                                                                                       "dst_peers": dst_res_pods})
         elif not_protocol is not None:
             connections.add_all_connections()
             connections.remove_protocol(not_protocol)
+            if self.optimized_run != 'false' and src_res_pods and dst_res_pods:
+                protocols = ProtocolSet(True)
+                protocols.remove_protocol(not_protocol)
+                conn_props = ConnectivityProperties.make_conn_props_from_dict({"protocols": protocols,
+                                                                               "src_peers": src_res_pods,
+                                                                               "dst_peers": dst_res_pods})
         else:
             connections.allow_all = True
-
+            if self.optimized_run != 'false':
+                conn_props = ConnectivityProperties.make_conn_props_from_dict({"src_peers": src_res_pods,
+                                                                               "dst_peers": dst_res_pods})
         self._verify_named_ports(rule, dst_res_pods, connections)
 
         if not src_res_pods and policy_selected_eps and (is_ingress or not is_profile):
             self.warning('Rule selects no source endpoints', rule)
         if not dst_res_pods and policy_selected_eps and (not is_ingress or not is_profile):
             self.warning('Rule selects no destination endpoints', rule)
 
-        return CalicoPolicyRule(src_res_pods, dst_res_pods, connections, action)
+        return CalicoPolicyRule(src_res_pods, dst_res_pods, connections, action, conn_props)
 
     def _verify_named_ports(self, rule, rule_eps, rule_conns):
         """
         Check the validity of named ports in a given rule: whether a relevant ep refers to the named port and whether
         the protocol defined in the policy matches the protocol defined by the ep. Issue warnings as required.
         :param dict rule: The unparsed rule (for reference in warnings)
         :param Peer.PeerSet rule_eps: The set of eps in which the named ports should be defined
```

### Comparing `network-config-analyzer-1.9.2/nca/Parsers/GenericYamlParser.py` & `network-config-analyzer-1.9.3/nca/Parsers/GenericYamlParser.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,14 @@
 # Copyright 2020- IBM Inc. All rights reserved
 # SPDX-License-Identifier: Apache2.0
 #
 
 from sys import stderr
 from enum import Enum
 from nca.CoreDS.DimensionsManager import DimensionsManager
-from nca.CoreDS.TcpLikeProperties import TcpLikeProperties
-from nca.CoreDS.MethodSet import MethodSet
-from nca.CoreDS.ConnectionSet import ConnectionSet
-from nca.CoreDS.PortSet import PortSet
 from nca.CoreDS.Peer import IpBlock
 from nca.Utils.NcaLogger import NcaLogger
 from nca.FileScanners.GenericTreeScanner import ObjectWithLocation
 
 
 class GenericYamlParser:
     """
@@ -222,30 +218,14 @@
         :return: None
         :raises SyntaxError: if the value is not within the defined domain for the relevant dimension
         """
         is_valid, err_message = DimensionsManager().validate_value_by_domain(value, dim_name, value_name)
         if not is_valid:
             self.syntax_error(err_message, array)
 
-    @staticmethod
-    def _get_connection_set_from_properties(dest_ports, method_set=MethodSet(True), paths_dfa=None, hosts_dfa=None):
-        """
-        get ConnectionSet with TCP allowed connections, corresponding to input properties cube
-        :param PortSet dest_ports: ports set for dset_ports dimension
-        :param MethodSet method_set: methods set for methods dimension
-        :param MinDFA paths_dfa: MinDFA obj for paths dimension
-        :param MinDFA hosts_dfa: MinDFA obj for hosts dimension
-        :return: ConnectionSet with TCP allowed connections , corresponding to input properties cube
-        """
-        tcp_properties = TcpLikeProperties(source_ports=PortSet(True), dest_ports=dest_ports, methods=method_set,
-                                           paths=paths_dfa, hosts=hosts_dfa)
-        res = ConnectionSet()
-        res.add_connections('TCP', tcp_properties)
-        return res
-
     def check_and_update_has_ipv6_addresses(self, peers):
         """
         checks if the peer list has ipv6 addresses
         updates self.has_ipv6_addresses=true if at least on peer is an IPblock with IPv6 addresses
         :param PeerSet peers: list of peers
         """
         for peer in peers:
```

### Comparing `network-config-analyzer-1.9.2/nca/Parsers/IngressPolicyYamlParser.py` & `network-config-analyzer-1.9.3/nca/Parsers/IngressPolicyYamlParser.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 #
 import re
 
 from nca.CoreDS.MinDFA import MinDFA
 from nca.CoreDS.DimensionsManager import DimensionsManager
 from nca.CoreDS.Peer import PeerSet
 from nca.CoreDS.PortSet import PortSet
+from nca.CoreDS.ConnectivityCube import ConnectivityCube
+from nca.CoreDS.ConnectivityProperties import ConnectivityProperties
 from nca.Resources.IngressPolicy import IngressPolicy
 from nca.Resources.NetworkPolicy import NetworkPolicy
 from .GenericIngressLikeYamlParser import GenericIngressLikeYamlParser
 
 
 class IngressPolicyYamlParser(GenericIngressLikeYamlParser):
     """
@@ -88,15 +90,19 @@
             else:
                 warning_msg += 'The rule path containing this backend service will be ignored'
             self.warning(warning_msg, service)
             return None, None, False
 
         service_port = srv.get_port_by_name(port_name) if port_name else srv.get_port_by_number(port_number)
         if not service_port:
-            self.syntax_error(f'Missing port {port_name if port_name else port_number} in the service', service)
+            port_str = f'{port_name if port_name else port_number}'
+            warning_msg = f'Ingress rule redirects traffic to {service_name}:{port_str}, '
+            warning_msg += f' but port {port_str} is not exposed by Service {service_name}'
+            self.warning(warning_msg, service)
+            return None, None, False
 
         rule_ports = PortSet()
         rule_ports.add_port(service_port.target_port)  # may be either a number or a named port
         return srv.target_pods, rule_ports, True
 
     def parse_ingress_path(self, path):
         """
@@ -177,85 +183,82 @@
         return res
 
     def _make_default_connections(self, hosts_dfa, paths_dfa=None):
         """
         Creates default backend connections for given hosts and paths
         :param MinDFA hosts_dfa: the hosts for the default connections
         :param MinDFA paths_dfa: the paths for the default connections
-        :return: TcpLikeProperties containing default connections or None (when no default backend exists)
+        :return: ConnectivityProperties containing default connections or None (when no default backend exists)
         """
-        default_conns = None
+        default_conns = ConnectivityProperties.make_empty_props()
         if self.default_backend_peers:
+            conn_cube = ConnectivityCube.make_from_dict({"dst_ports": self.default_backend_ports,
+                                                         "dst_peers": self.default_backend_peers})
+            if hosts_dfa:
+                conn_cube["hosts"] = hosts_dfa
             if paths_dfa:
-                default_conns = self._make_tcp_like_properties(self.default_backend_ports, self.default_backend_peers,
-                                                               paths_dfa, hosts_dfa)
-            else:
-                default_conns = self._make_tcp_like_properties(self.default_backend_ports, self.default_backend_peers,
-                                                               hosts_dfa=hosts_dfa)
+                conn_cube["paths"] = paths_dfa
+            default_conns = ConnectivityProperties.make_conn_props(conn_cube)
         return default_conns
 
     def parse_rule(self, rule):
         """
         Parses a single ingress rule, producing a number of IngressPolicyRules (per path).
         :param dict rule: The rule resource
-        :return: A tuple containing TcpLikeProperties including allowed connections for the given rule,
+        :return: A tuple containing ConnectivityProperties including allowed connections for the given rule,
         and a dfa for hosts
         """
         if rule is None:
             self.syntax_error('Ingress rule cannot be null. ')
 
         allowed_elements = {'host': [0, str], 'http': [0, dict]}
         self.check_fields_validity(rule, 'ingress rule', allowed_elements)
         hosts_dfa = self.parse_regex_host_value(rule.get("host"), rule)
         paths_array = self.get_key_array_and_validate_not_empty(rule.get('http'), 'paths')
-        allowed_conns = None
-        default_conns = None
+        allowed_conns = ConnectivityProperties.make_empty_props()
+        default_conns = ConnectivityProperties.make_empty_props()
         if paths_array is not None:
             all_paths_dfa = None
             parsed_paths = []
             for path in paths_array:
                 path_resources = self.parse_ingress_path(path)
                 if path_resources is not None:
                     parsed_paths.append(path_resources)
             if parsed_paths:
                 parsed_paths_with_dfa = self.segregate_longest_paths_and_make_dfa(parsed_paths)
+                conn_cube = ConnectivityCube.make_from_dict({"hosts": hosts_dfa})
                 for (_, paths_dfa, _, peers, ports) in parsed_paths_with_dfa:
                     # every path is converted to allowed connections
-                    conns = self._make_tcp_like_properties(ports, peers, paths_dfa, hosts_dfa)
-                    if not allowed_conns:
-                        allowed_conns = conns
-                    else:
-                        allowed_conns |= conns
+                    conn_cube.update({"dst_ports": ports, "dst_peers": peers, "paths": paths_dfa})
+                    conns = ConnectivityProperties.make_conn_props(conn_cube)
+                    allowed_conns |= conns
                     if not all_paths_dfa:
                         all_paths_dfa = paths_dfa
                     else:
                         all_paths_dfa = all_paths_dfa | paths_dfa  # pick all captured paths
                 # for this host, every path not captured by the above paths goes to the default backend or is denied
                 paths_remainder_dfa = DimensionsManager().get_dimension_domain_by_name('paths') - all_paths_dfa
                 default_conns = self._make_default_connections(hosts_dfa, paths_remainder_dfa)
         else:  # no paths --> everything for this host goes to the default backend or is denied
             default_conns = self._make_default_connections(hosts_dfa)
-        if allowed_conns and default_conns:
-            allowed_conns |= default_conns
-        elif default_conns:
-            allowed_conns = default_conns
+        allowed_conns |= default_conns
         return allowed_conns, hosts_dfa
 
     def parse_policy(self):
         """
         Parses the input object to create  IngressPolicy object (with deny rules only)
         :return: IngressPolicy object with proper deny egress_rules, or None for wrong input object
         """
         policy_name, policy_ns = self.parse_generic_yaml_objects_fields(self.policy, ['Ingress'],
                                                                         ['networking.k8s.io/v1'], 'k8s', True)
         if policy_name is None:
             return None  # Not an Ingress object
 
         self.namespace = self.peer_container.get_namespace(policy_ns)
-        res_policy = IngressPolicy(policy_name + '/allow', self.namespace, IngressPolicy.ActionType.Allow)
+        res_policy = IngressPolicy(policy_name + '/allow', self.namespace)
         res_policy.policy_kind = NetworkPolicy.PolicyType.Ingress
 
         policy_spec = self.policy['spec']
         allowed_spec_keys = {'defaultBackend': [0, dict], 'ingressClassName': [0, str],
                              'rules': [0, list], 'tls': [0, list]}
         self.check_fields_validity(policy_spec, 'Ingress spec', allowed_spec_keys)
 
@@ -263,37 +266,30 @@
                                                                                        True)
         # TODO extend to other ingress controllers
         res_policy.selected_peers = \
             self.peer_container.get_pods_with_service_name_containing_given_string('ingress-nginx')
         if not res_policy.selected_peers:
             self.missing_k8s_ingress_peers = True
             self.warning("No ingress-nginx pods found, the Ingress policy will have no effect")
-        allowed_conns = None
+        allowed_conns = ConnectivityProperties.make_empty_props()
         all_hosts_dfa = None
         for ingress_rule in policy_spec.get('rules', []):
             conns, hosts_dfa = self.parse_rule(ingress_rule)
-            if conns:
-                if not allowed_conns:
-                    allowed_conns = conns
-                else:
-                    allowed_conns |= conns
+            allowed_conns |= conns
             if hosts_dfa:
                 if not all_hosts_dfa:
                     all_hosts_dfa = hosts_dfa
                 else:
                     all_hosts_dfa = all_hosts_dfa | hosts_dfa
             else:
                 all_hosts_dfa = DimensionsManager().get_dimension_domain_by_name('hosts')
         # every host not captured by the ingress rules goes to the default backend
-        hosts_remainder_dfa = DimensionsManager().get_dimension_domain_by_name('hosts') - all_hosts_dfa
-        default_conns = self._make_default_connections(hosts_remainder_dfa)
-        if allowed_conns and default_conns:
+        if self.default_backend_peers:
+            hosts_remainder_dfa = DimensionsManager().get_dimension_domain_by_name('hosts') - all_hosts_dfa
+            default_conns = self._make_default_connections(hosts_remainder_dfa)
             allowed_conns |= default_conns
-        elif default_conns:
-            allowed_conns = default_conns
-
         # allowed_conns = none means that services referenced by this Ingress policy are not found,
         # then no connections rules to add (Ingress policy has no effect)
         if allowed_conns:
-            res_policy.add_rules(self._make_allow_rules(allowed_conns))
+            res_policy.add_rules(self._make_allow_rules(allowed_conns, res_policy.selected_peers))
         res_policy.findings = self.warning_msgs
         return res_policy
```

### Comparing `network-config-analyzer-1.9.2/nca/Parsers/IstioGenericYamlParser.py` & `network-config-analyzer-1.9.3/nca/Parsers/IstioGenericYamlParser.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,17 @@
         calculates the peers selected by current policy object
         :param dict workload_selector: the workload selector of the policy object yaml
         :param str dict_key: the key used in the selector for labels
         :return the list of peers selected by the policy object
         :rtype: Peer.PeerSet
         """
         if workload_selector is None:
-            selected_peers = self.peer_container.get_all_peers_group()
+            # istio selected peers may only be clusterEP
+            selected_peers = self.peer_container.get_all_peers_group(add_external_ips=False, include_globals=False,
+                                                                     include_dns_entries=False)
         else:
             selected_peers = self._parse_workload_selector(workload_selector, dict_key)
         # if policy's namespace is the root namespace, then it applies to all cluster's namespaces
         if self.namespace.name != istio_root_namespace:
             selected_peers &= self.peer_container.get_namespace_pods(self.namespace)
 
         return selected_peers
```

### Comparing `network-config-analyzer-1.9.2/nca/Parsers/IstioPolicyYamlParser.py` & `network-config-analyzer-1.9.3/nca/Parsers/IstioPolicyYamlParser.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from nca.CoreDS.MinDFA import MinDFA
 from nca.CoreDS.DimensionsManager import DimensionsManager
 from nca.CoreDS.Peer import IpBlock, PeerSet
 from nca.CoreDS.ConnectionSet import ConnectionSet
 from nca.CoreDS.PortSet import PortSet
 from nca.CoreDS.MethodSet import MethodSet
+from nca.CoreDS.ConnectivityProperties import ConnectivityProperties
 from nca.Resources.IstioNetworkPolicy import IstioNetworkPolicy, IstioPolicyRule
 from nca.Resources.IstioTrafficResources import istio_root_namespace
 from nca.Resources.NetworkPolicy import NetworkPolicy
 from .IstioGenericYamlParser import IstioGenericYamlParser
 
 
 class IstioPolicyYamlParser(IstioGenericYamlParser):
@@ -180,32 +181,32 @@
 
     def parse_key_values(self, key, values, not_values):
         """
         parse key and its values for a given condition component in a rule
         :param str key: the specified key str
         :param list values: a list of strings with values for this key
         :param list not_values: a list of strings with negative values for this key
-        :return: PeerSet or ConnectionSet (depends on the key) with allowed values
+        :return: PeerSet or ConnectivityProperties (depends on the key) with allowed values
         """
         if key == 'source.ip':
             return self.parse_ip_block(values, not_values)  # PeerSet
         elif key == 'source.namespace':
             return self.parse_namespaces(values, not_values)  # PeerSet
         elif key == 'source.principal':
             return self.parse_principals(values, not_values)  # PeerSet
         elif key == 'destination.port':
             dst_ports = self.get_rule_ports(values, not_values)  # PortSet
-            return self._get_connection_set_from_properties(dst_ports)  # ConnectionSet
+            return ConnectivityProperties.make_conn_props_from_dict({"dst_ports": dst_ports})
         return NotImplemented, False
 
     def parse_condition(self, condition):
         """
         parse a condition component in a rule
         :param dict condition: the condition to parse
-        :return: PeerSet or ConnectionSet (depends on the key) with allowed values
+        :return: PeerSet or ConnectivityProperties (depends on the key) with allowed values
         """
         allowed_elements = {'key': [1, str], 'values': [0, list], 'notValues': [0, list]}
         allowed_key_values = {'key': ['source.ip', 'source.namespace', 'source.principal', 'destination.port']}
         # https://istio.io/latest/docs/reference/config/security/conditions/
         # TODO: support additional key values: request.headers, remote.ip, request.auth.principal,
         #  request.auth.audiences, request.auth.presenter, request.auth.claims, destination.ip, connection.sni
         self.check_fields_validity(condition, 'authorization policy condition', allowed_elements, allowed_key_values)
@@ -214,15 +215,15 @@
 
         key = condition.get('key')
         values = condition.get('values')
         not_values = condition.get('notValues')
         if not values and not not_values:
             self.syntax_error('error parsing condition: at least one of values or not_values must be set. ', condition)
 
-        return self.parse_key_values(key, values, not_values)  # PeerSet or ConnectionSet
+        return self.parse_key_values(key, values, not_values)  # PeerSet or ConnectivityProperties
 
     # TODO: avoid code duplication with Calico version...
     def _parse_port(self, port, array):
         """
         Parse a single port in the array defined in the ports/notPorts part
         :param Union[int,str] port: The port to parse
         :param list array: The object containing the port (for reporting errors)
@@ -367,15 +368,15 @@
 
         return rule_methods
 
     def parse_operation(self, operation_dict):
         """
         parse an operation component in a rule
         :param dict operation_dict: the operation to parse
-        :return: ConnectionSet object with allowed connections
+        :return: ConnectivityProperties object with allowed connections
         """
 
         to_allowed_elements = {'operation': [1, dict]}
         self.check_fields_validity(operation_dict, 'authorization policy rule: to', to_allowed_elements)
 
         operation = operation_dict.get('operation')
         if operation is None:
@@ -392,16 +393,16 @@
 
         dst_ports = self.get_rule_ports(operation.get('ports'), operation.get('notPorts'))  # PortSet
         methods_set = self._get_methods_set(operation)
         paths_dfa = self.parse_regex_dimension_values("paths", operation.get("paths"), operation.get("notPaths"),
                                                       operation)
         hosts_dfa = self.parse_regex_dimension_values("hosts", operation.get("hosts"), operation.get("notHosts"),
                                                       operation)
-
-        return self._get_connection_set_from_properties(dst_ports, methods_set, paths_dfa, hosts_dfa)
+        return ConnectivityProperties.make_conn_props_from_dict({"dst_ports": dst_ports, "methods": methods_set,
+                                                                 "paths": paths_dfa, "hosts": hosts_dfa})
 
     def parse_source(self, source_dict):
         """
         Parse a source peer inside a rule (an element of the 'from' array)
         :param dict source_dict: The object to parse
         :return: A PeerSet object containing the set of peers defined by the selectors/ipblocks
         :rtype: Peer.PeerSet
@@ -454,20 +455,22 @@
             not_ip_blocks = source_peer.get('notIpBlocks')
             res &= self.parse_ip_block(ip_blocks, not_ip_blocks)
 
         return res
 
     #  A match occurs when at least one source, one operation and all conditions matches the request
     # https://istio.io/latest/docs/reference/config/security/authorization-policy/#Rule
-    def parse_ingress_rule(self, rule):
+    def parse_ingress_rule(self, rule, selected_peers):
         """
         Parse a single ingress rule, producing a IstioPolicyRule.
         :param dict rule: The dict with the rule fields
-        :return: A IstioPolicyRule with the proper PeerSet and ConnectionSet
-        :rtype: IstioPolicyRule
+        :param PeerSet selected_peers: The selected peers of the policy
+        :return: A tuple (IstioPolicyRule, ConnectivityProperties) with the proper PeerSet and ConnectionSet,
+        where ConnectivityProperties is an optimized rule format in a HyperCubeSet format
+        :rtype: tuple(IstioPolicyRule, ConnectivityProperties)
         """
         if rule is None:
             self.syntax_error('Authorization policy rule cannot be null. ')
 
         allowed_elements = {'from': [0, list], 'to': [0, list], 'when': [0, list]}
         self.check_fields_validity(rule, 'authorization policy rule', allowed_elements)
         for key_elem in allowed_elements:
@@ -481,38 +484,50 @@
                 res_peers |= self.parse_source(source_dict)
         else:  # no 'from' in the rule => all source peers allowed
             res_peers = self.peer_container.get_all_peers_group(True)
 
         to_array = self.get_key_array_and_validate_not_empty(rule, 'to')
         # currently parsing only ports
         # TODO: extend operations parsing to include other attributes
+        conn_props = ConnectivityProperties.make_empty_props()
         if to_array is not None:
-            connections = ConnectionSet()
             for operation_dict in to_array:
-                connections |= self.parse_operation(operation_dict)
+                conn_props |= self.parse_operation(operation_dict)
+            connections = ConnectionSet()
+            connections.add_connections('TCP', conn_props)
         else:  # no 'to' in the rule => all connections allowed
             connections = ConnectionSet(True)
+            conn_props = ConnectivityProperties.get_all_conns_props_per_config_peers(self.peer_container)
 
         # condition possible result value:
-        #         source-ip (from) , source-namespace (from) [Peerset], destination.port (to) [ConnectionSet]
-        # should update either res_pods or connections according to the condition
+        #         source-ip (from) , source-namespace (from) [Peerset], destination.port (to) [ConnectivityProperties]
+        # should update either res_pods or condition_props according to the condition
         condition_array = rule.get('when')  # this array can be empty (unlike 'to' and 'from')
         # the combined condition ("AND" of all conditions) should be applied
+        condition_conns = ConnectionSet(True)
+        condition_props = ConnectivityProperties.make_all_props()
         if condition_array is not None:
             for condition in condition_array:
                 condition_res = self.parse_condition(condition)
                 if isinstance(condition_res, PeerSet):
                     res_peers &= condition_res
-                elif isinstance(condition_res, ConnectionSet):
-                    connections &= condition_res
-
+                elif isinstance(condition_res, ConnectivityProperties):
+                    condition_props &= condition_res
+            condition_conns = ConnectionSet()
+            condition_conns.add_connections('TCP', condition_props)
         if not res_peers:
             self.warning('Rule selects no pods', rule)
-
-        return IstioPolicyRule(res_peers, connections)
+        if not res_peers or not selected_peers:
+            condition_props = ConnectivityProperties.make_empty_props()
+        else:
+            condition_props &= ConnectivityProperties.make_conn_props_from_dict({"src_peers": res_peers,
+                                                                                 "dst_peers": selected_peers})
+        connections &= condition_conns
+        conn_props &= condition_props
+        return IstioPolicyRule(res_peers, connections, conn_props)
 
     @staticmethod
     def parse_policy_action(action):
         """
         :param string action: the action to parse
         :return: IstioNetworkPolicy.ActionType Allow/Deny
         """
@@ -525,15 +540,16 @@
     def parse_policy(self):
         """
         Parses the input object to create a IstioNetworkPolicy object
         :return: a IstioNetworkPolicy object with proper PeerSets and ConnectionSets
         :rtype: IstioNetworkPolicy
         """
         policy_name, policy_ns = self.parse_generic_yaml_objects_fields(self.policy, ['AuthorizationPolicy'],
-                                                                        ['security.istio.io/v1beta1'], 'istio')
+                                                                        ['security.istio.io/v1beta1', 'security.istio.io/v1'],
+                                                                        'istio')
         if policy_name is None:
             return None  # not an Istio AuthorizationPolicy
         warn_if_missing = policy_ns != istio_root_namespace
         self.namespace = self.peer_container.get_namespace(policy_ns, warn_if_missing)
         res_policy = IstioNetworkPolicy(policy_name, self.namespace)
         res_policy.policy_kind = NetworkPolicy.PolicyType.IstioAuthorizationPolicy
 
@@ -551,15 +567,16 @@
         if action:
             res_policy.action = self.parse_policy_action(action)
         res_policy.affects_ingress = True
         res_policy.affects_egress = False
         pod_selector = policy_spec.get('selector')
         res_policy.selected_peers = self.update_policy_peers(pod_selector, 'matchLabels')
         for ingress_rule in policy_spec.get('rules', []):
-            res_policy.add_ingress_rule(self.parse_ingress_rule(ingress_rule))
+            rule = self.parse_ingress_rule(ingress_rule, res_policy.selected_peers)
+            res_policy.add_ingress_rule(rule)
         if not res_policy.ingress_rules and res_policy.action == IstioNetworkPolicy.ActionType.Deny:
             self.syntax_error("DENY action without rules is meaningless as it will never be triggered")
 
         res_policy.findings = self.warning_msgs
         res_policy.referenced_labels = self.referenced_labels
         res_policy.has_ipv6_addresses = self.has_ipv6_addresses
         return res_policy
```

### Comparing `network-config-analyzer-1.9.2/nca/Parsers/IstioTrafficResourcesYamlParser.py` & `network-config-analyzer-1.9.3/nca/Parsers/IstioTrafficResourcesYamlParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 # SPDX-License-Identifier: Apache2.0
 #
 
 from functools import reduce
 from nca.CoreDS.MinDFA import MinDFA
 from nca.CoreDS.Peer import PeerSet
 from nca.CoreDS.MethodSet import MethodSet
+from nca.CoreDS.ConnectivityCube import ConnectivityCube
+from nca.CoreDS.ConnectivityProperties import ConnectivityProperties
 from nca.Resources.IstioTrafficResources import Gateway, VirtualService
 from nca.Resources.IngressPolicy import IngressPolicy
 from nca.Resources.NetworkPolicy import NetworkPolicy
 from .GenericIngressLikeYamlParser import GenericIngressLikeYamlParser
 
 
 class IstioTrafficResourcesYamlParser(GenericIngressLikeYamlParser):
@@ -190,16 +192,16 @@
         :param VirtualService vs: the partially parsed VirtualService
         :param dict vs_spec: the virtual service resource
         """
         http = vs_spec.get('http')
         for route in http or []:
             self.check_fields_validity(route, f'HTTPRroute in the VirtualService {vs.full_name()}',
                                        {'name': [0, str], 'match': 0, 'route': 0, 'redirect': 3, 'delegate': 3,
-                                        'rewrite': 3, 'timeout': 3, 'retries': 3, 'fault': 3, 'mirror': 3,
-                                        'mirrorPercentage': 3, 'corsPolicy': 3, 'headers': 3})
+                                        'rewrite': 0, 'timeout': 0, 'retries': 0, 'fault': 0, 'mirror': 3,
+                                        'mirrorPercentage': 0, 'corsPolicy': 3, 'headers': 3})
             http_route = VirtualService.HTTPRoute()
             self.parse_http_match_request(route, http_route, vs)
             self.parse_http_route_destinations(route, http_route, vs)
             vs.add_http_route(http_route)
 
     def parse_istio_regex_string(self, resource, attr_name, vs_name):
         """
@@ -259,14 +261,16 @@
                                         'queryParams': [3, dict], 'sourceNamespace': [3, str]})
             uri_dfa = self.parse_istio_regex_string(item, 'uri', vs.full_name())
             if uri_dfa:
                 parsed_route.add_uri_dfa(uri_dfa)
             methods = self.parse_istio_regex_string(item, 'method', vs.full_name())
             if methods:
                 parsed_route.add_methods(methods)
+            else:
+                parsed_route.add_methods(MethodSet(True))
 
     def parse_http_route_destinations(self, route, parsed_route, vs):
         """
         Parse HTTPRouteDestination of a VirtualService and add the result to parsed_route
         :param dict route: the HttpRoute resource, as defined in
         https://istio.io/latest/docs/reference/config/networking/virtual-service/#HTTPRoute
         :param HTTPRoute parsed_route: the output parsed http route to contain the parsed attributes
@@ -328,25 +332,25 @@
         return self.peer_container.get_service_by_name_and_ns(service_name, namespace)
 
     def make_allowed_connections(self, vs, host_dfa):
         """
         Create allowed connections of the given VirtualService
         :param VirtualService vs: the given VirtualService and the given hosts
         :param MinDFA host_dfa: the hosts attribute
-        :return: TcpLikeProperties with TCP allowed connections
+        :return: ConnectivityProperties with allowed connections
         """
-        allowed_conns = None
+        allowed_conns = ConnectivityProperties.make_empty_props()
         for http_route in vs.http_routes:
+            conn_cube = ConnectivityCube.make_from_dict({"paths": http_route.uri_dfa, "hosts": host_dfa,
+                                                         "methods": http_route.methods})
             for dest in http_route.destinations:
-                conns = self._make_tcp_like_properties(dest.port, dest.service.target_pods, http_route.uri_dfa,
-                                                       host_dfa, http_route.methods)
-                if not allowed_conns:
-                    allowed_conns = conns
-                else:
-                    allowed_conns |= conns
+                conn_cube.update({"dst_ports": dest.port, "dst_peers": dest.service.target_pods})
+                conns = \
+                    ConnectivityProperties.make_conn_props(conn_cube)
+                allowed_conns |= conns
         return allowed_conns
 
     def create_istio_traffic_policies(self):
         """
         Create IngressPolicies according to the parsed Gateways and VirtualServices
         :return list[IngressPolicy]: the resulting policies
         """
@@ -382,21 +386,20 @@
                     peers = reduce(PeerSet.__or__, gtw_peers)
                     if peers_to_hosts.get(peers):
                         peers_to_hosts[peers] |= host_dfa
                     else:
                         peers_to_hosts[peers] = host_dfa
 
             for peer_set, host_dfa in peers_to_hosts.items():
-                res_policy = IngressPolicy(vs.name + '/' + str(host_dfa) + '/allow', vs.namespace,
-                                           IngressPolicy.ActionType.Allow)
+                res_policy = IngressPolicy(vs.name + '/' + str(host_dfa) + '/allow', vs.namespace)
                 res_policy.policy_kind = NetworkPolicy.PolicyType.Ingress
                 res_policy.selected_peers = peer_set
                 allowed_conns = self.make_allowed_connections(vs, host_dfa)
                 if allowed_conns:
-                    res_policy.add_rules(self._make_allow_rules(allowed_conns))
+                    res_policy.add_rules(self._make_allow_rules(allowed_conns, res_policy.selected_peers))
                     res_policy.findings = self.warning_msgs
                     vs_policies.append(res_policy)
             if not vs_policies:
                 self.warning(f'virtual service {vs.full_name()} does not affect traffic and is ignored')
             result.extend(vs_policies)
         unused_gateways = set(self.gateways.values()) - used_gateways
         if unused_gateways:
```

### Comparing `network-config-analyzer-1.9.2/nca/Parsers/K8sPolicyYamlParser.py` & `network-config-analyzer-1.9.3/nca/Parsers/K8sPolicyYamlParser.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,37 +3,40 @@
 # SPDX-License-Identifier: Apache2.0
 #
 
 import re
 from nca.CoreDS import Peer
 from nca.CoreDS.ConnectionSet import ConnectionSet
 from nca.CoreDS.PortSet import PortSet
-from nca.CoreDS.TcpLikeProperties import TcpLikeProperties
+from nca.CoreDS.ConnectivityCube import ConnectivityCube
+from nca.CoreDS.ConnectivityProperties import ConnectivityProperties
 from nca.CoreDS.ProtocolNameResolver import ProtocolNameResolver
+from nca.CoreDS.ProtocolSet import ProtocolSet
 from nca.Resources.NetworkPolicy import NetworkPolicy
 from nca.Resources.K8sNetworkPolicy import K8sNetworkPolicy, K8sPolicyRule
 from .GenericYamlParser import GenericYamlParser
 
 
 class K8sPolicyYamlParser(GenericYamlParser):
     """
     A parser for k8s NetworkPolicy objects
     """
 
-    def __init__(self, policy, peer_container, policy_file_name=''):
+    def __init__(self, policy, peer_container, policy_file_name='', optimized_run='false'):
         """
         :param dict policy: The policy object as provided by the yaml parser
         :param PeerContainer peer_container: The policy will be evaluated against this set of peers
         :param str policy_file_name: The name of the file in which the policy resides
         """
         GenericYamlParser.__init__(self, policy_file_name)
         self.policy = policy
         self.peer_container = peer_container
         self.namespace = None
         self.referenced_labels = set()
+        self.optimized_run = optimized_run
         # map from key to value - info about missing resources
         self.missing_pods_with_labels = {}
 
     def check_dns_subdomain_name(self, value, key_container):
         """
         checking validity of the resource name
         :param string value : The value assigned for the key
@@ -115,15 +118,15 @@
                                   f' of alphanumeric characters, "-", "_" or ".", and must start and end with an '
                                   f'alphanumeric character ', key_container)
 
     def parse_label_selector_requirement(self, requirement, namespace_selector):
         """
         Parse a LabelSelectorRequirement element
         :param dict requirement: The element to parse
-        :param bool namespace_selector: Whether or not this is in the context of namespaceSelector
+        :param bool namespace_selector: Whether this is in the context of namespaceSelector
         :return: A PeerSet containing the peers that satisfy the requirement
         :rtype: Peer.PeerSet
         """
         self.check_fields_validity(requirement, 'LabelSelectorRequirement', {'key': [1, str], 'operator': [1, str],
                                                                              'values': [0, list]},
                                    {'operator': ['In', 'NotIn', 'Exists', 'DoesNotExist']})
         key = requirement['key']
@@ -149,15 +152,15 @@
 
         return None
 
     def parse_label_selector(self, label_selector, namespace_selector=False):
         """
         Parse a LabelSelector element (can also come from a NamespaceSelector)
         :param dict label_selector: The element to parse
-        :param bool namespace_selector: Whether or not this is a namespaceSelector
+        :param bool namespace_selector: Whether this is a namespaceSelector
         :return: A PeerSet containing all the pods captured by this selection
         :rtype: Peer.PeerSet
         """
         if label_selector is None:
             return Peer.PeerSet()  # A None value means the selector selects nothing
         if not label_selector:  # empty
             return self.peer_container.get_all_peers_group()  # An empty value means the selector selects everything
@@ -257,26 +260,25 @@
             res = selected_pods
         return res
 
     def parse_port(self, port):
         """
         Parse an element of the "ports" phrase of a policy rule
         :param dict port: The element to parse
-        :return: A ConnectionSet representing the allowed connections by this element (protocols X port numbers)
-        :rtype: ConnectionSet
+        :return: A protocol and a port_set represented by this element
+        :rtype: tuple (str, PortSet)
         """
         self.check_fields_validity(port, 'NetworkPolicyPort', {'port': 0, 'protocol': [0, str], 'endPort': [0, int]},
                                    {'protocol': ['TCP', 'UDP', 'SCTP']})
         port_id = port.get('port')
         protocol = port.get('protocol')
         end_port_num = port.get('endPort')
         if not protocol:
             protocol = 'TCP'
 
-        res = ConnectionSet()
         dest_port_set = PortSet(port_id is None)
         if port_id is not None and end_port_num is not None:
             if isinstance(port_id, str):
                 self.syntax_error('endPort cannot be defined if the port field is defined '
                                   'as a named (string) port', port)
             if not isinstance(port_id, int):
                 self.syntax_error('type of port is not numerical in NetworkPolicyPort', port)
@@ -297,46 +299,66 @@
                     self.syntax_error('port name should contain only lowercase alphanumeric characters or "-", '
                                       'and start and end with alphanumeric characters', port)
 
             dest_port_set.add_port(port_id)
         elif end_port_num:
             self.syntax_error('endPort cannot be defined if the port field is not defined ', port)
 
-        res.add_connections(protocol, TcpLikeProperties(PortSet(True), dest_port_set))  # K8s doesn't reason about src ports
-        return res
+        return protocol, dest_port_set
 
-    def parse_ingress_egress_rule(self, rule, peer_array_key):
+    def parse_ingress_egress_rule(self, rule, peer_array_key, policy_selected_pods):
         """
         Parse a single ingres/egress rule, producing a K8sPolicyRule
         :param dict rule: The rule to parse
         :param str peer_array_key: The key which defined the peer set ('from' for ingress, 'to' for egress)
-        :return: A K8sPolicyRule with the proper PeerSet and ConnectionSet
+        :param Peer.PeerSet policy_selected_pods: The set of pods the policy applies to
+        :return: K8sPolicyRule with the proper PeerSet and attributes
         :rtype: K8sPolicyRule
         """
         self.check_fields_validity(rule, 'ingress/egress rule', {peer_array_key: [0, list], 'ports': [0, list]})
         peer_array = rule.get(peer_array_key, [])
         if peer_array:
             res_pods = Peer.PeerSet()
             for peer in peer_array:
                 res_pods |= self.parse_peer(peer)
         else:
             res_pods = self.peer_container.get_all_peers_group(True)
 
+        if peer_array_key == 'from':  # ingress
+            src_pods = res_pods
+            dst_pods = policy_selected_pods
+        else:  # egress
+            src_pods = policy_selected_pods
+            dst_pods = res_pods
+
+        res_opt_props = ConnectivityProperties.make_empty_props()
         ports_array = rule.get('ports', [])
         if ports_array:
-            res_ports = ConnectionSet()
+            res_conns = ConnectionSet()
             for port in ports_array:
-                res_ports |= self.parse_port(port)
+                protocol, dest_port_set = self.parse_port(port)
+                if isinstance(protocol, str):
+                    protocol = ProtocolNameResolver.get_protocol_number(protocol)
+                conn_cube = ConnectivityCube.make_from_dict({"dst_ports": dest_port_set})
+                # K8s doesn't reason about src ports
+                res_conns.add_connections(protocol, ConnectivityProperties.make_conn_props(conn_cube))
+                if self.optimized_run != 'false' and src_pods and dst_pods:
+                    protocols = ProtocolSet.get_protocol_set_with_single_protocol(protocol)
+                    conn_cube.update({"protocols": protocols, "src_peers": src_pods, "dst_peers": dst_pods})
+                    conn_props = ConnectivityProperties.make_conn_props(conn_cube)
+                    res_opt_props |= conn_props
         else:
-            res_ports = ConnectionSet(True)
-
+            res_conns = ConnectionSet(True)
+            if self.optimized_run != 'false':
+                res_opt_props = ConnectivityProperties.make_conn_props_from_dict({"src_peers": src_pods,
+                                                                                  "dst_peers": dst_pods})
         if not res_pods:
             self.warning('Rule selects no pods', rule)
 
-        return K8sPolicyRule(res_pods, res_ports)
+        return K8sPolicyRule(res_pods, res_conns, res_opt_props)
 
     def verify_named_ports(self, rule, rule_pods, rule_conns):
         """
         Check the validity of named ports in a given rule: whether a relevant pod refers to the named port and whether
         the protocol defined in the policy matches the protocol defined by the Pod. Issue warnings as required.
         :param dict rule: The unparsed rule (for reference in warnings)
         :param Peer.PeerSet rule_pods: The set of Pods in which the named ports should be defined
@@ -362,32 +384,35 @@
 
     def parse_ingress_rule(self, rule, policy_selected_pods):
         """
         Parse a single ingress rule, producing a K8sPolicyRule.
         Also, checking validity of named ports w.r.t. the policy's captured pods
         :param dict rule: The dict with the rule fields
         :param Peer.PeerSet policy_selected_pods: The set of pods the policy applies to
-        :return: A K8sPolicyRule with the proper PeerSet and ConnectionSet
-        :rtype: K8sPolicyRule
-        """
-        res = self.parse_ingress_egress_rule(rule, 'from')
-        self.verify_named_ports(rule, policy_selected_pods, res.port_set)
-        return res
+        :return: A tuple (K8sPolicyRule, ConnectivityProperties) with the proper PeerSet and attributes, where
+        ConnectivityProperties is an optimized rule format with protocols, src_peers and dst_peers in a HyperCubeSet
+        :rtype: tuple(K8sPolicyRule, ConnectivityProperties)
+        """
+        res_rule = self.parse_ingress_egress_rule(rule, 'from', policy_selected_pods)
+        self.verify_named_ports(rule, policy_selected_pods, res_rule.port_set)
+        return res_rule
 
-    def parse_egress_rule(self, rule):
+    def parse_egress_rule(self, rule, policy_selected_pods):
         """
         Parse a single egress rule, producing a K8sPolicyRule.
         Also, checking validity of named ports w.r.t. the rule's peer set
         :param dict rule: The dict with the rule fields
-        :return: A K8sPolicyRule with the proper PeerSet and ConnectionSet
-        :rtype: K8sPolicyRule
-        """
-        res = self.parse_ingress_egress_rule(rule, 'to')
-        self.verify_named_ports(rule, res.peer_set, res.port_set)
-        return res
+        :param Peer.PeerSet policy_selected_pods: The set of pods the policy applies to
+        :return: A tuple (K8sPolicyRule, ConnectivityProperties) with the proper PeerSet and attributes, where
+        ConnectivityProperties is an optimized rule format with protocols, src_peers and dst_peers in a HyperCubeSet
+        :rtype: tuple(K8sPolicyRule, ConnectivityProperties)
+        """
+        res_rule = self.parse_ingress_egress_rule(rule, 'to', policy_selected_pods)
+        self.verify_named_ports(rule, res_rule.peer_set, res_rule.port_set)
+        return res_rule
 
     def parse_policy(self):
         """
         Parses the input object to create a K8sNetworkPolicy object
         :return: a K8sNetworkPolicy object with proper PeerSets and ConnectionSets
         :rtype: K8sNetworkPolicy
         """
@@ -428,18 +453,20 @@
         pod_selector = policy_spec.get('podSelector')
         res_policy.selected_peers = self.parse_label_selector(pod_selector)
         res_policy.selected_peers &= self.peer_container.get_namespace_pods(self.namespace)
 
         ingress_rules = policy_spec.get('ingress', [])
         if ingress_rules:
             for ingress_rule in ingress_rules:
-                res_policy.add_ingress_rule(self.parse_ingress_rule(ingress_rule, res_policy.selected_peers))
+                rule = self.parse_ingress_rule(ingress_rule, res_policy.selected_peers)
+                res_policy.add_ingress_rule(rule)
 
         egress_rules = policy_spec.get('egress', [])
         if egress_rules:
             for egress_rule in egress_rules:
-                res_policy.add_egress_rule(self.parse_egress_rule(egress_rule))
+                rule = self.parse_egress_rule(egress_rule, res_policy.selected_peers)
+                res_policy.add_egress_rule(rule)
 
         res_policy.findings = self.warning_msgs
         res_policy.referenced_labels = self.referenced_labels
         res_policy.has_ipv6_addresses = self.has_ipv6_addresses
         return res_policy
```

### Comparing `network-config-analyzer-1.9.2/nca/Parsers/K8sServiceYamlParser.py` & `network-config-analyzer-1.9.3/nca/Parsers/K8sServiceYamlParser.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,19 +46,22 @@
         selector = service_spec.get('selector')
         if selector:
             for key, val in selector.items():
                 service.add_selector(key, val)
 
         ports = service_spec.get('ports')
         if ports is not None:
+            port_valid_keys = {'port': [0, int], 'name': [0, str], 'targetPort': 0, 'protocol': [0, str],
+                               'containerPort': 3, 'nodePort': 3, 'appProtocol': 3}
+            port_allowed_values = {'protocol': ['TCP', 'SCTP', 'UDP', 'HTTP', 'HTTPS', 'TLS']}
             for port in ports:
-                port_id = port.get('port')
-                if not port_id:
+                self.check_fields_validity(port, 'port', port_valid_keys, port_allowed_values)
+                port_num = port.get('port')
+                if not port_num:
                     continue
-                target_port = port.get('targetPort')
-                if not target_port:
-                    target_port = port_id
-                name = port.get('name', '')
-                if not service.add_port(K8sService.ServicePort(port_id, target_port,
-                                                               port.get('protocol', 'TCP'), name)):
-                    self.warning(f'The port {name} is not unique in Service {service.name}. Ignoring the port')
+                port_name = port.get('name', '')
+                if not service.add_port(K8sService.ServicePort(port_num=port_num, name=port_name,
+                                                               protocol=port.get('protocol', 'TCP'),
+                                                               target_port=port.get('targetPort', port_num))):
+                    self.warning(f'The port {port_name} is not unique in Service {service.name}. Ignoring the port')
+
         return service
```

### Comparing `network-config-analyzer-1.9.2/nca/Resources/IngressPolicy.py` & `network-config-analyzer-1.9.3/nca/Resources/IngressPolicy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 #
 # Copyright 2020- IBM Inc. All rights reserved
 # SPDX-License-Identifier: Apache2.0
 #
 
-from enum import IntEnum
 from nca.CoreDS.ConnectionSet import ConnectionSet
-from .NetworkPolicy import PolicyConnections, NetworkPolicy
+from nca.CoreDS.ConnectivityProperties import ConnectivityProperties
+from nca.CoreDS.Peer import PeerSet
+from .NetworkPolicy import PolicyConnections, OptimizedPolicyConnections, NetworkPolicy
 
 
 class IngressPolicyRule:
     """
     A class representing a single ingress rule in an Ingress object
     """
-    def __init__(self, peer_set, connections):
+    def __init__(self, peer_set, connections, opt_props):
         """
         :param Peer.PeerSet peer_set: The set of peers this rule allows connection to
         :param ConnectionSet connections: The set of connections allowed by this rule
         """
         self.peer_set = peer_set
         self.connections = connections
+        self.optimized_props = opt_props
+        # copy of optimized props (used by src_peers/dst_peers domain-updating mechanism)
+        self.optimized_props_copy = ConnectivityProperties()
 
     def __eq__(self, other):
         return self.peer_set == other.peer_set and self.connections == other.connections
 
     def contained_in(self, other):
         """
         :param IngressPolicyRule other: Another rule
@@ -35,43 +39,46 @@
 class IngressPolicy(NetworkPolicy):
     """
     This class implements ingress controller logic for incoming http(s) requests
     The logic is kept similarly to NetworkPolicy, where the selected_peers are the ingress controller peers,
     and the rules are egress_rules.
     """
 
-    class ActionType(IntEnum):
-        """
-        Everything that is not defined in Ingress rule's backend or in the default backend is denied
-        """
-        Deny = 0
-        Allow = 1
-
-    def __init__(self, name, namespace, action):
+    def __init__(self, name, namespace):
         """
         :param str name: Ingress name
         :param K8sNamespace namespace: the namespace containing this ingress
-        :param ActionType action: Allow/Deny
         """
         super().__init__(name, namespace)
         self.affects_ingress = False
         self.affects_egress = True
-        self.action = action
 
     def __eq__(self, other):
         return super().__eq__(other)
 
     def add_rules(self, rules):
         """
         Adding a given list of rules to the list of egress rules
         :param list rules: The list of rules to add
         :return: None
         """
         self.egress_rules.extend(rules)
 
+    def sync_opt_props(self):
+        """
+        If optimized props of the policy are not synchronized (self.optimized_props_in_sync is False),
+        compute optimized props of the policy according to the optimized props of its rules
+        """
+        if self.optimized_props_in_sync:
+            return
+        self._init_opt_props()
+        for rule in self.egress_rules:
+            self.optimized_allow_egress_props |= rule.optimized_props
+        self.optimized_props_in_sync = True
+
     def allowed_connections(self, from_peer, to_peer, is_ingress):
         """
         Evaluate the set of connections this ingress resource allows between two peers
         :param Peer.Peer from_peer: The source peer
         :param Peer.Peer to_peer:  The target peer
         :param bool is_ingress: For compatibility with other policies.
          Will return the set of allowed connections only for is_ingress being False.
@@ -82,22 +89,40 @@
         captured = from_peer in self.selected_peers
         if not captured:
             return PolicyConnections(False)
         if is_ingress:
             return PolicyConnections(False)
 
         allowed_conns = ConnectionSet()
-        denied_conns = ConnectionSet()
-        conns = allowed_conns if self.action == IngressPolicy.ActionType.Allow else denied_conns
         for rule in self.egress_rules:
             if to_peer in rule.peer_set:
                 assert not rule.connections.has_named_ports()
-                conns |= rule.connections
+                allowed_conns |= rule.connections
 
-        return PolicyConnections(True, allowed_conns, denied_conns)
+        return PolicyConnections(True, allowed_conns)
+
+    def allowed_connections_optimized(self, is_ingress):
+        """
+        Evaluate the set of connections this ingress resource allows between any two peers
+        :param bool is_ingress: For compatibility with other policies.
+         Will return the set of allowed connections only for is_ingress being False.
+        :return: A ConnectivityProperties object containing all allowed connections for any peers,
+        ConnectivityProperties object containing all denied connections,
+        and the peer set of captured peers by this policy.
+        :rtype: tuple (ConnectivityProperties, ConnectivityProperties, PeerSet)
+        """
+        self.sync_opt_props()
+        res_conns = OptimizedPolicyConnections()
+        if is_ingress:
+            res_conns.allowed_conns = ConnectivityProperties.make_empty_props()
+            res_conns.captured = PeerSet()
+        else:
+            res_conns.allowed_conns = self.optimized_allow_egress_props.copy()
+            res_conns.captured = self.selected_peers if self.affects_egress else PeerSet()
+        return res_conns
 
     def has_empty_rules(self, _config_name=''):
         """
         Checks whether the policy contains empty rules (rules that do not select any peers)
         :param str _config_name: is not used. Kept for compatibility with other policies.
         :return: A list of strings describing the emptiness + two sets of indexes of empty ingress/egress rules
         :rtype: list[str], set, set
@@ -119,38 +144,26 @@
         :param IngressPolicyRule rule_to_exclude: The one rule not to include in the copy
         :param bool ingress_rule: Whether the rule is an ingress or egress rule
         (for compatibility with network policies)
         :return: A copy of 'self' without the provided rule
         :rtype: IngressPolicy
         """
         assert not ingress_rule
-        res = IngressPolicy(self.name, self.namespace, self.action)
+        res = IngressPolicy(self.name, self.namespace)
         res.selected_peers = self.selected_peers
         res.affects_egress = self.affects_egress
         res.affects_ingress = self.affects_ingress
         res.policy_kind = self.policy_kind
         for rule in self.egress_rules:
             if rule != rule_to_exclude:
                 res.add_egress_rule(rule)
         return res
 
     def has_allow_rules(self):
         """
         :return: Whether the policy has rules that allow connections.
         :rtype: bool
         """
-        if self.action == IngressPolicy.ActionType.Allow:
-            for rule in self.egress_rules:
-                if rule.peer_set:
-                    return True
-        return False
-
-    def has_deny_rules(self):
-        """
-        :return: Whether the policy has deny rules
-        :rtype: bool
-        """
-        if self.action == IngressPolicy.ActionType.Deny:
-            for rule in self.egress_rules:
-                if rule.peer_set:
-                    return True
+        for rule in self.egress_rules:
+            if rule.peer_set:
+                return True
         return False
```

### Comparing `network-config-analyzer-1.9.2/nca/Resources/IstioNetworkPolicy.py` & `network-config-analyzer-1.9.3/nca/Resources/IstioNetworkPolicy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 #
 # Copyright 2020- IBM Inc. All rights reserved
 # SPDX-License-Identifier: Apache2.0
 #
 
 from enum import Enum
 from nca.CoreDS.ConnectionSet import ConnectionSet
+from nca.CoreDS.ConnectivityProperties import ConnectivityProperties
 from nca.CoreDS.Peer import PeerSet, IpBlock
-from .NetworkPolicy import PolicyConnections, NetworkPolicy
+from .NetworkPolicy import PolicyConnections, OptimizedPolicyConnections, NetworkPolicy
 
 
 class IstioPolicyRule:
     """
     A class representing a single ingress rule in a Istio AuthorizationPolicy object
     """
 
-    def __init__(self, peer_set, connections):
+    def __init__(self, peer_set, connections, opt_props):
         """
         :param Peer.PeerSet peer_set: The set of peers this rule allows connection from
         :param ConnectionSet connections: The set of connections allowed/denied by this rule (the action resides in the policy)
         """
         # TODO: extend connections (ConnectionSet) to represent HTTP/grpc requests attributes
         self.peer_set = peer_set
         self.connections = connections
+        self.optimized_props = opt_props
+        # copy of optimized props (used by src_peers/dst_peers domain-updating mechanism)
+        self.optimized_props_copy = ConnectivityProperties()
 
     def __eq__(self, other):
         return self.peer_set == other.peer_set and self.connections == other.connections
 
     def contained_in(self, other):
         """
         :param IstioPolicyRule other: Another rule
@@ -60,14 +64,31 @@
 
     def __lt__(self, other):  # required so we can evaluate the policies according to their order
         if isinstance(other, IstioNetworkPolicy):
             # 'deny' policies should be evaluated before 'allow' policies
             return self.action == IstioNetworkPolicy.ActionType.Deny
         return False
 
+    def sync_opt_props(self):
+        """
+        If optimized props of the policy are not synchronized (self.optimized_props_in_sync is False),
+        compute optimized props of the policy according to the optimized props of its rules
+        """
+        if self.optimized_props_in_sync:
+            return
+        self._init_opt_props()
+        for rule in self.ingress_rules:
+            if self.action == IstioNetworkPolicy.ActionType.Allow:
+                self.optimized_allow_ingress_props |= rule.optimized_props
+            elif self.action == IstioNetworkPolicy.ActionType.Deny:
+                self.optimized_deny_ingress_props |= rule.optimized_props
+
+        self.optimized_allow_egress_props = ConnectivityProperties.get_all_conns_props_per_domain_peers()
+        self.optimized_props_in_sync = True
+
     def allowed_connections(self, from_peer, to_peer, is_ingress):
         """
         Evaluate the set of connections this policy allows/denies/passes between two peers
         :param Peer.Peer from_peer: The source peer
         :param Peer.Peer to_peer:  The target peer
         :param bool is_ingress: whether we evaluate ingress rules only or egress rules only
         :return: A PolicyConnections object containing sets of allowed/denied/pass connections
@@ -88,14 +109,35 @@
         collected_conns = allowed_conns if self.action == IstioNetworkPolicy.ActionType.Allow else denied_conns
         for rule in self.ingress_rules:
             if from_peer in rule.peer_set:
                 collected_conns |= rule.connections
 
         return PolicyConnections(True, allowed_conns, denied_conns)
 
+    def allowed_connections_optimized(self, is_ingress):
+        """
+        Evaluate the set of connections this policy allows/denied/passed between any two peers
+        :param bool is_ingress: whether we evaluate ingress rules only or egress rules only
+        :return: A ConnectivityProperties object containing all allowed connections for relevant peers,
+        ConnectivityProperties object containing all denied connections,
+        and the peer set of captured peers by this policy.
+        :rtype: tuple (ConnectivityProperties, ConnectivityProperties, PeerSet)
+        """
+        self.sync_opt_props()
+        res_conns = OptimizedPolicyConnections()
+        if is_ingress:
+            res_conns.allowed_conns = self.optimized_allow_ingress_props.copy()
+            res_conns.denied_conns = self.optimized_deny_ingress_props.copy()
+            res_conns.captured = self.selected_peers
+        else:
+            res_conns.allowed_conns = self.optimized_allow_egress_props.copy()
+            res_conns.denied_conns = self.optimized_deny_egress_props.copy()
+            res_conns.captured = PeerSet()
+        return res_conns
+
     def referenced_ip_blocks(self, exclude_ipv6=False):
         """
         :param bool exclude_ipv6: indicates if to exclude the automatically added IPv6 addresses in the referenced ip_blocks.
         IPv6 addresses that are referenced in the policy by the user will always be included
         :return: A set of all ipblocks referenced in one of the policy rules (one Peer object per one ip range)
         :rtype: Peer.PeerSet
         """
```

### Comparing `network-config-analyzer-1.9.2/nca/Resources/IstioTrafficResources.py` & `network-config-analyzer-1.9.3/nca/Resources/IstioTrafficResources.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 # SPDX-License-Identifier: Apache2.0
 #
 
 from dataclasses import dataclass
 from nca.CoreDS.Peer import PeerSet
 from nca.CoreDS.PortSet import PortSet
 from nca.CoreDS.MinDFA import MinDFA
-from nca.CoreDS.MethodSet import MethodSet
 from .K8sService import K8sService
 
 
 # TODO: istio_root_namespace should be configurable from istio configuration, currently using default value for it
 # If namespace is set to istio root namespace, the policy object applies to all namespaces in a mesh
 istio_root_namespace = 'istio-config'
 
@@ -90,15 +89,15 @@
     class HTTPRoute:
         """
         A class for keeping a parsed http route of a VirtualService
         """
         def __init__(self):
             self.uri_dfa = None
 #            self.scheme_dfa = None  # not supported yet
-            self.methods = MethodSet()
+            self.methods = None
 #            self.authority_dfa = None  # not supported yet
             self.destinations = []
 
         def add_uri_dfa(self, uri_dfa):
             """
             Adds an uri_dfa (to be used as a 'path' property of the connections) to the http route
             :param MinDFA uri_dfa: the uri_dfa to add
```

### Comparing `network-config-analyzer-1.9.2/nca/Resources/K8sNamespace.py` & `network-config-analyzer-1.9.3/nca/Resources/K8sNamespace.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     """
     def __init__(self, name):
         self.name = name if name else 'default'
         # Namespace labels are stored in a dict as key-value pairs
         # Every namespace gets a fixed-key label with its name.
         # See https://kubernetes.io/docs/concepts/services-networking/network-policies/#targeting-a-namespace-by-its-name
         self.labels = {'kubernetes.io/metadata.name': name}
-        self.prior_default_sidecar = None  # the first injected default sidecar of the current namespace
 
     def __eq__(self, other):
         if isinstance(other, K8sNamespace):
             return self.name == other.name
         return False
 
     def __hash__(self):
```

### Comparing `network-config-analyzer-1.9.2/nca/Resources/K8sNetworkPolicy.py` & `network-config-analyzer-1.9.3/nca/Resources/K8sNetworkPolicy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 #
 # Copyright 2020- IBM Inc. All rights reserved
 # SPDX-License-Identifier: Apache2.0
 #
 from nca.CoreDS.ConnectionSet import ConnectionSet
+from nca.CoreDS.ConnectivityProperties import ConnectivityProperties
 from nca.CoreDS import Peer
-from .NetworkPolicy import PolicyConnections, NetworkPolicy
+from .NetworkPolicy import PolicyConnections, OptimizedPolicyConnections, NetworkPolicy
 
 
 class K8sPolicyRule:
     """
     A class representing a single ingress/egress rule in a K8s NetworkPolicy object
     """
-    def __init__(self, peer_set, port_set):
+    def __init__(self, peer_set, port_set, opt_props):
         """
         :param Peer.PeerSet peer_set: The set of peers this rule allows connection to/from
         :param ConnectionSet port_set: The set of connections allowed by this rule
         """
         self.peer_set = peer_set
         self.port_set = port_set
+        self.optimized_props = opt_props
+        # copy of optimized props (used by src_peers/dst_peers domain-updating mechanism)
+        self.optimized_props_copy = ConnectivityProperties()
 
     def __eq__(self, other):
         return self.peer_set == other.peer_set and self.port_set == other.port_set
 
     def contained_in(self, other):
         """
         :param K8sPolicyRule other: Another rule
@@ -31,14 +35,27 @@
         return self.peer_set.issubset(other.peer_set) and self.port_set.contained_in(other.port_set)
 
 
 class K8sNetworkPolicy(NetworkPolicy):
     """
     This class implements K8s-specific logic for NetworkPolicies
     """
+    def sync_opt_props(self):
+        """
+        If optimized props of the policy are not synchronized (self.optimized_props_in_sync is False),
+        compute optimized props of the policy according to the optimized props of its rules
+        """
+        if self.optimized_props_in_sync:
+            return
+        self._init_opt_props()
+        for rule in self.ingress_rules:
+            self.optimized_allow_ingress_props |= rule.optimized_props
+        for rule in self.egress_rules:
+            self.optimized_allow_egress_props |= rule.optimized_props
+        self.optimized_props_in_sync = True
 
     def allowed_connections(self, from_peer, to_peer, is_ingress):
         """
         Evaluate the set of connections this policy allows between two peers
         (either the allowed ingress into to_peer or the allowed egress from from_peer).
         :param Peer.Peer from_peer: The source peer
         :param Peer.Peer to_peer:  The target peer
@@ -58,14 +75,34 @@
             if other_peer in rule.peer_set:
                 rule_conns = rule.port_set.copy()  # we need a copy because convert_named_ports is destructive
                 rule_conns.convert_named_ports(to_peer.get_named_ports())
                 allowed_conns |= rule_conns
 
         return PolicyConnections(True, allowed_conns)
 
+    def allowed_connections_optimized(self, is_ingress):
+        """
+        Return the set of connections this policy allows between any two peers
+        (either ingress or egress).
+        :param bool is_ingress: whether we evaluate ingress rules only or egress rules only
+        :return: A ConnectivityProperties object containing all allowed connections for relevant peers,
+        None for denied connections (K8s does not have denied),
+        and the peer set of captured peers by this policy.
+        :rtype: tuple (ConnectivityProperties, ConnectivityProperties, PeerSet)
+        """
+        self.sync_opt_props()
+        res_conns = OptimizedPolicyConnections()
+        if is_ingress:
+            res_conns.allowed_conns = self.optimized_allow_ingress_props.copy()
+            res_conns.captured = self.selected_peers if self.affects_ingress else Peer.PeerSet()
+        else:
+            res_conns.allowed_conns = self.optimized_allow_egress_props.copy()
+            res_conns.captured = self.selected_peers if self.affects_egress else Peer.PeerSet()
+        return res_conns
+
     def clone_without_rule(self, rule_to_exclude, ingress_rule):
         """
         Makes a copy of 'self' without a given policy rule
         :param K8sPolicyRule rule_to_exclude: The one rule not to include in the copy
         :param bool ingress_rule: Whether the rule is an ingress or egress rule
         :return: A copy of 'self' without the provided rule
         :rtype: K8sNetworkPolicy
```

### Comparing `network-config-analyzer-1.9.2/nca/Resources/K8sService.py` & `network-config-analyzer-1.9.3/nca/Resources/K8sService.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 #
 # Copyright 2020- IBM Inc. All rights reserved
 # SPDX-License-Identifier: Apache2.0
 #
-
+from dataclasses import dataclass
 from enum import Enum
+from typing import Union
+
 from nca.CoreDS.Peer import PeerSet
 
 
 class K8sService:
     """
     Represents a K8s Service, storing its parameters
     """
 
     class ServiceType(Enum):
         ClusterIP = 0  # default
         NodePort = 1
         LoadBalancer = 2
         ExternalName = 3
 
+    @dataclass
     class ServicePort:
         """
         Represents a K8s Service port
         """
-        def __init__(self, port, target_port, protocol, name=''):
-            self.port = port
-            self.target_port = target_port  # a target port may be a number or a string (named port)
-            self.protocol = protocol
-            self.name = name
+        port_num: int
+        name: str
+        protocol: str
+        target_port: Union[str, int]
 
     def __init__(self, name, namespace_name):
         """
         :param str name: a service name
         :param str namespace_name: a namespce name
         """
         self.name = name
@@ -82,21 +84,21 @@
         return list(self.ports.values())[0] if len(self.ports) == 1 else None
 
     def get_port_by_name(self, name):
         return self.ports.get(name)
 
     def get_port_by_number(self, number):
         for port in self.ports.values():
-            if port.port == number:
+            if port.port_num == number:
                 return port
         return None
 
     def add_port(self, service_port):
         """
         Add a service port
-        :param ServicePort service_port: The port to add by the key servicePort.port
+        :param ServicePort service_port: The port to add by the key servicePort.port_num
         :return: True iff successfully added the port, i.e. the port with this name did not exist
         """
         if self.ports.get(service_port.name):
             return False
         self.ports[service_port.name] = service_port
         return True
```

### Comparing `network-config-analyzer-1.9.2/nca/SchemeRunner.py` & `network-config-analyzer-1.9.3/nca/SchemeRunner.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,38 +6,46 @@
 import time
 from os import path
 from nca.FileScanners.GenericTreeScanner import TreeScannerFactory
 from nca.Utils.OutputConfiguration import OutputConfiguration
 from nca.Parsers.GenericYamlParser import GenericYamlParser
 from nca.NetworkConfig.NetworkConfigQueryRunner import NetworkConfigQueryRunner
 from nca.NetworkConfig.ResourcesHandler import ResourcesHandler
+from nca.Utils.ExplTracker import ExplTracker
 
 
 class SchemeRunner(GenericYamlParser):
     """
     This class takes a scheme file, build all its network configurations and runs all its queries
     """
 
-    def __init__(self, scheme_file_name, output_format=None, output_path=None):
+    implemented_opt_queries = {'connectivityMap', 'equivalence', 'vacuity', 'redundancy', 'strongEquivalence'}
+
+    def __init__(self, scheme_file_name, output_format=None, output_path=None, optimized_run='false'):
         GenericYamlParser.__init__(self, scheme_file_name)
         self.network_configs = {}
         self.global_res = 0
         self.output_config_from_cli_args = dict()
         if output_format is not None:
             self.output_config_from_cli_args['outputFormat'] = output_format
         if output_path is not None:
             self.output_config_from_cli_args['outputPath'] = output_path
+        self.optimized_run = optimized_run
 
         scanner = TreeScannerFactory.get_scanner(scheme_file_name)
         for yaml_file in scanner.get_yamls():
             for yaml_doc in yaml_file.data:
                 self.scheme = yaml_doc
                 if not isinstance(self.scheme, dict):
                     self.syntax_error("The scheme's top-level object must be a map")
 
+    @staticmethod
+    def has_implemented_opt_queries(queries):
+        return SchemeRunner.implemented_opt_queries.intersection(queries)
+
     def _get_input_file(self, given_path, out_flag=False):
         """
         Attempts to locate a file specified in the scheme file (possibly relatively to the scheme file)
         :param str given_path: A relative/absolute path to the file
         :param bool out_flag: Indicates if the function is called with expected_output file,
         its absolute path needed even if it doesn't exist
         :return: A path where the file can be located
@@ -69,15 +77,15 @@
                 resource_path = self._get_input_file(resource[:-2])
                 resource_path += '/**'
             else:
                 resource_path = self._get_input_file(resource)
             input_file_list.append(resource_path)
         return input_file_list
 
-    def _add_config(self, config_entry, resources_handler):
+    def _add_config(self, config_entry, resources_handler, optimized_run):
         """
         Produces a NetworkConfig object for a given entry in the scheme file.
         Increases self.global_res if the number of warnings/error in the config does not match the expected number.
         :param dict config_entry: The scheme file entry
         :param ResourcesHandler resources_handler: the resources handler which already include the global peer container
         :return: A matching NetworkConfig object
         :rtype: NetworkConfig
@@ -97,15 +105,15 @@
         if np_list is None and resource_list is None:
             self.syntax_error(f'{config_name} must have an entry for network policies, '
                               f'either with networkPolicyList or resourceList key', config_entry)
         found_error = 0
         expected_error = config_entry.get('expectedError')
         try:
             network_config = resources_handler.get_network_config(np_list, ns_list, pod_list, resource_list,
-                                                                  config_name)
+                                                                  config_name, optimized_run=optimized_run)
             if not network_config:
                 self.warning(f'networkPolicyList {network_config.name} contains no networkPolicies',
                              np_list)
 
             expected_warnings = config_entry.get('expectedWarnings')
             if expected_warnings is not None:
                 warnings_found = network_config.get_num_findings()
@@ -136,21 +144,31 @@
         self.check_fields_validity(self.scheme, 'scheme', allowed_keys)
 
         # global resource files
         global_pod_list = self._handle_resources_list(self.scheme.get('podList', None))
         global_ns_list = self._handle_resources_list(self.scheme.get('namespaceList', None))
         global_resource_list = self._handle_resources_list(self.scheme.get('resourceList', None))
         resources_handler = ResourcesHandler()
-        resources_handler.set_global_peer_container(global_ns_list, global_pod_list, global_resource_list)
+        if self.optimized_run == 'true':
+            # we need to track configurations for the queries to use later-on
+            ExplTracker().activate()
+        resources_handler.set_global_peer_container(global_ns_list, global_pod_list, global_resource_list,
+                                                    self.optimized_run)
 
         # specified configs (non-global)
+        start = time.time()
         for config_entry in self.scheme.get('networkConfigList', []):
-            self._add_config(config_entry, resources_handler)
-
+            self._add_config(config_entry, resources_handler, self.optimized_run)
+        end_parse = time.time()
+        print(f'Finished parsing in {(end_parse - start):6.2f} seconds')
         self.run_queries(self.scheme.get('queries', []))
+        end_queries = time.time()
+        print(f'Parsing time: {(end_parse - start):6.2f} seconds')
+        print(f'Queries time: {(end_queries - end_parse):6.2f} seconds')
+        print(f'Total time: {(end_queries - start):6.2f} seconds')
         return self.global_res
 
     def get_query_output_config_obj(self, query):
         """
         return an output config object based on scheme query and cli arguments
         :param query: a query dict object from scheme file
         :return: an OutputConfiguration object
@@ -178,14 +196,19 @@
 
         for query in query_array:
             res = 0
             comparing_err = 0
             not_executed = 0
             self.check_fields_validity(query, 'query', allowed_elements)
             query_name = query['name']
+            if self.optimized_run == 'debug' or self.optimized_run == 'true':
+                # TODO - update/remove the optimization below when all queries are supported in optimized implementation
+                if not self.has_implemented_opt_queries(set(query.keys())):
+                    print(f'Skipping query {query_name} since it does not have optimized implementation yet')
+                    continue
             print('Running query', query_name)
             output_config_obj = self.get_query_output_config_obj(query)
             expected_output = self._get_input_file(query.get('expectedOutput', None), True)
             start = time.time()
             for query_key in query.keys():
                 if query_key not in ['name', 'expected', 'outputConfiguration', 'expectedOutput', 'expectedNotExecuted']:
                     res, comparing_err, not_executed =\
```

### Comparing `network-config-analyzer-1.9.2/nca/Utils/CmdlineRunner.py` & `network-config-analyzer-1.9.3/nca/Utils/CmdlineRunner.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.2/nca/Utils/NcaLogger.py` & `network-config-analyzer-1.9.3/nca/Utils/NcaLogger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,13 @@
 #
 # Copyright 2022 - IBM Inc. All rights reserved
 # SPDX-License-Identifier: Apache2.0
 #
 import sys
-
-
-class Singleton(type):
-    """
-    A metaclass implementing singleton for NcaLogger
-    """
-    _instances = {}
-
-    def __call__(cls, *args, **kwargs):
-        if cls not in cls._instances:
-            cls._instances[cls] = super(Singleton, cls).__call__(*args, **kwargs)
-        return cls._instances[cls]
+from nca.Utils.Utils import Singleton
 
 
 class NcaLogger(metaclass=Singleton):
     """
     NcaLogger is used to control warning messages issued by GenericYamlParser.
     Any warning message is sent to NcaLogger().log_message()
 
@@ -84,22 +73,26 @@
         return self._is_collecting_msgs
 
     def log_message(self, msg, file=None, level=None):
         """
         Log a message
         :param sting msg: message to log
         :param a file-like-object file: output stream
-        :param str level: the level of the message: (I)nfo, (W)arning
+        :param str level: the level of the message: (I)nfo, (W)arning, (E)rror
         """
         if level == 'I':
             msg = f'Info: {msg}'
         elif level == 'W':
             msg = f'Warning: {msg}'
             if not file:
                 file = sys.stderr
+        elif level == 'E':
+            msg = f'Error: {msg}'
+            if not file:
+                file = sys.stderr
 
         if self._is_collecting_msgs:
             if self.is_mute():
                 self._collected_messages.append(msg)
             else:
                 print(msg, file=file)
```

### Comparing `network-config-analyzer-1.9.2/nca/Utils/OutputConfiguration.py` & `network-config-analyzer-1.9.3/nca/Utils/OutputConfiguration.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #
 # Copyright 2020- IBM Inc. All rights reserved
 # SPDX-License-Identifier: Apache2.0
 #
 
 import json
 import os
+import sys
 from urllib import request
 from nca.Utils.CmdlineRunner import CmdlineRunner
 
 
 class OutputConfiguration(dict):
     """
     a class to handle output configuration per query
@@ -16,15 +17,15 @@
 
     def __init__(self, output_config_dict=None, query_name=''):
         default_output_config = {'fwRulesRunInTestMode': False, 'fwRulesDebug': False,
                                  'fwRulesGroupByLabelSinglePod': False, 'fwRulesFilterSystemNs': False,
                                  'fwRulesMaxIter': 10, 'outputFormat': 'txt', 'outputPath': None,
                                  'fwRulesOverrideAllowedLabels': None, 'prURL': None,
                                  'connectivityFilterIstioEdges': True, 'outputEndpoints': 'deployments',
-                                 'subset': {}, 'fullExplanation': False, 'excludeIPv6Range': True}
+                                 'subset': {}, 'explain': None, 'fullExplanation': False, 'excludeIPv6Range': True}
 
         super().__init__(default_output_config)
         if output_config_dict is not None:
             self.update(output_config_dict)
 
         self.queryName = query_name
         self.configName = ''
@@ -45,29 +46,33 @@
             print(f'{self.outputFormat} output format is not supported for this query')
             return
         path = self.outputPath
         if path is not None:
             # print output to a file
             if self.outputFormat == 'jpg':
                 tmp_dot_file = f'{path}.nca_tmp.dot'
+                dot_cmd = ['dot', tmp_dot_file, '-Tjpg', f'-o{path}']
                 try:
                     with open(tmp_dot_file, "w") as f:
                         f.write(output)
-                    CmdlineRunner.run_and_get_output(['dot', tmp_dot_file, '-Tjpg', f'-o{path}'])
+                    CmdlineRunner.run_and_get_output(dot_cmd)
                 except Exception as e:
-                    print(f'Failed to create a jpg file: {path}\n{e}')
+                    print(f'Failed to create a jpg file: {path}\n{e}', file=sys.stderr)
+                if not os.path.isfile(path):
+                    dot_cmd_string = ' '.join(dot_cmd)
+                    print(f'Command {dot_cmd_string}\n did not create {path}\n', file=sys.stderr)
                 if os.path.isfile(tmp_dot_file):
                     os.remove(tmp_dot_file)
             else:
                 try:
                     with open(path, "a") as f:
                         f.write(output)
                     print(f'wrote query output to: {path}')
                 except FileNotFoundError:
-                    print(f'FileNotFoundError: configured outputPath is: {path}')
+                    print(f'FileNotFoundError: configured outputPath is: {path}', file=sys.stderr)
         elif self.prURL is not None:
             self.write_git_comment(output)
         else:
             # print output to stdout
             print(output)
 
     def write_git_comment(self, comment_body):
```

### Comparing `network-config-analyzer-1.9.2/nca/Utils/OutputFilesFlags.py` & `network-config-analyzer-1.9.3/nca/Utils/OutputFilesFlags.py`

 * *Files identical despite different names*

### Comparing `network-config-analyzer-1.9.2/nca/nca_cli.py` & `network-config-analyzer-1.9.3/nca/nca_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 import argparse
 import time
 import os
 import sys
 import traceback
 from sys import stderr
 from pathlib import Path
+from nca.CoreDS.Peer import BasePeerSet
 from nca.Utils.OutputConfiguration import OutputConfiguration
 from nca.NetworkConfig.NetworkConfigQueryRunner import NetworkConfigQueryRunner
 from nca.NetworkConfig.ResourcesHandler import ResourcesHandler
 from nca.SchemeRunner import SchemeRunner
+from nca.Utils.ExplTracker import ExplTracker
 
 
 def _valid_path(path_location, allow_ghe=False, allowed_platforms=None):
     """
     A validator for paths in the command line, raising an exception if the path is invalid
     :param str path_location: The path to validate
     :param bool allow_ghe: Whether to allow url to github
@@ -128,33 +130,37 @@
     if path_list:
         for index, path in enumerate(path_list):
             if os.path.isdir(path):
                 path_list[index] = str(path) + '**'
     return path_list
 
 
-def run_args(args):
+def run_args(args):  # noqa: C901
     """
     Given the parsed cmdline, decide what to run
     :param Namespace args: argparse-style parsed cmdline
     :return: The number of queries with unexpected value (if a scheme file is used) or
              the query result (if command-line queries are used)
     :rtype: int
     """
+    # reset the singleton before running a new shceme or cli query
+    # so that configs from certain run do not affect a potential following run.
+    BasePeerSet.reset()
     if args.scheme:
-        return SchemeRunner(args.scheme, args.output_format, args.file_out).run_scheme()
+        return SchemeRunner(args.scheme, args.output_format, args.file_out, args.optimized_run).run_scheme()
     ns_list = args.ns_list
     pod_list = args.pod_list
     resource_list = args.resource_list
 
     output_config = OutputConfiguration({'outputFormat': args.output_format or 'txt',
                                          'outputPath': args.file_out or None,
                                          'prURL': args.pr_url or None,
                                          'outputEndpoints': args.output_endpoints,
                                          'subset': {},
+                                         'explain': [],
                                          'excludeIPv6Range': not args.print_ipv6})
     expected_output = None
     # default values are for sanity query
     # np_list will be taken as args.<query_name> if it is not equal to the args parser's const value i.e ['']
     np_list = args.sanity if args.sanity != [''] else None
     pair_query_flag = False
     query_name = 'sanity'
@@ -174,14 +180,19 @@
             lbl_dict = {}
             for lbl in lbl_list:
                 key, value = lbl.split(':')
                 lbl_dict[key] = value
             all_labels.append(lbl_dict)
         output_config['subset'].update({'label_subset': all_labels})
 
+    if args.explain is not None and args.optimized_run == 'true':
+        output_config['explain'] = args.explain
+        ExplTracker().activate()
+        ExplTracker().set_endpoints(output_config.outputEndpoints)
+
     if args.equiv is not None:
         np_list = args.equiv if args.equiv != [''] else None
         query_name = 'twoWayContainment'
         pair_query_flag = True
         base_as_second = True
 
     if args.interferes is not None:
@@ -208,27 +219,34 @@
 
     if args.semantic_diff is not None:
         np_list = args.semantic_diff if args.semantic_diff != [''] else None
         query_name = 'semanticDiff'
         pair_query_flag = True
         expected_output = args.expected_output or None
 
+    if args.optimized_run == 'debug' or args.optimized_run == 'true':
+        # TODO - update/remove the optimization below when all queries are supported in optimized implementation
+        if not SchemeRunner.has_implemented_opt_queries({query_name}):
+            print(f'Not running query {query_name} since it does not have optimized implementation yet')
+            return _compute_return_value(0, 0, 1)
+
     resources_handler = ResourcesHandler()
     network_config = resources_handler.get_network_config(_make_recursive(np_list), _make_recursive(ns_list),
                                                           _make_recursive(pod_list), _make_recursive(resource_list),
-                                                          save_flag=pair_query_flag)
+                                                          save_flag=pair_query_flag, optimized_run=args.optimized_run)
     if pair_query_flag:
         base_np_list = args.base_np_list
         base_resource_list = args.base_resource_list
         base_ns_list = args.base_ns_list
         base_pod_list = args.base_pod_list
         base_network_config = resources_handler.get_network_config(_make_recursive(base_np_list),
                                                                    _make_recursive(base_ns_list),
                                                                    _make_recursive(base_pod_list),
-                                                                   _make_recursive(base_resource_list))
+                                                                   _make_recursive(base_resource_list),
+                                                                   optimized_run=args.optimized_run)
         if base_as_second:
             network_configs_array = [network_config, base_network_config]
         else:
             network_configs_array = [base_network_config, network_config]
         return _execute_pair_configs_query(query_name, network_configs_array,
                                            output_config, expected_output)
 
@@ -289,32 +307,38 @@
     parser.add_argument('--ns_list', '-n', type=_namespace_list_valid_path, action='append',
                         help='A file/GHE url/cluster-type to read namespace list from '
                              '(may be specified multiple times)')
     parser.add_argument('--pod_list', '-p', type=_pod_list_valid_path, action='append',
                         help='A file/GHE url/cluster-type to read pod list from (may be specified multiple times)')
     parser.add_argument('--resource_list', '-r', type=_resource_list_valid_path, action='append',
                         help='Network policies entries or Filesystem or GHE location of base network resources ')
+    parser.add_argument('--explain', '-expl', type=str,
+                        help='A node or 2 nodes (a connection), to explain the configurations affecting them')
     parser.add_argument('--deployment_subset', '-ds', type=str,
                         help='A list of deployment names to subset the query by')
     parser.add_argument('--namespace_subset', '-nss', type=str,
                         help='A list of namespaces to subset the query by')
     parser.add_argument('--label_subset', '-lss', type=str, action='append',
                         help='A list of labels to subset the query by')
     parser.add_argument('--ghe_token', '--gh_token', type=str, help='A valid token to access a GitHub repository')
     parser.add_argument('--output_format', '-o', type=str,
-                        help='Output format specification (txt, csv, md, dot, jpg or yaml). The default is txt.')
+                        help='Output format specification (txt, txt_no_fw_rules, csv, md, dot, jpg or yaml). '
+                             'The default is txt.')
     parser.add_argument('--file_out', '-f', type=str, help='A file path to which output is redirected')
     parser.add_argument('--expected_output', type=str, help='A file path of the expected query output,'
                                                             'relevant only with --connectivity and --semantic_diff')
     parser.add_argument('--pr_url', type=str, help='The full api url for adding a PR comment')
     parser.add_argument('--return_0', action='store_true', help='Force a return value 0')
     parser.add_argument('--version', '-v', action='store_true', help='Print version and exit')
     parser.add_argument('--debug', '-d', action='store_true', help='Print debug information')
     parser.add_argument('--output_endpoints', choices=['pods', 'deployments'],
                         help='Choose endpoints type in output (pods/deployments)', default='deployments')
+    parser.add_argument('--optimized_run', '-opt', type=str,
+                        help='Whether to run optimized run (-opt=true), original run (-opt=false) - the default '
+                             'or the comparison of the both (debug)', default='false')
     parser.add_argument('--print_ipv6', action='store_true', help='Display IPv6 addresses connections too. '
                                                                   'If the policy reference IPv6 addresses, '
                                                                   'their connections will be printed anyway')
 
     args = parser.parse_args(argv)
 
     if args.version:
@@ -322,17 +346,20 @@
         with open(version_file_path) as version_file:
             print(f'NCA version {version_file.readline()}')
         return 0
 
     if args.ghe_token:
         os.environ['GHE_TOKEN'] = args.ghe_token
 
+    start = time.time()
     try:
         if args.period <= 0:
             ret_val = run_args(args)
+            end = time.time()
+            print(f'Total run time: {(end - start):6.2f} seconds')
             return 0 if args.return_0 else ret_val
 
         _do_every(args.period * 60, run_args, args)
     except Exception as e:
         print(f'Error: {e}', file=stderr)
         if args.debug:
             print(traceback.format_exc(), file=stderr)
```

### Comparing `network-config-analyzer-1.9.2/network_config_analyzer.egg-info/PKG-INFO` & `network-config-analyzer-1.9.3/network_config_analyzer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: network-config-analyzer
-Version: 1.9.2
+Version: 1.9.3
 Summary: An analyzer for Network Policies and other connectivity-configuration resources
 Home-page: https://github.com/IBM/network-config-analyzer
 Author: Ziv Nevo
 Author-email: nevo@il.ibm.com
 Project-URL: Bug Tracker, https://github.com/IBM/network-config-analyzer/issues
 Project-URL: NP-Guard Home, https://np-guard.github.io
 Classifier: Programming Language :: Python :: 3
@@ -97,29 +97,35 @@
 - `--label_subset  <A comma separated list of pairs (key:value) of labels (no spaces allowed)>`\
   Specifies the labels to include in the 'connectivity' query results. An element should include all the labels in this list to be included in the subset and in the results (AND operation). This switch may be specified multiple times and an element will be included if it matches one of the label-sets given in one of the switches (OR operation).
 - `--ghe_token <token>`\
   A valid token to access a GHE repository
 - `--period <minutes>`\
   Run NCA with given arguments every specified number of minutes
 - `--output_format <format>`\
-  Output format specification (txt/yaml/csv/md/dot/jpg).\
-  For jpg format, Graphviz executables must be installed and on user systems' PATH.\
+  Output format specification (txt/yaml/csv/md/dot/jpg/txt_no_fw_rules).\
+  `jpg` : Graphviz executables must be installed and on user systems' PATH.\
+  `txt_no_fw_rules`: supported for ConnectivityMap and SemanticDiff queries, printing connectivity rules for each pair of peers, without minimization and grouping of rules. (excluding  connections between workload to itself).
   *default:* txt\
   *shorthand:* `-o`
 - `--file_out <file name>`\
   A file path to redirect output into.\
   *shorthand* `-f`
 - `--expected_output <file name>`\
   A file path to the expected query output (for connectivity or semantic_diff queries).\
 - `--pr_url <URL>`\
    Write output as GitHub PR comment. URL points to the relevant `comments` resource in the GitHub API.\
    e.g., https://api.github.com/repos/shift-left-netconfig/online-boutique/issues/1/comments
 - `--output_endpoints`\
   Choose endpoints type in output (pods/deployments).\
   *default:* deployments
+  - `--explain`\
+  A pair of node names (comma separated) to explain the policies affecting their connection or lack of it. Relevant only for connectivity query.\
+  Connections including IP-Blocks will show only the configurations of the node in that connection (since, IP-Blocks does
+  not have configurations). IP-Blocks should be places in CIDR format as seen in the query results (run the connectivity query first, to see the nodes there).\
+  e.g. default/pod-A1,default/deployment-B1.
   - `--print_ipv6`\
   include IPv6 range in the query results even when the policies of the config do not contain any IPv6 addresses.
   
 
 For more information on command-line switches combinations, see [Common Query Patterns](docs/CommonQueryPatterns.md#cmdline-queries)
 
 ##### Simulating live cluster missing resources:
```

### Comparing `network-config-analyzer-1.9.2/network_config_analyzer.egg-info/SOURCES.txt` & `network-config-analyzer-1.9.3/network_config_analyzer.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,26 +7,29 @@
 nca/VERSION.txt
 nca/__init__.py
 nca/__main__.py
 nca/nca_cli.py
 nca/CoreDS/CanonicalHyperCubeSet.py
 nca/CoreDS/CanonicalIntervalSet.py
 nca/CoreDS/ConnectionSet.py
+nca/CoreDS/ConnectivityCube.py
+nca/CoreDS/ConnectivityProperties.py
 nca/CoreDS/DimensionsManager.py
-nca/CoreDS/ICMPDataSet.py
 nca/CoreDS/MethodSet.py
 nca/CoreDS/MinDFA.py
 nca/CoreDS/Peer.py
 nca/CoreDS/PortSet.py
 nca/CoreDS/ProtocolNameResolver.py
-nca/CoreDS/TcpLikeProperties.py
+nca/CoreDS/ProtocolSet.py
 nca/CoreDS/__init__.py
 nca/FWRules/ClusterInfo.py
 nca/FWRules/ConnectivityGraph.py
+nca/FWRules/DotGraph.py
 nca/FWRules/FWRule.py
+nca/FWRules/InteractiveConnectivityGraph.py
 nca/FWRules/MinimizeFWRules.py
 nca/FWRules/__init__.py
 nca/FileScanners/DirScanner.py
 nca/FileScanners/GenericTreeScanner.py
 nca/FileScanners/GitScanner.py
 nca/FileScanners/HelmScanner.py
 nca/FileScanners/__init__.py
@@ -46,14 +49,15 @@
 nca/NetworkConfig/LiveSim/istio_gateway/istio_gateway.yaml
 nca/Parsers/CalicoPolicyYamlParser.py
 nca/Parsers/GenericIngressLikeYamlParser.py
 nca/Parsers/GenericYamlParser.py
 nca/Parsers/IngressPolicyYamlParser.py
 nca/Parsers/IstioGenericYamlParser.py
 nca/Parsers/IstioPolicyYamlParser.py
+nca/Parsers/IstioServiceEntryYamlParser.py
 nca/Parsers/IstioSidecarYamlParser.py
 nca/Parsers/IstioTrafficResourcesYamlParser.py
 nca/Parsers/K8sPolicyYamlParser.py
 nca/Parsers/K8sServiceYamlParser.py
 nca/Parsers/__init__.py
 nca/Resources/CalicoNetworkPolicy.py
 nca/Resources/IngressPolicy.py
@@ -62,17 +66,19 @@
 nca/Resources/IstioTrafficResources.py
 nca/Resources/K8sNamespace.py
 nca/Resources/K8sNetworkPolicy.py
 nca/Resources/K8sService.py
 nca/Resources/NetworkPolicy.py
 nca/Resources/__init__.py
 nca/Utils/CmdlineRunner.py
+nca/Utils/ExplTracker.py
 nca/Utils/NcaLogger.py
 nca/Utils/OutputConfiguration.py
 nca/Utils/OutputFilesFlags.py
+nca/Utils/Utils.py
 nca/Utils/__init__.py
 network_config_analyzer.egg-info/PKG-INFO
 network_config_analyzer.egg-info/SOURCES.txt
 network_config_analyzer.egg-info/dependency_links.txt
 network_config_analyzer.egg-info/entry_points.txt
 network_config_analyzer.egg-info/requires.txt
 network_config_analyzer.egg-info/top_level.txt
```

### Comparing `network-config-analyzer-1.9.2/setup.cfg` & `network-config-analyzer-1.9.3/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,19 @@
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 
 [options]
 packages = find_namespace:
 include_package_data = True
 install_requires = 
-	ghapi==1.0.3
+	ghapi==1.0.4
 	PyYAML==6.0
 	greenery==4.0.0
+	networkx==3.1
+	beautifulsoup4==4.12.0
 python_requires = >=3.8
 
 [options.packages.find]
 include = nca*
 
 [options.package_data]
 * = VERSION.txt
```


# Comparing `tmp/pyipv8-2.8.0.tar.gz` & `tmp/pyipv8-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyipv8-2.8.0.tar", last modified: Wed Oct 27 07:17:53 2021, max compression
+gzip compressed data, was "pyipv8-2.9.0.tar", last modified: Fri Jun 24 09:51:20 2022, max compression
```

## Comparing `pyipv8-2.8.0.tar` & `pyipv8-2.9.0.tar`

### file list

```diff
@@ -1,289 +1,290 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.745526 pyipv8-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     7651 2021-10-27 07:17:39.000000 pyipv8-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5290 2021-10-27 07:17:53.745526 pyipv8-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4362 2021-10-27 07:17:39.000000 pyipv8-2.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.709526 pyipv8-2.8.0/ipv8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.709526 pyipv8-2.8.0/ipv8/REST/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/REST/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8650 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/REST/asyncio_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)    16281 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/REST/attestation_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     1300 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/REST/base_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)    12234 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/REST/dht_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)    23146 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/REST/identity_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     2900 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/REST/isolation_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     1472 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/REST/network_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     2081 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/REST/noblock_dht_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     7069 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/REST/overlays_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     4334 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/REST/rest_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     1285 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/REST/root_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     2817 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/REST/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)    15352 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/REST/tunnel_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.709526 pyipv8-2.8.0/ipv8/attestation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14330 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/communication_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     2221 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/default_identity_formats.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.713526 pyipv8-2.8.0/ipv8/attestation/identity/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2207 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/identity/attestation.py
--rw-r--r--   0 runner    (1001) docker     (121)    16321 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/identity/community.py
--rw-r--r--   0 runner    (1001) docker     (121)     8367 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/identity/database.py
--rw-r--r--   0 runner    (1001) docker     (121)    10851 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/identity/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     3465 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/identity/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)      779 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/identity/payload.py
--rw-r--r--   0 runner    (1001) docker     (121)     6039 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/identity_formats.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.713526 pyipv8-2.8.0/ipv8/attestation/schema/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3924 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/schema/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     3114 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/signed_object.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.713526 pyipv8-2.8.0/ipv8/attestation/tokentree/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/tokentree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4884 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/tokentree/token.py
--rw-r--r--   0 runner    (1001) docker     (121)     8739 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/tokentree/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.713526 pyipv8-2.8.0/ipv8/attestation/wallet/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.713526 pyipv8-2.8.0/ipv8/attestation/wallet/bonehexact/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/bonehexact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6672 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/bonehexact/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (121)     4826 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/bonehexact/attestation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2129 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/bonehexact/structs.py
--rw-r--r--   0 runner    (1001) docker     (121)     3662 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/caches.py
--rw-r--r--   0 runner    (1001) docker     (121)    23020 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/community.py
--rw-r--r--   0 runner    (1001) docker     (121)     4110 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/database.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.717526 pyipv8-2.8.0/ipv8/attestation/wallet/irmaexact/
--rw-r--r--   0 runner    (1001) docker     (121)      360 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/irmaexact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4853 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/irmaexact/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (121)     7560 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/irmaexact/enroll_script.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.717526 pyipv8-2.8.0/ipv8/attestation/wallet/irmaexact/gabi/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/irmaexact/gabi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4832 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/irmaexact/gabi/attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)     7439 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/irmaexact/gabi/builder.py
--rw-r--r--   0 runner    (1001) docker     (121)     5114 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/irmaexact/gabi/credential.py
--rw-r--r--   0 runner    (1001) docker     (121)     7009 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/irmaexact/gabi/keys.py
--rw-r--r--   0 runner    (1001) docker     (121)     5428 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/irmaexact/gabi/proofs.py
--rw-r--r--   0 runner    (1001) docker     (121)    27620 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/irmaexact/keydump.py
--rw-r--r--   0 runner    (1001) docker     (121)      755 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/irmaexact/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2694 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/payload.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.717526 pyipv8-2.8.0/ipv8/attestation/wallet/pengbaorange/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/pengbaorange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6871 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/pengbaorange/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/pengbaorange/attestation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4606 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/pengbaorange/boudot.py
--rw-r--r--   0 runner    (1001) docker     (121)     9445 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/pengbaorange/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.721526 pyipv8-2.8.0/ipv8/attestation/wallet/primitives/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      909 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/primitives/attestation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3617 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/primitives/boneh.py
--rw-r--r--   0 runner    (1001) docker     (121)     2334 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/primitives/cryptography_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2209 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/primitives/ec.py
--rw-r--r--   0 runner    (1001) docker     (121)     2575 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/primitives/structs.py
--rw-r--r--   0 runner    (1001) docker     (121)     8075 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/attestation/wallet/primitives/value.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.721526 pyipv8-2.8.0/ipv8/bootstrapping/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/bootstrapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2127 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/bootstrapping/bootstrapper_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.721526 pyipv8-2.8.0/ipv8/bootstrapping/dispersy/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/bootstrapping/dispersy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2897 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/bootstrapping/dispersy/bootstrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.721526 pyipv8-2.8.0/ipv8/bootstrapping/udpbroadcast/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/bootstrapping/udpbroadcast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3745 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/bootstrapping/udpbroadcast/bootstrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)    23995 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/community.py
--rw-r--r--   0 runner    (1001) docker     (121)    16261 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)    15631 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/database.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.721526 pyipv8-2.8.0/ipv8/dht/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/dht/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1925 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/dht/churn.py
--rw-r--r--   0 runner    (1001) docker     (121)    22886 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/dht/community.py
--rw-r--r--   0 runner    (1001) docker     (121)     8373 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/dht/discovery.py
--rw-r--r--   0 runner    (1001) docker     (121)     2437 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/dht/payload.py
--rw-r--r--   0 runner    (1001) docker     (121)     3011 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/dht/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     7978 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/dht/routing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2116 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/dht/storage.py
--rw-r--r--   0 runner    (1001) docker     (121)     3443 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/dht/trie.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.725526 pyipv8-2.8.0/ipv8/keyvault/
--rw-r--r--   0 runner    (1001) docker     (121)      883 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/keyvault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4840 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/keyvault/crypto.py
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/keyvault/keys.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.725526 pyipv8-2.8.0/ipv8/keyvault/private/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/keyvault/private/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1611 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/keyvault/private/libnaclkey.py
--rw-r--r--   0 runner    (1001) docker     (121)     3618 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/keyvault/private/m2crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.725526 pyipv8-2.8.0/ipv8/keyvault/public/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/keyvault/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1729 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/keyvault/public/libnaclkey.py
--rw-r--r--   0 runner    (1001) docker     (121)     3180 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/keyvault/public/m2crypto.py
--rw-r--r--   0 runner    (1001) docker     (121)    11240 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/lazy_community.py
--rw-r--r--   0 runner    (1001) docker     (121)    17292 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.725526 pyipv8-2.8.0/ipv8/messaging/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/messaging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.725526 pyipv8-2.8.0/ipv8/messaging/anonymization/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/messaging/anonymization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5364 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/messaging/anonymization/caches.py
--rw-r--r--   0 runner    (1001) docker     (121)    45331 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/messaging/anonymization/community.py
--rw-r--r--   0 runner    (1001) docker     (121)     2426 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/messaging/anonymization/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)    27957 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/messaging/anonymization/hidden_services.py
--rw-r--r--   0 runner    (1001) docker     (121)     8657 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/messaging/anonymization/payload.py
--rw-r--r--   0 runner    (1001) docker     (121)     3611 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/messaging/anonymization/pex.py
--rw-r--r--   0 runner    (1001) docker     (121)    16807 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/messaging/anonymization/tunnel.py
--rw-r--r--   0 runner    (1001) docker     (121)     2692 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/messaging/anonymization/tunnelcrypto.py
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/messaging/anonymization/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.725526 pyipv8-2.8.0/ipv8/messaging/interfaces/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/messaging/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.729526 pyipv8-2.8.0/ipv8/messaging/interfaces/dispatcher/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/messaging/interfaces/dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5592 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/messaging/interfaces/dispatcher/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)    14360 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/messaging/interfaces/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     1979 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/messaging/interfaces/network_stats.py
--rw-r--r--   0 runner    (1001) docker     (121)     6437 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/messaging/interfaces/statistics_endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.729526 pyipv8-2.8.0/ipv8/messaging/interfaces/udp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/messaging/interfaces/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4442 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/messaging/interfaces/udp/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     8795 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/messaging/lazy_payload.py
--rw-r--r--   0 runner    (1001) docker     (121)    12078 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/messaging/payload.py
--rw-r--r--   0 runner    (1001) docker     (121)     2886 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/messaging/payload_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (121)      870 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/messaging/payload_headers.py
--rw-r--r--   0 runner    (1001) docker     (121)    16532 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/messaging/serialization.py
--rw-r--r--   0 runner    (1001) docker     (121)     3930 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/overlay.py
--rw-r--r--   0 runner    (1001) docker     (121)     6196 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/peer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.729526 pyipv8-2.8.0/ipv8/peerdiscovery/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/peerdiscovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2618 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/peerdiscovery/churn.py
--rw-r--r--   0 runner    (1001) docker     (121)     7906 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/peerdiscovery/community.py
--rw-r--r--   0 runner    (1001) docker     (121)     6977 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/peerdiscovery/discovery.py
--rw-r--r--   0 runner    (1001) docker     (121)    14860 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/peerdiscovery/network.py
--rw-r--r--   0 runner    (1001) docker     (121)     4856 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/peerdiscovery/payload.py
--rw-r--r--   0 runner    (1001) docker     (121)    10844 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/requestcache.py
--rw-r--r--   0 runner    (1001) docker     (121)     7874 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/taskmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.729526 pyipv8-2.8.0/ipv8/test/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.733526 pyipv8-2.8.0/ipv8/test/REST/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/REST/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5518 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/REST/rest_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    19898 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/REST/test_attestation_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)    18919 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/REST/test_identity_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     4085 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/REST/test_isolation_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     5042 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/REST/test_network_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)    13042 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/REST/test_overlays_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.733526 pyipv8-2.8.0/ipv8/test/attestation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.733526 pyipv8-2.8.0/ipv8/test/attestation/identity/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7902 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/identity/test_identity.py
--rw-r--r--   0 runner    (1001) docker     (121)     7671 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/identity/test_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.733526 pyipv8-2.8.0/ipv8/test/attestation/tokentree/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/tokentree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3883 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/tokentree/test_token.py
--rw-r--r--   0 runner    (1001) docker     (121)     8718 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/tokentree/test_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.733526 pyipv8-2.8.0/ipv8/test/attestation/wallet/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1617 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/wallet/attestation.txt
--rw-r--r--   0 runner    (1001) docker     (121)    12341 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/wallet/attestation_big.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3388 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/wallet/attestation_range.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.733526 pyipv8-2.8.0/ipv8/test/attestation/wallet/bonehexact/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/wallet/bonehexact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4221 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/wallet/bonehexact/test_attestation.py
--rw-r--r--   0 runner    (1001) docker     (121)     9738 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/wallet/bonehexact/test_structs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.733526 pyipv8-2.8.0/ipv8/test/attestation/wallet/irmaexact/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/wallet/irmaexact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5618 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/wallet/irmaexact/test_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (121)     6449 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/wallet/irmaexact/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)    22325 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/wallet/irmaexact/test_credential.py
--rw-r--r--   0 runner    (1001) docker     (121)      874 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/wallet/irmaexact/test_keys.py
--rw-r--r--   0 runner    (1001) docker     (121)     8940 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/wallet/irmaexact/test_proofs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.733526 pyipv8-2.8.0/ipv8/test/attestation/wallet/pengbaorange/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/wallet/pengbaorange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6135 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/wallet/pengbaorange/test_boudot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.737526 pyipv8-2.8.0/ipv8/test/attestation/wallet/primitives/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/wallet/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5128 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/wallet/primitives/test_boneh.py
--rw-r--r--   0 runner    (1001) docker     (121)     1966 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/wallet/primitives/test_ec.py
--rw-r--r--   0 runner    (1001) docker     (121)     8344 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/wallet/primitives/test_value.py
--rw-r--r--   0 runner    (1001) docker     (121)    12823 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/attestation/wallet/test_attestation_community.py
--rw-r--r--   0 runner    (1001) docker     (121)     9983 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.737526 pyipv8-2.8.0/ipv8/test/bootstrapping/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/bootstrapping/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.737526 pyipv8-2.8.0/ipv8/test/bootstrapping/dispersy/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/bootstrapping/dispersy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3323 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/bootstrapping/dispersy/test_bootstrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.737526 pyipv8-2.8.0/ipv8/test/dht/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/dht/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      356 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/dht/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/dht/test_churn.py
--rw-r--r--   0 runner    (1001) docker     (121)    10050 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/dht/test_community.py
--rw-r--r--   0 runner    (1001) docker     (121)     4129 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/dht/test_discovery.py
--rw-r--r--   0 runner    (1001) docker     (121)     2925 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/dht/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     7130 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/dht/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1217 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/dht/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (121)     2760 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/dht/test_trie.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.737526 pyipv8-2.8.0/ipv8/test/keyvault/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/keyvault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5721 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/keyvault/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (121)     2596 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/keyvault/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (121)     2371 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/keyvault/test_signature.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.737526 pyipv8-2.8.0/ipv8/test/messaging/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/messaging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.737526 pyipv8-2.8.0/ipv8/test/messaging/anonymization/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/messaging/anonymization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      619 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/messaging/anonymization/mock.py
--rw-r--r--   0 runner    (1001) docker     (121)    20461 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/messaging/anonymization/test_community.py
--rw-r--r--   0 runner    (1001) docker     (121)     2706 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/messaging/anonymization/test_datachecker.py
--rw-r--r--   0 runner    (1001) docker     (121)     2047 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/messaging/anonymization/test_exit_socket.py
--rw-r--r--   0 runner    (1001) docker     (121)    13788 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/messaging/anonymization/test_hiddenservices.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.741526 pyipv8-2.8.0/ipv8/test/messaging/interfaces/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/messaging/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.741526 pyipv8-2.8.0/ipv8/test/messaging/interfaces/dispatcher/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/messaging/interfaces/dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9239 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/messaging/interfaces/dispatcher/test_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     3344 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/messaging/interfaces/test_network_stats.py
--rw-r--r--   0 runner    (1001) docker     (121)     9252 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/messaging/interfaces/test_statistics_endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.741526 pyipv8-2.8.0/ipv8/test/messaging/interfaces/udp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/messaging/interfaces/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2828 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/messaging/interfaces/udp/test_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)    13914 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/messaging/test_lazy_payload.py
--rw-r--r--   0 runner    (1001) docker     (121)    10282 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/messaging/test_payload_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (121)     6572 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/messaging/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.741526 pyipv8-2.8.0/ipv8/test/mocking/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/mocking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      838 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/mocking/community.py
--rw-r--r--   0 runner    (1001) docker     (121)      224 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/mocking/discovery.py
--rw-r--r--   0 runner    (1001) docker     (121)     4568 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/mocking/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     1152 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/mocking/exit_socket.py
--rw-r--r--   0 runner    (1001) docker     (121)     2818 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/mocking/ipv8.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.741526 pyipv8-2.8.0/ipv8/test/peerdiscovery/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/peerdiscovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4033 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/peerdiscovery/test_churn.py
--rw-r--r--   0 runner    (1001) docker     (121)     4340 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/peerdiscovery/test_community.py
--rw-r--r--   0 runner    (1001) docker     (121)     5881 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/peerdiscovery/test_edge_discovery.py
--rw-r--r--   0 runner    (1001) docker     (121)    21443 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/peerdiscovery/test_network.py
--rw-r--r--   0 runner    (1001) docker     (121)     4667 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/peerdiscovery/test_random_discovery.py
--rw-r--r--   0 runner    (1001) docker     (121)     2695 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/test_community_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)    13577 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     1046 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/test_database.py
--rw-r--r--   0 runner    (1001) docker     (121)    13684 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     6832 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/test_peer.py
--rw-r--r--   0 runner    (1001) docker     (121)     7055 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/test_requestcache.py
--rw-r--r--   0 runner    (1001) docker     (121)     5927 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/test_taskmanager.py
--rw-r--r--   0 runner    (1001) docker     (121)      875 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/test/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     2375 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/types.py
--rw-r--r--   0 runner    (1001) docker     (121)      822 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8/util.py
--rw-r--r--   0 runner    (1001) docker     (121)    11421 2021-10-27 07:17:39.000000 pyipv8-2.8.0/ipv8_service.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.741526 pyipv8-2.8.0/pyipv8.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5290 2021-10-27 07:17:53.000000 pyipv8-2.8.0/pyipv8.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8759 2021-10-27 07:17:53.000000 pyipv8-2.8.0/pyipv8.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-27 07:17:53.000000 pyipv8-2.8.0/pyipv8.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      141 2021-10-27 07:17:53.000000 pyipv8-2.8.0/pyipv8.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2021-10-27 07:17:53.000000 pyipv8-2.8.0/pyipv8.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-27 07:17:53.745526 pyipv8-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2021-10-27 07:17:39.000000 pyipv8-2.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.745526 pyipv8-2.8.0/simulation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2620 2021-10-27 07:17:39.000000 pyipv8-2.8.0/simulation/discrete_loop.py
--rw-r--r--   0 runner    (1001) docker     (121)      913 2021-10-27 07:17:39.000000 pyipv8-2.8.0/simulation/simulation_endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:53.745526 pyipv8-2.8.0/stresstest/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-27 07:17:39.000000 pyipv8-2.8.0/stresstest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       97 2021-10-27 07:17:39.000000 pyipv8-2.8.0/stresstest/__scriptpath__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4141 2021-10-27 07:17:39.000000 pyipv8-2.8.0/stresstest/bootstrap_introductions.py
--rw-r--r--   0 runner    (1001) docker     (121)      705 2021-10-27 07:17:39.000000 pyipv8-2.8.0/stresstest/bootstrap_introductions.r
--rw-r--r--   0 runner    (1001) docker     (121)     4639 2021-10-27 07:17:39.000000 pyipv8-2.8.0/stresstest/bootstrap_rtt.py
--rw-r--r--   0 runner    (1001) docker     (121)     2898 2021-10-27 07:17:39.000000 pyipv8-2.8.0/stresstest/peer_discovery.py
--rw-r--r--   0 runner    (1001) docker     (121)     2864 2021-10-27 07:17:39.000000 pyipv8-2.8.0/stresstest/peer_discovery_defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.221223 pyipv8-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     7651 2022-06-24 09:51:09.000000 pyipv8-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     5290 2022-06-24 09:51:20.221223 pyipv8-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4362 2022-06-24 09:51:09.000000 pyipv8-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.193216 pyipv8-2.9.0/ipv8/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.197217 pyipv8-2.9.0/ipv8/REST/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/REST/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8650 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/REST/asyncio_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16281 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/REST/attestation_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1300 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/REST/base_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12234 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/REST/dht_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23146 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/REST/identity_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2900 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/REST/isolation_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1472 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/REST/network_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2081 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/REST/noblock_dht_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7069 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/REST/overlays_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4334 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/REST/rest_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1285 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/REST/root_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2817 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/REST/schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15377 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/REST/tunnel_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.197217 pyipv8-2.9.0/ipv8/attestation/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14330 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/communication_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2221 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/default_identity_formats.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.197217 pyipv8-2.9.0/ipv8/attestation/identity/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2207 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/identity/attestation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16321 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/identity/community.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8367 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/identity/database.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10851 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/identity/manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3465 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/identity/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)      779 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/identity/payload.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6039 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/identity_formats.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.197217 pyipv8-2.9.0/ipv8/attestation/schema/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3924 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/schema/manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3114 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/signed_object.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.197217 pyipv8-2.9.0/ipv8/attestation/tokentree/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/tokentree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4884 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/tokentree/token.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8739 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/tokentree/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.197217 pyipv8-2.9.0/ipv8/attestation/wallet/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.197217 pyipv8-2.9.0/ipv8/attestation/wallet/bonehexact/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/bonehexact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6672 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/bonehexact/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4826 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/bonehexact/attestation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2129 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/bonehexact/structs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3662 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/caches.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23020 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/community.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4110 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/database.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.197217 pyipv8-2.9.0/ipv8/attestation/wallet/irmaexact/
+-rw-r--r--   0 runner    (1001) docker     (121)      360 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/irmaexact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4853 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/irmaexact/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7560 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/irmaexact/enroll_script.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.201218 pyipv8-2.9.0/ipv8/attestation/wallet/irmaexact/gabi/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/irmaexact/gabi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4832 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/irmaexact/gabi/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7439 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/irmaexact/gabi/builder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5114 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/irmaexact/gabi/credential.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7009 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/irmaexact/gabi/keys.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5428 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/irmaexact/gabi/proofs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27620 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/irmaexact/keydump.py
+-rw-r--r--   0 runner    (1001) docker     (121)      755 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/irmaexact/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2694 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/payload.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.201218 pyipv8-2.9.0/ipv8/attestation/wallet/pengbaorange/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/pengbaorange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6871 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/pengbaorange/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/pengbaorange/attestation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4606 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/pengbaorange/boudot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9445 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/pengbaorange/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.201218 pyipv8-2.9.0/ipv8/attestation/wallet/primitives/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      909 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/primitives/attestation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3617 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/primitives/boneh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2334 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/primitives/cryptography_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2209 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/primitives/ec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2575 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/primitives/structs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8075 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/attestation/wallet/primitives/value.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.201218 pyipv8-2.9.0/ipv8/bootstrapping/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/bootstrapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2127 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/bootstrapping/bootstrapper_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.201218 pyipv8-2.9.0/ipv8/bootstrapping/dispersy/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/bootstrapping/dispersy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3028 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/bootstrapping/dispersy/bootstrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.201218 pyipv8-2.9.0/ipv8/bootstrapping/udpbroadcast/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/bootstrapping/udpbroadcast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4115 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/bootstrapping/udpbroadcast/bootstrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24450 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/community.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16742 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15631 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/database.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.201218 pyipv8-2.9.0/ipv8/dht/
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/dht/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1925 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/dht/churn.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22886 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/dht/community.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8373 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/dht/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2437 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/dht/payload.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3011 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/dht/provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7978 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/dht/routing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2116 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/dht/storage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3443 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/dht/trie.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.201218 pyipv8-2.9.0/ipv8/keyvault/
+-rw-r--r--   0 runner    (1001) docker     (121)      883 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/keyvault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4840 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/keyvault/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/keyvault/keys.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.205219 pyipv8-2.9.0/ipv8/keyvault/private/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/keyvault/private/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1611 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/keyvault/private/libnaclkey.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3618 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/keyvault/private/m2crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.205219 pyipv8-2.9.0/ipv8/keyvault/public/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/keyvault/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1729 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/keyvault/public/libnaclkey.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3180 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/keyvault/public/m2crypto.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11240 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/lazy_community.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17303 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.205219 pyipv8-2.9.0/ipv8/messaging/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/messaging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.205219 pyipv8-2.9.0/ipv8/messaging/anonymization/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/messaging/anonymization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5502 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/messaging/anonymization/caches.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46019 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/messaging/anonymization/community.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2426 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/messaging/anonymization/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27957 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/messaging/anonymization/hidden_services.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8657 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/messaging/anonymization/payload.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3611 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/messaging/anonymization/pex.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17267 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/messaging/anonymization/tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2692 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/messaging/anonymization/tunnelcrypto.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/messaging/anonymization/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.205219 pyipv8-2.9.0/ipv8/messaging/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/messaging/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.205219 pyipv8-2.9.0/ipv8/messaging/interfaces/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/messaging/interfaces/dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5592 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/messaging/interfaces/dispatcher/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13869 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/messaging/interfaces/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1979 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/messaging/interfaces/network_stats.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6437 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/messaging/interfaces/statistics_endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.205219 pyipv8-2.9.0/ipv8/messaging/interfaces/udp/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/messaging/interfaces/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4442 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/messaging/interfaces/udp/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8675 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/messaging/lazy_payload.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12078 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/messaging/payload.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2886 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/messaging/payload_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (121)      870 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/messaging/payload_headers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16532 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/messaging/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3930 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6196 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/peer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.209220 pyipv8-2.9.0/ipv8/peerdiscovery/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/peerdiscovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2618 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/peerdiscovery/churn.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7906 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/peerdiscovery/community.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6977 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/peerdiscovery/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14860 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/peerdiscovery/network.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4856 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/peerdiscovery/payload.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10844 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/requestcache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7874 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/taskmanager.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.209220 pyipv8-2.9.0/ipv8/test/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.209220 pyipv8-2.9.0/ipv8/test/REST/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/REST/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5518 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/REST/rest_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19898 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/REST/test_attestation_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18919 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/REST/test_identity_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4085 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/REST/test_isolation_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5042 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/REST/test_network_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13042 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/REST/test_overlays_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.209220 pyipv8-2.9.0/ipv8/test/attestation/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.213221 pyipv8-2.9.0/ipv8/test/attestation/identity/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7902 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/identity/test_identity.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7671 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/identity/test_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.213221 pyipv8-2.9.0/ipv8/test/attestation/tokentree/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/tokentree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3883 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/tokentree/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8718 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/tokentree/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.213221 pyipv8-2.9.0/ipv8/test/attestation/wallet/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1617 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/wallet/attestation.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    12341 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/wallet/attestation_big.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3388 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/wallet/attestation_range.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.213221 pyipv8-2.9.0/ipv8/test/attestation/wallet/bonehexact/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/wallet/bonehexact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4221 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/wallet/bonehexact/test_attestation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9738 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/wallet/bonehexact/test_structs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.213221 pyipv8-2.9.0/ipv8/test/attestation/wallet/irmaexact/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/wallet/irmaexact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5618 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/wallet/irmaexact/test_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6449 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/wallet/irmaexact/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22325 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/wallet/irmaexact/test_credential.py
+-rw-r--r--   0 runner    (1001) docker     (121)      874 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/wallet/irmaexact/test_keys.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8940 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/wallet/irmaexact/test_proofs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.213221 pyipv8-2.9.0/ipv8/test/attestation/wallet/pengbaorange/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/wallet/pengbaorange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6135 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/wallet/pengbaorange/test_boudot.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.213221 pyipv8-2.9.0/ipv8/test/attestation/wallet/primitives/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/wallet/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5128 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/wallet/primitives/test_boneh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1966 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/wallet/primitives/test_ec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8344 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/wallet/primitives/test_value.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12823 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/attestation/wallet/test_attestation_community.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9983 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.213221 pyipv8-2.9.0/ipv8/test/bootstrapping/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/bootstrapping/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.217222 pyipv8-2.9.0/ipv8/test/bootstrapping/dispersy/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/bootstrapping/dispersy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3323 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/bootstrapping/dispersy/test_bootstrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.217222 pyipv8-2.9.0/ipv8/test/dht/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/dht/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      356 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/dht/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/dht/test_churn.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10050 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/dht/test_community.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4129 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/dht/test_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2925 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/dht/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7130 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/dht/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/dht/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2760 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/dht/test_trie.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.217222 pyipv8-2.9.0/ipv8/test/keyvault/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/keyvault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5721 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/keyvault/test_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2596 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/keyvault/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2371 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/keyvault/test_signature.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.217222 pyipv8-2.9.0/ipv8/test/messaging/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/messaging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.217222 pyipv8-2.9.0/ipv8/test/messaging/anonymization/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/messaging/anonymization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      619 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/messaging/anonymization/mock.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22426 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/messaging/anonymization/test_community.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2891 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/messaging/anonymization/test_datachecker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2047 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/messaging/anonymization/test_exit_socket.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13788 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/messaging/anonymization/test_hiddenservices.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.217222 pyipv8-2.9.0/ipv8/test/messaging/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/messaging/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.217222 pyipv8-2.9.0/ipv8/test/messaging/interfaces/dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/messaging/interfaces/dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9239 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/messaging/interfaces/dispatcher/test_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1315 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/messaging/interfaces/test_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3344 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/messaging/interfaces/test_network_stats.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9252 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/messaging/interfaces/test_statistics_endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.217222 pyipv8-2.9.0/ipv8/test/messaging/interfaces/udp/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/messaging/interfaces/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2828 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/messaging/interfaces/udp/test_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13914 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/messaging/test_lazy_payload.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10282 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/messaging/test_payload_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6572 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/messaging/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.221223 pyipv8-2.9.0/ipv8/test/mocking/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/mocking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      838 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/mocking/community.py
+-rw-r--r--   0 runner    (1001) docker     (121)      224 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/mocking/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4568 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/mocking/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1152 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/mocking/exit_socket.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2818 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/mocking/ipv8.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.221223 pyipv8-2.9.0/ipv8/test/peerdiscovery/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/peerdiscovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4033 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/peerdiscovery/test_churn.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4340 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/peerdiscovery/test_community.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5881 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/peerdiscovery/test_edge_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21443 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/peerdiscovery/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4667 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/peerdiscovery/test_random_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5438 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/test_community.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14348 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1046 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13713 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6832 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/test_peer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7516 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/test_requestcache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5927 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/test_taskmanager.py
+-rw-r--r--   0 runner    (1001) docker     (121)      875 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/test/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2375 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)      822 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11421 2022-06-24 09:51:09.000000 pyipv8-2.9.0/ipv8_service.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.221223 pyipv8-2.9.0/pyipv8.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5290 2022-06-24 09:51:20.000000 pyipv8-2.9.0/pyipv8.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     8800 2022-06-24 09:51:20.000000 pyipv8-2.9.0/pyipv8.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-24 09:51:20.000000 pyipv8-2.9.0/pyipv8.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2022-06-24 09:51:20.000000 pyipv8-2.9.0/pyipv8.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-06-24 09:51:20.000000 pyipv8-2.9.0/pyipv8.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-24 09:51:20.221223 pyipv8-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1501 2022-06-24 09:51:09.000000 pyipv8-2.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.221223 pyipv8-2.9.0/simulation/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2620 2022-06-24 09:51:09.000000 pyipv8-2.9.0/simulation/discrete_loop.py
+-rw-r--r--   0 runner    (1001) docker     (121)      913 2022-06-24 09:51:09.000000 pyipv8-2.9.0/simulation/simulation_endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:20.221223 pyipv8-2.9.0/stresstest/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-24 09:51:09.000000 pyipv8-2.9.0/stresstest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       97 2022-06-24 09:51:09.000000 pyipv8-2.9.0/stresstest/__scriptpath__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4141 2022-06-24 09:51:09.000000 pyipv8-2.9.0/stresstest/bootstrap_introductions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      705 2022-06-24 09:51:09.000000 pyipv8-2.9.0/stresstest/bootstrap_introductions.r
+-rw-r--r--   0 runner    (1001) docker     (121)     4639 2022-06-24 09:51:09.000000 pyipv8-2.9.0/stresstest/bootstrap_rtt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2898 2022-06-24 09:51:09.000000 pyipv8-2.9.0/stresstest/peer_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2864 2022-06-24 09:51:09.000000 pyipv8-2.9.0/stresstest/peer_discovery_defaults.py
```

### Comparing `pyipv8-2.8.0/LICENSE` & `pyipv8-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/PKG-INFO` & `pyipv8-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyipv8
-Version: 2.8.0
+Version: 2.9.0
 Summary: The Python implementation of the IPV8 library
 Home-page: https://github.com/Tribler/py-ipv8
 Author: Tribler
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pyipv8-2.8.0/README.md` & `pyipv8-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/REST/asyncio_endpoint.py` & `pyipv8-2.9.0/ipv8/REST/asyncio_endpoint.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/REST/attestation_endpoint.py` & `pyipv8-2.9.0/ipv8/REST/attestation_endpoint.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/REST/base_endpoint.py` & `pyipv8-2.9.0/ipv8/REST/base_endpoint.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/REST/dht_endpoint.py` & `pyipv8-2.9.0/ipv8/REST/dht_endpoint.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/REST/identity_endpoint.py` & `pyipv8-2.9.0/ipv8/REST/identity_endpoint.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/REST/isolation_endpoint.py` & `pyipv8-2.9.0/ipv8/REST/isolation_endpoint.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/REST/network_endpoint.py` & `pyipv8-2.9.0/ipv8/REST/network_endpoint.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/REST/noblock_dht_endpoint.py` & `pyipv8-2.9.0/ipv8/REST/noblock_dht_endpoint.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/REST/overlays_endpoint.py` & `pyipv8-2.9.0/ipv8/REST/overlays_endpoint.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/REST/rest_manager.py` & `pyipv8-2.9.0/ipv8/REST/rest_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
                                                                     error_middleware])
         self.root_endpoint.initialize(self.session)
 
         # Not using setup_aiohttp_apispec here, as we need access to the APISpec to set the security scheme
         aiohttp_apispec = AiohttpApiSpec(
             app=self.root_endpoint.app,
             title="IPv8 REST API documentation",
-            version="v2.8",  # Do not change manually! Handled by github_increment_version.py
+            version="v2.9",  # Do not change manually! Handled by github_increment_version.py
             url="/docs/swagger.json",
             swagger_path="/docs",
         )
         if api_key:
             # Set security scheme and apply to all endpoints
             aiohttp_apispec.spec.options['security'] = [{'apiKey': []}]
             aiohttp_apispec.spec.components.security_scheme('apiKey', {'type': 'apiKey',
```

### Comparing `pyipv8-2.8.0/ipv8/REST/root_endpoint.py` & `pyipv8-2.9.0/ipv8/REST/root_endpoint.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/REST/schema.py` & `pyipv8-2.9.0/ipv8/REST/schema.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/REST/tunnel_endpoint.py` & `pyipv8-2.9.0/ipv8/REST/tunnel_endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
             'description': 'The circuit_id of the circuit which is to be tested.',
             'type': 'integer',
         }],
         responses={
             200: {"schema": SpeedTestResponseSchema}
         }
     )
-    @json_schema(schema(SpeedTestRequest={
+    @json_schema(schema(SpeedTestExistingCircuitRequest={
         'request_size*': (Integer, 'Size of the requests to send (0..1500)'),
         'response_size*': (Integer, 'Size of the responses to send (0..1500)'),
         'num_packets*': (Integer, 'Number of packets to send'),
     }))
     async def speed_test_existing_circuit(self, request):
         if not request.match_info['circuit_id'].isdigit():
             return Response({"error": "circuit_id must be an integer"}, status=HTTP_BAD_REQUEST)
@@ -146,15 +146,15 @@
             'enum': ['upload', 'download'],
             'default': 'download'
         }],
         responses={
             200: {"schema": SpeedTestResponseSchema}
         }
     )
-    @json_schema(schema(SpeedTestRequest={
+    @json_schema(schema(SpeedTestNewCircuitRequest={
         'goals_hops': (Integer, 'Number of hops that the newly created circuit should have'),
         'request_size*': (Integer, 'Size of the requests to send (0..1500)'),
         'response_size*': (Integer, 'Size of the responses to send (0..1500)'),
         'num_packets*': (Integer, 'Number of packets to send'),
     }))
     async def speed_test_new_circuit(self, request):
         params = await request.json()
```

### Comparing `pyipv8-2.8.0/ipv8/attestation/communication_manager.py` & `pyipv8-2.9.0/ipv8/attestation/communication_manager.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/default_identity_formats.py` & `pyipv8-2.9.0/ipv8/attestation/default_identity_formats.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/identity/attestation.py` & `pyipv8-2.9.0/ipv8/attestation/identity/attestation.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/identity/community.py` & `pyipv8-2.9.0/ipv8/attestation/identity/community.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/identity/database.py` & `pyipv8-2.9.0/ipv8/attestation/identity/database.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/identity/manager.py` & `pyipv8-2.9.0/ipv8/attestation/identity/manager.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/identity/metadata.py` & `pyipv8-2.9.0/ipv8/attestation/identity/metadata.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/identity/payload.py` & `pyipv8-2.9.0/ipv8/attestation/identity/payload.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/identity_formats.py` & `pyipv8-2.9.0/ipv8/attestation/identity_formats.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/schema/manager.py` & `pyipv8-2.9.0/ipv8/attestation/schema/manager.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/signed_object.py` & `pyipv8-2.9.0/ipv8/attestation/signed_object.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/tokentree/token.py` & `pyipv8-2.9.0/ipv8/attestation/tokentree/token.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/tokentree/tree.py` & `pyipv8-2.9.0/ipv8/attestation/tokentree/tree.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/wallet/bonehexact/algorithm.py` & `pyipv8-2.9.0/ipv8/attestation/wallet/bonehexact/algorithm.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/wallet/bonehexact/attestation.py` & `pyipv8-2.9.0/ipv8/attestation/wallet/bonehexact/attestation.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/wallet/bonehexact/structs.py` & `pyipv8-2.9.0/ipv8/attestation/wallet/bonehexact/structs.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/wallet/caches.py` & `pyipv8-2.9.0/ipv8/attestation/wallet/caches.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/wallet/community.py` & `pyipv8-2.9.0/ipv8/attestation/wallet/community.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/wallet/database.py` & `pyipv8-2.9.0/ipv8/attestation/wallet/database.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/wallet/irmaexact/algorithm.py` & `pyipv8-2.9.0/ipv8/attestation/wallet/irmaexact/algorithm.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/wallet/irmaexact/enroll_script.py` & `pyipv8-2.9.0/ipv8/attestation/wallet/irmaexact/enroll_script.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/wallet/irmaexact/gabi/attributes.py` & `pyipv8-2.9.0/ipv8/attestation/wallet/irmaexact/gabi/attributes.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/wallet/irmaexact/gabi/builder.py` & `pyipv8-2.9.0/ipv8/attestation/wallet/irmaexact/gabi/builder.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/wallet/irmaexact/gabi/credential.py` & `pyipv8-2.9.0/ipv8/attestation/wallet/irmaexact/gabi/credential.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/wallet/irmaexact/gabi/keys.py` & `pyipv8-2.9.0/ipv8/attestation/wallet/irmaexact/gabi/keys.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/wallet/irmaexact/gabi/proofs.py` & `pyipv8-2.9.0/ipv8/attestation/wallet/irmaexact/gabi/proofs.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/wallet/irmaexact/keydump.py` & `pyipv8-2.9.0/ipv8/attestation/wallet/irmaexact/keydump.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/wallet/irmaexact/wrappers.py` & `pyipv8-2.9.0/ipv8/attestation/wallet/irmaexact/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/wallet/payload.py` & `pyipv8-2.9.0/ipv8/attestation/wallet/payload.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/wallet/pengbaorange/algorithm.py` & `pyipv8-2.9.0/ipv8/attestation/wallet/pengbaorange/algorithm.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/wallet/pengbaorange/attestation.py` & `pyipv8-2.9.0/ipv8/attestation/wallet/pengbaorange/attestation.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/wallet/pengbaorange/boudot.py` & `pyipv8-2.9.0/ipv8/attestation/wallet/pengbaorange/boudot.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/wallet/pengbaorange/structs.py` & `pyipv8-2.9.0/ipv8/attestation/wallet/pengbaorange/structs.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/wallet/primitives/attestation.py` & `pyipv8-2.9.0/ipv8/attestation/wallet/primitives/attestation.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/wallet/primitives/boneh.py` & `pyipv8-2.9.0/ipv8/attestation/wallet/primitives/boneh.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/wallet/primitives/cryptography_wrapper.py` & `pyipv8-2.9.0/ipv8/attestation/wallet/primitives/cryptography_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/wallet/primitives/ec.py` & `pyipv8-2.9.0/ipv8/attestation/wallet/primitives/ec.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/wallet/primitives/structs.py` & `pyipv8-2.9.0/ipv8/attestation/wallet/primitives/structs.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/attestation/wallet/primitives/value.py` & `pyipv8-2.9.0/ipv8/attestation/wallet/primitives/value.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/bootstrapping/bootstrapper_interface.py` & `pyipv8-2.9.0/ipv8/bootstrapping/bootstrapper_interface.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/bootstrapping/dispersy/bootstrapper.py` & `pyipv8-2.9.0/ipv8/bootstrapping/dispersy/bootstrapper.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 from ..bootstrapper_interface import Bootstrapper
 from ...community import Community
 from ...messaging.interfaces.udp.endpoint import UDPv4Address
 from ...types import Address
 from ...util import succeed
 
+# Workaround for unnecessarily failing gethostbyname from a worker thread (https://bugs.python.org/issue29288)
+u''.encode('idna')
+
 
 class DispersyBootstrapper(Bootstrapper):
 
     def __init__(self, ip_addresses, dns_addresses, bootstrap_timeout=30.0):
         self.ip_addresses = [UDPv4Address(*addr) for addr in ip_addresses]
         self.dns_addresses = dns_addresses
```

### Comparing `pyipv8-2.8.0/ipv8/bootstrapping/udpbroadcast/bootstrapper.py` & `pyipv8-2.9.0/ipv8/bootstrapping/udpbroadcast/bootstrapper.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 from asyncio import BaseTransport, DatagramProtocol, get_event_loop
 from asyncio.futures import Future
 from binascii import hexlify
 from socket import AF_INET, SOCK_DGRAM, SOL_SOCKET, SO_BROADCAST, SO_REUSEADDR, socket
+from time import time
 from typing import Coroutine, Iterable, Optional, Union
 
 from ..bootstrapper_interface import Bootstrapper
 from ...types import Address, Community
 from ...util import succeed
 
 
@@ -62,18 +63,22 @@
     def close(self) -> None:
         if self._transport is not None and not self._transport.is_closing():
             self._transport.close()
 
 
 class UDPBroadcastBootstrapper(Bootstrapper):
 
-    def __init__(self):
+    def __init__(self, bootstrap_timeout=30.0):
         self.endpoint = None
         self.overlay = None
 
+        self.bootstrap_timeout = bootstrap_timeout
+
+        self.last_bootstrap = 0
+
     async def initialize(self, overlay: Community) -> Union[Future, Coroutine]:  # pylint: disable=W0236
         self.overlay = overlay
 
         # Open the socket
         endpoint = BroadcastBootstrapEndpoint(overlay)
         success = await endpoint.open()
         if not success:
@@ -90,14 +95,18 @@
         Try to find a listener (fire and forget).
         """
         if self.endpoint is not None:
             for p in range(65535):
                 self.endpoint.send(('255.255.255.255', p), HDR_ANNOUNCE + service_prefix)
 
     async def get_addresses(self, overlay: Community, timeout: float) -> Iterable[Address]:
+        if time() - self.last_bootstrap < self.bootstrap_timeout:
+            return []
+        logging.debug("Bootstrapping %s, current peers %d", overlay.__class__.__name__, len(overlay.get_peers()))
+        self.last_bootstrap = time()
         self.beacon(overlay.get_prefix())
         return []
 
     def keep_alive(self, overlay: Community) -> None:
         self.beacon(overlay.get_prefix())
 
     def blacklist(self) -> Iterable[Address]:
```

### Comparing `pyipv8-2.8.0/ipv8/community.py` & `pyipv8-2.9.0/ipv8/community.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import sys
 from asyncio import ensure_future, iscoroutine
 from binascii import hexlify
 from functools import partial
 from random import choice, random
 from time import time
 from traceback import format_exception
+from typing import Optional
 
 from .lazy_community import EZPackOverlay, lazy_wrapper, lazy_wrapper_unsigned
 from .messaging.anonymization.endpoint import TunnelEndpoint
 from .messaging.interfaces.dispatcher.endpoint import FAST_ADDR_TO_INTERFACE, INTERFACES
 from .messaging.interfaces.udp.endpoint import UDPv4Address, UDPv4LANAddress, UDPv6Address
 from .messaging.payload import (IntroductionRequestPayload, IntroductionResponsePayload,
                                 NewIntroductionRequestPayload, NewIntroductionResponsePayload,
@@ -31,19 +32,25 @@
 
 DEFAULT_MAX_PEERS = 30
 
 
 class Community(EZPackOverlay):
 
     version = b'\x02'
-    community_id = b''
+    community_id: Optional[bytes] = None
 
     def __init__(self, my_peer, endpoint, network, max_peers=DEFAULT_MAX_PEERS, anonymize=False):
         super().__init__(self.community_id, my_peer, endpoint, network)
 
+        if self.community_id is None:
+            raise RuntimeError(f"Attempted to launch {self.__class__.__name__} without a community_id!")
+        if not isinstance(self.community_id, bytes):
+            raise RuntimeError(f"Attempted to launch {self.__class__.__name__} with a community_id that is not bytes!"
+                               f"\n{repr(self.community_id)}")
+
         self._prefix = b'\x00' + self.version + self.community_id
         self.endpoint.remove_listener(self)
         self.endpoint.add_prefix_listener(self, self._prefix)
         self.logger.debug("Launching %s with prefix %s.", self.__class__.__name__, hexlify(self._prefix).decode())
 
         self.max_peers = max_peers
         self.anonymize = anonymize
@@ -172,15 +179,15 @@
             self._initialize_bootstrappers()
         for bootstrapper in self.bootstrappers:
             task = self.register_anonymous_task(f"bootstrap {repr(bootstrapper)}", bootstrapper.get_addresses,
                                                 self, 60.0)
             task.add_done_callback(self.received_bootstrapped_addresses)
 
     def received_bootstrapped_addresses(self, addresses):
-        if addresses and addresses.result():
+        if addresses and not addresses.cancelled() and addresses.result():
             for address in list(addresses.result())[:self.max_peers]:
                 self.walk_to(address)
 
     def ensure_blacklisted(self, address):
         if address not in self.network.blacklist:
             self.network.blacklist.append(address)
```

### Comparing `pyipv8-2.8.0/ipv8/configuration.py` & `pyipv8-2.9.0/ipv8/configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
 
+import base64
 import copy
 import enum
 import typing
 from typing import Any, Dict
 
+from .keyvault.crypto import default_eccrypto
+
 DISPERSY_BOOTSTRAPPER: Dict[Any, Any] = {
     'class': "DispersyBootstrapper",
     'init': {
         'ip_addresses': [
             ("130.161.119.206", 6421),
             ("130.161.119.206", 6422),
             ("131.180.27.155", 6423),
@@ -335,15 +338,15 @@
         self.config['keys'].append({
             'alias': alias,
             'generation': generation,
             'file': file_path
         })
         return self
 
-    def add_key_from_bin(self, alias: str, key_bin_b64: str, file_path: typing.Optional[str] = None):
+    def add_key_from_bin(self, alias: str, key_bin_b64: str, file_path: typing.Optional[str] = None) -> ConfigBuilder:
         """
         Add a key by alias and  its raw key material, possibly stored at a certain file path.
 
         If a key already exists at the given file path, that will be loaded instead of the given key material.
 
         :param alias: the alias used to reference this key
         :param key_bin_b64: the base64 encoded private key material
@@ -358,14 +361,23 @@
             'bin': key_bin_b64
         }
         if file_path is not None:
             key_config['file'] = file_path
         self.config['keys'].append(key_config)
         return self
 
+    def add_ephemeral_key(self, alias: str) -> ConfigBuilder:
+        """
+        Add an ephemeral key, which is only stored in memory (i.e., not associated with a file).
+
+        :param alias: the alias used to reference this key
+        """
+        eph_key = default_eccrypto.generate_key("curve25519").key_to_bin()
+        return self.add_key_from_bin(alias, base64.b64encode(eph_key).decode(), "")
+
     def add_overlay(self,
                     overlay_class: str,
                     key_alias: str,
                     walkers: typing.List[WalkerDefinition],
                     bootstrappers: typing.List[BootstrapperDefinition],
                     initialize: typing.Dict[str, typing.Any],
                     on_start: typing.List[tuple],
```

### Comparing `pyipv8-2.8.0/ipv8/database.py` & `pyipv8-2.9.0/ipv8/database.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/dht/churn.py` & `pyipv8-2.9.0/ipv8/dht/churn.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/dht/community.py` & `pyipv8-2.9.0/ipv8/dht/community.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/dht/discovery.py` & `pyipv8-2.9.0/ipv8/dht/discovery.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/dht/payload.py` & `pyipv8-2.9.0/ipv8/dht/payload.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/dht/provider.py` & `pyipv8-2.9.0/ipv8/dht/provider.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/dht/routing.py` & `pyipv8-2.9.0/ipv8/dht/routing.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/dht/storage.py` & `pyipv8-2.9.0/ipv8/dht/storage.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/dht/trie.py` & `pyipv8-2.9.0/ipv8/dht/trie.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/keyvault/__init__.py` & `pyipv8-2.9.0/ipv8/keyvault/__init__.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/keyvault/crypto.py` & `pyipv8-2.9.0/ipv8/keyvault/crypto.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/keyvault/keys.py` & `pyipv8-2.9.0/ipv8/keyvault/keys.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/keyvault/private/libnaclkey.py` & `pyipv8-2.9.0/ipv8/keyvault/private/libnaclkey.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/keyvault/private/m2crypto.py` & `pyipv8-2.9.0/ipv8/keyvault/private/m2crypto.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/keyvault/public/libnaclkey.py` & `pyipv8-2.9.0/ipv8/keyvault/public/libnaclkey.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/keyvault/public/m2crypto.py` & `pyipv8-2.9.0/ipv8/keyvault/public/m2crypto.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/lazy_community.py` & `pyipv8-2.9.0/ipv8/lazy_community.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/loader.py` & `pyipv8-2.9.0/ipv8/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -329,15 +329,15 @@
 class CommunityLauncher:
 
     """
     Object in charge of preparing a Community for loading in IPv8.
     """
 
     def __init__(self):
-        super()
+        super().__init__()
         self.community_args = []
         self.community_kwargs = {}
 
     def get_name(self):
         """
         Get the launcher name, for pre-launch organisation.
```

### Comparing `pyipv8-2.8.0/ipv8/messaging/anonymization/caches.py` & `pyipv8-2.9.0/ipv8/messaging/anonymization/caches.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import logging
+import os
 import time
 from asyncio import Future
+from functools import reduce
 
 from .tunnel import CIRCUIT_STATE_CLOSING, CIRCUIT_STATE_READY
 from ...requestcache import NumberCache, RandomNumberCache
 
 
 class CreateRequestCache(RandomNumberCache):
     """
@@ -37,22 +39,23 @@
         self.timeout = timeout
 
     @property
     def timeout_delay(self):
         return float(self.timeout)
 
 
-class RetryRequestCache(RandomNumberCache):
+class RetryRequestCache(NumberCache):
     """
     Used to track adding additional hops to the circuit.
     """
     def __init__(self, community, circuit, candidates, max_tries, retry_func, timeout):
-        super().__init__(community.request_cache, "retry")
+        super().__init__(community.request_cache, "retry", circuit.circuit_id)
         self.community = community
         self.circuit = circuit
+        self.packet_identifier = reduce(lambda v, e: (v << 8) + e, os.urandom(2), 0)
         self.candidates = candidates
         self.max_tries = max_tries
         self.retry_func = retry_func
         self.timeout = timeout
         self.logger = logging.getLogger(__name__)
 
     @property
```

### Comparing `pyipv8-2.8.0/ipv8/messaging/anonymization/community.py` & `pyipv8-2.9.0/ipv8/messaging/anonymization/community.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,29 +299,40 @@
         alt_first_hops = [c for c in candidate_list if c != first_hop]
 
         circuit.unverified_hop = Hop(first_hop, flags=self.candidates.get(first_hop))
         circuit.unverified_hop.dh_secret, circuit.unverified_hop.dh_first_part = self.crypto.generate_diffie_secret()
 
         self.logger.info("Adding first hop %s:%d to circuit %d", *(first_hop.address + (circuit.circuit_id,)))
 
+        try:
+            self.request_cache.pop("retry", circuit.circuit_id)
+        except KeyError:
+            self.logger.info("Overwriting existing retry attempt for initial creation of circuit %d",
+                             circuit.circuit_id)
+
         cache = RetryRequestCache(self, circuit, alt_first_hops, max_tries - 1,
                                   self.send_initial_create, self.settings.next_hop_timeout)
         self.request_cache.add(cache)
 
         self.send_cell(first_hop, CreatePayload(circuit.circuit_id,
-                                                cache.number,
+                                                cache.packet_identifier,
                                                 self.my_peer.public_key.key_to_bin(),
                                                 circuit.unverified_hop.dh_first_part))
 
     @task
     async def remove_circuit(self, circuit_id, additional_info='', remove_now=False, destroy=False):
         """
         Remove a circuit and return a deferred that fires when all data associated with the circuit is destroyed.
         Optionally send a destroy message.
         """
+        try:
+            self.request_cache.pop("retry", circuit_id)
+        except KeyError:
+            pass  # All is good if there was no pending retry cache for this circuit: continue.
+
         circuit_to_remove = self.circuits.get(circuit_id, None)
         if circuit_to_remove is None:
             self.logger.warning('Cannot remove unknown circuit %d', circuit_id)
             return
 
         self.logger.info("Removing %s circuit %d %s", circuit_to_remove.ctype, circuit_id, additional_info)
 
@@ -510,19 +521,19 @@
         if circuit.state == CIRCUIT_STATE_EXTENDING:
             candidate_list_enc = payload.candidate_list_enc
             candidate_list_bin = self.crypto.decrypt_str(candidate_list_enc,
                                                          hop.session_keys[EXIT_NODE],
                                                          hop.session_keys[EXIT_NODE_SALT])
             candidate_list, _ = self.serializer.unpack('varlenH-list', candidate_list_bin)
 
-            cache = self.request_cache.pop("retry", payload.identifier)
+            cache = self.request_cache.pop("retry", circuit.circuit_id)
             self.send_extend(circuit, candidate_list, cache.max_tries if cache else 1)
 
         elif circuit.state == CIRCUIT_STATE_READY:
-            self.request_cache.pop("retry", payload.identifier)
+            self.request_cache.pop("retry", circuit.circuit_id)
 
     def send_extend(self, circuit, candidate_list, max_tries):
         ignore_candidates = [hop.node_public_key for hop in circuit.hops] + [self.my_peer.public_key.key_to_bin()]
         if circuit.required_exit:
             ignore_candidates.append(circuit.required_exit.public_key.key_to_bin())
 
         become_exit = circuit.goal_hops - 1 == len(circuit.hops)
@@ -556,20 +567,25 @@
 
             # Only retry if we are allowed to use another node
             if not become_exit or not circuit.required_exit:
                 alt_candidates = [c for c in candidate_list if c != extend_hop_public_bin]
             else:
                 alt_candidates = []
 
+            try:
+                self.request_cache.pop("retry", circuit.circuit_id)
+            except KeyError:
+                self.logger.info("Overwriting existing retry attempt for circuit %d", circuit.circuit_id)
+
             cache = RetryRequestCache(self, circuit, alt_candidates, max_tries - 1,
                                       self.send_extend, self.settings.next_hop_timeout)
             self.request_cache.add(cache)
 
             self.send_cell(circuit.peer, ExtendPayload(circuit.circuit_id,
-                                                       cache.number,
+                                                       cache.packet_identifier,
                                                        circuit.unverified_hop.node_public_key,
                                                        circuit.unverified_hop.dh_first_part,
                                                        extend_hop_addr))
 
         else:
             self.remove_circuit(circuit.circuit_id, "no candidates to extend")
 
@@ -719,15 +735,15 @@
 
             self.directions[request.from_circuit_id] = EXIT_NODE
             self.remove_exit_socket(request.from_circuit_id)
 
             self.send_cell(relay.peer,
                            ExtendedPayload(relay.circuit_id, request.extend_identifier,
                                            payload.key, payload.auth, payload.candidate_list_enc))
-        elif self.request_cache.has("retry", payload.identifier):
+        elif self.request_cache.has("retry", payload.circuit_id):
             circuit = self.circuits[circuit_id]
             self._ours_on_created_extended(circuit, payload)
         else:
             self.logger.warning("Received unexpected created for circuit %d", payload.circuit_id)
 
     @unpack_cell(ExtendPayload)
     async def on_extend(self, source_address, payload, _):
@@ -778,15 +794,15 @@
         self.request_cache.add(cache)
 
         self.send_cell(extend_candidate,
                        CreatePayload(to_circuit_id, cache.number, self.my_peer.public_key.key_to_bin(), payload.key))
 
     @unpack_cell(ExtendedPayload)
     def on_extended(self, source_address, payload, _):
-        if not self.request_cache.has("retry", payload.identifier):
+        if not self.request_cache.has("retry", payload.circuit_id):
             self.logger.warning("Received unexpected extended for circuit %s", payload.circuit_id)
             return
 
         circuit_id = payload.circuit_id
         circuit = self.circuits[circuit_id]
         self._ours_on_created_extended(circuit, payload)
```

### Comparing `pyipv8-2.8.0/ipv8/messaging/anonymization/endpoint.py` & `pyipv8-2.9.0/ipv8/messaging/anonymization/endpoint.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/messaging/anonymization/hidden_services.py` & `pyipv8-2.9.0/ipv8/messaging/anonymization/hidden_services.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/messaging/anonymization/payload.py` & `pyipv8-2.9.0/ipv8/messaging/anonymization/payload.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/messaging/anonymization/pex.py` & `pyipv8-2.9.0/ipv8/messaging/anonymization/pex.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/messaging/anonymization/tunnel.py` & `pyipv8-2.9.0/ipv8/messaging/anonymization/tunnel.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,22 +52,42 @@
 DESTROY_REASON_FORBIDDEN = 6
 
 
 class DataChecker(object):
 
     @staticmethod
     def could_be_utp(data):
+        """
+        Check if this data could be uTP (see also https://www.bittorrent.org/beps/bep_0029.html).
+
+        Packets should be 20 bytes or larger.
+
+        The type should be 0..4:
+         - 0: ST_DATA
+         - 1: ST_FIN
+         - 2: ST_STATE
+         - 3: ST_RESET
+         - 4: ST_SYN
+
+        The version should be 1.
+
+        The extension should be 0..3:
+         - 0: No extension
+         - 1: Selective ACK
+         - 2: Deprecated
+         - 3: Close reason
+        """
         if len(data) < 20:
             return False
         byte1, byte2 = unpack_from('!BB', data)
-        # Type should be 0..4, Ver should be 1
+        # Type and version
         if not (0 <= (byte1 >> 4) <= 4 and (byte1 & 15) == 1):
             return False
-        # Extension should be 0..2
-        if not (0 <= byte2 <= 2):
+        # Extension
+        if not (0 <= byte2 <= 3):
             return False
         return True
 
     @staticmethod
     def could_be_udp_tracker(data):
         # For the UDP tracker protocol the action field is either at position 0 or 8, and should be 0..3
         if len(data) >= 8 and (0 <= unpack_from('!I', data, 0)[0] <= 3)\
@@ -187,15 +207,15 @@
     def is_allowed(self, data):
         is_bt = DataChecker.could_be_bt(data)
         is_ipv8 = DataChecker.could_be_ipv8(data)
 
         if not (is_bt and PEER_FLAG_EXIT_BT in self.overlay.settings.peer_flags) \
            and not (is_ipv8 and PEER_FLAG_EXIT_IPV8 in self.overlay.settings.peer_flags) \
            and not (is_ipv8 and self.overlay._prefix == data[:22]):
-            self.logger.error("Dropping data packets, refusing to be an exit node (BT=%s, IPv8=%s)", is_bt, is_ipv8)
+            self.logger.warning("Dropping data packets, refusing to be an exit node (BT=%s, IPv8=%s)", is_bt, is_ipv8)
             return False
         return True
 
     def tunnel_data(self, source, data):
         self.logger.debug("Tunnel data to origin %s for circuit %s", ('0.0.0.0', 0), self.circuit_id)
         self.overlay.send_data(self.peer, self.circuit_id, ('0.0.0.0', 0), source, data)
```

### Comparing `pyipv8-2.8.0/ipv8/messaging/anonymization/tunnelcrypto.py` & `pyipv8-2.9.0/ipv8/messaging/anonymization/tunnelcrypto.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/messaging/anonymization/utils.py` & `pyipv8-2.9.0/ipv8/messaging/anonymization/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from asyncio import FIRST_COMPLETED, wait
 from statistics import mean, median
 from timeit import default_timer
 
-from ipv8.messaging.anonymization.tunnel import CIRCUIT_STATE_CLOSING
+from .tunnel import CIRCUIT_STATE_CLOSING
 
 
 async def run_speed_test(tc, circuit, request_size, response_size, num_requests, window=50):
     num_sent = 0
     num_ack = 0
     outstanding = set()
     start = default_timer()
```

### Comparing `pyipv8-2.8.0/ipv8/messaging/interfaces/dispatcher/endpoint.py` & `pyipv8-2.9.0/ipv8/messaging/interfaces/dispatcher/endpoint.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/messaging/interfaces/endpoint.py` & `pyipv8-2.9.0/ipv8/messaging/interfaces/endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,25 +210,21 @@
 
                 except ValueError:
                     # some interfaces are given that are invalid, we encountered one called ppp0
                     pass
 
                 else:
                     for option in addresses.get(netifaces.AF_INET, []):
-                        try:
-                            # On Windows netifaces currently returns IP addresses as unicode,
-                            # and on *nix it returns str. So, we convert any unicode objects to str.
-                            # Python 3 port update: In Python 3 everything is unicode and we should do nothing.
-                            # On Python 2 the above can happen: instead of checking for unicode, we check for `not str`.
-                            unicode_to_str = lambda s: s.encode('utf-8') if s and not isinstance(s, str) else s
-                            yield Interface(interface,
-                                            unicode_to_str(option.get("addr")),
-                                            unicode_to_str(option.get("netmask")),
-                                            unicode_to_str(option.get("broadcast")))
+                        addr, netmask, broadcast = [option.get(field) for field in ("addr", "netmask", "broadcast")]
+
+                        if netmask == "0.0.0.0":
+                            continue  # The network interface isn't bound to any network, so we skip it
 
+                        try:
+                            yield Interface(interface, addr, netmask, broadcast)
                         except TypeError:
                             # some interfaces have no netmask configured, causing a TypeError when
                             # trying to unpack _l_netmask
                             pass
         except OSError as e:
             logger = logging.getLogger("dispersy")
             logger.warning("failed to check network interfaces, error was: %r", e)
```

### Comparing `pyipv8-2.8.0/ipv8/messaging/interfaces/network_stats.py` & `pyipv8-2.9.0/ipv8/messaging/interfaces/network_stats.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/messaging/interfaces/statistics_endpoint.py` & `pyipv8-2.9.0/ipv8/messaging/interfaces/statistics_endpoint.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/messaging/interfaces/udp/endpoint.py` & `pyipv8-2.9.0/ipv8/messaging/interfaces/udp/endpoint.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/messaging/lazy_payload.py` & `pyipv8-2.9.0/ipv8/messaging/lazy_payload.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import inspect
 import types
-import typing
+from typing import Any, List, Type, TypeVar
 
 from .serialization import FormatListType, Payload
 
 
 class VariablePayload(Payload):
     """
     A Payload instance which mimics a struct. Useful for when you want a less verbose way to specify Payloads.
@@ -24,15 +24,15 @@
 
     If you require field-specific pack/unpack operations you can specify them using the `fix_pack_*` and
     `fix_unpack_*` methods.
     Custom packing and unpacking rules can be useful for compression methods like socket.inet_aton, which you only
     want to apply when actually sending over the wire.
     """
 
-    names: typing.List[str] = []
+    names: List[str] = []
 
     def __init__(self, *args, **kwargs):
         """
         Instantiate this VariablePayload class.
 
         :param args: the anonymous list of arguments, an index-based mapping to self.names and self.format_list
         :param kwargs: the named arguments, mapping to self.names and self.format_list (in no particular order)
@@ -85,25 +85,25 @@
     def _to_packlist_fmt(fmt: FormatListType) -> str:
         if isinstance(fmt, str):
             return fmt
         if isinstance(fmt, list):
             return 'payload-list'
         return 'payload'
 
-    def _fix_pack(self, name: str) -> typing.Any:
+    def _fix_pack(self, name: str) -> Any:
         """
         Check if there are custom rules for sending this field.
         """
         raw_value = getattr(self, name)
         custom_rule = "fix_pack_" + name
         if hasattr(self, custom_rule):
             return getattr(self, custom_rule)(raw_value)
         return raw_value
 
-    def to_pack_list(self) -> typing.List[tuple]:
+    def to_pack_list(self) -> List[tuple]:
         """
         Convert the VariablePayload to a Serializable pack list.
         This method will automatically pull from the available format names and set instance fields.
 
         :return: the pack list
         """
         out = []
@@ -113,15 +113,19 @@
             for _ in range(8 if self.format_list[i] == 'bits' else 1):
                 args.append(self._fix_pack(self.names[index]))
                 index += 1
             out.append((self._to_packlist_fmt(self.format_list[i]), *args))
         return out
 
 
-def _compile_init(names: typing.List[str]) -> types.CodeType:
+V = TypeVar('V', bound=VariablePayload)
+VT = Type[V]
+
+
+def _compile_init(names: List[str]) -> types.CodeType:
     """
     Compile the init function.
 
     Takes the form of:
 
      .. code-block :: Python
 
@@ -139,15 +143,15 @@
     Payload.__init__(self)
     %s
     """ % (', '.join(names),
            '\n    '.join(['self.%s = %s' % (name, name) for name in names]))
     return compile(f_code, f_code, 'exec')
 
 
-def _compile_from_unpack_list(src_cls: typing.Type[VariablePayload], names: typing.List[str]) -> types.CodeType:
+def _compile_from_unpack_list(src_cls: VT, names: List[str]) -> types.CodeType:
     """
     Compile the unpacking code.
 
     Takes the form of (``fix_unpack_`` is inserted if defined in the source class):
 
     .. code-block :: Python
 
@@ -167,17 +171,15 @@
     return cls(%s)
     """ % (arg_list, ', '.join(["None if %s is None else cls.fix_unpack_%s(%s)" % (name, name, name)
                                 if hasattr(src_cls, "fix_unpack_" + name)
                                 else name for name in names]))
     return compile(f_code, f_code, 'exec')
 
 
-def _compile_to_pack_list(src_cls: typing.Type[VariablePayload],
-                          format_list: typing.List[FormatListType],
-                          names: typing.List[str]) -> types.CodeType:
+def _compile_to_pack_list(src_cls: VT, format_list: List[FormatListType], names: List[str]) -> types.CodeType:
     """
     Compile the packing code.
 
     Takes the form of (``fix_pack_`` is inserted if defined in the source class):
 
     .. code-block :: Python
 
@@ -210,15 +212,15 @@
             index += 1
         derived_fmt = fmt if isinstance(fmt, str) else ("payload-list" if isinstance(fmt, list) else "payload")
         fmts.append('("%s", %s)' % (derived_fmt, ", ".join(args)))
     f_code %= ', '.join(fmts)
     return compile(f_code, f_code, 'exec')
 
 
-def vp_compile(vp_definition: typing.Type[VariablePayload]) -> typing.Type[VariablePayload]:
+def vp_compile(vp_definition: VT) -> VT:
     """
     JIT Compilation of a VariablePayload definition.
     """
 
     # We use ``exec`` purposefully here, disable the pylint warning:
     # pylint: disable=W0122
```

### Comparing `pyipv8-2.8.0/ipv8/messaging/payload.py` & `pyipv8-2.9.0/ipv8/messaging/payload.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/messaging/payload_dataclass.py` & `pyipv8-2.9.0/ipv8/messaging/payload_dataclass.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/messaging/payload_headers.py` & `pyipv8-2.9.0/ipv8/messaging/payload_headers.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/messaging/serialization.py` & `pyipv8-2.9.0/ipv8/messaging/serialization.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/overlay.py` & `pyipv8-2.9.0/ipv8/overlay.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/peer.py` & `pyipv8-2.9.0/ipv8/peer.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/peerdiscovery/churn.py` & `pyipv8-2.9.0/ipv8/peerdiscovery/churn.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/peerdiscovery/community.py` & `pyipv8-2.9.0/ipv8/peerdiscovery/community.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/peerdiscovery/discovery.py` & `pyipv8-2.9.0/ipv8/peerdiscovery/discovery.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/peerdiscovery/network.py` & `pyipv8-2.9.0/ipv8/peerdiscovery/network.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/peerdiscovery/payload.py` & `pyipv8-2.9.0/ipv8/peerdiscovery/payload.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/requestcache.py` & `pyipv8-2.9.0/ipv8/requestcache.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/taskmanager.py` & `pyipv8-2.9.0/ipv8/taskmanager.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/REST/rest_base.py` & `pyipv8-2.9.0/ipv8/test/REST/rest_base.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/REST/test_attestation_endpoint.py` & `pyipv8-2.9.0/ipv8/test/REST/test_attestation_endpoint.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/REST/test_identity_endpoint.py` & `pyipv8-2.9.0/ipv8/test/REST/test_identity_endpoint.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/REST/test_isolation_endpoint.py` & `pyipv8-2.9.0/ipv8/test/REST/test_isolation_endpoint.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/REST/test_network_endpoint.py` & `pyipv8-2.9.0/ipv8/test/REST/test_network_endpoint.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/REST/test_overlays_endpoint.py` & `pyipv8-2.9.0/ipv8/test/REST/test_overlays_endpoint.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/attestation/identity/test_identity.py` & `pyipv8-2.9.0/ipv8/test/attestation/identity/test_identity.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/attestation/identity/test_manager.py` & `pyipv8-2.9.0/ipv8/test/attestation/identity/test_manager.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/attestation/tokentree/test_token.py` & `pyipv8-2.9.0/ipv8/test/attestation/tokentree/test_token.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/attestation/tokentree/test_tree.py` & `pyipv8-2.9.0/ipv8/test/attestation/tokentree/test_tree.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/attestation/wallet/attestation.txt` & `pyipv8-2.9.0/ipv8/test/attestation/wallet/attestation.txt`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/attestation/wallet/attestation_big.txt` & `pyipv8-2.9.0/ipv8/test/attestation/wallet/attestation_big.txt`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/attestation/wallet/attestation_range.txt` & `pyipv8-2.9.0/ipv8/test/attestation/wallet/attestation_range.txt`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/attestation/wallet/bonehexact/test_attestation.py` & `pyipv8-2.9.0/ipv8/test/attestation/wallet/bonehexact/test_attestation.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/attestation/wallet/bonehexact/test_structs.py` & `pyipv8-2.9.0/ipv8/test/attestation/wallet/bonehexact/test_structs.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/attestation/wallet/irmaexact/test_algorithm.py` & `pyipv8-2.9.0/ipv8/test/attestation/wallet/irmaexact/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/attestation/wallet/irmaexact/test_builder.py` & `pyipv8-2.9.0/ipv8/test/attestation/wallet/irmaexact/test_builder.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/attestation/wallet/irmaexact/test_credential.py` & `pyipv8-2.9.0/ipv8/test/attestation/wallet/irmaexact/test_credential.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/attestation/wallet/irmaexact/test_keys.py` & `pyipv8-2.9.0/ipv8/test/attestation/wallet/irmaexact/test_keys.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/attestation/wallet/irmaexact/test_proofs.py` & `pyipv8-2.9.0/ipv8/test/attestation/wallet/irmaexact/test_proofs.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/attestation/wallet/pengbaorange/test_boudot.py` & `pyipv8-2.9.0/ipv8/test/attestation/wallet/pengbaorange/test_boudot.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/attestation/wallet/primitives/test_boneh.py` & `pyipv8-2.9.0/ipv8/test/attestation/wallet/primitives/test_boneh.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/attestation/wallet/primitives/test_ec.py` & `pyipv8-2.9.0/ipv8/test/attestation/wallet/primitives/test_ec.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/attestation/wallet/primitives/test_value.py` & `pyipv8-2.9.0/ipv8/test/attestation/wallet/primitives/test_value.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/attestation/wallet/test_attestation_community.py` & `pyipv8-2.9.0/ipv8/test/attestation/wallet/test_attestation_community.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/base.py` & `pyipv8-2.9.0/ipv8/test/base.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/bootstrapping/dispersy/test_bootstrapper.py` & `pyipv8-2.9.0/ipv8/test/bootstrapping/dispersy/test_bootstrapper.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/dht/test_churn.py` & `pyipv8-2.9.0/ipv8/test/dht/test_churn.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/dht/test_community.py` & `pyipv8-2.9.0/ipv8/test/dht/test_community.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/dht/test_discovery.py` & `pyipv8-2.9.0/ipv8/test/dht/test_discovery.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/dht/test_provider.py` & `pyipv8-2.9.0/ipv8/test/dht/test_provider.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/dht/test_routing.py` & `pyipv8-2.9.0/ipv8/test/dht/test_routing.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/dht/test_storage.py` & `pyipv8-2.9.0/ipv8/test/dht/test_storage.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/dht/test_trie.py` & `pyipv8-2.9.0/ipv8/test/dht/test_trie.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/keyvault/test_crypto.py` & `pyipv8-2.9.0/ipv8/test/keyvault/test_crypto.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/keyvault/test_serialization.py` & `pyipv8-2.9.0/ipv8/test/keyvault/test_serialization.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/keyvault/test_signature.py` & `pyipv8-2.9.0/ipv8/test/keyvault/test_signature.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/messaging/anonymization/mock.py` & `pyipv8-2.9.0/ipv8/test/messaging/anonymization/mock.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/messaging/anonymization/test_community.py` & `pyipv8-2.9.0/ipv8/test/messaging/anonymization/test_community.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from asyncio import Future
+from asyncio import Future, ensure_future, iscoroutine
+from functools import partial
 from unittest.mock import Mock
 
 from .mock import MockDHTProvider
 from ...base import TestBase
 from ...mocking.endpoint import MockEndpointListener
 from ...mocking.exit_socket import MockTunnelExitSocket
 from ...mocking.ipv8 import MockIPv8
@@ -10,14 +11,28 @@
 from ....messaging.anonymization.endpoint import TunnelEndpoint
 from ....messaging.anonymization.tunnel import (CIRCUIT_STATE_EXTENDING, PEER_FLAG_EXIT_BT,
                                                 PEER_FLAG_EXIT_IPV8, PEER_FLAG_SPEED_TEST)
 from ....messaging.interfaces.udp.endpoint import DomainAddress, UDPEndpoint
 from ....util import succeed
 
 
+def _on_packet_fragile_cb(self, source_address, data, circuit_id):
+    """
+    A fragile version of on_packet that crashes on message handling failures.
+
+    These failures won't actually cause IPv8 to crash in production, but you should probably handle these.
+
+    Add overlay classes to use in production mode to the ``production_overlay_classes`` list.
+    Filter nodes to run in production mode by overwriting ``TestBase.patch_overlays``.
+    """
+    result = self.decode_map_private[data[22]](source_address, data, circuit_id)
+    if iscoroutine(result):
+        self.register_anonymous_task('on_packet_from_circuit', ensure_future(result))
+
+
 class TestTunnelCommunity(TestBase):
 
     def setUp(self):
         super(TestTunnelCommunity, self).setUp()
         self.initialize(TunnelCommunity, 2)
 
         # An actual UDPEndpoint, if needed by the test (for catching exited data)
@@ -41,14 +56,19 @@
         ipv8.overlay.cancel_all_pending_tasks()
         # Finally, use the proper exitnode and circuit settings for manual creation
         ipv8.overlay.settings.min_circuits = 1
         ipv8.overlay.settings.max_circuits = 1
         ipv8.overlay.dht_provider = MockDHTProvider(ipv8.overlay.my_peer)
         return ipv8
 
+    def _patch_overlay(self, overlay):
+        super()._patch_overlay(overlay)
+        if overlay and overlay.__class__ not in self.production_overlay_classes:
+            overlay.on_packet_from_circuit = partial(_on_packet_fragile_cb, overlay)
+
     def assert_no_more_tunnels(self):
         """
         Utility method to check whether there are no more tunnels left
         """
         for node in self.nodes:
             self.assertFalse(node.overlay.exit_sockets)
             self.assertFalse(node.overlay.relay_from_to)
@@ -104,14 +124,36 @@
         await self.deliver_messages()
 
         # Node 0 should now have all of its required 1 hop circuits (1.0/100%)
         self.assertEqual(self.overlay(0).tunnels_ready(1), 1.0)
         # Node 1 has an exit socket open
         self.assertEqual(len(self.overlay(1).exit_sockets), 1)
 
+    async def test_create_circuit_destruct_initializing(self):
+        """
+        Check if a circuit is destructed and cleaned correctly while still initializing.
+        """
+        self.settings(1).peer_flags.add(PEER_FLAG_EXIT_BT)
+        await self.introduce_nodes()
+
+        # Let node 0 build a circuit of 1 hop with node 1
+        # We immediately remove it, before a response can be received
+        initializing_circuit = self.overlay(0).create_circuit(1).circuit_id
+        self.overlay(0).remove_circuit(initializing_circuit, remove_now=True)
+
+        # Let the circuit "creation" commence
+        await self.deliver_messages()
+
+        # Node 0 should have removed its initializing circuit
+        self.assertNotIn(initializing_circuit, self.overlay(0).circuits)
+        # Node 0 should not have any outstanding caches
+        self.assertListEqual(self.overlay(0).request_cache.get_tasks(), [])
+        # Node 1 has an exit socket open
+        self.assertEqual(len(self.overlay(1).exit_sockets), 1)
+
     async def test_create_circuit_no_exit(self):
         """
         Check if 1 hop circuit creation fails without exit nodes.
         """
         await self.introduce_nodes()
         self.overlay(0).build_tunnels(1)
```

### Comparing `pyipv8-2.8.0/ipv8/test/messaging/anonymization/test_datachecker.py` & `pyipv8-2.9.0/ipv8/test/messaging/anonymization/test_datachecker.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from ...base import TestBase
 from ....messaging.anonymization.tunnel import DataChecker
 
 tracker_pkt = unhexlify('00000417271019800000000012345678')
 dht_pkt = b'd1:ad2:id20:abcdefghij01234567899:info_hash20:mnopqrstuvwxyz123456e1:q9:get_peers1:t2:aa1:y1:qe'
 utp_pkt = unhexlify('210086446ed69ec1ddbd9e6000100000f32e86be')
+utp_ext3_pkt = unhexlify('110309d69087c1e7b69c0980001000009868b984000400000008')
 ipv8_pkt = unhexlify('0002123456789abcdef123456789abcdef123456789a00000001')
 tunnel_pkt = unhexlify('000281ded07332bdc775aa5a46f96de9f8f390bbc9f300000001')
 
 
 class TestDataChecker(TestBase):
 
     def test_could_be_dht(self):
@@ -35,14 +36,15 @@
     def test_could_be_utp(self):
         """
         Check if a UTP packet is correctly identified.
         """
         self.assertFalse(DataChecker.could_be_utp(tracker_pkt))
         self.assertFalse(DataChecker.could_be_utp(dht_pkt))
         self.assertTrue(DataChecker.could_be_utp(utp_pkt))
+        self.assertTrue(DataChecker.could_be_utp(utp_ext3_pkt))  # non-BEP29 extension 3 (close reason)
         self.assertFalse(DataChecker.could_be_utp(ipv8_pkt))
         self.assertFalse(DataChecker.could_be_utp(tunnel_pkt))
 
     def test_could_be_ipv8(self):
         """
         Check if a IPv8 packet is correctly identified.
         """
```

### Comparing `pyipv8-2.8.0/ipv8/test/messaging/anonymization/test_exit_socket.py` & `pyipv8-2.9.0/ipv8/test/messaging/anonymization/test_exit_socket.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/messaging/anonymization/test_hiddenservices.py` & `pyipv8-2.9.0/ipv8/test/messaging/anonymization/test_hiddenservices.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/messaging/interfaces/dispatcher/test_endpoint.py` & `pyipv8-2.9.0/ipv8/test/messaging/interfaces/dispatcher/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/messaging/interfaces/test_network_stats.py` & `pyipv8-2.9.0/ipv8/test/messaging/interfaces/test_network_stats.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/messaging/interfaces/test_statistics_endpoint.py` & `pyipv8-2.9.0/ipv8/test/messaging/interfaces/test_statistics_endpoint.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/messaging/interfaces/udp/test_endpoint.py` & `pyipv8-2.9.0/ipv8/test/messaging/interfaces/udp/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/messaging/test_lazy_payload.py` & `pyipv8-2.9.0/ipv8/test/messaging/test_lazy_payload.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/messaging/test_payload_dataclass.py` & `pyipv8-2.9.0/ipv8/test/messaging/test_payload_dataclass.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/messaging/test_serialization.py` & `pyipv8-2.9.0/ipv8/test/messaging/test_serialization.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/mocking/community.py` & `pyipv8-2.9.0/ipv8/test/mocking/community.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/mocking/endpoint.py` & `pyipv8-2.9.0/ipv8/test/mocking/endpoint.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/mocking/exit_socket.py` & `pyipv8-2.9.0/ipv8/test/mocking/exit_socket.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/mocking/ipv8.py` & `pyipv8-2.9.0/ipv8/test/mocking/ipv8.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/peerdiscovery/test_churn.py` & `pyipv8-2.9.0/ipv8/test/peerdiscovery/test_churn.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/peerdiscovery/test_community.py` & `pyipv8-2.9.0/ipv8/test/peerdiscovery/test_community.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/peerdiscovery/test_edge_discovery.py` & `pyipv8-2.9.0/ipv8/test/peerdiscovery/test_edge_discovery.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/peerdiscovery/test_network.py` & `pyipv8-2.9.0/ipv8/test/peerdiscovery/test_network.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/peerdiscovery/test_random_discovery.py` & `pyipv8-2.9.0/ipv8/test/peerdiscovery/test_random_discovery.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/test_configuration.py` & `pyipv8-2.9.0/ipv8/test/test_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+import base64
+
 from .base import TestBase
 from ..configuration import (Bootstrapper, BootstrapperDefinition, ConfigBuilder, DISPERSY_BOOTSTRAPPER, Strategy,
                              WalkerDefinition, get_default_configuration)
+from ..keyvault.crypto import default_eccrypto
+from ..keyvault.private.libnaclkey import LibNaCLSK
 
 
 class TestConfiguration(TestBase):
 
     def assertDictInDict(self, expected: dict, container: dict):
         self.assertTrue(any(all(entry.get(key) == expected[key] for key in expected.keys())
                             and len(entry) == len(expected)
@@ -129,14 +133,29 @@
             'file': "some file"
         }
         keys = builder.finalize()['keys']
 
         self.assertEqual(1 + len(get_default_configuration()['keys']), len(keys))
         self.assertTrue(any(set(entry.items()) == set(expected.items()) for entry in keys))
 
+    def test_add_ephemeral_key(self):
+        """
+        Check if ephemeral keys are created correctly.
+        """
+        builder = ConfigBuilder().add_ephemeral_key("my new key")
+
+        expected_keys = {'alias', 'bin', 'file'}
+        keys = builder.finalize()['keys']
+
+        self.assertEqual(1 + len(get_default_configuration()['keys']), len(keys))
+        self.assertTrue(any(entry.keys() == expected_keys for entry in keys))
+        self.assertEqual("my new key", keys[-1]["alias"])
+        self.assertEqual("", keys[-1]["file"])
+        self.assertIsInstance(default_eccrypto.key_from_private_bin(base64.b64decode(keys[-1]["bin"])), LibNaCLSK)
+
     def test_add_overlay_overwrite(self):
         """
         Check if the allow duplicate flag does not introduce duplicates.
         """
         builder = ConfigBuilder().add_overlay("DiscoveryCommunity", "anonymous id", [], [], {}, [],
                                               allow_duplicate=False)
```

### Comparing `pyipv8-2.8.0/ipv8/test/test_database.py` & `pyipv8-2.9.0/ipv8/test/test_database.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/test_loader.py` & `pyipv8-2.9.0/ipv8/test/test_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,22 +74,22 @@
         return [(MockWalk, {'some_attribute': 4}, 20)]
 
     def get_bootstrappers(self, session):
         return [(MockBootstrapper, {'some_attribute': 4})]
 
     def finalize(self, ipv8, session: MockSession, community: MockCommunity):
         session.community = community
-        return super()
+        super().finalize(ipv8, session, community)
 
 
 class TestCommunityLauncher(TestBase):
 
     def setUp(self):
         self.staged_launcher = StagedCommunityLauncher()
-        return super()
+        super().setUp()
 
     def test_not_before_list(self):
         """
         Check that the not_before decorator with multiple arguments equals the not_before() definition.
         """
         @after('CommunityLauncher1', 'CommunityLauncher2')
         class DecoratedCommunityLauncher(CommunityLauncher):
```

### Comparing `pyipv8-2.8.0/ipv8/test/test_peer.py` & `pyipv8-2.9.0/ipv8/test/test_peer.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/test_requestcache.py` & `pyipv8-2.9.0/ipv8/test/test_requestcache.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,30 +55,30 @@
         super().setUp()
         self.request_cache = RequestCache()
 
     async def test_shutdown(self):
         """
         Test if RequestCache does not allow new Caches after shutdown().
         """
-        num_tasks = len(all_tasks())
-        request_cache = RequestCache()  # This adds a task, don't use ``self.request_cache`` here!
-        request_cache.add(MockCache(request_cache))
-        self.assertEqual(len(all_tasks()), num_tasks + 2)
-        await request_cache.shutdown()
-        self.assertEqual(len(all_tasks()), num_tasks)
-        request_cache.add(MockCache(request_cache))
-        self.assertEqual(len(all_tasks()), num_tasks)
+        num_tasks = len(all_tasks())  # [Background tasks (depends on test runner) + RequestCache]
+        self.request_cache.add(MockCache(self.request_cache))
+        self.assertEqual(len(all_tasks()), num_tasks + 1)  # [Background + RequestCache + Cache]
+        await self.request_cache.shutdown()
+        self.assertEqual(len(all_tasks()), num_tasks - 1)  # [Background]
+        self.request_cache.add(MockCache(self.request_cache))  # No tasks should have been added
+        self.assertEqual(len(all_tasks()), num_tasks - 1)  # [Background]
 
     async def test_timeout(self):
         """
         Test if the cache.on_timeout() is called after the cache.timeout_delay.
         """
         cache = MockCache(self.request_cache)
         self.request_cache.add(cache)
         await cache.timed_out
+        await self.request_cache.shutdown()
 
     async def test_add_duplicate(self):
         """
         Test if adding a cache twice returns None as the newly added cache.
         """
         cache = MockCache(self.request_cache)
         self.request_cache.add(cache)
@@ -147,78 +147,92 @@
 
         with self.request_cache.passthrough():
             self.request_cache.add(cache)
             await sleep(0.0)
 
         self.assertTrue(cache.timed_out)
 
+        await self.request_cache.shutdown()
+
     async def test_passthrough_timeout(self):
         """
         Test if passthrough respects the timeout value.
         """
         cache = MockInfiniteCache(self.request_cache)
 
         with self.request_cache.passthrough(timeout=10.0):
             self.request_cache.add(cache)
             await sleep(0.0)
 
         self.assertFalse(cache.timed_out)
 
+        await self.request_cache.shutdown()
+
     async def test_passthrough_filter_one_match(self):
         """
         Test if passthrough filters correctly with one filter, that matches
         """
         cache = MockInfiniteCache(self.request_cache)
 
         with self.request_cache.passthrough(MockInfiniteCache):
             self.request_cache.add(cache)
             await sleep(0.0)
 
         self.assertTrue(cache.timed_out)
 
+        await self.request_cache.shutdown()
+
     async def test_passthrough_filter_one_mismatch(self):
         """
         Test if passthrough filters correctly with one filter, that doesn't match
         """
         cache = MockInfiniteCache(self.request_cache)
 
         with self.request_cache.passthrough(MockRegisteredCache):
             self.request_cache.add(cache)
             await sleep(0.0)
 
         self.assertFalse(cache.timed_out)
 
+        await self.request_cache.shutdown()
+
     async def test_passthrough_filter_many_match(self):
         """
         Test if passthrough filters correctly with many filters, that all match
         """
         cache = MockInfiniteCache(self.request_cache)
 
         with self.request_cache.passthrough(MockInfiniteCache, RandomNumberCache, NumberCache):
             self.request_cache.add(cache)
             await sleep(0.0)
 
         self.assertTrue(cache.timed_out)
 
+        await self.request_cache.shutdown()
+
     async def test_passthrough_filter_some_match(self):
         """
         Test if passthrough filters correctly with many filters, for which some match
         """
         cache = MockInfiniteCache(self.request_cache)
 
         with self.request_cache.passthrough(MockRegisteredCache, MockCache, RandomNumberCache):
             self.request_cache.add(cache)
             await sleep(0.0)
 
         self.assertTrue(cache.timed_out)
 
+        await self.request_cache.shutdown()
+
     async def test_passthrough_filter_no_match(self):
         """
         Test if passthrough filters correctly with many filters, for which none match
         """
         cache = MockInfiniteCache(self.request_cache)
 
         with self.request_cache.passthrough(MockRegisteredCache, MockCache):
             self.request_cache.add(cache)
             await sleep(0.0)
 
         self.assertFalse(cache.timed_out)
+
+        await self.request_cache.shutdown()
```

### Comparing `pyipv8-2.8.0/ipv8/test/test_taskmanager.py` & `pyipv8-2.9.0/ipv8/test/test_taskmanager.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/test/util.py` & `pyipv8-2.9.0/ipv8/test/util.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/types.py` & `pyipv8-2.9.0/ipv8/types.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8/util.py` & `pyipv8-2.9.0/ipv8/util.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/ipv8_service.py` & `pyipv8-2.9.0/ipv8_service.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/pyipv8.egg-info/PKG-INFO` & `pyipv8-2.9.0/pyipv8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyipv8
-Version: 2.8.0
+Version: 2.9.0
 Summary: The Python implementation of the IPV8 library
 Home-page: https://github.com/Tribler/py-ipv8
 Author: Tribler
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pyipv8-2.8.0/pyipv8.egg-info/SOURCES.txt` & `pyipv8-2.9.0/pyipv8.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 ipv8/peerdiscovery/churn.py
 ipv8/peerdiscovery/community.py
 ipv8/peerdiscovery/discovery.py
 ipv8/peerdiscovery/network.py
 ipv8/peerdiscovery/payload.py
 ipv8/test/__init__.py
 ipv8/test/base.py
-ipv8/test/test_community_compat.py
+ipv8/test/test_community.py
 ipv8/test/test_configuration.py
 ipv8/test/test_database.py
 ipv8/test/test_loader.py
 ipv8/test/test_peer.py
 ipv8/test/test_requestcache.py
 ipv8/test/test_taskmanager.py
 ipv8/test/util.py
@@ -198,14 +198,15 @@
 ipv8/test/messaging/anonymization/__init__.py
 ipv8/test/messaging/anonymization/mock.py
 ipv8/test/messaging/anonymization/test_community.py
 ipv8/test/messaging/anonymization/test_datachecker.py
 ipv8/test/messaging/anonymization/test_exit_socket.py
 ipv8/test/messaging/anonymization/test_hiddenservices.py
 ipv8/test/messaging/interfaces/__init__.py
+ipv8/test/messaging/interfaces/test_endpoint.py
 ipv8/test/messaging/interfaces/test_network_stats.py
 ipv8/test/messaging/interfaces/test_statistics_endpoint.py
 ipv8/test/messaging/interfaces/dispatcher/__init__.py
 ipv8/test/messaging/interfaces/dispatcher/test_endpoint.py
 ipv8/test/messaging/interfaces/udp/__init__.py
 ipv8/test/messaging/interfaces/udp/test_endpoint.py
 ipv8/test/mocking/__init__.py
```

### Comparing `pyipv8-2.8.0/setup.py` & `pyipv8-2.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 setup(
     name='pyipv8',
     author='Tribler',
     description='The Python implementation of the IPV8 library',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='2.8.0',  # Do not change manually! Handled by github_increment_version.py
+    version='2.9.0',  # Do not change manually! Handled by github_increment_version.py
     url='https://github.com/Tribler/py-ipv8',
     package_data={'': ['*.*']},
     packages=find_packages(),
     py_modules=['ipv8_service'],
     install_requires=[
         "cryptography",
         "libnacl",
```

### Comparing `pyipv8-2.8.0/simulation/discrete_loop.py` & `pyipv8-2.9.0/simulation/discrete_loop.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/simulation/simulation_endpoint.py` & `pyipv8-2.9.0/simulation/simulation_endpoint.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/stresstest/bootstrap_introductions.py` & `pyipv8-2.9.0/stresstest/bootstrap_introductions.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/stresstest/bootstrap_introductions.r` & `pyipv8-2.9.0/stresstest/bootstrap_introductions.r`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/stresstest/bootstrap_rtt.py` & `pyipv8-2.9.0/stresstest/bootstrap_rtt.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/stresstest/peer_discovery.py` & `pyipv8-2.9.0/stresstest/peer_discovery.py`

 * *Files identical despite different names*

### Comparing `pyipv8-2.8.0/stresstest/peer_discovery_defaults.py` & `pyipv8-2.9.0/stresstest/peer_discovery_defaults.py`

 * *Files identical despite different names*


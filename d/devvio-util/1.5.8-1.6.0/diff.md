# Comparing `tmp/devvio_util-1.5.8.tar.gz` & `tmp/devvio_util-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devvio_util-1.5.8.tar", last modified: Fri Jun 16 03:39:17 2023, max compression
+gzip compressed data, was "devvio_util-1.6.0.tar", last modified: Mon Jul 10 19:55:49 2023, max compression
```

## Comparing `devvio_util-1.5.8.tar` & `devvio_util-1.6.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:39:17.008532 devvio_util-1.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-16 03:39:17.008532 devvio_util-1.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:39:09.000000 devvio_util-1.5.8/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:39:17.000532 devvio_util-1.5.8/devvio_util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/lib_creds.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:39:17.008532 devvio_util-1.5.8/devvio_util/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/address.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/atomic_transaction_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/chainstate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/devv_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/devv_sign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/final_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/smart_coin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/primitives/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-16 03:39:09.000000 devvio_util-1.5.8/devvio_util/psql_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 03:39:17.004532 devvio_util-1.5.8/devvio_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-16 03:39:16.000000 devvio_util-1.5.8/devvio_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-16 03:39:16.000000 devvio_util-1.5.8/devvio_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 03:39:16.000000 devvio_util-1.5.8/devvio_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 03:39:16.000000 devvio_util-1.5.8/devvio_util.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 03:39:16.000000 devvio_util-1.5.8/devvio_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-16 03:39:16.000000 devvio_util-1.5.8/devvio_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 03:39:17.008532 devvio_util-1.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-16 03:39:09.000000 devvio_util-1.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:55:49.550386 devvio_util-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-10 19:55:49.550386 devvio_util-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:55:42.000000 devvio_util-1.6.0/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:55:49.550386 devvio_util-1.6.0/devvio_util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/lib_creds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:55:49.550386 devvio_util-1.6.0/devvio_util/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/atomic_transaction_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/chainstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/devv_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/devv_sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/final_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/smart_coin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/primitives/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-07-10 19:55:42.000000 devvio_util-1.6.0/devvio_util/psql_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:55:49.550386 devvio_util-1.6.0/devvio_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-10 19:55:49.000000 devvio_util-1.6.0/devvio_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-10 19:55:49.000000 devvio_util-1.6.0/devvio_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:55:49.000000 devvio_util-1.6.0/devvio_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:55:49.000000 devvio_util-1.6.0/devvio_util.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-10 19:55:49.000000 devvio_util-1.6.0/devvio_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-10 19:55:49.000000 devvio_util-1.6.0/devvio_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-10 19:55:49.550386 devvio_util-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-10 19:55:42.000000 devvio_util-1.6.0/setup.py
```

### Comparing `devvio_util-1.5.8/devvio_util/config.py` & `devvio_util-1.6.0/devvio_util/config.py`

 * *Files identical despite different names*

### Comparing `devvio_util-1.5.8/devvio_util/lib_creds.py` & `devvio_util-1.6.0/devvio_util/lib_creds.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# reload(sys)
-# sys.setdefaultencoding('utf-8')
 import json
 import boto3
 import base64
 from botocore.exceptions import ClientError
 from abc import ABC
 
 
@@ -78,15 +76,15 @@
                 # You provided a parameter value that is not valid for the current state of the resource.
                 # Deal with the exception here, and/or rethrow at your discretion.
                 raise e
             elif e.response["Error"]["Code"] == "ResourceNotFoundException":
                 # We can't find the resource that you asked for.
                 # Deal with the exception here, and/or rethrow at your discretion.
                 raise e
-            return None
+            return e
         else:
             # Decrypts secret using the associated KMS key.
             # Depending on whether the secret is a string or binary, one of these fields will be populated.
             if "SecretString" in get_secret_value_response:
                 secret = get_secret_value_response["SecretString"]
             else:
                 secret = base64.b64decode(get_secret_value_response["SecretBinary"])
```

### Comparing `devvio_util-1.5.8/devvio_util/primitives/chainstate.py` & `devvio_util-1.6.0/devvio_util/primitives/chainstate.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,62 +1,88 @@
 from devvio_util.primitives.devv_constants import kPROTOCOL_VERSION
 from devvio_util.primitives.address import Address
 from devvio_util.primitives.smart_coin import SmartCoin
 from devvio_util.primitives.summary import Summary
 
 
 class Chainstate:
-
+    """
+    Holds the state of the chain in the form of a map with wallet addresses as keys
+    and lists of coin/balance pairs as values
+    """
     def __init__(self):
         self._state_map = dict()
 
     def get_state_map(self) -> dict:
+        """
+        Returns the chainstate as a dictionary.
+        :return: A map with wallet addresses as keys and lists of coin/balance pairs as values
+        :rtype: dict
+        """
         return self._state_map
 
-    def get_amount(self, coin_id: int, addr: Address):
+    def get_amount(self, coin_id: int, addr: Address) -> int:
+        """
+        Returns the given wallet's balance for a coin.
+        :param coin_id: request balance for this coin
+        :type coin_id: int
+        :param addr: the Address of the wallet to check
+        :type addr: Address
+        :return: the wallet's coin balance
+        :rtype: int
+        """
         addr_iter = self._state_map.get(addr.get_hex_str())
         if addr_iter:
             coin_map = addr_iter[1]
             coin_iter = coin_map[coin_id]
             if coin_iter:
                 amount = coin_map[coin_id]
                 return amount
         return 0
 
-    def add_coin(self, coin: SmartCoin) -> bool:
-        no_error = True
-        if not coin:
-            return False
-        if not isinstance(self._state_map, dict):
-            return False
+    def add_coin(self, coin: SmartCoin):
+        """
+        Updates a wallet's coin balance for this Chainstate
+        :param coin: holds the coinId, Address, and amount to update the state map with
+        :type coin: SmartCoin
+        """
         it = self._state_map.get(coin.get_address().get_hex_str())
         if it and it.get(coin.get_coin()):
             it[coin.get_coin()] += coin.get_amount()
         elif it:
             it[coin.get_coin()] = coin.get_amount()
         else:
             inner = dict()
             inner[coin.get_coin()] = coin.get_amount()
             self._state_map[coin.get_address().get_hex_str()] = inner
-        return no_error
 
-    def update(self, summ: Summary) -> bool:
+    def update(self, summ: Summary):
+        """
+        Updates the Chainstate with a block's Summary
+        :param summ: summary of transactions within a block
+        :type summ: Summary
+        """
         if not summ.is_sane():
-            raise Exception('Chainstate update failed: Summary is not sane')
+            raise RuntimeError('Chainstate update failed: Summary is not sane')
         prev_state = self._state_map
         for xfer in summ.get_xfers():
             coin = SmartCoin(xfer.get_addr(), xfer.get_coin(), xfer.get_amount())
-            if not self.add_coin(coin):
+            try:
+                self.add_coin(coin)
+            except Exception as e:
                 self._state_map = prev_state
-                raise Exception(f'Chainstate update failed: failed to add SmartCoin to state '
-                                f'(addr:{coin.get_address()}; coin:{coin.get_coin()}; amount:{coin.get_amount()})')
-        return True
+                raise RuntimeError(f'Failed to add SmartCoin to Chainstate: {e} '
+                                   f'(addr:{coin.get_address()}; coin:{coin.get_coin()}; amount:{coin.get_amount()})')
 
 
 class ChainCheckpoint:
+    """
+    Holds a snapshot of the chainstate
+    """
     def __init__(self):
         self._version = kPROTOCOL_VERSION
         self._highest_block_hash = None
         self._chainstate_summary = None
         self._signer = None
         self._checkpoint_hash = None
         self._signature = None
+        raise NotImplementedError
```

### Comparing `devvio_util-1.5.8/devvio_util/primitives/devv_constants.py` & `devvio_util-1.6.0/devvio_util/primitives/devv_constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 kPREV_HASH_SIZE = 32
 
 kPEM_PREFIX = '-----BEGIN ENCRYPTED PRIVATE KEY-----\n'
 kPEM_SUFFIX = '\n-----END ENCRYPTED PRIVATE KEY-----'
 kPEM_PREFIX_SIZE = len(kPEM_PREFIX)
 kPEM_SUFFIX_SIZE = len(kPEM_SUFFIX)
 
+VALID_BLOCK_VERSIONS = [0, 1]
+
 
 class OpType:
     CREATE = 0
     MODIFY = 1
     SEND = 2
     DELETE = 3
     REVERT = 4
@@ -45,9 +47,9 @@
     SUMMARIZE = 6
     RECOVER = 7
     NUM_OPS = 8
 
     def get(self, op: str) -> int:
         try:
             return self.__getattribute__(op)
-        except Exception as e:
+        except Exception:
             raise Exception(f"Invalid op string {op}")
```

### Comparing `devvio_util-1.5.8/devvio_util/primitives/devv_sign.py` & `devvio_util-1.6.0/devvio_util/primitives/devv_sign.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 import pkg_resources
 
 kWALLET_CURVE = ec.SECP256K1()
 kNODE_CURVE = ec.SECP384R1()
 
 
 def crypto_sanity_check(pkey: str = None, pub: str or Address = None, aes_pass: str = None) -> tuple:
-    """ Tests the cryptographic methods in this devv_sign module. Can be used to validate a given keypair and aes key,
+    """
+    Tests the cryptographic methods in this devv_sign module. Can be used to validate a given keypair and aes key,
     otherwise will generate a test key
 
     :param pkey: str of private key, without PEM prefix/suffix or newlines
     :type pkey: str
     :param pub: public key as a hex string or devvio-util Address object
     :type pub: str
     :param aes_pass: aes key to decrypt/encrypt the pkey with
@@ -41,14 +42,21 @@
     sign_binary(pkey, pub, msg, aes_pass)
     crypto_version = str(pkg_resources.get_distribution('cryptography'))
     openssl_version = backend.openssl_version_text()
     return openssl_version, crypto_version
 
 
 def format_pkey(pkey: str) -> bytes:
+    """
+    Formats a plain private key to be loaded by EcSigner
+    :param pkey: private key string with no newlines or PEM-prefixes/suffixes
+    :type pkey: str
+    :return: binary for the PEM-formatted key (with no newlines)
+    :rtype: bytes
+    """
     return bytes(kPEM_PREFIX + pkey + kPEM_SUFFIX, 'utf-8')
 
 
 def sign_binary(pkey: str, pub: str or Address, msg: bytes, aes_pass: str) -> Signature:
     """ Signs the given msg binary using the given keypair and aes key, and validates the signature
 
     :param pkey: str of private key, without PEM prefix/suffix or newlines
@@ -79,17 +87,15 @@
             padding = b''
             for i in range(pad_len - sig_size):
                 padding += set_uint8(0)
             sig += padding
         elif sig_size > pad_len:
             sig = sig[:pad_len]
 
-        sig = Signature(sig)
-
-        return sig
+        return Signature(sig)
     except Exception as e:
         raise RuntimeError(f"Signature procedure failed ({e})")
 
 
 class EcSigner:
     """Can be used to parse PEM files, generate keypairs, create signatures, and verify signatures."""
     def __init__(self, pkey: bytes = None, pub: str or Address = None, aes_pass: str = None,
@@ -98,15 +104,16 @@
 
         :param pkey: bytes of private key in PEM format
         :type pkey: bytes
         :param pub: public key as a hex string or devvio-util Address object
         :type pub: str
         :param aes_pass: aes key to decrypt/encrypt the PEM file with; this is required
         :type aes_pass: str
-        :param curve: elliptic curve to use in generating/loading the key; defaults to devv_sign.kWALLET_CURVE (SECP256K1)
+        :param curve: elliptic curve to use in generating/loading the key;
+        defaults to devv_sign.kWALLET_CURVE (SECP256K1)
         :type curve: ec.EllipticCurve
         """
         if not aes_pass:
             raise ValueError('Invalid EcSigner: aes_pass cannot be empty')
         self._alg = ec.ECDSA(SHA256())
         self._curve = None
         self._pem_encryption = None
@@ -136,15 +143,15 @@
                 encoding=sz.Encoding.PEM,
                 format=sz.PrivateFormat.PKCS8,
                 encryption_algorithm=self._pem_encryption,
             )
 
             self._pub = ec_key.public_key()
         except Exception as e:
-            raise Exception(f'Invalid EcSigner: failed to generate EC key-pair ({e})')
+            raise RuntimeError(f'Invalid EcSigner: failed to generate EC key-pair ({e})')
 
     def _load_ec_key(self, pub: str or Address, aes_pass: str):
         """ Load a keypair from the given private key and aes key,
         and verify that its public address matches the given one
 
         :param pub: the given public key, to compare against the public key generated from the given private key
         :type pub: str
@@ -166,18 +173,17 @@
             password=bytes(aes_pass, 'utf-8'),
             backend=default_backend()
         )
 
         self._pem_encryption = None
         self._pub = self._pk.public_key()
 
-        if not isinstance(pub, Address):
-            pub = Address(pub)
-        if self.get_signer_addr() != pub:
-            raise Exception(f'Invalid EcSigner: could not reproduce public key')
+        pub_addr = pub if isinstance(pub, Address) else Address(pub)
+        if self.get_signer_addr() != pub_addr:
+            raise RuntimeError('Invalid EcSigner: could not reproduce public key')
 
     def get_pkey(self) -> str:
         """
         :return: this EcSigner's encrypted private key in string form, without PEM prefix/suffix or newlines
         :rtype: str
         """
         return self._pk.decode('utf-8')[kPEM_PREFIX_SIZE:-kPEM_SUFFIX_SIZE].replace('\n', '')
@@ -204,18 +210,18 @@
         :type msg: bytes
         :param verify: if True, verify the signature
         :type verify: bool
         :return: a new signature for the given bytes
         :rtype: bytes
         """
         if not msg or not isinstance(msg, bytes):
-            raise Exception(f'Invalid signing: cannot sign msg type {type(msg)}')
+            raise RuntimeError(f'Invalid signing: cannot sign msg type {type(msg)}')
         sig = self._pk.sign(msg, self._alg)
         if verify and not self.verify(sig, msg):
-            raise Exception('Invalid signing: failed sig verification')
+            raise RuntimeError('Invalid signing: failed sig verification')
         return sig
 
     def verify(self, sig, msg) -> bool:
         try:
             self._pub.verify(sig, msg, self._alg)
             return True
         except InvalidSignature:
```

### Comparing `devvio_util-1.5.8/devvio_util/primitives/transaction.py` & `devvio_util-1.6.0/devvio_util/primitives/transaction.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,100 +44,151 @@
             self._tx_size = buffer.get_next_uint64()
             self._xfer_size = buffer.get_next_uint64()
             self._payload_size = buffer.get_next_uint64()
             self._signer_size = buffer.get_int(self._tx_offset + kSIGNER_LENGTH_OFFSET, kUINT_SIZE) + 1
             self._signer = Address(buffer.get_bytes(self._tx_offset + kSIGNER_LENGTH_OFFSET, self._signer_size))
 
         if self._payload_size < kMIN_PAYLOAD_SIZE:
-            raise Exception(f"Invalid Transaction: bad payload size {self._payload_size}")
+            raise RuntimeError(f"Invalid Transaction: bad payload size {self._payload_size}")
 
         if not Address.is_valid_addr_size(self._signer_size):
-            raise Exception(f"Invalid Transaction: bad signer size {self._signer_size}")
+            raise RuntimeError(f"Invalid Transaction: bad signer size {self._signer_size}")
 
         if not is_legacy:
             flags = buffer.get_int(self._tx_offset + kFLAGS_OFFSET, kUINT_SIZE)
             if flags != 0:
-                raise Exception("Invalid Transaction: unknown flags")
+                raise RuntimeError("Invalid Transaction: unknown flags")
             oper = buffer.get_int(self._tx_offset + kOPERATION_OFFSET, kUINT_SIZE)
             if oper >= OpType.NUM_OPS:
-                raise Exception("Invalid Transaction: invalid operation")
+                raise RuntimeError("Invalid Transaction: invalid operation")
         else:
             oper = buffer.get_int(self._tx_offset + kLEGACY_OPERATION_OFFSET, kUINT_SIZE)
             if oper >= OpType.NUM_OPS:
-                raise Exception("Invalid Transaction: invalid operation")
+                raise RuntimeError("Invalid Transaction: invalid operation")
             self._is_legacy = True
         self._sig = self.get_sig_from_raw_blk(buffer)
         buffer.seek(self._tx_offset)
         self._canonical = buffer.get_next_bytes(self._tx_size)
         if not self._canonical:
-            raise Exception(f"Invalid Transaction: buffer too small for tx (< {self._tx_size}")
+            raise RuntimeError(f"Invalid Transaction: buffer too small for tx (< {self._tx_size}")
 
     def get_sig_from_raw_blk(self, buffer: InputBuffer) -> Signature:
         """
+        Get signature from InputBuffer.
         :param buffer: IO stream holding the Transaction binary
         :type buffer: InputBuffer
         :return: Signature object holding the sig for this transaction
         :rtype: Signature
         """
         if self._is_legacy:
             offset = self._tx_offset + kLEGACY_ENVELOPE_SIZE + self._payload_size + self._xfer_size + 1
         else:
             offset = kENVELOPE_SIZE + self._payload_size + self._xfer_size + self._signer_size
         sig_len = self._tx_size - offset
         return Signature(buffer.get_bytes(self._tx_offset + offset, sig_len))
 
     def get_sig(self) -> Signature:
+        """
+        Get transaction signature, if one exists
+        :return: tx signature
+        :rtype: Signature
+        """
         if self._sig:
             return self._sig
         if self._is_legacy:
             offset = kLEGACY_ENVELOPE_SIZE + self._payload_size + self._xfer_size + 1
         else:
             offset = kENVELOPE_SIZE + self._payload_size + self._xfer_size + self._signer_size
         raw_sig = self._canonical[offset:]
         if not raw_sig:
             return None
         return Signature(raw_sig)
 
     def get_op(self) -> int:
+        """
+        Pull transaction operation from canonical as an integer.
+        Consistent with devv_constants.OpTypes, where
+            CREATE = 0
+            MODIFY = 1
+            SEND = 2
+            DELETE = 3
+            REVERT = 4
+            CONFIRM = 5
+            SUMMARIZE = 6
+            RECOVER = 7
+
+        :return: tx operation
+        :rtype: int
+        """
         return self._canonical[kOPERATION_OFFSET] if not self._is_legacy else self._canonical[kLEGACY_OPERATION_OFFSET]
 
     def get_flags(self) -> int:
+        """
+        Pull flag from canonical as an integer.
+        :return: tx flag
+        :rtype: int
+        """
         return self._canonical[kFLAGS_OFFSET] if not self._is_legacy else None
 
     def get_timestamp(self) -> int:
+        """
+        Pull timestamp from canonical as an integer.
+        :return: tx timestamp
+        :rtype: int
+        """
         return get_int(self._canonical[kTIMESTAMP_OFFSET:kTIMESTAMP_OFFSET + 8], False)
 
     def get_payload(self) -> str:
+        """
+        Decode payload from canonical into a string.
+        :return: tx payload
+        :rtype: str
+        """
         if self._is_legacy:
             offset = kNODE_ADDR_BUF_SIZE + self._xfer_size + self._signer_size
         else:
             offset = kENVELOPE_SIZE + self._xfer_size + self._signer_size
         return self.get_canonical()[offset:offset + self._payload_size].decode('utf-8')
 
     def __len__(self):
         return self.get_size()
 
     def get_size(self) -> int:
+        """
+        Get transaction size, in number of bytes.
+        :return: tx size
+        :rtype: int
+        """
         return self._tx_size
 
     def get_canonical(self) -> bytes:
+        """
+        Get transaction binary.
+        :return: tx binary
+        :rtype: bytes
+        """
         return self._canonical
 
     def get_hex_str(self) -> str or None:
+        """
+        Get hex representation of tx binary.
+        :return: tx canonical as hex string
+        :rtype: str
+        """
         if not self._canonical:
             return None
         return self._canonical.hex()
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.get_hex_str()
 
-    def __bool__(self):
+    def __bool__(self) -> bool:
         return self._sig is not None
 
-    def __eq__(self, other):
+    def __eq__(self, other) -> bool:
         return self._sig == other.get_sig()
 
     def get_xfers_from_raw_blk(self, buffer: InputBuffer) -> list:
         """
         :param buffer: binary buffer holding the Transaction data
         :type buffer: InputBuffer
         :return: list of Transfer objects for this Transaction
@@ -155,22 +206,24 @@
         :rtype: list
         """
         buffer = InputBuffer(self._canonical)
         return Transfer.get_xfers_from_buffer(buffer, kENVELOPE_SIZE + self._signer_size, self._xfer_size)
 
     def get_message_digest(self) -> bytes:
         """
+        Get tx binary, excluding signature; this binary is the message used to generate new tx signatures.
         :return: transaction binary, excluding the signature if one is present.
         :rtype: bytes
         """
         return self._canonical[:kENVELOPE_SIZE + self._signer_size + self._xfer_size + self._payload_size]
 
-    def _pre_signature_init(self, oper: int, signer: Address, xfers: list, payload: bytes, flags: int,
-                           timestamp: int):
+    def _pre_signature_init(self, oper: int, signer: Address, xfers: list, payload: bytes, flags: int, timestamp: int):
         # TODO: accommodate serialization for legacy txs
+        if self._is_legacy:
+            raise NotImplementedError('Serialization only available for non-legacy txs')
         self._payload_size = len(payload)
 
         if self._payload_size < kMIN_PAYLOAD_SIZE:
             raise ValueError(f"Failed to serialize transaction, payload too small ({self._payload_size})")
 
         self._canonical = bytes()
         self._canonical += set_uint64(self._payload_size)
@@ -186,16 +239,16 @@
 
         self._xfer_size = 0
         for xfer in xfers:
             self._xfer_size += xfer.get_size() + 1
             self._canonical += xfer.get_canonical()
 
         self._signer_size = signer.get_size() + 1
-        self._tx_size = kENVELOPE_SIZE + self._signer_size + self._xfer_size + self._payload_size \
-                        + signer.get_corresponding_sig_size()
+        self._tx_size = kENVELOPE_SIZE + self._signer_size + self._xfer_size + \
+            self._payload_size + signer.get_corresponding_sig_size()
 
         self._canonical = set_uint64(self._tx_size) + set_uint64(self._xfer_size) + self._canonical
 
     def serialize(self, oper: int, xfers: list, payload: bytes, flags: int,
                   timestamp: int, sig: Signature = None, is_legacy: bool = False):
         """
         Initialize Transaction attributes and generate canonical form.
@@ -219,21 +272,21 @@
         """
         self._signer = None
         for xfer in xfers:
             if xfer.get_amount() < 0:
                 self._signer = xfer.get_addr()
                 break
         if not self._signer:
-            raise Exception('Invalid Transaction: one Transfer must have amount < 0')
+            raise RuntimeError('Invalid Transaction: one Transfer must have amount < 0')
 
         self._is_legacy = is_legacy
         self._pre_signature_init(oper, self._signer, xfers, payload, flags, timestamp)
         self._canonical += payload
         if (size := len(self._canonical)) != (exp_size := self._tx_size - self._signer.get_corresponding_sig_size()):
-            raise Exception(f"Invalid Transaction: unexpected canonical length ({size} != {exp_size})")
+            raise RuntimeError(f"Invalid Transaction: unexpected canonical length ({size} != {exp_size})")
         if sig:
             self.set_sig(sig)
         return self
 
     def set_sig(self, sig: Signature or str):
         """
         Add the given signature to the Transaction's current canonical form.
@@ -284,29 +337,33 @@
         :return: the initialized Transaction object
         :rtype: Transaction
         """
         try:
             # construct xfers
             xfers = [Transfer(xfer) for xfer in props['xfers']]
             if not xfers:
-                raise Exception('Invalid Transaction: failed to parse any xfers')
+                raise RuntimeError('Invalid Transaction: failed to parse any xfers')
 
             # get payload binary
             payload = bytes(props['payload'], 'utf-8')
 
             # check operation type
             if isinstance(props['op'], str):
                 op = OpType().get(props['op'])
             elif props['op'] >= OpType.NUM_OPS:
-                raise Exception(f"Invalid Transaction: bad op int {props['op']}")
+                raise RuntimeError(f"Invalid Transaction: bad op int {props['op']}")
             else:
                 op = props['op']
 
             # initialize attributes and construct canonical
             return self.serialize(op, xfers, payload, props['flags'], props['timestamp'],
                                   sig=props.get('sig'), is_legacy=props.get('legacy'))
         except KeyError as ke:
-            raise Exception(f"Invalid Transaction: failed to set property ({ke})")
+            raise RuntimeError(f"Invalid Transaction: failed to set property ({ke})")
 
     def get_signer(self) -> Address:
+        """
+        Return the Address corresponding to the Transfer with amount < 0
+        :return: the node or wallet in charge of signing this tx
+        :rtype: Address
+        """
         return self._signer
-
```

### Comparing `devvio_util-1.5.8/devvio_util/primitives/utils.py` & `devvio_util-1.6.0/devvio_util/primitives/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 from io import BytesIO
 from _io import BufferedReader
 from devvio_util.primitives.devv_constants import kUINT64_SIZE, kUINT32_SIZE, kUINT_SIZE, \
     kMERKLE_SIZE, kPREV_HASH_SIZE
 
 
 class InputBuffer:
+    """
+    Utilizes a BytesIO stream to parse various useful types.
+    Can be instantiated with a filepath, bytes object, or BytesIO object.
+    If used in a 'with' statement, will clean itself up upon exit.
+    """
     def __init__(self, file: str or bytes or BytesIO):
         if isinstance(file, str):
             self._reader = BytesIO(open(file, 'rb').read())
         elif isinstance(file, bytes):
             self._reader = BytesIO(file)
         elif isinstance(file, BytesIO):
             self._reader = file
         elif isinstance(file, BufferedReader):
             self._reader = BytesIO(file.read())
         else:
-            raise Exception(f"Invalid InputBuffer: need bytes, filepath, BytesIO, or BufferedReader\
+            raise RuntimeError(f"Invalid InputBuffer: need bytes, filepath, BytesIO, or BufferedReader\
                  (given {type(file)})")
         self._size = len(self._reader.read())
         self._reader.seek(0)
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args, **kwargs):
         self._reader.__exit__()
 
-    def __sizeof__(self):
+    def __sizeof__(self) -> int:
         return self._size
 
-    def __getitem__(self, index: tuple):
+    def __getitem__(self, index: tuple) -> bytes:
         offset, num_bytes = index
         return self.get_bytes(offset, num_bytes)
 
     def get_next_uint64(self, increment: bool = True) -> int:
         return self.get_next_int(kUINT64_SIZE, increment)
 
     def get_next_int64(self, increment: bool = True) -> int:
@@ -55,52 +60,56 @@
         result = self.get_next_bytes(num_bytes, increment).hex()
         return result
 
     def get_next_int(self, num_bytes: int, increment: bool = True, signed: bool = False, ) -> int:
         result = get_int(self.get_next_bytes(num_bytes, increment), signed)
         return result
 
-    def get_next_prefixed_obj(self, increment: bool = True):
+    def get_next_prefixed_obj(self, increment: bool = True) -> bytes:
         offset = self.tell()
         size = self.get_next_uint8()
         res = self.get_next_bytes(size)
         if not res or not increment:
             self.seek(offset)
         return res
 
     def get_next_bytes(self, num_bytes: int, increment: bool = True) -> bytes:
         result = self._reader.read(num_bytes)
         if not increment:
             self._reader.seek(self._reader.tell() - num_bytes)
         return result
 
-    def get_bytes(self, offset: int, num_bytes: int):
+    def get_bytes(self, offset: int, num_bytes: int) -> bytes:
         curr_offset = self._reader.tell()
         self._reader.seek(offset)
         result = self.get_next_bytes(num_bytes, False)
         self._reader.seek(curr_offset)
         return result
 
-    def get_int(self, offset: int, num_bytes: int):
+    def get_int(self, offset: int, num_bytes: int) -> int:
         curr_offset = self._reader.tell()
         self._reader.seek(offset)
         result = self.get_next_int(num_bytes, False)
         self._reader.seek(curr_offset)
         return result
 
     def seek(self, offset: int):
         self._reader.seek(offset)
 
     def tell(self) -> int:
         return self._reader.tell()
 
+    def read(self, size: int = -1):
+        return self._reader.read(size)
+
 
 def get_int(x: bytes, signed: bool) -> int:
     return int.from_bytes(x, 'little', signed=signed)
 
+
 def set_uint64(x: int) -> bytes:
     return set_int(x, kUINT64_SIZE, False)
 
 
 def set_uint32(x: int) -> bytes:
     return set_int(x, kUINT32_SIZE, False)
 
@@ -113,7 +122,9 @@
     return set_int(x, kUINT_SIZE, False)
 
 
 def set_int(x: int, num_bytes: int, signed: bool) -> bytes:
     return x.to_bytes(num_bytes, 'little', signed=signed)
 
 
+def is_hex(s: str) -> bool:
+    return not set(s) - set("abcdefABCDEF0123456789")
```

### Comparing `devvio_util-1.5.8/devvio_util.egg-info/SOURCES.txt` & `devvio_util-1.6.0/devvio_util.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 README.txt
 setup.cfg
 setup.py
 devvio_util/__init__.py
 devvio_util/config.py
 devvio_util/lib_creds.py
+devvio_util/logging.py
 devvio_util/psql_mixin.py
 devvio_util.egg-info/PKG-INFO
 devvio_util.egg-info/SOURCES.txt
 devvio_util.egg-info/dependency_links.txt
 devvio_util.egg-info/not-zip-safe
 devvio_util.egg-info/requires.txt
 devvio_util.egg-info/top_level.txt
 devvio_util/primitives/__init__.py
 devvio_util/primitives/address.py
 devvio_util/primitives/atomic_transaction_set.py
 devvio_util/primitives/chainstate.py
 devvio_util/primitives/devv_constants.py
 devvio_util/primitives/devv_sign.py
+devvio_util/primitives/errors.py
 devvio_util/primitives/final_block.py
 devvio_util/primitives/signature.py
 devvio_util/primitives/smart_coin.py
 devvio_util/primitives/summary.py
 devvio_util/primitives/transaction.py
 devvio_util/primitives/transfer.py
 devvio_util/primitives/utils.py
```

### Comparing `devvio_util-1.5.8/setup.py` & `devvio_util-1.6.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from setuptools import setup
+VERSION = 'v1.6.0'
 
 setup(name='devvio_util',
-      version='1.5.8',
+      version=VERSION,
       long_description=open('README.txt').read(),
       long_description_content_type='text/markdown',
       description='Utility to be used inside Devvio projects',
       author='Devvio Team',
       author_email='support@devv.io',
       license='Devvio',
       packages=['devvio_util', 'devvio_util/primitives'],
```


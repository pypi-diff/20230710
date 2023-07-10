# Comparing `tmp/pyCSM-1.0.2.tar.gz` & `tmp/pyCSM-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyCSM-1.0.2.tar", last modified: Tue Mar 28 19:56:38 2023, max compression
+gzip compressed data, was "pyCSM-1.0.3.tar", last modified: Mon Jul 10 15:36:13 2023, max compression
```

## Comparing `pyCSM-1.0.2.tar` & `pyCSM-1.0.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 blead761   (501) staff       (20)        0 2023-03-28 19:56:38.366373 pyCSM-1.0.2/
--rw-r--r--   0 blead761   (501) staff       (20)    11357 2022-04-11 15:23:08.000000 pyCSM-1.0.2/LICENSE
--rw-r--r--   0 blead761   (501) staff       (20)      727 2023-03-28 19:56:38.366229 pyCSM-1.0.2/PKG-INFO
--rw-r--r--   0 blead761   (501) staff       (20)     3808 2022-06-27 20:29:53.000000 pyCSM-1.0.2/README.md
-drwxr-xr-x   0 blead761   (501) staff       (20)        0 2023-03-28 19:56:38.359733 pyCSM-1.0.2/docs/
--rw-r--r--   0 blead761   (501) staff       (20)        0 2022-06-27 20:29:53.000000 pyCSM-1.0.2/docs/__init__.py
--rw-r--r--   0 blead761   (501) staff       (20)     2751 2022-06-22 19:08:15.000000 pyCSM-1.0.2/docs/conf.py
-drwxr-xr-x   0 blead761   (501) staff       (20)        0 2023-03-28 19:56:38.360064 pyCSM-1.0.2/pyCSM/
--rw-r--r--   0 blead761   (501) staff       (20)        0 2022-06-27 20:29:53.000000 pyCSM-1.0.2/pyCSM/__init__.py
-drwxr-xr-x   0 blead761   (501) staff       (20)        0 2023-03-28 19:56:38.361274 pyCSM-1.0.2/pyCSM/authorization/
--rw-r--r--   0 blead761   (501) staff       (20)        0 2022-06-27 20:29:53.000000 pyCSM-1.0.2/pyCSM/authorization/__init__.py
--rw-r--r--   0 blead761   (501) staff       (20)     1854 2022-09-09 20:08:40.000000 pyCSM-1.0.2/pyCSM/authorization/auth.py
-drwxr-xr-x   0 blead761   (501) staff       (20)        0 2023-03-28 19:56:38.362944 pyCSM-1.0.2/pyCSM/clients/
--rw-r--r--   0 blead761   (501) staff       (20)        0 2022-06-27 20:29:53.000000 pyCSM-1.0.2/pyCSM/clients/__init__.py
--rw-r--r--   0 blead761   (501) staff       (20)    17982 2023-03-28 19:52:14.000000 pyCSM-1.0.2/pyCSM/clients/hardware_client.py
--rw-r--r--   0 blead761   (501) staff       (20)    32174 2022-09-09 20:08:40.000000 pyCSM-1.0.2/pyCSM/clients/session_client.py
--rw-r--r--   0 blead761   (501) staff       (20)    22896 2023-03-28 19:52:14.000000 pyCSM-1.0.2/pyCSM/clients/system_client.py
-drwxr-xr-x   0 blead761   (501) staff       (20)        0 2023-03-28 19:56:38.363248 pyCSM-1.0.2/pyCSM/services/
--rw-r--r--   0 blead761   (501) staff       (20)        0 2022-06-27 20:29:53.000000 pyCSM-1.0.2/pyCSM/services/__init__.py
-drwxr-xr-x   0 blead761   (501) staff       (20)        0 2023-03-28 19:56:38.363565 pyCSM-1.0.2/pyCSM/services/hardware_service/
--rw-r--r--   0 blead761   (501) staff       (20)        0 2022-06-27 20:29:53.000000 pyCSM-1.0.2/pyCSM/services/hardware_service/__init__.py
--rw-r--r--   0 blead761   (501) staff       (20)    17907 2023-03-28 19:52:14.000000 pyCSM-1.0.2/pyCSM/services/hardware_service/hardware_service.py
-drwxr-xr-x   0 blead761   (501) staff       (20)        0 2023-03-28 19:56:38.364673 pyCSM-1.0.2/pyCSM/services/session_service/
--rw-r--r--   0 blead761   (501) staff       (20)        0 2022-06-27 20:29:53.000000 pyCSM-1.0.2/pyCSM/services/session_service/__init__.py
--rw-r--r--   0 blead761   (501) staff       (20)     7808 2022-09-09 20:08:40.000000 pyCSM-1.0.2/pyCSM/services/session_service/copyset_service.py
--rw-r--r--   0 blead761   (501) staff       (20)     4146 2022-09-09 20:08:40.000000 pyCSM-1.0.2/pyCSM/services/session_service/schedule_service.py
--rw-r--r--   0 blead761   (501) staff       (20)    21899 2022-09-09 20:08:40.000000 pyCSM-1.0.2/pyCSM/services/session_service/session_service.py
-drwxr-xr-x   0 blead761   (501) staff       (20)        0 2023-03-28 19:56:38.365214 pyCSM-1.0.2/pyCSM/services/system_service/
--rw-r--r--   0 blead761   (501) staff       (20)        0 2022-06-27 20:29:53.000000 pyCSM-1.0.2/pyCSM/services/system_service/__init__.py
--rw-r--r--   0 blead761   (501) staff       (20)    18706 2023-03-28 19:52:14.000000 pyCSM-1.0.2/pyCSM/services/system_service/system_service.py
-drwxr-xr-x   0 blead761   (501) staff       (20)        0 2023-03-28 19:56:38.365787 pyCSM-1.0.2/pyCSM/util/
--rw-r--r--   0 blead761   (501) staff       (20)        0 2022-09-09 20:02:33.000000 pyCSM-1.0.2/pyCSM/util/__init__.py
--rw-r--r--   0 blead761   (501) staff       (20)      675 2022-09-09 20:08:40.000000 pyCSM-1.0.2/pyCSM/util/utility.py
-drwxr-xr-x   0 blead761   (501) staff       (20)        0 2023-03-28 19:56:38.360968 pyCSM-1.0.2/pyCSM.egg-info/
--rw-r--r--   0 blead761   (501) staff       (20)      727 2023-03-28 19:56:38.000000 pyCSM-1.0.2/pyCSM.egg-info/PKG-INFO
--rw-r--r--   0 blead761   (501) staff       (20)      852 2023-03-28 19:56:38.000000 pyCSM-1.0.2/pyCSM.egg-info/SOURCES.txt
--rw-r--r--   0 blead761   (501) staff       (20)        1 2023-03-28 19:56:38.000000 pyCSM-1.0.2/pyCSM.egg-info/dependency_links.txt
--rw-r--r--   0 blead761   (501) staff       (20)       83 2023-03-28 19:56:38.000000 pyCSM-1.0.2/pyCSM.egg-info/requires.txt
--rw-r--r--   0 blead761   (501) staff       (20)       17 2023-03-28 19:56:38.000000 pyCSM-1.0.2/pyCSM.egg-info/top_level.txt
--rw-r--r--   0 blead761   (501) staff       (20)       38 2023-03-28 19:56:38.366427 pyCSM-1.0.2/setup.cfg
--rw-r--r--   0 blead761   (501) staff       (20)     1003 2023-03-28 19:51:57.000000 pyCSM-1.0.2/setup.py
+drwxr-xr-x   0 blead761   (501) staff       (20)        0 2023-07-10 15:36:13.044863 pyCSM-1.0.3/
+-rw-r--r--   0 blead761   (501) staff       (20)    11357 2022-04-11 15:23:08.000000 pyCSM-1.0.3/LICENSE
+-rw-r--r--   0 blead761   (501) staff       (20)      727 2023-07-10 15:36:13.044738 pyCSM-1.0.3/PKG-INFO
+-rw-r--r--   0 blead761   (501) staff       (20)     3808 2022-06-27 20:29:53.000000 pyCSM-1.0.3/README.md
+drwxr-xr-x   0 blead761   (501) staff       (20)        0 2023-07-10 15:36:13.039411 pyCSM-1.0.3/docs/
+-rw-r--r--   0 blead761   (501) staff       (20)        0 2022-06-27 20:29:53.000000 pyCSM-1.0.3/docs/__init__.py
+-rw-r--r--   0 blead761   (501) staff       (20)     2751 2022-06-22 19:08:15.000000 pyCSM-1.0.3/docs/conf.py
+drwxr-xr-x   0 blead761   (501) staff       (20)        0 2023-07-10 15:36:13.039600 pyCSM-1.0.3/pyCSM/
+-rw-r--r--   0 blead761   (501) staff       (20)        0 2022-06-27 20:29:53.000000 pyCSM-1.0.3/pyCSM/__init__.py
+drwxr-xr-x   0 blead761   (501) staff       (20)        0 2023-07-10 15:36:13.040540 pyCSM-1.0.3/pyCSM/authorization/
+-rw-r--r--   0 blead761   (501) staff       (20)        0 2022-06-27 20:29:53.000000 pyCSM-1.0.3/pyCSM/authorization/__init__.py
+-rw-r--r--   0 blead761   (501) staff       (20)     1854 2022-09-09 20:08:40.000000 pyCSM-1.0.3/pyCSM/authorization/auth.py
+drwxr-xr-x   0 blead761   (501) staff       (20)        0 2023-07-10 15:36:13.041855 pyCSM-1.0.3/pyCSM/clients/
+-rw-r--r--   0 blead761   (501) staff       (20)        0 2022-06-27 20:29:53.000000 pyCSM-1.0.3/pyCSM/clients/__init__.py
+-rw-r--r--   0 blead761   (501) staff       (20)    19861 2023-07-10 15:24:54.000000 pyCSM-1.0.3/pyCSM/clients/hardware_client.py
+-rw-r--r--   0 blead761   (501) staff       (20)    32174 2022-09-09 20:08:40.000000 pyCSM-1.0.3/pyCSM/clients/session_client.py
+-rw-r--r--   0 blead761   (501) staff       (20)    22896 2023-03-28 20:00:33.000000 pyCSM-1.0.3/pyCSM/clients/system_client.py
+drwxr-xr-x   0 blead761   (501) staff       (20)        0 2023-07-10 15:36:13.042250 pyCSM-1.0.3/pyCSM/services/
+-rw-r--r--   0 blead761   (501) staff       (20)        0 2022-06-27 20:29:53.000000 pyCSM-1.0.3/pyCSM/services/__init__.py
+drwxr-xr-x   0 blead761   (501) staff       (20)        0 2023-07-10 15:36:13.042548 pyCSM-1.0.3/pyCSM/services/hardware_service/
+-rw-r--r--   0 blead761   (501) staff       (20)        0 2022-06-27 20:29:53.000000 pyCSM-1.0.3/pyCSM/services/hardware_service/__init__.py
+-rw-r--r--   0 blead761   (501) staff       (20)    20245 2023-07-10 15:24:54.000000 pyCSM-1.0.3/pyCSM/services/hardware_service/hardware_service.py
+drwxr-xr-x   0 blead761   (501) staff       (20)        0 2023-07-10 15:36:13.043557 pyCSM-1.0.3/pyCSM/services/session_service/
+-rw-r--r--   0 blead761   (501) staff       (20)        0 2022-06-27 20:29:53.000000 pyCSM-1.0.3/pyCSM/services/session_service/__init__.py
+-rw-r--r--   0 blead761   (501) staff       (20)     7808 2022-09-09 20:08:40.000000 pyCSM-1.0.3/pyCSM/services/session_service/copyset_service.py
+-rw-r--r--   0 blead761   (501) staff       (20)     4146 2022-09-09 20:08:40.000000 pyCSM-1.0.3/pyCSM/services/session_service/schedule_service.py
+-rw-r--r--   0 blead761   (501) staff       (20)    21899 2022-09-09 20:08:40.000000 pyCSM-1.0.3/pyCSM/services/session_service/session_service.py
+drwxr-xr-x   0 blead761   (501) staff       (20)        0 2023-07-10 15:36:13.043906 pyCSM-1.0.3/pyCSM/services/system_service/
+-rw-r--r--   0 blead761   (501) staff       (20)        0 2022-06-27 20:29:53.000000 pyCSM-1.0.3/pyCSM/services/system_service/__init__.py
+-rw-r--r--   0 blead761   (501) staff       (20)    18706 2023-03-28 20:00:33.000000 pyCSM-1.0.3/pyCSM/services/system_service/system_service.py
+drwxr-xr-x   0 blead761   (501) staff       (20)        0 2023-07-10 15:36:13.044420 pyCSM-1.0.3/pyCSM/util/
+-rw-r--r--   0 blead761   (501) staff       (20)        0 2022-09-09 20:02:33.000000 pyCSM-1.0.3/pyCSM/util/__init__.py
+-rw-r--r--   0 blead761   (501) staff       (20)      675 2022-09-09 20:08:40.000000 pyCSM-1.0.3/pyCSM/util/utility.py
+drwxr-xr-x   0 blead761   (501) staff       (20)        0 2023-07-10 15:36:13.040271 pyCSM-1.0.3/pyCSM.egg-info/
+-rw-r--r--   0 blead761   (501) staff       (20)      727 2023-07-10 15:36:13.000000 pyCSM-1.0.3/pyCSM.egg-info/PKG-INFO
+-rw-r--r--   0 blead761   (501) staff       (20)      852 2023-07-10 15:36:13.000000 pyCSM-1.0.3/pyCSM.egg-info/SOURCES.txt
+-rw-r--r--   0 blead761   (501) staff       (20)        1 2023-07-10 15:36:13.000000 pyCSM-1.0.3/pyCSM.egg-info/dependency_links.txt
+-rw-r--r--   0 blead761   (501) staff       (20)       83 2023-07-10 15:36:13.000000 pyCSM-1.0.3/pyCSM.egg-info/requires.txt
+-rw-r--r--   0 blead761   (501) staff       (20)       17 2023-07-10 15:36:13.000000 pyCSM-1.0.3/pyCSM.egg-info/top_level.txt
+-rw-r--r--   0 blead761   (501) staff       (20)       38 2023-07-10 15:36:13.044909 pyCSM-1.0.3/setup.cfg
+-rw-r--r--   0 blead761   (501) staff       (20)     1003 2023-07-10 15:32:27.000000 pyCSM-1.0.3/setup.py
```

### Comparing `pyCSM-1.0.2/LICENSE` & `pyCSM-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyCSM-1.0.2/README.md` & `pyCSM-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyCSM-1.0.2/docs/conf.py` & `pyCSM-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyCSM-1.0.2/pyCSM/authorization/auth.py` & `pyCSM-1.0.3/pyCSM/authorization/auth.py`

 * *Files identical despite different names*

### Comparing `pyCSM-1.0.2/pyCSM/clients/hardware_client.py` & `pyCSM-1.0.3/pyCSM/clients/hardware_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -359,14 +359,44 @@
                                              password, username, host_port)
         if resp.status_code == 401:
             self.tk = auth.get_token(self.base_url, self.username, self.password)
             return hardware_service.add_zos_host(self.base_url, self.tk, host_ip,
                                                  password, username, host_port)
         return resp
 
+
+    def get_zos_candidate(self):
+        """
+        This method will query for the devices in REST that are attached to the zos system
+
+        Returns:
+            JSON String representing the result of the command.
+            'I' = successful, 'W' = warning, 'E' = error.
+        """
+        resp = hardware_service.get_zos_candidate(self.base_url, self.tk)
+        if resp.status_code == 401:
+            self.tk = auth.get_token(self.base_url, self.username, self.password)
+            return hardware_service.get_zos_candidate(self.base_url, self.tk)
+        return resp
+
+    def get_zos_host(self):
+        """
+        This method will get the information for all zos host connections.
+
+        Returns:
+            JSON String representing the result of the command.
+            'I' = successful, 'W' = warning, 'E' = error.
+        """
+        resp = hardware_service.get_zos_host(self.base_url, self.tk)
+        if resp.status_code == 401:
+            self.tk = auth.get_token(self.base_url, self.username, self.password)
+            return hardware_service.get_zos_host(self.base_url, self.tk)
+        return resp
+
+
     def remove_zos_host(self, host_ip, host_port):
         """
         This method will create a zos connection to the current IP
 
         Args:
             host_ip (str): Primary IP address for the zos system.
             host_port (str): Port for the zos system
@@ -379,14 +409,35 @@
                                                 host_port)
         if resp.status_code == 401:
             self.tk = auth.get_token(self.base_url, self.username, self.password)
             return hardware_service.remove_zos_host(self.base_url, self.tk, host_ip,
                                                     host_port)
         return resp
 
+
+    def add_zos_device(self, device_id):
+        """
+        This method will add a storage system through the zoshost connection.
+
+        Args:
+            device_id (str): Storage system name in the format "DS8000:BOX:2107.KXZ91".
+            connection_type (str): type of connection
+
+        Returns:
+            JSON String representing the result of the command.
+            'I' = successful, 'W' = warning, 'E' = error.
+        """
+        resp = hardware_service.add_zos_device(self.base_url, self.tk, device_id)
+        if resp.status_code == 401:
+            self.tk = auth.get_token(self.base_url, self.username, self.password)
+            return hardware_service.add_zos_device(self.base_url, self.tk, device_id)
+        return resp
+
+
+
     def get_volumes_by_wwn(self, wwn_name):
         """
         Return the information for all volumes based on the list of WWNs passed in.
 
         Args:
             wwn_name (str): The volume wwn you would like to query or a subset of the volume wwn for a volume list
```

### Comparing `pyCSM-1.0.2/pyCSM/clients/session_client.py` & `pyCSM-1.0.3/pyCSM/clients/session_client.py`

 * *Files identical despite different names*

### Comparing `pyCSM-1.0.2/pyCSM/clients/system_client.py` & `pyCSM-1.0.3/pyCSM/clients/system_client.py`

 * *Files identical despite different names*

### Comparing `pyCSM-1.0.2/pyCSM/services/hardware_service/hardware_service.py` & `pyCSM-1.0.3/pyCSM/services/hardware_service/hardware_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -405,14 +405,42 @@
         "deviceusername": device_username,
         "name": connection_name
     }
 
     return requests.put(put_url, headers=headers, data=params, verify=properties["verify"], cert=properties["cert"])
 
 
+
+def get_zos_candidate(url, tk):
+    """
+    This method will query for the devices in REST that are attached to the zos system.
+
+    Args:
+        url (str): Base url of CSM server. ex. https://servername:port/CSM/web.
+        tk (str): Rest token for the CSM server.
+
+    Returns:
+        JSON String representing the result of the command.
+        'I' = successful, 'W' = warning, 'E' = error.
+    """
+    get_url = f"{url}/storagedevices/zoscandidate"
+    headers = {
+        "Accept-Language": properties["language"],
+        "X-Auth-Token": str(tk),
+        "Content-Type": "application/x-www-form-urlencoded"
+    }
+
+    params = {
+    }
+
+    return requests.get(get_url, headers=headers, data=params, verify=properties["verify"], cert=properties["cert"])
+
+
+
+
 def add_zos_host(url, tk, host_ip, password, username, host_port):
     """
     This method will create a zos connection to the current IP
 
     Args:
         url (str): Base url of CSM server. ex. https://servername:port/CSM/web.
         tk (str): Rest token for the CSM server.
@@ -468,14 +496,65 @@
         "hostport": host_port
     }
 
     return requests.delete(delete_url, headers=headers, data=params, verify=properties["verify"], cert=properties["cert"])
 
 
 
+
+def add_zos_device(url, tk, device_id):
+    """
+    This method will add a storage system through the zoshost connection.
+
+    Args:
+        url (str): Base url of CSM server. ex. https://servername:port/CSM/web.
+        tk (str): Rest token for the CSM server.
+        device_id (str): Storage system name in the format "DS8000:BOX:2107.KXZ91".
+
+    Returns:
+        JSON String representing the result of the command.
+        'I' = successful, 'W' = warning, 'E' = error.
+    """
+    put_url = f"{url}/storagedevices/zosdevice"
+    headers = {
+        "Accept-Language": properties["language"],
+        "X-Auth-Token": str(tk),
+        "Content-Type": "application/x-www-form-urlencoded"
+    }
+
+    params = {
+        "deviceid": device_id
+    }
+
+    return requests.put(put_url, headers=headers, data=params, verify=properties["verify"], cert=properties["cert"])
+
+
+def get_zos_host(url, tk):
+    """
+    This method will get the information for all zos host connections.
+
+    Args:
+        url (str): Base url of CSM server. ex. https://servername:port/CSM/web.
+        tk (str): Rest token for the CSM server.
+
+    Returns:
+        JSON String representing the result of the command.
+        'I' = successful, 'W' = warning, 'E' = error.
+    """
+    get_url = f"{url}/storagedevices/zoshost"
+    headers = {
+        "Accept-Language": properties["language"],
+        "X-Auth-Token": str(tk),
+        "Content-Type": "application/x-www-form-urlencoded"
+    }
+    return requests.get(get_url, headers=headers,  verify=properties["verify"], cert=properties["cert"])
+
+
+
+
 def get_volumes_by_wwn(url, tk, wwn_name):
     """
     Return the information for all volumes based on the list of WWNs passed in.
 
     Args:
         url (str): Base url of CSM server. ex. https://servername:port/CSM/web.
         tk (str): Rest token for the CSM server.
```

### Comparing `pyCSM-1.0.2/pyCSM/services/session_service/copyset_service.py` & `pyCSM-1.0.3/pyCSM/services/session_service/copyset_service.py`

 * *Files identical despite different names*

### Comparing `pyCSM-1.0.2/pyCSM/services/session_service/schedule_service.py` & `pyCSM-1.0.3/pyCSM/services/session_service/schedule_service.py`

 * *Files identical despite different names*

### Comparing `pyCSM-1.0.2/pyCSM/services/session_service/session_service.py` & `pyCSM-1.0.3/pyCSM/services/session_service/session_service.py`

 * *Files identical despite different names*

### Comparing `pyCSM-1.0.2/pyCSM/services/system_service/system_service.py` & `pyCSM-1.0.3/pyCSM/services/system_service/system_service.py`

 * *Files identical despite different names*

### Comparing `pyCSM-1.0.2/pyCSM/util/utility.py` & `pyCSM-1.0.3/pyCSM/util/utility.py`

 * *Files identical despite different names*

### Comparing `pyCSM-1.0.2/pyCSM.egg-info/SOURCES.txt` & `pyCSM-1.0.3/pyCSM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyCSM-1.0.2/setup.py` & `pyCSM-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     install_requires = f.read().splitlines()
 
 setup(
     name='pyCSM',
     description="CSM Python Client",
     long_description="CSM RESTful API Python Client.",
     author="Dominic Blea",
-    version='1.0.2',
+    version='1.0.3',
     author_email="dblea00@ibm.com",
     maintainer="Dominic Blea",
     keywords=["IBM", "CSM Storage"],
     install_requires=install_requires,
     license="Apache License, Version 2.0",
     include_package_data=True,
     packages=find_packages(),
```


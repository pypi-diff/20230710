# Comparing `tmp/ntdsdotsqlite-1.0.0.tar.gz` & `tmp/ntdsdotsqlite-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntdsdotsqlite-1.0.0.tar", max compression
+gzip compressed data, was "ntdsdotsqlite-1.1.1.tar", max compression
```

## Comparing `ntdsdotsqlite-1.0.0.tar` & `ntdsdotsqlite-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2023-04-24 19:34:15.811658 ntdsdotsqlite-1.0.0/ntdsdotsqlite/__init__.py
--rw-r--r--   0        0        0      852 2023-07-08 21:57:45.406401 ntdsdotsqlite-1.0.0/ntdsdotsqlite/__main__.py
--rw-r--r--   0        0        0      389 2023-07-05 17:21:18.207904 ntdsdotsqlite-1.0.0/ntdsdotsqlite/basehandler.py
--rw-r--r--   0        0        0     5536 2023-07-08 21:41:52.675922 ntdsdotsqlite-1.0.0/ntdsdotsqlite/computerhandler.py
--rw-r--r--   0        0        0     2117 2023-07-08 19:51:20.130174 ntdsdotsqlite-1.0.0/ntdsdotsqlite/containerhandler.py
--rw-r--r--   0        0        0     4145 2023-05-06 15:44:55.688794 ntdsdotsqlite-1.0.0/ntdsdotsqlite/decrypt.py
--rw-r--r--   0        0        0     4508 2023-07-07 17:30:48.617916 ntdsdotsqlite-1.0.0/ntdsdotsqlite/domainhandler.py
--rw-r--r--   0        0        0     1788 2023-07-05 20:40:04.710251 ntdsdotsqlite-1.0.0/ntdsdotsqlite/grouphandler.py
--rw-r--r--   0        0        0     2951 2023-07-08 21:49:06.058097 ntdsdotsqlite-1.0.0/ntdsdotsqlite/model.sql
--rw-r--r--   0        0        0     5839 2023-07-08 22:19:51.689577 ntdsdotsqlite-1.0.0/ntdsdotsqlite/ntdsdotsqlite.py
--rw-r--r--   0        0        0     2107 2023-07-08 20:19:52.784084 ntdsdotsqlite-1.0.0/ntdsdotsqlite/organizationalunithandler.py
--rw-r--r--   0        0        0     5894 2023-07-08 21:37:05.683105 ntdsdotsqlite-1.0.0/ntdsdotsqlite/personhandler.py
--rw-r--r--   0        0        0    26948 2023-07-05 17:06:07.989661 ntdsdotsqlite-1.0.0/ntdsdotsqlite/secretsdump.py
--rw-r--r--   0        0        0     2076 2023-07-06 20:00:49.679037 ntdsdotsqlite-1.0.0/ntdsdotsqlite/trusteddomainhandler.py
--rw-r--r--   0        0        0     3678 2023-07-08 22:04:51.106889 ntdsdotsqlite-1.0.0/ntdsdotsqlite/utils.py
--rw-r--r--   0        0        0      713 2023-07-08 22:16:21.344278 ntdsdotsqlite-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2005 2023-05-08 16:12:51.277756 ntdsdotsqlite-1.0.0/README.md
--rw-r--r--   0        0        0     2813 1970-01-01 00:00:00.000000 ntdsdotsqlite-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-10 06:29:54.935247 ntdsdotsqlite-1.1.1/ntdsdotsqlite/__init__.py
+-rw-r--r--   0        0        0      821 2023-07-10 06:29:54.935247 ntdsdotsqlite-1.1.1/ntdsdotsqlite/__main__.py
+-rw-r--r--   0        0        0      376 2023-07-10 06:29:54.935247 ntdsdotsqlite-1.1.1/ntdsdotsqlite/basehandler.py
+-rw-r--r--   0        0        0     7755 2023-07-10 06:36:05.781938 ntdsdotsqlite-1.1.1/ntdsdotsqlite/computerhandler.py
+-rw-r--r--   0        0        0     2066 2023-07-10 06:29:54.936247 ntdsdotsqlite-1.1.1/ntdsdotsqlite/containerhandler.py
+-rw-r--r--   0        0        0    10571 2023-07-10 06:44:44.229932 ntdsdotsqlite-1.1.1/ntdsdotsqlite/decrypt.py
+-rw-r--r--   0        0        0     6847 2023-07-10 06:29:54.937247 ntdsdotsqlite-1.1.1/ntdsdotsqlite/domainhandler.py
+-rw-r--r--   0        0        0     1743 2023-07-10 06:29:54.937913 ntdsdotsqlite-1.1.1/ntdsdotsqlite/grouphandler.py
+-rw-r--r--   0        0        0     3279 2023-07-10 06:29:54.938417 ntdsdotsqlite-1.1.1/ntdsdotsqlite/model.sql
+-rw-r--r--   0        0        0     5733 2023-07-10 06:46:22.669573 ntdsdotsqlite-1.1.1/ntdsdotsqlite/ntdsdotsqlite.py
+-rw-r--r--   0        0        0     2054 2023-07-10 06:29:54.938417 ntdsdotsqlite-1.1.1/ntdsdotsqlite/organizationalunithandler.py
+-rw-r--r--   0        0        0     8022 2023-07-10 06:36:02.910641 ntdsdotsqlite-1.1.1/ntdsdotsqlite/personhandler.py
+-rw-r--r--   0        0        0     2022 2023-07-10 06:29:54.939050 ntdsdotsqlite-1.1.1/ntdsdotsqlite/trusteddomainhandler.py
+-rw-r--r--   0        0        0     3561 2023-07-10 06:29:54.939050 ntdsdotsqlite-1.1.1/ntdsdotsqlite/utils.py
+-rw-r--r--   0        0        0      691 2023-07-10 07:11:25.333467 ntdsdotsqlite-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1494 2023-07-10 06:29:54.934246 ntdsdotsqlite-1.1.1/README.md
+-rw-r--r--   0        0        0     2400 1970-01-01 00:00:00.000000 ntdsdotsqlite-1.1.1/setup.py
+-rw-r--r--   0        0        0     2337 1970-01-01 00:00:00.000000 ntdsdotsqlite-1.1.1/PKG-INFO
```

### Comparing `ntdsdotsqlite-1.0.0/ntdsdotsqlite/__main__.py` & `ntdsdotsqlite-1.1.1/ntdsdotsqlite/__main__.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from pathlib import Path
-import argparse
-
-from ntdsdotsqlite.ntdsdotsqlite import run
-
-
-def main():
-    parser = argparse.ArgumentParser(
-        prog="NTDS.sqlite",
-        description=(
-            "This tool helps dumping NTDS.DIT file to an SQLite database"
-        )
-    )
-    parser.add_argument("NTDS", help="The NTDS.DIT file", type=Path)
-    parser.add_argument(
-        "--system", required=False,
-        help=(
-            "The SYSTEM hive to decrypt hashes. If not provided, hashes will "
-            "be encrypted inside the sqlite database."
-        )
-    )
-    parser.add_argument(
-        "-o", "--outfile", required=True,
-        help="The sqlite database. Example : NTDS.sqlite"
-    )
-    args = parser.parse_args()
-    run(args.NTDS, args.outfile, args.system)
-
-
-if __name__ == "__main__":
-    main()
+from pathlib import Path
+import argparse
+
+from ntdsdotsqlite.ntdsdotsqlite import run
+
+
+def main():
+    parser = argparse.ArgumentParser(
+        prog="NTDS.sqlite",
+        description=(
+            "This tool helps dumping NTDS.DIT file to an SQLite database"
+        )
+    )
+    parser.add_argument("NTDS", help="The NTDS.DIT file", type=Path)
+    parser.add_argument(
+        "--system", required=False,
+        help=(
+            "The SYSTEM hive to decrypt hashes. If not provided, hashes will "
+            "be encrypted inside the sqlite database."
+        )
+    )
+    parser.add_argument(
+        "-o", "--outfile", required=True,
+        help="The sqlite database. Example : NTDS.sqlite"
+    )
+    args = parser.parse_args()
+    run(args.NTDS, args.outfile, args.system)
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `ntdsdotsqlite-1.0.0/ntdsdotsqlite/containerhandler.py` & `ntdsdotsqlite-1.1.1/ntdsdotsqlite/containerhandler.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from ntdsdotsqlite.basehandler import BaseHandler
-from ntdsdotsqlite.utils import escape_dn_chars
-
-
-class ContainerHandler(BaseHandler):
-    def handle(self, row):
-        container = {
-            "id": row.get("DNT_col"),
-            "name": row.get(self.attributes["name"]),
-            "cn": row.get(self.attributes["cn"]),
-            "description": row.get(self.attributes["description"]),
-            "parent": row.get("PDNT_col"),
-            "is_deleted": row.get(self.attributes["isDeleted"]) == 1
-        }
-        stmt = """
-            INSERT INTO containers VALUES (
-            :id, :name, :description, :cn, :parent, Null, :is_deleted
-            )
-        """
-        self.sqlite_db.execute(stmt, container)
-
-    def callback(self):
-        # compute DNs
-        roots = {domain_id: domain_DN for domain_id, domain_DN in self.sqlite_db.execute(
-            "SELECT id, dn FROM domain_dns"
-        ).fetchall()}
-        containers = {
-            c_id: {"id": c_id, "name": name, "parent": parent, "cn": cn}
-            for c_id, name, parent, cn in self.sqlite_db.execute(
-                "SELECT id, name, parent, commonname FROM containers"
-            ).fetchall()
-        }
-        for container in containers.values():
-            cur_object = container
-            parts = [f"CN={escape_dn_chars(cur_object['cn'])}"]
-            while True:
-                if cur_object["parent"] in containers.keys():
-                    cur_object = containers[cur_object["parent"]]
-                    parts.append(f"CN={escape_dn_chars(cur_object['cn'])}")
-                elif cur_object["parent"] in roots.keys():
-                    parts.append(roots[cur_object["parent"]])
-                    break
-                else:
-                    break
-            container["dn"] = ",".join(parts)
-            if ",DC=" not in container["dn"]:
-                container["dn"] = ""
-            self.sqlite_db.execute(
-                "UPDATE containers SET dn=? WHERE id=?", (container["dn"], container["id"])
-            )
-        self.sqlite_db.commit()
+from ntdsdotsqlite.basehandler import BaseHandler
+from ntdsdotsqlite.utils import escape_dn_chars
+
+
+class ContainerHandler(BaseHandler):
+    def handle(self, row):
+        container = {
+            "id": row.get("DNT_col"),
+            "name": row.get(self.attributes["name"]),
+            "cn": row.get(self.attributes["cn"]),
+            "description": row.get(self.attributes["description"]),
+            "parent": row.get("PDNT_col"),
+            "is_deleted": row.get(self.attributes["isDeleted"]) == 1
+        }
+        stmt = """
+            INSERT INTO containers VALUES (
+            :id, :name, :description, :cn, :parent, Null, :is_deleted
+            )
+        """
+        self.sqlite_db.execute(stmt, container)
+
+    def callback(self):
+        # compute DNs
+        roots = {domain_id: domain_DN for domain_id, domain_DN in self.sqlite_db.execute(
+            "SELECT id, dn FROM domain_dns"
+        ).fetchall()}
+        containers = {
+            c_id: {"id": c_id, "name": name, "parent": parent, "cn": cn}
+            for c_id, name, parent, cn in self.sqlite_db.execute(
+                "SELECT id, name, parent, commonname FROM containers"
+            ).fetchall()
+        }
+        for container in containers.values():
+            cur_object = container
+            parts = [f"CN={escape_dn_chars(cur_object['cn'])}"]
+            while True:
+                if cur_object["parent"] in containers.keys():
+                    cur_object = containers[cur_object["parent"]]
+                    parts.append(f"CN={escape_dn_chars(cur_object['cn'])}")
+                elif cur_object["parent"] in roots.keys():
+                    parts.append(roots[cur_object["parent"]])
+                    break
+                else:
+                    break
+            container["dn"] = ",".join(parts)
+            if ",DC=" not in container["dn"]:
+                container["dn"] = ""
+            self.sqlite_db.execute(
+                "UPDATE containers SET dn=? WHERE id=?", (container["dn"], container["id"])
+            )
+        self.sqlite_db.commit()
```

### Comparing `ntdsdotsqlite-1.0.0/ntdsdotsqlite/model.sql` & `ntdsdotsqlite-1.1.1/ntdsdotsqlite/model.sql`

 * *Files 10% similar despite different names*

```diff
@@ -23,33 +23,38 @@
     gplink TEXT,
     SID TEXT,
     dn TEXT
 );
 
 CREATE TABLE user_accounts (
     id INTEGER PRIMARY KEY,
-    nthash BLOB,
-    lmhash BLOB,
+    encrypted_nthash BLOB,
+    nthash TEXT,
+    encrypted_lmhash BLOB,
+    lmhash TEXT,
     UAC INTEGER,
     description TEXT,
     lastLogonTimestamp INTEGER,
     pwdlastset INTEGER,
     admincount INTEGER,
     displayName TEXT,
     GUID TEXT,
     SID TEXT,
     SPN JSON,
     domain INTEGER,
     UPN TEXT,
     login TEXT,
     samaccountname TEXT,
     commonname TEXT,
-    supplementalCredentials BLOB,
-    lmPwdHistory BLOB,
-    ntPwdHistory BLOB,
+    encrypted_supplementalCredentials BLOB,
+    supplementalCredentials JSON,
+    encrypted_lmPwdHistory BLOB,
+    lmPwdHistory JSON,
+    encrypted_ntPwdHistory BLOB,
+    ntPwdHistory JSON,
     accountExpires INTEGER,
     UAC_flags JSON,
     parent_OU INTEGER,
     dn TEXT,
     isDeleted BOOLEAN,
     primaryGroup INTEGER,
     memberOf JSON,
@@ -70,33 +75,38 @@
     description TEXT,
     memberOf JSON,
     FOREIGN KEY (id) REFERENCES domains (domain)
 );
 
 CREATE TABLE machine_accounts (
     id INTEGER PRIMARY KEY,
-    nthash BLOB,
-    lmhash BLOB,
+    encrypted_nthash BLOB,
+    nthash TEXT,
+    encrypted_lmhash BLOB,
+    lmhash TEXT,
     UAC INTEGER,
     description TEXT,
     lastLogonTimestamp INTEGER,
     pwdlastset INTEGER,
     admincount INTEGER,
     displayName TEXT,
     GUID TEXT,
     SID TEXT,
     SPN JSON,
     domain INTEGER,
     UPN TEXT,
     login TEXT,
     samaccountname TEXT,
     commonname TEXT,
-    supplementalCredentials BLOB,
-    lmPwdHistory BLOB,
-    ntPwdHistory BLOB,
+    encrypted_supplementalCredentials BLOB,
+    supplementalCredentials JSON,
+    encrypted_lmPwdHistory BLOB,
+    lmPwdHistory JSON,
+    encrypted_ntPwdHistory BLOB,
+    ntPwdHistory JSON,
     accountExpires TEXT,
     UAC_flags JSON,
     parent_OU INTEGER,
     dn TEXT,
     isDeleted BOOLEAN,
     primaryGroup INTEGER,
     isDisabled BOOLEAN,
```

### Comparing `ntdsdotsqlite-1.0.0/ntdsdotsqlite/ntdsdotsqlite.py` & `ntdsdotsqlite-1.1.1/ntdsdotsqlite/ntdsdotsqlite.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-from ntdsdotsqlite.organizationalunithandler import OrganizationalUnitHandler
-from ntdsdotsqlite.trusteddomainhandler import TrustedDomainHandler
-from ntdsdotsqlite.utils import create_database, compute_links
-from ntdsdotsqlite.containerhandler import ContainerHandler
-from ntdsdotsqlite.computerhandler import ComputerHandler
-from ntdsdotsqlite.personhandler import PersonHandler
-from ntdsdotsqlite.domainhandler import DomainHandler
-from ntdsdotsqlite.grouphandler import GroupHandler
-from ntdsdotsqlite.decrypt import decrypt_sqlite
-from collections import OrderedDict
-from dissect.esedb import EseDB
-from tqdm import tqdm
-import sqlite3
-import re
-
-
-def run(ese_path, outpath, system_path):
-    create_database(outpath)
-    sqlite_db = sqlite3.connect(outpath)
-    fd = open(ese_path, "rb")
-    ese_db = EseDB(fd)
-    # Getting column names and base initialization stuff
-    attribute_dnt = None
-    class_dnt = None
-    # attributes_raw : {131532: "ATTm131532"}
-    attributes_raw = {}
-    # attributes: {"displayName": "ATTm131532"}
-    attributes = {}
-    # classes: {"person": 1511}
-    classes = {}
-    link_relations = compute_links(ese_db)
-    # each class instance here are used to handle the addition of new objects in the sqlite
-    # these classes should have a handle(row) method and a callback() method. They are instantiated
-    # with the sqlite_db handle and the colnames dictionary. handle(row) is called live when a row
-    # is caught with the class set in key of this dictionary, the callback method is called after
-    # the ntds has been read entirely.
-    # This dict can be ordered to choose in which order the callbacks will be called !
-    caught_classes = OrderedDict({
-        "domainDNS": DomainHandler(sqlite_db, attributes, ese_db),
-        "trustedDomain": TrustedDomainHandler(sqlite_db, attributes, ese_db),
-        "group": GroupHandler(link_relations, sqlite_db, attributes, ese_db),
-        "container": ContainerHandler(sqlite_db, attributes, ese_db),
-        "organizationalUnit": OrganizationalUnitHandler(sqlite_db, attributes, ese_db),
-        "person": PersonHandler(link_relations, sqlite_db, attributes, ese_db),
-        "computer": ComputerHandler(sqlite_db, attributes, ese_db)
-    })
-    # "direct access" classes : {1511: SpecificHandler(...)}
-    da_classes = {}
-    attributeID_attr = "ATTc131102"
-    schemaGuid_attr = "ATTk589972"
-    lDAPDisplayName_attr = "ATTm131532"
-    objectCategory_attr = "ATTb590606"
-    attributeSchema_sguid = b"\x80\x7a\x96\xbf\xe6\x0d\xd0\x11\xa2\x85\x00\xaa\x00\x30\x49\xe2"
-    classSchema_sguid = b"\x83\x7a\x96\xbf\xe6\x0d\xd0\x11\xa2\x85\x00\xaa\x00\x30\x49\xe2"
-    d_reg = re.compile(r"(\d+$)")
-    msysobjects = ese_db.table("MSysObjects")
-    for row in msysobjects.records():
-        if (name := row.Name).startswith('ATT'):
-            res = d_reg.search(name)
-            attributes_raw[name[res.start():]] = name
-    datatable = ese_db.table("datatable")
-    cnt = 0
-    for row in datatable.records():
-        cnt += 1
-    datatable = ese_db.table("datatable")
-    for row in datatable.records():
-        sguid = row.get(schemaGuid_attr)
-        if sguid is not None and sguid == attributeSchema_sguid:
-            attribute_dnt = row.get("DNT_col")
-        if sguid is not None and sguid == classSchema_sguid:
-            class_dnt = row.get("DNT_col")
-        if attribute_dnt is not None and class_dnt is not None:
-            break
-    tmp_rows = []
-    store_tmp = True
-    for row in tqdm(datatable.records(), total=cnt):
-        obj_category = row.get(objectCategory_attr)
-        # if the row is an attribute name :
-        if obj_category == attribute_dnt:
-            try:
-                # match it with its value/raw name in msysobject and store it for later
-                attributes[row.get(lDAPDisplayName_attr)] = (
-                    attributes_raw[str(row.get(attributeID_attr))]
-                )
-            except KeyError:
-                # Here an "AttributeSchema" object has been seen with an attributeID which is not
-                # in the MSYSobjects table...
-                pass
-        # if the row is a class name :
-        if obj_category == class_dnt:
-            # store its DNT to use it later and match it against objectCategory attribute
-            class_name = row.get(lDAPDisplayName_attr)
-            dnt = row.get("DNT_col")
-            classes[class_name] = dnt
-            # if this class happens to be in the caught classes list, we keep a secondary
-            # index for later use with O(1) instead of O(len(caught_classes.keys()))
-            if class_name in caught_classes.keys():
-                da_classes[dnt] = caught_classes[class_name]
-                if len(da_classes.keys()) == len(caught_classes.keys()):
-                    store_tmp = False
-        # trigger the handle method of the associated handler if it exists
-        try:
-            da_classes[obj_category].handle(row)
-        except KeyError:
-            if store_tmp:
-                tmp_rows.append(row)
-    # manage the first "few" rows we saw when classes and attributes were not set up yet
-    for row in filter(lambda r: r.get(attributes["objectCategory"]) in da_classes.keys(), tmp_rows):
-        obj_category = row.get(objectCategory_attr)
-        da_classes[obj_category].handle(row)
-    sqlite_db.commit()
-    # Trigger callbacks for all caught classes
-    for _, obj in caught_classes.items():
-        obj.callback()
-        sqlite_db.commit()
-    # Decrypt stuff if system hive provided
-    if system_path:
-        print("Decrypting stuff with SYSTEM hive ...")
-        decrypt_sqlite(sqlite_db, ese_path, system_path)
-    if sqlite_db:
-        sqlite_db.close()
-    fd.close()
+from ntdsdotsqlite.organizationalunithandler import OrganizationalUnitHandler
+from ntdsdotsqlite.trusteddomainhandler import TrustedDomainHandler
+from ntdsdotsqlite.utils import create_database, compute_links
+from ntdsdotsqlite.containerhandler import ContainerHandler
+from ntdsdotsqlite.computerhandler import ComputerHandler
+from ntdsdotsqlite.personhandler import PersonHandler
+from ntdsdotsqlite.domainhandler import DomainHandler
+from ntdsdotsqlite.grouphandler import GroupHandler
+from ntdsdotsqlite.decrypt import getBootKey
+from collections import OrderedDict
+from dissect.esedb import EseDB
+from tqdm import tqdm
+import sqlite3
+import re
+
+
+def run(ese_path, outpath, system_path, quiet=False):
+    create_database(outpath)
+    sqlite_db = sqlite3.connect(outpath)
+    fd = open(ese_path, "rb")
+    ese_db = EseDB(fd)
+    # Getting column names and base initialization stuff
+    attribute_dnt = None
+    class_dnt = None
+    # attributes_raw : {131532: "ATTm131532"}
+    attributes_raw = {}
+    # attributes: {"displayName": "ATTm131532"}
+    attributes = {}
+    # classes: {"person": 1511}
+    classes = {}
+    link_relations = compute_links(ese_db)
+    # catch the bootkey in the SYSTEM hive if any
+    bootkey = getBootKey(system_path) if system_path else None
+    # each class instance here are used to handle the addition of new objects in the sqlite
+    # these classes should have a handle(row) method and a callback() method. They are instantiated
+    # with the sqlite_db handle and the colnames dictionary. handle(row) is called live when a row
+    # is caught with the class set in key of this dictionary, the callback method is called after
+    # the ntds has been read entirely.
+    # This dict can be ordered to choose in which order the callbacks will be called !
+    dh = DomainHandler(sqlite_db, attributes, ese_db, bootkey)
+    caught_classes = OrderedDict({
+        "domainDNS": dh,
+        "trustedDomain": TrustedDomainHandler(sqlite_db, attributes, ese_db),
+        "group": GroupHandler(link_relations, sqlite_db, attributes, ese_db),
+        "container": ContainerHandler(sqlite_db, attributes, ese_db),
+        "organizationalUnit": OrganizationalUnitHandler(sqlite_db, attributes, ese_db),
+        "person": PersonHandler(link_relations, sqlite_db, attributes, ese_db, dh),
+        "computer": ComputerHandler(sqlite_db, attributes, ese_db, dh)
+    })
+    # "direct access" classes : {1511: SpecificHandler(...)}
+    da_classes = {}
+    attributeID_attr = "ATTc131102"
+    schemaGuid_attr = "ATTk589972"
+    lDAPDisplayName_attr = "ATTm131532"
+    objectCategory_attr = "ATTb590606"
+    attributeSchema_sguid = b"\x80\x7a\x96\xbf\xe6\x0d\xd0\x11\xa2\x85\x00\xaa\x00\x30\x49\xe2"
+    classSchema_sguid = b"\x83\x7a\x96\xbf\xe6\x0d\xd0\x11\xa2\x85\x00\xaa\x00\x30\x49\xe2"
+    d_reg = re.compile(r"(\d+$)")
+    msysobjects = ese_db.table("MSysObjects")
+    for row in msysobjects.records():
+        if (name := row.Name).startswith('ATT'):
+            res = d_reg.search(name)
+            attributes_raw[name[res.start():]] = name
+    datatable = ese_db.table("datatable")
+    cnt = 0
+    for row in datatable.records():
+        cnt += 1
+    datatable = ese_db.table("datatable")
+    for row in datatable.records():
+        sguid = row.get(schemaGuid_attr)
+        if sguid is not None and sguid == attributeSchema_sguid:
+            attribute_dnt = row.get("DNT_col")
+        if sguid is not None and sguid == classSchema_sguid:
+            class_dnt = row.get("DNT_col")
+        if attribute_dnt is not None and class_dnt is not None:
+            break
+    tmp_rows = []
+
+    store_tmp = True
+    for row in (tqdm(datatable.records(), total=cnt) if not quiet else datatable.records()):
+        obj_category = row.get(objectCategory_attr)
+        # if the row is an attribute name :
+        if obj_category == attribute_dnt:
+            try:
+                # match it with its value/raw name in msysobject and store it for later
+                attributes[row.get(lDAPDisplayName_attr)] = (
+                    attributes_raw[str(row.get(attributeID_attr))]
+                )
+            except KeyError:
+                # Here an "AttributeSchema" object has been seen with an attributeID which is not
+                # in the MSYSobjects table...
+                pass
+        # if the row is a class name :
+        if obj_category == class_dnt:
+            # store its DNT to use it later and match it against objectCategory attribute
+            class_name = row.get(lDAPDisplayName_attr)
+            dnt = row.get("DNT_col")
+            classes[class_name] = dnt
+            # if this class happens to be in the caught classes list, we keep a secondary
+            # index for later use with O(1) instead of O(len(caught_classes.keys()))
+            if class_name in caught_classes.keys():
+                da_classes[dnt] = caught_classes[class_name]
+                if len(da_classes.keys()) == len(caught_classes.keys()):
+                    store_tmp = False
+        # trigger the handle method of the associated handler if it exists
+        try:
+            da_classes[obj_category].handle(row)
+        except KeyError:
+            if store_tmp:
+                tmp_rows.append(row)
+    # manage the first "few" rows we saw when classes and attributes were not set up yet
+    for row in filter(lambda r: r.get(attributes["objectCategory"]) in da_classes.keys(), tmp_rows):
+        obj_category = row.get(objectCategory_attr)
+        da_classes[obj_category].handle(row)
+    sqlite_db.commit()
+    # Trigger callbacks for all caught classes
+    for _, obj in caught_classes.items():
+        obj.callback()
+        sqlite_db.commit()
+    if sqlite_db:
+        sqlite_db.close()
+    fd.close()
```

### Comparing `ntdsdotsqlite-1.0.0/ntdsdotsqlite/organizationalunithandler.py` & `ntdsdotsqlite-1.1.1/ntdsdotsqlite/organizationalunithandler.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-from ntdsdotsqlite.basehandler import BaseHandler
-from ntdsdotsqlite.utils import escape_dn_chars
-
-
-class OrganizationalUnitHandler(BaseHandler):
-    def handle(self, row):
-        ou_object = {
-            "id": row.get("DNT_col"),
-            "description": row.get(self.attributes["description"]),
-            "name": row.get(self.attributes["name"]),
-            "parent": row.get("PDNT_col"),
-            "isDeleted": row.get(self.attributes["isDeleted"]) == 1
-        }
-        stmt = """
-            INSERT INTO organizational_units VALUES (
-            :id, :name, :description, :parent, Null, :isDeleted
-            )
-        """
-        self.sqlite_db.execute(stmt, ou_object)
-
-    def callback(self):
-        # Compute DNs
-        roots = {domain_id: domain_DN for domain_id, domain_DN in self.sqlite_db.execute(
-            "SELECT id, dn FROM domain_dns"
-        ).fetchall()}
-        ous = self.sqlite_db.execute("SELECT id, parent, name FROM organizational_units").fetchall()
-        ous = {
-            ou_id: {"id": ou_id, "name": name, "parent": parent}
-            for ou_id, parent, name in ous
-        }
-        for ou_id, ou in ous.items():
-            dn_prefix = "OU=" + escape_dn_chars(ou["name"])
-            cur_object = ou
-            while True:
-                parent_dnt = cur_object["parent"]
-                if parent_dnt in ous.keys():
-                    parent = ous[parent_dnt]
-                elif parent_dnt in roots.keys():
-                    dn_prefix += ("," + roots[parent_dnt])
-                    break
-                else:
-                    print(
-                        f"Warning: could not compute DN of OU {cur_object['name']}."
-                    )
-                    break
-                cur_object = parent
-                name = parent["name"]
-                dn_prefix += "," + "OU=" + escape_dn_chars(name)
-            self.sqlite_db.execute(
-                "UPDATE organizational_units SET dn=? WHERE id=?",
-                (dn_prefix, ou_id)
-            )
-        self.sqlite_db.commit()
+from ntdsdotsqlite.basehandler import BaseHandler
+from ntdsdotsqlite.utils import escape_dn_chars
+
+
+class OrganizationalUnitHandler(BaseHandler):
+    def handle(self, row):
+        ou_object = {
+            "id": row.get("DNT_col"),
+            "description": row.get(self.attributes["description"]),
+            "name": row.get(self.attributes["name"]),
+            "parent": row.get("PDNT_col"),
+            "isDeleted": row.get(self.attributes["isDeleted"]) == 1
+        }
+        stmt = """
+            INSERT INTO organizational_units VALUES (
+            :id, :name, :description, :parent, Null, :isDeleted
+            )
+        """
+        self.sqlite_db.execute(stmt, ou_object)
+
+    def callback(self):
+        # Compute DNs
+        roots = {domain_id: domain_DN for domain_id, domain_DN in self.sqlite_db.execute(
+            "SELECT id, dn FROM domain_dns"
+        ).fetchall()}
+        ous = self.sqlite_db.execute("SELECT id, parent, name FROM organizational_units").fetchall()
+        ous = {
+            ou_id: {"id": ou_id, "name": name, "parent": parent}
+            for ou_id, parent, name in ous
+        }
+        for ou_id, ou in ous.items():
+            dn_prefix = "OU=" + escape_dn_chars(ou["name"])
+            cur_object = ou
+            while True:
+                parent_dnt = cur_object["parent"]
+                if parent_dnt in ous.keys():
+                    parent = ous[parent_dnt]
+                elif parent_dnt in roots.keys():
+                    dn_prefix += ("," + roots[parent_dnt])
+                    break
+                else:
+                    print(
+                        f"Warning: could not compute DN of OU {cur_object['name']}."
+                    )
+                    break
+                cur_object = parent
+                name = parent["name"]
+                dn_prefix += "," + "OU=" + escape_dn_chars(name)
+            self.sqlite_db.execute(
+                "UPDATE organizational_units SET dn=? WHERE id=?",
+                (dn_prefix, ou_id)
+            )
+        self.sqlite_db.commit()
```

### Comparing `ntdsdotsqlite-1.0.0/ntdsdotsqlite/personhandler.py` & `ntdsdotsqlite-1.1.1/ntdsdotsqlite/computerhandler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,126 +1,159 @@
-from ntdsdotsqlite.utils import hundredns_to_datetime, UAC_FLAGS
-from ntdsdotsqlite.utils import raw_to_guid, raw_to_sid
-from ntdsdotsqlite.basehandler import BaseHandler
-from ntdsdotsqlite.utils import escape_dn_chars
-
-import json
-
-
-class PersonHandler(BaseHandler):
-    def __init__(self, links, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.links = links
-
-    def handle(self, row):
-        lastLogonTimestamp = row.get(self.attributes["lastLogonTimestamp"])
-        pwdlastset = row.get(self.attributes["pwdLastSet"])
-        if pwdlastset:
-            pwdlastset = hundredns_to_datetime(pwdlastset)
-        if lastLogonTimestamp:
-            lastLogonTimestamp = hundredns_to_datetime(lastLogonTimestamp)
-        admincount = row.get(self.attributes["adminCount"])
-        if admincount is None:
-            admincount = 0
-        spn = row.get(self.attributes["servicePrincipalName"])
-        accountExpires = row.get(self.attributes["accountExpires"])
-        if accountExpires:
-            if accountExpires and accountExpires == 0 or accountExpires == 0x7FFFFFFFFFFFFFFF:
-                accountExpires = 0
-            else:
-                accountExpires = hundredns_to_datetime(accountExpires)
-        uac = row.get(self.attributes["userAccountControl"])
-        sid = row.get(self.attributes["objectSid"])
-        guid = row.get(self.attributes["objectGUID"])
-        account = {
-            "id": row.get("DNT_col"), "description": row.get(self.attributes["description"]),
-            "UAC": uac,
-            "SID": raw_to_sid(sid) if sid else None,
-            "samaccountname": row.get(self.attributes["sAMAccountName"]),
-            # unix epoch or NULL if password never set
-            "pwdLastSet": pwdlastset,
-            "nthash": row.get(self.attributes["unicodePwd"]),
-            "commonname": row.get(self.attributes["cn"]),
-            "GUID": raw_to_guid(guid) if guid else None,
-            "adminCount": admincount,
-            "displayName": row.get(self.attributes["displayName"]),
-            "UPN": row.get(self.attributes["userPrincipalName"]),
-            "supplementalCredentials": row.get(self.attributes["supplementalCredentials"]),
-            # unix epoch
-            "lastLogonTimestamp": lastLogonTimestamp,
-            "lmPwdHistory": row.get(self.attributes["lmPwdHistory"]),
-            "ntPwdHistory": row.get(self.attributes["ntPwdHistory"]),
-            "accountExpires": accountExpires,
-            "SPN": spn,
-            "lmhash": row.get(self.attributes["dBCSPwd"]),
-            "parent": row.get("PDNT_col"),
-            "isDeleted": row.get(self.attributes["isDeleted"]) == 1,
-            "primaryGroup": row.get(self.attributes["primaryGroupID"])
-        }
-        account["login"] = (
-            account["UPN"].split("@")[0] if account["UPN"]
-            else account["samaccountname"]
-        )
-        if (spn := account["SPN"]):
-            if type(spn) is str:
-                account["SPN"] = json.dumps([spn])
-            elif type(spn) is list:
-                account["SPN"] = json.dumps(spn)
-            else:
-                print(f"SPN type unknown : {spn} - {type(spn)}")
-                print(account)
-                exit(1)
-        if uac:
-            uac_flags = {
-                k.name: True if uac & k.value else False for k in UAC_FLAGS
-            }
-            account["uac_flags"] = json.dumps(uac_flags)
-            account["isDisabled"] = uac_flags["ACCOUNTDISABLE"]
-        else:
-            account["uac_flags"] = None
-            account["isDisabled"] = None
-        stmt = """
-            INSERT INTO user_accounts VALUES (
-            :id, :nthash, :lmhash, :UAC, :description, :lastLogonTimestamp,
-            :pwdLastSet, :adminCount, :displayName, :GUID, :SID, :SPN,
-            Null, :UPN, :login, :samaccountname, :commonname,
-            :supplementalCredentials, :lmPwdHistory, :ntPwdHistory, :accountExpires,
-            :uac_flags, :parent, Null, :isDeleted, :primaryGroup,
-            Null, :isDisabled
-            )
-        """
-        self.sqlite_db.execute(stmt, account)
-
-    def callback(self):
-        # set the domain id
-        domain_id = self.sqlite_db.execute("SELECT id FROM domains").fetchone()[0]
-        ous = {
-            oid: dn for oid, dn in self.sqlite_db.execute("SELECT id, dn FROM organizational_units")
-        }
-        users = self.sqlite_db.execute(
-            "SELECT id, commonname, parent_OU, primaryGroup FROM user_accounts"
-        )
-        containers = {
-            cid: cdn for (cid, cdn) in self.sqlite_db.execute("SELECT id, dn FROM containers")
-        }
-        domains = {
-            did: ddn for (did, ddn) in self.sqlite_db.execute("SELECT id, dn FROM domain_dns")
-        }
-        group_ids = [x[0] for x in self.sqlite_db.execute("SELECT id FROM groups").fetchall()]
-        for uid, cn, parent_OU, primaryGroup in users:
-            # Compute DN
-            if parent_OU in ous.keys():
-                dn = f"CN={escape_dn_chars(cn)},{ous[parent_OU]}"
-            elif parent_OU in containers.keys():
-                dn = f"CN={escape_dn_chars(cn)},{containers[parent_OU]}"
-            elif parent_OU in domains.keys():
-                dn = f"CN={escape_dn_chars(cn)},{domains[parent_OU]}"
-            else:
-                print(f"Warning: could not compute DN of user {cn}")
-            links_list = self.links[uid]
-            memberof = json.dumps([link for link in links_list if link in group_ids])
-            self.sqlite_db.execute(
-                "UPDATE user_accounts set domain=?, memberOf=?, primaryGroup=("
-                f"SELECT id from groups WHERE SID LIKE '%-{primaryGroup}'"
-                "), dn=? WHERE id=?",
-                (domain_id, memberof, dn, uid)
-            )
+from ntdsdotsqlite.decrypt import decrypt_hash, decrypt_history, decryptSupplementalInfo
+from ntdsdotsqlite.utils import hundredns_to_datetime, UAC_FLAGS
+from ntdsdotsqlite.utils import raw_to_guid, raw_to_sid
+from ntdsdotsqlite.basehandler import BaseHandler
+from ntdsdotsqlite.utils import escape_dn_chars
+import json
+
+
+class ComputerHandler(BaseHandler):
+    def __init__(self, sqlite_db, attributes, ese_db, dh):
+        super().__init__(sqlite_db, attributes, ese_db)
+        self.should_decrypt = dh.bootkey is not None
+        self.peklist = dh.pek
+        self.could_not_decrypt_yet = list()
+
+    def handle(self, row):
+        lastLogonTimestamp = row.get(self.attributes["lastLogonTimestamp"])
+        pwdlastset = row.get(self.attributes["pwdLastSet"])
+        if pwdlastset:
+            pwdlastset = hundredns_to_datetime(pwdlastset)
+        if lastLogonTimestamp:
+            lastLogonTimestamp = hundredns_to_datetime(lastLogonTimestamp)
+        admincount = row.get(self.attributes["adminCount"])
+        if admincount is None:
+            admincount = 0
+        spn = row.get(self.attributes["servicePrincipalName"])
+        accountExpires = row.get(self.attributes["accountExpires"])
+        if accountExpires:
+            if accountExpires and accountExpires == 0 or accountExpires == 0x7FFFFFFFFFFFFFFF:
+                accountExpires = 0
+            else:
+                accountExpires = hundredns_to_datetime(accountExpires)
+        uac = row.get(self.attributes["userAccountControl"])
+        sid = row.get(self.attributes["objectSid"])
+        guid = row.get(self.attributes["objectGUID"])
+        account = {
+            "id": row.get("DNT_col"), "description": row.get(self.attributes["description"]),
+            "UAC": uac,
+            "SID": raw_to_sid(sid) if sid else None,
+            "samaccountname": row.get(self.attributes["sAMAccountName"]),
+            # unix epoch or NULL if password never set
+            "pwdLastSet": pwdlastset,
+            "encrypted_nthash": row.get(self.attributes["unicodePwd"]),
+            "nthash": None,
+            "commonname": row.get(self.attributes["cn"]),
+            "GUID": raw_to_guid(guid) if guid else None,
+            "adminCount": admincount,
+            "displayName": row.get(self.attributes["displayName"]),
+            "UPN": row.get(self.attributes["userPrincipalName"]),
+            "encrypted_supplementalCredentials": (
+                row.get(self.attributes["supplementalCredentials"])
+            ),
+            "supplementalCredentials": None,
+            # unix epoch
+            "lastLogonTimestamp": lastLogonTimestamp,
+            "encrypted_lmPwdHistory": row.get(self.attributes["lmPwdHistory"]),
+            "lmPwdHistory": None,
+            "encrypted_ntPwdHistory": row.get(self.attributes["ntPwdHistory"]),
+            "ntPwdHistory": None,
+            "accountExpires": accountExpires,
+            "SPN": spn,
+            "encrypted_lmhash": row.get(self.attributes["dBCSPwd"]),
+            "lmhash": None,
+            "parent": row.get("PDNT_col"),
+            "isDeleted": row.get(self.attributes["isDeleted"]) == 1,
+            "primaryGroup": row.get(self.attributes["primaryGroupID"])
+        }
+        account["login"] = (
+            account["UPN"].split("@")[0] if account["UPN"]
+            else account["samaccountname"]
+        )
+        if (spn := account["SPN"]):
+            if type(spn) is str:
+                account["SPN"] = json.dumps([spn])
+            elif type(spn) is list:
+                account["SPN"] = json.dumps(spn)
+            else:
+                print(f"SPN type unknown : {spn} - {type(spn)}")
+                print(account)
+                exit(1)
+        if uac:
+            uac_flags = {
+                k.name: True if uac & k.value else False for k in UAC_FLAGS
+            }
+            account["uac_flags"] = json.dumps(uac_flags)
+            account["isDisabled"] = uac_flags["ACCOUNTDISABLE"]
+        else:
+            account["uac_flags"] = None
+            account["isDisabled"] = None
+        if self.should_decrypt:
+            try:
+                account["nthash"] = decrypt_hash(self.peklist, account, "nt")
+                account["lmhash"] = decrypt_hash(self.peklist, account, "lm")
+                account["lmPwdHistory"] = json.dumps(decrypt_history(self.peklist, account, "lm"))
+                account["ntPwdHistory"] = json.dumps(decrypt_history(self.peklist, account, "nt"))
+                account["supplementalCredentials"] = json.dumps(
+                    decryptSupplementalInfo(self.peklist, account)
+                )
+            except IndexError:
+                self.could_not_decrypt_yet.append(account)
+        stmt = """
+            INSERT INTO machine_accounts VALUES (
+            :id, :encrypted_nthash, :nthash, :encrypted_lmhash, :lmhash, :UAC, :description,
+            :lastLogonTimestamp, :pwdLastSet, :adminCount, :displayName, :GUID, :SID, :SPN,
+            Null, :UPN, :login, :samaccountname, :commonname, :encrypted_supplementalCredentials,
+            :supplementalCredentials, :encrypted_lmPwdHistory, :lmPwdHistory,
+            :encrypted_ntPwdHistory, :ntPwdHistory, :accountExpires, :uac_flags, :parent, Null,
+            :isDeleted, :primaryGroup, :isDisabled
+            )
+        """
+        self.sqlite_db.execute(stmt, account)
+
+    def callback(self):
+        # set the domain id
+        domain_id = self.sqlite_db.execute("SELECT id FROM domains").fetchone()[0]
+        ous = {
+            oid: dn for oid, dn in self.sqlite_db.execute("SELECT id, dn FROM organizational_units")
+        }
+        machines = self.sqlite_db.execute(
+            "SELECT id, commonname, parent_OU, primaryGroup FROM user_accounts"
+        )
+        containers = {
+            cid: cdn for (cid, cdn) in self.sqlite_db.execute("SELECT id, dn FROM containers")
+        }
+        domains = {
+            did: ddn for (did, ddn) in self.sqlite_db.execute("SELECT id, dn FROM domain_dns")
+        }
+        for uid, cn, parent_OU, primaryGroup in machines:
+            # Compute DN
+            if parent_OU in ous.keys():
+                dn = f"CN={escape_dn_chars(cn)},{ous[parent_OU]}"
+            elif parent_OU in containers.keys():
+                dn = f"CN={escape_dn_chars(cn)},{containers[parent_OU]}"
+            elif parent_OU in domains.keys():
+                dn = f"CN={escape_dn_chars(cn)},{domains[parent_OU]}"
+            else:
+                print(f"Warning: could not compute DN of machine {cn}")
+            self.sqlite_db.execute(
+                "UPDATE machine_accounts set domain=?, primaryGroup=("
+                f"SELECT id from groups WHERE SID LIKE '%-{primaryGroup}'"
+                "), dn=? WHERE id=?",
+                (domain_id, dn, uid)
+            )
+        # Decrypt users we could not decrypt previously
+        for account in self.could_not_decrypt_yet:
+            account["nthash"] = decrypt_hash(self.peklist, account, "nt")
+            account["lmhash"] = decrypt_hash(self.peklist, account, "lm")
+            account["lmPwdHistory"] = decrypt_history(self.peklist, account, "lm")
+            account["ntPwdHistory"] = decrypt_history(self.peklist, account, "nt")
+            account["supplementalCredentials"] = decryptSupplementalInfo(self.peklist, account)
+            self.sqlite_db.execute(
+                "UPDATE user_accounts set nthash=?, lmhash=?, ntPwdHistory=?, lmPwdHistory=?, "
+                "supplementalCredentials=? WHERE id=?",
+                (
+                    account["nthash"], account["lmhash"], json.dumps(account["ntPwdHistory"]),
+                    json.dumps(account["lmPwdHistory"]),
+                    json.dumps(account["supplementalCredentials"]), account["id"]
+                )
+            )
```

### Comparing `ntdsdotsqlite-1.0.0/ntdsdotsqlite/trusteddomainhandler.py` & `ntdsdotsqlite-1.1.1/ntdsdotsqlite/trusteddomainhandler.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-from ntdsdotsqlite.utils import raw_to_guid, raw_to_sid
-from ntdsdotsqlite.basehandler import BaseHandler
-from ntdsdotsqlite.utils import TRUST_FLAGS
-import json
-
-
-class TrustedDomainHandler(BaseHandler):
-    def handle(self, row):
-        sid = row.get(self.attributes["objectSid"])
-        sid = raw_to_sid(sid) if sid else None,
-        dnt_id = row.get("DNT_col")
-        guid = row.get(self.attributes["objectGUID"])
-        guid = raw_to_guid(guid) if guid else None
-        commonname = row.get(self.attributes["cn"])
-        name = row.get(self.attributes["name"])
-        trustattributes = row.get(self.attributes["trustAttributes"])
-        trustdirection = (
-            "disabled" if (direction := row.get(self.attributes["trustDirection"])) == 0 else
-            "inbound" if direction == 1 else
-            "outbound" if direction == 2 else
-            "bidirectional" if direction == 3 else
-            None
-        )
-        trustpartner = row.get(self.attributes["trustPartner"])
-        trusttype = (
-            "downlevel" if (ttype := row.get(self.attributes["trustType"])) == 1 else
-            "uplevel" if ttype == 2 else
-            "MIT" if ttype == 3 else
-            "DCE" if ttype == 4 else
-            None
-        )
-        attribute_flags = {
-            f.name: True if trustattributes & f.value else False for f in TRUST_FLAGS
-        }
-        trust = {
-            "id": dnt_id,
-            "commonname": commonname,
-            "name": name,
-            "trustAttributes": trustattributes,
-            "attributeFlags": json.dumps(attribute_flags),
-            "trustDirection": trustdirection,
-            "trustPartner": trustpartner,
-            "trustType": trusttype
-        }
-        stmt = """
-            INSERT INTO trusted_domains VALUES (
-            :id, :commonname, :name, :trustAttributes, :trustDirection, :trustPartner, :trustType,
-            :attributeFlags
-            )
-        """
-        self.sqlite_db.execute(stmt, trust)
-
-    def callback(self):
-        pass
+from ntdsdotsqlite.utils import raw_to_guid, raw_to_sid
+from ntdsdotsqlite.basehandler import BaseHandler
+from ntdsdotsqlite.utils import TRUST_FLAGS
+import json
+
+
+class TrustedDomainHandler(BaseHandler):
+    def handle(self, row):
+        sid = row.get(self.attributes["objectSid"])
+        sid = raw_to_sid(sid) if sid else None,
+        dnt_id = row.get("DNT_col")
+        guid = row.get(self.attributes["objectGUID"])
+        guid = raw_to_guid(guid) if guid else None
+        commonname = row.get(self.attributes["cn"])
+        name = row.get(self.attributes["name"])
+        trustattributes = row.get(self.attributes["trustAttributes"])
+        trustdirection = (
+            "disabled" if (direction := row.get(self.attributes["trustDirection"])) == 0 else
+            "inbound" if direction == 1 else
+            "outbound" if direction == 2 else
+            "bidirectional" if direction == 3 else
+            None
+        )
+        trustpartner = row.get(self.attributes["trustPartner"])
+        trusttype = (
+            "downlevel" if (ttype := row.get(self.attributes["trustType"])) == 1 else
+            "uplevel" if ttype == 2 else
+            "MIT" if ttype == 3 else
+            "DCE" if ttype == 4 else
+            None
+        )
+        attribute_flags = {
+            f.name: True if trustattributes & f.value else False for f in TRUST_FLAGS
+        }
+        trust = {
+            "id": dnt_id,
+            "commonname": commonname,
+            "name": name,
+            "trustAttributes": trustattributes,
+            "attributeFlags": json.dumps(attribute_flags),
+            "trustDirection": trustdirection,
+            "trustPartner": trustpartner,
+            "trustType": trusttype
+        }
+        stmt = """
+            INSERT INTO trusted_domains VALUES (
+            :id, :commonname, :name, :trustAttributes, :trustDirection, :trustPartner, :trustType,
+            :attributeFlags
+            )
+        """
+        self.sqlite_db.execute(stmt, trust)
+
+    def callback(self):
+        pass
```

### Comparing `ntdsdotsqlite-1.0.0/ntdsdotsqlite/utils.py` & `ntdsdotsqlite-1.1.1/ntdsdotsqlite/utils.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-from datetime import datetime, timedelta
-from collections import defaultdict
-from enum import IntFlag
-from pathlib import Path
-import sqlite3
-
-
-# transforms a guid from raw hex byte returned by dissect to a correct GUID string
-def raw_to_guid(raw):
-    p1 = raw[:4][::-1].hex()
-    p2 = raw[4:6][::-1].hex()
-    p3 = raw[6:8][::-1].hex()
-    p4 = raw[8:10].hex()
-    p5 = raw[10:].hex()
-    return f"{p1}-{p2}-{p3}-{p4}-{p5}"
-
-
-# Transforms raw bytes returned by dessect to a correct SID string
-def raw_to_sid(raw):
-    rev = str(int(raw[0]))
-    nb_dashes = int(raw[1])
-    id_auth_value = int.from_bytes(raw[2:8], "big")
-    subparts = []
-    for i in range(nb_dashes):
-        endianess = "big" if i == nb_dashes - 1 else "little"
-        subparts.append(str(int.from_bytes(raw[8+(i*4):8+(i*4)+4], endianess)))
-    return f"S-{rev}-{id_auth_value}-{'-'.join(subparts)}"
-
-
-# Translates microsoft duration/datetime format (intervals of 100ns) to python datetime object
-def hundredns_to_datetime(ns):
-    return timedelta(seconds=ns / 10000000) + datetime(1601, 1, 1)
-
-
-# Writes an initial sqlite database, with the chosen sql representation of an NTDS db.
-def create_database(sqlite_path):
-    # overwrite database if already existing
-    f = open(sqlite_path, "w")
-    f.close()
-    db = sqlite3.connect(sqlite_path)
-    script = open(Path(__file__).parent / "model.sql", "r").read()
-    cursor = db.cursor()
-    cursor.executescript(script)
-    if db:
-        db.close()
-
-
-class TRUST_FLAGS(IntFlag):
-    NON_TRANSITIVE = 0x1
-    UPLEVEL_ONLY = 0x2
-    QUARANTINED_DOMAIN = 0x4
-    FOREST_TRANSITIVE = 0x8
-    CROSS_ORGANIZATION = 0x10
-    WITHIN_FOREST = 0x20
-    TREAT_AS_EXTERNAL = 0x40
-    USES_RC4_ENCRYPTION = 0x80
-    CROSS_ORGANIZATION_NO_TGT_DELEGATION = 0x200
-    PIM_TRUST = 0x400
-
-
-class UAC_FLAGS(IntFlag):
-    SCRIPT = 0x0001
-    ACCOUNTDISABLE = 0x0002
-    HOMEDIR_REQUIRED = 0x0008
-    LOCKOUT = 0x0010
-    PASSWD_NOTREQD = 0x0020
-    PASSWD_CANT_CHANGE = 0x0040
-    ENCRYPTED_TEXT_PWD_ALLOWED = 0x0080
-    TEMP_DUPLICATE_ACCOUNT = 0x0100
-    NORMAL_ACCOUNT = 0x0200
-    INTERDOMAIN_TRUST_ACCOUNT = 0x0800
-    WORKSTATION_TRUST_ACCOUNT = 0x1000
-    SERVER_TRUST_ACCOUNT = 0x2000
-    DONT_EXPIRE_PASSWORD = 0x10000
-    MNS_LOGON_ACCOUNT = 0x20000
-    SMARTCARD_REQUIRED = 0x40000
-    TRUSTED_FOR_DELEGATION = 0x80000
-    NOT_DELEGATED = 0x100000
-    USE_DES_KEY_ONLY = 0x200000
-    DONT_REQ_PREAUTH = 0x400000
-    PASSWORD_EXPIRED = 0x800000
-    TRUSTED_TO_AUTH_FOR_DELEGATION = 0x1000000
-    PARTIAL_SECRETS_ACCOUNT = 0x04000000
-
-
-# Extracted from python-ldap/Lib/ldap/dn.py, in order to remove one dependency
-# that would need to be compiled otherwise.
-def escape_dn_chars(s):
-    """
-    Escape all DN special characters found in s
-    with a back-slash (see RFC 4514, section 2.4)
-    """
-    if s:
-        s = s.replace('\\', '\\\\')
-        s = s.replace(',', '\\,')
-        s = s.replace('+', '\\+')
-        s = s.replace('"', '\\"')
-        s = s.replace('<', '\\<')
-        s = s.replace('>', '\\>')
-        s = s.replace(';', '\\;')
-        s = s.replace('=', '\\=')
-        s = s.replace('\000', '\\\000')
-        if s[-1] == ' ':
-            s = ''.join((s[:-1], '\\ '))
-        if s[0] == '#' or s[0] == ' ':
-            s = ''.join(('\\', s))
-    return s
-
-
-def compute_links(ese_db):
-    links = ese_db.table("link_table")
-    relations = defaultdict(list)
-    for link in links.records():
-        flink = link.get("link_DNT")
-        blink = link.get("backlink_DNT")
-        relations[blink].append(flink)
-    return relations
+from datetime import datetime, timedelta
+from collections import defaultdict
+from enum import IntFlag
+from pathlib import Path
+import sqlite3
+
+
+# transforms a guid from raw hex byte returned by dissect to a correct GUID string
+def raw_to_guid(raw):
+    p1 = raw[:4][::-1].hex()
+    p2 = raw[4:6][::-1].hex()
+    p3 = raw[6:8][::-1].hex()
+    p4 = raw[8:10].hex()
+    p5 = raw[10:].hex()
+    return f"{p1}-{p2}-{p3}-{p4}-{p5}"
+
+
+# Transforms raw bytes returned by dessect to a correct SID string
+def raw_to_sid(raw):
+    rev = str(int(raw[0]))
+    nb_dashes = int(raw[1])
+    id_auth_value = int.from_bytes(raw[2:8], "big")
+    subparts = []
+    for i in range(nb_dashes):
+        endianess = "big" if i == nb_dashes - 1 else "little"
+        subparts.append(str(int.from_bytes(raw[8+(i*4):8+(i*4)+4], endianess)))
+    return f"S-{rev}-{id_auth_value}-{'-'.join(subparts)}"
+
+
+# Translates microsoft duration/datetime format (intervals of 100ns) to python datetime object
+def hundredns_to_datetime(ns):
+    return timedelta(seconds=ns / 10000000) + datetime(1601, 1, 1)
+
+
+# Writes an initial sqlite database, with the chosen sql representation of an NTDS db.
+def create_database(sqlite_path):
+    # overwrite database if already existing
+    f = open(sqlite_path, "w")
+    f.close()
+    db = sqlite3.connect(sqlite_path)
+    script = open(Path(__file__).parent / "model.sql", "r").read()
+    cursor = db.cursor()
+    cursor.executescript(script)
+    if db:
+        db.close()
+
+
+class TRUST_FLAGS(IntFlag):
+    NON_TRANSITIVE = 0x1
+    UPLEVEL_ONLY = 0x2
+    QUARANTINED_DOMAIN = 0x4
+    FOREST_TRANSITIVE = 0x8
+    CROSS_ORGANIZATION = 0x10
+    WITHIN_FOREST = 0x20
+    TREAT_AS_EXTERNAL = 0x40
+    USES_RC4_ENCRYPTION = 0x80
+    CROSS_ORGANIZATION_NO_TGT_DELEGATION = 0x200
+    PIM_TRUST = 0x400
+
+
+class UAC_FLAGS(IntFlag):
+    SCRIPT = 0x0001
+    ACCOUNTDISABLE = 0x0002
+    HOMEDIR_REQUIRED = 0x0008
+    LOCKOUT = 0x0010
+    PASSWD_NOTREQD = 0x0020
+    PASSWD_CANT_CHANGE = 0x0040
+    ENCRYPTED_TEXT_PWD_ALLOWED = 0x0080
+    TEMP_DUPLICATE_ACCOUNT = 0x0100
+    NORMAL_ACCOUNT = 0x0200
+    INTERDOMAIN_TRUST_ACCOUNT = 0x0800
+    WORKSTATION_TRUST_ACCOUNT = 0x1000
+    SERVER_TRUST_ACCOUNT = 0x2000
+    DONT_EXPIRE_PASSWORD = 0x10000
+    MNS_LOGON_ACCOUNT = 0x20000
+    SMARTCARD_REQUIRED = 0x40000
+    TRUSTED_FOR_DELEGATION = 0x80000
+    NOT_DELEGATED = 0x100000
+    USE_DES_KEY_ONLY = 0x200000
+    DONT_REQ_PREAUTH = 0x400000
+    PASSWORD_EXPIRED = 0x800000
+    TRUSTED_TO_AUTH_FOR_DELEGATION = 0x1000000
+    PARTIAL_SECRETS_ACCOUNT = 0x04000000
+
+
+# Extracted from python-ldap/Lib/ldap/dn.py, in order to remove one dependency
+# that would need to be compiled otherwise.
+def escape_dn_chars(s):
+    """
+    Escape all DN special characters found in s
+    with a back-slash (see RFC 4514, section 2.4)
+    """
+    if s:
+        s = s.replace('\\', '\\\\')
+        s = s.replace(',', '\\,')
+        s = s.replace('+', '\\+')
+        s = s.replace('"', '\\"')
+        s = s.replace('<', '\\<')
+        s = s.replace('>', '\\>')
+        s = s.replace(';', '\\;')
+        s = s.replace('=', '\\=')
+        s = s.replace('\000', '\\\000')
+        if s[-1] == ' ':
+            s = ''.join((s[:-1], '\\ '))
+        if s[0] == '#' or s[0] == ' ':
+            s = ''.join(('\\', s))
+    return s
+
+
+def compute_links(ese_db):
+    links = ese_db.table("link_table")
+    relations = defaultdict(list)
+    for link in links.records():
+        flink = link.get("link_DNT")
+        blink = link.get("backlink_DNT")
+        relations[blink].append(flink)
+    return relations
```

### Comparing `ntdsdotsqlite-1.0.0/README.md` & `ntdsdotsqlite-1.1.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-# NTDS.Sqlite
-
-This software can be used either directly as a CLI utility or as a library to get an SQLite database from an NTDS.DIT one. Encrypted bits can be decrypted if the associated system hive is provided altogether.
-
-# Installation
-
-`python -m pip install ntdsdotsqlite`
-
-# Usage
-
-`ntdsdotsqlite NTDS.DIT --system SYSTEM -o NTDS.sqlite`
-
-```
-usage: NTDS.sqlite [-h] [--system SYSTEM] -o OUTFILE NTDS
-
-This tool helps dumping NTDS.DIT file to an SQLite database
-
-positional arguments:
-  NTDS                  The NTDS.DIT file
-
-optional arguments:
-  -h, --help            show this help message and exit
-  --system SYSTEM       The SYSTEM hive to decrypt hashes. If not provided, hashes will be encrypted inside the sqlite database.
-  -o OUTFILE, --outfile OUTFILE
-                        The sqlite database. Example : NTDS.sqlite
-```
-
-# SQL model
-
-The SQL model is described in the `sql_model.md` file in this repository. Basicaly, not all objects are extracted (at all), but the following are retrieved as of today : domain object, user accounts, machine accounts, groups, organizational units and containers. I thought these would be the most useful. If you need more object classes to be extracted or additional attributes, feel free to open an issue or a pull request !
-
-Similarly, if you see inconsistence in some data (especially in links between objects), dont hesitate to open issues, documentation is very rare on this topic and I had to do some testing/guessing to understand how OUs, groups and accounts are linked together in the NTDS database.
-
-# Performances
-
-Performances can be a bit low for huge NTDS files. I made the choice not to store the whole NTDS in memory as they can grow quite huge (several gigabytes). A few large things are still put in memory such as links between objects and organizational units (to build distinguished names faster). These should not represent too much data to work with even with multiple gigabytes NTDS files.
+# NTDS.Sqlite
+
+This software can be used either directly as a CLI utility or as a library to get an SQLite database from an NTDS.DIT one. Encrypted bits can be decrypted if the associated system hive is provided altogether.
+
+# Installation
+
+`python -m pip install ntdsdotsqlite`
+
+# Usage
+
+`ntdsdotsqlite NTDS.DIT --system SYSTEM -o NTDS.sqlite`
+
+```
+usage: NTDS.sqlite [-h] [--system SYSTEM] -o OUTFILE NTDS
+
+This tool helps dumping NTDS.DIT file to an SQLite database
+
+positional arguments:
+  NTDS                  The NTDS.DIT file
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --system SYSTEM       The SYSTEM hive to decrypt hashes. If not provided, hashes will be encrypted inside the sqlite database.
+  -o OUTFILE, --outfile OUTFILE
+                        The sqlite database. Example : NTDS.sqlite
+```
+
+# SQL model
+
+The SQL model is described in the `sql_model.md` file in this repository. Basicaly, not all objects are extracted (at all), but the following are retrieved as of today : domain object, user accounts, machine accounts, groups, organizational units and containers. I thought these would be the most useful. If you need more object classes to be extracted or additional attributes, feel free to open an issue or a pull request !
+
+# Performances
+
+Performances can be a bit low for huge NTDS files. The whole NTDS is not stored in memory to prevent memory exhaustion when working on huge files (NTDS databases can grow to several gigabytes).
```

### Comparing `ntdsdotsqlite-1.0.0/PKG-INFO` & `ntdsdotsqlite-1.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntdsdotsqlite
-Version: 1.0.0
+Version: 1.1.1
 Summary: A small utility to get an SQLite  database from an NTDS.DIT file.
 Home-page: https://github.com/almandin/ntdsdotsqlite
 License: Beerware
 Author: Virgile Jarry
 Author-email: virgile@mailbox.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -46,12 +46,11 @@
                         The sqlite database. Example : NTDS.sqlite
 ```
 
 # SQL model
 
 The SQL model is described in the `sql_model.md` file in this repository. Basicaly, not all objects are extracted (at all), but the following are retrieved as of today : domain object, user accounts, machine accounts, groups, organizational units and containers. I thought these would be the most useful. If you need more object classes to be extracted or additional attributes, feel free to open an issue or a pull request !
 
-Similarly, if you see inconsistence in some data (especially in links between objects), dont hesitate to open issues, documentation is very rare on this topic and I had to do some testing/guessing to understand how OUs, groups and accounts are linked together in the NTDS database.
-
 # Performances
 
-Performances can be a bit low for huge NTDS files. I made the choice not to store the whole NTDS in memory as they can grow quite huge (several gigabytes). A few large things are still put in memory such as links between objects and organizational units (to build distinguished names faster). These should not represent too much data to work with even with multiple gigabytes NTDS files.
+Performances can be a bit low for huge NTDS files. The whole NTDS is not stored in memory to prevent memory exhaustion when working on huge files (NTDS databases can grow to several gigabytes).
+
```


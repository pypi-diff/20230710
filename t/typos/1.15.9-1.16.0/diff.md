# Comparing `tmp/typos-1.15.9.tar.gz` & `tmp/typos-1.16.0.tar.gz`

## Comparing `typos-1.15.9.tar` & `typos-1.16.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 typos-1.15.9/local_dependencies/varcon-core/Cargo.toml
--rw-r--r--   0     1001      123     1488 2023-06-30 14:48:33.000000 typos-1.15.9/local_dependencies/varcon-core/src/borrowed.rs
--rw-r--r--   0     1001      123     2850 2023-06-30 14:48:33.000000 typos-1.15.9/local_dependencies/varcon-core/src/lib.rs
--rw-r--r--   0     1001      123    16454 2023-06-30 14:48:33.000000 typos-1.15.9/local_dependencies/varcon-core/src/parser.rs
--rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 typos-1.15.9/local_dependencies/typos-dict/Cargo.toml
--rw-r--r--   0     1001      123  7025517 2023-06-30 14:48:33.000000 typos-1.15.9/local_dependencies/typos-dict/src/dict_codegen.rs
--rw-r--r--   0     1001      123       51 2023-06-30 14:48:33.000000 typos-1.15.9/local_dependencies/typos-dict/src/lib.rs
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 typos-1.15.9/local_dependencies/dictgen/Cargo.toml
--rw-r--r--   0     1001      123      130 2023-06-30 14:48:33.000000 typos-1.15.9/local_dependencies/dictgen/src/lib.rs
--rw-r--r--   0     1001      123     2687 2023-06-30 14:48:33.000000 typos-1.15.9/local_dependencies/dictgen/src/map.rs
--rw-r--r--   0     1001      123     3726 2023-06-30 14:48:33.000000 typos-1.15.9/local_dependencies/dictgen/src/table.rs
--rw-r--r--   0     1001      123    10637 2023-06-30 14:48:33.000000 typos-1.15.9/local_dependencies/dictgen/src/trie.rs
--rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 typos-1.15.9/local_dependencies/typos/Cargo.toml
--rw-r--r--   0     1001      123     2794 2023-06-30 14:48:33.000000 typos-1.15.9/local_dependencies/typos/src/check.rs
--rw-r--r--   0     1001      123     2175 2023-06-30 14:48:33.000000 typos-1.15.9/local_dependencies/typos/src/dict.rs
--rw-r--r--   0     1001      123       74 2023-06-30 14:48:33.000000 typos-1.15.9/local_dependencies/typos/src/lib.rs
--rw-r--r--   0     1001      123    44720 2023-06-30 14:48:33.000000 typos-1.15.9/local_dependencies/typos/src/tokens.rs
--rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 typos-1.15.9/local_dependencies/typos-vars/Cargo.toml
--rw-r--r--   0     1001      123      117 2023-06-30 14:48:33.000000 typos-1.15.9/local_dependencies/typos-vars/src/lib.rs
--rw-r--r--   0     1001      123  6086180 2023-06-30 14:48:33.000000 typos-1.15.9/local_dependencies/typos-vars/src/vars_codegen.rs
--rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 typos-1.15.9/pyproject.toml
--rw-r--r--   0        0        0     3030 1970-01-01 00:00:00.000000 typos-1.15.9/rust_src/typos-cli/Cargo.toml
--rw-r--r--   0     1001      123     2221 2023-06-30 14:48:33.000000 typos-1.15.9/rust_src/typos-cli/benches/checks.rs
--rw-r--r--   0     1001      123     4586 2023-06-30 14:48:33.000000 typos-1.15.9/rust_src/typos-cli/benches/corrections.rs
--rw-r--r--   0     1001      123     1347 2023-06-30 14:48:33.000000 typos-1.15.9/rust_src/typos-cli/benches/data.rs
--rw-r--r--   0     1001      123     3306 2023-06-30 14:48:33.000000 typos-1.15.9/rust_src/typos-cli/benches/tokenize.rs
--rw-r--r--   0     1001      123     8452 2023-06-30 14:48:33.000000 typos-1.15.9/rust_src/typos-cli/src/bin/typos-cli/args.rs
--rw-r--r--   0     1001      123     9824 2023-06-30 14:48:33.000000 typos-1.15.9/rust_src/typos-cli/src/bin/typos-cli/main.rs
--rw-r--r--   0     1001      123    12622 2023-06-30 14:48:33.000000 typos-1.15.9/rust_src/typos-cli/src/bin/typos-cli/report.rs
--rw-r--r--   0     1001      123    21859 2023-06-30 14:48:33.000000 typos-1.15.9/rust_src/typos-cli/src/config.rs
--rw-r--r--   0     1001      123    10240 2023-06-30 14:48:33.000000 typos-1.15.9/rust_src/typos-cli/src/default_types.rs
--rw-r--r--   0     1001      123    11574 2023-06-30 14:48:33.000000 typos-1.15.9/rust_src/typos-cli/src/dict.rs
--rw-r--r--   0     1001      123    32621 2023-06-30 14:48:33.000000 typos-1.15.9/rust_src/typos-cli/src/file.rs
--rw-r--r--   0     1001      123     5919 2023-06-30 14:48:33.000000 typos-1.15.9/rust_src/typos-cli/src/file_type.rs
--rw-r--r--   0     1001      123      299 2023-06-30 14:48:33.000000 typos-1.15.9/rust_src/typos-cli/src/lib.rs
--rw-r--r--   0     1001      123    17558 2023-06-30 14:48:33.000000 typos-1.15.9/rust_src/typos-cli/src/policy.rs
--rw-r--r--   0     1001      123     5561 2023-06-30 14:48:33.000000 typos-1.15.9/rust_src/typos-cli/src/report.rs
--rw-r--r--   0     1001      123      207 2023-06-30 14:48:33.000000 typos-1.15.9/rust_src/typos-cli/tests/cmd/false-positives.in/README.md
--rw-r--r--   0     1001      123    53454 2023-06-30 14:48:33.000000 typos-1.15.9/Cargo.lock
--rw-r--r--   0        0        0     5371 1970-01-01 00:00:00.000000 typos-1.15.9/PKG-INFO
+-rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 typos-1.16.0/local_dependencies/typos-dict/Cargo.toml
+-rw-r--r--   0     1001      123  7035769 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/typos-dict/src/dict_codegen.rs
+-rw-r--r--   0     1001      123       51 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/typos-dict/src/lib.rs
+-rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 typos-1.16.0/local_dependencies/varcon-core/Cargo.toml
+-rw-r--r--   0     1001      123     1488 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/varcon-core/src/borrowed.rs
+-rw-r--r--   0     1001      123     2850 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/varcon-core/src/lib.rs
+-rw-r--r--   0     1001      123    16454 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/varcon-core/src/parser.rs
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 typos-1.16.0/local_dependencies/dictgen/Cargo.toml
+-rw-r--r--   0     1001      123      130 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/dictgen/src/lib.rs
+-rw-r--r--   0     1001      123     2687 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/dictgen/src/map.rs
+-rw-r--r--   0     1001      123     3726 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/dictgen/src/table.rs
+-rw-r--r--   0     1001      123    10637 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/dictgen/src/trie.rs
+-rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 typos-1.16.0/local_dependencies/typos-vars/Cargo.toml
+-rw-r--r--   0     1001      123      117 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/typos-vars/src/lib.rs
+-rw-r--r--   0     1001      123  6086180 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/typos-vars/src/vars_codegen.rs
+-rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 typos-1.16.0/local_dependencies/typos/Cargo.toml
+-rw-r--r--   0     1001      123     2794 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/typos/src/check.rs
+-rw-r--r--   0     1001      123     2175 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/typos/src/dict.rs
+-rw-r--r--   0     1001      123       74 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/typos/src/lib.rs
+-rw-r--r--   0     1001      123    44720 2023-07-10 15:05:23.000000 typos-1.16.0/local_dependencies/typos/src/tokens.rs
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 typos-1.16.0/pyproject.toml
+-rw-r--r--   0        0        0     3030 1970-01-01 00:00:00.000000 typos-1.16.0/rust_src/typos-cli/Cargo.toml
+-rw-r--r--   0     1001      123     2221 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/benches/checks.rs
+-rw-r--r--   0     1001      123     4586 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/benches/corrections.rs
+-rw-r--r--   0     1001      123     1347 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/benches/data.rs
+-rw-r--r--   0     1001      123     3306 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/benches/tokenize.rs
+-rw-r--r--   0     1001      123     8452 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/src/bin/typos-cli/args.rs
+-rw-r--r--   0     1001      123     9824 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/src/bin/typos-cli/main.rs
+-rw-r--r--   0     1001      123    12622 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/src/bin/typos-cli/report.rs
+-rw-r--r--   0     1001      123    21859 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/src/config.rs
+-rw-r--r--   0     1001      123    10240 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/src/default_types.rs
+-rw-r--r--   0     1001      123    11574 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/src/dict.rs
+-rw-r--r--   0     1001      123    32621 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/src/file.rs
+-rw-r--r--   0     1001      123     6791 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/src/file_type.rs
+-rw-r--r--   0     1001      123      299 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/src/lib.rs
+-rw-r--r--   0     1001      123    17558 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/src/policy.rs
+-rw-r--r--   0     1001      123     5561 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/src/report.rs
+-rw-r--r--   0     1001      123      207 2023-07-10 15:05:23.000000 typos-1.16.0/rust_src/typos-cli/tests/cmd/false-positives.in/README.md
+-rw-r--r--   0     1001      123    53454 2023-07-10 15:05:23.000000 typos-1.16.0/Cargo.lock
+-rw-r--r--   0        0        0     5371 1970-01-01 00:00:00.000000 typos-1.16.0/PKG-INFO
```

### Comparing `typos-1.15.9/local_dependencies/varcon-core/Cargo.toml` & `typos-1.16.0/local_dependencies/varcon-core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/local_dependencies/varcon-core/src/borrowed.rs` & `typos-1.16.0/local_dependencies/varcon-core/src/borrowed.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/local_dependencies/varcon-core/src/lib.rs` & `typos-1.16.0/local_dependencies/varcon-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/local_dependencies/varcon-core/src/parser.rs` & `typos-1.16.0/local_dependencies/varcon-core/src/parser.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/local_dependencies/typos-dict/Cargo.toml` & `typos-1.16.0/local_dependencies/typos-dict/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "typos-dict"
-version = "0.10.5"
+version = "0.10.6"
 description = "Source Code Spelling Correction"
 readme = "../../README.md"
 categories = ["development-tools", "text-processing"]
 keywords = ["development", "spelling"]
 license= "MIT OR Apache-2.0"
 repository= "https://github.com/crate-ci/typos"
 edition= "2021"
```

### Comparing `typos-1.15.9/local_dependencies/typos-dict/src/dict_codegen.rs` & `typos-1.16.0/local_dependencies/typos-dict/src/dict_codegen.rs`

 * *Files 0% similar despite different names*

```diff
@@ -839,14 +839,15 @@
         dictgen::InsensitiveStr::Ascii("kload"),
         dictgen::InsensitiveStr::Ascii("kloads"),
         dictgen::InsensitiveStr::Ascii("ks"),
         dictgen::InsensitiveStr::Ascii("n"),
         dictgen::InsensitiveStr::Ascii("nf"),
         dictgen::InsensitiveStr::Ascii("nly"),
         dictgen::InsensitiveStr::Ascii("nt"),
+        dictgen::InsensitiveStr::Ascii("rker"),
     ],
     values: &[
         &["word"],
         &["wrote"],
         &["wrong"],
         &["work"],
         &["worked"],
@@ -856,14 +857,15 @@
         &["workload"],
         &["workloads"],
         &["works"],
         &["wrong"],
         &["wrong"],
         &["wrongly"],
         &["wrong"],
+        &["worker"],
     ],
     range: 1..=6,
 };
 
 static WORD_WRN_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_WRN_CHILDREN),
     value: None,
@@ -1281,14 +1283,15 @@
         dictgen::InsensitiveStr::Ascii("bennches"),
         dictgen::InsensitiveStr::Ascii("bnech"),
         dictgen::InsensitiveStr::Ascii("bneches"),
         dictgen::InsensitiveStr::Ascii("boos"),
         dictgen::InsensitiveStr::Ascii("d"),
         dictgen::InsensitiveStr::Ascii("e"),
         dictgen::InsensitiveStr::Ascii("es"),
+        dictgen::InsensitiveStr::Ascii("faround"),
         dictgen::InsensitiveStr::Ascii("fore"),
         dictgen::InsensitiveStr::Ascii("fow"),
         dictgen::InsensitiveStr::Ascii("fows"),
         dictgen::InsensitiveStr::Ascii("froce"),
         dictgen::InsensitiveStr::Ascii("ign"),
         dictgen::InsensitiveStr::Ascii("ingest"),
         dictgen::InsensitiveStr::Ascii("ins"),
@@ -1341,14 +1344,15 @@
         &["workbenches"],
         &["workbench"],
         &["workbenches"],
         &["workbooks"],
         &["worked", "works"],
         &["work", "worked", "works"],
         &["works", "workers"],
+        &["workaround"],
         &["workforce"],
         &["workflow"],
         &["workflows"],
         &["workforce"],
         &["working"],
         &["workings"],
         &["workings"],
@@ -1419,17 +1423,24 @@
 
 pub static WORD_WORD_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("l"),
         dictgen::InsensitiveStr::Ascii("lview"),
         dictgen::InsensitiveStr::Ascii("lwide"),
         dictgen::InsensitiveStr::Ascii("pres"),
+        dictgen::InsensitiveStr::Ascii("presss"),
     ],
-    values: &[&["world"], &["worldview"], &["worldwide"], &["wordpress"]],
-    range: 1..=5,
+    values: &[
+        &["world"],
+        &["worldview"],
+        &["worldwide"],
+        &["wordpress"],
+        &["wordpress"],
+    ],
+    range: 1..=6,
 };
 
 static WORD_WORC_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_WORC_CHILDREN),
     value: None,
 };
 
@@ -2447,15 +2458,15 @@
     Some(&WORD_WHN_NODE),
     Some(&WORD_WHO_NODE),
     None,
     None,
     Some(&WORD_WHR_NODE),
     Some(&WORD_WHS_NODE),
     Some(&WORD_WHT_NODE),
-    None,
+    Some(&WORD_WHU_NODE),
     None,
     None,
     None,
     Some(&WORD_WHY_NODE),
     None,
 ];
 
@@ -2470,14 +2481,25 @@
         dictgen::InsensitiveStr::Ascii("th"),
         dictgen::InsensitiveStr::Ascii("thout"),
     ],
     values: &[&["what", "why"], &["with"], &["without"]],
     range: 1..=5,
 };
 
+static WORD_WHU_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
+    children: dictgen::DictTrieChild::Flat(&WORD_WHU_CHILDREN),
+    value: None,
+};
+
+pub static WORD_WHU_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
+    keys: &[dictgen::InsensitiveStr::Ascii("le")],
+    values: &[&["while", "whole"]],
+    range: 2..=2,
+};
+
 static WORD_WHT_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_WHT_CHILDREN),
     value: None,
 };
 
 pub static WORD_WHT_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
@@ -3121,15 +3143,15 @@
     keys: &[dictgen::InsensitiveStr::Ascii("e")],
     values: &[&["wedge"]],
     range: 1..=1,
 };
 
 static WORD_WEE_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_WEE_CHILDREN),
-    value: None,
+    value: Some(&["we"]),
 };
 
 pub static WORD_WEE_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("rd"),
         dictgen::InsensitiveStr::Ascii("rdly"),
         dictgen::InsensitiveStr::Ascii("v"),
@@ -3192,32 +3214,34 @@
     value: None,
 };
 
 pub static WORD_WEB_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("age"),
         dictgen::InsensitiveStr::Ascii("apge"),
+        dictgen::InsensitiveStr::Ascii("assemby"),
         dictgen::InsensitiveStr::Ascii("books"),
         dictgen::InsensitiveStr::Ascii("hools"),
         dictgen::InsensitiveStr::Ascii("iste"),
         dictgen::InsensitiveStr::Ascii("istes"),
         dictgen::InsensitiveStr::Ascii("stie"),
         dictgen::InsensitiveStr::Ascii("sties"),
     ],
     values: &[
         &["webpage"],
         &["webpage"],
+        &["webassembly"],
         &["webhooks"],
         &["webhooks"],
         &["website"],
         &["websites"],
         &["website"],
         &["websites"],
     ],
-    range: 3..=5,
+    range: 3..=7,
 };
 
 static WORD_WEA_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_WEA_CHILDREN),
     value: None,
 };
 
@@ -6544,14 +6568,15 @@
     children: dictgen::DictTrieChild::Flat(&WORD_VEC_CHILDREN),
     value: None,
 };
 
 pub static WORD_VEC_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("hiles"),
+        dictgen::InsensitiveStr::Ascii("otor"),
         dictgen::InsensitiveStr::Ascii("otr"),
         dictgen::InsensitiveStr::Ascii("otrs"),
         dictgen::InsensitiveStr::Ascii("tices"),
         dictgen::InsensitiveStr::Ascii("tore"),
         dictgen::InsensitiveStr::Ascii("tores"),
         dictgen::InsensitiveStr::Ascii("torss"),
         dictgen::InsensitiveStr::Ascii("tror"),
@@ -6559,14 +6584,15 @@
         dictgen::InsensitiveStr::Ascii("tros"),
         dictgen::InsensitiveStr::Ascii("vtor"),
         dictgen::InsensitiveStr::Ascii("vtors"),
     ],
     values: &[
         &["vehicles"],
         &["vector"],
+        &["vector"],
         &["vectors"],
         &["vertices"],
         &["vector"],
         &["vectors"],
         &["vectors"],
         &["vector"],
         &["vectors"],
@@ -9543,15 +9569,15 @@
 };
 
 pub static WORD_UNSA_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("ble"),
         dictgen::InsensitiveStr::Ascii("nfe"),
     ],
-    values: &[&["unusable", "usable", "unstable"], &["unsafe"]],
+    values: &[&["unusable", "usable", "unstable", "unable"], &["unsafe"]],
     range: 3..=3,
 };
 
 static WORD_UNR_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Nested(&WORD_UNR_CHILDREN),
     value: None,
 };
@@ -11189,14 +11215,15 @@
         dictgen::InsensitiveStr::Ascii("ortunatley"),
         dictgen::InsensitiveStr::Ascii("ortunatly"),
         dictgen::InsensitiveStr::Ascii("ortune"),
         dictgen::InsensitiveStr::Ascii("ortuneatly"),
         dictgen::InsensitiveStr::Ascii("ortunetely"),
         dictgen::InsensitiveStr::Ascii("ortunetly"),
         dictgen::InsensitiveStr::Ascii("ortuntaly"),
+        dictgen::InsensitiveStr::Ascii("ortuntely"),
         dictgen::InsensitiveStr::Ascii("orunate"),
         dictgen::InsensitiveStr::Ascii("orunately"),
         dictgen::InsensitiveStr::Ascii("orutunate"),
         dictgen::InsensitiveStr::Ascii("orutunately"),
         dictgen::InsensitiveStr::Ascii("otunately"),
         dictgen::InsensitiveStr::Ascii("ourtunately"),
         dictgen::InsensitiveStr::Ascii("ourtunetly"),
@@ -11242,14 +11269,15 @@
         &["unfortunately"],
         &["unfortunately"],
         &["unfortunate"],
         &["unfortunately"],
         &["unfortunately"],
         &["unfortunately"],
         &["unfortunately"],
+        &["unfortunately"],
         &["unfortunate"],
         &["unfortunately"],
         &["unfortunate"],
         &["unfortunately"],
         &["unfortunately"],
         &["unfortunately"],
         &["unfortunately"],
@@ -13259,15 +13287,15 @@
 
 static WORD_UNA_CHILDREN: [Option<&dictgen::DictTrieNode<&'static [&'static str]>>; 26] = [
     None,
     Some(&WORD_UNAB_NODE),
     Some(&WORD_UNAC_NODE),
     Some(&WORD_UNAD_NODE),
     None,
-    None,
+    Some(&WORD_UNAF_NODE),
     None,
     Some(&WORD_UNAH_NODE),
     None,
     None,
     None,
     Some(&WORD_UNAL_NODE),
     Some(&WORD_UNAM_NODE),
@@ -13557,32 +13585,44 @@
 static WORD_UNAL_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_UNAL_CHILDREN),
     value: None,
 };
 
 pub static WORD_UNAL_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
+        dictgen::InsensitiveStr::Ascii("be"),
         dictgen::InsensitiveStr::Ascii("e"),
         dictgen::InsensitiveStr::Ascii("llowed"),
     ],
-    values: &[&["unable"], &["unallowed"]],
+    values: &[&["unable"], &["unable"], &["unallowed"]],
     range: 1..=6,
 };
 
 static WORD_UNAH_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_UNAH_CHILDREN),
     value: None,
 };
 
 pub static WORD_UNAH_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[dictgen::InsensitiveStr::Ascii("ppy")],
     values: &[&["unhappy"]],
     range: 3..=3,
 };
 
+static WORD_UNAF_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
+    children: dictgen::DictTrieChild::Flat(&WORD_UNAF_CHILDREN),
+    value: None,
+};
+
+pub static WORD_UNAF_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
+    keys: &[dictgen::InsensitiveStr::Ascii("ected")],
+    values: &[&["unaffected"]],
+    range: 5..=5,
+};
+
 static WORD_UNAD_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_UNAD_CHILDREN),
     value: None,
 };
 
 pub static WORD_UNAD_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
@@ -14347,23 +14387,25 @@
     children: dictgen::DictTrieChild::Flat(&WORD_TUP_CHILDREN),
     value: None,
 };
 
 pub static WORD_TUP_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("el"),
+        dictgen::InsensitiveStr::Ascii("es"),
         dictgen::InsensitiveStr::Ascii("less"),
         dictgen::InsensitiveStr::Ascii("parware"),
         dictgen::InsensitiveStr::Ascii("perwears"),
         dictgen::InsensitiveStr::Ascii("ple"),
         dictgen::InsensitiveStr::Ascii("ples"),
     ],
     values: &[
         &["tuple"],
         &["tuples"],
+        &["tuples"],
         &["tupperware"],
         &["tupperware"],
         &["tuple"],
         &["tuples"],
     ],
     range: 2..=8,
 };
@@ -17621,14 +17663,15 @@
 static WORD_TRAI_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_TRAI_CHILDREN),
     value: None,
 };
 
 pub static WORD_TRAI_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
+        dictgen::InsensitiveStr::Ascii("ds"),
         dictgen::InsensitiveStr::Ascii("ge"),
         dictgen::InsensitiveStr::Ascii("ger"),
         dictgen::InsensitiveStr::Ascii("gers"),
         dictgen::InsensitiveStr::Ascii("ges"),
         dictgen::InsensitiveStr::Ascii("ging"),
         dictgen::InsensitiveStr::Ascii("ing"),
         dictgen::InsensitiveStr::Ascii("leras"),
@@ -17654,14 +17697,15 @@
         dictgen::InsensitiveStr::Ascii("nwreak"),
         dictgen::InsensitiveStr::Ascii("nwrek"),
         dictgen::InsensitiveStr::Ascii("toris"),
         dictgen::InsensitiveStr::Ascii("torus"),
         dictgen::InsensitiveStr::Ascii("tour"),
     ],
     values: &[
+        &["traits", "triads"],
         &["triage"],
         &["triager"],
         &["triagers"],
         &["triages"],
         &["triaging"],
         &["trailing", "training"],
         &["trailers"],
@@ -17839,20 +17883,21 @@
 static WORD_TP_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_TP_CHILDREN),
     value: None,
 };
 
 pub static WORD_TP_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
+        dictgen::InsensitiveStr::Ascii("os"),
         dictgen::InsensitiveStr::Ascii("ye"),
         dictgen::InsensitiveStr::Ascii("yed"),
         dictgen::InsensitiveStr::Ascii("yes"),
         dictgen::InsensitiveStr::Ascii("yo"),
     ],
-    values: &[&["type"], &["typed"], &["types"], &["typo"]],
+    values: &[&["typos"], &["type"], &["typed"], &["types"], &["typo"]],
     range: 2..=3,
 };
 
 static WORD_TO_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Nested(&WORD_TO_CHILDREN),
     value: None,
 };
@@ -18273,20 +18318,27 @@
 static WORD_TON_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_TON_CHILDREN),
     value: None,
 };
 
 pub static WORD_TON_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
+        dictgen::InsensitiveStr::Ascii("ange"),
         dictgen::InsensitiveStr::Ascii("giht"),
         dictgen::InsensitiveStr::Ascii("guers"),
         dictgen::InsensitiveStr::Ascii("ihgt"),
         dictgen::InsensitiveStr::Ascii("uges"),
     ],
-    values: &[&["tonight"], &["tongues"], &["tonight"], &["tongues"]],
+    values: &[
+        &["tonnage"],
+        &["tonight"],
+        &["tongues"],
+        &["tonight"],
+        &["tongues"],
+    ],
     range: 4..=5,
 };
 
 static WORD_TOM_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_TOM_CHILDREN),
     value: None,
 };
@@ -18313,14 +18365,15 @@
     children: dictgen::DictTrieChild::Flat(&WORD_TOL_CHILDREN),
     value: None,
 };
 
 pub static WORD_TOL_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("arable"),
+        dictgen::InsensitiveStr::Ascii("earnce"),
         dictgen::InsensitiveStr::Ascii("elerance"),
         dictgen::InsensitiveStr::Ascii("en"),
         dictgen::InsensitiveStr::Ascii("ens"),
         dictgen::InsensitiveStr::Ascii("erabe"),
         dictgen::InsensitiveStr::Ascii("eranz"),
         dictgen::InsensitiveStr::Ascii("erence"),
         dictgen::InsensitiveStr::Ascii("erences"),
@@ -18335,14 +18388,15 @@
         dictgen::InsensitiveStr::Ascii("orance"),
         dictgen::InsensitiveStr::Ascii("orances"),
         dictgen::InsensitiveStr::Ascii("orant"),
     ],
     values: &[
         &["tolerable"],
         &["tolerance"],
+        &["tolerance"],
         &["token"],
         &["tokens"],
         &["tolerable"],
         &["tolerance"],
         &["tolerance"],
         &["tolerances"],
         &["tolerant"],
@@ -20495,14 +20549,15 @@
         dictgen::InsensitiveStr::Ascii("cases"),
         dictgen::InsensitiveStr::Ascii("e"),
         dictgen::InsensitiveStr::Ascii("ed"),
         dictgen::InsensitiveStr::Ascii("ellate"),
         dictgen::InsensitiveStr::Ascii("ellated"),
         dictgen::InsensitiveStr::Ascii("ellation"),
         dictgen::InsensitiveStr::Ascii("ellator"),
+        dictgen::InsensitiveStr::Ascii("ing"),
         dictgen::InsensitiveStr::Ascii("itcle"),
         dictgen::InsensitiveStr::Ascii("itcles"),
         dictgen::InsensitiveStr::Ascii("ited"),
         dictgen::InsensitiveStr::Ascii("itfy"),
         dictgen::InsensitiveStr::Ascii("itmony"),
         dictgen::InsensitiveStr::Ascii("sealte"),
         dictgen::InsensitiveStr::Ascii("sealted"),
@@ -20526,25 +20581,27 @@
         dictgen::InsensitiveStr::Ascii("ticlular"),
         dictgen::InsensitiveStr::Ascii("tifiy"),
         dictgen::InsensitiveStr::Ascii("tiing"),
         dictgen::InsensitiveStr::Ascii("timoney"),
         dictgen::InsensitiveStr::Ascii("tin"),
         dictgen::InsensitiveStr::Ascii("tng"),
         dictgen::InsensitiveStr::Ascii("tomony"),
+        dictgen::InsensitiveStr::Ascii("tsdata"),
         dictgen::InsensitiveStr::Ascii("tsing"),
     ],
     values: &[
         &["testcase"],
         &["testcases"],
         &["these", "tease", "terse"],
         &["used", "teased", "tested"],
         &["tessellate"],
         &["tessellated"],
         &["tessellation"],
         &["tessellator"],
+        &["testing"],
         &["testicle"],
         &["testicles"],
         &["tested"],
         &["testify"],
         &["testimony"],
         &["tessellate"],
         &["tessellated"],
@@ -20568,14 +20625,15 @@
         &["testicular"],
         &["testify"],
         &["testing"],
         &["testimony"],
         &["testing"],
         &["testing"],
         &["testimony"],
+        &["testdata"],
         &["testing"],
     ],
     range: 1..=9,
 };
 
 static WORD_TER_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Nested(&WORD_TER_CHILDREN),
@@ -20814,14 +20872,15 @@
         dictgen::InsensitiveStr::Ascii("niates"),
         dictgen::InsensitiveStr::Ascii("niating"),
         dictgen::InsensitiveStr::Ascii("niation"),
         dictgen::InsensitiveStr::Ascii("niations"),
         dictgen::InsensitiveStr::Ascii("niator"),
         dictgen::InsensitiveStr::Ascii("niators"),
         dictgen::InsensitiveStr::Ascii("o"),
+        dictgen::InsensitiveStr::Ascii("onology"),
         dictgen::InsensitiveStr::Ascii("ostat"),
         dictgen::InsensitiveStr::Ascii("peratue"),
         dictgen::InsensitiveStr::Ascii("peratues"),
         dictgen::InsensitiveStr::Ascii("perature"),
         dictgen::InsensitiveStr::Ascii("peratures"),
         dictgen::InsensitiveStr::Ascii("plate"),
         dictgen::InsensitiveStr::Ascii("plated"),
@@ -20875,14 +20934,15 @@
         &["terminates"],
         &["terminating"],
         &["termination"],
         &["terminations"],
         &["terminator"],
         &["terminators"],
         &["thermo"],
+        &["terminology"],
         &["thermostat"],
         &["temperature"],
         &["temperatures"],
         &["temperature"],
         &["temperatures"],
         &["template"],
         &["templated"],
@@ -29721,17 +29781,18 @@
     value: None,
 };
 
 pub static WORD_STD_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("anard"),
         dictgen::InsensitiveStr::Ascii("anards"),
+        dictgen::InsensitiveStr::Ascii("errr"),
     ],
-    values: &[&["standard"], &["standards"]],
-    range: 5..=6,
+    values: &[&["standard"], &["standards"], &["stderr"]],
+    range: 4..=6,
 };
 
 static WORD_STC_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_STC_CHILDREN),
     value: None,
 };
 
@@ -30481,14 +30542,15 @@
     children: dictgen::DictTrieChild::Flat(&WORD_STAB_CHILDREN),
     value: None,
 };
 
 pub static WORD_STAB_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("alization"),
+        dictgen::InsensitiveStr::Ascii("alized"),
         dictgen::InsensitiveStr::Ascii("el"),
         dictgen::InsensitiveStr::Ascii("elized"),
         dictgen::InsensitiveStr::Ascii("ilitation"),
         dictgen::InsensitiveStr::Ascii("ilite"),
         dictgen::InsensitiveStr::Ascii("ilited"),
         dictgen::InsensitiveStr::Ascii("ilites"),
         dictgen::InsensitiveStr::Ascii("iliting"),
@@ -30503,14 +30565,15 @@
         dictgen::InsensitiveStr::Ascii("lility"),
         dictgen::InsensitiveStr::Ascii("lilization"),
         dictgen::InsensitiveStr::Ascii("lize"),
         dictgen::InsensitiveStr::Ascii("lizied"),
     ],
     values: &[
         &["stabilization"],
+        &["stabilized"],
         &["stable"],
         &["stabilized"],
         &["stabilization"],
         &["stabilize"],
         &["stabilized"],
         &["stabilizes"],
         &["stabilizing"],
@@ -34732,117 +34795,135 @@
         &["move"],
         &["smtp", "smtpe"],
     ],
     range: 2..=9,
 };
 
 static WORD_SL_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
-    children: dictgen::DictTrieChild::Flat(&WORD_SL_CHILDREN),
+    children: dictgen::DictTrieChild::Nested(&WORD_SL_CHILDREN),
+    value: None,
+};
+
+static WORD_SL_CHILDREN: [Option<&dictgen::DictTrieNode<&'static [&'static str]>>; 26] = [
+    Some(&WORD_SLA_NODE),
+    None,
+    None,
+    Some(&WORD_SLD_NODE),
+    Some(&WORD_SLE_NODE),
+    None,
+    None,
+    None,
+    Some(&WORD_SLI_NODE),
+    None,
+    None,
+    None,
+    None,
+    None,
+    Some(&WORD_SLO_NODE),
+    None,
+    Some(&WORD_SLQ_NODE),
+    None,
+    None,
+    None,
+    Some(&WORD_SLU_NODE),
+    None,
+    None,
+    None,
+    None,
+    None,
+];
+
+static WORD_SLU_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
+    children: dictgen::DictTrieChild::Flat(&WORD_SLU_CHILDREN),
     value: None,
 };
 
-pub static WORD_SL_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
+pub static WORD_SLU_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
-        dictgen::InsensitiveStr::Ascii("ac"),
-        dictgen::InsensitiveStr::Ascii("ach"),
-        dictgen::InsensitiveStr::Ascii("aches"),
-        dictgen::InsensitiveStr::Ascii("anguage"),
-        dictgen::InsensitiveStr::Ascii("anguages"),
-        dictgen::InsensitiveStr::Ascii("aptoon"),
-        dictgen::InsensitiveStr::Ascii("ase"),
-        dictgen::InsensitiveStr::Ascii("ases"),
-        dictgen::InsensitiveStr::Ascii("ashs"),
-        dictgen::InsensitiveStr::Ascii("aughted"),
-        dictgen::InsensitiveStr::Ascii("aughterd"),
-        dictgen::InsensitiveStr::Ascii("augterhouses"),
-        dictgen::InsensitiveStr::Ascii("augther"),
-        dictgen::InsensitiveStr::Ascii("augthered"),
-        dictgen::InsensitiveStr::Ascii("augthering"),
-        dictgen::InsensitiveStr::Ascii("avage"),
-        dictgen::InsensitiveStr::Ascii("averly"),
-        dictgen::InsensitiveStr::Ascii("ayign"),
-        dictgen::InsensitiveStr::Ascii("diers"),
-        dictgen::InsensitiveStr::Ascii("ect"),
-        dictgen::InsensitiveStr::Ascii("ected"),
-        dictgen::InsensitiveStr::Ascii("ecting"),
-        dictgen::InsensitiveStr::Ascii("ection"),
-        dictgen::InsensitiveStr::Ascii("eect"),
-        dictgen::InsensitiveStr::Ascii("eeped"),
-        dictgen::InsensitiveStr::Ascii("eepp"),
-        dictgen::InsensitiveStr::Ascii("efies"),
-        dictgen::InsensitiveStr::Ascii("efishness"),
-        dictgen::InsensitiveStr::Ascii("ewth"),
-        dictgen::InsensitiveStr::Ascii("ewthed"),
-        dictgen::InsensitiveStr::Ascii("ewthing"),
-        dictgen::InsensitiveStr::Ascii("ewths"),
-        dictgen::InsensitiveStr::Ascii("icable"),
-        dictgen::InsensitiveStr::Ascii("ienced"),
-        dictgen::InsensitiveStr::Ascii("ient"),
-        dictgen::InsensitiveStr::Ascii("iently"),
-        dictgen::InsensitiveStr::Ascii("ighlty"),
-        dictgen::InsensitiveStr::Ascii("ighly"),
-        dictgen::InsensitiveStr::Ascii("ightl"),
-        dictgen::InsensitiveStr::Ascii("ighty"),
-        dictgen::InsensitiveStr::Ascii("ignt"),
-        dictgen::InsensitiveStr::Ascii("igntly"),
-        dictgen::InsensitiveStr::Ascii("igth"),
-        dictgen::InsensitiveStr::Ascii("igthly"),
-        dictgen::InsensitiveStr::Ascii("igtly"),
-        dictgen::InsensitiveStr::Ascii("iped"),
-        dictgen::InsensitiveStr::Ascii("ipperies"),
-        dictgen::InsensitiveStr::Ascii("ipperly"),
-        dictgen::InsensitiveStr::Ascii("ippes"),
-        dictgen::InsensitiveStr::Ascii("ippey"),
-        dictgen::InsensitiveStr::Ascii("iseshow"),
-        dictgen::InsensitiveStr::Ascii("ite"),
-        dictgen::InsensitiveStr::Ascii("ooth"),
-        dictgen::InsensitiveStr::Ascii("oothed"),
-        dictgen::InsensitiveStr::Ascii("oothing"),
-        dictgen::InsensitiveStr::Ascii("ooths"),
-        dictgen::InsensitiveStr::Ascii("oughtering"),
-        dictgen::InsensitiveStr::Ascii("owy"),
-        dictgen::InsensitiveStr::Ascii("q"),
-        dictgen::InsensitiveStr::Ascii("uaghter"),
-        dictgen::InsensitiveStr::Ascii("uaghtered"),
-        dictgen::InsensitiveStr::Ascii("uaghtering"),
-        dictgen::InsensitiveStr::Ascii("uggify"),
+        dictgen::InsensitiveStr::Ascii("aghter"),
+        dictgen::InsensitiveStr::Ascii("aghtered"),
+        dictgen::InsensitiveStr::Ascii("aghtering"),
+        dictgen::InsensitiveStr::Ascii("ggify"),
     ],
     values: &[
-        &["slack"],
-        &["slash"],
-        &["slashes"],
-        &["language"],
-        &["languages"],
-        &["splatoon"],
-        &["slash"],
-        &["slashes"],
-        &["slashes"],
-        &["slaughtered"],
-        &["slaughtered"],
-        &["slaughterhouses"],
         &["slaughter"],
         &["slaughtered"],
         &["slaughtering"],
-        &["salvage"],
-        &["slavery"],
-        &["slaying"],
-        &["sliders"],
-        &["select"],
-        &["selected"],
-        &["selecting"],
-        &["selection"],
-        &["select"],
-        &["slept"],
-        &["sleep"],
-        &["selfies"],
-        &["selfishness"],
-        &["sleuth"],
-        &["sleuthed"],
+        &["slugify"],
+    ],
+    range: 5..=9,
+};
+
+static WORD_SLQ_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
+    children: dictgen::DictTrieChild::Flat(&WORD_SLQ_CHILDREN),
+    value: Some(&["sql"]),
+};
+
+pub static WORD_SLQ_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
+    keys: &[],
+    values: &[],
+    range: 0..=0,
+};
+
+static WORD_SLO_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
+    children: dictgen::DictTrieChild::Flat(&WORD_SLO_CHILDREN),
+    value: None,
+};
+
+pub static WORD_SLO_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
+    keys: &[
+        dictgen::InsensitiveStr::Ascii("oth"),
+        dictgen::InsensitiveStr::Ascii("othed"),
+        dictgen::InsensitiveStr::Ascii("othing"),
+        dictgen::InsensitiveStr::Ascii("oths"),
+        dictgen::InsensitiveStr::Ascii("table"),
+        dictgen::InsensitiveStr::Ascii("ughtering"),
+        dictgen::InsensitiveStr::Ascii("wy"),
+    ],
+    values: &[
+        &["sleuth", "sloth", "sooth"],
+        &["sleuthing"],
         &["sleuthing"],
         &["sleuths"],
+        &["slottable"],
+        &["slaughtering"],
+        &["slowly"],
+    ],
+    range: 2..=9,
+};
+
+static WORD_SLI_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
+    children: dictgen::DictTrieChild::Flat(&WORD_SLI_CHILDREN),
+    value: None,
+};
+
+pub static WORD_SLI_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
+    keys: &[
+        dictgen::InsensitiveStr::Ascii("cable"),
+        dictgen::InsensitiveStr::Ascii("enced"),
+        dictgen::InsensitiveStr::Ascii("ent"),
+        dictgen::InsensitiveStr::Ascii("ently"),
+        dictgen::InsensitiveStr::Ascii("ghlty"),
+        dictgen::InsensitiveStr::Ascii("ghly"),
+        dictgen::InsensitiveStr::Ascii("ghtl"),
+        dictgen::InsensitiveStr::Ascii("ghty"),
+        dictgen::InsensitiveStr::Ascii("gnt"),
+        dictgen::InsensitiveStr::Ascii("gntly"),
+        dictgen::InsensitiveStr::Ascii("gth"),
+        dictgen::InsensitiveStr::Ascii("gthly"),
+        dictgen::InsensitiveStr::Ascii("gtly"),
+        dictgen::InsensitiveStr::Ascii("ped"),
+        dictgen::InsensitiveStr::Ascii("pperies"),
+        dictgen::InsensitiveStr::Ascii("pperly"),
+        dictgen::InsensitiveStr::Ascii("ppes"),
+        dictgen::InsensitiveStr::Ascii("ppey"),
+        dictgen::InsensitiveStr::Ascii("seshow"),
+        dictgen::InsensitiveStr::Ascii("te"),
+    ],
+    values: &[
         &["sliceable"],
         &["silenced"],
         &["silent"],
         &["silently"],
         &["slightly"],
         &["slightly"],
         &["slightly"],
@@ -34855,27 +34936,115 @@
         &["slipped"],
         &["slippers"],
         &["slippery"],
         &["slippers"],
         &["slippery"],
         &["slideshow"],
         &["elite", "site", "sleight", "slide"],
-        &["sleuth", "sloth", "sooth"],
-        &["sleuthing"],
+    ],
+    range: 2..=7,
+};
+
+static WORD_SLE_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
+    children: dictgen::DictTrieChild::Flat(&WORD_SLE_CHILDREN),
+    value: None,
+};
+
+pub static WORD_SLE_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
+    keys: &[
+        dictgen::InsensitiveStr::Ascii("ct"),
+        dictgen::InsensitiveStr::Ascii("cted"),
+        dictgen::InsensitiveStr::Ascii("cting"),
+        dictgen::InsensitiveStr::Ascii("ction"),
+        dictgen::InsensitiveStr::Ascii("ect"),
+        dictgen::InsensitiveStr::Ascii("eped"),
+        dictgen::InsensitiveStr::Ascii("epp"),
+        dictgen::InsensitiveStr::Ascii("fies"),
+        dictgen::InsensitiveStr::Ascii("fishness"),
+        dictgen::InsensitiveStr::Ascii("wth"),
+        dictgen::InsensitiveStr::Ascii("wthed"),
+        dictgen::InsensitiveStr::Ascii("wthing"),
+        dictgen::InsensitiveStr::Ascii("wths"),
+    ],
+    values: &[
+        &["select"],
+        &["selected"],
+        &["selecting"],
+        &["selection"],
+        &["select"],
+        &["slept"],
+        &["sleep"],
+        &["selfies"],
+        &["selfishness"],
+        &["sleuth"],
+        &["sleuthed"],
         &["sleuthing"],
         &["sleuths"],
-        &["slaughtering"],
-        &["slowly"],
-        &["sql"],
+    ],
+    range: 2..=8,
+};
+
+static WORD_SLD_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
+    children: dictgen::DictTrieChild::Flat(&WORD_SLD_CHILDREN),
+    value: None,
+};
+
+pub static WORD_SLD_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
+    keys: &[dictgen::InsensitiveStr::Ascii("iers")],
+    values: &[&["sliders"]],
+    range: 4..=4,
+};
+
+static WORD_SLA_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
+    children: dictgen::DictTrieChild::Flat(&WORD_SLA_CHILDREN),
+    value: None,
+};
+
+pub static WORD_SLA_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
+    keys: &[
+        dictgen::InsensitiveStr::Ascii("c"),
+        dictgen::InsensitiveStr::Ascii("ch"),
+        dictgen::InsensitiveStr::Ascii("ches"),
+        dictgen::InsensitiveStr::Ascii("nguage"),
+        dictgen::InsensitiveStr::Ascii("nguages"),
+        dictgen::InsensitiveStr::Ascii("ptoon"),
+        dictgen::InsensitiveStr::Ascii("se"),
+        dictgen::InsensitiveStr::Ascii("ses"),
+        dictgen::InsensitiveStr::Ascii("shs"),
+        dictgen::InsensitiveStr::Ascii("ughted"),
+        dictgen::InsensitiveStr::Ascii("ughterd"),
+        dictgen::InsensitiveStr::Ascii("ugterhouses"),
+        dictgen::InsensitiveStr::Ascii("ugther"),
+        dictgen::InsensitiveStr::Ascii("ugthered"),
+        dictgen::InsensitiveStr::Ascii("ugthering"),
+        dictgen::InsensitiveStr::Ascii("vage"),
+        dictgen::InsensitiveStr::Ascii("verly"),
+        dictgen::InsensitiveStr::Ascii("yign"),
+    ],
+    values: &[
+        &["slack"],
+        &["slash"],
+        &["slashes"],
+        &["language"],
+        &["languages"],
+        &["splatoon"],
+        &["slash"],
+        &["slashes"],
+        &["slashes"],
+        &["slaughtered"],
+        &["slaughtered"],
+        &["slaughterhouses"],
         &["slaughter"],
         &["slaughtered"],
         &["slaughtering"],
-        &["slugify"],
+        &["salvage"],
+        &["slavery"],
+        &["slaying"],
     ],
-    range: 1..=12,
+    range: 1..=11,
 };
 
 static WORD_SK_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Nested(&WORD_SK_CHILDREN),
     value: None,
 };
 
@@ -40243,14 +40412,16 @@
         dictgen::InsensitiveStr::Ascii("ault"),
         dictgen::InsensitiveStr::Ascii("aults"),
         dictgen::InsensitiveStr::Ascii("egrated"),
         dictgen::InsensitiveStr::Ascii("ement"),
         dictgen::InsensitiveStr::Ascii("ementation"),
         dictgen::InsensitiveStr::Ascii("emented"),
         dictgen::InsensitiveStr::Ascii("ements"),
+        dictgen::InsensitiveStr::Ascii("emnt"),
+        dictgen::InsensitiveStr::Ascii("emntation"),
         dictgen::InsensitiveStr::Ascii("emnts"),
         dictgen::InsensitiveStr::Ascii("ergation"),
         dictgen::InsensitiveStr::Ascii("fualt"),
         dictgen::InsensitiveStr::Ascii("fualts"),
         dictgen::InsensitiveStr::Ascii("mantation"),
         dictgen::InsensitiveStr::Ascii("mend"),
         dictgen::InsensitiveStr::Ascii("mendation"),
@@ -40264,14 +40435,15 @@
         dictgen::InsensitiveStr::Ascii("menst"),
         dictgen::InsensitiveStr::Ascii("mentaion"),
         dictgen::InsensitiveStr::Ascii("mente"),
         dictgen::InsensitiveStr::Ascii("mentes"),
         dictgen::InsensitiveStr::Ascii("metn"),
         dictgen::InsensitiveStr::Ascii("metned"),
         dictgen::InsensitiveStr::Ascii("metns"),
+        dictgen::InsensitiveStr::Ascii("mnet"),
         dictgen::InsensitiveStr::Ascii("ragated"),
         dictgen::InsensitiveStr::Ascii("ragation"),
         dictgen::InsensitiveStr::Ascii("regacion"),
         dictgen::InsensitiveStr::Ascii("regaded"),
         dictgen::InsensitiveStr::Ascii("regatie"),
         dictgen::InsensitiveStr::Ascii("retated"),
         dictgen::InsensitiveStr::Ascii("retation"),
@@ -40287,14 +40459,16 @@
         &["segfault"],
         &["segfaults"],
         &["segregated"],
         &["segment"],
         &["segmentation"],
         &["segmented"],
         &["segments"],
+        &["segment"],
+        &["segmentation"],
         &["segments"],
         &["segregation"],
         &["segfault"],
         &["segfaults"],
         &["segmentation"],
         &["segment"],
         &["segmentation"],
@@ -40308,14 +40482,15 @@
         &["segments"],
         &["segmentation"],
         &["segment"],
         &["segments"],
         &["segment"],
         &["segmented"],
         &["segments"],
+        &["segment"],
         &["segregated"],
         &["segregation"],
         &["segregation"],
         &["segregated"],
         &["segregated"],
         &["segregated"],
         &["segregation"],
@@ -43107,14 +43282,15 @@
         dictgen::InsensitiveStr::Ascii("gters"),
         dictgen::InsensitiveStr::Ascii("idmentary"),
         dictgen::InsensitiveStr::Ascii("lebok"),
         dictgen::InsensitiveStr::Ascii("leboook"),
         dictgen::InsensitiveStr::Ascii("lle"),
         dictgen::InsensitiveStr::Ascii("matic"),
         dictgen::InsensitiveStr::Ascii("morus"),
+        dictgen::InsensitiveStr::Ascii("mtime"),
         dictgen::InsensitiveStr::Ascii("muors"),
         dictgen::InsensitiveStr::Ascii("ning"),
         dictgen::InsensitiveStr::Ascii("nn"),
         dictgen::InsensitiveStr::Ascii("nned"),
         dictgen::InsensitiveStr::Ascii("nnging"),
         dictgen::InsensitiveStr::Ascii("nnig"),
         dictgen::InsensitiveStr::Ascii("nnign"),
@@ -43149,14 +43325,15 @@
         &["rutgers"],
         &["rudimentary"],
         &["rulebook"],
         &["rulebook"],
         &["rule"],
         &["rheumatic"],
         &["rumors"],
+        &["runtime"],
         &["rumors"],
         &["running", "ruining"],
         &["run"],
         &["ran", "run", "ruined"],
         &["running", "rummaging"],
         &["running"],
         &["running"],
@@ -45576,14 +45753,16 @@
         dictgen::InsensitiveStr::Ascii("rrektion"),
         dictgen::InsensitiveStr::Ascii("rse"),
         dictgen::InsensitiveStr::Ascii("rsive"),
         dictgen::InsensitiveStr::Ascii("rsively"),
         dictgen::InsensitiveStr::Ascii("se"),
         dictgen::InsensitiveStr::Ascii("sed"),
         dictgen::InsensitiveStr::Ascii("t"),
+        dictgen::InsensitiveStr::Ascii("tl"),
+        dictgen::InsensitiveStr::Ascii("tls"),
         dictgen::InsensitiveStr::Ascii("ts"),
     ],
     values: &[
         &["reusable"],
         &["reusables"],
         &["resubstitution"],
         &["rescued"],
@@ -45623,14 +45802,16 @@
         &["resurrection"],
         &["recurse", "resource"],
         &["recursive", "resourceful"],
         &["recursively"],
         &["reuse"],
         &["reused", "refused", "resumed"],
         &["result"],
+        &["result"],
+        &["results"],
         &["results"],
     ],
     range: 1..=9,
 };
 
 static WORD_REST_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Nested(&WORD_REST_CHILDREN),
@@ -47488,14 +47669,15 @@
         dictgen::InsensitiveStr::Ascii("eum"),
         dictgen::InsensitiveStr::Ascii("lme"),
         dictgen::InsensitiveStr::Ascii("me"),
         dictgen::InsensitiveStr::Ascii("rd"),
         dictgen::InsensitiveStr::Ascii("reing"),
         dictgen::InsensitiveStr::Ascii("remenet"),
         dictgen::InsensitiveStr::Ascii("remenets"),
+        dictgen::InsensitiveStr::Ascii("remenht"),
         dictgen::InsensitiveStr::Ascii("remnt"),
         dictgen::InsensitiveStr::Ascii("rment"),
         dictgen::InsensitiveStr::Ascii("rmentes"),
         dictgen::InsensitiveStr::Ascii("rments"),
         dictgen::InsensitiveStr::Ascii("sit"),
         dictgen::InsensitiveStr::Ascii("sits"),
     ],
@@ -47521,14 +47703,15 @@
         &["requiem"],
         &["required"],
         &["requiring"],
         &["requirement"],
         &["requirements"],
         &["requirement"],
         &["requirement"],
+        &["requirement"],
         &["requirements"],
         &["requirements"],
         &["requisite"],
         &["requisites"],
     ],
     range: 2..=8,
 };
@@ -55370,14 +55553,15 @@
     value: None,
 };
 
 pub static WORD_RECA_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("hed"),
         dictgen::InsensitiveStr::Ascii("l"),
+        dictgen::InsensitiveStr::Ascii("lcelated"),
         dictgen::InsensitiveStr::Ascii("lcualte"),
         dictgen::InsensitiveStr::Ascii("lcualted"),
         dictgen::InsensitiveStr::Ascii("lcualtes"),
         dictgen::InsensitiveStr::Ascii("lcualting"),
         dictgen::InsensitiveStr::Ascii("lcualtion"),
         dictgen::InsensitiveStr::Ascii("lcualtions"),
         dictgen::InsensitiveStr::Ascii("lcuate"),
@@ -55393,14 +55577,15 @@
         dictgen::InsensitiveStr::Ascii("ngle"),
         dictgen::InsensitiveStr::Ascii("ngles"),
         dictgen::InsensitiveStr::Ascii("tions"),
     ],
     values: &[
         &["reached"],
         &["recall"],
+        &["recalculated"],
         &["recalculate"],
         &["recalculated"],
         &["recalculates"],
         &["recalculating"],
         &["recalculation"],
         &["recalculations"],
         &["recalculate"],
@@ -55976,15 +56161,15 @@
         &["relation", "reaction"],
         &["relations", "reactions"],
         &["relationships"],
         &["relative", "reactive"],
         &["relatively"],
         &["relatives"],
         &["relativity"],
-        &["really", "relay"],
+        &["really", "relay", "real"],
         &["really"],
     ],
     range: 1..=10,
 };
 
 static WORD_REAK_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_REAK_CHILDREN),
@@ -58629,17 +58814,20 @@
 
 static WORD_PRV_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_PRV_CHILDREN),
     value: None,
 };
 
 pub static WORD_PRV_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
-    keys: &[dictgen::InsensitiveStr::Ascii("iate")],
-    values: &[&["private"]],
-    range: 4..=4,
+    keys: &[
+        dictgen::InsensitiveStr::Ascii("iate"),
+        dictgen::InsensitiveStr::Ascii("ode"),
+    ],
+    values: &[&["private"], &["provide"]],
+    range: 3..=4,
 };
 
 static WORD_PRU_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_PRU_CHILDREN),
     value: None,
 };
 
@@ -60015,17 +60203,20 @@
 
 static WORD_PROPG_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_PROPG_CHILDREN),
     value: None,
 };
 
 pub static WORD_PROPG_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
-    keys: &[dictgen::InsensitiveStr::Ascii("ated")],
-    values: &[&["propagated"]],
-    range: 4..=4,
+    keys: &[
+        dictgen::InsensitiveStr::Ascii("ated"),
+        dictgen::InsensitiveStr::Ascii("ating"),
+    ],
+    values: &[&["propagated"], &["propagating"]],
+    range: 4..=5,
 };
 
 static WORD_PROPE_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_PROPE_CHILDREN),
     value: None,
 };
 
@@ -60376,18 +60567,20 @@
         dictgen::InsensitiveStr::Ascii("iscuos"),
         dictgen::InsensitiveStr::Ascii("iscus"),
         dictgen::InsensitiveStr::Ascii("iss"),
         dictgen::InsensitiveStr::Ascii("isse"),
         dictgen::InsensitiveStr::Ascii("issed"),
         dictgen::InsensitiveStr::Ascii("isses"),
         dictgen::InsensitiveStr::Ascii("issing"),
+        dictgen::InsensitiveStr::Ascii("itives"),
         dictgen::InsensitiveStr::Ascii("ixity"),
         dictgen::InsensitiveStr::Ascii("mpt"),
         dictgen::InsensitiveStr::Ascii("mpts"),
         dictgen::InsensitiveStr::Ascii("ocional"),
+        dictgen::InsensitiveStr::Ascii("ordials"),
         dictgen::InsensitiveStr::Ascii("ose"),
         dictgen::InsensitiveStr::Ascii("oteurs"),
         dictgen::InsensitiveStr::Ascii("otheus"),
         dictgen::InsensitiveStr::Ascii("otinal"),
         dictgen::InsensitiveStr::Ascii("otionnal"),
         dictgen::InsensitiveStr::Ascii("ots"),
         dictgen::InsensitiveStr::Ascii("otted"),
@@ -60439,18 +60632,20 @@
         &["promiscuous"],
         &["promiscuous"],
         &["promise"],
         &["promise", "promises", "promised"],
         &["promised"],
         &["promises"],
         &["promising"],
+        &["primitives"],
         &["proximity"],
         &["prompt"],
         &["prompts"],
         &["promotional"],
+        &["primordials"],
         &["promotes"],
         &["promotes"],
         &["prometheus"],
         &["promotional"],
         &["promotional"],
         &["promotes"],
         &["promoted"],
@@ -62647,14 +62842,15 @@
         dictgen::InsensitiveStr::Ascii("itiv"),
         dictgen::InsensitiveStr::Ascii("itve"),
         dictgen::InsensitiveStr::Ascii("itves"),
         dictgen::InsensitiveStr::Ascii("ive"),
         dictgen::InsensitiveStr::Ascii("ordal"),
         dictgen::InsensitiveStr::Ascii("tiive"),
         dictgen::InsensitiveStr::Ascii("tive"),
+        dictgen::InsensitiveStr::Ascii("tives"),
     ],
     values: &[
         &["primaries"],
         &["primarily"],
         &["primary"],
         &["primarily"],
         &["primarily"],
@@ -62672,14 +62868,15 @@
         &["primitive"],
         &["primitive"],
         &["primitives"],
         &["primitive"],
         &["primordial"],
         &["primitive"],
         &["primitive"],
+        &["primitives"],
     ],
     range: 2..=7,
 };
 
 static WORD_PRIE_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_PRIE_CHILDREN),
     value: None,
@@ -63774,26 +63971,28 @@
     children: dictgen::DictTrieChild::Flat(&WORD_PREO_CHILDREN),
     value: None,
 };
 
 pub static WORD_PREO_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("cess"),
+        dictgen::InsensitiveStr::Ascii("cessing"),
         dictgen::InsensitiveStr::Ascii("cupation"),
         dictgen::InsensitiveStr::Ascii("perty"),
         dictgen::InsensitiveStr::Ascii("rded"),
         dictgen::InsensitiveStr::Ascii("rderd"),
         dictgen::InsensitiveStr::Ascii("rderded"),
         dictgen::InsensitiveStr::Ascii("rderers"),
         dictgen::InsensitiveStr::Ascii("rderes"),
         dictgen::InsensitiveStr::Ascii("rdes"),
         dictgen::InsensitiveStr::Ascii("xide"),
     ],
     values: &[
         &["process"],
+        &["processing", "preprocessing"],
         &["preoccupation"],
         &["property"],
         &["preordered"],
         &["preordered"],
         &["preordered"],
         &["preorders"],
         &["preorders"],
@@ -64427,14 +64626,15 @@
         dictgen::InsensitiveStr::Ascii("catble"),
         dictgen::InsensitiveStr::Ascii("ccion"),
         dictgen::InsensitiveStr::Ascii("cement"),
         dictgen::InsensitiveStr::Ascii("cessor"),
         dictgen::InsensitiveStr::Ascii("cessors"),
         dictgen::InsensitiveStr::Ascii("ceted"),
         dictgen::InsensitiveStr::Ascii("ciment"),
+        dictgen::InsensitiveStr::Ascii("ciotn"),
         dictgen::InsensitiveStr::Ascii("cited"),
         dictgen::InsensitiveStr::Ascii("citng"),
         dictgen::InsensitiveStr::Ascii("citon"),
         dictgen::InsensitiveStr::Ascii("citons"),
         dictgen::InsensitiveStr::Ascii("citve"),
         dictgen::InsensitiveStr::Ascii("ckted"),
         dictgen::InsensitiveStr::Ascii("ctave"),
@@ -64455,22 +64655,23 @@
         &["predictable"],
         &["prediction"],
         &["predicament"],
         &["predecessor"],
         &["predecessors"],
         &["predicated"],
         &["predicament"],
+        &["prediction"],
         &["predicated"],
         &["predicting"],
         &["prediction"],
         &["predictions"],
         &["predictive"],
         &["predicated"],
         &["predictive"],
-        &["predictive"],
+        &["predictive", "predicted"],
         &["predictable"],
         &["predictive"],
         &["prediction"],
         &["predictions"],
         &["prediction"],
         &["predicament"],
         &["predictions"],
@@ -65302,20 +65503,22 @@
 static WORD_POU_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_POU_CHILDREN),
     value: None,
 };
 
 pub static WORD_POU_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
+        dictgen::InsensitiveStr::Ascii("late"),
         dictgen::InsensitiveStr::Ascii("lations"),
         dictgen::InsensitiveStr::Ascii("nt"),
         dictgen::InsensitiveStr::Ascii("nts"),
         dictgen::InsensitiveStr::Ascii("pular"),
     ],
     values: &[
+        &["populate"],
         &["populations"],
         &["point", "pound"],
         &["points"],
         &["popular"],
     ],
     range: 2..=7,
 };
@@ -66448,15 +66651,15 @@
     Some(&WORD_POLI_NODE),
     None,
     None,
     Some(&WORD_POLL_NODE),
     None,
     None,
     Some(&WORD_POLO_NODE),
-    None,
+    Some(&WORD_POLP_NODE),
     None,
     None,
     None,
     Some(&WORD_POLT_NODE),
     Some(&WORD_POLU_NODE),
     None,
     None,
@@ -66560,14 +66763,25 @@
         &["politically"],
         &["politics"],
         &["poultry"],
     ],
     range: 2..=6,
 };
 
+static WORD_POLP_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
+    children: dictgen::DictTrieChild::Flat(&WORD_POLP_CHILDREN),
+    value: None,
+};
+
+pub static WORD_POLP_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
+    keys: &[dictgen::InsensitiveStr::Ascii("ulate")],
+    values: &[&["populate"]],
+    range: 5..=5,
+};
+
 static WORD_POLO_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_POLO_CHILDREN),
     value: None,
 };
 
 pub static WORD_POLO_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
@@ -66800,14 +67014,15 @@
 pub static WORD_POI_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("cies"),
         dictgen::InsensitiveStr::Ascii("cy"),
         dictgen::InsensitiveStr::Ascii("gnat"),
         dictgen::InsensitiveStr::Ascii("int"),
         dictgen::InsensitiveStr::Ascii("ints"),
+        dictgen::InsensitiveStr::Ascii("n"),
         dictgen::InsensitiveStr::Ascii("nd"),
         dictgen::InsensitiveStr::Ascii("ndcloud"),
         dictgen::InsensitiveStr::Ascii("neer"),
         dictgen::InsensitiveStr::Ascii("ner"),
         dictgen::InsensitiveStr::Ascii("ng"),
         dictgen::InsensitiveStr::Ascii("ngant"),
         dictgen::InsensitiveStr::Ascii("nits"),
@@ -66863,14 +67078,15 @@
     values: &[
         &["policies"],
         &["policy"],
         &["poignant"],
         &["point"],
         &["points"],
         &["point"],
+        &["point"],
         &["pointcloud"],
         &["pioneer"],
         &["pointer"],
         &["point"],
         &["poignant"],
         &["points"],
         &["pointer"],
@@ -71149,18 +71365,19 @@
     children: dictgen::DictTrieChild::Flat(&WORD_PENT_CHILDREN),
     value: None,
 };
 
 pub static WORD_PENT_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("agoon"),
+        dictgen::InsensitiveStr::Ascii("alty"),
         dictgen::InsensitiveStr::Ascii("sylvania"),
         dictgen::InsensitiveStr::Ascii("uim"),
     ],
-    values: &[&["pentagon"], &["pennsylvania"], &["pentium"]],
+    values: &[&["pentagon"], &["penalty"], &["pennsylvania"], &["pentium"]],
     range: 3..=8,
 };
 
 static WORD_PENS_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_PENS_CHILDREN),
     value: None,
 };
@@ -73627,27 +73844,29 @@
 pub static WORD_PARAR_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("agraph"),
         dictgen::InsensitiveStr::Ascii("aph"),
         dictgen::InsensitiveStr::Ascii("eter"),
         dictgen::InsensitiveStr::Ascii("gaph"),
         dictgen::InsensitiveStr::Ascii("gaphs"),
+        dictgen::InsensitiveStr::Ascii("m"),
         dictgen::InsensitiveStr::Ascii("meter"),
         dictgen::InsensitiveStr::Ascii("meters"),
     ],
     values: &[
         &["paragraph"],
         &["paragraph"],
         &["parameter"],
         &["paragraph"],
         &["paragraphs"],
+        &["param"],
         &["parameter"],
         &["parameters"],
     ],
-    range: 3..=6,
+    range: 1..=6,
 };
 
 static WORD_PARAP_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_PARAP_CHILDREN),
     value: None,
 };
 
@@ -74848,15 +75067,15 @@
         &["overwrite"],
     ],
     range: 3..=8,
 };
 
 static WORD_OVE_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Nested(&WORD_OVE_CHILDREN),
-    value: None,
+    value: Some(&["oven", "over"]),
 };
 
 static WORD_OVE_CHILDREN: [Option<&dictgen::DictTrieNode<&'static [&'static str]>>; 26] = [
     None,
     None,
     None,
     None,
@@ -77735,18 +77954,20 @@
     value: None,
 };
 
 pub static WORD_OPU_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("late"),
         dictgen::InsensitiveStr::Ascii("lates"),
+        dictgen::InsensitiveStr::Ascii("tput"),
     ],
     values: &[
         &["populate", "opiate", "opulent"],
         &["populates", "opiates"],
+        &["output"],
     ],
     range: 4..=5,
 };
 
 static WORD_OPT_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Nested(&WORD_OPT_CHILDREN),
     value: None,
@@ -78097,14 +78318,15 @@
         dictgen::InsensitiveStr::Ascii("resssing"),
         dictgen::InsensitiveStr::Ascii("resssion"),
         dictgen::InsensitiveStr::Ascii("rotunities"),
         dictgen::InsensitiveStr::Ascii("rotunity"),
         dictgen::InsensitiveStr::Ascii("roximate"),
         dictgen::InsensitiveStr::Ascii("s"),
         dictgen::InsensitiveStr::Ascii("sofite"),
+        dictgen::InsensitiveStr::Ascii("urtinity"),
         dictgen::InsensitiveStr::Ascii("urtunities"),
         dictgen::InsensitiveStr::Ascii("urtunity"),
     ],
     values: &[
         &["openly"],
         &["operate"],
         &["operated"],
@@ -78140,14 +78362,15 @@
         &["oppressing"],
         &["oppression"],
         &["opportunities"],
         &["opportunity"],
         &["approximate"],
         &["oops"],
         &["opposite"],
+        &["opportunity"],
         &["opportunities"],
         &["opportunity"],
     ],
     range: 1..=12,
 };
 
 static WORD_OPO_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
@@ -78810,15 +79033,15 @@
         &["contains"],
         &["ontario"],
         &["context"],
         &["ontario"],
         &["controlled"],
         &["convenience"],
         &["conventions"],
-        &["own"],
+        &["own", "now"],
         &["owned"],
         &["ennui"],
         &["owner"],
         &["ownership"],
         &["owning"],
         &["owns"],
         &["only", "on", "one"],
@@ -79291,14 +79514,15 @@
         dictgen::InsensitiveStr::Ascii("eted"),
         dictgen::InsensitiveStr::Ascii("eting"),
         dictgen::InsensitiveStr::Ascii("etp"),
         dictgen::InsensitiveStr::Ascii("ett"),
         dictgen::InsensitiveStr::Ascii("ited"),
         dictgen::InsensitiveStr::Ascii("pirng"),
         dictgen::InsensitiveStr::Ascii("rping"),
+        dictgen::InsensitiveStr::Ascii("t"),
         dictgen::InsensitiveStr::Ascii("tets"),
     ],
     values: &[
         &["offence"],
         &["offense"],
         &["offenses"],
         &["offset"],
@@ -79306,17 +79530,18 @@
         &["offsetted"],
         &["offsetting"],
         &["offset"],
         &["offset"],
         &["offside"],
         &["offspring"],
         &["offspring"],
+        &["offset"],
         &["offsets"],
     ],
-    range: 2..=5,
+    range: 1..=5,
 };
 
 static WORD_OFFR_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_OFFR_CHILDREN),
     value: None,
 };
 
@@ -81713,14 +81938,15 @@
         dictgen::InsensitiveStr::Ascii("htwestern"),
         dictgen::InsensitiveStr::Ascii("ifications"),
         dictgen::InsensitiveStr::Ascii("mailzation"),
         dictgen::InsensitiveStr::Ascii("maized"),
         dictgen::InsensitiveStr::Ascii("male"),
         dictgen::InsensitiveStr::Ascii("males"),
         dictgen::InsensitiveStr::Ascii("malis"),
+        dictgen::InsensitiveStr::Ascii("malizd"),
         dictgen::InsensitiveStr::Ascii("mall"),
         dictgen::InsensitiveStr::Ascii("mallized"),
         dictgen::InsensitiveStr::Ascii("malls"),
         dictgen::InsensitiveStr::Ascii("malos"),
         dictgen::InsensitiveStr::Ascii("maly"),
         dictgen::InsensitiveStr::Ascii("malyl"),
         dictgen::InsensitiveStr::Ascii("malyly"),
@@ -81777,14 +82003,15 @@
         &["northwestern"],
         &["notifications"],
         &["normalization"],
         &["normalized"],
         &["normal"],
         &["normals"],
         &["normals"],
+        &["normalized"],
         &["normal", "normally"],
         &["normalized"],
         &["normals"],
         &["normals"],
         &["normally"],
         &["normally"],
         &["normally"],
@@ -84988,19 +85215,20 @@
 static WORD_NECA_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_NECA_CHILDREN),
     value: None,
 };
 
 pub static WORD_NECA_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
+        dictgen::InsensitiveStr::Ascii("ssary"),
         dictgen::InsensitiveStr::Ascii("ssery"),
         dictgen::InsensitiveStr::Ascii("ssry"),
         dictgen::InsensitiveStr::Ascii("use"),
     ],
-    values: &[&["necessary"], &["necessary"], &["because"]],
+    values: &[&["necessary"], &["necessary"], &["necessary"], &["because"]],
     range: 3..=5,
 };
 
 static WORD_NEA_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_NEA_CHILDREN),
     value: None,
 };
@@ -87585,14 +87813,15 @@
         dictgen::InsensitiveStr::Ascii("litihic"),
         dictgen::InsensitiveStr::Ascii("loge"),
         dictgen::InsensitiveStr::Ascii("lopies"),
         dictgen::InsensitiveStr::Ascii("lopy"),
         dictgen::InsensitiveStr::Ascii("lothic"),
         dictgen::InsensitiveStr::Ascii("louge"),
         dictgen::InsensitiveStr::Ascii("lythic"),
+        dictgen::InsensitiveStr::Ascii("morpize"),
         dictgen::InsensitiveStr::Ascii("ntonicity"),
         dictgen::InsensitiveStr::Ascii("pace"),
         dictgen::InsensitiveStr::Ascii("pilies"),
         dictgen::InsensitiveStr::Ascii("ploies"),
         dictgen::InsensitiveStr::Ascii("ploy"),
         dictgen::InsensitiveStr::Ascii("polets"),
         dictgen::InsensitiveStr::Ascii("police"),
@@ -87624,14 +87853,15 @@
         &["monolithic"],
         &["monologue"],
         &["monopolies"],
         &["monopoly"],
         &["monolithic"],
         &["monologue"],
         &["monolithic"],
+        &["monomorphize"],
         &["monotonicity"],
         &["monospace"],
         &["monopolies"],
         &["monopolies"],
         &["monopoly"],
         &["monopolies"],
         &["monopolies"],
@@ -92795,14 +93025,15 @@
 };
 
 pub static WORD_MAY_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("alsia"),
         dictgen::InsensitiveStr::Ascii("alsian"),
         dictgen::InsensitiveStr::Ascii("balline"),
+        dictgen::InsensitiveStr::Ascii("bed"),
         dictgen::InsensitiveStr::Ascii("bee"),
         dictgen::InsensitiveStr::Ascii("belle"),
         dictgen::InsensitiveStr::Ascii("belleine"),
         dictgen::InsensitiveStr::Ascii("bellene"),
         dictgen::InsensitiveStr::Ascii("bellibe"),
         dictgen::InsensitiveStr::Ascii("belliene"),
         dictgen::InsensitiveStr::Ascii("bellinne"),
@@ -92816,14 +93047,15 @@
         dictgen::InsensitiveStr::Ascii("ybe"),
     ],
     values: &[
         &["malaysia"],
         &["malaysian"],
         &["maybelline"],
         &["maybe"],
+        &["maybe"],
         &["maybelline"],
         &["maybelline"],
         &["maybelline"],
         &["maybelline"],
         &["maybelline"],
         &["maybelline"],
         &["maybelline"],
@@ -98392,14 +98624,15 @@
         dictgen::InsensitiveStr::Ascii("itudie"),
         dictgen::InsensitiveStr::Ascii("itudine"),
         dictgen::InsensitiveStr::Ascii("itue"),
         dictgen::InsensitiveStr::Ascii("itute"),
         dictgen::InsensitiveStr::Ascii("nern"),
         dictgen::InsensitiveStr::Ascii("ops"),
         dictgen::InsensitiveStr::Ascii("set"),
+        dictgen::InsensitiveStr::Ascii("st"),
         dictgen::InsensitiveStr::Ascii("titude"),
     ],
     values: &[
         &["alteration"],
         &["later", "latest"],
         &["latest"],
         &["latin"],
@@ -98407,14 +98640,15 @@
         &["latitude"],
         &["latitude"],
         &["latitude"],
         &["latitude"],
         &["lantern"],
         &["laptops"],
         &["latest"],
+        &["latest"],
         &["latitude"],
     ],
     range: 2..=7,
 };
 
 static WORD_LAS_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_LAS_CHILDREN),
@@ -101195,14 +101429,15 @@
         dictgen::InsensitiveStr::Ascii("ratable"),
         dictgen::InsensitiveStr::Ascii("rater"),
         dictgen::InsensitiveStr::Ascii("raterate"),
         dictgen::InsensitiveStr::Ascii("ratered"),
         dictgen::InsensitiveStr::Ascii("ratior"),
         dictgen::InsensitiveStr::Ascii("ratiors"),
         dictgen::InsensitiveStr::Ascii("ratons"),
+        dictgen::InsensitiveStr::Ascii("reate"),
         dictgen::InsensitiveStr::Ascii("reating"),
         dictgen::InsensitiveStr::Ascii("reator"),
         dictgen::InsensitiveStr::Ascii("rface"),
         dictgen::InsensitiveStr::Ascii("rfaces"),
         dictgen::InsensitiveStr::Ascii("rm"),
         dictgen::InsensitiveStr::Ascii("rnations"),
         dictgen::InsensitiveStr::Ascii("rpreter"),
@@ -101235,14 +101470,15 @@
         &["iterable"],
         &["iterator"],
         &["iterate"],
         &["iterated"],
         &["iterator"],
         &["iterators"],
         &["iterations"],
+        &["iterate"],
         &["iterating"],
         &["iterator"],
         &["interface"],
         &["interfaces"],
         &["term", "item", "intern"],
         &["iterations"],
         &["interpreter"],
@@ -108390,14 +108626,15 @@
         dictgen::InsensitiveStr::Ascii("erets"),
         dictgen::InsensitiveStr::Ascii("eriet"),
         dictgen::InsensitiveStr::Ascii("erint"),
         dictgen::InsensitiveStr::Ascii("erintly"),
         dictgen::InsensitiveStr::Ascii("eritablility"),
         dictgen::InsensitiveStr::Ascii("eritage"),
         dictgen::InsensitiveStr::Ascii("eritence"),
+        dictgen::InsensitiveStr::Ascii("eritences"),
         dictgen::InsensitiveStr::Ascii("erith"),
         dictgen::InsensitiveStr::Ascii("erithed"),
         dictgen::InsensitiveStr::Ascii("erithing"),
         dictgen::InsensitiveStr::Ascii("eriths"),
         dictgen::InsensitiveStr::Ascii("eritted"),
         dictgen::InsensitiveStr::Ascii("ernetly"),
         dictgen::InsensitiveStr::Ascii("errit"),
@@ -108433,14 +108670,15 @@
         &["inherits"],
         &["inherit"],
         &["inherit"],
         &["inherently"],
         &["inheritability"],
         &["heritage", "inheritance"],
         &["inheritance"],
+        &["inheritances"],
         &["inherit"],
         &["inherited"],
         &["inheriting"],
         &["inherits"],
         &["inherited"],
         &["inherently"],
         &["inherit"],
@@ -111551,24 +111789,26 @@
     keys: &[
         dictgen::InsensitiveStr::Ascii("patibility"),
         dictgen::InsensitiveStr::Ascii("patible"),
         dictgen::InsensitiveStr::Ascii("ptibele"),
         dictgen::InsensitiveStr::Ascii("ptibelities"),
         dictgen::InsensitiveStr::Ascii("ptibelity"),
         dictgen::InsensitiveStr::Ascii("ptible"),
+        dictgen::InsensitiveStr::Ascii("tible"),
     ],
     values: &[
         &["incompatibility"],
         &["incompatible"],
         &["incompatible"],
         &["incompatibilities"],
         &["incompatibility"],
         &["incompatible"],
+        &["incompatible"],
     ],
-    range: 6..=11,
+    range: 5..=11,
 };
 
 static WORD_INCOH_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_INCOH_CHILDREN),
     value: None,
 };
 
@@ -115468,21 +115708,28 @@
 static WORD_IDENI_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_IDENI_CHILDREN),
     value: None,
 };
 
 pub static WORD_IDENI_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
+        dictgen::InsensitiveStr::Ascii("fiable"),
         dictgen::InsensitiveStr::Ascii("tfy"),
         dictgen::InsensitiveStr::Ascii("ties"),
         dictgen::InsensitiveStr::Ascii("tify"),
         dictgen::InsensitiveStr::Ascii("ty"),
     ],
-    values: &[&["identify"], &["identities"], &["identify"], &["identity"]],
-    range: 2..=4,
+    values: &[
+        &["identifiable"],
+        &["identify"],
+        &["identities"],
+        &["identify"],
+        &["identity"],
+    ],
+    range: 2..=6,
 };
 
 static WORD_IDENF_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_IDENF_CHILDREN),
     value: None,
 };
 
@@ -121776,14 +122023,15 @@
         dictgen::InsensitiveStr::Ascii("erate"),
         dictgen::InsensitiveStr::Ascii("erated"),
         dictgen::InsensitiveStr::Ascii("erates"),
         dictgen::InsensitiveStr::Ascii("erating"),
         dictgen::InsensitiveStr::Ascii("eration"),
         dictgen::InsensitiveStr::Ascii("erations"),
         dictgen::InsensitiveStr::Ascii("eric"),
+        dictgen::InsensitiveStr::Ascii("ored"),
         dictgen::InsensitiveStr::Ascii("orung"),
     ],
     values: &[
         &["ganking"],
         &["gnawed"],
         &["general"],
         &["generally"],
@@ -121791,14 +122039,15 @@
         &["generate"],
         &["generated"],
         &["generates"],
         &["generating"],
         &["generation"],
         &["generations"],
         &["generic"],
+        &["ignored"],
         &["ignoring"],
     ],
     range: 4..=8,
 };
 
 static WORD_GM_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_GM_CHILDREN),
@@ -124564,14 +124813,15 @@
         dictgen::InsensitiveStr::Ascii("mal"),
         dictgen::InsensitiveStr::Ascii("mat"),
         dictgen::InsensitiveStr::Ascii("mated"),
         dictgen::InsensitiveStr::Ascii("mates"),
         dictgen::InsensitiveStr::Ascii("mating"),
         dictgen::InsensitiveStr::Ascii("mation"),
         dictgen::InsensitiveStr::Ascii("mats"),
+        dictgen::InsensitiveStr::Ascii("matted"),
         dictgen::InsensitiveStr::Ascii("matting"),
         dictgen::InsensitiveStr::Ascii("me"),
         dictgen::InsensitiveStr::Ascii("med"),
         dictgen::InsensitiveStr::Ascii("merly"),
         dictgen::InsensitiveStr::Ascii("midable"),
         dictgen::InsensitiveStr::Ascii("mm"),
         dictgen::InsensitiveStr::Ascii("ms"),
@@ -124609,14 +124859,15 @@
         &["formal"],
         &["format"],
         &["formatted"],
         &["formats"],
         &["formatting"],
         &["formation"],
         &["formats"],
+        &["formatted"],
         &["formatting"],
         &["from"],
         &["formed"],
         &["formerly"],
         &["formidable"],
         &["from"],
         &["forms"],
@@ -125661,14 +125912,15 @@
         dictgen::InsensitiveStr::Ascii("inable"),
         dictgen::InsensitiveStr::Ascii("itable"),
         dictgen::InsensitiveStr::Ascii("matted"),
         dictgen::InsensitiveStr::Ascii("ost"),
         dictgen::InsensitiveStr::Ascii("t"),
         dictgen::InsensitiveStr::Ascii("ua"),
         dictgen::InsensitiveStr::Ascii("ual"),
+        dictgen::InsensitiveStr::Ascii("uala"),
         dictgen::InsensitiveStr::Ascii("uale"),
         dictgen::InsensitiveStr::Ascii("uals"),
         dictgen::InsensitiveStr::Ascii("ualte"),
         dictgen::InsensitiveStr::Ascii("uladas"),
         dictgen::InsensitiveStr::Ascii("ulados"),
         dictgen::InsensitiveStr::Ascii("ulaes"),
         dictgen::InsensitiveStr::Ascii("ulaical"),
@@ -125719,14 +125971,15 @@
         &["formidable"],
         &["formidable"],
         &["formatted"],
         &["foremost"],
         &["format"],
         &["formula"],
         &["formula"],
+        &["formula"],
         &["formulae"],
         &["formulas"],
         &["formulate"],
         &["formulas"],
         &["formulas"],
         &["formulas"],
         &["formulaic"],
@@ -127306,24 +127559,26 @@
 
 pub static WORD_FIX_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("e"),
         dictgen::InsensitiveStr::Ascii("el"),
         dictgen::InsensitiveStr::Ascii("els"),
         dictgen::InsensitiveStr::Ascii("eme"),
+        dictgen::InsensitiveStr::Ascii("utre"),
         dictgen::InsensitiveStr::Ascii("wd"),
     ],
     values: &[
         &["fixed", "fixes", "fix", "fixme", "fixer"],
         &["pixel"],
         &["pixels"],
         &["fixme"],
+        &["fixture"],
         &["fixed"],
     ],
-    range: 1..=3,
+    range: 1..=4,
 };
 
 static WORD_FIV_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_FIV_CHILDREN),
     value: None,
 };
 
@@ -127588,14 +127843,15 @@
     children: dictgen::DictTrieChild::Flat(&WORD_FINI_CHILDREN),
     value: None,
 };
 
 pub static WORD_FINI_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("alization"),
+        dictgen::InsensitiveStr::Ascii("alize"),
         dictgen::InsensitiveStr::Ascii("alizing"),
         dictgen::InsensitiveStr::Ascii("lizes"),
         dictgen::InsensitiveStr::Ascii("nsh"),
         dictgen::InsensitiveStr::Ascii("nshed"),
         dictgen::InsensitiveStr::Ascii("sch"),
         dictgen::InsensitiveStr::Ascii("sched"),
         dictgen::InsensitiveStr::Ascii("sed"),
@@ -127603,14 +127859,15 @@
         dictgen::InsensitiveStr::Ascii("shied"),
         dictgen::InsensitiveStr::Ascii("shs"),
         dictgen::InsensitiveStr::Ascii("sse"),
         dictgen::InsensitiveStr::Ascii("tel"),
     ],
     values: &[
         &["finalization"],
+        &["finalize"],
         &["finalizing"],
         &["finalizes"],
         &["finnish"],
         &["finished"],
         &["finish", "finnish"],
         &["finished"],
         &["finished"],
@@ -135498,14 +135755,15 @@
         dictgen::InsensitiveStr::Ascii("eples"),
         dictgen::InsensitiveStr::Ascii("ied"),
         dictgen::InsensitiveStr::Ascii("in"),
         dictgen::InsensitiveStr::Ascii("inated"),
         dictgen::InsensitiveStr::Ascii("ind"),
         dictgen::InsensitiveStr::Ascii("inerad"),
         dictgen::InsensitiveStr::Ascii("ing"),
+        dictgen::InsensitiveStr::Ascii("ininig"),
         dictgen::InsensitiveStr::Ascii("inining"),
         dictgen::InsensitiveStr::Ascii("le"),
         dictgen::InsensitiveStr::Ascii("les"),
         dictgen::InsensitiveStr::Ascii("lpe"),
         dictgen::InsensitiveStr::Ascii("lpes"),
         dictgen::InsensitiveStr::Ascii("nple"),
         dictgen::InsensitiveStr::Ascii("nples"),
@@ -135526,14 +135784,15 @@
         &["examined"],
         &["examine", "examining"],
         &["examined"],
         &["examined"],
         &["examined"],
         &["examining"],
         &["examining"],
+        &["examining"],
         &["example"],
         &["examples"],
         &["example"],
         &["examples"],
         &["example"],
         &["examples"],
         &["example"],
@@ -135909,16 +136168,17 @@
 };
 
 pub static WORD_EVEY_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("one"),
         dictgen::InsensitiveStr::Ascii("r"),
         dictgen::InsensitiveStr::Ascii("rones"),
+        dictgen::InsensitiveStr::Ascii("thing"),
     ],
-    values: &[&["everyone"], &["every"], &["everyones"]],
+    values: &[&["everyone"], &["every"], &["everyones"], &["everything"]],
     range: 1..=5,
 };
 
 static WORD_EVES_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_EVES_CHILDREN),
     value: None,
 };
@@ -140161,22 +140421,24 @@
     children: dictgen::DictTrieChild::Flat(&WORD_EMO_CHILDREN),
     value: None,
 };
 
 pub static WORD_EMO_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("bdiment"),
+        dictgen::InsensitiveStr::Ascii("iji"),
         dictgen::InsensitiveStr::Ascii("tionaly"),
         dictgen::InsensitiveStr::Ascii("tionella"),
         dictgen::InsensitiveStr::Ascii("ty"),
         dictgen::InsensitiveStr::Ascii("ugh"),
         dictgen::InsensitiveStr::Ascii("ught"),
     ],
     values: &[
         &["embodiment"],
+        &["emoji"],
         &["emotionally"],
         &["emotionally"],
         &["empty"],
         &["enough"],
         &["enough"],
     ],
     range: 2..=8,
@@ -140259,26 +140521,28 @@
         dictgen::InsensitiveStr::Ascii("ited"),
         dictgen::InsensitiveStr::Ascii("nate"),
         dictgen::InsensitiveStr::Ascii("nated"),
         dictgen::InsensitiveStr::Ascii("pres"),
         dictgen::InsensitiveStr::Ascii("sion"),
         dictgen::InsensitiveStr::Ascii("ss"),
         dictgen::InsensitiveStr::Ascii("ssed"),
+        dictgen::InsensitiveStr::Ascii("table"),
         dictgen::InsensitiveStr::Ascii("ted"),
         dictgen::InsensitiveStr::Ascii("ting"),
         dictgen::InsensitiveStr::Ascii("tion"),
     ],
     values: &[
         &["emitted"],
         &["emanate"],
         &["emanated"],
         &["empires"],
         &["emission"],
         &["remiss", "amiss", "amass"],
         &["amassed", "amiss"],
+        &["emittable"],
         &["emitted"],
         &["emitting"],
         &["emission", "emotion"],
     ],
     range: 2..=5,
 };
 
@@ -151109,14 +151373,15 @@
         dictgen::InsensitiveStr::Ascii("lopmently"),
         dictgen::InsensitiveStr::Ascii("lopmentwise"),
         dictgen::InsensitiveStr::Ascii("lopmet"),
         dictgen::InsensitiveStr::Ascii("lopmetn"),
         dictgen::InsensitiveStr::Ascii("lopmetns"),
         dictgen::InsensitiveStr::Ascii("lopmets"),
         dictgen::InsensitiveStr::Ascii("lopmnet"),
+        dictgen::InsensitiveStr::Ascii("lopoment"),
         dictgen::InsensitiveStr::Ascii("lopors"),
         dictgen::InsensitiveStr::Ascii("lopp"),
         dictgen::InsensitiveStr::Ascii("loppe"),
         dictgen::InsensitiveStr::Ascii("lopped"),
         dictgen::InsensitiveStr::Ascii("loppement"),
         dictgen::InsensitiveStr::Ascii("lopper"),
         dictgen::InsensitiveStr::Ascii("loppers"),
@@ -151164,14 +151429,15 @@
         &["developmental"],
         &["developments"],
         &["developments", "development"],
         &["developments"],
         &["developments"],
         &["developments"],
         &["developments"],
+        &["development"],
         &["develops"],
         &["develop"],
         &["develop"],
         &["developed"],
         &["development"],
         &["developer"],
         &["developers"],
@@ -151673,14 +151939,15 @@
         dictgen::InsensitiveStr::Ascii("tas"),
         dictgen::InsensitiveStr::Ascii("te"),
         dictgen::InsensitiveStr::Ascii("tected"),
         dictgen::InsensitiveStr::Ascii("tes"),
         dictgen::InsensitiveStr::Ascii("tetd"),
         dictgen::InsensitiveStr::Ascii("tie"),
         dictgen::InsensitiveStr::Ascii("tiona"),
+        dictgen::InsensitiveStr::Ascii("tionn"),
         dictgen::InsensitiveStr::Ascii("tivs"),
         dictgen::InsensitiveStr::Ascii("toare"),
         dictgen::InsensitiveStr::Ascii("tsion"),
         dictgen::InsensitiveStr::Ascii("tsions"),
         dictgen::InsensitiveStr::Ascii("tt"),
     ],
     values: &[
@@ -151696,14 +151963,15 @@
         &["detects"],
         &["detected", "detect", "detects"],
         &["detected"],
         &["detects"],
         &["detected"],
         &["detectives"],
         &["detection", "detections"],
+        &["detection"],
         &["detectives"],
         &["detector"],
         &["detection"],
         &["detections"],
         &["detect"],
     ],
     range: 1..=6,
@@ -154433,14 +154701,15 @@
     value: None,
 };
 
 pub static WORD_DEPD_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("en"),
         dictgen::InsensitiveStr::Ascii("ence"),
+        dictgen::InsensitiveStr::Ascii("encencies"),
         dictgen::InsensitiveStr::Ascii("encente"),
         dictgen::InsensitiveStr::Ascii("encentes"),
         dictgen::InsensitiveStr::Ascii("ences"),
         dictgen::InsensitiveStr::Ascii("encies"),
         dictgen::InsensitiveStr::Ascii("ency"),
         dictgen::InsensitiveStr::Ascii("end"),
         dictgen::InsensitiveStr::Ascii("endancies"),
@@ -154470,14 +154739,15 @@
         dictgen::InsensitiveStr::Ascii("ens"),
         dictgen::InsensitiveStr::Ascii("ent"),
         dictgen::InsensitiveStr::Ascii("ents"),
     ],
     values: &[
         &["depend"],
         &["dependence"],
+        &["dependencies"],
         &["dependence"],
         &["dependences"],
         &["dependences"],
         &["dependencies"],
         &["dependency"],
         &["depend"],
         &["dependencies"],
@@ -160104,16 +160374,17 @@
 };
 
 pub static WORD_CURA_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("ge"),
         dictgen::InsensitiveStr::Ascii("geous"),
         dictgen::InsensitiveStr::Ascii("tin"),
+        dictgen::InsensitiveStr::Ascii("ture"),
     ],
-    values: &[&["courage"], &["courageous"], &["curtain"]],
+    values: &[&["courage"], &["courageous"], &["curtain"], &["curvature"]],
     range: 2..=5,
 };
 
 static WORD_CUP_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_CUP_CHILDREN),
     value: None,
 };
@@ -164943,19 +165214,24 @@
     children: dictgen::DictTrieChild::Flat(&WORD_CONVERA_CHILDREN),
     value: None,
 };
 
 pub static WORD_CONVERA_CHILDREN: dictgen::DictTable<&'static [&'static str]> =
     dictgen::DictTable {
         keys: &[
+            dictgen::InsensitiveStr::Ascii("ge"),
             dictgen::InsensitiveStr::Ascii("stion"),
             dictgen::InsensitiveStr::Ascii("stions"),
         ],
-        values: &[&["conversations"], &["conservation"]],
-        range: 5..=6,
+        values: &[
+            &["converge", "coverage"],
+            &["conversations"],
+            &["conservation"],
+        ],
+        range: 2..=6,
     };
 
 static WORD_CONVEN_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_CONVEN_CHILDREN),
     value: None,
 };
 
@@ -167302,17 +167578,20 @@
 static WORD_CONSTRO_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_CONSTRO_CHILDREN),
     value: None,
 };
 
 pub static WORD_CONSTRO_CHILDREN: dictgen::DictTable<&'static [&'static str]> =
     dictgen::DictTable {
-        keys: &[dictgen::InsensitiveStr::Ascii("llers")],
-        values: &[&["controllers"]],
-        range: 5..=5,
+        keys: &[
+            dictgen::InsensitiveStr::Ascii("l"),
+            dictgen::InsensitiveStr::Ascii("llers"),
+        ],
+        values: &[&["control"], &["controllers"]],
+        range: 1..=5,
     };
 
 static WORD_CONSTRI_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_CONSTRI_CHILDREN),
     value: None,
 };
 
@@ -172462,14 +172741,15 @@
         dictgen::InsensitiveStr::Ascii("tin"),
         dictgen::InsensitiveStr::Ascii("tiom"),
         dictgen::InsensitiveStr::Ascii("tition"),
         dictgen::InsensitiveStr::Ascii("tito"),
         dictgen::InsensitiveStr::Ascii("tley"),
         dictgen::InsensitiveStr::Ascii("tly"),
         dictgen::InsensitiveStr::Ascii("tness"),
+        dictgen::InsensitiveStr::Ascii("tor"),
         dictgen::InsensitiveStr::Ascii("ts"),
         dictgen::InsensitiveStr::Ascii("tte"),
         dictgen::InsensitiveStr::Ascii("ttly"),
         dictgen::InsensitiveStr::Ascii("ty"),
         dictgen::InsensitiveStr::Ascii("xers"),
         dictgen::InsensitiveStr::Ascii("xety"),
         dictgen::InsensitiveStr::Ascii("xitiy"),
@@ -172524,14 +172804,15 @@
         &["completion"],
         &["completion"],
         &["completion"],
         &["completion"],
         &["completely"],
         &["completely"],
         &["completeness"],
+        &["completer", "completion"],
         &["completes"],
         &["complete"],
         &["completely"],
         &["completely"],
         &["complexes"],
         &["complexity"],
         &["complexity"],
@@ -174912,14 +175193,15 @@
         dictgen::InsensitiveStr::Ascii("pny"),
         dictgen::InsensitiveStr::Ascii("prable"),
         dictgen::InsensitiveStr::Ascii("pre"),
         dictgen::InsensitiveStr::Ascii("pres"),
         dictgen::InsensitiveStr::Ascii("pring"),
         dictgen::InsensitiveStr::Ascii("prison"),
         dictgen::InsensitiveStr::Ascii("prisons"),
+        dictgen::InsensitiveStr::Ascii("pt"),
         dictgen::InsensitiveStr::Ascii("ptibele"),
         dictgen::InsensitiveStr::Ascii("ptibelities"),
         dictgen::InsensitiveStr::Ascii("ptibelity"),
         dictgen::InsensitiveStr::Ascii("ptible"),
         dictgen::InsensitiveStr::Ascii("rators"),
         dictgen::InsensitiveStr::Ascii("rde"),
         dictgen::InsensitiveStr::Ascii("tibility"),
@@ -174952,14 +175234,15 @@
         &["company"],
         &["comparable"],
         &["compare"],
         &["compares"],
         &["comparing"],
         &["comparison"],
         &["comparisons"],
+        &["compat"],
         &["compatible"],
         &["compatibilities"],
         &["compatibility"],
         &["compatible"],
         &["comparators"],
         &["comrade"],
         &["compatibility"],
@@ -175504,14 +175787,15 @@
         dictgen::InsensitiveStr::Ascii("sion"),
         dictgen::InsensitiveStr::Ascii("spe"),
         dictgen::InsensitiveStr::Ascii("sped"),
         dictgen::InsensitiveStr::Ascii("spes"),
         dictgen::InsensitiveStr::Ascii("spible"),
         dictgen::InsensitiveStr::Ascii("sping"),
         dictgen::InsensitiveStr::Ascii("taral"),
+        dictgen::InsensitiveStr::Ascii("ter"),
         dictgen::InsensitiveStr::Ascii("terial"),
         dictgen::InsensitiveStr::Ascii("terol"),
         dictgen::InsensitiveStr::Ascii("tiong"),
         dictgen::InsensitiveStr::Ascii("toral"),
     ],
     values: &[
         &["collaborate"],
@@ -175546,14 +175830,15 @@
         &["collision"],
         &["collapse"],
         &["collapsed"],
         &["collapses"],
         &["collapsible"],
         &["collapsing"],
         &["collateral"],
+        &["collator"],
         &["collateral"],
         &["collateral"],
         &["collation"],
         &["collateral"],
     ],
     range: 2..=10,
 };
@@ -175561,19 +175846,20 @@
 static WORD_COLI_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_COLI_CHILDREN),
     value: None,
 };
 
 pub static WORD_COLI_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
+        dictgen::InsensitiveStr::Ascii("de"),
         dictgen::InsensitiveStr::Ascii("sion"),
         dictgen::InsensitiveStr::Ascii("ssion"),
     ],
-    values: &[&["collision"], &["collision"]],
-    range: 4..=5,
+    values: &[&["collide"], &["collision"], &["collision"]],
+    range: 2..=5,
 };
 
 static WORD_COLG_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_COLG_CHILDREN),
     value: None,
 };
 
@@ -176056,15 +176342,15 @@
     children: dictgen::DictTrieChild::Nested(&WORD_COA_CHILDREN),
     value: None,
 };
 
 static WORD_COA_CHILDREN: [Option<&dictgen::DictTrieNode<&'static [&'static str]>>; 26] = [
     None,
     None,
-    None,
+    Some(&WORD_COAC_NODE),
     None,
     None,
     None,
     None,
     None,
     None,
     None,
@@ -176329,14 +176615,25 @@
         &["coalescence"],
         &["coalesces"],
         &["coalescing"],
     ],
     range: 2..=7,
 };
 
+static WORD_COAC_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
+    children: dictgen::DictTrieChild::Flat(&WORD_COAC_CHILDREN),
+    value: None,
+};
+
+pub static WORD_COAC_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
+    keys: &[dictgen::InsensitiveStr::Ascii("hig")],
+    values: &[&["coaching"]],
+    range: 3..=3,
+};
+
 static WORD_CN_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_CN_CHILDREN),
     value: None,
 };
 
 pub static WORD_CN_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
@@ -176659,14 +176956,15 @@
         dictgen::InsensitiveStr::Ascii("nets"),
         dictgen::InsensitiveStr::Ascii("nicaly"),
         dictgen::InsensitiveStr::Ascii("nicas"),
         dictgen::InsensitiveStr::Ascii("nicos"),
         dictgen::InsensitiveStr::Ascii("pbaord"),
         dictgen::InsensitiveStr::Ascii("pboad"),
         dictgen::InsensitiveStr::Ascii("pboads"),
+        dictgen::InsensitiveStr::Ascii("ped"),
         dictgen::InsensitiveStr::Ascii("poard"),
         dictgen::InsensitiveStr::Ascii("poards"),
         dictgen::InsensitiveStr::Ascii("poing"),
         dictgen::InsensitiveStr::Ascii("shay"),
         dictgen::InsensitiveStr::Ascii("shays"),
         dictgen::InsensitiveStr::Ascii("shey"),
         dictgen::InsensitiveStr::Ascii("sheys"),
@@ -176718,14 +177016,15 @@
         &["clients"],
         &["clinically"],
         &["clinics"],
         &["clinics"],
         &["clipboard"],
         &["clipboard"],
         &["clipboards"],
+        &["clipped"],
         &["clipboard"],
         &["clipboards"],
         &["clipping"],
         &["cliché"],
         &["clichés"],
         &["cliché"],
         &["clichés"],
@@ -178280,17 +178579,20 @@
 
 static WORD_CIE_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_CIE_CHILDREN),
     value: None,
 };
 
 pub static WORD_CIE_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
-    keys: &[dictgen::InsensitiveStr::Ascii("lings")],
-    values: &[&["ceilings"]],
-    range: 5..=5,
+    keys: &[
+        dictgen::InsensitiveStr::Ascii("lings"),
+        dictgen::InsensitiveStr::Ascii("nts"),
+    ],
+    values: &[&["ceilings"], &["clients"]],
+    range: 3..=5,
 };
 
 static WORD_CIC_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_CIC_CHILDREN),
     value: None,
 };
 
@@ -185435,14 +185737,15 @@
         dictgen::InsensitiveStr::Ascii("ild"),
         dictgen::InsensitiveStr::Ascii("k"),
         dictgen::InsensitiveStr::Ascii("l"),
         dictgen::InsensitiveStr::Ascii("ldd"),
         dictgen::InsensitiveStr::Ascii("lded"),
         dictgen::InsensitiveStr::Ascii("ldes"),
         dictgen::InsensitiveStr::Ascii("ldins"),
+        dictgen::InsensitiveStr::Ascii("ldning"),
         dictgen::InsensitiveStr::Ascii("ldpackge"),
         dictgen::InsensitiveStr::Ascii("ldpackges"),
         dictgen::InsensitiveStr::Ascii("ling"),
         dictgen::InsensitiveStr::Ascii("lings"),
         dictgen::InsensitiveStr::Ascii("llt"),
         dictgen::InsensitiveStr::Ascii("ls"),
         dictgen::InsensitiveStr::Ascii("lter"),
@@ -185479,14 +185782,15 @@
         &["build"],
         &["bulk"],
         &["build", "built"],
         &["build", "builds"],
         &["built"],
         &["builders"],
         &["buildings"],
+        &["building"],
         &["buildpackage"],
         &["buildpackages"],
         &["building"],
         &["buildings"],
         &["built"],
         &["builds"],
         &["builder"],
@@ -190701,16 +191005,17 @@
 };
 
 pub static WORD_BAI_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("sc"),
         dictgen::InsensitiveStr::Ascii("scly"),
         dictgen::InsensitiveStr::Ascii("sed"),
+        dictgen::InsensitiveStr::Ascii("ses"),
     ],
-    values: &[&["basic"], &["basically"], &["raised"]],
+    values: &[&["basic"], &["basically"], &["raised"], &["biases"]],
     range: 2..=4,
 };
 
 static WORD_BAH_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_BAH_CHILDREN),
     value: None,
 };
@@ -190908,23 +191213,25 @@
 pub static WORD_BACKW_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("ad"),
         dictgen::InsensitiveStr::Ascii("ardss"),
         dictgen::InsensitiveStr::Ascii("are"),
         dictgen::InsensitiveStr::Ascii("ark"),
         dictgen::InsensitiveStr::Ascii("ars"),
+        dictgen::InsensitiveStr::Ascii("ord"),
         dictgen::InsensitiveStr::Ascii("rad"),
     ],
     values: &[
         &["backward"],
         &["backwards"],
         &["backward"],
         &["backward"],
         &["backward", "backwards"],
         &["backward"],
+        &["backward"],
     ],
     range: 2..=5,
 };
 
 static WORD_BACKT_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Flat(&WORD_BACKT_CHILDREN),
     value: None,
@@ -191633,14 +191940,15 @@
 
 pub static WORD_AVI_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("able"),
         dictgen::InsensitiveStr::Ascii("aiton"),
         dictgen::InsensitiveStr::Ascii("alability"),
         dictgen::InsensitiveStr::Ascii("alable"),
+        dictgen::InsensitiveStr::Ascii("alible"),
         dictgen::InsensitiveStr::Ascii("lability"),
         dictgen::InsensitiveStr::Ascii("lable"),
         dictgen::InsensitiveStr::Ascii("od"),
         dictgen::InsensitiveStr::Ascii("oded"),
         dictgen::InsensitiveStr::Ascii("oding"),
         dictgen::InsensitiveStr::Ascii("ods"),
         dictgen::InsensitiveStr::Ascii("sories"),
@@ -191649,14 +191957,15 @@
         dictgen::InsensitiveStr::Ascii("sory"),
     ],
     values: &[
         &["available"],
         &["aviation"],
         &["availability"],
         &["available"],
+        &["available"],
         &["availability"],
         &["available"],
         &["avoid"],
         &["avoided"],
         &["avoiding"],
         &["avoids"],
         &["advisories"],
@@ -194915,14 +195224,15 @@
         dictgen::InsensitiveStr::Ascii("metricaly"),
         dictgen::InsensitiveStr::Ascii("mmeric"),
         dictgen::InsensitiveStr::Ascii("mmetri"),
         dictgen::InsensitiveStr::Ascii("nchnous"),
         dictgen::InsensitiveStr::Ascii("nchonous"),
         dictgen::InsensitiveStr::Ascii("nchonously"),
         dictgen::InsensitiveStr::Ascii("nchornous"),
+        dictgen::InsensitiveStr::Ascii("nchornously"),
         dictgen::InsensitiveStr::Ascii("nchoronous"),
         dictgen::InsensitiveStr::Ascii("nchrnous"),
         dictgen::InsensitiveStr::Ascii("nchrnously"),
         dictgen::InsensitiveStr::Ascii("nchromous"),
         dictgen::InsensitiveStr::Ascii("nchron"),
         dictgen::InsensitiveStr::Ascii("nchroneously"),
         dictgen::InsensitiveStr::Ascii("nchronious"),
@@ -194953,14 +195263,15 @@
         &["asymmetrically"],
         &["asymmetric"],
         &["asymmetric", "asymmetry"],
         &["asynchronous"],
         &["asynchronous"],
         &["asynchronously"],
         &["asynchronous"],
+        &["asynchronously"],
         &["asynchronous"],
         &["asynchronous"],
         &["asynchronously"],
         &["asynchronous"],
         &["asynchronous"],
         &["asynchronously"],
         &["asynchronous"],
@@ -195349,14 +195660,15 @@
         dictgen::InsensitiveStr::Ascii("asin"),
         dictgen::InsensitiveStr::Ascii("asins"),
         dictgen::InsensitiveStr::Ascii("assans"),
         dictgen::InsensitiveStr::Ascii("embler"),
         dictgen::InsensitiveStr::Ascii("embly"),
         dictgen::InsensitiveStr::Ascii("ert"),
         dictgen::InsensitiveStr::Ascii("ertion"),
+        dictgen::InsensitiveStr::Ascii("et"),
         dictgen::InsensitiveStr::Ascii("its"),
         dictgen::InsensitiveStr::Ascii("ociate"),
         dictgen::InsensitiveStr::Ascii("ociated"),
         dictgen::InsensitiveStr::Ascii("ociation"),
         dictgen::InsensitiveStr::Ascii("ume"),
         dictgen::InsensitiveStr::Ascii("umes"),
         dictgen::InsensitiveStr::Ascii("uming"),
@@ -195365,23 +195677,24 @@
         &["assassin"],
         &["assassins"],
         &["assassins"],
         &["assembler"],
         &["assembly"],
         &["assert"],
         &["assertion"],
+        &["asset"],
         &["assists"],
         &["associated"],
         &["associated"],
         &["association"],
         &["assume"],
         &["assumes"],
         &["assuming"],
     ],
-    range: 3..=8,
+    range: 2..=8,
 };
 
 static WORD_ASSO_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Nested(&WORD_ASSO_CHILDREN),
     value: None,
 };
 
@@ -199474,14 +199787,15 @@
         dictgen::InsensitiveStr::Ascii("ie"),
         dictgen::InsensitiveStr::Ascii("iences"),
         dictgen::InsensitiveStr::Ascii("ikation"),
         dictgen::InsensitiveStr::Ascii("ikations"),
         dictgen::InsensitiveStr::Ascii("ikay"),
         dictgen::InsensitiveStr::Ascii("ikays"),
         dictgen::InsensitiveStr::Ascii("ing"),
+        dictgen::InsensitiveStr::Ascii("izes"),
         dictgen::InsensitiveStr::Ascii("lied"),
         dictgen::InsensitiveStr::Ascii("ly"),
         dictgen::InsensitiveStr::Ascii("uad"),
         dictgen::InsensitiveStr::Ascii("uase"),
         dictgen::InsensitiveStr::Ascii("yable"),
         dictgen::InsensitiveStr::Ascii("ycable"),
         dictgen::InsensitiveStr::Ascii("yed"),
@@ -199537,14 +199851,15 @@
         &["applied", "apply"],
         &["appliances"],
         &["application"],
         &["applications"],
         &["appliqué"],
         &["appliqués"],
         &["applying", "appalling"],
+        &["applies"],
         &["applied"],
         &["apply"],
         &["applaud"],
         &["applause"],
         &["applicable"],
         &["applicable"],
         &["applied"],
@@ -200290,14 +200605,15 @@
     children: dictgen::DictTrieChild::Flat(&WORD_ANU_CHILDREN),
     value: None,
 };
 
 pub static WORD_ANU_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("al"),
+        dictgen::InsensitiveStr::Ascii("alized"),
         dictgen::InsensitiveStr::Ascii("ally"),
         dictgen::InsensitiveStr::Ascii("glar"),
         dictgen::InsensitiveStr::Ascii("led"),
         dictgen::InsensitiveStr::Ascii("ling"),
         dictgen::InsensitiveStr::Ascii("ll"),
         dictgen::InsensitiveStr::Ascii("lled"),
         dictgen::InsensitiveStr::Ascii("lling"),
@@ -200305,28 +200621,29 @@
         dictgen::InsensitiveStr::Ascii("ls"),
         dictgen::InsensitiveStr::Ascii("mber"),
         dictgen::InsensitiveStr::Ascii("rism"),
         dictgen::InsensitiveStr::Ascii("where"),
     ],
     values: &[
         &["annual"],
+        &["annualized"],
         &["annually"],
         &["angular"],
         &["annulled"],
         &["annulling"],
         &["annul"],
         &["annulled"],
         &["annulling"],
         &["annulled"],
         &["annulls"],
         &["number"],
         &["aneurism"],
         &["anywhere"],
     ],
-    range: 2..=5,
+    range: 2..=6,
 };
 
 static WORD_ANT_NODE: dictgen::DictTrieNode<&'static [&'static str]> = dictgen::DictTrieNode {
     children: dictgen::DictTrieChild::Nested(&WORD_ANT_CHILDREN),
     value: None,
 };
 
@@ -207745,14 +208062,15 @@
 
 pub static WORD_ACU_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("al"),
         dictgen::InsensitiveStr::Ascii("ally"),
         dictgen::InsensitiveStr::Ascii("ired"),
         dictgen::InsensitiveStr::Ascii("ires"),
+        dictgen::InsensitiveStr::Ascii("malated"),
         dictgen::InsensitiveStr::Ascii("mulate"),
         dictgen::InsensitiveStr::Ascii("mulated"),
         dictgen::InsensitiveStr::Ascii("mulates"),
         dictgen::InsensitiveStr::Ascii("mulating"),
         dictgen::InsensitiveStr::Ascii("mulation"),
         dictgen::InsensitiveStr::Ascii("mulative"),
         dictgen::InsensitiveStr::Ascii("mulator"),
@@ -207772,14 +208090,15 @@
         dictgen::InsensitiveStr::Ascii("tual"),
     ],
     values: &[
         &["actual"],
         &["actually"],
         &["acquired"],
         &["acquires"],
+        &["accumulated"],
         &["accumulate"],
         &["accumulated"],
         &["accumulates"],
         &["accumulating"],
         &["accumulation"],
         &["accumulative"],
         &["accumulator"],
@@ -208877,14 +209196,15 @@
         dictgen::InsensitiveStr::Ascii("ally"),
         dictgen::InsensitiveStr::Ascii("arcy"),
         dictgen::InsensitiveStr::Ascii("arte"),
         dictgen::InsensitiveStr::Ascii("artely"),
         dictgen::InsensitiveStr::Ascii("astion"),
         dictgen::InsensitiveStr::Ascii("lumate"),
         dictgen::InsensitiveStr::Ascii("lumated"),
+        dictgen::InsensitiveStr::Ascii("lumating"),
         dictgen::InsensitiveStr::Ascii("lumation"),
         dictgen::InsensitiveStr::Ascii("malate"),
         dictgen::InsensitiveStr::Ascii("malated"),
         dictgen::InsensitiveStr::Ascii("malates"),
         dictgen::InsensitiveStr::Ascii("malation"),
         dictgen::InsensitiveStr::Ascii("malator"),
         dictgen::InsensitiveStr::Ascii("malte"),
@@ -208939,14 +209259,15 @@
         &["actually"],
         &["accuracy"],
         &["accurate"],
         &["accurately"],
         &["accusation"],
         &["accumulate"],
         &["accumulated"],
+        &["accumulating"],
         &["accumulation"],
         &["accumulate"],
         &["accumulated"],
         &["accumulates"],
         &["accumulation"],
         &["accumulator"],
         &["accumulate"],
@@ -210020,14 +210341,15 @@
     children: dictgen::DictTrieChild::Flat(&WORD_ACCC_CHILDREN),
     value: None,
 };
 
 pub static WORD_ACCC_CHILDREN: dictgen::DictTable<&'static [&'static str]> = dictgen::DictTable {
     keys: &[
         dictgen::InsensitiveStr::Ascii("ept"),
+        dictgen::InsensitiveStr::Ascii("eptable"),
         dictgen::InsensitiveStr::Ascii("epted"),
         dictgen::InsensitiveStr::Ascii("epting"),
         dictgen::InsensitiveStr::Ascii("epts"),
         dictgen::InsensitiveStr::Ascii("es"),
         dictgen::InsensitiveStr::Ascii("ess"),
         dictgen::InsensitiveStr::Ascii("essd"),
         dictgen::InsensitiveStr::Ascii("essed"),
@@ -210050,14 +210372,15 @@
         dictgen::InsensitiveStr::Ascii("uracy"),
         dictgen::InsensitiveStr::Ascii("urate"),
         dictgen::InsensitiveStr::Ascii("urately"),
         dictgen::InsensitiveStr::Ascii("used"),
     ],
     values: &[
         &["accept"],
+        &["acceptable"],
         &["accepted"],
         &["accepting"],
         &["accepts"],
         &["access"],
         &["access"],
         &["accessed"],
         &["accessed"],
```

### Comparing `typos-1.15.9/local_dependencies/dictgen/Cargo.toml` & `typos-1.16.0/local_dependencies/dictgen/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/local_dependencies/dictgen/src/map.rs` & `typos-1.16.0/local_dependencies/dictgen/src/map.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/local_dependencies/dictgen/src/table.rs` & `typos-1.16.0/local_dependencies/dictgen/src/table.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/local_dependencies/dictgen/src/trie.rs` & `typos-1.16.0/local_dependencies/dictgen/src/trie.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/local_dependencies/typos/Cargo.toml` & `typos-1.16.0/local_dependencies/typos/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/local_dependencies/typos/src/check.rs` & `typos-1.16.0/local_dependencies/typos/src/check.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/local_dependencies/typos/src/dict.rs` & `typos-1.16.0/local_dependencies/typos/src/dict.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/local_dependencies/typos/src/tokens.rs` & `typos-1.16.0/local_dependencies/typos/src/tokens.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/local_dependencies/typos-vars/Cargo.toml` & `typos-1.16.0/local_dependencies/typos-vars/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/local_dependencies/typos-vars/src/vars_codegen.rs` & `typos-1.16.0/local_dependencies/typos-vars/src/vars_codegen.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/rust_src/typos-cli/Cargo.toml` & `typos-1.16.0/rust_src/typos-cli/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "typos-cli"
-version = "1.15.9"
+version = "1.16.0"
 description = "Source Code Spelling Correction"
 readme = "../../README.md"
 categories = ["development-tools", "text-processing"]
 keywords = ["development", "spelling"]
 license= "MIT OR Apache-2.0"
 repository= "https://github.com/crate-ci/typos"
 edition= "2021"
```

### Comparing `typos-1.15.9/rust_src/typos-cli/benches/checks.rs` & `typos-1.16.0/rust_src/typos-cli/benches/checks.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/rust_src/typos-cli/benches/corrections.rs` & `typos-1.16.0/rust_src/typos-cli/benches/corrections.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/rust_src/typos-cli/benches/data.rs` & `typos-1.16.0/rust_src/typos-cli/benches/data.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/rust_src/typos-cli/benches/tokenize.rs` & `typos-1.16.0/rust_src/typos-cli/benches/tokenize.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/rust_src/typos-cli/src/bin/typos-cli/args.rs` & `typos-1.16.0/rust_src/typos-cli/src/bin/typos-cli/args.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/rust_src/typos-cli/src/bin/typos-cli/main.rs` & `typos-1.16.0/rust_src/typos-cli/src/bin/typos-cli/main.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/rust_src/typos-cli/src/bin/typos-cli/report.rs` & `typos-1.16.0/rust_src/typos-cli/src/bin/typos-cli/report.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/rust_src/typos-cli/src/config.rs` & `typos-1.16.0/rust_src/typos-cli/src/config.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/rust_src/typos-cli/src/default_types.rs` & `typos-1.16.0/rust_src/typos-cli/src/default_types.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/rust_src/typos-cli/src/dict.rs` & `typos-1.16.0/rust_src/typos-cli/src/dict.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/rust_src/typos-cli/src/file.rs` & `typos-1.16.0/rust_src/typos-cli/src/file.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/rust_src/typos-cli/src/file_type.rs` & `typos-1.16.0/rust_src/typos-cli/src/file_type.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 use std::collections::BTreeMap;
+use std::path::Path;
 
 use kstring::KString;
 
 #[derive(Default, Clone, Debug)]
 pub struct TypesBuilder {
     definitions: BTreeMap<KString, Vec<(KString, usize)>>,
 }
@@ -119,17 +120,32 @@
 
 impl Types {
     pub fn definitions(&self) -> &BTreeMap<KString, Vec<KString>> {
         &self.definitions
     }
 
     pub fn file_matched(&self, path: &std::path::Path) -> Option<&str> {
-        let file_name = path.file_name()?;
+        let mut mpath = Path::new(path);
         let mut matches = self.matches.get_or_default().borrow_mut();
-        self.set.matches_into(file_name, &mut *matches);
+        loop {
+            self.set.matches_into(mpath.file_name()?, &mut *matches);
+            if !matches.is_empty() {
+                break;
+            }
+            match mpath.extension() {
+                None => break,
+                Some(ext) => {
+                    if ext == "in" {
+                        mpath = Path::new(mpath.file_stem()?);
+                        continue;
+                    }
+                }
+            }
+            break;
+        }
         matches
             .last()
             .copied()
             .map(|i| self.glob_to_name[i].as_str())
     }
 }
 
@@ -157,22 +173,30 @@
 
     fn types() -> &'static [(&'static str, &'static [&'static str])] {
         &[
             ("html", &["*.html", "*.htm"]),
             ("js", &["*.js"]),
             ("json", &["*.json"]),
             ("lock", &["package-lock.json", "*.lock"]),
+            ("js-in", &["*.js.in"]),
         ]
     }
+    fn in_types() -> &'static [(&'static str, &'static [&'static str])] {
+        &[("html", &["*.html", "*.htm"]), ("in-canary", &["*.in"])]
+    }
 
     matched!(basic_match, types(), "leftpad.js", "js");
     matched!(multi_def_1, types(), "index.html", "html");
     matched!(multi_def_2, types(), "index.htm", "html");
     matched!(no_match, types(), "leftpad.ada", None);
     matched!(more_specific, types(), "package-lock.json", "lock");
+    matched!(basic_in, types(), "index.html.in", "html");
+    matched!(basic_in_in, types(), "index.html.in.in", "html");
+    matched!(ext_plus_in, types(), "foo.js.in", "js-in");
+    matched!(toplevel_in, in_types(), "index.html.in", "in-canary");
 
     macro_rules! sort {
         ($name:ident, $actual:expr, $expected:expr) => {
             #[test]
             fn $name() {
                 let expected = $expected.into_iter().collect::<Vec<&str>>();
```

### Comparing `typos-1.15.9/rust_src/typos-cli/src/policy.rs` & `typos-1.16.0/rust_src/typos-cli/src/policy.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/rust_src/typos-cli/src/report.rs` & `typos-1.16.0/rust_src/typos-cli/src/report.rs`

 * *Files identical despite different names*

### Comparing `typos-1.15.9/Cargo.lock` & `typos-1.16.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1649,15 +1649,15 @@
  "unicode-segmentation",
  "unicode-xid",
  "winnow",
 ]
 
 [[package]]
 name = "typos-cli"
-version = "1.15.9"
+version = "1.16.0"
 dependencies = [
  "ahash",
  "anstream",
  "anstyle",
  "anyhow",
  "assert_fs",
  "atty",
@@ -1697,15 +1697,15 @@
  "unicode-segmentation",
  "unicode-width",
  "varcon-core",
 ]
 
 [[package]]
 name = "typos-dict"
-version = "0.10.5"
+version = "0.10.6"
 dependencies = [
  "codegenrs",
  "csv",
  "dictgen",
  "edit-distance",
  "indexmap 2.0.0",
  "itertools",
```

### Comparing `typos-1.15.9/PKG-INFO` & `typos-1.16.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typos
-Version: 1.15.9
+Version: 1.16.0
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Source Code Spelling Correction
 Keywords: development,spelling
```


# Comparing `tmp/ast_grep_cli-0.7.2.tar.gz` & `tmp/ast_grep_cli-0.8.0.tar.gz`

## Comparing `ast_grep_cli-0.7.2.tar` & `ast_grep_cli-0.8.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-lsp/Cargo.toml
--rw-r--r--   0     1001      123    11369 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-lsp/src/lib.rs
--rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/Cargo.toml
--rw-r--r--   0     1001      123     2331 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/language.rs
--rw-r--r--   0     1001      123     3858 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/lib.rs
--rw-r--r--   0     1001      123    14850 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/match_tree.rs
--rw-r--r--   0     1001      123     3480 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/matcher/kind.rs
--rw-r--r--   0     1001      123     3783 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/matcher/node_match.rs
--rw-r--r--   0     1001      123    11138 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/matcher/pattern.rs
--rw-r--r--   0     1001      123      982 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/matcher/text.rs
--rw-r--r--   0     1001      123     6540 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/matcher.rs
--rw-r--r--   0     1001      123    11359 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/meta_var.rs
--rw-r--r--   0     1001      123    15431 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/node.rs
--rw-r--r--   0     1001      123    16351 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/ops.rs
--rw-r--r--   0     1001      123     3089 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/pinned.rs
--rw-r--r--   0     1001      123    10936 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/replacer/indent.rs
--rw-r--r--   0     1001      123     6181 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/replacer/structural.rs
--rw-r--r--   0     1001      123     9380 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/replacer/template.rs
--rw-r--r--   0     1001      123     2572 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/replacer.rs
--rw-r--r--   0     1001      123     8489 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/source.rs
--rw-r--r--   0     1001      123    16414 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/traversal.rs
--rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/Cargo.toml
--rw-r--r--   0     1001      123     6946 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/constraints.rs
--rw-r--r--   0     1001      123     6838 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/deserialize_env.rs
--rw-r--r--   0     1001      123     4880 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/lib.rs
--rw-r--r--   0     1001      123     2765 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/maybe.rs
--rw-r--r--   0     1001      123     6514 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/referent_rule.rs
--rw-r--r--   0     1001      123    16160 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/relational_rule/mod.rs
--rw-r--r--   0     1001      123     4138 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs
--rw-r--r--   0     1001      123    13151 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/rule.rs
--rw-r--r--   0     1001      123     6357 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/rule_collection.rs
--rw-r--r--   0     1001      123    11610 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/rule_config.rs
--rw-r--r--   0     1001      123     6716 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/transform.rs
--rw-r--r--   0        0        0      617 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-dynamic/Cargo.toml
--rw-r--r--   0     1001      123     7730 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-dynamic/src/lib.rs
--rw-r--r--   0        0        0     2035 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/Cargo.toml
--rw-r--r--   0     1001      123     1911 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/cpp.rs
--rw-r--r--   0     1001      123     1815 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/csharp.rs
--rw-r--r--   0     1001      123     1515 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/css.rs
--rw-r--r--   0     1001      123     2024 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/go.rs
--rw-r--r--   0     1001      123    10142 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/lib.rs
--rw-r--r--   0     1001      123     2990 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/parsers.rs
--rw-r--r--   0     1001      123     3114 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/python.rs
--rw-r--r--   0     1001      123     2915 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/rust.rs
--rw-r--r--   0     1001      123     2041 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/scala.rs
--rw-r--r--   0        0        0     1587 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.2/crates/cli/Cargo.toml
--rw-r--r--   0     1001      123      249 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/bin/ast-grep.rs
--rw-r--r--   0     1001      123    11003 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/config.rs
--rw-r--r--   0     1001      123    10194 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/error.rs
--rw-r--r--   0     1001      123     4312 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/lang.rs
--rw-r--r--   0     1001      123     4996 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/lib.rs
--rw-r--r--   0     1001      123     1015 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/lsp.rs
--rw-r--r--   0     1001      123       94 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/main.rs
--rw-r--r--   0     1001      123    10205 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/new.rs
--rw-r--r--   0     1001      123    22621 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/print/colored_print.rs
--rw-r--r--   0     1001      123     7648 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/print/interactive_print.rs
--rw-r--r--   0     1001      123     9327 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/print/json_print.rs
--rw-r--r--   0     1001      123     3179 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/print/mod.rs
--rw-r--r--   0     1001      123     9072 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/run.rs
--rw-r--r--   0     1001      123    10673 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/scan.rs
--rw-r--r--   0     1001      123     7418 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/utils.rs
--rw-r--r--   0     1001      123    24629 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/src/verify.rs
--rw-r--r--   0     1001      123      593 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/tests/common/mod.rs
--rw-r--r--   0     1001      123      971 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/tests/run_test.rs
--rw-r--r--   0     1001      123     1409 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/tests/scan_test.rs
--rw-r--r--   0     1001      123     1025 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/tests/verify_test.rs
--rw-r--r--   0     1001      123     1236 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/pyproject.toml
--rw-r--r--   0     1001      123    60241 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/crates/cli/Cargo.lock
--rw-r--r--   0     1001      123     4951 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/README.md
--rw-r--r--   0     1001      123     1077 2023-07-09 20:52:42.000000 ast_grep_cli-0.7.2/LICENSE
--rw-r--r--   0        0        0     6206 1970-01-01 00:00:00.000000 ast_grep_cli-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/Cargo.toml
+-rw-r--r--   0     1001      123     6946 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/constraints.rs
+-rw-r--r--   0     1001      123     6838 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/deserialize_env.rs
+-rw-r--r--   0     1001      123     4880 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/lib.rs
+-rw-r--r--   0     1001      123     2765 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/maybe.rs
+-rw-r--r--   0     1001      123     6514 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/referent_rule.rs
+-rw-r--r--   0     1001      123    16160 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/relational_rule/mod.rs
+-rw-r--r--   0     1001      123     4138 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs
+-rw-r--r--   0     1001      123    13151 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/rule.rs
+-rw-r--r--   0     1001      123     6357 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/rule_collection.rs
+-rw-r--r--   0     1001      123    11610 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/rule_config.rs
+-rw-r--r--   0     1001      123     6716 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/transform.rs
+-rw-r--r--   0        0        0      617 1970-01-01 00:00:00.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-dynamic/Cargo.toml
+-rw-r--r--   0     1001      123     7730 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-dynamic/src/lib.rs
+-rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/Cargo.toml
+-rw-r--r--   0     1001      123     2331 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/language.rs
+-rw-r--r--   0     1001      123     3858 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/lib.rs
+-rw-r--r--   0     1001      123    14850 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/match_tree.rs
+-rw-r--r--   0     1001      123     3480 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/matcher/kind.rs
+-rw-r--r--   0     1001      123     3783 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/matcher/node_match.rs
+-rw-r--r--   0     1001      123    11138 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/matcher/pattern.rs
+-rw-r--r--   0     1001      123      982 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/matcher/text.rs
+-rw-r--r--   0     1001      123     6540 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/matcher.rs
+-rw-r--r--   0     1001      123    11359 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/meta_var.rs
+-rw-r--r--   0     1001      123    15431 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/node.rs
+-rw-r--r--   0     1001      123    16351 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/ops.rs
+-rw-r--r--   0     1001      123     3089 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/pinned.rs
+-rw-r--r--   0     1001      123    10936 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/replacer/indent.rs
+-rw-r--r--   0     1001      123     6181 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/replacer/structural.rs
+-rw-r--r--   0     1001      123     9380 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/replacer/template.rs
+-rw-r--r--   0     1001      123     2572 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/replacer.rs
+-rw-r--r--   0     1001      123     8489 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/source.rs
+-rw-r--r--   0     1001      123    16414 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/traversal.rs
+-rw-r--r--   0        0        0     2035 1970-01-01 00:00:00.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/Cargo.toml
+-rw-r--r--   0     1001      123     1911 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/cpp.rs
+-rw-r--r--   0     1001      123     1815 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/csharp.rs
+-rw-r--r--   0     1001      123     1515 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/css.rs
+-rw-r--r--   0     1001      123     2024 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/go.rs
+-rw-r--r--   0     1001      123    10142 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/lib.rs
+-rw-r--r--   0     1001      123     2990 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/parsers.rs
+-rw-r--r--   0     1001      123     3114 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/python.rs
+-rw-r--r--   0     1001      123     2915 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/rust.rs
+-rw-r--r--   0     1001      123     2041 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/scala.rs
+-rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-lsp/Cargo.toml
+-rw-r--r--   0     1001      123    11369 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/local_dependencies/ast-grep-lsp/src/lib.rs
+-rw-r--r--   0        0        0     1587 1970-01-01 00:00:00.000000 ast_grep_cli-0.8.0/crates/cli/Cargo.toml
+-rw-r--r--   0     1001      123      249 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/bin/ast-grep.rs
+-rw-r--r--   0     1001      123    11003 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/config.rs
+-rw-r--r--   0     1001      123    10194 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/error.rs
+-rw-r--r--   0     1001      123     4312 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/lang.rs
+-rw-r--r--   0     1001      123     4996 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/lib.rs
+-rw-r--r--   0     1001      123     1015 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/lsp.rs
+-rw-r--r--   0     1001      123       94 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/main.rs
+-rw-r--r--   0     1001      123    10205 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/new.rs
+-rw-r--r--   0     1001      123    22621 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/print/colored_print.rs
+-rw-r--r--   0     1001      123     7648 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/print/interactive_print.rs
+-rw-r--r--   0     1001      123     9327 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/print/json_print.rs
+-rw-r--r--   0     1001      123     3179 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/print/mod.rs
+-rw-r--r--   0     1001      123     9039 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/run.rs
+-rw-r--r--   0     1001      123    10644 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/scan.rs
+-rw-r--r--   0     1001      123     7418 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/utils.rs
+-rw-r--r--   0     1001      123    24629 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/src/verify.rs
+-rw-r--r--   0     1001      123      593 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/tests/common/mod.rs
+-rw-r--r--   0     1001      123      901 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/tests/run_test.rs
+-rw-r--r--   0     1001      123     1363 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/tests/scan_test.rs
+-rw-r--r--   0     1001      123     1025 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/tests/verify_test.rs
+-rw-r--r--   0     1001      123     1236 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/pyproject.toml
+-rw-r--r--   0     1001      123    60241 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/crates/cli/Cargo.lock
+-rw-r--r--   0     1001      123     4951 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/README.md
+-rw-r--r--   0     1001      123     1077 2023-07-10 20:10:08.000000 ast_grep_cli-0.8.0/LICENSE
+-rw-r--r--   0        0        0     6206 1970-01-01 00:00:00.000000 ast_grep_cli-0.8.0/PKG-INFO
```

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-lsp/Cargo.toml` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-lsp/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [package]
 name = "ast-grep-lsp"
 description = "Search and Rewrite code at large scale using precise AST pattern"
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
-version= "0.7.2"
+version= "0.8.0"
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
 
 [dependencies]
```

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-lsp/src/lib.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-lsp/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/Cargo.toml` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 documentation= "https://ast-grep.github.io/guide/introduction.html"
 edition= "2021"
 homepage= "https://ast-grep.github.io/"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.7.2"
+version= "0.8.0"
 
 [dependencies]
 bit-set= { version = "0.5.3" }
 regex = { version = "1.9.1" , optional = true }
 thiserror= "1.0.43"
 tree-sitter= { version = "0.9.2", package = "tree-sitter-facade-sg" }
```

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/language.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/language.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/lib.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/match_tree.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/match_tree.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/matcher/kind.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/matcher/kind.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/matcher/node_match.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/matcher/node_match.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/matcher/pattern.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/matcher/pattern.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/matcher/text.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/matcher/text.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/matcher.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/matcher.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/meta_var.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/meta_var.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/node.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/node.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/ops.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/ops.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/pinned.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/pinned.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/replacer/indent.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/replacer/indent.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/replacer/structural.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/replacer/structural.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/replacer/template.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/replacer/template.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/replacer.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/replacer.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/source.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/source.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-core/src/traversal.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-core/src/traversal.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/Cargo.toml` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/Cargo.toml`

 * *Files 21% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.7.2"
+version= "0.8.0"
 
 [features]
 default = ["regex"]
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
```

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/constraints.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/constraints.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/deserialize_env.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/deserialize_env.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/lib.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/maybe.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/maybe.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/referent_rule.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/referent_rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/relational_rule/mod.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/relational_rule/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/relational_rule/stop_by.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/rule.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/rule.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/rule_collection.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/rule_collection.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/rule_config.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/rule_config.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-config/src/transform.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-config/src/transform.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-dynamic/Cargo.toml` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-dynamic/Cargo.toml`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.7.2"
+version= "0.8.0"
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
 
 ignore= { version = "0.4.20" }
 libloading = "0.8"
 serde= { version = "1.0", features = ["derive"] }
```

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-dynamic/src/lib.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-dynamic/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/Cargo.toml` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 license= "MIT"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
-version= "0.7.2"
+version= "0.8.0"
 
 [dependencies]
 ast-grep-core.path = "../ast-grep-core"
 
 ignore= { version = "0.4.20" }
 serde= { version = "1.0", features = ["derive"] }
```

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/cpp.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/cpp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/csharp.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/csharp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/css.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/css.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/go.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/go.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/lib.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/parsers.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/parsers.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/python.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/python.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/rust.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/rust.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/local_dependencies/ast-grep-language/src/scala.rs` & `ast_grep_cli-0.8.0/local_dependencies/ast-grep-language/src/scala.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/crates/cli/Cargo.toml` & `ast_grep_cli-0.8.0/crates/cli/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 keywords = ["ast", "pattern", "codemod", "search", "rewrite"]
 categories = ["command-line-utilities", "development-tools", "parsing"]
 default-run = "sg"
 # use relative path because maturin does not recognize
 readme = "../../README.md"
 license-file = "../../LICENSE"
 
-version= "0.7.2"
+version= "0.8.0"
 authors= ["Herrington Darkholme <2883231+HerringtonDarkholme@users.noreply.github.com>"]
 edition= "2021"
 # license.workspace = true
 documentation= "https://ast-grep.github.io/guide/introduction.html"
 homepage= "https://ast-grep.github.io/"
 repository= "https://github.com/ast-grep/ast-grep"
 rust-version= "1.63"
```

### Comparing `ast_grep_cli-0.7.2/crates/cli/src/config.rs` & `ast_grep_cli-0.8.0/crates/cli/src/config.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/crates/cli/src/error.rs` & `ast_grep_cli-0.8.0/crates/cli/src/error.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/crates/cli/src/lang.rs` & `ast_grep_cli-0.8.0/crates/cli/src/lang.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/crates/cli/src/lib.rs` & `ast_grep_cli-0.8.0/crates/cli/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/crates/cli/src/lsp.rs` & `ast_grep_cli-0.8.0/crates/cli/src/lsp.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/crates/cli/src/new.rs` & `ast_grep_cli-0.8.0/crates/cli/src/new.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/crates/cli/src/print/colored_print.rs` & `ast_grep_cli-0.8.0/crates/cli/src/print/colored_print.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/crates/cli/src/print/interactive_print.rs` & `ast_grep_cli-0.8.0/crates/cli/src/print/interactive_print.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/crates/cli/src/print/json_print.rs` & `ast_grep_cli-0.8.0/crates/cli/src/print/json_print.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/crates/cli/src/print/mod.rs` & `ast_grep_cli-0.8.0/crates/cli/src/print/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/crates/cli/src/run.rs` & `ast_grep_cli-0.8.0/crates/cli/src/run.rs`

 * *Files 3% similar despite different names*

```diff
@@ -83,41 +83,41 @@
   color: ColorArg,
 
   /// Do not respect hidden file system or ignore files (.gitignore, .ignore, etc.).
   /// You can suppress multiple ignore files by passing `no-ignore` multiple times.
   #[clap(long, action = clap::ArgAction::Append)]
   no_ignore: Vec<IgnoreFile>,
 
-  /// Disable search code from StdIn.
+  /// Enable search code from StdIn.
   ///
-  /// Use this if you need search files but ast-grep is launched from another process.
-  /// You can also use the environment variable `AST_GREP_NO_STDIN` to disable StdIn mode.
+  /// Use this if you need to take code stream from standard input.
+  /// If the environment variable `AST_GREP_NO_STDIN` exist, ast-grep will disable StdIn mode.
   #[clap(long)]
-  no_stdin: bool,
+  stdin: bool,
 }
 
 // Every run will include Search or Replace
 // Search or Replace by arguments `pattern` and `rewrite` passed from CLI
 pub fn run_with_pattern(arg: RunArg) -> Result<()> {
   if arg.json {
     return run_pattern_with_printer(arg, JSONPrinter::stdout());
   }
   let printer = ColoredPrinter::stdout(arg.color).heading(arg.heading);
   let interactive = arg.interactive || arg.accept_all;
   if interactive {
-    let from_stdin = !arg.no_stdin && is_from_stdin();
+    let from_stdin = arg.stdin && is_from_stdin();
     let printer = InteractivePrinter::new(printer, arg.accept_all, from_stdin)?;
     run_pattern_with_printer(arg, printer)
   } else {
     run_pattern_with_printer(arg, printer)
   }
 }
 
 fn run_pattern_with_printer(arg: RunArg, printer: impl Printer + Sync) -> Result<()> {
-  if !arg.no_stdin && is_from_stdin() {
+  if arg.stdin && is_from_stdin() {
     run_std_in(RunWithSpecificLang::new(arg, printer)?)
   } else if arg.lang.is_some() {
     run_worker(RunWithSpecificLang::new(arg, printer)?)
   } else {
     run_worker(RunWithInferredLang { arg, printer })
   }
 }
@@ -266,15 +266,15 @@
   #[test]
   fn test_run_with_pattern() {
     let arg = RunArg {
       pattern: "console.log".to_string(),
       rewrite: None,
       color: ColorArg::Never,
       no_ignore: vec![],
-      no_stdin: true,
+      stdin: false,
       interactive: false,
       lang: None,
       json: false,
       heading: Heading::Never,
       debug_query: false,
       accept_all: false,
       paths: vec![PathBuf::from(".")],
@@ -291,13 +291,13 @@
       no_ignore: vec![],
       interactive: false,
       lang: Some(SupportLang::Rust.into()),
       json: false,
       heading: Heading::Never,
       debug_query: false,
       accept_all: false,
-      no_stdin: false,
+      stdin: true,
       paths: vec![PathBuf::from(".")],
     };
     assert!(run_with_pattern(arg).is_ok())
   }
 }
```

### Comparing `ast_grep_cli-0.7.2/crates/cli/src/scan.rs` & `ast_grep_cli-0.8.0/crates/cli/src/scan.rs`

 * *Files 4% similar despite different names*

```diff
@@ -53,41 +53,41 @@
   #[clap(value_parser, default_value = ".")]
   paths: Vec<PathBuf>,
 
   /// Do not respect ignore files. You can suppress multiple ignore files by passing `no-ignore` multiple times.
   #[clap(long, action = clap::ArgAction::Append)]
   no_ignore: Vec<IgnoreFile>,
 
-  /// Disable search code from StdIn.
+  /// Enable search code from StdIn.
   ///
-  /// Use this if you need search files but ast-grep is launched from another process.
-  /// You can also use the environment variable `AST_GREP_NO_STDIN` to disable StdIn mode.
+  /// Use this if you need to take code stream from standard input.
+  /// If the environment variable `AST_GREP_NO_STDIN` exist, ast-grep will disable StdIn mode.
   #[clap(long)]
-  no_stdin: bool,
+  stdin: bool,
 }
 
 pub fn run_with_config(arg: ScanArg) -> Result<()> {
   register_custom_language(arg.config.clone());
   if arg.json {
     let printer = JSONPrinter::stdout();
     return run_scan(arg, printer);
   }
   let printer = ColoredPrinter::stdout(arg.color).style(arg.report_style);
   let interactive = arg.interactive || arg.accept_all;
   if interactive {
-    let from_stdin = !arg.no_stdin && is_from_stdin();
+    let from_stdin = arg.stdin && is_from_stdin();
     let printer = InteractivePrinter::new(printer, arg.accept_all, from_stdin)?;
     run_scan(arg, printer)
   } else {
     run_scan(arg, printer)
   }
 }
 
 fn run_scan<P: Printer + Sync>(arg: ScanArg, printer: P) -> Result<()> {
-  if !arg.no_stdin && is_from_stdin() {
+  if arg.stdin && is_from_stdin() {
     let worker = ScanWithRule::try_new(arg, printer)?;
     run_std_in(worker)
   } else {
     let worker = ScanWithConfig::try_new(arg, printer)?;
     run_worker(worker)
   }
 }
@@ -344,12 +344,12 @@
       report_style: ReportStyle::Rich,
       color: ColorArg::Never,
       no_ignore: vec![],
       interactive: false,
       json: false,
       accept_all: false,
       paths: vec![PathBuf::from(".")],
-      no_stdin: true,
+      stdin: false,
     };
     assert!(run_with_config(arg).is_ok());
   }
 }
```

### Comparing `ast_grep_cli-0.7.2/crates/cli/src/utils.rs` & `ast_grep_cli-0.8.0/crates/cli/src/utils.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/crates/cli/src/verify.rs` & `ast_grep_cli-0.8.0/crates/cli/src/verify.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/crates/cli/tests/common/mod.rs` & `ast_grep_cli-0.8.0/crates/cli/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/crates/cli/tests/run_test.rs` & `ast_grep_cli-0.8.0/crates/cli/tests/run_test.rs`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,27 @@
 use predicates::prelude::*;
 use predicates::str::contains;
 
 #[test]
 fn test_simple_infer_lang() -> Result<()> {
   let dir = create_test_files([("a.ts", "console.log(123)"), ("b.rs", "console.log(456)")])?;
   Command::cargo_bin("sg")?
-    .env("AST_GREP_NO_STDIN", "1")
     .current_dir(dir.path())
     .args(["-p", "console.log($A)"])
     .assert()
     .success()
     .stdout(contains("console.log(123)"))
     .stdout(contains("console.log(456)"));
   Ok(())
 }
 
 #[test]
 fn test_simple_specific_lang() -> Result<()> {
   let dir = create_test_files([("a.ts", "console.log(123)"), ("b.rs", "console.log(456)")])?;
   Command::cargo_bin("sg")?
-    .env("AST_GREP_NO_STDIN", "1")
     .current_dir(dir.path())
     .args(["-p", "console.log($A)", "-l", "rs"])
     .assert()
     .success()
     .stdout(contains("console.log(123)").not())
     .stdout(contains("console.log(456)"));
   Ok(())
```

### Comparing `ast_grep_cli-0.7.2/crates/cli/tests/scan_test.rs` & `ast_grep_cli-0.8.0/crates/cli/tests/scan_test.rs`

 * *Files 10% similar despite different names*

```diff
@@ -47,25 +47,24 @@
   main_with_args(args)
 }
 
 #[test]
 fn test_sg_scan() -> Result<()> {
   let dir = setup()?;
   let config = dir.path().join("sgconfig.yml");
-  let ret = sg(&format!("sg scan -c {} --no-stdin", config.display()));
+  let ret = sg(&format!("sg scan -c {}", config.display()));
   assert!(ret.is_ok());
   drop(dir);
   Ok(())
 }
 
 #[test]
 fn test_sg_rule_off() -> Result<()> {
   let dir = setup()?;
   Command::cargo_bin("sg")?
-    .env("AST_GREP_NO_STDIN", "1")
     .current_dir(dir.path())
     .args(["scan"])
     .assert()
     .success()
     .stdout(contains("on-rule"))
     .stdout(contains("off-rule").not());
   drop(dir);
```

### Comparing `ast_grep_cli-0.7.2/crates/cli/tests/verify_test.rs` & `ast_grep_cli-0.8.0/crates/cli/tests/verify_test.rs`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/pyproject.toml` & `ast_grep_cli-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "ast-grep-cli"
-version = "0.7.2"
+version = "0.8.0"
 description = "Structural Search and Rewrite code at large scale using precise AST pattern."
 authors = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 maintainers = [{ name = "Herrington Darkholme", email = "2883231+HerringtonDarkholme@users.noreply.github.com" }]
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = [
   "ast",
```

### Comparing `ast_grep_cli-0.7.2/crates/cli/Cargo.lock` & `ast_grep_cli-0.8.0/crates/cli/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
  "predicates-core",
  "predicates-tree",
  "wait-timeout",
 ]
 
 [[package]]
 name = "ast-grep"
-version = "0.7.2"
+version = "0.8.0"
 dependencies = [
  "ansi_term",
  "anyhow",
  "assert_cmd",
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-dynamic",
@@ -131,15 +131,15 @@
  "similar",
  "tempdir",
  "tokio",
 ]
 
 [[package]]
 name = "ast-grep-config"
-version = "0.7.2"
+version = "0.8.0"
 dependencies = [
  "anyhow",
  "ast-grep-core",
  "bit-set",
  "globset",
  "regex",
  "serde",
@@ -147,38 +147,38 @@
  "tempdir",
  "thiserror",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-core"
-version = "0.7.2"
+version = "0.8.0"
 dependencies = [
  "bit-set",
  "regex",
  "thiserror",
  "tree-sitter-facade-sg",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-dynamic"
-version = "0.7.2"
+version = "0.8.0"
 dependencies = [
  "ast-grep-core",
  "ignore",
  "libloading 0.8.0",
  "serde",
  "thiserror",
  "tree-sitter",
 ]
 
 [[package]]
 name = "ast-grep-language"
-version = "0.7.2"
+version = "0.8.0"
 dependencies = [
  "ast-grep-core",
  "ast-grep-tree-sitter-c-sharp",
  "ignore",
  "serde",
  "tree-sitter-c",
  "tree-sitter-cpp",
@@ -196,27 +196,27 @@
  "tree-sitter-swift",
  "tree-sitter-thrift",
  "tree-sitter-typescript",
 ]
 
 [[package]]
 name = "ast-grep-lsp"
-version = "0.7.2"
+version = "0.8.0"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "dashmap",
  "serde",
  "serde_json",
  "tower-lsp",
 ]
 
 [[package]]
 name = "ast-grep-napi"
-version = "0.7.2"
+version = "0.8.0"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ignore",
  "napi",
  "napi-build",
  "napi-derive",
@@ -277,15 +277,15 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "benches"
-version = "0.7.2"
+version = "0.8.0"
 dependencies = [
  "ast-grep-config",
  "ast-grep-core",
  "ast-grep-language",
  "criterion",
 ]
```

### Comparing `ast_grep_cli-0.7.2/README.md` & `ast_grep_cli-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/LICENSE` & `ast_grep_cli-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ast_grep_cli-0.7.2/PKG-INFO` & `ast_grep_cli-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ast-grep-cli
-Version: 0.7.2
+Version: 0.8.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Security
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ast-grep-cli Version: 0.7.2 Classifier: Development
+Metadata-Version: 2.1 Name: ast-grep-cli Version: 0.8.0 Classifier: Development
 Status :: 3 - Alpha Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Rust Classifier: Topic :: Security Classifier: Topic :: Software Development
 :: Quality Assurance Classifier: Topic :: Software Development Classifier:
 Topic :: Text Processing License-File: LICENSE License-File: LICENSE Summary:
 Structural Search and Rewrite code at large scale using precise AST pattern.
```


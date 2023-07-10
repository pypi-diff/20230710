# Comparing `tmp/robotcode_language_server-0.46.0.tar.gz` & `tmp/robotcode_language_server-0.47.0.tar.gz`

## Comparing `robotcode_language_server-0.46.0.tar` & `robotcode_language_server-0.47.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/__version__.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/cli.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/__init__.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/decorators.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/has_extend_capabilities.py
--rw-r--r--   0        0        0    12397 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/protocol.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/server.py
--rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/text_document.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/__init__.py
--rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/code_action.py
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/code_lens.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/commands.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/completion.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/declaration.py
--rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/definition.py
--rw-r--r--   0        0        0    21103 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/diagnostics.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/document_highlight.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/document_symbols.py
--rw-r--r--   0        0        0    15048 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/documents.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/folding_range.py
--rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/formatting.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/hover.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/implementation.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/inlay_hint.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/inline_value.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/protocol_part.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/references.py
--rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/rename.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/selection_range.py
--rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/semantic_tokens.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/signature_help.py
--rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/window.py
--rw-r--r--   0        0        0    19239 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/workspace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/__init__.py
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/configuration.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/languages.py
--rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/protocol.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/diagnostics/__init__.py
--rw-r--r--   0        0        0    39564 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
--rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/diagnostics/entities.py
--rw-r--r--   0        0        0    58494 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
--rw-r--r--   0        0        0    68132 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
--rw-r--r--   0        0        0    83910 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/__init__.py
--rw-r--r--   0        0        0    15318 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
--rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
--rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/codelens.py
--rw-r--r--   0        0        0    85362 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/completion.py
--rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py
--rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/diagnostics.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/document_highlight.py
--rw-r--r--   0        0        0     9868 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/document_symbols.py
--rw-r--r--   0        0        0    19395 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/documents_cache.py
--rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/folding_range.py
--rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/formatting.py
--rw-r--r--   0        0        0    26508 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/goto.py
--rw-r--r--   0        0        0    23815 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/hover.py
--rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/inline_value.py
--rw-r--r--   0        0        0    24217 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/model_helper.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/protocol_part.py
--rw-r--r--   0        0        0    19638 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/references.py
--rw-r--r--   0        0        0    24952 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/rename.py
--rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
--rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/selection_range.py
--rw-r--r--   0        0        0    42889 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
--rw-r--r--   0        0        0    15705 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/signature_help.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/utils/__init__.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/utils/_variables.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/utils/ast_utils.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/utils/async_ast.py
--rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/utils/match.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/utils/robot_path.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/utils/variables.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/utils/version.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/LICENSE.txt
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/README.md
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/pyproject.toml
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 robotcode_language_server-0.46.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/__version__.py
+-rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/cli.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/__init__.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/decorators.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/has_extend_capabilities.py
+-rw-r--r--   0        0        0    12397 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/protocol.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/server.py
+-rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/text_document.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/__init__.py
+-rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/code_action.py
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/code_lens.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/commands.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/completion.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/declaration.py
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/definition.py
+-rw-r--r--   0        0        0    21103 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/diagnostics.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/document_highlight.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/document_symbols.py
+-rw-r--r--   0        0        0    15048 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/documents.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/folding_range.py
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/formatting.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/hover.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/implementation.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/inline_value.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/protocol_part.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/references.py
+-rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/rename.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/selection_range.py
+-rw-r--r--   0        0        0     6963 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/semantic_tokens.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/signature_help.py
+-rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/window.py
+-rw-r--r--   0        0        0    19239 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/workspace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/__init__.py
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/configuration.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/languages.py
+-rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/protocol.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/diagnostics/__init__.py
+-rw-r--r--   0        0        0    40988 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
+-rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/diagnostics/entities.py
+-rw-r--r--   0        0        0    58866 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
+-rw-r--r--   0        0        0    71453 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
+-rw-r--r--   0        0        0    83910 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/__init__.py
+-rw-r--r--   0        0        0    15318 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
+-rw-r--r--   0        0        0     7151 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
+-rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/codelens.py
+-rw-r--r--   0        0        0    89225 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/completion.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py
+-rw-r--r--   0        0        0    16867 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/diagnostics.py
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/document_highlight.py
+-rw-r--r--   0        0        0     9868 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/document_symbols.py
+-rw-r--r--   0        0        0    19395 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/documents_cache.py
+-rw-r--r--   0        0        0     4384 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/folding_range.py
+-rw-r--r--   0        0        0     8495 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/formatting.py
+-rw-r--r--   0        0        0    26508 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/goto.py
+-rw-r--r--   0        0        0    23815 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/hover.py
+-rw-r--r--   0        0        0     8872 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/inline_value.py
+-rw-r--r--   0        0        0    24217 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/model_helper.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/protocol_part.py
+-rw-r--r--   0        0        0    19638 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/references.py
+-rw-r--r--   0        0        0    24952 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/rename.py
+-rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
+-rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/selection_range.py
+-rw-r--r--   0        0        0    42889 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
+-rw-r--r--   0        0        0    15705 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/signature_help.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/utils/__init__.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/utils/_variables.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/utils/ast_utils.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/utils/async_ast.py
+-rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/utils/match.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/utils/robot_path.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/utils/variables.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/utils/version.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/LICENSE.txt
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/README.md
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/pyproject.toml
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 robotcode_language_server-0.47.0/PKG-INFO
```

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/cli.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 
     with RobotLanguageServer(
         mode=mode, tcp_params=TcpParams(addresses or "127.0.0.1", port), pipe_name=pipe_name, profile=profile
     ) as server:
         server.run()
 
 
+# mypy: disable-error-code="misc, arg-type, attr-defined"
+
+
 @click.command(
     add_help_option=True,
     epilog='Use "-- --help" to see `robot` help.',
 )
 @add_options(
     *server_options(
         ServerMode.STDIO,
```

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/decorators.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/decorators.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/protocol.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/server.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/text_document.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/text_document.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/code_action.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/code_action.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/code_lens.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/code_lens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/commands.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/commands.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/completion.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/completion.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/declaration.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/declaration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/definition.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/definition.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/diagnostics.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/document_highlight.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/document_symbols.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/documents.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/documents.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/folding_range.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/formatting.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/hover.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/implementation.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/implementation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/inlay_hint.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/inline_value.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/references.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/rename.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/selection_range.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/semantic_tokens.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/signature_help.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/window.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/window.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/common/parts/workspace.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/common/parts/workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/configuration.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/configuration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/protocol.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/server.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py`

 * *Files 8% similar despite different names*

```diff
@@ -879,27 +879,56 @@
                     message=d.message,
                     severity=d.severity,
                     code=d.code,
                 )
 
         await self.generic_visit(node)
 
+    async def visit_ForceTags(self, node: ast.AST) -> None:  # noqa: N802
+        from robot.parsing.lexer.tokens import Token as RobotToken
+        from robot.parsing.model.statements import ForceTags
+
+        if get_robot_version() >= (6, 0):
+            tag = cast(ForceTags, node).get_token(RobotToken.FORCE_TAGS)
+            if tag.value.upper() == "FORCE TAGS":
+                self.append_diagnostics(
+                    range=range_from_node_or_token(node, tag),
+                    message="`Force Tags` is deprecated in favour of new `Test Tags` setting.",
+                    severity=DiagnosticSeverity.INFORMATION,
+                    tags=[DiagnosticTag.DEPRECATED],
+                    code="DeprecatedHyphenTag",
+                )
+
+    async def visit_DefaultTags(self, node: ast.AST) -> None:  # noqa: N802
+        from robot.parsing.lexer.tokens import Token as RobotToken
+        from robot.parsing.model.statements import ForceTags
+
+        if get_robot_version() >= (6, 0):
+            tag = cast(ForceTags, node).get_token(RobotToken.DEFAULT_TAGS)
+            self.append_diagnostics(
+                range=range_from_node_or_token(node, tag),
+                message="`Force Tags` is deprecated in favour of new `Test Tags` setting.",
+                severity=DiagnosticSeverity.INFORMATION,
+                tags=[DiagnosticTag.DEPRECATED],
+                code="DeprecatedHyphenTag",
+            )
+
     async def visit_Tags(self, node: ast.AST) -> None:  # noqa: N802
         from robot.parsing.lexer.tokens import Token as RobotToken
         from robot.parsing.model.statements import Tags
 
         if get_robot_version() >= (6, 0):
             tags = cast(Tags, node)
 
             for tag in tags.get_tokens(RobotToken.ARGUMENT):
                 if tag.value and tag.value.startswith("-"):
                     self.append_diagnostics(
                         range=range_from_node_or_token(node, tag),
                         message=f"Settings tags starting with a hyphen using the '[Tags]' setting "
-                        f"is deprecated. In Robot Framework 5.2 this syntax will be used "
+                        f"is deprecated. In Robot Framework 7.0 this syntax will be used "
                         f"for removing tags. Escape '{tag.value}' like '\\{tag.value}' to use the "
                         f"literal value and to avoid this warning.",
                         severity=DiagnosticSeverity.WARNING,
                         tags=[DiagnosticTag.DEPRECATED],
                         code="DeprecatedHyphenTag",
                     )
```

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/diagnostics/entities.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/diagnostics/entities.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1099,28 +1099,36 @@
                                 f"Failed to load library meta data for library {name} from {spec_path}"
                             ) from e
                     except (SystemExit, KeyboardInterrupt):
                         raise
                     except BaseException as e:
                         self._logger.exception(e)
 
-            with ProcessPoolExecutor(max_workers=1, mp_context=mp.get_context("spawn")) as executor:
+            executor = ProcessPoolExecutor(max_workers=1, mp_context=mp.get_context("spawn"))
+            try:
                 result = await asyncio.wait_for(
                     asyncio.get_running_loop().run_in_executor(
                         executor,
                         get_library_doc,
                         name,
                         args,
                         working_dir,
                         base_dir,
                         await self.get_resolvable_command_line_variables(),
                         variables,
                     ),
                     LOAD_LIBRARY_TIME_OUT,
                 )
+            except (SystemExit, KeyboardInterrupt):
+                raise
+            except BaseException as e:
+                self._logger.exception(e)
+                raise
+            finally:
+                executor.shutdown(wait=True)
 
             if result.stdout:
                 self._logger.warning(lambda: f"stdout captured at loading library {name}{args!r}:\n{result.stdout}")
             try:
                 if meta is not None:
                     meta_file = Path(self.lib_doc_cache_path, meta.filepath_base.with_suffix(".meta.json"))
                     spec_file = Path(self.lib_doc_cache_path, meta.filepath_base.with_suffix(".spec.json"))
@@ -1346,54 +1354,61 @@
                                 f"Failed to load library meta data for library {name} from {spec_path}"
                             ) from e
                     except (SystemExit, KeyboardInterrupt):
                         raise
                     except BaseException as e:
                         self._logger.exception(e)
 
-            with ProcessPoolExecutor(max_workers=1, mp_context=mp.get_context("spawn")) as executor:
+            executor = ProcessPoolExecutor(max_workers=1, mp_context=mp.get_context("spawn"))
+            try:
                 result = await asyncio.wait_for(
                     asyncio.get_running_loop().run_in_executor(
                         executor,
                         get_variables_doc,
                         name,
                         args,
                         str(self.folder.to_path()),
                         base_dir,
                         await self.get_resolvable_command_line_variables() if resolve_command_line_vars else None,
                         variables,
                     ),
                     LOAD_LIBRARY_TIME_OUT,
                 )
+            except (SystemExit, KeyboardInterrupt):
+                raise
+            except BaseException as e:
+                self._logger.exception(e)
+                raise
+            finally:
+                executor.shutdown(True)
 
-                if result.stdout:
-                    self._logger.warning(
-                        lambda: f"stdout captured at loading variables {name}{args!r}:\n{result.stdout}"
-                    )
+            if result.stdout:
+                self._logger.warning(lambda: f"stdout captured at loading variables {name}{args!r}:\n{result.stdout}")
 
-                try:
-                    if meta is not None:
-                        meta_file = Path(self.variables_doc_cache_path, meta.filepath_base.with_suffix(".meta.json"))
-                        spec_file = Path(self.variables_doc_cache_path, meta.filepath_base.with_suffix(".spec.json"))
-                        spec_file.parent.mkdir(parents=True, exist_ok=True)
+            try:
+                if meta is not None:
+                    meta_file = Path(self.variables_doc_cache_path, meta.filepath_base.with_suffix(".meta.json"))
+                    spec_file = Path(self.variables_doc_cache_path, meta.filepath_base.with_suffix(".spec.json"))
+                    spec_file.parent.mkdir(parents=True, exist_ok=True)
 
-                        try:
-                            spec_file.write_text(as_json(result), "utf-8")
-                        except (SystemExit, KeyboardInterrupt):
-                            raise
-                        except BaseException as e:
-                            raise RuntimeError(f"Cannot write spec file for variables '{name}' to '{spec_file}'") from e
-                        meta_file.write_text(as_json(meta), "utf-8")
-                    else:
-                        self._logger.debug(lambda: f"Skip caching variables {name}{args!r}")
-                except (SystemExit, KeyboardInterrupt):
-                    raise
-                except BaseException as e:
-                    self._logger.exception(e)
-                return result
+                    try:
+                        spec_file.write_text(as_json(result), "utf-8")
+                    except (SystemExit, KeyboardInterrupt):
+                        raise
+                    except BaseException as e:
+                        raise RuntimeError(f"Cannot write spec file for variables '{name}' to '{spec_file}'") from e
+                    meta_file.write_text(as_json(meta), "utf-8")
+                else:
+                    self._logger.debug(lambda: f"Skip caching variables {name}{args!r}")
+            except (SystemExit, KeyboardInterrupt):
+                raise
+            except BaseException as e:
+                self._logger.exception(e)
+
+            return result
 
         resolved_args = resolve_args(
             args,
             str(self.folder.to_path()),
             base_dir,
             await self.get_resolvable_command_line_variables() if resolve_command_line_vars else None,
             variables,
```

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py`

 * *Files 2% similar despite different names*

```diff
@@ -847,21 +847,65 @@
                 entries.append("Keywords")
             # TODO if self.data_types:
             #    entries.append("Data types")
 
         return "\n".join(f"- [{entry}](#{entry.lower().replace(' ', '-')})" for entry in entries)
 
 
+def var_repr(value: Any) -> str:
+    if value is None:
+        return ""
+
+    if isinstance(value, NativeValue):
+        value = value.value
+
+    if value is None:
+        return "${None}"
+
+    if isinstance(value, (int, float, bool)):
+        return f"${{{value!r}}}"
+
+    if isinstance(value, str) and value == "":
+        return "${EMPTY}"
+
+    if isinstance(value, str) and value == " ":
+        return "${SPACE}"
+
+    if isinstance(value, str):
+        return value
+
+    return "${{ " + repr(value) + " }}"
+
+
 @dataclass
 class VariablesDoc(LibraryDoc):
     type: str = "VARIABLES"
     scope: str = "GLOBAL"
 
     variables: List[ImportedVariableDefinition] = field(default_factory=list)
 
+    def to_markdown(self, add_signature: bool = True, only_doc: bool = True, header_level: int = 2) -> str:
+        result = super().to_markdown(add_signature, only_doc, header_level)
+
+        if self.variables:
+            result += "\n---\n\n"
+
+            result += "\n```robotframework"
+            result += "\n*** Variables ***"
+
+            for var in self.variables:
+                result += "\n" + var.name
+                if var.has_value:
+                    result += "    " + var_repr(var.value)
+                else:
+                    result += "    ..."
+            result += "\n```"
+
+        return result
+
 
 def is_library_by_path(path: str) -> bool:
     return path.lower().endswith((".py", "/", os.sep))
 
 
 def is_variables_by_path(path: str) -> bool:
     if get_robot_version() >= (6, 1):
@@ -1559,37 +1603,41 @@
     working_dir: str = ".",
     base_dir: str = ".",
     command_line_variables: Optional[Dict[str, Optional[Any]]] = None,
     variables: Optional[Dict[str, Optional[Any]]] = None,
 ) -> VariablesDoc:
     from robot.libdocpkg.robotbuilder import KeywordDocBuilder
     from robot.output import LOGGER
-    from robot.running.handlers import _PythonHandler
+    from robot.running.handlers import _PythonHandler, _PythonInitHandler
     from robot.utils.importer import Importer
     from robot.variables.filesetter import PythonImporter, YamlImporter
 
     if get_robot_version() >= (6, 1):
         from robot.variables.filesetter import JsonImporter
 
     import_name: str = name
     stem = Path(name).stem
     module_spec: Optional[ModuleSpec] = None
     source: Optional[str] = None
     try:
+        python_import = False
+
         with _std_capture() as std_capturer:
             import_name = find_variables(name, working_dir, base_dir, command_line_variables, variables)
             get_variables = None
 
             if import_name.lower().endswith((".yaml", ".yml")):
                 source = import_name
                 importer = YamlImporter()
             elif get_robot_version() >= (6, 1) and import_name.lower().endswith(".json"):
                 source = import_name
                 importer = JsonImporter()
             else:
+                python_import = True
+
                 if not is_variables_by_path(import_name):
                     module_spec = get_module_spec(import_name)
 
                 # skip antigravity easter egg
                 # see https://python-history.blogspot.com/2010/06/import-antigravity.html
                 if import_name.lower() in ["antigravity"] or import_name.lower().endswith("antigravity.py"):
                     raise IgnoreEasterEggLibraryWarning(f"Ignoring import for python easter egg '{import_name}'.")
@@ -1641,51 +1689,88 @@
                 source=source or module_spec.origin if module_spec is not None else import_name,
                 module_spec=module_spec,
                 variables=vars,
                 stdout=std_capturer.getvalue(),
                 python_path=sys.path,
             )
 
-            if get_variables is not None:
-
-                class VarHandler(_PythonHandler):
-                    def _get_name(self, handler_name: Any, handler_method: Any) -> Any:
-                        return get_variables.__name__ if get_variables is not None else ""
+            if python_import:
+                if get_variables is not None:
 
-                    def _get_initial_handler(self, library: Any, name: Any, method: Any) -> Any:
-                        return None
-
-                vars_initializer = VarHandler(libdoc, get_variables.__name__, get_variables)
+                    class VarHandler(_PythonHandler):
+                        def _get_name(self, handler_name: Any, handler_method: Any) -> Any:
+                            return get_variables.__name__ if get_variables is not None else ""
+
+                        def _get_initial_handler(self, library: Any, name: Any, method: Any) -> Any:
+                            return None
+
+                    vars_initializer = VarHandler(libdoc, get_variables.__name__, get_variables)
+
+                    libdoc.inits = KeywordStore(
+                        keywords=[
+                            KeywordDoc(
+                                name=libdoc.name,
+                                args=[KeywordArgumentDoc.from_robot(a) for a in kw[0].args],
+                                doc=kw[0].doc,
+                                source=kw[0].source,
+                                line_no=kw[0].lineno if kw[0].lineno is not None else -1,
+                                col_offset=-1,
+                                end_col_offset=-1,
+                                end_line_no=-1,
+                                type="library",
+                                libname=libdoc.name,
+                                libtype=libdoc.type,
+                                longname=f"{libdoc.name}.{kw[0].name}",
+                                is_initializer=True,
+                                arguments=ArgumentSpec.from_robot_argument_spec(kw[1].arguments),
+                                parent=libdoc.digest,
+                            )
+                            for kw in [
+                                (KeywordDocBuilder().build_keyword(k), k)
+                                for k in [KeywordWrapper(vars_initializer, libdoc.source or "")]
+                            ]
+                        ]
+                    )
+                else:
+                    get_variables = getattr(libcode, "__init__", None) or getattr(libcode, "__init__", None)
 
-                libdoc.inits = KeywordStore(
-                    keywords=[
-                        KeywordDoc(
-                            name=libdoc.name,
-                            args=[KeywordArgumentDoc.from_robot(a) for a in kw[0].args],
-                            doc=kw[0].doc,
-                            tags=list(kw[0].tags),
-                            source=kw[0].source,
-                            line_no=kw[0].lineno if kw[0].lineno is not None else -1,
-                            col_offset=-1,
-                            end_col_offset=-1,
-                            end_line_no=-1,
-                            type="library",
-                            libname=libdoc.name,
-                            libtype=libdoc.type,
-                            longname=f"{libdoc.name}.{kw[0].name}",
-                            is_initializer=True,
-                            arguments=ArgumentSpec.from_robot_argument_spec(kw[1].arguments),
-                            parent=libdoc.digest,
+                    class InitVarHandler(_PythonInitHandler):
+                        def _get_name(self, handler_name: Any, handler_method: Any) -> Any:
+                            return get_variables.__name__ if get_variables is not None else ""
+
+                        def _get_initial_handler(self, library: Any, name: Any, method: Any) -> Any:
+                            return None
+
+                    if get_variables is not None:
+                        vars_initializer = InitVarHandler(libdoc, get_variables.__name__, get_variables, None)
+
+                        libdoc.inits = KeywordStore(
+                            keywords=[
+                                KeywordDoc(
+                                    name=libdoc.name,
+                                    args=[],
+                                    doc=kw[0].doc,
+                                    source=kw[0].source,
+                                    line_no=kw[0].lineno if kw[0].lineno is not None else -1,
+                                    col_offset=-1,
+                                    end_col_offset=-1,
+                                    end_line_no=-1,
+                                    type="library",
+                                    libname=libdoc.name,
+                                    libtype=libdoc.type,
+                                    longname=f"{libdoc.name}.{kw[0].name}",
+                                    is_initializer=True,
+                                    parent=libdoc.digest,
+                                )
+                                for kw in [
+                                    (KeywordDocBuilder().build_keyword(k), k)
+                                    for k in [KeywordWrapper(vars_initializer, libdoc.source or "")]
+                                ]
+                            ]
                         )
-                        for kw in [
-                            (KeywordDocBuilder().build_keyword(k), k)
-                            for k in [KeywordWrapper(vars_initializer, libdoc.source or "")]
-                        ]
-                    ]
-                )
 
             return libdoc
     except (SystemExit, KeyboardInterrupt, IgnoreEasterEggLibraryWarning):
         raise
     except BaseException as e:
         return VariablesDoc(
             name=stem,
```

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/codelens.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/codelens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/completion.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -2105,7 +2105,111 @@
         from robot.parsing.model.statements import Fixture
 
         name_token = cast(Fixture, node).get_token(RobotToken.NAME)
         if name_token is None or name_token.value is None or name_token.value.upper() in ("", "NONE"):
             return None
 
         return await self._complete_KeywordCall_or_Fixture(RobotToken.NAME, node, nodes_at_position, position, context)
+
+    async def create_tags_completion_items(self, range: Optional[Range]) -> List[CompletionItem]:
+        built_in_tags = {
+            "robot:continue-on-failure",
+            "robot:stop-on-failure",
+            "robot:no-dry-run",
+            "robot:exit",
+        }
+
+        if get_robot_version() >= (5, 0):
+            built_in_tags.add("robot:skip")
+            built_in_tags.add("robot:skip-on-failure")
+            built_in_tags.add("robot:exclude")
+            built_in_tags.add("robot:recursive-continue-on-failure")
+
+        if get_robot_version() >= (6, 0):
+            built_in_tags.add("robot:recursive-stop-on-failure")
+            built_in_tags.add("robot:private")
+
+        if get_robot_version() >= (6, 1):
+            built_in_tags.add("robot:flatten")
+
+        return [
+            CompletionItem(
+                label=tag,
+                kind=CompletionItemKind.ENUM_MEMBER,
+                detail="Reserved Tag",
+                sort_text=f"080_{tag}",
+                insert_text_format=InsertTextFormat.PLAIN_TEXT,
+                text_edit=TextEdit(range=range, new_text=f"{tag}") if range is not None else None,
+            )
+            for tag in built_in_tags
+        ]
+
+    async def _complete_ForceTags_or_KeywordTags_or_DefaultTags_Tags(  # noqa: N802
+        self,
+        node: ast.AST,
+        nodes_at_position: List[ast.AST],
+        position: Position,
+        context: Optional[CompletionContext],
+    ) -> Union[List[CompletionItem], CompletionList, None]:
+        from robot.parsing.lexer.tokens import Token as RobotToken
+        from robot.parsing.model.statements import Statement
+
+        statement = cast(Statement, node)
+        tokens = get_tokens_at_position(statement, position)
+
+        if not tokens:
+            return None
+
+        if tokens[-1].type == RobotToken.ARGUMENT:
+            return await self.create_tags_completion_items(range_from_token(tokens[-1]))
+
+        if len(tokens) > 1 and tokens[-2].type == RobotToken.ARGUMENT:
+            return await self.create_tags_completion_items(range_from_token(tokens[-2]))
+
+        if whitespace_at_begin_of_token(tokens[-1]) >= 2:
+            return await self.create_tags_completion_items(None)
+
+        return None
+
+    async def complete_ForceTags(  # noqa: N802
+        self,
+        node: ast.AST,
+        nodes_at_position: List[ast.AST],
+        position: Position,
+        context: Optional[CompletionContext],
+    ) -> Union[List[CompletionItem], CompletionList, None]:
+        return await self._complete_ForceTags_or_KeywordTags_or_DefaultTags_Tags(
+            node, nodes_at_position, position, context
+        )
+
+    async def complete_KeywordTags(  # noqa: N802
+        self,
+        node: ast.AST,
+        nodes_at_position: List[ast.AST],
+        position: Position,
+        context: Optional[CompletionContext],
+    ) -> Union[List[CompletionItem], CompletionList, None]:
+        return await self._complete_ForceTags_or_KeywordTags_or_DefaultTags_Tags(
+            node, nodes_at_position, position, context
+        )
+
+    async def complete_DefaultTags(  # noqa: N802
+        self,
+        node: ast.AST,
+        nodes_at_position: List[ast.AST],
+        position: Position,
+        context: Optional[CompletionContext],
+    ) -> Union[List[CompletionItem], CompletionList, None]:
+        return await self._complete_ForceTags_or_KeywordTags_or_DefaultTags_Tags(
+            node, nodes_at_position, position, context
+        )
+
+    async def complete_Tags(  # noqa: N802
+        self,
+        node: ast.AST,
+        nodes_at_position: List[ast.AST],
+        position: Position,
+        context: Optional[CompletionContext],
+    ) -> Union[List[CompletionItem], CompletionList, None]:
+        return await self._complete_ForceTags_or_KeywordTags_or_DefaultTags_Tags(
+            node, nodes_at_position, position, context
+        )
```

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/diagnostics.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/document_highlight.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/document_symbols.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/documents_cache.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/documents_cache.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/folding_range.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/formatting.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/goto.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/goto.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/hover.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/inline_value.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/model_helper.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/model_helper.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/references.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/rename.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,19 @@
             if extension_config.configurations:
                 config.configure = set(extension_config.configurations)
 
             class MyRobocop(Robocop):
                 async def run_check(self, ast_model, filename, source=None):  # type: ignore
                     await check_canceled()
 
-                    if robocop_version >= (2, 4):
+                    if robocop_version >= (4, 0):
+                        from robocop.utils.disablers import DisablersFinder
+
+                        disablers = DisablersFinder(ast_model)
+                    elif robocop_version >= (2, 4):
                         from robocop.utils import DisablersFinder
 
                         disablers = DisablersFinder(filename=filename, source=source)
 
                     else:
                         self.register_disablers(filename, source)
                         disablers = self.disabler
```

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/selection_range.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/parts/signature_help.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/utils/_variables.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/utils/_variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/utils/ast_utils.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/utils/ast_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/utils/async_ast.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/utils/async_ast.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/utils/robot_path.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/utils/robot_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/src/robotcode/language_server/robotframework/utils/variables.py` & `robotcode_language_server-0.47.0/src/robotcode/language_server/robotframework/utils/variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/.gitignore` & `robotcode_language_server-0.47.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/LICENSE.txt` & `robotcode_language_server-0.47.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/README.md` & `robotcode_language_server-0.47.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.46.0/pyproject.toml` & `robotcode_language_server-0.47.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -23,16 +23,16 @@
   "Topic :: Utilities",
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-jsonrpc2==0.46.0",
-  "robotcode==0.46.0",
+  "robotcode-jsonrpc2==0.47.0",
+  "robotcode==0.47.0",
 ]
 dynamic = ["version"]
 
 [project.entry-points.robotcode]
 langserver = "robotcode.language_server.hooks"
 
 [project.urls]
```

### Comparing `robotcode_language_server-0.46.0/PKG-INFO` & `robotcode_language_server-0.47.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-language-server
-Version: 0.46.0
+Version: 0.47.0
 Summary: RobotCode Language Server for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,16 +21,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-jsonrpc2==0.46.0
-Requires-Dist: robotcode==0.46.0
+Requires-Dist: robotcode-jsonrpc2==0.47.0
+Requires-Dist: robotcode==0.47.0
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-language-server
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
```


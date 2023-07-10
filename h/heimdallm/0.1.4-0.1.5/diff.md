# Comparing `tmp/heimdallm-0.1.4.tar.gz` & `tmp/heimdallm-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heimdallm-0.1.4.tar", max compression
+gzip compressed data, was "heimdallm-0.1.5.tar", max compression
```

## Comparing `heimdallm-0.1.4.tar` & `heimdallm-0.1.5.tar`

### file list

```diff
@@ -1,33 +1,45 @@
--rw-r--r--   0        0        0      750 2023-07-05 13:16:58.063326 heimdallm-0.1.4/CONTRIBUTING.md
--rw-r--r--   0        0        0    34523 2023-07-05 13:16:58.063326 heimdallm-0.1.4/LICENSE
--rw-r--r--   0        0        0     6993 2023-07-05 13:16:58.063326 heimdallm-0.1.4/README.md
--rw-r--r--   0        0        0       81 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/__init__.py
--rw-r--r--   0        0        0     6498 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/bifrost.py
--rw-r--r--   0        0        0        0 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/bifrosts/sql/__init__.py
--rw-r--r--   0        0        0     6621 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/bifrosts/sql/exc.py
--rw-r--r--   0        0        0        0 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/bifrosts/sql/mysql/__init__.py
--rw-r--r--   0        0        0     3441 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/bifrosts/sql/mysql/presets.py
--rw-r--r--   0        0        0        0 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/bifrosts/sql/sqlite/__init__.py
--rw-r--r--   0        0        0     3707 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/bifrosts/sql/sqlite/presets.py
--rw-r--r--   0        0        0        0 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/bifrosts/sql/sqlite/select/__init__.py
--rw-r--r--   0        0        0     4693 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/bifrosts/sql/sqlite/select/bifrost.py
--rw-r--r--   0        0        0     4744 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/bifrosts/sql/sqlite/select/envelope.py
--rw-r--r--   0        0        0     1331 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/bifrosts/sql/sqlite/select/envelopes/base.j2
--rw-r--r--   0        0        0     4756 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/bifrosts/sql/sqlite/select/reconstruct.py
--rw-r--r--   0        0        0     6704 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/bifrosts/sql/sqlite/select/sqlite.lark
--rw-r--r--   0        0        0    11100 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/bifrosts/sql/sqlite/select/validator.py
--rw-r--r--   0        0        0    16112 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/bifrosts/sql/sqlite/select/visitors.py
--rw-r--r--   0        0        0        0 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/bifrosts/sql/sqlite/utils/__init__.py
--rw-r--r--   0        0        0      993 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/bifrosts/sql/sqlite/utils/identifier.py
--rw-r--r--   0        0        0     2716 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/bifrosts/sql/sqlite/utils/visitors.py
--rw-r--r--   0        0        0     5691 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/bifrosts/sql/utils.py
--rw-r--r--   0        0        0     1376 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/constraints.py
--rw-r--r--   0        0        0     1643 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/envelope.py
--rw-r--r--   0        0        0      734 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/llm.py
--rw-r--r--   0        0        0        0 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/llm_providers/__init__.py
--rw-r--r--   0        0        0      793 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/llm_providers/mock.py
--rw-r--r--   0        0        0     2399 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/llm_providers/openai.py
--rw-r--r--   0        0        0        0 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/support/__init__.py
--rw-r--r--   0        0        0     1051 2023-07-05 13:16:58.067326 heimdallm-0.1.4/heimdallm/support/github.py
--rw-r--r--   0        0        0     1564 2023-07-05 13:16:58.099327 heimdallm-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     8303 1970-01-01 00:00:00.000000 heimdallm-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      750 2023-07-10 01:19:55.056303 heimdallm-0.1.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0    34523 2023-07-10 01:19:55.056303 heimdallm-0.1.5/LICENSE
+-rw-r--r--   0        0        0     6958 2023-07-10 01:19:55.056303 heimdallm-0.1.5/README.md
+-rw-r--r--   0        0        0       81 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/__init__.py
+-rw-r--r--   0        0        0     6583 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrost.py
+-rw-r--r--   0        0        0        0 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/__init__.py
+-rw-r--r--   0        0        0     5293 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/bifrost.py
+-rw-r--r--   0        0        0     5688 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/common.py
+-rw-r--r--   0        0        0     6014 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/envelope.py
+-rw-r--r--   0        0        0     1234 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/envelopes/sql/mysql/select.j2
+-rw-r--r--   0        0        0     1331 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/envelopes/sql/sqlite/select.j2
+-rw-r--r--   0        0        0        0 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/envelopes/sql/test.j2
+-rw-r--r--   0        0        0     6668 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/exc.py
+-rw-r--r--   0        0        0        0 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/mysql/__init__.py
+-rw-r--r--   0        0        0    15919 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/mysql/presets.py
+-rw-r--r--   0        0        0        0 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/mysql/select/__init__.py
+-rw-r--r--   0        0        0     1545 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/mysql/select/bifrost.py
+-rw-r--r--   0        0        0      563 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/mysql/select/envelope.py
+-rw-r--r--   0        0        0     6391 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/mysql/select/grammar.lark
+-rw-r--r--   0        0        0      685 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/mysql/select/validator.py
+-rw-r--r--   0        0        0     5029 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/reconstruct.py
+-rw-r--r--   0        0        0        0 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/sqlite/__init__.py
+-rw-r--r--   0        0        0     3707 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/sqlite/presets.py
+-rw-r--r--   0        0        0        0 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/sqlite/select/__init__.py
+-rw-r--r--   0        0        0     1971 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/sqlite/select/bifrost.py
+-rw-r--r--   0        0        0      564 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/sqlite/select/envelope.py
+-rw-r--r--   0        0        0     6737 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/sqlite/select/grammar.lark
+-rw-r--r--   0        0        0      685 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/sqlite/select/validator.py
+-rw-r--r--   0        0        0        0 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/utils/__init__.py
+-rw-r--r--   0        0        0     1546 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/utils/identifier.py
+-rw-r--r--   0        0        0    11519 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/validator.py
+-rw-r--r--   0        0        0        0 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/visitors/__Init__.py
+-rw-r--r--   0        0        0     3005 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/visitors/aliases.py
+-rw-r--r--   0        0        0     2947 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/visitors/ambiguity.py
+-rw-r--r--   0        0        0    14153 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/bifrosts/sql/visitors/facets.py
+-rw-r--r--   0        0        0     1451 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/constraints.py
+-rw-r--r--   0        0        0     1643 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/envelope.py
+-rw-r--r--   0        0        0      734 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/llm.py
+-rw-r--r--   0        0        0        0 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/llm_providers/__init__.py
+-rw-r--r--   0        0        0      793 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/llm_providers/mock.py
+-rw-r--r--   0        0        0     2433 2023-07-10 01:19:55.060303 heimdallm-0.1.5/heimdallm/llm_providers/openai.py
+-rw-r--r--   0        0        0        0 2023-07-10 01:19:55.064303 heimdallm-0.1.5/heimdallm/support/__init__.py
+-rw-r--r--   0        0        0     1051 2023-07-10 01:19:55.064303 heimdallm-0.1.5/heimdallm/support/github.py
+-rw-r--r--   0        0        0     1621 2023-07-10 01:19:55.092303 heimdallm-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     8268 1970-01-01 00:00:00.000000 heimdallm-0.1.5/PKG-INFO
```

### Comparing `heimdallm-0.1.4/CONTRIBUTING.md` & `heimdallm-0.1.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.4/LICENSE` & `heimdallm-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.4/README.md` & `heimdallm-0.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # HeimdaLLM
 
 > Heimdall, the watchman of the gods, dwelt at its entrance, where he guarded Bifrost,
 > the shimmering path connecting the realms.
 
-[![Heimdall](https://raw.githubusercontent.com/amoffat/HeimdaLLM/main/docs/source/images/heimdall.png)](https://docs.heimdallm.ai)
+[![Heimdall](https://raw.githubusercontent.com/amoffat/HeimdaLLM/main/docs/source/images/heimdall.png)](https://heimdallm.ai)
 [![Build status](https://github.com/amoffat/HeimdaLLM/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/amoffat/HeimdaLLM/actions)
 [![Docs](https://img.shields.io/badge/Documentation-purple.svg)](https://docs.heimdallm.ai)
 [![GitHub Sponsors](https://img.shields.io/github/sponsors/amoffat)](https://github.com/sponsors/amoffat)
 [![PyPI](https://img.shields.io/pypi/v/heimdallm)](https://pypi.org/project/heimdallm/)
 [![License: Commercial](https://img.shields.io/badge/License-Commercial-blue.svg)](https://forms.gle/frEPeeJx81Cmwva78)
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 [![Coverage Status](https://coveralls.io/repos/github/amoffat/HeimdaLLM/badge.svg?branch=dev)](https://coveralls.io/github/amoffat/HeimdaLLM?branch=dev)
@@ -95,17 +95,19 @@
 
 To understand some of the potential vulnerabilities, take a look at the [attack
 surface](https://docs.heimdallm.ai/en/latest/attack_surface.html) to see the risks and
 the mitigations.
 
 # 📚 Database support
 
-Currently, sqlite's flavor of SQL is supported. There is active development for the
-other top relational SQL databases. To help me prioritize, please vote on which database
-you would like to see supported:
+- Sqlite
+- MySQL
+
+There is active development for the other top relational SQL databases. To help me
+prioritize, please vote on which database you would like to see supported:
 
 [![Static Badge](https://img.shields.io/badge/Vote!-here-limegreen)](https://github.com/amoffat/HeimdaLLM/discussions/2)
 
 # 📜 License
 
 HeimdaLLM is dual-licensed for open-source or for commercial use.
```

### Comparing `heimdallm-0.1.4/heimdallm/bifrost.py` & `heimdallm-0.1.5/heimdallm/bifrost.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from typing import Callable, Sequence
+from typing import TYPE_CHECKING, Callable, Sequence
 
 import structlog
 from lark import Lark, ParseTree
 
-from heimdallm.constraints import ConstraintValidator
-from heimdallm.envelope import PromptEnvelope
-from heimdallm.llm import LLMIntegration
+if TYPE_CHECKING:
+    import heimdallm.constraints
+    import heimdallm.envelope
+    from heimdallm.llm import LLMIntegration
 
 LOG = structlog.get_logger(__name__)
 
 
 class Bifrost:
     """The Bifrost is the bridge from the outside world to your secure systems. It is
     responsible for a rigorous parsing and validation of the output of the :term:`LLM`.
@@ -29,19 +30,19 @@
         to validate the parse tree returned by the ``tree_producer``. Only one validator
         needs to succeed for validation to pass.
     """
 
     def __init__(
         self,
         *,
-        llm: LLMIntegration,
-        prompt_envelope: PromptEnvelope,
+        llm: "LLMIntegration",
+        prompt_envelope: "heimdallm.envelope.PromptEnvelope",
         grammar: Lark,
         tree_producer: Callable[[Lark, str], ParseTree],
-        constraint_validators: Sequence[ConstraintValidator],
+        constraint_validators: Sequence["heimdallm.constraints.ConstraintValidator"],
     ):
         self.llm = llm
         self.prompt_envelope = prompt_envelope
         self.grammar = grammar
         self.tree_producer = tree_producer
         self.constraint_validators = constraint_validators
 
@@ -131,39 +132,39 @@
         log.info("Validation succeeded")
 
         return trusted_llm_output
 
     def _try_validator(
         self,
         log: structlog.BoundLogger,
-        validator: ConstraintValidator,
+        validator: "heimdallm.constraints.ConstraintValidator",
         autofix: bool,
-        untrusted_llm_input: str,
+        untrusted_llm_output: str,
         tree: ParseTree,
     ) -> str:
         """Attempt validation with an individual constraint validator."""
 
         if autofix:
             log.info("Autofixing parse tree and reconstructing the input")
             try:
-                untrusted_llm_output = validator.fix(self.grammar, tree)
+                untrusted_llm_output = validator.fix(self, self.grammar, tree)
             except Exception as e:
                 log.exception("Autofix failed")
                 raise e
             log.info("Re-parsing reconstructed output")
             try:
                 tree = self.parse(untrusted_llm_output)
             except Exception as e:
                 log.exception("Reparse failed")
                 raise e
             log.info("Reconstruction succeeded")
 
         # throws a bifrost-specific exception
         log.info("Validating parse tree")
-        validator.validate(untrusted_llm_input, tree)
+        validator.validate(self, untrusted_llm_output, tree)
         log.info("Validation succeeded")
 
         return untrusted_llm_output
 
     def parse(self, untrusted_llm_output: str) -> ParseTree:
         """Converts the :term:`LLM` output into a parse tree. Override it in a subclass
         to throw custom exceptions based on the grammar and parse state.
```

### Comparing `heimdallm-0.1.4/heimdallm/bifrosts/sql/exc.py` & `heimdallm-0.1.5/heimdallm/bifrosts/sql/exc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 import lark
 
 from heimdallm.support.github import make_ambiguous_parse_issue
 
-from .utils import FqColumn, JoinCondition, RequiredConstraint
+if TYPE_CHECKING:
+    from .common import FqColumn, JoinCondition, RequiredConstraint
 
 
 class BaseException(Exception):
     """This is a convenience base class for all HeimdaLLM SQL exceptions to them easier
     to catch.
 
     :meta private:
@@ -89,15 +90,15 @@
 
 class IllegalSelectedColumn(BaseException):
     """
     Thrown when a column is selected that is not allowed by the constraint validator and
     it was not automatically removed because :doc:`/reconstruction` is disabled.
 
     :param column: The column that was selected. This is not a :class:`FqColumn
-        <heimdallm.bifrosts.sql.utils.FqColumn>` because we may not always have a table
+        <heimdallm.bifrosts.sql.common.FqColumn>` because we may not always have a table
         name.
     """
 
     def __init__(self, *, column: str):
         message = f"Column `{column}` is not allowed in SELECT"
         super().__init__(message)
         self.column = column
@@ -107,43 +108,43 @@
     """
     Thrown when a column is used in a ``JOIN`` condition or a ``WHERE`` condition that
     is not allowed by the constraint validator.
 
     :param column: The column that was used in the condition.
     """
 
-    def __init__(self, *, column: FqColumn):
+    def __init__(self, *, column: "FqColumn"):
         message = f"Column `{column}` is not allowed in WHERE"
         super().__init__(message)
         self.column = column
 
 
 class MissingRequiredConstraint(BaseException):
-    def __init__(self, *, column: FqColumn, placeholder: str):
+    def __init__(self, *, column: "FqColumn", placeholder: str):
         message = f"Missing required constraint `{column}`=:{placeholder}"
         super().__init__(message)
         self.column = column
         self.placeholder = placeholder
 
 
 class MissingRequiredIdentity(BaseException):
-    def __init__(self, *, identities: set[RequiredConstraint]):
+    def __init__(self, *, identities: set["RequiredConstraint"]):
         message = f"Missing one required identities: {identities!r}"
         super().__init__(message)
         self.identities = identities
 
 
 class IllegalJoinTable(BaseException):
     """
     Thrown when a join spec is not allowed by the constraint validator.
 
     :param join: The join spec that was not allowed.
     """
 
-    def __init__(self, *, join: JoinCondition):
+    def __init__(self, *, join: "JoinCondition"):
         message = f"Join condition {join} is not allowed"
         super().__init__(message)
         self.join = join
 
 
 class IllegalJoinType(BaseException):
     """
```

### Comparing `heimdallm-0.1.4/heimdallm/bifrosts/sql/sqlite/presets.py` & `heimdallm-0.1.5/heimdallm/bifrosts/sql/sqlite/presets.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.4/heimdallm/bifrosts/sql/sqlite/select/bifrost.py` & `heimdallm-0.1.5/heimdallm/bifrosts/sql/bifrost.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,47 @@
-import sqlite3
-from pathlib import Path
-from typing import Callable, Sequence, Union
+from abc import ABC, abstractmethod
+from typing import TYPE_CHECKING, Callable, Sequence, Union
 
 import lark
 from lark import Lark, ParseTree
 from lark.exceptions import VisitError
 
-from heimdallm.bifrost import Bifrost
+from heimdallm.bifrost import Bifrost as _BaseBifrost
 from heimdallm.bifrosts.sql import exc
-from heimdallm.envelope import PromptEnvelope
 from heimdallm.llm import LLMIntegration
 from heimdallm.llm_providers.mock import EchoMockLLM
 
-from .envelope import TestSQLPromptEnvelope
-from .validator import SQLConstraintValidator
-from .visitors import AmbiguityResolver
+if TYPE_CHECKING:
+    import heimdallm.bifrosts.sql.envelope
+    import heimdallm.bifrosts.sql.validator
 
-_THIS_DIR = Path(__file__).parent
-_GRAMMAR_PATH = _THIS_DIR / "sqlite.lark"
+from .envelope import TestSQLPromptEnvelope
+from .visitors.ambiguity import AmbiguityResolver
 
 
-def _build_grammar() -> Lark:
+class Bifrost(_BaseBifrost, ABC):
     """
-    returns a limited sqlite SELECT grammar
+    An abstract Bifrost for traversing SQL ``SELECT`` queries. This is used by the
+    different SQL dialects.
 
-    noteworthy:
-        - no outer joins
-        - no subqueries
-
-    theoretically, subqueries could be allowed, but it would be more work, and
-    i'm not yet convinced that an LLM produces subqueries often enough to make
-    it worth it.
-
-    outer joins are unsafe because the join constraint is not applied to the
-    rows that would be considered "outer."
-    """
-    with open(_GRAMMAR_PATH, "r") as h:
-        grammar = Lark(
-            ambiguity="explicit",
-            maybe_placeholders=False,
-            grammar=h,
-        )
-    return grammar
-
-
-def _build_tree_producer() -> Callable[[Lark, str], ParseTree]:
-    def parse(grammar: Lark, untrusted_query: str) -> ParseTree:
-        ambig_tree = grammar.parse(untrusted_query)
-        try:
-            final_tree = AmbiguityResolver(untrusted_query).transform(ambig_tree)
-        except VisitError as e:
-            if isinstance(e.orig_exc, exc.BaseException):
-                raise e.orig_exc
-            raise e
-        return final_tree
-
-    return parse
-
-
-def get_schema(conn: sqlite3.Connection):
-    """a convenience function to get the schema of a sqlite database. you
-    probably want to write your own function to do this, one that doesn't
-    include tables and columns that you care about sending to the LLM"""
-    schema = []
-    for line in conn.iterdump():
-        if "CREATE TABLE" in line:
-            schema.append(line)
-    return "\n".join(schema)
-
-
-class SQLBifrost(Bifrost):
-    """A Bifrost for traversing SQL ``SELECT`` queries.
-
-    :vartype value: str
+    :param llm: The LLM integration to use.
+    :param prompt_envelope: The prompt envelope used to wrap the untrusted human input
+        and unwrap the untrusted LLM output.
+    :param constraint_validators: A sequence of constraint validators that will be used
+        to validate the parse tree returned by the ``tree_producer``. Only one validator
+        needs to succeed for validation to pass.
     """
 
     # for tests
     @classmethod
     def mocked(
         cls,
         constraint_validators: Union[
-            SQLConstraintValidator, Sequence[SQLConstraintValidator]
+            "heimdallm.bifrosts.sql.validator.ConstraintValidator",
+            Sequence["heimdallm.bifrosts.sql.validator.ConstraintValidator"],
         ],
     ):
         """A convenience method for our tests. This creates a Bifrost that assumes its
         untrusted input is a SQL query already, so it does not need to communicate with
         the LLM, only parse and validate it.
 
         :param constraint_validators: A constraint validator or sequence of constraint
@@ -106,31 +63,83 @@
             ),
         )
 
     def __init__(
         self,
         *,
         llm: LLMIntegration,
-        prompt_envelope: PromptEnvelope,
-        constraint_validators: Sequence[SQLConstraintValidator],
+        prompt_envelope: "heimdallm.bifrosts.sql.envelope.PromptEnvelope",
+        constraint_validators: Sequence[
+            "heimdallm.bifrosts.sql.validator.ConstraintValidator"
+        ],
     ):
         super().__init__(
             llm=llm,
             prompt_envelope=prompt_envelope,
-            grammar=_build_grammar(),
-            tree_producer=_build_tree_producer(),
+            grammar=self.build_grammar(),
+            tree_producer=self.build_tree_producer(),
             constraint_validators=constraint_validators,
         )
 
+    @classmethod
+    @abstractmethod
+    def reserved_keywords(cls) -> set[str]:
+        """
+        Returns the reserved keywords for the SQL dialect. Must be implemented in the
+        subclass.
+
+        :return: The reserved keywords.
+        :meta private:
+        """
+        raise NotImplementedError
+
+    @classmethod
+    def build_tree_producer(cls) -> Callable[[Lark, str], ParseTree]:
+        """
+        Produces a that can create a single parse tree. May be implemented in a subclass
+        if you want to do custom ambiguity resolution.
+
+        :return: The parse tree producer.
+        :meta private:
+        """
+
+        def parse(grammar: Lark, untrusted_query: str) -> ParseTree:
+            ambig_tree = grammar.parse(untrusted_query)
+            try:
+                final_tree = AmbiguityResolver(
+                    untrusted_query,
+                    cls.reserved_keywords(),
+                ).transform(ambig_tree)
+            except VisitError as e:
+                if isinstance(e.orig_exc, exc.BaseException):
+                    raise e.orig_exc
+                raise e
+            return final_tree
+
+        return parse
+
+    @staticmethod
+    @abstractmethod
+    def build_grammar() -> Lark:
+        """
+        Produces the grammar that will be used to parse the dialect of SQL. Must be
+        implemented in a subclass.
+
+        :return: The Lark grammar for the SQL dialect.
+        :meta private:
+        """
+        raise NotImplementedError
+
     def parse(self, untrusted_llm_output: str) -> ParseTree:
         """Parse the unwrapped SQL query from the LLM's output. Raise a SQL-specific
         exception if the query is not valid.
 
         :param untrusted_llm_output: The output from the LLM, which should be a SQL
-            query. If it isn't, then our :meth:`SQLPromptEnvelope.unwrap` method failed.
+            query. If it isn't, then our
+            :meth:`heimdallm.bifrosts.sql.envelope.PromptEnvelope.unwrap` method failed.
         :raises InvalidQuery: If the query is not valid.
         :return: The Lark parse tree for the query.
 
         :meta private:
         """
         try:
             return super().parse(untrusted_llm_output)
```

### Comparing `heimdallm-0.1.4/heimdallm/bifrosts/sql/sqlite/select/envelope.py` & `heimdallm-0.1.5/heimdallm/bifrosts/sql/envelope.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,67 @@
 import re
+from abc import abstractmethod
 from itertools import chain
 from pathlib import Path
-from typing import Sequence, cast
+from typing import TYPE_CHECKING, Sequence, cast
 
 import jinja2
 
-from heimdallm.envelope import PromptEnvelope as _PromptEnvelope
+from heimdallm.envelope import PromptEnvelope as _BasePromptEnvelope
 from heimdallm.llm import LLMIntegration
 
-from .validator import SQLConstraintValidator
+if TYPE_CHECKING:
+    import heimdallm.bifrosts.sql.validator
 
 THIS_DIR = Path(__file__).parent
 _TMPL_ENV = jinja2.Environment(
     loader=jinja2.FileSystemLoader(THIS_DIR / "envelopes"),
     undefined=jinja2.StrictUndefined,
 )
 
 
-class SQLPromptEnvelope(_PromptEnvelope):
+class PromptEnvelope(_BasePromptEnvelope):
     """The purpose of the prompt envelope is to wrap the untrusted input in additional
     context for the LLM to produce the correct output. We do not do validation in the
     envelope, because it is impossible to prevent prompt injection.
 
     While not necessary to subclass, you are recommended to do so if you want to
     customize the envelope.
 
     :param llm: The LLM integration being sent the human input. This can be used to
-        tweak the :meth:`wrap` and :meth`unwrap` methods to account for quirks of the
+        tweak the :meth:`wrap` and :meth:`unwrap` methods to account for quirks of the
         specific LLM.
     :param db_schema: The database schema of the database being queried. It is passed to
         the LLM so that the LLM knows how the tables and columns are connected.
     :param validators: The validators to use to validate the output of the LLM. They
         aren't used to validate here, but some of the validator's properties are added
         to the envelope to help guide the LLM to produce the correct output.
     """
 
     def __init__(
         self,
         *,
         llm: LLMIntegration,
         db_schema: str,
-        validators: Sequence[SQLConstraintValidator],
+        validators: Sequence["heimdallm.bifrosts.sql.validator.ConstraintValidator"],
     ):
         self.db_schema = db_schema
         self.validators = validators
         super().__init__(llm=llm)
 
+    @abstractmethod
     def template(self, env: jinja2.Environment) -> jinja2.Template:
         """
         Returns the template to use for the envelope. Override in a subclass for
         complete customization.
 
         :param env: The environment to use to load the template.
         :return: The template to use for the envelope.
         """
-        return env.get_template("base.j2")
+        raise NotImplementedError
 
     @property
     def params(self) -> dict:
         """Returns a dictionary of additional parameters to be passed to the template.
         Override in a subclass for complete control over values that you want in the
         envelope.
 
@@ -96,15 +99,15 @@
         # assume the LLM did what we said and delimited the output with ```
         if "```" in untrusted_llm_output:
             # sometimes the LLM is silly and likes to include the word "sql" inside
             # the delimiters. silly LLM!
             match = cast(
                 re.Match,
                 re.search(
-                    r"```(?:sql)?(.*)```",
+                    r"```(?:sql)?(.*?)```",
                     untrusted_llm_output,
                     flags=re.DOTALL | re.IGNORECASE,
                 ),
             )
             unpacked = match.group(1)
         # otherwise, just return the whole thing, and we'll attempt to parse it
         # as is
@@ -113,13 +116,39 @@
             # when instructed not to, oh well.
             unpacked = re.sub(r"^\s*sql\n+", "", untrusted_llm_output)
 
         unpacked = unpacked.strip()
         return unpacked
 
 
-class TestSQLPromptEnvelope(SQLPromptEnvelope):
+class TestSQLPromptEnvelope(PromptEnvelope):
+    """
+    A test envelope specifically for :meth:`Bifrost.mocked
+    <heimdallm.bifrosts.sql.bifrost.Bifrost.mocked>`
+
+    :param llm: The LLM integration being sent the human input. This can be used to
+        tweak the :meth:`wrap` and :meth:`unwrap() <PromptEnvelope.unwrap>` methods to
+        account for quirks of the specific LLM.
+    :param db_schema: The database schema of the database being queried. It is passed to
+        the LLM so that the LLM knows how the tables and columns are connected.
+    :param validators: The validators to use to validate the output of the LLM. They
+        aren't used to validate here, but some of the validator's properties are added
+        to the envelope to help guide the LLM to produce the correct output.
+
+    :meta private:
+    """
+
     def wrap(self, untrusted_input: str) -> str:
         # build the envelope, but don't actually use it. this exercises the
         # envelope code as part of a full integration
         super().wrap(untrusted_input)
         return untrusted_input
+
+    def template(self, env: jinja2.Environment) -> jinja2.Template:
+        """
+        Returns the template to use for the envelope. Override in a subclass for
+        complete customization.
+
+        :param env: The environment to use to load the template.
+        :return: The template to use for the envelope.
+        """
+        return env.get_template("sql/test.j2")
```

### Comparing `heimdallm-0.1.4/heimdallm/bifrosts/sql/sqlite/select/envelopes/base.j2` & `heimdallm-0.1.5/heimdallm/bifrosts/sql/envelopes/sql/sqlite/select.j2`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.4/heimdallm/bifrosts/sql/sqlite/select/reconstruct.py` & `heimdallm-0.1.5/heimdallm/bifrosts/sql/reconstruct.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import cast
 
 from lark import Discard, Token
 from lark import Transformer as _Transformer
 from lark import Tree
 
-from ... import exc
-from ...utils import FqColumn
-from ..utils.identifier import get_identifier
-from ..utils.visitors import AliasCollector
-from .validator import SQLConstraintValidator
+from . import exc
+from .common import FqColumn
+from .utils.identifier import get_identifier, is_count_function
+from .validator import ConstraintValidator
+from .visitors.aliases import AliasCollector
 
 
 def _build_limit_tree(limit, offset=None):
     children = [
         Token("LIMIT", "LIMIT"),
         Tree(
             "limit",
@@ -64,18 +64,19 @@
     constraints, but could with those alterations. currently, these are just the
     following:
 
         - adding or lowering a limit on the number of rows
         - removing illegal selected columns
     """
 
-    def __init__(self, validator: SQLConstraintValidator):
+    def __init__(self, validator: ConstraintValidator, reserved_keywords: set[str]):
         self._validator = validator
-        self._collector = AliasCollector()
-        self._last_discarded_column = None
+        self._collector = AliasCollector(reserved_keywords=reserved_keywords)
+        self._last_discarded_column: FqColumn | None = None
+        self._reserved_keywords = reserved_keywords
         super().__init__()
 
     def transform(self, tree):
         self._collector.visit(tree)
         return super().transform(tree)
 
     def select_statement(self, children):
@@ -97,23 +98,26 @@
         # if there's no children, it means we discarded every column selected, meaning
         # that they were all illegal columns. since we can't proceed without a column,
         # go ahead and raise an exception about illegal column.
         if not children:
             raise exc.IllegalSelectedColumn(column=self._last_discarded_column.name)
         return Tree("selected_columns", children)
 
-    def selected_column(self, children):
+    def selected_column(self, children: list[Tree | Token]):
         """ensures that every selected column is allowed"""
         selected = children[0]
-        if isinstance(selected, Tree):
+        if is_count_function(selected):
+            pass
+
+        elif isinstance(selected, Tree):
             for fq_column_node in selected.find_data("fq_column"):
                 table_node, column_node = fq_column_node.children
 
-                maybe_table_alias = get_identifier(table_node)
-                column_name = get_identifier(column_node)
+                maybe_table_alias = get_identifier(table_node, self._reserved_keywords)
+                column_name = get_identifier(column_node, self._reserved_keywords)
 
                 table_name = self._collector._aliased_tables.get(
                     maybe_table_alias, maybe_table_alias
                 )
                 column = FqColumn(table=table_name, column=column_name)
                 if not self._validator.select_column_allowed(column):
                     self._last_discarded_column = column
```

### Comparing `heimdallm-0.1.4/heimdallm/bifrosts/sql/sqlite/select/sqlite.lark` & `heimdallm-0.1.5/heimdallm/bifrosts/sql/sqlite/select/grammar.lark`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 // we use a placeholder for the limit clause because we need to be able to insert one
 // automatically in the case of reconstruction. if we didn't have a placeholder, we'd
 // have to examine ever clause child in `select_statement` to try to figure out where
 // to insert our new limit. having a placeholder simplifies this greatly.
 limit_placeholder : limit_clause?
 
 // serves as a basis for table and column names
+// NOTE this is dialect specific
 !quoted_identifier : "`" IDENTIFIER "`"
     | "\"" IDENTIFIER "\""
     | "[" IDENTIFIER "]"
 unquoted_identifier : IDENTIFIER
 IDENTIFIER : /[a-zA-Z_][a-zA-Z0-9_]*/
 
 selected_table : aliased_table | table_name
```

### Comparing `heimdallm-0.1.4/heimdallm/bifrosts/sql/sqlite/select/validator.py` & `heimdallm-0.1.5/heimdallm/bifrosts/sql/validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 from itertools import chain
 from typing import Optional, Sequence, cast
 
 from lark import Lark, ParseTree
 from lark.exceptions import VisitError
 from lark.reconstruct import Reconstructor
 
+from heimdallm.bifrost import Bifrost
 from heimdallm.bifrosts.sql import exc
-from heimdallm.constraints import ConstraintValidator as _ConstraintValidator
+from heimdallm.bifrosts.sql.bifrost import Bifrost as _SQLBifrost
+from heimdallm.constraints import ConstraintValidator as _BaseConstraintValidator
 
-from ...utils import ANY_JOIN, FqColumn, JoinCondition, RequiredConstraint
-from .. import presets
-from ..utils.visitors import AliasCollector
-from .visitors import FacetCollector, Facets
+from .common import ANY_JOIN, FqColumn, JoinCondition, RequiredConstraint
+from .visitors.aliases import AliasCollector
+from .visitors.facets import FacetCollector, Facets
 
 
-class SQLConstraintValidator(_ConstraintValidator):
+class ConstraintValidator(_BaseConstraintValidator):
     """
     This validator checks different of a SQL query. You are intended to derive this
     class and implement its methods."""
 
     @abstractmethod
     def requester_identities(self) -> Sequence[RequiredConstraint]:
         """Returns the possible identities of the requester, as represented in the
@@ -53,15 +54,15 @@
             JOIN inventory i ON f.film_id=i.film_id
             JOIN rental r
                 ON i.inventory_id=r.inventory_id
                 AND r.customer_id=:customer_id
 
         Both ``rental.customer_id`` and ``customer.customer_id`` are valid requester
         identities, so ou need to specify both of them by returning a
-        :class:`RequiredConstraint` for each of them.
+        :class:`heimdallm.bifrosts.sql.common.RequiredConstraint` for each of them.
 
         :return: The sequence of possible requester identities.
         """
         raise NotImplementedError(
             "You must explicitly provide the requester identity, "
             "or an empty list for full access (dangerous)"
         )
@@ -114,79 +115,89 @@
         the query will be reconstructed to include the correct limit.
 
         :return: The maximum number of rows that can be returned by a query, or None if
             unlimited.
         """
         return None
 
+    @abstractmethod
     def can_use_function(self, function: str) -> bool:
         """
         Returns whether or not a SQL function is allowed to be used anywhere in the
         query. By default, this checks the function against the list of safe functions
         that we have curated by hand.
 
         :param function: The *lowercase* name of the function.
         :return: Whether or not the function is allowed.
         """
-        return function in presets.safe_functions
+        raise NotImplementedError
 
     def condition_column_allowed(self, fq_column: FqColumn) -> bool:
         """
         Checks if a column is allowed to be used in a ``WHERE``, ``JOIN``, ``HAVING``,
         or ``ORDER BY``. By default, this calls :meth:`select_column_allowed`, but if
         you override this method and want to preserve that behavior, you should call
         yourself.
 
         :param fq_column: The fully-qualified column.
         :return: Whether or not the column is allowed to be used in a condition.
         """
         # let's default to "if you can see it, you can use it"
         return self.select_column_allowed(fq_column)
 
-    def fix(self, grammar: Lark, tree: ParseTree) -> str:
+    def fix(self, bifrost: Bifrost, grammar: Lark, tree: ParseTree) -> str:
         """A parse tree may be valid SQL, but it may not be valid according to
         the validator's constraints. we may be able to make intelligent
         decisions about those constraints, and fix the parse tree though, for
         example, by adding a limit to a query.
 
         :meta private:
         """
 
         # gets around a circular import issue
-        from heimdallm.bifrosts.sql.sqlite.select import reconstruct
+        from heimdallm.bifrosts.sql import reconstruct
 
-        transform = reconstruct.ReconstructTransformer(self)
+        transform = reconstruct.ReconstructTransformer(
+            self,
+            cast(_SQLBifrost, bifrost).reserved_keywords(),
+        )
         try:
             fixed_tree = transform.transform(tree)
         except VisitError as e:
             if isinstance(e.orig_exc, exc.BaseException):
                 raise e.orig_exc
             raise e
 
         output = Reconstructor(grammar).reconstruct(
             fixed_tree,
             postproc=reconstruct.postproc,
         )
         return output
 
-    def validate(self, untrusted_input: str, tree: ParseTree):
+    def validate(self, bifrost: Bifrost, untrusted_input: str, tree: ParseTree):
         """Analyze the parsed tree and validate it against our SQL constraints
 
         :param untrusted_input: The original query string. This is passed in so that if
             we need to raise an exception that references it, we can.
         :param tree: The parsed tree from the original query string.
 
         :meta private:
         """
         try:
-            alias_collector = AliasCollector()
+            alias_collector = AliasCollector(
+                cast(_SQLBifrost, bifrost).reserved_keywords()
+            )
             alias_collector.visit(tree)
 
             facets = Facets()
-            facet_collector = FacetCollector(facets, alias_collector)
+            facet_collector = FacetCollector(
+                facets,
+                alias_collector,
+                cast(_SQLBifrost, bifrost).reserved_keywords(),
+            )
             facet_collector.visit(tree)
         except exc.GeneralParseError:
             raise exc.InvalidQuery(query=untrusted_input)
 
         # check the select column allowlist
         for fq_column in facets.selected_columns:
             if not self.select_column_allowed(fq_column):
```

### Comparing `heimdallm-0.1.4/heimdallm/bifrosts/sql/sqlite/select/visitors.py` & `heimdallm-0.1.5/heimdallm/bifrosts/sql/visitors/facets.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from collections import defaultdict as dd
-from typing import MutableMapping, Optional
+from typing import MutableMapping, Optional, cast
 
-from lark import Token, Transformer, Tree, Visitor
+from lark import Token, Tree, Visitor
 
-from ... import exc
-from ...utils import FqColumn, JoinCondition, RequiredConstraint
-from ..utils.identifier import get_identifier
-from ..utils.visitors import AliasCollector
+from .. import exc
+from ..common import FqColumn, JoinCondition, RequiredConstraint
+from ..utils.identifier import get_identifier, is_count_function
+from .aliases import AliasCollector
 
 
 class Facets:
     """this simple class is used to collect all of the facets of a query, so
     that we can easily validate them with a constraint validator"""
 
     def __init__(self) -> None:
@@ -36,51 +36,57 @@
         self.limit: Optional[int] = None
 
 
 class FacetCollector(Visitor):
     """collects all of the facets of the query that we care about. this will
     feed directly into the constraint validator"""
 
-    def __init__(self, facets: Facets, collector: AliasCollector):
+    def __init__(
+        self,
+        facets: Facets,
+        collector: AliasCollector,
+        reserved_keywords: set[str],
+    ):
         self._collector = collector
         self._facets = facets
+        self._reserved_keywords = reserved_keywords
 
-    def _resolve_column(self, node):
+    def _resolve_column(self, node: Tree):
         if node.data == "column_alias":
-            maybe_alias = get_identifier(node)
+            maybe_alias = get_identifier(node, self._reserved_keywords)
             table, column = self._collector._aliased_columns.get(
                 maybe_alias, (None, maybe_alias)
             )
             return table, column
 
         # should never happen
         raise RuntimeError(f"unknown column reference type: {type(node)}")
 
-    def _resolve_table(self, table_ref):
+    def _resolve_table(self, table_ref: Tree | Token):
         if isinstance(table_ref, Tree):
             if table_ref.data == "aliased_table":
-                table_name = get_identifier(table_ref)
+                table_name = get_identifier(table_ref, self._reserved_keywords)
                 return table_name
 
             elif table_ref.data == "table_name":
                 # we have no way of knowing if this is an alias or not, other
                 # than testing for its existence in the collector's alias map
-                maybe_alias = get_identifier(table_ref)
+                maybe_alias = get_identifier(table_ref, self._reserved_keywords)
                 table = self._collector._aliased_tables.get(maybe_alias, maybe_alias)
                 return table
 
         elif isinstance(table_ref, Token):
             return table_ref.value
 
         # should never happen
         raise RuntimeError(f"unknown table reference type: {type(table_ref)}")
 
-    def join(self, node):
-        if join_type := list(node.find_data("illegal_join")):
-            join_type = join_type[0].children[0].type
+    def join(self, node: Tree):
+        if join_type_nodes := list(node.find_data("illegal_join")):
+            join_type = cast(Token, join_type_nodes[0].children[0]).type
             raise exc.IllegalJoinType(join_type=join_type)
 
         joined_table = node.children[1].children[0]
         joined_table_name = self._resolve_table(joined_table)
 
         # if a required_comparison node exists, it means it is actually required
         # (enforced by the grammar, see grammar comments). a required comparison has
@@ -89,15 +95,15 @@
             self._add_required_comparison(required_comparison)
 
         for condition in node.find_data("connecting_join_condition"):
             # from_table may be an alias, but from_column will always be authoritative.
             # the LHS of the join condition is always a fully-qualified column
             from_fq_column_node = condition.children[0]
             from_table_node, from_column_node = from_fq_column_node.children
-            from_column = get_identifier(from_column_node)
+            from_column = get_identifier(from_column_node, self._reserved_keywords)
             from_table = self._resolve_table(from_table_node)
 
             # conditions in a join are compared against are allowed conditions, so
             # record the LHS
             self._collect_condition_column(from_fq_column_node)
 
             # to_table may be an alias, but to_column will always be authoritative.
@@ -111,15 +117,15 @@
             elif (
                 isinstance(to_fq_column_node, Tree)
                 and to_fq_column_node.data != "fq_column"
             ):
                 continue
 
             to_table, to_column_node = to_fq_column_node.children
-            to_column = get_identifier(to_column_node)
+            to_column = get_identifier(to_column_node, self._reserved_keywords)
 
             to_table = self._resolve_table(to_table)
 
             # the joined table must be one of the parts of the join condition
             if joined_table_name != from_table and joined_table_name != to_table:
                 self._facets.bad_joins.append(joined_table_name)
                 continue
@@ -133,91 +139,99 @@
             join_spec = JoinCondition(
                 f"{from_table}.{from_column}",
                 f"{to_table}.{to_column}",
             )
             self._facets.joined_tables[from_table].add(join_spec)
             self._facets.joined_tables[to_table].add(join_spec)
 
-    def selected_table(self, node):
+    def selected_table(self, node: Tree):
         table_node = list(node.find_data("table_name"))[0]
-        table_name = get_identifier(table_node)
+        table_name = get_identifier(table_node, self._reserved_keywords)
         self._facets.selected_table = table_name
 
-    def selected_column(self, node):
+    def selected_column(self, node: Tree):
         child = node.children[0]
 
         if isinstance(child, Token) and child.type == "COUNT_STAR":
             return
 
         elif isinstance(child, Token) and child.type == "ALL_COLUMNS":
             raise exc.IllegalSelectedColumn(column="*")
 
+        # if we're aliasing COUNT(*), it's safe to ignore, since it doesn't
+        # reveal any of the underlying values
+        elif is_count_function(child):
+            return
+
         elif isinstance(child, Tree):
             # if it's an aliased column, we need to ensure that the thing being aliased
             # isn't a non-fully-qualified column. we do that by looking for
             # `column_alias`
             if child.data == "aliased_column":
                 alias_child = child.children[0]
                 # if we're aliasing COUNT(*), it's safe to ignore, since it doesn't
                 # reveal any of the underlying values
                 if isinstance(alias_child, Token) and alias_child.type == "COUNT_STAR":
                     return
 
                 if list(alias_child.find_data("column_alias")):
-                    alias = get_identifier(alias_child)
+                    alias = get_identifier(alias_child, self._reserved_keywords)
                     raise exc.UnqualifiedColumn(column=alias)
 
             # if the column looks like a column alias (meaning a non-fully-qualified
             # column), then that's an error, because we only work with fully-qualified
             # columns
             elif child.data == "column_alias":
-                alias = get_identifier(child)
+                alias = get_identifier(child, self._reserved_keywords)
                 raise exc.UnqualifiedColumn(column=alias)
 
             # if we're not an aliased column, but we contain a column alias somewhere,
             # that's an error, because we only work with fully-qualified columns
             elif column_alias := list(child.find_data("column_alias")):
-                alias = get_identifier(column_alias[0])
+                alias = get_identifier(column_alias[0], self._reserved_keywords)
                 raise exc.UnqualifiedColumn(column=alias)
 
             # if we've made it this far, we're sure we're dealing with a fully-qualified
             # column, or a non-column based expression
             try:
                 table_node = next(child.find_data("table_name"))
             # it's some non-column expression, which we don't care about
             except StopIteration:
                 pass
             # there's a fully qualified column there, so we'll record it
             else:
                 table_name = self._resolve_table(table_node)
                 # column_name will always be authoritative, even if it is aliased in
                 # this node
-                column_name = get_identifier(list(child.find_data("column_name"))[0])
+                column_name = get_identifier(
+                    list(child.find_data("column_name"))[0],
+                    self._reserved_keywords,
+                )
                 self._facets.selected_columns.add(
                     FqColumn(
                         table=table_name,
                         column=column_name,
                     )
                 )
 
-    def _add_required_comparison(self, node):
+    def _add_required_comparison(self, node: Tree):
         """takes a node representing a required comparison and adds it to the
         facets"""
         maybe_fq_column_node, placeholder = node.children
-        placeholder_name = placeholder.children[0].value
+        placeholder_name = cast(Token, placeholder.children[0]).value
 
         if maybe_fq_column_node.data == "column_alias":
             table_name, column_name = self._resolve_column(maybe_fq_column_node)
 
         elif maybe_fq_column_node.data == "fq_column":
             fq_column_node = maybe_fq_column_node
             table_node, column_node = fq_column_node.children
 
             table_name = self._resolve_table(table_node)
-            column_name = get_identifier(column_node)
+            column_name = get_identifier(column_node, self._reserved_keywords)
         else:
             raise RuntimeError(
                 f"Unknown required column type {type(maybe_fq_column_node)}"
             )
 
         self._facets.required_constraints.add(
             RequiredConstraint(
@@ -256,23 +270,23 @@
                     level_stack.append(child)
 
             for child in reversed(level_stack):
                 stack.append(child)
                 if child.data == "required_comparison":
                     self._add_required_comparison(child)
 
-    def _collect_condition_column(self, node):
+    def _collect_condition_column(self, node: Tree):
         """here we'll parse out the columns that are referenced anywhere in the
         WHERE, regardless of the depth of the expression. we care if a column is being
         referenced at all, even optionally, because that will be checked against the
         allowlist"""
         for fq_column_node in node.find_data("fq_column"):
             table_node, column_node = fq_column_node.children
             table_name = self._resolve_table(table_node)
-            column_name = get_identifier(column_node)
+            column_name = get_identifier(column_node, self._reserved_keywords)
             self._facets.condition_columns.add(
                 FqColumn(
                     table=table_name,
                     column=column_name,
                 )
             )
 
@@ -294,79 +308,12 @@
                 )
             )
 
     where_condition = _collect_condition_column
     having_condition = _collect_condition_column
     order_column = _collect_condition_column
 
-    def limit(self, node):
-        self._facets.limit = int(node.children[0].value)
-
-    def function_name(self, node):
-        self._facets.functions.add(node.children[0].value.lower())
-
+    def limit(self, node: Tree):
+        self._facets.limit = int(cast(Token, node.children[0]).value)
 
-class AmbiguityResolver(Transformer):
-    """this transformer's purpose is to resolve ambiguities in the parse tree
-    that can only be resolved through some extra knowledge that would be
-    difficult to embed in the grammar itself.
-    """
-
-    def __init__(self, query: str):
-        self.query = query
-        super().__init__()
-
-    def test_alias(self, i, tree, trees) -> bool:
-        """
-        This resolves ambiguities in the parse tree related to aliases. For
-        example, the following query is ambiguous:
-
-            select t1.secret from t1 left join t2 on t1.jid = t2.jid
-
-        Is "left" an alias for "t1", or is it part of the "left join"? It's
-        ambiguous. We know it's not ambiguous because "left" is a keyword, but
-        the parser can't know this. This class resolves those ambiguities by
-        looking at all possible ambiguous parse trees in the ambiguity, and
-        selecting only the one that does not have an alias conflict with a
-        reserved keyword.
-        """
-        for alias_node in tree.find_data("generic_alias"):
-            try:
-                get_identifier(alias_node)
-            except exc.ReservedKeyword:
-                return False
-        return True
-
-    def test_req_comparisons(self, i, tree, trees) -> bool:
-        """in a where_condition rule, the children can include
-        `relational_comparison` and `required_comparison` rules, which are
-        ambiguous, because required comparisons are a subset of relational
-        comparisons. we always prefer to interpret the ambiguity as a required
-        comparison though, because it is more strict, and it satisfies our
-        required comparison validator constraints"""
-        if tree.data in ("where_condition", "join_condition"):
-            return tree.children[0].data == "required_comparison"
-        return True
-
-    def test_arith_expr(self, i, tree, trees) -> bool:
-        """the arith_expr node is recursive, so it can be ambiguous. just choose the
-        first parse of it, since this node doesn't really matter"""
-        if tree.data == "arith_expr":
-            return i == 0
-        return True
-
-    def _ambig(self, trees):
-        def test_tree(i, tree):
-            return (
-                self.test_alias(i, tree, trees)
-                and self.test_req_comparisons(i, tree, trees)
-                and self.test_arith_expr(i, tree, trees)
-            )
-
-        pruned_trees = [tree for i, tree in enumerate(trees) if test_tree(i, tree)]
-
-        if len(pruned_trees) == 0:
-            raise exc.InvalidQuery(query=self.query)
-        elif len(pruned_trees) == 1:
-            return pruned_trees[0]
-        else:
-            raise exc.AmbiguousParse(trees=pruned_trees, query=self.query)
+    def function_name(self, node: Tree):
+        self._facets.functions.add(cast(Token, node.children[0]).value.lower())
```

### Comparing `heimdallm-0.1.4/heimdallm/bifrosts/sql/sqlite/utils/visitors.py` & `heimdallm-0.1.5/heimdallm/bifrosts/sql/visitors/aliases.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,61 @@
-from lark import Token, Visitor
+from lark import Token, Tree, Visitor
 
-from .identifier import get_identifier
+from ..utils.identifier import get_identifier
 
 
 class AliasCollector(Visitor):
     """collects all of our table and column aliases and maps them back to the
     authoritative name. we have to do this pass first, before any other passes,
     because the tree may not evaluate in the order that would allow us to
     resolve aliases."""
 
-    def __init__(self):
+    def __init__(self, reserved_keywords: set[str]):
         # aliased table names from the FROM clause, as well as JOIN clauses.
         # they map from the alias name to the table name.
-        self._aliased_tables = {}
+        self._aliased_tables: dict[str, str] = {}
         # aliased column names from the SELECT clause. they map from the alias
         # name to the (table, column) tuple
-        self._aliased_columns = {}
+        self._aliased_columns: dict[str, tuple[str | None, str | None]] = {}
+        self._reserved_keywords = reserved_keywords
 
     def _resolve_table(self, table):
         return self._aliased_tables.get(table, table)
 
     # tables are aliased in the FROM clause of a SELECT statement, or when a
     # table is JOINed. it's here that we know the authoritative table name and
     # its aliased, which may be used in other parts of the query
-    def aliased_table(self, node):
+    def aliased_table(self, node: Tree):
         table_node, _as, alias_node = node.children
-        table_name = get_identifier(table_node)
-        alias = get_identifier(alias_node)
+        table_name = get_identifier(table_node, self._reserved_keywords)
+        alias = get_identifier(alias_node, self._reserved_keywords)
         self._aliased_tables[alias] = table_name
 
         # inefficient, but backfill the correct table alias for any columns
         for key, (tn, cn) in list(self._aliased_columns.items()):
             if tn == alias:
                 self._aliased_columns[key] = (table_name, cn)
 
     # columns are aliased in the column list of a SELECT statement. we assume
     # that all aliased columns are fully qualified by table name. note, however,
     # that the table name may be an alias itself.
-    def aliased_column(self, node):
+    def aliased_column(self, node: Tree):
         value_node, _as, alias_node = node.children
-        alias_name = get_identifier(alias_node)
+        alias_name = get_identifier(alias_node, self._reserved_keywords)
 
         if isinstance(value_node, Token):
             if value_node.type == "COUNT_STAR":
                 self._aliased_columns[alias_name] = (None, None)
             return
 
         # there may be multiple columns referenced in this alias column, for
         # example if we're running a function on multiple columns and aliasing
         # the result. so we need to look at each fq_column individually
         for fq_column_node in value_node.find_data("fq_column"):
             table_node, column_node = fq_column_node.children
-            table_name = get_identifier(table_node)
-            column_name = get_identifier(column_node)
+            table_name = get_identifier(table_node, self._reserved_keywords)
+            column_name = get_identifier(column_node, self._reserved_keywords)
 
             # do we already have a table alias for this column? use that instead for
             # the table name
             table_name = self._resolve_table(table_name)
             self._aliased_columns[alias_name] = (table_name, column_name)
```

### Comparing `heimdallm-0.1.4/heimdallm/bifrosts/sql/utils.py` & `heimdallm-0.1.5/heimdallm/bifrosts/sql/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     the fully-qualified columns does not matter; matching will work correctly in the
     code.
 
     :param first: The first fully-qualified column.
     :param second: The second fully-qualified column.
     :param identity: If the columns specified in this join condition can also be used as
         a :meth:`requester identity
-        <heimdallm.bifrosts.sql.sqlite.select.validator.SQLConstraintValidator.requester_identities>`
+        <heimdallm.bifrosts.sql.sqlite.select.validator.ConstraintValidator.requester_identities>`
         for the query, then this should be set to the name of the placeholder where the
         identity will be populated at runtime.
     """
 
     __slots__ = ("first", "second", "identity_placeholder")
 
     def __init__(self, first: str, second: str, *, identity: Optional[str] = None):
```

### Comparing `heimdallm-0.1.4/heimdallm/constraints.py` & `heimdallm-0.1.5/heimdallm/constraints.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from abc import ABC, abstractmethod
 
 from lark import Lark, ParseTree
 
+from heimdallm.bifrost import Bifrost
+
 
 class ConstraintValidator(ABC):
     """This is the base class for all constraint validators. It is used to validate
     the parse tree of the untrusted input, and to fix the parse tree if it fails a
     soft-validation pass."""
 
     @abstractmethod
-    def fix(self, grammar: Lark, tree: ParseTree) -> str:
+    def fix(self, bifrost: Bifrost, grammar: Lark, tree: ParseTree) -> str:
         """If the tree fails validation in a soft-pass, attempt to reconstruct it
         to satisfy the constraints. If the tree cannot be reconstructed, throw a
         Bifrost-specific exception
 
         :param grammar: The Lark grammar used to parse the untrusted input. This is
             often used by :class:`lark.reconstruct.Reconstructor` to fix the parse tree.
         :param tree: The resulting parse tree of the untrusted input.
         """
         raise NotImplementedError
 
     @abstractmethod
-    def validate(self, untrusted_input: str, tree: ParseTree):
+    def validate(self, biforst: Bifrost, untrusted_input: str, tree: ParseTree):
         """This performs the Bifrost-specific validation of the parse tree. It throws a
         Bifrost-specific exception if the tree does not pass the constraints.
 
         :param untrusted_input: The untrusted input, which can be used to provide extra
             context if we need to raise an exception.
         :param tree: The resulting parse tree of the untrusted input.
         """
```

### Comparing `heimdallm-0.1.4/heimdallm/envelope.py` & `heimdallm-0.1.5/heimdallm/envelope.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.4/heimdallm/llm.py` & `heimdallm-0.1.5/heimdallm/llm.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.4/heimdallm/llm_providers/mock.py` & `heimdallm-0.1.5/heimdallm/llm_providers/mock.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.4/heimdallm/llm_providers/openai.py` & `heimdallm-0.1.5/heimdallm/llm_providers/openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,15 @@
             ],
         )
         untrusted_llm_output = chat_completion.choices[0].message.content
         return untrusted_llm_output
 
     def _complete_via_completion(self, prompt):
         response = openai.Completion.create(
+            api_key=self.api_key,
             engine=self.model,
             prompt=prompt,
             max_tokens=256,
             n=1,
             stop=None,
             temperature=0.7,
         )
```

### Comparing `heimdallm-0.1.4/heimdallm/support/github.py` & `heimdallm-0.1.5/heimdallm/support/github.py`

 * *Files identical despite different names*

### Comparing `heimdallm-0.1.4/pyproject.toml` & `heimdallm-0.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "heimdallm"
-version = "0.1.4"
+version = "0.1.5"
 description = "Construct trusted SQL queries from untrusted input"
 homepage = "https://github.com/amoffat/HeimdaLLM"
 repository = "https://github.com/amoffat/HeimdaLLM"
 documentation = "https://heimdallm.readthedocs.io/en/latest/"
 authors = ["Andrew Moffat <arwmoffat@gmail.com>"]
 maintainers = ["Andrew Moffat <arwmoffat@gmail.com>"]
 keywords = ["sql", "llm", "ai"]
@@ -49,11 +49,13 @@
 flake8 = "^6.0.0"
 ipykernel = "^6.23.3"
 sphinx = ">=1.6,<7"
 sphinx-rtd-theme = "^1.2.2"
 toml = "^0.10.2"
 types-toml = "^0.10.8.6"
 munch = "^4.0.0"
+mysql-connector-python = "^8.0.33"
+pre-commit = "^3.3.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `heimdallm-0.1.4/PKG-INFO` & `heimdallm-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heimdallm
-Version: 0.1.4
+Version: 0.1.5
 Summary: Construct trusted SQL queries from untrusted input
 Home-page: https://github.com/amoffat/HeimdaLLM
 License: AGPL-3.0
 Keywords: sql,llm,ai
 Author: Andrew Moffat
 Author-email: arwmoffat@gmail.com
 Maintainer: Andrew Moffat
@@ -30,15 +30,15 @@
 Description-Content-Type: text/markdown
 
 # HeimdaLLM
 
 > Heimdall, the watchman of the gods, dwelt at its entrance, where he guarded Bifrost,
 > the shimmering path connecting the realms.
 
-[![Heimdall](https://raw.githubusercontent.com/amoffat/HeimdaLLM/main/docs/source/images/heimdall.png)](https://docs.heimdallm.ai)
+[![Heimdall](https://raw.githubusercontent.com/amoffat/HeimdaLLM/main/docs/source/images/heimdall.png)](https://heimdallm.ai)
 [![Build status](https://github.com/amoffat/HeimdaLLM/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/amoffat/HeimdaLLM/actions)
 [![Docs](https://img.shields.io/badge/Documentation-purple.svg)](https://docs.heimdallm.ai)
 [![GitHub Sponsors](https://img.shields.io/github/sponsors/amoffat)](https://github.com/sponsors/amoffat)
 [![PyPI](https://img.shields.io/pypi/v/heimdallm)](https://pypi.org/project/heimdallm/)
 [![License: Commercial](https://img.shields.io/badge/License-Commercial-blue.svg)](https://forms.gle/frEPeeJx81Cmwva78)
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
 [![Coverage Status](https://coveralls.io/repos/github/amoffat/HeimdaLLM/badge.svg?branch=dev)](https://coveralls.io/github/amoffat/HeimdaLLM?branch=dev)
@@ -126,17 +126,19 @@
 
 To understand some of the potential vulnerabilities, take a look at the [attack
 surface](https://docs.heimdallm.ai/en/latest/attack_surface.html) to see the risks and
 the mitigations.
 
 # 📚 Database support
 
-Currently, sqlite's flavor of SQL is supported. There is active development for the
-other top relational SQL databases. To help me prioritize, please vote on which database
-you would like to see supported:
+- Sqlite
+- MySQL
+
+There is active development for the other top relational SQL databases. To help me
+prioritize, please vote on which database you would like to see supported:
 
 [![Static Badge](https://img.shields.io/badge/Vote!-here-limegreen)](https://github.com/amoffat/HeimdaLLM/discussions/2)
 
 # 📜 License
 
 HeimdaLLM is dual-licensed for open-source or for commercial use.
```

